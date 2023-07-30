# Comparing `tmp/nadia-proof-0.1.7.tar.gz` & `tmp/nadia-proof-0.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nadia-proof-0.1.7.tar", last modified: Mon Jul 24 18:42:53 2023, max compression
+gzip compressed data, was "nadia-proof-0.1.8.tar", last modified: Sun Jul 30 14:27:05 2023, max compression
```

## Comparing `nadia-proof-0.1.7.tar` & `nadia-proof-0.1.8.tar`

### file list

```diff
@@ -1,20 +1,21 @@
-drwxrwxrwx   0        0        0        0 2023-07-24 18:42:53.051271 nadia-proof-0.1.7/
--rw-rw-rw-   0        0        0     4898 2023-07-24 18:42:53.050264 nadia-proof-0.1.7/PKG-INFO
--rw-rw-rw-   0        0        0     4311 2023-03-08 00:14:38.000000 nadia-proof-0.1.7/README.md
--rw-rw-rw-   0        0        0     1094 2022-11-18 21:07:18.000000 nadia-proof-0.1.7/license.txt
--rw-rw-rw-   0        0        0       42 2023-07-24 18:42:53.052262 nadia-proof-0.1.7/setup.cfg
--rw-rw-rw-   0        0        0      986 2023-07-24 18:42:46.000000 nadia-proof-0.1.7/setup.py
-drwxrwxrwx   0        0        0        0 2023-07-24 18:42:52.990261 nadia-proof-0.1.7/src/
-drwxrwxrwx   0        0        0        0 2023-07-24 18:42:53.017261 nadia-proof-0.1.7/src/nadia/
--rw-rw-rw-   0        0        0        0 2023-05-01 15:14:32.000000 nadia-proof-0.1.7/src/nadia/__init__.py
--rw-rw-rw-   0        0        0     2114 2022-12-23 14:27:18.000000 nadia-proof-0.1.7/src/nadia/example_theorems.py
--rw-rw-rw-   0        0        0     1498 2023-05-01 14:59:06.000000 nadia-proof-0.1.7/src/nadia/nadia_pt.py
--rw-rw-rw-   0        0        0      301 2023-05-01 14:57:00.000000 nadia-proof-0.1.7/src/nadia/nadia_pt_basic_usage.py
--rw-rw-rw-   0        0        0   121095 2023-07-24 18:30:48.000000 nadia-proof-0.1.7/src/nadia/nadia_pt_fo.py
--rw-rw-rw-   0        0        0    18419 2023-07-24 18:30:48.000000 nadia-proof-0.1.7/src/nadia/nadia_pt_gui.py
-drwxrwxrwx   0        0        0        0 2023-07-24 18:42:53.046266 nadia-proof-0.1.7/src/nadia_proof.egg-info/
--rw-rw-rw-   0        0        0     4898 2023-07-24 18:42:52.000000 nadia-proof-0.1.7/src/nadia_proof.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      383 2023-07-24 18:42:52.000000 nadia-proof-0.1.7/src/nadia_proof.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-24 18:42:52.000000 nadia-proof-0.1.7/src/nadia_proof.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       16 2023-07-24 18:42:52.000000 nadia-proof-0.1.7/src/nadia_proof.egg-info/requires.txt
--rw-rw-rw-   0        0        0        6 2023-07-24 18:42:52.000000 nadia-proof-0.1.7/src/nadia_proof.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-30 14:27:05.586721 nadia-proof-0.1.8/
+-rw-rw-rw-   0        0        0     4929 2023-07-30 14:27:05.585721 nadia-proof-0.1.8/PKG-INFO
+-rw-rw-rw-   0        0        0     4342 2023-07-30 14:23:15.000000 nadia-proof-0.1.8/README.md
+-rw-rw-rw-   0        0        0     1094 2022-11-18 21:07:18.000000 nadia-proof-0.1.8/license.txt
+-rw-rw-rw-   0        0        0       42 2023-07-30 14:27:05.587722 nadia-proof-0.1.8/setup.cfg
+-rw-rw-rw-   0        0        0      986 2023-07-30 14:20:40.000000 nadia-proof-0.1.8/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-30 14:27:05.493722 nadia-proof-0.1.8/src/
+drwxrwxrwx   0        0        0        0 2023-07-30 14:27:05.556719 nadia-proof-0.1.8/src/nadia/
+-rw-rw-rw-   0        0        0        0 2023-05-01 15:14:32.000000 nadia-proof-0.1.8/src/nadia/__init__.py
+-rw-rw-rw-   0        0        0     1607 2023-07-30 14:20:05.000000 nadia-proof-0.1.8/src/nadia/__main__.py
+-rw-rw-rw-   0        0        0     2114 2022-12-23 14:27:18.000000 nadia-proof-0.1.8/src/nadia/example_theorems.py
+-rw-rw-rw-   0        0        0     1498 2023-05-01 14:59:06.000000 nadia-proof-0.1.8/src/nadia/nadia_pt.py
+-rw-rw-rw-   0        0        0      301 2023-05-01 14:57:00.000000 nadia-proof-0.1.8/src/nadia/nadia_pt_basic_usage.py
+-rw-rw-rw-   0        0        0   122158 2023-07-29 13:23:23.000000 nadia-proof-0.1.8/src/nadia/nadia_pt_fo.py
+-rw-rw-rw-   0        0        0    18419 2023-07-24 18:30:48.000000 nadia-proof-0.1.8/src/nadia/nadia_pt_gui.py
+drwxrwxrwx   0        0        0        0 2023-07-30 14:27:05.583720 nadia-proof-0.1.8/src/nadia_proof.egg-info/
+-rw-rw-rw-   0        0        0     4929 2023-07-30 14:27:05.000000 nadia-proof-0.1.8/src/nadia_proof.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      405 2023-07-30 14:27:05.000000 nadia-proof-0.1.8/src/nadia_proof.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-30 14:27:05.000000 nadia-proof-0.1.8/src/nadia_proof.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       16 2023-07-30 14:27:05.000000 nadia-proof-0.1.8/src/nadia_proof.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        6 2023-07-30 14:27:05.000000 nadia-proof-0.1.8/src/nadia_proof.egg-info/top_level.txt
```

### Comparing `nadia-proof-0.1.7/PKG-INFO` & `nadia-proof-0.1.8/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nadia-proof
-Version: 0.1.7
+Version: 0.1.8
 Summary: NADIA is a proof assistant for teaching natural deduction to computer science students. NADIA allows students to write their proofs and automatically checks whether the proofs are correct and, if not, displays any errors found.
 Home-page: https://github.com/daviromero/nadia
 Author: Davi Romero de Vasconcelos
 Author-email: daviromero@ufc.br
 License: MIT
 Keywords: Natural Deduction,Teaching Logic,Educational Software
 Platform: UNKNOWN
@@ -35,21 +35,23 @@
 - The justifications for the premises  use the reserved word `pre`.
 
 | Symbol |  $\lnot$ | $\land$ | $\lor$ | $\rightarrow$ | $\forall x$ | $\exists x$ | $\bot$ | box | $\vdash$ |
 | :---:  |  :---:  | :---: | :---:  | :---:  | :---:  | :---:  | :---:  | :---:  | :---: |
 | LaTeX  |  $\backslash\textrm{lnot}$ | $\backslash\textrm{land}$ | $\backslash\textrm{lor}$ | $\backslash\textrm{rightarrow}$ | $\backslash\textrm{forall x}$ | $\backslash\textrm{exists x}$ | $\backslash\textrm{bot}$ | $[.~]$ | $\backslash\textrm{vdash}$ |
 | NADIA |  ~  | \& | $\mid$ | -> | Ax | Ex | @  | { } | \|- |
 
-![](https://github.com/daviromero/nadia/blob/main/NADIA-EXAMPLE.png)
+![](https://raw.githubusercontent.com/daviromero/nadia/main/NADIA-EXAMPLE.png)
 
 ## License
 NADIA is available by [**MIT License**](https://github.com/daviromero/nadia/blob/main/license.txt).
 
 ## Requirements:
-- You must install [rply 0.7.8 package](https://pypi.org/project/rply/)
+You must install 
+- [rply 0.7.8 package](https://pypi.org/project/rply/)
+- ipywidgets
 
 ## Install
 
 To install NADIA from Github, run the following command:
 ```bash
 pip install git+https://github.com/daviromero/nadia.git
 ```
@@ -58,15 +60,15 @@
 ```bash
 pip install nadia-proof
 ```
 
 ## NADIA
 You can run NADIA with the command line: 
 ```bash
-python nadia_pt.py [-i input_file] [-o output_file]
+python -m nadia -i [input_proof_file] [-t input_theorem]
 ```
 ## NADIA in Voila
 You can run NADIA in Jupyter Nootebook or in a [VoilÃ ](https://voila.readthedocs.io/) 
 ```bash
 voila nadia_pt.ipynb
 ```
 ## NADIA in your code
```

### Comparing `nadia-proof-0.1.7/README.md` & `nadia-proof-0.1.8/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -22,21 +22,23 @@
 - The justifications for the premises  use the reserved word `pre`.
 
 | Symbol |  $\lnot$ | $\land$ | $\lor$ | $\rightarrow$ | $\forall x$ | $\exists x$ | $\bot$ | box | $\vdash$ |
 | :---:  |  :---:  | :---: | :---:  | :---:  | :---:  | :---:  | :---:  | :---:  | :---: |
 | LaTeX  |  $\backslash\textrm{lnot}$ | $\backslash\textrm{land}$ | $\backslash\textrm{lor}$ | $\backslash\textrm{rightarrow}$ | $\backslash\textrm{forall x}$ | $\backslash\textrm{exists x}$ | $\backslash\textrm{bot}$ | $[.~]$ | $\backslash\textrm{vdash}$ |
 | NADIA |  ~  | \& | $\mid$ | -> | Ax | Ex | @  | { } | \|- |
 
-![](https://github.com/daviromero/nadia/blob/main/NADIA-EXAMPLE.png)
+![](https://raw.githubusercontent.com/daviromero/nadia/main/NADIA-EXAMPLE.png)
 
 ## License
 NADIA is available by [**MIT License**](https://github.com/daviromero/nadia/blob/main/license.txt).
 
 ## Requirements:
-- You must install [rply 0.7.8 package](https://pypi.org/project/rply/)
+You must install 
+- [rply 0.7.8 package](https://pypi.org/project/rply/)
+- ipywidgets
 
 ## Install
 
 To install NADIA from Github, run the following command:
 ```bash
 pip install git+https://github.com/daviromero/nadia.git
 ```
@@ -45,15 +47,15 @@
 ```bash
 pip install nadia-proof
 ```
 
 ## NADIA
 You can run NADIA with the command line: 
 ```bash
-python nadia_pt.py [-i input_file] [-o output_file]
+python -m nadia -i [input_proof_file] [-t input_theorem]
 ```
 ## NADIA in Voila
 You can run NADIA in Jupyter Nootebook or in a [Voilà](https://voila.readthedocs.io/) 
 ```bash
 voila nadia_pt.ipynb
 ```
 ## NADIA in your code
```

### Comparing `nadia-proof-0.1.7/license.txt` & `nadia-proof-0.1.8/license.txt`

 * *Files identical despite different names*

### Comparing `nadia-proof-0.1.7/setup.py` & `nadia-proof-0.1.8/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 # read the contents of your README file
 from pathlib import Path
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text()
 
 setup(
     name='nadia-proof',
-    version='0.1.7',
+    version='0.1.8',
     license='MIT',
     author="Davi Romero de Vasconcelos",
     author_email='daviromero@ufc.br',
     packages=find_packages('src'),
     package_dir={'': 'src'},
     url='https://github.com/daviromero/nadia',
     description='''NADIA is a proof assistant for teaching natural deduction to computer science students. NADIA allows students to write their proofs and automatically checks whether the proofs are correct and, if not, displays any errors found.''',
```

### Comparing `nadia-proof-0.1.7/src/nadia/example_theorems.py` & `nadia-proof-0.1.8/src/nadia/example_theorems.py`

 * *Files identical despite different names*

### Comparing `nadia-proof-0.1.7/src/nadia/nadia_pt.py` & `nadia-proof-0.1.8/src/nadia/nadia_pt.py`

 * *Files identical despite different names*

### Comparing `nadia-proof-0.1.7/src/nadia/nadia_pt_fo.py` & `nadia-proof-0.1.8/src/nadia/nadia_pt_fo.py`

 * *Files 2% similar despite different names*

```diff
@@ -697,35 +697,35 @@
         for key, scope in self.symbol_table.items():
             if key != 'scope_0':
                 if(scope['end_line'] == line):
                     return (line - int(scope['start_line']))
         return 0
 
 ## dados_json.py
-import json
+#import json
 
 class natural_deduction_return:
     def __init__(self):
         self.premisses = []
         self.conclusion = None
         self.gentzen = ""
         self.fitch = ""
         self.errors = []
 
     def add_error(self, error):
         self.errors.append(error)
 
-    def to_json(self):
-        result = {
-            'gentzen': self.gentzen,
-            'fitch': self.fitch,
-            'errors': self.errors
-        }
-        with open("result.json", "w", encoding='utf8') as f:
-            f.write(json.dumps(result, sort_keys=True, indent=3, ensure_ascii=False))
+ #   def to_json(self):
+ #       result = {
+ #           'gentzen': self.gentzen,
+ #           'fitch': self.fitch,
+ #           'errors': self.errors
+ #       }
+#        with open("result.json", "w", encoding='utf8') as f:
+#            f.write(json.dumps(result, sort_keys=True, indent=3, ensure_ascii=False))
 
 ## File constants.py
 class constants:
   REFERENCED_FORMULE_NONE = 0
   INVALID_RESULT = 1 # Conclusão inválida da regra
   UNEXPECT_RESULT = 2 # Escolha errada de regra
   SUCCESS = 3
@@ -1443,15 +1443,15 @@
 import sys
 import copy
 
 deduction_result = natural_deduction_return()
 
 def value_error_handle(exctype, value, tb):
     deduction_result.add_error(str(value))
-    deduction_result.to_json()
+#    deduction_result.to_json()
 
 sys.excepthook = value_error_handle
 
 class ParserNadia():
     def __init__(self, state):
         self.state = state
         self.pg = ParserGenerator(
@@ -2228,35 +2228,54 @@
     def toLatex(premisses,conclusion,parentheses=False):
       if (premisses==[]):
         return '\\vdash '+conclusion.toLatex(parentheses=parentheses)
       else:
         return ", ".join(f.toLatex(parentheses=parentheses) for f in premisses) +' \\vdash '+conclusion.toLatex(parentheses=parentheses)
 
 
-def check_proof(text_input, show_fitch=True, show_gentzen=True):
+def check_proof(input_proof, input_theorem=None, display_theorem=True, display_fitch=True, display_gentzen=True):
     try:
-        result = ParserNadia.getProof(text_input)
+        result = ParserNadia.getProof(input_proof)
         r = ''
+
         if(result.errors==[]):
-            r += "A demonstração está correta."
-            if show_fitch:
+            s_theorem = ParserNadia.toString(result.premisses, result.conclusion)
+            if input_theorem!=None: 
+                premisses, conclusion = ParserTheorem.getTheorem(input_theorem)
+                if conclusion == None:
+                    return f'{input_theorem} não é um teorema válido!'
+
+                set_premisses = set([p.toString() for p in premisses])
+                set_premisses_result = set([p.toString() for p in result.premisses])
+                if(conclusion==result.conclusion and set_premisses==set_premisses_result):
+                    r += "A demonstração está correta."
+                    if display_theorem:
+                       r += "\n"+s_theorem
+                else:
+                    r += f"Sua demostração de {s_theorem} é válida, mas é diferente da demonstração solicitada {input_theorem}"
+            else:
+                r += "A demonstração está correta."
+                if display_theorem:
+                    r += "\n"+s_theorem
+            if display_fitch:
                 r += "\n\nCódigo da demonstração no estilo Fitch em Latex:\n"
                 r += str(result.fitch)
-            if show_gentzen:
+            if display_gentzen:
                 r += "\n\nCódigo da demonstração no estilo Gentzen em Latex:\n"
                 r += str(result.gentzen)
         else:
             r += "Os seguintes erros foram encontrados:\n\n"
             for error in result.errors:
                 r += str(error)
         return r
     except ValueError:
         s = traceback.format_exc()
         result = (s.split("@@"))[-1]
         r = "Os seguintes erros foram encontrados:\n\n"
+        r += result
         return r
     else:
         pass
 
 
 
 # PARSER DE UM TEOREMA
```

### Comparing `nadia-proof-0.1.7/src/nadia/nadia_pt_gui.py` & `nadia-proof-0.1.8/src/nadia/nadia_pt_gui.py`

 * *Files identical despite different names*

### Comparing `nadia-proof-0.1.7/src/nadia_proof.egg-info/PKG-INFO` & `nadia-proof-0.1.8/src/nadia_proof.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nadia-proof
-Version: 0.1.7
+Version: 0.1.8
 Summary: NADIA is a proof assistant for teaching natural deduction to computer science students. NADIA allows students to write their proofs and automatically checks whether the proofs are correct and, if not, displays any errors found.
 Home-page: https://github.com/daviromero/nadia
 Author: Davi Romero de Vasconcelos
 Author-email: daviromero@ufc.br
 License: MIT
 Keywords: Natural Deduction,Teaching Logic,Educational Software
 Platform: UNKNOWN
@@ -35,21 +35,23 @@
 - The justifications for the premises  use the reserved word `pre`.
 
 | Symbol |  $\lnot$ | $\land$ | $\lor$ | $\rightarrow$ | $\forall x$ | $\exists x$ | $\bot$ | box | $\vdash$ |
 | :---:  |  :---:  | :---: | :---:  | :---:  | :---:  | :---:  | :---:  | :---:  | :---: |
 | LaTeX  |  $\backslash\textrm{lnot}$ | $\backslash\textrm{land}$ | $\backslash\textrm{lor}$ | $\backslash\textrm{rightarrow}$ | $\backslash\textrm{forall x}$ | $\backslash\textrm{exists x}$ | $\backslash\textrm{bot}$ | $[.~]$ | $\backslash\textrm{vdash}$ |
 | NADIA |  ~  | \& | $\mid$ | -> | Ax | Ex | @  | { } | \|- |
 
-![](https://github.com/daviromero/nadia/blob/main/NADIA-EXAMPLE.png)
+![](https://raw.githubusercontent.com/daviromero/nadia/main/NADIA-EXAMPLE.png)
 
 ## License
 NADIA is available by [**MIT License**](https://github.com/daviromero/nadia/blob/main/license.txt).
 
 ## Requirements:
-- You must install [rply 0.7.8 package](https://pypi.org/project/rply/)
+You must install 
+- [rply 0.7.8 package](https://pypi.org/project/rply/)
+- ipywidgets
 
 ## Install
 
 To install NADIA from Github, run the following command:
 ```bash
 pip install git+https://github.com/daviromero/nadia.git
 ```
@@ -58,15 +60,15 @@
 ```bash
 pip install nadia-proof
 ```
 
 ## NADIA
 You can run NADIA with the command line: 
 ```bash
-python nadia_pt.py [-i input_file] [-o output_file]
+python -m nadia -i [input_proof_file] [-t input_theorem]
 ```
 ## NADIA in Voila
 You can run NADIA in Jupyter Nootebook or in a [VoilÃ ](https://voila.readthedocs.io/) 
 ```bash
 voila nadia_pt.ipynb
 ```
 ## NADIA in your code
```

