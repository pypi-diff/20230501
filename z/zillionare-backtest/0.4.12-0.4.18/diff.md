# Comparing `tmp/zillionare-backtest-0.4.12.tar.gz` & `tmp/zillionare_backtest-0.4.18.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "zillionare-backtest-0.4.12.tar", max compression
+gzip compressed data, was "zillionare_backtest-0.4.18.tar", max compression
```

## Comparing `zillionare-backtest-0.4.12.tar` & `zillionare_backtest-0.4.18.tar`

### file list

```diff
@@ -1,46 +1,45 @@
--rw-r--r--   0        0        0     1068 2022-09-03 11:53:20.705929 zillionare-backtest-0.4.12/LICENSE
--rw-r--r--   0        0        0     6660 2022-09-03 11:53:20.705929 zillionare-backtest-0.4.12/README.md
--rw-r--r--   0        0        0      114 2022-09-03 11:53:20.705929 zillionare-backtest-0.4.12/backtest/__init__.py
--rw-r--r--   0        0        0     2160 2022-09-03 11:53:20.705929 zillionare-backtest-0.4.12/backtest/app.py
--rw-r--r--   0        0        0     2924 2022-09-03 11:53:20.709930 zillionare-backtest-0.4.12/backtest/cli.py
--rw-r--r--   0        0        0        0 2022-09-03 11:53:20.709930 zillionare-backtest-0.4.12/backtest/common/__init__.py
--rw-r--r--   0        0        0     2048 2022-09-03 11:53:20.709930 zillionare-backtest-0.4.12/backtest/common/errors.py
--rw-r--r--   0        0        0     6281 2022-09-03 11:53:20.709930 zillionare-backtest-0.4.12/backtest/common/helper.py
--rw-r--r--   0        0        0     1077 2022-09-03 11:53:20.709930 zillionare-backtest-0.4.12/backtest/config/__init__.py
--rw-r--r--   0        0        0     1796 2022-09-03 11:53:20.709930 zillionare-backtest-0.4.12/backtest/config/defaults.yaml
--rw-r--r--   0        0        0      862 2022-09-03 11:53:20.709930 zillionare-backtest-0.4.12/backtest/config/dev.yaml
--rw-r--r--   0        0        0     1165 2022-09-03 11:53:20.709930 zillionare-backtest-0.4.12/backtest/config/schema.py
--rw-r--r--   0        0        0      501 2022-09-03 11:53:20.709930 zillionare-backtest-0.4.12/backtest/feed/__init__.py
--rw-r--r--   0        0        0     3423 2022-09-03 11:53:20.709930 zillionare-backtest-0.4.12/backtest/feed/basefeed.py
--rw-r--r--   0        0        0     5422 2022-09-03 11:53:20.709930 zillionare-backtest-0.4.12/backtest/feed/zillionarefeed.py
--rw-r--r--   0        0        0       62 2022-09-03 11:53:20.709930 zillionare-backtest-0.4.12/backtest/trade/__init__.py
--rw-r--r--   0        0        0    47089 2022-09-03 11:53:20.709930 zillionare-backtest-0.4.12/backtest/trade/broker.py
--rw-r--r--   0        0        0     2989 2022-09-03 11:53:20.709930 zillionare-backtest-0.4.12/backtest/trade/datatypes.py
--rw-r--r--   0        0        0     3911 2022-09-03 11:53:20.709930 zillionare-backtest-0.4.12/backtest/trade/trade.py
--rw-r--r--   0        0        0      910 2022-09-03 11:53:20.709930 zillionare-backtest-0.4.12/backtest/trade/transaction.py
--rw-r--r--   0        0        0       50 2022-09-03 11:53:20.709930 zillionare-backtest-0.4.12/backtest/web/__init__.py
--rw-r--r--   0        0        0     4115 2022-09-03 11:53:20.709930 zillionare-backtest-0.4.12/backtest/web/accounts.py
--rw-r--r--   0        0        0    13822 2022-09-03 11:53:20.709930 zillionare-backtest-0.4.12/backtest/web/interfaces.py
--rw-r--r--   0        0        0     3027 2022-09-03 11:53:20.717930 zillionare-backtest-0.4.12/pyproject.toml
--rw-r--r--   0        0        0     8067 2022-09-03 11:53:20.717930 zillionare-backtest-0.4.12/tests/__init__.py
--rw-r--r--   0        0        0        0 2022-09-03 11:53:20.717930 zillionare-backtest-0.4.12/tests/common/__init__.py
--rw-r--r--   0        0        0     1844 2022-09-03 11:53:20.717930 zillionare-backtest-0.4.12/tests/common/test_helper.py
--rw-r--r--   0        0        0     3289 2022-09-03 11:53:20.717930 zillionare-backtest-0.4.12/tests/data/bars_1d.pkl
--rw-r--r--   0        0        0   613076 2022-09-03 11:53:20.721930 zillionare-backtest-0.4.12/tests/data/bars_1m.pkl
--rw-r--r--   0        0        0      700 2022-09-03 11:53:20.721930 zillionare-backtest-0.4.12/tests/data/hljh_1d.csv
--rw-r--r--   0        0        0   163810 2022-09-03 11:53:20.721930 zillionare-backtest-0.4.12/tests/data/hljh_1m.csv
--rw-r--r--   0        0        0     1073 2022-09-03 11:53:20.721930 zillionare-backtest-0.4.12/tests/data/limits.csv
--rw-r--r--   0        0        0      438 2022-09-03 11:53:20.721930 zillionare-backtest-0.4.12/tests/data/readme.md
--rw-r--r--   0        0        0      665 2022-09-03 11:53:20.721930 zillionare-backtest-0.4.12/tests/data/tyst_1d.csv
--rw-r--r--   0        0        0   156635 2022-09-03 11:53:20.725930 zillionare-backtest-0.4.12/tests/data/tyst_1m.csv
--rw-r--r--   0        0        0    11225 2022-09-03 11:53:20.725930 zillionare-backtest-0.4.12/tests/data/validation.xlsx
--rw-r--r--   0        0        0        0 2022-09-03 11:53:20.725930 zillionare-backtest-0.4.12/tests/feed/__init__.py
--rw-r--r--   0        0        0     8414 2022-09-03 11:53:20.725930 zillionare-backtest-0.4.12/tests/feed/test_zillionarefeed.py
--rw-r--r--   0        0        0      840 2022-09-03 11:53:20.725930 zillionare-backtest-0.4.12/tests/test_app.py
--rw-r--r--   0        0        0      650 2022-09-03 11:53:20.725930 zillionare-backtest-0.4.12/tests/test_cli.py
--rw-r--r--   0        0        0        0 2022-09-03 11:53:20.725930 zillionare-backtest-0.4.12/tests/trade/__init__.py
--rw-r--r--   0        0        0    38689 2022-09-03 11:53:20.725930 zillionare-backtest-0.4.12/tests/trade/test_broker.py
--rw-r--r--   0        0        0        0 2022-09-03 11:53:20.725930 zillionare-backtest-0.4.12/tests/web/__init__.py
--rw-r--r--   0        0        0    19287 2022-09-03 11:53:20.725930 zillionare-backtest-0.4.12/tests/web/test_interfaces.py
--rw-r--r--   0        0        0     8836 1970-01-01 00:00:00.000000 zillionare-backtest-0.4.12/setup.py
--rw-r--r--   0        0        0     9218 1970-01-01 00:00:00.000000 zillionare-backtest-0.4.12/PKG-INFO
+-rw-r--r--   0        0        0     1068 2023-02-06 14:55:37.972351 zillionare_backtest-0.4.18/LICENSE
+-rw-r--r--   0        0        0     7504 2023-04-30 02:28:40.884883 zillionare_backtest-0.4.18/README.md
+-rw-r--r--   0        0        0      114 2023-02-06 14:55:37.972351 zillionare_backtest-0.4.18/backtest/__init__.py
+-rw-r--r--   0        0        0     2160 2023-02-14 02:11:34.858631 zillionare_backtest-0.4.18/backtest/app.py
+-rw-r--r--   0        0        0     2924 2023-02-06 14:55:37.972351 zillionare_backtest-0.4.18/backtest/cli.py
+-rw-r--r--   0        0        0        0 2023-02-06 14:55:37.972351 zillionare_backtest-0.4.18/backtest/common/__init__.py
+-rw-r--r--   0        0        0     2180 2023-02-06 14:55:37.972351 zillionare_backtest-0.4.18/backtest/common/errors.py
+-rw-r--r--   0        0        0     6281 2023-02-06 14:55:37.972351 zillionare_backtest-0.4.18/backtest/common/helper.py
+-rw-r--r--   0        0        0     1077 2023-02-06 14:55:37.972351 zillionare_backtest-0.4.18/backtest/config/__init__.py
+-rw-r--r--   0        0        0     1109 2023-05-01 07:03:53.365967 zillionare_backtest-0.4.18/backtest/config/defaults.yaml
+-rw-r--r--   0        0        0      862 2023-05-01 08:43:15.780342 zillionare_backtest-0.4.18/backtest/config/dev.yaml
+-rw-r--r--   0        0        0     1165 2023-02-06 14:55:37.972351 zillionare_backtest-0.4.18/backtest/config/schema.py
+-rw-r--r--   0        0        0      501 2023-02-06 14:55:37.972351 zillionare_backtest-0.4.18/backtest/feed/__init__.py
+-rw-r--r--   0        0        0     3423 2023-02-06 14:55:37.972351 zillionare_backtest-0.4.18/backtest/feed/basefeed.py
+-rw-r--r--   0        0        0     5422 2023-02-06 14:55:37.972351 zillionare_backtest-0.4.18/backtest/feed/zillionarefeed.py
+-rw-r--r--   0        0        0       62 2023-02-06 14:55:37.972351 zillionare_backtest-0.4.18/backtest/trade/__init__.py
+-rw-r--r--   0        0        0    48445 2023-05-01 09:23:29.569986 zillionare_backtest-0.4.18/backtest/trade/broker.py
+-rw-r--r--   0        0        0     2989 2023-02-06 14:55:37.976351 zillionare_backtest-0.4.18/backtest/trade/datatypes.py
+-rw-r--r--   0        0        0     3999 2023-02-06 14:55:37.976351 zillionare_backtest-0.4.18/backtest/trade/trade.py
+-rw-r--r--   0        0        0     1100 2023-04-29 08:15:19.279077 zillionare_backtest-0.4.18/backtest/trade/transaction.py
+-rw-r--r--   0        0        0       50 2023-02-06 14:55:37.976351 zillionare_backtest-0.4.18/backtest/web/__init__.py
+-rw-r--r--   0        0        0     4115 2023-02-06 14:55:37.976351 zillionare_backtest-0.4.18/backtest/web/accounts.py
+-rw-r--r--   0        0        0    13822 2023-04-30 02:15:22.554201 zillionare_backtest-0.4.18/backtest/web/interfaces.py
+-rw-r--r--   0        0        0     3027 2023-05-01 09:42:52.723800 zillionare_backtest-0.4.18/pyproject.toml
+-rw-r--r--   0        0        0     8067 2023-02-06 14:55:38.156353 zillionare_backtest-0.4.18/tests/__init__.py
+-rw-r--r--   0        0        0        0 2023-02-06 14:55:38.156353 zillionare_backtest-0.4.18/tests/common/__init__.py
+-rw-r--r--   0        0        0     1844 2023-02-06 14:55:38.156353 zillionare_backtest-0.4.18/tests/common/test_helper.py
+-rw-r--r--   0        0        0     3289 2023-02-06 14:55:38.156353 zillionare_backtest-0.4.18/tests/data/bars_1d.pkl
+-rw-r--r--   0        0        0   613076 2023-02-06 14:55:38.164353 zillionare_backtest-0.4.18/tests/data/bars_1m.pkl
+-rw-r--r--   0        0        0      700 2023-04-29 14:40:00.305575 zillionare_backtest-0.4.18/tests/data/hljh_1d.csv
+-rw-r--r--   0        0        0   163810 2023-04-29 14:37:20.922040 zillionare_backtest-0.4.18/tests/data/hljh_1m.csv
+-rw-r--r--   0        0        0     1073 2023-02-06 14:55:38.164353 zillionare_backtest-0.4.18/tests/data/limits.csv
+-rw-r--r--   0        0        0      438 2023-02-06 14:55:38.164353 zillionare_backtest-0.4.18/tests/data/readme.md
+-rw-r--r--   0        0        0      665 2023-02-06 14:55:38.164353 zillionare_backtest-0.4.18/tests/data/tyst_1d.csv
+-rw-r--r--   0        0        0   156635 2023-02-06 14:55:38.168353 zillionare_backtest-0.4.18/tests/data/tyst_1m.csv
+-rw-r--r--   0        0        0    11225 2023-02-06 14:55:38.168353 zillionare_backtest-0.4.18/tests/data/validation.xlsx
+-rw-r--r--   0        0        0        0 2023-02-06 14:55:38.168353 zillionare_backtest-0.4.18/tests/feed/__init__.py
+-rw-r--r--   0        0        0     8414 2023-02-06 14:55:38.168353 zillionare_backtest-0.4.18/tests/feed/test_zillionarefeed.py
+-rw-r--r--   0        0        0      840 2023-02-06 14:55:38.168353 zillionare_backtest-0.4.18/tests/test_app.py
+-rw-r--r--   0        0        0      650 2023-02-06 14:55:38.168353 zillionare_backtest-0.4.18/tests/test_cli.py
+-rw-r--r--   0        0        0        0 2023-02-06 14:55:38.168353 zillionare_backtest-0.4.18/tests/trade/__init__.py
+-rw-r--r--   0        0        0    39691 2023-05-01 09:07:39.605377 zillionare_backtest-0.4.18/tests/trade/test_broker.py
+-rw-r--r--   0        0        0        0 2023-02-06 14:55:38.172353 zillionare_backtest-0.4.18/tests/web/__init__.py
+-rw-r--r--   0        0        0    19344 2023-05-01 09:28:17.262527 zillionare_backtest-0.4.18/tests/web/test_interfaces.py
+-rw-r--r--   0        0        0    10047 1970-01-01 00:00:00.000000 zillionare_backtest-0.4.18/PKG-INFO
```

### Comparing `zillionare-backtest-0.4.12/LICENSE` & `zillionare_backtest-0.4.18/LICENSE`

 * *Files identical despite different names*

### Comparing `zillionare-backtest-0.4.12/README.md` & `zillionare_backtest-0.4.18/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -147,271 +147,323 @@
 00000920: 9a84 e683 85e5 86b5 e4b8 8bef bc8c e682  ................
 00000930: a8e5 8faf e4bb a5e5 9ca8 e99a 8fe5 908e  ................
 00000940: e980 9ae8 bf87 5b64 656c 6574 655f 6163  ......[delete_ac
 00000950: 636f 756e 7473 5d5b 6261 636b 7465 7374  counts][backtest
 00000960: 2e77 6562 2e69 6e74 6572 6661 6365 732e  .web.interfaces.
 00000970: 6465 6c65 7465 5f61 6363 6f75 6e74 735d  delete_accounts]
 00000980: e69d a5e5 88a0 e999 a4e8 b4a6 e688 b7e3  ................
-00000990: 8082 0a0a 2323 20e4 baa4 e698 93e6 92ae  ....## .........
-000009a0: e590 880a 0ae6 82a8 e58f afe4 bba5 e980  ................
-000009b0: 9ae8 bf87 5b62 7579 5d5b 6261 636b 7465  ....[buy][backte
-000009c0: 7374 2e77 6562 2e69 6e74 6572 6661 6365  st.web.interface
-000009d0: 732e 6275 795d 2c20 5b6d 6172 6b65 745f  s.buy], [market_
-000009e0: 6275 795d 5b62 6163 6b74 6573 742e 7765  buy][backtest.we
-000009f0: 622e 696e 7465 7266 6163 6573 2e6d 6172  b.interfaces.mar
-00000a00: 6b65 745f 6275 795d 2c20 5b73 656c 6c5d  ket_buy], [sell]
-00000a10: 5b62 6163 6b74 6573 742e 7765 622e 696e  [backtest.web.in
-00000a20: 7465 7266 6163 6573 2e73 656c 6c5d 2c20  terfaces.sell], 
-00000a30: 5b6d 6172 6b65 745f 7365 6c6c 5d5b 6261  [market_sell][ba
-00000a40: 636b 7465 7374 2e77 6562 2e69 6e74 6572  cktest.web.inter
-00000a50: 6661 6365 732e 6d61 726b 6574 5f73 656c  faces.market_sel
-00000a60: 6c5d e592 8c5b 7365 6c6c 5f70 6572 6365  l]...[sell_perce
-00000a70: 6e74 5d5b 6261 636b 7465 7374 2e77 6562  nt][backtest.web
-00000a80: 2e69 6e74 6572 6661 6365 732e 7365 6c6c  .interfaces.sell
-00000a90: 5f70 6572 6365 6e74 5de6 9da5 e8bf 9be8  _percent].......
-00000aa0: a18c e4ba a4e6 9893 e380 820a 0a23 2320  .............## 
-00000ab0: e78a b6e6 8081 e8b7 9fe8 b8aa 0a0a e682  ................
-00000ac0: a8e5 8faf e4bb a5e9 809a e8bf 875b 696e  .............[in
-00000ad0: 666f 5d5b 6261 636b 7465 7374 2e77 6562  fo][backtest.web
-00000ae0: 2e69 6e74 6572 6661 6365 732e 696e 666f  .interfaces.info
-00000af0: 5de6 9da5 e69f a5e7 9c8b e8b4 a6e6 88b7  ]...............
-00000b00: e79a 84e5 9fba e69c ace4 bfa1 e681 afef  ................
-00000b10: bc8c e6af 94e5 a682 e5bd 93e5 898d e680  ................
-00000b20: bbe8 b584 e4ba a7e3 8081 e68c 81e4 bb93  ................
-00000b30: e380 81e6 9cac e987 91e3 8081 e79b 88e5  ................
-00000b40: 88a9 e7ad 89e3 8082 e682 a8e8 bf98 e58f  ................
-00000b50: afe4 bba5 e980 9ae8 bf87 5b70 6f73 6974  ..........[posit
-00000b60: 696f 6e73 5d5b 6261 636b 7465 7374 2e77  ions][backtest.w
-00000b70: 6562 2e69 6e74 6572 6661 6365 732e 706f  eb.interfaces.po
-00000b80: 7369 7469 6f6e 735d e380 815b 6269 6c6c  sitions]...[bill
-00000b90: 735d 5b62 6163 6b74 6573 742e 7765 622e  s][backtest.web.
-00000ba0: 696e 7465 7266 6163 6573 2e62 696c 6c73  interfaces.bills
-00000bb0: 5de6 9da5 e69f a5e7 9c8b e8b4 a6e6 88b7  ]...............
-00000bc0: e79a 84e6 8c81 e4bb 93e3 8081 e4ba a4e6  ................
-00000bd0: 9893 e58e 86e5 8fb2 e8ae b0e5 bd95 0a23  ...............#
-00000be0: 2320 e7ad 96e7 95a5 e8af 84e4 bcb0 0a0a  # ..............
-00000bf0: 5b6d 6574 7269 6373 5d5b 6261 636b 7465  [metrics][backte
-00000c00: 7374 2e77 6562 2e69 6e74 6572 6661 6365  st.web.interface
-00000c10: 732e 6d65 7472 6963 735d e696 b9e6 b395  s.metrics]......
-00000c20: e5b0 86e8 bf94 e59b 9ee7 ad96 e795 a5e7  ................
-00000c30: 9a84 e590 84e9 a1b9 e68c 87e6 a087 efbc  ................
-00000c40: 8ce6 af94 e5a6 8273 6861 7270 652c 2073  .......sharpe, s
-00000c50: 6f72 7469 6e6f 2c20 6361 6c6d 6172 2c20  ortino, calmar, 
-00000c60: 7769 6e20 7261 7465 2c20 6d61 7820 6472  win rate, max dr
-00000c70: 6177 646f 776e e7ad 89e3 8082 e682 a8e8  awdown..........
-00000c80: bf98 e58f afe4 bba5 e4bc a0e5 85a5 e4b8  ................
-00000c90: 80e4 b8aa e58f 82e8 8083 e6a0 87e7 9a84  ................
-00000ca0: efbc 8c62 6163 6b74 6573 74e5 b086 e5af  ...backtest.....
-00000cb0: b9e5 8f82 e880 83e6 a087 e79a 84e4 b99f  ................
-00000cc0: e590 8ce6 a0b7 e8ae a1e7 ae97 e4b8 8ae8  ................
-00000cd0: bfb0 e68c 87e6 a087 e380 820a 0a23 20e5  .............# .
-00000ce0: 85b3 e994 aee6 a682 e5bf b50a 0a23 2320  .............## 
-00000cf0: e5a4 8de6 9d83 e5a4 84e7 9086 0ae6 82a8  ................
-00000d00: e79a 84e7 ad96 e795 a5e5 9ca8 e58f 91e5  ................
-00000d10: 87ba e4b9 b0e5 8d96 e4bf a1e5 8fb7 e697  ................
-00000d20: b6ef bc8c e5ba 94e8 afa5 e4bd bfe7 94a8  ................
-00000d30: e4b8 8e60 6f72 6465 725f 7469 6d65 60e4  ...`order_time`.
-00000d40: b880 e887 b4e7 9a84 e78e b0e4 bbb7 efbc  ................
-00000d50: 8ce8 808c e4b8 8de6 98af e4bb bbe4 bd95  ................
-00000d60: e5a4 8de6 9d83 e4bb b7e3 8082 e5a6 82e6  ................
-00000d70: 9e9c e682 a8e7 9a84 e68c 81e4 bb93 e59c  ................
-00000d80: a8e6 8c81 e69c 89e6 9c9f e997 b4ef bc8c  ................
-00000d90: e58f 91e7 949f e4ba 86e5 8886 e7ba a2e9  ................
-00000da0: 8081 e882 a1ef bc8c e59b 9ee6 b58b e69c  ................
-00000db0: 8de5 8aa1 e599 a8e4 bc9a e887 aae5 8aa8  ................
-00000dc0: e5b0 86e5 8886 e7ba a2e9 8081 e882 a1e8  ................
-00000dd0: bdac e68d a2e6 8890 e882 a1e6 95b0 e58a  ................
-00000de0: a0e5 88b0 e682 a8e7 9a84 e68c 81e4 bb93  ................
-00000df0: e4b8 ade3 8082 e5bd 93e6 82a8 e69c 80e7  ................
-00000e00: bb88 e6b8 85e7 a9ba e68c 81e4 bb93 e697  ................
-00000e10: b6ef bc8c e58f afe4 bba5 e980 9ae8 bf87  ................
-00000e20: 6062 696c 6c73 60e6 8ea5 e58f a3e6 9fa5  `bills`.........
-00000e30: e8af a2e5 88b0 e588 86e7 baa2 e980 81e8  ................
-00000e40: 82a1 e79a 84e6 8890 e4ba a4e6 8385 e586  ................
-00000e50: b5ef bc88 e8ae b0e5 bd95 e4b8 ba58 4458  .............XDX
-00000e60: 52e7 b1bb e59e 8be7 9a84 e5a7 94e6 8998  R...............
-00000e70: efbc 89e3 8082 0a0a 2323 20e6 92ae e590  ........## .....
-00000e80: 88e6 9cba e588 b60a e59c a8e6 92ae e590  ................
-00000e90: 88e6 97b6 efbc 8c62 6163 6b74 6573 74e9  .......backtest.
-00000ea0: a696 e585 88e4 bb8e 6461 7461 2066 6565  ........data fee
-00000eb0: 6465 72e4 b8ad e88e b7e5 8f96 606f 7264  der.........`ord
-00000ec0: 6572 5f74 696d 6560 e4bb a5e5 908e efbc  er_time`........
-00000ed0: 88e5 90ab efbc 89e7 9a84 e8a1 8ce6 8385  ................
-00000ee0: e695 b0e6 8dae e380 82e6 8ea5 e4b8 8be6  ................
-00000ef0: 9da5 e58e bbe6 8e89 e5a4 84e5 9ca8 e6b6  ................
-00000f00: a8e8 b78c e581 9ce4 b8ad e79a 84e9 82a3  ................
-00000f10: e4ba 9b62 6172 efbc 88e5 a682 e69e 9ce6  ...bar..........
-00000f20: 98af e5a7 94e4 b9b0 efbc 8ce5 8899 e58e  ................
-00000f30: bbe6 8e89 e5b7 b2e5 a484 e59c a8e6 b6a8  ................
-00000f40: e581 9ce6 9c9f e997 b4e7 9a84 6261 72ef  ............bar.
-00000f50: bc8c e58f 8de4 b98b e4ba a6e7 84b6 efbc  ................
-00000f60: 89e3 8082 e59c a8e5 89a9 e4b8 8be7 9a84  ................
-00000f70: 6261 72e4 b8ad efbc 8c62 6163 6b74 6573  bar......backtes
-00000f80: 74e4 bc9a e980 89e6 8ba9 e4bb b7e6 a0bc  t...............
-00000f90: e4bd 8ee4 ba8e e5a7 94e6 8998 e4bb b7e7  ................
-00000fa0: 9a84 e982 a3e4 ba9b 6261 72ef bc88 e5a6  ........bar.....
-00000fb0: 82e6 9e9c e698 afe5 a794 e58d 96ef bc8c  ................
-00000fc0: e588 99e9 8089 e68b a9e4 bbb7 e6a0 bce9  ................
-00000fd0: ab98 e4ba 8ee5 a794 e689 98e4 bbb7 e79a  ................
-00000fe0: 84e9 82a3 e4ba 9b62 6172 efbc 892c e4be  .......bar...,..
-00000ff0: 9de9 a1ba e5ba 8fe5 8cb9 e985 8de5 a794  ................
-00001000: e689 98e9 878f efbc 8ce7 9bb4 e588 b0e5  ................
-00001010: a794 e689 98e9 878f e585 a8e9 83a8 e8a2  ................
-00001020: abe5 8cb9 e985 8de4 b8ba e6ad a2e3 8082  ................
-00001030: e69c 80e5 908e efbc 8c62 6163 6b74 6573  .........backtes
-00001040: 74e5 b086 e58c b9e9 858d e588 b0e7 9a84  t...............
-00001050: 6261 72e7 9a84 e987 8fe5 928c e4bb b7e6  bar.............
-00001060: a0bc e8bf 9be8 a18c e58a a0e6 9d83 e5b9  ................
-00001070: b3e5 9d87 efbc 8ce5 be97 e588 b0e6 8890  ................
-00001080: e4ba a4e5 9d87 e4bb b7e3 8082 0a0a e5bd  ................
-00001090: 9362 6163 6b74 6573 74e4 bdbf e794 a87a  .backtest......z
-000010a0: 696c 6c69 6f6e 6172 652d 6665 6564 e69d  illionare-feed..
-000010b0: a5e6 8f90 e4be 9be6 92ae e590 88e6 95b0  ................
-000010c0: e68d aee6 97b6 efbc 8ce7 94b1 e4ba 8ee7  ................
-000010d0: bcba e5b0 91e7 9b98 e58f a3e6 95b0 e68d  ................
-000010e0: aeef bc8c 7a69 6c6c 696f 6e61 7265 2d66  ....zillionare-f
-000010f0: 6565 64e4 bdbf e794 a8e5 8886 e992 9fe7  eed.............
-00001100: baa7 e8a1 8ce6 8385 e695 b0e6 8dae e4b8  ................
-00001110: ade7 9a84 6063 6c6f 7365 60e4 bbb7 e6a0  ....`close`.....
-00001120: bce5 928c 6076 6f6c 756d 6560 e69d a5e8  ....`volume`....
-00001130: bf9b e8a1 8ce6 92ae e590 88e3 8082 e59b  ................
-00001140: a0e6 ada4 efbc 8ce5 8faf e883 bde5 87ba  ................
-00001150: e78e b0e6 9f90 e4b8 80e5 8886 e992 9fe7  ................
-00001160: 9a84 e69c 80e9 ab98 e4bb b7e6 8896 e880  ................
-00001170: 85e6 9c80 e4bd 8ee4 bbb7 e58f afe8 83bd  ................
-00001180: e6bb a1e8 b6b3 e8bf 87e6 82a8 e79a 84e5  ................
-00001190: a794 e689 98e4 bbb7 e8a6 81e6 b182 efbc  ................
-000011a0: 8ce4 bd86 6261 636b 7465 7374 e5b9 b6e6  ....backtest....
-000011b0: 9caa e688 90e4 baa4 e692 aee5 9088 e79a  ................
-000011c0: 84e6 8385 e586 b5e3 8082 e688 91e4 bbac  ................
-000011d0: e8bf 99e6 a0b7 e8ae bee8 aea1 efbc 8ce4  ................
-000011e0: b8bb e8a6 81e8 8083 e899 91e5 88b0 e5bd  ................
-000011f0: 93e8 82a1 e4bb b7e8 bebe e588 b0e6 9c80  ................
-00001200: e9ab 98e6 8896 e880 85e6 9c80 e4bd 8ee7  ................
-00001210: 82b9 e697 b6ef bc8c e5bd 93e6 97b6 e79a  ................
-00001220: 84e6 8890 e4ba a4e9 878f e4b8 8de8 b6b3  ................
-00001230: e4bb a5e6 bba1 e8b6 b3e5 a794 e689 98e9  ................
-00001240: 878f e380 82e7 8eb0 e59c a862 6163 6b74  ...........backt
-00001250: 6573 74e7 9a84 e8ae bee8 aea1 efbc 8ce5  est.............
-00001260: 8faf e883 bde7 ad96 e795 a5e7 9a84 e9b2  ................
-00001270: 81e6 a392 e680 a7e6 9bb4 e5a5 bde3 8082  ................
-00001280: 0a0a e4bd 9ce4 b8ba e4b8 80e4 b8aa e4be  ................
-00001290: 8be5 a496 efbc 8ce5 a682 e69e 9ce5 a794  ................
-000012a0: e689 98e6 97b6 e79a 8460 6f72 6465 725f  .........`order_
-000012b0: 7469 6d65 60e4 b8ba 393a 3331 e588 86e4  time`...9:31....
-000012c0: b98b e589 8def bc8c 6261 636b 7465 7374  ........backtest
-000012d0: e5b0 86e4 bc9a e4bd bfe7 94a8 393a 3331  ............9:31
-000012e0: e588 86e9 929f e7ba bfe7 9a84 e5bc 80e7  ................
-000012f0: 9b98 e4bb b7ef bc8c e880 8ce4 b88d e698  ................
-00001300: af39 3a33 31e5 8886 e79a 84e6 94b6 e79b  .9:31...........
-00001310: 98e4 bbb7 e69d a5e8 bf9b e8a1 8ce6 92ae  ................
-00001320: e590 88ef bc8c e4bb a5e6 bba1 e8b6 b3e9  ................
-00001330: 83a8 e588 86e7 ad96 e795 a5e9 9c80 e8a6  ................
-00001340: 81e4 bba5 2a2a e6ac a1e6 97a5 e5bc 80e7  ....**..........
-00001350: 9b98 e4bb b72a 2ae4 b9b0 e585 a5e7 9a84  .....**.........
-00001360: e99c 80e6 b182 e380 820a 0ae5 8fa6 e5a4  ................
-00001370: 96ef bc8c e682 a8e4 b99f e5ba 94e8 afa5  ................
-00001380: e6b3 a8e6 848f e588 b0ef bc8c 7a69 6c6c  ............zill
-00001390: 696f 6e61 7265 2d66 6565 64e4 bdbf e794  ionare-feed.....
-000013a0: a8e5 8886 e992 9fe7 babf e69d a5e6 9bbf  ................
-000013b0: e4bb a3e4 ba86 e79b 98e5 8fa3 e695 b0e6  ................
-000013c0: 8dae efbc 8ce5 b0bd e7ae a1e5 9ca8 e7bb  ................
-000013d0: 9de5 a4a7 e5a4 9ae6 95b0 e683 85e5 bda2  ................
-000013e0: e4b8 8bef bc8c e8bf 99e6 a0b7 e581 9ae4  ................
-000013f0: b88d e4bc 9ae6 9c89 e4bb 80e4 b988 e5bd  ................
-00001400: b1e5 938d efbc 8ce4 bd86 e4b8 a4e8 8085  ................
-00001410: e6af 95e7 ab9f e698 afe4 b88d e590 8ce7  ................
-00001420: 9a84 e380 82e4 b880 e888 ace6 9da5 e8af  ................
-00001430: b4ef bc8c e688 90e4 baa4 e987 8fe8 82af  ................
-00001440: e5ae 9ae5 b08f e4ba 8ee7 9b98 e58f a3e7  ................
-00001450: 9a84 e5a7 94e4 b9b0 e5a7 94e5 8d96 e987  ................
-00001460: 8fe3 8082 e59b a0e6 ada4 efbc 8ce5 9ca8  ................
-00001470: e59b 9ee6 b58b e4b8 ade5 87ba e78e b0e4  ................
-00001480: b9b0 e58d 96e5 a794 e689 98e9 878f e4b8  ................
-00001490: 8de8 b6b3 e79a 84e6 8385 e586 b5e6 97b6  ................
-000014a0: efbc 8ce5 afb9 e5ba 94e7 9a84 e5ae 9ee7  ................
-000014b0: 9b98 e588 99e4 b88d e4b8 80e5 ae9a e587  ................
-000014c0: bae7 8eb0 e380 82e5 9ca8 e8bf 99e7 a78d  ................
-000014d0: e683 85e5 86b5 e4b8 8bef bc8c e58f afe4  ................
-000014e0: bba5 e980 82e5 bd93 e8b0 83e4 bd8e e7ad  ................
-000014f0: 96e7 95a5 e79a 84e6 9cac e987 91e8 aebe  ................
-00001500: e7bd aee3 8082 e58f a6e5 a496 e4b8 80e4  ................
-00001510: b8aa e5b7 aee5 bc82 e698 afef bc8c e588  ................
-00001520: 86e9 929f e688 90e4 baa4 e4bb b7e5 bf85  ................
-00001530: e784 b6e4 b88d e7ad 89e5 908c e4ba 8ee7  ................
-00001540: 9b98 e58f a3e6 8890 e4ba a4e4 bbb7 efbc  ................
-00001550: 8ce5 9ba0 e6ad a4e4 bc9a e5bc 95e5 85a5  ................
-00001560: e4b8 80e5 ae9a e79a 84e8 afaf e5b7 aee3  ................
-00001570: 8082 e4b8 8de8 bf87 e995 bfe6 9c9f e69d  ................
-00001580: a5e7 9c8b efbc 8ce8 bf99 e7a7 8de8 afaf  ................
-00001590: e5b7 aee5 ba94 e8af a5e6 98af e99b b6e5  ................
-000015a0: 9d87 e580 bce7 9a84 efbc 8ce5 9ba0 e6ad  ................
-000015b0: a4e5 afb9 e7bb 9de5 a4a7 e5a4 9ae6 95b0  ................
-000015c0: e7ad 96e7 95a5 e4b8 8de4 bc9a e4ba a7e7  ................
-000015d0: 949f e5ae 9ee8 b4a8 e5bd b1e5 938d e380  ................
-000015e0: 820a 0a21 2121 696e 666f 0a20 2020 20e4  ...!!!info.    .
-000015f0: ba86 e8a7 a362 6163 6b74 6573 74e7 9a84  .....backtest...
-00001600: e692 aee5 9088 e69c bae5 88b6 e590 8eef  ................
-00001610: bc8c e682 a8e5 ba94 e8af a5e5 b7b2 e7bb  ................
-00001620: 8fe6 988e e799 bdef bc8c e6ad a3e7 a1ae  ................
-00001630: e8ae bee5 ae9a e7ad 96e7 95a5 e79a 84e6  ................
-00001640: 9cac e987 9128 6070 7269 6e63 6970 616c  .....(`principal
-00001650: 6029 e4bc 9ae4 bdbf e5be 97e5 9b9e e6b5  `)..............
-00001660: 8be7 9a84 e7b3 bbe7 bb9f e8af afe5 b7ae  ................
-00001670: e69b b4e5 b08f e380 820a 0a23 2320 e5a7  ...........## ..
-00001680: 94e4 b9b0 e5a7 94e5 8d96 0ae5 a794 e4b9  ................
-00001690: b0e6 97b6 efbc 8ce5 a794 e4b9 b0e9 878f  ................
-000016a0: e5bf 85e9 a1bb e698 af31 3030 e882 a1e7  .........100....
-000016b0: 9a84 e695 b4e6 95b0 e580 8de3 8082 e8bf  ................
-000016c0: 99e4 b8aa e999 90e5 88b6 e4b8 8ee5 ae9e  ................
-000016d0: e79b 98e6 98af e4b8 80e8 87b4 e79a 84e3  ................
-000016e0: 8082 e590 8ce6 a0b7 efbc 8ce6 82a8 e79a  ................
-000016f0: 84e5 88b8 e595 86e5 afb9 e5a7 94e5 8d96  ................
-00001700: e4ba a4e6 9893 e4b9 9fe5 819a e4ba 86e9  ................
-00001710: 9990 e588 b6ef bc8c e4bd 86e5 9b9e e6b5  ................
-00001720: 8be6 9c8d e58a a1e5 99a8 e5b9 b6e6 9caa  ................
-00001730: e5af b9e6 ada4 e8bf 9be8 a18c e999 90e5  ................
-00001740: 88b6 e380 82e7 bb8f e8af 84e4 bcb0 efbc  ................
-00001750: 8ce5 8ebb e68e 89e8 bf99 e4b8 aae9 9990  ................
-00001760: e588 b6e5 b9b6 e4b8 8de4 bc9a e5af b9e7  ................
-00001770: ad96 e795 a5e7 9a84 e69c 89e6 9588 e680  ................
-00001780: a7e4 baa7 e794 9fe4 bbbb e4bd 95e5 bdb1  ................
-00001790: e593 8def bc8c e4bd 86e4 bc9a e7ae 80e5  ................
-000017a0: 8c96 e7ad 96e7 95a5 e79a 84e7 bc96 e586  ................
-000017b0: 99e3 8082 0a0a 2323 20e5 819c e789 8ce5  ......## .......
-000017c0: a484 e790 860a e5a6 82e6 9e9c e69f 90e6  ................
-000017d0: 94af e68c 81e4 bb93 e882 a1e5 bd93 e589  ................
-000017e0: 8de5 819c e789 8cef bc8c e59c a8e8 aea1  ................
-000017f0: e7ae 97e6 8c81 e4bb 93e5 b882 e580 bce6  ................
-00001800: 97b6 efbc 8ce7 b3bb e7bb 9fe4 bc9a e4bd  ................
-00001810: bfe7 94a8 e581 9ce7 898c e589 8de7 9a84  ................
-00001820: e694 b6e7 9b98 e4bb b7e6 9da5 e8ae a1e7  ................
-00001830: ae97 e5b8 82e5 80bc e380 82e4 b8ba e680  ................
-00001840: a7e8 83bd e4bc 98e5 8c96 e880 83e9 aa8c  ................
-00001850: efbc 8ce5 a682 e69e 9ce4 b880 e694 afe8  ................
-00001860: 82a1 e7a5 a8e5 819c e789 8ce6 97b6 e997  ................
-00001870: b4e8 b685 e8bf 8735 3030 e4b8 aae4 baa4  .......500......
-00001880: e698 93e6 97a5 efbc 8ce5 8899 e7b3 bbe7  ................
-00001890: bb9f e5b0 86e6 94be e5bc 83e7 bba7 e7bb  ................
-000018a0: ade5 9091 e589 8de6 909c e7b4 a2e5 819c  ................
-000018b0: e789 8ce5 898d e79a 84e6 94b6 e79b 98e4  ................
-000018c0: bbb7 efbc 8ce6 94b9 e794 a8e4 b9b0 e585  ................
-000018d0: a5e6 97b6 e79a 84e6 8890 e4ba a4e5 9d87  ................
-000018e0: e4bb b7e6 9da5 e4bb a3e6 9bbf e380 82e8  ................
-000018f0: bf99 e7a7 8de6 8385 e586 b5e5 ba94 e8af  ................
-00001900: a5e7 9bb8 e5bd 93e7 bd95 e8a7 81e3 8082  ................
-00001910: 0a23 20e7 8988 e69c ace5 8e86 e58f b20a  .# .............
-00001920: e585 b3e4 ba8e e789 88e6 9cac e58e 86e5  ................
-00001930: 8fb2 efbc 8ce8 afb7 e69f a5e9 9885 5be7  ..............[.
-00001940: 8988 e69c ace5 8e86 e58f b25d 2868 6973  ...........](his
-00001950: 746f 7279 290a 2320 4372 6564 6974 730a  tory).# Credits.
-00001960: 0a5a 696c 6c69 6f6e 6172 652d 6261 636b  .Zillionare-back
-00001970: 7465 7374 e9a1 b9e7 9bae e698 afe9 809a  test............
-00001980: e8bf 875b 5079 7468 6f6e 2050 726f 6a65  ...[Python Proje
-00001990: 6374 2057 697a 6172 645d 287a 696c 6c69  ct Wizard](zilli
-000019a0: 6f6e 6172 652e 6769 7468 7562 2e69 6f2f  onare.github.io/
-000019b0: 7079 7468 6f6e 2d70 726f 6a65 6374 2d77  python-project-w
-000019c0: 697a 6172 6429 e588 9be5 bbba e79a 84e3  izard)..........
-000019d0: 8082 0a0a 0a5b 5e31 5d3a e6ad a4e5 8a9f  .....[^1]:......
-000019e0: e883 bde5 9ca8 302e 342e 78e7 8988 e69c  ......0.4.x.....
-000019f0: ace4 b8ad e5b0 9ae4 b88d e58f afe7 94a8  ................
-00001a00: e380 820a                                ....
+00000990: 8082 0a0a e59c a8e5 9b9e e6b5 8be5 ae8c  ................
+000009a0: e688 90e6 97b6 efbc 8ce8 afb7 e8ae b0e5  ................
+000009b0: be97 e8b0 83e7 94a8 7374 6f70 5f62 6163  ........stop_bac
+000009c0: 6b74 6573 74e3 8082 0a0a e59c a8e5 9b9e  ktest...........
+000009d0: e6b5 8be5 ae8c e688 90e6 97b6 efbc 8c73  ...............s
+000009e0: 746f 705f 6261 636b 7465 7374 e4bc 9ae5  top_backtest....
+000009f0: b086 e8b5 84e4 baa7 e8a1 a8e6 9bb4 e696  ................
+00000a00: b0e5 88b0 e59b 9ee6 b58b e7bb 93e6 9d9f  ................
+00000a10: e697 a5ef bc88 e590 a6e5 8899 efbc 8ce5  ................
+00000a20: 8faa e69b b4e6 96b0 e588 b0e6 9c80 e590  ................
+00000a30: 8ee4 b880 e6ac a1e4 baa4 e698 93e5 bd93  ................
+00000a40: e5a4 a9ef bc8c e59b a0e4 b8ba e69c 8de5  ................
+00000a50: 8aa1 e599 a8e5 ae8c e585 a8e7 94b1 e5ae  ................
+00000a60: a2e6 88b7 e7ab afe6 9da5 e9a9 b1e5 8aa8  ................
+00000a70: efbc 8ce8 87aa e5b7 b1e6 b2a1 e69c 89e6  ................
+00000a80: 97b6 e997 b4e6 a682 e5bf b5ef bc89 e380  ................
+00000a90: 82e4 bd86 e5b9 b6e4 b88d e4bc 9ae5 afb9  ................
+00000aa0: e5bd 93e5 898d e68c 81e4 bb93 e8bf 9be8  ................
+00000ab0: a18c e58d 96e5 87ba e693 8de4 bd9c efbc  ................
+00000ac0: 8ce5 8e9f e59b a0e6 98af efbc 9a0a 312e  ..............1.
+00000ad0: 20e5 8d96 e587 bae6 938d e4bd 9ce5 b086   ...............
+00000ae0: e4bf aee6 94b9 7472 616e 7361 6374 696f  ......transactio
+00000af0: 6e73 e8a1 a8e3 8082 e880 8ce6 96b0 e5a2  ns..............
+00000b00: 9ee7 9a84 7472 616e 7361 6374 696f 6ee5  ....transaction.
+00000b10: b9b6 e4b8 8de6 98af e7ad 96e7 95a5 e8a7  ................
+00000b20: a6e5 8f91 e79a 840a 322e 20e4 b88d e588  ........2. .....
+00000b30: a9e4 ba8e e8af 84e4 bcb0 e7ad 96e7 95a5  ................
+00000b40: e79a 84e7 9c9f e5ae 9ee6 8385 e586 b5e3  ................
+00000b50: 8082 e5a6 82e6 9e9c e59c a8e5 9b9e e6b5  ................
+00000b60: 8be6 9c9f e587 bae7 8eb0 e4bb 85e6 9c89  ................
+00000b70: e4b8 80e7 ac94 e79c 9fe5 ae9e e4ba a4e6  ................
+00000b80: 9893 efbc 8ce5 85b6 e5ae 83e9 83bd e698  ................
+00000b90: afe8 a2ab e7bb 88e6 9cab e5bc bae5 b9b3  ................
+00000ba0: e79a 84e8 af9d efbc 8ce9 82a3 e4b9 88e6  ................
+00000bb0: ada4 e6ac a1e5 9b9e e6b5 8be5 ae9e e999  ................
+00000bc0: 85e4 b88a e58f afe8 83bd e59c a8e6 97b6  ................
+00000bd0: e997 b4e4 b88a e380 81e6 8896 e880 85e7  ................
+00000be0: ad96 e795 a5e5 91a8 e69c 9fe4 b88a e6b2  ................
+00000bf0: a1e6 9c89 e980 89e5 a5bd e380 82e5 a682  ................
+00000c00: e69e 9ce5 9b9e e6b5 8be7 b3bb e7bb 9fe8  ................
+00000c10: bf9b e8a1 8ce5 bcba e5b9 b3ef bc8c e5b0  ................
+00000c20: b1e5 8faf e883 bde6 8ea9 e79b 96e8 bf99  ................
+00000c30: e7a7 8de4 ba8b e5ae 9ee3 8082 0a33 2e20  .............3. 
+00000c40: e59c a8e5 9b9e e6b5 8be7 bb88 e69c abe6  ................
+00000c50: 9c9f efbc 8ce5 8faf e883 bde5 ad98 e59c  ................
+00000c60: a8e8 82a1 e7a5 a8e5 9ba0 e8b7 8ce5 819c  ................
+00000c70: e880 8ce6 97a0 e6b3 95e5 8d96 e587 bae7  ................
+00000c80: 9a84 e683 85e5 86b5 efbc 9be6 8896 e880  ................
+00000c90: 85e8 82a1 e7a5 a8e5 819c e789 8ce4 b8ad  ................
+00000ca0: efbc 8ce6 97a0 e6b3 95e5 8d96 e587 bae3  ................
+00000cb0: 8082 e8bf 99e4 ba9b e683 85e5 86b5 e4b8  ................
+00000cc0: 8bef bc8c e6a8 a1e6 8b9f e58d 96e5 87ba  ................
+00000cd0: e4b9 9fe6 9c89 e99a bee5 baa6 e380 820a  ................
+00000ce0: 2323 20e4 baa4 e698 93e6 92ae e590 880a  ## .............
+00000cf0: 0ae6 82a8 e58f afe4 bba5 e980 9ae8 bf87  ................
+00000d00: 5b62 7579 5d5b 6261 636b 7465 7374 2e77  [buy][backtest.w
+00000d10: 6562 2e69 6e74 6572 6661 6365 732e 6275  eb.interfaces.bu
+00000d20: 795d 2c20 5b6d 6172 6b65 745f 6275 795d  y], [market_buy]
+00000d30: 5b62 6163 6b74 6573 742e 7765 622e 696e  [backtest.web.in
+00000d40: 7465 7266 6163 6573 2e6d 6172 6b65 745f  terfaces.market_
+00000d50: 6275 795d 2c20 5b73 656c 6c5d 5b62 6163  buy], [sell][bac
+00000d60: 6b74 6573 742e 7765 622e 696e 7465 7266  ktest.web.interf
+00000d70: 6163 6573 2e73 656c 6c5d 2c20 5b6d 6172  aces.sell], [mar
+00000d80: 6b65 745f 7365 6c6c 5d5b 6261 636b 7465  ket_sell][backte
+00000d90: 7374 2e77 6562 2e69 6e74 6572 6661 6365  st.web.interface
+00000da0: 732e 6d61 726b 6574 5f73 656c 6c5d e592  s.market_sell]..
+00000db0: 8c5b 7365 6c6c 5f70 6572 6365 6e74 5d5b  .[sell_percent][
+00000dc0: 6261 636b 7465 7374 2e77 6562 2e69 6e74  backtest.web.int
+00000dd0: 6572 6661 6365 732e 7365 6c6c 5f70 6572  erfaces.sell_per
+00000de0: 6365 6e74 5de6 9da5 e8bf 9be8 a18c e4ba  cent]...........
+00000df0: a4e6 9893 e380 820a 0a23 2320 e78a b6e6  .........## ....
+00000e00: 8081 e8b7 9fe8 b8aa 0a0a e682 a8e5 8faf  ................
+00000e10: e4bb a5e9 809a e8bf 875b 696e 666f 5d5b  .........[info][
+00000e20: 6261 636b 7465 7374 2e77 6562 2e69 6e74  backtest.web.int
+00000e30: 6572 6661 6365 732e 696e 666f 5de6 9da5  erfaces.info]...
+00000e40: e69f a5e7 9c8b e8b4 a6e6 88b7 e79a 84e5  ................
+00000e50: 9fba e69c ace4 bfa1 e681 afef bc8c e6af  ................
+00000e60: 94e5 a682 e5bd 93e5 898d e680 bbe8 b584  ................
+00000e70: e4ba a7e3 8081 e68c 81e4 bb93 e380 81e6  ................
+00000e80: 9cac e987 91e3 8081 e79b 88e5 88a9 e7ad  ................
+00000e90: 89e3 8082 e682 a8e8 bf98 e58f afe4 bba5  ................
+00000ea0: e980 9ae8 bf87 5b70 6f73 6974 696f 6e73  ......[positions
+00000eb0: 5d5b 6261 636b 7465 7374 2e77 6562 2e69  ][backtest.web.i
+00000ec0: 6e74 6572 6661 6365 732e 706f 7369 7469  nterfaces.positi
+00000ed0: 6f6e 735d e380 815b 6269 6c6c 735d 5b62  ons]...[bills][b
+00000ee0: 6163 6b74 6573 742e 7765 622e 696e 7465  acktest.web.inte
+00000ef0: 7266 6163 6573 2e62 696c 6c73 5de6 9da5  rfaces.bills]...
+00000f00: e69f a5e7 9c8b e8b4 a6e6 88b7 e79a 84e6  ................
+00000f10: 8c81 e4bb 93e3 8081 e4ba a4e6 9893 e58e  ................
+00000f20: 86e5 8fb2 e8ae b0e5 bd95 0a23 2320 e7ad  ...........## ..
+00000f30: 96e7 95a5 e8af 84e4 bcb0 0a0a 5b6d 6574  ............[met
+00000f40: 7269 6373 5d5b 6261 636b 7465 7374 2e77  rics][backtest.w
+00000f50: 6562 2e69 6e74 6572 6661 6365 732e 6d65  eb.interfaces.me
+00000f60: 7472 6963 735d e696 b9e6 b395 e5b0 86e8  trics]..........
+00000f70: bf94 e59b 9ee7 ad96 e795 a5e7 9a84 e590  ................
+00000f80: 84e9 a1b9 e68c 87e6 a087 efbc 8ce6 af94  ................
+00000f90: e5a6 8273 6861 7270 652c 2073 6f72 7469  ...sharpe, sorti
+00000fa0: 6e6f 2c20 6361 6c6d 6172 2c20 7769 6e20  no, calmar, win 
+00000fb0: 7261 7465 2c20 6d61 7820 6472 6177 646f  rate, max drawdo
+00000fc0: 776e e7ad 89e3 8082 e682 a8e8 bf98 e58f  wn..............
+00000fd0: afe4 bba5 e4bc a0e5 85a5 e4b8 80e4 b8aa  ................
+00000fe0: e58f 82e8 8083 e6a0 87e7 9a84 efbc 8c62  ...............b
+00000ff0: 6163 6b74 6573 74e5 b086 e5af b9e5 8f82  acktest.........
+00001000: e880 83e6 a087 e79a 84e4 b99f e590 8ce6  ................
+00001010: a0b7 e8ae a1e7 ae97 e4b8 8ae8 bfb0 e68c  ................
+00001020: 87e6 a087 e380 820a 0a23 20e5 85b3 e994  .........# .....
+00001030: aee6 a682 e5bf b50a 0a23 2320 e5a4 8de6  .........## ....
+00001040: 9d83 e5a4 84e7 9086 0ae6 82a8 e79a 84e7  ................
+00001050: ad96 e795 a5e5 9ca8 e58f 91e5 87ba e4b9  ................
+00001060: b0e5 8d96 e4bf a1e5 8fb7 e697 b6ef bc8c  ................
+00001070: e5ba 94e8 afa5 e4bd bfe7 94a8 e4b8 8e60  ...............`
+00001080: 6f72 6465 725f 7469 6d65 60e4 b880 e887  order_time`.....
+00001090: b4e7 9a84 e78e b0e4 bbb7 efbc 8ce8 808c  ................
+000010a0: e4b8 8de6 98af e4bb bbe4 bd95 e5a4 8de6  ................
+000010b0: 9d83 e4bb b7e3 8082 e5a6 82e6 9e9c e682  ................
+000010c0: a8e7 9a84 e68c 81e4 bb93 e59c a8e6 8c81  ................
+000010d0: e69c 89e6 9c9f e997 b4ef bc8c e58f 91e7  ................
+000010e0: 949f e4ba 86e5 8886 e7ba a2e9 8081 e882  ................
+000010f0: a1ef bc8c e59b 9ee6 b58b e69c 8de5 8aa1  ................
+00001100: e599 a8e4 bc9a e887 aae5 8aa8 e5b0 86e5  ................
+00001110: 8886 e7ba a2e9 8081 e882 a1e8 bdac e68d  ................
+00001120: a2e6 8890 e882 a1e6 95b0 e58a a0e5 88b0  ................
+00001130: e682 a8e7 9a84 e68c 81e4 bb93 e4b8 ade3  ................
+00001140: 8082 e5bd 93e6 82a8 e69c 80e7 bb88 e6b8  ................
+00001150: 85e7 a9ba e68c 81e4 bb93 e697 b6ef bc8c  ................
+00001160: e58f afe4 bba5 e980 9ae8 bf87 6062 696c  ............`bil
+00001170: 6c73 60e6 8ea5 e58f a3e6 9fa5 e8af a2e5  ls`.............
+00001180: 88b0 e588 86e7 baa2 e980 81e8 82a1 e79a  ................
+00001190: 84e6 8890 e4ba a4e6 8385 e586 b5ef bc88  ................
+000011a0: e8ae b0e5 bd95 e4b8 ba58 4458 52e7 b1bb  .........XDXR...
+000011b0: e59e 8be7 9a84 e5a7 94e6 8998 efbc 89e3  ................
+000011c0: 8082 0a0a 2323 20e6 92ae e590 88e6 9cba  ....## .........
+000011d0: e588 b60a e59c a8e6 92ae e590 88e6 97b6  ................
+000011e0: efbc 8c62 6163 6b74 6573 74e9 a696 e585  ...backtest.....
+000011f0: 88e4 bb8e 6461 7461 2066 6565 6465 72e4  ....data feeder.
+00001200: b8ad e88e b7e5 8f96 606f 7264 6572 5f74  ........`order_t
+00001210: 696d 6560 e4bb a5e5 908e efbc 88e5 90ab  ime`............
+00001220: efbc 89e7 9a84 e8a1 8ce6 8385 e695 b0e6  ................
+00001230: 8dae e380 82e6 8ea5 e4b8 8be6 9da5 e58e  ................
+00001240: bbe6 8e89 e5a4 84e5 9ca8 e6b6 a8e8 b78c  ................
+00001250: e581 9ce4 b8ad e79a 84e9 82a3 e4ba 9b62  ...............b
+00001260: 6172 efbc 88e5 a682 e69e 9ce6 98af e5a7  ar..............
+00001270: 94e4 b9b0 efbc 8ce5 8899 e58e bbe6 8e89  ................
+00001280: e5b7 b2e5 a484 e59c a8e6 b6a8 e581 9ce6  ................
+00001290: 9c9f e997 b4e7 9a84 6261 72ef bc8c e58f  ........bar.....
+000012a0: 8de4 b98b e4ba a6e7 84b6 efbc 89e3 8082  ................
+000012b0: e59c a8e5 89a9 e4b8 8be7 9a84 6261 72e4  ............bar.
+000012c0: b8ad efbc 8c62 6163 6b74 6573 74e4 bc9a  .....backtest...
+000012d0: e980 89e6 8ba9 e4bb b7e6 a0bc e4bd 8ee4  ................
+000012e0: ba8e e5a7 94e6 8998 e4bb b7e7 9a84 e982  ................
+000012f0: a3e4 ba9b 6261 72ef bc88 e5a6 82e6 9e9c  ....bar.........
+00001300: e698 afe5 a794 e58d 96ef bc8c e588 99e9  ................
+00001310: 8089 e68b a9e4 bbb7 e6a0 bce9 ab98 e4ba  ................
+00001320: 8ee5 a794 e689 98e4 bbb7 e79a 84e9 82a3  ................
+00001330: e4ba 9b62 6172 efbc 892c e4be 9de9 a1ba  ...bar...,......
+00001340: e5ba 8fe5 8cb9 e985 8de5 a794 e689 98e9  ................
+00001350: 878f efbc 8ce7 9bb4 e588 b0e5 a794 e689  ................
+00001360: 98e9 878f e585 a8e9 83a8 e8a2 abe5 8cb9  ................
+00001370: e985 8de4 b8ba e6ad a2e3 8082 e69c 80e5  ................
+00001380: 908e efbc 8c62 6163 6b74 6573 74e5 b086  .....backtest...
+00001390: e58c b9e9 858d e588 b0e7 9a84 6261 72e7  ............bar.
+000013a0: 9a84 e987 8fe5 928c e4bb b7e6 a0bc e8bf  ................
+000013b0: 9be8 a18c e58a a0e6 9d83 e5b9 b3e5 9d87  ................
+000013c0: efbc 8ce5 be97 e588 b0e6 8890 e4ba a4e5  ................
+000013d0: 9d87 e4bb b7e3 8082 0a0a e5bd 9362 6163  .............bac
+000013e0: 6b74 6573 74e4 bdbf e794 a87a 696c 6c69  ktest......zilli
+000013f0: 6f6e 6172 652d 6665 6564 e69d a5e6 8f90  onare-feed......
+00001400: e4be 9be6 92ae e590 88e6 95b0 e68d aee6  ................
+00001410: 97b6 efbc 8ce7 94b1 e4ba 8ee7 bcba e5b0  ................
+00001420: 91e7 9b98 e58f a3e6 95b0 e68d aeef bc8c  ................
+00001430: 7a69 6c6c 696f 6e61 7265 2d66 6565 64e4  zillionare-feed.
+00001440: bdbf e794 a8e5 8886 e992 9fe7 baa7 e8a1  ................
+00001450: 8ce6 8385 e695 b0e6 8dae e4b8 ade7 9a84  ................
+00001460: 6063 6c6f 7365 60e4 bbb7 e6a0 bce5 928c  `close`.........
+00001470: 6076 6f6c 756d 6560 e69d a5e8 bf9b e8a1  `volume`........
+00001480: 8ce6 92ae e590 88e3 8082 e59b a0e6 ada4  ................
+00001490: efbc 8ce5 8faf e883 bde5 87ba e78e b0e6  ................
+000014a0: 9f90 e4b8 80e5 8886 e992 9fe7 9a84 e69c  ................
+000014b0: 80e9 ab98 e4bb b7e6 8896 e880 85e6 9c80  ................
+000014c0: e4bd 8ee4 bbb7 e58f afe8 83bd e6bb a1e8  ................
+000014d0: b6b3 e8bf 87e6 82a8 e79a 84e5 a794 e689  ................
+000014e0: 98e4 bbb7 e8a6 81e6 b182 efbc 8ce4 bd86  ................
+000014f0: 6261 636b 7465 7374 e5b9 b6e6 9caa e688  backtest........
+00001500: 90e4 baa4 e692 aee5 9088 e79a 84e6 8385  ................
+00001510: e586 b5e3 8082 e688 91e4 bbac e8bf 99e6  ................
+00001520: a0b7 e8ae bee8 aea1 efbc 8ce4 b8bb e8a6  ................
+00001530: 81e8 8083 e899 91e5 88b0 e5bd 93e8 82a1  ................
+00001540: e4bb b7e8 bebe e588 b0e6 9c80 e9ab 98e6  ................
+00001550: 8896 e880 85e6 9c80 e4bd 8ee7 82b9 e697  ................
+00001560: b6ef bc8c e5bd 93e6 97b6 e79a 84e6 8890  ................
+00001570: e4ba a4e9 878f e4b8 8de8 b6b3 e4bb a5e6  ................
+00001580: bba1 e8b6 b3e5 a794 e689 98e9 878f e380  ................
+00001590: 82e7 8eb0 e59c a862 6163 6b74 6573 74e7  .......backtest.
+000015a0: 9a84 e8ae bee8 aea1 efbc 8ce5 8faf e883  ................
+000015b0: bde7 ad96 e795 a5e7 9a84 e9b2 81e6 a392  ................
+000015c0: e680 a7e6 9bb4 e5a5 bde3 8082 0a0a e4bd  ................
+000015d0: 9ce4 b8ba e4b8 80e4 b8aa e4be 8be5 a496  ................
+000015e0: efbc 8ce5 a682 e69e 9ce5 a794 e689 98e6  ................
+000015f0: 97b6 e79a 8460 6f72 6465 725f 7469 6d65  .....`order_time
+00001600: 60e4 b8ba 393a 3331 e588 86e4 b98b e589  `...9:31........
+00001610: 8def bc8c 6261 636b 7465 7374 e5b0 86e4  ....backtest....
+00001620: bc9a e4bd bfe7 94a8 393a 3331 e588 86e9  ........9:31....
+00001630: 929f e7ba bfe7 9a84 e5bc 80e7 9b98 e4bb  ................
+00001640: b7ef bc8c e880 8ce4 b88d e698 af39 3a33  .............9:3
+00001650: 31e5 8886 e79a 84e6 94b6 e79b 98e4 bbb7  1...............
+00001660: e69d a5e8 bf9b e8a1 8ce6 92ae e590 88ef  ................
+00001670: bc8c e4bb a5e6 bba1 e8b6 b3e9 83a8 e588  ................
+00001680: 86e7 ad96 e795 a5e9 9c80 e8a6 81e4 bba5  ................
+00001690: 2a2a e6ac a1e6 97a5 e5bc 80e7 9b98 e4bb  **..............
+000016a0: b72a 2ae4 b9b0 e585 a5e7 9a84 e99c 80e6  .**.............
+000016b0: b182 e380 820a 0ae5 8fa6 e5a4 96ef bc8c  ................
+000016c0: e682 a8e4 b99f e5ba 94e8 afa5 e6b3 a8e6  ................
+000016d0: 848f e588 b0ef bc8c 7a69 6c6c 696f 6e61  ........zilliona
+000016e0: 7265 2d66 6565 64e4 bdbf e794 a8e5 8886  re-feed.........
+000016f0: e992 9fe7 babf e69d a5e6 9bbf e4bb a3e4  ................
+00001700: ba86 e79b 98e5 8fa3 e695 b0e6 8dae efbc  ................
+00001710: 8ce5 b0bd e7ae a1e5 9ca8 e7bb 9de5 a4a7  ................
+00001720: e5a4 9ae6 95b0 e683 85e5 bda2 e4b8 8bef  ................
+00001730: bc8c e8bf 99e6 a0b7 e581 9ae4 b88d e4bc  ................
+00001740: 9ae6 9c89 e4bb 80e4 b988 e5bd b1e5 938d  ................
+00001750: efbc 8ce4 bd86 e4b8 a4e8 8085 e6af 95e7  ................
+00001760: ab9f e698 afe4 b88d e590 8ce7 9a84 e380  ................
+00001770: 82e4 b880 e888 ace6 9da5 e8af b4ef bc8c  ................
+00001780: e688 90e4 baa4 e987 8fe8 82af e5ae 9ae5  ................
+00001790: b08f e4ba 8ee7 9b98 e58f a3e7 9a84 e5a7  ................
+000017a0: 94e4 b9b0 e5a7 94e5 8d96 e987 8fe3 8082  ................
+000017b0: e59b a0e6 ada4 efbc 8ce5 9ca8 e59b 9ee6  ................
+000017c0: b58b e4b8 ade5 87ba e78e b0e4 b9b0 e58d  ................
+000017d0: 96e5 a794 e689 98e9 878f e4b8 8de8 b6b3  ................
+000017e0: e79a 84e6 8385 e586 b5e6 97b6 efbc 8ce5  ................
+000017f0: afb9 e5ba 94e7 9a84 e5ae 9ee7 9b98 e588  ................
+00001800: 99e4 b88d e4b8 80e5 ae9a e587 bae7 8eb0  ................
+00001810: e380 82e5 9ca8 e8bf 99e7 a78d e683 85e5  ................
+00001820: 86b5 e4b8 8bef bc8c e58f afe4 bba5 e980  ................
+00001830: 82e5 bd93 e8b0 83e4 bd8e e7ad 96e7 95a5  ................
+00001840: e79a 84e6 9cac e987 91e8 aebe e7bd aee3  ................
+00001850: 8082 e58f a6e5 a496 e4b8 80e4 b8aa e5b7  ................
+00001860: aee5 bc82 e698 afef bc8c e588 86e9 929f  ................
+00001870: e688 90e4 baa4 e4bb b7e5 bf85 e784 b6e4  ................
+00001880: b88d e7ad 89e5 908c e4ba 8ee7 9b98 e58f  ................
+00001890: a3e6 8890 e4ba a4e4 bbb7 efbc 8ce5 9ba0  ................
+000018a0: e6ad a4e4 bc9a e5bc 95e5 85a5 e4b8 80e5  ................
+000018b0: ae9a e79a 84e8 afaf e5b7 aee3 8082 e4b8  ................
+000018c0: 8de8 bf87 e995 bfe6 9c9f e69d a5e7 9c8b  ................
+000018d0: efbc 8ce8 bf99 e7a7 8de8 afaf e5b7 aee5  ................
+000018e0: ba94 e8af a5e6 98af e99b b6e5 9d87 e580  ................
+000018f0: bce7 9a84 efbc 8ce5 9ba0 e6ad a4e5 afb9  ................
+00001900: e7bb 9de5 a4a7 e5a4 9ae6 95b0 e7ad 96e7  ................
+00001910: 95a5 e4b8 8de4 bc9a e4ba a7e7 949f e5ae  ................
+00001920: 9ee8 b4a8 e5bd b1e5 938d e380 820a 0a21  ...............!
+00001930: 2121 696e 666f 0a20 2020 20e4 ba86 e8a7  !!info.    .....
+00001940: a362 6163 6b74 6573 74e7 9a84 e692 aee5  .backtest.......
+00001950: 9088 e69c bae5 88b6 e590 8eef bc8c e682  ................
+00001960: a8e5 ba94 e8af a5e5 b7b2 e7bb 8fe6 988e  ................
+00001970: e799 bdef bc8c e6ad a3e7 a1ae e8ae bee5  ................
+00001980: ae9a e7ad 96e7 95a5 e79a 84e6 9cac e987  ................
+00001990: 9128 6070 7269 6e63 6970 616c 6029 e4bc  .(`principal`)..
+000019a0: 9ae4 bdbf e5be 97e5 9b9e e6b5 8be7 9a84  ................
+000019b0: e7b3 bbe7 bb9f e8af afe5 b7ae e69b b4e5  ................
+000019c0: b08f e380 820a 0a23 2320 e5a7 94e4 b9b0  .......## ......
+000019d0: e5a7 94e5 8d96 0ae5 a794 e4b9 b0e6 97b6  ................
+000019e0: efbc 8ce5 a794 e4b9 b0e9 878f e5bf 85e9  ................
+000019f0: a1bb e698 af31 3030 e882 a1e7 9a84 e695  .....100........
+00001a00: b4e6 95b0 e580 8de3 8082 e8bf 99e4 b8aa  ................
+00001a10: e999 90e5 88b6 e4b8 8ee5 ae9e e79b 98e6  ................
+00001a20: 98af e4b8 80e8 87b4 e79a 84e3 8082 e590  ................
+00001a30: 8ce6 a0b7 efbc 8ce6 82a8 e79a 84e5 88b8  ................
+00001a40: e595 86e5 afb9 e5a7 94e5 8d96 e4ba a4e6  ................
+00001a50: 9893 e4b9 9fe5 819a e4ba 86e9 9990 e588  ................
+00001a60: b6ef bc8c e4bd 86e5 9b9e e6b5 8be6 9c8d  ................
+00001a70: e58a a1e5 99a8 e5b9 b6e6 9caa e5af b9e6  ................
+00001a80: ada4 e8bf 9be8 a18c e999 90e5 88b6 e380  ................
+00001a90: 82e7 bb8f e8af 84e4 bcb0 efbc 8ce5 8ebb  ................
+00001aa0: e68e 89e8 bf99 e4b8 aae9 9990 e588 b6e5  ................
+00001ab0: b9b6 e4b8 8de4 bc9a e5af b9e7 ad96 e795  ................
+00001ac0: a5e7 9a84 e69c 89e6 9588 e680 a7e4 baa7  ................
+00001ad0: e794 9fe4 bbbb e4bd 95e5 bdb1 e593 8def  ................
+00001ae0: bc8c e4bd 86e4 bc9a e7ae 80e5 8c96 e7ad  ................
+00001af0: 96e7 95a5 e79a 84e7 bc96 e586 99e3 8082  ................
+00001b00: 0a0a 2323 20e5 819c e789 8ce5 a484 e790  ..## ...........
+00001b10: 860a e5a6 82e6 9e9c e69f 90e6 94af e68c  ................
+00001b20: 81e4 bb93 e882 a1e5 bd93 e589 8de5 819c  ................
+00001b30: e789 8cef bc8c e59c a8e8 aea1 e7ae 97e6  ................
+00001b40: 8c81 e4bb 93e5 b882 e580 bce6 97b6 efbc  ................
+00001b50: 8ce7 b3bb e7bb 9fe4 bc9a e4bd bfe7 94a8  ................
+00001b60: e581 9ce7 898c e589 8de7 9a84 e694 b6e7  ................
+00001b70: 9b98 e4bb b7e6 9da5 e8ae a1e7 ae97 e5b8  ................
+00001b80: 82e5 80bc e380 82e4 b8ba e680 a7e8 83bd  ................
+00001b90: e4bc 98e5 8c96 e880 83e9 aa8c efbc 8ce5  ................
+00001ba0: a682 e69e 9ce4 b880 e694 afe8 82a1 e7a5  ................
+00001bb0: a8e5 819c e789 8ce6 97b6 e997 b4e8 b685  ................
+00001bc0: e8bf 8735 3030 e4b8 aae4 baa4 e698 93e6  ...500..........
+00001bd0: 97a5 efbc 8ce5 8899 e7b3 bbe7 bb9f e5b0  ................
+00001be0: 86e6 94be e5bc 83e7 bba7 e7bb ade5 9091  ................
+00001bf0: e589 8de6 909c e7b4 a2e5 819c e789 8ce5  ................
+00001c00: 898d e79a 84e6 94b6 e79b 98e4 bbb7 efbc  ................
+00001c10: 8ce6 94b9 e794 a8e4 b9b0 e585 a5e6 97b6  ................
+00001c20: e79a 84e6 8890 e4ba a4e5 9d87 e4bb b7e6  ................
+00001c30: 9da5 e4bb a3e6 9bbf e380 82e8 bf99 e7a7  ................
+00001c40: 8de6 8385 e586 b5e5 ba94 e8af a5e7 9bb8  ................
+00001c50: e5bd 93e7 bd95 e8a7 81e3 8082 0a23 20e7  .............# .
+00001c60: 8988 e69c ace5 8e86 e58f b20a e585 b3e4  ................
+00001c70: ba8e e789 88e6 9cac e58e 86e5 8fb2 efbc  ................
+00001c80: 8ce8 afb7 e69f a5e9 9885 5be7 8988 e69c  ..........[.....
+00001c90: ace5 8e86 e58f b25d 2868 6973 746f 7279  .......](history
+00001ca0: 290a 2320 4372 6564 6974 730a 0a5a 696c  ).# Credits..Zil
+00001cb0: 6c69 6f6e 6172 652d 6261 636b 7465 7374  lionare-backtest
+00001cc0: e9a1 b9e7 9bae e698 afe9 809a e8bf 875b  ...............[
+00001cd0: 5079 7468 6f6e 2050 726f 6a65 6374 2057  Python Project W
+00001ce0: 697a 6172 645d 287a 696c 6c69 6f6e 6172  izard](zillionar
+00001cf0: 652e 6769 7468 7562 2e69 6f2f 7079 7468  e.github.io/pyth
+00001d00: 6f6e 2d70 726f 6a65 6374 2d77 697a 6172  on-project-wizar
+00001d10: 6429 e588 9be5 bbba e79a 84e3 8082 0a0a  d)..............
+00001d20: 0a5b 5e31 5d3a e6ad a4e5 8a9f e883 bde5  .[^1]:..........
+00001d30: 9ca8 302e 342e 78e7 8988 e69c ace4 b8ad  ..0.4.x.........
+00001d40: e5b0 9ae4 b88d e58f afe7 94a8 e380 820a  ................
```

### Comparing `zillionare-backtest-0.4.12/backtest/app.py` & `zillionare_backtest-0.4.18/backtest/app.py`

 * *Files identical despite different names*

### Comparing `zillionare-backtest-0.4.12/backtest/cli.py` & `zillionare_backtest-0.4.18/backtest/cli.py`

 * *Files identical despite different names*

### Comparing `zillionare-backtest-0.4.12/backtest/common/errors.py` & `zillionare_backtest-0.4.18/backtest/common/errors.py`

 * *Files 4% similar despite different names*

```diff
@@ -38,14 +38,15 @@
     REACH_BUY_LIMIT = -3
     REACH_SELL_LIMIT = -4
     NO_POSITION = -5
     PRICE_NOT_MEET = -6
     NODATA_FOR_MATCH = -7
     NODATA = -8
     TIME_REWIND = -9
+    VOLUME_NOT_ENOUGH = -10
 
     def __init__(self, status_code: int, **kwargs):
         self.status_code = status_code
         self.message = self.__template__().format(**kwargs)
 
     def __template__(self):
         return {
@@ -54,8 +55,9 @@
             EntrustError.REACH_BUY_LIMIT: "不能在涨停板上买入{security}, {time}",
             EntrustError.REACH_SELL_LIMIT: "不能在跌停板上卖出{security}, {time}",
             EntrustError.NO_POSITION: "{security}在{time}期间没有持仓",
             EntrustError.PRICE_NOT_MEET: "{security}现价未达到委托价:{entrust}",
             EntrustError.NODATA_FOR_MATCH: "没有匹配到{security}在{time}的成交数据",
             EntrustError.NODATA: "获取{security}在{time}的行情数据失败，请检查日期是否为交易日，或者当天是否停牌",
             EntrustError.TIME_REWIND: "委托时间必须递增出现。当前{time}, 前一个委托时间{last_trade_time}",
+            EntrustError.VOLUME_NOT_ENOUGH: "{security}委托价{price}达到，但成交量为零。",
         }.get(self.status_code)
```

### Comparing `zillionare-backtest-0.4.12/backtest/common/helper.py` & `zillionare_backtest-0.4.18/backtest/common/helper.py`

 * *Files identical despite different names*

### Comparing `zillionare-backtest-0.4.12/backtest/config/__init__.py` & `zillionare_backtest-0.4.18/backtest/config/__init__.py`

 * *Files identical despite different names*

### Comparing `zillionare-backtest-0.4.12/backtest/config/dev.yaml` & `zillionare_backtest-0.4.18/backtest/config/dev.yaml`

 * *Files identical despite different names*

### Comparing `zillionare-backtest-0.4.12/backtest/config/schema.py` & `zillionare_backtest-0.4.18/backtest/config/schema.py`

 * *Files identical despite different names*

### Comparing `zillionare-backtest-0.4.12/backtest/feed/basefeed.py` & `zillionare_backtest-0.4.18/backtest/feed/basefeed.py`

 * *Files identical despite different names*

### Comparing `zillionare-backtest-0.4.12/backtest/feed/zillionarefeed.py` & `zillionare_backtest-0.4.18/backtest/feed/zillionarefeed.py`

 * *Files identical despite different names*

### Comparing `zillionare-backtest-0.4.12/backtest/trade/broker.py` & `zillionare_backtest-0.4.18/backtest/trade/broker.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 """
 Broker是一个交易代理。每一个交易代理对应一个账户，记录了该账户下的交易记录、每日持仓记录和每日市值记录等数据，并提供交易撮合的具体实现。
 """
 import asyncio
 import datetime
 import logging
 import uuid
-from typing import Dict, List, Tuple
+from typing import Dict, List, Optional, Tuple, Union
 
 import arrow
 import cfg4py
 import numpy as np
 from coretypes import Frame, FrameType
 from empyrical import (
     annual_return,
@@ -36,14 +36,15 @@
     cash_dtype,
     daily_position_dtype,
     float_ts_dtype,
     position_dtype,
     rich_assets_dtype,
 )
 from backtest.trade.trade import Trade
+from backtest.trade.transaction import Transaction
 
 cfg = cfg4py.get_instance()
 logger = logging.getLogger(__name__)
 entrustlog = logging.getLogger("entrust")
 tradelog = logging.getLogger("trade")
 
 
@@ -97,15 +98,15 @@
         # 委托列表，包括废单和未成交委托
         self.entrusts = {}
 
         # 所有的成交列表，包括买入和卖出，已关闭和未关闭的
         self.trades = {}
 
         # trasaction = buy + sell trade
-        self.transactions = []
+        self.transactions: List[Transaction] = []
 
         self._lock = asyncio.Lock()
 
     def __getstate__(self):
         # self._lock is not pickable
         state = self.__dict__.copy()
         del state["_lock"]
@@ -224,15 +225,17 @@
 
         result = self._positions[self._positions["date"] == dt]
         if result.size == 0:
             raise ValueError(f"{dt} not found")
 
         return result[list(dtype.names)].astype(dtype)
 
-    async def recalc_assets(self, end: datetime.date = None):
+    async def recalc_assets(
+        self, start: Optional[datetime.date] = None, end: Optional[datetime.date] = None
+    ):
         """重新计算账户的每日资产
 
         计算完成后，资产表将包括从账户开始前一日，到`end`日的资产数据。从账户开始前一日起，是为了方便计算首个交易日的收益。
 
         Args:
             end: 计算到哪一天的资产，默认为空，即计算到最后一个交易日（非回测），或者回测结束日。
 
@@ -250,15 +253,15 @@
                 return np.array([], dtype=rich_assets_dtype)
 
             _before_start = tf.day_shift(start, -1)
             self._assets = np.array(
                 [(_before_start, self.principal)], dtype=assets_dtype
             )
 
-        start = tf.day_shift(self._assets[-1]["date"], 1)
+        start = start or tf.day_shift(self._assets[-1]["date"], 1)
         if start >= end:
             return
 
         # 待补齐的资产日
         frames = [tf.int2date(d) for d in tf.get_frames(start, end, FrameType.DAY)]
         # 从最后一个资产日到`end`，持仓应都是一样的
         position = self.get_position(end, position_dtype)
@@ -298,15 +301,15 @@
             if i is None:
                 self._assets = np.append(
                     self._assets,
                     np.array([(frame, float(cash + mv))], dtype=assets_dtype),
                     axis=0,
                 )
             else:
-                self._assets[i]["cash"] = float(cash + mv)
+                self._assets[i]["assets"] = float(cash + mv)
 
     async def info(self, dt: datetime.date = None) -> Dict:
         """`dt`日的账号相关信息
 
         Returns:
             Dict: 账号相关信息：
 
@@ -432,15 +435,18 @@
         assert len(pos) <= 1, "date should be unique"
         if len(pos) == 0:
             return None
 
         return pos[0]
 
     async def _calc_assets(self, date: datetime.date) -> Tuple[float]:
-        """计算某日的总资产，并缓存
+        """计算某日的总资产
+
+        此函数不更新资产表，以避免资产表中留下空洞。比如：
+        当前最后交易日为4月10日，4月17日发生一笔委卖，导致cash/position记录更新到4/17，但资产表仍然保持在4月10日，此时如果缓存该记录，将导致资产表中留下空洞。
 
         Args:
             date: 计算哪一天的资产
 
         Returns:
             返回总资产, 可用资金, 持仓市值
         """
@@ -469,23 +475,14 @@
                     market_value += shares * price
                 else:
                     price = positions[positions["security"] == sec]["price"].item()
                     market_value += shares * price
 
         assets = cash + market_value
 
-        i = self._index_of(self._assets, date)
-        if i is None:
-            self._assets = np.append(
-                self._assets, np.array([(date, assets)], dtype=assets_dtype)
-            )
-        else:
-            # don't use self._assets[self._assets["date"] == date], this always return copy
-            self._assets[i]["assets"] = assets
-
         return assets, cash, market_value
 
     @property
     def position(self) -> np.ndarray:
         """获取当前持仓
 
         如果要获取历史上某天的持仓，请使用`get_position`方法。
@@ -550,42 +547,47 @@
 
         if self.mode == "bt" and bid_time.date() > self.bt_stop:
             self._bt_stopped = True
             await self.recalc_assets()
             logger.warning("委托时间超过回测结束时间: %s, %s", bid_time, self.bt_stop)
             raise AccountError(f"下单时间为{bid_time},而账户已于{self.bt_stop}冻结。")
 
-    async def buy(self, *args, **kwargs) -> Trade:
+    async def buy(
+        self,
+        security: str,
+        bid_price: float,
+        bid_shares: int,
+        bid_time: datetime.datetime,
+    ) -> Trade:
         """买入委托
 
         买入以尽可能实现委托为目标。如果可用资金不足，但能买入部分股票，则部分买入。
 
         如果bid_price为None，则使用涨停价买入。
 
         Args:
             security str: 证券代码
             bid_price float: 委托价格。如果为None，则为市价委托
             bid_shares int: 询买的股数
             bid_time datetime.datetime: 委托时间
-            request_id str: 请求ID
 
         Returns:
             [Trade][backtest.trade.trade.Trade]对象
         """
         # 同一个账户，也可能出现并发的买单和卖单，这些操作必须串行化
         async with self.lock:
-            return await self._buy(*args, **kwargs)
+            return await self._buy(security, bid_price, bid_shares, bid_time)
 
     async def _buy(
         self,
         security: str,
         bid_price: float,
         bid_shares: int,
         bid_time: datetime.datetime,
-    ) -> Dict:
+    ) -> Trade:
         entrustlog.info(
             f"{bid_time}\t{security}\t{bid_shares}\t{bid_price}\t{EntrustSide.BUY}"
         )
         assert (
             type(bid_time) is datetime.datetime
         ), f"{bid_time} is not type of datetime"
 
@@ -645,15 +647,18 @@
                 EntrustError.NO_CASH,
                 account=self.account_name,
                 required=100 * bid_price,
                 available=self.cash,
             )
 
         mean_price, filled, close_time = self._match_buy(bars, shares_to_buy)
-
+        if filled == 0:
+            raise EntrustError(
+                EntrustError.VOLUME_NOT_ENOUGH, security=security, price=bid_price
+            )
         return await self._fill_buy_order(en, mean_price, filled, close_time)
 
     def _match_buy(
         self, bid_queue, shares_to_buy
     ) -> Tuple[float, float, datetime.datetime]:
         """计算此次买入的成交均价和成交量
 
@@ -775,28 +780,29 @@
 
         Args:
             bid_time: 委托时间
 
         Returns:
             无
         """
+        logger.info("bid_time is %s", bid_time)
         await self._calendar_validation(bid_time)
 
         # 补齐可用将资金表
         if self._cash.size == 0:
             start = tf.day_shift(self.account_start_date, -1)
             end = bid_time.date()
             frames = tf.get_frames(start, end, FrameType.DAY)
             _cash = [(tf.int2date(frame), self.principal) for frame in frames]
             self._cash = np.array(_cash, dtype=cash_dtype)
         else:
             prev, cash = self._cash[-1]
 
             frames = tf.get_frames(prev, bid_time, FrameType.DAY)[1:]
-            if frames.size > 0:
+            if len(frames) > 0:
                 recs = [(tf.int2date(date), cash) for date in frames]
 
                 self._cash = np.concatenate(
                     (self._cash, np.array(recs, dtype=cash_dtype))
                 )
 
         await self._fillup_positions(bid_time)
@@ -868,15 +874,15 @@
                         paddings["price"][i + 1].item(),
                         adjust_share,
                         0,
                         EntrustSide.XDXR,
                         order_time,
                     )
                     self.trades[trade.tid] = trade
-                    self._update_unclosed_trades(trade.tid, order_time.date())
+                    self._update_unclosed_trades(trade.tid, bid_time.date())
 
             paddings["sellable"][1:] = paddings["shares"][:-1]
 
             padding_positions.extend(paddings[1:])
 
         if len(padding_positions):
             padding_positions.sort(key=lambda x: x[0])
@@ -927,18 +933,20 @@
                     trade.security,
                     old_shares + trade.shares,
                     old_sellable,
                     (old_price * old_shares + new_shares * new_price)
                     / (old_shares + new_shares),
                 )
             else:
-                shares = math_round(old_shares - trade.shares, 4)
-                sellable = math_round(old_sellable - trade.shares, 4)
-                if shares == 0:
+                shares = old_shares - trade.shares
+                sellable = old_sellable - trade.shares
+                if shares <= 0.1:
                     old_price = 0
+                    shares = 0
+                    sellable = 0
                 self._positions[i] = (
                     bid_date,
                     trade.security,
                     shares,
                     sellable,
                     old_price,  # 卖出时成本不变，除非已清空
                 )
@@ -962,26 +970,35 @@
             self._assets = np.array(
                 [(_before_start, self.principal)], dtype=assets_dtype
             )
 
         start = tf.day_shift(self._assets[-1]["date"], 1)
         end = tf.day_shift(bid_time, -1)
         if start < end:
-            await self.recalc_assets(end)
+            await self.recalc_assets(start, end)
 
-        bid_time = bid_time.date()
+        bid_date = bid_time.date()
 
         # _before_trade应该已经为当日交易准备好了可用资金数据
-        assert self._cash[-1]["date"] == bid_time
+        assert self._cash[-1]["date"] == bid_date
         self._cash[-1]["cash"] += cash_change
 
-        assets, cash, mv = await self._calc_assets(bid_time)
+        assets, cash, mv = await self._calc_assets(bid_date)
+
+        i = self._index_of(self._assets, bid_date)
+        if i is None:
+            self._assets = np.append(
+                self._assets, np.array([(bid_date, assets)], dtype=assets_dtype)
+            )
+        else:
+            # don't use self._assets[self._assets["date"] == date], this always return copy
+            self._assets[i]["assets"] = assets
 
         info = np.array(
-            [(bid_time, assets, cash, mv, cash_change)],
+            [(bid_date, assets, cash, mv, cash_change)],
             dtype=[
                 ("date", "O"),
                 ("assets", float),
                 ("cash", float),
                 ("market value", float),
                 ("change", float),
             ],
@@ -1064,35 +1081,41 @@
         )
 
         await self._update_assets(refund, en.bid_time)
 
         await emit.emit(E_BACKTEST, {"sell": jsonify(exit_trades)})
         return exit_trades
 
-    async def sell(self, *args, **kwargs) -> List[Trade]:
+    async def sell(
+        self,
+        security: str,
+        bid_price: Union[None, float],
+        bid_shares: float,
+        bid_time: datetime.datetime,
+    ) -> List[Trade]:
         """卖出委托
 
         Args:
             security str: 委托证券代码
-            price float: 出售价格，如果为None，则为市价委托
+            bid_price float: 出售价格，如果为None，则为市价委托
             bid_shares float: 询卖股数。注意我们不限制必须以100的倍数卖出。
             bid_time datetime.datetime: 委托时间
 
         Returns:
             成交记录列表,每个元素都是一个[Trade][backtest.trade.trade.Trade]对象
 
         """
         # 同一个账户，也可能出现并发的买单和卖单，这些操作必须串行化
         async with self.lock:
-            return await self._sell(*args, **kwargs)
+            return await self._sell(security, bid_price, bid_shares, bid_time)
 
     async def _sell(
         self,
         security: str,
-        bid_price: float,
+        bid_price: Union[None, float],
         bid_shares: float,
         bid_time: datetime.datetime,
     ) -> List[Trade]:
         await self._before_trade(bid_time)
 
         feed = get_app_context().feed
 
@@ -1125,14 +1148,15 @@
         c, v = bars["price"], bars["volume"]
 
         cum_v = np.cumsum(v)
 
         shares_to_sell = self._get_sellable_shares(security, bid_shares, bid_time)
         if shares_to_sell == 0:
             logger.info("卖出失败: %s %s %s, 可用股数为0", security, bid_shares, bid_time)
+            logger.info("%s", self.get_unclosed_trades(bid_time.date()))
             raise EntrustError(
                 EntrustError.NO_POSITION, security=security, time=bid_time
             )
 
         # until i the order can be filled
         where_total_filled = np.argwhere(cum_v >= shares_to_sell)
         if len(where_total_filled) == 0:
@@ -1182,15 +1206,15 @@
         shares = 0
         for tid in self.get_unclosed_trades(bid_time.date()):
             t = self.trades[tid]
             if t.security == security and t.time.date() < bid_time.date():
                 assert t.closed is False
                 shares += t._unsell
 
-        if shares - shares_asked < 1.0:
+        if shares - shares_asked < 100:
             return shares
         return min(shares_asked, shares)
 
     def _remove_for_buy(
         self,
         security: str,
         order_time: datetime.datetime,
@@ -1247,17 +1271,17 @@
 
     def freeze(self):
         """冻结账户，停止接收新的委托"""
         self._bt_stopped = True
 
     async def metrics(
         self,
-        start: datetime.date = None,
-        end: datetime.date = None,
-        baseline: str = None,
+        start: Optional[datetime.date] = None,
+        end: Optional[datetime.date] = None,
+        baseline: Optional[str] = None,
     ) -> Dict:
         """获取指定时间段的账户指标
 
         Args:
             start: 开始时间
             end: 结束时间
             baseline: 参考标的
@@ -1294,17 +1318,25 @@
         except Exception:
             rf = 0
 
         start = min(start or self.account_start_date, self.account_start_date)
         end = max(end or self.account_end_date, self.account_end_date)
 
         tx = []
+        logger.info("%s tx in total", len(self.transactions))
         for t in self.transactions:
             if t.entry_time.date() >= start and t.exit_time.date() <= end:
                 tx.append(t)
+            else:
+                logger.info(
+                    "tx %s not in range, start: %s, end: %s",
+                    t.sec,
+                    t.entry_time,
+                    t.exit_time,
+                )
 
         # 资产暴露时间
         window = tf.count_day_frames(start, end)
         total_tx = len(tx)
 
         if total_tx == 0:
             return {
```

### Comparing `zillionare-backtest-0.4.12/backtest/trade/datatypes.py` & `zillionare_backtest-0.4.18/backtest/trade/datatypes.py`

 * *Files identical despite different names*

### Comparing `zillionare-backtest-0.4.12/backtest/trade/trade.py` & `zillionare_backtest-0.4.18/backtest/trade/trade.py`

 * *Files 5% similar despite different names*

```diff
@@ -43,14 +43,17 @@
         self.side = side
 
         # only for buying trade
         self._unsell = shares
         self._unamortized_fee = fee
         self.closed = False
 
+        if side == EntrustSide.XDXR:
+            logger.info("XDXR entrust: %s", self)
+
     def __str__(self):
         return f"证券代码: {self.security}\n成交方向: {self.side}\n成交均价: {self.price}\n数量: {self.shares}\n手续费: {self.fee}\n委托号: {self.eid}\n成交号: {self.tid}\n成交时间: {self.time}\n"
 
     def to_dict(self) -> dict:
         """将Trade对象转换为字典格式。
 
         Returns:
```

### Comparing `zillionare-backtest-0.4.12/backtest/web/accounts.py` & `zillionare_backtest-0.4.18/backtest/web/accounts.py`

 * *Files identical despite different names*

### Comparing `zillionare-backtest-0.4.12/backtest/web/interfaces.py` & `zillionare_backtest-0.4.18/backtest/web/interfaces.py`

 * *Files identical despite different names*

### Comparing `zillionare-backtest-0.4.12/pyproject.toml` & `zillionare_backtest-0.4.18/pyproject.toml`

 * *Files 9% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [tool]
 [tool.poetry]
 name = "zillionare-backtest"
-version = "0.4.12"
+version = "0.4.18"
 homepage = "https://github.com/zillionare/backtest"
 description = "zillionare backtest framework."
 authors = ["Aaron Yang <aaron_yang@jieyu.ai>"]
 readme = "README.md"
 license =  "MIT"
 classifiers=[
     'Development Status :: 2 - Pre-Alpha',
@@ -17,16 +17,17 @@
 packages = [
     { include = "backtest" },
     { include = "tests"},
 ]
 
 [[tool.poetry.source]]
 name = "ali"
-url = "https://mirrors.aliyun.com/pypi/simple/"
-secondary = true
+url = "https://mirrors.aliyun.com/pypi/simple"
+default = true
+secondary = false
 
 [tool.poetry.dependencies]
 python = ">=3.8,<3.9"
 fire = "0.4.0"
 
 black  = { version = "^22.3.0", optional = true}
 isort  = { version = "5.10.1", optional = true}
@@ -47,27 +48,26 @@
 toml = {version = "^0.10.2", optional = true}
 livereload = {version = "^2.6.3", optional = true}
 pyreadline = {version = "^2.1", optional = true}
 mike = { version="^1.1.2", optional=true}
 sanic = "^21.12.1"
 cfg4py = "^0.9.4"
 expiringdict = "^1.2.1"
-aioredis = "1.3.1"
+aioredis = "^2.0"
 zillionare-core-types = "^0.5.2"
 psutil = "^5.9.0"
 tqdm = "^4.63.0"
 pandas = "^1.4.1"
 sanic-testing = {version = "^0.8.2", optional = true}
 Jinja2 = {version = "~3.0", optional = true}
 tabulate = "^0.8.9"
-pyemit = "0.4.5"
 async-timeout = "^4.0"
-arrow = "^1.2.2"
-httpx = "^0.23.0"
-zillionare-omicron = {version = "^2.0.0.a42", allow-prereleases = true}
+zillionare-omicron = {version = "^2.0.0a57", allow-prereleases = true}
+pyemit = "^0.5.0"
+websockets = "<11.0"
 
 [tool.poetry.extras]
 test = [
     "pytest",
     "pytest-cov",
     "sanic-testing"
     ]
```

### Comparing `zillionare-backtest-0.4.12/tests/__init__.py` & `zillionare_backtest-0.4.18/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `zillionare-backtest-0.4.12/tests/common/test_helper.py` & `zillionare_backtest-0.4.18/tests/common/test_helper.py`

 * *Files identical despite different names*

### Comparing `zillionare-backtest-0.4.12/tests/data/bars_1d.pkl` & `zillionare_backtest-0.4.18/tests/data/bars_1d.pkl`

 * *Files identical despite different names*

### Comparing `zillionare-backtest-0.4.12/tests/data/bars_1m.pkl` & `zillionare_backtest-0.4.18/tests/data/bars_1m.pkl`

 * *Files identical despite different names*

### Comparing `zillionare-backtest-0.4.12/tests/data/hljh_1d.csv` & `zillionare_backtest-0.4.18/tests/data/hljh_1d.csv`

 * *Files identical despite different names*

### Comparing `zillionare-backtest-0.4.12/tests/data/hljh_1m.csv` & `zillionare_backtest-0.4.18/tests/data/hljh_1m.csv`

 * *Files identical despite different names*

### Comparing `zillionare-backtest-0.4.12/tests/data/limits.csv` & `zillionare_backtest-0.4.18/tests/data/limits.csv`

 * *Files identical despite different names*

### Comparing `zillionare-backtest-0.4.12/tests/data/tyst_1d.csv` & `zillionare_backtest-0.4.18/tests/data/tyst_1d.csv`

 * *Files identical despite different names*

### Comparing `zillionare-backtest-0.4.12/tests/data/tyst_1m.csv` & `zillionare_backtest-0.4.18/tests/data/tyst_1m.csv`

 * *Files identical despite different names*

### Comparing `zillionare-backtest-0.4.12/tests/data/validation.xlsx` & `zillionare_backtest-0.4.18/tests/data/validation.xlsx`

 * *Files identical despite different names*

### Comparing `zillionare-backtest-0.4.12/tests/feed/test_zillionarefeed.py` & `zillionare_backtest-0.4.18/tests/feed/test_zillionarefeed.py`

 * *Files identical despite different names*

### Comparing `zillionare-backtest-0.4.12/tests/test_app.py` & `zillionare_backtest-0.4.18/tests/test_app.py`

 * *Files identical despite different names*

### Comparing `zillionare-backtest-0.4.12/tests/test_cli.py` & `zillionare_backtest-0.4.18/tests/test_cli.py`

 * *Files identical despite different names*

### Comparing `zillionare-backtest-0.4.12/tests/trade/test_broker.py` & `zillionare_backtest-0.4.18/tests/trade/test_broker.py`

 * *Files 1% similar despite different names*

```diff
@@ -961,7 +961,36 @@
                 datetime.date(2022, 3, 14),
             ],
             list(actual.keys()),
         )
         np.testing.assert_array_almost_equal(
             [13.49, 12.37, 10.6], list(actual.values()), decimal=2
         )
+
+    @pytest.mark.skip(os.environ.get("IS_GITHUB"))
+    async def test_issue_with_local_omicron(self):
+        try:
+            config_dir = os.path.expanduser("~/zillionare/notebook")
+            cfg = cfg4py.init(config_dir)
+
+            await omicron.close()
+            await omicron.init()
+            await emit.start(emit.Engine.REDIS, start_server=True, dsn=cfg.redis.dsn)
+
+            self.ctx = get_app_context()
+            self.ctx.feed = ZillionareFeed()
+            await self.ctx.feed.init()
+
+            start = datetime.date(2022, 10, 1)
+            end = datetime.date(2022, 10, 31)
+
+            broker = Broker("test", 1_000_000, 1e-4, start, end)
+            await broker.buy(
+                "300539.XSHE", 9.26, 1000, datetime.datetime(2022, 10, 10, 9, 31)
+            )
+            await broker.sell(
+                "300539.XSHE", 8.98, 1000, datetime.datetime(2022, 10, 21, 9, 30)
+            )
+
+        finally:
+            await emit.stop()
+            await omicron.close()
```

### Comparing `zillionare-backtest-0.4.12/tests/web/test_interfaces.py` & `zillionare_backtest-0.4.18/tests/web/test_interfaces.py`

 * *Files 2% similar despite different names*

```diff
@@ -546,14 +546,15 @@
             },
         )
 
         self.assertEqual(response["security"], "002537.XSHE")
         self.assertAlmostEqual(response["price"], 9.420000076293945, 2)
         self.assertEqual(response["filled"], 500)
 
+        await post("stop_backtest", self.token, data={})
         response = await get("assets", self.token, start="2022-03-01", end="2022-03-14")
 
         exp = [
             1000039.53,
             1000514.53,
             1000594.53,
             1000084.53,
```

### Comparing `zillionare-backtest-0.4.12/PKG-INFO` & `zillionare_backtest-0.4.18/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: zillionare-backtest
-Version: 0.4.12
+Version: 0.4.18
 Summary: zillionare backtest framework.
 Home-page: https://github.com/zillionare/backtest
 License: MIT
 Author: Aaron Yang
 Author-email: aaron_yang@jieyu.ai
 Requires-Python: >=3.8,<3.9
 Classifier: Development Status :: 2 - Pre-Alpha
@@ -13,51 +13,50 @@
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.8
 Provides-Extra: dev
 Provides-Extra: doc
 Provides-Extra: test
-Requires-Dist: Jinja2 (>=3.0,<3.1); extra == "doc"
-Requires-Dist: aioredis (==1.3.1)
-Requires-Dist: arrow (>=1.2.2,<2.0.0)
+Requires-Dist: Jinja2 (>=3.0,<3.1) ; extra == "doc"
+Requires-Dist: aioredis (>=2.0,<3.0)
 Requires-Dist: async-timeout (>=4.0,<5.0)
-Requires-Dist: black (>=22.3.0,<23.0.0); extra == "dev"
+Requires-Dist: black (>=22.3.0,<23.0.0) ; extra == "dev"
 Requires-Dist: cfg4py (>=0.9.4,<0.10.0)
 Requires-Dist: expiringdict (>=1.2.1,<2.0.0)
 Requires-Dist: fire (==0.4.0)
-Requires-Dist: flake8 (==4.0.1); extra == "dev"
-Requires-Dist: flake8-docstrings (>=1.6.0,<2.0.0); extra == "dev"
-Requires-Dist: httpx (>=0.23.0,<0.24.0)
-Requires-Dist: isort (==5.10.1); extra == "dev"
-Requires-Dist: livereload (>=2.6.3,<3.0.0); extra == "doc"
-Requires-Dist: mike (>=1.1.2,<2.0.0); extra == "doc"
-Requires-Dist: mkdocs (>=1.2.3,<2.0.0); extra == "doc"
-Requires-Dist: mkdocs-autorefs (>=0.4.1,<0.5.0); extra == "doc"
-Requires-Dist: mkdocs-include-markdown-plugin (>=3.2.3,<4.0.0); extra == "doc"
-Requires-Dist: mkdocs-material (>=8.1.11,<9.0.0); extra == "doc"
+Requires-Dist: flake8 (==4.0.1) ; extra == "dev"
+Requires-Dist: flake8-docstrings (>=1.6.0,<2.0.0) ; extra == "dev"
+Requires-Dist: isort (==5.10.1) ; extra == "dev"
+Requires-Dist: livereload (>=2.6.3,<3.0.0) ; extra == "doc"
+Requires-Dist: mike (>=1.1.2,<2.0.0) ; extra == "doc"
+Requires-Dist: mkdocs (>=1.2.3,<2.0.0) ; extra == "doc"
+Requires-Dist: mkdocs-autorefs (>=0.4.1,<0.5.0) ; extra == "doc"
+Requires-Dist: mkdocs-include-markdown-plugin (>=3.2.3,<4.0.0) ; extra == "doc"
+Requires-Dist: mkdocs-material (>=8.1.11,<9.0.0) ; extra == "doc"
 Requires-Dist: mkdocs-material-extensions (>=1.0.3,<2.0.0)
-Requires-Dist: mkdocstrings (>=0.18.0,<0.19.0); extra == "doc"
+Requires-Dist: mkdocstrings (>=0.18.0,<0.19.0) ; extra == "doc"
 Requires-Dist: pandas (>=1.4.1,<2.0.0)
-Requires-Dist: pre-commit (>=2.17.0,<3.0.0); extra == "dev"
+Requires-Dist: pre-commit (>=2.17.0,<3.0.0) ; extra == "dev"
 Requires-Dist: psutil (>=5.9.0,<6.0.0)
-Requires-Dist: pyemit (==0.4.5)
+Requires-Dist: pyemit (>=0.5.0,<0.6.0)
 Requires-Dist: pyreadline (>=2.1,<3.0)
-Requires-Dist: pytest (>=7.0.1,<8.0.0); extra == "test"
-Requires-Dist: pytest-cov (>=3.0.0,<4.0.0); extra == "test"
+Requires-Dist: pytest (>=7.0.1,<8.0.0) ; extra == "test"
+Requires-Dist: pytest-cov (>=3.0.0,<4.0.0) ; extra == "test"
 Requires-Dist: sanic (>=21.12.1,<22.0.0)
-Requires-Dist: sanic-testing (>=0.8.2,<0.9.0); extra == "test"
+Requires-Dist: sanic-testing (>=0.8.2,<0.9.0) ; extra == "test"
 Requires-Dist: tabulate (>=0.8.9,<0.9.0)
-Requires-Dist: toml (>=0.10.2,<0.11.0); extra == "dev"
-Requires-Dist: tox (>=3.24.5,<4.0.0); extra == "dev"
+Requires-Dist: toml (>=0.10.2,<0.11.0) ; extra == "dev"
+Requires-Dist: tox (>=3.24.5,<4.0.0) ; extra == "dev"
 Requires-Dist: tqdm (>=4.63.0,<5.0.0)
-Requires-Dist: twine (>=3.8.0,<4.0.0); extra == "dev"
-Requires-Dist: virtualenv (>=20.13.1,<21.0.0); extra == "dev"
+Requires-Dist: twine (>=3.8.0,<4.0.0) ; extra == "dev"
+Requires-Dist: virtualenv (>=20.13.1,<21.0.0) ; extra == "dev"
+Requires-Dist: websockets (<11.0)
 Requires-Dist: zillionare-core-types (>=0.5.2,<0.6.0)
-Requires-Dist: zillionare-omicron (>=2.0.0.a42,<3.0.0)
+Requires-Dist: zillionare-omicron (>=2.0.0a57,<3.0.0)
 Description-Content-Type: text/markdown
 
 [![Version](http://img.shields.io/pypi/v/zillionare-backtest?color=brightgreen)](https://pypi.python.org/pypi/zillionare-backtest)
 [![CI Status](https://github.com/zillionare/backtesting/actions/workflows/release.yml/badge.svg)](https://github.com/zillionare/backtesting)
 [![Code Coverage](https://img.shields.io/codecov/c/github/zillionare/backtesting)](https://app.codecov.io/gh/zillionare/backtesting)
 [![Downloads](https://pepy.tech/badge/zillionare-backtest)](https://pepy.tech/project/zillionare-backtest)
 [![License](https://img.shields.io/badge/License-MIT.svg)](https://opensource.org/licenses/MIT)
@@ -73,14 +72,20 @@
 
 这种设计意味着，您的策略可以不使用大富翁数据框架，甚至可以不使用zillionare-trader-client（您可以自定义一套接口并实现，使之能同时适配您的交易接口和backtest接口）。因此，您的策略可以在任何时候，切换到最适合的量化框架。
 
 # 功能
 ## 账户管理
 当您开始回测时，先通过[start_backtest][backtest.web.interfaces.start_backtest]来创建一个账户。在知道该账户的`name`与`token`的情况下，您可以在随后通过[delete_accounts][backtest.web.interfaces.delete_accounts]来删除账户。
 
+在回测完成时，请记得调用stop_backtest。
+
+在回测完成时，stop_backtest会将资产表更新到回测结束日（否则，只更新到最后一次交易当天，因为服务器完全由客户端来驱动，自己没有时间概念）。但并不会对当前持仓进行卖出操作，原因是：
+1. 卖出操作将修改transactions表。而新增的transaction并不是策略触发的
+2. 不利于评估策略的真实情况。如果在回测期出现仅有一笔真实交易，其它都是被终末强平的话，那么此次回测实际上可能在时间上、或者策略周期上没有选好。如果回测系统进行强平，就可能掩盖这种事实。
+3. 在回测终末期，可能存在股票因跌停而无法卖出的情况；或者股票停牌中，无法卖出。这些情况下，模拟卖出也有难度。
 ## 交易撮合
 
 您可以通过[buy][backtest.web.interfaces.buy], [market_buy][backtest.web.interfaces.market_buy], [sell][backtest.web.interfaces.sell], [market_sell][backtest.web.interfaces.market_sell]和[sell_percent][backtest.web.interfaces.sell_percent]来进行交易。
 
 ## 状态跟踪
 
 您可以通过[info][backtest.web.interfaces.info]来查看账户的基本信息，比如当前总资产、持仓、本金、盈利等。您还可以通过[positions][backtest.web.interfaces.positions]、[bills][backtest.web.interfaces.bills]来查看账户的持仓、交易历史记录
```

