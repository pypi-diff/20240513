# Comparing `tmp/orb_billing-1.50.1.tar.gz` & `tmp/orb_billing-1.51.0.tar.gz`

## Comparing `orb_billing-1.50.1.tar` & `orb_billing-1.51.0.tar`

### file list

```diff
@@ -1,184 +1,184 @@
--rw-r--r--   0        0        0     2976 2020-02-02 00:00:00.000000 orb_billing-1.50.1/src/orb/__init__.py
--rw-r--r--   0        0        0    65289 2020-02-02 00:00:00.000000 orb_billing-1.50.1/src/orb/_base_client.py
--rw-r--r--   0        0        0    27569 2020-02-02 00:00:00.000000 orb_billing-1.50.1/src/orb/_client.py
--rw-r--r--   0        0        0     6389 2020-02-02 00:00:00.000000 orb_billing-1.50.1/src/orb/_compat.py
--rw-r--r--   0        0        0      464 2020-02-02 00:00:00.000000 orb_billing-1.50.1/src/orb/_constants.py
--rw-r--r--   0        0        0    15693 2020-02-02 00:00:00.000000 orb_billing-1.50.1/src/orb/_exceptions.py
--rw-r--r--   0        0        0     3565 2020-02-02 00:00:00.000000 orb_billing-1.50.1/src/orb/_files.py
--rw-r--r--   0        0        0    15418 2020-02-02 00:00:00.000000 orb_billing-1.50.1/src/orb/_legacy_response.py
--rw-r--r--   0        0        0    26096 2020-02-02 00:00:00.000000 orb_billing-1.50.1/src/orb/_models.py
--rw-r--r--   0        0        0     4846 2020-02-02 00:00:00.000000 orb_billing-1.50.1/src/orb/_qs.py
--rw-r--r--   0        0        0     1082 2020-02-02 00:00:00.000000 orb_billing-1.50.1/src/orb/_resource.py
--rw-r--r--   0        0        0    28559 2020-02-02 00:00:00.000000 orb_billing-1.50.1/src/orb/_response.py
--rw-r--r--   0        0        0    10088 2020-02-02 00:00:00.000000 orb_billing-1.50.1/src/orb/_streaming.py
--rw-r--r--   0        0        0     6223 2020-02-02 00:00:00.000000 orb_billing-1.50.1/src/orb/_types.py
--rw-r--r--   0        0        0      156 2020-02-02 00:00:00.000000 orb_billing-1.50.1/src/orb/_version.py
--rw-r--r--   0        0        0     1748 2020-02-02 00:00:00.000000 orb_billing-1.50.1/src/orb/pagination.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 orb_billing-1.50.1/src/orb/py.typed
--rw-r--r--   0        0        0     1847 2020-02-02 00:00:00.000000 orb_billing-1.50.1/src/orb/_utils/__init__.py
--rw-r--r--   0        0        0      765 2020-02-02 00:00:00.000000 orb_billing-1.50.1/src/orb/_utils/_logs.py
--rw-r--r--   0        0        0     1910 2020-02-02 00:00:00.000000 orb_billing-1.50.1/src/orb/_utils/_proxy.py
--rw-r--r--   0        0        0      289 2020-02-02 00:00:00.000000 orb_billing-1.50.1/src/orb/_utils/_streams.py
--rw-r--r--   0        0        0     2269 2020-02-02 00:00:00.000000 orb_billing-1.50.1/src/orb/_utils/_sync.py
--rw-r--r--   0        0        0    12958 2020-02-02 00:00:00.000000 orb_billing-1.50.1/src/orb/_utils/_transform.py
--rw-r--r--   0        0        0     3838 2020-02-02 00:00:00.000000 orb_billing-1.50.1/src/orb/_utils/_typing.py
--rw-r--r--   0        0        0    11497 2020-02-02 00:00:00.000000 orb_billing-1.50.1/src/orb/_utils/_utils.py
--rw-r--r--   0        0        0      224 2020-02-02 00:00:00.000000 orb_billing-1.50.1/src/orb/lib/.keep
--rw-r--r--   0        0        0     5181 2020-02-02 00:00:00.000000 orb_billing-1.50.1/src/orb/resources/__init__.py
--rw-r--r--   0        0        0    38318 2020-02-02 00:00:00.000000 orb_billing-1.50.1/src/orb/resources/alerts.py
--rw-r--r--   0        0        0     9545 2020-02-02 00:00:00.000000 orb_billing-1.50.1/src/orb/resources/credit_notes.py
--rw-r--r--   0        0        0     7970 2020-02-02 00:00:00.000000 orb_billing-1.50.1/src/orb/resources/invoice_line_items.py
--rw-r--r--   0        0        0    39562 2020-02-02 00:00:00.000000 orb_billing-1.50.1/src/orb/resources/invoices.py
--rw-r--r--   0        0        0    12177 2020-02-02 00:00:00.000000 orb_billing-1.50.1/src/orb/resources/items.py
--rw-r--r--   0        0        0    16140 2020-02-02 00:00:00.000000 orb_billing-1.50.1/src/orb/resources/metrics.py
--rw-r--r--   0        0        0   163148 2020-02-02 00:00:00.000000 orb_billing-1.50.1/src/orb/resources/subscriptions.py
--rw-r--r--   0        0        0     4512 2020-02-02 00:00:00.000000 orb_billing-1.50.1/src/orb/resources/top_level.py
--rw-r--r--   0        0        0     6428 2020-02-02 00:00:00.000000 orb_billing-1.50.1/src/orb/resources/webhooks.py
--rw-r--r--   0        0        0      914 2020-02-02 00:00:00.000000 orb_billing-1.50.1/src/orb/resources/coupons/__init__.py
--rw-r--r--   0        0        0    20895 2020-02-02 00:00:00.000000 orb_billing-1.50.1/src/orb/resources/coupons/coupons.py
--rw-r--r--   0        0        0     6995 2020-02-02 00:00:00.000000 orb_billing-1.50.1/src/orb/resources/coupons/subscriptions.py
--rw-r--r--   0        0        0     2068 2020-02-02 00:00:00.000000 orb_billing-1.50.1/src/orb/resources/customers/__init__.py
--rw-r--r--   0        0        0    16173 2020-02-02 00:00:00.000000 orb_billing-1.50.1/src/orb/resources/customers/balance_transactions.py
--rw-r--r--   0        0        0    44995 2020-02-02 00:00:00.000000 orb_billing-1.50.1/src/orb/resources/customers/costs.py
--rw-r--r--   0        0        0   159002 2020-02-02 00:00:00.000000 orb_billing-1.50.1/src/orb/resources/customers/customers.py
--rw-r--r--   0        0        0    31859 2020-02-02 00:00:00.000000 orb_billing-1.50.1/src/orb/resources/customers/usage.py
--rw-r--r--   0        0        0     1178 2020-02-02 00:00:00.000000 orb_billing-1.50.1/src/orb/resources/customers/credits/__init__.py
--rw-r--r--   0        0        0    14550 2020-02-02 00:00:00.000000 orb_billing-1.50.1/src/orb/resources/customers/credits/credits.py
--rw-r--r--   0        0        0   203726 2020-02-02 00:00:00.000000 orb_billing-1.50.1/src/orb/resources/customers/credits/ledger.py
--rw-r--r--   0        0        0    34978 2020-02-02 00:00:00.000000 orb_billing-1.50.1/src/orb/resources/customers/credits/top_ups.py
--rw-r--r--   0        0        0      849 2020-02-02 00:00:00.000000 orb_billing-1.50.1/src/orb/resources/events/__init__.py
--rw-r--r--   0        0        0    28366 2020-02-02 00:00:00.000000 orb_billing-1.50.1/src/orb/resources/events/backfills.py
--rw-r--r--   0        0        0    53314 2020-02-02 00:00:00.000000 orb_billing-1.50.1/src/orb/resources/events/events.py
--rw-r--r--   0        0        0      903 2020-02-02 00:00:00.000000 orb_billing-1.50.1/src/orb/resources/plans/__init__.py
--rw-r--r--   0        0        0    13319 2020-02-02 00:00:00.000000 orb_billing-1.50.1/src/orb/resources/plans/external_plan_id.py
--rw-r--r--   0        0        0    25451 2020-02-02 00:00:00.000000 orb_billing-1.50.1/src/orb/resources/plans/plans.py
--rw-r--r--   0        0        0      929 2020-02-02 00:00:00.000000 orb_billing-1.50.1/src/orb/resources/prices/__init__.py
--rw-r--r--   0        0        0     5668 2020-02-02 00:00:00.000000 orb_billing-1.50.1/src/orb/resources/prices/external_price_id.py
--rw-r--r--   0        0        0   134801 2020-02-02 00:00:00.000000 orb_billing-1.50.1/src/orb/resources/prices/prices.py
--rw-r--r--   0        0        0     5773 2020-02-02 00:00:00.000000 orb_billing-1.50.1/src/orb/types/__init__.py
--rw-r--r--   0        0        0     1693 2020-02-02 00:00:00.000000 orb_billing-1.50.1/src/orb/types/alert.py
--rw-r--r--   0        0        0      915 2020-02-02 00:00:00.000000 orb_billing-1.50.1/src/orb/types/alert_create_for_customer_params.py
--rw-r--r--   0        0        0      931 2020-02-02 00:00:00.000000 orb_billing-1.50.1/src/orb/types/alert_create_for_external_customer_params.py
--rw-r--r--   0        0        0      881 2020-02-02 00:00:00.000000 orb_billing-1.50.1/src/orb/types/alert_create_for_subscription_params.py
--rw-r--r--   0        0        0     1315 2020-02-02 00:00:00.000000 orb_billing-1.50.1/src/orb/types/alert_list_params.py
--rw-r--r--   0        0        0     2213 2020-02-02 00:00:00.000000 orb_billing-1.50.1/src/orb/types/coupon.py
--rw-r--r--   0        0        0     1306 2020-02-02 00:00:00.000000 orb_billing-1.50.1/src/orb/types/coupon_create_params.py
--rw-r--r--   0        0        0      743 2020-02-02 00:00:00.000000 orb_billing-1.50.1/src/orb/types/coupon_list_params.py
--rw-r--r--   0        0        0     3875 2020-02-02 00:00:00.000000 orb_billing-1.50.1/src/orb/types/credit_note.py
--rw-r--r--   0        0        0      510 2020-02-02 00:00:00.000000 orb_billing-1.50.1/src/orb/types/credit_note_list_params.py
--rw-r--r--   0        0        0    21166 2020-02-02 00:00:00.000000 orb_billing-1.50.1/src/orb/types/customer.py
--rw-r--r--   0        0        0    22228 2020-02-02 00:00:00.000000 orb_billing-1.50.1/src/orb/types/customer_create_params.py
--rw-r--r--   0        0        0     1049 2020-02-02 00:00:00.000000 orb_billing-1.50.1/src/orb/types/customer_list_params.py
--rw-r--r--   0        0        0    21988 2020-02-02 00:00:00.000000 orb_billing-1.50.1/src/orb/types/customer_update_by_external_id_params.py
--rw-r--r--   0        0        0    21964 2020-02-02 00:00:00.000000 orb_billing-1.50.1/src/orb/types/customer_update_params.py
--rw-r--r--   0        0        0      484 2020-02-02 00:00:00.000000 orb_billing-1.50.1/src/orb/types/evaluate_price_group.py
--rw-r--r--   0        0        0      290 2020-02-02 00:00:00.000000 orb_billing-1.50.1/src/orb/types/event_deprecate_response.py
--rw-r--r--   0        0        0     1780 2020-02-02 00:00:00.000000 orb_billing-1.50.1/src/orb/types/event_ingest_params.py
--rw-r--r--   0        0        0     1013 2020-02-02 00:00:00.000000 orb_billing-1.50.1/src/orb/types/event_ingest_response.py
--rw-r--r--   0        0        0     1114 2020-02-02 00:00:00.000000 orb_billing-1.50.1/src/orb/types/event_search_params.py
--rw-r--r--   0        0        0     1278 2020-02-02 00:00:00.000000 orb_billing-1.50.1/src/orb/types/event_search_response.py
--rw-r--r--   0        0        0     1185 2020-02-02 00:00:00.000000 orb_billing-1.50.1/src/orb/types/event_update_params.py
--rw-r--r--   0        0        0      279 2020-02-02 00:00:00.000000 orb_billing-1.50.1/src/orb/types/event_update_response.py
--rw-r--r--   0        0        0    38126 2020-02-02 00:00:00.000000 orb_billing-1.50.1/src/orb/types/invoice.py
--rw-r--r--   0        0        0     2874 2020-02-02 00:00:00.000000 orb_billing-1.50.1/src/orb/types/invoice_create_params.py
--rw-r--r--   0        0        0      290 2020-02-02 00:00:00.000000 orb_billing-1.50.1/src/orb/types/invoice_fetch_upcoming_params.py
--rw-r--r--   0        0        0    38167 2020-02-02 00:00:00.000000 orb_billing-1.50.1/src/orb/types/invoice_fetch_upcoming_response.py
--rw-r--r--   0        0        0     1181 2020-02-02 00:00:00.000000 orb_billing-1.50.1/src/orb/types/invoice_line_item_create_params.py
--rw-r--r--   0        0        0    11595 2020-02-02 00:00:00.000000 orb_billing-1.50.1/src/orb/types/invoice_line_item_create_response.py
--rw-r--r--   0        0        0     1877 2020-02-02 00:00:00.000000 orb_billing-1.50.1/src/orb/types/invoice_list_params.py
--rw-r--r--   0        0        0      710 2020-02-02 00:00:00.000000 orb_billing-1.50.1/src/orb/types/invoice_mark_paid_params.py
--rw-r--r--   0        0        0      568 2020-02-02 00:00:00.000000 orb_billing-1.50.1/src/orb/types/item.py
--rw-r--r--   0        0        0      311 2020-02-02 00:00:00.000000 orb_billing-1.50.1/src/orb/types/item_create_params.py
--rw-r--r--   0        0        0      498 2020-02-02 00:00:00.000000 orb_billing-1.50.1/src/orb/types/item_list_params.py
--rw-r--r--   0        0        0      823 2020-02-02 00:00:00.000000 orb_billing-1.50.1/src/orb/types/metric_create_params.py
--rw-r--r--   0        0        0      978 2020-02-02 00:00:00.000000 orb_billing-1.50.1/src/orb/types/metric_create_response.py
--rw-r--r--   0        0        0      976 2020-02-02 00:00:00.000000 orb_billing-1.50.1/src/orb/types/metric_fetch_response.py
--rw-r--r--   0        0        0     1045 2020-02-02 00:00:00.000000 orb_billing-1.50.1/src/orb/types/metric_list_params.py
--rw-r--r--   0        0        0      974 2020-02-02 00:00:00.000000 orb_billing-1.50.1/src/orb/types/metric_list_response.py
--rw-r--r--   0        0        0     5035 2020-02-02 00:00:00.000000 orb_billing-1.50.1/src/orb/types/plan.py
--rw-r--r--   0        0        0    24502 2020-02-02 00:00:00.000000 orb_billing-1.50.1/src/orb/types/plan_create_params.py
--rw-r--r--   0        0        0     1177 2020-02-02 00:00:00.000000 orb_billing-1.50.1/src/orb/types/plan_list_params.py
--rw-r--r--   0        0        0      791 2020-02-02 00:00:00.000000 orb_billing-1.50.1/src/orb/types/plan_update_params.py
--rw-r--r--   0        0        0    36618 2020-02-02 00:00:00.000000 orb_billing-1.50.1/src/orb/types/price.py
--rw-r--r--   0        0        0    28352 2020-02-02 00:00:00.000000 orb_billing-1.50.1/src/orb/types/price_create_params.py
--rw-r--r--   0        0        0     1306 2020-02-02 00:00:00.000000 orb_billing-1.50.1/src/orb/types/price_evaluate_params.py
--rw-r--r--   0        0        0      311 2020-02-02 00:00:00.000000 orb_billing-1.50.1/src/orb/types/price_evaluate_response.py
--rw-r--r--   0        0        0      500 2020-02-02 00:00:00.000000 orb_billing-1.50.1/src/orb/types/price_list_params.py
--rw-r--r--   0        0        0    17011 2020-02-02 00:00:00.000000 orb_billing-1.50.1/src/orb/types/subscription.py
--rw-r--r--   0        0        0      781 2020-02-02 00:00:00.000000 orb_billing-1.50.1/src/orb/types/subscription_cancel_params.py
--rw-r--r--   0        0        0    31028 2020-02-02 00:00:00.000000 orb_billing-1.50.1/src/orb/types/subscription_create_params.py
--rw-r--r--   0        0        0     1016 2020-02-02 00:00:00.000000 orb_billing-1.50.1/src/orb/types/subscription_fetch_costs_params.py
--rw-r--r--   0        0        0     7850 2020-02-02 00:00:00.000000 orb_billing-1.50.1/src/orb/types/subscription_fetch_costs_response.py
--rw-r--r--   0        0        0     1075 2020-02-02 00:00:00.000000 orb_billing-1.50.1/src/orb/types/subscription_fetch_schedule_params.py
--rw-r--r--   0        0        0      737 2020-02-02 00:00:00.000000 orb_billing-1.50.1/src/orb/types/subscription_fetch_schedule_response.py
--rw-r--r--   0        0        0     1906 2020-02-02 00:00:00.000000 orb_billing-1.50.1/src/orb/types/subscription_fetch_usage_params.py
--rw-r--r--   0        0        0     1201 2020-02-02 00:00:00.000000 orb_billing-1.50.1/src/orb/types/subscription_list_params.py
--rw-r--r--   0        0        0    33927 2020-02-02 00:00:00.000000 orb_billing-1.50.1/src/orb/types/subscription_price_intervals_params.py
--rw-r--r--   0        0        0    31434 2020-02-02 00:00:00.000000 orb_billing-1.50.1/src/orb/types/subscription_schedule_plan_change_params.py
--rw-r--r--   0        0        0      594 2020-02-02 00:00:00.000000 orb_billing-1.50.1/src/orb/types/subscription_trigger_phase_params.py
--rw-r--r--   0        0        0      431 2020-02-02 00:00:00.000000 orb_billing-1.50.1/src/orb/types/subscription_unschedule_fixed_fee_quantity_updates_params.py
--rw-r--r--   0        0        0     1168 2020-02-02 00:00:00.000000 orb_billing-1.50.1/src/orb/types/subscription_update_fixed_fee_quantity_params.py
--rw-r--r--   0        0        0     1593 2020-02-02 00:00:00.000000 orb_billing-1.50.1/src/orb/types/subscription_update_params.py
--rw-r--r--   0        0        0     2083 2020-02-02 00:00:00.000000 orb_billing-1.50.1/src/orb/types/subscription_usage.py
--rw-r--r--   0        0        0      379 2020-02-02 00:00:00.000000 orb_billing-1.50.1/src/orb/types/subscriptions.py
--rw-r--r--   0        0        0      216 2020-02-02 00:00:00.000000 orb_billing-1.50.1/src/orb/types/top_level_ping_response.py
--rw-r--r--   0        0        0      485 2020-02-02 00:00:00.000000 orb_billing-1.50.1/src/orb/types/beta/evaluate_price_group.py
--rw-r--r--   0        0        0     1307 2020-02-02 00:00:00.000000 orb_billing-1.50.1/src/orb/types/beta/price_evaluate_params.py
--rw-r--r--   0        0        0      312 2020-02-02 00:00:00.000000 orb_billing-1.50.1/src/orb/types/beta/price_evaluate_response.py
--rw-r--r--   0        0        0      210 2020-02-02 00:00:00.000000 orb_billing-1.50.1/src/orb/types/coupons/__init__.py
--rw-r--r--   0        0        0      514 2020-02-02 00:00:00.000000 orb_billing-1.50.1/src/orb/types/coupons/subscription_list_params.py
--rw-r--r--   0        0        0     1657 2020-02-02 00:00:00.000000 orb_billing-1.50.1/src/orb/types/customers/__init__.py
--rw-r--r--   0        0        0      508 2020-02-02 00:00:00.000000 orb_billing-1.50.1/src/orb/types/customers/balance_transaction_create_params.py
--rw-r--r--   0        0        0     1513 2020-02-02 00:00:00.000000 orb_billing-1.50.1/src/orb/types/customers/balance_transaction_create_response.py
--rw-r--r--   0        0        0     1130 2020-02-02 00:00:00.000000 orb_billing-1.50.1/src/orb/types/customers/balance_transaction_list_params.py
--rw-r--r--   0        0        0     1509 2020-02-02 00:00:00.000000 orb_billing-1.50.1/src/orb/types/customers/balance_transaction_list_response.py
--rw-r--r--   0        0        0     1013 2020-02-02 00:00:00.000000 orb_billing-1.50.1/src/orb/types/customers/cost_list_by_external_id_params.py
--rw-r--r--   0        0        0     7848 2020-02-02 00:00:00.000000 orb_billing-1.50.1/src/orb/types/customers/cost_list_by_external_id_response.py
--rw-r--r--   0        0        0      989 2020-02-02 00:00:00.000000 orb_billing-1.50.1/src/orb/types/customers/cost_list_params.py
--rw-r--r--   0        0        0     7824 2020-02-02 00:00:00.000000 orb_billing-1.50.1/src/orb/types/customers/cost_list_response.py
--rw-r--r--   0        0        0      616 2020-02-02 00:00:00.000000 orb_billing-1.50.1/src/orb/types/customers/credit_list_by_external_id_params.py
--rw-r--r--   0        0        0      534 2020-02-02 00:00:00.000000 orb_billing-1.50.1/src/orb/types/customers/credit_list_by_external_id_response.py
--rw-r--r--   0        0        0      592 2020-02-02 00:00:00.000000 orb_billing-1.50.1/src/orb/types/customers/credit_list_params.py
--rw-r--r--   0        0        0      510 2020-02-02 00:00:00.000000 orb_billing-1.50.1/src/orb/types/customers/credit_list_response.py
--rw-r--r--   0        0        0     1701 2020-02-02 00:00:00.000000 orb_billing-1.50.1/src/orb/types/customers/usage_update_by_external_id_params.py
--rw-r--r--   0        0        0      531 2020-02-02 00:00:00.000000 orb_billing-1.50.1/src/orb/types/customers/usage_update_by_external_id_response.py
--rw-r--r--   0        0        0     1677 2020-02-02 00:00:00.000000 orb_billing-1.50.1/src/orb/types/customers/usage_update_params.py
--rw-r--r--   0        0        0      507 2020-02-02 00:00:00.000000 orb_billing-1.50.1/src/orb/types/customers/usage_update_response.py
--rw-r--r--   0        0        0     1701 2020-02-02 00:00:00.000000 orb_billing-1.50.1/src/orb/types/customers/credits/__init__.py
--rw-r--r--   0        0        0     8686 2020-02-02 00:00:00.000000 orb_billing-1.50.1/src/orb/types/customers/credits/ledger_create_entry_by_external_id_params.py
--rw-r--r--   0        0        0     8821 2020-02-02 00:00:00.000000 orb_billing-1.50.1/src/orb/types/customers/credits/ledger_create_entry_by_external_id_response.py
--rw-r--r--   0        0        0     8662 2020-02-02 00:00:00.000000 orb_billing-1.50.1/src/orb/types/customers/credits/ledger_create_entry_params.py
--rw-r--r--   0        0        0     8797 2020-02-02 00:00:00.000000 orb_billing-1.50.1/src/orb/types/customers/credits/ledger_create_entry_response.py
--rw-r--r--   0        0        0     1446 2020-02-02 00:00:00.000000 orb_billing-1.50.1/src/orb/types/customers/credits/ledger_list_by_external_id_params.py
--rw-r--r--   0        0        0     8807 2020-02-02 00:00:00.000000 orb_billing-1.50.1/src/orb/types/customers/credits/ledger_list_by_external_id_response.py
--rw-r--r--   0        0        0     1422 2020-02-02 00:00:00.000000 orb_billing-1.50.1/src/orb/types/customers/credits/ledger_list_params.py
--rw-r--r--   0        0        0     8783 2020-02-02 00:00:00.000000 orb_billing-1.50.1/src/orb/types/customers/credits/ledger_list_response.py
--rw-r--r--   0        0        0     1976 2020-02-02 00:00:00.000000 orb_billing-1.50.1/src/orb/types/customers/credits/top_up_create_by_external_id_params.py
--rw-r--r--   0        0        0     1913 2020-02-02 00:00:00.000000 orb_billing-1.50.1/src/orb/types/customers/credits/top_up_create_by_external_id_response.py
--rw-r--r--   0        0        0     1952 2020-02-02 00:00:00.000000 orb_billing-1.50.1/src/orb/types/customers/credits/top_up_create_params.py
--rw-r--r--   0        0        0     1889 2020-02-02 00:00:00.000000 orb_billing-1.50.1/src/orb/types/customers/credits/top_up_create_response.py
--rw-r--r--   0        0        0      524 2020-02-02 00:00:00.000000 orb_billing-1.50.1/src/orb/types/customers/credits/top_up_list_by_external_id_params.py
--rw-r--r--   0        0        0     1909 2020-02-02 00:00:00.000000 orb_billing-1.50.1/src/orb/types/customers/credits/top_up_list_by_external_id_response.py
--rw-r--r--   0        0        0      500 2020-02-02 00:00:00.000000 orb_billing-1.50.1/src/orb/types/customers/credits/top_up_list_params.py
--rw-r--r--   0        0        0     1885 2020-02-02 00:00:00.000000 orb_billing-1.50.1/src/orb/types/customers/credits/top_up_list_response.py
--rw-r--r--   0        0        0      702 2020-02-02 00:00:00.000000 orb_billing-1.50.1/src/orb/types/events/__init__.py
--rw-r--r--   0        0        0     1050 2020-02-02 00:00:00.000000 orb_billing-1.50.1/src/orb/types/events/backfill_close_response.py
--rw-r--r--   0        0        0     1508 2020-02-02 00:00:00.000000 orb_billing-1.50.1/src/orb/types/events/backfill_create_params.py
--rw-r--r--   0        0        0     1052 2020-02-02 00:00:00.000000 orb_billing-1.50.1/src/orb/types/events/backfill_create_response.py
--rw-r--r--   0        0        0     1050 2020-02-02 00:00:00.000000 orb_billing-1.50.1/src/orb/types/events/backfill_fetch_response.py
--rw-r--r--   0        0        0      506 2020-02-02 00:00:00.000000 orb_billing-1.50.1/src/orb/types/events/backfill_list_params.py
--rw-r--r--   0        0        0     1048 2020-02-02 00:00:00.000000 orb_billing-1.50.1/src/orb/types/events/backfill_list_response.py
--rw-r--r--   0        0        0     1052 2020-02-02 00:00:00.000000 orb_billing-1.50.1/src/orb/types/events/backfill_revert_response.py
--rw-r--r--   0        0        0      224 2020-02-02 00:00:00.000000 orb_billing-1.50.1/src/orb/types/plans/__init__.py
--rw-r--r--   0        0        0      811 2020-02-02 00:00:00.000000 orb_billing-1.50.1/src/orb/types/plans/external_plan_id_update_params.py
--rw-r--r--   0        0        0      122 2020-02-02 00:00:00.000000 orb_billing-1.50.1/src/orb/types/prices/__init__.py
--rw-r--r--   0        0        0      298 2020-02-02 00:00:00.000000 orb_billing-1.50.1/src/orb/types/shared/__init__.py
--rw-r--r--   0        0        0      233 2020-02-02 00:00:00.000000 orb_billing-1.50.1/src/orb/types/shared/billing_cycle_relative_date.py
--rw-r--r--   0        0        0     2160 2020-02-02 00:00:00.000000 orb_billing-1.50.1/src/orb/types/shared/discount.py
--rw-r--r--   0        0        0      280 2020-02-02 00:00:00.000000 orb_billing-1.50.1/src/orb/types/shared/pagination_metadata.py
--rw-r--r--   0        0        0      181 2020-02-02 00:00:00.000000 orb_billing-1.50.1/src/orb/types/shared_params/__init__.py
--rw-r--r--   0        0        0      269 2020-02-02 00:00:00.000000 orb_billing-1.50.1/src/orb/types/shared_params/billing_cycle_relative_date.py
--rw-r--r--   0        0        0      101 2020-02-02 00:00:00.000000 orb_billing-1.50.1/.gitignore
--rw-r--r--   0        0        0    11333 2020-02-02 00:00:00.000000 orb_billing-1.50.1/LICENSE
--rw-r--r--   0        0        0     4371 2020-02-02 00:00:00.000000 orb_billing-1.50.1/pyproject.toml
--rw-r--r--   0        0        0    15252 2020-02-02 00:00:00.000000 orb_billing-1.50.1/PKG-INFO
+-rw-r--r--   0        0        0     2976 2020-02-02 00:00:00.000000 orb_billing-1.51.0/src/orb/__init__.py
+-rw-r--r--   0        0        0    65289 2020-02-02 00:00:00.000000 orb_billing-1.51.0/src/orb/_base_client.py
+-rw-r--r--   0        0        0    27569 2020-02-02 00:00:00.000000 orb_billing-1.51.0/src/orb/_client.py
+-rw-r--r--   0        0        0     6389 2020-02-02 00:00:00.000000 orb_billing-1.51.0/src/orb/_compat.py
+-rw-r--r--   0        0        0      464 2020-02-02 00:00:00.000000 orb_billing-1.51.0/src/orb/_constants.py
+-rw-r--r--   0        0        0    15693 2020-02-02 00:00:00.000000 orb_billing-1.51.0/src/orb/_exceptions.py
+-rw-r--r--   0        0        0     3565 2020-02-02 00:00:00.000000 orb_billing-1.51.0/src/orb/_files.py
+-rw-r--r--   0        0        0    15418 2020-02-02 00:00:00.000000 orb_billing-1.51.0/src/orb/_legacy_response.py
+-rw-r--r--   0        0        0    26096 2020-02-02 00:00:00.000000 orb_billing-1.51.0/src/orb/_models.py
+-rw-r--r--   0        0        0     4846 2020-02-02 00:00:00.000000 orb_billing-1.51.0/src/orb/_qs.py
+-rw-r--r--   0        0        0     1082 2020-02-02 00:00:00.000000 orb_billing-1.51.0/src/orb/_resource.py
+-rw-r--r--   0        0        0    28559 2020-02-02 00:00:00.000000 orb_billing-1.51.0/src/orb/_response.py
+-rw-r--r--   0        0        0    10088 2020-02-02 00:00:00.000000 orb_billing-1.51.0/src/orb/_streaming.py
+-rw-r--r--   0        0        0     6223 2020-02-02 00:00:00.000000 orb_billing-1.51.0/src/orb/_types.py
+-rw-r--r--   0        0        0      156 2020-02-02 00:00:00.000000 orb_billing-1.51.0/src/orb/_version.py
+-rw-r--r--   0        0        0     1748 2020-02-02 00:00:00.000000 orb_billing-1.51.0/src/orb/pagination.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 orb_billing-1.51.0/src/orb/py.typed
+-rw-r--r--   0        0        0     1847 2020-02-02 00:00:00.000000 orb_billing-1.51.0/src/orb/_utils/__init__.py
+-rw-r--r--   0        0        0      765 2020-02-02 00:00:00.000000 orb_billing-1.51.0/src/orb/_utils/_logs.py
+-rw-r--r--   0        0        0     1910 2020-02-02 00:00:00.000000 orb_billing-1.51.0/src/orb/_utils/_proxy.py
+-rw-r--r--   0        0        0      289 2020-02-02 00:00:00.000000 orb_billing-1.51.0/src/orb/_utils/_streams.py
+-rw-r--r--   0        0        0     2269 2020-02-02 00:00:00.000000 orb_billing-1.51.0/src/orb/_utils/_sync.py
+-rw-r--r--   0        0        0    12958 2020-02-02 00:00:00.000000 orb_billing-1.51.0/src/orb/_utils/_transform.py
+-rw-r--r--   0        0        0     3838 2020-02-02 00:00:00.000000 orb_billing-1.51.0/src/orb/_utils/_typing.py
+-rw-r--r--   0        0        0    11497 2020-02-02 00:00:00.000000 orb_billing-1.51.0/src/orb/_utils/_utils.py
+-rw-r--r--   0        0        0      224 2020-02-02 00:00:00.000000 orb_billing-1.51.0/src/orb/lib/.keep
+-rw-r--r--   0        0        0     5181 2020-02-02 00:00:00.000000 orb_billing-1.51.0/src/orb/resources/__init__.py
+-rw-r--r--   0        0        0    38318 2020-02-02 00:00:00.000000 orb_billing-1.51.0/src/orb/resources/alerts.py
+-rw-r--r--   0        0        0     9545 2020-02-02 00:00:00.000000 orb_billing-1.51.0/src/orb/resources/credit_notes.py
+-rw-r--r--   0        0        0     7970 2020-02-02 00:00:00.000000 orb_billing-1.51.0/src/orb/resources/invoice_line_items.py
+-rw-r--r--   0        0        0    39562 2020-02-02 00:00:00.000000 orb_billing-1.51.0/src/orb/resources/invoices.py
+-rw-r--r--   0        0        0    12177 2020-02-02 00:00:00.000000 orb_billing-1.51.0/src/orb/resources/items.py
+-rw-r--r--   0        0        0    16140 2020-02-02 00:00:00.000000 orb_billing-1.51.0/src/orb/resources/metrics.py
+-rw-r--r--   0        0        0   163156 2020-02-02 00:00:00.000000 orb_billing-1.51.0/src/orb/resources/subscriptions.py
+-rw-r--r--   0        0        0     4512 2020-02-02 00:00:00.000000 orb_billing-1.51.0/src/orb/resources/top_level.py
+-rw-r--r--   0        0        0     6428 2020-02-02 00:00:00.000000 orb_billing-1.51.0/src/orb/resources/webhooks.py
+-rw-r--r--   0        0        0      914 2020-02-02 00:00:00.000000 orb_billing-1.51.0/src/orb/resources/coupons/__init__.py
+-rw-r--r--   0        0        0    20895 2020-02-02 00:00:00.000000 orb_billing-1.51.0/src/orb/resources/coupons/coupons.py
+-rw-r--r--   0        0        0     6995 2020-02-02 00:00:00.000000 orb_billing-1.51.0/src/orb/resources/coupons/subscriptions.py
+-rw-r--r--   0        0        0     2068 2020-02-02 00:00:00.000000 orb_billing-1.51.0/src/orb/resources/customers/__init__.py
+-rw-r--r--   0        0        0    16173 2020-02-02 00:00:00.000000 orb_billing-1.51.0/src/orb/resources/customers/balance_transactions.py
+-rw-r--r--   0        0        0    44995 2020-02-02 00:00:00.000000 orb_billing-1.51.0/src/orb/resources/customers/costs.py
+-rw-r--r--   0        0        0   159002 2020-02-02 00:00:00.000000 orb_billing-1.51.0/src/orb/resources/customers/customers.py
+-rw-r--r--   0        0        0    31859 2020-02-02 00:00:00.000000 orb_billing-1.51.0/src/orb/resources/customers/usage.py
+-rw-r--r--   0        0        0     1178 2020-02-02 00:00:00.000000 orb_billing-1.51.0/src/orb/resources/customers/credits/__init__.py
+-rw-r--r--   0        0        0    14550 2020-02-02 00:00:00.000000 orb_billing-1.51.0/src/orb/resources/customers/credits/credits.py
+-rw-r--r--   0        0        0   203726 2020-02-02 00:00:00.000000 orb_billing-1.51.0/src/orb/resources/customers/credits/ledger.py
+-rw-r--r--   0        0        0    34978 2020-02-02 00:00:00.000000 orb_billing-1.51.0/src/orb/resources/customers/credits/top_ups.py
+-rw-r--r--   0        0        0      849 2020-02-02 00:00:00.000000 orb_billing-1.51.0/src/orb/resources/events/__init__.py
+-rw-r--r--   0        0        0    28366 2020-02-02 00:00:00.000000 orb_billing-1.51.0/src/orb/resources/events/backfills.py
+-rw-r--r--   0        0        0    52972 2020-02-02 00:00:00.000000 orb_billing-1.51.0/src/orb/resources/events/events.py
+-rw-r--r--   0        0        0      903 2020-02-02 00:00:00.000000 orb_billing-1.51.0/src/orb/resources/plans/__init__.py
+-rw-r--r--   0        0        0    13319 2020-02-02 00:00:00.000000 orb_billing-1.51.0/src/orb/resources/plans/external_plan_id.py
+-rw-r--r--   0        0        0    25451 2020-02-02 00:00:00.000000 orb_billing-1.51.0/src/orb/resources/plans/plans.py
+-rw-r--r--   0        0        0      929 2020-02-02 00:00:00.000000 orb_billing-1.51.0/src/orb/resources/prices/__init__.py
+-rw-r--r--   0        0        0     5668 2020-02-02 00:00:00.000000 orb_billing-1.51.0/src/orb/resources/prices/external_price_id.py
+-rw-r--r--   0        0        0   134801 2020-02-02 00:00:00.000000 orb_billing-1.51.0/src/orb/resources/prices/prices.py
+-rw-r--r--   0        0        0     5773 2020-02-02 00:00:00.000000 orb_billing-1.51.0/src/orb/types/__init__.py
+-rw-r--r--   0        0        0     1693 2020-02-02 00:00:00.000000 orb_billing-1.51.0/src/orb/types/alert.py
+-rw-r--r--   0        0        0      915 2020-02-02 00:00:00.000000 orb_billing-1.51.0/src/orb/types/alert_create_for_customer_params.py
+-rw-r--r--   0        0        0      931 2020-02-02 00:00:00.000000 orb_billing-1.51.0/src/orb/types/alert_create_for_external_customer_params.py
+-rw-r--r--   0        0        0      881 2020-02-02 00:00:00.000000 orb_billing-1.51.0/src/orb/types/alert_create_for_subscription_params.py
+-rw-r--r--   0        0        0     1315 2020-02-02 00:00:00.000000 orb_billing-1.51.0/src/orb/types/alert_list_params.py
+-rw-r--r--   0        0        0     2213 2020-02-02 00:00:00.000000 orb_billing-1.51.0/src/orb/types/coupon.py
+-rw-r--r--   0        0        0     1306 2020-02-02 00:00:00.000000 orb_billing-1.51.0/src/orb/types/coupon_create_params.py
+-rw-r--r--   0        0        0      743 2020-02-02 00:00:00.000000 orb_billing-1.51.0/src/orb/types/coupon_list_params.py
+-rw-r--r--   0        0        0     3875 2020-02-02 00:00:00.000000 orb_billing-1.51.0/src/orb/types/credit_note.py
+-rw-r--r--   0        0        0      510 2020-02-02 00:00:00.000000 orb_billing-1.51.0/src/orb/types/credit_note_list_params.py
+-rw-r--r--   0        0        0    21166 2020-02-02 00:00:00.000000 orb_billing-1.51.0/src/orb/types/customer.py
+-rw-r--r--   0        0        0    22228 2020-02-02 00:00:00.000000 orb_billing-1.51.0/src/orb/types/customer_create_params.py
+-rw-r--r--   0        0        0     1049 2020-02-02 00:00:00.000000 orb_billing-1.51.0/src/orb/types/customer_list_params.py
+-rw-r--r--   0        0        0    21988 2020-02-02 00:00:00.000000 orb_billing-1.51.0/src/orb/types/customer_update_by_external_id_params.py
+-rw-r--r--   0        0        0    21964 2020-02-02 00:00:00.000000 orb_billing-1.51.0/src/orb/types/customer_update_params.py
+-rw-r--r--   0        0        0      484 2020-02-02 00:00:00.000000 orb_billing-1.51.0/src/orb/types/evaluate_price_group.py
+-rw-r--r--   0        0        0      290 2020-02-02 00:00:00.000000 orb_billing-1.51.0/src/orb/types/event_deprecate_response.py
+-rw-r--r--   0        0        0     1780 2020-02-02 00:00:00.000000 orb_billing-1.51.0/src/orb/types/event_ingest_params.py
+-rw-r--r--   0        0        0     1013 2020-02-02 00:00:00.000000 orb_billing-1.51.0/src/orb/types/event_ingest_response.py
+-rw-r--r--   0        0        0     1114 2020-02-02 00:00:00.000000 orb_billing-1.51.0/src/orb/types/event_search_params.py
+-rw-r--r--   0        0        0     1278 2020-02-02 00:00:00.000000 orb_billing-1.51.0/src/orb/types/event_search_response.py
+-rw-r--r--   0        0        0     1185 2020-02-02 00:00:00.000000 orb_billing-1.51.0/src/orb/types/event_update_params.py
+-rw-r--r--   0        0        0      279 2020-02-02 00:00:00.000000 orb_billing-1.51.0/src/orb/types/event_update_response.py
+-rw-r--r--   0        0        0    38126 2020-02-02 00:00:00.000000 orb_billing-1.51.0/src/orb/types/invoice.py
+-rw-r--r--   0        0        0     2874 2020-02-02 00:00:00.000000 orb_billing-1.51.0/src/orb/types/invoice_create_params.py
+-rw-r--r--   0        0        0      290 2020-02-02 00:00:00.000000 orb_billing-1.51.0/src/orb/types/invoice_fetch_upcoming_params.py
+-rw-r--r--   0        0        0    38167 2020-02-02 00:00:00.000000 orb_billing-1.51.0/src/orb/types/invoice_fetch_upcoming_response.py
+-rw-r--r--   0        0        0     1181 2020-02-02 00:00:00.000000 orb_billing-1.51.0/src/orb/types/invoice_line_item_create_params.py
+-rw-r--r--   0        0        0    11595 2020-02-02 00:00:00.000000 orb_billing-1.51.0/src/orb/types/invoice_line_item_create_response.py
+-rw-r--r--   0        0        0     1877 2020-02-02 00:00:00.000000 orb_billing-1.51.0/src/orb/types/invoice_list_params.py
+-rw-r--r--   0        0        0      710 2020-02-02 00:00:00.000000 orb_billing-1.51.0/src/orb/types/invoice_mark_paid_params.py
+-rw-r--r--   0        0        0      568 2020-02-02 00:00:00.000000 orb_billing-1.51.0/src/orb/types/item.py
+-rw-r--r--   0        0        0      311 2020-02-02 00:00:00.000000 orb_billing-1.51.0/src/orb/types/item_create_params.py
+-rw-r--r--   0        0        0      498 2020-02-02 00:00:00.000000 orb_billing-1.51.0/src/orb/types/item_list_params.py
+-rw-r--r--   0        0        0      823 2020-02-02 00:00:00.000000 orb_billing-1.51.0/src/orb/types/metric_create_params.py
+-rw-r--r--   0        0        0      978 2020-02-02 00:00:00.000000 orb_billing-1.51.0/src/orb/types/metric_create_response.py
+-rw-r--r--   0        0        0      976 2020-02-02 00:00:00.000000 orb_billing-1.51.0/src/orb/types/metric_fetch_response.py
+-rw-r--r--   0        0        0     1045 2020-02-02 00:00:00.000000 orb_billing-1.51.0/src/orb/types/metric_list_params.py
+-rw-r--r--   0        0        0      974 2020-02-02 00:00:00.000000 orb_billing-1.51.0/src/orb/types/metric_list_response.py
+-rw-r--r--   0        0        0     5035 2020-02-02 00:00:00.000000 orb_billing-1.51.0/src/orb/types/plan.py
+-rw-r--r--   0        0        0    24502 2020-02-02 00:00:00.000000 orb_billing-1.51.0/src/orb/types/plan_create_params.py
+-rw-r--r--   0        0        0     1177 2020-02-02 00:00:00.000000 orb_billing-1.51.0/src/orb/types/plan_list_params.py
+-rw-r--r--   0        0        0      791 2020-02-02 00:00:00.000000 orb_billing-1.51.0/src/orb/types/plan_update_params.py
+-rw-r--r--   0        0        0    36618 2020-02-02 00:00:00.000000 orb_billing-1.51.0/src/orb/types/price.py
+-rw-r--r--   0        0        0    28352 2020-02-02 00:00:00.000000 orb_billing-1.51.0/src/orb/types/price_create_params.py
+-rw-r--r--   0        0        0     1306 2020-02-02 00:00:00.000000 orb_billing-1.51.0/src/orb/types/price_evaluate_params.py
+-rw-r--r--   0        0        0      311 2020-02-02 00:00:00.000000 orb_billing-1.51.0/src/orb/types/price_evaluate_response.py
+-rw-r--r--   0        0        0      500 2020-02-02 00:00:00.000000 orb_billing-1.51.0/src/orb/types/price_list_params.py
+-rw-r--r--   0        0        0    17011 2020-02-02 00:00:00.000000 orb_billing-1.51.0/src/orb/types/subscription.py
+-rw-r--r--   0        0        0      781 2020-02-02 00:00:00.000000 orb_billing-1.51.0/src/orb/types/subscription_cancel_params.py
+-rw-r--r--   0        0        0    31030 2020-02-02 00:00:00.000000 orb_billing-1.51.0/src/orb/types/subscription_create_params.py
+-rw-r--r--   0        0        0     1016 2020-02-02 00:00:00.000000 orb_billing-1.51.0/src/orb/types/subscription_fetch_costs_params.py
+-rw-r--r--   0        0        0     7850 2020-02-02 00:00:00.000000 orb_billing-1.51.0/src/orb/types/subscription_fetch_costs_response.py
+-rw-r--r--   0        0        0     1075 2020-02-02 00:00:00.000000 orb_billing-1.51.0/src/orb/types/subscription_fetch_schedule_params.py
+-rw-r--r--   0        0        0      737 2020-02-02 00:00:00.000000 orb_billing-1.51.0/src/orb/types/subscription_fetch_schedule_response.py
+-rw-r--r--   0        0        0     1906 2020-02-02 00:00:00.000000 orb_billing-1.51.0/src/orb/types/subscription_fetch_usage_params.py
+-rw-r--r--   0        0        0     1201 2020-02-02 00:00:00.000000 orb_billing-1.51.0/src/orb/types/subscription_list_params.py
+-rw-r--r--   0        0        0    33927 2020-02-02 00:00:00.000000 orb_billing-1.51.0/src/orb/types/subscription_price_intervals_params.py
+-rw-r--r--   0        0        0    31436 2020-02-02 00:00:00.000000 orb_billing-1.51.0/src/orb/types/subscription_schedule_plan_change_params.py
+-rw-r--r--   0        0        0      594 2020-02-02 00:00:00.000000 orb_billing-1.51.0/src/orb/types/subscription_trigger_phase_params.py
+-rw-r--r--   0        0        0      431 2020-02-02 00:00:00.000000 orb_billing-1.51.0/src/orb/types/subscription_unschedule_fixed_fee_quantity_updates_params.py
+-rw-r--r--   0        0        0     1168 2020-02-02 00:00:00.000000 orb_billing-1.51.0/src/orb/types/subscription_update_fixed_fee_quantity_params.py
+-rw-r--r--   0        0        0     1593 2020-02-02 00:00:00.000000 orb_billing-1.51.0/src/orb/types/subscription_update_params.py
+-rw-r--r--   0        0        0     2083 2020-02-02 00:00:00.000000 orb_billing-1.51.0/src/orb/types/subscription_usage.py
+-rw-r--r--   0        0        0      379 2020-02-02 00:00:00.000000 orb_billing-1.51.0/src/orb/types/subscriptions.py
+-rw-r--r--   0        0        0      216 2020-02-02 00:00:00.000000 orb_billing-1.51.0/src/orb/types/top_level_ping_response.py
+-rw-r--r--   0        0        0      485 2020-02-02 00:00:00.000000 orb_billing-1.51.0/src/orb/types/beta/evaluate_price_group.py
+-rw-r--r--   0        0        0     1307 2020-02-02 00:00:00.000000 orb_billing-1.51.0/src/orb/types/beta/price_evaluate_params.py
+-rw-r--r--   0        0        0      312 2020-02-02 00:00:00.000000 orb_billing-1.51.0/src/orb/types/beta/price_evaluate_response.py
+-rw-r--r--   0        0        0      210 2020-02-02 00:00:00.000000 orb_billing-1.51.0/src/orb/types/coupons/__init__.py
+-rw-r--r--   0        0        0      514 2020-02-02 00:00:00.000000 orb_billing-1.51.0/src/orb/types/coupons/subscription_list_params.py
+-rw-r--r--   0        0        0     1657 2020-02-02 00:00:00.000000 orb_billing-1.51.0/src/orb/types/customers/__init__.py
+-rw-r--r--   0        0        0      508 2020-02-02 00:00:00.000000 orb_billing-1.51.0/src/orb/types/customers/balance_transaction_create_params.py
+-rw-r--r--   0        0        0     1513 2020-02-02 00:00:00.000000 orb_billing-1.51.0/src/orb/types/customers/balance_transaction_create_response.py
+-rw-r--r--   0        0        0     1130 2020-02-02 00:00:00.000000 orb_billing-1.51.0/src/orb/types/customers/balance_transaction_list_params.py
+-rw-r--r--   0        0        0     1509 2020-02-02 00:00:00.000000 orb_billing-1.51.0/src/orb/types/customers/balance_transaction_list_response.py
+-rw-r--r--   0        0        0     1013 2020-02-02 00:00:00.000000 orb_billing-1.51.0/src/orb/types/customers/cost_list_by_external_id_params.py
+-rw-r--r--   0        0        0     7848 2020-02-02 00:00:00.000000 orb_billing-1.51.0/src/orb/types/customers/cost_list_by_external_id_response.py
+-rw-r--r--   0        0        0      989 2020-02-02 00:00:00.000000 orb_billing-1.51.0/src/orb/types/customers/cost_list_params.py
+-rw-r--r--   0        0        0     7824 2020-02-02 00:00:00.000000 orb_billing-1.51.0/src/orb/types/customers/cost_list_response.py
+-rw-r--r--   0        0        0      616 2020-02-02 00:00:00.000000 orb_billing-1.51.0/src/orb/types/customers/credit_list_by_external_id_params.py
+-rw-r--r--   0        0        0      534 2020-02-02 00:00:00.000000 orb_billing-1.51.0/src/orb/types/customers/credit_list_by_external_id_response.py
+-rw-r--r--   0        0        0      592 2020-02-02 00:00:00.000000 orb_billing-1.51.0/src/orb/types/customers/credit_list_params.py
+-rw-r--r--   0        0        0      510 2020-02-02 00:00:00.000000 orb_billing-1.51.0/src/orb/types/customers/credit_list_response.py
+-rw-r--r--   0        0        0     1701 2020-02-02 00:00:00.000000 orb_billing-1.51.0/src/orb/types/customers/usage_update_by_external_id_params.py
+-rw-r--r--   0        0        0      531 2020-02-02 00:00:00.000000 orb_billing-1.51.0/src/orb/types/customers/usage_update_by_external_id_response.py
+-rw-r--r--   0        0        0     1677 2020-02-02 00:00:00.000000 orb_billing-1.51.0/src/orb/types/customers/usage_update_params.py
+-rw-r--r--   0        0        0      507 2020-02-02 00:00:00.000000 orb_billing-1.51.0/src/orb/types/customers/usage_update_response.py
+-rw-r--r--   0        0        0     1701 2020-02-02 00:00:00.000000 orb_billing-1.51.0/src/orb/types/customers/credits/__init__.py
+-rw-r--r--   0        0        0     8686 2020-02-02 00:00:00.000000 orb_billing-1.51.0/src/orb/types/customers/credits/ledger_create_entry_by_external_id_params.py
+-rw-r--r--   0        0        0     8821 2020-02-02 00:00:00.000000 orb_billing-1.51.0/src/orb/types/customers/credits/ledger_create_entry_by_external_id_response.py
+-rw-r--r--   0        0        0     8662 2020-02-02 00:00:00.000000 orb_billing-1.51.0/src/orb/types/customers/credits/ledger_create_entry_params.py
+-rw-r--r--   0        0        0     8797 2020-02-02 00:00:00.000000 orb_billing-1.51.0/src/orb/types/customers/credits/ledger_create_entry_response.py
+-rw-r--r--   0        0        0     1446 2020-02-02 00:00:00.000000 orb_billing-1.51.0/src/orb/types/customers/credits/ledger_list_by_external_id_params.py
+-rw-r--r--   0        0        0     8807 2020-02-02 00:00:00.000000 orb_billing-1.51.0/src/orb/types/customers/credits/ledger_list_by_external_id_response.py
+-rw-r--r--   0        0        0     1422 2020-02-02 00:00:00.000000 orb_billing-1.51.0/src/orb/types/customers/credits/ledger_list_params.py
+-rw-r--r--   0        0        0     8783 2020-02-02 00:00:00.000000 orb_billing-1.51.0/src/orb/types/customers/credits/ledger_list_response.py
+-rw-r--r--   0        0        0     1976 2020-02-02 00:00:00.000000 orb_billing-1.51.0/src/orb/types/customers/credits/top_up_create_by_external_id_params.py
+-rw-r--r--   0        0        0     1913 2020-02-02 00:00:00.000000 orb_billing-1.51.0/src/orb/types/customers/credits/top_up_create_by_external_id_response.py
+-rw-r--r--   0        0        0     1952 2020-02-02 00:00:00.000000 orb_billing-1.51.0/src/orb/types/customers/credits/top_up_create_params.py
+-rw-r--r--   0        0        0     1889 2020-02-02 00:00:00.000000 orb_billing-1.51.0/src/orb/types/customers/credits/top_up_create_response.py
+-rw-r--r--   0        0        0      524 2020-02-02 00:00:00.000000 orb_billing-1.51.0/src/orb/types/customers/credits/top_up_list_by_external_id_params.py
+-rw-r--r--   0        0        0     1909 2020-02-02 00:00:00.000000 orb_billing-1.51.0/src/orb/types/customers/credits/top_up_list_by_external_id_response.py
+-rw-r--r--   0        0        0      500 2020-02-02 00:00:00.000000 orb_billing-1.51.0/src/orb/types/customers/credits/top_up_list_params.py
+-rw-r--r--   0        0        0     1885 2020-02-02 00:00:00.000000 orb_billing-1.51.0/src/orb/types/customers/credits/top_up_list_response.py
+-rw-r--r--   0        0        0      702 2020-02-02 00:00:00.000000 orb_billing-1.51.0/src/orb/types/events/__init__.py
+-rw-r--r--   0        0        0     1050 2020-02-02 00:00:00.000000 orb_billing-1.51.0/src/orb/types/events/backfill_close_response.py
+-rw-r--r--   0        0        0     1508 2020-02-02 00:00:00.000000 orb_billing-1.51.0/src/orb/types/events/backfill_create_params.py
+-rw-r--r--   0        0        0     1052 2020-02-02 00:00:00.000000 orb_billing-1.51.0/src/orb/types/events/backfill_create_response.py
+-rw-r--r--   0        0        0     1050 2020-02-02 00:00:00.000000 orb_billing-1.51.0/src/orb/types/events/backfill_fetch_response.py
+-rw-r--r--   0        0        0      506 2020-02-02 00:00:00.000000 orb_billing-1.51.0/src/orb/types/events/backfill_list_params.py
+-rw-r--r--   0        0        0     1048 2020-02-02 00:00:00.000000 orb_billing-1.51.0/src/orb/types/events/backfill_list_response.py
+-rw-r--r--   0        0        0     1052 2020-02-02 00:00:00.000000 orb_billing-1.51.0/src/orb/types/events/backfill_revert_response.py
+-rw-r--r--   0        0        0      224 2020-02-02 00:00:00.000000 orb_billing-1.51.0/src/orb/types/plans/__init__.py
+-rw-r--r--   0        0        0      811 2020-02-02 00:00:00.000000 orb_billing-1.51.0/src/orb/types/plans/external_plan_id_update_params.py
+-rw-r--r--   0        0        0      122 2020-02-02 00:00:00.000000 orb_billing-1.51.0/src/orb/types/prices/__init__.py
+-rw-r--r--   0        0        0      298 2020-02-02 00:00:00.000000 orb_billing-1.51.0/src/orb/types/shared/__init__.py
+-rw-r--r--   0        0        0      233 2020-02-02 00:00:00.000000 orb_billing-1.51.0/src/orb/types/shared/billing_cycle_relative_date.py
+-rw-r--r--   0        0        0     2160 2020-02-02 00:00:00.000000 orb_billing-1.51.0/src/orb/types/shared/discount.py
+-rw-r--r--   0        0        0      280 2020-02-02 00:00:00.000000 orb_billing-1.51.0/src/orb/types/shared/pagination_metadata.py
+-rw-r--r--   0        0        0      181 2020-02-02 00:00:00.000000 orb_billing-1.51.0/src/orb/types/shared_params/__init__.py
+-rw-r--r--   0        0        0      269 2020-02-02 00:00:00.000000 orb_billing-1.51.0/src/orb/types/shared_params/billing_cycle_relative_date.py
+-rw-r--r--   0        0        0      101 2020-02-02 00:00:00.000000 orb_billing-1.51.0/.gitignore
+-rw-r--r--   0        0        0    11333 2020-02-02 00:00:00.000000 orb_billing-1.51.0/LICENSE
+-rw-r--r--   0        0        0     4371 2020-02-02 00:00:00.000000 orb_billing-1.51.0/pyproject.toml
+-rw-r--r--   0        0        0    15252 2020-02-02 00:00:00.000000 orb_billing-1.51.0/PKG-INFO
```

### Comparing `orb_billing-1.50.1/src/orb/__init__.py` & `orb_billing-1.51.0/src/orb/__init__.py`

 * *Files identical despite different names*

### Comparing `orb_billing-1.50.1/src/orb/_base_client.py` & `orb_billing-1.51.0/src/orb/_base_client.py`

 * *Files identical despite different names*

### Comparing `orb_billing-1.50.1/src/orb/_client.py` & `orb_billing-1.51.0/src/orb/_client.py`

 * *Files identical despite different names*

### Comparing `orb_billing-1.50.1/src/orb/_compat.py` & `orb_billing-1.51.0/src/orb/_compat.py`

 * *Files identical despite different names*

### Comparing `orb_billing-1.50.1/src/orb/_exceptions.py` & `orb_billing-1.51.0/src/orb/_exceptions.py`

 * *Files identical despite different names*

### Comparing `orb_billing-1.50.1/src/orb/_files.py` & `orb_billing-1.51.0/src/orb/_files.py`

 * *Files identical despite different names*

### Comparing `orb_billing-1.50.1/src/orb/_legacy_response.py` & `orb_billing-1.51.0/src/orb/_legacy_response.py`

 * *Files identical despite different names*

### Comparing `orb_billing-1.50.1/src/orb/_models.py` & `orb_billing-1.51.0/src/orb/_models.py`

 * *Files identical despite different names*

### Comparing `orb_billing-1.50.1/src/orb/_qs.py` & `orb_billing-1.51.0/src/orb/_qs.py`

 * *Files identical despite different names*

### Comparing `orb_billing-1.50.1/src/orb/_resource.py` & `orb_billing-1.51.0/src/orb/_resource.py`

 * *Files identical despite different names*

### Comparing `orb_billing-1.50.1/src/orb/_response.py` & `orb_billing-1.51.0/src/orb/_response.py`

 * *Files identical despite different names*

### Comparing `orb_billing-1.50.1/src/orb/_streaming.py` & `orb_billing-1.51.0/src/orb/_streaming.py`

 * *Files identical despite different names*

### Comparing `orb_billing-1.50.1/src/orb/_types.py` & `orb_billing-1.51.0/src/orb/_types.py`

 * *Files identical despite different names*

### Comparing `orb_billing-1.50.1/src/orb/pagination.py` & `orb_billing-1.51.0/src/orb/pagination.py`

 * *Files identical despite different names*

### Comparing `orb_billing-1.50.1/src/orb/_utils/__init__.py` & `orb_billing-1.51.0/src/orb/_utils/__init__.py`

 * *Files identical despite different names*

### Comparing `orb_billing-1.50.1/src/orb/_utils/_logs.py` & `orb_billing-1.51.0/src/orb/_utils/_logs.py`

 * *Files identical despite different names*

### Comparing `orb_billing-1.50.1/src/orb/_utils/_proxy.py` & `orb_billing-1.51.0/src/orb/_utils/_proxy.py`

 * *Files identical despite different names*

### Comparing `orb_billing-1.50.1/src/orb/_utils/_sync.py` & `orb_billing-1.51.0/src/orb/_utils/_sync.py`

 * *Files identical despite different names*

### Comparing `orb_billing-1.50.1/src/orb/_utils/_transform.py` & `orb_billing-1.51.0/src/orb/_utils/_transform.py`

 * *Files identical despite different names*

### Comparing `orb_billing-1.50.1/src/orb/_utils/_typing.py` & `orb_billing-1.51.0/src/orb/_utils/_typing.py`

 * *Files identical despite different names*

### Comparing `orb_billing-1.50.1/src/orb/_utils/_utils.py` & `orb_billing-1.51.0/src/orb/_utils/_utils.py`

 * *Files identical despite different names*

### Comparing `orb_billing-1.50.1/src/orb/resources/__init__.py` & `orb_billing-1.51.0/src/orb/resources/__init__.py`

 * *Files identical despite different names*

### Comparing `orb_billing-1.50.1/src/orb/resources/alerts.py` & `orb_billing-1.51.0/src/orb/resources/alerts.py`

 * *Files identical despite different names*

### Comparing `orb_billing-1.50.1/src/orb/resources/credit_notes.py` & `orb_billing-1.51.0/src/orb/resources/credit_notes.py`

 * *Files identical despite different names*

### Comparing `orb_billing-1.50.1/src/orb/resources/invoice_line_items.py` & `orb_billing-1.51.0/src/orb/resources/invoice_line_items.py`

 * *Files identical despite different names*

### Comparing `orb_billing-1.50.1/src/orb/resources/invoices.py` & `orb_billing-1.51.0/src/orb/resources/invoices.py`

 * *Files identical despite different names*

### Comparing `orb_billing-1.50.1/src/orb/resources/items.py` & `orb_billing-1.51.0/src/orb/resources/items.py`

 * *Files identical despite different names*

### Comparing `orb_billing-1.50.1/src/orb/resources/metrics.py` & `orb_billing-1.51.0/src/orb/resources/metrics.py`

 * *Files identical despite different names*

### Comparing `orb_billing-1.50.1/src/orb/resources/subscriptions.py` & `orb_billing-1.51.0/src/orb/resources/subscriptions.py`

 * *Files 0% similar despite different names*

```diff
@@ -68,15 +68,15 @@
         external_marketplace: Optional[Literal["google", "aws", "azure"]] | NotGiven = NOT_GIVEN,
         external_marketplace_reporting_id: Optional[str] | NotGiven = NOT_GIVEN,
         external_plan_id: Optional[str] | NotGiven = NOT_GIVEN,
         initial_phase_order: Optional[int] | NotGiven = NOT_GIVEN,
         invoicing_threshold: Optional[str] | NotGiven = NOT_GIVEN,
         metadata: Optional[Dict[str, Optional[str]]] | NotGiven = NOT_GIVEN,
         net_terms: Optional[int] | NotGiven = NOT_GIVEN,
-        per_credit_overage_amount: Optional[str] | NotGiven = NOT_GIVEN,
+        per_credit_overage_amount: Optional[float] | NotGiven = NOT_GIVEN,
         plan_id: Optional[str] | NotGiven = NOT_GIVEN,
         price_overrides: Optional[Iterable[subscription_create_params.PriceOverride]] | NotGiven = NOT_GIVEN,
         start_date: Union[str, datetime, None] | NotGiven = NOT_GIVEN,
         # Use the following arguments if you need to pass additional parameters to the API that aren't available via kwargs.
         # The extra values given here take precedence over values defined on the client or passed to this method.
         extra_headers: Headers | None = None,
         extra_query: Query | None = None,
@@ -1362,15 +1362,15 @@
         | NotGiven = NOT_GIVEN,
         change_date: Optional[str] | NotGiven = NOT_GIVEN,
         coupon_redemption_code: Optional[str] | NotGiven = NOT_GIVEN,
         credits_overage_rate: Optional[float] | NotGiven = NOT_GIVEN,
         external_plan_id: Optional[str] | NotGiven = NOT_GIVEN,
         initial_phase_order: Optional[int] | NotGiven = NOT_GIVEN,
         invoicing_threshold: Optional[str] | NotGiven = NOT_GIVEN,
-        per_credit_overage_amount: Optional[str] | NotGiven = NOT_GIVEN,
+        per_credit_overage_amount: Optional[float] | NotGiven = NOT_GIVEN,
         plan_id: Optional[str] | NotGiven = NOT_GIVEN,
         price_overrides: Optional[Iterable[subscription_schedule_plan_change_params.PriceOverride]]
         | NotGiven = NOT_GIVEN,
         # Use the following arguments if you need to pass additional parameters to the API that aren't available via kwargs.
         # The extra values given here take precedence over values defined on the client or passed to this method.
         extra_headers: Headers | None = None,
         extra_query: Query | None = None,
@@ -1780,15 +1780,15 @@
         external_marketplace: Optional[Literal["google", "aws", "azure"]] | NotGiven = NOT_GIVEN,
         external_marketplace_reporting_id: Optional[str] | NotGiven = NOT_GIVEN,
         external_plan_id: Optional[str] | NotGiven = NOT_GIVEN,
         initial_phase_order: Optional[int] | NotGiven = NOT_GIVEN,
         invoicing_threshold: Optional[str] | NotGiven = NOT_GIVEN,
         metadata: Optional[Dict[str, Optional[str]]] | NotGiven = NOT_GIVEN,
         net_terms: Optional[int] | NotGiven = NOT_GIVEN,
-        per_credit_overage_amount: Optional[str] | NotGiven = NOT_GIVEN,
+        per_credit_overage_amount: Optional[float] | NotGiven = NOT_GIVEN,
         plan_id: Optional[str] | NotGiven = NOT_GIVEN,
         price_overrides: Optional[Iterable[subscription_create_params.PriceOverride]] | NotGiven = NOT_GIVEN,
         start_date: Union[str, datetime, None] | NotGiven = NOT_GIVEN,
         # Use the following arguments if you need to pass additional parameters to the API that aren't available via kwargs.
         # The extra values given here take precedence over values defined on the client or passed to this method.
         extra_headers: Headers | None = None,
         extra_query: Query | None = None,
@@ -3074,15 +3074,15 @@
         | NotGiven = NOT_GIVEN,
         change_date: Optional[str] | NotGiven = NOT_GIVEN,
         coupon_redemption_code: Optional[str] | NotGiven = NOT_GIVEN,
         credits_overage_rate: Optional[float] | NotGiven = NOT_GIVEN,
         external_plan_id: Optional[str] | NotGiven = NOT_GIVEN,
         initial_phase_order: Optional[int] | NotGiven = NOT_GIVEN,
         invoicing_threshold: Optional[str] | NotGiven = NOT_GIVEN,
-        per_credit_overage_amount: Optional[str] | NotGiven = NOT_GIVEN,
+        per_credit_overage_amount: Optional[float] | NotGiven = NOT_GIVEN,
         plan_id: Optional[str] | NotGiven = NOT_GIVEN,
         price_overrides: Optional[Iterable[subscription_schedule_plan_change_params.PriceOverride]]
         | NotGiven = NOT_GIVEN,
         # Use the following arguments if you need to pass additional parameters to the API that aren't available via kwargs.
         # The extra values given here take precedence over values defined on the client or passed to this method.
         extra_headers: Headers | None = None,
         extra_query: Query | None = None,
```

### Comparing `orb_billing-1.50.1/src/orb/resources/top_level.py` & `orb_billing-1.51.0/src/orb/resources/top_level.py`

 * *Files identical despite different names*

### Comparing `orb_billing-1.50.1/src/orb/resources/webhooks.py` & `orb_billing-1.51.0/src/orb/resources/webhooks.py`

 * *Files identical despite different names*

### Comparing `orb_billing-1.50.1/src/orb/resources/coupons/__init__.py` & `orb_billing-1.51.0/src/orb/resources/coupons/__init__.py`

 * *Files identical despite different names*

### Comparing `orb_billing-1.50.1/src/orb/resources/coupons/coupons.py` & `orb_billing-1.51.0/src/orb/resources/coupons/coupons.py`

 * *Files identical despite different names*

### Comparing `orb_billing-1.50.1/src/orb/resources/coupons/subscriptions.py` & `orb_billing-1.51.0/src/orb/resources/coupons/subscriptions.py`

 * *Files identical despite different names*

### Comparing `orb_billing-1.50.1/src/orb/resources/customers/__init__.py` & `orb_billing-1.51.0/src/orb/resources/customers/__init__.py`

 * *Files identical despite different names*

### Comparing `orb_billing-1.50.1/src/orb/resources/customers/balance_transactions.py` & `orb_billing-1.51.0/src/orb/resources/customers/balance_transactions.py`

 * *Files identical despite different names*

### Comparing `orb_billing-1.50.1/src/orb/resources/customers/costs.py` & `orb_billing-1.51.0/src/orb/resources/customers/costs.py`

 * *Files identical despite different names*

### Comparing `orb_billing-1.50.1/src/orb/resources/customers/customers.py` & `orb_billing-1.51.0/src/orb/resources/customers/customers.py`

 * *Files identical despite different names*

### Comparing `orb_billing-1.50.1/src/orb/resources/customers/usage.py` & `orb_billing-1.51.0/src/orb/resources/customers/usage.py`

 * *Files identical despite different names*

### Comparing `orb_billing-1.50.1/src/orb/resources/customers/credits/__init__.py` & `orb_billing-1.51.0/src/orb/resources/customers/credits/__init__.py`

 * *Files identical despite different names*

### Comparing `orb_billing-1.50.1/src/orb/resources/customers/credits/credits.py` & `orb_billing-1.51.0/src/orb/resources/customers/credits/credits.py`

 * *Files identical despite different names*

### Comparing `orb_billing-1.50.1/src/orb/resources/customers/credits/ledger.py` & `orb_billing-1.51.0/src/orb/resources/customers/credits/ledger.py`

 * *Files identical despite different names*

### Comparing `orb_billing-1.50.1/src/orb/resources/customers/credits/top_ups.py` & `orb_billing-1.51.0/src/orb/resources/customers/credits/top_ups.py`

 * *Files identical despite different names*

### Comparing `orb_billing-1.50.1/src/orb/resources/events/__init__.py` & `orb_billing-1.51.0/src/orb/resources/events/__init__.py`

 * *Files identical despite different names*

### Comparing `orb_billing-1.50.1/src/orb/resources/events/backfills.py` & `orb_billing-1.51.0/src/orb/resources/events/backfills.py`

 * *Files identical despite different names*

### Comparing `orb_billing-1.50.1/src/orb/resources/events/events.py` & `orb_billing-1.51.0/src/orb/resources/events/events.py`

 * *Files 1% similar despite different names*

```diff
@@ -369,20 +369,18 @@
         Orb’s validation ensures that you recognize errors in your events as quickly as
         possible, and the API provides informative error messages to help you fix
         problems quickly.
 
         We validate the following:
 
         - Exactly one of `customer_id` and `external_customer_id` should be specified.
-        - If specified, `customer_id` must identify a Customer resource within Orb. We
-          do not support sending events for customers that have not been provisioned.
-          Similarly, if specified, `external_customer_id` must be an identifier that is
-          associated with an Orb Customer resource. Note: During our initial integration
-          period, this enforcement will be temporarily turned into a warning to ensure
-          smooth customer migration.
+        - If the `customer_id` is specified, the customer in Orb must exist.
+        - If the `external_customer_id` is specified, the customer in Orb does not need
+          to exist. Events will be attributed to any future customers with the
+          `external_customer_id` on subscription creation.
         - `timestamp` must conform to ISO 8601 and represent a timestamp at most 1 hour
           in the future. This timestamp should be sent in UTC timezone (no timezone
           offset).
 
         ## Idempotency and retry semantics
 
         Orb's idempotency guarantees allow you to implement safe retry logic in the
@@ -896,20 +894,18 @@
         Orb’s validation ensures that you recognize errors in your events as quickly as
         possible, and the API provides informative error messages to help you fix
         problems quickly.
 
         We validate the following:
 
         - Exactly one of `customer_id` and `external_customer_id` should be specified.
-        - If specified, `customer_id` must identify a Customer resource within Orb. We
-          do not support sending events for customers that have not been provisioned.
-          Similarly, if specified, `external_customer_id` must be an identifier that is
-          associated with an Orb Customer resource. Note: During our initial integration
-          period, this enforcement will be temporarily turned into a warning to ensure
-          smooth customer migration.
+        - If the `customer_id` is specified, the customer in Orb must exist.
+        - If the `external_customer_id` is specified, the customer in Orb does not need
+          to exist. Events will be attributed to any future customers with the
+          `external_customer_id` on subscription creation.
         - `timestamp` must conform to ISO 8601 and represent a timestamp at most 1 hour
           in the future. This timestamp should be sent in UTC timezone (no timezone
           offset).
 
         ## Idempotency and retry semantics
 
         Orb's idempotency guarantees allow you to implement safe retry logic in the
```

### Comparing `orb_billing-1.50.1/src/orb/resources/plans/__init__.py` & `orb_billing-1.51.0/src/orb/resources/plans/__init__.py`

 * *Files identical despite different names*

### Comparing `orb_billing-1.50.1/src/orb/resources/plans/external_plan_id.py` & `orb_billing-1.51.0/src/orb/resources/plans/external_plan_id.py`

 * *Files identical despite different names*

### Comparing `orb_billing-1.50.1/src/orb/resources/plans/plans.py` & `orb_billing-1.51.0/src/orb/resources/plans/plans.py`

 * *Files identical despite different names*

### Comparing `orb_billing-1.50.1/src/orb/resources/prices/__init__.py` & `orb_billing-1.51.0/src/orb/resources/prices/__init__.py`

 * *Files identical despite different names*

### Comparing `orb_billing-1.50.1/src/orb/resources/prices/external_price_id.py` & `orb_billing-1.51.0/src/orb/resources/prices/external_price_id.py`

 * *Files identical despite different names*

### Comparing `orb_billing-1.50.1/src/orb/resources/prices/prices.py` & `orb_billing-1.51.0/src/orb/resources/prices/prices.py`

 * *Files identical despite different names*

### Comparing `orb_billing-1.50.1/src/orb/types/__init__.py` & `orb_billing-1.51.0/src/orb/types/__init__.py`

 * *Files identical despite different names*

### Comparing `orb_billing-1.50.1/src/orb/types/alert.py` & `orb_billing-1.51.0/src/orb/types/alert.py`

 * *Files identical despite different names*

### Comparing `orb_billing-1.50.1/src/orb/types/alert_create_for_customer_params.py` & `orb_billing-1.51.0/src/orb/types/alert_create_for_customer_params.py`

 * *Files identical despite different names*

### Comparing `orb_billing-1.50.1/src/orb/types/alert_create_for_external_customer_params.py` & `orb_billing-1.51.0/src/orb/types/alert_create_for_external_customer_params.py`

 * *Files identical despite different names*

### Comparing `orb_billing-1.50.1/src/orb/types/alert_create_for_subscription_params.py` & `orb_billing-1.51.0/src/orb/types/alert_create_for_subscription_params.py`

 * *Files identical despite different names*

### Comparing `orb_billing-1.50.1/src/orb/types/alert_list_params.py` & `orb_billing-1.51.0/src/orb/types/alert_list_params.py`

 * *Files identical despite different names*

### Comparing `orb_billing-1.50.1/src/orb/types/coupon.py` & `orb_billing-1.51.0/src/orb/types/coupon.py`

 * *Files identical despite different names*

### Comparing `orb_billing-1.50.1/src/orb/types/coupon_create_params.py` & `orb_billing-1.51.0/src/orb/types/coupon_create_params.py`

 * *Files identical despite different names*

### Comparing `orb_billing-1.50.1/src/orb/types/coupon_list_params.py` & `orb_billing-1.51.0/src/orb/types/coupon_list_params.py`

 * *Files identical despite different names*

### Comparing `orb_billing-1.50.1/src/orb/types/credit_note.py` & `orb_billing-1.51.0/src/orb/types/credit_note.py`

 * *Files identical despite different names*

### Comparing `orb_billing-1.50.1/src/orb/types/customer.py` & `orb_billing-1.51.0/src/orb/types/customer.py`

 * *Files identical despite different names*

### Comparing `orb_billing-1.50.1/src/orb/types/customer_create_params.py` & `orb_billing-1.51.0/src/orb/types/customer_create_params.py`

 * *Files identical despite different names*

### Comparing `orb_billing-1.50.1/src/orb/types/customer_list_params.py` & `orb_billing-1.51.0/src/orb/types/customer_list_params.py`

 * *Files identical despite different names*

### Comparing `orb_billing-1.50.1/src/orb/types/customer_update_by_external_id_params.py` & `orb_billing-1.51.0/src/orb/types/customer_update_by_external_id_params.py`

 * *Files identical despite different names*

### Comparing `orb_billing-1.50.1/src/orb/types/customer_update_params.py` & `orb_billing-1.51.0/src/orb/types/customer_update_params.py`

 * *Files identical despite different names*

### Comparing `orb_billing-1.50.1/src/orb/types/event_ingest_params.py` & `orb_billing-1.51.0/src/orb/types/event_ingest_params.py`

 * *Files identical despite different names*

### Comparing `orb_billing-1.50.1/src/orb/types/event_ingest_response.py` & `orb_billing-1.51.0/src/orb/types/event_ingest_response.py`

 * *Files identical despite different names*

### Comparing `orb_billing-1.50.1/src/orb/types/event_search_params.py` & `orb_billing-1.51.0/src/orb/types/event_search_params.py`

 * *Files identical despite different names*

### Comparing `orb_billing-1.50.1/src/orb/types/event_search_response.py` & `orb_billing-1.51.0/src/orb/types/event_search_response.py`

 * *Files identical despite different names*

### Comparing `orb_billing-1.50.1/src/orb/types/event_update_params.py` & `orb_billing-1.51.0/src/orb/types/event_update_params.py`

 * *Files identical despite different names*

### Comparing `orb_billing-1.50.1/src/orb/types/invoice.py` & `orb_billing-1.51.0/src/orb/types/invoice.py`

 * *Files identical despite different names*

### Comparing `orb_billing-1.50.1/src/orb/types/invoice_create_params.py` & `orb_billing-1.51.0/src/orb/types/invoice_create_params.py`

 * *Files identical despite different names*

### Comparing `orb_billing-1.50.1/src/orb/types/invoice_fetch_upcoming_response.py` & `orb_billing-1.51.0/src/orb/types/invoice_fetch_upcoming_response.py`

 * *Files identical despite different names*

### Comparing `orb_billing-1.50.1/src/orb/types/invoice_line_item_create_params.py` & `orb_billing-1.51.0/src/orb/types/invoice_line_item_create_params.py`

 * *Files identical despite different names*

### Comparing `orb_billing-1.50.1/src/orb/types/invoice_line_item_create_response.py` & `orb_billing-1.51.0/src/orb/types/invoice_line_item_create_response.py`

 * *Files identical despite different names*

### Comparing `orb_billing-1.50.1/src/orb/types/invoice_list_params.py` & `orb_billing-1.51.0/src/orb/types/invoice_list_params.py`

 * *Files identical despite different names*

### Comparing `orb_billing-1.50.1/src/orb/types/invoice_mark_paid_params.py` & `orb_billing-1.51.0/src/orb/types/invoice_mark_paid_params.py`

 * *Files identical despite different names*

### Comparing `orb_billing-1.50.1/src/orb/types/item.py` & `orb_billing-1.51.0/src/orb/types/item.py`

 * *Files identical despite different names*

### Comparing `orb_billing-1.50.1/src/orb/types/metric_create_params.py` & `orb_billing-1.51.0/src/orb/types/metric_create_params.py`

 * *Files identical despite different names*

### Comparing `orb_billing-1.50.1/src/orb/types/metric_create_response.py` & `orb_billing-1.51.0/src/orb/types/metric_create_response.py`

 * *Files identical despite different names*

### Comparing `orb_billing-1.50.1/src/orb/types/metric_fetch_response.py` & `orb_billing-1.51.0/src/orb/types/metric_fetch_response.py`

 * *Files identical despite different names*

### Comparing `orb_billing-1.50.1/src/orb/types/metric_list_params.py` & `orb_billing-1.51.0/src/orb/types/metric_list_params.py`

 * *Files identical despite different names*

### Comparing `orb_billing-1.50.1/src/orb/types/metric_list_response.py` & `orb_billing-1.51.0/src/orb/types/metric_list_response.py`

 * *Files identical despite different names*

### Comparing `orb_billing-1.50.1/src/orb/types/plan.py` & `orb_billing-1.51.0/src/orb/types/plan.py`

 * *Files identical despite different names*

### Comparing `orb_billing-1.50.1/src/orb/types/plan_create_params.py` & `orb_billing-1.51.0/src/orb/types/plan_create_params.py`

 * *Files identical despite different names*

### Comparing `orb_billing-1.50.1/src/orb/types/plan_list_params.py` & `orb_billing-1.51.0/src/orb/types/plan_list_params.py`

 * *Files identical despite different names*

### Comparing `orb_billing-1.50.1/src/orb/types/plan_update_params.py` & `orb_billing-1.51.0/src/orb/types/plan_update_params.py`

 * *Files identical despite different names*

### Comparing `orb_billing-1.50.1/src/orb/types/price.py` & `orb_billing-1.51.0/src/orb/types/price.py`

 * *Files identical despite different names*

### Comparing `orb_billing-1.50.1/src/orb/types/price_create_params.py` & `orb_billing-1.51.0/src/orb/types/price_create_params.py`

 * *Files identical despite different names*

### Comparing `orb_billing-1.50.1/src/orb/types/price_evaluate_params.py` & `orb_billing-1.51.0/src/orb/types/price_evaluate_params.py`

 * *Files identical despite different names*

### Comparing `orb_billing-1.50.1/src/orb/types/subscription.py` & `orb_billing-1.51.0/src/orb/types/subscription.py`

 * *Files identical despite different names*

### Comparing `orb_billing-1.50.1/src/orb/types/subscription_cancel_params.py` & `orb_billing-1.51.0/src/orb/types/subscription_cancel_params.py`

 * *Files identical despite different names*

### Comparing `orb_billing-1.50.1/src/orb/types/subscription_create_params.py` & `orb_billing-1.51.0/src/orb/types/subscription_create_params.py`

 * *Files 0% similar despite different names*

```diff
@@ -91,15 +91,15 @@
 
     Individual keys can be removed by setting the value to `null`, and the entire
     metadata mapping can be cleared by setting `metadata` to `null`.
     """
 
     net_terms: Optional[int]
 
-    per_credit_overage_amount: Optional[str]
+    per_credit_overage_amount: Optional[float]
 
     plan_id: Optional[str]
     """The plan that the given subscription should be switched to.
 
     Note that either this property or `external_plan_id` must be specified.
     """
```

### Comparing `orb_billing-1.50.1/src/orb/types/subscription_fetch_costs_params.py` & `orb_billing-1.51.0/src/orb/types/subscription_fetch_costs_params.py`

 * *Files identical despite different names*

### Comparing `orb_billing-1.50.1/src/orb/types/subscription_fetch_costs_response.py` & `orb_billing-1.51.0/src/orb/types/subscription_fetch_costs_response.py`

 * *Files identical despite different names*

### Comparing `orb_billing-1.50.1/src/orb/types/subscription_fetch_schedule_params.py` & `orb_billing-1.51.0/src/orb/types/subscription_fetch_schedule_params.py`

 * *Files identical despite different names*

### Comparing `orb_billing-1.50.1/src/orb/types/subscription_fetch_schedule_response.py` & `orb_billing-1.51.0/src/orb/types/subscription_fetch_schedule_response.py`

 * *Files identical despite different names*

### Comparing `orb_billing-1.50.1/src/orb/types/subscription_fetch_usage_params.py` & `orb_billing-1.51.0/src/orb/types/subscription_fetch_usage_params.py`

 * *Files identical despite different names*

### Comparing `orb_billing-1.50.1/src/orb/types/subscription_list_params.py` & `orb_billing-1.51.0/src/orb/types/subscription_list_params.py`

 * *Files identical despite different names*

### Comparing `orb_billing-1.50.1/src/orb/types/subscription_price_intervals_params.py` & `orb_billing-1.51.0/src/orb/types/subscription_price_intervals_params.py`

 * *Files identical despite different names*

### Comparing `orb_billing-1.50.1/src/orb/types/subscription_schedule_plan_change_params.py` & `orb_billing-1.51.0/src/orb/types/subscription_schedule_plan_change_params.py`

 * *Files 0% similar despite different names*

```diff
@@ -93,15 +93,15 @@
     invoicing_threshold: Optional[str]
     """
     When this subscription's accrued usage reaches this threshold, an invoice will
     be issued for the subscription. If not specified, invoices will only be issued
     at the end of the billing period.
     """
 
-    per_credit_overage_amount: Optional[str]
+    per_credit_overage_amount: Optional[float]
 
     plan_id: Optional[str]
     """The plan that the given subscription should be switched to.
 
     Note that either this property or `external_plan_id` must be specified.
     """
```

### Comparing `orb_billing-1.50.1/src/orb/types/subscription_trigger_phase_params.py` & `orb_billing-1.51.0/src/orb/types/subscription_trigger_phase_params.py`

 * *Files identical despite different names*

### Comparing `orb_billing-1.50.1/src/orb/types/subscription_update_fixed_fee_quantity_params.py` & `orb_billing-1.51.0/src/orb/types/subscription_update_fixed_fee_quantity_params.py`

 * *Files identical despite different names*

### Comparing `orb_billing-1.50.1/src/orb/types/subscription_update_params.py` & `orb_billing-1.51.0/src/orb/types/subscription_update_params.py`

 * *Files identical despite different names*

### Comparing `orb_billing-1.50.1/src/orb/types/subscription_usage.py` & `orb_billing-1.51.0/src/orb/types/subscription_usage.py`

 * *Files identical despite different names*

### Comparing `orb_billing-1.50.1/src/orb/types/beta/price_evaluate_params.py` & `orb_billing-1.51.0/src/orb/types/beta/price_evaluate_params.py`

 * *Files identical despite different names*

### Comparing `orb_billing-1.50.1/src/orb/types/coupons/subscription_list_params.py` & `orb_billing-1.51.0/src/orb/types/coupons/subscription_list_params.py`

 * *Files identical despite different names*

### Comparing `orb_billing-1.50.1/src/orb/types/customers/__init__.py` & `orb_billing-1.51.0/src/orb/types/customers/__init__.py`

 * *Files identical despite different names*

### Comparing `orb_billing-1.50.1/src/orb/types/customers/balance_transaction_create_response.py` & `orb_billing-1.51.0/src/orb/types/customers/balance_transaction_create_response.py`

 * *Files identical despite different names*

### Comparing `orb_billing-1.50.1/src/orb/types/customers/balance_transaction_list_params.py` & `orb_billing-1.51.0/src/orb/types/customers/balance_transaction_list_params.py`

 * *Files identical despite different names*

### Comparing `orb_billing-1.50.1/src/orb/types/customers/balance_transaction_list_response.py` & `orb_billing-1.51.0/src/orb/types/customers/balance_transaction_list_response.py`

 * *Files identical despite different names*

### Comparing `orb_billing-1.50.1/src/orb/types/customers/cost_list_by_external_id_params.py` & `orb_billing-1.51.0/src/orb/types/customers/cost_list_by_external_id_params.py`

 * *Files identical despite different names*

### Comparing `orb_billing-1.50.1/src/orb/types/customers/cost_list_by_external_id_response.py` & `orb_billing-1.51.0/src/orb/types/customers/cost_list_by_external_id_response.py`

 * *Files identical despite different names*

### Comparing `orb_billing-1.50.1/src/orb/types/customers/cost_list_params.py` & `orb_billing-1.51.0/src/orb/types/customers/cost_list_params.py`

 * *Files identical despite different names*

### Comparing `orb_billing-1.50.1/src/orb/types/customers/cost_list_response.py` & `orb_billing-1.51.0/src/orb/types/customers/cost_list_response.py`

 * *Files identical despite different names*

### Comparing `orb_billing-1.50.1/src/orb/types/customers/credit_list_by_external_id_params.py` & `orb_billing-1.51.0/src/orb/types/customers/credit_list_by_external_id_params.py`

 * *Files identical despite different names*

### Comparing `orb_billing-1.50.1/src/orb/types/customers/credit_list_by_external_id_response.py` & `orb_billing-1.51.0/src/orb/types/customers/credit_list_by_external_id_response.py`

 * *Files identical despite different names*

### Comparing `orb_billing-1.50.1/src/orb/types/customers/credit_list_params.py` & `orb_billing-1.51.0/src/orb/types/customers/credit_list_params.py`

 * *Files identical despite different names*

### Comparing `orb_billing-1.50.1/src/orb/types/customers/usage_update_by_external_id_params.py` & `orb_billing-1.51.0/src/orb/types/customers/usage_update_by_external_id_params.py`

 * *Files identical despite different names*

### Comparing `orb_billing-1.50.1/src/orb/types/customers/usage_update_by_external_id_response.py` & `orb_billing-1.51.0/src/orb/types/customers/usage_update_by_external_id_response.py`

 * *Files identical despite different names*

### Comparing `orb_billing-1.50.1/src/orb/types/customers/usage_update_params.py` & `orb_billing-1.51.0/src/orb/types/customers/usage_update_params.py`

 * *Files identical despite different names*

### Comparing `orb_billing-1.50.1/src/orb/types/customers/credits/__init__.py` & `orb_billing-1.51.0/src/orb/types/customers/credits/__init__.py`

 * *Files identical despite different names*

### Comparing `orb_billing-1.50.1/src/orb/types/customers/credits/ledger_create_entry_by_external_id_params.py` & `orb_billing-1.51.0/src/orb/types/customers/credits/ledger_create_entry_by_external_id_params.py`

 * *Files identical despite different names*

### Comparing `orb_billing-1.50.1/src/orb/types/customers/credits/ledger_create_entry_by_external_id_response.py` & `orb_billing-1.51.0/src/orb/types/customers/credits/ledger_create_entry_by_external_id_response.py`

 * *Files identical despite different names*

### Comparing `orb_billing-1.50.1/src/orb/types/customers/credits/ledger_create_entry_params.py` & `orb_billing-1.51.0/src/orb/types/customers/credits/ledger_create_entry_params.py`

 * *Files identical despite different names*

### Comparing `orb_billing-1.50.1/src/orb/types/customers/credits/ledger_create_entry_response.py` & `orb_billing-1.51.0/src/orb/types/customers/credits/ledger_create_entry_response.py`

 * *Files identical despite different names*

### Comparing `orb_billing-1.50.1/src/orb/types/customers/credits/ledger_list_by_external_id_params.py` & `orb_billing-1.51.0/src/orb/types/customers/credits/ledger_list_by_external_id_params.py`

 * *Files identical despite different names*

### Comparing `orb_billing-1.50.1/src/orb/types/customers/credits/ledger_list_by_external_id_response.py` & `orb_billing-1.51.0/src/orb/types/customers/credits/ledger_list_by_external_id_response.py`

 * *Files identical despite different names*

### Comparing `orb_billing-1.50.1/src/orb/types/customers/credits/ledger_list_params.py` & `orb_billing-1.51.0/src/orb/types/customers/credits/ledger_list_params.py`

 * *Files identical despite different names*

### Comparing `orb_billing-1.50.1/src/orb/types/customers/credits/ledger_list_response.py` & `orb_billing-1.51.0/src/orb/types/customers/credits/ledger_list_response.py`

 * *Files identical despite different names*

### Comparing `orb_billing-1.50.1/src/orb/types/customers/credits/top_up_create_by_external_id_params.py` & `orb_billing-1.51.0/src/orb/types/customers/credits/top_up_create_by_external_id_params.py`

 * *Files identical despite different names*

### Comparing `orb_billing-1.50.1/src/orb/types/customers/credits/top_up_create_by_external_id_response.py` & `orb_billing-1.51.0/src/orb/types/customers/credits/top_up_create_by_external_id_response.py`

 * *Files identical despite different names*

### Comparing `orb_billing-1.50.1/src/orb/types/customers/credits/top_up_create_params.py` & `orb_billing-1.51.0/src/orb/types/customers/credits/top_up_create_params.py`

 * *Files identical despite different names*

### Comparing `orb_billing-1.50.1/src/orb/types/customers/credits/top_up_create_response.py` & `orb_billing-1.51.0/src/orb/types/customers/credits/top_up_create_response.py`

 * *Files identical despite different names*

### Comparing `orb_billing-1.50.1/src/orb/types/customers/credits/top_up_list_by_external_id_params.py` & `orb_billing-1.51.0/src/orb/types/customers/credits/top_up_list_by_external_id_params.py`

 * *Files identical despite different names*

### Comparing `orb_billing-1.50.1/src/orb/types/customers/credits/top_up_list_by_external_id_response.py` & `orb_billing-1.51.0/src/orb/types/customers/credits/top_up_list_by_external_id_response.py`

 * *Files identical despite different names*

### Comparing `orb_billing-1.50.1/src/orb/types/customers/credits/top_up_list_response.py` & `orb_billing-1.51.0/src/orb/types/customers/credits/top_up_list_response.py`

 * *Files identical despite different names*

### Comparing `orb_billing-1.50.1/src/orb/types/events/__init__.py` & `orb_billing-1.51.0/src/orb/types/events/__init__.py`

 * *Files identical despite different names*

### Comparing `orb_billing-1.50.1/src/orb/types/events/backfill_close_response.py` & `orb_billing-1.51.0/src/orb/types/events/backfill_close_response.py`

 * *Files identical despite different names*

### Comparing `orb_billing-1.50.1/src/orb/types/events/backfill_create_params.py` & `orb_billing-1.51.0/src/orb/types/events/backfill_create_params.py`

 * *Files identical despite different names*

### Comparing `orb_billing-1.50.1/src/orb/types/events/backfill_create_response.py` & `orb_billing-1.51.0/src/orb/types/events/backfill_create_response.py`

 * *Files identical despite different names*

### Comparing `orb_billing-1.50.1/src/orb/types/events/backfill_fetch_response.py` & `orb_billing-1.51.0/src/orb/types/events/backfill_fetch_response.py`

 * *Files identical despite different names*

### Comparing `orb_billing-1.50.1/src/orb/types/events/backfill_list_response.py` & `orb_billing-1.51.0/src/orb/types/events/backfill_list_response.py`

 * *Files identical despite different names*

### Comparing `orb_billing-1.50.1/src/orb/types/events/backfill_revert_response.py` & `orb_billing-1.51.0/src/orb/types/events/backfill_revert_response.py`

 * *Files identical despite different names*

### Comparing `orb_billing-1.50.1/src/orb/types/plans/external_plan_id_update_params.py` & `orb_billing-1.51.0/src/orb/types/plans/external_plan_id_update_params.py`

 * *Files identical despite different names*

### Comparing `orb_billing-1.50.1/src/orb/types/shared/discount.py` & `orb_billing-1.51.0/src/orb/types/shared/discount.py`

 * *Files identical despite different names*

### Comparing `orb_billing-1.50.1/LICENSE` & `orb_billing-1.51.0/LICENSE`

 * *Files identical despite different names*

### Comparing `orb_billing-1.50.1/pyproject.toml` & `orb_billing-1.51.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "orb-billing"
-version = "1.50.1"
+version = "1.51.0"
 description = "The official Python library for the orb API"
 dynamic = ["readme"]
 license = "Apache-2.0"
 authors = [
 { name = "Orb", email = "team@withorb.com" },
 ]
 dependencies = [
```

### Comparing `orb_billing-1.50.1/PKG-INFO` & `orb_billing-1.51.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: orb-billing
-Version: 1.50.1
+Version: 1.51.0
 Summary: The official Python library for the orb API
 Project-URL: Homepage, https://github.com/orbcorp/orb-python
 Project-URL: Repository, https://github.com/orbcorp/orb-python
 Author-email: Orb <team@withorb.com>
 License-Expression: Apache-2.0
 License-File: LICENSE
 Classifier: Intended Audience :: Developers
```
