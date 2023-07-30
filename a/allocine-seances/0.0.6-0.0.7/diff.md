# Comparing `tmp/allocine-seances-0.0.6.tar.gz` & `tmp/allocine-seances-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "allocine-seances-0.0.6.tar", last modified: Sat Jul 22 12:55:18 2023, max compression
+gzip compressed data, was "allocine-seances-0.0.7.tar", last modified: Sun Jul 30 17:45:33 2023, max compression
```

## Comparing `allocine-seances-0.0.6.tar` & `allocine-seances-0.0.7.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2023-07-22 12:55:18.817734 allocine-seances-0.0.6/
--rw-rw-rw-   0        0        0     1088 2023-04-15 16:16:47.000000 allocine-seances-0.0.6/LICENSE
--rw-rw-rw-   0        0        0     4607 2023-07-22 12:55:18.815214 allocine-seances-0.0.6/PKG-INFO
--rw-rw-rw-   0        0        0     2779 2023-04-15 18:32:35.000000 allocine-seances-0.0.6/README.md
--rw-rw-rw-   0        0        0      721 2023-07-22 12:55:01.000000 allocine-seances-0.0.6/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-07-22 12:55:18.818737 allocine-seances-0.0.6/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-07-22 12:55:18.783983 allocine-seances-0.0.6/src/
-drwxrwxrwx   0        0        0        0 2023-07-22 12:55:18.790511 allocine-seances-0.0.6/src/allocineAPI/
--rw-rw-rw-   0        0        0        0 2023-04-15 16:02:27.000000 allocine-seances-0.0.6/src/allocineAPI/__init__.py
--rw-rw-rw-   0        0        0     9755 2023-07-22 12:52:52.000000 allocine-seances-0.0.6/src/allocineAPI/allocineAPI.py
-drwxrwxrwx   0        0        0        0 2023-07-22 12:55:18.813210 allocine-seances-0.0.6/src/allocine_seances.egg-info/
--rw-rw-rw-   0        0        0     4607 2023-07-22 12:55:18.000000 allocine-seances-0.0.6/src/allocine_seances.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      310 2023-07-22 12:55:18.000000 allocine-seances-0.0.6/src/allocine_seances.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-22 12:55:18.000000 allocine-seances-0.0.6/src/allocine_seances.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       15 2023-07-22 12:55:18.000000 allocine-seances-0.0.6/src/allocine_seances.egg-info/requires.txt
--rw-rw-rw-   0        0        0       12 2023-07-22 12:55:18.000000 allocine-seances-0.0.6/src/allocine_seances.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-30 17:45:33.438221 allocine-seances-0.0.7/
+-rw-rw-rw-   0        0        0     1088 2023-04-15 16:16:47.000000 allocine-seances-0.0.7/LICENSE
+-rw-rw-rw-   0        0        0     4693 2023-07-30 17:45:33.438221 allocine-seances-0.0.7/PKG-INFO
+-rw-rw-rw-   0        0        0     2865 2023-07-30 17:43:56.000000 allocine-seances-0.0.7/README.md
+-rw-rw-rw-   0        0        0      721 2023-07-30 17:43:56.000000 allocine-seances-0.0.7/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-07-30 17:45:33.438221 allocine-seances-0.0.7/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-07-30 17:45:33.418152 allocine-seances-0.0.7/src/
+drwxrwxrwx   0        0        0        0 2023-07-30 17:45:33.425650 allocine-seances-0.0.7/src/allocineAPI/
+-rw-rw-rw-   0        0        0        0 2023-04-15 16:02:27.000000 allocine-seances-0.0.7/src/allocineAPI/__init__.py
+-rw-rw-rw-   0        0        0     9743 2023-07-30 17:37:20.000000 allocine-seances-0.0.7/src/allocineAPI/allocineAPI.py
+drwxrwxrwx   0        0        0        0 2023-07-30 17:45:33.438221 allocine-seances-0.0.7/src/allocine_seances.egg-info/
+-rw-rw-rw-   0        0        0     4693 2023-07-30 17:45:33.000000 allocine-seances-0.0.7/src/allocine_seances.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      310 2023-07-30 17:45:33.000000 allocine-seances-0.0.7/src/allocine_seances.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-30 17:45:33.000000 allocine-seances-0.0.7/src/allocine_seances.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       15 2023-07-30 17:45:33.000000 allocine-seances-0.0.7/src/allocine_seances.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       12 2023-07-30 17:45:33.000000 allocine-seances-0.0.7/src/allocine_seances.egg-info/top_level.txt
```

### Comparing `allocine-seances-0.0.6/LICENSE` & `allocine-seances-0.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `allocine-seances-0.0.6/PKG-INFO` & `allocine-seances-0.0.7/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: allocine-seances
-Version: 0.0.6
+Version: 0.0.7
 Summary: Récupération des scéances de cinémas sur allociné
 Author-email: lefevre-dev <louislefevre.dev@gmail.com>
 License: MIT License
         
         Copyright (c) [year] [fullname]
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -29,16 +29,22 @@
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
+# Package
+https://pypi.org/project/allocine-seances/
+```
+pip install allocine-seances
+```
+
 # Description
-<ins>Objectif</ins> : récupération des horaires des séances de cinéma.
+Objectif : récupération des horaires des séances de cinéma.
 
 Les méthodes ```get_top_villes()```, ```get_departements()``` et ```get_circuit()``` retournent un id d’emplacement.
 
 La méthode ```get_cinema(id_location)``` retourne un id de cinéma pour un emplacement donné.
 
 La méthode ```get_showtime(id_cinema, day_shift)``` retourne la liste des séances pour un cinema donné et un jour. le paramètre day_shift (entier positif) représente le décalage en jour par rapport à la date actuelle.
```

### Comparing `allocine-seances-0.0.6/README.md` & `allocine-seances-0.0.7/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -1,9 +1,15 @@
+# Package
+https://pypi.org/project/allocine-seances/
+```
+pip install allocine-seances
+```
+
 # Description
-<ins>Objectif</ins> : récupération des horaires des séances de cinéma.
+Objectif : récupération des horaires des séances de cinéma.
 
 Les méthodes ```get_top_villes()```, ```get_departements()``` et ```get_circuit()``` retournent un id d’emplacement.
 
 La méthode ```get_cinema(id_location)``` retourne un id de cinéma pour un emplacement donné.
 
 La méthode ```get_showtime(id_cinema, day_shift)``` retourne la liste des séances pour un cinema donné et un jour. le paramètre day_shift (entier positif) représente le décalage en jour par rapport à la date actuelle.
```

### Comparing `allocine-seances-0.0.6/pyproject.toml` & `allocine-seances-0.0.7/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "allocine-seances"
-version = "0.0.6"
+version = "0.0.7"
 authors = [
   { name="lefevre-dev", email="louislefevre.dev@gmail.com" },
 ]
 description = "Récupération des scéances de cinémas sur allociné"
 readme = "README.md"
 requires-python = ">=3.7"
 license = { file = "LICENSE" }
```

### Comparing `allocine-seances-0.0.6/src/allocineAPI/allocineAPI.py` & `allocine-seances-0.0.7/src/allocineAPI/allocineAPI.py`

 * *Files 6% similar despite different names*

```diff
@@ -170,28 +170,27 @@
                     lst_internal_ids.append(element["movie"]["internalId"])
                     title = element["movie"]["title"]
                     originalTitle = element["movie"]["originalTitle"]
                     synopsisFull = element["movie"]["synopsisFull"]
                     urlPoster = element["movie"]["poster"]["url"]
                     runtime = element["movie"]["runtime"]
                     languages = list(element["movie"]["languages"])
-                    if element["movie"]["releases"][0]["releaseDate"] is not None:
-                        releaseDate = element["movie"]["releases"][0]["releaseDate"]["date"]
-                    else:
-                        releaseDate = ""
                     hasDvdRelease = element["movie"]["flags"]["hasDvdRelease"]
+                    isPremiere = element["movie"]["customFlags"]["isPremiere"]
+                    weeklyOuting = element["movie"]["customFlags"]["weeklyOuting"]
                     formated_data.append({
                         "title": title,
                         "originalTitle": originalTitle,
                         "synopsisFull": synopsisFull,
                         "urlPoster": urlPoster,
                         "runtime": runtime,
                         "languages": languages,
-                        "releaseDate": releaseDate,
-                        "hasDvdRelease": hasDvdRelease
+                        "hasDvdRelease": hasDvdRelease,
+                        "isPremiere": isPremiere,
+                        "weeklyOuting": weeklyOuting
                     })
         return formated_data
 
 
 class URLs:
     BASE_URL = "https://www.allocine.fr/"
     SEANCES = "salle/"
@@ -213,15 +212,15 @@
     def showtime_url(id_cinema, day_shift, page):
         return URLs.BASE_URL + URLs.SHOWTIMES + id_cinema + "/d-" + str(day_shift) + "/p-" + str(page)
 
 
 if __name__ == '__main__':
     api = allocineAPI()
 
-    films = api.get_movies('P0671')  # Film cité international aujourd'hui
+    films = api.get_movies('P0671', verbose_url=True)  # Film cité international aujourd'hui
     for film in films:
         print(film)
 
     print("\n")
 
     films = api.get_movies('P0671', day_shift=1)  # Film cité international demain
     for film in films:
```

### Comparing `allocine-seances-0.0.6/src/allocine_seances.egg-info/PKG-INFO` & `allocine-seances-0.0.7/src/allocine_seances.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: allocine-seances
-Version: 0.0.6
+Version: 0.0.7
 Summary: Récupération des scéances de cinémas sur allociné
 Author-email: lefevre-dev <louislefevre.dev@gmail.com>
 License: MIT License
         
         Copyright (c) [year] [fullname]
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -29,16 +29,22 @@
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
+# Package
+https://pypi.org/project/allocine-seances/
+```
+pip install allocine-seances
+```
+
 # Description
-<ins>Objectif</ins> : récupération des horaires des séances de cinéma.
+Objectif : récupération des horaires des séances de cinéma.
 
 Les méthodes ```get_top_villes()```, ```get_departements()``` et ```get_circuit()``` retournent un id d’emplacement.
 
 La méthode ```get_cinema(id_location)``` retourne un id de cinéma pour un emplacement donné.
 
 La méthode ```get_showtime(id_cinema, day_shift)``` retourne la liste des séances pour un cinema donné et un jour. le paramètre day_shift (entier positif) représente le décalage en jour par rapport à la date actuelle.
```

