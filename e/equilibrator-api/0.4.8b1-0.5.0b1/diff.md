# Comparing `tmp/equilibrator-api-0.4.8b1.tar.gz` & `tmp/equilibrator-api-0.5.0b1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "equilibrator-api-0.4.8b1.tar", last modified: Sun Jul  2 09:01:36 2023, max compression
+gzip compressed data, was "equilibrator-api-0.5.0b1.tar", last modified: Sun Jul 30 12:15:52 2023, max compression
```

## Comparing `equilibrator-api-0.4.8b1.tar` & `equilibrator-api-0.5.0b1.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-02 09:01:36.081604 equilibrator-api-0.4.8b1/
--rw-rw-rw-   0 root         (0) root         (0)     1311 2023-07-02 09:01:24.000000 equilibrator-api-0.4.8b1/LICENSE
--rw-rw-rw-   0 root         (0) root         (0)       97 2023-07-02 09:01:24.000000 equilibrator-api-0.4.8b1/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     4732 2023-07-02 09:01:36.081604 equilibrator-api-0.4.8b1/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     3302 2023-07-02 09:01:24.000000 equilibrator-api-0.4.8b1/README.md
--rw-rw-rw-   0 root         (0) root         (0)      177 2023-07-02 09:01:24.000000 equilibrator-api-0.4.8b1/pyproject.toml
--rw-rw-rw-   0 root         (0) root         (0)     1992 2023-07-02 09:01:36.081604 equilibrator-api-0.4.8b1/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)      195 2023-07-02 09:01:24.000000 equilibrator-api-0.4.8b1/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-02 09:01:36.075604 equilibrator-api-0.4.8b1/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-02 09:01:36.082604 equilibrator-api-0.4.8b1/src/equilibrator_api/
--rw-rw-rw-   0 root         (0) root         (0)     2180 2023-07-02 09:01:24.000000 equilibrator-api-0.4.8b1/src/equilibrator_api/__init__.py
--rw-r--r--   0 root         (0) root         (0)      499 2023-07-02 09:01:36.082604 equilibrator-api-0.4.8b1/src/equilibrator_api/_version.py
--rw-rw-rw-   0 root         (0) root         (0)     3047 2023-07-02 09:01:24.000000 equilibrator-api-0.4.8b1/src/equilibrator_api/compatibility.py
--rw-rw-rw-   0 root         (0) root         (0)    34583 2023-07-02 09:01:24.000000 equilibrator-api-0.4.8b1/src/equilibrator_api/component_contribution.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-02 09:01:36.080604 equilibrator-api-0.4.8b1/src/equilibrator_api/data/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-02 09:01:24.000000 equilibrator-api-0.4.8b1/src/equilibrator_api/data/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     4237 2023-07-02 09:01:24.000000 equilibrator-api-0.4.8b1/src/equilibrator_api/data/cofactors.csv
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-02 09:01:36.081604 equilibrator-api-0.4.8b1/src/equilibrator_api/model/
--rw-rw-rw-   0 root         (0) root         (0)     2171 2023-07-02 09:01:24.000000 equilibrator-api-0.4.8b1/src/equilibrator_api/model/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    10479 2023-07-02 09:01:24.000000 equilibrator-api-0.4.8b1/src/equilibrator_api/model/bounds.py
--rw-rw-rw-   0 root         (0) root         (0)    34592 2023-07-02 09:01:24.000000 equilibrator-api-0.4.8b1/src/equilibrator_api/model/model.py
--rw-rw-rw-   0 root         (0) root         (0)    18294 2023-07-02 09:01:24.000000 equilibrator-api-0.4.8b1/src/equilibrator_api/phased_compound.py
--rw-rw-rw-   0 root         (0) root         (0)    15969 2023-07-02 09:01:24.000000 equilibrator-api-0.4.8b1/src/equilibrator_api/phased_reaction.py
--rw-rw-rw-   0 root         (0) root         (0)     4154 2023-07-02 09:01:24.000000 equilibrator-api-0.4.8b1/src/equilibrator_api/reaction_parser.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-02 09:01:36.080604 equilibrator-api-0.4.8b1/src/equilibrator_api.egg-info/
--rw-r--r--   0 root         (0) root         (0)     4732 2023-07-02 09:01:36.000000 equilibrator-api-0.4.8b1/src/equilibrator_api.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      796 2023-07-02 09:01:36.000000 equilibrator-api-0.4.8b1/src/equilibrator_api.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-02 09:01:36.000000 equilibrator-api-0.4.8b1/src/equilibrator_api.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      292 2023-07-02 09:01:36.000000 equilibrator-api-0.4.8b1/src/equilibrator_api.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       17 2023-07-02 09:01:36.000000 equilibrator-api-0.4.8b1/src/equilibrator_api.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-02 09:01:36.000000 equilibrator-api-0.4.8b1/src/equilibrator_api.egg-info/zip-safe
--rw-rw-rw-   0 root         (0) root         (0)    68615 2023-07-02 09:01:24.000000 equilibrator-api-0.4.8b1/versioneer.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-30 12:15:52.723698 equilibrator-api-0.5.0b1/
+-rw-rw-rw-   0 root         (0) root         (0)     1311 2023-07-30 12:15:41.000000 equilibrator-api-0.5.0b1/LICENSE
+-rw-rw-rw-   0 root         (0) root         (0)       97 2023-07-30 12:15:41.000000 equilibrator-api-0.5.0b1/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     4633 2023-07-30 12:15:52.724698 equilibrator-api-0.5.0b1/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     3302 2023-07-30 12:15:41.000000 equilibrator-api-0.5.0b1/README.md
+-rw-rw-rw-   0 root         (0) root         (0)      177 2023-07-30 12:15:41.000000 equilibrator-api-0.5.0b1/pyproject.toml
+-rw-rw-rw-   0 root         (0) root         (0)     1931 2023-07-30 12:15:52.724698 equilibrator-api-0.5.0b1/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)      195 2023-07-30 12:15:41.000000 equilibrator-api-0.5.0b1/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-30 12:15:52.717698 equilibrator-api-0.5.0b1/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-30 12:15:52.724698 equilibrator-api-0.5.0b1/src/equilibrator_api/
+-rw-rw-rw-   0 root         (0) root         (0)     2180 2023-07-30 12:15:41.000000 equilibrator-api-0.5.0b1/src/equilibrator_api/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      499 2023-07-30 12:15:52.724698 equilibrator-api-0.5.0b1/src/equilibrator_api/_version.py
+-rw-rw-rw-   0 root         (0) root         (0)     3047 2023-07-30 12:15:41.000000 equilibrator-api-0.5.0b1/src/equilibrator_api/compatibility.py
+-rw-rw-rw-   0 root         (0) root         (0)    35662 2023-07-30 12:15:41.000000 equilibrator-api-0.5.0b1/src/equilibrator_api/component_contribution.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-30 12:15:52.723698 equilibrator-api-0.5.0b1/src/equilibrator_api/data/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-30 12:15:41.000000 equilibrator-api-0.5.0b1/src/equilibrator_api/data/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     4237 2023-07-30 12:15:41.000000 equilibrator-api-0.5.0b1/src/equilibrator_api/data/cofactors.csv
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-30 12:15:52.723698 equilibrator-api-0.5.0b1/src/equilibrator_api/model/
+-rw-rw-rw-   0 root         (0) root         (0)     2171 2023-07-30 12:15:41.000000 equilibrator-api-0.5.0b1/src/equilibrator_api/model/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    10479 2023-07-30 12:15:41.000000 equilibrator-api-0.5.0b1/src/equilibrator_api/model/bounds.py
+-rw-rw-rw-   0 root         (0) root         (0)    34576 2023-07-30 12:15:41.000000 equilibrator-api-0.5.0b1/src/equilibrator_api/model/model.py
+-rw-rw-rw-   0 root         (0) root         (0)    18294 2023-07-30 12:15:41.000000 equilibrator-api-0.5.0b1/src/equilibrator_api/phased_compound.py
+-rw-rw-rw-   0 root         (0) root         (0)    15969 2023-07-30 12:15:41.000000 equilibrator-api-0.5.0b1/src/equilibrator_api/phased_reaction.py
+-rw-rw-rw-   0 root         (0) root         (0)     4154 2023-07-30 12:15:41.000000 equilibrator-api-0.5.0b1/src/equilibrator_api/reaction_parser.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-30 12:15:52.722698 equilibrator-api-0.5.0b1/src/equilibrator_api.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     4633 2023-07-30 12:15:52.000000 equilibrator-api-0.5.0b1/src/equilibrator_api.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      796 2023-07-30 12:15:52.000000 equilibrator-api-0.5.0b1/src/equilibrator_api.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-30 12:15:52.000000 equilibrator-api-0.5.0b1/src/equilibrator_api.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      307 2023-07-30 12:15:52.000000 equilibrator-api-0.5.0b1/src/equilibrator_api.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       17 2023-07-30 12:15:52.000000 equilibrator-api-0.5.0b1/src/equilibrator_api.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-30 12:15:52.000000 equilibrator-api-0.5.0b1/src/equilibrator_api.egg-info/zip-safe
+-rw-rw-rw-   0 root         (0) root         (0)    68615 2023-07-30 12:15:41.000000 equilibrator-api-0.5.0b1/versioneer.py
```

### Comparing `equilibrator-api-0.4.8b1/LICENSE` & `equilibrator-api-0.5.0b1/LICENSE`

 * *Files identical despite different names*

### Comparing `equilibrator-api-0.4.8b1/PKG-INFO` & `equilibrator-api-0.5.0b1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: equilibrator-api
-Version: 0.4.8b1
+Version: 0.5.0b1
 Summary: Calculation of standard thermodynamic potentials of biochemical reactions.
 Home-page: https://gitlab.com/equilibrator/equilibrator-api/
 Download-URL: https://pypi.org/project/equilibrator-api/
 Author: Elad Noor, Moritz E. Beber
 Author-email: eladn@weizmann.ac.il, midnighter@posteo.net
 License: MIT
 Project-URL: Source Code, https://gitlab.com/equilibrator/equilibrator-api/
@@ -12,22 +12,20 @@
 Keywords: component contribution,Gibbs energy,biochemical reaction,eQuilibrator
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3 :: Only
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Scientific/Engineering :: Bio-Informatics
 Classifier: Topic :: Scientific/Engineering :: Chemistry
-Requires-Python: >=3.6
+Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 Provides-Extra: test
 Provides-Extra: development
 Provides-Extra: deployment
 License-File: LICENSE
 
 # eQuilibrator - a thermodynamics calculator for biochemical reactions
```

### Comparing `equilibrator-api-0.4.8b1/README.md` & `equilibrator-api-0.5.0b1/README.md`

 * *Files identical despite different names*

### Comparing `equilibrator-api-0.4.8b1/setup.cfg` & `equilibrator-api-0.5.0b1/setup.cfg`

 * *Files 9% similar despite different names*

```diff
@@ -10,19 +10,17 @@
 classifiers = 
 	Development Status :: 4 - Beta
 	Intended Audience :: Science/Research
 	License :: OSI Approved :: MIT License
 	Natural Language :: English
 	Operating System :: OS Independent
 	Programming Language :: Python :: 3 :: Only
-	Programming Language :: Python :: 3.6
-	Programming Language :: Python :: 3.7
-	Programming Language :: Python :: 3.8
 	Programming Language :: Python :: 3.9
 	Programming Language :: Python :: 3.10
+	Programming Language :: Python :: 3.11
 	Topic :: Scientific/Engineering :: Bio-Informatics
 	Topic :: Scientific/Engineering :: Chemistry
 license = MIT
 description = Calculation of standard thermodynamic potentials of biochemical reactions.
 long_description = file: README.md
 long_description_content_type = text/markdown
 keywords = 
@@ -32,17 +30,17 @@
 	eQuilibrator
 
 [options]
 zip_safe = True
 install_requires = 
 	pyparsing~=3.0
 	python-slugify~=5.0
-	equilibrator-cache~=0.4.3
-	component-contribution~=0.4.4
-python_requires = >=3.6
+	equilibrator-cache~=0.5.0b2
+	component-contribution~=0.5.0b1
+python_requires = >=3.9
 tests_require = 
 	tox
 packages = find:
 package_dir = 
 	= src
 
 [options.packages.find]
@@ -53,19 +51,20 @@
 	cobra
 	pytest
 	pytest-cov
 	pytest-raises
 	pytest-allclose
 	sbtab~=1.0
 development = 
-	black~=22.1
-	isort~=5.10
-	safety~=1.10
-	tox~=3.24
-	twine~=3.8
+	black~=23.7
+	isort~=5.12
+	flake8~=6.1
+	safety~=2.3
+	tox==3.28
+	twine~=4.0
 deployment = 
 	click
 	click-log
 	python-dateutil
 	requests
 
 [options.package_data]
```

### Comparing `equilibrator-api-0.4.8b1/src/equilibrator_api/__init__.py` & `equilibrator-api-0.5.0b1/src/equilibrator_api/__init__.py`

 * *Files identical despite different names*

### Comparing `equilibrator-api-0.4.8b1/src/equilibrator_api/compatibility.py` & `equilibrator-api-0.5.0b1/src/equilibrator_api/compatibility.py`

 * *Files identical despite different names*

### Comparing `equilibrator-api-0.4.8b1/src/equilibrator_api/component_contribution.py` & `equilibrator-api-0.5.0b1/src/equilibrator_api/component_contribution.py`

 * *Files 2% similar despite different names*

```diff
@@ -225,15 +225,15 @@
 
     @staticmethod
     def initialize_custom_version(
         rmse_inf: Q_ = default_rmse_inf,
         ccache_settings: ZenodoSettings = DEFAULT_COMPOUND_CACHE_SETTINGS,
         cc_params_settings: ZenodoSettings = DEFAULT_CC_PARAMS_SETTINGS,
     ) -> "ComponentContribution":
-        """Initialize a ComponentContribution object with custom Zenodo versions.
+        """Initialize ComponentContribution object with custom Zenodo versions.
 
         Parameters
         ----------
         rmse_inf : Quantity, optional
             Set the factor by which to multiply the error
             covariance matrix for reactions outside the span of
             Component Contribution.
@@ -613,15 +613,15 @@
             # at the same time minimizes the norm2 of the estimate vector.
             _, _, _, P_N = LINALG.invert_project(X.T)
             standard_dg_prime = P_N @ standard_dg_prime
 
         return standard_dg_prime, dg_uncertainty
 
     def physiological_dg_prime(self, reaction: PhasedReaction) -> ureg.Measurement:
-        """Calculate the dG'm of a single reaction.
+        r"""Calculate the dG'm of a single reaction.
 
         Assume all aqueous reactants are at 1 mM, gas reactants at 1 mbar and
         the rest at their standard concentration.
 
         Returns
         -------
         standard_dg_primes : ndarray
@@ -635,16 +635,48 @@
             sampling (where 'standard_dg_primes' is the mean of that Gaussian).
         """
         return (
             self.standard_dg_prime(reaction)
             + self.RT * reaction.physiological_dg_correction()
         )
 
+    def dgf_prime_sensitivity_to_p_h(self, compound: Compound) -> ureg.Quantity:
+        r"""Calculate the sensitivity of the chemical formation energy to pH.
+
+        Returns
+        -------
+        Quantity
+            The derivative of :math:`\Delta G_f` with respect to pH, in kJ/mol.
+        """
+        return self.predictor.dgf_prime_sensitivity_to_p_h(
+            compound,
+            p_h=self.p_h,
+            p_mg=self.p_mg,
+            ionic_strength=self.ionic_strength,
+            temperature=self.temperature,
+        )
+
+    def dg_prime_sensitivity_to_p_h(self, reaction: PhasedReaction) -> ureg.Quantity:
+        r"""Calculate the sensitivity of the chemical reaction energy to pH.
+
+        Returns
+        -------
+        Quantity
+            The derivative of :math:`\Delta G_r` with respect to pH, in kJ/mol.
+        """
+        return self.predictor.dg_prime_sensitivity_to_p_h(
+            reaction,
+            p_h=self.p_h,
+            p_mg=self.p_mg,
+            ionic_strength=self.ionic_strength,
+            temperature=self.temperature,
+        )
+
     def ln_reversibility_index(self, reaction: PhasedReaction) -> ureg.Measurement:
-        """Calculate the reversibility index (ln Gamma) of a single reaction.
+        r"""Calculate the reversibility index (ln Gamma) of a single reaction.
 
         Returns
         -------
         ln_RI : ureg.Measurement
             the reversibility index (in natural log scale).
         """
         physiological_dg_prime = self.physiological_dg_prime(reaction)
```

### Comparing `equilibrator-api-0.4.8b1/src/equilibrator_api/data/cofactors.csv` & `equilibrator-api-0.5.0b1/src/equilibrator_api/data/cofactors.csv`

 * *Files identical despite different names*

### Comparing `equilibrator-api-0.4.8b1/src/equilibrator_api/model/__init__.py` & `equilibrator-api-0.5.0b1/src/equilibrator_api/model/__init__.py`

 * *Files identical despite different names*

### Comparing `equilibrator-api-0.4.8b1/src/equilibrator_api/model/bounds.py` & `equilibrator-api-0.5.0b1/src/equilibrator_api/model/bounds.py`

 * *Files identical despite different names*

### Comparing `equilibrator-api-0.4.8b1/src/equilibrator_api/model/model.py` & `equilibrator-api-0.5.0b1/src/equilibrator_api/model/model.py`

 * *Files 0% similar despite different names*

```diff
@@ -374,27 +374,27 @@
         """
         return np.array(
             list(map(float, self._bounds.get_ln_upper_bounds(self.compounds)))
         )
 
     @property
     def ln_conc_mu(self) -> np.array:
-        """Get the mean of the log concentration distribution based on the bounds.
+        """Get mean of log concentration distribution based on the bounds.
 
         The order of compounds is according to the stoichiometric matrix index.
 
         Returns
         -------
         a NumPy array with the mean of the log concentrations
         """
         return (self.ln_conc_ub + self.ln_conc_lb) / 2.0
 
     @property
     def ln_conc_sigma(self) -> np.array:
-        """Get the stdev of the log concentration distribution based on the bounds.
+        """Get stdev of log concentration distribution based on the bounds.
 
         Returns
         -------
         a NumPy array with the stdev of the log concentrations
         """
         ci = (self.ln_conc_ub - self.ln_conc_lb) / 2.0
         return ci / stats.chi2.ppf(self.ln_conc_confidence, 1) ** (0.5)
```

### Comparing `equilibrator-api-0.4.8b1/src/equilibrator_api/phased_compound.py` & `equilibrator-api-0.5.0b1/src/equilibrator_api/phased_compound.py`

 * *Files identical despite different names*

### Comparing `equilibrator-api-0.4.8b1/src/equilibrator_api/phased_reaction.py` & `equilibrator-api-0.5.0b1/src/equilibrator_api/phased_reaction.py`

 * *Files identical despite different names*

### Comparing `equilibrator-api-0.4.8b1/src/equilibrator_api/reaction_parser.py` & `equilibrator-api-0.5.0b1/src/equilibrator_api/reaction_parser.py`

 * *Files identical despite different names*

### Comparing `equilibrator-api-0.4.8b1/src/equilibrator_api.egg-info/PKG-INFO` & `equilibrator-api-0.5.0b1/src/equilibrator_api.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: equilibrator-api
-Version: 0.4.8b1
+Version: 0.5.0b1
 Summary: Calculation of standard thermodynamic potentials of biochemical reactions.
 Home-page: https://gitlab.com/equilibrator/equilibrator-api/
 Download-URL: https://pypi.org/project/equilibrator-api/
 Author: Elad Noor, Moritz E. Beber
 Author-email: eladn@weizmann.ac.il, midnighter@posteo.net
 License: MIT
 Project-URL: Source Code, https://gitlab.com/equilibrator/equilibrator-api/
@@ -12,22 +12,20 @@
 Keywords: component contribution,Gibbs energy,biochemical reaction,eQuilibrator
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3 :: Only
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Scientific/Engineering :: Bio-Informatics
 Classifier: Topic :: Scientific/Engineering :: Chemistry
-Requires-Python: >=3.6
+Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 Provides-Extra: test
 Provides-Extra: development
 Provides-Extra: deployment
 License-File: LICENSE
 
 # eQuilibrator - a thermodynamics calculator for biochemical reactions
```

### Comparing `equilibrator-api-0.4.8b1/src/equilibrator_api.egg-info/SOURCES.txt` & `equilibrator-api-0.5.0b1/src/equilibrator_api.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `equilibrator-api-0.4.8b1/versioneer.py` & `equilibrator-api-0.5.0b1/versioneer.py`

 * *Files identical despite different names*

