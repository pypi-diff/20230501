# Comparing `tmp/dxsp-1.5.1.tar.gz` & `tmp/dxsp-1.5.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dxsp-1.5.1.tar", max compression
+gzip compressed data, was "dxsp-1.5.3.tar", max compression
```

## Comparing `dxsp-1.5.1.tar` & `dxsp-1.5.3.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0     1064 2023-04-30 20:46:32.534129 dxsp-1.5.1/LICENSE
--rw-r--r--   0        0        0     3225 2023-04-30 20:46:32.534129 dxsp-1.5.1/README.md
--rw-r--r--   0        0        0       38 2023-04-30 20:46:32.534129 dxsp-1.5.1/dxsp/.gitignore
--rw-r--r--   0        0        0      169 2023-04-30 20:46:33.422140 dxsp-1.5.1/dxsp/__init__.py
--rw-r--r--   0        0        0        1 2023-04-30 20:46:32.534129 dxsp-1.5.1/dxsp/assets/__init__.py
--rw-r--r--   0        0        0     8887 2023-04-30 20:46:32.534129 dxsp-1.5.1/dxsp/assets/blockchains.py
--rw-r--r--   0        0        0      392 2023-04-30 20:46:32.534129 dxsp-1.5.1/dxsp/config.py
--rw-r--r--   0        0        0      564 2023-04-30 20:46:32.534129 dxsp-1.5.1/dxsp/default_settings.toml
--rw-r--r--   0        0        0    27903 2023-04-30 20:46:32.534129 dxsp-1.5.1/dxsp/main.py
--rw-r--r--   0        0        0     1015 2023-04-30 20:46:33.422140 dxsp-1.5.1/pyproject.toml
--rw-r--r--   0        0        0     4028 1970-01-01 00:00:00.000000 dxsp-1.5.1/PKG-INFO
+-rw-r--r--   0        0        0     1064 2023-05-01 14:22:52.068491 dxsp-1.5.3/LICENSE
+-rw-r--r--   0        0        0     3225 2023-05-01 14:22:52.068491 dxsp-1.5.3/README.md
+-rw-r--r--   0        0        0       38 2023-05-01 14:22:52.068491 dxsp-1.5.3/dxsp/.gitignore
+-rw-r--r--   0        0        0      169 2023-05-01 14:22:52.812491 dxsp-1.5.3/dxsp/__init__.py
+-rw-r--r--   0        0        0        1 2023-05-01 14:22:52.068491 dxsp-1.5.3/dxsp/assets/__init__.py
+-rw-r--r--   0        0        0     8887 2023-05-01 14:22:52.068491 dxsp-1.5.3/dxsp/assets/blockchains.py
+-rw-r--r--   0        0        0      392 2023-05-01 14:22:52.068491 dxsp-1.5.3/dxsp/config.py
+-rw-r--r--   0        0        0      564 2023-05-01 14:22:52.068491 dxsp-1.5.3/dxsp/default_settings.toml
+-rw-r--r--   0        0        0    29591 2023-05-01 14:22:52.068491 dxsp-1.5.3/dxsp/main.py
+-rw-r--r--   0        0        0     1015 2023-05-01 14:22:52.812491 dxsp-1.5.3/pyproject.toml
+-rw-r--r--   0        0        0     4028 1970-01-01 00:00:00.000000 dxsp-1.5.3/PKG-INFO
```

### Comparing `dxsp-1.5.1/LICENSE` & `dxsp-1.5.3/LICENSE`

 * *Files identical despite different names*

### Comparing `dxsp-1.5.1/README.md` & `dxsp-1.5.3/README.md`

 * *Files identical despite different names*

### Comparing `dxsp-1.5.1/dxsp/assets/blockchains.py` & `dxsp-1.5.3/dxsp/assets/blockchains.py`

 * *Files identical despite different names*

### Comparing `dxsp-1.5.1/dxsp/default_settings.toml` & `dxsp-1.5.3/dxsp/default_settings.toml`

 * *Files identical despite different names*

### Comparing `dxsp-1.5.1/dxsp/main.py` & `dxsp-1.5.3/dxsp/main.py`

 * *Files 3% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 from web3 import Web3
 
 
 class DexSwap:
     """Do a swap."""
 
     def __init__(self,
-                 chain_id: int = 1, 
+                 chain_id: int = 1,
                  wallet_address: str | None = None,
                  private_key: str | None = None,
                  block_explorer_api: str | None = None,
                  block_explorer_url: str | None = None,
                  rpc: str | None = None,
                  w3: Web3 | None = None,
                  protocol_type: str | None = None,
@@ -102,15 +102,15 @@
                 self.dex_exchange is None
                 or self.dex_exchange != blockchain["uniswap_v3"]
             ):
                 self.router = blockchain["uniswap_v2"]
             else:
                 self.router = blockchain["uniswap_v3"]
         else:
-            self.router = self.dex_router 
+            self.router = self.dex_router
         self.logger.debug("self.router %s",self.router)
 
         self.name = "TBD"
         self.logger.debug("self.name %s",self.name)
 
         self.base_trading_symbol = base_trading_symbol
         if self.base_trading_symbol is None:
@@ -124,22 +124,30 @@
         assetplatform = self.gecko_api.get_asset_platforms()
         output_dict = [x for x in assetplatform if x['chain_identifier'] == int(self.chain_id)]
         self.gecko_platform = output_dict[0]['id']
         self.logger.debug("self.gecko_platform %s",self.gecko_platform)
         # self.gasPrice = gasPrice
         # self.gasLimit = gasLimit
 
-    async def _get(self, url, params=None, headers=None):
+    async def _get(
+                self,
+                url,
+                params=None,
+                headers=None
+            ):
         headers = { "User-Agent": "Mozilla/5.0" }
         self.logger.debug("_get url %s",url)
-        response = requests.get(url,params =params,headers=headers)
+        response = requests.get(url,params =params,headers=headers, timeout=10)
         #self.logger.debug(f"response _get {response}")
         return response.json()
 
-    async def get_quote(self, symbol):
+    async def get_quote(
+                self,
+                symbol
+            ):
         self.logger.debug("get_quote %s",symbol)
         asset_in_address = await self.search_contract(symbol)
         self.logger.debug("asset_in_address %s", asset_in_address)
         asset_out_symbol = self.base_trading_symbol
         asset_out_address = await self.search_contract(asset_out_symbol)
         self.logger.debug("asset_out_address %s",asset_out_address)
         if asset_out_address is None:
@@ -164,82 +172,95 @@
                 return round(quote_readable,2)
             if self.protocol_type in ["uniswap_v2","uniswap_v3"]:
                 return
         except Exception as e:
             self.logger.error("get_quote %s", e)
             return
 
-    async def execute_order(self,direction,instrument,stop_loss=10000,take_profit=10000,quantity=1,amount_trading_option=1,order_type='swap'):
-        self.logger.debug("execute_order %s %s %s",direction,instrument, order_type)
+    async def execute_order(
+                self,
+                action,
+                instrument,
+                stop_loss=10000,
+                take_profit=10000,
+                quantity=1,
+                amount_trading_option=1,
+                order_type='swap'
+        ):
+        """execute swap function"""
+        self.logger.debug("execute_order %s %s %s",action,instrument, order_type)
         if order_type == 'swap':
             self.logger.debug("execute_order %s",order_type)
             try:
-                asset_out_symbol = self.base_trading_symbol if direction=="BUY" else instrument
-                asset_in_symbol = instrument if direction=="BUY" else self.base_trading_symbol
+                asset_out_symbol = self.base_trading_symbol if action=="BUY" else instrument
+                asset_in_symbol = instrument if action=="BUY" else self.base_trading_symbol
                 asset_out_contract = await self.get_token_contract(asset_out_symbol)
                 asset_out_decimals = asset_out_contract.functions.decimals().call()
                 asset_out_balance = await self.get_token_balance(asset_out_symbol)
                 if amount_trading_option == 1:
-                    asset_out_amount = ((asset_out_balance)/(10 ** asset_out_decimals))*(float(quantity)/100) #buy or sell %p percentage DEFAULT OPTION
+                    #buy or sell %p percentage DEFAULT OPTION
+                    asset_out_amount = ((asset_out_balance)/
+                                        (10 ** asset_out_decimals))*(float(quantity)/100)
                 if amount_trading_option == 2:
-                    asset_out_amount = (asset_out_balance)/(10 ** asset_out_decimals) #SELL all token in case of sell order for example
-          
-                swap = self.get_swap(
+                    #SELL all token in case of sell order for example
+                    asset_out_amount = (asset_out_balance)/(10 ** asset_out_decimals)
+                order = self.get_swap(
                         asset_out_symbol,
                         asset_in_symbol,
                         asset_out_amount
                         )
-
+                if order:
+                    return order['confirmation']
             except Exception as e:
                 self.logger.debug("error execute_order %s",e)
-                return
+                return "error processing order in DXSP"
 
         if order_type == 'market':
             self.logger.debug("execute_order %s", order_type)
             return
         if order_type == 'limit':
             self.logger.debug("execute_order %s", order_type)
             return
 
     async def get_swap(
-                self, 
-                asset_out_symbol: str, 
+                self,
+                asset_out_symbol: str,
                 asset_in_symbol: str,
-                amount: int, 
-                slippage_tolerance_percentage = 2 
+                amount: int,
+                slippage_tolerance_percentage = 2
         ):
         """main swap function"""
 
         self.logger.debug("get_swap %s %s %s", asset_out_symbol, asset_in_symbol, amount)
         try:
-            #ASSET OUT 
+            #ASSET OUT
             asset_out_address = await self.search_contract(asset_out_symbol)
             asset_out_contract = await self.get_token_contract(asset_out_symbol)
             self.logger.debug("asset_out_address %s %s",asset_out_address,asset_out_symbol)
             if asset_out_contract is None:
                 return
             asset_out_decimals=asset_out_contract.functions.decimals().call()
             asset_out_balance = await self.get_token_balance(asset_out_symbol)
             self.logger.debug("asset_out_balance %s",asset_out_balance)
             if asset_out_balance == 0:
                 self.logger.warning("No Money")
-                return 
-            #ASSETS IN 
+                return
+            #ASSETS IN
             asset_in_address = await self.search_contract(asset_in_symbol)
             self.logger.debug("asset_in_address %s", asset_in_address)
             if asset_in_address is None:
                 return
 
             #AMOUNT
             asset_out_decimals = asset_out_contract.functions.decimals().call()
             self.logger.debug("asset_out_decimals %s",asset_out_decimals)
             asset_out_amount = amount * 10 ** asset_out_decimals
             slippage = slippage_tolerance_percentage # defaulted to 2% slippage if not given
             self.logger.debug("slippage %s",slippage)
-            asset_out_amount_converted = self.w3.to_wei(amount,'ether')
+            asset_out_amount_converted = self.w3.to_wei(asset_out_amount,'ether')
 
             transaction_amount = int((asset_out_amount_converted *(slippage/100)))
             self.logger.debug("transaction_amount %s",transaction_amount)
 
             #VERIFY IF ASSET OUT IS APPROVED otherwise get it approved
             await self.get_approve(asset_out_address)
 
@@ -289,17 +310,19 @@
                     order['id'] = transaction_receipt['transactionHash']
                     order['timestamp'] = transaction_block['timestamp']
                     order['instrument'] = asset_out_symbol
                     order['contract'] = asset_out_address
                     order['amount'] = transaction_amount
                     order['fee'] = transaction_receipt['gasUsed']
                     order['price'] = "TBD"
-                    order['confirmation'] = "TBD"
-                    #response+= f"\n➕ Size: {round(ex.from_wei(transaction_amount, 'ether'),5)}\n⚫️ Entry: {await fetch_gecko_asset_price(asset_in_symbol)}USD \nℹ️ {txHash}\n⛽️ {txHashDetail['gasUsed']}\n🗓️ {datetime.now()}"
-            #logger.info(msg=f"{response}")
+                    order['confirmation']= f"➕ Size: {order['amount']}\n\
+                                        ⚫️ Entry: {order['price']}\n\
+                                        ℹ️ {order['id']}\n\
+                                        🗓️ {order['timestamp']}"
+                    self.logger.info("order %s",order)
                     return order
         except Exception as e:
             self.logger.error("get_swap %s",e)
             return
 
     async def get_block_explorer_status(self,txHash):
         self.logger.debug("get_block_explorer_status %s",txHash)
@@ -316,15 +339,19 @@
     #         output_dict = [x for x in assetplatform if x['chain_identifier'] == int(self.chain_id)]
     #         self.logger.debug(f"search_gecko_platform search {output_dict}")
     #         return output_dict[0]['id']
     #     except Exception as e:
     #         self.logger.debug(f"error search_gecko_platform {e}")
     #         return
 
-    async def search_contract(self, token):
+    async def search_contract(
+                            self, 
+                            token
+                            ):
+        """search a contract function"""
         self.logger.debug("search_contract")
 
         try:
             token_contract = await self.get_contract_address(settings.TOKEN_PERSONAL_LIST,token)
             self.logger.debug("personal_list")
             if token_contract is None:
                 token_contract = await self.get_contract_address(settings.TOKEN_TESTNET_LIST,token)
@@ -341,14 +368,15 @@
             else:
                 self.logger.debug("no contract found for %s",token)
         except Exception as e:
             self.logger.error("search_contract %s",e)
             return
 
     async def search_gecko(self,token):
+        """search coingecko"""
         self.logger.debug("search_gecko %s",token)
         try:
             search_results = self.gecko_api.search(query=token)
             search_dict = search_results['coins']
             #self.logger.debug(f"search_dict {search_dict}")
             filtered_dict = [x for x in search_dict if x['symbol'] == token.upper()]
             api_dict = [ sub['api_symbol'] for sub in filtered_dict ]
@@ -361,72 +389,87 @@
                 except KeyError:
                     pass
         except Exception as e:
             self.logger.error("search_gecko %s", e)
             return
 
     async def search_gecko_contract(self,token):
+        """search coingecko contract"""
         self.logger.debug("🦎search_gecko_contract %s", token)
         self.logger.debug("🦎self.gecko_platform %s", self.gecko_platform)
         try:
             coin_info = await self.search_gecko(token)
             if coin_info is not None:
-                coin_info['platforms'][f'{self.gecko_platform}']
-                self.logger.debug("🦎search_gecko_coin_info %s",token)
                 return coin_info['platforms'][f'{self.gecko_platform}']
         except Exception as e:
             self.logger.error(f"error search_gecko_contract {e}")
             return
 
-    async def get_contract_address(self,token_list_url, symbol):
+    async def get_contract_address(
+                            self,
+                            token_list_url,
+                            symbol
+                        ):
+        """get token address from json list"""
         self.logger.debug("get_contract_address %s %s",token_list_url, symbol)
         try:
             token_list = await self._get(token_list_url)
             token_search = token_list['tokens']
             for keyval in token_search:
                 if (keyval['symbol'] == symbol and keyval['chainId'] == self.chain_id):
                     return keyval['address']
         except Exception as e:
             self.logger.debug("get_contract_address %s", e)
             return
 
-    async def get_token_contract(self, token):
+    async def get_token_contract(
+                                self,
+                                token
+                            ):
+        """get token contract (ABI+address)"""
         self.logger.debug("get_token_contract %s",token)
         try:
             token_address = await self.search_contract(token)
             token_abi = await self.get_abi(token_address)
             return self.w3.eth.contract(address=token_address, abi=token_abi)
         except Exception as e:
             self.logger.error("get_token_contract %s",e)
             return
 
 
 ####UTILS
-    async def get_approve(self, asset_out_address: str, amount=None):
+    async def get_approve(
+                        self,
+                        asset_out_address: str,
+                        amount=None
+                    ):
         self.logger.debug("get_approve %s", asset_out_address)
         if self.protocol_type in ["1inch","1inch_limit"]:
             approval_check_URL = f"{self.dex_url}/approve/allowance?tokenAddress={asset_out_address}&walletAddress={self.wallet_address}"
             approval_response = await self._get(approval_check_URL)
             approval_check = approval_response['allowance']
             if (approval_check==0):
                 approval_URL = f"{self.dex_url}/approve/transaction?tokenAddress={asset_out_address}"
                 approval_response = await self._get(approval_URL)
         elif self.protocol_type in ["uniswap_v2","uniswap_v3"]:
             asset_out_abi= await self.get_abi(asset_out_address)
-            asset_out_contract = self.w3.eth.contract(address=asset_out_address, abi=asset_out_abi)           
+            asset_out_contract = self.w3.eth.contract(address=asset_out_address, abi=asset_out_abi)
             approval_check = asset_out_contract.functions.allowance(self.w3.to_checksum_address(self.wallet_address), self.w3.to_checksum_address(self.router)).call()
             if (approval_check==0):
                 approved_amount = (self.w3.to_wei(2**64-1,'ether'))
                 asset_out_abi = await self.get_abi(asset_out_address)
                 asset_out_contract = self.w3.eth.contract(address=asset_out_address, abi=asset_out_abi)
                 approval_TX = asset_out_contract.functions.approve(self.w3.to_checksum_address(self.router), approved_amount)
                 approval_txHash = await self.get_sign(approval_TX)
                 approval_txHash_complete = self.w3.eth.wait_for_transaction_receipt(approval_txHash, timeout=120, poll_latency=0.1)
 
-    async def get_sign(self, tx):
+    async def get_sign(
+                    self,
+                    tx
+                ):
         self.logger.debug("get_sign %s", tx)
         try:
             if self.protocol_type in ['uniswap_v2','uniswap_v3']:
                 tx_params = {
                 'from': self.wallet_address,
                 'gas': await self.get_gas(tx),
                 'gasPrice': await self.get_gasPrice(tx),
@@ -442,15 +485,18 @@
             signed = self.w3.eth.account.sign_transaction(tx, self.private_key)
             raw_tx = signed.rawTransaction
             return self.w3.eth.send_raw_transaction(raw_tx)
         except Exception as e:
             self.logger.error(" get_sign %s", e)
             return
 
-    async def get_gas(self, tx):
+    async def get_gas(
+                    self,
+                    tx
+                ):
         self.logger.debug("get_gas %s",tx)
         gasestimate= self.w3.eth.estimate_gas(tx) * 1.25
         return int(self.w3.to_wei(gasestimate,'wei'))
 
     async def get_gasPrice(self, tx):
         self.logger.debug("get_gasPrice %s", tx)
         gasprice = self.w3.eth.generate_gas_price()
@@ -477,66 +523,84 @@
             # https://github.com/tintinweb/smart-contract-sanctuary
             #https://raw.githubusercontent.com/tintinweb/smart-contract-sanctuary-optimism/master/contracts/mainnet/1f/1F98431c8aD98523631AE4a59f267346ea31F984_UniswapV3Factory.sol
 
         except Exception as e:
             self.logger.error("error get_abi %s", e)
             return
 
-#####USERS
+#####USERS RELATED
 
     # async def get_wallet_auth(self):
     #     try:
     #         return
     #     except Exception as e:
     #         self.logger.error("get_wallet_auth error: %s",e)
     #         return
 
-    async def get_token_balance(self, token):
+    async def get_token_balance(
+                                self,
+                                token
+                            ):
         self.logger.debug("get_token_balance %s", token)
         try:
             token_address = await self.search_contract(token)
             token_abi =  await self.get_abi(token_address)
             token_contract = self.w3.eth.contract(address=token_address, abi=token_abi)
             token_balance = token_contract.functions.balanceOf(self.wallet_address).call()
             self.logger.debug("token_address %s token_balance %s",token_address,token_balance)
             # (ex.from_wei(await fetch_token_balance(basesymbol), 'ether'), 5)
             return 0 if token_balance <=0 or token_balance is None else token_balance
         except Exception as e:
             self.logger.error("get_token_balance %s: %s",token, e)
             return 0
 
-    async def get_basecoin_balance(self):
-        bal_base_trading_symbol = await self.get_token_balance(self.base_trading_symbol)
-            # return round(ex.from_wei(await fetch_token_balance(basesymbol), 'ether'), 5)
-        return bal_base_trading_symbol
-        # bal = round(ex.from_wei(bal,'ether'),5)
+    async def get_basecoin_balance(
+                                self
+                            ):
+        try:
+            bal_base_trading_symbol = await self.get_token_balance(self.base_trading_symbol)
+                # return round(ex.from_wei(await fetch_token_balance(basesymbol), 'ether'), 5)
+            return bal_base_trading_symbol
+            # bal = round(ex.from_wei(bal,'ether'),5)
+        except Exception as e:
+            self.logger.error("get_basecoin_balance %s: %s",token, e)
+            return 0
 
-    async def get_stablecoin_balance(self):
+    async def get_stablecoin_balance(
+                                self
+                            ):
         toptokens = ["USDT","USDC","BUSD","DAI"]
-        for i in toptokens:
-            bal_toptoken = await self.get_token_balance(i)
-            if bal_toptoken:
-                msg += f"\n💵{bal_toptoken} {i}"
-            # bal = round(ex.from_wei(bal,'ether'),5)
+        try:
+            for i in toptokens:
+                bal_toptoken = await self.get_token_balance(i)
+                if bal_toptoken:
+                    msg += f"\n💵{bal_toptoken} {i}"
+                # bal = round(ex.from_wei(bal,'ether'),5)
+        except Exception as e:
+            self.logger.error("get_stablecoin_balance error: %s", e)
+            return 0
 
-    async def get_account_balance(self):
+    async def get_account_balance(
+                            self
+                        ):
         toptokens = ["USDT","USDC"]
         try:
             for i in toptokens:
                 bal_toptoken = await self.get_token_balance(i)
                 if bal_toptoken:
                     msg += f"\n💵{bal_toptoken} {i}"
                     return msg
         except Exception as e:
             self.logger.error("get_account_balance error: %s", e)
-            return 0
+            return "balance error"
             # bal = round(ex.from_wei(bal,'ether'),5)
 
-    async def get_account_position(self):
-        
+    async def get_account_position(
+                            self
+                        ):
         try:
             self.logger.debug("get_account_position")
             # asset_position_address= await search_contract(asset_out_symbol)
             # asset_position_abi= await fetch_abi_dex(asset_out_address)
             # asset_position_contract = ex.eth.contract(address=asset_out_address, abi=asset_out_abi)
             # open_positions = asset_position_contract.functions.getOpenPositions(walletaddress).call()
             return
```

### Comparing `dxsp-1.5.1/pyproject.toml` & `dxsp-1.5.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "dxsp"
-version = "1.5.1"
+version = "1.5.3"
 description = "DXSP (DeX SwaP), A defi swap helper package. Swap made easy."
 authors = ["mraniki <8766259+mraniki@users.noreply.github.com>"]
 license = "MIT License"
 readme = "README.md"
 
 
 [tool.poetry.urls]
```

### Comparing `dxsp-1.5.1/PKG-INFO` & `dxsp-1.5.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dxsp
-Version: 1.5.1
+Version: 1.5.3
 Summary: DXSP (DeX SwaP), A defi swap helper package. Swap made easy.
 License: MIT
 Author: mraniki
 Author-email: 8766259+mraniki@users.noreply.github.com
 Requires-Python: >=3.9,<3.11
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

