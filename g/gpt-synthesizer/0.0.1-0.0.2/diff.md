# Comparing `tmp/gpt-synthesizer-0.0.1.tar.gz` & `tmp/gpt-synthesizer-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gpt-synthesizer-0.0.1.tar", last modified: Sun Jul 30 20:05:33 2023, max compression
+gzip compressed data, was "gpt-synthesizer-0.0.2.tar", last modified: Sun Jul 30 20:22:05 2023, max compression
```

## Comparing `gpt-synthesizer-0.0.1.tar` & `gpt-synthesizer-0.0.2.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxrwxrwx   0 arash     (1000) arash     (1000)        0 2023-07-30 20:05:33.039314 gpt-synthesizer-0.0.1/
--rwxrwxrwx   0 arash     (1000) arash     (1000)     1078 2023-07-30 03:33:11.000000 gpt-synthesizer-0.0.1/LICENSE
--rwxrwxrwx   0 arash     (1000) arash     (1000)     6839 2023-07-30 20:05:33.038855 gpt-synthesizer-0.0.1/PKG-INFO
--rwxrwxrwx   0 arash     (1000) arash     (1000)     4690 2023-07-30 20:04:53.000000 gpt-synthesizer-0.0.1/README.md
-drwxrwxrwx   0 arash     (1000) arash     (1000)        0 2023-07-30 20:05:33.033544 gpt-synthesizer-0.0.1/gpt_synthesizer/
--rwxrwxrwx   0 arash     (1000) arash     (1000)        0 2023-07-13 19:46:26.000000 gpt-synthesizer-0.0.1/gpt_synthesizer/__init__.py
--rwxrwxrwx   0 arash     (1000) arash     (1000)     1404 2023-07-30 19:34:37.000000 gpt-synthesizer-0.0.1/gpt_synthesizer/generate_code.py
--rwxrwxrwx   0 arash     (1000) arash     (1000)     4384 2023-07-30 19:34:50.000000 gpt-synthesizer-0.0.1/gpt_synthesizer/main.py
--rwxrwxrwx   0 arash     (1000) arash     (1000)      504 2023-07-30 19:35:37.000000 gpt-synthesizer-0.0.1/gpt_synthesizer/model.py
--rwxrwxrwx   0 arash     (1000) arash     (1000)     3886 2023-07-30 02:47:57.000000 gpt-synthesizer-0.0.1/gpt_synthesizer/parser.py
--rwxrwxrwx   0 arash     (1000) arash     (1000)     7845 2023-07-30 19:35:08.000000 gpt-synthesizer-0.0.1/gpt_synthesizer/prompt.py
--rwxrwxrwx   0 arash     (1000) arash     (1000)     1848 2023-07-30 02:47:57.000000 gpt-synthesizer-0.0.1/gpt_synthesizer/ui.py
-drwxrwxrwx   0 arash     (1000) arash     (1000)        0 2023-07-30 20:05:33.037705 gpt-synthesizer-0.0.1/gpt_synthesizer.egg-info/
--rwxrwxrwx   0 arash     (1000) arash     (1000)     6839 2023-07-30 20:05:33.000000 gpt-synthesizer-0.0.1/gpt_synthesizer.egg-info/PKG-INFO
--rwxrwxrwx   0 arash     (1000) arash     (1000)      452 2023-07-30 20:05:33.000000 gpt-synthesizer-0.0.1/gpt_synthesizer.egg-info/SOURCES.txt
--rwxrwxrwx   0 arash     (1000) arash     (1000)        1 2023-07-30 20:05:33.000000 gpt-synthesizer-0.0.1/gpt_synthesizer.egg-info/dependency_links.txt
--rwxrwxrwx   0 arash     (1000) arash     (1000)       62 2023-07-30 20:05:33.000000 gpt-synthesizer-0.0.1/gpt_synthesizer.egg-info/entry_points.txt
--rwxrwxrwx   0 arash     (1000) arash     (1000)       42 2023-07-30 20:05:33.000000 gpt-synthesizer-0.0.1/gpt_synthesizer.egg-info/requires.txt
--rwxrwxrwx   0 arash     (1000) arash     (1000)       16 2023-07-30 20:05:33.000000 gpt-synthesizer-0.0.1/gpt_synthesizer.egg-info/top_level.txt
--rwxrwxrwx   0 arash     (1000) arash     (1000)     1290 2023-07-30 20:02:44.000000 gpt-synthesizer-0.0.1/pyproject.toml
--rwxrwxrwx   0 arash     (1000) arash     (1000)       38 2023-07-30 20:05:33.039465 gpt-synthesizer-0.0.1/setup.cfg
+drwxrwxrwx   0 arash     (1000) arash     (1000)        0 2023-07-30 20:22:05.782729 gpt-synthesizer-0.0.2/
+-rwxrwxrwx   0 arash     (1000) arash     (1000)     1078 2023-07-30 03:33:11.000000 gpt-synthesizer-0.0.2/LICENSE
+-rwxrwxrwx   0 arash     (1000) arash     (1000)     6989 2023-07-30 20:22:05.782404 gpt-synthesizer-0.0.2/PKG-INFO
+-rwxrwxrwx   0 arash     (1000) arash     (1000)     4840 2023-07-30 20:20:15.000000 gpt-synthesizer-0.0.2/README.md
+drwxrwxrwx   0 arash     (1000) arash     (1000)        0 2023-07-30 20:22:05.777143 gpt-synthesizer-0.0.2/gpt_synthesizer/
+-rwxrwxrwx   0 arash     (1000) arash     (1000)        0 2023-07-13 19:46:26.000000 gpt-synthesizer-0.0.2/gpt_synthesizer/__init__.py
+-rwxrwxrwx   0 arash     (1000) arash     (1000)     1404 2023-07-30 19:34:37.000000 gpt-synthesizer-0.0.2/gpt_synthesizer/generate_code.py
+-rwxrwxrwx   0 arash     (1000) arash     (1000)     4384 2023-07-30 19:34:50.000000 gpt-synthesizer-0.0.2/gpt_synthesizer/main.py
+-rwxrwxrwx   0 arash     (1000) arash     (1000)      504 2023-07-30 19:35:37.000000 gpt-synthesizer-0.0.2/gpt_synthesizer/model.py
+-rwxrwxrwx   0 arash     (1000) arash     (1000)     3886 2023-07-30 02:47:57.000000 gpt-synthesizer-0.0.2/gpt_synthesizer/parser.py
+-rwxrwxrwx   0 arash     (1000) arash     (1000)     7845 2023-07-30 19:35:08.000000 gpt-synthesizer-0.0.2/gpt_synthesizer/prompt.py
+-rwxrwxrwx   0 arash     (1000) arash     (1000)     1848 2023-07-30 02:47:57.000000 gpt-synthesizer-0.0.2/gpt_synthesizer/ui.py
+drwxrwxrwx   0 arash     (1000) arash     (1000)        0 2023-07-30 20:22:05.781595 gpt-synthesizer-0.0.2/gpt_synthesizer.egg-info/
+-rwxrwxrwx   0 arash     (1000) arash     (1000)     6989 2023-07-30 20:22:05.000000 gpt-synthesizer-0.0.2/gpt_synthesizer.egg-info/PKG-INFO
+-rwxrwxrwx   0 arash     (1000) arash     (1000)      452 2023-07-30 20:22:05.000000 gpt-synthesizer-0.0.2/gpt_synthesizer.egg-info/SOURCES.txt
+-rwxrwxrwx   0 arash     (1000) arash     (1000)        1 2023-07-30 20:22:05.000000 gpt-synthesizer-0.0.2/gpt_synthesizer.egg-info/dependency_links.txt
+-rwxrwxrwx   0 arash     (1000) arash     (1000)       62 2023-07-30 20:22:05.000000 gpt-synthesizer-0.0.2/gpt_synthesizer.egg-info/entry_points.txt
+-rwxrwxrwx   0 arash     (1000) arash     (1000)       42 2023-07-30 20:22:05.000000 gpt-synthesizer-0.0.2/gpt_synthesizer.egg-info/requires.txt
+-rwxrwxrwx   0 arash     (1000) arash     (1000)       16 2023-07-30 20:22:05.000000 gpt-synthesizer-0.0.2/gpt_synthesizer.egg-info/top_level.txt
+-rwxrwxrwx   0 arash     (1000) arash     (1000)     1290 2023-07-30 20:21:33.000000 gpt-synthesizer-0.0.2/pyproject.toml
+-rwxrwxrwx   0 arash     (1000) arash     (1000)       38 2023-07-30 20:22:05.782848 gpt-synthesizer-0.0.2/setup.cfg
```

### Comparing `gpt-synthesizer-0.0.1/LICENSE` & `gpt-synthesizer-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `gpt-synthesizer-0.0.1/PKG-INFO` & `gpt-synthesizer-0.0.2/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gpt-synthesizer
-Version: 0.0.1
+Version: 0.0.2
 Summary: Collaboratively build an entire codebase for any project with the help of an AI
 Author-email: RoboCoach Technologies <robocoachtechnologies@gmail.com>
 License: MIT License
         
         Copyright (c) 2023 RoboCoach Inc
         
         Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the “Software”), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
@@ -42,14 +42,20 @@
 - For development:
   - `git clone https://github.com/RoboCoachTechnologies/GPT-Synthesizer.git`
   - `cd gpt-synthesizer`
   - `pip install -e .`
 
 ## Usage
 
+GPT Synthesizer uses OpenAI's `gpt-3.5-turbo-16k` as the default LLM.
+
+- Setup your OpenAI API key: `export OPENAI_API_KEY=[your api key]`
+
+**Run**:
+
 - Start GPT Synthesizer by typing `gpt-synthesizer` in the terminal.
 - Briefly tell your programming task and the implementation language:
   - `Programming task: *I want to implement an edge detection method from live camera feed.*`
   - `Programming language: *python*`
 - GPT Synthesizer will analyze your task and suggest a set of components needed for the implementation.
   - You can add more components by listing them in quotation marks: `Components to be added: *Add 'component 1: what component 1 does', 'component 2: what component 2 does', and 'component 3: what component 3 does' to the list of components.*`
   - You can remove any redundant component in a similar manner: `Components to be removed: *Remove 'component 1' and 'component 2' from the list of components.*`
```

### Comparing `gpt-synthesizer-0.0.1/README.md` & `gpt-synthesizer-0.0.2/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -11,14 +11,20 @@
 - For development:
   - `git clone https://github.com/RoboCoachTechnologies/GPT-Synthesizer.git`
   - `cd gpt-synthesizer`
   - `pip install -e .`
 
 ## Usage
 
+GPT Synthesizer uses OpenAI's `gpt-3.5-turbo-16k` as the default LLM.
+
+- Setup your OpenAI API key: `export OPENAI_API_KEY=[your api key]`
+
+**Run**:
+
 - Start GPT Synthesizer by typing `gpt-synthesizer` in the terminal.
 - Briefly tell your programming task and the implementation language:
   - `Programming task: *I want to implement an edge detection method from live camera feed.*`
   - `Programming language: *python*`
 - GPT Synthesizer will analyze your task and suggest a set of components needed for the implementation.
   - You can add more components by listing them in quotation marks: `Components to be added: *Add 'component 1: what component 1 does', 'component 2: what component 2 does', and 'component 3: what component 3 does' to the list of components.*`
   - You can remove any redundant component in a similar manner: `Components to be removed: *Remove 'component 1' and 'component 2' from the list of components.*`
```

### Comparing `gpt-synthesizer-0.0.1/gpt_synthesizer/generate_code.py` & `gpt-synthesizer-0.0.2/gpt_synthesizer/generate_code.py`

 * *Files identical despite different names*

### Comparing `gpt-synthesizer-0.0.1/gpt_synthesizer/main.py` & `gpt-synthesizer-0.0.2/gpt_synthesizer/main.py`

 * *Files identical despite different names*

### Comparing `gpt-synthesizer-0.0.1/gpt_synthesizer/parser.py` & `gpt-synthesizer-0.0.2/gpt_synthesizer/parser.py`

 * *Files identical despite different names*

### Comparing `gpt-synthesizer-0.0.1/gpt_synthesizer/prompt.py` & `gpt-synthesizer-0.0.2/gpt_synthesizer/prompt.py`

 * *Files identical despite different names*

### Comparing `gpt-synthesizer-0.0.1/gpt_synthesizer/ui.py` & `gpt-synthesizer-0.0.2/gpt_synthesizer/ui.py`

 * *Files identical despite different names*

### Comparing `gpt-synthesizer-0.0.1/gpt_synthesizer.egg-info/PKG-INFO` & `gpt-synthesizer-0.0.2/gpt_synthesizer.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gpt-synthesizer
-Version: 0.0.1
+Version: 0.0.2
 Summary: Collaboratively build an entire codebase for any project with the help of an AI
 Author-email: RoboCoach Technologies <robocoachtechnologies@gmail.com>
 License: MIT License
         
         Copyright (c) 2023 RoboCoach Inc
         
         Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the “Software”), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
@@ -42,14 +42,20 @@
 - For development:
   - `git clone https://github.com/RoboCoachTechnologies/GPT-Synthesizer.git`
   - `cd gpt-synthesizer`
   - `pip install -e .`
 
 ## Usage
 
+GPT Synthesizer uses OpenAI's `gpt-3.5-turbo-16k` as the default LLM.
+
+- Setup your OpenAI API key: `export OPENAI_API_KEY=[your api key]`
+
+**Run**:
+
 - Start GPT Synthesizer by typing `gpt-synthesizer` in the terminal.
 - Briefly tell your programming task and the implementation language:
   - `Programming task: *I want to implement an edge detection method from live camera feed.*`
   - `Programming language: *python*`
 - GPT Synthesizer will analyze your task and suggest a set of components needed for the implementation.
   - You can add more components by listing them in quotation marks: `Components to be added: *Add 'component 1: what component 1 does', 'component 2: what component 2 does', and 'component 3: what component 3 does' to the list of components.*`
   - You can remove any redundant component in a similar manner: `Components to be removed: *Remove 'component 1' and 'component 2' from the list of components.*`
```

### Comparing `gpt-synthesizer-0.0.1/pyproject.toml` & `gpt-synthesizer-0.0.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires      = ["setuptools>=61.0.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "gpt-synthesizer"
-version = "0.0.1"
+version = "0.0.2"
 description = "Collaboratively build an entire codebase for any project with the help of an AI"
 readme = "README.md"
 authors = [{ name = "RoboCoach Technologies", email = "robocoachtechnologies@gmail.com" }]
 license = { file = "LICENSE" }
 classifiers = [
     "Development Status :: 2 - Pre-Alpha",
     "License :: OSI Approved :: MIT License",
```

