# Comparing `tmp/ebcdic_parser-3.0.0.tar.gz` & `tmp/ebcdic_parser-3.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "D:\Projects\ebcdic-parser\dist\.tmp-p3xg8nvn\ebcdic_parser-3.0.0.tar", last modified: Mon Jul 24 03:59:16 2023, max compression
+gzip compressed data, was "D:\Projects\ebcdic-parser\dist\.tmp-oqnuh1lu\ebcdic_parser-3.1.0.tar", last modified: Sun Jul 30 14:50:51 2023, max compression
```

## Comparing `ebcdic_parser-3.0.0.tar` & `ebcdic_parser-3.1.0.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxrwxrwx   0        0        0        0 2023-07-24 03:59:16.000000 ebcdic_parser-3.0.0/
--rw-rw-rw-   0        0        0       16 2020-07-12 02:48:58.000000 ebcdic_parser-3.0.0/AUTHORS
--rw-rw-rw-   0        0        0     1066 2020-07-12 02:48:58.000000 ebcdic_parser-3.0.0/LICENSE
--rw-rw-rw-   0        0        0     9481 2023-07-24 03:59:16.000000 ebcdic_parser-3.0.0/PKG-INFO
--rw-rw-rw-   0        0        0     8602 2022-11-11 04:16:50.000000 ebcdic_parser-3.0.0/README.md
--rw-rw-rw-   0        0        0       86 2023-07-18 03:12:01.000000 ebcdic_parser-3.0.0/pyproject.toml
--rw-rw-rw-   0        0        0      783 2023-07-24 03:59:16.000000 ebcdic_parser-3.0.0/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-07-24 03:59:16.000000 ebcdic_parser-3.0.0/src/
-drwxrwxrwx   0        0        0        0 2023-07-24 03:59:16.000000 ebcdic_parser-3.0.0/src/ebcdic_parser/
--rw-rw-rw-   0        0        0        0 2023-07-18 02:52:18.000000 ebcdic_parser-3.0.0/src/ebcdic_parser/__init__.py
--rw-rw-rw-   0        0        0    58886 2023-07-22 14:12:41.000000 ebcdic_parser-3.0.0/src/ebcdic_parser/convert.py
-drwxrwxrwx   0        0        0        0 2023-07-24 03:59:16.000000 ebcdic_parser-3.0.0/src/ebcdic_parser.egg-info/
--rw-rw-rw-   0        0        0     9481 2023-07-24 03:59:16.000000 ebcdic_parser-3.0.0/src/ebcdic_parser.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      390 2023-07-24 03:59:16.000000 ebcdic_parser-3.0.0/src/ebcdic_parser.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-24 03:59:16.000000 ebcdic_parser-3.0.0/src/ebcdic_parser.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       14 2023-07-24 03:59:16.000000 ebcdic_parser-3.0.0/src/ebcdic_parser.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-07-24 03:59:16.000000 ebcdic_parser-3.0.0/tests/
--rw-rw-rw-   0        0        0    17737 2020-07-12 02:48:58.000000 ebcdic_parser-3.0.0/tests/test_functional.py
--rw-rw-rw-   0        0        0     6168 2020-07-12 02:48:58.000000 ebcdic_parser-3.0.0/tests/test_system_311_calls_for_service_requests_all_strings.py
--rw-rw-rw-   0        0        0     5949 2020-07-12 02:48:58.000000 ebcdic_parser-3.0.0/tests/test_system_common.py
+drwxrwxrwx   0        0        0        0 2023-07-30 14:50:51.000000 ebcdic_parser-3.1.0/
+-rw-rw-rw-   0        0        0       16 2020-07-12 02:48:58.000000 ebcdic_parser-3.1.0/AUTHORS
+-rw-rw-rw-   0        0        0     1066 2020-07-12 02:48:58.000000 ebcdic_parser-3.1.0/LICENSE
+-rw-rw-rw-   0        0        0    11978 2023-07-30 14:50:51.000000 ebcdic_parser-3.1.0/PKG-INFO
+-rw-rw-rw-   0        0        0    11042 2023-07-30 14:47:33.000000 ebcdic_parser-3.1.0/README.md
+-rw-rw-rw-   0        0        0       86 2023-07-18 03:12:01.000000 ebcdic_parser-3.1.0/pyproject.toml
+-rw-rw-rw-   0        0        0      783 2023-07-30 14:50:51.000000 ebcdic_parser-3.1.0/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-07-30 14:50:51.000000 ebcdic_parser-3.1.0/src/
+drwxrwxrwx   0        0        0        0 2023-07-30 14:50:51.000000 ebcdic_parser-3.1.0/src/ebcdic_parser/
+-rw-rw-rw-   0        0        0        0 2023-07-18 02:52:18.000000 ebcdic_parser-3.1.0/src/ebcdic_parser/__init__.py
+-rw-rw-rw-   0        0        0    59241 2023-07-30 14:36:53.000000 ebcdic_parser-3.1.0/src/ebcdic_parser/convert.py
+drwxrwxrwx   0        0        0        0 2023-07-30 14:50:51.000000 ebcdic_parser-3.1.0/src/ebcdic_parser.egg-info/
+-rw-rw-rw-   0        0        0    11978 2023-07-30 14:50:51.000000 ebcdic_parser-3.1.0/src/ebcdic_parser.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      390 2023-07-30 14:50:51.000000 ebcdic_parser-3.1.0/src/ebcdic_parser.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-30 14:50:51.000000 ebcdic_parser-3.1.0/src/ebcdic_parser.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       14 2023-07-30 14:50:51.000000 ebcdic_parser-3.1.0/src/ebcdic_parser.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-30 14:50:51.000000 ebcdic_parser-3.1.0/tests/
+-rw-rw-rw-   0        0        0    17737 2020-07-12 02:48:58.000000 ebcdic_parser-3.1.0/tests/test_functional.py
+-rw-rw-rw-   0        0        0     6168 2020-07-12 02:48:58.000000 ebcdic_parser-3.1.0/tests/test_system_311_calls_for_service_requests_all_strings.py
+-rw-rw-rw-   0        0        0     5949 2020-07-12 02:48:58.000000 ebcdic_parser-3.1.0/tests/test_system_common.py
```

### Comparing `ebcdic_parser-3.0.0/LICENSE` & `ebcdic_parser-3.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `ebcdic_parser-3.0.0/PKG-INFO` & `ebcdic_parser-3.1.0/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ebcdic_parser
-Version: 3.0.0
+Version: 3.1.0
 Summary: Convert mainframe EBCDIC data into Unicode ASCII delimited text files
 Home-page: https://github.com/larandvit/ebcdic-parser
 Author: Vitaly Saversky
 Author-email: larandvit@hotmail.com
 Project-URL: Bug Tracker, https://github.com/larandvit/ebcdic-parser/issues
 Project-URL: repository, https://github.com/larandvit/ebcdic-parser
 Classifier: Programming Language :: Python :: 3
@@ -26,20 +26,20 @@
  
 Conversion rules are a driver to parse EBCDIC data.
 
 ## Features
 
 * Supported layouts
     1. Single schema
-       * Original [COBOL layout](test_data/pr_p1_p2_gas_disposition/oga0861.pdf) and corresponding [conversion rules](layout_repository/gsf102_rules.json) file
+       * Original [COBOL layout](tests/test_data/pr_p1_p2_gas_disposition/oga0861.pdf) and corresponding [conversion rules](tests/layout_repository/gsf102_rules.json) file
     2. Multi-schema fixed record length
-       * Original [COBOL layout](test_data/ola013k/ola013k.pdf) and corresponding [conversion rules](layout_repository/ola013k_rules.json) file
+       * Original [COBOL layout](tests/test_data/ola013k/ola013k.pdf) and corresponding [conversion rules](tests/layout_repository/ola013k_rules.json) file
     3. Multi-schema variable record length
     4. Single schema variable record length
-       * Original [COBOL layout](test_data/service_segment_data/129.1DP.pdf) and corresponding [conversion rules](layout_repository/service_segment_data.json) file
+       * Original [COBOL layout](tests/test_data/service_segment_data/129.1DP.pdf) and corresponding [conversion rules](tests/layout_repository/service_segment_data.json) file
  
 * Fixing anomalies in EBCDIC files
     1. Skip header
     2. Skip footer
     3. Remove invalid characters
   
 * Adding relationship keys
@@ -48,14 +48,16 @@
      
 * Applicable encodings
     1. Python
     2. Java
     
 * Debug mode to troubleshoot layouts
 
+* Pip package or command prompt usage
+
 ## Conversion rules sample
 Detailed information about conversion rules setup file can be found in [Engine Rules](https://github.com/larandvit/ebcdic-parser/blob/master/docs/engine_rules_manual.md) manual. [COBOL Engine Rules Dictionary](https://github.com/larandvit/ebcdic-parser/blob/master/docs/cobol_engine_rules_dictionary.md) manual describes how to convert COBOL data types into engine rules layout.
 ```json
 {
     "description": "conversion rules sample",
     "header": [
         {
@@ -82,33 +84,84 @@
                 }
             ]
         }
     ]
 }
 ```
 
-## Installation
-It doesn't request any special installation if you are planning to use only Python encodings.
+## Pip Usage
 
-In case of using Java encodings, it has to be installed [javabridge](https://pypi.org/project/javabridge/) Python library. There is a constant in the code for including the javabridge library.
+### Installation
+
+```bash
+pip install ebcdic_parser
+```
+
+### Sample
+
+```python
+from ebcdic_parser.convert import run 
+
+
+run("../tests/test_data/311_calls_for_service_requests_all_strings/311_calls_for_service_requests_sample.dat", 
+    "../tests/test_data/311_calls_for_service_requests_all_strings/output",
+    "../tests/layout_repository/311_calls_for_service_requests_all_strings.json",
+    outputDelimiter=',')
+```
 
-## Usage
+### Run Function
+
+```
+run(inputFile, 
+    outputFolder,
+    layoutFile,
+    logfolder='',
+    pythonEncoding=True,
+    encodingName='cp037',
+    outputDelimiter=`\t`,
+    outputFileExtension=`.txt`,
+    ignoreConversionErrors=False,
+    groupRecords=False,
+    groupRecordsLevel2=False,
+    verbose=True,
+    debug=False,
+    cliMode=False):
 ```
-usage: ebcdic_parser.py [-h] --inputfile "input file path" --outputfolder
+
+
+* **inputfile** - input EBCDIC file path. Mandatory parameter. Absolute and relative paths are acceptable.
+* **outputfolder** - output folder to store delimited files. Mandatory parameter. Absolute and relative paths are acceptable.
+* **layoutfile** - layout file path. Mandatory parameter. Absolute and relative paths are acceptable.
+* **outputdelimiter** - output text file delimiter. Optional parameter. Default value is `\t`.
+* **outputfileextension** - output text file extension. Optional parameter. Default value is `.txt`.
+* **ignoreconversionerrors** - ignore any conversion error. Optional parameter. Default value is `False`.
+* **logfolder** - output folder to store log file. Optional parameter. Default value is the current folder. Absolute and relative paths are acceptable.
+* **pythonencoding** - use Python encoding rather than Java. Optional parameter. Default value is `True`.
+* **encodingname** - code page name to encode characters (Python or Java). Optional parameter. Default value is `cp037`.
+* **grouprecords** - create relationships between records. Optional parameter. Default value is `False'.
+* **grouprecordslevel2** - create relationships between records for level 2. Optional parameter. Default value is `False`.
+* **verbose** - show extended information on screen. Optional parameter. Default value is `True`.
+* **debug** - show debug information. Optional parameter. Default value is `False`.
+* **cliMode** - a flag how it run in command prompt or Pip installation.  
+
+
+## Command Prompt Usage
+```
+usage: convert.py [-h] --inputfile "input file path" --outputfolder
                         "output folder" --layoutfile "layout file"
                         [--outputdelimiter [delimiter]]
                         [--outputfileextension [extension]]
                         [--ignoreconversionerrors [yes/no]]
                         [--logfolder [log folder]] [--pythonencoding [yes/no]]
                         [--encodingname [encoding name]]
                         [--grouprecords [yes/no]]
                         [--grouprecordslevel2 [yes/no]] [--verbose [yes/no]]
                         [--debug [yes/no]]
 
-Convert EBCDIC data into delimited text format. Version 2.3.0
+Convert EBCDIC data into delimited text format. Version x.x.x
 
 Supported file formats:
 (1) Single schema
 (2) Multi-schema fixed length
 (3) Multi-schema variable length
 (4) Single schema variable length
 
@@ -143,64 +196,63 @@
                         create relationships between records for level 2
   --verbose [yes/no]    show information on screen
   --debug [yes/no]      show debug information
 
 Exit codes: 0 - successful completion, 1 - completion with any error
 ```
 
-## Samples
 ### Single schema #1
 
 ```bash
-ebcdic_parser.py --inputfile "./test_data/311_calls_for_service_requests_all_strings/311_calls_for_service_requests_sample.dat" --outputfolder "./test_data/311_calls_for_service_requests_all_strings/output" --layoutfile "./layout_repository/311_calls_for_service_requests_all_strings.json" --outputdelimiter ,
+convert.py --inputfile "../../tests/test_data/311_calls_for_service_requests_all_strings/311_calls_for_service_requests_sample.dat" --outputfolder "../../tests/test_data/311_calls_for_service_requests_all_strings/output" --layoutfile "../../tests/layout_repository/311_calls_for_service_requests_all_strings.json" --outputdelimiter ,
 ```
 
-* Output location: ./test_data/311_calls_for_service_requests_all_strings/output
+* Output location: ./tests/test_data/311_calls_for_service_requests_all_strings/output
 * Outptut format: comma delimited ASCII file
 * Log file: ./ebcdic_parser.log
 
 ### Single schema in debug mode #1
 
 ```bash
-ebcdic_parser.py --inputfile "./test_data/311_calls_for_service_requests_all_strings/311_calls_for_service_requests_sample.dat" --outputfolder "./test_data/311_calls_for_service_requests_all_strings/output" --layoutfile "./layout_repository/311_calls_for_service_requests_all_strings.json" --outputdelimiter , --debug yes
+convert.py --inputfile "../../tests/test_data/311_calls_for_service_requests_all_strings/311_calls_for_service_requests_sample.dat" --outputfolder "../../tests/test_data/311_calls_for_service_requests_all_strings/output" --layoutfile "../../tests/layout_repository/311_calls_for_service_requests_all_strings.json" --outputdelimiter , --debug yes
 ```
 
-* Output location: ./test_data/311_calls_for_service_requests_all_strings/output
+* Output location: ./tests/tests/test_data/311_calls_for_service_requests_all_strings/output
 * Outptut format: comma delimited ASCII file
 * Log file: ./ebcdic_parser.log
 
 ### Single schema #2
 
 ```bash
-ebcdic_parser.py --inputfile "./test_data/pr_p1_p2_gas_disposition/gsf102.ebc" --outputfolder "./test_data/pr_p1_p2_gas_disposition/output" --layoutfile "./layout_repository/gsf102_rules.json" --logfolder "./test_data/pr_p1_p2_gas_disposition/log"
+convert.py --inputfile "../../tests/test_data/pr_p1_p2_gas_disposition/gsf102.ebc" --outputfolder "../../tests/test_data/pr_p1_p2_gas_disposition/output" --layoutfile "../../tests/layout_repository/gsf102_rules.json" --logfolder "../../tests/test_data/pr_p1_p2_gas_disposition/log"
 ```
 
-* Output location: ./test_data/pr_p1_p2_gas_disposition/output
+* Output location: ./tests/test_data/pr_p1_p2_gas_disposition/output
 * Outptut format: tab delimited ASCII file
-* Log folder: ./test_data/pr_p1_p2_gas_disposition/log
+* Log folder: ./tests/test_data/pr_p1_p2_gas_disposition/log/ebcdic_parser.log
 
 ### Multi-schema fixed record length
 
 ```bash
-ebcdic_parser.py --inputfile "./test_data/ola013k/olf001l.ebc" --outputfolder "./test_data/ola013k/output" --layoutfile "./layout_repository/ola013k_rules.json" --logfolder "./test_data/ola013k/log"
+convert.py --inputfile "../../tests/test_data/ola013k/olf001l.ebc" --outputfolder "../../tests/test_data/ola013k/output" --layoutfile "../../tests/layout_repository/ola013k_rules.json"
 ```
 
-* Output location: ./test_data/ola013k/output
+* Output location: ./tests/test_data/ola013k/output
 * Outptut format: tab delimited ASCII file
-* Log folder: ./test_data/ola013k/log
+* Log folder: ./ebcdic_parser.log
 
 ### Single schema variable record length
 
 ```bash
-ebcdic_parser.py --inputfile "./test_data/service_segment_data/RG197.SERVSEG.Y70.ebc" --outputfolder "./test_data/service_segment_data/output" --layoutfile "./layout_repository/service_segment_data.json" --logfolder "./test_data/service_segment_data/log"
+convert.py --inputfile "../../tests/test_data/service_segment_data/RG197.SERVSEG.Y70.ebc" --outputfolder "../../tests/test_data/service_segment_data/output" --layoutfile "../../tests/layout_repository/service_segment_data.json"
 ```
 
-* Output location: ./test_data/service_segment_data/output
+* Output location: ./tests/test_data/service_segment_data/output
 * Outptut format: tab delimited ASCII file
-* Log folder: ./test_data/service_segment_data/log
+* Log folder: ./ebcdic_parser.log
 
 ## Testing
 ### Functional tests
 
 Those tests cover testing of each data type. 
 ```
 test_functional.py
@@ -212,14 +264,19 @@
 converter_to_ebcdic.py
 ```
 * Run tests
 ```
 test_system_311_calls_for_service_requests_all_strings.py
 ```
 
+## Java Encodings
+It doesn't request any special installation if you are planning to use only Python encodings.
+
+In case of using Java encodings, it has to be installed [javabridge](https://pypi.org/project/javabridge/) Python library. There is a constant in the code for including the javabridge library.
+
 ## Contributing
 Please read [CONTRIBUTING.md](https://github.com/larandvit/ebcdic-parser/blob/master/CONTRIBUTING.md) for details on our code of conduct, and the process for submitting pull requests to us.
  
 ## License
 This project is licensed under the MIT License - see the [LICENSE](https://github.com/larandvit/ebcdic-parser/blob/master/LICENSE) file for details
 
 ## Acknowledgments
```

### Comparing `ebcdic_parser-3.0.0/README.md` & `ebcdic_parser-3.1.0/README.md`

 * *Files 19% similar despite different names*

```diff
@@ -9,20 +9,20 @@
  
 Conversion rules are a driver to parse EBCDIC data.
 
 ## Features
 
 * Supported layouts
     1. Single schema
-       * Original [COBOL layout](test_data/pr_p1_p2_gas_disposition/oga0861.pdf) and corresponding [conversion rules](layout_repository/gsf102_rules.json) file
+       * Original [COBOL layout](tests/test_data/pr_p1_p2_gas_disposition/oga0861.pdf) and corresponding [conversion rules](tests/layout_repository/gsf102_rules.json) file
     2. Multi-schema fixed record length
-       * Original [COBOL layout](test_data/ola013k/ola013k.pdf) and corresponding [conversion rules](layout_repository/ola013k_rules.json) file
+       * Original [COBOL layout](tests/test_data/ola013k/ola013k.pdf) and corresponding [conversion rules](tests/layout_repository/ola013k_rules.json) file
     3. Multi-schema variable record length
     4. Single schema variable record length
-       * Original [COBOL layout](test_data/service_segment_data/129.1DP.pdf) and corresponding [conversion rules](layout_repository/service_segment_data.json) file
+       * Original [COBOL layout](tests/test_data/service_segment_data/129.1DP.pdf) and corresponding [conversion rules](tests/layout_repository/service_segment_data.json) file
  
 * Fixing anomalies in EBCDIC files
     1. Skip header
     2. Skip footer
     3. Remove invalid characters
   
 * Adding relationship keys
@@ -31,14 +31,16 @@
      
 * Applicable encodings
     1. Python
     2. Java
     
 * Debug mode to troubleshoot layouts
 
+* Pip package or command prompt usage
+
 ## Conversion rules sample
 Detailed information about conversion rules setup file can be found in [Engine Rules](https://github.com/larandvit/ebcdic-parser/blob/master/docs/engine_rules_manual.md) manual. [COBOL Engine Rules Dictionary](https://github.com/larandvit/ebcdic-parser/blob/master/docs/cobol_engine_rules_dictionary.md) manual describes how to convert COBOL data types into engine rules layout.
 ```json
 {
     "description": "conversion rules sample",
     "header": [
         {
@@ -65,33 +67,84 @@
                 }
             ]
         }
     ]
 }
 ```
 
-## Installation
-It doesn't request any special installation if you are planning to use only Python encodings.
+## Pip Usage
 
-In case of using Java encodings, it has to be installed [javabridge](https://pypi.org/project/javabridge/) Python library. There is a constant in the code for including the javabridge library.
+### Installation
+
+```bash
+pip install ebcdic_parser
+```
+
+### Sample
+
+```python
+from ebcdic_parser.convert import run 
+
+
+run("../tests/test_data/311_calls_for_service_requests_all_strings/311_calls_for_service_requests_sample.dat", 
+    "../tests/test_data/311_calls_for_service_requests_all_strings/output",
+    "../tests/layout_repository/311_calls_for_service_requests_all_strings.json",
+    outputDelimiter=',')
+```
 
-## Usage
+### Run Function
+
+```
+run(inputFile, 
+    outputFolder,
+    layoutFile,
+    logfolder='',
+    pythonEncoding=True,
+    encodingName='cp037',
+    outputDelimiter=`\t`,
+    outputFileExtension=`.txt`,
+    ignoreConversionErrors=False,
+    groupRecords=False,
+    groupRecordsLevel2=False,
+    verbose=True,
+    debug=False,
+    cliMode=False):
 ```
-usage: ebcdic_parser.py [-h] --inputfile "input file path" --outputfolder
+
+
+* **inputfile** - input EBCDIC file path. Mandatory parameter. Absolute and relative paths are acceptable.
+* **outputfolder** - output folder to store delimited files. Mandatory parameter. Absolute and relative paths are acceptable.
+* **layoutfile** - layout file path. Mandatory parameter. Absolute and relative paths are acceptable.
+* **outputdelimiter** - output text file delimiter. Optional parameter. Default value is `\t`.
+* **outputfileextension** - output text file extension. Optional parameter. Default value is `.txt`.
+* **ignoreconversionerrors** - ignore any conversion error. Optional parameter. Default value is `False`.
+* **logfolder** - output folder to store log file. Optional parameter. Default value is the current folder. Absolute and relative paths are acceptable.
+* **pythonencoding** - use Python encoding rather than Java. Optional parameter. Default value is `True`.
+* **encodingname** - code page name to encode characters (Python or Java). Optional parameter. Default value is `cp037`.
+* **grouprecords** - create relationships between records. Optional parameter. Default value is `False'.
+* **grouprecordslevel2** - create relationships between records for level 2. Optional parameter. Default value is `False`.
+* **verbose** - show extended information on screen. Optional parameter. Default value is `True`.
+* **debug** - show debug information. Optional parameter. Default value is `False`.
+* **cliMode** - a flag how it run in command prompt or Pip installation.  
+
+
+## Command Prompt Usage
+```
+usage: convert.py [-h] --inputfile "input file path" --outputfolder
                         "output folder" --layoutfile "layout file"
                         [--outputdelimiter [delimiter]]
                         [--outputfileextension [extension]]
                         [--ignoreconversionerrors [yes/no]]
                         [--logfolder [log folder]] [--pythonencoding [yes/no]]
                         [--encodingname [encoding name]]
                         [--grouprecords [yes/no]]
                         [--grouprecordslevel2 [yes/no]] [--verbose [yes/no]]
                         [--debug [yes/no]]
 
-Convert EBCDIC data into delimited text format. Version 2.3.0
+Convert EBCDIC data into delimited text format. Version x.x.x
 
 Supported file formats:
 (1) Single schema
 (2) Multi-schema fixed length
 (3) Multi-schema variable length
 (4) Single schema variable length
 
@@ -126,64 +179,63 @@
                         create relationships between records for level 2
   --verbose [yes/no]    show information on screen
   --debug [yes/no]      show debug information
 
 Exit codes: 0 - successful completion, 1 - completion with any error
 ```
 
-## Samples
 ### Single schema #1
 
 ```bash
-ebcdic_parser.py --inputfile "./test_data/311_calls_for_service_requests_all_strings/311_calls_for_service_requests_sample.dat" --outputfolder "./test_data/311_calls_for_service_requests_all_strings/output" --layoutfile "./layout_repository/311_calls_for_service_requests_all_strings.json" --outputdelimiter ,
+convert.py --inputfile "../../tests/test_data/311_calls_for_service_requests_all_strings/311_calls_for_service_requests_sample.dat" --outputfolder "../../tests/test_data/311_calls_for_service_requests_all_strings/output" --layoutfile "../../tests/layout_repository/311_calls_for_service_requests_all_strings.json" --outputdelimiter ,
 ```
 
-* Output location: ./test_data/311_calls_for_service_requests_all_strings/output
+* Output location: ./tests/test_data/311_calls_for_service_requests_all_strings/output
 * Outptut format: comma delimited ASCII file
 * Log file: ./ebcdic_parser.log
 
 ### Single schema in debug mode #1
 
 ```bash
-ebcdic_parser.py --inputfile "./test_data/311_calls_for_service_requests_all_strings/311_calls_for_service_requests_sample.dat" --outputfolder "./test_data/311_calls_for_service_requests_all_strings/output" --layoutfile "./layout_repository/311_calls_for_service_requests_all_strings.json" --outputdelimiter , --debug yes
+convert.py --inputfile "../../tests/test_data/311_calls_for_service_requests_all_strings/311_calls_for_service_requests_sample.dat" --outputfolder "../../tests/test_data/311_calls_for_service_requests_all_strings/output" --layoutfile "../../tests/layout_repository/311_calls_for_service_requests_all_strings.json" --outputdelimiter , --debug yes
 ```
 
-* Output location: ./test_data/311_calls_for_service_requests_all_strings/output
+* Output location: ./tests/tests/test_data/311_calls_for_service_requests_all_strings/output
 * Outptut format: comma delimited ASCII file
 * Log file: ./ebcdic_parser.log
 
 ### Single schema #2
 
 ```bash
-ebcdic_parser.py --inputfile "./test_data/pr_p1_p2_gas_disposition/gsf102.ebc" --outputfolder "./test_data/pr_p1_p2_gas_disposition/output" --layoutfile "./layout_repository/gsf102_rules.json" --logfolder "./test_data/pr_p1_p2_gas_disposition/log"
+convert.py --inputfile "../../tests/test_data/pr_p1_p2_gas_disposition/gsf102.ebc" --outputfolder "../../tests/test_data/pr_p1_p2_gas_disposition/output" --layoutfile "../../tests/layout_repository/gsf102_rules.json" --logfolder "../../tests/test_data/pr_p1_p2_gas_disposition/log"
 ```
 
-* Output location: ./test_data/pr_p1_p2_gas_disposition/output
+* Output location: ./tests/test_data/pr_p1_p2_gas_disposition/output
 * Outptut format: tab delimited ASCII file
-* Log folder: ./test_data/pr_p1_p2_gas_disposition/log
+* Log folder: ./tests/test_data/pr_p1_p2_gas_disposition/log/ebcdic_parser.log
 
 ### Multi-schema fixed record length
 
 ```bash
-ebcdic_parser.py --inputfile "./test_data/ola013k/olf001l.ebc" --outputfolder "./test_data/ola013k/output" --layoutfile "./layout_repository/ola013k_rules.json" --logfolder "./test_data/ola013k/log"
+convert.py --inputfile "../../tests/test_data/ola013k/olf001l.ebc" --outputfolder "../../tests/test_data/ola013k/output" --layoutfile "../../tests/layout_repository/ola013k_rules.json"
 ```
 
-* Output location: ./test_data/ola013k/output
+* Output location: ./tests/test_data/ola013k/output
 * Outptut format: tab delimited ASCII file
-* Log folder: ./test_data/ola013k/log
+* Log folder: ./ebcdic_parser.log
 
 ### Single schema variable record length
 
 ```bash
-ebcdic_parser.py --inputfile "./test_data/service_segment_data/RG197.SERVSEG.Y70.ebc" --outputfolder "./test_data/service_segment_data/output" --layoutfile "./layout_repository/service_segment_data.json" --logfolder "./test_data/service_segment_data/log"
+convert.py --inputfile "../../tests/test_data/service_segment_data/RG197.SERVSEG.Y70.ebc" --outputfolder "../../tests/test_data/service_segment_data/output" --layoutfile "../../tests/layout_repository/service_segment_data.json"
 ```
 
-* Output location: ./test_data/service_segment_data/output
+* Output location: ./tests/test_data/service_segment_data/output
 * Outptut format: tab delimited ASCII file
-* Log folder: ./test_data/service_segment_data/log
+* Log folder: ./ebcdic_parser.log
 
 ## Testing
 ### Functional tests
 
 Those tests cover testing of each data type. 
 ```
 test_functional.py
@@ -195,14 +247,19 @@
 converter_to_ebcdic.py
 ```
 * Run tests
 ```
 test_system_311_calls_for_service_requests_all_strings.py
 ```
 
+## Java Encodings
+It doesn't request any special installation if you are planning to use only Python encodings.
+
+In case of using Java encodings, it has to be installed [javabridge](https://pypi.org/project/javabridge/) Python library. There is a constant in the code for including the javabridge library.
+
 ## Contributing
 Please read [CONTRIBUTING.md](https://github.com/larandvit/ebcdic-parser/blob/master/CONTRIBUTING.md) for details on our code of conduct, and the process for submitting pull requests to us.
  
 ## License
 This project is licensed under the MIT License - see the [LICENSE](https://github.com/larandvit/ebcdic-parser/blob/master/LICENSE) file for details
 
 ## Acknowledgments
```

### Comparing `ebcdic_parser-3.0.0/setup.cfg` & `ebcdic_parser-3.1.0/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
 00000010: 203d 2065 6263 6469 635f 7061 7273 6572   = ebcdic_parser
-00000020: 0d0a 7665 7273 696f 6e20 3d20 332e 302e  ..version = 3.0.
+00000020: 0d0a 7665 7273 696f 6e20 3d20 332e 312e  ..version = 3.1.
 00000030: 300d 0a61 7574 686f 7220 3d20 5669 7461  0..author = Vita
 00000040: 6c79 2053 6176 6572 736b 790d 0a61 7574  ly Saversky..aut
 00000050: 686f 725f 656d 6169 6c20 3d20 6c61 7261  hor_email = lara
 00000060: 6e64 7669 7440 686f 746d 6169 6c2e 636f  ndvit@hotmail.co
 00000070: 6d0d 0a64 6573 6372 6970 7469 6f6e 203d  m..description =
 00000080: 2043 6f6e 7665 7274 206d 6169 6e66 7261   Convert mainfra
 00000090: 6d65 2045 4243 4449 4320 6461 7461 2069  me EBCDIC data i
```

### Comparing `ebcdic_parser-3.0.0/src/ebcdic_parser/convert.py` & `ebcdic_parser-3.1.0/src/ebcdic_parser/convert.py`

 * *Files 2% similar despite different names*

```diff
@@ -34,15 +34,15 @@
 import re
 
 import unicodedata
 
 __author__ = "Vitaly Saversky"
 __date__ = "2017-10-04"
 __credits__ = ["Vitaly Saversky"]
-__version__ = "3.0.0"
+__version__ = "3.1.0"
 __maintainer__ = "Vitaly Saversky"
 __email__ = "larandvit@hotmail.com"
 __status__ = "Production"
 
 class FileFormat(IntEnum):
     SingleSchema = 1
     MultiSchemaFixed = 2
@@ -524,27 +524,36 @@
         
 def convert_error_message(recordLayoutType, field, fieldBytes, catchedError):
     return "Conversation error\t" + "Layout type: " + recordLayoutType + "\t" + str(field.name) + "\t" + str(fieldBytes) + "\t" + str(catchedError)
 
 def show_bytes(record):
     return [hex(num) for num in record]
 
+def current_folder():
+    return Path(__file__).parent
+
+def log_path(logFolder):
+    logFolder = str(logFolder)
+    logFilePath = path.join(path.dirname(__file__) if logFolder=="" else (current_folder() /logFolder).resolve(), LOGFILENAME)
+    return logFilePath
+
 def run(inputFile, 
         outputFolder,
         layoutFile,
         logfolder='',
         pythonEncoding=PYTHONENCODING,
         encodingName=INPUTENCODING,
         outputDelimiter=DELIMITER,
         outputFileExtension=OUTPUTFILEEXTENSION,
         ignoreConversionErrors=IGNORECONVERSIONERRORS,
         groupRecords=GROUPRECORDS,
         groupRecordsLevel2=GROUPRECORDSLEVEL2,
         verbose=VERBOSE,
-        debug=DEBUG_MODE):
+        debug=DEBUG_MODE,
+        cliMode=False):
     
     returnCode = 1
     
     dataConverter = None
     
     # store references to open output files. Keys as file names
     outputOpenFiles = {}
@@ -561,23 +570,24 @@
         filePath = inputFile
         outputFolder 
         layoutPath = layoutFile
         
         DELIMITER = outputDelimiter
         OUTPUTFILEEXTENSION = outputFileExtension
         IGNORECONVERSIONERRORS = ignoreConversionErrors
-        LOGFILEPATH = path.join(path.dirname(__file__) if logfolder=="" else logfolder, LOGFILENAME)
+        LOGFILEPATH = log_path(logfolder)
         PYTHONENCODING = pythonEncoding
         INPUTENCODING = encodingName
         GROUPRECORDS = groupRecords
         GROUPRECORDSLEVEL2 = groupRecordsLevel2
         VERBOSE = verbose
         DEBUG_MODE = debug
         
-        sys.stdout = Logger(LOGFILEPATH, VERBOSE)
+        if not cliMode:
+            sys.stdout = Logger(LOGFILEPATH, VERBOSE)
         
         fileName, fileExtension  = path.splitext(path.basename(filePath))
         
         # conversion engine class
         dataConverter = DataConverter(PYTHONENCODING, INPUTENCODING)
         
         # layout definitions and other supplemental info
@@ -1052,40 +1062,38 @@
         parser.add_argument("--grouprecordslevel2", nargs="?", default="yes" if GROUPRECORDSLEVEL2 else "no", choices=["yes","no"], help="create relationships between records for level 2", metavar='yes/no')
         parser.add_argument("--verbose", nargs="?", default="yes" if VERBOSE else "no", choices=["yes","no"], help="show information on screen", metavar='yes/no')
         parser.add_argument("--debug", nargs="?", default="yes" if DEBUG_MODE else "no", choices=["yes","no"], help="show debug information", metavar='yes/no')
     
         args = parser.parse_args()
         wrongArgumentsFlag = False
         
-        currentFolder = Path(__file__).parent
-        
         # mandatory arguments########################################################
-        filePath = (currentFolder / args.inputfile[0]).resolve()
-        outputFolder = (currentFolder / args.outputfolder[0]).resolve()
-        layoutPath = (currentFolder / args.layoutfile[0]).resolve()
+        filePath = (current_folder() / args.inputfile[0]).resolve()
+        outputFolder = (current_folder() / args.outputfolder[0]).resolve()
+        layoutPath = (current_folder() / args.layoutfile[0]).resolve()
         ##############################################################################
         
         # optional arguments##########################################################
         DELIMITER = args.outputdelimiter
         OUTPUTFILEEXTENSION = args.outputfileextension
         IGNORECONVERSIONERRORS = True if args.ignoreconversionerrors=="yes" else False
-        LOGFILEPATH = path.join(path.dirname(__file__) if args.logfolder=="" else args.logfolder, LOGFILENAME)
+        LOGFILEPATH = log_path(args.logfolder)
         PYTHONENCODING = True if args.pythonencoding=="yes" else False
         INPUTENCODING = args.encodingname
         GROUPRECORDS = True if args.grouprecords=="yes" else False
         GROUPRECORDSLEVEL2 = True if args.grouprecordslevel2=="yes" else False
         VERBOSE = True if args.verbose=="yes" else False
         DEBUG_MODE = True if args.debug=="yes" else False
         ##############################################################################
         
         sys.stdout = Logger(LOGFILEPATH, VERBOSE)
-        
         fileFolder = path.dirname(filePath)
         fileName, fileExtension  = path.splitext(path.basename(filePath))
         
+        print()
         print("Application version:", __version__)
         print("Stated:", datetime.datetime.now())
         print("Parameters:")
         print("-----------------------------------")
         print(f"Data folder: {fileFolder}")
         print(f"Output folder: {outputFolder}")
         print(f"Layout file: {layoutPath}")
@@ -1107,15 +1115,28 @@
             raise KnownIssue(layoutDefinition.errorDescription)
         
         print("Format:", "(" + str(layoutDefinition.fileFormat) + ")", FILEFORMATS[layoutDefinition.fileFormat])
         
         print("-----------------------------------")
         print()
         
-        run(filePath, outputFolder, layoutPath, args.logfolder, PYTHONENCODING, INPUTENCODING, DELIMITER, OUTPUTFILEEXTENSION, IGNORECONVERSIONERRORS, GROUPRECORDS, GROUPRECORDSLEVEL2, VERBOSE, DEBUG_MODE)
+        run(filePath, 
+            outputFolder, 
+            layoutPath, 
+            args.logfolder, 
+            PYTHONENCODING, 
+            INPUTENCODING, 
+            DELIMITER, 
+            OUTPUTFILEEXTENSION, 
+            IGNORECONVERSIONERRORS, 
+            GROUPRECORDS, 
+            GROUPRECORDSLEVEL2, 
+            VERBOSE, 
+            DEBUG_MODE,
+            cliMode=True)
          
     except KnownIssue as descr:
         print(descr)
             
     except SystemExit:
         #just used to catch system exit exception initiated by sys.exit()
         pass
```

### Comparing `ebcdic_parser-3.0.0/src/ebcdic_parser.egg-info/PKG-INFO` & `ebcdic_parser-3.1.0/src/ebcdic_parser.egg-info/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ebcdic-parser
-Version: 3.0.0
+Version: 3.1.0
 Summary: Convert mainframe EBCDIC data into Unicode ASCII delimited text files
 Home-page: https://github.com/larandvit/ebcdic-parser
 Author: Vitaly Saversky
 Author-email: larandvit@hotmail.com
 Project-URL: Bug Tracker, https://github.com/larandvit/ebcdic-parser/issues
 Project-URL: repository, https://github.com/larandvit/ebcdic-parser
 Classifier: Programming Language :: Python :: 3
@@ -26,20 +26,20 @@
  
 Conversion rules are a driver to parse EBCDIC data.
 
 ## Features
 
 * Supported layouts
     1. Single schema
-       * Original [COBOL layout](test_data/pr_p1_p2_gas_disposition/oga0861.pdf) and corresponding [conversion rules](layout_repository/gsf102_rules.json) file
+       * Original [COBOL layout](tests/test_data/pr_p1_p2_gas_disposition/oga0861.pdf) and corresponding [conversion rules](tests/layout_repository/gsf102_rules.json) file
     2. Multi-schema fixed record length
-       * Original [COBOL layout](test_data/ola013k/ola013k.pdf) and corresponding [conversion rules](layout_repository/ola013k_rules.json) file
+       * Original [COBOL layout](tests/test_data/ola013k/ola013k.pdf) and corresponding [conversion rules](tests/layout_repository/ola013k_rules.json) file
     3. Multi-schema variable record length
     4. Single schema variable record length
-       * Original [COBOL layout](test_data/service_segment_data/129.1DP.pdf) and corresponding [conversion rules](layout_repository/service_segment_data.json) file
+       * Original [COBOL layout](tests/test_data/service_segment_data/129.1DP.pdf) and corresponding [conversion rules](tests/layout_repository/service_segment_data.json) file
  
 * Fixing anomalies in EBCDIC files
     1. Skip header
     2. Skip footer
     3. Remove invalid characters
   
 * Adding relationship keys
@@ -48,14 +48,16 @@
      
 * Applicable encodings
     1. Python
     2. Java
     
 * Debug mode to troubleshoot layouts
 
+* Pip package or command prompt usage
+
 ## Conversion rules sample
 Detailed information about conversion rules setup file can be found in [Engine Rules](https://github.com/larandvit/ebcdic-parser/blob/master/docs/engine_rules_manual.md) manual. [COBOL Engine Rules Dictionary](https://github.com/larandvit/ebcdic-parser/blob/master/docs/cobol_engine_rules_dictionary.md) manual describes how to convert COBOL data types into engine rules layout.
 ```json
 {
     "description": "conversion rules sample",
     "header": [
         {
@@ -82,33 +84,84 @@
                 }
             ]
         }
     ]
 }
 ```
 
-## Installation
-It doesn't request any special installation if you are planning to use only Python encodings.
+## Pip Usage
 
-In case of using Java encodings, it has to be installed [javabridge](https://pypi.org/project/javabridge/) Python library. There is a constant in the code for including the javabridge library.
+### Installation
+
+```bash
+pip install ebcdic_parser
+```
+
+### Sample
+
+```python
+from ebcdic_parser.convert import run 
+
+
+run("../tests/test_data/311_calls_for_service_requests_all_strings/311_calls_for_service_requests_sample.dat", 
+    "../tests/test_data/311_calls_for_service_requests_all_strings/output",
+    "../tests/layout_repository/311_calls_for_service_requests_all_strings.json",
+    outputDelimiter=',')
+```
 
-## Usage
+### Run Function
+
+```
+run(inputFile, 
+    outputFolder,
+    layoutFile,
+    logfolder='',
+    pythonEncoding=True,
+    encodingName='cp037',
+    outputDelimiter=`\t`,
+    outputFileExtension=`.txt`,
+    ignoreConversionErrors=False,
+    groupRecords=False,
+    groupRecordsLevel2=False,
+    verbose=True,
+    debug=False,
+    cliMode=False):
 ```
-usage: ebcdic_parser.py [-h] --inputfile "input file path" --outputfolder
+
+
+* **inputfile** - input EBCDIC file path. Mandatory parameter. Absolute and relative paths are acceptable.
+* **outputfolder** - output folder to store delimited files. Mandatory parameter. Absolute and relative paths are acceptable.
+* **layoutfile** - layout file path. Mandatory parameter. Absolute and relative paths are acceptable.
+* **outputdelimiter** - output text file delimiter. Optional parameter. Default value is `\t`.
+* **outputfileextension** - output text file extension. Optional parameter. Default value is `.txt`.
+* **ignoreconversionerrors** - ignore any conversion error. Optional parameter. Default value is `False`.
+* **logfolder** - output folder to store log file. Optional parameter. Default value is the current folder. Absolute and relative paths are acceptable.
+* **pythonencoding** - use Python encoding rather than Java. Optional parameter. Default value is `True`.
+* **encodingname** - code page name to encode characters (Python or Java). Optional parameter. Default value is `cp037`.
+* **grouprecords** - create relationships between records. Optional parameter. Default value is `False'.
+* **grouprecordslevel2** - create relationships between records for level 2. Optional parameter. Default value is `False`.
+* **verbose** - show extended information on screen. Optional parameter. Default value is `True`.
+* **debug** - show debug information. Optional parameter. Default value is `False`.
+* **cliMode** - a flag how it run in command prompt or Pip installation.  
+
+
+## Command Prompt Usage
+```
+usage: convert.py [-h] --inputfile "input file path" --outputfolder
                         "output folder" --layoutfile "layout file"
                         [--outputdelimiter [delimiter]]
                         [--outputfileextension [extension]]
                         [--ignoreconversionerrors [yes/no]]
                         [--logfolder [log folder]] [--pythonencoding [yes/no]]
                         [--encodingname [encoding name]]
                         [--grouprecords [yes/no]]
                         [--grouprecordslevel2 [yes/no]] [--verbose [yes/no]]
                         [--debug [yes/no]]
 
-Convert EBCDIC data into delimited text format. Version 2.3.0
+Convert EBCDIC data into delimited text format. Version x.x.x
 
 Supported file formats:
 (1) Single schema
 (2) Multi-schema fixed length
 (3) Multi-schema variable length
 (4) Single schema variable length
 
@@ -143,64 +196,63 @@
                         create relationships between records for level 2
   --verbose [yes/no]    show information on screen
   --debug [yes/no]      show debug information
 
 Exit codes: 0 - successful completion, 1 - completion with any error
 ```
 
-## Samples
 ### Single schema #1
 
 ```bash
-ebcdic_parser.py --inputfile "./test_data/311_calls_for_service_requests_all_strings/311_calls_for_service_requests_sample.dat" --outputfolder "./test_data/311_calls_for_service_requests_all_strings/output" --layoutfile "./layout_repository/311_calls_for_service_requests_all_strings.json" --outputdelimiter ,
+convert.py --inputfile "../../tests/test_data/311_calls_for_service_requests_all_strings/311_calls_for_service_requests_sample.dat" --outputfolder "../../tests/test_data/311_calls_for_service_requests_all_strings/output" --layoutfile "../../tests/layout_repository/311_calls_for_service_requests_all_strings.json" --outputdelimiter ,
 ```
 
-* Output location: ./test_data/311_calls_for_service_requests_all_strings/output
+* Output location: ./tests/test_data/311_calls_for_service_requests_all_strings/output
 * Outptut format: comma delimited ASCII file
 * Log file: ./ebcdic_parser.log
 
 ### Single schema in debug mode #1
 
 ```bash
-ebcdic_parser.py --inputfile "./test_data/311_calls_for_service_requests_all_strings/311_calls_for_service_requests_sample.dat" --outputfolder "./test_data/311_calls_for_service_requests_all_strings/output" --layoutfile "./layout_repository/311_calls_for_service_requests_all_strings.json" --outputdelimiter , --debug yes
+convert.py --inputfile "../../tests/test_data/311_calls_for_service_requests_all_strings/311_calls_for_service_requests_sample.dat" --outputfolder "../../tests/test_data/311_calls_for_service_requests_all_strings/output" --layoutfile "../../tests/layout_repository/311_calls_for_service_requests_all_strings.json" --outputdelimiter , --debug yes
 ```
 
-* Output location: ./test_data/311_calls_for_service_requests_all_strings/output
+* Output location: ./tests/tests/test_data/311_calls_for_service_requests_all_strings/output
 * Outptut format: comma delimited ASCII file
 * Log file: ./ebcdic_parser.log
 
 ### Single schema #2
 
 ```bash
-ebcdic_parser.py --inputfile "./test_data/pr_p1_p2_gas_disposition/gsf102.ebc" --outputfolder "./test_data/pr_p1_p2_gas_disposition/output" --layoutfile "./layout_repository/gsf102_rules.json" --logfolder "./test_data/pr_p1_p2_gas_disposition/log"
+convert.py --inputfile "../../tests/test_data/pr_p1_p2_gas_disposition/gsf102.ebc" --outputfolder "../../tests/test_data/pr_p1_p2_gas_disposition/output" --layoutfile "../../tests/layout_repository/gsf102_rules.json" --logfolder "../../tests/test_data/pr_p1_p2_gas_disposition/log"
 ```
 
-* Output location: ./test_data/pr_p1_p2_gas_disposition/output
+* Output location: ./tests/test_data/pr_p1_p2_gas_disposition/output
 * Outptut format: tab delimited ASCII file
-* Log folder: ./test_data/pr_p1_p2_gas_disposition/log
+* Log folder: ./tests/test_data/pr_p1_p2_gas_disposition/log/ebcdic_parser.log
 
 ### Multi-schema fixed record length
 
 ```bash
-ebcdic_parser.py --inputfile "./test_data/ola013k/olf001l.ebc" --outputfolder "./test_data/ola013k/output" --layoutfile "./layout_repository/ola013k_rules.json" --logfolder "./test_data/ola013k/log"
+convert.py --inputfile "../../tests/test_data/ola013k/olf001l.ebc" --outputfolder "../../tests/test_data/ola013k/output" --layoutfile "../../tests/layout_repository/ola013k_rules.json"
 ```
 
-* Output location: ./test_data/ola013k/output
+* Output location: ./tests/test_data/ola013k/output
 * Outptut format: tab delimited ASCII file
-* Log folder: ./test_data/ola013k/log
+* Log folder: ./ebcdic_parser.log
 
 ### Single schema variable record length
 
 ```bash
-ebcdic_parser.py --inputfile "./test_data/service_segment_data/RG197.SERVSEG.Y70.ebc" --outputfolder "./test_data/service_segment_data/output" --layoutfile "./layout_repository/service_segment_data.json" --logfolder "./test_data/service_segment_data/log"
+convert.py --inputfile "../../tests/test_data/service_segment_data/RG197.SERVSEG.Y70.ebc" --outputfolder "../../tests/test_data/service_segment_data/output" --layoutfile "../../tests/layout_repository/service_segment_data.json"
 ```
 
-* Output location: ./test_data/service_segment_data/output
+* Output location: ./tests/test_data/service_segment_data/output
 * Outptut format: tab delimited ASCII file
-* Log folder: ./test_data/service_segment_data/log
+* Log folder: ./ebcdic_parser.log
 
 ## Testing
 ### Functional tests
 
 Those tests cover testing of each data type. 
 ```
 test_functional.py
@@ -212,14 +264,19 @@
 converter_to_ebcdic.py
 ```
 * Run tests
 ```
 test_system_311_calls_for_service_requests_all_strings.py
 ```
 
+## Java Encodings
+It doesn't request any special installation if you are planning to use only Python encodings.
+
+In case of using Java encodings, it has to be installed [javabridge](https://pypi.org/project/javabridge/) Python library. There is a constant in the code for including the javabridge library.
+
 ## Contributing
 Please read [CONTRIBUTING.md](https://github.com/larandvit/ebcdic-parser/blob/master/CONTRIBUTING.md) for details on our code of conduct, and the process for submitting pull requests to us.
  
 ## License
 This project is licensed under the MIT License - see the [LICENSE](https://github.com/larandvit/ebcdic-parser/blob/master/LICENSE) file for details
 
 ## Acknowledgments
```

### Comparing `ebcdic_parser-3.0.0/tests/test_functional.py` & `ebcdic_parser-3.1.0/tests/test_functional.py`

 * *Files identical despite different names*

### Comparing `ebcdic_parser-3.0.0/tests/test_system_311_calls_for_service_requests_all_strings.py` & `ebcdic_parser-3.1.0/tests/test_system_311_calls_for_service_requests_all_strings.py`

 * *Files identical despite different names*

### Comparing `ebcdic_parser-3.0.0/tests/test_system_common.py` & `ebcdic_parser-3.1.0/tests/test_system_common.py`

 * *Files identical despite different names*

