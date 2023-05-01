# Comparing `tmp/express-option-chain-1.0.5.tar.gz` & `tmp/express-option-chain-1.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "express-option-chain-1.0.5.tar", last modified: Tue Feb 14 21:37:49 2023, max compression
+gzip compressed data, was "express-option-chain-1.0.6.tar", last modified: Mon May  1 00:18:08 2023, max compression
```

## Comparing `express-option-chain-1.0.5.tar` & `express-option-chain-1.0.6.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 prramakrishn   (502) staff       (20)        0 2023-02-14 21:37:49.835573 express-option-chain-1.0.5/
--rw-r--r--   0 prramakrishn   (502) staff       (20)     1066 2023-02-14 21:24:15.000000 express-option-chain-1.0.5/LICENSE
--rw-r--r--   0 prramakrishn   (502) staff       (20)    18597 2023-02-14 21:37:49.835248 express-option-chain-1.0.5/PKG-INFO
--rw-r--r--   0 prramakrishn   (502) staff       (20)    16692 2023-02-14 21:35:37.000000 express-option-chain-1.0.5/README.md
--rw-r--r--   0 prramakrishn   (502) staff       (20)      977 2023-02-14 21:37:25.000000 express-option-chain-1.0.5/pyproject.toml
--rw-r--r--   0 prramakrishn   (502) staff       (20)       38 2023-02-14 21:37:49.835626 express-option-chain-1.0.5/setup.cfg
-drwxr-xr-x   0 prramakrishn   (502) staff       (20)        0 2023-02-14 21:37:49.825786 express-option-chain-1.0.5/src/
--rw-r--r--   0 prramakrishn   (502) staff       (20)        0 2023-01-29 21:09:29.000000 express-option-chain-1.0.5/src/__init__.py
-drwxr-xr-x   0 prramakrishn   (502) staff       (20)        0 2023-02-14 21:37:49.827990 express-option-chain-1.0.5/src/express_option_chain.egg-info/
--rw-r--r--   0 prramakrishn   (502) staff       (20)    18597 2023-02-14 21:37:49.000000 express-option-chain-1.0.5/src/express_option_chain.egg-info/PKG-INFO
--rw-r--r--   0 prramakrishn   (502) staff       (20)      848 2023-02-14 21:37:49.000000 express-option-chain-1.0.5/src/express_option_chain.egg-info/SOURCES.txt
--rw-r--r--   0 prramakrishn   (502) staff       (20)        1 2023-02-14 21:37:49.000000 express-option-chain-1.0.5/src/express_option_chain.egg-info/dependency_links.txt
--rw-r--r--   0 prramakrishn   (502) staff       (20)       27 2023-02-14 21:37:49.000000 express-option-chain-1.0.5/src/express_option_chain.egg-info/requires.txt
--rw-r--r--   0 prramakrishn   (502) staff       (20)       28 2023-02-14 21:37:49.000000 express-option-chain-1.0.5/src/express_option_chain.egg-info/top_level.txt
-drwxr-xr-x   0 prramakrishn   (502) staff       (20)        0 2023-02-14 21:37:49.832461 express-option-chain-1.0.5/src/expressoptionchain/
--rw-r--r--   0 prramakrishn   (502) staff       (20)        0 2023-02-13 11:10:01.000000 express-option-chain-1.0.5/src/expressoptionchain/__init__.py
-drwxr-xr-x   0 prramakrishn   (502) staff       (20)        0 2023-02-14 21:37:49.834744 express-option-chain-1.0.5/src/expressoptionchain/examples/
--rw-r--r--   0 prramakrishn   (502) staff       (20)        0 2023-02-13 11:10:01.000000 express-option-chain-1.0.5/src/expressoptionchain/examples/__init__.py
--rw-r--r--   0 prramakrishn   (502) staff       (20)      987 2023-02-14 17:57:57.000000 express-option-chain-1.0.5/src/expressoptionchain/examples/advanced_usage.py
--rw-r--r--   0 prramakrishn   (502) staff       (20)      450 2023-02-14 18:43:28.000000 express-option-chain-1.0.5/src/expressoptionchain/examples/fetch_option_chain.py
--rw-r--r--   0 prramakrishn   (502) staff       (20)     2487 2023-02-14 17:57:57.000000 express-option-chain-1.0.5/src/expressoptionchain/examples/runner.py
--rw-r--r--   0 prramakrishn   (502) staff       (20)     1728 2023-02-14 19:04:55.000000 express-option-chain-1.0.5/src/expressoptionchain/examples/start_option_chain_process.py
--rw-r--r--   0 prramakrishn   (502) staff       (20)      173 2023-02-14 17:24:12.000000 express-option-chain-1.0.5/src/expressoptionchain/exceptions.py
--rw-r--r--   0 prramakrishn   (502) staff       (20)      914 2023-02-14 21:25:26.000000 express-option-chain-1.0.5/src/expressoptionchain/helper.py
--rw-r--r--   0 prramakrishn   (502) staff       (20)    14272 2023-02-14 12:35:46.000000 express-option-chain-1.0.5/src/expressoptionchain/instrument_manager.py
--rw-r--r--   0 prramakrishn   (502) staff       (20)     1261 2023-02-14 20:11:35.000000 express-option-chain-1.0.5/src/expressoptionchain/kite_connector.py
--rw-r--r--   0 prramakrishn   (502) staff       (20)     7378 2023-02-14 12:35:46.000000 express-option-chain-1.0.5/src/expressoptionchain/option_chain.py
--rw-r--r--   0 prramakrishn   (502) staff       (20)    14516 2023-02-14 20:11:35.000000 express-option-chain-1.0.5/src/expressoptionchain/option_stream.py
--rw-r--r--   0 prramakrishn   (502) staff       (20)      409 2023-02-14 21:37:09.000000 express-option-chain-1.0.5/src/expressoptionchain/redis_helper.py
+drwxr-xr-x   0 prramakrishn   (502) staff       (20)        0 2023-05-01 00:18:08.897921 express-option-chain-1.0.6/
+-rw-r--r--   0 prramakrishn   (502) staff       (20)     1066 2023-02-14 21:24:15.000000 express-option-chain-1.0.6/LICENSE
+-rw-r--r--   0 prramakrishn   (502) staff       (20)    18514 2023-05-01 00:18:08.897586 express-option-chain-1.0.6/PKG-INFO
+-rw-r--r--   0 prramakrishn   (502) staff       (20)    16725 2023-05-01 00:14:47.000000 express-option-chain-1.0.6/README.md
+-rw-r--r--   0 prramakrishn   (502) staff       (20)      861 2023-05-01 00:13:16.000000 express-option-chain-1.0.6/pyproject.toml
+-rw-r--r--   0 prramakrishn   (502) staff       (20)       38 2023-05-01 00:18:08.897987 express-option-chain-1.0.6/setup.cfg
+drwxr-xr-x   0 prramakrishn   (502) staff       (20)        0 2023-05-01 00:18:08.886501 express-option-chain-1.0.6/src/
+-rw-r--r--   0 prramakrishn   (502) staff       (20)        0 2023-01-29 21:09:29.000000 express-option-chain-1.0.6/src/__init__.py
+drwxr-xr-x   0 prramakrishn   (502) staff       (20)        0 2023-05-01 00:18:08.889459 express-option-chain-1.0.6/src/express_option_chain.egg-info/
+-rw-r--r--   0 prramakrishn   (502) staff       (20)    18514 2023-05-01 00:18:08.000000 express-option-chain-1.0.6/src/express_option_chain.egg-info/PKG-INFO
+-rw-r--r--   0 prramakrishn   (502) staff       (20)      848 2023-05-01 00:18:08.000000 express-option-chain-1.0.6/src/express_option_chain.egg-info/SOURCES.txt
+-rw-r--r--   0 prramakrishn   (502) staff       (20)        1 2023-05-01 00:18:08.000000 express-option-chain-1.0.6/src/express_option_chain.egg-info/dependency_links.txt
+-rw-r--r--   0 prramakrishn   (502) staff       (20)       27 2023-05-01 00:18:08.000000 express-option-chain-1.0.6/src/express_option_chain.egg-info/requires.txt
+-rw-r--r--   0 prramakrishn   (502) staff       (20)       28 2023-05-01 00:18:08.000000 express-option-chain-1.0.6/src/express_option_chain.egg-info/top_level.txt
+drwxr-xr-x   0 prramakrishn   (502) staff       (20)        0 2023-05-01 00:18:08.894159 express-option-chain-1.0.6/src/expressoptionchain/
+-rw-r--r--   0 prramakrishn   (502) staff       (20)        0 2023-02-13 11:10:01.000000 express-option-chain-1.0.6/src/expressoptionchain/__init__.py
+drwxr-xr-x   0 prramakrishn   (502) staff       (20)        0 2023-05-01 00:18:08.896949 express-option-chain-1.0.6/src/expressoptionchain/examples/
+-rw-r--r--   0 prramakrishn   (502) staff       (20)        0 2023-02-13 11:10:01.000000 express-option-chain-1.0.6/src/expressoptionchain/examples/__init__.py
+-rw-r--r--   0 prramakrishn   (502) staff       (20)      987 2023-02-14 17:57:57.000000 express-option-chain-1.0.6/src/expressoptionchain/examples/advanced_usage.py
+-rw-r--r--   0 prramakrishn   (502) staff       (20)      450 2023-02-14 18:43:28.000000 express-option-chain-1.0.6/src/expressoptionchain/examples/fetch_option_chain.py
+-rw-r--r--   0 prramakrishn   (502) staff       (20)     2492 2023-05-01 00:07:53.000000 express-option-chain-1.0.6/src/expressoptionchain/examples/runner.py
+-rw-r--r--   0 prramakrishn   (502) staff       (20)     1728 2023-02-14 19:04:55.000000 express-option-chain-1.0.6/src/expressoptionchain/examples/start_option_chain_process.py
+-rw-r--r--   0 prramakrishn   (502) staff       (20)      173 2023-02-14 17:24:12.000000 express-option-chain-1.0.6/src/expressoptionchain/exceptions.py
+-rw-r--r--   0 prramakrishn   (502) staff       (20)      914 2023-02-14 21:25:26.000000 express-option-chain-1.0.6/src/expressoptionchain/helper.py
+-rw-r--r--   0 prramakrishn   (502) staff       (20)    14449 2023-05-01 00:05:24.000000 express-option-chain-1.0.6/src/expressoptionchain/instrument_manager.py
+-rw-r--r--   0 prramakrishn   (502) staff       (20)     1261 2023-02-14 20:11:35.000000 express-option-chain-1.0.6/src/expressoptionchain/kite_connector.py
+-rw-r--r--   0 prramakrishn   (502) staff       (20)     7378 2023-02-14 12:35:46.000000 express-option-chain-1.0.6/src/expressoptionchain/option_chain.py
+-rw-r--r--   0 prramakrishn   (502) staff       (20)    14516 2023-04-30 23:57:00.000000 express-option-chain-1.0.6/src/expressoptionchain/option_stream.py
+-rw-r--r--   0 prramakrishn   (502) staff       (20)      409 2023-02-14 21:37:09.000000 express-option-chain-1.0.6/src/expressoptionchain/redis_helper.py
```

### Comparing `express-option-chain-1.0.5/LICENSE` & `express-option-chain-1.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `express-option-chain-1.0.5/PKG-INFO` & `express-option-chain-1.0.6/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: express-option-chain
-Version: 1.0.5
-Summary: This library uses Kite Connect APIs to fetch the option chain of all the derivatives present in Indian stock market. It supports all the exchanges including NFO, MCX, CDS and BCD. It also provides API to fetch the option chain of an asset.
+Version: 1.0.6
+Summary: This library utilizes Kite Connect APIs to fetch the option chain of all the derivatives traded in the Indian stock market.
 Author-email: Prajwal Ramakrishna <prajwaldr9@gmail.com>
 License: Copyright (c) 2023, Prajwal Ramakrishna.
         
         Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the "Software"), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
         
         The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.
         
@@ -19,15 +19,15 @@
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Express Option Chain - Option Chain Stream for Indian Stock Market built with Kite APIs
 
-This library utilizes Kite Connect APIs to fetch the option chain of all the derivatives traded in the Indian stock market. With support for all exchanges, including NFO, MCX, CDS, and BCD, comprehensive options chain data can be streamed effortlessly in real-time. The library provides a convenient API to fetch the option chain of the assets.
+This library utilizes Kite Connect APIs to fetch the Option Chain of all the derivatives traded in the Indian stock market. With support for all exchanges, including NFO, MCX, CDS, and BCD, comprehensive option chain data can be streamed effortlessly in real-time. The library provides a convenient API to fetch the option chain of the assets.
 
 Some major features are
 
 * ✅ Light weight
 * ⚡️ Optimized for speed - Uses parallel connections through Python Multiprocessing
 * 📈 Supports subscribing to all the derivatives across all exchanges (NFO for equity, MCX, CDS, BCD) in a single API
 * ⏱️ No considerable difference in execution time even when subscribed to all the symbols present in Indian exchanges -
@@ -534,9 +534,9 @@
 are stored in redis hash. Storage of ticks is handled by separate worker threads. Another worker thread calculates the
 option chain using the stored ticks.
 
 OptionChainFetcher class provides an interface to fetch the quotes stored in the database.
 
 ## Contact
 
-Feel free to contact me if you need any support regarding the usage of this library. If there are bugs, please create an
+Feel free to [contact me](https://github.com/pramakrishn) if you need any support regarding the usage of this library. If there are bugs, please create an
 issue in GitHub.
```

### Comparing `express-option-chain-1.0.5/README.md` & `express-option-chain-1.0.6/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # Express Option Chain - Option Chain Stream for Indian Stock Market built with Kite APIs
 
-This library utilizes Kite Connect APIs to fetch the option chain of all the derivatives traded in the Indian stock market. With support for all exchanges, including NFO, MCX, CDS, and BCD, comprehensive options chain data can be streamed effortlessly in real-time. The library provides a convenient API to fetch the option chain of the assets.
+This library utilizes Kite Connect APIs to fetch the Option Chain of all the derivatives traded in the Indian stock market. With support for all exchanges, including NFO, MCX, CDS, and BCD, comprehensive option chain data can be streamed effortlessly in real-time. The library provides a convenient API to fetch the option chain of the assets.
 
 Some major features are
 
 * ✅ Light weight
 * ⚡️ Optimized for speed - Uses parallel connections through Python Multiprocessing
 * 📈 Supports subscribing to all the derivatives across all exchanges (NFO for equity, MCX, CDS, BCD) in a single API
 * ⏱️ No considerable difference in execution time even when subscribed to all the symbols present in Indian exchanges -
@@ -511,9 +511,9 @@
 are stored in redis hash. Storage of ticks is handled by separate worker threads. Another worker thread calculates the
 option chain using the stored ticks.
 
 OptionChainFetcher class provides an interface to fetch the quotes stored in the database.
 
 ## Contact
 
-Feel free to contact me if you need any support regarding the usage of this library. If there are bugs, please create an
+Feel free to [contact me](https://github.com/pramakrishn) if you need any support regarding the usage of this library. If there are bugs, please create an
 issue in GitHub.
```

### Comparing `express-option-chain-1.0.5/pyproject.toml` & `express-option-chain-1.0.6/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -2,16 +2,16 @@
 
 [build-system]
 requires = ["setuptools>=61.0.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "express-option-chain"
-version = "1.0.5"
-description = "This library uses Kite Connect APIs to fetch the option chain of all the derivatives present in Indian stock market. It supports all the exchanges including NFO, MCX, CDS and BCD. It also provides API to fetch the option chain of an asset."
+version = "1.0.6"
+description = "This library utilizes Kite Connect APIs to fetch the option chain of all the derivatives traded in the Indian stock market."
 readme = "README.md"
 authors = [{ name = "Prajwal Ramakrishna", email = "prajwaldr9@gmail.com" }]
 license = { file = "LICENSE" }
 classifiers = [
     "License :: OSI Approved :: MIT License",
     "Programming Language :: Python",
     "Programming Language :: Python :: 3",
```

### Comparing `express-option-chain-1.0.5/src/express_option_chain.egg-info/PKG-INFO` & `express-option-chain-1.0.6/src/express_option_chain.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: express-option-chain
-Version: 1.0.5
-Summary: This library uses Kite Connect APIs to fetch the option chain of all the derivatives present in Indian stock market. It supports all the exchanges including NFO, MCX, CDS and BCD. It also provides API to fetch the option chain of an asset.
+Version: 1.0.6
+Summary: This library utilizes Kite Connect APIs to fetch the option chain of all the derivatives traded in the Indian stock market.
 Author-email: Prajwal Ramakrishna <prajwaldr9@gmail.com>
 License: Copyright (c) 2023, Prajwal Ramakrishna.
         
         Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the "Software"), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
         
         The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.
         
@@ -19,15 +19,15 @@
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Express Option Chain - Option Chain Stream for Indian Stock Market built with Kite APIs
 
-This library utilizes Kite Connect APIs to fetch the option chain of all the derivatives traded in the Indian stock market. With support for all exchanges, including NFO, MCX, CDS, and BCD, comprehensive options chain data can be streamed effortlessly in real-time. The library provides a convenient API to fetch the option chain of the assets.
+This library utilizes Kite Connect APIs to fetch the Option Chain of all the derivatives traded in the Indian stock market. With support for all exchanges, including NFO, MCX, CDS, and BCD, comprehensive option chain data can be streamed effortlessly in real-time. The library provides a convenient API to fetch the option chain of the assets.
 
 Some major features are
 
 * ✅ Light weight
 * ⚡️ Optimized for speed - Uses parallel connections through Python Multiprocessing
 * 📈 Supports subscribing to all the derivatives across all exchanges (NFO for equity, MCX, CDS, BCD) in a single API
 * ⏱️ No considerable difference in execution time even when subscribed to all the symbols present in Indian exchanges -
@@ -534,9 +534,9 @@
 are stored in redis hash. Storage of ticks is handled by separate worker threads. Another worker thread calculates the
 option chain using the stored ticks.
 
 OptionChainFetcher class provides an interface to fetch the quotes stored in the database.
 
 ## Contact
 
-Feel free to contact me if you need any support regarding the usage of this library. If there are bugs, please create an
+Feel free to [contact me](https://github.com/pramakrishn) if you need any support regarding the usage of this library. If there are bugs, please create an
 issue in GitHub.
```

### Comparing `express-option-chain-1.0.5/src/express_option_chain.egg-info/SOURCES.txt` & `express-option-chain-1.0.6/src/express_option_chain.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `express-option-chain-1.0.5/src/expressoptionchain/examples/advanced_usage.py` & `express-option-chain-1.0.6/src/expressoptionchain/examples/advanced_usage.py`

 * *Files identical despite different names*

### Comparing `express-option-chain-1.0.5/src/expressoptionchain/examples/runner.py` & `express-option-chain-1.0.6/src/expressoptionchain/examples/runner.py`

 * *Files 3% similar despite different names*

```diff
@@ -7,19 +7,20 @@
              datefmt='%Y-%m-%d %H:%M:%S')
 log = logging.getLogger(__name__)
 
 from expressoptionchain.helper import get_secrets
 
 if __name__ == '__main__':
     secrets = get_secrets()
-    expiry = '23-02-2023'
-    text = '''BANKNIFTY, AARTIIND, ABB, ABBOTINDIA, ABCAPITAL, ABFRL, ACC, ADANIENT, ADANIPORTS, ALKEM, AMBUJACEM, APOLLOHOSP, APOLLOTYRE, ASHOKLEY, ASIANPAINT, ASTRAL, ATUL, AUBANK, AUROPHARMA, AXISBANK, BAJAJ-AUTO, BAJAJFINSV, BAJFINANCE, BALKRISIND, BALRAMCHIN, BANDHANBNK, BANKBARODA, BATAINDIA, BEL, BERGEPAINT, BHARATFORG, BHARTIARTL, BHEL, BIOCON, BOSCHLTD, BPCL, BRITANNIA, BSOFT, CANBK, CANFINHOME, CHAMBLFERT, CHOLAFIN, CIPLA, COALINDIA, COFORGE, COLPAL, CONCOR, COROMANDEL, CROMPTON, CUB, CUMMINSIND, DABUR, DALBHARAT, DEEPAKNTR, DELTACORP, DIVISLAB, DIXON, DLF, DRREDDY, EICHERMOT, ESCORTS, EXIDEIND, FEDERALBNK, FSL, GAIL, GLENMARK, GMRINFRA, GNFC, GODREJCP, GODREJPROP, GRANULES, GRASIM, GUJGASLTD, HAL, HAVELLS, HCLTECH, HDFC, HDFCAMC, HDFCBANK, HDFCLIFE, HEROMOTOCO, HINDALCO, HINDCOPPER, HINDPETRO, HINDUNILVR, HONAUT, ICICIBANK, ICICIGI, ICICIPRULI, IDEA, IDFC, IDFCFIRSTB, IEX, IGL, INDHOTEL, INDIACEM, INDIAMART, INDIGO, INDUSINDBK, INDUSTOWER, INFY, INTELLECT, IOC, IPCALAB, IRCTC, ITC, JINDALSTEL, JKCEMENT, JSWSTEEL, JUBLFOOD, KOTAKBANK, L&TFH, LALPATHLAB, LAURUSLABS, LICHSGFIN, LT, LTIM, LTTS, LUPIN, M&M, M&MFIN, MANAPPURAM, MARICO, MARUTI, MCX, METROPOLIS, MFSL, MGL, MOTHERSON, MPHASIS, MRF, MUTHOOTFIN, NATIONALUM, NAUKRI, NAVINFLUOR, NESTLEIND, NMDC, NTPC, OBEROIRLTY, OFSS, ONGC, PAGEIND, PEL, PERSISTENT, PETRONET, PFC, PIDILITIND, PIIND, PNB, POLYCAB, POWERGRID, PVR, RAIN, RAMCOCEM, RBLBANK, RECLTD, RELIANCE, SAIL, SBICARD, SBILIFE, SBIN, SHREECEM, SHRIRAMFIN, SIEMENS, SRF, SUNPHARMA, SUNTV, SYNGENE, TATACHEM, TATACOMM, TATACONSUM, TATAMOTORS, TATAPOWER, TATASTEEL, TCS, TECHM, TITAN, TORNTPHARM, TORNTPOWER, TRENT, TVSMOTOR, UBL, ULTRACEMCO, UPL, VEDL, VOLTAS, WHIRLPOOL, WIPRO, ZEEL, ZYDUSLIFE'''
+    expiry = '25-05-2023'
+    text = '''BANKNIFTY, AARTIIND, ABB, ABBOTINDIA, ABCAPITAL, ABFRL, ACC, ADANIENT, ADANIPORTS, ALKEM, AMBUJACEM, APOLLOHOSP, APOLLOTYRE, ASHOKLEY, ASIANPAINT, ASTRAL, ATUL, AUBANK, AUROPHARMA, AXISBANK, BAJAJ-AUTO, BAJAJFINSV, BAJFINANCE, BALKRISIND, BALRAMCHIN, BANDHANBNK, BANKBARODA, BATAINDIA, BEL, BERGEPAINT, BHARATFORG, BHARTIARTL, BHEL, BIOCON, BOSCHLTD, BPCL, BRITANNIA, BSOFT, CANBK, CANFINHOME, CHAMBLFERT, CHOLAFIN, CIPLA, COALINDIA, COFORGE, COLPAL, CONCOR, COROMANDEL, CROMPTON, CUB, CUMMINSIND, DABUR, DALBHARAT, DEEPAKNTR, DELTACORP, DIVISLAB, DIXON, DLF, DRREDDY, EICHERMOT, ESCORTS, EXIDEIND, FEDERALBNK, GAIL, GLENMARK, GMRINFRA, GNFC, GODREJCP, GODREJPROP, GRANULES, GRASIM, GUJGASLTD, HAL, HAVELLS, HCLTECH, HDFC, HDFCAMC, HDFCBANK, HDFCLIFE, HEROMOTOCO, HINDALCO, HINDCOPPER, HINDPETRO, HINDUNILVR, ICICIBANK, ICICIGI, ICICIPRULI, IDEA, IDFC, IDFCFIRSTB, IEX, IGL, INDHOTEL, INDIACEM, INDIAMART, INDIGO, INDUSINDBK, INDUSTOWER, INFY, INTELLECT, IOC, IPCALAB, IRCTC, ITC, JINDALSTEL, JKCEMENT, JSWSTEEL, JUBLFOOD, KOTAKBANK, L&TFH, LALPATHLAB, LAURUSLABS, LICHSGFIN, LT, LTIM, LTTS, LUPIN, M&M, M&MFIN, MANAPPURAM, MARICO, MARUTI, MCX, METROPOLIS, MFSL, MGL, MOTHERSON, MPHASIS, MRF, MUTHOOTFIN, NATIONALUM, NAUKRI, NAVINFLUOR, NESTLEIND, NMDC, NTPC, OBEROIRLTY, OFSS, ONGC, PAGEIND, PEL, PERSISTENT, PETRONET, PFC, PIDILITIND, PIIND, PNB, POLYCAB, POWERGRID, PVR, RAIN, RAMCOCEM, RBLBANK, RECLTD, RELIANCE, SAIL, SBICARD, SBILIFE, SBIN, SHREECEM, SHRIRAMFIN, SIEMENS, SRF, SUNPHARMA, SUNTV, SYNGENE, TATACHEM, TATACOMM, TATACONSUM, TATAMOTORS, TATAPOWER, TATASTEEL, TCS, TECHM, TITAN, TORNTPHARM, TRENT, TVSMOTOR, UBL, ULTRACEMCO, UPL, VEDL, VOLTAS, WHIRLPOOL, WIPRO, ZEEL, ZYDUSLIFE'''
     symbols = []
     for item in text.split(', '):
         symbols.append(f'NFO:{item}')
+    symbols.append(f'MCX:ZINC')
 
     # option stream should be started in main module
-    criteria = {'name': 'percentage', 'properties': {'value': 12.5}}
+    criteria = {'name': 'percentage', 'properties': {'value': 11}}
 
     stream = OptionStream(symbols, secrets, expiry=expiry, criteria=criteria)
     stream.start()
```

### Comparing `express-option-chain-1.0.5/src/expressoptionchain/examples/start_option_chain_process.py` & `express-option-chain-1.0.6/src/expressoptionchain/examples/start_option_chain_process.py`

 * *Files identical despite different names*

### Comparing `express-option-chain-1.0.5/src/expressoptionchain/helper.py` & `express-option-chain-1.0.6/src/expressoptionchain/helper.py`

 * *Files identical despite different names*

### Comparing `express-option-chain-1.0.5/src/expressoptionchain/instrument_manager.py` & `express-option-chain-1.0.6/src/expressoptionchain/instrument_manager.py`

 * *Files 1% similar despite different names*

```diff
@@ -226,14 +226,17 @@
                     # non equity options are not supported yet
                     all_tokens.extend(
                         self.get_token_info_for_trading_symbol(trading_symbol, expiry))
                     log.debug('trading symbol does not have nfo, hence adding all tokens')
                     continue
 
                 expiry_to_token_info_map = helper.get_hash_value(self.db, 'option_token_info', trading_symbol)
+                if not expiry_to_token_info_map:
+                    log.error(f'Trading symbol {trading_symbol} not found or is removed from fno')
+                    continue
                 if expiry not in expiry_to_token_info_map:
                     raise KiteInstrumentManagerException(
                         f'Expiry {expiry} token info not found for symbol {trading_symbol}')
                 nse_symbol = trading_symbol.replace('NFO', 'NSE')
                 ltp = self.db.hget('ltp', nse_symbol)
                 if not ltp:
                     # index options won't have ltp
```

### Comparing `express-option-chain-1.0.5/src/expressoptionchain/kite_connector.py` & `express-option-chain-1.0.6/src/expressoptionchain/kite_connector.py`

 * *Files identical despite different names*

### Comparing `express-option-chain-1.0.5/src/expressoptionchain/option_chain.py` & `express-option-chain-1.0.6/src/expressoptionchain/option_chain.py`

 * *Files identical despite different names*

### Comparing `express-option-chain-1.0.5/src/expressoptionchain/option_stream.py` & `express-option-chain-1.0.6/src/expressoptionchain/option_stream.py`

 * *Files identical despite different names*

