# Comparing `tmp/koios-api-1.0.10.tar.gz` & `tmp/koios-api-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "koios-api-1.0.10.tar", last modified: Thu May 11 14:46:14 2023, max compression
+gzip compressed data, was "koios-api-1.0.2.tar", last modified: Sat Apr 22 10:16:55 2023, max compression
```

## Comparing `koios-api-1.0.10.tar` & `koios-api-1.0.2.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxrwxr-x   0 george    (1000) george    (1000)        0 2023-05-11 14:46:14.787757 koios-api-1.0.10/
--rw-rw-r--   0 george    (1000) george    (1000)     1080 2023-04-22 10:04:11.000000 koios-api-1.0.10/LICENSE
--rw-rw-r--   0 george    (1000) george    (1000)   106198 2023-05-11 14:46:14.787757 koios-api-1.0.10/PKG-INFO
--rw-rw-r--   0 george    (1000) george    (1000)   105559 2023-05-11 14:23:40.000000 koios-api-1.0.10/README.md
--rw-rw-r--   0 george    (1000) george    (1000)      795 2023-05-11 12:09:00.000000 koios-api-1.0.10/pyproject.toml
--rw-rw-r--   0 george    (1000) george    (1000)       38 2023-05-11 14:46:14.787757 koios-api-1.0.10/setup.cfg
-drwxrwxr-x   0 george    (1000) george    (1000)        0 2023-05-11 14:46:14.783757 koios-api-1.0.10/src/
-drwxrwxr-x   0 george    (1000) george    (1000)        0 2023-05-11 14:46:14.783757 koios-api-1.0.10/src/koios_api/
--rw-rw-r--   0 george    (1000) george    (1000)     1393 2023-05-11 12:12:45.000000 koios-api-1.0.10/src/koios_api/__config__.py
--rw-rw-r--   0 george    (1000) george    (1000)      228 2022-10-13 07:47:20.000000 koios-api-1.0.10/src/koios_api/__init__.py
--rw-rw-r--   0 george    (1000) george    (1000)    10489 2023-05-11 12:03:05.000000 koios-api-1.0.10/src/koios_api/account.py
--rw-rw-r--   0 george    (1000) george    (1000)     5649 2023-05-11 12:03:19.000000 koios-api-1.0.10/src/koios_api/address.py
--rw-rw-r--   0 george    (1000) george    (1000)    16024 2023-05-11 13:26:52.000000 koios-api-1.0.10/src/koios_api/asset.py
--rw-rw-r--   0 george    (1000) george    (1000)     3177 2023-05-11 12:03:49.000000 koios-api-1.0.10/src/koios_api/block.py
--rw-rw-r--   0 george    (1000) george    (1000)     2690 2023-05-11 08:51:55.000000 koios-api-1.0.10/src/koios_api/epoch.py
--rw-rw-r--   0 george    (1000) george    (1000)     2514 2023-05-11 08:41:06.000000 koios-api-1.0.10/src/koios_api/network.py
--rw-rw-r--   0 george    (1000) george    (1000)    10429 2023-05-11 12:04:12.000000 koios-api-1.0.10/src/koios_api/pool.py
--rw-rw-r--   0 george    (1000) george    (1000)     3595 2023-05-11 12:04:31.000000 koios-api-1.0.10/src/koios_api/script.py
--rw-rw-r--   0 george    (1000) george    (1000)     5414 2023-05-11 12:04:23.000000 koios-api-1.0.10/src/koios_api/transactions.py
-drwxrwxr-x   0 george    (1000) george    (1000)        0 2023-05-11 14:46:14.783757 koios-api-1.0.10/src/koios_api.egg-info/
--rw-rw-r--   0 george    (1000) george    (1000)   106198 2023-05-11 14:46:14.000000 koios-api-1.0.10/src/koios_api.egg-info/PKG-INFO
--rw-rw-r--   0 george    (1000) george    (1000)      490 2023-05-11 14:46:14.000000 koios-api-1.0.10/src/koios_api.egg-info/SOURCES.txt
--rw-rw-r--   0 george    (1000) george    (1000)        1 2023-05-11 14:46:14.000000 koios-api-1.0.10/src/koios_api.egg-info/dependency_links.txt
--rw-rw-r--   0 george    (1000) george    (1000)       17 2023-05-11 14:46:14.000000 koios-api-1.0.10/src/koios_api.egg-info/requires.txt
--rw-rw-r--   0 george    (1000) george    (1000)       16 2023-05-11 14:46:14.000000 koios-api-1.0.10/src/koios_api.egg-info/top_level.txt
+drwxrwxr-x   0 george    (1000) george    (1000)        0 2023-04-22 10:16:55.746351 koios-api-1.0.2/
+-rw-rw-r--   0 george    (1000) george    (1000)     1080 2023-04-22 10:04:11.000000 koios-api-1.0.2/LICENSE
+-rw-rw-r--   0 george    (1000) george    (1000)    91762 2023-04-22 10:16:55.746351 koios-api-1.0.2/PKG-INFO
+-rw-rw-r--   0 george    (1000) george    (1000)    91124 2022-12-28 16:12:38.000000 koios-api-1.0.2/README.md
+-rw-rw-r--   0 george    (1000) george    (1000)      794 2022-12-28 10:57:33.000000 koios-api-1.0.2/pyproject.toml
+-rw-rw-r--   0 george    (1000) george    (1000)       38 2023-04-22 10:16:55.746351 koios-api-1.0.2/setup.cfg
+drwxrwxr-x   0 george    (1000) george    (1000)        0 2023-04-22 10:16:55.742351 koios-api-1.0.2/src/
+drwxrwxr-x   0 george    (1000) george    (1000)        0 2023-04-22 10:16:55.742351 koios-api-1.0.2/src/koios_api/
+-rw-rw-r--   0 george    (1000) george    (1000)     1194 2022-12-11 21:55:43.000000 koios-api-1.0.2/src/koios_api/__config__.py
+-rw-rw-r--   0 george    (1000) george    (1000)      228 2022-10-13 07:47:20.000000 koios-api-1.0.2/src/koios_api/__init__.py
+-rw-rw-r--   0 george    (1000) george    (1000)     8947 2023-04-22 09:41:53.000000 koios-api-1.0.2/src/koios_api/account.py
+-rw-rw-r--   0 george    (1000) george    (1000)     4543 2023-04-22 09:42:17.000000 koios-api-1.0.2/src/koios_api/address.py
+-rw-rw-r--   0 george    (1000) george    (1000)     9922 2023-04-22 10:00:30.000000 koios-api-1.0.2/src/koios_api/asset.py
+-rw-rw-r--   0 george    (1000) george    (1000)     3083 2023-04-22 10:00:44.000000 koios-api-1.0.2/src/koios_api/block.py
+-rw-rw-r--   0 george    (1000) george    (1000)     2335 2023-04-22 09:24:27.000000 koios-api-1.0.2/src/koios_api/epoch.py
+-rw-rw-r--   0 george    (1000) george    (1000)     1922 2023-04-22 09:26:11.000000 koios-api-1.0.2/src/koios_api/network.py
+-rw-rw-r--   0 george    (1000) george    (1000)    10281 2023-04-22 10:02:08.000000 koios-api-1.0.2/src/koios_api/pool.py
+-rw-rw-r--   0 george    (1000) george    (1000)     3549 2023-04-22 10:02:30.000000 koios-api-1.0.2/src/koios_api/script.py
+-rw-rw-r--   0 george    (1000) george    (1000)     5338 2023-04-22 10:02:44.000000 koios-api-1.0.2/src/koios_api/transactions.py
+drwxrwxr-x   0 george    (1000) george    (1000)        0 2023-04-22 10:16:55.746351 koios-api-1.0.2/src/koios_api.egg-info/
+-rw-rw-r--   0 george    (1000) george    (1000)    91762 2023-04-22 10:16:55.000000 koios-api-1.0.2/src/koios_api.egg-info/PKG-INFO
+-rw-rw-r--   0 george    (1000) george    (1000)      490 2023-04-22 10:16:55.000000 koios-api-1.0.2/src/koios_api.egg-info/SOURCES.txt
+-rw-rw-r--   0 george    (1000) george    (1000)        1 2023-04-22 10:16:55.000000 koios-api-1.0.2/src/koios_api.egg-info/dependency_links.txt
+-rw-rw-r--   0 george    (1000) george    (1000)       17 2023-04-22 10:16:55.000000 koios-api-1.0.2/src/koios_api.egg-info/requires.txt
+-rw-rw-r--   0 george    (1000) george    (1000)       16 2023-04-22 10:16:55.000000 koios-api-1.0.2/src/koios_api.egg-info/top_level.txt
```

### Comparing `koios-api-1.0.10/LICENSE` & `koios-api-1.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `koios-api-1.0.10/PKG-INFO` & `koios-api-1.0.2/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: koios-api
-Version: 1.0.10
+Version: 1.0.2
 Summary: A python package for the Cardano Blockchain Koios API (https://api.koios.rest/)
 Author-email: APEX Stake Pool <cardanoapexpool@gmail.com>
 Project-URL: Homepage, https://github.com/cardano-apexpool/koios-api-python
 Project-URL: Bug Tracker, https://github.com/cardano-apexpool/koios-api-python/issues
 Keywords: koios,cardano,blockchain,REST,API
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
@@ -69,15 +69,14 @@
 
 ## Modules
 
 [Network](#Network)<br>
 [get_tip](#get_tip) Get the tip info about the latest block seen by chain<br>
 [get_genesis](#get_genesis) Get the Genesis parameters used to start specific era on chain<br>
 [get_totals](#get_totals) Get the circulating utxo, treasury, rewards, supply and reserves in lovelace for specified epoch, all epochs if empty<br>
-[get_param_updates](#get_param_updates) Get all parameter update proposals submitted to the chain starting Shelley era<br>
 
 [Epoch](#Epoch)<br>
 [get_epoch_info](#get_epoch_info) Get the epoch information, all epochs if no epoch specified<br>
 [get_epoch_params](#get_epoch_params) Get the protocol parameters for specific epoch, returns information about all epochs if no epoch specified<br>
 [get_epoch_block_protocols](#get_epoch_block_protocols) Get the information about block protocol distribution in epoch<br>
 
 [Block](#Block)<br>
@@ -92,29 +91,33 @@
 [get_tx_metalabels](#get_tx_metalabels) Get a list of all transaction metadata labels<br>
 [submit_tx](#submit_tx) Submit an already serialized transaction to the network<br>
 [get_tx_status](#get_tx_status) Get the number of block confirmations for a given transaction hash list<br>
 
 [Address](#Address)<br>
 [get_address_info](#get_address_info) Get the transaction hash list of input address array, optionally filtering after specified block height (inclusive)<br>
 [get_address_txs](#get_address_txs) Get the transaction hash list of input address array, optionally filtering after specified block height (inclusive)<br>
-[get_credential_utxos](#get_credential_utxos) Get a list of UTxO against input payment credential array including their balances<br>
 [get_address_assets](#get_address_assets) Get the list of all the assets (policy, name and quantity) for given addresses<br>
 [get_credential_txs](#get_credential_txs) Get the transaction hash list of input payment credential array, optionally filtering after specified block height (inclusive)<br>
 
+[Account](#Account)<br>
+[get_account_list](#get_account_list) Get a list of all accounts<br>
+[get_account_info](#get_account_info) Get the account information for given stake addresses (accounts)<br>
+[get_account_info_cached](#get_account_info_cached) Get the cached account information for given stake addresses (accounts)<br>
+[get_account_rewards](#get_account_rewards) Get the full rewards history (including MIR) for given stake addresses (accounts)<br>
+[get_account_updates](#get_account_updates) Get the account updates (registration, deregistration, delegation and withdrawals) for given stake addresses (accounts)<br>
+[get_account_addresses](#get_account_addresses) Get all addresses associated with given staking accounts<br>
+[get_account_assets](#get_account_assets) Get the native asset balance of given accounts<br>
+[get_account_history](#get_account_history) Get the staking history of given stake addresses (accounts)<br>
+
 [Asset](#Asset)<br>
 [get_asset_list](#get_asset_list) Get the list of all native assets (paginated)<br>
-[get_asset_token_registry](#get_asset_token_registry) Get a list of assets registered via token registry on github<br>
-[get_asset_addresses](#get_asset_addresses) Get the list of all addresses holding a given asset<br>
-[get_asset_nft_address](#get_asset_nft_address) Get the address where specified NFT currently reside on.<br>
+[get_asset_address_list](#get_asset_address_list) Get the list of all addresses holding a given asset<br>
 [get_asset_info](#get_asset_info) Get the information of an asset including first minting & token registry metadata<br>
-[get_asset_info_bulk](#get_asset_info_bulk) Get the information of a list of assets including first minting & token registry metadata<br>
 [get_asset_history](#get_asset_history) Get the mint/burn history of an asset<br>
-[get_policy_asset_addresses](#get_policy_asset_addresses) Get the list of addresses with quantity for each asset on the given policy<br>
-[get_policy_asset_info](#get_policy_asset_info) Get the information for all assets under the same policy<br>
-[get_policy_asset_list](#get_policy_asset_list) Get the list of asset under the given policy (including balances)<br>
+[get_asset_policy_info](#get_asset_policy_info) Get the information for all assets under the same policy<br>
 [get_asset_summary](#get_asset_summary) Get the summary of an asset (total transactions exclude minting/total wallets include only wallets with asset balance)<br>
 [get_asset_txs](#get_asset_txs) Get the list of all asset transaction hashes (the newest first)<br>
 
 [Pool](#Pool)<br>
 [get_pools_list](#get_pools_list) A list of all currently registered/retiring (not retired) pools<br>
 [get_pool_info](#get_pool_info) Current pool statuses and details for a specified list of pool ids<br>
 [get_pool_stake_snapshot](#get_pool_stake_snapshot) Returns Mark, Set and Go stake snapshots for the selected pool, useful for leaderlog calculation<br>
@@ -129,31 +132,20 @@
 
 [Script](#Script)<br>
 [get_native_script_list](#get_native_script_list) The list of all existing native script hashes along with their creation transaction hashes<br>
 [get_plutus_script_list](#get_plutus_script_list) The list of all existing native script hashes along with their creation transaction hashes<br>
 [get_script_redeemers](#get_script_redeemers) The list of all redeemers for a given script hash<br>
 [get_datum_info](#get_datum_info) The list of datum information for given datum hashes<br>
 
-[Stake Account](#Stake Account)<br>
-[get_account_list](#get_account_list) Get a list of all accounts<br>
-[get_account_info](#get_account_info) Get the account information for given stake addresses (accounts)<br>
-[get_account_utxos](#get_account_utxos) Get a list of all UTxOs for a given stake address (account)<br>
-[get_account_info_cached](#get_account_info_cached) Get the cached account information for given stake addresses (accounts)<br>
-[get_account_rewards](#get_account_rewards) Get the full rewards history (including MIR) for given stake addresses (accounts)<br>
-[get_account_updates](#get_account_updates) Get the account updates (registration, deregistration, delegation and withdrawals) for given stake addresses (accounts)<br>
-[get_account_addresses](#get_account_addresses) Get all addresses associated with given staking accounts<br>
-[get_account_assets](#get_account_assets) Get the native asset balance of given accounts<br>
-[get_account_history](#get_account_history) Get the staking history of given stake addresses (accounts)<br>
-
 ### Network
 
 #### get_tip
 Get the tip info about the latest block seen by chain<br>
 Parameters: none<br>
-Returns: The tip information as a list of one dictionary<br>
+Returns: The tip information as a list of one map<br>
 Example:<br>
 `tip = get_tip()`<br>
 Example response:
 ```json
 [
   {
     "hash": "442765ab5660346a6af3ba7667bbd35934e6219a52f0f53a80f28d27a70309c1",
@@ -165,15 +157,15 @@
   }
 ]
 ```
 
 #### get_genesis
 Get the Genesis parameters used to start specific era on chain<br>
 Parameters: none<br>
-Returns: Genesis parameters used to start each era on chain as a list of one dictionary<br>
+Returns: Genesis parameters used to start each era on chain as a list of one map<br>
 Example:<br>
 `genesis = get_genesis()`<br>
 Example response:
 ```json
 [
   {
     "networkmagic": "764824073",
@@ -191,15 +183,15 @@
   }
 ]
 ```
 
 #### get_totals
 Get the circulating utxo, treasury, rewards, supply and reserves in lovelace for specified epoch, all epochs if empty<br>
 Parameters: Epoch (optional)<br>
-Returns: Supply/reserves/utxo/fees/treasury stats as a list of one dictionary (if the epoch is specified) or a list of all available epochs (if the epoch parameter is not specified)<br>
+Returns: Supply/reserves/utxo/fees/treasury stats as a list of one map (if the epoch is specified) or a list of all available epochs (if the epoch parameter is not specified)<br>
 Example:<br>
 `totals = get_totals(380)`<br>
 Example response:
 ```json
 [
   {
     "epoch_no": 380,
@@ -208,50 +200,20 @@
     "reward": "635180192555825",
     "supply": "35230640457275590",
     "reserves": "9769359542724410"
   }
 ]
 ```
 
-#### get_param_updates
-Get all parameter update proposals submitted to the chain starting Shelley era<br>
-Parameters: none<br>
-Returns: All parameter update proposals<br>
-Example:<br>
-`param_updates = get_param_updates()`<br>
-```json
-[
-  {
-    "tx_hash": "b516588da34b58b7d32b6a057f513e16ea8c87de46615631be3316d8a8847d46",
-    "block_height": 4533644,
-    "block_time": 1596923351,
-    "epoch_no": 210,
-    "data": {
-      "decentralisation": 0.9
-    }
-  },
-  {
-    "tx_hash": "784902982af484f78d10f1587072f5a6b888ed0c1296d4ecf1e21c0251696ca1",
-    "block_height": 4558648,
-    "block_time": 1597425824,
-    "epoch_no": 211,
-    "data": {
-      "decentralisation": 0.8
-    }
-  },
-  ...
-]
-```
-
 ### Epoch
 
 #### get_epoch_info
 Get the epoch information, all epochs if no epoch specified<br>
 Parameters: Epoch (optional)<br>
-Returns: The list of epoch info dictionaries<br>
+Returns: The list of epoch info maps<br>
 Example:<br>
 `epoch_info = get_epoch_info(379)`<br>
 Example response:
 ```json
 [
   {
     "epoch_no": 379,
@@ -269,15 +231,15 @@
   }
 ]
 ```
 
 #### get_epoch_params
 Get the protocol parameters for specific epoch, returns information about all epochs if no epoch specified<br>
 Parameters: Epoch (optional)<br>
-Returns: The list of epoch protocol parameters dictionaries<br>
+Returns: The list of epoch protocol parameters maps<br>
 Example:<br>
 `epoch_params = get_epoch_params(380)`<br>
 Example response:
 ```json
 [
   {
     "epoch_no": 380,
@@ -315,15 +277,15 @@
   }
 ]
 ```
 
 #### get_epoch_block_protocols
 Get the information about block protocol distribution in epoch<br>
 Parameters: Epoch (optional)<br>
-Returns: The list of epoch protocol distribution dictionaries<br>
+Returns: The list of epoch protocol distribution maps<br>
 Example:<br>
 `epoch_block_protocols = get_epoch_block_protocols(380)`<br>
 Example response:
 ```json
 [
   {
     "proto_major": 7,
@@ -339,15 +301,15 @@
 ```
 
 ### Block
 
 #### get_blocks
 Get summarised details about all blocks (paginated - latest first)<br>
 Parameters: The maximum number of blocks to return<br>
-Returns: The list of block dictionaries (the newest first)<br>
+Returns: The list of block maps (the newest first)<br>
 Example:<br>
 `blocks = get_blocks(3)`<br>
 Example response:
 ```json
 [
   {
     "hash": "8e33bb588feff6414469779d724923064688615535280f8982c9981410cd06f6",
@@ -396,15 +358,15 @@
   }
 ]
 ```
 
 #### get_block_info
 Get detailed information about a specific block<br>
 Parameters: Block hash as string (for one block) or list of block hashes (for multiple blocks)<br>
-Returns: The list of block dictionaries<br>
+Returns: The list of block maps<br>
 Example:<br>
 `block_info = get_block_info('8e33bb588feff6414469779d724923064688615535280f8982c9981410cd06f6')`<br>
 Example response:
 ```json
 [
   {
     "hash": "8e33bb588feff6414469779d724923064688615535280f8982c9981410cd06f6",
@@ -429,15 +391,15 @@
   }
 ]
 ```
 
 #### get_block_txs
 Get a list of all transactions included in provided blocks<br>
 Parameters: Block(s) hash(es) as string (for one block) or list of block hashes (for multiple blocks)<br>
-Returns: The list of transaction dictionaries by block<br>
+Returns: The list of transaction maps by block<br>
 Example:<br>
 `block_txs = get_block_txs('8e33bb588feff6414469779d724923064688615535280f8982c9981410cd06f6')`<br>
 Example response:
 ```json
 [
   {
     "block_hash": "8e33bb588feff6414469779d724923064688615535280f8982c9981410cd06f6",
@@ -467,15 +429,15 @@
 ```
 
 ### Transactions
 
 #### get_tx_info
 Get detailed information about transaction(s)<br>
 Parameters: Transaction(s) hash(es) as a string (for one transaction) or list (for multiple transactions)<br>
-Returns: The list of transactions details dictionaries<br>
+Returns: The list of transactions details maps<br>
 Example:<br>
 `tx_info = get_tx_info('99f2aefba2a4a5a550aeed9d91d3adabe77a286ec45c345c7980a208364f76c6')`<br>
 Example response:
 ```json
 [
   {
     "tx_hash": "99f2aefba2a4a5a550aeed9d91d3adabe77a286ec45c345c7980a208364f76c6",
@@ -569,15 +531,15 @@
   }
 ]
 ```
 
 #### get_tx_utxos
 Get UTxO set (inputs/outputs) of transactions<br>
 Parameters: Transaction(s) hash(es) as a string (for one transaction) or list (for multiple transactions)<br>
-Returns: The list of transactions UTxOs dictionaries<br>
+Returns: The list of transactions UTxOs maps<br>
 Example:<br>
 `tx_utxos = get_tx_utxos('bf685dde61d36b8acd259b2bd00a69a2e8359d2a69b75aa3a0eff9d38ca1f2ef')`<br>
 Example response:
 ```json
 [
   {
     "tx_hash": "bf685dde61d36b8acd259b2bd00a69a2e8359d2a69b75aa3a0eff9d38ca1f2ef",
@@ -646,15 +608,15 @@
   }
 ]
 ```
 
 #### get_tx_metadata
 Get metadata information (if any) for given transaction(s)<br>
 Parameters: Transaction(s) hash(es) as a string (for one transaction) or list (for multiple transactions)<br>
-Returns: The list of transactions metadata dictionaries<br>
+Returns: The list of transactions metadata maps<br>
 Example:<br>
 `tx_metadata = get_tx_metadata('291b5533227331999eca2e63934c1061e5f85993e77747a90d9901413d7bb937')`<br>
 Example response:
 ```json
 [
   {
     "tx_hash": "291b5533227331999eca2e63934c1061e5f85993e77747a90d9901413d7bb937",
@@ -674,15 +636,15 @@
   }
 ]
 ```
 
 #### get_tx_metalabels
 Get a list of all transaction metadata labels<br>
 Parameters: none<br>
-Returns: The list of transaction metadata labels dictionaries<br>
+Returns: The list of transaction metadata labels maps<br>
 Example:<br>
 `tx_metalabels = get_tx_metalabels()`<br>
 Example response:
 ```json
 [
   {
     "key": "0"
@@ -722,15 +684,15 @@
 ```
 0eec38dc1d2d021f477a890d754e66c49fe74a9fd972793076587496c9850060
 ```
 
 #### get_tx_status
 Get the number of block confirmations for a given transaction hash list<br>
 Parameters: Transaction(s) hash(es) as a string (for one transaction) or list (for multiple transactions)<br>
-Returns: The list of transactions block confirmations dictionaries<br>
+Returns: The list of transactions block confirmations maps<br>
 Example:<br>
 `tx_status = get_tx_status('0eec38dc1d2d021f477a890d754e66c49fe74a9fd972793076587496c9850060')`<br>
 Example response:
 ```json
 [
   {
     "tx_hash": "0eec38dc1d2d021f477a890d754e66c49fe74a9fd972793076587496c9850060",
@@ -740,15 +702,15 @@
 ```
 
 ### Address
 
 #### get_address_info
 Get the transaction hash list of input address array, optionally filtering after specified block height (inclusive)<br>
 Parameters: Payment address(es) as string (for one address) or list (for multiple addresses)<br>
-Returns: The list of transactions dictionaries<br>
+Returns: The list of transactions maps<br>
 Example:<br>
 `address_info = get_address_info('addr1q8wv876ptu0qhujmh2awdcnpcc0ctgdz8e8qvv29k8hucwft99azzjfn9l2658p483uljfdd00ef5rzg58y5km6gj9jqcp0ws7')`<br>
 Example response:
 ```json
 [
   {
     "address": "addr1q8wv876ptu0qhujmh2awdcnpcc0ctgdz8e8qvv29k8hucwft99azzjfn9l2658p483uljfdd00ef5rzg58y5km6gj9jqcp0ws7",
@@ -771,15 +733,15 @@
   }
 ]
 ```
 
 #### get_address_txs
 Get the transaction hash list of input address array, optionally filtering after specified block height (inclusive)<br>
 Parameters: Payment address(es) as string (for one address) or list (for multiple addresses)<br>
-Returns: The list of transactions dictionaries<br>
+Returns: The list of transactions maps<br>
 Example:<br>
 `address_txs = get_address_txs('addr1q8wv876ptu0qhujmh2awdcnpcc0ctgdz8e8qvv29k8hucwft99azzjfn9l2658p483uljfdd00ef5rzg58y5km6gj9jqcp0ws7')`<br>
 Example response:
 ```json
 [
   {
     "tx_hash": "c626fe027d09db2b6c63ba67e3638911ff70e3b691a7e5c03e75c0d3a168c973",
@@ -805,61 +767,18 @@
     "epoch_no": 373,
     "block_height": 7971352,
     "block_time": 1667570778
   }
 ]
 ```
 
-#### get_credential_utxos
-Get a list of UTxO against input payment credential array including their balances<br>
-Parameters: Payment credential(s) as string (for one credential) or list (for multiple credentials)<br>
-Returns: The list of UTxO against input payment credential array including their balances<br>
-Example:<br>
-`credential_utxos = get_credential_utxos('0c35748e147183cd784875e78a5b372fa6975e9ac6406d6015c09bac')`<br>
-Example response:<br>
-```json
-[
-  {
-    "tx_hash": "8e9b85284f92ad85416d4fb0a3ff5d3bbd9b57c4a4d97a8d39dc99316eace0cf",
-    "tx_index": 0,
-    "value": "5000000"
-  },
-  {
-    "tx_hash": "e7333c01d3c2887767aca13e5c74fb858fbf0119cd90d944869ee72b8b81f523",
-    "tx_index": 1,
-    "value": "20432286"
-  },
-  {
-    "tx_hash": "ecfbbc335ec203b10ee65faddf06fb0ceac27c36ef3a76047fbf820f6e9ed7f2",
-    "tx_index": 2,
-    "value": "2301540"
-  },
-  {
-    "tx_hash": "b70a9107a38e776c0b1d94a1578c393a1ce01ea8e28ed56c5c724a2639e31bfe",
-    "tx_index": 2,
-    "value": "1150770"
-  },
-  {
-    "tx_hash": "1107afdada22f259aa798de57ca3839e212e977467628c85315326917a13dd3b",
-    "tx_index": 2,
-    "value": "1150770"
-  },
-  ...
-  {
-    "tx_hash": "b9d519ff9309dd78a7e8031aef2fa6b21358478efed5f0bdf234fa10c83eede7",
-    "tx_index": 1,
-    "value": "137666866"
-  }
-]
-```
-
 #### get_address_assets
 Get the list of all the assets (policy, name and quantity) for given addresses<br>
 Parameters: Payment address(es) as string (for one address) or list (for multiple addresses)<br>
-Returns: The list of assets dictionaries by address<br>
+Returns: The list of assets maps by address<br>
 Example:<br>
 `address_assets = get_address_assets('addr1qywp2795uk4uusknpseu3fcwy8ew57dnuaeutnxaa5j6ulp4u2anham4xet066yjc6xjxcymujvvwlfhj8k8gxfl2nvs73rvzh')`<br>
 Example response:
 ```json
 [
   {
     "address": "addr1qywp2795uk4uusknpseu3fcwy8ew57dnuaeutnxaa5j6ulp4u2anham4xet066yjc6xjxcymujvvwlfhj8k8gxfl2nvs73rvzh",
@@ -887,15 +806,15 @@
   }
 ]
 ```
 
 #### get_credential_txs
 Get the transaction hash list of input payment credential array, optionally filtering after specified block height (inclusive)<br>
 Parameters: Credential(s) as string (for one credential) or list (for multiple credentials)<br>
-Returns: The list of address information dictionaries<br>
+Returns: The list of address information maps<br>
 Example:<br>
 `credential_txs = get_credential_txs('dcc3fb415f1e0bf25bbabae6e261c61f85a1a23e4e063145b1efcc39')`<br>
 Example response:
 ```json
 [
   {
     "tx_hash": "c626fe027d09db2b6c63ba67e3638911ff70e3b691a7e5c03e75c0d3a168c973",
@@ -915,23 +834,268 @@
     "epoch_no": 373,
     "block_height": 7971352,
     "block_time": 1667570778
   }
 ]
 ```
 
+### Account
+
+#### get_account_list
+Get a list of all accounts<br>
+Parameters:<br>
+The offset (optional) to start from, default 0<br>
+The maximum number of accounts to return (optional), default 0 (no limit)<br>
+Returns: The list of accounts maps<br>
+This takes a very long time to execute (about one hour), because the total number of accounts is in the millions range.<br>
+Example:<br>
+`account_list = get_account_list()`<br>
+Example response:
+```json
+[
+  {
+    "id": "stake1uyfmzu5qqy70a8kq4c8rw09q0w0ktfcxppwujejnsh6tyrg5c774g"
+  },
+  {
+    "id": "stake1uydhlh7f2kkw9eazct5zyzlrvj32gjnkmt2v5qf6t8rut4qwch8ey"
+  },
+  {
+    "id": "stake1uxsgkz6fvgws5wn80vckwvghzapnhfmf0672nmmkm2tt9fcaau5sw"
+  },
+  ...
+]
+```
+
+#### get_account_info
+Get the account information for given stake addresses (accounts)<br>
+Parameters: Stake address(es), as a string (for one address) or a list (for multiple addresses)<br>
+Returns: The list of account information maps<br>
+Example:<br>
+`account_info = get_account_info('stake1uy4jj73pfyejl4d2rs6nc70eykkhhu56p3y2rj2tdayfzeqnjyh0j')`<br>
+Example response:
+```json
+[
+  {
+    "stake_address": "stake1uy4jj73pfyejl4d2rs6nc70eykkhhu56p3y2rj2tdayfzeqnjyh0j",
+    "status": "registered",
+    "delegated_pool": "pool18r2y72aue5nmv489xtnfxl36vzusq95qst6urd87yd5hgzms04c",
+    "total_balance": "20418617",
+    "utxo": "20418617",
+    "rewards": "0",
+    "withdrawals": "0",
+    "rewards_available": "0",
+    "reserves": "0",
+    "treasury": "0"
+  }
+]
+```
+
+#### get_account_info_cached
+Get the cached account information for given stake addresses (accounts)<br>
+Parameters: Stake address(es), as a string (for one address) or a list (for multiple addresses)<br>
+Returns: The list of account information maps<br>
+Example:<br>
+`account_info_cached = get_account_info_cached('stake1uy4jj73pfyejl4d2rs6nc70eykkhhu56p3y2rj2tdayfzeqnjyh0j')`<br>
+Example response:
+```json
+[
+  {
+    "stake_address": "stake1uy4jj73pfyejl4d2rs6nc70eykkhhu56p3y2rj2tdayfzeqnjyh0j",
+    "status": "registered",
+    "delegated_pool": "pool18r2y72aue5nmv489xtnfxl36vzusq95qst6urd87yd5hgzms04c",
+    "total_balance": "20418617",
+    "utxo": "20418617",
+    "rewards": "0",
+    "withdrawals": "0",
+    "rewards_available": "0",
+    "reserves": "0",
+    "treasury": "0"
+  }
+]
+```
+
+#### get_account_rewards
+Get the full rewards history (including MIR) for given stake addresses (accounts)<br>
+Parameters:<br>
+Stake address(es), as a string (for one address) or a list (for multiple addresses)<br>
+Epoch (optional), default: current epoch<br>
+Returns: The list of rewards maps by account (stake address)<br>
+Example:<br>
+`account_rewards = get_account_rewards('stake1u8lhspu67x3jejzcfrh487rtu3hnm26cg0jsn0mgh2y6n9q9ve26z')`<br>
+Example response:
+```json
+[
+  {
+    "stake_address": "stake1u8lhspu67x3jejzcfrh487rtu3hnm26cg0jsn0mgh2y6n9q9ve26z",
+    "rewards": [
+      {
+        "earned_epoch": 233,
+        "spendable_epoch": 235,
+        "amount": "3990414",
+        "type": "member",
+        "pool_id": "pool1jdhjfcu34lq88rypdtslzwyf27uh0h3apcr9mjd68zhc69r29fy"
+      },
+      {
+        "earned_epoch": 234,
+        "spendable_epoch": 236,
+        "amount": "2792902",
+        "type": "member",
+        "pool_id": "pool1jdhjfcu34lq88rypdtslzwyf27uh0h3apcr9mjd68zhc69r29fy"
+      },
+      ...
+      {
+        "earned_epoch": 379,
+        "spendable_epoch": 381,
+        "amount": "6496870",
+        "type": "member",
+        "pool_id": "pool12wpfng6cu7dz38yduaul3ngfm44xhv5xmech68m5fwe4wu77udd"
+      }
+    ]
+  }
+]
+```
+
+#### get_account_updates
+Get the account updates (registration, deregistration, delegation and withdrawals) for given stake addresses (accounts)<br>
+Parameters: Stake address(es), as a string (for one address) or a list (for multiple addresses)<br>
+Returns: The list of account updates maps by account (stake address)<br>
+Example:<br>
+`account_updates = get_account_updates('stake1u8lhspu67x3jejzcfrh487rtu3hnm26cg0jsn0mgh2y6n9q9ve26z')`<br>
+Example response:
+```json
+[
+  {
+    "stake_address": "stake1u8lhspu67x3jejzcfrh487rtu3hnm26cg0jsn0mgh2y6n9q9ve26z",
+    "updates": [
+      {
+        "action_type": "withdrawal",
+        "tx_hash": "487bc75f00fe934dad33683271cca8540fe868eef7025962678f179a1a111ecc",
+        "epoch_no": 324,
+        "epoch_slot": 70687,
+        "absolute_slot": 54675487,
+        "block_time": 1646241778
+      },
+      {
+        "action_type": "withdrawal",
+        "tx_hash": "eb3ffa01f434e210716151fd9001af82529e371a91c20af02512942f988a2119",
+        "epoch_no": 269,
+        "epoch_slot": 339679,
+        "absolute_slot": 31184479,
+        "block_time": 1622750770
+      },
+      ...
+      {
+        "action_type": "withdrawal",
+        "tx_hash": "b056dcbff9b908e1bd3ed015466f64486538058ba3553dbf885b216d88343370",
+        "epoch_no": 252,
+        "epoch_slot": 58375,
+        "absolute_slot": 23559175,
+        "block_time": 1615125466
+      }
+    ]
+  }
+]
+```
+
+#### get_account_addresses
+Get all addresses associated with given staking accounts<br>
+Parameters: Stake address(es), as a string (for one address) or a list (for multiple addresses)<br>
+Returns: The list of addresses maps by account (stake address)<br>
+Example:<br>
+`account_addresses = get_account_addresses('stake1u8lhspu67x3jejzcfrh487rtu3hnm26cg0jsn0mgh2y6n9q9ve26z')`<br>
+Example response:
+```json
+[
+  {
+    "stake_address": "stake1u8lhspu67x3jejzcfrh487rtu3hnm26cg0jsn0mgh2y6n9q9ve26z",
+    "addresses": [
+      "addr1qxwjxvzv8rmyutcjp0647w4n05wv7aez9jdmqcxn8a9sshll0qre4udr9ny9sj8020uxher08k44ssl9pxlk3w5f4x2qjyz9yf"
+    ]
+  }
+]
+```
+
+#### get_account_assets
+Get the native asset balance of given accounts<br>
+Parameters: Stake address(es), as a string (for one address) or a list (for multiple addresses)<br>
+Returns: The list of account assets maps by account (stake address)<br>
+Example:<br>
+`account_assets = get_account_assets('stake1u8lhspu67x3jejzcfrh487rtu3hnm26cg0jsn0mgh2y6n9q9ve26z')`<br>
+Example response:
+```json
+[
+  {
+    "stake_address": "stake1u8lhspu67x3jejzcfrh487rtu3hnm26cg0jsn0mgh2y6n9q9ve26z",
+    "asset_list": [
+      {
+        "policy_id": "0029cb7c88c7567b63d1a512c0ed626aa169688ec980730c0473b913",
+        "asset_name": "6c70202302",
+        "fingerprint": "asset1awuysx8hc686uz0dykmvmc7jfut2ulceucf6yc",
+        "quantity": "418089787"
+      },
+      {
+        "policy_id": "0029cb7c88c7567b63d1a512c0ed626aa169688ec980730c0473b913",
+        "asset_name": "6c7020f302",
+        "fingerprint": "asset1mcq0awl6awlaqg0ywukf94q0mnau263l9rght5",
+        "quantity": "586811406"
+      },
+      ...
+      {
+        "policy_id": "ea2d23f1fa631b414252824c153f2d6ba833506477a929770a4dd9c2",
+        "asset_name": "4d414442554c",
+        "fingerprint": "asset1q0kwjy669gmsqpvxp4lr0sp26pdm0dafme3qp2",
+        "quantity": "500"
+      }
+    ]
+  }
+]
+```
+
+#### get_account_history
+Get the staking history of given stake addresses (accounts)<br>
+Parameters: Stake address(es), as a string (for one address) or a list (for multiple addresses)<br>
+Returns: The list of staking history maps by account (stake address)<br>
+Example:<br>
+`account_history = get_account_history('stake1u8lhspu67x3jejzcfrh487rtu3hnm26cg0jsn0mgh2y6n9q9ve26z')`<br>
+Example response:
+```json
+[
+  {
+    "stake_address": "stake1u8lhspu67x3jejzcfrh487rtu3hnm26cg0jsn0mgh2y6n9q9ve26z",
+    "history": [
+      {
+        "pool_id": "pool1jdhjfcu34lq88rypdtslzwyf27uh0h3apcr9mjd68zhc69r29fy",
+        "epoch_no": 233,
+        "active_stake": "4655706122"
+      },
+      {
+        "pool_id": "pool1jdhjfcu34lq88rypdtslzwyf27uh0h3apcr9mjd68zhc69r29fy",
+        "epoch_no": 234,
+        "active_stake": "5020706122"
+      },
+      ...
+      {
+        "pool_id": "pool12wpfng6cu7dz38yduaul3ngfm44xhv5xmech68m5fwe4wu77udd",
+        "epoch_no": 381,
+        "active_stake": "10247851319"
+      }
+    ]
+  }
+]
+```
+
 ### Asset
 
 #### get_asset_list
 Get the list of all native assets (paginated)<br>
 Parameters:<br>
 Asset Policy (optional), default: all policies<br>
 The offset (optional) to start from, default 0<br>
 The maximum number of accounts to return (optional), default 0 (no limit)<br>
-Returns: The list of assets dictionaries by policy<br>
+Returns: The list of assets maps by policy<br>
 Example:<br>
 `asset_list = get_asset_list()`<br>
 Example response:
 ```json
 [
   {
     "policy_id": "00000002df633853f6a47465c9496721d2d5b1291b8398016c0e87ae",
@@ -949,98 +1113,38 @@
     "asset_name": "43726565707942616c6c7a57316231303137",
     "fingerprint": "asset12dvnasghksl5k7w696nd5t692j6myexapwjh0d"
   },
   ...
 ]
 ```
 
-#### get_asset_token_registry
-Get a list of assets registered via token registry on github<br>
-Parameters: none<br>
-Returns: The list of assets registered via token registry on github<br>
-Example:<br>
-`asset_token_registry = get_asset_token_registry()`<br>
-Example response:<br>
-```json
-[
-  {
-    "policy_id": "00000002df633853f6a47465c9496721d2d5b1291b8398016c0e87ae",
-    "asset_name": "6e7574636f696e",
-    "asset_name_ascii": "nutcoin",
-    "ticker": "NUT",
-    "description": "The legendary Nutcoin, the first native asset minted on Cardano.",
-    "url": "https://fivebinaries.com/nutcoin",
-    "decimals": 0,
-    "logo": "iVBORw0KGgoAAAANSUhEUgAAAGQA....2rCPgau2EAAAAASUVORK5CYII="
-  },
-  {
-    "policy_id": "00109530994ea381c0bfe0936c85ea01bfe2765c24ef6dad5740c33e",
-    "asset_name": "486f646c657220436f616c6974696f6e20436f696e",
-    "asset_name_ascii": "Hodler Coalition Coin",
-    "ticker": "HODLR",
-    "description": "Stake ₳DA with the Hodler Coalition. Save the World.",
-    "url": "https://www.hodlerstaking.com/",
-    "decimals": 4,
-    "logo": "iVBORw0KGgoAAAANSUhEUgAAARAAA...4RtRz5t2G8zAAAAAElFTkSuQmCC"
-  },
-  {
-    "policy_id": "0011fbab202151eca9e9ef7680569d9419d12e51e693cb05a2edd2ed",
-    "asset_name": "4341524b",
-    "asset_name_ascii": "Cardano Ark Token",
-    "ticker": "CARK",
-    "description": "Utility token for the Cardano Ark",
-    "url": "https://www.cardanoark.com/",
-    "decimals": 0,
-    "logo": ""
-  },
-  ...
-]
-```
-
-#### get_asset_addresses
+#### get_asset_address_list
 Get the list of all addresses holding a given asset<br>
 Parameters:<br>
 Asset Policy<br>
 Asset Name in hexadecimal format (optional), default: all policy assets<br>
-Returns: List of dictionaries with the wallets holding the asset and the amount of assets per wallet<br>
+Returns: List of maps with the wallets holding the asset and the amount of assets per wallet<br>
 Example:<br>
 `asset_address_list = get_asset_address_list('07697e6ca1e21777ac76f26d0779c53f7d08e47b9e32d23bd8fed9cd', '4379626572696130363936')`<br>
 Example response:
 ```json
 [
   {
     "payment_address": "addr1qywp2795uk4uusknpseu3fcwy8ew57dnuaeutnxaa5j6ulp4u2anham4xet066yjc6xjxcymujvvwlfhj8k8gxfl2nvs73rvzh",
     "quantity": "1"
   }
 ]
 ```
 
-#### get_asset_nft_address
-Get the address where specified NFT currently reside on.<br>
-Parameters:<br>
-Asset Policy<br>
-Asset Name in hexadecimal format<br>
-Returns: The wallet address holding the NFT as a list of one dictionary<br>
-Example:<br>
-`asset_nft_address = get_asset_nft_address('07697e6ca1e21777ac76f26d0779c53f7d08e47b9e32d23bd8fed9cd', '4379626572696130363936')`<br>
-Example response:
-```json
-[
-  {
-    "payment_address": "addr1qywp2795uk4uusknpseu3fcwy8ew57dnuaeutnxaa5j6ulp4u2anham4xet066yjc6xjxcymujvvwlfhj8k8gxfl2nvs73rvzh"
-  }
-]
-```
-
 #### get_asset_info
 Get the information of an asset including first minting & token registry metadata<br>
 Parameters:
 Asset Policy<br>
 Asset Name in hexadecimal format (optional), default: all policy assets<br>
-Returns: List of dictionaries with the wallets holding the asset and the amount of assets per wallet<br>
+Returns: List of maps with the wallets holding the asset and the amount of assets per wallet<br>
 Example:<br>
 `asset_info = get_asset_info('07697e6ca1e21777ac76f26d0779c53f7d08e47b9e32d23bd8fed9cd', '4379626572696130363936')`<br>
 Example response:
 ```json
 [
   {
     "policy_id": "07697e6ca1e21777ac76f26d0779c53f7d08e47b9e32d23bd8fed9cd",
@@ -1088,97 +1192,20 @@
       }
     },
     "token_registry_metadata": null
   }
 ]
 ```
 
-#### get_asset_info_bulk
-Get the information of a list of assets including first minting & token registry metadata<br>
-Parameters:<br>
-Assets List in tge following format: `['policy.name_hex']`<br>
-Returns: List of assets including first minting & token registry metadata<br>
-Example:<br>
-`asset_info_bulk = get_asset_info_bulk(['221b1b9ebccab1512262347491557279ac0afac63b4fbd10fc596c8a.437562656e7369734d757368726f6f6d', '221b1b9ebccab1512262347491557279ac0afac63b4fbd10fc596c8a.417a7a69654d757368726f6f6d'])`<br>
-Example response:
-```json
-[
-  {
-    "policy_id": "221b1b9ebccab1512262347491557279ac0afac63b4fbd10fc596c8a",
-    "asset_name": "437562656e7369734d757368726f6f6d",
-    "asset_name_ascii": "CubensisMushroom",
-    "fingerprint": "asset1csgmd2qwycgmqdck4dgqzzwm7xclhkqrhxs2pw",
-    "minting_tx_hash": "c29fd9f0c71793eb06e7cf055e8529740b0486a802b8e9019df4853c6dec03a0",
-    "total_supply": "7576",
-    "mint_cnt": 1,
-    "burn_cnt": 0,
-    "creation_time": 1680393600,
-    "minting_tx_metadata": {
-      "721": {
-        "version": "1.0",
-        "221b1b9ebccab1512262347491557279ac0afac63b4fbd10fc596c8a": {
-          "CubensisMushroom": {
-            "name": "CubensisMushroom",
-            "files": [
-              {
-                "src": "ipfs://QmQNTa19H5WnYtRiHqzNK2drC9rRTzmkxtu7tS57WZkNuZ",
-                "name": "Cubensis",
-                "mediaType": "image/png"
-              }
-            ],
-            "image": "ipfs://QmQNTa19H5WnYtRiHqzNK2drC9rRTzmkxtu7tS57WZkNuZ",
-            "project": "Chilled Kongs",
-            "mediaType": "image/png"
-          }
-        }
-      }
-    },
-    "token_registry_metadata": null
-  },
-  {
-    "policy_id": "221b1b9ebccab1512262347491557279ac0afac63b4fbd10fc596c8a",
-    "asset_name": "417a7a69654d757368726f6f6d",
-    "asset_name_ascii": "AzzieMushroom",
-    "fingerprint": "asset1kfskmlcvlsvpvr093staxj2788qlrkcrssf26a",
-    "minting_tx_hash": "e4b94e3a5e95953acfb50e3c2fd005b2839ca79c4294b62bbf7d2afdf96dd009",
-    "total_supply": "1305",
-    "mint_cnt": 1,
-    "burn_cnt": 0,
-    "creation_time": 1680393600,
-    "minting_tx_metadata": {
-      "721": {
-        "version": "1.0",
-        "221b1b9ebccab1512262347491557279ac0afac63b4fbd10fc596c8a": {
-          "AzzieMushroom": {
-            "name": "AzzieMushroom",
-            "files": [
-              {
-                "src": "ipfs://QmeAdLCKgXhxtDAcpPq5vgpRCqYWCGFMzb9jx4YEif3nWR",
-                "name": "Azzie",
-                "mediaType": "image/png"
-              }
-            ],
-            "image": "ipfs://QmeAdLCKgXhxtDAcpPq5vgpRCqYWCGFMzb9jx4YEif3nWR",
-            "project": "Chilled Kongs",
-            "mediaType": "image/png"
-          }
-        }
-      }
-    },
-    "token_registry_metadata": null
-  }
-]
-```
-
 #### get_asset_history
 Get the mint/burn history of an asset<br>
 Parameters:<br>
 Asset Policy<br>
 Asset Name in hexadecimal format (optional), default: all policy assets<br>
-Returns: List of dictionaries with the mint/burn history of an asset<br>
+Returns: List of maps with the mint/burn history of an asset<br>
 Example:<br>
 `asset_history = get_asset_history('07697e6ca1e21777ac76f26d0779c53f7d08e47b9e32d23bd8fed9cd', '4379626572696130363936')`<br>
 Example response:
 ```json
 [
   {
     "policy_id": "07697e6ca1e21777ac76f26d0779c53f7d08e47b9e32d23bd8fed9cd",
@@ -1229,49 +1256,20 @@
         ]
       }
     ]
   }
 ]
 ```
 
-#### get_policy_asset_addresses
-Get the list of addresses with quantity for each asset on the given policy<br>
-Parameters: Asset Policy<br>
-Returns: List of addresses with quantity for each asset on the given policy<br>
-Example:<br>
-`asset_policy_info = get_policy_asset_addresses('07697e6ca1e21777ac76f26d0779c53f7d08e47b9e32d23bd8fed9cd')`<br>
-Example response:
-```json
-[
-  {
-    "asset_name": "4379626572696130303233",
-    "payment_address": "addr1qxu5vk5xafdp39d95ya06d6uya8ldua7crpdzd2an07uw8mrtndmfr0d4qarvgj2wasdwlvrnlqt262jn5asnws7aekssq73gf",
-    "quantity": "1"
-  },
-  {
-    "asset_name": "4379626572696130303330",
-    "payment_address": "addr1q9wj7ylly5nz2kel6huy966tcsw2l3ct9at7m3euhfxyv246nlp3dj9pda2rphtzycwexsaapyk73k25y3j5neyhg45s879sk4",
-    "quantity": "1"
-  },
-  ...
-  {
-    "asset_name": "4379626572696132383338",
-    "payment_address": "addr1qxg2l50ryn6z23543v6nujvkql9zwj7f7hvsjwalw6jvf25n5k332a42ge9w5en95g9af59fft32g0la0qtfr9vfyyesccney2",
-    "quantity": "1"
-  }
-]
-```
-
-
-#### get_policy_asset_info
-Get the list of asset under the given policy (including balances)<br>
+#### get_asset_policy_info
+Get the information for all assets under the same policy<br>
 Parameters: Asset Policy<br>
-Returns: List of dictionaries with the policy assets<br>
+Returns: List of maps with the policy assets<br>
 Example:<br>
-`asset_policy_info = get_policy_asset_info('07697e6ca1e21777ac76f26d0779c53f7d08e47b9e32d23bd8fed9cd')`<br>
+`asset_policy_info = get_asset_policy_info('07697e6ca1e21777ac76f26d0779c53f7d08e47b9e32d23bd8fed9cd')`<br>
 Example response:
 ```json
 [
   {
     "asset_name": "",
     "asset_name_ascii": "",
     "fingerprint": "asset1pht97cylpt7azuu9mwhmd9c9zdgmumwrrm5yrc",
@@ -1405,127 +1403,20 @@
     "token_registry_metadata": null,
     "total_supply": "1",
     "creation_time": 1670493734
   }
 ]
 ```
 
-#### get_policy_asset_list
-Get the list of asset under the given policy (including balances)<br>
-Parameters: Asset Policy<br>
-Returns: List of dictionaries with the asset under the given policy<br>
-Example:<br>
-`asset_policy_list = get_policy_asset_list('07697e6ca1e21777ac76f26d0779c53f7d08e47b9e32d23bd8fed9cd')`<br>
-Example response:
-```json
-[
-  {
-    "asset_name": "",
-    "asset_name_ascii": "",
-    "fingerprint": "asset1pht97cylpt7azuu9mwhmd9c9zdgmumwrrm5yrc",
-    "minting_tx_hash": "90415fda215ff5098d7fa1385c7358c589066332068b720380726e3ef0b26de4",
-    "total_supply": "0",
-    "mint_cnt": 1,
-    "burn_cnt": 1,
-    "creation_time": 1665100800,
-    "minting_tx_metadata": {
-      "777": {
-        "addr": [
-          "addr1qy36jns6h4w4f80u6xed49k6qn9c7tk4x4us5kaxztjq8x3un2me8nvc5ke",
-          "gvll0gnwlj2ypzfhhqpns47u76gafttmq208x4d"
-        ],
-        "rate": "0.05"
-      }
-    },
-    "token_registry_metadata": null
-  },
-  ...
-  {
-    "asset_name": "4379626572696130333939",
-    "asset_name_ascii": "Cyberia0399",
-    "fingerprint": "asset1g7tgq2ly8uhtzcz79uhay8tq46h9rq62arfm8s",
-    "minting_tx_hash": "98db0a36106a92149b256887f6300f2b228e14d24d488e4b1614920083cd64ff",
-    "total_supply": "1",
-    "mint_cnt": 1,
-    "burn_cnt": 0,
-    "creation_time": 1665187200,
-    "minting_tx_metadata": {
-      "721": {
-        "nonce": "c966f455d3e03537",
-        "07697e6ca1e21777ac76f26d0779c53f7d08e47b9e32d23bd8fed9cd": {
-          "Cyberia0399": {
-            "Pose": "Lunge pose - Anjaneyasana",
-            "Skin": "Gold",
-            "name": "Cyberia Chakra Planet #0399",
-            "files": [
-              {
-                "src": "ipfs://QmVsMggcQE3da9xuZv7uvJRH84gs5ebGQ8kxVPSQw52XRf",
-                "name": "Please wait while your experience below loads.",
-                "mediaType": "image/jpg"
-              },
-              {
-                "src": "ipfs://QmSHyNm11PrqyrUXszKtsz52ADH6A934c3gw41H7CMCj7D",
-                "mediaType": "text/html"
-              }
-            ],
-            "image": "ipfs://QmVsMggcQE3da9xuZv7uvJRH84gs5ebGQ8kxVPSQw52XRf",
-            "Artist": "Srink",
-            "Avatar": "Male",
-            "Chakra": "Sacral - Svadhisthana",
-            "Mantra": "VAM",
-            "Discord": "https://dsc.gg/cyberiacnft",
-            "Twitter": "https://twitter.com/cyberiaCNFT",
-            "Website": "https://cyberia.gg/",
-            "Function": "Sexual and Creative Energy",
-            "Location": "Below the Belly Button",
-            "Collection": "Chakra Planets",
-            "Planet colour": "Orange"
-          },
-          "Cyberia2795": {
-            "Pose": "Headstand - Sirsasana",
-            "Skin": "Gold",
-            "name": "Cyberia Chakra Planet #2795",
-            "files": [
-              {
-                "src": "ipfs://QmZ4TGY2Jzy5JGaD3S7RLsrP9K8jbp44e7463iHAGitM5a",
-                "name": "Please wait while your experience below loads.",
-                "mediaType": "image/jpg"
-              },
-              {
-                "src": "ipfs://QmcEqKkAcxeGNZimSiQZ2duZA4sx4xJawh35VwuJoS3A9m",
-                "mediaType": "text/html"
-              }
-            ],
-            "image": "ipfs://QmZ4TGY2Jzy5JGaD3S7RLsrP9K8jbp44e7463iHAGitM5a",
-            "Artist": "Srink",
-            "Avatar": "Female",
-            "Chakra": "Crown - Sahasrara",
-            "Mantra": "OM",
-            "Discord": "https://dsc.gg/cyberiacnft",
-            "Twitter": "https://twitter.com/cyberiaCNFT",
-            "Website": "https://cyberia.gg/",
-            "Function": "Spiritual Connection",
-            "Location": "Top of the Head",
-            "Collection": "Chakra Planets",
-            "Planet colour": "Purple"
-          }
-        }
-      }
-    },
-    "token_registry_metadata": null
-  }
-]
-```
-
 #### get_asset_summary
 Get the summary of an asset (total transactions exclude minting/total wallets include only wallets with asset balance)<br>
 Parameters:<br>
 Asset Policy<br>
 Asset Name in hexadecimal format (optional), default: all policy assets<br>
-Returns: List of dictionaries with the mint/burn history of an asset<br>
+Returns: List of maps with the mint/burn history of an asset<br>
 Example:<br>
 `asset_summary = get_asset_summary('07697e6ca1e21777ac76f26d0779c53f7d08e47b9e32d23bd8fed9cd', '4379626572696131313535')`<br>
 Example response:
 ```json
 [
   {
     "policy_id": "07697e6ca1e21777ac76f26d0779c53f7d08e47b9e32d23bd8fed9cd",
@@ -1541,15 +1432,15 @@
 #### get_asset_txs
 Get the list of all asset transaction hashes (the newest first)<br>
 Parameters:<br>
 Asset Policy<br>
 Asset Name in hexadecimal format (optional), default: all policy assets<br>
 Block number (optional) - return only the transactions after this block<br>
 History boolean (optional) - include all historical transactions, setting to false includes only the non-empty ones<br>
-Returns: List of dictionaries with the mint/burn history of an asset<br>
+Returns: List of maps with the mint/burn history of an asset<br>
 Example:<br>
 `asset_txs = get_asset_txs('07697e6ca1e21777ac76f26d0779c53f7d08e47b9e32d23bd8fed9cd', '4379626572696131313535')`<br>
 Example response:
 ```json
 [
   {
     "tx_hash": "d4ac560398b95e6435bd6657e39fe5638f7c5bfaa6ffa6b8fa9bfae0b4882666",
@@ -1561,15 +1452,15 @@
 ```
 
 ### Pool
 
 #### get_pools_list
 A list of all currently registered/retiring (not retired) pools<br>
 Parameters: none<br>
-Returns: The list of stake pool dictionaries<br>
+Returns: The list of stake pool maps<br>
 Example:<br>
 `pool_list = get_pool_list()`<br>
 Example response:
 ```json
 [
   {
     "pool_id_bech32": "pool100wj94uzf54vup2hdzk0afng4dhjaqggt7j434mtgm8v2gfvfgp",
@@ -1656,15 +1547,15 @@
   }
 ]
 ```
 
 #### get_pool_stake_snapshot
 Returns Mark, Set and Go stake snapshots for the selected pool, useful for leaderlog calculation<br>
 Parameters: Stake pool bech32 id<br>
-Returns: Pool snapshot as list of dictionaries by epoch (current and previous 2)<br>
+Returns: Pool snapshot as list of maps by epoch (current and previous 2)<br>
 Example:<br>
 `pool_stake_snapshot = get_pool_stake_snapshot('pool155efqn9xpcf73pphkk88cmlkdwx4ulkg606tne970qswczg3asc')`<br>
 Example response:
 ```json
 [
   {
     "snapshot": "Go",
@@ -1689,15 +1580,15 @@
   }
 ]
 ```
 
 #### get_pool_delegators
 Returns information about live delegators for a given pool<br>
 Parameters Stake pool bech32 id<br>
-Returns: The list of pool delegators dictionaries<br>
+Returns: The list of pool delegators maps<br>
 Example:<br>
 `pool_delegators = get_pool_delegators('pool12wpfng6cu7dz38yduaul3ngfm44xhv5xmech68m5fwe4wu77udd')`<br>
 Example response:
 ```json
 [
   {
     "stake_address": "stake1u80603g5n7vtycl75c60jmv56jx3cw53v23xv0txkpcu8kcwr2k27",
@@ -1722,15 +1613,15 @@
 ```
 
 #### get_pool_delegators_history
 Returns information about active delegators (incl. history) for a given pool and epoch number (all epochs if not specified)<br>
 Parameters:<br>
 Stake pool bech32 id<br>
 Epoch (optional)<br>
-Returns: The list of pool delegators dictionaries<br>
+Returns: The list of pool delegators maps<br>
 Example:<br>
 `pool_delegators_history = get_pool_delegators_history('pool12wpfng6cu7dz38yduaul3ngfm44xhv5xmech68m5fwe4wu77udd', 380)`<br>
 Example response:
 ```json
 [
   {
     "stake_address": "stake1uyezz2wzt4rl5wug8ju8zshvfzkw2lksw8jfp0wpueq2nccnnkwxh",
@@ -1752,15 +1643,15 @@
 ```
 
 #### get_pool_blocks
 Returns information about blocks minted by a given pool for all epochs (or _epoch_no if provided)<br>
 Parameters:<br>
 Stake pool bech32 id<br>
 Epoch (optional)<br>
-Returns: The list of pool blocks dictionaries<br>
+Returns: The list of pool blocks maps<br>
 Example:<br>
 `pool_blocks = get_pool_blocks('pool12wpfng6cu7dz38yduaul3ngfm44xhv5xmech68m5fwe4wu77udd', 380)`<br>
 Example response:
 ```json
 [
   {
     "epoch_no": 380,
@@ -1782,15 +1673,15 @@
 ```
 
 #### get_pool_history
 Returns information about pool stake, block and reward history in a given epoch (or all epochs that pool existed for, in descending order if no epoch number was provided)<br>
 Parameters:<br>
 Stake pool bech32 id<br>
 Epoch (optional)<br>
-Returns:  Information about pool stake, block and reward history as a list dictionaries by epoch (descending)<br>
+Returns:  Information about pool stake, block and reward history as a list maps by epoch (descending)<br>
 Example:<br>
 `pool_history = get_pool_history('pool12wpfng6cu7dz38yduaul3ngfm44xhv5xmech68m5fwe4wu77udd', 379)`<br>
 Example response:
 ```json
 [
   {
     "epoch_no": 379,
@@ -1807,15 +1698,15 @@
   }
 ]
 ```
 
 #### get_pool_updates
 Returns all pool updates for all pools or only updates for specific pool if specified<br>
 Parameters: Stake pool bech32 id (optional)<br>
-Returns: pool updates as a list of dictionaries<br>
+Returns: pool updates as a list of maps<br>
 Example:<br>
 `pool_updates = get_pool_updates('pool12wpfng6cu7dz38yduaul3ngfm44xhv5xmech68m5fwe4wu77udd')`<br>
 Example response:
 ```json
 [
   {
     "tx_hash": "6358622ef9c7a395aaf1590661330a17095fef3c39caa2ae319c737c85bfacb9",
@@ -1896,15 +1787,15 @@
   ...
 ]
 ```
 
 #### get_pool_relays
 A list of registered relays for all currently registered/retiring (not retired) pools<br>
 Parameters: none<br>
-Returns: The list of relays dictionaries by stake pool<br>
+Returns: The list of relays maps by stake pool<br>
 Example:<br>
 `pool_relays = get_pool_relays()`<br>
 Example response:
 ```json
 [
   {
     "pool_id_bech32": "pool100wj94uzf54vup2hdzk0afng4dhjaqggt7j434mtgm8v2gfvfgp",
@@ -1945,15 +1836,15 @@
   ...
 ]
 ```
 
 #### get_pool_metadata
 A list of registered relays for all currently registered/retiring (not retired) pools<br>
 Parameters: Stake pool bech32 ID(s) as string (for one stake pool) or list of stake pool bech32 IDs (for multiple stake pools)<br>
-Returns: The list of pool metadata dictionaries<br>
+Returns: The list of pool metadata maps<br>
 Example:<br>
 `pool_metadata = get_pool_metadata('pool1auvwj75q70s7jce63nvptujs6460kvyxqn0wjegkz4mhja7g5t6')`<br>
 Example response:
 ```json
 [
   {
     "pool_id_bech32": "pool1auvwj75q70s7jce63nvptujs6460kvyxqn0wjegkz4mhja7g5t6",
@@ -1968,15 +1859,15 @@
   }
 ]
 ```
 
 #### get_retiring_pools
 Get the retiring stake pools list<br>
 Parameters: none<br>
-Returns: The list of retiring pools dictionaries<br>
+Returns: The list of retiring pools maps<br>
 Example:<br>
 `retiring_pools = get_retiring_pools()`<br>
 Example response:
 ```json
 [
   {
     "tx_hash": "39a046ef9b5b9e149d24bae8c86f6fb93b08d57312615d22b6a3e73279198e73",
@@ -2040,15 +1931,15 @@
 ```
 
 ### Script
 
 #### get_native_script_list
 List of all existing native script hashes along with their creation transaction hashes<br>
 Parameters: none<br>
-Returns: The list of all native scripts dictionaries<br>
+Returns: The list of all native scripts maps<br>
 Example:<br>
 `native_script_list = get_native_script_list()`<br>
 Example response:
 ```json
 [
   {
     "script_hash": "65c197d565e88a20885e535f93755682444d3c02fd44dd70883fe89e",
@@ -2093,15 +1984,15 @@
   ...
 ]
 ```
 
 #### get_plutus_script_list
 List of all existing native script hashes along with their creation transaction hashes<br>
 Parameters: none<br>
-Returns: The list of all plutus scripts dictionaries<br>
+Returns: The list of all plutus scripts maps<br>
 Example:<br>
 `plutus_script_list = get_plutus_script_list()`<br>
 Example response:
 ```json
 [
   {
     "script_hash": "c916b3d14a51087cc967223aad3f2e4e5c01993f5429719c32c2061e",
@@ -2118,15 +2009,15 @@
   ...
 ]
 ```
 
 #### get_script_redeemers
 List of all redeemers for a given script hash<br>
 Parameters: Script hash<br>
-Returns: Redeemers list as dictionary<br>
+Returns: Redeemers list as map<br>
 Example:<br>
 `script_redeemers = get_script_redeemers('c1996b36d11bf42103745844cc5ee9bf13fde475fa909809e2da7261')`<br>
 Example response:
 ```json
 [
   {
     "script_hash": "c1996b36d11bf42103745844cc5ee9bf13fde475fa909809e2da7261",
@@ -2147,312 +2038,22 @@
   }
 ]
 ```
 
 #### get_datum_info
 List of datum information for given datum hashes<br>
 Parameters: Datum hash(es) as string (for one datum hash) or list (for a list of datum hashes)<br>
-Returns Datum information as list of dictionaries<br>
+Returns Datum information as list of maps<br>
 Example:<br>
 `datum_info = get_datum_info('45b0cfc220ceec5b7c1c62c4d4193d38e4eba48e8815729ce75f9c0ab0e4c1c0')`<br>
 Example response:
 ```json
 [
   {
     "hash": "45b0cfc220ceec5b7c1c62c4d4193d38e4eba48e8815729ce75f9c0ab0e4c1c0",
     "value": {
       "list": []
     },
     "bytes": "80"
   }
 ]
 ```
-
-### Stake Account
-
-#### get_account_list
-Get a list of all accounts<br>
-Parameters:<br>
-The offset (optional) to start from, default 0<br>
-The maximum number of accounts to return (optional), default 0 (no limit)<br>
-Returns: The list of accounts dictionaries<br>
-This takes a very long time to execute (about one hour), because the total number of accounts is in the millions range.<br>
-Example:<br>
-`account_list = get_account_list()`<br>
-Example response:
-```json
-[
-  {
-    "id": "stake1uyfmzu5qqy70a8kq4c8rw09q0w0ktfcxppwujejnsh6tyrg5c774g"
-  },
-  {
-    "id": "stake1uydhlh7f2kkw9eazct5zyzlrvj32gjnkmt2v5qf6t8rut4qwch8ey"
-  },
-  {
-    "id": "stake1uxsgkz6fvgws5wn80vckwvghzapnhfmf0672nmmkm2tt9fcaau5sw"
-  },
-  ...
-]
-```
-
-#### get_account_info
-Get the account information for given stake addresses (accounts)<br>
-Parameters: Stake address(es), as a string (for one address) or a list (for multiple addresses)<br>
-Returns: The list of account information dictionaries<br>
-Example:<br>
-`account_info = get_account_info('stake1uy4jj73pfyejl4d2rs6nc70eykkhhu56p3y2rj2tdayfzeqnjyh0j')`<br>
-Example response:
-```json
-[
-  {
-    "stake_address": "stake1uy4jj73pfyejl4d2rs6nc70eykkhhu56p3y2rj2tdayfzeqnjyh0j",
-    "status": "registered",
-    "delegated_pool": "pool18r2y72aue5nmv489xtnfxl36vzusq95qst6urd87yd5hgzms04c",
-    "total_balance": "20418617",
-    "utxo": "20418617",
-    "rewards": "0",
-    "withdrawals": "0",
-    "rewards_available": "0",
-    "reserves": "0",
-    "treasury": "0"
-  }
-]
-```
-
-#### get_account_utxos
-Get a list of assets registered via token registry on github<br>
-Parameters: Stake address<br>
-Returns: The list of all UTxOs at all payment addresses associated with the stake address<br>
-Example:<br>
-`account_utxos = get_account_utxos('stake1ux5r7myfhycj234wpqyhh3h8skgwvq0hsstpw52f66857uq95cas6')`
-Example response:<br>
-```json
-[
-  {
-	"tx_hash": "215bcaa7b13c491db28d5525d9b2a13a7d8ddabd563da8113a449ab33a6a60be",
-	"tx_index": 2,
-	"address": "addr1q9dwzug2qzdsqvpvrn886nqdtwr02n9kxtwqsxce2gacvedg8akgnwf3y4r2uzqf00rw0pvsucql0pqkzag5n450facqeuerev",
-	"value": "85813474",
-	"block_height": 8214437,
-	"block_time": 1672580966
-  },
-  {
-	"tx_hash": "1eb26dce2f471fbe32aa8cb303f5e8d8078d1da4dbbb78a7bc135036bb3f2f9c",
-	"tx_index": 0,
-	"address": "addr1q88u9gz83nhs9p5pud9kyucx8sg0ygae2p9a4g2p2y55c4ag8akgnwf3y4r2uzqf00rw0pvsucql0pqkzag5n450facqqyd2n7",
-	"value": "110094569",
-	"block_height": 8406870,
-	"block_time": 1676555396
-  },
-  {
-	"tx_hash": "d530de851c2f867f2174c1073b04bdb9f2e2d16029fcfb488e8150ba66976d43",
-	"tx_index": 0,
-	"address": "addr1qxyp2wsafavj47dpc6uqgqx8se3969jn4crfk7y4zwd7vfag8akgnwf3y4r2uzqf00rw0pvsucql0pqkzag5n450facqlyvudm",
-	"value": "1249900",
-	"block_height": 8489290,
-	"block_time": 1678248733
-  },
-  ...
-  {
-	"tx_hash": "d8e3ca8b36f9a785ff33f01aa5460f9248ea94acd621ea187093206b04aa6e30",
-	"tx_index": 0,
-	"address": "addr1q8txa88kt6rpdv3zzn8ghx7u4udf6rpj690rfdvlqn35fldg8akgnwf3y4r2uzqf00rw0pvsucql0pqkzag5n450facqplx97u",
-	"value": "54000000",
-	"block_height": 8759577,
-	"block_time": 1683809438
-  }
-]
-```
-
-#### get_account_info_cached
-Get the cached account information for given stake addresses (accounts)<br>
-Parameters: Stake address(es), as a string (for one address) or a list (for multiple addresses)<br>
-Returns: The list of account information dictionaries<br>
-Example:<br>
-`account_info_cached = get_account_info_cached('stake1uy4jj73pfyejl4d2rs6nc70eykkhhu56p3y2rj2tdayfzeqnjyh0j')`<br>
-Example response:
-```json
-[
-  {
-    "stake_address": "stake1uy4jj73pfyejl4d2rs6nc70eykkhhu56p3y2rj2tdayfzeqnjyh0j",
-    "status": "registered",
-    "delegated_pool": "pool18r2y72aue5nmv489xtnfxl36vzusq95qst6urd87yd5hgzms04c",
-    "total_balance": "20418617",
-    "utxo": "20418617",
-    "rewards": "0",
-    "withdrawals": "0",
-    "rewards_available": "0",
-    "reserves": "0",
-    "treasury": "0"
-  }
-]
-```
-
-#### get_account_rewards
-Get the full rewards history (including MIR) for given stake addresses (accounts)<br>
-Parameters:<br>
-Stake address(es), as a string (for one address) or a list (for multiple addresses)<br>
-Epoch (optional), default: current epoch<br>
-Returns: The list of rewards dictionaries by account (stake address)<br>
-Example:<br>
-`account_rewards = get_account_rewards('stake1u8lhspu67x3jejzcfrh487rtu3hnm26cg0jsn0mgh2y6n9q9ve26z')`<br>
-Example response:
-```json
-[
-  {
-    "stake_address": "stake1u8lhspu67x3jejzcfrh487rtu3hnm26cg0jsn0mgh2y6n9q9ve26z",
-    "rewards": [
-      {
-        "earned_epoch": 233,
-        "spendable_epoch": 235,
-        "amount": "3990414",
-        "type": "member",
-        "pool_id": "pool1jdhjfcu34lq88rypdtslzwyf27uh0h3apcr9mjd68zhc69r29fy"
-      },
-      {
-        "earned_epoch": 234,
-        "spendable_epoch": 236,
-        "amount": "2792902",
-        "type": "member",
-        "pool_id": "pool1jdhjfcu34lq88rypdtslzwyf27uh0h3apcr9mjd68zhc69r29fy"
-      },
-      ...
-      {
-        "earned_epoch": 379,
-        "spendable_epoch": 381,
-        "amount": "6496870",
-        "type": "member",
-        "pool_id": "pool12wpfng6cu7dz38yduaul3ngfm44xhv5xmech68m5fwe4wu77udd"
-      }
-    ]
-  }
-]
-```
-
-#### get_account_updates
-Get the account updates (registration, deregistration, delegation and withdrawals) for given stake addresses (accounts)<br>
-Parameters: Stake address(es), as a string (for one address) or a list (for multiple addresses)<br>
-Returns: The list of account updates dictionaries by account (stake address)<br>
-Example:<br>
-`account_updates = get_account_updates('stake1u8lhspu67x3jejzcfrh487rtu3hnm26cg0jsn0mgh2y6n9q9ve26z')`<br>
-Example response:
-```json
-[
-  {
-    "stake_address": "stake1u8lhspu67x3jejzcfrh487rtu3hnm26cg0jsn0mgh2y6n9q9ve26z",
-    "updates": [
-      {
-        "action_type": "withdrawal",
-        "tx_hash": "487bc75f00fe934dad33683271cca8540fe868eef7025962678f179a1a111ecc",
-        "epoch_no": 324,
-        "epoch_slot": 70687,
-        "absolute_slot": 54675487,
-        "block_time": 1646241778
-      },
-      {
-        "action_type": "withdrawal",
-        "tx_hash": "eb3ffa01f434e210716151fd9001af82529e371a91c20af02512942f988a2119",
-        "epoch_no": 269,
-        "epoch_slot": 339679,
-        "absolute_slot": 31184479,
-        "block_time": 1622750770
-      },
-      ...
-      {
-        "action_type": "withdrawal",
-        "tx_hash": "b056dcbff9b908e1bd3ed015466f64486538058ba3553dbf885b216d88343370",
-        "epoch_no": 252,
-        "epoch_slot": 58375,
-        "absolute_slot": 23559175,
-        "block_time": 1615125466
-      }
-    ]
-  }
-]
-```
-
-#### get_account_addresses
-Get all addresses associated with given staking accounts<br>
-Parameters: Stake address(es), as a string (for one address) or a list (for multiple addresses)<br>
-Returns: The list of addresses dictionaries by account (stake address)<br>
-Example:<br>
-`account_addresses = get_account_addresses('stake1u8lhspu67x3jejzcfrh487rtu3hnm26cg0jsn0mgh2y6n9q9ve26z')`<br>
-Example response:
-```json
-[
-  {
-    "stake_address": "stake1u8lhspu67x3jejzcfrh487rtu3hnm26cg0jsn0mgh2y6n9q9ve26z",
-    "addresses": [
-      "addr1qxwjxvzv8rmyutcjp0647w4n05wv7aez9jdmqcxn8a9sshll0qre4udr9ny9sj8020uxher08k44ssl9pxlk3w5f4x2qjyz9yf"
-    ]
-  }
-]
-```
-
-#### get_account_assets
-Get the native asset balance of given accounts<br>
-Parameters: Stake address(es), as a string (for one address) or a list (for multiple addresses)<br>
-Returns: The list of account assets dictionaries by account (stake address)<br>
-Example:<br>
-`account_assets = get_account_assets('stake1u8lhspu67x3jejzcfrh487rtu3hnm26cg0jsn0mgh2y6n9q9ve26z')`<br>
-Example response:
-```json
-[
-  {
-    "stake_address": "stake1u8lhspu67x3jejzcfrh487rtu3hnm26cg0jsn0mgh2y6n9q9ve26z",
-    "asset_list": [
-      {
-        "policy_id": "0029cb7c88c7567b63d1a512c0ed626aa169688ec980730c0473b913",
-        "asset_name": "6c70202302",
-        "fingerprint": "asset1awuysx8hc686uz0dykmvmc7jfut2ulceucf6yc",
-        "quantity": "418089787"
-      },
-      {
-        "policy_id": "0029cb7c88c7567b63d1a512c0ed626aa169688ec980730c0473b913",
-        "asset_name": "6c7020f302",
-        "fingerprint": "asset1mcq0awl6awlaqg0ywukf94q0mnau263l9rght5",
-        "quantity": "586811406"
-      },
-      ...
-      {
-        "policy_id": "ea2d23f1fa631b414252824c153f2d6ba833506477a929770a4dd9c2",
-        "asset_name": "4d414442554c",
-        "fingerprint": "asset1q0kwjy669gmsqpvxp4lr0sp26pdm0dafme3qp2",
-        "quantity": "500"
-      }
-    ]
-  }
-]
-```
-
-#### get_account_history
-Get the staking history of given stake addresses (accounts)<br>
-Parameters: Stake address(es), as a string (for one address) or a list (for multiple addresses)<br>
-Returns: The list of staking history dictionaries by account (stake address)<br>
-Example:<br>
-`account_history = get_account_history('stake1u8lhspu67x3jejzcfrh487rtu3hnm26cg0jsn0mgh2y6n9q9ve26z')`<br>
-Example response:
-```json
-[
-  {
-    "stake_address": "stake1u8lhspu67x3jejzcfrh487rtu3hnm26cg0jsn0mgh2y6n9q9ve26z",
-    "history": [
-      {
-        "pool_id": "pool1jdhjfcu34lq88rypdtslzwyf27uh0h3apcr9mjd68zhc69r29fy",
-        "epoch_no": 233,
-        "active_stake": "4655706122"
-      },
-      {
-        "pool_id": "pool1jdhjfcu34lq88rypdtslzwyf27uh0h3apcr9mjd68zhc69r29fy",
-        "epoch_no": 234,
-        "active_stake": "5020706122"
-      },
-      ...
-      {
-        "pool_id": "pool12wpfng6cu7dz38yduaul3ngfm44xhv5xmech68m5fwe4wu77udd",
-        "epoch_no": 381,
-        "active_stake": "10247851319"
-      }
-    ]
-  }
-]
-```
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `koios-api-1.0.10/README.md` & `koios-api-1.0.2/src/koios_api.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,7 +1,22 @@
+Metadata-Version: 2.1
+Name: koios-api
+Version: 1.0.2
+Summary: A python package for the Cardano Blockchain Koios API (https://api.koios.rest/)
+Author-email: APEX Stake Pool <cardanoapexpool@gmail.com>
+Project-URL: Homepage, https://github.com/cardano-apexpool/koios-api-python
+Project-URL: Bug Tracker, https://github.com/cardano-apexpool/koios-api-python/issues
+Keywords: koios,cardano,blockchain,REST,API
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Requires-Python: >=3.7
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
 # koios-api-python
 A python package for the Cardano Blockchain Koios API (https://api.koios.rest/)
 
 ## Install
 To install the module, type the following command:
 ```bash
 pip3 install koios_api
@@ -54,15 +69,14 @@
 
 ## Modules
 
 [Network](#Network)<br>
 [get_tip](#get_tip) Get the tip info about the latest block seen by chain<br>
 [get_genesis](#get_genesis) Get the Genesis parameters used to start specific era on chain<br>
 [get_totals](#get_totals) Get the circulating utxo, treasury, rewards, supply and reserves in lovelace for specified epoch, all epochs if empty<br>
-[get_param_updates](#get_param_updates) Get all parameter update proposals submitted to the chain starting Shelley era<br>
 
 [Epoch](#Epoch)<br>
 [get_epoch_info](#get_epoch_info) Get the epoch information, all epochs if no epoch specified<br>
 [get_epoch_params](#get_epoch_params) Get the protocol parameters for specific epoch, returns information about all epochs if no epoch specified<br>
 [get_epoch_block_protocols](#get_epoch_block_protocols) Get the information about block protocol distribution in epoch<br>
 
 [Block](#Block)<br>
@@ -77,29 +91,33 @@
 [get_tx_metalabels](#get_tx_metalabels) Get a list of all transaction metadata labels<br>
 [submit_tx](#submit_tx) Submit an already serialized transaction to the network<br>
 [get_tx_status](#get_tx_status) Get the number of block confirmations for a given transaction hash list<br>
 
 [Address](#Address)<br>
 [get_address_info](#get_address_info) Get the transaction hash list of input address array, optionally filtering after specified block height (inclusive)<br>
 [get_address_txs](#get_address_txs) Get the transaction hash list of input address array, optionally filtering after specified block height (inclusive)<br>
-[get_credential_utxos](#get_credential_utxos) Get a list of UTxO against input payment credential array including their balances<br>
 [get_address_assets](#get_address_assets) Get the list of all the assets (policy, name and quantity) for given addresses<br>
 [get_credential_txs](#get_credential_txs) Get the transaction hash list of input payment credential array, optionally filtering after specified block height (inclusive)<br>
 
+[Account](#Account)<br>
+[get_account_list](#get_account_list) Get a list of all accounts<br>
+[get_account_info](#get_account_info) Get the account information for given stake addresses (accounts)<br>
+[get_account_info_cached](#get_account_info_cached) Get the cached account information for given stake addresses (accounts)<br>
+[get_account_rewards](#get_account_rewards) Get the full rewards history (including MIR) for given stake addresses (accounts)<br>
+[get_account_updates](#get_account_updates) Get the account updates (registration, deregistration, delegation and withdrawals) for given stake addresses (accounts)<br>
+[get_account_addresses](#get_account_addresses) Get all addresses associated with given staking accounts<br>
+[get_account_assets](#get_account_assets) Get the native asset balance of given accounts<br>
+[get_account_history](#get_account_history) Get the staking history of given stake addresses (accounts)<br>
+
 [Asset](#Asset)<br>
 [get_asset_list](#get_asset_list) Get the list of all native assets (paginated)<br>
-[get_asset_token_registry](#get_asset_token_registry) Get a list of assets registered via token registry on github<br>
-[get_asset_addresses](#get_asset_addresses) Get the list of all addresses holding a given asset<br>
-[get_asset_nft_address](#get_asset_nft_address) Get the address where specified NFT currently reside on.<br>
+[get_asset_address_list](#get_asset_address_list) Get the list of all addresses holding a given asset<br>
 [get_asset_info](#get_asset_info) Get the information of an asset including first minting & token registry metadata<br>
-[get_asset_info_bulk](#get_asset_info_bulk) Get the information of a list of assets including first minting & token registry metadata<br>
 [get_asset_history](#get_asset_history) Get the mint/burn history of an asset<br>
-[get_policy_asset_addresses](#get_policy_asset_addresses) Get the list of addresses with quantity for each asset on the given policy<br>
-[get_policy_asset_info](#get_policy_asset_info) Get the information for all assets under the same policy<br>
-[get_policy_asset_list](#get_policy_asset_list) Get the list of asset under the given policy (including balances)<br>
+[get_asset_policy_info](#get_asset_policy_info) Get the information for all assets under the same policy<br>
 [get_asset_summary](#get_asset_summary) Get the summary of an asset (total transactions exclude minting/total wallets include only wallets with asset balance)<br>
 [get_asset_txs](#get_asset_txs) Get the list of all asset transaction hashes (the newest first)<br>
 
 [Pool](#Pool)<br>
 [get_pools_list](#get_pools_list) A list of all currently registered/retiring (not retired) pools<br>
 [get_pool_info](#get_pool_info) Current pool statuses and details for a specified list of pool ids<br>
 [get_pool_stake_snapshot](#get_pool_stake_snapshot) Returns Mark, Set and Go stake snapshots for the selected pool, useful for leaderlog calculation<br>
@@ -114,31 +132,20 @@
 
 [Script](#Script)<br>
 [get_native_script_list](#get_native_script_list) The list of all existing native script hashes along with their creation transaction hashes<br>
 [get_plutus_script_list](#get_plutus_script_list) The list of all existing native script hashes along with their creation transaction hashes<br>
 [get_script_redeemers](#get_script_redeemers) The list of all redeemers for a given script hash<br>
 [get_datum_info](#get_datum_info) The list of datum information for given datum hashes<br>
 
-[Stake Account](#Stake Account)<br>
-[get_account_list](#get_account_list) Get a list of all accounts<br>
-[get_account_info](#get_account_info) Get the account information for given stake addresses (accounts)<br>
-[get_account_utxos](#get_account_utxos) Get a list of all UTxOs for a given stake address (account)<br>
-[get_account_info_cached](#get_account_info_cached) Get the cached account information for given stake addresses (accounts)<br>
-[get_account_rewards](#get_account_rewards) Get the full rewards history (including MIR) for given stake addresses (accounts)<br>
-[get_account_updates](#get_account_updates) Get the account updates (registration, deregistration, delegation and withdrawals) for given stake addresses (accounts)<br>
-[get_account_addresses](#get_account_addresses) Get all addresses associated with given staking accounts<br>
-[get_account_assets](#get_account_assets) Get the native asset balance of given accounts<br>
-[get_account_history](#get_account_history) Get the staking history of given stake addresses (accounts)<br>
-
 ### Network
 
 #### get_tip
 Get the tip info about the latest block seen by chain<br>
 Parameters: none<br>
-Returns: The tip information as a list of one dictionary<br>
+Returns: The tip information as a list of one map<br>
 Example:<br>
 `tip = get_tip()`<br>
 Example response:
 ```json
 [
   {
     "hash": "442765ab5660346a6af3ba7667bbd35934e6219a52f0f53a80f28d27a70309c1",
@@ -150,15 +157,15 @@
   }
 ]
 ```
 
 #### get_genesis
 Get the Genesis parameters used to start specific era on chain<br>
 Parameters: none<br>
-Returns: Genesis parameters used to start each era on chain as a list of one dictionary<br>
+Returns: Genesis parameters used to start each era on chain as a list of one map<br>
 Example:<br>
 `genesis = get_genesis()`<br>
 Example response:
 ```json
 [
   {
     "networkmagic": "764824073",
@@ -176,15 +183,15 @@
   }
 ]
 ```
 
 #### get_totals
 Get the circulating utxo, treasury, rewards, supply and reserves in lovelace for specified epoch, all epochs if empty<br>
 Parameters: Epoch (optional)<br>
-Returns: Supply/reserves/utxo/fees/treasury stats as a list of one dictionary (if the epoch is specified) or a list of all available epochs (if the epoch parameter is not specified)<br>
+Returns: Supply/reserves/utxo/fees/treasury stats as a list of one map (if the epoch is specified) or a list of all available epochs (if the epoch parameter is not specified)<br>
 Example:<br>
 `totals = get_totals(380)`<br>
 Example response:
 ```json
 [
   {
     "epoch_no": 380,
@@ -193,50 +200,20 @@
     "reward": "635180192555825",
     "supply": "35230640457275590",
     "reserves": "9769359542724410"
   }
 ]
 ```
 
-#### get_param_updates
-Get all parameter update proposals submitted to the chain starting Shelley era<br>
-Parameters: none<br>
-Returns: All parameter update proposals<br>
-Example:<br>
-`param_updates = get_param_updates()`<br>
-```json
-[
-  {
-    "tx_hash": "b516588da34b58b7d32b6a057f513e16ea8c87de46615631be3316d8a8847d46",
-    "block_height": 4533644,
-    "block_time": 1596923351,
-    "epoch_no": 210,
-    "data": {
-      "decentralisation": 0.9
-    }
-  },
-  {
-    "tx_hash": "784902982af484f78d10f1587072f5a6b888ed0c1296d4ecf1e21c0251696ca1",
-    "block_height": 4558648,
-    "block_time": 1597425824,
-    "epoch_no": 211,
-    "data": {
-      "decentralisation": 0.8
-    }
-  },
-  ...
-]
-```
-
 ### Epoch
 
 #### get_epoch_info
 Get the epoch information, all epochs if no epoch specified<br>
 Parameters: Epoch (optional)<br>
-Returns: The list of epoch info dictionaries<br>
+Returns: The list of epoch info maps<br>
 Example:<br>
 `epoch_info = get_epoch_info(379)`<br>
 Example response:
 ```json
 [
   {
     "epoch_no": 379,
@@ -254,15 +231,15 @@
   }
 ]
 ```
 
 #### get_epoch_params
 Get the protocol parameters for specific epoch, returns information about all epochs if no epoch specified<br>
 Parameters: Epoch (optional)<br>
-Returns: The list of epoch protocol parameters dictionaries<br>
+Returns: The list of epoch protocol parameters maps<br>
 Example:<br>
 `epoch_params = get_epoch_params(380)`<br>
 Example response:
 ```json
 [
   {
     "epoch_no": 380,
@@ -300,15 +277,15 @@
   }
 ]
 ```
 
 #### get_epoch_block_protocols
 Get the information about block protocol distribution in epoch<br>
 Parameters: Epoch (optional)<br>
-Returns: The list of epoch protocol distribution dictionaries<br>
+Returns: The list of epoch protocol distribution maps<br>
 Example:<br>
 `epoch_block_protocols = get_epoch_block_protocols(380)`<br>
 Example response:
 ```json
 [
   {
     "proto_major": 7,
@@ -324,15 +301,15 @@
 ```
 
 ### Block
 
 #### get_blocks
 Get summarised details about all blocks (paginated - latest first)<br>
 Parameters: The maximum number of blocks to return<br>
-Returns: The list of block dictionaries (the newest first)<br>
+Returns: The list of block maps (the newest first)<br>
 Example:<br>
 `blocks = get_blocks(3)`<br>
 Example response:
 ```json
 [
   {
     "hash": "8e33bb588feff6414469779d724923064688615535280f8982c9981410cd06f6",
@@ -381,15 +358,15 @@
   }
 ]
 ```
 
 #### get_block_info
 Get detailed information about a specific block<br>
 Parameters: Block hash as string (for one block) or list of block hashes (for multiple blocks)<br>
-Returns: The list of block dictionaries<br>
+Returns: The list of block maps<br>
 Example:<br>
 `block_info = get_block_info('8e33bb588feff6414469779d724923064688615535280f8982c9981410cd06f6')`<br>
 Example response:
 ```json
 [
   {
     "hash": "8e33bb588feff6414469779d724923064688615535280f8982c9981410cd06f6",
@@ -414,15 +391,15 @@
   }
 ]
 ```
 
 #### get_block_txs
 Get a list of all transactions included in provided blocks<br>
 Parameters: Block(s) hash(es) as string (for one block) or list of block hashes (for multiple blocks)<br>
-Returns: The list of transaction dictionaries by block<br>
+Returns: The list of transaction maps by block<br>
 Example:<br>
 `block_txs = get_block_txs('8e33bb588feff6414469779d724923064688615535280f8982c9981410cd06f6')`<br>
 Example response:
 ```json
 [
   {
     "block_hash": "8e33bb588feff6414469779d724923064688615535280f8982c9981410cd06f6",
@@ -452,15 +429,15 @@
 ```
 
 ### Transactions
 
 #### get_tx_info
 Get detailed information about transaction(s)<br>
 Parameters: Transaction(s) hash(es) as a string (for one transaction) or list (for multiple transactions)<br>
-Returns: The list of transactions details dictionaries<br>
+Returns: The list of transactions details maps<br>
 Example:<br>
 `tx_info = get_tx_info('99f2aefba2a4a5a550aeed9d91d3adabe77a286ec45c345c7980a208364f76c6')`<br>
 Example response:
 ```json
 [
   {
     "tx_hash": "99f2aefba2a4a5a550aeed9d91d3adabe77a286ec45c345c7980a208364f76c6",
@@ -554,15 +531,15 @@
   }
 ]
 ```
 
 #### get_tx_utxos
 Get UTxO set (inputs/outputs) of transactions<br>
 Parameters: Transaction(s) hash(es) as a string (for one transaction) or list (for multiple transactions)<br>
-Returns: The list of transactions UTxOs dictionaries<br>
+Returns: The list of transactions UTxOs maps<br>
 Example:<br>
 `tx_utxos = get_tx_utxos('bf685dde61d36b8acd259b2bd00a69a2e8359d2a69b75aa3a0eff9d38ca1f2ef')`<br>
 Example response:
 ```json
 [
   {
     "tx_hash": "bf685dde61d36b8acd259b2bd00a69a2e8359d2a69b75aa3a0eff9d38ca1f2ef",
@@ -631,15 +608,15 @@
   }
 ]
 ```
 
 #### get_tx_metadata
 Get metadata information (if any) for given transaction(s)<br>
 Parameters: Transaction(s) hash(es) as a string (for one transaction) or list (for multiple transactions)<br>
-Returns: The list of transactions metadata dictionaries<br>
+Returns: The list of transactions metadata maps<br>
 Example:<br>
 `tx_metadata = get_tx_metadata('291b5533227331999eca2e63934c1061e5f85993e77747a90d9901413d7bb937')`<br>
 Example response:
 ```json
 [
   {
     "tx_hash": "291b5533227331999eca2e63934c1061e5f85993e77747a90d9901413d7bb937",
@@ -659,15 +636,15 @@
   }
 ]
 ```
 
 #### get_tx_metalabels
 Get a list of all transaction metadata labels<br>
 Parameters: none<br>
-Returns: The list of transaction metadata labels dictionaries<br>
+Returns: The list of transaction metadata labels maps<br>
 Example:<br>
 `tx_metalabels = get_tx_metalabels()`<br>
 Example response:
 ```json
 [
   {
     "key": "0"
@@ -707,15 +684,15 @@
 ```
 0eec38dc1d2d021f477a890d754e66c49fe74a9fd972793076587496c9850060
 ```
 
 #### get_tx_status
 Get the number of block confirmations for a given transaction hash list<br>
 Parameters: Transaction(s) hash(es) as a string (for one transaction) or list (for multiple transactions)<br>
-Returns: The list of transactions block confirmations dictionaries<br>
+Returns: The list of transactions block confirmations maps<br>
 Example:<br>
 `tx_status = get_tx_status('0eec38dc1d2d021f477a890d754e66c49fe74a9fd972793076587496c9850060')`<br>
 Example response:
 ```json
 [
   {
     "tx_hash": "0eec38dc1d2d021f477a890d754e66c49fe74a9fd972793076587496c9850060",
@@ -725,15 +702,15 @@
 ```
 
 ### Address
 
 #### get_address_info
 Get the transaction hash list of input address array, optionally filtering after specified block height (inclusive)<br>
 Parameters: Payment address(es) as string (for one address) or list (for multiple addresses)<br>
-Returns: The list of transactions dictionaries<br>
+Returns: The list of transactions maps<br>
 Example:<br>
 `address_info = get_address_info('addr1q8wv876ptu0qhujmh2awdcnpcc0ctgdz8e8qvv29k8hucwft99azzjfn9l2658p483uljfdd00ef5rzg58y5km6gj9jqcp0ws7')`<br>
 Example response:
 ```json
 [
   {
     "address": "addr1q8wv876ptu0qhujmh2awdcnpcc0ctgdz8e8qvv29k8hucwft99azzjfn9l2658p483uljfdd00ef5rzg58y5km6gj9jqcp0ws7",
@@ -756,15 +733,15 @@
   }
 ]
 ```
 
 #### get_address_txs
 Get the transaction hash list of input address array, optionally filtering after specified block height (inclusive)<br>
 Parameters: Payment address(es) as string (for one address) or list (for multiple addresses)<br>
-Returns: The list of transactions dictionaries<br>
+Returns: The list of transactions maps<br>
 Example:<br>
 `address_txs = get_address_txs('addr1q8wv876ptu0qhujmh2awdcnpcc0ctgdz8e8qvv29k8hucwft99azzjfn9l2658p483uljfdd00ef5rzg58y5km6gj9jqcp0ws7')`<br>
 Example response:
 ```json
 [
   {
     "tx_hash": "c626fe027d09db2b6c63ba67e3638911ff70e3b691a7e5c03e75c0d3a168c973",
@@ -790,61 +767,18 @@
     "epoch_no": 373,
     "block_height": 7971352,
     "block_time": 1667570778
   }
 ]
 ```
 
-#### get_credential_utxos
-Get a list of UTxO against input payment credential array including their balances<br>
-Parameters: Payment credential(s) as string (for one credential) or list (for multiple credentials)<br>
-Returns: The list of UTxO against input payment credential array including their balances<br>
-Example:<br>
-`credential_utxos = get_credential_utxos('0c35748e147183cd784875e78a5b372fa6975e9ac6406d6015c09bac')`<br>
-Example response:<br>
-```json
-[
-  {
-    "tx_hash": "8e9b85284f92ad85416d4fb0a3ff5d3bbd9b57c4a4d97a8d39dc99316eace0cf",
-    "tx_index": 0,
-    "value": "5000000"
-  },
-  {
-    "tx_hash": "e7333c01d3c2887767aca13e5c74fb858fbf0119cd90d944869ee72b8b81f523",
-    "tx_index": 1,
-    "value": "20432286"
-  },
-  {
-    "tx_hash": "ecfbbc335ec203b10ee65faddf06fb0ceac27c36ef3a76047fbf820f6e9ed7f2",
-    "tx_index": 2,
-    "value": "2301540"
-  },
-  {
-    "tx_hash": "b70a9107a38e776c0b1d94a1578c393a1ce01ea8e28ed56c5c724a2639e31bfe",
-    "tx_index": 2,
-    "value": "1150770"
-  },
-  {
-    "tx_hash": "1107afdada22f259aa798de57ca3839e212e977467628c85315326917a13dd3b",
-    "tx_index": 2,
-    "value": "1150770"
-  },
-  ...
-  {
-    "tx_hash": "b9d519ff9309dd78a7e8031aef2fa6b21358478efed5f0bdf234fa10c83eede7",
-    "tx_index": 1,
-    "value": "137666866"
-  }
-]
-```
-
 #### get_address_assets
 Get the list of all the assets (policy, name and quantity) for given addresses<br>
 Parameters: Payment address(es) as string (for one address) or list (for multiple addresses)<br>
-Returns: The list of assets dictionaries by address<br>
+Returns: The list of assets maps by address<br>
 Example:<br>
 `address_assets = get_address_assets('addr1qywp2795uk4uusknpseu3fcwy8ew57dnuaeutnxaa5j6ulp4u2anham4xet066yjc6xjxcymujvvwlfhj8k8gxfl2nvs73rvzh')`<br>
 Example response:
 ```json
 [
   {
     "address": "addr1qywp2795uk4uusknpseu3fcwy8ew57dnuaeutnxaa5j6ulp4u2anham4xet066yjc6xjxcymujvvwlfhj8k8gxfl2nvs73rvzh",
@@ -872,15 +806,15 @@
   }
 ]
 ```
 
 #### get_credential_txs
 Get the transaction hash list of input payment credential array, optionally filtering after specified block height (inclusive)<br>
 Parameters: Credential(s) as string (for one credential) or list (for multiple credentials)<br>
-Returns: The list of address information dictionaries<br>
+Returns: The list of address information maps<br>
 Example:<br>
 `credential_txs = get_credential_txs('dcc3fb415f1e0bf25bbabae6e261c61f85a1a23e4e063145b1efcc39')`<br>
 Example response:
 ```json
 [
   {
     "tx_hash": "c626fe027d09db2b6c63ba67e3638911ff70e3b691a7e5c03e75c0d3a168c973",
@@ -900,23 +834,268 @@
     "epoch_no": 373,
     "block_height": 7971352,
     "block_time": 1667570778
   }
 ]
 ```
 
+### Account
+
+#### get_account_list
+Get a list of all accounts<br>
+Parameters:<br>
+The offset (optional) to start from, default 0<br>
+The maximum number of accounts to return (optional), default 0 (no limit)<br>
+Returns: The list of accounts maps<br>
+This takes a very long time to execute (about one hour), because the total number of accounts is in the millions range.<br>
+Example:<br>
+`account_list = get_account_list()`<br>
+Example response:
+```json
+[
+  {
+    "id": "stake1uyfmzu5qqy70a8kq4c8rw09q0w0ktfcxppwujejnsh6tyrg5c774g"
+  },
+  {
+    "id": "stake1uydhlh7f2kkw9eazct5zyzlrvj32gjnkmt2v5qf6t8rut4qwch8ey"
+  },
+  {
+    "id": "stake1uxsgkz6fvgws5wn80vckwvghzapnhfmf0672nmmkm2tt9fcaau5sw"
+  },
+  ...
+]
+```
+
+#### get_account_info
+Get the account information for given stake addresses (accounts)<br>
+Parameters: Stake address(es), as a string (for one address) or a list (for multiple addresses)<br>
+Returns: The list of account information maps<br>
+Example:<br>
+`account_info = get_account_info('stake1uy4jj73pfyejl4d2rs6nc70eykkhhu56p3y2rj2tdayfzeqnjyh0j')`<br>
+Example response:
+```json
+[
+  {
+    "stake_address": "stake1uy4jj73pfyejl4d2rs6nc70eykkhhu56p3y2rj2tdayfzeqnjyh0j",
+    "status": "registered",
+    "delegated_pool": "pool18r2y72aue5nmv489xtnfxl36vzusq95qst6urd87yd5hgzms04c",
+    "total_balance": "20418617",
+    "utxo": "20418617",
+    "rewards": "0",
+    "withdrawals": "0",
+    "rewards_available": "0",
+    "reserves": "0",
+    "treasury": "0"
+  }
+]
+```
+
+#### get_account_info_cached
+Get the cached account information for given stake addresses (accounts)<br>
+Parameters: Stake address(es), as a string (for one address) or a list (for multiple addresses)<br>
+Returns: The list of account information maps<br>
+Example:<br>
+`account_info_cached = get_account_info_cached('stake1uy4jj73pfyejl4d2rs6nc70eykkhhu56p3y2rj2tdayfzeqnjyh0j')`<br>
+Example response:
+```json
+[
+  {
+    "stake_address": "stake1uy4jj73pfyejl4d2rs6nc70eykkhhu56p3y2rj2tdayfzeqnjyh0j",
+    "status": "registered",
+    "delegated_pool": "pool18r2y72aue5nmv489xtnfxl36vzusq95qst6urd87yd5hgzms04c",
+    "total_balance": "20418617",
+    "utxo": "20418617",
+    "rewards": "0",
+    "withdrawals": "0",
+    "rewards_available": "0",
+    "reserves": "0",
+    "treasury": "0"
+  }
+]
+```
+
+#### get_account_rewards
+Get the full rewards history (including MIR) for given stake addresses (accounts)<br>
+Parameters:<br>
+Stake address(es), as a string (for one address) or a list (for multiple addresses)<br>
+Epoch (optional), default: current epoch<br>
+Returns: The list of rewards maps by account (stake address)<br>
+Example:<br>
+`account_rewards = get_account_rewards('stake1u8lhspu67x3jejzcfrh487rtu3hnm26cg0jsn0mgh2y6n9q9ve26z')`<br>
+Example response:
+```json
+[
+  {
+    "stake_address": "stake1u8lhspu67x3jejzcfrh487rtu3hnm26cg0jsn0mgh2y6n9q9ve26z",
+    "rewards": [
+      {
+        "earned_epoch": 233,
+        "spendable_epoch": 235,
+        "amount": "3990414",
+        "type": "member",
+        "pool_id": "pool1jdhjfcu34lq88rypdtslzwyf27uh0h3apcr9mjd68zhc69r29fy"
+      },
+      {
+        "earned_epoch": 234,
+        "spendable_epoch": 236,
+        "amount": "2792902",
+        "type": "member",
+        "pool_id": "pool1jdhjfcu34lq88rypdtslzwyf27uh0h3apcr9mjd68zhc69r29fy"
+      },
+      ...
+      {
+        "earned_epoch": 379,
+        "spendable_epoch": 381,
+        "amount": "6496870",
+        "type": "member",
+        "pool_id": "pool12wpfng6cu7dz38yduaul3ngfm44xhv5xmech68m5fwe4wu77udd"
+      }
+    ]
+  }
+]
+```
+
+#### get_account_updates
+Get the account updates (registration, deregistration, delegation and withdrawals) for given stake addresses (accounts)<br>
+Parameters: Stake address(es), as a string (for one address) or a list (for multiple addresses)<br>
+Returns: The list of account updates maps by account (stake address)<br>
+Example:<br>
+`account_updates = get_account_updates('stake1u8lhspu67x3jejzcfrh487rtu3hnm26cg0jsn0mgh2y6n9q9ve26z')`<br>
+Example response:
+```json
+[
+  {
+    "stake_address": "stake1u8lhspu67x3jejzcfrh487rtu3hnm26cg0jsn0mgh2y6n9q9ve26z",
+    "updates": [
+      {
+        "action_type": "withdrawal",
+        "tx_hash": "487bc75f00fe934dad33683271cca8540fe868eef7025962678f179a1a111ecc",
+        "epoch_no": 324,
+        "epoch_slot": 70687,
+        "absolute_slot": 54675487,
+        "block_time": 1646241778
+      },
+      {
+        "action_type": "withdrawal",
+        "tx_hash": "eb3ffa01f434e210716151fd9001af82529e371a91c20af02512942f988a2119",
+        "epoch_no": 269,
+        "epoch_slot": 339679,
+        "absolute_slot": 31184479,
+        "block_time": 1622750770
+      },
+      ...
+      {
+        "action_type": "withdrawal",
+        "tx_hash": "b056dcbff9b908e1bd3ed015466f64486538058ba3553dbf885b216d88343370",
+        "epoch_no": 252,
+        "epoch_slot": 58375,
+        "absolute_slot": 23559175,
+        "block_time": 1615125466
+      }
+    ]
+  }
+]
+```
+
+#### get_account_addresses
+Get all addresses associated with given staking accounts<br>
+Parameters: Stake address(es), as a string (for one address) or a list (for multiple addresses)<br>
+Returns: The list of addresses maps by account (stake address)<br>
+Example:<br>
+`account_addresses = get_account_addresses('stake1u8lhspu67x3jejzcfrh487rtu3hnm26cg0jsn0mgh2y6n9q9ve26z')`<br>
+Example response:
+```json
+[
+  {
+    "stake_address": "stake1u8lhspu67x3jejzcfrh487rtu3hnm26cg0jsn0mgh2y6n9q9ve26z",
+    "addresses": [
+      "addr1qxwjxvzv8rmyutcjp0647w4n05wv7aez9jdmqcxn8a9sshll0qre4udr9ny9sj8020uxher08k44ssl9pxlk3w5f4x2qjyz9yf"
+    ]
+  }
+]
+```
+
+#### get_account_assets
+Get the native asset balance of given accounts<br>
+Parameters: Stake address(es), as a string (for one address) or a list (for multiple addresses)<br>
+Returns: The list of account assets maps by account (stake address)<br>
+Example:<br>
+`account_assets = get_account_assets('stake1u8lhspu67x3jejzcfrh487rtu3hnm26cg0jsn0mgh2y6n9q9ve26z')`<br>
+Example response:
+```json
+[
+  {
+    "stake_address": "stake1u8lhspu67x3jejzcfrh487rtu3hnm26cg0jsn0mgh2y6n9q9ve26z",
+    "asset_list": [
+      {
+        "policy_id": "0029cb7c88c7567b63d1a512c0ed626aa169688ec980730c0473b913",
+        "asset_name": "6c70202302",
+        "fingerprint": "asset1awuysx8hc686uz0dykmvmc7jfut2ulceucf6yc",
+        "quantity": "418089787"
+      },
+      {
+        "policy_id": "0029cb7c88c7567b63d1a512c0ed626aa169688ec980730c0473b913",
+        "asset_name": "6c7020f302",
+        "fingerprint": "asset1mcq0awl6awlaqg0ywukf94q0mnau263l9rght5",
+        "quantity": "586811406"
+      },
+      ...
+      {
+        "policy_id": "ea2d23f1fa631b414252824c153f2d6ba833506477a929770a4dd9c2",
+        "asset_name": "4d414442554c",
+        "fingerprint": "asset1q0kwjy669gmsqpvxp4lr0sp26pdm0dafme3qp2",
+        "quantity": "500"
+      }
+    ]
+  }
+]
+```
+
+#### get_account_history
+Get the staking history of given stake addresses (accounts)<br>
+Parameters: Stake address(es), as a string (for one address) or a list (for multiple addresses)<br>
+Returns: The list of staking history maps by account (stake address)<br>
+Example:<br>
+`account_history = get_account_history('stake1u8lhspu67x3jejzcfrh487rtu3hnm26cg0jsn0mgh2y6n9q9ve26z')`<br>
+Example response:
+```json
+[
+  {
+    "stake_address": "stake1u8lhspu67x3jejzcfrh487rtu3hnm26cg0jsn0mgh2y6n9q9ve26z",
+    "history": [
+      {
+        "pool_id": "pool1jdhjfcu34lq88rypdtslzwyf27uh0h3apcr9mjd68zhc69r29fy",
+        "epoch_no": 233,
+        "active_stake": "4655706122"
+      },
+      {
+        "pool_id": "pool1jdhjfcu34lq88rypdtslzwyf27uh0h3apcr9mjd68zhc69r29fy",
+        "epoch_no": 234,
+        "active_stake": "5020706122"
+      },
+      ...
+      {
+        "pool_id": "pool12wpfng6cu7dz38yduaul3ngfm44xhv5xmech68m5fwe4wu77udd",
+        "epoch_no": 381,
+        "active_stake": "10247851319"
+      }
+    ]
+  }
+]
+```
+
 ### Asset
 
 #### get_asset_list
 Get the list of all native assets (paginated)<br>
 Parameters:<br>
 Asset Policy (optional), default: all policies<br>
 The offset (optional) to start from, default 0<br>
 The maximum number of accounts to return (optional), default 0 (no limit)<br>
-Returns: The list of assets dictionaries by policy<br>
+Returns: The list of assets maps by policy<br>
 Example:<br>
 `asset_list = get_asset_list()`<br>
 Example response:
 ```json
 [
   {
     "policy_id": "00000002df633853f6a47465c9496721d2d5b1291b8398016c0e87ae",
@@ -934,98 +1113,38 @@
     "asset_name": "43726565707942616c6c7a57316231303137",
     "fingerprint": "asset12dvnasghksl5k7w696nd5t692j6myexapwjh0d"
   },
   ...
 ]
 ```
 
-#### get_asset_token_registry
-Get a list of assets registered via token registry on github<br>
-Parameters: none<br>
-Returns: The list of assets registered via token registry on github<br>
-Example:<br>
-`asset_token_registry = get_asset_token_registry()`<br>
-Example response:<br>
-```json
-[
-  {
-    "policy_id": "00000002df633853f6a47465c9496721d2d5b1291b8398016c0e87ae",
-    "asset_name": "6e7574636f696e",
-    "asset_name_ascii": "nutcoin",
-    "ticker": "NUT",
-    "description": "The legendary Nutcoin, the first native asset minted on Cardano.",
-    "url": "https://fivebinaries.com/nutcoin",
-    "decimals": 0,
-    "logo": "iVBORw0KGgoAAAANSUhEUgAAAGQA....2rCPgau2EAAAAASUVORK5CYII="
-  },
-  {
-    "policy_id": "00109530994ea381c0bfe0936c85ea01bfe2765c24ef6dad5740c33e",
-    "asset_name": "486f646c657220436f616c6974696f6e20436f696e",
-    "asset_name_ascii": "Hodler Coalition Coin",
-    "ticker": "HODLR",
-    "description": "Stake ₳DA with the Hodler Coalition. Save the World.",
-    "url": "https://www.hodlerstaking.com/",
-    "decimals": 4,
-    "logo": "iVBORw0KGgoAAAANSUhEUgAAARAAA...4RtRz5t2G8zAAAAAElFTkSuQmCC"
-  },
-  {
-    "policy_id": "0011fbab202151eca9e9ef7680569d9419d12e51e693cb05a2edd2ed",
-    "asset_name": "4341524b",
-    "asset_name_ascii": "Cardano Ark Token",
-    "ticker": "CARK",
-    "description": "Utility token for the Cardano Ark",
-    "url": "https://www.cardanoark.com/",
-    "decimals": 0,
-    "logo": ""
-  },
-  ...
-]
-```
-
-#### get_asset_addresses
+#### get_asset_address_list
 Get the list of all addresses holding a given asset<br>
 Parameters:<br>
 Asset Policy<br>
 Asset Name in hexadecimal format (optional), default: all policy assets<br>
-Returns: List of dictionaries with the wallets holding the asset and the amount of assets per wallet<br>
+Returns: List of maps with the wallets holding the asset and the amount of assets per wallet<br>
 Example:<br>
 `asset_address_list = get_asset_address_list('07697e6ca1e21777ac76f26d0779c53f7d08e47b9e32d23bd8fed9cd', '4379626572696130363936')`<br>
 Example response:
 ```json
 [
   {
     "payment_address": "addr1qywp2795uk4uusknpseu3fcwy8ew57dnuaeutnxaa5j6ulp4u2anham4xet066yjc6xjxcymujvvwlfhj8k8gxfl2nvs73rvzh",
     "quantity": "1"
   }
 ]
 ```
 
-#### get_asset_nft_address
-Get the address where specified NFT currently reside on.<br>
-Parameters:<br>
-Asset Policy<br>
-Asset Name in hexadecimal format<br>
-Returns: The wallet address holding the NFT as a list of one dictionary<br>
-Example:<br>
-`asset_nft_address = get_asset_nft_address('07697e6ca1e21777ac76f26d0779c53f7d08e47b9e32d23bd8fed9cd', '4379626572696130363936')`<br>
-Example response:
-```json
-[
-  {
-    "payment_address": "addr1qywp2795uk4uusknpseu3fcwy8ew57dnuaeutnxaa5j6ulp4u2anham4xet066yjc6xjxcymujvvwlfhj8k8gxfl2nvs73rvzh"
-  }
-]
-```
-
 #### get_asset_info
 Get the information of an asset including first minting & token registry metadata<br>
 Parameters:
 Asset Policy<br>
 Asset Name in hexadecimal format (optional), default: all policy assets<br>
-Returns: List of dictionaries with the wallets holding the asset and the amount of assets per wallet<br>
+Returns: List of maps with the wallets holding the asset and the amount of assets per wallet<br>
 Example:<br>
 `asset_info = get_asset_info('07697e6ca1e21777ac76f26d0779c53f7d08e47b9e32d23bd8fed9cd', '4379626572696130363936')`<br>
 Example response:
 ```json
 [
   {
     "policy_id": "07697e6ca1e21777ac76f26d0779c53f7d08e47b9e32d23bd8fed9cd",
@@ -1073,97 +1192,20 @@
       }
     },
     "token_registry_metadata": null
   }
 ]
 ```
 
-#### get_asset_info_bulk
-Get the information of a list of assets including first minting & token registry metadata<br>
-Parameters:<br>
-Assets List in tge following format: `['policy.name_hex']`<br>
-Returns: List of assets including first minting & token registry metadata<br>
-Example:<br>
-`asset_info_bulk = get_asset_info_bulk(['221b1b9ebccab1512262347491557279ac0afac63b4fbd10fc596c8a.437562656e7369734d757368726f6f6d', '221b1b9ebccab1512262347491557279ac0afac63b4fbd10fc596c8a.417a7a69654d757368726f6f6d'])`<br>
-Example response:
-```json
-[
-  {
-    "policy_id": "221b1b9ebccab1512262347491557279ac0afac63b4fbd10fc596c8a",
-    "asset_name": "437562656e7369734d757368726f6f6d",
-    "asset_name_ascii": "CubensisMushroom",
-    "fingerprint": "asset1csgmd2qwycgmqdck4dgqzzwm7xclhkqrhxs2pw",
-    "minting_tx_hash": "c29fd9f0c71793eb06e7cf055e8529740b0486a802b8e9019df4853c6dec03a0",
-    "total_supply": "7576",
-    "mint_cnt": 1,
-    "burn_cnt": 0,
-    "creation_time": 1680393600,
-    "minting_tx_metadata": {
-      "721": {
-        "version": "1.0",
-        "221b1b9ebccab1512262347491557279ac0afac63b4fbd10fc596c8a": {
-          "CubensisMushroom": {
-            "name": "CubensisMushroom",
-            "files": [
-              {
-                "src": "ipfs://QmQNTa19H5WnYtRiHqzNK2drC9rRTzmkxtu7tS57WZkNuZ",
-                "name": "Cubensis",
-                "mediaType": "image/png"
-              }
-            ],
-            "image": "ipfs://QmQNTa19H5WnYtRiHqzNK2drC9rRTzmkxtu7tS57WZkNuZ",
-            "project": "Chilled Kongs",
-            "mediaType": "image/png"
-          }
-        }
-      }
-    },
-    "token_registry_metadata": null
-  },
-  {
-    "policy_id": "221b1b9ebccab1512262347491557279ac0afac63b4fbd10fc596c8a",
-    "asset_name": "417a7a69654d757368726f6f6d",
-    "asset_name_ascii": "AzzieMushroom",
-    "fingerprint": "asset1kfskmlcvlsvpvr093staxj2788qlrkcrssf26a",
-    "minting_tx_hash": "e4b94e3a5e95953acfb50e3c2fd005b2839ca79c4294b62bbf7d2afdf96dd009",
-    "total_supply": "1305",
-    "mint_cnt": 1,
-    "burn_cnt": 0,
-    "creation_time": 1680393600,
-    "minting_tx_metadata": {
-      "721": {
-        "version": "1.0",
-        "221b1b9ebccab1512262347491557279ac0afac63b4fbd10fc596c8a": {
-          "AzzieMushroom": {
-            "name": "AzzieMushroom",
-            "files": [
-              {
-                "src": "ipfs://QmeAdLCKgXhxtDAcpPq5vgpRCqYWCGFMzb9jx4YEif3nWR",
-                "name": "Azzie",
-                "mediaType": "image/png"
-              }
-            ],
-            "image": "ipfs://QmeAdLCKgXhxtDAcpPq5vgpRCqYWCGFMzb9jx4YEif3nWR",
-            "project": "Chilled Kongs",
-            "mediaType": "image/png"
-          }
-        }
-      }
-    },
-    "token_registry_metadata": null
-  }
-]
-```
-
 #### get_asset_history
 Get the mint/burn history of an asset<br>
 Parameters:<br>
 Asset Policy<br>
 Asset Name in hexadecimal format (optional), default: all policy assets<br>
-Returns: List of dictionaries with the mint/burn history of an asset<br>
+Returns: List of maps with the mint/burn history of an asset<br>
 Example:<br>
 `asset_history = get_asset_history('07697e6ca1e21777ac76f26d0779c53f7d08e47b9e32d23bd8fed9cd', '4379626572696130363936')`<br>
 Example response:
 ```json
 [
   {
     "policy_id": "07697e6ca1e21777ac76f26d0779c53f7d08e47b9e32d23bd8fed9cd",
@@ -1214,49 +1256,20 @@
         ]
       }
     ]
   }
 ]
 ```
 
-#### get_policy_asset_addresses
-Get the list of addresses with quantity for each asset on the given policy<br>
-Parameters: Asset Policy<br>
-Returns: List of addresses with quantity for each asset on the given policy<br>
-Example:<br>
-`asset_policy_info = get_policy_asset_addresses('07697e6ca1e21777ac76f26d0779c53f7d08e47b9e32d23bd8fed9cd')`<br>
-Example response:
-```json
-[
-  {
-    "asset_name": "4379626572696130303233",
-    "payment_address": "addr1qxu5vk5xafdp39d95ya06d6uya8ldua7crpdzd2an07uw8mrtndmfr0d4qarvgj2wasdwlvrnlqt262jn5asnws7aekssq73gf",
-    "quantity": "1"
-  },
-  {
-    "asset_name": "4379626572696130303330",
-    "payment_address": "addr1q9wj7ylly5nz2kel6huy966tcsw2l3ct9at7m3euhfxyv246nlp3dj9pda2rphtzycwexsaapyk73k25y3j5neyhg45s879sk4",
-    "quantity": "1"
-  },
-  ...
-  {
-    "asset_name": "4379626572696132383338",
-    "payment_address": "addr1qxg2l50ryn6z23543v6nujvkql9zwj7f7hvsjwalw6jvf25n5k332a42ge9w5en95g9af59fft32g0la0qtfr9vfyyesccney2",
-    "quantity": "1"
-  }
-]
-```
-
-
-#### get_policy_asset_info
-Get the list of asset under the given policy (including balances)<br>
+#### get_asset_policy_info
+Get the information for all assets under the same policy<br>
 Parameters: Asset Policy<br>
-Returns: List of dictionaries with the policy assets<br>
+Returns: List of maps with the policy assets<br>
 Example:<br>
-`asset_policy_info = get_policy_asset_info('07697e6ca1e21777ac76f26d0779c53f7d08e47b9e32d23bd8fed9cd')`<br>
+`asset_policy_info = get_asset_policy_info('07697e6ca1e21777ac76f26d0779c53f7d08e47b9e32d23bd8fed9cd')`<br>
 Example response:
 ```json
 [
   {
     "asset_name": "",
     "asset_name_ascii": "",
     "fingerprint": "asset1pht97cylpt7azuu9mwhmd9c9zdgmumwrrm5yrc",
@@ -1390,127 +1403,20 @@
     "token_registry_metadata": null,
     "total_supply": "1",
     "creation_time": 1670493734
   }
 ]
 ```
 
-#### get_policy_asset_list
-Get the list of asset under the given policy (including balances)<br>
-Parameters: Asset Policy<br>
-Returns: List of dictionaries with the asset under the given policy<br>
-Example:<br>
-`asset_policy_list = get_policy_asset_list('07697e6ca1e21777ac76f26d0779c53f7d08e47b9e32d23bd8fed9cd')`<br>
-Example response:
-```json
-[
-  {
-    "asset_name": "",
-    "asset_name_ascii": "",
-    "fingerprint": "asset1pht97cylpt7azuu9mwhmd9c9zdgmumwrrm5yrc",
-    "minting_tx_hash": "90415fda215ff5098d7fa1385c7358c589066332068b720380726e3ef0b26de4",
-    "total_supply": "0",
-    "mint_cnt": 1,
-    "burn_cnt": 1,
-    "creation_time": 1665100800,
-    "minting_tx_metadata": {
-      "777": {
-        "addr": [
-          "addr1qy36jns6h4w4f80u6xed49k6qn9c7tk4x4us5kaxztjq8x3un2me8nvc5ke",
-          "gvll0gnwlj2ypzfhhqpns47u76gafttmq208x4d"
-        ],
-        "rate": "0.05"
-      }
-    },
-    "token_registry_metadata": null
-  },
-  ...
-  {
-    "asset_name": "4379626572696130333939",
-    "asset_name_ascii": "Cyberia0399",
-    "fingerprint": "asset1g7tgq2ly8uhtzcz79uhay8tq46h9rq62arfm8s",
-    "minting_tx_hash": "98db0a36106a92149b256887f6300f2b228e14d24d488e4b1614920083cd64ff",
-    "total_supply": "1",
-    "mint_cnt": 1,
-    "burn_cnt": 0,
-    "creation_time": 1665187200,
-    "minting_tx_metadata": {
-      "721": {
-        "nonce": "c966f455d3e03537",
-        "07697e6ca1e21777ac76f26d0779c53f7d08e47b9e32d23bd8fed9cd": {
-          "Cyberia0399": {
-            "Pose": "Lunge pose - Anjaneyasana",
-            "Skin": "Gold",
-            "name": "Cyberia Chakra Planet #0399",
-            "files": [
-              {
-                "src": "ipfs://QmVsMggcQE3da9xuZv7uvJRH84gs5ebGQ8kxVPSQw52XRf",
-                "name": "Please wait while your experience below loads.",
-                "mediaType": "image/jpg"
-              },
-              {
-                "src": "ipfs://QmSHyNm11PrqyrUXszKtsz52ADH6A934c3gw41H7CMCj7D",
-                "mediaType": "text/html"
-              }
-            ],
-            "image": "ipfs://QmVsMggcQE3da9xuZv7uvJRH84gs5ebGQ8kxVPSQw52XRf",
-            "Artist": "Srink",
-            "Avatar": "Male",
-            "Chakra": "Sacral - Svadhisthana",
-            "Mantra": "VAM",
-            "Discord": "https://dsc.gg/cyberiacnft",
-            "Twitter": "https://twitter.com/cyberiaCNFT",
-            "Website": "https://cyberia.gg/",
-            "Function": "Sexual and Creative Energy",
-            "Location": "Below the Belly Button",
-            "Collection": "Chakra Planets",
-            "Planet colour": "Orange"
-          },
-          "Cyberia2795": {
-            "Pose": "Headstand - Sirsasana",
-            "Skin": "Gold",
-            "name": "Cyberia Chakra Planet #2795",
-            "files": [
-              {
-                "src": "ipfs://QmZ4TGY2Jzy5JGaD3S7RLsrP9K8jbp44e7463iHAGitM5a",
-                "name": "Please wait while your experience below loads.",
-                "mediaType": "image/jpg"
-              },
-              {
-                "src": "ipfs://QmcEqKkAcxeGNZimSiQZ2duZA4sx4xJawh35VwuJoS3A9m",
-                "mediaType": "text/html"
-              }
-            ],
-            "image": "ipfs://QmZ4TGY2Jzy5JGaD3S7RLsrP9K8jbp44e7463iHAGitM5a",
-            "Artist": "Srink",
-            "Avatar": "Female",
-            "Chakra": "Crown - Sahasrara",
-            "Mantra": "OM",
-            "Discord": "https://dsc.gg/cyberiacnft",
-            "Twitter": "https://twitter.com/cyberiaCNFT",
-            "Website": "https://cyberia.gg/",
-            "Function": "Spiritual Connection",
-            "Location": "Top of the Head",
-            "Collection": "Chakra Planets",
-            "Planet colour": "Purple"
-          }
-        }
-      }
-    },
-    "token_registry_metadata": null
-  }
-]
-```
-
 #### get_asset_summary
 Get the summary of an asset (total transactions exclude minting/total wallets include only wallets with asset balance)<br>
 Parameters:<br>
 Asset Policy<br>
 Asset Name in hexadecimal format (optional), default: all policy assets<br>
-Returns: List of dictionaries with the mint/burn history of an asset<br>
+Returns: List of maps with the mint/burn history of an asset<br>
 Example:<br>
 `asset_summary = get_asset_summary('07697e6ca1e21777ac76f26d0779c53f7d08e47b9e32d23bd8fed9cd', '4379626572696131313535')`<br>
 Example response:
 ```json
 [
   {
     "policy_id": "07697e6ca1e21777ac76f26d0779c53f7d08e47b9e32d23bd8fed9cd",
@@ -1526,15 +1432,15 @@
 #### get_asset_txs
 Get the list of all asset transaction hashes (the newest first)<br>
 Parameters:<br>
 Asset Policy<br>
 Asset Name in hexadecimal format (optional), default: all policy assets<br>
 Block number (optional) - return only the transactions after this block<br>
 History boolean (optional) - include all historical transactions, setting to false includes only the non-empty ones<br>
-Returns: List of dictionaries with the mint/burn history of an asset<br>
+Returns: List of maps with the mint/burn history of an asset<br>
 Example:<br>
 `asset_txs = get_asset_txs('07697e6ca1e21777ac76f26d0779c53f7d08e47b9e32d23bd8fed9cd', '4379626572696131313535')`<br>
 Example response:
 ```json
 [
   {
     "tx_hash": "d4ac560398b95e6435bd6657e39fe5638f7c5bfaa6ffa6b8fa9bfae0b4882666",
@@ -1546,15 +1452,15 @@
 ```
 
 ### Pool
 
 #### get_pools_list
 A list of all currently registered/retiring (not retired) pools<br>
 Parameters: none<br>
-Returns: The list of stake pool dictionaries<br>
+Returns: The list of stake pool maps<br>
 Example:<br>
 `pool_list = get_pool_list()`<br>
 Example response:
 ```json
 [
   {
     "pool_id_bech32": "pool100wj94uzf54vup2hdzk0afng4dhjaqggt7j434mtgm8v2gfvfgp",
@@ -1641,15 +1547,15 @@
   }
 ]
 ```
 
 #### get_pool_stake_snapshot
 Returns Mark, Set and Go stake snapshots for the selected pool, useful for leaderlog calculation<br>
 Parameters: Stake pool bech32 id<br>
-Returns: Pool snapshot as list of dictionaries by epoch (current and previous 2)<br>
+Returns: Pool snapshot as list of maps by epoch (current and previous 2)<br>
 Example:<br>
 `pool_stake_snapshot = get_pool_stake_snapshot('pool155efqn9xpcf73pphkk88cmlkdwx4ulkg606tne970qswczg3asc')`<br>
 Example response:
 ```json
 [
   {
     "snapshot": "Go",
@@ -1674,15 +1580,15 @@
   }
 ]
 ```
 
 #### get_pool_delegators
 Returns information about live delegators for a given pool<br>
 Parameters Stake pool bech32 id<br>
-Returns: The list of pool delegators dictionaries<br>
+Returns: The list of pool delegators maps<br>
 Example:<br>
 `pool_delegators = get_pool_delegators('pool12wpfng6cu7dz38yduaul3ngfm44xhv5xmech68m5fwe4wu77udd')`<br>
 Example response:
 ```json
 [
   {
     "stake_address": "stake1u80603g5n7vtycl75c60jmv56jx3cw53v23xv0txkpcu8kcwr2k27",
@@ -1707,15 +1613,15 @@
 ```
 
 #### get_pool_delegators_history
 Returns information about active delegators (incl. history) for a given pool and epoch number (all epochs if not specified)<br>
 Parameters:<br>
 Stake pool bech32 id<br>
 Epoch (optional)<br>
-Returns: The list of pool delegators dictionaries<br>
+Returns: The list of pool delegators maps<br>
 Example:<br>
 `pool_delegators_history = get_pool_delegators_history('pool12wpfng6cu7dz38yduaul3ngfm44xhv5xmech68m5fwe4wu77udd', 380)`<br>
 Example response:
 ```json
 [
   {
     "stake_address": "stake1uyezz2wzt4rl5wug8ju8zshvfzkw2lksw8jfp0wpueq2nccnnkwxh",
@@ -1737,15 +1643,15 @@
 ```
 
 #### get_pool_blocks
 Returns information about blocks minted by a given pool for all epochs (or _epoch_no if provided)<br>
 Parameters:<br>
 Stake pool bech32 id<br>
 Epoch (optional)<br>
-Returns: The list of pool blocks dictionaries<br>
+Returns: The list of pool blocks maps<br>
 Example:<br>
 `pool_blocks = get_pool_blocks('pool12wpfng6cu7dz38yduaul3ngfm44xhv5xmech68m5fwe4wu77udd', 380)`<br>
 Example response:
 ```json
 [
   {
     "epoch_no": 380,
@@ -1767,15 +1673,15 @@
 ```
 
 #### get_pool_history
 Returns information about pool stake, block and reward history in a given epoch (or all epochs that pool existed for, in descending order if no epoch number was provided)<br>
 Parameters:<br>
 Stake pool bech32 id<br>
 Epoch (optional)<br>
-Returns:  Information about pool stake, block and reward history as a list dictionaries by epoch (descending)<br>
+Returns:  Information about pool stake, block and reward history as a list maps by epoch (descending)<br>
 Example:<br>
 `pool_history = get_pool_history('pool12wpfng6cu7dz38yduaul3ngfm44xhv5xmech68m5fwe4wu77udd', 379)`<br>
 Example response:
 ```json
 [
   {
     "epoch_no": 379,
@@ -1792,15 +1698,15 @@
   }
 ]
 ```
 
 #### get_pool_updates
 Returns all pool updates for all pools or only updates for specific pool if specified<br>
 Parameters: Stake pool bech32 id (optional)<br>
-Returns: pool updates as a list of dictionaries<br>
+Returns: pool updates as a list of maps<br>
 Example:<br>
 `pool_updates = get_pool_updates('pool12wpfng6cu7dz38yduaul3ngfm44xhv5xmech68m5fwe4wu77udd')`<br>
 Example response:
 ```json
 [
   {
     "tx_hash": "6358622ef9c7a395aaf1590661330a17095fef3c39caa2ae319c737c85bfacb9",
@@ -1881,15 +1787,15 @@
   ...
 ]
 ```
 
 #### get_pool_relays
 A list of registered relays for all currently registered/retiring (not retired) pools<br>
 Parameters: none<br>
-Returns: The list of relays dictionaries by stake pool<br>
+Returns: The list of relays maps by stake pool<br>
 Example:<br>
 `pool_relays = get_pool_relays()`<br>
 Example response:
 ```json
 [
   {
     "pool_id_bech32": "pool100wj94uzf54vup2hdzk0afng4dhjaqggt7j434mtgm8v2gfvfgp",
@@ -1930,15 +1836,15 @@
   ...
 ]
 ```
 
 #### get_pool_metadata
 A list of registered relays for all currently registered/retiring (not retired) pools<br>
 Parameters: Stake pool bech32 ID(s) as string (for one stake pool) or list of stake pool bech32 IDs (for multiple stake pools)<br>
-Returns: The list of pool metadata dictionaries<br>
+Returns: The list of pool metadata maps<br>
 Example:<br>
 `pool_metadata = get_pool_metadata('pool1auvwj75q70s7jce63nvptujs6460kvyxqn0wjegkz4mhja7g5t6')`<br>
 Example response:
 ```json
 [
   {
     "pool_id_bech32": "pool1auvwj75q70s7jce63nvptujs6460kvyxqn0wjegkz4mhja7g5t6",
@@ -1953,15 +1859,15 @@
   }
 ]
 ```
 
 #### get_retiring_pools
 Get the retiring stake pools list<br>
 Parameters: none<br>
-Returns: The list of retiring pools dictionaries<br>
+Returns: The list of retiring pools maps<br>
 Example:<br>
 `retiring_pools = get_retiring_pools()`<br>
 Example response:
 ```json
 [
   {
     "tx_hash": "39a046ef9b5b9e149d24bae8c86f6fb93b08d57312615d22b6a3e73279198e73",
@@ -2025,15 +1931,15 @@
 ```
 
 ### Script
 
 #### get_native_script_list
 List of all existing native script hashes along with their creation transaction hashes<br>
 Parameters: none<br>
-Returns: The list of all native scripts dictionaries<br>
+Returns: The list of all native scripts maps<br>
 Example:<br>
 `native_script_list = get_native_script_list()`<br>
 Example response:
 ```json
 [
   {
     "script_hash": "65c197d565e88a20885e535f93755682444d3c02fd44dd70883fe89e",
@@ -2078,15 +1984,15 @@
   ...
 ]
 ```
 
 #### get_plutus_script_list
 List of all existing native script hashes along with their creation transaction hashes<br>
 Parameters: none<br>
-Returns: The list of all plutus scripts dictionaries<br>
+Returns: The list of all plutus scripts maps<br>
 Example:<br>
 `plutus_script_list = get_plutus_script_list()`<br>
 Example response:
 ```json
 [
   {
     "script_hash": "c916b3d14a51087cc967223aad3f2e4e5c01993f5429719c32c2061e",
@@ -2103,15 +2009,15 @@
   ...
 ]
 ```
 
 #### get_script_redeemers
 List of all redeemers for a given script hash<br>
 Parameters: Script hash<br>
-Returns: Redeemers list as dictionary<br>
+Returns: Redeemers list as map<br>
 Example:<br>
 `script_redeemers = get_script_redeemers('c1996b36d11bf42103745844cc5ee9bf13fde475fa909809e2da7261')`<br>
 Example response:
 ```json
 [
   {
     "script_hash": "c1996b36d11bf42103745844cc5ee9bf13fde475fa909809e2da7261",
@@ -2132,312 +2038,22 @@
   }
 ]
 ```
 
 #### get_datum_info
 List of datum information for given datum hashes<br>
 Parameters: Datum hash(es) as string (for one datum hash) or list (for a list of datum hashes)<br>
-Returns Datum information as list of dictionaries<br>
+Returns Datum information as list of maps<br>
 Example:<br>
 `datum_info = get_datum_info('45b0cfc220ceec5b7c1c62c4d4193d38e4eba48e8815729ce75f9c0ab0e4c1c0')`<br>
 Example response:
 ```json
 [
   {
     "hash": "45b0cfc220ceec5b7c1c62c4d4193d38e4eba48e8815729ce75f9c0ab0e4c1c0",
     "value": {
       "list": []
     },
     "bytes": "80"
   }
 ]
 ```
-
-### Stake Account
-
-#### get_account_list
-Get a list of all accounts<br>
-Parameters:<br>
-The offset (optional) to start from, default 0<br>
-The maximum number of accounts to return (optional), default 0 (no limit)<br>
-Returns: The list of accounts dictionaries<br>
-This takes a very long time to execute (about one hour), because the total number of accounts is in the millions range.<br>
-Example:<br>
-`account_list = get_account_list()`<br>
-Example response:
-```json
-[
-  {
-    "id": "stake1uyfmzu5qqy70a8kq4c8rw09q0w0ktfcxppwujejnsh6tyrg5c774g"
-  },
-  {
-    "id": "stake1uydhlh7f2kkw9eazct5zyzlrvj32gjnkmt2v5qf6t8rut4qwch8ey"
-  },
-  {
-    "id": "stake1uxsgkz6fvgws5wn80vckwvghzapnhfmf0672nmmkm2tt9fcaau5sw"
-  },
-  ...
-]
-```
-
-#### get_account_info
-Get the account information for given stake addresses (accounts)<br>
-Parameters: Stake address(es), as a string (for one address) or a list (for multiple addresses)<br>
-Returns: The list of account information dictionaries<br>
-Example:<br>
-`account_info = get_account_info('stake1uy4jj73pfyejl4d2rs6nc70eykkhhu56p3y2rj2tdayfzeqnjyh0j')`<br>
-Example response:
-```json
-[
-  {
-    "stake_address": "stake1uy4jj73pfyejl4d2rs6nc70eykkhhu56p3y2rj2tdayfzeqnjyh0j",
-    "status": "registered",
-    "delegated_pool": "pool18r2y72aue5nmv489xtnfxl36vzusq95qst6urd87yd5hgzms04c",
-    "total_balance": "20418617",
-    "utxo": "20418617",
-    "rewards": "0",
-    "withdrawals": "0",
-    "rewards_available": "0",
-    "reserves": "0",
-    "treasury": "0"
-  }
-]
-```
-
-#### get_account_utxos
-Get a list of assets registered via token registry on github<br>
-Parameters: Stake address<br>
-Returns: The list of all UTxOs at all payment addresses associated with the stake address<br>
-Example:<br>
-`account_utxos = get_account_utxos('stake1ux5r7myfhycj234wpqyhh3h8skgwvq0hsstpw52f66857uq95cas6')`
-Example response:<br>
-```json
-[
-  {
-	"tx_hash": "215bcaa7b13c491db28d5525d9b2a13a7d8ddabd563da8113a449ab33a6a60be",
-	"tx_index": 2,
-	"address": "addr1q9dwzug2qzdsqvpvrn886nqdtwr02n9kxtwqsxce2gacvedg8akgnwf3y4r2uzqf00rw0pvsucql0pqkzag5n450facqeuerev",
-	"value": "85813474",
-	"block_height": 8214437,
-	"block_time": 1672580966
-  },
-  {
-	"tx_hash": "1eb26dce2f471fbe32aa8cb303f5e8d8078d1da4dbbb78a7bc135036bb3f2f9c",
-	"tx_index": 0,
-	"address": "addr1q88u9gz83nhs9p5pud9kyucx8sg0ygae2p9a4g2p2y55c4ag8akgnwf3y4r2uzqf00rw0pvsucql0pqkzag5n450facqqyd2n7",
-	"value": "110094569",
-	"block_height": 8406870,
-	"block_time": 1676555396
-  },
-  {
-	"tx_hash": "d530de851c2f867f2174c1073b04bdb9f2e2d16029fcfb488e8150ba66976d43",
-	"tx_index": 0,
-	"address": "addr1qxyp2wsafavj47dpc6uqgqx8se3969jn4crfk7y4zwd7vfag8akgnwf3y4r2uzqf00rw0pvsucql0pqkzag5n450facqlyvudm",
-	"value": "1249900",
-	"block_height": 8489290,
-	"block_time": 1678248733
-  },
-  ...
-  {
-	"tx_hash": "d8e3ca8b36f9a785ff33f01aa5460f9248ea94acd621ea187093206b04aa6e30",
-	"tx_index": 0,
-	"address": "addr1q8txa88kt6rpdv3zzn8ghx7u4udf6rpj690rfdvlqn35fldg8akgnwf3y4r2uzqf00rw0pvsucql0pqkzag5n450facqplx97u",
-	"value": "54000000",
-	"block_height": 8759577,
-	"block_time": 1683809438
-  }
-]
-```
-
-#### get_account_info_cached
-Get the cached account information for given stake addresses (accounts)<br>
-Parameters: Stake address(es), as a string (for one address) or a list (for multiple addresses)<br>
-Returns: The list of account information dictionaries<br>
-Example:<br>
-`account_info_cached = get_account_info_cached('stake1uy4jj73pfyejl4d2rs6nc70eykkhhu56p3y2rj2tdayfzeqnjyh0j')`<br>
-Example response:
-```json
-[
-  {
-    "stake_address": "stake1uy4jj73pfyejl4d2rs6nc70eykkhhu56p3y2rj2tdayfzeqnjyh0j",
-    "status": "registered",
-    "delegated_pool": "pool18r2y72aue5nmv489xtnfxl36vzusq95qst6urd87yd5hgzms04c",
-    "total_balance": "20418617",
-    "utxo": "20418617",
-    "rewards": "0",
-    "withdrawals": "0",
-    "rewards_available": "0",
-    "reserves": "0",
-    "treasury": "0"
-  }
-]
-```
-
-#### get_account_rewards
-Get the full rewards history (including MIR) for given stake addresses (accounts)<br>
-Parameters:<br>
-Stake address(es), as a string (for one address) or a list (for multiple addresses)<br>
-Epoch (optional), default: current epoch<br>
-Returns: The list of rewards dictionaries by account (stake address)<br>
-Example:<br>
-`account_rewards = get_account_rewards('stake1u8lhspu67x3jejzcfrh487rtu3hnm26cg0jsn0mgh2y6n9q9ve26z')`<br>
-Example response:
-```json
-[
-  {
-    "stake_address": "stake1u8lhspu67x3jejzcfrh487rtu3hnm26cg0jsn0mgh2y6n9q9ve26z",
-    "rewards": [
-      {
-        "earned_epoch": 233,
-        "spendable_epoch": 235,
-        "amount": "3990414",
-        "type": "member",
-        "pool_id": "pool1jdhjfcu34lq88rypdtslzwyf27uh0h3apcr9mjd68zhc69r29fy"
-      },
-      {
-        "earned_epoch": 234,
-        "spendable_epoch": 236,
-        "amount": "2792902",
-        "type": "member",
-        "pool_id": "pool1jdhjfcu34lq88rypdtslzwyf27uh0h3apcr9mjd68zhc69r29fy"
-      },
-      ...
-      {
-        "earned_epoch": 379,
-        "spendable_epoch": 381,
-        "amount": "6496870",
-        "type": "member",
-        "pool_id": "pool12wpfng6cu7dz38yduaul3ngfm44xhv5xmech68m5fwe4wu77udd"
-      }
-    ]
-  }
-]
-```
-
-#### get_account_updates
-Get the account updates (registration, deregistration, delegation and withdrawals) for given stake addresses (accounts)<br>
-Parameters: Stake address(es), as a string (for one address) or a list (for multiple addresses)<br>
-Returns: The list of account updates dictionaries by account (stake address)<br>
-Example:<br>
-`account_updates = get_account_updates('stake1u8lhspu67x3jejzcfrh487rtu3hnm26cg0jsn0mgh2y6n9q9ve26z')`<br>
-Example response:
-```json
-[
-  {
-    "stake_address": "stake1u8lhspu67x3jejzcfrh487rtu3hnm26cg0jsn0mgh2y6n9q9ve26z",
-    "updates": [
-      {
-        "action_type": "withdrawal",
-        "tx_hash": "487bc75f00fe934dad33683271cca8540fe868eef7025962678f179a1a111ecc",
-        "epoch_no": 324,
-        "epoch_slot": 70687,
-        "absolute_slot": 54675487,
-        "block_time": 1646241778
-      },
-      {
-        "action_type": "withdrawal",
-        "tx_hash": "eb3ffa01f434e210716151fd9001af82529e371a91c20af02512942f988a2119",
-        "epoch_no": 269,
-        "epoch_slot": 339679,
-        "absolute_slot": 31184479,
-        "block_time": 1622750770
-      },
-      ...
-      {
-        "action_type": "withdrawal",
-        "tx_hash": "b056dcbff9b908e1bd3ed015466f64486538058ba3553dbf885b216d88343370",
-        "epoch_no": 252,
-        "epoch_slot": 58375,
-        "absolute_slot": 23559175,
-        "block_time": 1615125466
-      }
-    ]
-  }
-]
-```
-
-#### get_account_addresses
-Get all addresses associated with given staking accounts<br>
-Parameters: Stake address(es), as a string (for one address) or a list (for multiple addresses)<br>
-Returns: The list of addresses dictionaries by account (stake address)<br>
-Example:<br>
-`account_addresses = get_account_addresses('stake1u8lhspu67x3jejzcfrh487rtu3hnm26cg0jsn0mgh2y6n9q9ve26z')`<br>
-Example response:
-```json
-[
-  {
-    "stake_address": "stake1u8lhspu67x3jejzcfrh487rtu3hnm26cg0jsn0mgh2y6n9q9ve26z",
-    "addresses": [
-      "addr1qxwjxvzv8rmyutcjp0647w4n05wv7aez9jdmqcxn8a9sshll0qre4udr9ny9sj8020uxher08k44ssl9pxlk3w5f4x2qjyz9yf"
-    ]
-  }
-]
-```
-
-#### get_account_assets
-Get the native asset balance of given accounts<br>
-Parameters: Stake address(es), as a string (for one address) or a list (for multiple addresses)<br>
-Returns: The list of account assets dictionaries by account (stake address)<br>
-Example:<br>
-`account_assets = get_account_assets('stake1u8lhspu67x3jejzcfrh487rtu3hnm26cg0jsn0mgh2y6n9q9ve26z')`<br>
-Example response:
-```json
-[
-  {
-    "stake_address": "stake1u8lhspu67x3jejzcfrh487rtu3hnm26cg0jsn0mgh2y6n9q9ve26z",
-    "asset_list": [
-      {
-        "policy_id": "0029cb7c88c7567b63d1a512c0ed626aa169688ec980730c0473b913",
-        "asset_name": "6c70202302",
-        "fingerprint": "asset1awuysx8hc686uz0dykmvmc7jfut2ulceucf6yc",
-        "quantity": "418089787"
-      },
-      {
-        "policy_id": "0029cb7c88c7567b63d1a512c0ed626aa169688ec980730c0473b913",
-        "asset_name": "6c7020f302",
-        "fingerprint": "asset1mcq0awl6awlaqg0ywukf94q0mnau263l9rght5",
-        "quantity": "586811406"
-      },
-      ...
-      {
-        "policy_id": "ea2d23f1fa631b414252824c153f2d6ba833506477a929770a4dd9c2",
-        "asset_name": "4d414442554c",
-        "fingerprint": "asset1q0kwjy669gmsqpvxp4lr0sp26pdm0dafme3qp2",
-        "quantity": "500"
-      }
-    ]
-  }
-]
-```
-
-#### get_account_history
-Get the staking history of given stake addresses (accounts)<br>
-Parameters: Stake address(es), as a string (for one address) or a list (for multiple addresses)<br>
-Returns: The list of staking history dictionaries by account (stake address)<br>
-Example:<br>
-`account_history = get_account_history('stake1u8lhspu67x3jejzcfrh487rtu3hnm26cg0jsn0mgh2y6n9q9ve26z')`<br>
-Example response:
-```json
-[
-  {
-    "stake_address": "stake1u8lhspu67x3jejzcfrh487rtu3hnm26cg0jsn0mgh2y6n9q9ve26z",
-    "history": [
-      {
-        "pool_id": "pool1jdhjfcu34lq88rypdtslzwyf27uh0h3apcr9mjd68zhc69r29fy",
-        "epoch_no": 233,
-        "active_stake": "4655706122"
-      },
-      {
-        "pool_id": "pool1jdhjfcu34lq88rypdtslzwyf27uh0h3apcr9mjd68zhc69r29fy",
-        "epoch_no": 234,
-        "active_stake": "5020706122"
-      },
-      ...
-      {
-        "pool_id": "pool12wpfng6cu7dz38yduaul3ngfm44xhv5xmech68m5fwe4wu77udd",
-        "epoch_no": 381,
-        "active_stake": "10247851319"
-      }
-    ]
-  }
-]
-```
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `koios-api-1.0.10/pyproject.toml` & `koios-api-1.0.2/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [build-system]
 requires = ['setuptools>=61.0']
 build-backend = 'setuptools.build_meta'
 [project]
 name = "koios-api"
-version = "1.0.10"
+version = "1.0.2"
 authors = [
   { name="APEX Stake Pool", email="cardanoapexpool@gmail.com" },
 ]
 description = "A python package for the Cardano Blockchain Koios API (https://api.koios.rest/)"
 keywords = [
     "koios",
     "cardano",
```

### Comparing `koios-api-1.0.10/src/koios_api/account.py` & `koios-api-1.0.2/src/koios_api/account.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 import json
 import requests
 import inspect
 from time import sleep
 from .__config__ import *
 
 
-def get_account_list(offset: int = 0, limit: int = 0) -> list:
+def get_account_list(offset=0, limit=0):
     """
     https://api.koios.rest/#get-/account_list
-    Get a list of all stake addresses that have at least 1 transaction
+    Get a list of all accounts
     :param offset: The offset to start from (optional)
     :param limit: The maximum number of accounts to return (optional)
     :returns: The list of accounts maps
     """
     url = API_BASE_URL + '/account_list'
     headers = {'Accept': 'application/json', 'Content-Type': 'application/json'}
     parameters = {}
@@ -21,31 +21,29 @@
         if offset > 0:
             parameters['offset'] = offset
         while True:
             try:
                 resp = json.loads(requests.get(url, headers=headers, params=parameters).text)
                 break
             except Exception as e:
-                print(f"Exception in {inspect.getframeinfo(inspect.currentframe()).function}: {e}")
+                print('Exception in %s: %s' % (inspect.getframeinfo(inspect.currentframe()).function, e))
                 sleep(SLEEP_TIME)
                 print('offset: %s, retrying...' % offset)
         account_list += resp
-        if len(resp) < API_RESP_COUNT:
-            if 0 < limit <= len(account_list):
-                account_list = account_list[0:limit]
+        if len(resp) < 1000:
             break
         else:
             offset += len(resp)
         if 0 < limit <= len(account_list):
             account_list = account_list[0:limit]
             break
     return account_list
 
 
-def get_account_info(addr: [str, list]) -> list:
+def get_account_info(addr):
     """
     https://api.koios.rest/#post-/account_info
     Get the account information for given stake addresses (accounts)
     :param addr: Stake address(es), as a string (for one address) or a list (for multiple addresses)
     :returns: The list of account information maps
     """
     url = API_BASE_URL + '/account_info'
@@ -56,58 +54,23 @@
     else:
         stake_addresses['_stake_addresses'] = [addr]
     while True:
         try:
             resp = json.loads(requests.post(url, headers=headers, data=json.dumps(stake_addresses)).text)
             break
         except Exception as e:
-            print(f"Exception in {inspect.getframeinfo(inspect.currentframe()).function}: {e}")
+            print('Exception in %s: %s' % (inspect.getframeinfo(inspect.currentframe()).function, e))
             sleep(SLEEP_TIME)
             print('retrying...')
     return resp
 
 
-def get_account_utxos(addr: str, offset: int = 0, limit: int = 0) -> list:
+def get_account_info_cached(addr):
     """
-    https://api.koios.rest/#get-/account_utxos
-    :param addr: Cardano staking address (reward account) in bech32 format
-    :param offset: The offset to start from (optional)
-    :param limit: The maximum number of UTxOs to return (optional)
-    :return: The list of all UTxOs for a given stake address (account)
-    """
-    url = API_BASE_URL + '/account_utxos'
-    parameters = {'_stake_address': addr}
-    utxos = []
-    while True:
-        if offset > 0:
-            parameters['offset'] = offset
-        while True:
-            try:
-                resp = json.loads(requests.get(url, params=parameters).text)
-                break
-            except Exception as e:
-                print(f"Exception in {inspect.getframeinfo(inspect.currentframe()).function}: {e}")
-                sleep(SLEEP_TIME)
-                print('retrying...')
-        utxos += resp
-        if len(resp) < API_RESP_COUNT:
-            if 0 < limit <= len(utxos):
-                utxos = utxos[0:limit]
-            break
-        else:
-            offset += len(resp)
-        if 0 < limit <= len(utxos):
-            utxos = utxos[0:limit]
-            break
-    return utxos
-
-
-def get_account_info_cached(addr: [str, list]) -> list:
-    """
-    https://api.koios.rest/#post-/account_info_cached
+    https://api.koios.rest/#post-/account_info
     Get the cached account information for given stake addresses (accounts)
     :param addr: Stake address(es), as a string (for one address) or a list (for multiple addresses)
     :returns: The list of account information maps
     """
     url = API_BASE_URL + '/account_info_cached'
     headers = {'Accept': 'application/json', 'Content-Type': 'application/json'}
     stake_addresses = {}
@@ -116,21 +79,21 @@
     else:
         stake_addresses['_stake_addresses'] = [addr]
     while True:
         try:
             resp = json.loads(requests.post(url, headers=headers, data=json.dumps(stake_addresses)).text)
             break
         except Exception as e:
-            print(f"Exception in {inspect.getframeinfo(inspect.currentframe()).function}: {e}")
+            print('Exception in %s: %s' % (inspect.getframeinfo(inspect.currentframe()).function, e))
             sleep(SLEEP_TIME)
             print('retrying...')
     return resp
 
 
-def get_account_rewards(addr: [str, list], epoch: int = 0) -> list:
+def get_account_rewards(addr, epoch=0):
     """
     https://api.koios.rest/#post-/account_rewards
     Get the full rewards history (including MIR) for given stake addresses (accounts)
     :param addr: Stake address(es), as a string (for one address) or a list (for multiple addresses)
     :param epoch: Epoch (optional), default: current epoch
     :returns: The list of rewards maps by account (stake address)
     """
@@ -144,21 +107,21 @@
     if isinstance(epoch, int) and epoch > 0:
         stake_addresses['_epoch_no'] = epoch
     while True:
         try:
             resp = json.loads(requests.post(url, headers=headers, data=json.dumps(stake_addresses)).text)
             break
         except Exception as e:
-            print(f"Exception in {inspect.getframeinfo(inspect.currentframe()).function}: {e}")
+            print('Exception in %s: %s' % (inspect.getframeinfo(inspect.currentframe()).function, e))
             sleep(SLEEP_TIME)
             print('retrying...')
     return resp
 
 
-def get_account_updates(addr: [str, list]) -> list:
+def get_account_updates(addr):
     """
     https://api.koios.rest/#post-/account_updates
     Get the account updates (registration, deregistration, delegation and withdrawals)
     for given stake addresses (accounts)
     :param addr: Stake address(es), as a string (for one address) or a list (for multiple addresses)
     :returns: The list of account updates maps by account (stake address)
     """
@@ -170,21 +133,21 @@
     else:
         stake_addresses['_stake_addresses'] = [addr]
     while True:
         try:
             resp = json.loads(requests.post(url, headers=headers, data=json.dumps(stake_addresses)).text)
             break
         except Exception as e:
-            print(f"Exception in {inspect.getframeinfo(inspect.currentframe()).function}: {e}")
+            print('Exception in %s: %s' % (inspect.getframeinfo(inspect.currentframe()).function, e))
             sleep(SLEEP_TIME)
             print('retrying...')
     return resp
 
 
-def get_account_addresses(addr: [str, list]) -> list:
+def get_account_addresses(addr):
     """
     https://api.koios.rest/#post-/account_addresses
     Get all addresses associated with given staking accounts
     :param addr: Stake address(es), as a string (for one address) or a list (for multiple addresses)
     :returns: The list of addresses maps by account (stake address)
     """
     url = API_BASE_URL + '/account_addresses'
@@ -195,21 +158,21 @@
     else:
         stake_addresses['_stake_addresses'] = [addr]
     while True:
         try:
             resp = json.loads(requests.post(url, headers=headers, data=json.dumps(stake_addresses)).text)
             break
         except Exception as e:
-            print(f"Exception in {inspect.getframeinfo(inspect.currentframe()).function}: {e}")
+            print('Exception in %s: %s' % (inspect.getframeinfo(inspect.currentframe()).function, e))
             sleep(SLEEP_TIME)
             print('retrying...')
     return resp
 
 
-def get_account_assets(addr: [str, list]) -> list:
+def get_account_assets(addr):
     """
     https://api.koios.rest/#post-/account_assets
     Get the native asset balance of given accounts
     :param addr: Stake address(es), as a string (for one address) or a list (for multiple addresses)
     :returns: The list of account assets maps by account (stake address)
     """
     url = API_BASE_URL + '/account_assets'
@@ -227,26 +190,26 @@
             parameters['offset'] = offset
         while True:
             try:
                 resp = json.loads(requests.post(url, headers=headers, params=parameters,
                                                 data=json.dumps(stake_addresses)).text)
                 break
             except Exception as e:
-                print(f"Exception in {inspect.getframeinfo(inspect.currentframe()).function}: {e}")
+                print('Exception in %s: %s' % (inspect.getframeinfo(inspect.currentframe()).function, e))
                 sleep(SLEEP_TIME)
                 print('retrying...')
         assets += resp
-        if len(resp) < API_RESP_COUNT:
+        if len(resp) < 1000:
             break
         else:
             offset += len(resp)
     return assets
 
 
-def get_account_history(addr: [str, list], epoch: int = 0) -> list:
+def get_account_history(addr, epoch=0):
     """
     https://api.koios.rest/#post-/account_history
     Get the staking history of given stake addresses (accounts)
     :param addr: Stake address(es), as a string (for one address) or a list (for multiple addresses)
     :param epoch: Epoch (optional) to fetch information for, default: all epochs
     :returns: The list of staking history maps by account (stake address)
     """
@@ -260,11 +223,11 @@
     if epoch:
         stake_addresses['_epoch_no'] = epoch
     while True:
         try:
             resp = json.loads(requests.post(url, headers=headers, data=json.dumps(stake_addresses)).text)
             break
         except Exception as e:
-            print(f"Exception in {inspect.getframeinfo(inspect.currentframe()).function}: {e}")
+            print('Exception in %s: %s' % (inspect.getframeinfo(inspect.currentframe()).function, e))
             sleep(SLEEP_TIME)
             print('retrying...')
     return resp
```

### Comparing `koios-api-1.0.10/src/koios_api/address.py` & `koios-api-1.0.2/src/koios_api/address.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import json
 import requests
 import inspect
 from time import sleep
 from .__config__ import *
 
 
-def get_address_info(addr: [str, list]) -> list:
+def get_address_info(addr):
     """
     https://api.koios.rest/#post-/address_info
     Get address info - balance, associated stake address (if any) and UTxO set for given addresses
     :param addr: Payment address(es) as string (for one address) or list (for multiple addresses)
     :returns: The list of address information maps
     """
     url = API_BASE_URL + '/address_info'
@@ -20,21 +20,21 @@
     else:
         addresses['_addresses'] = [addr]
     while True:
         try:
             resp = json.loads(requests.post(url, headers=headers, data=json.dumps(addresses)).text)
             break
         except Exception as e:
-            print(f"Exception in {inspect.getframeinfo(inspect.currentframe()).function}: {e}")
+            print('Exception in %s: %s' % (inspect.getframeinfo(inspect.currentframe()).function, e))
             sleep(SLEEP_TIME)
             print('retrying...')
     return resp
 
 
-def get_address_txs(addr: [str, list], block_height: int = 0) -> list:
+def get_address_txs(addr, block_height=0):
     """
     https://api.koios.rest/#post-/address_txs
     Get the transaction hash list of input address array, optionally filtering after specified block height (inclusive)
     :param addr: Payment address(es) as string (for one address) or list (for multiple addresses)
     :param block_height: Return only the transactions after this block height. Optional.
     :returns: The list of transactions maps
     """
@@ -48,46 +48,21 @@
     if block_height > 0:
         addresses['_after_block_height'] = block_height
     while True:
         try:
             resp = json.loads(requests.post(url, headers=headers, data=json.dumps(addresses)).text)
             break
         except Exception as e:
-            print(f"Exception in {inspect.getframeinfo(inspect.currentframe()).function}: {e}")
+            print('Exception in %s: %s' % (inspect.getframeinfo(inspect.currentframe()).function, e))
             sleep(SLEEP_TIME)
             print('retrying...')
     return resp
 
 
-def get_credential_utxos(cred: [str, list]) -> list:
-    """
-    https://api.koios.rest/#post-/credential_utxos
-    Get a list of UTxO against input payment credential array including their balances
-    :param cred: Payment credential in hex format as string (for one credential) or list (for multiple credentials)
-    :returns: The list of input payment credentials maps
-    """
-    url = API_BASE_URL + '/credential_utxos'
-    headers = {'Accept': 'application/json', 'Content-Type': 'application/json'}
-    credentials = {}
-    if isinstance(cred, list):
-        credentials['_payment_credentials'] = cred
-    else:
-        credentials['_payment_credentials'] = [cred]
-    while True:
-        try:
-            resp = json.loads(requests.post(url, headers=headers, data=json.dumps(credentials)).text)
-            break
-        except Exception as e:
-            print(f"Exception in {inspect.getframeinfo(inspect.currentframe()).function}: {e}")
-            sleep(SLEEP_TIME)
-            print('retrying...')
-    return resp
-
-
-def get_address_assets(addr: [str, list]) -> list:
+def get_address_assets(addr):
     """
     https://api.koios.rest/#post-/address_assets
     Get the list of all the assets (policy, name and quantity) for given addresses
     :param addr: Payment address(es) as string (for one address) or list (for multiple addresses)
     :returns: The list of assets maps by address
     """
     url = API_BASE_URL + '/address_assets'
@@ -105,26 +80,26 @@
             parameters['offset'] = offset
         while True:
             try:
                 resp = json.loads(requests.post(url, headers=headers, params=parameters,
                                                 data=json.dumps(addresses)).text)
                 break
             except Exception as e:
-                print(f"Exception in {inspect.getframeinfo(inspect.currentframe()).function}: {e}")
+                print('Exception in %s: %s' % (inspect.getframeinfo(inspect.currentframe()).function, e))
                 sleep(SLEEP_TIME)
                 print('retrying...')
         assets += resp
-        if len(resp) < API_RESP_COUNT:
+        if len(resp) < 1000:
             break
         else:
             offset += len(resp)
     return assets
 
 
-def get_credential_txs(cred: [str, list]) -> list:
+def get_credential_txs(cred):
     """
     https://api.koios.rest/#post-/credential_txs
     Get the transaction hash list of input payment credential array,
     optionally filtering after specified block height (inclusive)
     :param cred: Credential(s) as string (for one credential) or list (for multiple credentials)
     :returns: The list of address information maps
     """
@@ -136,11 +111,11 @@
     else:
         credentials['_payment_credentials'] = [cred]
     while True:
         try:
             resp = json.loads(requests.post(url, headers=headers, data=json.dumps(credentials)).text)
             break
         except Exception as e:
-            print(f"Exception in {inspect.getframeinfo(inspect.currentframe()).function}: {e}")
+            print('Exception in %s: %s' % (inspect.getframeinfo(inspect.currentframe()).function, e))
             sleep(SLEEP_TIME)
             print('retrying...')
     return resp
```

### Comparing `koios-api-1.0.10/src/koios_api/asset.py` & `koios-api-1.0.2/src/koios_api/asset.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import json
 import requests
 import inspect
 from time import sleep
 from .__config__ import *
 
 
-def get_asset_list(policy: str = '', offset: int = 0, limit: int = 0) -> list:
+def get_asset_list(policy='', offset=0, limit=0):
     """
     https://api.koios.rest/#get-/asset_list
     Get the list of all native assets (paginated)
     :param policy: Asset Policy (optional), default: all policies
     :param offset: The offset to start from (optional)
     :param limit: The maximum number of accounts to return (optional)
     :returns: The list of assets maps by policy
@@ -23,60 +23,29 @@
         if isinstance(policy, str) and policy != '':
             parameters['policy_id'] = 'eq.' + policy
         while True:
             try:
                 resp = json.loads(requests.get(url, params=parameters).text)
                 break
             except Exception as e:
-                print(f"Exception in {inspect.getframeinfo(inspect.currentframe()).function}: {e}")
+                print('Exception in %s: %s' % (inspect.getframeinfo(inspect.currentframe()).function, e))
                 sleep(SLEEP_TIME)
                 print('retrying...')
         assets_names_hex += resp
-        if len(resp) < API_RESP_COUNT:
-            if 0 < limit <= len(assets_names_hex):
-                assets_names_hex = assets_names_hex[0:limit]
+        if len(resp) < 1000:
             break
         else:
             offset += len(resp)
         if 0 < limit <= len(assets_names_hex):
             assets_names_hex = assets_names_hex[0:limit]
             break
     return assets_names_hex
 
 
-def get_asset_token_registry() -> list:
-    """
-    https://api.koios.rest/#get-/asset_token_registry
-    Get a list of assets registered via token registry on github
-    :returns: List of assets registered via token registry on github
-    """
-    url = API_BASE_URL + '/asset_token_registry'
-    parameters = {}
-    assets_token_registry = []
-    offset = 0
-    while True:
-        if offset > 0:
-            parameters['offset'] = offset
-        while True:
-            try:
-                resp = json.loads(requests.get(url, params=parameters).text)
-                break
-            except Exception as e:
-                print(f"Exception in {inspect.getframeinfo(inspect.currentframe()).function}: {e}")
-                sleep(SLEEP_TIME)
-                print('offset: %d, retrying...' % offset)
-        assets_token_registry += resp
-        if len(resp) < API_RESP_COUNT:
-            break
-        else:
-            offset += len(resp)
-    return assets_token_registry
-
-
-def get_asset_addresses(policy: str, name: str = '') -> list:
+def get_asset_addresses(policy, name=''):
     """
     https://api.koios.rest/#get-/asset_addresses
     Get the list of all addresses holding a given asset
     :param policy: Asset Policy
     :param name: Asset Name in hexadecimal format (optional), default: all policy assets
     :returns: List of maps with the wallets holding the asset and the amount of assets per wallet
     """
@@ -90,26 +59,26 @@
         if offset > 0:
             parameters['offset'] = offset
         while True:
             try:
                 resp = json.loads(requests.get(url, params=parameters).text)
                 break
             except Exception as e:
-                print(f"Exception in {inspect.getframeinfo(inspect.currentframe()).function}: {e}")
+                print('Exception in %s: %s' % (inspect.getframeinfo(inspect.currentframe()).function, e))
                 sleep(SLEEP_TIME)
                 print('offset: %d, retrying...' % offset)
         wallets += resp
-        if len(resp) < API_RESP_COUNT:
+        if len(resp) < 1000:
             break
         else:
             offset += len(resp)
     return wallets
 
 
-def get_asset_address_list(policy: str, name: str = '') -> list:
+def get_asset_address_list(policy, name=''):
     """
     DEPRECATED
     https://api.koios.rest/#get-/asset_address_list
     Get the list of all addresses holding a given asset
     :param policy: Asset Policy
     :param name: Asset Name in hexadecimal format (optional), default: all policy assets
     :returns: List of maps with the wallets holding the asset and the amount of assets per wallet
@@ -122,102 +91,49 @@
     while True:
         paginated_url = url + '&offset=%d' % offset
         while True:
             try:
                 resp = json.loads(requests.get(paginated_url).text)
                 break
             except Exception as e:
-                print(f"Exception in {inspect.getframeinfo(inspect.currentframe()).function}: {e}")
-                sleep(SLEEP_TIME)
-                print('offset: %d, retrying...' % offset)
-        wallets += resp
-        if len(resp) < API_RESP_COUNT:
-            break
-        else:
-            offset += len(resp)
-    return wallets
-
-
-def get_asset_nft_address(policy: str, name: str = '') -> list:
-    """
-    https://api.koios.rest/#get-/asset_nft_address
-    Get the address where specified NFT currently reside on.
-    :param policy: Asset Policy
-    :param name: Asset Name in hexadecimal format
-    :returns: List of maps with the wallets holding the asset and the amount of assets per wallet
-    """
-    url = API_BASE_URL + '/asset_nft_address'
-    parameters = {'_asset_policy': policy, '_asset_name': name}
-    wallets = []
-    offset = 0
-    while True:
-        if offset > 0:
-            parameters['offset'] = offset
-        while True:
-            try:
-                resp = json.loads(requests.get(url, params=parameters).text)
-                break
-            except Exception as e:
-                print(f"Exception in {inspect.getframeinfo(inspect.currentframe()).function}: {e}")
+                print('Exception in %s: %s' % (inspect.getframeinfo(inspect.currentframe()).function, e))
                 sleep(SLEEP_TIME)
                 print('offset: %d, retrying...' % offset)
         wallets += resp
-        if len(resp) < API_RESP_COUNT:
+        if len(resp) < 1000:
             break
         else:
             offset += len(resp)
     return wallets
 
 
-def get_asset_info(policy: str, name: str = '') -> list:
+def get_asset_info(policy, name=''):
     """
     https://api.koios.rest/#get-/asset_info
     Get the information of an asset including first minting & token registry metadata
     :param policy: Asset Policy
-    :param name: Asset Name in hexadecimal format
+    :param name: Asset Name in hexadecimal format (optional), default: all policy assets
     :returns: List of maps with the wallets holding the asset and the amount of assets per wallet
     """
     url = API_BASE_URL + '/asset_info'
-    parameters = {'_asset_policy': policy, '_asset_name': name}
+    parameters = {'_asset_policy': policy}
+    if isinstance(name, str) and name != '':
+        parameters['_asset_name=%s'] = name
     while True:
         try:
             resp = json.loads(requests.get(url, params=parameters).text)
             break
         except Exception as e:
-            print(f"Exception in {inspect.getframeinfo(inspect.currentframe()).function}: {e}")
-            sleep(SLEEP_TIME)
-            print('retrying...')
-    return resp
-
-
-def get_asset_info_bulk(assets: list) -> list:
-    """
-    https://api.koios.rest/#post-/asset_info
-    Get the information of a list of assets including first minting & token registry metadata
-    :param assets: Asset list in the format [policy.name_hex]
-    :returns: List of maps with the assets including first minting & token registry metadata
-    """
-    url = API_BASE_URL + '/asset_info'
-    headers = {'Accept': 'application/json', 'Content-Type': 'application/json'}
-    parameters = {'_asset_list': []}
-    for asset in assets:
-        asset_split = asset.split('.')
-        parameters['_asset_list'].append([asset_split[0], asset_split[1]])
-    while True:
-        try:
-            resp = json.loads(requests.post(url, headers=headers, data=json.dumps(parameters)).text)
-            break
-        except Exception as e:
-            print(f"Exception in {inspect.getframeinfo(inspect.currentframe()).function}: {e}")
+            print('Exception in %s: %s' % (inspect.getframeinfo(inspect.currentframe()).function, e))
             sleep(SLEEP_TIME)
             print('retrying...')
     return resp
 
 
-def get_asset_history(policy: str, name: str = '') -> list:
+def get_asset_history(policy, name=''):
     """
     https://api.koios.rest/#get-/asset_history
     Get the mint/burn history of an asset
     :param policy: Asset Policy
     :param name: Asset Name in hexadecimal format (optional), default: all policy assets
     :returns: List of maps with the mint/burn history of an asset
     """
@@ -231,98 +147,56 @@
         if offset > 0:
             parameters['offset'] = offset
         while True:
             try:
                 resp = json.loads(requests.get(url, params=parameters).text)
                 break
             except Exception as e:
-                print(f"Exception in {inspect.getframeinfo(inspect.currentframe()).function}: {e}")
+                print('Exception in %s: %s' % (inspect.getframeinfo(inspect.currentframe()).function, e))
                 sleep(SLEEP_TIME)
                 print('retrying...')
         assets += resp
-        if len(resp) < API_RESP_COUNT:
+        if len(resp) < 1000:
             break
         else:
             offset += len(resp)
     return assets
 
 
-def get_policy_asset_addresses(policy: str, offset: int = 0, limit: int = 0) -> list:
-    """
-    https://api.koios.rest/#get-/policy_asset_addresses
-    Get the list of addresses with quantity for each asset on the given policy
-    :param policy: Asset Policy
-    :param offset: The offset to start from (optional)
-    :param limit: The maximum number of accounts to return (optional)
-    :returns: List of maps with addresses and quantity for each asset on the given policy
-    """
-    url = API_BASE_URL + '/policy_asset_addresses'
-    parameters = {'_asset_policy': policy}
-    asset_addresses = []
-    while True:
-        if offset > 0:
-            parameters['offset'] = offset
-        while True:
-            try:
-                resp = json.loads(requests.get(url, params=parameters).text)
-                break
-            except Exception as e:
-                print(f"Exception in {inspect.getframeinfo(inspect.currentframe()).function}: {e}")
-                sleep(SLEEP_TIME)
-                print('retrying...')
-        asset_addresses += resp
-        if len(resp) < API_RESP_COUNT:
-            if 0 < limit <= len(asset_addresses):
-                asset_addresses = asset_addresses[0:limit]
-            break
-        else:
-            offset += len(resp)
-        if 0 < limit <= len(asset_addresses):
-            asset_addresses = asset_addresses[0:limit]
-            break
-    return asset_addresses
-
-
-def get_policy_asset_info(policy: str, offset: int = 0, limit: int = 0) -> list:
+def get_policy_asset_info(policy):
     """
     https://api.koios.rest/#get-/policy_asset_info
     Get the information for all assets under the same policy
     :param policy: Asset Policy
-    :param offset: The offset to start from (optional)
-    :param limit: The maximum number of accounts to return (optional)
     :returns: List of maps with the policy assets
     """
     url = API_BASE_URL + '/policy_asset_info'
     parameters = {'_asset_policy': policy}
     assets = []
+    offset = 0
     while True:
         if offset > 0:
             parameters['offset'] = offset
         while True:
             try:
                 resp = json.loads(requests.get(url, params=parameters).text)
                 break
             except Exception as e:
-                print(f"Exception in {inspect.getframeinfo(inspect.currentframe()).function}: {e}")
+                print('Exception in %s: %s' % (inspect.getframeinfo(inspect.currentframe()).function, e))
                 sleep(SLEEP_TIME)
                 print('retrying...')
         assets += resp
-        if len(resp) < API_RESP_COUNT:
-            if 0 < limit <= len(assets):
-                assets = assets[0:limit]
+        if len(resp) < 1000:
             break
         else:
             offset += len(resp)
-        if 0 < limit <= len(assets):
-            assets = assets[0:limit]
-            break
     return assets
 
 
-def get_asset_policy_info(policy: str) -> list:
+def get_asset_policy_info(policy):
     """
     DEPRECATED
     https://api.koios.rest/#get-/asset_policy_info
     Get the information for all assets under the same policy
     :param policy: Asset Policy
     :returns: List of maps with the policy assets
     """
@@ -332,110 +206,77 @@
     while True:
         paginated_url = url + '&offset=%d' % offset
         while True:
             try:
                 resp = json.loads(requests.get(paginated_url).text)
                 break
             except Exception as e:
-                print(f"Exception in {inspect.getframeinfo(inspect.currentframe()).function}: {e}")
-                sleep(SLEEP_TIME)
-                print('retrying...')
-        assets += resp
-        if len(resp) < API_RESP_COUNT:
-            break
-        else:
-            offset += len(resp)
-    return assets
-
-
-def get_policy_asset_list(policy: str, offset: int = 0, limit: int = 0) -> list:
-    """
-    https://api.koios.rest/#get-/policy_asset_list
-    Get the list of asset under the given policy (including balances)
-    :param policy: Asset Policy
-    :param offset: The offset to start from (optional)
-    :param limit: The maximum number of accounts to return (optional)
-    :returns: List of maps with the policy assets
-    """
-    url = API_BASE_URL + '/policy_asset_info'
-    parameters = {'_asset_policy': policy}
-    assets = []
-    while True:
-        if offset > 0:
-            parameters['offset'] = offset
-        while True:
-            try:
-                resp = json.loads(requests.get(url, params=parameters).text)
-                break
-            except Exception as e:
-                print(f"Exception in {inspect.getframeinfo(inspect.currentframe()).function}: {e}")
+                print('Exception in %s: %s' % (inspect.getframeinfo(inspect.currentframe()).function, e))
                 sleep(SLEEP_TIME)
                 print('retrying...')
         assets += resp
-        if len(resp) < API_RESP_COUNT:
-            if 0 < limit <= len(assets):
-                assets = assets[0:limit]
+        if len(resp) < 1000:
             break
         else:
             offset += len(resp)
-        if 0 < limit <= len(assets):
-            assets = assets[0:limit]
-            break
     return assets
 
 
-def get_asset_summary(policy: str, name: str = '') -> list:
+def get_asset_summary(policy, name=''):
     """
     Get the summary of an asset (total transactions exclude minting/total wallets
     include only wallets with asset balance)
     :param policy: Asset Policy
     :param name: Asset Name in hexadecimal format (optional), default: all policy assets
     :returns: List of maps with the mint/burn history of an asset
     """
     url = API_BASE_URL + '/asset_summary'
-    parameters = {'_asset_policy': policy, '_asset_name': name}
+    parameters = {'_asset_policy': policy}
+    if isinstance(name, str) and name != '':
+        parameters['_asset_name'] = name
     while True:
         try:
             resp = json.loads(requests.get(url, params=parameters).text)
             break
         except Exception as e:
-            print(f"Exception in {inspect.getframeinfo(inspect.currentframe()).function}: {e}")
+            print('Exception in %s: %s' % (inspect.getframeinfo(inspect.currentframe()).function, e))
             sleep(SLEEP_TIME)
             print('retrying...')
     return resp
 
 
-def get_asset_txs(policy: str, name: str = '', block: int = 0, history: bool = False) -> list:
+def get_asset_txs(policy, name='', block=0, history=False):
     """
     Get the list of all asset transaction hashes (the newest first)
     :param policy: Asset Policy
     :param name: Asset Name in hexadecimal format (optional), default: all policy assets
     :param block: (optional) Return only the transactions after this block
     :param history: (optional) Include all historical transactions, setting to false includes only the non-empty ones
     :returns: List of maps with the mint/burn history of an asset
     """
     url = API_BASE_URL + '/asset_txs'
-    parameters = {
-        '_asset_policy': policy,
-        '_asset_name': name,
-        '_after_block_height': block,
-        '_history': str(history).lower()
-    }
+    parameters = {'_asset_policy': policy}
+    if isinstance(name, str) and name != '':
+        parameters['_asset_name'] = name
+    if isinstance(block, int) and block > 0:
+        parameters['_after_block_height'] = block
+    if isinstance(history, bool):
+        parameters['_history'] = str(history).lower()
     assets_txs = []
     offset = 0
     while True:
         if offset > 0:
             parameters['offset'] = offset
         while True:
             try:
                 resp = json.loads(requests.get(url, params=parameters).text)
                 break
             except Exception as e:
-                print(f"Exception in {inspect.getframeinfo(inspect.currentframe()).function}: {e}")
+                print('Exception in %s: %s' % (inspect.getframeinfo(inspect.currentframe()).function, e))
                 sleep(SLEEP_TIME)
                 print('retrying...')
         assets_txs += resp
-        if len(resp) < API_RESP_COUNT:
+        if len(resp) < 1000:
             break
         else:
             offset += len(resp)
     return assets_txs
```

### Comparing `koios-api-1.0.10/src/koios_api/block.py` & `koios-api-1.0.2/src/koios_api/block.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import json
 import requests
 import inspect
 from time import sleep
 from .__config__ import *
 
 
-def get_blocks(limit: int = 0) -> list:
+def get_blocks(limit=0):
     """
     https://api.koios.rest/#get-/blocks
     Get summarised details about all blocks (paginated - latest first)
     :param limit: the limit of the returned blocks number
     :returns: The list of block maps (the newest first)
     """
     url = API_BASE_URL + '/blocks'
@@ -22,33 +22,32 @@
         if isinstance(limit, int) and limit > 0:
             parameters['limit'] = limit
         while True:
             try:
                 resp = json.loads(requests.get(url, params=parameters).text)
                 break
             except Exception as e:
-                print(f"Exception in {inspect.getframeinfo(inspect.currentframe()).function}: {e}")
+                print('Exception in %s: %s' % (inspect.getframeinfo(inspect.currentframe()).function, e))
                 sleep(SLEEP_TIME)
                 print('retrying...')
         blocks += resp
-        if len(resp) < API_RESP_COUNT:
+        if len(resp) < 1000:
             break
         else:
             offset += len(resp)
         if isinstance(limit, int) and len(blocks) > limit:
             break
     if isinstance(limit, int) and limit > 0:
         return blocks[0:limit]
     else:
         return blocks
 
 
-def get_block_info(block: [str, list]) -> list:
+def get_block_info(block):
     """
-    https://api.koios.rest/#post-/block_info
     Get detailed information about a specific block
     :param block: Block hash as string (for one block) or list of block hashes (for multiple blocks)
     :returns: The list of block maps
     """
     url = API_BASE_URL + '/block_info'
     headers = {'Accept': 'application/json', 'Content-Type': 'application/json'}
     block_hashes = {}
@@ -57,21 +56,21 @@
     else:
         block_hashes['_block_hashes'] = [block]
     while True:
         try:
             resp = json.loads(requests.post(url, headers=headers, data=json.dumps(block_hashes)).text)
             break
         except Exception as e:
-            print(f"Exception in {inspect.getframeinfo(inspect.currentframe()).function}: {e}")
+            print('Exception in %s: %s' % (inspect.getframeinfo(inspect.currentframe()).function, e))
             sleep(SLEEP_TIME)
             print('retrying...')
     return resp
 
 
-def get_block_txs(block: [str, list]) -> list:
+def get_block_txs(block):
     """
     https://api.koios.rest/#post-/block_txs
     Get a list of all transactions included in provided blocks
     :param block: Block hash as string (for one block) or list of block hashes (for multiple blocks)
     :returns: The list of transaction maps by block
     """
     url = API_BASE_URL + '/block_txs'
@@ -82,11 +81,11 @@
     else:
         block_hashes['_block_hashes'] = [block]
     while True:
         try:
             resp = json.loads(requests.post(url, headers=headers, data=json.dumps(block_hashes)).text)
             break
         except Exception as e:
-            print(f"Exception in {inspect.getframeinfo(inspect.currentframe()).function}: {e}")
+            print('Exception in %s: %s' % (inspect.getframeinfo(inspect.currentframe()).function, e))
             sleep(SLEEP_TIME)
             print('retrying...')
     return resp
```

### Comparing `koios-api-1.0.10/src/koios_api/network.py` & `koios-api-1.0.2/src/koios_api/network.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,51 +1,51 @@
 import json
 import requests
 import inspect
 from time import sleep
 from .__config__ import *
 
 
-def get_tip() -> list:
+def get_tip():
     """
     https://api.koios.rest/#get-/tip
     Get the tip info about the latest block seen by chain
     :returns: A list with the tip as a map
     """
     url = API_BASE_URL + '/tip'
     while True:
         try:
             resp = json.loads(requests.get(url).text)
             break
         except Exception as e:
-            print(f"Exception in {inspect.getframeinfo(inspect.currentframe()).function}: {e}")
+            print('Exception in %s: %s' % (inspect.getframeinfo(inspect.currentframe()).function, e))
             sleep(SLEEP_TIME)
             print('retrying...')
     return resp
 
 
-def get_genesis() -> list:
+def get_genesis():
     """
     https://api.koios.rest/#get-/genesis
     Get the Genesis parameters used to start specific era on chain
     :returns: A list with the genesis parameters map
     """
     url = API_BASE_URL + '/genesis'
     while True:
         try:
             resp = json.loads(requests.get(url).text)
             break
         except Exception as e:
-            print(f"Exception in {inspect.getframeinfo(inspect.currentframe()).function}: {e}")
+            print('Exception in %s: %s' % (inspect.getframeinfo(inspect.currentframe()).function, e))
             sleep(SLEEP_TIME)
             print('retrying...')
     return resp
 
 
-def get_totals(epoch: int = 0) -> list:
+def get_totals(epoch=0):
     """
     https://api.koios.rest/#get-/totals
     Get the circulating utxo, treasury, rewards, supply and reserves in lovelace
     for specified epoch, all epochs if empty
     :param epoch: (Optional) The epoch
     :returns: The list of tokenomic stats maps
     """
@@ -54,29 +54,11 @@
     if isinstance(epoch, int) and epoch > 0:
         parameters['_epoch_no'] = epoch
     while True:
         try:
             resp = json.loads(requests.get(url, params=parameters).text)
             break
         except Exception as e:
-            print(f"Exception in {inspect.getframeinfo(inspect.currentframe()).function}: {e}")
-            sleep(SLEEP_TIME)
-            print('retrying...')
-    return resp
-
-
-def get_param_updates() -> list:
-    """
-    https://api.koios.rest/#get-/param_updates
-    Get all parameter update proposals submitted to the chain starting Shelley era
-    :returns: A list with the parameters updates
-    """
-    url = API_BASE_URL + '/param_updates'
-    while True:
-        try:
-            resp = json.loads(requests.get(url).text)
-            break
-        except Exception as e:
-            print(f"Exception in {inspect.getframeinfo(inspect.currentframe()).function}: {e}")
+            print('Exception in %s: %s' % (inspect.getframeinfo(inspect.currentframe()).function, e))
             sleep(SLEEP_TIME)
             print('retrying...')
     return resp
```

### Comparing `koios-api-1.0.10/src/koios_api/pool.py` & `koios-api-1.0.2/src/koios_api/pool.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import json
 import requests
 import inspect
 from time import sleep
 from .__config__ import *
 
 
-def get_pools_list() -> list:
+def get_pools_list():
     """
     https://api.koios.rest/#get-/pool_list
     A list of all currently registered/retiring (not retired) pools
     :returns: The list of stake pool maps
     """
     url = API_BASE_URL + '/pool_list'
     headers = {'Accept': 'application/json', 'Content-Type': 'application/json'}
@@ -20,26 +20,26 @@
         if offset > 0:
             parameters['offset'] = offset
         while True:
             try:
                 resp = json.loads(requests.get(url, headers=headers, params=parameters).text)
                 break
             except Exception as e:
-                print(f"Exception in {inspect.getframeinfo(inspect.currentframe()).function}: {e}")
+                print('Exception in %s: %s' % (inspect.getframeinfo(inspect.currentframe()).function, e))
                 sleep(SLEEP_TIME)
                 print('retrying...')
         pools_list += resp
-        if len(resp) < API_RESP_COUNT:
+        if len(resp) < 1000:
             break
         else:
             offset += len(resp)
     return pools_list
 
 
-def get_pool_info(pool_id: [str, list]) -> list:
+def get_pool_info(pool_id):
     """
     https://api.koios.rest/#post-/pool_info
     Current pool statuses and details for a specified list of pool ids
     :param pool_id: Stake pool bech32 ID as string (for one stake pool)
     or list of stake pool bech32 IDs (for multiple stake pools)
     :returns: pool_info
     """
@@ -51,41 +51,41 @@
     else:
         pool_ids['_pool_bech32_ids'] = [pool_id]
     while True:
         try:
             resp = json.loads(requests.post(url, headers=headers, data=json.dumps(pool_ids)).text)
             break
         except Exception as e:
-            print(f"Exception in {inspect.getframeinfo(inspect.currentframe()).function}: {e}")
+            print('Exception in %s: %s' % (inspect.getframeinfo(inspect.currentframe()).function, e))
             sleep(SLEEP_TIME)
             print('retrying...')
     return resp
 
 
-def get_pool_stake_snapshot(pool_id: str) -> list:
+def get_pool_stake_snapshot(pool_id):
     """
     https://api.koios.rest/#get-/pool_stake_snapshot
     Returns Mark, Set and Go stake snapshots for the selected pool, useful for leaderlog calculation
     :param pool_id: stake pool bech32 id
     :returns: Pool snapshot as list of maps by epoch (current and previous 2)
     """
     url = API_BASE_URL + '/pool_stake_snapshot'
     parameters = {'_pool_bech32': pool_id}
     while True:
         try:
             resp = json.loads(requests.get(url, params=parameters).text)
             break
         except Exception as e:
-            print(f"Exception in {inspect.getframeinfo(inspect.currentframe()).function}: {e}")
+            print('Exception in %s: %s' % (inspect.getframeinfo(inspect.currentframe()).function, e))
             sleep(SLEEP_TIME)
             print('retrying...')
     return resp
 
 
-def get_pool_delegators(pool_id: str) -> list:
+def get_pool_delegators(pool_id):
     """
     https://api.koios.rest/#get-/pool_delegators
     Return information about live delegators for a given pool.
     :param pool_id: stake pool bech32 id
     :returns: The list of pool delegators maps
     """
     url = API_BASE_URL + '/pool_delegators'
@@ -96,26 +96,26 @@
         if offset > 0:
             parameters['offset'] = offset
         while True:
             try:
                 resp = json.loads(requests.get(url, params=parameters).text)
                 break
             except Exception as e:
-                print(f"Exception in {inspect.getframeinfo(inspect.currentframe()).function}: {e}")
+                print('Exception in %s: %s' % (inspect.getframeinfo(inspect.currentframe()).function, e))
                 sleep(SLEEP_TIME)
                 print('retrying...')
         delegators += resp
-        if len(resp) < API_RESP_COUNT:
+        if len(resp) < 1000:
             break
         else:
             offset += len(resp)
     return delegators
 
 
-def get_pool_delegators_history(pool_id: str, epoch: int = 0) -> list:
+def get_pool_delegators_history(pool_id, epoch=0):
     """
     https://api.koios.rest/#get-/pool_delegators_history
     Return information about active delegators (incl. history) for a given pool and epoch number
     (all epochs if not specified).
     :param pool_id: stake pool bech32 id
     :param epoch: (optional) epoch
     :returns: The list of pool delegators maps
@@ -130,26 +130,26 @@
         if offset > 0:
             parameters['offset'] = offset
         while True:
             try:
                 resp = json.loads(requests.get(url, params=parameters).text)
                 break
             except Exception as e:
-                print(f"Exception in {inspect.getframeinfo(inspect.currentframe()).function}: {e}")
+                print('Exception in %s: %s' % (inspect.getframeinfo(inspect.currentframe()).function, e))
                 sleep(SLEEP_TIME)
                 print('retrying...')
         delegators += resp
-        if len(resp) < API_RESP_COUNT:
+        if len(resp) < 1000:
             break
         else:
             offset += len(resp)
     return delegators
 
 
-def get_pool_blocks(pool_id: str, epoch: int = 0) -> list:
+def get_pool_blocks(pool_id, epoch=0):
     """
     https://api.koios.rest/#get-/pool_blocks
     Return information about blocks minted by a given pool for all epochs (or _epoch_no if provided)
     :param pool_id: stake pool bech32 id
     :param epoch: (optional) epoch
     :returns: The list of pool blocks maps
     """
@@ -163,26 +163,26 @@
         if offset > 0:
             parameters['offset'] = offset
         while True:
             try:
                 resp = json.loads(requests.get(url, params=parameters).text)
                 break
             except Exception as e:
-                print(f"Exception in {inspect.getframeinfo(inspect.currentframe()).function}: {e}")
+                print('Exception in %s: %s' % (inspect.getframeinfo(inspect.currentframe()).function, e))
                 sleep(SLEEP_TIME)
                 print('retrying...')
         blocks += resp
-        if len(resp) < API_RESP_COUNT:
+        if len(resp) < 1000:
             break
         else:
             offset += len(resp)
     return blocks
 
 
-def get_pool_history(pool_id: str, epoch: int = 0) -> list:
+def get_pool_history(pool_id, epoch=0):
     """
     https://api.koios.rest/#get-/pool_history
     Return information about pool stake, block and reward history in a given epoch _epoch_no
     (or all epochs that pool existed for, in descending order if no _epoch_no was provided)
     :param pool_id: stake pool bech32 id
     :param epoch: (optional) epoch
     :returns: pool_history
@@ -192,53 +192,53 @@
     if isinstance(epoch, int) and epoch > 0:
         parameters['_epoch_no'] = epoch
     while True:
         try:
             resp = json.loads(requests.get(url, params=parameters).text)
             break
         except Exception as e:
-            print(f"Exception in {inspect.getframeinfo(inspect.currentframe()).function}: {e}")
+            print('Exception in %s: %s' % (inspect.getframeinfo(inspect.currentframe()).function, e))
             sleep(SLEEP_TIME)
             print('retrying...')
     return resp
 
 
-def get_pool_updates(pool_id: str = '') -> list:
+def get_pool_updates(pool_id=''):
     """
     https://api.koios.rest/#get-/pool_updates
     Return all pool updates for all pools or only updates for specific pool if specified
     :param pool_id: stake pool bech32 id
     :returns: pool_updates
     """
     url = API_BASE_URL + '/pool_updates'
     parameters = {}
     pool_updates = []
     offset = 0
-    if pool_id:
-        parameters['_pool_bech32'] = pool_id
     while True:
+        if pool_id:
+            parameters['_pool_bech32'] = pool_id
         if offset > 0:
             parameters['offset'] = offset
         while True:
             try:
                 resp = json.loads(requests.get(url, params=parameters).text)
                 break
             except Exception as e:
-                print(f"Exception in {inspect.getframeinfo(inspect.currentframe()).function}: {e}")
+                print('Exception in %s: %s' % (inspect.getframeinfo(inspect.currentframe()).function, e))
                 sleep(SLEEP_TIME)
                 print('retrying...')
         pool_updates += resp
-        if len(resp) < API_RESP_COUNT:
+        if len(resp) < 1000:
             break
         else:
             offset += len(resp)
     return pool_updates
 
 
-def get_pool_relays() -> list:
+def get_pool_relays():
     """
     https://api.koios.rest/#get-/pool_relays
     A list of registered relays for all currently registered/retiring (not retired) pools
     :returns: The list of relays maps by stake pool
     """
     url = API_BASE_URL + '/pool_relays'
     parameters = {}
@@ -248,28 +248,28 @@
         if offset > 0:
             parameters['offset'] = offset
         while True:
             try:
                 resp = json.loads(requests.get(url, params=parameters).text)
                 break
             except Exception as e:
-                print(f"Exception in {inspect.getframeinfo(inspect.currentframe()).function}: {e}")
+                print('Exception in %s: %s' % (inspect.getframeinfo(inspect.currentframe()).function, e))
                 sleep(SLEEP_TIME)
                 print('retrying...')
         relays += resp
-        if len(resp) < API_RESP_COUNT:
+        if len(resp) < 1000:
             break
         else:
             offset += len(resp)
     return relays
 
 
-def get_pool_metadata(pool_id: str) -> list:
+def get_pool_metadata(pool_id):
     """
-    https://api.koios.rest/#post-/pool_metadata
+    https://api.koios.rest/#get-/pool_relays
     A list of registered relays for all currently registered/retiring (not retired) pools
     :param pool_id: stake pool bech32 id
     :returns: The list of pool metadata maps
     """
     url = API_BASE_URL + '/pool_metadata'
     headers = {'Accept': 'application/json', 'Content-Type': 'application/json'}
     pool_ids = {}
@@ -278,30 +278,30 @@
     else:
         pool_ids['_pool_bech32_ids'] = [pool_id]
     while True:
         try:
             resp = json.loads(requests.post(url, headers=headers, data=json.dumps(pool_ids)).text)
             break
         except Exception as e:
-            print(f"Exception in {inspect.getframeinfo(inspect.currentframe()).function}: {e}")
+            print('Exception in %s: %s' % (inspect.getframeinfo(inspect.currentframe()).function, e))
             sleep(SLEEP_TIME)
             print('retrying...')
     return resp
 
 
-def get_retiring_pools() -> list:
+def get_retiring_pools():
     """
     Get the retiring stake pools list
     :returns: The list of retiring pools maps
     """
     headers = {'Accept': 'application/json', 'Content-Type': 'application/json'}
     url = API_BASE_URL + '/pool_updates'
     parameters = {'pool_status': 'eq.retiring'}
     while True:
         try:
             resp = json.loads(requests.get(url, headers=headers, params=parameters).text)
             break
         except Exception as e:
-            print(f"Exception in {inspect.getframeinfo(inspect.currentframe()).function}: {e}")
+            print('Exception in %s: %s' % (inspect.getframeinfo(inspect.currentframe()).function, e))
             sleep(SLEEP_TIME)
             print('retrying...')
     return resp
```

### Comparing `koios-api-1.0.10/src/koios_api/script.py` & `koios-api-1.0.2/src/koios_api/script.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import json
 import requests
 import inspect
 from time import sleep
 from .__config__ import *
 
 
-def get_native_script_list() -> list:
+def get_native_script_list():
     """
     https://api.koios.rest/#get-/native_script_list
     List of all existing native script hashes along with their creation transaction hashes
     :returns: The list of all native scripts maps
     """
     url = API_BASE_URL + '/native_script_list'
     parameters = {}
@@ -19,26 +19,26 @@
         if offset > 0:
             parameters['offset'] = offset
         while True:
             try:
                 resp = json.loads(requests.get(url, params=parameters).text)
                 break
             except Exception as e:
-                print(f"Exception in {inspect.getframeinfo(inspect.currentframe()).function}: {e}")
+                print('Exception in %s: %s' % (inspect.getframeinfo(inspect.currentframe()).function, e))
                 sleep(SLEEP_TIME)
                 print('Offset %d, retrying...' % offset)
         scripts_list += resp
-        if len(resp) < API_RESP_COUNT:
+        if len(resp) < 1000:
             break
         else:
             offset += len(resp)
     return scripts_list
 
 
-def get_plutus_script_list() -> list:
+def get_plutus_script_list():
     """
     https://api.koios.rest/#get-/plutus_script_list
     List of all existing native script hashes along with their creation transaction hashes
     :returns: The list of all plutus scripts maps
     """
     url = API_BASE_URL + '/plutus_script_list'
     parameters = {}
@@ -48,46 +48,46 @@
         if offset > 0:
             parameters['offset'] = offset
         while True:
             try:
                 resp = json.loads(requests.get(url, params=parameters).text)
                 break
             except Exception as e:
-                print(f"Exception in {inspect.getframeinfo(inspect.currentframe()).function}: {e}")
+                print('Exception in %s: %s' % (inspect.getframeinfo(inspect.currentframe()).function, e))
                 sleep(SLEEP_TIME)
                 print('Offset %d, retrying...' % offset)
         scripts_list += resp
-        if len(resp) < API_RESP_COUNT:
+        if len(resp) < 1000:
             break
         else:
             offset += len(resp)
     return scripts_list
 
 
-def get_script_redeemers(script: str) -> list:
+def get_script_redeemers(script):
     """
     https://api.koios.rest/#get-/script_redeemers
     List of all redeemers for a given script hash
     :param script: script hash
     :returns resp: redeemers list as map
     """
     url = API_BASE_URL + '/script_redeemers'
     parameters = {'_script_hash':  script}
     while True:
         try:
             resp = json.loads(requests.get(url, params=parameters).text)
             break
         except Exception as e:
-            print(f"Exception in {inspect.getframeinfo(inspect.currentframe()).function}: {e}")
+            print('Exception in %s: %s' % (inspect.getframeinfo(inspect.currentframe()).function, e))
             sleep(SLEEP_TIME)
             print('retrying...')
     return resp
 
 
-def get_datum_info(datum: [str, list]) -> list:
+def get_datum_info(datum):
     """
     https://api.koios.rest/#post-/datum_info
     List of datum information for given datum hashes
     :param datum: datum hash as string (for one datum hash) or list (for a list of datum hashes)
     :returns resp: datum information as list of maps
     """
     url = API_BASE_URL + '/datum_info'
@@ -98,11 +98,11 @@
     else:
         datum_hashes['_datum_hashes'] = [datum]
     while True:
         try:
             resp = json.loads(requests.post(url, headers=headers, data=json.dumps(datum_hashes)).text)
             break
         except Exception as e:
-            print(f"Exception in {inspect.getframeinfo(inspect.currentframe()).function}: {e}")
+            print('Exception in %s: %s' % (inspect.getframeinfo(inspect.currentframe()).function, e))
             sleep(SLEEP_TIME)
             print('retrying...')
     return resp
```

### Comparing `koios-api-1.0.10/src/koios_api/transactions.py` & `koios-api-1.0.2/src/koios_api/transactions.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import json
 import requests
 import inspect
 from time import sleep
 from .__config__ import *
 
 
-def get_tx_info(txs: [str, list]) -> list:
+def get_tx_info(txs):
     """
     https://api.koios.rest/#post-/tx_info
     Get detailed information about transaction(s)
     :param txs: transaction hash as a string (for one transaction) or list (for multiple transactions)
     :returns: The list of transactions details maps
     """
     url = API_BASE_URL + '/tx_info'
@@ -20,21 +20,21 @@
     else:
         tx_hashes['_tx_hashes'] = [txs]
     while True:
         try:
             resp = json.loads(requests.post(url, headers=headers, data=json.dumps(tx_hashes)).text)
             break
         except Exception as e:
-            print(f"Exception in {inspect.getframeinfo(inspect.currentframe()).function}: {e}")
+            print('Exception in %s: %s' % (inspect.getframeinfo(inspect.currentframe()).function, e))
             sleep(SLEEP_TIME)
             print('retrying...')
     return resp
 
 
-def get_tx_utxos(txs: [str, list]) -> list:
+def get_tx_utxos(txs):
     """
     https://api.koios.rest/#post-/tx_utxos
     Get UTxO set (inputs/outputs) of transactions.
     :param txs: transaction hash as a string (for one transaction) or list (for multiple transactions)
     :returns: The list of transactions UTxOs maps
     """
     url = API_BASE_URL + '/tx_utxos'
@@ -45,21 +45,21 @@
     else:
         tx_hashes['_tx_hashes'] = [txs]
     while True:
         try:
             resp = json.loads(requests.post(url, headers=headers, data=json.dumps(tx_hashes)).text)
             break
         except Exception as e:
-            print(f"Exception in {inspect.getframeinfo(inspect.currentframe()).function}: {e}")
+            print('Exception in %s: %s' % (inspect.getframeinfo(inspect.currentframe()).function, e))
             sleep(SLEEP_TIME)
             print('retrying...')
     return resp
 
 
-def get_tx_metadata(txs: [str, list]) -> list:
+def get_tx_metadata(txs):
     """
     https://api.koios.rest/#post-/tx_metadata
     Get metadata information (if any) for given transaction(s)
     :param txs: transaction hash as a string (for one transaction) or list (for multiple transactions)
     :returns: The list of transactions metadata maps
     """
     url = API_BASE_URL + '/tx_metadata'
@@ -70,21 +70,21 @@
     else:
         tx_hashes['_tx_hashes'] = [txs]
     while True:
         try:
             resp = json.loads(requests.post(url, headers=headers, data=json.dumps(tx_hashes)).text)
             break
         except Exception as e:
-            print(f"Exception in {inspect.getframeinfo(inspect.currentframe()).function}: {e}")
+            print('Exception in %s: %s' % (inspect.getframeinfo(inspect.currentframe()).function, e))
             sleep(SLEEP_TIME)
             print('retrying...')
     return resp
 
 
-def get_tx_metalabels() -> list:
+def get_tx_metalabels():
     """
     https://api.koios.rest/#get-/tx_metalabels
     Get a list of all transaction metadata labels
     :returns: The list of transaction metadata labels maps
     """
     url = API_BASE_URL + '/tx_metalabels'
     parameters = {}
@@ -94,46 +94,46 @@
         if offset > 0:
             parameters['offset'] = offset
         while True:
             try:
                 resp = json.loads(requests.get(url, params=parameters).text)
                 break
             except Exception as e:
-                print(f"Exception in {inspect.getframeinfo(inspect.currentframe()).function}: {e}")
+                print('Exception in %s: %s' % (inspect.getframeinfo(inspect.currentframe()).function, e))
                 sleep(SLEEP_TIME)
-                print(f"Offset {offset}, retrying...")
+                print('Offset %d, retrying...' % offset)
         metalabels_list += resp
-        if len(resp) < API_RESP_COUNT:
+        if len(resp) < 1000:
             break
         else:
             offset += len(resp)
     return metalabels_list
 
 
-def submit_tx(tx: str) -> str:
+def submit_tx(tx):
     """
     https://api.koios.rest/#post-/submittx
     Submit an already serialized transaction to the network.
     :param tx: transaction in cbor format
     :returns: transaction hash
     """
     url = API_BASE_URL + '/submittx'
     headers = {'Accept': 'application/json', 'Content-Type': 'application/cbor'}
     while True:
         try:
             resp = json.loads(requests.post(url, headers=headers, data=tx).text)
             break
         except Exception as e:
-            print(f"Exception in {inspect.getframeinfo(inspect.currentframe()).function}: {e}")
+            print('Exception in %s: %s' % (inspect.getframeinfo(inspect.currentframe()).function, e))
             sleep(SLEEP_TIME)
             print('retrying...')
     return resp
 
 
-def get_tx_status(txs: [str, list]) -> list:
+def get_tx_status(txs):
     """
     https://api.koios.rest/#post-/tx_status
     Get the number of block confirmations for a given transaction hash list
     :param txs: transaction hash as a string (for one transaction) or list (for multiple transactions)
     :returns: The list of transactions block confirmations maps
     """
     url = API_BASE_URL + '/tx_status'
@@ -144,11 +144,11 @@
     else:
         tx_hashes['_tx_hashes'] = [txs]
     while True:
         try:
             resp = json.loads(requests.post(url, headers=headers, data=json.dumps(tx_hashes)).text)
             break
         except Exception as e:
-            print(f"Exception in {inspect.getframeinfo(inspect.currentframe()).function}: {e}")
+            print('Exception in %s: %s' % (inspect.getframeinfo(inspect.currentframe()).function, e))
             sleep(SLEEP_TIME)
             print('retrying...')
     return resp
```

### Comparing `koios-api-1.0.10/src/koios_api.egg-info/PKG-INFO` & `koios-api-1.0.2/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,22 +1,7 @@
-Metadata-Version: 2.1
-Name: koios-api
-Version: 1.0.10
-Summary: A python package for the Cardano Blockchain Koios API (https://api.koios.rest/)
-Author-email: APEX Stake Pool <cardanoapexpool@gmail.com>
-Project-URL: Homepage, https://github.com/cardano-apexpool/koios-api-python
-Project-URL: Bug Tracker, https://github.com/cardano-apexpool/koios-api-python/issues
-Keywords: koios,cardano,blockchain,REST,API
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.7
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 # koios-api-python
 A python package for the Cardano Blockchain Koios API (https://api.koios.rest/)
 
 ## Install
 To install the module, type the following command:
 ```bash
 pip3 install koios_api
@@ -69,15 +54,14 @@
 
 ## Modules
 
 [Network](#Network)<br>
 [get_tip](#get_tip) Get the tip info about the latest block seen by chain<br>
 [get_genesis](#get_genesis) Get the Genesis parameters used to start specific era on chain<br>
 [get_totals](#get_totals) Get the circulating utxo, treasury, rewards, supply and reserves in lovelace for specified epoch, all epochs if empty<br>
-[get_param_updates](#get_param_updates) Get all parameter update proposals submitted to the chain starting Shelley era<br>
 
 [Epoch](#Epoch)<br>
 [get_epoch_info](#get_epoch_info) Get the epoch information, all epochs if no epoch specified<br>
 [get_epoch_params](#get_epoch_params) Get the protocol parameters for specific epoch, returns information about all epochs if no epoch specified<br>
 [get_epoch_block_protocols](#get_epoch_block_protocols) Get the information about block protocol distribution in epoch<br>
 
 [Block](#Block)<br>
@@ -92,29 +76,33 @@
 [get_tx_metalabels](#get_tx_metalabels) Get a list of all transaction metadata labels<br>
 [submit_tx](#submit_tx) Submit an already serialized transaction to the network<br>
 [get_tx_status](#get_tx_status) Get the number of block confirmations for a given transaction hash list<br>
 
 [Address](#Address)<br>
 [get_address_info](#get_address_info) Get the transaction hash list of input address array, optionally filtering after specified block height (inclusive)<br>
 [get_address_txs](#get_address_txs) Get the transaction hash list of input address array, optionally filtering after specified block height (inclusive)<br>
-[get_credential_utxos](#get_credential_utxos) Get a list of UTxO against input payment credential array including their balances<br>
 [get_address_assets](#get_address_assets) Get the list of all the assets (policy, name and quantity) for given addresses<br>
 [get_credential_txs](#get_credential_txs) Get the transaction hash list of input payment credential array, optionally filtering after specified block height (inclusive)<br>
 
+[Account](#Account)<br>
+[get_account_list](#get_account_list) Get a list of all accounts<br>
+[get_account_info](#get_account_info) Get the account information for given stake addresses (accounts)<br>
+[get_account_info_cached](#get_account_info_cached) Get the cached account information for given stake addresses (accounts)<br>
+[get_account_rewards](#get_account_rewards) Get the full rewards history (including MIR) for given stake addresses (accounts)<br>
+[get_account_updates](#get_account_updates) Get the account updates (registration, deregistration, delegation and withdrawals) for given stake addresses (accounts)<br>
+[get_account_addresses](#get_account_addresses) Get all addresses associated with given staking accounts<br>
+[get_account_assets](#get_account_assets) Get the native asset balance of given accounts<br>
+[get_account_history](#get_account_history) Get the staking history of given stake addresses (accounts)<br>
+
 [Asset](#Asset)<br>
 [get_asset_list](#get_asset_list) Get the list of all native assets (paginated)<br>
-[get_asset_token_registry](#get_asset_token_registry) Get a list of assets registered via token registry on github<br>
-[get_asset_addresses](#get_asset_addresses) Get the list of all addresses holding a given asset<br>
-[get_asset_nft_address](#get_asset_nft_address) Get the address where specified NFT currently reside on.<br>
+[get_asset_address_list](#get_asset_address_list) Get the list of all addresses holding a given asset<br>
 [get_asset_info](#get_asset_info) Get the information of an asset including first minting & token registry metadata<br>
-[get_asset_info_bulk](#get_asset_info_bulk) Get the information of a list of assets including first minting & token registry metadata<br>
 [get_asset_history](#get_asset_history) Get the mint/burn history of an asset<br>
-[get_policy_asset_addresses](#get_policy_asset_addresses) Get the list of addresses with quantity for each asset on the given policy<br>
-[get_policy_asset_info](#get_policy_asset_info) Get the information for all assets under the same policy<br>
-[get_policy_asset_list](#get_policy_asset_list) Get the list of asset under the given policy (including balances)<br>
+[get_asset_policy_info](#get_asset_policy_info) Get the information for all assets under the same policy<br>
 [get_asset_summary](#get_asset_summary) Get the summary of an asset (total transactions exclude minting/total wallets include only wallets with asset balance)<br>
 [get_asset_txs](#get_asset_txs) Get the list of all asset transaction hashes (the newest first)<br>
 
 [Pool](#Pool)<br>
 [get_pools_list](#get_pools_list) A list of all currently registered/retiring (not retired) pools<br>
 [get_pool_info](#get_pool_info) Current pool statuses and details for a specified list of pool ids<br>
 [get_pool_stake_snapshot](#get_pool_stake_snapshot) Returns Mark, Set and Go stake snapshots for the selected pool, useful for leaderlog calculation<br>
@@ -129,31 +117,20 @@
 
 [Script](#Script)<br>
 [get_native_script_list](#get_native_script_list) The list of all existing native script hashes along with their creation transaction hashes<br>
 [get_plutus_script_list](#get_plutus_script_list) The list of all existing native script hashes along with their creation transaction hashes<br>
 [get_script_redeemers](#get_script_redeemers) The list of all redeemers for a given script hash<br>
 [get_datum_info](#get_datum_info) The list of datum information for given datum hashes<br>
 
-[Stake Account](#Stake Account)<br>
-[get_account_list](#get_account_list) Get a list of all accounts<br>
-[get_account_info](#get_account_info) Get the account information for given stake addresses (accounts)<br>
-[get_account_utxos](#get_account_utxos) Get a list of all UTxOs for a given stake address (account)<br>
-[get_account_info_cached](#get_account_info_cached) Get the cached account information for given stake addresses (accounts)<br>
-[get_account_rewards](#get_account_rewards) Get the full rewards history (including MIR) for given stake addresses (accounts)<br>
-[get_account_updates](#get_account_updates) Get the account updates (registration, deregistration, delegation and withdrawals) for given stake addresses (accounts)<br>
-[get_account_addresses](#get_account_addresses) Get all addresses associated with given staking accounts<br>
-[get_account_assets](#get_account_assets) Get the native asset balance of given accounts<br>
-[get_account_history](#get_account_history) Get the staking history of given stake addresses (accounts)<br>
-
 ### Network
 
 #### get_tip
 Get the tip info about the latest block seen by chain<br>
 Parameters: none<br>
-Returns: The tip information as a list of one dictionary<br>
+Returns: The tip information as a list of one map<br>
 Example:<br>
 `tip = get_tip()`<br>
 Example response:
 ```json
 [
   {
     "hash": "442765ab5660346a6af3ba7667bbd35934e6219a52f0f53a80f28d27a70309c1",
@@ -165,15 +142,15 @@
   }
 ]
 ```
 
 #### get_genesis
 Get the Genesis parameters used to start specific era on chain<br>
 Parameters: none<br>
-Returns: Genesis parameters used to start each era on chain as a list of one dictionary<br>
+Returns: Genesis parameters used to start each era on chain as a list of one map<br>
 Example:<br>
 `genesis = get_genesis()`<br>
 Example response:
 ```json
 [
   {
     "networkmagic": "764824073",
@@ -191,15 +168,15 @@
   }
 ]
 ```
 
 #### get_totals
 Get the circulating utxo, treasury, rewards, supply and reserves in lovelace for specified epoch, all epochs if empty<br>
 Parameters: Epoch (optional)<br>
-Returns: Supply/reserves/utxo/fees/treasury stats as a list of one dictionary (if the epoch is specified) or a list of all available epochs (if the epoch parameter is not specified)<br>
+Returns: Supply/reserves/utxo/fees/treasury stats as a list of one map (if the epoch is specified) or a list of all available epochs (if the epoch parameter is not specified)<br>
 Example:<br>
 `totals = get_totals(380)`<br>
 Example response:
 ```json
 [
   {
     "epoch_no": 380,
@@ -208,50 +185,20 @@
     "reward": "635180192555825",
     "supply": "35230640457275590",
     "reserves": "9769359542724410"
   }
 ]
 ```
 
-#### get_param_updates
-Get all parameter update proposals submitted to the chain starting Shelley era<br>
-Parameters: none<br>
-Returns: All parameter update proposals<br>
-Example:<br>
-`param_updates = get_param_updates()`<br>
-```json
-[
-  {
-    "tx_hash": "b516588da34b58b7d32b6a057f513e16ea8c87de46615631be3316d8a8847d46",
-    "block_height": 4533644,
-    "block_time": 1596923351,
-    "epoch_no": 210,
-    "data": {
-      "decentralisation": 0.9
-    }
-  },
-  {
-    "tx_hash": "784902982af484f78d10f1587072f5a6b888ed0c1296d4ecf1e21c0251696ca1",
-    "block_height": 4558648,
-    "block_time": 1597425824,
-    "epoch_no": 211,
-    "data": {
-      "decentralisation": 0.8
-    }
-  },
-  ...
-]
-```
-
 ### Epoch
 
 #### get_epoch_info
 Get the epoch information, all epochs if no epoch specified<br>
 Parameters: Epoch (optional)<br>
-Returns: The list of epoch info dictionaries<br>
+Returns: The list of epoch info maps<br>
 Example:<br>
 `epoch_info = get_epoch_info(379)`<br>
 Example response:
 ```json
 [
   {
     "epoch_no": 379,
@@ -269,15 +216,15 @@
   }
 ]
 ```
 
 #### get_epoch_params
 Get the protocol parameters for specific epoch, returns information about all epochs if no epoch specified<br>
 Parameters: Epoch (optional)<br>
-Returns: The list of epoch protocol parameters dictionaries<br>
+Returns: The list of epoch protocol parameters maps<br>
 Example:<br>
 `epoch_params = get_epoch_params(380)`<br>
 Example response:
 ```json
 [
   {
     "epoch_no": 380,
@@ -315,15 +262,15 @@
   }
 ]
 ```
 
 #### get_epoch_block_protocols
 Get the information about block protocol distribution in epoch<br>
 Parameters: Epoch (optional)<br>
-Returns: The list of epoch protocol distribution dictionaries<br>
+Returns: The list of epoch protocol distribution maps<br>
 Example:<br>
 `epoch_block_protocols = get_epoch_block_protocols(380)`<br>
 Example response:
 ```json
 [
   {
     "proto_major": 7,
@@ -339,15 +286,15 @@
 ```
 
 ### Block
 
 #### get_blocks
 Get summarised details about all blocks (paginated - latest first)<br>
 Parameters: The maximum number of blocks to return<br>
-Returns: The list of block dictionaries (the newest first)<br>
+Returns: The list of block maps (the newest first)<br>
 Example:<br>
 `blocks = get_blocks(3)`<br>
 Example response:
 ```json
 [
   {
     "hash": "8e33bb588feff6414469779d724923064688615535280f8982c9981410cd06f6",
@@ -396,15 +343,15 @@
   }
 ]
 ```
 
 #### get_block_info
 Get detailed information about a specific block<br>
 Parameters: Block hash as string (for one block) or list of block hashes (for multiple blocks)<br>
-Returns: The list of block dictionaries<br>
+Returns: The list of block maps<br>
 Example:<br>
 `block_info = get_block_info('8e33bb588feff6414469779d724923064688615535280f8982c9981410cd06f6')`<br>
 Example response:
 ```json
 [
   {
     "hash": "8e33bb588feff6414469779d724923064688615535280f8982c9981410cd06f6",
@@ -429,15 +376,15 @@
   }
 ]
 ```
 
 #### get_block_txs
 Get a list of all transactions included in provided blocks<br>
 Parameters: Block(s) hash(es) as string (for one block) or list of block hashes (for multiple blocks)<br>
-Returns: The list of transaction dictionaries by block<br>
+Returns: The list of transaction maps by block<br>
 Example:<br>
 `block_txs = get_block_txs('8e33bb588feff6414469779d724923064688615535280f8982c9981410cd06f6')`<br>
 Example response:
 ```json
 [
   {
     "block_hash": "8e33bb588feff6414469779d724923064688615535280f8982c9981410cd06f6",
@@ -467,15 +414,15 @@
 ```
 
 ### Transactions
 
 #### get_tx_info
 Get detailed information about transaction(s)<br>
 Parameters: Transaction(s) hash(es) as a string (for one transaction) or list (for multiple transactions)<br>
-Returns: The list of transactions details dictionaries<br>
+Returns: The list of transactions details maps<br>
 Example:<br>
 `tx_info = get_tx_info('99f2aefba2a4a5a550aeed9d91d3adabe77a286ec45c345c7980a208364f76c6')`<br>
 Example response:
 ```json
 [
   {
     "tx_hash": "99f2aefba2a4a5a550aeed9d91d3adabe77a286ec45c345c7980a208364f76c6",
@@ -569,15 +516,15 @@
   }
 ]
 ```
 
 #### get_tx_utxos
 Get UTxO set (inputs/outputs) of transactions<br>
 Parameters: Transaction(s) hash(es) as a string (for one transaction) or list (for multiple transactions)<br>
-Returns: The list of transactions UTxOs dictionaries<br>
+Returns: The list of transactions UTxOs maps<br>
 Example:<br>
 `tx_utxos = get_tx_utxos('bf685dde61d36b8acd259b2bd00a69a2e8359d2a69b75aa3a0eff9d38ca1f2ef')`<br>
 Example response:
 ```json
 [
   {
     "tx_hash": "bf685dde61d36b8acd259b2bd00a69a2e8359d2a69b75aa3a0eff9d38ca1f2ef",
@@ -646,15 +593,15 @@
   }
 ]
 ```
 
 #### get_tx_metadata
 Get metadata information (if any) for given transaction(s)<br>
 Parameters: Transaction(s) hash(es) as a string (for one transaction) or list (for multiple transactions)<br>
-Returns: The list of transactions metadata dictionaries<br>
+Returns: The list of transactions metadata maps<br>
 Example:<br>
 `tx_metadata = get_tx_metadata('291b5533227331999eca2e63934c1061e5f85993e77747a90d9901413d7bb937')`<br>
 Example response:
 ```json
 [
   {
     "tx_hash": "291b5533227331999eca2e63934c1061e5f85993e77747a90d9901413d7bb937",
@@ -674,15 +621,15 @@
   }
 ]
 ```
 
 #### get_tx_metalabels
 Get a list of all transaction metadata labels<br>
 Parameters: none<br>
-Returns: The list of transaction metadata labels dictionaries<br>
+Returns: The list of transaction metadata labels maps<br>
 Example:<br>
 `tx_metalabels = get_tx_metalabels()`<br>
 Example response:
 ```json
 [
   {
     "key": "0"
@@ -722,15 +669,15 @@
 ```
 0eec38dc1d2d021f477a890d754e66c49fe74a9fd972793076587496c9850060
 ```
 
 #### get_tx_status
 Get the number of block confirmations for a given transaction hash list<br>
 Parameters: Transaction(s) hash(es) as a string (for one transaction) or list (for multiple transactions)<br>
-Returns: The list of transactions block confirmations dictionaries<br>
+Returns: The list of transactions block confirmations maps<br>
 Example:<br>
 `tx_status = get_tx_status('0eec38dc1d2d021f477a890d754e66c49fe74a9fd972793076587496c9850060')`<br>
 Example response:
 ```json
 [
   {
     "tx_hash": "0eec38dc1d2d021f477a890d754e66c49fe74a9fd972793076587496c9850060",
@@ -740,15 +687,15 @@
 ```
 
 ### Address
 
 #### get_address_info
 Get the transaction hash list of input address array, optionally filtering after specified block height (inclusive)<br>
 Parameters: Payment address(es) as string (for one address) or list (for multiple addresses)<br>
-Returns: The list of transactions dictionaries<br>
+Returns: The list of transactions maps<br>
 Example:<br>
 `address_info = get_address_info('addr1q8wv876ptu0qhujmh2awdcnpcc0ctgdz8e8qvv29k8hucwft99azzjfn9l2658p483uljfdd00ef5rzg58y5km6gj9jqcp0ws7')`<br>
 Example response:
 ```json
 [
   {
     "address": "addr1q8wv876ptu0qhujmh2awdcnpcc0ctgdz8e8qvv29k8hucwft99azzjfn9l2658p483uljfdd00ef5rzg58y5km6gj9jqcp0ws7",
@@ -771,15 +718,15 @@
   }
 ]
 ```
 
 #### get_address_txs
 Get the transaction hash list of input address array, optionally filtering after specified block height (inclusive)<br>
 Parameters: Payment address(es) as string (for one address) or list (for multiple addresses)<br>
-Returns: The list of transactions dictionaries<br>
+Returns: The list of transactions maps<br>
 Example:<br>
 `address_txs = get_address_txs('addr1q8wv876ptu0qhujmh2awdcnpcc0ctgdz8e8qvv29k8hucwft99azzjfn9l2658p483uljfdd00ef5rzg58y5km6gj9jqcp0ws7')`<br>
 Example response:
 ```json
 [
   {
     "tx_hash": "c626fe027d09db2b6c63ba67e3638911ff70e3b691a7e5c03e75c0d3a168c973",
@@ -805,61 +752,18 @@
     "epoch_no": 373,
     "block_height": 7971352,
     "block_time": 1667570778
   }
 ]
 ```
 
-#### get_credential_utxos
-Get a list of UTxO against input payment credential array including their balances<br>
-Parameters: Payment credential(s) as string (for one credential) or list (for multiple credentials)<br>
-Returns: The list of UTxO against input payment credential array including their balances<br>
-Example:<br>
-`credential_utxos = get_credential_utxos('0c35748e147183cd784875e78a5b372fa6975e9ac6406d6015c09bac')`<br>
-Example response:<br>
-```json
-[
-  {
-    "tx_hash": "8e9b85284f92ad85416d4fb0a3ff5d3bbd9b57c4a4d97a8d39dc99316eace0cf",
-    "tx_index": 0,
-    "value": "5000000"
-  },
-  {
-    "tx_hash": "e7333c01d3c2887767aca13e5c74fb858fbf0119cd90d944869ee72b8b81f523",
-    "tx_index": 1,
-    "value": "20432286"
-  },
-  {
-    "tx_hash": "ecfbbc335ec203b10ee65faddf06fb0ceac27c36ef3a76047fbf820f6e9ed7f2",
-    "tx_index": 2,
-    "value": "2301540"
-  },
-  {
-    "tx_hash": "b70a9107a38e776c0b1d94a1578c393a1ce01ea8e28ed56c5c724a2639e31bfe",
-    "tx_index": 2,
-    "value": "1150770"
-  },
-  {
-    "tx_hash": "1107afdada22f259aa798de57ca3839e212e977467628c85315326917a13dd3b",
-    "tx_index": 2,
-    "value": "1150770"
-  },
-  ...
-  {
-    "tx_hash": "b9d519ff9309dd78a7e8031aef2fa6b21358478efed5f0bdf234fa10c83eede7",
-    "tx_index": 1,
-    "value": "137666866"
-  }
-]
-```
-
 #### get_address_assets
 Get the list of all the assets (policy, name and quantity) for given addresses<br>
 Parameters: Payment address(es) as string (for one address) or list (for multiple addresses)<br>
-Returns: The list of assets dictionaries by address<br>
+Returns: The list of assets maps by address<br>
 Example:<br>
 `address_assets = get_address_assets('addr1qywp2795uk4uusknpseu3fcwy8ew57dnuaeutnxaa5j6ulp4u2anham4xet066yjc6xjxcymujvvwlfhj8k8gxfl2nvs73rvzh')`<br>
 Example response:
 ```json
 [
   {
     "address": "addr1qywp2795uk4uusknpseu3fcwy8ew57dnuaeutnxaa5j6ulp4u2anham4xet066yjc6xjxcymujvvwlfhj8k8gxfl2nvs73rvzh",
@@ -887,15 +791,15 @@
   }
 ]
 ```
 
 #### get_credential_txs
 Get the transaction hash list of input payment credential array, optionally filtering after specified block height (inclusive)<br>
 Parameters: Credential(s) as string (for one credential) or list (for multiple credentials)<br>
-Returns: The list of address information dictionaries<br>
+Returns: The list of address information maps<br>
 Example:<br>
 `credential_txs = get_credential_txs('dcc3fb415f1e0bf25bbabae6e261c61f85a1a23e4e063145b1efcc39')`<br>
 Example response:
 ```json
 [
   {
     "tx_hash": "c626fe027d09db2b6c63ba67e3638911ff70e3b691a7e5c03e75c0d3a168c973",
@@ -915,23 +819,268 @@
     "epoch_no": 373,
     "block_height": 7971352,
     "block_time": 1667570778
   }
 ]
 ```
 
+### Account
+
+#### get_account_list
+Get a list of all accounts<br>
+Parameters:<br>
+The offset (optional) to start from, default 0<br>
+The maximum number of accounts to return (optional), default 0 (no limit)<br>
+Returns: The list of accounts maps<br>
+This takes a very long time to execute (about one hour), because the total number of accounts is in the millions range.<br>
+Example:<br>
+`account_list = get_account_list()`<br>
+Example response:
+```json
+[
+  {
+    "id": "stake1uyfmzu5qqy70a8kq4c8rw09q0w0ktfcxppwujejnsh6tyrg5c774g"
+  },
+  {
+    "id": "stake1uydhlh7f2kkw9eazct5zyzlrvj32gjnkmt2v5qf6t8rut4qwch8ey"
+  },
+  {
+    "id": "stake1uxsgkz6fvgws5wn80vckwvghzapnhfmf0672nmmkm2tt9fcaau5sw"
+  },
+  ...
+]
+```
+
+#### get_account_info
+Get the account information for given stake addresses (accounts)<br>
+Parameters: Stake address(es), as a string (for one address) or a list (for multiple addresses)<br>
+Returns: The list of account information maps<br>
+Example:<br>
+`account_info = get_account_info('stake1uy4jj73pfyejl4d2rs6nc70eykkhhu56p3y2rj2tdayfzeqnjyh0j')`<br>
+Example response:
+```json
+[
+  {
+    "stake_address": "stake1uy4jj73pfyejl4d2rs6nc70eykkhhu56p3y2rj2tdayfzeqnjyh0j",
+    "status": "registered",
+    "delegated_pool": "pool18r2y72aue5nmv489xtnfxl36vzusq95qst6urd87yd5hgzms04c",
+    "total_balance": "20418617",
+    "utxo": "20418617",
+    "rewards": "0",
+    "withdrawals": "0",
+    "rewards_available": "0",
+    "reserves": "0",
+    "treasury": "0"
+  }
+]
+```
+
+#### get_account_info_cached
+Get the cached account information for given stake addresses (accounts)<br>
+Parameters: Stake address(es), as a string (for one address) or a list (for multiple addresses)<br>
+Returns: The list of account information maps<br>
+Example:<br>
+`account_info_cached = get_account_info_cached('stake1uy4jj73pfyejl4d2rs6nc70eykkhhu56p3y2rj2tdayfzeqnjyh0j')`<br>
+Example response:
+```json
+[
+  {
+    "stake_address": "stake1uy4jj73pfyejl4d2rs6nc70eykkhhu56p3y2rj2tdayfzeqnjyh0j",
+    "status": "registered",
+    "delegated_pool": "pool18r2y72aue5nmv489xtnfxl36vzusq95qst6urd87yd5hgzms04c",
+    "total_balance": "20418617",
+    "utxo": "20418617",
+    "rewards": "0",
+    "withdrawals": "0",
+    "rewards_available": "0",
+    "reserves": "0",
+    "treasury": "0"
+  }
+]
+```
+
+#### get_account_rewards
+Get the full rewards history (including MIR) for given stake addresses (accounts)<br>
+Parameters:<br>
+Stake address(es), as a string (for one address) or a list (for multiple addresses)<br>
+Epoch (optional), default: current epoch<br>
+Returns: The list of rewards maps by account (stake address)<br>
+Example:<br>
+`account_rewards = get_account_rewards('stake1u8lhspu67x3jejzcfrh487rtu3hnm26cg0jsn0mgh2y6n9q9ve26z')`<br>
+Example response:
+```json
+[
+  {
+    "stake_address": "stake1u8lhspu67x3jejzcfrh487rtu3hnm26cg0jsn0mgh2y6n9q9ve26z",
+    "rewards": [
+      {
+        "earned_epoch": 233,
+        "spendable_epoch": 235,
+        "amount": "3990414",
+        "type": "member",
+        "pool_id": "pool1jdhjfcu34lq88rypdtslzwyf27uh0h3apcr9mjd68zhc69r29fy"
+      },
+      {
+        "earned_epoch": 234,
+        "spendable_epoch": 236,
+        "amount": "2792902",
+        "type": "member",
+        "pool_id": "pool1jdhjfcu34lq88rypdtslzwyf27uh0h3apcr9mjd68zhc69r29fy"
+      },
+      ...
+      {
+        "earned_epoch": 379,
+        "spendable_epoch": 381,
+        "amount": "6496870",
+        "type": "member",
+        "pool_id": "pool12wpfng6cu7dz38yduaul3ngfm44xhv5xmech68m5fwe4wu77udd"
+      }
+    ]
+  }
+]
+```
+
+#### get_account_updates
+Get the account updates (registration, deregistration, delegation and withdrawals) for given stake addresses (accounts)<br>
+Parameters: Stake address(es), as a string (for one address) or a list (for multiple addresses)<br>
+Returns: The list of account updates maps by account (stake address)<br>
+Example:<br>
+`account_updates = get_account_updates('stake1u8lhspu67x3jejzcfrh487rtu3hnm26cg0jsn0mgh2y6n9q9ve26z')`<br>
+Example response:
+```json
+[
+  {
+    "stake_address": "stake1u8lhspu67x3jejzcfrh487rtu3hnm26cg0jsn0mgh2y6n9q9ve26z",
+    "updates": [
+      {
+        "action_type": "withdrawal",
+        "tx_hash": "487bc75f00fe934dad33683271cca8540fe868eef7025962678f179a1a111ecc",
+        "epoch_no": 324,
+        "epoch_slot": 70687,
+        "absolute_slot": 54675487,
+        "block_time": 1646241778
+      },
+      {
+        "action_type": "withdrawal",
+        "tx_hash": "eb3ffa01f434e210716151fd9001af82529e371a91c20af02512942f988a2119",
+        "epoch_no": 269,
+        "epoch_slot": 339679,
+        "absolute_slot": 31184479,
+        "block_time": 1622750770
+      },
+      ...
+      {
+        "action_type": "withdrawal",
+        "tx_hash": "b056dcbff9b908e1bd3ed015466f64486538058ba3553dbf885b216d88343370",
+        "epoch_no": 252,
+        "epoch_slot": 58375,
+        "absolute_slot": 23559175,
+        "block_time": 1615125466
+      }
+    ]
+  }
+]
+```
+
+#### get_account_addresses
+Get all addresses associated with given staking accounts<br>
+Parameters: Stake address(es), as a string (for one address) or a list (for multiple addresses)<br>
+Returns: The list of addresses maps by account (stake address)<br>
+Example:<br>
+`account_addresses = get_account_addresses('stake1u8lhspu67x3jejzcfrh487rtu3hnm26cg0jsn0mgh2y6n9q9ve26z')`<br>
+Example response:
+```json
+[
+  {
+    "stake_address": "stake1u8lhspu67x3jejzcfrh487rtu3hnm26cg0jsn0mgh2y6n9q9ve26z",
+    "addresses": [
+      "addr1qxwjxvzv8rmyutcjp0647w4n05wv7aez9jdmqcxn8a9sshll0qre4udr9ny9sj8020uxher08k44ssl9pxlk3w5f4x2qjyz9yf"
+    ]
+  }
+]
+```
+
+#### get_account_assets
+Get the native asset balance of given accounts<br>
+Parameters: Stake address(es), as a string (for one address) or a list (for multiple addresses)<br>
+Returns: The list of account assets maps by account (stake address)<br>
+Example:<br>
+`account_assets = get_account_assets('stake1u8lhspu67x3jejzcfrh487rtu3hnm26cg0jsn0mgh2y6n9q9ve26z')`<br>
+Example response:
+```json
+[
+  {
+    "stake_address": "stake1u8lhspu67x3jejzcfrh487rtu3hnm26cg0jsn0mgh2y6n9q9ve26z",
+    "asset_list": [
+      {
+        "policy_id": "0029cb7c88c7567b63d1a512c0ed626aa169688ec980730c0473b913",
+        "asset_name": "6c70202302",
+        "fingerprint": "asset1awuysx8hc686uz0dykmvmc7jfut2ulceucf6yc",
+        "quantity": "418089787"
+      },
+      {
+        "policy_id": "0029cb7c88c7567b63d1a512c0ed626aa169688ec980730c0473b913",
+        "asset_name": "6c7020f302",
+        "fingerprint": "asset1mcq0awl6awlaqg0ywukf94q0mnau263l9rght5",
+        "quantity": "586811406"
+      },
+      ...
+      {
+        "policy_id": "ea2d23f1fa631b414252824c153f2d6ba833506477a929770a4dd9c2",
+        "asset_name": "4d414442554c",
+        "fingerprint": "asset1q0kwjy669gmsqpvxp4lr0sp26pdm0dafme3qp2",
+        "quantity": "500"
+      }
+    ]
+  }
+]
+```
+
+#### get_account_history
+Get the staking history of given stake addresses (accounts)<br>
+Parameters: Stake address(es), as a string (for one address) or a list (for multiple addresses)<br>
+Returns: The list of staking history maps by account (stake address)<br>
+Example:<br>
+`account_history = get_account_history('stake1u8lhspu67x3jejzcfrh487rtu3hnm26cg0jsn0mgh2y6n9q9ve26z')`<br>
+Example response:
+```json
+[
+  {
+    "stake_address": "stake1u8lhspu67x3jejzcfrh487rtu3hnm26cg0jsn0mgh2y6n9q9ve26z",
+    "history": [
+      {
+        "pool_id": "pool1jdhjfcu34lq88rypdtslzwyf27uh0h3apcr9mjd68zhc69r29fy",
+        "epoch_no": 233,
+        "active_stake": "4655706122"
+      },
+      {
+        "pool_id": "pool1jdhjfcu34lq88rypdtslzwyf27uh0h3apcr9mjd68zhc69r29fy",
+        "epoch_no": 234,
+        "active_stake": "5020706122"
+      },
+      ...
+      {
+        "pool_id": "pool12wpfng6cu7dz38yduaul3ngfm44xhv5xmech68m5fwe4wu77udd",
+        "epoch_no": 381,
+        "active_stake": "10247851319"
+      }
+    ]
+  }
+]
+```
+
 ### Asset
 
 #### get_asset_list
 Get the list of all native assets (paginated)<br>
 Parameters:<br>
 Asset Policy (optional), default: all policies<br>
 The offset (optional) to start from, default 0<br>
 The maximum number of accounts to return (optional), default 0 (no limit)<br>
-Returns: The list of assets dictionaries by policy<br>
+Returns: The list of assets maps by policy<br>
 Example:<br>
 `asset_list = get_asset_list()`<br>
 Example response:
 ```json
 [
   {
     "policy_id": "00000002df633853f6a47465c9496721d2d5b1291b8398016c0e87ae",
@@ -949,98 +1098,38 @@
     "asset_name": "43726565707942616c6c7a57316231303137",
     "fingerprint": "asset12dvnasghksl5k7w696nd5t692j6myexapwjh0d"
   },
   ...
 ]
 ```
 
-#### get_asset_token_registry
-Get a list of assets registered via token registry on github<br>
-Parameters: none<br>
-Returns: The list of assets registered via token registry on github<br>
-Example:<br>
-`asset_token_registry = get_asset_token_registry()`<br>
-Example response:<br>
-```json
-[
-  {
-    "policy_id": "00000002df633853f6a47465c9496721d2d5b1291b8398016c0e87ae",
-    "asset_name": "6e7574636f696e",
-    "asset_name_ascii": "nutcoin",
-    "ticker": "NUT",
-    "description": "The legendary Nutcoin, the first native asset minted on Cardano.",
-    "url": "https://fivebinaries.com/nutcoin",
-    "decimals": 0,
-    "logo": "iVBORw0KGgoAAAANSUhEUgAAAGQA....2rCPgau2EAAAAASUVORK5CYII="
-  },
-  {
-    "policy_id": "00109530994ea381c0bfe0936c85ea01bfe2765c24ef6dad5740c33e",
-    "asset_name": "486f646c657220436f616c6974696f6e20436f696e",
-    "asset_name_ascii": "Hodler Coalition Coin",
-    "ticker": "HODLR",
-    "description": "Stake ₳DA with the Hodler Coalition. Save the World.",
-    "url": "https://www.hodlerstaking.com/",
-    "decimals": 4,
-    "logo": "iVBORw0KGgoAAAANSUhEUgAAARAAA...4RtRz5t2G8zAAAAAElFTkSuQmCC"
-  },
-  {
-    "policy_id": "0011fbab202151eca9e9ef7680569d9419d12e51e693cb05a2edd2ed",
-    "asset_name": "4341524b",
-    "asset_name_ascii": "Cardano Ark Token",
-    "ticker": "CARK",
-    "description": "Utility token for the Cardano Ark",
-    "url": "https://www.cardanoark.com/",
-    "decimals": 0,
-    "logo": ""
-  },
-  ...
-]
-```
-
-#### get_asset_addresses
+#### get_asset_address_list
 Get the list of all addresses holding a given asset<br>
 Parameters:<br>
 Asset Policy<br>
 Asset Name in hexadecimal format (optional), default: all policy assets<br>
-Returns: List of dictionaries with the wallets holding the asset and the amount of assets per wallet<br>
+Returns: List of maps with the wallets holding the asset and the amount of assets per wallet<br>
 Example:<br>
 `asset_address_list = get_asset_address_list('07697e6ca1e21777ac76f26d0779c53f7d08e47b9e32d23bd8fed9cd', '4379626572696130363936')`<br>
 Example response:
 ```json
 [
   {
     "payment_address": "addr1qywp2795uk4uusknpseu3fcwy8ew57dnuaeutnxaa5j6ulp4u2anham4xet066yjc6xjxcymujvvwlfhj8k8gxfl2nvs73rvzh",
     "quantity": "1"
   }
 ]
 ```
 
-#### get_asset_nft_address
-Get the address where specified NFT currently reside on.<br>
-Parameters:<br>
-Asset Policy<br>
-Asset Name in hexadecimal format<br>
-Returns: The wallet address holding the NFT as a list of one dictionary<br>
-Example:<br>
-`asset_nft_address = get_asset_nft_address('07697e6ca1e21777ac76f26d0779c53f7d08e47b9e32d23bd8fed9cd', '4379626572696130363936')`<br>
-Example response:
-```json
-[
-  {
-    "payment_address": "addr1qywp2795uk4uusknpseu3fcwy8ew57dnuaeutnxaa5j6ulp4u2anham4xet066yjc6xjxcymujvvwlfhj8k8gxfl2nvs73rvzh"
-  }
-]
-```
-
 #### get_asset_info
 Get the information of an asset including first minting & token registry metadata<br>
 Parameters:
 Asset Policy<br>
 Asset Name in hexadecimal format (optional), default: all policy assets<br>
-Returns: List of dictionaries with the wallets holding the asset and the amount of assets per wallet<br>
+Returns: List of maps with the wallets holding the asset and the amount of assets per wallet<br>
 Example:<br>
 `asset_info = get_asset_info('07697e6ca1e21777ac76f26d0779c53f7d08e47b9e32d23bd8fed9cd', '4379626572696130363936')`<br>
 Example response:
 ```json
 [
   {
     "policy_id": "07697e6ca1e21777ac76f26d0779c53f7d08e47b9e32d23bd8fed9cd",
@@ -1088,97 +1177,20 @@
       }
     },
     "token_registry_metadata": null
   }
 ]
 ```
 
-#### get_asset_info_bulk
-Get the information of a list of assets including first minting & token registry metadata<br>
-Parameters:<br>
-Assets List in tge following format: `['policy.name_hex']`<br>
-Returns: List of assets including first minting & token registry metadata<br>
-Example:<br>
-`asset_info_bulk = get_asset_info_bulk(['221b1b9ebccab1512262347491557279ac0afac63b4fbd10fc596c8a.437562656e7369734d757368726f6f6d', '221b1b9ebccab1512262347491557279ac0afac63b4fbd10fc596c8a.417a7a69654d757368726f6f6d'])`<br>
-Example response:
-```json
-[
-  {
-    "policy_id": "221b1b9ebccab1512262347491557279ac0afac63b4fbd10fc596c8a",
-    "asset_name": "437562656e7369734d757368726f6f6d",
-    "asset_name_ascii": "CubensisMushroom",
-    "fingerprint": "asset1csgmd2qwycgmqdck4dgqzzwm7xclhkqrhxs2pw",
-    "minting_tx_hash": "c29fd9f0c71793eb06e7cf055e8529740b0486a802b8e9019df4853c6dec03a0",
-    "total_supply": "7576",
-    "mint_cnt": 1,
-    "burn_cnt": 0,
-    "creation_time": 1680393600,
-    "minting_tx_metadata": {
-      "721": {
-        "version": "1.0",
-        "221b1b9ebccab1512262347491557279ac0afac63b4fbd10fc596c8a": {
-          "CubensisMushroom": {
-            "name": "CubensisMushroom",
-            "files": [
-              {
-                "src": "ipfs://QmQNTa19H5WnYtRiHqzNK2drC9rRTzmkxtu7tS57WZkNuZ",
-                "name": "Cubensis",
-                "mediaType": "image/png"
-              }
-            ],
-            "image": "ipfs://QmQNTa19H5WnYtRiHqzNK2drC9rRTzmkxtu7tS57WZkNuZ",
-            "project": "Chilled Kongs",
-            "mediaType": "image/png"
-          }
-        }
-      }
-    },
-    "token_registry_metadata": null
-  },
-  {
-    "policy_id": "221b1b9ebccab1512262347491557279ac0afac63b4fbd10fc596c8a",
-    "asset_name": "417a7a69654d757368726f6f6d",
-    "asset_name_ascii": "AzzieMushroom",
-    "fingerprint": "asset1kfskmlcvlsvpvr093staxj2788qlrkcrssf26a",
-    "minting_tx_hash": "e4b94e3a5e95953acfb50e3c2fd005b2839ca79c4294b62bbf7d2afdf96dd009",
-    "total_supply": "1305",
-    "mint_cnt": 1,
-    "burn_cnt": 0,
-    "creation_time": 1680393600,
-    "minting_tx_metadata": {
-      "721": {
-        "version": "1.0",
-        "221b1b9ebccab1512262347491557279ac0afac63b4fbd10fc596c8a": {
-          "AzzieMushroom": {
-            "name": "AzzieMushroom",
-            "files": [
-              {
-                "src": "ipfs://QmeAdLCKgXhxtDAcpPq5vgpRCqYWCGFMzb9jx4YEif3nWR",
-                "name": "Azzie",
-                "mediaType": "image/png"
-              }
-            ],
-            "image": "ipfs://QmeAdLCKgXhxtDAcpPq5vgpRCqYWCGFMzb9jx4YEif3nWR",
-            "project": "Chilled Kongs",
-            "mediaType": "image/png"
-          }
-        }
-      }
-    },
-    "token_registry_metadata": null
-  }
-]
-```
-
 #### get_asset_history
 Get the mint/burn history of an asset<br>
 Parameters:<br>
 Asset Policy<br>
 Asset Name in hexadecimal format (optional), default: all policy assets<br>
-Returns: List of dictionaries with the mint/burn history of an asset<br>
+Returns: List of maps with the mint/burn history of an asset<br>
 Example:<br>
 `asset_history = get_asset_history('07697e6ca1e21777ac76f26d0779c53f7d08e47b9e32d23bd8fed9cd', '4379626572696130363936')`<br>
 Example response:
 ```json
 [
   {
     "policy_id": "07697e6ca1e21777ac76f26d0779c53f7d08e47b9e32d23bd8fed9cd",
@@ -1229,49 +1241,20 @@
         ]
       }
     ]
   }
 ]
 ```
 
-#### get_policy_asset_addresses
-Get the list of addresses with quantity for each asset on the given policy<br>
-Parameters: Asset Policy<br>
-Returns: List of addresses with quantity for each asset on the given policy<br>
-Example:<br>
-`asset_policy_info = get_policy_asset_addresses('07697e6ca1e21777ac76f26d0779c53f7d08e47b9e32d23bd8fed9cd')`<br>
-Example response:
-```json
-[
-  {
-    "asset_name": "4379626572696130303233",
-    "payment_address": "addr1qxu5vk5xafdp39d95ya06d6uya8ldua7crpdzd2an07uw8mrtndmfr0d4qarvgj2wasdwlvrnlqt262jn5asnws7aekssq73gf",
-    "quantity": "1"
-  },
-  {
-    "asset_name": "4379626572696130303330",
-    "payment_address": "addr1q9wj7ylly5nz2kel6huy966tcsw2l3ct9at7m3euhfxyv246nlp3dj9pda2rphtzycwexsaapyk73k25y3j5neyhg45s879sk4",
-    "quantity": "1"
-  },
-  ...
-  {
-    "asset_name": "4379626572696132383338",
-    "payment_address": "addr1qxg2l50ryn6z23543v6nujvkql9zwj7f7hvsjwalw6jvf25n5k332a42ge9w5en95g9af59fft32g0la0qtfr9vfyyesccney2",
-    "quantity": "1"
-  }
-]
-```
-
-
-#### get_policy_asset_info
-Get the list of asset under the given policy (including balances)<br>
+#### get_asset_policy_info
+Get the information for all assets under the same policy<br>
 Parameters: Asset Policy<br>
-Returns: List of dictionaries with the policy assets<br>
+Returns: List of maps with the policy assets<br>
 Example:<br>
-`asset_policy_info = get_policy_asset_info('07697e6ca1e21777ac76f26d0779c53f7d08e47b9e32d23bd8fed9cd')`<br>
+`asset_policy_info = get_asset_policy_info('07697e6ca1e21777ac76f26d0779c53f7d08e47b9e32d23bd8fed9cd')`<br>
 Example response:
 ```json
 [
   {
     "asset_name": "",
     "asset_name_ascii": "",
     "fingerprint": "asset1pht97cylpt7azuu9mwhmd9c9zdgmumwrrm5yrc",
@@ -1405,127 +1388,20 @@
     "token_registry_metadata": null,
     "total_supply": "1",
     "creation_time": 1670493734
   }
 ]
 ```
 
-#### get_policy_asset_list
-Get the list of asset under the given policy (including balances)<br>
-Parameters: Asset Policy<br>
-Returns: List of dictionaries with the asset under the given policy<br>
-Example:<br>
-`asset_policy_list = get_policy_asset_list('07697e6ca1e21777ac76f26d0779c53f7d08e47b9e32d23bd8fed9cd')`<br>
-Example response:
-```json
-[
-  {
-    "asset_name": "",
-    "asset_name_ascii": "",
-    "fingerprint": "asset1pht97cylpt7azuu9mwhmd9c9zdgmumwrrm5yrc",
-    "minting_tx_hash": "90415fda215ff5098d7fa1385c7358c589066332068b720380726e3ef0b26de4",
-    "total_supply": "0",
-    "mint_cnt": 1,
-    "burn_cnt": 1,
-    "creation_time": 1665100800,
-    "minting_tx_metadata": {
-      "777": {
-        "addr": [
-          "addr1qy36jns6h4w4f80u6xed49k6qn9c7tk4x4us5kaxztjq8x3un2me8nvc5ke",
-          "gvll0gnwlj2ypzfhhqpns47u76gafttmq208x4d"
-        ],
-        "rate": "0.05"
-      }
-    },
-    "token_registry_metadata": null
-  },
-  ...
-  {
-    "asset_name": "4379626572696130333939",
-    "asset_name_ascii": "Cyberia0399",
-    "fingerprint": "asset1g7tgq2ly8uhtzcz79uhay8tq46h9rq62arfm8s",
-    "minting_tx_hash": "98db0a36106a92149b256887f6300f2b228e14d24d488e4b1614920083cd64ff",
-    "total_supply": "1",
-    "mint_cnt": 1,
-    "burn_cnt": 0,
-    "creation_time": 1665187200,
-    "minting_tx_metadata": {
-      "721": {
-        "nonce": "c966f455d3e03537",
-        "07697e6ca1e21777ac76f26d0779c53f7d08e47b9e32d23bd8fed9cd": {
-          "Cyberia0399": {
-            "Pose": "Lunge pose - Anjaneyasana",
-            "Skin": "Gold",
-            "name": "Cyberia Chakra Planet #0399",
-            "files": [
-              {
-                "src": "ipfs://QmVsMggcQE3da9xuZv7uvJRH84gs5ebGQ8kxVPSQw52XRf",
-                "name": "Please wait while your experience below loads.",
-                "mediaType": "image/jpg"
-              },
-              {
-                "src": "ipfs://QmSHyNm11PrqyrUXszKtsz52ADH6A934c3gw41H7CMCj7D",
-                "mediaType": "text/html"
-              }
-            ],
-            "image": "ipfs://QmVsMggcQE3da9xuZv7uvJRH84gs5ebGQ8kxVPSQw52XRf",
-            "Artist": "Srink",
-            "Avatar": "Male",
-            "Chakra": "Sacral - Svadhisthana",
-            "Mantra": "VAM",
-            "Discord": "https://dsc.gg/cyberiacnft",
-            "Twitter": "https://twitter.com/cyberiaCNFT",
-            "Website": "https://cyberia.gg/",
-            "Function": "Sexual and Creative Energy",
-            "Location": "Below the Belly Button",
-            "Collection": "Chakra Planets",
-            "Planet colour": "Orange"
-          },
-          "Cyberia2795": {
-            "Pose": "Headstand - Sirsasana",
-            "Skin": "Gold",
-            "name": "Cyberia Chakra Planet #2795",
-            "files": [
-              {
-                "src": "ipfs://QmZ4TGY2Jzy5JGaD3S7RLsrP9K8jbp44e7463iHAGitM5a",
-                "name": "Please wait while your experience below loads.",
-                "mediaType": "image/jpg"
-              },
-              {
-                "src": "ipfs://QmcEqKkAcxeGNZimSiQZ2duZA4sx4xJawh35VwuJoS3A9m",
-                "mediaType": "text/html"
-              }
-            ],
-            "image": "ipfs://QmZ4TGY2Jzy5JGaD3S7RLsrP9K8jbp44e7463iHAGitM5a",
-            "Artist": "Srink",
-            "Avatar": "Female",
-            "Chakra": "Crown - Sahasrara",
-            "Mantra": "OM",
-            "Discord": "https://dsc.gg/cyberiacnft",
-            "Twitter": "https://twitter.com/cyberiaCNFT",
-            "Website": "https://cyberia.gg/",
-            "Function": "Spiritual Connection",
-            "Location": "Top of the Head",
-            "Collection": "Chakra Planets",
-            "Planet colour": "Purple"
-          }
-        }
-      }
-    },
-    "token_registry_metadata": null
-  }
-]
-```
-
 #### get_asset_summary
 Get the summary of an asset (total transactions exclude minting/total wallets include only wallets with asset balance)<br>
 Parameters:<br>
 Asset Policy<br>
 Asset Name in hexadecimal format (optional), default: all policy assets<br>
-Returns: List of dictionaries with the mint/burn history of an asset<br>
+Returns: List of maps with the mint/burn history of an asset<br>
 Example:<br>
 `asset_summary = get_asset_summary('07697e6ca1e21777ac76f26d0779c53f7d08e47b9e32d23bd8fed9cd', '4379626572696131313535')`<br>
 Example response:
 ```json
 [
   {
     "policy_id": "07697e6ca1e21777ac76f26d0779c53f7d08e47b9e32d23bd8fed9cd",
@@ -1541,15 +1417,15 @@
 #### get_asset_txs
 Get the list of all asset transaction hashes (the newest first)<br>
 Parameters:<br>
 Asset Policy<br>
 Asset Name in hexadecimal format (optional), default: all policy assets<br>
 Block number (optional) - return only the transactions after this block<br>
 History boolean (optional) - include all historical transactions, setting to false includes only the non-empty ones<br>
-Returns: List of dictionaries with the mint/burn history of an asset<br>
+Returns: List of maps with the mint/burn history of an asset<br>
 Example:<br>
 `asset_txs = get_asset_txs('07697e6ca1e21777ac76f26d0779c53f7d08e47b9e32d23bd8fed9cd', '4379626572696131313535')`<br>
 Example response:
 ```json
 [
   {
     "tx_hash": "d4ac560398b95e6435bd6657e39fe5638f7c5bfaa6ffa6b8fa9bfae0b4882666",
@@ -1561,15 +1437,15 @@
 ```
 
 ### Pool
 
 #### get_pools_list
 A list of all currently registered/retiring (not retired) pools<br>
 Parameters: none<br>
-Returns: The list of stake pool dictionaries<br>
+Returns: The list of stake pool maps<br>
 Example:<br>
 `pool_list = get_pool_list()`<br>
 Example response:
 ```json
 [
   {
     "pool_id_bech32": "pool100wj94uzf54vup2hdzk0afng4dhjaqggt7j434mtgm8v2gfvfgp",
@@ -1656,15 +1532,15 @@
   }
 ]
 ```
 
 #### get_pool_stake_snapshot
 Returns Mark, Set and Go stake snapshots for the selected pool, useful for leaderlog calculation<br>
 Parameters: Stake pool bech32 id<br>
-Returns: Pool snapshot as list of dictionaries by epoch (current and previous 2)<br>
+Returns: Pool snapshot as list of maps by epoch (current and previous 2)<br>
 Example:<br>
 `pool_stake_snapshot = get_pool_stake_snapshot('pool155efqn9xpcf73pphkk88cmlkdwx4ulkg606tne970qswczg3asc')`<br>
 Example response:
 ```json
 [
   {
     "snapshot": "Go",
@@ -1689,15 +1565,15 @@
   }
 ]
 ```
 
 #### get_pool_delegators
 Returns information about live delegators for a given pool<br>
 Parameters Stake pool bech32 id<br>
-Returns: The list of pool delegators dictionaries<br>
+Returns: The list of pool delegators maps<br>
 Example:<br>
 `pool_delegators = get_pool_delegators('pool12wpfng6cu7dz38yduaul3ngfm44xhv5xmech68m5fwe4wu77udd')`<br>
 Example response:
 ```json
 [
   {
     "stake_address": "stake1u80603g5n7vtycl75c60jmv56jx3cw53v23xv0txkpcu8kcwr2k27",
@@ -1722,15 +1598,15 @@
 ```
 
 #### get_pool_delegators_history
 Returns information about active delegators (incl. history) for a given pool and epoch number (all epochs if not specified)<br>
 Parameters:<br>
 Stake pool bech32 id<br>
 Epoch (optional)<br>
-Returns: The list of pool delegators dictionaries<br>
+Returns: The list of pool delegators maps<br>
 Example:<br>
 `pool_delegators_history = get_pool_delegators_history('pool12wpfng6cu7dz38yduaul3ngfm44xhv5xmech68m5fwe4wu77udd', 380)`<br>
 Example response:
 ```json
 [
   {
     "stake_address": "stake1uyezz2wzt4rl5wug8ju8zshvfzkw2lksw8jfp0wpueq2nccnnkwxh",
@@ -1752,15 +1628,15 @@
 ```
 
 #### get_pool_blocks
 Returns information about blocks minted by a given pool for all epochs (or _epoch_no if provided)<br>
 Parameters:<br>
 Stake pool bech32 id<br>
 Epoch (optional)<br>
-Returns: The list of pool blocks dictionaries<br>
+Returns: The list of pool blocks maps<br>
 Example:<br>
 `pool_blocks = get_pool_blocks('pool12wpfng6cu7dz38yduaul3ngfm44xhv5xmech68m5fwe4wu77udd', 380)`<br>
 Example response:
 ```json
 [
   {
     "epoch_no": 380,
@@ -1782,15 +1658,15 @@
 ```
 
 #### get_pool_history
 Returns information about pool stake, block and reward history in a given epoch (or all epochs that pool existed for, in descending order if no epoch number was provided)<br>
 Parameters:<br>
 Stake pool bech32 id<br>
 Epoch (optional)<br>
-Returns:  Information about pool stake, block and reward history as a list dictionaries by epoch (descending)<br>
+Returns:  Information about pool stake, block and reward history as a list maps by epoch (descending)<br>
 Example:<br>
 `pool_history = get_pool_history('pool12wpfng6cu7dz38yduaul3ngfm44xhv5xmech68m5fwe4wu77udd', 379)`<br>
 Example response:
 ```json
 [
   {
     "epoch_no": 379,
@@ -1807,15 +1683,15 @@
   }
 ]
 ```
 
 #### get_pool_updates
 Returns all pool updates for all pools or only updates for specific pool if specified<br>
 Parameters: Stake pool bech32 id (optional)<br>
-Returns: pool updates as a list of dictionaries<br>
+Returns: pool updates as a list of maps<br>
 Example:<br>
 `pool_updates = get_pool_updates('pool12wpfng6cu7dz38yduaul3ngfm44xhv5xmech68m5fwe4wu77udd')`<br>
 Example response:
 ```json
 [
   {
     "tx_hash": "6358622ef9c7a395aaf1590661330a17095fef3c39caa2ae319c737c85bfacb9",
@@ -1896,15 +1772,15 @@
   ...
 ]
 ```
 
 #### get_pool_relays
 A list of registered relays for all currently registered/retiring (not retired) pools<br>
 Parameters: none<br>
-Returns: The list of relays dictionaries by stake pool<br>
+Returns: The list of relays maps by stake pool<br>
 Example:<br>
 `pool_relays = get_pool_relays()`<br>
 Example response:
 ```json
 [
   {
     "pool_id_bech32": "pool100wj94uzf54vup2hdzk0afng4dhjaqggt7j434mtgm8v2gfvfgp",
@@ -1945,15 +1821,15 @@
   ...
 ]
 ```
 
 #### get_pool_metadata
 A list of registered relays for all currently registered/retiring (not retired) pools<br>
 Parameters: Stake pool bech32 ID(s) as string (for one stake pool) or list of stake pool bech32 IDs (for multiple stake pools)<br>
-Returns: The list of pool metadata dictionaries<br>
+Returns: The list of pool metadata maps<br>
 Example:<br>
 `pool_metadata = get_pool_metadata('pool1auvwj75q70s7jce63nvptujs6460kvyxqn0wjegkz4mhja7g5t6')`<br>
 Example response:
 ```json
 [
   {
     "pool_id_bech32": "pool1auvwj75q70s7jce63nvptujs6460kvyxqn0wjegkz4mhja7g5t6",
@@ -1968,15 +1844,15 @@
   }
 ]
 ```
 
 #### get_retiring_pools
 Get the retiring stake pools list<br>
 Parameters: none<br>
-Returns: The list of retiring pools dictionaries<br>
+Returns: The list of retiring pools maps<br>
 Example:<br>
 `retiring_pools = get_retiring_pools()`<br>
 Example response:
 ```json
 [
   {
     "tx_hash": "39a046ef9b5b9e149d24bae8c86f6fb93b08d57312615d22b6a3e73279198e73",
@@ -2040,15 +1916,15 @@
 ```
 
 ### Script
 
 #### get_native_script_list
 List of all existing native script hashes along with their creation transaction hashes<br>
 Parameters: none<br>
-Returns: The list of all native scripts dictionaries<br>
+Returns: The list of all native scripts maps<br>
 Example:<br>
 `native_script_list = get_native_script_list()`<br>
 Example response:
 ```json
 [
   {
     "script_hash": "65c197d565e88a20885e535f93755682444d3c02fd44dd70883fe89e",
@@ -2093,15 +1969,15 @@
   ...
 ]
 ```
 
 #### get_plutus_script_list
 List of all existing native script hashes along with their creation transaction hashes<br>
 Parameters: none<br>
-Returns: The list of all plutus scripts dictionaries<br>
+Returns: The list of all plutus scripts maps<br>
 Example:<br>
 `plutus_script_list = get_plutus_script_list()`<br>
 Example response:
 ```json
 [
   {
     "script_hash": "c916b3d14a51087cc967223aad3f2e4e5c01993f5429719c32c2061e",
@@ -2118,15 +1994,15 @@
   ...
 ]
 ```
 
 #### get_script_redeemers
 List of all redeemers for a given script hash<br>
 Parameters: Script hash<br>
-Returns: Redeemers list as dictionary<br>
+Returns: Redeemers list as map<br>
 Example:<br>
 `script_redeemers = get_script_redeemers('c1996b36d11bf42103745844cc5ee9bf13fde475fa909809e2da7261')`<br>
 Example response:
 ```json
 [
   {
     "script_hash": "c1996b36d11bf42103745844cc5ee9bf13fde475fa909809e2da7261",
@@ -2147,312 +2023,22 @@
   }
 ]
 ```
 
 #### get_datum_info
 List of datum information for given datum hashes<br>
 Parameters: Datum hash(es) as string (for one datum hash) or list (for a list of datum hashes)<br>
-Returns Datum information as list of dictionaries<br>
+Returns Datum information as list of maps<br>
 Example:<br>
 `datum_info = get_datum_info('45b0cfc220ceec5b7c1c62c4d4193d38e4eba48e8815729ce75f9c0ab0e4c1c0')`<br>
 Example response:
 ```json
 [
   {
     "hash": "45b0cfc220ceec5b7c1c62c4d4193d38e4eba48e8815729ce75f9c0ab0e4c1c0",
     "value": {
       "list": []
     },
     "bytes": "80"
   }
 ]
 ```
-
-### Stake Account
-
-#### get_account_list
-Get a list of all accounts<br>
-Parameters:<br>
-The offset (optional) to start from, default 0<br>
-The maximum number of accounts to return (optional), default 0 (no limit)<br>
-Returns: The list of accounts dictionaries<br>
-This takes a very long time to execute (about one hour), because the total number of accounts is in the millions range.<br>
-Example:<br>
-`account_list = get_account_list()`<br>
-Example response:
-```json
-[
-  {
-    "id": "stake1uyfmzu5qqy70a8kq4c8rw09q0w0ktfcxppwujejnsh6tyrg5c774g"
-  },
-  {
-    "id": "stake1uydhlh7f2kkw9eazct5zyzlrvj32gjnkmt2v5qf6t8rut4qwch8ey"
-  },
-  {
-    "id": "stake1uxsgkz6fvgws5wn80vckwvghzapnhfmf0672nmmkm2tt9fcaau5sw"
-  },
-  ...
-]
-```
-
-#### get_account_info
-Get the account information for given stake addresses (accounts)<br>
-Parameters: Stake address(es), as a string (for one address) or a list (for multiple addresses)<br>
-Returns: The list of account information dictionaries<br>
-Example:<br>
-`account_info = get_account_info('stake1uy4jj73pfyejl4d2rs6nc70eykkhhu56p3y2rj2tdayfzeqnjyh0j')`<br>
-Example response:
-```json
-[
-  {
-    "stake_address": "stake1uy4jj73pfyejl4d2rs6nc70eykkhhu56p3y2rj2tdayfzeqnjyh0j",
-    "status": "registered",
-    "delegated_pool": "pool18r2y72aue5nmv489xtnfxl36vzusq95qst6urd87yd5hgzms04c",
-    "total_balance": "20418617",
-    "utxo": "20418617",
-    "rewards": "0",
-    "withdrawals": "0",
-    "rewards_available": "0",
-    "reserves": "0",
-    "treasury": "0"
-  }
-]
-```
-
-#### get_account_utxos
-Get a list of assets registered via token registry on github<br>
-Parameters: Stake address<br>
-Returns: The list of all UTxOs at all payment addresses associated with the stake address<br>
-Example:<br>
-`account_utxos = get_account_utxos('stake1ux5r7myfhycj234wpqyhh3h8skgwvq0hsstpw52f66857uq95cas6')`
-Example response:<br>
-```json
-[
-  {
-	"tx_hash": "215bcaa7b13c491db28d5525d9b2a13a7d8ddabd563da8113a449ab33a6a60be",
-	"tx_index": 2,
-	"address": "addr1q9dwzug2qzdsqvpvrn886nqdtwr02n9kxtwqsxce2gacvedg8akgnwf3y4r2uzqf00rw0pvsucql0pqkzag5n450facqeuerev",
-	"value": "85813474",
-	"block_height": 8214437,
-	"block_time": 1672580966
-  },
-  {
-	"tx_hash": "1eb26dce2f471fbe32aa8cb303f5e8d8078d1da4dbbb78a7bc135036bb3f2f9c",
-	"tx_index": 0,
-	"address": "addr1q88u9gz83nhs9p5pud9kyucx8sg0ygae2p9a4g2p2y55c4ag8akgnwf3y4r2uzqf00rw0pvsucql0pqkzag5n450facqqyd2n7",
-	"value": "110094569",
-	"block_height": 8406870,
-	"block_time": 1676555396
-  },
-  {
-	"tx_hash": "d530de851c2f867f2174c1073b04bdb9f2e2d16029fcfb488e8150ba66976d43",
-	"tx_index": 0,
-	"address": "addr1qxyp2wsafavj47dpc6uqgqx8se3969jn4crfk7y4zwd7vfag8akgnwf3y4r2uzqf00rw0pvsucql0pqkzag5n450facqlyvudm",
-	"value": "1249900",
-	"block_height": 8489290,
-	"block_time": 1678248733
-  },
-  ...
-  {
-	"tx_hash": "d8e3ca8b36f9a785ff33f01aa5460f9248ea94acd621ea187093206b04aa6e30",
-	"tx_index": 0,
-	"address": "addr1q8txa88kt6rpdv3zzn8ghx7u4udf6rpj690rfdvlqn35fldg8akgnwf3y4r2uzqf00rw0pvsucql0pqkzag5n450facqplx97u",
-	"value": "54000000",
-	"block_height": 8759577,
-	"block_time": 1683809438
-  }
-]
-```
-
-#### get_account_info_cached
-Get the cached account information for given stake addresses (accounts)<br>
-Parameters: Stake address(es), as a string (for one address) or a list (for multiple addresses)<br>
-Returns: The list of account information dictionaries<br>
-Example:<br>
-`account_info_cached = get_account_info_cached('stake1uy4jj73pfyejl4d2rs6nc70eykkhhu56p3y2rj2tdayfzeqnjyh0j')`<br>
-Example response:
-```json
-[
-  {
-    "stake_address": "stake1uy4jj73pfyejl4d2rs6nc70eykkhhu56p3y2rj2tdayfzeqnjyh0j",
-    "status": "registered",
-    "delegated_pool": "pool18r2y72aue5nmv489xtnfxl36vzusq95qst6urd87yd5hgzms04c",
-    "total_balance": "20418617",
-    "utxo": "20418617",
-    "rewards": "0",
-    "withdrawals": "0",
-    "rewards_available": "0",
-    "reserves": "0",
-    "treasury": "0"
-  }
-]
-```
-
-#### get_account_rewards
-Get the full rewards history (including MIR) for given stake addresses (accounts)<br>
-Parameters:<br>
-Stake address(es), as a string (for one address) or a list (for multiple addresses)<br>
-Epoch (optional), default: current epoch<br>
-Returns: The list of rewards dictionaries by account (stake address)<br>
-Example:<br>
-`account_rewards = get_account_rewards('stake1u8lhspu67x3jejzcfrh487rtu3hnm26cg0jsn0mgh2y6n9q9ve26z')`<br>
-Example response:
-```json
-[
-  {
-    "stake_address": "stake1u8lhspu67x3jejzcfrh487rtu3hnm26cg0jsn0mgh2y6n9q9ve26z",
-    "rewards": [
-      {
-        "earned_epoch": 233,
-        "spendable_epoch": 235,
-        "amount": "3990414",
-        "type": "member",
-        "pool_id": "pool1jdhjfcu34lq88rypdtslzwyf27uh0h3apcr9mjd68zhc69r29fy"
-      },
-      {
-        "earned_epoch": 234,
-        "spendable_epoch": 236,
-        "amount": "2792902",
-        "type": "member",
-        "pool_id": "pool1jdhjfcu34lq88rypdtslzwyf27uh0h3apcr9mjd68zhc69r29fy"
-      },
-      ...
-      {
-        "earned_epoch": 379,
-        "spendable_epoch": 381,
-        "amount": "6496870",
-        "type": "member",
-        "pool_id": "pool12wpfng6cu7dz38yduaul3ngfm44xhv5xmech68m5fwe4wu77udd"
-      }
-    ]
-  }
-]
-```
-
-#### get_account_updates
-Get the account updates (registration, deregistration, delegation and withdrawals) for given stake addresses (accounts)<br>
-Parameters: Stake address(es), as a string (for one address) or a list (for multiple addresses)<br>
-Returns: The list of account updates dictionaries by account (stake address)<br>
-Example:<br>
-`account_updates = get_account_updates('stake1u8lhspu67x3jejzcfrh487rtu3hnm26cg0jsn0mgh2y6n9q9ve26z')`<br>
-Example response:
-```json
-[
-  {
-    "stake_address": "stake1u8lhspu67x3jejzcfrh487rtu3hnm26cg0jsn0mgh2y6n9q9ve26z",
-    "updates": [
-      {
-        "action_type": "withdrawal",
-        "tx_hash": "487bc75f00fe934dad33683271cca8540fe868eef7025962678f179a1a111ecc",
-        "epoch_no": 324,
-        "epoch_slot": 70687,
-        "absolute_slot": 54675487,
-        "block_time": 1646241778
-      },
-      {
-        "action_type": "withdrawal",
-        "tx_hash": "eb3ffa01f434e210716151fd9001af82529e371a91c20af02512942f988a2119",
-        "epoch_no": 269,
-        "epoch_slot": 339679,
-        "absolute_slot": 31184479,
-        "block_time": 1622750770
-      },
-      ...
-      {
-        "action_type": "withdrawal",
-        "tx_hash": "b056dcbff9b908e1bd3ed015466f64486538058ba3553dbf885b216d88343370",
-        "epoch_no": 252,
-        "epoch_slot": 58375,
-        "absolute_slot": 23559175,
-        "block_time": 1615125466
-      }
-    ]
-  }
-]
-```
-
-#### get_account_addresses
-Get all addresses associated with given staking accounts<br>
-Parameters: Stake address(es), as a string (for one address) or a list (for multiple addresses)<br>
-Returns: The list of addresses dictionaries by account (stake address)<br>
-Example:<br>
-`account_addresses = get_account_addresses('stake1u8lhspu67x3jejzcfrh487rtu3hnm26cg0jsn0mgh2y6n9q9ve26z')`<br>
-Example response:
-```json
-[
-  {
-    "stake_address": "stake1u8lhspu67x3jejzcfrh487rtu3hnm26cg0jsn0mgh2y6n9q9ve26z",
-    "addresses": [
-      "addr1qxwjxvzv8rmyutcjp0647w4n05wv7aez9jdmqcxn8a9sshll0qre4udr9ny9sj8020uxher08k44ssl9pxlk3w5f4x2qjyz9yf"
-    ]
-  }
-]
-```
-
-#### get_account_assets
-Get the native asset balance of given accounts<br>
-Parameters: Stake address(es), as a string (for one address) or a list (for multiple addresses)<br>
-Returns: The list of account assets dictionaries by account (stake address)<br>
-Example:<br>
-`account_assets = get_account_assets('stake1u8lhspu67x3jejzcfrh487rtu3hnm26cg0jsn0mgh2y6n9q9ve26z')`<br>
-Example response:
-```json
-[
-  {
-    "stake_address": "stake1u8lhspu67x3jejzcfrh487rtu3hnm26cg0jsn0mgh2y6n9q9ve26z",
-    "asset_list": [
-      {
-        "policy_id": "0029cb7c88c7567b63d1a512c0ed626aa169688ec980730c0473b913",
-        "asset_name": "6c70202302",
-        "fingerprint": "asset1awuysx8hc686uz0dykmvmc7jfut2ulceucf6yc",
-        "quantity": "418089787"
-      },
-      {
-        "policy_id": "0029cb7c88c7567b63d1a512c0ed626aa169688ec980730c0473b913",
-        "asset_name": "6c7020f302",
-        "fingerprint": "asset1mcq0awl6awlaqg0ywukf94q0mnau263l9rght5",
-        "quantity": "586811406"
-      },
-      ...
-      {
-        "policy_id": "ea2d23f1fa631b414252824c153f2d6ba833506477a929770a4dd9c2",
-        "asset_name": "4d414442554c",
-        "fingerprint": "asset1q0kwjy669gmsqpvxp4lr0sp26pdm0dafme3qp2",
-        "quantity": "500"
-      }
-    ]
-  }
-]
-```
-
-#### get_account_history
-Get the staking history of given stake addresses (accounts)<br>
-Parameters: Stake address(es), as a string (for one address) or a list (for multiple addresses)<br>
-Returns: The list of staking history dictionaries by account (stake address)<br>
-Example:<br>
-`account_history = get_account_history('stake1u8lhspu67x3jejzcfrh487rtu3hnm26cg0jsn0mgh2y6n9q9ve26z')`<br>
-Example response:
-```json
-[
-  {
-    "stake_address": "stake1u8lhspu67x3jejzcfrh487rtu3hnm26cg0jsn0mgh2y6n9q9ve26z",
-    "history": [
-      {
-        "pool_id": "pool1jdhjfcu34lq88rypdtslzwyf27uh0h3apcr9mjd68zhc69r29fy",
-        "epoch_no": 233,
-        "active_stake": "4655706122"
-      },
-      {
-        "pool_id": "pool1jdhjfcu34lq88rypdtslzwyf27uh0h3apcr9mjd68zhc69r29fy",
-        "epoch_no": 234,
-        "active_stake": "5020706122"
-      },
-      ...
-      {
-        "pool_id": "pool12wpfng6cu7dz38yduaul3ngfm44xhv5xmech68m5fwe4wu77udd",
-        "epoch_no": 381,
-        "active_stake": "10247851319"
-      }
-    ]
-  }
-]
-```
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

