# Comparing `tmp/moss_decoder-0.4.3.tar.gz` & `tmp/moss_decoder-0.5.0.tar.gz`

## Comparing `moss_decoder-0.4.3.tar` & `moss_decoder-0.5.0.tar`

### file list

```diff
@@ -1,24 +1,30 @@
--rw-r--r--   0        0        0      962 1970-01-01 00:00:00.000000 moss_decoder-0.4.3/Cargo.toml
--rw-r--r--   0     1001      123      633 2023-07-26 15:05:22.000000 moss_decoder-0.4.3/.CERN-gitlab-ci.yml
--rw-r--r--   0     1001      123     2835 2023-07-26 15:05:22.000000 moss_decoder-0.4.3/.github/workflows/CI.yml
--rw-r--r--   0     1001      123      373 2023-07-26 15:05:22.000000 moss_decoder-0.4.3/.github/workflows/bench-py.yml
--rw-r--r--   0     1001      123      404 2023-07-26 15:05:22.000000 moss_decoder-0.4.3/.github/workflows/rust.yml
--rw-r--r--   0     1001      123      714 2023-07-26 15:05:22.000000 moss_decoder-0.4.3/.gitignore
--rw-r--r--   0     1001      123      757 2023-07-26 15:05:22.000000 moss_decoder-0.4.3/.pre-commit-config.yaml
--rw-r--r--   0     1001      123     3100 2023-07-26 15:05:22.000000 moss_decoder-0.4.3/README.md
--rw-r--r--   0     1001      123      874 2023-07-26 15:05:22.000000 moss_decoder-0.4.3/moss_decoder.pyi
--rw-r--r--   0     1001      123      641 2023-07-26 15:05:22.000000 moss_decoder-0.4.3/pyproject.toml
--rw-r--r--   0     1001      123  4458776 2023-07-26 15:05:22.000000 moss_decoder-0.4.3/python310.dll
--rw-r--r--   0     1001      123     9630 2023-07-26 15:05:22.000000 moss_decoder-0.4.3/src/lib.rs
--rw-r--r--   0     1001      123     1880 2023-07-26 15:05:22.000000 moss_decoder-0.4.3/src/moss_protocol/moss_hit.rs
--rw-r--r--   0     1001      123     1843 2023-07-26 15:05:22.000000 moss_decoder-0.4.3/src/moss_protocol/moss_packet.rs
--rw-r--r--   0     1001      123     1674 2023-07-26 15:05:22.000000 moss_decoder-0.4.3/src/moss_protocol.rs
--rwxr-xr-x   0     1001      123      427 2023-07-26 15:05:22.000000 moss_decoder-0.4.3/tests/bench_dev_vs_prod.sh
--rw-r--r--   0     1001      123     7102 2023-07-26 15:05:22.000000 moss_decoder-0.4.3/tests/integration.py
--rw-r--r--   0     1001      123     6118 2023-07-26 15:05:22.000000 moss_decoder-0.4.3/tests/integration_test.rs
--rw-r--r--   0     1001      123  9582576 2023-07-26 15:05:22.000000 moss_decoder-0.4.3/tests/moss_noise.raw
--rwxr-xr-x   0     1001      123     1190 2023-07-26 15:05:22.000000 moss_decoder-0.4.3/tests/performance_dev_py.sh
--rwxr-xr-x   0     1001      123      820 2023-07-26 15:05:22.000000 moss_decoder-0.4.3/tests/performance_prod_py.sh
--rw-r--r--   0     1001      123      895 2023-07-26 15:05:22.000000 moss_decoder-0.4.3/tests/utils.sh
--rw-r--r--   0     1001      123     8066 2023-07-26 15:05:22.000000 moss_decoder-0.4.3/Cargo.lock
--rw-r--r--   0        0        0     3654 1970-01-01 00:00:00.000000 moss_decoder-0.4.3/PKG-INFO
+-rw-r--r--   0        0        0     1057 1970-01-01 00:00:00.000000 moss_decoder-0.5.0/Cargo.toml
+-rw-r--r--   0     1001      123      633 2023-07-30 08:49:32.000000 moss_decoder-0.5.0/.CERN-gitlab-ci.yml
+-rw-r--r--   0     1001      123     2835 2023-07-30 08:49:32.000000 moss_decoder-0.5.0/.github/workflows/CI.yml
+-rw-r--r--   0     1001      123      373 2023-07-30 08:49:32.000000 moss_decoder-0.5.0/.github/workflows/bench-py.yml
+-rw-r--r--   0     1001      123      404 2023-07-30 08:49:32.000000 moss_decoder-0.5.0/.github/workflows/rust.yml
+-rw-r--r--   0     1001      123      714 2023-07-30 08:49:32.000000 moss_decoder-0.5.0/.gitignore
+-rw-r--r--   0     1001      123      757 2023-07-30 08:49:32.000000 moss_decoder-0.5.0/.pre-commit-config.yaml
+-rw-r--r--   0     1001      123     7244 2023-07-30 08:49:32.000000 moss_decoder-0.5.0/README.md
+-rw-r--r--   0     1001      123      360 2023-07-30 08:49:32.000000 moss_decoder-0.5.0/benches/benchmark.rs
+-rw-r--r--   0     1001      123      555 2023-07-30 08:49:32.000000 moss_decoder-0.5.0/benches/decode_from_file_bench.rs
+-rw-r--r--   0     1001      123      859 2023-07-30 08:49:32.000000 moss_decoder-0.5.0/benches/decode_multiple_events_bench.rs
+-rw-r--r--   0     1001      123      839 2023-07-30 08:49:32.000000 moss_decoder-0.5.0/benches/decode_single_event_bench.rs
+-rw-r--r--   0     1001      123     1099 2023-07-30 08:49:32.000000 moss_decoder-0.5.0/moss_decoder.pyi
+-rw-r--r--   0     1001      123      641 2023-07-30 08:49:32.000000 moss_decoder-0.5.0/pyproject.toml
+-rw-r--r--   0     1001      123  4458776 2023-07-30 08:49:32.000000 moss_decoder-0.5.0/python310.dll
+-rw-r--r--   0     1001      123    20323 2023-07-30 08:49:32.000000 moss_decoder-0.5.0/src/lib.rs
+-rw-r--r--   0     1001      123     1880 2023-07-30 08:49:32.000000 moss_decoder-0.5.0/src/moss_protocol/moss_hit.rs
+-rw-r--r--   0     1001      123     1854 2023-07-30 08:49:32.000000 moss_decoder-0.5.0/src/moss_protocol/moss_packet.rs
+-rw-r--r--   0     1001      123     1762 2023-07-30 08:49:32.000000 moss_decoder-0.5.0/src/moss_protocol.rs
+-rw-r--r--   0     1001      123    10569 2023-07-30 08:49:32.000000 moss_decoder-0.5.0/src/moss_protocol_fsm.rs
+-rw-r--r--   0     1001      123    11217 2023-07-30 08:49:32.000000 moss_decoder-0.5.0/src/moss_protocol_nested_fsm.rs
+-rwxr-xr-x   0     1001      123      427 2023-07-30 08:49:32.000000 moss_decoder-0.5.0/tests/bench_dev_vs_prod.sh
+-rw-r--r--   0     1001      123     7400 2023-07-30 08:49:32.000000 moss_decoder-0.5.0/tests/integration.py
+-rw-r--r--   0     1001      123     9194 2023-07-30 08:49:32.000000 moss_decoder-0.5.0/tests/integration_test.rs
+-rw-r--r--   0     1001      123  9582576 2023-07-30 08:49:32.000000 moss_decoder-0.5.0/tests/moss_noise.raw
+-rwxr-xr-x   0     1001      123     1190 2023-07-30 08:49:32.000000 moss_decoder-0.5.0/tests/performance_dev_py.sh
+-rwxr-xr-x   0     1001      123      820 2023-07-30 08:49:32.000000 moss_decoder-0.5.0/tests/performance_prod_py.sh
+-rw-r--r--   0     1001      123      895 2023-07-30 08:49:32.000000 moss_decoder-0.5.0/tests/utils.sh
+-rw-r--r--   0     1001      123    24141 2023-07-30 08:49:32.000000 moss_decoder-0.5.0/Cargo.lock
+-rw-r--r--   0        0        0     7798 1970-01-01 00:00:00.000000 moss_decoder-0.5.0/PKG-INFO
```

### Comparing `moss_decoder-0.4.3/Cargo.toml` & `moss_decoder-0.5.0/Cargo.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,25 +1,33 @@
 [package]
 name = "moss_decoder"
-version = "0.4.3"
+version = "0.5.0"
 edition = "2021"
 authors = ["Marc Beck König <mbkj@tutamail.com>"]
 license = "MIT OR Apache-2.0"
 description = "Python module providing a decoder for the MOSS chip protocol."
 categories = ["python-module"]
 
 
 
 # See more keys and their definitions at https://doc.rust-lang.org/cargo/reference/manifest.html
 [lib]
 name = "moss_decoder"
 crate-type = ["cdylib", "rlib"]
 
+[dependencies]
+sm = "0.9.0"
+
 [dev-dependencies]
 pretty_assertions = "1.4.0"
+criterion = "0.5.1"
+
+[[bench]]
+name = "benchmark"
+harness = false
 
 [dependencies.pyo3]
 version = "*"
 
 [features]
 # Fix for linker issues with `cargo test`
 ## Works now by running `cargo test --no-default-features
```

### Comparing `moss_decoder-0.4.3/.CERN-gitlab-ci.yml` & `moss_decoder-0.5.0/.CERN-gitlab-ci.yml`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -19,13 +19,13 @@
     when: manual
     needs: []
     dependencies: []
     cache: []
     image: ${DOCKER_REGISTRY}/python-rust
     script:
         - python -m pip install maturin
-        - maturin build --release
         - PATH="/root/.cargo/bin:${PATH}"
+        - maturin build --release
     artifacts:
         name: "${CI_COMMIT_SHA}"
         paths:
         - $CI_PROJECT_DIR/target/
```

### Comparing `moss_decoder-0.4.3/.github/workflows/CI.yml` & `moss_decoder-0.5.0/.github/workflows/CI.yml`

 * *Files identical despite different names*

### Comparing `moss_decoder-0.4.3/.gitignore` & `moss_decoder-0.5.0/.gitignore`

 * *Files identical despite different names*

### Comparing `moss_decoder-0.4.3/.pre-commit-config.yaml` & `moss_decoder-0.5.0/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `moss_decoder-0.4.3/moss_decoder.pyi` & `moss_decoder-0.5.0/moss_decoder.pyi`

 * *Files 9% similar despite different names*

```diff
@@ -24,7 +24,11 @@
         self.unit_id = unit_id
         self.hits = []
 
 def decode_event(raw_bytes: bytes) -> tuple[MossPacket, int]: ...
 def decode_event_noexcept(raw_bytes: bytes) -> tuple[MossPacket, int]: ...
 def decode_multiple_events(raw_bytes: bytes) -> tuple[list[MossPacket], int]: ...
 def decode_from_file(path: str | Path) -> list[MossPacket]: ...
+
+def decode_event_fsm(raw_bytes: bytes) -> tuple[MossPacket, int]: ...
+def decode_multiple_events_fsm(raw_bytes: bytes) -> tuple[list[MossPacket], int]: ...
+def decode_from_file_fsm(path: str | Path) -> list[MossPacket]: ...
```

### Comparing `moss_decoder-0.4.3/pyproject.toml` & `moss_decoder-0.5.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `moss_decoder-0.4.3/python310.dll` & `moss_decoder-0.5.0/python310.dll`

 * *Files identical despite different names*

### Comparing `moss_decoder-0.4.3/src/moss_protocol/moss_hit.rs` & `moss_decoder-0.5.0/src/moss_protocol/moss_hit.rs`

 * *Files identical despite different names*

### Comparing `moss_decoder-0.4.3/src/moss_protocol/moss_packet.rs` & `moss_decoder-0.5.0/src/moss_protocol/moss_packet.rs`

 * *Files 5% similar despite different names*

```diff
@@ -13,15 +13,15 @@
     /// The hits in the packet.
     pub hits: Vec<MossHit>,
 }
 
 #[pymethods]
 impl MossPacket {
     #[new]
-    fn new(unit_id: u8) -> Self {
+    pub(crate) fn new(unit_id: u8) -> Self {
         Self {
             unit_id,
             hits: Vec::new(),
         }
     }
 
     fn __repr__(slf: &PyCell<Self>) -> PyResult<String> {
```

### Comparing `moss_decoder-0.4.3/src/moss_protocol.rs` & `moss_decoder-0.5.0/src/moss_protocol.rs`

 * *Files 14% similar despite different names*

```diff
@@ -14,22 +14,22 @@
     Data1,
     Data2,
     Delimiter,
     ProtocolError,
 }
 
 impl MossWord {
-    const IDLE: u8 = 0xFF; // 1111_1111 (default)
-    const UNIT_FRAME_HEADER: u8 = 0b1101_0000; // 1101_<unit_id[3:0]>
-    const UNIT_FRAME_TRAILER: u8 = 0b1110_0000; // 1110_0000
-    const REGION_HEADER: u8 = 0b1100_0000; // 1100_00_<region_id[1:0]>
-    const DATA_0: u8 = 0b0000_0000; // 00_<hit_row_pos[8:3]>
-    const DATA_1: u8 = 0b0100_0000; // 01_<hit_row_pos[2:0]>_<hit_col_pos[8:6]>
-    const DATA_2: u8 = 0b1000_0000; // 10_<hit_col_pos[5:0]>
-    const DELIMITER: u8 = 0xFA; // subject to change (FPGA implementation detail)
+    pub(super) const IDLE: u8 = 0xFF; // 1111_1111 (default)
+    pub(super) const UNIT_FRAME_HEADER: u8 = 0b1101_0000; // 1101_<unit_id[3:0]>
+    pub(super) const UNIT_FRAME_TRAILER: u8 = 0b1110_0000; // 1110_0000
+    pub(super) const REGION_HEADER: u8 = 0b1100_0000; // 1100_00_<region_id[1:0]>
+    pub(super) const DATA_0: u8 = 0b0000_0000; // 00_<hit_row_pos[8:3]>
+    pub(super) const DATA_1: u8 = 0b0100_0000; // 01_<hit_row_pos[2:0]>_<hit_col_pos[8:6]>
+    pub(super) const DATA_2: u8 = 0b1000_0000; // 10_<hit_col_pos[5:0]>
+    pub(super) const DELIMITER: u8 = 0xFA; // subject to change (FPGA implementation detail)
 
     pub fn from_byte(b: u8) -> MossWord {
         match b {
             // Exact matches
             Self::IDLE => MossWord::Idle,
             Self::UNIT_FRAME_TRAILER => MossWord::UnitFrameTrailer,
             six_msb if six_msb & 0xFC == Self::REGION_HEADER => MossWord::RegionHeader,
```

### Comparing `moss_decoder-0.4.3/tests/integration.py` & `moss_decoder-0.5.0/tests/integration.py`

 * *Files 1% similar despite different names*

```diff
@@ -43,39 +43,44 @@
         + region_header_3
         + unit_frame_trailer
         + padding
     )
     return simple_packet
 
 
-def decode_multi_event(raw_bytes: bytes) -> tuple[list["MossPacket"], int]:
+def decode_multi_event(raw_bytes: bytes, fsm: bool = False) -> tuple[list["MossPacket"], int]:
     """Takes `bytes` and decodes it as `MossPacket`s.
     returns a tuple of `list[MossPackets]` and an int that indicates the
     index where the last MOSS trailer was seen
     """
-    packets, last_trailer_idx = moss_decoder.decode_multiple_events(raw_bytes)
+    if fsm is True:
+        packets, last_trailer_idx = moss_decoder.decode_multiple_events_fsm(
+        raw_bytes)
+    else:
+        packets, last_trailer_idx = moss_decoder.decode_multiple_events(
+        raw_bytes)
 
     return packets, last_trailer_idx
 
 
-def test_decode_multi_event():
+def test_decode_multi_event(fsm: bool = False):
     """Test that multiple events are correctly decoded from raw bytes"""
     print(
         (
-            "=== Test that multiple events \
-           are correctly decoded from raw bytes ==="
+            "=== Test that multiple events"
+            "are correctly decoded from raw bytes ==="
         )
     )
     raw_bytes = read_bytes_from_file(FILE_PATH)
     byte_count = len(raw_bytes)
     last_byte_idx = byte_count - 1
 
     print(f"Read {byte_count} bytes")
 
-    packets, last_trailer_idx = decode_multi_event(raw_bytes=raw_bytes)
+    packets, last_trailer_idx = decode_multi_event(raw_bytes=raw_bytes, fsm=fsm)
 
     print(f"Decoded {len(packets)} packets")
 
     print(f"Last trailer at index: {last_trailer_idx}/{last_byte_idx}")
     remainder_count = last_byte_idx - last_trailer_idx
     print(f"Remainder: {remainder_count} byte(s)")
 
@@ -217,14 +222,17 @@
 
     test_fundamental_class_comparisons()
 
     start = time.time()
     test_decode_multi_event()
     print(f"Done in: {time.time()-start:.3f} s\n")
     start = time.time()
+    test_decode_multi_event(fsm=True)
+    print(f"Done in: {time.time()-start:.3f} s\n")
+    start = time.time()
     test_moss_packet_print()
     print(f"Done in: {time.time()-start:.3f} s\n")
     start = time.time()
     test_100k_single_decodes()
     print(f"Done in: {time.time()-start:.3f} s\n")
     start = time.time()
     test_100k_single_decodes(noexcept=True)
```

### Comparing `moss_decoder-0.4.3/tests/moss_noise.raw` & `moss_decoder-0.5.0/tests/moss_noise.raw`

 * *Files identical despite different names*

### Comparing `moss_decoder-0.4.3/tests/performance_dev_py.sh` & `moss_decoder-0.5.0/tests/performance_dev_py.sh`

 * *Files identical despite different names*

### Comparing `moss_decoder-0.4.3/tests/performance_prod_py.sh` & `moss_decoder-0.5.0/tests/performance_prod_py.sh`

 * *Files identical despite different names*

### Comparing `moss_decoder-0.4.3/tests/utils.sh` & `moss_decoder-0.5.0/tests/utils.sh`

 * *Files identical despite different names*

