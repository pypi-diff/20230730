# Comparing `tmp/anita-0.1.8.tar.gz` & `tmp/anita-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "anita-0.1.8.tar", last modified: Fri Dec 23 14:59:55 2022, max compression
+gzip compressed data, was "anita-0.1.9.tar", last modified: Wed Mar  8 00:02:15 2023, max compression
```

## Comparing `anita-0.1.8.tar` & `anita-0.1.9.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxrwxrwx   0        0        0        0 2022-12-23 14:59:55.895485 anita-0.1.8/
--rw-rw-rw-   0        0        0     5418 2022-12-23 14:59:55.893487 anita-0.1.8/PKG-INFO
--rw-rw-rw-   0        0        0     4835 2022-12-23 14:53:44.000000 anita-0.1.8/README.md
--rw-rw-rw-   0        0        0     1089 2022-12-23 14:18:21.000000 anita-0.1.8/license.txt
--rw-rw-rw-   0        0        0       42 2022-12-23 14:59:55.895485 anita-0.1.8/setup.cfg
--rw-rw-rw-   0        0        0      959 2022-12-23 14:54:02.000000 anita-0.1.8/setup.py
-drwxrwxrwx   0        0        0        0 2022-12-23 14:59:55.845493 anita-0.1.8/src/
-drwxrwxrwx   0        0        0        0 2022-12-23 14:59:55.875490 anita-0.1.8/src/anita/
--rw-rw-rw-   0        0        0        0 2022-12-23 14:17:48.000000 anita-0.1.8/src/anita/__init__.py
--rw-rw-rw-   0        0        0     2949 2022-12-23 14:23:23.000000 anita-0.1.8/src/anita/anita_en.py
--rw-rw-rw-   0        0        0      321 2022-12-23 14:20:24.000000 anita-0.1.8/src/anita/anita_en_basic_usage.py
--rw-rw-rw-   0        0        0   138958 2022-11-18 19:23:35.000000 anita-0.1.8/src/anita/anita_en_fo.py
--rw-rw-rw-   0        0        0    17912 2022-12-23 14:27:57.000000 anita-0.1.8/src/anita/anita_en_gui.py
--rw-rw-rw-   0        0        0     3056 2022-12-23 14:22:13.000000 anita-0.1.8/src/anita/anita_pt.py
--rw-rw-rw-   0        0        0      320 2022-12-23 14:21:23.000000 anita-0.1.8/src/anita/anita_pt_basic_usage.py
--rw-rw-rw-   0        0        0   141117 2022-11-18 19:23:35.000000 anita-0.1.8/src/anita/anita_pt_fo.py
--rw-rw-rw-   0        0        0    18056 2022-12-23 14:25:47.000000 anita-0.1.8/src/anita/anita_pt_gui.py
--rw-rw-rw-   0        0        0     2114 2022-12-23 14:27:18.000000 anita-0.1.8/src/anita/example_theorems.py
-drwxrwxrwx   0        0        0        0 2022-12-23 14:59:55.891486 anita-0.1.8/src/anita.egg-info/
--rw-rw-rw-   0        0        0     5418 2022-12-23 14:59:55.000000 anita-0.1.8/src/anita.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      460 2022-12-23 14:59:55.000000 anita-0.1.8/src/anita.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2022-12-23 14:59:55.000000 anita-0.1.8/src/anita.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        5 2022-12-23 14:59:55.000000 anita-0.1.8/src/anita.egg-info/requires.txt
--rw-rw-rw-   0        0        0        6 2022-12-23 14:59:55.000000 anita-0.1.8/src/anita.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-03-08 00:02:15.886428 anita-0.1.9/
+-rw-rw-rw-   0        0        0     5491 2023-03-08 00:02:15.886119 anita-0.1.9/PKG-INFO
+-rw-rw-rw-   0        0        0     4908 2022-12-23 17:49:15.000000 anita-0.1.9/README.md
+-rw-rw-rw-   0        0        0     1089 2022-12-23 14:18:21.000000 anita-0.1.9/license.txt
+-rw-rw-rw-   0        0        0       42 2023-03-08 00:02:15.887184 anita-0.1.9/setup.cfg
+-rw-rw-rw-   0        0        0      980 2023-03-07 23:59:02.000000 anita-0.1.9/setup.py
+drwxrwxrwx   0        0        0        0 2023-03-08 00:02:15.817123 anita-0.1.9/src/
+drwxrwxrwx   0        0        0        0 2023-03-08 00:02:15.847123 anita-0.1.9/src/anita/
+-rw-rw-rw-   0        0        0        0 2022-12-23 14:17:48.000000 anita-0.1.9/src/anita/__init__.py
+-rw-rw-rw-   0        0        0     2955 2022-12-23 18:26:19.000000 anita-0.1.9/src/anita/anita_en.py
+-rw-rw-rw-   0        0        0      321 2022-12-23 14:20:24.000000 anita-0.1.9/src/anita/anita_en_basic_usage.py
+-rw-rw-rw-   0        0        0   138958 2022-11-18 19:23:35.000000 anita-0.1.9/src/anita/anita_en_fo.py
+-rw-rw-rw-   0        0        0    17463 2023-02-17 13:01:39.000000 anita-0.1.9/src/anita/anita_en_gui.py
+-rw-rw-rw-   0        0        0     3062 2022-12-23 18:27:12.000000 anita-0.1.9/src/anita/anita_pt.py
+-rw-rw-rw-   0        0        0      320 2022-12-23 14:21:23.000000 anita-0.1.9/src/anita/anita_pt_basic_usage.py
+-rw-rw-rw-   0        0        0   141117 2022-11-18 19:23:35.000000 anita-0.1.9/src/anita/anita_pt_fo.py
+-rw-rw-rw-   0        0        0    19007 2023-03-08 00:00:05.000000 anita-0.1.9/src/anita/anita_pt_gui.py
+-rw-rw-rw-   0        0        0     2114 2022-12-23 14:27:18.000000 anita-0.1.9/src/anita/example_theorems.py
+drwxrwxrwx   0        0        0        0 2023-03-08 00:02:15.884118 anita-0.1.9/src/anita.egg-info/
+-rw-rw-rw-   0        0        0     5491 2023-03-08 00:02:15.000000 anita-0.1.9/src/anita.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      460 2023-03-08 00:02:15.000000 anita-0.1.9/src/anita.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-03-08 00:02:15.000000 anita-0.1.9/src/anita.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       16 2023-03-08 00:02:15.000000 anita-0.1.9/src/anita.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        6 2023-03-08 00:02:15.000000 anita-0.1.9/src/anita.egg-info/top_level.txt
```

### Comparing `anita-0.1.8/PKG-INFO` & `anita-0.1.9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 Metadata-Version: 2.1
 Name: anita
-Version: 0.1.8
+Version: 0.1.9
 Summary: ANITA is a proof assistant for teaching analytic tableaux to computer science students. ANITA allows students to write their proofs and automatically checks whether the proofs are correct and, if not, displays any errors found.
 Home-page: https://github.com/daviromero/anita
 Author: Davi Romero de Vasconcelos
 Author-email: daviromero@ufc.br
 License: MIT
 Keywords: Analytic Tableaux,Teaching Logic,Educational Software
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
 License-File: license.txt
 
 # Analytic Tableau Proof Assistant (ANITA)
 
 The ANITA is a tool written in Python that can be used as a desktop application, or in a [web platform](https://sistemas.quixada.ufc.br/anita/en/). The main idea is that the students can write their proofs as similar as possible to what is available in the textbooks and to what the students would usually write on paper. ANITA allows the students to automatically check whether a proof in the analytic tableaux is valid. If the proof is not correct, ANITA will display the errors of the proof. So, the students may make mistakes and learn from the errors. The web interface is very easy-to-use and has: 
-- An area for editing the proof in plain text. The students should write a proof in the Fitch-style (see [AT Rules](AT-Rules.pdf)).
+- An area for editing the proof in plain text. The students should write a proof in Fitch-style (see [AT Rules](https://github.com/daviromero/anita/blob/main/AT-Rules.pdf)).
 - A message area to display whether the proof is valid, the countermodel, or the errors on the proof.
 - And the following links: 
   - Check, to check the correctness of the proof; 
   - Manual, to view a document with the inference rules and examples; 
   - LaTeX, to generate the LaTeX code of the trees from a valid proof. Use the `qtree` package in your LaTeX code; 
   - LaTeX in Overleaf, to open the proof source code directly in [Overleaf](http://overleaf.com/) that is a collaborative platform for editing LaTeX
 
@@ -37,27 +37,27 @@
 | :---:  |  :---:  | :---: | :---:  | :---:  | :---:  | :---:  | :---:  | :---:  | :---: |
 | LaTeX  |  $\backslash\textrm{lnot}$ | $\backslash\textrm{land}$ | $\backslash\textrm{lor}$ | $\backslash\textrm{rightarrow}$ | $\backslash\textrm{forall x}$ | $\backslash\textrm{exists x}$ | $\backslash\textrm{bot}$ | $[.~]$ | $\backslash\textrm{vdash}$ |
 | ANITA |  ~  | \& | $\mid$ | -> | Ax | Ex | @  | { } | \|- |
 
 ![](ANITA-EXAMPLE.png)
 
 ## License
-ANITA is available by a ![**MIT License**](license.txt).
+ANITA is available by [**MIT License**](https://github.com/daviromero/anita/blob/main/license.txt).
 
 ## Requirements:
-- You must install the [rply 0.7.8 package](https://pypi.org/project/rply/)
+- You must install [rply 0.7.8 package](https://pypi.org/project/rply/)
 
 ## Install
 
-To install ANITA from the Github, run the following command:
+To install ANITA from Github, run the following command:
 ```bash
 pip install git+https://github.com/daviromero/anita.git
 ```
 
-To install ANITA from the PyPi repository, run the following command:
+To install ANITA from PyPi repository, run the following command:
 ```bash
 pip install anita
 ```
 
 ## ANITA
 You can run ANITA with the command line: 
 ```bash
```

### Comparing `anita-0.1.8/README.md` & `anita-0.1.9/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # Analytic Tableau Proof Assistant (ANITA)
 
 The ANITA is a tool written in Python that can be used as a desktop application, or in a [web platform](https://sistemas.quixada.ufc.br/anita/en/). The main idea is that the students can write their proofs as similar as possible to what is available in the textbooks and to what the students would usually write on paper. ANITA allows the students to automatically check whether a proof in the analytic tableaux is valid. If the proof is not correct, ANITA will display the errors of the proof. So, the students may make mistakes and learn from the errors. The web interface is very easy-to-use and has: 
-- An area for editing the proof in plain text. The students should write a proof in the Fitch-style (see [AT Rules](AT-Rules.pdf)).
+- An area for editing the proof in plain text. The students should write a proof in Fitch-style (see [AT Rules](https://github.com/daviromero/anita/blob/main/AT-Rules.pdf)).
 - A message area to display whether the proof is valid, the countermodel, or the errors on the proof.
 - And the following links: 
   - Check, to check the correctness of the proof; 
   - Manual, to view a document with the inference rules and examples; 
   - LaTeX, to generate the LaTeX code of the trees from a valid proof. Use the `qtree` package in your LaTeX code; 
   - LaTeX in Overleaf, to open the proof source code directly in [Overleaf](http://overleaf.com/) that is a collaborative platform for editing LaTeX
 
@@ -24,27 +24,27 @@
 | :---:  |  :---:  | :---: | :---:  | :---:  | :---:  | :---:  | :---:  | :---:  | :---: |
 | LaTeX  |  $\backslash\textrm{lnot}$ | $\backslash\textrm{land}$ | $\backslash\textrm{lor}$ | $\backslash\textrm{rightarrow}$ | $\backslash\textrm{forall x}$ | $\backslash\textrm{exists x}$ | $\backslash\textrm{bot}$ | $[.~]$ | $\backslash\textrm{vdash}$ |
 | ANITA |  ~  | \& | $\mid$ | -> | Ax | Ex | @  | { } | \|- |
 
 ![](ANITA-EXAMPLE.png)
 
 ## License
-ANITA is available by a ![**MIT License**](license.txt).
+ANITA is available by [**MIT License**](https://github.com/daviromero/anita/blob/main/license.txt).
 
 ## Requirements:
-- You must install the [rply 0.7.8 package](https://pypi.org/project/rply/)
+- You must install [rply 0.7.8 package](https://pypi.org/project/rply/)
 
 ## Install
 
-To install ANITA from the Github, run the following command:
+To install ANITA from Github, run the following command:
 ```bash
 pip install git+https://github.com/daviromero/anita.git
 ```
 
-To install ANITA from the PyPi repository, run the following command:
+To install ANITA from PyPi repository, run the following command:
 ```bash
 pip install anita
 ```
 
 ## ANITA
 You can run ANITA with the command line: 
 ```bash
```

### Comparing `anita-0.1.8/license.txt` & `anita-0.1.9/license.txt`

 * *Files identical despite different names*

### Comparing `anita-0.1.8/setup.py` & `anita-0.1.9/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -3,23 +3,24 @@
 # read the contents of your README file
 from pathlib import Path
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text()
 
 setup(
     name='anita',
-    version='0.1.8',
+    version='0.1.9',
     license='MIT',
     author="Davi Romero de Vasconcelos",
     author_email='daviromero@ufc.br',
     packages=find_packages('src'),
     package_dir={'': 'src'},
     url='https://github.com/daviromero/anita',
     description='''ANITA is a proof assistant for teaching analytic tableaux to computer science students. ANITA allows students to write their proofs and automatically checks whether the proofs are correct and, if not, displays any errors found.''',
     long_description=long_description,
     long_description_content_type='text/markdown',
     keywords='Analytic Tableaux, Teaching Logic, Educational Software', 
     install_requires=[
-          'rply',
+        'rply',
+        'ipywidgets',
       ],
 
 )
```

### Comparing `anita-0.1.8/src/anita/anita_en.py` & `anita-0.1.9/src/anita/anita_en.py`

 * *Files 11% similar despite different names*

```diff
@@ -2,16 +2,16 @@
 import argparse
 import traceback
 
 parser = argparse.ArgumentParser(description='Analytic Tableau Proof Assistant (ANITA).')
 parser.add_argument("-i", type=str,help="Input file with the proof in ANITA.")
 parser.add_argument("-o", type=str,help="Output file of result of the checking of the proof in ANITA.")
 args = parser.parse_args()
-fileName = 'example_anita.txt'
-fileSave = 'result_anita.txt'
+fileName = 'example_anita_en.txt'
+fileSave = 'result_anita_en.txt'
 if args.i is not None: fileName = args.i
 if args.o is not None: fileSave = args.o
 try:
     f = open(fileName, 'r')
     input_proof = f.read()
     result = anita.anita_en_fo.ParserAnita.getProof(input_proof)
     with open(fileSave, "w", encoding='utf8') as fs:
```

### Comparing `anita-0.1.8/src/anita/anita_en_fo.py` & `anita-0.1.9/src/anita/anita_en_fo.py`

 * *Files identical despite different names*

### Comparing `anita-0.1.8/src/anita/anita_en_gui.py` & `anita-0.1.9/src/anita/anita_en_gui.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import ipywidgets as widgets
-from IPython.display import display, Markdown
+from IPython.display import display, Markdown, HTML
 import traceback
-from anita.anita_pt_fo import ParserAnita, ParserTheorem, ParserFormula
+from anita.anita_en_fo import ParserAnita, ParserTheorem, ParserFormula
 
 def anita(input_string='', height_layout='300px'):
   layout = widgets.Layout(width='90%', height=height_layout)
   run = widgets.Button(description="Check")
   input = widgets.Textarea(
       value=input_string,
       placeholder='Enter you proof',
@@ -23,34 +23,34 @@
     output.clear_output()
     with output:
       try:
           result = ParserAnita.getProof(input.value)
           if(result.errors==[]):
             msg = []
             if(result.is_closed):
-              display(Markdown(rf'**<font color="blue">Congratulations! The proof of {result.theorem} is valid.</font>**'))
+              display(HTML(rf'<font color="blue">Congratulations! The proof of {result.theorem} is valid.</font>'))
             else:
               if result.saturared_branches!=[]:
-                display(Markdown(rf'**<font color="blue">Theorem {result.theorem} is not valid.</font>**'))              
+                display(HTML(rf'<font color="blue">Theorem {result.theorem} is not valid.</font>'))              
                 msg.append("Countermodels:")
                 for s_v in result.counter_examples:
                   msg.append(s_v)                  
               else:
-                display(Markdown(rf'**<font color="red">The proof of {result.theorem} is not complete.</font>**'))              
+                display(HTML(rf'<font color="red">The proof of {result.theorem} is not complete.</font>'))              
                 msg.append("The branches below are not saturated:")
                 for rules in result.open_branches:
                   msg.append("Branch:")
                   msg.append('<br>'.join([r.toString() for r in reversed(rules)]))
             if(cLatex.value):
               msg.append("LaTeX Code:")
               msg.append("%"+result.latex_theorem)
               msg.append(result.colored_latex)
             display(widgets.HTML('<br>'.join(msg)))       
           else:
-            display(Markdown(rf'**<font color="red">The proof is not correct:</font>**'))
+            display(HTML(rf'<font color="red">The proof is not correct:</font>'))
             for error in result.errors:
                 print(error)
       except ValueError:
           s = traceback.format_exc()
           result = (s.split("@@"))[-1]
           print (f'{result}')
       else:
@@ -59,62 +59,62 @@
 
 
 def anita_theorem(input_theorem, input_proof='', height_layout='300px',default_gentzen=False, default_fitch=False):
   layout = widgets.Layout(width='90%', height=height_layout)
   run = widgets.Button(description="Check")
   input = widgets.Textarea(
       value=input_proof,
-      placeholder='Digite sua demonstração:',
+      placeholder='Enter you proof:',
       description='',
       layout=layout
       )
   premisses, conclusion = ParserTheorem.getTheorem(input_theorem)
   if conclusion == None:
-    display(Markdown(rf'**<font color="red">{input_theorem} não é um teorema válido!</font>**'))
+    display(HTML(rf'<font color="red">Theorem {input_theorem} is not valid.</font>'))              
     return
-  cLatex = widgets.Checkbox(value=False, description='Exibir Latex')
+  cLatex = widgets.Checkbox(value=False, description='Display Latex')
   output = widgets.Output()
   wButtons = widgets.HBox([run, cLatex])
   
-  display(widgets.HTML(f'<h3>Digite a demonstração de {input_theorem} em Tableau Analítico:</h3>'), 
+  display(widgets.HTML(f'<h3Enter the proof of {input_theorem} in Analytic Tableau:</h3>'), 
           input, wButtons, output)
   
   def on_button_run_clicked(_):
     output.clear_output()
     with output:
       try:
           result = ParserAnita.getProof(input.value)
           if(result.errors==[]):
               set_premisses = set([p.toString() for p in premisses])
               set_premisses_result = set([p.toString() for p in result.premisses])
               if(conclusion==result.conclusion and set_premisses==set_premisses_result):
                 msg = []
                 if(result.is_closed):
-                  display(Markdown(rf'**<font color="blue">Parabéns! A demonstraçãoo de {result.theorem} está correta.</font>**'))
+                  display(HTML(rf'<font color="blue">Congratulations! The proof of {result.theorem} is valid.</font>'))
                 else:
                   if result.saturared_branches!=[]:
-                    display(Markdown(rf'**<font color="blue">O teorema {result.theorem} não é válido.</font>**'))              
-                    msg.append("São contra-exemplos:")
+                    display(HTML(rf'<font color="blue">Theorem {result.theorem} is not valid.</font>'))              
+                    msg.append("Countermodels:")
                     for s_v in result.counter_examples:
                       msg.append(s_v)                  
                   else:
-                    display(Markdown(rf'**<font color="red">A demonstração de {result.theorem} não está completa.</font>**'))              
-                    msg.append("Os ramos abaixo não estão saturados:")
+                    display(HTML(rf'<font color="red">The proof of {result.theorem} is not complete.</font>'))              
+                    msg.append("The branches below are not saturated:")
                     for rules in result.open_branches:
-                      msg.append("Ramo:")
+                      msg.append("Branch:")
                       msg.append('<br>'.join([r.toString() for r in reversed(rules)]))
                 if(cLatex.value):
-                  msg.append("Código Latex:")
+                  msg.append("Latex Code:")
                   msg.append("%"+result.latex_theorem)
                   msg.append(result.colored_latex)
                 display(widgets.HTML('<br>'.join(msg)))       
               else:
-                display(Markdown(rf'**<font color="red">Sua demostração de {result.theorem} é válida, mas é diferente da demonstração solicitada {input_theorem}!</font>**'))
+                display(HTML(rf'<font color="red">Proof of {result.theorem} is valid, but it is not {input_theorem}!</font>'))
           else:
-            display(Markdown(rf'**<font color="red">Sua demonstração contém os seguintes erros:</font>**'))
+            display(HTML(rf'<font color="red">The proof is not correct:</font>'))
             for error in result.errors:
                 print(error)
       except ValueError:
           s = traceback.format_exc()
           result = (s.split("@@"))[-1]
           print (f'{result}')
       else:
@@ -129,33 +129,33 @@
     value=None, 
     description='Answer:',
     disabled=False
 )
   output = widgets.Output()
   wButtons = widgets.HBox([run])
   
-  display(Markdown(rf'**The variable {input_var} is substitutable by the term {input_term} in the formula {input_formula}:**'))
+  display(HTML(rf'The variable {input_var} is substitutable by the term {input_term} in the formula {input_formula}:'))
   display(cResult, wButtons, output)
 
   def on_button_run_clicked(_):
     output.clear_output()
     with output:
       try:
           f = ParserFormula.getFormula(input_formula)
           if(f!=None):
             if (f.is_substitutable(input_var,input_term) and cResult.value=='Yes'):
-              display(Markdown(r'**<font color="blue">Congratulations you got the question right!</font>**'))              
-              display(Markdown(rf'The variable {input_var} **is substitutable** by the term {input_term} in the formula {input_formula}.'))              
+              display(HTML(r'<font color="blue">Congratulations you got the question right!</font>'))              
+              display(HTML(rf'The variable {input_var} is substitutable by the term {input_term} in the formula {input_formula}.'))              
             elif not f.is_substitutable(input_var,input_term) and cResult.value=='No':
-              display(Markdown(r'**<font color="blue">Congratulations you got the question right!</font>**'))              
-              display(Markdown(rf'The variable {input_var} **is not substitutable** by the term {input_term} in the formula {input_formula}.')) 
+              display(HTML(r'<font color="blue">Congratulations you got the question right!</font>'))              
+              display(HTML(rf'The variable {input_var} is not substitutable by the term {input_term} in the formula {input_formula}.')) 
             else:
-              display(Markdown(rf'**<font color="red">Unfortunately, you got the question wrong.</font>**'))
+              display(HTML(rf'<font color="red">Unfortunately, you got the question wrong.</font>'))
           else:
-            display(Markdown(r'**<font color="red">Formula definition is not correct, check if all rules are applied correctly. Remember that a formula is defined by the following BNF: F :== P | ~ P | Q & Q | P | Q | P -> Q | P <-> Q | (P), where P,Q (in capital letters) are atoms.</font>**'))
+            display(HTML(r'<font color="red">Formula definition is not correct, check if all rules are applied correctly. Remember that a formula is defined by the following BNF: F :== P | ~ P | Q & Q | P | Q | P -> Q | P <-> Q | (P), where P,Q (in capital letters) are atoms.</font>'))
       except ValueError:
           s = traceback.format_exc()
           result = (s.split("@@"))[-1]
           print (f'{result}')
       else:
           pass
   run.on_click(on_button_run_clicked)
@@ -168,31 +168,31 @@
       placeholder='Enter the variables separated by ; (semicolon)',
       description='',
       layout=layout
       )
   output = widgets.Output()
   wButtons = widgets.HBox([run])
   
-  display(Markdown(rf'**Enter the set of variables of the formula {input_formula}:**'))
-  display(Markdown(r'Each element of your set must be separated by ; (semicolon)'))
+  display(HTML(rf'Enter the set of variables of the formula {input_formula}:'))
+  display(HTML(r'Each element of your set must be separated by ; (semicolon)'))
   display(input, wButtons, output)
 
   def on_button_run_clicked(_):
     output.clear_output()
     with output:
       try:
           result = ParserFormula.getFormula(input_formula)
           variables = set([x.strip() for x in input.value.strip().split(";")])
           if(result!=None):
             if variables==result.all_variables():
-              display(Markdown(r'**<font color="blue">Congratulations, you got the question right!</font>**'))              
+              display(HTML(r'<font color="blue">Congratulations, you got the question right!</font>'))              
             else:
-              display(Markdown(rf'**<font color="red">Unfortunately, you got the question wrong.</font>**'))
+              display(HTML(rf'<font color="red">Unfortunately, you got the question wrong.</font>'))
           else:
-            display(Markdown(r'**<font color="red">Formula definition is not correct, check if all rules are applied correctly. Remember that a formula is defined by the following BNF: F :== P | ~ P | Q & Q | P | Q | P -> Q | P <-> Q | (P), where P,Q (in capital letters) are atoms.</font>**'))
+            display(HTML(r'<font color="red">Formula definition is not correct, check if all rules are applied correctly. Remember that a formula is defined by the following BNF: F :== P | ~ P | Q & Q | P | Q | P -> Q | P <-> Q | (P), where P,Q (in capital letters) are atoms.</font>'))
       except ValueError:
           s = traceback.format_exc()
           result = (s.split("@@"))[-1]
           print (f'{result}')
       else:
           pass
   run.on_click(on_button_run_clicked)
@@ -206,31 +206,31 @@
       placeholder='Enter the variables separated by ; (semicolon)',
       description='',
       layout=layout
       )
   output = widgets.Output()
   wButtons = widgets.HBox([run])
   
-  display(Markdown(rf'**Enter the set of the free variables of the formula {input_formula}:**'))
-  display(Markdown(r'Each element of your set must be separated by ; (semicolon)'))
+  display(HTML(rf'Enter the set of the free variables of the formula {input_formula}:'))
+  display(HTML(r'Each element of your set must be separated by ; (semicolon)'))
   display(input, wButtons, output)
 
   def on_button_run_clicked(_):
     output.clear_output()
     with output:
       try:
           result = ParserFormula.getFormula(input_formula)
           variables = set([x.strip() for x in input.value.strip().split(";")])
           if(result!=None):
             if variables==result.free_variables():
-              display(Markdown(r'**<font color="blue">Congratulations, you got the question right!</font>**'))              
+              display(HTML(r'<font color="blue">Congratulations, you got the question right!</font>'))              
             else:
-              display(Markdown(rf'**<font color="red">Unfortunately, you got the question wrong.</font>**'))
+              display(HTML(rf'<font color="red">Unfortunately, you got the question wrong.</font>'))
           else:
-            display(Markdown(r'**<font color="red">Formula definition is not correct, check if all rules are applied correctly. Remember that a formula is defined by the following BNF: F :== P | ~ P | Q & Q | P | Q | P -> Q | P <-> Q | (P), where P,Q (in capital letters) are atoms.</font>**'))
+            display(HTML(r'<font color="red">Formula definition is not correct, check if all rules are applied correctly. Remember that a formula is defined by the following BNF: F :== P | ~ P | Q & Q | P | Q | P -> Q | P <-> Q | (P), where P,Q (in capital letters) are atoms.</font>'))
       except ValueError:
           s = traceback.format_exc()
           result = (s.split("@@"))[-1]
           print (f'{result}')
       else:
           pass
   run.on_click(on_button_run_clicked)
@@ -243,31 +243,31 @@
       placeholder='Enter the variables separated by ; (semicolon)',
       description='',
       layout=layout
       )
   output = widgets.Output()
   wButtons = widgets.HBox([run])
   
-  display(Markdown(rf'**Enter the set of bound variables of the formula {input_formula}:**'))
-  display(Markdown(r'Each element of your set must be separated by ; (semicolon)'))
+  display(HTML(rf'Enter the set of bound variables of the formula {input_formula}:'))
+  display(HTML(r'Each element of your set must be separated by ; (semicolon)'))
   display(input, wButtons, output)
 
   def on_button_run_clicked(_):
     output.clear_output()
     with output:
       try:
           result = ParserFormula.getFormula(input_formula)
           variables = set([x.strip() for x in input.value.strip().split(";")])
           if(result!=None):
             if variables==result.bound_variables():
-              display(Markdown(r'**<font color="blue">Congratulations, you got the question right!</font>**'))              
+              display(HTML(r'<font color="blue">Congratulations, you got the question right!</font>'))              
             else:
-              display(Markdown(rf'**<font color="red">Unfortunately, you got the question wrong.</font>**'))
+              display(HTML(rf'<font color="red">Unfortunately, you got the question wrong.</font>'))
           else:
-            display(Markdown(r'**<font color="red">Formula definition is not correct, check if all rules are applied correctly. Remember that a formula is defined by the following BNF: F :== P | ~ P | Q & Q | P | Q | P -> Q | P <-> Q | (P), where P,Q (in capital letters) are atoms.</font>**'))
+            display(HTML(r'<font color="red">Formula definition is not correct, check if all rules are applied correctly. Remember that a formula is defined by the following BNF: F :== P | ~ P | Q & Q | P | Q | P -> Q | P <-> Q | (P), where P,Q (in capital letters) are atoms.</font>'))
       except ValueError:
           s = traceback.format_exc()
           result = (s.split("@@"))[-1]
           print (f'{result}')
       else:
           pass
   run.on_click(on_button_run_clicked)
@@ -282,35 +282,35 @@
       layout=layout
       )
   cParentheses = widgets.Checkbox(value=False, description='Display Formula with Parentheses')
   cLatex = widgets.Checkbox(value=False, description='Display Formula in Latex')
   output = widgets.Output()
   wButtons = widgets.HBox([run, cParentheses, cLatex])
   
-  display(Markdown(rf'**Enter the formula that results from substitution the variable {input_var} with the term {input_term} in the formula {input_formula}:**'))
+  display(HTML(rf'Enter the formula that results from substitution the variable {input_var} with the term {input_term} in the formula {input_formula}:'))
   display(input, wButtons, output)
 
   def on_button_run_clicked(_):
     output.clear_output()
     with output:
       try:
           f = ParserFormula.getFormula(input_formula)
           result = ParserFormula.getFormula(input.value)
           if(result!=None):
             if result==f.substitution(input_var,input_term):
-              display(Markdown(r'**<font color="blue">Congratulations this is the correct substitution:</font>**'))              
+              display(HTML(r'<font color="blue">Congratulations this is the correct substitution:</font>'))              
               if(cLatex.value):
                 s = result.toLatex(parentheses=cParentheses.value)
                 display(Markdown(rf'${s}$'))
               else:
-                display(Markdown(rf'{result.toString(parentheses=cParentheses.value)}'))
+                display(HTML(rf'{result.toString(parentheses=cParentheses.value)}'))
             else:
-              display(Markdown(rf'**<font color="red">The formula {result.toString()} is not the result of substitution {input_var} with {input_term} in the formula {input_formula}.</font>**'))
+              display(HTML(rf'<font color="red">The formula {result.toString()} is not the result of substitution {input_var} with {input_term} in the formula {input_formula}.</font>'))
           else:
-            display(Markdown(r'**<font color="red">Formula definition is not correct, check if all rules are applied correctly. Remember that a formula is defined by the following BNF: F :== P | ~ P | Q & Q | P | Q | P -> Q | P <-> Q | (P), where P,Q (in capital letters) are atoms.</font>**'))
+            display(HTML(r'<font color="red">Formula definition is not correct, check if all rules are applied correctly. Remember that a formula is defined by the following BNF: F :== P | ~ P | Q & Q | P | Q | P -> Q | P <-> Q | (P), where P,Q (in capital letters) are atoms.</font>'))
       except ValueError:
           s = traceback.format_exc()
           result = (s.split("@@"))[-1]
           print (f'{result}')
       else:
           pass
   run.on_click(on_button_run_clicked)
@@ -322,33 +322,33 @@
   wButtons = widgets.HBox([run])
   cResult = widgets.RadioButtons(
     options=['Yes', 'No'],
     value=None, 
     description='Answer:',
     disabled=False
 )
-  questao = '**Consider the following statements:**'
+  questao = 'Consider the following statements:'
   i = 1
   for assumption in input_assumptions:
     questao += f'\n1. {assumption}'
     i+=1
-  questao+='\n**Can we conclude that the statement below follows logically from the statements above?**'
+  questao+='\nCan we conclude that the statement below follows logically from the statements above?'
   questao+=f'\n{i}. {input_conclusion}'
-  display(Markdown(questao))
+  display(HTML(questao))
   display(widgets.HBox([cResult,wButtons]), output)
 
   def on_button_run_clicked(_):
     output.clear_output()
     with output:
       if (cResult.value==None):
-        display(Markdown('<font color="red">**Choose one of the alternatives! Try again!**</font>'))
+        display(HTML('<font color="red">Choose one of the alternatives! Try again!</font>'))
       elif(result_value==(cResult.value=='Yes')):
-        display(Markdown('<font color="blue">**Congratulations, you got the question right.**</font>'))
+        display(HTML('<font color="blue">Congratulations, you got the question right.</font>'))
       else:
-        display(Markdown('<font color="red">**Unfortunately, you got the question wrong. Try again!**</font>'))
+        display(HTML('<font color="red">Unfortunately, you got the question wrong. Try again!</font>'))
   run.on_click(on_button_run_clicked)
 
 def verify_formula(input_string=''):
   layout = widgets.Layout(width='90%')
   run = widgets.Button(description="Check")
   input = widgets.Text(
       value=input_string,
@@ -357,31 +357,31 @@
       layout=layout
       )
   cParentheses = widgets.Checkbox(value=False, description='Display Formula with Parentheses')
   cLatex = widgets.Checkbox(value=False, description='Display Formula in Latex')
   output = widgets.Output()
   wButtons = widgets.HBox([run, cParentheses, cLatex])
   
-  display(Markdown(r'**Enter your formula:**'))
+  display(HTML(r'Enter your formula:'))
   display(input, wButtons, output)
 
   def on_button_run_clicked(_):
     output.clear_output()
     with output:
       try:
           result = ParserFormula.getFormula(input.value)
           if(result!=None):
-              display(Markdown(r'**<font color="blue">Congratulations this is a formula of logic:</font>**'))
+              display(HTML(r'<font color="blue">Congratulations this is a formula of logic:</font>'))
               if(cLatex.value):
                 s = result.toLatex(parentheses=cParentheses.value)
                 display(Markdown(rf'${s}$'))
               else:
-                display(Markdown(rf'{result.toString(parentheses=cParentheses.value)}'))
+                display(HTML(rf'{result.toString(parentheses=cParentheses.value)}'))
           else:
-            display(Markdown(r'**<font color="red">Formula definition is not correct, check if all rules are applied correctly. Remember that a formula is defined by the following BNF: F :== P | ~ P | Q & Q | P | Q | P -> Q | P <-> Q | (P), where P,Q (in capital letters) are atoms.</font>**'))
+            display(HTML(r'<font color="red">Formula definition is not correct, check if all rules are applied correctly. Remember that a formula is defined by the following BNF: F :== P | ~ P | Q & Q | P | Q | P -> Q | P <-> Q | (P), where P,Q (in capital letters) are atoms.</font>'))
       except ValueError:
           s = traceback.format_exc()
           result = (s.split("@@"))[-1]
           print (f'{result}')
       else:
           pass
   run.on_click(on_button_run_clicked)
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `anita-0.1.8/src/anita/anita_pt.py` & `anita-0.1.9/src/anita/anita_pt.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,16 +2,16 @@
 import argparse
 import traceback
 
 parser = argparse.ArgumentParser(description='Analytic Tableau Proof Assistant (ANITA).')
 parser.add_argument("-i", type=str,help="Arquivo de entrada com a prova em ANITA.")
 parser.add_argument("-o", type=str,help="Arquivo de saída do resultado da verificação da prova na ANITA")
 args = parser.parse_args()
-fileName = 'example_anita.txt'
-fileSave = 'result_anita.txt'
+fileName = 'example_anita_pt.txt'
+fileSave = 'result_anita_pt.txt'
 if args.i is not None: fileName = args.i
 if args.o is not None: fileSave = args.o
 
 try:
     f = open(fileName, 'r')
     input_proof = f.read()
     result = anita.anita_pt_fo.ParserAnita.getProof(input_proof)
```

### Comparing `anita-0.1.8/src/anita/anita_pt_fo.py` & `anita-0.1.9/src/anita/anita_pt_fo.py`

 * *Files identical despite different names*

### Comparing `anita-0.1.8/src/anita/anita_pt_gui.py` & `anita-0.1.9/src/anita/anita_pt_gui.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,27 +1,49 @@
 import ipywidgets as widgets
-from IPython.display import display, Markdown
+from IPython.display import display, Markdown, HTML
 import traceback
 from anita.anita_pt_fo import ParserAnita, ParserTheorem, ParserFormula
 
-def anita(input_string='', height_layout='300px'):
+def anita(input_proof='', input_text_assumptions=[], input_text_conclusion='', height_layout='300px'):
   layout = widgets.Layout(width='90%', height=height_layout)
   run = widgets.Button(description="Verificar")
   input = widgets.Textarea(
-      value=input_string,
+      value=input_proof,
       placeholder='Digite sua demonstração',
       description='',
       layout=layout
       )
   cLatex = widgets.Checkbox(value=False, description='Exibir Latex')
   output = widgets.Output()
   wButtons = widgets.HBox([run, cLatex])
-  
-  display(widgets.HTML('<h3>Digite sua demonstração em Tableau Analítico:</h3>'), 
-          input, wButtons, output)
+  if input_text_conclusion!='':
+    display(Markdown( r'<b>Considere as seguintes afirmações:</b>'))
+    q_assumptions =''
+    i = 1
+    for assumption in input_text_assumptions:
+      q_assumptions += f'\n1. {assumption}'
+      i+=1
+    display(Markdown(q_assumptions))
+    display(Markdown(r'<b>Considere a afirmação abaixo segue logicamente das afirmações acima:'))
+    q_conclusion =f'\n{i}. {input_text_conclusion}'
+    display(Markdown(q_conclusion))
+    display(Markdown('### Represente as afirmações acima em lógica e digite sua demonstração em Tableau Analítico:'))
+    if input_proof=='':
+      # input.value = '# Considere a seguinte linguagem não lógica:\n# - ...\n# - ...\n# - ...\n# Representamos as afirmações através das seguintes fórmulas:'
+      input.value = '# Representamos as afirmações através das seguintes fórmulas:'
+      i = 1
+      for assumption in input_text_assumptions:
+        input.value += f'\n# {i}. ... para "{assumption}"'
+        i+=1
+      input.value += f'\n# {i}. ... para "{input_text_conclusion}"'
+      input.value += '\n# Assim, devemos demonstrar que o raciocínio abaixo é válido:'
+      input.value += '\n# ...'
+  else:  
+    display(Markdown('### Digite sua demonstração em Tableau Analítico:'))
+  display(input, wButtons, output)
 
   def on_button_run_clicked(_):
     output.clear_output()
     with output:
       try:
           result = ParserAnita.getProof(input.value)
           if(result.errors==[]):
@@ -65,15 +87,15 @@
       value=input_proof,
       placeholder='Digite sua demonstração:',
       description='',
       layout=layout
       )
   premisses, conclusion = ParserTheorem.getTheorem(input_theorem)
   if conclusion == None:
-    display(Markdown(rf'**<font color="red">{input_theorem} não é um teorema válido!</font>**'))
+    display(HTML(rf'<font color="red">{input_theorem} não é um teorema válido!</font>'))
     return
   cLatex = widgets.Checkbox(value=False, description='Exibir Latex')
   output = widgets.Output()
   wButtons = widgets.HBox([run, cLatex])
   
   display(widgets.HTML(f'<h3>Digite a demonstração de {input_theorem} em Tableau Analítico:</h3>'), 
           input, wButtons, output)
@@ -85,36 +107,36 @@
           result = ParserAnita.getProof(input.value)
           if(result.errors==[]):
               set_premisses = set([p.toString() for p in premisses])
               set_premisses_result = set([p.toString() for p in result.premisses])
               if(conclusion==result.conclusion and set_premisses==set_premisses_result):
                 msg = []
                 if(result.is_closed):
-                  display(Markdown(rf'**<font color="blue">Parabéns! A demonstraçãoo de {result.theorem} está correta.</font>**'))
+                  display(HTML(rf'<font color="blue">Parabéns! A demonstraçãoo de {result.theorem} está correta.</font>'))
                 else:
                   if result.saturared_branches!=[]:
-                    display(Markdown(rf'**<font color="blue">O teorema {result.theorem} não é válido.</font>**'))              
+                    display(HTML(rf'<font color="blue">O teorema {result.theorem} não é válido.</font>'))              
                     msg.append("São contra-exemplos:")
                     for s_v in result.counter_examples:
                       msg.append(s_v)                  
                   else:
-                    display(Markdown(rf'**<font color="red">A demonstração de {result.theorem} não está completa.</font>**'))              
+                    display(HTML(rf'<font color="red">A demonstração de {result.theorem} não está completa.</font>'))              
                     msg.append("Os ramos abaixo não estão saturados:")
                     for rules in result.open_branches:
                       msg.append("Ramo:")
                       msg.append('<br>'.join([r.toString() for r in reversed(rules)]))
                 if(cLatex.value):
                   msg.append("Código Latex:")
                   msg.append("%"+result.latex_theorem)
                   msg.append(result.colored_latex)
                 display(widgets.HTML('<br>'.join(msg)))       
               else:
-                display(Markdown(rf'**<font color="red">Sua demostração de {result.theorem} é válida, mas é diferente da demonstração solicitada {input_theorem}!</font>**'))
+                display(HTML(rf'<font color="red">Sua demostração de {result.theorem} é válida, mas é diferente da demonstração solicitada {input_theorem}!</font>'))
           else:
-            display(Markdown(rf'**<font color="red">Sua demonstração contém os seguintes erros:</font>**'))
+            display(HTML(rf'<font color="red">Sua demonstração contém os seguintes erros:</font>'))
             for error in result.errors:
                 print(error)
       except ValueError:
           s = traceback.format_exc()
           result = (s.split("@@"))[-1]
           print (f'{result}')
       else:
@@ -129,33 +151,33 @@
     value=None, 
     description='Resposta:',
     disabled=False
 )
   output = widgets.Output()
   wButtons = widgets.HBox([run])
   
-  display(Markdown(rf'**A variável {input_var} é substituível pelo termo {input_term} na fórmula {input_formula}:**'))
+  display(HTML(rf'A variável {input_var} é substituível pelo termo {input_term} na fórmula {input_formula}:'))
   display(cResult, wButtons, output)
 
   def on_button_run_clicked(_):
     output.clear_output()
     with output:
       try:
           f = ParserFormula.getFormula(input_formula)
           if(f!=None):
             if (f.is_substitutable(input_var,input_term) and cResult.value=='Sim'):
-              display(Markdown(r'**<font color="blue">Parabéns você acertou a questão!</font>**'))              
-              display(Markdown(rf'A variável {input_var} **é substituível** pelo termo {input_term} na fórmula {input_formula}.'))              
+              display(HTML(r'<font color="blue">Parabéns você acertou a questão!</font>'))              
+              display(HTML(rf'A variável {input_var} é substituível pelo termo {input_term} na fórmula {input_formula}.'))              
             elif not f.is_substitutable(input_var,input_term) and cResult.value=='Não':
-              display(Markdown(r'**<font color="blue">Parabéns você acertou a questão!</font>**'))              
-              display(Markdown(rf'A variável {input_var} **não é substituível** pelo termo {input_term} na fórmula {input_formula}.')) 
+              display(HTML(r'<font color="blue">Parabéns você acertou a questão!</font>'))              
+              display(HTML(rf'A variável {input_var} não é substituível pelo termo {input_term} na fórmula {input_formula}.')) 
             else:
-              display(Markdown(rf'**<font color="red">Infelizmente, você errou a questão.</font>**'))
+              display(HTML(rf'<font color="red">Infelizmente, você errou a questão.</font>'))
           else:
-            display(Markdown(r'**<font color="red">A definição da fórmula não está correta, verifique se todas regras foram aplicadas corretamente. Lembre-se que uma fórmula é definida pela seguinte BNF: F :== P | ~ P | P & Q | P | Q | P -> Q | P <-> Q | (P), onde P,Q (em caixa alta) são átomos.</font>**'))
+            display(HTML(r'<font color="red">A definição da fórmula não está correta, verifique se todas regras foram aplicadas corretamente. Lembre-se que uma fórmula é definida pela seguinte BNF: F :== P | ~ P | P & Q | P | Q | P -> Q | P <-> Q | (P), onde P,Q (em caixa alta) são átomos.</font>'))
       except ValueError:
           s = traceback.format_exc()
           result = (s.split("@@"))[-1]
           print (f'{result}')
       else:
           pass
   run.on_click(on_button_run_clicked)
@@ -168,31 +190,31 @@
       placeholder='Digite as variáveis separadas por ;',
       description='',
       layout=layout
       )
   output = widgets.Output()
   wButtons = widgets.HBox([run])
   
-  display(Markdown(rf'**Digite o conjunto de variávels da fórmula {input_formula}:**'))
-  display(Markdown(r'Cada elemento do seu conjunto deve ser separado por ; (ponto-e-vírgula)'))
+  display(HTML(rf'Digite o conjunto de variávels da fórmula {input_formula}:'))
+  display(HTML(r'Cada elemento do seu conjunto deve ser separado por ; (ponto-e-vírgula)'))
   display(input, wButtons, output)
 
   def on_button_run_clicked(_):
     output.clear_output()
     with output:
       try:
           result = ParserFormula.getFormula(input_formula)
           variables = set([x.strip() for x in input.value.strip().split(";")])
           if(result!=None):
             if variables==result.all_variables():
-              display(Markdown(r'**<font color="blue">Parabéns você acertou a questão.</font>**'))              
+              display(HTML(r'<font color="blue">Parabéns você acertou a questão.</font>'))              
             else:
-              display(Markdown(rf'**<font color="red">Você errou a questão.</font>**'))
+              display(HTML(rf'<font color="red">Você errou a questão.</font>'))
           else:
-            display(Markdown(r'**<font color="red">A definição da fórmula não está correta, verifique se todas regras foram aplicadas corretamente. Lembre-se que uma fórmula é definida pela seguinte BNF: F :== P | ~ P | P & Q | P | Q | P -> Q | P <-> Q | (P), onde P,Q (em caixa alta) são átomos.</font>**'))
+            display(HTML(r'<font color="red">A definição da fórmula não está correta, verifique se todas regras foram aplicadas corretamente. Lembre-se que uma fórmula é definida pela seguinte BNF: F :== P | ~ P | P & Q | P | Q | P -> Q | P <-> Q | (P), onde P,Q (em caixa alta) são átomos.</font>'))
       except ValueError:
           s = traceback.format_exc()
           result = (s.split("@@"))[-1]
           print (f'{result}')
       else:
           pass
   run.on_click(on_button_run_clicked)
@@ -206,31 +228,31 @@
       placeholder='Digite as variáveis separadas por ;',
       description='',
       layout=layout
       )
   output = widgets.Output()
   wButtons = widgets.HBox([run])
   
-  display(Markdown(rf'**Digite o conjunto de variávels livres da fórmula {input_formula}:**'))
-  display(Markdown(r'Cada elemento do seu conjunto deve ser separado por ; (ponto-e-vírgula)'))
+  display(HTML(rf'Digite o conjunto de variávels livres da fórmula {input_formula}:'))
+  display(HTML(r'Cada elemento do seu conjunto deve ser separado por ; (ponto-e-vírgula)'))
   display(input, wButtons, output)
 
   def on_button_run_clicked(_):
     output.clear_output()
     with output:
       try:
           result = ParserFormula.getFormula(input_formula)
           variables = set([x.strip() for x in input.value.strip().split(";")])
           if(result!=None):
             if variables==result.free_variables():
-              display(Markdown(r'**<font color="blue">Parabéns você acertou a questão.</font>**'))              
+              display(HTML(r'<font color="blue">Parabéns você acertou a questão.</font>'))              
             else:
-              display(Markdown(rf'**<font color="red">Você errou a questão.</font>**'))
+              display(HTML(rf'<font color="red">Você errou a questão.</font>'))
           else:
-            display(Markdown(r'**<font color="red">A definição da fórmula não está correta, verifique se todas regras foram aplicadas corretamente. Lembre-se que uma fórmula é definida pela seguinte BNF: F :== P | ~ P | P & Q | P | Q | P -> Q | P <-> Q | (P), onde P,Q (em caixa alta) são átomos.</font>**'))
+            display(HTML(r'<font color="red">A definição da fórmula não está correta, verifique se todas regras foram aplicadas corretamente. Lembre-se que uma fórmula é definida pela seguinte BNF: F :== P | ~ P | P & Q | P | Q | P -> Q | P <-> Q | (P), onde P,Q (em caixa alta) são átomos.</font>'))
       except ValueError:
           s = traceback.format_exc()
           result = (s.split("@@"))[-1]
           print (f'{result}')
       else:
           pass
   run.on_click(on_button_run_clicked)
@@ -243,31 +265,31 @@
       placeholder='Digite as variáveis separadas por ;',
       description='',
       layout=layout
       )
   output = widgets.Output()
   wButtons = widgets.HBox([run])
   
-  display(Markdown(rf'**Digite o conjunto de variávels ligadas da fórmula {input_formula}:**'))
-  display(Markdown(r'Cada elemento do seu conjunto deve ser separado por ; (ponto-e-vírgula)'))
+  display(HTML(rf'Digite o conjunto de variávels ligadas da fórmula {input_formula}:'))
+  display(HTML(r'Cada elemento do seu conjunto deve ser separado por ; (ponto-e-vírgula)'))
   display(input, wButtons, output)
 
   def on_button_run_clicked(_):
     output.clear_output()
     with output:
       try:
           result = ParserFormula.getFormula(input_formula)
           variables = set([x.strip() for x in input.value.strip().split(";")])
           if(result!=None):
             if variables==result.bound_variables():
-              display(Markdown(r'**<font color="blue">Parabéns você acertou a questão.</font>**'))              
+              display(HTML(r'<font color="blue">Parabéns você acertou a questão.</font>'))              
             else:
-              display(Markdown(rf'**<font color="red">Você errou a questão.</font>**'))
+              display(HTML(rf'<font color="red">Você errou a questão.</font>'))
           else:
-            display(Markdown(r'**<font color="red">A definição da fórmula não está correta, verifique se todas regras foram aplicadas corretamente. Lembre-se que uma fórmula é definida pela seguinte BNF: F :== P | ~ P | P & Q | P | Q | P -> Q | P <-> Q | (P), onde P,Q (em caixa alta) são átomos.</font>**'))
+            display(HTML(r'<font color="red">A definição da fórmula não está correta, verifique se todas regras foram aplicadas corretamente. Lembre-se que uma fórmula é definida pela seguinte BNF: F :== P | ~ P | P & Q | P | Q | P -> Q | P <-> Q | (P), onde P,Q (em caixa alta) são átomos.</font>'))
       except ValueError:
           s = traceback.format_exc()
           result = (s.split("@@"))[-1]
           print (f'{result}')
       else:
           pass
   run.on_click(on_button_run_clicked)
@@ -282,35 +304,35 @@
       layout=layout
       )
   cParentheses = widgets.Checkbox(value=False, description='Exibir Fórmula com Parênteses')
   cLatex = widgets.Checkbox(value=False, description='Exibir Fórmula em Latex')
   output = widgets.Output()
   wButtons = widgets.HBox([run, cParentheses, cLatex])
   
-  display(Markdown(rf'**Digite a fórmula que é resultado da substituição da variável {input_var} pelo termo {input_term} na fórmula {input_formula}:**'))
+  display(HTML(rf'Digite a fórmula que é resultado da substituição da variável {input_var} pelo termo {input_term} na fórmula {input_formula}:'))
   display(input, wButtons, output)
 
   def on_button_run_clicked(_):
     output.clear_output()
     with output:
       try:
           f = ParserFormula.getFormula(input_formula)
           result = ParserFormula.getFormula(input.value)
           if(result!=None):
             if result==f.substitution(input_var,input_term):
-              display(Markdown(r'**<font color="blue">Parabéns essa é a subtituição correta:</font>**'))              
+              display(HTML(r'<font color="blue">Parabéns essa é a subtituição correta:</font>'))              
               if(cLatex.value):
                 s = result.toLatex(parentheses=cParentheses.value)
                 display(Markdown(rf'${s}$'))
               else:
-                display(Markdown(rf'{result.toString(parentheses=cParentheses.value)}'))
+                display(HTML(rf'{result.toString(parentheses=cParentheses.value)}'))
             else:
-              display(Markdown(rf'**<font color="red">A fórmula {result.toString()} não é o resultado da substituição de {input_var} por {input_term} na fórmula {input_formula}.</font>**'))
+              display(HTML(rf'<font color="red">A fórmula {result.toString()} não é o resultado da substituição de {input_var} por {input_term} na fórmula {input_formula}.</font>'))
           else:
-            display(Markdown(r'**<font color="red">A definição da fórmula não está correta, verifique se todas regras foram aplicadas corretamente. Lembre-se que uma fórmula é definida pela seguinte BNF: F :== P | ~ P | P & Q | P | Q | P -> Q | P <-> Q | (P), onde P,Q (em caixa alta) são átomos.</font>**'))
+            display(HTML(r'<font color="red">A definição da fórmula não está correta, verifique se todas regras foram aplicadas corretamente. Lembre-se que uma fórmula é definida pela seguinte BNF: F :== P | ~ P | P & Q | P | Q | P -> Q | P <-> Q | (P), onde P,Q (em caixa alta) são átomos.</font>'))
       except ValueError:
           s = traceback.format_exc()
           result = (s.split("@@"))[-1]
           print (f'{result}')
       else:
           pass
   run.on_click(on_button_run_clicked)
@@ -323,33 +345,33 @@
   wButtons = widgets.HBox([run])
   cResult = widgets.RadioButtons(
     options=['Sim', 'Não'],
     value=None, 
     description='Resposta:',
     disabled=False
 )
-  questao = '**Considere as seguintes afirmações:**'
+  questao = 'Considere as seguintes afirmações:'
   i = 1
   for assumption in input_assumptions:
     questao += f'\n1. {assumption}'
     i+=1
-  questao+='\n**Podemos concluir que a afirmação abaixo segue logicamente das afirmações acima?**'
+  questao+='\nPodemos concluir que a afirmação abaixo segue logicamente das afirmações acima?'
   questao+=f'\n{i}. {input_conclusion}'
-  display(Markdown(questao))
+  display(HTML(questao))
   display(widgets.HBox([cResult,wButtons]), output)
 
   def on_button_run_clicked(_):
     output.clear_output()
     with output:
       if (cResult.value==None):
-        display(Markdown('<font color="red">**Escolha uma das alternativas! Tente novamente!**</font>'))
+        display(HTML('<font color="red">Escolha uma das alternativas! Tente novamente!</font>'))
       elif(result_value==(cResult.value=='Sim')):
-        display(Markdown('<font color="blue">**Parabéns, você acertou a questão.**</font>'))
+        display(HTML('<font color="blue">Parabéns, você acertou a questão.</font>'))
       else:
-        display(Markdown('<font color="red">**Infelizmente, você errou a questão. Tente novamente!**</font>'))
+        display(HTML('<font color="red">Infelizmente, você errou a questão. Tente novamente!</font>'))
   run.on_click(on_button_run_clicked)
 
 def verify_formula(input_string=''):
   layout = widgets.Layout(width='90%')
   run = widgets.Button(description="Verificar")
   input = widgets.Text(
       value=input_string,
@@ -358,31 +380,31 @@
       layout=layout
       )
   cParentheses = widgets.Checkbox(value=False, description='Exibir Fórmula com Parênteses')
   cLatex = widgets.Checkbox(value=False, description='Exibir Fórmula em Latex')
   output = widgets.Output()
   wButtons = widgets.HBox([run, cParentheses, cLatex])
   
-  display(Markdown(r'**Digite sua fórmula:**'))
+  display(HTML(r'Digite sua fórmula:'))
   display(input, wButtons, output)
 
   def on_button_run_clicked(_):
     output.clear_output()
     with output:
       try:
           result = ParserFormula.getFormula(input.value)
           if(result!=None):
-              display(Markdown(r'**<font color="blue">Parabéns essa é uma fórmula da lógica:</font>**'))
+              display(HTML(r'<font color="blue">Parabéns essa é uma fórmula da lógica:</font>'))
               if(cLatex.value):
                 s = result.toLatex(parentheses=cParentheses.value)
                 display(Markdown(rf'${s}$'))
               else:
-                display(Markdown(rf'{result.toString(parentheses=cParentheses.value)}'))
+                display(HTML(rf'{result.toString(parentheses=cParentheses.value)}'))
           else:
-            display(Markdown(r'**<font color="red">A definição da fórmula não está correta, verifique se todas regras foram aplicadas corretamente. Lembre-se que uma fórmula é definida pela seguinte BNF: F :== P | ~ P | P & Q | P | Q | P -> Q | P <-> Q | (P), onde P,Q (em caixa alta) são átomos.</font>**'))
+            display(HTML(r'<font color="red">A definição da fórmula não está correta, verifique se todas regras foram aplicadas corretamente. Lembre-se que uma fórmula é definida pela seguinte BNF: F :== P | ~ P | P & Q | P | Q | P -> Q | P <-> Q | (P), onde P,Q (em caixa alta) são átomos.</font>'))
       except ValueError:
           s = traceback.format_exc()
           result = (s.split("@@"))[-1]
           print (f'{result}')
       else:
           pass
   run.on_click(on_button_run_clicked)
```

### Comparing `anita-0.1.8/src/anita/example_theorems.py` & `anita-0.1.9/src/anita/example_theorems.py`

 * *Files identical despite different names*

### Comparing `anita-0.1.8/src/anita.egg-info/PKG-INFO` & `anita-0.1.9/src/anita.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 Metadata-Version: 2.1
 Name: anita
-Version: 0.1.8
+Version: 0.1.9
 Summary: ANITA is a proof assistant for teaching analytic tableaux to computer science students. ANITA allows students to write their proofs and automatically checks whether the proofs are correct and, if not, displays any errors found.
 Home-page: https://github.com/daviromero/anita
 Author: Davi Romero de Vasconcelos
 Author-email: daviromero@ufc.br
 License: MIT
 Keywords: Analytic Tableaux,Teaching Logic,Educational Software
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
 License-File: license.txt
 
 # Analytic Tableau Proof Assistant (ANITA)
 
 The ANITA is a tool written in Python that can be used as a desktop application, or in a [web platform](https://sistemas.quixada.ufc.br/anita/en/). The main idea is that the students can write their proofs as similar as possible to what is available in the textbooks and to what the students would usually write on paper. ANITA allows the students to automatically check whether a proof in the analytic tableaux is valid. If the proof is not correct, ANITA will display the errors of the proof. So, the students may make mistakes and learn from the errors. The web interface is very easy-to-use and has: 
-- An area for editing the proof in plain text. The students should write a proof in the Fitch-style (see [AT Rules](AT-Rules.pdf)).
+- An area for editing the proof in plain text. The students should write a proof in Fitch-style (see [AT Rules](https://github.com/daviromero/anita/blob/main/AT-Rules.pdf)).
 - A message area to display whether the proof is valid, the countermodel, or the errors on the proof.
 - And the following links: 
   - Check, to check the correctness of the proof; 
   - Manual, to view a document with the inference rules and examples; 
   - LaTeX, to generate the LaTeX code of the trees from a valid proof. Use the `qtree` package in your LaTeX code; 
   - LaTeX in Overleaf, to open the proof source code directly in [Overleaf](http://overleaf.com/) that is a collaborative platform for editing LaTeX
 
@@ -37,27 +37,27 @@
 | :---:  |  :---:  | :---: | :---:  | :---:  | :---:  | :---:  | :---:  | :---:  | :---: |
 | LaTeX  |  $\backslash\textrm{lnot}$ | $\backslash\textrm{land}$ | $\backslash\textrm{lor}$ | $\backslash\textrm{rightarrow}$ | $\backslash\textrm{forall x}$ | $\backslash\textrm{exists x}$ | $\backslash\textrm{bot}$ | $[.~]$ | $\backslash\textrm{vdash}$ |
 | ANITA |  ~  | \& | $\mid$ | -> | Ax | Ex | @  | { } | \|- |
 
 ![](ANITA-EXAMPLE.png)
 
 ## License
-ANITA is available by a ![**MIT License**](license.txt).
+ANITA is available by [**MIT License**](https://github.com/daviromero/anita/blob/main/license.txt).
 
 ## Requirements:
-- You must install the [rply 0.7.8 package](https://pypi.org/project/rply/)
+- You must install [rply 0.7.8 package](https://pypi.org/project/rply/)
 
 ## Install
 
-To install ANITA from the Github, run the following command:
+To install ANITA from Github, run the following command:
 ```bash
 pip install git+https://github.com/daviromero/anita.git
 ```
 
-To install ANITA from the PyPi repository, run the following command:
+To install ANITA from PyPi repository, run the following command:
 ```bash
 pip install anita
 ```
 
 ## ANITA
 You can run ANITA with the command line: 
 ```bash
```

