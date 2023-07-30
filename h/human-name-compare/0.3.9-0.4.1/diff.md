# Comparing `tmp/human-name-compare-0.3.9.tar.gz` & `tmp/human-name-compare-0.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/human-name-compare-0.3.9.tar", last modified: Wed Jan 27 09:58:44 2021, max compression
+gzip compressed data, was "human-name-compare-0.4.1.tar", last modified: Sun Jul 30 14:59:34 2023, max compression
```

## Comparing `human-name-compare-0.3.9.tar` & `human-name-compare-0.4.1.tar`

### file list

```diff
@@ -1,14 +1,15 @@
-drwxr-xr-x   0 caziel     (501) staff       (20)        0 2021-01-27 09:58:44.000000 human-name-compare-0.3.9/
--rw-r--r--   0 caziel     (501) staff       (20)     2232 2021-01-27 09:58:44.000000 human-name-compare-0.3.9/PKG-INFO
--rwxr-xr-x   0 caziel     (501) staff       (20)      854 2020-07-22 16:48:33.000000 human-name-compare-0.3.9/hn-compare
-drwxr-xr-x   0 caziel     (501) staff       (20)        0 2021-01-27 09:58:44.000000 human-name-compare-0.3.9/human_name_compare/
--rw-r--r--   0 caziel     (501) staff       (20)    15092 2021-01-27 09:48:02.000000 human-name-compare-0.3.9/human_name_compare/__init__.py
--rw-r--r--   0 caziel     (501) staff       (20)     1523 2020-07-22 14:49:44.000000 human-name-compare-0.3.9/logger.py
--rw-r--r--   0 caziel     (501) staff       (20)     1313 2020-07-22 15:53:30.000000 human-name-compare-0.3.9/README.md
--rw-r--r--   0 caziel     (501) staff       (20)      870 2021-01-27 09:56:50.000000 human-name-compare-0.3.9/setup.py
--rw-r--r--   0 caziel     (501) staff       (20)       38 2021-01-27 09:58:44.000000 human-name-compare-0.3.9/setup.cfg
-drwxr-xr-x   0 caziel     (501) staff       (20)        0 2021-01-27 09:58:44.000000 human-name-compare-0.3.9/human_name_compare.egg-info/
--rw-r--r--   0 caziel     (501) staff       (20)     2232 2021-01-27 09:58:44.000000 human-name-compare-0.3.9/human_name_compare.egg-info/PKG-INFO
--rw-r--r--   0 caziel     (501) staff       (20)      240 2021-01-27 09:58:44.000000 human-name-compare-0.3.9/human_name_compare.egg-info/SOURCES.txt
--rw-r--r--   0 caziel     (501) staff       (20)       19 2021-01-27 09:58:44.000000 human-name-compare-0.3.9/human_name_compare.egg-info/top_level.txt
--rw-r--r--   0 caziel     (501) staff       (20)        1 2021-01-27 09:58:44.000000 human-name-compare-0.3.9/human_name_compare.egg-info/dependency_links.txt
+drwxr-xr-x   0 caziel     (501) staff       (20)        0 2023-07-30 14:59:34.059553 human-name-compare-0.4.1/
+-rw-r--r--   0 caziel     (501) staff       (20)     1098 2020-07-22 15:20:00.000000 human-name-compare-0.4.1/LICENSE.txt
+-rw-r--r--   0 caziel     (501) staff       (20)     1875 2023-07-30 14:59:34.059122 human-name-compare-0.4.1/PKG-INFO
+-rw-r--r--   0 caziel     (501) staff       (20)     1313 2020-07-22 15:53:30.000000 human-name-compare-0.4.1/README.md
+-rwxr-xr-x   0 caziel     (501) staff       (20)      854 2020-07-22 16:48:33.000000 human-name-compare-0.4.1/hn-compare
+drwxr-xr-x   0 caziel     (501) staff       (20)        0 2023-07-30 14:59:34.056800 human-name-compare-0.4.1/human_name_compare/
+-rw-r--r--   0 caziel     (501) staff       (20)    16592 2023-07-30 14:57:01.000000 human-name-compare-0.4.1/human_name_compare/__init__.py
+drwxr-xr-x   0 caziel     (501) staff       (20)        0 2023-07-30 14:59:34.058582 human-name-compare-0.4.1/human_name_compare.egg-info/
+-rw-r--r--   0 caziel     (501) staff       (20)     1875 2023-07-30 14:59:34.000000 human-name-compare-0.4.1/human_name_compare.egg-info/PKG-INFO
+-rw-r--r--   0 caziel     (501) staff       (20)      252 2023-07-30 14:59:34.000000 human-name-compare-0.4.1/human_name_compare.egg-info/SOURCES.txt
+-rw-r--r--   0 caziel     (501) staff       (20)        1 2023-07-30 14:59:34.000000 human-name-compare-0.4.1/human_name_compare.egg-info/dependency_links.txt
+-rw-r--r--   0 caziel     (501) staff       (20)       19 2023-07-30 14:59:34.000000 human-name-compare-0.4.1/human_name_compare.egg-info/top_level.txt
+-rw-r--r--   0 caziel     (501) staff       (20)     1523 2020-07-22 14:49:44.000000 human-name-compare-0.4.1/logger.py
+-rw-r--r--   0 caziel     (501) staff       (20)       38 2023-07-30 14:59:34.059669 human-name-compare-0.4.1/setup.cfg
+-rw-r--r--   0 caziel     (501) staff       (20)      870 2023-07-30 14:59:31.000000 human-name-compare-0.4.1/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `human-name-compare-0.3.9/PKG-INFO` & `human-name-compare-0.4.1/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,58 +1,58 @@
 Metadata-Version: 2.1
 Name: human-name-compare
-Version: 0.3.9
+Version: 0.4.1
 Summary: a tool for comparing human names
 Home-page: https://github.com/digitalkaoz/py_human_name_compare
+Download-URL: https://github.com/digitalkaoz/py_human_name_compare/archive/0.4.1.tar.gz
 Author: Robert Schoenthal
 Author-email: robert.schoenthal@gmail.com
-License: UNKNOWN
-Download-URL: https://github.com/digitalkaoz/py_human_name_compare/archive/0.3.9.tar.gz
-Description: # Human Name Compare
-        
-        ![human_name_compare](https://github.com/digitalkaoz/py_human_name_compare/workflows/human_name_compare/badge.svg)
-        [![PyPI version](https://badge.fury.io/py/human-name-compare.svg)](https://badge.fury.io/py/human-name-compare)
-        
-        
-        the Problem:
-        
-        Check if `Dr. Peter Müller` and `Peter K. Müller` and `Dr. med. Peter Karsten Müller` and `P. Müller` indicate if its the same person
-        
-        There are gazillion tiny bits and pieces which makes this trivial task hard e.g.:
-        
-        * "R. Schönthal" "Robert Schönthal" - the only have initials on one side
-        * "Erik Schönthal" "Robert Schönthal" - the firstname name doesnt match
-        * "Robert Erik Schönthal" "Robert Peter Schönthal" - the middle name doesnt match 
-        * "Robert-Erik Schönthal" "Robert Erik Schönthal" - we have an "-" in our firstnames
-        * "Robeert Schönthal" "Robert Schönthal" - the firstname has a typo
-        * "Robert Müller" "Robert Schönthal" - the lastname doesnt match
-        * "Herr Robert Müller" "Dr. med. Robert Schönthal" - we have some prefixes
-        
-        and so on...
-        
-        ## Usage
-        
-        ### CLI
-        
-        ```shell script
-        $ hn-compare compare "Robert Schönthal" "Robert Schönthal"
-        ```
-        
-        ### Python
-        
-        ```python
-        from human_name_compare import match_name
-        
-        match_name("Robert Schönthal", "Robert Schönthal")
-        ```
-        
-        ## Tests
-        
-        ````shell script
-        $ python -m pytest .
-        ````
 Keywords: NLP,HUMANNAME
-Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
+License-File: LICENSE.txt
+
+# Human Name Compare
+
+![human_name_compare](https://github.com/digitalkaoz/py_human_name_compare/workflows/human_name_compare/badge.svg)
+[![PyPI version](https://badge.fury.io/py/human-name-compare.svg)](https://badge.fury.io/py/human-name-compare)
+
+
+the Problem:
+
+Check if `Dr. Peter Müller` and `Peter K. Müller` and `Dr. med. Peter Karsten Müller` and `P. Müller` indicate if its the same person
+
+There are gazillion tiny bits and pieces which makes this trivial task hard e.g.:
+
+* "R. Schönthal" "Robert Schönthal" - the only have initials on one side
+* "Erik Schönthal" "Robert Schönthal" - the firstname name doesnt match
+* "Robert Erik Schönthal" "Robert Peter Schönthal" - the middle name doesnt match 
+* "Robert-Erik Schönthal" "Robert Erik Schönthal" - we have an "-" in our firstnames
+* "Robeert Schönthal" "Robert Schönthal" - the firstname has a typo
+* "Robert Müller" "Robert Schönthal" - the lastname doesnt match
+* "Herr Robert Müller" "Dr. med. Robert Schönthal" - we have some prefixes
+
+and so on...
+
+## Usage
+
+### CLI
+
+```shell script
+$ hn-compare compare "Robert Schönthal" "Robert Schönthal"
+```
+
+### Python
+
+```python
+from human_name_compare import match_name
+
+match_name("Robert Schönthal", "Robert Schönthal")
+```
+
+## Tests
+
+````shell script
+$ python -m pytest .
+````
```

### Comparing `human-name-compare-0.3.9/hn-compare` & `human-name-compare-0.4.1/hn-compare`

 * *Files identical despite different names*

### Comparing `human-name-compare-0.3.9/human_name_compare/__init__.py` & `human-name-compare-0.4.1/human_name_compare/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,95 +1,111 @@
 import re
 import unicodedata
 from typing import Optional, List
 
 import gender_guesser.detector as gender
-from Levenshtein._levenshtein import distance
+from Levenshtein import distance
 from nameparser import HumanName
 from nameparser.config import Constants
 
 _additional_titles = ["med.", "Dipl.", "Psych.", "Apl.", "Ass.", "rer.", "nat.", "phil.", "univ.", "Priv.", "Doz.",
                       "PD", "Prof. (FH)", "Dott.", "MUDr.", "MU", "habil.", "Dr./Univ.", "Dott./Univ.", "Doctor-medic",
                       "Med.", "sc.", "medic.", "dent.", "AO", "a.o.", "OFA", "oec.", "troph.", "Doctor-medic",
                       "Honorarprof.", "Doctor-medic/Univ.", "Universitätsprof.", "Phys.", "PMU", "Dipl.-Psych.",
                       "chem.", "Biol.", "Ph.D.", "hom.", "disc.", "pol.", "M.B", "M.Sc.", "MSc", "MHBA",
                       "Honorarprofessorin", "PH", "M.A.", "Honorem/RCh", "Dr./TR", "Tip", "M.D./Afghanistan",
                       "M.B.CH.B", "Sanitätsrat", "dr/Universität", "-Ing.", "DrPH", "jur.", "Cirug./EC",
                       "professor/NGMU", "Ing.", "M.D./Ain", "Universität", "M.D./SYR", "EC", "pocetny", "vet.",
                       "DrM/Univ.", "Cirug.", "drs.", "h.c.", "d-r", "M. A.", "M. D./Univ.", "Diplom-Sozialwirt",
-                      "B.Ch.", "M.B.", "scient.", "pth.", "Dipl.-Psych.",
+                      "B.Ch.", "M.B.", "scient.", "pth.", "Dipl.-Psych.","Bac.",
                       "D.O.", "DAAO", "Ch.B./Univ.", "HMA", "Diplom-Psychologe", "physiol.", "P.H.", "hab.", "M.B.B.S.",
                       "hum.", "M.D.", "/OAK", "vrac", "Diplom-Biologe", "dr/Univ.", "Docteur", "Médecine/Univ.",
                       "B.M.D.", "doktor", "medicine", "/Mediz.", "M.B.", "M.D./Univ.", "M.B.,B.Ch.(ET)", "M.S.P.",
                       "Conf.", "MScIH", "MaHM", "Medica", "MOM", "M.Sc.", "Profesor", "Honorario", "honorary", "Lic.",
                       "Assistant", "agr.", "soc.", "Privatdozent", "ZA.", "ZA", "dr./Uni.", "OA", "Doctor-Medic/IMF",
                       "Privat-Dozent", "MB", "ChB", "Duktur", "fi-t-tibb", "al-bashari", "Priv-Doz.", "I.N.E.S.S.",
                       "Stom.", "MS/Tufts", "ZÄ", "Dr./IMF", "B.D.S./Univ.", "D.D.S.", "/IMF", "Mag.", "LA", "CA", "MBA",
                       "Prim.", "mult.", "MAS", "Univ.-Prof.", "Assoz.-Prof.", "PD", "PhD", "MSc", "DM", "asoc.", "FEBO",
                       "Oradea", "Doc.", "Deptl.", "MB.Ch.B.", "OMR", "OMD", "Fachärztin", "D.A.L.M.", "DEAA", "jun.",
                       "Assistenzärztin", "Klinikdirektor", "Soz.", "M.B.A.", "FEAN", "FNCS", "IFAANS", "M.S.",
                       "Med.-Dir.", "Sportwiss.", "OTA", "a.D.", "medic/R", "B.S.", "M.B.", "Ch.B.", "D.A.L.M.", "MaHM",
-                      "B.A.", "UIPA", "universae/Semmelweis", "Doktor-e-reste-ye", "dr.sc.", "VUB", "Doktoru/Univ.",
+                      "B.A.", "UIPA", "universae/Semmelweis", "Doktor-e-reste-ye", "dr.sc.", "VUB", "DoktoFru/Univ.",
                       "Doktor-i", "pezeski/Univ.", "medic/Univ.", "medicinae", "universae", "San.-Rat", "Medizinalrat",
                       "Dott/Univ.", "M.D./Univ.Damaskus", "Ped.", "/I.N.E.S.S.", "LL.M.", "Ltd.", "Doktor-e", "M.sc.",
                       "Lic./Univ.", "pezeski/Univ.", "Odessa/UdSSR", "Medizinaldirektor", "Doktore", "pezeski/",
                       "Diplom-Biologin", "/Univ.", "dr.sc.", "-Phys.", "Universitätsprofessor", "Dozent", "MoHM",
                       "Oberfeldarzt", "reste-ye", "Doktora-ye", "reshte-ye", "pezeshki", "Tg.-Mures", "Akademische",
                       "Direktorin", "Diplom-Sozialpädagogin", "M.P.H.", "postgrad.", "asociat/Univ.", "-medic/IMF",
                       "-medic/IMP", "San.", "-Rat", "-medic", "medic/IM", "-med.", "-medic/ifM", "Frf.", "Honprof.",
                       "Theol.", "MPH-HAM", "D.E.A.A.", "Frhr.", "Drs.", "FEBS"]
 
 _surname_titles = ["Von ", "von ", "van ", "Van ", "dos ", "Dos "]
 
 # some titles are actual names, the result would be None, therefore we remove some
-_remove_title = ["mahdi", "graf", "singer", "lama", "pastor", "imam", "jun", "baba","baron"]
+_remove_title = ["mahdi", "graf", "singer", "lama", "pastor", "imam", "jun", "baba", "baron"]
 
 constants = Constants()
 for a in _additional_titles:
     constants.titles.add(a)
 for a in _remove_title:
     constants.titles.remove(a)
 
 guess_gender = gender.Detector()
 
 
 def normalize_title(inp: str) -> Optional[str]:
     """
     normalizes medical titles
     """
-    if inp is None:
+    if type(inp) is not str:
         return None
-    return inp.replace("Professor", "Prof.") \
-        .replace("doktor medicine", "Dr. med.") \
-        .replace("Doktor", "Dr.") \
-        .replace("dr/Universität", "Dr. Univ.") \
+
+    if inp.strip() == "":
+        return None
+    return inp.replace("dr/Universität", "Dr. Univ.") \
+        .replace("Universitätsprofessor", "Prof. Univ.") \
         .replace("Universitätsprof.", "Prof. Univ.") \
+        .replace("Univ. Doz.", "PD") \
         .replace("Universität", "Univ.") \
+        .replace("Professor", "Prof.") \
+        .replace("prof.", "Prof.") \
+        .replace("doktor medicine", "Dr. med.") \
+        .replace("Doktor", "Dr.") \
         .replace("Doctor", "Dr.") \
         .replace("dr.", "Dr.") \
         .replace("medic.", "med.") \
         .replace("Priv. -Doz.", "PD") \
         .replace("Priv-Doz.", "PD") \
         .replace("Privatdozent", "PD") \
         .replace("Privat - Dozent", "PD") \
         .replace("Priv.-Doz.", "PD") \
+        .replace("Priv.Doz.", "PD") \
+        .replace("Priv. Doz.", "PD") \
+        .replace("PDDr.", "PD Dr.") \
+        .replace("PD.", "PD") \
         .replace(" / ", " ") \
         .replace("./", ". ") \
         .replace(". /", ". ") \
         .replace(" - ", " ") \
         .replace(".-", ".") \
+        .replace(". -", ". ") \
+        .replace('Dr.med.', 'Dr. med.').replace('Dr', 'Dr.').replace('Prof', 'Prof.')\
+        .replace('..', '.').replace('.','. ') \
         .replace("  ", " ") \
-        .replace(". -", ". ").strip()
+        .strip()
 
 
 def person_title(inp: str, normalize=True) -> Optional[str]:
     """
     extract the medic title from "GENDER? TITLE? NAME" strings
     """
-    if inp is None or inp.strip() == "":
+    if type(inp) is not str:
+        return None
+
+    if inp.strip() == "":
         return None
     inp = _remove_gender(inp)
 
     # fix titles at the end
     if "," not in inp:
         for t in _additional_titles:
             if inp.endswith(t):
@@ -121,26 +137,29 @@
             city = inp.replace(title, "").strip().split(" ")[0]
             if guess_gender.get_gender(city) == 'unknown':
                 title = "{} {} {}".format(title, city, t)
 
     if title is not None and normalize is True:
         title = normalize_title(title)
 
-    return None if title.strip() == "" else title
+    return None if title is None or title.strip() == "" else title
 
 
 def remove_title(inp: str) -> Optional[str]:
     """
-    removes the medic title from a string so the real medic name persists
+    removes the academic title from a string so the real medic name persists
     Args:
         inp: the medic name with title
 
     Returns: only the medic name
     """
-    if inp is None:
+    if type(inp) is not str:
+        return None
+
+    if inp.strip() == "":
         return None
 
     title = person_title(inp, False)
     cleaned_title = person_title(inp)
     if title is not None:
         for t in title.split(" "):
             if len(t) == 1:
@@ -159,15 +178,15 @@
     if inp.endswith(","):
         inp = inp[:-1]
     return inp
 
 
 def _clean_name(inp: str) -> Optional[str]:
     """
-    removes possible nicknames (FH) from the Medic name
+    removes possible nicknames (FH) from the Person name
     """
     if inp is None:
         return None
 
     if ";" in inp:
         inp = inp[0:inp.index(";")]
     if "|" in inp:
@@ -182,15 +201,15 @@
             inp = inp.replace("({})".format(nn), "").replace("  ", " ")
 
     return inp.replace("/ ", " ").replace("  ", " ")
 
 
 def _remove_gender(inp: str) -> Optional[str]:
     """
-    removes Mann|Frau prefixes from the Medic Name
+    removes gender Mann|Frau prefixes from the name
     """
     if inp is None:
         return None
 
     prefixes = ["Herr ", "Herrn ", "Frau ", "Fr. "]
 
     for p in prefixes:
@@ -207,16 +226,19 @@
     Args:
         inp: the full name
     Return: the HumanName object for further work
     """
     if inp is None or inp.strip() == "":
         return None
 
+    if type(inp) is not str:
+        return None
+
     if " " not in inp and "." in inp:
-        #if there are missing spaces, split them up
+        # if there are missing spaces, split them up
         inp = inp.replace(".", ". ")
 
     inp = inp.title()
     # remove gender and title
     inp = _remove_gender(inp)
     inp = remove_title(inp)
 
@@ -282,24 +304,30 @@
     return string
 
 
 def person_name(inp: str) -> Optional[str]:
     """
     extract the person name from "GENDER? TITLE? NAME" strings
     """
+    if type(inp) is not str:
+        return None
+
+    if inp.strip() == "":
+        return None
+
     n = parse_name(inp)
     if n is None:
         return None
 
     return "{} {} {}".format(n.first, n.middle, n.last).replace("  ", " ").strip()
 
 
 def match_name(own: str, other: str) -> bool:
     """
-    compares 2 medic names (respects missing middle names, or abbrev. name parts)
+    compares 2 names (respects missing middle names, or abbrev. name parts)
 
     Args:
         own: the first name
         other: the last name
 
     Returns: True if both names match
     """
@@ -332,15 +360,31 @@
     hn_other.last = " ".join(hn_other.last_list)
     hn_own.last_list = _remove_surname_titles(hn_own.last_list)
     hn_own.last = " ".join(hn_own.last_list)
 
     # if the last names doesnt match, we skip here
     own_lasts = " ".join([on.lower() for on in hn_own.last_list])
     other_lasts = " ".join([on.lower() for on in hn_other.last_list])
-    if own_lasts != other_lasts and distance(own_lasts, other_lasts) > 1:
+
+    # compound surnames
+    if "-" in own_lasts or "-" in other_lasts:
+        own_lasts_splitted = own_lasts.split("-")
+        other_lasts_splitted = other_lasts.split("-")
+        matches = 0
+        for o in own_lasts_splitted:
+            for ot in other_lasts_splitted:
+                if o == ot or distance(o, ot) <= 1 and (len(o) >= 5 or len(ot) >= 5):
+                    matches += 1
+        for o in reversed(own_lasts_splitted):
+            for ot in other_lasts_splitted:
+                if o == ot or distance(o, ot) <= 1 and (len(o) >= 5 or len(ot) >= 5):
+                    matches += 1
+        if matches < 2:
+            return False
+    elif own_lasts[0] != other_lasts[0] or (own_lasts != other_lasts and distance(own_lasts, other_lasts) > 1):
         return False
 
     def _match_name_list(name: str, other: List[str]):
         if name in other:
             # full name match
             return True
         elif name.endswith(".") and name in ["{}.".format(f[0:len(name) - 1]) for f in other]:
@@ -360,19 +404,20 @@
     # check if the firstnames matches (if one side has no firstname we assume a match
     first_name_matches = True if (hn_own.first == "" or hn_other.first == "") else _compare_names(hn_own.first_list,
                                                                                                   hn_other.first_list)
     own_first_middles = hn_own.first + hn_own.middle
     other_first_middles = hn_other.first + hn_other.middle
 
     # check if the firstnames+middlename matches (if one side has no firstname we assume a match
-    first_name_matches_fuzzy = own_first_middles.lower() == other_first_middles.lower() or (own_first_middles.startswith(other_first_middles) or other_first_middles.startswith(own_first_middles))
+    first_name_matches_fuzzy = own_first_middles.lower() == other_first_middles.lower() or (
+                own_first_middles.startswith(other_first_middles) or other_first_middles.startswith(own_first_middles))
 
     if first_name_matches is False or first_name_matches_fuzzy is False:
         # if the initials dont match, dont match
-        if hn_own.first[0] != hn_other.first[0]:
+        if (len(hn_own.first) > 0 and len(hn_own.first) > 0) and hn_own.first[0] != hn_other.first[0]:
             return False
 
         # if the names are longer than 5 and start with the same letter we allow tiny typos
         l_distance = distance(hn_own.first, hn_other.first)
         if l_distance < 2 and (len(hn_other.first) >= 5 or len(hn_own.first) >= 5):
             first_name_matches = True
```

### Comparing `human-name-compare-0.3.9/logger.py` & `human-name-compare-0.4.1/logger.py`

 * *Files identical despite different names*

### Comparing `human-name-compare-0.3.9/README.md` & `human-name-compare-0.4.1/README.md`

 * *Files identical despite different names*

### Comparing `human-name-compare-0.3.9/setup.py` & `human-name-compare-0.4.1/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name='human-name-compare',
-    version='0.3.9',
+    version='0.4.1',
     scripts=['hn-compare'],
     author="Robert Schoenthal",
     author_email="robert.schoenthal@gmail.com",
     description="a tool for comparing human names",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/digitalkaoz/py_human_name_compare",
-    download_url="https://github.com/digitalkaoz/py_human_name_compare/archive/0.3.9.tar.gz",
+    download_url="https://github.com/digitalkaoz/py_human_name_compare/archive/0.4.1.tar.gz",
     packages=['human_name_compare'],
     package_dir={'human_name_compare': 'human_name_compare'},
     keywords=['NLP', 'HUMANNAME'],
     classifiers=[
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent",
```

### Comparing `human-name-compare-0.3.9/human_name_compare.egg-info/PKG-INFO` & `human-name-compare-0.4.1/human_name_compare.egg-info/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,58 +1,58 @@
 Metadata-Version: 2.1
 Name: human-name-compare
-Version: 0.3.9
+Version: 0.4.1
 Summary: a tool for comparing human names
 Home-page: https://github.com/digitalkaoz/py_human_name_compare
+Download-URL: https://github.com/digitalkaoz/py_human_name_compare/archive/0.4.1.tar.gz
 Author: Robert Schoenthal
 Author-email: robert.schoenthal@gmail.com
-License: UNKNOWN
-Download-URL: https://github.com/digitalkaoz/py_human_name_compare/archive/0.3.9.tar.gz
-Description: # Human Name Compare
-        
-        ![human_name_compare](https://github.com/digitalkaoz/py_human_name_compare/workflows/human_name_compare/badge.svg)
-        [![PyPI version](https://badge.fury.io/py/human-name-compare.svg)](https://badge.fury.io/py/human-name-compare)
-        
-        
-        the Problem:
-        
-        Check if `Dr. Peter Müller` and `Peter K. Müller` and `Dr. med. Peter Karsten Müller` and `P. Müller` indicate if its the same person
-        
-        There are gazillion tiny bits and pieces which makes this trivial task hard e.g.:
-        
-        * "R. Schönthal" "Robert Schönthal" - the only have initials on one side
-        * "Erik Schönthal" "Robert Schönthal" - the firstname name doesnt match
-        * "Robert Erik Schönthal" "Robert Peter Schönthal" - the middle name doesnt match 
-        * "Robert-Erik Schönthal" "Robert Erik Schönthal" - we have an "-" in our firstnames
-        * "Robeert Schönthal" "Robert Schönthal" - the firstname has a typo
-        * "Robert Müller" "Robert Schönthal" - the lastname doesnt match
-        * "Herr Robert Müller" "Dr. med. Robert Schönthal" - we have some prefixes
-        
-        and so on...
-        
-        ## Usage
-        
-        ### CLI
-        
-        ```shell script
-        $ hn-compare compare "Robert Schönthal" "Robert Schönthal"
-        ```
-        
-        ### Python
-        
-        ```python
-        from human_name_compare import match_name
-        
-        match_name("Robert Schönthal", "Robert Schönthal")
-        ```
-        
-        ## Tests
-        
-        ````shell script
-        $ python -m pytest .
-        ````
 Keywords: NLP,HUMANNAME
-Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
+License-File: LICENSE.txt
+
+# Human Name Compare
+
+![human_name_compare](https://github.com/digitalkaoz/py_human_name_compare/workflows/human_name_compare/badge.svg)
+[![PyPI version](https://badge.fury.io/py/human-name-compare.svg)](https://badge.fury.io/py/human-name-compare)
+
+
+the Problem:
+
+Check if `Dr. Peter Müller` and `Peter K. Müller` and `Dr. med. Peter Karsten Müller` and `P. Müller` indicate if its the same person
+
+There are gazillion tiny bits and pieces which makes this trivial task hard e.g.:
+
+* "R. Schönthal" "Robert Schönthal" - the only have initials on one side
+* "Erik Schönthal" "Robert Schönthal" - the firstname name doesnt match
+* "Robert Erik Schönthal" "Robert Peter Schönthal" - the middle name doesnt match 
+* "Robert-Erik Schönthal" "Robert Erik Schönthal" - we have an "-" in our firstnames
+* "Robeert Schönthal" "Robert Schönthal" - the firstname has a typo
+* "Robert Müller" "Robert Schönthal" - the lastname doesnt match
+* "Herr Robert Müller" "Dr. med. Robert Schönthal" - we have some prefixes
+
+and so on...
+
+## Usage
+
+### CLI
+
+```shell script
+$ hn-compare compare "Robert Schönthal" "Robert Schönthal"
+```
+
+### Python
+
+```python
+from human_name_compare import match_name
+
+match_name("Robert Schönthal", "Robert Schönthal")
+```
+
+## Tests
+
+````shell script
+$ python -m pytest .
+````
```

