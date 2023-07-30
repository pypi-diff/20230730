# Comparing `tmp/empiric_network-1.6.8.tar.gz` & `tmp/empiric_network-1.6.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "empiric_network-1.6.8.tar", max compression
+gzip compressed data, was "empiric_network-1.6.9.tar", max compression
```

## Comparing `empiric_network-1.6.8.tar` & `empiric_network-1.6.9.tar`

### file list

```diff
@@ -1,47 +1,47 @@
--rw-r--r--   0        0        0      284 2023-07-27 17:59:52.841356 empiric_network-1.6.8/README.md
--rw-r--r--   0        0        0        0 2023-07-27 17:59:52.841356 empiric_network-1.6.8/empiric/__init__.py
--rw-r--r--   0        0        0      193 2023-07-27 17:59:52.841356 empiric_network-1.6.8/empiric/core/__init__.py
--rw-r--r--   0        0        0      284 2023-07-27 17:59:52.841356 empiric_network-1.6.8/empiric/core/abis/__init__.py
--rw-r--r--   0        0        0    31179 2023-07-27 17:59:52.841356 empiric_network-1.6.8/empiric/core/abis/oracle.py
--rw-r--r--   0        0        0     1436 2023-07-27 17:59:52.841356 empiric_network-1.6.8/empiric/core/abis/proxy.py
--rw-r--r--   0        0        0     3896 2023-07-27 17:59:52.841356 empiric_network-1.6.8/empiric/core/abis/publisher_registry.py
--rw-r--r--   0        0        0     5912 2023-07-27 17:59:52.841356 empiric_network-1.6.8/empiric/core/abis/randomness.py
--rw-r--r--   0        0        0      868 2023-07-27 17:59:52.841356 empiric_network-1.6.8/empiric/core/abis/summary_stats.py
--rw-r--r--   0        0        0     4257 2023-07-27 17:59:52.841356 empiric_network-1.6.8/empiric/core/client.py
--rw-r--r--   0        0        0     2618 2023-07-27 17:59:52.841356 empiric_network-1.6.8/empiric/core/config.py
--rw-r--r--   0        0        0     3922 2023-07-27 17:59:52.841356 empiric_network-1.6.8/empiric/core/contract.py
--rw-r--r--   0        0        0    10045 2023-07-27 17:59:52.841356 empiric_network-1.6.8/empiric/core/entry.py
--rw-r--r--   0        0        0      387 2023-07-27 17:59:52.841356 empiric_network-1.6.8/empiric/core/logger.py
--rw-r--r--   0        0        0      295 2023-07-27 17:59:52.841356 empiric_network-1.6.8/empiric/core/mixins/__init__.py
--rw-r--r--   0        0        0    25441 2023-07-27 17:59:52.841356 empiric_network-1.6.8/empiric/core/mixins/evm.py
--rw-r--r--   0        0        0     3074 2023-07-27 17:59:52.841356 empiric_network-1.6.8/empiric/core/mixins/nonce.py
--rw-r--r--   0        0        0     9442 2023-07-27 17:59:52.841356 empiric_network-1.6.8/empiric/core/mixins/oracle.py
--rw-r--r--   0        0        0     2287 2023-07-27 17:59:52.841356 empiric_network-1.6.8/empiric/core/mixins/publisher_registry.py
--rw-r--r--   0        0        0     3065 2023-07-27 17:59:52.841356 empiric_network-1.6.8/empiric/core/mixins/randomness.py
--rw-r--r--   0        0        0      669 2023-07-27 17:59:52.841356 empiric_network-1.6.8/empiric/core/mixins/transactions.py
--rw-r--r--   0        0        0     4177 2023-07-27 17:59:52.841356 empiric_network-1.6.8/empiric/core/types.py
--rw-r--r--   0        0        0      880 2023-07-27 17:59:52.841356 empiric_network-1.6.8/empiric/core/utils.py
--rw-r--r--   0        0        0       82 2023-07-27 17:59:52.841356 empiric_network-1.6.8/empiric/publisher/__init__.py
--rw-r--r--   0        0        0     3368 2023-07-27 17:59:52.841356 empiric_network-1.6.8/empiric/publisher/assets.py
--rw-r--r--   0        0        0     2262 2023-07-27 17:59:52.841356 empiric_network-1.6.8/empiric/publisher/client.py
--rw-r--r--   0        0        0      354 2023-07-27 17:59:52.841356 empiric_network-1.6.8/empiric/publisher/fetchers/__init__.py
--rw-r--r--   0        0        0     3755 2023-07-27 17:59:52.841356 empiric_network-1.6.8/empiric/publisher/fetchers/ascendex.py
--rw-r--r--   0        0        0     3017 2023-07-27 17:59:52.841356 empiric_network-1.6.8/empiric/publisher/fetchers/bitstamp.py
--rw-r--r--   0        0        0     3380 2023-07-27 17:59:52.841356 empiric_network-1.6.8/empiric/publisher/fetchers/cex.py
--rw-r--r--   0        0        0     2953 2023-07-27 17:59:52.841356 empiric_network-1.6.8/empiric/publisher/fetchers/coinbase.py
--rw-r--r--   0        0        0     3980 2023-07-27 17:59:52.841356 empiric_network-1.6.8/empiric/publisher/fetchers/coingecko.py
--rw-r--r--   0        0        0     3826 2023-07-27 17:59:52.841356 empiric_network-1.6.8/empiric/publisher/fetchers/defillama.py
--rw-r--r--   0        0        0     3814 2023-07-27 17:59:52.841356 empiric_network-1.6.8/empiric/publisher/fetchers/gemini.py
--rw-r--r--   0        0        0     3754 2023-07-27 17:59:52.841356 empiric_network-1.6.8/empiric/publisher/fetchers/kaiko.py
--rw-r--r--   0        0        0     3631 2023-07-27 17:59:52.841356 empiric_network-1.6.8/empiric/publisher/fetchers/okx.py
--rw-r--r--   0        0        0     3762 2023-07-27 17:59:52.845356 empiric_network-1.6.8/empiric/publisher/fetchers/thegraph.py
--rw-r--r--   0        0        0      113 2023-07-27 17:59:52.845356 empiric_network-1.6.8/empiric/publisher/future_fetchers/__init__.py
--rw-r--r--   0        0        0     6306 2023-07-27 17:59:52.845356 empiric_network-1.6.8/empiric/publisher/future_fetchers/binance.py
--rw-r--r--   0        0        0     3791 2023-07-27 17:59:52.845356 empiric_network-1.6.8/empiric/publisher/future_fetchers/bybit.py
--rw-r--r--   0        0        0     6647 2023-07-27 17:59:52.845356 empiric_network-1.6.8/empiric/publisher/future_fetchers/okx.py
--rw-r--r--   0        0        0     4282 2023-07-27 17:59:52.845356 empiric_network-1.6.8/empiric/publisher/future_fetchers/test.py
--rw-r--r--   0        0        0      668 2023-07-27 17:59:52.845356 empiric_network-1.6.8/empiric/publisher/types.py
--rw-r--r--   0        0        0        0 2023-07-27 17:59:52.845356 empiric_network-1.6.8/empiric/test/__init__.py
--rw-r--r--   0        0        0     5965 2023-07-27 17:59:52.845356 empiric_network-1.6.8/empiric/test/interface_consistency.py
--rw-r--r--   0        0        0     1016 2023-07-27 17:59:52.845356 empiric_network-1.6.8/pyproject.toml
--rw-r--r--   0        0        0     1038 1970-01-01 00:00:00.000000 empiric_network-1.6.8/PKG-INFO
+-rw-r--r--   0        0        0      284 2023-07-30 13:29:10.491216 empiric_network-1.6.9/README.md
+-rw-r--r--   0        0        0        0 2023-07-30 13:29:10.491216 empiric_network-1.6.9/empiric/__init__.py
+-rw-r--r--   0        0        0      193 2023-07-30 13:29:10.491216 empiric_network-1.6.9/empiric/core/__init__.py
+-rw-r--r--   0        0        0      284 2023-07-30 13:29:10.491216 empiric_network-1.6.9/empiric/core/abis/__init__.py
+-rw-r--r--   0        0        0    31179 2023-07-30 13:29:10.491216 empiric_network-1.6.9/empiric/core/abis/oracle.py
+-rw-r--r--   0        0        0     1436 2023-07-30 13:29:10.491216 empiric_network-1.6.9/empiric/core/abis/proxy.py
+-rw-r--r--   0        0        0     3896 2023-07-30 13:29:10.491216 empiric_network-1.6.9/empiric/core/abis/publisher_registry.py
+-rw-r--r--   0        0        0     5912 2023-07-30 13:29:10.491216 empiric_network-1.6.9/empiric/core/abis/randomness.py
+-rw-r--r--   0        0        0      868 2023-07-30 13:29:10.491216 empiric_network-1.6.9/empiric/core/abis/summary_stats.py
+-rw-r--r--   0        0        0     4257 2023-07-30 13:29:10.491216 empiric_network-1.6.9/empiric/core/client.py
+-rw-r--r--   0        0        0     2618 2023-07-30 13:29:10.491216 empiric_network-1.6.9/empiric/core/config.py
+-rw-r--r--   0        0        0     3922 2023-07-30 13:29:10.491216 empiric_network-1.6.9/empiric/core/contract.py
+-rw-r--r--   0        0        0    10045 2023-07-30 13:29:10.491216 empiric_network-1.6.9/empiric/core/entry.py
+-rw-r--r--   0        0        0      387 2023-07-30 13:29:10.491216 empiric_network-1.6.9/empiric/core/logger.py
+-rw-r--r--   0        0        0      295 2023-07-30 13:29:10.491216 empiric_network-1.6.9/empiric/core/mixins/__init__.py
+-rw-r--r--   0        0        0    25441 2023-07-30 13:29:10.491216 empiric_network-1.6.9/empiric/core/mixins/evm.py
+-rw-r--r--   0        0        0     3074 2023-07-30 13:29:10.491216 empiric_network-1.6.9/empiric/core/mixins/nonce.py
+-rw-r--r--   0        0        0    10871 2023-07-30 13:29:10.491216 empiric_network-1.6.9/empiric/core/mixins/oracle.py
+-rw-r--r--   0        0        0     2287 2023-07-30 13:29:10.491216 empiric_network-1.6.9/empiric/core/mixins/publisher_registry.py
+-rw-r--r--   0        0        0     3065 2023-07-30 13:29:10.491216 empiric_network-1.6.9/empiric/core/mixins/randomness.py
+-rw-r--r--   0        0        0      669 2023-07-30 13:29:10.491216 empiric_network-1.6.9/empiric/core/mixins/transactions.py
+-rw-r--r--   0        0        0     4177 2023-07-30 13:29:10.491216 empiric_network-1.6.9/empiric/core/types.py
+-rw-r--r--   0        0        0      880 2023-07-30 13:29:10.491216 empiric_network-1.6.9/empiric/core/utils.py
+-rw-r--r--   0        0        0       82 2023-07-30 13:29:10.491216 empiric_network-1.6.9/empiric/publisher/__init__.py
+-rw-r--r--   0        0        0     3708 2023-07-30 13:29:10.491216 empiric_network-1.6.9/empiric/publisher/assets.py
+-rw-r--r--   0        0        0     2262 2023-07-30 13:29:10.491216 empiric_network-1.6.9/empiric/publisher/client.py
+-rw-r--r--   0        0        0      354 2023-07-30 13:29:10.491216 empiric_network-1.6.9/empiric/publisher/fetchers/__init__.py
+-rw-r--r--   0        0        0     3755 2023-07-30 13:29:10.491216 empiric_network-1.6.9/empiric/publisher/fetchers/ascendex.py
+-rw-r--r--   0        0        0     3017 2023-07-30 13:29:10.491216 empiric_network-1.6.9/empiric/publisher/fetchers/bitstamp.py
+-rw-r--r--   0        0        0     3380 2023-07-30 13:29:10.491216 empiric_network-1.6.9/empiric/publisher/fetchers/cex.py
+-rw-r--r--   0        0        0     2953 2023-07-30 13:29:10.491216 empiric_network-1.6.9/empiric/publisher/fetchers/coinbase.py
+-rw-r--r--   0        0        0     3980 2023-07-30 13:29:10.491216 empiric_network-1.6.9/empiric/publisher/fetchers/coingecko.py
+-rw-r--r--   0        0        0     3826 2023-07-30 13:29:10.491216 empiric_network-1.6.9/empiric/publisher/fetchers/defillama.py
+-rw-r--r--   0        0        0     3814 2023-07-30 13:29:10.491216 empiric_network-1.6.9/empiric/publisher/fetchers/gemini.py
+-rw-r--r--   0        0        0     3754 2023-07-30 13:29:10.491216 empiric_network-1.6.9/empiric/publisher/fetchers/kaiko.py
+-rw-r--r--   0        0        0     3631 2023-07-30 13:29:10.491216 empiric_network-1.6.9/empiric/publisher/fetchers/okx.py
+-rw-r--r--   0        0        0     3762 2023-07-30 13:29:10.491216 empiric_network-1.6.9/empiric/publisher/fetchers/thegraph.py
+-rw-r--r--   0        0        0      113 2023-07-30 13:29:10.491216 empiric_network-1.6.9/empiric/publisher/future_fetchers/__init__.py
+-rw-r--r--   0        0        0     6306 2023-07-30 13:29:10.491216 empiric_network-1.6.9/empiric/publisher/future_fetchers/binance.py
+-rw-r--r--   0        0        0     3791 2023-07-30 13:29:10.491216 empiric_network-1.6.9/empiric/publisher/future_fetchers/bybit.py
+-rw-r--r--   0        0        0     6647 2023-07-30 13:29:10.491216 empiric_network-1.6.9/empiric/publisher/future_fetchers/okx.py
+-rw-r--r--   0        0        0     4282 2023-07-30 13:29:10.491216 empiric_network-1.6.9/empiric/publisher/future_fetchers/test.py
+-rw-r--r--   0        0        0      668 2023-07-30 13:29:10.491216 empiric_network-1.6.9/empiric/publisher/types.py
+-rw-r--r--   0        0        0        0 2023-07-30 13:29:10.491216 empiric_network-1.6.9/empiric/test/__init__.py
+-rw-r--r--   0        0        0     5965 2023-07-30 13:29:10.491216 empiric_network-1.6.9/empiric/test/interface_consistency.py
+-rw-r--r--   0        0        0     1016 2023-07-30 13:29:10.491216 empiric_network-1.6.9/pyproject.toml
+-rw-r--r--   0        0        0     1038 1970-01-01 00:00:00.000000 empiric_network-1.6.9/PKG-INFO
```

### Comparing `empiric_network-1.6.8/empiric/core/abis/oracle.py` & `empiric_network-1.6.9/empiric/core/abis/oracle.py`

 * *Files identical despite different names*

### Comparing `empiric_network-1.6.8/empiric/core/abis/proxy.py` & `empiric_network-1.6.9/empiric/core/abis/proxy.py`

 * *Files identical despite different names*

### Comparing `empiric_network-1.6.8/empiric/core/abis/publisher_registry.py` & `empiric_network-1.6.9/empiric/core/abis/publisher_registry.py`

 * *Files identical despite different names*

### Comparing `empiric_network-1.6.8/empiric/core/abis/randomness.py` & `empiric_network-1.6.9/empiric/core/abis/randomness.py`

 * *Files identical despite different names*

### Comparing `empiric_network-1.6.8/empiric/core/abis/summary_stats.py` & `empiric_network-1.6.9/empiric/core/abis/summary_stats.py`

 * *Files identical despite different names*

### Comparing `empiric_network-1.6.8/empiric/core/client.py` & `empiric_network-1.6.9/empiric/core/client.py`

 * *Files identical despite different names*

### Comparing `empiric_network-1.6.8/empiric/core/config.py` & `empiric_network-1.6.9/empiric/core/config.py`

 * *Files identical despite different names*

### Comparing `empiric_network-1.6.8/empiric/core/contract.py` & `empiric_network-1.6.9/empiric/core/contract.py`

 * *Files identical despite different names*

### Comparing `empiric_network-1.6.8/empiric/core/entry.py` & `empiric_network-1.6.9/empiric/core/entry.py`

 * *Files identical despite different names*

### Comparing `empiric_network-1.6.8/empiric/core/mixins/evm.py` & `empiric_network-1.6.9/empiric/core/mixins/evm.py`

 * *Files identical despite different names*

### Comparing `empiric_network-1.6.8/empiric/core/mixins/nonce.py` & `empiric_network-1.6.9/empiric/core/mixins/nonce.py`

 * *Files identical despite different names*

### Comparing `empiric_network-1.6.8/empiric/core/mixins/oracle.py` & `empiric_network-1.6.9/empiric/core/mixins/oracle.py`

 * *Files 3% similar despite different names*

```diff
@@ -229,14 +229,53 @@
             pair_id,
             expiry_timestamp,
             aggregation_mode,
             max_fee=max_fee,
         )
         return invocation
 
+    async def set_future_checkpoints(
+        self,
+        pair_ids: List[int],
+        expiry_timestamps: List[int],
+        aggregation_mode: int = str_to_felt("MEDIAN"),
+        max_fee=int(1e16),
+        pagination: Optional[int] = 15,
+    ) -> InvokeResult:
+        if not self.is_user_client:
+            raise AttributeError(
+                "Must set account.  You may do this by invoking self._setup_account_client(private_key, account_contract_address)"
+            )
+
+        if pagination:
+            ix = 0
+            while ix < len(pair_ids):
+                pair_ids_subset = pair_ids[ix : ix + pagination]
+                invocation = await self.oracle.set_future_checkpoints.invoke(
+                    pair_ids_subset,
+                    expiry_timestamps,
+                    aggregation_mode,
+                    callback=self.track_nonce,
+                    max_fee=max_fee,
+                )
+                ix += pagination
+                logger.debug(str(invocation))
+                logger.info(
+                    f"Set future checkpoints for {len(pair_ids_subset)} pair IDs with transaction {hex(invocation.hash)}"
+                )
+        else:
+            invocation = await self.oracle.set_future_checkpoints.invoke(
+                pair_ids,
+                expiry_timestamps,
+                aggregation_mode,
+                max_fee=max_fee,
+            )
+
+        return invocation
+
     async def set_checkpoints(
         self,
         pair_ids: List[int],
         aggregation_mode: int = str_to_felt("MEDIAN"),
         max_fee=int(1e18),
         pagination: Optional[int] = 15,
     ) -> InvokeResult:
@@ -247,24 +286,24 @@
         if pagination:
             ix = 0
             while ix < len(pair_ids):
                 pair_ids_subset = pair_ids[ix : ix + pagination]
                 invocation = await self.oracle.set_checkpoints.invoke(
                     pair_ids_subset,
                     aggregation_mode,
-                    callback=self.track_nonce,
+                    # callback=self.track_nonce,
                     max_fee=max_fee,
                 )
                 ix += pagination
                 logger.debug(str(invocation))
                 logger.info(
                     f"Set checkpoints for {len(pair_ids_subset)} pair IDs with transaction {hex(invocation.hash)}"
                 )
         else:
             invocation = await self.oracle.set_checkpoints.invoke(
                 pair_ids,
                 aggregation_mode,
-                callback=self.track_nonce,
+                # callback=self.track_nonce,
                 max_fee=max_fee,
             )
 
         return invocation
```

### Comparing `empiric_network-1.6.8/empiric/core/mixins/publisher_registry.py` & `empiric_network-1.6.9/empiric/core/mixins/publisher_registry.py`

 * *Files identical despite different names*

### Comparing `empiric_network-1.6.8/empiric/core/mixins/randomness.py` & `empiric_network-1.6.9/empiric/core/mixins/randomness.py`

 * *Files identical despite different names*

### Comparing `empiric_network-1.6.8/empiric/core/mixins/transactions.py` & `empiric_network-1.6.9/empiric/core/mixins/transactions.py`

 * *Files identical despite different names*

### Comparing `empiric_network-1.6.8/empiric/core/types.py` & `empiric_network-1.6.9/empiric/core/types.py`

 * *Files identical despite different names*

### Comparing `empiric_network-1.6.8/empiric/core/utils.py` & `empiric_network-1.6.9/empiric/core/utils.py`

 * *Files identical despite different names*

### Comparing `empiric_network-1.6.8/empiric/publisher/assets.py` & `empiric_network-1.6.9/empiric/publisher/assets.py`

 * *Files 11% similar despite different names*

```diff
@@ -79,17 +79,27 @@
 
 _EMPIRIC_FUTURE_ASSET_BY_KEY: Dict[str, EmpiricFutureAsset] = {
     key_for_asset(asset): asset
     for asset in EMPIRIC_ALL_ASSETS
     if asset["type"] == "FUTURE"
 }
 
+_EMPIRIC_ALL_ASSET_BY_KEY: Dict[str, EmpiricAsset] ={
+    key_for_asset(asset): asset
+    for asset in EMPIRIC_ALL_ASSETS
+}
+
 
 def get_spot_asset_spec_for_pair_id(pair_id: str) -> EmpiricSpotAsset:
     if pair_id not in _EMPIRIC_ASSET_BY_KEY:
         raise ValueError(f"Pair ID not found: {pair_id}")
     return _EMPIRIC_ASSET_BY_KEY[pair_id]
 
 def get_future_asset_spec_for_pair_id(pair_id: str) -> EmpiricFutureAsset:
     if pair_id not in _EMPIRIC_FUTURE_ASSET_BY_KEY:
         raise ValueError(f"Pair ID not found: {pair_id}")
     return _EMPIRIC_FUTURE_ASSET_BY_KEY[pair_id]
+
+def get_asset_spec_for_pair_id(pair_id: str) -> EmpiricAsset:
+    if pair_id not in _EMPIRIC_ALL_ASSET_BY_KEY:
+        raise ValueError(f"Pair ID not found: {pair_id}")
+    return _EMPIRIC_ALL_ASSET_BY_KEY[pair_id]
```

### Comparing `empiric_network-1.6.8/empiric/publisher/client.py` & `empiric_network-1.6.9/empiric/publisher/client.py`

 * *Files identical despite different names*

### Comparing `empiric_network-1.6.8/empiric/publisher/fetchers/ascendex.py` & `empiric_network-1.6.9/empiric/publisher/fetchers/ascendex.py`

 * *Files identical despite different names*

### Comparing `empiric_network-1.6.8/empiric/publisher/fetchers/bitstamp.py` & `empiric_network-1.6.9/empiric/publisher/fetchers/bitstamp.py`

 * *Files identical despite different names*

### Comparing `empiric_network-1.6.8/empiric/publisher/fetchers/cex.py` & `empiric_network-1.6.9/empiric/publisher/fetchers/cex.py`

 * *Files identical despite different names*

### Comparing `empiric_network-1.6.8/empiric/publisher/fetchers/coinbase.py` & `empiric_network-1.6.9/empiric/publisher/fetchers/coinbase.py`

 * *Files identical despite different names*

### Comparing `empiric_network-1.6.8/empiric/publisher/fetchers/coingecko.py` & `empiric_network-1.6.9/empiric/publisher/fetchers/coingecko.py`

 * *Files identical despite different names*

### Comparing `empiric_network-1.6.8/empiric/publisher/fetchers/defillama.py` & `empiric_network-1.6.9/empiric/publisher/fetchers/defillama.py`

 * *Files identical despite different names*

### Comparing `empiric_network-1.6.8/empiric/publisher/fetchers/gemini.py` & `empiric_network-1.6.9/empiric/publisher/fetchers/gemini.py`

 * *Files identical despite different names*

### Comparing `empiric_network-1.6.8/empiric/publisher/fetchers/kaiko.py` & `empiric_network-1.6.9/empiric/publisher/fetchers/kaiko.py`

 * *Files identical despite different names*

### Comparing `empiric_network-1.6.8/empiric/publisher/fetchers/okx.py` & `empiric_network-1.6.9/empiric/publisher/fetchers/okx.py`

 * *Files identical despite different names*

### Comparing `empiric_network-1.6.8/empiric/publisher/fetchers/thegraph.py` & `empiric_network-1.6.9/empiric/publisher/fetchers/thegraph.py`

 * *Files identical despite different names*

### Comparing `empiric_network-1.6.8/empiric/publisher/future_fetchers/binance.py` & `empiric_network-1.6.9/empiric/publisher/future_fetchers/binance.py`

 * *Files identical despite different names*

### Comparing `empiric_network-1.6.8/empiric/publisher/future_fetchers/bybit.py` & `empiric_network-1.6.9/empiric/publisher/future_fetchers/bybit.py`

 * *Files identical despite different names*

### Comparing `empiric_network-1.6.8/empiric/publisher/future_fetchers/okx.py` & `empiric_network-1.6.9/empiric/publisher/future_fetchers/okx.py`

 * *Files identical despite different names*

### Comparing `empiric_network-1.6.8/empiric/publisher/future_fetchers/test.py` & `empiric_network-1.6.9/empiric/publisher/future_fetchers/test.py`

 * *Files identical despite different names*

### Comparing `empiric_network-1.6.8/empiric/publisher/types.py` & `empiric_network-1.6.9/empiric/publisher/types.py`

 * *Files identical despite different names*

### Comparing `empiric_network-1.6.8/empiric/test/interface_consistency.py` & `empiric_network-1.6.9/empiric/test/interface_consistency.py`

 * *Files identical despite different names*

### Comparing `empiric_network-1.6.8/pyproject.toml` & `empiric_network-1.6.9/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 build-backend = "poetry.core.masonry.api"
 
 [tool.isort]
 profile = "black"
 
 [tool.poetry]
 name = "empiric-network"
-version = "1.6.8"
+version = "1.6.9"
 authors = ["Pragma <contact@pragmaoracle.com>"]
 description = "Core package for rollup-native Pragma Oracle"
 readme = "README.md"
 homepage = "https://pragmaoracle.com"
 repository = "https://github.com/Astraly-Labs/Pragma"
 documentation = "https://docs.pragmaoracle.com"
 classifiers = [
```

### Comparing `empiric_network-1.6.8/PKG-INFO` & `empiric_network-1.6.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: empiric-network
-Version: 1.6.8
+Version: 1.6.9
 Summary: Core package for rollup-native Pragma Oracle
 Home-page: https://pragmaoracle.com
 Author: Pragma
 Author-email: contact@pragmaoracle.com
 Requires-Python: >=3.9,<3.10
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

