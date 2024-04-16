# Comparing `tmp/olas_operate_middleware-0.1.0rc3.tar.gz` & `tmp/olas_operate_middleware-0.1.0rc4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "olas_operate_middleware-0.1.0rc3.tar", max compression
+gzip compressed data, was "olas_operate_middleware-0.1.0rc4.tar", max compression
```

## Comparing `olas_operate_middleware-0.1.0rc3.tar` & `olas_operate_middleware-0.1.0rc4.tar`

### file list

```diff
@@ -1,37 +1,37 @@
--rw-r--r--   0        0        0    11339 2024-02-06 05:22:56.471559 olas_operate_middleware-0.1.0rc3/LICENSE
--rw-r--r--   0        0        0     4282 2024-03-05 05:48:41.164427 olas_operate_middleware-0.1.0rc3/README.md
--rw-r--r--   0        0        0      803 2024-02-27 08:48:06.011840 olas_operate_middleware-0.1.0rc3/operate/__init__.py
--rw-r--r--   0        0        0      804 2024-04-05 14:54:43.348635 olas_operate_middleware-0.1.0rc3/operate/account/__init__.py
--rw-r--r--   0        0        0     2109 2024-04-05 14:54:43.349000 olas_operate_middleware-0.1.0rc3/operate/account/user.py
--rw-r--r--   0        0        0    17481 2024-04-11 14:01:32.694321 olas_operate_middleware-0.1.0rc3/operate/cli.py
--rw-r--r--   0        0        0     1091 2024-02-27 08:48:06.012404 olas_operate_middleware-0.1.0rc3/operate/constants.py
--rw-r--r--   0        0        0      864 2024-03-08 10:47:59.399920 olas_operate_middleware-0.1.0rc3/operate/data/__init__.py
--rw-r--r--   0        0        0      809 2024-02-27 08:48:06.013275 olas_operate_middleware-0.1.0rc3/operate/data/contracts/__init__.py
--rw-r--r--   0        0        0      866 2024-02-27 08:48:06.013458 olas_operate_middleware-0.1.0rc3/operate/data/contracts/service_staking_token/__init__.py
--rw-r--r--   0        0        0    82730 2024-02-27 08:48:06.014051 olas_operate_middleware-0.1.0rc3/operate/data/contracts/service_staking_token/build/ServiceStakingToken.json
--rw-r--r--   0        0        0     5847 2024-02-27 08:48:06.014506 olas_operate_middleware-0.1.0rc3/operate/data/contracts/service_staking_token/contract.py
--rw-r--r--   0        0        0      724 2024-02-27 08:48:06.014716 olas_operate_middleware-0.1.0rc3/operate/data/contracts/service_staking_token/contract.yaml
--rw-r--r--   0        0        0      868 2024-02-28 14:31:11.754886 olas_operate_middleware-0.1.0rc3/operate/data/contracts/uniswap_v2_erc20/__init__.py
--rw-r--r--   0        0        0    14169 2024-02-28 14:31:11.755175 olas_operate_middleware-0.1.0rc3/operate/data/contracts/uniswap_v2_erc20/build/IUniswapV2ERC20.json
--rw-r--r--   0        0        0     6985 2024-03-08 10:47:59.400374 olas_operate_middleware-0.1.0rc3/operate/data/contracts/uniswap_v2_erc20/contract.py
--rw-r--r--   0        0        0      741 2024-02-28 14:31:11.755543 olas_operate_middleware-0.1.0rc3/operate/data/contracts/uniswap_v2_erc20/contract.yaml
--rw-r--r--   0        0        0     4646 2024-03-14 12:31:10.592254 olas_operate_middleware-0.1.0rc3/operate/http/__init__.py
--rw-r--r--   0        0        0     1232 2024-02-27 08:48:06.014903 olas_operate_middleware-0.1.0rc3/operate/http/exceptions.py
--rw-r--r--   0        0        0     2809 2024-03-27 11:16:42.979679 olas_operate_middleware-0.1.0rc3/operate/keys.py
--rw-r--r--   0        0        0     2849 2024-04-05 14:54:43.350001 olas_operate_middleware-0.1.0rc3/operate/ledger/__init__.py
--rw-r--r--   0        0        0     1154 2024-03-08 10:47:59.401479 olas_operate_middleware-0.1.0rc3/operate/ledger/base.py
--rw-r--r--   0        0        0     1510 2024-03-08 10:47:59.401635 olas_operate_middleware-0.1.0rc3/operate/ledger/ethereum.py
--rw-r--r--   0        0        0     1610 2024-03-08 10:47:59.401789 olas_operate_middleware-0.1.0rc3/operate/ledger/profiles.py
--rw-r--r--   0        0        0     1199 2024-03-08 10:47:59.401953 olas_operate_middleware-0.1.0rc3/operate/ledger/solana.py
--rw-r--r--   0        0        0     3880 2024-04-05 14:54:43.350296 olas_operate_middleware-0.1.0rc3/operate/resource.py
--rw-r--r--   0        0        0      855 2024-03-27 11:16:42.980219 olas_operate_middleware-0.1.0rc3/operate/services/__init__.py
--rw-r--r--   0        0        0    16425 2024-04-11 14:01:32.695097 olas_operate_middleware-0.1.0rc3/operate/services/manage.py
--rw-r--r--   0        0        0    21677 2024-04-05 14:54:43.352503 olas_operate_middleware-0.1.0rc3/operate/services/protocol.py
--rw-r--r--   0        0        0    13412 2024-04-11 14:01:32.695617 olas_operate_middleware-0.1.0rc3/operate/services/service.py
--rw-r--r--   0        0        0     5357 2024-04-05 14:54:43.352823 olas_operate_middleware-0.1.0rc3/operate/types.py
--rw-r--r--   0        0        0      808 2024-04-05 14:54:43.353285 olas_operate_middleware-0.1.0rc3/operate/utils/__init__.py
--rw-r--r--   0        0        0     6082 2024-04-05 14:54:43.353744 olas_operate_middleware-0.1.0rc3/operate/utils/gnosis.py
--rw-r--r--   0        0        0      813 2024-04-05 14:54:43.353950 olas_operate_middleware-0.1.0rc3/operate/wallet/__init__.py
--rw-r--r--   0        0        0     8662 2024-04-11 14:01:32.695981 olas_operate_middleware-0.1.0rc3/operate/wallet/master.py
--rw-r--r--   0        0        0      803 2024-04-11 14:03:40.857830 olas_operate_middleware-0.1.0rc3/pyproject.toml
--rw-r--r--   0        0        0     5092 1970-01-01 00:00:00.000000 olas_operate_middleware-0.1.0rc3/PKG-INFO
+-rw-r--r--   0        0        0    11339 2024-02-06 05:22:56.471559 olas_operate_middleware-0.1.0rc4/LICENSE
+-rw-r--r--   0        0        0     4282 2024-03-05 05:48:41.164427 olas_operate_middleware-0.1.0rc4/README.md
+-rw-r--r--   0        0        0      803 2024-02-27 08:48:06.011840 olas_operate_middleware-0.1.0rc4/operate/__init__.py
+-rw-r--r--   0        0        0      804 2024-04-05 14:54:43.348635 olas_operate_middleware-0.1.0rc4/operate/account/__init__.py
+-rw-r--r--   0        0        0     2109 2024-04-05 14:54:43.349000 olas_operate_middleware-0.1.0rc4/operate/account/user.py
+-rw-r--r--   0        0        0    17479 2024-04-16 04:07:53.585535 olas_operate_middleware-0.1.0rc4/operate/cli.py
+-rw-r--r--   0        0        0     1091 2024-02-27 08:48:06.012404 olas_operate_middleware-0.1.0rc4/operate/constants.py
+-rw-r--r--   0        0        0      864 2024-03-08 10:47:59.399920 olas_operate_middleware-0.1.0rc4/operate/data/__init__.py
+-rw-r--r--   0        0        0      809 2024-02-27 08:48:06.013275 olas_operate_middleware-0.1.0rc4/operate/data/contracts/__init__.py
+-rw-r--r--   0        0        0      866 2024-02-27 08:48:06.013458 olas_operate_middleware-0.1.0rc4/operate/data/contracts/service_staking_token/__init__.py
+-rw-r--r--   0        0        0    82730 2024-02-27 08:48:06.014051 olas_operate_middleware-0.1.0rc4/operate/data/contracts/service_staking_token/build/ServiceStakingToken.json
+-rw-r--r--   0        0        0     5847 2024-02-27 08:48:06.014506 olas_operate_middleware-0.1.0rc4/operate/data/contracts/service_staking_token/contract.py
+-rw-r--r--   0        0        0      724 2024-02-27 08:48:06.014716 olas_operate_middleware-0.1.0rc4/operate/data/contracts/service_staking_token/contract.yaml
+-rw-r--r--   0        0        0      868 2024-02-28 14:31:11.754886 olas_operate_middleware-0.1.0rc4/operate/data/contracts/uniswap_v2_erc20/__init__.py
+-rw-r--r--   0        0        0    14169 2024-02-28 14:31:11.755175 olas_operate_middleware-0.1.0rc4/operate/data/contracts/uniswap_v2_erc20/build/IUniswapV2ERC20.json
+-rw-r--r--   0        0        0     6985 2024-03-08 10:47:59.400374 olas_operate_middleware-0.1.0rc4/operate/data/contracts/uniswap_v2_erc20/contract.py
+-rw-r--r--   0        0        0      741 2024-02-28 14:31:11.755543 olas_operate_middleware-0.1.0rc4/operate/data/contracts/uniswap_v2_erc20/contract.yaml
+-rw-r--r--   0        0        0     4646 2024-03-14 12:31:10.592254 olas_operate_middleware-0.1.0rc4/operate/http/__init__.py
+-rw-r--r--   0        0        0     1232 2024-02-27 08:48:06.014903 olas_operate_middleware-0.1.0rc4/operate/http/exceptions.py
+-rw-r--r--   0        0        0     2809 2024-03-27 11:16:42.979679 olas_operate_middleware-0.1.0rc4/operate/keys.py
+-rw-r--r--   0        0        0     2883 2024-04-16 04:14:40.060498 olas_operate_middleware-0.1.0rc4/operate/ledger/__init__.py
+-rw-r--r--   0        0        0     1154 2024-03-08 10:47:59.401479 olas_operate_middleware-0.1.0rc4/operate/ledger/base.py
+-rw-r--r--   0        0        0     1510 2024-03-08 10:47:59.401635 olas_operate_middleware-0.1.0rc4/operate/ledger/ethereum.py
+-rw-r--r--   0        0        0     1610 2024-03-08 10:47:59.401789 olas_operate_middleware-0.1.0rc4/operate/ledger/profiles.py
+-rw-r--r--   0        0        0     1199 2024-03-08 10:47:59.401953 olas_operate_middleware-0.1.0rc4/operate/ledger/solana.py
+-rw-r--r--   0        0        0     3880 2024-04-05 14:54:43.350296 olas_operate_middleware-0.1.0rc4/operate/resource.py
+-rw-r--r--   0        0        0      855 2024-03-27 11:16:42.980219 olas_operate_middleware-0.1.0rc4/operate/services/__init__.py
+-rw-r--r--   0        0        0    16425 2024-04-11 14:01:32.695097 olas_operate_middleware-0.1.0rc4/operate/services/manage.py
+-rw-r--r--   0        0        0    21677 2024-04-05 14:54:43.352503 olas_operate_middleware-0.1.0rc4/operate/services/protocol.py
+-rw-r--r--   0        0        0    13695 2024-04-16 04:14:40.061038 olas_operate_middleware-0.1.0rc4/operate/services/service.py
+-rw-r--r--   0        0        0     5357 2024-04-05 14:54:43.352823 olas_operate_middleware-0.1.0rc4/operate/types.py
+-rw-r--r--   0        0        0      808 2024-04-05 14:54:43.353285 olas_operate_middleware-0.1.0rc4/operate/utils/__init__.py
+-rw-r--r--   0        0        0     6082 2024-04-05 14:54:43.353744 olas_operate_middleware-0.1.0rc4/operate/utils/gnosis.py
+-rw-r--r--   0        0        0      813 2024-04-05 14:54:43.353950 olas_operate_middleware-0.1.0rc4/operate/wallet/__init__.py
+-rw-r--r--   0        0        0     8662 2024-04-15 16:15:46.952707 olas_operate_middleware-0.1.0rc4/operate/wallet/master.py
+-rw-r--r--   0        0        0      818 2024-04-16 04:17:39.321459 olas_operate_middleware-0.1.0rc4/pyproject.toml
+-rw-r--r--   0        0        0     5122 1970-01-01 00:00:00.000000 olas_operate_middleware-0.1.0rc4/PKG-INFO
```

### Comparing `olas_operate_middleware-0.1.0rc3/LICENSE` & `olas_operate_middleware-0.1.0rc4/LICENSE`

 * *Files identical despite different names*

### Comparing `olas_operate_middleware-0.1.0rc3/README.md` & `olas_operate_middleware-0.1.0rc4/README.md`

 * *Files identical despite different names*

### Comparing `olas_operate_middleware-0.1.0rc3/operate/__init__.py` & `olas_operate_middleware-0.1.0rc4/operate/__init__.py`

 * *Files identical despite different names*

### Comparing `olas_operate_middleware-0.1.0rc3/operate/account/__init__.py` & `olas_operate_middleware-0.1.0rc4/operate/account/__init__.py`

 * *Files identical despite different names*

### Comparing `olas_operate_middleware-0.1.0rc3/operate/account/user.py` & `olas_operate_middleware-0.1.0rc4/operate/account/user.py`

 * *Files identical despite different names*

### Comparing `olas_operate_middleware-0.1.0rc3/operate/cli.py` & `olas_operate_middleware-0.1.0rc4/operate/cli.py`

 * *Files 0% similar despite different names*

```diff
@@ -432,29 +432,29 @@
         deployment = (
             operate.service_manager()
             .create_or_load(
                 request.path_params["service"],
             )
             .deployment
         )
-        deployment.build(force=False)
+        deployment.build(force=True)
         return JSONResponse(content=deployment.json)
 
     @app.post("/api/services/{service}/deployment/start")
     @with_retries
     async def _start_service_locally(request: Request) -> JSONResponse:
         """Create a service."""
         deployment = (
             operate.service_manager()
             .create_or_load(
                 request.path_params["service"],
             )
             .deployment
         )
-        deployment.build(force=False)
+        deployment.build(force=True)
         operate.service_manager().fund_service(hash=request.path_params["service"])
         deployment.start()
         return JSONResponse(content=deployment.json)
 
     @app.post("/api/services/{service}/deployment/stop")
     @with_retries
     async def _stop_service_locally(request: Request) -> JSONResponse:
```

### Comparing `olas_operate_middleware-0.1.0rc3/operate/constants.py` & `olas_operate_middleware-0.1.0rc4/operate/constants.py`

 * *Files identical despite different names*

### Comparing `olas_operate_middleware-0.1.0rc3/operate/data/__init__.py` & `olas_operate_middleware-0.1.0rc4/operate/data/__init__.py`

 * *Files identical despite different names*

### Comparing `olas_operate_middleware-0.1.0rc3/operate/data/contracts/__init__.py` & `olas_operate_middleware-0.1.0rc4/operate/data/contracts/__init__.py`

 * *Files identical despite different names*

### Comparing `olas_operate_middleware-0.1.0rc3/operate/data/contracts/service_staking_token/__init__.py` & `olas_operate_middleware-0.1.0rc4/operate/data/contracts/service_staking_token/__init__.py`

 * *Files identical despite different names*

### Comparing `olas_operate_middleware-0.1.0rc3/operate/data/contracts/service_staking_token/build/ServiceStakingToken.json` & `olas_operate_middleware-0.1.0rc4/operate/data/contracts/service_staking_token/build/ServiceStakingToken.json`

 * *Files identical despite different names*

### Comparing `olas_operate_middleware-0.1.0rc3/operate/data/contracts/service_staking_token/contract.py` & `olas_operate_middleware-0.1.0rc4/operate/data/contracts/service_staking_token/contract.py`

 * *Files identical despite different names*

### Comparing `olas_operate_middleware-0.1.0rc3/operate/data/contracts/service_staking_token/contract.yaml` & `olas_operate_middleware-0.1.0rc4/operate/data/contracts/service_staking_token/contract.yaml`

 * *Files identical despite different names*

### Comparing `olas_operate_middleware-0.1.0rc3/operate/data/contracts/uniswap_v2_erc20/__init__.py` & `olas_operate_middleware-0.1.0rc4/operate/data/contracts/uniswap_v2_erc20/__init__.py`

 * *Files identical despite different names*

### Comparing `olas_operate_middleware-0.1.0rc3/operate/data/contracts/uniswap_v2_erc20/build/IUniswapV2ERC20.json` & `olas_operate_middleware-0.1.0rc4/operate/data/contracts/uniswap_v2_erc20/build/IUniswapV2ERC20.json`

 * *Files identical despite different names*

### Comparing `olas_operate_middleware-0.1.0rc3/operate/data/contracts/uniswap_v2_erc20/contract.py` & `olas_operate_middleware-0.1.0rc4/operate/data/contracts/uniswap_v2_erc20/contract.py`

 * *Files identical despite different names*

### Comparing `olas_operate_middleware-0.1.0rc3/operate/data/contracts/uniswap_v2_erc20/contract.yaml` & `olas_operate_middleware-0.1.0rc4/operate/data/contracts/uniswap_v2_erc20/contract.yaml`

 * *Files identical despite different names*

### Comparing `olas_operate_middleware-0.1.0rc3/operate/http/__init__.py` & `olas_operate_middleware-0.1.0rc4/operate/http/__init__.py`

 * *Files identical despite different names*

### Comparing `olas_operate_middleware-0.1.0rc3/operate/http/exceptions.py` & `olas_operate_middleware-0.1.0rc4/operate/http/exceptions.py`

 * *Files identical despite different names*

### Comparing `olas_operate_middleware-0.1.0rc3/operate/keys.py` & `olas_operate_middleware-0.1.0rc4/operate/keys.py`

 * *Files identical despite different names*

### Comparing `olas_operate_middleware-0.1.0rc3/operate/ledger/__init__.py` & `olas_operate_middleware-0.1.0rc4/operate/ledger/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -25,15 +25,17 @@
 from operate.ledger.base import LedgerHelper
 from operate.ledger.ethereum import Ethereum
 from operate.ledger.solana import Solana
 from operate.types import ChainType, LedgerType
 
 
 ETHEREUM_RPC = os.environ.get("DEV_RPC", "https://ethereum.publicnode.com")
-GNOSIS_RPC = os.environ.get("DEV_RPC", "https://rpc.gnosischain.com")
+GNOSIS_RPC = os.environ.get(
+    "DEV_RPC", "https://go.getblock.io/2a1fa1ade5d547ca86eab099c35ce2a7"
+)
 GOERLI_RPC = os.environ.get("DEV_RPC", "https://ethereum-goerli.publicnode.com")
 SOLANA_RPC = os.environ.get("DEV_RPC", "https://api.mainnet-beta.solana.com")
 
 
 DEFAULT_RPCS = {
     ChainType.ETHEREUM: ETHEREUM_RPC,
     ChainType.GNOSIS: GNOSIS_RPC,
```

### Comparing `olas_operate_middleware-0.1.0rc3/operate/ledger/base.py` & `olas_operate_middleware-0.1.0rc4/operate/ledger/base.py`

 * *Files identical despite different names*

### Comparing `olas_operate_middleware-0.1.0rc3/operate/ledger/ethereum.py` & `olas_operate_middleware-0.1.0rc4/operate/ledger/ethereum.py`

 * *Files identical despite different names*

### Comparing `olas_operate_middleware-0.1.0rc3/operate/ledger/profiles.py` & `olas_operate_middleware-0.1.0rc4/operate/ledger/profiles.py`

 * *Files identical despite different names*

### Comparing `olas_operate_middleware-0.1.0rc3/operate/ledger/solana.py` & `olas_operate_middleware-0.1.0rc4/operate/ledger/solana.py`

 * *Files identical despite different names*

### Comparing `olas_operate_middleware-0.1.0rc3/operate/resource.py` & `olas_operate_middleware-0.1.0rc4/operate/resource.py`

 * *Files identical despite different names*

### Comparing `olas_operate_middleware-0.1.0rc3/operate/services/__init__.py` & `olas_operate_middleware-0.1.0rc4/operate/services/__init__.py`

 * *Files identical despite different names*

### Comparing `olas_operate_middleware-0.1.0rc3/operate/services/manage.py` & `olas_operate_middleware-0.1.0rc4/operate/services/manage.py`

 * *Files identical despite different names*

### Comparing `olas_operate_middleware-0.1.0rc3/operate/services/protocol.py` & `olas_operate_middleware-0.1.0rc4/operate/services/protocol.py`

 * *Files identical despite different names*

### Comparing `olas_operate_middleware-0.1.0rc3/operate/services/service.py` & `olas_operate_middleware-0.1.0rc4/operate/services/service.py`

 * *Files 1% similar despite different names*

```diff
@@ -230,15 +230,25 @@
             return
         if build.exists() and force:
             shutil.rmtree(build)
         mkdirs(build_dir=build)
 
         keys_file = self.path / KEYS_JSON
         keys_file.write_text(
-            json.dumps([key.json for key in service.keys], indent=4),
+            json.dumps(
+                [
+                    {
+                        "address": key.address,
+                        "private_key": key.private_key,
+                        "ledger": key.ledger.name.lower(),
+                    }
+                    for key in service.keys
+                ],
+                indent=4,
+            ),
             encoding="utf-8",
         )
         try:
             builder = ServiceBuilder.from_dir(
                 path=service.service_path,
                 keys_file=keys_file,
                 number_of_agents=len(service.keys),
```

### Comparing `olas_operate_middleware-0.1.0rc3/operate/types.py` & `olas_operate_middleware-0.1.0rc4/operate/types.py`

 * *Files identical despite different names*

### Comparing `olas_operate_middleware-0.1.0rc3/operate/utils/__init__.py` & `olas_operate_middleware-0.1.0rc4/operate/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `olas_operate_middleware-0.1.0rc3/operate/utils/gnosis.py` & `olas_operate_middleware-0.1.0rc4/operate/utils/gnosis.py`

 * *Files identical despite different names*

### Comparing `olas_operate_middleware-0.1.0rc3/operate/wallet/__init__.py` & `olas_operate_middleware-0.1.0rc4/operate/wallet/__init__.py`

 * *Files identical despite different names*

### Comparing `olas_operate_middleware-0.1.0rc3/operate/wallet/master.py` & `olas_operate_middleware-0.1.0rc4/operate/wallet/master.py`

 * *Files identical despite different names*

### Comparing `olas_operate_middleware-0.1.0rc3/pyproject.toml` & `olas_operate_middleware-0.1.0rc4/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "olas-operate-middleware"
-version = "0.1.0-rc3"
+version = "0.1.0-rc4"
 description = ""
 authors = ["David Vilela <dvilelaf@gmail.com>", "Viraj Patel <vptl185@gmail.com>"]
 readme = "README.md"
 packages = [
     { include = "operate" }
 ]
 include = [
@@ -23,11 +23,12 @@
 open-aea-ledger-ethereum = ">=1.50.0"
 docker = "6.1.2"
 clea = ">=0.1.0rc4"
 starlette = ">=0.36.3"
 uvicorn = ">=0.27.0"
 requests-toolbelt = "1.0.0"
 fastapi = ">=0.110.0"
+web3 = "6.1.0"
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `olas_operate_middleware-0.1.0rc3/PKG-INFO` & `olas_operate_middleware-0.1.0rc4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: olas-operate-middleware
-Version: 0.1.0rc3
+Version: 0.1.0rc4
 Summary: 
 Author: David Vilela
 Author-email: dvilelaf@gmail.com
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
@@ -15,14 +15,15 @@
 Requires-Dist: docker (==6.1.2)
 Requires-Dist: fastapi (>=0.110.0)
 Requires-Dist: open-aea-ledger-ethereum (>=1.50.0)
 Requires-Dist: open-autonomy (>=0.14.10)
 Requires-Dist: requests-toolbelt (==1.0.0)
 Requires-Dist: starlette (>=0.36.3)
 Requires-Dist: uvicorn (>=0.27.0)
+Requires-Dist: web3 (==6.1.0)
 Description-Content-Type: text/markdown
 
 # Olas Operate
 Electron + NextJS + Python Backend application to one-click run Agents.
 
 ## Technologies Used
 - Electron
```

