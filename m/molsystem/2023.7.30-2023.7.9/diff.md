# Comparing `tmp/molsystem-2023.7.30.tar.gz` & `tmp/molsystem-2023.7.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "molsystem-2023.7.30.tar", last modified: Sun Jul 30 21:28:09 2023, max compression
+gzip compressed data, was "molsystem-2023.7.9.tar", last modified: Mon Jul 10 17:31:09 2023, max compression
```

## Comparing `molsystem-2023.7.30.tar` & `molsystem-2023.7.9.tar`

### file list

```diff
@@ -1,107 +1,104 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 21:28:09.009064 molsystem-2023.7.30/
--rw-r--r--   0 runner    (1001) docker     (123)      147 2023-07-30 21:27:55.000000 molsystem-2023.7.30/AUTHORS.rst
--rw-r--r--   0 runner    (1001) docker     (123)     3246 2023-07-30 21:27:55.000000 molsystem-2023.7.30/CONTRIBUTING.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2544 2023-07-30 21:27:55.000000 molsystem-2023.7.30/HISTORY.rst
--rw-r--r--   0 runner    (1001) docker     (123)     7652 2023-07-30 21:27:55.000000 molsystem-2023.7.30/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      319 2023-07-30 21:27:55.000000 molsystem-2023.7.30/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     7143 2023-07-30 21:28:09.009064 molsystem-2023.7.30/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3702 2023-07-30 21:27:55.000000 molsystem-2023.7.30/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 21:28:08.993064 molsystem-2023.7.30/docs/
--rw-r--r--   0 runner    (1001) docker     (123)     6774 2023-07-30 21:27:55.000000 molsystem-2023.7.30/docs/Makefile
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 21:28:08.997064 molsystem-2023.7.30/docs/_static/
--rw-r--r--   0 runner    (1001) docker     (123)    20790 2023-07-30 21:27:55.000000 molsystem-2023.7.30/docs/_static/SEAMM inverted.png
--rw-r--r--   0 runner    (1001) docker     (123)    17802 2023-07-30 21:27:55.000000 molsystem-2023.7.30/docs/_static/SEAMM logo.png
--rw-r--r--   0 runner    (1001) docker     (123)    79373 2023-07-30 21:27:55.000000 molsystem-2023.7.30/docs/_static/molssi_main_logo.png
--rw-r--r--   0 runner    (1001) docker     (123)    68255 2023-07-30 21:27:55.000000 molsystem-2023.7.30/docs/_static/molssi_main_logo_inverted_white.png
--rw-r--r--   0 runner    (1001) docker     (123)    63967 2023-07-30 21:27:55.000000 molsystem-2023.7.30/docs/_static/molssi_square.png
--rw-r--r--   0 runner    (1001) docker     (123)    32355 2023-07-30 21:27:55.000000 molsystem-2023.7.30/docs/_static/nsf.png
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 21:28:08.997064 molsystem-2023.7.30/docs/api/
--rw-r--r--   0 runner    (1001) docker     (123)      182 2023-07-30 21:27:55.000000 molsystem-2023.7.30/docs/api/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-07-30 21:27:55.000000 molsystem-2023.7.30/docs/authors.rst
--rwxr-xr-x   0 runner    (1001) docker     (123)     9525 2023-07-30 21:27:55.000000 molsystem-2023.7.30/docs/conf.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 21:28:08.997064 molsystem-2023.7.30/docs/developer_guide/
--rw-r--r--   0 runner    (1001) docker     (123)       36 2023-07-30 21:27:55.000000 molsystem-2023.7.30/docs/developer_guide/contributing.rst
--rw-r--r--   0 runner    (1001) docker     (123)      223 2023-07-30 21:27:55.000000 molsystem-2023.7.30/docs/developer_guide/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1147 2023-07-30 21:27:55.000000 molsystem-2023.7.30/docs/developer_guide/installation.rst
--rw-r--r--   0 runner    (1001) docker     (123)       73 2023-07-30 21:27:55.000000 molsystem-2023.7.30/docs/developer_guide/usage.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 21:28:08.997064 molsystem-2023.7.30/docs/getting_started/
--rw-r--r--   0 runner    (1001) docker     (123)     1351 2023-07-30 21:27:55.000000 molsystem-2023.7.30/docs/getting_started/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-07-30 21:27:55.000000 molsystem-2023.7.30/docs/history.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1282 2023-07-30 21:27:55.000000 molsystem-2023.7.30/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)     6465 2023-07-30 21:27:55.000000 molsystem-2023.7.30/docs/make.bat
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 21:28:08.997064 molsystem-2023.7.30/docs/user_guide/
--rw-r--r--   0 runner    (1001) docker     (123)      699 2023-07-30 21:27:55.000000 molsystem-2023.7.30/docs/user_guide/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 21:28:09.009064 molsystem-2023.7.30/molsystem/
--rw-r--r--   0 runner    (1001) docker     (123)      668 2023-07-30 21:27:55.000000 molsystem-2023.7.30/molsystem/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      501 2023-07-30 21:28:09.009064 molsystem-2023.7.30/molsystem/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)    43870 2023-07-30 21:27:55.000000 molsystem-2023.7.30/molsystem/atoms.py
--rw-r--r--   0 runner    (1001) docker     (123)    26433 2023-07-30 21:27:55.000000 molsystem-2023.7.30/molsystem/bonds.py
--rw-r--r--   0 runner    (1001) docker     (123)    19739 2023-07-30 21:27:55.000000 molsystem-2023.7.30/molsystem/cell.py
--rw-r--r--   0 runner    (1001) docker     (123)    33626 2023-07-30 21:27:55.000000 molsystem-2023.7.30/molsystem/cif.py
--rw-r--r--   0 runner    (1001) docker     (123)     1524 2023-07-30 21:27:55.000000 molsystem-2023.7.30/molsystem/cms_schema.py
--rw-r--r--   0 runner    (1001) docker     (123)     3579 2023-07-30 21:27:55.000000 molsystem-2023.7.30/molsystem/column.py
--rw-r--r--   0 runner    (1001) docker     (123)    29395 2023-07-30 21:27:55.000000 molsystem-2023.7.30/molsystem/configuration.py
--rw-r--r--   0 runner    (1001) docker     (123)     6062 2023-07-30 21:27:55.000000 molsystem-2023.7.30/molsystem/configuration_properties.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 21:28:09.001064 molsystem-2023.7.30/molsystem/data/
--rw-r--r--   0 runner    (1001) docker     (123)     1781 2023-07-30 21:27:55.000000 molsystem-2023.7.30/molsystem/data/standard_properties.csv
--rw-r--r--   0 runner    (1001) docker     (123)    26799 2023-07-30 21:27:55.000000 molsystem-2023.7.30/molsystem/elements.py
--rw-r--r--   0 runner    (1001) docker     (123)     2377 2023-07-30 21:27:55.000000 molsystem-2023.7.30/molsystem/frozencolumn.py
--rw-r--r--   0 runner    (1001) docker     (123)     4491 2023-07-30 21:27:55.000000 molsystem-2023.7.30/molsystem/inchi.py
--rw-r--r--   0 runner    (1001) docker     (123)     6557 2023-07-30 21:27:55.000000 molsystem-2023.7.30/molsystem/molfile.py
--rw-r--r--   0 runner    (1001) docker     (123)     4858 2023-07-30 21:27:55.000000 molsystem-2023.7.30/molsystem/openbabel.py
--rw-r--r--   0 runner    (1001) docker     (123)    18217 2023-07-30 21:27:55.000000 molsystem-2023.7.30/molsystem/pdb.py
--rw-r--r--   0 runner    (1001) docker     (123)    33067 2023-07-30 21:27:55.000000 molsystem-2023.7.30/molsystem/properties.py
--rw-r--r--   0 runner    (1001) docker     (123)     3100 2023-07-30 21:27:55.000000 molsystem-2023.7.30/molsystem/qcschema.py
--rw-r--r--   0 runner    (1001) docker     (123)     3441 2023-07-30 21:27:55.000000 molsystem-2023.7.30/molsystem/rdkit_.py
--rw-r--r--   0 runner    (1001) docker     (123)     7191 2023-07-30 21:27:55.000000 molsystem-2023.7.30/molsystem/smiles.py
--rw-r--r--   0 runner    (1001) docker     (123)     2595 2023-07-30 21:27:55.000000 molsystem-2023.7.30/molsystem/subset.py
--rw-r--r--   0 runner    (1001) docker     (123)     6376 2023-07-30 21:27:55.000000 molsystem-2023.7.30/molsystem/subsets.py
--rw-r--r--   0 runner    (1001) docker     (123)     4294 2023-07-30 21:27:55.000000 molsystem-2023.7.30/molsystem/symmetry.py
--rw-r--r--   0 runner    (1001) docker     (123)    19366 2023-07-30 21:27:55.000000 molsystem-2023.7.30/molsystem/system.py
--rw-r--r--   0 runner    (1001) docker     (123)    35772 2023-07-30 21:27:55.000000 molsystem-2023.7.30/molsystem/system_db.py
--rw-r--r--   0 runner    (1001) docker     (123)     5588 2023-07-30 21:27:55.000000 molsystem-2023.7.30/molsystem/system_properties.py
--rw-r--r--   0 runner    (1001) docker     (123)    26830 2023-07-30 21:27:55.000000 molsystem-2023.7.30/molsystem/table.py
--rw-r--r--   0 runner    (1001) docker     (123)     7916 2023-07-30 21:27:55.000000 molsystem-2023.7.30/molsystem/template.py
--rw-r--r--   0 runner    (1001) docker     (123)     8247 2023-07-30 21:27:55.000000 molsystem-2023.7.30/molsystem/templates.py
--rw-r--r--   0 runner    (1001) docker     (123)    17862 2023-07-30 21:27:55.000000 molsystem-2023.7.30/molsystem/topology.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 21:28:09.001064 molsystem-2023.7.30/molsystem.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     7143 2023-07-30 21:28:08.000000 molsystem-2023.7.30/molsystem.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2156 2023-07-30 21:28:08.000000 molsystem-2023.7.30/molsystem.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-30 21:28:08.000000 molsystem-2023.7.30/molsystem.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       34 2023-07-30 21:28:08.000000 molsystem-2023.7.30/molsystem.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-07-30 21:28:08.000000 molsystem-2023.7.30/molsystem.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      357 2023-07-30 21:28:09.009064 molsystem-2023.7.30/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2672 2023-07-30 21:27:55.000000 molsystem-2023.7.30/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 21:28:09.005064 molsystem-2023.7.30/tests/
--rw-r--r--   0 runner    (1001) docker     (123)       64 2023-07-30 21:27:55.000000 molsystem-2023.7.30/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13045 2023-07-30 21:27:55.000000 molsystem-2023.7.30/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 21:28:09.009064 molsystem-2023.7.30/tests/data/
--rw-r--r--   0 runner    (1001) docker     (123)   269083 2023-07-30 21:27:55.000000 molsystem-2023.7.30/tests/data/1n9v.cif
--rw-r--r--   0 runner    (1001) docker     (123)  1055288 2023-07-30 21:27:55.000000 molsystem-2023.7.30/tests/data/aa-variants-v1.cif
--rw-r--r--   0 runner    (1001) docker     (123)     4318 2023-07-30 21:27:55.000000 molsystem-2023.7.30/tests/data/acy.mmcif
--rw-r--r--   0 runner    (1001) docker     (123)   117392 2023-07-30 21:27:55.000000 molsystem-2023.7.30/tests/data/aminoacids.mmcif
--rw-r--r--   0 runner    (1001) docker     (123)     3692 2023-07-30 21:27:55.000000 molsystem-2023.7.30/tests/data/hoh.mmcif
--rw-r--r--   0 runner    (1001) docker     (123)     8016 2023-07-30 21:27:55.000000 molsystem-2023.7.30/tests/test_angiotensin.py
--rw-r--r--   0 runner    (1001) docker     (123)    12879 2023-07-30 21:27:55.000000 molsystem-2023.7.30/tests/test_atoms.py
--rw-r--r--   0 runner    (1001) docker     (123)     4415 2023-07-30 21:27:55.000000 molsystem-2023.7.30/tests/test_bonds.py
--rw-r--r--   0 runner    (1001) docker     (123)     2797 2023-07-30 21:27:55.000000 molsystem-2023.7.30/tests/test_cell.py
--rw-r--r--   0 runner    (1001) docker     (123)     7047 2023-07-30 21:27:55.000000 molsystem-2023.7.30/tests/test_cif.py
--rw-r--r--   0 runner    (1001) docker     (123)     1820 2023-07-30 21:27:55.000000 molsystem-2023.7.30/tests/test_configuration_properties.py
--rw-r--r--   0 runner    (1001) docker     (123)     1485 2023-07-30 21:27:55.000000 molsystem-2023.7.30/tests/test_configurations.py
--rw-r--r--   0 runner    (1001) docker     (123)     1804 2023-07-30 21:27:55.000000 molsystem-2023.7.30/tests/test_inchi.py
--rw-r--r--   0 runner    (1001) docker     (123)     3608 2023-07-30 21:27:55.000000 molsystem-2023.7.30/tests/test_molfile.py
--rw-r--r--   0 runner    (1001) docker     (123)    18784 2023-07-30 21:27:55.000000 molsystem-2023.7.30/tests/test_openbabel.py
--rw-r--r--   0 runner    (1001) docker     (123)    10334 2023-07-30 21:27:55.000000 molsystem-2023.7.30/tests/test_pdb.py
--rw-r--r--   0 runner    (1001) docker     (123)     2442 2023-07-30 21:27:55.000000 molsystem-2023.7.30/tests/test_properties.py
--rw-r--r--   0 runner    (1001) docker     (123)     3168 2023-07-30 21:27:55.000000 molsystem-2023.7.30/tests/test_property_timings.py
--rw-r--r--   0 runner    (1001) docker     (123)     2751 2023-07-30 21:27:55.000000 molsystem-2023.7.30/tests/test_qcschema.py
--rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-07-30 21:27:55.000000 molsystem-2023.7.30/tests/test_rdkit.py
--rw-r--r--   0 runner    (1001) docker     (123)     1636 2023-07-30 21:27:55.000000 molsystem-2023.7.30/tests/test_smiles.py
--rw-r--r--   0 runner    (1001) docker     (123)     1733 2023-07-30 21:27:55.000000 molsystem-2023.7.30/tests/test_subsets.py
--rw-r--r--   0 runner    (1001) docker     (123)     2254 2023-07-30 21:27:55.000000 molsystem-2023.7.30/tests/test_system.py
--rw-r--r--   0 runner    (1001) docker     (123)     4633 2023-07-30 21:27:55.000000 molsystem-2023.7.30/tests/test_system_db.py
--rw-r--r--   0 runner    (1001) docker     (123)    14598 2023-07-30 21:27:55.000000 molsystem-2023.7.30/tests/test_table.py
--rw-r--r--   0 runner    (1001) docker     (123)     5837 2023-07-30 21:27:55.000000 molsystem-2023.7.30/tests/test_templates.py
--rw-r--r--   0 runner    (1001) docker     (123)     5719 2023-07-30 21:27:55.000000 molsystem-2023.7.30/tests/test_timings.py
--rw-r--r--   0 runner    (1001) docker     (123)     2988 2023-07-30 21:27:55.000000 molsystem-2023.7.30/tests/test_topology.py
--rw-r--r--   0 runner    (1001) docker     (123)    68611 2023-07-30 21:27:55.000000 molsystem-2023.7.30/versioneer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 17:31:09.740878 molsystem-2023.7.9/
+-rw-r--r--   0 runner    (1001) docker     (123)      147 2023-07-10 17:30:46.000000 molsystem-2023.7.9/AUTHORS.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     3246 2023-07-10 17:30:46.000000 molsystem-2023.7.9/CONTRIBUTING.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1861 2023-07-10 17:30:46.000000 molsystem-2023.7.9/HISTORY.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     7652 2023-07-10 17:30:46.000000 molsystem-2023.7.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      319 2023-07-10 17:30:46.000000 molsystem-2023.7.9/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     6459 2023-07-10 17:31:09.740878 molsystem-2023.7.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3702 2023-07-10 17:30:46.000000 molsystem-2023.7.9/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 17:31:09.724878 molsystem-2023.7.9/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)     6774 2023-07-10 17:30:46.000000 molsystem-2023.7.9/docs/Makefile
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 17:31:09.724878 molsystem-2023.7.9/docs/_static/
+-rw-r--r--   0 runner    (1001) docker     (123)    20790 2023-07-10 17:30:46.000000 molsystem-2023.7.9/docs/_static/SEAMM inverted.png
+-rw-r--r--   0 runner    (1001) docker     (123)    17802 2023-07-10 17:30:46.000000 molsystem-2023.7.9/docs/_static/SEAMM logo.png
+-rw-r--r--   0 runner    (1001) docker     (123)    79373 2023-07-10 17:30:46.000000 molsystem-2023.7.9/docs/_static/molssi_main_logo.png
+-rw-r--r--   0 runner    (1001) docker     (123)    68255 2023-07-10 17:30:46.000000 molsystem-2023.7.9/docs/_static/molssi_main_logo_inverted_white.png
+-rw-r--r--   0 runner    (1001) docker     (123)    63967 2023-07-10 17:30:46.000000 molsystem-2023.7.9/docs/_static/molssi_square.png
+-rw-r--r--   0 runner    (1001) docker     (123)    32355 2023-07-10 17:30:46.000000 molsystem-2023.7.9/docs/_static/nsf.png
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 17:31:09.724878 molsystem-2023.7.9/docs/api/
+-rw-r--r--   0 runner    (1001) docker     (123)      182 2023-07-10 17:30:46.000000 molsystem-2023.7.9/docs/api/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-07-10 17:30:46.000000 molsystem-2023.7.9/docs/authors.rst
+-rwxr-xr-x   0 runner    (1001) docker     (123)     9525 2023-07-10 17:30:46.000000 molsystem-2023.7.9/docs/conf.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 17:31:09.724878 molsystem-2023.7.9/docs/developer_guide/
+-rw-r--r--   0 runner    (1001) docker     (123)       36 2023-07-10 17:30:46.000000 molsystem-2023.7.9/docs/developer_guide/contributing.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      223 2023-07-10 17:30:46.000000 molsystem-2023.7.9/docs/developer_guide/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1147 2023-07-10 17:30:46.000000 molsystem-2023.7.9/docs/developer_guide/installation.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       73 2023-07-10 17:30:46.000000 molsystem-2023.7.9/docs/developer_guide/usage.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 17:31:09.724878 molsystem-2023.7.9/docs/getting_started/
+-rw-r--r--   0 runner    (1001) docker     (123)     1351 2023-07-10 17:30:46.000000 molsystem-2023.7.9/docs/getting_started/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-07-10 17:30:46.000000 molsystem-2023.7.9/docs/history.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1282 2023-07-10 17:30:46.000000 molsystem-2023.7.9/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     6465 2023-07-10 17:30:46.000000 molsystem-2023.7.9/docs/make.bat
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 17:31:09.724878 molsystem-2023.7.9/docs/user_guide/
+-rw-r--r--   0 runner    (1001) docker     (123)      699 2023-07-10 17:30:46.000000 molsystem-2023.7.9/docs/user_guide/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 17:31:09.744878 molsystem-2023.7.9/molsystem/
+-rw-r--r--   0 runner    (1001) docker     (123)      668 2023-07-10 17:30:46.000000 molsystem-2023.7.9/molsystem/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      500 2023-07-10 17:31:09.744878 molsystem-2023.7.9/molsystem/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)    43870 2023-07-10 17:30:46.000000 molsystem-2023.7.9/molsystem/atoms.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26433 2023-07-10 17:30:46.000000 molsystem-2023.7.9/molsystem/bonds.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19739 2023-07-10 17:30:46.000000 molsystem-2023.7.9/molsystem/cell.py
+-rw-r--r--   0 runner    (1001) docker     (123)    33626 2023-07-10 17:30:46.000000 molsystem-2023.7.9/molsystem/cif.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1524 2023-07-10 17:30:46.000000 molsystem-2023.7.9/molsystem/cms_schema.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3579 2023-07-10 17:30:46.000000 molsystem-2023.7.9/molsystem/column.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29349 2023-07-10 17:30:46.000000 molsystem-2023.7.9/molsystem/configuration.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5794 2023-07-10 17:30:46.000000 molsystem-2023.7.9/molsystem/configuration_properties.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 17:31:09.732878 molsystem-2023.7.9/molsystem/data/
+-rw-r--r--   0 runner    (1001) docker     (123)     1781 2023-07-10 17:30:46.000000 molsystem-2023.7.9/molsystem/data/standard_properties.csv
+-rw-r--r--   0 runner    (1001) docker     (123)    26799 2023-07-10 17:30:46.000000 molsystem-2023.7.9/molsystem/elements.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2377 2023-07-10 17:30:46.000000 molsystem-2023.7.9/molsystem/frozencolumn.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6557 2023-07-10 17:30:46.000000 molsystem-2023.7.9/molsystem/molfile.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4826 2023-07-10 17:30:46.000000 molsystem-2023.7.9/molsystem/openbabel.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18217 2023-07-10 17:30:46.000000 molsystem-2023.7.9/molsystem/pdb.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28940 2023-07-10 17:30:46.000000 molsystem-2023.7.9/molsystem/properties.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2920 2023-07-10 17:30:46.000000 molsystem-2023.7.9/molsystem/qcschema.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3441 2023-07-10 17:30:46.000000 molsystem-2023.7.9/molsystem/rdkit_.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5939 2023-07-10 17:30:46.000000 molsystem-2023.7.9/molsystem/smiles.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2553 2023-07-10 17:30:46.000000 molsystem-2023.7.9/molsystem/subset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6376 2023-07-10 17:30:46.000000 molsystem-2023.7.9/molsystem/subsets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4294 2023-07-10 17:30:46.000000 molsystem-2023.7.9/molsystem/symmetry.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19366 2023-07-10 17:30:46.000000 molsystem-2023.7.9/molsystem/system.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32852 2023-07-10 17:30:46.000000 molsystem-2023.7.9/molsystem/system_db.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5300 2023-07-10 17:30:46.000000 molsystem-2023.7.9/molsystem/system_properties.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26830 2023-07-10 17:30:46.000000 molsystem-2023.7.9/molsystem/table.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7874 2023-07-10 17:30:46.000000 molsystem-2023.7.9/molsystem/template.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8247 2023-07-10 17:30:46.000000 molsystem-2023.7.9/molsystem/templates.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17862 2023-07-10 17:30:46.000000 molsystem-2023.7.9/molsystem/topology.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 17:31:09.732878 molsystem-2023.7.9/molsystem.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     6459 2023-07-10 17:31:09.000000 molsystem-2023.7.9/molsystem.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2094 2023-07-10 17:31:09.000000 molsystem-2023.7.9/molsystem.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-10 17:31:09.000000 molsystem-2023.7.9/molsystem.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       34 2023-07-10 17:31:09.000000 molsystem-2023.7.9/molsystem.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-07-10 17:31:09.000000 molsystem-2023.7.9/molsystem.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      357 2023-07-10 17:31:09.740878 molsystem-2023.7.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2672 2023-07-10 17:30:46.000000 molsystem-2023.7.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 17:31:09.736878 molsystem-2023.7.9/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)       64 2023-07-10 17:30:46.000000 molsystem-2023.7.9/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13045 2023-07-10 17:30:46.000000 molsystem-2023.7.9/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 17:31:09.740878 molsystem-2023.7.9/tests/data/
+-rw-r--r--   0 runner    (1001) docker     (123)   269083 2023-07-10 17:30:46.000000 molsystem-2023.7.9/tests/data/1n9v.cif
+-rw-r--r--   0 runner    (1001) docker     (123)  1055288 2023-07-10 17:30:46.000000 molsystem-2023.7.9/tests/data/aa-variants-v1.cif
+-rw-r--r--   0 runner    (1001) docker     (123)     4318 2023-07-10 17:30:46.000000 molsystem-2023.7.9/tests/data/acy.mmcif
+-rw-r--r--   0 runner    (1001) docker     (123)   117392 2023-07-10 17:30:46.000000 molsystem-2023.7.9/tests/data/aminoacids.mmcif
+-rw-r--r--   0 runner    (1001) docker     (123)     3692 2023-07-10 17:30:46.000000 molsystem-2023.7.9/tests/data/hoh.mmcif
+-rw-r--r--   0 runner    (1001) docker     (123)     8016 2023-07-10 17:30:46.000000 molsystem-2023.7.9/tests/test_angiotensin.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12879 2023-07-10 17:30:46.000000 molsystem-2023.7.9/tests/test_atoms.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4415 2023-07-10 17:30:46.000000 molsystem-2023.7.9/tests/test_bonds.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2797 2023-07-10 17:30:46.000000 molsystem-2023.7.9/tests/test_cell.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7047 2023-07-10 17:30:46.000000 molsystem-2023.7.9/tests/test_cif.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1820 2023-07-10 17:30:46.000000 molsystem-2023.7.9/tests/test_configuration_properties.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1485 2023-07-10 17:30:46.000000 molsystem-2023.7.9/tests/test_configurations.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3608 2023-07-10 17:30:46.000000 molsystem-2023.7.9/tests/test_molfile.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18784 2023-07-10 17:30:46.000000 molsystem-2023.7.9/tests/test_openbabel.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10334 2023-07-10 17:30:46.000000 molsystem-2023.7.9/tests/test_pdb.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2442 2023-07-10 17:30:46.000000 molsystem-2023.7.9/tests/test_properties.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3168 2023-07-10 17:30:46.000000 molsystem-2023.7.9/tests/test_property_timings.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-07-10 17:30:46.000000 molsystem-2023.7.9/tests/test_rdkit.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1636 2023-07-10 17:30:46.000000 molsystem-2023.7.9/tests/test_smiles.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1733 2023-07-10 17:30:46.000000 molsystem-2023.7.9/tests/test_subsets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2254 2023-07-10 17:30:46.000000 molsystem-2023.7.9/tests/test_system.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4633 2023-07-10 17:30:46.000000 molsystem-2023.7.9/tests/test_system_db.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14598 2023-07-10 17:30:46.000000 molsystem-2023.7.9/tests/test_table.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5837 2023-07-10 17:30:46.000000 molsystem-2023.7.9/tests/test_templates.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5719 2023-07-10 17:30:46.000000 molsystem-2023.7.9/tests/test_timings.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2988 2023-07-10 17:30:46.000000 molsystem-2023.7.9/tests/test_topology.py
+-rw-r--r--   0 runner    (1001) docker     (123)    68611 2023-07-10 17:30:46.000000 molsystem-2023.7.9/versioneer.py
```

### Comparing `molsystem-2023.7.30/CONTRIBUTING.rst` & `molsystem-2023.7.9/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `molsystem-2023.7.30/HISTORY.rst` & `molsystem-2023.7.9/HISTORY.rst`

 * *Files 16% similar despite different names*

```diff
@@ -1,28 +1,13 @@
 =======
 History
 =======
 
-2023.7.30 -- Improved handling of properties
-    * Added ability to get lists of systems or configurations filtered by name
-    * Improved handling of properties on just a system, not configuration
-    * Added ability to filter properties retrieved
-    * Improved handling of properties when creating OpenBabel OB_MOL object
-      
-2023.7.26 -- Bugfix: error in QCSchema bonds; enhancement: RDKit
-    * Fixed bug in the bond indices in QCSchema
-    * Added ability to use RDKit for SMILES and InChI
-
-2023.7.18.1 -- Added support for creating structures from InChIKeys
-    * Uses PubChem to translate the InChiKey to InChI.
-       
-2023.7.18 -- Added support for InChI and InChIKeys
-
 2023.7.9 -- Added JSON properties
-    * Added properties stored as JSON, which allows, vectors, tensors, etc.
+    * Added properties sotred as JSON, which allows, vectors, tensors, etc.
       
 2023.4.6 -- Enhancements for CIF files
     * Handle uncertainties in CIF files expressed as '(x)' at end of value.
 
 2023.3.30 -- Enhancements to QCSchema support
     * Improved naming of molecule in QCSchema
     * Added creation of configurations from QCSchema objects.
```

### Comparing `molsystem-2023.7.30/LICENSE` & `molsystem-2023.7.9/LICENSE`

 * *Files identical despite different names*

### Comparing `molsystem-2023.7.30/PKG-INFO` & `molsystem-2023.7.9/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: molsystem
-Version: 2023.7.30
+Version: 2023.7.9
 Summary: molsystem
 Home-page: https://github.com/molssi-seamm/molsystem
 Author: Paul Saxe
 Author-email: psaxe@molssi.org
 License: GNU Lesser General Public License v3 or later (LGPLv3+)
 Keywords: molsystem,SEAMM
 Platform: Linux
@@ -110,31 +110,16 @@
 .. _`National Science Foundation`: https://www.nsf.gov
 
 
 =======
 History
 =======
 
-2023.7.30 -- Improved handling of properties
-    * Added ability to get lists of systems or configurations filtered by name
-    * Improved handling of properties on just a system, not configuration
-    * Added ability to filter properties retrieved
-    * Improved handling of properties when creating OpenBabel OB_MOL object
-      
-2023.7.26 -- Bugfix: error in QCSchema bonds; enhancement: RDKit
-    * Fixed bug in the bond indices in QCSchema
-    * Added ability to use RDKit for SMILES and InChI
-
-2023.7.18.1 -- Added support for creating structures from InChIKeys
-    * Uses PubChem to translate the InChiKey to InChI.
-       
-2023.7.18 -- Added support for InChI and InChIKeys
-
 2023.7.9 -- Added JSON properties
-    * Added properties stored as JSON, which allows, vectors, tensors, etc.
+    * Added properties sotred as JSON, which allows, vectors, tensors, etc.
       
 2023.4.6 -- Enhancements for CIF files
     * Handle uncertainties in CIF files expressed as '(x)' at end of value.
 
 2023.3.30 -- Enhancements to QCSchema support
     * Improved naming of molecule in QCSchema
     * Added creation of configurations from QCSchema objects.
```

### Comparing `molsystem-2023.7.30/README.rst` & `molsystem-2023.7.9/README.rst`

 * *Files identical despite different names*

### Comparing `molsystem-2023.7.30/docs/Makefile` & `molsystem-2023.7.9/docs/Makefile`

 * *Files identical despite different names*

### Comparing `molsystem-2023.7.30/docs/_static/SEAMM inverted.png` & `molsystem-2023.7.9/docs/_static/SEAMM inverted.png`

 * *Files identical despite different names*

### Comparing `molsystem-2023.7.30/docs/_static/SEAMM logo.png` & `molsystem-2023.7.9/docs/_static/SEAMM logo.png`

 * *Files identical despite different names*

### Comparing `molsystem-2023.7.30/docs/_static/molssi_main_logo.png` & `molsystem-2023.7.9/docs/_static/molssi_main_logo.png`

 * *Files identical despite different names*

### Comparing `molsystem-2023.7.30/docs/_static/molssi_main_logo_inverted_white.png` & `molsystem-2023.7.9/docs/_static/molssi_main_logo_inverted_white.png`

 * *Files identical despite different names*

### Comparing `molsystem-2023.7.30/docs/_static/molssi_square.png` & `molsystem-2023.7.9/docs/_static/molssi_square.png`

 * *Files identical despite different names*

### Comparing `molsystem-2023.7.30/docs/_static/nsf.png` & `molsystem-2023.7.9/docs/_static/nsf.png`

 * *Files identical despite different names*

### Comparing `molsystem-2023.7.30/docs/conf.py` & `molsystem-2023.7.9/docs/conf.py`

 * *Files identical despite different names*

### Comparing `molsystem-2023.7.30/docs/developer_guide/installation.rst` & `molsystem-2023.7.9/docs/developer_guide/installation.rst`

 * *Files identical despite different names*

### Comparing `molsystem-2023.7.30/docs/getting_started/index.rst` & `molsystem-2023.7.9/docs/getting_started/index.rst`

 * *Files identical despite different names*

### Comparing `molsystem-2023.7.30/docs/index.rst` & `molsystem-2023.7.9/docs/index.rst`

 * *Files identical despite different names*

### Comparing `molsystem-2023.7.30/docs/make.bat` & `molsystem-2023.7.9/docs/make.bat`

 * *Files identical despite different names*

### Comparing `molsystem-2023.7.30/docs/user_guide/index.rst` & `molsystem-2023.7.9/docs/user_guide/index.rst`

 * *Files identical despite different names*

### Comparing `molsystem-2023.7.30/molsystem/__init__.py` & `molsystem-2023.7.9/molsystem/__init__.py`

 * *Files identical despite different names*

### Comparing `molsystem-2023.7.30/molsystem/atoms.py` & `molsystem-2023.7.9/molsystem/atoms.py`

 * *Files identical despite different names*

### Comparing `molsystem-2023.7.30/molsystem/bonds.py` & `molsystem-2023.7.9/molsystem/bonds.py`

 * *Files identical despite different names*

### Comparing `molsystem-2023.7.30/molsystem/cell.py` & `molsystem-2023.7.9/molsystem/cell.py`

 * *Files identical despite different names*

### Comparing `molsystem-2023.7.30/molsystem/cif.py` & `molsystem-2023.7.9/molsystem/cif.py`

 * *Files identical despite different names*

### Comparing `molsystem-2023.7.30/molsystem/cms_schema.py` & `molsystem-2023.7.9/molsystem/cms_schema.py`

 * *Files identical despite different names*

### Comparing `molsystem-2023.7.30/molsystem/column.py` & `molsystem-2023.7.9/molsystem/column.py`

 * *Files identical despite different names*

### Comparing `molsystem-2023.7.30/molsystem/configuration.py` & `molsystem-2023.7.9/molsystem/configuration.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,15 +10,14 @@
 
 from .atoms import _Atoms
 from .bonds import _Bonds
 from .cell import _Cell
 from .cif import CIFMixin
 from .cms_schema import CMSSchemaMixin
 from .configuration_properties import _ConfigurationProperties
-from .inchi import InChIMixin
 from .molfile import MolFileMixin
 from .openbabel import OpenBabelMixin
 from .rdkit_ import RDKitMixin
 from .pdb import PDBMixin
 from .qcschema import QCSchemaMixin
 from .smiles import SMILESMixin
 from .subsets import _Subsets
@@ -30,15 +29,14 @@
 
 
 class _Configuration(
     PDBMixin,
     MolFileMixin,
     CIFMixin,
     CMSSchemaMixin,
-    InChIMixin,
     SMILESMixin,
     TopologyMixin,
     OpenBabelMixin,
     RDKitMixin,
     QCSchemaMixin,
     object,
 ):
```

### Comparing `molsystem-2023.7.30/molsystem/configuration_properties.py` & `molsystem-2023.7.9/molsystem/configuration_properties.py`

 * *Files 4% similar despite different names*

```diff
@@ -54,34 +54,28 @@
         """
         return self.properties.description(_property)
 
     def exists(self, name):
         """A thin wrapper of the _Properties method."""
         return self.properties.exists(name)
 
-    def get(self, _property="all", include_system_properties=False):
+    def get(self, _property="all"):
         """Get the given property value for this configuration.
 
         Parameters
         ----------
         _property : int or str
             The id or name of the property.
-        include_system_properties : bool=False
-            Whether to include properties that are on the system, not any configuration
 
         Returns
         -------
         int, float, or str
             The value of the property.
         """
-        return self.properties.get(
-            self._cid,
-            _property,
-            include_system_properties=include_system_properties,
-        )
+        return self.properties.get(self._cid, _property)
 
     def id(self, name):
         """The id for a property
 
         Parameters
         ----------
         name : str
```

### Comparing `molsystem-2023.7.30/molsystem/data/standard_properties.csv` & `molsystem-2023.7.9/molsystem/data/standard_properties.csv`

 * *Files identical despite different names*

### Comparing `molsystem-2023.7.30/molsystem/elements.py` & `molsystem-2023.7.9/molsystem/elements.py`

 * *Files identical despite different names*

### Comparing `molsystem-2023.7.30/molsystem/frozencolumn.py` & `molsystem-2023.7.9/molsystem/frozencolumn.py`

 * *Files identical despite different names*

### Comparing `molsystem-2023.7.30/molsystem/molfile.py` & `molsystem-2023.7.9/molsystem/molfile.py`

 * *Files identical despite different names*

### Comparing `molsystem-2023.7.30/molsystem/openbabel.py` & `molsystem-2023.7.9/molsystem/openbabel.py`

 * *Files 1% similar despite different names*

```diff
@@ -43,15 +43,15 @@
                 self.spin_multiplicity = multiplicity
             ob_mol.SetTotalSpinMultiplicity(self.spin_multiplicity)
 
         # Set local radical character
         ob_mol.AssignSpinMultiplicity(True)
 
         if properties == "all":
-            data = self.properties.get("all", include_system_properties=True)
+            data = self.properties.get("all")
             pair = openbabel.OBPairData()
             for key, value in data.items():
                 pair.SetAttribute(key)
                 pair.SetValue(str(value))
                 ob_mol.CloneData(pair)
 
         return ob_mol
```

### Comparing `molsystem-2023.7.30/molsystem/pdb.py` & `molsystem-2023.7.9/molsystem/pdb.py`

 * *Files identical despite different names*

### Comparing `molsystem-2023.7.30/molsystem/properties.py` & `molsystem-2023.7.9/molsystem/properties.py`

 * *Files 6% similar despite different names*

```diff
@@ -313,102 +313,55 @@
         -------
         bool
             True if the property is registered, False otherwise.
         """
         self.cursor.execute("SELECT COUNT(*) FROM property WHERE name = ?", (name,))
         return self.cursor.fetchone()[0] != 0
 
-    def get(self, configuration_id, _property="all", include_system_properties=False):
+    def get(self, configuration_id, _property="all"):
         """Get the given property value for the configuration.
 
         Parameters
         ----------
         configuration_id : int
             The id of the configuration.
         _property : int or str, or "all"
             The id or name of the property, or all properties if "all".
-        include_system_properties : bool=False
-            Whether to include properties that are on the system, not any configuration
 
         Returns
         -------
         int, float, or str
             The value of the property.
         """
-        if include_system_properties:
-            self.cursor.execute(
-                "SELECT system FROM configuration WHERE id = ?", (configuration_id,)
-            )
-            system_id = self.cursor.fetchone()[0]
-
         if _property == "all":
-            sql = (
-                "SELECT name, type, value\n"
-                "  FROM property, float_data\n"
-                " WHERE float_data.property = property.id AND configuration = ?\n"
-                " UNION \n"
-                "SELECT name, type, value\n"
-                "  FROM property, int_data\n"
-                " WHERE int_data.property = property.id AND configuration = ?\n"
-                " UNION \n"
-                "SELECT name, type, value\n"
-                "  FROM property, str_data\n"
-                " WHERE str_data.property = property.id AND configuration = ?\n"
-                " UNION \n"
-                "SELECT name, type, value\n"
-                "  FROM property, json_data\n"
-                " WHERE json_data.property = property.id AND configuration = ?"
+            sql = "SELECT name, type, value"
+            sql += "  FROM property, float_data"
+            sql += " WHERE float_data.property = property.id AND configuration = ?"
+            sql += " UNION "
+            sql += "SELECT name, type, value"
+            sql += "  FROM property, int_data"
+            sql += " WHERE int_data.property = property.id AND configuration = ?"
+            sql += " UNION "
+            sql += "SELECT name, type, value"
+            sql += "  FROM property, str_data"
+            sql += " WHERE str_data.property = property.id AND configuration = ?"
+            sql += " UNION "
+            sql += "SELECT name, type, value"
+            sql += "  FROM property, json_data"
+            sql += " WHERE json_data.property = property.id AND configuration = ?"
+
+            self.cursor.execute(
+                sql,
+                (
+                    configuration_id,
+                    configuration_id,
+                    configuration_id,
+                    configuration_id,
+                ),
             )
-            if include_system_properties:
-                sql += (
-                    "\n"
-                    " UNION \n"
-                    "SELECT name, type, value\n"
-                    "  FROM property, float_data\n"
-                    " WHERE float_data.property = property.id"
-                    "   AND configuration IS NULL AND system = ?\n"
-                    " UNION \n"
-                    "SELECT name, type, value\n"
-                    "  FROM property, int_data\n"
-                    " WHERE int_data.property = property.id"
-                    "   AND configuration IS NULL AND system = ?\n"
-                    " UNION \n"
-                    "SELECT name, type, value\n"
-                    "  FROM property, str_data\n"
-                    " WHERE str_data.property = property.id"
-                    "   AND configuration IS NULL AND system = ?\n"
-                    " UNION \n"
-                    "SELECT name, type, value\n"
-                    "  FROM property, json_data\n"
-                    " WHERE json_data.property = property.id"
-                    "   AND configuration IS NULL AND system = ? \n"
-                )
-                self.cursor.execute(
-                    sql,
-                    (
-                        configuration_id,
-                        configuration_id,
-                        configuration_id,
-                        configuration_id,
-                        system_id,
-                        system_id,
-                        system_id,
-                        system_id,
-                    ),
-                )
-            else:
-                self.cursor.execute(
-                    sql,
-                    (
-                        configuration_id,
-                        configuration_id,
-                        configuration_id,
-                        configuration_id,
-                    ),
-                )
 
             result = {}
             for row in self.cursor:
                 name, _type, value = row
                 if _type == "float":
                     result[name] = float(value)
                 elif _type == "int":
@@ -425,98 +378,61 @@
                 else:
                     raise ValueError(f"Property '{_property}' does not exist.")
             else:
                 pid = _property
 
             ptype = self.type(pid)
             sql = (
-                f"SELECT value FROM {ptype}_data\n"
+                f"SELECT value FROM {ptype}_data"
                 "  WHERE configuration = ? AND property = ?"
             )
-            if include_system_properties:
-                sql += (
-                    "\n"
-                    "  UNION \n"
-                    f"SELECT value FROM {ptype}_data\n"
-                    "  WHERE configuration IS NULL and system = ? AND property = ?"
-                )
-                self.cursor.execute(sql, (configuration_id, pid, system_id, pid))
-            else:
-                self.cursor.execute(sql, (configuration_id, pid))
+            self.cursor.execute(sql, (configuration_id, pid))
             result = self.cursor.fetchone()
             if result is None:
                 raise ValueError(
                     f"Property {_property} does not exist for configuration "
                     f"{configuration_id}"
                 )
             if ptype == "json":
                 return json.loads(result[0])
             else:
                 return result[0]
 
-    def get_for_system(
-        self, system_id, _property="all", include_configuration_properties=False
-    ):
+    def get_for_system(self, system_id, _property="all"):
         """Get the given property value(s) for the system.
 
         Parameters
         ----------
         system_id : int
             The id of the system.
         _property : int or str of "all"
             The id or name of the property, or "all" for all properties.
-        include_configuration_properties : bool=False
-            Whether to include properties from any configuration in the system.
 
         Returns
         -------
         [int, float, or str]
             The value(s) of the property.
         """
         if _property == "all":
-            if include_configuration_properties:
-                sql = (
-                    "SELECT name, type, value\n"
-                    "  FROM property, float_data\n"
-                    " WHERE float_data.property = property.id AND system = ?\n"
-                    " UNION \n"
-                    "SELECT name, type, value\n"
-                    "  FROM property, int_data\n"
-                    " WHERE int_data.property = property.id AND system = ?\n"
-                    " UNION \n"
-                    "SELECT name, type, value\n"
-                    "  FROM property, str_data\n"
-                    " WHERE str_data.property = property.id AND system = ?\n"
-                    " UNION \n"
-                    "SELECT name, type, value\n"
-                    "  FROM property, json_data\n"
-                    " WHERE json_data.property = property.id AND system = ?\n"
-                )
-            else:
-                sql = (
-                    "SELECT name, type, value\n"
-                    "  FROM property, float_data\n"
-                    " WHERE float_data.property = property.id"
-                    "   AND configuration is NULL AND system = ?\n"
-                    " UNION \n"
-                    "SELECT name, type, value\n"
-                    "  FROM property, int_data\n"
-                    " WHERE int_data.property = property.id"
-                    "   AND configuration is NULL AND system = ?\n"
-                    " UNION \n"
-                    "SELECT name, type, value\n"
-                    "  FROM property, str_data\n"
-                    " WHERE str_data.property = property.id"
-                    "   AND configuration is NULL AND system = ?\n"
-                    " UNION \n"
-                    "SELECT name, type, value\n"
-                    "  FROM property, json_data\n"
-                    " WHERE json_data.property = property.id"
-                    "   AND configuration is NULL AND system = ?\n"
-                )
+            sql = "SELECT name, type, value"
+            sql += "  FROM property, float_data"
+            sql += " WHERE float_data.property = property.id AND system = ?"
+            sql += " UNION "
+            sql += "SELECT name, type, value"
+            sql += "  FROM property, int_data"
+            sql += " WHERE int_data.property = property.id AND system = ?"
+            sql += " UNION "
+            sql += "SELECT name, type, value"
+            sql += "  FROM property, str_data"
+            sql += " WHERE str_data.property = property.id AND system = ?"
+            sql += " UNION "
+            sql += "SELECT name, type, value"
+            sql += "  FROM property, json_data"
+            sql += " WHERE json_data.property = property.id AND system = ?"
+
             self.cursor.execute(sql, (system_id, system_id, system_id, system_id))
 
             result = {}
             for row in self.cursor:
                 name, _type, value = row
                 if _type == "float":
                     result[name] = float(value)
@@ -532,23 +448,15 @@
                     pid = self.id(_property)
                 else:
                     raise ValueError(f"Property '{_property}' does not exist.")
             else:
                 pid = _property
             ptype = self.type(pid)
 
-            if include_configuration_properties:
-                sql = (
-                    f"SELECT value FROM {ptype}_data WHERE system = ? AND property = ?"
-                )
-            else:
-                sql = (
-                    f"SELECT value FROM {ptype}_data"
-                    "  WHERE configuration ISNULL AND system = ? AND property = ?"
-                )
+            sql = f"SELECT value FROM {ptype}_data WHERE system = ? AND property = ?"
             result = []
             for row in self.db.execute(sql, (system_id, pid)):
                 if ptype == "json":
                     result.append(json.loads(row[0]))
                 else:
                     result.append(row[0])
```

### Comparing `molsystem-2023.7.30/molsystem/qcschema.py` & `molsystem-2023.7.9/molsystem/qcschema.py`

 * *Files 12% similar despite different names*

```diff
@@ -20,29 +20,27 @@
             "schema_version": 2,
         }
 
         # Symbols and coordinates (in Bohr)
         result["symbols"] = [*self.atoms.symbols]
         factor = Q_(1.0, "Å").m_as("a_0")
         xyz = []
-        # round() below helps tests work across platforms. 9 digits are enough!
         for row in self.atoms.get_coordinates(fractionals=False):
             for val in row:
-                xyz.append(round(val * factor, 9))
+                xyz.append(val * factor)
         result["geometry"] = xyz
 
         # Charge and multiplicity
         result["molecular_charge"] = self.charge
         result["molecular_multiplicity"] = self.spin_multiplicity
 
         # Bonds, if any
         bonds = []
-        index = {j: i for i, j in zip(range(self.n_atoms), self.atoms.ids)}
         for row in self.bonds.bonds():
-            bonds.append((index[row["i"]], index[row["j"]], row["bondorder"]))
+            bonds.append((row["i"], row["j"], row["bondorder"]))
         if len(bonds) > 0:
             result["connectivity"] = bonds
 
         # Molecules (fragments in QCSchema speak)
         result["fragments"] = self.find_molecules(as_indices=True)
 
         result["name"] = f"{self.system.name} / {self.name}"
```

### Comparing `molsystem-2023.7.30/molsystem/rdkit_.py` & `molsystem-2023.7.9/molsystem/rdkit_.py`

 * *Files identical despite different names*

### Comparing `molsystem-2023.7.30/molsystem/smiles.py` & `molsystem-2023.7.9/molsystem/smiles.py`

 * *Files 24% similar despite different names*

```diff
@@ -8,20 +8,14 @@
     from openbabel import openbabel
 except ModuleNotFoundError:
     print(
         "Please install openbabel using conda:\n"
         "     conda install -c conda-forge openbabel"
     )
     raise
-try:
-    from rdkit import Chem
-    from rdkit.Chem import AllChem
-except ModuleNotFoundError:
-    print("Please install RDKit using conda:\n     conda install -c conda-forge rdkit")
-    raise
 
 logger = logging.getLogger(__name__)
 
 
 class SMILESMixin:
     """A mixin for handling SMILES."""
 
@@ -36,107 +30,81 @@
         return self.to_smarts()
 
     @property
     def smiles(self):
         """Return the SMILES string for this object."""
         return self.to_smiles()
 
-    def to_smiles(self, canonical=False, hydrogens=False, isomeric=True, rdkit=False):
+    def to_smiles(self, canonical=False, hydrogens=False):
         """Create the SMILES string from the system.
 
         Parameters
         ----------
         canonical : bool = False
             Whether to create canonical SMILES
         hydrogens : bool = False
             Whether to keep H's in the SMILES string.
-        isomeric : bool = True
-            Whether to use isomeric SMILES
-        rdkit : bool = False
-            Whether to use RDKit rather than default of OpenBabel
 
         Returns
         -------
         str
             The SMILES string, or (SMILES, name) if the rname is requested
         """
         logger.info("to_smiles")
 
-        if rdkit:
-            mol = self.to_RDKMol()
-            if isomeric:
-                Chem.FindPotentialStereo(mol)
-            if hydrogens:
-                mol2 = mol
-            else:
-                mol2 = AllChem.RemoveHs(mol)
-            if canonical:
-                smiles = Chem.MolToSmiles(mol2, isomericSmiles=isomeric)
-            else:
-                smiles = Chem.MolToSmiles(
-                    mol2, isomericSmiles=isomeric, canonical=False
-                )
+        obConversion = openbabel.OBConversion()
+        if canonical:
+            obConversion.SetOutFormat("can")
         else:
-            obConversion = openbabel.OBConversion()
-            if canonical:
-                obConversion.SetOutFormat("can")
-            else:
-                obConversion.SetOutFormat("smi")
-
-            mol = self.to_OBMol()
-
-            if hydrogens:
-                obConversion.AddOption("h")
-            if not isomeric:
-                obConversion.AddOption("i")
-            smiles = obConversion.WriteString(mol)
+            obConversion.SetOutFormat("smi")
+
+        mol = self.to_OBMol()
+
+        if hydrogens:
+            obConversion.AddOption("h")
+        smiles = obConversion.WriteString(mol)
 
         logger.info(f"smiles = '{smiles}'")
 
         return smiles.strip()
 
-    def from_smiles(self, smiles, name=None, rdkit=False):
+    def from_smiles(self, smiles, name=None):
         """Create the system from a SMILES string.
 
         Parameters
         ----------
         smiles : str
             The SMILES string
         name : str = None
             The name of the molecule
-        rdkit : bool = False
-            Whether to use RDKit rather than default of OpenBabel
 
         Returns
         -------
         None
         """
 
         save = self.name
 
-        if rdkit:
-            mol = Chem.rdmolfiles.MolFromSmiles(smiles)
-            mol = Chem.AddHs(mol)
-            AllChem.EmbedMolecule(mol)
-            self.from_RDKMol(mol)
-        else:
-            obConversion = openbabel.OBConversion()
-            obConversion.SetInAndOutFormats("smi", "mdl")
-            obConversion.AddOption("3")
-            mol = openbabel.OBMol()
-            obConversion.ReadString(mol, smiles)
-
-            # Add hydrogens
-            mol.AddHydrogens()
-
-            # Get coordinates for a 3-D structure
-            builder = openbabel.OBBuilder()
-            builder.Build(mol)
+        obConversion = openbabel.OBConversion()
+        obConversion.SetInAndOutFormats("smi", "mdl")
+        obConversion.AddOption("3")
+        mol = openbabel.OBMol()
+        obConversion.ReadString(mol, smiles)
+
+        # Add hydrogens
+        mol.AddHydrogens()
+
+        # Get coordinates for a 3-D structure
+        builder = openbabel.OBBuilder()
+        builder.Build(mol)
+
+        # molfile = obConversion.WriteString(mol)
+        # self.from_molfile_text(molfile)
 
-            self.from_OBMol(mol)
+        self.from_OBMol(mol)
 
         if name is not None:
             self.name = name
         else:
             self.name = save
 
     def to_smarts(self):
```

### Comparing `molsystem-2023.7.30/molsystem/subset.py` & `molsystem-2023.7.9/molsystem/subset.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,21 +1,20 @@
 # -*- coding: utf-8 -*-
 import logging
 
 from .atoms import _SubsetAtoms
 from .bonds import _SubsetBonds
-from .inchi import InChIMixin
 from .openbabel import OpenBabelMixin
 from .smiles import SMILESMixin
 from .template import _Template
 
 logger = logging.getLogger(__name__)
 
 
-class _Subset(InChIMixin, SMILESMixin, OpenBabelMixin, object):
+class _Subset(SMILESMixin, OpenBabelMixin, object):
     """A class providing the API for a subset.
 
     Parameters
     ----------
     sid : int
         The id of the subset in the subset table.
     logger : logging.Logger = logger
```

### Comparing `molsystem-2023.7.30/molsystem/subsets.py` & `molsystem-2023.7.9/molsystem/subsets.py`

 * *Files identical despite different names*

### Comparing `molsystem-2023.7.30/molsystem/symmetry.py` & `molsystem-2023.7.9/molsystem/symmetry.py`

 * *Files identical despite different names*

### Comparing `molsystem-2023.7.30/molsystem/system.py` & `molsystem-2023.7.9/molsystem/system.py`

 * *Files identical despite different names*

### Comparing `molsystem-2023.7.30/molsystem/system_db.py` & `molsystem-2023.7.9/molsystem/system_db.py`

 * *Files 4% similar despite different names*

```diff
@@ -309,24 +309,14 @@
         # Detach the other database if needed
         if detach:
             self.detach(other)
 
         return result
 
     @property
-    def configurations(self):
-        """The list of configuration objects."""
-        return [_Configuration(_id, self) for _id in self.configuration_ids]
-
-    @property
-    def configuration_ids(self):
-        """The list of configuration ids."""
-        return [row[0] for row in self.db.execute("SELECT id FROM configuration")]
-
-    @property
     def cursor(self):
         """A database cursor."""
         return self._cursor
 
     @property
     def db(self):
         """The database connection."""
@@ -682,58 +672,14 @@
         Returns
         -------
         _Configuration
             The requested configuration.
         """
         return _Configuration(_id=cid, system_db=self)
 
-    def get_configurations(self, pattern="*"):
-        """Return the configurations matching the glob pattern.
-
-        Parameters
-        ----------
-        pattern : list or str = "*"
-            The glob-style pattern for matching the configuration names
-
-        Returns
-        -------
-        [_configuration]
-            The requested configuration ids
-        """
-        return [
-            _Configuration(_id, self) for _id in self.get_configuration_ids(pattern)
-        ]
-
-    def get_configuration_ids(self, pattern="*"):
-        """Return the configuration ids matching the glob pattern.
-
-        Parameters
-        ----------
-        pattern : list or str = "*"
-            The glob-style pattern for matching the configuration names
-
-        Returns
-        -------
-        [int]
-            The requested configuration ids
-        """
-        if pattern == "*":
-            return [row[0] for row in self.db.execute("SELECT id FROM configuration")]
-
-        if isinstance(pattern, list):
-            sql = "\n UNION \n".join(
-                ["SELECT id FROM configuration WHERE name GLOB ?"] * len(pattern)
-            )
-            params = pattern
-        else:
-            sql = "SELECT id FROM configuration WHERE name GLOB ?"
-            params = (pattern,)
-
-        return [row[0] for row in self.db.execute(sql, params)]
-
     def get_system(self, id_or_name):
         """Get the specified system object.
 
         Parameters
         ----------
         id_or_name : int or str
             The id (int) or name (str) of the system
@@ -757,55 +703,14 @@
                 raise ValueError(f"The system '{id_or_name}' does not exist.")
             elif len(systems) > 1:
                 raise ValueError(f"There is more than one system named '{id_or_name}'")
             else:
                 id_or_name = systems[0]
         return _System(self, id_or_name)
 
-    def get_systems(self, pattern="*"):
-        """Return the systems matching the glob pattern.
-
-        Parameters
-        ----------
-        pattern : list or str = "*"
-            The glob-style pattern for matching the system names
-
-        Returns
-        -------
-        [_system]
-            The requested system ids
-        """
-        return [_System(self, _id) for _id in self.get_system_ids(pattern)]
-
-    def get_system_ids(self, pattern="*"):
-        """Return the system ids matching the glob pattern.
-
-        Parameters
-        ----------
-        pattern : list or str = "*"
-            The glob-style pattern for matching the system names
-
-        Returns
-        -------
-        [int]
-            The requested system ids
-        """
-        if pattern == "*":
-            return [row[0] for row in self.db.execute("SELECT id FROM system")]
-
-        if isinstance(pattern, list):
-            sql = "\n UNION \n".join(
-                ["SELECT id FROM system WHERE name GLOB ?"] * len(pattern)
-            )
-            params = pattern
-        else:
-            sql = "SELECT id FROM system WHERE name GLOB ?"
-            params = (pattern,)
-        return [row[0] for row in self.db.execute(sql, params)]
-
     def is_attached(self, other):
         """Return whether another system is attached to this one.
 
         Parameters
         ----------
         other : SystemDB
             The other SystemDB object containing the database
```

### Comparing `molsystem-2023.7.30/molsystem/system_properties.py` & `molsystem-2023.7.9/molsystem/system_properties.py`

 * *Files 4% similar despite different names*

```diff
@@ -54,34 +54,28 @@
         """
         return self.properties.description(_property)
 
     def exists(self, name):
         """A thin wrapper of the _Properties method."""
         return self.properties.exists(name)
 
-    def get(self, _property="all", include_configuration_properties=False):
+    def get(self, _property="all"):
         """Get the given property value for this system.
 
         Parameters
         ----------
         _property : int or str
             The id or name of the property.
 
         Returns
         -------
         int, float, or str
             The value of the property.
-        include_configuration_properties : bool=False
-            Whether to include properties from any configuration in the system.
         """
-        return self.properties.get_for_system(
-            self._sid,
-            _property,
-            include_configuration_properties=include_configuration_properties,
-        )
+        return self.properties.get_for_system(self._sid, _property)
 
     def id(self, name):
         """The id for a property
 
         Parameters
         ----------
         name : str
```

### Comparing `molsystem-2023.7.30/molsystem/table.py` & `molsystem-2023.7.9/molsystem/table.py`

 * *Files identical despite different names*

### Comparing `molsystem-2023.7.30/molsystem/template.py` & `molsystem-2023.7.9/molsystem/template.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,18 +1,17 @@
 # -*- coding: utf-8 -*-
 import logging
 
-from .inchi import InChIMixin
 from .openbabel import OpenBabelMixin
 from .smiles import SMILESMixin
 
 logger = logging.getLogger(__name__)
 
 
-class _Template(InChIMixin, SMILESMixin, OpenBabelMixin, object):
+class _Template(SMILESMixin, OpenBabelMixin, object):
     """A class providing the API for templates.
 
     There are two types of templates:
 
     simple
         Which have a category and name, which together are unique.
     full
```

### Comparing `molsystem-2023.7.30/molsystem/templates.py` & `molsystem-2023.7.9/molsystem/templates.py`

 * *Files identical despite different names*

### Comparing `molsystem-2023.7.30/molsystem/topology.py` & `molsystem-2023.7.9/molsystem/topology.py`

 * *Files identical despite different names*

### Comparing `molsystem-2023.7.30/molsystem.egg-info/PKG-INFO` & `molsystem-2023.7.9/molsystem.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: molsystem
-Version: 2023.7.30
+Version: 2023.7.9
 Summary: molsystem
 Home-page: https://github.com/molssi-seamm/molsystem
 Author: Paul Saxe
 Author-email: psaxe@molssi.org
 License: GNU Lesser General Public License v3 or later (LGPLv3+)
 Keywords: molsystem,SEAMM
 Platform: Linux
@@ -110,31 +110,16 @@
 .. _`National Science Foundation`: https://www.nsf.gov
 
 
 =======
 History
 =======
 
-2023.7.30 -- Improved handling of properties
-    * Added ability to get lists of systems or configurations filtered by name
-    * Improved handling of properties on just a system, not configuration
-    * Added ability to filter properties retrieved
-    * Improved handling of properties when creating OpenBabel OB_MOL object
-      
-2023.7.26 -- Bugfix: error in QCSchema bonds; enhancement: RDKit
-    * Fixed bug in the bond indices in QCSchema
-    * Added ability to use RDKit for SMILES and InChI
-
-2023.7.18.1 -- Added support for creating structures from InChIKeys
-    * Uses PubChem to translate the InChiKey to InChI.
-       
-2023.7.18 -- Added support for InChI and InChIKeys
-
 2023.7.9 -- Added JSON properties
-    * Added properties stored as JSON, which allows, vectors, tensors, etc.
+    * Added properties sotred as JSON, which allows, vectors, tensors, etc.
       
 2023.4.6 -- Enhancements for CIF files
     * Handle uncertainties in CIF files expressed as '(x)' at end of value.
 
 2023.3.30 -- Enhancements to QCSchema support
     * Improved naming of molecule in QCSchema
     * Added creation of configurations from QCSchema objects.
```

### Comparing `molsystem-2023.7.30/molsystem.egg-info/SOURCES.txt` & `molsystem-2023.7.9/molsystem.egg-info/SOURCES.txt`

 * *Files 5% similar despite different names*

```diff
@@ -34,15 +34,14 @@
 molsystem/cif.py
 molsystem/cms_schema.py
 molsystem/column.py
 molsystem/configuration.py
 molsystem/configuration_properties.py
 molsystem/elements.py
 molsystem/frozencolumn.py
-molsystem/inchi.py
 molsystem/molfile.py
 molsystem/openbabel.py
 molsystem/pdb.py
 molsystem/properties.py
 molsystem/qcschema.py
 molsystem/rdkit_.py
 molsystem/smiles.py
@@ -67,21 +66,19 @@
 tests/test_angiotensin.py
 tests/test_atoms.py
 tests/test_bonds.py
 tests/test_cell.py
 tests/test_cif.py
 tests/test_configuration_properties.py
 tests/test_configurations.py
-tests/test_inchi.py
 tests/test_molfile.py
 tests/test_openbabel.py
 tests/test_pdb.py
 tests/test_properties.py
 tests/test_property_timings.py
-tests/test_qcschema.py
 tests/test_rdkit.py
 tests/test_smiles.py
 tests/test_subsets.py
 tests/test_system.py
 tests/test_system_db.py
 tests/test_table.py
 tests/test_templates.py
```

### Comparing `molsystem-2023.7.30/setup.py` & `molsystem-2023.7.9/setup.py`

 * *Files identical despite different names*

### Comparing `molsystem-2023.7.30/tests/conftest.py` & `molsystem-2023.7.9/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `molsystem-2023.7.30/tests/data/1n9v.cif` & `molsystem-2023.7.9/tests/data/1n9v.cif`

 * *Files identical despite different names*

### Comparing `molsystem-2023.7.30/tests/data/aa-variants-v1.cif` & `molsystem-2023.7.9/tests/data/aa-variants-v1.cif`

 * *Files identical despite different names*

### Comparing `molsystem-2023.7.30/tests/data/acy.mmcif` & `molsystem-2023.7.9/tests/data/acy.mmcif`

 * *Files identical despite different names*

### Comparing `molsystem-2023.7.30/tests/data/aminoacids.mmcif` & `molsystem-2023.7.9/tests/data/aminoacids.mmcif`

 * *Files identical despite different names*

### Comparing `molsystem-2023.7.30/tests/data/hoh.mmcif` & `molsystem-2023.7.9/tests/data/hoh.mmcif`

 * *Files identical despite different names*

### Comparing `molsystem-2023.7.30/tests/test_angiotensin.py` & `molsystem-2023.7.9/tests/test_angiotensin.py`

 * *Files identical despite different names*

### Comparing `molsystem-2023.7.30/tests/test_atoms.py` & `molsystem-2023.7.9/tests/test_atoms.py`

 * *Files identical despite different names*

### Comparing `molsystem-2023.7.30/tests/test_bonds.py` & `molsystem-2023.7.9/tests/test_bonds.py`

 * *Files identical despite different names*

### Comparing `molsystem-2023.7.30/tests/test_cell.py` & `molsystem-2023.7.9/tests/test_cell.py`

 * *Files identical despite different names*

### Comparing `molsystem-2023.7.30/tests/test_cif.py` & `molsystem-2023.7.9/tests/test_cif.py`

 * *Files identical despite different names*

### Comparing `molsystem-2023.7.30/tests/test_configuration_properties.py` & `molsystem-2023.7.9/tests/test_configuration_properties.py`

 * *Files identical despite different names*

### Comparing `molsystem-2023.7.30/tests/test_configurations.py` & `molsystem-2023.7.9/tests/test_configurations.py`

 * *Files identical despite different names*

### Comparing `molsystem-2023.7.30/tests/test_inchi.py` & `molsystem-2023.7.9/tests/test_smiles.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,75 +1,72 @@
 #!/usr/bin/env python
 # -*- coding: utf-8 -*-
 
 import pytest  # noqa: F401
 
-"""Tests for handling InChI."""
+"""Tests for handling SMILES."""
 
 
-def test_to_inchi(AceticAcid):
-    """Create a InChI string from a system"""
-    correct = "InChI=1S/C2H4O2/c1-2(3)4/h1H3,(H,3,4)"
-    inchi = AceticAcid.to_inchi()
+def test_to_smiles(AceticAcid):
+    """Create a SMILES string from a system"""
+    correct = "CC(=O)O"
+    smiles = AceticAcid.to_smiles()
 
-    if inchi != correct:
-        print(inchi)
-    assert inchi == correct
+    if smiles != correct:
+        print(smiles)
+    assert smiles == correct
 
 
-def test_to_inchikey(AceticAcid):
-    """Create a InChIKey string from a system"""
-    correct = "QTBSBXVTEAMEQO-UHFFFAOYSA-N"
-    inchi = AceticAcid.to_inchi(key=True)
+def test_to_smiles_with_name(AceticAcid):
+    """Create a SMILES string from a system"""
+    correct = "CC(=O)O"
+    smiles = AceticAcid.smiles
 
-    if inchi != correct:
-        print(inchi)
-    assert inchi == correct
+    if smiles != correct:
+        print(smiles)
+    assert smiles == correct
 
 
-def test_to_inchi_with_name(AceticAcid):
-    """Create a InChI string from a system, adding the name"""
-    correct = "InChI=1S/C2H4O2/c1-2(3)4/h1H3,(H,3,4)"
-    inchi = AceticAcid.inchi
+def test_to_canonical_smiles(AceticAcid):
+    """Create a SMILES string from a system"""
+    correct = "CC(=O)O"
+    smiles = AceticAcid.to_smiles(canonical=True)
 
-    if inchi != correct:
-        print(inchi)
-    assert inchi == correct
+    if smiles != correct:
+        print(smiles)
+    assert smiles == correct
 
 
 def test_several_molecules(CH3COOH_3H2O):
     """System with acetic acid and 3 waters"""
     system = CH3COOH_3H2O
-    correct = "InChI=1S/C2H4O2.3H2O/c1-2(3)4;;;/h1H3,(H,3,4);3*1H2"
+    correct = "CC(=O)O.O.O.O"
 
-    inchi = system.to_inchi()
+    smiles = system.to_smiles()
 
-    if inchi != correct:
-        print(inchi)
-    assert inchi == correct
+    if smiles != correct:
+        print(smiles)
+    assert smiles == correct
 
 
-def test_from_inchi(configuration):
-    """Create a configuration from InChI"""
-    correct = "CC(=O)O"
-    configuration.from_inchi(
-        "InChI=1S/C2H4O2/c1-2(3)4/h1H3,(H,3,4)", name="acetic acid"
-    )
-    result = configuration.to_smiles(canonical=True)
+def test_several_molecules_canonical(CH3COOH_3H2O):
+    """System with acetic acid and 3 waters"""
+    system = CH3COOH_3H2O
+    correct = "CC(=O)O.O.O.O"
 
-    if result != correct:
-        print(result)
+    smiles = system.to_smiles(canonical=True)
 
-    assert result == correct
+    if smiles != correct:
+        print(smiles)
+    assert smiles == correct
 
 
-def test_from_inchikey(configuration):
-    """Create a configuration from an InChIKey"""
+def test_from_smiles(configuration):
+    """Create a configuration from SMILES"""
     correct = "CC(=O)O"
-
-    configuration.from_inchikey("QTBSBXVTEAMEQO-UHFFFAOYSA-N")
+    configuration.from_smiles("OC(=O)C", name="acetic acid")
     result = configuration.to_smiles(canonical=True)
 
     if result != correct:
         print(result)
 
     assert result == correct
```

### Comparing `molsystem-2023.7.30/tests/test_molfile.py` & `molsystem-2023.7.9/tests/test_molfile.py`

 * *Files identical despite different names*

### Comparing `molsystem-2023.7.30/tests/test_openbabel.py` & `molsystem-2023.7.9/tests/test_openbabel.py`

 * *Files identical despite different names*

### Comparing `molsystem-2023.7.30/tests/test_pdb.py` & `molsystem-2023.7.9/tests/test_pdb.py`

 * *Files identical despite different names*

### Comparing `molsystem-2023.7.30/tests/test_properties.py` & `molsystem-2023.7.9/tests/test_properties.py`

 * *Files identical despite different names*

### Comparing `molsystem-2023.7.30/tests/test_property_timings.py` & `molsystem-2023.7.9/tests/test_property_timings.py`

 * *Files identical despite different names*

### Comparing `molsystem-2023.7.30/tests/test_rdkit.py` & `molsystem-2023.7.9/tests/test_rdkit.py`

 * *Files identical despite different names*

### Comparing `molsystem-2023.7.30/tests/test_subsets.py` & `molsystem-2023.7.9/tests/test_subsets.py`

 * *Files identical despite different names*

### Comparing `molsystem-2023.7.30/tests/test_system.py` & `molsystem-2023.7.9/tests/test_system.py`

 * *Files identical despite different names*

### Comparing `molsystem-2023.7.30/tests/test_system_db.py` & `molsystem-2023.7.9/tests/test_system_db.py`

 * *Files identical despite different names*

### Comparing `molsystem-2023.7.30/tests/test_table.py` & `molsystem-2023.7.9/tests/test_table.py`

 * *Files identical despite different names*

### Comparing `molsystem-2023.7.30/tests/test_templates.py` & `molsystem-2023.7.9/tests/test_templates.py`

 * *Files identical despite different names*

### Comparing `molsystem-2023.7.30/tests/test_timings.py` & `molsystem-2023.7.9/tests/test_timings.py`

 * *Files identical despite different names*

### Comparing `molsystem-2023.7.30/tests/test_topology.py` & `molsystem-2023.7.9/tests/test_topology.py`

 * *Files identical despite different names*

### Comparing `molsystem-2023.7.30/versioneer.py` & `molsystem-2023.7.9/versioneer.py`

 * *Files identical despite different names*

