# Comparing `tmp/yandex_api_client-0.0.1.tar.gz` & `tmp/yandex_api_client-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "yandex_api_client-0.0.1.tar", max compression
+gzip compressed data, was "yandex_api_client-0.0.2.tar", max compression
```

## Comparing `yandex_api_client-0.0.1.tar` & `yandex_api_client-0.0.2.tar`

### file list

```diff
@@ -1,548 +1,548 @@
--rw-r--r--   0        0        0   124349 2024-04-09 12:18:56.000000 yandex_api_client-0.0.1/README.md
--rw-r--r--   0        0        0      737 2024-04-09 12:25:21.329816 yandex_api_client-0.0.1/pyproject.toml
--rw-r--r--   0        0        0    45454 2024-04-09 12:18:56.000000 yandex_api_client-0.0.1/yandex_api_client/__init__.py
--rw-r--r--   0        0        0     2213 2024-04-09 12:18:56.000000 yandex_api_client-0.0.1/yandex_api_client/api/__init__.py
--rw-r--r--   0        0        0    90394 2024-04-09 12:18:56.000000 yandex_api_client-0.0.1/yandex_api_client/api/bids_api.py
--rw-r--r--   0        0        0   112390 2024-04-09 12:18:56.000000 yandex_api_client-0.0.1/yandex_api_client/api/business_offer_mappings_api.py
--rw-r--r--   0        0        0    90231 2024-04-09 12:18:56.000000 yandex_api_client-0.0.1/yandex_api_client/api/campaigns_api.py
--rw-r--r--   0        0        0    11904 2024-04-09 12:18:56.000000 yandex_api_client-0.0.1/yandex_api_client/api/categories_api.py
--rw-r--r--   0        0        0    87315 2024-04-09 12:18:56.000000 yandex_api_client-0.0.1/yandex_api_client/api/chats_api.py
--rw-r--r--   0        0        0    55369 2024-04-09 12:18:56.000000 yandex_api_client-0.0.1/yandex_api_client/api/content_api.py
--rw-r--r--   0        0        0  2022454 2024-04-09 12:18:56.000000 yandex_api_client-0.0.1/yandex_api_client/api/dbs_api.py
--rw-r--r--   0        0        0    12196 2024-04-09 12:18:56.000000 yandex_api_client-0.0.1/yandex_api_client/api/delivery_services_api.py
--rw-r--r--   0        0        0  1401649 2024-04-09 12:18:56.000000 yandex_api_client-0.0.1/yandex_api_client/api/express_api.py
--rw-r--r--   0        0        0  1788698 2024-04-09 12:18:56.000000 yandex_api_client-0.0.1/yandex_api_client/api/fbs_api.py
--rw-r--r--   0        0        0  1189525 2024-04-09 12:18:56.000000 yandex_api_client-0.0.1/yandex_api_client/api/fby_api.py
--rw-r--r--   0        0        0    49736 2024-04-09 12:18:56.000000 yandex_api_client-0.0.1/yandex_api_client/api/feed_categories_api.py
--rw-r--r--   0        0        0    24266 2024-04-09 12:18:56.000000 yandex_api_client-0.0.1/yandex_api_client/api/feedbacks_api.py
--rw-r--r--   0        0        0   103931 2024-04-09 12:18:56.000000 yandex_api_client-0.0.1/yandex_api_client/api/feeds_api.py
--rw-r--r--   0        0        0    19823 2024-04-09 12:18:56.000000 yandex_api_client-0.0.1/yandex_api_client/api/goods_stats_api.py
--rw-r--r--   0        0        0    63690 2024-04-09 12:18:56.000000 yandex_api_client-0.0.1/yandex_api_client/api/hidden_offers_api.py
--rw-r--r--   0        0        0   129885 2024-04-09 12:18:56.000000 yandex_api_client-0.0.1/yandex_api_client/api/models_api.py
--rw-r--r--   0        0        0   113854 2024-04-09 12:18:56.000000 yandex_api_client-0.0.1/yandex_api_client/api/offer_mappings_api.py
--rw-r--r--   0        0        0   141946 2024-04-09 12:18:56.000000 yandex_api_client-0.0.1/yandex_api_client/api/offers_api.py
--rw-r--r--   0        0        0    33987 2024-04-09 12:18:56.000000 yandex_api_client-0.0.1/yandex_api_client/api/order_business_information_api.py
--rw-r--r--   0        0        0    94574 2024-04-09 12:18:56.000000 yandex_api_client-0.0.1/yandex_api_client/api/order_delivery_api.py
--rw-r--r--   0        0        0    54373 2024-04-09 12:18:56.000000 yandex_api_client-0.0.1/yandex_api_client/api/order_labels_api.py
--rw-r--r--   0        0        0   300755 2024-04-09 12:18:56.000000 yandex_api_client-0.0.1/yandex_api_client/api/orders_api.py
--rw-r--r--   0        0        0    24751 2024-04-09 12:18:56.000000 yandex_api_client-0.0.1/yandex_api_client/api/orders_stats_api.py
--rw-r--r--   0        0        0    57754 2024-04-09 12:18:56.000000 yandex_api_client-0.0.1/yandex_api_client/api/outlet_licenses_api.py
--rw-r--r--   0        0        0    95593 2024-04-09 12:18:56.000000 yandex_api_client-0.0.1/yandex_api_client/api/outlets_api.py
--rw-r--r--   0        0        0    84650 2024-04-09 12:18:56.000000 yandex_api_client-0.0.1/yandex_api_client/api/price_quarantine_api.py
--rw-r--r--   0        0        0   100684 2024-04-09 12:18:56.000000 yandex_api_client-0.0.1/yandex_api_client/api/prices_api.py
--rw-r--r--   0        0        0    54645 2024-04-09 12:18:56.000000 yandex_api_client-0.0.1/yandex_api_client/api/regions_api.py
--rw-r--r--   0        0        0   172650 2024-04-09 12:18:56.000000 yandex_api_client-0.0.1/yandex_api_client/api/reports_api.py
--rw-r--r--   0        0        0   120073 2024-04-09 12:18:56.000000 yandex_api_client-0.0.1/yandex_api_client/api/returns_api.py
--rw-r--r--   0        0        0   227303 2024-04-09 12:18:56.000000 yandex_api_client-0.0.1/yandex_api_client/api/shipments_api.py
--rw-r--r--   0        0        0    41006 2024-04-09 12:18:56.000000 yandex_api_client-0.0.1/yandex_api_client/api/stocks_api.py
--rw-r--r--   0        0        0    15857 2024-04-09 12:18:56.000000 yandex_api_client-0.0.1/yandex_api_client/api/tariffs_api.py
--rw-r--r--   0        0        0    27100 2024-04-09 12:18:56.000000 yandex_api_client-0.0.1/yandex_api_client/api/warehouses_api.py
--rw-r--r--   0        0        0    25001 2024-04-09 12:18:56.000000 yandex_api_client-0.0.1/yandex_api_client/api_client.py
--rw-r--r--   0        0        0      674 2024-04-09 12:18:56.000000 yandex_api_client-0.0.1/yandex_api_client/api_response.py
--rw-r--r--   0        0        0    15057 2024-04-09 12:18:56.000000 yandex_api_client-0.0.1/yandex_api_client/configuration.py
--rw-r--r--   0        0        0     6343 2024-04-09 12:18:56.000000 yandex_api_client-0.0.1/yandex_api_client/exceptions.py
--rw-r--r--   0        0        0    42718 2024-04-09 12:18:56.000000 yandex_api_client-0.0.1/yandex_api_client/models/__init__.py
--rw-r--r--   0        0        0     3519 2024-04-09 12:18:54.000000 yandex_api_client-0.0.1/yandex_api_client/models/accept_order_cancellation_request.py
--rw-r--r--   0        0        0     3547 2024-04-09 12:18:54.000000 yandex_api_client-0.0.1/yandex_api_client/models/add_hidden_offers_request.py
--rw-r--r--   0        0        0     3684 2024-04-09 12:18:54.000000 yandex_api_client-0.0.1/yandex_api_client/models/add_offers_to_archive_dto.py
--rw-r--r--   0        0        0     4671 2024-04-09 12:18:54.000000 yandex_api_client-0.0.1/yandex_api_client/models/add_offers_to_archive_error_dto.py
--rw-r--r--   0        0        0     1446 2024-04-09 12:18:54.000000 yandex_api_client-0.0.1/yandex_api_client/models/add_offers_to_archive_error_type.py
--rw-r--r--   0        0        0     3181 2024-04-09 12:18:54.000000 yandex_api_client-0.0.1/yandex_api_client/models/add_offers_to_archive_request.py
--rw-r--r--   0        0        0     3379 2024-04-09 12:18:54.000000 yandex_api_client-0.0.1/yandex_api_client/models/add_offers_to_archive_response.py
--rw-r--r--   0        0        0     3152 2024-04-09 12:18:54.000000 yandex_api_client-0.0.1/yandex_api_client/models/age_dto.py
--rw-r--r--   0        0        0     1297 2024-04-09 12:18:54.000000 yandex_api_client-0.0.1/yandex_api_client/models/age_unit_type.py
--rw-r--r--   0        0        0     3605 2024-04-09 12:18:54.000000 yandex_api_client-0.0.1/yandex_api_client/models/api_client_data_error_response.py
--rw-r--r--   0        0        0     3010 2024-04-09 12:18:54.000000 yandex_api_client-0.0.1/yandex_api_client/models/api_error_dto.py
--rw-r--r--   0        0        0     3578 2024-04-09 12:18:54.000000 yandex_api_client-0.0.1/yandex_api_client/models/api_error_response.py
--rw-r--r--   0        0        0     3714 2024-04-09 12:18:54.000000 yandex_api_client-0.0.1/yandex_api_client/models/api_forbidden_error_response.py
--rw-r--r--   0        0        0     3598 2024-04-09 12:18:54.000000 yandex_api_client-0.0.1/yandex_api_client/models/api_limit_error_response.py
--rw-r--r--   0        0        0     3653 2024-04-09 12:18:54.000000 yandex_api_client-0.0.1/yandex_api_client/models/api_locked_error_response.py
--rw-r--r--   0        0        0     3587 2024-04-09 12:18:54.000000 yandex_api_client-0.0.1/yandex_api_client/models/api_not_found_error_response.py
--rw-r--r--   0        0        0     2932 2024-04-09 12:18:54.000000 yandex_api_client-0.0.1/yandex_api_client/models/api_response.py
--rw-r--r--   0        0        0     1233 2024-04-09 12:18:54.000000 yandex_api_client-0.0.1/yandex_api_client/models/api_response_status_type.py
--rw-r--r--   0        0        0     3572 2024-04-09 12:18:54.000000 yandex_api_client-0.0.1/yandex_api_client/models/api_server_error_response.py
--rw-r--r--   0        0        0     3623 2024-04-09 12:18:54.000000 yandex_api_client-0.0.1/yandex_api_client/models/api_unauthorized_error_response.py
--rw-r--r--   0        0        0     5034 2024-04-09 12:18:54.000000 yandex_api_client-0.0.1/yandex_api_client/models/base_campaign_offer_dto.py
--rw-r--r--   0        0        0    20952 2024-04-09 12:18:54.000000 yandex_api_client-0.0.1/yandex_api_client/models/base_offer_dto.py
--rw-r--r--   0        0        0     3140 2024-04-09 12:18:54.000000 yandex_api_client-0.0.1/yandex_api_client/models/base_price_dto.py
--rw-r--r--   0        0        0     3215 2024-04-09 12:18:54.000000 yandex_api_client-0.0.1/yandex_api_client/models/bid_recommendation_item_dto.py
--rw-r--r--   0        0        0     6779 2024-04-09 12:18:54.000000 yandex_api_client-0.0.1/yandex_api_client/models/brief_order_item_dto.py
--rw-r--r--   0        0        0     5192 2024-04-09 12:18:54.000000 yandex_api_client-0.0.1/yandex_api_client/models/brief_order_item_instance_dto.py
--rw-r--r--   0        0        0     3055 2024-04-09 12:18:54.000000 yandex_api_client-0.0.1/yandex_api_client/models/business_dto.py
--rw-r--r--   0        0        0     4748 2024-04-09 12:18:54.000000 yandex_api_client-0.0.1/yandex_api_client/models/calculate_tariffs_offer_dto.py
--rw-r--r--   0        0        0     4370 2024-04-09 12:18:54.000000 yandex_api_client-0.0.1/yandex_api_client/models/calculate_tariffs_offer_info_dto.py
--rw-r--r--   0        0        0     4036 2024-04-09 12:18:54.000000 yandex_api_client-0.0.1/yandex_api_client/models/calculate_tariffs_parameters_dto.py
--rw-r--r--   0        0        0     4016 2024-04-09 12:18:54.000000 yandex_api_client-0.0.1/yandex_api_client/models/calculate_tariffs_request.py
--rw-r--r--   0        0        0     3367 2024-04-09 12:18:54.000000 yandex_api_client-0.0.1/yandex_api_client/models/calculate_tariffs_response.py
--rw-r--r--   0        0        0     3435 2024-04-09 12:18:54.000000 yandex_api_client-0.0.1/yandex_api_client/models/calculate_tariffs_response_dto.py
--rw-r--r--   0        0        0     3863 2024-04-09 12:18:54.000000 yandex_api_client-0.0.1/yandex_api_client/models/calculated_tariff_dto.py
--rw-r--r--   0        0        0     2302 2024-04-09 12:18:54.000000 yandex_api_client-0.0.1/yandex_api_client/models/calculated_tariff_type.py
--rw-r--r--   0        0        0     3907 2024-04-09 12:18:54.000000 yandex_api_client-0.0.1/yandex_api_client/models/campaign_dto.py
--rw-r--r--   0        0        0     3271 2024-04-09 12:18:54.000000 yandex_api_client-0.0.1/yandex_api_client/models/campaign_settings_delivery_dto.py
--rw-r--r--   0        0        0     5631 2024-04-09 12:18:54.000000 yandex_api_client-0.0.1/yandex_api_client/models/campaign_settings_dto.py
--rw-r--r--   0        0        0     4078 2024-04-09 12:18:54.000000 yandex_api_client-0.0.1/yandex_api_client/models/campaign_settings_local_region_dto.py
--rw-r--r--   0        0        0     5568 2024-04-09 12:18:54.000000 yandex_api_client-0.0.1/yandex_api_client/models/campaign_settings_schedule_dto.py
--rw-r--r--   0        0        0     1630 2024-04-09 12:18:54.000000 yandex_api_client-0.0.1/yandex_api_client/models/campaign_settings_schedule_source_type.py
--rw-r--r--   0        0        0     3290 2024-04-09 12:18:54.000000 yandex_api_client-0.0.1/yandex_api_client/models/campaign_settings_time_period_dto.py
--rw-r--r--   0        0        0     3955 2024-04-09 12:18:54.000000 yandex_api_client-0.0.1/yandex_api_client/models/category_content_parameters_dto.py
--rw-r--r--   0        0        0     3769 2024-04-09 12:18:54.000000 yandex_api_client-0.0.1/yandex_api_client/models/category_dto.py
--rw-r--r--   0        0        0     7672 2024-04-09 12:18:54.000000 yandex_api_client-0.0.1/yandex_api_client/models/category_parameter_dto.py
--rw-r--r--   0        0        0     3607 2024-04-09 12:18:54.000000 yandex_api_client-0.0.1/yandex_api_client/models/category_parameter_unit_dto.py
--rw-r--r--   0        0        0     6847 2024-04-09 12:18:54.000000 yandex_api_client-0.0.1/yandex_api_client/models/change_outlet_request.py
--rw-r--r--   0        0        0     4556 2024-04-09 12:18:54.000000 yandex_api_client-0.0.1/yandex_api_client/models/chat_message_dto.py
--rw-r--r--   0        0        0     3195 2024-04-09 12:18:54.000000 yandex_api_client-0.0.1/yandex_api_client/models/chat_message_payload_dto.py
--rw-r--r--   0        0        0     1503 2024-04-09 12:18:54.000000 yandex_api_client-0.0.1/yandex_api_client/models/chat_message_sender_type.py
--rw-r--r--   0        0        0     3863 2024-04-09 12:18:54.000000 yandex_api_client-0.0.1/yandex_api_client/models/chat_messages_result_dto.py
--rw-r--r--   0        0        0     1768 2024-04-09 12:18:54.000000 yandex_api_client-0.0.1/yandex_api_client/models/chat_status_type.py
--rw-r--r--   0        0        0     1292 2024-04-09 12:18:54.000000 yandex_api_client-0.0.1/yandex_api_client/models/chat_type.py
--rw-r--r--   0        0        0     3112 2024-04-09 12:18:54.000000 yandex_api_client-0.0.1/yandex_api_client/models/confirm_prices_request.py
--rw-r--r--   0        0        0     3088 2024-04-09 12:18:54.000000 yandex_api_client-0.0.1/yandex_api_client/models/confirm_shipment_request.py
--rw-r--r--   0        0        0     2966 2024-04-09 12:18:54.000000 yandex_api_client-0.0.1/yandex_api_client/models/create_chat_request.py
--rw-r--r--   0        0        0     3338 2024-04-09 12:18:54.000000 yandex_api_client-0.0.1/yandex_api_client/models/create_chat_response.py
--rw-r--r--   0        0        0     2925 2024-04-09 12:18:54.000000 yandex_api_client-0.0.1/yandex_api_client/models/create_chat_result_dto.py
--rw-r--r--   0        0        0     3363 2024-04-09 12:18:54.000000 yandex_api_client-0.0.1/yandex_api_client/models/create_outlet_response.py
--rw-r--r--   0        0        0     3373 2024-04-09 12:18:54.000000 yandex_api_client-0.0.1/yandex_api_client/models/currency_type.py
--rw-r--r--   0        0        0     1594 2024-04-09 12:18:54.000000 yandex_api_client-0.0.1/yandex_api_client/models/day_of_week_type.py
--rw-r--r--   0        0        0     3225 2024-04-09 12:18:54.000000 yandex_api_client-0.0.1/yandex_api_client/models/delete_campaign_offers_dto.py
--rw-r--r--   0        0        0     3159 2024-04-09 12:18:54.000000 yandex_api_client-0.0.1/yandex_api_client/models/delete_campaign_offers_request.py
--rw-r--r--   0        0        0     3390 2024-04-09 12:18:54.000000 yandex_api_client-0.0.1/yandex_api_client/models/delete_campaign_offers_response.py
--rw-r--r--   0        0        0     3581 2024-04-09 12:18:54.000000 yandex_api_client-0.0.1/yandex_api_client/models/delete_hidden_offers_request.py
--rw-r--r--   0        0        0     3267 2024-04-09 12:18:54.000000 yandex_api_client-0.0.1/yandex_api_client/models/delete_offers_dto.py
--rw-r--r--   0        0        0     3274 2024-04-09 12:18:54.000000 yandex_api_client-0.0.1/yandex_api_client/models/delete_offers_from_archive_dto.py
--rw-r--r--   0        0        0     3216 2024-04-09 12:18:54.000000 yandex_api_client-0.0.1/yandex_api_client/models/delete_offers_from_archive_request.py
--rw-r--r--   0        0        0     3420 2024-04-09 12:18:54.000000 yandex_api_client-0.0.1/yandex_api_client/models/delete_offers_from_archive_response.py
--rw-r--r--   0        0        0     3145 2024-04-09 12:18:54.000000 yandex_api_client-0.0.1/yandex_api_client/models/delete_offers_request.py
--rw-r--r--   0        0        0     3333 2024-04-09 12:18:54.000000 yandex_api_client-0.0.1/yandex_api_client/models/delete_offers_response.py
--rw-r--r--   0        0        0     3101 2024-04-09 12:18:54.000000 yandex_api_client-0.0.1/yandex_api_client/models/delivery_service_dto.py
--rw-r--r--   0        0        0     3079 2024-04-09 12:18:54.000000 yandex_api_client-0.0.1/yandex_api_client/models/delivery_service_info_dto.py
--rw-r--r--   0        0        0     3567 2024-04-09 12:18:54.000000 yandex_api_client-0.0.1/yandex_api_client/models/delivery_services_dto.py
--rw-r--r--   0        0        0     3291 2024-04-09 12:18:54.000000 yandex_api_client-0.0.1/yandex_api_client/models/document_dto.py
--rw-r--r--   0        0        0     3538 2024-04-09 12:18:54.000000 yandex_api_client-0.0.1/yandex_api_client/models/eac_verification_result_dto.py
--rw-r--r--   0        0        0     1622 2024-04-09 12:18:54.000000 yandex_api_client-0.0.1/yandex_api_client/models/eac_verification_status_type.py
--rw-r--r--   0        0        0     2911 2024-04-09 12:18:54.000000 yandex_api_client-0.0.1/yandex_api_client/models/empty_api_response.py
--rw-r--r--   0        0        0    24444 2024-04-09 12:18:54.000000 yandex_api_client-0.0.1/yandex_api_client/models/enriched_mappings_offer_dto.py
--rw-r--r--   0        0        0     5279 2024-04-09 12:18:54.000000 yandex_api_client-0.0.1/yandex_api_client/models/enriched_model_dto.py
--rw-r--r--   0        0        0     3822 2024-04-09 12:18:54.000000 yandex_api_client-0.0.1/yandex_api_client/models/enriched_order_box_layout_dto.py
--rw-r--r--   0        0        0     3546 2024-04-09 12:18:54.000000 yandex_api_client-0.0.1/yandex_api_client/models/feed_category_dto.py
--rw-r--r--   0        0        0     4162 2024-04-09 12:18:54.000000 yandex_api_client-0.0.1/yandex_api_client/models/feed_content_dto.py
--rw-r--r--   0        0        0     3026 2024-04-09 12:18:54.000000 yandex_api_client-0.0.1/yandex_api_client/models/feed_content_error_dto.py
--rw-r--r--   0        0        0     2144 2024-04-09 12:18:54.000000 yandex_api_client-0.0.1/yandex_api_client/models/feed_content_error_type.py
--rw-r--r--   0        0        0     3339 2024-04-09 12:18:54.000000 yandex_api_client-0.0.1/yandex_api_client/models/feed_download_dto.py
--rw-r--r--   0        0        0     3611 2024-04-09 12:18:54.000000 yandex_api_client-0.0.1/yandex_api_client/models/feed_download_error_dto.py
--rw-r--r--   0        0        0     1897 2024-04-09 12:18:54.000000 yandex_api_client-0.0.1/yandex_api_client/models/feed_download_error_type.py
--rw-r--r--   0        0        0     6395 2024-04-09 12:18:54.000000 yandex_api_client-0.0.1/yandex_api_client/models/feed_dto.py
--rw-r--r--   0        0        0     3722 2024-04-09 12:18:54.000000 yandex_api_client-0.0.1/yandex_api_client/models/feed_index_logs_error_dto.py
--rw-r--r--   0        0        0     2790 2024-04-09 12:18:54.000000 yandex_api_client-0.0.1/yandex_api_client/models/feed_index_logs_error_type.py
--rw-r--r--   0        0        0     2936 2024-04-09 12:18:54.000000 yandex_api_client-0.0.1/yandex_api_client/models/feed_index_logs_feed_dto.py
--rw-r--r--   0        0        0     1778 2024-04-09 12:18:54.000000 yandex_api_client-0.0.1/yandex_api_client/models/feed_index_logs_index_type.py
--rw-r--r--   0        0        0     3365 2024-04-09 12:18:54.000000 yandex_api_client-0.0.1/yandex_api_client/models/feed_index_logs_offers_dto.py
--rw-r--r--   0        0        0     5508 2024-04-09 12:18:54.000000 yandex_api_client-0.0.1/yandex_api_client/models/feed_index_logs_record_dto.py
--rw-r--r--   0        0        0     4292 2024-04-09 12:18:54.000000 yandex_api_client-0.0.1/yandex_api_client/models/feed_index_logs_result_dto.py
--rw-r--r--   0        0        0     1610 2024-04-09 12:18:54.000000 yandex_api_client-0.0.1/yandex_api_client/models/feed_index_logs_status_type.py
--rw-r--r--   0        0        0     4144 2024-04-09 12:18:54.000000 yandex_api_client-0.0.1/yandex_api_client/models/feed_parameter_dto.py
--rw-r--r--   0        0        0     3441 2024-04-09 12:18:54.000000 yandex_api_client-0.0.1/yandex_api_client/models/feed_placement_dto.py
--rw-r--r--   0        0        0     4089 2024-04-09 12:18:54.000000 yandex_api_client-0.0.1/yandex_api_client/models/feed_publication_dto.py
--rw-r--r--   0        0        0     3688 2024-04-09 12:18:54.000000 yandex_api_client-0.0.1/yandex_api_client/models/feed_publication_full_dto.py
--rw-r--r--   0        0        0     3967 2024-04-09 12:18:54.000000 yandex_api_client-0.0.1/yandex_api_client/models/feed_publication_price_and_stock_update_dto.py
--rw-r--r--   0        0        0     1539 2024-04-09 12:18:54.000000 yandex_api_client-0.0.1/yandex_api_client/models/feed_status_type.py
--rw-r--r--   0        0        0     3403 2024-04-09 12:18:54.000000 yandex_api_client-0.0.1/yandex_api_client/models/feedback_author_dto.py
--rw-r--r--   0        0        0     3177 2024-04-09 12:18:54.000000 yandex_api_client-0.0.1/yandex_api_client/models/feedback_comment_author_dto.py
--rw-r--r--   0        0        0     1326 2024-04-09 12:18:54.000000 yandex_api_client-0.0.1/yandex_api_client/models/feedback_comment_author_type.py
--rw-r--r--   0        0        0     5115 2024-04-09 12:18:54.000000 yandex_api_client-0.0.1/yandex_api_client/models/feedback_comment_dto.py
--rw-r--r--   0        0        0     1422 2024-04-09 12:18:54.000000 yandex_api_client-0.0.1/yandex_api_client/models/feedback_delivery_type.py
--rw-r--r--   0        0        0     7363 2024-04-09 12:18:54.000000 yandex_api_client-0.0.1/yandex_api_client/models/feedback_dto.py
--rw-r--r--   0        0        0     4226 2024-04-09 12:18:54.000000 yandex_api_client-0.0.1/yandex_api_client/models/feedback_factor_dto.py
--rw-r--r--   0        0        0     4961 2024-04-09 12:18:54.000000 yandex_api_client-0.0.1/yandex_api_client/models/feedback_grades_dto.py
--rw-r--r--   0        0        0     3966 2024-04-09 12:18:54.000000 yandex_api_client-0.0.1/yandex_api_client/models/feedback_list_dto.py
--rw-r--r--   0        0        0     3211 2024-04-09 12:18:54.000000 yandex_api_client-0.0.1/yandex_api_client/models/feedback_order_dto.py
--rw-r--r--   0        0        0     2909 2024-04-09 12:18:54.000000 yandex_api_client-0.0.1/yandex_api_client/models/feedback_shop_dto.py
--rw-r--r--   0        0        0     1361 2024-04-09 12:18:54.000000 yandex_api_client-0.0.1/yandex_api_client/models/feedback_state_type.py
--rw-r--r--   0        0        0     1496 2024-04-09 12:18:54.000000 yandex_api_client-0.0.1/yandex_api_client/models/field_state_type.py
--rw-r--r--   0        0        0     3932 2024-04-09 12:18:54.000000 yandex_api_client-0.0.1/yandex_api_client/models/flipping_pager_dto.py
--rw-r--r--   0        0        0     3063 2024-04-09 12:18:54.000000 yandex_api_client-0.0.1/yandex_api_client/models/forward_scrolling_pager_dto.py
--rw-r--r--   0        0        0     3451 2024-04-09 12:18:54.000000 yandex_api_client-0.0.1/yandex_api_client/models/fulfillment_warehouse_dto.py
--rw-r--r--   0        0        0     3499 2024-04-09 12:18:54.000000 yandex_api_client-0.0.1/yandex_api_client/models/fulfillment_warehouses_dto.py
--rw-r--r--   0        0        0     8277 2024-04-09 12:18:54.000000 yandex_api_client-0.0.1/yandex_api_client/models/full_outlet_dto.py
--rw-r--r--   0        0        0     6796 2024-04-09 12:18:54.000000 yandex_api_client-0.0.1/yandex_api_client/models/full_outlet_license_dto.py
--rw-r--r--   0        0        0     3374 2024-04-09 12:18:54.000000 yandex_api_client-0.0.1/yandex_api_client/models/generate_boost_consolidated_request.py
--rw-r--r--   0        0        0     5140 2024-04-09 12:18:54.000000 yandex_api_client-0.0.1/yandex_api_client/models/generate_goods_movement_report_request.py
--rw-r--r--   0        0        0     3427 2024-04-09 12:18:54.000000 yandex_api_client-0.0.1/yandex_api_client/models/generate_goods_realization_report_request.py
--rw-r--r--   0        0        0     3005 2024-04-09 12:18:54.000000 yandex_api_client-0.0.1/yandex_api_client/models/generate_goods_turnover_request.py
--rw-r--r--   0        0        0     4614 2024-04-09 12:18:54.000000 yandex_api_client-0.0.1/yandex_api_client/models/generate_prices_report_request.py
--rw-r--r--   0        0        0     3523 2024-04-09 12:18:54.000000 yandex_api_client-0.0.1/yandex_api_client/models/generate_report_dto.py
--rw-r--r--   0        0        0     3357 2024-04-09 12:18:54.000000 yandex_api_client-0.0.1/yandex_api_client/models/generate_report_response.py
--rw-r--r--   0        0        0     3498 2024-04-09 12:18:54.000000 yandex_api_client-0.0.1/yandex_api_client/models/generate_shipment_list_document_report_request.py
--rw-r--r--   0        0        0     4309 2024-04-09 12:18:54.000000 yandex_api_client-0.0.1/yandex_api_client/models/generate_shows_sales_report_request.py
--rw-r--r--   0        0        0     4324 2024-04-09 12:18:54.000000 yandex_api_client-0.0.1/yandex_api_client/models/generate_stocks_on_warehouses_report_request.py
--rw-r--r--   0        0        0     5458 2024-04-09 12:18:54.000000 yandex_api_client-0.0.1/yandex_api_client/models/generate_united_marketplace_services_report_request.py
--rw-r--r--   0        0        0     4912 2024-04-09 12:18:54.000000 yandex_api_client-0.0.1/yandex_api_client/models/generate_united_netting_report_request.py
--rw-r--r--   0        0        0     3665 2024-04-09 12:18:54.000000 yandex_api_client-0.0.1/yandex_api_client/models/generate_united_orders_request.py
--rw-r--r--   0        0        0     3381 2024-04-09 12:18:54.000000 yandex_api_client-0.0.1/yandex_api_client/models/get_all_offers_response.py
--rw-r--r--   0        0        0     3435 2024-04-09 12:18:54.000000 yandex_api_client-0.0.1/yandex_api_client/models/get_bids_info_request.py
--rw-r--r--   0        0        0     3321 2024-04-09 12:18:54.000000 yandex_api_client-0.0.1/yandex_api_client/models/get_bids_info_response.py
--rw-r--r--   0        0        0     3827 2024-04-09 12:18:54.000000 yandex_api_client-0.0.1/yandex_api_client/models/get_bids_info_response_dto.py
--rw-r--r--   0        0        0     3134 2024-04-09 12:18:54.000000 yandex_api_client-0.0.1/yandex_api_client/models/get_bids_recommendations_request.py
--rw-r--r--   0        0        0     3398 2024-04-09 12:18:54.000000 yandex_api_client-0.0.1/yandex_api_client/models/get_bids_recommendations_response.py
--rw-r--r--   0        0        0     3619 2024-04-09 12:18:54.000000 yandex_api_client-0.0.1/yandex_api_client/models/get_bids_recommendations_response_dto.py
--rw-r--r--   0        0        0     3359 2024-04-09 12:18:54.000000 yandex_api_client-0.0.1/yandex_api_client/models/get_business_buyer_info_response.py
--rw-r--r--   0        0        0     3391 2024-04-09 12:18:54.000000 yandex_api_client-0.0.1/yandex_api_client/models/get_business_documents_info_response.py
--rw-r--r--   0        0        0     3887 2024-04-09 12:18:54.000000 yandex_api_client-0.0.1/yandex_api_client/models/get_campaign_categories_response.py
--rw-r--r--   0        0        0     3005 2024-04-09 12:18:54.000000 yandex_api_client-0.0.1/yandex_api_client/models/get_campaign_logins_response.py
--rw-r--r--   0        0        0     7604 2024-04-09 12:18:54.000000 yandex_api_client-0.0.1/yandex_api_client/models/get_campaign_offer_dto.py
--rw-r--r--   0        0        0     4623 2024-04-09 12:18:54.000000 yandex_api_client-0.0.1/yandex_api_client/models/get_campaign_offers_request.py
--rw-r--r--   0        0        0     3420 2024-04-09 12:18:54.000000 yandex_api_client-0.0.1/yandex_api_client/models/get_campaign_offers_response.py
--rw-r--r--   0        0        0     3872 2024-04-09 12:18:54.000000 yandex_api_client-0.0.1/yandex_api_client/models/get_campaign_offers_result_dto.py
--rw-r--r--   0        0        0     3147 2024-04-09 12:18:54.000000 yandex_api_client-0.0.1/yandex_api_client/models/get_campaign_region_response.py
--rw-r--r--   0        0        0     3171 2024-04-09 12:18:54.000000 yandex_api_client-0.0.1/yandex_api_client/models/get_campaign_response.py
--rw-r--r--   0        0        0     3214 2024-04-09 12:18:54.000000 yandex_api_client-0.0.1/yandex_api_client/models/get_campaign_settings_response.py
--rw-r--r--   0        0        0     3853 2024-04-09 12:18:54.000000 yandex_api_client-0.0.1/yandex_api_client/models/get_campaigns_response.py
--rw-r--r--   0        0        0     3289 2024-04-09 12:18:54.000000 yandex_api_client-0.0.1/yandex_api_client/models/get_categories_response.py
--rw-r--r--   0        0        0     3519 2024-04-09 12:18:54.000000 yandex_api_client-0.0.1/yandex_api_client/models/get_category_content_parameters_response.py
--rw-r--r--   0        0        0     3195 2024-04-09 12:18:54.000000 yandex_api_client-0.0.1/yandex_api_client/models/get_chat_history_request.py
--rw-r--r--   0        0        0     3335 2024-04-09 12:18:54.000000 yandex_api_client-0.0.1/yandex_api_client/models/get_chat_history_response.py
--rw-r--r--   0        0        0     3702 2024-04-09 12:18:54.000000 yandex_api_client-0.0.1/yandex_api_client/models/get_chat_info_dto.py
--rw-r--r--   0        0        0     3764 2024-04-09 12:18:54.000000 yandex_api_client-0.0.1/yandex_api_client/models/get_chats_info_dto.py
--rw-r--r--   0        0        0     3642 2024-04-09 12:18:54.000000 yandex_api_client-0.0.1/yandex_api_client/models/get_chats_request.py
--rw-r--r--   0        0        0     3287 2024-04-09 12:18:54.000000 yandex_api_client-0.0.1/yandex_api_client/models/get_chats_response.py
--rw-r--r--   0        0        0     3203 2024-04-09 12:18:54.000000 yandex_api_client-0.0.1/yandex_api_client/models/get_delivery_services_response.py
--rw-r--r--   0        0        0     3880 2024-04-09 12:18:54.000000 yandex_api_client-0.0.1/yandex_api_client/models/get_feed_categories_response.py
--rw-r--r--   0        0        0     3348 2024-04-09 12:18:54.000000 yandex_api_client-0.0.1/yandex_api_client/models/get_feed_index_logs_response.py
--rw-r--r--   0        0        0     3105 2024-04-09 12:18:54.000000 yandex_api_client-0.0.1/yandex_api_client/models/get_feed_response.py
--rw-r--r--   0        0        0     3314 2024-04-09 12:18:54.000000 yandex_api_client-0.0.1/yandex_api_client/models/get_feedback_list_response.py
--rw-r--r--   0        0        0     3370 2024-04-09 12:18:54.000000 yandex_api_client-0.0.1/yandex_api_client/models/get_feeds_response.py
--rw-r--r--   0        0        0     3386 2024-04-09 12:18:54.000000 yandex_api_client-0.0.1/yandex_api_client/models/get_fulfillment_warehouses_response.py
--rw-r--r--   0        0        0     3296 2024-04-09 12:18:54.000000 yandex_api_client-0.0.1/yandex_api_client/models/get_goods_stats_request.py
--rw-r--r--   0        0        0     3339 2024-04-09 12:18:54.000000 yandex_api_client-0.0.1/yandex_api_client/models/get_goods_stats_response.py
--rw-r--r--   0        0        0     3386 2024-04-09 12:18:54.000000 yandex_api_client-0.0.1/yandex_api_client/models/get_hidden_offers_response.py
--rw-r--r--   0        0        0     3911 2024-04-09 12:18:54.000000 yandex_api_client-0.0.1/yandex_api_client/models/get_hidden_offers_result_dto.py
--rw-r--r--   0        0        0     4863 2024-04-09 12:18:54.000000 yandex_api_client-0.0.1/yandex_api_client/models/get_mapping_dto.py
--rw-r--r--   0        0        0     4196 2024-04-09 12:18:54.000000 yandex_api_client-0.0.1/yandex_api_client/models/get_models_offers_response.py
--rw-r--r--   0        0        0     2931 2024-04-09 12:18:54.000000 yandex_api_client-0.0.1/yandex_api_client/models/get_models_request.py
--rw-r--r--   0        0        0     4126 2024-04-09 12:18:54.000000 yandex_api_client-0.0.1/yandex_api_client/models/get_models_response.py
--rw-r--r--   0        0        0     4215 2024-04-09 12:18:54.000000 yandex_api_client-0.0.1/yandex_api_client/models/get_offer_cards_content_status_request.py
--rw-r--r--   0        0        0     3459 2024-04-09 12:18:54.000000 yandex_api_client-0.0.1/yandex_api_client/models/get_offer_cards_content_status_response.py
--rw-r--r--   0        0        0    24819 2024-04-09 12:18:54.000000 yandex_api_client-0.0.1/yandex_api_client/models/get_offer_dto.py
--rw-r--r--   0        0        0     3501 2024-04-09 12:18:55.000000 yandex_api_client-0.0.1/yandex_api_client/models/get_offer_mapping_dto.py
--rw-r--r--   0        0        0     3418 2024-04-09 12:18:55.000000 yandex_api_client-0.0.1/yandex_api_client/models/get_offer_mapping_entries_response.py
--rw-r--r--   0        0        0     5016 2024-04-09 12:18:55.000000 yandex_api_client-0.0.1/yandex_api_client/models/get_offer_mappings_request.py
--rw-r--r--   0        0        0     3360 2024-04-09 12:18:55.000000 yandex_api_client-0.0.1/yandex_api_client/models/get_offer_mappings_response.py
--rw-r--r--   0        0        0     3923 2024-04-09 12:18:55.000000 yandex_api_client-0.0.1/yandex_api_client/models/get_offer_mappings_result_dto.py
--rw-r--r--   0        0        0     4205 2024-04-09 12:18:55.000000 yandex_api_client-0.0.1/yandex_api_client/models/get_offer_recommendations_request.py
--rw-r--r--   0        0        0     3403 2024-04-09 12:18:55.000000 yandex_api_client-0.0.1/yandex_api_client/models/get_offer_recommendations_response.py
--rw-r--r--   0        0        0     3791 2024-04-09 12:18:55.000000 yandex_api_client-0.0.1/yandex_api_client/models/get_offers_response.py
--rw-r--r--   0        0        0     3331 2024-04-09 12:18:55.000000 yandex_api_client-0.0.1/yandex_api_client/models/get_order_buyer_info_response.py
--rw-r--r--   0        0        0     3364 2024-04-09 12:18:55.000000 yandex_api_client-0.0.1/yandex_api_client/models/get_order_labels_data_response.py
--rw-r--r--   0        0        0     3062 2024-04-09 12:18:55.000000 yandex_api_client-0.0.1/yandex_api_client/models/get_order_response.py
--rw-r--r--   0        0        0     3794 2024-04-09 12:18:55.000000 yandex_api_client-0.0.1/yandex_api_client/models/get_orders_response.py
--rw-r--r--   0        0        0     5466 2024-04-09 12:18:55.000000 yandex_api_client-0.0.1/yandex_api_client/models/get_orders_stats_request.py
--rw-r--r--   0        0        0     3354 2024-04-09 12:18:55.000000 yandex_api_client-0.0.1/yandex_api_client/models/get_orders_stats_response.py
--rw-r--r--   0        0        0     3363 2024-04-09 12:18:55.000000 yandex_api_client-0.0.1/yandex_api_client/models/get_outlet_licenses_response.py
--rw-r--r--   0        0        0     3156 2024-04-09 12:18:55.000000 yandex_api_client-0.0.1/yandex_api_client/models/get_outlet_response.py
--rw-r--r--   0        0        0     4244 2024-04-09 12:18:55.000000 yandex_api_client-0.0.1/yandex_api_client/models/get_outlets_response.py
--rw-r--r--   0        0        0     3410 2024-04-09 12:18:55.000000 yandex_api_client-0.0.1/yandex_api_client/models/get_price_dto.py
--rw-r--r--   0        0        0     4044 2024-04-09 12:18:55.000000 yandex_api_client-0.0.1/yandex_api_client/models/get_price_with_discount_dto.py
--rw-r--r--   0        0        0     4422 2024-04-09 12:18:55.000000 yandex_api_client-0.0.1/yandex_api_client/models/get_price_with_vat_dto.py
--rw-r--r--   0        0        0     3058 2024-04-09 12:18:55.000000 yandex_api_client-0.0.1/yandex_api_client/models/get_prices_by_offer_ids_request.py
--rw-r--r--   0        0        0     3437 2024-04-09 12:18:55.000000 yandex_api_client-0.0.1/yandex_api_client/models/get_prices_by_offer_ids_response.py
--rw-r--r--   0        0        0     3364 2024-04-09 12:18:55.000000 yandex_api_client-0.0.1/yandex_api_client/models/get_prices_response.py
--rw-r--r--   0        0        0     4778 2024-04-09 12:18:55.000000 yandex_api_client-0.0.1/yandex_api_client/models/get_quarantine_offers_request.py
--rw-r--r--   0        0        0     3436 2024-04-09 12:18:55.000000 yandex_api_client-0.0.1/yandex_api_client/models/get_quarantine_offers_response.py
--rw-r--r--   0        0        0     3880 2024-04-09 12:18:55.000000 yandex_api_client-0.0.1/yandex_api_client/models/get_quarantine_offers_result_dto.py
--rw-r--r--   0        0        0     3529 2024-04-09 12:18:55.000000 yandex_api_client-0.0.1/yandex_api_client/models/get_region_with_children_response.py
--rw-r--r--   0        0        0     3782 2024-04-09 12:18:55.000000 yandex_api_client-0.0.1/yandex_api_client/models/get_regions_response.py
--rw-r--r--   0        0        0     3345 2024-04-09 12:18:55.000000 yandex_api_client-0.0.1/yandex_api_client/models/get_report_info_response.py
--rw-r--r--   0        0        0     3265 2024-04-09 12:18:55.000000 yandex_api_client-0.0.1/yandex_api_client/models/get_return_response.py
--rw-r--r--   0        0        0     3294 2024-04-09 12:18:55.000000 yandex_api_client-0.0.1/yandex_api_client/models/get_returns_response.py
--rw-r--r--   0        0        0     3363 2024-04-09 12:18:55.000000 yandex_api_client-0.0.1/yandex_api_client/models/get_shipment_orders_info_response.py
--rw-r--r--   0        0        0     3281 2024-04-09 12:18:55.000000 yandex_api_client-0.0.1/yandex_api_client/models/get_shipment_response.py
--rw-r--r--   0        0        0     3535 2024-04-09 12:18:55.000000 yandex_api_client-0.0.1/yandex_api_client/models/get_suggested_offer_mapping_entries_request.py
--rw-r--r--   0        0        0     3493 2024-04-09 12:18:55.000000 yandex_api_client-0.0.1/yandex_api_client/models/get_suggested_offer_mapping_entries_response.py
--rw-r--r--   0        0        0     3425 2024-04-09 12:18:55.000000 yandex_api_client-0.0.1/yandex_api_client/models/get_suggested_offer_mappings_request.py
--rw-r--r--   0        0        0     3433 2024-04-09 12:18:55.000000 yandex_api_client-0.0.1/yandex_api_client/models/get_suggested_offer_mappings_response.py
--rw-r--r--   0        0        0     3488 2024-04-09 12:18:55.000000 yandex_api_client-0.0.1/yandex_api_client/models/get_suggested_offer_mappings_result_dto.py
--rw-r--r--   0        0        0     3929 2024-04-09 12:18:55.000000 yandex_api_client-0.0.1/yandex_api_client/models/get_warehouse_stocks_dto.py
--rw-r--r--   0        0        0     4589 2024-04-09 12:18:55.000000 yandex_api_client-0.0.1/yandex_api_client/models/get_warehouse_stocks_request.py
--rw-r--r--   0        0        0     3351 2024-04-09 12:18:55.000000 yandex_api_client-0.0.1/yandex_api_client/models/get_warehouse_stocks_response.py
--rw-r--r--   0        0        0     3297 2024-04-09 12:18:55.000000 yandex_api_client-0.0.1/yandex_api_client/models/get_warehouses_response.py
--rw-r--r--   0        0        0     3412 2024-04-09 12:18:55.000000 yandex_api_client-0.0.1/yandex_api_client/models/goods_stats_dto.py
--rw-r--r--   0        0        0     8466 2024-04-09 12:18:55.000000 yandex_api_client-0.0.1/yandex_api_client/models/goods_stats_goods_dto.py
--rw-r--r--   0        0        0     3758 2024-04-09 12:18:55.000000 yandex_api_client-0.0.1/yandex_api_client/models/goods_stats_warehouse_dto.py
--rw-r--r--   0        0        0     3844 2024-04-09 12:18:55.000000 yandex_api_client-0.0.1/yandex_api_client/models/goods_stats_weight_dimensions_dto.py
--rw-r--r--   0        0        0     3043 2024-04-09 12:18:55.000000 yandex_api_client-0.0.1/yandex_api_client/models/gps_dto.py
--rw-r--r--   0        0        0     4495 2024-04-09 12:18:55.000000 yandex_api_client-0.0.1/yandex_api_client/models/hidden_offer_dto.py
--rw-r--r--   0        0        0     1552 2024-04-09 12:18:55.000000 yandex_api_client-0.0.1/yandex_api_client/models/license_check_status_type.py
--rw-r--r--   0        0        0     1347 2024-04-09 12:18:55.000000 yandex_api_client-0.0.1/yandex_api_client/models/license_type.py
--rw-r--r--   0        0        0     4262 2024-04-09 12:18:55.000000 yandex_api_client-0.0.1/yandex_api_client/models/logistic_pickup_point_dto.py
--rw-r--r--   0        0        0     1847 2024-04-09 12:18:55.000000 yandex_api_client-0.0.1/yandex_api_client/models/logistic_point_type.py
--rw-r--r--   0        0        0    22333 2024-04-09 12:18:55.000000 yandex_api_client-0.0.1/yandex_api_client/models/mappings_offer_dto.py
--rw-r--r--   0        0        0    22165 2024-04-09 12:18:55.000000 yandex_api_client-0.0.1/yandex_api_client/models/mappings_offer_info_dto.py
--rw-r--r--   0        0        0     3441 2024-04-09 12:18:55.000000 yandex_api_client-0.0.1/yandex_api_client/models/model_dto.py
--rw-r--r--   0        0        0     6237 2024-04-09 12:18:55.000000 yandex_api_client-0.0.1/yandex_api_client/models/model_offer_dto.py
--rw-r--r--   0        0        0     3461 2024-04-09 12:18:55.000000 yandex_api_client-0.0.1/yandex_api_client/models/model_price_dto.py
--rw-r--r--   0        0        0     1988 2024-04-09 12:18:55.000000 yandex_api_client-0.0.1/yandex_api_client/models/offer_availability_status_type.py
--rw-r--r--   0        0        0     3132 2024-04-09 12:18:55.000000 yandex_api_client-0.0.1/yandex_api_client/models/offer_campaign_status_dto.py
--rw-r--r--   0        0        0     2061 2024-04-09 12:18:55.000000 yandex_api_client-0.0.1/yandex_api_client/models/offer_campaign_status_type.py
--rw-r--r--   0        0        0     8069 2024-04-09 12:18:55.000000 yandex_api_client-0.0.1/yandex_api_client/models/offer_card_dto.py
--rw-r--r--   0        0        0     3354 2024-04-09 12:18:55.000000 yandex_api_client-0.0.1/yandex_api_client/models/offer_card_recommendation_dto.py
--rw-r--r--   0        0        0     4454 2024-04-09 12:18:55.000000 yandex_api_client-0.0.1/yandex_api_client/models/offer_card_recommendation_type.py
--rw-r--r--   0        0        0     2484 2024-04-09 12:18:55.000000 yandex_api_client-0.0.1/yandex_api_client/models/offer_card_status_type.py
--rw-r--r--   0        0        0     4025 2024-04-09 12:18:55.000000 yandex_api_client-0.0.1/yandex_api_client/models/offer_cards_content_status_dto.py
--rw-r--r--   0        0        0     3421 2024-04-09 12:18:55.000000 yandex_api_client-0.0.1/yandex_api_client/models/offer_condition_dto.py
--rw-r--r--   0        0        0     1472 2024-04-09 12:18:55.000000 yandex_api_client-0.0.1/yandex_api_client/models/offer_condition_quality_type.py
--rw-r--r--   0        0        0     2153 2024-04-09 12:18:55.000000 yandex_api_client-0.0.1/yandex_api_client/models/offer_condition_type.py
--rw-r--r--   0        0        0     5806 2024-04-09 12:18:55.000000 yandex_api_client-0.0.1/yandex_api_client/models/offer_content_dto.py
--rw-r--r--   0        0        0     3349 2024-04-09 12:18:55.000000 yandex_api_client-0.0.1/yandex_api_client/models/offer_content_error_dto.py
--rw-r--r--   0        0        0     2424 2024-04-09 12:18:55.000000 yandex_api_client-0.0.1/yandex_api_client/models/offer_content_error_type.py
--rw-r--r--   0        0        0     8257 2024-04-09 12:18:55.000000 yandex_api_client-0.0.1/yandex_api_client/models/offer_dto.py
--rw-r--r--   0        0        0     3100 2024-04-09 12:18:55.000000 yandex_api_client-0.0.1/yandex_api_client/models/offer_error_dto.py
--rw-r--r--   0        0        0     5887 2024-04-09 12:18:55.000000 yandex_api_client-0.0.1/yandex_api_client/models/offer_for_recommendation_dto.py
--rw-r--r--   0        0        0     3152 2024-04-09 12:18:55.000000 yandex_api_client-0.0.1/yandex_api_client/models/offer_manual_dto.py
--rw-r--r--   0        0        0     3746 2024-04-09 12:18:55.000000 yandex_api_client-0.0.1/yandex_api_client/models/offer_mapping_dto.py
--rw-r--r--   0        0        0     4026 2024-04-09 12:18:55.000000 yandex_api_client-0.0.1/yandex_api_client/models/offer_mapping_entries_dto.py
--rw-r--r--   0        0        0     4562 2024-04-09 12:18:55.000000 yandex_api_client-0.0.1/yandex_api_client/models/offer_mapping_entry_dto.py
--rw-r--r--   0        0        0     4191 2024-04-09 12:18:55.000000 yandex_api_client-0.0.1/yandex_api_client/models/offer_mapping_info_dto.py
--rw-r--r--   0        0        0     1239 2024-04-09 12:18:55.000000 yandex_api_client-0.0.1/yandex_api_client/models/offer_mapping_kind_type.py
--rw-r--r--   0        0        0     3490 2024-04-09 12:18:55.000000 yandex_api_client-0.0.1/yandex_api_client/models/offer_mapping_suggestions_list_dto.py
--rw-r--r--   0        0        0     3696 2024-04-09 12:18:55.000000 yandex_api_client-0.0.1/yandex_api_client/models/offer_param_dto.py
--rw-r--r--   0        0        0     3897 2024-04-09 12:18:55.000000 yandex_api_client-0.0.1/yandex_api_client/models/offer_price_by_offer_ids_list_response_dto.py
--rw-r--r--   0        0        0     5184 2024-04-09 12:18:55.000000 yandex_api_client-0.0.1/yandex_api_client/models/offer_price_by_offer_ids_response_dto.py
--rw-r--r--   0        0        0     7514 2024-04-09 12:18:55.000000 yandex_api_client-0.0.1/yandex_api_client/models/offer_price_dto.py
--rw-r--r--   0        0        0     3019 2024-04-09 12:18:55.000000 yandex_api_client-0.0.1/yandex_api_client/models/offer_price_feed_dto.py
--rw-r--r--   0        0        0     4054 2024-04-09 12:18:55.000000 yandex_api_client-0.0.1/yandex_api_client/models/offer_price_list_response_dto.py
--rw-r--r--   0        0        0     4207 2024-04-09 12:18:55.000000 yandex_api_client-0.0.1/yandex_api_client/models/offer_price_response_dto.py
--rw-r--r--   0        0        0     3238 2024-04-09 12:18:55.000000 yandex_api_client-0.0.1/yandex_api_client/models/offer_processing_note_dto.py
--rw-r--r--   0        0        0     6259 2024-04-09 12:18:55.000000 yandex_api_client-0.0.1/yandex_api_client/models/offer_processing_note_type.py
--rw-r--r--   0        0        0     3725 2024-04-09 12:18:55.000000 yandex_api_client-0.0.1/yandex_api_client/models/offer_processing_state_dto.py
--rw-r--r--   0        0        0     2806 2024-04-09 12:18:55.000000 yandex_api_client-0.0.1/yandex_api_client/models/offer_processing_status_type.py
--rw-r--r--   0        0        0     3728 2024-04-09 12:18:55.000000 yandex_api_client-0.0.1/yandex_api_client/models/offer_recommendation_dto.py
--rw-r--r--   0        0        0     5872 2024-04-09 12:18:55.000000 yandex_api_client-0.0.1/yandex_api_client/models/offer_recommendation_info_dto.py
--rw-r--r--   0        0        0     4047 2024-04-09 12:18:55.000000 yandex_api_client-0.0.1/yandex_api_client/models/offer_recommendations_result_dto.py
--rw-r--r--   0        0        0     3276 2024-04-09 12:18:55.000000 yandex_api_client-0.0.1/yandex_api_client/models/offer_selling_program_dto.py
--rw-r--r--   0        0        0     1386 2024-04-09 12:18:55.000000 yandex_api_client-0.0.1/yandex_api_client/models/offer_selling_program_status_type.py
--rw-r--r--   0        0        0     1900 2024-04-09 12:18:55.000000 yandex_api_client-0.0.1/yandex_api_client/models/offer_type.py
--rw-r--r--   0        0        0     3749 2024-04-09 12:18:55.000000 yandex_api_client-0.0.1/yandex_api_client/models/offer_weight_dimensions_dto.py
--rw-r--r--   0        0        0     3371 2024-04-09 12:18:55.000000 yandex_api_client-0.0.1/yandex_api_client/models/offers_dto.py
--rw-r--r--   0        0        0     3499 2024-04-09 12:18:55.000000 yandex_api_client-0.0.1/yandex_api_client/models/option_values_limited_dto.py
--rw-r--r--   0        0        0     3602 2024-04-09 12:18:55.000000 yandex_api_client-0.0.1/yandex_api_client/models/order_box_layout_dto.py
--rw-r--r--   0        0        0     5090 2024-04-09 12:18:55.000000 yandex_api_client-0.0.1/yandex_api_client/models/order_box_layout_item_dto.py
--rw-r--r--   0        0        0     3219 2024-04-09 12:18:55.000000 yandex_api_client-0.0.1/yandex_api_client/models/order_box_layout_partial_count_dto.py
--rw-r--r--   0        0        0     3409 2024-04-09 12:18:55.000000 yandex_api_client-0.0.1/yandex_api_client/models/order_boxes_layout_dto.py
--rw-r--r--   0        0        0     3517 2024-04-09 12:18:55.000000 yandex_api_client-0.0.1/yandex_api_client/models/order_business_buyer_dto.py
--rw-r--r--   0        0        0     4401 2024-04-09 12:18:55.000000 yandex_api_client-0.0.1/yandex_api_client/models/order_business_documents_dto.py
--rw-r--r--   0        0        0     3690 2024-04-09 12:18:55.000000 yandex_api_client-0.0.1/yandex_api_client/models/order_buyer_basic_info_dto.py
--rw-r--r--   0        0        0     3792 2024-04-09 12:18:55.000000 yandex_api_client-0.0.1/yandex_api_client/models/order_buyer_dto.py
--rw-r--r--   0        0        0     4155 2024-04-09 12:18:55.000000 yandex_api_client-0.0.1/yandex_api_client/models/order_buyer_info_dto.py
--rw-r--r--   0        0        0     1330 2024-04-09 12:18:55.000000 yandex_api_client-0.0.1/yandex_api_client/models/order_buyer_type.py
--rw-r--r--   0        0        0     1504 2024-04-09 12:18:55.000000 yandex_api_client-0.0.1/yandex_api_client/models/order_cancellation_reason_type.py
--rw-r--r--   0        0        0     3830 2024-04-09 12:18:55.000000 yandex_api_client-0.0.1/yandex_api_client/models/order_courier_dto.py
--rw-r--r--   0        0        0     5760 2024-04-09 12:18:55.000000 yandex_api_client-0.0.1/yandex_api_client/models/order_delivery_address_dto.py
--rw-r--r--   0        0        0     3020 2024-04-09 12:18:55.000000 yandex_api_client-0.0.1/yandex_api_client/models/order_delivery_date_dto.py
--rw-r--r--   0        0        0     1971 2024-04-09 12:18:55.000000 yandex_api_client-0.0.1/yandex_api_client/models/order_delivery_date_reason_type.py
--rw-r--r--   0        0        0     4466 2024-04-09 12:18:55.000000 yandex_api_client-0.0.1/yandex_api_client/models/order_delivery_dates_dto.py
--rw-r--r--   0        0        0     1945 2024-04-09 12:18:55.000000 yandex_api_client-0.0.1/yandex_api_client/models/order_delivery_dispatch_type.py
--rw-r--r--   0        0        0     9811 2024-04-09 12:18:55.000000 yandex_api_client-0.0.1/yandex_api_client/models/order_delivery_dto.py
--rw-r--r--   0        0        0     1648 2024-04-09 12:18:55.000000 yandex_api_client-0.0.1/yandex_api_client/models/order_delivery_eac_type.py
--rw-r--r--   0        0        0     1676 2024-04-09 12:18:55.000000 yandex_api_client-0.0.1/yandex_api_client/models/order_delivery_partner_type.py
--rw-r--r--   0        0        0     1506 2024-04-09 12:18:55.000000 yandex_api_client-0.0.1/yandex_api_client/models/order_delivery_type.py
--rw-r--r--   0        0        0     3824 2024-04-09 12:18:55.000000 yandex_api_client-0.0.1/yandex_api_client/models/order_digital_item_dto.py
--rw-r--r--   0        0        0     1326 2024-04-09 12:18:55.000000 yandex_api_client-0.0.1/yandex_api_client/models/order_document_status_type.py
--rw-r--r--   0        0        0    12140 2024-04-09 12:18:55.000000 yandex_api_client-0.0.1/yandex_api_client/models/order_dto.py
--rw-r--r--   0        0        0     3423 2024-04-09 12:18:55.000000 yandex_api_client-0.0.1/yandex_api_client/models/order_item_detail_dto.py
--rw-r--r--   0        0        0    13849 2024-04-09 12:18:55.000000 yandex_api_client-0.0.1/yandex_api_client/models/order_item_dto.py
--rw-r--r--   0        0        0     5232 2024-04-09 12:18:55.000000 yandex_api_client-0.0.1/yandex_api_client/models/order_item_instance_dto.py
--rw-r--r--   0        0        0     3960 2024-04-09 12:18:55.000000 yandex_api_client-0.0.1/yandex_api_client/models/order_item_instance_modification_dto.py
--rw-r--r--   0        0        0     1286 2024-04-09 12:18:55.000000 yandex_api_client-0.0.1/yandex_api_client/models/order_item_instance_type.py
--rw-r--r--   0        0        0     4709 2024-04-09 12:18:55.000000 yandex_api_client-0.0.1/yandex_api_client/models/order_item_modification_dto.py
--rw-r--r--   0        0        0     4438 2024-04-09 12:18:55.000000 yandex_api_client-0.0.1/yandex_api_client/models/order_item_promo_dto.py
--rw-r--r--   0        0        0     1297 2024-04-09 12:18:55.000000 yandex_api_client-0.0.1/yandex_api_client/models/order_item_status_type.py
--rw-r--r--   0        0        0     3470 2024-04-09 12:18:55.000000 yandex_api_client-0.0.1/yandex_api_client/models/order_item_subsidy_dto.py
--rw-r--r--   0        0        0     1389 2024-04-09 12:18:55.000000 yandex_api_client-0.0.1/yandex_api_client/models/order_items_modification_request_reason_type.py
--rw-r--r--   0        0        0     3580 2024-04-09 12:18:55.000000 yandex_api_client-0.0.1/yandex_api_client/models/order_items_modification_result_dto.py
--rw-r--r--   0        0        0     4239 2024-04-09 12:18:55.000000 yandex_api_client-0.0.1/yandex_api_client/models/order_label_dto.py
--rw-r--r--   0        0        0     1664 2024-04-09 12:18:55.000000 yandex_api_client-0.0.1/yandex_api_client/models/order_lift_type.py
--rw-r--r--   0        0        0     3225 2024-04-09 12:18:55.000000 yandex_api_client-0.0.1/yandex_api_client/models/order_parcel_box_dto.py
--rw-r--r--   0        0        0     1381 2024-04-09 12:18:55.000000 yandex_api_client-0.0.1/yandex_api_client/models/order_parcel_status_type.py
--rw-r--r--   0        0        0     3028 2024-04-09 12:18:55.000000 yandex_api_client-0.0.1/yandex_api_client/models/order_payment_method_type.py
--rw-r--r--   0        0        0     1535 2024-04-09 12:18:55.000000 yandex_api_client-0.0.1/yandex_api_client/models/order_payment_type.py
--rw-r--r--   0        0        0     3359 2024-04-09 12:18:55.000000 yandex_api_client-0.0.1/yandex_api_client/models/order_promo_type.py
--rw-r--r--   0        0        0     5487 2024-04-09 12:18:55.000000 yandex_api_client-0.0.1/yandex_api_client/models/order_shipment_dto.py
--rw-r--r--   0        0        0     3213 2024-04-09 12:18:55.000000 yandex_api_client-0.0.1/yandex_api_client/models/order_state_dto.py
--rw-r--r--   0        0        0     2823 2024-04-09 12:18:55.000000 yandex_api_client-0.0.1/yandex_api_client/models/order_stats_status_type.py
--rw-r--r--   0        0        0     3064 2024-04-09 12:18:55.000000 yandex_api_client-0.0.1/yandex_api_client/models/order_status_change_delivery_dates_dto.py
--rw-r--r--   0        0        0     3227 2024-04-09 12:18:55.000000 yandex_api_client-0.0.1/yandex_api_client/models/order_status_change_delivery_dto.py
--rw-r--r--   0        0        0     3517 2024-04-09 12:18:55.000000 yandex_api_client-0.0.1/yandex_api_client/models/order_status_change_dto.py
--rw-r--r--   0        0        0     2147 2024-04-09 12:18:55.000000 yandex_api_client-0.0.1/yandex_api_client/models/order_status_type.py
--rw-r--r--   0        0        0     1952 2024-04-09 12:18:55.000000 yandex_api_client-0.0.1/yandex_api_client/models/order_subsidy_type.py
--rw-r--r--   0        0        0     9431 2024-04-09 12:18:55.000000 yandex_api_client-0.0.1/yandex_api_client/models/order_substatus_type.py
--rw-r--r--   0        0        0     2234 2024-04-09 12:18:55.000000 yandex_api_client-0.0.1/yandex_api_client/models/order_tax_system_type.py
--rw-r--r--   0        0        0     3421 2024-04-09 12:18:55.000000 yandex_api_client-0.0.1/yandex_api_client/models/order_track_dto.py
--rw-r--r--   0        0        0     1471 2024-04-09 12:18:55.000000 yandex_api_client-0.0.1/yandex_api_client/models/order_update_status_type.py
--rw-r--r--   0        0        0     2494 2024-04-09 12:18:55.000000 yandex_api_client-0.0.1/yandex_api_client/models/order_vat_type.py
--rw-r--r--   0        0        0     3461 2024-04-09 12:18:55.000000 yandex_api_client-0.0.1/yandex_api_client/models/orders_shipment_info_dto.py
--rw-r--r--   0        0        0     3385 2024-04-09 12:18:55.000000 yandex_api_client-0.0.1/yandex_api_client/models/orders_stats_commission_dto.py
--rw-r--r--   0        0        0     2748 2024-04-09 12:18:55.000000 yandex_api_client-0.0.1/yandex_api_client/models/orders_stats_commission_type.py
--rw-r--r--   0        0        0     3153 2024-04-09 12:18:55.000000 yandex_api_client-0.0.1/yandex_api_client/models/orders_stats_delivery_region_dto.py
--rw-r--r--   0        0        0     3898 2024-04-09 12:18:55.000000 yandex_api_client-0.0.1/yandex_api_client/models/orders_stats_details_dto.py
--rw-r--r--   0        0        0     3824 2024-04-09 12:18:55.000000 yandex_api_client-0.0.1/yandex_api_client/models/orders_stats_dto.py
--rw-r--r--   0        0        0     9813 2024-04-09 12:18:55.000000 yandex_api_client-0.0.1/yandex_api_client/models/orders_stats_item_dto.py
--rw-r--r--   0        0        0     1430 2024-04-09 12:18:55.000000 yandex_api_client-0.0.1/yandex_api_client/models/orders_stats_item_status_type.py
--rw-r--r--   0        0        0     8086 2024-04-09 12:18:55.000000 yandex_api_client-0.0.1/yandex_api_client/models/orders_stats_order_dto.py
--rw-r--r--   0        0        0     1576 2024-04-09 12:18:55.000000 yandex_api_client-0.0.1/yandex_api_client/models/orders_stats_order_payment_type.py
--rw-r--r--   0        0        0     4571 2024-04-09 12:18:55.000000 yandex_api_client-0.0.1/yandex_api_client/models/orders_stats_payment_dto.py
--rw-r--r--   0        0        0     3222 2024-04-09 12:18:55.000000 yandex_api_client-0.0.1/yandex_api_client/models/orders_stats_payment_order_dto.py
--rw-r--r--   0        0        0     1748 2024-04-09 12:18:55.000000 yandex_api_client-0.0.1/yandex_api_client/models/orders_stats_payment_source_type.py
--rw-r--r--   0        0        0     1356 2024-04-09 12:18:55.000000 yandex_api_client-0.0.1/yandex_api_client/models/orders_stats_payment_type.py
--rw-r--r--   0        0        0     3674 2024-04-09 12:18:55.000000 yandex_api_client-0.0.1/yandex_api_client/models/orders_stats_price_dto.py
--rw-r--r--   0        0        0     1565 2024-04-09 12:18:55.000000 yandex_api_client-0.0.1/yandex_api_client/models/orders_stats_price_type.py
--rw-r--r--   0        0        0     1488 2024-04-09 12:18:55.000000 yandex_api_client-0.0.1/yandex_api_client/models/orders_stats_stock_type.py
--rw-r--r--   0        0        0     3130 2024-04-09 12:18:55.000000 yandex_api_client-0.0.1/yandex_api_client/models/orders_stats_warehouse_dto.py
--rw-r--r--   0        0        0     5461 2024-04-09 12:18:55.000000 yandex_api_client-0.0.1/yandex_api_client/models/outlet_address_dto.py
--rw-r--r--   0        0        0     8909 2024-04-09 12:18:55.000000 yandex_api_client-0.0.1/yandex_api_client/models/outlet_delivery_rule_dto.py
--rw-r--r--   0        0        0     6846 2024-04-09 12:18:55.000000 yandex_api_client-0.0.1/yandex_api_client/models/outlet_dto.py
--rw-r--r--   0        0        0     6149 2024-04-09 12:18:55.000000 yandex_api_client-0.0.1/yandex_api_client/models/outlet_license_dto.py
--rw-r--r--   0        0        0     3508 2024-04-09 12:18:55.000000 yandex_api_client-0.0.1/yandex_api_client/models/outlet_licenses_response_dto.py
--rw-r--r--   0        0        0     3039 2024-04-09 12:18:55.000000 yandex_api_client-0.0.1/yandex_api_client/models/outlet_response_dto.py
--rw-r--r--   0        0        0     1672 2024-04-09 12:18:55.000000 yandex_api_client-0.0.1/yandex_api_client/models/outlet_status_type.py
--rw-r--r--   0        0        0     1592 2024-04-09 12:18:55.000000 yandex_api_client-0.0.1/yandex_api_client/models/outlet_type.py
--rw-r--r--   0        0        0     1445 2024-04-09 12:18:55.000000 yandex_api_client-0.0.1/yandex_api_client/models/outlet_visibility_type.py
--rw-r--r--   0        0        0     4252 2024-04-09 12:18:55.000000 yandex_api_client-0.0.1/yandex_api_client/models/outlet_working_schedule_dto.py
--rw-r--r--   0        0        0     3650 2024-04-09 12:18:55.000000 yandex_api_client-0.0.1/yandex_api_client/models/outlet_working_schedule_item_dto.py
--rw-r--r--   0        0        0     1758 2024-04-09 12:18:55.000000 yandex_api_client-0.0.1/yandex_api_client/models/page_format_type.py
--rw-r--r--   0        0        0     3774 2024-04-09 12:18:55.000000 yandex_api_client-0.0.1/yandex_api_client/models/paged_returns_dto.py
--rw-r--r--   0        0        0     3195 2024-04-09 12:18:55.000000 yandex_api_client-0.0.1/yandex_api_client/models/pallets_count_dto.py
--rw-r--r--   0        0        0     1424 2024-04-09 12:18:55.000000 yandex_api_client-0.0.1/yandex_api_client/models/parameter_type.py
--rw-r--r--   0        0        0     3460 2024-04-09 12:18:55.000000 yandex_api_client-0.0.1/yandex_api_client/models/parameter_value_constraints_dto.py
--rw-r--r--   0        0        0     4632 2024-04-09 12:18:55.000000 yandex_api_client-0.0.1/yandex_api_client/models/parameter_value_dto.py
--rw-r--r--   0        0        0     3212 2024-04-09 12:18:55.000000 yandex_api_client-0.0.1/yandex_api_client/models/parameter_value_option_dto.py
--rw-r--r--   0        0        0     4104 2024-04-09 12:18:55.000000 yandex_api_client-0.0.1/yandex_api_client/models/parcel_box_dto.py
--rw-r--r--   0        0        0     6283 2024-04-09 12:18:55.000000 yandex_api_client-0.0.1/yandex_api_client/models/parcel_box_label_dto.py
--rw-r--r--   0        0        0     3519 2024-04-09 12:18:55.000000 yandex_api_client-0.0.1/yandex_api_client/models/parcel_dto.py
--rw-r--r--   0        0        0     3334 2024-04-09 12:18:55.000000 yandex_api_client-0.0.1/yandex_api_client/models/partner_shipment_warehouse_dto.py
--rw-r--r--   0        0        0     1644 2024-04-09 12:18:55.000000 yandex_api_client-0.0.1/yandex_api_client/models/payment_frequency_type.py
--rw-r--r--   0        0        0     3442 2024-04-09 12:18:55.000000 yandex_api_client-0.0.1/yandex_api_client/models/pickup_address_dto.py
--rw-r--r--   0        0        0     1354 2024-04-09 12:18:55.000000 yandex_api_client-0.0.1/yandex_api_client/models/placement_type.py
--rw-r--r--   0        0        0     3816 2024-04-09 12:18:55.000000 yandex_api_client-0.0.1/yandex_api_client/models/price_competitiveness_thresholds_dto.py
--rw-r--r--   0        0        0     1427 2024-04-09 12:18:55.000000 yandex_api_client-0.0.1/yandex_api_client/models/price_competitiveness_type.py
--rw-r--r--   0        0        0     4189 2024-04-09 12:18:55.000000 yandex_api_client-0.0.1/yandex_api_client/models/price_dto.py
--rw-r--r--   0        0        0     3900 2024-04-09 12:18:55.000000 yandex_api_client-0.0.1/yandex_api_client/models/price_quarantine_verdict_dto.py
--rw-r--r--   0        0        0     1871 2024-04-09 12:18:55.000000 yandex_api_client-0.0.1/yandex_api_client/models/price_quarantine_verdict_param_name_type.py
--rw-r--r--   0        0        0     3138 2024-04-09 12:18:55.000000 yandex_api_client-0.0.1/yandex_api_client/models/price_quarantine_verdict_parameter_dto.py
--rw-r--r--   0        0        0     2195 2024-04-09 12:18:55.000000 yandex_api_client-0.0.1/yandex_api_client/models/price_quarantine_verdict_type.py
--rw-r--r--   0        0        0     3525 2024-04-09 12:18:55.000000 yandex_api_client-0.0.1/yandex_api_client/models/price_recommendation_item_dto.py
--rw-r--r--   0        0        0     3081 2024-04-09 12:18:55.000000 yandex_api_client-0.0.1/yandex_api_client/models/price_suggest_dto.py
--rw-r--r--   0        0        0     5465 2024-04-09 12:18:55.000000 yandex_api_client-0.0.1/yandex_api_client/models/price_suggest_offer_dto.py
--rw-r--r--   0        0        0     4268 2024-04-09 12:18:55.000000 yandex_api_client-0.0.1/yandex_api_client/models/price_suggest_type.py
--rw-r--r--   0        0        0     3828 2024-04-09 12:18:55.000000 yandex_api_client-0.0.1/yandex_api_client/models/provide_order_digital_codes_request.py
--rw-r--r--   0        0        0     3494 2024-04-09 12:18:55.000000 yandex_api_client-0.0.1/yandex_api_client/models/provide_order_item_identifiers_request.py
--rw-r--r--   0        0        0     3428 2024-04-09 12:18:55.000000 yandex_api_client-0.0.1/yandex_api_client/models/provide_order_item_identifiers_response.py
--rw-r--r--   0        0        0     3488 2024-04-09 12:18:55.000000 yandex_api_client-0.0.1/yandex_api_client/models/put_sku_bids_request.py
--rw-r--r--   0        0        0     4219 2024-04-09 12:18:55.000000 yandex_api_client-0.0.1/yandex_api_client/models/quantum_dto.py
--rw-r--r--   0        0        0     6144 2024-04-09 12:18:55.000000 yandex_api_client-0.0.1/yandex_api_client/models/quarantine_offer_dto.py
--rw-r--r--   0        0        0     1460 2024-04-09 12:18:55.000000 yandex_api_client-0.0.1/yandex_api_client/models/recipient_type.py
--rw-r--r--   0        0        0     2391 2024-04-09 12:18:55.000000 yandex_api_client-0.0.1/yandex_api_client/models/refund_status_type.py
--rw-r--r--   0        0        0     4100 2024-04-09 12:18:55.000000 yandex_api_client-0.0.1/yandex_api_client/models/region_dto.py
--rw-r--r--   0        0        0     2019 2024-04-09 12:18:55.000000 yandex_api_client-0.0.1/yandex_api_client/models/region_type.py
--rw-r--r--   0        0        0     3503 2024-04-09 12:18:55.000000 yandex_api_client-0.0.1/yandex_api_client/models/regional_model_info_dto.py
--rw-r--r--   0        0        0     1387 2024-04-09 12:18:55.000000 yandex_api_client-0.0.1/yandex_api_client/models/report_format_type.py
--rw-r--r--   0        0        0     4220 2024-04-09 12:18:55.000000 yandex_api_client-0.0.1/yandex_api_client/models/report_info_dto.py
--rw-r--r--   0        0        0     1547 2024-04-09 12:18:55.000000 yandex_api_client-0.0.1/yandex_api_client/models/report_status_type.py
--rw-r--r--   0        0        0     1546 2024-04-09 12:18:55.000000 yandex_api_client-0.0.1/yandex_api_client/models/report_sub_status_type.py
--rw-r--r--   0        0        0     4753 2024-04-09 12:18:55.000000 yandex_api_client-0.0.1/yandex_api_client/models/return_decision_dto.py
--rw-r--r--   0        0        0     2000 2024-04-09 12:18:55.000000 yandex_api_client-0.0.1/yandex_api_client/models/return_decision_reason_type.py
--rw-r--r--   0        0        0     2530 2024-04-09 12:18:55.000000 yandex_api_client-0.0.1/yandex_api_client/models/return_decision_subreason_type.py
--rw-r--r--   0        0        0     1989 2024-04-09 12:18:55.000000 yandex_api_client-0.0.1/yandex_api_client/models/return_decision_type.py
--rw-r--r--   0        0        0     5892 2024-04-09 12:18:55.000000 yandex_api_client-0.0.1/yandex_api_client/models/return_dto.py
--rw-r--r--   0        0        0     3620 2024-04-09 12:18:55.000000 yandex_api_client-0.0.1/yandex_api_client/models/return_instance_dto.py
--rw-r--r--   0        0        0     1661 2024-04-09 12:18:55.000000 yandex_api_client-0.0.1/yandex_api_client/models/return_instance_status_type.py
--rw-r--r--   0        0        0     1653 2024-04-09 12:18:55.000000 yandex_api_client-0.0.1/yandex_api_client/models/return_instance_stock_type.py
--rw-r--r--   0        0        0     6784 2024-04-09 12:18:55.000000 yandex_api_client-0.0.1/yandex_api_client/models/return_item_dto.py
--rw-r--r--   0        0        0     1500 2024-04-09 12:18:55.000000 yandex_api_client-0.0.1/yandex_api_client/models/return_request_decision_type.py
--rw-r--r--   0        0        0     2399 2024-04-09 12:18:55.000000 yandex_api_client-0.0.1/yandex_api_client/models/return_shipment_status_type.py
--rw-r--r--   0        0        0     1430 2024-04-09 12:18:55.000000 yandex_api_client-0.0.1/yandex_api_client/models/return_type.py
--rw-r--r--   0        0        0     3315 2024-04-09 12:18:55.000000 yandex_api_client-0.0.1/yandex_api_client/models/scrolling_pager_dto.py
--rw-r--r--   0        0        0     4480 2024-04-09 12:18:55.000000 yandex_api_client-0.0.1/yandex_api_client/models/search_models_response.py
--rw-r--r--   0        0        0     3924 2024-04-09 12:18:55.000000 yandex_api_client-0.0.1/yandex_api_client/models/search_shipments_request.py
--rw-r--r--   0        0        0     3410 2024-04-09 12:18:55.000000 yandex_api_client-0.0.1/yandex_api_client/models/search_shipments_response.py
--rw-r--r--   0        0        0     3909 2024-04-09 12:18:55.000000 yandex_api_client-0.0.1/yandex_api_client/models/search_shipments_response_dto.py
--rw-r--r--   0        0        0     1366 2024-04-09 12:18:55.000000 yandex_api_client-0.0.1/yandex_api_client/models/selling_program_type.py
--rw-r--r--   0        0        0     3118 2024-04-09 12:18:55.000000 yandex_api_client-0.0.1/yandex_api_client/models/send_message_to_chat_request.py
--rw-r--r--   0        0        0     3514 2024-04-09 12:18:55.000000 yandex_api_client-0.0.1/yandex_api_client/models/set_feed_params_request.py
--rw-r--r--   0        0        0     3782 2024-04-09 12:18:55.000000 yandex_api_client-0.0.1/yandex_api_client/models/set_order_box_layout_request.py
--rw-r--r--   0        0        0     3339 2024-04-09 12:18:55.000000 yandex_api_client-0.0.1/yandex_api_client/models/set_order_box_layout_response.py
--rw-r--r--   0        0        0     3317 2024-04-09 12:18:55.000000 yandex_api_client-0.0.1/yandex_api_client/models/set_order_delivery_date_request.py
--rw-r--r--   0        0        0     3385 2024-04-09 12:18:55.000000 yandex_api_client-0.0.1/yandex_api_client/models/set_order_delivery_track_code_request.py
--rw-r--r--   0        0        0     3534 2024-04-09 12:18:55.000000 yandex_api_client-0.0.1/yandex_api_client/models/set_order_shipment_boxes_request.py
--rw-r--r--   0        0        0     3342 2024-04-09 12:18:55.000000 yandex_api_client-0.0.1/yandex_api_client/models/set_order_shipment_boxes_response.py
--rw-r--r--   0        0        0     3812 2024-04-09 12:18:55.000000 yandex_api_client-0.0.1/yandex_api_client/models/set_return_decision_request.py
--rw-r--r--   0        0        0     3106 2024-04-09 12:18:55.000000 yandex_api_client-0.0.1/yandex_api_client/models/set_shipment_pallets_count_request.py
--rw-r--r--   0        0        0     1829 2024-04-09 12:18:55.000000 yandex_api_client-0.0.1/yandex_api_client/models/shipment_action_type.py
--rw-r--r--   0        0        0     3614 2024-04-09 12:18:55.000000 yandex_api_client-0.0.1/yandex_api_client/models/shipment_boxes_dto.py
--rw-r--r--   0        0        0     6683 2024-04-09 12:18:55.000000 yandex_api_client-0.0.1/yandex_api_client/models/shipment_dto.py
--rw-r--r--   0        0        0     5781 2024-04-09 12:18:55.000000 yandex_api_client-0.0.1/yandex_api_client/models/shipment_info_dto.py
--rw-r--r--   0        0        0     1352 2024-04-09 12:18:55.000000 yandex_api_client-0.0.1/yandex_api_client/models/shipment_pallet_label_page_format_type.py
--rw-r--r--   0        0        0     3410 2024-04-09 12:18:55.000000 yandex_api_client-0.0.1/yandex_api_client/models/shipment_status_change_dto.py
--rw-r--r--   0        0        0     2153 2024-04-09 12:18:55.000000 yandex_api_client-0.0.1/yandex_api_client/models/shipment_status_type.py
--rw-r--r--   0        0        0     1577 2024-04-09 12:18:55.000000 yandex_api_client-0.0.1/yandex_api_client/models/shipment_type.py
--rw-r--r--   0        0        0     1448 2024-04-09 12:18:55.000000 yandex_api_client-0.0.1/yandex_api_client/models/shows_sales_grouping_type.py
--rw-r--r--   0        0        0     4534 2024-04-09 12:18:55.000000 yandex_api_client-0.0.1/yandex_api_client/models/sku_bid_item_dto.py
--rw-r--r--   0        0        0     6469 2024-04-09 12:18:55.000000 yandex_api_client-0.0.1/yandex_api_client/models/sku_bid_recommendation_item_dto.py
--rw-r--r--   0        0        0     1399 2024-04-09 12:18:55.000000 yandex_api_client-0.0.1/yandex_api_client/models/sort_order_type.py
--rw-r--r--   0        0        0     4773 2024-04-09 12:18:55.000000 yandex_api_client-0.0.1/yandex_api_client/models/suggest_offer_price_dto.py
--rw-r--r--   0        0        0     3498 2024-04-09 12:18:55.000000 yandex_api_client-0.0.1/yandex_api_client/models/suggest_prices_request.py
--rw-r--r--   0        0        0     3393 2024-04-09 12:18:55.000000 yandex_api_client-0.0.1/yandex_api_client/models/suggest_prices_response.py
--rw-r--r--   0        0        0     3493 2024-04-09 12:18:55.000000 yandex_api_client-0.0.1/yandex_api_client/models/suggest_prices_result_dto.py
--rw-r--r--   0        0        0     9763 2024-04-09 12:18:55.000000 yandex_api_client-0.0.1/yandex_api_client/models/suggested_offer_dto.py
--rw-r--r--   0        0        0     3590 2024-04-09 12:18:55.000000 yandex_api_client-0.0.1/yandex_api_client/models/suggested_offer_mapping_dto.py
--rw-r--r--   0        0        0     4188 2024-04-09 12:18:55.000000 yandex_api_client-0.0.1/yandex_api_client/models/tariff_dto.py
--rw-r--r--   0        0        0     3051 2024-04-09 12:18:55.000000 yandex_api_client-0.0.1/yandex_api_client/models/tariff_parameter_dto.py
--rw-r--r--   0        0        0     4820 2024-04-09 12:18:55.000000 yandex_api_client-0.0.1/yandex_api_client/models/tariff_type.py
--rw-r--r--   0        0        0     3561 2024-04-09 12:18:55.000000 yandex_api_client-0.0.1/yandex_api_client/models/time_period_dto.py
--rw-r--r--   0        0        0     1421 2024-04-09 12:18:55.000000 yandex_api_client-0.0.1/yandex_api_client/models/time_unit_type.py
--rw-r--r--   0        0        0     2959 2024-04-09 12:18:55.000000 yandex_api_client-0.0.1/yandex_api_client/models/track_dto.py
--rw-r--r--   0        0        0     3146 2024-04-09 12:18:55.000000 yandex_api_client-0.0.1/yandex_api_client/models/transfer_orders_from_shipment_request.py
--rw-r--r--   0        0        0     3260 2024-04-09 12:18:55.000000 yandex_api_client-0.0.1/yandex_api_client/models/turnover_dto.py
--rw-r--r--   0        0        0     1770 2024-04-09 12:18:55.000000 yandex_api_client-0.0.1/yandex_api_client/models/turnover_type.py
--rw-r--r--   0        0        0     3225 2024-04-09 12:18:55.000000 yandex_api_client-0.0.1/yandex_api_client/models/unit_dto.py
--rw-r--r--   0        0        0     4863 2024-04-09 12:18:55.000000 yandex_api_client-0.0.1/yandex_api_client/models/update_business_offer_price_dto.py
--rw-r--r--   0        0        0     3571 2024-04-09 12:18:55.000000 yandex_api_client-0.0.1/yandex_api_client/models/update_business_prices_request.py
--rw-r--r--   0        0        0     5520 2024-04-09 12:18:55.000000 yandex_api_client-0.0.1/yandex_api_client/models/update_campaign_offer_dto.py
--rw-r--r--   0        0        0     3611 2024-04-09 12:18:55.000000 yandex_api_client-0.0.1/yandex_api_client/models/update_campaign_offers_request.py
--rw-r--r--   0        0        0     3423 2024-04-09 12:18:55.000000 yandex_api_client-0.0.1/yandex_api_client/models/update_mapping_dto.py
--rw-r--r--   0        0        0    22156 2024-04-09 12:18:55.000000 yandex_api_client-0.0.1/yandex_api_client/models/update_mappings_offer_dto.py
--rw-r--r--   0        0        0     3658 2024-04-09 12:18:55.000000 yandex_api_client-0.0.1/yandex_api_client/models/update_offer_content_request.py
--rw-r--r--   0        0        0     3978 2024-04-09 12:18:55.000000 yandex_api_client-0.0.1/yandex_api_client/models/update_offer_content_response.py
--rw-r--r--   0        0        0     5928 2024-04-09 12:18:55.000000 yandex_api_client-0.0.1/yandex_api_client/models/update_offer_content_result_dto.py
--rw-r--r--   0        0        0    22344 2024-04-09 12:18:55.000000 yandex_api_client-0.0.1/yandex_api_client/models/update_offer_dto.py
--rw-r--r--   0        0        0     3517 2024-04-09 12:18:55.000000 yandex_api_client-0.0.1/yandex_api_client/models/update_offer_mapping_dto.py
--rw-r--r--   0        0        0     4748 2024-04-09 12:18:55.000000 yandex_api_client-0.0.1/yandex_api_client/models/update_offer_mapping_entry_dto.py
--rw-r--r--   0        0        0     3718 2024-04-09 12:18:55.000000 yandex_api_client-0.0.1/yandex_api_client/models/update_offer_mapping_entry_request.py
--rw-r--r--   0        0        0     3634 2024-04-09 12:18:55.000000 yandex_api_client-0.0.1/yandex_api_client/models/update_offer_mappings_request.py
--rw-r--r--   0        0        0     3893 2024-04-09 12:18:55.000000 yandex_api_client-0.0.1/yandex_api_client/models/update_order_item_request.py
--rw-r--r--   0        0        0     3963 2024-04-09 12:18:55.000000 yandex_api_client-0.0.1/yandex_api_client/models/update_order_status_dto.py
--rw-r--r--   0        0        0     3117 2024-04-09 12:18:55.000000 yandex_api_client-0.0.1/yandex_api_client/models/update_order_status_request.py
--rw-r--r--   0        0        0     3146 2024-04-09 12:18:55.000000 yandex_api_client-0.0.1/yandex_api_client/models/update_order_status_response.py
--rw-r--r--   0        0        0     3482 2024-04-09 12:18:55.000000 yandex_api_client-0.0.1/yandex_api_client/models/update_order_statuses_dto.py
--rw-r--r--   0        0        0     3440 2024-04-09 12:18:55.000000 yandex_api_client-0.0.1/yandex_api_client/models/update_order_statuses_request.py
--rw-r--r--   0        0        0     3359 2024-04-09 12:18:55.000000 yandex_api_client-0.0.1/yandex_api_client/models/update_order_statuses_response.py
--rw-r--r--   0        0        0     3233 2024-04-09 12:18:55.000000 yandex_api_client-0.0.1/yandex_api_client/models/update_order_storage_limit_request.py
--rw-r--r--   0        0        0     3683 2024-04-09 12:18:55.000000 yandex_api_client-0.0.1/yandex_api_client/models/update_outlet_license_request.py
--rw-r--r--   0        0        0     3783 2024-04-09 12:18:55.000000 yandex_api_client-0.0.1/yandex_api_client/models/update_price_with_discount_dto.py
--rw-r--r--   0        0        0     3441 2024-04-09 12:18:55.000000 yandex_api_client-0.0.1/yandex_api_client/models/update_prices_request.py
--rw-r--r--   0        0        0     5110 2024-04-09 12:18:55.000000 yandex_api_client-0.0.1/yandex_api_client/models/update_stock_dto.py
--rw-r--r--   0        0        0     3588 2024-04-09 12:18:55.000000 yandex_api_client-0.0.1/yandex_api_client/models/update_stock_item_dto.py
--rw-r--r--   0        0        0     3497 2024-04-09 12:18:55.000000 yandex_api_client-0.0.1/yandex_api_client/models/update_stocks_request.py
--rw-r--r--   0        0        0     2957 2024-04-09 12:18:55.000000 yandex_api_client-0.0.1/yandex_api_client/models/update_time_dto.py
--rw-r--r--   0        0        0     4744 2024-04-09 12:18:55.000000 yandex_api_client-0.0.1/yandex_api_client/models/value_restriction_dto.py
--rw-r--r--   0        0        0     2923 2024-04-09 12:18:55.000000 yandex_api_client-0.0.1/yandex_api_client/models/verify_order_eac_request.py
--rw-r--r--   0        0        0     3347 2024-04-09 12:18:55.000000 yandex_api_client-0.0.1/yandex_api_client/models/verify_order_eac_response.py
--rw-r--r--   0        0        0     3979 2024-04-09 12:18:55.000000 yandex_api_client-0.0.1/yandex_api_client/models/warehouse_address_dto.py
--rw-r--r--   0        0        0     3843 2024-04-09 12:18:55.000000 yandex_api_client-0.0.1/yandex_api_client/models/warehouse_dto.py
--rw-r--r--   0        0        0     3962 2024-04-09 12:18:55.000000 yandex_api_client-0.0.1/yandex_api_client/models/warehouse_group_dto.py
--rw-r--r--   0        0        0     6040 2024-04-09 12:18:55.000000 yandex_api_client-0.0.1/yandex_api_client/models/warehouse_offer_dto.py
--rw-r--r--   0        0        0     3598 2024-04-09 12:18:55.000000 yandex_api_client-0.0.1/yandex_api_client/models/warehouse_offers_dto.py
--rw-r--r--   0        0        0     3051 2024-04-09 12:18:55.000000 yandex_api_client-0.0.1/yandex_api_client/models/warehouse_stock_dto.py
--rw-r--r--   0        0        0     2523 2024-04-09 12:18:55.000000 yandex_api_client-0.0.1/yandex_api_client/models/warehouse_stock_type.py
--rw-r--r--   0        0        0     4215 2024-04-09 12:18:55.000000 yandex_api_client-0.0.1/yandex_api_client/models/warehouses_dto.py
--rw-r--r--   0        0        0        0 2024-04-09 12:18:56.000000 yandex_api_client-0.0.1/yandex_api_client/py.typed
--rw-r--r--   0        0        0    10188 2024-04-09 12:18:56.000000 yandex_api_client-0.0.1/yandex_api_client/rest.py
--rw-r--r--   0        0        0   125216 1970-01-01 00:00:00.000000 yandex_api_client-0.0.1/PKG-INFO
+-rw-r--r--   0        0        0   124349 2024-04-09 12:18:56.000000 yandex_api_client-0.0.2/README.md
+-rw-r--r--   0        0        0      737 2024-05-13 13:19:03.308409 yandex_api_client-0.0.2/pyproject.toml
+-rw-r--r--   0        0        0    45454 2024-04-09 12:18:56.000000 yandex_api_client-0.0.2/yandex_api_client/__init__.py
+-rw-r--r--   0        0        0     2213 2024-04-09 12:18:56.000000 yandex_api_client-0.0.2/yandex_api_client/api/__init__.py
+-rw-r--r--   0        0        0    90394 2024-04-09 12:18:56.000000 yandex_api_client-0.0.2/yandex_api_client/api/bids_api.py
+-rw-r--r--   0        0        0   112390 2024-04-09 12:18:56.000000 yandex_api_client-0.0.2/yandex_api_client/api/business_offer_mappings_api.py
+-rw-r--r--   0        0        0    90231 2024-04-09 12:18:56.000000 yandex_api_client-0.0.2/yandex_api_client/api/campaigns_api.py
+-rw-r--r--   0        0        0    11904 2024-04-09 12:18:56.000000 yandex_api_client-0.0.2/yandex_api_client/api/categories_api.py
+-rw-r--r--   0        0        0    87315 2024-04-09 12:18:56.000000 yandex_api_client-0.0.2/yandex_api_client/api/chats_api.py
+-rw-r--r--   0        0        0    55369 2024-04-09 12:18:56.000000 yandex_api_client-0.0.2/yandex_api_client/api/content_api.py
+-rw-r--r--   0        0        0  2022454 2024-04-09 12:18:56.000000 yandex_api_client-0.0.2/yandex_api_client/api/dbs_api.py
+-rw-r--r--   0        0        0    12196 2024-04-09 12:18:56.000000 yandex_api_client-0.0.2/yandex_api_client/api/delivery_services_api.py
+-rw-r--r--   0        0        0  1401649 2024-04-09 12:18:56.000000 yandex_api_client-0.0.2/yandex_api_client/api/express_api.py
+-rw-r--r--   0        0        0  1788698 2024-04-09 12:18:56.000000 yandex_api_client-0.0.2/yandex_api_client/api/fbs_api.py
+-rw-r--r--   0        0        0  1189525 2024-04-09 12:18:56.000000 yandex_api_client-0.0.2/yandex_api_client/api/fby_api.py
+-rw-r--r--   0        0        0    49736 2024-04-09 12:18:56.000000 yandex_api_client-0.0.2/yandex_api_client/api/feed_categories_api.py
+-rw-r--r--   0        0        0    24266 2024-04-09 12:18:56.000000 yandex_api_client-0.0.2/yandex_api_client/api/feedbacks_api.py
+-rw-r--r--   0        0        0   103931 2024-04-09 12:18:56.000000 yandex_api_client-0.0.2/yandex_api_client/api/feeds_api.py
+-rw-r--r--   0        0        0    19823 2024-04-09 12:18:56.000000 yandex_api_client-0.0.2/yandex_api_client/api/goods_stats_api.py
+-rw-r--r--   0        0        0    63690 2024-04-09 12:18:56.000000 yandex_api_client-0.0.2/yandex_api_client/api/hidden_offers_api.py
+-rw-r--r--   0        0        0   129885 2024-04-09 12:18:56.000000 yandex_api_client-0.0.2/yandex_api_client/api/models_api.py
+-rw-r--r--   0        0        0   113854 2024-04-09 12:18:56.000000 yandex_api_client-0.0.2/yandex_api_client/api/offer_mappings_api.py
+-rw-r--r--   0        0        0   141946 2024-04-09 12:18:56.000000 yandex_api_client-0.0.2/yandex_api_client/api/offers_api.py
+-rw-r--r--   0        0        0    33987 2024-04-09 12:18:56.000000 yandex_api_client-0.0.2/yandex_api_client/api/order_business_information_api.py
+-rw-r--r--   0        0        0    94574 2024-04-09 12:18:56.000000 yandex_api_client-0.0.2/yandex_api_client/api/order_delivery_api.py
+-rw-r--r--   0        0        0    54373 2024-04-09 12:18:56.000000 yandex_api_client-0.0.2/yandex_api_client/api/order_labels_api.py
+-rw-r--r--   0        0        0   300755 2024-04-09 12:18:56.000000 yandex_api_client-0.0.2/yandex_api_client/api/orders_api.py
+-rw-r--r--   0        0        0    24751 2024-04-09 12:18:56.000000 yandex_api_client-0.0.2/yandex_api_client/api/orders_stats_api.py
+-rw-r--r--   0        0        0    57754 2024-04-09 12:18:56.000000 yandex_api_client-0.0.2/yandex_api_client/api/outlet_licenses_api.py
+-rw-r--r--   0        0        0    95593 2024-04-09 12:18:56.000000 yandex_api_client-0.0.2/yandex_api_client/api/outlets_api.py
+-rw-r--r--   0        0        0    84650 2024-04-09 12:18:56.000000 yandex_api_client-0.0.2/yandex_api_client/api/price_quarantine_api.py
+-rw-r--r--   0        0        0   100684 2024-04-09 12:18:56.000000 yandex_api_client-0.0.2/yandex_api_client/api/prices_api.py
+-rw-r--r--   0        0        0    54645 2024-04-09 12:18:56.000000 yandex_api_client-0.0.2/yandex_api_client/api/regions_api.py
+-rw-r--r--   0        0        0   172650 2024-04-09 12:18:56.000000 yandex_api_client-0.0.2/yandex_api_client/api/reports_api.py
+-rw-r--r--   0        0        0   120073 2024-04-09 12:18:56.000000 yandex_api_client-0.0.2/yandex_api_client/api/returns_api.py
+-rw-r--r--   0        0        0   227303 2024-04-09 12:18:56.000000 yandex_api_client-0.0.2/yandex_api_client/api/shipments_api.py
+-rw-r--r--   0        0        0    41006 2024-04-09 12:18:56.000000 yandex_api_client-0.0.2/yandex_api_client/api/stocks_api.py
+-rw-r--r--   0        0        0    15857 2024-04-09 12:18:56.000000 yandex_api_client-0.0.2/yandex_api_client/api/tariffs_api.py
+-rw-r--r--   0        0        0    27100 2024-04-09 12:18:56.000000 yandex_api_client-0.0.2/yandex_api_client/api/warehouses_api.py
+-rw-r--r--   0        0        0    25001 2024-04-09 12:18:56.000000 yandex_api_client-0.0.2/yandex_api_client/api_client.py
+-rw-r--r--   0        0        0      674 2024-04-09 12:18:56.000000 yandex_api_client-0.0.2/yandex_api_client/api_response.py
+-rw-r--r--   0        0        0    15057 2024-04-09 12:18:56.000000 yandex_api_client-0.0.2/yandex_api_client/configuration.py
+-rw-r--r--   0        0        0     6343 2024-04-09 12:18:56.000000 yandex_api_client-0.0.2/yandex_api_client/exceptions.py
+-rw-r--r--   0        0        0    42718 2024-04-09 12:18:56.000000 yandex_api_client-0.0.2/yandex_api_client/models/__init__.py
+-rw-r--r--   0        0        0     3519 2024-04-09 12:18:54.000000 yandex_api_client-0.0.2/yandex_api_client/models/accept_order_cancellation_request.py
+-rw-r--r--   0        0        0     3547 2024-04-09 12:18:54.000000 yandex_api_client-0.0.2/yandex_api_client/models/add_hidden_offers_request.py
+-rw-r--r--   0        0        0     3684 2024-04-09 12:18:54.000000 yandex_api_client-0.0.2/yandex_api_client/models/add_offers_to_archive_dto.py
+-rw-r--r--   0        0        0     4671 2024-04-09 12:18:54.000000 yandex_api_client-0.0.2/yandex_api_client/models/add_offers_to_archive_error_dto.py
+-rw-r--r--   0        0        0     1446 2024-04-09 12:18:54.000000 yandex_api_client-0.0.2/yandex_api_client/models/add_offers_to_archive_error_type.py
+-rw-r--r--   0        0        0     3181 2024-04-09 12:18:54.000000 yandex_api_client-0.0.2/yandex_api_client/models/add_offers_to_archive_request.py
+-rw-r--r--   0        0        0     3379 2024-04-09 12:18:54.000000 yandex_api_client-0.0.2/yandex_api_client/models/add_offers_to_archive_response.py
+-rw-r--r--   0        0        0     3152 2024-04-09 12:18:54.000000 yandex_api_client-0.0.2/yandex_api_client/models/age_dto.py
+-rw-r--r--   0        0        0     1297 2024-04-09 12:18:54.000000 yandex_api_client-0.0.2/yandex_api_client/models/age_unit_type.py
+-rw-r--r--   0        0        0     3605 2024-04-09 12:18:54.000000 yandex_api_client-0.0.2/yandex_api_client/models/api_client_data_error_response.py
+-rw-r--r--   0        0        0     3010 2024-04-09 12:18:54.000000 yandex_api_client-0.0.2/yandex_api_client/models/api_error_dto.py
+-rw-r--r--   0        0        0     3578 2024-04-09 12:18:54.000000 yandex_api_client-0.0.2/yandex_api_client/models/api_error_response.py
+-rw-r--r--   0        0        0     3714 2024-04-09 12:18:54.000000 yandex_api_client-0.0.2/yandex_api_client/models/api_forbidden_error_response.py
+-rw-r--r--   0        0        0     3598 2024-04-09 12:18:54.000000 yandex_api_client-0.0.2/yandex_api_client/models/api_limit_error_response.py
+-rw-r--r--   0        0        0     3653 2024-04-09 12:18:54.000000 yandex_api_client-0.0.2/yandex_api_client/models/api_locked_error_response.py
+-rw-r--r--   0        0        0     3587 2024-04-09 12:18:54.000000 yandex_api_client-0.0.2/yandex_api_client/models/api_not_found_error_response.py
+-rw-r--r--   0        0        0     2932 2024-04-09 12:18:54.000000 yandex_api_client-0.0.2/yandex_api_client/models/api_response.py
+-rw-r--r--   0        0        0     1233 2024-04-09 12:18:54.000000 yandex_api_client-0.0.2/yandex_api_client/models/api_response_status_type.py
+-rw-r--r--   0        0        0     3572 2024-04-09 12:18:54.000000 yandex_api_client-0.0.2/yandex_api_client/models/api_server_error_response.py
+-rw-r--r--   0        0        0     3623 2024-04-09 12:18:54.000000 yandex_api_client-0.0.2/yandex_api_client/models/api_unauthorized_error_response.py
+-rw-r--r--   0        0        0     5034 2024-04-09 12:18:54.000000 yandex_api_client-0.0.2/yandex_api_client/models/base_campaign_offer_dto.py
+-rw-r--r--   0        0        0    20952 2024-04-09 12:18:54.000000 yandex_api_client-0.0.2/yandex_api_client/models/base_offer_dto.py
+-rw-r--r--   0        0        0     3140 2024-04-09 12:18:54.000000 yandex_api_client-0.0.2/yandex_api_client/models/base_price_dto.py
+-rw-r--r--   0        0        0     3215 2024-04-09 12:18:54.000000 yandex_api_client-0.0.2/yandex_api_client/models/bid_recommendation_item_dto.py
+-rw-r--r--   0        0        0     6779 2024-04-09 12:18:54.000000 yandex_api_client-0.0.2/yandex_api_client/models/brief_order_item_dto.py
+-rw-r--r--   0        0        0     5192 2024-04-09 12:18:54.000000 yandex_api_client-0.0.2/yandex_api_client/models/brief_order_item_instance_dto.py
+-rw-r--r--   0        0        0     3055 2024-04-09 12:18:54.000000 yandex_api_client-0.0.2/yandex_api_client/models/business_dto.py
+-rw-r--r--   0        0        0     4748 2024-04-09 12:18:54.000000 yandex_api_client-0.0.2/yandex_api_client/models/calculate_tariffs_offer_dto.py
+-rw-r--r--   0        0        0     4370 2024-04-09 12:18:54.000000 yandex_api_client-0.0.2/yandex_api_client/models/calculate_tariffs_offer_info_dto.py
+-rw-r--r--   0        0        0     4036 2024-04-09 12:18:54.000000 yandex_api_client-0.0.2/yandex_api_client/models/calculate_tariffs_parameters_dto.py
+-rw-r--r--   0        0        0     4016 2024-04-09 12:18:54.000000 yandex_api_client-0.0.2/yandex_api_client/models/calculate_tariffs_request.py
+-rw-r--r--   0        0        0     3367 2024-04-09 12:18:54.000000 yandex_api_client-0.0.2/yandex_api_client/models/calculate_tariffs_response.py
+-rw-r--r--   0        0        0     3435 2024-04-09 12:18:54.000000 yandex_api_client-0.0.2/yandex_api_client/models/calculate_tariffs_response_dto.py
+-rw-r--r--   0        0        0     3863 2024-04-09 12:18:54.000000 yandex_api_client-0.0.2/yandex_api_client/models/calculated_tariff_dto.py
+-rw-r--r--   0        0        0     2302 2024-04-09 12:18:54.000000 yandex_api_client-0.0.2/yandex_api_client/models/calculated_tariff_type.py
+-rw-r--r--   0        0        0     3907 2024-04-09 12:18:54.000000 yandex_api_client-0.0.2/yandex_api_client/models/campaign_dto.py
+-rw-r--r--   0        0        0     3271 2024-04-09 12:18:54.000000 yandex_api_client-0.0.2/yandex_api_client/models/campaign_settings_delivery_dto.py
+-rw-r--r--   0        0        0     5631 2024-04-09 12:18:54.000000 yandex_api_client-0.0.2/yandex_api_client/models/campaign_settings_dto.py
+-rw-r--r--   0        0        0     4078 2024-04-09 12:18:54.000000 yandex_api_client-0.0.2/yandex_api_client/models/campaign_settings_local_region_dto.py
+-rw-r--r--   0        0        0     5568 2024-04-09 12:18:54.000000 yandex_api_client-0.0.2/yandex_api_client/models/campaign_settings_schedule_dto.py
+-rw-r--r--   0        0        0     1630 2024-04-09 12:18:54.000000 yandex_api_client-0.0.2/yandex_api_client/models/campaign_settings_schedule_source_type.py
+-rw-r--r--   0        0        0     3290 2024-04-09 12:18:54.000000 yandex_api_client-0.0.2/yandex_api_client/models/campaign_settings_time_period_dto.py
+-rw-r--r--   0        0        0     3955 2024-04-09 12:18:54.000000 yandex_api_client-0.0.2/yandex_api_client/models/category_content_parameters_dto.py
+-rw-r--r--   0        0        0     3769 2024-04-09 12:18:54.000000 yandex_api_client-0.0.2/yandex_api_client/models/category_dto.py
+-rw-r--r--   0        0        0     7672 2024-04-09 12:18:54.000000 yandex_api_client-0.0.2/yandex_api_client/models/category_parameter_dto.py
+-rw-r--r--   0        0        0     3607 2024-04-09 12:18:54.000000 yandex_api_client-0.0.2/yandex_api_client/models/category_parameter_unit_dto.py
+-rw-r--r--   0        0        0     6847 2024-04-09 12:18:54.000000 yandex_api_client-0.0.2/yandex_api_client/models/change_outlet_request.py
+-rw-r--r--   0        0        0     4556 2024-04-09 12:18:54.000000 yandex_api_client-0.0.2/yandex_api_client/models/chat_message_dto.py
+-rw-r--r--   0        0        0     3195 2024-04-09 12:18:54.000000 yandex_api_client-0.0.2/yandex_api_client/models/chat_message_payload_dto.py
+-rw-r--r--   0        0        0     1503 2024-04-09 12:18:54.000000 yandex_api_client-0.0.2/yandex_api_client/models/chat_message_sender_type.py
+-rw-r--r--   0        0        0     3863 2024-04-09 12:18:54.000000 yandex_api_client-0.0.2/yandex_api_client/models/chat_messages_result_dto.py
+-rw-r--r--   0        0        0     1768 2024-04-09 12:18:54.000000 yandex_api_client-0.0.2/yandex_api_client/models/chat_status_type.py
+-rw-r--r--   0        0        0     1292 2024-04-09 12:18:54.000000 yandex_api_client-0.0.2/yandex_api_client/models/chat_type.py
+-rw-r--r--   0        0        0     3112 2024-04-09 12:18:54.000000 yandex_api_client-0.0.2/yandex_api_client/models/confirm_prices_request.py
+-rw-r--r--   0        0        0     3088 2024-04-09 12:18:54.000000 yandex_api_client-0.0.2/yandex_api_client/models/confirm_shipment_request.py
+-rw-r--r--   0        0        0     2966 2024-04-09 12:18:54.000000 yandex_api_client-0.0.2/yandex_api_client/models/create_chat_request.py
+-rw-r--r--   0        0        0     3338 2024-04-09 12:18:54.000000 yandex_api_client-0.0.2/yandex_api_client/models/create_chat_response.py
+-rw-r--r--   0        0        0     2925 2024-04-09 12:18:54.000000 yandex_api_client-0.0.2/yandex_api_client/models/create_chat_result_dto.py
+-rw-r--r--   0        0        0     3363 2024-04-09 12:18:54.000000 yandex_api_client-0.0.2/yandex_api_client/models/create_outlet_response.py
+-rw-r--r--   0        0        0     3373 2024-04-09 12:18:54.000000 yandex_api_client-0.0.2/yandex_api_client/models/currency_type.py
+-rw-r--r--   0        0        0     1594 2024-04-09 12:18:54.000000 yandex_api_client-0.0.2/yandex_api_client/models/day_of_week_type.py
+-rw-r--r--   0        0        0     3225 2024-04-09 12:18:54.000000 yandex_api_client-0.0.2/yandex_api_client/models/delete_campaign_offers_dto.py
+-rw-r--r--   0        0        0     3159 2024-04-09 12:18:54.000000 yandex_api_client-0.0.2/yandex_api_client/models/delete_campaign_offers_request.py
+-rw-r--r--   0        0        0     3390 2024-04-09 12:18:54.000000 yandex_api_client-0.0.2/yandex_api_client/models/delete_campaign_offers_response.py
+-rw-r--r--   0        0        0     3581 2024-04-09 12:18:54.000000 yandex_api_client-0.0.2/yandex_api_client/models/delete_hidden_offers_request.py
+-rw-r--r--   0        0        0     3267 2024-04-09 12:18:54.000000 yandex_api_client-0.0.2/yandex_api_client/models/delete_offers_dto.py
+-rw-r--r--   0        0        0     3274 2024-04-09 12:18:54.000000 yandex_api_client-0.0.2/yandex_api_client/models/delete_offers_from_archive_dto.py
+-rw-r--r--   0        0        0     3216 2024-04-09 12:18:54.000000 yandex_api_client-0.0.2/yandex_api_client/models/delete_offers_from_archive_request.py
+-rw-r--r--   0        0        0     3420 2024-04-09 12:18:54.000000 yandex_api_client-0.0.2/yandex_api_client/models/delete_offers_from_archive_response.py
+-rw-r--r--   0        0        0     3145 2024-04-09 12:18:54.000000 yandex_api_client-0.0.2/yandex_api_client/models/delete_offers_request.py
+-rw-r--r--   0        0        0     3333 2024-04-09 12:18:54.000000 yandex_api_client-0.0.2/yandex_api_client/models/delete_offers_response.py
+-rw-r--r--   0        0        0     3101 2024-04-09 12:18:54.000000 yandex_api_client-0.0.2/yandex_api_client/models/delivery_service_dto.py
+-rw-r--r--   0        0        0     3079 2024-04-09 12:18:54.000000 yandex_api_client-0.0.2/yandex_api_client/models/delivery_service_info_dto.py
+-rw-r--r--   0        0        0     3567 2024-04-09 12:18:54.000000 yandex_api_client-0.0.2/yandex_api_client/models/delivery_services_dto.py
+-rw-r--r--   0        0        0     3291 2024-04-09 12:18:54.000000 yandex_api_client-0.0.2/yandex_api_client/models/document_dto.py
+-rw-r--r--   0        0        0     3538 2024-04-09 12:18:54.000000 yandex_api_client-0.0.2/yandex_api_client/models/eac_verification_result_dto.py
+-rw-r--r--   0        0        0     1622 2024-04-09 12:18:54.000000 yandex_api_client-0.0.2/yandex_api_client/models/eac_verification_status_type.py
+-rw-r--r--   0        0        0     2911 2024-04-09 12:18:54.000000 yandex_api_client-0.0.2/yandex_api_client/models/empty_api_response.py
+-rw-r--r--   0        0        0    24444 2024-04-09 12:18:54.000000 yandex_api_client-0.0.2/yandex_api_client/models/enriched_mappings_offer_dto.py
+-rw-r--r--   0        0        0     5279 2024-04-09 12:18:54.000000 yandex_api_client-0.0.2/yandex_api_client/models/enriched_model_dto.py
+-rw-r--r--   0        0        0     3822 2024-04-09 12:18:54.000000 yandex_api_client-0.0.2/yandex_api_client/models/enriched_order_box_layout_dto.py
+-rw-r--r--   0        0        0     3546 2024-04-09 12:18:54.000000 yandex_api_client-0.0.2/yandex_api_client/models/feed_category_dto.py
+-rw-r--r--   0        0        0     4162 2024-04-09 12:18:54.000000 yandex_api_client-0.0.2/yandex_api_client/models/feed_content_dto.py
+-rw-r--r--   0        0        0     3026 2024-04-09 12:18:54.000000 yandex_api_client-0.0.2/yandex_api_client/models/feed_content_error_dto.py
+-rw-r--r--   0        0        0     2144 2024-04-09 12:18:54.000000 yandex_api_client-0.0.2/yandex_api_client/models/feed_content_error_type.py
+-rw-r--r--   0        0        0     3339 2024-04-09 12:18:54.000000 yandex_api_client-0.0.2/yandex_api_client/models/feed_download_dto.py
+-rw-r--r--   0        0        0     3611 2024-04-09 12:18:54.000000 yandex_api_client-0.0.2/yandex_api_client/models/feed_download_error_dto.py
+-rw-r--r--   0        0        0     1897 2024-04-09 12:18:54.000000 yandex_api_client-0.0.2/yandex_api_client/models/feed_download_error_type.py
+-rw-r--r--   0        0        0     6395 2024-04-09 12:18:54.000000 yandex_api_client-0.0.2/yandex_api_client/models/feed_dto.py
+-rw-r--r--   0        0        0     3722 2024-04-09 12:18:54.000000 yandex_api_client-0.0.2/yandex_api_client/models/feed_index_logs_error_dto.py
+-rw-r--r--   0        0        0     2790 2024-04-09 12:18:54.000000 yandex_api_client-0.0.2/yandex_api_client/models/feed_index_logs_error_type.py
+-rw-r--r--   0        0        0     2936 2024-04-09 12:18:54.000000 yandex_api_client-0.0.2/yandex_api_client/models/feed_index_logs_feed_dto.py
+-rw-r--r--   0        0        0     1778 2024-04-09 12:18:54.000000 yandex_api_client-0.0.2/yandex_api_client/models/feed_index_logs_index_type.py
+-rw-r--r--   0        0        0     3365 2024-04-09 12:18:54.000000 yandex_api_client-0.0.2/yandex_api_client/models/feed_index_logs_offers_dto.py
+-rw-r--r--   0        0        0     5508 2024-04-09 12:18:54.000000 yandex_api_client-0.0.2/yandex_api_client/models/feed_index_logs_record_dto.py
+-rw-r--r--   0        0        0     4292 2024-04-09 12:18:54.000000 yandex_api_client-0.0.2/yandex_api_client/models/feed_index_logs_result_dto.py
+-rw-r--r--   0        0        0     1610 2024-04-09 12:18:54.000000 yandex_api_client-0.0.2/yandex_api_client/models/feed_index_logs_status_type.py
+-rw-r--r--   0        0        0     4144 2024-04-09 12:18:54.000000 yandex_api_client-0.0.2/yandex_api_client/models/feed_parameter_dto.py
+-rw-r--r--   0        0        0     3441 2024-04-09 12:18:54.000000 yandex_api_client-0.0.2/yandex_api_client/models/feed_placement_dto.py
+-rw-r--r--   0        0        0     4089 2024-04-09 12:18:54.000000 yandex_api_client-0.0.2/yandex_api_client/models/feed_publication_dto.py
+-rw-r--r--   0        0        0     3688 2024-04-09 12:18:54.000000 yandex_api_client-0.0.2/yandex_api_client/models/feed_publication_full_dto.py
+-rw-r--r--   0        0        0     3967 2024-04-09 12:18:54.000000 yandex_api_client-0.0.2/yandex_api_client/models/feed_publication_price_and_stock_update_dto.py
+-rw-r--r--   0        0        0     1539 2024-04-09 12:18:54.000000 yandex_api_client-0.0.2/yandex_api_client/models/feed_status_type.py
+-rw-r--r--   0        0        0     3403 2024-04-09 12:18:54.000000 yandex_api_client-0.0.2/yandex_api_client/models/feedback_author_dto.py
+-rw-r--r--   0        0        0     3177 2024-04-09 12:18:54.000000 yandex_api_client-0.0.2/yandex_api_client/models/feedback_comment_author_dto.py
+-rw-r--r--   0        0        0     1326 2024-04-09 12:18:54.000000 yandex_api_client-0.0.2/yandex_api_client/models/feedback_comment_author_type.py
+-rw-r--r--   0        0        0     5115 2024-04-09 12:18:54.000000 yandex_api_client-0.0.2/yandex_api_client/models/feedback_comment_dto.py
+-rw-r--r--   0        0        0     1422 2024-04-09 12:18:54.000000 yandex_api_client-0.0.2/yandex_api_client/models/feedback_delivery_type.py
+-rw-r--r--   0        0        0     7363 2024-04-09 12:18:54.000000 yandex_api_client-0.0.2/yandex_api_client/models/feedback_dto.py
+-rw-r--r--   0        0        0     4226 2024-04-09 12:18:54.000000 yandex_api_client-0.0.2/yandex_api_client/models/feedback_factor_dto.py
+-rw-r--r--   0        0        0     4961 2024-04-09 12:18:54.000000 yandex_api_client-0.0.2/yandex_api_client/models/feedback_grades_dto.py
+-rw-r--r--   0        0        0     3966 2024-04-09 12:18:54.000000 yandex_api_client-0.0.2/yandex_api_client/models/feedback_list_dto.py
+-rw-r--r--   0        0        0     3211 2024-04-09 12:18:54.000000 yandex_api_client-0.0.2/yandex_api_client/models/feedback_order_dto.py
+-rw-r--r--   0        0        0     2909 2024-04-09 12:18:54.000000 yandex_api_client-0.0.2/yandex_api_client/models/feedback_shop_dto.py
+-rw-r--r--   0        0        0     1361 2024-04-09 12:18:54.000000 yandex_api_client-0.0.2/yandex_api_client/models/feedback_state_type.py
+-rw-r--r--   0        0        0     1496 2024-04-09 12:18:54.000000 yandex_api_client-0.0.2/yandex_api_client/models/field_state_type.py
+-rw-r--r--   0        0        0     3932 2024-04-09 12:18:54.000000 yandex_api_client-0.0.2/yandex_api_client/models/flipping_pager_dto.py
+-rw-r--r--   0        0        0     3063 2024-04-09 12:18:54.000000 yandex_api_client-0.0.2/yandex_api_client/models/forward_scrolling_pager_dto.py
+-rw-r--r--   0        0        0     3451 2024-04-09 12:18:54.000000 yandex_api_client-0.0.2/yandex_api_client/models/fulfillment_warehouse_dto.py
+-rw-r--r--   0        0        0     3499 2024-04-09 12:18:54.000000 yandex_api_client-0.0.2/yandex_api_client/models/fulfillment_warehouses_dto.py
+-rw-r--r--   0        0        0     8277 2024-04-09 12:18:54.000000 yandex_api_client-0.0.2/yandex_api_client/models/full_outlet_dto.py
+-rw-r--r--   0        0        0     6796 2024-04-09 12:18:54.000000 yandex_api_client-0.0.2/yandex_api_client/models/full_outlet_license_dto.py
+-rw-r--r--   0        0        0     3374 2024-04-09 12:18:54.000000 yandex_api_client-0.0.2/yandex_api_client/models/generate_boost_consolidated_request.py
+-rw-r--r--   0        0        0     5140 2024-04-09 12:18:54.000000 yandex_api_client-0.0.2/yandex_api_client/models/generate_goods_movement_report_request.py
+-rw-r--r--   0        0        0     3427 2024-04-09 12:18:54.000000 yandex_api_client-0.0.2/yandex_api_client/models/generate_goods_realization_report_request.py
+-rw-r--r--   0        0        0     3005 2024-04-09 12:18:54.000000 yandex_api_client-0.0.2/yandex_api_client/models/generate_goods_turnover_request.py
+-rw-r--r--   0        0        0     4614 2024-04-09 12:18:54.000000 yandex_api_client-0.0.2/yandex_api_client/models/generate_prices_report_request.py
+-rw-r--r--   0        0        0     3523 2024-04-09 12:18:54.000000 yandex_api_client-0.0.2/yandex_api_client/models/generate_report_dto.py
+-rw-r--r--   0        0        0     3357 2024-04-09 12:18:54.000000 yandex_api_client-0.0.2/yandex_api_client/models/generate_report_response.py
+-rw-r--r--   0        0        0     3498 2024-04-09 12:18:54.000000 yandex_api_client-0.0.2/yandex_api_client/models/generate_shipment_list_document_report_request.py
+-rw-r--r--   0        0        0     4309 2024-04-09 12:18:54.000000 yandex_api_client-0.0.2/yandex_api_client/models/generate_shows_sales_report_request.py
+-rw-r--r--   0        0        0     4324 2024-04-09 12:18:54.000000 yandex_api_client-0.0.2/yandex_api_client/models/generate_stocks_on_warehouses_report_request.py
+-rw-r--r--   0        0        0     5458 2024-04-09 12:18:54.000000 yandex_api_client-0.0.2/yandex_api_client/models/generate_united_marketplace_services_report_request.py
+-rw-r--r--   0        0        0     4912 2024-04-09 12:18:54.000000 yandex_api_client-0.0.2/yandex_api_client/models/generate_united_netting_report_request.py
+-rw-r--r--   0        0        0     3665 2024-04-09 12:18:54.000000 yandex_api_client-0.0.2/yandex_api_client/models/generate_united_orders_request.py
+-rw-r--r--   0        0        0     3381 2024-04-09 12:18:54.000000 yandex_api_client-0.0.2/yandex_api_client/models/get_all_offers_response.py
+-rw-r--r--   0        0        0     3435 2024-04-09 12:18:54.000000 yandex_api_client-0.0.2/yandex_api_client/models/get_bids_info_request.py
+-rw-r--r--   0        0        0     3321 2024-04-09 12:18:54.000000 yandex_api_client-0.0.2/yandex_api_client/models/get_bids_info_response.py
+-rw-r--r--   0        0        0     3827 2024-04-09 12:18:54.000000 yandex_api_client-0.0.2/yandex_api_client/models/get_bids_info_response_dto.py
+-rw-r--r--   0        0        0     3134 2024-04-09 12:18:54.000000 yandex_api_client-0.0.2/yandex_api_client/models/get_bids_recommendations_request.py
+-rw-r--r--   0        0        0     3398 2024-04-09 12:18:54.000000 yandex_api_client-0.0.2/yandex_api_client/models/get_bids_recommendations_response.py
+-rw-r--r--   0        0        0     3619 2024-04-09 12:18:54.000000 yandex_api_client-0.0.2/yandex_api_client/models/get_bids_recommendations_response_dto.py
+-rw-r--r--   0        0        0     3359 2024-04-09 12:18:54.000000 yandex_api_client-0.0.2/yandex_api_client/models/get_business_buyer_info_response.py
+-rw-r--r--   0        0        0     3391 2024-04-09 12:18:54.000000 yandex_api_client-0.0.2/yandex_api_client/models/get_business_documents_info_response.py
+-rw-r--r--   0        0        0     3887 2024-04-09 12:18:54.000000 yandex_api_client-0.0.2/yandex_api_client/models/get_campaign_categories_response.py
+-rw-r--r--   0        0        0     3005 2024-04-09 12:18:54.000000 yandex_api_client-0.0.2/yandex_api_client/models/get_campaign_logins_response.py
+-rw-r--r--   0        0        0     7604 2024-04-09 12:18:54.000000 yandex_api_client-0.0.2/yandex_api_client/models/get_campaign_offer_dto.py
+-rw-r--r--   0        0        0     4623 2024-04-09 12:18:54.000000 yandex_api_client-0.0.2/yandex_api_client/models/get_campaign_offers_request.py
+-rw-r--r--   0        0        0     3420 2024-04-09 12:18:54.000000 yandex_api_client-0.0.2/yandex_api_client/models/get_campaign_offers_response.py
+-rw-r--r--   0        0        0     3872 2024-04-09 12:18:54.000000 yandex_api_client-0.0.2/yandex_api_client/models/get_campaign_offers_result_dto.py
+-rw-r--r--   0        0        0     3147 2024-04-09 12:18:54.000000 yandex_api_client-0.0.2/yandex_api_client/models/get_campaign_region_response.py
+-rw-r--r--   0        0        0     3171 2024-04-09 12:18:54.000000 yandex_api_client-0.0.2/yandex_api_client/models/get_campaign_response.py
+-rw-r--r--   0        0        0     3214 2024-04-09 12:18:54.000000 yandex_api_client-0.0.2/yandex_api_client/models/get_campaign_settings_response.py
+-rw-r--r--   0        0        0     3853 2024-04-09 12:18:54.000000 yandex_api_client-0.0.2/yandex_api_client/models/get_campaigns_response.py
+-rw-r--r--   0        0        0     3289 2024-04-09 12:18:54.000000 yandex_api_client-0.0.2/yandex_api_client/models/get_categories_response.py
+-rw-r--r--   0        0        0     3519 2024-04-09 12:18:54.000000 yandex_api_client-0.0.2/yandex_api_client/models/get_category_content_parameters_response.py
+-rw-r--r--   0        0        0     3195 2024-04-09 12:18:54.000000 yandex_api_client-0.0.2/yandex_api_client/models/get_chat_history_request.py
+-rw-r--r--   0        0        0     3335 2024-04-09 12:18:54.000000 yandex_api_client-0.0.2/yandex_api_client/models/get_chat_history_response.py
+-rw-r--r--   0        0        0     3702 2024-04-09 12:18:54.000000 yandex_api_client-0.0.2/yandex_api_client/models/get_chat_info_dto.py
+-rw-r--r--   0        0        0     3764 2024-04-09 12:18:54.000000 yandex_api_client-0.0.2/yandex_api_client/models/get_chats_info_dto.py
+-rw-r--r--   0        0        0     3642 2024-04-09 12:18:54.000000 yandex_api_client-0.0.2/yandex_api_client/models/get_chats_request.py
+-rw-r--r--   0        0        0     3287 2024-04-09 12:18:54.000000 yandex_api_client-0.0.2/yandex_api_client/models/get_chats_response.py
+-rw-r--r--   0        0        0     3203 2024-04-09 12:18:54.000000 yandex_api_client-0.0.2/yandex_api_client/models/get_delivery_services_response.py
+-rw-r--r--   0        0        0     3880 2024-04-09 12:18:54.000000 yandex_api_client-0.0.2/yandex_api_client/models/get_feed_categories_response.py
+-rw-r--r--   0        0        0     3348 2024-04-09 12:18:54.000000 yandex_api_client-0.0.2/yandex_api_client/models/get_feed_index_logs_response.py
+-rw-r--r--   0        0        0     3105 2024-04-09 12:18:54.000000 yandex_api_client-0.0.2/yandex_api_client/models/get_feed_response.py
+-rw-r--r--   0        0        0     3314 2024-04-09 12:18:54.000000 yandex_api_client-0.0.2/yandex_api_client/models/get_feedback_list_response.py
+-rw-r--r--   0        0        0     3370 2024-04-09 12:18:54.000000 yandex_api_client-0.0.2/yandex_api_client/models/get_feeds_response.py
+-rw-r--r--   0        0        0     3386 2024-04-09 12:18:54.000000 yandex_api_client-0.0.2/yandex_api_client/models/get_fulfillment_warehouses_response.py
+-rw-r--r--   0        0        0     3296 2024-04-09 12:18:54.000000 yandex_api_client-0.0.2/yandex_api_client/models/get_goods_stats_request.py
+-rw-r--r--   0        0        0     3339 2024-04-09 12:18:54.000000 yandex_api_client-0.0.2/yandex_api_client/models/get_goods_stats_response.py
+-rw-r--r--   0        0        0     3386 2024-04-09 12:18:54.000000 yandex_api_client-0.0.2/yandex_api_client/models/get_hidden_offers_response.py
+-rw-r--r--   0        0        0     3911 2024-04-09 12:18:54.000000 yandex_api_client-0.0.2/yandex_api_client/models/get_hidden_offers_result_dto.py
+-rw-r--r--   0        0        0     4863 2024-04-09 12:18:54.000000 yandex_api_client-0.0.2/yandex_api_client/models/get_mapping_dto.py
+-rw-r--r--   0        0        0     4196 2024-04-09 12:18:54.000000 yandex_api_client-0.0.2/yandex_api_client/models/get_models_offers_response.py
+-rw-r--r--   0        0        0     2931 2024-04-09 12:18:54.000000 yandex_api_client-0.0.2/yandex_api_client/models/get_models_request.py
+-rw-r--r--   0        0        0     4126 2024-04-09 12:18:54.000000 yandex_api_client-0.0.2/yandex_api_client/models/get_models_response.py
+-rw-r--r--   0        0        0     4215 2024-04-09 12:18:54.000000 yandex_api_client-0.0.2/yandex_api_client/models/get_offer_cards_content_status_request.py
+-rw-r--r--   0        0        0     3459 2024-04-09 12:18:54.000000 yandex_api_client-0.0.2/yandex_api_client/models/get_offer_cards_content_status_response.py
+-rw-r--r--   0        0        0    24819 2024-04-09 12:18:54.000000 yandex_api_client-0.0.2/yandex_api_client/models/get_offer_dto.py
+-rw-r--r--   0        0        0     3501 2024-04-09 12:18:55.000000 yandex_api_client-0.0.2/yandex_api_client/models/get_offer_mapping_dto.py
+-rw-r--r--   0        0        0     3418 2024-04-09 12:18:55.000000 yandex_api_client-0.0.2/yandex_api_client/models/get_offer_mapping_entries_response.py
+-rw-r--r--   0        0        0     5016 2024-04-09 12:18:55.000000 yandex_api_client-0.0.2/yandex_api_client/models/get_offer_mappings_request.py
+-rw-r--r--   0        0        0     3360 2024-04-09 12:18:55.000000 yandex_api_client-0.0.2/yandex_api_client/models/get_offer_mappings_response.py
+-rw-r--r--   0        0        0     3923 2024-04-09 12:18:55.000000 yandex_api_client-0.0.2/yandex_api_client/models/get_offer_mappings_result_dto.py
+-rw-r--r--   0        0        0     4205 2024-04-09 12:18:55.000000 yandex_api_client-0.0.2/yandex_api_client/models/get_offer_recommendations_request.py
+-rw-r--r--   0        0        0     3403 2024-04-09 12:18:55.000000 yandex_api_client-0.0.2/yandex_api_client/models/get_offer_recommendations_response.py
+-rw-r--r--   0        0        0     3791 2024-04-09 12:18:55.000000 yandex_api_client-0.0.2/yandex_api_client/models/get_offers_response.py
+-rw-r--r--   0        0        0     3331 2024-04-09 12:18:55.000000 yandex_api_client-0.0.2/yandex_api_client/models/get_order_buyer_info_response.py
+-rw-r--r--   0        0        0     3364 2024-04-09 12:18:55.000000 yandex_api_client-0.0.2/yandex_api_client/models/get_order_labels_data_response.py
+-rw-r--r--   0        0        0     3062 2024-04-09 12:18:55.000000 yandex_api_client-0.0.2/yandex_api_client/models/get_order_response.py
+-rw-r--r--   0        0        0     3794 2024-04-09 12:18:55.000000 yandex_api_client-0.0.2/yandex_api_client/models/get_orders_response.py
+-rw-r--r--   0        0        0     5466 2024-04-09 12:18:55.000000 yandex_api_client-0.0.2/yandex_api_client/models/get_orders_stats_request.py
+-rw-r--r--   0        0        0     3354 2024-04-09 12:18:55.000000 yandex_api_client-0.0.2/yandex_api_client/models/get_orders_stats_response.py
+-rw-r--r--   0        0        0     3363 2024-04-09 12:18:55.000000 yandex_api_client-0.0.2/yandex_api_client/models/get_outlet_licenses_response.py
+-rw-r--r--   0        0        0     3156 2024-04-09 12:18:55.000000 yandex_api_client-0.0.2/yandex_api_client/models/get_outlet_response.py
+-rw-r--r--   0        0        0     4244 2024-04-09 12:18:55.000000 yandex_api_client-0.0.2/yandex_api_client/models/get_outlets_response.py
+-rw-r--r--   0        0        0     3410 2024-04-09 12:18:55.000000 yandex_api_client-0.0.2/yandex_api_client/models/get_price_dto.py
+-rw-r--r--   0        0        0     4044 2024-04-09 12:18:55.000000 yandex_api_client-0.0.2/yandex_api_client/models/get_price_with_discount_dto.py
+-rw-r--r--   0        0        0     4422 2024-04-09 12:18:55.000000 yandex_api_client-0.0.2/yandex_api_client/models/get_price_with_vat_dto.py
+-rw-r--r--   0        0        0     3058 2024-04-09 12:18:55.000000 yandex_api_client-0.0.2/yandex_api_client/models/get_prices_by_offer_ids_request.py
+-rw-r--r--   0        0        0     3437 2024-04-09 12:18:55.000000 yandex_api_client-0.0.2/yandex_api_client/models/get_prices_by_offer_ids_response.py
+-rw-r--r--   0        0        0     3364 2024-04-09 12:18:55.000000 yandex_api_client-0.0.2/yandex_api_client/models/get_prices_response.py
+-rw-r--r--   0        0        0     4778 2024-04-09 12:18:55.000000 yandex_api_client-0.0.2/yandex_api_client/models/get_quarantine_offers_request.py
+-rw-r--r--   0        0        0     3436 2024-04-09 12:18:55.000000 yandex_api_client-0.0.2/yandex_api_client/models/get_quarantine_offers_response.py
+-rw-r--r--   0        0        0     3880 2024-04-09 12:18:55.000000 yandex_api_client-0.0.2/yandex_api_client/models/get_quarantine_offers_result_dto.py
+-rw-r--r--   0        0        0     3529 2024-04-09 12:18:55.000000 yandex_api_client-0.0.2/yandex_api_client/models/get_region_with_children_response.py
+-rw-r--r--   0        0        0     3782 2024-04-09 12:18:55.000000 yandex_api_client-0.0.2/yandex_api_client/models/get_regions_response.py
+-rw-r--r--   0        0        0     3345 2024-04-09 12:18:55.000000 yandex_api_client-0.0.2/yandex_api_client/models/get_report_info_response.py
+-rw-r--r--   0        0        0     3265 2024-04-09 12:18:55.000000 yandex_api_client-0.0.2/yandex_api_client/models/get_return_response.py
+-rw-r--r--   0        0        0     3294 2024-04-09 12:18:55.000000 yandex_api_client-0.0.2/yandex_api_client/models/get_returns_response.py
+-rw-r--r--   0        0        0     3363 2024-04-09 12:18:55.000000 yandex_api_client-0.0.2/yandex_api_client/models/get_shipment_orders_info_response.py
+-rw-r--r--   0        0        0     3281 2024-04-09 12:18:55.000000 yandex_api_client-0.0.2/yandex_api_client/models/get_shipment_response.py
+-rw-r--r--   0        0        0     3535 2024-04-09 12:18:55.000000 yandex_api_client-0.0.2/yandex_api_client/models/get_suggested_offer_mapping_entries_request.py
+-rw-r--r--   0        0        0     3493 2024-04-09 12:18:55.000000 yandex_api_client-0.0.2/yandex_api_client/models/get_suggested_offer_mapping_entries_response.py
+-rw-r--r--   0        0        0     3425 2024-04-09 12:18:55.000000 yandex_api_client-0.0.2/yandex_api_client/models/get_suggested_offer_mappings_request.py
+-rw-r--r--   0        0        0     3433 2024-04-09 12:18:55.000000 yandex_api_client-0.0.2/yandex_api_client/models/get_suggested_offer_mappings_response.py
+-rw-r--r--   0        0        0     3488 2024-04-09 12:18:55.000000 yandex_api_client-0.0.2/yandex_api_client/models/get_suggested_offer_mappings_result_dto.py
+-rw-r--r--   0        0        0     3929 2024-04-09 12:18:55.000000 yandex_api_client-0.0.2/yandex_api_client/models/get_warehouse_stocks_dto.py
+-rw-r--r--   0        0        0     4589 2024-04-09 12:18:55.000000 yandex_api_client-0.0.2/yandex_api_client/models/get_warehouse_stocks_request.py
+-rw-r--r--   0        0        0     3351 2024-04-09 12:18:55.000000 yandex_api_client-0.0.2/yandex_api_client/models/get_warehouse_stocks_response.py
+-rw-r--r--   0        0        0     3297 2024-04-09 12:18:55.000000 yandex_api_client-0.0.2/yandex_api_client/models/get_warehouses_response.py
+-rw-r--r--   0        0        0     3412 2024-04-09 12:18:55.000000 yandex_api_client-0.0.2/yandex_api_client/models/goods_stats_dto.py
+-rw-r--r--   0        0        0     8466 2024-04-09 12:18:55.000000 yandex_api_client-0.0.2/yandex_api_client/models/goods_stats_goods_dto.py
+-rw-r--r--   0        0        0     3758 2024-04-09 12:18:55.000000 yandex_api_client-0.0.2/yandex_api_client/models/goods_stats_warehouse_dto.py
+-rw-r--r--   0        0        0     3844 2024-04-09 12:18:55.000000 yandex_api_client-0.0.2/yandex_api_client/models/goods_stats_weight_dimensions_dto.py
+-rw-r--r--   0        0        0     3043 2024-04-09 12:18:55.000000 yandex_api_client-0.0.2/yandex_api_client/models/gps_dto.py
+-rw-r--r--   0        0        0     4495 2024-04-09 12:18:55.000000 yandex_api_client-0.0.2/yandex_api_client/models/hidden_offer_dto.py
+-rw-r--r--   0        0        0     1552 2024-04-09 12:18:55.000000 yandex_api_client-0.0.2/yandex_api_client/models/license_check_status_type.py
+-rw-r--r--   0        0        0     1347 2024-04-09 12:18:55.000000 yandex_api_client-0.0.2/yandex_api_client/models/license_type.py
+-rw-r--r--   0        0        0     4262 2024-04-09 12:18:55.000000 yandex_api_client-0.0.2/yandex_api_client/models/logistic_pickup_point_dto.py
+-rw-r--r--   0        0        0     1847 2024-04-09 12:18:55.000000 yandex_api_client-0.0.2/yandex_api_client/models/logistic_point_type.py
+-rw-r--r--   0        0        0    22333 2024-04-09 12:18:55.000000 yandex_api_client-0.0.2/yandex_api_client/models/mappings_offer_dto.py
+-rw-r--r--   0        0        0    22165 2024-04-09 12:18:55.000000 yandex_api_client-0.0.2/yandex_api_client/models/mappings_offer_info_dto.py
+-rw-r--r--   0        0        0     3441 2024-04-09 12:18:55.000000 yandex_api_client-0.0.2/yandex_api_client/models/model_dto.py
+-rw-r--r--   0        0        0     6237 2024-04-09 12:18:55.000000 yandex_api_client-0.0.2/yandex_api_client/models/model_offer_dto.py
+-rw-r--r--   0        0        0     3461 2024-04-09 12:18:55.000000 yandex_api_client-0.0.2/yandex_api_client/models/model_price_dto.py
+-rw-r--r--   0        0        0     1988 2024-04-09 12:18:55.000000 yandex_api_client-0.0.2/yandex_api_client/models/offer_availability_status_type.py
+-rw-r--r--   0        0        0     3132 2024-04-09 12:18:55.000000 yandex_api_client-0.0.2/yandex_api_client/models/offer_campaign_status_dto.py
+-rw-r--r--   0        0        0     2061 2024-04-09 12:18:55.000000 yandex_api_client-0.0.2/yandex_api_client/models/offer_campaign_status_type.py
+-rw-r--r--   0        0        0     8069 2024-04-09 12:18:55.000000 yandex_api_client-0.0.2/yandex_api_client/models/offer_card_dto.py
+-rw-r--r--   0        0        0     3354 2024-04-09 12:18:55.000000 yandex_api_client-0.0.2/yandex_api_client/models/offer_card_recommendation_dto.py
+-rw-r--r--   0        0        0     4454 2024-04-09 12:18:55.000000 yandex_api_client-0.0.2/yandex_api_client/models/offer_card_recommendation_type.py
+-rw-r--r--   0        0        0     2484 2024-04-09 12:18:55.000000 yandex_api_client-0.0.2/yandex_api_client/models/offer_card_status_type.py
+-rw-r--r--   0        0        0     4025 2024-04-09 12:18:55.000000 yandex_api_client-0.0.2/yandex_api_client/models/offer_cards_content_status_dto.py
+-rw-r--r--   0        0        0     3421 2024-04-09 12:18:55.000000 yandex_api_client-0.0.2/yandex_api_client/models/offer_condition_dto.py
+-rw-r--r--   0        0        0     1472 2024-04-09 12:18:55.000000 yandex_api_client-0.0.2/yandex_api_client/models/offer_condition_quality_type.py
+-rw-r--r--   0        0        0     2153 2024-04-09 12:18:55.000000 yandex_api_client-0.0.2/yandex_api_client/models/offer_condition_type.py
+-rw-r--r--   0        0        0     5806 2024-04-09 12:18:55.000000 yandex_api_client-0.0.2/yandex_api_client/models/offer_content_dto.py
+-rw-r--r--   0        0        0     3349 2024-04-09 12:18:55.000000 yandex_api_client-0.0.2/yandex_api_client/models/offer_content_error_dto.py
+-rw-r--r--   0        0        0     2424 2024-04-09 12:18:55.000000 yandex_api_client-0.0.2/yandex_api_client/models/offer_content_error_type.py
+-rw-r--r--   0        0        0     8257 2024-04-09 12:18:55.000000 yandex_api_client-0.0.2/yandex_api_client/models/offer_dto.py
+-rw-r--r--   0        0        0     3100 2024-04-09 12:18:55.000000 yandex_api_client-0.0.2/yandex_api_client/models/offer_error_dto.py
+-rw-r--r--   0        0        0     5887 2024-04-09 12:18:55.000000 yandex_api_client-0.0.2/yandex_api_client/models/offer_for_recommendation_dto.py
+-rw-r--r--   0        0        0     3152 2024-04-09 12:18:55.000000 yandex_api_client-0.0.2/yandex_api_client/models/offer_manual_dto.py
+-rw-r--r--   0        0        0     3746 2024-04-09 12:18:55.000000 yandex_api_client-0.0.2/yandex_api_client/models/offer_mapping_dto.py
+-rw-r--r--   0        0        0     4026 2024-04-09 12:18:55.000000 yandex_api_client-0.0.2/yandex_api_client/models/offer_mapping_entries_dto.py
+-rw-r--r--   0        0        0     4562 2024-04-09 12:18:55.000000 yandex_api_client-0.0.2/yandex_api_client/models/offer_mapping_entry_dto.py
+-rw-r--r--   0        0        0     4191 2024-04-09 12:18:55.000000 yandex_api_client-0.0.2/yandex_api_client/models/offer_mapping_info_dto.py
+-rw-r--r--   0        0        0     1239 2024-04-09 12:18:55.000000 yandex_api_client-0.0.2/yandex_api_client/models/offer_mapping_kind_type.py
+-rw-r--r--   0        0        0     3490 2024-04-09 12:18:55.000000 yandex_api_client-0.0.2/yandex_api_client/models/offer_mapping_suggestions_list_dto.py
+-rw-r--r--   0        0        0     3696 2024-04-09 12:18:55.000000 yandex_api_client-0.0.2/yandex_api_client/models/offer_param_dto.py
+-rw-r--r--   0        0        0     3897 2024-04-09 12:18:55.000000 yandex_api_client-0.0.2/yandex_api_client/models/offer_price_by_offer_ids_list_response_dto.py
+-rw-r--r--   0        0        0     5184 2024-04-09 12:18:55.000000 yandex_api_client-0.0.2/yandex_api_client/models/offer_price_by_offer_ids_response_dto.py
+-rw-r--r--   0        0        0     7514 2024-04-09 12:18:55.000000 yandex_api_client-0.0.2/yandex_api_client/models/offer_price_dto.py
+-rw-r--r--   0        0        0     3019 2024-04-09 12:18:55.000000 yandex_api_client-0.0.2/yandex_api_client/models/offer_price_feed_dto.py
+-rw-r--r--   0        0        0     4054 2024-04-09 12:18:55.000000 yandex_api_client-0.0.2/yandex_api_client/models/offer_price_list_response_dto.py
+-rw-r--r--   0        0        0     4207 2024-04-09 12:18:55.000000 yandex_api_client-0.0.2/yandex_api_client/models/offer_price_response_dto.py
+-rw-r--r--   0        0        0     3238 2024-04-09 12:18:55.000000 yandex_api_client-0.0.2/yandex_api_client/models/offer_processing_note_dto.py
+-rw-r--r--   0        0        0     6259 2024-04-09 12:18:55.000000 yandex_api_client-0.0.2/yandex_api_client/models/offer_processing_note_type.py
+-rw-r--r--   0        0        0     3725 2024-04-09 12:18:55.000000 yandex_api_client-0.0.2/yandex_api_client/models/offer_processing_state_dto.py
+-rw-r--r--   0        0        0     2806 2024-04-09 12:18:55.000000 yandex_api_client-0.0.2/yandex_api_client/models/offer_processing_status_type.py
+-rw-r--r--   0        0        0     3728 2024-04-09 12:18:55.000000 yandex_api_client-0.0.2/yandex_api_client/models/offer_recommendation_dto.py
+-rw-r--r--   0        0        0     5872 2024-04-09 12:18:55.000000 yandex_api_client-0.0.2/yandex_api_client/models/offer_recommendation_info_dto.py
+-rw-r--r--   0        0        0     4047 2024-04-09 12:18:55.000000 yandex_api_client-0.0.2/yandex_api_client/models/offer_recommendations_result_dto.py
+-rw-r--r--   0        0        0     3276 2024-04-09 12:18:55.000000 yandex_api_client-0.0.2/yandex_api_client/models/offer_selling_program_dto.py
+-rw-r--r--   0        0        0     1386 2024-04-09 12:18:55.000000 yandex_api_client-0.0.2/yandex_api_client/models/offer_selling_program_status_type.py
+-rw-r--r--   0        0        0     1900 2024-04-09 12:18:55.000000 yandex_api_client-0.0.2/yandex_api_client/models/offer_type.py
+-rw-r--r--   0        0        0     3773 2024-05-13 13:18:43.820928 yandex_api_client-0.0.2/yandex_api_client/models/offer_weight_dimensions_dto.py
+-rw-r--r--   0        0        0     3371 2024-04-09 12:18:55.000000 yandex_api_client-0.0.2/yandex_api_client/models/offers_dto.py
+-rw-r--r--   0        0        0     3499 2024-04-09 12:18:55.000000 yandex_api_client-0.0.2/yandex_api_client/models/option_values_limited_dto.py
+-rw-r--r--   0        0        0     3602 2024-04-09 12:18:55.000000 yandex_api_client-0.0.2/yandex_api_client/models/order_box_layout_dto.py
+-rw-r--r--   0        0        0     5090 2024-04-09 12:18:55.000000 yandex_api_client-0.0.2/yandex_api_client/models/order_box_layout_item_dto.py
+-rw-r--r--   0        0        0     3219 2024-04-09 12:18:55.000000 yandex_api_client-0.0.2/yandex_api_client/models/order_box_layout_partial_count_dto.py
+-rw-r--r--   0        0        0     3409 2024-04-09 12:18:55.000000 yandex_api_client-0.0.2/yandex_api_client/models/order_boxes_layout_dto.py
+-rw-r--r--   0        0        0     3517 2024-04-09 12:18:55.000000 yandex_api_client-0.0.2/yandex_api_client/models/order_business_buyer_dto.py
+-rw-r--r--   0        0        0     4401 2024-04-09 12:18:55.000000 yandex_api_client-0.0.2/yandex_api_client/models/order_business_documents_dto.py
+-rw-r--r--   0        0        0     3690 2024-04-09 12:18:55.000000 yandex_api_client-0.0.2/yandex_api_client/models/order_buyer_basic_info_dto.py
+-rw-r--r--   0        0        0     3792 2024-04-09 12:18:55.000000 yandex_api_client-0.0.2/yandex_api_client/models/order_buyer_dto.py
+-rw-r--r--   0        0        0     4155 2024-04-09 12:18:55.000000 yandex_api_client-0.0.2/yandex_api_client/models/order_buyer_info_dto.py
+-rw-r--r--   0        0        0     1330 2024-04-09 12:18:55.000000 yandex_api_client-0.0.2/yandex_api_client/models/order_buyer_type.py
+-rw-r--r--   0        0        0     1504 2024-04-09 12:18:55.000000 yandex_api_client-0.0.2/yandex_api_client/models/order_cancellation_reason_type.py
+-rw-r--r--   0        0        0     3830 2024-04-09 12:18:55.000000 yandex_api_client-0.0.2/yandex_api_client/models/order_courier_dto.py
+-rw-r--r--   0        0        0     5760 2024-04-09 12:18:55.000000 yandex_api_client-0.0.2/yandex_api_client/models/order_delivery_address_dto.py
+-rw-r--r--   0        0        0     3020 2024-04-09 12:18:55.000000 yandex_api_client-0.0.2/yandex_api_client/models/order_delivery_date_dto.py
+-rw-r--r--   0        0        0     1971 2024-04-09 12:18:55.000000 yandex_api_client-0.0.2/yandex_api_client/models/order_delivery_date_reason_type.py
+-rw-r--r--   0        0        0     4466 2024-04-09 12:18:55.000000 yandex_api_client-0.0.2/yandex_api_client/models/order_delivery_dates_dto.py
+-rw-r--r--   0        0        0     1945 2024-04-09 12:18:55.000000 yandex_api_client-0.0.2/yandex_api_client/models/order_delivery_dispatch_type.py
+-rw-r--r--   0        0        0     9811 2024-04-09 12:18:55.000000 yandex_api_client-0.0.2/yandex_api_client/models/order_delivery_dto.py
+-rw-r--r--   0        0        0     1648 2024-04-09 12:18:55.000000 yandex_api_client-0.0.2/yandex_api_client/models/order_delivery_eac_type.py
+-rw-r--r--   0        0        0     1676 2024-04-09 12:18:55.000000 yandex_api_client-0.0.2/yandex_api_client/models/order_delivery_partner_type.py
+-rw-r--r--   0        0        0     1506 2024-04-09 12:18:55.000000 yandex_api_client-0.0.2/yandex_api_client/models/order_delivery_type.py
+-rw-r--r--   0        0        0     3824 2024-04-09 12:18:55.000000 yandex_api_client-0.0.2/yandex_api_client/models/order_digital_item_dto.py
+-rw-r--r--   0        0        0     1326 2024-04-09 12:18:55.000000 yandex_api_client-0.0.2/yandex_api_client/models/order_document_status_type.py
+-rw-r--r--   0        0        0    12140 2024-04-09 12:18:55.000000 yandex_api_client-0.0.2/yandex_api_client/models/order_dto.py
+-rw-r--r--   0        0        0     3423 2024-04-09 12:18:55.000000 yandex_api_client-0.0.2/yandex_api_client/models/order_item_detail_dto.py
+-rw-r--r--   0        0        0    13849 2024-04-09 12:18:55.000000 yandex_api_client-0.0.2/yandex_api_client/models/order_item_dto.py
+-rw-r--r--   0        0        0     5232 2024-04-09 12:18:55.000000 yandex_api_client-0.0.2/yandex_api_client/models/order_item_instance_dto.py
+-rw-r--r--   0        0        0     3960 2024-04-09 12:18:55.000000 yandex_api_client-0.0.2/yandex_api_client/models/order_item_instance_modification_dto.py
+-rw-r--r--   0        0        0     1286 2024-04-09 12:18:55.000000 yandex_api_client-0.0.2/yandex_api_client/models/order_item_instance_type.py
+-rw-r--r--   0        0        0     4709 2024-04-09 12:18:55.000000 yandex_api_client-0.0.2/yandex_api_client/models/order_item_modification_dto.py
+-rw-r--r--   0        0        0     4438 2024-04-09 12:18:55.000000 yandex_api_client-0.0.2/yandex_api_client/models/order_item_promo_dto.py
+-rw-r--r--   0        0        0     1297 2024-04-09 12:18:55.000000 yandex_api_client-0.0.2/yandex_api_client/models/order_item_status_type.py
+-rw-r--r--   0        0        0     3470 2024-04-09 12:18:55.000000 yandex_api_client-0.0.2/yandex_api_client/models/order_item_subsidy_dto.py
+-rw-r--r--   0        0        0     1389 2024-04-09 12:18:55.000000 yandex_api_client-0.0.2/yandex_api_client/models/order_items_modification_request_reason_type.py
+-rw-r--r--   0        0        0     3580 2024-04-09 12:18:55.000000 yandex_api_client-0.0.2/yandex_api_client/models/order_items_modification_result_dto.py
+-rw-r--r--   0        0        0     4239 2024-04-09 12:18:55.000000 yandex_api_client-0.0.2/yandex_api_client/models/order_label_dto.py
+-rw-r--r--   0        0        0     1664 2024-04-09 12:18:55.000000 yandex_api_client-0.0.2/yandex_api_client/models/order_lift_type.py
+-rw-r--r--   0        0        0     3225 2024-04-09 12:18:55.000000 yandex_api_client-0.0.2/yandex_api_client/models/order_parcel_box_dto.py
+-rw-r--r--   0        0        0     1381 2024-04-09 12:18:55.000000 yandex_api_client-0.0.2/yandex_api_client/models/order_parcel_status_type.py
+-rw-r--r--   0        0        0     3028 2024-04-09 12:18:55.000000 yandex_api_client-0.0.2/yandex_api_client/models/order_payment_method_type.py
+-rw-r--r--   0        0        0     1535 2024-04-09 12:18:55.000000 yandex_api_client-0.0.2/yandex_api_client/models/order_payment_type.py
+-rw-r--r--   0        0        0     3359 2024-04-09 12:18:55.000000 yandex_api_client-0.0.2/yandex_api_client/models/order_promo_type.py
+-rw-r--r--   0        0        0     5487 2024-04-09 12:18:55.000000 yandex_api_client-0.0.2/yandex_api_client/models/order_shipment_dto.py
+-rw-r--r--   0        0        0     3213 2024-04-09 12:18:55.000000 yandex_api_client-0.0.2/yandex_api_client/models/order_state_dto.py
+-rw-r--r--   0        0        0     2823 2024-04-09 12:18:55.000000 yandex_api_client-0.0.2/yandex_api_client/models/order_stats_status_type.py
+-rw-r--r--   0        0        0     3064 2024-04-09 12:18:55.000000 yandex_api_client-0.0.2/yandex_api_client/models/order_status_change_delivery_dates_dto.py
+-rw-r--r--   0        0        0     3227 2024-04-09 12:18:55.000000 yandex_api_client-0.0.2/yandex_api_client/models/order_status_change_delivery_dto.py
+-rw-r--r--   0        0        0     3517 2024-04-09 12:18:55.000000 yandex_api_client-0.0.2/yandex_api_client/models/order_status_change_dto.py
+-rw-r--r--   0        0        0     2147 2024-04-09 12:18:55.000000 yandex_api_client-0.0.2/yandex_api_client/models/order_status_type.py
+-rw-r--r--   0        0        0     1952 2024-04-09 12:18:55.000000 yandex_api_client-0.0.2/yandex_api_client/models/order_subsidy_type.py
+-rw-r--r--   0        0        0     9431 2024-04-09 12:18:55.000000 yandex_api_client-0.0.2/yandex_api_client/models/order_substatus_type.py
+-rw-r--r--   0        0        0     2234 2024-04-09 12:18:55.000000 yandex_api_client-0.0.2/yandex_api_client/models/order_tax_system_type.py
+-rw-r--r--   0        0        0     3421 2024-04-09 12:18:55.000000 yandex_api_client-0.0.2/yandex_api_client/models/order_track_dto.py
+-rw-r--r--   0        0        0     1471 2024-04-09 12:18:55.000000 yandex_api_client-0.0.2/yandex_api_client/models/order_update_status_type.py
+-rw-r--r--   0        0        0     2494 2024-04-09 12:18:55.000000 yandex_api_client-0.0.2/yandex_api_client/models/order_vat_type.py
+-rw-r--r--   0        0        0     3461 2024-04-09 12:18:55.000000 yandex_api_client-0.0.2/yandex_api_client/models/orders_shipment_info_dto.py
+-rw-r--r--   0        0        0     3385 2024-04-09 12:18:55.000000 yandex_api_client-0.0.2/yandex_api_client/models/orders_stats_commission_dto.py
+-rw-r--r--   0        0        0     2748 2024-04-09 12:18:55.000000 yandex_api_client-0.0.2/yandex_api_client/models/orders_stats_commission_type.py
+-rw-r--r--   0        0        0     3153 2024-04-09 12:18:55.000000 yandex_api_client-0.0.2/yandex_api_client/models/orders_stats_delivery_region_dto.py
+-rw-r--r--   0        0        0     3898 2024-04-09 12:18:55.000000 yandex_api_client-0.0.2/yandex_api_client/models/orders_stats_details_dto.py
+-rw-r--r--   0        0        0     3824 2024-04-09 12:18:55.000000 yandex_api_client-0.0.2/yandex_api_client/models/orders_stats_dto.py
+-rw-r--r--   0        0        0     9813 2024-04-09 12:18:55.000000 yandex_api_client-0.0.2/yandex_api_client/models/orders_stats_item_dto.py
+-rw-r--r--   0        0        0     1430 2024-04-09 12:18:55.000000 yandex_api_client-0.0.2/yandex_api_client/models/orders_stats_item_status_type.py
+-rw-r--r--   0        0        0     8086 2024-04-09 12:18:55.000000 yandex_api_client-0.0.2/yandex_api_client/models/orders_stats_order_dto.py
+-rw-r--r--   0        0        0     1576 2024-04-09 12:18:55.000000 yandex_api_client-0.0.2/yandex_api_client/models/orders_stats_order_payment_type.py
+-rw-r--r--   0        0        0     4571 2024-04-09 12:18:55.000000 yandex_api_client-0.0.2/yandex_api_client/models/orders_stats_payment_dto.py
+-rw-r--r--   0        0        0     3222 2024-04-09 12:18:55.000000 yandex_api_client-0.0.2/yandex_api_client/models/orders_stats_payment_order_dto.py
+-rw-r--r--   0        0        0     1748 2024-04-09 12:18:55.000000 yandex_api_client-0.0.2/yandex_api_client/models/orders_stats_payment_source_type.py
+-rw-r--r--   0        0        0     1356 2024-04-09 12:18:55.000000 yandex_api_client-0.0.2/yandex_api_client/models/orders_stats_payment_type.py
+-rw-r--r--   0        0        0     3674 2024-04-09 12:18:55.000000 yandex_api_client-0.0.2/yandex_api_client/models/orders_stats_price_dto.py
+-rw-r--r--   0        0        0     1565 2024-04-09 12:18:55.000000 yandex_api_client-0.0.2/yandex_api_client/models/orders_stats_price_type.py
+-rw-r--r--   0        0        0     1488 2024-04-09 12:18:55.000000 yandex_api_client-0.0.2/yandex_api_client/models/orders_stats_stock_type.py
+-rw-r--r--   0        0        0     3130 2024-04-09 12:18:55.000000 yandex_api_client-0.0.2/yandex_api_client/models/orders_stats_warehouse_dto.py
+-rw-r--r--   0        0        0     5461 2024-04-09 12:18:55.000000 yandex_api_client-0.0.2/yandex_api_client/models/outlet_address_dto.py
+-rw-r--r--   0        0        0     8909 2024-04-09 12:18:55.000000 yandex_api_client-0.0.2/yandex_api_client/models/outlet_delivery_rule_dto.py
+-rw-r--r--   0        0        0     6846 2024-04-09 12:18:55.000000 yandex_api_client-0.0.2/yandex_api_client/models/outlet_dto.py
+-rw-r--r--   0        0        0     6149 2024-04-09 12:18:55.000000 yandex_api_client-0.0.2/yandex_api_client/models/outlet_license_dto.py
+-rw-r--r--   0        0        0     3508 2024-04-09 12:18:55.000000 yandex_api_client-0.0.2/yandex_api_client/models/outlet_licenses_response_dto.py
+-rw-r--r--   0        0        0     3039 2024-04-09 12:18:55.000000 yandex_api_client-0.0.2/yandex_api_client/models/outlet_response_dto.py
+-rw-r--r--   0        0        0     1672 2024-04-09 12:18:55.000000 yandex_api_client-0.0.2/yandex_api_client/models/outlet_status_type.py
+-rw-r--r--   0        0        0     1592 2024-04-09 12:18:55.000000 yandex_api_client-0.0.2/yandex_api_client/models/outlet_type.py
+-rw-r--r--   0        0        0     1445 2024-04-09 12:18:55.000000 yandex_api_client-0.0.2/yandex_api_client/models/outlet_visibility_type.py
+-rw-r--r--   0        0        0     4252 2024-04-09 12:18:55.000000 yandex_api_client-0.0.2/yandex_api_client/models/outlet_working_schedule_dto.py
+-rw-r--r--   0        0        0     3650 2024-04-09 12:18:55.000000 yandex_api_client-0.0.2/yandex_api_client/models/outlet_working_schedule_item_dto.py
+-rw-r--r--   0        0        0     1758 2024-04-09 12:18:55.000000 yandex_api_client-0.0.2/yandex_api_client/models/page_format_type.py
+-rw-r--r--   0        0        0     3774 2024-04-09 12:18:55.000000 yandex_api_client-0.0.2/yandex_api_client/models/paged_returns_dto.py
+-rw-r--r--   0        0        0     3195 2024-04-09 12:18:55.000000 yandex_api_client-0.0.2/yandex_api_client/models/pallets_count_dto.py
+-rw-r--r--   0        0        0     1424 2024-04-09 12:18:55.000000 yandex_api_client-0.0.2/yandex_api_client/models/parameter_type.py
+-rw-r--r--   0        0        0     3460 2024-04-09 12:18:55.000000 yandex_api_client-0.0.2/yandex_api_client/models/parameter_value_constraints_dto.py
+-rw-r--r--   0        0        0     4632 2024-04-09 12:18:55.000000 yandex_api_client-0.0.2/yandex_api_client/models/parameter_value_dto.py
+-rw-r--r--   0        0        0     3212 2024-04-09 12:18:55.000000 yandex_api_client-0.0.2/yandex_api_client/models/parameter_value_option_dto.py
+-rw-r--r--   0        0        0     4104 2024-04-09 12:18:55.000000 yandex_api_client-0.0.2/yandex_api_client/models/parcel_box_dto.py
+-rw-r--r--   0        0        0     6283 2024-04-09 12:18:55.000000 yandex_api_client-0.0.2/yandex_api_client/models/parcel_box_label_dto.py
+-rw-r--r--   0        0        0     3519 2024-04-09 12:18:55.000000 yandex_api_client-0.0.2/yandex_api_client/models/parcel_dto.py
+-rw-r--r--   0        0        0     3334 2024-04-09 12:18:55.000000 yandex_api_client-0.0.2/yandex_api_client/models/partner_shipment_warehouse_dto.py
+-rw-r--r--   0        0        0     1644 2024-04-09 12:18:55.000000 yandex_api_client-0.0.2/yandex_api_client/models/payment_frequency_type.py
+-rw-r--r--   0        0        0     3442 2024-04-09 12:18:55.000000 yandex_api_client-0.0.2/yandex_api_client/models/pickup_address_dto.py
+-rw-r--r--   0        0        0     1354 2024-04-09 12:18:55.000000 yandex_api_client-0.0.2/yandex_api_client/models/placement_type.py
+-rw-r--r--   0        0        0     3816 2024-04-09 12:18:55.000000 yandex_api_client-0.0.2/yandex_api_client/models/price_competitiveness_thresholds_dto.py
+-rw-r--r--   0        0        0     1427 2024-04-09 12:18:55.000000 yandex_api_client-0.0.2/yandex_api_client/models/price_competitiveness_type.py
+-rw-r--r--   0        0        0     4189 2024-04-09 12:18:55.000000 yandex_api_client-0.0.2/yandex_api_client/models/price_dto.py
+-rw-r--r--   0        0        0     3900 2024-04-09 12:18:55.000000 yandex_api_client-0.0.2/yandex_api_client/models/price_quarantine_verdict_dto.py
+-rw-r--r--   0        0        0     1871 2024-04-09 12:18:55.000000 yandex_api_client-0.0.2/yandex_api_client/models/price_quarantine_verdict_param_name_type.py
+-rw-r--r--   0        0        0     3138 2024-04-09 12:18:55.000000 yandex_api_client-0.0.2/yandex_api_client/models/price_quarantine_verdict_parameter_dto.py
+-rw-r--r--   0        0        0     2195 2024-04-09 12:18:55.000000 yandex_api_client-0.0.2/yandex_api_client/models/price_quarantine_verdict_type.py
+-rw-r--r--   0        0        0     3525 2024-04-09 12:18:55.000000 yandex_api_client-0.0.2/yandex_api_client/models/price_recommendation_item_dto.py
+-rw-r--r--   0        0        0     3081 2024-04-09 12:18:55.000000 yandex_api_client-0.0.2/yandex_api_client/models/price_suggest_dto.py
+-rw-r--r--   0        0        0     5465 2024-04-09 12:18:55.000000 yandex_api_client-0.0.2/yandex_api_client/models/price_suggest_offer_dto.py
+-rw-r--r--   0        0        0     4268 2024-04-09 12:18:55.000000 yandex_api_client-0.0.2/yandex_api_client/models/price_suggest_type.py
+-rw-r--r--   0        0        0     3828 2024-04-09 12:18:55.000000 yandex_api_client-0.0.2/yandex_api_client/models/provide_order_digital_codes_request.py
+-rw-r--r--   0        0        0     3494 2024-04-09 12:18:55.000000 yandex_api_client-0.0.2/yandex_api_client/models/provide_order_item_identifiers_request.py
+-rw-r--r--   0        0        0     3428 2024-04-09 12:18:55.000000 yandex_api_client-0.0.2/yandex_api_client/models/provide_order_item_identifiers_response.py
+-rw-r--r--   0        0        0     3488 2024-04-09 12:18:55.000000 yandex_api_client-0.0.2/yandex_api_client/models/put_sku_bids_request.py
+-rw-r--r--   0        0        0     4219 2024-04-09 12:18:55.000000 yandex_api_client-0.0.2/yandex_api_client/models/quantum_dto.py
+-rw-r--r--   0        0        0     6144 2024-04-09 12:18:55.000000 yandex_api_client-0.0.2/yandex_api_client/models/quarantine_offer_dto.py
+-rw-r--r--   0        0        0     1460 2024-04-09 12:18:55.000000 yandex_api_client-0.0.2/yandex_api_client/models/recipient_type.py
+-rw-r--r--   0        0        0     2391 2024-04-09 12:18:55.000000 yandex_api_client-0.0.2/yandex_api_client/models/refund_status_type.py
+-rw-r--r--   0        0        0     4100 2024-04-09 12:18:55.000000 yandex_api_client-0.0.2/yandex_api_client/models/region_dto.py
+-rw-r--r--   0        0        0     2019 2024-04-09 12:18:55.000000 yandex_api_client-0.0.2/yandex_api_client/models/region_type.py
+-rw-r--r--   0        0        0     3503 2024-04-09 12:18:55.000000 yandex_api_client-0.0.2/yandex_api_client/models/regional_model_info_dto.py
+-rw-r--r--   0        0        0     1387 2024-04-09 12:18:55.000000 yandex_api_client-0.0.2/yandex_api_client/models/report_format_type.py
+-rw-r--r--   0        0        0     4220 2024-04-09 12:18:55.000000 yandex_api_client-0.0.2/yandex_api_client/models/report_info_dto.py
+-rw-r--r--   0        0        0     1547 2024-04-09 12:18:55.000000 yandex_api_client-0.0.2/yandex_api_client/models/report_status_type.py
+-rw-r--r--   0        0        0     1546 2024-04-09 12:18:55.000000 yandex_api_client-0.0.2/yandex_api_client/models/report_sub_status_type.py
+-rw-r--r--   0        0        0     4753 2024-04-09 12:18:55.000000 yandex_api_client-0.0.2/yandex_api_client/models/return_decision_dto.py
+-rw-r--r--   0        0        0     2000 2024-04-09 12:18:55.000000 yandex_api_client-0.0.2/yandex_api_client/models/return_decision_reason_type.py
+-rw-r--r--   0        0        0     2530 2024-04-09 12:18:55.000000 yandex_api_client-0.0.2/yandex_api_client/models/return_decision_subreason_type.py
+-rw-r--r--   0        0        0     1989 2024-04-09 12:18:55.000000 yandex_api_client-0.0.2/yandex_api_client/models/return_decision_type.py
+-rw-r--r--   0        0        0     5892 2024-04-09 12:18:55.000000 yandex_api_client-0.0.2/yandex_api_client/models/return_dto.py
+-rw-r--r--   0        0        0     3620 2024-04-09 12:18:55.000000 yandex_api_client-0.0.2/yandex_api_client/models/return_instance_dto.py
+-rw-r--r--   0        0        0     1661 2024-04-09 12:18:55.000000 yandex_api_client-0.0.2/yandex_api_client/models/return_instance_status_type.py
+-rw-r--r--   0        0        0     1653 2024-04-09 12:18:55.000000 yandex_api_client-0.0.2/yandex_api_client/models/return_instance_stock_type.py
+-rw-r--r--   0        0        0     6784 2024-04-09 12:18:55.000000 yandex_api_client-0.0.2/yandex_api_client/models/return_item_dto.py
+-rw-r--r--   0        0        0     1500 2024-04-09 12:18:55.000000 yandex_api_client-0.0.2/yandex_api_client/models/return_request_decision_type.py
+-rw-r--r--   0        0        0     2399 2024-04-09 12:18:55.000000 yandex_api_client-0.0.2/yandex_api_client/models/return_shipment_status_type.py
+-rw-r--r--   0        0        0     1430 2024-04-09 12:18:55.000000 yandex_api_client-0.0.2/yandex_api_client/models/return_type.py
+-rw-r--r--   0        0        0     3315 2024-04-09 12:18:55.000000 yandex_api_client-0.0.2/yandex_api_client/models/scrolling_pager_dto.py
+-rw-r--r--   0        0        0     4480 2024-04-09 12:18:55.000000 yandex_api_client-0.0.2/yandex_api_client/models/search_models_response.py
+-rw-r--r--   0        0        0     3924 2024-04-09 12:18:55.000000 yandex_api_client-0.0.2/yandex_api_client/models/search_shipments_request.py
+-rw-r--r--   0        0        0     3410 2024-04-09 12:18:55.000000 yandex_api_client-0.0.2/yandex_api_client/models/search_shipments_response.py
+-rw-r--r--   0        0        0     3909 2024-04-09 12:18:55.000000 yandex_api_client-0.0.2/yandex_api_client/models/search_shipments_response_dto.py
+-rw-r--r--   0        0        0     1366 2024-04-09 12:18:55.000000 yandex_api_client-0.0.2/yandex_api_client/models/selling_program_type.py
+-rw-r--r--   0        0        0     3118 2024-04-09 12:18:55.000000 yandex_api_client-0.0.2/yandex_api_client/models/send_message_to_chat_request.py
+-rw-r--r--   0        0        0     3514 2024-04-09 12:18:55.000000 yandex_api_client-0.0.2/yandex_api_client/models/set_feed_params_request.py
+-rw-r--r--   0        0        0     3782 2024-04-09 12:18:55.000000 yandex_api_client-0.0.2/yandex_api_client/models/set_order_box_layout_request.py
+-rw-r--r--   0        0        0     3339 2024-04-09 12:18:55.000000 yandex_api_client-0.0.2/yandex_api_client/models/set_order_box_layout_response.py
+-rw-r--r--   0        0        0     3317 2024-04-09 12:18:55.000000 yandex_api_client-0.0.2/yandex_api_client/models/set_order_delivery_date_request.py
+-rw-r--r--   0        0        0     3385 2024-04-09 12:18:55.000000 yandex_api_client-0.0.2/yandex_api_client/models/set_order_delivery_track_code_request.py
+-rw-r--r--   0        0        0     3534 2024-04-09 12:18:55.000000 yandex_api_client-0.0.2/yandex_api_client/models/set_order_shipment_boxes_request.py
+-rw-r--r--   0        0        0     3342 2024-04-09 12:18:55.000000 yandex_api_client-0.0.2/yandex_api_client/models/set_order_shipment_boxes_response.py
+-rw-r--r--   0        0        0     3812 2024-04-09 12:18:55.000000 yandex_api_client-0.0.2/yandex_api_client/models/set_return_decision_request.py
+-rw-r--r--   0        0        0     3106 2024-04-09 12:18:55.000000 yandex_api_client-0.0.2/yandex_api_client/models/set_shipment_pallets_count_request.py
+-rw-r--r--   0        0        0     1829 2024-04-09 12:18:55.000000 yandex_api_client-0.0.2/yandex_api_client/models/shipment_action_type.py
+-rw-r--r--   0        0        0     3614 2024-04-09 12:18:55.000000 yandex_api_client-0.0.2/yandex_api_client/models/shipment_boxes_dto.py
+-rw-r--r--   0        0        0     6683 2024-04-09 12:18:55.000000 yandex_api_client-0.0.2/yandex_api_client/models/shipment_dto.py
+-rw-r--r--   0        0        0     5781 2024-04-09 12:18:55.000000 yandex_api_client-0.0.2/yandex_api_client/models/shipment_info_dto.py
+-rw-r--r--   0        0        0     1352 2024-04-09 12:18:55.000000 yandex_api_client-0.0.2/yandex_api_client/models/shipment_pallet_label_page_format_type.py
+-rw-r--r--   0        0        0     3410 2024-04-09 12:18:55.000000 yandex_api_client-0.0.2/yandex_api_client/models/shipment_status_change_dto.py
+-rw-r--r--   0        0        0     2153 2024-04-09 12:18:55.000000 yandex_api_client-0.0.2/yandex_api_client/models/shipment_status_type.py
+-rw-r--r--   0        0        0     1577 2024-04-09 12:18:55.000000 yandex_api_client-0.0.2/yandex_api_client/models/shipment_type.py
+-rw-r--r--   0        0        0     1448 2024-04-09 12:18:55.000000 yandex_api_client-0.0.2/yandex_api_client/models/shows_sales_grouping_type.py
+-rw-r--r--   0        0        0     4534 2024-04-09 12:18:55.000000 yandex_api_client-0.0.2/yandex_api_client/models/sku_bid_item_dto.py
+-rw-r--r--   0        0        0     6469 2024-04-09 12:18:55.000000 yandex_api_client-0.0.2/yandex_api_client/models/sku_bid_recommendation_item_dto.py
+-rw-r--r--   0        0        0     1399 2024-04-09 12:18:55.000000 yandex_api_client-0.0.2/yandex_api_client/models/sort_order_type.py
+-rw-r--r--   0        0        0     4773 2024-04-09 12:18:55.000000 yandex_api_client-0.0.2/yandex_api_client/models/suggest_offer_price_dto.py
+-rw-r--r--   0        0        0     3498 2024-04-09 12:18:55.000000 yandex_api_client-0.0.2/yandex_api_client/models/suggest_prices_request.py
+-rw-r--r--   0        0        0     3393 2024-04-09 12:18:55.000000 yandex_api_client-0.0.2/yandex_api_client/models/suggest_prices_response.py
+-rw-r--r--   0        0        0     3493 2024-04-09 12:18:55.000000 yandex_api_client-0.0.2/yandex_api_client/models/suggest_prices_result_dto.py
+-rw-r--r--   0        0        0     9763 2024-04-09 12:18:55.000000 yandex_api_client-0.0.2/yandex_api_client/models/suggested_offer_dto.py
+-rw-r--r--   0        0        0     3590 2024-04-09 12:18:55.000000 yandex_api_client-0.0.2/yandex_api_client/models/suggested_offer_mapping_dto.py
+-rw-r--r--   0        0        0     4188 2024-04-09 12:18:55.000000 yandex_api_client-0.0.2/yandex_api_client/models/tariff_dto.py
+-rw-r--r--   0        0        0     3051 2024-04-09 12:18:55.000000 yandex_api_client-0.0.2/yandex_api_client/models/tariff_parameter_dto.py
+-rw-r--r--   0        0        0     4820 2024-04-09 12:18:55.000000 yandex_api_client-0.0.2/yandex_api_client/models/tariff_type.py
+-rw-r--r--   0        0        0     3561 2024-04-09 12:18:55.000000 yandex_api_client-0.0.2/yandex_api_client/models/time_period_dto.py
+-rw-r--r--   0        0        0     1421 2024-04-09 12:18:55.000000 yandex_api_client-0.0.2/yandex_api_client/models/time_unit_type.py
+-rw-r--r--   0        0        0     2959 2024-04-09 12:18:55.000000 yandex_api_client-0.0.2/yandex_api_client/models/track_dto.py
+-rw-r--r--   0        0        0     3146 2024-04-09 12:18:55.000000 yandex_api_client-0.0.2/yandex_api_client/models/transfer_orders_from_shipment_request.py
+-rw-r--r--   0        0        0     3260 2024-04-09 12:18:55.000000 yandex_api_client-0.0.2/yandex_api_client/models/turnover_dto.py
+-rw-r--r--   0        0        0     1770 2024-04-09 12:18:55.000000 yandex_api_client-0.0.2/yandex_api_client/models/turnover_type.py
+-rw-r--r--   0        0        0     3225 2024-04-09 12:18:55.000000 yandex_api_client-0.0.2/yandex_api_client/models/unit_dto.py
+-rw-r--r--   0        0        0     4863 2024-04-09 12:18:55.000000 yandex_api_client-0.0.2/yandex_api_client/models/update_business_offer_price_dto.py
+-rw-r--r--   0        0        0     3571 2024-04-09 12:18:55.000000 yandex_api_client-0.0.2/yandex_api_client/models/update_business_prices_request.py
+-rw-r--r--   0        0        0     5520 2024-04-09 12:18:55.000000 yandex_api_client-0.0.2/yandex_api_client/models/update_campaign_offer_dto.py
+-rw-r--r--   0        0        0     3611 2024-04-09 12:18:55.000000 yandex_api_client-0.0.2/yandex_api_client/models/update_campaign_offers_request.py
+-rw-r--r--   0        0        0     3423 2024-04-09 12:18:55.000000 yandex_api_client-0.0.2/yandex_api_client/models/update_mapping_dto.py
+-rw-r--r--   0        0        0    22156 2024-04-09 12:18:55.000000 yandex_api_client-0.0.2/yandex_api_client/models/update_mappings_offer_dto.py
+-rw-r--r--   0        0        0     3658 2024-04-09 12:18:55.000000 yandex_api_client-0.0.2/yandex_api_client/models/update_offer_content_request.py
+-rw-r--r--   0        0        0     3978 2024-04-09 12:18:55.000000 yandex_api_client-0.0.2/yandex_api_client/models/update_offer_content_response.py
+-rw-r--r--   0        0        0     5928 2024-04-09 12:18:55.000000 yandex_api_client-0.0.2/yandex_api_client/models/update_offer_content_result_dto.py
+-rw-r--r--   0        0        0    22344 2024-04-09 12:18:55.000000 yandex_api_client-0.0.2/yandex_api_client/models/update_offer_dto.py
+-rw-r--r--   0        0        0     3517 2024-04-09 12:18:55.000000 yandex_api_client-0.0.2/yandex_api_client/models/update_offer_mapping_dto.py
+-rw-r--r--   0        0        0     4748 2024-04-09 12:18:55.000000 yandex_api_client-0.0.2/yandex_api_client/models/update_offer_mapping_entry_dto.py
+-rw-r--r--   0        0        0     3718 2024-04-09 12:18:55.000000 yandex_api_client-0.0.2/yandex_api_client/models/update_offer_mapping_entry_request.py
+-rw-r--r--   0        0        0     3634 2024-04-09 12:18:55.000000 yandex_api_client-0.0.2/yandex_api_client/models/update_offer_mappings_request.py
+-rw-r--r--   0        0        0     3893 2024-04-09 12:18:55.000000 yandex_api_client-0.0.2/yandex_api_client/models/update_order_item_request.py
+-rw-r--r--   0        0        0     3963 2024-04-09 12:18:55.000000 yandex_api_client-0.0.2/yandex_api_client/models/update_order_status_dto.py
+-rw-r--r--   0        0        0     3117 2024-04-09 12:18:55.000000 yandex_api_client-0.0.2/yandex_api_client/models/update_order_status_request.py
+-rw-r--r--   0        0        0     3146 2024-04-09 12:18:55.000000 yandex_api_client-0.0.2/yandex_api_client/models/update_order_status_response.py
+-rw-r--r--   0        0        0     3482 2024-04-09 12:18:55.000000 yandex_api_client-0.0.2/yandex_api_client/models/update_order_statuses_dto.py
+-rw-r--r--   0        0        0     3440 2024-04-09 12:18:55.000000 yandex_api_client-0.0.2/yandex_api_client/models/update_order_statuses_request.py
+-rw-r--r--   0        0        0     3359 2024-04-09 12:18:55.000000 yandex_api_client-0.0.2/yandex_api_client/models/update_order_statuses_response.py
+-rw-r--r--   0        0        0     3233 2024-04-09 12:18:55.000000 yandex_api_client-0.0.2/yandex_api_client/models/update_order_storage_limit_request.py
+-rw-r--r--   0        0        0     3683 2024-04-09 12:18:55.000000 yandex_api_client-0.0.2/yandex_api_client/models/update_outlet_license_request.py
+-rw-r--r--   0        0        0     3783 2024-04-09 12:18:55.000000 yandex_api_client-0.0.2/yandex_api_client/models/update_price_with_discount_dto.py
+-rw-r--r--   0        0        0     3441 2024-04-09 12:18:55.000000 yandex_api_client-0.0.2/yandex_api_client/models/update_prices_request.py
+-rw-r--r--   0        0        0     5110 2024-04-09 12:18:55.000000 yandex_api_client-0.0.2/yandex_api_client/models/update_stock_dto.py
+-rw-r--r--   0        0        0     3588 2024-04-09 12:18:55.000000 yandex_api_client-0.0.2/yandex_api_client/models/update_stock_item_dto.py
+-rw-r--r--   0        0        0     3497 2024-04-09 12:18:55.000000 yandex_api_client-0.0.2/yandex_api_client/models/update_stocks_request.py
+-rw-r--r--   0        0        0     2957 2024-04-09 12:18:55.000000 yandex_api_client-0.0.2/yandex_api_client/models/update_time_dto.py
+-rw-r--r--   0        0        0     4744 2024-04-09 12:18:55.000000 yandex_api_client-0.0.2/yandex_api_client/models/value_restriction_dto.py
+-rw-r--r--   0        0        0     2923 2024-04-09 12:18:55.000000 yandex_api_client-0.0.2/yandex_api_client/models/verify_order_eac_request.py
+-rw-r--r--   0        0        0     3347 2024-04-09 12:18:55.000000 yandex_api_client-0.0.2/yandex_api_client/models/verify_order_eac_response.py
+-rw-r--r--   0        0        0     3979 2024-04-09 12:18:55.000000 yandex_api_client-0.0.2/yandex_api_client/models/warehouse_address_dto.py
+-rw-r--r--   0        0        0     3843 2024-04-09 12:18:55.000000 yandex_api_client-0.0.2/yandex_api_client/models/warehouse_dto.py
+-rw-r--r--   0        0        0     3962 2024-04-09 12:18:55.000000 yandex_api_client-0.0.2/yandex_api_client/models/warehouse_group_dto.py
+-rw-r--r--   0        0        0     6040 2024-04-09 12:18:55.000000 yandex_api_client-0.0.2/yandex_api_client/models/warehouse_offer_dto.py
+-rw-r--r--   0        0        0     3598 2024-04-09 12:18:55.000000 yandex_api_client-0.0.2/yandex_api_client/models/warehouse_offers_dto.py
+-rw-r--r--   0        0        0     3051 2024-04-09 12:18:55.000000 yandex_api_client-0.0.2/yandex_api_client/models/warehouse_stock_dto.py
+-rw-r--r--   0        0        0     2523 2024-04-09 12:18:55.000000 yandex_api_client-0.0.2/yandex_api_client/models/warehouse_stock_type.py
+-rw-r--r--   0        0        0     4215 2024-04-09 12:18:55.000000 yandex_api_client-0.0.2/yandex_api_client/models/warehouses_dto.py
+-rw-r--r--   0        0        0        0 2024-04-09 12:18:56.000000 yandex_api_client-0.0.2/yandex_api_client/py.typed
+-rw-r--r--   0        0        0    10188 2024-04-09 12:18:56.000000 yandex_api_client-0.0.2/yandex_api_client/rest.py
+-rw-r--r--   0        0        0   125216 1970-01-01 00:00:00.000000 yandex_api_client-0.0.2/PKG-INFO
```

### Comparing `yandex_api_client-0.0.1/README.md` & `yandex_api_client-0.0.2/README.md`

 * *Files identical despite different names*

### Comparing `yandex_api_client-0.0.1/pyproject.toml` & `yandex_api_client-0.0.2/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "yandex_api_client"
-version = "0.0.1"
+version = "0.0.2"
 description = ""
 authors = ["OpenAPI Generator Community <team@openapitools.org>"]
 license = "BSD 3-Clause"
 readme = "README.md"
 keywords = ["OpenAPI", "OpenAPI-Generator", "Партнерский API Маркета"]
 include = ["yandex_api_client/py.typed"]
```

### Comparing `yandex_api_client-0.0.1/yandex_api_client/__init__.py` & `yandex_api_client-0.0.2/yandex_api_client/__init__.py`

 * *Files identical despite different names*

### Comparing `yandex_api_client-0.0.1/yandex_api_client/api/__init__.py` & `yandex_api_client-0.0.2/yandex_api_client/api/__init__.py`

 * *Files identical despite different names*

### Comparing `yandex_api_client-0.0.1/yandex_api_client/api/bids_api.py` & `yandex_api_client-0.0.2/yandex_api_client/api/bids_api.py`

 * *Files identical despite different names*

### Comparing `yandex_api_client-0.0.1/yandex_api_client/api/business_offer_mappings_api.py` & `yandex_api_client-0.0.2/yandex_api_client/api/business_offer_mappings_api.py`

 * *Files identical despite different names*

### Comparing `yandex_api_client-0.0.1/yandex_api_client/api/campaigns_api.py` & `yandex_api_client-0.0.2/yandex_api_client/api/campaigns_api.py`

 * *Files identical despite different names*

### Comparing `yandex_api_client-0.0.1/yandex_api_client/api/categories_api.py` & `yandex_api_client-0.0.2/yandex_api_client/api/categories_api.py`

 * *Files identical despite different names*

### Comparing `yandex_api_client-0.0.1/yandex_api_client/api/chats_api.py` & `yandex_api_client-0.0.2/yandex_api_client/api/chats_api.py`

 * *Files identical despite different names*

### Comparing `yandex_api_client-0.0.1/yandex_api_client/api/content_api.py` & `yandex_api_client-0.0.2/yandex_api_client/api/content_api.py`

 * *Files identical despite different names*

### Comparing `yandex_api_client-0.0.1/yandex_api_client/api/dbs_api.py` & `yandex_api_client-0.0.2/yandex_api_client/api/dbs_api.py`

 * *Files identical despite different names*

### Comparing `yandex_api_client-0.0.1/yandex_api_client/api/delivery_services_api.py` & `yandex_api_client-0.0.2/yandex_api_client/api/delivery_services_api.py`

 * *Files identical despite different names*

### Comparing `yandex_api_client-0.0.1/yandex_api_client/api/express_api.py` & `yandex_api_client-0.0.2/yandex_api_client/api/express_api.py`

 * *Files identical despite different names*

### Comparing `yandex_api_client-0.0.1/yandex_api_client/api/fbs_api.py` & `yandex_api_client-0.0.2/yandex_api_client/api/fbs_api.py`

 * *Files identical despite different names*

### Comparing `yandex_api_client-0.0.1/yandex_api_client/api/fby_api.py` & `yandex_api_client-0.0.2/yandex_api_client/api/fby_api.py`

 * *Files identical despite different names*

### Comparing `yandex_api_client-0.0.1/yandex_api_client/api/feed_categories_api.py` & `yandex_api_client-0.0.2/yandex_api_client/api/feed_categories_api.py`

 * *Files identical despite different names*

### Comparing `yandex_api_client-0.0.1/yandex_api_client/api/feedbacks_api.py` & `yandex_api_client-0.0.2/yandex_api_client/api/feedbacks_api.py`

 * *Files identical despite different names*

### Comparing `yandex_api_client-0.0.1/yandex_api_client/api/feeds_api.py` & `yandex_api_client-0.0.2/yandex_api_client/api/feeds_api.py`

 * *Files identical despite different names*

### Comparing `yandex_api_client-0.0.1/yandex_api_client/api/goods_stats_api.py` & `yandex_api_client-0.0.2/yandex_api_client/api/goods_stats_api.py`

 * *Files identical despite different names*

### Comparing `yandex_api_client-0.0.1/yandex_api_client/api/hidden_offers_api.py` & `yandex_api_client-0.0.2/yandex_api_client/api/hidden_offers_api.py`

 * *Files identical despite different names*

### Comparing `yandex_api_client-0.0.1/yandex_api_client/api/models_api.py` & `yandex_api_client-0.0.2/yandex_api_client/api/models_api.py`

 * *Files identical despite different names*

### Comparing `yandex_api_client-0.0.1/yandex_api_client/api/offer_mappings_api.py` & `yandex_api_client-0.0.2/yandex_api_client/api/offer_mappings_api.py`

 * *Files identical despite different names*

### Comparing `yandex_api_client-0.0.1/yandex_api_client/api/offers_api.py` & `yandex_api_client-0.0.2/yandex_api_client/api/offers_api.py`

 * *Files identical despite different names*

### Comparing `yandex_api_client-0.0.1/yandex_api_client/api/order_business_information_api.py` & `yandex_api_client-0.0.2/yandex_api_client/api/order_business_information_api.py`

 * *Files identical despite different names*

### Comparing `yandex_api_client-0.0.1/yandex_api_client/api/order_delivery_api.py` & `yandex_api_client-0.0.2/yandex_api_client/api/order_delivery_api.py`

 * *Files identical despite different names*

### Comparing `yandex_api_client-0.0.1/yandex_api_client/api/order_labels_api.py` & `yandex_api_client-0.0.2/yandex_api_client/api/order_labels_api.py`

 * *Files identical despite different names*

### Comparing `yandex_api_client-0.0.1/yandex_api_client/api/orders_api.py` & `yandex_api_client-0.0.2/yandex_api_client/api/orders_api.py`

 * *Files identical despite different names*

### Comparing `yandex_api_client-0.0.1/yandex_api_client/api/orders_stats_api.py` & `yandex_api_client-0.0.2/yandex_api_client/api/orders_stats_api.py`

 * *Files identical despite different names*

### Comparing `yandex_api_client-0.0.1/yandex_api_client/api/outlet_licenses_api.py` & `yandex_api_client-0.0.2/yandex_api_client/api/outlet_licenses_api.py`

 * *Files identical despite different names*

### Comparing `yandex_api_client-0.0.1/yandex_api_client/api/outlets_api.py` & `yandex_api_client-0.0.2/yandex_api_client/api/outlets_api.py`

 * *Files identical despite different names*

### Comparing `yandex_api_client-0.0.1/yandex_api_client/api/price_quarantine_api.py` & `yandex_api_client-0.0.2/yandex_api_client/api/price_quarantine_api.py`

 * *Files identical despite different names*

### Comparing `yandex_api_client-0.0.1/yandex_api_client/api/prices_api.py` & `yandex_api_client-0.0.2/yandex_api_client/api/prices_api.py`

 * *Files identical despite different names*

### Comparing `yandex_api_client-0.0.1/yandex_api_client/api/regions_api.py` & `yandex_api_client-0.0.2/yandex_api_client/api/regions_api.py`

 * *Files identical despite different names*

### Comparing `yandex_api_client-0.0.1/yandex_api_client/api/reports_api.py` & `yandex_api_client-0.0.2/yandex_api_client/api/reports_api.py`

 * *Files identical despite different names*

### Comparing `yandex_api_client-0.0.1/yandex_api_client/api/returns_api.py` & `yandex_api_client-0.0.2/yandex_api_client/api/returns_api.py`

 * *Files identical despite different names*

### Comparing `yandex_api_client-0.0.1/yandex_api_client/api/shipments_api.py` & `yandex_api_client-0.0.2/yandex_api_client/api/shipments_api.py`

 * *Files identical despite different names*

### Comparing `yandex_api_client-0.0.1/yandex_api_client/api/stocks_api.py` & `yandex_api_client-0.0.2/yandex_api_client/api/stocks_api.py`

 * *Files identical despite different names*

### Comparing `yandex_api_client-0.0.1/yandex_api_client/api/tariffs_api.py` & `yandex_api_client-0.0.2/yandex_api_client/api/tariffs_api.py`

 * *Files identical despite different names*

### Comparing `yandex_api_client-0.0.1/yandex_api_client/api/warehouses_api.py` & `yandex_api_client-0.0.2/yandex_api_client/api/warehouses_api.py`

 * *Files identical despite different names*

### Comparing `yandex_api_client-0.0.1/yandex_api_client/api_client.py` & `yandex_api_client-0.0.2/yandex_api_client/api_client.py`

 * *Files identical despite different names*

### Comparing `yandex_api_client-0.0.1/yandex_api_client/api_response.py` & `yandex_api_client-0.0.2/yandex_api_client/api_response.py`

 * *Files identical despite different names*

### Comparing `yandex_api_client-0.0.1/yandex_api_client/configuration.py` & `yandex_api_client-0.0.2/yandex_api_client/configuration.py`

 * *Files identical despite different names*

### Comparing `yandex_api_client-0.0.1/yandex_api_client/exceptions.py` & `yandex_api_client-0.0.2/yandex_api_client/exceptions.py`

 * *Files identical despite different names*

### Comparing `yandex_api_client-0.0.1/yandex_api_client/models/__init__.py` & `yandex_api_client-0.0.2/yandex_api_client/models/__init__.py`

 * *Files identical despite different names*

### Comparing `yandex_api_client-0.0.1/yandex_api_client/models/accept_order_cancellation_request.py` & `yandex_api_client-0.0.2/yandex_api_client/models/accept_order_cancellation_request.py`

 * *Files identical despite different names*

### Comparing `yandex_api_client-0.0.1/yandex_api_client/models/add_hidden_offers_request.py` & `yandex_api_client-0.0.2/yandex_api_client/models/add_hidden_offers_request.py`

 * *Files identical despite different names*

### Comparing `yandex_api_client-0.0.1/yandex_api_client/models/add_offers_to_archive_dto.py` & `yandex_api_client-0.0.2/yandex_api_client/models/add_offers_to_archive_dto.py`

 * *Files identical despite different names*

### Comparing `yandex_api_client-0.0.1/yandex_api_client/models/add_offers_to_archive_error_dto.py` & `yandex_api_client-0.0.2/yandex_api_client/models/add_offers_to_archive_error_dto.py`

 * *Files identical despite different names*

### Comparing `yandex_api_client-0.0.1/yandex_api_client/models/add_offers_to_archive_error_type.py` & `yandex_api_client-0.0.2/yandex_api_client/models/add_offers_to_archive_error_type.py`

 * *Files identical despite different names*

### Comparing `yandex_api_client-0.0.1/yandex_api_client/models/add_offers_to_archive_request.py` & `yandex_api_client-0.0.2/yandex_api_client/models/add_offers_to_archive_request.py`

 * *Files identical despite different names*

### Comparing `yandex_api_client-0.0.1/yandex_api_client/models/add_offers_to_archive_response.py` & `yandex_api_client-0.0.2/yandex_api_client/models/add_offers_to_archive_response.py`

 * *Files identical despite different names*

### Comparing `yandex_api_client-0.0.1/yandex_api_client/models/age_dto.py` & `yandex_api_client-0.0.2/yandex_api_client/models/age_dto.py`

 * *Files identical despite different names*

### Comparing `yandex_api_client-0.0.1/yandex_api_client/models/age_unit_type.py` & `yandex_api_client-0.0.2/yandex_api_client/models/age_unit_type.py`

 * *Files identical despite different names*

### Comparing `yandex_api_client-0.0.1/yandex_api_client/models/api_client_data_error_response.py` & `yandex_api_client-0.0.2/yandex_api_client/models/api_client_data_error_response.py`

 * *Files identical despite different names*

### Comparing `yandex_api_client-0.0.1/yandex_api_client/models/api_error_dto.py` & `yandex_api_client-0.0.2/yandex_api_client/models/api_error_dto.py`

 * *Files identical despite different names*

### Comparing `yandex_api_client-0.0.1/yandex_api_client/models/api_error_response.py` & `yandex_api_client-0.0.2/yandex_api_client/models/api_error_response.py`

 * *Files identical despite different names*

### Comparing `yandex_api_client-0.0.1/yandex_api_client/models/api_forbidden_error_response.py` & `yandex_api_client-0.0.2/yandex_api_client/models/api_forbidden_error_response.py`

 * *Files identical despite different names*

### Comparing `yandex_api_client-0.0.1/yandex_api_client/models/api_limit_error_response.py` & `yandex_api_client-0.0.2/yandex_api_client/models/api_limit_error_response.py`

 * *Files identical despite different names*

### Comparing `yandex_api_client-0.0.1/yandex_api_client/models/api_locked_error_response.py` & `yandex_api_client-0.0.2/yandex_api_client/models/api_locked_error_response.py`

 * *Files identical despite different names*

### Comparing `yandex_api_client-0.0.1/yandex_api_client/models/api_not_found_error_response.py` & `yandex_api_client-0.0.2/yandex_api_client/models/api_not_found_error_response.py`

 * *Files identical despite different names*

### Comparing `yandex_api_client-0.0.1/yandex_api_client/models/api_response.py` & `yandex_api_client-0.0.2/yandex_api_client/models/api_response.py`

 * *Files identical despite different names*

### Comparing `yandex_api_client-0.0.1/yandex_api_client/models/api_response_status_type.py` & `yandex_api_client-0.0.2/yandex_api_client/models/api_response_status_type.py`

 * *Files identical despite different names*

### Comparing `yandex_api_client-0.0.1/yandex_api_client/models/api_server_error_response.py` & `yandex_api_client-0.0.2/yandex_api_client/models/api_server_error_response.py`

 * *Files identical despite different names*

### Comparing `yandex_api_client-0.0.1/yandex_api_client/models/api_unauthorized_error_response.py` & `yandex_api_client-0.0.2/yandex_api_client/models/api_unauthorized_error_response.py`

 * *Files identical despite different names*

### Comparing `yandex_api_client-0.0.1/yandex_api_client/models/base_campaign_offer_dto.py` & `yandex_api_client-0.0.2/yandex_api_client/models/base_campaign_offer_dto.py`

 * *Files identical despite different names*

### Comparing `yandex_api_client-0.0.1/yandex_api_client/models/base_offer_dto.py` & `yandex_api_client-0.0.2/yandex_api_client/models/base_offer_dto.py`

 * *Files identical despite different names*

### Comparing `yandex_api_client-0.0.1/yandex_api_client/models/base_price_dto.py` & `yandex_api_client-0.0.2/yandex_api_client/models/base_price_dto.py`

 * *Files identical despite different names*

### Comparing `yandex_api_client-0.0.1/yandex_api_client/models/bid_recommendation_item_dto.py` & `yandex_api_client-0.0.2/yandex_api_client/models/bid_recommendation_item_dto.py`

 * *Files identical despite different names*

### Comparing `yandex_api_client-0.0.1/yandex_api_client/models/brief_order_item_dto.py` & `yandex_api_client-0.0.2/yandex_api_client/models/brief_order_item_dto.py`

 * *Files identical despite different names*

### Comparing `yandex_api_client-0.0.1/yandex_api_client/models/brief_order_item_instance_dto.py` & `yandex_api_client-0.0.2/yandex_api_client/models/brief_order_item_instance_dto.py`

 * *Files identical despite different names*

### Comparing `yandex_api_client-0.0.1/yandex_api_client/models/business_dto.py` & `yandex_api_client-0.0.2/yandex_api_client/models/business_dto.py`

 * *Files identical despite different names*

### Comparing `yandex_api_client-0.0.1/yandex_api_client/models/calculate_tariffs_offer_dto.py` & `yandex_api_client-0.0.2/yandex_api_client/models/calculate_tariffs_offer_dto.py`

 * *Files identical despite different names*

### Comparing `yandex_api_client-0.0.1/yandex_api_client/models/calculate_tariffs_offer_info_dto.py` & `yandex_api_client-0.0.2/yandex_api_client/models/calculate_tariffs_offer_info_dto.py`

 * *Files identical despite different names*

### Comparing `yandex_api_client-0.0.1/yandex_api_client/models/calculate_tariffs_parameters_dto.py` & `yandex_api_client-0.0.2/yandex_api_client/models/calculate_tariffs_parameters_dto.py`

 * *Files identical despite different names*

### Comparing `yandex_api_client-0.0.1/yandex_api_client/models/calculate_tariffs_request.py` & `yandex_api_client-0.0.2/yandex_api_client/models/calculate_tariffs_request.py`

 * *Files identical despite different names*

### Comparing `yandex_api_client-0.0.1/yandex_api_client/models/calculate_tariffs_response.py` & `yandex_api_client-0.0.2/yandex_api_client/models/calculate_tariffs_response.py`

 * *Files identical despite different names*

### Comparing `yandex_api_client-0.0.1/yandex_api_client/models/calculate_tariffs_response_dto.py` & `yandex_api_client-0.0.2/yandex_api_client/models/calculate_tariffs_response_dto.py`

 * *Files identical despite different names*

### Comparing `yandex_api_client-0.0.1/yandex_api_client/models/calculated_tariff_dto.py` & `yandex_api_client-0.0.2/yandex_api_client/models/calculated_tariff_dto.py`

 * *Files identical despite different names*

### Comparing `yandex_api_client-0.0.1/yandex_api_client/models/calculated_tariff_type.py` & `yandex_api_client-0.0.2/yandex_api_client/models/calculated_tariff_type.py`

 * *Files identical despite different names*

### Comparing `yandex_api_client-0.0.1/yandex_api_client/models/campaign_dto.py` & `yandex_api_client-0.0.2/yandex_api_client/models/campaign_dto.py`

 * *Files identical despite different names*

### Comparing `yandex_api_client-0.0.1/yandex_api_client/models/campaign_settings_delivery_dto.py` & `yandex_api_client-0.0.2/yandex_api_client/models/campaign_settings_delivery_dto.py`

 * *Files identical despite different names*

### Comparing `yandex_api_client-0.0.1/yandex_api_client/models/campaign_settings_dto.py` & `yandex_api_client-0.0.2/yandex_api_client/models/campaign_settings_dto.py`

 * *Files identical despite different names*

### Comparing `yandex_api_client-0.0.1/yandex_api_client/models/campaign_settings_local_region_dto.py` & `yandex_api_client-0.0.2/yandex_api_client/models/campaign_settings_local_region_dto.py`

 * *Files identical despite different names*

### Comparing `yandex_api_client-0.0.1/yandex_api_client/models/campaign_settings_schedule_dto.py` & `yandex_api_client-0.0.2/yandex_api_client/models/campaign_settings_schedule_dto.py`

 * *Files identical despite different names*

### Comparing `yandex_api_client-0.0.1/yandex_api_client/models/campaign_settings_schedule_source_type.py` & `yandex_api_client-0.0.2/yandex_api_client/models/campaign_settings_schedule_source_type.py`

 * *Files identical despite different names*

### Comparing `yandex_api_client-0.0.1/yandex_api_client/models/campaign_settings_time_period_dto.py` & `yandex_api_client-0.0.2/yandex_api_client/models/campaign_settings_time_period_dto.py`

 * *Files identical despite different names*

### Comparing `yandex_api_client-0.0.1/yandex_api_client/models/category_content_parameters_dto.py` & `yandex_api_client-0.0.2/yandex_api_client/models/category_content_parameters_dto.py`

 * *Files identical despite different names*

### Comparing `yandex_api_client-0.0.1/yandex_api_client/models/category_dto.py` & `yandex_api_client-0.0.2/yandex_api_client/models/category_dto.py`

 * *Files identical despite different names*

### Comparing `yandex_api_client-0.0.1/yandex_api_client/models/category_parameter_dto.py` & `yandex_api_client-0.0.2/yandex_api_client/models/category_parameter_dto.py`

 * *Files identical despite different names*

### Comparing `yandex_api_client-0.0.1/yandex_api_client/models/category_parameter_unit_dto.py` & `yandex_api_client-0.0.2/yandex_api_client/models/category_parameter_unit_dto.py`

 * *Files identical despite different names*

### Comparing `yandex_api_client-0.0.1/yandex_api_client/models/change_outlet_request.py` & `yandex_api_client-0.0.2/yandex_api_client/models/change_outlet_request.py`

 * *Files identical despite different names*

### Comparing `yandex_api_client-0.0.1/yandex_api_client/models/chat_message_dto.py` & `yandex_api_client-0.0.2/yandex_api_client/models/chat_message_dto.py`

 * *Files identical despite different names*

### Comparing `yandex_api_client-0.0.1/yandex_api_client/models/chat_message_payload_dto.py` & `yandex_api_client-0.0.2/yandex_api_client/models/chat_message_payload_dto.py`

 * *Files identical despite different names*

### Comparing `yandex_api_client-0.0.1/yandex_api_client/models/chat_message_sender_type.py` & `yandex_api_client-0.0.2/yandex_api_client/models/chat_message_sender_type.py`

 * *Files identical despite different names*

### Comparing `yandex_api_client-0.0.1/yandex_api_client/models/chat_messages_result_dto.py` & `yandex_api_client-0.0.2/yandex_api_client/models/chat_messages_result_dto.py`

 * *Files identical despite different names*

### Comparing `yandex_api_client-0.0.1/yandex_api_client/models/chat_status_type.py` & `yandex_api_client-0.0.2/yandex_api_client/models/chat_status_type.py`

 * *Files identical despite different names*

### Comparing `yandex_api_client-0.0.1/yandex_api_client/models/chat_type.py` & `yandex_api_client-0.0.2/yandex_api_client/models/chat_type.py`

 * *Files identical despite different names*

### Comparing `yandex_api_client-0.0.1/yandex_api_client/models/confirm_prices_request.py` & `yandex_api_client-0.0.2/yandex_api_client/models/confirm_prices_request.py`

 * *Files identical despite different names*

### Comparing `yandex_api_client-0.0.1/yandex_api_client/models/confirm_shipment_request.py` & `yandex_api_client-0.0.2/yandex_api_client/models/confirm_shipment_request.py`

 * *Files identical despite different names*

### Comparing `yandex_api_client-0.0.1/yandex_api_client/models/create_chat_request.py` & `yandex_api_client-0.0.2/yandex_api_client/models/create_chat_request.py`

 * *Files identical despite different names*

### Comparing `yandex_api_client-0.0.1/yandex_api_client/models/create_chat_response.py` & `yandex_api_client-0.0.2/yandex_api_client/models/create_chat_response.py`

 * *Files identical despite different names*

### Comparing `yandex_api_client-0.0.1/yandex_api_client/models/create_chat_result_dto.py` & `yandex_api_client-0.0.2/yandex_api_client/models/create_chat_result_dto.py`

 * *Files identical despite different names*

### Comparing `yandex_api_client-0.0.1/yandex_api_client/models/create_outlet_response.py` & `yandex_api_client-0.0.2/yandex_api_client/models/create_outlet_response.py`

 * *Files identical despite different names*

### Comparing `yandex_api_client-0.0.1/yandex_api_client/models/currency_type.py` & `yandex_api_client-0.0.2/yandex_api_client/models/currency_type.py`

 * *Files identical despite different names*

### Comparing `yandex_api_client-0.0.1/yandex_api_client/models/day_of_week_type.py` & `yandex_api_client-0.0.2/yandex_api_client/models/day_of_week_type.py`

 * *Files identical despite different names*

### Comparing `yandex_api_client-0.0.1/yandex_api_client/models/delete_campaign_offers_dto.py` & `yandex_api_client-0.0.2/yandex_api_client/models/delete_campaign_offers_dto.py`

 * *Files identical despite different names*

### Comparing `yandex_api_client-0.0.1/yandex_api_client/models/delete_campaign_offers_request.py` & `yandex_api_client-0.0.2/yandex_api_client/models/delete_campaign_offers_request.py`

 * *Files identical despite different names*

### Comparing `yandex_api_client-0.0.1/yandex_api_client/models/delete_campaign_offers_response.py` & `yandex_api_client-0.0.2/yandex_api_client/models/delete_campaign_offers_response.py`

 * *Files identical despite different names*

### Comparing `yandex_api_client-0.0.1/yandex_api_client/models/delete_hidden_offers_request.py` & `yandex_api_client-0.0.2/yandex_api_client/models/delete_hidden_offers_request.py`

 * *Files identical despite different names*

### Comparing `yandex_api_client-0.0.1/yandex_api_client/models/delete_offers_dto.py` & `yandex_api_client-0.0.2/yandex_api_client/models/delete_offers_dto.py`

 * *Files identical despite different names*

### Comparing `yandex_api_client-0.0.1/yandex_api_client/models/delete_offers_from_archive_dto.py` & `yandex_api_client-0.0.2/yandex_api_client/models/delete_offers_from_archive_dto.py`

 * *Files identical despite different names*

### Comparing `yandex_api_client-0.0.1/yandex_api_client/models/delete_offers_from_archive_request.py` & `yandex_api_client-0.0.2/yandex_api_client/models/delete_offers_from_archive_request.py`

 * *Files identical despite different names*

### Comparing `yandex_api_client-0.0.1/yandex_api_client/models/delete_offers_from_archive_response.py` & `yandex_api_client-0.0.2/yandex_api_client/models/delete_offers_from_archive_response.py`

 * *Files identical despite different names*

### Comparing `yandex_api_client-0.0.1/yandex_api_client/models/delete_offers_request.py` & `yandex_api_client-0.0.2/yandex_api_client/models/delete_offers_request.py`

 * *Files identical despite different names*

### Comparing `yandex_api_client-0.0.1/yandex_api_client/models/delete_offers_response.py` & `yandex_api_client-0.0.2/yandex_api_client/models/delete_offers_response.py`

 * *Files identical despite different names*

### Comparing `yandex_api_client-0.0.1/yandex_api_client/models/delivery_service_dto.py` & `yandex_api_client-0.0.2/yandex_api_client/models/delivery_service_dto.py`

 * *Files identical despite different names*

### Comparing `yandex_api_client-0.0.1/yandex_api_client/models/delivery_service_info_dto.py` & `yandex_api_client-0.0.2/yandex_api_client/models/delivery_service_info_dto.py`

 * *Files identical despite different names*

### Comparing `yandex_api_client-0.0.1/yandex_api_client/models/delivery_services_dto.py` & `yandex_api_client-0.0.2/yandex_api_client/models/delivery_services_dto.py`

 * *Files identical despite different names*

### Comparing `yandex_api_client-0.0.1/yandex_api_client/models/document_dto.py` & `yandex_api_client-0.0.2/yandex_api_client/models/document_dto.py`

 * *Files identical despite different names*

### Comparing `yandex_api_client-0.0.1/yandex_api_client/models/eac_verification_result_dto.py` & `yandex_api_client-0.0.2/yandex_api_client/models/eac_verification_result_dto.py`

 * *Files identical despite different names*

### Comparing `yandex_api_client-0.0.1/yandex_api_client/models/eac_verification_status_type.py` & `yandex_api_client-0.0.2/yandex_api_client/models/eac_verification_status_type.py`

 * *Files identical despite different names*

### Comparing `yandex_api_client-0.0.1/yandex_api_client/models/empty_api_response.py` & `yandex_api_client-0.0.2/yandex_api_client/models/empty_api_response.py`

 * *Files identical despite different names*

### Comparing `yandex_api_client-0.0.1/yandex_api_client/models/enriched_mappings_offer_dto.py` & `yandex_api_client-0.0.2/yandex_api_client/models/enriched_mappings_offer_dto.py`

 * *Files identical despite different names*

### Comparing `yandex_api_client-0.0.1/yandex_api_client/models/enriched_model_dto.py` & `yandex_api_client-0.0.2/yandex_api_client/models/enriched_model_dto.py`

 * *Files identical despite different names*

### Comparing `yandex_api_client-0.0.1/yandex_api_client/models/enriched_order_box_layout_dto.py` & `yandex_api_client-0.0.2/yandex_api_client/models/enriched_order_box_layout_dto.py`

 * *Files identical despite different names*

### Comparing `yandex_api_client-0.0.1/yandex_api_client/models/feed_category_dto.py` & `yandex_api_client-0.0.2/yandex_api_client/models/feed_category_dto.py`

 * *Files identical despite different names*

### Comparing `yandex_api_client-0.0.1/yandex_api_client/models/feed_content_dto.py` & `yandex_api_client-0.0.2/yandex_api_client/models/feed_content_dto.py`

 * *Files identical despite different names*

### Comparing `yandex_api_client-0.0.1/yandex_api_client/models/feed_content_error_dto.py` & `yandex_api_client-0.0.2/yandex_api_client/models/feed_content_error_dto.py`

 * *Files identical despite different names*

### Comparing `yandex_api_client-0.0.1/yandex_api_client/models/feed_content_error_type.py` & `yandex_api_client-0.0.2/yandex_api_client/models/feed_content_error_type.py`

 * *Files identical despite different names*

### Comparing `yandex_api_client-0.0.1/yandex_api_client/models/feed_download_dto.py` & `yandex_api_client-0.0.2/yandex_api_client/models/feed_download_dto.py`

 * *Files identical despite different names*

### Comparing `yandex_api_client-0.0.1/yandex_api_client/models/feed_download_error_dto.py` & `yandex_api_client-0.0.2/yandex_api_client/models/feed_download_error_dto.py`

 * *Files identical despite different names*

### Comparing `yandex_api_client-0.0.1/yandex_api_client/models/feed_download_error_type.py` & `yandex_api_client-0.0.2/yandex_api_client/models/feed_download_error_type.py`

 * *Files identical despite different names*

### Comparing `yandex_api_client-0.0.1/yandex_api_client/models/feed_dto.py` & `yandex_api_client-0.0.2/yandex_api_client/models/feed_dto.py`

 * *Files identical despite different names*

### Comparing `yandex_api_client-0.0.1/yandex_api_client/models/feed_index_logs_error_dto.py` & `yandex_api_client-0.0.2/yandex_api_client/models/feed_index_logs_error_dto.py`

 * *Files identical despite different names*

### Comparing `yandex_api_client-0.0.1/yandex_api_client/models/feed_index_logs_error_type.py` & `yandex_api_client-0.0.2/yandex_api_client/models/feed_index_logs_error_type.py`

 * *Files identical despite different names*

### Comparing `yandex_api_client-0.0.1/yandex_api_client/models/feed_index_logs_feed_dto.py` & `yandex_api_client-0.0.2/yandex_api_client/models/feed_index_logs_feed_dto.py`

 * *Files identical despite different names*

### Comparing `yandex_api_client-0.0.1/yandex_api_client/models/feed_index_logs_index_type.py` & `yandex_api_client-0.0.2/yandex_api_client/models/feed_index_logs_index_type.py`

 * *Files identical despite different names*

### Comparing `yandex_api_client-0.0.1/yandex_api_client/models/feed_index_logs_offers_dto.py` & `yandex_api_client-0.0.2/yandex_api_client/models/feed_index_logs_offers_dto.py`

 * *Files identical despite different names*

### Comparing `yandex_api_client-0.0.1/yandex_api_client/models/feed_index_logs_record_dto.py` & `yandex_api_client-0.0.2/yandex_api_client/models/feed_index_logs_record_dto.py`

 * *Files identical despite different names*

### Comparing `yandex_api_client-0.0.1/yandex_api_client/models/feed_index_logs_result_dto.py` & `yandex_api_client-0.0.2/yandex_api_client/models/feed_index_logs_result_dto.py`

 * *Files identical despite different names*

### Comparing `yandex_api_client-0.0.1/yandex_api_client/models/feed_index_logs_status_type.py` & `yandex_api_client-0.0.2/yandex_api_client/models/feed_index_logs_status_type.py`

 * *Files identical despite different names*

### Comparing `yandex_api_client-0.0.1/yandex_api_client/models/feed_parameter_dto.py` & `yandex_api_client-0.0.2/yandex_api_client/models/feed_parameter_dto.py`

 * *Files identical despite different names*

### Comparing `yandex_api_client-0.0.1/yandex_api_client/models/feed_placement_dto.py` & `yandex_api_client-0.0.2/yandex_api_client/models/feed_placement_dto.py`

 * *Files identical despite different names*

### Comparing `yandex_api_client-0.0.1/yandex_api_client/models/feed_publication_dto.py` & `yandex_api_client-0.0.2/yandex_api_client/models/feed_publication_dto.py`

 * *Files identical despite different names*

### Comparing `yandex_api_client-0.0.1/yandex_api_client/models/feed_publication_full_dto.py` & `yandex_api_client-0.0.2/yandex_api_client/models/feed_publication_full_dto.py`

 * *Files identical despite different names*

### Comparing `yandex_api_client-0.0.1/yandex_api_client/models/feed_publication_price_and_stock_update_dto.py` & `yandex_api_client-0.0.2/yandex_api_client/models/feed_publication_price_and_stock_update_dto.py`

 * *Files identical despite different names*

### Comparing `yandex_api_client-0.0.1/yandex_api_client/models/feed_status_type.py` & `yandex_api_client-0.0.2/yandex_api_client/models/feed_status_type.py`

 * *Files identical despite different names*

### Comparing `yandex_api_client-0.0.1/yandex_api_client/models/feedback_author_dto.py` & `yandex_api_client-0.0.2/yandex_api_client/models/feedback_author_dto.py`

 * *Files identical despite different names*

### Comparing `yandex_api_client-0.0.1/yandex_api_client/models/feedback_comment_author_dto.py` & `yandex_api_client-0.0.2/yandex_api_client/models/feedback_comment_author_dto.py`

 * *Files identical despite different names*

### Comparing `yandex_api_client-0.0.1/yandex_api_client/models/feedback_comment_author_type.py` & `yandex_api_client-0.0.2/yandex_api_client/models/feedback_comment_author_type.py`

 * *Files identical despite different names*

### Comparing `yandex_api_client-0.0.1/yandex_api_client/models/feedback_comment_dto.py` & `yandex_api_client-0.0.2/yandex_api_client/models/feedback_comment_dto.py`

 * *Files identical despite different names*

### Comparing `yandex_api_client-0.0.1/yandex_api_client/models/feedback_delivery_type.py` & `yandex_api_client-0.0.2/yandex_api_client/models/feedback_delivery_type.py`

 * *Files identical despite different names*

### Comparing `yandex_api_client-0.0.1/yandex_api_client/models/feedback_dto.py` & `yandex_api_client-0.0.2/yandex_api_client/models/feedback_dto.py`

 * *Files identical despite different names*

### Comparing `yandex_api_client-0.0.1/yandex_api_client/models/feedback_factor_dto.py` & `yandex_api_client-0.0.2/yandex_api_client/models/feedback_factor_dto.py`

 * *Files identical despite different names*

### Comparing `yandex_api_client-0.0.1/yandex_api_client/models/feedback_grades_dto.py` & `yandex_api_client-0.0.2/yandex_api_client/models/feedback_grades_dto.py`

 * *Files identical despite different names*

### Comparing `yandex_api_client-0.0.1/yandex_api_client/models/feedback_list_dto.py` & `yandex_api_client-0.0.2/yandex_api_client/models/feedback_list_dto.py`

 * *Files identical despite different names*

### Comparing `yandex_api_client-0.0.1/yandex_api_client/models/feedback_order_dto.py` & `yandex_api_client-0.0.2/yandex_api_client/models/feedback_order_dto.py`

 * *Files identical despite different names*

### Comparing `yandex_api_client-0.0.1/yandex_api_client/models/feedback_shop_dto.py` & `yandex_api_client-0.0.2/yandex_api_client/models/feedback_shop_dto.py`

 * *Files identical despite different names*

### Comparing `yandex_api_client-0.0.1/yandex_api_client/models/feedback_state_type.py` & `yandex_api_client-0.0.2/yandex_api_client/models/feedback_state_type.py`

 * *Files identical despite different names*

### Comparing `yandex_api_client-0.0.1/yandex_api_client/models/field_state_type.py` & `yandex_api_client-0.0.2/yandex_api_client/models/field_state_type.py`

 * *Files identical despite different names*

### Comparing `yandex_api_client-0.0.1/yandex_api_client/models/flipping_pager_dto.py` & `yandex_api_client-0.0.2/yandex_api_client/models/flipping_pager_dto.py`

 * *Files identical despite different names*

### Comparing `yandex_api_client-0.0.1/yandex_api_client/models/forward_scrolling_pager_dto.py` & `yandex_api_client-0.0.2/yandex_api_client/models/forward_scrolling_pager_dto.py`

 * *Files identical despite different names*

### Comparing `yandex_api_client-0.0.1/yandex_api_client/models/fulfillment_warehouse_dto.py` & `yandex_api_client-0.0.2/yandex_api_client/models/fulfillment_warehouse_dto.py`

 * *Files identical despite different names*

### Comparing `yandex_api_client-0.0.1/yandex_api_client/models/fulfillment_warehouses_dto.py` & `yandex_api_client-0.0.2/yandex_api_client/models/fulfillment_warehouses_dto.py`

 * *Files identical despite different names*

### Comparing `yandex_api_client-0.0.1/yandex_api_client/models/full_outlet_dto.py` & `yandex_api_client-0.0.2/yandex_api_client/models/full_outlet_dto.py`

 * *Files identical despite different names*

### Comparing `yandex_api_client-0.0.1/yandex_api_client/models/full_outlet_license_dto.py` & `yandex_api_client-0.0.2/yandex_api_client/models/full_outlet_license_dto.py`

 * *Files identical despite different names*

### Comparing `yandex_api_client-0.0.1/yandex_api_client/models/generate_boost_consolidated_request.py` & `yandex_api_client-0.0.2/yandex_api_client/models/generate_boost_consolidated_request.py`

 * *Files identical despite different names*

### Comparing `yandex_api_client-0.0.1/yandex_api_client/models/generate_goods_movement_report_request.py` & `yandex_api_client-0.0.2/yandex_api_client/models/generate_goods_movement_report_request.py`

 * *Files identical despite different names*

### Comparing `yandex_api_client-0.0.1/yandex_api_client/models/generate_goods_realization_report_request.py` & `yandex_api_client-0.0.2/yandex_api_client/models/generate_goods_realization_report_request.py`

 * *Files identical despite different names*

### Comparing `yandex_api_client-0.0.1/yandex_api_client/models/generate_goods_turnover_request.py` & `yandex_api_client-0.0.2/yandex_api_client/models/generate_goods_turnover_request.py`

 * *Files identical despite different names*

### Comparing `yandex_api_client-0.0.1/yandex_api_client/models/generate_prices_report_request.py` & `yandex_api_client-0.0.2/yandex_api_client/models/generate_prices_report_request.py`

 * *Files identical despite different names*

### Comparing `yandex_api_client-0.0.1/yandex_api_client/models/generate_report_dto.py` & `yandex_api_client-0.0.2/yandex_api_client/models/generate_report_dto.py`

 * *Files identical despite different names*

### Comparing `yandex_api_client-0.0.1/yandex_api_client/models/generate_report_response.py` & `yandex_api_client-0.0.2/yandex_api_client/models/generate_report_response.py`

 * *Files identical despite different names*

### Comparing `yandex_api_client-0.0.1/yandex_api_client/models/generate_shipment_list_document_report_request.py` & `yandex_api_client-0.0.2/yandex_api_client/models/generate_shipment_list_document_report_request.py`

 * *Files identical despite different names*

### Comparing `yandex_api_client-0.0.1/yandex_api_client/models/generate_shows_sales_report_request.py` & `yandex_api_client-0.0.2/yandex_api_client/models/generate_shows_sales_report_request.py`

 * *Files identical despite different names*

### Comparing `yandex_api_client-0.0.1/yandex_api_client/models/generate_stocks_on_warehouses_report_request.py` & `yandex_api_client-0.0.2/yandex_api_client/models/generate_stocks_on_warehouses_report_request.py`

 * *Files identical despite different names*

### Comparing `yandex_api_client-0.0.1/yandex_api_client/models/generate_united_marketplace_services_report_request.py` & `yandex_api_client-0.0.2/yandex_api_client/models/generate_united_marketplace_services_report_request.py`

 * *Files identical despite different names*

### Comparing `yandex_api_client-0.0.1/yandex_api_client/models/generate_united_netting_report_request.py` & `yandex_api_client-0.0.2/yandex_api_client/models/generate_united_netting_report_request.py`

 * *Files identical despite different names*

### Comparing `yandex_api_client-0.0.1/yandex_api_client/models/generate_united_orders_request.py` & `yandex_api_client-0.0.2/yandex_api_client/models/generate_united_orders_request.py`

 * *Files identical despite different names*

### Comparing `yandex_api_client-0.0.1/yandex_api_client/models/get_all_offers_response.py` & `yandex_api_client-0.0.2/yandex_api_client/models/get_all_offers_response.py`

 * *Files identical despite different names*

### Comparing `yandex_api_client-0.0.1/yandex_api_client/models/get_bids_info_request.py` & `yandex_api_client-0.0.2/yandex_api_client/models/get_bids_info_request.py`

 * *Files identical despite different names*

### Comparing `yandex_api_client-0.0.1/yandex_api_client/models/get_bids_info_response.py` & `yandex_api_client-0.0.2/yandex_api_client/models/get_bids_info_response.py`

 * *Files identical despite different names*

### Comparing `yandex_api_client-0.0.1/yandex_api_client/models/get_bids_info_response_dto.py` & `yandex_api_client-0.0.2/yandex_api_client/models/get_bids_info_response_dto.py`

 * *Files identical despite different names*

### Comparing `yandex_api_client-0.0.1/yandex_api_client/models/get_bids_recommendations_request.py` & `yandex_api_client-0.0.2/yandex_api_client/models/get_bids_recommendations_request.py`

 * *Files identical despite different names*

### Comparing `yandex_api_client-0.0.1/yandex_api_client/models/get_bids_recommendations_response.py` & `yandex_api_client-0.0.2/yandex_api_client/models/get_bids_recommendations_response.py`

 * *Files identical despite different names*

### Comparing `yandex_api_client-0.0.1/yandex_api_client/models/get_bids_recommendations_response_dto.py` & `yandex_api_client-0.0.2/yandex_api_client/models/get_bids_recommendations_response_dto.py`

 * *Files identical despite different names*

### Comparing `yandex_api_client-0.0.1/yandex_api_client/models/get_business_buyer_info_response.py` & `yandex_api_client-0.0.2/yandex_api_client/models/get_business_buyer_info_response.py`

 * *Files identical despite different names*

### Comparing `yandex_api_client-0.0.1/yandex_api_client/models/get_business_documents_info_response.py` & `yandex_api_client-0.0.2/yandex_api_client/models/get_business_documents_info_response.py`

 * *Files identical despite different names*

### Comparing `yandex_api_client-0.0.1/yandex_api_client/models/get_campaign_categories_response.py` & `yandex_api_client-0.0.2/yandex_api_client/models/get_campaign_categories_response.py`

 * *Files identical despite different names*

### Comparing `yandex_api_client-0.0.1/yandex_api_client/models/get_campaign_logins_response.py` & `yandex_api_client-0.0.2/yandex_api_client/models/get_campaign_logins_response.py`

 * *Files identical despite different names*

### Comparing `yandex_api_client-0.0.1/yandex_api_client/models/get_campaign_offer_dto.py` & `yandex_api_client-0.0.2/yandex_api_client/models/get_campaign_offer_dto.py`

 * *Files identical despite different names*

### Comparing `yandex_api_client-0.0.1/yandex_api_client/models/get_campaign_offers_request.py` & `yandex_api_client-0.0.2/yandex_api_client/models/get_campaign_offers_request.py`

 * *Files identical despite different names*

### Comparing `yandex_api_client-0.0.1/yandex_api_client/models/get_campaign_offers_response.py` & `yandex_api_client-0.0.2/yandex_api_client/models/get_campaign_offers_response.py`

 * *Files identical despite different names*

### Comparing `yandex_api_client-0.0.1/yandex_api_client/models/get_campaign_offers_result_dto.py` & `yandex_api_client-0.0.2/yandex_api_client/models/get_campaign_offers_result_dto.py`

 * *Files identical despite different names*

### Comparing `yandex_api_client-0.0.1/yandex_api_client/models/get_campaign_region_response.py` & `yandex_api_client-0.0.2/yandex_api_client/models/get_campaign_region_response.py`

 * *Files identical despite different names*

### Comparing `yandex_api_client-0.0.1/yandex_api_client/models/get_campaign_response.py` & `yandex_api_client-0.0.2/yandex_api_client/models/get_campaign_response.py`

 * *Files identical despite different names*

### Comparing `yandex_api_client-0.0.1/yandex_api_client/models/get_campaign_settings_response.py` & `yandex_api_client-0.0.2/yandex_api_client/models/get_campaign_settings_response.py`

 * *Files identical despite different names*

### Comparing `yandex_api_client-0.0.1/yandex_api_client/models/get_campaigns_response.py` & `yandex_api_client-0.0.2/yandex_api_client/models/get_campaigns_response.py`

 * *Files identical despite different names*

### Comparing `yandex_api_client-0.0.1/yandex_api_client/models/get_categories_response.py` & `yandex_api_client-0.0.2/yandex_api_client/models/get_categories_response.py`

 * *Files identical despite different names*

### Comparing `yandex_api_client-0.0.1/yandex_api_client/models/get_category_content_parameters_response.py` & `yandex_api_client-0.0.2/yandex_api_client/models/get_category_content_parameters_response.py`

 * *Files identical despite different names*

### Comparing `yandex_api_client-0.0.1/yandex_api_client/models/get_chat_history_request.py` & `yandex_api_client-0.0.2/yandex_api_client/models/get_chat_history_request.py`

 * *Files identical despite different names*

### Comparing `yandex_api_client-0.0.1/yandex_api_client/models/get_chat_history_response.py` & `yandex_api_client-0.0.2/yandex_api_client/models/get_chat_history_response.py`

 * *Files identical despite different names*

### Comparing `yandex_api_client-0.0.1/yandex_api_client/models/get_chat_info_dto.py` & `yandex_api_client-0.0.2/yandex_api_client/models/get_chat_info_dto.py`

 * *Files identical despite different names*

### Comparing `yandex_api_client-0.0.1/yandex_api_client/models/get_chats_info_dto.py` & `yandex_api_client-0.0.2/yandex_api_client/models/get_chats_info_dto.py`

 * *Files identical despite different names*

### Comparing `yandex_api_client-0.0.1/yandex_api_client/models/get_chats_request.py` & `yandex_api_client-0.0.2/yandex_api_client/models/get_chats_request.py`

 * *Files identical despite different names*

### Comparing `yandex_api_client-0.0.1/yandex_api_client/models/get_chats_response.py` & `yandex_api_client-0.0.2/yandex_api_client/models/get_chats_response.py`

 * *Files identical despite different names*

### Comparing `yandex_api_client-0.0.1/yandex_api_client/models/get_delivery_services_response.py` & `yandex_api_client-0.0.2/yandex_api_client/models/get_delivery_services_response.py`

 * *Files identical despite different names*

### Comparing `yandex_api_client-0.0.1/yandex_api_client/models/get_feed_categories_response.py` & `yandex_api_client-0.0.2/yandex_api_client/models/get_feed_categories_response.py`

 * *Files identical despite different names*

### Comparing `yandex_api_client-0.0.1/yandex_api_client/models/get_feed_index_logs_response.py` & `yandex_api_client-0.0.2/yandex_api_client/models/get_feed_index_logs_response.py`

 * *Files identical despite different names*

### Comparing `yandex_api_client-0.0.1/yandex_api_client/models/get_feed_response.py` & `yandex_api_client-0.0.2/yandex_api_client/models/get_feed_response.py`

 * *Files identical despite different names*

### Comparing `yandex_api_client-0.0.1/yandex_api_client/models/get_feedback_list_response.py` & `yandex_api_client-0.0.2/yandex_api_client/models/get_feedback_list_response.py`

 * *Files identical despite different names*

### Comparing `yandex_api_client-0.0.1/yandex_api_client/models/get_feeds_response.py` & `yandex_api_client-0.0.2/yandex_api_client/models/get_feeds_response.py`

 * *Files identical despite different names*

### Comparing `yandex_api_client-0.0.1/yandex_api_client/models/get_fulfillment_warehouses_response.py` & `yandex_api_client-0.0.2/yandex_api_client/models/get_fulfillment_warehouses_response.py`

 * *Files identical despite different names*

### Comparing `yandex_api_client-0.0.1/yandex_api_client/models/get_goods_stats_request.py` & `yandex_api_client-0.0.2/yandex_api_client/models/get_goods_stats_request.py`

 * *Files identical despite different names*

### Comparing `yandex_api_client-0.0.1/yandex_api_client/models/get_goods_stats_response.py` & `yandex_api_client-0.0.2/yandex_api_client/models/get_goods_stats_response.py`

 * *Files identical despite different names*

### Comparing `yandex_api_client-0.0.1/yandex_api_client/models/get_hidden_offers_response.py` & `yandex_api_client-0.0.2/yandex_api_client/models/get_hidden_offers_response.py`

 * *Files identical despite different names*

### Comparing `yandex_api_client-0.0.1/yandex_api_client/models/get_hidden_offers_result_dto.py` & `yandex_api_client-0.0.2/yandex_api_client/models/get_hidden_offers_result_dto.py`

 * *Files identical despite different names*

### Comparing `yandex_api_client-0.0.1/yandex_api_client/models/get_mapping_dto.py` & `yandex_api_client-0.0.2/yandex_api_client/models/get_mapping_dto.py`

 * *Files identical despite different names*

### Comparing `yandex_api_client-0.0.1/yandex_api_client/models/get_models_offers_response.py` & `yandex_api_client-0.0.2/yandex_api_client/models/get_models_offers_response.py`

 * *Files identical despite different names*

### Comparing `yandex_api_client-0.0.1/yandex_api_client/models/get_models_request.py` & `yandex_api_client-0.0.2/yandex_api_client/models/get_models_request.py`

 * *Files identical despite different names*

### Comparing `yandex_api_client-0.0.1/yandex_api_client/models/get_models_response.py` & `yandex_api_client-0.0.2/yandex_api_client/models/get_models_response.py`

 * *Files identical despite different names*

### Comparing `yandex_api_client-0.0.1/yandex_api_client/models/get_offer_cards_content_status_request.py` & `yandex_api_client-0.0.2/yandex_api_client/models/get_offer_cards_content_status_request.py`

 * *Files identical despite different names*

### Comparing `yandex_api_client-0.0.1/yandex_api_client/models/get_offer_cards_content_status_response.py` & `yandex_api_client-0.0.2/yandex_api_client/models/get_offer_cards_content_status_response.py`

 * *Files identical despite different names*

### Comparing `yandex_api_client-0.0.1/yandex_api_client/models/get_offer_dto.py` & `yandex_api_client-0.0.2/yandex_api_client/models/get_offer_dto.py`

 * *Files identical despite different names*

### Comparing `yandex_api_client-0.0.1/yandex_api_client/models/get_offer_mapping_dto.py` & `yandex_api_client-0.0.2/yandex_api_client/models/get_offer_mapping_dto.py`

 * *Files identical despite different names*

### Comparing `yandex_api_client-0.0.1/yandex_api_client/models/get_offer_mapping_entries_response.py` & `yandex_api_client-0.0.2/yandex_api_client/models/get_offer_mapping_entries_response.py`

 * *Files identical despite different names*

### Comparing `yandex_api_client-0.0.1/yandex_api_client/models/get_offer_mappings_request.py` & `yandex_api_client-0.0.2/yandex_api_client/models/get_offer_mappings_request.py`

 * *Files identical despite different names*

### Comparing `yandex_api_client-0.0.1/yandex_api_client/models/get_offer_mappings_response.py` & `yandex_api_client-0.0.2/yandex_api_client/models/get_offer_mappings_response.py`

 * *Files identical despite different names*

### Comparing `yandex_api_client-0.0.1/yandex_api_client/models/get_offer_mappings_result_dto.py` & `yandex_api_client-0.0.2/yandex_api_client/models/get_offer_mappings_result_dto.py`

 * *Files identical despite different names*

### Comparing `yandex_api_client-0.0.1/yandex_api_client/models/get_offer_recommendations_request.py` & `yandex_api_client-0.0.2/yandex_api_client/models/get_offer_recommendations_request.py`

 * *Files identical despite different names*

### Comparing `yandex_api_client-0.0.1/yandex_api_client/models/get_offer_recommendations_response.py` & `yandex_api_client-0.0.2/yandex_api_client/models/get_offer_recommendations_response.py`

 * *Files identical despite different names*

### Comparing `yandex_api_client-0.0.1/yandex_api_client/models/get_offers_response.py` & `yandex_api_client-0.0.2/yandex_api_client/models/get_offers_response.py`

 * *Files identical despite different names*

### Comparing `yandex_api_client-0.0.1/yandex_api_client/models/get_order_buyer_info_response.py` & `yandex_api_client-0.0.2/yandex_api_client/models/get_order_buyer_info_response.py`

 * *Files identical despite different names*

### Comparing `yandex_api_client-0.0.1/yandex_api_client/models/get_order_labels_data_response.py` & `yandex_api_client-0.0.2/yandex_api_client/models/get_order_labels_data_response.py`

 * *Files identical despite different names*

### Comparing `yandex_api_client-0.0.1/yandex_api_client/models/get_order_response.py` & `yandex_api_client-0.0.2/yandex_api_client/models/get_order_response.py`

 * *Files identical despite different names*

### Comparing `yandex_api_client-0.0.1/yandex_api_client/models/get_orders_response.py` & `yandex_api_client-0.0.2/yandex_api_client/models/get_orders_response.py`

 * *Files identical despite different names*

### Comparing `yandex_api_client-0.0.1/yandex_api_client/models/get_orders_stats_request.py` & `yandex_api_client-0.0.2/yandex_api_client/models/get_orders_stats_request.py`

 * *Files identical despite different names*

### Comparing `yandex_api_client-0.0.1/yandex_api_client/models/get_orders_stats_response.py` & `yandex_api_client-0.0.2/yandex_api_client/models/get_orders_stats_response.py`

 * *Files identical despite different names*

### Comparing `yandex_api_client-0.0.1/yandex_api_client/models/get_outlet_licenses_response.py` & `yandex_api_client-0.0.2/yandex_api_client/models/get_outlet_licenses_response.py`

 * *Files identical despite different names*

### Comparing `yandex_api_client-0.0.1/yandex_api_client/models/get_outlet_response.py` & `yandex_api_client-0.0.2/yandex_api_client/models/get_outlet_response.py`

 * *Files identical despite different names*

### Comparing `yandex_api_client-0.0.1/yandex_api_client/models/get_outlets_response.py` & `yandex_api_client-0.0.2/yandex_api_client/models/get_outlets_response.py`

 * *Files identical despite different names*

### Comparing `yandex_api_client-0.0.1/yandex_api_client/models/get_price_dto.py` & `yandex_api_client-0.0.2/yandex_api_client/models/get_price_dto.py`

 * *Files identical despite different names*

### Comparing `yandex_api_client-0.0.1/yandex_api_client/models/get_price_with_discount_dto.py` & `yandex_api_client-0.0.2/yandex_api_client/models/get_price_with_discount_dto.py`

 * *Files identical despite different names*

### Comparing `yandex_api_client-0.0.1/yandex_api_client/models/get_price_with_vat_dto.py` & `yandex_api_client-0.0.2/yandex_api_client/models/get_price_with_vat_dto.py`

 * *Files identical despite different names*

### Comparing `yandex_api_client-0.0.1/yandex_api_client/models/get_prices_by_offer_ids_request.py` & `yandex_api_client-0.0.2/yandex_api_client/models/get_prices_by_offer_ids_request.py`

 * *Files identical despite different names*

### Comparing `yandex_api_client-0.0.1/yandex_api_client/models/get_prices_by_offer_ids_response.py` & `yandex_api_client-0.0.2/yandex_api_client/models/get_prices_by_offer_ids_response.py`

 * *Files identical despite different names*

### Comparing `yandex_api_client-0.0.1/yandex_api_client/models/get_prices_response.py` & `yandex_api_client-0.0.2/yandex_api_client/models/get_prices_response.py`

 * *Files identical despite different names*

### Comparing `yandex_api_client-0.0.1/yandex_api_client/models/get_quarantine_offers_request.py` & `yandex_api_client-0.0.2/yandex_api_client/models/get_quarantine_offers_request.py`

 * *Files identical despite different names*

### Comparing `yandex_api_client-0.0.1/yandex_api_client/models/get_quarantine_offers_response.py` & `yandex_api_client-0.0.2/yandex_api_client/models/get_quarantine_offers_response.py`

 * *Files identical despite different names*

### Comparing `yandex_api_client-0.0.1/yandex_api_client/models/get_quarantine_offers_result_dto.py` & `yandex_api_client-0.0.2/yandex_api_client/models/get_quarantine_offers_result_dto.py`

 * *Files identical despite different names*

### Comparing `yandex_api_client-0.0.1/yandex_api_client/models/get_region_with_children_response.py` & `yandex_api_client-0.0.2/yandex_api_client/models/get_region_with_children_response.py`

 * *Files identical despite different names*

### Comparing `yandex_api_client-0.0.1/yandex_api_client/models/get_regions_response.py` & `yandex_api_client-0.0.2/yandex_api_client/models/get_regions_response.py`

 * *Files identical despite different names*

### Comparing `yandex_api_client-0.0.1/yandex_api_client/models/get_report_info_response.py` & `yandex_api_client-0.0.2/yandex_api_client/models/get_report_info_response.py`

 * *Files identical despite different names*

### Comparing `yandex_api_client-0.0.1/yandex_api_client/models/get_return_response.py` & `yandex_api_client-0.0.2/yandex_api_client/models/get_return_response.py`

 * *Files identical despite different names*

### Comparing `yandex_api_client-0.0.1/yandex_api_client/models/get_returns_response.py` & `yandex_api_client-0.0.2/yandex_api_client/models/get_returns_response.py`

 * *Files identical despite different names*

### Comparing `yandex_api_client-0.0.1/yandex_api_client/models/get_shipment_orders_info_response.py` & `yandex_api_client-0.0.2/yandex_api_client/models/get_shipment_orders_info_response.py`

 * *Files identical despite different names*

### Comparing `yandex_api_client-0.0.1/yandex_api_client/models/get_shipment_response.py` & `yandex_api_client-0.0.2/yandex_api_client/models/get_shipment_response.py`

 * *Files identical despite different names*

### Comparing `yandex_api_client-0.0.1/yandex_api_client/models/get_suggested_offer_mapping_entries_request.py` & `yandex_api_client-0.0.2/yandex_api_client/models/get_suggested_offer_mapping_entries_request.py`

 * *Files identical despite different names*

### Comparing `yandex_api_client-0.0.1/yandex_api_client/models/get_suggested_offer_mapping_entries_response.py` & `yandex_api_client-0.0.2/yandex_api_client/models/get_suggested_offer_mapping_entries_response.py`

 * *Files identical despite different names*

### Comparing `yandex_api_client-0.0.1/yandex_api_client/models/get_suggested_offer_mappings_request.py` & `yandex_api_client-0.0.2/yandex_api_client/models/get_suggested_offer_mappings_request.py`

 * *Files identical despite different names*

### Comparing `yandex_api_client-0.0.1/yandex_api_client/models/get_suggested_offer_mappings_response.py` & `yandex_api_client-0.0.2/yandex_api_client/models/get_suggested_offer_mappings_response.py`

 * *Files identical despite different names*

### Comparing `yandex_api_client-0.0.1/yandex_api_client/models/get_suggested_offer_mappings_result_dto.py` & `yandex_api_client-0.0.2/yandex_api_client/models/get_suggested_offer_mappings_result_dto.py`

 * *Files identical despite different names*

### Comparing `yandex_api_client-0.0.1/yandex_api_client/models/get_warehouse_stocks_dto.py` & `yandex_api_client-0.0.2/yandex_api_client/models/get_warehouse_stocks_dto.py`

 * *Files identical despite different names*

### Comparing `yandex_api_client-0.0.1/yandex_api_client/models/get_warehouse_stocks_request.py` & `yandex_api_client-0.0.2/yandex_api_client/models/get_warehouse_stocks_request.py`

 * *Files identical despite different names*

### Comparing `yandex_api_client-0.0.1/yandex_api_client/models/get_warehouse_stocks_response.py` & `yandex_api_client-0.0.2/yandex_api_client/models/get_warehouse_stocks_response.py`

 * *Files identical despite different names*

### Comparing `yandex_api_client-0.0.1/yandex_api_client/models/get_warehouses_response.py` & `yandex_api_client-0.0.2/yandex_api_client/models/get_warehouses_response.py`

 * *Files identical despite different names*

### Comparing `yandex_api_client-0.0.1/yandex_api_client/models/goods_stats_dto.py` & `yandex_api_client-0.0.2/yandex_api_client/models/goods_stats_dto.py`

 * *Files identical despite different names*

### Comparing `yandex_api_client-0.0.1/yandex_api_client/models/goods_stats_goods_dto.py` & `yandex_api_client-0.0.2/yandex_api_client/models/goods_stats_goods_dto.py`

 * *Files identical despite different names*

### Comparing `yandex_api_client-0.0.1/yandex_api_client/models/goods_stats_warehouse_dto.py` & `yandex_api_client-0.0.2/yandex_api_client/models/goods_stats_warehouse_dto.py`

 * *Files identical despite different names*

### Comparing `yandex_api_client-0.0.1/yandex_api_client/models/goods_stats_weight_dimensions_dto.py` & `yandex_api_client-0.0.2/yandex_api_client/models/goods_stats_weight_dimensions_dto.py`

 * *Files identical despite different names*

### Comparing `yandex_api_client-0.0.1/yandex_api_client/models/gps_dto.py` & `yandex_api_client-0.0.2/yandex_api_client/models/gps_dto.py`

 * *Files identical despite different names*

### Comparing `yandex_api_client-0.0.1/yandex_api_client/models/hidden_offer_dto.py` & `yandex_api_client-0.0.2/yandex_api_client/models/hidden_offer_dto.py`

 * *Files identical despite different names*

### Comparing `yandex_api_client-0.0.1/yandex_api_client/models/license_check_status_type.py` & `yandex_api_client-0.0.2/yandex_api_client/models/license_check_status_type.py`

 * *Files identical despite different names*

### Comparing `yandex_api_client-0.0.1/yandex_api_client/models/license_type.py` & `yandex_api_client-0.0.2/yandex_api_client/models/license_type.py`

 * *Files identical despite different names*

### Comparing `yandex_api_client-0.0.1/yandex_api_client/models/logistic_pickup_point_dto.py` & `yandex_api_client-0.0.2/yandex_api_client/models/logistic_pickup_point_dto.py`

 * *Files identical despite different names*

### Comparing `yandex_api_client-0.0.1/yandex_api_client/models/logistic_point_type.py` & `yandex_api_client-0.0.2/yandex_api_client/models/logistic_point_type.py`

 * *Files identical despite different names*

### Comparing `yandex_api_client-0.0.1/yandex_api_client/models/mappings_offer_dto.py` & `yandex_api_client-0.0.2/yandex_api_client/models/mappings_offer_dto.py`

 * *Files identical despite different names*

### Comparing `yandex_api_client-0.0.1/yandex_api_client/models/mappings_offer_info_dto.py` & `yandex_api_client-0.0.2/yandex_api_client/models/mappings_offer_info_dto.py`

 * *Files identical despite different names*

### Comparing `yandex_api_client-0.0.1/yandex_api_client/models/model_dto.py` & `yandex_api_client-0.0.2/yandex_api_client/models/model_dto.py`

 * *Files identical despite different names*

### Comparing `yandex_api_client-0.0.1/yandex_api_client/models/model_offer_dto.py` & `yandex_api_client-0.0.2/yandex_api_client/models/model_offer_dto.py`

 * *Files identical despite different names*

### Comparing `yandex_api_client-0.0.1/yandex_api_client/models/model_price_dto.py` & `yandex_api_client-0.0.2/yandex_api_client/models/model_price_dto.py`

 * *Files identical despite different names*

### Comparing `yandex_api_client-0.0.1/yandex_api_client/models/offer_availability_status_type.py` & `yandex_api_client-0.0.2/yandex_api_client/models/offer_availability_status_type.py`

 * *Files identical despite different names*

### Comparing `yandex_api_client-0.0.1/yandex_api_client/models/offer_campaign_status_dto.py` & `yandex_api_client-0.0.2/yandex_api_client/models/offer_campaign_status_dto.py`

 * *Files identical despite different names*

### Comparing `yandex_api_client-0.0.1/yandex_api_client/models/offer_campaign_status_type.py` & `yandex_api_client-0.0.2/yandex_api_client/models/offer_campaign_status_type.py`

 * *Files identical despite different names*

### Comparing `yandex_api_client-0.0.1/yandex_api_client/models/offer_card_dto.py` & `yandex_api_client-0.0.2/yandex_api_client/models/offer_card_dto.py`

 * *Files identical despite different names*

### Comparing `yandex_api_client-0.0.1/yandex_api_client/models/offer_card_recommendation_dto.py` & `yandex_api_client-0.0.2/yandex_api_client/models/offer_card_recommendation_dto.py`

 * *Files identical despite different names*

### Comparing `yandex_api_client-0.0.1/yandex_api_client/models/offer_card_recommendation_type.py` & `yandex_api_client-0.0.2/yandex_api_client/models/offer_card_recommendation_type.py`

 * *Files identical despite different names*

### Comparing `yandex_api_client-0.0.1/yandex_api_client/models/offer_card_status_type.py` & `yandex_api_client-0.0.2/yandex_api_client/models/offer_card_status_type.py`

 * *Files identical despite different names*

### Comparing `yandex_api_client-0.0.1/yandex_api_client/models/offer_cards_content_status_dto.py` & `yandex_api_client-0.0.2/yandex_api_client/models/offer_cards_content_status_dto.py`

 * *Files identical despite different names*

### Comparing `yandex_api_client-0.0.1/yandex_api_client/models/offer_condition_dto.py` & `yandex_api_client-0.0.2/yandex_api_client/models/offer_condition_dto.py`

 * *Files identical despite different names*

### Comparing `yandex_api_client-0.0.1/yandex_api_client/models/offer_condition_quality_type.py` & `yandex_api_client-0.0.2/yandex_api_client/models/offer_condition_quality_type.py`

 * *Files identical despite different names*

### Comparing `yandex_api_client-0.0.1/yandex_api_client/models/offer_condition_type.py` & `yandex_api_client-0.0.2/yandex_api_client/models/offer_condition_type.py`

 * *Files identical despite different names*

### Comparing `yandex_api_client-0.0.1/yandex_api_client/models/offer_content_dto.py` & `yandex_api_client-0.0.2/yandex_api_client/models/offer_content_dto.py`

 * *Files identical despite different names*

### Comparing `yandex_api_client-0.0.1/yandex_api_client/models/offer_content_error_dto.py` & `yandex_api_client-0.0.2/yandex_api_client/models/offer_content_error_dto.py`

 * *Files identical despite different names*

### Comparing `yandex_api_client-0.0.1/yandex_api_client/models/offer_content_error_type.py` & `yandex_api_client-0.0.2/yandex_api_client/models/offer_content_error_type.py`

 * *Files identical despite different names*

### Comparing `yandex_api_client-0.0.1/yandex_api_client/models/offer_dto.py` & `yandex_api_client-0.0.2/yandex_api_client/models/offer_dto.py`

 * *Files identical despite different names*

### Comparing `yandex_api_client-0.0.1/yandex_api_client/models/offer_error_dto.py` & `yandex_api_client-0.0.2/yandex_api_client/models/offer_error_dto.py`

 * *Files identical despite different names*

### Comparing `yandex_api_client-0.0.1/yandex_api_client/models/offer_for_recommendation_dto.py` & `yandex_api_client-0.0.2/yandex_api_client/models/offer_for_recommendation_dto.py`

 * *Files identical despite different names*

### Comparing `yandex_api_client-0.0.1/yandex_api_client/models/offer_manual_dto.py` & `yandex_api_client-0.0.2/yandex_api_client/models/offer_manual_dto.py`

 * *Files identical despite different names*

### Comparing `yandex_api_client-0.0.1/yandex_api_client/models/offer_mapping_dto.py` & `yandex_api_client-0.0.2/yandex_api_client/models/offer_mapping_dto.py`

 * *Files identical despite different names*

### Comparing `yandex_api_client-0.0.1/yandex_api_client/models/offer_mapping_entries_dto.py` & `yandex_api_client-0.0.2/yandex_api_client/models/offer_mapping_entries_dto.py`

 * *Files identical despite different names*

### Comparing `yandex_api_client-0.0.1/yandex_api_client/models/offer_mapping_entry_dto.py` & `yandex_api_client-0.0.2/yandex_api_client/models/offer_mapping_entry_dto.py`

 * *Files identical despite different names*

### Comparing `yandex_api_client-0.0.1/yandex_api_client/models/offer_mapping_info_dto.py` & `yandex_api_client-0.0.2/yandex_api_client/models/offer_mapping_info_dto.py`

 * *Files identical despite different names*

### Comparing `yandex_api_client-0.0.1/yandex_api_client/models/offer_mapping_kind_type.py` & `yandex_api_client-0.0.2/yandex_api_client/models/offer_mapping_kind_type.py`

 * *Files identical despite different names*

### Comparing `yandex_api_client-0.0.1/yandex_api_client/models/offer_mapping_suggestions_list_dto.py` & `yandex_api_client-0.0.2/yandex_api_client/models/offer_mapping_suggestions_list_dto.py`

 * *Files identical despite different names*

### Comparing `yandex_api_client-0.0.1/yandex_api_client/models/offer_param_dto.py` & `yandex_api_client-0.0.2/yandex_api_client/models/offer_param_dto.py`

 * *Files identical despite different names*

### Comparing `yandex_api_client-0.0.1/yandex_api_client/models/offer_price_by_offer_ids_list_response_dto.py` & `yandex_api_client-0.0.2/yandex_api_client/models/offer_price_by_offer_ids_list_response_dto.py`

 * *Files identical despite different names*

### Comparing `yandex_api_client-0.0.1/yandex_api_client/models/offer_price_by_offer_ids_response_dto.py` & `yandex_api_client-0.0.2/yandex_api_client/models/offer_price_by_offer_ids_response_dto.py`

 * *Files identical despite different names*

### Comparing `yandex_api_client-0.0.1/yandex_api_client/models/offer_price_dto.py` & `yandex_api_client-0.0.2/yandex_api_client/models/offer_price_dto.py`

 * *Files identical despite different names*

### Comparing `yandex_api_client-0.0.1/yandex_api_client/models/offer_price_feed_dto.py` & `yandex_api_client-0.0.2/yandex_api_client/models/offer_price_feed_dto.py`

 * *Files identical despite different names*

### Comparing `yandex_api_client-0.0.1/yandex_api_client/models/offer_price_list_response_dto.py` & `yandex_api_client-0.0.2/yandex_api_client/models/offer_price_list_response_dto.py`

 * *Files identical despite different names*

### Comparing `yandex_api_client-0.0.1/yandex_api_client/models/offer_price_response_dto.py` & `yandex_api_client-0.0.2/yandex_api_client/models/offer_price_response_dto.py`

 * *Files identical despite different names*

### Comparing `yandex_api_client-0.0.1/yandex_api_client/models/offer_processing_note_dto.py` & `yandex_api_client-0.0.2/yandex_api_client/models/offer_processing_note_dto.py`

 * *Files identical despite different names*

### Comparing `yandex_api_client-0.0.1/yandex_api_client/models/offer_processing_note_type.py` & `yandex_api_client-0.0.2/yandex_api_client/models/offer_processing_note_type.py`

 * *Files identical despite different names*

### Comparing `yandex_api_client-0.0.1/yandex_api_client/models/offer_processing_state_dto.py` & `yandex_api_client-0.0.2/yandex_api_client/models/offer_processing_state_dto.py`

 * *Files identical despite different names*

### Comparing `yandex_api_client-0.0.1/yandex_api_client/models/offer_processing_status_type.py` & `yandex_api_client-0.0.2/yandex_api_client/models/offer_processing_status_type.py`

 * *Files identical despite different names*

### Comparing `yandex_api_client-0.0.1/yandex_api_client/models/offer_recommendation_dto.py` & `yandex_api_client-0.0.2/yandex_api_client/models/offer_recommendation_dto.py`

 * *Files identical despite different names*

### Comparing `yandex_api_client-0.0.1/yandex_api_client/models/offer_recommendation_info_dto.py` & `yandex_api_client-0.0.2/yandex_api_client/models/offer_recommendation_info_dto.py`

 * *Files identical despite different names*

### Comparing `yandex_api_client-0.0.1/yandex_api_client/models/offer_recommendations_result_dto.py` & `yandex_api_client-0.0.2/yandex_api_client/models/offer_recommendations_result_dto.py`

 * *Files identical despite different names*

### Comparing `yandex_api_client-0.0.1/yandex_api_client/models/offer_selling_program_dto.py` & `yandex_api_client-0.0.2/yandex_api_client/models/offer_selling_program_dto.py`

 * *Files identical despite different names*

### Comparing `yandex_api_client-0.0.1/yandex_api_client/models/offer_selling_program_status_type.py` & `yandex_api_client-0.0.2/yandex_api_client/models/offer_selling_program_status_type.py`

 * *Files identical despite different names*

### Comparing `yandex_api_client-0.0.1/yandex_api_client/models/offer_type.py` & `yandex_api_client-0.0.2/yandex_api_client/models/offer_type.py`

 * *Files identical despite different names*

### Comparing `yandex_api_client-0.0.1/yandex_api_client/models/offer_weight_dimensions_dto.py` & `yandex_api_client-0.0.2/yandex_api_client/models/offer_weight_dimensions_dto.py`

 * *Files 4% similar despite different names*

```diff
@@ -26,18 +26,18 @@
 except ImportError:
     from typing_extensions import Self
 
 class OfferWeightDimensionsDTO(BaseModel):
     """
     Габариты упаковки и вес товара.  Если товар занимает несколько коробок, перед измерением размеров сложите их компактно.  ![Схема измерения многоместных грузов](../../_images/reference/boxes-measure.png) 
     """ # noqa: E501
-    length: Union[StrictFloat, StrictInt] = Field(description="Длина упаковки в см. ")
-    width: Union[StrictFloat, StrictInt] = Field(description="Ширина упаковки в см. ")
-    height: Union[StrictFloat, StrictInt] = Field(description="Высота упаковки в см. ")
-    weight: Union[StrictFloat, StrictInt] = Field(description="Вес товара в кг с учетом упаковки (брутто). ")
+    length: Union[StrictFloat, StrictInt, None] = Field(description="Длина упаковки в см. ")
+    width: Union[StrictFloat, StrictInt, None] = Field(description="Ширина упаковки в см. ")
+    height: Union[StrictFloat, StrictInt, None] = Field(description="Высота упаковки в см. ")
+    weight: Union[StrictFloat, StrictInt, None] = Field(description="Вес товара в кг с учетом упаковки (брутто). ")
     __properties: ClassVar[List[str]] = ["length", "width", "height", "weight"]
 
     model_config = {
         "populate_by_name": True,
         "validate_assignment": True,
         "protected_namespaces": (),
     }
```

### Comparing `yandex_api_client-0.0.1/yandex_api_client/models/offers_dto.py` & `yandex_api_client-0.0.2/yandex_api_client/models/offers_dto.py`

 * *Files identical despite different names*

### Comparing `yandex_api_client-0.0.1/yandex_api_client/models/option_values_limited_dto.py` & `yandex_api_client-0.0.2/yandex_api_client/models/option_values_limited_dto.py`

 * *Files identical despite different names*

### Comparing `yandex_api_client-0.0.1/yandex_api_client/models/order_box_layout_dto.py` & `yandex_api_client-0.0.2/yandex_api_client/models/order_box_layout_dto.py`

 * *Files identical despite different names*

### Comparing `yandex_api_client-0.0.1/yandex_api_client/models/order_box_layout_item_dto.py` & `yandex_api_client-0.0.2/yandex_api_client/models/order_box_layout_item_dto.py`

 * *Files identical despite different names*

### Comparing `yandex_api_client-0.0.1/yandex_api_client/models/order_box_layout_partial_count_dto.py` & `yandex_api_client-0.0.2/yandex_api_client/models/order_box_layout_partial_count_dto.py`

 * *Files identical despite different names*

### Comparing `yandex_api_client-0.0.1/yandex_api_client/models/order_boxes_layout_dto.py` & `yandex_api_client-0.0.2/yandex_api_client/models/order_boxes_layout_dto.py`

 * *Files identical despite different names*

### Comparing `yandex_api_client-0.0.1/yandex_api_client/models/order_business_buyer_dto.py` & `yandex_api_client-0.0.2/yandex_api_client/models/order_business_buyer_dto.py`

 * *Files identical despite different names*

### Comparing `yandex_api_client-0.0.1/yandex_api_client/models/order_business_documents_dto.py` & `yandex_api_client-0.0.2/yandex_api_client/models/order_business_documents_dto.py`

 * *Files identical despite different names*

### Comparing `yandex_api_client-0.0.1/yandex_api_client/models/order_buyer_basic_info_dto.py` & `yandex_api_client-0.0.2/yandex_api_client/models/order_buyer_basic_info_dto.py`

 * *Files identical despite different names*

### Comparing `yandex_api_client-0.0.1/yandex_api_client/models/order_buyer_dto.py` & `yandex_api_client-0.0.2/yandex_api_client/models/order_buyer_dto.py`

 * *Files identical despite different names*

### Comparing `yandex_api_client-0.0.1/yandex_api_client/models/order_buyer_info_dto.py` & `yandex_api_client-0.0.2/yandex_api_client/models/order_buyer_info_dto.py`

 * *Files identical despite different names*

### Comparing `yandex_api_client-0.0.1/yandex_api_client/models/order_buyer_type.py` & `yandex_api_client-0.0.2/yandex_api_client/models/order_buyer_type.py`

 * *Files identical despite different names*

### Comparing `yandex_api_client-0.0.1/yandex_api_client/models/order_cancellation_reason_type.py` & `yandex_api_client-0.0.2/yandex_api_client/models/order_cancellation_reason_type.py`

 * *Files identical despite different names*

### Comparing `yandex_api_client-0.0.1/yandex_api_client/models/order_courier_dto.py` & `yandex_api_client-0.0.2/yandex_api_client/models/order_courier_dto.py`

 * *Files identical despite different names*

### Comparing `yandex_api_client-0.0.1/yandex_api_client/models/order_delivery_address_dto.py` & `yandex_api_client-0.0.2/yandex_api_client/models/order_delivery_address_dto.py`

 * *Files identical despite different names*

### Comparing `yandex_api_client-0.0.1/yandex_api_client/models/order_delivery_date_dto.py` & `yandex_api_client-0.0.2/yandex_api_client/models/order_delivery_date_dto.py`

 * *Files identical despite different names*

### Comparing `yandex_api_client-0.0.1/yandex_api_client/models/order_delivery_date_reason_type.py` & `yandex_api_client-0.0.2/yandex_api_client/models/order_delivery_date_reason_type.py`

 * *Files identical despite different names*

### Comparing `yandex_api_client-0.0.1/yandex_api_client/models/order_delivery_dates_dto.py` & `yandex_api_client-0.0.2/yandex_api_client/models/order_delivery_dates_dto.py`

 * *Files identical despite different names*

### Comparing `yandex_api_client-0.0.1/yandex_api_client/models/order_delivery_dispatch_type.py` & `yandex_api_client-0.0.2/yandex_api_client/models/order_delivery_dispatch_type.py`

 * *Files identical despite different names*

### Comparing `yandex_api_client-0.0.1/yandex_api_client/models/order_delivery_dto.py` & `yandex_api_client-0.0.2/yandex_api_client/models/order_delivery_dto.py`

 * *Files identical despite different names*

### Comparing `yandex_api_client-0.0.1/yandex_api_client/models/order_delivery_eac_type.py` & `yandex_api_client-0.0.2/yandex_api_client/models/order_delivery_eac_type.py`

 * *Files identical despite different names*

### Comparing `yandex_api_client-0.0.1/yandex_api_client/models/order_delivery_partner_type.py` & `yandex_api_client-0.0.2/yandex_api_client/models/order_delivery_partner_type.py`

 * *Files identical despite different names*

### Comparing `yandex_api_client-0.0.1/yandex_api_client/models/order_delivery_type.py` & `yandex_api_client-0.0.2/yandex_api_client/models/order_delivery_type.py`

 * *Files identical despite different names*

### Comparing `yandex_api_client-0.0.1/yandex_api_client/models/order_digital_item_dto.py` & `yandex_api_client-0.0.2/yandex_api_client/models/order_digital_item_dto.py`

 * *Files identical despite different names*

### Comparing `yandex_api_client-0.0.1/yandex_api_client/models/order_document_status_type.py` & `yandex_api_client-0.0.2/yandex_api_client/models/order_document_status_type.py`

 * *Files identical despite different names*

### Comparing `yandex_api_client-0.0.1/yandex_api_client/models/order_dto.py` & `yandex_api_client-0.0.2/yandex_api_client/models/order_dto.py`

 * *Files identical despite different names*

### Comparing `yandex_api_client-0.0.1/yandex_api_client/models/order_item_detail_dto.py` & `yandex_api_client-0.0.2/yandex_api_client/models/order_item_detail_dto.py`

 * *Files identical despite different names*

### Comparing `yandex_api_client-0.0.1/yandex_api_client/models/order_item_dto.py` & `yandex_api_client-0.0.2/yandex_api_client/models/order_item_dto.py`

 * *Files identical despite different names*

### Comparing `yandex_api_client-0.0.1/yandex_api_client/models/order_item_instance_dto.py` & `yandex_api_client-0.0.2/yandex_api_client/models/order_item_instance_dto.py`

 * *Files identical despite different names*

### Comparing `yandex_api_client-0.0.1/yandex_api_client/models/order_item_instance_modification_dto.py` & `yandex_api_client-0.0.2/yandex_api_client/models/order_item_instance_modification_dto.py`

 * *Files identical despite different names*

### Comparing `yandex_api_client-0.0.1/yandex_api_client/models/order_item_instance_type.py` & `yandex_api_client-0.0.2/yandex_api_client/models/order_item_instance_type.py`

 * *Files identical despite different names*

### Comparing `yandex_api_client-0.0.1/yandex_api_client/models/order_item_modification_dto.py` & `yandex_api_client-0.0.2/yandex_api_client/models/order_item_modification_dto.py`

 * *Files identical despite different names*

### Comparing `yandex_api_client-0.0.1/yandex_api_client/models/order_item_promo_dto.py` & `yandex_api_client-0.0.2/yandex_api_client/models/order_item_promo_dto.py`

 * *Files identical despite different names*

### Comparing `yandex_api_client-0.0.1/yandex_api_client/models/order_item_status_type.py` & `yandex_api_client-0.0.2/yandex_api_client/models/order_item_status_type.py`

 * *Files identical despite different names*

### Comparing `yandex_api_client-0.0.1/yandex_api_client/models/order_item_subsidy_dto.py` & `yandex_api_client-0.0.2/yandex_api_client/models/order_item_subsidy_dto.py`

 * *Files identical despite different names*

### Comparing `yandex_api_client-0.0.1/yandex_api_client/models/order_items_modification_request_reason_type.py` & `yandex_api_client-0.0.2/yandex_api_client/models/order_items_modification_request_reason_type.py`

 * *Files identical despite different names*

### Comparing `yandex_api_client-0.0.1/yandex_api_client/models/order_items_modification_result_dto.py` & `yandex_api_client-0.0.2/yandex_api_client/models/order_items_modification_result_dto.py`

 * *Files identical despite different names*

### Comparing `yandex_api_client-0.0.1/yandex_api_client/models/order_label_dto.py` & `yandex_api_client-0.0.2/yandex_api_client/models/order_label_dto.py`

 * *Files identical despite different names*

### Comparing `yandex_api_client-0.0.1/yandex_api_client/models/order_lift_type.py` & `yandex_api_client-0.0.2/yandex_api_client/models/order_lift_type.py`

 * *Files identical despite different names*

### Comparing `yandex_api_client-0.0.1/yandex_api_client/models/order_parcel_box_dto.py` & `yandex_api_client-0.0.2/yandex_api_client/models/order_parcel_box_dto.py`

 * *Files identical despite different names*

### Comparing `yandex_api_client-0.0.1/yandex_api_client/models/order_parcel_status_type.py` & `yandex_api_client-0.0.2/yandex_api_client/models/order_parcel_status_type.py`

 * *Files identical despite different names*

### Comparing `yandex_api_client-0.0.1/yandex_api_client/models/order_payment_method_type.py` & `yandex_api_client-0.0.2/yandex_api_client/models/order_payment_method_type.py`

 * *Files identical despite different names*

### Comparing `yandex_api_client-0.0.1/yandex_api_client/models/order_payment_type.py` & `yandex_api_client-0.0.2/yandex_api_client/models/order_payment_type.py`

 * *Files identical despite different names*

### Comparing `yandex_api_client-0.0.1/yandex_api_client/models/order_promo_type.py` & `yandex_api_client-0.0.2/yandex_api_client/models/order_promo_type.py`

 * *Files identical despite different names*

### Comparing `yandex_api_client-0.0.1/yandex_api_client/models/order_shipment_dto.py` & `yandex_api_client-0.0.2/yandex_api_client/models/order_shipment_dto.py`

 * *Files identical despite different names*

### Comparing `yandex_api_client-0.0.1/yandex_api_client/models/order_state_dto.py` & `yandex_api_client-0.0.2/yandex_api_client/models/order_state_dto.py`

 * *Files identical despite different names*

### Comparing `yandex_api_client-0.0.1/yandex_api_client/models/order_stats_status_type.py` & `yandex_api_client-0.0.2/yandex_api_client/models/order_stats_status_type.py`

 * *Files identical despite different names*

### Comparing `yandex_api_client-0.0.1/yandex_api_client/models/order_status_change_delivery_dates_dto.py` & `yandex_api_client-0.0.2/yandex_api_client/models/order_status_change_delivery_dates_dto.py`

 * *Files identical despite different names*

### Comparing `yandex_api_client-0.0.1/yandex_api_client/models/order_status_change_delivery_dto.py` & `yandex_api_client-0.0.2/yandex_api_client/models/order_status_change_delivery_dto.py`

 * *Files identical despite different names*

### Comparing `yandex_api_client-0.0.1/yandex_api_client/models/order_status_change_dto.py` & `yandex_api_client-0.0.2/yandex_api_client/models/order_status_change_dto.py`

 * *Files identical despite different names*

### Comparing `yandex_api_client-0.0.1/yandex_api_client/models/order_status_type.py` & `yandex_api_client-0.0.2/yandex_api_client/models/order_status_type.py`

 * *Files identical despite different names*

### Comparing `yandex_api_client-0.0.1/yandex_api_client/models/order_subsidy_type.py` & `yandex_api_client-0.0.2/yandex_api_client/models/order_subsidy_type.py`

 * *Files identical despite different names*

### Comparing `yandex_api_client-0.0.1/yandex_api_client/models/order_substatus_type.py` & `yandex_api_client-0.0.2/yandex_api_client/models/order_substatus_type.py`

 * *Files identical despite different names*

### Comparing `yandex_api_client-0.0.1/yandex_api_client/models/order_tax_system_type.py` & `yandex_api_client-0.0.2/yandex_api_client/models/order_tax_system_type.py`

 * *Files identical despite different names*

### Comparing `yandex_api_client-0.0.1/yandex_api_client/models/order_track_dto.py` & `yandex_api_client-0.0.2/yandex_api_client/models/order_track_dto.py`

 * *Files identical despite different names*

### Comparing `yandex_api_client-0.0.1/yandex_api_client/models/order_update_status_type.py` & `yandex_api_client-0.0.2/yandex_api_client/models/order_update_status_type.py`

 * *Files identical despite different names*

### Comparing `yandex_api_client-0.0.1/yandex_api_client/models/order_vat_type.py` & `yandex_api_client-0.0.2/yandex_api_client/models/order_vat_type.py`

 * *Files identical despite different names*

### Comparing `yandex_api_client-0.0.1/yandex_api_client/models/orders_shipment_info_dto.py` & `yandex_api_client-0.0.2/yandex_api_client/models/orders_shipment_info_dto.py`

 * *Files identical despite different names*

### Comparing `yandex_api_client-0.0.1/yandex_api_client/models/orders_stats_commission_dto.py` & `yandex_api_client-0.0.2/yandex_api_client/models/orders_stats_commission_dto.py`

 * *Files identical despite different names*

### Comparing `yandex_api_client-0.0.1/yandex_api_client/models/orders_stats_commission_type.py` & `yandex_api_client-0.0.2/yandex_api_client/models/orders_stats_commission_type.py`

 * *Files identical despite different names*

### Comparing `yandex_api_client-0.0.1/yandex_api_client/models/orders_stats_delivery_region_dto.py` & `yandex_api_client-0.0.2/yandex_api_client/models/orders_stats_delivery_region_dto.py`

 * *Files identical despite different names*

### Comparing `yandex_api_client-0.0.1/yandex_api_client/models/orders_stats_details_dto.py` & `yandex_api_client-0.0.2/yandex_api_client/models/orders_stats_details_dto.py`

 * *Files identical despite different names*

### Comparing `yandex_api_client-0.0.1/yandex_api_client/models/orders_stats_dto.py` & `yandex_api_client-0.0.2/yandex_api_client/models/orders_stats_dto.py`

 * *Files identical despite different names*

### Comparing `yandex_api_client-0.0.1/yandex_api_client/models/orders_stats_item_dto.py` & `yandex_api_client-0.0.2/yandex_api_client/models/orders_stats_item_dto.py`

 * *Files identical despite different names*

### Comparing `yandex_api_client-0.0.1/yandex_api_client/models/orders_stats_item_status_type.py` & `yandex_api_client-0.0.2/yandex_api_client/models/orders_stats_item_status_type.py`

 * *Files identical despite different names*

### Comparing `yandex_api_client-0.0.1/yandex_api_client/models/orders_stats_order_dto.py` & `yandex_api_client-0.0.2/yandex_api_client/models/orders_stats_order_dto.py`

 * *Files identical despite different names*

### Comparing `yandex_api_client-0.0.1/yandex_api_client/models/orders_stats_order_payment_type.py` & `yandex_api_client-0.0.2/yandex_api_client/models/orders_stats_order_payment_type.py`

 * *Files identical despite different names*

### Comparing `yandex_api_client-0.0.1/yandex_api_client/models/orders_stats_payment_dto.py` & `yandex_api_client-0.0.2/yandex_api_client/models/orders_stats_payment_dto.py`

 * *Files identical despite different names*

### Comparing `yandex_api_client-0.0.1/yandex_api_client/models/orders_stats_payment_order_dto.py` & `yandex_api_client-0.0.2/yandex_api_client/models/orders_stats_payment_order_dto.py`

 * *Files identical despite different names*

### Comparing `yandex_api_client-0.0.1/yandex_api_client/models/orders_stats_payment_source_type.py` & `yandex_api_client-0.0.2/yandex_api_client/models/orders_stats_payment_source_type.py`

 * *Files identical despite different names*

### Comparing `yandex_api_client-0.0.1/yandex_api_client/models/orders_stats_payment_type.py` & `yandex_api_client-0.0.2/yandex_api_client/models/orders_stats_payment_type.py`

 * *Files identical despite different names*

### Comparing `yandex_api_client-0.0.1/yandex_api_client/models/orders_stats_price_dto.py` & `yandex_api_client-0.0.2/yandex_api_client/models/orders_stats_price_dto.py`

 * *Files identical despite different names*

### Comparing `yandex_api_client-0.0.1/yandex_api_client/models/orders_stats_price_type.py` & `yandex_api_client-0.0.2/yandex_api_client/models/orders_stats_price_type.py`

 * *Files identical despite different names*

### Comparing `yandex_api_client-0.0.1/yandex_api_client/models/orders_stats_stock_type.py` & `yandex_api_client-0.0.2/yandex_api_client/models/orders_stats_stock_type.py`

 * *Files identical despite different names*

### Comparing `yandex_api_client-0.0.1/yandex_api_client/models/orders_stats_warehouse_dto.py` & `yandex_api_client-0.0.2/yandex_api_client/models/orders_stats_warehouse_dto.py`

 * *Files identical despite different names*

### Comparing `yandex_api_client-0.0.1/yandex_api_client/models/outlet_address_dto.py` & `yandex_api_client-0.0.2/yandex_api_client/models/outlet_address_dto.py`

 * *Files identical despite different names*

### Comparing `yandex_api_client-0.0.1/yandex_api_client/models/outlet_delivery_rule_dto.py` & `yandex_api_client-0.0.2/yandex_api_client/models/outlet_delivery_rule_dto.py`

 * *Files identical despite different names*

### Comparing `yandex_api_client-0.0.1/yandex_api_client/models/outlet_dto.py` & `yandex_api_client-0.0.2/yandex_api_client/models/outlet_dto.py`

 * *Files identical despite different names*

### Comparing `yandex_api_client-0.0.1/yandex_api_client/models/outlet_license_dto.py` & `yandex_api_client-0.0.2/yandex_api_client/models/outlet_license_dto.py`

 * *Files identical despite different names*

### Comparing `yandex_api_client-0.0.1/yandex_api_client/models/outlet_licenses_response_dto.py` & `yandex_api_client-0.0.2/yandex_api_client/models/outlet_licenses_response_dto.py`

 * *Files identical despite different names*

### Comparing `yandex_api_client-0.0.1/yandex_api_client/models/outlet_response_dto.py` & `yandex_api_client-0.0.2/yandex_api_client/models/outlet_response_dto.py`

 * *Files identical despite different names*

### Comparing `yandex_api_client-0.0.1/yandex_api_client/models/outlet_status_type.py` & `yandex_api_client-0.0.2/yandex_api_client/models/outlet_status_type.py`

 * *Files identical despite different names*

### Comparing `yandex_api_client-0.0.1/yandex_api_client/models/outlet_type.py` & `yandex_api_client-0.0.2/yandex_api_client/models/outlet_type.py`

 * *Files identical despite different names*

### Comparing `yandex_api_client-0.0.1/yandex_api_client/models/outlet_visibility_type.py` & `yandex_api_client-0.0.2/yandex_api_client/models/outlet_visibility_type.py`

 * *Files identical despite different names*

### Comparing `yandex_api_client-0.0.1/yandex_api_client/models/outlet_working_schedule_dto.py` & `yandex_api_client-0.0.2/yandex_api_client/models/outlet_working_schedule_dto.py`

 * *Files identical despite different names*

### Comparing `yandex_api_client-0.0.1/yandex_api_client/models/outlet_working_schedule_item_dto.py` & `yandex_api_client-0.0.2/yandex_api_client/models/outlet_working_schedule_item_dto.py`

 * *Files identical despite different names*

### Comparing `yandex_api_client-0.0.1/yandex_api_client/models/page_format_type.py` & `yandex_api_client-0.0.2/yandex_api_client/models/page_format_type.py`

 * *Files identical despite different names*

### Comparing `yandex_api_client-0.0.1/yandex_api_client/models/paged_returns_dto.py` & `yandex_api_client-0.0.2/yandex_api_client/models/paged_returns_dto.py`

 * *Files identical despite different names*

### Comparing `yandex_api_client-0.0.1/yandex_api_client/models/pallets_count_dto.py` & `yandex_api_client-0.0.2/yandex_api_client/models/pallets_count_dto.py`

 * *Files identical despite different names*

### Comparing `yandex_api_client-0.0.1/yandex_api_client/models/parameter_type.py` & `yandex_api_client-0.0.2/yandex_api_client/models/parameter_type.py`

 * *Files identical despite different names*

### Comparing `yandex_api_client-0.0.1/yandex_api_client/models/parameter_value_constraints_dto.py` & `yandex_api_client-0.0.2/yandex_api_client/models/parameter_value_constraints_dto.py`

 * *Files identical despite different names*

### Comparing `yandex_api_client-0.0.1/yandex_api_client/models/parameter_value_dto.py` & `yandex_api_client-0.0.2/yandex_api_client/models/parameter_value_dto.py`

 * *Files identical despite different names*

### Comparing `yandex_api_client-0.0.1/yandex_api_client/models/parameter_value_option_dto.py` & `yandex_api_client-0.0.2/yandex_api_client/models/parameter_value_option_dto.py`

 * *Files identical despite different names*

### Comparing `yandex_api_client-0.0.1/yandex_api_client/models/parcel_box_dto.py` & `yandex_api_client-0.0.2/yandex_api_client/models/parcel_box_dto.py`

 * *Files identical despite different names*

### Comparing `yandex_api_client-0.0.1/yandex_api_client/models/parcel_box_label_dto.py` & `yandex_api_client-0.0.2/yandex_api_client/models/parcel_box_label_dto.py`

 * *Files identical despite different names*

### Comparing `yandex_api_client-0.0.1/yandex_api_client/models/parcel_dto.py` & `yandex_api_client-0.0.2/yandex_api_client/models/parcel_dto.py`

 * *Files identical despite different names*

### Comparing `yandex_api_client-0.0.1/yandex_api_client/models/partner_shipment_warehouse_dto.py` & `yandex_api_client-0.0.2/yandex_api_client/models/partner_shipment_warehouse_dto.py`

 * *Files identical despite different names*

### Comparing `yandex_api_client-0.0.1/yandex_api_client/models/payment_frequency_type.py` & `yandex_api_client-0.0.2/yandex_api_client/models/payment_frequency_type.py`

 * *Files identical despite different names*

### Comparing `yandex_api_client-0.0.1/yandex_api_client/models/pickup_address_dto.py` & `yandex_api_client-0.0.2/yandex_api_client/models/pickup_address_dto.py`

 * *Files identical despite different names*

### Comparing `yandex_api_client-0.0.1/yandex_api_client/models/placement_type.py` & `yandex_api_client-0.0.2/yandex_api_client/models/placement_type.py`

 * *Files identical despite different names*

### Comparing `yandex_api_client-0.0.1/yandex_api_client/models/price_competitiveness_thresholds_dto.py` & `yandex_api_client-0.0.2/yandex_api_client/models/price_competitiveness_thresholds_dto.py`

 * *Files identical despite different names*

### Comparing `yandex_api_client-0.0.1/yandex_api_client/models/price_competitiveness_type.py` & `yandex_api_client-0.0.2/yandex_api_client/models/price_competitiveness_type.py`

 * *Files identical despite different names*

### Comparing `yandex_api_client-0.0.1/yandex_api_client/models/price_dto.py` & `yandex_api_client-0.0.2/yandex_api_client/models/price_dto.py`

 * *Files identical despite different names*

### Comparing `yandex_api_client-0.0.1/yandex_api_client/models/price_quarantine_verdict_dto.py` & `yandex_api_client-0.0.2/yandex_api_client/models/price_quarantine_verdict_dto.py`

 * *Files identical despite different names*

### Comparing `yandex_api_client-0.0.1/yandex_api_client/models/price_quarantine_verdict_param_name_type.py` & `yandex_api_client-0.0.2/yandex_api_client/models/price_quarantine_verdict_param_name_type.py`

 * *Files identical despite different names*

### Comparing `yandex_api_client-0.0.1/yandex_api_client/models/price_quarantine_verdict_parameter_dto.py` & `yandex_api_client-0.0.2/yandex_api_client/models/price_quarantine_verdict_parameter_dto.py`

 * *Files identical despite different names*

### Comparing `yandex_api_client-0.0.1/yandex_api_client/models/price_quarantine_verdict_type.py` & `yandex_api_client-0.0.2/yandex_api_client/models/price_quarantine_verdict_type.py`

 * *Files identical despite different names*

### Comparing `yandex_api_client-0.0.1/yandex_api_client/models/price_recommendation_item_dto.py` & `yandex_api_client-0.0.2/yandex_api_client/models/price_recommendation_item_dto.py`

 * *Files identical despite different names*

### Comparing `yandex_api_client-0.0.1/yandex_api_client/models/price_suggest_dto.py` & `yandex_api_client-0.0.2/yandex_api_client/models/price_suggest_dto.py`

 * *Files identical despite different names*

### Comparing `yandex_api_client-0.0.1/yandex_api_client/models/price_suggest_offer_dto.py` & `yandex_api_client-0.0.2/yandex_api_client/models/price_suggest_offer_dto.py`

 * *Files identical despite different names*

### Comparing `yandex_api_client-0.0.1/yandex_api_client/models/price_suggest_type.py` & `yandex_api_client-0.0.2/yandex_api_client/models/price_suggest_type.py`

 * *Files identical despite different names*

### Comparing `yandex_api_client-0.0.1/yandex_api_client/models/provide_order_digital_codes_request.py` & `yandex_api_client-0.0.2/yandex_api_client/models/provide_order_digital_codes_request.py`

 * *Files identical despite different names*

### Comparing `yandex_api_client-0.0.1/yandex_api_client/models/provide_order_item_identifiers_request.py` & `yandex_api_client-0.0.2/yandex_api_client/models/provide_order_item_identifiers_request.py`

 * *Files identical despite different names*

### Comparing `yandex_api_client-0.0.1/yandex_api_client/models/provide_order_item_identifiers_response.py` & `yandex_api_client-0.0.2/yandex_api_client/models/provide_order_item_identifiers_response.py`

 * *Files identical despite different names*

### Comparing `yandex_api_client-0.0.1/yandex_api_client/models/put_sku_bids_request.py` & `yandex_api_client-0.0.2/yandex_api_client/models/put_sku_bids_request.py`

 * *Files identical despite different names*

### Comparing `yandex_api_client-0.0.1/yandex_api_client/models/quantum_dto.py` & `yandex_api_client-0.0.2/yandex_api_client/models/quantum_dto.py`

 * *Files identical despite different names*

### Comparing `yandex_api_client-0.0.1/yandex_api_client/models/quarantine_offer_dto.py` & `yandex_api_client-0.0.2/yandex_api_client/models/quarantine_offer_dto.py`

 * *Files identical despite different names*

### Comparing `yandex_api_client-0.0.1/yandex_api_client/models/recipient_type.py` & `yandex_api_client-0.0.2/yandex_api_client/models/recipient_type.py`

 * *Files identical despite different names*

### Comparing `yandex_api_client-0.0.1/yandex_api_client/models/refund_status_type.py` & `yandex_api_client-0.0.2/yandex_api_client/models/refund_status_type.py`

 * *Files identical despite different names*

### Comparing `yandex_api_client-0.0.1/yandex_api_client/models/region_dto.py` & `yandex_api_client-0.0.2/yandex_api_client/models/region_dto.py`

 * *Files identical despite different names*

### Comparing `yandex_api_client-0.0.1/yandex_api_client/models/region_type.py` & `yandex_api_client-0.0.2/yandex_api_client/models/region_type.py`

 * *Files identical despite different names*

### Comparing `yandex_api_client-0.0.1/yandex_api_client/models/regional_model_info_dto.py` & `yandex_api_client-0.0.2/yandex_api_client/models/regional_model_info_dto.py`

 * *Files identical despite different names*

### Comparing `yandex_api_client-0.0.1/yandex_api_client/models/report_format_type.py` & `yandex_api_client-0.0.2/yandex_api_client/models/report_format_type.py`

 * *Files identical despite different names*

### Comparing `yandex_api_client-0.0.1/yandex_api_client/models/report_info_dto.py` & `yandex_api_client-0.0.2/yandex_api_client/models/report_info_dto.py`

 * *Files identical despite different names*

### Comparing `yandex_api_client-0.0.1/yandex_api_client/models/report_status_type.py` & `yandex_api_client-0.0.2/yandex_api_client/models/report_status_type.py`

 * *Files identical despite different names*

### Comparing `yandex_api_client-0.0.1/yandex_api_client/models/report_sub_status_type.py` & `yandex_api_client-0.0.2/yandex_api_client/models/report_sub_status_type.py`

 * *Files identical despite different names*

### Comparing `yandex_api_client-0.0.1/yandex_api_client/models/return_decision_dto.py` & `yandex_api_client-0.0.2/yandex_api_client/models/return_decision_dto.py`

 * *Files identical despite different names*

### Comparing `yandex_api_client-0.0.1/yandex_api_client/models/return_decision_reason_type.py` & `yandex_api_client-0.0.2/yandex_api_client/models/return_decision_reason_type.py`

 * *Files identical despite different names*

### Comparing `yandex_api_client-0.0.1/yandex_api_client/models/return_decision_subreason_type.py` & `yandex_api_client-0.0.2/yandex_api_client/models/return_decision_subreason_type.py`

 * *Files identical despite different names*

### Comparing `yandex_api_client-0.0.1/yandex_api_client/models/return_decision_type.py` & `yandex_api_client-0.0.2/yandex_api_client/models/return_decision_type.py`

 * *Files identical despite different names*

### Comparing `yandex_api_client-0.0.1/yandex_api_client/models/return_dto.py` & `yandex_api_client-0.0.2/yandex_api_client/models/return_dto.py`

 * *Files identical despite different names*

### Comparing `yandex_api_client-0.0.1/yandex_api_client/models/return_instance_dto.py` & `yandex_api_client-0.0.2/yandex_api_client/models/return_instance_dto.py`

 * *Files identical despite different names*

### Comparing `yandex_api_client-0.0.1/yandex_api_client/models/return_instance_status_type.py` & `yandex_api_client-0.0.2/yandex_api_client/models/return_instance_status_type.py`

 * *Files identical despite different names*

### Comparing `yandex_api_client-0.0.1/yandex_api_client/models/return_instance_stock_type.py` & `yandex_api_client-0.0.2/yandex_api_client/models/return_instance_stock_type.py`

 * *Files identical despite different names*

### Comparing `yandex_api_client-0.0.1/yandex_api_client/models/return_item_dto.py` & `yandex_api_client-0.0.2/yandex_api_client/models/return_item_dto.py`

 * *Files identical despite different names*

### Comparing `yandex_api_client-0.0.1/yandex_api_client/models/return_request_decision_type.py` & `yandex_api_client-0.0.2/yandex_api_client/models/return_request_decision_type.py`

 * *Files identical despite different names*

### Comparing `yandex_api_client-0.0.1/yandex_api_client/models/return_shipment_status_type.py` & `yandex_api_client-0.0.2/yandex_api_client/models/return_shipment_status_type.py`

 * *Files identical despite different names*

### Comparing `yandex_api_client-0.0.1/yandex_api_client/models/return_type.py` & `yandex_api_client-0.0.2/yandex_api_client/models/return_type.py`

 * *Files identical despite different names*

### Comparing `yandex_api_client-0.0.1/yandex_api_client/models/scrolling_pager_dto.py` & `yandex_api_client-0.0.2/yandex_api_client/models/scrolling_pager_dto.py`

 * *Files identical despite different names*

### Comparing `yandex_api_client-0.0.1/yandex_api_client/models/search_models_response.py` & `yandex_api_client-0.0.2/yandex_api_client/models/search_models_response.py`

 * *Files identical despite different names*

### Comparing `yandex_api_client-0.0.1/yandex_api_client/models/search_shipments_request.py` & `yandex_api_client-0.0.2/yandex_api_client/models/search_shipments_request.py`

 * *Files identical despite different names*

### Comparing `yandex_api_client-0.0.1/yandex_api_client/models/search_shipments_response.py` & `yandex_api_client-0.0.2/yandex_api_client/models/search_shipments_response.py`

 * *Files identical despite different names*

### Comparing `yandex_api_client-0.0.1/yandex_api_client/models/search_shipments_response_dto.py` & `yandex_api_client-0.0.2/yandex_api_client/models/search_shipments_response_dto.py`

 * *Files identical despite different names*

### Comparing `yandex_api_client-0.0.1/yandex_api_client/models/selling_program_type.py` & `yandex_api_client-0.0.2/yandex_api_client/models/selling_program_type.py`

 * *Files identical despite different names*

### Comparing `yandex_api_client-0.0.1/yandex_api_client/models/send_message_to_chat_request.py` & `yandex_api_client-0.0.2/yandex_api_client/models/send_message_to_chat_request.py`

 * *Files identical despite different names*

### Comparing `yandex_api_client-0.0.1/yandex_api_client/models/set_feed_params_request.py` & `yandex_api_client-0.0.2/yandex_api_client/models/set_feed_params_request.py`

 * *Files identical despite different names*

### Comparing `yandex_api_client-0.0.1/yandex_api_client/models/set_order_box_layout_request.py` & `yandex_api_client-0.0.2/yandex_api_client/models/set_order_box_layout_request.py`

 * *Files identical despite different names*

### Comparing `yandex_api_client-0.0.1/yandex_api_client/models/set_order_box_layout_response.py` & `yandex_api_client-0.0.2/yandex_api_client/models/set_order_box_layout_response.py`

 * *Files identical despite different names*

### Comparing `yandex_api_client-0.0.1/yandex_api_client/models/set_order_delivery_date_request.py` & `yandex_api_client-0.0.2/yandex_api_client/models/set_order_delivery_date_request.py`

 * *Files identical despite different names*

### Comparing `yandex_api_client-0.0.1/yandex_api_client/models/set_order_delivery_track_code_request.py` & `yandex_api_client-0.0.2/yandex_api_client/models/set_order_delivery_track_code_request.py`

 * *Files identical despite different names*

### Comparing `yandex_api_client-0.0.1/yandex_api_client/models/set_order_shipment_boxes_request.py` & `yandex_api_client-0.0.2/yandex_api_client/models/set_order_shipment_boxes_request.py`

 * *Files identical despite different names*

### Comparing `yandex_api_client-0.0.1/yandex_api_client/models/set_order_shipment_boxes_response.py` & `yandex_api_client-0.0.2/yandex_api_client/models/set_order_shipment_boxes_response.py`

 * *Files identical despite different names*

### Comparing `yandex_api_client-0.0.1/yandex_api_client/models/set_return_decision_request.py` & `yandex_api_client-0.0.2/yandex_api_client/models/set_return_decision_request.py`

 * *Files identical despite different names*

### Comparing `yandex_api_client-0.0.1/yandex_api_client/models/set_shipment_pallets_count_request.py` & `yandex_api_client-0.0.2/yandex_api_client/models/set_shipment_pallets_count_request.py`

 * *Files identical despite different names*

### Comparing `yandex_api_client-0.0.1/yandex_api_client/models/shipment_action_type.py` & `yandex_api_client-0.0.2/yandex_api_client/models/shipment_action_type.py`

 * *Files identical despite different names*

### Comparing `yandex_api_client-0.0.1/yandex_api_client/models/shipment_boxes_dto.py` & `yandex_api_client-0.0.2/yandex_api_client/models/shipment_boxes_dto.py`

 * *Files identical despite different names*

### Comparing `yandex_api_client-0.0.1/yandex_api_client/models/shipment_dto.py` & `yandex_api_client-0.0.2/yandex_api_client/models/shipment_dto.py`

 * *Files identical despite different names*

### Comparing `yandex_api_client-0.0.1/yandex_api_client/models/shipment_info_dto.py` & `yandex_api_client-0.0.2/yandex_api_client/models/shipment_info_dto.py`

 * *Files identical despite different names*

### Comparing `yandex_api_client-0.0.1/yandex_api_client/models/shipment_pallet_label_page_format_type.py` & `yandex_api_client-0.0.2/yandex_api_client/models/shipment_pallet_label_page_format_type.py`

 * *Files identical despite different names*

### Comparing `yandex_api_client-0.0.1/yandex_api_client/models/shipment_status_change_dto.py` & `yandex_api_client-0.0.2/yandex_api_client/models/shipment_status_change_dto.py`

 * *Files identical despite different names*

### Comparing `yandex_api_client-0.0.1/yandex_api_client/models/shipment_status_type.py` & `yandex_api_client-0.0.2/yandex_api_client/models/shipment_status_type.py`

 * *Files identical despite different names*

### Comparing `yandex_api_client-0.0.1/yandex_api_client/models/shipment_type.py` & `yandex_api_client-0.0.2/yandex_api_client/models/shipment_type.py`

 * *Files identical despite different names*

### Comparing `yandex_api_client-0.0.1/yandex_api_client/models/shows_sales_grouping_type.py` & `yandex_api_client-0.0.2/yandex_api_client/models/shows_sales_grouping_type.py`

 * *Files identical despite different names*

### Comparing `yandex_api_client-0.0.1/yandex_api_client/models/sku_bid_item_dto.py` & `yandex_api_client-0.0.2/yandex_api_client/models/sku_bid_item_dto.py`

 * *Files identical despite different names*

### Comparing `yandex_api_client-0.0.1/yandex_api_client/models/sku_bid_recommendation_item_dto.py` & `yandex_api_client-0.0.2/yandex_api_client/models/sku_bid_recommendation_item_dto.py`

 * *Files identical despite different names*

### Comparing `yandex_api_client-0.0.1/yandex_api_client/models/sort_order_type.py` & `yandex_api_client-0.0.2/yandex_api_client/models/sort_order_type.py`

 * *Files identical despite different names*

### Comparing `yandex_api_client-0.0.1/yandex_api_client/models/suggest_offer_price_dto.py` & `yandex_api_client-0.0.2/yandex_api_client/models/suggest_offer_price_dto.py`

 * *Files identical despite different names*

### Comparing `yandex_api_client-0.0.1/yandex_api_client/models/suggest_prices_request.py` & `yandex_api_client-0.0.2/yandex_api_client/models/suggest_prices_request.py`

 * *Files identical despite different names*

### Comparing `yandex_api_client-0.0.1/yandex_api_client/models/suggest_prices_response.py` & `yandex_api_client-0.0.2/yandex_api_client/models/suggest_prices_response.py`

 * *Files identical despite different names*

### Comparing `yandex_api_client-0.0.1/yandex_api_client/models/suggest_prices_result_dto.py` & `yandex_api_client-0.0.2/yandex_api_client/models/suggest_prices_result_dto.py`

 * *Files identical despite different names*

### Comparing `yandex_api_client-0.0.1/yandex_api_client/models/suggested_offer_dto.py` & `yandex_api_client-0.0.2/yandex_api_client/models/suggested_offer_dto.py`

 * *Files identical despite different names*

### Comparing `yandex_api_client-0.0.1/yandex_api_client/models/suggested_offer_mapping_dto.py` & `yandex_api_client-0.0.2/yandex_api_client/models/suggested_offer_mapping_dto.py`

 * *Files identical despite different names*

### Comparing `yandex_api_client-0.0.1/yandex_api_client/models/tariff_dto.py` & `yandex_api_client-0.0.2/yandex_api_client/models/tariff_dto.py`

 * *Files identical despite different names*

### Comparing `yandex_api_client-0.0.1/yandex_api_client/models/tariff_parameter_dto.py` & `yandex_api_client-0.0.2/yandex_api_client/models/tariff_parameter_dto.py`

 * *Files identical despite different names*

### Comparing `yandex_api_client-0.0.1/yandex_api_client/models/tariff_type.py` & `yandex_api_client-0.0.2/yandex_api_client/models/tariff_type.py`

 * *Files identical despite different names*

### Comparing `yandex_api_client-0.0.1/yandex_api_client/models/time_period_dto.py` & `yandex_api_client-0.0.2/yandex_api_client/models/time_period_dto.py`

 * *Files identical despite different names*

### Comparing `yandex_api_client-0.0.1/yandex_api_client/models/time_unit_type.py` & `yandex_api_client-0.0.2/yandex_api_client/models/time_unit_type.py`

 * *Files identical despite different names*

### Comparing `yandex_api_client-0.0.1/yandex_api_client/models/track_dto.py` & `yandex_api_client-0.0.2/yandex_api_client/models/track_dto.py`

 * *Files identical despite different names*

### Comparing `yandex_api_client-0.0.1/yandex_api_client/models/transfer_orders_from_shipment_request.py` & `yandex_api_client-0.0.2/yandex_api_client/models/transfer_orders_from_shipment_request.py`

 * *Files identical despite different names*

### Comparing `yandex_api_client-0.0.1/yandex_api_client/models/turnover_dto.py` & `yandex_api_client-0.0.2/yandex_api_client/models/turnover_dto.py`

 * *Files identical despite different names*

### Comparing `yandex_api_client-0.0.1/yandex_api_client/models/turnover_type.py` & `yandex_api_client-0.0.2/yandex_api_client/models/turnover_type.py`

 * *Files identical despite different names*

### Comparing `yandex_api_client-0.0.1/yandex_api_client/models/unit_dto.py` & `yandex_api_client-0.0.2/yandex_api_client/models/unit_dto.py`

 * *Files identical despite different names*

### Comparing `yandex_api_client-0.0.1/yandex_api_client/models/update_business_offer_price_dto.py` & `yandex_api_client-0.0.2/yandex_api_client/models/update_business_offer_price_dto.py`

 * *Files identical despite different names*

### Comparing `yandex_api_client-0.0.1/yandex_api_client/models/update_business_prices_request.py` & `yandex_api_client-0.0.2/yandex_api_client/models/update_business_prices_request.py`

 * *Files identical despite different names*

### Comparing `yandex_api_client-0.0.1/yandex_api_client/models/update_campaign_offer_dto.py` & `yandex_api_client-0.0.2/yandex_api_client/models/update_campaign_offer_dto.py`

 * *Files identical despite different names*

### Comparing `yandex_api_client-0.0.1/yandex_api_client/models/update_campaign_offers_request.py` & `yandex_api_client-0.0.2/yandex_api_client/models/update_campaign_offers_request.py`

 * *Files identical despite different names*

### Comparing `yandex_api_client-0.0.1/yandex_api_client/models/update_mapping_dto.py` & `yandex_api_client-0.0.2/yandex_api_client/models/update_mapping_dto.py`

 * *Files identical despite different names*

### Comparing `yandex_api_client-0.0.1/yandex_api_client/models/update_mappings_offer_dto.py` & `yandex_api_client-0.0.2/yandex_api_client/models/update_mappings_offer_dto.py`

 * *Files identical despite different names*

### Comparing `yandex_api_client-0.0.1/yandex_api_client/models/update_offer_content_request.py` & `yandex_api_client-0.0.2/yandex_api_client/models/update_offer_content_request.py`

 * *Files identical despite different names*

### Comparing `yandex_api_client-0.0.1/yandex_api_client/models/update_offer_content_response.py` & `yandex_api_client-0.0.2/yandex_api_client/models/update_offer_content_response.py`

 * *Files identical despite different names*

### Comparing `yandex_api_client-0.0.1/yandex_api_client/models/update_offer_content_result_dto.py` & `yandex_api_client-0.0.2/yandex_api_client/models/update_offer_content_result_dto.py`

 * *Files identical despite different names*

### Comparing `yandex_api_client-0.0.1/yandex_api_client/models/update_offer_dto.py` & `yandex_api_client-0.0.2/yandex_api_client/models/update_offer_dto.py`

 * *Files identical despite different names*

### Comparing `yandex_api_client-0.0.1/yandex_api_client/models/update_offer_mapping_dto.py` & `yandex_api_client-0.0.2/yandex_api_client/models/update_offer_mapping_dto.py`

 * *Files identical despite different names*

### Comparing `yandex_api_client-0.0.1/yandex_api_client/models/update_offer_mapping_entry_dto.py` & `yandex_api_client-0.0.2/yandex_api_client/models/update_offer_mapping_entry_dto.py`

 * *Files identical despite different names*

### Comparing `yandex_api_client-0.0.1/yandex_api_client/models/update_offer_mapping_entry_request.py` & `yandex_api_client-0.0.2/yandex_api_client/models/update_offer_mapping_entry_request.py`

 * *Files identical despite different names*

### Comparing `yandex_api_client-0.0.1/yandex_api_client/models/update_offer_mappings_request.py` & `yandex_api_client-0.0.2/yandex_api_client/models/update_offer_mappings_request.py`

 * *Files identical despite different names*

### Comparing `yandex_api_client-0.0.1/yandex_api_client/models/update_order_item_request.py` & `yandex_api_client-0.0.2/yandex_api_client/models/update_order_item_request.py`

 * *Files identical despite different names*

### Comparing `yandex_api_client-0.0.1/yandex_api_client/models/update_order_status_dto.py` & `yandex_api_client-0.0.2/yandex_api_client/models/update_order_status_dto.py`

 * *Files identical despite different names*

### Comparing `yandex_api_client-0.0.1/yandex_api_client/models/update_order_status_request.py` & `yandex_api_client-0.0.2/yandex_api_client/models/update_order_status_request.py`

 * *Files identical despite different names*

### Comparing `yandex_api_client-0.0.1/yandex_api_client/models/update_order_status_response.py` & `yandex_api_client-0.0.2/yandex_api_client/models/update_order_status_response.py`

 * *Files identical despite different names*

### Comparing `yandex_api_client-0.0.1/yandex_api_client/models/update_order_statuses_dto.py` & `yandex_api_client-0.0.2/yandex_api_client/models/update_order_statuses_dto.py`

 * *Files identical despite different names*

### Comparing `yandex_api_client-0.0.1/yandex_api_client/models/update_order_statuses_request.py` & `yandex_api_client-0.0.2/yandex_api_client/models/update_order_statuses_request.py`

 * *Files identical despite different names*

### Comparing `yandex_api_client-0.0.1/yandex_api_client/models/update_order_statuses_response.py` & `yandex_api_client-0.0.2/yandex_api_client/models/update_order_statuses_response.py`

 * *Files identical despite different names*

### Comparing `yandex_api_client-0.0.1/yandex_api_client/models/update_order_storage_limit_request.py` & `yandex_api_client-0.0.2/yandex_api_client/models/update_order_storage_limit_request.py`

 * *Files identical despite different names*

### Comparing `yandex_api_client-0.0.1/yandex_api_client/models/update_outlet_license_request.py` & `yandex_api_client-0.0.2/yandex_api_client/models/update_outlet_license_request.py`

 * *Files identical despite different names*

### Comparing `yandex_api_client-0.0.1/yandex_api_client/models/update_price_with_discount_dto.py` & `yandex_api_client-0.0.2/yandex_api_client/models/update_price_with_discount_dto.py`

 * *Files identical despite different names*

### Comparing `yandex_api_client-0.0.1/yandex_api_client/models/update_prices_request.py` & `yandex_api_client-0.0.2/yandex_api_client/models/update_prices_request.py`

 * *Files identical despite different names*

### Comparing `yandex_api_client-0.0.1/yandex_api_client/models/update_stock_dto.py` & `yandex_api_client-0.0.2/yandex_api_client/models/update_stock_dto.py`

 * *Files identical despite different names*

### Comparing `yandex_api_client-0.0.1/yandex_api_client/models/update_stock_item_dto.py` & `yandex_api_client-0.0.2/yandex_api_client/models/update_stock_item_dto.py`

 * *Files identical despite different names*

### Comparing `yandex_api_client-0.0.1/yandex_api_client/models/update_stocks_request.py` & `yandex_api_client-0.0.2/yandex_api_client/models/update_stocks_request.py`

 * *Files identical despite different names*

### Comparing `yandex_api_client-0.0.1/yandex_api_client/models/update_time_dto.py` & `yandex_api_client-0.0.2/yandex_api_client/models/update_time_dto.py`

 * *Files identical despite different names*

### Comparing `yandex_api_client-0.0.1/yandex_api_client/models/value_restriction_dto.py` & `yandex_api_client-0.0.2/yandex_api_client/models/value_restriction_dto.py`

 * *Files identical despite different names*

### Comparing `yandex_api_client-0.0.1/yandex_api_client/models/verify_order_eac_request.py` & `yandex_api_client-0.0.2/yandex_api_client/models/verify_order_eac_request.py`

 * *Files identical despite different names*

### Comparing `yandex_api_client-0.0.1/yandex_api_client/models/verify_order_eac_response.py` & `yandex_api_client-0.0.2/yandex_api_client/models/verify_order_eac_response.py`

 * *Files identical despite different names*

### Comparing `yandex_api_client-0.0.1/yandex_api_client/models/warehouse_address_dto.py` & `yandex_api_client-0.0.2/yandex_api_client/models/warehouse_address_dto.py`

 * *Files identical despite different names*

### Comparing `yandex_api_client-0.0.1/yandex_api_client/models/warehouse_dto.py` & `yandex_api_client-0.0.2/yandex_api_client/models/warehouse_dto.py`

 * *Files identical despite different names*

### Comparing `yandex_api_client-0.0.1/yandex_api_client/models/warehouse_group_dto.py` & `yandex_api_client-0.0.2/yandex_api_client/models/warehouse_group_dto.py`

 * *Files identical despite different names*

### Comparing `yandex_api_client-0.0.1/yandex_api_client/models/warehouse_offer_dto.py` & `yandex_api_client-0.0.2/yandex_api_client/models/warehouse_offer_dto.py`

 * *Files identical despite different names*

### Comparing `yandex_api_client-0.0.1/yandex_api_client/models/warehouse_offers_dto.py` & `yandex_api_client-0.0.2/yandex_api_client/models/warehouse_offers_dto.py`

 * *Files identical despite different names*

### Comparing `yandex_api_client-0.0.1/yandex_api_client/models/warehouse_stock_dto.py` & `yandex_api_client-0.0.2/yandex_api_client/models/warehouse_stock_dto.py`

 * *Files identical despite different names*

### Comparing `yandex_api_client-0.0.1/yandex_api_client/models/warehouse_stock_type.py` & `yandex_api_client-0.0.2/yandex_api_client/models/warehouse_stock_type.py`

 * *Files identical despite different names*

### Comparing `yandex_api_client-0.0.1/yandex_api_client/models/warehouses_dto.py` & `yandex_api_client-0.0.2/yandex_api_client/models/warehouses_dto.py`

 * *Files identical despite different names*

### Comparing `yandex_api_client-0.0.1/yandex_api_client/rest.py` & `yandex_api_client-0.0.2/yandex_api_client/rest.py`

 * *Files identical despite different names*

### Comparing `yandex_api_client-0.0.1/PKG-INFO` & `yandex_api_client-0.0.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: yandex_api_client
-Version: 0.0.1
+Version: 0.0.2
 Summary: 
 License: BSD 3-Clause
 Keywords: OpenAPI,OpenAPI-Generator,Партнерский API Маркета
 Author: OpenAPI Generator Community
 Author-email: team@openapitools.org
 Requires-Python: >=3.9,<4.0
 Classifier: License :: Other/Proprietary License
```

