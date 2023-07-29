# Comparing `tmp/tinyfive-0.0.15.tar.gz` & `tmp/tinyfive-1.0.0.tar.gz`

## Comparing `tinyfive-0.0.15.tar` & `tinyfive-1.0.0.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 tinyfive-0.0.15/tinyfive/__init__.py
--rw-r--r--   0        0        0    32329 2020-02-02 00:00:00.000000 tinyfive-0.0.15/tinyfive/machine.py
--rw-r--r--   0        0        0     1068 2020-02-02 00:00:00.000000 tinyfive-0.0.15/LICENSE
--rw-r--r--   0        0        0    28769 2020-02-02 00:00:00.000000 tinyfive-0.0.15/README.md
--rw-r--r--   0        0        0      925 2020-02-02 00:00:00.000000 tinyfive-0.0.15/pyproject.toml
--rw-r--r--   0        0        0    29369 2020-02-02 00:00:00.000000 tinyfive-0.0.15/PKG-INFO
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 tinyfive-1.0.0/tinyfive/__init__.py
+-rw-r--r--   0        0        0    32329 2020-02-02 00:00:00.000000 tinyfive-1.0.0/tinyfive/machine.py
+-rw-r--r--   0        0        0     1068 2020-02-02 00:00:00.000000 tinyfive-1.0.0/LICENSE
+-rw-r--r--   0        0        0    28463 2020-02-02 00:00:00.000000 tinyfive-1.0.0/README.md
+-rw-r--r--   0        0        0      998 2020-02-02 00:00:00.000000 tinyfive-1.0.0/pyproject.toml
+-rw-r--r--   0        0        0    29062 2020-02-02 00:00:00.000000 tinyfive-1.0.0/PKG-INFO
```

### Comparing `tinyfive-0.0.15/tinyfive/machine.py` & `tinyfive-1.0.0/tinyfive/machine.py`

 * *Files identical despite different names*

### Comparing `tinyfive-0.0.15/LICENSE` & `tinyfive-1.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `tinyfive-0.0.15/README.md` & `tinyfive-1.0.0/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -381,15 +381,14 @@
 # Output: True
 ```
 The table below shows a speedup of 1.7 with the following caveats:
 - The bit-widths don't make sense for fixed point (in general, multiplying two 32-bit integers produces a 64-bit product; and adding 4 of these products requires up to 66 bits).
 - For runtime calculations, we assume that our RISC-V CPU can only perform one instruction per cycle (while many RISC-V cores can perform multiple instructions per cycle).
 - We assume all 31 registers can be used, which is unrealistic because we ignore register allocation conventions such as the procedure
 calling conventions specified [here](https://github.com/riscv-non-isa/riscv-elf-psabi-doc).
-- For 16x16 or larger matrices, [Strassen's algorithm](https://en.wikipedia.org/wiki/Strassen_algorithm) and [DeepMind's AlphaTensor](https://www.deepmind.com/blog/discovering-novel-algorithms-with-alphatensor) can reduce the total number of multiplications and additions if they are applied recursively.
 
 |             | Image | Registers | Load | Store | Mul | Add | Branch | Total ops | Speedup |
 |:-----------:|:-----:|:---------:|:----:|:-----:|:---:|:---:|:------:|:---------:|:-------:|
 | Example 3.3 | 92B   | 9         | 80   | 16    | 64  | 89  | 20     | 269       | 1       |
 | Example 3.4 | 640B  | 22        | 32   | 16    | 64  | 48  | 0      | 160       | 1.7     |
 
 ### Example 4: Neural network layers
@@ -450,15 +449,15 @@
 - TinyFive is still under construction, many things haven't been implemented and tested yet.
 - 37 of the 40 base instructions (RV32I), all instructions of the M-extension (RV32M) and the F-extension (RV32F) with the default rounding mode are already implemented, and many of them are tested.  (The three missing RV32I instructions `fence`, `ebreak`, and `ecall` are not applicable here.)
 - Remaining work: improve testing, add more extensions. See TODOs in the code for more details.
 - Stay updated by following us on [Twitter](https://twitter.com/OpenMachine_AI), [Post.news](https://post.news/@/openmachine), and [LinkedIn](https://www.linkedin.com/in/nilsgraef/).
 
 ## Speed
 - TinyFive is not optimized for speed (but for ease-of-use and [LOC](https://en.wikipedia.org/wiki/Source_lines_of_code)).
-- You might be able to use [Codon](https://github.com/exaloop/codon) or PyPy to speed up TinyFive (see e.g. the [Pydgin paper](https://www.csl.cornell.edu/~berkin/ilbeyi-pydgin-riscv2016.pdf) for details).
+- You might be able to use PyPy or [Codon](https://github.com/exaloop/codon) to speed up TinyFive (see e.g. the [Pydgin paper](https://www.csl.cornell.edu/~berkin/ilbeyi-pydgin-riscv2016.pdf) for details).
 - If you only use the upper-case instructions such as `ADD()`, then TinyFive is very fast because there is no instruction decoding. And you should be able to accelerate it on a GPU or TPU.
 - If you use the lower-case instructions with `asm()` and `exe()`, then execution of these functions is slow as they involve look-up and string matching with O(n) complexity where "n" is the total number of instructions. The current implementations of `asm()` and `dec()` are optimized for ease-of-use and readability. A faster implementation would collapse multiple look-ups into one look-up, optimize the pattern-matching for the instruction decoding (bits -> instruction), and change the order of the instructions so that more frequently used instructions are at the top of the list. [Here is an older version](https://github.com/OpenMachine-ai/tinyfive/blob/2aa4987391561c9c6692602ed3fccdeaee333e0b/tinyfive.py) of TinyFive with a faster `dec()` function that collapses two look-ups (`bits -> instruction` and `instruction -> uppeer-case instruction`) and doesn't use `fnmatch`.
 
 ## Comparison
 The table below compares TinyFive with other [ISS](https://en.wikipedia.org/wiki/Instruction_set_simulator) and emulator projects.
 
 | ISS | Author | Language | Mature? | Extensions | LOC |
@@ -471,15 +470,15 @@
 | [riscvOVPsim](https://github.com/riscv-ovpsim/imperas-riscv-tests) | Imperas              | C         | Yes              | All           | |
 | [Whisper](https://github.com/chipsalliance/SweRV-ISS)              | Western Digital      | C, C++    | Yes | Almost all                 | |
 | [Sail Model](https://github.com/riscv/sail-riscv)                  | Cambridge, Edinburgh | Sail, C   | Yes | All                        | |
 | [PiMaker/rvc](https://github.com/PiMaker/rvc)                      | PiMaker              | C         |     |                            | |
 | [mini-rv32ima](https://github.com/cnlohr/mini-rv32ima)             | Charles Lohr         | C         |     | A, I, M, Zifencei, Zicsr   | < 1k |
 
 ## References
-- [HuggingFive :raised_hand_with_fingers_splayed:](https://github.com/OpenMachine-ai/HuggingFive)
+- [HuggingFive:raised_hand_with_fingers_splayed:](https://github.com/OpenMachine-ai/HuggingFive)
 - Official [RISC-V spec](https://github.com/riscv/riscv-isa-manual/releases/download/Ratified-IMAFDQC/riscv-spec-20191213.pdf)
 - See [this RISC-V card](https://inst.eecs.berkeley.edu/~cs61c/fa18/img/riscvcard.pdf) for a brief description of most instructions. See also the [RISC-V reference card](http://riscvbook.com/greencard-20181213.pdf).
 - Book [The RISC-V Reader: An Open Architecture Atlas](https://www.abebooks.com/book-search/author/patterson-david-waterman-andrew/) by David Patterson and Andrew Waterman. Appendix A of this book defines all instructions. The Spanish version of this book is [available for free](http://riscvbook.com/spanish/guia-practica-de-risc-v-1.0.5.pdf),
 other free versions are [available here](http://riscvbook.com).
 - Pydgin [paper](https://www.csl.cornell.edu/~berkin/ilbeyi-pydgin-riscv2016.pdf) and [video](https://youtu.be/-p_AGki7Vsk)
 - [Online simulator](https://ascslab.org/research/briscv/simulator/simulator.html) for debug
```

#### html2text {}

```diff
@@ -235,19 +235,15 @@
 caveats: - The bit-widths don't make sense for fixed point (in general,
 multiplying two 32-bit integers produces a 64-bit product; and adding 4 of
 these products requires up to 66 bits). - For runtime calculations, we assume
 that our RISC-V CPU can only perform one instruction per cycle (while many
 RISC-V cores can perform multiple instructions per cycle). - We assume all 31
 registers can be used, which is unrealistic because we ignore register
 allocation conventions such as the procedure calling conventions specified
-[here](https://github.com/riscv-non-isa/riscv-elf-psabi-doc). - For 16x16 or
-larger matrices, [Strassen's algorithm](https://en.wikipedia.org/wiki/
-Strassen_algorithm) and [DeepMind's AlphaTensor](https://www.deepmind.com/blog/
-discovering-novel-algorithms-with-alphatensor) can reduce the total number of
-multiplications and additions if they are applied recursively. | | Image |
+[here](https://github.com/riscv-non-isa/riscv-elf-psabi-doc). | | Image |
 Registers | Load | Store | Mul | Add | Branch | Total ops | Speedup | |:-------
 ----:|:-----:|:---------:|:----:|:-----:|:---:|:---:|:------:|:---------:|:----
 ---:| | Example 3.3 | 92B | 9 | 80 | 16 | 64 | 89 | 20 | 269 | 1 | | Example
 3.4 | 640B | 22 | 32 | 16 | 64 | 48 | 0 | 160 | 1.7 | ### Example 4: Neural
 network layers Coming soon, see [file layer_examples.py](layer_examples.py) for
 now ### Example 5: MobileNet Coming soon-ish, see [file mobilenet_v1_0.25.py]
 (mobilenet_v1_0.25.py) for now ## Running in colab [Colab] This is the quickest
@@ -280,19 +276,19 @@
 are already implemented, and many of them are tested. (The three missing RV32I
 instructions `fence`, `ebreak`, and `ecall` are not applicable here.) -
 Remaining work: improve testing, add more extensions. See TODOs in the code for
 more details. - Stay updated by following us on [Twitter](https://twitter.com/
 OpenMachine_AI), [Post.news](https://post.news/@/openmachine), and [LinkedIn]
 (https://www.linkedin.com/in/nilsgraef/). ## Speed - TinyFive is not optimized
 for speed (but for ease-of-use and [LOC](https://en.wikipedia.org/wiki/
-Source_lines_of_code)). - You might be able to use [Codon](https://github.com/
-exaloop/codon) or PyPy to speed up TinyFive (see e.g. the [Pydgin paper](https:
-//www.csl.cornell.edu/~berkin/ilbeyi-pydgin-riscv2016.pdf) for details). - If
-you only use the upper-case instructions such as `ADD()`, then TinyFive is very
-fast because there is no instruction decoding. And you should be able to
+Source_lines_of_code)). - You might be able to use PyPy or [Codon](https://
+github.com/exaloop/codon) to speed up TinyFive (see e.g. the [Pydgin paper]
+(https://www.csl.cornell.edu/~berkin/ilbeyi-pydgin-riscv2016.pdf) for details).
+- If you only use the upper-case instructions such as `ADD()`, then TinyFive is
+very fast because there is no instruction decoding. And you should be able to
 accelerate it on a GPU or TPU. - If you use the lower-case instructions with
 `asm()` and `exe()`, then execution of these functions is slow as they involve
 look-up and string matching with O(n) complexity where "n" is the total number
 of instructions. The current implementations of `asm()` and `dec()` are
 optimized for ease-of-use and readability. A faster implementation would
 collapse multiple look-ups into one look-up, optimize the pattern-matching for
 the instruction decoding (bits -> instruction), and change the order of the
@@ -314,17 +310,17 @@
 /en.wikipedia.org/wiki/Fabrice_Bellard) | C | Yes | All | | | [riscvOVPsim]
 (https://github.com/riscv-ovpsim/imperas-riscv-tests) | Imperas | C | Yes | All
 | | | [Whisper](https://github.com/chipsalliance/SweRV-ISS) | Western Digital |
 C, C++ | Yes | Almost all | | | [Sail Model](https://github.com/riscv/sail-
 riscv) | Cambridge, Edinburgh | Sail, C | Yes | All | | | [PiMaker/rvc](https:/
 /github.com/PiMaker/rvc) | PiMaker | C | | | | | [mini-rv32ima](https://
 github.com/cnlohr/mini-rv32ima) | Charles Lohr | C | | A, I, M, Zifencei, Zicsr
-| < 1k | ## References - [HuggingFive :raised_hand_with_fingers_splayed:]
-(https://github.com/OpenMachine-ai/HuggingFive) - Official [RISC-V spec](https:
-//github.com/riscv/riscv-isa-manual/releases/download/Ratified-IMAFDQC/riscv-
+| < 1k | ## References - [HuggingFive:raised_hand_with_fingers_splayed:](https:
+//github.com/OpenMachine-ai/HuggingFive) - Official [RISC-V spec](https://
+github.com/riscv/riscv-isa-manual/releases/download/Ratified-IMAFDQC/riscv-
 spec-20191213.pdf) - See [this RISC-V card](https://inst.eecs.berkeley.edu/
 ~cs61c/fa18/img/riscvcard.pdf) for a brief description of most instructions.
 See also the [RISC-V reference card](http://riscvbook.com/greencard-
 20181213.pdf). - Book [The RISC-V Reader: An Open Architecture Atlas](https://
 www.abebooks.com/book-search/author/patterson-david-waterman-andrew/) by David
 Patterson and Andrew Waterman. Appendix A of this book defines all
 instructions. The Spanish version of this book is [available for free](http://
```

### Comparing `tinyfive-0.0.15/pyproject.toml` & `tinyfive-1.0.0/pyproject.toml`

 * *Files 13% similar despite different names*

```diff
@@ -5,25 +5,26 @@
 
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "tinyfive"
-version = "0.0.15"
+# version numbering A.B.C: A is major version, B is minor version, and C is patch
+version = "1.0.0"
 authors = [
-  { name="Open Machine", email="tinyfive@openmachine.ai" },
+  {name="Open Machine", email="tinyfive@openmachine.ai"},
 ]
 description = "TinyFive is a lightweight RISC-V emulator and assembler written entirely in Python"
 readme = "README.md"
 requires-python = ">=3.6"
 classifiers = [
-    "Programming Language :: Python :: 3",
-    "License :: OSI Approved :: MIT License",
-    "Operating System :: OS Independent",
+  "Programming Language :: Python :: 3",
+  "License :: OSI Approved :: MIT License",
+  "Operating System :: OS Independent",
 ]
 dependencies = [
   "numpy>1.20.0",
 ]
 
 [project.urls]
 "Homepage" = "https://github.com/OpenMachine-ai/tinyfive"
```

### Comparing `tinyfive-0.0.15/PKG-INFO` & `tinyfive-1.0.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tinyfive
-Version: 0.0.15
+Version: 1.0.0
 Summary: TinyFive is a lightweight RISC-V emulator and assembler written entirely in Python
 Project-URL: Homepage, https://github.com/OpenMachine-ai/tinyfive
 Project-URL: Bug Tracker, https://github.com/OpenMachine-ai/tinyfive/issues
 Author-email: Open Machine <tinyfive@openmachine.ai>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -396,15 +396,14 @@
 # Output: True
 ```
 The table below shows a speedup of 1.7 with the following caveats:
 - The bit-widths don't make sense for fixed point (in general, multiplying two 32-bit integers produces a 64-bit product; and adding 4 of these products requires up to 66 bits).
 - For runtime calculations, we assume that our RISC-V CPU can only perform one instruction per cycle (while many RISC-V cores can perform multiple instructions per cycle).
 - We assume all 31 registers can be used, which is unrealistic because we ignore register allocation conventions such as the procedure
 calling conventions specified [here](https://github.com/riscv-non-isa/riscv-elf-psabi-doc).
-- For 16x16 or larger matrices, [Strassen's algorithm](https://en.wikipedia.org/wiki/Strassen_algorithm) and [DeepMind's AlphaTensor](https://www.deepmind.com/blog/discovering-novel-algorithms-with-alphatensor) can reduce the total number of multiplications and additions if they are applied recursively.
 
 |             | Image | Registers | Load | Store | Mul | Add | Branch | Total ops | Speedup |
 |:-----------:|:-----:|:---------:|:----:|:-----:|:---:|:---:|:------:|:---------:|:-------:|
 | Example 3.3 | 92B   | 9         | 80   | 16    | 64  | 89  | 20     | 269       | 1       |
 | Example 3.4 | 640B  | 22        | 32   | 16    | 64  | 48  | 0      | 160       | 1.7     |
 
 ### Example 4: Neural network layers
@@ -465,15 +464,15 @@
 - TinyFive is still under construction, many things haven't been implemented and tested yet.
 - 37 of the 40 base instructions (RV32I), all instructions of the M-extension (RV32M) and the F-extension (RV32F) with the default rounding mode are already implemented, and many of them are tested.  (The three missing RV32I instructions `fence`, `ebreak`, and `ecall` are not applicable here.)
 - Remaining work: improve testing, add more extensions. See TODOs in the code for more details.
 - Stay updated by following us on [Twitter](https://twitter.com/OpenMachine_AI), [Post.news](https://post.news/@/openmachine), and [LinkedIn](https://www.linkedin.com/in/nilsgraef/).
 
 ## Speed
 - TinyFive is not optimized for speed (but for ease-of-use and [LOC](https://en.wikipedia.org/wiki/Source_lines_of_code)).
-- You might be able to use [Codon](https://github.com/exaloop/codon) or PyPy to speed up TinyFive (see e.g. the [Pydgin paper](https://www.csl.cornell.edu/~berkin/ilbeyi-pydgin-riscv2016.pdf) for details).
+- You might be able to use PyPy or [Codon](https://github.com/exaloop/codon) to speed up TinyFive (see e.g. the [Pydgin paper](https://www.csl.cornell.edu/~berkin/ilbeyi-pydgin-riscv2016.pdf) for details).
 - If you only use the upper-case instructions such as `ADD()`, then TinyFive is very fast because there is no instruction decoding. And you should be able to accelerate it on a GPU or TPU.
 - If you use the lower-case instructions with `asm()` and `exe()`, then execution of these functions is slow as they involve look-up and string matching with O(n) complexity where "n" is the total number of instructions. The current implementations of `asm()` and `dec()` are optimized for ease-of-use and readability. A faster implementation would collapse multiple look-ups into one look-up, optimize the pattern-matching for the instruction decoding (bits -> instruction), and change the order of the instructions so that more frequently used instructions are at the top of the list. [Here is an older version](https://github.com/OpenMachine-ai/tinyfive/blob/2aa4987391561c9c6692602ed3fccdeaee333e0b/tinyfive.py) of TinyFive with a faster `dec()` function that collapses two look-ups (`bits -> instruction` and `instruction -> uppeer-case instruction`) and doesn't use `fnmatch`.
 
 ## Comparison
 The table below compares TinyFive with other [ISS](https://en.wikipedia.org/wiki/Instruction_set_simulator) and emulator projects.
 
 | ISS | Author | Language | Mature? | Extensions | LOC |
@@ -486,15 +485,15 @@
 | [riscvOVPsim](https://github.com/riscv-ovpsim/imperas-riscv-tests) | Imperas              | C         | Yes              | All           | |
 | [Whisper](https://github.com/chipsalliance/SweRV-ISS)              | Western Digital      | C, C++    | Yes | Almost all                 | |
 | [Sail Model](https://github.com/riscv/sail-riscv)                  | Cambridge, Edinburgh | Sail, C   | Yes | All                        | |
 | [PiMaker/rvc](https://github.com/PiMaker/rvc)                      | PiMaker              | C         |     |                            | |
 | [mini-rv32ima](https://github.com/cnlohr/mini-rv32ima)             | Charles Lohr         | C         |     | A, I, M, Zifencei, Zicsr   | < 1k |
 
 ## References
-- [HuggingFive :raised_hand_with_fingers_splayed:](https://github.com/OpenMachine-ai/HuggingFive)
+- [HuggingFive:raised_hand_with_fingers_splayed:](https://github.com/OpenMachine-ai/HuggingFive)
 - Official [RISC-V spec](https://github.com/riscv/riscv-isa-manual/releases/download/Ratified-IMAFDQC/riscv-spec-20191213.pdf)
 - See [this RISC-V card](https://inst.eecs.berkeley.edu/~cs61c/fa18/img/riscvcard.pdf) for a brief description of most instructions. See also the [RISC-V reference card](http://riscvbook.com/greencard-20181213.pdf).
 - Book [The RISC-V Reader: An Open Architecture Atlas](https://www.abebooks.com/book-search/author/patterson-david-waterman-andrew/) by David Patterson and Andrew Waterman. Appendix A of this book defines all instructions. The Spanish version of this book is [available for free](http://riscvbook.com/spanish/guia-practica-de-risc-v-1.0.5.pdf),
 other free versions are [available here](http://riscvbook.com).
 - Pydgin [paper](https://www.csl.cornell.edu/~berkin/ilbeyi-pydgin-riscv2016.pdf) and [video](https://youtu.be/-p_AGki7Vsk)
 - [Online simulator](https://ascslab.org/research/briscv/simulator/simulator.html) for debug
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: tinyfive Version: 0.0.15 Summary: TinyFive is a
+Metadata-Version: 2.1 Name: tinyfive Version: 1.0.0 Summary: TinyFive is a
 lightweight RISC-V emulator and assembler written entirely in Python Project-
 URL: Homepage, https://github.com/OpenMachine-ai/tinyfive Project-URL: Bug
 Tracker, https://github.com/OpenMachine-ai/tinyfive/issues Author-email: Open
 Machine
 openmachine.ai> License-File: LICENSE Classifier: License :: OSI Approved ::
 MIT License Classifier: Operating System :: OS Independent Classifier:
 Programming Language :: Python :: 3 Requires-Python: >=3.6 Requires-Dist:
@@ -244,19 +244,15 @@
 caveats: - The bit-widths don't make sense for fixed point (in general,
 multiplying two 32-bit integers produces a 64-bit product; and adding 4 of
 these products requires up to 66 bits). - For runtime calculations, we assume
 that our RISC-V CPU can only perform one instruction per cycle (while many
 RISC-V cores can perform multiple instructions per cycle). - We assume all 31
 registers can be used, which is unrealistic because we ignore register
 allocation conventions such as the procedure calling conventions specified
-[here](https://github.com/riscv-non-isa/riscv-elf-psabi-doc). - For 16x16 or
-larger matrices, [Strassen's algorithm](https://en.wikipedia.org/wiki/
-Strassen_algorithm) and [DeepMind's AlphaTensor](https://www.deepmind.com/blog/
-discovering-novel-algorithms-with-alphatensor) can reduce the total number of
-multiplications and additions if they are applied recursively. | | Image |
+[here](https://github.com/riscv-non-isa/riscv-elf-psabi-doc). | | Image |
 Registers | Load | Store | Mul | Add | Branch | Total ops | Speedup | |:-------
 ----:|:-----:|:---------:|:----:|:-----:|:---:|:---:|:------:|:---------:|:----
 ---:| | Example 3.3 | 92B | 9 | 80 | 16 | 64 | 89 | 20 | 269 | 1 | | Example
 3.4 | 640B | 22 | 32 | 16 | 64 | 48 | 0 | 160 | 1.7 | ### Example 4: Neural
 network layers Coming soon, see [file layer_examples.py](layer_examples.py) for
 now ### Example 5: MobileNet Coming soon-ish, see [file mobilenet_v1_0.25.py]
 (mobilenet_v1_0.25.py) for now ## Running in colab [Colab] This is the quickest
@@ -289,19 +285,19 @@
 are already implemented, and many of them are tested. (The three missing RV32I
 instructions `fence`, `ebreak`, and `ecall` are not applicable here.) -
 Remaining work: improve testing, add more extensions. See TODOs in the code for
 more details. - Stay updated by following us on [Twitter](https://twitter.com/
 OpenMachine_AI), [Post.news](https://post.news/@/openmachine), and [LinkedIn]
 (https://www.linkedin.com/in/nilsgraef/). ## Speed - TinyFive is not optimized
 for speed (but for ease-of-use and [LOC](https://en.wikipedia.org/wiki/
-Source_lines_of_code)). - You might be able to use [Codon](https://github.com/
-exaloop/codon) or PyPy to speed up TinyFive (see e.g. the [Pydgin paper](https:
-//www.csl.cornell.edu/~berkin/ilbeyi-pydgin-riscv2016.pdf) for details). - If
-you only use the upper-case instructions such as `ADD()`, then TinyFive is very
-fast because there is no instruction decoding. And you should be able to
+Source_lines_of_code)). - You might be able to use PyPy or [Codon](https://
+github.com/exaloop/codon) to speed up TinyFive (see e.g. the [Pydgin paper]
+(https://www.csl.cornell.edu/~berkin/ilbeyi-pydgin-riscv2016.pdf) for details).
+- If you only use the upper-case instructions such as `ADD()`, then TinyFive is
+very fast because there is no instruction decoding. And you should be able to
 accelerate it on a GPU or TPU. - If you use the lower-case instructions with
 `asm()` and `exe()`, then execution of these functions is slow as they involve
 look-up and string matching with O(n) complexity where "n" is the total number
 of instructions. The current implementations of `asm()` and `dec()` are
 optimized for ease-of-use and readability. A faster implementation would
 collapse multiple look-ups into one look-up, optimize the pattern-matching for
 the instruction decoding (bits -> instruction), and change the order of the
@@ -323,17 +319,17 @@
 /en.wikipedia.org/wiki/Fabrice_Bellard) | C | Yes | All | | | [riscvOVPsim]
 (https://github.com/riscv-ovpsim/imperas-riscv-tests) | Imperas | C | Yes | All
 | | | [Whisper](https://github.com/chipsalliance/SweRV-ISS) | Western Digital |
 C, C++ | Yes | Almost all | | | [Sail Model](https://github.com/riscv/sail-
 riscv) | Cambridge, Edinburgh | Sail, C | Yes | All | | | [PiMaker/rvc](https:/
 /github.com/PiMaker/rvc) | PiMaker | C | | | | | [mini-rv32ima](https://
 github.com/cnlohr/mini-rv32ima) | Charles Lohr | C | | A, I, M, Zifencei, Zicsr
-| < 1k | ## References - [HuggingFive :raised_hand_with_fingers_splayed:]
-(https://github.com/OpenMachine-ai/HuggingFive) - Official [RISC-V spec](https:
-//github.com/riscv/riscv-isa-manual/releases/download/Ratified-IMAFDQC/riscv-
+| < 1k | ## References - [HuggingFive:raised_hand_with_fingers_splayed:](https:
+//github.com/OpenMachine-ai/HuggingFive) - Official [RISC-V spec](https://
+github.com/riscv/riscv-isa-manual/releases/download/Ratified-IMAFDQC/riscv-
 spec-20191213.pdf) - See [this RISC-V card](https://inst.eecs.berkeley.edu/
 ~cs61c/fa18/img/riscvcard.pdf) for a brief description of most instructions.
 See also the [RISC-V reference card](http://riscvbook.com/greencard-
 20181213.pdf). - Book [The RISC-V Reader: An Open Architecture Atlas](https://
 www.abebooks.com/book-search/author/patterson-david-waterman-andrew/) by David
 Patterson and Andrew Waterman. Appendix A of this book defines all
 instructions. The Spanish version of this book is [available for free](http://
```

