# Comparing `tmp/pysui_fastcrypto-0.1.3.tar.gz` & `tmp/pysui_fastcrypto-0.1.4.tar.gz`

## Comparing `pysui_fastcrypto-0.1.3.tar` & `pysui_fastcrypto-0.1.4.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0      533 1970-01-01 00:00:00.000000 pysui_fastcrypto-0.1.3/Cargo.toml
--rw-r--r--   0      501       20       38 2023-07-18 11:56:07.000000 pysui_fastcrypto-0.1.3/.gitignore
--rw-r--r--   0      501       20      839 2023-07-26 19:01:11.000000 pysui_fastcrypto-0.1.3/CHANGELOG.md
--rw-r--r--   0      501       20    11357 2023-07-23 20:18:01.000000 pysui_fastcrypto-0.1.3/LICENSE
--rw-r--r--   0      501       20      143 2023-07-25 20:14:51.000000 pysui_fastcrypto-0.1.3/README.rst
--rw-r--r--   0      501       20      720 2023-07-25 11:41:22.000000 pysui_fastcrypto-0.1.3/pyproject.toml
--rw-r--r--   0      501       20       15 2023-07-23 20:45:50.000000 pysui_fastcrypto-0.1.3/requirements.txt
--rw-r--r--   0      501       20    18016 2023-07-26 19:07:58.000000 pysui_fastcrypto-0.1.3/src/lib.rs
--rw-r--r--   0      501       20    54330 2023-07-25 19:44:38.000000 pysui_fastcrypto-0.1.3/Cargo.lock
--rw-r--r--   0        0        0      699 1970-01-01 00:00:00.000000 pysui_fastcrypto-0.1.3/PKG-INFO
+-rw-r--r--   0        0        0      533 1970-01-01 00:00:00.000000 pysui_fastcrypto-0.1.4/Cargo.toml
+-rw-r--r--   0      501       20       38 2023-07-18 11:56:07.000000 pysui_fastcrypto-0.1.4/.gitignore
+-rw-r--r--   0      501       20      969 2023-07-30 09:04:52.000000 pysui_fastcrypto-0.1.4/CHANGELOG.md
+-rw-r--r--   0      501       20    11357 2023-07-23 20:18:01.000000 pysui_fastcrypto-0.1.4/LICENSE
+-rw-r--r--   0      501       20     1413 2023-07-30 09:00:32.000000 pysui_fastcrypto-0.1.4/README.rst
+-rw-r--r--   0      501       20      720 2023-07-25 11:41:22.000000 pysui_fastcrypto-0.1.4/pyproject.toml
+-rw-r--r--   0      501       20       15 2023-07-23 20:45:50.000000 pysui_fastcrypto-0.1.4/requirements.txt
+-rw-r--r--   0      501       20    18594 2023-07-30 08:25:43.000000 pysui_fastcrypto-0.1.4/src/lib.rs
+-rw-r--r--   0      501       20    54330 2023-07-30 09:03:23.000000 pysui_fastcrypto-0.1.4/Cargo.lock
+-rw-r--r--   0        0        0     1969 1970-01-01 00:00:00.000000 pysui_fastcrypto-0.1.4/PKG-INFO
```

### Comparing `pysui_fastcrypto-0.1.3/Cargo.toml` & `pysui_fastcrypto-0.1.4/Cargo.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [package]
 name = "pysui-fastcrypto"
-version = "0.1.3"
+version = "0.1.4"
 license = "Apache-2.0"
 edition = "2021"
 
 [lib]
 name = "pysui_fastcrypto"
 # "cdylib" is necessary to produce a shared library for Python to import from.
 crate-type = ["cdylib"]
```

### Comparing `pysui_fastcrypto-0.1.3/CHANGELOG.md` & `pysui_fastcrypto-0.1.4/CHANGELOG.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,25 +1,41 @@
 # Changelog
 
 All notable changes to this project will be documented in this file.
 
 The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.0.0/),
 and this project adheres to [Semantic Versioning](https://semver.org/spec/v2.0.0.html).
 
-## [0.1.3] - Unpublished
+## [0.1.4] - 2023-07-30
+
+### Added
+
+- Rust documentation
+
+### Fixed
+
+### Changed
+
+- Updated README.rst
+
+### Removed
+
+
+## [0.1.3] - 2023-07-28
 
 ### Added
 
 - `keys_from_mnemonics` takes phrase and derivation path
 
 ### Fixed
 
 ### Changed
 
 - `keys_from_keystring` and `generate_new_keypair` now return private key bytess instead of token
+- README.rst
 
 ### Removed
 
 - Returning the SignatureScheme from `generate_new_keypair` and `keys_from_mnemonics`
 - Returning the mnemonic phrase from `keys_from_mnemonics
 
 ## [0.1.2] - 2023-07-25
```

### Comparing `pysui_fastcrypto-0.1.3/LICENSE` & `pysui_fastcrypto-0.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `pysui_fastcrypto-0.1.3/pyproject.toml` & `pysui_fastcrypto-0.1.4/pyproject.toml`

 * *Files identical despite different names*

### Comparing `pysui_fastcrypto-0.1.3/src/lib.rs` & `pysui_fastcrypto-0.1.4/src/lib.rs`

 * *Files 3% similar despite different names*

```diff
@@ -1,7 +1,13 @@
+//! pysui-fastcrypto is a python wrapper for fundental use by pysui crypto functions.
+//!
+//! Portions of the code in this crate were used from MystenLabs Sui repository
+//! pysui-fastcrypto, fastcrypto and Sui code are all licensed under the Apache License, Version 2.0
+//!
+
 use anyhow::{anyhow, Result};
 use base64ct::Encoding as _;
 use bip32::{ChildNumber, DerivationPath, XPrv};
 use bip39::{Language, Mnemonic, MnemonicType, Seed};
 
 use fastcrypto::{
     ed25519::{Ed25519KeyPair, Ed25519PrivateKey, Ed25519PublicKey},
@@ -67,41 +73,41 @@
 
 /// Signature Schemes supported by Sui
 #[derive(Clone, Debug, PartialEq, Eq)]
 pub enum SignatureScheme {
     ED25519,
     Secp256k1,
     Secp256r1,
-    BLS12381, // This is currently not supported for user Sui Address.
-    MultiSig,
-    ZkLoginAuthenticator,
+    BLS12381,             // This is currently not supported for user Sui Address.
+    MultiSig,             // This is handles directly in pysui
+    ZkLoginAuthenticator, // This is currently not supported in pysui
 }
 
 impl SignatureScheme {
-    /// Get the byte value of a scheme
+    /// Return the byte value of a scheme
     pub fn flag(&self) -> u8 {
         match self {
             SignatureScheme::ED25519 => 0x00,
             SignatureScheme::Secp256k1 => 0x01,
             SignatureScheme::Secp256r1 => 0x02,
-            SignatureScheme::MultiSig => 0x03,
+            SignatureScheme::MultiSig => 0x03, // This is handles directly in pysui
             SignatureScheme::BLS12381 => 0x04, // This is currently not supported for user Sui Address.
-            SignatureScheme::ZkLoginAuthenticator => 0x05,
+            SignatureScheme::ZkLoginAuthenticator => 0x05, // This is currently not supported in pysui
         }
     }
 
     /// Return a scheme from a string
     pub fn from_flag(flag: &str) -> Result<SignatureScheme> {
         let byte_int = flag
             .parse::<u8>()
             .map_err(|_| anyhow!("Invalid key scheme".to_string()))?;
         Self::from_flag_byte(&byte_int)
     }
 
-    /// Return a scheme from a bytes
+    /// Return a scheme from a byte
     pub fn from_flag_byte(byte_int: &u8) -> Result<SignatureScheme> {
         match byte_int {
             0x00 => Ok(SignatureScheme::ED25519),
             0x01 => Ok(SignatureScheme::Secp256k1),
             0x02 => Ok(SignatureScheme::Secp256r1),
             0x03 => Ok(SignatureScheme::MultiSig),
             0x04 => Ok(SignatureScheme::BLS12381),
@@ -201,15 +207,16 @@
 fn keypair_from_keystring(keystring: String) -> Result<(SignatureScheme, SuiKeyPair), LibError> {
     let b64b = &mut VecDeque::from(Base64::decode(&keystring)?);
     let kscheme = SignatureScheme::from_flag_byte(&b64b.pop_front().unwrap())?;
     let rembytes = b64b.make_contiguous();
     Ok((kscheme.clone(), kp_from_bytes(kscheme, &rembytes)?))
 }
 
-pub fn validate_path(
+/// Validate that the given path is correct in the context of the key scheme
+fn validate_path(
     key_scheme: &SignatureScheme,
     path: Option<DerivationPath>,
 ) -> Result<DerivationPath, LibError> {
     match key_scheme {
         SignatureScheme::ED25519 => {
             match path.clone() {
                 Some(p) => {
@@ -344,15 +351,15 @@
         | SignatureScheme::ZkLoginAuthenticator => Err(anyhow!(format!(
             "key derivation not supported {:?}",
             key_scheme
         ))),
     }
 }
 
-/// Generate a new keypair with derivation path and optional mnemonic word lengths for phrase
+/// Generate a new keypair with optional derivation path and optional mnemonic word lengths for phrase
 fn new_keypair(
     scheme: u8,
     derivation_path: Option<String>,
     word_length: Option<String>,
 ) -> Result<(String, SuiKeyPair)> {
     let scheme = SignatureScheme::from_flag_byte(&scheme).unwrap();
     let dvpath = match derivation_path {
@@ -397,42 +404,47 @@
         },
     }
 }
 
 /// Returns a keystrings scheme, public key bytes and a token from a Sui keystring.
 /// Assumes that the inbound keystring is valid (e.g. `flag | private_key bytes`)
 #[pyfunction]
-fn keys_from_keystring(in_str: String) -> (u8, Vec<u8>, Vec<u8>) {
+pub fn keys_from_keystring(in_str: String) -> (u8, Vec<u8>, Vec<u8>) {
     assert!(in_str.len() != 0, "Requires valid keystring");
     let (scheme, kp) = keypair_from_keystring(in_str).unwrap();
     (scheme.flag(), kp.pubkey().as_bytes(), kp.as_bytes())
 }
 
 /// Returns a new keystrings scheme, public and private key bytes and a token.
 /// Assumes that the inbound keystring is valid (e.g. `flag | private_key bytes`)
 #[pyfunction]
-fn generate_new_keypair(
+pub fn generate_new_keypair(
     in_scheme: u8,
     derv_path: Option<String>,
     word_count: Option<String>,
 ) -> (String, Vec<u8>, Vec<u8>) {
     let (phrase, kp) = new_keypair(in_scheme, derv_path, word_count).unwrap();
     (phrase, kp.pubkey().as_bytes(), kp.as_bytes())
 }
 
 /// Returns keystrings scheme, public and private key bytes from mnemonic phrase and derivation path
 #[pyfunction]
-fn keys_from_mnemonics(scheme: u8, derivation_path: String, phrase: String) -> (Vec<u8>, Vec<u8>) {
+pub fn keys_from_mnemonics(
+    scheme: u8,
+    derivation_path: String,
+    phrase: String,
+) -> (Vec<u8>, Vec<u8>) {
     let kp = recover_keypair(scheme, derivation_path, phrase).unwrap();
     (kp.pubkey().as_bytes(), kp.as_bytes())
 }
+
 /// Signs a message with optional intent, otherwise default is used
 /// The in_data string is the tx_bytes string
 #[pyfunction]
-fn sign_digest(
+pub fn sign_digest(
     in_scheme: u8,
     prv_bytes: Vec<u8>,
     in_data: String,
     intent: Option<Vec<u8>>,
 ) -> Vec<u8> {
     let kp = kp_from_bytes(
         SignatureScheme::from_flag_byte(&in_scheme).unwrap(),
```

### Comparing `pysui_fastcrypto-0.1.3/Cargo.lock` & `pysui_fastcrypto-0.1.4/Cargo.lock`

 * *Files 0% similar despite different names*

```diff
@@ -1407,15 +1407,15 @@
  "proc-macro2",
  "quote",
  "syn 1.0.109",
 ]
 
 [[package]]
 name = "pysui-fastcrypto"
-version = "0.1.3"
+version = "0.1.4"
 dependencies = [
  "anyhow",
  "base64ct",
  "bip32",
  "fastcrypto",
  "pyo3",
  "slip10_ed25519",
```

