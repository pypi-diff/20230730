# Comparing `tmp/pyglove-0.4.3.dev20230729.tar.gz` & `tmp/pyglove-0.4.3.dev20230730.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyglove-0.4.3.dev20230729.tar", last modified: Sat Jul 29 08:06:15 2023, max compression
+gzip compressed data, was "pyglove-0.4.3.dev20230730.tar", last modified: Sun Jul 30 08:06:26 2023, max compression
```

## Comparing `pyglove-0.4.3.dev20230729.tar` & `pyglove-0.4.3.dev20230730.tar`

### file list

```diff
@@ -1,196 +1,196 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 08:06:15.074096 pyglove-0.4.3.dev20230729/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-07-29 08:06:01.000000 pyglove-0.4.3.dev20230729/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     6624 2023-07-29 08:06:15.074096 pyglove-0.4.3.dev20230729/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5532 2023-07-29 08:06:13.000000 pyglove-0.4.3.dev20230729/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 08:06:15.026094 pyglove-0.4.3.dev20230729/pyglove/
--rw-r--r--   0 runner    (1001) docker     (123)     1352 2023-07-29 08:06:01.000000 pyglove-0.4.3.dev20230729/pyglove/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 08:06:15.030094 pyglove-0.4.3.dev20230729/pyglove/core/
--rw-r--r--   0 runner    (1001) docker     (123)     8549 2023-07-29 08:06:01.000000 pyglove-0.4.3.dev20230729/pyglove/core/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 08:06:15.030094 pyglove-0.4.3.dev20230729/pyglove/core/detouring/
--rw-r--r--   0 runner    (1001) docker     (123)     1891 2023-07-29 08:06:01.000000 pyglove-0.4.3.dev20230729/pyglove/core/detouring/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13312 2023-07-29 08:06:01.000000 pyglove-0.4.3.dev20230729/pyglove/core/detouring/class_detour.py
--rw-r--r--   0 runner    (1001) docker     (123)     5507 2023-07-29 08:06:01.000000 pyglove-0.4.3.dev20230729/pyglove/core/detouring/class_detour_test.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 08:06:15.038095 pyglove-0.4.3.dev20230729/pyglove/core/geno/
--rw-r--r--   0 runner    (1001) docker     (123)     4767 2023-07-29 08:06:01.000000 pyglove-0.4.3.dev20230729/pyglove/core/geno/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    64411 2023-07-29 08:06:01.000000 pyglove-0.4.3.dev20230729/pyglove/core/geno/base.py
--rw-r--r--   0 runner    (1001) docker     (123)    38561 2023-07-29 08:06:01.000000 pyglove-0.4.3.dev20230729/pyglove/core/geno/base_test.py
--rw-r--r--   0 runner    (1001) docker     (123)    28154 2023-07-29 08:06:01.000000 pyglove-0.4.3.dev20230729/pyglove/core/geno/categorical.py
--rw-r--r--   0 runner    (1001) docker     (123)    18444 2023-07-29 08:06:01.000000 pyglove-0.4.3.dev20230729/pyglove/core/geno/categorical_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     7194 2023-07-29 08:06:01.000000 pyglove-0.4.3.dev20230729/pyglove/core/geno/custom.py
--rw-r--r--   0 runner    (1001) docker     (123)     5938 2023-07-29 08:06:01.000000 pyglove-0.4.3.dev20230729/pyglove/core/geno/custom_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     5205 2023-07-29 08:06:01.000000 pyglove-0.4.3.dev20230729/pyglove/core/geno/deduping.py
--rw-r--r--   0 runner    (1001) docker     (123)     4583 2023-07-29 08:06:01.000000 pyglove-0.4.3.dev20230729/pyglove/core/geno/deduping_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     8959 2023-07-29 08:06:01.000000 pyglove-0.4.3.dev20230729/pyglove/core/geno/dna_generator.py
--rw-r--r--   0 runner    (1001) docker     (123)     4731 2023-07-29 08:06:01.000000 pyglove-0.4.3.dev20230729/pyglove/core/geno/dna_generator_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     8330 2023-07-29 08:06:01.000000 pyglove-0.4.3.dev20230729/pyglove/core/geno/numerical.py
--rw-r--r--   0 runner    (1001) docker     (123)     5796 2023-07-29 08:06:01.000000 pyglove-0.4.3.dev20230729/pyglove/core/geno/numerical_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     2619 2023-07-29 08:06:01.000000 pyglove-0.4.3.dev20230729/pyglove/core/geno/random.py
--rw-r--r--   0 runner    (1001) docker     (123)     4941 2023-07-29 08:06:01.000000 pyglove-0.4.3.dev20230729/pyglove/core/geno/random_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     9296 2023-07-29 08:06:01.000000 pyglove-0.4.3.dev20230729/pyglove/core/geno/space.py
--rw-r--r--   0 runner    (1001) docker     (123)    16554 2023-07-29 08:06:01.000000 pyglove-0.4.3.dev20230729/pyglove/core/geno/space_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     1322 2023-07-29 08:06:01.000000 pyglove-0.4.3.dev20230729/pyglove/core/geno/sweeping.py
--rw-r--r--   0 runner    (1001) docker     (123)     2709 2023-07-29 08:06:01.000000 pyglove-0.4.3.dev20230729/pyglove/core/geno/sweeping_test.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 08:06:15.046095 pyglove-0.4.3.dev20230729/pyglove/core/hyper/
--rw-r--r--   0 runner    (1001) docker     (123)     5020 2023-07-29 08:06:01.000000 pyglove-0.4.3.dev20230729/pyglove/core/hyper/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7069 2023-07-29 08:06:01.000000 pyglove-0.4.3.dev20230729/pyglove/core/hyper/base.py
--rw-r--r--   0 runner    (1001) docker     (123)    23216 2023-07-29 08:06:01.000000 pyglove-0.4.3.dev20230729/pyglove/core/hyper/categorical.py
--rw-r--r--   0 runner    (1001) docker     (123)    13533 2023-07-29 08:06:01.000000 pyglove-0.4.3.dev20230729/pyglove/core/hyper/categorical_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     5750 2023-07-29 08:06:01.000000 pyglove-0.4.3.dev20230729/pyglove/core/hyper/custom.py
--rw-r--r--   0 runner    (1001) docker     (123)     3556 2023-07-29 08:06:01.000000 pyglove-0.4.3.dev20230729/pyglove/core/hyper/custom_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     6130 2023-07-29 08:06:01.000000 pyglove-0.4.3.dev20230729/pyglove/core/hyper/derived.py
--rw-r--r--   0 runner    (1001) docker     (123)     4283 2023-07-29 08:06:01.000000 pyglove-0.4.3.dev20230729/pyglove/core/hyper/derived_test.py
--rw-r--r--   0 runner    (1001) docker     (123)    22813 2023-07-29 08:06:01.000000 pyglove-0.4.3.dev20230729/pyglove/core/hyper/dynamic_evaluation.py
--rw-r--r--   0 runner    (1001) docker     (123)    17149 2023-07-29 08:06:01.000000 pyglove-0.4.3.dev20230729/pyglove/core/hyper/dynamic_evaluation_test.py
--rw-r--r--   0 runner    (1001) docker     (123)    10161 2023-07-29 08:06:01.000000 pyglove-0.4.3.dev20230729/pyglove/core/hyper/evolvable.py
--rw-r--r--   0 runner    (1001) docker     (123)     7505 2023-07-29 08:06:01.000000 pyglove-0.4.3.dev20230729/pyglove/core/hyper/evolvable_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     6921 2023-07-29 08:06:01.000000 pyglove-0.4.3.dev20230729/pyglove/core/hyper/iter.py
--rw-r--r--   0 runner    (1001) docker     (123)     3906 2023-07-29 08:06:01.000000 pyglove-0.4.3.dev20230729/pyglove/core/hyper/iter_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     8206 2023-07-29 08:06:01.000000 pyglove-0.4.3.dev20230729/pyglove/core/hyper/numerical.py
--rw-r--r--   0 runner    (1001) docker     (123)     4259 2023-07-29 08:06:01.000000 pyglove-0.4.3.dev20230729/pyglove/core/hyper/numerical_test.py
--rw-r--r--   0 runner    (1001) docker     (123)    22325 2023-07-29 08:06:01.000000 pyglove-0.4.3.dev20230729/pyglove/core/hyper/object_template.py
--rw-r--r--   0 runner    (1001) docker     (123)     9105 2023-07-29 08:06:01.000000 pyglove-0.4.3.dev20230729/pyglove/core/hyper/object_template_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     2456 2023-07-29 08:06:01.000000 pyglove-0.4.3.dev20230729/pyglove/core/logging.py
--rw-r--r--   0 runner    (1001) docker     (123)     1956 2023-07-29 08:06:01.000000 pyglove-0.4.3.dev20230729/pyglove/core/logging_test.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 08:06:15.054095 pyglove-0.4.3.dev20230729/pyglove/core/object_utils/
--rw-r--r--   0 runner    (1001) docker     (123)     7649 2023-07-29 08:06:01.000000 pyglove-0.4.3.dev20230729/pyglove/core/object_utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1568 2023-07-29 08:06:01.000000 pyglove-0.4.3.dev20230729/pyglove/core/object_utils/codegen.py
--rw-r--r--   0 runner    (1001) docker     (123)     2166 2023-07-29 08:06:01.000000 pyglove-0.4.3.dev20230729/pyglove/core/object_utils/codegen_test.py
--rw-r--r--   0 runner    (1001) docker     (123)    15301 2023-07-29 08:06:01.000000 pyglove-0.4.3.dev20230729/pyglove/core/object_utils/common_traits.py
--rw-r--r--   0 runner    (1001) docker     (123)     3685 2023-07-29 08:06:01.000000 pyglove-0.4.3.dev20230729/pyglove/core/object_utils/common_traits_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     4303 2023-07-29 08:06:01.000000 pyglove-0.4.3.dev20230729/pyglove/core/object_utils/docstr_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     3165 2023-07-29 08:06:01.000000 pyglove-0.4.3.dev20230729/pyglove/core/object_utils/docstr_utils_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     6852 2023-07-29 08:06:01.000000 pyglove-0.4.3.dev20230729/pyglove/core/object_utils/formatting.py
--rw-r--r--   0 runner    (1001) docker     (123)     5901 2023-07-29 08:06:01.000000 pyglove-0.4.3.dev20230729/pyglove/core/object_utils/formatting_test.py
--rw-r--r--   0 runner    (1001) docker     (123)    19754 2023-07-29 08:06:01.000000 pyglove-0.4.3.dev20230729/pyglove/core/object_utils/hierarchical.py
--rw-r--r--   0 runner    (1001) docker     (123)    21150 2023-07-29 08:06:01.000000 pyglove-0.4.3.dev20230729/pyglove/core/object_utils/hierarchical_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     1268 2023-07-29 08:06:01.000000 pyglove-0.4.3.dev20230729/pyglove/core/object_utils/missing.py
--rw-r--r--   0 runner    (1001) docker     (123)     1178 2023-07-29 08:06:01.000000 pyglove-0.4.3.dev20230729/pyglove/core/object_utils/missing_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     3850 2023-07-29 08:06:01.000000 pyglove-0.4.3.dev20230729/pyglove/core/object_utils/thread_local.py
--rw-r--r--   0 runner    (1001) docker     (123)     5391 2023-07-29 08:06:01.000000 pyglove-0.4.3.dev20230729/pyglove/core/object_utils/thread_local_test.py
--rw-r--r--   0 runner    (1001) docker     (123)    18160 2023-07-29 08:06:01.000000 pyglove-0.4.3.dev20230729/pyglove/core/object_utils/value_location.py
--rw-r--r--   0 runner    (1001) docker     (123)    13083 2023-07-29 08:06:01.000000 pyglove-0.4.3.dev20230729/pyglove/core/object_utils/value_location_test.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 08:06:15.054095 pyglove-0.4.3.dev20230729/pyglove/core/patching/
--rw-r--r--   0 runner    (1001) docker     (123)     2059 2023-07-29 08:06:01.000000 pyglove-0.4.3.dev20230729/pyglove/core/patching/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3377 2023-07-29 08:06:01.000000 pyglove-0.4.3.dev20230729/pyglove/core/patching/object_factory.py
--rw-r--r--   0 runner    (1001) docker     (123)     3973 2023-07-29 08:06:01.000000 pyglove-0.4.3.dev20230729/pyglove/core/patching/object_factory_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     7872 2023-07-29 08:06:01.000000 pyglove-0.4.3.dev20230729/pyglove/core/patching/pattern_based.py
--rw-r--r--   0 runner    (1001) docker     (123)     2771 2023-07-29 08:06:01.000000 pyglove-0.4.3.dev20230729/pyglove/core/patching/pattern_based_test.py
--rw-r--r--   0 runner    (1001) docker     (123)    16675 2023-07-29 08:06:01.000000 pyglove-0.4.3.dev20230729/pyglove/core/patching/rule_based.py
--rw-r--r--   0 runner    (1001) docker     (123)    17894 2023-07-29 08:06:01.000000 pyglove-0.4.3.dev20230729/pyglove/core/patching/rule_based_test.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 08:06:15.062095 pyglove-0.4.3.dev20230729/pyglove/core/symbolic/
--rw-r--r--   0 runner    (1001) docker     (123)     6023 2023-07-29 08:06:01.000000 pyglove-0.4.3.dev20230729/pyglove/core/symbolic/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    78519 2023-07-29 08:06:01.000000 pyglove-0.4.3.dev20230729/pyglove/core/symbolic/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     4273 2023-07-29 08:06:01.000000 pyglove-0.4.3.dev20230729/pyglove/core/symbolic/base_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     6138 2023-07-29 08:06:01.000000 pyglove-0.4.3.dev20230729/pyglove/core/symbolic/boilerplate.py
--rw-r--r--   0 runner    (1001) docker     (123)     4614 2023-07-29 08:06:01.000000 pyglove-0.4.3.dev20230729/pyglove/core/symbolic/boilerplate_test.py
--rw-r--r--   0 runner    (1001) docker     (123)    22715 2023-07-29 08:06:01.000000 pyglove-0.4.3.dev20230729/pyglove/core/symbolic/class_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (123)    21508 2023-07-29 08:06:01.000000 pyglove-0.4.3.dev20230729/pyglove/core/symbolic/class_wrapper_test.py
--rw-r--r--   0 runner    (1001) docker     (123)    11904 2023-07-29 08:06:01.000000 pyglove-0.4.3.dev20230729/pyglove/core/symbolic/compounding.py
--rw-r--r--   0 runner    (1001) docker     (123)     8343 2023-07-29 08:06:01.000000 pyglove-0.4.3.dev20230729/pyglove/core/symbolic/compounding_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     1983 2023-07-29 08:06:01.000000 pyglove-0.4.3.dev20230729/pyglove/core/symbolic/contextual.py
--rw-r--r--   0 runner    (1001) docker     (123)     1348 2023-07-29 08:06:01.000000 pyglove-0.4.3.dev20230729/pyglove/core/symbolic/contextual_test.py
--rw-r--r--   0 runner    (1001) docker     (123)    35745 2023-07-29 08:06:01.000000 pyglove-0.4.3.dev20230729/pyglove/core/symbolic/dict.py
--rw-r--r--   0 runner    (1001) docker     (123)    64268 2023-07-29 08:06:01.000000 pyglove-0.4.3.dev20230729/pyglove/core/symbolic/dict_test.py
--rw-r--r--   0 runner    (1001) docker     (123)    10676 2023-07-29 08:06:01.000000 pyglove-0.4.3.dev20230729/pyglove/core/symbolic/diff.py
--rw-r--r--   0 runner    (1001) docker     (123)    10007 2023-07-29 08:06:01.000000 pyglove-0.4.3.dev20230729/pyglove/core/symbolic/diff_test.py
--rw-r--r--   0 runner    (1001) docker     (123)    12097 2023-07-29 08:06:01.000000 pyglove-0.4.3.dev20230729/pyglove/core/symbolic/flags.py
--rw-r--r--   0 runner    (1001) docker     (123)     5483 2023-07-29 08:06:01.000000 pyglove-0.4.3.dev20230729/pyglove/core/symbolic/flags_test.py
--rw-r--r--   0 runner    (1001) docker     (123)    24039 2023-07-29 08:06:01.000000 pyglove-0.4.3.dev20230729/pyglove/core/symbolic/functor.py
--rw-r--r--   0 runner    (1001) docker     (123)    29174 2023-07-29 08:06:01.000000 pyglove-0.4.3.dev20230729/pyglove/core/symbolic/functor_test.py
--rw-r--r--   0 runner    (1001) docker     (123)    30269 2023-07-29 08:06:01.000000 pyglove-0.4.3.dev20230729/pyglove/core/symbolic/list.py
--rw-r--r--   0 runner    (1001) docker     (123)    57466 2023-07-29 08:06:01.000000 pyglove-0.4.3.dev20230729/pyglove/core/symbolic/list_test.py
--rw-r--r--   0 runner    (1001) docker     (123)    36989 2023-07-29 08:06:01.000000 pyglove-0.4.3.dev20230729/pyglove/core/symbolic/object.py
--rw-r--r--   0 runner    (1001) docker     (123)    84993 2023-07-29 08:06:01.000000 pyglove-0.4.3.dev20230729/pyglove/core/symbolic/object_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     5139 2023-07-29 08:06:01.000000 pyglove-0.4.3.dev20230729/pyglove/core/symbolic/origin.py
--rw-r--r--   0 runner    (1001) docker     (123)     2393 2023-07-29 08:06:01.000000 pyglove-0.4.3.dev20230729/pyglove/core/symbolic/origin_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     3244 2023-07-29 08:06:01.000000 pyglove-0.4.3.dev20230729/pyglove/core/symbolic/pure_symbolic.py
--rw-r--r--   0 runner    (1001) docker     (123)    12688 2023-07-29 08:06:01.000000 pyglove-0.4.3.dev20230729/pyglove/core/symbolic/schema_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     1911 2023-07-29 08:06:01.000000 pyglove-0.4.3.dev20230729/pyglove/core/symbolic/schema_utils_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     6582 2023-07-29 08:06:01.000000 pyglove-0.4.3.dev20230729/pyglove/core/symbolic/symbolize.py
--rw-r--r--   0 runner    (1001) docker     (123)     6165 2023-07-29 08:06:01.000000 pyglove-0.4.3.dev20230729/pyglove/core/symbolic/symbolize_test.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 08:06:15.066095 pyglove-0.4.3.dev20230729/pyglove/core/tuning/
--rw-r--r--   0 runner    (1001) docker     (123)     2229 2023-07-29 08:06:01.000000 pyglove-0.4.3.dev20230729/pyglove/core/tuning/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5597 2023-07-29 08:06:01.000000 pyglove-0.4.3.dev20230729/pyglove/core/tuning/backend.py
--rw-r--r--   0 runner    (1001) docker     (123)     1999 2023-07-29 08:06:01.000000 pyglove-0.4.3.dev20230729/pyglove/core/tuning/backend_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     2102 2023-07-29 08:06:01.000000 pyglove-0.4.3.dev20230729/pyglove/core/tuning/early_stopping.py
--rw-r--r--   0 runner    (1001) docker     (123)    13832 2023-07-29 08:06:01.000000 pyglove-0.4.3.dev20230729/pyglove/core/tuning/local_backend.py
--rw-r--r--   0 runner    (1001) docker     (123)    17756 2023-07-29 08:06:01.000000 pyglove-0.4.3.dev20230729/pyglove/core/tuning/protocols.py
--rw-r--r--   0 runner    (1001) docker     (123)     1883 2023-07-29 08:06:01.000000 pyglove-0.4.3.dev20230729/pyglove/core/tuning/protocols_test.py
--rw-r--r--   0 runner    (1001) docker     (123)    12975 2023-07-29 08:06:01.000000 pyglove-0.4.3.dev20230729/pyglove/core/tuning/sample.py
--rw-r--r--   0 runner    (1001) docker     (123)    17552 2023-07-29 08:06:01.000000 pyglove-0.4.3.dev20230729/pyglove/core/tuning/sample_test.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 08:06:15.070096 pyglove-0.4.3.dev20230729/pyglove/core/typing/
--rw-r--r--   0 runner    (1001) docker     (123)    13301 2023-07-29 08:06:01.000000 pyglove-0.4.3.dev20230729/pyglove/core/typing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7786 2023-07-29 08:06:01.000000 pyglove-0.4.3.dev20230729/pyglove/core/typing/annotation_conversion.py
--rw-r--r--   0 runner    (1001) docker     (123)     9998 2023-07-29 08:06:01.000000 pyglove-0.4.3.dev20230729/pyglove/core/typing/annotation_conversion_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     1626 2023-07-29 08:06:01.000000 pyglove-0.4.3.dev20230729/pyglove/core/typing/callable_ext.py
--rw-r--r--   0 runner    (1001) docker     (123)     2056 2023-07-29 08:06:01.000000 pyglove-0.4.3.dev20230729/pyglove/core/typing/callable_ext_test.py
--rw-r--r--   0 runner    (1001) docker     (123)    12647 2023-07-29 08:06:01.000000 pyglove-0.4.3.dev20230729/pyglove/core/typing/callable_signature.py
--rw-r--r--   0 runner    (1001) docker     (123)    11000 2023-07-29 08:06:01.000000 pyglove-0.4.3.dev20230729/pyglove/core/typing/callable_signature_test.py
--rw-r--r--   0 runner    (1001) docker     (123)    49558 2023-07-29 08:06:01.000000 pyglove-0.4.3.dev20230729/pyglove/core/typing/class_schema.py
--rw-r--r--   0 runner    (1001) docker     (123)    25636 2023-07-29 08:06:01.000000 pyglove-0.4.3.dev20230729/pyglove/core/typing/class_schema_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     8172 2023-07-29 08:06:01.000000 pyglove-0.4.3.dev20230729/pyglove/core/typing/class_schema_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     7145 2023-07-29 08:06:01.000000 pyglove-0.4.3.dev20230729/pyglove/core/typing/class_schema_utils_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     2218 2023-07-29 08:06:01.000000 pyglove-0.4.3.dev20230729/pyglove/core/typing/custom_typing.py
--rw-r--r--   0 runner    (1001) docker     (123)     3795 2023-07-29 08:06:01.000000 pyglove-0.4.3.dev20230729/pyglove/core/typing/generic.py
--rw-r--r--   0 runner    (1001) docker     (123)     4728 2023-07-29 08:06:01.000000 pyglove-0.4.3.dev20230729/pyglove/core/typing/generic_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     8193 2023-07-29 08:06:01.000000 pyglove-0.4.3.dev20230729/pyglove/core/typing/key_specs.py
--rw-r--r--   0 runner    (1001) docker     (123)     5536 2023-07-29 08:06:01.000000 pyglove-0.4.3.dev20230729/pyglove/core/typing/key_specs_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     2069 2023-07-29 08:06:01.000000 pyglove-0.4.3.dev20230729/pyglove/core/typing/pytype_support.py
--rw-r--r--   0 runner    (1001) docker     (123)     5329 2023-07-29 08:06:01.000000 pyglove-0.4.3.dev20230729/pyglove/core/typing/type_conversion.py
--rw-r--r--   0 runner    (1001) docker     (123)     5241 2023-07-29 08:06:01.000000 pyglove-0.4.3.dev20230729/pyglove/core/typing/type_conversion_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     2784 2023-07-29 08:06:01.000000 pyglove-0.4.3.dev20230729/pyglove/core/typing/typed_missing.py
--rw-r--r--   0 runner    (1001) docker     (123)     2381 2023-07-29 08:06:01.000000 pyglove-0.4.3.dev20230729/pyglove/core/typing/typed_missing_test.py
--rw-r--r--   0 runner    (1001) docker     (123)    79809 2023-07-29 08:06:01.000000 pyglove-0.4.3.dev20230729/pyglove/core/typing/value_specs.py
--rw-r--r--   0 runner    (1001) docker     (123)   105460 2023-07-29 08:06:01.000000 pyglove-0.4.3.dev20230729/pyglove/core/typing/value_specs_test.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 08:06:15.070096 pyglove-0.4.3.dev20230729/pyglove/ext/
--rw-r--r--   0 runner    (1001) docker     (123)      755 2023-07-29 08:06:01.000000 pyglove-0.4.3.dev20230729/pyglove/ext/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 08:06:15.070096 pyglove-0.4.3.dev20230729/pyglove/ext/early_stopping/
--rw-r--r--   0 runner    (1001) docker     (123)     1116 2023-07-29 08:06:01.000000 pyglove-0.4.3.dev20230729/pyglove/ext/early_stopping/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2358 2023-07-29 08:06:01.000000 pyglove-0.4.3.dev20230729/pyglove/ext/early_stopping/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     2796 2023-07-29 08:06:01.000000 pyglove-0.4.3.dev20230729/pyglove/ext/early_stopping/base_test.py
--rw-r--r--   0 runner    (1001) docker     (123)    10117 2023-07-29 08:06:01.000000 pyglove-0.4.3.dev20230729/pyglove/ext/early_stopping/step_wise.py
--rw-r--r--   0 runner    (1001) docker     (123)     9032 2023-07-29 08:06:01.000000 pyglove-0.4.3.dev20230729/pyglove/ext/early_stopping/step_wise_test.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 08:06:15.070096 pyglove-0.4.3.dev20230729/pyglove/ext/evolution/
--rw-r--r--   0 runner    (1001) docker     (123)     3214 2023-07-29 08:06:01.000000 pyglove-0.4.3.dev20230729/pyglove/ext/evolution/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    50090 2023-07-29 08:06:01.000000 pyglove-0.4.3.dev20230729/pyglove/ext/evolution/base.py
--rw-r--r--   0 runner    (1001) docker     (123)    29936 2023-07-29 08:06:01.000000 pyglove-0.4.3.dev20230729/pyglove/ext/evolution/base_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     1688 2023-07-29 08:06:01.000000 pyglove-0.4.3.dev20230729/pyglove/ext/evolution/hill_climb.py
--rw-r--r--   0 runner    (1001) docker     (123)     3110 2023-07-29 08:06:01.000000 pyglove-0.4.3.dev20230729/pyglove/ext/evolution/hill_climb_test.py
--rw-r--r--   0 runner    (1001) docker     (123)    10062 2023-07-29 08:06:01.000000 pyglove-0.4.3.dev20230729/pyglove/ext/evolution/mutators.py
--rw-r--r--   0 runner    (1001) docker     (123)    17975 2023-07-29 08:06:01.000000 pyglove-0.4.3.dev20230729/pyglove/ext/evolution/mutators_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     8162 2023-07-29 08:06:01.000000 pyglove-0.4.3.dev20230729/pyglove/ext/evolution/neat.py
--rw-r--r--   0 runner    (1001) docker     (123)     4474 2023-07-29 08:06:01.000000 pyglove-0.4.3.dev20230729/pyglove/ext/evolution/neat_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     6427 2023-07-29 08:06:01.000000 pyglove-0.4.3.dev20230729/pyglove/ext/evolution/nsga2.py
--rw-r--r--   0 runner    (1001) docker     (123)     8430 2023-07-29 08:06:01.000000 pyglove-0.4.3.dev20230729/pyglove/ext/evolution/nsga2_test.py
--rw-r--r--   0 runner    (1001) docker     (123)    40354 2023-07-29 08:06:01.000000 pyglove-0.4.3.dev20230729/pyglove/ext/evolution/recombinators.py
--rw-r--r--   0 runner    (1001) docker     (123)    19290 2023-07-29 08:06:01.000000 pyglove-0.4.3.dev20230729/pyglove/ext/evolution/recombinators_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     1954 2023-07-29 08:06:01.000000 pyglove-0.4.3.dev20230729/pyglove/ext/evolution/regularized_evolution.py
--rw-r--r--   0 runner    (1001) docker     (123)     3472 2023-07-29 08:06:01.000000 pyglove-0.4.3.dev20230729/pyglove/ext/evolution/regularized_evolution_test.py
--rw-r--r--   0 runner    (1001) docker     (123)    12102 2023-07-29 08:06:01.000000 pyglove-0.4.3.dev20230729/pyglove/ext/evolution/selectors.py
--rw-r--r--   0 runner    (1001) docker     (123)     7714 2023-07-29 08:06:01.000000 pyglove-0.4.3.dev20230729/pyglove/ext/evolution/selectors_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     4761 2023-07-29 08:06:01.000000 pyglove-0.4.3.dev20230729/pyglove/ext/evolution/where.py
--rw-r--r--   0 runner    (1001) docker     (123)     1931 2023-07-29 08:06:01.000000 pyglove-0.4.3.dev20230729/pyglove/ext/evolution/where_test.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 08:06:15.074096 pyglove-0.4.3.dev20230729/pyglove/ext/mutfun/
--rw-r--r--   0 runner    (1001) docker     (123)     4959 2023-07-29 08:06:01.000000 pyglove-0.4.3.dev20230729/pyglove/ext/mutfun/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    16703 2023-07-29 08:06:01.000000 pyglove-0.4.3.dev20230729/pyglove/ext/mutfun/base.py
--rw-r--r--   0 runner    (1001) docker     (123)    21312 2023-07-29 08:06:01.000000 pyglove-0.4.3.dev20230729/pyglove/ext/mutfun/base_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     5667 2023-07-29 08:06:01.000000 pyglove-0.4.3.dev20230729/pyglove/ext/mutfun/basic_ops.py
--rw-r--r--   0 runner    (1001) docker     (123)    11244 2023-07-29 08:06:01.000000 pyglove-0.4.3.dev20230729/pyglove/ext/mutfun/basic_ops_test.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 08:06:15.074096 pyglove-0.4.3.dev20230729/pyglove/ext/scalars/
--rw-r--r--   0 runner    (1001) docker     (123)     2749 2023-07-29 08:06:01.000000 pyglove-0.4.3.dev20230729/pyglove/ext/scalars/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7102 2023-07-29 08:06:01.000000 pyglove-0.4.3.dev20230729/pyglove/ext/scalars/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     3095 2023-07-29 08:06:01.000000 pyglove-0.4.3.dev20230729/pyglove/ext/scalars/base_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     3188 2023-07-29 08:06:01.000000 pyglove-0.4.3.dev20230729/pyglove/ext/scalars/maths.py
--rw-r--r--   0 runner    (1001) docker     (123)     3923 2023-07-29 08:06:01.000000 pyglove-0.4.3.dev20230729/pyglove/ext/scalars/maths_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     4198 2023-07-29 08:06:01.000000 pyglove-0.4.3.dev20230729/pyglove/ext/scalars/randoms.py
--rw-r--r--   0 runner    (1001) docker     (123)     2000 2023-07-29 08:06:01.000000 pyglove-0.4.3.dev20230729/pyglove/ext/scalars/randoms_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     3789 2023-07-29 08:06:01.000000 pyglove-0.4.3.dev20230729/pyglove/ext/scalars/step_wise.py
--rw-r--r--   0 runner    (1001) docker     (123)     2540 2023-07-29 08:06:01.000000 pyglove-0.4.3.dev20230729/pyglove/ext/scalars/step_wise_test.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 08:06:15.030094 pyglove-0.4.3.dev20230729/pyglove.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     6624 2023-07-29 08:06:14.000000 pyglove-0.4.3.dev20230729/pyglove.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     6325 2023-07-29 08:06:14.000000 pyglove-0.4.3.dev20230729/pyglove.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-29 08:06:14.000000 pyglove-0.4.3.dev20230729/pyglove.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-07-29 08:06:14.000000 pyglove-0.4.3.dev20230729/pyglove.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-07-29 08:06:14.000000 pyglove-0.4.3.dev20230729/pyglove.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-29 08:06:15.074096 pyglove-0.4.3.dev20230729/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     3574 2023-07-29 08:06:01.000000 pyglove-0.4.3.dev20230729/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 08:06:26.140596 pyglove-0.4.3.dev20230730/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-07-30 08:06:12.000000 pyglove-0.4.3.dev20230730/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     6624 2023-07-30 08:06:26.140596 pyglove-0.4.3.dev20230730/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5532 2023-07-30 08:06:24.000000 pyglove-0.4.3.dev20230730/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 08:06:26.124596 pyglove-0.4.3.dev20230730/pyglove/
+-rw-r--r--   0 runner    (1001) docker     (123)     1352 2023-07-30 08:06:12.000000 pyglove-0.4.3.dev20230730/pyglove/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 08:06:26.128596 pyglove-0.4.3.dev20230730/pyglove/core/
+-rw-r--r--   0 runner    (1001) docker     (123)     8339 2023-07-30 08:06:12.000000 pyglove-0.4.3.dev20230730/pyglove/core/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 08:06:26.128596 pyglove-0.4.3.dev20230730/pyglove/core/detouring/
+-rw-r--r--   0 runner    (1001) docker     (123)     1891 2023-07-30 08:06:12.000000 pyglove-0.4.3.dev20230730/pyglove/core/detouring/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13312 2023-07-30 08:06:12.000000 pyglove-0.4.3.dev20230730/pyglove/core/detouring/class_detour.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5507 2023-07-30 08:06:12.000000 pyglove-0.4.3.dev20230730/pyglove/core/detouring/class_detour_test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 08:06:26.128596 pyglove-0.4.3.dev20230730/pyglove/core/geno/
+-rw-r--r--   0 runner    (1001) docker     (123)     4767 2023-07-30 08:06:12.000000 pyglove-0.4.3.dev20230730/pyglove/core/geno/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    64411 2023-07-30 08:06:12.000000 pyglove-0.4.3.dev20230730/pyglove/core/geno/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    38561 2023-07-30 08:06:12.000000 pyglove-0.4.3.dev20230730/pyglove/core/geno/base_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28154 2023-07-30 08:06:12.000000 pyglove-0.4.3.dev20230730/pyglove/core/geno/categorical.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18444 2023-07-30 08:06:12.000000 pyglove-0.4.3.dev20230730/pyglove/core/geno/categorical_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7194 2023-07-30 08:06:12.000000 pyglove-0.4.3.dev20230730/pyglove/core/geno/custom.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5938 2023-07-30 08:06:12.000000 pyglove-0.4.3.dev20230730/pyglove/core/geno/custom_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5205 2023-07-30 08:06:12.000000 pyglove-0.4.3.dev20230730/pyglove/core/geno/deduping.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4583 2023-07-30 08:06:12.000000 pyglove-0.4.3.dev20230730/pyglove/core/geno/deduping_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8959 2023-07-30 08:06:12.000000 pyglove-0.4.3.dev20230730/pyglove/core/geno/dna_generator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4731 2023-07-30 08:06:12.000000 pyglove-0.4.3.dev20230730/pyglove/core/geno/dna_generator_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8330 2023-07-30 08:06:12.000000 pyglove-0.4.3.dev20230730/pyglove/core/geno/numerical.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5796 2023-07-30 08:06:12.000000 pyglove-0.4.3.dev20230730/pyglove/core/geno/numerical_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2619 2023-07-30 08:06:12.000000 pyglove-0.4.3.dev20230730/pyglove/core/geno/random.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4941 2023-07-30 08:06:12.000000 pyglove-0.4.3.dev20230730/pyglove/core/geno/random_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9296 2023-07-30 08:06:12.000000 pyglove-0.4.3.dev20230730/pyglove/core/geno/space.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16554 2023-07-30 08:06:12.000000 pyglove-0.4.3.dev20230730/pyglove/core/geno/space_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1322 2023-07-30 08:06:12.000000 pyglove-0.4.3.dev20230730/pyglove/core/geno/sweeping.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2709 2023-07-30 08:06:12.000000 pyglove-0.4.3.dev20230730/pyglove/core/geno/sweeping_test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 08:06:26.128596 pyglove-0.4.3.dev20230730/pyglove/core/hyper/
+-rw-r--r--   0 runner    (1001) docker     (123)     5020 2023-07-30 08:06:12.000000 pyglove-0.4.3.dev20230730/pyglove/core/hyper/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7069 2023-07-30 08:06:12.000000 pyglove-0.4.3.dev20230730/pyglove/core/hyper/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23216 2023-07-30 08:06:12.000000 pyglove-0.4.3.dev20230730/pyglove/core/hyper/categorical.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13533 2023-07-30 08:06:12.000000 pyglove-0.4.3.dev20230730/pyglove/core/hyper/categorical_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5750 2023-07-30 08:06:12.000000 pyglove-0.4.3.dev20230730/pyglove/core/hyper/custom.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3556 2023-07-30 08:06:12.000000 pyglove-0.4.3.dev20230730/pyglove/core/hyper/custom_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6130 2023-07-30 08:06:12.000000 pyglove-0.4.3.dev20230730/pyglove/core/hyper/derived.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4283 2023-07-30 08:06:12.000000 pyglove-0.4.3.dev20230730/pyglove/core/hyper/derived_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22813 2023-07-30 08:06:12.000000 pyglove-0.4.3.dev20230730/pyglove/core/hyper/dynamic_evaluation.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17149 2023-07-30 08:06:12.000000 pyglove-0.4.3.dev20230730/pyglove/core/hyper/dynamic_evaluation_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10161 2023-07-30 08:06:12.000000 pyglove-0.4.3.dev20230730/pyglove/core/hyper/evolvable.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7505 2023-07-30 08:06:12.000000 pyglove-0.4.3.dev20230730/pyglove/core/hyper/evolvable_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6921 2023-07-30 08:06:12.000000 pyglove-0.4.3.dev20230730/pyglove/core/hyper/iter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3906 2023-07-30 08:06:12.000000 pyglove-0.4.3.dev20230730/pyglove/core/hyper/iter_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8206 2023-07-30 08:06:12.000000 pyglove-0.4.3.dev20230730/pyglove/core/hyper/numerical.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4259 2023-07-30 08:06:12.000000 pyglove-0.4.3.dev20230730/pyglove/core/hyper/numerical_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22325 2023-07-30 08:06:12.000000 pyglove-0.4.3.dev20230730/pyglove/core/hyper/object_template.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9105 2023-07-30 08:06:12.000000 pyglove-0.4.3.dev20230730/pyglove/core/hyper/object_template_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2456 2023-07-30 08:06:12.000000 pyglove-0.4.3.dev20230730/pyglove/core/logging.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1956 2023-07-30 08:06:12.000000 pyglove-0.4.3.dev20230730/pyglove/core/logging_test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 08:06:26.132596 pyglove-0.4.3.dev20230730/pyglove/core/object_utils/
+-rw-r--r--   0 runner    (1001) docker     (123)     7649 2023-07-30 08:06:12.000000 pyglove-0.4.3.dev20230730/pyglove/core/object_utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1568 2023-07-30 08:06:12.000000 pyglove-0.4.3.dev20230730/pyglove/core/object_utils/codegen.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2166 2023-07-30 08:06:12.000000 pyglove-0.4.3.dev20230730/pyglove/core/object_utils/codegen_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15301 2023-07-30 08:06:12.000000 pyglove-0.4.3.dev20230730/pyglove/core/object_utils/common_traits.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3685 2023-07-30 08:06:12.000000 pyglove-0.4.3.dev20230730/pyglove/core/object_utils/common_traits_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4303 2023-07-30 08:06:12.000000 pyglove-0.4.3.dev20230730/pyglove/core/object_utils/docstr_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3165 2023-07-30 08:06:12.000000 pyglove-0.4.3.dev20230730/pyglove/core/object_utils/docstr_utils_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6852 2023-07-30 08:06:12.000000 pyglove-0.4.3.dev20230730/pyglove/core/object_utils/formatting.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5901 2023-07-30 08:06:12.000000 pyglove-0.4.3.dev20230730/pyglove/core/object_utils/formatting_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19754 2023-07-30 08:06:12.000000 pyglove-0.4.3.dev20230730/pyglove/core/object_utils/hierarchical.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21150 2023-07-30 08:06:12.000000 pyglove-0.4.3.dev20230730/pyglove/core/object_utils/hierarchical_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1268 2023-07-30 08:06:12.000000 pyglove-0.4.3.dev20230730/pyglove/core/object_utils/missing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1178 2023-07-30 08:06:12.000000 pyglove-0.4.3.dev20230730/pyglove/core/object_utils/missing_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3850 2023-07-30 08:06:12.000000 pyglove-0.4.3.dev20230730/pyglove/core/object_utils/thread_local.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5391 2023-07-30 08:06:12.000000 pyglove-0.4.3.dev20230730/pyglove/core/object_utils/thread_local_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18160 2023-07-30 08:06:12.000000 pyglove-0.4.3.dev20230730/pyglove/core/object_utils/value_location.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13083 2023-07-30 08:06:12.000000 pyglove-0.4.3.dev20230730/pyglove/core/object_utils/value_location_test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 08:06:26.132596 pyglove-0.4.3.dev20230730/pyglove/core/patching/
+-rw-r--r--   0 runner    (1001) docker     (123)     2059 2023-07-30 08:06:12.000000 pyglove-0.4.3.dev20230730/pyglove/core/patching/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3377 2023-07-30 08:06:12.000000 pyglove-0.4.3.dev20230730/pyglove/core/patching/object_factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3973 2023-07-30 08:06:12.000000 pyglove-0.4.3.dev20230730/pyglove/core/patching/object_factory_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7872 2023-07-30 08:06:12.000000 pyglove-0.4.3.dev20230730/pyglove/core/patching/pattern_based.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2771 2023-07-30 08:06:12.000000 pyglove-0.4.3.dev20230730/pyglove/core/patching/pattern_based_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16675 2023-07-30 08:06:12.000000 pyglove-0.4.3.dev20230730/pyglove/core/patching/rule_based.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17894 2023-07-30 08:06:12.000000 pyglove-0.4.3.dev20230730/pyglove/core/patching/rule_based_test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 08:06:26.136596 pyglove-0.4.3.dev20230730/pyglove/core/symbolic/
+-rw-r--r--   0 runner    (1001) docker     (123)     5889 2023-07-30 08:06:12.000000 pyglove-0.4.3.dev20230730/pyglove/core/symbolic/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    73654 2023-07-30 08:06:12.000000 pyglove-0.4.3.dev20230730/pyglove/core/symbolic/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2875 2023-07-30 08:06:12.000000 pyglove-0.4.3.dev20230730/pyglove/core/symbolic/base_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6138 2023-07-30 08:06:12.000000 pyglove-0.4.3.dev20230730/pyglove/core/symbolic/boilerplate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4614 2023-07-30 08:06:12.000000 pyglove-0.4.3.dev20230730/pyglove/core/symbolic/boilerplate_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22715 2023-07-30 08:06:12.000000 pyglove-0.4.3.dev20230730/pyglove/core/symbolic/class_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21508 2023-07-30 08:06:12.000000 pyglove-0.4.3.dev20230730/pyglove/core/symbolic/class_wrapper_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11932 2023-07-30 08:06:12.000000 pyglove-0.4.3.dev20230730/pyglove/core/symbolic/compounding.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8356 2023-07-30 08:06:12.000000 pyglove-0.4.3.dev20230730/pyglove/core/symbolic/compounding_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    35118 2023-07-30 08:06:12.000000 pyglove-0.4.3.dev20230730/pyglove/core/symbolic/dict.py
+-rw-r--r--   0 runner    (1001) docker     (123)    64587 2023-07-30 08:06:12.000000 pyglove-0.4.3.dev20230730/pyglove/core/symbolic/dict_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10676 2023-07-30 08:06:12.000000 pyglove-0.4.3.dev20230730/pyglove/core/symbolic/diff.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10007 2023-07-30 08:06:12.000000 pyglove-0.4.3.dev20230730/pyglove/core/symbolic/diff_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12097 2023-07-30 08:06:12.000000 pyglove-0.4.3.dev20230730/pyglove/core/symbolic/flags.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5483 2023-07-30 08:06:12.000000 pyglove-0.4.3.dev20230730/pyglove/core/symbolic/flags_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24039 2023-07-30 08:06:12.000000 pyglove-0.4.3.dev20230730/pyglove/core/symbolic/functor.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29174 2023-07-30 08:06:12.000000 pyglove-0.4.3.dev20230730/pyglove/core/symbolic/functor_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3192 2023-07-30 08:06:12.000000 pyglove-0.4.3.dev20230730/pyglove/core/symbolic/inferred.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1270 2023-07-30 08:06:12.000000 pyglove-0.4.3.dev20230730/pyglove/core/symbolic/inferred_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30062 2023-07-30 08:06:12.000000 pyglove-0.4.3.dev20230730/pyglove/core/symbolic/list.py
+-rw-r--r--   0 runner    (1001) docker     (123)    57908 2023-07-30 08:06:12.000000 pyglove-0.4.3.dev20230730/pyglove/core/symbolic/list_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    36808 2023-07-30 08:06:12.000000 pyglove-0.4.3.dev20230730/pyglove/core/symbolic/object.py
+-rw-r--r--   0 runner    (1001) docker     (123)    82689 2023-07-30 08:06:12.000000 pyglove-0.4.3.dev20230730/pyglove/core/symbolic/object_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5139 2023-07-30 08:06:12.000000 pyglove-0.4.3.dev20230730/pyglove/core/symbolic/origin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2393 2023-07-30 08:06:12.000000 pyglove-0.4.3.dev20230730/pyglove/core/symbolic/origin_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3244 2023-07-30 08:06:12.000000 pyglove-0.4.3.dev20230730/pyglove/core/symbolic/pure_symbolic.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12688 2023-07-30 08:06:12.000000 pyglove-0.4.3.dev20230730/pyglove/core/symbolic/schema_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1911 2023-07-30 08:06:12.000000 pyglove-0.4.3.dev20230730/pyglove/core/symbolic/schema_utils_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6582 2023-07-30 08:06:12.000000 pyglove-0.4.3.dev20230730/pyglove/core/symbolic/symbolize.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6165 2023-07-30 08:06:12.000000 pyglove-0.4.3.dev20230730/pyglove/core/symbolic/symbolize_test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 08:06:26.136596 pyglove-0.4.3.dev20230730/pyglove/core/tuning/
+-rw-r--r--   0 runner    (1001) docker     (123)     2229 2023-07-30 08:06:12.000000 pyglove-0.4.3.dev20230730/pyglove/core/tuning/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5597 2023-07-30 08:06:12.000000 pyglove-0.4.3.dev20230730/pyglove/core/tuning/backend.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1999 2023-07-30 08:06:12.000000 pyglove-0.4.3.dev20230730/pyglove/core/tuning/backend_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2102 2023-07-30 08:06:12.000000 pyglove-0.4.3.dev20230730/pyglove/core/tuning/early_stopping.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13832 2023-07-30 08:06:12.000000 pyglove-0.4.3.dev20230730/pyglove/core/tuning/local_backend.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17756 2023-07-30 08:06:12.000000 pyglove-0.4.3.dev20230730/pyglove/core/tuning/protocols.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1883 2023-07-30 08:06:12.000000 pyglove-0.4.3.dev20230730/pyglove/core/tuning/protocols_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12975 2023-07-30 08:06:12.000000 pyglove-0.4.3.dev20230730/pyglove/core/tuning/sample.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17552 2023-07-30 08:06:12.000000 pyglove-0.4.3.dev20230730/pyglove/core/tuning/sample_test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 08:06:26.136596 pyglove-0.4.3.dev20230730/pyglove/core/typing/
+-rw-r--r--   0 runner    (1001) docker     (123)    13301 2023-07-30 08:06:12.000000 pyglove-0.4.3.dev20230730/pyglove/core/typing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7786 2023-07-30 08:06:12.000000 pyglove-0.4.3.dev20230730/pyglove/core/typing/annotation_conversion.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9998 2023-07-30 08:06:12.000000 pyglove-0.4.3.dev20230730/pyglove/core/typing/annotation_conversion_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1626 2023-07-30 08:06:12.000000 pyglove-0.4.3.dev20230730/pyglove/core/typing/callable_ext.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2056 2023-07-30 08:06:12.000000 pyglove-0.4.3.dev20230730/pyglove/core/typing/callable_ext_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12647 2023-07-30 08:06:12.000000 pyglove-0.4.3.dev20230730/pyglove/core/typing/callable_signature.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11000 2023-07-30 08:06:12.000000 pyglove-0.4.3.dev20230730/pyglove/core/typing/callable_signature_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    49558 2023-07-30 08:06:12.000000 pyglove-0.4.3.dev20230730/pyglove/core/typing/class_schema.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25636 2023-07-30 08:06:12.000000 pyglove-0.4.3.dev20230730/pyglove/core/typing/class_schema_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8172 2023-07-30 08:06:12.000000 pyglove-0.4.3.dev20230730/pyglove/core/typing/class_schema_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7145 2023-07-30 08:06:12.000000 pyglove-0.4.3.dev20230730/pyglove/core/typing/class_schema_utils_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2218 2023-07-30 08:06:12.000000 pyglove-0.4.3.dev20230730/pyglove/core/typing/custom_typing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3795 2023-07-30 08:06:12.000000 pyglove-0.4.3.dev20230730/pyglove/core/typing/generic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4728 2023-07-30 08:06:12.000000 pyglove-0.4.3.dev20230730/pyglove/core/typing/generic_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8193 2023-07-30 08:06:12.000000 pyglove-0.4.3.dev20230730/pyglove/core/typing/key_specs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5536 2023-07-30 08:06:12.000000 pyglove-0.4.3.dev20230730/pyglove/core/typing/key_specs_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2069 2023-07-30 08:06:12.000000 pyglove-0.4.3.dev20230730/pyglove/core/typing/pytype_support.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5329 2023-07-30 08:06:12.000000 pyglove-0.4.3.dev20230730/pyglove/core/typing/type_conversion.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5241 2023-07-30 08:06:12.000000 pyglove-0.4.3.dev20230730/pyglove/core/typing/type_conversion_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2784 2023-07-30 08:06:12.000000 pyglove-0.4.3.dev20230730/pyglove/core/typing/typed_missing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2381 2023-07-30 08:06:12.000000 pyglove-0.4.3.dev20230730/pyglove/core/typing/typed_missing_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    79809 2023-07-30 08:06:12.000000 pyglove-0.4.3.dev20230730/pyglove/core/typing/value_specs.py
+-rw-r--r--   0 runner    (1001) docker     (123)   105460 2023-07-30 08:06:12.000000 pyglove-0.4.3.dev20230730/pyglove/core/typing/value_specs_test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 08:06:26.136596 pyglove-0.4.3.dev20230730/pyglove/ext/
+-rw-r--r--   0 runner    (1001) docker     (123)      755 2023-07-30 08:06:12.000000 pyglove-0.4.3.dev20230730/pyglove/ext/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 08:06:26.140596 pyglove-0.4.3.dev20230730/pyglove/ext/early_stopping/
+-rw-r--r--   0 runner    (1001) docker     (123)     1116 2023-07-30 08:06:12.000000 pyglove-0.4.3.dev20230730/pyglove/ext/early_stopping/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2358 2023-07-30 08:06:12.000000 pyglove-0.4.3.dev20230730/pyglove/ext/early_stopping/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2796 2023-07-30 08:06:12.000000 pyglove-0.4.3.dev20230730/pyglove/ext/early_stopping/base_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10117 2023-07-30 08:06:12.000000 pyglove-0.4.3.dev20230730/pyglove/ext/early_stopping/step_wise.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9032 2023-07-30 08:06:12.000000 pyglove-0.4.3.dev20230730/pyglove/ext/early_stopping/step_wise_test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 08:06:26.140596 pyglove-0.4.3.dev20230730/pyglove/ext/evolution/
+-rw-r--r--   0 runner    (1001) docker     (123)     3214 2023-07-30 08:06:12.000000 pyglove-0.4.3.dev20230730/pyglove/ext/evolution/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    50090 2023-07-30 08:06:12.000000 pyglove-0.4.3.dev20230730/pyglove/ext/evolution/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29936 2023-07-30 08:06:12.000000 pyglove-0.4.3.dev20230730/pyglove/ext/evolution/base_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1688 2023-07-30 08:06:12.000000 pyglove-0.4.3.dev20230730/pyglove/ext/evolution/hill_climb.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3110 2023-07-30 08:06:12.000000 pyglove-0.4.3.dev20230730/pyglove/ext/evolution/hill_climb_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10062 2023-07-30 08:06:12.000000 pyglove-0.4.3.dev20230730/pyglove/ext/evolution/mutators.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17975 2023-07-30 08:06:12.000000 pyglove-0.4.3.dev20230730/pyglove/ext/evolution/mutators_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8162 2023-07-30 08:06:12.000000 pyglove-0.4.3.dev20230730/pyglove/ext/evolution/neat.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4474 2023-07-30 08:06:12.000000 pyglove-0.4.3.dev20230730/pyglove/ext/evolution/neat_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6427 2023-07-30 08:06:12.000000 pyglove-0.4.3.dev20230730/pyglove/ext/evolution/nsga2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8430 2023-07-30 08:06:12.000000 pyglove-0.4.3.dev20230730/pyglove/ext/evolution/nsga2_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    40354 2023-07-30 08:06:12.000000 pyglove-0.4.3.dev20230730/pyglove/ext/evolution/recombinators.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19290 2023-07-30 08:06:12.000000 pyglove-0.4.3.dev20230730/pyglove/ext/evolution/recombinators_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1954 2023-07-30 08:06:12.000000 pyglove-0.4.3.dev20230730/pyglove/ext/evolution/regularized_evolution.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3472 2023-07-30 08:06:12.000000 pyglove-0.4.3.dev20230730/pyglove/ext/evolution/regularized_evolution_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12102 2023-07-30 08:06:12.000000 pyglove-0.4.3.dev20230730/pyglove/ext/evolution/selectors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7714 2023-07-30 08:06:12.000000 pyglove-0.4.3.dev20230730/pyglove/ext/evolution/selectors_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4761 2023-07-30 08:06:12.000000 pyglove-0.4.3.dev20230730/pyglove/ext/evolution/where.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1931 2023-07-30 08:06:12.000000 pyglove-0.4.3.dev20230730/pyglove/ext/evolution/where_test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 08:06:26.140596 pyglove-0.4.3.dev20230730/pyglove/ext/mutfun/
+-rw-r--r--   0 runner    (1001) docker     (123)     4959 2023-07-30 08:06:12.000000 pyglove-0.4.3.dev20230730/pyglove/ext/mutfun/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16703 2023-07-30 08:06:12.000000 pyglove-0.4.3.dev20230730/pyglove/ext/mutfun/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21312 2023-07-30 08:06:12.000000 pyglove-0.4.3.dev20230730/pyglove/ext/mutfun/base_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5667 2023-07-30 08:06:12.000000 pyglove-0.4.3.dev20230730/pyglove/ext/mutfun/basic_ops.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11244 2023-07-30 08:06:12.000000 pyglove-0.4.3.dev20230730/pyglove/ext/mutfun/basic_ops_test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 08:06:26.140596 pyglove-0.4.3.dev20230730/pyglove/ext/scalars/
+-rw-r--r--   0 runner    (1001) docker     (123)     2749 2023-07-30 08:06:12.000000 pyglove-0.4.3.dev20230730/pyglove/ext/scalars/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7102 2023-07-30 08:06:12.000000 pyglove-0.4.3.dev20230730/pyglove/ext/scalars/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3095 2023-07-30 08:06:12.000000 pyglove-0.4.3.dev20230730/pyglove/ext/scalars/base_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3188 2023-07-30 08:06:12.000000 pyglove-0.4.3.dev20230730/pyglove/ext/scalars/maths.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3923 2023-07-30 08:06:12.000000 pyglove-0.4.3.dev20230730/pyglove/ext/scalars/maths_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4198 2023-07-30 08:06:12.000000 pyglove-0.4.3.dev20230730/pyglove/ext/scalars/randoms.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2000 2023-07-30 08:06:12.000000 pyglove-0.4.3.dev20230730/pyglove/ext/scalars/randoms_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3789 2023-07-30 08:06:12.000000 pyglove-0.4.3.dev20230730/pyglove/ext/scalars/step_wise.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2540 2023-07-30 08:06:12.000000 pyglove-0.4.3.dev20230730/pyglove/ext/scalars/step_wise_test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 08:06:26.128596 pyglove-0.4.3.dev20230730/pyglove.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     6624 2023-07-30 08:06:26.000000 pyglove-0.4.3.dev20230730/pyglove.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6321 2023-07-30 08:06:26.000000 pyglove-0.4.3.dev20230730/pyglove.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-30 08:06:26.000000 pyglove-0.4.3.dev20230730/pyglove.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-07-30 08:06:26.000000 pyglove-0.4.3.dev20230730/pyglove.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-07-30 08:06:26.000000 pyglove-0.4.3.dev20230730/pyglove.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-30 08:06:26.140596 pyglove-0.4.3.dev20230730/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     3574 2023-07-30 08:06:12.000000 pyglove-0.4.3.dev20230730/setup.py
```

### Comparing `pyglove-0.4.3.dev20230729/LICENSE` & `pyglove-0.4.3.dev20230730/LICENSE`

 * *Files identical despite different names*

### Comparing `pyglove-0.4.3.dev20230729/PKG-INFO` & `pyglove-0.4.3.dev20230730/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyglove
-Version: 0.4.3.dev20230729
+Version: 0.4.3.dev20230730
 Summary: PyGlove: A library for manipulating Python objects.
 Home-page: https://github.com/google/pyglove
 Author: PyGlove Authors
 Author-email: pyglove-authors@google.com
 License: Apache License 2.0
 Keywords: ai machine learning automl mutable symbolic framework meta-programming
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `pyglove-0.4.3.dev20230729/README.md` & `pyglove-0.4.3.dev20230730/README.md`

 * *Files identical despite different names*

### Comparing `pyglove-0.4.3.dev20230729/pyglove/__init__.py` & `pyglove-0.4.3.dev20230730/pyglove/__init__.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.4.3.dev20230729/pyglove/core/__init__.py` & `pyglove-0.4.3.dev20230730/pyglove/core/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -161,23 +161,17 @@
 
 # Auxiliary classes:
 Origin = symbolic.Origin
 FieldUpdate = symbolic.FieldUpdate
 Insertion = symbolic.Insertion
 WritePermissionError = symbolic.WritePermissionError
 
-# Contextual value marker.
-ContextualValue = symbolic.ContextualValue
-ContextualGetter = symbolic.ContextualGetter
-
-# Decorator for making contextual getters.
-contextual_getter = symbolic.contextual_getter
-
-# Context object for computing contextual attribute.
-GetAttributeContext = symbolic.GetAttributeContext
+# Inferentiable classes.
+Inferentiable = symbolic.Inferential
+InferredValue = symbolic.InferredValue
 
 #
 # Symbols from 'typing.py'
 #
 
 # NOTE(daiyip): we introduce 'typing' as an alias for 'schema' sub-module, since
 # it may be easier to comprehend when users use pytype.
```

### Comparing `pyglove-0.4.3.dev20230729/pyglove/core/detouring/__init__.py` & `pyglove-0.4.3.dev20230730/pyglove/core/detouring/__init__.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.4.3.dev20230729/pyglove/core/detouring/class_detour.py` & `pyglove-0.4.3.dev20230730/pyglove/core/detouring/class_detour.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.4.3.dev20230729/pyglove/core/detouring/class_detour_test.py` & `pyglove-0.4.3.dev20230730/pyglove/core/detouring/class_detour_test.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.4.3.dev20230729/pyglove/core/geno/__init__.py` & `pyglove-0.4.3.dev20230730/pyglove/core/geno/__init__.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.4.3.dev20230729/pyglove/core/geno/base.py` & `pyglove-0.4.3.dev20230730/pyglove/core/geno/base.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.4.3.dev20230729/pyglove/core/geno/base_test.py` & `pyglove-0.4.3.dev20230730/pyglove/core/geno/base_test.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.4.3.dev20230729/pyglove/core/geno/categorical.py` & `pyglove-0.4.3.dev20230730/pyglove/core/geno/categorical.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.4.3.dev20230729/pyglove/core/geno/categorical_test.py` & `pyglove-0.4.3.dev20230730/pyglove/core/geno/categorical_test.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.4.3.dev20230729/pyglove/core/geno/custom.py` & `pyglove-0.4.3.dev20230730/pyglove/core/geno/custom.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.4.3.dev20230729/pyglove/core/geno/custom_test.py` & `pyglove-0.4.3.dev20230730/pyglove/core/geno/custom_test.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.4.3.dev20230729/pyglove/core/geno/deduping.py` & `pyglove-0.4.3.dev20230730/pyglove/core/geno/deduping.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.4.3.dev20230729/pyglove/core/geno/deduping_test.py` & `pyglove-0.4.3.dev20230730/pyglove/core/geno/deduping_test.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.4.3.dev20230729/pyglove/core/geno/dna_generator.py` & `pyglove-0.4.3.dev20230730/pyglove/core/geno/dna_generator.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.4.3.dev20230729/pyglove/core/geno/dna_generator_test.py` & `pyglove-0.4.3.dev20230730/pyglove/core/geno/dna_generator_test.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.4.3.dev20230729/pyglove/core/geno/numerical.py` & `pyglove-0.4.3.dev20230730/pyglove/core/geno/numerical.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.4.3.dev20230729/pyglove/core/geno/numerical_test.py` & `pyglove-0.4.3.dev20230730/pyglove/core/geno/numerical_test.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.4.3.dev20230729/pyglove/core/geno/random.py` & `pyglove-0.4.3.dev20230730/pyglove/core/geno/random.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.4.3.dev20230729/pyglove/core/geno/random_test.py` & `pyglove-0.4.3.dev20230730/pyglove/core/geno/random_test.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.4.3.dev20230729/pyglove/core/geno/space.py` & `pyglove-0.4.3.dev20230730/pyglove/core/geno/space.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.4.3.dev20230729/pyglove/core/geno/space_test.py` & `pyglove-0.4.3.dev20230730/pyglove/core/geno/space_test.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.4.3.dev20230729/pyglove/core/geno/sweeping.py` & `pyglove-0.4.3.dev20230730/pyglove/core/geno/sweeping.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.4.3.dev20230729/pyglove/core/geno/sweeping_test.py` & `pyglove-0.4.3.dev20230730/pyglove/core/geno/sweeping_test.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.4.3.dev20230729/pyglove/core/hyper/__init__.py` & `pyglove-0.4.3.dev20230730/pyglove/core/hyper/__init__.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.4.3.dev20230729/pyglove/core/hyper/base.py` & `pyglove-0.4.3.dev20230730/pyglove/core/hyper/base.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.4.3.dev20230729/pyglove/core/hyper/categorical.py` & `pyglove-0.4.3.dev20230730/pyglove/core/hyper/categorical.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.4.3.dev20230729/pyglove/core/hyper/categorical_test.py` & `pyglove-0.4.3.dev20230730/pyglove/core/hyper/categorical_test.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.4.3.dev20230729/pyglove/core/hyper/custom.py` & `pyglove-0.4.3.dev20230730/pyglove/core/hyper/custom.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.4.3.dev20230729/pyglove/core/hyper/custom_test.py` & `pyglove-0.4.3.dev20230730/pyglove/core/hyper/custom_test.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.4.3.dev20230729/pyglove/core/hyper/derived.py` & `pyglove-0.4.3.dev20230730/pyglove/core/hyper/derived.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.4.3.dev20230729/pyglove/core/hyper/derived_test.py` & `pyglove-0.4.3.dev20230730/pyglove/core/hyper/derived_test.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.4.3.dev20230729/pyglove/core/hyper/dynamic_evaluation.py` & `pyglove-0.4.3.dev20230730/pyglove/core/hyper/dynamic_evaluation.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.4.3.dev20230729/pyglove/core/hyper/dynamic_evaluation_test.py` & `pyglove-0.4.3.dev20230730/pyglove/core/hyper/dynamic_evaluation_test.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.4.3.dev20230729/pyglove/core/hyper/evolvable.py` & `pyglove-0.4.3.dev20230730/pyglove/core/hyper/evolvable.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.4.3.dev20230729/pyglove/core/hyper/evolvable_test.py` & `pyglove-0.4.3.dev20230730/pyglove/core/hyper/evolvable_test.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.4.3.dev20230729/pyglove/core/hyper/iter.py` & `pyglove-0.4.3.dev20230730/pyglove/core/hyper/iter.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.4.3.dev20230729/pyglove/core/hyper/iter_test.py` & `pyglove-0.4.3.dev20230730/pyglove/core/hyper/iter_test.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.4.3.dev20230729/pyglove/core/hyper/numerical.py` & `pyglove-0.4.3.dev20230730/pyglove/core/hyper/numerical.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.4.3.dev20230729/pyglove/core/hyper/numerical_test.py` & `pyglove-0.4.3.dev20230730/pyglove/core/hyper/numerical_test.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.4.3.dev20230729/pyglove/core/hyper/object_template.py` & `pyglove-0.4.3.dev20230730/pyglove/core/hyper/object_template.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.4.3.dev20230729/pyglove/core/hyper/object_template_test.py` & `pyglove-0.4.3.dev20230730/pyglove/core/hyper/object_template_test.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.4.3.dev20230729/pyglove/core/logging.py` & `pyglove-0.4.3.dev20230730/pyglove/core/logging.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.4.3.dev20230729/pyglove/core/logging_test.py` & `pyglove-0.4.3.dev20230730/pyglove/core/logging_test.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.4.3.dev20230729/pyglove/core/object_utils/__init__.py` & `pyglove-0.4.3.dev20230730/pyglove/core/object_utils/__init__.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.4.3.dev20230729/pyglove/core/object_utils/codegen.py` & `pyglove-0.4.3.dev20230730/pyglove/core/object_utils/codegen.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.4.3.dev20230729/pyglove/core/object_utils/codegen_test.py` & `pyglove-0.4.3.dev20230730/pyglove/core/object_utils/codegen_test.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.4.3.dev20230729/pyglove/core/object_utils/common_traits.py` & `pyglove-0.4.3.dev20230730/pyglove/core/object_utils/common_traits.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.4.3.dev20230729/pyglove/core/object_utils/common_traits_test.py` & `pyglove-0.4.3.dev20230730/pyglove/core/object_utils/common_traits_test.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.4.3.dev20230729/pyglove/core/object_utils/docstr_utils.py` & `pyglove-0.4.3.dev20230730/pyglove/core/object_utils/docstr_utils.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.4.3.dev20230729/pyglove/core/object_utils/docstr_utils_test.py` & `pyglove-0.4.3.dev20230730/pyglove/core/object_utils/docstr_utils_test.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.4.3.dev20230729/pyglove/core/object_utils/formatting.py` & `pyglove-0.4.3.dev20230730/pyglove/core/object_utils/formatting.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.4.3.dev20230729/pyglove/core/object_utils/formatting_test.py` & `pyglove-0.4.3.dev20230730/pyglove/core/object_utils/formatting_test.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.4.3.dev20230729/pyglove/core/object_utils/hierarchical.py` & `pyglove-0.4.3.dev20230730/pyglove/core/object_utils/hierarchical.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.4.3.dev20230729/pyglove/core/object_utils/hierarchical_test.py` & `pyglove-0.4.3.dev20230730/pyglove/core/object_utils/hierarchical_test.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.4.3.dev20230729/pyglove/core/object_utils/missing.py` & `pyglove-0.4.3.dev20230730/pyglove/core/object_utils/missing.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.4.3.dev20230729/pyglove/core/object_utils/missing_test.py` & `pyglove-0.4.3.dev20230730/pyglove/core/object_utils/missing_test.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.4.3.dev20230729/pyglove/core/object_utils/thread_local.py` & `pyglove-0.4.3.dev20230730/pyglove/core/object_utils/thread_local.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.4.3.dev20230729/pyglove/core/object_utils/thread_local_test.py` & `pyglove-0.4.3.dev20230730/pyglove/core/object_utils/thread_local_test.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.4.3.dev20230729/pyglove/core/object_utils/value_location.py` & `pyglove-0.4.3.dev20230730/pyglove/core/object_utils/value_location.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.4.3.dev20230729/pyglove/core/object_utils/value_location_test.py` & `pyglove-0.4.3.dev20230730/pyglove/core/object_utils/value_location_test.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.4.3.dev20230729/pyglove/core/patching/__init__.py` & `pyglove-0.4.3.dev20230730/pyglove/core/patching/__init__.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.4.3.dev20230729/pyglove/core/patching/object_factory.py` & `pyglove-0.4.3.dev20230730/pyglove/core/patching/object_factory.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.4.3.dev20230729/pyglove/core/patching/object_factory_test.py` & `pyglove-0.4.3.dev20230730/pyglove/core/patching/object_factory_test.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.4.3.dev20230729/pyglove/core/patching/pattern_based.py` & `pyglove-0.4.3.dev20230730/pyglove/core/patching/pattern_based.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.4.3.dev20230729/pyglove/core/patching/pattern_based_test.py` & `pyglove-0.4.3.dev20230730/pyglove/core/patching/pattern_based_test.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.4.3.dev20230729/pyglove/core/patching/rule_based.py` & `pyglove-0.4.3.dev20230730/pyglove/core/patching/rule_based.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.4.3.dev20230729/pyglove/core/patching/rule_based_test.py` & `pyglove-0.4.3.dev20230730/pyglove/core/patching/rule_based_test.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.4.3.dev20230729/pyglove/core/symbolic/__init__.py` & `pyglove-0.4.3.dev20230730/pyglove/core/symbolic/__init__.py`

 * *Files 22% similar despite different names*

```diff
@@ -56,21 +56,19 @@
 
 from pyglove.core.symbolic.flags import notify_on_change
 from pyglove.core.symbolic.flags import is_change_notification_enabled
 
 from pyglove.core.symbolic.flags import auto_call_functors
 from pyglove.core.symbolic.flags import should_call_functors_during_init
 
-# Marker for contextual values.
-from pyglove.core.symbolic.base import ContextualValue
-from pyglove.core.symbolic.contextual import ContextualGetter
-from pyglove.core.symbolic.contextual import contextual_getter
+# Inferential values
+from pyglove.core.symbolic.base import Inferential
 
-# GetAttribute context for computing contextual values.
-from pyglove.core.symbolic.base import GetAttributeContext
+from pyglove.core.symbolic.inferred import InferredValue
+from pyglove.core.symbolic.inferred import ValueFromParentChain
 
 # Symbolic types and their definition helpers.
 from pyglove.core.symbolic.base import Symbolic
 from pyglove.core.symbolic.list import List
 from pyglove.core.symbolic.dict import Dict
 
 from pyglove.core.symbolic.object import ObjectMeta
```

### Comparing `pyglove-0.4.3.dev20230729/pyglove/core/symbolic/base.py` & `pyglove-0.4.3.dev20230730/pyglove/core/symbolic/base.py`

 * *Files 3% similar despite different names*

```diff
@@ -11,15 +11,14 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 """Symbolic type base."""
 
 import abc
 import copy
-import dataclasses
 import enum
 import inspect
 import json
 import re
 import sys
 import typing
 from typing import Any, Callable, Dict, Iterator, List, Optional, Tuple, Type, Union
@@ -110,133 +109,80 @@
   # Returning only the immediate matched descendants.
   IMMEDIATE = 1
 
   # Returning only the leaf matched descendants.
   LEAF = 2
 
 
-@dataclasses.dataclass
-class GetAttributeContext:
-  """The context for computing a contextual value.
-
-  Attributes:
-    key: The key of symbolic attribute to request value.
-    container: An optional symbolic object as the current container to retrieve
-      the contextual value. If None, it means that there is no further container
-      to search for. Otherwise, it is a parent in the symbolic containing chain
-      for current attempt.
-    owner: The owner of the contextual attribute.
-  """
-
-  key: Union[str, int]
-  container: Optional['Symbolic']
-  owner: 'Symbolic'
-
-
-class ContextualValue(
-    pg_typing.CustomTyping,
-    object_utils.JSONConvertible,
-    object_utils.Formattable,
-):
-  """Base class for contextual value markers.
-
-  Contextual value markers allows a symbolic attribute to be late bound
-  based on the entire symbolic tree where current symbolic value is part of.
-  As a result, users could access the late bound values directly through
-  symbolic attributes.
-
-  For example::
+class TopologyAware(metaclass=abc.ABCMeta):
+  """Interface for objects that are aware of the topology it is part of."""
 
-    class A(pg.Object):
-      x: int
-      y: int = pg.ContextualValue()
+  @property
+  @abc.abstractmethod
+  def sym_parent(self) -> Optional['TopologyAware']:
+    """Returns the parent of this object."""
 
-    # Not okay: `x` is not contextual and is not specified.
-    A()
+  @abc.abstractmethod
+  def sym_setparent(self, parent: Optional['TopologyAware']) -> None:
+    """Sets the parent of this object."""
 
-    # Okay: both `x` and `y` are specified.
-    A(x=1, y=2)
+  @property
+  @abc.abstractmethod
+  def sym_path(self) -> object_utils.KeyPath:
+    """Returns the path of this object under its topology."""
 
-    # Okay: `y` is contextual, hence optional.
-    a = A(x=1)
+  @abc.abstractmethod
+  def sym_setpath(self, path: object_utils.KeyPath) -> None:
+    """Sets the path of this object under its topology."""
 
-    # Raises: `y` is neither specified during __init__
-    # nor provided from the context.
-    a.y
 
-    d = pg.Dict(y=2, z=pg.Dict(a=a))
+class Inferential(TopologyAware, pg_typing.CustomTyping):
+  """Interface for values that could be dynamically inferred upon read.
 
-    # `a.y` now refers to `d.a` since `d` is in its symbolic parent chain,
-    # aka. context.
-    assert a.y == 2
+  Inferential values are objects whose values are not determined directly but
+  are instead derived from other sources, such as references (:class:`pg.Ref`)
+  to other objects or computed based on their context
+  (:class:`pg.symbolic.ValueFromParentChain`) such as the symbolic tree they
+  reside in.
+
+  When inferential values are utilized as symbolic attributes, we can obtain
+  their original definition by invoking :meth:`pg.Symbolic.sym_getattr`, and
+  their inferred values can be retrieved by calling
+  :meth:`pg.Symbolic.sym_inferred`. The values retrieved from :class:`pg.Dict`,
+  :class:`pg.List` and :class:`pg.Object` through `__getitem__` or
+  `__getattribute__` are all inferred values.
   """
 
-  def get(self, context: GetAttributeContext) -> Any:
-    """Try get the contextual value for a symbolic attribute from a parent.
+  @abc.abstractmethod
+  def infer(self, **kwargs) -> Any:
+    """Returns the inferred value.
 
     Args:
-      context: a `GetAttributeContext` object representing curent context.
+      **kwargs: Optional keyword arguments for inference, which are usually
+        inferential subclass specific.
 
     Returns:
-      The value for the requested symbolic attribute from the current context.
-        If ``pg.MISSING_VALUE``, it means that current symbolic parent cannot
-          provide a contextual value for the attribute, so the current context
-          is moved upward, until it reaches to the root of the symbolic tree.
-        If a ``pg.ContextualValue`` object, it will use the new contextual
-          marker returned to resolve its value from its symbolic parent chains.
-    """
-    return self.value_from(context)
-
-  def value_from(self, context: GetAttributeContext) -> Any:
-    """Try get the contextual value for a symbolic attribute from a parent."""
-    if context.container is None:
-      return pg_typing.MISSING_VALUE
-
-    if isinstance(context.key, int):
-      if isinstance(context.container, list):
-        return context.container[context.key]
-      else:
-        return pg_typing.MISSING_VALUE
-    return getattr(context.container, context.key, pg_typing.MISSING_VALUE)
+      Inferred value.
 
-  def custom_apply(self, *args, **kwargs: Any) -> Tuple[bool, Any]:
-    # This is to make a ``ContextualValue`` object assignable
-    # to any symbolic attribute.
-    return (False, self)
-
-  def format(
-      self,
-      compact: bool = False,
-      verbose: bool = True,
-      root_indent: int = 0,
-      **kwargs: Any,
-  ) -> str:
-    del compact, verbose, root_indent, kwargs
-    return 'ContextualValue()'
-
-  def to_json(self, **kwargs: Any) -> Dict[str, Any]:
-    return self.to_json_dict({})
-
-  def __eq__(self, other: Any) -> bool:
-    # NOTE(daiyip): We do strict type match here since subclasses might
-    # have their own __eq__ logic.
-    return type(other) is ContextualValue  # pylint: disable=unidiomatic-typecheck
-
-  def __ne__(self, other: Any) -> bool:
-    return not self.__eq__(other)
+    Raises:
+      AttributeError: If the value cannot be inferred.
+    """
 
 
 # Value marker for raising errors if a attribute does not exist or cannot
 # be computed.
 _RAISE_IF_NOT_FOUND = (pg_typing.MISSING_VALUE,)
 
 
-class Symbolic(object_utils.JSONConvertible,
-               object_utils.MaybePartial,
-               object_utils.Formattable):
+class Symbolic(
+    TopologyAware,
+    object_utils.JSONConvertible,
+    object_utils.MaybePartial,
+    object_utils.Formattable,
+):
   """Base for all symbolic types.
 
   Symbolic types are types that provide interfaces for symbolic programming,
   based on which symbolic objects can be created. In PyGlove, there are three
   categories of symbolic types:
 
     * Symbolic classes: Defined by :class:`pyglove.Object` subclasses,
@@ -496,141 +442,65 @@
       return path.get(self, default)
 
   @abc.abstractmethod
   def sym_hasattr(self, key: Union[str, int]) -> bool:
     """Returns if a symbolic attribute exists."""
 
   def sym_getattr(
-      self,
-      key: Union[str, int],
-      default: Any = object_utils.MISSING_VALUE) -> Any:
+      self, key: Union[str, int], default: Any = _RAISE_IF_NOT_FOUND
+  ) -> Any:
     """Gets a symbolic attribute.
 
     Args:
       key: Key of symbolic attribute.
       default: Default value if attribute does not exist. If absent,
 
     Returns:
       Value of symbolic attribute if found, otherwise the default value
       if it's specified.
 
     Raises:
-      AttributeError if `key` does not exist and `default` is
-        ``pg.MISSING_VALUE``.
+      AttributeError if `key` does not exist and `default` is not provided.
     """
     if not self.sym_hasattr(key):
-      if default != object_utils.MISSING_VALUE:
-        return default
-      raise AttributeError(
-          self._error_message(
-              f'{self.__class__!r} object has no symbolic attribute {key!r}.'))
+      if default is _RAISE_IF_NOT_FOUND:
+        raise AttributeError(
+            self._error_message(
+                f'{self.__class__!r} object has no symbolic attribute {key!r}.'
+            )
+        )
+      return default
     return self._sym_getattr(key)
 
-  def sym_contextual_hasattr(
-      self,
-      key: Union[str, int],
-      getter: Optional[ContextualValue] = None,
-      start: Union[
-          'Symbolic', object_utils.MissingValue
-      ] = pg_typing.MISSING_VALUE,
-  ) -> bool:
-    """Returns True if an attribute exists from current object's context.
-
-    Args:
-      key: Key of symbolic attribute.
-      getter: An optional ``ContextualValue`` object as the value retriever.
-      start: An object from current object to the root of the composition as the
-        starting point of context lookup (upward). If ``pg.MISSING_VALUE``, it
-        will start with current node.
-
-    Returns:
-      True if the attribute exists. Otherwise False.
-    """
-    getter = getter or ContextualValue()
-    v = self.sym_contextual_getattr(
-        key, default=pg_typing.MISSING_VALUE, getter=getter, start=start
+  def sym_inferrable(self, key: Union[str, int], **kwargs) -> bool:
+    """Returns True if the attribute under key can be inferred."""
+    return (
+        self.sym_inferred(key, pg_typing.MISSING_VALUE, **kwargs)
+        != pg_typing.MISSING_VALUE
     )
-    return v != pg_typing.MISSING_VALUE
 
-  def sym_contextual_getattr(
+  def sym_inferred(
       self,
       key: Union[str, int],
-      default: Any = (object_utils.MISSING_VALUE,),
-      getter: Optional[ContextualValue] = None,
-      start: Union[
-          'Symbolic', object_utils.MissingValue
-      ] = pg_typing.MISSING_VALUE,
+      default: Any = _RAISE_IF_NOT_FOUND,
+      **kwargs,
   ) -> Any:
-    """Gets a key from current object's context (symbolic parent chain).
-
-    Args:
-      key: Key of symbolic attribute.
-      default: Default value if attribute does not exist. If absent,
-        `AttributeError` will be thrown.
-      getter: An optional ``ContextualValue`` object as the value retriever.
-      start: An object from current object to the root of the composition as the
-        starting point of context lookup (upward). If ``pg.MISSING_VALUE``, it
-        will start with current node.
-
-    Returns:
-      Value of symbolic attribute if found, otherwise the default value
-      if it's specified.
-
-    Raises:
-      AttributeError if `key` does not exist along the parent chain and
-        default value is not ``pg.MISSING_VALUE``.
-    """
-    getter = getter or ContextualValue()
-    if start == pg_typing.MISSING_VALUE:
-      current = self
+    """Returns the inferred value of the attribute under key."""
+    if default is _RAISE_IF_NOT_FOUND:
+      return self._sym_inferred(key, **kwargs)
     else:
-      current = typing.cast(Symbolic, start)
-
-    while True:
-      context = GetAttributeContext(key=key, container=current, owner=self)
-      v = getter.get(context)
-      # NOTE(daiyip): when the ContextualValue value from the parent returns
-      # another ContextualValue object, we should follow the new return value's
-      # instruction instead of the original one.
-      if isinstance(v, ContextualValue):
-        getter = v
-      elif v != object_utils.MISSING_VALUE:
-        return v
-
-      if current is not None:
-        current = current.sym_parent
-      else:
-        break
-
-    if default != (object_utils.MISSING_VALUE,):
-      return default
-    raise AttributeError(
-        self._error_message(
-            f'`{key}` is not found under its context '
-            '(along its symbolic parent chain).'
-        )
-    )
-
-  def sym_value(
-      self, key: Union[str, int], default: Any = _RAISE_IF_NOT_FOUND
-  ) -> Any:
-    """Gets the value of a symbolic attribute (with resolving ContextualValue).
-
-    Args:
-      key: The key of the symbolic attribute.
-      default: The default value if the key does not exist or contextual value
-        cannot be resolved. If not specified, attribute error will be risen.
+      try:
+        return self._sym_inferred(key, **kwargs)
+      except Exception:  # pylint: disable=broad-exception-caught
+        return default
 
-    Returns:
-      The value of the symbolic attribute after resolving the
-        ``pg.ContextualValue``.
-    """
-    v = self._sym_value(key, default)
-    if v is _RAISE_IF_NOT_FOUND:
-      raise AttributeError(key)
+  def _sym_inferred(self, key: Union[str, int], **kwargs) -> Any:
+    v = self.sym_getattr(key)
+    if isinstance(v, Inferential):
+      v = v.infer(**kwargs)
     return v
 
   @abc.abstractmethod
   def sym_keys(self) -> Iterator[Union[str, int]]:
     """Iterates the keys of symbolic attributes."""
 
   @abc.abstractmethod
@@ -1189,28 +1059,14 @@
     return self.sym_clone(deep=True, memo=memo)
 
   #
   # Proteted methods to implement from subclasses
   #
 
   @abc.abstractmethod
-  def _sym_value(self, key: Union[str, int], default: Any) -> Any:
-    """Gets the value of a symbolic attribute (with resolving ContextualValue).
-
-    Args:
-      key: The key of the symbolic attribute.
-      default: The default value if the key does not exist or contextual value
-        cannot be resolved.
-
-    Returns:
-      The value of the symbolic attribute after resolving the
-        ``pg.ContextualValue``.
-    """
-
-  @abc.abstractmethod
   def _sym_rebind(
       self, path_value_pairs: Dict[object_utils.KeyPath, Any]
       ) -> List[FieldUpdate]:
     """Subclass specific rebind implementation.
 
     Args:
       path_value_pairs: A dictionary of key path to new field value.
@@ -1310,25 +1166,25 @@
       # object tree, this prevents it from having multiple parents. See
       # List._formalized_value for similar logic.
       root_path = object_utils.KeyPath(key, self.sym_path)
       if (value.sym_parent is not None and
           (value.sym_parent is not self
            or root_path != value.sym_path)):
         value = value.clone()
-      value.sym_setpath(root_path)
-      # NOTE(daiyip): Dict may set '_pass_through_parent' member to True when
-      # it's used as the field container of an Object.
-      if getattr(self, '_pass_through_parent', False):
-        parent = self.sym_parent
-      else:
-        parent = self
-      value.sym_setparent(parent)
       value.set_accessor_writable(self.accessor_writable)
+
+    if isinstance(value, TopologyAware):
+      value.sym_setpath(object_utils.KeyPath(key, self.sym_path))
+      value.sym_setparent(self._sym_parent_for_children())
     return value
 
+  def _sym_parent_for_children(self) -> Optional['Symbolic']:
+    """Returns the symbolic parent for children."""
+    return self
+
   def _set_item_of_current_tree(
       self, path: object_utils.KeyPath, value: Any) -> Optional[FieldUpdate]:
     """Set a field of current tree by key path and return its parent."""
     assert isinstance(path, object_utils.KeyPath), path
     if not path:
       raise KeyError(
           self._error_message(
@@ -1701,15 +1557,15 @@
         return False
     return True
   elif isinstance(left, dict):
     if (not isinstance(right, dict)
         or len(left) != len(right)
         or set(left.keys()) != set(right.keys())):
       return False
-    # NOTE(daiyip): pg.Dict.__getitem__ will trigger contextual value
+    # NOTE(daiyip): pg.Dict.__getitem__ will trigger inferred value
     # evaluation, therefore we always get its symbolic form during traversal.
     left_items = left.sym_items if isinstance(left, Symbolic) else left.items
     right_item = (
         right.sym_getattr if isinstance(right, Symbolic) else right.__getitem__)
     for k, v in left_items():
       if ne(v, right_item(k)):
         return False
```

### Comparing `pyglove-0.4.3.dev20230729/pyglove/core/symbolic/base_test.py` & `pyglove-0.4.3.dev20230730/pyglove/core/symbolic/base_test.py`

 * *Files 24% similar despite different names*

```diff
@@ -10,15 +10,14 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 """Tests for pyglove.symbolic.base."""
 
 import copy
-import dataclasses
 import unittest
 
 from pyglove.core import object_utils
 from pyglove.core import typing as pg_typing
 from pyglove.core.symbolic import base
 from pyglove.core.symbolic.dict import Dict
 
@@ -82,58 +81,9 @@
     )
 
     self.assertNotEqual(
         base.FieldUpdate(object_utils.KeyPath('a'), x, f, 1, 2), Dict()
     )
 
 
-class ContextualValueTest(unittest.TestCase):
-  """Tests for `pg.symbolic.ContextualValue`."""
-
-  def test_str(self):
-    self.assertEqual(str(base.ContextualValue()), 'ContextualValue()')
-
-  def test_repr(self):
-    self.assertEqual(repr(base.ContextualValue()), 'ContextualValue()')
-
-  def test_eq(self):
-    self.assertEqual(base.ContextualValue(), base.ContextualValue())
-    self.assertNotEqual(base.ContextualValue(), 1)
-
-  def test_call(self):
-    @dataclasses.dataclass
-    class A:
-      x: int = 1
-      y: int = 2
-
-    self.assertEqual(
-        base.ContextualValue().get(base.GetAttributeContext('x', A(), Dict())),
-        1,
-    )
-    self.assertEqual(
-        base.ContextualValue().get(base.GetAttributeContext(0, [0, 1], Dict())),
-        0,
-    )
-    self.assertEqual(
-        base.ContextualValue().get(base.GetAttributeContext(0, Dict(), Dict())),
-        pg_typing.MISSING_VALUE,
-    )
-
-  def test_custom_typing(self):
-    v = base.ContextualValue()
-    self.assertIs(pg_typing.Int().apply(v), v)
-    self.assertIs(pg_typing.Str().apply(v), v)
-
-  def test_to_json(self):
-    self.assertEqual(
-        base.to_json(base.ContextualValue()),
-        {'_type': f'{base.ContextualValue.__module__}.ContextualValue'},
-    )
-
-  def test_from_json(self):
-    self.assertEqual(
-        base.from_json(base.ContextualValue().to_json()), base.ContextualValue()
-    )
-
-
 if __name__ == '__main__':
   unittest.main()
```

### Comparing `pyglove-0.4.3.dev20230729/pyglove/core/symbolic/boilerplate.py` & `pyglove-0.4.3.dev20230730/pyglove/core/symbolic/boilerplate.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.4.3.dev20230729/pyglove/core/symbolic/boilerplate_test.py` & `pyglove-0.4.3.dev20230730/pyglove/core/symbolic/boilerplate_test.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.4.3.dev20230729/pyglove/core/symbolic/class_wrapper.py` & `pyglove-0.4.3.dev20230730/pyglove/core/symbolic/class_wrapper.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.4.3.dev20230729/pyglove/core/symbolic/class_wrapper_test.py` & `pyglove-0.4.3.dev20230730/pyglove/core/symbolic/class_wrapper_test.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.4.3.dev20230729/pyglove/core/symbolic/compounding.py` & `pyglove-0.4.3.dev20230730/pyglove/core/symbolic/compounding.py`

 * *Files 2% similar despite different names*

```diff
@@ -171,28 +171,28 @@
     @property
     def decomposed(self):
       if self._sym_decomposed is None:
         # Build the compound object.
         self._sym_decomposed = factory_fn(**self.sym_init_args)
 
         # This allows the decomposed symbolic object to access the parent chain
-        # for value retrieval of contextual attributes.
+        # for value retrieval of inferred attributes.
         if isinstance(self._sym_decomposed, Symbolic):
           self._sym_decomposed.sym_setparent(self.sym_parent)
       return self._sym_decomposed
 
     def _on_parent_change(self, old_parent, new_parent):
       """Override to allow decomposed object to follow parent chain change."""
       super()._on_parent_change(old_parent, new_parent)
       if isinstance(self._sym_decomposed, Symbolic):
         self._sym_decomposed.sym_setparent(new_parent)
 
-    def sym_value(self, name: str) -> Any:
-      # Bypass the user base' `sym_value` if it's overriden.
-      return Compound.sym_value(self, name)
+    def _sym_inferred(self, key: str, **kwargs) -> Any:
+      # Bypass the user base' `_sym_inferred` if it's overriden.
+      return Compound._sym_inferred(self, key, **kwargs)
 
     def __getattribute__(self, name: str):
       if (
           name.startswith('_')
           or name in _COMPOUND_OWNED_ATTR_NAMES
           or name in self.sym_init_args
       ):
```

### Comparing `pyglove-0.4.3.dev20230729/pyglove/core/symbolic/compounding_test.py` & `pyglove-0.4.3.dev20230730/pyglove/core/symbolic/compounding_test.py`

 * *Files 5% similar despite different names*

```diff
@@ -16,18 +16,18 @@
 import abc
 import dataclasses
 import sys
 import unittest
 
 from pyglove.core import object_utils
 from pyglove.core import typing as pg_typing
-from pyglove.core.symbolic.base import ContextualValue
 from pyglove.core.symbolic.compounding import compound as pg_compound
 from pyglove.core.symbolic.compounding import compound_class as pg_compound_class
 from pyglove.core.symbolic.dict import Dict
+from pyglove.core.symbolic.inferred import ValueFromParentChain
 from pyglove.core.symbolic.object import Object
 
 
 class BasicTest(unittest.TestCase):
 
   def test_basics(self):
     @dataclasses.dataclass
@@ -227,17 +227,17 @@
     def bar():
       return Bar()
 
     b = bar()
     self.assertEqual(b.bar, 1)
     self.assertEqual(b.foo(1), 1)
 
-  def test_contextual_attr_access(self):
+  def test_inferred_value_access(self):
     class Foo(Object):
-      x: int = ContextualValue()
+      x: int = ValueFromParentChain()
 
     @pg_compound(Foo)
     def foo():
       return Foo()
 
     f = foo()
     d = Dict(x=1, y=f)
```

### Comparing `pyglove-0.4.3.dev20230729/pyglove/core/symbolic/contextual.py` & `pyglove-0.4.3.dev20230730/pyglove/core/tuning/early_stopping.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,53 +1,64 @@
-# Copyright 2023 The PyGlove Authors
+# Copyright 2022 The PyGlove Authors
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #      http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
-"""Customizable contextual value markers."""
-from typing import Any
-from pyglove.core.symbolic import base
-from pyglove.core.symbolic import functor
-
-
-class ContextualGetter(functor.Functor, base.ContextualValue):
-  """Base for functor-based contextual getter."""
-
-  def value_from(self, context: base.GetAttributeContext) -> Any:
-    return self.__call__(context)
-
-
-def contextual_getter(args=None, returns=None, **kwargs):
-  """Decorator that makes ContextualGetter class from function.
-
-  Examples::
-
-    @pg.contextual_getter
-    def static_value(self, name, context, value):
-      return value
-
-    class A(pg.Object):
-      x: pg.ContextualValue = static_value(value=1)
-
-  Args:
-    args: A list of tuples that defines the schema for function arguments.
-      Please see `functor_class` for detailed explanation of `args`. If None, it
-      will be inferenced from the function argument annotations.
-    returns: Optional value spec for return value. If None, it will be inferred
-      from the function return value annotation.
-    **kwargs: Additional keyword argments for controlling the behavior of
-      functor creation. Please refer to :func:`pg.symbolic.functor_class` for
-      more details.
-
-  Returns:
-    A function that converts a regular function into a ``pg.ContextualGetter``
-      subclass.
-  """
-  return functor.functor(args, returns, base_class=ContextualGetter, **kwargs)
+"""Interface for early stopping policies."""
+
+import abc
+from typing import Iterable, Optional
+
+from pyglove.core import geno
+from pyglove.core import symbolic
+from pyglove.core.tuning.protocols import Trial
+
+
+class EarlyStoppingPolicy(symbolic.Object):
+  """Interface for early stopping policy."""
+
+  def setup(self, dna_spec: geno.DNASpec) -> None:
+    """Setup states of an early stopping policy based on dna_spec.
+
+    Args:
+      dna_spec: DNASpec for DNA to propose.
+
+    Raises:
+      RuntimeError: if dna_spec is not supported.
+    """
+    self._dna_spec = dna_spec
+
+  @property
+  def dna_spec(self) -> Optional[geno.DNASpec]:
+    return getattr(self, '_dna_spec', None)
+
+  @abc.abstractmethod
+  def should_stop_early(self, trial: Trial) -> bool:
+    """Should stop the input trial early based on its measurements."""
+
+  def recover(self, history: Iterable[Trial]) -> None:
+    """Recover states by replaying the trial history.
+
+    Subclass can override.
+
+    NOTE: `recover` will always be called before the first `should_stop_early`
+    is called. It could be called multiple times if there are multiple source
+    of history, e.g: trials from a previous study and existing trials from
+    current study.
+
+    The default behavior is to replay `should_stop_early` on all intermediate
+    measurements on all trials.
+
+    Args:
+      history: An iterable object of trials.
+    """
+    for trial in history:
+      if trial.status in ['COMPLETED', 'PENDING', 'STOPPING']:
+        self.should_stop_early(trial)
```

### Comparing `pyglove-0.4.3.dev20230729/pyglove/core/symbolic/contextual_test.py` & `pyglove-0.4.3.dev20230730/pyglove/core/symbolic/inferred_test.py`

 * *Files 21% similar despite different names*

```diff
@@ -7,35 +7,34 @@
 #      http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
-"""Tests for pyglove.symbolic.ContextualGetter."""
+"""Tests for pyglove.symbolic.inferred."""
 
 import unittest
 
-from pyglove.core.symbolic import base
-from pyglove.core.symbolic import contextual
+from pyglove.core import typing as pg_typing
+from pyglove.core.symbolic import inferred
 from pyglove.core.symbolic.dict import Dict
 
 
-class ContextualGetterTest(unittest.TestCase):
-  """Tests for `pg.symbolic.ContextualGetter`."""
+class ValueFromParentChain(unittest.TestCase):
+  """Tests for `pg.symbolic.ValueFromParentChain`."""
 
-  def test_basics(self):
-    @contextual.contextual_getter
-    def static_value(context, v):
-      del context
-      return v
-
-    getter = static_value(v=1)  # pylint: disable=no-value-for-parameter
-    self.assertIsInstance(getter, base.ContextualValue)
-    self.assertEqual(
-        getter.get(base.GetAttributeContext('x', Dict(), Dict())), 1
-    )
-    self.assertEqual(base.from_json(base.to_json(getter)), getter)
+  def test_inference(self):
+    v = Dict(y=1, x=Dict(x=1, y=inferred.ValueFromParentChain()))
+    self.assertEqual(v.x.y, 1)
+
+    v.rebind(y=2)
+    self.assertEqual(v.x.y, 2)
+
+  def test_custom_typing(self):
+    v = inferred.ValueFromParentChain()
+    self.assertIs(pg_typing.Int().apply(v), v)
+    self.assertIs(pg_typing.Str().apply(v), v)
 
 
 if __name__ == '__main__':
   unittest.main()
```

### Comparing `pyglove-0.4.3.dev20230729/pyglove/core/symbolic/dict.py` & `pyglove-0.4.3.dev20230730/pyglove/core/symbolic/dict.py`

 * *Files 2% similar despite different names*

```diff
@@ -323,14 +323,19 @@
           allow_partial=base.accepts_partial(self),
           child_transform=base.symbolic_transform_fn(self._allow_partial),
           root_path=self.sym_path)
     else:
       self._value_spec = value_spec
     return self
 
+  def _sym_parent_for_children(self) -> Optional[base.Symbolic]:
+    if self._as_object_attributes_container:
+      return self.sym_parent
+    return self
+
   def _sym_rebind(
       self, path_value_pairs: typing.Dict[object_utils.KeyPath, Any]
       ) -> List[base.FieldUpdate]:
     """Subclass specific rebind implementation."""
     updates = []
     for k, v in path_value_pairs.items():
       update = self._set_item_of_current_tree(k, v)
@@ -460,15 +465,15 @@
   def sym_setparent(self, parent: base.Symbolic):
     """Override set parent of Dict to handle the passing through scenario."""
     super().sym_setparent(parent)
     # NOTE(daiyip): when flag `as_object_attributes_container` is on, it sets
     # the parent of child symbolic values using its parent.
     if self._as_object_attributes_container:
       for v in self.sym_values():
-        if isinstance(v, base.Symbolic):
+        if isinstance(v, base.TopologyAware):
           v.sym_setparent(parent)
 
   def sym_hash(self) -> int:
     """Symbolic hashing."""
     return base.sym_hash(
         (self.__class__,
          tuple([base.sym_hash((k, v)) for k, v in self.sym_items()
@@ -501,15 +506,15 @@
   def _update_children_paths(
       self,
       old_path: object_utils.KeyPath,
       new_path: object_utils.KeyPath) -> None:
     """Update children paths according to root_path of current node."""
     del old_path
     for k, v in self.sym_items():
-      if isinstance(v, base.Symbolic):
+      if isinstance(v, base.TopologyAware):
         v.sym_setpath(object_utils.KeyPath(k, new_path))
 
   def _set_item_without_permission_check(  # pytype: disable=signature-mismatch  # overriding-parameter-type-checks
       self, key: str, value: Any) -> Optional[base.FieldUpdate]:
     """Set item without permission check."""
     if not isinstance(key, str):
       raise KeyError(self._error_message(
@@ -529,15 +534,15 @@
         else:
           container_cls = self.__class__
         raise KeyError(
             self._error_message(
                 f'Key \'{key}\' is not allowed for {container_cls}.'))
 
     # Detach old value from object tree.
-    if isinstance(old_value, base.Symbolic):
+    if isinstance(old_value, base.TopologyAware):
       old_value.sym_setparent(None)
       old_value.sym_setpath(object_utils.KeyPath())
 
     if (pg_typing.MISSING_VALUE == value and
         (not field or isinstance(field.key, pg_typing.NonConstKey))):
       if key in self:
         # Using pg.MISSING_VALUE for deleting keys.
@@ -588,32 +593,14 @@
 
   def _on_change(self, field_updates: typing.Dict[object_utils.KeyPath,
                                                   base.FieldUpdate]):
     """On change event of Dict."""
     if self._onchange_callback:
       self._onchange_callback(field_updates)
 
-  def _sym_value(self, key: str, default: Any) -> Any:  # pytype: disable=signature-mismatch
-    """Evalutes a symbolic attribute with resolving contextual values."""
-    if key not in self:
-      return default
-    v = super().__getitem__(key)
-    if isinstance(v, base.ContextualValue):
-      start = self.sym_parent
-      # NOTE(daiyip): The parent of `pg.Object`'s attribute dict points to
-      # the `pg.Object` instance once it's set up. Here we let the ancester
-      # traversal to bypass `pg.Object` to avoid double entry, which causes
-      # dead loop.
-      if self._as_object_attributes_container and self.sym_parent is not None:
-        start = start.sym_parent
-      v = self.sym_contextual_getattr(
-          key, default=default, getter=v, start=start
-      )
-    return v
-
   def _init_kwargs(self) -> typing.Dict[str, Any]:
     kwargs = super()._init_kwargs()
     if not self._accessor_writable:
       kwargs['accessor_writable'] = False
     if self._onchange_callback is not None:
       kwargs['onchange_callback'] = self._onchange_callback
     # NOTE(daiyip): We do not serialize ValueSpec for now as in most use
@@ -626,18 +613,18 @@
 
   def __setstate__(self, state) -> None:
     """Customizes pickle.load."""
     self.__init__(state['value'], **state['kwargs'])
 
   def __getitem__(self, key: str) -> Any:
     """Get item in this Dict."""
-    v = self.sym_value(key, default=_RAISE_IF_NOT_FOUND)
-    if v is _RAISE_IF_NOT_FOUND:
-      raise KeyError(key)
-    return v
+    try:
+      return self.sym_inferred(key)
+    except AttributeError as e:
+      raise KeyError(key) from e
 
   def __setitem__(self, key: str, value: Any) -> None:
     """Set item in this Dict.
 
     Args:
       key: String key. (Please be noted that key path is not supported.)
       value: Value to be inserted.
@@ -724,15 +711,15 @@
   def __delattr__(self, name: str) -> None:
     """Delete an attribute."""
     del self[name]
 
   def __getattr__(self, name: str) -> Any:
     """Get attribute that is not defined as property."""
     if name in self:
-      return self[name]
+      return self.sym_inferred(name)
     raise AttributeError(
         f'Attribute \'{name}\' does not exist in {self.__class__!r}.')
 
   def __iter__(self):
     """Iterate keys in field declaration order."""
     return self.sym_keys()
```

### Comparing `pyglove-0.4.3.dev20230729/pyglove/core/symbolic/dict_test.py` & `pyglove-0.4.3.dev20230730/pyglove/core/symbolic/dict_test.py`

 * *Files 4% similar despite different names*

```diff
@@ -18,16 +18,16 @@
 import io
 import pickle
 import unittest
 
 from pyglove.core import object_utils
 from pyglove.core import typing as pg_typing
 from pyglove.core.symbolic import base
-from pyglove.core.symbolic import contextual
 from pyglove.core.symbolic import flags
+from pyglove.core.symbolic import inferred
 from pyglove.core.symbolic import object as pg_object
 from pyglove.core.symbolic.dict import Dict
 from pyglove.core.symbolic.list import List
 from pyglove.core.symbolic.pure_symbolic import NonDeterministic
 from pyglove.core.symbolic.pure_symbolic import PureSymbolic
 
 
@@ -65,17 +65,17 @@
 
     # Schematized dict.
     vs = pg_typing.Dict([('a', pg_typing.Int())])
     sd = Dict(a=1, value_spec=vs)
     self.assertIs(sd.value_spec, vs)
     self.assertEqual(sd, dict(a=1))
 
-    # Dict with contextual value
-    sd = Dict(Dict(x=base.ContextualValue()))
-    self.assertEqual(sd, dict(x=base.ContextualValue()))
+    # Dict with inferred value
+    sd = Dict(Dict(x=inferred.ValueFromParentChain()))
+    self.assertEqual(sd, dict(x=inferred.ValueFromParentChain()))
 
     with self.assertRaisesRegex(
         ValueError, 'Required value is not specified.'):
       Dict(value_spec=vs)
 
     # Schematized dict with default value.
     vs = pg_typing.Dict([('a', pg_typing.Int(default=0))])
@@ -326,27 +326,27 @@
     self.assertEqual(sd, dict(a=1))
     sd['x1'] = 2
     sd['x2'] = 3
     self.assertEqual(sd, dict(a=1, x1=2, x2=3))
     with self.assertRaisesRegex(KeyError, 'Key \'y1\' is not allowed'):
       sd['y1'] = 4
 
-    # Set item with a contextual value.
+    # Set item with an inferred value.
     sd = Dict(x=1)
-    sd.x = base.ContextualValue()
-    self.assertEqual(sd.sym_getattr('x'), base.ContextualValue())
+    sd.x = inferred.ValueFromParentChain()
+    self.assertEqual(sd.sym_getattr('x'), inferred.ValueFromParentChain())
 
   def test_getitem(self):
     sd = Dict(a=1)
     self.assertEqual(sd['a'], 1)
     with self.assertRaisesRegex(KeyError, 'x'):
       _ = sd['x']
 
-    sd = Dict(x=base.ContextualValue())
-    with self.assertRaisesRegex(AttributeError, 'x'):
+    sd = Dict(x=inferred.ValueFromParentChain())
+    with self.assertRaisesRegex(KeyError, 'x'):
       _ = sd['x']
 
     sdd = Dict(x=Dict(foo=0), y=sd)
     self.assertIs(sd['x'], sdd['x'])
 
   def test_delitem(self):
     # Delete an item from a schemaless dict.
@@ -419,16 +419,16 @@
 
   def test_getattr(self):
     sd = Dict(a=1)
     self.assertEqual(sd.a, 1)
     with self.assertRaisesRegex(AttributeError, 'Attribute .* does not exist'):
       _ = sd.x
 
-    # Test contextual.
-    sd = Dict(x=base.ContextualValue())
+    # Test inferred value.
+    sd = Dict(x=inferred.ValueFromParentChain())
     with self.assertRaisesRegex(
         AttributeError, '`x` is not found under its context'
     ):
       _ = sd.x
 
     p = Dict(x=Dict(p='foo'), y=Dict(z=sd))
     self.assertEqual(sd.x, Dict(p='foo'))
@@ -617,18 +617,18 @@
     with self.assertRaisesRegex(KeyError, 'Key .* is not allowed'):
       sd.setdefault('y', 1)
 
     sd = Dict.partial(value_spec=pg_typing.Dict([('a', pg_typing.Int())]))
     self.assertEqual(sd.setdefault('a', 1), 1)
 
     sd = Dict()
-    sd.setdefault('x', base.ContextualValue())
-    self.assertEqual(sd.sym_getattr('x'), base.ContextualValue())
+    sd.setdefault('x', inferred.ValueFromParentChain())
+    self.assertEqual(sd.sym_getattr('x'), inferred.ValueFromParentChain())
     sd.setdefault('x', 1)
-    self.assertEqual(sd.sym_getattr('x'), base.ContextualValue())
+    self.assertEqual(sd.sym_getattr('x'), inferred.ValueFromParentChain())
 
   def test_update(self):
     sd = Dict(b=0, a=1, c=2)
     with flags.as_sealed():
       with self.assertRaisesRegex(
           base.WritePermissionError, 'Cannot rebind key .* of sealed Dict'):
         sd.update(a=1)
@@ -817,28 +817,27 @@
     self.assertEqual(sd.sym_getattr('x'), 1)
     self.assertIsNone(sd.sym_getattr('a', None))
     with self.assertRaisesRegex(
         AttributeError,
         '.* object has no symbolic attribute \'a\'.'):
       sd.sym_getattr('a')
 
-    sd = Dict(x=base.ContextualValue())
-    self.assertEqual(sd.sym_getattr('x'), base.ContextualValue())
-
-  def test_sym_value(self):
-    @contextual.contextual_getter
-    def static_value(context, v):
-      del context
-      return v
+    sd = Dict(x=inferred.ValueFromParentChain())
+    self.assertEqual(sd.sym_getattr('x'), inferred.ValueFromParentChain())
 
-    sd = Dict(x=1, y=static_value(v=0))  # pylint: disable=no-value-for-parameter
-    self.assertEqual(sd.sym_value('x'), 1)
-    self.assertEqual(sd.sym_value('y'), 0)
+  def test_sym_inferred(self):
+    sd = Dict(x=1, y=inferred.ValueFromParentChain())  # pylint: disable=no-value-for-parameter
+    self.assertEqual(sd.sym_inferred('x'), 1)
+    with self.assertRaisesRegex(AttributeError, 'y'):
+      _ = sd.sym_inferred('y')
     with self.assertRaisesRegex(AttributeError, 'z'):
-      _ = sd.sym_value('z')
+      _ = sd.sym_inferred('z')
+
+    sd = Dict(y=1, x=Dict(x=Dict(y=inferred.ValueFromParentChain())))
+    self.assertEqual(sd.x.x.y, 1)
 
   def test_sym_field(self):
     sd = Dict(x=1, y=Dict(z=2))
     self.assertIsNone(sd.sym_field)
 
     spec = pg_typing.Dict([
         ('x', pg_typing.Int()),
@@ -866,55 +865,58 @@
 
     sd = Dict(x=1, z=3, y=2, value_spec=pg_typing.Dict([
         (pg_typing.StrKey(), pg_typing.Int())
     ]))
     self.assertEqual(next(sd.sym_keys()), 'x')
     self.assertEqual(list(sd.sym_keys()), ['x', 'z', 'y'])
 
-    sd = Dict(x=1, y=base.ContextualValue())
+    sd = Dict(x=1, y=inferred.ValueFromParentChain())
     self.assertEqual(next(sd.sym_keys()), 'x')
     self.assertEqual(list(sd.sym_keys()), ['x', 'y'])
 
   def test_sym_values(self):
     sd = Dict(x=1, y=2)
     self.assertEqual(next(sd.sym_values()), 1)
     self.assertEqual(list(sd.sym_values()), [1, 2])
 
     sd = Dict(x=1, z=3, y=2, value_spec=pg_typing.Dict([
         (pg_typing.StrKey(), pg_typing.Int())
     ]))
     self.assertEqual(next(sd.sym_values()), 1)
     self.assertEqual(list(sd.sym_values()), [1, 3, 2])
 
-    sd = Dict(x=1, y=base.ContextualValue())
+    sd = Dict(x=1, y=inferred.ValueFromParentChain())
     self.assertEqual(next(sd.sym_values()), 1)
-    self.assertEqual(list(sd.sym_values()), [1, base.ContextualValue()])
+    self.assertEqual(
+        list(sd.sym_values()), [1, inferred.ValueFromParentChain()]
+    )
 
   def test_sym_items(self):
     sd = Dict(x=1, y=2)
     self.assertEqual(next(sd.sym_items()), ('x', 1))
     self.assertEqual(list(sd.sym_items()), [('x', 1), ('y', 2)])
 
     sd = Dict(x=1, z=3, y=2, value_spec=pg_typing.Dict([
         (pg_typing.StrKey(), pg_typing.Int())
     ]))
     self.assertEqual(next(sd.sym_items()), ('x', 1))
     self.assertEqual(list(sd.sym_items()), [('x', 1), ('z', 3), ('y', 2)])
 
-    sd = Dict(x=1, y=base.ContextualValue())
+    sd = Dict(x=1, y=inferred.ValueFromParentChain())
     self.assertEqual(next(sd.sym_items()), ('x', 1))
     self.assertEqual(
-        list(sd.sym_items()), [('x', 1), ('y', base.ContextualValue())]
+        list(sd.sym_items()), [('x', 1), ('y', inferred.ValueFromParentChain())]
     )
 
   def test_sym_jsonify(self):
     # Refer to SerializationTest for more detailed tests.
-    sd = Dict(x=1, y=base.ContextualValue())
+    sd = Dict(x=1, y=inferred.ValueFromParentChain())
     self.assertEqual(
-        sd.sym_jsonify(), {'x': 1, 'y': base.ContextualValue().to_json()}
+        sd.sym_jsonify(),
+        {'x': 1, 'y': inferred.ValueFromParentChain().to_json()},
     )
 
   def test_sym_rebind(self):
     # Refer to RebindTest for more detailed tests.
     sd = Dict(x=1, y=2)
     sd.sym_rebind(x=2)
     self.assertEqual(sd, dict(x=2, y=2))
@@ -972,17 +974,17 @@
     # Refer to `test_missing_values` for more details.
     sd = Dict.partial(x=1, value_spec=pg_typing.Dict([
         ('x', pg_typing.Int()),
         ('y', pg_typing.Int()),
     ]))
     self.assertEqual(sd.sym_missing(), {'y': MISSING_VALUE})
 
-    # Test contextual value as the default value.
+    # Test inferred value as the default value.
     sd = Dict(
-        x=base.ContextualValue(),
+        x=inferred.ValueFromParentChain(),
         value_spec=pg_typing.Dict([
             ('x', pg_typing.Int()),
         ]),
     )
     self.assertEqual(sd.sym_missing(), {})
 
   def test_sym_nondefault(self):
@@ -993,33 +995,35 @@
             ('z', pg_typing.Int(default=1))
         ])),
     ]))
     self.assertEqual(sd.sym_nondefault(), {'x': 1})
     sd.rebind({'y.z': 2}, x=0)
     self.assertEqual(sd.sym_nondefault(), {'y.z': 2})
 
-    # Test contextual value as the default value.
+    # Test inferred value as the default value.
     sd = Dict(
         x=1,
         value_spec=pg_typing.Dict([
-            ('x', pg_typing.Int(default=base.ContextualValue())),
+            ('x', pg_typing.Int(default=inferred.ValueFromParentChain())),
         ]),
     )
     self.assertEqual(sd.sym_nondefault(), {'x': 1})
-    sd.rebind(x=base.ContextualValue())
+    sd.rebind(x=inferred.ValueFromParentChain())
     self.assertEqual(sd.sym_nondefault(), {})
 
-    # Test contextual value as the specified value.
+    # Test inferred value as the specified value.
     sd = Dict(
-        x=base.ContextualValue(),
+        x=inferred.ValueFromParentChain(),
         value_spec=pg_typing.Dict([
             ('x', pg_typing.Int(default=1)),
         ]),
     )
-    self.assertEqual(sd.sym_nondefault(), {'x': base.ContextualValue()})
+    self.assertEqual(
+        sd.sym_nondefault(), {'x': inferred.ValueFromParentChain()}
+    )
     sd.rebind(x=1)
     self.assertEqual(sd.sym_nondefault(), {})
 
   def test_sym_puresymbolic(self):
     self.assertFalse(Dict(x=1).sym_puresymbolic)
 
     class A(PureSymbolic):
@@ -1059,16 +1063,20 @@
     self.assertEqual(Dict(), Dict())
     self.assertTrue(Dict().sym_eq(Dict()))
     self.assertTrue(base.eq(Dict(), Dict()))
 
     self.assertEqual(Dict(a=1), Dict(a=1))
     self.assertTrue(Dict(a=1).sym_eq(Dict(a=1)))
     self.assertTrue(base.eq(Dict(a=1), Dict(a=1)))
-    self.assertTrue(base.eq(Dict(x=base.ContextualValue()),
-                            Dict(x=base.ContextualValue())))
+    self.assertTrue(
+        base.eq(
+            Dict(x=inferred.ValueFromParentChain()),
+            Dict(x=inferred.ValueFromParentChain()),
+        )
+    )
     self.assertEqual(
         Dict(a=1),
         Dict(a=1, value_spec=pg_typing.Dict([('a', pg_typing.Int())])))
     self.assertTrue(base.eq(
         Dict(a=1),
         Dict(a=1, value_spec=pg_typing.Dict([('a', pg_typing.Int())]))))
     self.assertEqual(Dict(a=Dict()), Dict(a=dict()))
@@ -1297,21 +1305,21 @@
 
       with self.assertRaisesRegex(
           base.WritePermissionError,
           'Cannot del Dict field by attribute or key while accessor_writable '
           'is set to False.'):
         del sd['a']
 
-    # Test with contextual value.
-    @contextual.contextual_getter
-    def unresolvable(k, p):
-      del k, p
-      return pg_typing.MISSING_VALUE
+    # Test with inferred value.
+    class Unresolvable(inferred.InferredValue):
 
-    sd = Dict(x=unresolvable())  # pylint: disable=no-value-for-parameter
+      def infer(self):
+        raise ValueError()
+
+    sd = Dict(x=Unresolvable())  # pylint: disable=no-value-for-parameter
     sd.set_accessor_writable(False)
     self.assertFalse(sd.sym_getattr('x').accessor_writable)
     with self.assertRaisesRegex(
         base.WritePermissionError,
         'Cannot modify Dict field by attribute or key while '
         'accessor_writable is set to False.',
     ):
@@ -1460,21 +1468,21 @@
     sd = Dict(a=Dict())
     self.assertFalse(sd.is_sealed)
     self.assertFalse(sd.a.is_sealed)
     sd.seal()
     self.assertTrue(sd.is_sealed)
     self.assertTrue(sd.a.is_sealed)
 
-    # Test with contextual value.
-    @contextual.contextual_getter
-    def unresolvable(k, p):
-      del k, p
-      return pg_typing.MISSING_VALUE
+    # Test with inferred value.
+    class Unresolvable(inferred.InferredValue):
+
+      def infer(self):
+        raise ValueError()
 
-    sd = Dict(x=unresolvable())  # pylint: disable=no-value-for-parameter
+    sd = Dict(x=Unresolvable())
     sd.seal()
     self.assertTrue(sd.sym_getattr('x').is_sealed)
     sd.seal(False)
     self.assertFalse(sd.sym_getattr('x').is_sealed)
 
 
 class RebindTest(unittest.TestCase):
@@ -1512,26 +1520,26 @@
     # Rebind using both update dict and kwargs.
     sd = Dict(a=1, b=2, c=3)
     sd.rebind({'a': 2, 'b': 3}, a=3, c=3)
     self.assertEqual(sd, dict(a=3, b=3, c=3))
 
   def test_rebind_with_context_value(self):
     sd = Dict(a=1, b=2)
-    sd.rebind(a=base.ContextualValue())
-    self.assertEqual(sd, dict(a=base.ContextualValue(), b=2))
+    sd.rebind(a=inferred.ValueFromParentChain())
+    self.assertEqual(sd, dict(a=inferred.ValueFromParentChain(), b=2))
 
     sd = Dict(
         a=1,
         b=2,
         value_spec=pg_typing.Dict(
             [('a', pg_typing.Int()), ('b', pg_typing.Int())]
         ),
     )
-    sd.rebind(a=base.ContextualValue())
-    self.assertEqual(sd, dict(a=base.ContextualValue(), b=2))
+    sd.rebind(a=inferred.ValueFromParentChain())
+    self.assertEqual(sd, dict(a=inferred.ValueFromParentChain(), b=2))
 
   def test_rebind_with_typing(self):
     spec = pg_typing.Dict([
         ('a', pg_typing.Int(default=0)),
         ('b', pg_typing.Str(regex='foo.*')),
         ('c', pg_typing.Dict([
             ('x', pg_typing.Int(min_value=1, default=1)),
@@ -1849,15 +1857,15 @@
   def test_from_json(self):
     spec = pg_typing.Dict([
         ('w', pg_typing.Str()),
         ('x', pg_typing.Int()),
         ('y', pg_typing.Str().noneable()),
         # Frozen field shall not be written.
         ('z', pg_typing.Bool(True).freeze()),
-        ('p', pg_typing.Int(default=base.ContextualValue())),
+        ('p', pg_typing.Int(default=inferred.ValueFromParentChain())),
     ])
     self.assertEqual(
         base.from_json_str('{"x": 1}').use_value_spec(spec, allow_partial=True),
         Dict.partial(x=1, value_spec=spec))
 
   def test_to_json_on_regular_dict(self):
     self.assertEqual(
@@ -2051,20 +2059,20 @@
                   )
                 }
               ]
             }
           }
         }"""))
 
-  def test_noncompact_with_contextual_value(self):
+  def test_noncompact_with_inferred_value(self):
     self.assertEqual(
-        Dict(x=1, y=base.ContextualValue()).format(compact=False),
+        Dict(x=1, y=inferred.ValueFromParentChain()).format(compact=False),
         inspect.cleandoc("""{
             x = 1,
-            y = ContextualValue()
+            y = ValueFromParentChain()
           }
         """),
     )
 
 
 def _on_change_callback(updates):
   del updates
```

### Comparing `pyglove-0.4.3.dev20230729/pyglove/core/symbolic/diff.py` & `pyglove-0.4.3.dev20230730/pyglove/core/symbolic/diff.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.4.3.dev20230729/pyglove/core/symbolic/diff_test.py` & `pyglove-0.4.3.dev20230730/pyglove/core/symbolic/diff_test.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.4.3.dev20230729/pyglove/core/symbolic/flags.py` & `pyglove-0.4.3.dev20230730/pyglove/core/symbolic/flags.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.4.3.dev20230729/pyglove/core/symbolic/flags_test.py` & `pyglove-0.4.3.dev20230730/pyglove/core/symbolic/flags_test.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.4.3.dev20230729/pyglove/core/symbolic/functor.py` & `pyglove-0.4.3.dev20230730/pyglove/core/symbolic/functor.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.4.3.dev20230729/pyglove/core/symbolic/functor_test.py` & `pyglove-0.4.3.dev20230730/pyglove/core/symbolic/functor_test.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.4.3.dev20230729/pyglove/core/symbolic/list.py` & `pyglove-0.4.3.dev20230730/pyglove/core/symbolic/list.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,14 +11,15 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 """Symbolic list."""
 
 import dataclasses
 import math
+import numbers
 import typing
 from typing import Any, Callable, Dict, Iterable, Iterator, Optional, Tuple, Union
 from pyglove.core import object_utils
 from pyglove.core import typing as pg_typing
 from pyglove.core.symbolic import base
 from pyglove.core.symbolic import flags
 
@@ -275,15 +276,16 @@
     del key
     if self._value_spec is None:
       return None
     return self._value_spec.element
 
   def sym_hasattr(self, key: Union[str, int]) -> bool:
     """Tests if a symbolic attribute exists."""
-    return isinstance(key, int) and key >= -len(self) and key < len(self)
+    return (isinstance(key, numbers.Integral)
+            and key >= -len(self) and key < len(self))
 
   def sym_keys(self) -> Iterator[int]:
     """Symbolically iterates indices."""
     for i in range(len(self)):
       yield i
 
   def sym_values(self) -> Iterator[Any]:
@@ -386,21 +388,21 @@
   def _update_children_paths(
       self,
       old_path: object_utils.KeyPath,
       new_path: object_utils.KeyPath) -> None:
     """Update children paths according to root_path of current node."""
     del old_path
     for idx, item in self.sym_items():
-      if isinstance(item, base.Symbolic):
+      if isinstance(item, base.TopologyAware):
         item.sym_setpath(object_utils.KeyPath(idx, new_path))
 
   def _set_item_without_permission_check(  # pytype: disable=signature-mismatch  # overriding-parameter-type-checks
       self, key: int, value: Any) -> Optional[base.FieldUpdate]:
     """Set or add an item without permission check."""
-    assert isinstance(key, int), key
+    assert isinstance(key, numbers.Integral), key
     index = key
     if index >= len(self):
       # Appending MISSING_VALUE is considered no-op.
       if value == pg_typing.MISSING_VALUE:
         return None
       index = len(self)
     should_insert = False
@@ -419,15 +421,15 @@
     new_value = self._formalized_value(index, value)
     if index < len(self):
       if should_insert:
         list.insert(self, index, new_value)
       else:
         list.__setitem__(self, index, new_value)
         # Detach old value from object tree.
-        if isinstance(old_value, base.Symbolic):
+        if isinstance(old_value, base.TopologyAware):
           old_value.sym_setparent(None)
     else:
       super().append(new_value)
     return base.FieldUpdate(
         self.sym_path + index, self,
         self._value_spec.element if self._value_spec else None,
         old_value, new_value)
@@ -464,15 +466,15 @@
         keys_to_remove.append(i)
     if keys_to_remove:
       for i in reversed(keys_to_remove):
         list.__delitem__(self, i)
 
     # Update paths for children.
     for idx, item in self.sym_items():
-      if isinstance(item, base.Symbolic) and item.sym_path.key != idx:
+      if isinstance(item, base.TopologyAware) and item.sym_path.key != idx:
         item.sym_setpath(object_utils.KeyPath(idx, self.sym_path))
 
     if self._onchange_callback is not None:
       self._onchange_callback(field_updates)
 
   def _parse_slice(self, index: slice) -> Tuple[int, int, int]:
     start = index.start if index.start is not None else 0
@@ -486,33 +488,14 @@
     stop = min(len(self), stop)
     if stop < 0:
       stop += len(self)
 
     step = index.step if index.step is not None else 1
     return start, stop, step
 
-  def _sym_value(self, key: int, default: Any) -> Any:  # pytype: disable=signature-mismatch
-    try:
-      v = super().__getitem__(key)
-    except IndexError:
-      return default
-
-    def _eval(i, v):
-      if isinstance(v, base.ContextualValue):
-        return self.sym_contextual_getattr(
-            i, default=default, getter=v, start=self.sym_parent
-        )
-      return v
-
-    if isinstance(key, slice):
-      return [
-          _eval(k, v[i]) for i, k in enumerate(range(*self._parse_slice(key)))
-      ]
-    return _eval(key, v)
-
   def _init_kwargs(self) -> typing.Dict[str, Any]:
     kwargs = super()._init_kwargs()
     if not self._accessor_writable:
       kwargs['accessor_writable'] = False
     if self._onchange_callback is not None:
       kwargs['onchange_callback'] = self._onchange_callback
     # NOTE(daiyip): We do not serialize ValueSpec for now as in most use
@@ -525,18 +508,23 @@
 
   def __setstate__(self, state) -> None:
     """Customizes pickle.load."""
     self.__init__(state['value'], **state['kwargs'])
 
   def __getitem__(self, index) -> Any:
     """Gets the item at a given position."""
-    v = self.sym_value(index, _RAISE_IF_NOT_FOUND)
-    if v is _RAISE_IF_NOT_FOUND:
-      raise IndexError('list index out of range')
-    return v
+    if isinstance(index, numbers.Integral):
+      if index < -len(self) or index >= len(self):
+        raise IndexError('list index out of range')
+      return self.sym_inferred(index)
+    elif isinstance(index, slice):
+      return [self[i] for i in range(*self._parse_slice(index))]
+    else:
+      raise TypeError(
+          f'list index must be an integer. Encountered {index!r}.')
 
   def __setitem__(self, index, value: Any) -> None:
     """Set item in this List."""
     if base.treats_as_sealed(self):
       raise base.WritePermissionError(
           self._error_message('Cannot set item for a sealed List.'))
 
@@ -567,15 +555,15 @@
       updates = []
       for i, r in enumerate(replacements):
         update = self._set_item_without_permission_check(start + i * step, r)
         if update is not None:
           updates.append(update)
       if flags.is_change_notification_enabled() and updates:
         self._notify_field_updates(updates)
-    elif isinstance(index, int):
+    elif isinstance(index, numbers.Integral):
       if index < -len(self) or index >= len(self):
         raise IndexError(
             f'list assignment index out of range. '
             f'Length={len(self)}, index={index}')
       update = self._set_item_without_permission_check(index, value)
       if flags.is_change_notification_enabled() and update:
         self._notify_field_updates([update])
@@ -589,15 +577,15 @@
       raise base.WritePermissionError('Cannot delete item from a sealed List.')
 
     if not base.writtable_via_accessors(self):
       raise base.WritePermissionError(
           self._error_message('Cannot delete List item while accessor_writable '
                               'is set to False. '
                               'Use \'rebind\' method instead.'))
-    if not isinstance(index, int):
+    if not isinstance(index, numbers.Integral):
       raise TypeError(
           f'list index must be an integer. Encountered {index!r}.')
 
     if index < -len(self) or index >= len(self):
       raise IndexError(
           f'list index out of range. '
           f'Length={len(self)}, index={index}')
```

### Comparing `pyglove-0.4.3.dev20230729/pyglove/core/symbolic/list_test.py` & `pyglove-0.4.3.dev20230730/pyglove/core/symbolic/list_test.py`

 * *Files 7% similar despite different names*

```diff
@@ -13,21 +13,22 @@
 # limitations under the License.
 """Tests for pyglove.List."""
 
 import copy
 import inspect
 import io
 import pickle
+from typing import Any
 import unittest
 
 from pyglove.core import object_utils
 from pyglove.core import typing as pg_typing
 from pyglove.core.symbolic import base
-from pyglove.core.symbolic import contextual
 from pyglove.core.symbolic import flags
+from pyglove.core.symbolic import inferred
 from pyglove.core.symbolic import object as pg_object
 from pyglove.core.symbolic.dict import Dict
 from pyglove.core.symbolic.list import Insertion
 from pyglove.core.symbolic.list import List
 from pyglove.core.symbolic.pure_symbolic import NonDeterministic
 from pyglove.core.symbolic.pure_symbolic import PureSymbolic
 
@@ -56,17 +57,17 @@
 
     # Schematized list.
     vs = pg_typing.List(pg_typing.Int())
     sl = List([1], value_spec=vs)
     self.assertIs(sl.value_spec, vs)
     self.assertEqual(sl, [1])
 
-    # List with contextual value.
-    sl = List(List([base.ContextualValue()]))
-    self.assertEqual(sl, [base.ContextualValue()])
+    # List with inferred values.
+    sl = List(List([inferred.ValueFromParentChain()]))
+    self.assertEqual(sl, [inferred.ValueFromParentChain()])
 
     with self.assertRaisesRegex(
         TypeError, '.* must be a `pg.typing.List` object.'):
       List(value_spec=pg_typing.Int())
 
   def test_partial(self):
     spec = pg_typing.List(pg_typing.Dict([
@@ -265,22 +266,24 @@
     # Slicing.
     sl = List([0, 1, 2])
     self.assertEqual(sl[:-1], [0, 1])
     self.assertEqual(sl[1:], [1, 2])
     self.assertEqual(sl[:], [0, 1, 2])
 
     # Context value
-    sl = List([base.ContextualValue(), 2, base.ContextualValue()])
+    sl = List(
+        [inferred.ValueFromParentChain(), 2, inferred.ValueFromParentChain()]
+    )
     with self.assertRaises(AttributeError):
       _ = sl[0]
 
     sl2 = List([123, sl, 456])
     self.assertEqual(sl[0], 123)
 
-    # Slicing contextual values.
+    # Slicing inferred values.
     self.assertEqual(sl[1:], [2, 456])
     self.assertEqual(sl[:-1], [123, 2])
     self.assertEqual(sl[::2], [123, 456])
     self.assertEqual(sl[::], [123, 2, 456])
     self.assertEqual(sl[-1:0:-1], [456, 2])
     del sl2
 
@@ -338,32 +341,32 @@
     sl.seal()
     with self.assertRaisesRegex(
         base.WritePermissionError, 'Cannot append element on a sealed List.'):
       sl.append(4)
 
   def test_extend(self):
     sl = List([0, 1])
-    sl.extend([2, base.ContextualValue()])
-    self.assertEqual(sl, [0, 1, 2, base.ContextualValue()])
+    sl.extend([2, inferred.ValueFromParentChain()])
+    self.assertEqual(sl, [0, 1, 2, inferred.ValueFromParentChain()])
 
     sl = List([0, 1], value_spec=pg_typing.List(pg_typing.Int(), max_size=4))
     with self.assertRaisesRegex(
         ValueError,
         'Cannot extend List: the number of elements .* exceeds max size'):
       sl.extend([2, 3, 4])
     self.assertEqual(sl, [0, 1])
     sl.seal()
     with self.assertRaisesRegex(
         base.WritePermissionError, 'Cannot extend a sealed List.'):
       sl.extend([0, 1])
 
   def test_concatenate(self):
-    sl = List([0]) + List([base.ContextualValue()])
+    sl = List([0]) + List([inferred.ValueFromParentChain()])
     self.assertIsInstance(sl, List)
-    self.assertEqual(sl, [0, base.ContextualValue()])
+    self.assertEqual(sl, [0, inferred.ValueFromParentChain()])
 
     spec = pg_typing.List(pg_typing.Int(min_value=0))
     sl = List([0], value_spec=spec) + [1, 2]
     self.assertIsInstance(sl, List)
     self.assertIs(sl.value_spec, spec)
     self.assertEqual(sl, [0, 1, 2])
 
@@ -419,17 +422,17 @@
       sl.remove(2)
 
     sl = List([0, 1], value_spec=pg_typing.List(pg_typing.Int(), min_size=2))
     with self.assertRaisesRegex(
         ValueError, 'Cannot remove item: min size .* is reached'):
       sl.remove(1)
 
-    # Remove contextual value.
-    sl = List([base.ContextualValue()])
-    sl.remove(base.ContextualValue())
+    # Remove inferred value.
+    sl = List([inferred.ValueFromParentChain()])
+    sl.remove(inferred.ValueFromParentChain())
     self.assertEqual(sl, [])
 
   def test_pop(self):
     sl = List([0, 1, 2])
     self.assertEqual(sl.pop(), 2)
     self.assertEqual(sl, [0, 1])
 
@@ -440,19 +443,19 @@
 
     with self.assertRaisesRegex(IndexError, 'pop index out of range'):
       _ = sl.pop(5)
 
     with self.assertRaisesRegex(IndexError, 'pop index out of range'):
       _ = sl.pop(-3)
 
-    # pop with contextual value.
-    sl = List([base.ContextualValue()])
+    # pop with inferred value.
+    sl = List([inferred.ValueFromParentChain()])
     with self.assertRaises(AttributeError):
       sl.pop()
-    self.assertEqual(sl, [base.ContextualValue()])
+    self.assertEqual(sl, [inferred.ValueFromParentChain()])
 
     sl2 = List([23, sl, 45])
     self.assertEqual(len(sl), 1)
     self.assertEqual(sl[0], 23)
     self.assertEqual(sl.pop(), 23)
     self.assertEqual(sl, [])
     del sl2
@@ -502,46 +505,54 @@
   def test_index(self):
     sl = List([0, 1, 2, 1])
     self.assertEqual(sl.index(1), 1)
     with self.assertRaisesRegex(
         ValueError, '3 is not in list'):
       _ = sl.index(3)
 
-    # Index of contextual value is based on its symbolic form.
+    # Index of inferred value is based on its symbolic form.
     # TODO(daiyip): revise the behavior.
-    sl = List([0, base.ContextualValue(), 1])
-    self.assertEqual(sl.index(base.ContextualValue()), 1)
+    sl = List([0, inferred.ValueFromParentChain(), 1])
+    self.assertEqual(sl.index(inferred.ValueFromParentChain()), 1)
     self.assertEqual(sl.index(1), 2)
 
   def test_count(self):
-    # Count of contextual value is also based on its symbolic form.
+    # Count of inferred value is also based on its symbolic form.
     # TODO(daiyip): revise the behavior.
-    sl = List([0, 1, base.ContextualValue(), 2, 1, base.ContextualValue()])
+    sl = List([
+        0,
+        1,
+        inferred.ValueFromParentChain(),
+        2,
+        1,
+        inferred.ValueFromParentChain(),
+    ])
     self.assertEqual(sl.count(1), 2)
     self.assertEqual(sl.count(3), 0)
-    self.assertEqual(sl.count(base.ContextualValue()), 2)
+    self.assertEqual(sl.count(inferred.ValueFromParentChain()), 2)
 
   def test_copy(self):
 
     class A:
       pass
 
-    sl = List([base.ContextualValue(), A(), dict(x=A()), list([A()])])
+    sl = List([inferred.ValueFromParentChain(), A(), dict(x=A()), list([A()])])
     sl2 = sl.copy()
     self.assertIsInstance(sl2, List)
     self.assertEqual(sl, sl2)
     self.assertIsNot(sl, sl2)
     self.assertIs(sl[1], sl2[1])
     self.assertIsNot(sl[2], sl2[2])
     self.assertIsNot(sl[3], sl2[3])
     self.assertIs(sl[2].x, sl2[2].x)
     self.assertIs(sl[3][0], sl2[3][0])
 
     sl = List(
-        [base.ContextualValue()], value_spec=pg_typing.List(pg_typing.Int())
+        [inferred.ValueFromParentChain()],
+        value_spec=pg_typing.List(pg_typing.Int()),
     )
     sl2 = sl.copy()
     self.assertIs(sl.value_spec, sl2.value_spec)
 
     # Test copy.copy.
     sl = List([0, A(), dict(x=A()), list([A()])])
     sl3 = copy.copy(sl)
@@ -560,15 +571,17 @@
 
       def __init__(self, v):
         self.v = v
 
       def __eq__(self, other):
         return isinstance(other, B) and self.v == other.v
 
-    sl = List([base.ContextualValue(), B(1), dict(x=B(2)), list([B(3)])])
+    sl = List(
+        [inferred.ValueFromParentChain(), B(1), dict(x=B(2)), list([B(3)])]
+    )
     sl4 = copy.deepcopy(sl)
     self.assertIsInstance(sl4, List)
     self.assertEqual(sl, sl4)
     self.assertIsNot(sl, sl4)
     self.assertIsNot(sl[1], sl4[1])
     self.assertIsNot(sl[2], sl4[2])
     self.assertIsNot(sl[3], sl4[3])
@@ -582,40 +595,40 @@
 
     sl.append(-1)
     sl.seal()
     with self.assertRaisesRegex(
         base.WritePermissionError, 'Cannot sort a sealed List'):
       sl.sort()
 
-    # List with contextual value cannot be sorted.
-    sl = List([0, 2, base.ContextualValue(), 3])
+    # List with inferred value cannot be sorted.
+    sl = List([0, 2, inferred.ValueFromParentChain(), 3])
     with self.assertRaises(TypeError):
       sl.sort()
 
   def test_reverse(self):
     sl = List([0, 2, 1, 3])
     sl.reverse()
     self.assertEqual(sl, [3, 1, 2, 0])
 
     sl.seal()
     with self.assertRaisesRegex(
         base.WritePermissionError, 'Cannot reverse a sealed List'):
       sl.reverse()
 
-    # List with contextual value is reversed in its symbolic form.
-    sl = List([0, 2, base.ContextualValue(), 3])
+    # List with inferred value is reversed in its symbolic form.
+    sl = List([0, 2, inferred.ValueFromParentChain(), 3])
     sl.reverse()
-    self.assertEqual(sl, [3, base.ContextualValue(), 2, 0])
+    self.assertEqual(sl, [3, inferred.ValueFromParentChain(), 2, 0])
 
   def test_in(self):
-    sl = List([0, 1, base.ContextualValue()])
+    sl = List([0, 1, inferred.ValueFromParentChain()])
     self.assertIn(1, sl)
     self.assertNotIn(3, sl)
     # In-test is based on the symbolic form.
-    self.assertIn(base.ContextualValue(), sl)
+    self.assertIn(inferred.ValueFromParentChain(), sl)
 
   def test_iter(self):
     sl = List([0, 1, 2, 3])
     self.assertEqual(list(sl), [0, 1, 2, 3])
 
   def test_non_default(self):
     sl = List([0])
@@ -691,25 +704,26 @@
     self.assertIsNone(sl.sym_getattr(1, None))
     self.assertIsNone(sl.sym_getattr('x', None))
     with self.assertRaisesRegex(
         AttributeError,
         '.* object has no symbolic attribute 1.'):
       sl.sym_getattr(1)
 
-  def test_sym_value(self):
-    @contextual.contextual_getter
-    def static_value(context, v):
-      del context
-      return v
-
-    sd = List([1, static_value(v=0)])  # pylint: disable=no-value-for-parameter
-    self.assertEqual(sd.sym_value(0), 1)
-    self.assertEqual(sd.sym_value(1), 0)
+  def test_sym_inferred(self):
+    class StaticValue(inferred.InferredValue):
+      v: Any
+
+      def infer(self):
+        return self.v
+
+    sd = List([1, StaticValue(0)])  # pylint: disable=no-value-for-parameter
+    self.assertEqual(sd.sym_inferred(0), 1)
+    self.assertEqual(sd.sym_inferred(1), 0)
     with self.assertRaisesRegex(AttributeError, '2'):
-      _ = sd.sym_value(2)
+      _ = sd.sym_inferred(2)
 
   def test_sym_field(self):
     sl = List([dict(x=[], y={})])
     self.assertIsNone(sl.sym_field)
 
     spec = pg_typing.List(pg_typing.Dict([
         ('x', pg_typing.List(pg_typing.Int())),
@@ -746,66 +760,75 @@
     sl = List([dict(x=1), dict(x=2)], value_spec=pg_typing.List(pg_typing.Dict([
         ('x', pg_typing.Int()),
         ('y', pg_typing.Int(default=0))
     ])))
     self.assertEqual(next(sl.sym_values()), dict(x=1, y=0))
     self.assertEqual(list(sl.sym_values()), [dict(x=1, y=0), dict(x=2, y=0)])
 
-    sl = List([1, base.ContextualValue()])
+    sl = List([1, inferred.ValueFromParentChain()])
     self.assertEqual(next(sl.sym_values()), 1)
-    self.assertEqual(list(sl.sym_values()), [1, base.ContextualValue()])
+    self.assertEqual(
+        list(sl.sym_values()), [1, inferred.ValueFromParentChain()]
+    )
 
   def test_sym_items(self):
     sl = List(['a', 'b'])
     self.assertEqual(next(sl.sym_items()), (0, 'a'))
     self.assertEqual(list(sl.sym_items()), [(0, 'a'), (1, 'b')])
 
     sl = List([dict(x=1), dict(x=2)], value_spec=pg_typing.List(pg_typing.Dict([
         ('x', pg_typing.Int()),
         ('y', pg_typing.Int(default=0))
     ])))
     self.assertEqual(next(sl.sym_items()), (0, dict(x=1, y=0)))
     self.assertEqual(
         list(sl.sym_items()), [(0, dict(x=1, y=0)), (1, dict(x=2, y=0))])
 
-    sl = List([1, base.ContextualValue()])
+    sl = List([1, inferred.ValueFromParentChain()])
     self.assertEqual(next(sl.sym_items()), (0, 1))
     self.assertEqual(
-        list(sl.sym_items()), [(0, 1), (1, base.ContextualValue())]
+        list(sl.sym_items()), [(0, 1), (1, inferred.ValueFromParentChain())]
     )
 
   def test_sym_jsonify(self):
     # Refer to SerializationTest for more detailed tests.
-    sl = List([0, base.ContextualValue()])
-    self.assertEqual(sl.sym_jsonify(), [0, base.ContextualValue().to_json()])
+    sl = List([0, inferred.ValueFromParentChain()])
+    self.assertEqual(
+        sl.sym_jsonify(), [0, inferred.ValueFromParentChain().to_json()]
+    )
 
   def test_sym_rebind(self):
     # Refer to RebindTest for more detailed tests.
     sl = List([0, 1, 2])
-    sl.sym_rebind(
-        {0: MISSING_VALUE, 1: 3, 2: Insertion(4), 4: base.ContextualValue()}
+    sl.sym_rebind({
+        0: MISSING_VALUE,
+        1: 3,
+        2: Insertion(4),
+        4: inferred.ValueFromParentChain(),
+    })
+    self.assertEqual(
+        list(sl.sym_values()), [3, 4, 2, inferred.ValueFromParentChain()]
     )
-    self.assertEqual(list(sl.sym_values()), [3, 4, 2, base.ContextualValue()])
 
   def test_sym_clone(self):
     class A():
       pass
 
-    sl = List([[], dict(), A(), base.ContextualValue()])
+    sl = List([[], dict(), A(), inferred.ValueFromParentChain()])
     sl2 = sl.clone()
     self.assertEqual(sl, sl2)
     self.assertIsNot(sl, sl2)
     # Symbolic members are always copied by value.
     self.assertIsNot(sl[0], sl2[0])
     self.assertIsNot(sl[1], sl2[1])
 
     # Non-symbolic members are copied by reference.
     self.assertIs(sl[2], sl2[2])
 
-    # Contextual values are copied by symbols.
+    # Inferred values are copied by symbols.
     self.assertEqual(sl.sym_getattr(3), sl.sym_getattr(3))
 
     spec = pg_typing.List(pg_typing.Dict([
         (pg_typing.StrKey(), pg_typing.Any())
     ]))
     sl = List([Dict(x=list(), z=dict(), y=A())], value_spec=spec)
     sl2 = sl.sym_clone(deep=True)
@@ -837,36 +860,38 @@
     self.assertTrue(sl.sym_partial)
     sl.rebind({'[0].y.z': 2})
     self.assertFalse(sl.sym_partial)
 
   def test_sym_missing(self):
     # Refer to `test_missing_values` for more details.
     sl = List.partial(
-        [dict(x=base.ContextualValue())],
+        [dict(x=inferred.ValueFromParentChain())],
         value_spec=pg_typing.List(
             pg_typing.Dict([
                 ('x', pg_typing.Int()),
                 ('y', pg_typing.Int()),
             ])
         ),
     )
     self.assertEqual(sl.sym_missing(), {'[0].y': MISSING_VALUE})
 
   def test_sym_nondefault(self):
     # Refer to `test_non_default_values` for more details.
     sl = List(
-        [dict(x=base.ContextualValue())],
+        [dict(x=inferred.ValueFromParentChain())],
         value_spec=pg_typing.List(
             pg_typing.Dict([
                 ('x', pg_typing.Int(default=0)),
                 ('y', pg_typing.Dict([('z', pg_typing.Int(default=1))])),
             ])
         ),
     )
-    self.assertEqual(sl.sym_nondefault(), {'[0].x': base.ContextualValue()})
+    self.assertEqual(
+        sl.sym_nondefault(), {'[0].x': inferred.ValueFromParentChain()}
+    )
     sl.rebind({'[0].y.z': 2, '[0].x': 0})
     self.assertEqual(sl.sym_nondefault(), {'[0].y.z': 2})
 
   def test_sym_puresymbolic(self):
     self.assertFalse(List().sym_puresymbolic)
 
     class A(PureSymbolic):
@@ -1241,28 +1266,30 @@
     sl = List([[]])
     self.assertFalse(sl.is_sealed)
     self.assertFalse(sl[0].is_sealed)
     sl.seal()
     self.assertTrue(sl.is_sealed)
     self.assertTrue(sl[0].is_sealed)
 
-  def test_contextual(self):
-    # Test contextual access for schemaless list.
-    # Okay: sl[1] is contextual.
-    @contextual.contextual_getter
-    def redirected_value(context, key):
-      if context.container:
-        return getattr(context.container, key)
-      return object_utils.MISSING_VALUE
+  def test_inferred(self):
+    # Test inferred values for schemaless list.
+    # Okay: sl[1] is inferred.
+
+    class ValueFromRedirectedKey(inferred.ValueFromParentChain):
+      key: str
+
+      @property
+      def inference_key(self):
+        return self.key
 
-    sl = List([0, redirected_value(key='a')])  # pylint: disable=no-value-for-parameter
+    sl = List([0, ValueFromRedirectedKey('a')])
 
     self.assertEqual(sl[0], 0)
     with self.assertRaisesRegex(
-        AttributeError, '`1` is not found under its context'
+        AttributeError, '`a` is not found under its context'
     ):
       _ = sl[1]
 
     sd = Dict(x=sl, a=Dict(y=2))
     self.assertIs(sl[1], sd.a)
```

### Comparing `pyglove-0.4.3.dev20230729/pyglove/core/symbolic/object.py` & `pyglove-0.4.3.dev20230730/pyglove/core/symbolic/object.py`

 * *Files 2% similar despite different names*

```diff
@@ -380,15 +380,15 @@
   @classmethod
   def _create_sym_attribute(cls, attr_name, field):
     """Customizable trait: template of single symbolic attribute."""
     return property(
         object_utils.make_function(
             attr_name,
             ['self'],
-            [f"return self.sym_value('{attr_name}')"],
+            [f"return self.sym_inferred('{attr_name}')"],
             return_type=field.value.annotation,
         )
     )
 
   @classmethod
   def _begin_annotation_inference(cls) -> None:
     """Event that is triggered before annotation inference begins."""
@@ -809,18 +809,15 @@
   def __getattribute__(self, name: str) -> Any:
     """Override to accomondate symbolic attributes with variable keys."""
     try:
       return super().__getattribute__(name)
     except AttributeError as error:
       if not self.allow_symbolic_attribute or not self.sym_hasattr(name):
         raise error
-      return self.sym_value(name)
-
-  def _sym_value(self, key: str, default: Any) -> Any:  # pytype: disable=signature-mismatch
-    return self._sym_attributes._sym_value(key, default)  # pylint: disable=protected-access
+      return self.sym_inferred(name)
 
   def __eq__(self, other: Any) -> bool:
     """Operator==."""
     if self.use_symbolic_comparison:
       return self.sym_eq(other)
     return super().__eq__(other)
```

### Comparing `pyglove-0.4.3.dev20230729/pyglove/core/symbolic/object_test.py` & `pyglove-0.4.3.dev20230730/pyglove/core/symbolic/object_test.py`

 * *Files 4% similar despite different names*

```diff
@@ -21,16 +21,16 @@
 import tempfile
 import typing
 import unittest
 
 from pyglove.core import object_utils
 from pyglove.core import typing as pg_typing
 from pyglove.core.symbolic import base
-from pyglove.core.symbolic import contextual
 from pyglove.core.symbolic import flags
+from pyglove.core.symbolic import inferred
 from pyglove.core.symbolic.base import query as pg_query
 from pyglove.core.symbolic.base import traverse as pg_traverse
 from pyglove.core.symbolic.dict import Dict
 from pyglove.core.symbolic.functor import functor as pg_functor
 from pyglove.core.symbolic.list import List
 from pyglove.core.symbolic.object import members as pg_members
 from pyglove.core.symbolic.object import Object
@@ -604,15 +604,15 @@
     self.assertEqual(a.x, 1)
     self.assertTrue(a.y)      # Use default value from the field definition.
     self.assertEqual(a.z, 2)  # Non-symbolic field.
 
     class B(Object):
       x: int
 
-    b = B(base.ContextualValue())
+    b = B(inferred.ValueFromParentChain())
     with self.assertRaises(AttributeError):
       _ = b.x
 
     sd = Dict(x=1, b=b)
     self.assertEqual(sd.b.x, 1)
 
   def test_non_default(self):
@@ -653,19 +653,19 @@
         a.missing_values(flatten=False),
         {'x': MISSING_VALUE, 'z': {'p': MISSING_VALUE}})
 
     # After rebind, the non_default_values are updated.
     a.rebind({'x': 1, 'y': MISSING_VALUE, 'z.p': 1.0})
     self.assertEqual(a.missing_values(), {})
 
-    # Test contextual value as the default value.
+    # Test inferred value as the default value.
     class B(Object):
       x: int
 
-    b = B(base.ContextualValue())
+    b = B(inferred.ValueFromParentChain())
     self.assertEqual(b.sym_missing(), {})
 
   def test_sym_has(self):
 
     @pg_members([
         ('x', pg_typing.Any())
     ])
@@ -687,15 +687,18 @@
     @pg_members([('x', pg_typing.Any()), ('p', pg_typing.Any().noneable())])
     class A(Object):
 
       def _on_bound(self):
         super()._on_bound()
         self.y = 1
 
-    a = A(A(dict(y=A(1, p=base.ContextualValue()))), p=base.ContextualValue())
+    a = A(
+        A(dict(y=A(1, p=inferred.ValueFromParentChain()))),
+        p=inferred.ValueFromParentChain(),
+    )
 
     self.assertIs(a.sym_get('x'), a.x)
     self.assertIs(a.sym_get('p'), a.sym_getattr('p'))
     self.assertIs(a.sym_get('x.x'), a.x.x)
     self.assertIs(a.sym_get(object_utils.KeyPath.parse('x.x.y')), a.x.x.y)
     self.assertIs(a.sym_get(object_utils.KeyPath.parse('x.x.y.x')), a.x.x.y.x)
     self.assertIs(
@@ -746,16 +749,16 @@
       def _on_bound(self):
         super()._on_bound()
         self.y = 1
 
     a = A(1)
     self.assertEqual(a.sym_getattr('x'), 1)
 
-    a = A(x=base.ContextualValue())
-    self.assertEqual(a.sym_getattr('x'), base.ContextualValue())
+    a = A(x=inferred.ValueFromParentChain())
+    self.assertEqual(a.sym_getattr('x'), inferred.ValueFromParentChain())
 
     with self.assertRaisesRegex(
         AttributeError, 'has no symbolic attribute \'y\''):
       _ = a.sym_getattr('y')
 
     @pg_members([
         (pg_typing.StrKey('x.*'), pg_typing.Int())
@@ -769,107 +772,44 @@
 
     self.assertEqual(b.sym_getattr('x1'), 1)
     self.assertEqual(b.sym_getattr('x2'), 2)
     with self.assertRaisesRegex(
         AttributeError, 'has no symbolic attribute \'y\''):
       _ = b.sym_getattr('y')
 
-  def test_sym_value(self):
-    @contextual.contextual_getter
-    def static_value(context, v):
-      del context
-      return v
+  def test_sym_inferred(self):
+    class StaticValue(inferred.InferredValue):
+      v: typing.Any
+
+      def infer(self):
+        return self.v
 
     class A(Object):
       x: int = 1
-      y: int = static_value(v=0)  # pylint: disable=no-value-for-parameter
+      y: int = StaticValue(v=0)
 
     a = A()
-    self.assertEqual(a.sym_value('x'), 1)
-    self.assertEqual(a.sym_value('y'), 0)
+    self.assertEqual(a.sym_inferred('x'), 1)
+    self.assertEqual(a.sym_inferred('y'), 0)
+    self.assertEqual(a.sym_inferred('y', None), 0)
     with self.assertRaisesRegex(AttributeError, 'z'):
-      _ = a.sym_value('z')
-
-  def test_sym_contextual_hasattr(self):
-    class A(Object):
-      x: int
-      y: int = 1
-      z: int = base.ContextualValue()
-
-    a = A(0)
-    _ = Dict(p=Dict(a=a, b=3), z=2)
-    self.assertTrue(a.sym_contextual_hasattr('x'))
-    self.assertTrue(a.sym_contextual_hasattr('y'))
-    self.assertTrue(a.sym_contextual_hasattr('z'))
-
-    # Custom start.
-    self.assertFalse(a.sym_contextual_hasattr('x', start=a.sym_parent))
-    self.assertFalse(a.sym_contextual_hasattr('y', start=a.sym_parent))
-    self.assertTrue(a.sym_contextual_hasattr('z', start=a.sym_parent))
-
-    # Custom getter.
-    @contextual.contextual_getter
-    def redirected_value(context, key):
-      if context.container:
-        return getattr(context.container, key)
-      return pg_typing.MISSING_VALUE
-
-    getter = redirected_value(key='b')  # pylint: disable=no-value-for-parameter
-    self.assertTrue(a.sym_contextual_hasattr('x', getter, start=a.sym_parent))
-    self.assertTrue(a.sym_contextual_hasattr('y', getter, start=a.sym_parent))
-    self.assertTrue(a.sym_contextual_hasattr('z', getter, start=a.sym_parent))
+      _ = a.sym_inferred('z')
+    self.assertIsNone(a.sym_inferred('z', None))
 
-  def test_sym_contextual_getattr(self):
+  def test_sym_inferrable(self):
     class A(Object):
       x: int
       y: int = 1
-      z: int = base.ContextualValue()
-
-    a = A(0)
-
-    with self.assertRaises(AttributeError):
-      _ = a.z
+      z: int = inferred.ValueFromParentChain()
 
+    a = A.partial()
     _ = Dict(p=Dict(a=a, b=3), z=2)
-    self.assertEqual(a.z, 2)
-
-    self.assertEqual(a.sym_contextual_getattr('x'), 0)
-    self.assertEqual(a.sym_contextual_getattr('y'), 1)
-    self.assertEqual(a.sym_contextual_getattr('z'), 2)
-
-    # Custom start.
-    with self.assertRaisesRegex(
-        AttributeError, '`x` is not found under its context'
-    ):
-      a.sym_contextual_getattr('x', start=a.sym_parent)
-
-    with self.assertRaisesRegex(
-        AttributeError, '`y` is not found under its context'
-    ):
-      a.sym_contextual_getattr('y', start=a.sym_parent)
-
-    self.assertEqual(a.sym_contextual_getattr('z', start=a.sym_parent), 2)
-
-    # Custom getter.
-    @contextual.contextual_getter
-    def redirected_value(context, key):
-      if context.container:
-        return getattr(context.container, key)
-      return pg_typing.MISSING_VALUE
-
-    getter = redirected_value(key='b')  # pylint: disable=no-value-for-parameter
-    self.assertEqual(
-        a.sym_contextual_getattr('x', getter=getter, start=a.sym_parent), 3
-    )
-    self.assertEqual(
-        a.sym_contextual_getattr('y', getter=getter, start=a.sym_parent), 3
-    )
-    self.assertEqual(
-        a.sym_contextual_getattr('z', getter=getter, start=a.sym_parent), 3
-    )
+    self.assertFalse(a.sym_inferrable('x'))
+    self.assertTrue(a.sym_inferrable('y'))
+    self.assertTrue(a.sym_inferrable('z'))
 
   def test_sym_field(self):
 
     @pg_members([
         ('x', pg_typing.Any())
     ])
     class A(Object):
@@ -1241,15 +1181,19 @@
     class A(Object):
       pass
 
     # Use cases that `__eq__` and `sym_eq` have the same results.
     self.assertEqual(A(1), A(1))
     self.assertTrue(base.eq(A(1), A(1)))
     self.assertTrue(
-        base.eq(A(base.ContextualValue()), A(base.ContextualValue())))
+        base.eq(
+            A(inferred.ValueFromParentChain()),
+            A(inferred.ValueFromParentChain()),
+        )
+    )
 
     self.assertEqual(A.partial(), A.partial())
     self.assertTrue(base.eq(A.partial(), A.partial()))
 
     # Use case that `__eq__` rules both Python equality and `pg.eq`.
     class X:
 
@@ -1952,20 +1896,20 @@
         'Variable positional argument .* should be declared with '
         '`pg.typing.List.*`'):
 
       @pg_members([], init_arg_list=['*y'])
       class E(B):  # pylint: disable=unused-variable
         pass
 
-  def test_contextual(self):
+  def test_inferred(self):
     class A(Object):
       x: int
-      y: str = base.ContextualValue()
+      y: str = inferred.ValueFromParentChain()
 
-    # Okay: `A.y` is contextual.
+    # Okay: `A.y` is an inferred value.
     a = A(1)
 
     # Not okay: `A.y` is not yet available in its context.
     with self.assertRaisesRegex(
         AttributeError, '`y` is not found under its context'
     ):
       _ = a.y
@@ -1976,39 +1920,34 @@
     # Clear context by reset a's parent.
     a.sym_setparent(None)
     with self.assertRaisesRegex(
         AttributeError, '`y` is not found under its context'
     ):
       _ = a.y
 
-    # Test parent contextual value with custom getter.
-    @contextual.contextual_getter
-    def redirected_value(context, key):
-      if context.container:
-        return getattr(context.container, key)
-      return pg_typing.MISSING_VALUE
+    # Test a custom inferred value.
+    class ValueFromRedirectedKey(inferred.ValueFromParentChain):
+      key: str
 
-    sd = Dict(a='bar', b=Dict(x=a, y=redirected_value(key='a')))  # pylint: disable=no-value-for-parameter
+      @property
+      def inference_key(self):
+        return self.key
+
+    sd = Dict(a='bar', b=Dict(x=a, y=ValueFromRedirectedKey('a')))
 
     # a.y is redirected to sd.a.
     self.assertEqual(a.y, 'bar')
 
-    @contextual.contextual_getter
-    def immediate_attr(context):
-      if context.container:
-        return context.container.sym_getattr(context.key)
-      return pg_typing.MISSING_VALUE
-
     class B(Object):
-      x: int = immediate_attr()  # pylint: disable=no-value-for-parameter
+      x: int = inferred.ValueFromParentChain()  # pylint: disable=no-value-for-parameter
 
     b = B()
-    sd = Dict(a='bar', b=Dict(b=b, x=redirected_value(key='a')))  # pylint: disable=no-value-for-parameter
+    _ = Dict(a='bar', b=Dict(b=b, x=ValueFromRedirectedKey('a')))
 
-    # a.y is redirected to sd.a.
+    # b.x -> parent.x -> parent.parent.a
     self.assertEqual(b.x, 'bar')
 
 
 class RebindTest(unittest.TestCase):
   """Dedicated tests for `pg.Dict.rebind`."""
 
   def test_rebind_with_kwargs(self):
```

### Comparing `pyglove-0.4.3.dev20230729/pyglove/core/symbolic/origin.py` & `pyglove-0.4.3.dev20230730/pyglove/core/symbolic/origin.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.4.3.dev20230729/pyglove/core/symbolic/origin_test.py` & `pyglove-0.4.3.dev20230730/pyglove/core/symbolic/origin_test.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.4.3.dev20230729/pyglove/core/symbolic/pure_symbolic.py` & `pyglove-0.4.3.dev20230730/pyglove/core/symbolic/pure_symbolic.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.4.3.dev20230729/pyglove/core/symbolic/schema_utils.py` & `pyglove-0.4.3.dev20230730/pyglove/core/symbolic/schema_utils.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.4.3.dev20230729/pyglove/core/symbolic/schema_utils_test.py` & `pyglove-0.4.3.dev20230730/pyglove/core/symbolic/schema_utils_test.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.4.3.dev20230729/pyglove/core/symbolic/symbolize.py` & `pyglove-0.4.3.dev20230730/pyglove/core/symbolic/symbolize.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.4.3.dev20230729/pyglove/core/symbolic/symbolize_test.py` & `pyglove-0.4.3.dev20230730/pyglove/core/symbolic/symbolize_test.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.4.3.dev20230729/pyglove/core/tuning/__init__.py` & `pyglove-0.4.3.dev20230730/pyglove/core/tuning/__init__.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.4.3.dev20230729/pyglove/core/tuning/backend.py` & `pyglove-0.4.3.dev20230730/pyglove/core/tuning/backend.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.4.3.dev20230729/pyglove/core/tuning/backend_test.py` & `pyglove-0.4.3.dev20230730/pyglove/core/tuning/backend_test.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.4.3.dev20230729/pyglove/core/tuning/local_backend.py` & `pyglove-0.4.3.dev20230730/pyglove/core/tuning/local_backend.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.4.3.dev20230729/pyglove/core/tuning/protocols.py` & `pyglove-0.4.3.dev20230730/pyglove/core/tuning/protocols.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.4.3.dev20230729/pyglove/core/tuning/protocols_test.py` & `pyglove-0.4.3.dev20230730/pyglove/core/tuning/protocols_test.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.4.3.dev20230729/pyglove/core/tuning/sample.py` & `pyglove-0.4.3.dev20230730/pyglove/core/tuning/sample.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.4.3.dev20230729/pyglove/core/tuning/sample_test.py` & `pyglove-0.4.3.dev20230730/pyglove/core/tuning/sample_test.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.4.3.dev20230729/pyglove/core/typing/__init__.py` & `pyglove-0.4.3.dev20230730/pyglove/core/typing/__init__.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.4.3.dev20230729/pyglove/core/typing/annotation_conversion.py` & `pyglove-0.4.3.dev20230730/pyglove/core/typing/annotation_conversion.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.4.3.dev20230729/pyglove/core/typing/annotation_conversion_test.py` & `pyglove-0.4.3.dev20230730/pyglove/core/typing/annotation_conversion_test.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.4.3.dev20230729/pyglove/core/typing/callable_ext.py` & `pyglove-0.4.3.dev20230730/pyglove/core/typing/callable_ext.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.4.3.dev20230729/pyglove/core/typing/callable_ext_test.py` & `pyglove-0.4.3.dev20230730/pyglove/core/typing/callable_ext_test.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.4.3.dev20230729/pyglove/core/typing/callable_signature.py` & `pyglove-0.4.3.dev20230730/pyglove/core/typing/callable_signature.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.4.3.dev20230729/pyglove/core/typing/callable_signature_test.py` & `pyglove-0.4.3.dev20230730/pyglove/core/typing/callable_signature_test.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.4.3.dev20230729/pyglove/core/typing/class_schema.py` & `pyglove-0.4.3.dev20230730/pyglove/core/typing/class_schema.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.4.3.dev20230729/pyglove/core/typing/class_schema_test.py` & `pyglove-0.4.3.dev20230730/pyglove/core/typing/class_schema_test.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.4.3.dev20230729/pyglove/core/typing/class_schema_utils.py` & `pyglove-0.4.3.dev20230730/pyglove/core/typing/class_schema_utils.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.4.3.dev20230729/pyglove/core/typing/class_schema_utils_test.py` & `pyglove-0.4.3.dev20230730/pyglove/core/typing/class_schema_utils_test.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.4.3.dev20230729/pyglove/core/typing/custom_typing.py` & `pyglove-0.4.3.dev20230730/pyglove/core/typing/custom_typing.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.4.3.dev20230729/pyglove/core/typing/generic.py` & `pyglove-0.4.3.dev20230730/pyglove/core/typing/generic.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.4.3.dev20230729/pyglove/core/typing/generic_test.py` & `pyglove-0.4.3.dev20230730/pyglove/core/typing/generic_test.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.4.3.dev20230729/pyglove/core/typing/key_specs.py` & `pyglove-0.4.3.dev20230730/pyglove/core/typing/key_specs.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.4.3.dev20230729/pyglove/core/typing/key_specs_test.py` & `pyglove-0.4.3.dev20230730/pyglove/core/typing/key_specs_test.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.4.3.dev20230729/pyglove/core/typing/pytype_support.py` & `pyglove-0.4.3.dev20230730/pyglove/core/typing/pytype_support.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.4.3.dev20230729/pyglove/core/typing/type_conversion.py` & `pyglove-0.4.3.dev20230730/pyglove/core/typing/type_conversion.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.4.3.dev20230729/pyglove/core/typing/type_conversion_test.py` & `pyglove-0.4.3.dev20230730/pyglove/core/typing/type_conversion_test.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.4.3.dev20230729/pyglove/core/typing/typed_missing.py` & `pyglove-0.4.3.dev20230730/pyglove/core/typing/typed_missing.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.4.3.dev20230729/pyglove/core/typing/typed_missing_test.py` & `pyglove-0.4.3.dev20230730/pyglove/core/typing/typed_missing_test.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.4.3.dev20230729/pyglove/core/typing/value_specs.py` & `pyglove-0.4.3.dev20230730/pyglove/core/typing/value_specs.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.4.3.dev20230729/pyglove/core/typing/value_specs_test.py` & `pyglove-0.4.3.dev20230730/pyglove/core/typing/value_specs_test.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.4.3.dev20230729/pyglove/ext/__init__.py` & `pyglove-0.4.3.dev20230730/pyglove/ext/__init__.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.4.3.dev20230729/pyglove/ext/early_stopping/__init__.py` & `pyglove-0.4.3.dev20230730/pyglove/ext/early_stopping/__init__.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.4.3.dev20230729/pyglove/ext/early_stopping/base.py` & `pyglove-0.4.3.dev20230730/pyglove/ext/early_stopping/base.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.4.3.dev20230729/pyglove/ext/early_stopping/base_test.py` & `pyglove-0.4.3.dev20230730/pyglove/ext/early_stopping/base_test.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.4.3.dev20230729/pyglove/ext/early_stopping/step_wise.py` & `pyglove-0.4.3.dev20230730/pyglove/ext/early_stopping/step_wise.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.4.3.dev20230729/pyglove/ext/early_stopping/step_wise_test.py` & `pyglove-0.4.3.dev20230730/pyglove/ext/early_stopping/step_wise_test.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.4.3.dev20230729/pyglove/ext/evolution/__init__.py` & `pyglove-0.4.3.dev20230730/pyglove/ext/evolution/__init__.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.4.3.dev20230729/pyglove/ext/evolution/base.py` & `pyglove-0.4.3.dev20230730/pyglove/ext/evolution/base.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.4.3.dev20230729/pyglove/ext/evolution/base_test.py` & `pyglove-0.4.3.dev20230730/pyglove/ext/evolution/base_test.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.4.3.dev20230729/pyglove/ext/evolution/hill_climb.py` & `pyglove-0.4.3.dev20230730/pyglove/ext/evolution/hill_climb.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.4.3.dev20230729/pyglove/ext/evolution/hill_climb_test.py` & `pyglove-0.4.3.dev20230730/pyglove/ext/evolution/hill_climb_test.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.4.3.dev20230729/pyglove/ext/evolution/mutators.py` & `pyglove-0.4.3.dev20230730/pyglove/ext/evolution/mutators.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.4.3.dev20230729/pyglove/ext/evolution/mutators_test.py` & `pyglove-0.4.3.dev20230730/pyglove/ext/evolution/mutators_test.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.4.3.dev20230729/pyglove/ext/evolution/neat.py` & `pyglove-0.4.3.dev20230730/pyglove/ext/evolution/neat.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.4.3.dev20230729/pyglove/ext/evolution/neat_test.py` & `pyglove-0.4.3.dev20230730/pyglove/ext/evolution/neat_test.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.4.3.dev20230729/pyglove/ext/evolution/nsga2.py` & `pyglove-0.4.3.dev20230730/pyglove/ext/evolution/nsga2.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.4.3.dev20230729/pyglove/ext/evolution/nsga2_test.py` & `pyglove-0.4.3.dev20230730/pyglove/ext/evolution/nsga2_test.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.4.3.dev20230729/pyglove/ext/evolution/recombinators.py` & `pyglove-0.4.3.dev20230730/pyglove/ext/evolution/recombinators.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.4.3.dev20230729/pyglove/ext/evolution/recombinators_test.py` & `pyglove-0.4.3.dev20230730/pyglove/ext/evolution/recombinators_test.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.4.3.dev20230729/pyglove/ext/evolution/regularized_evolution.py` & `pyglove-0.4.3.dev20230730/pyglove/ext/evolution/regularized_evolution.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.4.3.dev20230729/pyglove/ext/evolution/regularized_evolution_test.py` & `pyglove-0.4.3.dev20230730/pyglove/ext/evolution/regularized_evolution_test.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.4.3.dev20230729/pyglove/ext/evolution/selectors.py` & `pyglove-0.4.3.dev20230730/pyglove/ext/evolution/selectors.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.4.3.dev20230729/pyglove/ext/evolution/selectors_test.py` & `pyglove-0.4.3.dev20230730/pyglove/ext/evolution/selectors_test.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.4.3.dev20230729/pyglove/ext/evolution/where.py` & `pyglove-0.4.3.dev20230730/pyglove/ext/evolution/where.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.4.3.dev20230729/pyglove/ext/evolution/where_test.py` & `pyglove-0.4.3.dev20230730/pyglove/ext/evolution/where_test.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.4.3.dev20230729/pyglove/ext/mutfun/__init__.py` & `pyglove-0.4.3.dev20230730/pyglove/ext/mutfun/__init__.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.4.3.dev20230729/pyglove/ext/mutfun/base.py` & `pyglove-0.4.3.dev20230730/pyglove/ext/mutfun/base.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.4.3.dev20230729/pyglove/ext/mutfun/base_test.py` & `pyglove-0.4.3.dev20230730/pyglove/ext/mutfun/base_test.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.4.3.dev20230729/pyglove/ext/mutfun/basic_ops.py` & `pyglove-0.4.3.dev20230730/pyglove/ext/mutfun/basic_ops.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.4.3.dev20230729/pyglove/ext/mutfun/basic_ops_test.py` & `pyglove-0.4.3.dev20230730/pyglove/ext/mutfun/basic_ops_test.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.4.3.dev20230729/pyglove/ext/scalars/__init__.py` & `pyglove-0.4.3.dev20230730/pyglove/ext/scalars/__init__.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.4.3.dev20230729/pyglove/ext/scalars/base.py` & `pyglove-0.4.3.dev20230730/pyglove/ext/scalars/base.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.4.3.dev20230729/pyglove/ext/scalars/base_test.py` & `pyglove-0.4.3.dev20230730/pyglove/ext/scalars/base_test.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.4.3.dev20230729/pyglove/ext/scalars/maths.py` & `pyglove-0.4.3.dev20230730/pyglove/ext/scalars/maths.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.4.3.dev20230729/pyglove/ext/scalars/maths_test.py` & `pyglove-0.4.3.dev20230730/pyglove/ext/scalars/maths_test.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.4.3.dev20230729/pyglove/ext/scalars/randoms.py` & `pyglove-0.4.3.dev20230730/pyglove/ext/scalars/randoms.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.4.3.dev20230729/pyglove/ext/scalars/randoms_test.py` & `pyglove-0.4.3.dev20230730/pyglove/ext/scalars/randoms_test.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.4.3.dev20230729/pyglove/ext/scalars/step_wise.py` & `pyglove-0.4.3.dev20230730/pyglove/ext/scalars/step_wise.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.4.3.dev20230729/pyglove/ext/scalars/step_wise_test.py` & `pyglove-0.4.3.dev20230730/pyglove/ext/scalars/step_wise_test.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.4.3.dev20230729/pyglove.egg-info/PKG-INFO` & `pyglove-0.4.3.dev20230730/pyglove.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyglove
-Version: 0.4.3.dev20230729
+Version: 0.4.3.dev20230730
 Summary: PyGlove: A library for manipulating Python objects.
 Home-page: https://github.com/google/pyglove
 Author: PyGlove Authors
 Author-email: pyglove-authors@google.com
 License: Apache License 2.0
 Keywords: ai machine learning automl mutable symbolic framework meta-programming
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `pyglove-0.4.3.dev20230729/pyglove.egg-info/SOURCES.txt` & `pyglove-0.4.3.dev20230730/pyglove.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -79,24 +79,24 @@
 pyglove/core/symbolic/base_test.py
 pyglove/core/symbolic/boilerplate.py
 pyglove/core/symbolic/boilerplate_test.py
 pyglove/core/symbolic/class_wrapper.py
 pyglove/core/symbolic/class_wrapper_test.py
 pyglove/core/symbolic/compounding.py
 pyglove/core/symbolic/compounding_test.py
-pyglove/core/symbolic/contextual.py
-pyglove/core/symbolic/contextual_test.py
 pyglove/core/symbolic/dict.py
 pyglove/core/symbolic/dict_test.py
 pyglove/core/symbolic/diff.py
 pyglove/core/symbolic/diff_test.py
 pyglove/core/symbolic/flags.py
 pyglove/core/symbolic/flags_test.py
 pyglove/core/symbolic/functor.py
 pyglove/core/symbolic/functor_test.py
+pyglove/core/symbolic/inferred.py
+pyglove/core/symbolic/inferred_test.py
 pyglove/core/symbolic/list.py
 pyglove/core/symbolic/list_test.py
 pyglove/core/symbolic/object.py
 pyglove/core/symbolic/object_test.py
 pyglove/core/symbolic/origin.py
 pyglove/core/symbolic/origin_test.py
 pyglove/core/symbolic/pure_symbolic.py
```

### Comparing `pyglove-0.4.3.dev20230729/setup.py` & `pyglove-0.4.3.dev20230730/setup.py`

 * *Files identical despite different names*

