# Comparing `tmp/cheb3-0.7.5.tar.gz` & `tmp/cheb3-0.7.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cheb3-0.7.5.tar", last modified: Sun Jun 11 04:38:53 2023, max compression
+gzip compressed data, was "cheb3-0.7.6.tar", last modified: Sun Jul 30 07:47:18 2023, max compression
```

## Comparing `cheb3-0.7.5.tar` & `cheb3-0.7.6.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 04:38:53.967335 cheb3-0.7.5/
--rw-r--r--   0 runner    (1001) docker     (123)     1063 2023-06-11 04:38:44.000000 cheb3-0.7.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     3001 2023-06-11 04:38:53.967335 cheb3-0.7.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2379 2023-06-11 04:38:44.000000 cheb3-0.7.5/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 04:38:53.967335 cheb3-0.7.5/cheb3/
--rw-r--r--   0 runner    (1001) docker     (123)      177 2023-06-11 04:38:44.000000 cheb3-0.7.5/cheb3/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3443 2023-06-11 04:38:44.000000 cheb3-0.7.5/cheb3/account.py
--rw-r--r--   0 runner    (1001) docker     (123)     2801 2023-06-11 04:38:44.000000 cheb3-0.7.5/cheb3/connection.py
--rw-r--r--   0 runner    (1001) docker     (123)       81 2023-06-11 04:38:44.000000 cheb3-0.7.5/cheb3/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     9400 2023-06-11 04:38:44.000000 cheb3-0.7.5/cheb3/contract.py
--rw-r--r--   0 runner    (1001) docker     (123)     9207 2023-06-11 04:38:44.000000 cheb3-0.7.5/cheb3/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 04:38:53.967335 cheb3-0.7.5/cheb3.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3001 2023-06-11 04:38:53.000000 cheb3-0.7.5/cheb3.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      283 2023-06-11 04:38:53.000000 cheb3-0.7.5/cheb3.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-11 04:38:53.000000 cheb3-0.7.5/cheb3.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       29 2023-06-11 04:38:53.000000 cheb3-0.7.5/cheb3.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-06-11 04:38:53.000000 cheb3-0.7.5/cheb3.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      734 2023-06-11 04:38:44.000000 cheb3-0.7.5/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-11 04:38:53.967335 cheb3-0.7.5/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 07:47:18.794118 cheb3-0.7.6/
+-rw-r--r--   0 runner    (1001) docker     (123)     1063 2023-07-30 07:47:08.000000 cheb3-0.7.6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      621 2023-07-30 07:47:18.794118 cheb3-0.7.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1306 2023-07-30 07:47:08.000000 cheb3-0.7.6/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 07:47:18.794118 cheb3-0.7.6/cheb3/
+-rw-r--r--   0 runner    (1001) docker     (123)      177 2023-07-30 07:47:08.000000 cheb3-0.7.6/cheb3/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3529 2023-07-30 07:47:08.000000 cheb3-0.7.6/cheb3/account.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2801 2023-07-30 07:47:08.000000 cheb3-0.7.6/cheb3/connection.py
+-rw-r--r--   0 runner    (1001) docker     (123)       81 2023-07-30 07:47:08.000000 cheb3-0.7.6/cheb3/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9400 2023-07-30 07:47:08.000000 cheb3-0.7.6/cheb3/contract.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9197 2023-07-30 07:47:08.000000 cheb3-0.7.6/cheb3/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 07:47:18.794118 cheb3-0.7.6/cheb3.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      621 2023-07-30 07:47:18.000000 cheb3-0.7.6/cheb3.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      284 2023-07-30 07:47:18.000000 cheb3-0.7.6/cheb3.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-30 07:47:18.000000 cheb3-0.7.6/cheb3.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       29 2023-07-30 07:47:18.000000 cheb3-0.7.6/cheb3.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-07-30 07:47:18.000000 cheb3-0.7.6/cheb3.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      734 2023-07-30 07:47:08.000000 cheb3-0.7.6/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-30 07:47:18.794118 cheb3-0.7.6/setup.cfg
```

### Comparing `cheb3-0.7.5/LICENSE` & `cheb3-0.7.6/LICENSE`

 * *Files identical despite different names*

### Comparing `cheb3-0.7.5/cheb3/account.py` & `cheb3-0.7.6/cheb3/account.py`

 * *Files 5% similar despite different names*

```diff
@@ -55,14 +55,16 @@
         :type to: HexStr
         :param data: The transaction data, defaults to `0x`.
         :type data: HexStr
 
         :rtype: ~hexbytes.main.HexBytes
         """
 
+        to = Web3.to_checksum_address(to)
+
         return self.w3.eth.call(
             {
                 "to": to,
                 "from": self.address,
                 "data": data,
             }
         )
@@ -80,14 +82,16 @@
         Keyword Args:
             gas_price (int): Specify the gas price for the transaction.
             gas_limit (int): Specify the maximum gas the transaction can use.
 
         :rtype: TxReceipt
         """
 
+        to = Web3.to_checksum_address(to)
+
         tx = {
             "from": self.address,
             "to": to,
             "chainId": self.w3.eth.chain_id,
             "nonce": self.w3.eth.get_transaction_count(self.address),
             "value": value,
             "gasPrice": kwargs.get("gas_price", self.w3.eth.gas_price),
```

### Comparing `cheb3-0.7.5/cheb3/connection.py` & `cheb3-0.7.6/cheb3/connection.py`

 * *Files identical despite different names*

### Comparing `cheb3-0.7.5/cheb3/contract.py` & `cheb3-0.7.6/cheb3/contract.py`

 * *Files identical despite different names*

### Comparing `cheb3-0.7.5/cheb3/utils.py` & `cheb3-0.7.6/cheb3/utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -85,21 +85,21 @@
         contracts[cn] = (
             compiled[f"<stdin>:{cn}"]["abi"],
             compiled[f"<stdin>:{cn}"]["bin"],
         )
     return contracts
 
 
-def decode_data(encoded_data: Union[HexBytes, HexStr], types: Union[str, Iterable[str]]) -> Union[Any, Tuple[Any]]:
+def decode_data(encoded_data: Union[HexBytes, HexStr], types: Iterable[str]) -> Union[Any, Tuple[Any]]:
     r"""The same as `abi.decode` in Solidity.
 
     Examples:
 
         >>> # decode a single value
-        >>> decode_data(b'\xd0!\xb0\xc3\x07\xaf\x00\x9b?\xbe\x03\x99M\xb4\xfa\x9fy\x17 \x84'.rjust(32, b'\0'), 'address')
+        >>> decode_data(b'\xd0!\xb0\xc3\x07\xaf\x00\x9b?\xbe\x03\x99M\xb4\xfa\x9fy\x17 \x84'.rjust(32, b'\0'), ['address'])
         '0xd021b0c307af009b3fbe03994db4fa9f79172084'
         >>> # decode multiple values
         >>> decode_data('000000000000000000000000000000000000000000000000058d15e17628\
         00000000000000000000000000000000000000000000000000000000000000000064000000000\
         00000000000000000000000000000000000000000000000645f7142',\
         ('uint112', 'uint112', 'uint32'))
         (400000000000000000, 100, 1683976514)
```

### Comparing `cheb3-0.7.5/pyproject.toml` & `cheb3-0.7.6/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "cheb3"
-version = "0.7.5"
+version = "0.7.6"
 authors = [{name = "YanhuiJessica",email = "y4nhv1@gmail.com"}]
 description = "Web3 CTF tool based on web3.py"
 readme = "README.md"
 requires-python = ">=3.8"
 dependencies = [
   "web3>=6.0.0",
   "py-solc-x",
```

