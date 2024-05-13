# Comparing `tmp/danielutils-0.9.82.tar.gz` & `tmp/danielutils-0.9.83.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "danielutils-0.9.82.tar", last modified: Wed May  1 18:25:52 2024, max compression
+gzip compressed data, was "danielutils-0.9.83.tar", last modified: Wed May  1 23:01:55 2024, max compression
```

## Comparing `danielutils-0.9.82.tar` & `danielutils-0.9.83.tar`

### file list

```diff
@@ -1,229 +1,231 @@
-drwxrwxrwx   0        0        0        0 2024-05-01 18:25:52.847260 danielutils-0.9.82/
--rw-rw-rw-   0        0        0     1091 2023-05-29 13:19:53.000000 danielutils-0.9.82/LICENSE
--rw-rw-rw-   0        0        0       34 2024-05-01 18:25:51.000000 danielutils-0.9.82/MANIFEST.in
--rw-rw-rw-   0        0        0     4593 2024-05-01 18:25:52.847260 danielutils-0.9.82/PKG-INFO
--rw-rw-rw-   0        0        0     2650 2024-05-01 18:25:24.000000 danielutils-0.9.82/README.md
-drwxrwxrwx   0        0        0        0 2024-05-01 18:25:52.746371 danielutils-0.9.82/danielutils/
--rw-rw-rw-   0        0        0     1399 2024-05-01 12:22:07.000000 danielutils-0.9.82/danielutils/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-01 18:25:52.749687 danielutils-0.9.82/danielutils/abstractions/
--rw-rw-rw-   0        0        0       77 2024-04-21 19:46:54.000000 danielutils-0.9.82/danielutils/abstractions/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-01 18:25:52.752687 danielutils-0.9.82/danielutils/abstractions/database/
--rw-rw-rw-   0        0        0       57 2024-04-21 18:12:14.000000 danielutils-0.9.82/danielutils/abstractions/database/__init__.py
--rw-rw-rw-   0        0        0     2772 2024-04-17 20:37:10.000000 danielutils-0.9.82/danielutils/abstractions/database/cached_database.py
--rw-rw-rw-   0        0        0     2621 2024-04-28 08:07:23.000000 danielutils-0.9.82/danielutils/abstractions/database/database.py
--rw-rw-rw-   0        0        0     1048 2024-04-25 20:10:37.000000 danielutils-0.9.82/danielutils/abstractions/database/redis_database.py
-drwxrwxrwx   0        0        0        0 2024-05-01 18:25:52.754735 danielutils-0.9.82/danielutils/abstractions/multiprogramming/
--rw-rw-rw-   0        0        0       74 2024-04-21 19:21:56.000000 danielutils-0.9.82/danielutils/abstractions/multiprogramming/__init__.py
--rw-rw-rw-   0        0        0      374 2024-04-17 20:37:10.000000 danielutils-0.9.82/danielutils/abstractions/multiprogramming/multi_id.py
--rw-rw-rw-   0        0        0     2392 2024-04-28 08:12:35.000000 danielutils-0.9.82/danielutils/abstractions/multiprogramming/worker.py
--rw-rw-rw-   0        0        0     2412 2024-04-28 08:12:35.000000 danielutils-0.9.82/danielutils/abstractions/multiprogramming/worker_pool.py
--rw-rw-rw-   0        0        0     3144 2024-04-28 08:12:35.000000 danielutils-0.9.82/danielutils/abstractions/repl.py
--rw-rw-rw-   0        0        0     5663 2024-03-21 20:59:13.000000 danielutils-0.9.82/danielutils/aliases.py
-drwxrwxrwx   0        0        0        0 2024-05-01 18:25:52.756779 danielutils-0.9.82/danielutils/better_builtins/
--rw-rw-rw-   0        0        0       78 2024-04-21 18:23:39.000000 danielutils-0.9.82/danielutils/better_builtins/__init__.py
--rw-rw-rw-   0        0        0     1221 2024-03-21 20:59:13.000000 danielutils-0.9.82/danielutils/better_builtins/counter.py
--rw-rw-rw-   0        0        0     7174 2024-04-21 18:12:40.000000 danielutils-0.9.82/danielutils/better_builtins/frange.py
-drwxrwxrwx   0        0        0        0 2024-05-01 18:25:52.760106 danielutils-0.9.82/danielutils/better_builtins/typed_builtins/
--rw-rw-rw-   0        0        0       88 2024-03-21 20:59:13.000000 danielutils-0.9.82/danielutils/better_builtins/typed_builtins/__init__.py
--rw-rw-rw-   0        0        0     4704 2024-04-28 08:12:35.000000 danielutils-0.9.82/danielutils/better_builtins/typed_builtins/factory.py
--rw-rw-rw-   0        0        0      913 2024-03-21 20:59:13.000000 danielutils-0.9.82/danielutils/better_builtins/typed_builtins/tdict.py
--rw-rw-rw-   0        0        0     7210 2024-04-28 08:12:13.000000 danielutils-0.9.82/danielutils/better_builtins/typed_builtins/tlist.py
--rw-rw-rw-   0        0        0     2031 2024-03-21 20:59:13.000000 danielutils-0.9.82/danielutils/better_builtins/typed_builtins/tset.py
--rw-rw-rw-   0        0        0      294 2024-03-21 20:59:13.000000 danielutils-0.9.82/danielutils/better_builtins/typed_builtins/ttuple.py
--rw-rw-rw-   0        0        0     5472 2024-04-28 08:19:09.000000 danielutils-0.9.82/danielutils/colors.py
-drwxrwxrwx   0        0        0        0 2024-05-01 18:25:52.762321 danielutils-0.9.82/danielutils/context_managers/
--rw-rw-rw-   0        0        0       58 2024-05-01 15:20:06.000000 danielutils-0.9.82/danielutils/context_managers/__init__.py
--rw-rw-rw-   0        0        0      874 2024-05-01 15:31:36.000000 danielutils-0.9.82/danielutils/context_managers/attr_context.py
--rw-rw-rw-   0        0        0     1122 2024-05-01 17:13:09.000000 danielutils-0.9.82/danielutils/context_managers/temporary_file.py
--rw-rw-rw-   0        0        0      210 2024-03-21 20:59:13.000000 danielutils-0.9.82/danielutils/convenience.py
-drwxrwxrwx   0        0        0        0 2024-05-01 18:25:52.763322 danielutils-0.9.82/danielutils/conversions/
--rw-rw-rw-   0        0        0       73 2024-03-21 20:59:13.000000 danielutils-0.9.82/danielutils/conversions/__init__.py
--rw-rw-rw-   0        0        0     2362 2024-04-28 08:19:08.000000 danielutils-0.9.82/danielutils/conversions/main_conversions.py
-drwxrwxrwx   0        0        0        0 2024-05-01 18:25:52.766157 danielutils-0.9.82/danielutils/conversions/specialized_conversions/
--rw-rw-rw-   0        0        0       46 2024-03-21 20:59:13.000000 danielutils-0.9.82/danielutils/conversions/specialized_conversions/__init__.py
--rw-rw-rw-   0        0        0      507 2024-03-21 23:16:41.000000 danielutils-0.9.82/danielutils/conversions/specialized_conversions/to_hex.py
--rw-rw-rw-   0        0        0      543 2024-04-28 08:12:13.000000 danielutils-0.9.82/danielutils/conversions/specialized_conversions/to_int.py
-drwxrwxrwx   0        0        0        0 2024-05-01 18:25:52.769163 danielutils-0.9.82/danielutils/data_structures/
--rw-rw-rw-   0        0        0      163 2024-04-17 20:37:10.000000 danielutils-0.9.82/danielutils/data_structures/__init__.py
--rw-rw-rw-   0        0        0     1224 2024-04-17 20:37:10.000000 danielutils-0.9.82/danielutils/data_structures/comparer.py
--rw-rw-rw-   0        0        0      273 2024-04-17 20:37:10.000000 danielutils-0.9.82/danielutils/data_structures/default_dict.py
--rw-rw-rw-   0        0        0      632 2023-09-25 13:19:42.000000 danielutils-0.9.82/danielutils/data_structures/functions.py
-drwxrwxrwx   0        0        0        0 2024-05-01 18:25:52.772080 danielutils-0.9.82/danielutils/data_structures/graph/
--rw-rw-rw-   0        0        0       97 2024-04-17 20:37:10.000000 danielutils-0.9.82/danielutils/data_structures/graph/__init__.py
--rw-rw-rw-   0        0        0     2066 2024-04-18 18:33:41.000000 danielutils-0.9.82/danielutils/data_structures/graph/binary_node.py
--rw-rw-rw-   0        0        0     6877 2024-04-28 08:12:24.000000 danielutils-0.9.82/danielutils/data_structures/graph/graph.py
--rw-rw-rw-   0        0        0     3141 2024-04-28 08:12:13.000000 danielutils-0.9.82/danielutils/data_structures/graph/multinode.py
--rw-rw-rw-   0        0        0     1647 2024-03-28 19:42:06.000000 danielutils-0.9.82/danielutils/data_structures/graph/node.py
-drwxrwxrwx   0        0        0        0 2024-05-01 18:25:52.774085 danielutils-0.9.82/danielutils/data_structures/heap/
--rw-rw-rw-   0        0        0       71 2024-03-28 19:45:24.000000 danielutils-0.9.82/danielutils/data_structures/heap/__init__.py
--rw-rw-rw-   0        0        0     3092 2024-04-17 20:37:10.000000 danielutils-0.9.82/danielutils/data_structures/heap/heap.py
--rw-rw-rw-   0        0        0      292 2024-03-28 19:45:24.000000 danielutils-0.9.82/danielutils/data_structures/heap/max_heap.py
--rw-rw-rw-   0        0        0      300 2024-03-28 19:45:24.000000 danielutils-0.9.82/danielutils/data_structures/heap/min_heap.py
-drwxrwxrwx   0        0        0        0 2024-05-01 18:25:52.777494 danielutils-0.9.82/danielutils/data_structures/queue/
--rw-rw-rw-   0        0        0       82 2024-03-28 19:35:07.000000 danielutils-0.9.82/danielutils/data_structures/queue/__init__.py
--rw-rw-rw-   0        0        0      260 2024-03-28 19:35:13.000000 danielutils-0.9.82/danielutils/data_structures/queue/atomic_queue.py
--rw-rw-rw-   0        0        0     3661 2024-03-28 19:35:07.000000 danielutils-0.9.82/danielutils/data_structures/queue/priority_queue.py
--rw-rw-rw-   0        0        0     1615 2024-04-28 08:12:13.000000 danielutils-0.9.82/danielutils/data_structures/queue/queue.py
--rw-rw-rw-   0        0        0     2143 2024-04-17 20:37:10.000000 danielutils-0.9.82/danielutils/data_structures/stack.py
-drwxrwxrwx   0        0        0        0 2024-05-01 18:25:52.779493 danielutils-0.9.82/danielutils/data_structures/trees/
--rw-rw-rw-   0        0        0       63 2024-04-17 20:37:10.000000 danielutils-0.9.82/danielutils/data_structures/trees/__init__.py
--rw-rw-rw-   0        0        0     2636 2024-04-28 08:12:00.000000 danielutils-0.9.82/danielutils/data_structures/trees/binary_syntax_tree.py
--rw-rw-rw-   0        0        0     1618 2024-04-18 18:33:41.000000 danielutils-0.9.82/danielutils/data_structures/trees/binary_tree.py
--rw-rw-rw-   0        0        0      675 2024-04-28 08:19:08.000000 danielutils-0.9.82/danielutils/date.py
--rw-rw-rw-   0        0        0      232 2023-08-07 20:06:13.000000 danielutils-0.9.82/danielutils/date_time.py
-drwxrwxrwx   0        0        0        0 2024-05-01 18:25:52.790493 danielutils-0.9.82/danielutils/decorators/
--rw-rw-rw-   0        0        0      466 2024-04-25 20:44:13.000000 danielutils-0.9.82/danielutils/decorators/__init__.py
--rw-rw-rw-   0        0        0      756 2024-04-28 08:19:08.000000 danielutils-0.9.82/danielutils/decorators/atomic.py
--rw-rw-rw-   0        0        0     1385 2024-04-28 08:19:08.000000 danielutils-0.9.82/danielutils/decorators/attach.py
--rw-rw-rw-   0        0        0      730 2024-03-21 20:59:13.000000 danielutils-0.9.82/danielutils/decorators/chain_decorators.py
--rw-rw-rw-   0        0        0     1089 2024-04-28 08:19:08.000000 danielutils-0.9.82/danielutils/decorators/decorate_conditionally.py
--rw-rw-rw-   0        0        0     1008 2024-04-27 18:49:37.000000 danielutils-0.9.82/danielutils/decorators/delay_call.py
--rw-rw-rw-   0        0        0     1290 2024-04-27 18:48:35.000000 danielutils-0.9.82/danielutils/decorators/deprecate.py
--rw-rw-rw-   0        0        0     1023 2024-04-25 20:44:13.000000 danielutils-0.9.82/danielutils/decorators/final.py
--rw-rw-rw-   0        0        0     1696 2024-04-28 08:19:08.000000 danielutils-0.9.82/danielutils/decorators/limit_recursion.py
--rw-rw-rw-   0        0        0      806 2024-04-28 08:19:08.000000 danielutils-0.9.82/danielutils/decorators/memo.py
--rw-rw-rw-   0        0        0     7521 2024-04-28 08:13:16.000000 danielutils-0.9.82/danielutils/decorators/overload.py
--rw-rw-rw-   0        0        0      837 2024-04-28 08:19:09.000000 danielutils-0.9.82/danielutils/decorators/partially_implemented.py
--rw-rw-rw-   0        0        0     1716 2024-04-21 19:46:04.000000 danielutils-0.9.82/danielutils/decorators/processify.py
--rw-rw-rw-   0        0        0     1095 2024-03-21 20:59:13.000000 danielutils-0.9.82/danielutils/decorators/property.py
--rw-rw-rw-   0        0        0      776 2024-04-17 20:37:10.000000 danielutils-0.9.82/danielutils/decorators/singleton.py
--rw-rw-rw-   0        0        0      729 2024-05-01 18:07:01.000000 danielutils-0.9.82/danielutils/decorators/threadify.py
--rw-rw-rw-   0        0        0     1998 2024-04-28 08:19:08.000000 danielutils-0.9.82/danielutils/decorators/timeout.py
--rw-rw-rw-   0        0        0     3746 2024-04-28 08:13:33.000000 danielutils-0.9.82/danielutils/decorators/total_ordering.py
--rw-rw-rw-   0        0        0     9556 2024-04-28 08:19:08.000000 danielutils-0.9.82/danielutils/decorators/validate.py
--rw-rw-rw-   0        0        0     2163 2024-03-21 20:59:13.000000 danielutils-0.9.82/danielutils/exceptions.py
-drwxrwxrwx   0        0        0        0 2024-05-01 18:25:52.795450 danielutils-0.9.82/danielutils/functions/
--rw-rw-rw-   0        0        0      235 2024-04-21 19:19:56.000000 danielutils-0.9.82/danielutils/functions/__init__.py
--rw-rw-rw-   0        0        0     1085 2024-04-28 08:12:35.000000 danielutils-0.9.82/danielutils/functions/areoneof.py
--rw-rw-rw-   0        0        0      638 2024-03-21 20:59:13.000000 danielutils-0.9.82/danielutils/functions/check_foreach.py
--rw-rw-rw-   0        0        0      791 2024-04-21 19:19:56.000000 danielutils-0.9.82/danielutils/functions/flatten.py
--rw-rw-rw-   0        0        0    10122 2024-04-28 08:10:10.000000 danielutils-0.9.82/danielutils/functions/isoftype.py
--rw-rw-rw-   0        0        0     1582 2024-04-28 08:12:35.000000 danielutils-0.9.82/danielutils/functions/isoneof.py
--rw-rw-rw-   0        0        0     1292 2024-04-28 08:07:23.000000 danielutils-0.9.82/danielutils/functions/multiloop.py
--rw-rw-rw-   0        0        0      639 2024-03-21 20:59:13.000000 danielutils-0.9.82/danielutils/functions/powerset.py
--rw-rw-rw-   0        0        0      288 2024-03-21 20:59:13.000000 danielutils-0.9.82/danielutils/functions/subseteq.py
--rw-rw-rw-   0        0        0     1008 2024-04-28 08:12:24.000000 danielutils-0.9.82/danielutils/functions/types_subseteq.py
-drwxrwxrwx   0        0        0        0 2024-05-01 18:25:52.797974 danielutils-0.9.82/danielutils/generators/
--rw-rw-rw-   0        0        0      108 2024-03-21 20:59:13.000000 danielutils-0.9.82/danielutils/generators/__init__.py
--rw-rw-rw-   0        0        0     1285 2024-03-21 20:59:13.000000 danielutils-0.9.82/danielutils/generators/conditional_generator.py
--rw-rw-rw-   0        0        0      478 2024-04-28 08:19:09.000000 danielutils-0.9.82/danielutils/generators/generator_from_stream.py
--rw-rw-rw-   0        0        0     2859 2024-04-28 08:12:35.000000 danielutils-0.9.82/danielutils/generators/join_generators.py
--rw-rw-rw-   0        0        0     2105 2024-04-28 08:19:08.000000 danielutils-0.9.82/danielutils/internet.py
--rw-rw-rw-   0        0        0    12329 2024-04-28 08:19:14.000000 danielutils-0.9.82/danielutils/io_.py
-drwxrwxrwx   0        0        0        0 2024-05-01 18:25:52.800980 danielutils-0.9.82/danielutils/math_/
--rw-rw-rw-   0        0        0       79 2024-04-21 18:05:24.000000 danielutils-0.9.82/danielutils/math_/__init__.py
--rw-rw-rw-   0        0        0     7682 2024-03-21 20:59:13.000000 danielutils-0.9.82/danielutils/math_/constants.py
--rw-rw-rw-   0        0        0      642 2024-04-28 08:19:09.000000 danielutils-0.9.82/danielutils/math_/functions.py
--rw-rw-rw-   0        0        0     1063 2024-04-21 18:05:24.000000 danielutils-0.9.82/danielutils/math_/math_print.py
--rw-rw-rw-   0        0        0     4044 2024-04-28 08:12:00.000000 danielutils-0.9.82/danielutils/math_/math_symbols.py
-drwxrwxrwx   0        0        0        0 2024-05-01 18:25:52.801980 danielutils-0.9.82/danielutils/math_/polynomial/
--rw-rw-rw-   0        0        0       25 2024-04-21 18:05:24.000000 danielutils-0.9.82/danielutils/math_/polynomial/__init__.py
--rw-rw-rw-   0        0        0      835 2024-04-28 08:12:13.000000 danielutils-0.9.82/danielutils/math_/polynomial/polinomial.py
-drwxrwxrwx   0        0        0        0 2024-05-01 18:25:52.807022 danielutils-0.9.82/danielutils/metaclasses/
--rw-rw-rw-   0        0        0      169 2024-03-21 23:16:41.000000 danielutils-0.9.82/danielutils/metaclasses/__init__.py
--rw-rw-rw-   0        0        0      695 2024-03-21 20:59:13.000000 danielutils-0.9.82/danielutils/metaclasses/atomic_class_meta.py
--rw-rw-rw-   0        0        0     2511 2024-03-21 20:59:13.000000 danielutils-0.9.82/danielutils/metaclasses/implicit_data_deleter_meta.py
--rw-rw-rw-   0        0        0     1495 2024-04-21 18:13:57.000000 danielutils-0.9.82/danielutils/metaclasses/instance_cache_meta.py
--rw-rw-rw-   0        0        0    10932 2024-04-28 08:12:24.000000 danielutils-0.9.82/danielutils/metaclasses/interface.py
--rw-rw-rw-   0        0        0     1754 2024-03-21 20:59:13.000000 danielutils-0.9.82/danielutils/metaclasses/overload_meta.py
-drwxrwxrwx   0        0        0        0 2024-05-01 18:25:52.808022 danielutils-0.9.82/danielutils/mock_/
--rw-rw-rw-   0        0        0       58 2024-04-21 18:12:14.000000 danielutils-0.9.82/danielutils/mock_/__init__.py
--rw-rw-rw-   0        0        0     2017 2024-04-21 19:46:04.000000 danielutils-0.9.82/danielutils/mock_/mock_database.py
--rw-rw-rw-   0        0        0      419 2024-04-17 20:37:10.000000 danielutils-0.9.82/danielutils/mock_/mock_module.py
--rw-rw-rw-   0        0        0     1032 2024-03-21 20:59:13.000000 danielutils-0.9.82/danielutils/path.py
--rw-rw-rw-   0        0        0     2801 2024-04-21 18:05:24.000000 danielutils-0.9.82/danielutils/print_.py
-drwxrwxrwx   0        0        0        0 2024-05-01 18:25:52.810066 danielutils-0.9.82/danielutils/protocols/
--rw-rw-rw-   0        0        0       49 2024-04-17 20:37:10.000000 danielutils-0.9.82/danielutils/protocols/__init__.py
--rw-rw-rw-   0        0        0      446 2024-04-28 08:12:00.000000 danielutils-0.9.82/danielutils/protocols/dictable.py
--rw-rw-rw-   0        0        0      203 2024-04-17 20:37:10.000000 danielutils-0.9.82/danielutils/protocols/evaluable.py
--rw-rw-rw-   0        0        0        0 2023-08-09 09:08:58.000000 danielutils-0.9.82/danielutils/py.typed
-drwxrwxrwx   0        0        0        0 2024-05-01 18:25:52.811065 danielutils-0.9.82/danielutils/reflection/
--rw-rw-rw-   0        0        0     1516 2024-04-21 18:21:37.000000 danielutils-0.9.82/danielutils/reflection/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-01 18:25:52.812063 danielutils-0.9.82/danielutils/reflection/class_/
--rw-rw-rw-   0        0        0       31 2024-04-21 18:21:37.000000 danielutils-0.9.82/danielutils/reflection/class_/__init__.py
--rw-rw-rw-   0        0        0     5507 2024-04-28 08:12:35.000000 danielutils-0.9.82/danielutils/reflection/class_/class_reflection.py
-drwxrwxrwx   0        0        0        0 2024-05-01 18:25:52.813064 danielutils-0.9.82/danielutils/reflection/file/
--rw-rw-rw-   0        0        0       30 2024-04-21 18:21:37.000000 danielutils-0.9.82/danielutils/reflection/file/__init__.py
--rw-rw-rw-   0        0        0     1657 2024-04-27 18:35:37.000000 danielutils-0.9.82/danielutils/reflection/file/file_reflection.py
-drwxrwxrwx   0        0        0        0 2024-05-01 18:25:52.814102 danielutils-0.9.82/danielutils/reflection/function/
--rw-rw-rw-   0        0        0       35 2024-04-21 18:21:37.000000 danielutils-0.9.82/danielutils/reflection/function/__init__.py
--rw-rw-rw-   0        0        0     4453 2024-04-28 08:12:24.000000 danielutils-0.9.82/danielutils/reflection/function/function_reflections.py
-drwxrwxrwx   0        0        0        0 2024-05-01 18:25:52.819103 danielutils-0.9.82/danielutils/reflection/interpreter/
--rw-rw-rw-   0        0        0      179 2024-04-21 19:19:56.000000 danielutils-0.9.82/danielutils/reflection/interpreter/__init__.py
--rw-rw-rw-   0        0        0     1074 2024-04-25 20:37:30.000000 danielutils-0.9.82/danielutils/reflection/interpreter/callstack.py
--rw-rw-rw-   0        0        0      441 2024-04-28 08:12:13.000000 danielutils-0.9.82/danielutils/reflection/interpreter/get_traceback.py
--rw-rw-rw-   0        0        0      622 2024-04-17 20:37:10.000000 danielutils-0.9.82/danielutils/reflection/interpreter/os_.py
--rw-rw-rw-   0        0        0     1023 2024-04-17 20:37:10.000000 danielutils-0.9.82/danielutils/reflection/interpreter/packages.py
--rw-rw-rw-   0        0        0      621 2024-04-28 08:12:35.000000 danielutils-0.9.82/danielutils/reflection/interpreter/python_version.py
--rw-rw-rw-   0        0        0      489 2024-03-21 20:59:13.000000 danielutils-0.9.82/danielutils/reflection/interpreter/signals.py
--rw-rw-rw-   0        0        0     5733 2024-04-28 08:12:24.000000 danielutils-0.9.82/danielutils/reflection/interpreter/tracer.py
-drwxrwxrwx   0        0        0        0 2024-05-01 18:25:52.821103 danielutils-0.9.82/danielutils/reflection/module/
--rw-rw-rw-   0        0        0       68 2024-04-21 18:27:13.000000 danielutils-0.9.82/danielutils/reflection/module/__init__.py
--rw-rw-rw-   0        0        0      507 2024-03-21 20:59:13.000000 danielutils-0.9.82/danielutils/reflection/module/module_reflections.py
--rw-rw-rw-   0        0        0     4714 2024-04-28 08:12:24.000000 danielutils-0.9.82/danielutils/reflection/module/package_reflection.py
-drwxrwxrwx   0        0        0        0 2024-05-01 18:25:52.822103 danielutils-0.9.82/danielutils/snippets/
--rw-rw-rw-   0        0        0       24 2024-03-21 20:59:13.000000 danielutils-0.9.82/danielutils/snippets/__init__.py
--rw-rw-rw-   0        0        0      433 2024-03-21 20:59:13.000000 danielutils-0.9.82/danielutils/snippets/try_get.py
-drwxrwxrwx   0        0        0        0 2024-05-01 18:25:52.824103 danielutils-0.9.82/danielutils/system/
--rw-rw-rw-   0        0        0       84 2024-05-01 12:22:07.000000 danielutils-0.9.82/danielutils/system/__init__.py
--rw-rw-rw-   0        0        0     6863 2024-04-28 08:19:08.000000 danielutils-0.9.82/danielutils/system/independent.py
--rw-rw-rw-   0        0        0     4790 2024-05-01 17:51:36.000000 danielutils-0.9.82/danielutils/system/layered_command.py
-drwxrwxrwx   0        0        0        0 2024-05-01 18:25:52.826103 danielutils-0.9.82/danielutils/system/windows/
--rw-rw-rw-   0        0        0       50 2024-03-21 20:59:13.000000 danielutils-0.9.82/danielutils/system/windows/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-01 18:25:52.827103 danielutils-0.9.82/danielutils/system/windows/utils/
--rw-rw-rw-   0        0        0       25 2024-03-21 20:59:13.000000 danielutils-0.9.82/danielutils/system/windows/utils/__init__.py
--rw-rw-rw-   0        0        0      499 2024-04-17 20:37:10.000000 danielutils-0.9.82/danielutils/system/windows/utils/filetime.py
--rw-rw-rw-   0        0        0     6064 2024-03-21 20:59:13.000000 danielutils-0.9.82/danielutils/system/windows/win32_ctime.py
--rw-rw-rw-   0        0        0     2253 2024-03-21 20:59:13.000000 danielutils-0.9.82/danielutils/system/windows/windows.py
--rw-rw-rw-   0        0        0     4213 2024-04-28 08:19:08.000000 danielutils-0.9.82/danielutils/text.py
--rw-rw-rw-   0        0        0     1225 2024-04-27 18:53:17.000000 danielutils-0.9.82/danielutils/time.py
--rw-rw-rw-   0        0        0     1723 2024-04-28 08:12:13.000000 danielutils-0.9.82/danielutils/tqdm_.py
-drwxrwxrwx   0        0        0        0 2024-05-01 18:25:52.827103 danielutils-0.9.82/danielutils/university/
--rw-rw-rw-   0        0        0       74 2024-04-17 20:37:10.000000 danielutils-0.9.82/danielutils/university/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-01 18:25:52.829103 danielutils-0.9.82/danielutils/university/databases/
--rw-rw-rw-   0        0        0       20 2024-03-21 20:59:13.000000 danielutils-0.9.82/danielutils/university/databases/__init__.py
--rw-rw-rw-   0        0        0    24890 2024-04-28 08:12:35.000000 danielutils-0.9.82/danielutils/university/databases/all.py
-drwxrwxrwx   0        0        0        0 2024-05-01 18:25:52.830103 danielutils-0.9.82/danielutils/university/oop/
--rw-rw-rw-   0        0        0       25 2024-04-17 20:37:10.000000 danielutils-0.9.82/danielutils/university/oop/__init__.py
--rw-rw-rw-   0        0        0      802 2024-04-28 08:13:50.000000 danielutils-0.9.82/danielutils/university/oop/observer.py
--rw-rw-rw-   0        0        0       87 2024-04-17 20:37:10.000000 danielutils-0.9.82/danielutils/university/oop/strategy.py
-drwxrwxrwx   0        0        0        0 2024-05-01 18:25:52.834104 danielutils-0.9.82/danielutils/university/probability/
--rw-rw-rw-   0        0        0      189 2024-04-21 22:41:40.000000 danielutils-0.9.82/danielutils/university/probability/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-01 18:25:52.836254 danielutils-0.9.82/danielutils/university/probability/conditional_variable/
--rw-rw-rw-   0        0        0       89 2024-04-17 20:37:10.000000 danielutils-0.9.82/danielutils/university/probability/conditional_variable/__init__.py
--rw-rw-rw-   0        0        0     4004 2024-04-25 21:21:07.000000 danielutils-0.9.82/danielutils/university/probability/conditional_variable/conditional_variable.py
-drwxrwxrwx   0        0        0        0 2024-05-01 18:25:52.836254 danielutils-0.9.82/danielutils/university/probability/conditional_variable/continuous/
--rw-rw-rw-   0        0        0        0 2024-04-17 20:37:10.000000 danielutils-0.9.82/danielutils/university/probability/conditional_variable/continuous/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-01 18:25:52.841260 danielutils-0.9.82/danielutils/university/probability/conditional_variable/discrete/
--rw-rw-rw-   0        0        0      209 2024-04-17 20:37:10.000000 danielutils-0.9.82/danielutils/university/probability/conditional_variable/discrete/__init__.py
--rw-rw-rw-   0        0        0     1149 2024-04-21 22:51:43.000000 danielutils-0.9.82/danielutils/university/probability/conditional_variable/discrete/bernoulli.py
--rw-rw-rw-   0        0        0     1257 2024-04-21 22:51:43.000000 danielutils-0.9.82/danielutils/university/probability/conditional_variable/discrete/binomial.py
--rw-rw-rw-   0        0        0     1108 2024-04-21 22:51:43.000000 danielutils-0.9.82/danielutils/university/probability/conditional_variable/discrete/conditional_from_discrete_probability_func.py
--rw-rw-rw-   0        0        0     1370 2024-04-21 22:51:43.000000 danielutils-0.9.82/danielutils/university/probability/conditional_variable/discrete/discrete.py
--rw-rw-rw-   0        0        0     1652 2024-04-28 08:12:35.000000 danielutils-0.9.82/danielutils/university/probability/conditional_variable/discrete/geometric.py
--rw-rw-rw-   0        0        0      992 2024-04-21 22:51:43.000000 danielutils-0.9.82/danielutils/university/probability/conditional_variable/discrete/poisson.py
--rw-rw-rw-   0        0        0     1040 2024-04-21 22:51:43.000000 danielutils-0.9.82/danielutils/university/probability/conditional_variable/discrete/uniform.py
--rw-rw-rw-   0        0        0      904 2024-04-21 22:41:40.000000 danielutils-0.9.82/danielutils/university/probability/distributions.py
-drwxrwxrwx   0        0        0        0 2024-05-01 18:25:52.843260 danielutils-0.9.82/danielutils/university/probability/expressions/
--rw-rw-rw-   0        0        0       79 2024-04-17 22:49:00.000000 danielutils-0.9.82/danielutils/university/probability/expressions/__init__.py
--rw-rw-rw-   0        0        0     7439 2024-04-25 21:20:42.000000 danielutils-0.9.82/danielutils/university/probability/expressions/accumulation_expression.py
--rw-rw-rw-   0        0        0     4391 2024-04-25 21:20:53.000000 danielutils-0.9.82/danielutils/university/probability/expressions/probability_expression.py
-drwxrwxrwx   0        0        0        0 2024-05-01 18:25:52.846260 danielutils-0.9.82/danielutils/university/probability/funcs/
--rw-rw-rw-   0        0        0      120 2024-04-17 20:37:10.000000 danielutils-0.9.82/danielutils/university/probability/funcs/__init__.py
--rw-rw-rw-   0        0        0      338 2024-04-21 22:41:40.000000 danielutils-0.9.82/danielutils/university/probability/funcs/covariance.py
--rw-rw-rw-   0        0        0     1173 2024-04-21 22:41:40.000000 danielutils-0.9.82/danielutils/university/probability/funcs/expected_value.py
--rw-rw-rw-   0        0        0      306 2024-04-17 20:37:10.000000 danielutils-0.9.82/danielutils/university/probability/funcs/probability_function.py
--rw-rw-rw-   0        0        0      437 2024-04-21 22:41:40.000000 danielutils-0.9.82/danielutils/university/probability/funcs/variance.py
--rw-rw-rw-   0        0        0     1987 2024-04-28 08:12:24.000000 danielutils-0.9.82/danielutils/university/probability/operator.py
--rw-rw-rw-   0        0        0      641 2024-04-18 18:33:41.000000 danielutils-0.9.82/danielutils/university/probability/protocols.py
--rw-rw-rw-   0        0        0     2055 2024-04-21 22:51:43.000000 danielutils-0.9.82/danielutils/university/probability/supp.py
--rw-rw-rw-   0        0        0     1182 2024-04-25 20:08:45.000000 danielutils-0.9.82/danielutils/university/probability/transformation.py
--rw-rw-rw-   0        0        0      322 2024-04-28 08:07:53.000000 danielutils-0.9.82/danielutils/versioned_imports.py
-drwxrwxrwx   0        0        0        0 2024-05-01 18:25:52.748689 danielutils-0.9.82/danielutils.egg-info/
--rw-rw-rw-   0        0        0     4593 2024-05-01 18:25:52.000000 danielutils-0.9.82/danielutils.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     7860 2024-05-01 18:25:52.000000 danielutils-0.9.82/danielutils.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-01 18:25:52.000000 danielutils-0.9.82/danielutils.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       12 2024-05-01 18:25:52.000000 danielutils-0.9.82/danielutils.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      977 2024-05-01 18:25:51.000000 danielutils-0.9.82/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-05-01 18:25:52.847260 danielutils-0.9.82/setup.cfg
--rw-rw-rw-   0        0        0       41 2024-05-01 18:25:51.000000 danielutils-0.9.82/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-01 23:01:55.369031 danielutils-0.9.83/
+-rw-rw-rw-   0        0        0     1091 2023-05-29 13:19:53.000000 danielutils-0.9.83/LICENSE
+-rw-rw-rw-   0        0        0       34 2024-05-01 23:01:54.000000 danielutils-0.9.83/MANIFEST.in
+-rw-rw-rw-   0        0        0     4593 2024-05-01 23:01:55.368036 danielutils-0.9.83/PKG-INFO
+-rw-rw-rw-   0        0        0     2650 2024-05-01 23:01:26.000000 danielutils-0.9.83/README.md
+drwxrwxrwx   0        0        0        0 2024-05-01 23:01:55.268561 danielutils-0.9.83/danielutils/
+-rw-rw-rw-   0        0        0     1404 2024-05-01 22:07:57.000000 danielutils-0.9.83/danielutils/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-01 23:01:55.271562 danielutils-0.9.83/danielutils/abstractions/
+-rw-rw-rw-   0        0        0       77 2024-04-21 19:46:54.000000 danielutils-0.9.83/danielutils/abstractions/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-01 23:01:55.273918 danielutils-0.9.83/danielutils/abstractions/database/
+-rw-rw-rw-   0        0        0       57 2024-04-21 18:12:14.000000 danielutils-0.9.83/danielutils/abstractions/database/__init__.py
+-rw-rw-rw-   0        0        0     2772 2024-04-17 20:37:10.000000 danielutils-0.9.83/danielutils/abstractions/database/cached_database.py
+-rw-rw-rw-   0        0        0     2621 2024-04-28 08:07:23.000000 danielutils-0.9.83/danielutils/abstractions/database/database.py
+-rw-rw-rw-   0        0        0     1048 2024-04-25 20:10:37.000000 danielutils-0.9.83/danielutils/abstractions/database/redis_database.py
+drwxrwxrwx   0        0        0        0 2024-05-01 23:01:55.276925 danielutils-0.9.83/danielutils/abstractions/multiprogramming/
+-rw-rw-rw-   0        0        0       74 2024-04-21 19:21:56.000000 danielutils-0.9.83/danielutils/abstractions/multiprogramming/__init__.py
+-rw-rw-rw-   0        0        0      374 2024-04-17 20:37:10.000000 danielutils-0.9.83/danielutils/abstractions/multiprogramming/multi_id.py
+-rw-rw-rw-   0        0        0     2392 2024-04-28 08:12:35.000000 danielutils-0.9.83/danielutils/abstractions/multiprogramming/worker.py
+-rw-rw-rw-   0        0        0     2412 2024-04-28 08:12:35.000000 danielutils-0.9.83/danielutils/abstractions/multiprogramming/worker_pool.py
+-rw-rw-rw-   0        0        0     3144 2024-04-28 08:12:35.000000 danielutils-0.9.83/danielutils/abstractions/repl.py
+-rw-rw-rw-   0        0        0     5663 2024-03-21 20:59:13.000000 danielutils-0.9.83/danielutils/aliases.py
+drwxrwxrwx   0        0        0        0 2024-05-01 23:01:55.277971 danielutils-0.9.83/danielutils/better_builtins/
+-rw-rw-rw-   0        0        0       78 2024-04-21 18:23:39.000000 danielutils-0.9.83/danielutils/better_builtins/__init__.py
+-rw-rw-rw-   0        0        0     1221 2024-03-21 20:59:13.000000 danielutils-0.9.83/danielutils/better_builtins/counter.py
+-rw-rw-rw-   0        0        0     7174 2024-04-21 18:12:40.000000 danielutils-0.9.83/danielutils/better_builtins/frange.py
+drwxrwxrwx   0        0        0        0 2024-05-01 23:01:55.281969 danielutils-0.9.83/danielutils/better_builtins/typed_builtins/
+-rw-rw-rw-   0        0        0       88 2024-03-21 20:59:13.000000 danielutils-0.9.83/danielutils/better_builtins/typed_builtins/__init__.py
+-rw-rw-rw-   0        0        0     4704 2024-04-28 08:12:35.000000 danielutils-0.9.83/danielutils/better_builtins/typed_builtins/factory.py
+-rw-rw-rw-   0        0        0      913 2024-03-21 20:59:13.000000 danielutils-0.9.83/danielutils/better_builtins/typed_builtins/tdict.py
+-rw-rw-rw-   0        0        0     7210 2024-04-28 08:12:13.000000 danielutils-0.9.83/danielutils/better_builtins/typed_builtins/tlist.py
+-rw-rw-rw-   0        0        0     2031 2024-03-21 20:59:13.000000 danielutils-0.9.83/danielutils/better_builtins/typed_builtins/tset.py
+-rw-rw-rw-   0        0        0      294 2024-03-21 20:59:13.000000 danielutils-0.9.83/danielutils/better_builtins/typed_builtins/ttuple.py
+-rw-rw-rw-   0        0        0     5472 2024-04-28 08:19:09.000000 danielutils-0.9.83/danielutils/colors.py
+drwxrwxrwx   0        0        0        0 2024-05-01 23:01:55.284004 danielutils-0.9.83/danielutils/context_managers/
+-rw-rw-rw-   0        0        0       58 2024-05-01 15:20:06.000000 danielutils-0.9.83/danielutils/context_managers/__init__.py
+-rw-rw-rw-   0        0        0      874 2024-05-01 15:31:36.000000 danielutils-0.9.83/danielutils/context_managers/attr_context.py
+-rw-rw-rw-   0        0        0     1122 2024-05-01 17:13:09.000000 danielutils-0.9.83/danielutils/context_managers/temporary_file.py
+-rw-rw-rw-   0        0        0      210 2024-03-21 20:59:13.000000 danielutils-0.9.83/danielutils/convenience.py
+drwxrwxrwx   0        0        0        0 2024-05-01 23:01:55.285004 danielutils-0.9.83/danielutils/conversions/
+-rw-rw-rw-   0        0        0       73 2024-03-21 20:59:13.000000 danielutils-0.9.83/danielutils/conversions/__init__.py
+-rw-rw-rw-   0        0        0     2362 2024-04-28 08:19:08.000000 danielutils-0.9.83/danielutils/conversions/main_conversions.py
+drwxrwxrwx   0        0        0        0 2024-05-01 23:01:55.287004 danielutils-0.9.83/danielutils/conversions/specialized_conversions/
+-rw-rw-rw-   0        0        0       46 2024-03-21 20:59:13.000000 danielutils-0.9.83/danielutils/conversions/specialized_conversions/__init__.py
+-rw-rw-rw-   0        0        0      507 2024-03-21 23:16:41.000000 danielutils-0.9.83/danielutils/conversions/specialized_conversions/to_hex.py
+-rw-rw-rw-   0        0        0      543 2024-04-28 08:12:13.000000 danielutils-0.9.83/danielutils/conversions/specialized_conversions/to_int.py
+drwxrwxrwx   0        0        0        0 2024-05-01 23:01:55.289762 danielutils-0.9.83/danielutils/data_structures/
+-rw-rw-rw-   0        0        0      163 2024-04-17 20:37:10.000000 danielutils-0.9.83/danielutils/data_structures/__init__.py
+-rw-rw-rw-   0        0        0     1224 2024-04-17 20:37:10.000000 danielutils-0.9.83/danielutils/data_structures/comparer.py
+-rw-rw-rw-   0        0        0      273 2024-04-17 20:37:10.000000 danielutils-0.9.83/danielutils/data_structures/default_dict.py
+-rw-rw-rw-   0        0        0      632 2023-09-25 13:19:42.000000 danielutils-0.9.83/danielutils/data_structures/functions.py
+drwxrwxrwx   0        0        0        0 2024-05-01 23:01:55.292762 danielutils-0.9.83/danielutils/data_structures/graph/
+-rw-rw-rw-   0        0        0       97 2024-04-17 20:37:10.000000 danielutils-0.9.83/danielutils/data_structures/graph/__init__.py
+-rw-rw-rw-   0        0        0     2066 2024-04-18 18:33:41.000000 danielutils-0.9.83/danielutils/data_structures/graph/binary_node.py
+-rw-rw-rw-   0        0        0     6877 2024-04-28 08:12:24.000000 danielutils-0.9.83/danielutils/data_structures/graph/graph.py
+-rw-rw-rw-   0        0        0     3141 2024-04-28 08:12:13.000000 danielutils-0.9.83/danielutils/data_structures/graph/multinode.py
+-rw-rw-rw-   0        0        0     1647 2024-03-28 19:42:06.000000 danielutils-0.9.83/danielutils/data_structures/graph/node.py
+drwxrwxrwx   0        0        0        0 2024-05-01 23:01:55.295807 danielutils-0.9.83/danielutils/data_structures/heap/
+-rw-rw-rw-   0        0        0       71 2024-03-28 19:45:24.000000 danielutils-0.9.83/danielutils/data_structures/heap/__init__.py
+-rw-rw-rw-   0        0        0     3092 2024-04-17 20:37:10.000000 danielutils-0.9.83/danielutils/data_structures/heap/heap.py
+-rw-rw-rw-   0        0        0      292 2024-03-28 19:45:24.000000 danielutils-0.9.83/danielutils/data_structures/heap/max_heap.py
+-rw-rw-rw-   0        0        0      300 2024-03-28 19:45:24.000000 danielutils-0.9.83/danielutils/data_structures/heap/min_heap.py
+drwxrwxrwx   0        0        0        0 2024-05-01 23:01:55.297807 danielutils-0.9.83/danielutils/data_structures/queue/
+-rw-rw-rw-   0        0        0       82 2024-03-28 19:35:07.000000 danielutils-0.9.83/danielutils/data_structures/queue/__init__.py
+-rw-rw-rw-   0        0        0      260 2024-03-28 19:35:13.000000 danielutils-0.9.83/danielutils/data_structures/queue/atomic_queue.py
+-rw-rw-rw-   0        0        0     3661 2024-03-28 19:35:07.000000 danielutils-0.9.83/danielutils/data_structures/queue/priority_queue.py
+-rw-rw-rw-   0        0        0     1615 2024-04-28 08:12:13.000000 danielutils-0.9.83/danielutils/data_structures/queue/queue.py
+-rw-rw-rw-   0        0        0     2143 2024-04-17 20:37:10.000000 danielutils-0.9.83/danielutils/data_structures/stack.py
+drwxrwxrwx   0        0        0        0 2024-05-01 23:01:55.299844 danielutils-0.9.83/danielutils/data_structures/trees/
+-rw-rw-rw-   0        0        0       63 2024-04-17 20:37:10.000000 danielutils-0.9.83/danielutils/data_structures/trees/__init__.py
+-rw-rw-rw-   0        0        0     2636 2024-04-28 08:12:00.000000 danielutils-0.9.83/danielutils/data_structures/trees/binary_syntax_tree.py
+-rw-rw-rw-   0        0        0     1618 2024-04-18 18:33:41.000000 danielutils-0.9.83/danielutils/data_structures/trees/binary_tree.py
+-rw-rw-rw-   0        0        0      675 2024-04-28 08:19:08.000000 danielutils-0.9.83/danielutils/date.py
+-rw-rw-rw-   0        0        0      232 2023-08-07 20:06:13.000000 danielutils-0.9.83/danielutils/date_time.py
+drwxrwxrwx   0        0        0        0 2024-05-01 23:01:55.309915 danielutils-0.9.83/danielutils/decorators/
+-rw-rw-rw-   0        0        0      466 2024-04-25 20:44:13.000000 danielutils-0.9.83/danielutils/decorators/__init__.py
+-rw-rw-rw-   0        0        0      756 2024-04-28 08:19:08.000000 danielutils-0.9.83/danielutils/decorators/atomic.py
+-rw-rw-rw-   0        0        0     1385 2024-04-28 08:19:08.000000 danielutils-0.9.83/danielutils/decorators/attach.py
+-rw-rw-rw-   0        0        0      730 2024-03-21 20:59:13.000000 danielutils-0.9.83/danielutils/decorators/chain_decorators.py
+-rw-rw-rw-   0        0        0     1089 2024-04-28 08:19:08.000000 danielutils-0.9.83/danielutils/decorators/decorate_conditionally.py
+-rw-rw-rw-   0        0        0     1008 2024-04-27 18:49:37.000000 danielutils-0.9.83/danielutils/decorators/delay_call.py
+-rw-rw-rw-   0        0        0     1290 2024-04-27 18:48:35.000000 danielutils-0.9.83/danielutils/decorators/deprecate.py
+-rw-rw-rw-   0        0        0     1023 2024-04-25 20:44:13.000000 danielutils-0.9.83/danielutils/decorators/final.py
+-rw-rw-rw-   0        0        0     1696 2024-04-28 08:19:08.000000 danielutils-0.9.83/danielutils/decorators/limit_recursion.py
+-rw-rw-rw-   0        0        0      806 2024-04-28 08:19:08.000000 danielutils-0.9.83/danielutils/decorators/memo.py
+-rw-rw-rw-   0        0        0     7521 2024-04-28 08:13:16.000000 danielutils-0.9.83/danielutils/decorators/overload.py
+-rw-rw-rw-   0        0        0      837 2024-04-28 08:19:09.000000 danielutils-0.9.83/danielutils/decorators/partially_implemented.py
+-rw-rw-rw-   0        0        0     1716 2024-04-21 19:46:04.000000 danielutils-0.9.83/danielutils/decorators/processify.py
+-rw-rw-rw-   0        0        0     1095 2024-03-21 20:59:13.000000 danielutils-0.9.83/danielutils/decorators/property.py
+-rw-rw-rw-   0        0        0      776 2024-04-17 20:37:10.000000 danielutils-0.9.83/danielutils/decorators/singleton.py
+-rw-rw-rw-   0        0        0      729 2024-05-01 18:07:01.000000 danielutils-0.9.83/danielutils/decorators/threadify.py
+-rw-rw-rw-   0        0        0     1998 2024-04-28 08:19:08.000000 danielutils-0.9.83/danielutils/decorators/timeout.py
+-rw-rw-rw-   0        0        0     3746 2024-04-28 08:13:33.000000 danielutils-0.9.83/danielutils/decorators/total_ordering.py
+-rw-rw-rw-   0        0        0     9556 2024-04-28 08:19:08.000000 danielutils-0.9.83/danielutils/decorators/validate.py
+-rw-rw-rw-   0        0        0     2163 2024-03-21 20:59:13.000000 danielutils-0.9.83/danielutils/exceptions.py
+drwxrwxrwx   0        0        0        0 2024-05-01 23:01:55.316584 danielutils-0.9.83/danielutils/functions/
+-rw-rw-rw-   0        0        0      262 2024-05-01 18:34:21.000000 danielutils-0.9.83/danielutils/functions/__init__.py
+-rw-rw-rw-   0        0        0     1085 2024-04-28 08:12:35.000000 danielutils-0.9.83/danielutils/functions/areoneof.py
+-rw-rw-rw-   0        0        0      638 2024-03-21 20:59:13.000000 danielutils-0.9.83/danielutils/functions/check_foreach.py
+-rw-rw-rw-   0        0        0      791 2024-04-21 19:19:56.000000 danielutils-0.9.83/danielutils/functions/flatten.py
+-rw-rw-rw-   0        0        0    10122 2024-04-28 08:10:10.000000 danielutils-0.9.83/danielutils/functions/isoftype.py
+-rw-rw-rw-   0        0        0     1582 2024-04-28 08:12:35.000000 danielutils-0.9.83/danielutils/functions/isoneof.py
+-rw-rw-rw-   0        0        0     1292 2024-04-28 08:07:23.000000 danielutils-0.9.83/danielutils/functions/multiloop.py
+-rw-rw-rw-   0        0        0      997 2024-05-01 18:34:08.000000 danielutils-0.9.83/danielutils/functions/parallel_for.py
+-rw-rw-rw-   0        0        0      639 2024-03-21 20:59:13.000000 danielutils-0.9.83/danielutils/functions/powerset.py
+-rw-rw-rw-   0        0        0      288 2024-03-21 20:59:13.000000 danielutils-0.9.83/danielutils/functions/subseteq.py
+-rw-rw-rw-   0        0        0     1008 2024-04-28 08:12:24.000000 danielutils-0.9.83/danielutils/functions/types_subseteq.py
+drwxrwxrwx   0        0        0        0 2024-05-01 23:01:55.318585 danielutils-0.9.83/danielutils/generators/
+-rw-rw-rw-   0        0        0      108 2024-03-21 20:59:13.000000 danielutils-0.9.83/danielutils/generators/__init__.py
+-rw-rw-rw-   0        0        0     1285 2024-03-21 20:59:13.000000 danielutils-0.9.83/danielutils/generators/conditional_generator.py
+-rw-rw-rw-   0        0        0      478 2024-04-28 08:19:09.000000 danielutils-0.9.83/danielutils/generators/generator_from_stream.py
+-rw-rw-rw-   0        0        0     2859 2024-04-28 08:12:35.000000 danielutils-0.9.83/danielutils/generators/join_generators.py
+-rw-rw-rw-   0        0        0     2105 2024-04-28 08:19:08.000000 danielutils-0.9.83/danielutils/internet.py
+-rw-rw-rw-   0        0        0    12329 2024-04-28 08:19:14.000000 danielutils-0.9.83/danielutils/io_.py
+drwxrwxrwx   0        0        0        0 2024-05-01 23:01:55.321860 danielutils-0.9.83/danielutils/math_/
+-rw-rw-rw-   0        0        0       52 2024-05-01 22:57:34.000000 danielutils-0.9.83/danielutils/math_/__init__.py
+-rw-rw-rw-   0        0        0     7682 2024-03-21 20:59:13.000000 danielutils-0.9.83/danielutils/math_/constants.py
+-rw-rw-rw-   0        0        0      642 2024-04-28 08:19:09.000000 danielutils-0.9.83/danielutils/math_/functions.py
+-rw-rw-rw-   0        0        0     1063 2024-04-21 18:05:24.000000 danielutils-0.9.83/danielutils/math_/math_print.py
+-rw-rw-rw-   0        0        0     4044 2024-04-28 08:12:00.000000 danielutils-0.9.83/danielutils/math_/math_symbols.py
+drwxrwxrwx   0        0        0        0 2024-05-01 23:01:55.325900 danielutils-0.9.83/danielutils/metaclasses/
+-rw-rw-rw-   0        0        0      169 2024-03-21 23:16:41.000000 danielutils-0.9.83/danielutils/metaclasses/__init__.py
+-rw-rw-rw-   0        0        0      695 2024-03-21 20:59:13.000000 danielutils-0.9.83/danielutils/metaclasses/atomic_class_meta.py
+-rw-rw-rw-   0        0        0     2511 2024-03-21 20:59:13.000000 danielutils-0.9.83/danielutils/metaclasses/implicit_data_deleter_meta.py
+-rw-rw-rw-   0        0        0     1495 2024-04-21 18:13:57.000000 danielutils-0.9.83/danielutils/metaclasses/instance_cache_meta.py
+-rw-rw-rw-   0        0        0    10932 2024-04-28 08:12:24.000000 danielutils-0.9.83/danielutils/metaclasses/interface.py
+-rw-rw-rw-   0        0        0     1754 2024-03-21 20:59:13.000000 danielutils-0.9.83/danielutils/metaclasses/overload_meta.py
+drwxrwxrwx   0        0        0        0 2024-05-01 23:01:55.327902 danielutils-0.9.83/danielutils/mock_/
+-rw-rw-rw-   0        0        0       58 2024-05-01 22:55:24.000000 danielutils-0.9.83/danielutils/mock_/__init__.py
+-rw-rw-rw-   0        0        0     2017 2024-04-21 19:46:04.000000 danielutils-0.9.83/danielutils/mock_/mock_database.py
+-rw-rw-rw-   0        0        0      419 2024-04-17 20:37:10.000000 danielutils-0.9.83/danielutils/mock_/mock_module.py
+-rw-rw-rw-   0        0        0     1032 2024-03-21 20:59:13.000000 danielutils-0.9.83/danielutils/path.py
+-rw-rw-rw-   0        0        0     3845 2024-05-01 23:00:56.000000 danielutils-0.9.83/danielutils/print_.py
+drwxrwxrwx   0        0        0        0 2024-05-01 23:01:55.329901 danielutils-0.9.83/danielutils/progress_bar/
+-rw-rw-rw-   0        0        0       98 2024-05-01 22:55:24.000000 danielutils-0.9.83/danielutils/progress_bar/__init__.py
+-rw-rw-rw-   0        0        0     3433 2024-05-01 22:56:22.000000 danielutils-0.9.83/danielutils/progress_bar/ascii_progress_bar.py
+-rw-rw-rw-   0        0        0     1499 2024-05-01 22:15:58.000000 danielutils-0.9.83/danielutils/progress_bar/progress_bar.py
+-rw-rw-rw-   0        0        0     1745 2024-05-01 22:51:57.000000 danielutils-0.9.83/danielutils/progress_bar/progress_bar_pool.py
+drwxrwxrwx   0        0        0        0 2024-05-01 23:01:55.331902 danielutils-0.9.83/danielutils/protocols/
+-rw-rw-rw-   0        0        0       49 2024-04-17 20:37:10.000000 danielutils-0.9.83/danielutils/protocols/__init__.py
+-rw-rw-rw-   0        0        0      446 2024-04-28 08:12:00.000000 danielutils-0.9.83/danielutils/protocols/dictable.py
+-rw-rw-rw-   0        0        0      203 2024-04-17 20:37:10.000000 danielutils-0.9.83/danielutils/protocols/evaluable.py
+-rw-rw-rw-   0        0        0        0 2023-08-09 09:08:58.000000 danielutils-0.9.83/danielutils/py.typed
+drwxrwxrwx   0        0        0        0 2024-05-01 23:01:55.332901 danielutils-0.9.83/danielutils/reflection/
+-rw-rw-rw-   0        0        0     1516 2024-04-21 18:21:37.000000 danielutils-0.9.83/danielutils/reflection/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-01 23:01:55.333901 danielutils-0.9.83/danielutils/reflection/class_/
+-rw-rw-rw-   0        0        0       31 2024-04-21 18:21:37.000000 danielutils-0.9.83/danielutils/reflection/class_/__init__.py
+-rw-rw-rw-   0        0        0     5507 2024-04-28 08:12:35.000000 danielutils-0.9.83/danielutils/reflection/class_/class_reflection.py
+drwxrwxrwx   0        0        0        0 2024-05-01 23:01:55.334941 danielutils-0.9.83/danielutils/reflection/file/
+-rw-rw-rw-   0        0        0       30 2024-04-21 18:21:37.000000 danielutils-0.9.83/danielutils/reflection/file/__init__.py
+-rw-rw-rw-   0        0        0     1657 2024-04-27 18:35:37.000000 danielutils-0.9.83/danielutils/reflection/file/file_reflection.py
+drwxrwxrwx   0        0        0        0 2024-05-01 23:01:55.335940 danielutils-0.9.83/danielutils/reflection/function/
+-rw-rw-rw-   0        0        0       35 2024-04-21 18:21:37.000000 danielutils-0.9.83/danielutils/reflection/function/__init__.py
+-rw-rw-rw-   0        0        0     4453 2024-04-28 08:12:24.000000 danielutils-0.9.83/danielutils/reflection/function/function_reflections.py
+drwxrwxrwx   0        0        0        0 2024-05-01 23:01:55.340982 danielutils-0.9.83/danielutils/reflection/interpreter/
+-rw-rw-rw-   0        0        0      179 2024-04-21 19:19:56.000000 danielutils-0.9.83/danielutils/reflection/interpreter/__init__.py
+-rw-rw-rw-   0        0        0     1074 2024-04-25 20:37:30.000000 danielutils-0.9.83/danielutils/reflection/interpreter/callstack.py
+-rw-rw-rw-   0        0        0      441 2024-04-28 08:12:13.000000 danielutils-0.9.83/danielutils/reflection/interpreter/get_traceback.py
+-rw-rw-rw-   0        0        0      622 2024-04-17 20:37:10.000000 danielutils-0.9.83/danielutils/reflection/interpreter/os_.py
+-rw-rw-rw-   0        0        0     1023 2024-04-17 20:37:10.000000 danielutils-0.9.83/danielutils/reflection/interpreter/packages.py
+-rw-rw-rw-   0        0        0      621 2024-04-28 08:12:35.000000 danielutils-0.9.83/danielutils/reflection/interpreter/python_version.py
+-rw-rw-rw-   0        0        0      489 2024-03-21 20:59:13.000000 danielutils-0.9.83/danielutils/reflection/interpreter/signals.py
+-rw-rw-rw-   0        0        0     5733 2024-04-28 08:12:24.000000 danielutils-0.9.83/danielutils/reflection/interpreter/tracer.py
+drwxrwxrwx   0        0        0        0 2024-05-01 23:01:55.341982 danielutils-0.9.83/danielutils/reflection/module/
+-rw-rw-rw-   0        0        0       68 2024-04-21 18:27:13.000000 danielutils-0.9.83/danielutils/reflection/module/__init__.py
+-rw-rw-rw-   0        0        0      507 2024-03-21 20:59:13.000000 danielutils-0.9.83/danielutils/reflection/module/module_reflections.py
+-rw-rw-rw-   0        0        0     4714 2024-04-28 08:12:24.000000 danielutils-0.9.83/danielutils/reflection/module/package_reflection.py
+drwxrwxrwx   0        0        0        0 2024-05-01 23:01:55.342983 danielutils-0.9.83/danielutils/snippets/
+-rw-rw-rw-   0        0        0       24 2024-03-21 20:59:13.000000 danielutils-0.9.83/danielutils/snippets/__init__.py
+-rw-rw-rw-   0        0        0      433 2024-03-21 20:59:13.000000 danielutils-0.9.83/danielutils/snippets/try_get.py
+drwxrwxrwx   0        0        0        0 2024-05-01 23:01:55.345012 danielutils-0.9.83/danielutils/system/
+-rw-rw-rw-   0        0        0       84 2024-05-01 12:22:07.000000 danielutils-0.9.83/danielutils/system/__init__.py
+-rw-rw-rw-   0        0        0     6863 2024-04-28 08:19:08.000000 danielutils-0.9.83/danielutils/system/independent.py
+-rw-rw-rw-   0        0        0     4944 2024-05-01 19:12:58.000000 danielutils-0.9.83/danielutils/system/layered_command.py
+drwxrwxrwx   0        0        0        0 2024-05-01 23:01:55.347013 danielutils-0.9.83/danielutils/system/windows/
+-rw-rw-rw-   0        0        0       50 2024-03-21 20:59:13.000000 danielutils-0.9.83/danielutils/system/windows/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-01 23:01:55.348012 danielutils-0.9.83/danielutils/system/windows/utils/
+-rw-rw-rw-   0        0        0       25 2024-03-21 20:59:13.000000 danielutils-0.9.83/danielutils/system/windows/utils/__init__.py
+-rw-rw-rw-   0        0        0      499 2024-04-17 20:37:10.000000 danielutils-0.9.83/danielutils/system/windows/utils/filetime.py
+-rw-rw-rw-   0        0        0     6064 2024-03-21 20:59:13.000000 danielutils-0.9.83/danielutils/system/windows/win32_ctime.py
+-rw-rw-rw-   0        0        0     2253 2024-03-21 20:59:13.000000 danielutils-0.9.83/danielutils/system/windows/windows.py
+-rw-rw-rw-   0        0        0     4213 2024-04-28 08:19:08.000000 danielutils-0.9.83/danielutils/text.py
+-rw-rw-rw-   0        0        0     1225 2024-04-27 18:53:17.000000 danielutils-0.9.83/danielutils/time.py
+drwxrwxrwx   0        0        0        0 2024-05-01 23:01:55.349012 danielutils-0.9.83/danielutils/university/
+-rw-rw-rw-   0        0        0       74 2024-04-17 20:37:10.000000 danielutils-0.9.83/danielutils/university/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-01 23:01:55.350016 danielutils-0.9.83/danielutils/university/databases/
+-rw-rw-rw-   0        0        0       20 2024-03-21 20:59:13.000000 danielutils-0.9.83/danielutils/university/databases/__init__.py
+-rw-rw-rw-   0        0        0    24890 2024-04-28 08:12:35.000000 danielutils-0.9.83/danielutils/university/databases/all.py
+drwxrwxrwx   0        0        0        0 2024-05-01 23:01:55.352016 danielutils-0.9.83/danielutils/university/oop/
+-rw-rw-rw-   0        0        0       25 2024-04-17 20:37:10.000000 danielutils-0.9.83/danielutils/university/oop/__init__.py
+-rw-rw-rw-   0        0        0      802 2024-04-28 08:13:50.000000 danielutils-0.9.83/danielutils/university/oop/observer.py
+-rw-rw-rw-   0        0        0       87 2024-04-17 20:37:10.000000 danielutils-0.9.83/danielutils/university/oop/strategy.py
+drwxrwxrwx   0        0        0        0 2024-05-01 23:01:55.354904 danielutils-0.9.83/danielutils/university/probability/
+-rw-rw-rw-   0        0        0      189 2024-04-21 22:41:40.000000 danielutils-0.9.83/danielutils/university/probability/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-01 23:01:55.356986 danielutils-0.9.83/danielutils/university/probability/conditional_variable/
+-rw-rw-rw-   0        0        0       89 2024-04-17 20:37:10.000000 danielutils-0.9.83/danielutils/university/probability/conditional_variable/__init__.py
+-rw-rw-rw-   0        0        0     4004 2024-04-25 21:21:07.000000 danielutils-0.9.83/danielutils/university/probability/conditional_variable/conditional_variable.py
+drwxrwxrwx   0        0        0        0 2024-05-01 23:01:55.356986 danielutils-0.9.83/danielutils/university/probability/conditional_variable/continuous/
+-rw-rw-rw-   0        0        0        0 2024-04-17 20:37:10.000000 danielutils-0.9.83/danielutils/university/probability/conditional_variable/continuous/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-01 23:01:55.361987 danielutils-0.9.83/danielutils/university/probability/conditional_variable/discrete/
+-rw-rw-rw-   0        0        0      209 2024-04-17 20:37:10.000000 danielutils-0.9.83/danielutils/university/probability/conditional_variable/discrete/__init__.py
+-rw-rw-rw-   0        0        0     1149 2024-04-21 22:51:43.000000 danielutils-0.9.83/danielutils/university/probability/conditional_variable/discrete/bernoulli.py
+-rw-rw-rw-   0        0        0     1257 2024-04-21 22:51:43.000000 danielutils-0.9.83/danielutils/university/probability/conditional_variable/discrete/binomial.py
+-rw-rw-rw-   0        0        0     1108 2024-04-21 22:51:43.000000 danielutils-0.9.83/danielutils/university/probability/conditional_variable/discrete/conditional_from_discrete_probability_func.py
+-rw-rw-rw-   0        0        0     1370 2024-04-21 22:51:43.000000 danielutils-0.9.83/danielutils/university/probability/conditional_variable/discrete/discrete.py
+-rw-rw-rw-   0        0        0     1652 2024-04-28 08:12:35.000000 danielutils-0.9.83/danielutils/university/probability/conditional_variable/discrete/geometric.py
+-rw-rw-rw-   0        0        0      992 2024-04-21 22:51:43.000000 danielutils-0.9.83/danielutils/university/probability/conditional_variable/discrete/poisson.py
+-rw-rw-rw-   0        0        0     1040 2024-04-21 22:51:43.000000 danielutils-0.9.83/danielutils/university/probability/conditional_variable/discrete/uniform.py
+-rw-rw-rw-   0        0        0      904 2024-04-21 22:41:40.000000 danielutils-0.9.83/danielutils/university/probability/distributions.py
+drwxrwxrwx   0        0        0        0 2024-05-01 23:01:55.363987 danielutils-0.9.83/danielutils/university/probability/expressions/
+-rw-rw-rw-   0        0        0       79 2024-04-17 22:49:00.000000 danielutils-0.9.83/danielutils/university/probability/expressions/__init__.py
+-rw-rw-rw-   0        0        0     7439 2024-04-25 21:20:42.000000 danielutils-0.9.83/danielutils/university/probability/expressions/accumulation_expression.py
+-rw-rw-rw-   0        0        0     4391 2024-04-25 21:20:53.000000 danielutils-0.9.83/danielutils/university/probability/expressions/probability_expression.py
+drwxrwxrwx   0        0        0        0 2024-05-01 23:01:55.367031 danielutils-0.9.83/danielutils/university/probability/funcs/
+-rw-rw-rw-   0        0        0      120 2024-04-17 20:37:10.000000 danielutils-0.9.83/danielutils/university/probability/funcs/__init__.py
+-rw-rw-rw-   0        0        0      338 2024-04-21 22:41:40.000000 danielutils-0.9.83/danielutils/university/probability/funcs/covariance.py
+-rw-rw-rw-   0        0        0     1173 2024-04-21 22:41:40.000000 danielutils-0.9.83/danielutils/university/probability/funcs/expected_value.py
+-rw-rw-rw-   0        0        0      306 2024-04-17 20:37:10.000000 danielutils-0.9.83/danielutils/university/probability/funcs/probability_function.py
+-rw-rw-rw-   0        0        0      437 2024-04-21 22:41:40.000000 danielutils-0.9.83/danielutils/university/probability/funcs/variance.py
+-rw-rw-rw-   0        0        0     1987 2024-04-28 08:12:24.000000 danielutils-0.9.83/danielutils/university/probability/operator.py
+-rw-rw-rw-   0        0        0      641 2024-04-18 18:33:41.000000 danielutils-0.9.83/danielutils/university/probability/protocols.py
+-rw-rw-rw-   0        0        0     2055 2024-04-21 22:51:43.000000 danielutils-0.9.83/danielutils/university/probability/supp.py
+-rw-rw-rw-   0        0        0     1182 2024-04-25 20:08:45.000000 danielutils-0.9.83/danielutils/university/probability/transformation.py
+-rw-rw-rw-   0        0        0      322 2024-04-28 08:07:53.000000 danielutils-0.9.83/danielutils/versioned_imports.py
+drwxrwxrwx   0        0        0        0 2024-05-01 23:01:55.270561 danielutils-0.9.83/danielutils.egg-info/
+-rw-rw-rw-   0        0        0     4593 2024-05-01 23:01:55.000000 danielutils-0.9.83/danielutils.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     7964 2024-05-01 23:01:55.000000 danielutils-0.9.83/danielutils.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-01 23:01:55.000000 danielutils-0.9.83/danielutils.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       12 2024-05-01 23:01:55.000000 danielutils-0.9.83/danielutils.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      977 2024-05-01 23:01:54.000000 danielutils-0.9.83/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-05-01 23:01:55.369031 danielutils-0.9.83/setup.cfg
+-rw-rw-rw-   0        0        0       41 2024-05-01 23:01:54.000000 danielutils-0.9.83/setup.py
```

### Comparing `danielutils-0.9.82/LICENSE` & `danielutils-0.9.83/LICENSE`

 * *Files identical despite different names*

### Comparing `danielutils-0.9.82/PKG-INFO` & `danielutils-0.9.83/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: danielutils
-Version: 0.9.82
+Version: 0.9.83
 Summary: A python utils library for things I find useful
 Author-email: danielnachumdev <danielnachumdev@gmail.com>
 License: MIT License
         
         Copyright (c) 2022 danielnachumdev
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -37,15 +37,15 @@
 
 
 [![Python package](https://github.com/danielnachumdev/danielutils/actions/workflows/python-package.yml/badge.svg)](https://github.com/danielnachumdev/danielutils/actions/workflows/python-package.yml)
 [![Pylint](https://github.com/danielnachumdev/danielutils/actions/workflows/pylint.yml/badge.svg)](https://github.com/danielnachumdev/danielutils/actions/workflows/pylint.yml)
 [![Python 3.10.11](https://img.shields.io/badge/python-3.10.11-blue.svg)](https://www.python.org/downloads/release/python-31011/)
 [![gitleaks](https://github.com/danielnachumdev/danielutils/actions/workflows/gitleaks.yml/badge.svg)](https://github.com/danielnachumdev/danielutils/actions/workflows/gitleaks.yml)
 [![CodeQL](https://github.com/danielnachumdev/danielutils/actions/workflows/github-code-scanning/codeql/badge.svg)](https://github.com/danielnachumdev/danielutils/actions/workflows/github-code-scanning/codeql)
-# danielutils v=0.9.82
+# danielutils v=0.9.83
 A utils library for things that I find useful for my coding workflow.\
 Feel free to use and / or contribute / improve my code :)
 
 THIS PACKAGE IS IN DEVELOPMENT AND SUBJECT TO CHANGE, USE AT YOUR OWN RISK!
 
 **Tested python versions**: `3.8.0`*, `3.9.0`, `3.10.13`
```

### Comparing `danielutils-0.9.82/README.md` & `danielutils-0.9.83/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 
 [![Python package](https://github.com/danielnachumdev/danielutils/actions/workflows/python-package.yml/badge.svg)](https://github.com/danielnachumdev/danielutils/actions/workflows/python-package.yml)
 [![Pylint](https://github.com/danielnachumdev/danielutils/actions/workflows/pylint.yml/badge.svg)](https://github.com/danielnachumdev/danielutils/actions/workflows/pylint.yml)
 [![Python 3.10.11](https://img.shields.io/badge/python-3.10.11-blue.svg)](https://www.python.org/downloads/release/python-31011/)
 [![gitleaks](https://github.com/danielnachumdev/danielutils/actions/workflows/gitleaks.yml/badge.svg)](https://github.com/danielnachumdev/danielutils/actions/workflows/gitleaks.yml)
 [![CodeQL](https://github.com/danielnachumdev/danielutils/actions/workflows/github-code-scanning/codeql/badge.svg)](https://github.com/danielnachumdev/danielutils/actions/workflows/github-code-scanning/codeql)
-# danielutils v=0.9.82
+# danielutils v=0.9.83
 A utils library for things that I find useful for my coding workflow.\
 Feel free to use and / or contribute / improve my code :)
 
 THIS PACKAGE IS IN DEVELOPMENT AND SUBJECT TO CHANGE, USE AT YOUR OWN RISK!
 
 **Tested python versions**: `3.8.0`*, `3.9.0`, `3.10.13`
```

### Comparing `danielutils-0.9.82/danielutils/__init__.py` & `danielutils-0.9.83/danielutils/__init__.py`

 * *Files 9% similar despite different names*

```diff
@@ -13,17 +13,16 @@
 from .protocols import *
 # =================================================================
 # ========================= ORDER MATTERS =========================
 # =================================================================
 
 from .reflection import *
 from .decorators import *
-
 # ========== NEEDS REFLECTION ==========
-from .tqdm_ import *
+from .progress_bar import *
 # ========== NEEDS DECORATORS ==========
 from .colors import *
 # ========== NEEDS BOTH ==========
 
 from .functions import *
 from .io_ import *
 from .system import *
```

### Comparing `danielutils-0.9.82/danielutils/abstractions/database/cached_database.py` & `danielutils-0.9.83/danielutils/abstractions/database/cached_database.py`

 * *Files identical despite different names*

### Comparing `danielutils-0.9.82/danielutils/abstractions/database/database.py` & `danielutils-0.9.83/danielutils/abstractions/database/database.py`

 * *Files identical despite different names*

### Comparing `danielutils-0.9.82/danielutils/abstractions/database/redis_database.py` & `danielutils-0.9.83/danielutils/abstractions/database/redis_database.py`

 * *Files identical despite different names*

### Comparing `danielutils-0.9.82/danielutils/abstractions/multiprogramming/worker.py` & `danielutils-0.9.83/danielutils/abstractions/multiprogramming/worker.py`

 * *Files identical despite different names*

### Comparing `danielutils-0.9.82/danielutils/abstractions/multiprogramming/worker_pool.py` & `danielutils-0.9.83/danielutils/abstractions/multiprogramming/worker_pool.py`

 * *Files identical despite different names*

### Comparing `danielutils-0.9.82/danielutils/abstractions/repl.py` & `danielutils-0.9.83/danielutils/abstractions/repl.py`

 * *Files identical despite different names*

### Comparing `danielutils-0.9.82/danielutils/aliases.py` & `danielutils-0.9.83/danielutils/aliases.py`

 * *Files identical despite different names*

### Comparing `danielutils-0.9.82/danielutils/better_builtins/counter.py` & `danielutils-0.9.83/danielutils/better_builtins/counter.py`

 * *Files identical despite different names*

### Comparing `danielutils-0.9.82/danielutils/better_builtins/frange.py` & `danielutils-0.9.83/danielutils/better_builtins/frange.py`

 * *Files identical despite different names*

### Comparing `danielutils-0.9.82/danielutils/better_builtins/typed_builtins/factory.py` & `danielutils-0.9.83/danielutils/better_builtins/typed_builtins/factory.py`

 * *Files identical despite different names*

### Comparing `danielutils-0.9.82/danielutils/better_builtins/typed_builtins/tdict.py` & `danielutils-0.9.83/danielutils/better_builtins/typed_builtins/tdict.py`

 * *Files identical despite different names*

### Comparing `danielutils-0.9.82/danielutils/better_builtins/typed_builtins/tlist.py` & `danielutils-0.9.83/danielutils/better_builtins/typed_builtins/tlist.py`

 * *Files identical despite different names*

### Comparing `danielutils-0.9.82/danielutils/better_builtins/typed_builtins/tset.py` & `danielutils-0.9.83/danielutils/better_builtins/typed_builtins/tset.py`

 * *Files identical despite different names*

### Comparing `danielutils-0.9.82/danielutils/colors.py` & `danielutils-0.9.83/danielutils/colors.py`

 * *Files identical despite different names*

### Comparing `danielutils-0.9.82/danielutils/context_managers/attr_context.py` & `danielutils-0.9.83/danielutils/context_managers/attr_context.py`

 * *Files identical despite different names*

### Comparing `danielutils-0.9.82/danielutils/context_managers/temporary_file.py` & `danielutils-0.9.83/danielutils/context_managers/temporary_file.py`

 * *Files identical despite different names*

### Comparing `danielutils-0.9.82/danielutils/conversions/main_conversions.py` & `danielutils-0.9.83/danielutils/conversions/main_conversions.py`

 * *Files identical despite different names*

### Comparing `danielutils-0.9.82/danielutils/conversions/specialized_conversions/to_int.py` & `danielutils-0.9.83/danielutils/conversions/specialized_conversions/to_int.py`

 * *Files identical despite different names*

### Comparing `danielutils-0.9.82/danielutils/data_structures/comparer.py` & `danielutils-0.9.83/danielutils/data_structures/comparer.py`

 * *Files identical despite different names*

### Comparing `danielutils-0.9.82/danielutils/data_structures/functions.py` & `danielutils-0.9.83/danielutils/data_structures/functions.py`

 * *Files identical despite different names*

### Comparing `danielutils-0.9.82/danielutils/data_structures/graph/binary_node.py` & `danielutils-0.9.83/danielutils/data_structures/graph/binary_node.py`

 * *Files identical despite different names*

### Comparing `danielutils-0.9.82/danielutils/data_structures/graph/graph.py` & `danielutils-0.9.83/danielutils/data_structures/graph/graph.py`

 * *Files identical despite different names*

### Comparing `danielutils-0.9.82/danielutils/data_structures/graph/multinode.py` & `danielutils-0.9.83/danielutils/data_structures/graph/multinode.py`

 * *Files identical despite different names*

### Comparing `danielutils-0.9.82/danielutils/data_structures/graph/node.py` & `danielutils-0.9.83/danielutils/data_structures/graph/node.py`

 * *Files identical despite different names*

### Comparing `danielutils-0.9.82/danielutils/data_structures/heap/heap.py` & `danielutils-0.9.83/danielutils/data_structures/heap/heap.py`

 * *Files identical despite different names*

### Comparing `danielutils-0.9.82/danielutils/data_structures/queue/priority_queue.py` & `danielutils-0.9.83/danielutils/data_structures/queue/priority_queue.py`

 * *Files identical despite different names*

### Comparing `danielutils-0.9.82/danielutils/data_structures/queue/queue.py` & `danielutils-0.9.83/danielutils/data_structures/queue/queue.py`

 * *Files identical despite different names*

### Comparing `danielutils-0.9.82/danielutils/data_structures/stack.py` & `danielutils-0.9.83/danielutils/data_structures/stack.py`

 * *Files identical despite different names*

### Comparing `danielutils-0.9.82/danielutils/data_structures/trees/binary_syntax_tree.py` & `danielutils-0.9.83/danielutils/data_structures/trees/binary_syntax_tree.py`

 * *Files identical despite different names*

### Comparing `danielutils-0.9.82/danielutils/data_structures/trees/binary_tree.py` & `danielutils-0.9.83/danielutils/data_structures/trees/binary_tree.py`

 * *Files identical despite different names*

### Comparing `danielutils-0.9.82/danielutils/date.py` & `danielutils-0.9.83/danielutils/date.py`

 * *Files identical despite different names*

### Comparing `danielutils-0.9.82/danielutils/decorators/atomic.py` & `danielutils-0.9.83/danielutils/decorators/atomic.py`

 * *Files identical despite different names*

### Comparing `danielutils-0.9.82/danielutils/decorators/attach.py` & `danielutils-0.9.83/danielutils/decorators/attach.py`

 * *Files identical despite different names*

### Comparing `danielutils-0.9.82/danielutils/decorators/chain_decorators.py` & `danielutils-0.9.83/danielutils/decorators/chain_decorators.py`

 * *Files identical despite different names*

### Comparing `danielutils-0.9.82/danielutils/decorators/decorate_conditionally.py` & `danielutils-0.9.83/danielutils/decorators/decorate_conditionally.py`

 * *Files identical despite different names*

### Comparing `danielutils-0.9.82/danielutils/decorators/delay_call.py` & `danielutils-0.9.83/danielutils/decorators/delay_call.py`

 * *Files identical despite different names*

### Comparing `danielutils-0.9.82/danielutils/decorators/deprecate.py` & `danielutils-0.9.83/danielutils/decorators/deprecate.py`

 * *Files identical despite different names*

### Comparing `danielutils-0.9.82/danielutils/decorators/final.py` & `danielutils-0.9.83/danielutils/decorators/final.py`

 * *Files identical despite different names*

### Comparing `danielutils-0.9.82/danielutils/decorators/limit_recursion.py` & `danielutils-0.9.83/danielutils/decorators/limit_recursion.py`

 * *Files identical despite different names*

### Comparing `danielutils-0.9.82/danielutils/decorators/memo.py` & `danielutils-0.9.83/danielutils/decorators/memo.py`

 * *Files identical despite different names*

### Comparing `danielutils-0.9.82/danielutils/decorators/overload.py` & `danielutils-0.9.83/danielutils/decorators/overload.py`

 * *Files identical despite different names*

### Comparing `danielutils-0.9.82/danielutils/decorators/partially_implemented.py` & `danielutils-0.9.83/danielutils/decorators/partially_implemented.py`

 * *Files identical despite different names*

### Comparing `danielutils-0.9.82/danielutils/decorators/processify.py` & `danielutils-0.9.83/danielutils/decorators/processify.py`

 * *Files identical despite different names*

### Comparing `danielutils-0.9.82/danielutils/decorators/property.py` & `danielutils-0.9.83/danielutils/decorators/property.py`

 * *Files identical despite different names*

### Comparing `danielutils-0.9.82/danielutils/decorators/singleton.py` & `danielutils-0.9.83/danielutils/decorators/singleton.py`

 * *Files identical despite different names*

### Comparing `danielutils-0.9.82/danielutils/decorators/threadify.py` & `danielutils-0.9.83/danielutils/decorators/threadify.py`

 * *Files identical despite different names*

### Comparing `danielutils-0.9.82/danielutils/decorators/timeout.py` & `danielutils-0.9.83/danielutils/decorators/timeout.py`

 * *Files identical despite different names*

### Comparing `danielutils-0.9.82/danielutils/decorators/total_ordering.py` & `danielutils-0.9.83/danielutils/decorators/total_ordering.py`

 * *Files identical despite different names*

### Comparing `danielutils-0.9.82/danielutils/decorators/validate.py` & `danielutils-0.9.83/danielutils/decorators/validate.py`

 * *Files identical despite different names*

### Comparing `danielutils-0.9.82/danielutils/exceptions.py` & `danielutils-0.9.83/danielutils/exceptions.py`

 * *Files identical despite different names*

### Comparing `danielutils-0.9.82/danielutils/functions/areoneof.py` & `danielutils-0.9.83/danielutils/functions/areoneof.py`

 * *Files identical despite different names*

### Comparing `danielutils-0.9.82/danielutils/functions/check_foreach.py` & `danielutils-0.9.83/danielutils/functions/check_foreach.py`

 * *Files identical despite different names*

### Comparing `danielutils-0.9.82/danielutils/functions/flatten.py` & `danielutils-0.9.83/danielutils/functions/flatten.py`

 * *Files identical despite different names*

### Comparing `danielutils-0.9.82/danielutils/functions/isoftype.py` & `danielutils-0.9.83/danielutils/functions/isoftype.py`

 * *Files identical despite different names*

### Comparing `danielutils-0.9.82/danielutils/functions/isoneof.py` & `danielutils-0.9.83/danielutils/functions/isoneof.py`

 * *Files identical despite different names*

### Comparing `danielutils-0.9.82/danielutils/functions/multiloop.py` & `danielutils-0.9.83/danielutils/functions/multiloop.py`

 * *Files identical despite different names*

### Comparing `danielutils-0.9.82/danielutils/functions/powerset.py` & `danielutils-0.9.83/danielutils/functions/powerset.py`

 * *Files identical despite different names*

### Comparing `danielutils-0.9.82/danielutils/functions/types_subseteq.py` & `danielutils-0.9.83/danielutils/functions/types_subseteq.py`

 * *Files identical despite different names*

### Comparing `danielutils-0.9.82/danielutils/generators/conditional_generator.py` & `danielutils-0.9.83/danielutils/generators/conditional_generator.py`

 * *Files identical despite different names*

### Comparing `danielutils-0.9.82/danielutils/generators/join_generators.py` & `danielutils-0.9.83/danielutils/generators/join_generators.py`

 * *Files identical despite different names*

### Comparing `danielutils-0.9.82/danielutils/internet.py` & `danielutils-0.9.83/danielutils/internet.py`

 * *Files identical despite different names*

### Comparing `danielutils-0.9.82/danielutils/io_.py` & `danielutils-0.9.83/danielutils/io_.py`

 * *Files identical despite different names*

### Comparing `danielutils-0.9.82/danielutils/math_/constants.py` & `danielutils-0.9.83/danielutils/math_/constants.py`

 * *Files identical despite different names*

### Comparing `danielutils-0.9.82/danielutils/math_/functions.py` & `danielutils-0.9.83/danielutils/math_/functions.py`

 * *Files identical despite different names*

### Comparing `danielutils-0.9.82/danielutils/math_/math_print.py` & `danielutils-0.9.83/danielutils/math_/math_print.py`

 * *Files identical despite different names*

### Comparing `danielutils-0.9.82/danielutils/math_/math_symbols.py` & `danielutils-0.9.83/danielutils/math_/math_symbols.py`

 * *Files identical despite different names*

### Comparing `danielutils-0.9.82/danielutils/metaclasses/atomic_class_meta.py` & `danielutils-0.9.83/danielutils/metaclasses/atomic_class_meta.py`

 * *Files identical despite different names*

### Comparing `danielutils-0.9.82/danielutils/metaclasses/implicit_data_deleter_meta.py` & `danielutils-0.9.83/danielutils/metaclasses/implicit_data_deleter_meta.py`

 * *Files identical despite different names*

### Comparing `danielutils-0.9.82/danielutils/metaclasses/instance_cache_meta.py` & `danielutils-0.9.83/danielutils/metaclasses/instance_cache_meta.py`

 * *Files identical despite different names*

### Comparing `danielutils-0.9.82/danielutils/metaclasses/interface.py` & `danielutils-0.9.83/danielutils/metaclasses/interface.py`

 * *Files identical despite different names*

### Comparing `danielutils-0.9.82/danielutils/metaclasses/overload_meta.py` & `danielutils-0.9.83/danielutils/metaclasses/overload_meta.py`

 * *Files identical despite different names*

### Comparing `danielutils-0.9.82/danielutils/mock_/mock_database.py` & `danielutils-0.9.83/danielutils/mock_/mock_database.py`

 * *Files identical despite different names*

### Comparing `danielutils-0.9.82/danielutils/path.py` & `danielutils-0.9.83/danielutils/path.py`

 * *Files identical despite different names*

### Comparing `danielutils-0.9.82/danielutils/reflection/__init__.py` & `danielutils-0.9.83/danielutils/reflection/__init__.py`

 * *Files identical despite different names*

### Comparing `danielutils-0.9.82/danielutils/reflection/class_/class_reflection.py` & `danielutils-0.9.83/danielutils/reflection/class_/class_reflection.py`

 * *Files identical despite different names*

### Comparing `danielutils-0.9.82/danielutils/reflection/file/file_reflection.py` & `danielutils-0.9.83/danielutils/reflection/file/file_reflection.py`

 * *Files identical despite different names*

### Comparing `danielutils-0.9.82/danielutils/reflection/function/function_reflections.py` & `danielutils-0.9.83/danielutils/reflection/function/function_reflections.py`

 * *Files identical despite different names*

### Comparing `danielutils-0.9.82/danielutils/reflection/interpreter/callstack.py` & `danielutils-0.9.83/danielutils/reflection/interpreter/callstack.py`

 * *Files identical despite different names*

### Comparing `danielutils-0.9.82/danielutils/reflection/interpreter/os_.py` & `danielutils-0.9.83/danielutils/reflection/interpreter/os_.py`

 * *Files identical despite different names*

### Comparing `danielutils-0.9.82/danielutils/reflection/interpreter/packages.py` & `danielutils-0.9.83/danielutils/reflection/interpreter/packages.py`

 * *Files identical despite different names*

### Comparing `danielutils-0.9.82/danielutils/reflection/interpreter/python_version.py` & `danielutils-0.9.83/danielutils/reflection/interpreter/python_version.py`

 * *Files identical despite different names*

### Comparing `danielutils-0.9.82/danielutils/reflection/interpreter/tracer.py` & `danielutils-0.9.83/danielutils/reflection/interpreter/tracer.py`

 * *Files identical despite different names*

### Comparing `danielutils-0.9.82/danielutils/reflection/module/package_reflection.py` & `danielutils-0.9.83/danielutils/reflection/module/package_reflection.py`

 * *Files identical despite different names*

### Comparing `danielutils-0.9.82/danielutils/system/independent.py` & `danielutils-0.9.83/danielutils/system/independent.py`

 * *Files identical despite different names*

### Comparing `danielutils-0.9.82/danielutils/system/layered_command.py` & `danielutils-0.9.83/danielutils/system/layered_command.py`

 * *Files 6% similar despite different names*

```diff
@@ -8,14 +8,22 @@
     class_flush_stdout: bool = True
     class_flush_stderr: bool = True
     class_raise_on_fail: bool = True
     class_verbose: bool = False
     _class_prev_instance: Optional['LayeredCommand'] = None
     _id: int = 0
 
+    @property
+    def prev(self):
+        return self._prev_instance
+
+    @prev.setter
+    def prev(self, value: Optional['LayeredCommand'] = None):
+        self._prev_instance = value
+
     def __init__(
             self,
             command: Optional[str] = None,
             *,
             prev_instance: Optional['LayeredCommand'] = None,
             instance_flush_stdout: Optional[bool] = None,
             instance_flush_stderr: Optional[bool] = None,
@@ -33,25 +41,25 @@
         self._executor = os.system
         self._has_entered: bool = False
 
     def __enter__(self):
         self._open()
         return self
 
+    def __exit__(self, exc_type, exc_val, exc_tb):
+        if self.prev is self._cur_class_prev_instance:
+            LayeredCommand._class_prev_instance = self.prev
+
     def _open(self) -> None:
         self._has_entered = True
 
-    def __exit__(self, exc_type, exc_val, exc_tb):
-        if self._prev_instance is self._cur_class_prev_instance:
-            LayeredCommand._class_prev_instance = self._prev_instance
-
     def _build_command(self, *commands: str) -> str:
         res = ""
-        if self._prev_instance is not None:
-            prev = self._prev_instance._build_command()
+        if self.prev is not None:
+            prev = self.prev._build_command()
             res += f"{prev} & " if prev != "" else ""
         if self._command != "":
             return res + " & ".join([self._command, *commands])
         return res + " & ".join(commands)
 
     def _error(self, predicate: bool, command: str, code: int, command_verbose: Optional[bool]) -> None:
         if predicate:
```

### Comparing `danielutils-0.9.82/danielutils/system/windows/win32_ctime.py` & `danielutils-0.9.83/danielutils/system/windows/win32_ctime.py`

 * *Files identical despite different names*

### Comparing `danielutils-0.9.82/danielutils/system/windows/windows.py` & `danielutils-0.9.83/danielutils/system/windows/windows.py`

 * *Files identical despite different names*

### Comparing `danielutils-0.9.82/danielutils/text.py` & `danielutils-0.9.83/danielutils/text.py`

 * *Files identical despite different names*

### Comparing `danielutils-0.9.82/danielutils/time.py` & `danielutils-0.9.83/danielutils/time.py`

 * *Files identical despite different names*

### Comparing `danielutils-0.9.82/danielutils/university/databases/all.py` & `danielutils-0.9.83/danielutils/university/databases/all.py`

 * *Files identical despite different names*

### Comparing `danielutils-0.9.82/danielutils/university/oop/observer.py` & `danielutils-0.9.83/danielutils/university/oop/observer.py`

 * *Files identical despite different names*

### Comparing `danielutils-0.9.82/danielutils/university/probability/conditional_variable/conditional_variable.py` & `danielutils-0.9.83/danielutils/university/probability/conditional_variable/conditional_variable.py`

 * *Files identical despite different names*

### Comparing `danielutils-0.9.82/danielutils/university/probability/conditional_variable/discrete/bernoulli.py` & `danielutils-0.9.83/danielutils/university/probability/conditional_variable/discrete/bernoulli.py`

 * *Files identical despite different names*

### Comparing `danielutils-0.9.82/danielutils/university/probability/conditional_variable/discrete/binomial.py` & `danielutils-0.9.83/danielutils/university/probability/conditional_variable/discrete/binomial.py`

 * *Files identical despite different names*

### Comparing `danielutils-0.9.82/danielutils/university/probability/conditional_variable/discrete/conditional_from_discrete_probability_func.py` & `danielutils-0.9.83/danielutils/university/probability/conditional_variable/discrete/conditional_from_discrete_probability_func.py`

 * *Files identical despite different names*

### Comparing `danielutils-0.9.82/danielutils/university/probability/conditional_variable/discrete/discrete.py` & `danielutils-0.9.83/danielutils/university/probability/conditional_variable/discrete/discrete.py`

 * *Files identical despite different names*

### Comparing `danielutils-0.9.82/danielutils/university/probability/conditional_variable/discrete/geometric.py` & `danielutils-0.9.83/danielutils/university/probability/conditional_variable/discrete/geometric.py`

 * *Files identical despite different names*

### Comparing `danielutils-0.9.82/danielutils/university/probability/conditional_variable/discrete/poisson.py` & `danielutils-0.9.83/danielutils/university/probability/conditional_variable/discrete/poisson.py`

 * *Files identical despite different names*

### Comparing `danielutils-0.9.82/danielutils/university/probability/conditional_variable/discrete/uniform.py` & `danielutils-0.9.83/danielutils/university/probability/conditional_variable/discrete/uniform.py`

 * *Files identical despite different names*

### Comparing `danielutils-0.9.82/danielutils/university/probability/distributions.py` & `danielutils-0.9.83/danielutils/university/probability/distributions.py`

 * *Files identical despite different names*

### Comparing `danielutils-0.9.82/danielutils/university/probability/expressions/accumulation_expression.py` & `danielutils-0.9.83/danielutils/university/probability/expressions/accumulation_expression.py`

 * *Files identical despite different names*

### Comparing `danielutils-0.9.82/danielutils/university/probability/expressions/probability_expression.py` & `danielutils-0.9.83/danielutils/university/probability/expressions/probability_expression.py`

 * *Files identical despite different names*

### Comparing `danielutils-0.9.82/danielutils/university/probability/funcs/expected_value.py` & `danielutils-0.9.83/danielutils/university/probability/funcs/expected_value.py`

 * *Files identical despite different names*

### Comparing `danielutils-0.9.82/danielutils/university/probability/operator.py` & `danielutils-0.9.83/danielutils/university/probability/operator.py`

 * *Files identical despite different names*

### Comparing `danielutils-0.9.82/danielutils/university/probability/protocols.py` & `danielutils-0.9.83/danielutils/university/probability/protocols.py`

 * *Files identical despite different names*

### Comparing `danielutils-0.9.82/danielutils/university/probability/supp.py` & `danielutils-0.9.83/danielutils/university/probability/supp.py`

 * *Files identical despite different names*

### Comparing `danielutils-0.9.82/danielutils/university/probability/transformation.py` & `danielutils-0.9.83/danielutils/university/probability/transformation.py`

 * *Files identical despite different names*

### Comparing `danielutils-0.9.82/danielutils.egg-info/PKG-INFO` & `danielutils-0.9.83/danielutils.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: danielutils
-Version: 0.9.82
+Version: 0.9.83
 Summary: A python utils library for things I find useful
 Author-email: danielnachumdev <danielnachumdev@gmail.com>
 License: MIT License
         
         Copyright (c) 2022 danielnachumdev
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -37,15 +37,15 @@
 
 
 [![Python package](https://github.com/danielnachumdev/danielutils/actions/workflows/python-package.yml/badge.svg)](https://github.com/danielnachumdev/danielutils/actions/workflows/python-package.yml)
 [![Pylint](https://github.com/danielnachumdev/danielutils/actions/workflows/pylint.yml/badge.svg)](https://github.com/danielnachumdev/danielutils/actions/workflows/pylint.yml)
 [![Python 3.10.11](https://img.shields.io/badge/python-3.10.11-blue.svg)](https://www.python.org/downloads/release/python-31011/)
 [![gitleaks](https://github.com/danielnachumdev/danielutils/actions/workflows/gitleaks.yml/badge.svg)](https://github.com/danielnachumdev/danielutils/actions/workflows/gitleaks.yml)
 [![CodeQL](https://github.com/danielnachumdev/danielutils/actions/workflows/github-code-scanning/codeql/badge.svg)](https://github.com/danielnachumdev/danielutils/actions/workflows/github-code-scanning/codeql)
-# danielutils v=0.9.82
+# danielutils v=0.9.83
 A utils library for things that I find useful for my coding workflow.\
 Feel free to use and / or contribute / improve my code :)
 
 THIS PACKAGE IS IN DEVELOPMENT AND SUBJECT TO CHANGE, USE AT YOUR OWN RISK!
 
 **Tested python versions**: `3.8.0`*, `3.9.0`, `3.10.13`
```

### Comparing `danielutils-0.9.82/danielutils.egg-info/SOURCES.txt` & `danielutils-0.9.83/danielutils.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -13,15 +13,14 @@
 danielutils/internet.py
 danielutils/io_.py
 danielutils/path.py
 danielutils/print_.py
 danielutils/py.typed
 danielutils/text.py
 danielutils/time.py
-danielutils/tqdm_.py
 danielutils/versioned_imports.py
 danielutils.egg-info/PKG-INFO
 danielutils.egg-info/SOURCES.txt
 danielutils.egg-info/dependency_links.txt
 danielutils.egg-info/top_level.txt
 danielutils/abstractions/__init__.py
 danielutils/abstractions/repl.py
@@ -93,37 +92,40 @@
 danielutils/functions/__init__.py
 danielutils/functions/areoneof.py
 danielutils/functions/check_foreach.py
 danielutils/functions/flatten.py
 danielutils/functions/isoftype.py
 danielutils/functions/isoneof.py
 danielutils/functions/multiloop.py
+danielutils/functions/parallel_for.py
 danielutils/functions/powerset.py
 danielutils/functions/subseteq.py
 danielutils/functions/types_subseteq.py
 danielutils/generators/__init__.py
 danielutils/generators/conditional_generator.py
 danielutils/generators/generator_from_stream.py
 danielutils/generators/join_generators.py
 danielutils/math_/__init__.py
 danielutils/math_/constants.py
 danielutils/math_/functions.py
 danielutils/math_/math_print.py
 danielutils/math_/math_symbols.py
-danielutils/math_/polynomial/__init__.py
-danielutils/math_/polynomial/polinomial.py
 danielutils/metaclasses/__init__.py
 danielutils/metaclasses/atomic_class_meta.py
 danielutils/metaclasses/implicit_data_deleter_meta.py
 danielutils/metaclasses/instance_cache_meta.py
 danielutils/metaclasses/interface.py
 danielutils/metaclasses/overload_meta.py
 danielutils/mock_/__init__.py
 danielutils/mock_/mock_database.py
 danielutils/mock_/mock_module.py
+danielutils/progress_bar/__init__.py
+danielutils/progress_bar/ascii_progress_bar.py
+danielutils/progress_bar/progress_bar.py
+danielutils/progress_bar/progress_bar_pool.py
 danielutils/protocols/__init__.py
 danielutils/protocols/dictable.py
 danielutils/protocols/evaluable.py
 danielutils/reflection/__init__.py
 danielutils/reflection/class_/__init__.py
 danielutils/reflection/class_/class_reflection.py
 danielutils/reflection/file/__init__.py
```

### Comparing `danielutils-0.9.82/pyproject.toml` & `danielutils-0.9.83/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "danielutils"
-version = "0.9.82"
+version = "0.9.83"
 authors = [
     { name = "danielnachumdev", email = "danielnachumdev@gmail.com" },
 ]
 dependencies = []
 keywords = ['functions', 'decorators', 'methods', 'better_builtins', 'metaclasses']
 license = { "file" = "./LICENSE" }
 description = "A python utils library for things I find useful"
```

