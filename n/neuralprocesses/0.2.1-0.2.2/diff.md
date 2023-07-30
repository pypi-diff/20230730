# Comparing `tmp/neuralprocesses-0.2.1.tar.gz` & `tmp/neuralprocesses-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "neuralprocesses-0.2.1.tar", last modified: Sun Jun  4 12:54:02 2023, max compression
+gzip compressed data, was "neuralprocesses-0.2.2.tar", last modified: Sun Jul 30 19:37:25 2023, max compression
```

## Comparing `neuralprocesses-0.2.1.tar` & `neuralprocesses-0.2.2.tar`

### file list

```diff
@@ -1,166 +1,166 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 12:54:02.672667 neuralprocesses-0.2.1/
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-06-04 12:53:45.000000 neuralprocesses-0.2.1/.coveragerc
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 12:54:02.636667 neuralprocesses-0.2.1/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 12:54:02.644667 neuralprocesses-0.2.1/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      972 2023-06-04 12:53:45.000000 neuralprocesses-0.2.1/.github/workflows/build_book.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1289 2023-06-04 12:53:45.000000 neuralprocesses-0.2.1/.github/workflows/ci.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1095 2023-06-04 12:53:45.000000 neuralprocesses-0.2.1/.github/workflows/publish.yml
--rw-r--r--   0 runner    (1001) docker     (123)      566 2023-06-04 12:53:45.000000 neuralprocesses-0.2.1/.github/workflows/style.yml
--rw-r--r--   0 runner    (1001) docker     (123)      301 2023-06-04 12:53:45.000000 neuralprocesses-0.2.1/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      125 2023-06-04 12:53:45.000000 neuralprocesses-0.2.1/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-06-04 12:53:45.000000 neuralprocesses-0.2.1/LICENCE.txt
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-06-04 12:53:45.000000 neuralprocesses-0.2.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)      209 2023-06-04 12:53:45.000000 neuralprocesses-0.2.1/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)     2349 2023-06-04 12:54:02.672667 neuralprocesses-0.2.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2005 2023-06-04 12:53:45.000000 neuralprocesses-0.2.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 12:54:02.644667 neuralprocesses-0.2.1/docs/
--rw-r--r--   0 runner    (1001) docker     (123)      817 2023-06-04 12:53:45.000000 neuralprocesses-0.2.1/docs/_config.yml
--rw-r--r--   0 runner    (1001) docker     (123)      227 2023-06-04 12:53:45.000000 neuralprocesses-0.2.1/docs/_toc.yml
--rw-r--r--   0 runner    (1001) docker     (123)     3338 2023-06-04 12:53:45.000000 neuralprocesses-0.2.1/docs/advanced_usage.md
--rw-r--r--   0 runner    (1001) docker     (123)      638 2023-06-04 12:53:45.000000 neuralprocesses-0.2.1/docs/architectures.rst
--rw-r--r--   0 runner    (1001) docker     (123)     5342 2023-06-04 12:53:45.000000 neuralprocesses-0.2.1/docs/basic_usage.md
--rw-r--r--   0 runner    (1001) docker     (123)     3915 2023-06-04 12:53:45.000000 neuralprocesses-0.2.1/docs/build_your_own_model.md
--rw-r--r--   0 runner    (1001) docker     (123)     1176 2023-06-04 12:53:45.000000 neuralprocesses-0.2.1/docs/coders.rst
--rw-r--r--   0 runner    (1001) docker     (123)       43 2023-06-04 12:53:45.000000 neuralprocesses-0.2.1/docs/intro.md
--rw-r--r--   0 runner    (1001) docker     (123)     9854 2023-06-04 12:53:45.000000 neuralprocesses-0.2.1/docs/logo.png
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-06-04 12:53:45.000000 neuralprocesses-0.2.1/docs/references.bib
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 12:54:02.648667 neuralprocesses-0.2.1/experiment/
--rw-r--r--   0 runner    (1001) docker     (123)       60 2023-06-04 12:53:45.000000 neuralprocesses-0.2.1/experiment/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 12:54:02.648667 neuralprocesses-0.2.1/experiment/data/
--rw-r--r--   0 runner    (1001) docker     (123)      134 2023-06-04 12:53:45.000000 neuralprocesses-0.2.1/experiment/data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1533 2023-06-04 12:53:45.000000 neuralprocesses-0.2.1/experiment/data/antarctica.py
--rw-r--r--   0 runner    (1001) docker     (123)     2984 2023-06-04 12:53:45.000000 neuralprocesses-0.2.1/experiment/data/eeg.py
--rw-r--r--   0 runner    (1001) docker     (123)     3336 2023-06-04 12:53:45.000000 neuralprocesses-0.2.1/experiment/data/gp.py
--rw-r--r--   0 runner    (1001) docker     (123)     3633 2023-06-04 12:53:45.000000 neuralprocesses-0.2.1/experiment/data/predprey.py
--rw-r--r--   0 runner    (1001) docker     (123)     5348 2023-06-04 12:53:45.000000 neuralprocesses-0.2.1/experiment/data/temperature.py
--rw-r--r--   0 runner    (1001) docker     (123)      618 2023-06-04 12:53:45.000000 neuralprocesses-0.2.1/experiment/data/util.py
--rw-r--r--   0 runner    (1001) docker     (123)     6464 2023-06-04 12:53:45.000000 neuralprocesses-0.2.1/experiment/plot.py
--rw-r--r--   0 runner    (1001) docker     (123)     8322 2023-06-04 12:53:45.000000 neuralprocesses-0.2.1/experiment/util.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 12:54:02.652667 neuralprocesses-0.2.1/neuralprocesses/
--rw-r--r--   0 runner    (1001) docker     (123)     1115 2023-06-04 12:53:45.000000 neuralprocesses-0.2.1/neuralprocesses/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-06-04 12:54:02.000000 neuralprocesses-0.2.1/neuralprocesses/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)     3232 2023-06-04 12:53:45.000000 neuralprocesses-0.2.1/neuralprocesses/aggregate.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 12:54:02.652667 neuralprocesses-0.2.1/neuralprocesses/architectures/
--rw-r--r--   0 runner    (1001) docker     (123)      112 2023-06-04 12:53:45.000000 neuralprocesses-0.2.1/neuralprocesses/architectures/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2839 2023-06-04 12:53:45.000000 neuralprocesses-0.2.1/neuralprocesses/architectures/agnp.py
--rw-r--r--   0 runner    (1001) docker     (123)    10822 2023-06-04 12:53:45.000000 neuralprocesses-0.2.1/neuralprocesses/architectures/climate.py
--rw-r--r--   0 runner    (1001) docker     (123)    15136 2023-06-04 12:53:45.000000 neuralprocesses-0.2.1/neuralprocesses/architectures/convgnp.py
--rw-r--r--   0 runner    (1001) docker     (123)    13208 2023-06-04 12:53:45.000000 neuralprocesses-0.2.1/neuralprocesses/architectures/fullconvgnp.py
--rw-r--r--   0 runner    (1001) docker     (123)     8064 2023-06-04 12:53:45.000000 neuralprocesses-0.2.1/neuralprocesses/architectures/gnp.py
--rw-r--r--   0 runner    (1001) docker     (123)     3566 2023-06-04 12:53:45.000000 neuralprocesses-0.2.1/neuralprocesses/architectures/util.py
--rw-r--r--   0 runner    (1001) docker     (123)      521 2023-06-04 12:53:45.000000 neuralprocesses-0.2.1/neuralprocesses/augment.py
--rw-r--r--   0 runner    (1001) docker     (123)     1546 2023-06-04 12:53:45.000000 neuralprocesses-0.2.1/neuralprocesses/chain.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 12:54:02.656667 neuralprocesses-0.2.1/neuralprocesses/coders/
--rw-r--r--   0 runner    (1001) docker     (123)      295 2023-06-04 12:53:45.000000 neuralprocesses-0.2.1/neuralprocesses/coders/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7435 2023-06-04 12:53:45.000000 neuralprocesses-0.2.1/neuralprocesses/coders/aggregate.py
--rw-r--r--   0 runner    (1001) docker     (123)     5368 2023-06-04 12:53:45.000000 neuralprocesses-0.2.1/neuralprocesses/coders/attention.py
--rw-r--r--   0 runner    (1001) docker     (123)     1383 2023-06-04 12:53:45.000000 neuralprocesses-0.2.1/neuralprocesses/coders/augment.py
--rw-r--r--   0 runner    (1001) docker     (123)      335 2023-06-04 12:53:45.000000 neuralprocesses-0.2.1/neuralprocesses/coders/copy.py
--rw-r--r--   0 runner    (1001) docker     (123)      799 2023-06-04 12:53:45.000000 neuralprocesses-0.2.1/neuralprocesses/coders/deepset.py
--rw-r--r--   0 runner    (1001) docker     (123)     3029 2023-06-04 12:53:45.000000 neuralprocesses-0.2.1/neuralprocesses/coders/densecov.py
--rw-r--r--   0 runner    (1001) docker     (123)     1647 2023-06-04 12:53:45.000000 neuralprocesses-0.2.1/neuralprocesses/coders/functional.py
--rw-r--r--   0 runner    (1001) docker     (123)      805 2023-06-04 12:53:45.000000 neuralprocesses-0.2.1/neuralprocesses/coders/fuse.py
--rw-r--r--   0 runner    (1001) docker     (123)      472 2023-06-04 12:53:45.000000 neuralprocesses-0.2.1/neuralprocesses/coders/inputs.py
--rw-r--r--   0 runner    (1001) docker     (123)     2288 2023-06-04 12:53:45.000000 neuralprocesses-0.2.1/neuralprocesses/coders/mapdiag.py
--rw-r--r--   0 runner    (1001) docker     (123)    25181 2023-06-04 12:53:45.000000 neuralprocesses-0.2.1/neuralprocesses/coders/nn.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 12:54:02.656667 neuralprocesses-0.2.1/neuralprocesses/coders/setconv/
--rw-r--r--   0 runner    (1001) docker     (123)       70 2023-06-04 12:53:45.000000 neuralprocesses-0.2.1/neuralprocesses/coders/setconv/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3947 2023-06-04 12:53:45.000000 neuralprocesses-0.2.1/neuralprocesses/coders/setconv/density.py
--rw-r--r--   0 runner    (1001) docker     (123)      905 2023-06-04 12:53:45.000000 neuralprocesses-0.2.1/neuralprocesses/coders/setconv/identity.py
--rw-r--r--   0 runner    (1001) docker     (123)     4832 2023-06-04 12:53:45.000000 neuralprocesses-0.2.1/neuralprocesses/coders/setconv/setconv.py
--rw-r--r--   0 runner    (1001) docker     (123)     4073 2023-06-04 12:53:45.000000 neuralprocesses-0.2.1/neuralprocesses/coders/shaping.py
--rw-r--r--   0 runner    (1001) docker     (123)     4362 2023-06-04 12:53:45.000000 neuralprocesses-0.2.1/neuralprocesses/coding.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 12:54:02.660667 neuralprocesses-0.2.1/neuralprocesses/data/
--rw-r--r--   0 runner    (1001) docker     (123)      223 2023-06-04 12:53:45.000000 neuralprocesses-0.2.1/neuralprocesses/data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11033 2023-06-04 12:53:45.000000 neuralprocesses-0.2.1/neuralprocesses/data/antarctica.py
--rw-r--r--   0 runner    (1001) docker     (123)     3318 2023-06-04 12:53:45.000000 neuralprocesses-0.2.1/neuralprocesses/data/batch.py
--rw-r--r--   0 runner    (1001) docker     (123)     2333 2023-06-04 12:53:45.000000 neuralprocesses-0.2.1/neuralprocesses/data/bimodal.py
--rw-r--r--   0 runner    (1001) docker     (123)    14216 2023-06-04 12:53:45.000000 neuralprocesses-0.2.1/neuralprocesses/data/data.py
--rw-r--r--   0 runner    (1001) docker     (123)     6860 2023-06-04 12:53:45.000000 neuralprocesses-0.2.1/neuralprocesses/data/eeg.py
--rw-r--r--   0 runner    (1001) docker     (123)     3880 2023-06-04 12:53:45.000000 neuralprocesses-0.2.1/neuralprocesses/data/gp.py
--rw-r--r--   0 runner    (1001) docker     (123)     3033 2023-06-04 12:53:45.000000 neuralprocesses-0.2.1/neuralprocesses/data/mixgp.py
--rw-r--r--   0 runner    (1001) docker     (123)     1152 2023-06-04 12:53:45.000000 neuralprocesses-0.2.1/neuralprocesses/data/mixture.py
--rw-r--r--   0 runner    (1001) docker     (123)     5400 2023-06-04 12:53:45.000000 neuralprocesses-0.2.1/neuralprocesses/data/predefined.py
--rw-r--r--   0 runner    (1001) docker     (123)    12613 2023-06-04 12:53:45.000000 neuralprocesses-0.2.1/neuralprocesses/data/predprey.py
--rw-r--r--   0 runner    (1001) docker     (123)     2414 2023-06-04 12:53:45.000000 neuralprocesses-0.2.1/neuralprocesses/data/sawtooth.py
--rw-r--r--   0 runner    (1001) docker     (123)    27362 2023-06-04 12:53:45.000000 neuralprocesses-0.2.1/neuralprocesses/data/temperature.py
--rw-r--r--   0 runner    (1001) docker     (123)      544 2023-06-04 12:53:45.000000 neuralprocesses-0.2.1/neuralprocesses/data/util.py
--rw-r--r--   0 runner    (1001) docker     (123)     1578 2023-06-04 12:53:45.000000 neuralprocesses-0.2.1/neuralprocesses/datadims.py
--rw-r--r--   0 runner    (1001) docker     (123)     5015 2023-06-04 12:53:45.000000 neuralprocesses-0.2.1/neuralprocesses/disc.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 12:54:02.664667 neuralprocesses-0.2.1/neuralprocesses/dist/
--rw-r--r--   0 runner    (1001) docker     (123)      178 2023-06-04 12:53:45.000000 neuralprocesses-0.2.1/neuralprocesses/dist/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3397 2023-06-04 12:53:45.000000 neuralprocesses-0.2.1/neuralprocesses/dist/beta.py
--rw-r--r--   0 runner    (1001) docker     (123)     2547 2023-06-04 12:53:45.000000 neuralprocesses-0.2.1/neuralprocesses/dist/dirac.py
--rw-r--r--   0 runner    (1001) docker     (123)     3430 2023-06-04 12:53:45.000000 neuralprocesses-0.2.1/neuralprocesses/dist/dist.py
--rw-r--r--   0 runner    (1001) docker     (123)     2002 2023-06-04 12:53:45.000000 neuralprocesses-0.2.1/neuralprocesses/dist/geom.py
--rw-r--r--   0 runner    (1001) docker     (123)     8774 2023-06-04 12:53:45.000000 neuralprocesses-0.2.1/neuralprocesses/dist/normal.py
--rw-r--r--   0 runner    (1001) docker     (123)     7430 2023-06-04 12:53:45.000000 neuralprocesses-0.2.1/neuralprocesses/dist/spikeslab.py
--rw-r--r--   0 runner    (1001) docker     (123)     7710 2023-06-04 12:53:45.000000 neuralprocesses-0.2.1/neuralprocesses/dist/transformed.py
--rw-r--r--   0 runner    (1001) docker     (123)     2178 2023-06-04 12:53:45.000000 neuralprocesses-0.2.1/neuralprocesses/dist/uniform.py
--rw-r--r--   0 runner    (1001) docker     (123)    11566 2023-06-04 12:53:45.000000 neuralprocesses-0.2.1/neuralprocesses/likelihood.py
--rw-r--r--   0 runner    (1001) docker     (123)     3434 2023-06-04 12:53:45.000000 neuralprocesses-0.2.1/neuralprocesses/mask.py
--rw-r--r--   0 runner    (1001) docker     (123)     4935 2023-06-04 12:53:45.000000 neuralprocesses-0.2.1/neuralprocesses/materialise.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 12:54:02.664667 neuralprocesses-0.2.1/neuralprocesses/model/
--rw-r--r--   0 runner    (1001) docker     (123)      104 2023-06-04 12:53:45.000000 neuralprocesses-0.2.1/neuralprocesses/model/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11392 2023-06-04 12:53:45.000000 neuralprocesses-0.2.1/neuralprocesses/model/ar.py
--rw-r--r--   0 runner    (1001) docker     (123)     5008 2023-06-04 12:53:45.000000 neuralprocesses-0.2.1/neuralprocesses/model/elbo.py
--rw-r--r--   0 runner    (1001) docker     (123)     3289 2023-06-04 12:53:45.000000 neuralprocesses-0.2.1/neuralprocesses/model/loglik.py
--rw-r--r--   0 runner    (1001) docker     (123)     3678 2023-06-04 12:53:45.000000 neuralprocesses-0.2.1/neuralprocesses/model/model.py
--rw-r--r--   0 runner    (1001) docker     (123)     4017 2023-06-04 12:53:45.000000 neuralprocesses-0.2.1/neuralprocesses/model/predict.py
--rw-r--r--   0 runner    (1001) docker     (123)     3248 2023-06-04 12:53:45.000000 neuralprocesses-0.2.1/neuralprocesses/model/util.py
--rw-r--r--   0 runner    (1001) docker     (123)      679 2023-06-04 12:53:45.000000 neuralprocesses-0.2.1/neuralprocesses/numdata.py
--rw-r--r--   0 runner    (1001) docker     (123)     3520 2023-06-04 12:53:45.000000 neuralprocesses-0.2.1/neuralprocesses/parallel.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 12:54:02.664667 neuralprocesses-0.2.1/neuralprocesses/tensorflow/
--rw-r--r--   0 runner    (1001) docker     (123)     1037 2023-06-04 12:53:45.000000 neuralprocesses-0.2.1/neuralprocesses/tensorflow/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10168 2023-06-04 12:53:45.000000 neuralprocesses-0.2.1/neuralprocesses/tensorflow/nn.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 12:54:02.668667 neuralprocesses-0.2.1/neuralprocesses/torch/
--rw-r--r--   0 runner    (1001) docker     (123)      796 2023-06-04 12:53:45.000000 neuralprocesses-0.2.1/neuralprocesses/torch/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7071 2023-06-04 12:53:45.000000 neuralprocesses-0.2.1/neuralprocesses/torch/nn.py
--rw-r--r--   0 runner    (1001) docker     (123)     6413 2023-06-04 12:53:45.000000 neuralprocesses-0.2.1/neuralprocesses/util.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 12:54:02.652667 neuralprocesses-0.2.1/neuralprocesses.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2349 2023-06-04 12:54:02.000000 neuralprocesses-0.2.1/neuralprocesses.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3954 2023-06-04 12:54:02.000000 neuralprocesses-0.2.1/neuralprocesses.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-04 12:54:02.000000 neuralprocesses-0.2.1/neuralprocesses.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       98 2023-06-04 12:54:02.000000 neuralprocesses-0.2.1/neuralprocesses.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       33 2023-06-04 12:54:02.000000 neuralprocesses-0.2.1/neuralprocesses.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      242 2023-06-04 12:53:45.000000 neuralprocesses-0.2.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      232 2023-06-04 12:53:45.000000 neuralprocesses-0.2.1/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)    11863 2023-06-04 12:53:45.000000 neuralprocesses-0.2.1/schedule.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 12:54:02.668667 neuralprocesses-0.2.1/scripts/
--rw-r--r--   0 runner    (1001) docker     (123)     4120 2023-06-04 12:53:45.000000 neuralprocesses-0.2.1/scripts/predprey.py
--rw-r--r--   0 runner    (1001) docker     (123)     1056 2023-06-04 12:53:45.000000 neuralprocesses-0.2.1/scripts/predprey_visualise.py
--rw-r--r--   0 runner    (1001) docker     (123)     3080 2023-06-04 12:53:45.000000 neuralprocesses-0.2.1/scripts/sawtooth_sample_ar.py
--rw-r--r--   0 runner    (1001) docker     (123)     3863 2023-06-04 12:53:45.000000 neuralprocesses-0.2.1/scripts/synthetic_extra.py
--rw-r--r--   0 runner    (1001) docker     (123)    15625 2023-06-04 12:53:45.000000 neuralprocesses-0.2.1/scripts/synthetic_parse.py
--rw-r--r--   0 runner    (1001) docker     (123)     2078 2023-06-04 12:53:45.000000 neuralprocesses-0.2.1/scripts/temperature_mae.py
--rw-r--r--   0 runner    (1001) docker     (123)     2077 2023-06-04 12:53:45.000000 neuralprocesses-0.2.1/scripts/temperature_summarise_folds.py
--rw-r--r--   0 runner    (1001) docker     (123)     3838 2023-06-04 12:53:45.000000 neuralprocesses-0.2.1/scripts/temperature_visualise.py
--rw-r--r--   0 runner    (1001) docker     (123)      379 2023-06-04 12:54:02.672667 neuralprocesses-0.2.1/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (123)      355 2023-06-04 12:53:45.000000 neuralprocesses-0.2.1/setup.py
--rw-r--r--   0 runner    (1001) docker     (123)    27121 2023-06-04 12:53:45.000000 neuralprocesses-0.2.1/tables.ipynb
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 12:54:02.672667 neuralprocesses-0.2.1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      149 2023-06-04 12:53:45.000000 neuralprocesses-0.2.1/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 12:54:02.672667 neuralprocesses-0.2.1/tests/coders/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-04 12:53:45.000000 neuralprocesses-0.2.1/tests/coders/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1048 2023-06-04 12:53:45.000000 neuralprocesses-0.2.1/tests/coders/test_shaping.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 12:54:02.672667 neuralprocesses-0.2.1/tests/dists/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-04 12:53:45.000000 neuralprocesses-0.2.1/tests/dists/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1959 2023-06-04 12:53:45.000000 neuralprocesses-0.2.1/tests/dists/test_normal.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 12:54:02.672667 neuralprocesses-0.2.1/tests/gnp/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-04 12:53:45.000000 neuralprocesses-0.2.1/tests/gnp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1109 2023-06-04 12:53:45.000000 neuralprocesses-0.2.1/tests/gnp/autoencoding.py
--rw-r--r--   0 runner    (1001) docker     (123)     1100 2023-06-04 12:53:45.000000 neuralprocesses-0.2.1/tests/gnp/gnp.py
--rw-r--r--   0 runner    (1001) docker     (123)      527 2023-06-04 12:53:45.000000 neuralprocesses-0.2.1/tests/gnp/util.py
--rw-r--r--   0 runner    (1001) docker     (123)    13948 2023-06-04 12:53:45.000000 neuralprocesses-0.2.1/tests/test_architectures.py
--rw-r--r--   0 runner    (1001) docker     (123)     1769 2023-06-04 12:53:45.000000 neuralprocesses-0.2.1/tests/test_augment.py
--rw-r--r--   0 runner    (1001) docker     (123)      340 2023-06-04 12:53:45.000000 neuralprocesses-0.2.1/tests/test_chain.py
--rw-r--r--   0 runner    (1001) docker     (123)     8001 2023-06-04 12:53:45.000000 neuralprocesses-0.2.1/tests/test_data.py
--rw-r--r--   0 runner    (1001) docker     (123)      806 2023-06-04 12:53:45.000000 neuralprocesses-0.2.1/tests/test_discretisation.py
--rw-r--r--   0 runner    (1001) docker     (123)     1255 2023-06-04 12:53:45.000000 neuralprocesses-0.2.1/tests/test_distribution.py
--rw-r--r--   0 runner    (1001) docker     (123)     1004 2023-06-04 12:53:45.000000 neuralprocesses-0.2.1/tests/test_mask.py
--rw-r--r--   0 runner    (1001) docker     (123)     1534 2023-06-04 12:53:45.000000 neuralprocesses-0.2.1/tests/test_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     1853 2023-06-04 12:53:45.000000 neuralprocesses-0.2.1/tests/test_unet.py
--rw-r--r--   0 runner    (1001) docker     (123)      268 2023-06-04 12:53:45.000000 neuralprocesses-0.2.1/tests/test_util.py
--rw-r--r--   0 runner    (1001) docker     (123)     1930 2023-06-04 12:53:45.000000 neuralprocesses-0.2.1/tests/util.py
--rw-r--r--   0 runner    (1001) docker     (123)     9301 2023-06-04 12:53:45.000000 neuralprocesses-0.2.1/todo.tasks
--rw-r--r--   0 runner    (1001) docker     (123)    26899 2023-06-04 12:53:45.000000 neuralprocesses-0.2.1/train.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 19:37:25.307177 neuralprocesses-0.2.2/
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-07-30 19:37:15.000000 neuralprocesses-0.2.2/.coveragerc
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 19:37:25.287176 neuralprocesses-0.2.2/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 19:37:25.291176 neuralprocesses-0.2.2/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      972 2023-07-30 19:37:15.000000 neuralprocesses-0.2.2/.github/workflows/build_book.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1289 2023-07-30 19:37:15.000000 neuralprocesses-0.2.2/.github/workflows/ci.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1095 2023-07-30 19:37:15.000000 neuralprocesses-0.2.2/.github/workflows/publish.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      566 2023-07-30 19:37:15.000000 neuralprocesses-0.2.2/.github/workflows/style.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      301 2023-07-30 19:37:15.000000 neuralprocesses-0.2.2/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      125 2023-07-30 19:37:15.000000 neuralprocesses-0.2.2/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-07-30 19:37:15.000000 neuralprocesses-0.2.2/LICENCE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-30 19:37:15.000000 neuralprocesses-0.2.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)      209 2023-07-30 19:37:15.000000 neuralprocesses-0.2.2/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)     2349 2023-07-30 19:37:25.307177 neuralprocesses-0.2.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2005 2023-07-30 19:37:15.000000 neuralprocesses-0.2.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 19:37:25.291176 neuralprocesses-0.2.2/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)      817 2023-07-30 19:37:15.000000 neuralprocesses-0.2.2/docs/_config.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      227 2023-07-30 19:37:15.000000 neuralprocesses-0.2.2/docs/_toc.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     3338 2023-07-30 19:37:15.000000 neuralprocesses-0.2.2/docs/advanced_usage.md
+-rw-r--r--   0 runner    (1001) docker     (123)      638 2023-07-30 19:37:15.000000 neuralprocesses-0.2.2/docs/architectures.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     5342 2023-07-30 19:37:15.000000 neuralprocesses-0.2.2/docs/basic_usage.md
+-rw-r--r--   0 runner    (1001) docker     (123)     3915 2023-07-30 19:37:15.000000 neuralprocesses-0.2.2/docs/build_your_own_model.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1176 2023-07-30 19:37:15.000000 neuralprocesses-0.2.2/docs/coders.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-07-30 19:37:15.000000 neuralprocesses-0.2.2/docs/intro.md
+-rw-r--r--   0 runner    (1001) docker     (123)     9854 2023-07-30 19:37:15.000000 neuralprocesses-0.2.2/docs/logo.png
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-07-30 19:37:15.000000 neuralprocesses-0.2.2/docs/references.bib
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 19:37:25.295176 neuralprocesses-0.2.2/experiment/
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-07-30 19:37:15.000000 neuralprocesses-0.2.2/experiment/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 19:37:25.295176 neuralprocesses-0.2.2/experiment/data/
+-rw-r--r--   0 runner    (1001) docker     (123)      134 2023-07-30 19:37:15.000000 neuralprocesses-0.2.2/experiment/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1533 2023-07-30 19:37:15.000000 neuralprocesses-0.2.2/experiment/data/antarctica.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2984 2023-07-30 19:37:15.000000 neuralprocesses-0.2.2/experiment/data/eeg.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3336 2023-07-30 19:37:15.000000 neuralprocesses-0.2.2/experiment/data/gp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3633 2023-07-30 19:37:15.000000 neuralprocesses-0.2.2/experiment/data/predprey.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5348 2023-07-30 19:37:15.000000 neuralprocesses-0.2.2/experiment/data/temperature.py
+-rw-r--r--   0 runner    (1001) docker     (123)      618 2023-07-30 19:37:15.000000 neuralprocesses-0.2.2/experiment/data/util.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6464 2023-07-30 19:37:15.000000 neuralprocesses-0.2.2/experiment/plot.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8322 2023-07-30 19:37:15.000000 neuralprocesses-0.2.2/experiment/util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 19:37:25.295176 neuralprocesses-0.2.2/neuralprocesses/
+-rw-r--r--   0 runner    (1001) docker     (123)     1115 2023-07-30 19:37:15.000000 neuralprocesses-0.2.2/neuralprocesses/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-07-30 19:37:25.000000 neuralprocesses-0.2.2/neuralprocesses/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3232 2023-07-30 19:37:15.000000 neuralprocesses-0.2.2/neuralprocesses/aggregate.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 19:37:25.295176 neuralprocesses-0.2.2/neuralprocesses/architectures/
+-rw-r--r--   0 runner    (1001) docker     (123)      112 2023-07-30 19:37:15.000000 neuralprocesses-0.2.2/neuralprocesses/architectures/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2839 2023-07-30 19:37:15.000000 neuralprocesses-0.2.2/neuralprocesses/architectures/agnp.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10822 2023-07-30 19:37:15.000000 neuralprocesses-0.2.2/neuralprocesses/architectures/climate.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15136 2023-07-30 19:37:15.000000 neuralprocesses-0.2.2/neuralprocesses/architectures/convgnp.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13208 2023-07-30 19:37:15.000000 neuralprocesses-0.2.2/neuralprocesses/architectures/fullconvgnp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8064 2023-07-30 19:37:15.000000 neuralprocesses-0.2.2/neuralprocesses/architectures/gnp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3566 2023-07-30 19:37:15.000000 neuralprocesses-0.2.2/neuralprocesses/architectures/util.py
+-rw-r--r--   0 runner    (1001) docker     (123)      521 2023-07-30 19:37:15.000000 neuralprocesses-0.2.2/neuralprocesses/augment.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1546 2023-07-30 19:37:15.000000 neuralprocesses-0.2.2/neuralprocesses/chain.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 19:37:25.299177 neuralprocesses-0.2.2/neuralprocesses/coders/
+-rw-r--r--   0 runner    (1001) docker     (123)      295 2023-07-30 19:37:15.000000 neuralprocesses-0.2.2/neuralprocesses/coders/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7435 2023-07-30 19:37:15.000000 neuralprocesses-0.2.2/neuralprocesses/coders/aggregate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5368 2023-07-30 19:37:15.000000 neuralprocesses-0.2.2/neuralprocesses/coders/attention.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1383 2023-07-30 19:37:15.000000 neuralprocesses-0.2.2/neuralprocesses/coders/augment.py
+-rw-r--r--   0 runner    (1001) docker     (123)      335 2023-07-30 19:37:15.000000 neuralprocesses-0.2.2/neuralprocesses/coders/copy.py
+-rw-r--r--   0 runner    (1001) docker     (123)      799 2023-07-30 19:37:15.000000 neuralprocesses-0.2.2/neuralprocesses/coders/deepset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3029 2023-07-30 19:37:15.000000 neuralprocesses-0.2.2/neuralprocesses/coders/densecov.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1647 2023-07-30 19:37:15.000000 neuralprocesses-0.2.2/neuralprocesses/coders/functional.py
+-rw-r--r--   0 runner    (1001) docker     (123)      805 2023-07-30 19:37:15.000000 neuralprocesses-0.2.2/neuralprocesses/coders/fuse.py
+-rw-r--r--   0 runner    (1001) docker     (123)      472 2023-07-30 19:37:15.000000 neuralprocesses-0.2.2/neuralprocesses/coders/inputs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2288 2023-07-30 19:37:15.000000 neuralprocesses-0.2.2/neuralprocesses/coders/mapdiag.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25181 2023-07-30 19:37:15.000000 neuralprocesses-0.2.2/neuralprocesses/coders/nn.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 19:37:25.299177 neuralprocesses-0.2.2/neuralprocesses/coders/setconv/
+-rw-r--r--   0 runner    (1001) docker     (123)       70 2023-07-30 19:37:15.000000 neuralprocesses-0.2.2/neuralprocesses/coders/setconv/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3947 2023-07-30 19:37:15.000000 neuralprocesses-0.2.2/neuralprocesses/coders/setconv/density.py
+-rw-r--r--   0 runner    (1001) docker     (123)      905 2023-07-30 19:37:15.000000 neuralprocesses-0.2.2/neuralprocesses/coders/setconv/identity.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4832 2023-07-30 19:37:15.000000 neuralprocesses-0.2.2/neuralprocesses/coders/setconv/setconv.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4073 2023-07-30 19:37:15.000000 neuralprocesses-0.2.2/neuralprocesses/coders/shaping.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4362 2023-07-30 19:37:15.000000 neuralprocesses-0.2.2/neuralprocesses/coding.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 19:37:25.299177 neuralprocesses-0.2.2/neuralprocesses/data/
+-rw-r--r--   0 runner    (1001) docker     (123)      223 2023-07-30 19:37:15.000000 neuralprocesses-0.2.2/neuralprocesses/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11033 2023-07-30 19:37:15.000000 neuralprocesses-0.2.2/neuralprocesses/data/antarctica.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3318 2023-07-30 19:37:15.000000 neuralprocesses-0.2.2/neuralprocesses/data/batch.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2333 2023-07-30 19:37:15.000000 neuralprocesses-0.2.2/neuralprocesses/data/bimodal.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14216 2023-07-30 19:37:15.000000 neuralprocesses-0.2.2/neuralprocesses/data/data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6860 2023-07-30 19:37:15.000000 neuralprocesses-0.2.2/neuralprocesses/data/eeg.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3880 2023-07-30 19:37:15.000000 neuralprocesses-0.2.2/neuralprocesses/data/gp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3033 2023-07-30 19:37:15.000000 neuralprocesses-0.2.2/neuralprocesses/data/mixgp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1152 2023-07-30 19:37:15.000000 neuralprocesses-0.2.2/neuralprocesses/data/mixture.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5400 2023-07-30 19:37:15.000000 neuralprocesses-0.2.2/neuralprocesses/data/predefined.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12613 2023-07-30 19:37:15.000000 neuralprocesses-0.2.2/neuralprocesses/data/predprey.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2414 2023-07-30 19:37:15.000000 neuralprocesses-0.2.2/neuralprocesses/data/sawtooth.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27362 2023-07-30 19:37:15.000000 neuralprocesses-0.2.2/neuralprocesses/data/temperature.py
+-rw-r--r--   0 runner    (1001) docker     (123)      544 2023-07-30 19:37:15.000000 neuralprocesses-0.2.2/neuralprocesses/data/util.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1578 2023-07-30 19:37:15.000000 neuralprocesses-0.2.2/neuralprocesses/datadims.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5015 2023-07-30 19:37:15.000000 neuralprocesses-0.2.2/neuralprocesses/disc.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 19:37:25.303176 neuralprocesses-0.2.2/neuralprocesses/dist/
+-rw-r--r--   0 runner    (1001) docker     (123)      178 2023-07-30 19:37:15.000000 neuralprocesses-0.2.2/neuralprocesses/dist/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3397 2023-07-30 19:37:15.000000 neuralprocesses-0.2.2/neuralprocesses/dist/beta.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2547 2023-07-30 19:37:15.000000 neuralprocesses-0.2.2/neuralprocesses/dist/dirac.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3430 2023-07-30 19:37:15.000000 neuralprocesses-0.2.2/neuralprocesses/dist/dist.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2002 2023-07-30 19:37:15.000000 neuralprocesses-0.2.2/neuralprocesses/dist/geom.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8774 2023-07-30 19:37:15.000000 neuralprocesses-0.2.2/neuralprocesses/dist/normal.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7430 2023-07-30 19:37:15.000000 neuralprocesses-0.2.2/neuralprocesses/dist/spikeslab.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7710 2023-07-30 19:37:15.000000 neuralprocesses-0.2.2/neuralprocesses/dist/transformed.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2178 2023-07-30 19:37:15.000000 neuralprocesses-0.2.2/neuralprocesses/dist/uniform.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11566 2023-07-30 19:37:15.000000 neuralprocesses-0.2.2/neuralprocesses/likelihood.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3638 2023-07-30 19:37:15.000000 neuralprocesses-0.2.2/neuralprocesses/mask.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4935 2023-07-30 19:37:15.000000 neuralprocesses-0.2.2/neuralprocesses/materialise.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 19:37:25.303176 neuralprocesses-0.2.2/neuralprocesses/model/
+-rw-r--r--   0 runner    (1001) docker     (123)      104 2023-07-30 19:37:15.000000 neuralprocesses-0.2.2/neuralprocesses/model/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11392 2023-07-30 19:37:15.000000 neuralprocesses-0.2.2/neuralprocesses/model/ar.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5008 2023-07-30 19:37:15.000000 neuralprocesses-0.2.2/neuralprocesses/model/elbo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3289 2023-07-30 19:37:15.000000 neuralprocesses-0.2.2/neuralprocesses/model/loglik.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3678 2023-07-30 19:37:15.000000 neuralprocesses-0.2.2/neuralprocesses/model/model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4017 2023-07-30 19:37:15.000000 neuralprocesses-0.2.2/neuralprocesses/model/predict.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3248 2023-07-30 19:37:15.000000 neuralprocesses-0.2.2/neuralprocesses/model/util.py
+-rw-r--r--   0 runner    (1001) docker     (123)      679 2023-07-30 19:37:15.000000 neuralprocesses-0.2.2/neuralprocesses/numdata.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3520 2023-07-30 19:37:15.000000 neuralprocesses-0.2.2/neuralprocesses/parallel.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 19:37:25.303176 neuralprocesses-0.2.2/neuralprocesses/tensorflow/
+-rw-r--r--   0 runner    (1001) docker     (123)     1037 2023-07-30 19:37:15.000000 neuralprocesses-0.2.2/neuralprocesses/tensorflow/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10168 2023-07-30 19:37:15.000000 neuralprocesses-0.2.2/neuralprocesses/tensorflow/nn.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 19:37:25.303176 neuralprocesses-0.2.2/neuralprocesses/torch/
+-rw-r--r--   0 runner    (1001) docker     (123)      796 2023-07-30 19:37:15.000000 neuralprocesses-0.2.2/neuralprocesses/torch/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7071 2023-07-30 19:37:15.000000 neuralprocesses-0.2.2/neuralprocesses/torch/nn.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6413 2023-07-30 19:37:15.000000 neuralprocesses-0.2.2/neuralprocesses/util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 19:37:25.295176 neuralprocesses-0.2.2/neuralprocesses.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2349 2023-07-30 19:37:25.000000 neuralprocesses-0.2.2/neuralprocesses.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3954 2023-07-30 19:37:25.000000 neuralprocesses-0.2.2/neuralprocesses.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-30 19:37:25.000000 neuralprocesses-0.2.2/neuralprocesses.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       98 2023-07-30 19:37:25.000000 neuralprocesses-0.2.2/neuralprocesses.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-07-30 19:37:25.000000 neuralprocesses-0.2.2/neuralprocesses.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      242 2023-07-30 19:37:15.000000 neuralprocesses-0.2.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      232 2023-07-30 19:37:15.000000 neuralprocesses-0.2.2/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    11863 2023-07-30 19:37:15.000000 neuralprocesses-0.2.2/schedule.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 19:37:25.303176 neuralprocesses-0.2.2/scripts/
+-rw-r--r--   0 runner    (1001) docker     (123)     4120 2023-07-30 19:37:15.000000 neuralprocesses-0.2.2/scripts/predprey.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1056 2023-07-30 19:37:15.000000 neuralprocesses-0.2.2/scripts/predprey_visualise.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3080 2023-07-30 19:37:15.000000 neuralprocesses-0.2.2/scripts/sawtooth_sample_ar.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3863 2023-07-30 19:37:15.000000 neuralprocesses-0.2.2/scripts/synthetic_extra.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15625 2023-07-30 19:37:15.000000 neuralprocesses-0.2.2/scripts/synthetic_parse.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2078 2023-07-30 19:37:15.000000 neuralprocesses-0.2.2/scripts/temperature_mae.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2077 2023-07-30 19:37:15.000000 neuralprocesses-0.2.2/scripts/temperature_summarise_folds.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3838 2023-07-30 19:37:15.000000 neuralprocesses-0.2.2/scripts/temperature_visualise.py
+-rw-r--r--   0 runner    (1001) docker     (123)      379 2023-07-30 19:37:25.307177 neuralprocesses-0.2.2/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (123)      355 2023-07-30 19:37:15.000000 neuralprocesses-0.2.2/setup.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27121 2023-07-30 19:37:15.000000 neuralprocesses-0.2.2/tables.ipynb
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 19:37:25.307177 neuralprocesses-0.2.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      149 2023-07-30 19:37:15.000000 neuralprocesses-0.2.2/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 19:37:25.307177 neuralprocesses-0.2.2/tests/coders/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-30 19:37:15.000000 neuralprocesses-0.2.2/tests/coders/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1048 2023-07-30 19:37:15.000000 neuralprocesses-0.2.2/tests/coders/test_shaping.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 19:37:25.307177 neuralprocesses-0.2.2/tests/dists/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-30 19:37:15.000000 neuralprocesses-0.2.2/tests/dists/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1959 2023-07-30 19:37:15.000000 neuralprocesses-0.2.2/tests/dists/test_normal.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 19:37:25.307177 neuralprocesses-0.2.2/tests/gnp/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-30 19:37:15.000000 neuralprocesses-0.2.2/tests/gnp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1109 2023-07-30 19:37:15.000000 neuralprocesses-0.2.2/tests/gnp/autoencoding.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1100 2023-07-30 19:37:15.000000 neuralprocesses-0.2.2/tests/gnp/gnp.py
+-rw-r--r--   0 runner    (1001) docker     (123)      527 2023-07-30 19:37:15.000000 neuralprocesses-0.2.2/tests/gnp/util.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13948 2023-07-30 19:37:15.000000 neuralprocesses-0.2.2/tests/test_architectures.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1769 2023-07-30 19:37:15.000000 neuralprocesses-0.2.2/tests/test_augment.py
+-rw-r--r--   0 runner    (1001) docker     (123)      340 2023-07-30 19:37:15.000000 neuralprocesses-0.2.2/tests/test_chain.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8001 2023-07-30 19:37:15.000000 neuralprocesses-0.2.2/tests/test_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)      806 2023-07-30 19:37:15.000000 neuralprocesses-0.2.2/tests/test_discretisation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1255 2023-07-30 19:37:15.000000 neuralprocesses-0.2.2/tests/test_distribution.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1749 2023-07-30 19:37:15.000000 neuralprocesses-0.2.2/tests/test_mask.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1534 2023-07-30 19:37:15.000000 neuralprocesses-0.2.2/tests/test_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1853 2023-07-30 19:37:15.000000 neuralprocesses-0.2.2/tests/test_unet.py
+-rw-r--r--   0 runner    (1001) docker     (123)      268 2023-07-30 19:37:15.000000 neuralprocesses-0.2.2/tests/test_util.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1930 2023-07-30 19:37:15.000000 neuralprocesses-0.2.2/tests/util.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9301 2023-07-30 19:37:15.000000 neuralprocesses-0.2.2/todo.tasks
+-rw-r--r--   0 runner    (1001) docker     (123)    26899 2023-07-30 19:37:15.000000 neuralprocesses-0.2.2/train.py
```

### Comparing `neuralprocesses-0.2.1/.github/workflows/build_book.yml` & `neuralprocesses-0.2.2/.github/workflows/build_book.yml`

 * *Files identical despite different names*

### Comparing `neuralprocesses-0.2.1/.github/workflows/ci.yml` & `neuralprocesses-0.2.2/.github/workflows/ci.yml`

 * *Files identical despite different names*

### Comparing `neuralprocesses-0.2.1/.github/workflows/publish.yml` & `neuralprocesses-0.2.2/.github/workflows/publish.yml`

 * *Files identical despite different names*

### Comparing `neuralprocesses-0.2.1/.github/workflows/style.yml` & `neuralprocesses-0.2.2/.github/workflows/style.yml`

 * *Files identical despite different names*

### Comparing `neuralprocesses-0.2.1/LICENCE.txt` & `neuralprocesses-0.2.2/LICENCE.txt`

 * *Files identical despite different names*

### Comparing `neuralprocesses-0.2.1/PKG-INFO` & `neuralprocesses-0.2.2/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: neuralprocesses
-Version: 0.2.1
+Version: 0.2.2
 Summary: A framework for composing Neural Processes in Python
 Home-page: https://github.com/wesselb/neuralprocesses
 Author: Wessel Bruinsma
 Author-email: wessel.p.bruinsma@gmail.com
 License: MIT
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
```

### Comparing `neuralprocesses-0.2.1/README.md` & `neuralprocesses-0.2.2/README.md`

 * *Files identical despite different names*

### Comparing `neuralprocesses-0.2.1/docs/_config.yml` & `neuralprocesses-0.2.2/docs/_config.yml`

 * *Files identical despite different names*

### Comparing `neuralprocesses-0.2.1/docs/advanced_usage.md` & `neuralprocesses-0.2.2/docs/advanced_usage.md`

 * *Files identical despite different names*

### Comparing `neuralprocesses-0.2.1/docs/architectures.rst` & `neuralprocesses-0.2.2/docs/architectures.rst`

 * *Files identical despite different names*

### Comparing `neuralprocesses-0.2.1/docs/basic_usage.md` & `neuralprocesses-0.2.2/docs/basic_usage.md`

 * *Files identical despite different names*

### Comparing `neuralprocesses-0.2.1/docs/build_your_own_model.md` & `neuralprocesses-0.2.2/docs/build_your_own_model.md`

 * *Files identical despite different names*

### Comparing `neuralprocesses-0.2.1/docs/coders.rst` & `neuralprocesses-0.2.2/docs/coders.rst`

 * *Files identical despite different names*

### Comparing `neuralprocesses-0.2.1/docs/logo.png` & `neuralprocesses-0.2.2/docs/logo.png`

 * *Files identical despite different names*

### Comparing `neuralprocesses-0.2.1/experiment/data/antarctica.py` & `neuralprocesses-0.2.2/experiment/data/antarctica.py`

 * *Files identical despite different names*

### Comparing `neuralprocesses-0.2.1/experiment/data/eeg.py` & `neuralprocesses-0.2.2/experiment/data/eeg.py`

 * *Files identical despite different names*

### Comparing `neuralprocesses-0.2.1/experiment/data/gp.py` & `neuralprocesses-0.2.2/experiment/data/gp.py`

 * *Files identical despite different names*

### Comparing `neuralprocesses-0.2.1/experiment/data/predprey.py` & `neuralprocesses-0.2.2/experiment/data/predprey.py`

 * *Files identical despite different names*

### Comparing `neuralprocesses-0.2.1/experiment/data/temperature.py` & `neuralprocesses-0.2.2/experiment/data/temperature.py`

 * *Files identical despite different names*

### Comparing `neuralprocesses-0.2.1/experiment/data/util.py` & `neuralprocesses-0.2.2/experiment/data/util.py`

 * *Files identical despite different names*

### Comparing `neuralprocesses-0.2.1/experiment/plot.py` & `neuralprocesses-0.2.2/experiment/plot.py`

 * *Files identical despite different names*

### Comparing `neuralprocesses-0.2.1/experiment/util.py` & `neuralprocesses-0.2.2/experiment/util.py`

 * *Files identical despite different names*

### Comparing `neuralprocesses-0.2.1/neuralprocesses/__init__.py` & `neuralprocesses-0.2.2/neuralprocesses/__init__.py`

 * *Files identical despite different names*

### Comparing `neuralprocesses-0.2.1/neuralprocesses/aggregate.py` & `neuralprocesses-0.2.2/neuralprocesses/aggregate.py`

 * *Files identical despite different names*

### Comparing `neuralprocesses-0.2.1/neuralprocesses/architectures/agnp.py` & `neuralprocesses-0.2.2/neuralprocesses/architectures/agnp.py`

 * *Files identical despite different names*

### Comparing `neuralprocesses-0.2.1/neuralprocesses/architectures/climate.py` & `neuralprocesses-0.2.2/neuralprocesses/architectures/climate.py`

 * *Files identical despite different names*

### Comparing `neuralprocesses-0.2.1/neuralprocesses/architectures/convgnp.py` & `neuralprocesses-0.2.2/neuralprocesses/architectures/convgnp.py`

 * *Files identical despite different names*

### Comparing `neuralprocesses-0.2.1/neuralprocesses/architectures/fullconvgnp.py` & `neuralprocesses-0.2.2/neuralprocesses/architectures/fullconvgnp.py`

 * *Files identical despite different names*

### Comparing `neuralprocesses-0.2.1/neuralprocesses/architectures/gnp.py` & `neuralprocesses-0.2.2/neuralprocesses/architectures/gnp.py`

 * *Files identical despite different names*

### Comparing `neuralprocesses-0.2.1/neuralprocesses/architectures/util.py` & `neuralprocesses-0.2.2/neuralprocesses/architectures/util.py`

 * *Files identical despite different names*

### Comparing `neuralprocesses-0.2.1/neuralprocesses/augment.py` & `neuralprocesses-0.2.2/neuralprocesses/augment.py`

 * *Files identical despite different names*

### Comparing `neuralprocesses-0.2.1/neuralprocesses/chain.py` & `neuralprocesses-0.2.2/neuralprocesses/chain.py`

 * *Files identical despite different names*

### Comparing `neuralprocesses-0.2.1/neuralprocesses/coders/aggregate.py` & `neuralprocesses-0.2.2/neuralprocesses/coders/aggregate.py`

 * *Files identical despite different names*

### Comparing `neuralprocesses-0.2.1/neuralprocesses/coders/attention.py` & `neuralprocesses-0.2.2/neuralprocesses/coders/attention.py`

 * *Files identical despite different names*

### Comparing `neuralprocesses-0.2.1/neuralprocesses/coders/augment.py` & `neuralprocesses-0.2.2/neuralprocesses/coders/augment.py`

 * *Files identical despite different names*

### Comparing `neuralprocesses-0.2.1/neuralprocesses/coders/deepset.py` & `neuralprocesses-0.2.2/neuralprocesses/coders/deepset.py`

 * *Files identical despite different names*

### Comparing `neuralprocesses-0.2.1/neuralprocesses/coders/densecov.py` & `neuralprocesses-0.2.2/neuralprocesses/coders/densecov.py`

 * *Files identical despite different names*

### Comparing `neuralprocesses-0.2.1/neuralprocesses/coders/functional.py` & `neuralprocesses-0.2.2/neuralprocesses/coders/functional.py`

 * *Files identical despite different names*

### Comparing `neuralprocesses-0.2.1/neuralprocesses/coders/fuse.py` & `neuralprocesses-0.2.2/neuralprocesses/coders/fuse.py`

 * *Files identical despite different names*

### Comparing `neuralprocesses-0.2.1/neuralprocesses/coders/mapdiag.py` & `neuralprocesses-0.2.2/neuralprocesses/coders/mapdiag.py`

 * *Files identical despite different names*

### Comparing `neuralprocesses-0.2.1/neuralprocesses/coders/nn.py` & `neuralprocesses-0.2.2/neuralprocesses/coders/nn.py`

 * *Files identical despite different names*

### Comparing `neuralprocesses-0.2.1/neuralprocesses/coders/setconv/density.py` & `neuralprocesses-0.2.2/neuralprocesses/coders/setconv/density.py`

 * *Files identical despite different names*

### Comparing `neuralprocesses-0.2.1/neuralprocesses/coders/setconv/identity.py` & `neuralprocesses-0.2.2/neuralprocesses/coders/setconv/identity.py`

 * *Files identical despite different names*

### Comparing `neuralprocesses-0.2.1/neuralprocesses/coders/setconv/setconv.py` & `neuralprocesses-0.2.2/neuralprocesses/coders/setconv/setconv.py`

 * *Files identical despite different names*

### Comparing `neuralprocesses-0.2.1/neuralprocesses/coders/shaping.py` & `neuralprocesses-0.2.2/neuralprocesses/coders/shaping.py`

 * *Files identical despite different names*

### Comparing `neuralprocesses-0.2.1/neuralprocesses/coding.py` & `neuralprocesses-0.2.2/neuralprocesses/coding.py`

 * *Files identical despite different names*

### Comparing `neuralprocesses-0.2.1/neuralprocesses/data/antarctica.py` & `neuralprocesses-0.2.2/neuralprocesses/data/antarctica.py`

 * *Files identical despite different names*

### Comparing `neuralprocesses-0.2.1/neuralprocesses/data/batch.py` & `neuralprocesses-0.2.2/neuralprocesses/data/batch.py`

 * *Files identical despite different names*

### Comparing `neuralprocesses-0.2.1/neuralprocesses/data/bimodal.py` & `neuralprocesses-0.2.2/neuralprocesses/data/bimodal.py`

 * *Files identical despite different names*

### Comparing `neuralprocesses-0.2.1/neuralprocesses/data/data.py` & `neuralprocesses-0.2.2/neuralprocesses/data/data.py`

 * *Files identical despite different names*

### Comparing `neuralprocesses-0.2.1/neuralprocesses/data/eeg.py` & `neuralprocesses-0.2.2/neuralprocesses/data/eeg.py`

 * *Files identical despite different names*

### Comparing `neuralprocesses-0.2.1/neuralprocesses/data/gp.py` & `neuralprocesses-0.2.2/neuralprocesses/data/gp.py`

 * *Files identical despite different names*

### Comparing `neuralprocesses-0.2.1/neuralprocesses/data/mixgp.py` & `neuralprocesses-0.2.2/neuralprocesses/data/mixgp.py`

 * *Files identical despite different names*

### Comparing `neuralprocesses-0.2.1/neuralprocesses/data/mixture.py` & `neuralprocesses-0.2.2/neuralprocesses/data/mixture.py`

 * *Files identical despite different names*

### Comparing `neuralprocesses-0.2.1/neuralprocesses/data/predefined.py` & `neuralprocesses-0.2.2/neuralprocesses/data/predefined.py`

 * *Files identical despite different names*

### Comparing `neuralprocesses-0.2.1/neuralprocesses/data/predprey.py` & `neuralprocesses-0.2.2/neuralprocesses/data/predprey.py`

 * *Files identical despite different names*

### Comparing `neuralprocesses-0.2.1/neuralprocesses/data/sawtooth.py` & `neuralprocesses-0.2.2/neuralprocesses/data/sawtooth.py`

 * *Files identical despite different names*

### Comparing `neuralprocesses-0.2.1/neuralprocesses/data/temperature.py` & `neuralprocesses-0.2.2/neuralprocesses/data/temperature.py`

 * *Files identical despite different names*

### Comparing `neuralprocesses-0.2.1/neuralprocesses/data/util.py` & `neuralprocesses-0.2.2/neuralprocesses/data/util.py`

 * *Files identical despite different names*

### Comparing `neuralprocesses-0.2.1/neuralprocesses/datadims.py` & `neuralprocesses-0.2.2/neuralprocesses/datadims.py`

 * *Files identical despite different names*

### Comparing `neuralprocesses-0.2.1/neuralprocesses/disc.py` & `neuralprocesses-0.2.2/neuralprocesses/disc.py`

 * *Files identical despite different names*

### Comparing `neuralprocesses-0.2.1/neuralprocesses/dist/beta.py` & `neuralprocesses-0.2.2/neuralprocesses/dist/beta.py`

 * *Files identical despite different names*

### Comparing `neuralprocesses-0.2.1/neuralprocesses/dist/dirac.py` & `neuralprocesses-0.2.2/neuralprocesses/dist/dirac.py`

 * *Files identical despite different names*

### Comparing `neuralprocesses-0.2.1/neuralprocesses/dist/dist.py` & `neuralprocesses-0.2.2/neuralprocesses/dist/dist.py`

 * *Files identical despite different names*

### Comparing `neuralprocesses-0.2.1/neuralprocesses/dist/geom.py` & `neuralprocesses-0.2.2/neuralprocesses/dist/geom.py`

 * *Files identical despite different names*

### Comparing `neuralprocesses-0.2.1/neuralprocesses/dist/normal.py` & `neuralprocesses-0.2.2/neuralprocesses/dist/normal.py`

 * *Files identical despite different names*

### Comparing `neuralprocesses-0.2.1/neuralprocesses/dist/spikeslab.py` & `neuralprocesses-0.2.2/neuralprocesses/dist/spikeslab.py`

 * *Files identical despite different names*

### Comparing `neuralprocesses-0.2.1/neuralprocesses/dist/transformed.py` & `neuralprocesses-0.2.2/neuralprocesses/dist/transformed.py`

 * *Files identical despite different names*

### Comparing `neuralprocesses-0.2.1/neuralprocesses/dist/uniform.py` & `neuralprocesses-0.2.2/neuralprocesses/dist/uniform.py`

 * *Files identical despite different names*

### Comparing `neuralprocesses-0.2.1/neuralprocesses/likelihood.py` & `neuralprocesses-0.2.2/neuralprocesses/likelihood.py`

 * *Files identical despite different names*

### Comparing `neuralprocesses-0.2.1/neuralprocesses/mask.py` & `neuralprocesses-0.2.2/neuralprocesses/mask.py`

 * *Files 12% similar despite different names*

```diff
@@ -36,23 +36,32 @@
     axis = resolve_axis(x, axis)
     shape = list(B.shape(x))
     shape[axis] = up_to - shape[axis]
     with B.on_device(x):
         return B.concat(x, B.zeros(B.dtype(x), *shape), axis=axis)
 
 
+def _ceil_to_closest_multiple(n, m):
+    d, r = divmod(n, m)
+    # If `n` is zero, then we must also round up.
+    if n == 0 or r > 0:
+        return (d + 1) * m
+    else:
+        return d * m
+
+
 @_dispatch
 def _determine_ns(xc: tuple, multiple: Union[int, tuple]):
     ns = [B.shape(xci, 2) for xci in xc]
 
     if not isinstance(multiple, tuple):
         multiple = (multiple,) * len(ns)
 
     # Ceil to the closest multiple of `multiple`.
-    ns = [((n - 1) // m + 1) * m for n, m in zip(ns, multiple)]
+    ns = [_ceil_to_closest_multiple(n, m) for n, m in zip(ns, multiple)]
 
     return ns
 
 
 @_dispatch
 def mask_context(xc: tuple, yc: B.Numeric, multiple=1):
     """Mask a context set.
```

### Comparing `neuralprocesses-0.2.1/neuralprocesses/materialise.py` & `neuralprocesses-0.2.2/neuralprocesses/materialise.py`

 * *Files identical despite different names*

### Comparing `neuralprocesses-0.2.1/neuralprocesses/model/ar.py` & `neuralprocesses-0.2.2/neuralprocesses/model/ar.py`

 * *Files identical despite different names*

### Comparing `neuralprocesses-0.2.1/neuralprocesses/model/elbo.py` & `neuralprocesses-0.2.2/neuralprocesses/model/elbo.py`

 * *Files identical despite different names*

### Comparing `neuralprocesses-0.2.1/neuralprocesses/model/loglik.py` & `neuralprocesses-0.2.2/neuralprocesses/model/loglik.py`

 * *Files identical despite different names*

### Comparing `neuralprocesses-0.2.1/neuralprocesses/model/model.py` & `neuralprocesses-0.2.2/neuralprocesses/model/model.py`

 * *Files identical despite different names*

### Comparing `neuralprocesses-0.2.1/neuralprocesses/model/predict.py` & `neuralprocesses-0.2.2/neuralprocesses/model/predict.py`

 * *Files identical despite different names*

### Comparing `neuralprocesses-0.2.1/neuralprocesses/model/util.py` & `neuralprocesses-0.2.2/neuralprocesses/model/util.py`

 * *Files identical despite different names*

### Comparing `neuralprocesses-0.2.1/neuralprocesses/numdata.py` & `neuralprocesses-0.2.2/neuralprocesses/numdata.py`

 * *Files identical despite different names*

### Comparing `neuralprocesses-0.2.1/neuralprocesses/parallel.py` & `neuralprocesses-0.2.2/neuralprocesses/parallel.py`

 * *Files identical despite different names*

### Comparing `neuralprocesses-0.2.1/neuralprocesses/tensorflow/__init__.py` & `neuralprocesses-0.2.2/neuralprocesses/tensorflow/__init__.py`

 * *Files identical despite different names*

### Comparing `neuralprocesses-0.2.1/neuralprocesses/tensorflow/nn.py` & `neuralprocesses-0.2.2/neuralprocesses/tensorflow/nn.py`

 * *Files identical despite different names*

### Comparing `neuralprocesses-0.2.1/neuralprocesses/torch/__init__.py` & `neuralprocesses-0.2.2/neuralprocesses/torch/__init__.py`

 * *Files identical despite different names*

### Comparing `neuralprocesses-0.2.1/neuralprocesses/torch/nn.py` & `neuralprocesses-0.2.2/neuralprocesses/torch/nn.py`

 * *Files identical despite different names*

### Comparing `neuralprocesses-0.2.1/neuralprocesses/util.py` & `neuralprocesses-0.2.2/neuralprocesses/util.py`

 * *Files identical despite different names*

### Comparing `neuralprocesses-0.2.1/neuralprocesses.egg-info/PKG-INFO` & `neuralprocesses-0.2.2/neuralprocesses.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: neuralprocesses
-Version: 0.2.1
+Version: 0.2.2
 Summary: A framework for composing Neural Processes in Python
 Home-page: https://github.com/wesselb/neuralprocesses
 Author: Wessel Bruinsma
 Author-email: wessel.p.bruinsma@gmail.com
 License: MIT
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
```

### Comparing `neuralprocesses-0.2.1/neuralprocesses.egg-info/SOURCES.txt` & `neuralprocesses-0.2.2/neuralprocesses.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `neuralprocesses-0.2.1/schedule.py` & `neuralprocesses-0.2.2/schedule.py`

 * *Files identical despite different names*

### Comparing `neuralprocesses-0.2.1/scripts/predprey.py` & `neuralprocesses-0.2.2/scripts/predprey.py`

 * *Files identical despite different names*

### Comparing `neuralprocesses-0.2.1/scripts/predprey_visualise.py` & `neuralprocesses-0.2.2/scripts/predprey_visualise.py`

 * *Files identical despite different names*

### Comparing `neuralprocesses-0.2.1/scripts/sawtooth_sample_ar.py` & `neuralprocesses-0.2.2/scripts/sawtooth_sample_ar.py`

 * *Files identical despite different names*

### Comparing `neuralprocesses-0.2.1/scripts/synthetic_extra.py` & `neuralprocesses-0.2.2/scripts/synthetic_extra.py`

 * *Files identical despite different names*

### Comparing `neuralprocesses-0.2.1/scripts/synthetic_parse.py` & `neuralprocesses-0.2.2/scripts/synthetic_parse.py`

 * *Files identical despite different names*

### Comparing `neuralprocesses-0.2.1/scripts/temperature_mae.py` & `neuralprocesses-0.2.2/scripts/temperature_mae.py`

 * *Files identical despite different names*

### Comparing `neuralprocesses-0.2.1/scripts/temperature_summarise_folds.py` & `neuralprocesses-0.2.2/scripts/temperature_summarise_folds.py`

 * *Files identical despite different names*

### Comparing `neuralprocesses-0.2.1/scripts/temperature_visualise.py` & `neuralprocesses-0.2.2/scripts/temperature_visualise.py`

 * *Files identical despite different names*

### Comparing `neuralprocesses-0.2.1/tables.ipynb` & `neuralprocesses-0.2.2/tables.ipynb`

 * *Files identical despite different names*

### Comparing `neuralprocesses-0.2.1/tests/coders/test_shaping.py` & `neuralprocesses-0.2.2/tests/coders/test_shaping.py`

 * *Files identical despite different names*

### Comparing `neuralprocesses-0.2.1/tests/dists/test_normal.py` & `neuralprocesses-0.2.2/tests/dists/test_normal.py`

 * *Files identical despite different names*

### Comparing `neuralprocesses-0.2.1/tests/gnp/autoencoding.py` & `neuralprocesses-0.2.2/tests/gnp/autoencoding.py`

 * *Files identical despite different names*

### Comparing `neuralprocesses-0.2.1/tests/gnp/gnp.py` & `neuralprocesses-0.2.2/tests/gnp/gnp.py`

 * *Files identical despite different names*

### Comparing `neuralprocesses-0.2.1/tests/gnp/util.py` & `neuralprocesses-0.2.2/tests/gnp/util.py`

 * *Files identical despite different names*

### Comparing `neuralprocesses-0.2.1/tests/test_architectures.py` & `neuralprocesses-0.2.2/tests/test_architectures.py`

 * *Files identical despite different names*

### Comparing `neuralprocesses-0.2.1/tests/test_augment.py` & `neuralprocesses-0.2.2/tests/test_augment.py`

 * *Files identical despite different names*

### Comparing `neuralprocesses-0.2.1/tests/test_data.py` & `neuralprocesses-0.2.2/tests/test_data.py`

 * *Files identical despite different names*

### Comparing `neuralprocesses-0.2.1/tests/test_discretisation.py` & `neuralprocesses-0.2.2/tests/test_discretisation.py`

 * *Files identical despite different names*

### Comparing `neuralprocesses-0.2.1/tests/test_distribution.py` & `neuralprocesses-0.2.2/tests/test_distribution.py`

 * *Files identical despite different names*

### Comparing `neuralprocesses-0.2.1/tests/test_model.py` & `neuralprocesses-0.2.2/tests/test_model.py`

 * *Files identical despite different names*

### Comparing `neuralprocesses-0.2.1/tests/test_unet.py` & `neuralprocesses-0.2.2/tests/test_unet.py`

 * *Files identical despite different names*

### Comparing `neuralprocesses-0.2.1/tests/util.py` & `neuralprocesses-0.2.2/tests/util.py`

 * *Files identical despite different names*

### Comparing `neuralprocesses-0.2.1/todo.tasks` & `neuralprocesses-0.2.2/todo.tasks`

 * *Files identical despite different names*

### Comparing `neuralprocesses-0.2.1/train.py` & `neuralprocesses-0.2.2/train.py`

 * *Files identical despite different names*

