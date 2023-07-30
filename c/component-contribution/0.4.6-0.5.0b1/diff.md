# Comparing `tmp/component-contribution-0.4.6.tar.gz` & `tmp/component-contribution-0.5.0b1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "component-contribution-0.4.6.tar", last modified: Sat Jul 29 14:46:47 2023, max compression
+gzip compressed data, was "component-contribution-0.5.0b1.tar", last modified: Sun Jul 30 10:48:04 2023, max compression
```

## Comparing `component-contribution-0.4.6.tar` & `component-contribution-0.5.0b1.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-29 14:46:47.155337 component-contribution-0.4.6/
--rw-rw-rw-   0 root         (0) root         (0)     1282 2023-07-29 14:46:35.000000 component-contribution-0.4.6/LICENSE
--rw-rw-rw-   0 root         (0) root         (0)      103 2023-07-29 14:46:35.000000 component-contribution-0.4.6/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     3064 2023-07-29 14:46:47.155337 component-contribution-0.4.6/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     1707 2023-07-29 14:46:35.000000 component-contribution-0.4.6/README.md
--rw-rw-rw-   0 root         (0) root         (0)      177 2023-07-29 14:46:35.000000 component-contribution-0.4.6/pyproject.toml
--rw-rw-rw-   0 root         (0) root         (0)     1955 2023-07-29 14:46:47.155337 component-contribution-0.4.6/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)      195 2023-07-29 14:46:35.000000 component-contribution-0.4.6/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-29 14:46:47.149336 component-contribution-0.4.6/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-29 14:46:47.155337 component-contribution-0.4.6/src/component_contribution/
--rw-rw-rw-   0 root         (0) root         (0)     3004 2023-07-29 14:46:35.000000 component-contribution-0.4.6/src/component_contribution/__init__.py
--rw-r--r--   0 root         (0) root         (0)      497 2023-07-29 14:46:47.156337 component-contribution-0.4.6/src/component_contribution/_version.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-29 14:46:47.154337 component-contribution-0.4.6/src/component_contribution/data/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-29 14:46:35.000000 component-contribution-0.4.6/src/component_contribution/data/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     3701 2023-07-29 14:46:35.000000 component-contribution-0.4.6/src/component_contribution/data/toy_training_data.csv
--rw-rw-rw-   0 root         (0) root         (0)     6476 2023-07-29 14:46:35.000000 component-contribution-0.4.6/src/component_contribution/linalg.py
--rw-rw-rw-   0 root         (0) root         (0)     4420 2023-07-29 14:46:35.000000 component-contribution-0.4.6/src/component_contribution/parameters.py
--rw-rw-rw-   0 root         (0) root         (0)    21974 2023-07-29 14:46:35.000000 component-contribution-0.4.6/src/component_contribution/predict.py
--rw-rw-rw-   0 root         (0) root         (0)    13507 2023-07-29 14:46:35.000000 component-contribution-0.4.6/src/component_contribution/preprocessor.py
--rw-rw-rw-   0 root         (0) root         (0)     8724 2023-07-29 14:46:35.000000 component-contribution-0.4.6/src/component_contribution/trainer.py
--rw-rw-rw-   0 root         (0) root         (0)    26829 2023-07-29 14:46:35.000000 component-contribution-0.4.6/src/component_contribution/training_data.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-29 14:46:47.154337 component-contribution-0.4.6/src/component_contribution.egg-info/
--rw-r--r--   0 root         (0) root         (0)     3064 2023-07-29 14:46:47.000000 component-contribution-0.4.6/src/component_contribution.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      788 2023-07-29 14:46:47.000000 component-contribution-0.4.6/src/component_contribution.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-29 14:46:47.000000 component-contribution-0.4.6/src/component_contribution.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      283 2023-07-29 14:46:47.000000 component-contribution-0.4.6/src/component_contribution.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       23 2023-07-29 14:46:47.000000 component-contribution-0.4.6/src/component_contribution.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-29 14:46:47.000000 component-contribution-0.4.6/src/component_contribution.egg-info/zip-safe
--rw-rw-rw-   0 root         (0) root         (0)    68611 2023-07-29 14:46:35.000000 component-contribution-0.4.6/versioneer.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-30 10:48:04.071328 component-contribution-0.5.0b1/
+-rw-rw-rw-   0 root         (0) root         (0)     1282 2023-07-30 10:47:52.000000 component-contribution-0.5.0b1/LICENSE
+-rw-rw-rw-   0 root         (0) root         (0)      103 2023-07-30 10:47:52.000000 component-contribution-0.5.0b1/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     3066 2023-07-30 10:48:04.071328 component-contribution-0.5.0b1/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     1707 2023-07-30 10:47:52.000000 component-contribution-0.5.0b1/README.md
+-rw-rw-rw-   0 root         (0) root         (0)      177 2023-07-30 10:47:52.000000 component-contribution-0.5.0b1/pyproject.toml
+-rw-rw-rw-   0 root         (0) root         (0)     1983 2023-07-30 10:48:04.071328 component-contribution-0.5.0b1/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)      195 2023-07-30 10:47:52.000000 component-contribution-0.5.0b1/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-30 10:48:04.066329 component-contribution-0.5.0b1/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-30 10:48:04.071328 component-contribution-0.5.0b1/src/component_contribution/
+-rw-rw-rw-   0 root         (0) root         (0)     3004 2023-07-30 10:47:52.000000 component-contribution-0.5.0b1/src/component_contribution/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      499 2023-07-30 10:48:04.071328 component-contribution-0.5.0b1/src/component_contribution/_version.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-30 10:48:04.071328 component-contribution-0.5.0b1/src/component_contribution/data/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-30 10:47:52.000000 component-contribution-0.5.0b1/src/component_contribution/data/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     3701 2023-07-30 10:47:52.000000 component-contribution-0.5.0b1/src/component_contribution/data/toy_training_data.csv
+-rw-rw-rw-   0 root         (0) root         (0)     6476 2023-07-30 10:47:52.000000 component-contribution-0.5.0b1/src/component_contribution/linalg.py
+-rw-rw-rw-   0 root         (0) root         (0)     4420 2023-07-30 10:47:52.000000 component-contribution-0.5.0b1/src/component_contribution/parameters.py
+-rw-rw-rw-   0 root         (0) root         (0)    21974 2023-07-30 10:47:52.000000 component-contribution-0.5.0b1/src/component_contribution/predict.py
+-rw-rw-rw-   0 root         (0) root         (0)    13507 2023-07-30 10:47:52.000000 component-contribution-0.5.0b1/src/component_contribution/preprocessor.py
+-rw-rw-rw-   0 root         (0) root         (0)     8724 2023-07-30 10:47:52.000000 component-contribution-0.5.0b1/src/component_contribution/trainer.py
+-rw-rw-rw-   0 root         (0) root         (0)    25505 2023-07-30 10:47:52.000000 component-contribution-0.5.0b1/src/component_contribution/training_data.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-30 10:48:04.070329 component-contribution-0.5.0b1/src/component_contribution.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     3066 2023-07-30 10:48:04.000000 component-contribution-0.5.0b1/src/component_contribution.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      788 2023-07-30 10:48:04.000000 component-contribution-0.5.0b1/src/component_contribution.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-30 10:48:04.000000 component-contribution-0.5.0b1/src/component_contribution.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      309 2023-07-30 10:48:04.000000 component-contribution-0.5.0b1/src/component_contribution.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       23 2023-07-30 10:48:04.000000 component-contribution-0.5.0b1/src/component_contribution.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-30 10:48:04.000000 component-contribution-0.5.0b1/src/component_contribution.egg-info/zip-safe
+-rw-rw-rw-   0 root         (0) root         (0)    68611 2023-07-30 10:47:52.000000 component-contribution-0.5.0b1/versioneer.py
```

### Comparing `component-contribution-0.4.6/LICENSE` & `component-contribution-0.5.0b1/LICENSE`

 * *Files identical despite different names*

### Comparing `component-contribution-0.4.6/PKG-INFO` & `component-contribution-0.5.0b1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: component-contribution
-Version: 0.4.6
+Version: 0.5.0b1
 Summary: Standard reaction Gibbs energy estimation for biochemical reactions.
 Home-page: https://gitlab.com/equilibrator/component-contribution
 Download-URL: https://pypi.org/project/component-contribution/
 Author: Elad Noor, Moritz E. Beber
 Author-email: eladn@weizmann.ac.il, midnighter@posteo.net
 License: MIT
 Project-URL: Source Code, https://gitlab.com/equilibrator/component-contribution
```

### Comparing `component-contribution-0.4.6/README.md` & `component-contribution-0.5.0b1/README.md`

 * *Files identical despite different names*

### Comparing `component-contribution-0.4.6/setup.cfg` & `component-contribution-0.5.0b1/setup.cfg`

 * *Files 12% similar despite different names*

```diff
@@ -29,16 +29,16 @@
 	biochemical reaction
 	eQuilibrator
 	cache
 
 [options]
 zip_safe = True
 install_requires = 
-	equilibrator-cache~=0.4.6
-	path~=16.3
+	equilibrator-cache~=0.5.0b2
+	path~=16.7
 	periodictable~=1.6
 	uncertainties~=3.1
 python_requires = >=3.9
 tests_require = 
 	tox
 packages = find:
 package_dir = 
@@ -53,18 +53,20 @@
 [options.extras_require]
 test = 
 	pytest~=7.0
 	pytest-cov~=3.0
 	pytest-raises~=0.11
 	pytest-mock~=3.7
 development = 
-	black~=22.3
+	black~=23.7
 	isort~=5.12
-	tox~=3.24
-	twine~=3.8
+	flake8~=6.1
+	safety~=2.3
+	tox==3.28
+	twine~=4.0
 deployment = 
 	click
 	click-log
 	python-dateutil
 	requests
 	equilibrator-assets
```

### Comparing `component-contribution-0.4.6/src/component_contribution/__init__.py` & `component-contribution-0.5.0b1/src/component_contribution/__init__.py`

 * *Files identical despite different names*

### Comparing `component-contribution-0.4.6/src/component_contribution/data/toy_training_data.csv` & `component-contribution-0.5.0b1/src/component_contribution/data/toy_training_data.csv`

 * *Files identical despite different names*

### Comparing `component-contribution-0.4.6/src/component_contribution/linalg.py` & `component-contribution-0.5.0b1/src/component_contribution/linalg.py`

 * *Files identical despite different names*

### Comparing `component-contribution-0.4.6/src/component_contribution/parameters.py` & `component-contribution-0.5.0b1/src/component_contribution/parameters.py`

 * *Files 0% similar despite different names*

```diff
@@ -78,15 +78,15 @@
 
         # convert the CCModelParameters object into a dictionary of NumPy
         # arrays. if one of the items is a pandas DataFrames, serialize it to 3
         # separate arrays (values, index, columns)
         param_dict = dict()
         for parameter_name in self._fields:
             parameter_value = self.__getattribute__(parameter_name)
-            if type(parameter_value) == pd.DataFrame:
+            if type(parameter_value) is pd.DataFrame:
                 param_dict[f"{parameter_name}_values"] = parameter_value.values
                 param_dict[f"{parameter_name}_index"] = parameter_value.index
                 param_dict[
                     f"{parameter_name}_columns"
                 ] = parameter_value.columns
             else:
                 param_dict[parameter_name] = parameter_value
```

### Comparing `component-contribution-0.4.6/src/component_contribution/predict.py` & `component-contribution-0.5.0b1/src/component_contribution/predict.py`

 * *Files identical despite different names*

### Comparing `component-contribution-0.4.6/src/component_contribution/preprocessor.py` & `component-contribution-0.5.0b1/src/component_contribution/preprocessor.py`

 * *Files identical despite different names*

### Comparing `component-contribution-0.4.6/src/component_contribution/trainer.py` & `component-contribution-0.5.0b1/src/component_contribution/trainer.py`

 * *Files identical despite different names*

### Comparing `component-contribution-0.4.6/src/component_contribution/training_data.py` & `component-contribution-0.5.0b1/src/component_contribution/training_data.py`

 * *Files 9% similar despite different names*

```diff
@@ -143,16 +143,20 @@
 
         logger.info("Applying reverse Legendre transform on dG' values")
         standard_dg = self._reverse_transform(
             override_ionic_strength=override_ionic_strength,
             override_temperature=override_temperature,
             override_p_mg=override_p_mg,
         )
+        standard_dg = pd.Series(
+            [x.m_as("kJ/mol") for x in standard_dg],
+            index=self.reaction_df.index,
+        ).apply(lambda x: Q_(x, "kJ/mol"))
         self.reaction_df = self.reaction_df.assign(
-            **{"standard_dg": list(standard_dg)}
+            **{"standard_dg": standard_dg}
         )
 
     @property
     def stoichiometric_matrix(self) -> pd.DataFrame:
         """Get the stoichiometric matrix as a DataFrame.
 
         :return: a Pandas DataFrame
@@ -226,15 +230,24 @@
             ("temperature", "[temperature]"),
             ("p_h", None),
             ("p_mg", None),
         ]:
             assert col in self.reaction_df.columns
 
             for v in self.reaction_df[col].values:
-                assert v.check(dim)
+                if pd.isnull(v):
+                    continue
+                try:
+                    assert v.check(
+                        dim
+                    ), f"value {v} in column {col} is not of dimension {dim}"
+                except AttributeError:
+                    raise ValueError(
+                        f"value {v} in column {col} is not a pint Quantity"
+                    )
 
     def _balance_reaction(self, rxn: Reaction) -> Union[Reaction, None]:
         """Try balancing the reaction with H2O and H+.
 
         :param rxn: A Reaction object
         :return: A balanced Reaction, or None
         """
@@ -299,15 +312,15 @@
         self.S.columns = self.reaction_df.index
 
     def _reverse_transform(
         self,
         override_ionic_strength: Optional[Q_] = None,
         override_temperature: Optional[Q_] = None,
         override_p_mg: Optional[Q_] = None,
-    ) -> Iterable[float]:
+    ) -> Iterable[Q_]:
         """Reverse Legendre transform.
 
         Parameters
         ----------
         override_ionic_strength : bool, optional
             If provided, overrides all ionic_strength values given in the data
             files with this value.
@@ -359,23 +372,14 @@
     def parse_formula(self, formula: str) -> Reaction:
         """Parse a chemical formula to create a Reaction object using ccache."""
         result = Reaction.parse_formula(self.ccache.get_compound, formula)
         if None in result.sparse:
             logger.error(formula)
         return result
 
-    def parse_inchi_key_formula(self, formula: str) -> Reaction:
-        """Parse a chemical formula to create a Reaction object using ccache."""
-        result = Reaction.parse_formula(
-            self.ccache.get_compound_by_inchi_key, formula
-        )
-        if None in result.sparse:
-            logger.error(formula)
-        return result
-
 
 class ToyTrainingDataFactory(TrainingDataFactory):
     """Define a factory for toy training data."""
 
     def __init__(self, *, ccache: CompoundCache, **kwargs) -> None:
         """Initialize a factory for creating toy training data sets."""
         super().__init__(ccache=ccache, **kwargs)
@@ -525,39 +529,29 @@
             ("temperature", "K"),
             ("p_h", None),
             ("p_mg", None),
         ]:
             tecr_df[col] = tecr_df[col].apply(Q_, args=(unit,))
 
         # calculate the dG'0 from the Keq and T
-        standard_dg_primes = [
-            (-R * row.temperature * np.log(row.K_prime)).to("kJ/mol")
-            for row in tecr_df.itertuples()
-        ]
+        standard_dg_primes = pd.Series(
+            [
+                (-R * row.temperature * np.log(row.K_prime)).m_as("kJ/mol")
+                for row in tecr_df.itertuples()
+            ]
+        ).apply(lambda x: Q_(x, "kJ/mol"))
         tecr_df = tecr_df.assign(
             **{"standard_dg_prime": standard_dg_primes, "balance": True}
         )
 
         # parse the reaction
-        mask = tecr_df["reaction_inchi_key"].notnull()
-        logger.info(
-            f"Parsing {mask.sum()}/{len(mask)} reactions with InChIKeys."
-        )
-        tecr_df.loc[mask, "reaction"] = [
-            self.parse_inchi_key_formula(rxn)
-            for rxn in tqdm(
-                tecr_df.loc[mask, "reaction_inchi_key"], desc="Parsing Reaction"
-            )
-        ]
-        logger.info(f"Parsing {(~mask).sum()}/{len(mask)} remaining reactions.")
-        tecr_df.loc[~mask, "reaction"] = [
+        logger.info(f"Parsing {tecr_df.shape[0]} reactions.")
+        tecr_df.loc[:, "reaction"] = [
             self.parse_formula(rxn)
-            for rxn in tqdm(
-                tecr_df.loc[~mask, "reaction"], desc="Parsing Reaction"
-            )
+            for rxn in tqdm(tecr_df.loc[:, "reaction"], desc="Parsing Reaction")
         ]
 
         # skip reactions that could not be parsed
         tecr_df = tecr_df[~pd.isnull(tecr_df["reaction"])]
 
         tecr_df.drop(
             ["url", "method", "K", "K_prime", "eval", "EC", "enzyme_name"],
@@ -579,31 +573,19 @@
 
         :return: a 2-tuple of the Pandas DataFrame of reactions, and the set
         of compounds that do not decompose into groups.
         """
         formation_df = pd.read_csv(formation_file)
         compounds = pd.Series(index=formation_df.index, dtype=object)
 
-        mask = formation_df["inchi_key"].notnull()
-        logger.info(
-            "Parsing %d/%d compounds with InChIKey.", mask.sum(), len(mask)
-        )
-        compounds[mask] = formation_df.loc[mask, "inchi_key"].apply(
-            self.ccache.get_compound_by_inchi_key
-        )
-
-        logger.info("Parsing %d remaining compounds.", (~mask).sum())
-        compounds[~mask] = formation_df.loc[~mask, "cid"].apply(
-            self.ccache.get_compound
-        )
+        logger.info("Parsing %d compounds.", formation_df.shape[0])
+        compounds = formation_df.loc[:, "cid"].apply(self.ccache.get_compound)
 
         if compounds.isnull().any():
-            missing_cids = formation_df.loc[
-                compounds.isnull(), ["cid", "inchi_key"]
-            ]
+            missing_cids = formation_df.loc[compounds.isnull(), ["cid"]]
             raise ParseException(
                 "Cannot find some of the compounds in the "
                 "cache: " + str(missing_cids)
             )
 
         compounds_that_do_not_decompose = set(
             compounds.loc[formation_df.decompose == 0].values
@@ -630,15 +612,15 @@
                     lambda c: Reaction({c: 1})
                 ),
                 "balance": False,
                 "description": formation_df["name"] + " formation",
             }
         )
         formation_df.drop(
-            ["name", "cid", "remark", "decompose", "inchi_key"],
+            ["name", "cid", "remark", "decompose"],
             axis=1,
             inplace=True,
         )
 
         logger.info(
             "Successfully added %d formation energies", formation_df.shape[0]
         )
@@ -662,53 +644,31 @@
             ("temperature", "K"),
             ("p_h", None),
             ("p_mg", None),
         ]:
             redox_df[col] = redox_df[col].apply(Q_, args=(unit,))
 
         compounds_ox = pd.Series(index=redox_df.index, dtype=object)
-        mask = redox_df["inchi_key_ox"].notnull()
-        logger.info(
-            "Parsing %d/%d oxidized compounds with InChIKey.",
-            mask.sum(),
-            len(mask),
-        )
-        compounds_ox[mask] = redox_df.loc[mask, "inchi_key_ox"].apply(
-            self.ccache.get_compound_by_inchi_key
-        )
-        logger.info("Parsing %d remaining oxidized compounds.", (~mask).sum())
-        compounds_ox[~mask] = redox_df.loc[~mask, "CID_ox"].apply(
-            self.ccache.get_compound
-        )
+        logger.info("Parsing %d oxidized compounds.", redox_df.shape[0])
+        compounds_ox = redox_df.loc[:, "CID_ox"].apply(self.ccache.get_compound)
         if compounds_ox.isnull().any():
-            exceptions = redox_df.loc[
-                compounds_ox.isnull(), ["name", "CID_ox", "inchi_key_ox"]
-            ]
+            exceptions = redox_df.loc[compounds_ox.isnull(), ["name", "CID_ox"]]
             raise ParseException(
                 f"Failed to find the following compounds in the cache:\n"
                 f"{exceptions}"
             )
 
         compounds_red = pd.Series(index=redox_df.index, dtype=object)
-        mask = redox_df["inchi_key_red"].notnull()
-        logger.info(
-            "Parsing %d/%d reduced compounds with InChIKey.",
-            mask.sum(),
-            len(mask),
-        )
-        compounds_red[mask] = redox_df.loc[mask, "inchi_key_red"].apply(
-            self.ccache.get_compound_by_inchi_key
-        )
-        logger.info("Parsing %d remaining reduced compounds.", (~mask).sum())
-        compounds_red[~mask] = redox_df.loc[~mask, "CID_red"].apply(
+        logger.info("Parsing %d reduced compounds.", redox_df.shape[0])
+        compounds_red = redox_df.loc[:, "CID_red"].apply(
             self.ccache.get_compound
         )
         if compounds_red.isnull().any():
             exceptions = redox_df.loc[
-                compounds_red.isnull(), ["name", "CID_red", "inchi_key_red"]
+                compounds_red.isnull(), ["name", "CID_red"]
             ]
             raise ParseException(
                 f"Failed to find the following compounds in the cache:\n"
                 f"{exceptions}"
             )
 
         compounds_that_do_not_decompose = set(
```

### Comparing `component-contribution-0.4.6/src/component_contribution.egg-info/PKG-INFO` & `component-contribution-0.5.0b1/src/component_contribution.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: component-contribution
-Version: 0.4.6
+Version: 0.5.0b1
 Summary: Standard reaction Gibbs energy estimation for biochemical reactions.
 Home-page: https://gitlab.com/equilibrator/component-contribution
 Download-URL: https://pypi.org/project/component-contribution/
 Author: Elad Noor, Moritz E. Beber
 Author-email: eladn@weizmann.ac.il, midnighter@posteo.net
 License: MIT
 Project-URL: Source Code, https://gitlab.com/equilibrator/component-contribution
```

### Comparing `component-contribution-0.4.6/src/component_contribution.egg-info/SOURCES.txt` & `component-contribution-0.5.0b1/src/component_contribution.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `component-contribution-0.4.6/versioneer.py` & `component-contribution-0.5.0b1/versioneer.py`

 * *Files identical despite different names*

