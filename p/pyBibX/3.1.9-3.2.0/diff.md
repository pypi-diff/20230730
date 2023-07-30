# Comparing `tmp/pyBibX-3.1.9.tar.gz` & `tmp/pyBibX-3.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\pyBibX-3.1.9.tar", last modified: Wed Jul 26 20:31:06 2023, max compression
+gzip compressed data, was "dist\pyBibX-3.2.0.tar", last modified: Sun Jul 30 01:01:27 2023, max compression
```

## Comparing `pyBibX-3.1.9.tar` & `pyBibX-3.2.0.tar`

### file list

```diff
@@ -1,48 +1,48 @@
-drwxrwxrwx   0        0        0        0 2023-07-26 20:31:06.000000 pyBibX-3.1.9/
--rw-rw-rw-   0        0        0      644 2022-03-01 19:24:07.000000 pyBibX-3.1.9/LICENSE
--rw-rw-rw-   0        0        0       40 2022-05-19 14:46:22.000000 pyBibX-3.1.9/MANIFEST.in
--rw-rw-rw-   0        0        0     9608 2023-07-26 20:31:06.000000 pyBibX-3.1.9/PKG-INFO
--rw-rw-rw-   0        0        0     9165 2023-05-06 14:18:32.000000 pyBibX-3.1.9/README.md
-drwxrwxrwx   0        0        0        0 2023-07-26 20:31:06.000000 pyBibX-3.1.9/pyBibX/
--rw-rw-rw-   0        0        0        1 2022-03-01 07:37:35.000000 pyBibX-3.1.9/pyBibX/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-26 20:31:06.000000 pyBibX-3.1.9/pyBibX/base/
--rw-rw-rw-   0        0        0       27 2022-03-16 15:26:25.000000 pyBibX-3.1.9/pyBibX/base/__init__.py
--rw-rw-rw-   0        0        0   268495 2023-07-26 20:29:07.000000 pyBibX-3.1.9/pyBibX/base/pbx.py
-drwxrwxrwx   0        0        0        0 2023-07-26 20:31:06.000000 pyBibX-3.1.9/pyBibX/base/stws/
--rw-rw-rw-   0        0        0     6482 2023-05-31 13:32:50.000000 pyBibX-3.1.9/pyBibX/base/stws/Stopwords-Arabic.txt
--rw-rw-rw-   0        0        0     1484 2017-07-30 20:46:06.000000 pyBibX-3.1.9/pyBibX/base/stws/Stopwords-Bengali.txt
--rw-rw-rw-   0        0        0     2408 2017-07-30 20:46:06.000000 pyBibX-3.1.9/pyBibX/base/stws/Stopwords-Bulgarian.txt
--rw-rw-rw-   0        0        0     3295 2023-05-28 21:46:34.000000 pyBibX-3.1.9/pyBibX/base/stws/Stopwords-Chinese.txt
--rw-rw-rw-   0        0        0     1934 2023-05-31 13:36:06.000000 pyBibX-3.1.9/pyBibX/base/stws/Stopwords-Czech.txt
--rw-rw-rw-   0        0        0     4284 2023-05-31 13:37:00.000000 pyBibX-3.1.9/pyBibX/base/stws/Stopwords-English.txt
--rw-rw-rw-   0        0        0     6219 2017-07-30 20:46:06.000000 pyBibX-3.1.9/pyBibX/base/stws/Stopwords-Finnish.txt
--rw-rw-rw-   0        0        0     3484 2023-05-31 13:37:46.000000 pyBibX-3.1.9/pyBibX/base/stws/Stopwords-French.txt
--rw-rw-rw-   0        0        0     4302 2023-05-31 13:39:46.000000 pyBibX-3.1.9/pyBibX/base/stws/Stopwords-German.txt
--rw-rw-rw-   0        0        0     7901 2023-05-28 21:47:27.000000 pyBibX-3.1.9/pyBibX/base/stws/Stopwords-Greek.txt
--rw-rw-rw-   0        0        0     1656 2023-05-28 21:47:36.000000 pyBibX-3.1.9/pyBibX/base/stws/Stopwords-Hebrew.txt
--rw-rw-rw-   0        0        0     2065 2017-07-30 20:46:06.000000 pyBibX-3.1.9/pyBibX/base/stws/Stopwords-Hindi.txt
--rw-rw-rw-   0        0        0     5552 2017-07-30 20:46:06.000000 pyBibX-3.1.9/pyBibX/base/stws/Stopwords-Hungarian.txt
--rw-rw-rw-   0        0        0     4074 2023-05-31 13:48:26.000000 pyBibX-3.1.9/pyBibX/base/stws/Stopwords-Italian.txt
--rw-rw-rw-   0        0        0     2202 2023-05-28 21:48:04.000000 pyBibX-3.1.9/pyBibX/base/stws/Stopwords-Japanese.txt
--rw-rw-rw-   0        0        0     7417 2023-05-28 21:48:29.000000 pyBibX-3.1.9/pyBibX/base/stws/Stopwords-Korean.txt
--rw-rw-rw-   0        0        0     1307 2017-07-30 20:46:06.000000 pyBibX-3.1.9/pyBibX/base/stws/Stopwords-Marathi.txt
--rw-rw-rw-   0        0        0     3274 2017-07-30 20:46:06.000000 pyBibX-3.1.9/pyBibX/base/stws/Stopwords-Persian.txt
--rw-rw-rw-   0        0        0      704 2017-07-30 20:46:06.000000 pyBibX-3.1.9/pyBibX/base/stws/Stopwords-Polish.txt
--rw-rw-rw-   0        0        0     3772 2019-05-09 13:59:54.000000 pyBibX-3.1.9/pyBibX/base/stws/Stopwords-Portuguese-br.txt
--rw-rw-rw-   0        0        0     1926 2017-07-30 20:46:06.000000 pyBibX-3.1.9/pyBibX/base/stws/Stopwords-Romanian.txt
--rw-rw-rw-   0        0        0     4963 2017-07-30 20:46:06.000000 pyBibX-3.1.9/pyBibX/base/stws/Stopwords-Russian.txt
--rw-rw-rw-   0        0        0      883 2023-05-28 21:48:40.000000 pyBibX-3.1.9/pyBibX/base/stws/Stopwords-Slovak.txt
--rw-rw-rw-   0        0        0     3128 2023-05-31 13:53:58.000000 pyBibX-3.1.9/pyBibX/base/stws/Stopwords-Spanish.txt
--rw-rw-rw-   0        0        0     2757 2017-07-30 20:46:06.000000 pyBibX-3.1.9/pyBibX/base/stws/Stopwords-Swedish.txt
--rw-rw-rw-   0        0        0     1521 2023-05-28 21:58:26.000000 pyBibX-3.1.9/pyBibX/base/stws/Stopwords-Thai.txt
--rw-rw-rw-   0        0        0      627 2023-05-28 21:49:00.000000 pyBibX-3.1.9/pyBibX/base/stws/Stopwords-Ukrainian.txt
--rw-rw-rw-   0        0        0        1 2022-03-01 07:37:35.000000 pyBibX-3.1.9/pyBibX/base/stws/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-26 20:31:06.000000 pyBibX-3.1.9/pyBibX.egg-info/
--rw-rw-rw-   0        0        0     9608 2023-07-26 20:31:04.000000 pyBibX-3.1.9/pyBibX.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1354 2023-07-26 20:31:05.000000 pyBibX-3.1.9/pyBibX.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-26 20:31:04.000000 pyBibX-3.1.9/pyBibX.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      218 2023-07-26 20:31:04.000000 pyBibX-3.1.9/pyBibX.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2023-07-26 20:31:04.000000 pyBibX-3.1.9/pyBibX.egg-info/top_level.txt
--rw-rw-rw-   0        0        0        2 2023-07-26 20:31:04.000000 pyBibX-3.1.9/pyBibX.egg-info/zip-safe
--rw-rw-rw-   0        0        0       42 2023-07-26 20:31:06.000000 pyBibX-3.1.9/setup.cfg
--rw-rw-rw-   0        0        0     1101 2023-07-26 20:29:21.000000 pyBibX-3.1.9/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-30 01:01:27.000000 pyBibX-3.2.0/
+-rw-rw-rw-   0        0        0      644 2022-03-01 19:24:07.000000 pyBibX-3.2.0/LICENSE
+-rw-rw-rw-   0        0        0       40 2022-05-19 14:46:22.000000 pyBibX-3.2.0/MANIFEST.in
+-rw-rw-rw-   0        0        0     9608 2023-07-30 01:01:27.000000 pyBibX-3.2.0/PKG-INFO
+-rw-rw-rw-   0        0        0     9165 2023-05-06 14:18:32.000000 pyBibX-3.2.0/README.md
+drwxrwxrwx   0        0        0        0 2023-07-30 01:01:27.000000 pyBibX-3.2.0/pyBibX/
+-rw-rw-rw-   0        0        0        1 2022-03-01 07:37:35.000000 pyBibX-3.2.0/pyBibX/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-30 01:01:27.000000 pyBibX-3.2.0/pyBibX/base/
+-rw-rw-rw-   0        0        0       27 2022-03-16 15:26:25.000000 pyBibX-3.2.0/pyBibX/base/__init__.py
+-rw-rw-rw-   0        0        0   275287 2023-07-30 00:36:53.000000 pyBibX-3.2.0/pyBibX/base/pbx.py
+drwxrwxrwx   0        0        0        0 2023-07-30 01:01:27.000000 pyBibX-3.2.0/pyBibX/base/stws/
+-rw-rw-rw-   0        0        0     6482 2023-05-31 13:32:50.000000 pyBibX-3.2.0/pyBibX/base/stws/Stopwords-Arabic.txt
+-rw-rw-rw-   0        0        0     1484 2017-07-30 20:46:06.000000 pyBibX-3.2.0/pyBibX/base/stws/Stopwords-Bengali.txt
+-rw-rw-rw-   0        0        0     2408 2017-07-30 20:46:06.000000 pyBibX-3.2.0/pyBibX/base/stws/Stopwords-Bulgarian.txt
+-rw-rw-rw-   0        0        0     3295 2023-05-28 21:46:34.000000 pyBibX-3.2.0/pyBibX/base/stws/Stopwords-Chinese.txt
+-rw-rw-rw-   0        0        0     1934 2023-05-31 13:36:06.000000 pyBibX-3.2.0/pyBibX/base/stws/Stopwords-Czech.txt
+-rw-rw-rw-   0        0        0     4284 2023-05-31 13:37:00.000000 pyBibX-3.2.0/pyBibX/base/stws/Stopwords-English.txt
+-rw-rw-rw-   0        0        0     6219 2017-07-30 20:46:06.000000 pyBibX-3.2.0/pyBibX/base/stws/Stopwords-Finnish.txt
+-rw-rw-rw-   0        0        0     3484 2023-05-31 13:37:46.000000 pyBibX-3.2.0/pyBibX/base/stws/Stopwords-French.txt
+-rw-rw-rw-   0        0        0     4302 2023-05-31 13:39:46.000000 pyBibX-3.2.0/pyBibX/base/stws/Stopwords-German.txt
+-rw-rw-rw-   0        0        0     7901 2023-05-28 21:47:27.000000 pyBibX-3.2.0/pyBibX/base/stws/Stopwords-Greek.txt
+-rw-rw-rw-   0        0        0     1656 2023-05-28 21:47:36.000000 pyBibX-3.2.0/pyBibX/base/stws/Stopwords-Hebrew.txt
+-rw-rw-rw-   0        0        0     2065 2017-07-30 20:46:06.000000 pyBibX-3.2.0/pyBibX/base/stws/Stopwords-Hindi.txt
+-rw-rw-rw-   0        0        0     5552 2017-07-30 20:46:06.000000 pyBibX-3.2.0/pyBibX/base/stws/Stopwords-Hungarian.txt
+-rw-rw-rw-   0        0        0     4074 2023-05-31 13:48:26.000000 pyBibX-3.2.0/pyBibX/base/stws/Stopwords-Italian.txt
+-rw-rw-rw-   0        0        0     2202 2023-05-28 21:48:04.000000 pyBibX-3.2.0/pyBibX/base/stws/Stopwords-Japanese.txt
+-rw-rw-rw-   0        0        0     7417 2023-05-28 21:48:29.000000 pyBibX-3.2.0/pyBibX/base/stws/Stopwords-Korean.txt
+-rw-rw-rw-   0        0        0     1307 2017-07-30 20:46:06.000000 pyBibX-3.2.0/pyBibX/base/stws/Stopwords-Marathi.txt
+-rw-rw-rw-   0        0        0     3274 2017-07-30 20:46:06.000000 pyBibX-3.2.0/pyBibX/base/stws/Stopwords-Persian.txt
+-rw-rw-rw-   0        0        0      704 2017-07-30 20:46:06.000000 pyBibX-3.2.0/pyBibX/base/stws/Stopwords-Polish.txt
+-rw-rw-rw-   0        0        0     3772 2019-05-09 13:59:54.000000 pyBibX-3.2.0/pyBibX/base/stws/Stopwords-Portuguese-br.txt
+-rw-rw-rw-   0        0        0     1926 2017-07-30 20:46:06.000000 pyBibX-3.2.0/pyBibX/base/stws/Stopwords-Romanian.txt
+-rw-rw-rw-   0        0        0     4963 2017-07-30 20:46:06.000000 pyBibX-3.2.0/pyBibX/base/stws/Stopwords-Russian.txt
+-rw-rw-rw-   0        0        0      883 2023-05-28 21:48:40.000000 pyBibX-3.2.0/pyBibX/base/stws/Stopwords-Slovak.txt
+-rw-rw-rw-   0        0        0     3128 2023-05-31 13:53:58.000000 pyBibX-3.2.0/pyBibX/base/stws/Stopwords-Spanish.txt
+-rw-rw-rw-   0        0        0     2757 2017-07-30 20:46:06.000000 pyBibX-3.2.0/pyBibX/base/stws/Stopwords-Swedish.txt
+-rw-rw-rw-   0        0        0     1521 2023-05-28 21:58:26.000000 pyBibX-3.2.0/pyBibX/base/stws/Stopwords-Thai.txt
+-rw-rw-rw-   0        0        0      627 2023-05-28 21:49:00.000000 pyBibX-3.2.0/pyBibX/base/stws/Stopwords-Ukrainian.txt
+-rw-rw-rw-   0        0        0        1 2022-03-01 07:37:35.000000 pyBibX-3.2.0/pyBibX/base/stws/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-30 01:01:27.000000 pyBibX-3.2.0/pyBibX.egg-info/
+-rw-rw-rw-   0        0        0     9608 2023-07-30 01:01:26.000000 pyBibX-3.2.0/pyBibX.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1354 2023-07-30 01:01:26.000000 pyBibX-3.2.0/pyBibX.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-30 01:01:26.000000 pyBibX-3.2.0/pyBibX.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      218 2023-07-30 01:01:26.000000 pyBibX-3.2.0/pyBibX.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2023-07-30 01:01:26.000000 pyBibX-3.2.0/pyBibX.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0        2 2023-07-30 01:01:26.000000 pyBibX-3.2.0/pyBibX.egg-info/zip-safe
+-rw-rw-rw-   0        0        0       42 2023-07-30 01:01:27.000000 pyBibX-3.2.0/setup.cfg
+-rw-rw-rw-   0        0        0     1101 2023-07-30 01:00:04.000000 pyBibX-3.2.0/setup.py
```

### Comparing `pyBibX-3.1.9/LICENSE` & `pyBibX-3.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pyBibX-3.1.9/PKG-INFO` & `pyBibX-3.2.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyBibX
-Version: 3.1.9
+Version: 3.2.0
 Summary: A Bibliometric and Scientometric Library Powered with Artificial Intelligence Tools
 Home-page: https://github.com/Valdecy/pyBibX
 Author: Valdecy Pereira
 Author-email: valdecy.pereira@gmail.com
 License: GNU
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `pyBibX-3.1.9/README.md` & `pyBibX-3.2.0/README.md`

 * *Files identical despite different names*

### Comparing `pyBibX-3.1.9/pyBibX/base/pbx.py` & `pyBibX-3.2.0/pyBibX/base/pbx.py`

 * *Files 2% similar despite different names*

```diff
@@ -4132,23 +4132,32 @@
         return summary
 
 ############################################################################
 
     # Function: Ask chatGPT about Authors Productivity by Year
     def ask_chatgpt_ap(self, char_limit = 4097, api_key = 'your_api_key_here', query = 'give me insights about the following information, related to authors productivity by year', model = 'text-davinci-003', max_tokens = 2000, n = 1, temperature = 0.8):
         def query_chatgpt(prompt, model = model, max_tokens = max_tokens, n = n, temperature = temperature):
-            response = openai.Completion.create(
-                                                engine      = model,
-                                                prompt      = prompt,
-                                                max_tokens  = max_tokens,
-                                                n           = n,
-                                                stop        = None,
-                                                temperature = temperature
-                                                )
-            return response.choices[0].text.strip()
+            try: 
+                response = openai.ChatCompletion.create(
+                                                        model      = model,
+                                                        messages   = [{'role': 'user', 'content': prompt}],
+                                                        max_tokens = max_tokens
+                                                        )
+                response = response['choices'][0]['message']['content']
+            except:
+                response = openai.Completion.create(
+                                                    engine      = model,
+                                                    prompt      = prompt,
+                                                    max_tokens  = max_tokens,
+                                                    n           = n,
+                                                    stop        = None,
+                                                    temperature = temperature
+                                                    )
+                response = response.choices[0].text.strip()
+            return response
         corpus = ''
         for author, row in self.ask_gpt_ap.iterrows():
             years        = [(year, row[year]) for year in row.index if row[year] > 0]
             paper_counts = ', '.join([f'({year}: {count} paper{"s" if count > 1 else ""})' for year, count in years])
             corpus       = corpus +  f'{author} {paper_counts}\n'
         openai.api_key = api_key
         prompt         = query + ':\n\n' + f'{corpus}\n'
@@ -4156,232 +4165,331 @@
         analyze        = query_chatgpt(prompt)
         print('Number of Characters: ' + str(len(prompt)))
         return analyze
     
     # Function: Ask chatGPT about Bar Plots 
     def ask_chatgpt_bp(self, char_limit = 4097, api_key = 'your_api_key_here', query = 'give me insights about the following information', model = 'text-davinci-003', max_tokens = 2000, n = 1, temperature = 0.8):
         def query_chatgpt(prompt, model = model, max_tokens = max_tokens, n = n, temperature = temperature):
-            response = openai.Completion.create(
-                                                engine      = model,
-                                                prompt      = prompt,
-                                                max_tokens  = max_tokens,
-                                                n           = n,
-                                                stop        = None,
-                                                temperature = temperature
-                                                )
-            return response.choices[0].text.strip()
+            try: 
+                response = openai.ChatCompletion.create(
+                                                        model      = model,
+                                                        messages   = [{'role': 'user', 'content': prompt}],
+                                                        max_tokens = max_tokens
+                                                        )
+                response = response['choices'][0]['message']['content']
+            except:
+                response = openai.Completion.create(
+                                                    engine      = model,
+                                                    prompt      = prompt,
+                                                    max_tokens  = max_tokens,
+                                                    n           = n,
+                                                    stop        = None,
+                                                    temperature = temperature
+                                                    )
+                response = response.choices[0].text.strip()
+            return response
         corpus         = self.ask_gpt_bp.to_string(index = False)    
         openai.api_key = api_key
         prompt         = query + ' regarding ' + self.ask_gpt_bp_t + ':\n\n' + f'{corpus}\n'
         prompt         = prompt[:char_limit]
         analyze        = query_chatgpt(prompt)
         print('Number of Characters: ' + str(len(prompt)))
         return analyze
     
     # Function: Ask chatGPT about Citation Analysis 
     def ask_chatgpt_citation(self, char_limit = 4097, api_key = 'your_api_key_here', query = 'give me insights about the following information', model = 'text-davinci-003', max_tokens = 2000, n = 1, temperature = 0.8):
         def query_chatgpt(prompt, model = model, max_tokens = max_tokens, n = n, temperature = temperature):
-            response = openai.Completion.create(
-                                                engine      = model,
-                                                prompt      = prompt,
-                                                max_tokens  = max_tokens,
-                                                n           = n,
-                                                stop        = None,
-                                                temperature = temperature
-                                                )
-            return response.choices[0].text.strip()
+            try: 
+                response = openai.ChatCompletion.create(
+                                                        model      = model,
+                                                        messages   = [{'role': 'user', 'content': prompt}],
+                                                        max_tokens = max_tokens
+                                                        )
+                response = response['choices'][0]['message']['content']
+            except:
+                response = openai.Completion.create(
+                                                    engine      = model,
+                                                    prompt      = prompt,
+                                                    max_tokens  = max_tokens,
+                                                    n           = n,
+                                                    stop        = None,
+                                                    temperature = temperature
+                                                    )
+                response = response.choices[0].text.strip()
+            return response
         corpus         = self.ask_gpt_nad.to_string(index = False)    
         openai.api_key = api_key
         prompt         = query + ':\n\n' + f'{corpus}\n'
         prompt         = prompt[:char_limit]
         analyze        = query_chatgpt(prompt)
         print('Number of Characters: ' + str(len(prompt)))
         return analyze
 
     # Function: Ask chatGPT about Collaboration Analysis
     def ask_chatgpt_colab(self, char_limit = 4097, api_key = 'your_api_key_here', query = 'give me insights about the following network information, knowing that Node 1 is connected with Node 2', model = 'text-davinci-003', max_tokens = 2000, n = 1, temperature = 0.8):
         def query_chatgpt(prompt, model = model, max_tokens = max_tokens, n = n, temperature = temperature):
-            response = openai.Completion.create(
-                                                engine      = model,
-                                                prompt      = prompt,
-                                                max_tokens  = max_tokens,
-                                                n           = n,
-                                                stop        = None,
-                                                temperature = temperature
-                                                )
-            return response.choices[0].text.strip()
+            try: 
+                response = openai.ChatCompletion.create(
+                                                        model      = model,
+                                                        messages   = [{'role': 'user', 'content': prompt}],
+                                                        max_tokens = max_tokens
+                                                        )
+                response = response['choices'][0]['message']['content']
+            except:
+                response = openai.Completion.create(
+                                                    engine      = model,
+                                                    prompt      = prompt,
+                                                    max_tokens  = max_tokens,
+                                                    n           = n,
+                                                    stop        = None,
+                                                    temperature = temperature
+                                                    )
+                response = response.choices[0].text.strip()
+            return response
         corpus         = self.ask_gpt_adj.to_string(index = False)
         openai.api_key = api_key
         prompt         = query + ':\n\n' + f'{corpus}\n'
         prompt         = prompt[:char_limit]
         analyze        = query_chatgpt(prompt)
         print('Number of Characters: ' + str(len(prompt)))
         return analyze
 
     # Function: Ask chatGPT about EDA Report 
     def ask_chatgpt_eda(self, char_limit = 4097, api_key = 'your_api_key_here', query = 'give me insights about the following information', model = 'text-davinci-003', max_tokens = 2000, n = 1, temperature = 0.8):
         def query_chatgpt(prompt, model = model, max_tokens = max_tokens, n = n, temperature = temperature):
-            response = openai.Completion.create(
-                                                engine      = model,
-                                                prompt      = prompt,
-                                                max_tokens  = max_tokens,
-                                                n           = n,
-                                                stop        = None,
-                                                temperature = temperature
-                                                )
-            return response.choices[0].text.strip()
+            try: 
+                response = openai.ChatCompletion.create(
+                                                        model      = model,
+                                                        messages   = [{'role': 'user', 'content': prompt}],
+                                                        max_tokens = max_tokens
+                                                        )
+                response = response['choices'][0]['message']['content']
+            except:
+                response = openai.Completion.create(
+                                                    engine      = model,
+                                                    prompt      = prompt,
+                                                    max_tokens  = max_tokens,
+                                                    n           = n,
+                                                    stop        = None,
+                                                    temperature = temperature
+                                                    )
+                response = response.choices[0].text.strip()
+            return response
         corpus         = self.ask_gpt_rt.to_string(index = False)    
         lines          = corpus.split('\n')
         corpus         = '\n'.join(' '.join(line.split()) for line in lines)
         openai.api_key = api_key
         prompt         = query + ':\n\n' + f'{corpus}\n'
         prompt         = prompt[:char_limit]
         analyze        = query_chatgpt(prompt)
         print('Number of Characters: ' + str(len(prompt)))
         return analyze
     
     # Function: Ask chatGPT about Evolution Plot
     def ask_chatgpt_ep(self, char_limit = 4097, api_key = 'your_api_key_here', query = 'give me insights about the following information, related to words apperance by year', model = 'text-davinci-003', max_tokens = 2000, n = 1, temperature = 0.8):
         def query_chatgpt(prompt, model = model, max_tokens = max_tokens, n = n, temperature = temperature):
-            response = openai.Completion.create(
-                                                engine      = model,
-                                                prompt      = prompt,
-                                                max_tokens  = max_tokens,
-                                                n           = n,
-                                                stop        = None,
-                                                temperature = temperature
-                                                )
-            return response.choices[0].text.strip()
+            try: 
+                response = openai.ChatCompletion.create(
+                                                        model      = model,
+                                                        messages   = [{'role': 'user', 'content': prompt}],
+                                                        max_tokens = max_tokens
+                                                        )
+                response = response['choices'][0]['message']['content']
+            except:
+                response = openai.Completion.create(
+                                                    engine      = model,
+                                                    prompt      = prompt,
+                                                    max_tokens  = max_tokens,
+                                                    n           = n,
+                                                    stop        = None,
+                                                    temperature = temperature
+                                                    )
+                response = response.choices[0].text.strip()
+            return response
         corpus         = self.ask_gpt_ep
         openai.api_key = api_key
         prompt         = query + ':\n\n' + f'{corpus}\n'
         prompt         = prompt[:char_limit]
         analyze        = query_chatgpt(prompt)
         print('Number of Characters: ' + str(len(prompt)))
         return analyze
 
     # Function: Ask chatGPT about Citation Analysis 
     def ask_chatgpt_hist(self, char_limit = 4097, api_key = 'your_api_key_here', query = 'give me insights about the following information relating the most influential references, also discover if there is relevant network connections', model = 'text-davinci-003', max_tokens = 2000, n = 1, temperature = 0.8):
         def query_chatgpt(prompt, model = model, max_tokens = max_tokens, n = n, temperature = temperature):
-            response = openai.Completion.create(
-                                                engine      = model,
-                                                prompt      = prompt,
-                                                max_tokens  = max_tokens,
-                                                n           = n,
-                                                stop        = None,
-                                                temperature = temperature
-                                                )
-            return response.choices[0].text.strip()
+            try: 
+                response = openai.ChatCompletion.create(
+                                                        model      = model,
+                                                        messages   = [{'role': 'user', 'content': prompt}],
+                                                        max_tokens = max_tokens
+                                                        )
+                response = response['choices'][0]['message']['content']
+            except:
+                response = openai.Completion.create(
+                                                    engine      = model,
+                                                    prompt      = prompt,
+                                                    max_tokens  = max_tokens,
+                                                    n           = n,
+                                                    stop        = None,
+                                                    temperature = temperature
+                                                    )
+                response = response.choices[0].text.strip()
+            return response
         corpus = []
         for i in range(0, self.ask_gpt_hist.shape[0]):
             corpus.append('Paper ' + self.ask_gpt_hist.iloc[i,0] + ' Cites Paper ' + self.ask_gpt_hist.iloc[i,1])
         corpus         = ', '.join(corpus)    
         openai.api_key = api_key
         prompt         = query + ':\n\n' + f'{corpus}\n'
         prompt         = prompt[:char_limit]
         analyze        = query_chatgpt(prompt)
         print('Number of Characters: ' + str(len(prompt)))
         return analyze
 
     # Function: Ask chatGPT about Map Analysis 
     def ask_chatgpt_map(self, char_limit = 4097, api_key = 'your_api_key_here', query = 'give me insights about the following information', model = 'text-davinci-003', max_tokens = 2000, n = 1, temperature = 0.8):
         def query_chatgpt(prompt, model = model, max_tokens = max_tokens, n = n, temperature = temperature):
-            response = openai.Completion.create(
-                                                engine      = model,
-                                                prompt      = prompt,
-                                                max_tokens  = max_tokens,
-                                                n           = n,
-                                                stop        = None,
-                                                temperature = temperature
-                                                )
-            return response.choices[0].text.strip()
+            try: 
+                response = openai.ChatCompletion.create(
+                                                        model      = model,
+                                                        messages   = [{'role': 'user', 'content': prompt}],
+                                                        max_tokens = max_tokens
+                                                        )
+                response = response['choices'][0]['message']['content']
+            except:
+                response = openai.Completion.create(
+                                                    engine      = model,
+                                                    prompt      = prompt,
+                                                    max_tokens  = max_tokens,
+                                                    n           = n,
+                                                    stop        = None,
+                                                    temperature = temperature
+                                                    )
+                response = response.choices[0].text.strip()
+            return response
         corpus         = self.ask_gpt_map.to_string(index = False)
         openai.api_key = api_key
         prompt         = query + ':\n\n' + f'{corpus}\n'
         prompt         = prompt[:char_limit]
         analyze        = query_chatgpt(prompt)
         print('Number of Characters: ' + str(len(prompt)))
         return analyze
 
     # Function: Ask chatGPT about N-Grms 
     def ask_chatgpt_ngrams(self, char_limit = 4097, api_key = 'your_api_key_here', query = 'give me insights about the following information relating the n-grams and their frequency', model = 'text-davinci-003', max_tokens = 2000, n = 1, temperature = 0.8):
         def query_chatgpt(prompt, model = model, max_tokens = max_tokens, n = n, temperature = temperature):
-            response = openai.Completion.create(
-                                                engine      = model,
-                                                prompt      = prompt,
-                                                max_tokens  = max_tokens,
-                                                n           = n,
-                                                stop        = None,
-                                                temperature = temperature
-                                                )
-            return response.choices[0].text.strip()
+            try: 
+                response = openai.ChatCompletion.create(
+                                                        model      = model,
+                                                        messages   = [{'role': 'user', 'content': prompt}],
+                                                        max_tokens = max_tokens
+                                                        )
+                response = response['choices'][0]['message']['content']
+            except:
+                response = openai.Completion.create(
+                                                    engine      = model,
+                                                    prompt      = prompt,
+                                                    max_tokens  = max_tokens,
+                                                    n           = n,
+                                                    stop        = None,
+                                                    temperature = temperature
+                                                    )
+                response = response.choices[0].text.strip()
+            return response
         corpus         = self.ask_gpt_ng.to_string(index = False)  
         lines          = corpus.split('\n')
         corpus         = '\n'.join(' '.join(line.split()) for line in lines)  
         openai.api_key = api_key
         prompt         = query + ':\n\n' + f'{corpus}\n'
         prompt         = prompt[:char_limit]
         analyze        = query_chatgpt(prompt)
         print('Number of Characters: ' + str(len(prompt)))
         return analyze
 
     # Function: Ask chatGPT about Sankey Diagram
     def ask_chatgpt_sankey(self, char_limit = 4097, api_key = 'your_api_key_here', query = 'give me insights about the following information from a network called Sankey', model = 'text-davinci-003', max_tokens = 2000, n = 1, temperature = 0.8):
         def query_chatgpt(prompt, model = model, max_tokens = max_tokens, n = n, temperature = temperature):
-            response = openai.Completion.create(
-                                                engine      = model,
-                                                prompt      = prompt,
-                                                max_tokens  = max_tokens,
-                                                n           = n,
-                                                stop        = None,
-                                                temperature = temperature
-                                                )
-            return response.choices[0].text.strip()
+            try: 
+                response = openai.ChatCompletion.create(
+                                                        model      = model,
+                                                        messages   = [{'role': 'user', 'content': prompt}],
+                                                        max_tokens = max_tokens
+                                                        )
+                response = response['choices'][0]['message']['content']
+            except:
+                response = openai.Completion.create(
+                                                    engine      = model,
+                                                    prompt      = prompt,
+                                                    max_tokens  = max_tokens,
+                                                    n           = n,
+                                                    stop        = None,
+                                                    temperature = temperature
+                                                    )
+                response = response.choices[0].text.strip()
+            return response
         corpus         = self.ask_gpt_sk.to_string(index = False)   
         lines          = corpus.split('\n')
         corpus         = '\n'.join(' '.join(line.split()) for line in lines)
         openai.api_key = api_key
         prompt         = query + ':\n\n' + f'{corpus}\n'
         prompt         = prompt[:char_limit]
         analyze        = query_chatgpt(prompt)
         print('Number of Characters: ' + str(len(prompt)))
         return analyze
 
     # Function: Ask chatGPT about Similarity Analysis 
     def ask_chatgpt_sim(self, char_limit = 4097, api_key = 'your_api_key_here', query = 'give me insights about the following information', model = 'text-davinci-003', max_tokens = 2000, n = 1, temperature = 0.8):
         def query_chatgpt(prompt, model = model, max_tokens = max_tokens, n = n, temperature = temperature):
-            response = openai.Completion.create(
-                                                engine      = model,
-                                                prompt      = prompt,
-                                                max_tokens  = max_tokens,
-                                                n           = n,
-                                                stop        = None,
-                                                temperature = temperature
-                                                )
-            return response.choices[0].text.strip()
+            try: 
+                response = openai.ChatCompletion.create(
+                                                        model      = model,
+                                                        messages   = [{'role': 'user', 'content': prompt}],
+                                                        max_tokens = max_tokens
+                                                        )
+                response = response['choices'][0]['message']['content']
+            except:
+                response = openai.Completion.create(
+                                                    engine      = model,
+                                                    prompt      = prompt,
+                                                    max_tokens  = max_tokens,
+                                                    n           = n,
+                                                    stop        = None,
+                                                    temperature = temperature
+                                                    )
+                response = response.choices[0].text.strip()
+            return response
         corpus         = self.ask_gpt_sim.to_string(index = False)
         openai.api_key = api_key
         prompt         = query + ':\n\n' + f'{corpus}\n'
         prompt         = prompt[:char_limit]
         analyze        = query_chatgpt(prompt)
         print('Number of Characters: ' + str(len(prompt)))
         return analyze
 
     # Function: Ask chatGPT about Wordcloud 
     def ask_chatgpt_wordcloud(self, char_limit = 4097, api_key = 'your_api_key_here', query = 'give me insights about the following information', model = 'text-davinci-003', max_tokens = 2000, n = 1, temperature = 0.8):
         def query_chatgpt(prompt, model = model, max_tokens = max_tokens, n = n, temperature = temperature):
-            response = openai.Completion.create(
-                                                engine      = model,
-                                                prompt      = prompt,
-                                                max_tokens  = max_tokens,
-                                                n           = n,
-                                                stop        = None,
-                                                temperature = temperature
-                                                )
-            return response.choices[0].text.strip()
+            try: 
+                response = openai.ChatCompletion.create(
+                                                        model      = model,
+                                                        messages   = [{'role': 'user', 'content': prompt}],
+                                                        max_tokens = max_tokens
+                                                        )
+                response = response['choices'][0]['message']['content']
+            except:
+                response = openai.Completion.create(
+                                                    engine      = model,
+                                                    prompt      = prompt,
+                                                    max_tokens  = max_tokens,
+                                                    n           = n,
+                                                    stop        = None,
+                                                    temperature = temperature
+                                                    )
+                response = response.choices[0].text.strip()
+            return response
         corpus         = pd.DataFrame.from_dict(self.ask_gpt_wd, orient = 'index', columns = ['Frequency'])    
         corpus         = corpus.reset_index().rename(columns = {'index': 'Word'})
         corpus         = corpus.to_string(index = False)
         lines          = corpus.split('\n')
         corpus         = '\n'.join(' '.join(line.split()) for line in lines)
         openai.api_key = api_key
         prompt         = query + ':\n\n' + f'{corpus}\n'
```

### Comparing `pyBibX-3.1.9/pyBibX/base/stws/Stopwords-Arabic.txt` & `pyBibX-3.2.0/pyBibX/base/stws/Stopwords-Arabic.txt`

 * *Files identical despite different names*

### Comparing `pyBibX-3.1.9/pyBibX/base/stws/Stopwords-Bengali.txt` & `pyBibX-3.2.0/pyBibX/base/stws/Stopwords-Bengali.txt`

 * *Files identical despite different names*

### Comparing `pyBibX-3.1.9/pyBibX/base/stws/Stopwords-Bulgarian.txt` & `pyBibX-3.2.0/pyBibX/base/stws/Stopwords-Bulgarian.txt`

 * *Files identical despite different names*

### Comparing `pyBibX-3.1.9/pyBibX/base/stws/Stopwords-Chinese.txt` & `pyBibX-3.2.0/pyBibX/base/stws/Stopwords-Chinese.txt`

 * *Files identical despite different names*

### Comparing `pyBibX-3.1.9/pyBibX/base/stws/Stopwords-Czech.txt` & `pyBibX-3.2.0/pyBibX/base/stws/Stopwords-Czech.txt`

 * *Files identical despite different names*

### Comparing `pyBibX-3.1.9/pyBibX/base/stws/Stopwords-English.txt` & `pyBibX-3.2.0/pyBibX/base/stws/Stopwords-English.txt`

 * *Files identical despite different names*

### Comparing `pyBibX-3.1.9/pyBibX/base/stws/Stopwords-Finnish.txt` & `pyBibX-3.2.0/pyBibX/base/stws/Stopwords-Finnish.txt`

 * *Files identical despite different names*

### Comparing `pyBibX-3.1.9/pyBibX/base/stws/Stopwords-French.txt` & `pyBibX-3.2.0/pyBibX/base/stws/Stopwords-French.txt`

 * *Files identical despite different names*

### Comparing `pyBibX-3.1.9/pyBibX/base/stws/Stopwords-German.txt` & `pyBibX-3.2.0/pyBibX/base/stws/Stopwords-German.txt`

 * *Files identical despite different names*

### Comparing `pyBibX-3.1.9/pyBibX/base/stws/Stopwords-Greek.txt` & `pyBibX-3.2.0/pyBibX/base/stws/Stopwords-Greek.txt`

 * *Files identical despite different names*

### Comparing `pyBibX-3.1.9/pyBibX/base/stws/Stopwords-Hebrew.txt` & `pyBibX-3.2.0/pyBibX/base/stws/Stopwords-Hebrew.txt`

 * *Files identical despite different names*

### Comparing `pyBibX-3.1.9/pyBibX/base/stws/Stopwords-Hindi.txt` & `pyBibX-3.2.0/pyBibX/base/stws/Stopwords-Hindi.txt`

 * *Files identical despite different names*

### Comparing `pyBibX-3.1.9/pyBibX/base/stws/Stopwords-Hungarian.txt` & `pyBibX-3.2.0/pyBibX/base/stws/Stopwords-Hungarian.txt`

 * *Files identical despite different names*

### Comparing `pyBibX-3.1.9/pyBibX/base/stws/Stopwords-Italian.txt` & `pyBibX-3.2.0/pyBibX/base/stws/Stopwords-Italian.txt`

 * *Files identical despite different names*

### Comparing `pyBibX-3.1.9/pyBibX/base/stws/Stopwords-Japanese.txt` & `pyBibX-3.2.0/pyBibX/base/stws/Stopwords-Japanese.txt`

 * *Files identical despite different names*

### Comparing `pyBibX-3.1.9/pyBibX/base/stws/Stopwords-Korean.txt` & `pyBibX-3.2.0/pyBibX/base/stws/Stopwords-Korean.txt`

 * *Files identical despite different names*

### Comparing `pyBibX-3.1.9/pyBibX/base/stws/Stopwords-Marathi.txt` & `pyBibX-3.2.0/pyBibX/base/stws/Stopwords-Marathi.txt`

 * *Files identical despite different names*

### Comparing `pyBibX-3.1.9/pyBibX/base/stws/Stopwords-Persian.txt` & `pyBibX-3.2.0/pyBibX/base/stws/Stopwords-Persian.txt`

 * *Files identical despite different names*

### Comparing `pyBibX-3.1.9/pyBibX/base/stws/Stopwords-Polish.txt` & `pyBibX-3.2.0/pyBibX/base/stws/Stopwords-Polish.txt`

 * *Files identical despite different names*

### Comparing `pyBibX-3.1.9/pyBibX/base/stws/Stopwords-Portuguese-br.txt` & `pyBibX-3.2.0/pyBibX/base/stws/Stopwords-Portuguese-br.txt`

 * *Files identical despite different names*

### Comparing `pyBibX-3.1.9/pyBibX/base/stws/Stopwords-Romanian.txt` & `pyBibX-3.2.0/pyBibX/base/stws/Stopwords-Romanian.txt`

 * *Files identical despite different names*

### Comparing `pyBibX-3.1.9/pyBibX/base/stws/Stopwords-Russian.txt` & `pyBibX-3.2.0/pyBibX/base/stws/Stopwords-Russian.txt`

 * *Files identical despite different names*

### Comparing `pyBibX-3.1.9/pyBibX/base/stws/Stopwords-Slovak.txt` & `pyBibX-3.2.0/pyBibX/base/stws/Stopwords-Slovak.txt`

 * *Files identical despite different names*

### Comparing `pyBibX-3.1.9/pyBibX/base/stws/Stopwords-Spanish.txt` & `pyBibX-3.2.0/pyBibX/base/stws/Stopwords-Spanish.txt`

 * *Files identical despite different names*

### Comparing `pyBibX-3.1.9/pyBibX/base/stws/Stopwords-Swedish.txt` & `pyBibX-3.2.0/pyBibX/base/stws/Stopwords-Swedish.txt`

 * *Files identical despite different names*

### Comparing `pyBibX-3.1.9/pyBibX/base/stws/Stopwords-Thai.txt` & `pyBibX-3.2.0/pyBibX/base/stws/Stopwords-Thai.txt`

 * *Files identical despite different names*

### Comparing `pyBibX-3.1.9/pyBibX/base/stws/Stopwords-Ukrainian.txt` & `pyBibX-3.2.0/pyBibX/base/stws/Stopwords-Ukrainian.txt`

 * *Files identical despite different names*

### Comparing `pyBibX-3.1.9/pyBibX.egg-info/PKG-INFO` & `pyBibX-3.2.0/pyBibX.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyBibX
-Version: 3.1.9
+Version: 3.2.0
 Summary: A Bibliometric and Scientometric Library Powered with Artificial Intelligence Tools
 Home-page: https://github.com/Valdecy/pyBibX
 Author: Valdecy Pereira
 Author-email: valdecy.pereira@gmail.com
 License: GNU
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `pyBibX-3.1.9/pyBibX.egg-info/SOURCES.txt` & `pyBibX-3.2.0/pyBibX.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pyBibX-3.1.9/setup.py` & `pyBibX-3.2.0/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from pathlib import Path
 
 this_directory = Path(__file__).parent
 long_description = (this_directory / 'README.md').read_text()
 
 setup(
     name='pyBibX',
-    version='3.1.9',
+    version='3.2.0',
     license='GNU',
     author='Valdecy Pereira',
     author_email='valdecy.pereira@gmail.com',
     url='https://github.com/Valdecy/pyBibX',
     packages=find_packages(),
     include_package_data=True,
     install_requires=[
```

