# Comparing `tmp/ical-8.0.1.tar.gz` & `tmp/ical-8.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ical-8.0.1.tar", last modified: Sat May 11 00:03:04 2024, max compression
+gzip compressed data, was "ical-8.0.2.tar", last modified: Mon May 13 00:06:06 2024, max compression
```

## Comparing `ical-8.0.1.tar` & `ical-8.0.2.tar`

### file list

```diff
@@ -1,83 +1,84 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 00:03:04.722622 ical-8.0.1/
--rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-05-11 00:03:00.000000 ical-8.0.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     3676 2024-05-11 00:03:04.722622 ical-8.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3170 2024-05-11 00:03:00.000000 ical-8.0.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 00:03:04.714622 ical-8.0.1/ical/
--rw-r--r--   0 runner    (1001) docker     (127)      292 2024-05-11 00:03:00.000000 ical-8.0.1/ical/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3479 2024-05-11 00:03:00.000000 ical-8.0.1/ical/alarm.py
--rw-r--r--   0 runner    (1001) docker     (127)     5075 2024-05-11 00:03:00.000000 ical-8.0.1/ical/calendar.py
--rw-r--r--   0 runner    (1001) docker     (127)     3258 2024-05-11 00:03:00.000000 ical-8.0.1/ical/calendar_stream.py
--rw-r--r--   0 runner    (1001) docker     (127)    13936 2024-05-11 00:03:00.000000 ical-8.0.1/ical/component.py
--rw-r--r--   0 runner    (1001) docker     (127)     1535 2024-05-11 00:03:00.000000 ical-8.0.1/ical/diagnostics.py
--rw-r--r--   0 runner    (1001) docker     (127)    17245 2024-05-11 00:03:00.000000 ical-8.0.1/ical/event.py
--rw-r--r--   0 runner    (1001) docker     (127)      888 2024-05-11 00:03:00.000000 ical-8.0.1/ical/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)     4162 2024-05-11 00:03:00.000000 ical-8.0.1/ical/freebusy.py
--rw-r--r--   0 runner    (1001) docker     (127)    13959 2024-05-11 00:03:00.000000 ical-8.0.1/ical/iter.py
--rw-r--r--   0 runner    (1001) docker     (127)     3728 2024-05-11 00:03:00.000000 ical-8.0.1/ical/journal.py
--rw-r--r--   0 runner    (1001) docker     (127)     2073 2024-05-11 00:03:00.000000 ical-8.0.1/ical/list.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 00:03:04.714622 ical-8.0.1/ical/parsing/
--rw-r--r--   0 runner    (1001) docker     (127)       45 2024-05-11 00:03:00.000000 ical-8.0.1/ical/parsing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4384 2024-05-11 00:03:00.000000 ical-8.0.1/ical/parsing/component.py
--rw-r--r--   0 runner    (1001) docker     (127)      388 2024-05-11 00:03:00.000000 ical-8.0.1/ical/parsing/const.py
--rw-r--r--   0 runner    (1001) docker     (127)   254594 2024-05-11 00:03:00.000000 ical-8.0.1/ical/parsing/emoji.py
--rw-r--r--   0 runner    (1001) docker     (127)     3311 2024-05-11 00:03:00.000000 ical-8.0.1/ical/parsing/parser.py
--rw-r--r--   0 runner    (1001) docker     (127)     3942 2024-05-11 00:03:00.000000 ical-8.0.1/ical/parsing/property.py
--rw-r--r--   0 runner    (1001) docker     (127)     2219 2024-05-11 00:03:00.000000 ical-8.0.1/ical/parsing/unicode.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-11 00:03:00.000000 ical-8.0.1/ical/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)     3652 2024-05-11 00:03:00.000000 ical-8.0.1/ical/recur_adapter.py
--rw-r--r--   0 runner    (1001) docker     (127)    18113 2024-05-11 00:03:00.000000 ical-8.0.1/ical/store.py
--rw-r--r--   0 runner    (1001) docker     (127)     3187 2024-05-11 00:03:00.000000 ical-8.0.1/ical/timeline.py
--rw-r--r--   0 runner    (1001) docker     (127)     4080 2024-05-11 00:03:00.000000 ical-8.0.1/ical/timespan.py
--rw-r--r--   0 runner    (1001) docker     (127)    11840 2024-05-11 00:03:00.000000 ical-8.0.1/ical/timezone.py
--rw-r--r--   0 runner    (1001) docker     (127)    14795 2024-05-11 00:03:00.000000 ical-8.0.1/ical/todo.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 00:03:04.718622 ical-8.0.1/ical/types/
--rw-r--r--   0 runner    (1001) docker     (127)      953 2024-05-11 00:03:00.000000 ical-8.0.1/ical/types/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      811 2024-05-11 00:03:00.000000 ical-8.0.1/ical/types/boolean.py
--rw-r--r--   0 runner    (1001) docker     (127)     3761 2024-05-11 00:03:00.000000 ical-8.0.1/ical/types/cal_address.py
--rw-r--r--   0 runner    (1001) docker     (127)      259 2024-05-11 00:03:00.000000 ical-8.0.1/ical/types/const.py
--rw-r--r--   0 runner    (1001) docker     (127)     6187 2024-05-11 00:03:00.000000 ical-8.0.1/ical/types/data_types.py
--rw-r--r--   0 runner    (1001) docker     (127)     1250 2024-05-11 00:03:00.000000 ical-8.0.1/ical/types/date.py
--rw-r--r--   0 runner    (1001) docker     (127)     3541 2024-05-11 00:03:00.000000 ical-8.0.1/ical/types/date_time.py
--rw-r--r--   0 runner    (1001) docker     (127)     2490 2024-05-11 00:03:00.000000 ical-8.0.1/ical/types/duration.py
--rw-r--r--   0 runner    (1001) docker     (127)      483 2024-05-11 00:03:00.000000 ical-8.0.1/ical/types/float.py
--rw-r--r--   0 runner    (1001) docker     (127)      886 2024-05-11 00:03:00.000000 ical-8.0.1/ical/types/geo.py
--rw-r--r--   0 runner    (1001) docker     (127)      548 2024-05-11 00:03:00.000000 ical-8.0.1/ical/types/integer.py
--rw-r--r--   0 runner    (1001) docker     (127)     1420 2024-05-11 00:03:00.000000 ical-8.0.1/ical/types/parsing.py
--rw-r--r--   0 runner    (1001) docker     (127)     4714 2024-05-11 00:03:00.000000 ical-8.0.1/ical/types/period.py
--rw-r--r--   0 runner    (1001) docker     (127)      735 2024-05-11 00:03:00.000000 ical-8.0.1/ical/types/priority.py
--rw-r--r--   0 runner    (1001) docker     (127)    12760 2024-05-11 00:03:00.000000 ical-8.0.1/ical/types/recur.py
--rw-r--r--   0 runner    (1001) docker     (127)     2276 2024-05-11 00:03:00.000000 ical-8.0.1/ical/types/relation.py
--rw-r--r--   0 runner    (1001) docker     (127)     1250 2024-05-11 00:03:00.000000 ical-8.0.1/ical/types/request_status.py
--rw-r--r--   0 runner    (1001) docker     (127)     1043 2024-05-11 00:03:00.000000 ical-8.0.1/ical/types/text.py
--rw-r--r--   0 runner    (1001) docker     (127)      526 2024-05-11 00:03:00.000000 ical-8.0.1/ical/types/uri.py
--rw-r--r--   0 runner    (1001) docker     (127)     1719 2024-05-11 00:03:00.000000 ical-8.0.1/ical/types/utc_offset.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 00:03:04.718622 ical-8.0.1/ical/tzif/
--rw-r--r--   0 runner    (1001) docker     (127)       41 2024-05-11 00:03:00.000000 ical-8.0.1/ical/tzif/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1381 2024-05-11 00:03:00.000000 ical-8.0.1/ical/tzif/model.py
--rw-r--r--   0 runner    (1001) docker     (127)     5614 2024-05-11 00:03:00.000000 ical-8.0.1/ical/tzif/timezoneinfo.py
--rw-r--r--   0 runner    (1001) docker     (127)     8460 2024-05-11 00:03:00.000000 ical-8.0.1/ical/tzif/tz_rule.py
--rw-r--r--   0 runner    (1001) docker     (127)     9623 2024-05-11 00:03:00.000000 ical-8.0.1/ical/tzif/tzif.py
--rw-r--r--   0 runner    (1001) docker     (127)     1430 2024-05-11 00:03:00.000000 ical-8.0.1/ical/util.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 00:03:04.722622 ical-8.0.1/ical.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3676 2024-05-11 00:03:04.000000 ical-8.0.1/ical.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1634 2024-05-11 00:03:04.000000 ical-8.0.1/ical.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-11 00:03:04.000000 ical-8.0.1/ical.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       71 2024-05-11 00:03:04.000000 ical-8.0.1/ical.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        5 2024-05-11 00:03:04.000000 ical-8.0.1/ical.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      727 2024-05-11 00:03:04.722622 ical-8.0.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)       80 2024-05-11 00:03:00.000000 ical-8.0.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 00:03:04.722622 ical-8.0.1/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     2771 2024-05-11 00:03:00.000000 ical-8.0.1/tests/test_alarm.py
--rw-r--r--   0 runner    (1001) docker     (127)    14362 2024-05-11 00:03:00.000000 ical-8.0.1/tests/test_calendar.py
--rw-r--r--   0 runner    (1001) docker     (127)     4660 2024-05-11 00:03:00.000000 ical-8.0.1/tests/test_calendar_stream.py
--rw-r--r--   0 runner    (1001) docker     (127)     3970 2024-05-11 00:03:00.000000 ical-8.0.1/tests/test_component.py
--rw-r--r--   0 runner    (1001) docker     (127)      736 2024-05-11 00:03:00.000000 ical-8.0.1/tests/test_diagnostics.py
--rw-r--r--   0 runner    (1001) docker     (127)    14361 2024-05-11 00:03:00.000000 ical-8.0.1/tests/test_event.py
--rw-r--r--   0 runner    (1001) docker     (127)     4079 2024-05-11 00:03:00.000000 ical-8.0.1/tests/test_freebusy.py
--rw-r--r--   0 runner    (1001) docker     (127)     4478 2024-05-11 00:03:00.000000 ical-8.0.1/tests/test_iter.py
--rw-r--r--   0 runner    (1001) docker     (127)     1160 2024-05-11 00:03:00.000000 ical-8.0.1/tests/test_journal.py
--rw-r--r--   0 runner    (1001) docker     (127)     3265 2024-05-11 00:03:00.000000 ical-8.0.1/tests/test_list.py
--rw-r--r--   0 runner    (1001) docker     (127)    43647 2024-05-11 00:03:00.000000 ical-8.0.1/tests/test_store.py
--rw-r--r--   0 runner    (1001) docker     (127)     1455 2024-05-11 00:03:00.000000 ical-8.0.1/tests/test_timeline.py
--rw-r--r--   0 runner    (1001) docker     (127)     6576 2024-05-11 00:03:00.000000 ical-8.0.1/tests/test_timezone.py
--rw-r--r--   0 runner    (1001) docker     (127)     9802 2024-05-11 00:03:00.000000 ical-8.0.1/tests/test_todo.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 00:06:06.877480 ical-8.0.2/
+-rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-05-13 00:06:02.000000 ical-8.0.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     3676 2024-05-13 00:06:06.877480 ical-8.0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3170 2024-05-13 00:06:02.000000 ical-8.0.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 00:06:06.869480 ical-8.0.2/ical/
+-rw-r--r--   0 runner    (1001) docker     (127)      292 2024-05-13 00:06:02.000000 ical-8.0.2/ical/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3479 2024-05-13 00:06:02.000000 ical-8.0.2/ical/alarm.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5075 2024-05-13 00:06:02.000000 ical-8.0.2/ical/calendar.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3258 2024-05-13 00:06:02.000000 ical-8.0.2/ical/calendar_stream.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13936 2024-05-13 00:06:02.000000 ical-8.0.2/ical/component.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1535 2024-05-13 00:06:02.000000 ical-8.0.2/ical/diagnostics.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17245 2024-05-13 00:06:02.000000 ical-8.0.2/ical/event.py
+-rw-r--r--   0 runner    (1001) docker     (127)      888 2024-05-13 00:06:02.000000 ical-8.0.2/ical/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4162 2024-05-13 00:06:02.000000 ical-8.0.2/ical/freebusy.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13959 2024-05-13 00:06:02.000000 ical-8.0.2/ical/iter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3728 2024-05-13 00:06:02.000000 ical-8.0.2/ical/journal.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2073 2024-05-13 00:06:02.000000 ical-8.0.2/ical/list.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 00:06:06.869480 ical-8.0.2/ical/parsing/
+-rw-r--r--   0 runner    (1001) docker     (127)       45 2024-05-13 00:06:02.000000 ical-8.0.2/ical/parsing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4384 2024-05-13 00:06:02.000000 ical-8.0.2/ical/parsing/component.py
+-rw-r--r--   0 runner    (1001) docker     (127)      388 2024-05-13 00:06:02.000000 ical-8.0.2/ical/parsing/const.py
+-rw-r--r--   0 runner    (1001) docker     (127)   254594 2024-05-13 00:06:02.000000 ical-8.0.2/ical/parsing/emoji.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3311 2024-05-13 00:06:02.000000 ical-8.0.2/ical/parsing/parser.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3942 2024-05-13 00:06:02.000000 ical-8.0.2/ical/parsing/property.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2219 2024-05-13 00:06:02.000000 ical-8.0.2/ical/parsing/unicode.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-13 00:06:02.000000 ical-8.0.2/ical/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)     3652 2024-05-13 00:06:02.000000 ical-8.0.2/ical/recur_adapter.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18113 2024-05-13 00:06:02.000000 ical-8.0.2/ical/store.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3187 2024-05-13 00:06:02.000000 ical-8.0.2/ical/timeline.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4080 2024-05-13 00:06:02.000000 ical-8.0.2/ical/timespan.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11840 2024-05-13 00:06:02.000000 ical-8.0.2/ical/timezone.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14795 2024-05-13 00:06:02.000000 ical-8.0.2/ical/todo.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 00:06:06.873479 ical-8.0.2/ical/types/
+-rw-r--r--   0 runner    (1001) docker     (127)      953 2024-05-13 00:06:02.000000 ical-8.0.2/ical/types/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      811 2024-05-13 00:06:02.000000 ical-8.0.2/ical/types/boolean.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3761 2024-05-13 00:06:02.000000 ical-8.0.2/ical/types/cal_address.py
+-rw-r--r--   0 runner    (1001) docker     (127)      259 2024-05-13 00:06:02.000000 ical-8.0.2/ical/types/const.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6187 2024-05-13 00:06:02.000000 ical-8.0.2/ical/types/data_types.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1250 2024-05-13 00:06:02.000000 ical-8.0.2/ical/types/date.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3541 2024-05-13 00:06:02.000000 ical-8.0.2/ical/types/date_time.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2490 2024-05-13 00:06:02.000000 ical-8.0.2/ical/types/duration.py
+-rw-r--r--   0 runner    (1001) docker     (127)      483 2024-05-13 00:06:02.000000 ical-8.0.2/ical/types/float.py
+-rw-r--r--   0 runner    (1001) docker     (127)      886 2024-05-13 00:06:02.000000 ical-8.0.2/ical/types/geo.py
+-rw-r--r--   0 runner    (1001) docker     (127)      548 2024-05-13 00:06:02.000000 ical-8.0.2/ical/types/integer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1420 2024-05-13 00:06:02.000000 ical-8.0.2/ical/types/parsing.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4714 2024-05-13 00:06:02.000000 ical-8.0.2/ical/types/period.py
+-rw-r--r--   0 runner    (1001) docker     (127)      735 2024-05-13 00:06:02.000000 ical-8.0.2/ical/types/priority.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12760 2024-05-13 00:06:02.000000 ical-8.0.2/ical/types/recur.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2276 2024-05-13 00:06:02.000000 ical-8.0.2/ical/types/relation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1250 2024-05-13 00:06:02.000000 ical-8.0.2/ical/types/request_status.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1043 2024-05-13 00:06:02.000000 ical-8.0.2/ical/types/text.py
+-rw-r--r--   0 runner    (1001) docker     (127)      526 2024-05-13 00:06:02.000000 ical-8.0.2/ical/types/uri.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1719 2024-05-13 00:06:02.000000 ical-8.0.2/ical/types/utc_offset.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 00:06:06.873479 ical-8.0.2/ical/tzif/
+-rw-r--r--   0 runner    (1001) docker     (127)       41 2024-05-13 00:06:02.000000 ical-8.0.2/ical/tzif/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1381 2024-05-13 00:06:02.000000 ical-8.0.2/ical/tzif/model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5614 2024-05-13 00:06:02.000000 ical-8.0.2/ical/tzif/timezoneinfo.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8460 2024-05-13 00:06:02.000000 ical-8.0.2/ical/tzif/tz_rule.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9623 2024-05-13 00:06:02.000000 ical-8.0.2/ical/tzif/tzif.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1430 2024-05-13 00:06:02.000000 ical-8.0.2/ical/util.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 00:06:06.877480 ical-8.0.2/ical.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3676 2024-05-13 00:06:06.000000 ical-8.0.2/ical.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1649 2024-05-13 00:06:06.000000 ical-8.0.2/ical.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-13 00:06:06.000000 ical-8.0.2/ical.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       71 2024-05-13 00:06:06.000000 ical-8.0.2/ical.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        5 2024-05-13 00:06:06.000000 ical-8.0.2/ical.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      890 2024-05-13 00:06:02.000000 ical-8.0.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      727 2024-05-13 00:06:06.881480 ical-8.0.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)       80 2024-05-13 00:06:02.000000 ical-8.0.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 00:06:06.877480 ical-8.0.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     2771 2024-05-13 00:06:02.000000 ical-8.0.2/tests/test_alarm.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14362 2024-05-13 00:06:02.000000 ical-8.0.2/tests/test_calendar.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4660 2024-05-13 00:06:02.000000 ical-8.0.2/tests/test_calendar_stream.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3970 2024-05-13 00:06:02.000000 ical-8.0.2/tests/test_component.py
+-rw-r--r--   0 runner    (1001) docker     (127)      736 2024-05-13 00:06:02.000000 ical-8.0.2/tests/test_diagnostics.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14361 2024-05-13 00:06:02.000000 ical-8.0.2/tests/test_event.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4079 2024-05-13 00:06:02.000000 ical-8.0.2/tests/test_freebusy.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4478 2024-05-13 00:06:02.000000 ical-8.0.2/tests/test_iter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1160 2024-05-13 00:06:02.000000 ical-8.0.2/tests/test_journal.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3265 2024-05-13 00:06:02.000000 ical-8.0.2/tests/test_list.py
+-rw-r--r--   0 runner    (1001) docker     (127)    43647 2024-05-13 00:06:02.000000 ical-8.0.2/tests/test_store.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1455 2024-05-13 00:06:02.000000 ical-8.0.2/tests/test_timeline.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6576 2024-05-13 00:06:02.000000 ical-8.0.2/tests/test_timezone.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9802 2024-05-13 00:06:02.000000 ical-8.0.2/tests/test_todo.py
```

### Comparing `ical-8.0.1/LICENSE` & `ical-8.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `ical-8.0.1/PKG-INFO` & `ical-8.0.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ical
-Version: 8.0.1
+Version: 8.0.2
 Summary: Python iCalendar implementation (rfc 2445)
 Home-page: https://github.com/allenporter/ical
 Author: Allen Porter
 Author-email: allen.porter@gmail.com
 License: Apache-2.0
 Classifier: License :: OSI Approved :: Apache Software License
 Requires-Python: >=3.10
```

### Comparing `ical-8.0.1/README.md` & `ical-8.0.2/README.md`

 * *Files identical despite different names*

### Comparing `ical-8.0.1/ical/alarm.py` & `ical-8.0.2/ical/alarm.py`

 * *Files identical despite different names*

### Comparing `ical-8.0.1/ical/calendar.py` & `ical-8.0.2/ical/calendar.py`

 * *Files identical despite different names*

### Comparing `ical-8.0.1/ical/calendar_stream.py` & `ical-8.0.2/ical/calendar_stream.py`

 * *Files identical despite different names*

### Comparing `ical-8.0.1/ical/component.py` & `ical-8.0.2/ical/component.py`

 * *Files identical despite different names*

### Comparing `ical-8.0.1/ical/diagnostics.py` & `ical-8.0.2/ical/diagnostics.py`

 * *Files identical despite different names*

### Comparing `ical-8.0.1/ical/event.py` & `ical-8.0.2/ical/event.py`

 * *Files identical despite different names*

### Comparing `ical-8.0.1/ical/exceptions.py` & `ical-8.0.2/ical/exceptions.py`

 * *Files identical despite different names*

### Comparing `ical-8.0.1/ical/freebusy.py` & `ical-8.0.2/ical/freebusy.py`

 * *Files identical despite different names*

### Comparing `ical-8.0.1/ical/iter.py` & `ical-8.0.2/ical/iter.py`

 * *Files identical despite different names*

### Comparing `ical-8.0.1/ical/journal.py` & `ical-8.0.2/ical/journal.py`

 * *Files identical despite different names*

### Comparing `ical-8.0.1/ical/list.py` & `ical-8.0.2/ical/list.py`

 * *Files identical despite different names*

### Comparing `ical-8.0.1/ical/parsing/component.py` & `ical-8.0.2/ical/parsing/component.py`

 * *Files identical despite different names*

### Comparing `ical-8.0.1/ical/parsing/emoji.py` & `ical-8.0.2/ical/parsing/emoji.py`

 * *Files identical despite different names*

### Comparing `ical-8.0.1/ical/parsing/parser.py` & `ical-8.0.2/ical/parsing/parser.py`

 * *Files identical despite different names*

### Comparing `ical-8.0.1/ical/parsing/property.py` & `ical-8.0.2/ical/parsing/property.py`

 * *Files identical despite different names*

### Comparing `ical-8.0.1/ical/parsing/unicode.py` & `ical-8.0.2/ical/parsing/unicode.py`

 * *Files identical despite different names*

### Comparing `ical-8.0.1/ical/recur_adapter.py` & `ical-8.0.2/ical/recur_adapter.py`

 * *Files identical despite different names*

### Comparing `ical-8.0.1/ical/store.py` & `ical-8.0.2/ical/store.py`

 * *Files identical despite different names*

### Comparing `ical-8.0.1/ical/timeline.py` & `ical-8.0.2/ical/timeline.py`

 * *Files identical despite different names*

### Comparing `ical-8.0.1/ical/timespan.py` & `ical-8.0.2/ical/timespan.py`

 * *Files identical despite different names*

### Comparing `ical-8.0.1/ical/timezone.py` & `ical-8.0.2/ical/timezone.py`

 * *Files identical despite different names*

### Comparing `ical-8.0.1/ical/todo.py` & `ical-8.0.2/ical/todo.py`

 * *Files identical despite different names*

### Comparing `ical-8.0.1/ical/types/__init__.py` & `ical-8.0.2/ical/types/__init__.py`

 * *Files identical despite different names*

### Comparing `ical-8.0.1/ical/types/boolean.py` & `ical-8.0.2/ical/types/boolean.py`

 * *Files identical despite different names*

### Comparing `ical-8.0.1/ical/types/cal_address.py` & `ical-8.0.2/ical/types/cal_address.py`

 * *Files identical despite different names*

### Comparing `ical-8.0.1/ical/types/data_types.py` & `ical-8.0.2/ical/types/data_types.py`

 * *Files identical despite different names*

### Comparing `ical-8.0.1/ical/types/date.py` & `ical-8.0.2/ical/types/date.py`

 * *Files identical despite different names*

### Comparing `ical-8.0.1/ical/types/date_time.py` & `ical-8.0.2/ical/types/date_time.py`

 * *Files identical despite different names*

### Comparing `ical-8.0.1/ical/types/duration.py` & `ical-8.0.2/ical/types/duration.py`

 * *Files identical despite different names*

### Comparing `ical-8.0.1/ical/types/geo.py` & `ical-8.0.2/ical/types/geo.py`

 * *Files identical despite different names*

### Comparing `ical-8.0.1/ical/types/integer.py` & `ical-8.0.2/ical/types/integer.py`

 * *Files identical despite different names*

### Comparing `ical-8.0.1/ical/types/parsing.py` & `ical-8.0.2/ical/types/parsing.py`

 * *Files identical despite different names*

### Comparing `ical-8.0.1/ical/types/period.py` & `ical-8.0.2/ical/types/period.py`

 * *Files identical despite different names*

### Comparing `ical-8.0.1/ical/types/priority.py` & `ical-8.0.2/ical/types/priority.py`

 * *Files identical despite different names*

### Comparing `ical-8.0.1/ical/types/recur.py` & `ical-8.0.2/ical/types/recur.py`

 * *Files identical despite different names*

### Comparing `ical-8.0.1/ical/types/relation.py` & `ical-8.0.2/ical/types/relation.py`

 * *Files identical despite different names*

### Comparing `ical-8.0.1/ical/types/request_status.py` & `ical-8.0.2/ical/types/request_status.py`

 * *Files identical despite different names*

### Comparing `ical-8.0.1/ical/types/text.py` & `ical-8.0.2/ical/types/text.py`

 * *Files identical despite different names*

### Comparing `ical-8.0.1/ical/types/uri.py` & `ical-8.0.2/ical/types/uri.py`

 * *Files identical despite different names*

### Comparing `ical-8.0.1/ical/types/utc_offset.py` & `ical-8.0.2/ical/types/utc_offset.py`

 * *Files identical despite different names*

### Comparing `ical-8.0.1/ical/tzif/model.py` & `ical-8.0.2/ical/tzif/model.py`

 * *Files identical despite different names*

### Comparing `ical-8.0.1/ical/tzif/timezoneinfo.py` & `ical-8.0.2/ical/tzif/timezoneinfo.py`

 * *Files identical despite different names*

### Comparing `ical-8.0.1/ical/tzif/tz_rule.py` & `ical-8.0.2/ical/tzif/tz_rule.py`

 * *Files identical despite different names*

### Comparing `ical-8.0.1/ical/tzif/tzif.py` & `ical-8.0.2/ical/tzif/tzif.py`

 * *Files identical despite different names*

### Comparing `ical-8.0.1/ical/util.py` & `ical-8.0.2/ical/util.py`

 * *Files identical despite different names*

### Comparing `ical-8.0.1/ical.egg-info/PKG-INFO` & `ical-8.0.2/ical.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ical
-Version: 8.0.1
+Version: 8.0.2
 Summary: Python iCalendar implementation (rfc 2445)
 Home-page: https://github.com/allenporter/ical
 Author: Allen Porter
 Author-email: allen.porter@gmail.com
 License: Apache-2.0
 Classifier: License :: OSI Approved :: Apache Software License
 Requires-Python: >=3.10
```

### Comparing `ical-8.0.1/ical.egg-info/SOURCES.txt` & `ical-8.0.2/ical.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 LICENSE
 README.md
+pyproject.toml
 setup.cfg
 setup.py
 ./ical/__init__.py
 ./ical/alarm.py
 ./ical/calendar.py
 ./ical/calendar_stream.py
 ./ical/component.py
```

### Comparing `ical-8.0.1/setup.cfg` & `ical-8.0.2/setup.cfg`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = ical
-version = 8.0.1
+version = 8.0.2
 description = Python iCalendar implementation (rfc 2445)
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/allenporter/ical
 author = Allen Porter
 author_email = allen.porter@gmail.com
 license = Apache-2.0
```

### Comparing `ical-8.0.1/tests/test_alarm.py` & `ical-8.0.2/tests/test_alarm.py`

 * *Files identical despite different names*

### Comparing `ical-8.0.1/tests/test_calendar.py` & `ical-8.0.2/tests/test_calendar.py`

 * *Files identical despite different names*

### Comparing `ical-8.0.1/tests/test_calendar_stream.py` & `ical-8.0.2/tests/test_calendar_stream.py`

 * *Files identical despite different names*

### Comparing `ical-8.0.1/tests/test_component.py` & `ical-8.0.2/tests/test_component.py`

 * *Files identical despite different names*

### Comparing `ical-8.0.1/tests/test_diagnostics.py` & `ical-8.0.2/tests/test_diagnostics.py`

 * *Files identical despite different names*

### Comparing `ical-8.0.1/tests/test_event.py` & `ical-8.0.2/tests/test_event.py`

 * *Files identical despite different names*

### Comparing `ical-8.0.1/tests/test_freebusy.py` & `ical-8.0.2/tests/test_freebusy.py`

 * *Files identical despite different names*

### Comparing `ical-8.0.1/tests/test_iter.py` & `ical-8.0.2/tests/test_iter.py`

 * *Files identical despite different names*

### Comparing `ical-8.0.1/tests/test_journal.py` & `ical-8.0.2/tests/test_journal.py`

 * *Files identical despite different names*

### Comparing `ical-8.0.1/tests/test_list.py` & `ical-8.0.2/tests/test_list.py`

 * *Files identical despite different names*

### Comparing `ical-8.0.1/tests/test_store.py` & `ical-8.0.2/tests/test_store.py`

 * *Files identical despite different names*

### Comparing `ical-8.0.1/tests/test_timeline.py` & `ical-8.0.2/tests/test_timeline.py`

 * *Files identical despite different names*

### Comparing `ical-8.0.1/tests/test_timezone.py` & `ical-8.0.2/tests/test_timezone.py`

 * *Files identical despite different names*

### Comparing `ical-8.0.1/tests/test_todo.py` & `ical-8.0.2/tests/test_todo.py`

 * *Files identical despite different names*

