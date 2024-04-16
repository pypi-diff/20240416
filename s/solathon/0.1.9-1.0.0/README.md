# Comparing `tmp/solathon-0.1.9.tar.gz` & `tmp/solathon-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "solathon-0.1.9.tar", max compression
+gzip compressed data, was "solathon-1.0.0.tar", max compression
```

## Comparing `solathon-0.1.9.tar` & `solathon-1.0.0.tar`

### file list

```diff
@@ -1,32 +1,32 @@
--rw-r--r--   0        0        0     1050 2024-01-06 21:15:59.435978 solathon-0.1.9/LICENSE
--rw-r--r--   0        0        0     1502 2024-01-06 21:15:59.435978 solathon-0.1.9/README.md
--rw-r--r--   0        0        0     1125 2024-03-08 21:01:32.517259 solathon-0.1.9/pyproject.toml
--rw-r--r--   0        0        0      213 2024-03-08 21:01:27.690501 solathon-0.1.9/solathon/__init__.py
--rw-r--r--   0        0        0    18172 2024-03-08 20:58:42.260584 solathon-0.1.9/solathon/async_client.py
--rw-r--r--   0        0        0    25342 2024-03-08 20:58:32.570384 solathon-0.1.9/solathon/client.py
--rw-r--r--   0        0        0       20 2024-01-06 21:15:59.439311 solathon-0.1.9/solathon/core/__init__.py
--rw-r--r--   0        0        0     3004 2024-01-06 21:15:59.439311 solathon-0.1.9/solathon/core/http.py
--rw-r--r--   0        0        0     5146 2024-01-06 21:15:59.439311 solathon-0.1.9/solathon/core/instructions.py
--rw-r--r--   0        0        0     3040 2024-01-06 21:15:59.439311 solathon-0.1.9/solathon/core/layouts.py
--rw-r--r--   0        0        0     6280 2024-01-07 20:01:57.832864 solathon-0.1.9/solathon/core/message.py
--rw-r--r--   0        0        0     4602 2024-01-06 21:15:59.439311 solathon-0.1.9/solathon/core/types/__init__.py
--rw-r--r--   0        0        0     1360 2024-01-25 09:54:40.427471 solathon-0.1.9/solathon/core/types/account_info.py
--rw-r--r--   0        0        0     6669 2024-01-06 21:15:59.439311 solathon-0.1.9/solathon/core/types/block.py
--rw-r--r--   0        0        0      778 2024-01-06 21:15:59.439311 solathon-0.1.9/solathon/core/types/cluster_node.py
--rw-r--r--   0        0        0     1426 2024-01-06 21:15:59.439311 solathon-0.1.9/solathon/core/types/epoch.py
--rw-r--r--   0        0        0     1750 2024-01-06 21:15:59.439311 solathon-0.1.9/solathon/core/types/inflation.py
--rw-r--r--   0        0        0     2395 2024-01-07 19:55:24.758478 solathon-0.1.9/solathon/keypair.py
--rw-r--r--   0        0        0     1305 2024-01-08 19:28:39.511834 solathon-0.1.9/solathon/publickey.py
--rw-r--r--   0        0        0      286 2024-01-06 21:16:57.563254 solathon-0.1.9/solathon/solana_pay/__init__.py
--rw-r--r--   0        0        0     1622 2024-01-07 20:11:35.958900 solathon-0.1.9/solathon/solana_pay/create_qr.py
--rw-r--r--   0        0        0     5128 2024-01-07 20:49:58.290008 solathon-0.1.9/solathon/solana_pay/create_transfer.py
--rw-r--r--   0        0        0     3129 2024-01-06 21:15:59.439311 solathon-0.1.9/solathon/solana_pay/encode_url.py
--rw-r--r--   0        0        0     3044 2024-01-11 21:42:03.545691 solathon-0.1.9/solathon/solana_pay/fetch_transaction.py
--rw-r--r--   0        0        0     1148 2024-01-08 19:28:39.511834 solathon-0.1.9/solathon/solana_pay/find_reference.py
--rw-r--r--   0        0        0     2592 2024-01-11 21:42:03.545691 solathon-0.1.9/solathon/solana_pay/parse_url.py
--rw-r--r--   0        0        0     3053 2024-01-06 21:15:59.439311 solathon-0.1.9/solathon/solana_pay/qr-logo.png
--rw-r--r--   0        0        0      914 2024-01-11 21:42:03.545691 solathon-0.1.9/solathon/solana_pay/types.py
--rw-r--r--   0        0        0     3507 2024-01-08 19:28:39.511834 solathon-0.1.9/solathon/solana_pay/validate_transfer.py
--rw-r--r--   0        0        0    11293 2024-01-07 20:07:29.119692 solathon-0.1.9/solathon/transaction.py
--rw-r--r--   0        0        0     2150 2024-01-06 21:16:46.463137 solathon-0.1.9/solathon/utils.py
--rw-r--r--   0        0        0     2754 1970-01-01 00:00:00.000000 solathon-0.1.9/PKG-INFO
+-rw-r--r--   0        0        0     1050 2024-04-16 13:48:37.758737 solathon-1.0.0/LICENSE
+-rw-r--r--   0        0        0     1428 2024-04-16 14:15:10.734716 solathon-1.0.0/README.md
+-rw-r--r--   0        0        0     1135 2024-04-16 14:15:34.950535 solathon-1.0.0/pyproject.toml
+-rw-r--r--   0        0        0      213 2024-04-16 14:31:44.119135 solathon-1.0.0/solathon/__init__.py
+-rw-r--r--   0        0        0    18172 2024-04-16 14:31:07.234418 solathon-1.0.0/solathon/async_client.py
+-rw-r--r--   0        0        0    26417 2024-04-16 14:11:21.518429 solathon-1.0.0/solathon/client.py
+-rw-r--r--   0        0        0       20 2024-04-16 13:48:37.765736 solathon-1.0.0/solathon/core/__init__.py
+-rw-r--r--   0        0        0     3004 2024-04-16 13:48:37.765736 solathon-1.0.0/solathon/core/http.py
+-rw-r--r--   0        0        0     5146 2024-04-16 13:48:37.765736 solathon-1.0.0/solathon/core/instructions.py
+-rw-r--r--   0        0        0     3040 2024-04-16 13:48:37.765736 solathon-1.0.0/solathon/core/layouts.py
+-rw-r--r--   0        0        0     6280 2024-04-16 13:48:37.765736 solathon-1.0.0/solathon/core/message.py
+-rw-r--r--   0        0        0     4602 2024-04-16 13:48:37.765736 solathon-1.0.0/solathon/core/types/__init__.py
+-rw-r--r--   0        0        0     1360 2024-04-16 13:48:37.765736 solathon-1.0.0/solathon/core/types/account_info.py
+-rw-r--r--   0        0        0     6669 2024-04-16 13:48:37.765736 solathon-1.0.0/solathon/core/types/block.py
+-rw-r--r--   0        0        0      778 2024-04-16 13:48:37.765736 solathon-1.0.0/solathon/core/types/cluster_node.py
+-rw-r--r--   0        0        0     1426 2024-04-16 13:48:37.765736 solathon-1.0.0/solathon/core/types/epoch.py
+-rw-r--r--   0        0        0     1750 2024-04-16 13:48:37.765736 solathon-1.0.0/solathon/core/types/inflation.py
+-rw-r--r--   0        0        0     2395 2024-04-16 14:28:08.682787 solathon-1.0.0/solathon/keypair.py
+-rw-r--r--   0        0        0     1222 2024-04-16 14:21:14.602960 solathon-1.0.0/solathon/publickey.py
+-rw-r--r--   0        0        0      286 2024-04-16 13:48:37.766737 solathon-1.0.0/solathon/solana_pay/__init__.py
+-rw-r--r--   0        0        0     1622 2024-04-16 13:48:37.766737 solathon-1.0.0/solathon/solana_pay/create_qr.py
+-rw-r--r--   0        0        0     5128 2024-04-16 13:48:37.766737 solathon-1.0.0/solathon/solana_pay/create_transfer.py
+-rw-r--r--   0        0        0     3129 2024-04-16 13:48:37.766737 solathon-1.0.0/solathon/solana_pay/encode_url.py
+-rw-r--r--   0        0        0     3044 2024-04-16 13:48:37.766737 solathon-1.0.0/solathon/solana_pay/fetch_transaction.py
+-rw-r--r--   0        0        0     1148 2024-04-16 13:48:37.766737 solathon-1.0.0/solathon/solana_pay/find_reference.py
+-rw-r--r--   0        0        0     2592 2024-04-16 13:48:37.766737 solathon-1.0.0/solathon/solana_pay/parse_url.py
+-rw-r--r--   0        0        0     3053 2024-04-16 13:48:37.766737 solathon-1.0.0/solathon/solana_pay/qr-logo.png
+-rw-r--r--   0        0        0      914 2024-04-16 13:48:37.766737 solathon-1.0.0/solathon/solana_pay/types.py
+-rw-r--r--   0        0        0     3507 2024-04-16 13:48:37.766737 solathon-1.0.0/solathon/solana_pay/validate_transfer.py
+-rw-r--r--   0        0        0    11293 2024-04-16 13:48:37.766737 solathon-1.0.0/solathon/transaction.py
+-rw-r--r--   0        0        0     2150 2024-04-16 13:48:37.766737 solathon-1.0.0/solathon/utils.py
+-rw-r--r--   0        0        0     2636 1970-01-01 00:00:00.000000 solathon-1.0.0/PKG-INFO
```

### Comparing `solathon-0.1.9/LICENSE` & `solathon-1.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `solathon-0.1.9/README.md` & `solathon-1.0.0/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -15,17 +15,14 @@
   <br>
 </p>
 
 <h1 align="center">Solathon</h1>
 
 Solathon is a high performance, easy to use and feature-rich Solana SDK for Python. Easy for beginners, powerful for real world applications.
 
-|🧪| The project is in beta phase|
-|---|-----------------------------|
-
 # ✨ Getting started
 ## Installation
 ```
 pip install solathon
 ```
 ## Client example
 ```python
```

#### html2text {}

```diff
@@ -1,13 +1,12 @@
                                 _[_S_o_l_a_t_h_o_n_ _l_o_g_o_]
                           _[_P_y_P_I_ _v_e_r_s_i_o_n_]_[_M_I_T_ _L_i_c_e_n_s_e_]
                             ************ SSoollaatthhoonn ************
 Solathon is a high performance, easy to use and feature-rich Solana SDK for
-Python. Easy for beginners, powerful for real world applications. |ð§ª| The
-project is in beta phase| |---|-----------------------------| # â¨ Getting
+Python. Easy for beginners, powerful for real world applications. # â¨ Getting
 started ## Installation ``` pip install solathon ``` ## Client example
 ```python from solathon import Client client = Client("https://
 api.devnet.solana.com") ``` ## Basic usage example ```python # Basic example of
 fetching a public key's balance from solathon import Client, PublicKey client =
 Client("https://api.devnet.solana.com") public_key = PublicKey
 ("B3BhJ1nvPvEhx3hq3nfK8hx4WYcKZdbhavSobZEA44ai") balance = client.get_balance
 (public_key) print(balance) ``` # ðï¸ Contribution Drop a pull request for
```

### Comparing `solathon-0.1.9/pyproject.toml` & `solathon-1.0.0/pyproject.toml`

 * *Files 9% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 [tool.poetry]
 name = "solathon"
-version = "0.1.9"
+version = "1.0.0"
 description = "High performance, easy to use and feature-rich Solana SDK for Python."
 license = "MIT"
 authors = ["GitBolt"]
 readme = "README.md"
 repository = "https://github.com/GitBolt/solathon"
-keywords = ["solana", "web3", "sdk", "blockchain"]
+keywords = ["solana", "web3", "sdk", "blockchain", "crypto"]
 classifiers = [
     "Intended Audience :: Developers",
     "Operating System :: OS Independent",
     "License :: OSI Approved :: MIT License",
     "Topic :: Software Development :: Libraries :: Python Modules",
     "Topic :: Software Development",
     "Programming Language :: Python :: 3.8",
```

### Comparing `solathon-0.1.9/solathon/async_client.py` & `solathon-1.0.0/solathon/async_client.py`

 * *Files identical despite different names*

### Comparing `solathon-0.1.9/solathon/client.py` & `solathon-1.0.0/solathon/client.py`

 * *Files 9% similar despite different names*

```diff
@@ -2,30 +2,69 @@
 
 from typing import Any, List, Literal, Optional, Text, Union
 
 from .utils import RPCRequestError, validate_commitment
 from .publickey import PublicKey
 from .core.http import HTTPClient
 from .transaction import Transaction
-from .core.types import (BlockHash, BlockHashType, Commitment, LargestAccounts, LargestAccountsType, PubKeyIdentity, PubKeyIdentityType, RPCResponse, 
-                         AccountInfo, AccountInfoType, Block, BlockType, BlockProductionType, BlockProduction, BlockCommitmentType, BlockCommitment, 
-                         ClusterNode, ClusterNodeType, Epoch, EpochType, EpochSchedule, EpochScheduleType, InflationGovernor, InflationGovernorType, 
-                         InflationRate, InflationRateType, InflationReward, InflationRewardType, ProgramAccount, ProgramAccountType, RecentPerformanceSamples, 
-                         RecentPerformanceSamplesType, SignatureStatus, SignatureStatusType, Supply, SupplyType, TransactionSignature, TransactionSignatureType, 
-                         TransactionElement, TransactionElementType)
+from .core.types import (
+    BlockHash,
+    BlockHashType,
+    Commitment,
+    LargestAccounts,
+    LargestAccountsType,
+    PubKeyIdentity,
+    PubKeyIdentityType,
+    RPCResponse,
+    AccountInfo,
+    AccountInfoType,
+    Block,
+    BlockType,
+    BlockProductionType,
+    BlockProduction,
+    BlockCommitmentType,
+    BlockCommitment,
+    ClusterNode,
+    ClusterNodeType,
+    Epoch,
+    EpochType,
+    EpochSchedule,
+    EpochScheduleType,
+    InflationGovernor,
+    InflationGovernorType,
+    InflationRate,
+    InflationRateType,
+    InflationReward,
+    InflationRewardType,
+    ProgramAccount,
+    ProgramAccountType,
+    RecentPerformanceSamples,
+    RecentPerformanceSamplesType,
+    SignatureStatus,
+    SignatureStatusType,
+    Supply,
+    SupplyType,
+    TransactionSignature,
+    TransactionSignatureType,
+    TransactionElement,
+    TransactionElementType,
+)
 
 
 ENDPOINTS = (
     "https://api.mainnet-beta.solana.com",
     "https://api.devnet.solana.com",
     "https://api.testnet.solana.com",
 )
 
+
 class Client:
-    def __init__(self, endpoint: Text, local: bool = False, clean_response: bool=True):
+    def __init__(
+        self, endpoint: Text, local: bool = False, clean_response: bool = True
+    ):
         """
         Initializes a new instance of the Client class.
 
         Args:
             endpoint (str): The endpoint to connect to.
             local (bool, optional): Whether to use a local development endpoint. Defaults to False.
             clean_response (bool, optional): Whether to clean the response from the RPC endpoint. Defaults to True.
@@ -45,48 +84,54 @@
 
     def refresh_http(self) -> None:
         """
         Refreshes the HTTP client.
         """
         self.http.refresh()
 
-    def get_account_info(self, public_key: PublicKey | Text, commitment: Optional[Commitment]=None) -> RPCResponse[AccountInfoType] | AccountInfo:
+    def get_account_info(
+        self, public_key: PublicKey | Text, commitment: Optional[Commitment] = None
+    ) -> RPCResponse[AccountInfoType] | AccountInfo:
         """
         Returns all the account info for the specified public key.
 
         Args:
             public_key (PublicKey | str): The public key of the account.
             commitment (Commitment, optional): The level of commitment desired when querying state.
 
         Returns:
             RPCResponse: The response from the RPC endpoint.
         """
         commitment = validate_commitment(commitment) if commitment else None
-        response = self.build_and_send_request("getAccountInfo", [public_key, commitment])
+        response = self.build_and_send_request(
+            "getAccountInfo", [public_key, commitment]
+        )
         if self.clean_response:
-            if response['value'] == None:
+            if response["value"] == None:
                 raise RPCRequestError(f"Account details not found: {public_key}")
-            return AccountInfo(response['value'])
+            return AccountInfo(response["value"])
         return response
 
-    def get_balance(self, public_key: PublicKey | Text, commitment: Optional[Commitment]=None) -> RPCResponse[int] | int:
+    def get_balance(
+        self, public_key: PublicKey | Text, commitment: Optional[Commitment] = None
+    ) -> RPCResponse[int] | int:
         """
         Returns the balance of the specified public key.
 
         Args:
             public_key (PublicKey | Text): The public key of the account.
             commitment (Commitment, optional): The level of commitment desired when querying state.
 
         Returns:
             RPCResponse: The response from the RPC endpoint.
         """
         commitment = validate_commitment(commitment) if commitment else None
         response = self.build_and_send_request("getBalance", [public_key, commitment])
         if self.clean_response:
-            return response['value']
+            return response["value"]
 
         return response
 
     def get_block(self, slot: int) -> RPCResponse[BlockType] | Block:
         """
         Returns the block at the specified slot.
 
@@ -97,59 +142,70 @@
             RPCResponse: The response from the RPC endpoint.
         """
         response = self.build_and_send_request("getBlock", [slot])
         if self.clean_response:
             return Block(response)
         return response
 
-    def get_block_height(self, commitment: Optional[Commitment]=None) -> RPCResponse[int] | int:
+    def get_block_height(
+        self, commitment: Optional[Commitment] = None
+    ) -> RPCResponse[int] | int:
         """
         Returns the current block height.
 
         Args:
             commitment (Commitment, optional): The level of commitment desired when querying state.
 
         Returns:
             RPCResponse: The response from the RPC endpoint.
         """
         commitment = validate_commitment(commitment) if commitment else None
         return self.build_and_send_request("getBlockHeight", [commitment])
 
-    def get_block_production(self, commitment: Optional[Commitment]=None) -> RPCResponse[BlockProductionType] | BlockProduction:
+    def get_block_production(
+        self, commitment: Optional[Commitment] = None
+    ) -> RPCResponse[BlockProductionType] | BlockProduction:
         """
         Returns the block production information.
 
         Args:
             commitment (Commitment, optional): The level of commitment desired when querying state.
 
         Returns:
             RPCResponse: The response from the RPC endpoint.
         """
         commitment = validate_commitment(commitment) if commitment else None
         response = self.build_and_send_request("getBlockProduction", [commitment])
         if self.clean_response:
-            return BlockProduction(response['value'])
+            return BlockProduction(response["value"])
         return response
 
-    def get_block_commitment(self, block: int) -> RPCResponse[BlockCommitmentType] | BlockCommitment:
+    def get_block_commitment(
+        self, block: int
+    ) -> RPCResponse[BlockCommitmentType] | BlockCommitment:
         """
         Returns the block commitment information for the specified block.
 
         Args:
             block (int): The block number.
 
         Returns:
             RPCResponse: The response from the RPC endpoint.
         """
         response = self.build_and_send_request("getBlockCommitment", [block])
         if self.clean_response:
             return BlockCommitment(response)
         return response
 
-    def get_blocks(self, start_slot: int, end_slot: int | None = None, commitment: Optional[Commitment]=None) -> RPCResponse[List[int]] | List[int]:
+    def get_blocks(
+        self,
+        start_slot: int,
+        end_slot: int | None = None,
+        commitment: Optional[Commitment] = None,
+    ) -> RPCResponse[List[int]] | List[int]:
         """
         Returns the blocks in the specified range.
 
         Args:
             start_slot (int): The start slot.
             end_slot (int | None, optional): The end slot. Defaults to None.
             commitment (Commitment, optional): The level of commitment desired when querying state.
@@ -161,15 +217,17 @@
         params = [start_slot]
         if end_slot:
             params.append(end_slot)
         params.append(commitment)
 
         return self.build_and_send_request("getBlocks", params)
 
-    def get_blocks_with_limit(self, start_slot: int, limit: int) -> RPCResponse[List[int]] | List[int]:
+    def get_blocks_with_limit(
+        self, start_slot: int, limit: int
+    ) -> RPCResponse[List[int]] | List[int]:
         """
         Returns the blocks in the specified range with a limit.
 
         Args:
             start_slot (int): The start slot.
             limit (int): The limit.
 
@@ -186,27 +244,31 @@
             block (int): The block number.
 
         Returns:
             RPCResponse: The response from the RPC endpoint.
         """
         return self.build_and_send_request("getBlockTime", [block])
 
-    def get_cluster_nodes(self) -> RPCResponse[List[ClusterNodeType]] | List[ClusterNode]:
+    def get_cluster_nodes(
+        self,
+    ) -> RPCResponse[List[ClusterNodeType]] | List[ClusterNode]:
         """
         Returns the cluster nodes.
 
         Returns:
             RPCResponse: The response from the RPC endpoint.
         """
         response = self.build_and_send_request("getClusterNodes", [None])
         if self.clean_response:
             return [ClusterNode(node) for node in response]
         return response
 
-    def get_epoch_info(self, commitment: Optional[Commitment]=None) -> RPCResponse[EpochType] | Epoch:
+    def get_epoch_info(
+        self, commitment: Optional[Commitment] = None
+    ) -> RPCResponse[EpochType] | Epoch:
         """
         Returns the epoch information.
 
         Args:
             commitment (Commitment, optional): The level of commitment desired when querying state.
 
         Returns:
@@ -226,29 +288,33 @@
             RPCResponse: The response from the RPC endpoint.
         """
         response = self.build_and_send_request("getEpochSchedule", [None])
         if self.clean_response:
             return EpochSchedule(response)
         return response
 
-    def get_fee_for_message(self, message: Text, commitment: Optional[Commitment]=None) -> RPCResponse[int] | int:
+    def get_fee_for_message(
+        self, message: Text, commitment: Optional[Commitment] = None
+    ) -> RPCResponse[int] | int:
         """
         Returns the fee for the specified message.
 
         Args:
             message (str): The message.
             commitment (Commitment, optional): The level of commitment desired when querying state.
 
         Returns:
             RPCResponse: The response from the RPC endpoint.
         """
         commitment = validate_commitment(commitment) if commitment else None
-        response = self.build_and_send_request("getFeeForMessage", [message, commitment])
+        response = self.build_and_send_request(
+            "getFeeForMessage", [message, commitment]
+        )
         if self.clean_response:
-            return response['value']
+            return response["value"]
         return response
 
     # Going to be deprecated
     def get_fees(self) -> RPCResponse:
         """
         Returns the fees.
 
@@ -292,15 +358,17 @@
             RPCResponse: The response from the RPC endpoint.
         """
         response = self.build_and_send_request("getIdentity", [None])
         if self.clean_response:
             return PubKeyIdentity(response)
         return response
 
-    def get_inflation_governor(self, commitment: Optional[Commitment]=None) -> RPCResponse[InflationGovernorType] | InflationGovernor:
+    def get_inflation_governor(
+        self, commitment: Optional[Commitment] = None
+    ) -> RPCResponse[InflationGovernorType] | InflationGovernor:
         """
         Returns the inflation governor.
 
         Args:
             commitment (Commitment, optional): The level of commitment desired when querying state.
 
         Returns:
@@ -320,15 +388,17 @@
             RPCResponse: The response from the RPC endpoint.
         """
         response = self.build_and_send_request("getInflationRate", [None])
         if self.clean_response:
             return InflationRate(response)
         return response
 
-    def get_inflation_reward(self, addresses: List[Text], commitment: Optional[Commitment]=None) -> RPCResponse[List[InflationRewardType]] | List[InflationReward]:
+    def get_inflation_reward(
+        self, addresses: List[Text], commitment: Optional[Commitment] = None
+    ) -> RPCResponse[List[InflationRewardType]] | List[InflationReward]:
         """
         Returns the inflation reward for the specified addresses.
 
         Args:
             addresses (list[str]): The addresses.
             commitment (Commitment, optional): The level of commitment desired when querying state.
 
@@ -338,27 +408,33 @@
         commitment = validate_commitment(commitment) if commitment else None
         addresses.append(commitment)
         response = self.build_and_send_request("getInflationReward", addresses)
         if self.clean_response:
             return [InflationReward(reward) for reward in response]
         return response
 
-    def get_largest_accounts(self) -> RPCResponse[List[LargestAccountsType]] | List[LargestAccounts]:
+    def get_largest_accounts(
+        self,
+    ) -> RPCResponse[List[LargestAccountsType]] | List[LargestAccounts]:
         """
         Returns the largest accounts.
 
         Returns:
             RPCResponse: The response from the RPC endpoint.
         """
         response = self.build_and_send_request("getLargestAccounts", [None])
         if self.clean_response:
-            return [LargestAccounts(account) for account in response['value']]
+            return [LargestAccounts(account) for account in response["value"]]
         return response
 
-    def get_leader_schedule(self) -> RPCResponse[dict[str, Union[List[int], Any]]] | dict[str, Union[List[int],Any]]:
+    def get_leader_schedule(
+        self,
+    ) -> (
+        RPCResponse[dict[str, Union[List[int], Any]]] | dict[str, Union[List[int], Any]]
+    ):
         """
         Returns the leader schedule.
 
         Returns:
             RPCResponse: The response from the RPC endpoint.
         """
         return self.build_and_send_request("getLeaderSchedule", [None])
@@ -377,15 +453,17 @@
         Returns the maximum shred insert slot.
 
         Returns:
             RPCResponse: The response from the RPC endpoint.
         """
         return self.build_and_send_request("getMaxShredInsertSlot", [None])
 
-    def get_minimum_balance_for_rent_exemption(self, acct_length: int, commitment: Optional[Commitment]=None) -> RPCResponse[int] | int:
+    def get_minimum_balance_for_rent_exemption(
+        self, acct_length: int, commitment: Optional[Commitment] = None
+    ) -> RPCResponse[int] | int:
         """
         Returns the minimum balance for rent exemption.
 
         Args:
             acct_length (int): The length of the account.
             commitment (Commitment, optional): The level of commitment desired when querying state.
 
@@ -393,30 +471,34 @@
             RPCResponse: The response from the RPC endpoint.
         """
         commitment = validate_commitment(commitment) if commitment else None
         return self.build_and_send_request(
             "getMinimumBalanceForRentExemption", [acct_length, commitment]
         )
 
-    def get_multiple_accounts(self, pubkeys: List[str]) -> RPCResponse[List[AccountInfoType]] | List[AccountInfo]:
+    def get_multiple_accounts(
+        self, pubkeys: List[str]
+    ) -> RPCResponse[List[AccountInfoType]] | List[AccountInfo]:
         """
         Returns the multiple accounts.
 
         Args:
             pubkeys (list): The public keys.
 
         Returns:
             RPCResponse: The response from the RPC endpoint.
         """
         response = self.build_and_send_request("getMultipleAccounts", pubkeys)
         if self.clean_response:
-            return [AccountInfo(account) for account in response['value']]
+            return [AccountInfo(account) for account in response["value"]]
         return response
 
-    def get_program_accounts(self, public_key: PublicKey) -> RPCResponse[List[ProgramAccountType]] | List[ProgramAccount]:
+    def get_program_accounts(
+        self, public_key: PublicKey
+    ) -> RPCResponse[List[ProgramAccountType]] | List[ProgramAccount]:
         """
         Returns the program accounts.
 
         Args:
             public_key (PublicKey): The public key.
 
         Returns:
@@ -424,74 +506,103 @@
         """
         response = self.build_and_send_request("getProgramAccounts", [public_key])
         if self.clean_response:
             return [ProgramAccount(account) for account in response]
         return response
 
     # Will switch to getFeeForMessage (latest)
-    def get_recent_blockhash(self, commitment: Optional[Commitment]=None) -> RPCResponse[BlockHashType] | BlockHash:
+    def get_recent_blockhash(
+        self, commitment: Optional[Commitment] = None
+    ) -> RPCResponse[BlockHashType] | BlockHash:
         """
         Returns the recent blockhash.
 
         Args:
             commitment (Commitment, optional): The level of commitment desired when querying state.
 
         Returns:
             RPCResponse: The response from the RPC endpoint.
         """
         commitment = validate_commitment(commitment) if commitment else None
         response = self.build_and_send_request("getRecentBlockhash", [commitment])
         if self.clean_response:
-            return BlockHash(response['value'])
+            return BlockHash(response["value"])
         return response
 
-    def get_recent_performance_samples(self, commitment: Optional[Commitment]=None) -> RPCResponse[List[RecentPerformanceSamplesType]] | List[RecentPerformanceSamples]:
+    def get_recent_performance_samples(
+        self, commitment: Optional[Commitment] = None
+    ) -> (
+        RPCResponse[List[RecentPerformanceSamplesType]] | List[RecentPerformanceSamples]
+    ):
         """
         Returns the recent performance samples.
 
         Args:
             commitment (Commitment, optional): The level of commitment desired when querying state.
 
         Returns:
             RPCResponse: The response from the RPC endpoint.
         """
         commitment = validate_commitment(commitment) if commitment else None
-        response = self.build_and_send_request("getRecentPerformanceSamples", [commitment])
+        response = self.build_and_send_request(
+            "getRecentPerformanceSamples", [commitment]
+        )
         if self.clean_response:
             return [RecentPerformanceSamples(sample) for sample in response]
         return response
 
-    def get_signatures_for_address(self, acct_address: Text) -> RPCResponse[List[TransactionSignatureType]] | List[TransactionSignature]:
+    def get_signatures_for_address(
+        self,
+        acct_address: Text,
+        limit: Optional[Text],
+        before: Optional[Text],
+        until: Optional[Text],
+    ) -> RPCResponse[List[TransactionSignatureType]] | List[TransactionSignature]:
         """
         Returns the signatures for the specified account address.
 
         Args:
             acct_address (str): The account address.
 
         Returns:
             RPCResponse: The response from the RPC endpoint.
         """
-        response = self.build_and_send_request("getSignaturesForAddress", [acct_address])
+        params = [acct_address]
+        options = {}
+
+        if limit is not None:
+            options["limit"] = limit
+        if before is not None:
+            options["before"] = before
+        if until is not None:
+            options["until"] = until
+
+        if options:
+            params.append(options)
+
+        response = self.build_and_send_request("getSignaturesForAddress", params)
         if self.clean_response:
             return [TransactionSignature(signature) for signature in response]
         return response
 
-    def get_signature_statuses(self, transaction_sigs: List[Text]) -> RPCResponse[List[SignatureStatusType]] | List[SignatureStatus]:
+    def get_signature_statuses(
+        self, transaction_sigs: List[Text]
+    ) -> RPCResponse[List[SignatureStatusType]] | List[SignatureStatus]:
         """
         Returns the signature statuses for the specified transaction signatures.
 
         Args:
             transaction_sigs (list[str]): The transaction signatures.
 
         Returns:
             RPCResponse: The response from the RPC endpoint.
         """
         response = self.build_and_send_request("getSignatureStatuses", transaction_sigs)
         if self.clean_response:
-            return [SignatureStatus(status) for status in response['value']]
+            return [SignatureStatus(status) for status in response["value"]]
         return response
 
     def get_slot(self) -> RPCResponse[int] | int:
         """
         Returns the current slot.
 
         Returns:
@@ -504,19 +615,22 @@
         Returns the supply.
 
         Returns:
             RPCResponse: The response from the RPC endpoint.
         """
         response = self.build_and_send_request("getSupply", [None])
         if self.clean_response:
-            return Supply(response['value'])
+            return Supply(response["value"])
         return response
 
     def get_token_accounts_by_owner(
-        self, public_key: Text | PublicKey, commitment: Optional[Commitment]=None, **kwargs
+        self,
+        public_key: Text | PublicKey,
+        commitment: Optional[Commitment] = None,
+        **kwargs,
     ) -> RPCResponse[List[ProgramAccountType]] | List[ProgramAccount]:
         """
         Returns the token accounts for the specified owner.
 
         Args:
             public_key (str | PublicKey): The public key of the owner.
             commitment (Commitment, optional): The level of commitment desired when querying state.
@@ -539,26 +653,25 @@
 
         commitment = validate_commitment(commitment) if commitment else None
         response = self.build_and_send_request(
             "getTokenAccountsByOwner",
             [
                 str(public_key),
                 {"mint": mint_id} if mint_id else {"programId": program_id},
-                {
-                    "encoding": encoding,
-                    "commitment": commitment
-                },
+                {"encoding": encoding, "commitment": commitment},
             ],
         )
         if self.clean_response:
-            return [ProgramAccount(account) for account in response['value']]
+            return [ProgramAccount(account) for account in response["value"]]
         return response
 
     def get_token_account_balance(
-        self, token_account: Text | PublicKey, commitment: Optional[Commitment]=None,
+        self,
+        token_account: Text | PublicKey,
+        commitment: Optional[Commitment] = None,
     ) -> RPCResponse:
         """
         Returns the token account balance for the specified owner.
 
         Args:
             token_account (str | PublicKey): The token account pubkey.
             commitment (Commitment, optional): The level of commitment desired when querying state.
@@ -571,58 +684,72 @@
         response = self.build_and_send_request(
             "getTokenAccountBalance",
             [
                 str(token_account),
             ],
         )
         if self.clean_response:
-            return response['value']
+            return response["value"]
         return response
 
-
-    def get_transaction(self, signature: Text, commitment: Optional[Commitment]=None) -> RPCResponse[TransactionElementType] | TransactionElement:
+    def get_transaction(
+        self, signature: Text, commitment: Optional[Commitment] = None
+    ) -> RPCResponse[TransactionElementType] | TransactionElement:
         """
         Sends a request to the Solana RPC endpoint to retrieve a transaction by its signature.
 
         Args:
             signature (str): The signature of the transaction to retrieve.
             commitment (Commitment, optional): The level of commitment desired when querying state.
 
         Returns:
             RPCResponse: The response from the Solana RPC endpoint.
         """
-        response = self.build_and_send_request("getTransaction", [signature, commitment])
+        response = self.build_and_send_request(
+            "getTransaction", [signature, commitment]
+        )
         if self.clean_response:
             if response == None:
                 raise ValueError("Transaction not found")
             return TransactionElement(response)
         return response
 
-    def build_and_send_request(self, method, params: List[Any]) -> RPCResponse | dict[str, Any] | List[dict[str, Any]]:
+    def build_and_send_request(
+        self, method, params: List[Any]
+    ) -> RPCResponse | dict[str, Any] | List[dict[str, Any]]:
         """
         Builds and sends an RPC request to the server.
 
         Args:
             method (str): The RPC method to call.
             params (List[Any]): The parameters to pass to the RPC method.
 
         Returns:
             RPCResponse: The response from the server.
         """
         data: dict[str, Any] = self.http.build_data(method=method, params=params)
         res: RPCResponse = self.http.send(data)
         if self.clean_response:
             if "error" in res:
-                raise RPCRequestError(f"Failed to fetch data from RPC endpoint. Error {res['error']['code']}: {res['error']['message']}")
-            
-            if isinstance(res['result'], dict) or isinstance(res['result'], list) or isinstance(res['result'], str) or res['result'] == None:
-                return res['result']
+                raise RPCRequestError(
+                    f"Failed to fetch data from RPC endpoint. Error {res['error']['code']}: {res['error']['message']}"
+                )
+
+            if (
+                isinstance(res["result"], dict)
+                or isinstance(res["result"], list)
+                or isinstance(res["result"], str)
+                or res["result"] == None
+            ):
+                return res["result"]
             else:
-                raise RPCRequestError(f"Invalid response from RPC endpoint. Expected types dict | list | str, got {type(res['result']).__name__}")
-            
+                raise RPCRequestError(
+                    f"Invalid response from RPC endpoint. Expected types dict | list | str, got {type(res['result']).__name__}"
+                )
+
         return res
 
     # Non "get" methods
     def request_airdrop(
         self, public_key: PublicKey | Text, lamports: int
     ) -> RPCResponse[str] | str:
         """
```

### Comparing `solathon-0.1.9/solathon/core/http.py` & `solathon-1.0.0/solathon/core/http.py`

 * *Files identical despite different names*

### Comparing `solathon-0.1.9/solathon/core/instructions.py` & `solathon-1.0.0/solathon/core/instructions.py`

 * *Files identical despite different names*

### Comparing `solathon-0.1.9/solathon/core/layouts.py` & `solathon-1.0.0/solathon/core/layouts.py`

 * *Files identical despite different names*

### Comparing `solathon-0.1.9/solathon/core/message.py` & `solathon-1.0.0/solathon/core/message.py`

 * *Files identical despite different names*

### Comparing `solathon-0.1.9/solathon/core/types/__init__.py` & `solathon-1.0.0/solathon/core/types/__init__.py`

 * *Files identical despite different names*

### Comparing `solathon-0.1.9/solathon/core/types/account_info.py` & `solathon-1.0.0/solathon/core/types/account_info.py`

 * *Files identical despite different names*

### Comparing `solathon-0.1.9/solathon/core/types/block.py` & `solathon-1.0.0/solathon/core/types/block.py`

 * *Files identical despite different names*

### Comparing `solathon-0.1.9/solathon/core/types/cluster_node.py` & `solathon-1.0.0/solathon/core/types/cluster_node.py`

 * *Files identical despite different names*

### Comparing `solathon-0.1.9/solathon/core/types/epoch.py` & `solathon-1.0.0/solathon/core/types/epoch.py`

 * *Files identical despite different names*

### Comparing `solathon-0.1.9/solathon/core/types/inflation.py` & `solathon-1.0.0/solathon/core/types/inflation.py`

 * *Files identical despite different names*

### Comparing `solathon-0.1.9/solathon/keypair.py` & `solathon-1.0.0/solathon/keypair.py`

 * *Files identical despite different names*

### Comparing `solathon-0.1.9/solathon/publickey.py` & `solathon-1.0.0/solathon/publickey.py`

 * *Files 16% similar despite different names*

```diff
@@ -2,29 +2,29 @@
 
 import base58
 
 
 class PublicKey:
     LENGTH = 32
 
-    def __init__(self, value: bytearray | bytes | int | str | list[int]):
+    def __init__(self, value: bytes | int | str | list[int] | bytearray):
         if isinstance(value, str):
             try:
                 self.byte_value = base58.b58decode(value)
             except ValueError:
-                raise ValueError("Invalid public key.")
+                raise ValueError("Invalid public key")
 
         elif isinstance(value, int):
             self.byte_value = bytes([value])
 
         else:
             self.byte_value = bytes(value)
 
         if len(self.byte_value) != self.LENGTH:
-            raise ValueError("Invalid public key, the length is wrong.")
+            raise ValueError("Invalid public key, the length must be 32 bytes")
 
     def __bytes__(self) -> bytes:
         return (
             self.byte_value
             if len(self.byte_value) == self.LENGTH
             else self.byte_value.rjust(self.LENGTH, b"\0")
         )
@@ -37,11 +37,8 @@
     
     def __eq__(self, __value: object) -> bool:
         if isinstance(__value, PublicKey):
             return self.byte_value == __value.byte_value
         return False
 
     def base58_encode(self) -> bytes:
-        return base58.b58encode(bytes(self))
-
-    def base58_decode(self) -> bytes:
-        return base58.b58decode(self.byte_value)
+        return base58.b58encode(bytes(self))
```

### Comparing `solathon-0.1.9/solathon/solana_pay/create_qr.py` & `solathon-1.0.0/solathon/solana_pay/create_qr.py`

 * *Files identical despite different names*

### Comparing `solathon-0.1.9/solathon/solana_pay/create_transfer.py` & `solathon-1.0.0/solathon/solana_pay/create_transfer.py`

 * *Files identical despite different names*

### Comparing `solathon-0.1.9/solathon/solana_pay/encode_url.py` & `solathon-1.0.0/solathon/solana_pay/encode_url.py`

 * *Files identical despite different names*

### Comparing `solathon-0.1.9/solathon/solana_pay/fetch_transaction.py` & `solathon-1.0.0/solathon/solana_pay/fetch_transaction.py`

 * *Files identical despite different names*

### Comparing `solathon-0.1.9/solathon/solana_pay/find_reference.py` & `solathon-1.0.0/solathon/solana_pay/find_reference.py`

 * *Files identical despite different names*

### Comparing `solathon-0.1.9/solathon/solana_pay/parse_url.py` & `solathon-1.0.0/solathon/solana_pay/parse_url.py`

 * *Files identical despite different names*

### Comparing `solathon-0.1.9/solathon/solana_pay/qr-logo.png` & `solathon-1.0.0/solathon/solana_pay/qr-logo.png`

 * *Files identical despite different names*

### Comparing `solathon-0.1.9/solathon/solana_pay/types.py` & `solathon-1.0.0/solathon/solana_pay/types.py`

 * *Files identical despite different names*

### Comparing `solathon-0.1.9/solathon/solana_pay/validate_transfer.py` & `solathon-1.0.0/solathon/solana_pay/validate_transfer.py`

 * *Files identical despite different names*

### Comparing `solathon-0.1.9/solathon/transaction.py` & `solathon-1.0.0/solathon/transaction.py`

 * *Files identical despite different names*

### Comparing `solathon-0.1.9/solathon/utils.py` & `solathon-1.0.0/solathon/utils.py`

 * *Files identical despite different names*

### Comparing `solathon-0.1.9/PKG-INFO` & `solathon-1.0.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,25 +1,24 @@
 Metadata-Version: 2.1
 Name: solathon
-Version: 0.1.9
+Version: 1.0.0
 Summary: High performance, easy to use and feature-rich Solana SDK for Python.
 Home-page: https://github.com/GitBolt/solathon
 License: MIT
-Keywords: solana,web3,sdk,blockchain
+Keywords: solana,web3,sdk,blockchain,crypto
 Author: GitBolt
 Requires-Python: >=3.8,<4.0
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: Software Development
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Requires-Dist: PyNaCl (>=1.5.0,<2.0.0)
 Requires-Dist: base58 (>=2.1.1,<3.0.0)
 Requires-Dist: construct (>=2.10.67,<3.0.0)
 Requires-Dist: httpx (>=0.22.0,<0.23.0)
 Requires-Dist: pillow (>=10.2.0,<11.0.0)
@@ -45,17 +44,14 @@
   <br>
 </p>
 
 <h1 align="center">Solathon</h1>
 
 Solathon is a high performance, easy to use and feature-rich Solana SDK for Python. Easy for beginners, powerful for real world applications.
 
-|🧪| The project is in beta phase|
-|---|-----------------------------|
-
 # ✨ Getting started
 ## Installation
 ```
 pip install solathon
 ```
 ## Client example
 ```python
```

#### html2text {}

```diff
@@ -1,30 +1,29 @@
-Metadata-Version: 2.1 Name: solathon Version: 0.1.9 Summary: High performance,
+Metadata-Version: 2.1 Name: solathon Version: 1.0.0 Summary: High performance,
 easy to use and feature-rich Solana SDK for Python. Home-page: https://
-github.com/GitBolt/solathon License: MIT Keywords: solana,web3,sdk,blockchain
-Author: GitBolt Requires-Python: >=3.8,<4.0 Classifier: Intended Audience ::
-Developers Classifier: License :: OSI Approved :: MIT License Classifier:
-Operating System :: OS Independent Classifier: Programming Language :: Python
-:: 3 Classifier: Programming Language :: Python :: 3.8 Classifier: Programming
-Language :: Python :: 3.9 Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11 Classifier: Programming
-Language :: Python :: 3.12 Classifier: Topic :: Software Development
-Classifier: Topic :: Software Development :: Libraries :: Python Modules
-Requires-Dist: PyNaCl (>=1.5.0,<2.0.0) Requires-Dist: base58 (>=2.1.1,<3.0.0)
-Requires-Dist: construct (>=2.10.67,<3.0.0) Requires-Dist: httpx
-(>=0.22.0,<0.23.0) Requires-Dist: pillow (>=10.2.0,<11.0.0) Requires-Dist:
-qrcode (>=7.4.2,<8.0.0) Requires-Dist: typing-extensions (>=4.1.1,<5.0.0) ;
-python_version == "3.10" Project-URL: Repository, https://github.com/GitBolt/
-solathon Description-Content-Type: text/markdown
+github.com/GitBolt/solathon License: MIT Keywords:
+solana,web3,sdk,blockchain,crypto Author: GitBolt Requires-Python: >=3.8,<4.0
+Classifier: Intended Audience :: Developers Classifier: License :: OSI Approved
+:: MIT License Classifier: Operating System :: OS Independent Classifier:
+Programming Language :: Python :: 3 Classifier: Programming Language :: Python
+:: 3.8 Classifier: Programming Language :: Python :: 3.9 Classifier:
+Programming Language :: Python :: 3.10 Classifier: Programming Language ::
+Python :: 3.11 Classifier: Topic :: Software Development Classifier: Topic ::
+Software Development :: Libraries :: Python Modules Requires-Dist: PyNaCl
+(>=1.5.0,<2.0.0) Requires-Dist: base58 (>=2.1.1,<3.0.0) Requires-Dist:
+construct (>=2.10.67,<3.0.0) Requires-Dist: httpx (>=0.22.0,<0.23.0) Requires-
+Dist: pillow (>=10.2.0,<11.0.0) Requires-Dist: qrcode (>=7.4.2,<8.0.0)
+Requires-Dist: typing-extensions (>=4.1.1,<5.0.0) ; python_version == "3.10"
+Project-URL: Repository, https://github.com/GitBolt/solathon Description-
+Content-Type: text/markdown
                                 _[_S_o_l_a_t_h_o_n_ _l_o_g_o_]
                           _[_P_y_P_I_ _v_e_r_s_i_o_n_]_[_M_I_T_ _L_i_c_e_n_s_e_]
                             ************ SSoollaatthhoonn ************
 Solathon is a high performance, easy to use and feature-rich Solana SDK for
-Python. Easy for beginners, powerful for real world applications. |ð§ª| The
-project is in beta phase| |---|-----------------------------| # â¨ Getting
+Python. Easy for beginners, powerful for real world applications. # â¨ Getting
 started ## Installation ``` pip install solathon ``` ## Client example
 ```python from solathon import Client client = Client("https://
 api.devnet.solana.com") ``` ## Basic usage example ```python # Basic example of
 fetching a public key's balance from solathon import Client, PublicKey client =
 Client("https://api.devnet.solana.com") public_key = PublicKey
 ("B3BhJ1nvPvEhx3hq3nfK8hx4WYcKZdbhavSobZEA44ai") balance = client.get_balance
 (public_key) print(balance) ``` # ðï¸ Contribution Drop a pull request for
```

