# Comparing `tmp/fireblocks_defi_sdk-1.0.2.tar.gz` & `tmp/fireblocks_defi_sdk-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fireblocks_defi_sdk-1.0.2.tar", last modified: Thu Jan 12 17:58:29 2023, max compression
+gzip compressed data, was "fireblocks_defi_sdk-1.1.0.tar", last modified: Mon May  1 08:29:05 2023, max compression
```

## Comparing `fireblocks_defi_sdk-1.0.2.tar` & `fireblocks_defi_sdk-1.1.0.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-12 17:58:29.124620 fireblocks_defi_sdk-1.0.2/
--rw-r--r--   0 runner    (1001) docker     (123)     1067 2023-01-12 17:58:05.000000 fireblocks_defi_sdk-1.0.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      949 2023-01-12 17:58:29.124620 fireblocks_defi_sdk-1.0.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1623 2023-01-12 17:58:05.000000 fireblocks_defi_sdk-1.0.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-12 17:58:29.120620 fireblocks_defi_sdk-1.0.2/fireblocks_defi_sdk.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      949 2023-01-12 17:58:29.000000 fireblocks_defi_sdk-1.0.2/fireblocks_defi_sdk.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      993 2023-01-12 17:58:29.000000 fireblocks_defi_sdk-1.0.2/fireblocks_defi_sdk.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-01-12 17:58:29.000000 fireblocks_defi_sdk-1.0.2/fireblocks_defi_sdk.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       36 2023-01-12 17:58:29.000000 fireblocks_defi_sdk-1.0.2/fireblocks_defi_sdk.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-01-12 17:58:29.000000 fireblocks_defi_sdk-1.0.2/fireblocks_defi_sdk.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-12 17:58:29.120620 fireblocks_defi_sdk-1.0.2/fireblocks_defi_sdk_py/
--rw-r--r--   0 runner    (1001) docker     (123)      138 2023-01-12 17:58:05.000000 fireblocks_defi_sdk-1.0.2/fireblocks_defi_sdk_py/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      804 2023-01-12 17:58:05.000000 fireblocks_defi_sdk-1.0.2/fireblocks_defi_sdk_py/chain.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-12 17:58:29.120620 fireblocks_defi_sdk-1.0.2/fireblocks_defi_sdk_py/tokenization/
--rw-r--r--   0 runner    (1001) docker     (123)       97 2023-01-12 17:58:05.000000 fireblocks_defi_sdk-1.0.2/fireblocks_defi_sdk_py/tokenization/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-12 17:58:29.120620 fireblocks_defi_sdk-1.0.2/fireblocks_defi_sdk_py/tokenization/examples/
--rw-r--r--   0 runner    (1001) docker     (123)     3744 2023-01-12 17:58:05.000000 fireblocks_defi_sdk-1.0.2/fireblocks_defi_sdk_py/tokenization/examples/custom_token_example.py
--rw-r--r--   0 runner    (1001) docker     (123)     3701 2023-01-12 17:58:05.000000 fireblocks_defi_sdk-1.0.2/fireblocks_defi_sdk_py/tokenization/examples/erc20_example.py
--rw-r--r--   0 runner    (1001) docker     (123)     2000 2023-01-12 17:58:05.000000 fireblocks_defi_sdk-1.0.2/fireblocks_defi_sdk_py/tokenization/examples/multi_token_example.py
--rw-r--r--   0 runner    (1001) docker     (123)     2691 2023-01-12 17:58:05.000000 fireblocks_defi_sdk-1.0.2/fireblocks_defi_sdk_py/tokenization/examples/nft_example.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-12 17:58:29.124620 fireblocks_defi_sdk-1.0.2/fireblocks_defi_sdk_py/tokenization/tokens/
--rw-r--r--   0 runner    (1001) docker     (123)      132 2023-01-12 17:58:05.000000 fireblocks_defi_sdk-1.0.2/fireblocks_defi_sdk_py/tokenization/tokens/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2340 2023-01-12 17:58:05.000000 fireblocks_defi_sdk-1.0.2/fireblocks_defi_sdk_py/tokenization/tokens/base_token.py
--rw-r--r--   0 runner    (1001) docker     (123)      383 2023-01-12 17:58:05.000000 fireblocks_defi_sdk-1.0.2/fireblocks_defi_sdk_py/tokenization/tokens/custom_token.py
--rw-r--r--   0 runner    (1001) docker     (123)     6494 2023-01-12 17:58:05.000000 fireblocks_defi_sdk-1.0.2/fireblocks_defi_sdk_py/tokenization/tokens/erc1155.py
--rw-r--r--   0 runner    (1001) docker     (123)     6949 2023-01-12 17:58:05.000000 fireblocks_defi_sdk-1.0.2/fireblocks_defi_sdk_py/tokenization/tokens/erc721.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-12 17:58:29.124620 fireblocks_defi_sdk-1.0.2/fireblocks_defi_sdk_py/tokenization/utils/
--rw-r--r--   0 runner    (1001) docker     (123)    12914 2023-01-12 17:58:05.000000 fireblocks_defi_sdk-1.0.2/fireblocks_defi_sdk_py/tokenization/utils/helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)     5762 2023-01-12 17:58:05.000000 fireblocks_defi_sdk-1.0.2/fireblocks_defi_sdk_py/web3_bridge.py
--rw-r--r--   0 runner    (1001) docker     (123)       79 2023-01-12 17:58:29.124620 fireblocks_defi_sdk-1.0.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1414 2023-01-12 17:58:18.000000 fireblocks_defi_sdk-1.0.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 08:29:05.148074 fireblocks_defi_sdk-1.1.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1067 2023-05-01 08:28:51.000000 fireblocks_defi_sdk-1.1.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      949 2023-05-01 08:29:05.148074 fireblocks_defi_sdk-1.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1825 2023-05-01 08:28:51.000000 fireblocks_defi_sdk-1.1.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 08:29:05.148074 fireblocks_defi_sdk-1.1.0/fireblocks_defi_sdk.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      949 2023-05-01 08:29:05.000000 fireblocks_defi_sdk-1.1.0/fireblocks_defi_sdk.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      993 2023-05-01 08:29:05.000000 fireblocks_defi_sdk-1.1.0/fireblocks_defi_sdk.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-01 08:29:05.000000 fireblocks_defi_sdk-1.1.0/fireblocks_defi_sdk.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       35 2023-05-01 08:29:05.000000 fireblocks_defi_sdk-1.1.0/fireblocks_defi_sdk.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-05-01 08:29:05.000000 fireblocks_defi_sdk-1.1.0/fireblocks_defi_sdk.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 08:29:05.148074 fireblocks_defi_sdk-1.1.0/fireblocks_defi_sdk_py/
+-rw-r--r--   0 runner    (1001) docker     (123)      138 2023-05-01 08:28:51.000000 fireblocks_defi_sdk-1.1.0/fireblocks_defi_sdk_py/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      804 2023-05-01 08:28:51.000000 fireblocks_defi_sdk-1.1.0/fireblocks_defi_sdk_py/chain.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 08:29:05.148074 fireblocks_defi_sdk-1.1.0/fireblocks_defi_sdk_py/tokenization/
+-rw-r--r--   0 runner    (1001) docker     (123)       97 2023-05-01 08:28:51.000000 fireblocks_defi_sdk-1.1.0/fireblocks_defi_sdk_py/tokenization/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 08:29:05.148074 fireblocks_defi_sdk-1.1.0/fireblocks_defi_sdk_py/tokenization/examples/
+-rw-r--r--   0 runner    (1001) docker     (123)     3738 2023-05-01 08:28:51.000000 fireblocks_defi_sdk-1.1.0/fireblocks_defi_sdk_py/tokenization/examples/custom_token_example.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3697 2023-05-01 08:28:51.000000 fireblocks_defi_sdk-1.1.0/fireblocks_defi_sdk_py/tokenization/examples/erc20_example.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2005 2023-05-01 08:28:51.000000 fireblocks_defi_sdk-1.1.0/fireblocks_defi_sdk_py/tokenization/examples/multi_token_example.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2686 2023-05-01 08:28:51.000000 fireblocks_defi_sdk-1.1.0/fireblocks_defi_sdk_py/tokenization/examples/nft_example.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 08:29:05.148074 fireblocks_defi_sdk-1.1.0/fireblocks_defi_sdk_py/tokenization/tokens/
+-rw-r--r--   0 runner    (1001) docker     (123)      132 2023-05-01 08:28:51.000000 fireblocks_defi_sdk-1.1.0/fireblocks_defi_sdk_py/tokenization/tokens/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2344 2023-05-01 08:28:51.000000 fireblocks_defi_sdk-1.1.0/fireblocks_defi_sdk_py/tokenization/tokens/base_token.py
+-rw-r--r--   0 runner    (1001) docker     (123)      385 2023-05-01 08:28:51.000000 fireblocks_defi_sdk-1.1.0/fireblocks_defi_sdk_py/tokenization/tokens/custom_token.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6518 2023-05-01 08:28:51.000000 fireblocks_defi_sdk-1.1.0/fireblocks_defi_sdk_py/tokenization/tokens/erc1155.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6977 2023-05-01 08:28:51.000000 fireblocks_defi_sdk-1.1.0/fireblocks_defi_sdk_py/tokenization/tokens/erc721.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 08:29:05.148074 fireblocks_defi_sdk-1.1.0/fireblocks_defi_sdk_py/tokenization/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)    12914 2023-05-01 08:28:51.000000 fireblocks_defi_sdk-1.1.0/fireblocks_defi_sdk_py/tokenization/utils/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5696 2023-05-01 08:28:51.000000 fireblocks_defi_sdk-1.1.0/fireblocks_defi_sdk_py/web3_bridge.py
+-rw-r--r--   0 runner    (1001) docker     (123)       79 2023-05-01 08:29:05.148074 fireblocks_defi_sdk-1.1.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1413 2023-05-01 08:28:57.000000 fireblocks_defi_sdk-1.1.0/setup.py
```

### Comparing `fireblocks_defi_sdk-1.0.2/LICENSE` & `fireblocks_defi_sdk-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `fireblocks_defi_sdk-1.0.2/PKG-INFO` & `fireblocks_defi_sdk-1.1.0/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: fireblocks_defi_sdk
-Version: 1.0.2
+Version: 1.1.0
 Summary: fireblocks_defi_sdk_py
 Home-page: https://github.com/fireblocks/fireblocks-defi-sdk-py
-Download-URL: https://github.com/fireblocks/fireblocks-defi-sdk-py/archive/refs/tags/1.0.2.tar.gz
+Download-URL: https://github.com/fireblocks/fireblocks-defi-sdk-py/archive/refs/tags/1.1.0.tar.gz
 Author: Fireblocks
 Author-email: fireblocks@fireblocks.com
 License: MIT
 Keywords: FIREBLOCKS,DeFi,SDK,PYTHON
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
```

### Comparing `fireblocks_defi_sdk-1.0.2/README.md` & `fireblocks_defi_sdk-1.1.0/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -1,7 +1,10 @@
+## Updates
+Check out our new SDK [Local-JSON-RPC](https://github.com/fireblocks/fireblocks-json-rpc) for an improved developer experience for using Python to interact with EVM chains using Fireblocks.
+
 # Fireblocks Python DeFi SDK
 [![PyPI version](https://badge.fury.io/py/fireblocks-defi-sdk.svg)](https://badge.fury.io/py/fireblocks-defi-sdk)
 
 The Fireblocks Python DeFi SDK provides an interoperability layer between Fireblocks Smart Contract API and common DeFi libraries.
 For more information on Fireblocks Smart Contract API and automating DeFi workflows on Fireblocks [read here](https://support.fireblocks.io/hc/en-us/articles/360017709160-Fireblocks-Smart-Contract-API).
 
 Please email us at support@fireblocks.com if you have questions or feedback.
```

### Comparing `fireblocks_defi_sdk-1.0.2/fireblocks_defi_sdk.egg-info/PKG-INFO` & `fireblocks_defi_sdk-1.1.0/fireblocks_defi_sdk.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: fireblocks-defi-sdk
-Version: 1.0.2
+Version: 1.1.0
 Summary: fireblocks_defi_sdk_py
 Home-page: https://github.com/fireblocks/fireblocks-defi-sdk-py
-Download-URL: https://github.com/fireblocks/fireblocks-defi-sdk-py/archive/refs/tags/1.0.2.tar.gz
+Download-URL: https://github.com/fireblocks/fireblocks-defi-sdk-py/archive/refs/tags/1.1.0.tar.gz
 Author: Fireblocks
 Author-email: fireblocks@fireblocks.com
 License: MIT
 Keywords: FIREBLOCKS,DeFi,SDK,PYTHON
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
```

### Comparing `fireblocks_defi_sdk-1.0.2/fireblocks_defi_sdk.egg-info/SOURCES.txt` & `fireblocks_defi_sdk-1.1.0/fireblocks_defi_sdk.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `fireblocks_defi_sdk-1.0.2/fireblocks_defi_sdk_py/chain.py` & `fireblocks_defi_sdk-1.1.0/fireblocks_defi_sdk_py/chain.py`

 * *Files identical despite different names*

### Comparing `fireblocks_defi_sdk-1.0.2/fireblocks_defi_sdk_py/tokenization/examples/custom_token_example.py` & `fireblocks_defi_sdk-1.1.0/fireblocks_defi_sdk_py/tokenization/examples/custom_token_example.py`

 * *Files 12% similar despite different names*

```diff
@@ -10,49 +10,49 @@
 VAULT_ID, SECONDARY_VAULT_ID = "0", "2"
 CONTRACT_ADDRESS = ""
 WHITELISTED_CONTRACT_UUID = ""  # This is the Fireblocks UUID of the whitelisted address.
 
 FILE_PATH, MODE = "some/path/to/my/contract", "r"
 
 if __name__ == "__main__":
-    # We start by building a bridge to the Ropsten network, including initiating a CustomToken object which will
+    # We start by building a bridge to the Goerli network, including initiating a CustomToken object which will
     # represent our custom contract. In order to initiate a CustomToken, we will need a contract ABI. This can be read
     # from another file, passed as a variable declared locally, or fetched from EtherScan using fetch_abi(address). We
     # will use the first.
-    ropsten_bridge = Web3Bridge(SDK, VAULT_ID, CONTRACT_ADDRESS, Chain.ROPSTEN, WHITELISTED_CONTRACT_UUID)
+    goerli_bridge = Web3Bridge(SDK, VAULT_ID, Chain.GOERLI, CONTRACT_ADDRESS, WHITELISTED_CONTRACT_UUID)
     with open(FILE_PATH, MODE) as file:
         contract_abi = file.read()
-    custom_contract_bridge = CustomToken(ropsten_bridge, contract_abi)
+    custom_contract_bridge = CustomToken(goerli_bridge, contract_abi)
 
     # Let's assume our ABI holds a transferOwnership write function, and a contractOwner function (returning a boolean).
     # We will first validate we own the contract and then transfer it to another vault in our account.
-    checked_address = custom_contract_bridge.web_provider.toChecksumAddress(custom_contract_bridge.wallet_address)
+    checked_address = custom_contract_bridge.web_provider.to_checksum_address(custom_contract_bridge.wallet_address)
     if custom_contract_bridge.call_read_function("contractOwner", checked_address):
         # We will initiate another bridge, as we will need the wallet address, and we will later on transfer it back.
-        secondary_ropsten_bridge = Web3Bridge(SDK, SECONDARY_VAULT_ID, CONTRACT_ADDRESS, Chain.ROPSTEN,
-                                              WHITELISTED_CONTRACT_UUID)
-        secondary_contract_bridge = CustomToken(secondary_ropsten_bridge, contract_abi)
+        secondary_goerli_brdige = Web3Bridge(SDK, SECONDARY_VAULT_ID, Chain.GOERLI, CONTRACT_ADDRESS,
+                                             WHITELISTED_CONTRACT_UUID)
+        secondary_contract_bridge = CustomToken(secondary_goerli_brdige, contract_abi)
         building_params = {"from": checked_address}
-        secondary_address = secondary_contract_bridge.web_provider.toChecksumAddress(
+        secondary_address = secondary_contract_bridge.web_provider.to_checksum_address(
             secondary_contract_bridge.wallet_address)
         transfer_ownership_raw_transaction = custom_contract_bridge. \
             call_write_function("transferOwnership",
                                 secondary_address,
                                 building_params=building_params)
 
         transfer_ownership_transaction = custom_contract_bridge.submit_transaction(transfer_ownership_raw_transaction)
-        if ropsten_bridge.check_tx_is_completed(transfer_ownership_transaction['id']) == TRANSACTION_STATUS_COMPLETED:
+        if goerli_bridge.check_tx_is_completed(transfer_ownership_transaction['id']) == TRANSACTION_STATUS_COMPLETED:
             print("Successfully transferred ownership from first wallet to the second one.")
             # We will now transfer the ownership back to our original wallet.
             building_params['from'] = secondary_address
             ownership_raw_transaction = secondary_contract_bridge. \
                 call_write_function("transferOwnership",
                                     checked_address,
                                     building_params=building_params)
             ownership_transaction = secondary_contract_bridge.submit_transaction(ownership_raw_transaction, "Returning")
-            if secondary_ropsten_bridge.check_tx_is_completed(ownership_transaction['id']) == \
+            if secondary_goerli_brdige.check_tx_is_completed(ownership_transaction['id']) == \
                     TRANSACTION_STATUS_COMPLETED:
                 print("Successfully transferred ownership from second wallet to the first one.")
             else:
                 print("Failed transferring ownership from the second wallet to the first.")
         else:
             print("Failed transferring ownership from the first wallet to the second.")
```

### Comparing `fireblocks_defi_sdk-1.0.2/fireblocks_defi_sdk_py/tokenization/examples/erc20_example.py` & `fireblocks_defi_sdk-1.1.0/fireblocks_defi_sdk_py/tokenization/examples/erc20_example.py`

 * *Files 4% similar despite different names*

```diff
@@ -9,49 +9,49 @@
 SDK = FireblocksSDK(API_SECRET, API_KEY)
 VAULT_ID = "0"
 CONTRACT_ADDRESS = ""
 RECEIVER_ADDRESS = ""
 TOKEN_AMOUNT = 10
 
 if __name__ == "__main__":
-    # We start by building a bridge to the Ropsten network, including initiating a CustomToken object which will
+    # We start by building a bridge to the Goerli network, including initiating a CustomToken object which will
     # represent our ERC20 contract. In order to initiate a CustomToken, we will need a contract ABI. This can be read
     # from another file, passed as a variable declared locally, or fetched from EtherScan using fetch_abi(address). We
     # will use the latter.
-    ropsten_bridge = Web3Bridge(SDK, VAULT_ID, CONTRACT_ADDRESS, Chain.ROPSTEN)
+    goerli_bridge = Web3Bridge(SDK, VAULT_ID, Chain.GOERLI, CONTRACT_ADDRESS)
     contract_abi = fetch_abi(CONTRACT_ADDRESS)
-    erc20_contract_bridge = CustomToken(ropsten_bridge, contract_abi)
+    erc20_contract_bridge = CustomToken(goerli_bridge, contract_abi)
 
     # We build functions through passing the function name exactly as it appears on the ABI, following by its arguments.
     # It's important to differentiate between a read (view) and write function. We will demonstrate both.
     total_supply = erc20_contract_bridge.call_read_function("totalSupply")
     my_balance = erc20_contract_bridge.call_read_function("balanceOf", erc20_contract_bridge.wallet_address)
 
     # Note how both of the functions above were not submitted to Fireblocks, as there is no need to sign these (read).
     # The below functions will demonstrate a write function, that will afterwards be submitted to Fireblocks.
 
     # We will mint a token (function receives address & amount) to our own address and then send it to another address.
     # We will also have to add the sender under the building_params in the following format:
-    checked_address = erc20_contract_bridge.web_provider.toChecksumAddress(erc20_contract_bridge.wallet_address)
+    checked_address = erc20_contract_bridge.web_provider.to_checksum_address(erc20_contract_bridge.wallet_address)
     # Web3 only accepts checkedSum addresses.
     building_params = {"from": checked_address}
     mint_raw_transaction = erc20_contract_bridge.call_write_function("mint", checked_address,
                                                                      TOKEN_AMOUNT,
                                                                      building_params=building_params)
     # We will now submit the transaction to Fireblocks.
     mint_transaction = erc20_contract_bridge.submit_transaction(mint_raw_transaction)
-    if ropsten_bridge.check_tx_is_completed(mint_transaction['id']) == TRANSACTION_STATUS_COMPLETED:
+    if goerli_bridge.check_tx_is_completed(mint_transaction['id']) == TRANSACTION_STATUS_COMPLETED:
         print(f"Successfully minted {TOKEN_AMOUNT} to {erc20_contract_bridge.wallet_address}")
         transfer_raw_transaction = erc20_contract_bridge.call_write_function("transferFrom",
                                                                              checked_address,
                                                                              RECEIVER_ADDRESS, TOKEN_AMOUNT,
                                                                              building_params=building_params)
         transfer_transaction = erc20_contract_bridge.submit_transaction(transfer_raw_transaction,
                                                                         "Transferring 10 minted tokens.")
-        if ropsten_bridge.check_tx_is_completed(transfer_transaction['id']):
+        if goerli_bridge.check_tx_is_completed(transfer_transaction['id']):
             print(
                 f"Successfully transferred {TOKEN_AMOUNT} from {erc20_contract_bridge.wallet_address} to "
                 f"{RECEIVER_ADDRESS}")
         else:
             print("Failed transferring minted tokens.")
     else:
         print("Failed minting new tokens.")
```

### Comparing `fireblocks_defi_sdk-1.0.2/fireblocks_defi_sdk_py/tokenization/examples/multi_token_example.py` & `fireblocks_defi_sdk-1.1.0/fireblocks_defi_sdk_py/tokenization/examples/multi_token_example.py`

 * *Files 10% similar despite different names*

```diff
@@ -10,30 +10,30 @@
 VAULT_ID = "0"
 CONTRACT = ""
 RECEIVER_ADDRESSES = ""
 # A list of ints representing the token IDs.
 TOKEN_IDS = [1, 2]
 
 if __name__ == "__main__":
-    # We start by building a bridge to the Kovan network, including initiating a ERC1155 object.
-    kovan_bridge = Web3Bridge(SDK, VAULT_ID, CONTRACT, Chain.KOVAN)
-    multi_token_contract_bridge = ERC1155(kovan_bridge)
+    # We start by building a bridge to the Goerli network, including initiating a ERC1155 object.
+    goerli_bridge = Web3Bridge(SDK, VAULT_ID, Chain.GOERLI, CONTRACT)
+    multi_token_contract_bridge = ERC1155(goerli_bridge)
 
     # ERC1155 implements all the basic capabilities mentioned in ERC721:
     # https://ethereum.org/en/developers/docs/standards/tokens/erc-1155/
     # This code will show a few examples using the functions mentioned above.
 
     # We will check the balance of tokens 1, 2 under the vault wallet address, and then use it to send all the tokens to
     # another address.
     tokens_balance = multi_token_contract_bridge.balance_of_batch(TOKEN_IDS)
     if tokens_balance:
         # Once again, the object will by default attempt to send assets from the given wallet address, unless defined
         # otherwise. We can also add a note to the transaction in Fireblocks.
         transfer_tokens = multi_token_contract_bridge.safe_batch_transfer_from(RECEIVER_ADDRESSES, TOKEN_IDS,
                                                                                tokens_balance,
                                                                                note="Transfer to another vault.")
-        transfer_result = kovan_bridge.check_tx_is_completed(transfer_tokens['id'])
+        transfer_result = goerli_bridge.check_tx_is_completed(transfer_tokens['id'])
 
         if transfer_result == TRANSACTION_STATUS_COMPLETED:
             print(f"{RECEIVER_ADDRESSES} now owns {tokens_balance} of tokens: {TOKEN_IDS}")
         else:
             print("Failed transferring tokens.")
```

### Comparing `fireblocks_defi_sdk-1.0.2/fireblocks_defi_sdk_py/tokenization/examples/nft_example.py` & `fireblocks_defi_sdk-1.1.0/fireblocks_defi_sdk_py/tokenization/examples/nft_example.py`

 * *Files 5% similar despite different names*

```diff
@@ -9,17 +9,17 @@
 SDK = FireblocksSDK(API_SECRET, API_KEY)
 VAULT_ID = "0"
 CONTRACT_ADDRESS = ""
 RECEIVER_ADDRESS = ""
 TOKEN_ID = 1
 
 if __name__ == "__main__":
-    # We start by building a bridge to the Ropsten network, including initiating a ERC721 object.
-    ropsten_bridge = Web3Bridge(SDK, VAULT_ID, CONTRACT_ADDRESS, Chain.ROPSTEN)
-    nft_contract_bridge = ERC721(ropsten_bridge)
+    # We start by building a bridge to the Goerli network, including initiating a ERC721 object.
+    goerli_bridge = Web3Bridge(SDK, VAULT_ID, Chain.GOERLI, CONTRACT_ADDRESS)
+    nft_contract_bridge = ERC721(goerli_bridge)
 
     # ERC721 implements all the basic capabilities mentioned in ERC721:
     # https://ethereum.org/en/developers/docs/standards/tokens/erc-721/
     # This code will show a few examples including the inherited supportsInterface from ERC165.
 
     # Each interface has a unique ID. If no parameter is passed onto the function, it checks for the default interface
     # of token, meaning - 721.
@@ -36,15 +36,15 @@
     if balance:
         # We will now verify if the owner of the token is indeed the wallet, and then transfer it to another address.
         token_owner = nft_contract_bridge.owner_of(TOKEN_ID)
         if token_owner == nft_contract_bridge.wallet_address:
             receiver_initial_balance = nft_contract_bridge.balance_of(RECEIVER_ADDRESS)
             # safe_transfer_from returns a dictionary with a status and id.
             transaction = nft_contract_bridge.safe_transfer_from(RECEIVER_ADDRESS, TOKEN_ID)
-            transaction_result = ropsten_bridge.check_tx_is_completed(transaction['id'])
+            transaction_result = goerli_bridge.check_tx_is_completed(transaction['id'])
 
             if transaction_result == TRANSACTION_STATUS_COMPLETED:
                 # After the transaction has been completed we check whether the balance of the receiver has been updated
                 if nft_contract_bridge.balance_of(RECEIVER_ADDRESS) == receiver_initial_balance + 1:
                     print(f"{RECEIVER_ADDRESS} has received the token successfully.")
             else:
                 print("Could not post transaction.")
```

### Comparing `fireblocks_defi_sdk-1.0.2/fireblocks_defi_sdk_py/tokenization/tokens/base_token.py` & `fireblocks_defi_sdk-1.1.0/fireblocks_defi_sdk_py/tokenization/tokens/base_token.py`

 * *Files 9% similar despite different names*

```diff
@@ -13,15 +13,15 @@
             raise ValueError("Bridge must contain a contract address (external_wallet_address).")
         self.web3_bridge = web3_bridge
         self.wallet_address = self.web3_bridge.fb_api_client.get_deposit_addresses(self.web3_bridge.source_vault_id,
                                                                                    self.web3_bridge.asset)[0][ADDRESS]
         self.web_provider = web3_bridge.web_provider
         self.abi = None
         self.contract: contract = self.web_provider.eth.contract(
-            address=self.web_provider.toChecksumAddress(self.web3_bridge.external_wallet_address)
+            address=self.web_provider.to_checksum_address(self.web3_bridge.external_wallet_address)
         )
 
     def __str__(self):
         return f"Contract [{self.web3_bridge.external_wallet_address}] | Chain [{self.web3_bridge.chain.value}]"
 
     def call_read_function(self, abi_function: str, *args):
         """
@@ -38,17 +38,17 @@
         :param abi_function:
         :param args:
         :param building_params:
         :return:
         """
         if not building_params:
             building_params = {}
-        return self.contract.get_function_by_name(abi_function)(*args).buildTransaction(building_params)
+        return self.contract.get_function_by_name(abi_function)(*args).build_transaction(building_params)
 
     def submit_transaction(self, transaction: dict, note: str = "") -> dict:
         """
-        Takes a ready transaction after being built (using web3 buildTransaction()) and transmits it to Fireblocks.
+        Takes a ready transaction after being built (using web3 build_transaction()) and transmits it to Fireblocks.
         :param note:
         :param transaction:
         :return:
         """
         return self.web3_bridge.send_transaction(transaction, note)
```

### Comparing `fireblocks_defi_sdk-1.0.2/fireblocks_defi_sdk_py/tokenization/tokens/erc1155.py` & `fireblocks_defi_sdk-1.1.0/fireblocks_defi_sdk_py/tokenization/tokens/erc1155.py`

 * *Files 20% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 class ERC1155(BaseToken):
     def __init__(self, web3_bridge: Web3Bridge):
         super().__init__(web3_bridge)
         self.abi = ERC1155_ABI
         self.contract: contract = self.web_provider.eth.contract(
-            address=self.web_provider.toChecksumAddress(self.web3_bridge.external_wallet_address),
+            address=self.web_provider.to_checksum_address(self.web3_bridge.external_wallet_address),
             abi=self.abi
         )
 
     # Payables
     def set_approval_for_all(self, operator_address: str, is_approved: bool, note: str = ""):
         """
         Provide an operator with approval permission or revoke them
         :param operator_address: Approved operator address
         :param is_approved: True to permit, False to revoke
         :param note: (Optional) Add a note to the transaction.
         :return: None
         """
-        checked_op_adr = self.web_provider.toChecksumAddress(operator_address)
+        checked_op_adr = self.web_provider.to_checksum_address(operator_address)
         return self.submit_transaction(self.call_write_function("setApprovalForAll", checked_op_adr, is_approved), note)
 
     def safe_transfer_from(self, to_address: str, token_id: int, amount: int, from_address: str = "",
                            data: bytes = bytearray(), note: str = ""):
         """
         :param to_address: The receiver of the token.
         :param token_id: The ID of the sent token.
@@ -34,25 +34,25 @@
         :param from_address: (Optional) The sender of the token, if it's not the wallet under Fireblocks.
         :param data: (Optional) Send additional data (bytes) only if required by contract.
         :param note: (Optional) Add a note to the transaction.
         :return: None
         """
         if not from_address:
             from_address = self.wallet_address
-        address_dict = {"from": self.web_provider.toChecksumAddress(from_address)}
-        checked_from_adr = self.web_provider.toChecksumAddress(from_address)
-        checked_to_adr = self.web_provider.toChecksumAddress(to_address)
+        address_dict = {"from": self.web_provider.to_checksum_address(from_address)}
+        checked_from_adr = self.web_provider.to_checksum_address(from_address)
+        checked_to_adr = self.web_provider.to_checksum_address(to_address)
 
         transaction = self.contract.functions.safeTransferFrom(
             checked_from_adr,
             checked_to_adr,
             token_id,
             amount,
             data
-        ).buildTransaction(address_dict)
+        ).build_transaction(address_dict)
 
         return self.submit_transaction(transaction, note)
 
     def safe_batch_transfer_from(self, to_address: str, token_ids: List[int], values: List[int], from_address: str = "",
                                  data: bytes = bytearray(), note: str = ""):
         """
         Length of token_ids and values must match. Moreover, the value of each token (at position x at [values]) to be
@@ -67,27 +67,27 @@
         :param from_address: (Optional) The sender of the token, if it's not the wallet under Fireblocks.
         :param data: (Optional) Send additional data (bytes) only if required by contract.
         :param note: (Optional) Add a note to the transaction.
         :return: None
         """
         if not from_address:
             from_address = self.wallet_address
-        address_dict = {"from": self.web_provider.toChecksumAddress(from_address)}
-        checked_from_adr = self.web_provider.toChecksumAddress(from_address)
-        checked_to_adr = self.web_provider.toChecksumAddress(to_address)
+        address_dict = {"from": self.web_provider.to_checksum_address(from_address)}
+        checked_from_adr = self.web_provider.to_checksum_address(from_address)
+        checked_to_adr = self.web_provider.to_checksum_address(to_address)
         if len(token_ids) != len(values):
             raise ValueError("Length of token_ids and values must match!")
 
         transaction = self.contract.functions.safeBatchTransferFrom(
             checked_from_adr,
             checked_to_adr,
             token_ids,
             values,
             data
-        ).buildTransaction(address_dict)
+        ).build_transaction(address_dict)
 
         return self.submit_transaction(transaction, note)
 
     # Views
     def supports_interface(self, interface_id: str = "0xd9b67a26") -> bool:
         """
         Checks if contract supports a certain interface.
@@ -113,28 +113,28 @@
 
         :param owners_list: A list of addresses
         :param id_list: A list of token Ids
         :return:
         """
         if not owners_list:
             owners_list = [self.wallet_address] * len(id_list)
-        checked_addresses = [self.web_provider.toChecksumAddress(address) for address in owners_list]
+        checked_addresses = [self.web_provider.to_checksum_address(address) for address in owners_list]
         return self.call_read_function("balanceOfBatch", checked_addresses, id_list)
 
     def is_approved_for_all(self, operator_address: str, owner_address: str = "") -> bool:
         """
         Validates whether an operator has been approved by a stated owner.
         :param operator_address: Address of the meant to be operator.
         :param owner_address: (Optional) Address of the owner, in case it's not the wallet address.
         :return: True whether operator is approved, False otherwise
         """
         if not owner_address:
             owner_address = self.wallet_address
-        owner_checked_address = self.web_provider.toChecksumAddress(owner_address)
-        operator_checked_address = self.web_provider.toChecksumAddress(operator_address)
+        owner_checked_address = self.web_provider.to_checksum_address(owner_address)
+        operator_checked_address = self.web_provider.to_checksum_address(operator_address)
         return self.call_read_function("isApprovedForAll", owner_checked_address, operator_checked_address)
 
     def uri(self, token_id: int) -> str:
         """
         :param token_id: URI id of a contract
         :return: The JSON metadata
         """
```

### Comparing `fireblocks_defi_sdk-1.0.2/fireblocks_defi_sdk_py/tokenization/tokens/erc721.py` & `fireblocks_defi_sdk-1.1.0/fireblocks_defi_sdk_py/tokenization/tokens/erc721.py`

 * *Files 8% similar despite different names*

```diff
@@ -3,32 +3,32 @@
 
 
 class ERC721(BaseToken):
     def __init__(self, web3_bridge: Web3Bridge):
         super().__init__(web3_bridge)
         self.abi = ERC721_ABI
         self.contract: contract = self.web_provider.eth.contract(
-            address=self.web_provider.toChecksumAddress(self.web3_bridge.external_wallet_address),
+            address=self.web_provider.to_checksum_address(self.web3_bridge.external_wallet_address),
             abi=self.abi
         )
 
     # Payables
     def approve(self, to_address: str, token_id: int, approver_address: str = "", note: str = ""):
         """
         Receives an address and a Token ID so the specified address can perform actions on it.
         :param to_address: The receiver of the token.
         :param token_id: The ID of the sent token.
         :param approver_address: The owner of the token.
         :param note: (Optional) Add a note to the transaction.
         :return: None
         """
-        checked_app_adr = self.web_provider.toChecksumAddress(to_address)
+        checked_app_adr = self.web_provider.to_checksum_address(to_address)
         if not approver_address:
             approver_address = self.wallet_address
-        address_dict = {"from": self.web_provider.toChecksumAddress(approver_address)}
+        address_dict = {"from": self.web_provider.to_checksum_address(approver_address)}
         return self.submit_transaction(self.call_write_function("approve", checked_app_adr, token_id,
                                                                 building_params=address_dict), note)
 
     def safe_transfer_from(self, to_address: str, token_id: int, from_address: str = "", data: bytes = bytearray(),
                            note: str = ""):
         """
         :param from_address: The sender of the token.
@@ -37,31 +37,31 @@
         :param from_address: (Optional) The sender of the token, if it's not the wallet under Fireblocks.
         :param data: (Optional) Send additional data (bytes) only if required by contract.
         :param note: (Optional) Add a note to the transaction.
         :return: None
         """
         if not from_address:
             from_address = self.wallet_address
-        address_dict = {"from": self.web_provider.toChecksumAddress(from_address)}
-        checked_from_adr = self.web_provider.toChecksumAddress(from_address)
-        checked_to_adr = self.web_provider.toChecksumAddress(to_address)
+        address_dict = {"from": self.web_provider.to_checksum_address(from_address)}
+        checked_from_adr = self.web_provider.to_checksum_address(from_address)
+        checked_to_adr = self.web_provider.to_checksum_address(to_address)
         if data:
             transaction = self.contract.functions.safeTransferFrom(
                 checked_from_adr,
                 checked_to_adr,
                 token_id,
                 data
-            ).buildTransaction(address_dict)
+            ).build_transaction(address_dict)
 
         else:
             transaction = self.contract.functions.safeTransferFrom(
                 checked_from_adr,
                 checked_to_adr,
                 token_id
-            ).buildTransaction(address_dict)
+            ).build_transaction(address_dict)
 
         return self.submit_transaction(transaction, note)
 
     def transfer_from(self, to_address: str, token_id: int, from_address: str = "", note: str = ""):
         """
         Do note it's encouraged to use safe_transfer_from instead.
         :param from_address: The sender of the token.
@@ -69,32 +69,32 @@
         :param token_id: The ID of the sent token.
         :param from_address: (Optional) The sender of the token, if it's not the wallet under Fireblocks.
         :param note: (Optional) Add a note to the transaction.
         :return: None
         """
         if not from_address:
             from_address = self.wallet_address
-        address_dict = {"from": self.web_provider.toChecksumAddress(from_address)}
-        checked_from_adr = self.web_provider.toChecksumAddress(from_address)
-        checked_to_adr = self.web_provider.toChecksumAddress(to_address)
+        address_dict = {"from": self.web_provider.to_checksum_address(from_address)}
+        checked_from_adr = self.web_provider.to_checksum_address(from_address)
+        checked_to_adr = self.web_provider.to_checksum_address(to_address)
         return self.submit_transaction(self.call_write_function("transferFrom",
                                                                 checked_from_adr,
                                                                 checked_to_adr,
                                                                 token_id,
                                                                 building_params=address_dict), note)
 
     def set_approval_for_all(self, operator_address: str, is_approved: bool, note: str = ""):
         """
         Provide an operator with approval permission or revoke them
         :param operator_address: Approved operator address
         :param is_approved: True to permit, False to revoke
         :param note: (Optional) Add a note to the transaction.
         :return: None
         """
-        checked_op_adr = self.web_provider.toChecksumAddress(operator_address)
+        checked_op_adr = self.web_provider.to_checksum_address(operator_address)
         return self.submit_transaction(self.call_write_function("setApprovalForAll", checked_op_adr, is_approved), note)
 
     # Views
     def supports_interface(self, interface_id: str = "0x80ac58cd") -> bool:
         """
         Checks if contract supports a certain interface.
         :param interface_id: The interface id. "0x80ac58cd" is ERC721 interface id. "0xd9b67a26" is ERC1155 interface id
@@ -114,27 +114,27 @@
     def is_approved_for_all(self, owner_address: str, operator_address: str) -> bool:
         """
         Validates whether an operator has been approved by a stated owner.
         :param owner_address: Address of the owner.
         :param operator_address: Address of the meant to be operator.
         :return: True whether operator is approved, False otherwise
         """
-        owner_checked_address = self.web_provider.toChecksumAddress(owner_address)
-        operator_checked_address = self.web_provider.toChecksumAddress(operator_address)
+        owner_checked_address = self.web_provider.to_checksum_address(owner_address)
+        operator_checked_address = self.web_provider.to_checksum_address(operator_address)
         return self.call_read_function("isApprovedForAll", owner_checked_address, operator_checked_address)
 
     def balance_of(self, owner_address: str = "") -> int:
         """
         Gets the balance of the address provided
         :param owner_address: Address to be checked
         :return: Balance (int)
         """
         if not owner_address:
             owner_address = self.wallet_address
-        owner_checked_address = self.web_provider.toChecksumAddress(owner_address)
+        owner_checked_address = self.web_provider.to_checksum_address(owner_address)
         return self.call_read_function("balanceOf", owner_checked_address)
 
     def owner_of(self, token_id: int) -> str:
         """
         Checks who owns the token ID.
         :param token_id: a number representing the token ID
         :return: The address (plain) of the owner
```

### Comparing `fireblocks_defi_sdk-1.0.2/fireblocks_defi_sdk_py/tokenization/utils/helpers.py` & `fireblocks_defi_sdk-1.1.0/fireblocks_defi_sdk_py/tokenization/utils/helpers.py`

 * *Files identical despite different names*

### Comparing `fireblocks_defi_sdk-1.0.2/fireblocks_defi_sdk_py/web3_bridge.py` & `fireblocks_defi_sdk-1.1.0/fireblocks_defi_sdk_py/web3_bridge.py`

 * *Files 1% similar despite different names*

```diff
@@ -31,15 +31,14 @@
     Chain.RSK: ('RBTC', "https://public-node.rsk.co"),
     Chain.RSK_TEST: ('RBTC_TEST', "https://public-node.testnet.rsk.co"),
     Chain.CELO: ('CELO', "https://rpc.ankr.com/celo"),
     Chain.CELO_BAK: ('CELO_BAK', "https://baklava-blockscout.celo-testnet.org/api/eth-rpc"),
     Chain.OPTIMISM: ('ETH-OPT', "https://rpc.ankr.com/optimism"),
     Chain.OPTIMISM_KOVAN: ('ETH-OPT_KOV', "https://optimism-kovan.infura.io/v3/9aa3d95b3bc440fa88ea12eaa4456161"),
     Chain.RONIN: ('RON', "https://api.roninchain.com/rpc"),
-    Chain.ARBITRUM: ('ETH-AETH', "https://rpc.ankr.com/arbitrum"),
     Chain.ARBITRUM_GOERLI: ('ETH-AETH_RIN', "https://goerli-rollup.arbitrum.io/rpc")
 }
 
 
 class Web3Bridge:
     def __init__(self, fb_api_client: FireblocksSDK,
                  vault_account_id: str,
@@ -59,15 +58,15 @@
         self.external_wallet_address = external_wallet_address
         self.asset: str = CHAIN_TO_ASSET_ID[self.chain][0]
         self.web_provider = Web3(Web3.HTTPProvider(CHAIN_TO_ASSET_ID[self.chain][1]))
         self.wl_uuid = wl_uuid
 
     def send_transaction(self, transaction: dict, note="") -> dict:
         """
-        Takes a ready transaction after being built (using web3 buildTransaction()) and transmits it to Fireblocks.
+        Takes a ready transaction after being built (using web3 build_transaction()) and transmits it to Fireblocks.
         :param transaction: A transaction object (dict) to submit to the blockchain.
         :param note: (Optional) A note to submit with the transaction.
         :return:
         """
         if self.wl_uuid:
             destination = TransferPeerPath(EXTERNAL_WALLET, self.wl_uuid)
         else:
```

### Comparing `fireblocks_defi_sdk-1.0.2/setup.py` & `fireblocks_defi_sdk-1.1.0/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -5,27 +5,27 @@
     packages=[
         'fireblocks_defi_sdk_py',
         'fireblocks_defi_sdk_py.tokenization',
         'fireblocks_defi_sdk_py.tokenization.tokens',
         'fireblocks_defi_sdk_py.tokenization.utils',
         'fireblocks_defi_sdk_py.tokenization.examples'
     ],
-    version='1.0.2',
+    version='1.1.0',
     license='MIT',
     description='fireblocks_defi_sdk_py',
     long_description="""Fireblocks python SDK""",
     long_description_content_type='text/markdown',
     author='Fireblocks',
     author_email='fireblocks@fireblocks.com',
     url='https://github.com/fireblocks/fireblocks-defi-sdk-py',
-    download_url='https://github.com/fireblocks/fireblocks-defi-sdk-py/archive/refs/tags/1.0.2.tar.gz',
+    download_url='https://github.com/fireblocks/fireblocks-defi-sdk-py/archive/refs/tags/1.1.0.tar.gz',
     keywords=['FIREBLOCKS', 'DeFi', 'SDK', 'PYTHON'],
     install_requires=[
-        'fireblocks_sdk==1.17.3',
-        'web3==5.26.0'
+        'fireblocks_sdk==1.19.0',
+        'web3==6.2.0'
     ],
     classifiers=[
         'Development Status :: 3 - Alpha',
         'Intended Audience :: Developers',
         'Topic :: Software Development :: Build Tools',
         'License :: OSI Approved :: MIT License',
         'Programming Language :: Python :: 3.6',
```

