# Comparing `tmp/pytoniq-0.0.6.tar.gz` & `tmp/pytoniq-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/pytoniq-0.0.6.tar", last modified: Thu Jul 27 17:45:07 2023, max compression
+gzip compressed data, was "pytoniq-0.0.7.tar", last modified: Sun Jul 30 15:05:36 2023, max compression
```

## Comparing `pytoniq-0.0.6.tar` & `pytoniq-0.0.7.tar`

### file list

```diff
@@ -1,77 +1,77 @@
-drwxr-xr-x   0 maxankurb   (501) staff       (20)        0 2023-07-27 17:45:07.344945 pytoniq-0.0.6/
--rw-r--r--   0 maxankurb   (501) staff       (20)       29 2023-07-27 17:44:46.000000 pytoniq-0.0.6/MANIFEST.in
--rw-r--r--   0 maxankurb   (501) staff       (20)    13684 2023-07-27 17:45:07.344669 pytoniq-0.0.6/PKG-INFO
--rw-r--r--   0 maxankurb   (501) staff       (20)    13278 2023-07-27 17:32:45.000000 pytoniq-0.0.6/README.md
-drwxr-xr-x   0 maxankurb   (501) staff       (20)        0 2023-07-27 17:45:07.301804 pytoniq-0.0.6/pytoniq/
--rw-r--r--   0 maxankurb   (501) staff       (20)      149 2023-07-23 15:42:41.000000 pytoniq-0.0.6/pytoniq/__init__.py
-drwxr-xr-x   0 maxankurb   (501) staff       (20)        0 2023-07-27 17:45:07.311255 pytoniq-0.0.6/pytoniq/boc/
--rw-r--r--   0 maxankurb   (501) staff       (20)      222 2023-07-23 15:42:41.000000 pytoniq-0.0.6/pytoniq/boc/__init__.py
--rw-r--r--   0 maxankurb   (501) staff       (20)     3700 2023-07-27 16:08:51.000000 pytoniq-0.0.6/pytoniq/boc/address.py
--rw-r--r--   0 maxankurb   (501) staff       (20)     4204 2023-07-21 09:13:36.000000 pytoniq-0.0.6/pytoniq/boc/builder.py
--rw-r--r--   0 maxankurb   (501) staff       (20)    11007 2023-07-23 16:49:28.000000 pytoniq-0.0.6/pytoniq/boc/cell.py
--rw-r--r--   0 maxankurb   (501) staff       (20)     9049 2023-07-23 10:03:55.000000 pytoniq-0.0.6/pytoniq/boc/deserialize.py
-drwxr-xr-x   0 maxankurb   (501) staff       (20)        0 2023-07-27 17:45:07.314760 pytoniq-0.0.6/pytoniq/boc/dict/
--rw-r--r--   0 maxankurb   (501) staff       (20)       41 2023-07-23 15:42:41.000000 pytoniq-0.0.6/pytoniq/boc/dict/__init__.py
--rw-r--r--   0 maxankurb   (501) staff       (20)     5060 2023-07-23 15:16:15.000000 pytoniq-0.0.6/pytoniq/boc/dict/dict.py
--rw-r--r--   0 maxankurb   (501) staff       (20)     3919 2023-07-23 17:27:59.000000 pytoniq-0.0.6/pytoniq/boc/dict/parse.py
--rw-r--r--   0 maxankurb   (501) staff       (20)     4989 2023-06-19 11:55:15.000000 pytoniq-0.0.6/pytoniq/boc/dict/utils.py
--rw-r--r--   0 maxankurb   (501) staff       (20)     1026 2023-07-23 13:47:12.000000 pytoniq-0.0.6/pytoniq/boc/exotic.py
--rw-r--r--   0 maxankurb   (501) staff       (20)     7521 2023-07-11 20:09:21.000000 pytoniq-0.0.6/pytoniq/boc/slice.py
--rw-r--r--   0 maxankurb   (501) staff       (20)     1866 2023-07-05 13:08:40.000000 pytoniq-0.0.6/pytoniq/boc/tvm_bitarray.py
--rw-r--r--   0 maxankurb   (501) staff       (20)      298 2023-07-13 12:16:46.000000 pytoniq-0.0.6/pytoniq/boc/utils.py
-drwxr-xr-x   0 maxankurb   (501) staff       (20)        0 2023-07-27 17:45:07.316264 pytoniq-0.0.6/pytoniq/contract/
--rw-r--r--   0 maxankurb   (501) staff       (20)       69 2023-07-23 15:42:41.000000 pytoniq-0.0.6/pytoniq/contract/__init__.py
--rw-r--r--   0 maxankurb   (501) staff       (20)     6750 2023-07-23 15:29:17.000000 pytoniq-0.0.6/pytoniq/contract/contract.py
-drwxr-xr-x   0 maxankurb   (501) staff       (20)        0 2023-07-27 17:45:07.317384 pytoniq-0.0.6/pytoniq/contract/nft/
--rw-r--r--   0 maxankurb   (501) staff       (20)       25 2023-07-27 17:13:15.000000 pytoniq-0.0.6/pytoniq/contract/nft/__init__.py
--rw-r--r--   0 maxankurb   (501) staff       (20)     3643 2023-07-27 17:10:31.000000 pytoniq-0.0.6/pytoniq/contract/nft/nft.py
--rw-r--r--   0 maxankurb   (501) staff       (20)      102 2023-07-22 17:41:04.000000 pytoniq-0.0.6/pytoniq/contract/utils.py
-drwxr-xr-x   0 maxankurb   (501) staff       (20)        0 2023-07-27 17:45:07.319168 pytoniq-0.0.6/pytoniq/contract/wallets/
--rw-r--r--   0 maxankurb   (501) staff       (20)      151 2023-07-23 15:42:41.000000 pytoniq-0.0.6/pytoniq/contract/wallets/__init__.py
--rw-r--r--   0 maxankurb   (501) staff       (20)     7615 2023-07-23 07:51:49.000000 pytoniq-0.0.6/pytoniq/contract/wallets/highload.py
--rw-r--r--   0 maxankurb   (501) staff       (20)    18779 2023-07-23 07:41:58.000000 pytoniq-0.0.6/pytoniq/contract/wallets/wallet.py
-drwxr-xr-x   0 maxankurb   (501) staff       (20)        0 2023-07-27 17:45:07.322256 pytoniq-0.0.6/pytoniq/crypto/
--rw-r--r--   0 maxankurb   (501) staff       (20)        0 2023-06-17 12:05:39.000000 pytoniq-0.0.6/pytoniq/crypto/__init__.py
--rw-r--r--   0 maxankurb   (501) staff       (20)     2087 2023-05-27 14:21:05.000000 pytoniq-0.0.6/pytoniq/crypto/ciphers.py
--rw-r--r--   0 maxankurb   (501) staff       (20)     6558 2023-06-17 13:10:44.000000 pytoniq-0.0.6/pytoniq/crypto/crc.py
--rw-r--r--   0 maxankurb   (501) staff       (20)    22014 2023-07-22 13:35:04.000000 pytoniq-0.0.6/pytoniq/crypto/keys.py
--rw-r--r--   0 maxankurb   (501) staff       (20)      820 2023-07-27 14:32:52.000000 pytoniq-0.0.6/pytoniq/crypto/signature.py
-drwxr-xr-x   0 maxankurb   (501) staff       (20)        0 2023-07-27 17:45:07.326392 pytoniq-0.0.6/pytoniq/liteclient/
--rw-r--r--   0 maxankurb   (501) staff       (20)       88 2023-07-23 15:42:41.000000 pytoniq-0.0.6/pytoniq/liteclient/__init__.py
--rw-r--r--   0 maxankurb   (501) staff       (20)    38171 2023-07-27 16:14:12.000000 pytoniq-0.0.6/pytoniq/liteclient/client.py
--rw-r--r--   0 maxankurb   (501) staff       (20)     5409 2023-07-27 15:47:44.000000 pytoniq-0.0.6/pytoniq/liteclient/sync.py
--rw-r--r--   0 maxankurb   (501) staff       (20)      625 2023-07-24 15:34:43.000000 pytoniq-0.0.6/pytoniq/liteclient/utils.py
-drwxr-xr-x   0 maxankurb   (501) staff       (20)        0 2023-07-27 17:45:07.327897 pytoniq-0.0.6/pytoniq/proof/
--rw-r--r--   0 maxankurb   (501) staff       (20)      186 2023-07-23 15:42:41.000000 pytoniq-0.0.6/pytoniq/proof/__init__.py
--rw-r--r--   0 maxankurb   (501) staff       (20)     6193 2023-07-21 11:26:13.000000 pytoniq-0.0.6/pytoniq/proof/check_proof.py
-drwxr-xr-x   0 maxankurb   (501) staff       (20)        0 2023-07-27 17:45:07.329629 pytoniq-0.0.6/pytoniq/tl/
--rw-r--r--   0 maxankurb   (501) staff       (20)      118 2023-07-23 15:42:41.000000 pytoniq-0.0.6/pytoniq/tl/__init__.py
--rw-r--r--   0 maxankurb   (501) staff       (20)     2990 2023-07-23 08:44:15.000000 pytoniq-0.0.6/pytoniq/tl/block.py
--rw-r--r--   0 maxankurb   (501) staff       (20)    14409 2023-07-27 14:57:28.000000 pytoniq-0.0.6/pytoniq/tl/generator.py
-drwxr-xr-x   0 maxankurb   (501) staff       (20)        0 2023-07-27 17:45:07.332088 pytoniq-0.0.6/pytoniq/tl/schemas/
--rw-r--r--   0 maxankurb   (501) staff       (20)     7204 2023-07-13 15:35:42.000000 pytoniq-0.0.6/pytoniq/tl/schemas/lite_api.tl
--rw-r--r--   0 maxankurb   (501) staff       (20)    45439 2023-06-17 21:53:59.000000 pytoniq-0.0.6/pytoniq/tl/schemas/ton_api.tl
--rw-r--r--   0 maxankurb   (501) staff       (20)    18697 2023-05-29 07:39:43.000000 pytoniq-0.0.6/pytoniq/tl/schemas/tonlib_api.tl
-drwxr-xr-x   0 maxankurb   (501) staff       (20)        0 2023-07-27 17:45:07.341346 pytoniq-0.0.6/pytoniq/tlb/
--rw-r--r--   0 maxankurb   (501) staff       (20)      924 2023-07-24 08:29:16.000000 pytoniq-0.0.6/pytoniq/tlb/__init__.py
--rw-r--r--   0 maxankurb   (501) staff       (20)    11853 2023-07-23 13:10:19.000000 pytoniq-0.0.6/pytoniq/tlb/account.py
--rw-r--r--   0 maxankurb   (501) staff       (20)    34959 2023-07-24 08:25:46.000000 pytoniq-0.0.6/pytoniq/tlb/block.py
--rw-r--r--   0 maxankurb   (501) staff       (20)     5137 2023-06-30 16:07:22.000000 pytoniq-0.0.6/pytoniq/tlb/code_generator.py
--rw-r--r--   0 maxankurb   (501) staff       (20)    56951 2023-07-13 14:13:51.000000 pytoniq-0.0.6/pytoniq/tlb/config.py
-drwxr-xr-x   0 maxankurb   (501) staff       (20)        0 2023-07-27 17:45:07.344070 pytoniq-0.0.6/pytoniq/tlb/custom/
--rw-r--r--   0 maxankurb   (501) staff       (20)       91 2023-07-27 17:13:15.000000 pytoniq-0.0.6/pytoniq/tlb/custom/__init__.py
--rw-r--r--   0 maxankurb   (501) staff       (20)     1436 2023-07-27 17:07:58.000000 pytoniq-0.0.6/pytoniq/tlb/custom/nft.py
--rw-r--r--   0 maxankurb   (501) staff       (20)     4584 2023-07-23 14:27:13.000000 pytoniq-0.0.6/pytoniq/tlb/custom/wallet.py
--rw-r--r--   0 maxankurb   (501) staff       (20)    12530 2023-07-27 17:28:35.000000 pytoniq-0.0.6/pytoniq/tlb/generator.py
--rw-r--r--   0 maxankurb   (501) staff       (20)      382 2023-07-23 14:10:34.000000 pytoniq-0.0.6/pytoniq/tlb/tlb.py
--rw-r--r--   0 maxankurb   (501) staff       (20)    44289 2023-07-23 17:25:49.000000 pytoniq-0.0.6/pytoniq/tlb/transaction.py
--rw-r--r--   0 maxankurb   (501) staff       (20)     2292 2023-07-12 11:03:41.000000 pytoniq-0.0.6/pytoniq/tlb/utils.py
--rw-r--r--   0 maxankurb   (501) staff       (20)    15591 2023-07-21 07:26:25.000000 pytoniq-0.0.6/pytoniq/tlb/vm_stack.py
-drwxr-xr-x   0 maxankurb   (501) staff       (20)        0 2023-07-27 17:45:07.304768 pytoniq-0.0.6/pytoniq.egg-info/
--rw-r--r--   0 maxankurb   (501) staff       (20)    13684 2023-07-27 17:45:07.000000 pytoniq-0.0.6/pytoniq.egg-info/PKG-INFO
--rw-r--r--   0 maxankurb   (501) staff       (20)     1552 2023-07-27 17:45:07.000000 pytoniq-0.0.6/pytoniq.egg-info/SOURCES.txt
--rw-r--r--   0 maxankurb   (501) staff       (20)        1 2023-07-27 17:45:07.000000 pytoniq-0.0.6/pytoniq.egg-info/dependency_links.txt
--rw-r--r--   0 maxankurb   (501) staff       (20)      101 2023-07-27 17:45:07.000000 pytoniq-0.0.6/pytoniq.egg-info/requires.txt
--rw-r--r--   0 maxankurb   (501) staff       (20)        8 2023-07-27 17:45:07.000000 pytoniq-0.0.6/pytoniq.egg-info/top_level.txt
--rw-r--r--   0 maxankurb   (501) staff       (20)       38 2023-07-27 17:45:07.345049 pytoniq-0.0.6/setup.cfg
--rw-r--r--   0 maxankurb   (501) staff       (20)      948 2023-07-27 17:44:57.000000 pytoniq-0.0.6/setup.py
+drwxr-xr-x   0 maxankurb   (501) staff       (20)        0 2023-07-30 15:05:36.647804 pytoniq-0.0.7/
+-rw-r--r--   0 maxankurb   (501) staff       (20)       29 2023-07-27 17:44:46.000000 pytoniq-0.0.7/MANIFEST.in
+-rw-r--r--   0 maxankurb   (501) staff       (20)    13684 2023-07-30 15:05:36.647040 pytoniq-0.0.7/PKG-INFO
+-rw-r--r--   0 maxankurb   (501) staff       (20)    13278 2023-07-27 17:32:45.000000 pytoniq-0.0.7/README.md
+drwxr-xr-x   0 maxankurb   (501) staff       (20)        0 2023-07-30 15:05:36.598394 pytoniq-0.0.7/pytoniq/
+-rw-r--r--   0 maxankurb   (501) staff       (20)      149 2023-07-23 15:42:41.000000 pytoniq-0.0.7/pytoniq/__init__.py
+drwxr-xr-x   0 maxankurb   (501) staff       (20)        0 2023-07-30 15:05:36.607803 pytoniq-0.0.7/pytoniq/boc/
+-rw-r--r--   0 maxankurb   (501) staff       (20)      222 2023-07-23 15:42:41.000000 pytoniq-0.0.7/pytoniq/boc/__init__.py
+-rw-r--r--   0 maxankurb   (501) staff       (20)     3700 2023-07-27 16:08:51.000000 pytoniq-0.0.7/pytoniq/boc/address.py
+-rw-r--r--   0 maxankurb   (501) staff       (20)     4204 2023-07-21 09:13:36.000000 pytoniq-0.0.7/pytoniq/boc/builder.py
+-rw-r--r--   0 maxankurb   (501) staff       (20)    11007 2023-07-23 16:49:28.000000 pytoniq-0.0.7/pytoniq/boc/cell.py
+-rw-r--r--   0 maxankurb   (501) staff       (20)     9079 2023-07-28 16:29:36.000000 pytoniq-0.0.7/pytoniq/boc/deserialize.py
+drwxr-xr-x   0 maxankurb   (501) staff       (20)        0 2023-07-30 15:05:36.610860 pytoniq-0.0.7/pytoniq/boc/dict/
+-rw-r--r--   0 maxankurb   (501) staff       (20)       41 2023-07-23 15:42:41.000000 pytoniq-0.0.7/pytoniq/boc/dict/__init__.py
+-rw-r--r--   0 maxankurb   (501) staff       (20)     5060 2023-07-23 15:16:15.000000 pytoniq-0.0.7/pytoniq/boc/dict/dict.py
+-rw-r--r--   0 maxankurb   (501) staff       (20)     3919 2023-07-23 17:27:59.000000 pytoniq-0.0.7/pytoniq/boc/dict/parse.py
+-rw-r--r--   0 maxankurb   (501) staff       (20)     4989 2023-06-19 11:55:15.000000 pytoniq-0.0.7/pytoniq/boc/dict/utils.py
+-rw-r--r--   0 maxankurb   (501) staff       (20)     1026 2023-07-23 13:47:12.000000 pytoniq-0.0.7/pytoniq/boc/exotic.py
+-rw-r--r--   0 maxankurb   (501) staff       (20)     7521 2023-07-11 20:09:21.000000 pytoniq-0.0.7/pytoniq/boc/slice.py
+-rw-r--r--   0 maxankurb   (501) staff       (20)     1866 2023-07-05 13:08:40.000000 pytoniq-0.0.7/pytoniq/boc/tvm_bitarray.py
+-rw-r--r--   0 maxankurb   (501) staff       (20)      298 2023-07-13 12:16:46.000000 pytoniq-0.0.7/pytoniq/boc/utils.py
+drwxr-xr-x   0 maxankurb   (501) staff       (20)        0 2023-07-30 15:05:36.613290 pytoniq-0.0.7/pytoniq/contract/
+-rw-r--r--   0 maxankurb   (501) staff       (20)       69 2023-07-23 15:42:41.000000 pytoniq-0.0.7/pytoniq/contract/__init__.py
+-rw-r--r--   0 maxankurb   (501) staff       (20)     6750 2023-07-28 19:24:43.000000 pytoniq-0.0.7/pytoniq/contract/contract.py
+drwxr-xr-x   0 maxankurb   (501) staff       (20)        0 2023-07-30 15:05:36.614773 pytoniq-0.0.7/pytoniq/contract/nft/
+-rw-r--r--   0 maxankurb   (501) staff       (20)       25 2023-07-27 17:13:15.000000 pytoniq-0.0.7/pytoniq/contract/nft/__init__.py
+-rw-r--r--   0 maxankurb   (501) staff       (20)     3643 2023-07-27 17:10:31.000000 pytoniq-0.0.7/pytoniq/contract/nft/nft.py
+-rw-r--r--   0 maxankurb   (501) staff       (20)      102 2023-07-22 17:41:04.000000 pytoniq-0.0.7/pytoniq/contract/utils.py
+drwxr-xr-x   0 maxankurb   (501) staff       (20)        0 2023-07-30 15:05:36.617205 pytoniq-0.0.7/pytoniq/contract/wallets/
+-rw-r--r--   0 maxankurb   (501) staff       (20)      151 2023-07-23 15:42:41.000000 pytoniq-0.0.7/pytoniq/contract/wallets/__init__.py
+-rw-r--r--   0 maxankurb   (501) staff       (20)     7615 2023-07-23 07:51:49.000000 pytoniq-0.0.7/pytoniq/contract/wallets/highload.py
+-rw-r--r--   0 maxankurb   (501) staff       (20)    18779 2023-07-23 07:41:58.000000 pytoniq-0.0.7/pytoniq/contract/wallets/wallet.py
+drwxr-xr-x   0 maxankurb   (501) staff       (20)        0 2023-07-30 15:05:36.620548 pytoniq-0.0.7/pytoniq/crypto/
+-rw-r--r--   0 maxankurb   (501) staff       (20)        0 2023-06-17 12:05:39.000000 pytoniq-0.0.7/pytoniq/crypto/__init__.py
+-rw-r--r--   0 maxankurb   (501) staff       (20)     2087 2023-05-27 14:21:05.000000 pytoniq-0.0.7/pytoniq/crypto/ciphers.py
+-rw-r--r--   0 maxankurb   (501) staff       (20)     6558 2023-06-17 13:10:44.000000 pytoniq-0.0.7/pytoniq/crypto/crc.py
+-rw-r--r--   0 maxankurb   (501) staff       (20)    22014 2023-07-22 13:35:04.000000 pytoniq-0.0.7/pytoniq/crypto/keys.py
+-rw-r--r--   0 maxankurb   (501) staff       (20)      820 2023-07-27 14:32:52.000000 pytoniq-0.0.7/pytoniq/crypto/signature.py
+drwxr-xr-x   0 maxankurb   (501) staff       (20)        0 2023-07-30 15:05:36.624807 pytoniq-0.0.7/pytoniq/liteclient/
+-rw-r--r--   0 maxankurb   (501) staff       (20)       88 2023-07-23 15:42:41.000000 pytoniq-0.0.7/pytoniq/liteclient/__init__.py
+-rw-r--r--   0 maxankurb   (501) staff       (20)    39226 2023-07-30 15:02:06.000000 pytoniq-0.0.7/pytoniq/liteclient/client.py
+-rw-r--r--   0 maxankurb   (501) staff       (20)     5409 2023-07-30 14:31:13.000000 pytoniq-0.0.7/pytoniq/liteclient/sync.py
+-rw-r--r--   0 maxankurb   (501) staff       (20)      625 2023-07-24 15:34:43.000000 pytoniq-0.0.7/pytoniq/liteclient/utils.py
+drwxr-xr-x   0 maxankurb   (501) staff       (20)        0 2023-07-30 15:05:36.626302 pytoniq-0.0.7/pytoniq/proof/
+-rw-r--r--   0 maxankurb   (501) staff       (20)      186 2023-07-23 15:42:41.000000 pytoniq-0.0.7/pytoniq/proof/__init__.py
+-rw-r--r--   0 maxankurb   (501) staff       (20)     6193 2023-07-21 11:26:13.000000 pytoniq-0.0.7/pytoniq/proof/check_proof.py
+drwxr-xr-x   0 maxankurb   (501) staff       (20)        0 2023-07-30 15:05:36.629267 pytoniq-0.0.7/pytoniq/tl/
+-rw-r--r--   0 maxankurb   (501) staff       (20)      118 2023-07-23 15:42:41.000000 pytoniq-0.0.7/pytoniq/tl/__init__.py
+-rw-r--r--   0 maxankurb   (501) staff       (20)     2990 2023-07-23 08:44:15.000000 pytoniq-0.0.7/pytoniq/tl/block.py
+-rw-r--r--   0 maxankurb   (501) staff       (20)    14400 2023-07-30 15:03:21.000000 pytoniq-0.0.7/pytoniq/tl/generator.py
+drwxr-xr-x   0 maxankurb   (501) staff       (20)        0 2023-07-30 15:05:36.631790 pytoniq-0.0.7/pytoniq/tl/schemas/
+-rw-r--r--   0 maxankurb   (501) staff       (20)     7204 2023-07-30 12:46:41.000000 pytoniq-0.0.7/pytoniq/tl/schemas/lite_api.tl
+-rw-r--r--   0 maxankurb   (501) staff       (20)    45439 2023-06-17 21:53:59.000000 pytoniq-0.0.7/pytoniq/tl/schemas/ton_api.tl
+-rw-r--r--   0 maxankurb   (501) staff       (20)    18697 2023-05-29 07:39:43.000000 pytoniq-0.0.7/pytoniq/tl/schemas/tonlib_api.tl
+drwxr-xr-x   0 maxankurb   (501) staff       (20)        0 2023-07-30 15:05:36.643910 pytoniq-0.0.7/pytoniq/tlb/
+-rw-r--r--   0 maxankurb   (501) staff       (20)      924 2023-07-24 08:29:16.000000 pytoniq-0.0.7/pytoniq/tlb/__init__.py
+-rw-r--r--   0 maxankurb   (501) staff       (20)    11853 2023-07-23 13:10:19.000000 pytoniq-0.0.7/pytoniq/tlb/account.py
+-rw-r--r--   0 maxankurb   (501) staff       (20)    34959 2023-07-24 08:25:46.000000 pytoniq-0.0.7/pytoniq/tlb/block.py
+-rw-r--r--   0 maxankurb   (501) staff       (20)     5137 2023-06-30 16:07:22.000000 pytoniq-0.0.7/pytoniq/tlb/code_generator.py
+-rw-r--r--   0 maxankurb   (501) staff       (20)    56951 2023-07-13 14:13:51.000000 pytoniq-0.0.7/pytoniq/tlb/config.py
+drwxr-xr-x   0 maxankurb   (501) staff       (20)        0 2023-07-30 15:05:36.645893 pytoniq-0.0.7/pytoniq/tlb/custom/
+-rw-r--r--   0 maxankurb   (501) staff       (20)       91 2023-07-27 17:13:15.000000 pytoniq-0.0.7/pytoniq/tlb/custom/__init__.py
+-rw-r--r--   0 maxankurb   (501) staff       (20)     1436 2023-07-27 17:07:58.000000 pytoniq-0.0.7/pytoniq/tlb/custom/nft.py
+-rw-r--r--   0 maxankurb   (501) staff       (20)     4584 2023-07-23 14:27:13.000000 pytoniq-0.0.7/pytoniq/tlb/custom/wallet.py
+-rw-r--r--   0 maxankurb   (501) staff       (20)    12530 2023-07-27 17:28:35.000000 pytoniq-0.0.7/pytoniq/tlb/generator.py
+-rw-r--r--   0 maxankurb   (501) staff       (20)      382 2023-07-23 14:10:34.000000 pytoniq-0.0.7/pytoniq/tlb/tlb.py
+-rw-r--r--   0 maxankurb   (501) staff       (20)    44289 2023-07-28 18:49:05.000000 pytoniq-0.0.7/pytoniq/tlb/transaction.py
+-rw-r--r--   0 maxankurb   (501) staff       (20)     2292 2023-07-12 11:03:41.000000 pytoniq-0.0.7/pytoniq/tlb/utils.py
+-rw-r--r--   0 maxankurb   (501) staff       (20)    15591 2023-07-21 07:26:25.000000 pytoniq-0.0.7/pytoniq/tlb/vm_stack.py
+drwxr-xr-x   0 maxankurb   (501) staff       (20)        0 2023-07-30 15:05:36.600487 pytoniq-0.0.7/pytoniq.egg-info/
+-rw-r--r--   0 maxankurb   (501) staff       (20)    13684 2023-07-30 15:05:36.000000 pytoniq-0.0.7/pytoniq.egg-info/PKG-INFO
+-rw-r--r--   0 maxankurb   (501) staff       (20)     1552 2023-07-30 15:05:36.000000 pytoniq-0.0.7/pytoniq.egg-info/SOURCES.txt
+-rw-r--r--   0 maxankurb   (501) staff       (20)        1 2023-07-30 15:05:36.000000 pytoniq-0.0.7/pytoniq.egg-info/dependency_links.txt
+-rw-r--r--   0 maxankurb   (501) staff       (20)      101 2023-07-30 15:05:36.000000 pytoniq-0.0.7/pytoniq.egg-info/requires.txt
+-rw-r--r--   0 maxankurb   (501) staff       (20)        8 2023-07-30 15:05:36.000000 pytoniq-0.0.7/pytoniq.egg-info/top_level.txt
+-rw-r--r--   0 maxankurb   (501) staff       (20)       38 2023-07-30 15:05:36.647899 pytoniq-0.0.7/setup.cfg
+-rw-r--r--   0 maxankurb   (501) staff       (20)      948 2023-07-30 15:05:20.000000 pytoniq-0.0.7/setup.py
```

### Comparing `pytoniq-0.0.6/PKG-INFO` & `pytoniq-0.0.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pytoniq
-Version: 0.0.6
+Version: 0.0.7
 Summary: TON Blockchain SDK
 Home-page: https://github.com/yungwine/pytoniq
 Author: Maksim Kurbatov
 Author-email: cyrbatoff@gmail.com
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Software Development :: Libraries
```

### Comparing `pytoniq-0.0.6/README.md` & `pytoniq-0.0.7/README.md`

 * *Files identical despite different names*

### Comparing `pytoniq-0.0.6/pytoniq/boc/address.py` & `pytoniq-0.0.7/pytoniq/boc/address.py`

 * *Files identical despite different names*

### Comparing `pytoniq-0.0.6/pytoniq/boc/builder.py` & `pytoniq-0.0.7/pytoniq/boc/builder.py`

 * *Files identical despite different names*

### Comparing `pytoniq-0.0.6/pytoniq/boc/cell.py` & `pytoniq-0.0.7/pytoniq/boc/cell.py`

 * *Files identical despite different names*

### Comparing `pytoniq-0.0.6/pytoniq/boc/deserialize.py` & `pytoniq-0.0.7/pytoniq/boc/deserialize.py`

 * *Files 1% similar despite different names*

```diff
@@ -58,15 +58,15 @@
         return f'<NullCell {len(self.bits)}[{self.bits.tobytes().hex().upper()}] -> {len(self.refs)} refs>'
 
     def __str__(self, t=1, comma=False) -> str:
         """
         :param t: \t symbols amount before text
         :param comma: "," after "}"
         """
-        text = f'{len(self.bits)}[{self.bits.tobytes().hex().upper()}]'
+        text = ('* ' * (self.type_ != -1)) + f'{len(self.bits)}[{self.bits.tobytes().hex().upper()}]'
         if self.refs:
             text += f' -> {{\n'
             for index, ref in enumerate(self.refs):
                 next_comma = True if index != len(self.refs) - 1 else False
                 text += '\t' * t + ref.__str__(t + 1, next_comma) + '\n'
             text += '\t' * (t - 1) + '}'
         if comma:
```

### Comparing `pytoniq-0.0.6/pytoniq/boc/dict/dict.py` & `pytoniq-0.0.7/pytoniq/boc/dict/dict.py`

 * *Files identical despite different names*

### Comparing `pytoniq-0.0.6/pytoniq/boc/dict/parse.py` & `pytoniq-0.0.7/pytoniq/boc/dict/parse.py`

 * *Files identical despite different names*

### Comparing `pytoniq-0.0.6/pytoniq/boc/dict/utils.py` & `pytoniq-0.0.7/pytoniq/boc/dict/utils.py`

 * *Files identical despite different names*

### Comparing `pytoniq-0.0.6/pytoniq/boc/exotic.py` & `pytoniq-0.0.7/pytoniq/boc/exotic.py`

 * *Files identical despite different names*

### Comparing `pytoniq-0.0.6/pytoniq/boc/slice.py` & `pytoniq-0.0.7/pytoniq/boc/slice.py`

 * *Files identical despite different names*

### Comparing `pytoniq-0.0.6/pytoniq/boc/tvm_bitarray.py` & `pytoniq-0.0.7/pytoniq/boc/tvm_bitarray.py`

 * *Files identical despite different names*

### Comparing `pytoniq-0.0.6/pytoniq/contract/contract.py` & `pytoniq-0.0.7/pytoniq/contract/contract.py`

 * *Files identical despite different names*

### Comparing `pytoniq-0.0.6/pytoniq/contract/nft/nft.py` & `pytoniq-0.0.7/pytoniq/contract/nft/nft.py`

 * *Files identical despite different names*

### Comparing `pytoniq-0.0.6/pytoniq/contract/wallets/highload.py` & `pytoniq-0.0.7/pytoniq/contract/wallets/highload.py`

 * *Files identical despite different names*

### Comparing `pytoniq-0.0.6/pytoniq/contract/wallets/wallet.py` & `pytoniq-0.0.7/pytoniq/contract/wallets/wallet.py`

 * *Files identical despite different names*

### Comparing `pytoniq-0.0.6/pytoniq/crypto/ciphers.py` & `pytoniq-0.0.7/pytoniq/crypto/ciphers.py`

 * *Files identical despite different names*

### Comparing `pytoniq-0.0.6/pytoniq/crypto/crc.py` & `pytoniq-0.0.7/pytoniq/crypto/crc.py`

 * *Files identical despite different names*

### Comparing `pytoniq-0.0.6/pytoniq/crypto/keys.py` & `pytoniq-0.0.7/pytoniq/crypto/keys.py`

 * *Files identical despite different names*

### Comparing `pytoniq-0.0.6/pytoniq/crypto/signature.py` & `pytoniq-0.0.7/pytoniq/crypto/signature.py`

 * *Files identical despite different names*

### Comparing `pytoniq-0.0.6/pytoniq/liteclient/client.py` & `pytoniq-0.0.7/pytoniq/liteclient/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 import base64
 import hashlib
 import logging
 import os
 import asyncio
 import socket
 import struct
+import time
 import typing
 
 import requests
 
 from .sync import persistent_state_ttl, choose_key_block, sync
 from .utils import init_mainnet_block, init_testnet_block
 from ..boc import Slice, Cell, Builder
@@ -73,15 +74,15 @@
         """########### connection ###########"""
         self.reader: asyncio.StreamReader = None
         self.writer: asyncio.StreamWriter = None
         self.listener: asyncio.Task = None
         self.pinger: asyncio.Task = None
         self.updater: asyncio.Task = None
         self.loop = asyncio.get_event_loop()
-        self.delta = 0.1  # listen delay
+        self.delta = 0.02  # listen delay
 
         """########### TL ###########"""
         if tl_schemas_path is None:
             tl_schemas_path = os.path.join(os.path.dirname(__file__), os.pardir, 'tl/schemas')
         self.schemas = TlGenerator(tl_schemas_path).generate()
         # for better performance:
         self.ping_sch = self.schemas.get_by_name('tcp.ping')
@@ -132,26 +133,28 @@
             # check hashsum
             assert hashlib.sha256(data_decrypted[:-32]).digest() == data_decrypted[-32:], 'incorrect checksum'
             result = self.deserialize_adnl_query(data_decrypted[:-32])
 
             if not result:
                 # for handshake
                 result = {}
-            if 'code' in result and 'message' in result:
-                raise LiteClientError(f'LiteClient crashed with {result["code"]} code. Message: {result["message"]}')
 
             qid = result.get('query_id', result.get('random_id'))  # return query_id for ordinary requests, random_id for ping-pong requests, None for handshake
 
             request = self.tasks.pop(qid)
-            request.set_result(result.get('answer', {}))
+
+            result = result.get('answer', {})
+            request.set_result(result)
 
     async def connect(self) -> None:
         handshake = self.handshake()
         self.reader, self.writer = await asyncio.open_connection(self.server.host, self.server.port)
         future = await self.send(handshake, None)
+        # async with asyncio.TaskGroup() as tg:
+        #     self.listener = tg.create_task(self.listen(), name='listener')
         self.listener = asyncio.create_task(self.listen(), name='listener')
         await self.update_last_blocks()
         self.pinger = asyncio.create_task(self.ping(), name='pinger')
         self.updater = asyncio.create_task(self.block_updater(), name='updater')
         await future
         self.inited = True
 
@@ -211,22 +214,31 @@
         while True:
             await asyncio.sleep(3)
             ping_query, qid = self.get_ping_query()
             pong = await self.send(ping_query, qid)
             await pong
             self.logger.debug(msg=f'ping - pong')
 
+    async def liteserver_query(self, query: bytes, qid: str) -> dict:
+        data = self.serialize_packet(query)
+        resp = await self.send_and_encrypt(data, qid)
+        await resp
+        result = resp.result()
+
+        if 'code' in result and 'message' in result:
+            await self.close()
+            raise LiteClientError(f'LiteClient crashed with {result["code"]} code. Message: {result["message"]}')
+
+        return resp.result()
+
     async def liteserver_request(self, tl_schema_name: str, data: dict) -> dict:
         schema = self.schemas.get_by_name('liteServer.' + tl_schema_name)
         self.logger.info(msg=f'requesting {tl_schema_name} with provided data {data}')
         data, qid = self.serialize_adnl_ls_query(schema, data)
-        data = self.serialize_packet(data)
-        resp = await self.send_and_encrypt(data, qid)
-        await resp
-        return resp.result()
+        return await self.liteserver_query(data, qid)
 
     @staticmethod
     def pack_block_id_ext(**kwargs):
         if not kwargs.get('shard'):
             kwargs['shard'] = -9223372036854775808
         if isinstance(kwargs['root_hash'], bytes):
             kwargs['root_hash'] = kwargs['root_hash'].hex()
@@ -254,24 +266,41 @@
         self.last_shard_blocks = shard_result
         self.logger.debug(msg=f'update blocks:\nlast_mc_block: {self.last_mc_block}\nlast_shard_blocks: {self.last_shard_blocks}')
 
     async def block_updater(self):
         if self.last_mc_block is None:
             self.last_mc_block = await self.get_trusted_last_mc_block()
         while True:
-            result = await self.wait_masterchain_seqno(self.last_mc_block.seqno + 1, timeout_ms=10000)
-            if result['code'] != 0:
-                logging.getLogger().warning(f'error response from liteserver in block updater: {result}')
+            await self.wait_masterchain_seqno(self.last_mc_block.seqno + 1, timeout_ms=10000, schema_name='getMasterchainInfo', data={})
             await self.update_last_blocks()
 
     async def get_masterchain_info(self):
         return await self.liteserver_request('getMasterchainInfo', {})
 
-    async def wait_masterchain_seqno(self, seqno: int, timeout_ms: int):
-        return await self.liteserver_request('waitMasterchainSeqno', {'seqno': seqno, 'timeout_ms': timeout_ms})
+    async def raw_wait_masterchain_seqno(self, seqno: int, timeout_ms: int, suffix: bytes = b''):
+        prefix = self.schemas.serialize(schema=self.schemas.get_by_name('liteServer.waitMasterchainSeqno'), data={'seqno': seqno, 'timeout_ms': timeout_ms})
+
+        qid = get_random(32)
+        data = self.schemas.serialize(
+            self.adnl_query_sch,
+            {'query_id': qid,
+             'query': self.schemas.serialize(self.ls_query_sch,
+                                             {'data': prefix + suffix}
+                                             )
+             }
+        )
+        return await self.liteserver_query(data, qid[::-1].hex())
+
+    async def wait_masterchain_seqno(self, seqno: int, timeout_ms: int, schema_name: str, data: dict = None):
+        if data is None:
+            data = {}
+
+        suffix = self.schemas.serialize(self.schemas.get_by_name('liteServer.' + schema_name), data)
+
+        return await self.raw_wait_masterchain_seqno(seqno, timeout_ms, suffix)
 
     async def get_masterchain_info_ext(self):
         return await self.liteserver_request('getMasterchainInfoExt', {'mode': 0})
 
     async def get_time(self):
         return await self.liteserver_request('getTime', {})
 
@@ -355,15 +384,14 @@
             trusted = True
         if isinstance(address, str):
             address = Address(address)
         account = address.to_tl_account_id()
 
         data = {'id': block.to_dict(), 'account': account}
         result = await self.liteserver_request('getAccountState', data)
-
         shrd_blk = BlockIdExt.from_dict(result['shardblk'])
         if not result['state']:
             return None, None  # account_none$0 = Account;
 
         account_state_root = Cell.one_from_boc(result['state'])
 
         if self.trust_level <= 1:
```

### Comparing `pytoniq-0.0.6/pytoniq/liteclient/sync.py` & `pytoniq-0.0.7/pytoniq/liteclient/sync.py`

 * *Files identical despite different names*

### Comparing `pytoniq-0.0.6/pytoniq/liteclient/utils.py` & `pytoniq-0.0.7/pytoniq/liteclient/utils.py`

 * *Files identical despite different names*

### Comparing `pytoniq-0.0.6/pytoniq/proof/check_proof.py` & `pytoniq-0.0.7/pytoniq/proof/check_proof.py`

 * *Files identical despite different names*

### Comparing `pytoniq-0.0.6/pytoniq/tl/block.py` & `pytoniq-0.0.7/pytoniq/tl/block.py`

 * *Files identical despite different names*

### Comparing `pytoniq-0.0.6/pytoniq/tl/generator.py` & `pytoniq-0.0.7/pytoniq/tl/generator.py`

 * *Files 2% similar despite different names*

```diff
@@ -183,16 +183,15 @@
         for field, type_ in schema.args.items():
             if 'mode' in type_ or 'flags' in type_:
                 type_ = type_.split('?')[1]
                 if data.get(field) is None:
                     continue
             value = data[field]
             result += self.serialize_field(type_, value)
-            # p = self.serialize_field(type_, value)
-            # print(field, type_, len(p), p.hex())
+        logger.log(level=5, msg=f'serialization result for schema {schema} is {result.hex()}')
         return result
 
     def deserialize(self, data: bytes, boxed: bool = True, args=None) -> typing.Tuple[typing.Union[dict, bytes], int]:
         i = 0
         result = {}
         if boxed:
             schema = self.get_by_id(data[i:i + 4], 'little')
```

### Comparing `pytoniq-0.0.6/pytoniq/tl/schemas/lite_api.tl` & `pytoniq-0.0.7/pytoniq/tl/schemas/lite_api.tl`

 * *Files identical despite different names*

### Comparing `pytoniq-0.0.6/pytoniq/tl/schemas/ton_api.tl` & `pytoniq-0.0.7/pytoniq/tl/schemas/ton_api.tl`

 * *Files identical despite different names*

### Comparing `pytoniq-0.0.6/pytoniq/tl/schemas/tonlib_api.tl` & `pytoniq-0.0.7/pytoniq/tl/schemas/tonlib_api.tl`

 * *Files identical despite different names*

### Comparing `pytoniq-0.0.6/pytoniq/tlb/__init__.py` & `pytoniq-0.0.7/pytoniq/tlb/__init__.py`

 * *Files identical despite different names*

### Comparing `pytoniq-0.0.6/pytoniq/tlb/account.py` & `pytoniq-0.0.7/pytoniq/tlb/account.py`

 * *Files identical despite different names*

### Comparing `pytoniq-0.0.6/pytoniq/tlb/block.py` & `pytoniq-0.0.7/pytoniq/tlb/block.py`

 * *Files identical despite different names*

### Comparing `pytoniq-0.0.6/pytoniq/tlb/code_generator.py` & `pytoniq-0.0.7/pytoniq/tlb/code_generator.py`

 * *Files identical despite different names*

### Comparing `pytoniq-0.0.6/pytoniq/tlb/config.py` & `pytoniq-0.0.7/pytoniq/tlb/config.py`

 * *Files identical despite different names*

### Comparing `pytoniq-0.0.6/pytoniq/tlb/custom/nft.py` & `pytoniq-0.0.7/pytoniq/tlb/custom/nft.py`

 * *Files identical despite different names*

### Comparing `pytoniq-0.0.6/pytoniq/tlb/custom/wallet.py` & `pytoniq-0.0.7/pytoniq/tlb/custom/wallet.py`

 * *Files identical despite different names*

### Comparing `pytoniq-0.0.6/pytoniq/tlb/generator.py` & `pytoniq-0.0.7/pytoniq/tlb/generator.py`

 * *Files identical despite different names*

### Comparing `pytoniq-0.0.6/pytoniq/tlb/transaction.py` & `pytoniq-0.0.7/pytoniq/tlb/transaction.py`

 * *Files identical despite different names*

### Comparing `pytoniq-0.0.6/pytoniq/tlb/utils.py` & `pytoniq-0.0.7/pytoniq/tlb/utils.py`

 * *Files identical despite different names*

### Comparing `pytoniq-0.0.6/pytoniq/tlb/vm_stack.py` & `pytoniq-0.0.7/pytoniq/tlb/vm_stack.py`

 * *Files identical despite different names*

### Comparing `pytoniq-0.0.6/pytoniq.egg-info/PKG-INFO` & `pytoniq-0.0.7/pytoniq.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pytoniq
-Version: 0.0.6
+Version: 0.0.7
 Summary: TON Blockchain SDK
 Home-page: https://github.com/yungwine/pytoniq
 Author: Maksim Kurbatov
 Author-email: cyrbatoff@gmail.com
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Software Development :: Libraries
```

### Comparing `pytoniq-0.0.6/pytoniq.egg-info/SOURCES.txt` & `pytoniq-0.0.7/pytoniq.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pytoniq-0.0.6/setup.py` & `pytoniq-0.0.7/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="pytoniq",
-    version="0.0.6",
+    version="0.0.7",
     author="Maksim Kurbatov",
     author_email="cyrbatoff@gmail.com",
     description="TON Blockchain SDK",
     long_description=long_description,
     long_description_content_type="text/markdown",
     packages=setuptools.find_packages('.', exclude=['tests', 'examples', 'pytoniq/adnl']),
     include_package_data=True,
```

