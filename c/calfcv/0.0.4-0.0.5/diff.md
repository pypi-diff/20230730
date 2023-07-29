# Comparing `tmp/calfcv-0.0.4.tar.gz` & `tmp/calfcv-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "calfcv-0.0.4.tar", last modified: Sat Jul 29 22:16:32 2023, max compression
+gzip compressed data, was "calfcv-0.0.5.tar", last modified: Sat Jul 29 22:44:54 2023, max compression
```

## Comparing `calfcv-0.0.4.tar` & `calfcv-0.0.5.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxrwxr-x   0 rolf      (1000) rolf      (1000)        0 2023-07-29 22:16:32.133685 calfcv-0.0.4/
--rw-rw-r--   0 rolf      (1000) rolf      (1000)     1495 2023-07-29 01:55:36.000000 calfcv-0.0.4/LICENSE
--rw-rw-r--   0 rolf      (1000) rolf      (1000)       25 2023-07-24 23:20:23.000000 calfcv-0.0.4/MANIFEST.in
--rw-rw-r--   0 rolf      (1000) rolf      (1000)     4964 2023-07-29 22:16:32.133685 calfcv-0.0.4/PKG-INFO
--rw-rw-r--   0 rolf      (1000) rolf      (1000)     4336 2023-07-29 20:32:45.000000 calfcv-0.0.4/README.rst
-drwxrwxr-x   0 rolf      (1000) rolf      (1000)        0 2023-07-29 22:16:32.129685 calfcv-0.0.4/calfcv/
--rw-rw-r--   0 rolf      (1000) rolf      (1000)       98 2023-07-28 23:01:34.000000 calfcv-0.0.4/calfcv/__init__.py
--rw-rw-r--   0 rolf      (1000) rolf      (1000)       22 2023-07-29 01:59:39.000000 calfcv-0.0.4/calfcv/_version.py
--rw-rw-r--   0 rolf      (1000) rolf      (1000)     8479 2023-07-29 02:15:49.000000 calfcv-0.0.4/calfcv/calfcv.py
-drwxrwxr-x   0 rolf      (1000) rolf      (1000)        0 2023-07-29 22:16:32.133685 calfcv-0.0.4/calfcv/tests/
--rw-rw-r--   0 rolf      (1000) rolf      (1000)        0 2023-07-24 23:20:23.000000 calfcv-0.0.4/calfcv/tests/__init__.py
--rw-rw-r--   0 rolf      (1000) rolf      (1000)     1563 2023-07-28 13:25:35.000000 calfcv-0.0.4/calfcv/tests/test_calfcv.py
--rw-rw-r--   0 rolf      (1000) rolf      (1000)      257 2023-07-28 12:52:06.000000 calfcv-0.0.4/calfcv/tests/test_common.py
-drwxrwxr-x   0 rolf      (1000) rolf      (1000)        0 2023-07-29 22:16:32.133685 calfcv-0.0.4/calfcv.egg-info/
--rw-rw-r--   0 rolf      (1000) rolf      (1000)     4964 2023-07-29 22:16:32.000000 calfcv-0.0.4/calfcv.egg-info/PKG-INFO
--rw-rw-r--   0 rolf      (1000) rolf      (1000)      380 2023-07-29 22:16:32.000000 calfcv-0.0.4/calfcv.egg-info/SOURCES.txt
--rw-rw-r--   0 rolf      (1000) rolf      (1000)        1 2023-07-29 22:16:32.000000 calfcv-0.0.4/calfcv.egg-info/dependency_links.txt
--rw-rw-r--   0 rolf      (1000) rolf      (1000)        1 2023-07-28 23:40:52.000000 calfcv-0.0.4/calfcv.egg-info/not-zip-safe
--rw-rw-r--   0 rolf      (1000) rolf      (1000)       25 2023-07-29 22:16:32.000000 calfcv-0.0.4/calfcv.egg-info/requires.txt
--rw-rw-r--   0 rolf      (1000) rolf      (1000)        7 2023-07-29 22:16:32.000000 calfcv-0.0.4/calfcv.egg-info/top_level.txt
--rw-rw-r--   0 rolf      (1000) rolf      (1000)       24 2023-07-24 23:20:23.000000 calfcv-0.0.4/requirements.txt
--rw-rw-r--   0 rolf      (1000) rolf      (1000)      148 2023-07-29 22:16:32.133685 calfcv-0.0.4/setup.cfg
--rw-rw-r--   0 rolf      (1000) rolf      (1000)     1929 2023-07-29 22:14:36.000000 calfcv-0.0.4/setup.py
+drwxrwxr-x   0 rolf      (1000) rolf      (1000)        0 2023-07-29 22:44:54.877823 calfcv-0.0.5/
+-rw-rw-r--   0 rolf      (1000) rolf      (1000)     1495 2023-07-29 01:55:36.000000 calfcv-0.0.5/LICENSE
+-rw-rw-r--   0 rolf      (1000) rolf      (1000)       25 2023-07-24 23:20:23.000000 calfcv-0.0.5/MANIFEST.in
+-rw-rw-r--   0 rolf      (1000) rolf      (1000)     4844 2023-07-29 22:44:54.877823 calfcv-0.0.5/PKG-INFO
+-rw-rw-r--   0 rolf      (1000) rolf      (1000)     4216 2023-07-29 22:44:22.000000 calfcv-0.0.5/README.rst
+drwxrwxr-x   0 rolf      (1000) rolf      (1000)        0 2023-07-29 22:44:54.877823 calfcv-0.0.5/calfcv/
+-rw-rw-r--   0 rolf      (1000) rolf      (1000)       98 2023-07-28 23:01:34.000000 calfcv-0.0.5/calfcv/__init__.py
+-rw-rw-r--   0 rolf      (1000) rolf      (1000)       22 2023-07-29 01:59:39.000000 calfcv-0.0.5/calfcv/_version.py
+-rw-rw-r--   0 rolf      (1000) rolf      (1000)     8479 2023-07-29 02:15:49.000000 calfcv-0.0.5/calfcv/calfcv.py
+drwxrwxr-x   0 rolf      (1000) rolf      (1000)        0 2023-07-29 22:44:54.877823 calfcv-0.0.5/calfcv/tests/
+-rw-rw-r--   0 rolf      (1000) rolf      (1000)        0 2023-07-24 23:20:23.000000 calfcv-0.0.5/calfcv/tests/__init__.py
+-rw-rw-r--   0 rolf      (1000) rolf      (1000)     1563 2023-07-28 13:25:35.000000 calfcv-0.0.5/calfcv/tests/test_calfcv.py
+-rw-rw-r--   0 rolf      (1000) rolf      (1000)      257 2023-07-28 12:52:06.000000 calfcv-0.0.5/calfcv/tests/test_common.py
+drwxrwxr-x   0 rolf      (1000) rolf      (1000)        0 2023-07-29 22:44:54.877823 calfcv-0.0.5/calfcv.egg-info/
+-rw-rw-r--   0 rolf      (1000) rolf      (1000)     4844 2023-07-29 22:44:54.000000 calfcv-0.0.5/calfcv.egg-info/PKG-INFO
+-rw-rw-r--   0 rolf      (1000) rolf      (1000)      380 2023-07-29 22:44:54.000000 calfcv-0.0.5/calfcv.egg-info/SOURCES.txt
+-rw-rw-r--   0 rolf      (1000) rolf      (1000)        1 2023-07-29 22:44:54.000000 calfcv-0.0.5/calfcv.egg-info/dependency_links.txt
+-rw-rw-r--   0 rolf      (1000) rolf      (1000)        1 2023-07-28 23:40:52.000000 calfcv-0.0.5/calfcv.egg-info/not-zip-safe
+-rw-rw-r--   0 rolf      (1000) rolf      (1000)       25 2023-07-29 22:44:54.000000 calfcv-0.0.5/calfcv.egg-info/requires.txt
+-rw-rw-r--   0 rolf      (1000) rolf      (1000)        7 2023-07-29 22:44:54.000000 calfcv-0.0.5/calfcv.egg-info/top_level.txt
+-rw-rw-r--   0 rolf      (1000) rolf      (1000)       24 2023-07-24 23:20:23.000000 calfcv-0.0.5/requirements.txt
+-rw-rw-r--   0 rolf      (1000) rolf      (1000)      148 2023-07-29 22:44:54.881823 calfcv-0.0.5/setup.cfg
+-rw-rw-r--   0 rolf      (1000) rolf      (1000)     1929 2023-07-29 22:34:53.000000 calfcv-0.0.5/setup.py
```

### Comparing `calfcv-0.0.4/LICENSE` & `calfcv-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `calfcv-0.0.4/PKG-INFO` & `calfcv-0.0.5/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: calfcv
-Version: 0.0.4
+Version: 0.0.5
 Summary: Coarse approximation linear function with cross validation
 Home-page: 
 Download-URL: https://github.com/scikit-learn-contrib/project-template
 Maintainer: Carlson Research, LLC
 Maintainer-email: hrolfrc@gmail.com
 License: new BSD
 Classifier: Intended Audience :: Science/Research
@@ -40,15 +40,15 @@
 
 Introduction
 ------------------
 This is a python implementation of the Coarse Approximation Linear Function (CALF). The implementation is based on the greedy forward selection algorithm described in the paper referenced below.
 
 Currently, CalfCV provides classification and prediction for two classes, the binomial case. Multinomial classification with more than two cases is not implemented.
 
-The feature matrix is scaled to remove the mean and have unit variance. Cross-validation is implemented to identify optimal score and coefficients. CalfCV is designed to be used with scikit-learn_ pipelines and composite estimators.
+The feature matrix is scaled to have zero mean and unit variance. Cross-validation is implemented to identify optimal score and coefficients. CalfCV is designed for use with scikit-learn_ pipelines and composite estimators.
 
 .. _scikit-learn: https://scikit-learn.org
 
 Example
 ------------------
 .. code:: ipython2
 
@@ -73,51 +73,50 @@
         random_state=seed
     )
     X_train, X_test, y_train, y_test = train_test_split(X, y, random_state=seed)
 
 Train the classifier
 ^^^^^^^^^^^^^^^^^^^^
 
-The best score is the best average auc
+The best score is the best average auc.
 
 .. code:: ipython2
 
     cls = CalfCV().fit(X_train, y_train)
     cls.best_score_
 
 
 
 
 .. parsed-literal::
 
     0.95
 
 
+The coefficients for the best score are in ``[-1, 0, 1]``.
 
-The coefficients for the best score
-^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
 
 .. code:: ipython2
 
     cls.best_coef_
 
 
 
 
 .. parsed-literal::
 
     [-1, 1, 0, 1, 1]
 
 
 
-The probabilities of class 1 are in the right column
+The probabilities of class 1 are in the last row
 ^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
 
 We vertically stack the ground truth on the top with the probabilities
-of 1 on the bottom. We show the first 5 entries.
+of class 1 on the bottom. We show the first 5 entries.
 
 
 
 .. code:: ipython2
 
     np.round(np.vstack((y_train, cls.predict_proba(X_train).T))[:, 0:5], 2)
 
@@ -147,18 +146,18 @@
 
 .. parsed-literal::
 
     0.9750000000000001
 
 
 
-The classifier has not seen the testing data
-^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
+The classifier will likely produce a lower score on unseen data
+^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
 
-Often we might get a lower score on the unseen data, but in this case we
+Often we get a lower score on the unseen data, but in this case we
 get a higher score.
 
 .. code:: ipython2
 
     roc_auc_score(y_true=y_test, y_score=cls.predict_proba(X_test)[:, 1])
 
 
@@ -166,20 +165,18 @@
 
 .. parsed-literal::
 
     1.0
 
 
 
-Predicting the classes produces a lower score than using the class probabilities
-^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
+Score using classes is lower than score than using probabilities
+^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
 
-The ground truth is on the top and the predicted class is on the bottom.
-The first column is the index. Sample 6 of y_test is predicted
-incorrectly but the others are correct.
+The ground truth is on the top and the predicted class is on the bottom. Sample 6 of y_test is predicted incorrectly but the others are correct.
 
 .. code:: ipython2
 
     y_pred = cls.predict(X_test)
     np.vstack((y_test, y_pred))
 
 
@@ -188,15 +185,14 @@
 .. parsed-literal::
 
     array([[0, 1, 1, 0, 1, 0, 0, 0],
            [0, 1, 1, 0, 1, 0, 1, 0]])
 
 
 
-The class prediction is expected to be lower than the auc prediction.
 
 .. code:: ipython2
 
     roc_auc_score(y_true=y_test, y_score=y_pred)
```

### Comparing `calfcv-0.0.4/README.rst` & `calfcv-0.0.5/README.rst`

 * *Files 16% similar despite different names*

```diff
@@ -22,15 +22,15 @@
 
 Introduction
 ------------------
 This is a python implementation of the Coarse Approximation Linear Function (CALF). The implementation is based on the greedy forward selection algorithm described in the paper referenced below.
 
 Currently, CalfCV provides classification and prediction for two classes, the binomial case. Multinomial classification with more than two cases is not implemented.
 
-The feature matrix is scaled to remove the mean and have unit variance. Cross-validation is implemented to identify optimal score and coefficients. CalfCV is designed to be used with scikit-learn_ pipelines and composite estimators.
+The feature matrix is scaled to have zero mean and unit variance. Cross-validation is implemented to identify optimal score and coefficients. CalfCV is designed for use with scikit-learn_ pipelines and composite estimators.
 
 .. _scikit-learn: https://scikit-learn.org
 
 Example
 ------------------
 .. code:: ipython2
 
@@ -55,51 +55,50 @@
         random_state=seed
     )
     X_train, X_test, y_train, y_test = train_test_split(X, y, random_state=seed)
 
 Train the classifier
 ^^^^^^^^^^^^^^^^^^^^
 
-The best score is the best average auc
+The best score is the best average auc.
 
 .. code:: ipython2
 
     cls = CalfCV().fit(X_train, y_train)
     cls.best_score_
 
 
 
 
 .. parsed-literal::
 
     0.95
 
 
+The coefficients for the best score are in ``[-1, 0, 1]``.
 
-The coefficients for the best score
-^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
 
 .. code:: ipython2
 
     cls.best_coef_
 
 
 
 
 .. parsed-literal::
 
     [-1, 1, 0, 1, 1]
 
 
 
-The probabilities of class 1 are in the right column
+The probabilities of class 1 are in the last row
 ^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
 
 We vertically stack the ground truth on the top with the probabilities
-of 1 on the bottom. We show the first 5 entries.
+of class 1 on the bottom. We show the first 5 entries.
 
 
 
 .. code:: ipython2
 
     np.round(np.vstack((y_train, cls.predict_proba(X_train).T))[:, 0:5], 2)
 
@@ -129,18 +128,18 @@
 
 .. parsed-literal::
 
     0.9750000000000001
 
 
 
-The classifier has not seen the testing data
-^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
+The classifier will likely produce a lower score on unseen data
+^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
 
-Often we might get a lower score on the unseen data, but in this case we
+Often we get a lower score on the unseen data, but in this case we
 get a higher score.
 
 .. code:: ipython2
 
     roc_auc_score(y_true=y_test, y_score=cls.predict_proba(X_test)[:, 1])
 
 
@@ -148,20 +147,18 @@
 
 .. parsed-literal::
 
     1.0
 
 
 
-Predicting the classes produces a lower score than using the class probabilities
-^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
+Score using classes is lower than score than using probabilities
+^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
 
-The ground truth is on the top and the predicted class is on the bottom.
-The first column is the index. Sample 6 of y_test is predicted
-incorrectly but the others are correct.
+The ground truth is on the top and the predicted class is on the bottom. Sample 6 of y_test is predicted incorrectly but the others are correct.
 
 .. code:: ipython2
 
     y_pred = cls.predict(X_test)
     np.vstack((y_test, y_pred))
 
 
@@ -170,15 +167,14 @@
 .. parsed-literal::
 
     array([[0, 1, 1, 0, 1, 0, 0, 0],
            [0, 1, 1, 0, 1, 0, 1, 0]])
 
 
 
-The class prediction is expected to be lower than the auc prediction.
 
 .. code:: ipython2
 
     roc_auc_score(y_true=y_test, y_score=y_pred)
```

### Comparing `calfcv-0.0.4/calfcv/calfcv.py` & `calfcv-0.0.5/calfcv/calfcv.py`

 * *Files identical despite different names*

### Comparing `calfcv-0.0.4/calfcv/tests/test_calfcv.py` & `calfcv-0.0.5/calfcv/tests/test_calfcv.py`

 * *Files identical despite different names*

### Comparing `calfcv-0.0.4/calfcv.egg-info/PKG-INFO` & `calfcv-0.0.5/calfcv.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: calfcv
-Version: 0.0.4
+Version: 0.0.5
 Summary: Coarse approximation linear function with cross validation
 Home-page: 
 Download-URL: https://github.com/scikit-learn-contrib/project-template
 Maintainer: Carlson Research, LLC
 Maintainer-email: hrolfrc@gmail.com
 License: new BSD
 Classifier: Intended Audience :: Science/Research
@@ -40,15 +40,15 @@
 
 Introduction
 ------------------
 This is a python implementation of the Coarse Approximation Linear Function (CALF). The implementation is based on the greedy forward selection algorithm described in the paper referenced below.
 
 Currently, CalfCV provides classification and prediction for two classes, the binomial case. Multinomial classification with more than two cases is not implemented.
 
-The feature matrix is scaled to remove the mean and have unit variance. Cross-validation is implemented to identify optimal score and coefficients. CalfCV is designed to be used with scikit-learn_ pipelines and composite estimators.
+The feature matrix is scaled to have zero mean and unit variance. Cross-validation is implemented to identify optimal score and coefficients. CalfCV is designed for use with scikit-learn_ pipelines and composite estimators.
 
 .. _scikit-learn: https://scikit-learn.org
 
 Example
 ------------------
 .. code:: ipython2
 
@@ -73,51 +73,50 @@
         random_state=seed
     )
     X_train, X_test, y_train, y_test = train_test_split(X, y, random_state=seed)
 
 Train the classifier
 ^^^^^^^^^^^^^^^^^^^^
 
-The best score is the best average auc
+The best score is the best average auc.
 
 .. code:: ipython2
 
     cls = CalfCV().fit(X_train, y_train)
     cls.best_score_
 
 
 
 
 .. parsed-literal::
 
     0.95
 
 
+The coefficients for the best score are in ``[-1, 0, 1]``.
 
-The coefficients for the best score
-^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
 
 .. code:: ipython2
 
     cls.best_coef_
 
 
 
 
 .. parsed-literal::
 
     [-1, 1, 0, 1, 1]
 
 
 
-The probabilities of class 1 are in the right column
+The probabilities of class 1 are in the last row
 ^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
 
 We vertically stack the ground truth on the top with the probabilities
-of 1 on the bottom. We show the first 5 entries.
+of class 1 on the bottom. We show the first 5 entries.
 
 
 
 .. code:: ipython2
 
     np.round(np.vstack((y_train, cls.predict_proba(X_train).T))[:, 0:5], 2)
 
@@ -147,18 +146,18 @@
 
 .. parsed-literal::
 
     0.9750000000000001
 
 
 
-The classifier has not seen the testing data
-^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
+The classifier will likely produce a lower score on unseen data
+^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
 
-Often we might get a lower score on the unseen data, but in this case we
+Often we get a lower score on the unseen data, but in this case we
 get a higher score.
 
 .. code:: ipython2
 
     roc_auc_score(y_true=y_test, y_score=cls.predict_proba(X_test)[:, 1])
 
 
@@ -166,20 +165,18 @@
 
 .. parsed-literal::
 
     1.0
 
 
 
-Predicting the classes produces a lower score than using the class probabilities
-^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
+Score using classes is lower than score than using probabilities
+^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
 
-The ground truth is on the top and the predicted class is on the bottom.
-The first column is the index. Sample 6 of y_test is predicted
-incorrectly but the others are correct.
+The ground truth is on the top and the predicted class is on the bottom. Sample 6 of y_test is predicted incorrectly but the others are correct.
 
 .. code:: ipython2
 
     y_pred = cls.predict(X_test)
     np.vstack((y_test, y_pred))
 
 
@@ -188,15 +185,14 @@
 .. parsed-literal::
 
     array([[0, 1, 1, 0, 1, 0, 0, 0],
            [0, 1, 1, 0, 1, 0, 1, 0]])
 
 
 
-The class prediction is expected to be lower than the auc prediction.
 
 .. code:: ipython2
 
     roc_auc_score(y_true=y_test, y_score=y_pred)
```

### Comparing `calfcv-0.0.4/setup.py` & `calfcv-0.0.5/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -26,15 +26,15 @@
 with codecs.open('README.rst', encoding='utf-8-sig') as f:
     LONG_DESCRIPTION = f.read()
 MAINTAINER = 'Carlson Research, LLC'
 MAINTAINER_EMAIL = 'hrolfrc@gmail.com'
 URL = ''
 LICENSE = 'new BSD'
 DOWNLOAD_URL = 'https://github.com/scikit-learn-contrib/project-template'
-VERSION = '0.0.4'
+VERSION = '0.0.5'
 INSTALL_REQUIRES = ['numpy', 'scipy', 'scikit-learn']
 CLASSIFIERS = ['Intended Audience :: Science/Research',
                'Intended Audience :: Developers',
                'Development Status :: 2 - Pre-Alpha',
                'License :: OSI Approved',
                'Topic :: Scientific/Engineering',
                'Operating System :: OS Independent',
```

