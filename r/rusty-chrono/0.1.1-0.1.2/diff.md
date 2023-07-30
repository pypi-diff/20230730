# Comparing `tmp/rusty_chrono-0.1.1.tar.gz` & `tmp/rusty_chrono-0.1.2.tar.gz`

## Comparing `rusty_chrono-0.1.1.tar` & `rusty_chrono-0.1.2.tar`

### file list

```diff
@@ -1,19 +1,20 @@
--rw-r--r--   0        0        0      358 1970-01-01 00:00:00.000000 rusty_chrono-0.1.1/Cargo.toml
--rw-r--r--   0      501       20     5297 2023-05-16 13:30:46.000000 rusty_chrono-0.1.1/.gitignore
--rw-r--r--   0      501       20      855 2023-07-30 02:02:20.000000 rusty_chrono-0.1.1/.gitlab-ci.yml
--rw-r--r--   0      501       20      886 2023-07-30 01:43:20.000000 rusty_chrono-0.1.1/Dockerfile
--rw-r--r--   0      501       20     1067 2023-05-17 12:29:26.000000 rusty_chrono-0.1.1/LICENSE
--rw-r--r--   0      501       20       22 2023-07-30 02:43:02.000000 rusty_chrono-0.1.1/README.md
--rw-r--r--   0      501       20      335 2023-07-30 02:24:39.000000 rusty_chrono-0.1.1/pyproject.toml
--rw-r--r--   0      501       20     1386 2023-06-01 01:46:23.000000 rusty_chrono-0.1.1/src/dateutil/date_errors.rs
--rw-r--r--   0      501       20     1122 2023-05-31 21:13:19.000000 rusty_chrono-0.1.1/src/dateutil/date_functions.rs
--rw-r--r--   0      501       20     1649 2023-05-31 19:46:51.000000 rusty_chrono-0.1.1/src/dateutil/date_parsing.rs
--rw-r--r--   0      501       20     5731 2023-06-01 01:49:36.000000 rusty_chrono-0.1.1/src/dateutil/dateutil_tests/date_functions_tests.rs
--rw-r--r--   0      501       20     3068 2023-06-01 01:49:42.000000 rusty_chrono-0.1.1/src/dateutil/dateutil_tests/date_parsing_tests.rs
--rw-r--r--   0      501       20       75 2023-05-31 19:54:29.000000 rusty_chrono-0.1.1/src/dateutil/dateutil_tests/mod.rs
--rw-r--r--   0      501       20      124 2023-05-31 20:48:24.000000 rusty_chrono-0.1.1/src/dateutil/mod.rs
--rw-r--r--   0      501       20      550 2023-05-31 21:18:38.000000 rusty_chrono-0.1.1/src/dateutil/time_fractions.rs
--rw-r--r--   0      501       20     2849 2023-07-30 01:28:59.000000 rusty_chrono-0.1.1/src/lib.rs
--rw-r--r--   0      501       20      661 2023-06-01 01:45:56.000000 rusty_chrono-0.1.1/test.py
--rw-r--r--   0      501       20    14655 2023-07-30 02:57:59.000000 rusty_chrono-0.1.1/Cargo.lock
--rw-r--r--   0        0        0      324 1970-01-01 00:00:00.000000 rusty_chrono-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0      266 1970-01-01 00:00:00.000000 rusty_chrono-0.1.2/Cargo.toml
+-rw-rw-rw-   0        0        0     5297 2023-07-30 21:53:52.000000 rusty_chrono-0.1.2/.gitignore
+-rw-rw-rw-   0        0        0     1448 2023-07-30 21:53:52.000000 rusty_chrono-0.1.2/.gitlab-ci.yml
+-rw-rw-rw-   0        0        0      886 2023-07-30 21:53:52.000000 rusty_chrono-0.1.2/Dockerfile
+-rw-rw-rw-   0        0        0     1067 2023-07-30 21:53:52.000000 rusty_chrono-0.1.2/LICENSE
+-rw-rw-rw-   0        0        0       22 2023-07-30 21:53:52.000000 rusty_chrono-0.1.2/README.md
+-rw-rw-rw-   0        0        0     1751 2023-07-30 21:53:52.000000 rusty_chrono-0.1.2/publish_script.py
+-rw-rw-rw-   0        0        0      335 2023-07-30 21:53:52.000000 rusty_chrono-0.1.2/pyproject.toml
+-rw-rw-rw-   0        0        0     1386 2023-07-30 21:53:52.000000 rusty_chrono-0.1.2/src/dateutil/date_errors.rs
+-rw-rw-rw-   0        0        0     1122 2023-07-30 21:53:52.000000 rusty_chrono-0.1.2/src/dateutil/date_functions.rs
+-rw-rw-rw-   0        0        0     1649 2023-07-30 21:53:52.000000 rusty_chrono-0.1.2/src/dateutil/date_parsing.rs
+-rw-rw-rw-   0        0        0     5731 2023-07-30 21:53:52.000000 rusty_chrono-0.1.2/src/dateutil/dateutil_tests/date_functions_tests.rs
+-rw-rw-rw-   0        0        0     3068 2023-07-30 21:53:52.000000 rusty_chrono-0.1.2/src/dateutil/dateutil_tests/date_parsing_tests.rs
+-rw-rw-rw-   0        0        0       75 2023-07-30 21:53:52.000000 rusty_chrono-0.1.2/src/dateutil/dateutil_tests/mod.rs
+-rw-rw-rw-   0        0        0      124 2023-07-30 21:53:52.000000 rusty_chrono-0.1.2/src/dateutil/mod.rs
+-rw-rw-rw-   0        0        0      550 2023-07-30 21:53:52.000000 rusty_chrono-0.1.2/src/dateutil/time_fractions.rs
+-rw-rw-rw-   0        0        0     2849 2023-07-30 21:53:52.000000 rusty_chrono-0.1.2/src/lib.rs
+-rw-rw-rw-   0        0        0      661 2023-07-30 21:53:52.000000 rusty_chrono-0.1.2/test.py
+-rw-r--r--   0        0        0    14585 2023-07-30 21:54:42.000000 rusty_chrono-0.1.2/Cargo.lock
+-rw-r--r--   0        0        0      324 1970-01-01 00:00:00.000000 rusty_chrono-0.1.2/PKG-INFO
```

### Comparing `rusty_chrono-0.1.1/.gitignore` & `rusty_chrono-0.1.2/.gitignore`

 * *Files identical despite different names*

### Comparing `rusty_chrono-0.1.1/Dockerfile` & `rusty_chrono-0.1.2/Dockerfile`

 * *Files identical despite different names*

### Comparing `rusty_chrono-0.1.1/LICENSE` & `rusty_chrono-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `rusty_chrono-0.1.1/src/dateutil/date_errors.rs` & `rusty_chrono-0.1.2/src/dateutil/date_errors.rs`

 * *Files identical despite different names*

### Comparing `rusty_chrono-0.1.1/src/dateutil/date_functions.rs` & `rusty_chrono-0.1.2/src/dateutil/date_functions.rs`

 * *Files identical despite different names*

### Comparing `rusty_chrono-0.1.1/src/dateutil/date_parsing.rs` & `rusty_chrono-0.1.2/src/dateutil/date_parsing.rs`

 * *Files identical despite different names*

### Comparing `rusty_chrono-0.1.1/src/dateutil/dateutil_tests/date_functions_tests.rs` & `rusty_chrono-0.1.2/src/dateutil/dateutil_tests/date_functions_tests.rs`

 * *Files identical despite different names*

### Comparing `rusty_chrono-0.1.1/src/dateutil/dateutil_tests/date_parsing_tests.rs` & `rusty_chrono-0.1.2/src/dateutil/dateutil_tests/date_parsing_tests.rs`

 * *Files identical despite different names*

### Comparing `rusty_chrono-0.1.1/src/dateutil/time_fractions.rs` & `rusty_chrono-0.1.2/src/dateutil/time_fractions.rs`

 * *Files identical despite different names*

### Comparing `rusty_chrono-0.1.1/src/lib.rs` & `rusty_chrono-0.1.2/src/lib.rs`

 * *Files identical despite different names*

### Comparing `rusty_chrono-0.1.1/test.py` & `rusty_chrono-0.1.2/test.py`

 * *Files identical despite different names*

### Comparing `rusty_chrono-0.1.1/Cargo.lock` & `rusty_chrono-0.1.2/Cargo.lock`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,18 @@
 # This file is automatically @generated by Cargo.
 # It is not intended for manual editing.
 version = 3
 
 [[package]]
+name = "android-tzdata"
+version = "0.1.1"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "e999941b234f3131b00bc13c22d06e8c5ff726d1b6318ac7eb276997bbb4fef0"
+
+[[package]]
 name = "android_system_properties"
 version = "0.1.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "819e7219dbd41043ac279b19830f2efc897156490d7fd6ea916720117ee66311"
 dependencies = [
  "libc",
 ]
@@ -21,17 +27,17 @@
 name = "bitflags"
 version = "1.3.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "bef38d45163c2f1dde094a7dfd33ccf595c92905c8f8f4fdc18d06fb1037718a"
 
 [[package]]
 name = "bumpalo"
-version = "3.12.2"
+version = "3.13.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "3c6ed94e98ecff0c12dd1b04c15ec0d7d9458ca8fe806cea6f12954efe74c63b"
+checksum = "a3e2c3daef883ecc1b5d58c15adae93470a91d425f3532ba1695849656af3fc1"
 
 [[package]]
 name = "cc"
 version = "1.0.79"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "50d30906286121d95be3d479533b458f87493b30a4b5f79a607db8f5d11aa91f"
 
@@ -39,38 +45,38 @@
 name = "cfg-if"
 version = "1.0.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "baf1de4339761588bc0619e3cbc0120ee582ebb74b53b4efbf79117bd2da40fd"
 
 [[package]]
 name = "chrono"
-version = "0.4.24"
+version = "0.4.26"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "4e3c5919066adf22df73762e50cffcde3a758f2a848b113b586d1f86728b673b"
+checksum = "ec837a71355b28f6556dbd569b37b3f363091c0bd4b2e735674521b4c5fd9bc5"
 dependencies = [
+ "android-tzdata",
  "iana-time-zone",
  "js-sys",
- "num-integer",
  "num-traits",
  "time",
  "wasm-bindgen",
  "winapi",
 ]
 
 [[package]]
 name = "core-foundation-sys"
 version = "0.8.4"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "e496a50fda8aacccc86d7529e2c1e0892dbd0f898a6b5645b5561b89c3210efa"
 
 [[package]]
 name = "iana-time-zone"
-version = "0.1.56"
+version = "0.1.57"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "0722cd7114b7de04316e7ea5456a0bbb20e4adb46fd27a3697adb812cff0f37c"
+checksum = "2fad5b825842d2b38bd206f3e81d6957625fd7f0a361e345c30e01a0ae2dd613"
 dependencies = [
  "android_system_properties",
  "core-foundation-sys",
  "iana-time-zone-haiku",
  "js-sys",
  "wasm-bindgen",
  "windows",
@@ -89,79 +95,66 @@
 name = "indoc"
 version = "1.0.9"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "bfa799dd5ed20a7e349f3b4639aa80d74549c81716d9ec4f994c9b5815598306"
 
 [[package]]
 name = "js-sys"
-version = "0.3.63"
+version = "0.3.64"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "2f37a4a5928311ac501dee68b3c7613a1037d0edb30c8e5427bd832d55d1b790"
+checksum = "c5f195fe497f702db0f318b07fdd68edb16955aed830df8363d837542f8f935a"
 dependencies = [
  "wasm-bindgen",
 ]
 
 [[package]]
 name = "libc"
-version = "0.2.144"
+version = "0.2.147"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "2b00cc1c228a6782d0f076e7b232802e0c5689d41bb5df366f2a6b6621cfdfe1"
+checksum = "b4668fb0ea861c1df094127ac5f1da3409a82116a4ba74fca2e58ef927159bb3"
 
 [[package]]
 name = "lock_api"
 version = "0.4.10"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "c1cc9717a20b1bb222f333e6a92fd32f7d8a18ddc5a3191a11af45dcbf4dcd16"
 dependencies = [
  "autocfg",
  "scopeguard",
 ]
 
 [[package]]
 name = "log"
-version = "0.4.17"
+version = "0.4.19"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "abb12e687cfb44aa40f41fc3978ef76448f9b6038cad6aef4259d3c095a2382e"
-dependencies = [
- "cfg-if",
-]
+checksum = "b06a4cde4c0f271a446782e3eff8de789548ce57dbc8eca9292c27f4a42004b4"
 
 [[package]]
 name = "memoffset"
 version = "0.9.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "5a634b1c61a95585bd15607c6ab0c4e5b226e695ff2800ba0cdccddf208c406c"
 dependencies = [
  "autocfg",
 ]
 
 [[package]]
-name = "num-integer"
-version = "0.1.45"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "225d3389fb3509a24c93f5c29eb6bde2586b98d9f016636dff58d7c6f7569cd9"
-dependencies = [
- "autocfg",
- "num-traits",
-]
-
-[[package]]
 name = "num-traits"
-version = "0.2.15"
+version = "0.2.16"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "578ede34cf02f8924ab9447f50c28075b4d3e5b269972345e7e0372b38c6cdcd"
+checksum = "f30b0abd723be7e2ffca1272140fac1a2f084c77ec3e123c192b66af1ee9e6c2"
 dependencies = [
  "autocfg",
 ]
 
 [[package]]
 name = "once_cell"
-version = "1.17.1"
+version = "1.18.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "b7e5500299e16ebb147ae15a00a942af264cf3688f47923b8fc2cd5858f23ad3"
+checksum = "dd8b5dd2ae5ed71462c540258bedcb51965123ad7e7ccf4b9a8cafaa4a63576d"
 
 [[package]]
 name = "parking_lot"
 version = "0.12.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "3742b2c103b9f06bc9fff0a37ff4912935851bee6d36f3c02bcc755bcfec228f"
 dependencies = [
@@ -204,17 +197,17 @@
  "proc-macro2",
  "quote",
  "version_check",
 ]
 
 [[package]]
 name = "proc-macro2"
-version = "1.0.57"
+version = "1.0.66"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "c4ec6d5fe0b140acb27c9a0444118cf55bfbb4e0b259739429abb4521dd67c16"
+checksum = "18fb31db3f9bddb2ea821cde30a9f70117e3f119938b5ee630b7403aa6e2ead9"
 dependencies = [
  "unicode-ident",
 ]
 
 [[package]]
 name = "pyo3"
 version = "0.19.1"
@@ -273,17 +266,17 @@
  "proc-macro2",
  "quote",
  "syn 1.0.109",
 ]
 
 [[package]]
 name = "quote"
-version = "1.0.27"
+version = "1.0.32"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "8f4f29d145265ec1c483c7c654450edde0bfe043d3938d6972630663356d9500"
+checksum = "50f3b39ccfb720540debaa0164757101c08ecb8d326b15358ce76a62c7e85965"
 dependencies = [
  "proc-macro2",
 ]
 
 [[package]]
 name = "redox_syscall"
 version = "0.3.5"
@@ -291,15 +284,15 @@
 checksum = "567664f262709473930a4bf9e51bf2ebf3348f2e748ccc50dea20646858f8f29"
 dependencies = [
  "bitflags",
 ]
 
 [[package]]
 name = "rusty_chrono"
-version = "0.1.1"
+version = "0.1.2"
 dependencies = [
  "chrono",
  "pyo3",
  "test-case",
 ]
 
 [[package]]
@@ -323,17 +316,17 @@
  "proc-macro2",
  "quote",
  "unicode-ident",
 ]
 
 [[package]]
 name = "syn"
-version = "2.0.16"
+version = "2.0.27"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "a6f671d4b5ffdb8eadec19c0ae67fe2639df8684bd7bc4b83d986b8db549cf01"
+checksum = "b60f673f44a8255b9c8c657daf66a596d435f2da81a555b06dc644d080ba45e0"
 dependencies = [
  "proc-macro2",
  "quote",
  "unicode-ident",
 ]
 
 [[package]]
@@ -386,17 +379,17 @@
  "libc",
  "wasi",
  "winapi",
 ]
 
 [[package]]
 name = "unicode-ident"
-version = "1.0.8"
+version = "1.0.11"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "e5464a87b239f13a63a501f2701565754bae92d243d4bb7eb12f6d57d2269bf4"
+checksum = "301abaae475aa91687eb82514b328ab47a211a533026cb25fc3e519b86adfc3c"
 
 [[package]]
 name = "unindent"
 version = "0.1.11"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "e1766d682d402817b5ac4490b3c3002d91dfa0d22812f341609f97b08757359c"
 
@@ -410,65 +403,65 @@
 name = "wasi"
 version = "0.10.0+wasi-snapshot-preview1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "1a143597ca7c7793eff794def352d41792a93c481eb1042423ff7ff72ba2c31f"
 
 [[package]]
 name = "wasm-bindgen"
-version = "0.2.86"
+version = "0.2.87"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "5bba0e8cb82ba49ff4e229459ff22a191bbe9a1cb3a341610c9c33efc27ddf73"
+checksum = "7706a72ab36d8cb1f80ffbf0e071533974a60d0a308d01a5d0375bf60499a342"
 dependencies = [
  "cfg-if",
  "wasm-bindgen-macro",
 ]
 
 [[package]]
 name = "wasm-bindgen-backend"
-version = "0.2.86"
+version = "0.2.87"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "19b04bc93f9d6bdee709f6bd2118f57dd6679cf1176a1af464fca3ab0d66d8fb"
+checksum = "5ef2b6d3c510e9625e5fe6f509ab07d66a760f0885d858736483c32ed7809abd"
 dependencies = [
  "bumpalo",
  "log",
  "once_cell",
  "proc-macro2",
  "quote",
- "syn 2.0.16",
+ "syn 2.0.27",
  "wasm-bindgen-shared",
 ]
 
 [[package]]
 name = "wasm-bindgen-macro"
-version = "0.2.86"
+version = "0.2.87"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "14d6b024f1a526bb0234f52840389927257beb670610081360e5a03c5df9c258"
+checksum = "dee495e55982a3bd48105a7b947fd2a9b4a8ae3010041b9e0faab3f9cd028f1d"
 dependencies = [
  "quote",
  "wasm-bindgen-macro-support",
 ]
 
 [[package]]
 name = "wasm-bindgen-macro-support"
-version = "0.2.86"
+version = "0.2.87"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "e128beba882dd1eb6200e1dc92ae6c5dbaa4311aa7bb211ca035779e5efc39f8"
+checksum = "54681b18a46765f095758388f2d0cf16eb8d4169b639ab575a8f5693af210c7b"
 dependencies = [
  "proc-macro2",
  "quote",
- "syn 2.0.16",
+ "syn 2.0.27",
  "wasm-bindgen-backend",
  "wasm-bindgen-shared",
 ]
 
 [[package]]
 name = "wasm-bindgen-shared"
-version = "0.2.86"
+version = "0.2.87"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "ed9d5b4305409d1fc9482fee2d7f9bcbf24b3972bf59817ef757e23982242a93"
+checksum = "ca6ad05a4870b2bf5fe995117d3728437bd27d7cd5f06f13c17443ef369775a1"
 
 [[package]]
 name = "winapi"
 version = "0.3.9"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "5c839a674fcd7a98952e593242ea400abe93992746761e38641405d28b00f419"
 dependencies = [
@@ -495,17 +488,17 @@
 checksum = "e686886bc078bc1b0b600cac0147aadb815089b6e4da64016cbd754b6342700f"
 dependencies = [
  "windows-targets",
 ]
 
 [[package]]
 name = "windows-targets"
-version = "0.48.0"
+version = "0.48.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "7b1eb6f0cd7c80c79759c929114ef071b87354ce476d9d94271031c0497adfd5"
+checksum = "05d4b17490f70499f20b9e791dcf6a299785ce8af4d709018206dc5b4953e95f"
 dependencies = [
  "windows_aarch64_gnullvm",
  "windows_aarch64_msvc",
  "windows_i686_gnu",
  "windows_i686_msvc",
  "windows_x86_64_gnu",
  "windows_x86_64_gnullvm",
```

