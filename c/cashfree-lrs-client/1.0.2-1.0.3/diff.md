# Comparing `tmp/cashfree_lrs_client-1.0.2.tar.gz` & `tmp/cashfree_lrs_client-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cashfree_lrs_client-1.0.2.tar", max compression
+gzip compressed data, was "cashfree_lrs_client-1.0.3.tar", max compression
```

## Comparing `cashfree_lrs_client-1.0.2.tar` & `cashfree_lrs_client-1.0.3.tar`

### file list

```diff
@@ -1,112 +1,112 @@
--rw-r--r--   0        0        0    12498 2023-05-01 07:34:04.939553 cashfree_lrs_client-1.0.2/README.md
--rw-r--r--   0        0        0      780 2023-05-01 07:34:04.959553 cashfree_lrs_client-1.0.2/cashfree_lrs_client/__init__.py
--rw-r--r--   0        0        0       99 2023-05-01 07:33:35.523573 cashfree_lrs_client-1.0.2/cashfree_lrs_client/api/__init__.py
--rw-r--r--   0        0        0    53538 2023-05-01 07:33:35.527573 cashfree_lrs_client-1.0.2/cashfree_lrs_client/api/default_api.py
--rw-r--r--   0        0        0    53218 2023-05-01 07:33:35.527573 cashfree_lrs_client-1.0.2/cashfree_lrs_client/api/lrs_api.py
--rw-r--r--   0        0        0    58509 2023-05-01 07:34:04.991553 cashfree_lrs_client-1.0.2/cashfree_lrs_client/api_client.py
--rw-r--r--   0        0        0      214 2023-05-01 07:34:05.015553 cashfree_lrs_client-1.0.2/cashfree_lrs_client/apis/__init__.py
--rw-r--r--   0        0        0     1655 2023-05-01 07:34:04.767553 cashfree_lrs_client-1.0.2/cashfree_lrs_client/apis/path_to_api.py
--rw-r--r--   0        0        0      246 2023-05-01 07:34:04.767553 cashfree_lrs_client-1.0.2/cashfree_lrs_client/apis/paths/__init__.py
--rw-r--r--   0        0        0      119 2023-05-01 07:34:04.783553 cashfree_lrs_client-1.0.2/cashfree_lrs_client/apis/paths/beneficiaries.py
--rw-r--r--   0        0        0      121 2023-05-01 07:34:04.771553 cashfree_lrs_client-1.0.2/cashfree_lrs_client/apis/paths/fx_rate_details.py
--rw-r--r--   0        0        0      105 2023-05-01 07:34:04.779553 cashfree_lrs_client-1.0.2/cashfree_lrs_client/apis/paths/orders.py
--rw-r--r--   0        0        0      137 2023-05-01 07:34:04.775553 cashfree_lrs_client-1.0.2/cashfree_lrs_client/apis/paths/orders_documents_upload.py
--rw-r--r--   0        0        0      153 2023-05-01 07:34:04.783553 cashfree_lrs_client-1.0.2/cashfree_lrs_client/apis/paths/orders_order_id_documents_upload.py
--rw-r--r--   0        0        0      136 2023-05-01 07:34:04.771553 cashfree_lrs_client-1.0.2/cashfree_lrs_client/apis/paths/orders_order_id_process.py
--rw-r--r--   0        0        0      111 2023-05-01 07:34:04.779553 cashfree_lrs_client-1.0.2/cashfree_lrs_client/apis/paths/remitters.py
--rw-r--r--   0        0        0      109 2023-05-01 07:34:04.775553 cashfree_lrs_client-1.0.2/cashfree_lrs_client/apis/paths/webhooks.py
--rw-r--r--   0        0        0      306 2023-05-01 07:34:04.763553 cashfree_lrs_client-1.0.2/cashfree_lrs_client/apis/tag_to_api.py
--rw-r--r--   0        0        0      308 2023-05-01 07:34:04.767553 cashfree_lrs_client-1.0.2/cashfree_lrs_client/apis/tags/__init__.py
--rw-r--r--   0        0        0     1162 2023-05-01 07:34:04.823553 cashfree_lrs_client-1.0.2/cashfree_lrs_client/apis/tags/lrs_api.py
--rw-r--r--   0        0        0    17326 2023-05-01 07:34:04.959553 cashfree_lrs_client-1.0.2/cashfree_lrs_client/configuration.py
--rw-r--r--   0        0        0     2815 2023-05-01 07:33:35.527573 cashfree_lrs_client-1.0.2/cashfree_lrs_client/docs/CreateBeneficiaryRequest.md
--rw-r--r--   0        0        0     2331 2023-05-01 07:33:35.527573 cashfree_lrs_client-1.0.2/cashfree_lrs_client/docs/CreateOrderRequest.md
--rw-r--r--   0        0        0     1337 2023-05-01 07:33:35.527573 cashfree_lrs_client-1.0.2/cashfree_lrs_client/docs/CreateOrderResponse.md
--rw-r--r--   0        0        0     2583 2023-05-01 07:33:35.527573 cashfree_lrs_client-1.0.2/cashfree_lrs_client/docs/CreateRemitterRequest.md
--rw-r--r--   0        0        0      389 2023-05-01 07:33:35.527573 cashfree_lrs_client-1.0.2/cashfree_lrs_client/docs/Currency.md
--rw-r--r--   0        0        0      859 2023-05-01 07:33:35.527573 cashfree_lrs_client-1.0.2/cashfree_lrs_client/docs/Error.md
--rw-r--r--   0        0        0     1656 2023-05-01 07:33:35.527573 cashfree_lrs_client-1.0.2/cashfree_lrs_client/docs/FetchForexRateRequest.md
--rw-r--r--   0        0        0    59748 2023-05-01 07:33:35.527573 cashfree_lrs_client-1.0.2/cashfree_lrs_client/docs/LrsApi.md
--rw-r--r--   0        0        0      343 2023-05-01 07:33:35.527573 cashfree_lrs_client-1.0.2/cashfree_lrs_client/docs/Purpose.md
--rw-r--r--   0        0        0     1239 2023-05-01 07:33:35.527573 cashfree_lrs_client-1.0.2/cashfree_lrs_client/docs/SetupWebhooksRequest.md
--rw-r--r--   0        0        0      896 2023-05-01 07:33:35.527573 cashfree_lrs_client-1.0.2/cashfree_lrs_client/docs/SuccessMessage.md
--rw-r--r--   0        0        0     4503 2023-05-01 07:34:04.963553 cashfree_lrs_client-1.0.2/cashfree_lrs_client/exceptions.py
--rw-r--r--   0        0        0      353 2023-05-01 07:34:05.011553 cashfree_lrs_client-1.0.2/cashfree_lrs_client/model/__init__.py
--rw-r--r--   0        0        0      884 2023-05-01 07:33:59.051553 cashfree_lrs_client-1.0.2/cashfree_lrs_client/model/amount.py
--rw-r--r--   0        0        0      815 2023-05-01 07:33:59.131553 cashfree_lrs_client-1.0.2/cashfree_lrs_client/model/amount.pyi
--rw-r--r--   0        0        0    14903 2023-05-01 07:33:59.987553 cashfree_lrs_client-1.0.2/cashfree_lrs_client/model/create_beneficiary_request.py
--rw-r--r--   0        0        0    13066 2023-05-01 07:34:00.551553 cashfree_lrs_client-1.0.2/cashfree_lrs_client/model/create_beneficiary_request.pyi
--rw-r--r--   0        0        0    11475 2023-05-01 07:34:01.079553 cashfree_lrs_client-1.0.2/cashfree_lrs_client/model/create_order_request.py
--rw-r--r--   0        0        0    10572 2023-05-01 07:34:01.295553 cashfree_lrs_client-1.0.2/cashfree_lrs_client/model/create_order_request.pyi
--rw-r--r--   0        0        0     8398 2023-05-01 07:34:01.567553 cashfree_lrs_client-1.0.2/cashfree_lrs_client/model/create_order_response.py
--rw-r--r--   0        0        0     8166 2023-05-01 07:34:01.707553 cashfree_lrs_client-1.0.2/cashfree_lrs_client/model/create_order_response.pyi
--rw-r--r--   0        0        0    12349 2023-05-01 07:34:02.151553 cashfree_lrs_client-1.0.2/cashfree_lrs_client/model/create_remitter_request.py
--rw-r--r--   0        0        0    10785 2023-05-01 07:34:02.407553 cashfree_lrs_client-1.0.2/cashfree_lrs_client/model/create_remitter_request.pyi
--rw-r--r--   0        0        0     1192 2023-05-01 07:34:02.507553 cashfree_lrs_client-1.0.2/cashfree_lrs_client/model/currency.py
--rw-r--r--   0        0        0     1031 2023-05-01 07:34:02.519553 cashfree_lrs_client-1.0.2/cashfree_lrs_client/model/currency.pyi
--rw-r--r--   0        0        0     3384 2023-05-01 07:34:02.567553 cashfree_lrs_client-1.0.2/cashfree_lrs_client/model/error.py
--rw-r--r--   0        0        0     3384 2023-05-01 07:34:02.603553 cashfree_lrs_client-1.0.2/cashfree_lrs_client/model/error.pyi
--rw-r--r--   0        0        0     5805 2023-05-01 07:34:02.667553 cashfree_lrs_client-1.0.2/cashfree_lrs_client/model/fetch_forex_rate_request.py
--rw-r--r--   0        0        0     5697 2023-05-01 07:34:02.715553 cashfree_lrs_client-1.0.2/cashfree_lrs_client/model/fetch_forex_rate_request.pyi
--rw-r--r--   0        0        0     1368 2023-05-01 07:34:02.759553 cashfree_lrs_client-1.0.2/cashfree_lrs_client/model/purpose.py
--rw-r--r--   0        0        0     1169 2023-05-01 07:34:02.767553 cashfree_lrs_client-1.0.2/cashfree_lrs_client/model/purpose.pyi
--rw-r--r--   0        0        0     3663 2023-05-01 07:34:02.815553 cashfree_lrs_client-1.0.2/cashfree_lrs_client/model/setup_webhooks_request.py
--rw-r--r--   0        0        0     3663 2023-05-01 07:34:02.851553 cashfree_lrs_client-1.0.2/cashfree_lrs_client/model/setup_webhooks_request.pyi
--rw-r--r--   0        0        0     2477 2023-05-01 07:34:02.899553 cashfree_lrs_client-1.0.2/cashfree_lrs_client/model/success_message.py
--rw-r--r--   0        0        0     2477 2023-05-01 07:34:02.915553 cashfree_lrs_client-1.0.2/cashfree_lrs_client/model/success_message.pyi
--rw-r--r--   0        0        0     1173 2023-05-01 07:34:05.011553 cashfree_lrs_client-1.0.2/cashfree_lrs_client/models/__init__.py
--rw-r--r--   0        0        0     1975 2023-05-01 07:33:35.527573 cashfree_lrs_client-1.0.2/cashfree_lrs_client/models/create_beneficiary200_response.py
--rw-r--r--   0        0        0     5826 2023-05-01 07:33:35.527573 cashfree_lrs_client-1.0.2/cashfree_lrs_client/models/create_beneficiary_request.py
--rw-r--r--   0        0        0     4904 2023-05-01 07:33:35.527573 cashfree_lrs_client-1.0.2/cashfree_lrs_client/models/create_order_request.py
--rw-r--r--   0        0        0     2951 2023-05-01 07:33:35.527573 cashfree_lrs_client-1.0.2/cashfree_lrs_client/models/create_order_response.py
--rw-r--r--   0        0        0     1951 2023-05-01 07:33:35.527573 cashfree_lrs_client-1.0.2/cashfree_lrs_client/models/create_remitter200_response.py
--rw-r--r--   0        0        0     5289 2023-05-01 07:33:35.527573 cashfree_lrs_client-1.0.2/cashfree_lrs_client/models/create_remitter_request.py
--rw-r--r--   0        0        0      608 2023-05-01 07:33:35.527573 cashfree_lrs_client-1.0.2/cashfree_lrs_client/models/currency.py
--rw-r--r--   0        0        0     1964 2023-05-01 07:33:35.527573 cashfree_lrs_client-1.0.2/cashfree_lrs_client/models/error.py
--rw-r--r--   0        0        0     3205 2023-05-01 07:33:35.527573 cashfree_lrs_client-1.0.2/cashfree_lrs_client/models/fetch_forex_rate_request.py
--rw-r--r--   0        0        0     2903 2023-05-01 07:33:35.527573 cashfree_lrs_client-1.0.2/cashfree_lrs_client/models/order_response.py
--rw-r--r--   0        0        0      626 2023-05-01 07:33:35.527573 cashfree_lrs_client-1.0.2/cashfree_lrs_client/models/purpose.py
--rw-r--r--   0        0        0     1943 2023-05-01 07:33:35.527573 cashfree_lrs_client-1.0.2/cashfree_lrs_client/models/setup_webhooks200_response.py
--rw-r--r--   0        0        0     2355 2023-05-01 07:33:35.527573 cashfree_lrs_client-1.0.2/cashfree_lrs_client/models/setup_webhooks_request.py
--rw-r--r--   0        0        0     1863 2023-05-01 07:33:35.527573 cashfree_lrs_client-1.0.2/cashfree_lrs_client/models/success_message.py
--rw-r--r--   0        0        0      644 2023-05-01 07:34:04.759553 cashfree_lrs_client-1.0.2/cashfree_lrs_client/paths/__init__.py
--rw-r--r--   0        0        0      323 2023-05-01 07:34:04.763553 cashfree_lrs_client-1.0.2/cashfree_lrs_client/paths/beneficiaries/__init__.py
--rw-r--r--   0        0        0    12582 2023-05-01 07:34:03.351553 cashfree_lrs_client-1.0.2/cashfree_lrs_client/paths/beneficiaries/post.py
--rw-r--r--   0        0        0    12396 2023-05-01 07:34:03.463553 cashfree_lrs_client-1.0.2/cashfree_lrs_client/paths/beneficiaries/post.pyi
--rw-r--r--   0        0        0      326 2023-05-01 07:34:04.759553 cashfree_lrs_client-1.0.2/cashfree_lrs_client/paths/fx_rate_details/__init__.py
--rw-r--r--   0        0        0    11760 2023-05-01 07:34:04.035553 cashfree_lrs_client-1.0.2/cashfree_lrs_client/paths/fx_rate_details/post.py
--rw-r--r--   0        0        0    11604 2023-05-01 07:34:04.139553 cashfree_lrs_client-1.0.2/cashfree_lrs_client/paths/fx_rate_details/post.pyi
--rw-r--r--   0        0        0      309 2023-05-01 07:34:04.759553 cashfree_lrs_client-1.0.2/cashfree_lrs_client/paths/orders/__init__.py
--rw-r--r--   0        0        0    13005 2023-05-01 07:34:03.591553 cashfree_lrs_client-1.0.2/cashfree_lrs_client/paths/orders/post.py
--rw-r--r--   0        0        0    12789 2023-05-01 07:34:03.707553 cashfree_lrs_client-1.0.2/cashfree_lrs_client/paths/orders/post.pyi
--rw-r--r--   0        0        0      343 2023-05-01 07:34:04.759553 cashfree_lrs_client-1.0.2/cashfree_lrs_client/paths/orders_documents_upload/__init__.py
--rw-r--r--   0        0        0    12334 2023-05-01 07:34:03.123553 cashfree_lrs_client-1.0.2/cashfree_lrs_client/paths/orders_documents_upload/post.py
--rw-r--r--   0        0        0    12148 2023-05-01 07:34:03.235553 cashfree_lrs_client-1.0.2/cashfree_lrs_client/paths/orders_documents_upload/post.pyi
--rw-r--r--   0        0        0      361 2023-05-01 07:34:04.763553 cashfree_lrs_client-1.0.2/cashfree_lrs_client/paths/orders_order_id_documents_upload/__init__.py
--rw-r--r--   0        0        0    15715 2023-05-01 07:34:04.631553 cashfree_lrs_client-1.0.2/cashfree_lrs_client/paths/orders_order_id_documents_upload/post.py
--rw-r--r--   0        0        0    15469 2023-05-01 07:34:04.755553 cashfree_lrs_client-1.0.2/cashfree_lrs_client/paths/orders_order_id_documents_upload/post.pyi
--rw-r--r--   0        0        0      343 2023-05-01 07:34:04.759553 cashfree_lrs_client-1.0.2/cashfree_lrs_client/paths/orders_order_id_process/__init__.py
--rw-r--r--   0        0        0     8093 2023-05-01 07:34:04.215553 cashfree_lrs_client-1.0.2/cashfree_lrs_client/paths/orders_order_id_process/post.py
--rw-r--r--   0        0        0     7937 2023-05-01 07:34:04.291553 cashfree_lrs_client-1.0.2/cashfree_lrs_client/paths/orders_order_id_process/post.pyi
--rw-r--r--   0        0        0      315 2023-05-01 07:34:04.763553 cashfree_lrs_client-1.0.2/cashfree_lrs_client/paths/remitters/__init__.py
--rw-r--r--   0        0        0    12525 2023-05-01 07:34:03.819553 cashfree_lrs_client-1.0.2/cashfree_lrs_client/paths/remitters/post.py
--rw-r--r--   0        0        0    12339 2023-05-01 07:34:03.931553 cashfree_lrs_client-1.0.2/cashfree_lrs_client/paths/remitters/post.pyi
--rw-r--r--   0        0        0      313 2023-05-01 07:34:04.759553 cashfree_lrs_client-1.0.2/cashfree_lrs_client/paths/webhooks/__init__.py
--rw-r--r--   0        0        0    11939 2023-05-01 07:34:04.399553 cashfree_lrs_client-1.0.2/cashfree_lrs_client/paths/webhooks/post.py
--rw-r--r--   0        0        0    11783 2023-05-01 07:34:04.503553 cashfree_lrs_client-1.0.2/cashfree_lrs_client/paths/webhooks/post.pyi
--rw-r--r--   0        0        0    10536 2023-05-01 07:34:04.995553 cashfree_lrs_client-1.0.2/cashfree_lrs_client/rest.py
--rw-r--r--   0        0        0    97649 2023-05-01 07:34:05.011553 cashfree_lrs_client-1.0.2/cashfree_lrs_client/schemas.py
--rw-r--r--   0        0        0        0 2023-05-01 07:33:35.531573 cashfree_lrs_client-1.0.2/cashfree_lrs_client/test/__init__.py
--rw-r--r--   0        0        0     2694 2023-05-01 07:33:35.531573 cashfree_lrs_client-1.0.2/cashfree_lrs_client/test/test_create_beneficiary_request.py
--rw-r--r--   0        0        0     2292 2023-05-01 07:33:35.531573 cashfree_lrs_client-1.0.2/cashfree_lrs_client/test/test_create_order_request.py
--rw-r--r--   0        0        0     1952 2023-05-01 07:33:35.531573 cashfree_lrs_client-1.0.2/cashfree_lrs_client/test/test_create_order_response.py
--rw-r--r--   0        0        0     2486 2023-05-01 07:33:35.531573 cashfree_lrs_client-1.0.2/cashfree_lrs_client/test/test_create_remitter_request.py
--rw-r--r--   0        0        0      738 2023-05-01 07:33:35.531573 cashfree_lrs_client-1.0.2/cashfree_lrs_client/test/test_currency.py
--rw-r--r--   0        0        0     1439 2023-05-01 07:33:35.531573 cashfree_lrs_client-1.0.2/cashfree_lrs_client/test/test_error.py
--rw-r--r--   0        0        0     1860 2023-05-01 07:33:35.531573 cashfree_lrs_client-1.0.2/cashfree_lrs_client/test/test_fetch_forex_rate_request.py
--rw-r--r--   0        0        0     1845 2023-05-01 07:33:35.531573 cashfree_lrs_client-1.0.2/cashfree_lrs_client/test/test_lrs_api.py
--rw-r--r--   0        0        0      731 2023-05-01 07:33:35.531573 cashfree_lrs_client-1.0.2/cashfree_lrs_client/test/test_purpose.py
--rw-r--r--   0        0        0     1737 2023-05-01 07:33:35.531573 cashfree_lrs_client-1.0.2/cashfree_lrs_client/test/test_setup_webhooks_request.py
--rw-r--r--   0        0        0     1493 2023-05-01 07:33:35.531573 cashfree_lrs_client-1.0.2/cashfree_lrs_client/test/test_success_message.py
--rw-r--r--   0        0        0      698 2023-05-01 07:33:49.363558 cashfree_lrs_client-1.0.2/pyproject.toml
--rw-r--r--   0        0        0    13295 1970-01-01 00:00:00.000000 cashfree_lrs_client-1.0.2/PKG-INFO
+-rw-r--r--   0        0        0     5213 2023-05-01 08:09:00.676026 cashfree_lrs_client-1.0.3/README.md
+-rw-r--r--   0        0        0     1647 2023-05-01 08:09:00.712026 cashfree_lrs_client-1.0.3/cashfree_lrs_client/__init__.py
+-rw-r--r--   0        0        0       99 2023-05-01 08:09:00.716026 cashfree_lrs_client-1.0.3/cashfree_lrs_client/api/__init__.py
+-rw-r--r--   0        0        0    53538 2023-05-01 08:08:38.267853 cashfree_lrs_client-1.0.3/cashfree_lrs_client/api/default_api.py
+-rw-r--r--   0        0        0    53367 2023-05-01 08:09:00.664026 cashfree_lrs_client-1.0.3/cashfree_lrs_client/api/lrs_api.py
+-rw-r--r--   0        0        0    29632 2023-05-01 08:09:00.724026 cashfree_lrs_client-1.0.3/cashfree_lrs_client/api_client.py
+-rw-r--r--   0        0        0      214 2023-05-01 08:08:38.267853 cashfree_lrs_client-1.0.3/cashfree_lrs_client/apis/__init__.py
+-rw-r--r--   0        0        0     1655 2023-05-01 08:08:38.267853 cashfree_lrs_client-1.0.3/cashfree_lrs_client/apis/path_to_api.py
+-rw-r--r--   0        0        0      246 2023-05-01 08:08:38.267853 cashfree_lrs_client-1.0.3/cashfree_lrs_client/apis/paths/__init__.py
+-rw-r--r--   0        0        0      119 2023-05-01 08:08:38.267853 cashfree_lrs_client-1.0.3/cashfree_lrs_client/apis/paths/beneficiaries.py
+-rw-r--r--   0        0        0      121 2023-05-01 08:08:38.267853 cashfree_lrs_client-1.0.3/cashfree_lrs_client/apis/paths/fx_rate_details.py
+-rw-r--r--   0        0        0      105 2023-05-01 08:08:38.267853 cashfree_lrs_client-1.0.3/cashfree_lrs_client/apis/paths/orders.py
+-rw-r--r--   0        0        0      137 2023-05-01 08:08:38.267853 cashfree_lrs_client-1.0.3/cashfree_lrs_client/apis/paths/orders_documents_upload.py
+-rw-r--r--   0        0        0      153 2023-05-01 08:08:38.267853 cashfree_lrs_client-1.0.3/cashfree_lrs_client/apis/paths/orders_order_id_documents_upload.py
+-rw-r--r--   0        0        0      136 2023-05-01 08:08:38.267853 cashfree_lrs_client-1.0.3/cashfree_lrs_client/apis/paths/orders_order_id_process.py
+-rw-r--r--   0        0        0      111 2023-05-01 08:08:38.267853 cashfree_lrs_client-1.0.3/cashfree_lrs_client/apis/paths/remitters.py
+-rw-r--r--   0        0        0      109 2023-05-01 08:08:38.267853 cashfree_lrs_client-1.0.3/cashfree_lrs_client/apis/paths/webhooks.py
+-rw-r--r--   0        0        0      306 2023-05-01 08:08:38.267853 cashfree_lrs_client-1.0.3/cashfree_lrs_client/apis/tag_to_api.py
+-rw-r--r--   0        0        0      308 2023-05-01 08:08:38.267853 cashfree_lrs_client-1.0.3/cashfree_lrs_client/apis/tags/__init__.py
+-rw-r--r--   0        0        0     1162 2023-05-01 08:08:38.267853 cashfree_lrs_client-1.0.3/cashfree_lrs_client/apis/tags/lrs_api.py
+-rw-r--r--   0        0        0    15922 2023-05-01 08:09:00.708026 cashfree_lrs_client-1.0.3/cashfree_lrs_client/configuration.py
+-rw-r--r--   0        0        0     2815 2023-05-01 08:08:38.267853 cashfree_lrs_client-1.0.3/cashfree_lrs_client/docs/CreateBeneficiaryRequest.md
+-rw-r--r--   0        0        0     2331 2023-05-01 08:08:38.267853 cashfree_lrs_client-1.0.3/cashfree_lrs_client/docs/CreateOrderRequest.md
+-rw-r--r--   0        0        0     1337 2023-05-01 08:08:38.267853 cashfree_lrs_client-1.0.3/cashfree_lrs_client/docs/CreateOrderResponse.md
+-rw-r--r--   0        0        0     2583 2023-05-01 08:08:38.267853 cashfree_lrs_client-1.0.3/cashfree_lrs_client/docs/CreateRemitterRequest.md
+-rw-r--r--   0        0        0      389 2023-05-01 08:08:38.267853 cashfree_lrs_client-1.0.3/cashfree_lrs_client/docs/Currency.md
+-rw-r--r--   0        0        0      859 2023-05-01 08:08:38.267853 cashfree_lrs_client-1.0.3/cashfree_lrs_client/docs/Error.md
+-rw-r--r--   0        0        0     1656 2023-05-01 08:08:38.267853 cashfree_lrs_client-1.0.3/cashfree_lrs_client/docs/FetchForexRateRequest.md
+-rw-r--r--   0        0        0    59748 2023-05-01 08:08:38.267853 cashfree_lrs_client-1.0.3/cashfree_lrs_client/docs/LrsApi.md
+-rw-r--r--   0        0        0      343 2023-05-01 08:08:38.271853 cashfree_lrs_client-1.0.3/cashfree_lrs_client/docs/Purpose.md
+-rw-r--r--   0        0        0     1239 2023-05-01 08:08:38.271853 cashfree_lrs_client-1.0.3/cashfree_lrs_client/docs/SetupWebhooksRequest.md
+-rw-r--r--   0        0        0      896 2023-05-01 08:08:38.271853 cashfree_lrs_client-1.0.3/cashfree_lrs_client/docs/SuccessMessage.md
+-rw-r--r--   0        0        0     5118 2023-05-01 08:09:00.720026 cashfree_lrs_client-1.0.3/cashfree_lrs_client/exceptions.py
+-rw-r--r--   0        0        0      353 2023-05-01 08:08:38.271853 cashfree_lrs_client-1.0.3/cashfree_lrs_client/model/__init__.py
+-rw-r--r--   0        0        0      884 2023-05-01 08:08:38.271853 cashfree_lrs_client-1.0.3/cashfree_lrs_client/model/amount.py
+-rw-r--r--   0        0        0      815 2023-05-01 08:08:38.271853 cashfree_lrs_client-1.0.3/cashfree_lrs_client/model/amount.pyi
+-rw-r--r--   0        0        0    14903 2023-05-01 08:08:38.271853 cashfree_lrs_client-1.0.3/cashfree_lrs_client/model/create_beneficiary_request.py
+-rw-r--r--   0        0        0    13066 2023-05-01 08:08:38.271853 cashfree_lrs_client-1.0.3/cashfree_lrs_client/model/create_beneficiary_request.pyi
+-rw-r--r--   0        0        0    11475 2023-05-01 08:08:38.271853 cashfree_lrs_client-1.0.3/cashfree_lrs_client/model/create_order_request.py
+-rw-r--r--   0        0        0    10572 2023-05-01 08:08:38.271853 cashfree_lrs_client-1.0.3/cashfree_lrs_client/model/create_order_request.pyi
+-rw-r--r--   0        0        0     8398 2023-05-01 08:08:38.271853 cashfree_lrs_client-1.0.3/cashfree_lrs_client/model/create_order_response.py
+-rw-r--r--   0        0        0     8166 2023-05-01 08:08:38.271853 cashfree_lrs_client-1.0.3/cashfree_lrs_client/model/create_order_response.pyi
+-rw-r--r--   0        0        0    12349 2023-05-01 08:08:38.271853 cashfree_lrs_client-1.0.3/cashfree_lrs_client/model/create_remitter_request.py
+-rw-r--r--   0        0        0    10785 2023-05-01 08:08:38.271853 cashfree_lrs_client-1.0.3/cashfree_lrs_client/model/create_remitter_request.pyi
+-rw-r--r--   0        0        0     1192 2023-05-01 08:08:38.271853 cashfree_lrs_client-1.0.3/cashfree_lrs_client/model/currency.py
+-rw-r--r--   0        0        0     1031 2023-05-01 08:08:38.271853 cashfree_lrs_client-1.0.3/cashfree_lrs_client/model/currency.pyi
+-rw-r--r--   0        0        0     3384 2023-05-01 08:08:38.271853 cashfree_lrs_client-1.0.3/cashfree_lrs_client/model/error.py
+-rw-r--r--   0        0        0     3384 2023-05-01 08:08:38.271853 cashfree_lrs_client-1.0.3/cashfree_lrs_client/model/error.pyi
+-rw-r--r--   0        0        0     5805 2023-05-01 08:08:38.271853 cashfree_lrs_client-1.0.3/cashfree_lrs_client/model/fetch_forex_rate_request.py
+-rw-r--r--   0        0        0     5697 2023-05-01 08:08:38.271853 cashfree_lrs_client-1.0.3/cashfree_lrs_client/model/fetch_forex_rate_request.pyi
+-rw-r--r--   0        0        0     1368 2023-05-01 08:08:38.271853 cashfree_lrs_client-1.0.3/cashfree_lrs_client/model/purpose.py
+-rw-r--r--   0        0        0     1169 2023-05-01 08:08:38.271853 cashfree_lrs_client-1.0.3/cashfree_lrs_client/model/purpose.pyi
+-rw-r--r--   0        0        0     3663 2023-05-01 08:08:38.271853 cashfree_lrs_client-1.0.3/cashfree_lrs_client/model/setup_webhooks_request.py
+-rw-r--r--   0        0        0     3663 2023-05-01 08:08:38.271853 cashfree_lrs_client-1.0.3/cashfree_lrs_client/model/setup_webhooks_request.pyi
+-rw-r--r--   0        0        0     2477 2023-05-01 08:08:38.271853 cashfree_lrs_client-1.0.3/cashfree_lrs_client/model/success_message.py
+-rw-r--r--   0        0        0     2477 2023-05-01 08:08:38.271853 cashfree_lrs_client-1.0.3/cashfree_lrs_client/model/success_message.pyi
+-rw-r--r--   0        0        0     1064 2023-05-01 08:09:00.712026 cashfree_lrs_client-1.0.3/cashfree_lrs_client/models/__init__.py
+-rw-r--r--   0        0        0     1975 2023-05-01 08:08:38.271853 cashfree_lrs_client-1.0.3/cashfree_lrs_client/models/create_beneficiary200_response.py
+-rw-r--r--   0        0        0     5832 2023-05-01 08:09:00.492024 cashfree_lrs_client-1.0.3/cashfree_lrs_client/models/create_beneficiary_request.py
+-rw-r--r--   0        0        0     5041 2023-05-01 08:09:00.504024 cashfree_lrs_client-1.0.3/cashfree_lrs_client/models/create_order_request.py
+-rw-r--r--   0        0        0     3426 2023-05-01 08:09:00.516024 cashfree_lrs_client-1.0.3/cashfree_lrs_client/models/create_order_response.py
+-rw-r--r--   0        0        0     1951 2023-05-01 08:08:38.271853 cashfree_lrs_client-1.0.3/cashfree_lrs_client/models/create_remitter200_response.py
+-rw-r--r--   0        0        0     5347 2023-05-01 08:09:00.528025 cashfree_lrs_client-1.0.3/cashfree_lrs_client/models/create_remitter_request.py
+-rw-r--r--   0        0        0      765 2023-05-01 08:09:00.532024 cashfree_lrs_client-1.0.3/cashfree_lrs_client/models/currency.py
+-rw-r--r--   0        0        0     2088 2023-05-01 08:09:00.544025 cashfree_lrs_client-1.0.3/cashfree_lrs_client/models/error.py
+-rw-r--r--   0        0        0     3279 2023-05-01 08:09:00.552025 cashfree_lrs_client-1.0.3/cashfree_lrs_client/models/fetch_forex_rate_request.py
+-rw-r--r--   0        0        0     2903 2023-05-01 08:08:38.271853 cashfree_lrs_client-1.0.3/cashfree_lrs_client/models/order_response.py
+-rw-r--r--   0        0        0      780 2023-05-01 08:09:00.556025 cashfree_lrs_client-1.0.3/cashfree_lrs_client/models/purpose.py
+-rw-r--r--   0        0        0     1943 2023-05-01 08:08:38.271853 cashfree_lrs_client-1.0.3/cashfree_lrs_client/models/setup_webhooks200_response.py
+-rw-r--r--   0        0        0     2361 2023-05-01 08:09:00.564025 cashfree_lrs_client-1.0.3/cashfree_lrs_client/models/setup_webhooks_request.py
+-rw-r--r--   0        0        0     1909 2023-05-01 08:09:00.568025 cashfree_lrs_client-1.0.3/cashfree_lrs_client/models/success_message.py
+-rw-r--r--   0        0        0      644 2023-05-01 08:08:38.271853 cashfree_lrs_client-1.0.3/cashfree_lrs_client/paths/__init__.py
+-rw-r--r--   0        0        0      323 2023-05-01 08:08:38.271853 cashfree_lrs_client-1.0.3/cashfree_lrs_client/paths/beneficiaries/__init__.py
+-rw-r--r--   0        0        0    12582 2023-05-01 08:08:38.271853 cashfree_lrs_client-1.0.3/cashfree_lrs_client/paths/beneficiaries/post.py
+-rw-r--r--   0        0        0    12396 2023-05-01 08:08:38.271853 cashfree_lrs_client-1.0.3/cashfree_lrs_client/paths/beneficiaries/post.pyi
+-rw-r--r--   0        0        0      326 2023-05-01 08:08:38.271853 cashfree_lrs_client-1.0.3/cashfree_lrs_client/paths/fx_rate_details/__init__.py
+-rw-r--r--   0        0        0    11760 2023-05-01 08:08:38.271853 cashfree_lrs_client-1.0.3/cashfree_lrs_client/paths/fx_rate_details/post.py
+-rw-r--r--   0        0        0    11604 2023-05-01 08:08:38.271853 cashfree_lrs_client-1.0.3/cashfree_lrs_client/paths/fx_rate_details/post.pyi
+-rw-r--r--   0        0        0      309 2023-05-01 08:08:38.271853 cashfree_lrs_client-1.0.3/cashfree_lrs_client/paths/orders/__init__.py
+-rw-r--r--   0        0        0    13005 2023-05-01 08:08:38.271853 cashfree_lrs_client-1.0.3/cashfree_lrs_client/paths/orders/post.py
+-rw-r--r--   0        0        0    12789 2023-05-01 08:08:38.271853 cashfree_lrs_client-1.0.3/cashfree_lrs_client/paths/orders/post.pyi
+-rw-r--r--   0        0        0      343 2023-05-01 08:08:38.271853 cashfree_lrs_client-1.0.3/cashfree_lrs_client/paths/orders_documents_upload/__init__.py
+-rw-r--r--   0        0        0    12334 2023-05-01 08:08:38.271853 cashfree_lrs_client-1.0.3/cashfree_lrs_client/paths/orders_documents_upload/post.py
+-rw-r--r--   0        0        0    12148 2023-05-01 08:08:38.271853 cashfree_lrs_client-1.0.3/cashfree_lrs_client/paths/orders_documents_upload/post.pyi
+-rw-r--r--   0        0        0      361 2023-05-01 08:08:38.271853 cashfree_lrs_client-1.0.3/cashfree_lrs_client/paths/orders_order_id_documents_upload/__init__.py
+-rw-r--r--   0        0        0    15715 2023-05-01 08:08:38.271853 cashfree_lrs_client-1.0.3/cashfree_lrs_client/paths/orders_order_id_documents_upload/post.py
+-rw-r--r--   0        0        0    15469 2023-05-01 08:08:38.271853 cashfree_lrs_client-1.0.3/cashfree_lrs_client/paths/orders_order_id_documents_upload/post.pyi
+-rw-r--r--   0        0        0      343 2023-05-01 08:08:38.271853 cashfree_lrs_client-1.0.3/cashfree_lrs_client/paths/orders_order_id_process/__init__.py
+-rw-r--r--   0        0        0     8093 2023-05-01 08:08:38.271853 cashfree_lrs_client-1.0.3/cashfree_lrs_client/paths/orders_order_id_process/post.py
+-rw-r--r--   0        0        0     7937 2023-05-01 08:08:38.271853 cashfree_lrs_client-1.0.3/cashfree_lrs_client/paths/orders_order_id_process/post.pyi
+-rw-r--r--   0        0        0      315 2023-05-01 08:08:38.271853 cashfree_lrs_client-1.0.3/cashfree_lrs_client/paths/remitters/__init__.py
+-rw-r--r--   0        0        0    12525 2023-05-01 08:08:38.271853 cashfree_lrs_client-1.0.3/cashfree_lrs_client/paths/remitters/post.py
+-rw-r--r--   0        0        0    12339 2023-05-01 08:08:38.271853 cashfree_lrs_client-1.0.3/cashfree_lrs_client/paths/remitters/post.pyi
+-rw-r--r--   0        0        0      313 2023-05-01 08:08:38.271853 cashfree_lrs_client-1.0.3/cashfree_lrs_client/paths/webhooks/__init__.py
+-rw-r--r--   0        0        0    11939 2023-05-01 08:08:38.271853 cashfree_lrs_client-1.0.3/cashfree_lrs_client/paths/webhooks/post.py
+-rw-r--r--   0        0        0    11783 2023-05-01 08:08:38.271853 cashfree_lrs_client-1.0.3/cashfree_lrs_client/paths/webhooks/post.pyi
+-rw-r--r--   0        0        0    12643 2023-05-01 08:09:00.728026 cashfree_lrs_client-1.0.3/cashfree_lrs_client/rest.py
+-rw-r--r--   0        0        0    97649 2023-05-01 08:08:38.271853 cashfree_lrs_client-1.0.3/cashfree_lrs_client/schemas.py
+-rw-r--r--   0        0        0        0 2023-05-01 08:08:38.271853 cashfree_lrs_client-1.0.3/cashfree_lrs_client/test/__init__.py
+-rw-r--r--   0        0        0     2694 2023-05-01 08:08:38.271853 cashfree_lrs_client-1.0.3/cashfree_lrs_client/test/test_create_beneficiary_request.py
+-rw-r--r--   0        0        0     2292 2023-05-01 08:08:38.271853 cashfree_lrs_client-1.0.3/cashfree_lrs_client/test/test_create_order_request.py
+-rw-r--r--   0        0        0     1952 2023-05-01 08:08:38.271853 cashfree_lrs_client-1.0.3/cashfree_lrs_client/test/test_create_order_response.py
+-rw-r--r--   0        0        0     2486 2023-05-01 08:08:38.271853 cashfree_lrs_client-1.0.3/cashfree_lrs_client/test/test_create_remitter_request.py
+-rw-r--r--   0        0        0      738 2023-05-01 08:08:38.271853 cashfree_lrs_client-1.0.3/cashfree_lrs_client/test/test_currency.py
+-rw-r--r--   0        0        0     1439 2023-05-01 08:08:38.271853 cashfree_lrs_client-1.0.3/cashfree_lrs_client/test/test_error.py
+-rw-r--r--   0        0        0     1860 2023-05-01 08:08:38.271853 cashfree_lrs_client-1.0.3/cashfree_lrs_client/test/test_fetch_forex_rate_request.py
+-rw-r--r--   0        0        0     1845 2023-05-01 08:08:38.271853 cashfree_lrs_client-1.0.3/cashfree_lrs_client/test/test_lrs_api.py
+-rw-r--r--   0        0        0      731 2023-05-01 08:08:38.271853 cashfree_lrs_client-1.0.3/cashfree_lrs_client/test/test_purpose.py
+-rw-r--r--   0        0        0     1737 2023-05-01 08:08:38.271853 cashfree_lrs_client-1.0.3/cashfree_lrs_client/test/test_setup_webhooks_request.py
+-rw-r--r--   0        0        0     1493 2023-05-01 08:08:38.271853 cashfree_lrs_client-1.0.3/cashfree_lrs_client/test/test_success_message.py
+-rw-r--r--   0        0        0      683 2023-05-01 08:09:00.704026 cashfree_lrs_client-1.0.3/pyproject.toml
+-rw-r--r--   0        0        0     6116 1970-01-01 00:00:00.000000 cashfree_lrs_client-1.0.3/PKG-INFO
```

### Comparing `cashfree_lrs_client-1.0.2/cashfree_lrs_client/api/default_api.py` & `cashfree_lrs_client-1.0.3/cashfree_lrs_client/api/default_api.py`

 * *Files identical despite different names*

### Comparing `cashfree_lrs_client-1.0.2/cashfree_lrs_client/api/lrs_api.py` & `cashfree_lrs_client-1.0.3/cashfree_lrs_client/api/lrs_api.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,30 +1,31 @@
 # coding: utf-8
 
 """
     Cashfree LRS
 
     CashFree LRS APIs (v2)  # noqa: E501
 
-    The version of the OpenAPI document: 1.0.0
+    The version of the OpenAPI document: 1.0.3
     Contact: nextgenapi@cashfree.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
 
 
 import re  # noqa: F401
+import io
 
 from pydantic import validate_arguments, ValidationError
 from typing_extensions import Annotated
 
 from pydantic import Field, StrictBytes, StrictStr, conlist
 
-from typing import Any, Dict, Optional
+from typing import Any, Dict, Optional, Union
 
 from cashfree_lrs_client.models.create_beneficiary_request import CreateBeneficiaryRequest
 from cashfree_lrs_client.models.create_order_request import CreateOrderRequest
 from cashfree_lrs_client.models.create_order_response import CreateOrderResponse
 from cashfree_lrs_client.models.create_remitter_request import CreateRemitterRequest
 from cashfree_lrs_client.models.fetch_forex_rate_request import FetchForexRateRequest
 from cashfree_lrs_client.models.setup_webhooks_request import SetupWebhooksRequest
@@ -46,15 +47,15 @@
 
     def __init__(self, api_client=None):
         if api_client is None:
             api_client = ApiClient.get_default()
         self.api_client = api_client
 
     @validate_arguments
-    def bulk_documents_upload(self, files : Annotated[conlist(StrictBytes), Field(..., description="Upload multiple document at a time. Accepted file type - .pdf. Maximum file size - 20 MB")], **kwargs) -> None:  # noqa: E501
+    def bulk_documents_upload(self, files : Annotated[conlist(Union[StrictBytes, StrictStr]), Field(..., description="Upload multiple document at a time. Accepted file type - .pdf. Maximum file size - 20 MB")], **kwargs) -> None:  # noqa: E501
         """Upload Documents in Bulk  # noqa: E501
 
         Use this API to Upload documents before Order creation  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
         >>> thread = api.bulk_documents_upload(files, async_req=True)
@@ -77,15 +78,15 @@
                  returns the request thread.
         :rtype: None
         """
         kwargs['_return_http_data_only'] = True
         return self.bulk_documents_upload_with_http_info(files, **kwargs)  # noqa: E501
 
     @validate_arguments
-    def bulk_documents_upload_with_http_info(self, files : Annotated[conlist(StrictBytes), Field(..., description="Upload multiple document at a time. Accepted file type - .pdf. Maximum file size - 20 MB")], **kwargs):  # noqa: E501
+    def bulk_documents_upload_with_http_info(self, files : Annotated[conlist(Union[StrictBytes, StrictStr]), Field(..., description="Upload multiple document at a time. Accepted file type - .pdf. Maximum file size - 20 MB")], **kwargs):  # noqa: E501
         """Upload Documents in Bulk  # noqa: E501
 
         Use this API to Upload documents before Order creation  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
         >>> thread = api.bulk_documents_upload_with_http_info(files, async_req=True)
@@ -300,15 +301,15 @@
         # process the header parameters
         _header_params = dict(_params.get('_headers', {}))
         # process the form parameters
         _form_params = []
         _files = {}
         # process the body parameter
         _body_params = None
-        if _params['create_beneficiary_request']:
+        if _params['create_beneficiary_request'] is not None:
             _body_params = _params['create_beneficiary_request']
 
         # set the HTTP header `Accept`
         _header_params['Accept'] = self.api_client.select_header_accept(
             ['application/json'])  # noqa: E501
 
         # set the HTTP header `Content-Type`
@@ -448,15 +449,15 @@
         # process the header parameters
         _header_params = dict(_params.get('_headers', {}))
         # process the form parameters
         _form_params = []
         _files = {}
         # process the body parameter
         _body_params = None
-        if _params['create_order_request']:
+        if _params['create_order_request'] is not None:
             _body_params = _params['create_order_request']
 
         # set the HTTP header `Accept`
         _header_params['Accept'] = self.api_client.select_header_accept(
             ['application/json'])  # noqa: E501
 
         # set the HTTP header `Content-Type`
@@ -597,15 +598,15 @@
         # process the header parameters
         _header_params = dict(_params.get('_headers', {}))
         # process the form parameters
         _form_params = []
         _files = {}
         # process the body parameter
         _body_params = None
-        if _params['create_remitter_request']:
+        if _params['create_remitter_request'] is not None:
             _body_params = _params['create_remitter_request']
 
         # set the HTTP header `Accept`
         _header_params['Accept'] = self.api_client.select_header_accept(
             ['application/json'])  # noqa: E501
 
         # set the HTTP header `Content-Type`
@@ -745,15 +746,15 @@
         # process the header parameters
         _header_params = dict(_params.get('_headers', {}))
         # process the form parameters
         _form_params = []
         _files = {}
         # process the body parameter
         _body_params = None
-        if _params['fetch_forex_rate_request']:
+        if _params['fetch_forex_rate_request'] is not None:
             _body_params = _params['fetch_forex_rate_request']
 
         # set the HTTP header `Accept`
         _header_params['Accept'] = self.api_client.select_header_accept(
             ['application/json'])  # noqa: E501
 
         # set the HTTP header `Content-Type`
@@ -1024,15 +1025,15 @@
         # process the header parameters
         _header_params = dict(_params.get('_headers', {}))
         # process the form parameters
         _form_params = []
         _files = {}
         # process the body parameter
         _body_params = None
-        if _params['setup_webhooks_request']:
+        if _params['setup_webhooks_request'] is not None:
             _body_params = _params['setup_webhooks_request']
 
         # set the HTTP header `Accept`
         _header_params['Accept'] = self.api_client.select_header_accept(
             ['application/json'])  # noqa: E501
 
         # set the HTTP header `Content-Type`
@@ -1063,15 +1064,15 @@
             _return_http_data_only=_params.get('_return_http_data_only'),  # noqa: E501
             _preload_content=_params.get('_preload_content', True),
             _request_timeout=_params.get('_request_timeout'),
             collection_formats=_collection_formats,
             _request_auth=_params.get('_request_auth'))
 
     @validate_arguments
-    def upload_documents(self, order_id : Annotated[StrictStr, Field(..., description="The subject Order ID")], files : Annotated[conlist(StrictBytes), Field(..., description="Upload multiple document at a time. Accepted file type - .pdf. Maximum file size - 20 MB")], **kwargs) -> object:  # noqa: E501
+    def upload_documents(self, order_id : Annotated[StrictStr, Field(..., description="The subject Order ID")], files : Annotated[conlist(Union[StrictBytes, StrictStr]), Field(..., description="Upload multiple document at a time. Accepted file type - .pdf. Maximum file size - 20 MB")], **kwargs) -> object:  # noqa: E501
         """Upload Documents  # noqa: E501
 
         Use this API to Upload documents on your Order ID.  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
         >>> thread = api.upload_documents(order_id, files, async_req=True)
@@ -1096,15 +1097,15 @@
                  returns the request thread.
         :rtype: object
         """
         kwargs['_return_http_data_only'] = True
         return self.upload_documents_with_http_info(order_id, files, **kwargs)  # noqa: E501
 
     @validate_arguments
-    def upload_documents_with_http_info(self, order_id : Annotated[StrictStr, Field(..., description="The subject Order ID")], files : Annotated[conlist(StrictBytes), Field(..., description="Upload multiple document at a time. Accepted file type - .pdf. Maximum file size - 20 MB")], **kwargs):  # noqa: E501
+    def upload_documents_with_http_info(self, order_id : Annotated[StrictStr, Field(..., description="The subject Order ID")], files : Annotated[conlist(Union[StrictBytes, StrictStr]), Field(..., description="Upload multiple document at a time. Accepted file type - .pdf. Maximum file size - 20 MB")], **kwargs):  # noqa: E501
         """Upload Documents  # noqa: E501
 
         Use this API to Upload documents on your Order ID.  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
         >>> thread = api.upload_documents_with_http_info(order_id, files, async_req=True)
```

### Comparing `cashfree_lrs_client-1.0.2/cashfree_lrs_client/apis/path_to_api.py` & `cashfree_lrs_client-1.0.3/cashfree_lrs_client/apis/path_to_api.py`

 * *Files identical despite different names*

### Comparing `cashfree_lrs_client-1.0.2/cashfree_lrs_client/apis/tags/lrs_api.py` & `cashfree_lrs_client-1.0.3/cashfree_lrs_client/apis/tags/lrs_api.py`

 * *Files identical despite different names*

### Comparing `cashfree_lrs_client-1.0.2/cashfree_lrs_client/configuration.py` & `cashfree_lrs_client-1.0.3/cashfree_lrs_client/configuration.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,85 +1,62 @@
 # coding: utf-8
 
 """
     Cashfree LRS
 
     CashFree LRS APIs (v2)  # noqa: E501
 
-    The version of the OpenAPI document: 1.0.2
+    The version of the OpenAPI document: 1.0.3
     Contact: nextgenapi@cashfree.com
-    Generated by: https://openapi-generator.tech
+    Generated by OpenAPI Generator (https://openapi-generator.tech)
+
+    Do not edit the class manually.
 """
 
+
 import copy
 import logging
 import multiprocessing
 import sys
 import urllib3
 
-from http import client as http_client
+import http.client as httplib
 from cashfree_lrs_client.exceptions import ApiValueError
 
-
 JSON_SCHEMA_VALIDATION_KEYWORDS = {
     'multipleOf', 'maximum', 'exclusiveMaximum',
     'minimum', 'exclusiveMinimum', 'maxLength',
-    'minLength', 'pattern', 'maxItems', 'minItems',
-    'uniqueItems', 'maxProperties', 'minProperties',
+    'minLength', 'pattern', 'maxItems', 'minItems'
 }
 
 class Configuration(object):
-    """NOTE: This class is auto generated by OpenAPI Generator
-
-    Ref: https://openapi-generator.tech
-    Do not edit the class manually.
+    """This class contains various settings of the API client.
 
-    :param host: Base url
+    :param host: Base url.
     :param api_key: Dict to store API key(s).
       Each entry in the dict specifies an API key.
       The dict key is the name of the security scheme in the OAS specification.
       The dict value is the API key secret.
-    :param api_key_prefix: Dict to store API prefix (e.g. Bearer)
+    :param api_key_prefix: Dict to store API prefix (e.g. Bearer).
       The dict key is the name of the security scheme in the OAS specification.
       The dict value is an API key prefix when generating the auth data.
-    :param username: Username for HTTP basic authentication
-    :param password: Password for HTTP basic authentication
-    :param discard_unknown_keys: Boolean value indicating whether to discard
-      unknown properties. A server may send a response that includes additional
-      properties that are not known by the client in the following scenarios:
-      1. The OpenAPI document is incomplete, i.e. it does not match the server
-         implementation.
-      2. The client was generated using an older version of the OpenAPI document
-         and the server has been upgraded since then.
-      If a schema in the OpenAPI document defines the additionalProperties attribute,
-      then all undeclared properties received by the server are injected into the
-      additional properties map. In that case, there are undeclared properties, and
-      nothing to discard.
-    :param disabled_client_side_validations (string): Comma-separated list of
-      JSON schema validation keywords to disable JSON schema structural validation
-      rules. The following keywords may be specified: multipleOf, maximum,
-      exclusiveMaximum, minimum, exclusiveMinimum, maxLength, minLength, pattern,
-      maxItems, minItems.
-      By default, the validation is performed for data generated locally by the client
-      and data received from the server, independent of any validation performed by
-      the server side. If the input data does not satisfy the JSON schema validation
-      rules specified in the OpenAPI document, an exception is raised.
-      If disabled_client_side_validations is set, structural validation is
-      disabled. This can be useful to troubleshoot data validation problem, such as
-      when the OpenAPI document validation rules do not match the actual API data
-      received by the server.
+    :param username: Username for HTTP basic authentication.
+    :param password: Password for HTTP basic authentication.
+    :param access_token: Access token.
     :param server_index: Index to servers configuration.
     :param server_variables: Mapping with string values to replace variables in
       templated server configuration. The validation of enums is performed for
       variables with defined enum values before.
     :param server_operation_index: Mapping from operation ID to an index to server
       configuration.
     :param server_operation_variables: Mapping from operation ID to a mapping with
       string values to replace variables in templated server configuration.
       The validation of enums is performed for variables with defined enum values before.
+    :param ssl_ca_cert: str - the path to a file of concatenated CA certificates
+      in PEM format.
 
     :Example:
 
     API Key Authentication Example.
     Given the following security scheme in the OpenAPI specification:
       components:
         securitySchemes:
@@ -97,26 +74,22 @@
 
     The following cookie will be added to the HTTP request:
        Cookie: JSESSIONID abc123
     """
 
     _default = None
 
-    def __init__(
-        self,
-        host=None,
-        api_key=None,
-        api_key_prefix=None,
-        discard_unknown_keys=False,
-        disabled_client_side_validations="",
-        server_index=None,
-        server_variables=None,
-        server_operation_index=None,
-        server_operation_variables=None,
-    ):
+    def __init__(self, host=None,
+                 api_key=None, api_key_prefix=None,
+                 username=None, password=None,
+                 access_token=None,
+                 server_index=None, server_variables=None,
+                 server_operation_index=None, server_operation_variables=None,
+                 ssl_ca_cert=None,
+                 ):
         """Constructor
         """
         self._base_path = "https://sandbox.cashfree.com/pg/lrs" if host is None else host
         """Default Base url
         """
         self.server_index = 0 if server_index is None and host is None else server_index
         self.server_operation_index = server_operation_index or {}
@@ -139,15 +112,23 @@
         if api_key_prefix:
             self.api_key_prefix = api_key_prefix
         """dict to store API prefix (e.g. Bearer)
         """
         self.refresh_api_key_hook = None
         """function hook to refresh API key if expired
         """
-        self.disabled_client_side_validations = disabled_client_side_validations
+        self.username = username
+        """Username for HTTP basic authentication
+        """
+        self.password = password
+        """Password for HTTP basic authentication
+        """
+        self.access_token = access_token
+        """Access token
+        """
         self.logger = {}
         """Logging Settings
         """
         self.logger["package_logger"] = logging.getLogger("cashfree_lrs_client")
         self.logger["urllib3_logger"] = logging.getLogger("urllib3")
         self.logger_format = '%(asctime)s %(levelname)s %(message)s'
         """Log format
@@ -166,15 +147,15 @@
         """
 
         self.verify_ssl = True
         """SSL/TLS verification
            Set this to false to skip verifying SSL certificate when calling API
            from https server.
         """
-        self.ssl_ca_cert = None
+        self.ssl_ca_cert = ssl_ca_cert
         """Set this to customize the certificate file to verify the peer.
         """
         self.cert_file = None
         """client certificate file
         """
         self.key_file = None
         """client key file
@@ -202,16 +183,25 @@
         """
         self.retries = None
         """Adding retries to override urllib3 default value 3
         """
         # Enable client side validation
         self.client_side_validation = True
 
-        # Options to pass down to the underlying urllib3 socket
         self.socket_options = None
+        """Options to pass down to the underlying urllib3 socket
+        """
+
+        self.datetime_format = "%Y-%m-%dT%H:%M:%S.%f%z"
+        """datetime format
+        """
+
+        self.date_format = "%Y-%m-%d"
+        """date format
+        """
 
     def __deepcopy__(self, memo):
         cls = self.__class__
         result = cls.__new__(cls)
         memo[id(self)] = result
         for k, v in self.__dict__.items():
             if k not in ('logger', 'logger_file_handler'):
@@ -221,46 +211,49 @@
         # use setters to configure loggers
         result.logger_file = self.logger_file
         result.debug = self.debug
         return result
 
     def __setattr__(self, name, value):
         object.__setattr__(self, name, value)
-        if name == 'disabled_client_side_validations':
-            s = set(filter(None, value.split(',')))
-            for v in s:
-                if v not in JSON_SCHEMA_VALIDATION_KEYWORDS:
-                    raise ApiValueError(
-                        "Invalid keyword: '{0}''".format(v))
-            self._disabled_client_side_validations = s
 
     @classmethod
     def set_default(cls, default):
         """Set default instance of configuration.
 
         It stores default configuration, which can be
         returned by get_default_copy method.
 
         :param default: object of Configuration
         """
-        cls._default = copy.deepcopy(default)
+        cls._default = default
 
     @classmethod
     def get_default_copy(cls):
-        """Return new instance of configuration.
+        """Deprecated. Please use `get_default` instead.
+
+        Deprecated. Please use `get_default` instead.
+
+        :return: The configuration object.
+        """
+        return cls.get_default()
+
+    @classmethod
+    def get_default(cls):
+        """Return the default configuration.
 
         This method returns newly created, based on default constructor,
         object of Configuration class or returns a copy of default
-        configuration passed by the set_default method.
+        configuration.
 
         :return: The configuration object.
         """
-        if cls._default is not None:
-            return copy.deepcopy(cls._default)
-        return Configuration()
+        if cls._default is None:
+            cls._default = Configuration()
+        return cls._default
 
     @property
     def logger_file(self):
         """The logger file.
 
         If the logger_file is None, then add stream handler and remove file
         handler. Otherwise, add file handler and remove stream handler.
@@ -306,23 +299,23 @@
         :type: bool
         """
         self.__debug = value
         if self.__debug:
             # if debug status is True, turn on debug logging
             for _, logger in self.logger.items():
                 logger.setLevel(logging.DEBUG)
-            # turn on http_client debug
-            http_client.HTTPConnection.debuglevel = 1
+            # turn on httplib debug
+            httplib.HTTPConnection.debuglevel = 1
         else:
             # if debug status is False, turn off debug logging,
             # setting log level to default `logging.WARNING`
             for _, logger in self.logger.items():
                 logger.setLevel(logging.WARNING)
-            # turn off http_client debug
-            http_client.HTTPConnection.debuglevel = 0
+            # turn off httplib debug
+            httplib.HTTPConnection.debuglevel = 0
 
     @property
     def logger_format(self):
         """The logger format.
 
         The logger_formatter will be updated when sets logger_format.
 
@@ -414,16 +407,16 @@
         """Gets the essential information for debugging.
 
         :return: The report for debugging.
         """
         return "Python SDK Debug Report:\n"\
                "OS: {env}\n"\
                "Python Version: {pyversion}\n"\
-               "Version of the API: 1.0.2\n"\
-               "SDK Package Version: 1.0.0".\
+               "Version of the API: 1.0.3\n"\
+               "SDK Package Version: 1.0.3".\
                format(env=sys.platform, pyversion=sys.version)
 
     def get_host_settings(self):
         """Gets an array of host settings
 
         :return: An array of host settings
         """
```

### Comparing `cashfree_lrs_client-1.0.2/cashfree_lrs_client/docs/CreateBeneficiaryRequest.md` & `cashfree_lrs_client-1.0.3/cashfree_lrs_client/docs/CreateBeneficiaryRequest.md`

 * *Files identical despite different names*

### Comparing `cashfree_lrs_client-1.0.2/cashfree_lrs_client/docs/CreateOrderRequest.md` & `cashfree_lrs_client-1.0.3/cashfree_lrs_client/docs/CreateOrderRequest.md`

 * *Files identical despite different names*

### Comparing `cashfree_lrs_client-1.0.2/cashfree_lrs_client/docs/CreateOrderResponse.md` & `cashfree_lrs_client-1.0.3/cashfree_lrs_client/docs/CreateOrderResponse.md`

 * *Files identical despite different names*

### Comparing `cashfree_lrs_client-1.0.2/cashfree_lrs_client/docs/CreateRemitterRequest.md` & `cashfree_lrs_client-1.0.3/cashfree_lrs_client/docs/CreateRemitterRequest.md`

 * *Files identical despite different names*

### Comparing `cashfree_lrs_client-1.0.2/cashfree_lrs_client/docs/Error.md` & `cashfree_lrs_client-1.0.3/cashfree_lrs_client/docs/Error.md`

 * *Files identical despite different names*

### Comparing `cashfree_lrs_client-1.0.2/cashfree_lrs_client/docs/FetchForexRateRequest.md` & `cashfree_lrs_client-1.0.3/cashfree_lrs_client/docs/FetchForexRateRequest.md`

 * *Files identical despite different names*

### Comparing `cashfree_lrs_client-1.0.2/cashfree_lrs_client/docs/LrsApi.md` & `cashfree_lrs_client-1.0.3/cashfree_lrs_client/docs/LrsApi.md`

 * *Files identical despite different names*

### Comparing `cashfree_lrs_client-1.0.2/cashfree_lrs_client/docs/SetupWebhooksRequest.md` & `cashfree_lrs_client-1.0.3/cashfree_lrs_client/docs/SetupWebhooksRequest.md`

 * *Files identical despite different names*

### Comparing `cashfree_lrs_client-1.0.2/cashfree_lrs_client/docs/SuccessMessage.md` & `cashfree_lrs_client-1.0.3/cashfree_lrs_client/docs/SuccessMessage.md`

 * *Files identical despite different names*

### Comparing `cashfree_lrs_client-1.0.2/cashfree_lrs_client/exceptions.py` & `cashfree_lrs_client-1.0.3/cashfree_lrs_client/exceptions.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,22 +1,20 @@
 # coding: utf-8
 
 """
     Cashfree LRS
 
     CashFree LRS APIs (v2)  # noqa: E501
 
-    The version of the OpenAPI document: 1.0.2
+    The version of the OpenAPI document: 1.0.3
     Contact: nextgenapi@cashfree.com
-    Generated by: https://openapi-generator.tech
-"""
-import dataclasses
-import typing
+    Generated by OpenAPI Generator (https://openapi-generator.tech)
 
-from urllib3._collections import HTTPHeaderDict
+    Do not edit the class manually.
+"""
 
 
 class OpenApiException(Exception):
     """The base exception class for all OpenAPIExceptions"""
 
 
 class ApiTypeError(OpenApiException, TypeError):
@@ -98,34 +96,27 @@
         self.path_to_item = path_to_item
         full_msg = msg
         if path_to_item:
             full_msg = "{0} at {1}".format(msg, render_path(path_to_item))
         super(ApiKeyError, self).__init__(full_msg)
 
 
-T = typing.TypeVar("T")
+class ApiException(OpenApiException):
 
-
-@dataclasses.dataclass
-class ApiException(OpenApiException, typing.Generic[T]):
-    status: int
-    reason: str
-    api_response: typing.Optional[T] = None
-
-    @property
-    def body(self) -> typing.Union[str, bytes, None]:
-        if not self.api_response:
-            return None
-        return self.api_response.response.data
-
-    @property
-    def headers(self) -> typing.Optional[HTTPHeaderDict]:
-        if not self.api_response:
-            return None
-        return self.api_response.response.getheaders()
+    def __init__(self, status=None, reason=None, http_resp=None):
+        if http_resp:
+            self.status = http_resp.status
+            self.reason = http_resp.reason
+            self.body = http_resp.data
+            self.headers = http_resp.getheaders()
+        else:
+            self.status = status
+            self.reason = reason
+            self.body = None
+            self.headers = None
 
     def __str__(self):
         """Custom error messages for exception"""
         error_message = "({0})\n"\
                         "Reason: {1}\n".format(self.status, self.reason)
         if self.headers:
             error_message += "HTTP response headers: {0}\n".format(
@@ -133,14 +124,38 @@
 
         if self.body:
             error_message += "HTTP response body: {0}\n".format(self.body)
 
         return error_message
 
 
+class NotFoundException(ApiException):
+
+    def __init__(self, status=None, reason=None, http_resp=None):
+        super(NotFoundException, self).__init__(status, reason, http_resp)
+
+
+class UnauthorizedException(ApiException):
+
+    def __init__(self, status=None, reason=None, http_resp=None):
+        super(UnauthorizedException, self).__init__(status, reason, http_resp)
+
+
+class ForbiddenException(ApiException):
+
+    def __init__(self, status=None, reason=None, http_resp=None):
+        super(ForbiddenException, self).__init__(status, reason, http_resp)
+
+
+class ServiceException(ApiException):
+
+    def __init__(self, status=None, reason=None, http_resp=None):
+        super(ServiceException, self).__init__(status, reason, http_resp)
+
+
 def render_path(path_to_item):
     """Returns a string representation of a path"""
     result = ""
     for pth in path_to_item:
         if isinstance(pth, int):
             result += "[{0}]".format(pth)
         else:
```

### Comparing `cashfree_lrs_client-1.0.2/cashfree_lrs_client/model/amount.py` & `cashfree_lrs_client-1.0.3/cashfree_lrs_client/model/amount.py`

 * *Files identical despite different names*

### Comparing `cashfree_lrs_client-1.0.2/cashfree_lrs_client/model/amount.pyi` & `cashfree_lrs_client-1.0.3/cashfree_lrs_client/model/amount.pyi`

 * *Files identical despite different names*

### Comparing `cashfree_lrs_client-1.0.2/cashfree_lrs_client/model/create_beneficiary_request.py` & `cashfree_lrs_client-1.0.3/cashfree_lrs_client/model/create_beneficiary_request.py`

 * *Files identical despite different names*

### Comparing `cashfree_lrs_client-1.0.2/cashfree_lrs_client/model/create_beneficiary_request.pyi` & `cashfree_lrs_client-1.0.3/cashfree_lrs_client/model/create_beneficiary_request.pyi`

 * *Files identical despite different names*

### Comparing `cashfree_lrs_client-1.0.2/cashfree_lrs_client/model/create_order_request.py` & `cashfree_lrs_client-1.0.3/cashfree_lrs_client/model/create_order_request.py`

 * *Files identical despite different names*

### Comparing `cashfree_lrs_client-1.0.2/cashfree_lrs_client/model/create_order_request.pyi` & `cashfree_lrs_client-1.0.3/cashfree_lrs_client/model/create_order_request.pyi`

 * *Files identical despite different names*

### Comparing `cashfree_lrs_client-1.0.2/cashfree_lrs_client/model/create_order_response.py` & `cashfree_lrs_client-1.0.3/cashfree_lrs_client/model/create_order_response.py`

 * *Files identical despite different names*

### Comparing `cashfree_lrs_client-1.0.2/cashfree_lrs_client/model/create_order_response.pyi` & `cashfree_lrs_client-1.0.3/cashfree_lrs_client/model/create_order_response.pyi`

 * *Files identical despite different names*

### Comparing `cashfree_lrs_client-1.0.2/cashfree_lrs_client/model/create_remitter_request.py` & `cashfree_lrs_client-1.0.3/cashfree_lrs_client/model/create_remitter_request.py`

 * *Files identical despite different names*

### Comparing `cashfree_lrs_client-1.0.2/cashfree_lrs_client/model/create_remitter_request.pyi` & `cashfree_lrs_client-1.0.3/cashfree_lrs_client/model/create_remitter_request.pyi`

 * *Files identical despite different names*

### Comparing `cashfree_lrs_client-1.0.2/cashfree_lrs_client/model/currency.py` & `cashfree_lrs_client-1.0.3/cashfree_lrs_client/model/currency.py`

 * *Files identical despite different names*

### Comparing `cashfree_lrs_client-1.0.2/cashfree_lrs_client/model/currency.pyi` & `cashfree_lrs_client-1.0.3/cashfree_lrs_client/model/currency.pyi`

 * *Files identical despite different names*

### Comparing `cashfree_lrs_client-1.0.2/cashfree_lrs_client/model/error.py` & `cashfree_lrs_client-1.0.3/cashfree_lrs_client/model/error.py`

 * *Files identical despite different names*

### Comparing `cashfree_lrs_client-1.0.2/cashfree_lrs_client/model/error.pyi` & `cashfree_lrs_client-1.0.3/cashfree_lrs_client/model/error.pyi`

 * *Files identical despite different names*

### Comparing `cashfree_lrs_client-1.0.2/cashfree_lrs_client/model/fetch_forex_rate_request.py` & `cashfree_lrs_client-1.0.3/cashfree_lrs_client/model/fetch_forex_rate_request.py`

 * *Files identical despite different names*

### Comparing `cashfree_lrs_client-1.0.2/cashfree_lrs_client/model/fetch_forex_rate_request.pyi` & `cashfree_lrs_client-1.0.3/cashfree_lrs_client/model/fetch_forex_rate_request.pyi`

 * *Files identical despite different names*

### Comparing `cashfree_lrs_client-1.0.2/cashfree_lrs_client/model/purpose.py` & `cashfree_lrs_client-1.0.3/cashfree_lrs_client/model/purpose.py`

 * *Files identical despite different names*

### Comparing `cashfree_lrs_client-1.0.2/cashfree_lrs_client/model/purpose.pyi` & `cashfree_lrs_client-1.0.3/cashfree_lrs_client/model/purpose.pyi`

 * *Files identical despite different names*

### Comparing `cashfree_lrs_client-1.0.2/cashfree_lrs_client/model/setup_webhooks_request.py` & `cashfree_lrs_client-1.0.3/cashfree_lrs_client/model/setup_webhooks_request.py`

 * *Files identical despite different names*

### Comparing `cashfree_lrs_client-1.0.2/cashfree_lrs_client/model/setup_webhooks_request.pyi` & `cashfree_lrs_client-1.0.3/cashfree_lrs_client/model/setup_webhooks_request.pyi`

 * *Files identical despite different names*

### Comparing `cashfree_lrs_client-1.0.2/cashfree_lrs_client/model/success_message.py` & `cashfree_lrs_client-1.0.3/cashfree_lrs_client/model/success_message.py`

 * *Files identical despite different names*

### Comparing `cashfree_lrs_client-1.0.2/cashfree_lrs_client/model/success_message.pyi` & `cashfree_lrs_client-1.0.3/cashfree_lrs_client/model/success_message.pyi`

 * *Files identical despite different names*

### Comparing `cashfree_lrs_client-1.0.2/cashfree_lrs_client/models/__init__.py` & `cashfree_lrs_client-1.0.3/cashfree_lrs_client/__init__.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,24 +1,43 @@
 # coding: utf-8
 
 # flake8: noqa
 
-# import all models into this package
-# if you have many models here with many references from one model to another this may
-# raise a RecursionError
-# to avoid this, import only the models that you directly need like:
-# from cashfree_lrs_client.model.pet import Pet
-# or import this package, but before doing it, use:
-# import sys
-# sys.setrecursionlimit(n)
-
-from cashfree_lrs_client.model.amount import Amount
-from cashfree_lrs_client.model.create_beneficiary_request import CreateBeneficiaryRequest
-from cashfree_lrs_client.model.create_order_request import CreateOrderRequest
-from cashfree_lrs_client.model.create_order_response import CreateOrderResponse
-from cashfree_lrs_client.model.create_remitter_request import CreateRemitterRequest
-from cashfree_lrs_client.model.currency import Currency
-from cashfree_lrs_client.model.error import Error
-from cashfree_lrs_client.model.fetch_forex_rate_request import FetchForexRateRequest
-from cashfree_lrs_client.model.purpose import Purpose
-from cashfree_lrs_client.model.setup_webhooks_request import SetupWebhooksRequest
-from cashfree_lrs_client.model.success_message import SuccessMessage
+"""
+    Cashfree LRS
+
+    CashFree LRS APIs (v2)  # noqa: E501
+
+    The version of the OpenAPI document: 1.0.3
+    Contact: nextgenapi@cashfree.com
+    Generated by OpenAPI Generator (https://openapi-generator.tech)
+
+    Do not edit the class manually.
+"""
+
+
+__version__ = "1.0.3"
+
+# import apis into sdk package
+from cashfree_lrs_client.api.lrs_api import LrsApi
+
+# import ApiClient
+from cashfree_lrs_client.api_client import ApiClient
+from cashfree_lrs_client.configuration import Configuration
+from cashfree_lrs_client.exceptions import OpenApiException
+from cashfree_lrs_client.exceptions import ApiTypeError
+from cashfree_lrs_client.exceptions import ApiValueError
+from cashfree_lrs_client.exceptions import ApiKeyError
+from cashfree_lrs_client.exceptions import ApiAttributeError
+from cashfree_lrs_client.exceptions import ApiException
+
+# import models into sdk package
+from cashfree_lrs_client.models.create_beneficiary_request import CreateBeneficiaryRequest
+from cashfree_lrs_client.models.create_order_request import CreateOrderRequest
+from cashfree_lrs_client.models.create_order_response import CreateOrderResponse
+from cashfree_lrs_client.models.create_remitter_request import CreateRemitterRequest
+from cashfree_lrs_client.models.currency import Currency
+from cashfree_lrs_client.models.error import Error
+from cashfree_lrs_client.models.fetch_forex_rate_request import FetchForexRateRequest
+from cashfree_lrs_client.models.purpose import Purpose
+from cashfree_lrs_client.models.setup_webhooks_request import SetupWebhooksRequest
+from cashfree_lrs_client.models.success_message import SuccessMessage
```

### Comparing `cashfree_lrs_client-1.0.2/cashfree_lrs_client/models/create_beneficiary200_response.py` & `cashfree_lrs_client-1.0.3/cashfree_lrs_client/models/create_beneficiary200_response.py`

 * *Files identical despite different names*

### Comparing `cashfree_lrs_client-1.0.2/cashfree_lrs_client/models/create_beneficiary_request.py` & `cashfree_lrs_client-1.0.3/cashfree_lrs_client/models/create_beneficiary_request.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,24 +1,23 @@
 # coding: utf-8
 
 """
     Cashfree LRS
 
     CashFree LRS APIs (v2)  # noqa: E501
 
-    The version of the OpenAPI document: 1.0.0
+    The version of the OpenAPI document: 1.0.3
     Contact: nextgenapi@cashfree.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
 
 
 from __future__ import annotations
-from inspect import getfullargspec
 import pprint
 import re  # noqa: F401
 import json
 
 
 from typing import Optional
 from pydantic import BaseModel, Field, constr
@@ -43,14 +42,15 @@
     city: constr(strict=True, max_length=200, min_length=3) = Field(..., description="City in which the beneficiary resides. Only alphabets are allowed.")
     state: constr(strict=True, max_length=200, min_length=3) = Field(..., description="State in which the beneficiary resides. Only alphabets are allowed.")
     country: constr(strict=True, max_length=2, min_length=2) = Field(..., description="Country in which the beneficiary resides. Only alphabets are allowed.")
     postal_code: constr(strict=True, max_length=15, min_length=1) = Field(..., description="Postal code of the beneficiary. Only alphanumeric characters are allowed. A maximum of 15 charcaters is allowed.")
     __properties = ["beneficiary_id", "account_holder_name", "account_number", "swift_code", "iban", "routing_number", "bank_name", "bank_address", "bank_country", "sort_code", "transit_code", "bsb_number", "address", "city", "state", "country", "postal_code"]
 
     class Config:
+        """Pydantic configuration"""
         allow_population_by_field_name = True
         validate_assignment = True
 
     def to_str(self) -> str:
         """Returns the string representation of the model using alias"""
         return pprint.pformat(self.dict(by_alias=True))
 
@@ -73,15 +73,15 @@
 
     @classmethod
     def from_dict(cls, obj: dict) -> CreateBeneficiaryRequest:
         """Create an instance of CreateBeneficiaryRequest from a dict"""
         if obj is None:
             return None
 
-        if type(obj) is not dict:
+        if not isinstance(obj, dict):
             return CreateBeneficiaryRequest.parse_obj(obj)
 
         _obj = CreateBeneficiaryRequest.parse_obj({
             "beneficiary_id": obj.get("beneficiary_id"),
             "account_holder_name": obj.get("account_holder_name"),
             "account_number": obj.get("account_number"),
             "swift_code": obj.get("swift_code"),
```

### Comparing `cashfree_lrs_client-1.0.2/cashfree_lrs_client/models/create_order_request.py` & `cashfree_lrs_client-1.0.3/cashfree_lrs_client/models/create_order_request.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,60 +1,61 @@
 # coding: utf-8
 
 """
     Cashfree LRS
 
     CashFree LRS APIs (v2)  # noqa: E501
 
-    The version of the OpenAPI document: 1.0.0
+    The version of the OpenAPI document: 1.0.3
     Contact: nextgenapi@cashfree.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
 
 
 from __future__ import annotations
-from inspect import getfullargspec
 import pprint
 import re  # noqa: F401
 import json
 
 
-from typing import Optional
-from pydantic import BaseModel, Field, StrictBool, StrictStr, confloat, constr, validator
+from typing import Optional, Union
+from pydantic import BaseModel, Field, StrictBool, StrictStr, confloat, conint, constr, validator
 from cashfree_lrs_client.models.currency import Currency
 from cashfree_lrs_client.models.purpose import Purpose
 
 class CreateOrderRequest(BaseModel):
     """
-    CreateOrderRequest
+    
     """
     order_id: constr(strict=True, max_length=50, min_length=1) = Field(..., description="Unique Order Id to place the order. Alphanumeric characters, hyphens and underscores are allowed. Maximum of 50 characters is allowed.")
-    to_currency: Currency = ...
-    to_amount: confloat(ge=1, strict=True) = Field(..., description="Final settlement amount in to_currency (Double with 2 decimals allowed)")
-    from_amount: Optional[confloat(ge=1, strict=True)] = Field(None, description="Amount in INR excluding GST, TCS and handling charges (Double with 2 decimals allowed)")
-    purpose: Purpose = ...
+    to_currency: Currency = Field(...)
+    to_amount: Union[confloat(ge=1, strict=True), conint(ge=1, strict=True)] = Field(..., description="Final settlement amount in to_currency (Double with 2 decimals allowed)")
+    from_amount: Optional[Union[confloat(ge=1, strict=True), conint(ge=1, strict=True)]] = Field(None, description="Amount in INR excluding GST, TCS and handling charges (Double with 2 decimals allowed)")
+    purpose: Purpose = Field(...)
     return_url: constr(strict=True, max_length=300, min_length=3) = Field(..., description="The URL to which customer will be redirected to after the payment (should accept query params cf_id and cf_token).")
     remitter_id: constr(strict=True, max_length=50, min_length=1) = Field(..., description="Unique remitter ID to identify the remitter. Alphanumeric characters, hyphens, and underscores are allowed. Maximum of 50 characters are allowed.")
     beneficiary_id: constr(strict=True, max_length=50, min_length=1) = Field(..., description="Unique Beneficiary ID to identify the beneficiary. Alphanumeric characters and underscores are allowed. Maximum of 50 characters is allowed.")
     customer_declaration: Optional[StrictStr] = Field(None, description="Amount in INR declared by Customer (Double with 2 decimals allowed)")
     doc_ids: Optional[StrictStr] = Field(None, description="Comma seperated bulk_doc_id provided from the upload APIs.")
-    customer_relationship: StrictStr = ...
+    customer_relationship: StrictStr = Field(...)
     education_loan: Optional[StrictBool] = Field(False, description="Whether the remitter has availed an education loan")
     remarks: Optional[StrictStr] = Field(None, description="Student ID?")
     __properties = ["order_id", "to_currency", "to_amount", "from_amount", "purpose", "return_url", "remitter_id", "beneficiary_id", "customer_declaration", "doc_ids", "customer_relationship", "education_loan", "remarks"]
 
     @validator('customer_relationship')
-    def customer_relationship_validate_enum(cls, v):
-        if v not in ('SELF', 'SON'):
+    def customer_relationship_validate_enum(cls, value):
+        """Validates the enum"""
+        if value not in ('SELF', 'SON'):
             raise ValueError("must be one of enum values ('SELF', 'SON')")
-        return v
+        return value
 
     class Config:
+        """Pydantic configuration"""
         allow_population_by_field_name = True
         validate_assignment = True
 
     def to_str(self) -> str:
         """Returns the string representation of the model using alias"""
         return pprint.pformat(self.dict(by_alias=True))
 
@@ -77,15 +78,15 @@
 
     @classmethod
     def from_dict(cls, obj: dict) -> CreateOrderRequest:
         """Create an instance of CreateOrderRequest from a dict"""
         if obj is None:
             return None
 
-        if type(obj) is not dict:
+        if not isinstance(obj, dict):
             return CreateOrderRequest.parse_obj(obj)
 
         _obj = CreateOrderRequest.parse_obj({
             "order_id": obj.get("order_id"),
             "to_currency": obj.get("to_currency"),
             "to_amount": obj.get("to_amount"),
             "from_amount": obj.get("from_amount"),
```

### Comparing `cashfree_lrs_client-1.0.2/cashfree_lrs_client/models/create_order_response.py` & `cashfree_lrs_client-1.0.3/cashfree_lrs_client/models/order_response.py`

 * *Files 8% similar despite different names*

```diff
@@ -19,17 +19,17 @@
 import re  # noqa: F401
 import json
 
 from datetime import datetime
 from typing import List, Optional
 from pydantic import BaseModel, StrictStr, confloat, conlist
 
-class CreateOrderResponse(BaseModel):
+class OrderResponse(BaseModel):
     """
-    CreateOrderResponse
+    OrderResponse
     """
     tcs: Optional[confloat(ge=0, strict=True)] = None
     gst: Optional[confloat(ge=0, strict=True)] = None
     fx_rate: Optional[confloat(ge=0, strict=True)] = None
     amount_to_pay: Optional[confloat(ge=0, strict=True)] = None
     handling_charges: Optional[confloat(ge=0, strict=True)] = None
     order_expiry_time: Optional[datetime] = None
@@ -47,36 +47,36 @@
         return pprint.pformat(self.dict(by_alias=True))
 
     def to_json(self) -> str:
         """Returns the JSON representation of the model using alias"""
         return json.dumps(self.to_dict())
 
     @classmethod
-    def from_json(cls, json_str: str) -> CreateOrderResponse:
-        """Create an instance of CreateOrderResponse from a JSON string"""
+    def from_json(cls, json_str: str) -> OrderResponse:
+        """Create an instance of OrderResponse from a JSON string"""
         return cls.from_dict(json.loads(json_str))
 
     def to_dict(self):
         """Returns the dictionary representation of the model using alias"""
         _dict = self.dict(by_alias=True,
                           exclude={
                           },
                           exclude_none=True)
         return _dict
 
     @classmethod
-    def from_dict(cls, obj: dict) -> CreateOrderResponse:
-        """Create an instance of CreateOrderResponse from a dict"""
+    def from_dict(cls, obj: dict) -> OrderResponse:
+        """Create an instance of OrderResponse from a dict"""
         if obj is None:
             return None
 
         if type(obj) is not dict:
-            return CreateOrderResponse.parse_obj(obj)
+            return OrderResponse.parse_obj(obj)
 
-        _obj = CreateOrderResponse.parse_obj({
+        _obj = OrderResponse.parse_obj({
             "tcs": obj.get("tcs"),
             "gst": obj.get("gst"),
             "fx_rate": obj.get("fx_rate"),
             "amount_to_pay": obj.get("amount_to_pay"),
             "handling_charges": obj.get("handling_charges"),
             "order_expiry_time": obj.get("order_expiry_time"),
             "payment_link": obj.get("payment_link"),
```

### Comparing `cashfree_lrs_client-1.0.2/cashfree_lrs_client/models/create_remitter200_response.py` & `cashfree_lrs_client-1.0.3/cashfree_lrs_client/models/create_remitter200_response.py`

 * *Files identical despite different names*

### Comparing `cashfree_lrs_client-1.0.2/cashfree_lrs_client/models/create_remitter_request.py` & `cashfree_lrs_client-1.0.3/cashfree_lrs_client/models/create_remitter_request.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,39 +1,38 @@
 # coding: utf-8
 
 """
     Cashfree LRS
 
     CashFree LRS APIs (v2)  # noqa: E501
 
-    The version of the OpenAPI document: 1.0.0
+    The version of the OpenAPI document: 1.0.3
     Contact: nextgenapi@cashfree.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
 
 
 from __future__ import annotations
-from inspect import getfullargspec
 import pprint
 import re  # noqa: F401
 import json
 
 
 from typing import Optional
 from pydantic import BaseModel, Field, constr, validator
 from cashfree_lrs_client.models.purpose import Purpose
 
 class CreateRemitterRequest(BaseModel):
     """
     CreateRemitterRequest
     """
     remitter_id: constr(strict=True, max_length=50, min_length=1) = Field(..., description="Unique remitter ID to identify the remitter. Alphanumeric characters, hyphens, and underscores are allowed. Maximum of 50 characters are allowed.")
-    purpose: Purpose = ...
+    purpose: Purpose = Field(...)
     account_number: constr(strict=True, max_length=25, min_length=9) = Field(..., description="Bank account number of the remitter.")
     ifsc: constr(strict=True, max_length=11, min_length=8) = Field(..., description="The IFSC information of the remitter bank account. It should be an alphanumeric value of 11 characters. The first 4 characters should be alphabets, the 5th character should be a 0, and the remaining 6 characters should be numerals.")
     pan: constr(strict=True, max_length=10, min_length=10) = Field(..., description="PAN of the remitter. Should include 10 characters. The first 5 characters are alphabets followed by 4 numbers and the 10th character is an alphabet.")
     name: constr(strict=True, max_length=50, min_length=3) = Field(..., description="Name of the remitter. Alphabets and spaces are allowed.")
     address: constr(strict=True, max_length=200, min_length=3) = Field(..., description="Address of the remitter. Alphanumeric charcaters, dot, and hyphens are allowed.")
     city: constr(strict=True, max_length=50, min_length=3) = Field(..., description="City of the remitter. Alphabets are only allowed.")
     state: constr(strict=True, max_length=50, min_length=3) = Field(..., description="State of the remitter. Alphabets are only allowed.")
@@ -41,20 +40,22 @@
     phone_number: Optional[constr(strict=True, max_length=10, min_length=10)] = Field(None, description="Phone number of the remitter. Only numbers and hyphens are allowed.")
     email: Optional[constr(strict=True, max_length=50, min_length=5)] = Field(None, description="Email address of the remitter. Example, abc@gmail.com")
     nationality: constr(strict=True, max_length=2, min_length=2) = Field(..., description="Nationality of the remitter. Only 2 alphabets are allowed. Example, IN for India.")
     bank_code: constr(strict=True, max_length=4) = Field(..., description="Remitter bank code. Required for net banking payments to perform bank account checks (TPV). Maximum of 4 characters allowed.")
     __properties = ["remitter_id", "purpose", "account_number", "ifsc", "pan", "name", "address", "city", "state", "postal_code", "phone_number", "email", "nationality", "bank_code"]
 
     @validator('nationality')
-    def nationality_validate_enum(cls, v):
-        if v not in ('IN', 'US'):
+    def nationality_validate_enum(cls, value):
+        """Validates the enum"""
+        if value not in ('IN', 'US'):
             raise ValueError("must be one of enum values ('IN', 'US')")
-        return v
+        return value
 
     class Config:
+        """Pydantic configuration"""
         allow_population_by_field_name = True
         validate_assignment = True
 
     def to_str(self) -> str:
         """Returns the string representation of the model using alias"""
         return pprint.pformat(self.dict(by_alias=True))
 
@@ -77,15 +78,15 @@
 
     @classmethod
     def from_dict(cls, obj: dict) -> CreateRemitterRequest:
         """Create an instance of CreateRemitterRequest from a dict"""
         if obj is None:
             return None
 
-        if type(obj) is not dict:
+        if not isinstance(obj, dict):
             return CreateRemitterRequest.parse_obj(obj)
 
         _obj = CreateRemitterRequest.parse_obj({
             "remitter_id": obj.get("remitter_id"),
             "purpose": obj.get("purpose"),
             "account_number": obj.get("account_number"),
             "ifsc": obj.get("ifsc"),
```

### Comparing `cashfree_lrs_client-1.0.2/cashfree_lrs_client/models/currency.py` & `cashfree_lrs_client-1.0.3/cashfree_lrs_client/models/currency.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 # coding: utf-8
 
 """
     Cashfree LRS
 
     CashFree LRS APIs (v2)  # noqa: E501
 
-    The version of the OpenAPI document: 1.0.0
+    The version of the OpenAPI document: 1.0.3
     Contact: nextgenapi@cashfree.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
 
 
-from inspect import getfullargspec
+import json
 import pprint
 import re  # noqa: F401
 from aenum import Enum, no_arg
 
 
 
 
@@ -29,7 +29,13 @@
 
     """
     allowed enum values
     """
     USD = 'USD'
     INR = 'INR'
 
+    @classmethod
+    def from_json(cls, json_str: str) -> Currency:
+        """Create an instance of Currency from a JSON string"""
+        return Currency(json.loads(json_str))
+
+
```

### Comparing `cashfree_lrs_client-1.0.2/cashfree_lrs_client/models/error.py` & `cashfree_lrs_client-1.0.3/cashfree_lrs_client/models/error.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,42 +1,42 @@
 # coding: utf-8
 
 """
     Cashfree LRS
 
     CashFree LRS APIs (v2)  # noqa: E501
 
-    The version of the OpenAPI document: 1.0.0
+    The version of the OpenAPI document: 1.0.3
     Contact: nextgenapi@cashfree.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
 
 
 from __future__ import annotations
-from inspect import getfullargspec
 import pprint
 import re  # noqa: F401
 import json
 
 
 from typing import Optional
 from pydantic import BaseModel, StrictStr
 
 class Error(BaseModel):
     """
-    Error response
+    Common error response
     """
     message: Optional[StrictStr] = None
     code: Optional[StrictStr] = None
     type: Optional[StrictStr] = None
     __properties = ["message", "code", "type"]
 
     class Config:
+        """Pydantic configuration"""
         allow_population_by_field_name = True
         validate_assignment = True
 
     def to_str(self) -> str:
         """Returns the string representation of the model using alias"""
         return pprint.pformat(self.dict(by_alias=True))
 
@@ -49,25 +49,28 @@
         """Create an instance of Error from a JSON string"""
         return cls.from_dict(json.loads(json_str))
 
     def to_dict(self):
         """Returns the dictionary representation of the model using alias"""
         _dict = self.dict(by_alias=True,
                           exclude={
+                            "message",
+                            "code",
+                            "type",
                           },
                           exclude_none=True)
         return _dict
 
     @classmethod
     def from_dict(cls, obj: dict) -> Error:
         """Create an instance of Error from a dict"""
         if obj is None:
             return None
 
-        if type(obj) is not dict:
+        if not isinstance(obj, dict):
             return Error.parse_obj(obj)
 
         _obj = Error.parse_obj({
             "message": obj.get("message"),
             "code": obj.get("code"),
             "type": obj.get("type")
         })
```

### Comparing `cashfree_lrs_client-1.0.2/cashfree_lrs_client/models/fetch_forex_rate_request.py` & `cashfree_lrs_client-1.0.3/cashfree_lrs_client/models/fetch_forex_rate_request.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,47 +1,47 @@
 # coding: utf-8
 
 """
     Cashfree LRS
 
     CashFree LRS APIs (v2)  # noqa: E501
 
-    The version of the OpenAPI document: 1.0.0
+    The version of the OpenAPI document: 1.0.3
     Contact: nextgenapi@cashfree.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
 
 
 from __future__ import annotations
-from inspect import getfullargspec
 import pprint
 import re  # noqa: F401
 import json
 
 
-from typing import Optional
-from pydantic import BaseModel, Field, StrictBool, StrictFloat, constr
+from typing import Optional, Union
+from pydantic import BaseModel, Field, StrictBool, StrictFloat, StrictInt, constr
 from cashfree_lrs_client.models.currency import Currency
 from cashfree_lrs_client.models.purpose import Purpose
 
 class FetchForexRateRequest(BaseModel):
     """
     FetchForexRateRequest
     """
-    to_currency: Currency = ...
-    to_amount: StrictFloat = Field(..., description="Final settlement amount in to_currency (Double with 2 decimals are allowed.)")
-    purpose: Purpose = ...
+    to_currency: Currency = Field(...)
+    to_amount: Union[StrictFloat, StrictInt] = Field(..., description="Final settlement amount in to_currency (Double with 2 decimals are allowed.)")
+    purpose: Purpose = Field(...)
     remitter_id: Optional[constr(strict=True, max_length=50, min_length=3)] = Field(None, description="Unique remitter ID to identify the remitter. Alphanumeric characters, hyphens, and underscores are allowed. Maximum of 50 characters are allowed. If remitter ID is not specificed the tcs value calculated is zero.")
-    customer_declaration: Optional[StrictFloat] = Field(None, description="Amount in INR declared by Customer (Double with 2 decimals are allowed.)")
+    customer_declaration: Optional[Union[StrictFloat, StrictInt]] = Field(None, description="Amount in INR declared by Customer (Double with 2 decimals are allowed.)")
     education_loan: Optional[StrictBool] = Field(False, description="Whether user has availed an education loan")
     __properties = ["to_currency", "to_amount", "purpose", "remitter_id", "customer_declaration", "education_loan"]
 
     class Config:
+        """Pydantic configuration"""
         allow_population_by_field_name = True
         validate_assignment = True
 
     def to_str(self) -> str:
         """Returns the string representation of the model using alias"""
         return pprint.pformat(self.dict(by_alias=True))
 
@@ -64,15 +64,15 @@
 
     @classmethod
     def from_dict(cls, obj: dict) -> FetchForexRateRequest:
         """Create an instance of FetchForexRateRequest from a dict"""
         if obj is None:
             return None
 
-        if type(obj) is not dict:
+        if not isinstance(obj, dict):
             return FetchForexRateRequest.parse_obj(obj)
 
         _obj = FetchForexRateRequest.parse_obj({
             "to_currency": obj.get("to_currency"),
             "to_amount": obj.get("to_amount"),
             "purpose": obj.get("purpose"),
             "remitter_id": obj.get("remitter_id"),
```

### Comparing `cashfree_lrs_client-1.0.2/cashfree_lrs_client/models/order_response.py` & `cashfree_lrs_client-1.0.3/cashfree_lrs_client/models/create_order_response.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,82 +1,85 @@
 # coding: utf-8
 
 """
     Cashfree LRS
 
     CashFree LRS APIs (v2)  # noqa: E501
 
-    The version of the OpenAPI document: 1.0.0
+    The version of the OpenAPI document: 1.0.3
     Contact: nextgenapi@cashfree.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
 
 
 from __future__ import annotations
-from inspect import getfullargspec
 import pprint
 import re  # noqa: F401
 import json
 
 from datetime import datetime
-from typing import List, Optional
-from pydantic import BaseModel, StrictStr, confloat, conlist
+from typing import List, Optional, Union
+from pydantic import BaseModel, Field, StrictStr, confloat, conint, conlist
 
-class OrderResponse(BaseModel):
+class CreateOrderResponse(BaseModel):
     """
-    OrderResponse
+    CreateOrderResponse
     """
-    tcs: Optional[confloat(ge=0, strict=True)] = None
-    gst: Optional[confloat(ge=0, strict=True)] = None
-    fx_rate: Optional[confloat(ge=0, strict=True)] = None
-    amount_to_pay: Optional[confloat(ge=0, strict=True)] = None
-    handling_charges: Optional[confloat(ge=0, strict=True)] = None
+    tcs: Optional[conint(strict=True, ge=0)] = None
+    gst: Optional[Union[confloat(ge=0, strict=True), conint(ge=0, strict=True)]] = Field(None, description="Amount that can be either Int64, Float or Double")
+    fx_rate: Optional[Union[confloat(ge=0, strict=True), conint(ge=0, strict=True)]] = Field(None, description="Amount that can be either Int64, Float or Double")
+    amount_to_pay: Optional[Union[confloat(ge=0, strict=True), conint(ge=0, strict=True)]] = Field(None, description="Amount that can be either Int64, Float or Double")
+    handling_charges: Optional[conint(strict=True, ge=0)] = None
     order_expiry_time: Optional[datetime] = None
     payment_link: Optional[StrictStr] = None
     order_token: Optional[StrictStr] = None
     missing_documents: Optional[conlist(StrictStr)] = None
     __properties = ["tcs", "gst", "fx_rate", "amount_to_pay", "handling_charges", "order_expiry_time", "payment_link", "order_token", "missing_documents"]
 
     class Config:
+        """Pydantic configuration"""
         allow_population_by_field_name = True
         validate_assignment = True
 
     def to_str(self) -> str:
         """Returns the string representation of the model using alias"""
         return pprint.pformat(self.dict(by_alias=True))
 
     def to_json(self) -> str:
         """Returns the JSON representation of the model using alias"""
         return json.dumps(self.to_dict())
 
     @classmethod
-    def from_json(cls, json_str: str) -> OrderResponse:
-        """Create an instance of OrderResponse from a JSON string"""
+    def from_json(cls, json_str: str) -> CreateOrderResponse:
+        """Create an instance of CreateOrderResponse from a JSON string"""
         return cls.from_dict(json.loads(json_str))
 
     def to_dict(self):
         """Returns the dictionary representation of the model using alias"""
         _dict = self.dict(by_alias=True,
                           exclude={
+                            "order_expiry_time",
+                            "payment_link",
+                            "order_token",
                           },
                           exclude_none=True)
         return _dict
 
     @classmethod
-    def from_dict(cls, obj: dict) -> OrderResponse:
-        """Create an instance of OrderResponse from a dict"""
+    def from_dict(cls, obj: dict) -> CreateOrderResponse:
+        """Create an instance of CreateOrderResponse from a dict"""
         if obj is None:
             return None
 
-        if type(obj) is not dict:
-            return OrderResponse.parse_obj(obj)
+        if not isinstance(obj, dict):
+            return CreateOrderResponse.parse_obj(obj)
 
-        _obj = OrderResponse.parse_obj({
+        _obj = CreateOrderResponse.parse_obj({
             "tcs": obj.get("tcs"),
             "gst": obj.get("gst"),
             "fx_rate": obj.get("fx_rate"),
             "amount_to_pay": obj.get("amount_to_pay"),
             "handling_charges": obj.get("handling_charges"),
             "order_expiry_time": obj.get("order_expiry_time"),
             "payment_link": obj.get("payment_link"),
```

### Comparing `cashfree_lrs_client-1.0.2/cashfree_lrs_client/models/setup_webhooks200_response.py` & `cashfree_lrs_client-1.0.3/cashfree_lrs_client/models/setup_webhooks200_response.py`

 * *Files identical despite different names*

### Comparing `cashfree_lrs_client-1.0.2/cashfree_lrs_client/models/setup_webhooks_request.py` & `cashfree_lrs_client-1.0.3/cashfree_lrs_client/models/setup_webhooks_request.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,24 +1,23 @@
 # coding: utf-8
 
 """
     Cashfree LRS
 
     CashFree LRS APIs (v2)  # noqa: E501
 
-    The version of the OpenAPI document: 1.0.0
+    The version of the OpenAPI document: 1.0.3
     Contact: nextgenapi@cashfree.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
 
 
 from __future__ import annotations
-from inspect import getfullargspec
 import pprint
 import re  # noqa: F401
 import json
 
 
 
 from pydantic import BaseModel, Field, StrictStr
@@ -29,14 +28,15 @@
     """
     payment_url: StrictStr = Field(..., description="Specify the URL where you want to receive information about payments.")
     refund_url: StrictStr = Field(..., description="Specify the URL where you want to receive information about refunds.")
     order_url: StrictStr = Field(..., description="Specify the URL where you want to receive information about orders.")
     __properties = ["payment_url", "refund_url", "order_url"]
 
     class Config:
+        """Pydantic configuration"""
         allow_population_by_field_name = True
         validate_assignment = True
 
     def to_str(self) -> str:
         """Returns the string representation of the model using alias"""
         return pprint.pformat(self.dict(by_alias=True))
 
@@ -59,15 +59,15 @@
 
     @classmethod
     def from_dict(cls, obj: dict) -> SetupWebhooksRequest:
         """Create an instance of SetupWebhooksRequest from a dict"""
         if obj is None:
             return None
 
-        if type(obj) is not dict:
+        if not isinstance(obj, dict):
             return SetupWebhooksRequest.parse_obj(obj)
 
         _obj = SetupWebhooksRequest.parse_obj({
             "payment_url": obj.get("payment_url"),
             "refund_url": obj.get("refund_url"),
             "order_url": obj.get("order_url")
         })
```

### Comparing `cashfree_lrs_client-1.0.2/cashfree_lrs_client/models/success_message.py` & `cashfree_lrs_client-1.0.3/cashfree_lrs_client/models/success_message.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,40 +1,40 @@
 # coding: utf-8
 
 """
     Cashfree LRS
 
     CashFree LRS APIs (v2)  # noqa: E501
 
-    The version of the OpenAPI document: 1.0.0
+    The version of the OpenAPI document: 1.0.3
     Contact: nextgenapi@cashfree.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
 
 
 from __future__ import annotations
-from inspect import getfullargspec
 import pprint
 import re  # noqa: F401
 import json
 
 
 from typing import Optional
 from pydantic import BaseModel, StrictStr
 
 class SuccessMessage(BaseModel):
     """
-    SuccessMessage
+    Success message for when API is processed successfully
     """
     message: Optional[StrictStr] = None
     __properties = ["message"]
 
     class Config:
+        """Pydantic configuration"""
         allow_population_by_field_name = True
         validate_assignment = True
 
     def to_str(self) -> str:
         """Returns the string representation of the model using alias"""
         return pprint.pformat(self.dict(by_alias=True))
 
@@ -57,15 +57,15 @@
 
     @classmethod
     def from_dict(cls, obj: dict) -> SuccessMessage:
         """Create an instance of SuccessMessage from a dict"""
         if obj is None:
             return None
 
-        if type(obj) is not dict:
+        if not isinstance(obj, dict):
             return SuccessMessage.parse_obj(obj)
 
         _obj = SuccessMessage.parse_obj({
             "message": obj.get("message")
         })
         return _obj
```

### Comparing `cashfree_lrs_client-1.0.2/cashfree_lrs_client/paths/__init__.py` & `cashfree_lrs_client-1.0.3/cashfree_lrs_client/paths/__init__.py`

 * *Files identical despite different names*

### Comparing `cashfree_lrs_client-1.0.2/cashfree_lrs_client/paths/beneficiaries/post.py` & `cashfree_lrs_client-1.0.3/cashfree_lrs_client/paths/beneficiaries/post.py`

 * *Files identical despite different names*

### Comparing `cashfree_lrs_client-1.0.2/cashfree_lrs_client/paths/beneficiaries/post.pyi` & `cashfree_lrs_client-1.0.3/cashfree_lrs_client/paths/beneficiaries/post.pyi`

 * *Files identical despite different names*

### Comparing `cashfree_lrs_client-1.0.2/cashfree_lrs_client/paths/fx_rate_details/post.py` & `cashfree_lrs_client-1.0.3/cashfree_lrs_client/paths/fx_rate_details/post.py`

 * *Files identical despite different names*

### Comparing `cashfree_lrs_client-1.0.2/cashfree_lrs_client/paths/fx_rate_details/post.pyi` & `cashfree_lrs_client-1.0.3/cashfree_lrs_client/paths/fx_rate_details/post.pyi`

 * *Files identical despite different names*

### Comparing `cashfree_lrs_client-1.0.2/cashfree_lrs_client/paths/orders/post.py` & `cashfree_lrs_client-1.0.3/cashfree_lrs_client/paths/orders/post.py`

 * *Files identical despite different names*

### Comparing `cashfree_lrs_client-1.0.2/cashfree_lrs_client/paths/orders/post.pyi` & `cashfree_lrs_client-1.0.3/cashfree_lrs_client/paths/orders/post.pyi`

 * *Files identical despite different names*

### Comparing `cashfree_lrs_client-1.0.2/cashfree_lrs_client/paths/orders_documents_upload/post.py` & `cashfree_lrs_client-1.0.3/cashfree_lrs_client/paths/orders_documents_upload/post.py`

 * *Files identical despite different names*

### Comparing `cashfree_lrs_client-1.0.2/cashfree_lrs_client/paths/orders_documents_upload/post.pyi` & `cashfree_lrs_client-1.0.3/cashfree_lrs_client/paths/orders_documents_upload/post.pyi`

 * *Files identical despite different names*

### Comparing `cashfree_lrs_client-1.0.2/cashfree_lrs_client/paths/orders_order_id_documents_upload/post.py` & `cashfree_lrs_client-1.0.3/cashfree_lrs_client/paths/orders_order_id_documents_upload/post.py`

 * *Files identical despite different names*

### Comparing `cashfree_lrs_client-1.0.2/cashfree_lrs_client/paths/orders_order_id_documents_upload/post.pyi` & `cashfree_lrs_client-1.0.3/cashfree_lrs_client/paths/orders_order_id_documents_upload/post.pyi`

 * *Files identical despite different names*

### Comparing `cashfree_lrs_client-1.0.2/cashfree_lrs_client/paths/orders_order_id_process/post.py` & `cashfree_lrs_client-1.0.3/cashfree_lrs_client/paths/orders_order_id_process/post.py`

 * *Files identical despite different names*

### Comparing `cashfree_lrs_client-1.0.2/cashfree_lrs_client/paths/orders_order_id_process/post.pyi` & `cashfree_lrs_client-1.0.3/cashfree_lrs_client/paths/orders_order_id_process/post.pyi`

 * *Files identical despite different names*

### Comparing `cashfree_lrs_client-1.0.2/cashfree_lrs_client/paths/remitters/post.py` & `cashfree_lrs_client-1.0.3/cashfree_lrs_client/paths/remitters/post.py`

 * *Files identical despite different names*

### Comparing `cashfree_lrs_client-1.0.2/cashfree_lrs_client/paths/remitters/post.pyi` & `cashfree_lrs_client-1.0.3/cashfree_lrs_client/paths/remitters/post.pyi`

 * *Files identical despite different names*

### Comparing `cashfree_lrs_client-1.0.2/cashfree_lrs_client/paths/webhooks/post.py` & `cashfree_lrs_client-1.0.3/cashfree_lrs_client/paths/webhooks/post.py`

 * *Files identical despite different names*

### Comparing `cashfree_lrs_client-1.0.2/cashfree_lrs_client/paths/webhooks/post.pyi` & `cashfree_lrs_client-1.0.3/cashfree_lrs_client/paths/webhooks/post.pyi`

 * *Files identical despite different names*

### Comparing `cashfree_lrs_client-1.0.2/cashfree_lrs_client/schemas.py` & `cashfree_lrs_client-1.0.3/cashfree_lrs_client/schemas.py`

 * *Files identical despite different names*

### Comparing `cashfree_lrs_client-1.0.2/cashfree_lrs_client/test/test_create_beneficiary_request.py` & `cashfree_lrs_client-1.0.3/cashfree_lrs_client/test/test_create_beneficiary_request.py`

 * *Files identical despite different names*

### Comparing `cashfree_lrs_client-1.0.2/cashfree_lrs_client/test/test_create_order_request.py` & `cashfree_lrs_client-1.0.3/cashfree_lrs_client/test/test_create_order_request.py`

 * *Files identical despite different names*

### Comparing `cashfree_lrs_client-1.0.2/cashfree_lrs_client/test/test_create_order_response.py` & `cashfree_lrs_client-1.0.3/cashfree_lrs_client/test/test_create_order_response.py`

 * *Files identical despite different names*

### Comparing `cashfree_lrs_client-1.0.2/cashfree_lrs_client/test/test_create_remitter_request.py` & `cashfree_lrs_client-1.0.3/cashfree_lrs_client/test/test_create_remitter_request.py`

 * *Files identical despite different names*

### Comparing `cashfree_lrs_client-1.0.2/cashfree_lrs_client/test/test_currency.py` & `cashfree_lrs_client-1.0.3/cashfree_lrs_client/test/test_currency.py`

 * *Files identical despite different names*

### Comparing `cashfree_lrs_client-1.0.2/cashfree_lrs_client/test/test_error.py` & `cashfree_lrs_client-1.0.3/cashfree_lrs_client/test/test_error.py`

 * *Files identical despite different names*

### Comparing `cashfree_lrs_client-1.0.2/cashfree_lrs_client/test/test_fetch_forex_rate_request.py` & `cashfree_lrs_client-1.0.3/cashfree_lrs_client/test/test_fetch_forex_rate_request.py`

 * *Files identical despite different names*

### Comparing `cashfree_lrs_client-1.0.2/cashfree_lrs_client/test/test_lrs_api.py` & `cashfree_lrs_client-1.0.3/cashfree_lrs_client/test/test_lrs_api.py`

 * *Files identical despite different names*

### Comparing `cashfree_lrs_client-1.0.2/cashfree_lrs_client/test/test_purpose.py` & `cashfree_lrs_client-1.0.3/cashfree_lrs_client/test/test_purpose.py`

 * *Files identical despite different names*

### Comparing `cashfree_lrs_client-1.0.2/cashfree_lrs_client/test/test_setup_webhooks_request.py` & `cashfree_lrs_client-1.0.3/cashfree_lrs_client/test/test_setup_webhooks_request.py`

 * *Files identical despite different names*

### Comparing `cashfree_lrs_client-1.0.2/cashfree_lrs_client/test/test_success_message.py` & `cashfree_lrs_client-1.0.3/cashfree_lrs_client/test/test_success_message.py`

 * *Files identical despite different names*

