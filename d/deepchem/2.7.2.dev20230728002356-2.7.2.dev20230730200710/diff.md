# Comparing `tmp/deepchem-2.7.2.dev20230728002356.tar.gz` & `tmp/deepchem-2.7.2.dev20230730200710.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "deepchem-2.7.2.dev20230728002356.tar", last modified: Fri Jul 28 00:23:57 2023, max compression
+gzip compressed data, was "deepchem-2.7.2.dev20230730200710.tar", last modified: Sun Jul 30 20:07:10 2023, max compression
```

## Comparing `deepchem-2.7.2.dev20230728002356.tar` & `deepchem-2.7.2.dev20230730200710.tar`

### file list

```diff
@@ -1,298 +1,298 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 00:23:57.175554 deepchem-2.7.2.dev20230728002356/
--rwxr-xr-x   0 runner    (1001) docker     (123)     1047 2023-07-28 00:23:40.000000 deepchem-2.7.2.dev20230728002356/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-07-28 00:23:57.175554 deepchem-2.7.2.dev20230728002356/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     7124 2023-07-28 00:23:40.000000 deepchem-2.7.2.dev20230728002356/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 00:23:57.151554 deepchem-2.7.2.dev20230728002356/deepchem/
--rw-r--r--   0 runner    (1001) docker     (123)      373 2023-07-28 00:23:40.000000 deepchem-2.7.2.dev20230728002356/deepchem/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 00:23:57.151554 deepchem-2.7.2.dev20230728002356/deepchem/data/
--rw-r--r--   0 runner    (1001) docker     (123)      939 2023-07-28 00:23:40.000000 deepchem-2.7.2.dev20230728002356/deepchem/data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    67994 2023-07-28 00:23:40.000000 deepchem-2.7.2.dev20230728002356/deepchem/data/data_loader.py
--rw-r--r--   0 runner    (1001) docker     (123)   118009 2023-07-28 00:23:40.000000 deepchem-2.7.2.dev20230728002356/deepchem/data/datasets.py
--rw-r--r--   0 runner    (1001) docker     (123)     7256 2023-07-28 00:23:40.000000 deepchem-2.7.2.dev20230728002356/deepchem/data/pytorch_datasets.py
--rw-r--r--   0 runner    (1001) docker     (123)    12606 2023-07-28 00:23:40.000000 deepchem-2.7.2.dev20230728002356/deepchem/data/supports.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 00:23:57.151554 deepchem-2.7.2.dev20230728002356/deepchem/dock/
--rw-r--r--   0 runner    (1001) docker     (123)      297 2023-07-28 00:23:40.000000 deepchem-2.7.2.dev20230728002356/deepchem/dock/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4910 2023-07-28 00:23:40.000000 deepchem-2.7.2.dev20230728002356/deepchem/dock/binding_pocket.py
--rw-r--r--   0 runner    (1001) docker     (123)     6105 2023-07-28 00:23:40.000000 deepchem-2.7.2.dev20230728002356/deepchem/dock/docking.py
--rw-r--r--   0 runner    (1001) docker     (123)    19576 2023-07-28 00:23:40.000000 deepchem-2.7.2.dev20230728002356/deepchem/dock/pose_generation.py
--rw-r--r--   0 runner    (1001) docker     (123)     6917 2023-07-28 00:23:40.000000 deepchem-2.7.2.dev20230728002356/deepchem/dock/pose_scoring.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 00:23:57.155554 deepchem-2.7.2.dev20230728002356/deepchem/feat/
--rw-r--r--   0 runner    (1001) docker     (123)     4521 2023-07-28 00:23:40.000000 deepchem-2.7.2.dev20230728002356/deepchem/feat/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7335 2023-07-28 00:23:40.000000 deepchem-2.7.2.dev20230728002356/deepchem/feat/atomic_conformation.py
--rw-r--r--   0 runner    (1001) docker     (123)    19458 2023-07-28 00:23:40.000000 deepchem-2.7.2.dev20230728002356/deepchem/feat/base_classes.py
--rw-r--r--   0 runner    (1001) docker     (123)     1904 2023-07-28 00:23:40.000000 deepchem-2.7.2.dev20230728002356/deepchem/feat/bert_tokenizer.py
--rw-r--r--   0 runner    (1001) docker     (123)     4368 2023-07-28 00:23:40.000000 deepchem-2.7.2.dev20230728002356/deepchem/feat/binding_pocket_features.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 00:23:57.155554 deepchem-2.7.2.dev20230728002356/deepchem/feat/complex_featurizers/
--rw-r--r--   0 runner    (1001) docker     (123)     1400 2023-07-28 00:23:40.000000 deepchem-2.7.2.dev20230728002356/deepchem/feat/complex_featurizers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12898 2023-07-28 00:23:40.000000 deepchem-2.7.2.dev20230728002356/deepchem/feat/complex_featurizers/complex_atomic_coordinates.py
--rw-r--r--   0 runner    (1001) docker     (123)    10769 2023-07-28 00:23:40.000000 deepchem-2.7.2.dev20230728002356/deepchem/feat/complex_featurizers/contact_fingerprints.py
--rw-r--r--   0 runner    (1001) docker     (123)    27676 2023-07-28 00:23:40.000000 deepchem-2.7.2.dev20230728002356/deepchem/feat/complex_featurizers/grid_featurizers.py
--rw-r--r--   0 runner    (1001) docker     (123)    20248 2023-07-28 00:23:40.000000 deepchem-2.7.2.dev20230728002356/deepchem/feat/complex_featurizers/rdkit_grid_featurizer.py
--rw-r--r--   0 runner    (1001) docker     (123)    11465 2023-07-28 00:23:40.000000 deepchem-2.7.2.dev20230728002356/deepchem/feat/complex_featurizers/splif_fingerprints.py
--rw-r--r--   0 runner    (1001) docker     (123)    11743 2023-07-28 00:23:40.000000 deepchem-2.7.2.dev20230728002356/deepchem/feat/dft_data.py
--rw-r--r--   0 runner    (1001) docker     (123)    22111 2023-07-28 00:23:40.000000 deepchem-2.7.2.dev20230728002356/deepchem/feat/graph_data.py
--rw-r--r--   0 runner    (1001) docker     (123)    38890 2023-07-28 00:23:40.000000 deepchem-2.7.2.dev20230728002356/deepchem/feat/graph_features.py
--rw-r--r--   0 runner    (1001) docker     (123)     1396 2023-07-28 00:23:40.000000 deepchem-2.7.2.dev20230728002356/deepchem/feat/huggingface_featurizer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 00:23:57.155554 deepchem-2.7.2.dev20230728002356/deepchem/feat/material_featurizers/
--rw-r--r--   0 runner    (1001) docker     (123)      489 2023-07-28 00:23:40.000000 deepchem-2.7.2.dev20230728002356/deepchem/feat/material_featurizers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7539 2023-07-28 00:23:40.000000 deepchem-2.7.2.dev20230728002356/deepchem/feat/material_featurizers/cgcnn_featurizer.py
--rw-r--r--   0 runner    (1001) docker     (123)     3508 2023-07-28 00:23:40.000000 deepchem-2.7.2.dev20230728002356/deepchem/feat/material_featurizers/element_property_fingerprint.py
--rw-r--r--   0 runner    (1001) docker     (123)     3232 2023-07-28 00:23:40.000000 deepchem-2.7.2.dev20230728002356/deepchem/feat/material_featurizers/elemnet_featurizer.py
--rw-r--r--   0 runner    (1001) docker     (123)    28058 2023-07-28 00:23:40.000000 deepchem-2.7.2.dev20230728002356/deepchem/feat/material_featurizers/lcnn_featurizer.py
--rw-r--r--   0 runner    (1001) docker     (123)     3823 2023-07-28 00:23:40.000000 deepchem-2.7.2.dev20230728002356/deepchem/feat/material_featurizers/sine_coulomb_matrix.py
--rw-r--r--   0 runner    (1001) docker     (123)    14808 2023-07-28 00:23:40.000000 deepchem-2.7.2.dev20230728002356/deepchem/feat/mol_graphs.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 00:23:57.155554 deepchem-2.7.2.dev20230728002356/deepchem/feat/molecule_featurizers/
--rw-r--r--   0 runner    (1001) docker     (123)     2156 2023-07-28 00:23:40.000000 deepchem-2.7.2.dev20230728002356/deepchem/feat/molecule_featurizers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2884 2023-07-28 00:23:40.000000 deepchem-2.7.2.dev20230728002356/deepchem/feat/molecule_featurizers/atomic_coordinates.py
--rw-r--r--   0 runner    (1001) docker     (123)     2376 2023-07-28 00:23:40.000000 deepchem-2.7.2.dev20230728002356/deepchem/feat/molecule_featurizers/bp_symmetry_function_input.py
--rw-r--r--   0 runner    (1001) docker     (123)     6488 2023-07-28 00:23:40.000000 deepchem-2.7.2.dev20230728002356/deepchem/feat/molecule_featurizers/circular_fingerprint.py
--rw-r--r--   0 runner    (1001) docker     (123)     9242 2023-07-28 00:23:40.000000 deepchem-2.7.2.dev20230728002356/deepchem/feat/molecule_featurizers/conformer_featurizer.py
--rw-r--r--   0 runner    (1001) docker     (123)    10925 2023-07-28 00:23:40.000000 deepchem-2.7.2.dev20230728002356/deepchem/feat/molecule_featurizers/coulomb_matrices.py
--rw-r--r--   0 runner    (1001) docker     (123)    19123 2023-07-28 00:23:40.000000 deepchem-2.7.2.dev20230728002356/deepchem/feat/molecule_featurizers/dmpnn_featurizer.py
--rw-r--r--   0 runner    (1001) docker     (123)     7507 2023-07-28 00:23:40.000000 deepchem-2.7.2.dev20230728002356/deepchem/feat/molecule_featurizers/grover_featurizer.py
--rw-r--r--   0 runner    (1001) docker     (123)     2046 2023-07-28 00:23:40.000000 deepchem-2.7.2.dev20230728002356/deepchem/feat/molecule_featurizers/maccs_keys_fingerprint.py
--rw-r--r--   0 runner    (1001) docker     (123)     8401 2023-07-28 00:23:40.000000 deepchem-2.7.2.dev20230728002356/deepchem/feat/molecule_featurizers/mat_featurizer.py
--rw-r--r--   0 runner    (1001) docker     (123)     7587 2023-07-28 00:23:40.000000 deepchem-2.7.2.dev20230728002356/deepchem/feat/molecule_featurizers/mol2vec_fingerprint.py
--rw-r--r--   0 runner    (1001) docker     (123)    20381 2023-07-28 00:23:40.000000 deepchem-2.7.2.dev20230728002356/deepchem/feat/molecule_featurizers/mol_graph_conv_featurizer.py
--rw-r--r--   0 runner    (1001) docker     (123)     9346 2023-07-28 00:23:40.000000 deepchem-2.7.2.dev20230728002356/deepchem/feat/molecule_featurizers/molgan_featurizer.py
--rw-r--r--   0 runner    (1001) docker     (123)     2835 2023-07-28 00:23:40.000000 deepchem-2.7.2.dev20230728002356/deepchem/feat/molecule_featurizers/mordred_descriptors.py
--rw-r--r--   0 runner    (1001) docker     (123)     5130 2023-07-28 00:23:40.000000 deepchem-2.7.2.dev20230728002356/deepchem/feat/molecule_featurizers/mxmnet_featurizer.py
--rw-r--r--   0 runner    (1001) docker     (123)     6359 2023-07-28 00:23:40.000000 deepchem-2.7.2.dev20230728002356/deepchem/feat/molecule_featurizers/one_hot_featurizer.py
--rw-r--r--   0 runner    (1001) docker     (123)     2258 2023-07-28 00:23:40.000000 deepchem-2.7.2.dev20230728002356/deepchem/feat/molecule_featurizers/pubchem_fingerprint.py
--rw-r--r--   0 runner    (1001) docker     (123)     1687 2023-07-28 00:23:40.000000 deepchem-2.7.2.dev20230728002356/deepchem/feat/molecule_featurizers/raw_featurizer.py
--rw-r--r--   0 runner    (1001) docker     (123)     9881 2023-07-28 00:23:40.000000 deepchem-2.7.2.dev20230728002356/deepchem/feat/molecule_featurizers/rdkit_descriptors.py
--rw-r--r--   0 runner    (1001) docker     (123)     7280 2023-07-28 00:23:40.000000 deepchem-2.7.2.dev20230728002356/deepchem/feat/molecule_featurizers/smiles_to_image.py
--rw-r--r--   0 runner    (1001) docker     (123)     5433 2023-07-28 00:23:40.000000 deepchem-2.7.2.dev20230728002356/deepchem/feat/molecule_featurizers/smiles_to_seq.py
--rw-r--r--   0 runner    (1001) docker     (123)     4313 2023-07-28 00:23:40.000000 deepchem-2.7.2.dev20230728002356/deepchem/feat/molecule_featurizers/snap_featurizer.py
--rw-r--r--   0 runner    (1001) docker     (123)     3448 2023-07-28 00:23:40.000000 deepchem-2.7.2.dev20230728002356/deepchem/feat/molecule_featurizers/sparse_matrix_one_hot_featurizer.py
--rw-r--r--   0 runner    (1001) docker     (123)     3909 2023-07-28 00:23:40.000000 deepchem-2.7.2.dev20230728002356/deepchem/feat/reaction_featurizer.py
--rw-r--r--   0 runner    (1001) docker     (123)     2326 2023-07-28 00:23:40.000000 deepchem-2.7.2.dev20230728002356/deepchem/feat/roberta_tokenizer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 00:23:57.159554 deepchem-2.7.2.dev20230728002356/deepchem/feat/sequence_featurizers/
--rw-r--r--   0 runner    (1001) docker     (123)      112 2023-07-28 00:23:40.000000 deepchem-2.7.2.dev20230728002356/deepchem/feat/sequence_featurizers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3383 2023-07-28 00:23:40.000000 deepchem-2.7.2.dev20230728002356/deepchem/feat/sequence_featurizers/position_frequency_matrix_featurizer.py
--rw-r--r--   0 runner    (1001) docker     (123)    11383 2023-07-28 00:23:40.000000 deepchem-2.7.2.dev20230728002356/deepchem/feat/smiles_tokenizer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 00:23:57.159554 deepchem-2.7.2.dev20230728002356/deepchem/feat/vocabulary_builders/
--rw-r--r--   0 runner    (1001) docker     (123)      278 2023-07-28 00:23:40.000000 deepchem-2.7.2.dev20230728002356/deepchem/feat/vocabulary_builders/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    18726 2023-07-28 00:23:40.000000 deepchem-2.7.2.dev20230728002356/deepchem/feat/vocabulary_builders/grover_vocab.py
--rw-r--r--   0 runner    (1001) docker     (123)     2315 2023-07-28 00:23:40.000000 deepchem-2.7.2.dev20230728002356/deepchem/feat/vocabulary_builders/hf_vocab.py
--rw-r--r--   0 runner    (1001) docker     (123)     1116 2023-07-28 00:23:40.000000 deepchem-2.7.2.dev20230728002356/deepchem/feat/vocabulary_builders/vocabulary_builder.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 00:23:57.159554 deepchem-2.7.2.dev20230728002356/deepchem/hyper/
--rw-r--r--   0 runner    (1001) docker     (123)      260 2023-07-28 00:23:40.000000 deepchem-2.7.2.dev20230728002356/deepchem/hyper/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5702 2023-07-28 00:23:40.000000 deepchem-2.7.2.dev20230728002356/deepchem/hyper/base_classes.py
--rw-r--r--   0 runner    (1001) docker     (123)    17151 2023-07-28 00:23:40.000000 deepchem-2.7.2.dev20230728002356/deepchem/hyper/gaussian_process.py
--rw-r--r--   0 runner    (1001) docker     (123)    10208 2023-07-28 00:23:40.000000 deepchem-2.7.2.dev20230728002356/deepchem/hyper/grid_search.py
--rw-r--r--   0 runner    (1001) docker     (123)    12427 2023-07-28 00:23:40.000000 deepchem-2.7.2.dev20230728002356/deepchem/hyper/random_search.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 00:23:57.159554 deepchem-2.7.2.dev20230728002356/deepchem/metalearning/
--rw-r--r--   0 runner    (1001) docker     (123)      118 2023-07-28 00:23:40.000000 deepchem-2.7.2.dev20230728002356/deepchem/metalearning/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10539 2023-07-28 00:23:40.000000 deepchem-2.7.2.dev20230728002356/deepchem/metalearning/maml.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 00:23:57.159554 deepchem-2.7.2.dev20230728002356/deepchem/metrics/
--rw-r--r--   0 runner    (1001) docker     (123)     2015 2023-07-28 00:23:40.000000 deepchem-2.7.2.dev20230728002356/deepchem/metrics/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7715 2023-07-28 00:23:40.000000 deepchem-2.7.2.dev20230728002356/deepchem/metrics/genomic_metrics.py
--rw-r--r--   0 runner    (1001) docker     (123)    31620 2023-07-28 00:23:40.000000 deepchem-2.7.2.dev20230728002356/deepchem/metrics/metric.py
--rw-r--r--   0 runner    (1001) docker     (123)     6533 2023-07-28 00:23:40.000000 deepchem-2.7.2.dev20230728002356/deepchem/metrics/score_function.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 00:23:57.159554 deepchem-2.7.2.dev20230728002356/deepchem/models/
--rw-r--r--   0 runner    (1001) docker     (123)     4780 2023-07-28 00:23:40.000000 deepchem-2.7.2.dev20230728002356/deepchem/models/IRV.py
--rw-r--r--   0 runner    (1001) docker     (123)     4420 2023-07-28 00:23:40.000000 deepchem-2.7.2.dev20230728002356/deepchem/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13833 2023-07-28 00:23:40.000000 deepchem-2.7.2.dev20230728002356/deepchem/models/atomic_conv.py
--rw-r--r--   0 runner    (1001) docker     (123)     4414 2023-07-28 00:23:40.000000 deepchem-2.7.2.dev20230728002356/deepchem/models/callbacks.py
--rw-r--r--   0 runner    (1001) docker     (123)    17354 2023-07-28 00:23:40.000000 deepchem-2.7.2.dev20230728002356/deepchem/models/chemnet_layers.py
--rw-r--r--   0 runner    (1001) docker     (123)    15504 2023-07-28 00:23:40.000000 deepchem-2.7.2.dev20230728002356/deepchem/models/chemnet_models.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 00:23:57.163554 deepchem-2.7.2.dev20230728002356/deepchem/models/dft/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 00:23:40.000000 deepchem-2.7.2.dev20230728002356/deepchem/models/dft/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9553 2023-07-28 00:23:40.000000 deepchem-2.7.2.dev20230728002356/deepchem/models/dft/dftxc.py
--rw-r--r--   0 runner    (1001) docker     (123)    14020 2023-07-28 00:23:40.000000 deepchem-2.7.2.dev20230728002356/deepchem/models/dft/nnxc.py
--rw-r--r--   0 runner    (1001) docker     (123)     4664 2023-07-28 00:23:40.000000 deepchem-2.7.2.dev20230728002356/deepchem/models/dft/scf.py
--rw-r--r--   0 runner    (1001) docker     (123)    23457 2023-07-28 00:23:40.000000 deepchem-2.7.2.dev20230728002356/deepchem/models/fcnet.py
--rw-r--r--   0 runner    (1001) docker     (123)    24548 2023-07-28 00:23:40.000000 deepchem-2.7.2.dev20230728002356/deepchem/models/gan.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 00:23:57.163554 deepchem-2.7.2.dev20230728002356/deepchem/models/gbdt_models/
--rw-r--r--   0 runner    (1001) docker     (123)       75 2023-07-28 00:23:40.000000 deepchem-2.7.2.dev20230728002356/deepchem/models/gbdt_models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5921 2023-07-28 00:23:40.000000 deepchem-2.7.2.dev20230728002356/deepchem/models/gbdt_models/gbdt_model.py
--rw-r--r--   0 runner    (1001) docker     (123)    57408 2023-07-28 00:23:40.000000 deepchem-2.7.2.dev20230728002356/deepchem/models/graph_models.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 00:23:57.163554 deepchem-2.7.2.dev20230728002356/deepchem/models/jax_models/
--rw-r--r--   0 runner    (1001) docker     (123)      133 2023-07-28 00:23:40.000000 deepchem-2.7.2.dev20230728002356/deepchem/models/jax_models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    28179 2023-07-28 00:23:40.000000 deepchem-2.7.2.dev20230728002356/deepchem/models/jax_models/jax_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     3408 2023-07-28 00:23:40.000000 deepchem-2.7.2.dev20230728002356/deepchem/models/jax_models/layers.py
--rw-r--r--   0 runner    (1001) docker     (123)    17070 2023-07-28 00:23:40.000000 deepchem-2.7.2.dev20230728002356/deepchem/models/jax_models/pinns_model.py
--rw-r--r--   0 runner    (1001) docker     (123)    56522 2023-07-28 00:23:40.000000 deepchem-2.7.2.dev20230728002356/deepchem/models/keras_model.py
--rw-r--r--   0 runner    (1001) docker     (123)   144759 2023-07-28 00:23:40.000000 deepchem-2.7.2.dev20230728002356/deepchem/models/layers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 00:23:57.163554 deepchem-2.7.2.dev20230728002356/deepchem/models/lightning/
--rw-r--r--   0 runner    (1001) docker     (123)      181 2023-07-28 00:23:40.000000 deepchem-2.7.2.dev20230728002356/deepchem/models/lightning/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1742 2023-07-28 00:23:40.000000 deepchem-2.7.2.dev20230728002356/deepchem/models/lightning/dc_lightning_dataset_module.py
--rw-r--r--   0 runner    (1001) docker     (123)     2447 2023-07-28 00:23:40.000000 deepchem-2.7.2.dev20230728002356/deepchem/models/lightning/dc_lightning_module.py
--rw-r--r--   0 runner    (1001) docker     (123)    61903 2023-07-28 00:23:40.000000 deepchem-2.7.2.dev20230728002356/deepchem/models/losses.py
--rw-r--r--   0 runner    (1001) docker     (123)     8256 2023-07-28 00:23:40.000000 deepchem-2.7.2.dev20230728002356/deepchem/models/models.py
--rw-r--r--   0 runner    (1001) docker     (123)    14135 2023-07-28 00:23:40.000000 deepchem-2.7.2.dev20230728002356/deepchem/models/molgan.py
--rw-r--r--   0 runner    (1001) docker     (123)     5437 2023-07-28 00:23:40.000000 deepchem-2.7.2.dev20230728002356/deepchem/models/multitask.py
--rw-r--r--   0 runner    (1001) docker     (123)    10975 2023-07-28 00:23:40.000000 deepchem-2.7.2.dev20230728002356/deepchem/models/normalizing_flows.py
--rw-r--r--   0 runner    (1001) docker     (123)    26871 2023-07-28 00:23:40.000000 deepchem-2.7.2.dev20230728002356/deepchem/models/optimizers.py
--rw-r--r--   0 runner    (1001) docker     (123)    13095 2023-07-28 00:23:40.000000 deepchem-2.7.2.dev20230728002356/deepchem/models/progressive_multitask.py
--rw-r--r--   0 runner    (1001) docker     (123)    17830 2023-07-28 00:23:40.000000 deepchem-2.7.2.dev20230728002356/deepchem/models/robust_multitask.py
--rw-r--r--   0 runner    (1001) docker     (123)     4546 2023-07-28 00:23:40.000000 deepchem-2.7.2.dev20230728002356/deepchem/models/scscore.py
--rw-r--r--   0 runner    (1001) docker     (123)    25969 2023-07-28 00:23:40.000000 deepchem-2.7.2.dev20230728002356/deepchem/models/seqtoseq.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 00:23:57.163554 deepchem-2.7.2.dev20230728002356/deepchem/models/sklearn_models/
--rw-r--r--   0 runner    (1001) docker     (123)       87 2023-07-28 00:23:40.000000 deepchem-2.7.2.dev20230728002356/deepchem/models/sklearn_models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5679 2023-07-28 00:23:40.000000 deepchem-2.7.2.dev20230728002356/deepchem/models/sklearn_models/sklearn_model.py
--rw-r--r--   0 runner    (1001) docker     (123)    10552 2023-07-28 00:23:40.000000 deepchem-2.7.2.dev20230728002356/deepchem/models/text_cnn.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 00:23:57.167554 deepchem-2.7.2.dev20230728002356/deepchem/models/torch_models/
--rw-r--r--   0 runner    (1001) docker     (123)     2343 2023-07-28 00:23:40.000000 deepchem-2.7.2.dev20230728002356/deepchem/models/torch_models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3633 2023-07-28 00:23:40.000000 deepchem-2.7.2.dev20230728002356/deepchem/models/torch_models/attention.py
--rw-r--r--   0 runner    (1001) docker     (123)    12226 2023-07-28 00:23:40.000000 deepchem-2.7.2.dev20230728002356/deepchem/models/torch_models/attentivefp.py
--rw-r--r--   0 runner    (1001) docker     (123)    14455 2023-07-28 00:23:40.000000 deepchem-2.7.2.dev20230728002356/deepchem/models/torch_models/cgcnn.py
--rw-r--r--   0 runner    (1001) docker     (123)     5551 2023-07-28 00:23:40.000000 deepchem-2.7.2.dev20230728002356/deepchem/models/torch_models/chemberta.py
--rw-r--r--   0 runner    (1001) docker     (123)     9543 2023-07-28 00:23:40.000000 deepchem-2.7.2.dev20230728002356/deepchem/models/torch_models/cnn.py
--rw-r--r--   0 runner    (1001) docker     (123)    31166 2023-07-28 00:23:40.000000 deepchem-2.7.2.dev20230728002356/deepchem/models/torch_models/dmpnn.py
--rw-r--r--   0 runner    (1001) docker     (123)     9721 2023-07-28 00:23:40.000000 deepchem-2.7.2.dev20230728002356/deepchem/models/torch_models/ferminet.py
--rw-r--r--   0 runner    (1001) docker     (123)    15845 2023-07-28 00:23:40.000000 deepchem-2.7.2.dev20230728002356/deepchem/models/torch_models/gat.py
--rw-r--r--   0 runner    (1001) docker     (123)    14944 2023-07-28 00:23:40.000000 deepchem-2.7.2.dev20230728002356/deepchem/models/torch_models/gcn.py
--rw-r--r--   0 runner    (1001) docker     (123)    51159 2023-07-28 00:23:40.000000 deepchem-2.7.2.dev20230728002356/deepchem/models/torch_models/gnn.py
--rw-r--r--   0 runner    (1001) docker     (123)    24969 2023-07-28 00:23:40.000000 deepchem-2.7.2.dev20230728002356/deepchem/models/torch_models/gnn3d.py
--rw-r--r--   0 runner    (1001) docker     (123)    38126 2023-07-28 00:23:40.000000 deepchem-2.7.2.dev20230728002356/deepchem/models/torch_models/grover.py
--rw-r--r--   0 runner    (1001) docker     (123)    38432 2023-07-28 00:23:40.000000 deepchem-2.7.2.dev20230728002356/deepchem/models/torch_models/grover_layers.py
--rw-r--r--   0 runner    (1001) docker     (123)    22942 2023-07-28 00:23:40.000000 deepchem-2.7.2.dev20230728002356/deepchem/models/torch_models/hf_models.py
--rw-r--r--   0 runner    (1001) docker     (123)    30077 2023-07-28 00:23:40.000000 deepchem-2.7.2.dev20230728002356/deepchem/models/torch_models/infograph.py
--rw-r--r--   0 runner    (1001) docker     (123)    19215 2023-07-28 00:23:40.000000 deepchem-2.7.2.dev20230728002356/deepchem/models/torch_models/kfac_optimizer.py
--rw-r--r--   0 runner    (1001) docker     (123)   172379 2023-07-28 00:23:40.000000 deepchem-2.7.2.dev20230728002356/deepchem/models/torch_models/layers.py
--rw-r--r--   0 runner    (1001) docker     (123)    18575 2023-07-28 00:23:40.000000 deepchem-2.7.2.dev20230728002356/deepchem/models/torch_models/lcnn.py
--rw-r--r--   0 runner    (1001) docker     (123)    17126 2023-07-28 00:23:40.000000 deepchem-2.7.2.dev20230728002356/deepchem/models/torch_models/mat.py
--rw-r--r--   0 runner    (1001) docker     (123)    11170 2023-07-28 00:23:40.000000 deepchem-2.7.2.dev20230728002356/deepchem/models/torch_models/megnet.py
--rw-r--r--   0 runner    (1001) docker     (123)    18122 2023-07-28 00:23:40.000000 deepchem-2.7.2.dev20230728002356/deepchem/models/torch_models/modular.py
--rw-r--r--   0 runner    (1001) docker     (123)    12074 2023-07-28 00:23:40.000000 deepchem-2.7.2.dev20230728002356/deepchem/models/torch_models/mpnn.py
--rw-r--r--   0 runner    (1001) docker     (123)     4165 2023-07-28 00:23:40.000000 deepchem-2.7.2.dev20230728002356/deepchem/models/torch_models/normalizing_flows_pytorch.py
--rw-r--r--   0 runner    (1001) docker     (123)    12297 2023-07-28 00:23:40.000000 deepchem-2.7.2.dev20230728002356/deepchem/models/torch_models/pagtn.py
--rw-r--r--   0 runner    (1001) docker     (123)    23016 2023-07-28 00:23:40.000000 deepchem-2.7.2.dev20230728002356/deepchem/models/torch_models/pna_gnn.py
--rw-r--r--   0 runner    (1001) docker     (123)     3528 2023-07-28 00:23:40.000000 deepchem-2.7.2.dev20230728002356/deepchem/models/torch_models/readout.py
--rw-r--r--   0 runner    (1001) docker     (123)    52726 2023-07-28 00:23:40.000000 deepchem-2.7.2.dev20230728002356/deepchem/models/torch_models/torch_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     5249 2023-07-28 00:23:40.000000 deepchem-2.7.2.dev20230728002356/deepchem/models/wandblogger.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 00:23:57.167554 deepchem-2.7.2.dev20230728002356/deepchem/molnet/
--rw-r--r--   0 runner    (1001) docker     (123)     3339 2023-07-28 00:23:40.000000 deepchem-2.7.2.dev20230728002356/deepchem/molnet/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11668 2023-07-28 00:23:40.000000 deepchem-2.7.2.dev20230728002356/deepchem/molnet/check_availability.py
--rw-r--r--   0 runner    (1001) docker     (123)     1845 2023-07-28 00:23:40.000000 deepchem-2.7.2.dev20230728002356/deepchem/molnet/defaults.py
--rw-r--r--   0 runner    (1001) docker     (123)    14702 2023-07-28 00:23:40.000000 deepchem-2.7.2.dev20230728002356/deepchem/molnet/dnasim.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 00:23:57.171554 deepchem-2.7.2.dev20230728002356/deepchem/molnet/load_function/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 00:23:40.000000 deepchem-2.7.2.dev20230728002356/deepchem/molnet/load_function/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5375 2023-07-28 00:23:40.000000 deepchem-2.7.2.dev20230728002356/deepchem/molnet/load_function/bace_datasets.py
--rw-r--r--   0 runner    (1001) docker     (123)    14202 2023-07-28 00:23:40.000000 deepchem-2.7.2.dev20230728002356/deepchem/molnet/load_function/bace_features.py
--rw-r--r--   0 runner    (1001) docker     (123)     5785 2023-07-28 00:23:40.000000 deepchem-2.7.2.dev20230728002356/deepchem/molnet/load_function/bbbc_datasets.py
--rw-r--r--   0 runner    (1001) docker     (123)     3604 2023-07-28 00:23:40.000000 deepchem-2.7.2.dev20230728002356/deepchem/molnet/load_function/bbbp_datasets.py
--rw-r--r--   0 runner    (1001) docker     (123)     2623 2023-07-28 00:23:40.000000 deepchem-2.7.2.dev20230728002356/deepchem/molnet/load_function/cell_counting_datasets.py
--rw-r--r--   0 runner    (1001) docker     (123)     4188 2023-07-28 00:23:40.000000 deepchem-2.7.2.dev20230728002356/deepchem/molnet/load_function/chembl25_datasets.py
--rw-r--r--   0 runner    (1001) docker     (123)     3706 2023-07-28 00:23:40.000000 deepchem-2.7.2.dev20230728002356/deepchem/molnet/load_function/chembl_datasets.py
--rw-r--r--   0 runner    (1001) docker     (123)    10252 2023-07-28 00:23:40.000000 deepchem-2.7.2.dev20230728002356/deepchem/molnet/load_function/chembl_tasks.py
--rw-r--r--   0 runner    (1001) docker     (123)     2625 2023-07-28 00:23:40.000000 deepchem-2.7.2.dev20230728002356/deepchem/molnet/load_function/clearance_datasets.py
--rw-r--r--   0 runner    (1001) docker     (123)     4245 2023-07-28 00:23:40.000000 deepchem-2.7.2.dev20230728002356/deepchem/molnet/load_function/clintox_datasets.py
--rw-r--r--   0 runner    (1001) docker     (123)     3507 2023-07-28 00:23:40.000000 deepchem-2.7.2.dev20230728002356/deepchem/molnet/load_function/delaney_datasets.py
--rw-r--r--   0 runner    (1001) docker     (123)     6957 2023-07-28 00:23:40.000000 deepchem-2.7.2.dev20230728002356/deepchem/molnet/load_function/factors_datasets.py
--rw-r--r--   0 runner    (1001) docker     (123)     3523 2023-07-28 00:23:40.000000 deepchem-2.7.2.dev20230728002356/deepchem/molnet/load_function/freesolv_dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)     3496 2023-07-28 00:23:40.000000 deepchem-2.7.2.dev20230728002356/deepchem/molnet/load_function/hiv_datasets.py
--rw-r--r--   0 runner    (1001) docker     (123)     3437 2023-07-28 00:23:40.000000 deepchem-2.7.2.dev20230728002356/deepchem/molnet/load_function/hopv_datasets.py
--rw-r--r--   0 runner    (1001) docker     (123)     2734 2023-07-28 00:23:40.000000 deepchem-2.7.2.dev20230728002356/deepchem/molnet/load_function/hppb_datasets.py
--rw-r--r--   0 runner    (1001) docker     (123)     6379 2023-07-28 00:23:40.000000 deepchem-2.7.2.dev20230728002356/deepchem/molnet/load_function/kaggle_datasets.py
--rw-r--r--   0 runner    (1001) docker     (123)   165414 2023-07-28 00:23:40.000000 deepchem-2.7.2.dev20230728002356/deepchem/molnet/load_function/kaggle_features.py
--rw-r--r--   0 runner    (1001) docker     (123)     8104 2023-07-28 00:23:40.000000 deepchem-2.7.2.dev20230728002356/deepchem/molnet/load_function/kinase_datasets.py
--rw-r--r--   0 runner    (1001) docker     (123)     3318 2023-07-28 00:23:40.000000 deepchem-2.7.2.dev20230728002356/deepchem/molnet/load_function/lipo_datasets.py
--rw-r--r--   0 runner    (1001) docker     (123)     9165 2023-07-28 00:23:40.000000 deepchem-2.7.2.dev20230728002356/deepchem/molnet/load_function/load_dataset_template.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 00:23:57.171554 deepchem-2.7.2.dev20230728002356/deepchem/molnet/load_function/material_datasets/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 00:23:40.000000 deepchem-2.7.2.dev20230728002356/deepchem/molnet/load_function/material_datasets/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4705 2023-07-28 00:23:40.000000 deepchem-2.7.2.dev20230728002356/deepchem/molnet/load_function/material_datasets/load_Pt_NO_surface_adsorbate_energy.py
--rw-r--r--   0 runner    (1001) docker     (123)     4474 2023-07-28 00:23:40.000000 deepchem-2.7.2.dev20230728002356/deepchem/molnet/load_function/material_datasets/load_bandgap.py
--rw-r--r--   0 runner    (1001) docker     (123)     4646 2023-07-28 00:23:40.000000 deepchem-2.7.2.dev20230728002356/deepchem/molnet/load_function/material_datasets/load_mp_formation_energy.py
--rw-r--r--   0 runner    (1001) docker     (123)     4589 2023-07-28 00:23:40.000000 deepchem-2.7.2.dev20230728002356/deepchem/molnet/load_function/material_datasets/load_mp_metallicity.py
--rw-r--r--   0 runner    (1001) docker     (123)     4516 2023-07-28 00:23:40.000000 deepchem-2.7.2.dev20230728002356/deepchem/molnet/load_function/material_datasets/load_perovskite.py
--rw-r--r--   0 runner    (1001) docker     (123)     8680 2023-07-28 00:23:40.000000 deepchem-2.7.2.dev20230728002356/deepchem/molnet/load_function/molnet_loader.py
--rw-r--r--   0 runner    (1001) docker     (123)     3631 2023-07-28 00:23:40.000000 deepchem-2.7.2.dev20230728002356/deepchem/molnet/load_function/muv_datasets.py
--rw-r--r--   0 runner    (1001) docker     (123)     3290 2023-07-28 00:23:40.000000 deepchem-2.7.2.dev20230728002356/deepchem/molnet/load_function/nci_datasets.py
--rw-r--r--   0 runner    (1001) docker     (123)     6927 2023-07-28 00:23:40.000000 deepchem-2.7.2.dev20230728002356/deepchem/molnet/load_function/pcba_datasets.py
--rw-r--r--   0 runner    (1001) docker     (123)     8586 2023-07-28 00:23:40.000000 deepchem-2.7.2.dev20230728002356/deepchem/molnet/load_function/pdbbind_datasets.py
--rw-r--r--   0 runner    (1001) docker     (123)     2549 2023-07-28 00:23:40.000000 deepchem-2.7.2.dev20230728002356/deepchem/molnet/load_function/ppb_datasets.py
--rw-r--r--   0 runner    (1001) docker     (123)     4800 2023-07-28 00:23:40.000000 deepchem-2.7.2.dev20230728002356/deepchem/molnet/load_function/qm7_datasets.py
--rw-r--r--   0 runner    (1001) docker     (123)     5045 2023-07-28 00:23:40.000000 deepchem-2.7.2.dev20230728002356/deepchem/molnet/load_function/qm8_datasets.py
--rw-r--r--   0 runner    (1001) docker     (123)     5697 2023-07-28 00:23:40.000000 deepchem-2.7.2.dev20230728002356/deepchem/molnet/load_function/qm9_datasets.py
--rw-r--r--   0 runner    (1001) docker     (123)     3567 2023-07-28 00:23:40.000000 deepchem-2.7.2.dev20230728002356/deepchem/molnet/load_function/sampl_datasets.py
--rw-r--r--   0 runner    (1001) docker     (123)     4640 2023-07-28 00:23:40.000000 deepchem-2.7.2.dev20230728002356/deepchem/molnet/load_function/sider_datasets.py
--rw-r--r--   0 runner    (1001) docker     (123)     3140 2023-07-28 00:23:40.000000 deepchem-2.7.2.dev20230728002356/deepchem/molnet/load_function/sweetlead_datasets.py
--rw-r--r--   0 runner    (1001) docker     (123)     2687 2023-07-28 00:23:40.000000 deepchem-2.7.2.dev20230728002356/deepchem/molnet/load_function/thermosol_datasets.py
--rw-r--r--   0 runner    (1001) docker     (123)     3530 2023-07-28 00:23:40.000000 deepchem-2.7.2.dev20230728002356/deepchem/molnet/load_function/tox21_datasets.py
--rw-r--r--   0 runner    (1001) docker     (123)    18900 2023-07-28 00:23:40.000000 deepchem-2.7.2.dev20230728002356/deepchem/molnet/load_function/toxcast_datasets.py
--rw-r--r--   0 runner    (1001) docker     (123)     7662 2023-07-28 00:23:40.000000 deepchem-2.7.2.dev20230728002356/deepchem/molnet/load_function/uspto_datasets.py
--rw-r--r--   0 runner    (1001) docker     (123)     6623 2023-07-28 00:23:40.000000 deepchem-2.7.2.dev20230728002356/deepchem/molnet/load_function/uv_datasets.py
--rw-r--r--   0 runner    (1001) docker     (123)     2036 2023-07-28 00:23:40.000000 deepchem-2.7.2.dev20230728002356/deepchem/molnet/load_function/uv_tasks.py
--rw-r--r--   0 runner    (1001) docker     (123)     6895 2023-07-28 00:23:40.000000 deepchem-2.7.2.dev20230728002356/deepchem/molnet/load_function/zinc15_datasets.py
--rw-r--r--   0 runner    (1001) docker     (123)     5319 2023-07-28 00:23:40.000000 deepchem-2.7.2.dev20230728002356/deepchem/molnet/preset_hyper_parameters.py
--rw-r--r--   0 runner    (1001) docker     (123)    13549 2023-07-28 00:23:40.000000 deepchem-2.7.2.dev20230728002356/deepchem/molnet/run_benchmark.py
--rw-r--r--   0 runner    (1001) docker     (123)     4874 2023-07-28 00:23:40.000000 deepchem-2.7.2.dev20230728002356/deepchem/molnet/run_benchmark_low_data.py
--rw-r--r--   0 runner    (1001) docker     (123)    36564 2023-07-28 00:23:40.000000 deepchem-2.7.2.dev20230728002356/deepchem/molnet/run_benchmark_models.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 00:23:57.171554 deepchem-2.7.2.dev20230728002356/deepchem/rl/
--rw-r--r--   0 runner    (1001) docker     (123)     9312 2023-07-28 00:23:40.000000 deepchem-2.7.2.dev20230728002356/deepchem/rl/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    23102 2023-07-28 00:23:40.000000 deepchem-2.7.2.dev20230728002356/deepchem/rl/a2c.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 00:23:57.171554 deepchem-2.7.2.dev20230728002356/deepchem/rl/envs/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 00:23:40.000000 deepchem-2.7.2.dev20230728002356/deepchem/rl/envs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1773 2023-07-28 00:23:40.000000 deepchem-2.7.2.dev20230728002356/deepchem/rl/envs/test_tictactoe.py
--rw-r--r--   0 runner    (1001) docker     (123)     3632 2023-07-28 00:23:40.000000 deepchem-2.7.2.dev20230728002356/deepchem/rl/envs/tictactoe.py
--rw-r--r--   0 runner    (1001) docker     (123)    25262 2023-07-28 00:23:40.000000 deepchem-2.7.2.dev20230728002356/deepchem/rl/ppo.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 00:23:57.171554 deepchem-2.7.2.dev20230728002356/deepchem/splits/
--rw-r--r--   0 runner    (1001) docker     (123)     1384 2023-07-28 00:23:40.000000 deepchem-2.7.2.dev20230728002356/deepchem/splits/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    63895 2023-07-28 00:23:40.000000 deepchem-2.7.2.dev20230728002356/deepchem/splits/splitters.py
--rw-r--r--   0 runner    (1001) docker     (123)     4017 2023-07-28 00:23:40.000000 deepchem-2.7.2.dev20230728002356/deepchem/splits/task_splitter.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 00:23:57.171554 deepchem-2.7.2.dev20230728002356/deepchem/trans/
--rw-r--r--   0 runner    (1001) docker     (123)     1255 2023-07-28 00:23:40.000000 deepchem-2.7.2.dev20230728002356/deepchem/trans/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6571 2023-07-28 00:23:40.000000 deepchem-2.7.2.dev20230728002356/deepchem/trans/duplicate.py
--rw-r--r--   0 runner    (1001) docker     (123)    91191 2023-07-28 00:23:40.000000 deepchem-2.7.2.dev20230728002356/deepchem/trans/transformers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 00:23:57.175554 deepchem-2.7.2.dev20230728002356/deepchem/utils/
--rw-r--r--   0 runner    (1001) docker     (123)     6141 2023-07-28 00:23:40.000000 deepchem-2.7.2.dev20230728002356/deepchem/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10069 2023-07-28 00:23:40.000000 deepchem-2.7.2.dev20230728002356/deepchem/utils/conformers.py
--rw-r--r--   0 runner    (1001) docker     (123)    13294 2023-07-28 00:23:40.000000 deepchem-2.7.2.dev20230728002356/deepchem/utils/coordinate_box_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    20923 2023-07-28 00:23:40.000000 deepchem-2.7.2.dev20230728002356/deepchem/utils/data_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     1840 2023-07-28 00:23:40.000000 deepchem-2.7.2.dev20230728002356/deepchem/utils/debug_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     3041 2023-07-28 00:23:40.000000 deepchem-2.7.2.dev20230728002356/deepchem/utils/dftutils.py
--rw-r--r--   0 runner    (1001) docker     (123)    10476 2023-07-28 00:23:40.000000 deepchem-2.7.2.dev20230728002356/deepchem/utils/docking_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    14881 2023-07-28 00:23:40.000000 deepchem-2.7.2.dev20230728002356/deepchem/utils/electron_sampler.py
--rw-r--r--   0 runner    (1001) docker     (123)    19454 2023-07-28 00:23:40.000000 deepchem-2.7.2.dev20230728002356/deepchem/utils/evaluate.py
--rw-r--r--   0 runner    (1001) docker     (123)     6134 2023-07-28 00:23:40.000000 deepchem-2.7.2.dev20230728002356/deepchem/utils/fake_data_generator.py
--rw-r--r--   0 runner    (1001) docker     (123)    13312 2023-07-28 00:23:40.000000 deepchem-2.7.2.dev20230728002356/deepchem/utils/fragment_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     3903 2023-07-28 00:23:40.000000 deepchem-2.7.2.dev20230728002356/deepchem/utils/genomics_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     8259 2023-07-28 00:23:40.000000 deepchem-2.7.2.dev20230728002356/deepchem/utils/geometry_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     6033 2023-07-28 00:23:40.000000 deepchem-2.7.2.dev20230728002356/deepchem/utils/graph_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     6554 2023-07-28 00:23:40.000000 deepchem-2.7.2.dev20230728002356/deepchem/utils/grover.py
--rw-r--r--   0 runner    (1001) docker     (123)     3644 2023-07-28 00:23:40.000000 deepchem-2.7.2.dev20230728002356/deepchem/utils/hash_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    19262 2023-07-28 00:23:40.000000 deepchem-2.7.2.dev20230728002356/deepchem/utils/molecule_feature_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    17713 2023-07-28 00:23:40.000000 deepchem-2.7.2.dev20230728002356/deepchem/utils/noncovalent_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    11749 2023-07-28 00:23:40.000000 deepchem-2.7.2.dev20230728002356/deepchem/utils/pdbqt_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     4341 2023-07-28 00:23:40.000000 deepchem-2.7.2.dev20230728002356/deepchem/utils/pytorch_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    65672 2023-07-28 00:23:40.000000 deepchem-2.7.2.dev20230728002356/deepchem/utils/rdkit_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      552 2023-07-28 00:23:40.000000 deepchem-2.7.2.dev20230728002356/deepchem/utils/save.py
--rw-r--r--   0 runner    (1001) docker     (123)     6815 2023-07-28 00:23:40.000000 deepchem-2.7.2.dev20230728002356/deepchem/utils/sequence_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 00:23:57.175554 deepchem-2.7.2.dev20230728002356/deepchem/utils/test/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 00:23:40.000000 deepchem-2.7.2.dev20230728002356/deepchem/utils/test/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6598 2023-07-28 00:23:40.000000 deepchem-2.7.2.dev20230728002356/deepchem/utils/test/test_coordinate_box_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      788 2023-07-28 00:23:40.000000 deepchem-2.7.2.dev20230728002356/deepchem/utils/test/test_data_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      896 2023-07-28 00:23:40.000000 deepchem-2.7.2.dev20230728002356/deepchem/utils/test/test_dftutils.py
--rw-r--r--   0 runner    (1001) docker     (123)     2258 2023-07-28 00:23:40.000000 deepchem-2.7.2.dev20230728002356/deepchem/utils/test/test_docking_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     3522 2023-07-28 00:23:40.000000 deepchem-2.7.2.dev20230728002356/deepchem/utils/test/test_electron_sampler.py
--rw-r--r--   0 runner    (1001) docker     (123)    12977 2023-07-28 00:23:40.000000 deepchem-2.7.2.dev20230728002356/deepchem/utils/test/test_evaluate.py
--rw-r--r--   0 runner    (1001) docker     (123)     2481 2023-07-28 00:23:40.000000 deepchem-2.7.2.dev20230728002356/deepchem/utils/test/test_fake_data_generator.py
--rw-r--r--   0 runner    (1001) docker     (123)     2610 2023-07-28 00:23:40.000000 deepchem-2.7.2.dev20230728002356/deepchem/utils/test/test_fragment_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     4684 2023-07-28 00:23:40.000000 deepchem-2.7.2.dev20230728002356/deepchem/utils/test/test_generator_evaluator.py
--rw-r--r--   0 runner    (1001) docker     (123)     1956 2023-07-28 00:23:40.000000 deepchem-2.7.2.dev20230728002356/deepchem/utils/test/test_genomics_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     3296 2023-07-28 00:23:40.000000 deepchem-2.7.2.dev20230728002356/deepchem/utils/test/test_geometry_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      866 2023-07-28 00:23:40.000000 deepchem-2.7.2.dev20230728002356/deepchem/utils/test/test_graph_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     1523 2023-07-28 00:23:40.000000 deepchem-2.7.2.dev20230728002356/deepchem/utils/test/test_grover.py
--rw-r--r--   0 runner    (1001) docker     (123)     1476 2023-07-28 00:23:40.000000 deepchem-2.7.2.dev20230728002356/deepchem/utils/test/test_hash_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     9115 2023-07-28 00:23:40.000000 deepchem-2.7.2.dev20230728002356/deepchem/utils/test/test_molecule_feature_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     6251 2023-07-28 00:23:40.000000 deepchem-2.7.2.dev20230728002356/deepchem/utils/test/test_noncovalent_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     3922 2023-07-28 00:23:40.000000 deepchem-2.7.2.dev20230728002356/deepchem/utils/test/test_pdbqt_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     1577 2023-07-28 00:23:40.000000 deepchem-2.7.2.dev20230728002356/deepchem/utils/test/test_pytorch_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     9005 2023-07-28 00:23:40.000000 deepchem-2.7.2.dev20230728002356/deepchem/utils/test/test_rdkit_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     2388 2023-07-28 00:23:40.000000 deepchem-2.7.2.dev20230728002356/deepchem/utils/test/test_sequence_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      386 2023-07-28 00:23:40.000000 deepchem-2.7.2.dev20230728002356/deepchem/utils/test/test_updated_scipy.py
--rw-r--r--   0 runner    (1001) docker     (123)     2859 2023-07-28 00:23:40.000000 deepchem-2.7.2.dev20230728002356/deepchem/utils/test/test_voxel_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      919 2023-07-28 00:23:40.000000 deepchem-2.7.2.dev20230728002356/deepchem/utils/typing.py
--rw-r--r--   0 runner    (1001) docker     (123)     1113 2023-07-28 00:23:40.000000 deepchem-2.7.2.dev20230728002356/deepchem/utils/vina_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     7797 2023-07-28 00:23:40.000000 deepchem-2.7.2.dev20230728002356/deepchem/utils/voxel_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 00:23:57.151554 deepchem-2.7.2.dev20230728002356/deepchem.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-07-28 00:23:57.000000 deepchem-2.7.2.dev20230728002356/deepchem.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    10767 2023-07-28 00:23:57.000000 deepchem-2.7.2.dev20230728002356/deepchem.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 00:23:57.000000 deepchem-2.7.2.dev20230728002356/deepchem.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      249 2023-07-28 00:23:57.000000 deepchem-2.7.2.dev20230728002356/deepchem.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-28 00:23:57.000000 deepchem-2.7.2.dev20230728002356/deepchem.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      701 2023-07-28 00:23:57.175554 deepchem-2.7.2.dev20230728002356/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2670 2023-07-28 00:23:40.000000 deepchem-2.7.2.dev20230728002356/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 20:07:10.932470 deepchem-2.7.2.dev20230730200710/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1047 2023-07-30 20:06:57.000000 deepchem-2.7.2.dev20230730200710/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-07-30 20:07:10.932470 deepchem-2.7.2.dev20230730200710/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     7124 2023-07-30 20:06:57.000000 deepchem-2.7.2.dev20230730200710/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 20:07:10.840470 deepchem-2.7.2.dev20230730200710/deepchem/
+-rw-r--r--   0 runner    (1001) docker     (123)      373 2023-07-30 20:06:57.000000 deepchem-2.7.2.dev20230730200710/deepchem/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 20:07:10.844470 deepchem-2.7.2.dev20230730200710/deepchem/data/
+-rw-r--r--   0 runner    (1001) docker     (123)      939 2023-07-30 20:06:57.000000 deepchem-2.7.2.dev20230730200710/deepchem/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    67994 2023-07-30 20:06:57.000000 deepchem-2.7.2.dev20230730200710/deepchem/data/data_loader.py
+-rw-r--r--   0 runner    (1001) docker     (123)   118009 2023-07-30 20:06:57.000000 deepchem-2.7.2.dev20230730200710/deepchem/data/datasets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7256 2023-07-30 20:06:57.000000 deepchem-2.7.2.dev20230730200710/deepchem/data/pytorch_datasets.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12606 2023-07-30 20:06:57.000000 deepchem-2.7.2.dev20230730200710/deepchem/data/supports.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 20:07:10.844470 deepchem-2.7.2.dev20230730200710/deepchem/dock/
+-rw-r--r--   0 runner    (1001) docker     (123)      297 2023-07-30 20:06:57.000000 deepchem-2.7.2.dev20230730200710/deepchem/dock/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4910 2023-07-30 20:06:57.000000 deepchem-2.7.2.dev20230730200710/deepchem/dock/binding_pocket.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6105 2023-07-30 20:06:57.000000 deepchem-2.7.2.dev20230730200710/deepchem/dock/docking.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19576 2023-07-30 20:06:57.000000 deepchem-2.7.2.dev20230730200710/deepchem/dock/pose_generation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6917 2023-07-30 20:06:57.000000 deepchem-2.7.2.dev20230730200710/deepchem/dock/pose_scoring.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 20:07:10.852470 deepchem-2.7.2.dev20230730200710/deepchem/feat/
+-rw-r--r--   0 runner    (1001) docker     (123)     4521 2023-07-30 20:06:57.000000 deepchem-2.7.2.dev20230730200710/deepchem/feat/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7335 2023-07-30 20:06:57.000000 deepchem-2.7.2.dev20230730200710/deepchem/feat/atomic_conformation.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19458 2023-07-30 20:06:57.000000 deepchem-2.7.2.dev20230730200710/deepchem/feat/base_classes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1904 2023-07-30 20:06:57.000000 deepchem-2.7.2.dev20230730200710/deepchem/feat/bert_tokenizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4368 2023-07-30 20:06:57.000000 deepchem-2.7.2.dev20230730200710/deepchem/feat/binding_pocket_features.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 20:07:10.852470 deepchem-2.7.2.dev20230730200710/deepchem/feat/complex_featurizers/
+-rw-r--r--   0 runner    (1001) docker     (123)     1400 2023-07-30 20:06:57.000000 deepchem-2.7.2.dev20230730200710/deepchem/feat/complex_featurizers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12898 2023-07-30 20:06:57.000000 deepchem-2.7.2.dev20230730200710/deepchem/feat/complex_featurizers/complex_atomic_coordinates.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10769 2023-07-30 20:06:57.000000 deepchem-2.7.2.dev20230730200710/deepchem/feat/complex_featurizers/contact_fingerprints.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27676 2023-07-30 20:06:57.000000 deepchem-2.7.2.dev20230730200710/deepchem/feat/complex_featurizers/grid_featurizers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20248 2023-07-30 20:06:57.000000 deepchem-2.7.2.dev20230730200710/deepchem/feat/complex_featurizers/rdkit_grid_featurizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11465 2023-07-30 20:06:57.000000 deepchem-2.7.2.dev20230730200710/deepchem/feat/complex_featurizers/splif_fingerprints.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11743 2023-07-30 20:06:57.000000 deepchem-2.7.2.dev20230730200710/deepchem/feat/dft_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22111 2023-07-30 20:06:57.000000 deepchem-2.7.2.dev20230730200710/deepchem/feat/graph_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)    38890 2023-07-30 20:06:57.000000 deepchem-2.7.2.dev20230730200710/deepchem/feat/graph_features.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1396 2023-07-30 20:06:57.000000 deepchem-2.7.2.dev20230730200710/deepchem/feat/huggingface_featurizer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 20:07:10.852470 deepchem-2.7.2.dev20230730200710/deepchem/feat/material_featurizers/
+-rw-r--r--   0 runner    (1001) docker     (123)      489 2023-07-30 20:06:57.000000 deepchem-2.7.2.dev20230730200710/deepchem/feat/material_featurizers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7539 2023-07-30 20:06:57.000000 deepchem-2.7.2.dev20230730200710/deepchem/feat/material_featurizers/cgcnn_featurizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3508 2023-07-30 20:06:57.000000 deepchem-2.7.2.dev20230730200710/deepchem/feat/material_featurizers/element_property_fingerprint.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3232 2023-07-30 20:06:57.000000 deepchem-2.7.2.dev20230730200710/deepchem/feat/material_featurizers/elemnet_featurizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28058 2023-07-30 20:06:57.000000 deepchem-2.7.2.dev20230730200710/deepchem/feat/material_featurizers/lcnn_featurizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3823 2023-07-30 20:06:57.000000 deepchem-2.7.2.dev20230730200710/deepchem/feat/material_featurizers/sine_coulomb_matrix.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14808 2023-07-30 20:06:57.000000 deepchem-2.7.2.dev20230730200710/deepchem/feat/mol_graphs.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 20:07:10.860470 deepchem-2.7.2.dev20230730200710/deepchem/feat/molecule_featurizers/
+-rw-r--r--   0 runner    (1001) docker     (123)     2156 2023-07-30 20:06:57.000000 deepchem-2.7.2.dev20230730200710/deepchem/feat/molecule_featurizers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2884 2023-07-30 20:06:57.000000 deepchem-2.7.2.dev20230730200710/deepchem/feat/molecule_featurizers/atomic_coordinates.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2376 2023-07-30 20:06:57.000000 deepchem-2.7.2.dev20230730200710/deepchem/feat/molecule_featurizers/bp_symmetry_function_input.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6488 2023-07-30 20:06:57.000000 deepchem-2.7.2.dev20230730200710/deepchem/feat/molecule_featurizers/circular_fingerprint.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9242 2023-07-30 20:06:57.000000 deepchem-2.7.2.dev20230730200710/deepchem/feat/molecule_featurizers/conformer_featurizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10925 2023-07-30 20:06:57.000000 deepchem-2.7.2.dev20230730200710/deepchem/feat/molecule_featurizers/coulomb_matrices.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19123 2023-07-30 20:06:57.000000 deepchem-2.7.2.dev20230730200710/deepchem/feat/molecule_featurizers/dmpnn_featurizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7507 2023-07-30 20:06:57.000000 deepchem-2.7.2.dev20230730200710/deepchem/feat/molecule_featurizers/grover_featurizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2046 2023-07-30 20:06:57.000000 deepchem-2.7.2.dev20230730200710/deepchem/feat/molecule_featurizers/maccs_keys_fingerprint.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8401 2023-07-30 20:06:57.000000 deepchem-2.7.2.dev20230730200710/deepchem/feat/molecule_featurizers/mat_featurizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7587 2023-07-30 20:06:57.000000 deepchem-2.7.2.dev20230730200710/deepchem/feat/molecule_featurizers/mol2vec_fingerprint.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20381 2023-07-30 20:06:57.000000 deepchem-2.7.2.dev20230730200710/deepchem/feat/molecule_featurizers/mol_graph_conv_featurizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9346 2023-07-30 20:06:57.000000 deepchem-2.7.2.dev20230730200710/deepchem/feat/molecule_featurizers/molgan_featurizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2835 2023-07-30 20:06:57.000000 deepchem-2.7.2.dev20230730200710/deepchem/feat/molecule_featurizers/mordred_descriptors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5130 2023-07-30 20:06:57.000000 deepchem-2.7.2.dev20230730200710/deepchem/feat/molecule_featurizers/mxmnet_featurizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6359 2023-07-30 20:06:57.000000 deepchem-2.7.2.dev20230730200710/deepchem/feat/molecule_featurizers/one_hot_featurizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2258 2023-07-30 20:06:57.000000 deepchem-2.7.2.dev20230730200710/deepchem/feat/molecule_featurizers/pubchem_fingerprint.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1687 2023-07-30 20:06:57.000000 deepchem-2.7.2.dev20230730200710/deepchem/feat/molecule_featurizers/raw_featurizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9881 2023-07-30 20:06:57.000000 deepchem-2.7.2.dev20230730200710/deepchem/feat/molecule_featurizers/rdkit_descriptors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7280 2023-07-30 20:06:57.000000 deepchem-2.7.2.dev20230730200710/deepchem/feat/molecule_featurizers/smiles_to_image.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5433 2023-07-30 20:06:57.000000 deepchem-2.7.2.dev20230730200710/deepchem/feat/molecule_featurizers/smiles_to_seq.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4313 2023-07-30 20:06:57.000000 deepchem-2.7.2.dev20230730200710/deepchem/feat/molecule_featurizers/snap_featurizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3448 2023-07-30 20:06:57.000000 deepchem-2.7.2.dev20230730200710/deepchem/feat/molecule_featurizers/sparse_matrix_one_hot_featurizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3909 2023-07-30 20:06:57.000000 deepchem-2.7.2.dev20230730200710/deepchem/feat/reaction_featurizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2326 2023-07-30 20:06:57.000000 deepchem-2.7.2.dev20230730200710/deepchem/feat/roberta_tokenizer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 20:07:10.860470 deepchem-2.7.2.dev20230730200710/deepchem/feat/sequence_featurizers/
+-rw-r--r--   0 runner    (1001) docker     (123)      112 2023-07-30 20:06:57.000000 deepchem-2.7.2.dev20230730200710/deepchem/feat/sequence_featurizers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3383 2023-07-30 20:06:57.000000 deepchem-2.7.2.dev20230730200710/deepchem/feat/sequence_featurizers/position_frequency_matrix_featurizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11383 2023-07-30 20:06:57.000000 deepchem-2.7.2.dev20230730200710/deepchem/feat/smiles_tokenizer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 20:07:10.860470 deepchem-2.7.2.dev20230730200710/deepchem/feat/vocabulary_builders/
+-rw-r--r--   0 runner    (1001) docker     (123)      278 2023-07-30 20:06:57.000000 deepchem-2.7.2.dev20230730200710/deepchem/feat/vocabulary_builders/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18726 2023-07-30 20:06:57.000000 deepchem-2.7.2.dev20230730200710/deepchem/feat/vocabulary_builders/grover_vocab.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2315 2023-07-30 20:06:57.000000 deepchem-2.7.2.dev20230730200710/deepchem/feat/vocabulary_builders/hf_vocab.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1116 2023-07-30 20:06:57.000000 deepchem-2.7.2.dev20230730200710/deepchem/feat/vocabulary_builders/vocabulary_builder.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 20:07:10.860470 deepchem-2.7.2.dev20230730200710/deepchem/hyper/
+-rw-r--r--   0 runner    (1001) docker     (123)      260 2023-07-30 20:06:57.000000 deepchem-2.7.2.dev20230730200710/deepchem/hyper/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5702 2023-07-30 20:06:57.000000 deepchem-2.7.2.dev20230730200710/deepchem/hyper/base_classes.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17151 2023-07-30 20:06:57.000000 deepchem-2.7.2.dev20230730200710/deepchem/hyper/gaussian_process.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10208 2023-07-30 20:06:57.000000 deepchem-2.7.2.dev20230730200710/deepchem/hyper/grid_search.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12427 2023-07-30 20:06:57.000000 deepchem-2.7.2.dev20230730200710/deepchem/hyper/random_search.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 20:07:10.860470 deepchem-2.7.2.dev20230730200710/deepchem/metalearning/
+-rw-r--r--   0 runner    (1001) docker     (123)      118 2023-07-30 20:06:57.000000 deepchem-2.7.2.dev20230730200710/deepchem/metalearning/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10539 2023-07-30 20:06:57.000000 deepchem-2.7.2.dev20230730200710/deepchem/metalearning/maml.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 20:07:10.860470 deepchem-2.7.2.dev20230730200710/deepchem/metrics/
+-rw-r--r--   0 runner    (1001) docker     (123)     2015 2023-07-30 20:06:57.000000 deepchem-2.7.2.dev20230730200710/deepchem/metrics/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7715 2023-07-30 20:06:57.000000 deepchem-2.7.2.dev20230730200710/deepchem/metrics/genomic_metrics.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31620 2023-07-30 20:06:57.000000 deepchem-2.7.2.dev20230730200710/deepchem/metrics/metric.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6533 2023-07-30 20:06:57.000000 deepchem-2.7.2.dev20230730200710/deepchem/metrics/score_function.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 20:07:10.868470 deepchem-2.7.2.dev20230730200710/deepchem/models/
+-rw-r--r--   0 runner    (1001) docker     (123)     4780 2023-07-30 20:06:57.000000 deepchem-2.7.2.dev20230730200710/deepchem/models/IRV.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4420 2023-07-30 20:06:57.000000 deepchem-2.7.2.dev20230730200710/deepchem/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13833 2023-07-30 20:06:57.000000 deepchem-2.7.2.dev20230730200710/deepchem/models/atomic_conv.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4414 2023-07-30 20:06:57.000000 deepchem-2.7.2.dev20230730200710/deepchem/models/callbacks.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17354 2023-07-30 20:06:57.000000 deepchem-2.7.2.dev20230730200710/deepchem/models/chemnet_layers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15504 2023-07-30 20:06:57.000000 deepchem-2.7.2.dev20230730200710/deepchem/models/chemnet_models.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 20:07:10.868470 deepchem-2.7.2.dev20230730200710/deepchem/models/dft/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-30 20:06:57.000000 deepchem-2.7.2.dev20230730200710/deepchem/models/dft/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9553 2023-07-30 20:06:57.000000 deepchem-2.7.2.dev20230730200710/deepchem/models/dft/dftxc.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14020 2023-07-30 20:06:57.000000 deepchem-2.7.2.dev20230730200710/deepchem/models/dft/nnxc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4664 2023-07-30 20:06:57.000000 deepchem-2.7.2.dev20230730200710/deepchem/models/dft/scf.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23457 2023-07-30 20:06:57.000000 deepchem-2.7.2.dev20230730200710/deepchem/models/fcnet.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24548 2023-07-30 20:06:57.000000 deepchem-2.7.2.dev20230730200710/deepchem/models/gan.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 20:07:10.868470 deepchem-2.7.2.dev20230730200710/deepchem/models/gbdt_models/
+-rw-r--r--   0 runner    (1001) docker     (123)       75 2023-07-30 20:06:57.000000 deepchem-2.7.2.dev20230730200710/deepchem/models/gbdt_models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5921 2023-07-30 20:06:57.000000 deepchem-2.7.2.dev20230730200710/deepchem/models/gbdt_models/gbdt_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)    57408 2023-07-30 20:06:57.000000 deepchem-2.7.2.dev20230730200710/deepchem/models/graph_models.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 20:07:10.868470 deepchem-2.7.2.dev20230730200710/deepchem/models/jax_models/
+-rw-r--r--   0 runner    (1001) docker     (123)      133 2023-07-30 20:06:57.000000 deepchem-2.7.2.dev20230730200710/deepchem/models/jax_models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28179 2023-07-30 20:06:57.000000 deepchem-2.7.2.dev20230730200710/deepchem/models/jax_models/jax_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3408 2023-07-30 20:06:57.000000 deepchem-2.7.2.dev20230730200710/deepchem/models/jax_models/layers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17070 2023-07-30 20:06:57.000000 deepchem-2.7.2.dev20230730200710/deepchem/models/jax_models/pinns_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)    56522 2023-07-30 20:06:57.000000 deepchem-2.7.2.dev20230730200710/deepchem/models/keras_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)   144759 2023-07-30 20:06:57.000000 deepchem-2.7.2.dev20230730200710/deepchem/models/layers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 20:07:10.868470 deepchem-2.7.2.dev20230730200710/deepchem/models/lightning/
+-rw-r--r--   0 runner    (1001) docker     (123)      181 2023-07-30 20:06:57.000000 deepchem-2.7.2.dev20230730200710/deepchem/models/lightning/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1742 2023-07-30 20:06:57.000000 deepchem-2.7.2.dev20230730200710/deepchem/models/lightning/dc_lightning_dataset_module.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2447 2023-07-30 20:06:57.000000 deepchem-2.7.2.dev20230730200710/deepchem/models/lightning/dc_lightning_module.py
+-rw-r--r--   0 runner    (1001) docker     (123)    61903 2023-07-30 20:06:57.000000 deepchem-2.7.2.dev20230730200710/deepchem/models/losses.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8256 2023-07-30 20:06:57.000000 deepchem-2.7.2.dev20230730200710/deepchem/models/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14135 2023-07-30 20:06:57.000000 deepchem-2.7.2.dev20230730200710/deepchem/models/molgan.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5437 2023-07-30 20:06:57.000000 deepchem-2.7.2.dev20230730200710/deepchem/models/multitask.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10975 2023-07-30 20:06:57.000000 deepchem-2.7.2.dev20230730200710/deepchem/models/normalizing_flows.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26871 2023-07-30 20:06:57.000000 deepchem-2.7.2.dev20230730200710/deepchem/models/optimizers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13095 2023-07-30 20:06:57.000000 deepchem-2.7.2.dev20230730200710/deepchem/models/progressive_multitask.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17830 2023-07-30 20:06:57.000000 deepchem-2.7.2.dev20230730200710/deepchem/models/robust_multitask.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4546 2023-07-30 20:06:57.000000 deepchem-2.7.2.dev20230730200710/deepchem/models/scscore.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25969 2023-07-30 20:06:57.000000 deepchem-2.7.2.dev20230730200710/deepchem/models/seqtoseq.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 20:07:10.868470 deepchem-2.7.2.dev20230730200710/deepchem/models/sklearn_models/
+-rw-r--r--   0 runner    (1001) docker     (123)       87 2023-07-30 20:06:57.000000 deepchem-2.7.2.dev20230730200710/deepchem/models/sklearn_models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5679 2023-07-30 20:06:57.000000 deepchem-2.7.2.dev20230730200710/deepchem/models/sklearn_models/sklearn_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10552 2023-07-30 20:06:57.000000 deepchem-2.7.2.dev20230730200710/deepchem/models/text_cnn.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 20:07:10.876470 deepchem-2.7.2.dev20230730200710/deepchem/models/torch_models/
+-rw-r--r--   0 runner    (1001) docker     (123)     2343 2023-07-30 20:06:57.000000 deepchem-2.7.2.dev20230730200710/deepchem/models/torch_models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3633 2023-07-30 20:06:57.000000 deepchem-2.7.2.dev20230730200710/deepchem/models/torch_models/attention.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12226 2023-07-30 20:06:57.000000 deepchem-2.7.2.dev20230730200710/deepchem/models/torch_models/attentivefp.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14455 2023-07-30 20:06:57.000000 deepchem-2.7.2.dev20230730200710/deepchem/models/torch_models/cgcnn.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5551 2023-07-30 20:06:57.000000 deepchem-2.7.2.dev20230730200710/deepchem/models/torch_models/chemberta.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9543 2023-07-30 20:06:57.000000 deepchem-2.7.2.dev20230730200710/deepchem/models/torch_models/cnn.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31166 2023-07-30 20:06:57.000000 deepchem-2.7.2.dev20230730200710/deepchem/models/torch_models/dmpnn.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9721 2023-07-30 20:06:57.000000 deepchem-2.7.2.dev20230730200710/deepchem/models/torch_models/ferminet.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15845 2023-07-30 20:06:57.000000 deepchem-2.7.2.dev20230730200710/deepchem/models/torch_models/gat.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14944 2023-07-30 20:06:57.000000 deepchem-2.7.2.dev20230730200710/deepchem/models/torch_models/gcn.py
+-rw-r--r--   0 runner    (1001) docker     (123)    51159 2023-07-30 20:06:57.000000 deepchem-2.7.2.dev20230730200710/deepchem/models/torch_models/gnn.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24969 2023-07-30 20:06:57.000000 deepchem-2.7.2.dev20230730200710/deepchem/models/torch_models/gnn3d.py
+-rw-r--r--   0 runner    (1001) docker     (123)    38126 2023-07-30 20:06:57.000000 deepchem-2.7.2.dev20230730200710/deepchem/models/torch_models/grover.py
+-rw-r--r--   0 runner    (1001) docker     (123)    38432 2023-07-30 20:06:57.000000 deepchem-2.7.2.dev20230730200710/deepchem/models/torch_models/grover_layers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22942 2023-07-30 20:06:57.000000 deepchem-2.7.2.dev20230730200710/deepchem/models/torch_models/hf_models.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30077 2023-07-30 20:06:57.000000 deepchem-2.7.2.dev20230730200710/deepchem/models/torch_models/infograph.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19215 2023-07-30 20:06:57.000000 deepchem-2.7.2.dev20230730200710/deepchem/models/torch_models/kfac_optimizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)   174380 2023-07-30 20:06:57.000000 deepchem-2.7.2.dev20230730200710/deepchem/models/torch_models/layers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18575 2023-07-30 20:06:57.000000 deepchem-2.7.2.dev20230730200710/deepchem/models/torch_models/lcnn.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17126 2023-07-30 20:06:57.000000 deepchem-2.7.2.dev20230730200710/deepchem/models/torch_models/mat.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11170 2023-07-30 20:06:57.000000 deepchem-2.7.2.dev20230730200710/deepchem/models/torch_models/megnet.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18122 2023-07-30 20:06:57.000000 deepchem-2.7.2.dev20230730200710/deepchem/models/torch_models/modular.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12074 2023-07-30 20:06:57.000000 deepchem-2.7.2.dev20230730200710/deepchem/models/torch_models/mpnn.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4165 2023-07-30 20:06:57.000000 deepchem-2.7.2.dev20230730200710/deepchem/models/torch_models/normalizing_flows_pytorch.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12297 2023-07-30 20:06:57.000000 deepchem-2.7.2.dev20230730200710/deepchem/models/torch_models/pagtn.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23016 2023-07-30 20:06:57.000000 deepchem-2.7.2.dev20230730200710/deepchem/models/torch_models/pna_gnn.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3528 2023-07-30 20:06:57.000000 deepchem-2.7.2.dev20230730200710/deepchem/models/torch_models/readout.py
+-rw-r--r--   0 runner    (1001) docker     (123)    52726 2023-07-30 20:06:57.000000 deepchem-2.7.2.dev20230730200710/deepchem/models/torch_models/torch_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5249 2023-07-30 20:06:57.000000 deepchem-2.7.2.dev20230730200710/deepchem/models/wandblogger.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 20:07:10.880470 deepchem-2.7.2.dev20230730200710/deepchem/molnet/
+-rw-r--r--   0 runner    (1001) docker     (123)     3339 2023-07-30 20:06:57.000000 deepchem-2.7.2.dev20230730200710/deepchem/molnet/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11668 2023-07-30 20:06:57.000000 deepchem-2.7.2.dev20230730200710/deepchem/molnet/check_availability.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1845 2023-07-30 20:06:57.000000 deepchem-2.7.2.dev20230730200710/deepchem/molnet/defaults.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14702 2023-07-30 20:06:57.000000 deepchem-2.7.2.dev20230730200710/deepchem/molnet/dnasim.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 20:07:10.900470 deepchem-2.7.2.dev20230730200710/deepchem/molnet/load_function/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-30 20:06:57.000000 deepchem-2.7.2.dev20230730200710/deepchem/molnet/load_function/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5375 2023-07-30 20:06:57.000000 deepchem-2.7.2.dev20230730200710/deepchem/molnet/load_function/bace_datasets.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14202 2023-07-30 20:06:57.000000 deepchem-2.7.2.dev20230730200710/deepchem/molnet/load_function/bace_features.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5785 2023-07-30 20:06:57.000000 deepchem-2.7.2.dev20230730200710/deepchem/molnet/load_function/bbbc_datasets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3604 2023-07-30 20:06:57.000000 deepchem-2.7.2.dev20230730200710/deepchem/molnet/load_function/bbbp_datasets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2623 2023-07-30 20:06:57.000000 deepchem-2.7.2.dev20230730200710/deepchem/molnet/load_function/cell_counting_datasets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4188 2023-07-30 20:06:57.000000 deepchem-2.7.2.dev20230730200710/deepchem/molnet/load_function/chembl25_datasets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3706 2023-07-30 20:06:57.000000 deepchem-2.7.2.dev20230730200710/deepchem/molnet/load_function/chembl_datasets.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10252 2023-07-30 20:06:57.000000 deepchem-2.7.2.dev20230730200710/deepchem/molnet/load_function/chembl_tasks.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2625 2023-07-30 20:06:57.000000 deepchem-2.7.2.dev20230730200710/deepchem/molnet/load_function/clearance_datasets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4245 2023-07-30 20:06:57.000000 deepchem-2.7.2.dev20230730200710/deepchem/molnet/load_function/clintox_datasets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3507 2023-07-30 20:06:57.000000 deepchem-2.7.2.dev20230730200710/deepchem/molnet/load_function/delaney_datasets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6957 2023-07-30 20:06:57.000000 deepchem-2.7.2.dev20230730200710/deepchem/molnet/load_function/factors_datasets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3523 2023-07-30 20:06:57.000000 deepchem-2.7.2.dev20230730200710/deepchem/molnet/load_function/freesolv_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3496 2023-07-30 20:06:57.000000 deepchem-2.7.2.dev20230730200710/deepchem/molnet/load_function/hiv_datasets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3437 2023-07-30 20:06:57.000000 deepchem-2.7.2.dev20230730200710/deepchem/molnet/load_function/hopv_datasets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2734 2023-07-30 20:06:57.000000 deepchem-2.7.2.dev20230730200710/deepchem/molnet/load_function/hppb_datasets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6379 2023-07-30 20:06:57.000000 deepchem-2.7.2.dev20230730200710/deepchem/molnet/load_function/kaggle_datasets.py
+-rw-r--r--   0 runner    (1001) docker     (123)   165414 2023-07-30 20:06:57.000000 deepchem-2.7.2.dev20230730200710/deepchem/molnet/load_function/kaggle_features.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8104 2023-07-30 20:06:57.000000 deepchem-2.7.2.dev20230730200710/deepchem/molnet/load_function/kinase_datasets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3318 2023-07-30 20:06:57.000000 deepchem-2.7.2.dev20230730200710/deepchem/molnet/load_function/lipo_datasets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9165 2023-07-30 20:06:57.000000 deepchem-2.7.2.dev20230730200710/deepchem/molnet/load_function/load_dataset_template.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 20:07:10.904470 deepchem-2.7.2.dev20230730200710/deepchem/molnet/load_function/material_datasets/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-30 20:06:57.000000 deepchem-2.7.2.dev20230730200710/deepchem/molnet/load_function/material_datasets/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4705 2023-07-30 20:06:57.000000 deepchem-2.7.2.dev20230730200710/deepchem/molnet/load_function/material_datasets/load_Pt_NO_surface_adsorbate_energy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4474 2023-07-30 20:06:57.000000 deepchem-2.7.2.dev20230730200710/deepchem/molnet/load_function/material_datasets/load_bandgap.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4646 2023-07-30 20:06:57.000000 deepchem-2.7.2.dev20230730200710/deepchem/molnet/load_function/material_datasets/load_mp_formation_energy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4589 2023-07-30 20:06:57.000000 deepchem-2.7.2.dev20230730200710/deepchem/molnet/load_function/material_datasets/load_mp_metallicity.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4516 2023-07-30 20:06:57.000000 deepchem-2.7.2.dev20230730200710/deepchem/molnet/load_function/material_datasets/load_perovskite.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8680 2023-07-30 20:06:57.000000 deepchem-2.7.2.dev20230730200710/deepchem/molnet/load_function/molnet_loader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3631 2023-07-30 20:06:57.000000 deepchem-2.7.2.dev20230730200710/deepchem/molnet/load_function/muv_datasets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3290 2023-07-30 20:06:57.000000 deepchem-2.7.2.dev20230730200710/deepchem/molnet/load_function/nci_datasets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6927 2023-07-30 20:06:57.000000 deepchem-2.7.2.dev20230730200710/deepchem/molnet/load_function/pcba_datasets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8586 2023-07-30 20:06:57.000000 deepchem-2.7.2.dev20230730200710/deepchem/molnet/load_function/pdbbind_datasets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2549 2023-07-30 20:06:57.000000 deepchem-2.7.2.dev20230730200710/deepchem/molnet/load_function/ppb_datasets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4800 2023-07-30 20:06:57.000000 deepchem-2.7.2.dev20230730200710/deepchem/molnet/load_function/qm7_datasets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5045 2023-07-30 20:06:57.000000 deepchem-2.7.2.dev20230730200710/deepchem/molnet/load_function/qm8_datasets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5697 2023-07-30 20:06:57.000000 deepchem-2.7.2.dev20230730200710/deepchem/molnet/load_function/qm9_datasets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3567 2023-07-30 20:06:57.000000 deepchem-2.7.2.dev20230730200710/deepchem/molnet/load_function/sampl_datasets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4640 2023-07-30 20:06:57.000000 deepchem-2.7.2.dev20230730200710/deepchem/molnet/load_function/sider_datasets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3140 2023-07-30 20:06:57.000000 deepchem-2.7.2.dev20230730200710/deepchem/molnet/load_function/sweetlead_datasets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2687 2023-07-30 20:06:57.000000 deepchem-2.7.2.dev20230730200710/deepchem/molnet/load_function/thermosol_datasets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3530 2023-07-30 20:06:57.000000 deepchem-2.7.2.dev20230730200710/deepchem/molnet/load_function/tox21_datasets.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18900 2023-07-30 20:06:57.000000 deepchem-2.7.2.dev20230730200710/deepchem/molnet/load_function/toxcast_datasets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7662 2023-07-30 20:06:57.000000 deepchem-2.7.2.dev20230730200710/deepchem/molnet/load_function/uspto_datasets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6623 2023-07-30 20:06:57.000000 deepchem-2.7.2.dev20230730200710/deepchem/molnet/load_function/uv_datasets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2036 2023-07-30 20:06:57.000000 deepchem-2.7.2.dev20230730200710/deepchem/molnet/load_function/uv_tasks.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6895 2023-07-30 20:06:57.000000 deepchem-2.7.2.dev20230730200710/deepchem/molnet/load_function/zinc15_datasets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5319 2023-07-30 20:06:57.000000 deepchem-2.7.2.dev20230730200710/deepchem/molnet/preset_hyper_parameters.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13549 2023-07-30 20:06:57.000000 deepchem-2.7.2.dev20230730200710/deepchem/molnet/run_benchmark.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4874 2023-07-30 20:06:57.000000 deepchem-2.7.2.dev20230730200710/deepchem/molnet/run_benchmark_low_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)    36564 2023-07-30 20:06:57.000000 deepchem-2.7.2.dev20230730200710/deepchem/molnet/run_benchmark_models.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 20:07:10.904470 deepchem-2.7.2.dev20230730200710/deepchem/rl/
+-rw-r--r--   0 runner    (1001) docker     (123)     9312 2023-07-30 20:06:57.000000 deepchem-2.7.2.dev20230730200710/deepchem/rl/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23102 2023-07-30 20:06:57.000000 deepchem-2.7.2.dev20230730200710/deepchem/rl/a2c.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 20:07:10.904470 deepchem-2.7.2.dev20230730200710/deepchem/rl/envs/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-30 20:06:57.000000 deepchem-2.7.2.dev20230730200710/deepchem/rl/envs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1773 2023-07-30 20:06:57.000000 deepchem-2.7.2.dev20230730200710/deepchem/rl/envs/test_tictactoe.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3632 2023-07-30 20:06:57.000000 deepchem-2.7.2.dev20230730200710/deepchem/rl/envs/tictactoe.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25262 2023-07-30 20:06:57.000000 deepchem-2.7.2.dev20230730200710/deepchem/rl/ppo.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 20:07:10.908470 deepchem-2.7.2.dev20230730200710/deepchem/splits/
+-rw-r--r--   0 runner    (1001) docker     (123)     1384 2023-07-30 20:06:57.000000 deepchem-2.7.2.dev20230730200710/deepchem/splits/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    63895 2023-07-30 20:06:57.000000 deepchem-2.7.2.dev20230730200710/deepchem/splits/splitters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4017 2023-07-30 20:06:57.000000 deepchem-2.7.2.dev20230730200710/deepchem/splits/task_splitter.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 20:07:10.908470 deepchem-2.7.2.dev20230730200710/deepchem/trans/
+-rw-r--r--   0 runner    (1001) docker     (123)     1255 2023-07-30 20:06:57.000000 deepchem-2.7.2.dev20230730200710/deepchem/trans/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6571 2023-07-30 20:06:57.000000 deepchem-2.7.2.dev20230730200710/deepchem/trans/duplicate.py
+-rw-r--r--   0 runner    (1001) docker     (123)    91191 2023-07-30 20:06:57.000000 deepchem-2.7.2.dev20230730200710/deepchem/trans/transformers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 20:07:10.920470 deepchem-2.7.2.dev20230730200710/deepchem/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)     6141 2023-07-30 20:06:57.000000 deepchem-2.7.2.dev20230730200710/deepchem/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10069 2023-07-30 20:06:57.000000 deepchem-2.7.2.dev20230730200710/deepchem/utils/conformers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13294 2023-07-30 20:06:57.000000 deepchem-2.7.2.dev20230730200710/deepchem/utils/coordinate_box_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20923 2023-07-30 20:06:57.000000 deepchem-2.7.2.dev20230730200710/deepchem/utils/data_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1840 2023-07-30 20:06:57.000000 deepchem-2.7.2.dev20230730200710/deepchem/utils/debug_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3041 2023-07-30 20:06:57.000000 deepchem-2.7.2.dev20230730200710/deepchem/utils/dftutils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10476 2023-07-30 20:06:57.000000 deepchem-2.7.2.dev20230730200710/deepchem/utils/docking_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14881 2023-07-30 20:06:57.000000 deepchem-2.7.2.dev20230730200710/deepchem/utils/electron_sampler.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19454 2023-07-30 20:06:57.000000 deepchem-2.7.2.dev20230730200710/deepchem/utils/evaluate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6134 2023-07-30 20:06:57.000000 deepchem-2.7.2.dev20230730200710/deepchem/utils/fake_data_generator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13312 2023-07-30 20:06:57.000000 deepchem-2.7.2.dev20230730200710/deepchem/utils/fragment_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3903 2023-07-30 20:06:57.000000 deepchem-2.7.2.dev20230730200710/deepchem/utils/genomics_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8259 2023-07-30 20:06:57.000000 deepchem-2.7.2.dev20230730200710/deepchem/utils/geometry_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6033 2023-07-30 20:06:57.000000 deepchem-2.7.2.dev20230730200710/deepchem/utils/graph_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6554 2023-07-30 20:06:57.000000 deepchem-2.7.2.dev20230730200710/deepchem/utils/grover.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3644 2023-07-30 20:06:57.000000 deepchem-2.7.2.dev20230730200710/deepchem/utils/hash_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19262 2023-07-30 20:06:57.000000 deepchem-2.7.2.dev20230730200710/deepchem/utils/molecule_feature_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17713 2023-07-30 20:06:57.000000 deepchem-2.7.2.dev20230730200710/deepchem/utils/noncovalent_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11749 2023-07-30 20:06:57.000000 deepchem-2.7.2.dev20230730200710/deepchem/utils/pdbqt_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4341 2023-07-30 20:06:57.000000 deepchem-2.7.2.dev20230730200710/deepchem/utils/pytorch_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    65672 2023-07-30 20:06:57.000000 deepchem-2.7.2.dev20230730200710/deepchem/utils/rdkit_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      552 2023-07-30 20:06:57.000000 deepchem-2.7.2.dev20230730200710/deepchem/utils/save.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6815 2023-07-30 20:06:57.000000 deepchem-2.7.2.dev20230730200710/deepchem/utils/sequence_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 20:07:10.932470 deepchem-2.7.2.dev20230730200710/deepchem/utils/test/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-30 20:06:57.000000 deepchem-2.7.2.dev20230730200710/deepchem/utils/test/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6598 2023-07-30 20:06:57.000000 deepchem-2.7.2.dev20230730200710/deepchem/utils/test/test_coordinate_box_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      788 2023-07-30 20:06:57.000000 deepchem-2.7.2.dev20230730200710/deepchem/utils/test/test_data_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      896 2023-07-30 20:06:57.000000 deepchem-2.7.2.dev20230730200710/deepchem/utils/test/test_dftutils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2258 2023-07-30 20:06:57.000000 deepchem-2.7.2.dev20230730200710/deepchem/utils/test/test_docking_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3522 2023-07-30 20:06:57.000000 deepchem-2.7.2.dev20230730200710/deepchem/utils/test/test_electron_sampler.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12977 2023-07-30 20:06:57.000000 deepchem-2.7.2.dev20230730200710/deepchem/utils/test/test_evaluate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2481 2023-07-30 20:06:57.000000 deepchem-2.7.2.dev20230730200710/deepchem/utils/test/test_fake_data_generator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2610 2023-07-30 20:06:57.000000 deepchem-2.7.2.dev20230730200710/deepchem/utils/test/test_fragment_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4684 2023-07-30 20:06:57.000000 deepchem-2.7.2.dev20230730200710/deepchem/utils/test/test_generator_evaluator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1956 2023-07-30 20:06:57.000000 deepchem-2.7.2.dev20230730200710/deepchem/utils/test/test_genomics_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3296 2023-07-30 20:06:57.000000 deepchem-2.7.2.dev20230730200710/deepchem/utils/test/test_geometry_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      866 2023-07-30 20:06:57.000000 deepchem-2.7.2.dev20230730200710/deepchem/utils/test/test_graph_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1523 2023-07-30 20:06:57.000000 deepchem-2.7.2.dev20230730200710/deepchem/utils/test/test_grover.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1476 2023-07-30 20:06:57.000000 deepchem-2.7.2.dev20230730200710/deepchem/utils/test/test_hash_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9115 2023-07-30 20:06:57.000000 deepchem-2.7.2.dev20230730200710/deepchem/utils/test/test_molecule_feature_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6251 2023-07-30 20:06:57.000000 deepchem-2.7.2.dev20230730200710/deepchem/utils/test/test_noncovalent_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3922 2023-07-30 20:06:57.000000 deepchem-2.7.2.dev20230730200710/deepchem/utils/test/test_pdbqt_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1577 2023-07-30 20:06:57.000000 deepchem-2.7.2.dev20230730200710/deepchem/utils/test/test_pytorch_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9005 2023-07-30 20:06:57.000000 deepchem-2.7.2.dev20230730200710/deepchem/utils/test/test_rdkit_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2388 2023-07-30 20:06:57.000000 deepchem-2.7.2.dev20230730200710/deepchem/utils/test/test_sequence_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      386 2023-07-30 20:06:57.000000 deepchem-2.7.2.dev20230730200710/deepchem/utils/test/test_updated_scipy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2859 2023-07-30 20:06:57.000000 deepchem-2.7.2.dev20230730200710/deepchem/utils/test/test_voxel_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      919 2023-07-30 20:06:57.000000 deepchem-2.7.2.dev20230730200710/deepchem/utils/typing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1113 2023-07-30 20:06:57.000000 deepchem-2.7.2.dev20230730200710/deepchem/utils/vina_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7797 2023-07-30 20:06:57.000000 deepchem-2.7.2.dev20230730200710/deepchem/utils/voxel_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 20:07:10.840470 deepchem-2.7.2.dev20230730200710/deepchem.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-07-30 20:07:10.000000 deepchem-2.7.2.dev20230730200710/deepchem.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    10767 2023-07-30 20:07:10.000000 deepchem-2.7.2.dev20230730200710/deepchem.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-30 20:07:10.000000 deepchem-2.7.2.dev20230730200710/deepchem.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      249 2023-07-30 20:07:10.000000 deepchem-2.7.2.dev20230730200710/deepchem.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-30 20:07:10.000000 deepchem-2.7.2.dev20230730200710/deepchem.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      701 2023-07-30 20:07:10.936470 deepchem-2.7.2.dev20230730200710/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2670 2023-07-30 20:06:57.000000 deepchem-2.7.2.dev20230730200710/setup.py
```

### Comparing `deepchem-2.7.2.dev20230728002356/LICENSE` & `deepchem-2.7.2.dev20230730200710/LICENSE`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230728002356/PKG-INFO` & `deepchem-2.7.2.dev20230730200710/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: deepchem
-Version: 2.7.2.dev20230728002356
+Version: 2.7.2.dev20230730200710
 Summary: Deep learning models for drug discovery,         quantum chemistry, and the life sciences.
 Home-page: https://github.com/deepchem/deepchem
 Maintainer: DeepChem contributors
 License: MIT
 Project-URL: Documentation, https://deepchem.readthedocs.io/en/latest/
 Project-URL: Source, https://github.com/deepchem/deepchem
 Keywords: deepchem,chemistry,biology,materials-science,life-science,drug-discovery
```

### Comparing `deepchem-2.7.2.dev20230728002356/README.md` & `deepchem-2.7.2.dev20230730200710/README.md`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230728002356/deepchem/data/__init__.py` & `deepchem-2.7.2.dev20230730200710/deepchem/data/__init__.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230728002356/deepchem/data/data_loader.py` & `deepchem-2.7.2.dev20230730200710/deepchem/data/data_loader.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230728002356/deepchem/data/datasets.py` & `deepchem-2.7.2.dev20230730200710/deepchem/data/datasets.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230728002356/deepchem/data/pytorch_datasets.py` & `deepchem-2.7.2.dev20230730200710/deepchem/data/pytorch_datasets.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230728002356/deepchem/data/supports.py` & `deepchem-2.7.2.dev20230730200710/deepchem/data/supports.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230728002356/deepchem/dock/binding_pocket.py` & `deepchem-2.7.2.dev20230730200710/deepchem/dock/binding_pocket.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230728002356/deepchem/dock/docking.py` & `deepchem-2.7.2.dev20230730200710/deepchem/dock/docking.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230728002356/deepchem/dock/pose_generation.py` & `deepchem-2.7.2.dev20230730200710/deepchem/dock/pose_generation.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230728002356/deepchem/dock/pose_scoring.py` & `deepchem-2.7.2.dev20230730200710/deepchem/dock/pose_scoring.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230728002356/deepchem/feat/__init__.py` & `deepchem-2.7.2.dev20230730200710/deepchem/feat/__init__.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230728002356/deepchem/feat/atomic_conformation.py` & `deepchem-2.7.2.dev20230730200710/deepchem/feat/atomic_conformation.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230728002356/deepchem/feat/base_classes.py` & `deepchem-2.7.2.dev20230730200710/deepchem/feat/base_classes.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230728002356/deepchem/feat/bert_tokenizer.py` & `deepchem-2.7.2.dev20230730200710/deepchem/feat/bert_tokenizer.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230728002356/deepchem/feat/binding_pocket_features.py` & `deepchem-2.7.2.dev20230730200710/deepchem/feat/binding_pocket_features.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230728002356/deepchem/feat/complex_featurizers/__init__.py` & `deepchem-2.7.2.dev20230730200710/deepchem/feat/complex_featurizers/__init__.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230728002356/deepchem/feat/complex_featurizers/complex_atomic_coordinates.py` & `deepchem-2.7.2.dev20230730200710/deepchem/feat/complex_featurizers/complex_atomic_coordinates.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230728002356/deepchem/feat/complex_featurizers/contact_fingerprints.py` & `deepchem-2.7.2.dev20230730200710/deepchem/feat/complex_featurizers/contact_fingerprints.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230728002356/deepchem/feat/complex_featurizers/grid_featurizers.py` & `deepchem-2.7.2.dev20230730200710/deepchem/feat/complex_featurizers/grid_featurizers.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230728002356/deepchem/feat/complex_featurizers/rdkit_grid_featurizer.py` & `deepchem-2.7.2.dev20230730200710/deepchem/feat/complex_featurizers/rdkit_grid_featurizer.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230728002356/deepchem/feat/complex_featurizers/splif_fingerprints.py` & `deepchem-2.7.2.dev20230730200710/deepchem/feat/complex_featurizers/splif_fingerprints.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230728002356/deepchem/feat/dft_data.py` & `deepchem-2.7.2.dev20230730200710/deepchem/feat/dft_data.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230728002356/deepchem/feat/graph_data.py` & `deepchem-2.7.2.dev20230730200710/deepchem/feat/graph_data.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230728002356/deepchem/feat/graph_features.py` & `deepchem-2.7.2.dev20230730200710/deepchem/feat/graph_features.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230728002356/deepchem/feat/huggingface_featurizer.py` & `deepchem-2.7.2.dev20230730200710/deepchem/feat/huggingface_featurizer.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230728002356/deepchem/feat/material_featurizers/cgcnn_featurizer.py` & `deepchem-2.7.2.dev20230730200710/deepchem/feat/material_featurizers/cgcnn_featurizer.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230728002356/deepchem/feat/material_featurizers/element_property_fingerprint.py` & `deepchem-2.7.2.dev20230730200710/deepchem/feat/material_featurizers/element_property_fingerprint.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230728002356/deepchem/feat/material_featurizers/elemnet_featurizer.py` & `deepchem-2.7.2.dev20230730200710/deepchem/feat/material_featurizers/elemnet_featurizer.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230728002356/deepchem/feat/material_featurizers/lcnn_featurizer.py` & `deepchem-2.7.2.dev20230730200710/deepchem/feat/material_featurizers/lcnn_featurizer.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230728002356/deepchem/feat/material_featurizers/sine_coulomb_matrix.py` & `deepchem-2.7.2.dev20230730200710/deepchem/feat/material_featurizers/sine_coulomb_matrix.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230728002356/deepchem/feat/mol_graphs.py` & `deepchem-2.7.2.dev20230730200710/deepchem/feat/mol_graphs.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230728002356/deepchem/feat/molecule_featurizers/__init__.py` & `deepchem-2.7.2.dev20230730200710/deepchem/feat/molecule_featurizers/__init__.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230728002356/deepchem/feat/molecule_featurizers/atomic_coordinates.py` & `deepchem-2.7.2.dev20230730200710/deepchem/feat/molecule_featurizers/atomic_coordinates.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230728002356/deepchem/feat/molecule_featurizers/bp_symmetry_function_input.py` & `deepchem-2.7.2.dev20230730200710/deepchem/feat/molecule_featurizers/bp_symmetry_function_input.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230728002356/deepchem/feat/molecule_featurizers/circular_fingerprint.py` & `deepchem-2.7.2.dev20230730200710/deepchem/feat/molecule_featurizers/circular_fingerprint.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230728002356/deepchem/feat/molecule_featurizers/conformer_featurizer.py` & `deepchem-2.7.2.dev20230730200710/deepchem/feat/molecule_featurizers/conformer_featurizer.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230728002356/deepchem/feat/molecule_featurizers/coulomb_matrices.py` & `deepchem-2.7.2.dev20230730200710/deepchem/feat/molecule_featurizers/coulomb_matrices.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230728002356/deepchem/feat/molecule_featurizers/dmpnn_featurizer.py` & `deepchem-2.7.2.dev20230730200710/deepchem/feat/molecule_featurizers/dmpnn_featurizer.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230728002356/deepchem/feat/molecule_featurizers/grover_featurizer.py` & `deepchem-2.7.2.dev20230730200710/deepchem/feat/molecule_featurizers/grover_featurizer.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230728002356/deepchem/feat/molecule_featurizers/maccs_keys_fingerprint.py` & `deepchem-2.7.2.dev20230730200710/deepchem/feat/molecule_featurizers/maccs_keys_fingerprint.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230728002356/deepchem/feat/molecule_featurizers/mat_featurizer.py` & `deepchem-2.7.2.dev20230730200710/deepchem/feat/molecule_featurizers/mat_featurizer.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230728002356/deepchem/feat/molecule_featurizers/mol2vec_fingerprint.py` & `deepchem-2.7.2.dev20230730200710/deepchem/feat/molecule_featurizers/mol2vec_fingerprint.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230728002356/deepchem/feat/molecule_featurizers/mol_graph_conv_featurizer.py` & `deepchem-2.7.2.dev20230730200710/deepchem/feat/molecule_featurizers/mol_graph_conv_featurizer.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230728002356/deepchem/feat/molecule_featurizers/molgan_featurizer.py` & `deepchem-2.7.2.dev20230730200710/deepchem/feat/molecule_featurizers/molgan_featurizer.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230728002356/deepchem/feat/molecule_featurizers/mordred_descriptors.py` & `deepchem-2.7.2.dev20230730200710/deepchem/feat/molecule_featurizers/mordred_descriptors.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230728002356/deepchem/feat/molecule_featurizers/mxmnet_featurizer.py` & `deepchem-2.7.2.dev20230730200710/deepchem/feat/molecule_featurizers/mxmnet_featurizer.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230728002356/deepchem/feat/molecule_featurizers/one_hot_featurizer.py` & `deepchem-2.7.2.dev20230730200710/deepchem/feat/molecule_featurizers/one_hot_featurizer.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230728002356/deepchem/feat/molecule_featurizers/pubchem_fingerprint.py` & `deepchem-2.7.2.dev20230730200710/deepchem/feat/molecule_featurizers/pubchem_fingerprint.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230728002356/deepchem/feat/molecule_featurizers/raw_featurizer.py` & `deepchem-2.7.2.dev20230730200710/deepchem/feat/molecule_featurizers/raw_featurizer.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230728002356/deepchem/feat/molecule_featurizers/rdkit_descriptors.py` & `deepchem-2.7.2.dev20230730200710/deepchem/feat/molecule_featurizers/rdkit_descriptors.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230728002356/deepchem/feat/molecule_featurizers/smiles_to_image.py` & `deepchem-2.7.2.dev20230730200710/deepchem/feat/molecule_featurizers/smiles_to_image.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230728002356/deepchem/feat/molecule_featurizers/smiles_to_seq.py` & `deepchem-2.7.2.dev20230730200710/deepchem/feat/molecule_featurizers/smiles_to_seq.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230728002356/deepchem/feat/molecule_featurizers/snap_featurizer.py` & `deepchem-2.7.2.dev20230730200710/deepchem/feat/molecule_featurizers/snap_featurizer.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230728002356/deepchem/feat/molecule_featurizers/sparse_matrix_one_hot_featurizer.py` & `deepchem-2.7.2.dev20230730200710/deepchem/feat/molecule_featurizers/sparse_matrix_one_hot_featurizer.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230728002356/deepchem/feat/reaction_featurizer.py` & `deepchem-2.7.2.dev20230730200710/deepchem/feat/reaction_featurizer.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230728002356/deepchem/feat/roberta_tokenizer.py` & `deepchem-2.7.2.dev20230730200710/deepchem/feat/roberta_tokenizer.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230728002356/deepchem/feat/sequence_featurizers/position_frequency_matrix_featurizer.py` & `deepchem-2.7.2.dev20230730200710/deepchem/feat/sequence_featurizers/position_frequency_matrix_featurizer.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230728002356/deepchem/feat/smiles_tokenizer.py` & `deepchem-2.7.2.dev20230730200710/deepchem/feat/smiles_tokenizer.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230728002356/deepchem/feat/vocabulary_builders/grover_vocab.py` & `deepchem-2.7.2.dev20230730200710/deepchem/feat/vocabulary_builders/grover_vocab.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230728002356/deepchem/feat/vocabulary_builders/hf_vocab.py` & `deepchem-2.7.2.dev20230730200710/deepchem/feat/vocabulary_builders/hf_vocab.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230728002356/deepchem/feat/vocabulary_builders/vocabulary_builder.py` & `deepchem-2.7.2.dev20230730200710/deepchem/feat/vocabulary_builders/vocabulary_builder.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230728002356/deepchem/hyper/base_classes.py` & `deepchem-2.7.2.dev20230730200710/deepchem/hyper/base_classes.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230728002356/deepchem/hyper/gaussian_process.py` & `deepchem-2.7.2.dev20230730200710/deepchem/hyper/gaussian_process.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230728002356/deepchem/hyper/grid_search.py` & `deepchem-2.7.2.dev20230730200710/deepchem/hyper/grid_search.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230728002356/deepchem/hyper/random_search.py` & `deepchem-2.7.2.dev20230730200710/deepchem/hyper/random_search.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230728002356/deepchem/metalearning/maml.py` & `deepchem-2.7.2.dev20230730200710/deepchem/metalearning/maml.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230728002356/deepchem/metrics/__init__.py` & `deepchem-2.7.2.dev20230730200710/deepchem/metrics/__init__.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230728002356/deepchem/metrics/genomic_metrics.py` & `deepchem-2.7.2.dev20230730200710/deepchem/metrics/genomic_metrics.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230728002356/deepchem/metrics/metric.py` & `deepchem-2.7.2.dev20230730200710/deepchem/metrics/metric.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230728002356/deepchem/metrics/score_function.py` & `deepchem-2.7.2.dev20230730200710/deepchem/metrics/score_function.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230728002356/deepchem/models/IRV.py` & `deepchem-2.7.2.dev20230730200710/deepchem/models/IRV.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230728002356/deepchem/models/__init__.py` & `deepchem-2.7.2.dev20230730200710/deepchem/models/__init__.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230728002356/deepchem/models/atomic_conv.py` & `deepchem-2.7.2.dev20230730200710/deepchem/models/atomic_conv.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230728002356/deepchem/models/callbacks.py` & `deepchem-2.7.2.dev20230730200710/deepchem/models/callbacks.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230728002356/deepchem/models/chemnet_layers.py` & `deepchem-2.7.2.dev20230730200710/deepchem/models/chemnet_layers.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230728002356/deepchem/models/chemnet_models.py` & `deepchem-2.7.2.dev20230730200710/deepchem/models/chemnet_models.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230728002356/deepchem/models/dft/dftxc.py` & `deepchem-2.7.2.dev20230730200710/deepchem/models/dft/dftxc.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230728002356/deepchem/models/dft/nnxc.py` & `deepchem-2.7.2.dev20230730200710/deepchem/models/dft/nnxc.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230728002356/deepchem/models/dft/scf.py` & `deepchem-2.7.2.dev20230730200710/deepchem/models/dft/scf.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230728002356/deepchem/models/fcnet.py` & `deepchem-2.7.2.dev20230730200710/deepchem/models/fcnet.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230728002356/deepchem/models/gan.py` & `deepchem-2.7.2.dev20230730200710/deepchem/models/gan.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230728002356/deepchem/models/gbdt_models/gbdt_model.py` & `deepchem-2.7.2.dev20230730200710/deepchem/models/gbdt_models/gbdt_model.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230728002356/deepchem/models/graph_models.py` & `deepchem-2.7.2.dev20230730200710/deepchem/models/graph_models.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230728002356/deepchem/models/jax_models/jax_model.py` & `deepchem-2.7.2.dev20230730200710/deepchem/models/jax_models/jax_model.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230728002356/deepchem/models/jax_models/layers.py` & `deepchem-2.7.2.dev20230730200710/deepchem/models/jax_models/layers.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230728002356/deepchem/models/jax_models/pinns_model.py` & `deepchem-2.7.2.dev20230730200710/deepchem/models/jax_models/pinns_model.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230728002356/deepchem/models/keras_model.py` & `deepchem-2.7.2.dev20230730200710/deepchem/models/keras_model.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230728002356/deepchem/models/layers.py` & `deepchem-2.7.2.dev20230730200710/deepchem/models/layers.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230728002356/deepchem/models/lightning/dc_lightning_dataset_module.py` & `deepchem-2.7.2.dev20230730200710/deepchem/models/lightning/dc_lightning_dataset_module.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230728002356/deepchem/models/lightning/dc_lightning_module.py` & `deepchem-2.7.2.dev20230730200710/deepchem/models/lightning/dc_lightning_module.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230728002356/deepchem/models/losses.py` & `deepchem-2.7.2.dev20230730200710/deepchem/models/losses.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230728002356/deepchem/models/models.py` & `deepchem-2.7.2.dev20230730200710/deepchem/models/models.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230728002356/deepchem/models/molgan.py` & `deepchem-2.7.2.dev20230730200710/deepchem/models/molgan.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230728002356/deepchem/models/multitask.py` & `deepchem-2.7.2.dev20230730200710/deepchem/models/multitask.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230728002356/deepchem/models/normalizing_flows.py` & `deepchem-2.7.2.dev20230730200710/deepchem/models/normalizing_flows.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230728002356/deepchem/models/optimizers.py` & `deepchem-2.7.2.dev20230730200710/deepchem/models/optimizers.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230728002356/deepchem/models/progressive_multitask.py` & `deepchem-2.7.2.dev20230730200710/deepchem/models/progressive_multitask.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230728002356/deepchem/models/robust_multitask.py` & `deepchem-2.7.2.dev20230730200710/deepchem/models/robust_multitask.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230728002356/deepchem/models/scscore.py` & `deepchem-2.7.2.dev20230730200710/deepchem/models/scscore.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230728002356/deepchem/models/seqtoseq.py` & `deepchem-2.7.2.dev20230730200710/deepchem/models/seqtoseq.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230728002356/deepchem/models/sklearn_models/sklearn_model.py` & `deepchem-2.7.2.dev20230730200710/deepchem/models/sklearn_models/sklearn_model.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230728002356/deepchem/models/text_cnn.py` & `deepchem-2.7.2.dev20230730200710/deepchem/models/text_cnn.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230728002356/deepchem/models/torch_models/__init__.py` & `deepchem-2.7.2.dev20230730200710/deepchem/models/torch_models/__init__.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230728002356/deepchem/models/torch_models/attention.py` & `deepchem-2.7.2.dev20230730200710/deepchem/models/torch_models/attention.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230728002356/deepchem/models/torch_models/attentivefp.py` & `deepchem-2.7.2.dev20230730200710/deepchem/models/torch_models/attentivefp.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230728002356/deepchem/models/torch_models/cgcnn.py` & `deepchem-2.7.2.dev20230730200710/deepchem/models/torch_models/cgcnn.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230728002356/deepchem/models/torch_models/chemberta.py` & `deepchem-2.7.2.dev20230730200710/deepchem/models/torch_models/chemberta.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230728002356/deepchem/models/torch_models/cnn.py` & `deepchem-2.7.2.dev20230730200710/deepchem/models/torch_models/cnn.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230728002356/deepchem/models/torch_models/dmpnn.py` & `deepchem-2.7.2.dev20230730200710/deepchem/models/torch_models/dmpnn.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230728002356/deepchem/models/torch_models/ferminet.py` & `deepchem-2.7.2.dev20230730200710/deepchem/models/torch_models/ferminet.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230728002356/deepchem/models/torch_models/gat.py` & `deepchem-2.7.2.dev20230730200710/deepchem/models/torch_models/gat.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230728002356/deepchem/models/torch_models/gcn.py` & `deepchem-2.7.2.dev20230730200710/deepchem/models/torch_models/gcn.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230728002356/deepchem/models/torch_models/gnn.py` & `deepchem-2.7.2.dev20230730200710/deepchem/models/torch_models/gnn.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230728002356/deepchem/models/torch_models/gnn3d.py` & `deepchem-2.7.2.dev20230730200710/deepchem/models/torch_models/gnn3d.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230728002356/deepchem/models/torch_models/grover.py` & `deepchem-2.7.2.dev20230730200710/deepchem/models/torch_models/grover.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230728002356/deepchem/models/torch_models/grover_layers.py` & `deepchem-2.7.2.dev20230730200710/deepchem/models/torch_models/grover_layers.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230728002356/deepchem/models/torch_models/hf_models.py` & `deepchem-2.7.2.dev20230730200710/deepchem/models/torch_models/hf_models.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230728002356/deepchem/models/torch_models/infograph.py` & `deepchem-2.7.2.dev20230730200710/deepchem/models/torch_models/infograph.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230728002356/deepchem/models/torch_models/kfac_optimizer.py` & `deepchem-2.7.2.dev20230730200710/deepchem/models/torch_models/kfac_optimizer.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230728002356/deepchem/models/torch_models/layers.py` & `deepchem-2.7.2.dev20230730200710/deepchem/models/torch_models/layers.py`

 * *Files 1% similar despite different names*

```diff
@@ -10767,8 +10767,133 @@
 0002a0e0: 206f 7574 7075 7420 2f20 746f 7263 682e   output / torch.
 0002a0f0: 7375 6d28 6f75 7470 7574 2c20 6469 6d3d  sum(output, dim=
 0002a100: 322c 206b 6565 7064 696d 3d54 7275 6529  2, keepdim=True)
 0002a110: 0a20 2020 2020 2020 206f 7574 7075 7420  .        output 
 0002a120: 3d20 6f75 7470 7574 2e76 6965 7728 2d31  = output.view(-1
 0002a130: 2c20 7365 6c66 2e6e 5f69 6e70 7574 202a  , self.n_input *
 0002a140: 2031 3129 0a20 2020 2020 2020 2072 6574   11).        ret
-0002a150: 7572 6e20 6f75 7470 7574 0a              urn output.
+0002a150: 7572 6e20 6f75 7470 7574 0a0a 0a63 6c61  urn output...cla
+0002a160: 7373 205f 4d58 4d4e 6574 456e 7665 6c6f  ss _MXMNetEnvelo
+0002a170: 7065 2874 6f72 6368 2e6e 6e2e 4d6f 6475  pe(torch.nn.Modu
+0002a180: 6c65 293a 0a20 2020 2022 2222 0a20 2020  le):.    """.   
+0002a190: 2041 2050 7954 6f72 6368 206d 6f64 756c   A PyTorch modul
+0002a1a0: 6520 696d 706c 656d 656e 7469 6e67 2061  e implementing a
+0002a1b0: 6e20 656e 7665 6c6f 7065 2066 756e 6374  n envelope funct
+0002a1c0: 696f 6e2e 2054 6869 7320 6973 2061 2068  ion. This is a h
+0002a1d0: 656c 7065 7220 636c 6173 7320 666f 7220  elper class for 
+0002a1e0: 4d58 4d4e 6574 5370 6865 7269 6361 6c42  MXMNetSphericalB
+0002a1f0: 6173 6973 4c61 7965 7220 616e 6420 4d58  asisLayer and MX
+0002a200: 4d4e 6574 4265 7373 656c 4261 7369 734c  MNetBesselBasisL
+0002a210: 6179 6572 2074 6f20 6265 2075 7365 6420  ayer to be used 
+0002a220: 696e 204d 584d 4e65 7420 4d6f 6465 6c2e  in MXMNet Model.
+0002a230: 0a0a 2020 2020 5468 6520 656e 7665 6c6f  ..    The envelo
+0002a240: 7065 2066 756e 6374 696f 6e20 6973 2064  pe function is d
+0002a250: 6566 696e 6564 2061 7320 666f 6c6c 6f77  efined as follow
+0002a260: 733a 0a20 2020 2065 6e76 2878 2920 3d20  s:.    env(x) = 
+0002a270: 3120 2f20 7820 2b20 6120 2a20 785e 6520  1 / x + a * x^e 
+0002a280: 2b20 6220 2a20 785e 2865 2b31 2920 2b20  + b * x^(e+1) + 
+0002a290: 6320 2a20 785e 2865 2b32 2920 2020 2020  c * x^(e+2)     
+0002a2a0: 2020 2069 6620 7820 3c20 310a 2020 2020     if x < 1.    
+0002a2b0: 656e 7628 7829 203d 2030 2020 2020 2020  env(x) = 0      
+0002a2c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0002a2d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0002a2e0: 2020 2020 2020 2020 2020 2020 6966 2078              if x
+0002a2f0: 203e 3d20 310a 0a20 2020 2077 6865 7265   >= 1..    where
+0002a300: 200a 2020 2020 2778 2720 6973 2074 6865   .    'x' is the
+0002a310: 2069 6e70 7574 2074 656e 736f 720a 2020   input tensor.  
+0002a320: 2020 2765 2720 6973 2074 6865 2065 7870    'e' is the exp
+0002a330: 6f6e 656e 7420 7061 7261 6d65 7465 720a  onent parameter.
+0002a340: 2020 2020 2761 2720 3d20 2d28 6520 2b20      'a' = -(e + 
+0002a350: 3129 202a 2028 6520 2b20 3229 202f 2032  1) * (e + 2) / 2
+0002a360: 0a20 2020 2027 6227 203d 2065 202a 2028  .    'b' = e * (
+0002a370: 6520 2b20 3229 0a20 2020 2027 6327 203d  e + 2).    'c' =
+0002a380: 202d 6520 2a20 2865 202b 2031 2920 2f20   -e * (e + 1) / 
+0002a390: 320a 0a20 2020 2045 7861 6d70 6c65 730a  2..    Examples.
+0002a3a0: 2020 2020 2d2d 2d2d 2d2d 2d2d 0a20 2020      --------.   
+0002a3b0: 203e 3e3e 2065 6e76 203d 205f 4d58 4d4e   >>> env = _MXMN
+0002a3c0: 6574 456e 7665 6c6f 7065 2865 7870 6f6e  etEnvelope(expon
+0002a3d0: 656e 743d 3229 0a20 2020 203e 3e3e 2069  ent=2).    >>> i
+0002a3e0: 6e70 7574 5f74 656e 736f 7220 3d20 746f  nput_tensor = to
+0002a3f0: 7263 682e 7465 6e73 6f72 285b 302e 352c  rch.tensor([0.5,
+0002a400: 2031 2e30 2c20 322e 302c 2033 2e30 5d29   1.0, 2.0, 3.0])
+0002a410: 0a20 2020 203e 3e3e 206f 7574 7075 7420  .    >>> output 
+0002a420: 3d20 656e 7628 696e 7075 745f 7465 6e73  = env(input_tens
+0002a430: 6f72 290a 2020 2020 3e3e 3e20 6f75 7470  or).    >>> outp
+0002a440: 7574 2e73 6861 7065 0a20 2020 2074 6f72  ut.shape.    tor
+0002a450: 6368 2e53 697a 6528 5b34 5d29 0a20 2020  ch.Size([4]).   
+0002a460: 2022 2222 0a0a 2020 2020 6465 6620 5f5f   """..    def __
+0002a470: 696e 6974 5f5f 2873 656c 662c 2065 7870  init__(self, exp
+0002a480: 6f6e 656e 743a 2069 6e74 293a 0a20 2020  onent: int):.   
+0002a490: 2020 2020 2022 2222 0a20 2020 2020 2020       """.       
+0002a4a0: 2050 6172 616d 6574 6572 730a 2020 2020   Parameters.    
+0002a4b0: 2020 2020 2d2d 2d2d 2d2d 2d2d 2d2d 0a20      ----------. 
+0002a4c0: 2020 2020 2020 2065 7870 6f6e 656e 743a         exponent:
+0002a4d0: 2066 6c6f 6174 200a 2020 2020 2020 2020   float .        
+0002a4e0: 2020 2020 5468 6520 6578 706f 6e65 6e74      The exponent
+0002a4f0: 2027 6527 2075 7365 6420 696e 2074 6865   'e' used in the
+0002a500: 2065 6e76 656c 6f70 6520 6675 6e63 7469   envelope functi
+0002a510: 6f6e 2e0a 2020 2020 2020 2020 2222 220a  on..        """.
+0002a520: 2020 2020 2020 2020 7375 7065 7228 5f4d          super(_M
+0002a530: 584d 4e65 7445 6e76 656c 6f70 652c 2073  XMNetEnvelope, s
+0002a540: 656c 6629 2e5f 5f69 6e69 745f 5f28 290a  elf).__init__().
+0002a550: 2020 2020 2020 2020 7365 6c66 2e65 3a20          self.e: 
+0002a560: 696e 7420 3d20 6578 706f 6e65 6e74 0a20  int = exponent. 
+0002a570: 2020 2020 2020 2073 656c 662e 613a 2066         self.a: f
+0002a580: 6c6f 6174 203d 202d 2873 656c 662e 6520  loat = -(self.e 
+0002a590: 2b20 3129 202a 2028 7365 6c66 2e65 202b  + 1) * (self.e +
+0002a5a0: 2032 2920 2f20 320a 2020 2020 2020 2020   2) / 2.        
+0002a5b0: 7365 6c66 2e62 3a20 666c 6f61 7420 3d20  self.b: float = 
+0002a5c0: 7365 6c66 2e65 202a 2028 7365 6c66 2e65  self.e * (self.e
+0002a5d0: 202b 2032 290a 2020 2020 2020 2020 7365   + 2).        se
+0002a5e0: 6c66 2e63 3a20 666c 6f61 7420 3d20 2d73  lf.c: float = -s
+0002a5f0: 656c 662e 6520 2a20 2873 656c 662e 6520  elf.e * (self.e 
+0002a600: 2b20 3129 202f 2032 0a0a 2020 2020 6465  + 1) / 2..    de
+0002a610: 6620 666f 7277 6172 6428 7365 6c66 2c20  f forward(self, 
+0002a620: 783a 2074 6f72 6368 2e54 656e 736f 7229  x: torch.Tensor)
+0002a630: 202d 3e20 746f 7263 682e 5465 6e73 6f72   -> torch.Tensor
+0002a640: 3a0a 2020 2020 2020 2020 2222 220a 2020  :.        """.  
+0002a650: 2020 2020 2020 436f 6d70 7574 6520 7468        Compute th
+0002a660: 6520 656e 7665 6c6f 7065 2066 756e 6374  e envelope funct
+0002a670: 696f 6e20 666f 7220 7468 6520 696e 7075  ion for the inpu
+0002a680: 7420 7465 6e73 6f72 2027 7827 2e0a 0a20  t tensor 'x'... 
+0002a690: 2020 2020 2020 2050 6172 616d 6574 6572         Parameter
+0002a6a0: 730a 2020 2020 2020 2020 2d2d 2d2d 2d2d  s.        ------
+0002a6b0: 2d2d 2d2d 0a20 2020 2020 2020 2078 3a20  ----.        x: 
+0002a6c0: 746f 7263 682e 5465 6e73 6f72 0a20 2020  torch.Tensor.   
+0002a6d0: 2020 2020 2020 2020 2054 6865 2049 6e70           The Inp
+0002a6e0: 7574 2074 656e 736f 720a 0a20 2020 2020  ut tensor..     
+0002a6f0: 2020 2052 6574 7572 6e73 0a20 2020 2020     Returns.     
+0002a700: 2020 202d 2d2d 2d2d 2d2d 0a20 2020 2020     -------.     
+0002a710: 2020 206f 7574 7075 743a 2074 6f72 6368     output: torch
+0002a720: 2e54 656e 736f 720a 2020 2020 2020 2020  .Tensor.        
+0002a730: 2020 2020 5468 6520 7465 6e73 6f72 2063      The tensor c
+0002a740: 6f6e 7461 696e 696e 6720 7468 6520 636f  ontaining the co
+0002a750: 6d70 7574 6564 2065 6e76 656c 6f70 6520  mputed envelope 
+0002a760: 7661 6c75 6573 2066 6f72 2065 6163 6820  values for each 
+0002a770: 656c 656d 656e 7420 6f66 2027 7827 2e0a  element of 'x'..
+0002a780: 2020 2020 2020 2020 2222 220a 2020 2020          """.    
+0002a790: 2020 2020 653a 2069 6e74 203d 2073 656c      e: int = sel
+0002a7a0: 662e 650a 2020 2020 2020 2020 613a 2066  f.e.        a: f
+0002a7b0: 6c6f 6174 203d 2073 656c 662e 610a 2020  loat = self.a.  
+0002a7c0: 2020 2020 2020 623a 2066 6c6f 6174 203d        b: float =
+0002a7d0: 2073 656c 662e 620a 2020 2020 2020 2020   self.b.        
+0002a7e0: 633a 2066 6c6f 6174 203d 2073 656c 662e  c: float = self.
+0002a7f0: 630a 0a20 2020 2020 2020 2078 5f70 6f77  c..        x_pow
+0002a800: 5f70 303a 2074 6f72 6368 2e54 656e 736f  _p0: torch.Tenso
+0002a810: 7220 3d20 782e 706f 7728 6529 0a20 2020  r = x.pow(e).   
+0002a820: 2020 2020 2078 5f70 6f77 5f70 313a 2074       x_pow_p1: t
+0002a830: 6f72 6368 2e54 656e 736f 7220 3d20 785f  orch.Tensor = x_
+0002a840: 706f 775f 7030 202a 2078 0a20 2020 2020  pow_p0 * x.     
+0002a850: 2020 2065 6e76 5f76 616c 3a20 746f 7263     env_val: torc
+0002a860: 682e 5465 6e73 6f72 203d 2031 2e20 2f20  h.Tensor = 1. / 
+0002a870: 7820 2b20 6120 2a20 785f 706f 775f 7030  x + a * x_pow_p0
+0002a880: 202b 2062 202a 2078 5f70 6f77 5f70 3120   + b * x_pow_p1 
+0002a890: 2b20 6320 2a20 785f 706f 775f 7031 202a  + c * x_pow_p1 *
+0002a8a0: 2078 0a0a 2020 2020 2020 2020 7a65 726f   x..        zero
+0002a8b0: 3a20 746f 7263 682e 5465 6e73 6f72 203d  : torch.Tensor =
+0002a8c0: 2074 6f72 6368 2e7a 6572 6f73 5f6c 696b   torch.zeros_lik
+0002a8d0: 6528 7829 0a20 2020 2020 2020 206f 7574  e(x).        out
+0002a8e0: 7075 743a 2074 6f72 6368 2e54 656e 736f  put: torch.Tenso
+0002a8f0: 7220 3d20 746f 7263 682e 7768 6572 6528  r = torch.where(
+0002a900: 7820 3c20 312c 2065 6e76 5f76 616c 2c20  x < 1, env_val, 
+0002a910: 7a65 726f 290a 2020 2020 2020 2020 7265  zero).        re
+0002a920: 7475 726e 206f 7574 7075 740a            turn output.
```

### Comparing `deepchem-2.7.2.dev20230728002356/deepchem/models/torch_models/lcnn.py` & `deepchem-2.7.2.dev20230730200710/deepchem/models/torch_models/lcnn.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230728002356/deepchem/models/torch_models/mat.py` & `deepchem-2.7.2.dev20230730200710/deepchem/models/torch_models/mat.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230728002356/deepchem/models/torch_models/megnet.py` & `deepchem-2.7.2.dev20230730200710/deepchem/models/torch_models/megnet.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230728002356/deepchem/models/torch_models/modular.py` & `deepchem-2.7.2.dev20230730200710/deepchem/models/torch_models/modular.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230728002356/deepchem/models/torch_models/mpnn.py` & `deepchem-2.7.2.dev20230730200710/deepchem/models/torch_models/mpnn.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230728002356/deepchem/models/torch_models/normalizing_flows_pytorch.py` & `deepchem-2.7.2.dev20230730200710/deepchem/models/torch_models/normalizing_flows_pytorch.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230728002356/deepchem/models/torch_models/pagtn.py` & `deepchem-2.7.2.dev20230730200710/deepchem/models/torch_models/pagtn.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230728002356/deepchem/models/torch_models/pna_gnn.py` & `deepchem-2.7.2.dev20230730200710/deepchem/models/torch_models/pna_gnn.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230728002356/deepchem/models/torch_models/readout.py` & `deepchem-2.7.2.dev20230730200710/deepchem/models/torch_models/readout.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230728002356/deepchem/models/torch_models/torch_model.py` & `deepchem-2.7.2.dev20230730200710/deepchem/models/torch_models/torch_model.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230728002356/deepchem/models/wandblogger.py` & `deepchem-2.7.2.dev20230730200710/deepchem/models/wandblogger.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230728002356/deepchem/molnet/__init__.py` & `deepchem-2.7.2.dev20230730200710/deepchem/molnet/__init__.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230728002356/deepchem/molnet/check_availability.py` & `deepchem-2.7.2.dev20230730200710/deepchem/molnet/check_availability.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230728002356/deepchem/molnet/defaults.py` & `deepchem-2.7.2.dev20230730200710/deepchem/molnet/defaults.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230728002356/deepchem/molnet/dnasim.py` & `deepchem-2.7.2.dev20230730200710/deepchem/molnet/dnasim.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230728002356/deepchem/molnet/load_function/bace_datasets.py` & `deepchem-2.7.2.dev20230730200710/deepchem/molnet/load_function/bace_datasets.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230728002356/deepchem/molnet/load_function/bace_features.py` & `deepchem-2.7.2.dev20230730200710/deepchem/molnet/load_function/bace_features.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230728002356/deepchem/molnet/load_function/bbbc_datasets.py` & `deepchem-2.7.2.dev20230730200710/deepchem/molnet/load_function/bbbc_datasets.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230728002356/deepchem/molnet/load_function/bbbp_datasets.py` & `deepchem-2.7.2.dev20230730200710/deepchem/molnet/load_function/bbbp_datasets.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230728002356/deepchem/molnet/load_function/cell_counting_datasets.py` & `deepchem-2.7.2.dev20230730200710/deepchem/molnet/load_function/cell_counting_datasets.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230728002356/deepchem/molnet/load_function/chembl25_datasets.py` & `deepchem-2.7.2.dev20230730200710/deepchem/molnet/load_function/chembl25_datasets.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230728002356/deepchem/molnet/load_function/chembl_datasets.py` & `deepchem-2.7.2.dev20230730200710/deepchem/molnet/load_function/chembl_datasets.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230728002356/deepchem/molnet/load_function/chembl_tasks.py` & `deepchem-2.7.2.dev20230730200710/deepchem/molnet/load_function/chembl_tasks.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230728002356/deepchem/molnet/load_function/clearance_datasets.py` & `deepchem-2.7.2.dev20230730200710/deepchem/molnet/load_function/clearance_datasets.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230728002356/deepchem/molnet/load_function/clintox_datasets.py` & `deepchem-2.7.2.dev20230730200710/deepchem/molnet/load_function/clintox_datasets.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230728002356/deepchem/molnet/load_function/delaney_datasets.py` & `deepchem-2.7.2.dev20230730200710/deepchem/molnet/load_function/delaney_datasets.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230728002356/deepchem/molnet/load_function/factors_datasets.py` & `deepchem-2.7.2.dev20230730200710/deepchem/molnet/load_function/factors_datasets.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230728002356/deepchem/molnet/load_function/freesolv_dataset.py` & `deepchem-2.7.2.dev20230730200710/deepchem/molnet/load_function/freesolv_dataset.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230728002356/deepchem/molnet/load_function/hiv_datasets.py` & `deepchem-2.7.2.dev20230730200710/deepchem/molnet/load_function/hiv_datasets.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230728002356/deepchem/molnet/load_function/hopv_datasets.py` & `deepchem-2.7.2.dev20230730200710/deepchem/molnet/load_function/hopv_datasets.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230728002356/deepchem/molnet/load_function/hppb_datasets.py` & `deepchem-2.7.2.dev20230730200710/deepchem/molnet/load_function/hppb_datasets.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230728002356/deepchem/molnet/load_function/kaggle_datasets.py` & `deepchem-2.7.2.dev20230730200710/deepchem/molnet/load_function/kaggle_datasets.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230728002356/deepchem/molnet/load_function/kaggle_features.py` & `deepchem-2.7.2.dev20230730200710/deepchem/molnet/load_function/kaggle_features.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230728002356/deepchem/molnet/load_function/kinase_datasets.py` & `deepchem-2.7.2.dev20230730200710/deepchem/molnet/load_function/kinase_datasets.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230728002356/deepchem/molnet/load_function/lipo_datasets.py` & `deepchem-2.7.2.dev20230730200710/deepchem/molnet/load_function/lipo_datasets.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230728002356/deepchem/molnet/load_function/load_dataset_template.py` & `deepchem-2.7.2.dev20230730200710/deepchem/molnet/load_function/load_dataset_template.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230728002356/deepchem/molnet/load_function/material_datasets/load_Pt_NO_surface_adsorbate_energy.py` & `deepchem-2.7.2.dev20230730200710/deepchem/molnet/load_function/material_datasets/load_Pt_NO_surface_adsorbate_energy.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230728002356/deepchem/molnet/load_function/material_datasets/load_bandgap.py` & `deepchem-2.7.2.dev20230730200710/deepchem/molnet/load_function/material_datasets/load_bandgap.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230728002356/deepchem/molnet/load_function/material_datasets/load_mp_formation_energy.py` & `deepchem-2.7.2.dev20230730200710/deepchem/molnet/load_function/material_datasets/load_mp_formation_energy.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230728002356/deepchem/molnet/load_function/material_datasets/load_mp_metallicity.py` & `deepchem-2.7.2.dev20230730200710/deepchem/molnet/load_function/material_datasets/load_mp_metallicity.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230728002356/deepchem/molnet/load_function/material_datasets/load_perovskite.py` & `deepchem-2.7.2.dev20230730200710/deepchem/molnet/load_function/material_datasets/load_perovskite.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230728002356/deepchem/molnet/load_function/molnet_loader.py` & `deepchem-2.7.2.dev20230730200710/deepchem/molnet/load_function/molnet_loader.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230728002356/deepchem/molnet/load_function/muv_datasets.py` & `deepchem-2.7.2.dev20230730200710/deepchem/molnet/load_function/muv_datasets.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230728002356/deepchem/molnet/load_function/nci_datasets.py` & `deepchem-2.7.2.dev20230730200710/deepchem/molnet/load_function/nci_datasets.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230728002356/deepchem/molnet/load_function/pcba_datasets.py` & `deepchem-2.7.2.dev20230730200710/deepchem/molnet/load_function/pcba_datasets.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230728002356/deepchem/molnet/load_function/pdbbind_datasets.py` & `deepchem-2.7.2.dev20230730200710/deepchem/molnet/load_function/pdbbind_datasets.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230728002356/deepchem/molnet/load_function/ppb_datasets.py` & `deepchem-2.7.2.dev20230730200710/deepchem/molnet/load_function/ppb_datasets.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230728002356/deepchem/molnet/load_function/qm7_datasets.py` & `deepchem-2.7.2.dev20230730200710/deepchem/molnet/load_function/qm7_datasets.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230728002356/deepchem/molnet/load_function/qm8_datasets.py` & `deepchem-2.7.2.dev20230730200710/deepchem/molnet/load_function/qm8_datasets.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230728002356/deepchem/molnet/load_function/qm9_datasets.py` & `deepchem-2.7.2.dev20230730200710/deepchem/molnet/load_function/qm9_datasets.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230728002356/deepchem/molnet/load_function/sampl_datasets.py` & `deepchem-2.7.2.dev20230730200710/deepchem/molnet/load_function/sampl_datasets.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230728002356/deepchem/molnet/load_function/sider_datasets.py` & `deepchem-2.7.2.dev20230730200710/deepchem/molnet/load_function/sider_datasets.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230728002356/deepchem/molnet/load_function/sweetlead_datasets.py` & `deepchem-2.7.2.dev20230730200710/deepchem/molnet/load_function/sweetlead_datasets.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230728002356/deepchem/molnet/load_function/thermosol_datasets.py` & `deepchem-2.7.2.dev20230730200710/deepchem/molnet/load_function/thermosol_datasets.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230728002356/deepchem/molnet/load_function/tox21_datasets.py` & `deepchem-2.7.2.dev20230730200710/deepchem/molnet/load_function/tox21_datasets.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230728002356/deepchem/molnet/load_function/toxcast_datasets.py` & `deepchem-2.7.2.dev20230730200710/deepchem/molnet/load_function/toxcast_datasets.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230728002356/deepchem/molnet/load_function/uspto_datasets.py` & `deepchem-2.7.2.dev20230730200710/deepchem/molnet/load_function/uspto_datasets.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230728002356/deepchem/molnet/load_function/uv_datasets.py` & `deepchem-2.7.2.dev20230730200710/deepchem/molnet/load_function/uv_datasets.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230728002356/deepchem/molnet/load_function/uv_tasks.py` & `deepchem-2.7.2.dev20230730200710/deepchem/molnet/load_function/uv_tasks.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230728002356/deepchem/molnet/load_function/zinc15_datasets.py` & `deepchem-2.7.2.dev20230730200710/deepchem/molnet/load_function/zinc15_datasets.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230728002356/deepchem/molnet/preset_hyper_parameters.py` & `deepchem-2.7.2.dev20230730200710/deepchem/molnet/preset_hyper_parameters.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230728002356/deepchem/molnet/run_benchmark.py` & `deepchem-2.7.2.dev20230730200710/deepchem/molnet/run_benchmark.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230728002356/deepchem/molnet/run_benchmark_low_data.py` & `deepchem-2.7.2.dev20230730200710/deepchem/molnet/run_benchmark_low_data.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230728002356/deepchem/molnet/run_benchmark_models.py` & `deepchem-2.7.2.dev20230730200710/deepchem/molnet/run_benchmark_models.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230728002356/deepchem/rl/__init__.py` & `deepchem-2.7.2.dev20230730200710/deepchem/rl/__init__.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230728002356/deepchem/rl/a2c.py` & `deepchem-2.7.2.dev20230730200710/deepchem/rl/a2c.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230728002356/deepchem/rl/envs/test_tictactoe.py` & `deepchem-2.7.2.dev20230730200710/deepchem/rl/envs/test_tictactoe.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230728002356/deepchem/rl/envs/tictactoe.py` & `deepchem-2.7.2.dev20230730200710/deepchem/rl/envs/tictactoe.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230728002356/deepchem/rl/ppo.py` & `deepchem-2.7.2.dev20230730200710/deepchem/rl/ppo.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230728002356/deepchem/splits/__init__.py` & `deepchem-2.7.2.dev20230730200710/deepchem/splits/__init__.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230728002356/deepchem/splits/splitters.py` & `deepchem-2.7.2.dev20230730200710/deepchem/splits/splitters.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230728002356/deepchem/splits/task_splitter.py` & `deepchem-2.7.2.dev20230730200710/deepchem/splits/task_splitter.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230728002356/deepchem/trans/__init__.py` & `deepchem-2.7.2.dev20230730200710/deepchem/trans/__init__.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230728002356/deepchem/trans/duplicate.py` & `deepchem-2.7.2.dev20230730200710/deepchem/trans/duplicate.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230728002356/deepchem/trans/transformers.py` & `deepchem-2.7.2.dev20230730200710/deepchem/trans/transformers.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230728002356/deepchem/utils/__init__.py` & `deepchem-2.7.2.dev20230730200710/deepchem/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230728002356/deepchem/utils/conformers.py` & `deepchem-2.7.2.dev20230730200710/deepchem/utils/conformers.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230728002356/deepchem/utils/coordinate_box_utils.py` & `deepchem-2.7.2.dev20230730200710/deepchem/utils/coordinate_box_utils.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230728002356/deepchem/utils/data_utils.py` & `deepchem-2.7.2.dev20230730200710/deepchem/utils/data_utils.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230728002356/deepchem/utils/debug_utils.py` & `deepchem-2.7.2.dev20230730200710/deepchem/utils/debug_utils.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230728002356/deepchem/utils/dftutils.py` & `deepchem-2.7.2.dev20230730200710/deepchem/utils/dftutils.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230728002356/deepchem/utils/docking_utils.py` & `deepchem-2.7.2.dev20230730200710/deepchem/utils/docking_utils.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230728002356/deepchem/utils/electron_sampler.py` & `deepchem-2.7.2.dev20230730200710/deepchem/utils/electron_sampler.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230728002356/deepchem/utils/evaluate.py` & `deepchem-2.7.2.dev20230730200710/deepchem/utils/evaluate.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230728002356/deepchem/utils/fake_data_generator.py` & `deepchem-2.7.2.dev20230730200710/deepchem/utils/fake_data_generator.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230728002356/deepchem/utils/fragment_utils.py` & `deepchem-2.7.2.dev20230730200710/deepchem/utils/fragment_utils.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230728002356/deepchem/utils/genomics_utils.py` & `deepchem-2.7.2.dev20230730200710/deepchem/utils/genomics_utils.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230728002356/deepchem/utils/geometry_utils.py` & `deepchem-2.7.2.dev20230730200710/deepchem/utils/geometry_utils.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230728002356/deepchem/utils/graph_utils.py` & `deepchem-2.7.2.dev20230730200710/deepchem/utils/graph_utils.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230728002356/deepchem/utils/grover.py` & `deepchem-2.7.2.dev20230730200710/deepchem/utils/grover.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230728002356/deepchem/utils/hash_utils.py` & `deepchem-2.7.2.dev20230730200710/deepchem/utils/hash_utils.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230728002356/deepchem/utils/molecule_feature_utils.py` & `deepchem-2.7.2.dev20230730200710/deepchem/utils/molecule_feature_utils.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230728002356/deepchem/utils/noncovalent_utils.py` & `deepchem-2.7.2.dev20230730200710/deepchem/utils/noncovalent_utils.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230728002356/deepchem/utils/pdbqt_utils.py` & `deepchem-2.7.2.dev20230730200710/deepchem/utils/pdbqt_utils.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230728002356/deepchem/utils/pytorch_utils.py` & `deepchem-2.7.2.dev20230730200710/deepchem/utils/pytorch_utils.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230728002356/deepchem/utils/rdkit_utils.py` & `deepchem-2.7.2.dev20230730200710/deepchem/utils/rdkit_utils.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230728002356/deepchem/utils/save.py` & `deepchem-2.7.2.dev20230730200710/deepchem/utils/save.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230728002356/deepchem/utils/sequence_utils.py` & `deepchem-2.7.2.dev20230730200710/deepchem/utils/sequence_utils.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230728002356/deepchem/utils/test/test_coordinate_box_utils.py` & `deepchem-2.7.2.dev20230730200710/deepchem/utils/test/test_coordinate_box_utils.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230728002356/deepchem/utils/test/test_data_utils.py` & `deepchem-2.7.2.dev20230730200710/deepchem/utils/test/test_data_utils.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230728002356/deepchem/utils/test/test_dftutils.py` & `deepchem-2.7.2.dev20230730200710/deepchem/utils/test/test_dftutils.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230728002356/deepchem/utils/test/test_docking_utils.py` & `deepchem-2.7.2.dev20230730200710/deepchem/utils/test/test_docking_utils.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230728002356/deepchem/utils/test/test_electron_sampler.py` & `deepchem-2.7.2.dev20230730200710/deepchem/utils/test/test_electron_sampler.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230728002356/deepchem/utils/test/test_evaluate.py` & `deepchem-2.7.2.dev20230730200710/deepchem/utils/test/test_evaluate.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230728002356/deepchem/utils/test/test_fake_data_generator.py` & `deepchem-2.7.2.dev20230730200710/deepchem/utils/test/test_fake_data_generator.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230728002356/deepchem/utils/test/test_fragment_utils.py` & `deepchem-2.7.2.dev20230730200710/deepchem/utils/test/test_fragment_utils.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230728002356/deepchem/utils/test/test_generator_evaluator.py` & `deepchem-2.7.2.dev20230730200710/deepchem/utils/test/test_generator_evaluator.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230728002356/deepchem/utils/test/test_genomics_utils.py` & `deepchem-2.7.2.dev20230730200710/deepchem/utils/test/test_genomics_utils.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230728002356/deepchem/utils/test/test_geometry_utils.py` & `deepchem-2.7.2.dev20230730200710/deepchem/utils/test/test_geometry_utils.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230728002356/deepchem/utils/test/test_graph_utils.py` & `deepchem-2.7.2.dev20230730200710/deepchem/utils/test/test_graph_utils.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230728002356/deepchem/utils/test/test_grover.py` & `deepchem-2.7.2.dev20230730200710/deepchem/utils/test/test_grover.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230728002356/deepchem/utils/test/test_hash_utils.py` & `deepchem-2.7.2.dev20230730200710/deepchem/utils/test/test_hash_utils.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230728002356/deepchem/utils/test/test_molecule_feature_utils.py` & `deepchem-2.7.2.dev20230730200710/deepchem/utils/test/test_molecule_feature_utils.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230728002356/deepchem/utils/test/test_noncovalent_utils.py` & `deepchem-2.7.2.dev20230730200710/deepchem/utils/test/test_noncovalent_utils.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230728002356/deepchem/utils/test/test_pdbqt_utils.py` & `deepchem-2.7.2.dev20230730200710/deepchem/utils/test/test_pdbqt_utils.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230728002356/deepchem/utils/test/test_pytorch_utils.py` & `deepchem-2.7.2.dev20230730200710/deepchem/utils/test/test_pytorch_utils.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230728002356/deepchem/utils/test/test_rdkit_utils.py` & `deepchem-2.7.2.dev20230730200710/deepchem/utils/test/test_rdkit_utils.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230728002356/deepchem/utils/test/test_sequence_utils.py` & `deepchem-2.7.2.dev20230730200710/deepchem/utils/test/test_sequence_utils.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230728002356/deepchem/utils/test/test_voxel_utils.py` & `deepchem-2.7.2.dev20230730200710/deepchem/utils/test/test_voxel_utils.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230728002356/deepchem/utils/typing.py` & `deepchem-2.7.2.dev20230730200710/deepchem/utils/typing.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230728002356/deepchem/utils/vina_utils.py` & `deepchem-2.7.2.dev20230730200710/deepchem/utils/vina_utils.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230728002356/deepchem/utils/voxel_utils.py` & `deepchem-2.7.2.dev20230730200710/deepchem/utils/voxel_utils.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230728002356/deepchem.egg-info/PKG-INFO` & `deepchem-2.7.2.dev20230730200710/deepchem.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: deepchem
-Version: 2.7.2.dev20230728002356
+Version: 2.7.2.dev20230730200710
 Summary: Deep learning models for drug discovery,         quantum chemistry, and the life sciences.
 Home-page: https://github.com/deepchem/deepchem
 Maintainer: DeepChem contributors
 License: MIT
 Project-URL: Documentation, https://deepchem.readthedocs.io/en/latest/
 Project-URL: Source, https://github.com/deepchem/deepchem
 Keywords: deepchem,chemistry,biology,materials-science,life-science,drug-discovery
```

### Comparing `deepchem-2.7.2.dev20230728002356/deepchem.egg-info/SOURCES.txt` & `deepchem-2.7.2.dev20230730200710/deepchem.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230728002356/setup.cfg` & `deepchem-2.7.2.dev20230730200710/setup.cfg`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230728002356/setup.py` & `deepchem-2.7.2.dev20230730200710/setup.py`

 * *Files identical despite different names*

