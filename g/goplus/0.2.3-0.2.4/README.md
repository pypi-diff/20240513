# Comparing `tmp/goplus-0.2.3.tar.gz` & `tmp/goplus-0.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "goplus-0.2.3.tar", last modified: Wed Mar  6 09:46:09 2024, max compression
+gzip compressed data, was "goplus-0.2.4.tar", last modified: Mon May 13 04:08:06 2024, max compression
```

## Comparing `goplus-0.2.3.tar` & `goplus-0.2.4.tar`

### file list

```diff
@@ -1,108 +1,108 @@
-drwxr-xr-x   0 cong       (501) staff       (20)        0 2024-03-06 09:46:09.308618 goplus-0.2.3/
--rw-r--r--   0 cong       (501) staff       (20)    11357 2023-04-27 08:29:42.000000 goplus-0.2.3/LICENSE
--rw-r--r--   0 cong       (501) staff       (20)      837 2024-03-06 09:46:09.308458 goplus-0.2.3/PKG-INFO
--rw-r--r--   0 cong       (501) staff       (20)      359 2023-07-06 10:35:12.000000 goplus-0.2.3/README.md
-drwxr-xr-x   0 cong       (501) staff       (20)        0 2024-03-06 09:46:09.280644 goplus-0.2.3/goplus/
--rw-r--r--   0 cong       (501) staff       (20)      590 2023-05-30 08:01:30.000000 goplus-0.2.3/goplus/__init__.py
--rw-r--r--   0 cong       (501) staff       (20)      654 2024-03-06 09:44:59.000000 goplus-0.2.3/goplus/__version__.py
--rw-r--r--   0 cong       (501) staff       (20)     1135 2023-05-30 08:01:30.000000 goplus-0.2.3/goplus/address.py
--rw-r--r--   0 cong       (501) staff       (20)     2227 2023-05-30 08:01:30.000000 goplus-0.2.3/goplus/approve.py
--rw-r--r--   0 cong       (501) staff       (20)     1481 2023-05-30 08:01:30.000000 goplus-0.2.3/goplus/auth.py
--rw-r--r--   0 cong       (501) staff       (20)      840 2023-05-30 08:01:30.000000 goplus-0.2.3/goplus/base.py
--rw-r--r--   0 cong       (501) staff       (20)      864 2023-05-30 08:01:30.000000 goplus-0.2.3/goplus/chain.py
--rw-r--r--   0 cong       (501) staff       (20)      982 2023-05-30 08:01:30.000000 goplus-0.2.3/goplus/dapp.py
--rw-r--r--   0 cong       (501) staff       (20)     1302 2023-05-30 08:01:30.000000 goplus-0.2.3/goplus/decode.py
--rw-r--r--   0 cong       (501) staff       (20)     1096 2023-08-02 02:25:02.000000 goplus-0.2.3/goplus/errorcode.py
--rw-r--r--   0 cong       (501) staff       (20)     1092 2023-05-30 08:01:30.000000 goplus-0.2.3/goplus/nft.py
--rw-r--r--   0 cong       (501) staff       (20)     1002 2023-05-30 08:01:30.000000 goplus-0.2.3/goplus/phishing_site.py
--rw-r--r--   0 cong       (501) staff       (20)     1144 2023-05-30 08:01:30.000000 goplus-0.2.3/goplus/rug_pull.py
--rw-r--r--   0 cong       (501) staff       (20)     1453 2023-05-30 08:01:30.000000 goplus-0.2.3/goplus/token.py
-drwxr-xr-x   0 cong       (501) staff       (20)        0 2024-03-06 09:46:09.281171 goplus-0.2.3/goplus.egg-info/
--rw-r--r--   0 cong       (501) staff       (20)      837 2024-03-06 09:46:09.000000 goplus-0.2.3/goplus.egg-info/PKG-INFO
--rw-r--r--   0 cong       (501) staff       (20)     4877 2024-03-06 09:46:09.000000 goplus-0.2.3/goplus.egg-info/SOURCES.txt
--rw-r--r--   0 cong       (501) staff       (20)        1 2024-03-06 09:46:09.000000 goplus-0.2.3/goplus.egg-info/dependency_links.txt
--rw-r--r--   0 cong       (501) staff       (20)       67 2024-03-06 09:46:09.000000 goplus-0.2.3/goplus.egg-info/requires.txt
--rw-r--r--   0 cong       (501) staff       (20)       22 2024-03-06 09:46:09.000000 goplus-0.2.3/goplus.egg-info/top_level.txt
--rw-r--r--   0 cong       (501) staff       (20)       38 2024-03-06 09:46:09.308658 goplus-0.2.3/setup.cfg
--rw-r--r--   0 cong       (501) staff       (20)     3592 2023-05-10 02:53:37.000000 goplus-0.2.3/setup.py
-drwxr-xr-x   0 cong       (501) staff       (20)        0 2024-03-06 09:46:09.282379 goplus-0.2.3/swagger_client/
--rw-r--r--   0 cong       (501) staff       (20)     7669 2024-03-06 09:44:32.000000 goplus-0.2.3/swagger_client/__init__.py
-drwxr-xr-x   0 cong       (501) staff       (20)        0 2024-03-06 09:46:09.286086 goplus-0.2.3/swagger_client/api/
--rw-r--r--   0 cong       (501) staff       (20)      761 2023-05-30 06:06:21.000000 goplus-0.2.3/swagger_client/api/__init__.py
--rw-r--r--   0 cong       (501) staff       (20)    11079 2024-03-06 09:44:32.000000 goplus-0.2.3/swagger_client/api/approve_controller_v_1_api.py
--rw-r--r--   0 cong       (501) staff       (20)    16962 2023-08-02 02:06:01.000000 goplus-0.2.3/swagger_client/api/approve_controller_v_2_api.py
--rw-r--r--   0 cong       (501) staff       (20)     4979 2023-07-21 07:25:36.000000 goplus-0.2.3/swagger_client/api/contract_abi_controller_api.py
--rw-r--r--   0 cong       (501) staff       (20)     4469 2023-07-21 07:25:36.000000 goplus-0.2.3/swagger_client/api/dapp_controller_api.py
--rw-r--r--   0 cong       (501) staff       (20)     5546 2023-07-21 07:25:36.000000 goplus-0.2.3/swagger_client/api/defi_controller_api.py
--rw-r--r--   0 cong       (501) staff       (20)     6465 2023-12-25 06:28:36.000000 goplus-0.2.3/swagger_client/api/nft_controller_api.py
--rw-r--r--   0 cong       (501) staff       (20)     4282 2023-05-30 06:06:46.000000 goplus-0.2.3/swagger_client/api/token_controller_api.py
--rw-r--r--   0 cong       (501) staff       (20)    10216 2023-12-25 06:28:36.000000 goplus-0.2.3/swagger_client/api/token_controller_v_1_api.py
--rw-r--r--   0 cong       (501) staff       (20)     4724 2023-07-21 07:25:36.000000 goplus-0.2.3/swagger_client/api/website_controller_api.py
--rw-r--r--   0 cong       (501) staff       (20)    25084 2023-07-26 13:12:08.000000 goplus-0.2.3/swagger_client/api_client.py
--rw-r--r--   0 cong       (501) staff       (20)     8010 2023-12-29 08:47:36.000000 goplus-0.2.3/swagger_client/configuration.py
-drwxr-xr-x   0 cong       (501) staff       (20)        0 2024-03-06 09:46:09.307987 goplus-0.2.3/swagger_client/models/
--rw-r--r--   0 cong       (501) staff       (20)     6843 2024-03-06 09:44:32.000000 goplus-0.2.3/swagger_client/models/__init__.py
--rw-r--r--   0 cong       (501) staff       (20)     7936 2023-05-30 06:06:46.000000 goplus-0.2.3/swagger_client/models/abi_address_info.py
--rw-r--r--   0 cong       (501) staff       (20)     5536 2023-05-30 06:06:46.000000 goplus-0.2.3/swagger_client/models/abi_param_info.py
--rw-r--r--   0 cong       (501) staff       (20)    10427 2023-05-30 06:06:46.000000 goplus-0.2.3/swagger_client/models/approve_address_info.py
--rw-r--r--   0 cong       (501) staff       (20)     7889 2023-05-30 06:06:46.000000 goplus-0.2.3/swagger_client/models/approve_erc1155_result.py
--rw-r--r--   0 cong       (501) staff       (20)    10642 2023-05-30 06:06:46.000000 goplus-0.2.3/swagger_client/models/approve_nft1155_list_response.py
--rw-r--r--   0 cong       (501) staff       (20)    10461 2023-05-30 06:06:46.000000 goplus-0.2.3/swagger_client/models/approve_nft_list_response.py
--rw-r--r--   0 cong       (501) staff       (20)     9647 2023-05-30 06:06:46.000000 goplus-0.2.3/swagger_client/models/approve_result.py
--rw-r--r--   0 cong       (501) staff       (20)    11415 2023-05-30 06:06:46.000000 goplus-0.2.3/swagger_client/models/approve_token_out_list_response.py
--rw-r--r--   0 cong       (501) staff       (20)     8748 2023-05-30 06:06:46.000000 goplus-0.2.3/swagger_client/models/approve_token_result.py
--rw-r--r--   0 cong       (501) staff       (20)     4933 2023-05-30 06:06:46.000000 goplus-0.2.3/swagger_client/models/audit_info.py
--rw-r--r--   0 cong       (501) staff       (20)    15388 2023-07-21 07:25:36.000000 goplus-0.2.3/swagger_client/models/contract_approve_response.py
--rw-r--r--   0 cong       (501) staff       (20)    11564 2023-05-30 06:06:46.000000 goplus-0.2.3/swagger_client/models/contracts.py
--rw-r--r--   0 cong       (501) staff       (20)     4468 2023-05-30 06:06:46.000000 goplus-0.2.3/swagger_client/models/contracts_security.py
--rw-r--r--   0 cong       (501) staff       (20)     9038 2023-05-30 06:06:46.000000 goplus-0.2.3/swagger_client/models/dapp_contract_security_response.py
--rw-r--r--   0 cong       (501) staff       (20)     5549 2023-12-25 06:28:36.000000 goplus-0.2.3/swagger_client/models/get_access_token_request.py
--rw-r--r--   0 cong       (501) staff       (20)     4144 2023-05-30 06:06:46.000000 goplus-0.2.3/swagger_client/models/get_access_token_response.py
--rw-r--r--   0 cong       (501) staff       (20)     4617 2023-07-21 07:25:36.000000 goplus-0.2.3/swagger_client/models/get_defi_info_response.py
--rw-r--r--   0 cong       (501) staff       (20)    12268 2023-07-21 07:25:36.000000 goplus-0.2.3/swagger_client/models/get_defi_info_response_result.py
--rw-r--r--   0 cong       (501) staff       (20)     5765 2023-06-21 02:21:31.000000 goplus-0.2.3/swagger_client/models/get_defi_info_response_result_owner.py
--rw-r--r--   0 cong       (501) staff       (20)     2684 2023-05-30 06:06:46.000000 goplus-0.2.3/swagger_client/models/json_object.py
--rw-r--r--   0 cong       (501) staff       (20)     2704 2023-06-21 02:21:31.000000 goplus-0.2.3/swagger_client/models/map_string_string.py
--rw-r--r--   0 cong       (501) staff       (20)     8209 2023-05-30 06:06:46.000000 goplus-0.2.3/swagger_client/models/parse_abi_data_request.py
--rw-r--r--   0 cong       (501) staff       (20)    10371 2023-05-30 06:06:46.000000 goplus-0.2.3/swagger_client/models/parse_abi_data_response.py
--rw-r--r--   0 cong       (501) staff       (20)     4826 2023-07-21 07:25:36.000000 goplus-0.2.3/swagger_client/models/response_wrapper_address_contract.py
--rw-r--r--   0 cong       (501) staff       (20)    23056 2023-07-21 07:25:36.000000 goplus-0.2.3/swagger_client/models/response_wrapper_address_contract_result.py
--rw-r--r--   0 cong       (501) staff       (20)     4915 2023-07-21 07:25:36.000000 goplus-0.2.3/swagger_client/models/response_wrapper_contract_approve_response.py
--rw-r--r--   0 cong       (501) staff       (20)     5010 2023-07-21 07:25:36.000000 goplus-0.2.3/swagger_client/models/response_wrapper_dapp_contract_security_response.py
--rw-r--r--   0 cong       (501) staff       (20)     4896 2023-07-21 07:25:36.000000 goplus-0.2.3/swagger_client/models/response_wrapper_get_access_token_response.py
--rw-r--r--   0 cong       (501) staff       (20)     4731 2023-07-21 07:25:36.000000 goplus-0.2.3/swagger_client/models/response_wrapper_get_nft_info.py
--rw-r--r--   0 cong       (501) staff       (20)    42512 2023-07-21 07:25:36.000000 goplus-0.2.3/swagger_client/models/response_wrapper_get_nft_info_result.py
--rw-r--r--   0 cong       (501) staff       (20)     7031 2023-05-30 06:06:46.000000 goplus-0.2.3/swagger_client/models/response_wrapper_get_nft_info_result_privileged_burn.py
--rw-r--r--   0 cong       (501) staff       (20)     7079 2023-05-30 06:06:46.000000 goplus-0.2.3/swagger_client/models/response_wrapper_get_nft_info_result_privileged_minting.py
--rw-r--r--   0 cong       (501) staff       (20)     7605 2023-05-30 06:06:46.000000 goplus-0.2.3/swagger_client/models/response_wrapper_get_nft_info_result_same_nfts.py
--rw-r--r--   0 cong       (501) staff       (20)     6999 2023-05-30 06:06:46.000000 goplus-0.2.3/swagger_client/models/response_wrapper_get_nft_info_result_self_destruct.py
--rw-r--r--   0 cong       (501) staff       (20)     7175 2023-05-30 06:06:46.000000 goplus-0.2.3/swagger_client/models/response_wrapper_get_nft_info_result_transfer_without_approval.py
--rw-r--r--   0 cong       (501) staff       (20)     4765 2023-07-21 07:25:36.000000 goplus-0.2.3/swagger_client/models/response_wrapper_json_object.py
--rw-r--r--   0 cong       (501) staff       (20)     5130 2023-07-21 07:25:36.000000 goplus-0.2.3/swagger_client/models/response_wrapper_list_approve_nft1155_list_response.py
--rw-r--r--   0 cong       (501) staff       (20)     5054 2023-07-21 07:25:36.000000 goplus-0.2.3/swagger_client/models/response_wrapper_list_approve_nft_list_response.py
--rw-r--r--   0 cong       (501) staff       (20)     5149 2023-07-21 07:25:36.000000 goplus-0.2.3/swagger_client/models/response_wrapper_list_approve_token_out_list_response.py
--rw-r--r--   0 cong       (501) staff       (20)     4958 2023-07-21 07:25:36.000000 goplus-0.2.3/swagger_client/models/response_wrapper_list_get_chains_list.py
--rw-r--r--   0 cong       (501) staff       (20)     4008 2023-05-30 06:06:46.000000 goplus-0.2.3/swagger_client/models/response_wrapper_list_get_chains_list_result.py
--rw-r--r--   0 cong       (501) staff       (20)     4826 2023-07-21 07:25:36.000000 goplus-0.2.3/swagger_client/models/response_wrapper_list_json_object.py
--rw-r--r--   0 cong       (501) staff       (20)     4836 2023-07-21 07:25:36.000000 goplus-0.2.3/swagger_client/models/response_wrapper_map_string_string.py
--rw-r--r--   0 cong       (501) staff       (20)     4858 2023-07-21 07:25:36.000000 goplus-0.2.3/swagger_client/models/response_wrapper_parse_abi_data_response.py
--rw-r--r--   0 cong       (501) staff       (20)     4771 2024-03-06 09:44:32.000000 goplus-0.2.3/swagger_client/models/response_wrapper_phishing_site.py
--rw-r--r--   0 cong       (501) staff       (20)     4957 2024-03-06 09:44:32.000000 goplus-0.2.3/swagger_client/models/response_wrapper_phishing_site_result.py
--rw-r--r--   0 cong       (501) staff       (20)    13698 2024-03-06 09:44:32.000000 goplus-0.2.3/swagger_client/models/response_wrapper_phishing_site_result_nft_risk.py
--rw-r--r--   0 cong       (501) staff       (20)     7173 2024-03-06 09:44:32.000000 goplus-0.2.3/swagger_client/models/response_wrapper_phishing_site_result_nft_risk_privileged_burn.py
--rw-r--r--   0 cong       (501) staff       (20)     7221 2024-03-06 09:44:32.000000 goplus-0.2.3/swagger_client/models/response_wrapper_phishing_site_result_nft_risk_privileged_minting.py
--rw-r--r--   0 cong       (501) staff       (20)     7141 2024-03-06 09:44:32.000000 goplus-0.2.3/swagger_client/models/response_wrapper_phishing_site_result_nft_risk_self_destruct.py
--rw-r--r--   0 cong       (501) staff       (20)     7317 2024-03-06 09:44:32.000000 goplus-0.2.3/swagger_client/models/response_wrapper_phishing_site_result_nft_risk_transfer_without_approval.py
--rw-r--r--   0 cong       (501) staff       (20)     9081 2024-03-06 09:44:32.000000 goplus-0.2.3/swagger_client/models/response_wrapper_phishing_site_result_website_contract_security.py
--rw-r--r--   0 cong       (501) staff       (20)     4915 2023-07-21 07:25:36.000000 goplus-0.2.3/swagger_client/models/response_wrapper_ta_token_security_response.py
--rw-r--r--   0 cong       (501) staff       (20)     4897 2023-07-21 07:25:36.000000 goplus-0.2.3/swagger_client/models/response_wrapper_token_security.py
--rw-r--r--   0 cong       (501) staff       (20)     4905 2023-05-30 06:06:46.000000 goplus-0.2.3/swagger_client/models/response_wrapper_token_security_dex.py
--rw-r--r--   0 cong       (501) staff       (20)     5264 2023-12-25 06:28:36.000000 goplus-0.2.3/swagger_client/models/response_wrapper_token_security_fake_token.py
--rw-r--r--   0 cong       (501) staff       (20)    10002 2023-12-25 06:28:36.000000 goplus-0.2.3/swagger_client/models/response_wrapper_token_security_holders.py
--rw-r--r--   0 cong       (501) staff       (20)     5269 2023-07-06 10:45:21.000000 goplus-0.2.3/swagger_client/models/response_wrapper_token_security_locked_detail.py
--rw-r--r--   0 cong       (501) staff       (20)    11049 2023-12-25 06:28:36.000000 goplus-0.2.3/swagger_client/models/response_wrapper_token_security_lp_holders.py
--rw-r--r--   0 cong       (501) staff       (20)     7453 2023-12-25 08:27:53.000000 goplus-0.2.3/swagger_client/models/response_wrapper_token_security_nft_list.py
--rw-r--r--   0 cong       (501) staff       (20)    72566 2023-12-25 06:28:36.000000 goplus-0.2.3/swagger_client/models/response_wrapper_token_security_result.py
--rw-r--r--   0 cong       (501) staff       (20)     4668 2023-07-21 07:25:36.000000 goplus-0.2.3/swagger_client/models/response_wrapperobject.py
--rw-r--r--   0 cong       (501) staff       (20)     3194 2023-05-30 06:06:46.000000 goplus-0.2.3/swagger_client/models/ta_token_security_response.py
--rw-r--r--   0 cong       (501) staff       (20)    13036 2023-05-30 06:06:46.000000 goplus-0.2.3/swagger_client/rest.py
+drwxr-xr-x   0 cong       (501) staff       (20)        0 2024-05-13 04:08:06.607703 goplus-0.2.4/
+-rw-r--r--   0 cong       (501) staff       (20)    11357 2023-04-27 08:29:42.000000 goplus-0.2.4/LICENSE
+-rw-r--r--   0 cong       (501) staff       (20)      837 2024-05-13 04:08:06.607511 goplus-0.2.4/PKG-INFO
+-rw-r--r--   0 cong       (501) staff       (20)      359 2023-07-06 10:35:12.000000 goplus-0.2.4/README.md
+drwxr-xr-x   0 cong       (501) staff       (20)        0 2024-05-13 04:08:06.578584 goplus-0.2.4/goplus/
+-rw-r--r--   0 cong       (501) staff       (20)      590 2023-05-30 08:01:30.000000 goplus-0.2.4/goplus/__init__.py
+-rw-r--r--   0 cong       (501) staff       (20)      654 2024-05-13 04:07:19.000000 goplus-0.2.4/goplus/__version__.py
+-rw-r--r--   0 cong       (501) staff       (20)     1135 2023-05-30 08:01:30.000000 goplus-0.2.4/goplus/address.py
+-rw-r--r--   0 cong       (501) staff       (20)     2227 2023-05-30 08:01:30.000000 goplus-0.2.4/goplus/approve.py
+-rw-r--r--   0 cong       (501) staff       (20)     1481 2023-05-30 08:01:30.000000 goplus-0.2.4/goplus/auth.py
+-rw-r--r--   0 cong       (501) staff       (20)      840 2023-05-30 08:01:30.000000 goplus-0.2.4/goplus/base.py
+-rw-r--r--   0 cong       (501) staff       (20)      864 2023-05-30 08:01:30.000000 goplus-0.2.4/goplus/chain.py
+-rw-r--r--   0 cong       (501) staff       (20)      982 2023-05-30 08:01:30.000000 goplus-0.2.4/goplus/dapp.py
+-rw-r--r--   0 cong       (501) staff       (20)     1302 2023-05-30 08:01:30.000000 goplus-0.2.4/goplus/decode.py
+-rw-r--r--   0 cong       (501) staff       (20)     1096 2023-08-02 02:25:02.000000 goplus-0.2.4/goplus/errorcode.py
+-rw-r--r--   0 cong       (501) staff       (20)     1092 2023-05-30 08:01:30.000000 goplus-0.2.4/goplus/nft.py
+-rw-r--r--   0 cong       (501) staff       (20)     1002 2023-05-30 08:01:30.000000 goplus-0.2.4/goplus/phishing_site.py
+-rw-r--r--   0 cong       (501) staff       (20)     1144 2023-05-30 08:01:30.000000 goplus-0.2.4/goplus/rug_pull.py
+-rw-r--r--   0 cong       (501) staff       (20)     1453 2023-05-30 08:01:30.000000 goplus-0.2.4/goplus/token.py
+drwxr-xr-x   0 cong       (501) staff       (20)        0 2024-05-13 04:08:06.579140 goplus-0.2.4/goplus.egg-info/
+-rw-r--r--   0 cong       (501) staff       (20)      837 2024-05-13 04:08:06.000000 goplus-0.2.4/goplus.egg-info/PKG-INFO
+-rw-r--r--   0 cong       (501) staff       (20)     4877 2024-05-13 04:08:06.000000 goplus-0.2.4/goplus.egg-info/SOURCES.txt
+-rw-r--r--   0 cong       (501) staff       (20)        1 2024-05-13 04:08:06.000000 goplus-0.2.4/goplus.egg-info/dependency_links.txt
+-rw-r--r--   0 cong       (501) staff       (20)       67 2024-05-13 04:08:06.000000 goplus-0.2.4/goplus.egg-info/requires.txt
+-rw-r--r--   0 cong       (501) staff       (20)       22 2024-05-13 04:08:06.000000 goplus-0.2.4/goplus.egg-info/top_level.txt
+-rw-r--r--   0 cong       (501) staff       (20)       38 2024-05-13 04:08:06.607746 goplus-0.2.4/setup.cfg
+-rw-r--r--   0 cong       (501) staff       (20)     3592 2023-05-10 02:53:37.000000 goplus-0.2.4/setup.py
+drwxr-xr-x   0 cong       (501) staff       (20)        0 2024-05-13 04:08:06.581297 goplus-0.2.4/swagger_client/
+-rw-r--r--   0 cong       (501) staff       (20)     7669 2024-03-06 09:44:32.000000 goplus-0.2.4/swagger_client/__init__.py
+drwxr-xr-x   0 cong       (501) staff       (20)        0 2024-05-13 04:08:06.584641 goplus-0.2.4/swagger_client/api/
+-rw-r--r--   0 cong       (501) staff       (20)      761 2023-05-30 06:06:21.000000 goplus-0.2.4/swagger_client/api/__init__.py
+-rw-r--r--   0 cong       (501) staff       (20)    11079 2024-03-06 09:44:32.000000 goplus-0.2.4/swagger_client/api/approve_controller_v_1_api.py
+-rw-r--r--   0 cong       (501) staff       (20)    16962 2023-08-02 02:06:01.000000 goplus-0.2.4/swagger_client/api/approve_controller_v_2_api.py
+-rw-r--r--   0 cong       (501) staff       (20)     4979 2023-07-21 07:25:36.000000 goplus-0.2.4/swagger_client/api/contract_abi_controller_api.py
+-rw-r--r--   0 cong       (501) staff       (20)     4469 2023-07-21 07:25:36.000000 goplus-0.2.4/swagger_client/api/dapp_controller_api.py
+-rw-r--r--   0 cong       (501) staff       (20)     5546 2023-07-21 07:25:36.000000 goplus-0.2.4/swagger_client/api/defi_controller_api.py
+-rw-r--r--   0 cong       (501) staff       (20)     6465 2023-12-25 06:28:36.000000 goplus-0.2.4/swagger_client/api/nft_controller_api.py
+-rw-r--r--   0 cong       (501) staff       (20)     4282 2023-05-30 06:06:46.000000 goplus-0.2.4/swagger_client/api/token_controller_api.py
+-rw-r--r--   0 cong       (501) staff       (20)    10216 2023-12-25 06:28:36.000000 goplus-0.2.4/swagger_client/api/token_controller_v_1_api.py
+-rw-r--r--   0 cong       (501) staff       (20)     4724 2023-07-21 07:25:36.000000 goplus-0.2.4/swagger_client/api/website_controller_api.py
+-rw-r--r--   0 cong       (501) staff       (20)    25084 2023-07-26 13:12:08.000000 goplus-0.2.4/swagger_client/api_client.py
+-rw-r--r--   0 cong       (501) staff       (20)     8010 2023-12-29 08:47:36.000000 goplus-0.2.4/swagger_client/configuration.py
+drwxr-xr-x   0 cong       (501) staff       (20)        0 2024-05-13 04:08:06.606760 goplus-0.2.4/swagger_client/models/
+-rw-r--r--   0 cong       (501) staff       (20)     6843 2024-03-06 09:44:32.000000 goplus-0.2.4/swagger_client/models/__init__.py
+-rw-r--r--   0 cong       (501) staff       (20)     7936 2023-05-30 06:06:46.000000 goplus-0.2.4/swagger_client/models/abi_address_info.py
+-rw-r--r--   0 cong       (501) staff       (20)     5536 2023-05-30 06:06:46.000000 goplus-0.2.4/swagger_client/models/abi_param_info.py
+-rw-r--r--   0 cong       (501) staff       (20)    10427 2023-05-30 06:06:46.000000 goplus-0.2.4/swagger_client/models/approve_address_info.py
+-rw-r--r--   0 cong       (501) staff       (20)     7889 2023-05-30 06:06:46.000000 goplus-0.2.4/swagger_client/models/approve_erc1155_result.py
+-rw-r--r--   0 cong       (501) staff       (20)    10642 2023-05-30 06:06:46.000000 goplus-0.2.4/swagger_client/models/approve_nft1155_list_response.py
+-rw-r--r--   0 cong       (501) staff       (20)    10461 2023-05-30 06:06:46.000000 goplus-0.2.4/swagger_client/models/approve_nft_list_response.py
+-rw-r--r--   0 cong       (501) staff       (20)     9647 2023-05-30 06:06:46.000000 goplus-0.2.4/swagger_client/models/approve_result.py
+-rw-r--r--   0 cong       (501) staff       (20)    11415 2023-05-30 06:06:46.000000 goplus-0.2.4/swagger_client/models/approve_token_out_list_response.py
+-rw-r--r--   0 cong       (501) staff       (20)     8748 2023-05-30 06:06:46.000000 goplus-0.2.4/swagger_client/models/approve_token_result.py
+-rw-r--r--   0 cong       (501) staff       (20)     4933 2023-05-30 06:06:46.000000 goplus-0.2.4/swagger_client/models/audit_info.py
+-rw-r--r--   0 cong       (501) staff       (20)    15388 2023-07-21 07:25:36.000000 goplus-0.2.4/swagger_client/models/contract_approve_response.py
+-rw-r--r--   0 cong       (501) staff       (20)    11564 2023-05-30 06:06:46.000000 goplus-0.2.4/swagger_client/models/contracts.py
+-rw-r--r--   0 cong       (501) staff       (20)     4468 2023-05-30 06:06:46.000000 goplus-0.2.4/swagger_client/models/contracts_security.py
+-rw-r--r--   0 cong       (501) staff       (20)     9038 2023-05-30 06:06:46.000000 goplus-0.2.4/swagger_client/models/dapp_contract_security_response.py
+-rw-r--r--   0 cong       (501) staff       (20)     5549 2023-12-25 06:28:36.000000 goplus-0.2.4/swagger_client/models/get_access_token_request.py
+-rw-r--r--   0 cong       (501) staff       (20)     4144 2023-05-30 06:06:46.000000 goplus-0.2.4/swagger_client/models/get_access_token_response.py
+-rw-r--r--   0 cong       (501) staff       (20)     4617 2023-07-21 07:25:36.000000 goplus-0.2.4/swagger_client/models/get_defi_info_response.py
+-rw-r--r--   0 cong       (501) staff       (20)    12268 2023-07-21 07:25:36.000000 goplus-0.2.4/swagger_client/models/get_defi_info_response_result.py
+-rw-r--r--   0 cong       (501) staff       (20)     5765 2023-06-21 02:21:31.000000 goplus-0.2.4/swagger_client/models/get_defi_info_response_result_owner.py
+-rw-r--r--   0 cong       (501) staff       (20)     2684 2023-05-30 06:06:46.000000 goplus-0.2.4/swagger_client/models/json_object.py
+-rw-r--r--   0 cong       (501) staff       (20)     2704 2023-06-21 02:21:31.000000 goplus-0.2.4/swagger_client/models/map_string_string.py
+-rw-r--r--   0 cong       (501) staff       (20)     8209 2023-05-30 06:06:46.000000 goplus-0.2.4/swagger_client/models/parse_abi_data_request.py
+-rw-r--r--   0 cong       (501) staff       (20)    10371 2023-05-30 06:06:46.000000 goplus-0.2.4/swagger_client/models/parse_abi_data_response.py
+-rw-r--r--   0 cong       (501) staff       (20)     4826 2023-07-21 07:25:36.000000 goplus-0.2.4/swagger_client/models/response_wrapper_address_contract.py
+-rw-r--r--   0 cong       (501) staff       (20)    27828 2024-05-13 04:07:10.000000 goplus-0.2.4/swagger_client/models/response_wrapper_address_contract_result.py
+-rw-r--r--   0 cong       (501) staff       (20)     4915 2023-07-21 07:25:36.000000 goplus-0.2.4/swagger_client/models/response_wrapper_contract_approve_response.py
+-rw-r--r--   0 cong       (501) staff       (20)     5010 2023-07-21 07:25:36.000000 goplus-0.2.4/swagger_client/models/response_wrapper_dapp_contract_security_response.py
+-rw-r--r--   0 cong       (501) staff       (20)     4896 2023-07-21 07:25:36.000000 goplus-0.2.4/swagger_client/models/response_wrapper_get_access_token_response.py
+-rw-r--r--   0 cong       (501) staff       (20)     4731 2023-07-21 07:25:36.000000 goplus-0.2.4/swagger_client/models/response_wrapper_get_nft_info.py
+-rw-r--r--   0 cong       (501) staff       (20)    42512 2023-07-21 07:25:36.000000 goplus-0.2.4/swagger_client/models/response_wrapper_get_nft_info_result.py
+-rw-r--r--   0 cong       (501) staff       (20)     7031 2023-05-30 06:06:46.000000 goplus-0.2.4/swagger_client/models/response_wrapper_get_nft_info_result_privileged_burn.py
+-rw-r--r--   0 cong       (501) staff       (20)     7079 2023-05-30 06:06:46.000000 goplus-0.2.4/swagger_client/models/response_wrapper_get_nft_info_result_privileged_minting.py
+-rw-r--r--   0 cong       (501) staff       (20)     7605 2023-05-30 06:06:46.000000 goplus-0.2.4/swagger_client/models/response_wrapper_get_nft_info_result_same_nfts.py
+-rw-r--r--   0 cong       (501) staff       (20)     6999 2023-05-30 06:06:46.000000 goplus-0.2.4/swagger_client/models/response_wrapper_get_nft_info_result_self_destruct.py
+-rw-r--r--   0 cong       (501) staff       (20)     7175 2023-05-30 06:06:46.000000 goplus-0.2.4/swagger_client/models/response_wrapper_get_nft_info_result_transfer_without_approval.py
+-rw-r--r--   0 cong       (501) staff       (20)     4765 2023-07-21 07:25:36.000000 goplus-0.2.4/swagger_client/models/response_wrapper_json_object.py
+-rw-r--r--   0 cong       (501) staff       (20)     5130 2023-07-21 07:25:36.000000 goplus-0.2.4/swagger_client/models/response_wrapper_list_approve_nft1155_list_response.py
+-rw-r--r--   0 cong       (501) staff       (20)     5054 2023-07-21 07:25:36.000000 goplus-0.2.4/swagger_client/models/response_wrapper_list_approve_nft_list_response.py
+-rw-r--r--   0 cong       (501) staff       (20)     5149 2023-07-21 07:25:36.000000 goplus-0.2.4/swagger_client/models/response_wrapper_list_approve_token_out_list_response.py
+-rw-r--r--   0 cong       (501) staff       (20)     4958 2023-07-21 07:25:36.000000 goplus-0.2.4/swagger_client/models/response_wrapper_list_get_chains_list.py
+-rw-r--r--   0 cong       (501) staff       (20)     4008 2023-05-30 06:06:46.000000 goplus-0.2.4/swagger_client/models/response_wrapper_list_get_chains_list_result.py
+-rw-r--r--   0 cong       (501) staff       (20)     4826 2023-07-21 07:25:36.000000 goplus-0.2.4/swagger_client/models/response_wrapper_list_json_object.py
+-rw-r--r--   0 cong       (501) staff       (20)     4836 2023-07-21 07:25:36.000000 goplus-0.2.4/swagger_client/models/response_wrapper_map_string_string.py
+-rw-r--r--   0 cong       (501) staff       (20)     4858 2023-07-21 07:25:36.000000 goplus-0.2.4/swagger_client/models/response_wrapper_parse_abi_data_response.py
+-rw-r--r--   0 cong       (501) staff       (20)     4771 2024-03-06 09:44:32.000000 goplus-0.2.4/swagger_client/models/response_wrapper_phishing_site.py
+-rw-r--r--   0 cong       (501) staff       (20)     4957 2024-03-06 09:44:32.000000 goplus-0.2.4/swagger_client/models/response_wrapper_phishing_site_result.py
+-rw-r--r--   0 cong       (501) staff       (20)    13698 2024-03-06 09:44:32.000000 goplus-0.2.4/swagger_client/models/response_wrapper_phishing_site_result_nft_risk.py
+-rw-r--r--   0 cong       (501) staff       (20)     7173 2024-03-06 09:44:32.000000 goplus-0.2.4/swagger_client/models/response_wrapper_phishing_site_result_nft_risk_privileged_burn.py
+-rw-r--r--   0 cong       (501) staff       (20)     7221 2024-03-06 09:44:32.000000 goplus-0.2.4/swagger_client/models/response_wrapper_phishing_site_result_nft_risk_privileged_minting.py
+-rw-r--r--   0 cong       (501) staff       (20)     7141 2024-03-06 09:44:32.000000 goplus-0.2.4/swagger_client/models/response_wrapper_phishing_site_result_nft_risk_self_destruct.py
+-rw-r--r--   0 cong       (501) staff       (20)     7317 2024-03-06 09:44:32.000000 goplus-0.2.4/swagger_client/models/response_wrapper_phishing_site_result_nft_risk_transfer_without_approval.py
+-rw-r--r--   0 cong       (501) staff       (20)     9081 2024-03-06 09:44:32.000000 goplus-0.2.4/swagger_client/models/response_wrapper_phishing_site_result_website_contract_security.py
+-rw-r--r--   0 cong       (501) staff       (20)     4915 2023-07-21 07:25:36.000000 goplus-0.2.4/swagger_client/models/response_wrapper_ta_token_security_response.py
+-rw-r--r--   0 cong       (501) staff       (20)     4897 2023-07-21 07:25:36.000000 goplus-0.2.4/swagger_client/models/response_wrapper_token_security.py
+-rw-r--r--   0 cong       (501) staff       (20)     4905 2023-05-30 06:06:46.000000 goplus-0.2.4/swagger_client/models/response_wrapper_token_security_dex.py
+-rw-r--r--   0 cong       (501) staff       (20)     5264 2023-12-25 06:28:36.000000 goplus-0.2.4/swagger_client/models/response_wrapper_token_security_fake_token.py
+-rw-r--r--   0 cong       (501) staff       (20)    10002 2023-12-25 06:28:36.000000 goplus-0.2.4/swagger_client/models/response_wrapper_token_security_holders.py
+-rw-r--r--   0 cong       (501) staff       (20)     5269 2023-07-06 10:45:21.000000 goplus-0.2.4/swagger_client/models/response_wrapper_token_security_locked_detail.py
+-rw-r--r--   0 cong       (501) staff       (20)    11049 2023-12-25 06:28:36.000000 goplus-0.2.4/swagger_client/models/response_wrapper_token_security_lp_holders.py
+-rw-r--r--   0 cong       (501) staff       (20)     7453 2023-12-25 08:27:53.000000 goplus-0.2.4/swagger_client/models/response_wrapper_token_security_nft_list.py
+-rw-r--r--   0 cong       (501) staff       (20)    72566 2023-12-25 06:28:36.000000 goplus-0.2.4/swagger_client/models/response_wrapper_token_security_result.py
+-rw-r--r--   0 cong       (501) staff       (20)     4668 2023-07-21 07:25:36.000000 goplus-0.2.4/swagger_client/models/response_wrapperobject.py
+-rw-r--r--   0 cong       (501) staff       (20)     3194 2023-05-30 06:06:46.000000 goplus-0.2.4/swagger_client/models/ta_token_security_response.py
+-rw-r--r--   0 cong       (501) staff       (20)    13036 2023-05-30 06:06:46.000000 goplus-0.2.4/swagger_client/rest.py
```

### Comparing `goplus-0.2.3/LICENSE` & `goplus-0.2.4/LICENSE`

 * *Files identical despite different names*

### Comparing `goplus-0.2.3/PKG-INFO` & `goplus-0.2.4/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: goplus
-Version: 0.2.3
+Version: 0.2.4
 Summary: GoPlus SDK
 Home-page: https://github.com/GoPlusSecurity/goplus-sdk-python
 Author: GoPlus
 Author-email: service@gopluslabs.io
 License: Apache License 2.0
 Platform: UNKNOWN
 Classifier: Intended Audience :: Developers
```

### Comparing `goplus-0.2.3/goplus/__init__.py` & `goplus-0.2.4/goplus/__init__.py`

 * *Files identical despite different names*

### Comparing `goplus-0.2.3/goplus/__version__.py` & `goplus-0.2.4/goplus/__version__.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,10 +7,10 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
-VERSION = (0, 2, 3)
+VERSION = (0, 2, 4)
 
 __version__ = ".".join(map(str, VERSION))
```

### Comparing `goplus-0.2.3/goplus/address.py` & `goplus-0.2.4/goplus/address.py`

 * *Files identical despite different names*

### Comparing `goplus-0.2.3/goplus/approve.py` & `goplus-0.2.4/goplus/approve.py`

 * *Files identical despite different names*

### Comparing `goplus-0.2.3/goplus/auth.py` & `goplus-0.2.4/goplus/auth.py`

 * *Files identical despite different names*

### Comparing `goplus-0.2.3/goplus/base.py` & `goplus-0.2.4/goplus/base.py`

 * *Files identical despite different names*

### Comparing `goplus-0.2.3/goplus/chain.py` & `goplus-0.2.4/goplus/chain.py`

 * *Files identical despite different names*

### Comparing `goplus-0.2.3/goplus/dapp.py` & `goplus-0.2.4/goplus/dapp.py`

 * *Files identical despite different names*

### Comparing `goplus-0.2.3/goplus/decode.py` & `goplus-0.2.4/goplus/decode.py`

 * *Files identical despite different names*

### Comparing `goplus-0.2.3/goplus/errorcode.py` & `goplus-0.2.4/goplus/errorcode.py`

 * *Files identical despite different names*

### Comparing `goplus-0.2.3/goplus/nft.py` & `goplus-0.2.4/goplus/nft.py`

 * *Files identical despite different names*

### Comparing `goplus-0.2.3/goplus/phishing_site.py` & `goplus-0.2.4/goplus/phishing_site.py`

 * *Files identical despite different names*

### Comparing `goplus-0.2.3/goplus/rug_pull.py` & `goplus-0.2.4/goplus/rug_pull.py`

 * *Files identical despite different names*

### Comparing `goplus-0.2.3/goplus/token.py` & `goplus-0.2.4/goplus/token.py`

 * *Files identical despite different names*

### Comparing `goplus-0.2.3/goplus.egg-info/PKG-INFO` & `goplus-0.2.4/goplus.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: goplus
-Version: 0.2.3
+Version: 0.2.4
 Summary: GoPlus SDK
 Home-page: https://github.com/GoPlusSecurity/goplus-sdk-python
 Author: GoPlus
 Author-email: service@gopluslabs.io
 License: Apache License 2.0
 Platform: UNKNOWN
 Classifier: Intended Audience :: Developers
```

### Comparing `goplus-0.2.3/goplus.egg-info/SOURCES.txt` & `goplus-0.2.4/goplus.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `goplus-0.2.3/setup.py` & `goplus-0.2.4/setup.py`

 * *Files identical despite different names*

### Comparing `goplus-0.2.3/swagger_client/__init__.py` & `goplus-0.2.4/swagger_client/__init__.py`

 * *Files identical despite different names*

### Comparing `goplus-0.2.3/swagger_client/api/__init__.py` & `goplus-0.2.4/swagger_client/api/__init__.py`

 * *Files identical despite different names*

### Comparing `goplus-0.2.3/swagger_client/api/approve_controller_v_1_api.py` & `goplus-0.2.4/swagger_client/api/approve_controller_v_1_api.py`

 * *Files identical despite different names*

### Comparing `goplus-0.2.3/swagger_client/api/approve_controller_v_2_api.py` & `goplus-0.2.4/swagger_client/api/approve_controller_v_2_api.py`

 * *Files identical despite different names*

### Comparing `goplus-0.2.3/swagger_client/api/contract_abi_controller_api.py` & `goplus-0.2.4/swagger_client/api/contract_abi_controller_api.py`

 * *Files identical despite different names*

### Comparing `goplus-0.2.3/swagger_client/api/dapp_controller_api.py` & `goplus-0.2.4/swagger_client/api/dapp_controller_api.py`

 * *Files identical despite different names*

### Comparing `goplus-0.2.3/swagger_client/api/defi_controller_api.py` & `goplus-0.2.4/swagger_client/api/defi_controller_api.py`

 * *Files identical despite different names*

### Comparing `goplus-0.2.3/swagger_client/api/nft_controller_api.py` & `goplus-0.2.4/swagger_client/api/nft_controller_api.py`

 * *Files identical despite different names*

### Comparing `goplus-0.2.3/swagger_client/api/token_controller_api.py` & `goplus-0.2.4/swagger_client/api/token_controller_api.py`

 * *Files identical despite different names*

### Comparing `goplus-0.2.3/swagger_client/api/token_controller_v_1_api.py` & `goplus-0.2.4/swagger_client/api/token_controller_v_1_api.py`

 * *Files identical despite different names*

### Comparing `goplus-0.2.3/swagger_client/api/website_controller_api.py` & `goplus-0.2.4/swagger_client/api/website_controller_api.py`

 * *Files identical despite different names*

### Comparing `goplus-0.2.3/swagger_client/api_client.py` & `goplus-0.2.4/swagger_client/api_client.py`

 * *Files identical despite different names*

### Comparing `goplus-0.2.3/swagger_client/configuration.py` & `goplus-0.2.4/swagger_client/configuration.py`

 * *Files identical despite different names*

### Comparing `goplus-0.2.3/swagger_client/models/__init__.py` & `goplus-0.2.4/swagger_client/models/__init__.py`

 * *Files identical despite different names*

### Comparing `goplus-0.2.3/swagger_client/models/abi_address_info.py` & `goplus-0.2.4/swagger_client/models/abi_address_info.py`

 * *Files identical despite different names*

### Comparing `goplus-0.2.3/swagger_client/models/abi_param_info.py` & `goplus-0.2.4/swagger_client/models/abi_param_info.py`

 * *Files identical despite different names*

### Comparing `goplus-0.2.3/swagger_client/models/approve_address_info.py` & `goplus-0.2.4/swagger_client/models/approve_address_info.py`

 * *Files identical despite different names*

### Comparing `goplus-0.2.3/swagger_client/models/approve_erc1155_result.py` & `goplus-0.2.4/swagger_client/models/approve_erc1155_result.py`

 * *Files identical despite different names*

### Comparing `goplus-0.2.3/swagger_client/models/approve_nft1155_list_response.py` & `goplus-0.2.4/swagger_client/models/approve_nft1155_list_response.py`

 * *Files identical despite different names*

### Comparing `goplus-0.2.3/swagger_client/models/approve_nft_list_response.py` & `goplus-0.2.4/swagger_client/models/approve_nft_list_response.py`

 * *Files identical despite different names*

### Comparing `goplus-0.2.3/swagger_client/models/approve_result.py` & `goplus-0.2.4/swagger_client/models/approve_result.py`

 * *Files identical despite different names*

### Comparing `goplus-0.2.3/swagger_client/models/approve_token_out_list_response.py` & `goplus-0.2.4/swagger_client/models/approve_token_out_list_response.py`

 * *Files identical despite different names*

### Comparing `goplus-0.2.3/swagger_client/models/approve_token_result.py` & `goplus-0.2.4/swagger_client/models/approve_token_result.py`

 * *Files identical despite different names*

### Comparing `goplus-0.2.3/swagger_client/models/audit_info.py` & `goplus-0.2.4/swagger_client/models/audit_info.py`

 * *Files identical despite different names*

### Comparing `goplus-0.2.3/swagger_client/models/contract_approve_response.py` & `goplus-0.2.4/swagger_client/models/contract_approve_response.py`

 * *Files identical despite different names*

### Comparing `goplus-0.2.3/swagger_client/models/contracts.py` & `goplus-0.2.4/swagger_client/models/contracts.py`

 * *Files identical despite different names*

### Comparing `goplus-0.2.3/swagger_client/models/contracts_security.py` & `goplus-0.2.4/swagger_client/models/contracts_security.py`

 * *Files identical despite different names*

### Comparing `goplus-0.2.3/swagger_client/models/dapp_contract_security_response.py` & `goplus-0.2.4/swagger_client/models/dapp_contract_security_response.py`

 * *Files identical despite different names*

### Comparing `goplus-0.2.3/swagger_client/models/get_access_token_request.py` & `goplus-0.2.4/swagger_client/models/get_access_token_request.py`

 * *Files identical despite different names*

### Comparing `goplus-0.2.3/swagger_client/models/get_access_token_response.py` & `goplus-0.2.4/swagger_client/models/get_access_token_response.py`

 * *Files identical despite different names*

### Comparing `goplus-0.2.3/swagger_client/models/get_defi_info_response.py` & `goplus-0.2.4/swagger_client/models/get_defi_info_response.py`

 * *Files identical despite different names*

### Comparing `goplus-0.2.3/swagger_client/models/get_defi_info_response_result.py` & `goplus-0.2.4/swagger_client/models/get_defi_info_response_result.py`

 * *Files identical despite different names*

### Comparing `goplus-0.2.3/swagger_client/models/get_defi_info_response_result_owner.py` & `goplus-0.2.4/swagger_client/models/get_defi_info_response_result_owner.py`

 * *Files identical despite different names*

### Comparing `goplus-0.2.3/swagger_client/models/json_object.py` & `goplus-0.2.4/swagger_client/models/json_object.py`

 * *Files identical despite different names*

### Comparing `goplus-0.2.3/swagger_client/models/map_string_string.py` & `goplus-0.2.4/swagger_client/models/map_string_string.py`

 * *Files identical despite different names*

### Comparing `goplus-0.2.3/swagger_client/models/parse_abi_data_request.py` & `goplus-0.2.4/swagger_client/models/parse_abi_data_request.py`

 * *Files identical despite different names*

### Comparing `goplus-0.2.3/swagger_client/models/parse_abi_data_response.py` & `goplus-0.2.4/swagger_client/models/parse_abi_data_response.py`

 * *Files identical despite different names*

### Comparing `goplus-0.2.3/swagger_client/models/response_wrapper_address_contract.py` & `goplus-0.2.4/swagger_client/models/response_wrapper_address_contract.py`

 * *Files identical despite different names*

### Comparing `goplus-0.2.3/swagger_client/models/response_wrapper_address_contract_result.py` & `goplus-0.2.4/swagger_client/models/response_wrapper_address_contract_result.py`

 * *Files 11% similar despite different names*

```diff
@@ -27,97 +27,117 @@
       attribute_map (dict): The key is attribute name
                             and the value is json key in definition.
     """
     swagger_types = {
         'cybercrime': 'str',
         'money_laundering': 'str',
         'number_of_malicious_contracts_created': 'str',
+        'gas_abuse': 'str',
         'financial_crime': 'str',
         'darkweb_transactions': 'str',
+        'reinit': 'str',
         'phishing_activities': 'str',
         'contract_address': 'str',
         'fake_kyc': 'str',
         'blacklist_doubt': 'str',
         'data_source': 'str',
+        'fake_standard_interface': 'str',
         'stealing_attack': 'str',
         'blackmail_activities': 'str',
         'sanctioned': 'str',
         'malicious_mining_activities': 'str',
         'mixer': 'str',
+        'fake_token': 'str',
         'honeypot_related_address': 'str'
     }
 
     attribute_map = {
         'cybercrime': 'cybercrime',
         'money_laundering': 'money_laundering',
         'number_of_malicious_contracts_created': 'number_of_malicious_contracts_created',
+        'gas_abuse': 'gas_abuse',
         'financial_crime': 'financial_crime',
         'darkweb_transactions': 'darkweb_transactions',
+        'reinit': 'reinit',
         'phishing_activities': 'phishing_activities',
         'contract_address': 'contract_address',
         'fake_kyc': 'fake_kyc',
         'blacklist_doubt': 'blacklist_doubt',
         'data_source': 'data_source',
+        'fake_standard_interface': 'fake_standard_interface',
         'stealing_attack': 'stealing_attack',
         'blackmail_activities': 'blackmail_activities',
         'sanctioned': 'sanctioned',
         'malicious_mining_activities': 'malicious_mining_activities',
         'mixer': 'mixer',
+        'fake_token': 'fake_token',
         'honeypot_related_address': 'honeypot_related_address'
     }
 
-    def __init__(self, cybercrime=None, money_laundering=None, number_of_malicious_contracts_created=None, financial_crime=None, darkweb_transactions=None, phishing_activities=None, contract_address=None, fake_kyc=None, blacklist_doubt=None, data_source=None, stealing_attack=None, blackmail_activities=None, sanctioned=None, malicious_mining_activities=None, mixer=None, honeypot_related_address=None):  # noqa: E501
+    def __init__(self, cybercrime=None, money_laundering=None, number_of_malicious_contracts_created=None, gas_abuse=None, financial_crime=None, darkweb_transactions=None, reinit=None, phishing_activities=None, contract_address=None, fake_kyc=None, blacklist_doubt=None, data_source=None, fake_standard_interface=None, stealing_attack=None, blackmail_activities=None, sanctioned=None, malicious_mining_activities=None, mixer=None, fake_token=None, honeypot_related_address=None):  # noqa: E501
         """ResponseWrapperAddressContractResult - a model defined in Swagger"""  # noqa: E501
         self._cybercrime = None
         self._money_laundering = None
         self._number_of_malicious_contracts_created = None
+        self._gas_abuse = None
         self._financial_crime = None
         self._darkweb_transactions = None
+        self._reinit = None
         self._phishing_activities = None
         self._contract_address = None
         self._fake_kyc = None
         self._blacklist_doubt = None
         self._data_source = None
+        self._fake_standard_interface = None
         self._stealing_attack = None
         self._blackmail_activities = None
         self._sanctioned = None
         self._malicious_mining_activities = None
         self._mixer = None
+        self._fake_token = None
         self._honeypot_related_address = None
         self.discriminator = None
         if cybercrime is not None:
             self.cybercrime = cybercrime
         if money_laundering is not None:
             self.money_laundering = money_laundering
         if number_of_malicious_contracts_created is not None:
             self.number_of_malicious_contracts_created = number_of_malicious_contracts_created
+        if gas_abuse is not None:
+            self.gas_abuse = gas_abuse
         if financial_crime is not None:
             self.financial_crime = financial_crime
         if darkweb_transactions is not None:
             self.darkweb_transactions = darkweb_transactions
+        if reinit is not None:
+            self.reinit = reinit
         if phishing_activities is not None:
             self.phishing_activities = phishing_activities
         if contract_address is not None:
             self.contract_address = contract_address
         if fake_kyc is not None:
             self.fake_kyc = fake_kyc
         if blacklist_doubt is not None:
             self.blacklist_doubt = blacklist_doubt
         if data_source is not None:
             self.data_source = data_source
+        if fake_standard_interface is not None:
+            self.fake_standard_interface = fake_standard_interface
         if stealing_attack is not None:
             self.stealing_attack = stealing_attack
         if blackmail_activities is not None:
             self.blackmail_activities = blackmail_activities
         if sanctioned is not None:
             self.sanctioned = sanctioned
         if malicious_mining_activities is not None:
             self.malicious_mining_activities = malicious_mining_activities
         if mixer is not None:
             self.mixer = mixer
+        if fake_token is not None:
+            self.fake_token = fake_token
         if honeypot_related_address is not None:
             self.honeypot_related_address = honeypot_related_address
 
     @property
     def cybercrime(self):
         """Gets the cybercrime of this ResponseWrapperAddressContractResult.  # noqa: E501
 
@@ -183,14 +203,37 @@
         :param number_of_malicious_contracts_created: The number_of_malicious_contracts_created of this ResponseWrapperAddressContractResult.  # noqa: E501
         :type: str
         """
 
         self._number_of_malicious_contracts_created = number_of_malicious_contracts_created
 
     @property
+    def gas_abuse(self):
+        """Gets the gas_abuse of this ResponseWrapperAddressContractResult.  # noqa: E501
+
+        It describes whether this address is cheating other user's gas fee to mint other assets.(Notice:Any interaction with such addresses may result in loss of property.)  # noqa: E501
+
+        :return: The gas_abuse of this ResponseWrapperAddressContractResult.  # noqa: E501
+        :rtype: str
+        """
+        return self._gas_abuse
+
+    @gas_abuse.setter
+    def gas_abuse(self, gas_abuse):
+        """Sets the gas_abuse of this ResponseWrapperAddressContractResult.
+
+        It describes whether this address is cheating other user's gas fee to mint other assets.(Notice:Any interaction with such addresses may result in loss of property.)  # noqa: E501
+
+        :param gas_abuse: The gas_abuse of this ResponseWrapperAddressContractResult.  # noqa: E501
+        :type: str
+        """
+
+        self._gas_abuse = gas_abuse
+
+    @property
     def financial_crime(self):
         """Gets the financial_crime of this ResponseWrapperAddressContractResult.  # noqa: E501
 
         It describes whether this address is involved in financial crime. \"1\" means true; \"0\" means false.  # noqa: E501
 
         :return: The financial_crime of this ResponseWrapperAddressContractResult.  # noqa: E501
         :rtype: str
@@ -229,14 +272,37 @@
         :param darkweb_transactions: The darkweb_transactions of this ResponseWrapperAddressContractResult.  # noqa: E501
         :type: str
         """
 
         self._darkweb_transactions = darkweb_transactions
 
     @property
+    def reinit(self):
+        """Gets the reinit of this ResponseWrapperAddressContractResult.  # noqa: E501
+
+        It describes whether this address/contract has been deployed more than onces, and can be deployed again.(Notice:If a contract can be reinited, the developer can change the contract code whenever he wants.)  # noqa: E501
+
+        :return: The reinit of this ResponseWrapperAddressContractResult.  # noqa: E501
+        :rtype: str
+        """
+        return self._reinit
+
+    @reinit.setter
+    def reinit(self, reinit):
+        """Sets the reinit of this ResponseWrapperAddressContractResult.
+
+        It describes whether this address/contract has been deployed more than onces, and can be deployed again.(Notice:If a contract can be reinited, the developer can change the contract code whenever he wants.)  # noqa: E501
+
+        :param reinit: The reinit of this ResponseWrapperAddressContractResult.  # noqa: E501
+        :type: str
+        """
+
+        self._reinit = reinit
+
+    @property
     def phishing_activities(self):
         """Gets the phishing_activities of this ResponseWrapperAddressContractResult.  # noqa: E501
 
         It describes whether this address has implemented phishing activities. \"1\" means true; \"0\" means false.  # noqa: E501
 
         :return: The phishing_activities of this ResponseWrapperAddressContractResult.  # noqa: E501
         :rtype: str
@@ -344,14 +410,37 @@
         :param data_source: The data_source of this ResponseWrapperAddressContractResult.  # noqa: E501
         :type: str
         """
 
         self._data_source = data_source
 
     @property
+    def fake_standard_interface(self):
+        """Gets the fake_standard_interface of this ResponseWrapperAddressContractResult.  # noqa: E501
+
+        It describes whether this contract contains standard interfaces that do not conform the requirements of the standard protocol.(Notice:Fake Standard Interface is mostly seen in scam assets.)  # noqa: E501
+
+        :return: The fake_standard_interface of this ResponseWrapperAddressContractResult.  # noqa: E501
+        :rtype: str
+        """
+        return self._fake_standard_interface
+
+    @fake_standard_interface.setter
+    def fake_standard_interface(self, fake_standard_interface):
+        """Sets the fake_standard_interface of this ResponseWrapperAddressContractResult.
+
+        It describes whether this contract contains standard interfaces that do not conform the requirements of the standard protocol.(Notice:Fake Standard Interface is mostly seen in scam assets.)  # noqa: E501
+
+        :param fake_standard_interface: The fake_standard_interface of this ResponseWrapperAddressContractResult.  # noqa: E501
+        :type: str
+        """
+
+        self._fake_standard_interface = fake_standard_interface
+
+    @property
     def stealing_attack(self):
         """Gets the stealing_attack of this ResponseWrapperAddressContractResult.  # noqa: E501
 
         It describes whether this address has implemented stealing attacks. \"1\" means true; \"0\" means false.  # noqa: E501
 
         :return: The stealing_attack of this ResponseWrapperAddressContractResult.  # noqa: E501
         :rtype: str
@@ -459,14 +548,37 @@
         :param mixer: The mixer of this ResponseWrapperAddressContractResult.  # noqa: E501
         :type: str
         """
 
         self._mixer = mixer
 
     @property
+    def fake_token(self):
+        """Gets the fake_token of this ResponseWrapperAddressContractResult.  # noqa: E501
+
+        It indicates whether the token is a counterfeit of a mainstream asset.  # noqa: E501
+
+        :return: The fake_token of this ResponseWrapperAddressContractResult.  # noqa: E501
+        :rtype: str
+        """
+        return self._fake_token
+
+    @fake_token.setter
+    def fake_token(self, fake_token):
+        """Sets the fake_token of this ResponseWrapperAddressContractResult.
+
+        It indicates whether the token is a counterfeit of a mainstream asset.  # noqa: E501
+
+        :param fake_token: The fake_token of this ResponseWrapperAddressContractResult.  # noqa: E501
+        :type: str
+        """
+
+        self._fake_token = fake_token
+
+    @property
     def honeypot_related_address(self):
         """Gets the honeypot_related_address of this ResponseWrapperAddressContractResult.  # noqa: E501
 
         It describes whether this address is related to honeypot tokens or has created scam tokens. \"1\" means true; \"0\" means false.(Notice:Addresses related to honeypot mean the creators or owners of the honeypot tokens. This is a dangerous address if the address is ralated to honeypot tokens.)  # noqa: E501
 
         :return: The honeypot_related_address of this ResponseWrapperAddressContractResult.  # noqa: E501
         :rtype: str
```

### Comparing `goplus-0.2.3/swagger_client/models/response_wrapper_contract_approve_response.py` & `goplus-0.2.4/swagger_client/models/response_wrapper_contract_approve_response.py`

 * *Files identical despite different names*

### Comparing `goplus-0.2.3/swagger_client/models/response_wrapper_dapp_contract_security_response.py` & `goplus-0.2.4/swagger_client/models/response_wrapper_dapp_contract_security_response.py`

 * *Files identical despite different names*

### Comparing `goplus-0.2.3/swagger_client/models/response_wrapper_get_access_token_response.py` & `goplus-0.2.4/swagger_client/models/response_wrapper_get_access_token_response.py`

 * *Files identical despite different names*

### Comparing `goplus-0.2.3/swagger_client/models/response_wrapper_get_nft_info.py` & `goplus-0.2.4/swagger_client/models/response_wrapper_get_nft_info.py`

 * *Files identical despite different names*

### Comparing `goplus-0.2.3/swagger_client/models/response_wrapper_get_nft_info_result.py` & `goplus-0.2.4/swagger_client/models/response_wrapper_get_nft_info_result.py`

 * *Files identical despite different names*

### Comparing `goplus-0.2.3/swagger_client/models/response_wrapper_get_nft_info_result_privileged_burn.py` & `goplus-0.2.4/swagger_client/models/response_wrapper_get_nft_info_result_privileged_burn.py`

 * *Files identical despite different names*

### Comparing `goplus-0.2.3/swagger_client/models/response_wrapper_get_nft_info_result_privileged_minting.py` & `goplus-0.2.4/swagger_client/models/response_wrapper_get_nft_info_result_privileged_minting.py`

 * *Files identical despite different names*

### Comparing `goplus-0.2.3/swagger_client/models/response_wrapper_get_nft_info_result_same_nfts.py` & `goplus-0.2.4/swagger_client/models/response_wrapper_get_nft_info_result_same_nfts.py`

 * *Files identical despite different names*

### Comparing `goplus-0.2.3/swagger_client/models/response_wrapper_get_nft_info_result_self_destruct.py` & `goplus-0.2.4/swagger_client/models/response_wrapper_get_nft_info_result_self_destruct.py`

 * *Files identical despite different names*

### Comparing `goplus-0.2.3/swagger_client/models/response_wrapper_get_nft_info_result_transfer_without_approval.py` & `goplus-0.2.4/swagger_client/models/response_wrapper_get_nft_info_result_transfer_without_approval.py`

 * *Files identical despite different names*

### Comparing `goplus-0.2.3/swagger_client/models/response_wrapper_json_object.py` & `goplus-0.2.4/swagger_client/models/response_wrapper_json_object.py`

 * *Files identical despite different names*

### Comparing `goplus-0.2.3/swagger_client/models/response_wrapper_list_approve_nft1155_list_response.py` & `goplus-0.2.4/swagger_client/models/response_wrapper_list_approve_nft1155_list_response.py`

 * *Files identical despite different names*

### Comparing `goplus-0.2.3/swagger_client/models/response_wrapper_list_approve_nft_list_response.py` & `goplus-0.2.4/swagger_client/models/response_wrapper_list_approve_nft_list_response.py`

 * *Files identical despite different names*

### Comparing `goplus-0.2.3/swagger_client/models/response_wrapper_list_approve_token_out_list_response.py` & `goplus-0.2.4/swagger_client/models/response_wrapper_list_approve_token_out_list_response.py`

 * *Files identical despite different names*

### Comparing `goplus-0.2.3/swagger_client/models/response_wrapper_list_get_chains_list.py` & `goplus-0.2.4/swagger_client/models/response_wrapper_list_get_chains_list.py`

 * *Files identical despite different names*

### Comparing `goplus-0.2.3/swagger_client/models/response_wrapper_list_get_chains_list_result.py` & `goplus-0.2.4/swagger_client/models/response_wrapper_list_get_chains_list_result.py`

 * *Files identical despite different names*

### Comparing `goplus-0.2.3/swagger_client/models/response_wrapper_list_json_object.py` & `goplus-0.2.4/swagger_client/models/response_wrapper_list_json_object.py`

 * *Files identical despite different names*

### Comparing `goplus-0.2.3/swagger_client/models/response_wrapper_map_string_string.py` & `goplus-0.2.4/swagger_client/models/response_wrapper_map_string_string.py`

 * *Files identical despite different names*

### Comparing `goplus-0.2.3/swagger_client/models/response_wrapper_parse_abi_data_response.py` & `goplus-0.2.4/swagger_client/models/response_wrapper_parse_abi_data_response.py`

 * *Files identical despite different names*

### Comparing `goplus-0.2.3/swagger_client/models/response_wrapper_phishing_site.py` & `goplus-0.2.4/swagger_client/models/response_wrapper_phishing_site.py`

 * *Files identical despite different names*

### Comparing `goplus-0.2.3/swagger_client/models/response_wrapper_phishing_site_result.py` & `goplus-0.2.4/swagger_client/models/response_wrapper_phishing_site_result.py`

 * *Files identical despite different names*

### Comparing `goplus-0.2.3/swagger_client/models/response_wrapper_phishing_site_result_nft_risk.py` & `goplus-0.2.4/swagger_client/models/response_wrapper_phishing_site_result_nft_risk.py`

 * *Files identical despite different names*

### Comparing `goplus-0.2.3/swagger_client/models/response_wrapper_phishing_site_result_nft_risk_privileged_burn.py` & `goplus-0.2.4/swagger_client/models/response_wrapper_phishing_site_result_nft_risk_privileged_burn.py`

 * *Files identical despite different names*

### Comparing `goplus-0.2.3/swagger_client/models/response_wrapper_phishing_site_result_nft_risk_privileged_minting.py` & `goplus-0.2.4/swagger_client/models/response_wrapper_phishing_site_result_nft_risk_privileged_minting.py`

 * *Files identical despite different names*

### Comparing `goplus-0.2.3/swagger_client/models/response_wrapper_phishing_site_result_nft_risk_self_destruct.py` & `goplus-0.2.4/swagger_client/models/response_wrapper_phishing_site_result_nft_risk_self_destruct.py`

 * *Files identical despite different names*

### Comparing `goplus-0.2.3/swagger_client/models/response_wrapper_phishing_site_result_nft_risk_transfer_without_approval.py` & `goplus-0.2.4/swagger_client/models/response_wrapper_phishing_site_result_nft_risk_transfer_without_approval.py`

 * *Files identical despite different names*

### Comparing `goplus-0.2.3/swagger_client/models/response_wrapper_phishing_site_result_website_contract_security.py` & `goplus-0.2.4/swagger_client/models/response_wrapper_phishing_site_result_website_contract_security.py`

 * *Files identical despite different names*

### Comparing `goplus-0.2.3/swagger_client/models/response_wrapper_ta_token_security_response.py` & `goplus-0.2.4/swagger_client/models/response_wrapper_ta_token_security_response.py`

 * *Files identical despite different names*

### Comparing `goplus-0.2.3/swagger_client/models/response_wrapper_token_security.py` & `goplus-0.2.4/swagger_client/models/response_wrapper_token_security.py`

 * *Files identical despite different names*

### Comparing `goplus-0.2.3/swagger_client/models/response_wrapper_token_security_dex.py` & `goplus-0.2.4/swagger_client/models/response_wrapper_token_security_dex.py`

 * *Files identical despite different names*

### Comparing `goplus-0.2.3/swagger_client/models/response_wrapper_token_security_fake_token.py` & `goplus-0.2.4/swagger_client/models/response_wrapper_token_security_fake_token.py`

 * *Files identical despite different names*

### Comparing `goplus-0.2.3/swagger_client/models/response_wrapper_token_security_holders.py` & `goplus-0.2.4/swagger_client/models/response_wrapper_token_security_holders.py`

 * *Files identical despite different names*

### Comparing `goplus-0.2.3/swagger_client/models/response_wrapper_token_security_locked_detail.py` & `goplus-0.2.4/swagger_client/models/response_wrapper_token_security_locked_detail.py`

 * *Files identical despite different names*

### Comparing `goplus-0.2.3/swagger_client/models/response_wrapper_token_security_lp_holders.py` & `goplus-0.2.4/swagger_client/models/response_wrapper_token_security_lp_holders.py`

 * *Files identical despite different names*

### Comparing `goplus-0.2.3/swagger_client/models/response_wrapper_token_security_nft_list.py` & `goplus-0.2.4/swagger_client/models/response_wrapper_token_security_nft_list.py`

 * *Files identical despite different names*

### Comparing `goplus-0.2.3/swagger_client/models/response_wrapper_token_security_result.py` & `goplus-0.2.4/swagger_client/models/response_wrapper_token_security_result.py`

 * *Files identical despite different names*

### Comparing `goplus-0.2.3/swagger_client/models/response_wrapperobject.py` & `goplus-0.2.4/swagger_client/models/response_wrapperobject.py`

 * *Files identical despite different names*

### Comparing `goplus-0.2.3/swagger_client/models/ta_token_security_response.py` & `goplus-0.2.4/swagger_client/models/ta_token_security_response.py`

 * *Files identical despite different names*

### Comparing `goplus-0.2.3/swagger_client/rest.py` & `goplus-0.2.4/swagger_client/rest.py`

 * *Files identical despite different names*

