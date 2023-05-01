# Comparing `tmp/cardano-nft-vending-machine-0.6.3.tar.gz` & `tmp/cardano-nft-vending-machine-0.6.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/Users/thaddeusdiamond/workspaces/wildtangz/cardano-vending-machine/dist/.tmp-qnpfdt7c/cardano-nft-vending-machine-0.6.3.tar", last modified: Sat Apr 15 01:56:09 2023, max compression
+gzip compressed data, was "/Users/thaddeusdiamond/workspaces/wildtangz/cardano-vending-machine/dist/.tmp-lgs6mp_f/cardano-nft-vending-machine-0.6.4.tar", last modified: Mon May  1 02:24:38 2023, max compression
```

## Comparing `cardano-nft-vending-machine-0.6.3.tar` & `cardano-nft-vending-machine-0.6.4.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxrwxr-x   0 thaddeusdiamond   (501) staff       (20)        0 2023-04-15 01:56:09.669736 cardano-nft-vending-machine-0.6.3/
--rw-rw-r--   0 thaddeusdiamond   (501) staff       (20)    11348 2022-06-01 02:40:16.000000 cardano-nft-vending-machine-0.6.3/LICENSE
--rw-rw-r--   0 thaddeusdiamond   (501) staff       (20)    13218 2023-04-15 01:56:09.669399 cardano-nft-vending-machine-0.6.3/PKG-INFO
--rw-rw-r--   0 thaddeusdiamond   (501) staff       (20)    12558 2023-04-01 01:43:17.000000 cardano-nft-vending-machine-0.6.3/README.md
--rw-rw-r--   0 thaddeusdiamond   (501) staff       (20)      960 2023-04-14 03:02:31.000000 cardano-nft-vending-machine-0.6.3/pyproject.toml
--rw-rw-r--   0 thaddeusdiamond   (501) staff       (20)       38 2023-04-15 01:56:09.669840 cardano-nft-vending-machine-0.6.3/setup.cfg
-drwxrwxr-x   0 thaddeusdiamond   (501) staff       (20)        0 2023-04-15 01:56:09.658271 cardano-nft-vending-machine-0.6.3/src/
-drwxrwxr-x   0 thaddeusdiamond   (501) staff       (20)        0 2023-04-15 01:56:09.660004 cardano-nft-vending-machine-0.6.3/src/cardano/
--rw-rw-r--   0 thaddeusdiamond   (501) staff       (20)        0 2022-06-01 02:40:43.000000 cardano-nft-vending-machine-0.6.3/src/cardano/__init__.py
-drwxrwxr-x   0 thaddeusdiamond   (501) staff       (20)        0 2023-04-15 01:56:09.662989 cardano-nft-vending-machine-0.6.3/src/cardano/wt/
--rw-rw-r--   0 thaddeusdiamond   (501) staff       (20)        0 2022-06-01 02:40:43.000000 cardano-nft-vending-machine-0.6.3/src/cardano/wt/__init__.py
--rw-rw-r--   0 thaddeusdiamond   (501) staff       (20)     4987 2023-02-15 06:22:29.000000 cardano-nft-vending-machine-0.6.3/src/cardano/wt/blockfrost.py
-drwxrwxr-x   0 thaddeusdiamond   (501) staff       (20)        0 2023-04-15 01:56:09.663956 cardano-nft-vending-machine-0.6.3/src/cardano/wt/bonuses/
--rw-rw-r--   0 thaddeusdiamond   (501) staff       (20)        0 2023-02-16 05:42:18.000000 cardano-nft-vending-machine-0.6.3/src/cardano/wt/bonuses/__init__.py
--rw-rw-r--   0 thaddeusdiamond   (501) staff       (20)      487 2023-02-16 05:42:18.000000 cardano-nft-vending-machine-0.6.3/src/cardano/wt/bonuses/bogo.py
--rw-rw-r--   0 thaddeusdiamond   (501) staff       (20)     2803 2022-10-04 18:29:05.000000 cardano-nft-vending-machine-0.6.3/src/cardano/wt/cardano_cli.py
--rw-rw-r--   0 thaddeusdiamond   (501) staff       (20)     5560 2023-03-09 19:37:45.000000 cardano-nft-vending-machine-0.6.3/src/cardano/wt/mint.py
--rw-rw-r--   0 thaddeusdiamond   (501) staff       (20)     9768 2023-04-13 20:07:17.000000 cardano-nft-vending-machine-0.6.3/src/cardano/wt/nft_vending_machine.py
--rw-rw-r--   0 thaddeusdiamond   (501) staff       (20)      838 2022-09-24 03:04:23.000000 cardano-nft-vending-machine-0.6.3/src/cardano/wt/utxo.py
-drwxrwxr-x   0 thaddeusdiamond   (501) staff       (20)        0 2023-04-15 01:56:09.666894 cardano-nft-vending-machine-0.6.3/src/cardano/wt/whitelist/
--rw-rw-r--   0 thaddeusdiamond   (501) staff       (20)        0 2022-09-24 03:04:23.000000 cardano-nft-vending-machine-0.6.3/src/cardano/wt/whitelist/__init__.py
--rw-rw-r--   0 thaddeusdiamond   (501) staff       (20)     4250 2023-03-31 02:08:34.000000 cardano-nft-vending-machine-0.6.3/src/cardano/wt/whitelist/asset_whitelist.py
--rw-rw-r--   0 thaddeusdiamond   (501) staff       (20)     2503 2023-03-31 02:08:34.000000 cardano-nft-vending-machine-0.6.3/src/cardano/wt/whitelist/filesystem.py
--rw-rw-r--   0 thaddeusdiamond   (501) staff       (20)     1140 2023-03-31 02:08:34.000000 cardano-nft-vending-machine-0.6.3/src/cardano/wt/whitelist/no_whitelist.py
--rw-rw-r--   0 thaddeusdiamond   (501) staff       (20)     4888 2023-03-31 02:08:34.000000 cardano-nft-vending-machine-0.6.3/src/cardano/wt/whitelist/wallet_whitelist.py
-drwxrwxr-x   0 thaddeusdiamond   (501) staff       (20)        0 2023-04-15 01:56:09.668886 cardano-nft-vending-machine-0.6.3/src/cardano_nft_vending_machine.egg-info/
--rw-rw-r--   0 thaddeusdiamond   (501) staff       (20)    13218 2023-04-15 01:56:09.000000 cardano-nft-vending-machine-0.6.3/src/cardano_nft_vending_machine.egg-info/PKG-INFO
--rw-rw-r--   0 thaddeusdiamond   (501) staff       (20)      772 2023-04-15 01:56:09.000000 cardano-nft-vending-machine-0.6.3/src/cardano_nft_vending_machine.egg-info/SOURCES.txt
--rw-rw-r--   0 thaddeusdiamond   (501) staff       (20)        1 2023-04-15 01:56:09.000000 cardano-nft-vending-machine-0.6.3/src/cardano_nft_vending_machine.egg-info/dependency_links.txt
--rw-rw-r--   0 thaddeusdiamond   (501) staff       (20)       53 2023-04-15 01:56:09.000000 cardano-nft-vending-machine-0.6.3/src/cardano_nft_vending_machine.egg-info/requires.txt
--rw-rw-r--   0 thaddeusdiamond   (501) staff       (20)        8 2023-04-15 01:56:09.000000 cardano-nft-vending-machine-0.6.3/src/cardano_nft_vending_machine.egg-info/top_level.txt
+drwxrwxr-x   0 thaddeusdiamond   (501) staff       (20)        0 2023-05-01 02:24:38.446302 cardano-nft-vending-machine-0.6.4/
+-rw-rw-r--   0 thaddeusdiamond   (501) staff       (20)    11348 2022-06-01 02:40:16.000000 cardano-nft-vending-machine-0.6.4/LICENSE
+-rw-rw-r--   0 thaddeusdiamond   (501) staff       (20)    13218 2023-05-01 02:24:38.446012 cardano-nft-vending-machine-0.6.4/PKG-INFO
+-rw-rw-r--   0 thaddeusdiamond   (501) staff       (20)    12558 2023-04-01 01:43:17.000000 cardano-nft-vending-machine-0.6.4/README.md
+-rw-rw-r--   0 thaddeusdiamond   (501) staff       (20)      960 2023-05-01 02:23:43.000000 cardano-nft-vending-machine-0.6.4/pyproject.toml
+-rw-rw-r--   0 thaddeusdiamond   (501) staff       (20)       38 2023-05-01 02:24:38.446392 cardano-nft-vending-machine-0.6.4/setup.cfg
+drwxrwxr-x   0 thaddeusdiamond   (501) staff       (20)        0 2023-05-01 02:24:38.439061 cardano-nft-vending-machine-0.6.4/src/
+drwxrwxr-x   0 thaddeusdiamond   (501) staff       (20)        0 2023-05-01 02:24:38.440181 cardano-nft-vending-machine-0.6.4/src/cardano/
+-rw-rw-r--   0 thaddeusdiamond   (501) staff       (20)        0 2022-06-01 02:40:43.000000 cardano-nft-vending-machine-0.6.4/src/cardano/__init__.py
+drwxrwxr-x   0 thaddeusdiamond   (501) staff       (20)        0 2023-05-01 02:24:38.442036 cardano-nft-vending-machine-0.6.4/src/cardano/wt/
+-rw-rw-r--   0 thaddeusdiamond   (501) staff       (20)        0 2022-06-01 02:40:43.000000 cardano-nft-vending-machine-0.6.4/src/cardano/wt/__init__.py
+-rw-rw-r--   0 thaddeusdiamond   (501) staff       (20)     4987 2023-02-15 06:22:29.000000 cardano-nft-vending-machine-0.6.4/src/cardano/wt/blockfrost.py
+drwxrwxr-x   0 thaddeusdiamond   (501) staff       (20)        0 2023-05-01 02:24:38.442619 cardano-nft-vending-machine-0.6.4/src/cardano/wt/bonuses/
+-rw-rw-r--   0 thaddeusdiamond   (501) staff       (20)        0 2023-02-16 05:42:18.000000 cardano-nft-vending-machine-0.6.4/src/cardano/wt/bonuses/__init__.py
+-rw-rw-r--   0 thaddeusdiamond   (501) staff       (20)      487 2023-02-16 05:42:18.000000 cardano-nft-vending-machine-0.6.4/src/cardano/wt/bonuses/bogo.py
+-rw-rw-r--   0 thaddeusdiamond   (501) staff       (20)     2803 2023-05-01 02:21:29.000000 cardano-nft-vending-machine-0.6.4/src/cardano/wt/cardano_cli.py
+-rw-rw-r--   0 thaddeusdiamond   (501) staff       (20)     5560 2023-05-01 02:21:29.000000 cardano-nft-vending-machine-0.6.4/src/cardano/wt/mint.py
+-rw-rw-r--   0 thaddeusdiamond   (501) staff       (20)     9769 2023-05-01 02:22:50.000000 cardano-nft-vending-machine-0.6.4/src/cardano/wt/nft_vending_machine.py
+-rw-rw-r--   0 thaddeusdiamond   (501) staff       (20)      838 2022-09-24 03:04:23.000000 cardano-nft-vending-machine-0.6.4/src/cardano/wt/utxo.py
+drwxrwxr-x   0 thaddeusdiamond   (501) staff       (20)        0 2023-05-01 02:24:38.444042 cardano-nft-vending-machine-0.6.4/src/cardano/wt/whitelist/
+-rw-rw-r--   0 thaddeusdiamond   (501) staff       (20)        0 2022-09-24 03:04:23.000000 cardano-nft-vending-machine-0.6.4/src/cardano/wt/whitelist/__init__.py
+-rw-rw-r--   0 thaddeusdiamond   (501) staff       (20)     4250 2023-03-31 02:08:34.000000 cardano-nft-vending-machine-0.6.4/src/cardano/wt/whitelist/asset_whitelist.py
+-rw-rw-r--   0 thaddeusdiamond   (501) staff       (20)     2503 2023-03-31 02:08:34.000000 cardano-nft-vending-machine-0.6.4/src/cardano/wt/whitelist/filesystem.py
+-rw-rw-r--   0 thaddeusdiamond   (501) staff       (20)     1140 2023-03-31 02:08:34.000000 cardano-nft-vending-machine-0.6.4/src/cardano/wt/whitelist/no_whitelist.py
+-rw-rw-r--   0 thaddeusdiamond   (501) staff       (20)     4888 2023-03-31 02:08:34.000000 cardano-nft-vending-machine-0.6.4/src/cardano/wt/whitelist/wallet_whitelist.py
+drwxrwxr-x   0 thaddeusdiamond   (501) staff       (20)        0 2023-05-01 02:24:38.445574 cardano-nft-vending-machine-0.6.4/src/cardano_nft_vending_machine.egg-info/
+-rw-rw-r--   0 thaddeusdiamond   (501) staff       (20)    13218 2023-05-01 02:24:38.000000 cardano-nft-vending-machine-0.6.4/src/cardano_nft_vending_machine.egg-info/PKG-INFO
+-rw-rw-r--   0 thaddeusdiamond   (501) staff       (20)      772 2023-05-01 02:24:38.000000 cardano-nft-vending-machine-0.6.4/src/cardano_nft_vending_machine.egg-info/SOURCES.txt
+-rw-rw-r--   0 thaddeusdiamond   (501) staff       (20)        1 2023-05-01 02:24:38.000000 cardano-nft-vending-machine-0.6.4/src/cardano_nft_vending_machine.egg-info/dependency_links.txt
+-rw-rw-r--   0 thaddeusdiamond   (501) staff       (20)       53 2023-05-01 02:24:38.000000 cardano-nft-vending-machine-0.6.4/src/cardano_nft_vending_machine.egg-info/requires.txt
+-rw-rw-r--   0 thaddeusdiamond   (501) staff       (20)        8 2023-05-01 02:24:38.000000 cardano-nft-vending-machine-0.6.4/src/cardano_nft_vending_machine.egg-info/top_level.txt
```

### Comparing `cardano-nft-vending-machine-0.6.3/LICENSE` & `cardano-nft-vending-machine-0.6.4/LICENSE`

 * *Files identical despite different names*

### Comparing `cardano-nft-vending-machine-0.6.3/PKG-INFO` & `cardano-nft-vending-machine-0.6.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cardano-nft-vending-machine
-Version: 0.6.3
+Version: 0.6.4
 Summary: Library to perform NFT mints automatically on the Cardano blockchain
 Project-URL: Documentation, https://thaddeusdiamond.github.io/cardano-nft-vending-machine/cardano/
 Project-URL: Source, https://github.com/thaddeusdiamond/cardano-nft-vending-machine
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: cardano-nft-vending-machine Version: 0.6.3 Summary:
+Metadata-Version: 2.1 Name: cardano-nft-vending-machine Version: 0.6.4 Summary:
 Library to perform NFT mints automatically on the Cardano blockchain Project-
 URL: Documentation, https://thaddeusdiamond.github.io/cardano-nft-vending-
 machine/cardano/ Project-URL: Source, https://github.com/thaddeusdiamond/
 cardano-nft-vending-machine Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License Classifier:
 Natural Language :: English Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3 Requires-Python: >=3.8
```

### Comparing `cardano-nft-vending-machine-0.6.3/README.md` & `cardano-nft-vending-machine-0.6.4/README.md`

 * *Files identical despite different names*

### Comparing `cardano-nft-vending-machine-0.6.3/pyproject.toml` & `cardano-nft-vending-machine-0.6.4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=62.3.2"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "cardano-nft-vending-machine"
-version = "0.6.3"
+version = "0.6.4"
 
 description = "Library to perform NFT mints automatically on the Cardano blockchain"
 readme = "README.md"
 classifiers = [
     "Intended Audience :: Developers",
     "License :: OSI Approved :: Apache Software License",
     "Natural Language :: English",
```

### Comparing `cardano-nft-vending-machine-0.6.3/src/cardano/wt/blockfrost.py` & `cardano-nft-vending-machine-0.6.4/src/cardano/wt/blockfrost.py`

 * *Files identical despite different names*

### Comparing `cardano-nft-vending-machine-0.6.3/src/cardano/wt/cardano_cli.py` & `cardano-nft-vending-machine-0.6.4/src/cardano/wt/cardano_cli.py`

 * *Files identical despite different names*

### Comparing `cardano-nft-vending-machine-0.6.3/src/cardano/wt/mint.py` & `cardano-nft-vending-machine-0.6.4/src/cardano/wt/mint.py`

 * *Files identical despite different names*

### Comparing `cardano-nft-vending-machine-0.6.3/src/cardano/wt/nft_vending_machine.py` & `cardano-nft-vending-machine-0.6.4/src/cardano/wt/nft_vending_machine.py`

 * *Files 0% similar despite different names*

```diff
@@ -52,15 +52,15 @@
         with open(metadata_file, 'r') as metadata_filehandle:
             policy_json = json.load(metadata_filehandle)['721'][self.mint.policy]
             return policy_json.keys()
 
     def __lock_and_merge(self, available_mints, num_mints, output_dir, locked_subdir, metadata_subdir, txn_id):
         combined_nft_metadata = {}
         for i in range(num_mints):
-            mint_metadata_filename = available_mints.pop()
+            mint_metadata_filename = available_mints.pop(0)
             mint_metadata_orig = os.path.join(self.mint.nfts_dir, mint_metadata_filename)
             with open(mint_metadata_orig, 'r') as mint_metadata_handle:
                 mint_metadata = json.load(mint_metadata_handle)
                 for nft_name, nft_metadata in mint_metadata['721'][self.mint.policy].items():
                     combined_nft_metadata[nft_name] = nft_metadata
             mint_metadata_locked = os.path.join(output_dir, locked_subdir, mint_metadata_filename)
             shutil.move(mint_metadata_orig, mint_metadata_locked)
```

### Comparing `cardano-nft-vending-machine-0.6.3/src/cardano/wt/utxo.py` & `cardano-nft-vending-machine-0.6.4/src/cardano/wt/utxo.py`

 * *Files identical despite different names*

### Comparing `cardano-nft-vending-machine-0.6.3/src/cardano/wt/whitelist/asset_whitelist.py` & `cardano-nft-vending-machine-0.6.4/src/cardano/wt/whitelist/asset_whitelist.py`

 * *Files identical despite different names*

### Comparing `cardano-nft-vending-machine-0.6.3/src/cardano/wt/whitelist/filesystem.py` & `cardano-nft-vending-machine-0.6.4/src/cardano/wt/whitelist/filesystem.py`

 * *Files identical despite different names*

### Comparing `cardano-nft-vending-machine-0.6.3/src/cardano/wt/whitelist/no_whitelist.py` & `cardano-nft-vending-machine-0.6.4/src/cardano/wt/whitelist/no_whitelist.py`

 * *Files identical despite different names*

### Comparing `cardano-nft-vending-machine-0.6.3/src/cardano/wt/whitelist/wallet_whitelist.py` & `cardano-nft-vending-machine-0.6.4/src/cardano/wt/whitelist/wallet_whitelist.py`

 * *Files identical despite different names*

### Comparing `cardano-nft-vending-machine-0.6.3/src/cardano_nft_vending_machine.egg-info/PKG-INFO` & `cardano-nft-vending-machine-0.6.4/src/cardano_nft_vending_machine.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cardano-nft-vending-machine
-Version: 0.6.3
+Version: 0.6.4
 Summary: Library to perform NFT mints automatically on the Cardano blockchain
 Project-URL: Documentation, https://thaddeusdiamond.github.io/cardano-nft-vending-machine/cardano/
 Project-URL: Source, https://github.com/thaddeusdiamond/cardano-nft-vending-machine
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: cardano-nft-vending-machine Version: 0.6.3 Summary:
+Metadata-Version: 2.1 Name: cardano-nft-vending-machine Version: 0.6.4 Summary:
 Library to perform NFT mints automatically on the Cardano blockchain Project-
 URL: Documentation, https://thaddeusdiamond.github.io/cardano-nft-vending-
 machine/cardano/ Project-URL: Source, https://github.com/thaddeusdiamond/
 cardano-nft-vending-machine Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License Classifier:
 Natural Language :: English Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3 Requires-Python: >=3.8
```

### Comparing `cardano-nft-vending-machine-0.6.3/src/cardano_nft_vending_machine.egg-info/SOURCES.txt` & `cardano-nft-vending-machine-0.6.4/src/cardano_nft_vending_machine.egg-info/SOURCES.txt`

 * *Files identical despite different names*

