# Comparing `tmp/cashfree_lrs_client-1.0.1.tar.gz` & `tmp/cashfree_lrs_client-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cashfree_lrs_client-1.0.1.tar", max compression
+gzip compressed data, was "cashfree_lrs_client-1.0.2.tar", max compression
```

## Comparing `cashfree_lrs_client-1.0.1.tar` & `cashfree_lrs_client-1.0.2.tar`

### file list

```diff
@@ -1,110 +1,112 @@
--rw-r--r--   0        0        0    12463 2023-04-28 19:23:15.998821 cashfree_lrs_client-1.0.1/README.md
--rw-r--r--   0        0        0      780 2023-04-28 19:23:16.022822 cashfree_lrs_client-1.0.1/cashfree_lrs_client/__init__.py
--rw-r--r--   0        0        0       99 2023-04-28 19:22:51.482474 cashfree_lrs_client-1.0.1/cashfree_lrs_client/api/__init__.py
--rw-r--r--   0        0        0    53538 2023-04-28 19:22:51.482474 cashfree_lrs_client-1.0.1/cashfree_lrs_client/api/default_api.py
--rw-r--r--   0        0        0    53218 2023-04-28 19:22:51.482474 cashfree_lrs_client-1.0.1/cashfree_lrs_client/api/lrs_api.py
--rw-r--r--   0        0        0    58509 2023-04-28 19:23:16.070822 cashfree_lrs_client-1.0.1/cashfree_lrs_client/api_client.py
--rw-r--r--   0        0        0      214 2023-04-28 19:23:16.114823 cashfree_lrs_client-1.0.1/cashfree_lrs_client/apis/__init__.py
--rw-r--r--   0        0        0     1655 2023-04-28 19:23:15.818819 cashfree_lrs_client-1.0.1/cashfree_lrs_client/apis/path_to_api.py
--rw-r--r--   0        0        0      246 2023-04-28 19:23:15.818819 cashfree_lrs_client-1.0.1/cashfree_lrs_client/apis/paths/__init__.py
--rw-r--r--   0        0        0      119 2023-04-28 19:23:15.838819 cashfree_lrs_client-1.0.1/cashfree_lrs_client/apis/paths/beneficiaries.py
--rw-r--r--   0        0        0      121 2023-04-28 19:23:15.822819 cashfree_lrs_client-1.0.1/cashfree_lrs_client/apis/paths/fx_rate_details.py
--rw-r--r--   0        0        0      105 2023-04-28 19:23:15.830819 cashfree_lrs_client-1.0.1/cashfree_lrs_client/apis/paths/orders.py
--rw-r--r--   0        0        0      137 2023-04-28 19:23:15.826819 cashfree_lrs_client-1.0.1/cashfree_lrs_client/apis/paths/orders_documents_upload.py
--rw-r--r--   0        0        0      153 2023-04-28 19:23:15.834819 cashfree_lrs_client-1.0.1/cashfree_lrs_client/apis/paths/orders_order_id_documents_upload.py
--rw-r--r--   0        0        0      136 2023-04-28 19:23:15.822819 cashfree_lrs_client-1.0.1/cashfree_lrs_client/apis/paths/orders_order_id_process.py
--rw-r--r--   0        0        0      111 2023-04-28 19:23:15.830819 cashfree_lrs_client-1.0.1/cashfree_lrs_client/apis/paths/remitters.py
--rw-r--r--   0        0        0      109 2023-04-28 19:23:15.826819 cashfree_lrs_client-1.0.1/cashfree_lrs_client/apis/paths/webhooks.py
--rw-r--r--   0        0        0      306 2023-04-28 19:23:15.818819 cashfree_lrs_client-1.0.1/cashfree_lrs_client/apis/tag_to_api.py
--rw-r--r--   0        0        0      308 2023-04-28 19:23:15.818819 cashfree_lrs_client-1.0.1/cashfree_lrs_client/apis/tags/__init__.py
--rw-r--r--   0        0        0     1162 2023-04-28 19:23:15.878820 cashfree_lrs_client-1.0.1/cashfree_lrs_client/apis/tags/lrs_api.py
--rw-r--r--   0        0        0    17326 2023-04-28 19:23:16.018822 cashfree_lrs_client-1.0.1/cashfree_lrs_client/configuration.py
--rw-r--r--   0        0        0     2815 2023-04-28 19:22:51.482474 cashfree_lrs_client-1.0.1/cashfree_lrs_client/docs/CreateBeneficiaryRequest.md
--rw-r--r--   0        0        0     2331 2023-04-28 19:22:51.486474 cashfree_lrs_client-1.0.1/cashfree_lrs_client/docs/CreateOrderRequest.md
--rw-r--r--   0        0        0     1337 2023-04-28 19:22:51.486474 cashfree_lrs_client-1.0.1/cashfree_lrs_client/docs/CreateOrderResponse.md
--rw-r--r--   0        0        0     2583 2023-04-28 19:22:51.486474 cashfree_lrs_client-1.0.1/cashfree_lrs_client/docs/CreateRemitterRequest.md
--rw-r--r--   0        0        0      389 2023-04-28 19:22:51.486474 cashfree_lrs_client-1.0.1/cashfree_lrs_client/docs/Currency.md
--rw-r--r--   0        0        0      859 2023-04-28 19:22:51.486474 cashfree_lrs_client-1.0.1/cashfree_lrs_client/docs/Error.md
--rw-r--r--   0        0        0     1656 2023-04-28 19:22:51.486474 cashfree_lrs_client-1.0.1/cashfree_lrs_client/docs/FetchForexRateRequest.md
--rw-r--r--   0        0        0    59748 2023-04-28 19:22:51.486474 cashfree_lrs_client-1.0.1/cashfree_lrs_client/docs/LrsApi.md
--rw-r--r--   0        0        0      343 2023-04-28 19:22:51.486474 cashfree_lrs_client-1.0.1/cashfree_lrs_client/docs/Purpose.md
--rw-r--r--   0        0        0     1239 2023-04-28 19:22:51.486474 cashfree_lrs_client-1.0.1/cashfree_lrs_client/docs/SetupWebhooksRequest.md
--rw-r--r--   0        0        0      896 2023-04-28 19:22:51.486474 cashfree_lrs_client-1.0.1/cashfree_lrs_client/docs/SuccessMessage.md
--rw-r--r--   0        0        0     4503 2023-04-28 19:23:16.022822 cashfree_lrs_client-1.0.1/cashfree_lrs_client/exceptions.py
--rw-r--r--   0        0        0      353 2023-04-28 19:23:16.114823 cashfree_lrs_client-1.0.1/cashfree_lrs_client/model/__init__.py
--rw-r--r--   0        0        0    14903 2023-04-28 19:23:10.962750 cashfree_lrs_client-1.0.1/cashfree_lrs_client/model/create_beneficiary_request.py
--rw-r--r--   0        0        0    13066 2023-04-28 19:23:11.554758 cashfree_lrs_client-1.0.1/cashfree_lrs_client/model/create_beneficiary_request.pyi
--rw-r--r--   0        0        0    11475 2023-04-28 19:23:12.030765 cashfree_lrs_client-1.0.1/cashfree_lrs_client/model/create_order_request.py
--rw-r--r--   0        0        0    10572 2023-04-28 19:23:12.246768 cashfree_lrs_client-1.0.1/cashfree_lrs_client/model/create_order_request.pyi
--rw-r--r--   0        0        0     9010 2023-04-28 19:23:12.606773 cashfree_lrs_client-1.0.1/cashfree_lrs_client/model/create_order_response.py
--rw-r--r--   0        0        0     8425 2023-04-28 19:23:12.794776 cashfree_lrs_client-1.0.1/cashfree_lrs_client/model/create_order_response.pyi
--rw-r--r--   0        0        0    12349 2023-04-28 19:23:13.218782 cashfree_lrs_client-1.0.1/cashfree_lrs_client/model/create_remitter_request.py
--rw-r--r--   0        0        0    10785 2023-04-28 19:23:13.370784 cashfree_lrs_client-1.0.1/cashfree_lrs_client/model/create_remitter_request.pyi
--rw-r--r--   0        0        0     1146 2023-04-28 19:23:13.454785 cashfree_lrs_client-1.0.1/cashfree_lrs_client/model/currency.py
--rw-r--r--   0        0        0     1031 2023-04-28 19:23:13.466786 cashfree_lrs_client-1.0.1/cashfree_lrs_client/model/currency.pyi
--rw-r--r--   0        0        0     3377 2023-04-28 19:23:13.518786 cashfree_lrs_client-1.0.1/cashfree_lrs_client/model/error.py
--rw-r--r--   0        0        0     3377 2023-04-28 19:23:13.566787 cashfree_lrs_client-1.0.1/cashfree_lrs_client/model/error.pyi
--rw-r--r--   0        0        0     5194 2023-04-28 19:23:13.626788 cashfree_lrs_client-1.0.1/cashfree_lrs_client/model/fetch_forex_rate_request.py
--rw-r--r--   0        0        0     5086 2023-04-28 19:23:13.662788 cashfree_lrs_client-1.0.1/cashfree_lrs_client/model/fetch_forex_rate_request.pyi
--rw-r--r--   0        0        0     1368 2023-04-28 19:23:13.702789 cashfree_lrs_client-1.0.1/cashfree_lrs_client/model/purpose.py
--rw-r--r--   0        0        0     1169 2023-04-28 19:23:13.710789 cashfree_lrs_client-1.0.1/cashfree_lrs_client/model/purpose.pyi
--rw-r--r--   0        0        0     3663 2023-04-28 19:23:13.766790 cashfree_lrs_client-1.0.1/cashfree_lrs_client/model/setup_webhooks_request.py
--rw-r--r--   0        0        0     3663 2023-04-28 19:23:13.798790 cashfree_lrs_client-1.0.1/cashfree_lrs_client/model/setup_webhooks_request.pyi
--rw-r--r--   0        0        0     2417 2023-04-28 19:23:13.846791 cashfree_lrs_client-1.0.1/cashfree_lrs_client/model/success_message.py
--rw-r--r--   0        0        0     2417 2023-04-28 19:23:13.866791 cashfree_lrs_client-1.0.1/cashfree_lrs_client/model/success_message.pyi
--rw-r--r--   0        0        0     1121 2023-04-28 19:23:16.114823 cashfree_lrs_client-1.0.1/cashfree_lrs_client/models/__init__.py
--rw-r--r--   0        0        0     1975 2023-04-28 19:22:51.486474 cashfree_lrs_client-1.0.1/cashfree_lrs_client/models/create_beneficiary200_response.py
--rw-r--r--   0        0        0     5826 2023-04-28 19:22:51.486474 cashfree_lrs_client-1.0.1/cashfree_lrs_client/models/create_beneficiary_request.py
--rw-r--r--   0        0        0     4904 2023-04-28 19:22:51.486474 cashfree_lrs_client-1.0.1/cashfree_lrs_client/models/create_order_request.py
--rw-r--r--   0        0        0     2951 2023-04-28 19:22:51.486474 cashfree_lrs_client-1.0.1/cashfree_lrs_client/models/create_order_response.py
--rw-r--r--   0        0        0     1951 2023-04-28 19:22:51.486474 cashfree_lrs_client-1.0.1/cashfree_lrs_client/models/create_remitter200_response.py
--rw-r--r--   0        0        0     5289 2023-04-28 19:22:51.486474 cashfree_lrs_client-1.0.1/cashfree_lrs_client/models/create_remitter_request.py
--rw-r--r--   0        0        0      608 2023-04-28 19:22:51.486474 cashfree_lrs_client-1.0.1/cashfree_lrs_client/models/currency.py
--rw-r--r--   0        0        0     1964 2023-04-28 19:22:51.486474 cashfree_lrs_client-1.0.1/cashfree_lrs_client/models/error.py
--rw-r--r--   0        0        0     3205 2023-04-28 19:22:51.486474 cashfree_lrs_client-1.0.1/cashfree_lrs_client/models/fetch_forex_rate_request.py
--rw-r--r--   0        0        0     2903 2023-04-28 19:22:51.486474 cashfree_lrs_client-1.0.1/cashfree_lrs_client/models/order_response.py
--rw-r--r--   0        0        0      626 2023-04-28 19:22:51.486474 cashfree_lrs_client-1.0.1/cashfree_lrs_client/models/purpose.py
--rw-r--r--   0        0        0     1943 2023-04-28 19:22:51.486474 cashfree_lrs_client-1.0.1/cashfree_lrs_client/models/setup_webhooks200_response.py
--rw-r--r--   0        0        0     2355 2023-04-28 19:22:51.486474 cashfree_lrs_client-1.0.1/cashfree_lrs_client/models/setup_webhooks_request.py
--rw-r--r--   0        0        0     1863 2023-04-28 19:22:51.486474 cashfree_lrs_client-1.0.1/cashfree_lrs_client/models/success_message.py
--rw-r--r--   0        0        0      644 2023-04-28 19:23:15.810819 cashfree_lrs_client-1.0.1/cashfree_lrs_client/paths/__init__.py
--rw-r--r--   0        0        0      323 2023-04-28 19:23:15.814819 cashfree_lrs_client-1.0.1/cashfree_lrs_client/paths/beneficiaries/__init__.py
--rw-r--r--   0        0        0    12582 2023-04-28 19:23:14.366798 cashfree_lrs_client-1.0.1/cashfree_lrs_client/paths/beneficiaries/post.py
--rw-r--r--   0        0        0    12396 2023-04-28 19:23:14.482800 cashfree_lrs_client-1.0.1/cashfree_lrs_client/paths/beneficiaries/post.pyi
--rw-r--r--   0        0        0      326 2023-04-28 19:23:15.810819 cashfree_lrs_client-1.0.1/cashfree_lrs_client/paths/fx_rate_details/__init__.py
--rw-r--r--   0        0        0    11760 2023-04-28 19:23:15.062808 cashfree_lrs_client-1.0.1/cashfree_lrs_client/paths/fx_rate_details/post.py
--rw-r--r--   0        0        0    11604 2023-04-28 19:23:15.170810 cashfree_lrs_client-1.0.1/cashfree_lrs_client/paths/fx_rate_details/post.pyi
--rw-r--r--   0        0        0      309 2023-04-28 19:23:15.814819 cashfree_lrs_client-1.0.1/cashfree_lrs_client/paths/orders/__init__.py
--rw-r--r--   0        0        0    13005 2023-04-28 19:23:14.606802 cashfree_lrs_client-1.0.1/cashfree_lrs_client/paths/orders/post.py
--rw-r--r--   0        0        0    12789 2023-04-28 19:23:14.726803 cashfree_lrs_client-1.0.1/cashfree_lrs_client/paths/orders/post.pyi
--rw-r--r--   0        0        0      343 2023-04-28 19:23:15.810819 cashfree_lrs_client-1.0.1/cashfree_lrs_client/paths/orders_documents_upload/__init__.py
--rw-r--r--   0        0        0    12334 2023-04-28 19:23:14.126795 cashfree_lrs_client-1.0.1/cashfree_lrs_client/paths/orders_documents_upload/post.py
--rw-r--r--   0        0        0    12148 2023-04-28 19:23:14.242797 cashfree_lrs_client-1.0.1/cashfree_lrs_client/paths/orders_documents_upload/post.pyi
--rw-r--r--   0        0        0      361 2023-04-28 19:23:15.814819 cashfree_lrs_client-1.0.1/cashfree_lrs_client/paths/orders_order_id_documents_upload/__init__.py
--rw-r--r--   0        0        0    15715 2023-04-28 19:23:15.674817 cashfree_lrs_client-1.0.1/cashfree_lrs_client/paths/orders_order_id_documents_upload/post.py
--rw-r--r--   0        0        0    15469 2023-04-28 19:23:15.806819 cashfree_lrs_client-1.0.1/cashfree_lrs_client/paths/orders_order_id_documents_upload/post.pyi
--rw-r--r--   0        0        0      343 2023-04-28 19:23:15.810819 cashfree_lrs_client-1.0.1/cashfree_lrs_client/paths/orders_order_id_process/__init__.py
--rw-r--r--   0        0        0     8093 2023-04-28 19:23:15.250811 cashfree_lrs_client-1.0.1/cashfree_lrs_client/paths/orders_order_id_process/post.py
--rw-r--r--   0        0        0     7937 2023-04-28 19:23:15.326812 cashfree_lrs_client-1.0.1/cashfree_lrs_client/paths/orders_order_id_process/post.pyi
--rw-r--r--   0        0        0      315 2023-04-28 19:23:15.814819 cashfree_lrs_client-1.0.1/cashfree_lrs_client/paths/remitters/__init__.py
--rw-r--r--   0        0        0    12525 2023-04-28 19:23:14.846805 cashfree_lrs_client-1.0.1/cashfree_lrs_client/paths/remitters/post.py
--rw-r--r--   0        0        0    12339 2023-04-28 19:23:14.958807 cashfree_lrs_client-1.0.1/cashfree_lrs_client/paths/remitters/post.pyi
--rw-r--r--   0        0        0      313 2023-04-28 19:23:15.810819 cashfree_lrs_client-1.0.1/cashfree_lrs_client/paths/webhooks/__init__.py
--rw-r--r--   0        0        0    11939 2023-04-28 19:23:15.438813 cashfree_lrs_client-1.0.1/cashfree_lrs_client/paths/webhooks/post.py
--rw-r--r--   0        0        0    11783 2023-04-28 19:23:15.546815 cashfree_lrs_client-1.0.1/cashfree_lrs_client/paths/webhooks/post.pyi
--rw-r--r--   0        0        0    10536 2023-04-28 19:23:16.074822 cashfree_lrs_client-1.0.1/cashfree_lrs_client/rest.py
--rw-r--r--   0        0        0    97649 2023-04-28 19:23:16.110823 cashfree_lrs_client-1.0.1/cashfree_lrs_client/schemas.py
--rw-r--r--   0        0        0        0 2023-04-28 19:22:51.486474 cashfree_lrs_client-1.0.1/cashfree_lrs_client/test/__init__.py
--rw-r--r--   0        0        0     2694 2023-04-28 19:22:51.486474 cashfree_lrs_client-1.0.1/cashfree_lrs_client/test/test_create_beneficiary_request.py
--rw-r--r--   0        0        0     2292 2023-04-28 19:22:51.486474 cashfree_lrs_client-1.0.1/cashfree_lrs_client/test/test_create_order_request.py
--rw-r--r--   0        0        0     1952 2023-04-28 19:22:51.486474 cashfree_lrs_client-1.0.1/cashfree_lrs_client/test/test_create_order_response.py
--rw-r--r--   0        0        0     2486 2023-04-28 19:22:51.486474 cashfree_lrs_client-1.0.1/cashfree_lrs_client/test/test_create_remitter_request.py
--rw-r--r--   0        0        0      738 2023-04-28 19:22:51.486474 cashfree_lrs_client-1.0.1/cashfree_lrs_client/test/test_currency.py
--rw-r--r--   0        0        0     1439 2023-04-28 19:22:51.486474 cashfree_lrs_client-1.0.1/cashfree_lrs_client/test/test_error.py
--rw-r--r--   0        0        0     1860 2023-04-28 19:22:51.486474 cashfree_lrs_client-1.0.1/cashfree_lrs_client/test/test_fetch_forex_rate_request.py
--rw-r--r--   0        0        0     1845 2023-04-28 19:22:51.486474 cashfree_lrs_client-1.0.1/cashfree_lrs_client/test/test_lrs_api.py
--rw-r--r--   0        0        0      731 2023-04-28 19:22:51.486474 cashfree_lrs_client-1.0.1/cashfree_lrs_client/test/test_purpose.py
--rw-r--r--   0        0        0     1737 2023-04-28 19:22:51.486474 cashfree_lrs_client-1.0.1/cashfree_lrs_client/test/test_setup_webhooks_request.py
--rw-r--r--   0        0        0     1493 2023-04-28 19:22:51.490475 cashfree_lrs_client-1.0.1/cashfree_lrs_client/test/test_success_message.py
--rw-r--r--   0        0        0      698 2023-04-28 19:23:01.382615 cashfree_lrs_client-1.0.1/pyproject.toml
--rw-r--r--   0        0        0    13260 1970-01-01 00:00:00.000000 cashfree_lrs_client-1.0.1/PKG-INFO
+-rw-r--r--   0        0        0    12498 2023-05-01 07:34:04.939553 cashfree_lrs_client-1.0.2/README.md
+-rw-r--r--   0        0        0      780 2023-05-01 07:34:04.959553 cashfree_lrs_client-1.0.2/cashfree_lrs_client/__init__.py
+-rw-r--r--   0        0        0       99 2023-05-01 07:33:35.523573 cashfree_lrs_client-1.0.2/cashfree_lrs_client/api/__init__.py
+-rw-r--r--   0        0        0    53538 2023-05-01 07:33:35.527573 cashfree_lrs_client-1.0.2/cashfree_lrs_client/api/default_api.py
+-rw-r--r--   0        0        0    53218 2023-05-01 07:33:35.527573 cashfree_lrs_client-1.0.2/cashfree_lrs_client/api/lrs_api.py
+-rw-r--r--   0        0        0    58509 2023-05-01 07:34:04.991553 cashfree_lrs_client-1.0.2/cashfree_lrs_client/api_client.py
+-rw-r--r--   0        0        0      214 2023-05-01 07:34:05.015553 cashfree_lrs_client-1.0.2/cashfree_lrs_client/apis/__init__.py
+-rw-r--r--   0        0        0     1655 2023-05-01 07:34:04.767553 cashfree_lrs_client-1.0.2/cashfree_lrs_client/apis/path_to_api.py
+-rw-r--r--   0        0        0      246 2023-05-01 07:34:04.767553 cashfree_lrs_client-1.0.2/cashfree_lrs_client/apis/paths/__init__.py
+-rw-r--r--   0        0        0      119 2023-05-01 07:34:04.783553 cashfree_lrs_client-1.0.2/cashfree_lrs_client/apis/paths/beneficiaries.py
+-rw-r--r--   0        0        0      121 2023-05-01 07:34:04.771553 cashfree_lrs_client-1.0.2/cashfree_lrs_client/apis/paths/fx_rate_details.py
+-rw-r--r--   0        0        0      105 2023-05-01 07:34:04.779553 cashfree_lrs_client-1.0.2/cashfree_lrs_client/apis/paths/orders.py
+-rw-r--r--   0        0        0      137 2023-05-01 07:34:04.775553 cashfree_lrs_client-1.0.2/cashfree_lrs_client/apis/paths/orders_documents_upload.py
+-rw-r--r--   0        0        0      153 2023-05-01 07:34:04.783553 cashfree_lrs_client-1.0.2/cashfree_lrs_client/apis/paths/orders_order_id_documents_upload.py
+-rw-r--r--   0        0        0      136 2023-05-01 07:34:04.771553 cashfree_lrs_client-1.0.2/cashfree_lrs_client/apis/paths/orders_order_id_process.py
+-rw-r--r--   0        0        0      111 2023-05-01 07:34:04.779553 cashfree_lrs_client-1.0.2/cashfree_lrs_client/apis/paths/remitters.py
+-rw-r--r--   0        0        0      109 2023-05-01 07:34:04.775553 cashfree_lrs_client-1.0.2/cashfree_lrs_client/apis/paths/webhooks.py
+-rw-r--r--   0        0        0      306 2023-05-01 07:34:04.763553 cashfree_lrs_client-1.0.2/cashfree_lrs_client/apis/tag_to_api.py
+-rw-r--r--   0        0        0      308 2023-05-01 07:34:04.767553 cashfree_lrs_client-1.0.2/cashfree_lrs_client/apis/tags/__init__.py
+-rw-r--r--   0        0        0     1162 2023-05-01 07:34:04.823553 cashfree_lrs_client-1.0.2/cashfree_lrs_client/apis/tags/lrs_api.py
+-rw-r--r--   0        0        0    17326 2023-05-01 07:34:04.959553 cashfree_lrs_client-1.0.2/cashfree_lrs_client/configuration.py
+-rw-r--r--   0        0        0     2815 2023-05-01 07:33:35.527573 cashfree_lrs_client-1.0.2/cashfree_lrs_client/docs/CreateBeneficiaryRequest.md
+-rw-r--r--   0        0        0     2331 2023-05-01 07:33:35.527573 cashfree_lrs_client-1.0.2/cashfree_lrs_client/docs/CreateOrderRequest.md
+-rw-r--r--   0        0        0     1337 2023-05-01 07:33:35.527573 cashfree_lrs_client-1.0.2/cashfree_lrs_client/docs/CreateOrderResponse.md
+-rw-r--r--   0        0        0     2583 2023-05-01 07:33:35.527573 cashfree_lrs_client-1.0.2/cashfree_lrs_client/docs/CreateRemitterRequest.md
+-rw-r--r--   0        0        0      389 2023-05-01 07:33:35.527573 cashfree_lrs_client-1.0.2/cashfree_lrs_client/docs/Currency.md
+-rw-r--r--   0        0        0      859 2023-05-01 07:33:35.527573 cashfree_lrs_client-1.0.2/cashfree_lrs_client/docs/Error.md
+-rw-r--r--   0        0        0     1656 2023-05-01 07:33:35.527573 cashfree_lrs_client-1.0.2/cashfree_lrs_client/docs/FetchForexRateRequest.md
+-rw-r--r--   0        0        0    59748 2023-05-01 07:33:35.527573 cashfree_lrs_client-1.0.2/cashfree_lrs_client/docs/LrsApi.md
+-rw-r--r--   0        0        0      343 2023-05-01 07:33:35.527573 cashfree_lrs_client-1.0.2/cashfree_lrs_client/docs/Purpose.md
+-rw-r--r--   0        0        0     1239 2023-05-01 07:33:35.527573 cashfree_lrs_client-1.0.2/cashfree_lrs_client/docs/SetupWebhooksRequest.md
+-rw-r--r--   0        0        0      896 2023-05-01 07:33:35.527573 cashfree_lrs_client-1.0.2/cashfree_lrs_client/docs/SuccessMessage.md
+-rw-r--r--   0        0        0     4503 2023-05-01 07:34:04.963553 cashfree_lrs_client-1.0.2/cashfree_lrs_client/exceptions.py
+-rw-r--r--   0        0        0      353 2023-05-01 07:34:05.011553 cashfree_lrs_client-1.0.2/cashfree_lrs_client/model/__init__.py
+-rw-r--r--   0        0        0      884 2023-05-01 07:33:59.051553 cashfree_lrs_client-1.0.2/cashfree_lrs_client/model/amount.py
+-rw-r--r--   0        0        0      815 2023-05-01 07:33:59.131553 cashfree_lrs_client-1.0.2/cashfree_lrs_client/model/amount.pyi
+-rw-r--r--   0        0        0    14903 2023-05-01 07:33:59.987553 cashfree_lrs_client-1.0.2/cashfree_lrs_client/model/create_beneficiary_request.py
+-rw-r--r--   0        0        0    13066 2023-05-01 07:34:00.551553 cashfree_lrs_client-1.0.2/cashfree_lrs_client/model/create_beneficiary_request.pyi
+-rw-r--r--   0        0        0    11475 2023-05-01 07:34:01.079553 cashfree_lrs_client-1.0.2/cashfree_lrs_client/model/create_order_request.py
+-rw-r--r--   0        0        0    10572 2023-05-01 07:34:01.295553 cashfree_lrs_client-1.0.2/cashfree_lrs_client/model/create_order_request.pyi
+-rw-r--r--   0        0        0     8398 2023-05-01 07:34:01.567553 cashfree_lrs_client-1.0.2/cashfree_lrs_client/model/create_order_response.py
+-rw-r--r--   0        0        0     8166 2023-05-01 07:34:01.707553 cashfree_lrs_client-1.0.2/cashfree_lrs_client/model/create_order_response.pyi
+-rw-r--r--   0        0        0    12349 2023-05-01 07:34:02.151553 cashfree_lrs_client-1.0.2/cashfree_lrs_client/model/create_remitter_request.py
+-rw-r--r--   0        0        0    10785 2023-05-01 07:34:02.407553 cashfree_lrs_client-1.0.2/cashfree_lrs_client/model/create_remitter_request.pyi
+-rw-r--r--   0        0        0     1192 2023-05-01 07:34:02.507553 cashfree_lrs_client-1.0.2/cashfree_lrs_client/model/currency.py
+-rw-r--r--   0        0        0     1031 2023-05-01 07:34:02.519553 cashfree_lrs_client-1.0.2/cashfree_lrs_client/model/currency.pyi
+-rw-r--r--   0        0        0     3384 2023-05-01 07:34:02.567553 cashfree_lrs_client-1.0.2/cashfree_lrs_client/model/error.py
+-rw-r--r--   0        0        0     3384 2023-05-01 07:34:02.603553 cashfree_lrs_client-1.0.2/cashfree_lrs_client/model/error.pyi
+-rw-r--r--   0        0        0     5805 2023-05-01 07:34:02.667553 cashfree_lrs_client-1.0.2/cashfree_lrs_client/model/fetch_forex_rate_request.py
+-rw-r--r--   0        0        0     5697 2023-05-01 07:34:02.715553 cashfree_lrs_client-1.0.2/cashfree_lrs_client/model/fetch_forex_rate_request.pyi
+-rw-r--r--   0        0        0     1368 2023-05-01 07:34:02.759553 cashfree_lrs_client-1.0.2/cashfree_lrs_client/model/purpose.py
+-rw-r--r--   0        0        0     1169 2023-05-01 07:34:02.767553 cashfree_lrs_client-1.0.2/cashfree_lrs_client/model/purpose.pyi
+-rw-r--r--   0        0        0     3663 2023-05-01 07:34:02.815553 cashfree_lrs_client-1.0.2/cashfree_lrs_client/model/setup_webhooks_request.py
+-rw-r--r--   0        0        0     3663 2023-05-01 07:34:02.851553 cashfree_lrs_client-1.0.2/cashfree_lrs_client/model/setup_webhooks_request.pyi
+-rw-r--r--   0        0        0     2477 2023-05-01 07:34:02.899553 cashfree_lrs_client-1.0.2/cashfree_lrs_client/model/success_message.py
+-rw-r--r--   0        0        0     2477 2023-05-01 07:34:02.915553 cashfree_lrs_client-1.0.2/cashfree_lrs_client/model/success_message.pyi
+-rw-r--r--   0        0        0     1173 2023-05-01 07:34:05.011553 cashfree_lrs_client-1.0.2/cashfree_lrs_client/models/__init__.py
+-rw-r--r--   0        0        0     1975 2023-05-01 07:33:35.527573 cashfree_lrs_client-1.0.2/cashfree_lrs_client/models/create_beneficiary200_response.py
+-rw-r--r--   0        0        0     5826 2023-05-01 07:33:35.527573 cashfree_lrs_client-1.0.2/cashfree_lrs_client/models/create_beneficiary_request.py
+-rw-r--r--   0        0        0     4904 2023-05-01 07:33:35.527573 cashfree_lrs_client-1.0.2/cashfree_lrs_client/models/create_order_request.py
+-rw-r--r--   0        0        0     2951 2023-05-01 07:33:35.527573 cashfree_lrs_client-1.0.2/cashfree_lrs_client/models/create_order_response.py
+-rw-r--r--   0        0        0     1951 2023-05-01 07:33:35.527573 cashfree_lrs_client-1.0.2/cashfree_lrs_client/models/create_remitter200_response.py
+-rw-r--r--   0        0        0     5289 2023-05-01 07:33:35.527573 cashfree_lrs_client-1.0.2/cashfree_lrs_client/models/create_remitter_request.py
+-rw-r--r--   0        0        0      608 2023-05-01 07:33:35.527573 cashfree_lrs_client-1.0.2/cashfree_lrs_client/models/currency.py
+-rw-r--r--   0        0        0     1964 2023-05-01 07:33:35.527573 cashfree_lrs_client-1.0.2/cashfree_lrs_client/models/error.py
+-rw-r--r--   0        0        0     3205 2023-05-01 07:33:35.527573 cashfree_lrs_client-1.0.2/cashfree_lrs_client/models/fetch_forex_rate_request.py
+-rw-r--r--   0        0        0     2903 2023-05-01 07:33:35.527573 cashfree_lrs_client-1.0.2/cashfree_lrs_client/models/order_response.py
+-rw-r--r--   0        0        0      626 2023-05-01 07:33:35.527573 cashfree_lrs_client-1.0.2/cashfree_lrs_client/models/purpose.py
+-rw-r--r--   0        0        0     1943 2023-05-01 07:33:35.527573 cashfree_lrs_client-1.0.2/cashfree_lrs_client/models/setup_webhooks200_response.py
+-rw-r--r--   0        0        0     2355 2023-05-01 07:33:35.527573 cashfree_lrs_client-1.0.2/cashfree_lrs_client/models/setup_webhooks_request.py
+-rw-r--r--   0        0        0     1863 2023-05-01 07:33:35.527573 cashfree_lrs_client-1.0.2/cashfree_lrs_client/models/success_message.py
+-rw-r--r--   0        0        0      644 2023-05-01 07:34:04.759553 cashfree_lrs_client-1.0.2/cashfree_lrs_client/paths/__init__.py
+-rw-r--r--   0        0        0      323 2023-05-01 07:34:04.763553 cashfree_lrs_client-1.0.2/cashfree_lrs_client/paths/beneficiaries/__init__.py
+-rw-r--r--   0        0        0    12582 2023-05-01 07:34:03.351553 cashfree_lrs_client-1.0.2/cashfree_lrs_client/paths/beneficiaries/post.py
+-rw-r--r--   0        0        0    12396 2023-05-01 07:34:03.463553 cashfree_lrs_client-1.0.2/cashfree_lrs_client/paths/beneficiaries/post.pyi
+-rw-r--r--   0        0        0      326 2023-05-01 07:34:04.759553 cashfree_lrs_client-1.0.2/cashfree_lrs_client/paths/fx_rate_details/__init__.py
+-rw-r--r--   0        0        0    11760 2023-05-01 07:34:04.035553 cashfree_lrs_client-1.0.2/cashfree_lrs_client/paths/fx_rate_details/post.py
+-rw-r--r--   0        0        0    11604 2023-05-01 07:34:04.139553 cashfree_lrs_client-1.0.2/cashfree_lrs_client/paths/fx_rate_details/post.pyi
+-rw-r--r--   0        0        0      309 2023-05-01 07:34:04.759553 cashfree_lrs_client-1.0.2/cashfree_lrs_client/paths/orders/__init__.py
+-rw-r--r--   0        0        0    13005 2023-05-01 07:34:03.591553 cashfree_lrs_client-1.0.2/cashfree_lrs_client/paths/orders/post.py
+-rw-r--r--   0        0        0    12789 2023-05-01 07:34:03.707553 cashfree_lrs_client-1.0.2/cashfree_lrs_client/paths/orders/post.pyi
+-rw-r--r--   0        0        0      343 2023-05-01 07:34:04.759553 cashfree_lrs_client-1.0.2/cashfree_lrs_client/paths/orders_documents_upload/__init__.py
+-rw-r--r--   0        0        0    12334 2023-05-01 07:34:03.123553 cashfree_lrs_client-1.0.2/cashfree_lrs_client/paths/orders_documents_upload/post.py
+-rw-r--r--   0        0        0    12148 2023-05-01 07:34:03.235553 cashfree_lrs_client-1.0.2/cashfree_lrs_client/paths/orders_documents_upload/post.pyi
+-rw-r--r--   0        0        0      361 2023-05-01 07:34:04.763553 cashfree_lrs_client-1.0.2/cashfree_lrs_client/paths/orders_order_id_documents_upload/__init__.py
+-rw-r--r--   0        0        0    15715 2023-05-01 07:34:04.631553 cashfree_lrs_client-1.0.2/cashfree_lrs_client/paths/orders_order_id_documents_upload/post.py
+-rw-r--r--   0        0        0    15469 2023-05-01 07:34:04.755553 cashfree_lrs_client-1.0.2/cashfree_lrs_client/paths/orders_order_id_documents_upload/post.pyi
+-rw-r--r--   0        0        0      343 2023-05-01 07:34:04.759553 cashfree_lrs_client-1.0.2/cashfree_lrs_client/paths/orders_order_id_process/__init__.py
+-rw-r--r--   0        0        0     8093 2023-05-01 07:34:04.215553 cashfree_lrs_client-1.0.2/cashfree_lrs_client/paths/orders_order_id_process/post.py
+-rw-r--r--   0        0        0     7937 2023-05-01 07:34:04.291553 cashfree_lrs_client-1.0.2/cashfree_lrs_client/paths/orders_order_id_process/post.pyi
+-rw-r--r--   0        0        0      315 2023-05-01 07:34:04.763553 cashfree_lrs_client-1.0.2/cashfree_lrs_client/paths/remitters/__init__.py
+-rw-r--r--   0        0        0    12525 2023-05-01 07:34:03.819553 cashfree_lrs_client-1.0.2/cashfree_lrs_client/paths/remitters/post.py
+-rw-r--r--   0        0        0    12339 2023-05-01 07:34:03.931553 cashfree_lrs_client-1.0.2/cashfree_lrs_client/paths/remitters/post.pyi
+-rw-r--r--   0        0        0      313 2023-05-01 07:34:04.759553 cashfree_lrs_client-1.0.2/cashfree_lrs_client/paths/webhooks/__init__.py
+-rw-r--r--   0        0        0    11939 2023-05-01 07:34:04.399553 cashfree_lrs_client-1.0.2/cashfree_lrs_client/paths/webhooks/post.py
+-rw-r--r--   0        0        0    11783 2023-05-01 07:34:04.503553 cashfree_lrs_client-1.0.2/cashfree_lrs_client/paths/webhooks/post.pyi
+-rw-r--r--   0        0        0    10536 2023-05-01 07:34:04.995553 cashfree_lrs_client-1.0.2/cashfree_lrs_client/rest.py
+-rw-r--r--   0        0        0    97649 2023-05-01 07:34:05.011553 cashfree_lrs_client-1.0.2/cashfree_lrs_client/schemas.py
+-rw-r--r--   0        0        0        0 2023-05-01 07:33:35.531573 cashfree_lrs_client-1.0.2/cashfree_lrs_client/test/__init__.py
+-rw-r--r--   0        0        0     2694 2023-05-01 07:33:35.531573 cashfree_lrs_client-1.0.2/cashfree_lrs_client/test/test_create_beneficiary_request.py
+-rw-r--r--   0        0        0     2292 2023-05-01 07:33:35.531573 cashfree_lrs_client-1.0.2/cashfree_lrs_client/test/test_create_order_request.py
+-rw-r--r--   0        0        0     1952 2023-05-01 07:33:35.531573 cashfree_lrs_client-1.0.2/cashfree_lrs_client/test/test_create_order_response.py
+-rw-r--r--   0        0        0     2486 2023-05-01 07:33:35.531573 cashfree_lrs_client-1.0.2/cashfree_lrs_client/test/test_create_remitter_request.py
+-rw-r--r--   0        0        0      738 2023-05-01 07:33:35.531573 cashfree_lrs_client-1.0.2/cashfree_lrs_client/test/test_currency.py
+-rw-r--r--   0        0        0     1439 2023-05-01 07:33:35.531573 cashfree_lrs_client-1.0.2/cashfree_lrs_client/test/test_error.py
+-rw-r--r--   0        0        0     1860 2023-05-01 07:33:35.531573 cashfree_lrs_client-1.0.2/cashfree_lrs_client/test/test_fetch_forex_rate_request.py
+-rw-r--r--   0        0        0     1845 2023-05-01 07:33:35.531573 cashfree_lrs_client-1.0.2/cashfree_lrs_client/test/test_lrs_api.py
+-rw-r--r--   0        0        0      731 2023-05-01 07:33:35.531573 cashfree_lrs_client-1.0.2/cashfree_lrs_client/test/test_purpose.py
+-rw-r--r--   0        0        0     1737 2023-05-01 07:33:35.531573 cashfree_lrs_client-1.0.2/cashfree_lrs_client/test/test_setup_webhooks_request.py
+-rw-r--r--   0        0        0     1493 2023-05-01 07:33:35.531573 cashfree_lrs_client-1.0.2/cashfree_lrs_client/test/test_success_message.py
+-rw-r--r--   0        0        0      698 2023-05-01 07:33:49.363558 cashfree_lrs_client-1.0.2/pyproject.toml
+-rw-r--r--   0        0        0    13295 1970-01-01 00:00:00.000000 cashfree_lrs_client-1.0.2/PKG-INFO
```

### Comparing `cashfree_lrs_client-1.0.1/README.md` & `cashfree_lrs_client-1.0.2/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # cashfree-lrs-client
 CashFree LRS APIs (v2)
 
 This Python package is automatically generated by the [OpenAPI Generator](https://openapi-generator.tech) project:
 
-- API version: 1.0.1
+- API version: 1.0.2
 - Package version: 1.0.0
 - Build package: org.openapitools.codegen.languages.PythonClientCodegen
 For more information, please visit [https://docs.cashfree.com](https://docs.cashfree.com)
 
 ## Requirements.
 
 Python &gt;&#x3D;3.7
@@ -210,14 +210,15 @@
 *LrsApi* | [**fetch_forex_rate**](docs/apis/tags/LrsApi.md#fetch_forex_rate) | **post** /fx-rate/details | Fetch FX Rate
 *LrsApi* | [**process_order**](docs/apis/tags/LrsApi.md#process_order) | **post** /orders/{order_id}/process | Process Order
 *LrsApi* | [**setup_webhooks**](docs/apis/tags/LrsApi.md#setup_webhooks) | **post** /webhooks | Setup Webhooks
 *LrsApi* | [**upload_documents**](docs/apis/tags/LrsApi.md#upload_documents) | **post** /orders/{order_id}/documents/upload | Upload Documents
 
 ## Documentation For Models
 
+ - [Amount](docs/models/Amount.md)
  - [CreateBeneficiaryRequest](docs/models/CreateBeneficiaryRequest.md)
  - [CreateOrderRequest](docs/models/CreateOrderRequest.md)
  - [CreateOrderResponse](docs/models/CreateOrderResponse.md)
  - [CreateRemitterRequest](docs/models/CreateRemitterRequest.md)
  - [Currency](docs/models/Currency.md)
  - [Error](docs/models/Error.md)
  - [FetchForexRateRequest](docs/models/FetchForexRateRequest.md)
```

### Comparing `cashfree_lrs_client-1.0.1/cashfree_lrs_client/__init__.py` & `cashfree_lrs_client-1.0.2/cashfree_lrs_client/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 # flake8: noqa
 
 """
     Cashfree LRS
 
     CashFree LRS APIs (v2)  # noqa: E501
 
-    The version of the OpenAPI document: 1.0.1
+    The version of the OpenAPI document: 1.0.2
     Contact: nextgenapi@cashfree.com
     Generated by: https://openapi-generator.tech
 """
 
 __version__ = "1.0.0"
 
 # import ApiClient
```

### Comparing `cashfree_lrs_client-1.0.1/cashfree_lrs_client/api/default_api.py` & `cashfree_lrs_client-1.0.2/cashfree_lrs_client/api/default_api.py`

 * *Files identical despite different names*

### Comparing `cashfree_lrs_client-1.0.1/cashfree_lrs_client/api/lrs_api.py` & `cashfree_lrs_client-1.0.2/cashfree_lrs_client/api/lrs_api.py`

 * *Files identical despite different names*

### Comparing `cashfree_lrs_client-1.0.1/cashfree_lrs_client/api_client.py` & `cashfree_lrs_client-1.0.2/cashfree_lrs_client/api_client.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # coding: utf-8
 """
     Cashfree LRS
 
     CashFree LRS APIs (v2)  # noqa: E501
 
-    The version of the OpenAPI document: 1.0.1
+    The version of the OpenAPI document: 1.0.2
     Contact: nextgenapi@cashfree.com
     Generated by: https://openapi-generator.tech
 """
 
 from dataclasses import dataclass
 from decimal import Decimal
 import enum
```

### Comparing `cashfree_lrs_client-1.0.1/cashfree_lrs_client/apis/path_to_api.py` & `cashfree_lrs_client-1.0.2/cashfree_lrs_client/apis/path_to_api.py`

 * *Files identical despite different names*

### Comparing `cashfree_lrs_client-1.0.1/cashfree_lrs_client/apis/tags/lrs_api.py` & `cashfree_lrs_client-1.0.2/cashfree_lrs_client/apis/tags/lrs_api.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Cashfree LRS
 
     CashFree LRS APIs (v2)  # noqa: E501
 
-    The version of the OpenAPI document: 1.0.1
+    The version of the OpenAPI document: 1.0.2
     Contact: nextgenapi@cashfree.com
     Generated by: https://openapi-generator.tech
 """
 
 from cashfree_lrs_client.paths.orders_documents_upload.post import BulkDocumentsUpload
 from cashfree_lrs_client.paths.beneficiaries.post import CreateBeneficiary
 from cashfree_lrs_client.paths.orders.post import CreateOrder
```

### Comparing `cashfree_lrs_client-1.0.1/cashfree_lrs_client/configuration.py` & `cashfree_lrs_client-1.0.2/cashfree_lrs_client/configuration.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Cashfree LRS
 
     CashFree LRS APIs (v2)  # noqa: E501
 
-    The version of the OpenAPI document: 1.0.1
+    The version of the OpenAPI document: 1.0.2
     Contact: nextgenapi@cashfree.com
     Generated by: https://openapi-generator.tech
 """
 
 import copy
 import logging
 import multiprocessing
@@ -414,15 +414,15 @@
         """Gets the essential information for debugging.
 
         :return: The report for debugging.
         """
         return "Python SDK Debug Report:\n"\
                "OS: {env}\n"\
                "Python Version: {pyversion}\n"\
-               "Version of the API: 1.0.1\n"\
+               "Version of the API: 1.0.2\n"\
                "SDK Package Version: 1.0.0".\
                format(env=sys.platform, pyversion=sys.version)
 
     def get_host_settings(self):
         """Gets an array of host settings
 
         :return: An array of host settings
```

### Comparing `cashfree_lrs_client-1.0.1/cashfree_lrs_client/docs/CreateBeneficiaryRequest.md` & `cashfree_lrs_client-1.0.2/cashfree_lrs_client/docs/CreateBeneficiaryRequest.md`

 * *Files identical despite different names*

### Comparing `cashfree_lrs_client-1.0.1/cashfree_lrs_client/docs/CreateOrderRequest.md` & `cashfree_lrs_client-1.0.2/cashfree_lrs_client/docs/CreateOrderRequest.md`

 * *Files identical despite different names*

### Comparing `cashfree_lrs_client-1.0.1/cashfree_lrs_client/docs/CreateOrderResponse.md` & `cashfree_lrs_client-1.0.2/cashfree_lrs_client/docs/CreateOrderResponse.md`

 * *Files identical despite different names*

### Comparing `cashfree_lrs_client-1.0.1/cashfree_lrs_client/docs/CreateRemitterRequest.md` & `cashfree_lrs_client-1.0.2/cashfree_lrs_client/docs/CreateRemitterRequest.md`

 * *Files identical despite different names*

### Comparing `cashfree_lrs_client-1.0.1/cashfree_lrs_client/docs/Error.md` & `cashfree_lrs_client-1.0.2/cashfree_lrs_client/docs/Error.md`

 * *Files identical despite different names*

### Comparing `cashfree_lrs_client-1.0.1/cashfree_lrs_client/docs/FetchForexRateRequest.md` & `cashfree_lrs_client-1.0.2/cashfree_lrs_client/docs/FetchForexRateRequest.md`

 * *Files identical despite different names*

### Comparing `cashfree_lrs_client-1.0.1/cashfree_lrs_client/docs/LrsApi.md` & `cashfree_lrs_client-1.0.2/cashfree_lrs_client/docs/LrsApi.md`

 * *Files identical despite different names*

### Comparing `cashfree_lrs_client-1.0.1/cashfree_lrs_client/docs/SetupWebhooksRequest.md` & `cashfree_lrs_client-1.0.2/cashfree_lrs_client/docs/SetupWebhooksRequest.md`

 * *Files identical despite different names*

### Comparing `cashfree_lrs_client-1.0.1/cashfree_lrs_client/docs/SuccessMessage.md` & `cashfree_lrs_client-1.0.2/cashfree_lrs_client/docs/SuccessMessage.md`

 * *Files identical despite different names*

### Comparing `cashfree_lrs_client-1.0.1/cashfree_lrs_client/exceptions.py` & `cashfree_lrs_client-1.0.2/cashfree_lrs_client/exceptions.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Cashfree LRS
 
     CashFree LRS APIs (v2)  # noqa: E501
 
-    The version of the OpenAPI document: 1.0.1
+    The version of the OpenAPI document: 1.0.2
     Contact: nextgenapi@cashfree.com
     Generated by: https://openapi-generator.tech
 """
 import dataclasses
 import typing
 
 from urllib3._collections import HTTPHeaderDict
```

### Comparing `cashfree_lrs_client-1.0.1/cashfree_lrs_client/model/create_beneficiary_request.py` & `cashfree_lrs_client-1.0.2/cashfree_lrs_client/model/create_beneficiary_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Cashfree LRS
 
     CashFree LRS APIs (v2)  # noqa: E501
 
-    The version of the OpenAPI document: 1.0.1
+    The version of the OpenAPI document: 1.0.2
     Contact: nextgenapi@cashfree.com
     Generated by: https://openapi-generator.tech
 """
 
 from datetime import date, datetime  # noqa: F401
 import decimal  # noqa: F401
 import functools  # noqa: F401
```

### Comparing `cashfree_lrs_client-1.0.1/cashfree_lrs_client/model/create_beneficiary_request.pyi` & `cashfree_lrs_client-1.0.2/cashfree_lrs_client/model/create_beneficiary_request.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Cashfree LRS
 
     CashFree LRS APIs (v2)  # noqa: E501
 
-    The version of the OpenAPI document: 1.0.1
+    The version of the OpenAPI document: 1.0.2
     Contact: nextgenapi@cashfree.com
     Generated by: https://openapi-generator.tech
 """
 
 from datetime import date, datetime  # noqa: F401
 import decimal  # noqa: F401
 import functools  # noqa: F401
```

### Comparing `cashfree_lrs_client-1.0.1/cashfree_lrs_client/model/create_order_request.py` & `cashfree_lrs_client-1.0.2/cashfree_lrs_client/model/create_order_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Cashfree LRS
 
     CashFree LRS APIs (v2)  # noqa: E501
 
-    The version of the OpenAPI document: 1.0.1
+    The version of the OpenAPI document: 1.0.2
     Contact: nextgenapi@cashfree.com
     Generated by: https://openapi-generator.tech
 """
 
 from datetime import date, datetime  # noqa: F401
 import decimal  # noqa: F401
 import functools  # noqa: F401
```

### Comparing `cashfree_lrs_client-1.0.1/cashfree_lrs_client/model/create_order_request.pyi` & `cashfree_lrs_client-1.0.2/cashfree_lrs_client/model/create_order_request.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Cashfree LRS
 
     CashFree LRS APIs (v2)  # noqa: E501
 
-    The version of the OpenAPI document: 1.0.1
+    The version of the OpenAPI document: 1.0.2
     Contact: nextgenapi@cashfree.com
     Generated by: https://openapi-generator.tech
 """
 
 from datetime import date, datetime  # noqa: F401
 import decimal  # noqa: F401
 import functools  # noqa: F401
```

### Comparing `cashfree_lrs_client-1.0.1/cashfree_lrs_client/model/create_order_response.py` & `cashfree_lrs_client-1.0.2/cashfree_lrs_client/model/create_order_response.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Cashfree LRS
 
     CashFree LRS APIs (v2)  # noqa: E501
 
-    The version of the OpenAPI document: 1.0.1
+    The version of the OpenAPI document: 1.0.2
     Contact: nextgenapi@cashfree.com
     Generated by: https://openapi-generator.tech
 """
 
 from datetime import date, datetime  # noqa: F401
 import decimal  # noqa: F401
 import functools  # noqa: F401
@@ -36,60 +36,42 @@
 
     class MetaOapg:
         
         class properties:
             
             
             class tcs(
-                schemas.Float64Schema
+                schemas.Int32Schema
             ):
             
             
                 class MetaOapg:
-                    format = 'double'
-                    inclusive_minimum = 0
-            
-            
-            class gst(
-                schemas.Float64Schema
-            ):
-            
-            
-                class MetaOapg:
-                    format = 'double'
-                    inclusive_minimum = 0
-            
-            
-            class fx_rate(
-                schemas.Float64Schema
-            ):
-            
-            
-                class MetaOapg:
-                    format = 'double'
-                    inclusive_minimum = 0
-            
-            
-            class amount_to_pay(
-                schemas.Float64Schema
-            ):
-            
-            
-                class MetaOapg:
-                    format = 'double'
+                    format = 'int32'
                     inclusive_minimum = 0
+        
+            @staticmethod
+            def gst() -> typing.Type['Amount']:
+                return Amount
+        
+            @staticmethod
+            def fx_rate() -> typing.Type['Amount']:
+                return Amount
+        
+            @staticmethod
+            def amount_to_pay() -> typing.Type['Amount']:
+                return Amount
             
             
             class handling_charges(
-                schemas.Float64Schema
+                schemas.Int32Schema
             ):
             
             
                 class MetaOapg:
-                    format = 'double'
+                    format = 'int32'
                     inclusive_minimum = 0
             order_expiry_time = schemas.DateTimeSchema
             payment_link = schemas.StrSchema
             order_token = schemas.StrSchema
             
             
             class missing_documents(
@@ -125,21 +107,21 @@
                 "missing_documents": missing_documents,
             }
     
     @typing.overload
     def __getitem__(self, name: typing_extensions.Literal["tcs"]) -> MetaOapg.properties.tcs: ...
     
     @typing.overload
-    def __getitem__(self, name: typing_extensions.Literal["gst"]) -> MetaOapg.properties.gst: ...
+    def __getitem__(self, name: typing_extensions.Literal["gst"]) -> 'Amount': ...
     
     @typing.overload
-    def __getitem__(self, name: typing_extensions.Literal["fx_rate"]) -> MetaOapg.properties.fx_rate: ...
+    def __getitem__(self, name: typing_extensions.Literal["fx_rate"]) -> 'Amount': ...
     
     @typing.overload
-    def __getitem__(self, name: typing_extensions.Literal["amount_to_pay"]) -> MetaOapg.properties.amount_to_pay: ...
+    def __getitem__(self, name: typing_extensions.Literal["amount_to_pay"]) -> 'Amount': ...
     
     @typing.overload
     def __getitem__(self, name: typing_extensions.Literal["handling_charges"]) -> MetaOapg.properties.handling_charges: ...
     
     @typing.overload
     def __getitem__(self, name: typing_extensions.Literal["order_expiry_time"]) -> MetaOapg.properties.order_expiry_time: ...
     
@@ -160,21 +142,21 @@
         return super().__getitem__(name)
     
     
     @typing.overload
     def get_item_oapg(self, name: typing_extensions.Literal["tcs"]) -> typing.Union[MetaOapg.properties.tcs, schemas.Unset]: ...
     
     @typing.overload
-    def get_item_oapg(self, name: typing_extensions.Literal["gst"]) -> typing.Union[MetaOapg.properties.gst, schemas.Unset]: ...
+    def get_item_oapg(self, name: typing_extensions.Literal["gst"]) -> typing.Union['Amount', schemas.Unset]: ...
     
     @typing.overload
-    def get_item_oapg(self, name: typing_extensions.Literal["fx_rate"]) -> typing.Union[MetaOapg.properties.fx_rate, schemas.Unset]: ...
+    def get_item_oapg(self, name: typing_extensions.Literal["fx_rate"]) -> typing.Union['Amount', schemas.Unset]: ...
     
     @typing.overload
-    def get_item_oapg(self, name: typing_extensions.Literal["amount_to_pay"]) -> typing.Union[MetaOapg.properties.amount_to_pay, schemas.Unset]: ...
+    def get_item_oapg(self, name: typing_extensions.Literal["amount_to_pay"]) -> typing.Union['Amount', schemas.Unset]: ...
     
     @typing.overload
     def get_item_oapg(self, name: typing_extensions.Literal["handling_charges"]) -> typing.Union[MetaOapg.properties.handling_charges, schemas.Unset]: ...
     
     @typing.overload
     def get_item_oapg(self, name: typing_extensions.Literal["order_expiry_time"]) -> typing.Union[MetaOapg.properties.order_expiry_time, schemas.Unset]: ...
     
@@ -193,19 +175,19 @@
     def get_item_oapg(self, name: typing.Union[typing_extensions.Literal["tcs", "gst", "fx_rate", "amount_to_pay", "handling_charges", "order_expiry_time", "payment_link", "order_token", "missing_documents", ], str]):
         return super().get_item_oapg(name)
     
 
     def __new__(
         cls,
         *_args: typing.Union[dict, frozendict.frozendict, ],
-        tcs: typing.Union[MetaOapg.properties.tcs, decimal.Decimal, int, float, schemas.Unset] = schemas.unset,
-        gst: typing.Union[MetaOapg.properties.gst, decimal.Decimal, int, float, schemas.Unset] = schemas.unset,
-        fx_rate: typing.Union[MetaOapg.properties.fx_rate, decimal.Decimal, int, float, schemas.Unset] = schemas.unset,
-        amount_to_pay: typing.Union[MetaOapg.properties.amount_to_pay, decimal.Decimal, int, float, schemas.Unset] = schemas.unset,
-        handling_charges: typing.Union[MetaOapg.properties.handling_charges, decimal.Decimal, int, float, schemas.Unset] = schemas.unset,
+        tcs: typing.Union[MetaOapg.properties.tcs, decimal.Decimal, int, schemas.Unset] = schemas.unset,
+        gst: typing.Union['Amount', schemas.Unset] = schemas.unset,
+        fx_rate: typing.Union['Amount', schemas.Unset] = schemas.unset,
+        amount_to_pay: typing.Union['Amount', schemas.Unset] = schemas.unset,
+        handling_charges: typing.Union[MetaOapg.properties.handling_charges, decimal.Decimal, int, schemas.Unset] = schemas.unset,
         order_expiry_time: typing.Union[MetaOapg.properties.order_expiry_time, str, datetime, schemas.Unset] = schemas.unset,
         payment_link: typing.Union[MetaOapg.properties.payment_link, str, schemas.Unset] = schemas.unset,
         order_token: typing.Union[MetaOapg.properties.order_token, str, schemas.Unset] = schemas.unset,
         missing_documents: typing.Union[MetaOapg.properties.missing_documents, list, tuple, schemas.Unset] = schemas.unset,
         _configuration: typing.Optional[schemas.Configuration] = None,
         **kwargs: typing.Union[schemas.AnyTypeSchema, dict, frozendict.frozendict, str, date, datetime, uuid.UUID, int, float, decimal.Decimal, None, list, tuple, bytes],
     ) -> 'CreateOrderResponse':
@@ -220,7 +202,9 @@
             order_expiry_time=order_expiry_time,
             payment_link=payment_link,
             order_token=order_token,
             missing_documents=missing_documents,
             _configuration=_configuration,
             **kwargs,
         )
+
+from cashfree_lrs_client.model.amount import Amount
```

### Comparing `cashfree_lrs_client-1.0.1/cashfree_lrs_client/model/create_remitter_request.py` & `cashfree_lrs_client-1.0.2/cashfree_lrs_client/model/create_remitter_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Cashfree LRS
 
     CashFree LRS APIs (v2)  # noqa: E501
 
-    The version of the OpenAPI document: 1.0.1
+    The version of the OpenAPI document: 1.0.2
     Contact: nextgenapi@cashfree.com
     Generated by: https://openapi-generator.tech
 """
 
 from datetime import date, datetime  # noqa: F401
 import decimal  # noqa: F401
 import functools  # noqa: F401
```

### Comparing `cashfree_lrs_client-1.0.1/cashfree_lrs_client/model/create_remitter_request.pyi` & `cashfree_lrs_client-1.0.2/cashfree_lrs_client/model/create_remitter_request.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Cashfree LRS
 
     CashFree LRS APIs (v2)  # noqa: E501
 
-    The version of the OpenAPI document: 1.0.1
+    The version of the OpenAPI document: 1.0.2
     Contact: nextgenapi@cashfree.com
     Generated by: https://openapi-generator.tech
 """
 
 from datetime import date, datetime  # noqa: F401
 import decimal  # noqa: F401
 import functools  # noqa: F401
```

### Comparing `cashfree_lrs_client-1.0.1/cashfree_lrs_client/model/currency.py` & `cashfree_lrs_client-1.0.2/cashfree_lrs_client/model/currency.pyi`

 * *Files 15% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Cashfree LRS
 
     CashFree LRS APIs (v2)  # noqa: E501
 
-    The version of the OpenAPI document: 1.0.1
+    The version of the OpenAPI document: 1.0.2
     Contact: nextgenapi@cashfree.com
     Generated by: https://openapi-generator.tech
 """
 
 from datetime import date, datetime  # noqa: F401
 import decimal  # noqa: F401
 import functools  # noqa: F401
@@ -31,21 +31,14 @@
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
 
     ISO Currency code of currency in which remittance needs to be settled. Only 3 characters are allowed.
     """
-
-
-    class MetaOapg:
-        enum_value_to_name = {
-            "USD": "USD",
-            "INR": "INR",
-        }
     
     @schemas.classproperty
     def USD(cls):
         return cls("USD")
     
     @schemas.classproperty
     def INR(cls):
```

### Comparing `cashfree_lrs_client-1.0.1/cashfree_lrs_client/model/currency.pyi` & `cashfree_lrs_client-1.0.2/cashfree_lrs_client/model/currency.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Cashfree LRS
 
     CashFree LRS APIs (v2)  # noqa: E501
 
-    The version of the OpenAPI document: 1.0.1
+    The version of the OpenAPI document: 1.0.2
     Contact: nextgenapi@cashfree.com
     Generated by: https://openapi-generator.tech
 """
 
 from datetime import date, datetime  # noqa: F401
 import decimal  # noqa: F401
 import functools  # noqa: F401
@@ -31,14 +31,23 @@
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
 
     ISO Currency code of currency in which remittance needs to be settled. Only 3 characters are allowed.
     """
+
+
+    class MetaOapg:
+        max_length = 3
+        min_length = 3
+        enum_value_to_name = {
+            "USD": "USD",
+            "INR": "INR",
+        }
     
     @schemas.classproperty
     def USD(cls):
         return cls("USD")
     
     @schemas.classproperty
     def INR(cls):
```

### Comparing `cashfree_lrs_client-1.0.1/cashfree_lrs_client/model/error.py` & `cashfree_lrs_client-1.0.2/cashfree_lrs_client/model/error.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Cashfree LRS
 
     CashFree LRS APIs (v2)  # noqa: E501
 
-    The version of the OpenAPI document: 1.0.1
+    The version of the OpenAPI document: 1.0.2
     Contact: nextgenapi@cashfree.com
     Generated by: https://openapi-generator.tech
 """
 
 from datetime import date, datetime  # noqa: F401
 import decimal  # noqa: F401
 import functools  # noqa: F401
@@ -28,15 +28,15 @@
     schemas.DictSchema
 ):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
 
-    Error response
+    Common error response
     """
 
 
     class MetaOapg:
         
         class properties:
             message = schemas.StrSchema
```

### Comparing `cashfree_lrs_client-1.0.1/cashfree_lrs_client/model/error.pyi` & `cashfree_lrs_client-1.0.2/cashfree_lrs_client/model/error.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Cashfree LRS
 
     CashFree LRS APIs (v2)  # noqa: E501
 
-    The version of the OpenAPI document: 1.0.1
+    The version of the OpenAPI document: 1.0.2
     Contact: nextgenapi@cashfree.com
     Generated by: https://openapi-generator.tech
 """
 
 from datetime import date, datetime  # noqa: F401
 import decimal  # noqa: F401
 import functools  # noqa: F401
@@ -28,15 +28,15 @@
     schemas.DictSchema
 ):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
 
-    Error response
+    Common error response
     """
 
 
     class MetaOapg:
         
         class properties:
             message = schemas.StrSchema
```

### Comparing `cashfree_lrs_client-1.0.1/cashfree_lrs_client/model/fetch_forex_rate_request.py` & `cashfree_lrs_client-1.0.2/cashfree_lrs_client/model/fetch_forex_rate_request.pyi`

 * *Files 6% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Cashfree LRS
 
     CashFree LRS APIs (v2)  # noqa: E501
 
-    The version of the OpenAPI document: 1.0.1
+    The version of the OpenAPI document: 1.0.2
     Contact: nextgenapi@cashfree.com
     Generated by: https://openapi-generator.tech
 """
 
 from datetime import date, datetime  # noqa: F401
 import decimal  # noqa: F401
 import functools  # noqa: F401
@@ -52,26 +52,24 @@
             def purpose() -> typing.Type['Purpose']:
                 return Purpose
             
             
             class remitter_id(
                 schemas.StrSchema
             ):
-            
-            
-                class MetaOapg:
-                    max_length = 50
-                    min_length = 3
+                pass
             customer_declaration = schemas.Float64Schema
+            education_loan = schemas.BoolSchema
             __annotations__ = {
                 "to_currency": to_currency,
                 "to_amount": to_amount,
                 "purpose": purpose,
                 "remitter_id": remitter_id,
                 "customer_declaration": customer_declaration,
+                "education_loan": education_loan,
             }
     
     to_amount: MetaOapg.properties.to_amount
     purpose: 'Purpose'
     to_currency: 'Currency'
     
     @typing.overload
@@ -86,17 +84,20 @@
     @typing.overload
     def __getitem__(self, name: typing_extensions.Literal["remitter_id"]) -> MetaOapg.properties.remitter_id: ...
     
     @typing.overload
     def __getitem__(self, name: typing_extensions.Literal["customer_declaration"]) -> MetaOapg.properties.customer_declaration: ...
     
     @typing.overload
+    def __getitem__(self, name: typing_extensions.Literal["education_loan"]) -> MetaOapg.properties.education_loan: ...
+    
+    @typing.overload
     def __getitem__(self, name: str) -> schemas.UnsetAnyTypeSchema: ...
     
-    def __getitem__(self, name: typing.Union[typing_extensions.Literal["to_currency", "to_amount", "purpose", "remitter_id", "customer_declaration", ], str]):
+    def __getitem__(self, name: typing.Union[typing_extensions.Literal["to_currency", "to_amount", "purpose", "remitter_id", "customer_declaration", "education_loan", ], str]):
         # dict_instance[name] accessor
         return super().__getitem__(name)
     
     
     @typing.overload
     def get_item_oapg(self, name: typing_extensions.Literal["to_currency"]) -> 'Currency': ...
     
@@ -109,38 +110,43 @@
     @typing.overload
     def get_item_oapg(self, name: typing_extensions.Literal["remitter_id"]) -> typing.Union[MetaOapg.properties.remitter_id, schemas.Unset]: ...
     
     @typing.overload
     def get_item_oapg(self, name: typing_extensions.Literal["customer_declaration"]) -> typing.Union[MetaOapg.properties.customer_declaration, schemas.Unset]: ...
     
     @typing.overload
+    def get_item_oapg(self, name: typing_extensions.Literal["education_loan"]) -> typing.Union[MetaOapg.properties.education_loan, schemas.Unset]: ...
+    
+    @typing.overload
     def get_item_oapg(self, name: str) -> typing.Union[schemas.UnsetAnyTypeSchema, schemas.Unset]: ...
     
-    def get_item_oapg(self, name: typing.Union[typing_extensions.Literal["to_currency", "to_amount", "purpose", "remitter_id", "customer_declaration", ], str]):
+    def get_item_oapg(self, name: typing.Union[typing_extensions.Literal["to_currency", "to_amount", "purpose", "remitter_id", "customer_declaration", "education_loan", ], str]):
         return super().get_item_oapg(name)
     
 
     def __new__(
         cls,
         *_args: typing.Union[dict, frozendict.frozendict, ],
         to_amount: typing.Union[MetaOapg.properties.to_amount, decimal.Decimal, int, float, ],
         purpose: 'Purpose',
         to_currency: 'Currency',
         remitter_id: typing.Union[MetaOapg.properties.remitter_id, str, schemas.Unset] = schemas.unset,
         customer_declaration: typing.Union[MetaOapg.properties.customer_declaration, decimal.Decimal, int, float, schemas.Unset] = schemas.unset,
+        education_loan: typing.Union[MetaOapg.properties.education_loan, bool, schemas.Unset] = schemas.unset,
         _configuration: typing.Optional[schemas.Configuration] = None,
         **kwargs: typing.Union[schemas.AnyTypeSchema, dict, frozendict.frozendict, str, date, datetime, uuid.UUID, int, float, decimal.Decimal, None, list, tuple, bytes],
     ) -> 'FetchForexRateRequest':
         return super().__new__(
             cls,
             *_args,
             to_amount=to_amount,
             purpose=purpose,
             to_currency=to_currency,
             remitter_id=remitter_id,
             customer_declaration=customer_declaration,
+            education_loan=education_loan,
             _configuration=_configuration,
             **kwargs,
         )
 
 from cashfree_lrs_client.model.currency import Currency
 from cashfree_lrs_client.model.purpose import Purpose
```

### Comparing `cashfree_lrs_client-1.0.1/cashfree_lrs_client/model/fetch_forex_rate_request.pyi` & `cashfree_lrs_client-1.0.2/cashfree_lrs_client/model/fetch_forex_rate_request.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Cashfree LRS
 
     CashFree LRS APIs (v2)  # noqa: E501
 
-    The version of the OpenAPI document: 1.0.1
+    The version of the OpenAPI document: 1.0.2
     Contact: nextgenapi@cashfree.com
     Generated by: https://openapi-generator.tech
 """
 
 from datetime import date, datetime  # noqa: F401
 import decimal  # noqa: F401
 import functools  # noqa: F401
@@ -52,22 +52,28 @@
             def purpose() -> typing.Type['Purpose']:
                 return Purpose
             
             
             class remitter_id(
                 schemas.StrSchema
             ):
-                pass
+            
+            
+                class MetaOapg:
+                    max_length = 50
+                    min_length = 3
             customer_declaration = schemas.Float64Schema
+            education_loan = schemas.BoolSchema
             __annotations__ = {
                 "to_currency": to_currency,
                 "to_amount": to_amount,
                 "purpose": purpose,
                 "remitter_id": remitter_id,
                 "customer_declaration": customer_declaration,
+                "education_loan": education_loan,
             }
     
     to_amount: MetaOapg.properties.to_amount
     purpose: 'Purpose'
     to_currency: 'Currency'
     
     @typing.overload
@@ -82,17 +88,20 @@
     @typing.overload
     def __getitem__(self, name: typing_extensions.Literal["remitter_id"]) -> MetaOapg.properties.remitter_id: ...
     
     @typing.overload
     def __getitem__(self, name: typing_extensions.Literal["customer_declaration"]) -> MetaOapg.properties.customer_declaration: ...
     
     @typing.overload
+    def __getitem__(self, name: typing_extensions.Literal["education_loan"]) -> MetaOapg.properties.education_loan: ...
+    
+    @typing.overload
     def __getitem__(self, name: str) -> schemas.UnsetAnyTypeSchema: ...
     
-    def __getitem__(self, name: typing.Union[typing_extensions.Literal["to_currency", "to_amount", "purpose", "remitter_id", "customer_declaration", ], str]):
+    def __getitem__(self, name: typing.Union[typing_extensions.Literal["to_currency", "to_amount", "purpose", "remitter_id", "customer_declaration", "education_loan", ], str]):
         # dict_instance[name] accessor
         return super().__getitem__(name)
     
     
     @typing.overload
     def get_item_oapg(self, name: typing_extensions.Literal["to_currency"]) -> 'Currency': ...
     
@@ -105,38 +114,43 @@
     @typing.overload
     def get_item_oapg(self, name: typing_extensions.Literal["remitter_id"]) -> typing.Union[MetaOapg.properties.remitter_id, schemas.Unset]: ...
     
     @typing.overload
     def get_item_oapg(self, name: typing_extensions.Literal["customer_declaration"]) -> typing.Union[MetaOapg.properties.customer_declaration, schemas.Unset]: ...
     
     @typing.overload
+    def get_item_oapg(self, name: typing_extensions.Literal["education_loan"]) -> typing.Union[MetaOapg.properties.education_loan, schemas.Unset]: ...
+    
+    @typing.overload
     def get_item_oapg(self, name: str) -> typing.Union[schemas.UnsetAnyTypeSchema, schemas.Unset]: ...
     
-    def get_item_oapg(self, name: typing.Union[typing_extensions.Literal["to_currency", "to_amount", "purpose", "remitter_id", "customer_declaration", ], str]):
+    def get_item_oapg(self, name: typing.Union[typing_extensions.Literal["to_currency", "to_amount", "purpose", "remitter_id", "customer_declaration", "education_loan", ], str]):
         return super().get_item_oapg(name)
     
 
     def __new__(
         cls,
         *_args: typing.Union[dict, frozendict.frozendict, ],
         to_amount: typing.Union[MetaOapg.properties.to_amount, decimal.Decimal, int, float, ],
         purpose: 'Purpose',
         to_currency: 'Currency',
         remitter_id: typing.Union[MetaOapg.properties.remitter_id, str, schemas.Unset] = schemas.unset,
         customer_declaration: typing.Union[MetaOapg.properties.customer_declaration, decimal.Decimal, int, float, schemas.Unset] = schemas.unset,
+        education_loan: typing.Union[MetaOapg.properties.education_loan, bool, schemas.Unset] = schemas.unset,
         _configuration: typing.Optional[schemas.Configuration] = None,
         **kwargs: typing.Union[schemas.AnyTypeSchema, dict, frozendict.frozendict, str, date, datetime, uuid.UUID, int, float, decimal.Decimal, None, list, tuple, bytes],
     ) -> 'FetchForexRateRequest':
         return super().__new__(
             cls,
             *_args,
             to_amount=to_amount,
             purpose=purpose,
             to_currency=to_currency,
             remitter_id=remitter_id,
             customer_declaration=customer_declaration,
+            education_loan=education_loan,
             _configuration=_configuration,
             **kwargs,
         )
 
 from cashfree_lrs_client.model.currency import Currency
 from cashfree_lrs_client.model.purpose import Purpose
```

### Comparing `cashfree_lrs_client-1.0.1/cashfree_lrs_client/model/purpose.py` & `cashfree_lrs_client-1.0.2/cashfree_lrs_client/model/purpose.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Cashfree LRS
 
     CashFree LRS APIs (v2)  # noqa: E501
 
-    The version of the OpenAPI document: 1.0.1
+    The version of the OpenAPI document: 1.0.2
     Contact: nextgenapi@cashfree.com
     Generated by: https://openapi-generator.tech
 """
 
 from datetime import date, datetime  # noqa: F401
 import decimal  # noqa: F401
 import functools  # noqa: F401
```

### Comparing `cashfree_lrs_client-1.0.1/cashfree_lrs_client/model/purpose.pyi` & `cashfree_lrs_client-1.0.2/cashfree_lrs_client/model/purpose.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Cashfree LRS
 
     CashFree LRS APIs (v2)  # noqa: E501
 
-    The version of the OpenAPI document: 1.0.1
+    The version of the OpenAPI document: 1.0.2
     Contact: nextgenapi@cashfree.com
     Generated by: https://openapi-generator.tech
 """
 
 from datetime import date, datetime  # noqa: F401
 import decimal  # noqa: F401
 import functools  # noqa: F401
```

### Comparing `cashfree_lrs_client-1.0.1/cashfree_lrs_client/model/setup_webhooks_request.py` & `cashfree_lrs_client-1.0.2/cashfree_lrs_client/model/setup_webhooks_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Cashfree LRS
 
     CashFree LRS APIs (v2)  # noqa: E501
 
-    The version of the OpenAPI document: 1.0.1
+    The version of the OpenAPI document: 1.0.2
     Contact: nextgenapi@cashfree.com
     Generated by: https://openapi-generator.tech
 """
 
 from datetime import date, datetime  # noqa: F401
 import decimal  # noqa: F401
 import functools  # noqa: F401
```

### Comparing `cashfree_lrs_client-1.0.1/cashfree_lrs_client/model/setup_webhooks_request.pyi` & `cashfree_lrs_client-1.0.2/cashfree_lrs_client/model/setup_webhooks_request.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Cashfree LRS
 
     CashFree LRS APIs (v2)  # noqa: E501
 
-    The version of the OpenAPI document: 1.0.1
+    The version of the OpenAPI document: 1.0.2
     Contact: nextgenapi@cashfree.com
     Generated by: https://openapi-generator.tech
 """
 
 from datetime import date, datetime  # noqa: F401
 import decimal  # noqa: F401
 import functools  # noqa: F401
```

### Comparing `cashfree_lrs_client-1.0.1/cashfree_lrs_client/model/success_message.py` & `cashfree_lrs_client-1.0.2/cashfree_lrs_client/model/success_message.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Cashfree LRS
 
     CashFree LRS APIs (v2)  # noqa: E501
 
-    The version of the OpenAPI document: 1.0.1
+    The version of the OpenAPI document: 1.0.2
     Contact: nextgenapi@cashfree.com
     Generated by: https://openapi-generator.tech
 """
 
 from datetime import date, datetime  # noqa: F401
 import decimal  # noqa: F401
 import functools  # noqa: F401
@@ -27,14 +27,16 @@
 class SuccessMessage(
     schemas.DictSchema
 ):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
+
+    Success message for when API is processed successfully
     """
 
 
     class MetaOapg:
         
         class properties:
             message = schemas.StrSchema
```

### Comparing `cashfree_lrs_client-1.0.1/cashfree_lrs_client/model/success_message.pyi` & `cashfree_lrs_client-1.0.2/cashfree_lrs_client/model/success_message.pyi`

 * *Files 6% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Cashfree LRS
 
     CashFree LRS APIs (v2)  # noqa: E501
 
-    The version of the OpenAPI document: 1.0.1
+    The version of the OpenAPI document: 1.0.2
     Contact: nextgenapi@cashfree.com
     Generated by: https://openapi-generator.tech
 """
 
 from datetime import date, datetime  # noqa: F401
 import decimal  # noqa: F401
 import functools  # noqa: F401
@@ -27,14 +27,16 @@
 class SuccessMessage(
     schemas.DictSchema
 ):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
+
+    Success message for when API is processed successfully
     """
 
 
     class MetaOapg:
         
         class properties:
             message = schemas.StrSchema
```

### Comparing `cashfree_lrs_client-1.0.1/cashfree_lrs_client/models/__init__.py` & `cashfree_lrs_client-1.0.2/cashfree_lrs_client/models/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 # raise a RecursionError
 # to avoid this, import only the models that you directly need like:
 # from cashfree_lrs_client.model.pet import Pet
 # or import this package, but before doing it, use:
 # import sys
 # sys.setrecursionlimit(n)
 
+from cashfree_lrs_client.model.amount import Amount
 from cashfree_lrs_client.model.create_beneficiary_request import CreateBeneficiaryRequest
 from cashfree_lrs_client.model.create_order_request import CreateOrderRequest
 from cashfree_lrs_client.model.create_order_response import CreateOrderResponse
 from cashfree_lrs_client.model.create_remitter_request import CreateRemitterRequest
 from cashfree_lrs_client.model.currency import Currency
 from cashfree_lrs_client.model.error import Error
 from cashfree_lrs_client.model.fetch_forex_rate_request import FetchForexRateRequest
```

### Comparing `cashfree_lrs_client-1.0.1/cashfree_lrs_client/models/create_beneficiary200_response.py` & `cashfree_lrs_client-1.0.2/cashfree_lrs_client/models/create_beneficiary200_response.py`

 * *Files identical despite different names*

### Comparing `cashfree_lrs_client-1.0.1/cashfree_lrs_client/models/create_beneficiary_request.py` & `cashfree_lrs_client-1.0.2/cashfree_lrs_client/models/create_beneficiary_request.py`

 * *Files identical despite different names*

### Comparing `cashfree_lrs_client-1.0.1/cashfree_lrs_client/models/create_order_request.py` & `cashfree_lrs_client-1.0.2/cashfree_lrs_client/models/create_order_request.py`

 * *Files identical despite different names*

### Comparing `cashfree_lrs_client-1.0.1/cashfree_lrs_client/models/create_order_response.py` & `cashfree_lrs_client-1.0.2/cashfree_lrs_client/models/create_order_response.py`

 * *Files identical despite different names*

### Comparing `cashfree_lrs_client-1.0.1/cashfree_lrs_client/models/create_remitter200_response.py` & `cashfree_lrs_client-1.0.2/cashfree_lrs_client/models/create_remitter200_response.py`

 * *Files identical despite different names*

### Comparing `cashfree_lrs_client-1.0.1/cashfree_lrs_client/models/create_remitter_request.py` & `cashfree_lrs_client-1.0.2/cashfree_lrs_client/models/create_remitter_request.py`

 * *Files identical despite different names*

### Comparing `cashfree_lrs_client-1.0.1/cashfree_lrs_client/models/currency.py` & `cashfree_lrs_client-1.0.2/cashfree_lrs_client/models/currency.py`

 * *Files identical despite different names*

### Comparing `cashfree_lrs_client-1.0.1/cashfree_lrs_client/models/error.py` & `cashfree_lrs_client-1.0.2/cashfree_lrs_client/models/error.py`

 * *Files identical despite different names*

### Comparing `cashfree_lrs_client-1.0.1/cashfree_lrs_client/models/fetch_forex_rate_request.py` & `cashfree_lrs_client-1.0.2/cashfree_lrs_client/models/fetch_forex_rate_request.py`

 * *Files identical despite different names*

### Comparing `cashfree_lrs_client-1.0.1/cashfree_lrs_client/models/order_response.py` & `cashfree_lrs_client-1.0.2/cashfree_lrs_client/models/order_response.py`

 * *Files identical despite different names*

### Comparing `cashfree_lrs_client-1.0.1/cashfree_lrs_client/models/purpose.py` & `cashfree_lrs_client-1.0.2/cashfree_lrs_client/models/purpose.py`

 * *Files identical despite different names*

### Comparing `cashfree_lrs_client-1.0.1/cashfree_lrs_client/models/setup_webhooks200_response.py` & `cashfree_lrs_client-1.0.2/cashfree_lrs_client/models/setup_webhooks200_response.py`

 * *Files identical despite different names*

### Comparing `cashfree_lrs_client-1.0.1/cashfree_lrs_client/models/setup_webhooks_request.py` & `cashfree_lrs_client-1.0.2/cashfree_lrs_client/models/setup_webhooks_request.py`

 * *Files identical despite different names*

### Comparing `cashfree_lrs_client-1.0.1/cashfree_lrs_client/models/success_message.py` & `cashfree_lrs_client-1.0.2/cashfree_lrs_client/models/success_message.py`

 * *Files identical despite different names*

### Comparing `cashfree_lrs_client-1.0.1/cashfree_lrs_client/paths/__init__.py` & `cashfree_lrs_client-1.0.2/cashfree_lrs_client/paths/__init__.py`

 * *Files identical despite different names*

### Comparing `cashfree_lrs_client-1.0.1/cashfree_lrs_client/paths/beneficiaries/post.py` & `cashfree_lrs_client-1.0.2/cashfree_lrs_client/paths/beneficiaries/post.py`

 * *Files identical despite different names*

### Comparing `cashfree_lrs_client-1.0.1/cashfree_lrs_client/paths/beneficiaries/post.pyi` & `cashfree_lrs_client-1.0.2/cashfree_lrs_client/paths/beneficiaries/post.pyi`

 * *Files identical despite different names*

### Comparing `cashfree_lrs_client-1.0.1/cashfree_lrs_client/paths/fx_rate_details/post.py` & `cashfree_lrs_client-1.0.2/cashfree_lrs_client/paths/fx_rate_details/post.py`

 * *Files identical despite different names*

### Comparing `cashfree_lrs_client-1.0.1/cashfree_lrs_client/paths/fx_rate_details/post.pyi` & `cashfree_lrs_client-1.0.2/cashfree_lrs_client/paths/fx_rate_details/post.pyi`

 * *Files identical despite different names*

### Comparing `cashfree_lrs_client-1.0.1/cashfree_lrs_client/paths/orders/post.py` & `cashfree_lrs_client-1.0.2/cashfree_lrs_client/paths/orders/post.py`

 * *Files identical despite different names*

### Comparing `cashfree_lrs_client-1.0.1/cashfree_lrs_client/paths/orders/post.pyi` & `cashfree_lrs_client-1.0.2/cashfree_lrs_client/paths/orders/post.pyi`

 * *Files identical despite different names*

### Comparing `cashfree_lrs_client-1.0.1/cashfree_lrs_client/paths/orders_documents_upload/post.py` & `cashfree_lrs_client-1.0.2/cashfree_lrs_client/paths/orders_documents_upload/post.py`

 * *Files identical despite different names*

### Comparing `cashfree_lrs_client-1.0.1/cashfree_lrs_client/paths/orders_documents_upload/post.pyi` & `cashfree_lrs_client-1.0.2/cashfree_lrs_client/paths/orders_documents_upload/post.pyi`

 * *Files identical despite different names*

### Comparing `cashfree_lrs_client-1.0.1/cashfree_lrs_client/paths/orders_order_id_documents_upload/post.py` & `cashfree_lrs_client-1.0.2/cashfree_lrs_client/paths/orders_order_id_documents_upload/post.py`

 * *Files identical despite different names*

### Comparing `cashfree_lrs_client-1.0.1/cashfree_lrs_client/paths/orders_order_id_documents_upload/post.pyi` & `cashfree_lrs_client-1.0.2/cashfree_lrs_client/paths/orders_order_id_documents_upload/post.pyi`

 * *Files identical despite different names*

### Comparing `cashfree_lrs_client-1.0.1/cashfree_lrs_client/paths/orders_order_id_process/post.py` & `cashfree_lrs_client-1.0.2/cashfree_lrs_client/paths/orders_order_id_process/post.py`

 * *Files identical despite different names*

### Comparing `cashfree_lrs_client-1.0.1/cashfree_lrs_client/paths/orders_order_id_process/post.pyi` & `cashfree_lrs_client-1.0.2/cashfree_lrs_client/paths/orders_order_id_process/post.pyi`

 * *Files identical despite different names*

### Comparing `cashfree_lrs_client-1.0.1/cashfree_lrs_client/paths/remitters/post.py` & `cashfree_lrs_client-1.0.2/cashfree_lrs_client/paths/remitters/post.py`

 * *Files identical despite different names*

### Comparing `cashfree_lrs_client-1.0.1/cashfree_lrs_client/paths/remitters/post.pyi` & `cashfree_lrs_client-1.0.2/cashfree_lrs_client/paths/remitters/post.pyi`

 * *Files identical despite different names*

### Comparing `cashfree_lrs_client-1.0.1/cashfree_lrs_client/paths/webhooks/post.py` & `cashfree_lrs_client-1.0.2/cashfree_lrs_client/paths/webhooks/post.py`

 * *Files identical despite different names*

### Comparing `cashfree_lrs_client-1.0.1/cashfree_lrs_client/paths/webhooks/post.pyi` & `cashfree_lrs_client-1.0.2/cashfree_lrs_client/paths/webhooks/post.pyi`

 * *Files identical despite different names*

### Comparing `cashfree_lrs_client-1.0.1/cashfree_lrs_client/rest.py` & `cashfree_lrs_client-1.0.2/cashfree_lrs_client/rest.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Cashfree LRS
 
     CashFree LRS APIs (v2)  # noqa: E501
 
-    The version of the OpenAPI document: 1.0.1
+    The version of the OpenAPI document: 1.0.2
     Contact: nextgenapi@cashfree.com
     Generated by: https://openapi-generator.tech
 """
 
 import logging
 import ssl
 from urllib.parse import urlencode
```

### Comparing `cashfree_lrs_client-1.0.1/cashfree_lrs_client/schemas.py` & `cashfree_lrs_client-1.0.2/cashfree_lrs_client/schemas.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Cashfree LRS
 
     CashFree LRS APIs (v2)  # noqa: E501
 
-    The version of the OpenAPI document: 1.0.1
+    The version of the OpenAPI document: 1.0.2
     Contact: nextgenapi@cashfree.com
     Generated by: https://openapi-generator.tech
 """
 
 from collections import defaultdict
 from datetime import date, datetime, timedelta  # noqa: F401
 import functools
```

### Comparing `cashfree_lrs_client-1.0.1/cashfree_lrs_client/test/test_create_beneficiary_request.py` & `cashfree_lrs_client-1.0.2/cashfree_lrs_client/test/test_create_beneficiary_request.py`

 * *Files identical despite different names*

### Comparing `cashfree_lrs_client-1.0.1/cashfree_lrs_client/test/test_create_order_request.py` & `cashfree_lrs_client-1.0.2/cashfree_lrs_client/test/test_create_order_request.py`

 * *Files identical despite different names*

### Comparing `cashfree_lrs_client-1.0.1/cashfree_lrs_client/test/test_create_order_response.py` & `cashfree_lrs_client-1.0.2/cashfree_lrs_client/test/test_create_order_response.py`

 * *Files identical despite different names*

### Comparing `cashfree_lrs_client-1.0.1/cashfree_lrs_client/test/test_create_remitter_request.py` & `cashfree_lrs_client-1.0.2/cashfree_lrs_client/test/test_create_remitter_request.py`

 * *Files identical despite different names*

### Comparing `cashfree_lrs_client-1.0.1/cashfree_lrs_client/test/test_currency.py` & `cashfree_lrs_client-1.0.2/cashfree_lrs_client/test/test_currency.py`

 * *Files identical despite different names*

### Comparing `cashfree_lrs_client-1.0.1/cashfree_lrs_client/test/test_error.py` & `cashfree_lrs_client-1.0.2/cashfree_lrs_client/test/test_error.py`

 * *Files identical despite different names*

### Comparing `cashfree_lrs_client-1.0.1/cashfree_lrs_client/test/test_fetch_forex_rate_request.py` & `cashfree_lrs_client-1.0.2/cashfree_lrs_client/test/test_fetch_forex_rate_request.py`

 * *Files identical despite different names*

### Comparing `cashfree_lrs_client-1.0.1/cashfree_lrs_client/test/test_lrs_api.py` & `cashfree_lrs_client-1.0.2/cashfree_lrs_client/test/test_lrs_api.py`

 * *Files identical despite different names*

### Comparing `cashfree_lrs_client-1.0.1/cashfree_lrs_client/test/test_purpose.py` & `cashfree_lrs_client-1.0.2/cashfree_lrs_client/test/test_purpose.py`

 * *Files identical despite different names*

### Comparing `cashfree_lrs_client-1.0.1/cashfree_lrs_client/test/test_setup_webhooks_request.py` & `cashfree_lrs_client-1.0.2/cashfree_lrs_client/test/test_setup_webhooks_request.py`

 * *Files identical despite different names*

### Comparing `cashfree_lrs_client-1.0.1/cashfree_lrs_client/test/test_success_message.py` & `cashfree_lrs_client-1.0.2/cashfree_lrs_client/test/test_success_message.py`

 * *Files identical despite different names*

### Comparing `cashfree_lrs_client-1.0.1/pyproject.toml` & `cashfree_lrs_client-1.0.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "cashfree_lrs_client"
-version = "1.0.1"
+version = "1.0.2"
 description = "Cashfree LRS"
 authors = ["Swadesh <dev@swadesh.co>", "CashFree <nextgenapi@cashfree.com>"]
 license = "NoLicense"
 readme = "README.md"
 repository = "https://github.com/SwadeshInc/cashfree_lrs_client"
 keywords = ["OpenAPI", "OpenAPI-Generator", "Cashfree LRS"]
```

### Comparing `cashfree_lrs_client-1.0.1/PKG-INFO` & `cashfree_lrs_client-1.0.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cashfree-lrs-client
-Version: 1.0.1
+Version: 1.0.2
 Summary: Cashfree LRS
 Home-page: https://github.com/SwadeshInc/cashfree_lrs_client
 License: NoLicense
 Keywords: OpenAPI,OpenAPI-Generator,Cashfree LRS
 Author: Swadesh
 Author-email: dev@swadesh.co
 Requires-Python: >=3.8.1,<4.0
@@ -21,15 +21,15 @@
 Description-Content-Type: text/markdown
 
 # cashfree-lrs-client
 CashFree LRS APIs (v2)
 
 This Python package is automatically generated by the [OpenAPI Generator](https://openapi-generator.tech) project:
 
-- API version: 1.0.1
+- API version: 1.0.2
 - Package version: 1.0.0
 - Build package: org.openapitools.codegen.languages.PythonClientCodegen
 For more information, please visit [https://docs.cashfree.com](https://docs.cashfree.com)
 
 ## Requirements.
 
 Python &gt;&#x3D;3.7
@@ -232,14 +232,15 @@
 *LrsApi* | [**fetch_forex_rate**](docs/apis/tags/LrsApi.md#fetch_forex_rate) | **post** /fx-rate/details | Fetch FX Rate
 *LrsApi* | [**process_order**](docs/apis/tags/LrsApi.md#process_order) | **post** /orders/{order_id}/process | Process Order
 *LrsApi* | [**setup_webhooks**](docs/apis/tags/LrsApi.md#setup_webhooks) | **post** /webhooks | Setup Webhooks
 *LrsApi* | [**upload_documents**](docs/apis/tags/LrsApi.md#upload_documents) | **post** /orders/{order_id}/documents/upload | Upload Documents
 
 ## Documentation For Models
 
+ - [Amount](docs/models/Amount.md)
  - [CreateBeneficiaryRequest](docs/models/CreateBeneficiaryRequest.md)
  - [CreateOrderRequest](docs/models/CreateOrderRequest.md)
  - [CreateOrderResponse](docs/models/CreateOrderResponse.md)
  - [CreateRemitterRequest](docs/models/CreateRemitterRequest.md)
  - [Currency](docs/models/Currency.md)
  - [Error](docs/models/Error.md)
  - [FetchForexRateRequest](docs/models/FetchForexRateRequest.md)
```

