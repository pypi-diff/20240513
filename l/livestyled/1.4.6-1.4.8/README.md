# Comparing `tmp/livestyled-1.4.6.tar.gz` & `tmp/livestyled-1.4.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "livestyled-1.4.6.tar", last modified: Wed Nov 22 16:59:40 2023, max compression
+gzip compressed data, was "livestyled-1.4.8.tar", last modified: Mon May 13 08:42:52 2024, max compression
```

## Comparing `livestyled-1.4.6.tar` & `livestyled-1.4.8.tar`

### file list

```diff
@@ -1,146 +1,147 @@
-drwxr-xr-x   0 tomrutherford   (501) staff       (20)        0 2023-11-22 16:59:40.684407 livestyled-1.4.6/
--rw-r--r--   0 tomrutherford   (501) staff       (20)     1067 2022-11-28 12:03:16.000000 livestyled-1.4.6/LICENSE
--rw-r--r--   0 tomrutherford   (501) staff       (20)      110 2022-11-28 12:03:16.000000 livestyled-1.4.6/MANIFEST.in
--rw-r--r--   0 tomrutherford   (501) staff       (20)      308 2023-11-22 16:59:40.683844 livestyled-1.4.6/PKG-INFO
--rw-r--r--   0 tomrutherford   (501) staff       (20)      268 2022-11-28 12:03:16.000000 livestyled-1.4.6/README.md
-drwxr-xr-x   0 tomrutherford   (501) staff       (20)        0 2023-11-22 16:59:40.593800 livestyled-1.4.6/livestyled/
--rw-r--r--   0 tomrutherford   (501) staff       (20)       22 2023-11-22 16:57:50.000000 livestyled-1.4.6/livestyled/__init__.py
--rw-r--r--   0 tomrutherford   (501) staff       (20)    11599 2022-11-28 12:03:16.000000 livestyled-1.4.6/livestyled/client.py
-drwxr-xr-x   0 tomrutherford   (501) staff       (20)        0 2023-11-22 16:59:40.627431 livestyled-1.4.6/livestyled/models/
--rw-r--r--   0 tomrutherford   (501) staff       (20)     3790 2022-11-28 12:03:16.000000 livestyled-1.4.6/livestyled/models/__init__.py
--rw-r--r--   0 tomrutherford   (501) staff       (20)     1166 2022-11-28 12:03:16.000000 livestyled-1.4.6/livestyled/models/app.py
--rw-r--r--   0 tomrutherford   (501) staff       (20)     1440 2022-11-28 12:03:16.000000 livestyled-1.4.6/livestyled/models/audience.py
--rw-r--r--   0 tomrutherford   (501) staff       (20)     1018 2022-11-28 12:03:16.000000 livestyled-1.4.6/livestyled/models/audience_device.py
--rw-r--r--   0 tomrutherford   (501) staff       (20)     2497 2022-11-28 12:03:16.000000 livestyled-1.4.6/livestyled/models/banner.py
--rw-r--r--   0 tomrutherford   (501) staff       (20)     2578 2022-11-28 12:03:16.000000 livestyled-1.4.6/livestyled/models/booking.py
--rw-r--r--   0 tomrutherford   (501) staff       (20)     1140 2022-11-28 12:03:16.000000 livestyled-1.4.6/livestyled/models/cohort.py
--rw-r--r--   0 tomrutherford   (501) staff       (20)     1306 2022-11-28 12:03:16.000000 livestyled-1.4.6/livestyled/models/competition.py
--rw-r--r--   0 tomrutherford   (501) staff       (20)     1975 2022-11-28 12:03:16.000000 livestyled-1.4.6/livestyled/models/device.py
--rw-r--r--   0 tomrutherford   (501) staff       (20)      680 2022-11-28 12:03:16.000000 livestyled-1.4.6/livestyled/models/device_consent.py
--rw-r--r--   0 tomrutherford   (501) staff       (20)     1924 2022-11-28 12:03:16.000000 livestyled-1.4.6/livestyled/models/device_form_data.py
--rw-r--r--   0 tomrutherford   (501) staff       (20)     2371 2022-11-28 12:03:16.000000 livestyled-1.4.6/livestyled/models/device_preference.py
--rw-r--r--   0 tomrutherford   (501) staff       (20)      408 2022-11-28 12:03:16.000000 livestyled-1.4.6/livestyled/models/device_push_consent.py
--rw-r--r--   0 tomrutherford   (501) staff       (20)     2093 2022-11-28 12:03:16.000000 livestyled-1.4.6/livestyled/models/device_reality.py
--rw-r--r--   0 tomrutherford   (501) staff       (20)     1557 2022-11-28 12:03:16.000000 livestyled-1.4.6/livestyled/models/device_token.py
--rw-r--r--   0 tomrutherford   (501) staff       (20)     2382 2023-11-22 16:57:50.000000 livestyled-1.4.6/livestyled/models/event.py
--rw-r--r--   0 tomrutherford   (501) staff       (20)       30 2022-11-28 12:03:16.000000 livestyled-1.4.6/livestyled/models/event_category.py
--rw-r--r--   0 tomrutherford   (501) staff       (20)      657 2022-11-28 12:03:16.000000 livestyled-1.4.6/livestyled/models/event_date.py
--rw-r--r--   0 tomrutherford   (501) staff       (20)       27 2022-11-28 12:03:16.000000 livestyled-1.4.6/livestyled/models/event_stage.py
--rw-r--r--   0 tomrutherford   (501) staff       (20)     5870 2022-11-28 12:03:16.000000 livestyled-1.4.6/livestyled/models/fixture.py
--rw-r--r--   0 tomrutherford   (501) staff       (20)     4573 2022-11-28 12:03:16.000000 livestyled-1.4.6/livestyled/models/form.py
--rw-r--r--   0 tomrutherford   (501) staff       (20)     2913 2022-11-28 12:03:16.000000 livestyled-1.4.6/livestyled/models/form_field.py
--rw-r--r--   0 tomrutherford   (501) staff       (20)     7288 2023-01-03 11:39:18.000000 livestyled-1.4.6/livestyled/models/fulfilment_point.py
--rw-r--r--   0 tomrutherford   (501) staff       (20)     4768 2022-11-28 12:03:16.000000 livestyled-1.4.6/livestyled/models/league_table.py
--rw-r--r--   0 tomrutherford   (501) staff       (20)     1542 2022-11-28 12:03:16.000000 livestyled-1.4.6/livestyled/models/location.py
--rw-r--r--   0 tomrutherford   (501) staff       (20)     1358 2022-11-28 12:03:16.000000 livestyled-1.4.6/livestyled/models/magic_field.py
--rw-r--r--   0 tomrutherford   (501) staff       (20)     1654 2022-11-28 12:03:16.000000 livestyled-1.4.6/livestyled/models/news.py
--rw-r--r--   0 tomrutherford   (501) staff       (20)     5358 2022-11-28 12:03:16.000000 livestyled-1.4.6/livestyled/models/order.py
--rw-r--r--   0 tomrutherford   (501) staff       (20)    14632 2022-11-28 12:03:16.000000 livestyled-1.4.6/livestyled/models/payment.py
--rw-r--r--   0 tomrutherford   (501) staff       (20)    16830 2023-01-12 13:18:11.000000 livestyled-1.4.6/livestyled/models/product.py
--rw-r--r--   0 tomrutherford   (501) staff       (20)     2475 2022-11-28 12:03:16.000000 livestyled-1.4.6/livestyled/models/push_broadcast.py
--rw-r--r--   0 tomrutherford   (501) staff       (20)     1682 2022-11-28 12:03:16.000000 livestyled-1.4.6/livestyled/models/push_consent.py
--rw-r--r--   0 tomrutherford   (501) staff       (20)     2894 2022-11-28 12:03:16.000000 livestyled-1.4.6/livestyled/models/reality.py
--rw-r--r--   0 tomrutherford   (501) staff       (20)     1875 2022-11-28 12:03:16.000000 livestyled-1.4.6/livestyled/models/screen.py
--rw-r--r--   0 tomrutherford   (501) staff       (20)     1119 2022-11-28 12:03:16.000000 livestyled-1.4.6/livestyled/models/season.py
--rw-r--r--   0 tomrutherford   (501) staff       (20)      654 2022-11-28 12:03:16.000000 livestyled-1.4.6/livestyled/models/sport_venue.py
--rw-r--r--   0 tomrutherford   (501) staff       (20)     1155 2022-11-28 12:03:16.000000 livestyled-1.4.6/livestyled/models/storage.py
--rw-r--r--   0 tomrutherford   (501) staff       (20)     1548 2022-11-28 12:03:16.000000 livestyled-1.4.6/livestyled/models/team.py
-drwxr-xr-x   0 tomrutherford   (501) staff       (20)        0 2023-11-22 16:59:40.633232 livestyled-1.4.6/livestyled/models/tests/
--rw-r--r--   0 tomrutherford   (501) staff       (20)        0 2022-11-28 12:03:16.000000 livestyled-1.4.6/livestyled/models/tests/__init__.py
--rw-r--r--   0 tomrutherford   (501) staff       (20)     1111 2022-11-28 12:03:16.000000 livestyled-1.4.6/livestyled/models/tests/test_device_form_data.py
--rw-r--r--   0 tomrutherford   (501) staff       (20)     1876 2022-11-28 12:03:16.000000 livestyled-1.4.6/livestyled/models/tests/test_fixture.py
--rw-r--r--   0 tomrutherford   (501) staff       (20)     3335 2022-11-28 12:03:16.000000 livestyled-1.4.6/livestyled/models/tests/test_form.py
--rw-r--r--   0 tomrutherford   (501) staff       (20)     2548 2022-11-28 12:03:16.000000 livestyled-1.4.6/livestyled/models/tests/test_form_field.py
--rw-r--r--   0 tomrutherford   (501) staff       (20)      447 2022-11-28 12:03:16.000000 livestyled-1.4.6/livestyled/models/tests/test_order.py
--rw-r--r--   0 tomrutherford   (501) staff       (20)      455 2022-11-28 12:03:16.000000 livestyled-1.4.6/livestyled/models/tests/test_team.py
--rw-r--r--   0 tomrutherford   (501) staff       (20)     5022 2023-07-03 15:42:35.000000 livestyled-1.4.6/livestyled/models/tests/test_ticket.py
--rw-r--r--   0 tomrutherford   (501) staff       (20)    13936 2023-07-03 15:42:35.000000 livestyled-1.4.6/livestyled/models/ticket.py
--rw-r--r--   0 tomrutherford   (501) staff       (20)     2908 2022-11-28 12:03:16.000000 livestyled-1.4.6/livestyled/models/ticket_auth.py
--rw-r--r--   0 tomrutherford   (501) staff       (20)     2504 2023-07-03 16:05:13.000000 livestyled-1.4.6/livestyled/models/ticket_integration.py
--rw-r--r--   0 tomrutherford   (501) staff       (20)     8877 2022-11-28 12:03:16.000000 livestyled-1.4.6/livestyled/models/user.py
--rw-r--r--   0 tomrutherford   (501) staff       (20)      526 2022-11-28 12:03:16.000000 livestyled-1.4.6/livestyled/models/user_cohort.py
--rw-r--r--   0 tomrutherford   (501) staff       (20)     4162 2022-11-28 12:03:16.000000 livestyled-1.4.6/livestyled/models/venue.py
--rw-r--r--   0 tomrutherford   (501) staff       (20)     3676 2022-11-28 12:03:16.000000 livestyled-1.4.6/livestyled/models/widget.py
--rw-r--r--   0 tomrutherford   (501) staff       (20)    48299 2022-11-28 16:23:37.000000 livestyled-1.4.6/livestyled/resource_client.py
-drwxr-xr-x   0 tomrutherford   (501) staff       (20)        0 2023-11-22 16:59:40.662469 livestyled-1.4.6/livestyled/schemas/
--rw-r--r--   0 tomrutherford   (501) staff       (20)     4518 2022-11-28 12:03:16.000000 livestyled-1.4.6/livestyled/schemas/__init__.py
--rw-r--r--   0 tomrutherford   (501) staff       (20)     1809 2022-11-28 12:03:16.000000 livestyled-1.4.6/livestyled/schemas/app.py
--rw-r--r--   0 tomrutherford   (501) staff       (20)     1423 2022-11-28 12:03:16.000000 livestyled-1.4.6/livestyled/schemas/audience.py
--rw-r--r--   0 tomrutherford   (501) staff       (20)      741 2022-11-28 12:03:16.000000 livestyled-1.4.6/livestyled/schemas/audience_device.py
--rw-r--r--   0 tomrutherford   (501) staff       (20)      965 2022-11-28 12:03:16.000000 livestyled-1.4.6/livestyled/schemas/banner.py
--rw-r--r--   0 tomrutherford   (501) staff       (20)      952 2022-11-28 12:03:16.000000 livestyled-1.4.6/livestyled/schemas/booking.py
--rw-r--r--   0 tomrutherford   (501) staff       (20)      485 2022-11-28 12:03:16.000000 livestyled-1.4.6/livestyled/schemas/cohort.py
--rw-r--r--   0 tomrutherford   (501) staff       (20)      589 2022-11-28 12:03:16.000000 livestyled-1.4.6/livestyled/schemas/competition.py
--rw-r--r--   0 tomrutherford   (501) staff       (20)     1714 2022-11-28 12:03:16.000000 livestyled-1.4.6/livestyled/schemas/device.py
--rw-r--r--   0 tomrutherford   (501) staff       (20)      904 2022-11-28 12:03:16.000000 livestyled-1.4.6/livestyled/schemas/device_consent.py
--rw-r--r--   0 tomrutherford   (501) staff       (20)     1044 2022-11-28 12:03:16.000000 livestyled-1.4.6/livestyled/schemas/device_form_data.py
--rw-r--r--   0 tomrutherford   (501) staff       (20)      935 2022-11-28 12:03:16.000000 livestyled-1.4.6/livestyled/schemas/device_preference.py
--rw-r--r--   0 tomrutherford   (501) staff       (20)      939 2022-11-28 12:03:16.000000 livestyled-1.4.6/livestyled/schemas/device_reality.py
--rw-r--r--   0 tomrutherford   (501) staff       (20)      613 2022-11-28 12:03:16.000000 livestyled-1.4.6/livestyled/schemas/device_token.py
--rw-r--r--   0 tomrutherford   (501) staff       (20)     1910 2023-11-22 16:57:50.000000 livestyled-1.4.6/livestyled/schemas/event.py
--rw-r--r--   0 tomrutherford   (501) staff       (20)      832 2022-11-28 12:03:16.000000 livestyled-1.4.6/livestyled/schemas/event_category.py
--rw-r--r--   0 tomrutherford   (501) staff       (20)      875 2022-11-28 12:03:16.000000 livestyled-1.4.6/livestyled/schemas/event_integration.py
--rw-r--r--   0 tomrutherford   (501) staff       (20)      748 2022-11-28 12:03:16.000000 livestyled-1.4.6/livestyled/schemas/event_stage.py
--rw-r--r--   0 tomrutherford   (501) staff       (20)     5097 2022-11-28 12:03:16.000000 livestyled-1.4.6/livestyled/schemas/fields.py
--rw-r--r--   0 tomrutherford   (501) staff       (20)     1857 2022-11-28 12:03:16.000000 livestyled-1.4.6/livestyled/schemas/fixture.py
--rw-r--r--   0 tomrutherford   (501) staff       (20)     1321 2022-11-28 12:03:16.000000 livestyled-1.4.6/livestyled/schemas/form.py
--rw-r--r--   0 tomrutherford   (501) staff       (20)      908 2022-11-28 12:03:16.000000 livestyled-1.4.6/livestyled/schemas/form_field.py
--rw-r--r--   0 tomrutherford   (501) staff       (20)     2416 2023-01-03 11:39:18.000000 livestyled-1.4.6/livestyled/schemas/fulfilment_point.py
--rw-r--r--   0 tomrutherford   (501) staff       (20)     1936 2022-11-28 12:03:16.000000 livestyled-1.4.6/livestyled/schemas/league_table.py
--rw-r--r--   0 tomrutherford   (501) staff       (20)      968 2022-11-28 12:03:16.000000 livestyled-1.4.6/livestyled/schemas/location.py
--rw-r--r--   0 tomrutherford   (501) staff       (20)      539 2022-11-28 12:03:16.000000 livestyled-1.4.6/livestyled/schemas/magic_field.py
--rw-r--r--   0 tomrutherford   (501) staff       (20)     1148 2022-11-28 12:03:16.000000 livestyled-1.4.6/livestyled/schemas/news.py
--rw-r--r--   0 tomrutherford   (501) staff       (20)     2874 2022-11-28 12:03:16.000000 livestyled-1.4.6/livestyled/schemas/order.py
--rw-r--r--   0 tomrutherford   (501) staff       (20)     5094 2022-11-28 12:03:16.000000 livestyled-1.4.6/livestyled/schemas/payment.py
--rw-r--r--   0 tomrutherford   (501) staff       (20)     5968 2022-11-28 12:03:16.000000 livestyled-1.4.6/livestyled/schemas/product.py
--rw-r--r--   0 tomrutherford   (501) staff       (20)     1013 2022-11-28 12:03:16.000000 livestyled-1.4.6/livestyled/schemas/push_broadcast.py
--rw-r--r--   0 tomrutherford   (501) staff       (20)      610 2022-11-28 12:03:16.000000 livestyled-1.4.6/livestyled/schemas/push_consent.py
--rw-r--r--   0 tomrutherford   (501) staff       (20)     1611 2022-11-28 12:03:16.000000 livestyled-1.4.6/livestyled/schemas/reality.py
--rw-r--r--   0 tomrutherford   (501) staff       (20)     1229 2022-11-28 12:03:16.000000 livestyled-1.4.6/livestyled/schemas/screen.py
--rw-r--r--   0 tomrutherford   (501) staff       (20)      442 2022-11-28 12:03:16.000000 livestyled-1.4.6/livestyled/schemas/season.py
--rw-r--r--   0 tomrutherford   (501) staff       (20)      318 2022-11-28 12:03:16.000000 livestyled-1.4.6/livestyled/schemas/sport_venue.py
--rw-r--r--   0 tomrutherford   (501) staff       (20)      481 2022-11-28 12:03:16.000000 livestyled-1.4.6/livestyled/schemas/storage.py
--rw-r--r--   0 tomrutherford   (501) staff       (20)      598 2022-11-28 12:03:16.000000 livestyled-1.4.6/livestyled/schemas/team.py
--rw-r--r--   0 tomrutherford   (501) staff       (20)     5988 2023-07-03 15:42:35.000000 livestyled-1.4.6/livestyled/schemas/ticket.py
--rw-r--r--   0 tomrutherford   (501) staff       (20)     1192 2022-11-28 12:03:16.000000 livestyled-1.4.6/livestyled/schemas/ticket_auth.py
--rw-r--r--   0 tomrutherford   (501) staff       (20)     1077 2022-11-28 12:03:16.000000 livestyled-1.4.6/livestyled/schemas/ticket_integration.py
--rw-r--r--   0 tomrutherford   (501) staff       (20)     4404 2022-11-28 12:03:16.000000 livestyled-1.4.6/livestyled/schemas/user.py
--rw-r--r--   0 tomrutherford   (501) staff       (20)      341 2022-11-28 12:03:16.000000 livestyled-1.4.6/livestyled/schemas/user_cohort.py
--rw-r--r--   0 tomrutherford   (501) staff       (20)       61 2022-11-28 12:03:16.000000 livestyled-1.4.6/livestyled/schemas/utils.py
--rw-r--r--   0 tomrutherford   (501) staff       (20)     1529 2022-11-28 12:03:16.000000 livestyled-1.4.6/livestyled/schemas/venue.py
--rw-r--r--   0 tomrutherford   (501) staff       (20)     1221 2022-11-28 12:03:16.000000 livestyled-1.4.6/livestyled/schemas/widget.py
-drwxr-xr-x   0 tomrutherford   (501) staff       (20)        0 2023-11-22 16:59:40.683018 livestyled-1.4.6/livestyled/tests/
--rw-r--r--   0 tomrutherford   (501) staff       (20)        0 2022-11-28 12:03:16.000000 livestyled-1.4.6/livestyled/tests/__init__.py
--rw-r--r--   0 tomrutherford   (501) staff       (20)     2070 2022-11-28 12:03:16.000000 livestyled-1.4.6/livestyled/tests/test_app.py
--rw-r--r--   0 tomrutherford   (501) staff       (20)     1352 2022-11-28 12:03:16.000000 livestyled-1.4.6/livestyled/tests/test_create_resource_from_data.py
--rw-r--r--   0 tomrutherford   (501) staff       (20)     4421 2022-11-28 12:03:16.000000 livestyled-1.4.6/livestyled/tests/test_device.py
--rw-r--r--   0 tomrutherford   (501) staff       (20)     2646 2022-11-28 16:23:37.000000 livestyled-1.4.6/livestyled/tests/test_resource_audience_device.py
--rw-r--r--   0 tomrutherford   (501) staff       (20)     1637 2022-11-28 12:03:16.000000 livestyled-1.4.6/livestyled/tests/test_resource_banners.py
--rw-r--r--   0 tomrutherford   (501) staff       (20)     3628 2022-11-28 12:03:16.000000 livestyled-1.4.6/livestyled/tests/test_resource_client_bookings.py
--rw-r--r--   0 tomrutherford   (501) staff       (20)      857 2022-11-28 12:03:16.000000 livestyled-1.4.6/livestyled/tests/test_resource_client_device.py
--rw-r--r--   0 tomrutherford   (501) staff       (20)     1107 2022-11-28 12:03:16.000000 livestyled-1.4.6/livestyled/tests/test_resource_client_device_form_data.py
--rw-r--r--   0 tomrutherford   (501) staff       (20)     1431 2022-11-28 12:03:16.000000 livestyled-1.4.6/livestyled/tests/test_resource_client_device_realities.py
--rw-r--r--   0 tomrutherford   (501) staff       (20)     2242 2022-11-28 12:03:16.000000 livestyled-1.4.6/livestyled/tests/test_resource_client_events.py
--rw-r--r--   0 tomrutherford   (501) staff       (20)     2085 2022-11-28 12:03:16.000000 livestyled-1.4.6/livestyled/tests/test_resource_client_fulfilment_points.py
--rw-r--r--   0 tomrutherford   (501) staff       (20)     2596 2022-11-28 12:03:16.000000 livestyled-1.4.6/livestyled/tests/test_resource_client_locations.py
--rw-r--r--   0 tomrutherford   (501) staff       (20)     3128 2022-11-28 12:03:16.000000 livestyled-1.4.6/livestyled/tests/test_resource_client_news.py
--rw-r--r--   0 tomrutherford   (501) staff       (20)     2450 2022-11-28 12:03:16.000000 livestyled-1.4.6/livestyled/tests/test_resource_client_orders.py
--rw-r--r--   0 tomrutherford   (501) staff       (20)     5123 2022-11-28 12:03:16.000000 livestyled-1.4.6/livestyled/tests/test_resource_client_products.py
--rw-r--r--   0 tomrutherford   (501) staff       (20)     4770 2022-11-28 12:03:16.000000 livestyled-1.4.6/livestyled/tests/test_resource_client_teams.py
--rw-r--r--   0 tomrutherford   (501) staff       (20)     7908 2023-07-03 15:42:35.000000 livestyled-1.4.6/livestyled/tests/test_resource_client_ticket.py
--rw-r--r--   0 tomrutherford   (501) staff       (20)     3362 2022-11-28 12:03:16.000000 livestyled-1.4.6/livestyled/tests/test_resource_client_ticket_auths.py
--rw-r--r--   0 tomrutherford   (501) staff       (20)     2719 2022-11-28 12:03:16.000000 livestyled-1.4.6/livestyled/tests/test_resource_client_user.py
--rw-r--r--   0 tomrutherford   (501) staff       (20)     3103 2022-11-28 12:03:16.000000 livestyled-1.4.6/livestyled/tests/test_resource_device_preferences.py
--rw-r--r--   0 tomrutherford   (501) staff       (20)     2010 2022-11-28 12:03:16.000000 livestyled-1.4.6/livestyled/tests/test_resource_screens.py
--rw-r--r--   0 tomrutherford   (501) staff       (20)     2055 2022-11-28 12:03:16.000000 livestyled-1.4.6/livestyled/tests/test_resource_widgets.py
--rw-r--r--   0 tomrutherford   (501) staff       (20)      658 2022-11-28 12:03:16.000000 livestyled-1.4.6/livestyled/tests/utils.py
--rw-r--r--   0 tomrutherford   (501) staff       (20)      411 2022-11-28 12:03:16.000000 livestyled-1.4.6/livestyled/utils.py
-drwxr-xr-x   0 tomrutherford   (501) staff       (20)        0 2023-11-22 16:59:40.596174 livestyled-1.4.6/livestyled.egg-info/
--rw-r--r--   0 tomrutherford   (501) staff       (20)      308 2023-11-22 16:59:40.000000 livestyled-1.4.6/livestyled.egg-info/PKG-INFO
--rw-r--r--   0 tomrutherford   (501) staff       (20)     4633 2023-11-22 16:59:40.000000 livestyled-1.4.6/livestyled.egg-info/SOURCES.txt
--rw-r--r--   0 tomrutherford   (501) staff       (20)        1 2023-11-22 16:59:40.000000 livestyled-1.4.6/livestyled.egg-info/dependency_links.txt
--rw-r--r--   0 tomrutherford   (501) staff       (20)       68 2023-11-22 16:59:40.000000 livestyled-1.4.6/livestyled.egg-info/requires.txt
--rw-r--r--   0 tomrutherford   (501) staff       (20)       11 2023-11-22 16:59:40.000000 livestyled-1.4.6/livestyled.egg-info/top_level.txt
--rw-r--r--   0 tomrutherford   (501) staff       (20)       68 2022-11-28 12:03:16.000000 livestyled-1.4.6/requirements.txt
--rw-r--r--   0 tomrutherford   (501) staff       (20)       38 2023-11-22 16:59:40.684507 livestyled-1.4.6/setup.cfg
--rw-r--r--   0 tomrutherford   (501) staff       (20)     1338 2022-11-28 12:03:16.000000 livestyled-1.4.6/setup.py
+drwxr-xr-x   0 tomrutherford   (501) staff       (20)        0 2024-05-13 08:42:52.988462 livestyled-1.4.8/
+-rw-r--r--   0 tomrutherford   (501) staff       (20)     1067 2022-11-28 12:03:16.000000 livestyled-1.4.8/LICENSE
+-rw-r--r--   0 tomrutherford   (501) staff       (20)      110 2022-11-28 12:03:16.000000 livestyled-1.4.8/MANIFEST.in
+-rw-r--r--   0 tomrutherford   (501) staff       (20)      242 2024-05-13 08:42:52.987940 livestyled-1.4.8/PKG-INFO
+-rw-r--r--   0 tomrutherford   (501) staff       (20)      268 2022-11-28 12:03:16.000000 livestyled-1.4.8/README.md
+drwxr-xr-x   0 tomrutherford   (501) staff       (20)        0 2024-05-13 08:42:52.855915 livestyled-1.4.8/livestyled/
+-rw-r--r--   0 tomrutherford   (501) staff       (20)       22 2024-05-13 08:24:16.000000 livestyled-1.4.8/livestyled/__init__.py
+-rw-r--r--   0 tomrutherford   (501) staff       (20)    11599 2022-11-28 12:03:16.000000 livestyled-1.4.8/livestyled/client.py
+drwxr-xr-x   0 tomrutherford   (501) staff       (20)        0 2024-05-13 08:42:52.902459 livestyled-1.4.8/livestyled/models/
+-rw-r--r--   0 tomrutherford   (501) staff       (20)     3790 2022-11-28 12:03:16.000000 livestyled-1.4.8/livestyled/models/__init__.py
+-rw-r--r--   0 tomrutherford   (501) staff       (20)     1166 2022-11-28 12:03:16.000000 livestyled-1.4.8/livestyled/models/app.py
+-rw-r--r--   0 tomrutherford   (501) staff       (20)     1440 2022-11-28 12:03:16.000000 livestyled-1.4.8/livestyled/models/audience.py
+-rw-r--r--   0 tomrutherford   (501) staff       (20)     1018 2022-11-28 12:03:16.000000 livestyled-1.4.8/livestyled/models/audience_device.py
+-rw-r--r--   0 tomrutherford   (501) staff       (20)     2497 2022-11-28 12:03:16.000000 livestyled-1.4.8/livestyled/models/banner.py
+-rw-r--r--   0 tomrutherford   (501) staff       (20)     2578 2022-11-28 12:03:16.000000 livestyled-1.4.8/livestyled/models/booking.py
+-rw-r--r--   0 tomrutherford   (501) staff       (20)     1140 2022-11-28 12:03:16.000000 livestyled-1.4.8/livestyled/models/cohort.py
+-rw-r--r--   0 tomrutherford   (501) staff       (20)     1306 2022-11-28 12:03:16.000000 livestyled-1.4.8/livestyled/models/competition.py
+-rw-r--r--   0 tomrutherford   (501) staff       (20)     1975 2022-11-28 12:03:16.000000 livestyled-1.4.8/livestyled/models/device.py
+-rw-r--r--   0 tomrutherford   (501) staff       (20)      680 2022-11-28 12:03:16.000000 livestyled-1.4.8/livestyled/models/device_consent.py
+-rw-r--r--   0 tomrutherford   (501) staff       (20)     1924 2022-11-28 12:03:16.000000 livestyled-1.4.8/livestyled/models/device_form_data.py
+-rw-r--r--   0 tomrutherford   (501) staff       (20)     2371 2022-11-28 12:03:16.000000 livestyled-1.4.8/livestyled/models/device_preference.py
+-rw-r--r--   0 tomrutherford   (501) staff       (20)      408 2022-11-28 12:03:16.000000 livestyled-1.4.8/livestyled/models/device_push_consent.py
+-rw-r--r--   0 tomrutherford   (501) staff       (20)     2093 2022-11-28 12:03:16.000000 livestyled-1.4.8/livestyled/models/device_reality.py
+-rw-r--r--   0 tomrutherford   (501) staff       (20)     1557 2022-11-28 12:03:16.000000 livestyled-1.4.8/livestyled/models/device_token.py
+-rw-r--r--   0 tomrutherford   (501) staff       (20)     2382 2023-11-22 16:57:50.000000 livestyled-1.4.8/livestyled/models/event.py
+-rw-r--r--   0 tomrutherford   (501) staff       (20)       30 2022-11-28 12:03:16.000000 livestyled-1.4.8/livestyled/models/event_category.py
+-rw-r--r--   0 tomrutherford   (501) staff       (20)      657 2022-11-28 12:03:16.000000 livestyled-1.4.8/livestyled/models/event_date.py
+-rw-r--r--   0 tomrutherford   (501) staff       (20)       27 2022-11-28 12:03:16.000000 livestyled-1.4.8/livestyled/models/event_stage.py
+-rw-r--r--   0 tomrutherford   (501) staff       (20)     5870 2022-11-28 12:03:16.000000 livestyled-1.4.8/livestyled/models/fixture.py
+-rw-r--r--   0 tomrutherford   (501) staff       (20)     4573 2022-11-28 12:03:16.000000 livestyled-1.4.8/livestyled/models/form.py
+-rw-r--r--   0 tomrutherford   (501) staff       (20)     2913 2022-11-28 12:03:16.000000 livestyled-1.4.8/livestyled/models/form_field.py
+-rw-r--r--   0 tomrutherford   (501) staff       (20)     7288 2023-01-03 11:39:18.000000 livestyled-1.4.8/livestyled/models/fulfilment_point.py
+-rw-r--r--   0 tomrutherford   (501) staff       (20)     4768 2022-11-28 12:03:16.000000 livestyled-1.4.8/livestyled/models/league_table.py
+-rw-r--r--   0 tomrutherford   (501) staff       (20)     1542 2022-11-28 12:03:16.000000 livestyled-1.4.8/livestyled/models/location.py
+-rw-r--r--   0 tomrutherford   (501) staff       (20)     1358 2022-11-28 12:03:16.000000 livestyled-1.4.8/livestyled/models/magic_field.py
+-rw-r--r--   0 tomrutherford   (501) staff       (20)     1654 2022-11-28 12:03:16.000000 livestyled-1.4.8/livestyled/models/news.py
+-rw-r--r--   0 tomrutherford   (501) staff       (20)     5358 2022-11-28 12:03:16.000000 livestyled-1.4.8/livestyled/models/order.py
+-rw-r--r--   0 tomrutherford   (501) staff       (20)    14632 2022-11-28 12:03:16.000000 livestyled-1.4.8/livestyled/models/payment.py
+-rw-r--r--   0 tomrutherford   (501) staff       (20)    16830 2023-01-12 13:18:11.000000 livestyled-1.4.8/livestyled/models/product.py
+-rw-r--r--   0 tomrutherford   (501) staff       (20)     2475 2022-11-28 12:03:16.000000 livestyled-1.4.8/livestyled/models/push_broadcast.py
+-rw-r--r--   0 tomrutherford   (501) staff       (20)     1682 2022-11-28 12:03:16.000000 livestyled-1.4.8/livestyled/models/push_consent.py
+-rw-r--r--   0 tomrutherford   (501) staff       (20)     2894 2022-11-28 12:03:16.000000 livestyled-1.4.8/livestyled/models/reality.py
+-rw-r--r--   0 tomrutherford   (501) staff       (20)     1875 2022-11-28 12:03:16.000000 livestyled-1.4.8/livestyled/models/screen.py
+-rw-r--r--   0 tomrutherford   (501) staff       (20)     1119 2022-11-28 12:03:16.000000 livestyled-1.4.8/livestyled/models/season.py
+-rw-r--r--   0 tomrutherford   (501) staff       (20)      654 2022-11-28 12:03:16.000000 livestyled-1.4.8/livestyled/models/sport_venue.py
+-rw-r--r--   0 tomrutherford   (501) staff       (20)     1155 2022-11-28 12:03:16.000000 livestyled-1.4.8/livestyled/models/storage.py
+-rw-r--r--   0 tomrutherford   (501) staff       (20)     1548 2022-11-28 12:03:16.000000 livestyled-1.4.8/livestyled/models/team.py
+drwxr-xr-x   0 tomrutherford   (501) staff       (20)        0 2024-05-13 08:42:52.910556 livestyled-1.4.8/livestyled/models/tests/
+-rw-r--r--   0 tomrutherford   (501) staff       (20)        0 2022-11-28 12:03:16.000000 livestyled-1.4.8/livestyled/models/tests/__init__.py
+-rw-r--r--   0 tomrutherford   (501) staff       (20)     1111 2022-11-28 12:03:16.000000 livestyled-1.4.8/livestyled/models/tests/test_device_form_data.py
+-rw-r--r--   0 tomrutherford   (501) staff       (20)     1876 2022-11-28 12:03:16.000000 livestyled-1.4.8/livestyled/models/tests/test_fixture.py
+-rw-r--r--   0 tomrutherford   (501) staff       (20)     3335 2022-11-28 12:03:16.000000 livestyled-1.4.8/livestyled/models/tests/test_form.py
+-rw-r--r--   0 tomrutherford   (501) staff       (20)     2548 2022-11-28 12:03:16.000000 livestyled-1.4.8/livestyled/models/tests/test_form_field.py
+-rw-r--r--   0 tomrutherford   (501) staff       (20)      447 2022-11-28 12:03:16.000000 livestyled-1.4.8/livestyled/models/tests/test_order.py
+-rw-r--r--   0 tomrutherford   (501) staff       (20)      455 2022-11-28 12:03:16.000000 livestyled-1.4.8/livestyled/models/tests/test_team.py
+-rw-r--r--   0 tomrutherford   (501) staff       (20)     5022 2023-07-03 15:42:35.000000 livestyled-1.4.8/livestyled/models/tests/test_ticket.py
+-rw-r--r--   0 tomrutherford   (501) staff       (20)    14123 2024-05-13 08:24:09.000000 livestyled-1.4.8/livestyled/models/ticket.py
+-rw-r--r--   0 tomrutherford   (501) staff       (20)     2908 2022-11-28 12:03:16.000000 livestyled-1.4.8/livestyled/models/ticket_auth.py
+-rw-r--r--   0 tomrutherford   (501) staff       (20)     2504 2023-07-03 16:05:13.000000 livestyled-1.4.8/livestyled/models/ticket_integration.py
+-rw-r--r--   0 tomrutherford   (501) staff       (20)     8877 2022-11-28 12:03:16.000000 livestyled-1.4.8/livestyled/models/user.py
+-rw-r--r--   0 tomrutherford   (501) staff       (20)      526 2022-11-28 12:03:16.000000 livestyled-1.4.8/livestyled/models/user_cohort.py
+-rw-r--r--   0 tomrutherford   (501) staff       (20)     4162 2022-11-28 12:03:16.000000 livestyled-1.4.8/livestyled/models/venue.py
+-rw-r--r--   0 tomrutherford   (501) staff       (20)     3676 2022-11-28 12:03:16.000000 livestyled-1.4.8/livestyled/models/widget.py
+-rw-r--r--   0 tomrutherford   (501) staff       (20)    48299 2022-11-28 16:23:37.000000 livestyled-1.4.8/livestyled/resource_client.py
+drwxr-xr-x   0 tomrutherford   (501) staff       (20)        0 2024-05-13 08:42:52.964500 livestyled-1.4.8/livestyled/schemas/
+-rw-r--r--   0 tomrutherford   (501) staff       (20)     4518 2022-11-28 12:03:16.000000 livestyled-1.4.8/livestyled/schemas/__init__.py
+-rw-r--r--   0 tomrutherford   (501) staff       (20)     1809 2022-11-28 12:03:16.000000 livestyled-1.4.8/livestyled/schemas/app.py
+-rw-r--r--   0 tomrutherford   (501) staff       (20)     1423 2022-11-28 12:03:16.000000 livestyled-1.4.8/livestyled/schemas/audience.py
+-rw-r--r--   0 tomrutherford   (501) staff       (20)      741 2022-11-28 12:03:16.000000 livestyled-1.4.8/livestyled/schemas/audience_device.py
+-rw-r--r--   0 tomrutherford   (501) staff       (20)      965 2022-11-28 12:03:16.000000 livestyled-1.4.8/livestyled/schemas/banner.py
+-rw-r--r--   0 tomrutherford   (501) staff       (20)      952 2022-11-28 12:03:16.000000 livestyled-1.4.8/livestyled/schemas/booking.py
+-rw-r--r--   0 tomrutherford   (501) staff       (20)      485 2022-11-28 12:03:16.000000 livestyled-1.4.8/livestyled/schemas/cohort.py
+-rw-r--r--   0 tomrutherford   (501) staff       (20)      589 2022-11-28 12:03:16.000000 livestyled-1.4.8/livestyled/schemas/competition.py
+-rw-r--r--   0 tomrutherford   (501) staff       (20)     1714 2022-11-28 12:03:16.000000 livestyled-1.4.8/livestyled/schemas/device.py
+-rw-r--r--   0 tomrutherford   (501) staff       (20)      904 2022-11-28 12:03:16.000000 livestyled-1.4.8/livestyled/schemas/device_consent.py
+-rw-r--r--   0 tomrutherford   (501) staff       (20)     1044 2022-11-28 12:03:16.000000 livestyled-1.4.8/livestyled/schemas/device_form_data.py
+-rw-r--r--   0 tomrutherford   (501) staff       (20)      935 2022-11-28 12:03:16.000000 livestyled-1.4.8/livestyled/schemas/device_preference.py
+-rw-r--r--   0 tomrutherford   (501) staff       (20)      939 2022-11-28 12:03:16.000000 livestyled-1.4.8/livestyled/schemas/device_reality.py
+-rw-r--r--   0 tomrutherford   (501) staff       (20)      613 2022-11-28 12:03:16.000000 livestyled-1.4.8/livestyled/schemas/device_token.py
+-rw-r--r--   0 tomrutherford   (501) staff       (20)     1910 2023-11-22 16:57:50.000000 livestyled-1.4.8/livestyled/schemas/event.py
+-rw-r--r--   0 tomrutherford   (501) staff       (20)      832 2022-11-28 12:03:16.000000 livestyled-1.4.8/livestyled/schemas/event_category.py
+-rw-r--r--   0 tomrutherford   (501) staff       (20)      875 2022-11-28 12:03:16.000000 livestyled-1.4.8/livestyled/schemas/event_integration.py
+-rw-r--r--   0 tomrutherford   (501) staff       (20)      748 2022-11-28 12:03:16.000000 livestyled-1.4.8/livestyled/schemas/event_stage.py
+-rw-r--r--   0 tomrutherford   (501) staff       (20)     5097 2022-11-28 12:03:16.000000 livestyled-1.4.8/livestyled/schemas/fields.py
+-rw-r--r--   0 tomrutherford   (501) staff       (20)     1857 2022-11-28 12:03:16.000000 livestyled-1.4.8/livestyled/schemas/fixture.py
+-rw-r--r--   0 tomrutherford   (501) staff       (20)     1321 2022-11-28 12:03:16.000000 livestyled-1.4.8/livestyled/schemas/form.py
+-rw-r--r--   0 tomrutherford   (501) staff       (20)      908 2022-11-28 12:03:16.000000 livestyled-1.4.8/livestyled/schemas/form_field.py
+-rw-r--r--   0 tomrutherford   (501) staff       (20)     2416 2023-01-03 11:39:18.000000 livestyled-1.4.8/livestyled/schemas/fulfilment_point.py
+-rw-r--r--   0 tomrutherford   (501) staff       (20)     1936 2022-11-28 12:03:16.000000 livestyled-1.4.8/livestyled/schemas/league_table.py
+-rw-r--r--   0 tomrutherford   (501) staff       (20)      968 2022-11-28 12:03:16.000000 livestyled-1.4.8/livestyled/schemas/location.py
+-rw-r--r--   0 tomrutherford   (501) staff       (20)      539 2022-11-28 12:03:16.000000 livestyled-1.4.8/livestyled/schemas/magic_field.py
+-rw-r--r--   0 tomrutherford   (501) staff       (20)     1148 2022-11-28 12:03:16.000000 livestyled-1.4.8/livestyled/schemas/news.py
+-rw-r--r--   0 tomrutherford   (501) staff       (20)     2874 2022-11-28 12:03:16.000000 livestyled-1.4.8/livestyled/schemas/order.py
+-rw-r--r--   0 tomrutherford   (501) staff       (20)     5094 2022-11-28 12:03:16.000000 livestyled-1.4.8/livestyled/schemas/payment.py
+-rw-r--r--   0 tomrutherford   (501) staff       (20)     5968 2022-11-28 12:03:16.000000 livestyled-1.4.8/livestyled/schemas/product.py
+-rw-r--r--   0 tomrutherford   (501) staff       (20)     1013 2022-11-28 12:03:16.000000 livestyled-1.4.8/livestyled/schemas/push_broadcast.py
+-rw-r--r--   0 tomrutherford   (501) staff       (20)      610 2022-11-28 12:03:16.000000 livestyled-1.4.8/livestyled/schemas/push_consent.py
+-rw-r--r--   0 tomrutherford   (501) staff       (20)     1611 2022-11-28 12:03:16.000000 livestyled-1.4.8/livestyled/schemas/reality.py
+-rw-r--r--   0 tomrutherford   (501) staff       (20)     1229 2022-11-28 12:03:16.000000 livestyled-1.4.8/livestyled/schemas/screen.py
+-rw-r--r--   0 tomrutherford   (501) staff       (20)      442 2022-11-28 12:03:16.000000 livestyled-1.4.8/livestyled/schemas/season.py
+-rw-r--r--   0 tomrutherford   (501) staff       (20)      318 2022-11-28 12:03:16.000000 livestyled-1.4.8/livestyled/schemas/sport_venue.py
+-rw-r--r--   0 tomrutherford   (501) staff       (20)      481 2022-11-28 12:03:16.000000 livestyled-1.4.8/livestyled/schemas/storage.py
+-rw-r--r--   0 tomrutherford   (501) staff       (20)      598 2022-11-28 12:03:16.000000 livestyled-1.4.8/livestyled/schemas/team.py
+-rw-r--r--   0 tomrutherford   (501) staff       (20)     6077 2024-05-13 08:24:09.000000 livestyled-1.4.8/livestyled/schemas/ticket.py
+-rw-r--r--   0 tomrutherford   (501) staff       (20)     1192 2022-11-28 12:03:16.000000 livestyled-1.4.8/livestyled/schemas/ticket_auth.py
+-rw-r--r--   0 tomrutherford   (501) staff       (20)     1077 2022-11-28 12:03:16.000000 livestyled-1.4.8/livestyled/schemas/ticket_integration.py
+-rw-r--r--   0 tomrutherford   (501) staff       (20)     4404 2022-11-28 12:03:16.000000 livestyled-1.4.8/livestyled/schemas/user.py
+-rw-r--r--   0 tomrutherford   (501) staff       (20)      341 2022-11-28 12:03:16.000000 livestyled-1.4.8/livestyled/schemas/user_cohort.py
+-rw-r--r--   0 tomrutherford   (501) staff       (20)       61 2022-11-28 12:03:16.000000 livestyled-1.4.8/livestyled/schemas/utils.py
+-rw-r--r--   0 tomrutherford   (501) staff       (20)     1529 2022-11-28 12:03:16.000000 livestyled-1.4.8/livestyled/schemas/venue.py
+-rw-r--r--   0 tomrutherford   (501) staff       (20)     1221 2022-11-28 12:03:16.000000 livestyled-1.4.8/livestyled/schemas/widget.py
+drwxr-xr-x   0 tomrutherford   (501) staff       (20)        0 2024-05-13 08:42:52.986756 livestyled-1.4.8/livestyled/tests/
+-rw-r--r--   0 tomrutherford   (501) staff       (20)        0 2022-11-28 12:03:16.000000 livestyled-1.4.8/livestyled/tests/__init__.py
+-rw-r--r--   0 tomrutherford   (501) staff       (20)     2070 2022-11-28 12:03:16.000000 livestyled-1.4.8/livestyled/tests/test_app.py
+-rw-r--r--   0 tomrutherford   (501) staff       (20)     1352 2022-11-28 12:03:16.000000 livestyled-1.4.8/livestyled/tests/test_create_resource_from_data.py
+-rw-r--r--   0 tomrutherford   (501) staff       (20)     4421 2022-11-28 12:03:16.000000 livestyled-1.4.8/livestyled/tests/test_device.py
+-rw-r--r--   0 tomrutherford   (501) staff       (20)     2646 2022-11-28 16:23:37.000000 livestyled-1.4.8/livestyled/tests/test_resource_audience_device.py
+-rw-r--r--   0 tomrutherford   (501) staff       (20)     1637 2022-11-28 12:03:16.000000 livestyled-1.4.8/livestyled/tests/test_resource_banners.py
+-rw-r--r--   0 tomrutherford   (501) staff       (20)     3628 2022-11-28 12:03:16.000000 livestyled-1.4.8/livestyled/tests/test_resource_client_bookings.py
+-rw-r--r--   0 tomrutherford   (501) staff       (20)      857 2022-11-28 12:03:16.000000 livestyled-1.4.8/livestyled/tests/test_resource_client_device.py
+-rw-r--r--   0 tomrutherford   (501) staff       (20)     1107 2022-11-28 12:03:16.000000 livestyled-1.4.8/livestyled/tests/test_resource_client_device_form_data.py
+-rw-r--r--   0 tomrutherford   (501) staff       (20)     1431 2022-11-28 12:03:16.000000 livestyled-1.4.8/livestyled/tests/test_resource_client_device_realities.py
+-rw-r--r--   0 tomrutherford   (501) staff       (20)     2242 2022-11-28 12:03:16.000000 livestyled-1.4.8/livestyled/tests/test_resource_client_events.py
+-rw-r--r--   0 tomrutherford   (501) staff       (20)     2085 2022-11-28 12:03:16.000000 livestyled-1.4.8/livestyled/tests/test_resource_client_fulfilment_points.py
+-rw-r--r--   0 tomrutherford   (501) staff       (20)     2596 2022-11-28 12:03:16.000000 livestyled-1.4.8/livestyled/tests/test_resource_client_locations.py
+-rw-r--r--   0 tomrutherford   (501) staff       (20)     3128 2022-11-28 12:03:16.000000 livestyled-1.4.8/livestyled/tests/test_resource_client_news.py
+-rw-r--r--   0 tomrutherford   (501) staff       (20)     2450 2022-11-28 12:03:16.000000 livestyled-1.4.8/livestyled/tests/test_resource_client_orders.py
+-rw-r--r--   0 tomrutherford   (501) staff       (20)     5123 2022-11-28 12:03:16.000000 livestyled-1.4.8/livestyled/tests/test_resource_client_products.py
+-rw-r--r--   0 tomrutherford   (501) staff       (20)     4770 2022-11-28 12:03:16.000000 livestyled-1.4.8/livestyled/tests/test_resource_client_teams.py
+-rw-r--r--   0 tomrutherford   (501) staff       (20)     8066 2024-05-13 08:24:09.000000 livestyled-1.4.8/livestyled/tests/test_resource_client_ticket.py
+-rw-r--r--   0 tomrutherford   (501) staff       (20)     3362 2022-11-28 12:03:16.000000 livestyled-1.4.8/livestyled/tests/test_resource_client_ticket_auths.py
+-rw-r--r--   0 tomrutherford   (501) staff       (20)     2719 2022-11-28 12:03:16.000000 livestyled-1.4.8/livestyled/tests/test_resource_client_user.py
+-rw-r--r--   0 tomrutherford   (501) staff       (20)     3103 2022-11-28 12:03:16.000000 livestyled-1.4.8/livestyled/tests/test_resource_device_preferences.py
+-rw-r--r--   0 tomrutherford   (501) staff       (20)     2010 2022-11-28 12:03:16.000000 livestyled-1.4.8/livestyled/tests/test_resource_screens.py
+-rw-r--r--   0 tomrutherford   (501) staff       (20)     2055 2022-11-28 12:03:16.000000 livestyled-1.4.8/livestyled/tests/test_resource_widgets.py
+-rw-r--r--   0 tomrutherford   (501) staff       (20)      658 2022-11-28 12:03:16.000000 livestyled-1.4.8/livestyled/tests/utils.py
+-rw-r--r--   0 tomrutherford   (501) staff       (20)      411 2022-11-28 12:03:16.000000 livestyled-1.4.8/livestyled/utils.py
+drwxr-xr-x   0 tomrutherford   (501) staff       (20)        0 2024-05-13 08:42:52.859992 livestyled-1.4.8/livestyled.egg-info/
+-rw-r--r--   0 tomrutherford   (501) staff       (20)      242 2024-05-13 08:42:52.000000 livestyled-1.4.8/livestyled.egg-info/PKG-INFO
+-rw-r--r--   0 tomrutherford   (501) staff       (20)     4670 2024-05-13 08:42:52.000000 livestyled-1.4.8/livestyled.egg-info/SOURCES.txt
+-rw-r--r--   0 tomrutherford   (501) staff       (20)        1 2024-05-13 08:42:52.000000 livestyled-1.4.8/livestyled.egg-info/dependency_links.txt
+-rw-r--r--   0 tomrutherford   (501) staff       (20)       27 2024-05-13 08:42:52.000000 livestyled-1.4.8/livestyled.egg-info/entry_points.txt
+-rw-r--r--   0 tomrutherford   (501) staff       (20)       68 2024-05-13 08:42:52.000000 livestyled-1.4.8/livestyled.egg-info/requires.txt
+-rw-r--r--   0 tomrutherford   (501) staff       (20)       11 2024-05-13 08:42:52.000000 livestyled-1.4.8/livestyled.egg-info/top_level.txt
+-rw-r--r--   0 tomrutherford   (501) staff       (20)       68 2022-11-28 12:03:16.000000 livestyled-1.4.8/requirements.txt
+-rw-r--r--   0 tomrutherford   (501) staff       (20)       38 2024-05-13 08:42:52.988645 livestyled-1.4.8/setup.cfg
+-rw-r--r--   0 tomrutherford   (501) staff       (20)     1338 2022-11-28 12:03:16.000000 livestyled-1.4.8/setup.py
```

### Comparing `livestyled-1.4.6/LICENSE` & `livestyled-1.4.8/LICENSE`

 * *Files identical despite different names*

### Comparing `livestyled-1.4.6/livestyled/client.py` & `livestyled-1.4.8/livestyled/client.py`

 * *Files identical despite different names*

### Comparing `livestyled-1.4.6/livestyled/models/__init__.py` & `livestyled-1.4.8/livestyled/models/__init__.py`

 * *Files identical despite different names*

### Comparing `livestyled-1.4.6/livestyled/models/app.py` & `livestyled-1.4.8/livestyled/models/app.py`

 * *Files identical despite different names*

### Comparing `livestyled-1.4.6/livestyled/models/audience.py` & `livestyled-1.4.8/livestyled/models/audience.py`

 * *Files identical despite different names*

### Comparing `livestyled-1.4.6/livestyled/models/audience_device.py` & `livestyled-1.4.8/livestyled/models/audience_device.py`

 * *Files identical despite different names*

### Comparing `livestyled-1.4.6/livestyled/models/banner.py` & `livestyled-1.4.8/livestyled/models/banner.py`

 * *Files identical despite different names*

### Comparing `livestyled-1.4.6/livestyled/models/booking.py` & `livestyled-1.4.8/livestyled/models/booking.py`

 * *Files identical despite different names*

### Comparing `livestyled-1.4.6/livestyled/models/cohort.py` & `livestyled-1.4.8/livestyled/models/cohort.py`

 * *Files identical despite different names*

### Comparing `livestyled-1.4.6/livestyled/models/competition.py` & `livestyled-1.4.8/livestyled/models/competition.py`

 * *Files identical despite different names*

### Comparing `livestyled-1.4.6/livestyled/models/device.py` & `livestyled-1.4.8/livestyled/models/device.py`

 * *Files identical despite different names*

### Comparing `livestyled-1.4.6/livestyled/models/device_consent.py` & `livestyled-1.4.8/livestyled/models/device_consent.py`

 * *Files identical despite different names*

### Comparing `livestyled-1.4.6/livestyled/models/device_form_data.py` & `livestyled-1.4.8/livestyled/models/device_form_data.py`

 * *Files identical despite different names*

### Comparing `livestyled-1.4.6/livestyled/models/device_preference.py` & `livestyled-1.4.8/livestyled/models/device_preference.py`

 * *Files identical despite different names*

### Comparing `livestyled-1.4.6/livestyled/models/device_reality.py` & `livestyled-1.4.8/livestyled/models/device_reality.py`

 * *Files identical despite different names*

### Comparing `livestyled-1.4.6/livestyled/models/device_token.py` & `livestyled-1.4.8/livestyled/models/device_token.py`

 * *Files identical despite different names*

### Comparing `livestyled-1.4.6/livestyled/models/event.py` & `livestyled-1.4.8/livestyled/models/event.py`

 * *Files identical despite different names*

### Comparing `livestyled-1.4.6/livestyled/models/event_date.py` & `livestyled-1.4.8/livestyled/models/event_date.py`

 * *Files identical despite different names*

### Comparing `livestyled-1.4.6/livestyled/models/fixture.py` & `livestyled-1.4.8/livestyled/models/fixture.py`

 * *Files identical despite different names*

### Comparing `livestyled-1.4.6/livestyled/models/form.py` & `livestyled-1.4.8/livestyled/models/form.py`

 * *Files identical despite different names*

### Comparing `livestyled-1.4.6/livestyled/models/form_field.py` & `livestyled-1.4.8/livestyled/models/form_field.py`

 * *Files identical despite different names*

### Comparing `livestyled-1.4.6/livestyled/models/fulfilment_point.py` & `livestyled-1.4.8/livestyled/models/fulfilment_point.py`

 * *Files identical despite different names*

### Comparing `livestyled-1.4.6/livestyled/models/league_table.py` & `livestyled-1.4.8/livestyled/models/league_table.py`

 * *Files identical despite different names*

### Comparing `livestyled-1.4.6/livestyled/models/location.py` & `livestyled-1.4.8/livestyled/models/location.py`

 * *Files identical despite different names*

### Comparing `livestyled-1.4.6/livestyled/models/magic_field.py` & `livestyled-1.4.8/livestyled/models/magic_field.py`

 * *Files identical despite different names*

### Comparing `livestyled-1.4.6/livestyled/models/news.py` & `livestyled-1.4.8/livestyled/models/news.py`

 * *Files identical despite different names*

### Comparing `livestyled-1.4.6/livestyled/models/order.py` & `livestyled-1.4.8/livestyled/models/order.py`

 * *Files identical despite different names*

### Comparing `livestyled-1.4.6/livestyled/models/payment.py` & `livestyled-1.4.8/livestyled/models/payment.py`

 * *Files identical despite different names*

### Comparing `livestyled-1.4.6/livestyled/models/product.py` & `livestyled-1.4.8/livestyled/models/product.py`

 * *Files identical despite different names*

### Comparing `livestyled-1.4.6/livestyled/models/push_broadcast.py` & `livestyled-1.4.8/livestyled/models/push_broadcast.py`

 * *Files identical despite different names*

### Comparing `livestyled-1.4.6/livestyled/models/push_consent.py` & `livestyled-1.4.8/livestyled/models/push_consent.py`

 * *Files identical despite different names*

### Comparing `livestyled-1.4.6/livestyled/models/reality.py` & `livestyled-1.4.8/livestyled/models/reality.py`

 * *Files identical despite different names*

### Comparing `livestyled-1.4.6/livestyled/models/screen.py` & `livestyled-1.4.8/livestyled/models/screen.py`

 * *Files identical despite different names*

### Comparing `livestyled-1.4.6/livestyled/models/season.py` & `livestyled-1.4.8/livestyled/models/season.py`

 * *Files identical despite different names*

### Comparing `livestyled-1.4.6/livestyled/models/sport_venue.py` & `livestyled-1.4.8/livestyled/models/sport_venue.py`

 * *Files identical despite different names*

### Comparing `livestyled-1.4.6/livestyled/models/storage.py` & `livestyled-1.4.8/livestyled/models/storage.py`

 * *Files identical despite different names*

### Comparing `livestyled-1.4.6/livestyled/models/team.py` & `livestyled-1.4.8/livestyled/models/team.py`

 * *Files identical despite different names*

### Comparing `livestyled-1.4.6/livestyled/models/tests/test_device_form_data.py` & `livestyled-1.4.8/livestyled/models/tests/test_device_form_data.py`

 * *Files identical despite different names*

### Comparing `livestyled-1.4.6/livestyled/models/tests/test_fixture.py` & `livestyled-1.4.8/livestyled/models/tests/test_fixture.py`

 * *Files identical despite different names*

### Comparing `livestyled-1.4.6/livestyled/models/tests/test_form.py` & `livestyled-1.4.8/livestyled/models/tests/test_form.py`

 * *Files identical despite different names*

### Comparing `livestyled-1.4.6/livestyled/models/tests/test_form_field.py` & `livestyled-1.4.8/livestyled/models/tests/test_form_field.py`

 * *Files identical despite different names*

### Comparing `livestyled-1.4.6/livestyled/models/tests/test_ticket.py` & `livestyled-1.4.8/livestyled/models/tests/test_ticket.py`

 * *Files identical despite different names*

### Comparing `livestyled-1.4.6/livestyled/models/ticket.py` & `livestyled-1.4.8/livestyled/models/ticket.py`

 * *Files 2% similar despite different names*

```diff
@@ -54,15 +54,16 @@
             event=None,
             ticket_auth=None,
             event_date=None,
             currency=None,
             external_card_ref=None,
             additional_fields=[],
             printed=True,
-            timezone=None
+            timezone=None,
+            ticket_type='ticket'
     ):
         self.id = id
         self.external_ticket_id = external_ticket_id
         self.external_movement_id = external_movement_id
         self.seat = seat
         self.qr_code_url = qr_code_url
         self.session_date = session_date
@@ -166,14 +167,15 @@
                 self.currency = Currency(**currency)
         else:
             self.currency = None
 
         self.additional_fields = additional_fields
         self.printed = printed
         self.timezone = timezone
+        self.ticket_type = ticket_type
 
     @classmethod
     def placeholder(
             cls,
             id
     ):
         return cls(
@@ -221,15 +223,16 @@
             ticket_integration=None,
             venue=None,
             event=None,
             currency=None,
             external_card_ref=None,
             additional_fields=[],
             printed=True,
-            timezone=None
+            timezone=None,
+            ticket_type='ticket'
         )
 
     @classmethod
     def create_new(
             cls,
             user: User or str or int,
             external_ticket_id=None,
@@ -272,15 +275,16 @@
             ticket_integration=None,
             venue: Venue or str or int or None = None,
             event: Event or str or int or None = None,
             currency: Currency or None = None,
             external_card_ref=None,
             additional_fields=None,
             printed=True,
-            timezone=None
+            timezone=None,
+            ticket_type='ticket'
     ):
         if additional_fields is None:
             additional_fields = []
         ticket = Ticket(
             id=None,
             external_ticket_id=external_ticket_id,
             external_movement_id=external_movement_id,
@@ -325,26 +329,27 @@
             ticket_integration=ticket_integration,
             venue=venue,
             event=event,
             currency=currency,
             external_card_ref=external_card_ref,
             additional_fields=additional_fields,
             printed=printed,
-            timezone=timezone
+            timezone=timezone,
+            ticket_type=ticket_type
         )
         if isinstance(user, (str, int)):
             user = User.placeholder(id=user)
         ticket._user = user
-        if isinstance(sharer, (str or int)):
+        if isinstance(sharer, (str, int)):
             sharer = User.placeholder(id=sharer)
         ticket._sharer = sharer
-        if isinstance(redeemer, (str or int)):
+        if isinstance(redeemer, (str, int)):
             redeemer = User.placeholder(id=redeemer)
         ticket._redeemer = redeemer
-        if isinstance(parent_ticket, (str or int)):
+        if isinstance(parent_ticket, (str, int)):
             parent_ticket = Ticket.placeholder(id=parent_ticket)
         ticket._parent_ticket = parent_ticket
         return ticket
 
     @property
     def user_id(self):
         if self._user:
@@ -394,15 +399,15 @@
         fields = (
             'external_ticket_id', 'seat', 'qr_code_url', 'session_date', 'title', 'legacy_external_event_id',
             'external_event_id', 'barcode', 'sector_name', 'venue_name', 'venue_room', 'client_name', 'premium',
             'client_email', 'price', 'status', 'can_share', 'sharer_email', 'redeemed_at', 'redeemer_id', 'share_code',
             'redeemer_email', 'parent_ticket', 'shared_at', 'legal_long_text', 'legal_short_text', 'map_url',
             'map_image_url', 'ticket_integration', 'entrance', 'row', 'section', 'price_code', 'price_type',
             'external_customer_ref', 'venue', 'event', 'event_date', 'currency', 'external_card_ref',
-            'additional_fields', 'printed', 'timezone'
+            'additional_fields', 'printed', 'timezone', 'ticket_type'
         )
         for field in fields:
             if getattr(self, field) != getattr(other, field):
                 if field == 'additional_fields' and getattr(other, field):
                     if getattr(self, field):
                         additional_fields = []
                         for current in getattr(other, field):
```

### Comparing `livestyled-1.4.6/livestyled/models/ticket_auth.py` & `livestyled-1.4.8/livestyled/models/ticket_auth.py`

 * *Files identical despite different names*

### Comparing `livestyled-1.4.6/livestyled/models/ticket_integration.py` & `livestyled-1.4.8/livestyled/models/ticket_integration.py`

 * *Files identical despite different names*

### Comparing `livestyled-1.4.6/livestyled/models/user.py` & `livestyled-1.4.8/livestyled/models/user.py`

 * *Files identical despite different names*

### Comparing `livestyled-1.4.6/livestyled/models/user_cohort.py` & `livestyled-1.4.8/livestyled/models/user_cohort.py`

 * *Files identical despite different names*

### Comparing `livestyled-1.4.6/livestyled/models/venue.py` & `livestyled-1.4.8/livestyled/models/venue.py`

 * *Files identical despite different names*

### Comparing `livestyled-1.4.6/livestyled/models/widget.py` & `livestyled-1.4.8/livestyled/models/widget.py`

 * *Files identical despite different names*

### Comparing `livestyled-1.4.6/livestyled/resource_client.py` & `livestyled-1.4.8/livestyled/resource_client.py`

 * *Files identical despite different names*

### Comparing `livestyled-1.4.6/livestyled/schemas/__init__.py` & `livestyled-1.4.8/livestyled/schemas/__init__.py`

 * *Files identical despite different names*

### Comparing `livestyled-1.4.6/livestyled/schemas/app.py` & `livestyled-1.4.8/livestyled/schemas/app.py`

 * *Files identical despite different names*

### Comparing `livestyled-1.4.6/livestyled/schemas/audience.py` & `livestyled-1.4.8/livestyled/schemas/audience.py`

 * *Files identical despite different names*

### Comparing `livestyled-1.4.6/livestyled/schemas/audience_device.py` & `livestyled-1.4.8/livestyled/schemas/audience_device.py`

 * *Files identical despite different names*

### Comparing `livestyled-1.4.6/livestyled/schemas/banner.py` & `livestyled-1.4.8/livestyled/schemas/banner.py`

 * *Files identical despite different names*

### Comparing `livestyled-1.4.6/livestyled/schemas/booking.py` & `livestyled-1.4.8/livestyled/schemas/booking.py`

 * *Files identical despite different names*

### Comparing `livestyled-1.4.6/livestyled/schemas/competition.py` & `livestyled-1.4.8/livestyled/schemas/competition.py`

 * *Files identical despite different names*

### Comparing `livestyled-1.4.6/livestyled/schemas/device.py` & `livestyled-1.4.8/livestyled/schemas/device.py`

 * *Files identical despite different names*

### Comparing `livestyled-1.4.6/livestyled/schemas/device_consent.py` & `livestyled-1.4.8/livestyled/schemas/device_consent.py`

 * *Files identical despite different names*

### Comparing `livestyled-1.4.6/livestyled/schemas/device_form_data.py` & `livestyled-1.4.8/livestyled/schemas/device_form_data.py`

 * *Files identical despite different names*

### Comparing `livestyled-1.4.6/livestyled/schemas/device_preference.py` & `livestyled-1.4.8/livestyled/schemas/device_preference.py`

 * *Files identical despite different names*

### Comparing `livestyled-1.4.6/livestyled/schemas/device_reality.py` & `livestyled-1.4.8/livestyled/schemas/device_reality.py`

 * *Files identical despite different names*

### Comparing `livestyled-1.4.6/livestyled/schemas/device_token.py` & `livestyled-1.4.8/livestyled/schemas/device_token.py`

 * *Files identical despite different names*

### Comparing `livestyled-1.4.6/livestyled/schemas/event.py` & `livestyled-1.4.8/livestyled/schemas/event.py`

 * *Files identical despite different names*

### Comparing `livestyled-1.4.6/livestyled/schemas/event_category.py` & `livestyled-1.4.8/livestyled/schemas/event_category.py`

 * *Files identical despite different names*

### Comparing `livestyled-1.4.6/livestyled/schemas/event_integration.py` & `livestyled-1.4.8/livestyled/schemas/event_integration.py`

 * *Files identical despite different names*

### Comparing `livestyled-1.4.6/livestyled/schemas/event_stage.py` & `livestyled-1.4.8/livestyled/schemas/event_stage.py`

 * *Files identical despite different names*

### Comparing `livestyled-1.4.6/livestyled/schemas/fields.py` & `livestyled-1.4.8/livestyled/schemas/fields.py`

 * *Files identical despite different names*

### Comparing `livestyled-1.4.6/livestyled/schemas/fixture.py` & `livestyled-1.4.8/livestyled/schemas/fixture.py`

 * *Files identical despite different names*

### Comparing `livestyled-1.4.6/livestyled/schemas/form.py` & `livestyled-1.4.8/livestyled/schemas/form.py`

 * *Files identical despite different names*

### Comparing `livestyled-1.4.6/livestyled/schemas/form_field.py` & `livestyled-1.4.8/livestyled/schemas/form_field.py`

 * *Files identical despite different names*

### Comparing `livestyled-1.4.6/livestyled/schemas/fulfilment_point.py` & `livestyled-1.4.8/livestyled/schemas/fulfilment_point.py`

 * *Files identical despite different names*

### Comparing `livestyled-1.4.6/livestyled/schemas/league_table.py` & `livestyled-1.4.8/livestyled/schemas/league_table.py`

 * *Files identical despite different names*

### Comparing `livestyled-1.4.6/livestyled/schemas/location.py` & `livestyled-1.4.8/livestyled/schemas/location.py`

 * *Files identical despite different names*

### Comparing `livestyled-1.4.6/livestyled/schemas/magic_field.py` & `livestyled-1.4.8/livestyled/schemas/magic_field.py`

 * *Files identical despite different names*

### Comparing `livestyled-1.4.6/livestyled/schemas/news.py` & `livestyled-1.4.8/livestyled/schemas/news.py`

 * *Files identical despite different names*

### Comparing `livestyled-1.4.6/livestyled/schemas/order.py` & `livestyled-1.4.8/livestyled/schemas/order.py`

 * *Files identical despite different names*

### Comparing `livestyled-1.4.6/livestyled/schemas/payment.py` & `livestyled-1.4.8/livestyled/schemas/payment.py`

 * *Files identical despite different names*

### Comparing `livestyled-1.4.6/livestyled/schemas/product.py` & `livestyled-1.4.8/livestyled/schemas/product.py`

 * *Files identical despite different names*

### Comparing `livestyled-1.4.6/livestyled/schemas/push_broadcast.py` & `livestyled-1.4.8/livestyled/schemas/push_broadcast.py`

 * *Files identical despite different names*

### Comparing `livestyled-1.4.6/livestyled/schemas/push_consent.py` & `livestyled-1.4.8/livestyled/schemas/push_consent.py`

 * *Files identical despite different names*

### Comparing `livestyled-1.4.6/livestyled/schemas/reality.py` & `livestyled-1.4.8/livestyled/schemas/reality.py`

 * *Files identical despite different names*

### Comparing `livestyled-1.4.6/livestyled/schemas/screen.py` & `livestyled-1.4.8/livestyled/schemas/screen.py`

 * *Files identical despite different names*

### Comparing `livestyled-1.4.6/livestyled/schemas/team.py` & `livestyled-1.4.8/livestyled/schemas/team.py`

 * *Files identical despite different names*

### Comparing `livestyled-1.4.6/livestyled/schemas/ticket.py` & `livestyled-1.4.8/livestyled/schemas/ticket.py`

 * *Files 2% similar despite different names*

```diff
@@ -97,7 +97,8 @@
     venue = RelatedResourceLinkField(schema=VenueSchema, required=False, missing=None)
     currency = RelatedResourceLinkField(schema=CurrencySchema, required=False, missing=None)
     external_card_ref = fields.String(data_key='externalCardRef', required=False, missing=None)
     additional_fields = fields.Nested(AdditionalFields, data_key='additionalFields', allow_none=True, missing=None,
                                       many=True)
     printed = fields.Boolean(allow_none=True, required=False, missing=True)
     timezone = fields.String(allow_none=True, required=False, missing=None)
+    ticket_type = fields.String(data_key='ticketType', required=False, allow_none=False)
```

### Comparing `livestyled-1.4.6/livestyled/schemas/ticket_auth.py` & `livestyled-1.4.8/livestyled/schemas/ticket_auth.py`

 * *Files identical despite different names*

### Comparing `livestyled-1.4.6/livestyled/schemas/ticket_integration.py` & `livestyled-1.4.8/livestyled/schemas/ticket_integration.py`

 * *Files identical despite different names*

### Comparing `livestyled-1.4.6/livestyled/schemas/user.py` & `livestyled-1.4.8/livestyled/schemas/user.py`

 * *Files identical despite different names*

### Comparing `livestyled-1.4.6/livestyled/schemas/venue.py` & `livestyled-1.4.8/livestyled/schemas/venue.py`

 * *Files identical despite different names*

### Comparing `livestyled-1.4.6/livestyled/schemas/widget.py` & `livestyled-1.4.8/livestyled/schemas/widget.py`

 * *Files identical despite different names*

### Comparing `livestyled-1.4.6/livestyled/tests/test_app.py` & `livestyled-1.4.8/livestyled/tests/test_app.py`

 * *Files identical despite different names*

### Comparing `livestyled-1.4.6/livestyled/tests/test_create_resource_from_data.py` & `livestyled-1.4.8/livestyled/tests/test_create_resource_from_data.py`

 * *Files identical despite different names*

### Comparing `livestyled-1.4.6/livestyled/tests/test_device.py` & `livestyled-1.4.8/livestyled/tests/test_device.py`

 * *Files identical despite different names*

### Comparing `livestyled-1.4.6/livestyled/tests/test_resource_audience_device.py` & `livestyled-1.4.8/livestyled/tests/test_resource_audience_device.py`

 * *Files identical despite different names*

### Comparing `livestyled-1.4.6/livestyled/tests/test_resource_banners.py` & `livestyled-1.4.8/livestyled/tests/test_resource_banners.py`

 * *Files identical despite different names*

### Comparing `livestyled-1.4.6/livestyled/tests/test_resource_client_bookings.py` & `livestyled-1.4.8/livestyled/tests/test_resource_client_bookings.py`

 * *Files identical despite different names*

### Comparing `livestyled-1.4.6/livestyled/tests/test_resource_client_device.py` & `livestyled-1.4.8/livestyled/tests/test_resource_client_device.py`

 * *Files identical despite different names*

### Comparing `livestyled-1.4.6/livestyled/tests/test_resource_client_device_form_data.py` & `livestyled-1.4.8/livestyled/tests/test_resource_client_device_form_data.py`

 * *Files identical despite different names*

### Comparing `livestyled-1.4.6/livestyled/tests/test_resource_client_device_realities.py` & `livestyled-1.4.8/livestyled/tests/test_resource_client_device_realities.py`

 * *Files identical despite different names*

### Comparing `livestyled-1.4.6/livestyled/tests/test_resource_client_events.py` & `livestyled-1.4.8/livestyled/tests/test_resource_client_events.py`

 * *Files identical despite different names*

### Comparing `livestyled-1.4.6/livestyled/tests/test_resource_client_fulfilment_points.py` & `livestyled-1.4.8/livestyled/tests/test_resource_client_fulfilment_points.py`

 * *Files identical despite different names*

### Comparing `livestyled-1.4.6/livestyled/tests/test_resource_client_locations.py` & `livestyled-1.4.8/livestyled/tests/test_resource_client_locations.py`

 * *Files identical despite different names*

### Comparing `livestyled-1.4.6/livestyled/tests/test_resource_client_news.py` & `livestyled-1.4.8/livestyled/tests/test_resource_client_news.py`

 * *Files identical despite different names*

### Comparing `livestyled-1.4.6/livestyled/tests/test_resource_client_orders.py` & `livestyled-1.4.8/livestyled/tests/test_resource_client_orders.py`

 * *Files identical despite different names*

### Comparing `livestyled-1.4.6/livestyled/tests/test_resource_client_products.py` & `livestyled-1.4.8/livestyled/tests/test_resource_client_products.py`

 * *Files identical despite different names*

### Comparing `livestyled-1.4.6/livestyled/tests/test_resource_client_teams.py` & `livestyled-1.4.8/livestyled/tests/test_resource_client_teams.py`

 * *Files identical despite different names*

### Comparing `livestyled-1.4.6/livestyled/tests/test_resource_client_ticket.py` & `livestyled-1.4.8/livestyled/tests/test_resource_client_ticket.py`

 * *Files 5% similar despite different names*

```diff
@@ -53,14 +53,15 @@
     assert ticket.sharer_email is None
     assert ticket.updated_at == datetime(2019, 5, 24, 12, 41, 22, tzinfo=timezone(timedelta(0), '+0000'))
     assert ticket.user_id is None
     assert ticket.user is None
     assert ticket.venue_name is None
     assert ticket.venue_room is None
     assert ticket.redeemed_at is None
+    assert ticket.ticket_type is 'ticket'
 
 
 def test_get_ticket_shared(requests_mock):
     mock_responses = (
         ('GET', 'https://' + TEST_API_DOMAIN + '/v4/tickets/44', 'mock_responses/ls_api/example_ticket_shared.json', 200),
     )
     configure_mock_responses(requests_mock, mock_responses, FIXTURES_DIR, CONTENT_TYPE)
@@ -99,14 +100,15 @@
     assert ticket.sharer_email == 'test@livestyled.com'
     assert ticket.updated_at == datetime(2019, 5, 24, 12, 41, 22, tzinfo=timezone(timedelta(0), '+0000'))
     assert ticket.user_id is None
     assert ticket.user is None
     assert ticket.venue_name is None
     assert ticket.venue_room is None
     assert ticket.redeemed_at is None
+    assert ticket.ticket_type is 'ticket'
 
 
 def test_get_ticket_shared_redeemed(requests_mock):
     mock_responses = (
         ('GET', 'https://' + TEST_API_DOMAIN + '/v4/tickets/44', 'mock_responses/ls_api/example_ticket_shared_redeemed.json', 200),
     )
     configure_mock_responses(requests_mock, mock_responses, FIXTURES_DIR, CONTENT_TYPE)
@@ -146,14 +148,15 @@
     assert ticket.sharer_email == 'test@livestyled.com'
     assert ticket.updated_at == datetime(2019, 5, 24, 13, 41, 22, tzinfo=timezone(timedelta(0), '+0000'))
     assert ticket.user_id is None
     assert ticket.user is None
     assert ticket.venue_name is None
     assert ticket.venue_room is None
     assert ticket.redeemed_at == datetime(2019, 5, 24, 13, 41, 22, tzinfo=timezone(timedelta(0), '+0000'))
+    assert ticket.ticket_type is 'ticket'
 
 
 def test_create_ticket(requests_mock):
 
     mock_responses = (
         ('POST', 'https://' + TEST_API_DOMAIN + '/v4/tickets', 'mock_responses/ls_api/create_ticket.json', 200),
     )
@@ -188,9 +191,10 @@
     assert json.loads(create_request.body) == {
         'canShare': False,
         'premium': False,
         'price': 0,
         'user': '/v4/users/1234',
         'ticketIntegration': '/v4/ticket_integrations/99',
         'additionalFields': [],
-        'printed': True
+        'printed': True,
+        'ticketType': 'ticket'
     }
```

### Comparing `livestyled-1.4.6/livestyled/tests/test_resource_client_ticket_auths.py` & `livestyled-1.4.8/livestyled/tests/test_resource_client_ticket_auths.py`

 * *Files identical despite different names*

### Comparing `livestyled-1.4.6/livestyled/tests/test_resource_client_user.py` & `livestyled-1.4.8/livestyled/tests/test_resource_client_user.py`

 * *Files identical despite different names*

### Comparing `livestyled-1.4.6/livestyled/tests/test_resource_device_preferences.py` & `livestyled-1.4.8/livestyled/tests/test_resource_device_preferences.py`

 * *Files identical despite different names*

### Comparing `livestyled-1.4.6/livestyled/tests/test_resource_screens.py` & `livestyled-1.4.8/livestyled/tests/test_resource_screens.py`

 * *Files identical despite different names*

### Comparing `livestyled-1.4.6/livestyled/tests/test_resource_widgets.py` & `livestyled-1.4.8/livestyled/tests/test_resource_widgets.py`

 * *Files identical despite different names*

### Comparing `livestyled-1.4.6/livestyled/tests/utils.py` & `livestyled-1.4.8/livestyled/tests/utils.py`

 * *Files identical despite different names*

### Comparing `livestyled-1.4.6/livestyled.egg-info/SOURCES.txt` & `livestyled-1.4.8/livestyled.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 livestyled/__init__.py
 livestyled/client.py
 livestyled/resource_client.py
 livestyled/utils.py
 livestyled.egg-info/PKG-INFO
 livestyled.egg-info/SOURCES.txt
 livestyled.egg-info/dependency_links.txt
+livestyled.egg-info/entry_points.txt
 livestyled.egg-info/requires.txt
 livestyled.egg-info/top_level.txt
 livestyled/models/__init__.py
 livestyled/models/app.py
 livestyled/models/audience.py
 livestyled/models/audience_device.py
 livestyled/models/banner.py
```

### Comparing `livestyled-1.4.6/setup.py` & `livestyled-1.4.8/setup.py`

 * *Files identical despite different names*

