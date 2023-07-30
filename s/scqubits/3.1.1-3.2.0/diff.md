# Comparing `tmp/scqubits-3.1.1.tar.gz` & `tmp/scqubits-3.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "scqubits-3.1.1.tar", last modified: Wed Apr 12 05:38:35 2023, max compression
+gzip compressed data, was "scqubits-3.2.0.tar", last modified: Sun Jul 30 02:49:31 2023, max compression
```

## Comparing `scqubits-3.1.1.tar` & `scqubits-3.2.0.tar`

### file list

```diff
@@ -1,132 +1,150 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 05:38:35.828381 scqubits-3.1.1/
--rwxr-xr-x   0 runner    (1001) docker     (123)     1549 2023-04-12 05:38:24.000000 scqubits-3.1.1/LICENSE
--rwxr-xr-x   0 runner    (1001) docker     (123)      237 2023-04-12 05:38:24.000000 scqubits-3.1.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1916 2023-04-12 05:38:35.828381 scqubits-3.1.1/PKG-INFO
--rwxr-xr-x   0 runner    (1001) docker     (123)     3439 2023-04-12 05:38:24.000000 scqubits-3.1.1/README.md
--rwxr-xr-x   0 runner    (1001) docker     (123)       61 2023-04-12 05:38:24.000000 scqubits-3.1.1/optional-requirements.txt
--rwxr-xr-x   0 runner    (1001) docker     (123)      100 2023-04-12 05:38:24.000000 scqubits-3.1.1/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 05:38:35.796381 scqubits-3.1.1/scqubits/
--rwxr-xr-x   0 runner    (1001) docker     (123)     3091 2023-04-12 05:38:24.000000 scqubits-3.1.1/scqubits/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 05:38:35.804381 scqubits-3.1.1/scqubits/core/
--rwxr-xr-x   0 runner    (1001) docker     (123)      482 2023-04-12 05:38:24.000000 scqubits-3.1.1/scqubits/core/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     6939 2023-04-12 05:38:24.000000 scqubits-3.1.1/scqubits/core/central_dispatch.py
--rw-r--r--   0 runner    (1001) docker     (123)   139627 2023-04-12 05:38:24.000000 scqubits-3.1.1/scqubits/core/circuit.py
--rw-r--r--   0 runner    (1001) docker     (123)    11416 2023-04-12 05:38:24.000000 scqubits-3.1.1/scqubits/core/circuit_utils.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1107 2023-04-12 05:38:24.000000 scqubits-3.1.1/scqubits/core/constants.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    54530 2023-04-12 05:38:24.000000 scqubits-3.1.1/scqubits/core/cos2phi_qubit.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3538 2023-04-12 05:38:24.000000 scqubits-3.1.1/scqubits/core/descriptors.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     9106 2023-04-12 05:38:24.000000 scqubits-3.1.1/scqubits/core/discretization.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    36737 2023-04-12 05:38:24.000000 scqubits-3.1.1/scqubits/core/flux_qubit.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    18938 2023-04-12 05:38:24.000000 scqubits-3.1.1/scqubits/core/fluxonium.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3645 2023-04-12 05:38:24.000000 scqubits-3.1.1/scqubits/core/generic_qubit.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    43780 2023-04-12 05:38:24.000000 scqubits-3.1.1/scqubits/core/hilbert_space.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    24921 2023-04-12 05:38:24.000000 scqubits-3.1.1/scqubits/core/namedslots_array.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    60033 2023-04-12 05:38:24.000000 scqubits-3.1.1/scqubits/core/noise.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     6580 2023-04-12 05:38:24.000000 scqubits-3.1.1/scqubits/core/operators.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     8974 2023-04-12 05:38:24.000000 scqubits-3.1.1/scqubits/core/oscillator.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    56815 2023-04-12 05:38:24.000000 scqubits-3.1.1/scqubits/core/param_sweep.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    42979 2023-04-12 05:38:24.000000 scqubits-3.1.1/scqubits/core/qubit_base.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 05:38:35.808381 scqubits-3.1.1/scqubits/core/qubit_img/
--rwxr-xr-x   0 runner    (1001) docker     (123)    87518 2023-04-12 05:38:24.000000 scqubits-3.1.1/scqubits/core/qubit_img/cos2phi-qubit.jpg
--rwxr-xr-x   0 runner    (1001) docker     (123)    97089 2023-04-12 05:38:24.000000 scqubits-3.1.1/scqubits/core/qubit_img/fixed-transmon.jpg
--rwxr-xr-x   0 runner    (1001) docker     (123)   106916 2023-04-12 05:38:24.000000 scqubits-3.1.1/scqubits/core/qubit_img/flux-qubit.jpg
--rwxr-xr-x   0 runner    (1001) docker     (123)   113985 2023-04-12 05:38:24.000000 scqubits-3.1.1/scqubits/core/qubit_img/fluxonium.jpg
--rwxr-xr-x   0 runner    (1001) docker     (123)   328242 2023-04-12 05:38:24.000000 scqubits-3.1.1/scqubits/core/qubit_img/fullzeropi.jpg
--rwxr-xr-x   0 runner    (1001) docker     (123)   255948 2023-04-12 05:38:24.000000 scqubits-3.1.1/scqubits/core/qubit_img/kerr-oscillator.jpg
--rwxr-xr-x   0 runner    (1001) docker     (123)   412869 2023-04-12 05:38:24.000000 scqubits-3.1.1/scqubits/core/qubit_img/oscillator.jpg
--rwxr-xr-x   0 runner    (1001) docker     (123)   133117 2023-04-12 05:38:24.000000 scqubits-3.1.1/scqubits/core/qubit_img/tunable-transmon.jpg
--rwxr-xr-x   0 runner    (1001) docker     (123)   295606 2023-04-12 05:38:24.000000 scqubits-3.1.1/scqubits/core/qubit_img/zeropi.jpg
--rwxr-xr-x   0 runner    (1001) docker     (123)    14843 2023-04-12 05:38:24.000000 scqubits-3.1.1/scqubits/core/spec_lookup.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     8507 2023-04-12 05:38:24.000000 scqubits-3.1.1/scqubits/core/storage.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3071 2023-04-12 05:38:24.000000 scqubits-3.1.1/scqubits/core/sweeps.py
--rw-r--r--   0 runner    (1001) docker     (123)    70527 2023-04-12 05:38:24.000000 scqubits-3.1.1/scqubits/core/symbolic_circuit.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    31094 2023-04-12 05:38:24.000000 scqubits-3.1.1/scqubits/core/transmon.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     4034 2023-04-12 05:38:24.000000 scqubits-3.1.1/scqubits/core/units.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    32843 2023-04-12 05:38:24.000000 scqubits-3.1.1/scqubits/core/zeropi.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    29519 2023-04-12 05:38:24.000000 scqubits-3.1.1/scqubits/core/zeropi_full.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 05:38:35.808381 scqubits-3.1.1/scqubits/explorer/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-12 05:38:24.000000 scqubits-3.1.1/scqubits/explorer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10044 2023-04-12 05:38:24.000000 scqubits-3.1.1/scqubits/explorer/explorer_panels.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 05:38:35.812381 scqubits-3.1.1/scqubits/io_utils/
--rwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 05:38:24.000000 scqubits-3.1.1/scqubits/io_utils/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     5884 2023-04-12 05:38:24.000000 scqubits-3.1.1/scqubits/io_utils/fileio.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    13961 2023-04-12 05:38:24.000000 scqubits-3.1.1/scqubits/io_utils/fileio_backends.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2395 2023-04-12 05:38:24.000000 scqubits-3.1.1/scqubits/io_utils/fileio_qutip.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    10969 2023-04-12 05:38:24.000000 scqubits-3.1.1/scqubits/io_utils/fileio_serializers.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     5030 2023-04-12 05:38:24.000000 scqubits-3.1.1/scqubits/settings.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      689 2023-04-12 05:38:24.000000 scqubits-3.1.1/scqubits/testing.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 05:38:35.812381 scqubits-3.1.1/scqubits/tests/
--rwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 05:38:24.000000 scqubits-3.1.1/scqubits/tests/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     9645 2023-04-12 05:38:24.000000 scqubits-3.1.1/scqubits/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 05:38:35.824381 scqubits-3.1.1/scqubits/tests/data/
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-04-12 05:38:24.000000 scqubits-3.1.1/scqubits/tests/data/circuit_DFC.yaml
--rw-r--r--   0 runner    (1001) docker     (123)       57 2023-04-12 05:38:24.000000 scqubits-3.1.1/scqubits/tests/data/circuit_fluxonium.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      146 2023-04-12 05:38:24.000000 scqubits-3.1.1/scqubits/tests/data/circuit_zeropi.yaml
--rwxr-xr-x   0 runner    (1001) docker     (123)    15496 2023-04-12 05:38:24.000000 scqubits-3.1.1/scqubits/tests/data/cos2phiqubit_1.hdf5
--rwxr-xr-x   0 runner    (1001) docker     (123)   214632 2023-04-12 05:38:24.000000 scqubits-3.1.1/scqubits/tests/data/cos2phiqubit_2.hdf5
--rwxr-xr-x   0 runner    (1001) docker     (123)   472471 2023-04-12 05:38:24.000000 scqubits-3.1.1/scqubits/tests/data/cos2phiqubit_4.hdf5
--rwxr-xr-x   0 runner    (1001) docker     (123)    16032 2023-04-12 05:38:24.000000 scqubits-3.1.1/scqubits/tests/data/cos2phiqubit_5.hdf5
--rwxr-xr-x   0 runner    (1001) docker     (123)    15048 2023-04-12 05:38:24.000000 scqubits-3.1.1/scqubits/tests/data/fluxonium_1.hdf5
--rwxr-xr-x   0 runner    (1001) docker     (123)    21667 2023-04-12 05:38:24.000000 scqubits-3.1.1/scqubits/tests/data/fluxonium_2.hdf5
--rwxr-xr-x   0 runner    (1001) docker     (123)   367163 2023-04-12 05:38:24.000000 scqubits-3.1.1/scqubits/tests/data/fluxonium_4.hdf5
--rwxr-xr-x   0 runner    (1001) docker     (123)    14512 2023-04-12 05:38:24.000000 scqubits-3.1.1/scqubits/tests/data/fluxonium_5.hdf5
--rwxr-xr-x   0 runner    (1001) docker     (123)    14136 2023-04-12 05:38:24.000000 scqubits-3.1.1/scqubits/tests/data/fluxqubit_1.hdf5
--rwxr-xr-x   0 runner    (1001) docker     (123)    39269 2023-04-12 05:38:24.000000 scqubits-3.1.1/scqubits/tests/data/fluxqubit_2.hdf5
--rwxr-xr-x   0 runner    (1001) docker     (123)  1205265 2023-04-12 05:38:24.000000 scqubits-3.1.1/scqubits/tests/data/fluxqubit_4.hdf5
--rwxr-xr-x   0 runner    (1001) docker     (123)    14960 2023-04-12 05:38:24.000000 scqubits-3.1.1/scqubits/tests/data/fluxqubit_5.hdf5
--rwxr-xr-x   0 runner    (1001) docker     (123)    17920 2023-04-12 05:38:24.000000 scqubits-3.1.1/scqubits/tests/data/fullzeropi_1.hdf5
--rw-r--r--   0 runner    (1001) docker     (123)    33599 2023-04-12 05:38:24.000000 scqubits-3.1.1/scqubits/tests/data/fullzeropi_2.hdf5
--rwxr-xr-x   0 runner    (1001) docker     (123)    13624 2023-04-12 05:38:24.000000 scqubits-3.1.1/scqubits/tests/data/transmon_1.hdf5
--rwxr-xr-x   0 runner    (1001) docker     (123)    18560 2023-04-12 05:38:24.000000 scqubits-3.1.1/scqubits/tests/data/transmon_2.hdf5
--rwxr-xr-x   0 runner    (1001) docker     (123)   120906 2023-04-12 05:38:24.000000 scqubits-3.1.1/scqubits/tests/data/transmon_4.hdf5
--rwxr-xr-x   0 runner    (1001) docker     (123)    14416 2023-04-12 05:38:24.000000 scqubits-3.1.1/scqubits/tests/data/transmon_5.hdf5
--rwxr-xr-x   0 runner    (1001) docker     (123)     9024 2023-04-12 05:38:24.000000 scqubits-3.1.1/scqubits/tests/data/zeropi-test.hdf5
--rwxr-xr-x   0 runner    (1001) docker     (123)    17664 2023-04-12 05:38:24.000000 scqubits-3.1.1/scqubits/tests/data/zeropi_1.hdf5
--rwxr-xr-x   0 runner    (1001) docker     (123)   788882 2023-04-12 05:38:24.000000 scqubits-3.1.1/scqubits/tests/data/zeropi_2.hdf5
--rwxr-xr-x   0 runner    (1001) docker     (123)  1761598 2023-04-12 05:38:24.000000 scqubits-3.1.1/scqubits/tests/data/zeropi_4.hdf5
--rwxr-xr-x   0 runner    (1001) docker     (123)    18200 2023-04-12 05:38:24.000000 scqubits-3.1.1/scqubits/tests/data/zeropi_5.hdf5
--rwxr-xr-x   0 runner    (1001) docker     (123)     9264 2023-04-12 05:38:24.000000 scqubits-3.1.1/scqubits/tests/data/zpifull-test.hdf5
--rwxr-xr-x   0 runner    (1001) docker     (123)     2659 2023-04-12 05:38:24.000000 scqubits-3.1.1/scqubits/tests/test_centraldispatch.py
--rw-r--r--   0 runner    (1001) docker     (123)     7666 2023-04-12 05:38:24.000000 scqubits-3.1.1/scqubits/tests/test_circuit.py
--rw-r--r--   0 runner    (1001) docker     (123)      960 2023-04-12 05:38:24.000000 scqubits-3.1.1/scqubits/tests/test_circuit_plot.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1020 2023-04-12 05:38:24.000000 scqubits-3.1.1/scqubits/tests/test_cos2phiqubit.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2501 2023-04-12 05:38:24.000000 scqubits-3.1.1/scqubits/tests/test_explorer.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      951 2023-04-12 05:38:24.000000 scqubits-3.1.1/scqubits/tests/test_fluxonium.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      953 2023-04-12 05:38:24.000000 scqubits-3.1.1/scqubits/tests/test_fluxqubit.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2110 2023-04-12 05:38:24.000000 scqubits-3.1.1/scqubits/tests/test_fullzeropi.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      595 2023-04-12 05:38:24.000000 scqubits-3.1.1/scqubits/tests/test_gui.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    16570 2023-04-12 05:38:24.000000 scqubits-3.1.1/scqubits/tests/test_hilbertspace.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1509 2023-04-12 05:38:24.000000 scqubits-3.1.1/scqubits/tests/test_namedslotsndarray.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     4731 2023-04-12 05:38:24.000000 scqubits-3.1.1/scqubits/tests/test_noise.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1545 2023-04-12 05:38:24.000000 scqubits-3.1.1/scqubits/tests/test_parameters.py
--rw-r--r--   0 runner    (1001) docker     (123)     4191 2023-04-12 05:38:24.000000 scqubits-3.1.1/scqubits/tests/test_parametersweep.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    16340 2023-04-12 05:38:24.000000 scqubits-3.1.1/scqubits/tests/test_spectrumlookup.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1172 2023-04-12 05:38:24.000000 scqubits-3.1.1/scqubits/tests/test_transmon.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1349 2023-04-12 05:38:24.000000 scqubits-3.1.1/scqubits/tests/test_units.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1006 2023-04-12 05:38:24.000000 scqubits-3.1.1/scqubits/tests/test_zeropi.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 05:38:35.828381 scqubits-3.1.1/scqubits/ui/
--rwxr-xr-x   0 runner    (1001) docker     (123)      619 2023-04-12 05:38:24.000000 scqubits-3.1.1/scqubits/ui/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    35028 2023-04-12 05:38:24.000000 scqubits-3.1.1/scqubits/ui/explorer_widget.py
--rw-r--r--   0 runner    (1001) docker     (123)    86193 2023-04-12 05:38:24.000000 scqubits-3.1.1/scqubits/ui/gui.py
--rw-r--r--   0 runner    (1001) docker     (123)     7240 2023-04-12 05:38:24.000000 scqubits-3.1.1/scqubits/ui/gui_defaults.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    15818 2023-04-12 05:38:24.000000 scqubits-3.1.1/scqubits/ui/hspace_widget.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2860 2023-04-12 05:38:24.000000 scqubits-3.1.1/scqubits/ui/qubit_widget.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 05:38:35.828381 scqubits-3.1.1/scqubits/utils/
--rwxr-xr-x   0 runner    (1001) docker     (123)      619 2023-04-12 05:38:24.000000 scqubits-3.1.1/scqubits/utils/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1856 2023-04-12 05:38:24.000000 scqubits-3.1.1/scqubits/utils/cpu_switch.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    11110 2023-04-12 05:38:24.000000 scqubits-3.1.1/scqubits/utils/misc.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     6892 2023-04-12 05:38:24.000000 scqubits-3.1.1/scqubits/utils/plot_defaults.py
--rw-r--r--   0 runner    (1001) docker     (123)     6899 2023-04-12 05:38:24.000000 scqubits-3.1.1/scqubits/utils/plot_utils.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    18701 2023-04-12 05:38:24.000000 scqubits-3.1.1/scqubits/utils/plotting.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    15622 2023-04-12 05:38:24.000000 scqubits-3.1.1/scqubits/utils/spectrum_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     1293 2023-04-12 05:38:24.000000 scqubits-3.1.1/scqubits/utils/typedefs.py
--rw-r--r--   0 runner    (1001) docker     (123)      105 2023-04-12 05:38:35.000000 scqubits-3.1.1/scqubits/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 05:38:35.800381 scqubits-3.1.1/scqubits.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1916 2023-04-12 05:38:35.000000 scqubits-3.1.1/scqubits.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3743 2023-04-12 05:38:35.000000 scqubits-3.1.1/scqubits.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-12 05:38:35.000000 scqubits-3.1.1/scqubits.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-12 05:38:35.000000 scqubits-3.1.1/scqubits.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      235 2023-04-12 05:38:35.000000 scqubits-3.1.1/scqubits.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)      101 2023-04-12 05:38:35.000000 scqubits-3.1.1/scqubits.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-12 05:38:35.828381 scqubits-3.1.1/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (123)     4759 2023-04-12 05:38:24.000000 scqubits-3.1.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 02:49:31.342536 scqubits-3.2.0/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1549 2023-07-30 02:49:21.000000 scqubits-3.2.0/LICENSE
+-rwxr-xr-x   0 runner    (1001) docker     (123)      261 2023-07-30 02:49:21.000000 scqubits-3.2.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1892 2023-07-30 02:49:31.342536 scqubits-3.2.0/PKG-INFO
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3853 2023-07-30 02:49:21.000000 scqubits-3.2.0/README.md
+-rwxr-xr-x   0 runner    (1001) docker     (123)       87 2023-07-30 02:49:21.000000 scqubits-3.2.0/optional-requirements.txt
+-rwxr-xr-x   0 runner    (1001) docker     (123)      122 2023-07-30 02:49:21.000000 scqubits-3.2.0/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 02:49:31.302534 scqubits-3.2.0/scqubits/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3469 2023-07-30 02:49:21.000000 scqubits-3.2.0/scqubits/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 02:49:31.314535 scqubits-3.2.0/scqubits/core/
+-rwxr-xr-x   0 runner    (1001) docker     (123)      482 2023-07-30 02:49:21.000000 scqubits-3.2.0/scqubits/core/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     6977 2023-07-30 02:49:21.000000 scqubits-3.2.0/scqubits/core/central_dispatch.py
+-rw-r--r--   0 runner    (1001) docker     (123)   140163 2023-07-30 02:49:21.000000 scqubits-3.2.0/scqubits/core/circuit.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11414 2023-07-30 02:49:21.000000 scqubits-3.2.0/scqubits/core/circuit_utils.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1107 2023-07-30 02:49:21.000000 scqubits-3.2.0/scqubits/core/constants.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    54792 2023-07-30 02:49:21.000000 scqubits-3.2.0/scqubits/core/cos2phi_qubit.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3568 2023-07-30 02:49:21.000000 scqubits-3.2.0/scqubits/core/descriptors.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    19398 2023-07-30 02:49:21.000000 scqubits-3.2.0/scqubits/core/diag.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     9106 2023-07-30 02:49:21.000000 scqubits-3.2.0/scqubits/core/discretization.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    38905 2023-07-30 02:49:21.000000 scqubits-3.2.0/scqubits/core/flux_qubit.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    19203 2023-07-30 02:49:21.000000 scqubits-3.2.0/scqubits/core/fluxonium.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3645 2023-07-30 02:49:21.000000 scqubits-3.2.0/scqubits/core/generic_qubit.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    48139 2023-07-30 02:49:21.000000 scqubits-3.2.0/scqubits/core/hilbert_space.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    24921 2023-07-30 02:49:21.000000 scqubits-3.2.0/scqubits/core/namedslots_array.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    60032 2023-07-30 02:49:21.000000 scqubits-3.2.0/scqubits/core/noise.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     6604 2023-07-30 02:49:21.000000 scqubits-3.2.0/scqubits/core/operators.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     8976 2023-07-30 02:49:21.000000 scqubits-3.2.0/scqubits/core/oscillator.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    58165 2023-07-30 02:49:21.000000 scqubits-3.2.0/scqubits/core/param_sweep.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    45364 2023-07-30 02:49:21.000000 scqubits-3.2.0/scqubits/core/qubit_base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 02:49:31.318535 scqubits-3.2.0/scqubits/core/qubit_img/
+-rw-r--r--   0 runner    (1001) docker     (123)   159663 2023-07-30 02:49:21.000000 scqubits-3.2.0/scqubits/core/qubit_img/Bifluxon.jpg
+-rw-r--r--   0 runner    (1001) docker     (123)   104902 2023-07-30 02:49:21.000000 scqubits-3.2.0/scqubits/core/qubit_img/Cos2PhiQubit.jpg
+-rw-r--r--   0 runner    (1001) docker     (123)   108284 2023-07-30 02:49:21.000000 scqubits-3.2.0/scqubits/core/qubit_img/FluxQubit.jpg
+-rwxr-xr-x   0 runner    (1001) docker     (123)   320438 2023-07-30 02:49:21.000000 scqubits-3.2.0/scqubits/core/qubit_img/Fluxonium.jpg
+-rwxr-xr-x   0 runner    (1001) docker     (123)   125604 2023-07-30 02:49:21.000000 scqubits-3.2.0/scqubits/core/qubit_img/FullZeroPi.jpg
+-rw-r--r--   0 runner    (1001) docker     (123)    63343 2023-07-30 02:49:21.000000 scqubits-3.2.0/scqubits/core/qubit_img/KerrOscillator.jpg
+-rwxr-xr-x   0 runner    (1001) docker     (123)    90602 2023-07-30 02:49:21.000000 scqubits-3.2.0/scqubits/core/qubit_img/Oscillator.jpg
+-rw-r--r--   0 runner    (1001) docker     (123)   154768 2023-07-30 02:49:21.000000 scqubits-3.2.0/scqubits/core/qubit_img/Snailmon.jpg
+-rw-r--r--   0 runner    (1001) docker     (123)    97656 2023-07-30 02:49:21.000000 scqubits-3.2.0/scqubits/core/qubit_img/Transmon.jpg
+-rw-r--r--   0 runner    (1001) docker     (123)   127799 2023-07-30 02:49:21.000000 scqubits-3.2.0/scqubits/core/qubit_img/TunableTransmon.jpg
+-rwxr-xr-x   0 runner    (1001) docker     (123)   116961 2023-07-30 02:49:21.000000 scqubits-3.2.0/scqubits/core/qubit_img/ZeroPi.jpg
+-rwxr-xr-x   0 runner    (1001) docker     (123)    16430 2023-07-30 02:49:21.000000 scqubits-3.2.0/scqubits/core/spec_lookup.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     9058 2023-07-30 02:49:21.000000 scqubits-3.2.0/scqubits/core/storage.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3071 2023-07-30 02:49:21.000000 scqubits-3.2.0/scqubits/core/sweeps.py
+-rw-r--r--   0 runner    (1001) docker     (123)    70528 2023-07-30 02:49:21.000000 scqubits-3.2.0/scqubits/core/symbolic_circuit.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    31586 2023-07-30 02:49:21.000000 scqubits-3.2.0/scqubits/core/transmon.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4865 2023-07-30 02:49:21.000000 scqubits-3.2.0/scqubits/core/units.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    33067 2023-07-30 02:49:21.000000 scqubits-3.2.0/scqubits/core/zeropi.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    29541 2023-07-30 02:49:21.000000 scqubits-3.2.0/scqubits/core/zeropi_full.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 02:49:31.318535 scqubits-3.2.0/scqubits/explorer/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-30 02:49:21.000000 scqubits-3.2.0/scqubits/explorer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11849 2023-07-30 02:49:21.000000 scqubits-3.2.0/scqubits/explorer/explorer_panels.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12577 2023-07-30 02:49:21.000000 scqubits-3.2.0/scqubits/explorer/explorer_settings.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24839 2023-07-30 02:49:21.000000 scqubits-3.2.0/scqubits/explorer/explorer_widget.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 02:49:31.322535 scqubits-3.2.0/scqubits/io_utils/
+-rwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 02:49:21.000000 scqubits-3.2.0/scqubits/io_utils/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     5914 2023-07-30 02:49:21.000000 scqubits-3.2.0/scqubits/io_utils/fileio.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    13959 2023-07-30 02:49:21.000000 scqubits-3.2.0/scqubits/io_utils/fileio_backends.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2395 2023-07-30 02:49:21.000000 scqubits-3.2.0/scqubits/io_utils/fileio_qutip.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    11332 2023-07-30 02:49:21.000000 scqubits-3.2.0/scqubits/io_utils/fileio_serializers.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     5414 2023-07-30 02:49:21.000000 scqubits-3.2.0/scqubits/settings.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      689 2023-07-30 02:49:21.000000 scqubits-3.2.0/scqubits/testing.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 02:49:31.326535 scqubits-3.2.0/scqubits/tests/
+-rwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 02:49:21.000000 scqubits-3.2.0/scqubits/tests/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     9776 2023-07-30 02:49:21.000000 scqubits-3.2.0/scqubits/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 02:49:31.338536 scqubits-3.2.0/scqubits/tests/data/
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-07-30 02:49:21.000000 scqubits-3.2.0/scqubits/tests/data/circuit_DFC.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       57 2023-07-30 02:49:21.000000 scqubits-3.2.0/scqubits/tests/data/circuit_fluxonium.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      146 2023-07-30 02:49:21.000000 scqubits-3.2.0/scqubits/tests/data/circuit_zeropi.yaml
+-rwxr-xr-x   0 runner    (1001) docker     (123)    15496 2023-07-30 02:49:21.000000 scqubits-3.2.0/scqubits/tests/data/cos2phiqubit_1.hdf5
+-rwxr-xr-x   0 runner    (1001) docker     (123)   214632 2023-07-30 02:49:21.000000 scqubits-3.2.0/scqubits/tests/data/cos2phiqubit_2.hdf5
+-rwxr-xr-x   0 runner    (1001) docker     (123)   472471 2023-07-30 02:49:21.000000 scqubits-3.2.0/scqubits/tests/data/cos2phiqubit_4.hdf5
+-rwxr-xr-x   0 runner    (1001) docker     (123)    16032 2023-07-30 02:49:21.000000 scqubits-3.2.0/scqubits/tests/data/cos2phiqubit_5.hdf5
+-rwxr-xr-x   0 runner    (1001) docker     (123)    15048 2023-07-30 02:49:21.000000 scqubits-3.2.0/scqubits/tests/data/fluxonium_1.hdf5
+-rwxr-xr-x   0 runner    (1001) docker     (123)    21667 2023-07-30 02:49:21.000000 scqubits-3.2.0/scqubits/tests/data/fluxonium_2.hdf5
+-rwxr-xr-x   0 runner    (1001) docker     (123)   367163 2023-07-30 02:49:21.000000 scqubits-3.2.0/scqubits/tests/data/fluxonium_4.hdf5
+-rwxr-xr-x   0 runner    (1001) docker     (123)    14512 2023-07-30 02:49:21.000000 scqubits-3.2.0/scqubits/tests/data/fluxonium_5.hdf5
+-rwxr-xr-x   0 runner    (1001) docker     (123)    14136 2023-07-30 02:49:21.000000 scqubits-3.2.0/scqubits/tests/data/fluxqubit_1.hdf5
+-rwxr-xr-x   0 runner    (1001) docker     (123)    39269 2023-07-30 02:49:21.000000 scqubits-3.2.0/scqubits/tests/data/fluxqubit_2.hdf5
+-rwxr-xr-x   0 runner    (1001) docker     (123)  1205265 2023-07-30 02:49:22.000000 scqubits-3.2.0/scqubits/tests/data/fluxqubit_4.hdf5
+-rwxr-xr-x   0 runner    (1001) docker     (123)    14960 2023-07-30 02:49:22.000000 scqubits-3.2.0/scqubits/tests/data/fluxqubit_5.hdf5
+-rwxr-xr-x   0 runner    (1001) docker     (123)    17920 2023-07-30 02:49:22.000000 scqubits-3.2.0/scqubits/tests/data/fullzeropi_1.hdf5
+-rw-r--r--   0 runner    (1001) docker     (123)    33599 2023-07-30 02:49:22.000000 scqubits-3.2.0/scqubits/tests/data/fullzeropi_2.hdf5
+-rw-r--r--   0 runner    (1001) docker     (123)    15824 2023-07-30 02:49:22.000000 scqubits-3.2.0/scqubits/tests/data/snailmon_1.hdf5
+-rw-r--r--   0 runner    (1001) docker     (123)    22048 2023-07-30 02:49:22.000000 scqubits-3.2.0/scqubits/tests/data/snailmon_2.hdf5
+-rw-r--r--   0 runner    (1001) docker     (123)   520543 2023-07-30 02:49:22.000000 scqubits-3.2.0/scqubits/tests/data/snailmon_4.hdf5
+-rw-r--r--   0 runner    (1001) docker     (123)    16360 2023-07-30 02:49:22.000000 scqubits-3.2.0/scqubits/tests/data/snailmon_5.hdf5
+-rwxr-xr-x   0 runner    (1001) docker     (123)    13624 2023-07-30 02:49:22.000000 scqubits-3.2.0/scqubits/tests/data/transmon_1.hdf5
+-rwxr-xr-x   0 runner    (1001) docker     (123)    18560 2023-07-30 02:49:22.000000 scqubits-3.2.0/scqubits/tests/data/transmon_2.hdf5
+-rwxr-xr-x   0 runner    (1001) docker     (123)   120906 2023-07-30 02:49:22.000000 scqubits-3.2.0/scqubits/tests/data/transmon_4.hdf5
+-rwxr-xr-x   0 runner    (1001) docker     (123)    14416 2023-07-30 02:49:22.000000 scqubits-3.2.0/scqubits/tests/data/transmon_5.hdf5
+-rwxr-xr-x   0 runner    (1001) docker     (123)     9024 2023-07-30 02:49:22.000000 scqubits-3.2.0/scqubits/tests/data/zeropi-test.hdf5
+-rwxr-xr-x   0 runner    (1001) docker     (123)    17664 2023-07-30 02:49:22.000000 scqubits-3.2.0/scqubits/tests/data/zeropi_1.hdf5
+-rwxr-xr-x   0 runner    (1001) docker     (123)   788882 2023-07-30 02:49:22.000000 scqubits-3.2.0/scqubits/tests/data/zeropi_2.hdf5
+-rwxr-xr-x   0 runner    (1001) docker     (123)  1761598 2023-07-30 02:49:22.000000 scqubits-3.2.0/scqubits/tests/data/zeropi_4.hdf5
+-rwxr-xr-x   0 runner    (1001) docker     (123)    18200 2023-07-30 02:49:22.000000 scqubits-3.2.0/scqubits/tests/data/zeropi_5.hdf5
+-rwxr-xr-x   0 runner    (1001) docker     (123)     9264 2023-07-30 02:49:22.000000 scqubits-3.2.0/scqubits/tests/data/zpifull-test.hdf5
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2659 2023-07-30 02:49:22.000000 scqubits-3.2.0/scqubits/tests/test_centraldispatch.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7666 2023-07-30 02:49:22.000000 scqubits-3.2.0/scqubits/tests/test_circuit.py
+-rw-r--r--   0 runner    (1001) docker     (123)      844 2023-07-30 02:49:22.000000 scqubits-3.2.0/scqubits/tests/test_circuit_plot.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1020 2023-07-30 02:49:22.000000 scqubits-3.2.0/scqubits/tests/test_cos2phiqubit.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2424 2023-07-30 02:49:22.000000 scqubits-3.2.0/scqubits/tests/test_explorer.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      951 2023-07-30 02:49:22.000000 scqubits-3.2.0/scqubits/tests/test_fluxonium.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      953 2023-07-30 02:49:22.000000 scqubits-3.2.0/scqubits/tests/test_fluxqubit.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2110 2023-07-30 02:49:22.000000 scqubits-3.2.0/scqubits/tests/test_fullzeropi.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      595 2023-07-30 02:49:22.000000 scqubits-3.2.0/scqubits/tests/test_gui.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    16570 2023-07-30 02:49:22.000000 scqubits-3.2.0/scqubits/tests/test_hilbertspace.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1509 2023-07-30 02:49:22.000000 scqubits-3.2.0/scqubits/tests/test_namedslotsndarray.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4762 2023-07-30 02:49:22.000000 scqubits-3.2.0/scqubits/tests/test_noise.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1545 2023-07-30 02:49:22.000000 scqubits-3.2.0/scqubits/tests/test_parameters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4191 2023-07-30 02:49:22.000000 scqubits-3.2.0/scqubits/tests/test_parametersweep.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    16340 2023-07-30 02:49:22.000000 scqubits-3.2.0/scqubits/tests/test_spectrumlookup.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1172 2023-07-30 02:49:22.000000 scqubits-3.2.0/scqubits/tests/test_transmon.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1349 2023-07-30 02:49:22.000000 scqubits-3.2.0/scqubits/tests/test_units.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1006 2023-07-30 02:49:22.000000 scqubits-3.2.0/scqubits/tests/test_zeropi.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 02:49:31.342536 scqubits-3.2.0/scqubits/ui/
+-rwxr-xr-x   0 runner    (1001) docker     (123)      619 2023-07-30 02:49:22.000000 scqubits-3.2.0/scqubits/ui/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    66972 2023-07-30 02:49:22.000000 scqubits-3.2.0/scqubits/ui/gui.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17276 2023-07-30 02:49:22.000000 scqubits-3.2.0/scqubits/ui/gui_custom_widgets.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11368 2023-07-30 02:49:22.000000 scqubits-3.2.0/scqubits/ui/gui_defaults.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3719 2023-07-30 02:49:22.000000 scqubits-3.2.0/scqubits/ui/gui_navbar.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15936 2023-07-30 02:49:22.000000 scqubits-3.2.0/scqubits/ui/gui_setup.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    21538 2023-07-30 02:49:22.000000 scqubits-3.2.0/scqubits/ui/hspace_widget.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 02:49:31.342536 scqubits-3.2.0/scqubits/ui/icons/
+-rw-r--r--   0 runner    (1001) docker     (123)     3660 2023-07-30 02:49:22.000000 scqubits-3.2.0/scqubits/ui/icons/En.png
+-rw-r--r--   0 runner    (1001) docker     (123)     5345 2023-07-30 02:49:22.000000 scqubits-3.2.0/scqubits/ui/icons/Me.png
+-rw-r--r--   0 runner    (1001) docker     (123)     9994 2023-07-30 02:49:22.000000 scqubits-3.2.0/scqubits/ui/icons/MeS.png
+-rw-r--r--   0 runner    (1001) docker     (123)     6495 2023-07-30 02:49:22.000000 scqubits-3.2.0/scqubits/ui/icons/T1.png
+-rw-r--r--   0 runner    (1001) docker     (123)    11754 2023-07-30 02:49:22.000000 scqubits-3.2.0/scqubits/ui/icons/psi.png
+-rw-r--r--   0 runner    (1001) docker     (123)     7272 2023-07-30 02:49:22.000000 scqubits-3.2.0/scqubits/ui/icons/scq-logo.png
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3167 2023-07-30 02:49:22.000000 scqubits-3.2.0/scqubits/ui/qubit_widget.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 02:49:31.342536 scqubits-3.2.0/scqubits/utils/
+-rwxr-xr-x   0 runner    (1001) docker     (123)      619 2023-07-30 02:49:22.000000 scqubits-3.2.0/scqubits/utils/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1856 2023-07-30 02:49:22.000000 scqubits-3.2.0/scqubits/utils/cpu_switch.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    13783 2023-07-30 02:49:22.000000 scqubits-3.2.0/scqubits/utils/misc.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     6892 2023-07-30 02:49:22.000000 scqubits-3.2.0/scqubits/utils/plot_defaults.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7046 2023-07-30 02:49:22.000000 scqubits-3.2.0/scqubits/utils/plot_utils.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    18985 2023-07-30 02:49:22.000000 scqubits-3.2.0/scqubits/utils/plotting.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    15915 2023-07-30 02:49:22.000000 scqubits-3.2.0/scqubits/utils/spectrum_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1293 2023-07-30 02:49:22.000000 scqubits-3.2.0/scqubits/utils/typedefs.py
+-rw-r--r--   0 runner    (1001) docker     (123)      105 2023-07-30 02:49:31.000000 scqubits-3.2.0/scqubits/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 02:49:31.306534 scqubits-3.2.0/scqubits.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1892 2023-07-30 02:49:31.000000 scqubits-3.2.0/scqubits.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4261 2023-07-30 02:49:31.000000 scqubits-3.2.0/scqubits.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-30 02:49:31.000000 scqubits-3.2.0/scqubits.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-30 02:49:31.000000 scqubits-3.2.0/scqubits.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      239 2023-07-30 02:49:31.000000 scqubits-3.2.0/scqubits.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      101 2023-07-30 02:49:31.000000 scqubits-3.2.0/scqubits.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-30 02:49:31.342536 scqubits-3.2.0/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4723 2023-07-30 02:49:22.000000 scqubits-3.2.0/setup.py
```

### Comparing `scqubits-3.1.1/LICENSE` & `scqubits-3.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `scqubits-3.1.1/PKG-INFO` & `scqubits-3.2.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: scqubits
-Version: 3.1.1
+Version: 3.2.0
 Summary: scqubits: superconducting qubits in Python
 Home-page: https://scqubits.readthedocs.io
 Author: Jens Koch, Peter Groszkowski
 Author-email: jens-koch@northwestern.edu, piotrekg@gmail.com
 License: BSD
 Keywords: superconducting qubits
 Platform: Linux
@@ -22,15 +22,14 @@
 Classifier: Operating System :: Unix
 Classifier: Operating System :: Microsoft :: Windows
 Requires-Python: >=3.7
 Provides-Extra: graphics
 Provides-Extra: explorer
 Provides-Extra: h5-support
 Provides-Extra: pathos
-Provides-Extra: fitting
 License-File: LICENSE
 
 
 scqubits is an open-source Python library for simulating superconducting qubits. It is
 meant to give the user a convenient way to obtain energy spectra of common
 superconducting qubits, plot energy levels as a function of external parameters,
 calculate matrix elements etc. The library further provides an interface to QuTiP,
```

### Comparing `scqubits-3.1.1/README.md` & `scqubits-3.2.0/README.md`

 * *Files 16% similar despite different names*

```diff
@@ -4,35 +4,44 @@
 [![Anaconda-Server Badge](https://anaconda.org/conda-forge/scqubits/badges/downloads.svg)](https://anaconda.org/conda-forge/scqubits)
 [![CodeFactor](https://www.codefactor.io/repository/github/scqubits/scqubits/badge)](https://www.codefactor.io/repository/github/scqubits/scqubits)
 [![codecov](https://codecov.io/gh/scqubits/scqubits/branch/master/graph/badge.svg?token=PUBXSHF6HU)](https://codecov.io/gh/scqubits/scqubits)
 
 
 [J. Koch](https://github.com/jkochNU), [P. Groszkowski](https://github.com/petergthatsme)
 
+<br>
+
+> **Join the scqubits mailing list!** Receive information about new releases
+> and opportunities to contribute
+> to new developments.
+> |[SIGN UP](https://sites.northwestern.edu/koch/scqubits-news-sign-up/)|
+> |---------------------------------------------------------------------|
+
+<br>
 
 scqubits is an open-source Python library for simulating superconducting qubits. It is meant to give the user
 a convenient way to obtain energy spectra of common superconducting qubits, plot energy levels as a function of
 external parameters, calculate matrix elements etc. The library further provides an interface to QuTiP, making it
 easy to work with composite Hilbert spaces consisting of coupled superconducting qubits and harmonic modes.
 Internally, numerics within scqubits is carried out with the help of Numpy and Scipy; plotting capabilities rely on
 Matplotlib.
 
 If scqubits is helpful to you in your research, please support its continued 
 development and maintenance. Use of scqubits in research publications is 
 appropriately acknowledged by citing:
 
->  Peter Groszkowski and Jens Koch,<br> 
->  *scqubits:  a Python package for superconducting qubits*,<br>
->  Quantum 5, 583 (2021).<br>
->  https://quantum-journal.org/papers/q-2021-11-17-583/
->
->  Sai Pavan Chitta, Tianpu Zhao, Ziwen Huang, Ian Mondragon-Shem, and Jens Koch,<br>
->  *Computer-aided quantization and numerical analysis of superconducting circuits*,<br>
->  arXiv:2206.08320 (2022).<br>
->  https://arxiv.org/abs/2206.08320
+&nbsp; &nbsp; Peter Groszkowski and Jens Koch,<br> 
+&nbsp; &nbsp; *scqubits:  a Python package for superconducting qubits*,<br>
+&nbsp; &nbsp; Quantum 5, 583 (2021).<br>
+&nbsp; &nbsp; https://quantum-journal.org/papers/q-2021-11-17-583/
+
+&nbsp; &nbsp; Sai Pavan Chitta, Tianpu Zhao, Ziwen Huang, Ian Mondragon-Shem, and Jens Koch,<br>
+&nbsp; &nbsp; *Computer-aided quantization and numerical analysis of superconducting circuits*,<br>
+&nbsp; &nbsp; New J. Phys. 24 103020 (2022).<br>
+&nbsp; &nbsp; https://iopscience.iop.org/article/10.1088/1367-2630/ac94f2
 
 
 
 Download and Installation
 -------------------------
 
 For Python 3.7, 3.8, 3.9, and 3.10: installation via conda is supported.
```

### Comparing `scqubits-3.1.1/scqubits/__init__.py` & `scqubits-3.2.0/scqubits/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -23,18 +23,23 @@
 
 from scqubits import settings
 
 # core
 from scqubits.core.central_dispatch import CentralDispatch
 from scqubits.core.cos2phi_qubit import Cos2PhiQubit
 from scqubits.core.discretization import Grid1d
+from scqubits.core.diag import DIAG_METHODS
 from scqubits.core.flux_qubit import FluxQubit
 from scqubits.core.fluxonium import Fluxonium
 from scqubits.core.generic_qubit import GenericQubit
-from scqubits.core.hilbert_space import HilbertSpace, InteractionTerm
+from scqubits.core.hilbert_space import (
+    HilbertSpace,
+    InteractionTerm,
+    InteractionTermStr,
+)
 from scqubits.core.noise import calc_therm_ratio
 from scqubits.core.oscillator import KerrOscillator, Oscillator
 from scqubits.core.param_sweep import ParameterSweep
 from scqubits.core.storage import DataStore, SpectrumData
 from scqubits.core.transmon import Transmon, TunableTransmon
 from scqubits.core.units import (
     from_standard_units,
@@ -46,32 +51,43 @@
 )
 from scqubits.core.zeropi import ZeroPi
 from scqubits.core.zeropi_full import FullZeroPi
 
 # file IO
 from scqubits.io_utils.fileio import read, write
 
+# diagonalization
+import scqubits.core.diag as diag
+from scqubits.core.diag import (
+    DIAG_METHODS,
+)
 
 # Import of custom-circuit modules needs to take place after other imports to
 # avoid circular import issues
 from scqubits.core.circuit import Circuit
 from scqubits.core.circuit_utils import truncation_template
 from scqubits.core.symbolic_circuit import SymbolicCircuit
 
 
 # GUI
 try:
-    from scqubits.ui.explorer_widget import Explorer
+    from scqubits.explorer.explorer_widget import Explorer
     from scqubits.ui.gui import GUI
-except NameError:
-    warnings.warn(
-        "scqubits: could not import GUI/Explorer - consider installing ipywidgets "
-        "(optional dependency)?",
-        ImportWarning,
-    )
+except (ImportError, NameError):
+
+    def Explorer(*args, **kwargs):
+        warnings.warn(
+            "scqubits: could not create Explorer - did you install the optional dependency ipyvuetify?"
+        )
+
+    def GUI(*args, **kwargs):
+        warnings.warn(
+            "scqubits: could not create GUI - did you install the optional dependency ipyvuetify?"
+        )
+
 
 # for showing scqubits info
 from scqubits.utils.misc import about, cite
 
 # spectrum utils
 from scqubits.utils.spectrum_utils import identity_wrap
```

### Comparing `scqubits-3.1.1/scqubits/core/central_dispatch.py` & `scqubits-3.2.0/scqubits/core/central_dispatch.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,14 +11,15 @@
 ############################################################################
 
 
 import logging
 import warnings
 import weakref
 from types import MethodType
+from typing import Optional
 from weakref import WeakKeyDictionary
 
 import scqubits.settings as settings
 
 LOGGER = logging.getLogger(__name__)
 
 # ---------------------------------------------------------------
@@ -64,15 +65,15 @@
         Returns
         -------
         dict
         """
         return self.clients_dict[event]
 
     def register(
-        self, event: str, who: "DispatchClient", callback: MethodType = None
+        self, event: str, who: "DispatchClient", callback: Optional[MethodType] = None
     ) -> None:
         """
         Register object `who` for event `event`. (This modifies `clients_dict`.)
 
         Parameters
         ----------
         event: str
```

### Comparing `scqubits-3.1.1/scqubits/core/circuit.py` & `scqubits-3.2.0/scqubits/core/circuit.py`

 * *Files 1% similar despite different names*

```diff
@@ -19,15 +19,14 @@
 from types import MethodType
 from typing import Any, Callable, Dict, List, Optional, Tuple, Union
 
 import numpy as np
 import qutip as qt
 import scipy as sp
 import sympy as sm
-
 from matplotlib import pyplot as plt
 from matplotlib.axes import Axes
 from matplotlib.figure import Figure
 from numpy import ndarray
 from scipy import sparse
 from scipy.sparse import csc_matrix
 from sympy import latex
@@ -122,14 +121,21 @@
         hamiltonian_symbolic: sm.Expr,
         system_hierarchy: Optional[List] = None,
         subsystem_trunc_dims: Optional[List] = None,
         truncated_dim: Optional[int] = 10,
     ):
         base.QuantumSystem.__init__(self, id_str=None)
 
+        # This class does not yet support custom diagonalization options, but these
+        # still have to be defined
+        self.evals_method = None
+        self.evals_method_options = None
+        self.esys_method = None
+        self.esys_method_options = None
+
         self.system_hierarchy = system_hierarchy
         self.truncated_dim = truncated_dim
         self.subsystem_trunc_dims = subsystem_trunc_dims
 
         self.is_child = True
         self.parent = parent
         self.hamiltonian_symbolic = hamiltonian_symbolic
@@ -825,15 +831,15 @@
                             list(self.subsystems.values()),
                             evecs=self.subsystems[subsys_index].get_eigenstates(),
                         )
         operator_list = list(operator_dict.values())
         return functools.reduce(builtin_op.mul, operator_list)
 
     def _generate_symbols_list(
-        self, var_str: str, iterable_list: List[int] or ndarray
+        self, var_str: str, iterable_list: Union[List[int], ndarray]
     ) -> List[sm.Symbol]:
         """
         Returns the list of symbols generated using the var_str + iterable as the name
         of the symbol.
 
         Parameters
         ----------
@@ -2903,14 +2909,21 @@
         symbolic_circuit = SymbolicCircuit.from_yaml(
             input_string,
             from_file=from_file,
             basis_completion=basis_completion,
             initiate_sym_calc=True,
         )
 
+        # This class does not yet support custom diagonalization options, but these
+        # still have to be defined
+        self.evals_method = None
+        self.evals_method_options = None
+        self.esys_method = None
+        self.esys_method_options = None
+
         sm.init_printing(pretty_print=False, order="none")
         self.is_child = False
         self.symbolic_circuit: SymbolicCircuit = symbolic_circuit
 
         self.ext_basis: str = ext_basis
         self.truncated_dim: int = truncated_dim
         self.system_hierarchy: list = None
```

### Comparing `scqubits-3.1.1/scqubits/core/circuit_utils.py` & `scqubits-3.2.0/scqubits/core/circuit_utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -7,20 +7,18 @@
 #    All rights reserved.
 #
 #    This source code is licensed under the BSD-style license found in the
 #    LICENSE file in the root directory of this source tree.
 ############################################################################
 
 import re
-
 from typing import TYPE_CHECKING, Any, Callable, List, Union
 
 import numpy as np
 import sympy as sm
-
 from numpy import ndarray
 from scipy import sparse
 from scipy.sparse import csc_matrix
 
 from scqubits.core import discretization as discretization
 from scqubits.utils.misc import flatten_list_recursive
```

### Comparing `scqubits-3.1.1/scqubits/core/constants.py` & `scqubits-3.2.0/scqubits/core/constants.py`

 * *Files identical despite different names*

### Comparing `scqubits-3.1.1/scqubits/core/cos2phi_qubit.py` & `scqubits-3.2.0/scqubits/core/cos2phi_qubit.py`

 * *Files 4% similar despite different names*

```diff
@@ -7,15 +7,14 @@
 #    All rights reserved.
 #
 #    This source code is licensed under the BSD-style license found in the
 #    LICENSE file in the root directory of this source tree.
 ############################################################################
 
 import math
-import os
 
 from abc import ABC, abstractmethod
 from typing import Any, Callable, Dict, List, Optional, Tuple, Union
 
 import numpy as np
 import scipy as sp
 
@@ -441,19 +440,19 @@
     dEJ:
         disorder in junction energy
     flux:
         external magnetic flux in units of one flux quantum
     ng:
         offset charge
     ncut:
-        cutoff of charge basis, -ncut <= :math:`n_\theta` <= ncut
+        cutoff in charge basis, -ncut <= :math:`n_\theta` <= ncut
     zeta_cut:
-        number of harmonic oscillator basis for :math:`\zeta` variable
+        number of harmonic oscillator basis states for :math:`\zeta` variable
     phi_cut:
-        number of harmonic oscillator basis for :math:`\phi` variable
+        number of harmonic oscillator basis states for :math:`\phi` variable
     truncated_dim:
         desired dimension of the truncated quantum system; expected: truncated_dim > 1
     id_str:
         optional string by which this instance can be referred to in `HilbertSpace`
         and `ParameterSweep`. If not provided, an id is auto-generated.
     """
     EJ = descriptors.WatchedProperty(float, "QUANTUMSYSTEM_UPDATE")
@@ -481,16 +480,27 @@
         flux: float,
         ng: float,
         ncut: int,
         zeta_cut: int,
         phi_cut: int,
         truncated_dim: int = 6,
         id_str: Optional[str] = None,
+        evals_method: Optional[str] = None,
+        evals_method_options: Optional[dict] = None,
+        esys_method: Optional[str] = None,
+        esys_method_options: Optional[dict] = None,
     ) -> None:
-        base.QuantumSystem.__init__(self, id_str=id_str)
+        base.QubitBaseClass.__init__(
+            self,
+            id_str=id_str,
+            evals_method=evals_method,
+            evals_method_options=evals_method_options,
+            esys_method=esys_method,
+            esys_method_options=esys_method_options,
+        )
         self.EJ = EJ
         self.ECJ = ECJ
         self.EL = EL
         self.EC = EC
         self.dL = dL
         self.dCJ = dCJ
         self.dEJ = dEJ
@@ -499,18 +509,14 @@
         self.ncut = ncut
         self.zeta_cut = zeta_cut
         self.phi_cut = phi_cut
         self.truncated_dim = truncated_dim
         self._default_phi_grid = discretization.Grid1d(-4 * np.pi, 4 * np.pi, 100)
         self._default_zeta_grid = discretization.Grid1d(-4 * np.pi, 4 * np.pi, 100)
         self._default_theta_grid = discretization.Grid1d(-0.5 * np.pi, 1.5 * np.pi, 100)
-        self._image_filename = os.path.join(
-            os.path.dirname(os.path.abspath(__file__)),
-            "qubit_img/cos2phi-qubit.jpg",
-        )
 
     @staticmethod
     def default_params() -> Dict[str, Any]:
         return {
             "EJ": 15.0,
             "ECJ": 2.0,
             "EL": 1.0,
```

### Comparing `scqubits-3.1.1/scqubits/core/descriptors.py` & `scqubits-3.2.0/scqubits/core/descriptors.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 #
 #    This source code is licensed under the BSD-style license found in the
 #    LICENSE file in the root directory of this source tree.
 ############################################################################
 
 # Recap on descriptors: see https://realpython.com/python-descriptors/
 
-from typing import Any, Generic, Type, TypeVar
+from typing import Any, Generic, Optional, Type, TypeVar
 
 from scqubits.core.central_dispatch import DispatchClient
 
 TargetType = TypeVar("TargetType")
 
 
 class ReadOnlyProperty(Generic[TargetType]):
@@ -58,16 +58,16 @@
         instance class, obtained in __set_name__
     """
 
     def __init__(
         self,
         target_type: Type[TargetType],
         event: str,
-        inner_object_name: str = None,
-        attr_name: str = None,
+        inner_object_name: Optional[str] = None,
+        attr_name: Optional[str] = None,
     ) -> None:
         self.event = event
         self.inner = inner_object_name
         self.attr_name = attr_name
 
     def __set_name__(self, owner, name: str) -> None:
         self.name = name
```

### Comparing `scqubits-3.1.1/scqubits/core/discretization.py` & `scqubits-3.2.0/scqubits/core/discretization.py`

 * *Files identical despite different names*

### Comparing `scqubits-3.1.1/scqubits/core/flux_qubit.py` & `scqubits-3.2.0/scqubits/core/flux_qubit.py`

 * *Files 3% similar despite different names*

```diff
@@ -6,16 +6,14 @@
 #    Copyright (c) 2019 and later, Jens Koch and Peter Groszkowski
 #    All rights reserved.
 #
 #    This source code is licensed under the BSD-style license found in the
 #    LICENSE file in the root directory of this source tree.
 ############################################################################
 
-import os
-
 from abc import ABC, abstractmethod
 from typing import Any, Dict, List, Optional, Tuple, Union
 
 import numpy as np
 import scipy as sp
 
 from matplotlib.axes import Axes
@@ -333,16 +331,27 @@
         ECg2: float,
         ng1: float,
         ng2: float,
         flux: float,
         ncut: int,
         truncated_dim: int = 6,
         id_str: Optional[str] = None,
+        evals_method: Optional[str] = None,
+        evals_method_options: Optional[dict] = None,
+        esys_method: Optional[str] = None,
+        esys_method_options: Optional[dict] = None,
     ) -> None:
-        base.QuantumSystem.__init__(self, id_str=id_str)
+        base.QubitBaseClass.__init__(
+            self,
+            id_str=id_str,
+            evals_method=evals_method,
+            evals_method_options=evals_method_options,
+            esys_method=esys_method,
+            esys_method_options=esys_method_options,
+        )
         self.EJ1 = EJ1
         self.EJ2 = EJ2
         self.EJ3 = EJ3
         self.ECJ1 = ECJ1
         self.ECJ2 = ECJ2
         self.ECJ3 = ECJ3
         self.ECg1 = ECg1
@@ -351,17 +360,14 @@
         self.ng2 = ng2
         self.flux = flux
         self.ncut = ncut
         self.truncated_dim = truncated_dim
         self._default_grid = discretization.Grid1d(
             -np.pi / 2, 3 * np.pi / 2, 100
         )  # for plotting in phi_j basis
-        self._image_filename = os.path.join(
-            os.path.dirname(os.path.abspath(__file__)), "qubit_img/flux-qubit.jpg"
-        )
 
     @staticmethod
     def default_params() -> Dict[str, Any]:
         return {
             "EJ1": 1.0,
             "EJ2": 1.0,
             "EJ3": 0.8,
@@ -381,14 +387,15 @@
     def supported_noise_channels(cls) -> List[str]:
         """Return a list of supported noise channels"""
         return [
             "tphi_1_over_f_cc1",
             "tphi_1_over_f_cc2",
             "tphi_1_over_f_cc3",
             "tphi_1_over_f_cc",
+            "tphi_1_over_f_flux",
             # 'tphi_1_over_f_ng1',
             # 'tphi_1_over_f_ng2',
             # 'tphi_1_over_f_ng',
         ]
 
     def EC_matrix(self) -> ndarray:
         """Return the charging energy matrix"""
@@ -405,22 +412,28 @@
         Cmat[1, 0] = -CJ3
 
         return np.linalg.inv(Cmat) / 2.0
 
     def _evals_calc(self, evals_count: int) -> ndarray:
         hamiltonian_mat = self.hamiltonian()
         evals = sp.linalg.eigh(
-            hamiltonian_mat, subset_by_index=(0, evals_count - 1), eigvals_only=True
+            hamiltonian_mat,
+            subset_by_index=(0, evals_count - 1),
+            eigvals_only=True,
+            check_finite=False,
         )
         return np.sort(evals)
 
     def _esys_calc(self, evals_count: int) -> Tuple[ndarray, ndarray]:
         hamiltonian_mat = self.hamiltonian()
         evals, evecs = sp.linalg.eigh(
-            hamiltonian_mat, subset_by_index=(0, evals_count - 1), eigvals_only=False
+            hamiltonian_mat,
+            subset_by_index=(0, evals_count - 1),
+            eigvals_only=False,
+            check_finite=False,
         )
         evals, evecs = spec_utils.order_eigensystem(evals, evecs)
         return evals, evecs
 
     def hilbertdim(self) -> int:
         """Return Hilbert space dimension."""
         return (2 * self.ncut + 1) ** 2
@@ -620,14 +633,56 @@
             * (
                 np.exp(-1j * 2 * np.pi * self.flux)
                 * np.kron(self._exp_i_phi_operator().T, self._exp_i_phi_operator())
             )
         )
         return self.process_op(native_op=native, energy_esys=energy_esys)
 
+    def d_hamiltonian_d_flux(
+        self, energy_esys: Union[bool, Tuple[ndarray, ndarray]] = False
+    ) -> ndarray:
+        """
+        Returns the operator representing a derivative of the Hamiltonian with respect to flux
+        in the native Hamiltonian basis or eigenenergy basis.
+
+        Parameters
+        ----------
+        energy_esys:
+            If `False` (default), returns operator in the native Hamiltonian basis.
+            If `True`, the energy eigenspectrum is computed, returns operator in the energy eigenbasis.
+            If `energy_esys = esys`, where esys is a tuple containing two ndarrays (eigenvalues and energy eigenvectors),
+            returns operator in the energy eigenbasis, and does not have to recalculate eigenspectrum.
+
+        Returns
+        -------
+            Operator in chosen basis as ndarray. If the eigenenergy basis is chosen,
+            unless `energy_esys` is specified, operator has dimensions of `truncated_dim`
+            x `truncated_dim`. Otherwise, if eigenenergy basis is chosen, operator has dimensions of m x m,
+            for m given eigenvectors.
+        """
+        native = (
+            2j
+            * np.pi
+            * (
+                -0.5
+                * self.EJ3
+                * (
+                    np.exp(1j * 2 * np.pi * self.flux)
+                    * np.kron(self._exp_i_phi_operator(), self._exp_i_phi_operator().T)
+                )
+                + 0.5
+                * self.EJ3
+                * (
+                    np.exp(-1j * 2 * np.pi * self.flux)
+                    * np.kron(self._exp_i_phi_operator().T, self._exp_i_phi_operator())
+                )
+            )
+        )
+        return self.process_op(native_op=native, energy_esys=energy_esys)
+
     def _n_operator(self) -> ndarray:
         diag_elements = np.arange(-self.ncut, self.ncut + 1, dtype=np.complex_)
         return np.diag(diag_elements)
 
     def _exp_i_phi_operator(self) -> ndarray:
         dim = 2 * self.ncut + 1
         off_diag_elements = np.ones(dim - 1, dtype=np.complex_)
```

### Comparing `scqubits-3.1.1/scqubits/core/fluxonium.py` & `scqubits-3.2.0/scqubits/core/fluxonium.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,15 +8,14 @@
 #
 #    This source code is licensed under the BSD-style license found in the
 #    LICENSE file in the root directory of this source tree.
 ############################################################################
 
 import cmath
 import math
-import os
 
 from typing import TYPE_CHECKING, Any, Dict, List, Optional, Tuple, Union
 
 import numpy as np
 import scipy as sp
 
 from numpy import ndarray
@@ -73,26 +72,34 @@
         EJ: float,
         EC: float,
         EL: float,
         flux: float,
         cutoff: int,
         truncated_dim: int = 6,
         id_str: Optional[str] = None,
+        evals_method: Optional[str] = None,
+        evals_method_options: Optional[dict] = None,
+        esys_method: Optional[str] = None,
+        esys_method_options: Optional[dict] = None,
     ) -> None:
-        base.QuantumSystem.__init__(self, id_str=id_str)
+        base.QubitBaseClass.__init__(
+            self,
+            id_str=id_str,
+            evals_method=evals_method,
+            evals_method_options=evals_method_options,
+            esys_method=esys_method,
+            esys_method_options=esys_method_options,
+        )
         self.EJ = EJ
         self.EC = EC
         self.EL = EL
         self.flux = flux
         self.cutoff = cutoff
         self.truncated_dim = truncated_dim
         self._default_grid = discretization.Grid1d(-4.5 * np.pi, 4.5 * np.pi, 151)
-        self._image_filename = os.path.join(
-            os.path.dirname(os.path.abspath(__file__)), "qubit_img/fluxonium.jpg"
-        )
 
     @staticmethod
     def default_params() -> Dict[str, Any]:
         return {
             "EJ": 8.9,
             "EC": 2.5,
             "EL": 0.5,
```

### Comparing `scqubits-3.1.1/scqubits/core/generic_qubit.py` & `scqubits-3.2.0/scqubits/core/generic_qubit.py`

 * *Files identical despite different names*

### Comparing `scqubits-3.1.1/scqubits/core/hilbert_space.py` & `scqubits-3.2.0/scqubits/core/hilbert_space.py`

 * *Files 2% similar despite different names*

```diff
@@ -35,14 +35,15 @@
 
 from numpy import ndarray
 from qutip.qobj import Qobj
 from scipy.sparse import csc_matrix, dia_matrix
 
 import scqubits.core.central_dispatch as dispatch
 import scqubits.core.descriptors as descriptors
+import scqubits.core.diag as diag
 import scqubits.core.oscillator as osc
 import scqubits.core.spec_lookup as spec_lookup
 import scqubits.core.storage as storage
 import scqubits.io_utils.fileio_qutip
 import scqubits.io_utils.fileio_serializers as serializers
 import scqubits.settings as settings
 import scqubits.ui.hspace_widget
@@ -50,14 +51,15 @@
 import scqubits.utils.misc as utils
 import scqubits.utils.spectrum_utils as spec_utils
 
 from scqubits.core.namedslots_array import NamedSlotsNdarray, Parameters
 from scqubits.core.storage import SpectrumData
 from scqubits.io_utils.fileio_qutip import QutipEigenstates
 
+
 if settings.IN_IPYTHON:
     from tqdm.notebook import tqdm
 else:
     from tqdm import tqdm
 
 if TYPE_CHECKING:
     from scqubits.io_utils.fileio import IOData
@@ -87,23 +89,24 @@
         list of tuples (subsys_index, operator)
     add_hc:
         If set to True, the interaction Hamiltonian is of type 2, and the Hermitian
         conjugate is added.
     """
 
     g_strength = descriptors.WatchedProperty(complex, "INTERACTIONTERM_UPDATE")
+
     operator_list = descriptors.WatchedProperty(
-        List[Tuple[int, Union[ndarray, csc_matrix]]], "INTERACTIONTERM_UPDATE"
-    )
+        List[Tuple[int, Union[ndarray, csc_matrix, Callable]]], "INTERACTIONTERM_UPDATE"
+    )  # Each item in the operator_list is a tuple (subsys_index, operator)
     add_hc = descriptors.WatchedProperty(bool, "INTERACTIONTERM_UPDATE")
 
     def __init__(
         self,
         g_strength: Union[float, complex],
-        operator_list: List[Tuple[int, Union[ndarray, csc_matrix]]],
+        operator_list: List[Tuple[int, Union[ndarray, csc_matrix, Callable]]],
         add_hc: bool = False,
     ) -> None:
         self.g_strength = g_strength
         self.operator_list = operator_list
         self.add_hc = add_hc
 
     def __repr__(self) -> str:
@@ -157,27 +160,63 @@
             hamiltonian *= op
         if self.add_hc:
             hamiltonian += hamiltonian.dag()
         return hamiltonian
 
     @staticmethod
     def id_wrap_all_ops(
-        operator_list: List[Tuple[int, Union[ndarray, csc_matrix]]],
+        operator_list: List[Tuple[int, Union[ndarray, csc_matrix, Callable]]],
         subsystem_list: List[QuantumSys],
         bare_esys: Optional[Dict[int, ndarray]] = None,
-    ) -> list:
+    ) -> List[Qobj]:
+        """
+        Returns a list of identity-wrapped operators, one for each operator in
+        operator_list. Note: at this point, any callable operator is actually evaluated.
+
+        Parameters
+        ----------
+        operator_list:
+            list of tuples (subsys_index, operator)
+        subsystem_list:
+            list of all quantum systems in HilbertSpace calling ``hamiltonian``,
+            needed for identity wrapping
+        bare_esys:
+            optionally, the bare eigensystems for each subsystem can be provided to
+            speed up computation; these are provided in dict form via <subsys>: esys)
+
+        Returns
+        -------
+            list of identity-wrapped operators
+
+        """
         id_wrapped_operators = []
         for subsys_index, operator in operator_list:
             if bare_esys is not None and subsys_index in bare_esys:
-                evecs = bare_esys[subsys_index][1]
+                esys = bare_esys[subsys_index]
+                evecs = esys[1]
             else:
+                esys = None
                 evecs = None
+
+            if callable(operator):
+                try:
+                    operator = operator(energy_esys=esys)
+                except TypeError:
+                    operator = operator()
+                op_in_eigenbasis = bool(esys)
+            else:
+                op_in_eigenbasis = False
+
             id_wrapped_operators.append(
                 spec_utils.identity_wrap(
-                    operator, subsystem_list[subsys_index], subsystem_list, evecs=evecs
+                    operator,
+                    subsystem_list[subsys_index],
+                    subsystem_list,
+                    evecs=evecs,
+                    op_in_eigenbasis=op_in_eigenbasis,
                 )
             )
         return id_wrapped_operators
 
 
 class InteractionTermStr(dispatch.DispatchClient, serializers.Serializable):
     """
@@ -339,14 +378,18 @@
     )
 
     def __init__(
         self,
         subsystem_list: List[QuantumSys],
         interaction_list: List[Union[InteractionTerm, InteractionTermStr]] = None,
         ignore_low_overlap: bool = False,
+        evals_method: Optional[str] = None,
+        evals_method_options: Optional[dict] = None,
+        esys_method: Optional[str] = None,
+        esys_method_options: Optional[dict] = None,
     ) -> None:
         if has_duplicate_id_str(subsystem_list):
             raise ValueError(
                 "Subsystem list must not contain multiple objects with "
                 "the same `id_str` name."
             )
         self._subsystems: List[QuantumSys] = subsystem_list
@@ -365,14 +408,19 @@
         self._osc_subsys_list = [
             subsys for subsys in self if isinstance(subsys, osc.Oscillator)
         ]
         self._qbt_subsys_list = [
             subsys for subsys in self if not isinstance(subsys, osc.Oscillator)
         ]
 
+        self.evals_method = evals_method
+        self.evals_method_options = evals_method_options
+        self.esys_method = esys_method
+        self.esys_method_options = esys_method_options
+
         # The following attributes are for compatibility with SpectrumLookupMixin
         self._data: Dict[str, Any] = {}
         self._parameters = Parameters({"dummy_parameter": np.array([0])})
         self._ignore_low_overlap = ignore_low_overlap
         self._current_param_indices = 0
         self._evals_count = self.dimension
         self._out_of_sync = False
@@ -537,15 +585,15 @@
     def subsystem_dims(self) -> List[int]:
         """Returns list of the Hilbert space dimensions of each subsystem"""
         return [subsystem.truncated_dim for subsystem in self]
 
     @property
     def dimension(self) -> int:
         """Returns total dimension of joint Hilbert space"""
-        return np.prod(np.asarray(self.subsystem_dims))  # type:ignore
+        return np.prod(np.asarray(self.subsystem_dims)).item()
 
     @property
     def subsystem_count(self) -> int:
         """Returns number of subsystems composing the joint Hilbert space"""
         return len(self._subsystems)
 
     ###################################################################################
@@ -615,51 +663,91 @@
     # HilbertSpace: energy spectrum
     ##################################################################################
     def eigenvals(
         self,
         evals_count: int = 6,
         bare_esys: Optional[Dict[int, Union[ndarray, List[ndarray]]]] = None,
     ) -> ndarray:
-        """Calculates eigenvalues of the full Hamiltonian using
-        `qutip.Qobj.eigenenergies()`.
+        """Calculates eigenvalues of the full Hamiltonian. Qutip's `qutip.Qobj.eigenenergies()` is
+        used by default, unless `self.evals_method` has been set to something other than `None`.
 
         Parameters
         ----------
         evals_count:
             number of desired eigenvalues/eigenstates
         bare_esys:
             optionally, the bare eigensystems for each subsystem can be provided to
             speed up computation; these are provided in dict form via <subsys>: esys
         """
+        # hamiltonian_mat = self.hamiltonian(bare_esys=bare_esys)  # type:ignore
+        # return hamiltonian_mat.eigenenergies(eigvals=evals_count)
+
         hamiltonian_mat = self.hamiltonian(bare_esys=bare_esys)  # type:ignore
-        return hamiltonian_mat.eigenenergies(eigvals=evals_count)
+
+        if not hasattr(self, "evals_method") or self.evals_method is None:
+            evals = hamiltonian_mat.eigenenergies(eigvals=evals_count)
+        else:
+            diagonalizer = (
+                diag.DIAG_METHODS[self.evals_method]
+                if isinstance(self.evals_method, str)
+                else self.evals_method
+            )
+            evals = diagonalizer(
+                hamiltonian_mat,
+                evals_count=evals_count,
+                **(
+                    {}
+                    if self.evals_method_options is None
+                    else self.evals_method_options
+                ),
+            )
+        return evals
 
     def eigensys(
         self,
         evals_count: int = 6,
         bare_esys: Optional[Dict[int, Union[ndarray, List[ndarray]]]] = None,
     ) -> Tuple[ndarray, QutipEigenstates]:
-        """Calculates eigenvalues and eigenvectors of the full Hamiltonian using
-        `qutip.Qobj.eigenstates()`.
+        """Calculates eigenvalues and eigenvectors of the full Hamiltonian. Qutip's
+        `qutip.Qobj.eigenenergies()` is used by default, unless `self.evals_method`
+        has been set to something other than `None`.
 
         Parameters
         ----------
         evals_count:
             number of desired eigenvalues/eigenstates
         bare_esys:
             optionally, the bare eigensystems for each subsystem can be provided to
             speed up computation; these are provided in dict form via <subsys>: esys
 
         Returns
         -------
             eigenvalues and eigenvectors
         """
+
         hamiltonian_mat = self.hamiltonian(bare_esys=bare_esys)  # type:ignore
-        evals, evecs = hamiltonian_mat.eigenstates(eigvals=evals_count)
+
+        if not hasattr(self, "esys_method") or self.esys_method is None:
+            evals, evecs = hamiltonian_mat.eigenstates(eigvals=evals_count)
+        else:
+            diagonalizer = (
+                diag.DIAG_METHODS[self.esys_method]
+                if isinstance(self.esys_method, str)
+                else self.esys_method
+            )
+            evals, evecs = diagonalizer(
+                hamiltonian_mat,
+                evals_count=evals_count,
+                **(
+                    {} if self.esys_method_options is None else self.esys_method_options
+                ),
+            )
+
         evecs = evecs.view(scqubits.io_utils.fileio_qutip.QutipEigenstates)
+
         return evals, evecs
 
     def _esys_for_paramval(
         self,
         paramval: float,
         update_hilbertspace: Callable,
         evals_count: int,
@@ -879,15 +967,15 @@
                 eigensystem_mapdata = list(
                     target_map(
                         func,
                         tqdm(
                             param_vals,
                             desc="Spectral data",
                             leave=False,
-                            disable=(num_cpus > 1),
+                            disable=(num_cpus > 1) or settings.PROGRESSBAR_DISABLED,
                         ),
                     )
                 )
             eigenvalue_table, eigenstate_table = spec_utils.recast_esys_mapdata(
                 eigensystem_mapdata
             )
         else:
@@ -904,15 +992,15 @@
                     list(
                         target_map(
                             func,
                             tqdm(
                                 param_vals,
                                 desc="Spectral data",
                                 leave=False,
-                                disable=(num_cpus > 1),
+                                disable=(num_cpus > 1) or settings.PROGRESSBAR_DISABLED,
                             ),
                         )
                     )
                 )
             eigenstate_table = None  # type: ignore
 
         return storage.SpectrumData(
@@ -927,15 +1015,19 @@
         """
         Standardize the phases of the (dressed) eigenvectors.
         """
         for idx, evec in enumerate(self._data["evecs"][0]):
             phase = spec_utils.extract_phase(evec.data.toarray())
             self._data["evecs"][0][idx] = evec * np.exp(-1j * phase)
 
-    def op_in_dressed_eigenbasis(self, **kwargs) -> Qobj:
+    def op_in_dressed_eigenbasis(
+        self,
+        op: Union[Tuple[Union[np.ndarray, csc_matrix], QuantumSys], Callable],
+        **kwargs,
+    ) -> Qobj:
         """
         Express a subsystem operator in the dressed eigenbasis of the full system
         (as opposed to both the "native basis" or "bare eigenbasis" of the subsystem).
         `op_in_dressed_eigenbasis(...)` offers two different interfaces:
 
         1. subsystem operators may be expressed as Callables
 
@@ -947,43 +1039,58 @@
            corresponding subsystem. In this case the user must additionally
            specify if the operator is in the native, subsystem-internal
            basis or the subsystem bare eigenbasis::
 
                 .op_in_dressed_eigenbasis(op=(<ndarray>, <subsys>),
                                           op_in_bare_eigenbasis=<Bool>)
         """
-        op_callable_or_tuple = kwargs.pop("op")
-        if isinstance(op_callable_or_tuple, Callable):
-            subsys_index, op = self._parse_op(op_callable_or_tuple)
-            return self._op_in_dressed_eigenbasis(
-                op, subsys_index, op_in_bare_eigenbasis=False
-            )
-        else:
-            op, subsys = op_callable_or_tuple
+        if isinstance(op, tuple):
+            op_matrix, subsys = op
             op_in_bare_eigenbasis = kwargs.pop("op_in_bare_eigenbasis", False)
             subsys_index = self.get_subsys_index(subsys)
-            return self._op_in_dressed_eigenbasis(
-                op, subsys_index, op_in_bare_eigenbasis
+            return self._op_matrix_to_dressed_eigenbasis(
+                op_matrix, subsys_index, op_in_bare_eigenbasis
             )
 
-    def _op_in_dressed_eigenbasis(
-        self, op: ndarray, subsys_index: int, op_in_bare_eigenbasis: bool = False
+        assert callable(op)
+        subsys_index = self.get_subsys_index(op.__self__)
+        return self._op_callable_to_dressed_eigenbasis(op, subsys_index)
+
+    def _op_matrix_to_dressed_eigenbasis(
+        self,
+        op: Union[np.ndarray, csc_matrix],
+        subsys_index: int,
+        op_in_bare_eigenbasis,
     ) -> Qobj:
         bare_evecs = self._data["bare_evecs"][subsys_index][0]
         id_wrapped_op = spec_utils.identity_wrap(
             op,
             self.subsystem_list[subsys_index],
             self.subsystem_list,
             op_in_eigenbasis=op_in_bare_eigenbasis,
             evecs=bare_evecs,
         )
         dressed_evecs = self._data["evecs"][0]
         dressed_op = id_wrapped_op.transform(dressed_evecs)
         return dressed_op
 
+    def _op_callable_to_dressed_eigenbasis(
+        self, op: Callable, subsys_index: int
+    ) -> Qobj:
+        bare_evecs = self._data["bare_evecs"][subsys_index][0]
+        id_wrapped_op = spec_utils.identity_wrap(
+            op,
+            self.subsystem_list[subsys_index],
+            self.subsystem_list,
+            evecs=bare_evecs,
+        )
+        dressed_evecs = self._data["evecs"][0]
+        dressed_op = id_wrapped_op.transform(dressed_evecs)
+        return dressed_op
+
     ###################################################################################
     # HilbertSpace: add interaction and parsing arguments to .add_interaction
     ###################################################################################
     def add_interaction(
         self, check_validity=True, id_str: Optional[str] = None, **kwargs
     ) -> None:
         """
@@ -1024,14 +1131,19 @@
                                      op2=(<str>, <Callable>),
                                      …)
         3. General Qobj operator
             Specify a fully identity-wrapped `qutip.Qobj` operator. Signature::
 
                 .add_interaction(qobj=<Qobj>)
 
+        Parameters
+        ----------
+        check_validity:
+            optional bool indicating whether to check the validity of the interaction;
+            switch this off for speed if you are sure the interaction is valid
         id_str:
             optional string by which this instance can be referred to in `HilbertSpace`
             and `ParameterSweep`. If not provided, an id is auto-generated.
         """
         if "expr" in kwargs:
             interaction: Union[
                 InteractionTerm, InteractionTermStr
@@ -1052,73 +1164,84 @@
         id_str = id_str or "Interaction_{}".format(len(self.interaction_list))
         self._interaction_term_by_id_str[id_str] = interaction
 
         if not check_validity:
             return None
         try:
             _ = self.interaction_hamiltonian()
-        except:
+        except Exception as inst:
             self.interaction_list.pop()
             del self._interaction_term_by_id_str[id_str]
-            raise ValueError("Invalid Interaction Term")
+            raise ValueError(f"Invalid Interaction Term. Exception: {inst}")
 
     def _parse_interactiontermstr(self, **kwargs) -> InteractionTermStr:
         expr = kwargs.pop("expr")
         add_hc = kwargs.pop("add_hc", False)
         const = kwargs.pop("const", None)
 
         operator_list = []
         for key in kwargs.keys():
             if re.match(r"op\d+$", key) is None:
                 raise TypeError("Unexpected keyword argument {}.".format(key))
-            operator_list.append(self._parse_op_by_name(kwargs[key]))
+            operator_list.append(self._parse_str_based_op(kwargs[key]))
 
         return InteractionTermStr(expr, operator_list, const=const, add_hc=add_hc)
 
     def _parse_interactionterm(self, **kwargs) -> InteractionTerm:
         g = kwargs.pop("g", None)
         if g is None:
             g = kwargs.pop("g_strength")
         add_hc = kwargs.pop("add_hc", False)
 
         operator_list = []
         for key in kwargs.keys():
             if re.match(r"op\d+$", key) is None:
                 raise TypeError("Unexpected keyword argument {}.".format(key))
-            subsys_index, op = self._parse_op(kwargs[key])
+            subsys_index, op = self._parse_non_strbased_op(kwargs[key])
             operator_list.append((subsys_index, op))
 
         return InteractionTerm(g, operator_list, add_hc=add_hc)
 
     @staticmethod
     def _parse_qobj(**kwargs) -> Qobj:
         op = kwargs["qobj"]
         if len(kwargs) > 1 or not isinstance(op, Qobj):
             raise TypeError("Cannot interpret specified operator {}".format(op))
         return kwargs["qobj"]
 
-    def _parse_op_by_name(
-        self, op_by_name
-    ) -> Tuple[int, str, Union[ndarray, csc_matrix, dia_matrix]]:
-        if not isinstance(op_by_name, tuple):
-            raise TypeError("Cannot interpret specified operator {}".format(op_by_name))
-        if len(op_by_name) == 3:
+    def _parse_str_based_op(
+        self,
+        keyword_value: Union[Tuple[str, ndarray, QuantumSys], Tuple[str, Callable]],
+    ) -> Tuple[int, str, Union[ndarray, csc_matrix, dia_matrix, Callable]]:
+        if not isinstance(keyword_value, tuple):
+            raise TypeError(
+                "Cannot interpret specified operator {}".format(keyword_value)
+            )
+        if len(keyword_value) == 3:
             # format expected:  (<op name as str>, <op as array>, <subsys as QuantumSystem>)
-            return self.get_subsys_index(op_by_name[2]), op_by_name[0], op_by_name[1]
+            return (
+                self.get_subsys_index(keyword_value[2]),
+                keyword_value[0],
+                keyword_value[1],
+            )
         # format expected (<op name as str)>, <QuantumSystem.method callable>)
         return (
-            self.get_subsys_index(op_by_name[1].__self__),
-            op_by_name[0],
-            op_by_name[1](),
+            self.get_subsys_index(keyword_value[1].__self__),
+            keyword_value[0],
+            keyword_value[1],
         )
 
-    def _parse_op(
-        self, op: Union[Callable, Tuple[Union[ndarray, csc_matrix], QuantumSys]]
-    ) -> Tuple[int, Union[ndarray, csc_matrix]]:
+    def _parse_non_strbased_op(
+        self,
+        op: Union[Callable, Tuple[Union[ndarray, csc_matrix], QuantumSys]],
+    ) -> Tuple[int, Union[ndarray, csc_matrix, Callable]]:
         if callable(op):
-            return self.get_subsys_index(op.__self__), op()  # type:ignore
+            return (
+                self.get_subsys_index(op.__self__),
+                op,
+            )  # store op here, not op() [v3.2]
         if not isinstance(op, tuple):
             raise TypeError("Cannot interpret specified operator {}".format(op))
         if len(op) == 2:
             # format expected:  (<op as array>, <subsys as QuantumSystem>)
             return self.get_subsys_index(op[1]), op[0]
         raise TypeError("Cannot interpret specified operator {}".format(op))
```

### Comparing `scqubits-3.1.1/scqubits/core/namedslots_array.py` & `scqubits-3.2.0/scqubits/core/namedslots_array.py`

 * *Files identical despite different names*

### Comparing `scqubits-3.1.1/scqubits/core/noise.py` & `scqubits-3.2.0/scqubits/core/noise.py`

 * *Files 0% similar despite different names*

```diff
@@ -12,16 +12,16 @@
 
 import math
 import warnings
 
 from abc import ABC, abstractmethod
 from typing import Any, Callable, Dict, List, Optional, Tuple, Union, cast
 
-import matplotlib.pyplot as plt
 import matplotlib as mpl
+import matplotlib.pyplot as plt
 import numpy as np
 import scipy as sp
 
 from matplotlib.axes import Axes
 from matplotlib.figure import Figure
 from matplotlib.offsetbox import AnchoredText
 from numpy import ndarray
@@ -30,15 +30,14 @@
 import scqubits.core.units as units
 import scqubits.settings as settings
 import scqubits.utils.plotting as plotting
 
 from scqubits.core.storage import SpectrumData
 from scqubits.settings import matplotlib_settings
 
-
 # flag that lets us show a warning about the default t1 behavior
 # (i.e., total=True setting) only once. Using the standard warnings
 # filtering does not seem to work in jupyter.
 _t1_default_warning_given_flag = False
 
 
 def calc_therm_ratio(
@@ -220,15 +219,15 @@
 
         # figure out how large the figure should be, based on how many plots we have.
         # We currently assume 2 plots per row
         figsize = kwargs.get(
             "figsize", (4, 3) if plot_grid == (1, 1) else (8, 3 * plot_grid[0])
         )
 
-        # If axes was given in fig_as, it should support the plot structure
+        # If axes was given in fig_ax, it should support the plot structure
         # consistent with plot_grid, otherwise the plotting routine below, will fail
         fig, axes = kwargs.get("fig_ax") or plt.subplots(*plot_grid, figsize=figsize)
 
         plotting_options = {
             "xlabel": param_name,
             "yscale": "log",
             "grid": True,
```

### Comparing `scqubits-3.1.1/scqubits/core/operators.py` & `scqubits-3.2.0/scqubits/core/operators.py`

 * *Files 3% similar despite different names*

```diff
@@ -6,21 +6,21 @@
 #    Copyright (c) 2019 and later, Jens Koch and Peter Groszkowski
 #    All rights reserved.
 #
 #    This source code is licensed under the BSD-style license found in the
 #    LICENSE file in the root directory of this source tree.
 ############################################################################
 
-from typing import Union
+from typing import Optional, Union
 
 import numpy as np
 import scipy as sp
 
 from numpy import ndarray
-from scipy.sparse import csc_matrix, dia_matrix
+from scipy.sparse import csc_matrix
 
 
 def annihilation(dimension: int) -> ndarray:
     """
     Returns a dense matrix of size dimension x dimension representing the annihilation
     operator in number basis.
     """
@@ -68,15 +68,17 @@
         sparse number operator matrix, size dimension x dimension
     """
     hubbardmat = sp.sparse.dok_matrix((dimension, dimension), dtype=np.float_)
     hubbardmat[j1, j2] = 1.0
     return hubbardmat.asformat("csc")
 
 
-def number(dimension: int, prefactor: Union[float, complex] = None) -> ndarray:
+def number(
+    dimension: int, prefactor: Optional[Union[float, complex]] = None
+) -> ndarray:
     """Number operator matrix of size dimension x dimension in sparse matrix
     representation. An additional prefactor can be directly included in the
     generation of the matrix by supplying 'prefactor'.
 
     Parameters
     ----------
     dimension:
@@ -92,15 +94,15 @@
     diag_elements = np.arange(dimension, dtype=np.float_)
     if prefactor:
         diag_elements *= prefactor
     return np.diagflat(diag_elements)
 
 
 def number_sparse(
-    dimension: int, prefactor: Union[float, complex] = None
+    dimension: int, prefactor: Optional[Union[float, complex]] = None
 ) -> csc_matrix:
     """Number operator matrix of size dimension x dimension in sparse matrix
     representation. An additional prefactor can be directly included in the
     generation of the matrix by supplying 'prefactor'.
 
     Parameters
     ----------
```

### Comparing `scqubits-3.1.1/scqubits/core/oscillator.py` & `scqubits-3.2.0/scqubits/core/oscillator.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,14 @@
 #    All rights reserved.
 #
 #    This source code is licensed under the BSD-style license found in the
 #    LICENSE file in the root directory of this source tree.
 ############################################################################
 
 import os
-
 from typing import Any, Dict, Optional, Tuple, Union
 
 import numpy as np
 import scipy as sp
 
 from numpy import ndarray
 from scipy.special import factorial, pbdv
@@ -144,15 +143,15 @@
         return self.truncated_dim
 
     def creation_operator(self) -> ndarray:
         """Returns the creation operator"""
         return op.creation(self.truncated_dim)
 
     def annihilation_operator(self) -> ndarray:
-        """Returns the creation operator"""
+        """Returns the annihilation operator"""
         return op.annihilation(self.truncated_dim)
 
     def matrixelement_table(self, *args, **kwargs) -> ndarray:
         raise NotImplementedError(
             "The Oscillator class does not implement the matrixelement_table method."
         )
 
@@ -161,30 +160,30 @@
         :math:`l_\text{osc} (a + a^{\dagger})/\sqrt{2}`, with :math:`a` representing
         an annihilation operator, and :math:`l_\text{osc}` the oscillator length.
         """
         if self.l_osc is None:
             raise ValueError(
                 "Variable l_osc has to be set to something other than None\n"
                 + "in order to use the phi_operator() method. This can be done by either\n"
-                + "passing it to the class constructor, or by setting it afterwords."
+                + "passing it to the class constructor, or by setting it afterwards."
             )
         a = op.annihilation(self.truncated_dim)
         return self.l_osc / np.sqrt(2) * (a + a.T)
 
     def n_operator(self) -> ndarray:
         r"""Returns the charge-number n operator defined as
         :math:`i (a^{\dagger} - a)/ ( \sqrt{2} l_\text{osc})`, with :math:`a` representing
         an annihilation operator, and :math:`l_\text{osc}` the oscillator length.
         """
 
         if self.l_osc is None:
             raise ValueError(
                 "Variable l_osc has to be set to something other than None\n"
                 + "in order to use the n_operator() method. This can be done by either\n"
-                + "passing it to the class constructor, or by setting it afterwords."
+                + "passing it to the class constructor, or by setting it afterwards."
             )
         a = op.annihilation(self.truncated_dim)
         return 1.0j / (self.l_osc * np.sqrt(2)) * (a.T - a)
 
 
 # -KerrOscillator class-------------------------------------------------------------------
 
@@ -224,15 +223,15 @@
             E_osc=E_osc,
             l_osc=l_osc,
             truncated_dim=truncated_dim,
             id_str=id_str,
         )
 
         self._image_filename = os.path.join(
-            os.path.dirname(os.path.abspath(__file__)), "qubit_img/kerr-oscillator.jpg"
+            os.path.dirname(os.path.abspath(__file__)), "qubit_img/KerrOscillator.jpg"
         )
 
     @staticmethod
     def default_params() -> Dict[str, Any]:
         return {
             "E_osc": 5.0,
             "K": 0.05,
```

### Comparing `scqubits-3.1.1/scqubits/core/param_sweep.py` & `scqubits-3.2.0/scqubits/core/param_sweep.py`

 * *Files 1% similar despite different names*

```diff
@@ -27,29 +27,28 @@
     Optional,
     Tuple,
     Union,
     overload,
 )
 
 import numpy as np
-
 from matplotlib.axes import Axes
 from matplotlib.figure import Figure
 from numpy import ndarray
 from qutip import Qobj
+from scipy.sparse import csc_matrix
 from typing_extensions import Literal
 
 import scqubits.core.central_dispatch as dispatch
 import scqubits.core.descriptors as descriptors
 import scqubits.core.sweeps as sweeps
 import scqubits.io_utils.fileio_serializers as serializers
 import scqubits.utils.cpu_switch as cpu_switch
 import scqubits.utils.misc as utils
 import scqubits.utils.plotting as plot
-
 from scqubits import settings as settings
 from scqubits.core.hilbert_space import HilbertSpace
 from scqubits.core.namedslots_array import (
     NamedSlotsNdarray,
     Parameters,
     convert_to_std_npindex,
 )
@@ -62,21 +61,24 @@
     from scqubits.io_utils.fileio import IOData
 
 if settings.IN_IPYTHON:
     from tqdm.notebook import tqdm
 else:
     from tqdm import tqdm
 
-from scqubits.utils.typedefs import GIndexTuple, NpIndices, QubitList
+from scqubits.utils.typedefs import GIndexTuple, NpIndices
 
 BareLabel = Tuple[int, ...]
 DressedLabel = int
 StateLabel = Union[DressedLabel, BareLabel]
 
 
+_faulty_interactionterm_warning_issued = False  # flag to ensure single-time warning
+
+
 class ParameterSlice:
     """
     Stores information about a 1d slice of a (possibly) multi-dimensional parameter
     sweep.
 
     Parameters
     ----------
@@ -118,14 +120,15 @@
     _lookup_exists = False
     _parameters = descriptors.WatchedProperty(Parameters, "PARAMETERSWEEP_UPDATE")
     _evals_count = descriptors.WatchedProperty(int, "PARAMETERSWEEP_UPDATE")
     _data = descriptors.WatchedProperty(Dict[str, ndarray], "PARAMETERSWEEP_UPDATE")
     _hilbertspace: HilbertSpace
 
     _out_of_sync = False
+    _out_of_sync_warning_issued = False
     _current_param_indices: NpIndices
 
     @property
     def hilbertspace(self) -> HilbertSpace:
         return self._hilbertspace
 
     @property
@@ -368,15 +371,15 @@
             state_full[subsys_index] = entry
         return tuple(state_full)
 
     def _process_subsystems_option(
         self, subsystems: Optional[Union[QuantumSystem, List[QuantumSystem]]]
     ) -> List[QuantumSystem]:
         if subsystems is None:
-            return self.hilbertspace.subsys_list
+            return self.hilbertspace.subsystem_list
         if isinstance(subsystems, list):
             return subsystems
         if isinstance(subsystems, QuantumSystem):
             return [subsystems]
         raise TypeError("Argument `subsystems` has invalid type.")
 
     def _process_initial_option(
@@ -949,25 +952,47 @@
         self._update_hilbertspace = self.set_update_func(update_hilbertspace)
         self._subsys_update_info = subsys_update_info
         self._data: Dict[str, Any] = {}
         self._bare_only = bare_only
         self._ignore_low_overlap = ignore_low_overlap
         self._deepcopy = deepcopy
         self._num_cpus = num_cpus
-        self.tqdm_disabled = settings.PROGRESSBAR_DISABLED or (num_cpus > 1)
 
         self._out_of_sync = False
         self.reset_preslicing()
 
         dispatch.CENTRAL_DISPATCH.register("PARAMETERSWEEP_UPDATE", self)
         dispatch.CENTRAL_DISPATCH.register("HILBERTSPACE_UPDATE", self)
 
+        global _faulty_interactionterm_warning_issued
+        if self.faulty_interactionterm_suspected() and not _faulty_interactionterm_warning_issued:
+            warnings.warn(
+                "The interactions specified for this HilbertSpace object involve coupling operators stored as fixed "
+                "matrices. This may be unintended, as the operators of quantum systems (specifically, their "
+                "representation with respect to some basis) may change as a function of sweep parameters. \nFor that "
+                "reason, it is recommended to use coupling operators specified as callable functions.\n",
+                UserWarning,
+            )
+            _faulty_interactionterm_warning_issued = True
+
         if autorun:
             self.run()
 
+    @property
+    def tqdm_disabled(self) -> bool:
+        return settings.PROGRESSBAR_DISABLED or (self._num_cpus > 1)
+
+    def faulty_interactionterm_suspected(self) -> bool:
+        """Check if any interaction terms are specified as fixed matrices"""
+        for interactionterm in self._hilbertspace.interaction_list:
+            for idx_operator in interactionterm.operator_list:
+                if isinstance(idx_operator[1], (ndarray, Qobj, csc_matrix)):
+                    return True
+        return False
+
     def cause_dispatch(self) -> None:
         initial_parameters = tuple(paramvals[0] for paramvals in self._parameters)
         self._update_hilbertspace(self, *initial_parameters)
 
     @classmethod
     def deserialize(cls, iodata: "IOData") -> "StoredSweep":
         pass
@@ -990,14 +1015,16 @@
         iodata.typename = "StoredSweep"
         return iodata
 
     def run(self) -> None:
         """Create all sweep data: bare spectral data, dressed spectral data, lookup
         data and custom sweep data."""
         # generate one dispatch before temporarily disabling CENTRAL_DISPATCH
+        self._out_of_sync = False
+        self._out_of_sync_warning_issued = False
 
         self._lookup_exists = True
         if self._deepcopy:
             stored_hilbertspace = copy.deepcopy(self.hilbertspace)
             self._hilbertspace = copy.deepcopy(self.hilbertspace)
         else:
             self.cause_dispatch()
@@ -1086,15 +1113,14 @@
             multidimensional array of the format
             array[p1, p2, p3, ..., pN] = np.asarray[[evals, evecs]]
         """
         fixed_paramnames = self._paramnames_no_subsys_update(subsystem)
         reduced_parameters = self._parameters.create_reduced(fixed_paramnames)
         total_count = np.prod([len(param_vals) for param_vals in reduced_parameters])
 
-        multi_cpu = self._num_cpus > 1
         target_map = cpu_switch.get_map_method(self._num_cpus)
 
         with utils.InfoBar(
             "Parallel compute bare eigensys for subsystem {} [num_cpus={}]".format(
                 subsystem.id_str, self._num_cpus
             ),
             self._num_cpus,
@@ -1107,15 +1133,15 @@
                         subsystem,
                     ),
                     itertools.product(*reduced_parameters.paramvals_list),
                 ),
                 total=total_count,
                 desc="Bare spectra",
                 leave=False,
-                disable=multi_cpu,
+                disable=self.tqdm_disabled,
             )
 
         bare_eigendata = np.asarray(list(bare_eigendata), dtype=object)
         bare_eigendata = bare_eigendata.reshape((*reduced_parameters.counts, 2))
 
         # Bare spectral data was only computed once for each parameter that has no
         # update effect on the subsystems. Now extend the array to reflect this
@@ -1160,15 +1186,14 @@
         """
 
         Returns
         -------
             NamedSlotsNdarray[<paramname1>, <paramname2>, ...] of eigenvalues,
             likewise for eigenvectors
         """
-        multi_cpu = self._num_cpus > 1
         target_map = cpu_switch.get_map_method(self._num_cpus)
         total_count = np.prod(self._parameters.counts)
 
         with utils.InfoBar(
             "Parallel compute dressed eigensys [num_cpus={}]".format(self._num_cpus),
             self._num_cpus,
         ) as p:
@@ -1182,15 +1207,15 @@
                             self._update_hilbertspace,
                         ),
                         itertools.product(*self._parameters.ranges),
                     ),
                     total=total_count,
                     desc="Dressed spectrum",
                     leave=False,
-                    disable=multi_cpu,
+                    disable=self.tqdm_disabled,
                 )
             )
 
         spectrum_data_ndarray = np.asarray(spectrum_data, dtype=object)
         spectrum_data_ndarray = spectrum_data_ndarray.reshape(
             (*self._parameters.counts, 2)
         )
```

### Comparing `scqubits-3.1.1/scqubits/core/qubit_base.py` & `scqubits-3.2.0/scqubits/core/qubit_base.py`

 * *Files 3% similar despite different names*

```diff
@@ -11,40 +11,42 @@
 ############################################################################
 """
 Provides the base classes for qubits
 """
 
 import functools
 import inspect
+import os
 
 from abc import ABC, ABCMeta, abstractmethod
 from typing import (
     TYPE_CHECKING,
     Any,
     Dict,
     Iterable,
     List,
     Optional,
     Tuple,
     Union,
     overload,
 )
 
-import matplotlib.pyplot as plt
 import matplotlib as mpl
+import matplotlib.pyplot as plt
 import numpy as np
 import scipy as sp
 
 from matplotlib.axes import Axes
 from matplotlib.figure import Figure
 from numpy import ndarray
 from scipy.sparse import csc_matrix, dia_matrix
 
 import scqubits.core.constants as constants
 import scqubits.core.descriptors as descriptors
+import scqubits.core.diag as diag
 import scqubits.core.units as units
 import scqubits.settings as settings
 import scqubits.ui.qubit_widget as ui
 import scqubits.utils.plotting as plot
 
 from scqubits.core.central_dispatch import DispatchClient
 from scqubits.core.discretization import Grid1d
@@ -113,14 +115,19 @@
             QuantumSystem._quantumsystem_counter -= 1
         except (NameError, AttributeError):
             pass
 
     def __init__(self, id_str: Union[str, None]):
         self._sys_type = type(self).__name__
         self._id_str = id_str or self._autogenerate_id_str()
+        self._image_filename = os.path.join(
+            os.path.dirname(os.path.abspath(__file__)),
+            "qubit_img",
+            type(self).__name__ + ".jpg",
+        )
 
     def __init_subclass__(cls):
         """Used to register all non-abstract _subclasses as a list in
         `QuantumSystem._subclasses`."""
         super().__init_subclass__()
         if not inspect.isabstract(cls):
             cls._subclasses.append(cls)
@@ -164,15 +171,26 @@
     @property
     def id_str(self):
         return self._id_str
 
     def get_initdata(self) -> Dict[str, Any]:
         """Returns dict appropriate for creating/initializing a new Serializable
         object."""
-        return {name: getattr(self, name) for name in self._init_params}
+        EXCLUDE = [
+            "evals_method",
+            "evals_method_options",
+            "esys_method",
+            "esys_method_options",
+        ]
+        initdata = {
+            name: getattr(self, name)
+            for name in self._init_params
+            if name not in EXCLUDE
+        }
+        return initdata
 
     @abstractmethod
     def hilbertdim(self) -> int:
         """Returns dimension of Hilbert space"""
 
     @classmethod
     def get_operator_names(cls) -> List[str]:
@@ -198,28 +216,36 @@
     def create(cls) -> "QuantumSystem":
         """Use ipywidgets to create a new class instance"""
         init_params = cls.default_params()
         instance = cls(**init_params)
         instance.widget()
         return instance
 
-    def widget(self, params: Dict[str, Any] = None):
+    def widget(self, params: Optional[Dict[str, Any]] = None):
         """Use ipywidgets to modify parameters of class instance"""
         init_params = params or self.get_initdata()
         init_params.pop("id_str", None)
         ui.create_widget(
-            self.set_params, init_params, image_filename=self._image_filename
+            self.set_params_from_gui, init_params, image_filename=self._image_filename
         )
 
     @staticmethod
     @abstractmethod
     def default_params() -> Dict[str, Any]:
         """Return dictionary with default parameter values for initialization of
         class instance"""
 
+    def set_params_from_gui(self, change):
+        """
+        Set new parameters through the provided dictionary.
+        """
+        param_name = change["owner"].name
+        param_val = change["owner"].num_value
+        setattr(self, param_name, param_val)
+
     def set_params(self, **kwargs):
         """
         Set new parameters through the provided dictionary.
         """
         for param_name, param_val in kwargs.items():
             setattr(self, param_name, param_val)
 
@@ -241,38 +267,58 @@
 
     # see PEP 526 https://www.python.org/dev/peps/pep-0526/#class-and-instance-variable-annotations
     truncated_dim: int  # type:ignore
     _default_grid: Grid1d
     _sys_type: str
     _init_params: list
 
+    def __init__(
+        self,
+        id_str: Union[str, None],
+        evals_method: Union[str, None] = None,
+        evals_method_options: Union[Dict, None] = None,
+        esys_method: Union[str, None] = None,
+        esys_method_options: Union[Dict, None] = None,
+    ):
+        super().__init__(id_str=id_str)
+        self.evals_method = evals_method
+        self.evals_method_options = evals_method_options
+        self.esys_method = esys_method
+        self.esys_method_options = esys_method_options
+
     @abstractmethod
     def hamiltonian(self):
         """Returns the Hamiltonian"""
 
     def _evals_calc(self, evals_count: int) -> ndarray:
         hamiltonian_mat = self.hamiltonian()
         evals = sp.linalg.eigh(
-            hamiltonian_mat, eigvals_only=True, subset_by_index=(0, evals_count - 1)
+            hamiltonian_mat,
+            eigvals_only=True,
+            subset_by_index=(0, evals_count - 1),
+            check_finite=False,
         )
         return np.sort(evals)
 
     def _esys_calc(self, evals_count: int) -> Tuple[ndarray, ndarray]:
         hamiltonian_mat = self.hamiltonian()
         evals, evecs = sp.linalg.eigh(
-            hamiltonian_mat, eigvals_only=False, subset_by_index=(0, evals_count - 1)
+            hamiltonian_mat,
+            eigvals_only=False,
+            subset_by_index=(0, evals_count - 1),
+            check_finite=False,
         )
         evals, evecs = order_eigensystem(evals, evecs)
         return evals, evecs
 
     @overload
     def eigenvals(
         self,
         evals_count: int = 6,
-        filename: str = None,
+        filename: Optional[str] = None,
         return_spectrumdata: "Literal[False]" = False,
     ) -> ndarray:
         ...
 
     @overload
     def eigenvals(
         self,
@@ -281,15 +327,15 @@
         return_spectrumdata: "Literal[True]",
     ) -> SpectrumData:
         ...
 
     def eigenvals(
         self,
         evals_count: int = 6,
-        filename: str = None,
+        filename: Optional[str] = None,
         return_spectrumdata: bool = False,
     ) -> Union[SpectrumData, ndarray]:
         """Calculates eigenvalues using `scipy.linalg.eigh`, returns numpy array of
         eigenvalues.
 
         Parameters
         ----------
@@ -302,28 +348,40 @@
             if set to true, the returned data is provided as a SpectrumData object
             (default value = False)
 
         Returns
         -------
             eigenvalues as ndarray or in form of a SpectrumData object
         """
-        evals = self._evals_calc(evals_count)
+        if not hasattr(self, "evals_method") or self.evals_method is None:
+            evals = self._evals_calc(evals_count)
+        else:
+            diagonalizer = (
+                diag.DIAG_METHODS[self.evals_method]
+                if isinstance(self.evals_method, str)
+                else self.evals_method
+            )
+            options = (
+                {} if self.esys_method_options is None else self.esys_method_options
+            )
+            evals = diagonalizer(self.hamiltonian(), evals_count, **options)
+
         if filename or return_spectrumdata:
             specdata = SpectrumData(
                 energy_table=evals, system_params=self.get_initdata()
             )
         if filename:
             specdata.filewrite(filename)
         return specdata if return_spectrumdata else evals
 
     @overload
     def eigensys(
         self,
         evals_count: int = 6,
-        filename: str = None,
+        filename: Optional[str] = None,
         return_spectrumdata: "Literal[False]" = False,
     ) -> Tuple[ndarray, ndarray]:
         ...
 
     @overload
     def eigensys(
         self,
@@ -332,37 +390,48 @@
         return_spectrumdata: "Literal[True]",
     ) -> SpectrumData:
         ...
 
     def eigensys(
         self,
         evals_count: int = 6,
-        filename: str = None,
+        filename: Optional[str] = None,
         return_spectrumdata: bool = False,
     ) -> Union[Tuple[ndarray, ndarray], SpectrumData]:
         """Calculates eigenvalues and corresponding eigenvectors using
         `scipy.linalg.eigh`. Returns two numpy arrays containing the eigenvalues and
         eigenvectors, respectively.
 
         Parameters
         ----------
         evals_count:
             number of desired eigenvalues/eigenstates (default value = 6)
         filename:
             path and filename without suffix, if file output desired
             (default value = None)
-        return_spectrumdata:
-            if set to true, the returned data is provided as a SpectrumData object
+        return_spectrumdata: if set to true, the returned data is provided as a SpectrumData object
             (default value = False)
 
         Returns
         -------
             eigenvalues, eigenvectors as numpy arrays or in form of a SpectrumData object
         """
-        evals, evecs = self._esys_calc(evals_count)
+        if not hasattr(self, "esys_method") or self.esys_method is None:
+            evals, evecs = self._esys_calc(evals_count)
+        else:
+            diagonalizer = (
+                diag.DIAG_METHODS[self.esys_method]
+                if isinstance(self.esys_method, str)
+                else self.esys_method
+            )
+            options = (
+                {} if self.esys_method_options is None else self.esys_method_options
+            )
+            evals, evecs = diagonalizer(self.hamiltonian(), evals_count, **options)
+
         if filename or return_spectrumdata:
             specdata = SpectrumData(
                 energy_table=evals, system_params=self.get_initdata(), state_table=evecs
             )
         if filename:
             specdata.filewrite(filename)
         return specdata if return_spectrumdata else (evals, evecs)
@@ -1127,15 +1196,15 @@
     @mpl.rc_context(matplotlib_settings)
     def plot_wavefunction(
         self,
         which: Union[int, Iterable[int]] = 0,
         mode: str = "real",
         esys: Tuple[ndarray, ndarray] = None,
         phi_grid: Grid1d = None,
-        scaling: float = None,
+        scaling: Optional[float] = None,
         **kwargs,
     ) -> Tuple[Figure, Axes]:
         """Plot 1d phase-basis wave function(s). Must be overwritten by
         higher-dimensional qubits like FluxQubits and ZeroPi.
 
         Parameters
         ----------
```

### Comparing `scqubits-3.1.1/scqubits/core/spec_lookup.py` & `scqubits-3.2.0/scqubits/core/spec_lookup.py`

 * *Files 8% similar despite different names*

```diff
@@ -116,26 +116,40 @@
     def _generate_single_mapping(
         self,
         param_indices: Tuple[int, ...],
     ) -> ndarray:
         """
         For a single set of parameter values, specified by a tuple of indices
         ``param_indices``, create an array of the dressed-state indices in an order
-        that corresponds one to one to the bare product states with largest overlap
+        that corresponds one-to-one to the bare product states with largest overlap
         (whenever possible).
 
         Parameters
         ----------
         param_indices:
             indices of the parameter values
+            Length of tuple must match the number of parameters in the `ParameterSweep` object inheriting from
+            `SpectrumLookupMixin`.
 
         Returns
         -------
-            dressed-state indices
+            1d array of dressed-state indices
+            Dimensions: (`self.hilbertspace.dimension`,)
+
+            Array which contains the dressed-state indices in an order that corresponds to the canonically ordered bare
+            product state basis, i.e. (0,0,0), (0,0,1), (0,0,2), ..., (0,1,0), (0,1,1), (0,1,2), ... etc.
+            For example, for two subsystems with two states each, the array [0, 2, 1, 3] would mean:
+            (0,0) corresponds to the dressed state 0,
+            (0,1) corresponds to the dressed state 2,
+            (1,0) corresponds to the dressed state 1,
+            (1,1) corresponds to the dressed state 3.
         """
+        # Overlaps between dressed energy eigenstates and bare product states, <e1, e2, ...| E_j>
+        # Since the Hamiltonian matrix is explicitly constructed in the bare product states basis, this is just the same
+        # as the matrix of eigenvectors handed back when diagonalizing the Hamiltonian matrix.
         overlap_matrix = spec_utils.convert_evecs_to_ndarray(
             self._data["evecs"][param_indices]
         )
 
         dim = self.hilbertspace.dimension
         dressed_indices: List[Union[int, None]] = [None] * dim
         for dressed_index in range(self._evals_count):
@@ -148,46 +162,54 @@
                 dressed_indices[int(max_position)] = dressed_index
 
         return np.asarray(dressed_indices)
 
     def set_npindextuple(
         self, param_indices: Optional[NpIndices] = None
     ) -> NpIndexTuple:
+        """
+        Convert the NpIndices parameter indices to a tuple of NpIndices.
+        """
         param_indices = param_indices or self._current_param_indices
         if not isinstance(param_indices, tuple):
             param_indices = (param_indices,)
         return param_indices
 
     @utils.check_lookup_exists
     @utils.check_sync_status
     def dressed_index(
         self,
         bare_labels: Tuple[int, ...],
-        param_indices: Optional[NpIndices] = None,
+        param_npindices: Optional[NpIndices] = None,
     ) -> Union[ndarray, int, None]:
         """
         For given bare product state return the corresponding dressed-state index.
 
         Parameters
         ----------
         bare_labels:
             bare_labels = (index, index2, ...)
-        param_indices:
+            Dimension: (`self.hilbertspace.subsystem_count`,)
+        param_npindices:
             indices of parameter values of interest
+            Depending on the nature of the slice, this can be a single parameter point or multiple ones.
 
         Returns
         -------
-            dressed state index closest to the specified bare state
+            dressed state index closest to the specified bare state with excitation numbers given by `bare_labels`.
+            If `param_npindices` spans multiple parameter points, then this returns a corresponding 1d array of
+            length dictated by the number of parameter points.
         """
-        param_indices = self.set_npindextuple(param_indices)
+        param_npindices = self.set_npindextuple(param_npindices)
         try:
             lookup_position = self._bare_product_states_labels.index(bare_labels)
         except ValueError:
             return None
-        return self._data["dressed_indices"][param_indices + (lookup_position,)]
+
+        return self._data["dressed_indices"][param_npindices + (lookup_position,)]
 
     @utils.check_lookup_exists
     @utils.check_sync_status
     def bare_index(
         self,
         dressed_index: int,
         param_indices: Optional[Tuple[int, ...]] = None,
@@ -262,47 +284,47 @@
 
     @utils.check_lookup_exists
     @utils.check_sync_status
     def energy_by_bare_index(
         self,
         bare_tuple: Tuple[int, ...],
         subtract_ground: bool = False,
-        param_indices: Optional[NpIndices] = None,
+        param_npindices: Optional[NpIndices] = None,
     ) -> Union[float, NamedSlotsNdarray]:  # the return value may also be np.nan
         """
         Look up dressed energy most closely corresponding to the given bare-state labels
 
         Parameters
         ----------
         bare_tuple:
             bare state indices
         subtract_ground:
             whether to subtract the ground state energy
-        param_indices:
+        param_npindices:
             indices specifying the set of parameters
 
         Returns
         -------
             dressed energies, if lookup successful, otherwise nan;
         """
-        param_indices = self.set_npindextuple(param_indices)
-        dressed_index = self.dressed_index(bare_tuple, param_indices)
+        param_npindices = self.set_npindextuple(param_npindices)
+        dressed_index = self.dressed_index(bare_tuple, param_npindices)
 
         if dressed_index is None:
             return np.nan  # type:ignore
         if isinstance(dressed_index, numbers.Number):
-            energy = self["evals"][param_indices + (dressed_index,)]
+            energy = self["evals"][param_npindices + (dressed_index,)]
             if subtract_ground:
-                energy -= self["evals"][param_indices + (0,)]
+                energy -= self["evals"][param_npindices + (0,)]
             return energy
 
         dressed_index = np.asarray(dressed_index)
         energies = np.empty_like(dressed_index, dtype=np.float_)
         it = np.nditer(dressed_index, flags=["multi_index", "refs_ok"])
-        sliced_energies = self["evals"][param_indices]
+        sliced_energies = self["evals"][param_npindices]
 
         for location in it:
             location = location.tolist()
             if location is None:
                 energies[it.multi_index] = np.nan
             else:
                 energies[it.multi_index] = sliced_energies[it.multi_index][location]
```

### Comparing `scqubits-3.1.1/scqubits/core/storage.py` & `scqubits-3.2.0/scqubits/core/storage.py`

 * *Files 3% similar despite different names*

```diff
@@ -62,20 +62,37 @@
 
         Parameters
         ----------
         potential_vals:
             array of potential energy values (that determine the energy range on the y axis
 
         """
+        self.amplitudes *= self.amplitude_scale_factor(potential_vals)
+
+    def amplitude_scale_factor(self, potential_vals: np.ndarray) -> float:
+        """
+        Returnn scale factor that converts the dimensionless amplitude to a (pseudo-)energy that allows us to plot
+        wavefunctions and potential energies in the same plot.
+
+        Parameters
+        ----------
+        potential_vals:
+            array of potential energy values (that determine the energy range on the y axis
+
+        Returns
+        -------
+            scale factor
+
+        """
         FILL_FACTOR = 0.1
         energy_range = np.max(potential_vals) - np.min(potential_vals)
         amplitude_range = np.max(self.amplitudes) - np.min(self.amplitudes)
         if amplitude_range < 1.0e-10:
             return 0.0
-        self.amplitudes *= FILL_FACTOR * energy_range / amplitude_range
+        return FILL_FACTOR * energy_range / amplitude_range
 
 
 # -WaveFunctionOnGrid class-------------------------------------------------------------
 
 
 class WaveFunctionOnGrid:
     """Container for wave function amplitudes defined on a coordinate grid (arbitrary
```

### Comparing `scqubits-3.1.1/scqubits/core/sweeps.py` & `scqubits-3.2.0/scqubits/core/sweeps.py`

 * *Files identical despite different names*

### Comparing `scqubits-3.1.1/scqubits/core/symbolic_circuit.py` & `scqubits-3.2.0/scqubits/core/symbolic_circuit.py`

 * *Files 0% similar despite different names*

```diff
@@ -8,32 +8,33 @@
 #    This source code is licensed under the BSD-style license found in the
 #    LICENSE file in the root directory of this source tree.
 ############################################################################
 
 import copy
 import itertools
 import warnings
-
 from symtable import Symbol
 from typing import Any, Dict, List, Optional, Set, Tuple, Union
 
 import numpy as np
 import scipy as sp
-import scqubits.io_utils.fileio_serializers as serializers
-import scqubits.settings as settings
 import sympy
 import yaml
 
 from numpy import ndarray
-from scqubits.utils.misc import flatten_list, is_float_string
 from sympy import symbols
 
+import scqubits.io_utils.fileio_serializers as serializers
+import scqubits.settings as settings
+
+from scqubits.utils.misc import flatten_list, is_string_float
+
 
 def process_word(word: str) -> Union[float, symbols]:
-    if is_float_string(word):
+    if is_string_float(word):
         return float(word)
     return symbols(word)
 
 
 def parse_branch_parameters(
     words: List[str], branch_type: str
 ) -> Tuple[List[float], Dict[Symbol, float]]:
@@ -60,15 +61,15 @@
         An exception is raised if the proper syntax is not followed when using variables
         in the input file.
     """
     branch_var_dict: Dict[Symbol, float] = {}
     branch_params: List[float] = []
     num_params = 2 if branch_type in ["JJ", "JJ2"] else 1
     for word in words[0:num_params]:
-        if not is_float_string(word):
+        if not is_string_float(word):
             if len(word.split("=")) > 2:
                 raise Exception("Syntax error in branch specification.")
             if len(word.split("=")) == 2:
                 var_str, init_val = word.split("=")
                 params = [process_word(var_str), process_word(init_val)]
             elif len(word.split("=")) == 1:
                 params = [process_word(word)]
```

### Comparing `scqubits-3.1.1/scqubits/core/transmon.py` & `scqubits-3.2.0/scqubits/core/transmon.py`

 * *Files 6% similar despite different names*

```diff
@@ -7,15 +7,14 @@
 #    All rights reserved.
 #
 #    This source code is licensed under the BSD-style license found in the
 #    LICENSE file in the root directory of this source tree.
 ############################################################################
 
 import math
-import os
 
 from typing import Any, Dict, List, Optional, Tuple, Union
 
 import numpy as np
 import scipy as sp
 
 from matplotlib.axes import Axes
@@ -35,15 +34,15 @@
 from scqubits.core.noise import NoisySystem
 from scqubits.core.storage import WaveFunction
 
 LevelsTuple = Tuple[int, ...]
 Transition = Tuple[int, int]
 TransitionsTuple = Tuple[Transition, ...]
 
-# -Cooper pair box / transmon----------------------------------------------
+# Cooper pair box / transmon
 
 
 class Transmon(base.QubitBaseClass1d, serializers.Serializable, NoisySystem):
     r"""Class for the Cooper-pair-box and transmon qubit. The Hamiltonian is
     represented in dense form in the number basis,
     :math:`H_\text{CPB}=4E_\text{C}(\hat{n}-n_g)^2-\frac{E_\text{J}}{2}(
     |n\rangle\langle n+1|+\text{h.c.})`.
@@ -76,26 +75,34 @@
         self,
         EJ: float,
         EC: float,
         ng: float,
         ncut: int,
         truncated_dim: int = 6,
         id_str: Optional[str] = None,
+        evals_method: Optional[str] = None,
+        evals_method_options: Optional[dict] = None,
+        esys_method: Optional[str] = None,
+        esys_method_options: Optional[dict] = None,
     ) -> None:
-        base.QuantumSystem.__init__(self, id_str=id_str)
+        base.QubitBaseClass.__init__(
+            self,
+            id_str=id_str,
+            evals_method=evals_method,
+            evals_method_options=evals_method_options,
+            esys_method=esys_method,
+            esys_method_options=esys_method_options,
+        )
         self.EJ = EJ
         self.EC = EC
         self.ng = ng
         self.ncut = ncut
         self.truncated_dim = truncated_dim
         self._default_grid = discretization.Grid1d(-np.pi, np.pi, 151)
         self._default_n_range = (-5, 6)
-        self._image_filename = os.path.join(
-            os.path.dirname(os.path.abspath(__file__)), "qubit_img/fixed-transmon.jpg"
-        )
 
     @staticmethod
     def default_params() -> Dict[str, Any]:
         return {"EJ": 15.0, "EC": 0.3, "ng": 0.0, "ncut": 30, "truncated_dim": 10}
 
     @classmethod
     def supported_noise_channels(cls) -> List[str]:
@@ -626,28 +633,36 @@
         EC: float,
         d: float,
         flux: float,
         ng: float,
         ncut: int,
         truncated_dim: int = 6,
         id_str: Optional[str] = None,
+        evals_method: Optional[str] = None,
+        evals_method_options: Optional[dict] = None,
+        esys_method: Optional[str] = None,
+        esys_method_options: Optional[dict] = None,
     ) -> None:
-        base.QuantumSystem.__init__(self, id_str=id_str)
+        base.QubitBaseClass.__init__(
+            self,
+            id_str=id_str,
+            evals_method=evals_method,
+            evals_method_options=evals_method_options,
+            esys_method=esys_method,
+            esys_method_options=esys_method_options,
+        )
         self.EJmax = EJmax
         self.EC = EC
         self.d = d
         self.flux = flux
         self.ng = ng
         self.ncut = ncut
         self.truncated_dim = truncated_dim
         self._default_grid = discretization.Grid1d(-np.pi, np.pi, 151)
         self._default_n_range = (-5, 6)
-        self._image_filename = os.path.join(
-            os.path.dirname(os.path.abspath(__file__)), "qubit_img/tunable-transmon.jpg"
-        )
 
     @property
     def EJ(self) -> float:  # type: ignore
         """This is the effective, flux dependent Josephson energy, playing the role
         of EJ in the parent class `Transmon`"""
         return self.EJmax * np.sqrt(
             np.cos(np.pi * self.flux) ** 2
@@ -677,22 +692,21 @@
             "t1_flux_bias_line",
             "t1_charge_impedance",
         ]
 
     def d_hamiltonian_d_flux(
         self, energy_esys: Union[bool, Tuple[ndarray, ndarray]] = False
     ) -> ndarray:
-        """
-        Returns operator representing a derivative of the Hamiltonian with respect to
+        r"""Returns operator representing a derivative of the Hamiltonian with respect to
         `flux` in the charge or eigenenergy basis.
 
-        Here, the derivative is taken with respect to flux before the qubit's :math:`\phi` degree of 
-        freedom in the Hamiltonian is shifted by a flux-dependent quantity :math:`\varphi_{0}` 
-        (see Eq. 2.17 and surrounding text in PRA 76, 042319 (2007)). Then only after the flux 
-        derivative is taken, both the Hamiltonian as well as its flux derivative are assumed to 
+        Here, the derivative is taken with respect to flux before the qubit's :math:`\phi` degree of
+        freedom in the Hamiltonian is shifted by a flux-dependent quantity :math:`\varphi_{0}`
+        (see Eq. 2.17 and surrounding text in PRA 76, 042319 (2007)). Then only after the flux
+        derivative is taken, both the Hamiltonian as well as its flux derivative are assumed to
         be shifted by :math:`\varphi_{0}`.
 
         Parameters
         ----------
         energy_esys:
             If `False` (default), returns operator in the charge basis.
             If `True`, the energy eigenspectrum is computed, returns operator in the energy eigenbasis.
@@ -713,15 +727,17 @@
             * np.sin(np.pi * self.flux)
             * (self.d**2 - 1)
             / np.sqrt(
                 np.cos(np.pi * self.flux) ** 2
                 + self.d**2 * np.sin(np.pi * self.flux) ** 2
             )
             * self.cos_phi_operator()
-            - np.pi * self.EJmax * self.d 
+            - np.pi
+            * self.EJmax
+            * self.d
             / np.sqrt(
                 np.cos(np.pi * self.flux) ** 2
                 + self.d**2 * np.sin(np.pi * self.flux) ** 2
             )
             * self.sin_phi_operator()
         )
         return self.process_op(native_op=native, energy_esys=energy_esys)
```

### Comparing `scqubits-3.1.1/scqubits/core/units.py` & `scqubits-3.2.0/scqubits/core/units.py`

 * *Files 23% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 #    This source code is licensed under the BSD-style license found in the
 #    LICENSE file in the root directory of this source tree.
 ############################################################################
 
 
 import warnings
 
-from typing import List
+from typing import List, Optional
 
 # Currently set units, referred to elsewhere as "system units" (must be one of the units
 # in `_supported_units`) Often, system units need to be converted to "standard
 # units", which are considered to be `[Hz]` or `2pi/[s]`
 _current_units = "GHz"
 
 # Units that we currently support
@@ -27,20 +27,36 @@
 _units_factor = {"GHz": 1e9, "MHz": 1e6, "kHz": 1e3, "Hz": 1.0}
 
 # labels for time units obtained from 1/frequency units
 _units_time_labels = {"GHz": r"$ns$", "MHz": r"$\mu s$", "kHz": r"$ms$", "Hz": r"$s$"}
 
 
 def get_units() -> str:
-    """Get system units."""
+    """The get_units function returns the current units of the system.
+
+    Returns
+    -------
+        The current units as a string
+    """
     return _current_units
 
 
 def set_units(units: str) -> str:
-    """Set system units."""
+    """The set_units function is used to set the system units for all qubit instances.
+    The default unit system is GHz, but this can be changed by calling `set_units()` with one of the `_supported_units`
+
+    Parameters
+    ----------
+    units:
+        Specify the units that are to be used in the system
+
+    Returns
+    -------
+        The units that were set
+    """
     # Importing here avoids a cyclic import problem.
     from scqubits.core.qubit_base import QuantumSystem
 
     # Show a warning if we are changing units after some `QuantumSystems`
     # may have been instantiated.
     if QuantumSystem._quantumsystem_counter > 0:
         with warnings.catch_warnings():
@@ -59,15 +75,15 @@
         )
 
     global _current_units
     _current_units = units
     return units
 
 
-def get_units_time_label(units: str = None) -> str:
+def get_units_time_label(units: Optional[str] = None) -> str:
     """Get a latex representation of 1/units"""
     units = units or _current_units
     if units not in _supported_units:
         raise ValueError(
             "Unsupported system units given. Must be one of: {}".format(
                 str(_supported_units)
             )
@@ -84,48 +100,56 @@
 def to_standard_units(value: float) -> float:
     r"""
     Converts `value` (a frequency or angular frequency) from currently set system units,
     to standard units (Hz or  2pi/s).
 
     Parameters
     ----------
-    value: float
+    value:
         a frequency or angular frequency assumed to be in system units.
 
     Returns
     -------
-    float:
         frequency or angular frequency converted to Hz or 2pi/s
     """
     return value * _units_factor[_current_units]
 
 
 def from_standard_units(value: float) -> float:
     r"""
     Converts `value` (a frequency or angular frequency) from standard units
     (`[Hz]` or  `2\pi / [s]`) to currently set system units.
 
     Parameters
     ----------
-    value: float
+    value:
         a frequency or angular frequency assumed to be in standard units
         (`[Hz]` or  `2\pi / [s]`)
+
     Returns
     -------
-    float:
         frequency or angular frequency converted to system units
 
     """
     return value / _units_factor[_current_units]
 
 
-def units_scale_factor(units: str = None) -> float:
-    """
-    Return a numerical scaling factor that converts form Hz to `units`.
-    (given as argument or, by default, stored in  `_current_units`) .
+def units_scale_factor(units: Optional[str] = None) -> float:
+    """The units_scale_factor function returns a numerical scaling factor that converts from Hz to the `units` given as
+    a string argument. If no argument is given, the current units stored in `_current_units` are used. If the units are
+    not supported, a `ValueError` is raised.
+
+    Parameters
+    ----------
+    units:
+        units to convert to (optional; if none given, default to `_current_units`)
+
+    Returns
+    -------
+        A numerical scaling factor that converts from Hz to `units` or `_current_units`.
     """
     units = _current_units if units is None else units
 
     if units not in _supported_units:
         raise ValueError(
             "Unsupported units given. Must be one of: {}".format(str(_supported_units))
         )
```

### Comparing `scqubits-3.1.1/scqubits/core/zeropi.py` & `scqubits-3.2.0/scqubits/core/zeropi.py`

 * *Files 6% similar despite different names*

```diff
@@ -6,15 +6,14 @@
 #    Copyright (c) 2019 and later, Jens Koch and Peter Groszkowski
 #    All rights reserved.
 #
 #    This source code is licensed under the BSD-style license found in the
 #    LICENSE file in the root directory of this source tree.
 ############################################################################
 
-import os
 import warnings
 
 from typing import Any, Dict, List, Optional, Tuple, Union
 
 import numpy as np
 
 from matplotlib.axes import Axes
@@ -26,15 +25,14 @@
 import scqubits.core.central_dispatch as dispatch
 import scqubits.core.constants as constants
 import scqubits.core.descriptors as descriptors
 import scqubits.core.discretization as discretization
 import scqubits.core.qubit_base as base
 import scqubits.core.storage as storage
 import scqubits.io_utils.fileio_serializers as serializers
-import scqubits.settings as settings
 import scqubits.ui.qubit_widget as ui
 import scqubits.utils.plotting as plot
 import scqubits.utils.spectrum_utils as utils
 
 from scqubits.core.discretization import Grid1d
 from scqubits.core.noise import NoisySystem
 from scqubits.core.storage import WaveFunctionOnGrid
@@ -42,15 +40,15 @@
 # - ZeroPi noise class
 
 
 class NoisyZeroPi(NoisySystem):
     pass
 
 
-# -Symmetric 0-pi qubit, phi discretized, theta in charge basis-------------------------
+# -Symmetric 0-pi qubit, phi discretized, theta in charge basis
 
 
 class ZeroPi(base.QubitBaseClass, serializers.Serializable, NoisyZeroPi):
     r"""Zero-Pi Qubit
 
     | [1] Brooks et al., Physical Review A, 87(5), 052306 (2013). http://doi.org/10.1103/PhysRevA.87.052306
     | [2] Dempster et al., Phys. Rev. B, 90, 094518 (2014). http://doi.org/10.1103/PhysRevB.90.094518
@@ -121,16 +119,27 @@
         grid: Grid1d,
         ncut: int,
         dEJ: float = 0.0,
         dCJ: float = 0.0,
         ECS: float = None,
         truncated_dim: int = 6,
         id_str: Optional[str] = None,
+        evals_method: Optional[str] = None,
+        evals_method_options: Optional[dict] = None,
+        esys_method: Optional[str] = None,
+        esys_method_options: Optional[dict] = None,
     ) -> None:
-        base.QuantumSystem.__init__(self, id_str=id_str)
+        base.QubitBaseClass.__init__(
+            self,
+            id_str=id_str,
+            evals_method=evals_method,
+            evals_method_options=evals_method_options,
+            esys_method=esys_method,
+            esys_method_options=esys_method_options,
+        )
 
         self.EJ = EJ
         self.EL = EL
         self.ECJ = ECJ
 
         if EC is None and ECS is None:
             raise ValueError("Argument missing: must either provide EC or ECS")
@@ -150,17 +159,14 @@
 
         # _default_grid is for *theta*, needed for plotting wavefunction
         self._default_grid = discretization.Grid1d(-np.pi / 2, 3 * np.pi / 2, 200)
 
         self._init_params.remove(
             "ECS"
         )  # used in for file Serializable purposes; remove ECS as init parameter
-        self._image_filename = os.path.join(
-            os.path.dirname(os.path.abspath(__file__)), "qubit_img/zeropi.jpg"
-        )
         dispatch.CENTRAL_DISPATCH.register("GRID_UPDATE", self)
 
     @staticmethod
     def default_params() -> Dict[str, Any]:
         return {
             "EJ": 10.0,
             "EL": 0.04,
@@ -198,18 +204,18 @@
         init_params = params or self.get_initdata()
         init_params.pop("id_str", None)
         del init_params["grid"]
         init_params["grid_max_val"] = self.grid.max_val
         init_params["grid_min_val"] = self.grid.min_val
         init_params["grid_pt_count"] = self.grid.pt_count
         ui.create_widget(
-            self.set_params, init_params, image_filename=self._image_filename
+            self.set_params_from_gui, init_params, image_filename=self._image_filename
         )
 
-    def set_params(self, **kwargs) -> None:
+    def set_params_from_gui(self, **kwargs) -> None:
         phi_grid = discretization.Grid1d(
             kwargs.pop("grid_min_val"),
             kwargs.pop("grid_max_val"),
             kwargs.pop("grid_pt_count"),
         )
         self.grid = phi_grid
         for param_name, param_val in kwargs.items():
```

### Comparing `scqubits-3.1.1/scqubits/core/zeropi_full.py` & `scqubits-3.2.0/scqubits/core/zeropi_full.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,16 +6,14 @@
 #    Copyright (c) 2019 and later, Jens Koch and Peter Groszkowski
 #    All rights reserved.
 #
 #    This source code is licensed under the BSD-style license found in the
 #    LICENSE file in the root directory of this source tree.
 ############################################################################
 
-import os
-
 from typing import Any, Dict, List, Optional, Tuple, Union
 
 import numpy as np
 
 from numpy import ndarray
 from scipy import sparse
 from scipy.sparse import csc_matrix
@@ -23,15 +21,14 @@
 import scqubits
 import scqubits.core.central_dispatch as dispatch
 import scqubits.core.descriptors as descriptors
 import scqubits.core.discretization as discretization
 import scqubits.core.operators as op
 import scqubits.core.qubit_base as base
 import scqubits.io_utils.fileio_serializers as serializers
-import scqubits.settings as settings
 import scqubits.ui.qubit_widget as ui
 import scqubits.utils.spectrum_utils as spec_utils
 
 from scqubits.core.discretization import Grid1d
 from scqubits.core.noise import NoisySystem
 
 # - ZeroPi noise class
@@ -186,17 +183,21 @@
         self.dC = dC
         self.dEL = dEL
         self.zeta_cutoff = zeta_cutoff
         self.truncated_dim = truncated_dim
         self._init_params.remove(
             "ECS"
         )  # used for file IO Serializable purposes; remove ECS as init parameter
-        self._image_filename = os.path.join(
-            os.path.dirname(os.path.abspath(__file__)), "qubit_img/fullzeropi.jpg"
-        )
+
+        # This class does not yet support custom diagonalization options, but these
+        # still have to be defined
+        self.evals_method = None
+        self.evals_method_options = None
+        self.esys_method = None
+        self.esys_method_options = None
 
         dispatch.CENTRAL_DISPATCH.register("GRID_UPDATE", self)
 
     @staticmethod
     def default_params() -> Dict[str, Any]:
         return {
             "EJ": 10.0,
@@ -239,26 +240,23 @@
         init_params = params or self.get_initdata()
         init_params.pop("id_str", None)
         del init_params["grid"]
         init_params["grid_max_val"] = self.grid.max_val
         init_params["grid_min_val"] = self.grid.min_val
         init_params["grid_pt_count"] = self.grid.pt_count
         ui.create_widget(
-            self.set_params, init_params, image_filename=self._image_filename
+            self.set_params_from_gui, init_params, image_filename=self._image_filename
         )
 
-    def set_params(self, **kwargs) -> None:
-        phi_grid = discretization.Grid1d(
-            kwargs.pop("grid_min_val"),
-            kwargs.pop("grid_max_val"),
-            kwargs.pop("grid_pt_count"),
-        )
-        self.grid = phi_grid
+    def set_params_from_gui(self, **kwargs) -> None:
         for param_name, param_val in kwargs.items():
-            setattr(self, param_name, param_val)
+            if "grid_" in param_name:
+                setattr(self.grid, param_name[5:], param_val)
+            else:
+                setattr(self, param_name, param_val)
 
     def receive(self, event: str, sender: object, **kwargs) -> None:
         if sender is self._zeropi.grid:
             self.broadcast("QUANTUMSYSTEM_UPDATE")
 
     def __str__(self) -> str:
         output = super().__str__()
@@ -630,30 +628,30 @@
         self, evals_count: int, hamiltonian_mat: csc_matrix = None
     ) -> ndarray:
         if hamiltonian_mat is None:
             hamiltonian_mat = self.hamiltonian()
         evals = spec_utils.eigsh_safe(
             hamiltonian_mat,
             k=evals_count,
-            sigma=0.0,
-            which="LM",
+            # sigma=0.0,
+            which="SA",
             return_eigenvectors=False,
         )
         return np.sort(evals)
 
     def _esys_calc(
         self, evals_count: int, hamiltonian_mat: csc_matrix = None
     ) -> Tuple[ndarray, ndarray]:
         if hamiltonian_mat is None:
             hamiltonian_mat = self.hamiltonian()
         evals, evecs = spec_utils.eigsh_safe(
             hamiltonian_mat,
             k=evals_count,
-            sigma=0.0,
-            which="LM",
+            # sigma=0.0,
+            which="SA",
             return_eigenvectors=True,
         )
         evals, evecs = spec_utils.order_eigensystem(evals, evecs)
         return evals, evecs
 
     def g_phi_coupling_matrix(self, zeropi_states: ndarray) -> ndarray:
         """Returns a matrix of coupling strengths g^\\phi_{ll'}
```

### Comparing `scqubits-3.1.1/scqubits/explorer/explorer_panels.py` & `scqubits-3.2.0/scqubits/explorer/explorer_panels.py`

 * *Files 14% similar despite different names*

```diff
@@ -6,82 +6,87 @@
 #    Copyright (c) 2019 and later, Jens Koch and Peter Groszkowski
 #    All rights reserved.
 #
 #    This source code is licensed under the BSD-style license found in the
 #    LICENSE file in the root directory of this source tree.
 ############################################################################
 
-from typing import TYPE_CHECKING, List, Tuple, Union
+import itertools
+
+from typing import TYPE_CHECKING, List, Optional, Tuple, Union
 
-# import matplotlib as mlp
 import numpy as np
 
 from matplotlib import rc_context
 from matplotlib.axes import Axes
 from matplotlib.figure import Figure
 
+import scqubits
+import scqubits.core.constants
 import scqubits.core.units as units
 import scqubits.utils.plotting as plot
 
 from scqubits import SpectrumData, settings
 from scqubits.core.namedslots_array import NamedSlotsNdarray
 from scqubits.core.oscillator import Oscillator
 from scqubits.settings import matplotlib_settings
 from scqubits.utils.misc import tuple_to_short_str
 
 if TYPE_CHECKING:
     from scqubits.core.param_sweep import ParameterSlice, ParameterSweep
-    from scqubits.core.qubit_base import QuantumSystem, QubitBaseClass, QubitBaseClass1d
+    from scqubits.core.qubit_base import QuantumSystem, QubitBaseClass
 
 
 @rc_context(matplotlib_settings)
 def display_bare_spectrum(
     sweep: "ParameterSweep",
     subsys: Union["QubitBaseClass", "Oscillator"],
     param_slice: "ParameterSlice",
     fig_ax: Tuple[Figure, Axes],
     evals_count: int = None,
     subtract_ground: bool = False,
-) -> None:
+) -> Tuple[Figure, Axes]:
     subsys_index = sweep.get_subsys_index(subsys)
-    title = "bare spectrum: {}".format(subsys.id_str)
+    title = "Bare Spectrum: {}\n".format(subsys.id_str)
 
     evals_count = evals_count or -1
 
     bare_evals = sweep["bare_evals"]["subsys":subsys_index][param_slice.fixed]
     if subtract_ground:
         bare_evals = bare_evals - bare_evals[:, 0, np.newaxis]
 
     fig, axes = bare_evals[:, 0:evals_count].plot(  # type:ignore
         title=title,
         ylabel="energy [{}]".format(units.get_units()),
         fig_ax=fig_ax,
     )
     axes.axvline(param_slice.param_val, color="gray", linestyle=":")
+    return fig, axes
 
 
 @rc_context(matplotlib_settings)
 def display_anharmonicity(
     sweep: "ParameterSweep",
     subsys: "QubitBaseClass",
     param_slice: "ParameterSlice",
     fig_ax: Tuple[Figure, Axes],
 ) -> None:
     subsys_index = sweep.get_subsys_index(subsys)
 
     bare_evals = sweep["bare_evals"]["subsys":subsys_index][param_slice.fixed]
     anharmonicity = bare_evals[..., 2] - 2 * bare_evals[..., 1] + bare_evals[..., 0]
 
-    title = "anharmonicity: {}".format(subsys.id_str)
+    title = "Anharmonicity: {}".format(subsys.id_str)
     fig, axes = anharmonicity.plot(  # type:ignore
         title=title,
         ylabel="anharmonicity [{}]".format(units.get_units()),
         fig_ax=fig_ax,
     )
     axes.axvline(param_slice.param_val, color="gray", linestyle=":")
+    return fig, axes
 
 
 @rc_context(matplotlib_settings)
 def display_matrixelements(
     sweep: "ParameterSweep",
     operator_name: str,
     subsys: "QubitBaseClass",
@@ -91,37 +96,48 @@
 ) -> None:
     subsys_index = sweep.get_subsys_index(subsys)
     evecs = sweep["bare_evecs"][subsys_index][param_slice.all]
 
     fig, axes = fig_ax
     axes.cla()
 
-    title = "{}: {}".format(subsys.id_str, operator_name)
+    title = f"{subsys.id_str}: matrix elements (fixed)"
     fig, axes = subsys.plot_matrixelements(
         operator_name,
         evecs,
         evals_count=subsys.truncated_dim,
         mode=mode_str,
         show3d=False,
-        show_numbers=True,
-        show_colorbar=False,
+        show_numbers=False,
+        show_colorbar=True,
         fig_ax=fig_ax,
         title=title,
     )
+    axes.text(
+        0.5,
+        1.05,
+        f"{scqubits.core.constants.MODE_STR_DICT[mode_str](operator_name)}",
+        fontsize=9,
+        fontweight=300,
+        horizontalalignment="center",
+        verticalalignment="bottom",
+        transform=axes.transAxes,
+    )
+    return fig, axes
 
 
 @rc_context(matplotlib_settings)
 def display_matrixelement_sweep(
     sweep: "ParameterSweep",
     operator_name: str,
     subsys: "QubitBaseClass",
     param_slice: "ParameterSlice",
     mode_str: str,
     fig_ax: Tuple[Figure, Axes],
-) -> None:
+) -> Tuple[Figure, Axes]:
     subsys_index = sweep.get_subsys_index(subsys)
     evals = sweep["bare_evals"][subsys_index][param_slice.fixed]
     evecs = sweep["bare_evecs"][subsys_index][param_slice.fixed]
 
     fig, axes = fig_ax
     axes.cla()
 
@@ -145,103 +161,124 @@
         evecs = specdata.state_table[index]
         matelem_table[index] = subsys.matrixelement_table(
             operator_name, evecs=evecs, evals_count=subsys.truncated_dim
         )
 
     specdata.matrixelem_table = matelem_table
 
-    title = "{}: {}".format(subsys.id_str, operator_name)
+    title = f"{subsys.id_str}: matrix elements (sweep)"
     fig, axes = plot.matelem_vs_paramvals(
         specdata, mode=mode_str, fig_ax=fig_ax, title=title
     )
     axes.axvline(param_slice.param_val, color="gray", linestyle=":")
+    return fig, axes
 
 
 @rc_context(matplotlib_settings)
 def display_bare_wavefunctions(
     sweep: "ParameterSweep",
     subsys: "QubitBaseClass",
     param_slice: "ParameterSlice",
     fig_ax: Tuple[Figure, Axes],
-) -> None:
+    mode="real",
+    which=-1,
+) -> Tuple[Figure, Axes]:
     subsys_index = sweep.get_subsys_index(subsys)
 
     evals = sweep["bare_evals"][subsys_index][param_slice.all]
     evecs = sweep["bare_evecs"][subsys_index][param_slice.all]
 
     settings.DISPATCH_ENABLED = False
     sweep._update_hilbertspace(sweep, *param_slice.all_values)
     settings.DISPATCH_ENABLED = True
 
-    title = "wavefunctions: {}".format(subsys.id_str)
-    __ = subsys.plot_wavefunction(
-        which=-1, esys=(evals, evecs), title=title, fig_ax=fig_ax
+    title = "Wavefunctions: {}".format(subsys.id_str)
+    return subsys.plot_wavefunction(
+        which=which, esys=(evals, evecs), mode=mode, title=title, fig_ax=fig_ax
     )
 
 
 @rc_context(matplotlib_settings)
 def display_transitions(
     sweep: "ParameterSweep",
     photon_number: int,
     subsys_list: List["QuantumSystem"],
     initial: Union[int, Tuple[int, ...]],
     sidebands: bool,
     param_slice: "ParameterSlice",
     fig_ax: Tuple[Figure, Axes],
-) -> None:
-    if len(subsys_list) == 1:
-        title = r"{}-photon {} transitions".format(photon_number, subsys_list[0].id_str)
+) -> Tuple[Figure, Axes]:
+    if photon_number == 1:
+        title = r"Transition Spectrum"
     else:
-        title = r"{}-photon transitions".format(photon_number)
+        title = r"{}-photon Transitions".format(photon_number)
     sliced_sweep = sweep if param_slice.fixed == tuple() else sweep[param_slice.fixed]
     fig, axes = sliced_sweep.plot_transitions(
         subsystems=subsys_list,
         initial=initial,
         photon_number=photon_number,
         title=title,
         sidebands=sidebands,
         fig_ax=fig_ax,
     )
     axes.axvline(param_slice.param_val, color="gray", linestyle=":")
 
+    info_string = "Highlighted: transitions for "
+    for sys in subsys_list:
+        info_string += sys.id_str + ", "
+    info_string += "with sidebands" if sidebands else "no sidebands"
+    axes.text(
+        0.5,
+        1.05,
+        info_string,
+        fontsize=9,
+        fontweight=300,
+        horizontalalignment="center",
+        verticalalignment="bottom",
+        transform=axes.transAxes,
+    )
+
+    return fig, axes
+
 
 @rc_context(matplotlib_settings)
 def display_cross_kerr(
     sweep: "ParameterSweep",
     subsys1: "QuantumSystem",
     subsys2: "QuantumSystem",
     param_slice: "ParameterSlice",
     fig_ax: Tuple[Figure, Axes],
-) -> None:
+    which: Optional[Union[int, Tuple[int, int]]] = None,
+) -> Tuple[Figure, Axes]:
     subsys1_index = sweep.get_subsys_index(subsys1)
     subsys2_index = sweep.get_subsys_index(subsys2)
     type_list = [type(sys) for sys in [subsys1, subsys2]]
     if type_list.count(Oscillator) == 1:
-        title = f"ac Stark: {subsys1.id_str} + {subsys2.id_str}"
-        ylabel = rf"ac Stark shift $\chi^{{{subsys1_index},{subsys2_index}}}$"
-        levels_list = [1]
+        title = f"AC Stark: {subsys1.id_str} + {subsys2.id_str}"
+        ylabel = rf"AC Stark Shift $\chi^{{{subsys1_index},{subsys2_index}}}_\ell$"
+        level = which or 1
         kerr_data = sweep["chi"][subsys1_index, subsys2_index]
         if param_slice.fixed != tuple():
             kerr_data = kerr_data[param_slice.fixed]
-        label_list = []
-        kerr_datasets = [kerr_data[..., level] for level in levels_list]
+        label_list = [level]
+        kerr_datasets = [kerr_data[..., level]]
     elif type_list.count(Oscillator) == 2:
-        title = r"cross-Kerr: {} - {}".format(subsys1.id_str, subsys2.id_str)
-        ylabel = r"Kerr coefficient $K_{{},{}}$".format(subsys1_index, subsys2_index)
+        title = r"Cross-Kerr: {} - {}".format(subsys1.id_str, subsys2.id_str)
+        ylabel = r"Kerr Coefficient $K_{{},{}}$".format(subsys1_index, subsys2_index)
         level_pairs = [(1, 1)]
         kerr_data = sweep["kerr"][subsys1_index, subsys2_index]
         if param_slice.fixed != tuple():
             kerr_data = kerr_data[param_slice.fixed]
         label_list = []
         kerr_datasets = [
             kerr_data[..., level1, level2] for level1, level2 in level_pairs
         ]
     else:
-        title = "cross-Kerr: {} \u2194 {}".format(subsys1.id_str, subsys2.id_str)
-        ylabel = r"Kerr coefficient $\Lambda^{{{},{}}}_{{ll'}}$".format(
+        title = "Cross-Kerr: {} \u2194 {}".format(subsys1.id_str, subsys2.id_str)
+        ylabel = r"Kerr Coefficient $\Lambda^{{{},{}}}_{{ll'}}$".format(
             subsys1_index, subsys2_index
         )
         level_pairs = [(0, 1), (1, 0), (1, 1), (1, 2), (2, 1), (2, 2)]
         kerr_data = sweep["kerr"][subsys1_index, subsys2_index]
         if param_slice.fixed != tuple():
             kerr_data = kerr_data[param_slice.fixed]
         label_list = [tuple_to_short_str(pair) for pair in level_pairs]
@@ -254,44 +291,71 @@
     fig, axes = kerr_namedarray.plot(
         title=title,
         label_list=label_list if label_list else None,
         ylabel=ylabel + "[{}]".format(units.get_units()),
         fig_ax=fig_ax,
     )
     axes.axvline(param_slice.param_val, color="gray", linestyle=":")
+    return fig, axes
 
 
 @rc_context(matplotlib_settings)
-def display_self_kerr(
+def display_qubit_self_kerr(
     sweep: "ParameterSweep",
     subsys: "QuantumSystem",
     param_slice: "ParameterSlice",
     fig_ax: Tuple[Figure, Axes],
-) -> None:
+    which: Optional[List[Tuple[int, int]]] = None,
+) -> Tuple[Figure, Axes]:
     subsys_index = sweep.get_subsys_index(subsys)
-    title = r"self-Kerr: {}".format(subsys.id_str)
-    if isinstance(subsys, Oscillator):
-        ylabel = "Kerr coefficient $K_{{{}}}$".format(subsys_index)
-    else:
-        ylabel = r"Kerr coefficient $\Lambda^{{{},{}}}_{{ll'}}$".format(
-            subsys_index, subsys_index
-        )
+    title = r"Self-Kerr: {}".format(subsys.id_str)
+    ylabel = r"Kerr coefficient $\Lambda^{{{},{}}}_{{ll}}$".format(
+        subsys_index, subsys_index
+    )
 
     kerr_data = sweep["kerr"][subsys_index, subsys_index]
     if param_slice.fixed != tuple():
         kerr_data = kerr_data[param_slice.fixed]
 
-    level_pairs = [(1, 1), (2, 2)]
+    if not which:
+        level_pairs = list(itertools.combinations(list(range(subsys.truncated_dim)), 2))
+    else:
+        level_pairs = which
 
     kerr_datasets = []
-    for level1, level2 in level_pairs:
-        kerr_datasets.append(kerr_data[..., level1, level2])
+    for pair in level_pairs:
+        kerr_datasets.append(kerr_data[..., pair[0], pair[1]])
     kerr_datasets = np.asarray(kerr_datasets).T
     kerr_namedarray = NamedSlotsNdarray(kerr_datasets, kerr_data.param_info)
 
     fig, axes = kerr_namedarray.plot(
         title=title,
-        label_list=["11", "22"],
+        label_list=level_pairs,
+        ylabel=ylabel + "[{}]".format(units.get_units()),
+        fig_ax=fig_ax,
+    )
+    axes.axvline(param_slice.param_val, color="gray", linestyle=":")
+    return fig, axes
+
+
+@rc_context(matplotlib_settings)
+def display_self_kerr(
+    sweep: "ParameterSweep",
+    subsys: Union[scqubits.Oscillator, scqubits.KerrOscillator],
+    param_slice: "ParameterSlice",
+    fig_ax: Tuple[Figure, Axes],
+) -> Tuple[Figure, Axes]:
+    subsys_index = sweep.get_subsys_index(subsys)
+    title = r"Self-Kerr: {}".format(subsys.id_str)
+
+    ylabel = "Kerr coefficient $K_{{{}}}$".format(subsys_index)
+    kerr_data = sweep["kerr"][subsys_index, subsys_index]
+    if param_slice.fixed != tuple():
+        kerr_data = kerr_data[param_slice.fixed]
+
+    fig, axes = kerr_data.plot(
+        title=title,
         ylabel=ylabel + "[{}]".format(units.get_units()),
         fig_ax=fig_ax,
     )
     axes.axvline(param_slice.param_val, color="gray", linestyle=":")
+    return fig, axes
```

### Comparing `scqubits-3.1.1/scqubits/io_utils/fileio.py` & `scqubits-3.2.0/scqubits/io_utils/fileio.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 ############################################################################
 """
 Helper routines for writing data to files.
 """
 
 import os
 
-from typing import TYPE_CHECKING, Any, Callable, Dict, Union
+from typing import TYPE_CHECKING, Any, Callable, Dict, Optional, Union
 
 from numpy import ndarray
 
 import scqubits.core.constants as const
 import scqubits.io_utils.fileio_serializers as io_serializers
 
 if TYPE_CHECKING:
@@ -150,16 +150,16 @@
             "Extension '{}' of given file name '{}' does not match any supported "
             "file type: {}".format(suffix, file_name, const.FILE_TYPES)
         )
 
     @staticmethod
     def get_reader(
         file_name: str,
-        file_handle: "h5py.Group" = None,
-        get_external_reader: Callable = None,
+        file_handle: Optional["h5py.Group"] = None,
+        get_external_reader: Optional[Callable] = None,
     ) -> Union["CSVReader", "H5Reader"]:
         """
         Based on the extension of the provided file name, return the appropriate
         reader engine.
         """
         if get_external_reader:
             return get_external_reader(file_name, file_handle=file_handle)
```

### Comparing `scqubits-3.1.1/scqubits/io_utils/fileio_backends.py` & `scqubits-3.2.0/scqubits/io_utils/fileio_backends.py`

 * *Files 0% similar despite different names*

```diff
@@ -18,23 +18,21 @@
 import os
 import re
 
 from abc import ABC, abstractmethod
 from typing import TYPE_CHECKING, Any, Dict, List, Tuple, Union
 
 import numpy as np
-
 from numpy import ndarray
 
 import scqubits.io_utils.fileio as io
 import scqubits.utils.misc as utils
 
 try:
     import h5py
-
     from h5py import AttributeManager, File, Group
 except ImportError:
     _HAS_H5PY = False
 else:
     _HAS_H5PY = True
 
 if TYPE_CHECKING:
```

### Comparing `scqubits-3.1.1/scqubits/io_utils/fileio_qutip.py` & `scqubits-3.2.0/scqubits/io_utils/fileio_qutip.py`

 * *Files identical despite different names*

### Comparing `scqubits-3.1.1/scqubits/io_utils/fileio_serializers.py` & `scqubits-3.2.0/scqubits/io_utils/fileio_serializers.py`

 * *Files 2% similar despite different names*

```diff
@@ -126,14 +126,25 @@
     ndarrays: Dict[str, ndarray],
     objects: Dict[str, object],
 ) -> Tuple[Dict, Dict, Dict]:
     attributes[name] = obj
     return attributes, ndarrays, objects
 
 
+def _add_boundmethod_attribute(
+    name: str,
+    obj: Any,
+    attributes: Dict[str, Any],
+    ndarrays: Dict[str, ndarray],
+    objects: Dict[str, object],
+) -> Tuple[Dict, Dict, Dict]:
+    attributes[name] = obj()
+    return attributes, ndarrays, objects
+
+
 TO_ATTRIBUTE = (Expr, str, Number, dict, OrderedDict, list, tuple, bool, np.bool_)
 TO_NDARRAY = (np.ndarray,)
 TO_OBJECT = (Serializable,)
 
 
 def type_dispatch(entity: Serializable) -> Callable:
     """
@@ -144,14 +155,16 @@
         return _add_attribute
     if isinstance(entity, TO_OBJECT):
         return _add_object
     if isinstance(entity, TO_NDARRAY):
         if entity.dtype == "O":
             return _add_object
         return _add_ndarray
+    if callable(entity) and "_operator" in entity.__name__:
+        return _add_boundmethod_attribute
     # no match, try treating as object, though this may fail
     return _add_object
 
 
 def Expr_serialize(expr_instance: Expr) -> "IOData":
     """
     Create an IODate instance for a sympy expression via string conversion
```

### Comparing `scqubits-3.1.1/scqubits/settings.py` & `scqubits-3.2.0/scqubits/settings.py`

 * *Files 13% similar despite different names*

```diff
@@ -23,29 +23,29 @@
 #
 #    This source code is licensed under the BSD-style license found in the
 #    LICENSE file in the root directory of this source tree.
 #######################################################################################
 
 import warnings
 
-from typing import Any, Type, Union
+from typing import Any, Optional, Type, Union
 
-import matplotlib as mpl
+import matplotlib.font_manager as mpl_font
 import numpy as np
 
 from cycler import cycler
 
 
 # Set format for output of warnings
 def warning_on_one_line(
     message: Union[Warning, str],
     category: Type[Warning],
     filename: str,
     lineno: int,
-    line: str = None,
+    line: Optional[str] = None,
 ) -> str:
     return "{}: {}\n {}: {}".format(category.__name__, message, filename, lineno)
 
 
 warnings.formatwarning = warning_on_one_line
 
 
@@ -89,16 +89,29 @@
 
 # Select multiprocessing library
 # Options:  'multiprocessing'
 #           'pathos'
 MULTIPROC = "pathos"
 
 # Matplotlib options -------------------------------------------------------------------
+# select fonts
+FONT_SELECTED = None
+try:
+    font_names = mpl_font.get_font_names()
+    for font in ["IBM Plex Sans", "Roboto", "Arial", "Helvetica"]:
+        if font in font_names:
+            FONT_SELECTED = font
+            break
+    if not FONT_SELECTED:
+        FONT_SELECTED = "sans-serif"
+except AttributeError:
+    FONT_SELECTED = "sans-serif"
+
 # set matplotlib defaults for use in @mpl.rc_context
-off_black = "0.2"
+OFF_BLACK = "0.2"
 matplotlib_settings = {
     "axes.prop_cycle": cycler(
         color=[
             "#016E82",
             "#333795",
             "#2E5EAC",
             "#4498D3",
@@ -108,41 +121,42 @@
             "#F47752",
             "#19B35A",
             "#EDE83B",
             "#ABD379",
             "#F9E6BE",
         ]
     ),
-    "font.family": "IBM Plex Sans, Roboto, Arial, Helvetica, DejaVu Sans",
+    "font.family": FONT_SELECTED,
     "font.size": 11,
     "font.weight": 500,
     "axes.labelsize": 11,
     "axes.titlesize": 11,
+    "axes.titleweight": 500,
     "xtick.labelsize": 10,
     "ytick.labelsize": 10,
-    "xtick.labelcolor": off_black,
-    "ytick.labelcolor": off_black,
-    "xtick.color": off_black,
-    "ytick.color": off_black,
-    "axes.labelcolor": off_black,
-    "axes.edgecolor": off_black,
-    "axes.titlecolor": off_black
+    "xtick.labelcolor": OFF_BLACK,
+    "ytick.labelcolor": OFF_BLACK,
+    "xtick.color": OFF_BLACK,
+    "ytick.color": OFF_BLACK,
+    "axes.labelcolor": OFF_BLACK,
+    "axes.edgecolor": OFF_BLACK,
+    "axes.titlecolor": OFF_BLACK,
 }
 
 
 # toggle top and right axes on and off
 DESPINE = True
 
 # This is a setting for number of points in stencil to approximate derivatives
 STENCIL = 7
 
 # global random number generator for consistent initial state vector v0 in ARPACK
-SEED = 63142
-RNG = np.random.default_rng(seed=SEED)
-RANDOM_ARRAY = RNG.random(size=10000000)
+_SEED = 63142
+_RNG = np.random.default_rng(seed=_SEED)
+RANDOM_ARRAY = _RNG.random(size=10000000)
 
 # toggle fuzzy value-based slicing and warnings about it on and off
 FUZZY_SLICING = False
 FUZZY_WARNING = True
 
 # Enable/disable warning about default used in t1 coherence calculations
 T1_DEFAULT_WARNING = True
```

### Comparing `scqubits-3.1.1/scqubits/testing.py` & `scqubits-3.2.0/scqubits/testing.py`

 * *Files identical despite different names*

### Comparing `scqubits-3.1.1/scqubits/tests/conftest.py` & `scqubits-3.2.0/scqubits/tests/conftest.py`

 * *Files 0% similar despite different names*

```diff
@@ -199,14 +199,16 @@
         testname = self.file_str + "_2." + io_type
         specdata = SpectrumData.create_from_file(DATADIR + testname)
         self.qbt = self.qbt_type(**specdata.system_params)
         evecs_reference = specdata.state_table
         return self.eigenvecs(io_type, evecs_reference)
 
     def test_plot_wavefunction(self, io_type):
+        if "plot_wavefunction" not in dir(self.qbt_type):
+            pytest.skip("This is expected, no reason for concern.")
         testname = self.file_str + "_1." + io_type
         specdata = SpectrumData.create_from_file(DATADIR + testname)
         self.qbt = self.qbt_type(**specdata.system_params)
         self.qbt.plot_wavefunction(esys=None, which=5, mode="real")
         self.qbt.plot_wavefunction(esys=None, which=9, mode="abs_sqr")
 
     def test_plot_evals_vs_paramvals(self, num_cpus, io_type):
@@ -259,13 +261,13 @@
             self.op1_str,
             self.param_name,
             self.param_list,
             select_elems=[(0, 0), (1, 4), (1, 0)],
         )
 
     def test_plot_potential(self, io_type):
+        if "plot_potential" not in dir(self.qbt_type):
+            pytest.skip("This is expected, no reason for concern.")
         testname = self.file_str + "_1.hdf5"
         specdata = SpectrumData.create_from_file(DATADIR + testname)
         self.qbt = self.qbt_type(**specdata.system_params)
-        if "plot_potential" not in dir(self.qbt):
-            pytest.skip("This is expected, no reason for concern.")
         self.qbt.plot_potential()
```

### Comparing `scqubits-3.1.1/scqubits/tests/data/cos2phiqubit_1.hdf5` & `scqubits-3.2.0/scqubits/tests/data/cos2phiqubit_1.hdf5`

 * *Files identical despite different names*

### Comparing `scqubits-3.1.1/scqubits/tests/data/cos2phiqubit_2.hdf5` & `scqubits-3.2.0/scqubits/tests/data/cos2phiqubit_2.hdf5`

 * *Files identical despite different names*

### Comparing `scqubits-3.1.1/scqubits/tests/data/cos2phiqubit_4.hdf5` & `scqubits-3.2.0/scqubits/tests/data/cos2phiqubit_4.hdf5`

 * *Files identical despite different names*

### Comparing `scqubits-3.1.1/scqubits/tests/data/cos2phiqubit_5.hdf5` & `scqubits-3.2.0/scqubits/tests/data/cos2phiqubit_5.hdf5`

 * *Files identical despite different names*

### Comparing `scqubits-3.1.1/scqubits/tests/data/fluxonium_1.hdf5` & `scqubits-3.2.0/scqubits/tests/data/fluxonium_1.hdf5`

 * *Files identical despite different names*

### Comparing `scqubits-3.1.1/scqubits/tests/data/fluxonium_2.hdf5` & `scqubits-3.2.0/scqubits/tests/data/fluxonium_2.hdf5`

 * *Files identical despite different names*

### Comparing `scqubits-3.1.1/scqubits/tests/data/fluxonium_4.hdf5` & `scqubits-3.2.0/scqubits/tests/data/fluxonium_4.hdf5`

 * *Files identical despite different names*

### Comparing `scqubits-3.1.1/scqubits/tests/data/fluxonium_5.hdf5` & `scqubits-3.2.0/scqubits/tests/data/fluxonium_5.hdf5`

 * *Files identical despite different names*

### Comparing `scqubits-3.1.1/scqubits/tests/data/fluxqubit_1.hdf5` & `scqubits-3.2.0/scqubits/tests/data/fluxqubit_1.hdf5`

 * *Files identical despite different names*

### Comparing `scqubits-3.1.1/scqubits/tests/data/fluxqubit_2.hdf5` & `scqubits-3.2.0/scqubits/tests/data/fluxqubit_2.hdf5`

 * *Files identical despite different names*

### Comparing `scqubits-3.1.1/scqubits/tests/data/fluxqubit_4.hdf5` & `scqubits-3.2.0/scqubits/tests/data/fluxqubit_4.hdf5`

 * *Files identical despite different names*

### Comparing `scqubits-3.1.1/scqubits/tests/data/fluxqubit_5.hdf5` & `scqubits-3.2.0/scqubits/tests/data/fluxqubit_5.hdf5`

 * *Files identical despite different names*

### Comparing `scqubits-3.1.1/scqubits/tests/data/fullzeropi_1.hdf5` & `scqubits-3.2.0/scqubits/tests/data/fullzeropi_1.hdf5`

 * *Files identical despite different names*

### Comparing `scqubits-3.1.1/scqubits/tests/data/fullzeropi_2.hdf5` & `scqubits-3.2.0/scqubits/tests/data/fullzeropi_2.hdf5`

 * *Files identical despite different names*

### Comparing `scqubits-3.1.1/scqubits/tests/data/transmon_1.hdf5` & `scqubits-3.2.0/scqubits/tests/data/transmon_1.hdf5`

 * *Files identical despite different names*

### Comparing `scqubits-3.1.1/scqubits/tests/data/transmon_2.hdf5` & `scqubits-3.2.0/scqubits/tests/data/transmon_2.hdf5`

 * *Files identical despite different names*

### Comparing `scqubits-3.1.1/scqubits/tests/data/transmon_4.hdf5` & `scqubits-3.2.0/scqubits/tests/data/transmon_4.hdf5`

 * *Files identical despite different names*

### Comparing `scqubits-3.1.1/scqubits/tests/data/transmon_5.hdf5` & `scqubits-3.2.0/scqubits/tests/data/transmon_5.hdf5`

 * *Files identical despite different names*

### Comparing `scqubits-3.1.1/scqubits/tests/data/zeropi-test.hdf5` & `scqubits-3.2.0/scqubits/tests/data/zeropi-test.hdf5`

 * *Files identical despite different names*

### Comparing `scqubits-3.1.1/scqubits/tests/data/zeropi_1.hdf5` & `scqubits-3.2.0/scqubits/tests/data/zeropi_1.hdf5`

 * *Files identical despite different names*

### Comparing `scqubits-3.1.1/scqubits/tests/data/zeropi_2.hdf5` & `scqubits-3.2.0/scqubits/tests/data/zeropi_2.hdf5`

 * *Files identical despite different names*

### Comparing `scqubits-3.1.1/scqubits/tests/data/zeropi_4.hdf5` & `scqubits-3.2.0/scqubits/tests/data/zeropi_4.hdf5`

 * *Files identical despite different names*

### Comparing `scqubits-3.1.1/scqubits/tests/data/zeropi_5.hdf5` & `scqubits-3.2.0/scqubits/tests/data/zeropi_5.hdf5`

 * *Files identical despite different names*

### Comparing `scqubits-3.1.1/scqubits/tests/data/zpifull-test.hdf5` & `scqubits-3.2.0/scqubits/tests/data/zpifull-test.hdf5`

 * *Files identical despite different names*

### Comparing `scqubits-3.1.1/scqubits/tests/test_centraldispatch.py` & `scqubits-3.2.0/scqubits/tests/test_centraldispatch.py`

 * *Files identical despite different names*

### Comparing `scqubits-3.1.1/scqubits/tests/test_circuit.py` & `scqubits-3.2.0/scqubits/tests/test_circuit.py`

 * *Files identical despite different names*

### Comparing `scqubits-3.1.1/scqubits/tests/test_circuit_plot.py` & `scqubits-3.2.0/scqubits/tests/test_circuit_plot.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,13 +1,10 @@
 import os
-import numpy as np
 
 import scqubits as scq
-from scqubits import truncation_template
-from scqubits.core.circuit_utils import example_circuit
 
 TESTDIR, _ = os.path.split(scq.__file__)
 TESTDIR = os.path.join(TESTDIR, "tests", "")
 DATADIR = os.path.join(TESTDIR, "data", "")
 
 
 circ = scq.Circuit(
```

### Comparing `scqubits-3.1.1/scqubits/tests/test_cos2phiqubit.py` & `scqubits-3.2.0/scqubits/tests/test_cos2phiqubit.py`

 * *Files identical despite different names*

### Comparing `scqubits-3.1.1/scqubits/tests/test_explorer.py` & `scqubits-3.2.0/scqubits/tests/test_explorer.py`

 * *Files 8% similar despite different names*

```diff
@@ -20,22 +20,22 @@
     tmon1 = scq.TunableTransmon(
         EJmax=40.0,
         EC=0.2,
         d=0.1,
         flux=0.0,
         ng=0.3,
         ncut=40,
-        truncated_dim=4,  # after diagonalization, we will keep 3 levels
+        truncated_dim=5,
     )
 
     tmon2 = scq.TunableTransmon(
         EJmax=15.0, EC=0.15, d=0.02, flux=0.0, ng=0.0, ncut=30, truncated_dim=5
     )
 
-    resonator = scq.Oscillator(E_osc=4.5, truncated_dim=4)  # up to 3 photons (0,1,2,3)
+    resonator = scq.Oscillator(E_osc=4.5, truncated_dim=4)
 
     hilbertspace = scq.HilbertSpace([tmon1, tmon2, resonator])
 
     g1 = 0.1  # coupling resonator-CPB1 (without charge matrix elements)
     g2 = 0.2  # coupling resonator-CPB2 (without charge matrix elements)
 
     hilbertspace.add_interaction(
```

### Comparing `scqubits-3.1.1/scqubits/tests/test_fluxonium.py` & `scqubits-3.2.0/scqubits/tests/test_fluxonium.py`

 * *Files identical despite different names*

### Comparing `scqubits-3.1.1/scqubits/tests/test_fluxqubit.py` & `scqubits-3.2.0/scqubits/tests/test_fluxqubit.py`

 * *Files identical despite different names*

### Comparing `scqubits-3.1.1/scqubits/tests/test_fullzeropi.py` & `scqubits-3.2.0/scqubits/tests/test_fullzeropi.py`

 * *Files identical despite different names*

### Comparing `scqubits-3.1.1/scqubits/tests/test_gui.py` & `scqubits-3.2.0/scqubits/tests/test_gui.py`

 * *Files identical despite different names*

### Comparing `scqubits-3.1.1/scqubits/tests/test_hilbertspace.py` & `scqubits-3.2.0/scqubits/tests/test_hilbertspace.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -9,17 +9,17 @@
 #
 #    This source code is licensed under the BSD-style license found in the
 #    LICENSE file in the root directory of this source tree.
 ############################################################################
 
 import numpy as np
 import pytest
+import qutip as qt
 
 import scqubits as scq
-import qutip as qt
 
 from scqubits.core.hilbert_space import HilbertSpace
 from scqubits.utils.spectrum_utils import get_matrixelement_table
 
 
 @pytest.mark.usefixtures("num_cpus")
 class TestHilbertSpace:
```

### Comparing `scqubits-3.1.1/scqubits/tests/test_namedslotsndarray.py` & `scqubits-3.2.0/scqubits/tests/test_namedslotsndarray.py`

 * *Files identical despite different names*

### Comparing `scqubits-3.1.1/scqubits/tests/test_noise.py` & `scqubits-3.2.0/scqubits/tests/test_noise.py`

 * *Files 6% similar despite different names*

```diff
@@ -66,16 +66,17 @@
     ),
     "FluxQubit": np.array(
         [
             44697811.55376147,
             44697796.19976752,
             1822725.05439264,
             1685277.68169804,
+            66760.19238822,
             np.inf,
-            842638.84084902,
+            61859.237880050845,
         ]
     ),
     "ZeroPi": np.array(
         [3806664.01882053, 41202847.68864658, np.inf, np.inf, np.inf, 3484716.71474053]
     ),
     "Cos2PhiQubit": np.array(
         [
```

### Comparing `scqubits-3.1.1/scqubits/tests/test_parameters.py` & `scqubits-3.2.0/scqubits/tests/test_parameters.py`

 * *Files identical despite different names*

### Comparing `scqubits-3.1.1/scqubits/tests/test_parametersweep.py` & `scqubits-3.2.0/scqubits/tests/test_parametersweep.py`

 * *Files identical despite different names*

### Comparing `scqubits-3.1.1/scqubits/tests/test_spectrumlookup.py` & `scqubits-3.2.0/scqubits/tests/test_spectrumlookup.py`

 * *Files identical despite different names*

### Comparing `scqubits-3.1.1/scqubits/tests/test_transmon.py` & `scqubits-3.2.0/scqubits/tests/test_transmon.py`

 * *Files identical despite different names*

### Comparing `scqubits-3.1.1/scqubits/tests/test_units.py` & `scqubits-3.2.0/scqubits/tests/test_units.py`

 * *Files identical despite different names*

### Comparing `scqubits-3.1.1/scqubits/tests/test_zeropi.py` & `scqubits-3.2.0/scqubits/tests/test_zeropi.py`

 * *Files identical despite different names*

### Comparing `scqubits-3.1.1/scqubits/ui/__init__.py` & `scqubits-3.2.0/scqubits/ui/__init__.py`

 * *Files identical despite different names*

### Comparing `scqubits-3.1.1/scqubits/ui/gui.py` & `scqubits-3.2.0/scqubits/ui/gui.py`

 * *Files 24% similar despite different names*

```diff
@@ -7,251 +7,174 @@
 #    All rights reserved.
 #
 #    This source code is licensed under the BSD-style license found in the
 #    LICENSE file in the root directory of this source tree.
 ############################################################################
 
 import math
-import warnings
 
-from distutils.version import StrictVersion
-
-from pathlib import Path
-from typing import Any, Callable, Dict, List, Optional, Tuple, Union
+from typing import Any, Dict, List, Optional, Tuple, Union
 
+import matplotlib
 import matplotlib.pyplot as plt
 import numpy as np
 
-import matplotlib
-from matplotlib import get_backend as get_matplotlib_backend
 from matplotlib.figure import Axes, Figure
 
+import scqubits as scq
+import scqubits.ui.gui_custom_widgets as ui
+import scqubits.ui.gui_defaults as gui_defaults
+import scqubits.ui.gui_navbar as gui_navbar
+import scqubits.utils.misc as utils
+
 from scqubits.core.discretization import Grid1d
-from scqubits.core.flux_qubit import FluxQubit
-from scqubits.core.zeropi import ZeroPi
-from scqubits.core.zeropi_full import FullZeroPi
 from scqubits.settings import matplotlib_settings
+from scqubits.ui.gui_custom_widgets import flex_column, flex_row
+from scqubits.ui.gui_defaults import NAV_COLOR
+from scqubits.ui.gui_setup import (
+    init_dict_v_noise_params,
+    init_dict_v_plot_options,
+    init_filename_textfield,
+    init_qubit_params_widgets_dict,
+    init_ranges_widgets_dict,
+    init_save_btn,
+)
+from scqubits.utils.misc import _HAS_WIDGET_BACKEND
 
 try:
-    from ipywidgets import (
-        Box,
-        Button,
-        Checkbox,
-        Dropdown,
-        FloatRangeSlider,
-        FloatSlider,
-        FloatText,
-        HBox,
-        HTML,
-        Image,
-        IntSlider,
-        IntText,
-        Label,
-        Layout,
-        Output,
-        SelectMultiple,
-        Tab,
-        Text,
-        ToggleButtons,
-        VBox,
-    )
+    import ipyvuetify as v
+    import ipywidgets
 except ImportError:
-    _HAS_IPYWIDGETS = False
+    _HAS_IPYVUETIFY = False
 else:
-    _HAS_IPYWIDGETS = True
+    _HAS_IPYVUETIFY = True
 
 try:
     from IPython.display import display
 except ImportError:
     _HAS_IPYTHON = False
 else:
     _HAS_IPYTHON = True
 
-MATPLOTLIB_WIDGET_BACKEND = "module://ipympl.backend_nbagg"
-_HAS_WIDGET_BACKEND = get_matplotlib_backend() == MATPLOTLIB_WIDGET_BACKEND
 
-import scqubits as scq
-import scqubits.ui.gui_defaults as gui_defaults
-import scqubits.core.noise as noise
-import scqubits.utils.misc as utils
-
-from scqubits.core.qubit_base import QubitBaseClass
+QUBITS_WITH_GRID_INIT = (scq.ZeroPi, scq.FullZeroPi)  #  scq.Bifluxon
+QUBITS_WITH_PHI_GRID = (
+    scq.Transmon,
+    scq.TunableTransmon,
+    scq.Fluxonium,
+    scq.FluxQubit,
+    scq.Cos2PhiQubit,
+)
+QUBITS_WITH_THETA_GRID = (scq.ZeroPi, scq.Cos2PhiQubit)  # scq.Bifluxon,
+QUBITS_WITHOUT_WAVEFUNCTION_PLOT = (scq.FullZeroPi,)  # scq.Snailmon
+QUBITS_WITH_2D_WAVEFUNCTION_PLOT = (
+    scq.FluxQubit,
+    scq.ZeroPi,
+    scq.Cos2PhiQubit,
+    # scq.Bifluxon,
+)
 
 
 class GUI:
-    # Handle to the most recently generated Figure, Axes tuple
-    fig_ax: Optional[Tuple[Figure, Axes]] = None
+    """Generates the GUI for scqubits, handling single-qubit properties"""
 
-    def __repr__(self):
-        return ""
+    fig_ax: Optional[
+        Tuple[Figure, Axes]
+    ] = None  # Handle to the most recently generated Figure, Axes tuple
+
+    no_plot_refresh_widgets = [
+        "info_panel",
+        "literature_params",
+        "link_HTML",
+    ]
 
-    @utils.Required(ipywidgets=_HAS_IPYWIDGETS, IPython=_HAS_IPYTHON)
+    @utils.Required(ipyvuetify=_HAS_IPYVUETIFY, IPython=_HAS_IPYTHON)
     def __init__(self):
-        scq.settings.PROGRESSBAR_DISABLED = False
+        utils.check_matplotlib_compatibility()
+
+        # scq.settings.PROGRESSBAR_DISABLED = False
         scq.settings.T1_DEFAULT_WARNING = False
-        if _HAS_WIDGET_BACKEND and StrictVersion(
-            matplotlib.__version__
-        ) < StrictVersion("3.5.1"):
-            warnings.warn(
-                "The widget backend requires Matplotlib >=3.5.1 for proper functioning",
-                UserWarning,
-            )
 
-        # Display Elements
-        self.fig: Figure
-        self.plot_output: Output = Output(layout={"width": "100%"})
-        self.tab_widget: Tab = Tab(layout=Layout(width="95%"))
-
-        self.active_qubit: QubitBaseClass
-        self.manual_update_bool: bool = False
-        self.plot_change_bool: bool = True
+        self.plot_renewal_requested = True
 
         self.active_defaults: Dict[str, Any] = {}
         self.qubit_params: Dict[str, Union[int, float, None]] = {}
-        self.ranges_widgets: Dict[str, Dict[str, Union[IntText, FloatText]]] = {}
         self.qubit_scan_params: Dict[str, Union[int, float, None]] = {}
-        self.noise_param_widgets: Dict[str, Union[FloatText, IntText]] = {}
 
-        self.qubit_and_plot_ToggleButtons: Dict[str, ToggleButtons] = {}
-        self.manual_update_and_save_widgets: Dict[str, Union[Checkbox, Button]] = {}
-        self.qubit_plot_options_widgets: Dict[
-            str,
-            Union[
-                Image,
-                Button,
-                Text,
-                Dropdown,
-                FloatSlider,
-                IntSlider,
-                FloatSlider,
-                SelectMultiple,
-                Checkbox,
-            ],
-        ] = {}
-        self.qubit_params_widgets: Dict[
-            str, Union[IntSlider, FloatSlider, FloatRangeSlider]
-        ] = {}
+        # Display Elements
+        self.fig: Optional[Figure] = None
+        self.v_plot_output = ipywidgets.Output(
+            layout=ipywidgets.Layout(overflow="hidden")
+        )
+        self.v_tabs: v.Tabs = v.Tabs(children=[], background_color=NAV_COLOR, height=35)
+        self.v_main_tab_container = v.Container()
+
+        self.navbar, self.navbar_elements = gui_navbar.create_navbar()
+
+        self.v_save_btn = init_save_btn()
+        self.v_save_filename = init_filename_textfield()
+
+        self.dict_v_ranges: Dict[str, Dict[str, ui.ValidatedNumberField]] = {}
+        self.dict_v_noise_params: Dict[str, ui.ValidatedNumberField] = {}
+        self.dict_v_plot_options: Dict[str, Any] = {}
+        self.dict_v_qubit_params: Dict[str, Any] = {}
 
         # ------------------------------------------------------------------------------
 
-        self.initialize_qubit_and_plot_ToggleButtons()
-        self.initialize_manual_update_and_save_widgets_dict()
-        starting_qubit = self.qubit_and_plot_ToggleButtons[
-            "qubit_buttons"
-        ].get_interact_value()
-
-        self.set_qubit(starting_qubit)
-
-        self.current_plot_option_refresh = self.get_plot_option_refresh()
-
-        self.initialize_display()
+        starting_qubit = self.navbar_elements["CHOOSE_QUBIT"].v_model
+        self.set_qubit_and_init_qubit_widgets(starting_qubit)
 
-        self.initialize_observe()
-
-        self.current_plot_option_refresh(None)
+        self.init_display()
+        self.init_observe()
+        self.refresh_current_plot(change=None)
 
     # Initialization Methods -----------------------------------------------------------
-    def initialize_qubit_and_plot_ToggleButtons(self) -> None:
-        """Creates all the ToggleButtons that controls
-        which qubit or plot the user can choose from.
-        """
-        self.qubit_and_plot_ToggleButtons = {
-            "qubit_buttons": ToggleButtons(
-                options=gui_defaults.supported_qubits, description="Qubits:"
-            ),
-            "plot_buttons": ToggleButtons(
-                options=gui_defaults.plot_choices,
-                description="Plot:",
-                button_style="info",
-                value="Wavefunctions",
-            ),
-        }
-
-    def initialize_manual_update_and_save_widgets_dict(self) -> None:
-        """Creates all the widgets associated with manually updating and
-        saving plots.
-        """
-        self.manual_update_and_save_widgets = {
-            "manual_update_checkbox": Checkbox(
-                value=False,
-                description="Manual Update",
-                indent=False,
-                layout=Layout(width="125px"),
-            ),
-            "update_button": Button(
-                description="Update", disabled=True, layout=Layout(width="100px")
-            ),
-            "save_button": Button(icon="save", layout=Layout(width="35px")),
-            "filename_text": Text(
-                value=str(Path.cwd().joinpath("plot.pdf")),
-                description="",
-                layout=Layout(width="500px"),
-            ),
-        }
-
-    def initialize_noise_param_widgets(self) -> None:
-        """Creates all the widgets associated with coherence times plots"""
-        self.noise_param_widgets.clear()
-        noise_params = ["T", "omega_low", "omega_high", "t_exp"]
-        noise_channels = self.active_qubit.supported_noise_channels()
-
-        if "tphi_1_over_f_flux" in noise_channels:
-            noise_params.append("A_flux")
-        if "tphi_1_over_f_cc" in noise_channels:
-            noise_params.append("A_cc")
-        if "tphi_1_over_f_ng" in noise_channels:
-            noise_params.append("A_ng")
-        if (
-            "t1_charge_impedance" in noise_channels
-            or "t1_flux_bias_line" in noise_channels
-        ):
-            noise_params.append("R_0")
-        if "t1_flux_bias_line" in noise_channels:
-            noise_params.append("M")
-        if "t1_quasiparticle_tunneling" in noise_channels:
-            noise_params.append("x_qp")
-            noise_params.append("Delta")
-
-        for noise_param in noise_params:
-            self.noise_param_widgets[noise_param] = FloatText(
-                value=noise.NOISE_PARAMS[noise_param],
-                description=noise_param,
-                step=0.001,
-            )
+    def __repr__(self):
+        return ""
 
-    def set_qubit(self, qubit_name: str) -> None:
+    def set_qubit_and_init_qubit_widgets(self, qubit_name: str) -> None:
         """Sets up the chosen qubit to be the active qubit
         and updates the active defaults and widget dictionaries
         accordingly.
         """
         if qubit_name in gui_defaults.slow_qubits:
             scq.settings.PROGRESSBAR_DISABLED = False
         else:
             scq.settings.PROGRESSBAR_DISABLED = True
 
         self.active_defaults = gui_defaults.qubit_defaults[qubit_name]
-        self.initialize_qubit(qubit_name)
-        self.initialize_noise_param_widgets()
-        self.initialize_qubit_params_dicts()
-        self.initialize_qubit_plot_options_widgets_dict()
-        self.initialize_qubit_params_widgets_dict()
-        self.initialize_ranges_widgets_dict()
-
-    def initialize_qubit(self, qubit_name: str) -> None:
-        """Initializes self.active_qubit to the user's choice
-        using the chosen qubit's default parameters.
-        """
+
         QubitClass = getattr(scq, qubit_name)
         init_params = QubitClass.default_params()
 
-        if qubit_name == "ZeroPi" or qubit_name == "FullZeroPi":
+        if QubitClass in QUBITS_WITH_GRID_INIT:
             init_params["grid"] = Grid1d(-7 * np.pi, 7 * np.pi, 200)
         self.active_qubit = QubitClass(**init_params)
 
-    def initialize_qubit_params_dicts(self) -> None:
+        self.active_qubit.truncated_dim = self.active_qubit.hilbertdim()
+        self.set_qubit_params()
+
+        self.dict_v_noise_params = init_dict_v_noise_params(self.active_qubit)
+        self.dict_v_qubit_params = init_qubit_params_widgets_dict(
+            qubit=self.active_qubit,
+            qubit_params=self.qubit_params,
+            defaults=self.active_defaults,
+        )
+        self.dict_v_plot_options = init_dict_v_plot_options(
+            self.active_qubit,
+            self.active_defaults,
+            scan_params=list(self.qubit_scan_params.keys()),
+        )
+        self.dict_v_ranges = init_ranges_widgets_dict(
+            qubit=self.active_qubit,
+            dict_v_qubit_params=self.dict_v_qubit_params,
+            dict_v_plot_options=self.dict_v_plot_options,
+        )
+
+    def set_qubit_params(self) -> None:
         """
         Initializes qubit_params and qubit_scan_params.
         Note that qubit_scan_params will be used to create the
         scan parameter dropdown options.
         """
         self.qubit_params.clear()
         self.qubit_scan_params.clear()
@@ -261,420 +184,200 @@
 
         for param_name, param_val in self.qubit_params.items():
             if "cut" in param_name:
                 pass
             else:
                 self.qubit_scan_params[param_name] = param_val
 
-    def initialize_qubit_plot_options_widgets_dict(self) -> None:
-        """Creates all the widgets that will be used for general plotting options."""
-        std_layout = Layout(width="95%")
-
-        current_qubit = self.qubit_and_plot_ToggleButtons[
-            "qubit_buttons"
-        ].get_interact_value()
-        operator_dropdown_list = self.active_qubit.get_operator_names()
-        scan_dropdown_list = self.qubit_scan_params.keys()
-        noise_channel_list = self.active_qubit.supported_noise_channels()
-        file = open(self.active_qubit._image_filename, "rb")
-        image = file.read()
-
-        self.qubit_plot_options_widgets = {
-            "qubit_info_image_widget": Image(
-                value=image, format="jpg", layout=Layout(width="80%")
-            ),
-            "scan_dropdown": Dropdown(
-                options=scan_dropdown_list,
-                value=self.active_defaults["scan_param"],
-                description="Scan over",
-                layout=std_layout,
-            ),
-            "mode_dropdown": Dropdown(
-                options=gui_defaults.mode_dropdown_list,
-                description="Plot as:",
-                layout=std_layout,
-            ),
-            "operator_dropdown": Dropdown(
-                options=operator_dropdown_list,
-                value=self.active_defaults["operator"],
-                description="Operator",
-                layout=std_layout,
-            ),
-            "noise_channel_multi-select": SelectMultiple(
-                options=noise_channel_list,
-                value=noise_channel_list,
-                description="Noise Channels",
-                layout=std_layout,
-            ),
-            "highest_state_slider": IntSlider(
-                min=1,
-                max=10,
-                value=5,
-                continuous_update=False,
-                layout=std_layout,
-                description="Highest State",
-            ),
-            "show_numbers_checkbox": Checkbox(
-                value=False, description="Show values", indent=False
-            ),
-            "show3d_checkbox": Checkbox(
-                value=True, description="Show 3D", indent=False
-            ),
-            "subtract_ground_checkbox": Checkbox(
-                value=True,
-                description="Subtract E\u2080",
-                indent=False,
-            ),
-            "i_text": IntText(value=1, step=1),
-            "j_text": IntText(value=0, step=1),
-            "t1_checkbox": Checkbox(
-                value=False,
-                description="Effective T1",
-                indent=False,
-            ),
-            "t2_checkbox": Checkbox(
-                value=False,
-                description="Effective T2",
-                indent=False,
-            ),
-        }
-
-        if current_qubit in ["Transmon", "TunableTransmon", "Fluxonium"]:
-            self.qubit_plot_options_widgets["manual_scale_checkbox"] = Checkbox(
-                value=False, description="Manual Scaling", indent=False
-            )
-            self.qubit_plot_options_widgets["multi_state_selector"] = SelectMultiple(
-                options=range(0, 10),
-                value=[0, 1, 2, 3, 4],
-                description="States",
-                continuous_update=False,
-                layout=std_layout,
-            )
-            self.qubit_plot_options_widgets["wavefunction_scale_slider"] = FloatSlider(
-                min=0.1,
-                max=4,
-                value=self.active_defaults["scale"],
-                disabled=True,
-                description="\u03c8 ampl.",
-                continuous_update=False,
-                layout=std_layout,
-            )
-        else:
-            self.qubit_plot_options_widgets["wavefunction_state_slider"] = IntSlider(
-                min=0,
-                max=9,
-                value=5,
-                continuous_update=False,
-                layout=std_layout,
-                description="State No.",
-            )
-
-        if current_qubit in gui_defaults.paramvals_from_papers.keys():
-            common_params_dropdown_list = ["Manual"]
-            common_params_dropdown_list.extend(
-                gui_defaults.paramvals_from_papers[current_qubit].keys()
-            )
-            self.qubit_plot_options_widgets["common_params_dropdown"] = Dropdown(
-                options=common_params_dropdown_list, layout=std_layout
-            )
-        else:
-            self.qubit_plot_options_widgets["common_params_dropdown"] = Label(
-                value="None"
-            )
-
-        self.qubit_plot_options_widgets["link_HTML"] = HTML(value="")
-
-    def initialize_qubit_params_widgets_dict(self) -> None:
-        """Creates all the widgets associated with the parameters of the
-        chosen qubit.
-        """
-        self.qubit_params_widgets.clear()
-        std_layout = Layout(width="45%")
-
-        if isinstance(self.active_qubit, (scq.ZeroPi, scq.FullZeroPi)):
-            grid_min = self.active_qubit.grid.min_val
-            grid_max = self.active_qubit.grid.max_val
-            self.qubit_params_widgets["grid"] = FloatRangeSlider(
-                min=-12 * np.pi,
-                max=12 * np.pi,
-                value=[grid_min, grid_max],
-                step=0.05,
-                description="Grid range",
-                continuous_update=False,
-                layout=std_layout,
-            )
-
-        for param_name, param_val in self.qubit_params.items():
-            if isinstance(param_val, int):
-                kwargs = (
-                    self.active_defaults.get(param_name) or self.active_defaults["int"]
-                )
-                self.qubit_params_widgets[param_name] = IntSlider(
-                    **kwargs,
-                    value=param_val,
-                    description="{}:".format(param_name),
-                    continuous_update=False,
-                    layout=std_layout,
-                )
-            else:
-                kwargs = (
-                    self.active_defaults.get(param_name)
-                    or self.active_defaults["float"]
-                )
-                self.qubit_params_widgets[param_name] = FloatSlider(
-                    **kwargs,
-                    value=param_val,
-                    step=0.01,
-                    description="{}:".format(param_name),
-                    continuous_update=False,
-                    layout=std_layout,
-                )
-
-    def initialize_ranges_widgets_dict(self) -> None:
-        """Creates all the widgets associated with changing the ranges of
-        certain qubit plot options as well as all of the qubit's parameters.
-        """
-        self.ranges_widgets.clear()
-        range_text_layout = Layout(width="45%")
-        total_dict = {**self.qubit_plot_options_widgets, **self.qubit_params_widgets}
-
-        for widget_name, widget in total_dict.items():
-            if widget_name == "noise_channel_multi-select":
-                continue
-
-            widget_min_text = None
-            widget_max_text = None
-
-            if isinstance(widget, IntSlider):
-                widget_min_text = IntText(
-                    value=widget.min,
-                    description="min=",
-                    layout=range_text_layout,
-                )
-                widget_max_text = IntText(
-                    value=widget.max,
-                    description="max=",
-                    layout=range_text_layout,
-                )
-            elif isinstance(widget, (FloatSlider, FloatRangeSlider)):
-                widget_min_text = FloatText(
-                    value=widget.min,
-                    description="min=",
-                    step=0.01,
-                    layout=range_text_layout,
-                )
-                widget_max_text = FloatText(
-                    value=widget.max,
-                    description="max=",
-                    step=0.01,
-                    layout=range_text_layout,
-                )
-            elif isinstance(widget, SelectMultiple):
-                min_val = widget.options[0]
-                max_val = widget.options[-1]
-
-                widget_min_text = IntText(
-                    value=min_val,
-                    description="min=",
-                    layout=range_text_layout,
-                )
-                widget_max_text = IntText(
-                    value=max_val,
-                    description="max=",
-                    layout=range_text_layout,
-                )
-            else:
-                continue
-
-            self.ranges_widgets[widget_name] = {
-                "min": widget_min_text,
-                "max": widget_max_text,
-            }
-
-        if isinstance(
-            self.active_qubit,
-            (scq.Transmon, scq.TunableTransmon, scq.Fluxonium, scq.FluxQubit),
-        ):
-            widget_min_text = FloatText(
-                value=self.active_qubit._default_grid.min_val,
-                description="min=",
-                step=0.01,
-                layout=range_text_layout,
-            )
-            widget_max_text = FloatText(
-                value=self.active_qubit._default_grid.max_val,
-                description="max=",
-                step=0.01,
-                layout=range_text_layout,
-            )
-            self.ranges_widgets["phi"] = {
-                "min": widget_min_text,
-                "max": widget_max_text,
-            }
-        elif isinstance(self.active_qubit, scq.ZeroPi):
-            widget_min_text = FloatText(
-                value=self.active_qubit._default_grid.min_val,
-                description="min=",
-                step=0.01,
-                layout=range_text_layout,
-            )
-            widget_max_text = FloatText(
-                value=self.active_qubit._default_grid.max_val,
-                description="max=",
-                step=0.01,
-                layout=range_text_layout,
-            )
-            self.ranges_widgets["theta"] = {
-                "min": widget_min_text,
-                "max": widget_max_text,
-            }
-        elif isinstance(self.active_qubit, scq.Cos2PhiQubit):
-            default_grids = {
-                "phi": self.active_qubit._default_phi_grid,
-                "theta": self.active_qubit._default_theta_grid,
-                "zeta": self.active_qubit._default_zeta_grid,
-            }
-            for param, param_grid in default_grids.items():
-                widget_min_text = FloatText(
-                    value=param_grid.min_val,
-                    description="min=",
-                    step=0.01,
-                    layout=range_text_layout,
-                )
-                widget_max_text = FloatText(
-                    value=param_grid.max_val,
-                    description="max=",
-                    step=0.01,
-                    layout=range_text_layout,
-                )
-                self.ranges_widgets[param] = {
-                    "min": widget_min_text,
-                    "max": widget_max_text,
-                }
-
-    def initialize_tab_widget(self) -> None:
+    def init_tab_widget(self) -> None:
         """Creates each of the tabs in self.tab_widget"""
-        qubit_plot_tab = self.qubit_plot_layout()
-        param_ranges_tab = self.ranges_layout()
-        qubit_info_tab = self.qubit_info_layout()
-        common_qubit_params_tab = self.common_qubit_params_layout()
-        noise_param_tab = self.noise_params_layout()
-
-        tab_titles = [
-            "Main",
-            "Qubit info",
-            "Literature params",
-            "Param ranges",
-            "Noise Params",
-        ]
-        self.tab_widget.children = [
-            qubit_plot_tab,
-            qubit_info_tab,
-            common_qubit_params_tab,
-            param_ranges_tab,
-            noise_param_tab,
-        ]
 
-        for title_index in range(len(self.tab_widget.children)):
-            self.tab_widget.set_title(title_index, tab_titles[title_index])
+        self.v_main_tab_container = v.Container(
+            class_="d-flex d-row px-2 mx-1",
+            dense=True,
+            children=[self.main_tab_widgets()],
+        )
+        param_ranges_tab = v.Sheet(
+            class_="d-flex flex-column flex-wrap overflow-auto",
+            dense=True,
+            style_="max-height: 500px;",
+            children=self.param_ranges_tab_widgets(),
+        )
+        qubit_info_sheet = v.Sheet(children=[self.qubit_info_tab()])
+        literature_tab = v.Sheet(
+            class_="d-flex flex-column", children=self.literature_params_tab_widgets()
+        )
+        noise_param_tab = v.Sheet(
+            class_="d-flex flex-column flex-wrap overflow-auto",
+            children=[self.noise_params_tab_widgets()],
+        )
+
+        self.v_tabs.children = [
+            v.Tab(children=["Main"]),
+            v.TabItem(key="Main", children=[self.v_main_tab_container]),
+            v.Tab(children=["Qubit info"]),
+            v.TabItem(key="Qubit info", children=[qubit_info_sheet]),
+            v.Tab(children=["Literature params"]),
+            v.TabItem(key="Literature params", children=[literature_tab]),
+            v.Tab(children=["Param ranges"]),
+            v.TabItem(key="Param ranges", children=[param_ranges_tab]),
+            v.Tab(children=["Noise params"]),
+            v.TabItem(key="Noise params", children=[noise_param_tab]),
+        ]
+        self.v_tabs.v_model = self.v_tabs.v_model or "Main"
+        self.v_tabs.align_with_title = True
 
-    def initialize_display(self) -> None:
+    def init_display(self) -> None:
         """Creates the components of the GUI and displays all these components."""
-        qubit_and_plot_choice_display = self.qubit_and_plot_ToggleButtons_layout()
-        self.initialize_tab_widget()
-        manual_update_display = self.manual_update_and_save_layout()
+
+        self.init_tab_widget()
+
+        save_widget = flex_row([self.v_save_btn, self.v_save_filename], class_="p-0")
+        update_widget = flex_column(
+            [self.navbar_elements["AUTO_UPDATING"], self.navbar_elements["DO_UPDATE"]],
+            class_="px-0",
+            style_="transform: scale(0.9); width: 150px; margin-left: 50px; margin-right: 0px;",
+        )
 
         display(
-            qubit_and_plot_choice_display,
-            self.tab_widget,
-            manual_update_display,
-            self.plot_output,
+            v.Container(
+                id="outermost_cntnr",
+                class_="ml-0 pl-0 mr-0 pr-0",
+                children=[
+                    self.navbar_elements["HEADER"],
+                    v.Container(
+                        id="below_header_cntnr",
+                        class_="d-flex flex-row pl-0 pr-0 mt-0 pt-0 ml-0",
+                        children=[
+                            self.navbar,
+                            v.Container(
+                                id="below_tabs_header_cntnr",
+                                class_="d-flex flex-column align-center ml-0 px-0 mx-0 my-0 py-0",
+                                children=[
+                                    self.v_tabs,
+                                    v.Card(
+                                        id="update_and_display_card",
+                                        class_="d-flex flex-row p-0",
+                                        style_="margin-left: 24px; margin-top: 5px",
+                                        width="100%",
+                                        children=[
+                                            update_widget,
+                                            flex_column(
+                                                [self.v_plot_output],
+                                                class_="p-0 m-0",
+                                                id="matplotlib_cntnr",
+                                            ),
+                                        ],
+                                    ),
+                                    save_widget,
+                                ],
+                            ),
+                        ],
+                    ),
+                ],
+            )
         )
 
-    def initialize_observe(self) -> None:
+    def init_observe(self) -> None:
         """Links all the necessary widgets to their desired function."""
-        self.qubit_and_plot_ToggleButtons["qubit_buttons"].observe(
-            self.qubit_change, names="value"
-        )
-        self.qubit_and_plot_ToggleButtons["plot_buttons"].observe(
-            self.plot_option_layout_refresh, names="value"
-        )
-        self.manual_update_and_save_widgets["manual_update_checkbox"].observe(
-            self.manual_update_checkbox, names="value"
+        self.navbar_elements["CHOOSE_QUBIT"].observe(
+            self.change_active_qubit, names="v_model"
         )
-        self.manual_update_and_save_widgets["update_button"].on_click(
-            self.manual_update_button_onclick
+        self.navbar_elements["CHOOSE_PLOT"].observe(
+            self.change_plot_type, names="v_model"
         )
-        self.manual_update_and_save_widgets["save_button"].on_click(
-            self.save_button_clicked_action
+        self.navbar_elements["AUTO_UPDATING"].observe(
+            self.toggle_auto_updating, names="v_model"
         )
-        self.observe_coherence_elements()
-        self.observe_ranges()
-        self.observe_plot_elements()
-        self.observe_plot_refresh()
+        self.navbar_elements["DO_UPDATE"].on_event(
+            "click", self.manual_update_button_onclick
+        )
+        self.v_save_btn.on_event("click", self.save_button_clicked_action)
+
+        self.observe_all()
+
+    def observe_all(self):
+        """Switch on monitoring of all widgets in the GUI."""
+        self.observe_coherence_widgets()
+        self.observe_range_widgets()
+        self.observe_plot_option_widgets()
+        self.activate_auto_plot_refresh()
+
+    def unobserve_all(self):
+        """Switch off monitoring of all widgets in the GUI and stop automatic refreshing of the plot."""
+        self.deactivate_auto_plot_refresh()
+        self.unobserve_coherence_widgets()
+        self.unobserve_range_widgets()
+        self.unobserve_plot_options_widget()
 
     # Retrieval Methods------------------------------------------------------------------
     def get_current_values(self) -> Dict[str, Union[int, float]]:
         """Obtains the current values from each of the qubit parameter
         sliders.
 
         Returns
         -------
             Dictionary of the current value for each of the qubit's parameters
         """
         current_values_dict = {}
-        for param_name, widget in self.qubit_params_widgets.items():
-            current_values_dict[param_name] = widget.get_interact_value()
+        for param_name, widget in self.dict_v_qubit_params.items():
+            if not hasattr(widget, "valid_entry") or widget.is_entry_valid():
+                current_values_dict[param_name] = (
+                    widget.num_value if hasattr(widget, "num_value") else widget.v_model
+                )
         return current_values_dict
 
-    def get_plot_option_refresh(self) -> Callable[[Any], None]:
+    def refresh_current_plot(self, change=None) -> None:
         """Obtains the current plot option
 
         Returns
         -------
             Method pertaining to refreshing the current plot option.
         """
-        current_plot_option = self.qubit_and_plot_ToggleButtons[
-            "plot_buttons"
-        ].get_interact_value()
-
-        if current_plot_option == "Energy spectrum":
-            plot_option_refresh = self.evals_vs_paramvals_plot_refresh
-        elif current_plot_option == "Wavefunctions":
-            plot_option_refresh = self.wavefunctions_plot_refresh
-        elif current_plot_option == "Matrix element scan":
-            plot_option_refresh = self.matelem_vs_paramvals_plot_refresh
-        elif current_plot_option == "Matrix elements":
-            plot_option_refresh = self.matrixelements_plot_refresh
-        elif current_plot_option == "Coherence times":
-            plot_option_refresh = self.coherence_vs_paramvals_plot_refresh
+        current_plot_option = self.navbar_elements["CHOOSE_PLOT"].v_model
 
-        return plot_option_refresh
+        if current_plot_option == 0:
+            self.evals_vs_paramvals_plot_refresh()
+            return
+        if current_plot_option == 1:
+            self.wavefunctions_plot_refresh()
+            return
+        if current_plot_option == 2:
+            self.matrixelements_plot_refresh()
+            return
+        if current_plot_option == 3:
+            self.matelem_vs_paramvals_plot_refresh()
+            return
+        if current_plot_option == 4:
+            self.coherence_vs_paramvals_plot_refresh()
+            return
+
+        raise Exception("Internal GUI exception:", current_plot_option)
 
     def update_params(self):
         """Uses the current parameter values to set the parameters of the
         active qubit.
         """
         current_values = self.get_current_values()
 
-        if isinstance(self.active_qubit, (scq.ZeroPi, scq.FullZeroPi)):
+        if isinstance(self.active_qubit, QUBITS_WITH_GRID_INIT):
             del current_values["grid"]
-            grid_min, grid_max = self.qubit_params_widgets["grid"].get_interact_value()
+            grid_min, grid_max = self.dict_v_qubit_params["grid"].v_model
             current_values["grid_min_val"] = grid_min
             current_values["grid_max_val"] = grid_max
             current_values["grid_pt_count"] = self.active_qubit.grid.pt_count
 
         self.active_qubit.set_params(**current_values)
 
     def check_ranges(
         self,
         new_min: Union[int, float],
         new_max: Union[int, float],
         widget_name: str,
-        text_widget: Dict[str, Union[IntText, FloatText]],
+        text_widget: dict,
         changed_widget_key: str,
     ) -> Tuple[Union[int, float], Union[int, float]]:
         """Adjusts range values so that they make sense/are viable.
 
         Parameters
         ----------
         new_min:
@@ -691,41 +394,27 @@
             widget has been changed
 
         Returns
         -------
             A tuple containing the viable minimum and maximum values for the
             corresponding parameter/qubit plot option widget
         """
-        if new_min <= 0 or ("cut" in widget_name and new_min == 1):
-            if widget_name == "highest_state_slider":
-                new_min = 1
-            elif widget_name in ("phi", "theta", "zeta", "flux", "grid"):
-                pass
-            elif widget_name == "wavefunction_scale_slider":
-                new_min = text_widget["min"].step
-            elif widget_name in self.qubit_params_widgets.keys():
-                if "cut" in widget_name:
-                    new_min = 2
-                else:
-                    new_min = self.active_defaults[widget_name]["min"]
+        if new_max < new_min:
+            if changed_widget_key == "min":
+                new_min = new_max
             else:
-                new_min = 0
-        if new_max <= new_min:
-            if changed_widget_key == "min=":
-                new_min = new_max - text_widget["max"].step
-            else:
-                new_max = new_min + text_widget["min"].step
+                new_max = new_min
         return new_min, new_max
 
     def update_range_values(
         self,
         new_min: Union[int, float],
         new_max: Union[int, float],
         widget_name: str,
-        text_widget: Dict[str, Union[IntText, FloatText]],
+        text_widget: dict,
     ):
         """Adjusts the values of the IntText/FloatText widgets
 
         Parameters
         ----------
         new_min:
             The current value of the minimum IntText/FloatText
@@ -733,611 +422,535 @@
            The current value of the maximum IntText/FloatText
         widget_name:
             The name of the corresponding parameter/qubit plot option
         text_widget:
             A dictionary that contains the minimum and maximum
             IntText/FloatText widgets
         """
-        text_widget["min"].value = new_min
-        text_widget["max"].value = new_max
+        text_widget["min"].v_model = new_min
+        text_widget["max"].v_model = new_max
 
-        if widget_name in self.qubit_plot_options_widgets.keys():
-            widget = self.qubit_plot_options_widgets[widget_name]
-        elif widget_name in self.qubit_params_widgets.keys():
-            widget = self.qubit_params_widgets[widget_name]
+        if widget_name in self.dict_v_plot_options.keys():
+            widget = self.dict_v_plot_options[widget_name]
+        elif widget_name in self.dict_v_qubit_params.keys():
+            widget = self.dict_v_qubit_params[widget_name]
         else:
             widget = None
 
-        if isinstance(widget, SelectMultiple):
-            current_values = list(widget.value)
+        if isinstance(widget, v.Select) and widget.multiple:
+            current_values = list(widget.v_model)
             new_values = []
-            widget.options = range(new_min, new_max + 1)
+            widget.items = list(range(int(new_min), int(new_max + 1)))
             for value in current_values:
-                if value in widget.options:
+                if value in widget.items:
                     new_values.append(value)
-            if len(new_values) == 0:
-                new_values.append(widget.options[0])
-            widget.value = new_values
+            widget.v_model = new_values
         elif widget is None:
             pass
+        elif hasattr(widget, "v_min"):
+            widget.v_min = new_min
+            widget.v_max = new_max
         else:
             widget.min = new_min
             widget.max = new_max
 
     # Observe Methods-------------------------------------------------------------------
-    def observe_ranges(self) -> None:
-        for text_widgets in self.ranges_widgets.values():
-            text_widgets["min"].observe(self.ranges_update, names="value")
-            text_widgets["max"].observe(self.ranges_update, names="value")
-
-    def unobserve_ranges(self) -> None:
-        for text_widgets in self.ranges_widgets.values():
-            text_widgets["min"].unobserve(self.ranges_update, names="value")
-            text_widgets["max"].unobserve(self.ranges_update, names="value")
+    def observe_range_widgets(self) -> None:
+        for text_widgets in self.dict_v_ranges.values():
+            text_widgets["min"].observe(self.ranges_update, names="num_value")
+            text_widgets["max"].observe(self.ranges_update, names="num_value")
+
+    def unobserve_range_widgets(self) -> None:
+        for text_widgets in self.dict_v_ranges.values():
+            text_widgets["min"].unobserve(self.ranges_update, names="num_value")
+            text_widgets["max"].unobserve(self.ranges_update, names="num_value")
 
-    def observe_plot_refresh(self) -> None:
-        if self.manual_update_bool:
-            return
-        qubit_plot_options_blacklist = [
-            "qubit_info_image_widget",
-            "common_params_dropdown",
-            "link_HTML",
-        ]
+    def activate_auto_plot_refresh(self) -> None:
         total_dict = {
-            **self.qubit_params_widgets,
-            **self.qubit_plot_options_widgets,
-            **self.noise_param_widgets,
+            **self.dict_v_qubit_params,
+            **self.dict_v_plot_options,
+            **self.dict_v_noise_params,
         }
         for widget_name, widget in total_dict.items():
-            if widget_name not in qubit_plot_options_blacklist:
-                widget.observe(self.plot_refresh, names="value")
+            if widget_name not in self.no_plot_refresh_widgets:
+                widget.observe(self.plot_refresh, names="v_model")
 
-    def unobserve_plot_refresh(self) -> None:
-        if self.manual_update_bool:
-            return
-        qubit_plot_options_blacklist = [
-            "qubit_info_image_widget",
-            "common_params_dropdown",
-            "link_HTML",
-        ]
+    def deactivate_auto_plot_refresh(self) -> None:
         total_dict = {
-            **self.qubit_params_widgets,
-            **self.qubit_plot_options_widgets,
-            **self.noise_param_widgets,
+            **self.dict_v_qubit_params,
+            **self.dict_v_plot_options,
+            **self.dict_v_noise_params,
         }
         for widget_name, widget in total_dict.items():
-            if widget_name not in qubit_plot_options_blacklist:
-                widget.unobserve(self.plot_refresh, names="value")
+            if widget_name not in self.no_plot_refresh_widgets:
+                try:
+                    widget.unobserve(self.plot_refresh, names="v_model")
+                except ValueError:
+                    pass
 
-    def observe_plot_elements(self) -> None:
+    def observe_plot_option_widgets(self) -> None:
         if isinstance(
             self.active_qubit, (scq.Transmon, scq.TunableTransmon, scq.Fluxonium)
         ):
-            self.qubit_plot_options_widgets["manual_scale_checkbox"].observe(
-                self.manual_scale_tf, names="value"
+            self.dict_v_plot_options["manual_wf_scaling"].observe(
+                self.toggle_manual_wf_scaling, names="v_model"
             )
-        self.qubit_plot_options_widgets["scan_dropdown"].observe(
-            self.scan_dropdown_refresh, names="value"
+
+        self.dict_v_plot_options["scan_param"].observe(
+            self.set_new_scan_param, names="v_model"
         )
-        self.qubit_plot_options_widgets["common_params_dropdown"].observe(
-            self.common_params_dropdown_link_refresh, names="value"
+        self.dict_v_plot_options["literature_params"].observe(
+            self.set_literature_params_and_refresh_plot, names="v_model"
         )
-        self.qubit_plot_options_widgets["common_params_dropdown"].observe(
-            self.common_params_dropdown_params_refresh, names="value"
+
+        self.dict_v_plot_options["literature_params"].observe(
+            self.literature_url_refresh, names="v_model"
         )
-        self.qubit_plot_options_widgets["t1_checkbox"].observe(
-            self.plot_change_bool_update, names="value"
+        self.dict_v_plot_options["t1_checkbox"].observe(
+            self.clear_plot, names="v_model"
         )
-        self.qubit_plot_options_widgets["t2_checkbox"].observe(
-            self.plot_change_bool_update, names="value"
+
+        self.dict_v_plot_options["t2_checkbox"].observe(
+            self.clear_plot, names="v_model"
         )
-        self.qubit_plot_options_widgets["show3d_checkbox"].observe(
-            self.plot_change_bool_update, names="value"
+        self.dict_v_plot_options["show3d_matelem"].observe(
+            self.clear_plot, names="v_model"
         )
-        self.qubit_plot_options_widgets["noise_channel_multi-select"].observe(
-            self.plot_change_bool_update, names="value"
+        self.dict_v_plot_options["noise_channel_multiselect"].observe(
+            self.clear_plot, names="v_model"
         )
 
-        for widget_name, widget in self.qubit_params_widgets.items():
+        for widget_name, widget in self.dict_v_qubit_params.items():
             if "cut" in widget_name:
-                widget.observe(self.adjust_state_widgets, names="value")
-            widget.observe(self.common_params_dropdown_value_refresh, names="value")
+                widget.observe(self.adjust_state_widgets, names="v_model")
+            widget.observe(self.check_user_override_literature_params, names="v_model")
 
-    def unobserve_plot_elements(self) -> None:
+    def unobserve_plot_options_widget(self) -> None:
         if isinstance(
             self.active_qubit, (scq.Transmon, scq.TunableTransmon, scq.Fluxonium)
         ):
-            self.qubit_plot_options_widgets["manual_scale_checkbox"].unobserve(
-                self.manual_scale_tf, names="value"
+            self.dict_v_plot_options["manual_wf_scaling"].unobserve(
+                self.toggle_manual_wf_scaling, names="v_model"
             )
-        self.qubit_plot_options_widgets["scan_dropdown"].unobserve(
-            self.scan_dropdown_refresh, names="value"
+
+        self.dict_v_plot_options["scan_param"].unobserve(
+            self.set_new_scan_param, names="v_model"
         )
-        self.qubit_plot_options_widgets["common_params_dropdown"].unobserve(
-            self.common_params_dropdown_link_refresh, names="value"
+        self.dict_v_plot_options["literature_params"].unobserve(
+            self.literature_url_refresh, names="v_model"
         )
-        self.qubit_plot_options_widgets["common_params_dropdown"].unobserve(
-            self.common_params_dropdown_params_refresh, names="value"
+        self.dict_v_plot_options["literature_params"].unobserve(
+            self.set_literature_params_and_refresh_plot, names="v_model"
         )
-        self.qubit_plot_options_widgets["t1_checkbox"].unobserve(
-            self.plot_change_bool_update, names="value"
+        self.dict_v_plot_options["t1_checkbox"].unobserve(
+            self.clear_plot, names="v_model"
         )
-        self.qubit_plot_options_widgets["t2_checkbox"].unobserve(
-            self.plot_change_bool_update, names="value"
+        self.dict_v_plot_options["t2_checkbox"].unobserve(
+            self.clear_plot, names="v_model"
         )
-        self.qubit_plot_options_widgets["show3d_checkbox"].unobserve(
-            self.plot_change_bool_update, names="value"
+        self.dict_v_plot_options["show3d_matelem"].unobserve(
+            self.clear_plot, names="v_model"
         )
-        self.qubit_plot_options_widgets["noise_channel_multi-select"].unobserve(
-            self.plot_change_bool_update, names="value"
+        self.dict_v_plot_options["noise_channel_multiselect"].unobserve(
+            self.clear_plot, names="v_model"
         )
 
-        for widget_name, widget in self.qubit_params_widgets.items():
+        for widget_name, widget in self.dict_v_qubit_params.items():
             if "cut" in widget_name:
-                widget.unobserve(self.adjust_state_widgets, names="value")
-            widget.unobserve(self.common_params_dropdown_value_refresh, names="value")
+                widget.unobserve(self.adjust_state_widgets, names="v_model")
+            widget.unobserve(
+                self.check_user_override_literature_params, names="v_model"
+            )
 
-    def observe_coherence_elements(self) -> None:
-        self.qubit_plot_options_widgets["i_text"].observe(
-            self.coherence_text, names="value"
+    def observe_coherence_widgets(self) -> None:
+        self.dict_v_plot_options["i_text"].observe(
+            self.check_coherence_params_bounds, names="num_value"
         )
-        self.qubit_plot_options_widgets["j_text"].observe(
-            self.coherence_text, names="value"
+        self.dict_v_plot_options["j_text"].observe(
+            self.check_coherence_params_bounds, names="num_value"
         )
 
-        for widget in self.noise_param_widgets.values():
-            widget.observe(self.coherence_text, names="value")
+        for widget in self.dict_v_noise_params.values():
+            widget.observe(self.check_coherence_params_bounds, names="num_value")
 
-    def unobserve_coherence_elements(self) -> None:
-        self.qubit_plot_options_widgets["i_text"].unobserve(
-            self.coherence_text, names="value"
+    def unobserve_coherence_widgets(self) -> None:
+        self.dict_v_plot_options["i_text"].unobserve(
+            self.check_coherence_params_bounds, names="num_value"
         )
-        self.qubit_plot_options_widgets["j_text"].unobserve(
-            self.coherence_text, names="value"
+        self.dict_v_plot_options["j_text"].unobserve(
+            self.check_coherence_params_bounds, names="num_value"
         )
 
-        for widget in self.noise_param_widgets.values():
-            widget.unobserve(self.coherence_text, names="value")
+        for widget in self.dict_v_noise_params.values():
+            widget.unobserve(self.check_coherence_params_bounds, names="num_value")
 
     # Eventhandler Methods -------------------------------------------------------------
-    def qubit_change(self, change) -> None:
-        self.plot_change_bool = True
-        self.plot_output.clear_output()
+    def change_active_qubit(self, change) -> None:
+        self.clear_plot()
+        self.unobserve_all()
+
         new_qubit = change["new"]
-        self.unobserve_ranges()
-        self.unobserve_coherence_elements()
-        self.unobserve_plot_elements()
-        self.unobserve_plot_refresh()
-        self.manual_update_and_save_widgets["manual_update_checkbox"].unobserve(
-            self.manual_update_checkbox, names="value"
-        )
         if new_qubit in gui_defaults.slow_qubits:
-            self.manual_update_and_save_widgets["manual_update_checkbox"].value = True
-            self.manual_update_and_save_widgets["update_button"].disabled = False
-            self.manual_update_bool = True
+            self.navbar_elements["AUTO_UPDATING"].v_model = False
+            self.auto_updating_off()
         else:
-            self.manual_update_and_save_widgets["manual_update_checkbox"].value = False
-            self.manual_update_and_save_widgets["update_button"].disabled = True
-            self.manual_update_bool = False
-        self.manual_update_and_save_widgets["manual_update_checkbox"].observe(
-            self.manual_update_checkbox, names="value"
-        )
-        self.set_qubit(new_qubit)
-        self.initialize_tab_widget()
-        self.observe_ranges()
-        self.observe_coherence_elements()
-        self.observe_plot_elements()
-        self.observe_plot_refresh()
-        self.plot_refresh(None)
-
-    def scan_dropdown_refresh(self, change) -> None:
-        self.qubit_params_widgets[change.old].disabled = False
-        self.qubit_params_widgets[change.new].disabled = True
-
-    def plot_option_layout_refresh(self, change) -> None:
-        self.plot_change_bool = True
-        self.plot_output.clear_output()
-        self.unobserve_ranges()
-        self.unobserve_plot_elements()
-        self.unobserve_plot_refresh()
-        self.current_plot_option_refresh = self.get_plot_option_refresh()
-        new_plot_option = self.plot_option_layout()
-
-        self.tab_widget.children[0].children[0].children = tuple(
-            new_plot_option.children
-        )
-        self.observe_ranges()
-        self.observe_plot_elements()
-        self.observe_plot_refresh()
-        self.plot_refresh(None)
+            self.navbar_elements["AUTO_UPDATING"].v_model = True
+            self.auto_updating_on()
+
+        self.set_qubit_and_init_qubit_widgets(new_qubit)
+
+        self.init_tab_widget()
+        self.change_plot_options()
+        if self.auto_updating:
+            self.refresh_current_plot()
+        self.observe_all()
+
+    def set_new_scan_param(self, change) -> None:
+        new_scan_param = change["new"]
+        for param in self.dict_v_plot_options["scan_param"].items:
+            self.dict_v_qubit_params[param].disabled = False
+        self.dict_v_qubit_params[new_scan_param].disabled = True
+        self.plot_refresh(change=None)
+
+    def change_plot_type(self, change) -> None:
+        self.clear_plot()
+
+        self.unobserve_all()
+        self.change_plot_options()
+        self.observe_all()
 
-    def manual_scale_tf(self, change) -> None:
+        if self.auto_updating:
+            self.plot_refresh(change=None)
+
+    def toggle_manual_wf_scaling(self, change) -> None:
         if change["new"]:
-            self.qubit_plot_options_widgets[
-                "wavefunction_scale_slider"
-            ].disabled = False
+            self.dict_v_plot_options["wavefunction_scale_slider"].disabled = False
         else:
-            self.qubit_plot_options_widgets["wavefunction_scale_slider"].disabled = True
+            self.dict_v_plot_options["wavefunction_scale_slider"].disabled = True
+
+    def check_coherence_params_bounds(self, change) -> None:
+        if change["owner"].error:
+            return
 
-    def coherence_text(self, change) -> None:
-        self.unobserve_coherence_elements()
-        self.unobserve_plot_refresh()
-        isNoiseParamChange = None
-        widget_key = change["owner"].description
-
-        if widget_key in self.noise_param_widgets.keys():
-            isNoiseParamChange = True
-            widget = self.noise_param_widgets[widget_key]
+        self.unobserve_coherence_widgets()
+        self.deactivate_auto_plot_refresh()
+
+        widget_key = change["owner"].label
+
+        if widget_key in self.dict_v_noise_params:
+            widget = change["owner"]
+            if int(change["new"]) <= 0:
+                widget.v_model = widget.step
         else:
-            isNoiseParamChange = False
-            i_text_widget = self.qubit_plot_options_widgets["i_text"]
-            j_text_widget = self.qubit_plot_options_widgets["j_text"]
-
-        if change["new"] <= 0:
-            if isNoiseParamChange:
-                if widget_key in self.noise_param_widgets.keys():
-                    widget.value = widget.step
-            else:
-                if i_text_widget.value <= 0:
-                    i_text_widget.value = 0
-                if j_text_widget.value <= 0:
-                    j_text_widget.value = 0
-
-        if not isNoiseParamChange:
-            if i_text_widget.value == j_text_widget.value:
-                i_text_widget.value = j_text_widget.value + j_text_widget.step
-        self.observe_coherence_elements()
-        self.observe_plot_refresh()
-
-    def plot_change_bool_update(self, change):
-        self.plot_output.clear_output()
-        self.plot_change_bool = True
+            i_text_widget = self.dict_v_plot_options["i_text"]
+            j_text_widget = self.dict_v_plot_options["j_text"]
 
-    def manual_update_checkbox(self, change) -> None:
+            if i_text_widget.num_value <= 0:
+                i_text_widget.v_model = 0
+            if j_text_widget.num_value <= 0:
+                j_text_widget.v_model = 0
+            if i_text_widget.v_model == j_text_widget.v_model:
+                i_text_widget.v_model = j_text_widget.num_value + 1
+
+        self.observe_coherence_widgets()
+        self.activate_auto_plot_refresh()
+
+    def clear_plot(self, *args):
+        self.v_plot_output.clear_output()
+        self.plot_renewal_requested = True
+
+    def auto_updating_off(self):
+        self.navbar_elements["DO_UPDATE"].disabled = False
+        self.deactivate_auto_plot_refresh()
+
+    def auto_updating_on(self):
+        self.navbar_elements["DO_UPDATE"].disabled = True
+        self.activate_auto_plot_refresh()
+
+    @property
+    def auto_updating(self):
+        return self.navbar_elements["AUTO_UPDATING"].v_model
+
+    def toggle_auto_updating(self, change) -> None:
         if change["new"]:
-            self.plot_output.clear_output()
-            self.manual_update_and_save_widgets["update_button"].disabled = False
-            self.unobserve_plot_refresh()
-            self.manual_update_bool = True
+            self.auto_updating_on()
         else:
-            self.manual_update_and_save_widgets["update_button"].disabled = True
-            self.manual_update_bool = False
-            self.observe_plot_refresh()
-            if len(self.plot_output.outputs) == 0:
-                self.plot_change_bool = True
-            self.plot_refresh(None)
+            self.auto_updating_off()
 
-    def manual_update_button_onclick(self, change) -> None:
+    def manual_update_button_onclick(self, widget, event, data) -> None:
         self.update_params()
-        if len(self.plot_output.outputs) == 0:
-            self.plot_change_bool = True
-        self.current_plot_option_refresh(None)
-
-    def common_params_dropdown_value_refresh(self, change) -> None:
-        current_qubit = self.qubit_and_plot_ToggleButtons[
-            "qubit_buttons"
-        ].get_interact_value()
-        current_dropdown_value = self.qubit_plot_options_widgets[
-            "common_params_dropdown"
-        ].get_interact_value()
+        if len(self.v_plot_output.outputs) == 0:
+            self.plot_renewal_requested = True
+        self.refresh_current_plot(change=None)
+
+    def check_user_override_literature_params(self, change) -> None:
+        current_qubit = self.navbar_elements["CHOOSE_QUBIT"].v_model
+        current_dropdown_value = self.dict_v_plot_options["literature_params"].v_model
 
         if current_qubit not in gui_defaults.paramvals_from_papers.keys():
             return
-        if current_dropdown_value != "Manual":
+        if current_dropdown_value != "User specified":
             for param_name, param_val in gui_defaults.paramvals_from_papers[
                 current_qubit
             ][current_dropdown_value]["params"].items():
-                if (
-                    self.qubit_params_widgets[param_name].get_interact_value()
-                    != param_val
-                ):
-                    self.qubit_plot_options_widgets[
-                        "common_params_dropdown"
-                    ].value = "Manual"
-
-    def common_params_dropdown_params_refresh(self, change) -> None:
-        current_qubit = self.qubit_and_plot_ToggleButtons[
-            "qubit_buttons"
-        ].get_interact_value()
-        current_dropdown_value = self.qubit_plot_options_widgets[
-            "common_params_dropdown"
-        ].get_interact_value()
+                if self.dict_v_qubit_params[param_name].num_value != param_val:
+                    self.dict_v_plot_options[
+                        "literature_params"
+                    ].v_model = "User specified"
+                    return
+
+    def set_literature_params_and_refresh_plot(self, change) -> None:
+        current_qubit = self.navbar_elements["CHOOSE_QUBIT"].v_model
+        current_dropdown_value = self.dict_v_plot_options["literature_params"].v_model
 
-        if current_dropdown_value == "Manual":
+        if current_dropdown_value == "User specified":
             return
-        self.unobserve_ranges()
-        self.unobserve_plot_refresh()
-        self.unobserve_plot_elements()
+
+        self.unobserve_all()
+        self.literature_url_refresh(None)
 
         params = gui_defaults.paramvals_from_papers[current_qubit][
             current_dropdown_value
         ]["params"]
         for param_name, param_val in params.items():
-            param_max = self.ranges_widgets[param_name]["max"].get_interact_value()
-            param_min = self.ranges_widgets[param_name]["min"].get_interact_value()
+            param_max = self.dict_v_ranges[param_name]["max"].v_model
+            param_min = self.dict_v_ranges[param_name]["min"].v_model
 
             if param_val < param_min:
-                self.ranges_widgets[param_name]["min"].value = self.active_defaults[
+                self.dict_v_ranges[param_name]["min"].v_model = self.active_defaults[
                     param_name
                 ]["min"]
-                self.qubit_params_widgets[param_name].min = self.active_defaults[
+                self.dict_v_qubit_params[param_name].v_min = self.active_defaults[
                     param_name
                 ]["min"]
             if param_val > param_max:
-                self.ranges_widgets[param_name]["max"].value = (
+                self.dict_v_ranges[param_name]["max"].v_model = (
+                    np.ceil(param_val / 10) * 10
+                )
+                self.dict_v_qubit_params[param_name].v_max = (
                     np.ceil(param_val / 10) * 10
                 )
-                self.qubit_params_widgets[param_name].max = np.ceil(param_val / 10) * 10
 
-            self.qubit_params_widgets[param_name].value = param_val
-        self.observe_ranges()
-        self.observe_plot_refresh()
-        self.observe_plot_elements()
-        self.plot_refresh(None)
-
-    def adjust_state_widgets(self, change) -> None:
-        self.unobserve_ranges()
-        self.unobserve_plot_refresh()
+            self.dict_v_qubit_params[param_name].v_model = param_val
+
+        self.observe_all()
+        self.plot_refresh(change=None)
+
+    def adjust_state_widgets(self, *args) -> None:
+        self.unobserve_all()
         self.update_params()
         hilbertdim = self.active_qubit.hilbertdim()
-        wavefunction_state_slider_text = self.ranges_widgets["highest_state_slider"]
+        wavefunction_state_slider_text = self.dict_v_ranges["highest_state"]
 
-        if wavefunction_state_slider_text["max"].get_interact_value() >= hilbertdim - 1:
-            new_min = wavefunction_state_slider_text["min"].get_interact_value()
-            new_max = hilbertdim - 2
+        if wavefunction_state_slider_text["max"].num_value >= hilbertdim - 1:
+            new_max = max(hilbertdim - 2, 0)
+            new_min = wavefunction_state_slider_text["min"].num_value
             new_min, new_max = self.check_ranges(
                 new_min,
                 new_max,
-                "highest_state_slider",
+                "highest_state",
                 wavefunction_state_slider_text,
-                "min=",
+                "min",
             )
             self.update_range_values(
-                new_min, new_max, "highest_state_slider", wavefunction_state_slider_text
+                new_min, new_max, "highest_state", wavefunction_state_slider_text
             )
 
         if isinstance(
             self.active_qubit, (scq.Transmon, scq.TunableTransmon, scq.Fluxonium)
         ):
-            multi_state_selector_text = self.ranges_widgets["multi_state_selector"]
-
-            if multi_state_selector_text["max"].get_interact_value() >= hilbertdim - 2:
-                new_min = multi_state_selector_text["min"].get_interact_value()
+            multi_state_selector_text = self.dict_v_ranges["multi_state_selector"]
+            if multi_state_selector_text["max"].num_value >= hilbertdim - 2:
+                new_min = multi_state_selector_text["min"].num_value
                 new_max = hilbertdim - 3
                 new_min, new_max = self.check_ranges(
                     new_min,
                     new_max,
                     "multi_state_selector",
                     multi_state_selector_text,
-                    "min=",
+                    "min",
                 )
                 self.update_range_values(
                     new_min, new_max, "multi_state_selector", multi_state_selector_text
                 )
         else:
-            wavefunction_state_slider_text = self.ranges_widgets[
+            wavefunction_state_slider_text = self.dict_v_ranges[
                 "wavefunction_state_slider"
             ]
 
-            if (
-                wavefunction_state_slider_text["max"].get_interact_value()
-                >= hilbertdim - 2
-            ):
-                new_min = wavefunction_state_slider_text["min"].get_interact_value()
+            if wavefunction_state_slider_text["max"].num_value >= hilbertdim - 2:
+                new_min = wavefunction_state_slider_text["min"].num_value
                 new_max = hilbertdim - 3
                 new_min, new_max = self.check_ranges(
                     new_min,
                     new_max,
                     "wavefunction_state_slider",
                     wavefunction_state_slider_text,
-                    "min=",
+                    "min",
                 )
                 self.update_range_values(
                     new_min,
                     new_max,
                     "wavefunction_state_slider",
                     wavefunction_state_slider_text,
                 )
-        self.observe_ranges()
-        self.observe_plot_refresh()
+        self.observe_all()
 
     def ranges_update(self, change) -> None:
-        self.unobserve_ranges()
-        self.unobserve_plot_refresh()
-        for widget_name, text_widgets in self.ranges_widgets.items():
-            new_min = text_widgets["min"].get_interact_value()
-            new_max = text_widgets["max"].get_interact_value()
-            changed_widget_key = change["owner"].description
+        self.unobserve_all()
+        for widget_name, text_widgets in self.dict_v_ranges.items():
+            new_min = text_widgets["min"].num_value
+            new_max = text_widgets["max"].num_value
+            changed_widget_key = change["owner"].label
 
             new_min, new_max = self.check_ranges(
                 new_min, new_max, widget_name, text_widgets, changed_widget_key
             )
 
             self.update_range_values(new_min, new_max, widget_name, text_widgets)
-        self.observe_ranges()
-        self.observe_plot_refresh()
-        self.adjust_state_widgets(None)
-        self.plot_refresh(None)
 
-    def save_button_clicked_action(self, change) -> None:
-        self.fig.savefig(self.manual_update_and_save_widgets["filename_text"].value)
+        for widget in self.dict_v_qubit_params.values():
+            widget.update_slider()
 
-    def plot_refresh(self, change):
+        self.observe_all()
+        self.adjust_state_widgets()
+        self.plot_refresh(change=None)
+
+    def save_button_clicked_action(self, widget, event, data) -> None:
+        self.fig.savefig(self.v_save_filename.v_model)
+
+    def plot_refresh(self, change, *args):
         self.update_params()
 
-        if not self.manual_update_bool:
-            self.current_plot_option_refresh(None)
+        if self.auto_updating:
+            self.refresh_current_plot(change=None)
 
-    def common_params_dropdown_link_refresh(self, change) -> None:
-        current_qubit = self.qubit_and_plot_ToggleButtons[
-            "qubit_buttons"
-        ].get_interact_value()
-        current_dropdown_value = self.qubit_plot_options_widgets[
-            "common_params_dropdown"
-        ].get_interact_value()
+    def literature_url_refresh(self, change) -> None:
+        current_qubit = self.navbar_elements["CHOOSE_QUBIT"].v_model
+        current_dropdown_value = self.dict_v_plot_options["literature_params"].v_model
 
-        if current_dropdown_value == "Manual":
-            self.qubit_plot_options_widgets["link_HTML"].value = ""
+        if current_dropdown_value == "User specified":
+            self.dict_v_plot_options["link_HTML"].children = [""]
         else:
             link = gui_defaults.paramvals_from_papers[current_qubit][
                 current_dropdown_value
             ]["link"]
-            self.qubit_plot_options_widgets["link_HTML"].value = (
-                "<a href=" + link + " target='_blank'>" + link + "</a>"
-            )
+            self.dict_v_plot_options["link_HTML"].tag = "a"
+            self.dict_v_plot_options["link_HTML"].attributes = {
+                "href": link,
+                "target": "_blank",
+            }
+            self.dict_v_plot_options["link_HTML"].children = [link]
 
-    def evals_vs_paramvals_plot_refresh(self, change) -> None:
-        scan_dropdown_value = self.qubit_plot_options_widgets[
-            "scan_dropdown"
-        ].get_interact_value()
-        scan_slider = self.qubit_params_widgets[scan_dropdown_value]
+    def evals_vs_paramvals_plot_refresh(self) -> None:
+        scan_dropdown_value = self.dict_v_plot_options["scan_param"].v_model
+        scan_slider = self.dict_v_qubit_params[scan_dropdown_value]
 
         value_dict = {
             "scan_value": scan_dropdown_value,
-            "scan_range": (scan_slider.min, scan_slider.max),
-            "subtract_ground_tf": self.qubit_plot_options_widgets[
-                "subtract_ground_checkbox"
-            ].get_interact_value(),
-            "eigenvalue_state_value": self.qubit_plot_options_widgets[
-                "highest_state_slider"
-            ].get_interact_value(),
+            "scan_range": (scan_slider.v_min, scan_slider.v_max),
+            "subtract_ground_tf": self.dict_v_plot_options["subtract_ground"].v_model,
+            "eigenvalue_state_value": self.dict_v_plot_options["highest_state"].v_model,
         }
 
         self.evals_vs_paramvals_plot(**value_dict)
 
     @matplotlib.rc_context(matplotlib_settings)
-    def wavefunctions_plot_refresh(self, change) -> None:
+    def wavefunctions_plot_refresh(self) -> None:
         value_dict = {
-            "mode_value": self.qubit_plot_options_widgets[
-                "mode_dropdown"
-            ].get_interact_value(),
+            "mode_value": gui_defaults.mode_dropdown_dict[
+                self.dict_v_plot_options["amplitude_mode"].v_model
+            ],
         }
 
-        if isinstance(self.active_qubit, scq.FullZeroPi):
+        if isinstance(self.active_qubit, QUBITS_WITHOUT_WAVEFUNCTION_PLOT):
             return
-        elif isinstance(
-            self.active_qubit, (scq.FluxQubit, scq.ZeroPi, scq.Cos2PhiQubit)
-        ):
+        # Remainder of block only for qubits that support wavefunction plots
+        elif isinstance(self.active_qubit, QUBITS_WITH_2D_WAVEFUNCTION_PLOT):
             value_dict["scale_value"] = None
-            value_dict["eigenvalue_states"] = self.qubit_plot_options_widgets[
+            value_dict["eigenvalue_states"] = self.dict_v_plot_options[
                 "wavefunction_state_slider"
-            ].get_interact_value()
-        else:
-            manual_scale_tf_value = self.qubit_plot_options_widgets[
-                "manual_scale_checkbox"
-            ].get_interact_value()
+            ].v_model
+        else:  # qubit with 1d wavefunction
+            manual_scale_tf_value = self.dict_v_plot_options[
+                "manual_wf_scaling"
+            ].v_model
 
             if manual_scale_tf_value:
-                value_dict["scale_value"] = self.qubit_plot_options_widgets[
+                value_dict["scale_value"] = self.dict_v_plot_options[
                     "wavefunction_scale_slider"
-                ].get_interact_value()
+                ].v_model
             else:
                 value_dict["scale_value"] = None
-            value_dict["eigenvalue_states"] = self.qubit_plot_options_widgets[
+            value_dict["eigenvalue_states"] = self.dict_v_plot_options[
                 "multi_state_selector"
-            ].get_interact_value()
+            ].v_model
 
-        if isinstance(
-            self.active_qubit,
-            (scq.Transmon, scq.TunableTransmon, scq.Fluxonium, scq.FluxQubit),
-        ):
+        if isinstance(self.active_qubit, QUBITS_WITH_PHI_GRID):
             value_dict["phi_grid"] = Grid1d(
-                min_val=self.ranges_widgets["phi"]["min"].get_interact_value(),
-                max_val=self.ranges_widgets["phi"]["max"].get_interact_value(),
+                min_val=self.dict_v_ranges["phi"]["min"].num_value,
+                max_val=self.dict_v_ranges["phi"]["max"].num_value,
                 pt_count=self.active_qubit._default_grid.pt_count,
             )
-        elif isinstance(self.active_qubit, scq.ZeroPi):
+        if isinstance(self.active_qubit, QUBITS_WITH_THETA_GRID):
             value_dict["theta_grid"] = Grid1d(
-                min_val=self.ranges_widgets["theta"]["min"].get_interact_value(),
-                max_val=self.ranges_widgets["theta"]["max"].get_interact_value(),
+                min_val=self.dict_v_ranges["theta"]["min"].num_value,
+                max_val=self.dict_v_ranges["theta"]["max"].num_value,
                 pt_count=self.active_qubit._default_grid.pt_count,
             )
-        elif isinstance(self.active_qubit, scq.Cos2PhiQubit):
-            value_dict["phi_grid"] = Grid1d(
-                min_val=self.ranges_widgets["phi"]["min"].get_interact_value(),
-                max_val=self.ranges_widgets["phi"]["max"].get_interact_value(),
-                pt_count=self.active_qubit._default_phi_grid.pt_count,
-            )
-            value_dict["theta_grid"] = Grid1d(
-                min_val=self.ranges_widgets["theta"]["min"].get_interact_value(),
-                max_val=self.ranges_widgets["theta"]["max"].get_interact_value(),
-                pt_count=self.active_qubit._default_theta_grid.pt_count,
-            )
-
         self.wavefunctions_plot(**value_dict)
 
-    def matelem_vs_paramvals_plot_refresh(self, change) -> None:
-        scan_dropdown_value = self.qubit_plot_options_widgets[
-            "scan_dropdown"
-        ].get_interact_value()
-        scan_slider = self.qubit_params_widgets[scan_dropdown_value]
+    def matelem_vs_paramvals_plot_refresh(self) -> None:
+        scan_dropdown_value = self.dict_v_plot_options["scan_param"].v_model
+        scan_slider = self.dict_v_qubit_params[scan_dropdown_value]
 
         value_dict = {
             "scan_value": scan_dropdown_value,
-            "scan_range": (scan_slider.min, scan_slider.max),
-            "operator_value": self.qubit_plot_options_widgets[
-                "operator_dropdown"
-            ].get_interact_value(),
-            "matrix_element_state_value": self.qubit_plot_options_widgets[
-                "highest_state_slider"
-            ].get_interact_value(),
-            "mode_value": self.qubit_plot_options_widgets[
-                "mode_dropdown"
-            ].get_interact_value(),
+            "scan_range": (scan_slider.v_min, scan_slider.v_max),
+            "operator_value": self.dict_v_plot_options["operator_choice"].v_model,
+            "matrix_element_state_value": self.dict_v_plot_options[
+                "highest_state"
+            ].v_model,
+            "mode_value": gui_defaults.mode_dropdown_dict[
+                self.dict_v_plot_options["amplitude_mode"].v_model
+            ],
         }
 
         self.matelem_vs_paramvals_plot(**value_dict)
 
-    def matrixelements_plot_refresh(self, change) -> None:
+    def matrixelements_plot_refresh(self) -> None:
         value_dict = {
-            "operator_value": self.qubit_plot_options_widgets[
-                "operator_dropdown"
-            ].get_interact_value(),
-            "eigenvalue_state_value": self.qubit_plot_options_widgets[
-                "highest_state_slider"
-            ].get_interact_value(),
-            "mode_value": self.qubit_plot_options_widgets[
-                "mode_dropdown"
-            ].get_interact_value(),
-            "show_numbers_tf": self.qubit_plot_options_widgets[
-                "show_numbers_checkbox"
-            ].get_interact_value(),
-            "show3d_tf": self.qubit_plot_options_widgets[
-                "show3d_checkbox"
-            ].get_interact_value(),
+            "operator_value": self.dict_v_plot_options["operator_choice"].v_model,
+            "eigenvalue_state_value": self.dict_v_plot_options["highest_state"].v_model,
+            "mode_value": gui_defaults.mode_dropdown_dict[
+                self.dict_v_plot_options["amplitude_mode"].v_model
+            ],
+            "show_numbers_tf": self.dict_v_plot_options["show_matelem_numbers"].v_model,
+            "show3d_tf": self.dict_v_plot_options["show3d_matelem"].v_model,
         }
-
         self.matrixelements_plot(**value_dict)
 
-    def coherence_vs_paramvals_plot_refresh(self, change) -> None:
-        t1_effective_tf = self.qubit_plot_options_widgets[
-            "t1_checkbox"
-        ].get_interact_value()
-        t2_effective_tf = self.qubit_plot_options_widgets[
-            "t2_checkbox"
-        ].get_interact_value()
-        scan_dropdown_value = self.qubit_plot_options_widgets[
-            "scan_dropdown"
-        ].get_interact_value()
-        scan_slider = self.qubit_params_widgets[scan_dropdown_value]
+    def coherence_vs_paramvals_plot_refresh(self) -> None:
+        t1_effective_tf = self.dict_v_plot_options["t1_checkbox"].v_model
+        t2_effective_tf = self.dict_v_plot_options["t2_checkbox"].v_model
+        scan_dropdown_value = self.dict_v_plot_options["scan_param"].v_model
+        scan_slider = self.dict_v_qubit_params[scan_dropdown_value]
         noise_channel_options = list(
-            self.qubit_plot_options_widgets[
-                "noise_channel_multi-select"
-            ].get_interact_value()
+            self.dict_v_plot_options["noise_channel_multiselect"].v_model
         )
         common_noise_options = {
-            "i": self.qubit_plot_options_widgets["i_text"].get_interact_value(),
-            "j": self.qubit_plot_options_widgets["j_text"].get_interact_value(),
-            "T": self.noise_param_widgets["T"].get_interact_value(),
+            "i": self.dict_v_plot_options["i_text"].num_value,
+            "j": self.dict_v_plot_options["j_text"].num_value,
+            "T": self.dict_v_noise_params["T"].num_value,
         }
         noise_params_dict = {}
 
-        for noise_param in self.noise_param_widgets.keys():
+        for noise_param in self.dict_v_noise_params.keys():
             if noise_param != "T":
-                param_val = self.noise_param_widgets[noise_param].get_interact_value()
+                param_val = self.dict_v_noise_params[noise_param].num_value
                 noise_params_dict[noise_param] = param_val
 
         noise_channels = {"t1_eff": [], "t2_eff": [], "coherence_times": []}
         for noise_channel in noise_channel_options:
             if "tphi_1_over_f" in noise_channel:
                 tphi_dict = {
                     "omega_low": noise_params_dict["omega_low"],
@@ -1409,381 +1022,290 @@
                 noise_channels["t2_eff"].append(noise_channel)
                 noise_channels["coherence_times"].append(noise_channel)
 
         value_dict = {
             "t1_effective_tf": t1_effective_tf,
             "t2_effective_tf": t2_effective_tf,
             "scan_value": scan_dropdown_value,
-            "scan_range": (scan_slider.min, scan_slider.max),
+            "scan_range": (scan_slider.v_min, scan_slider.v_max),
             "noise_channels": noise_channels,
             "common_noise_options": common_noise_options,
         }
 
         self.coherence_vs_paramvals_plot(**value_dict)
 
     # Layout Methods ------------------------------------------------------------------
-    def qubit_and_plot_ToggleButtons_layout(self) -> VBox:
-        qubit_choice_hbox = HBox([self.qubit_and_plot_ToggleButtons["qubit_buttons"]])
-        plot_choice_hbox = HBox([self.qubit_and_plot_ToggleButtons["plot_buttons"]])
-
-        qubit_and_plot_choice_vbox = VBox([qubit_choice_hbox, plot_choice_hbox])
-
-        return qubit_and_plot_choice_vbox
 
-    def manual_update_and_save_layout(self) -> HBox:
-        manual_update_HBox = HBox(
-            [
-                self.manual_update_and_save_widgets["manual_update_checkbox"],
-                self.manual_update_and_save_widgets["update_button"],
-            ],
-            layout=Layout(justify_content="flex-start"),
-        )
-
-        save_HBox = HBox(
-            [
-                self.manual_update_and_save_widgets["save_button"],
-                self.manual_update_and_save_widgets["filename_text"],
-            ],
-            layout=Layout(justify_content="flex-end"),
-        )
+    def param_ranges_tab_widgets(self) -> list:
+        ranges_widgets = []
 
-        manual_update_and_save_HBox = HBox(
-            [manual_update_HBox, save_HBox],
-            layout=Layout(width="95%", justify_content="space-between"),
-        )
-
-        return manual_update_and_save_HBox
-
-    def ranges_layout(self) -> HBox:
-        range_hbox_layout = Layout(width="50%", justify_content="flex-end")
-        grid_hbox_layout = Layout(
-            display="flex", flex_flow="row wrap", object_fit="contain", width="100%"
-        )
-        ranges_grid_hbox = HBox(layout=grid_hbox_layout)
-
-        for widget_name, text_widgets in self.ranges_widgets.items():
-            if widget_name == "highest_state_slider":
-                widget_name = "Highest State"
+        for widget_name, text_widgets in self.dict_v_ranges.items():
+            if widget_name == "highest_state":
+                widget_name = "Max level"
             elif widget_name == "multi_state_selector":
                 widget_name = "States"
             elif widget_name == "wavefunction_state_slider":
-                widget_name = "State No."
+                widget_name = "State no."
             elif widget_name == "wavefunction_scale_slider":
                 widget_name = "Scale"
             elif widget_name == "wavefunction_domain_slider":
                 widget_name = "Wavefunction"
 
-            range_hbox = HBox(layout=range_hbox_layout)
-            widget_label = Label(
-                value=widget_name + ":", layout=Layout(justify_content="flex-end")
-            )
-            range_hbox.children += (
-                widget_label,
-                HBox(
-                    [text_widgets["min"], text_widgets["max"]],
-                    layout=Layout(width="80%"),
-                ),
-            )
-
-            ranges_grid_hbox.children += (range_hbox,)
-
-        return ranges_grid_hbox
-
-    def qubit_plot_layout(self) -> HBox:
-        plot_option_vbox = self.plot_option_layout()
-        qubit_params_grid = self.qubit_params_grid_layout()
+            ranges_widgets += [
+                v.Container(
+                    class_="d-flex flex-row align-center",
+                    style_="max-width: 290px; transform: scale(0.9)",
+                    dense=True,
+                    children=[
+                        v.Text(class_="pr-3", children=[widget_name]),
+                        text_widgets["min"],
+                        text_widgets["max"],
+                    ],
+                )
+            ]
+        return ranges_widgets
 
-        qubit_plot_layout = HBox([plot_option_vbox, qubit_params_grid])
+    def main_tab_widgets(self) -> v.Container:
+        self.plot_options_dict = self.plot_options_widgets()
+        qubit_params_grid = self.qubit_params_widgets()
+
+        main_tab = v.Container(
+            id="main_tab_cntnr",
+            class_="d-flex flex-row mx-0 px-0",
+            width="100%",
+            children=[
+                v.Container(
+                    id="plot_options_cntnr",
+                    class_="d-flex align-start flex-column pb-0",
+                    style_="width: 48%; transform: scale(0.9)",
+                    children=self.plot_options_dict[0],
+                ),
+                v.Divider(vertical=True),
+                v.Container(
+                    id="qubit_params_cntnr",
+                    style_="width: 100%; max-height: 350px; transform: scale(0.9)",
+                    class_="d-flex align-start flex-column flex-wrap flex-align-content-start overflow-auto mx-1 px-2",
+                    children=qubit_params_grid,
+                ),
+            ],
+        )
+        return main_tab
 
-        return qubit_plot_layout
+    def change_plot_options(self):
+        current_plot_option = self.navbar_elements["CHOOSE_PLOT"].v_model
+        self.v_main_tab_container.children[0].children[
+            0
+        ].children = self.plot_options_dict[current_plot_option]
+
+        self.dict_v_plot_options["amplitude_mode"].v_model = (
+            "Re(·)" if current_plot_option < 2 else "|·|"
+        )
+        if current_plot_option in gui_defaults.gui_sweep_plots:
+            self.dict_v_qubit_params[
+                self.dict_v_plot_options["scan_param"].v_model
+            ].disabled = True
+        else:
+            self.dict_v_qubit_params[
+                self.dict_v_plot_options["scan_param"].v_model
+            ].disabled = False
 
-    def qubit_info_layout(self) -> Box:
-        qubit_info_box = Box(layout=Layout(justify_content="center"))
-        qubit_info_box.children = [
-            self.qubit_plot_options_widgets["qubit_info_image_widget"]
-        ]
+    def qubit_info_tab(self) -> v.Container:
+        qubit_info_box = v.Container(
+            class_="py-5",
+            style_="transform: scale(0.9)",
+            children=[self.dict_v_plot_options["info_panel"]],
+        )
 
         return qubit_info_box
 
-    def common_qubit_params_layout(self) -> HBox:
-        dropdown_box = Box(
-            [self.qubit_plot_options_widgets["common_params_dropdown"]],
-            layout=Layout(width="50%"),
-        )
-        link_box = Box(
-            [self.qubit_plot_options_widgets["link_HTML"]],
-            layout=Layout(display="flex", width="50%"),
-        )
-        common_qubit_params_HBox = HBox(
-            [dropdown_box, link_box], layout=Layout(width="100%")
-        )
-        return common_qubit_params_HBox
-
-    def noise_params_layout(self) -> HBox:
-        HBox_layout = Layout(display="flex", object_fit="contain", width="100%")
-        noise_params_grid = HBox(layout=HBox_layout)
-
-        params_size = len(self.noise_param_widgets)
-        if params_size > 6:
-            left_right_HBox_layout = Layout(
-                display="flex",
-                flex_flow="column nowrap",
-                object_fit="contain",
-                width="50%",
-            )
-            left_HBox = HBox(layout=left_right_HBox_layout)
-            right_HBox = HBox(layout=left_right_HBox_layout)
-
-            counter = 1
-            for noise_param_widget in self.noise_param_widgets.values():
-                noise_param_widget.layout.width = "50%"
-                if params_size % 2 == 0:
-                    if counter <= params_size / 2:
-                        left_HBox.children += (noise_param_widget,)
-                    else:
-                        right_HBox.children += (noise_param_widget,)
-                else:
-                    if counter <= params_size / 2 + 1:
-                        left_HBox.children += (noise_param_widget,)
-                    else:
-                        right_HBox.children += (noise_param_widget,)
-                counter += 1
-
-            noise_params_grid.children += (
-                left_HBox,
-                right_HBox,
-            )
-        else:
-            noise_params_grid.layout.flex_flow = "column nowrap"
-            noise_params_grid.children = list(self.noise_param_widgets.values())
+    def literature_params_tab_widgets(self) -> list:
+        return [
+            self.dict_v_plot_options["literature_params"],
+            self.dict_v_plot_options["link_HTML"],
+        ]
 
+    def noise_params_tab_widgets(self) -> v.Container:
+        noise_params_grid = v.Container(
+            class_="d-flex flex-column flex-wrap py-3",
+            children=[],
+            style_="max-height: 400px; transform: scale(0.9)",
+        )
+        noise_params_grid.children = list(self.dict_v_noise_params.values())
         return noise_params_grid
 
-    def plot_option_layout(self) -> VBox:
-        current_plot_option = self.qubit_and_plot_ToggleButtons[
-            "plot_buttons"
-        ].get_interact_value()
-        VBox_layout = Layout(width="35%")
-        plot_option_vbox = VBox(layout=VBox_layout)
-
-        if current_plot_option == "Energy spectrum":
-            plot_option_vbox.children += self.energy_scan_layout()
-        elif current_plot_option == "Wavefunctions":
-            plot_option_vbox.children += self.wavefunctions_layout()
-        elif current_plot_option == "Matrix element scan":
-            plot_option_vbox.children += self.matelem_scan_layout()
-        elif current_plot_option == "Matrix elements":
-            plot_option_vbox.children += self.matelem_layout()
-        elif current_plot_option == "Coherence times":
-            plot_option_vbox.children += self.coherence_times_layout()
-
-        return plot_option_vbox
-
-    def qubit_params_grid_layout(self) -> HBox:
-        HBox_layout = Layout(display="flex", object_fit="contain", width="65%")
-        qubit_params_grid = HBox(layout=HBox_layout)
-
-        params_size = len(self.qubit_params_widgets)
-        if params_size > 6:
-            left_right_HBox_layout = Layout(
-                display="flex",
-                flex_flow="column nowrap",
-                object_fit="contain",
-                width="50%",
-            )
-            left_HBox = HBox(layout=left_right_HBox_layout)
-            right_HBox = HBox(layout=left_right_HBox_layout)
+    def plot_options_widgets(self) -> Dict[int, tuple]:
+        plot_options_for_active_qubit = {
+            0: self.energy_spectrum_options_widgets(),
+            1: self.wavefunctions_options_widgets(),
+            2: self.matelem_options_widgets(),
+            3: self.matelem_scan_options_widgets(),
+            4: self.coherence_times_options_widgets(),
+        }
+        return plot_options_for_active_qubit
 
-            counter = 1
-            for param_slider in self.qubit_params_widgets.values():
-                param_slider.layout.width = "95%"
-                if params_size % 2 == 0:
-                    if counter <= params_size / 2:
-                        left_HBox.children += (param_slider,)
-                    else:
-                        right_HBox.children += (param_slider,)
-                else:
-                    if counter <= params_size / 2 + 1:
-                        left_HBox.children += (param_slider,)
-                    else:
-                        right_HBox.children += (param_slider,)
-                counter += 1
-
-            qubit_params_grid.children += (
-                left_HBox,
-                right_HBox,
-            )
-        else:
-            qubit_params_grid.layout.flex_flow = "column nowrap"
-            qubit_params_grid.children = list(self.qubit_params_widgets.values())
+    def qubit_params_widgets(self) -> list:
+        widget_list = []
 
-        return qubit_params_grid
+        for param_widget in self.dict_v_qubit_params.values():
+            if hasattr(param_widget, "widget"):
+                widget_list.append(param_widget.widget())
+            else:
+                widget_list.append(param_widget)
+        return widget_list
 
-    def energy_scan_layout(self) -> Tuple[Dropdown, Checkbox, IntSlider]:
+    def energy_spectrum_options_widgets(self) -> tuple:
         """Creates the children for energy scan layout.
 
         Returns
         -------
             Tuple of plot options widgets
         """
-        self.qubit_params_widgets[
-            self.qubit_plot_options_widgets["scan_dropdown"].value
+        self.dict_v_qubit_params[
+            self.dict_v_plot_options["scan_param"].v_model
         ].disabled = True
 
         plot_options_widgets_tuple = (
-            self.qubit_plot_options_widgets["scan_dropdown"],
-            self.qubit_plot_options_widgets["subtract_ground_checkbox"],
-            self.qubit_plot_options_widgets["highest_state_slider"],
+            self.dict_v_plot_options["scan_param"],
+            flex_column(
+                [
+                    self.dict_v_plot_options["highest_state"],
+                    self.dict_v_plot_options["subtract_ground"],
+                ]
+            ),
         )
-
         return plot_options_widgets_tuple
 
-    def matelem_scan_layout(self) -> Tuple[Dropdown, Dropdown, IntSlider, Dropdown]:
+    def matelem_scan_options_widgets(self) -> tuple:
         """Creates the children for matrix elements scan layout.
 
         Returns
         -------
             Tuple of plot options widgets
         """
-        self.qubit_plot_options_widgets["mode_dropdown"].value = self.active_defaults[
+        self.dict_v_plot_options["amplitude_mode"].v_model = self.active_defaults[
             "mode_matrixelem"
         ]
-        self.qubit_params_widgets[
-            self.qubit_plot_options_widgets["scan_dropdown"].value
+        self.dict_v_qubit_params[
+            self.dict_v_plot_options["scan_param"].v_model
         ].disabled = True
 
         plot_options_widgets_tuple = (
-            self.qubit_plot_options_widgets["operator_dropdown"],
-            self.qubit_plot_options_widgets["scan_dropdown"],
-            self.qubit_plot_options_widgets["highest_state_slider"],
-            self.qubit_plot_options_widgets["mode_dropdown"],
+            self.dict_v_plot_options["operator_choice"],
+            self.dict_v_plot_options["scan_param"],
+            self.dict_v_plot_options["highest_state"],
+            self.dict_v_plot_options["amplitude_mode"],
         )
 
         return plot_options_widgets_tuple
 
-    def wavefunctions_layout(
-        self,
-    ) -> Union[
-        Tuple[Label],
-        Tuple[Union[IntSlider, SelectMultiple], Dropdown],
-        Tuple[Union[IntSlider, SelectMultiple], Dropdown, Checkbox, IntSlider],
-    ]:
+    def wavefunctions_options_widgets(self) -> Any:
         """Creates the children for the wavefunctions layout.
 
         Returns
         -------
             Tuple of plot options widgets
         """
-        if isinstance(self.active_qubit, scq.FullZeroPi):
-            plot_options_widgets_tuple = (Label(value="Not implemented"),)
+        if isinstance(self.active_qubit, QUBITS_WITHOUT_WAVEFUNCTION_PLOT):
+            plot_options_widgets_tuple = (
+                v.Text(children=["Not implemented (configuration space >2d)"]),
+            )
         else:
-            self.qubit_plot_options_widgets[
-                "mode_dropdown"
-            ].value = self.active_defaults["mode_wavefunc"]
-            self.qubit_params_widgets[
-                self.qubit_plot_options_widgets["scan_dropdown"].value
+            self.dict_v_plot_options["amplitude_mode"].v_model = self.active_defaults[
+                "mode_wavefunc"
+            ]
+            self.dict_v_qubit_params[
+                self.dict_v_plot_options["scan_param"].v_model
             ].disabled = False
 
-            if isinstance(
-                self.active_qubit, (scq.FluxQubit, scq.ZeroPi, scq.Cos2PhiQubit)
-            ):
-                which_widget = self.qubit_plot_options_widgets[
-                    "wavefunction_state_slider"
-                ]
-            else:
-                which_widget = self.qubit_plot_options_widgets["multi_state_selector"]
-
-            if isinstance(
-                self.active_qubit, (scq.ZeroPi, scq.FluxQubit, scq.Cos2PhiQubit)
-            ):
+            if isinstance(self.active_qubit, QUBITS_WITH_2D_WAVEFUNCTION_PLOT):
+                which_widget = self.dict_v_plot_options["wavefunction_state_slider"]
                 plot_options_widgets_tuple = (
                     which_widget,
-                    self.qubit_plot_options_widgets["mode_dropdown"],
+                    self.dict_v_plot_options["amplitude_mode"],
                 )
-            else:
+            else:  # 1d wavefunction plot
+                which_widget = self.dict_v_plot_options["multi_state_selector"]
                 plot_options_widgets_tuple = (
                     which_widget,
-                    self.qubit_plot_options_widgets["mode_dropdown"],
-                    self.qubit_plot_options_widgets["manual_scale_checkbox"],
-                    self.qubit_plot_options_widgets["wavefunction_scale_slider"],
+                    self.dict_v_plot_options["amplitude_mode"],
+                    self.dict_v_plot_options["manual_wf_scaling"],
+                    self.dict_v_plot_options["wavefunction_scale_slider"],
                 )
 
         return plot_options_widgets_tuple
 
-    def matelem_layout(
+    def matelem_options_widgets(
         self,
-    ) -> Tuple[Dropdown, IntSlider, Dropdown, Checkbox, Checkbox]:
+    ) -> tuple:
         """Creates the children for matrix elements layout.
 
         Returns
         -------
             Tuple of plot options widgets
         """
-        self.qubit_plot_options_widgets["mode_dropdown"].value = self.active_defaults[
+        self.dict_v_plot_options["amplitude_mode"].v_model = self.active_defaults[
             "mode_matrixelem"
         ]
-        self.qubit_params_widgets[
-            self.qubit_plot_options_widgets["scan_dropdown"].value
+        self.dict_v_qubit_params[
+            self.dict_v_plot_options["scan_param"].v_model
         ].disabled = False
 
         plot_options_widgets_tuple = (
-            self.qubit_plot_options_widgets["operator_dropdown"],
-            self.qubit_plot_options_widgets["highest_state_slider"],
-            self.qubit_plot_options_widgets["mode_dropdown"],
-            self.qubit_plot_options_widgets["show_numbers_checkbox"],
-            self.qubit_plot_options_widgets["show3d_checkbox"],
+            self.dict_v_plot_options["operator_choice"],
+            self.dict_v_plot_options["highest_state"],
+            self.dict_v_plot_options["amplitude_mode"],
+            self.dict_v_plot_options["show_matelem_numbers"],
+            self.dict_v_plot_options["show3d_matelem"],
         )
 
         return plot_options_widgets_tuple
 
-    def coherence_times_layout(
+    def coherence_times_options_widgets(
         self,
-    ) -> Tuple[Dropdown, SelectMultiple]:
+    ) -> tuple:
         """Creates the children for matrix elements layout.
 
         Returns
         -------
             Tuple of plot options widgets
         """
-        self.qubit_params_widgets[
-            self.qubit_plot_options_widgets["scan_dropdown"].value
+        self.dict_v_qubit_params[
+            self.dict_v_plot_options["scan_param"].v_model
         ].disabled = True
-        self.qubit_plot_options_widgets["i_text"].layout = Layout(width="15%")
-        self.qubit_plot_options_widgets["j_text"].layout = Layout(width="15%")
-        self.qubit_plot_options_widgets["t2_checkbox"].layout = Layout(width="45%")
-        self.qubit_plot_options_widgets["t1_checkbox"].layout = Layout(width="45%")
-        text_HBox = HBox(
-            [
-                Label(value="Effective transitions from", layout=Layout(width="50%")),
-                self.qubit_plot_options_widgets["i_text"],
-                Label(value="to", layout=Layout(width="5%")),
-                self.qubit_plot_options_widgets["j_text"],
+        self.dict_v_plot_options["i_text"].style_ = "max-width: 50px"
+        self.dict_v_plot_options["j_text"].style_ = "max-width: 50px"
+        text_HBox = v.Container(
+            class_="d-flex flex-row align-bottom py-0",
+            children=[
+                v.Text(class_="pr-3", children=["Transitions between"]),
+                self.dict_v_plot_options["i_text"],
+                v.Text(class_="px-3 pt-2", children=["and"]),
+                self.dict_v_plot_options["j_text"],
             ],
-            layout=Layout(display="flex", justify_content="space-between", width="95%"),
+            dense=True,
         )
-        checkbox_HBox = HBox(
+        checkbox_HBox = flex_column(
             [
-                self.qubit_plot_options_widgets["t1_checkbox"],
-                self.qubit_plot_options_widgets["t2_checkbox"],
+                self.dict_v_plot_options["t1_checkbox"],
+                self.dict_v_plot_options["t2_checkbox"],
             ],
-            layout=Layout(display="flex", justify_content="space-between", width="95%"),
+            dense=True,
+            class_="py-0 my-0",
         )
 
         plot_options_widgets_tuple = (
-            self.qubit_plot_options_widgets["scan_dropdown"],
-            self.qubit_plot_options_widgets["noise_channel_multi-select"],
-            VBox(
-                [text_HBox, checkbox_HBox],
-                layout=Layout(width="95%"),
-            ),
+            self.dict_v_plot_options["scan_param"],
+            self.dict_v_plot_options["noise_channel_multiselect"],
+            flex_column([text_HBox, checkbox_HBox], class_="py-0"),
         )
 
         return plot_options_widgets_tuple
 
     # Plot functions------------------------------------------------------------------
+
     @matplotlib.rc_context(matplotlib_settings)
     def evals_vs_paramvals_plot(
         self,
         scan_value: str,
         scan_range: Tuple[float, float],
         eigenvalue_state_value: int,
         subtract_ground_tf: bool,
@@ -1801,42 +1323,42 @@
         eigenvalue_state_value:
             The number of states/eigenvalues that will be plotted.
         subtract_ground_tf:
             Determines whether we subtract away the ground energy or not.
             Initially set to False.
         """
         if not _HAS_WIDGET_BACKEND:
-            self.plot_output.clear_output(wait=True)
+            self.v_plot_output.clear_output(wait=True)
         scan_min, scan_max = scan_range
         np_list = np.linspace(scan_min, scan_max, self.active_defaults["num_sample"])
-        if self.plot_change_bool:
+        if self.plot_renewal_requested:
             self.fig, ax = self.active_qubit.plot_evals_vs_paramvals(
                 scan_value,
                 np_list,
                 evals_count=eigenvalue_state_value,
                 subtract_ground=subtract_ground_tf,
             )
-            self.plot_change_bool = False
+            self.plot_renewal_requested = False
             if _HAS_WIDGET_BACKEND:
                 self.fig.canvas.header_visible = False
-                with self.plot_output:
+                with self.v_plot_output:
                     plt.show()
         else:
             self.fig.axes[0].clear()
             self.active_qubit.plot_evals_vs_paramvals(
                 scan_value,
                 np_list,
                 evals_count=eigenvalue_state_value,
                 subtract_ground=subtract_ground_tf,
                 fig_ax=(self.fig, self.fig.axes[0]),
             )
         self.fig.set_figwidth(gui_defaults.FIG_WIDTH_INCHES)
         if not _HAS_WIDGET_BACKEND:
             plt.close("all")
-            with self.plot_output:
+            with self.v_plot_output:
                 display(self.fig)
         GUI.fig_ax = self.fig, self.fig.axes[0]
 
     @matplotlib.rc_context(matplotlib_settings)
     def wavefunctions_plot(
         self,
         eigenvalue_states: Union[List[int], int],
@@ -1856,84 +1378,84 @@
             Current value of the mode (e.g. real, imaginary, etc.)
         scale_value:
             The current value for the wavefunction scale
         phi_grid:
             Specifies the domain over which the wavefunction will be plotted.
         """
         if not _HAS_WIDGET_BACKEND:
-            self.plot_output.clear_output(wait=True)
+            self.v_plot_output.clear_output(wait=True)
 
         if isinstance(
             self.active_qubit, (scq.Transmon, scq.TunableTransmon, scq.Fluxonium)
         ):
-            self.plot_output.outputs = tuple(
+            self.v_plot_output.outputs = tuple(
                 elem
-                for elem in self.plot_output.outputs
-                if "Label" not in elem["data"]["text/plain"]
+                for elem in self.v_plot_output.outputs
+                if "data" in elem and "Label" not in elem["data"]["text/plain"]
             )
             if len(eigenvalue_states) == 0:
                 if _HAS_WIDGET_BACKEND:
                     self.fig.axes[0].clear()
-                error_label = Label(value="Please select at least one state.")
-                with self.plot_output:
+                error_label = v.Text(children=["Must select at least one state."])
+                with self.v_plot_output:
                     display(error_label)
                 return
-            if self.plot_change_bool:
+            if self.plot_renewal_requested:
                 self.fig, ax = self.active_qubit.plot_wavefunction(  # type:ignore
                     which=eigenvalue_states,
                     mode=mode_value,
                     scaling=scale_value,
                     phi_grid=phi_grid,
                 )
-                self.plot_change_bool = False
+                self.plot_renewal_requested = False
                 if _HAS_WIDGET_BACKEND:
                     self.fig.canvas.header_visible = False
-                    with self.plot_output:
+                    with self.v_plot_output:
                         plt.show()
             else:
                 self.fig.axes[0].clear()
                 self.active_qubit.plot_wavefunction(  # type:ignore
                     which=eigenvalue_states,
                     mode=mode_value,
                     scaling=scale_value,
                     phi_grid=phi_grid,
                     fig_ax=(self.fig, self.fig.axes[0]),
                 )
         else:
             if isinstance(self.active_qubit, scq.FluxQubit):
                 grid_dict = {"phi_grid": phi_grid}
-            elif isinstance(self.active_qubit, scq.ZeroPi):
+            elif isinstance(self.active_qubit, (scq.ZeroPi)):  # , scq.Bifluxon)):
                 grid_dict = {"theta_grid": theta_grid}
             elif isinstance(self.active_qubit, scq.Cos2PhiQubit):
                 grid_dict = {"phi_grid": phi_grid, "theta_grid": theta_grid}
 
-            if self.plot_change_bool:
+            if self.plot_renewal_requested:
                 self.fig, ax = self.active_qubit.plot_wavefunction(  # type:ignore
                     which=eigenvalue_states, mode=mode_value, **grid_dict
                 )
-                self.plot_change_bool = False
+                self.plot_renewal_requested = False
 
                 if _HAS_WIDGET_BACKEND:
                     self.fig.canvas.header_visible = False
-                    with self.plot_output:
+                    with self.v_plot_output:
                         plt.show()
             else:
                 self.fig.delaxes(self.fig.axes[1])
                 self.fig.axes[0].clear()
                 self.active_qubit.plot_wavefunction(  # type:ignore
                     which=eigenvalue_states,
                     mode=mode_value,
                     **grid_dict,
                     fig_ax=(self.fig, self.fig.axes[0]),
                 )
 
         self.fig.set_figwidth(gui_defaults.FIG_WIDTH_INCHES)
         if not _HAS_WIDGET_BACKEND:
             plt.close("all")
-            with self.plot_output:
+            with self.v_plot_output:
                 display(self.fig)
         GUI.fig_ax = self.fig, self.fig.axes[0]
 
     def matelem_vs_paramvals_plot(
         self,
         operator_value: str,
         scan_value: str,
@@ -1955,29 +1477,29 @@
             which plot_matelem_vs_paramvals() will plot over.
         matrix_element_state_value:
             The number of states/elements that will be shown.
         mode_value:
             Current value of the mode (e.g. real, imaginary, etc.)
         """
         if not _HAS_WIDGET_BACKEND:
-            self.plot_output.clear_output(wait=True)
+            self.v_plot_output.clear_output(wait=True)
         scan_min, scan_max = scan_range
         np_list = np.linspace(scan_min, scan_max, self.active_defaults["num_sample"])
-        if self.plot_change_bool:
+        if self.plot_renewal_requested:
             self.fig, ax = self.active_qubit.plot_matelem_vs_paramvals(
                 operator_value,
                 scan_value,
                 np_list,
                 select_elems=matrix_element_state_value,
                 mode=mode_value,
             )
-            self.plot_change_bool = False
+            self.plot_renewal_requested = False
             if _HAS_WIDGET_BACKEND:
                 self.fig.canvas.header_visible = False
-                with self.plot_output:
+                with self.v_plot_output:
                     plt.show()
         else:
             self.fig.axes[0].clear()
             self.active_qubit.plot_matelem_vs_paramvals(
                 operator_value,
                 scan_value,
                 np_list,
@@ -1985,15 +1507,15 @@
                 mode=mode_value,
                 fig_ax=(self.fig, self.fig.axes[0]),
             )
 
         self.fig.set_figwidth(gui_defaults.FIG_WIDTH_INCHES)
         if not _HAS_WIDGET_BACKEND:
             plt.close("all")
-            with self.plot_output:
+            with self.v_plot_output:
                 display(self.fig)
         GUI.fig_ax = self.fig, self.fig.axes
 
     def matrixelements_plot(
         self,
         operator_value: str,
         eigenvalue_state_value: int,
@@ -2016,27 +1538,27 @@
             Determines whether the numerical values will be shown in the 2D plot.
             Initially set to False.
         show3d_tf:
             Determines whether a 3D version of the 2D plot will be shown.
             Initially set to True.
         """
         if not _HAS_WIDGET_BACKEND:
-            self.plot_output.clear_output(wait=True)
-        if self.plot_change_bool:
+            self.v_plot_output.clear_output(wait=True)
+        if self.plot_renewal_requested:
             self.fig, ax = self.active_qubit.plot_matrixelements(
                 operator_value,
                 evals_count=eigenvalue_state_value,
                 mode=mode_value,
                 show_numbers=show_numbers_tf,
                 show3d=show3d_tf,
             )
-            self.plot_change_bool = False
+            self.plot_renewal_requested = False
             if _HAS_WIDGET_BACKEND:
                 self.fig.canvas.header_visible = False
-                with self.plot_output:
+                with self.v_plot_output:
                     plt.show()
         else:
             if show3d_tf:
                 self.fig.delaxes(self.fig.axes[2])
                 self.fig.delaxes(self.fig.axes[1])
                 self.fig.add_subplot(122)
                 axes = (self.fig.axes[0], self.fig.axes[1])
@@ -2054,15 +1576,15 @@
                 show3d=show3d_tf,
                 fig_ax=(self.fig, axes),
             )
 
         self.fig.set_figwidth(gui_defaults.FIG_WIDTH_INCHES)
         if not _HAS_WIDGET_BACKEND:
             plt.close("all")
-            with self.plot_output:
+            with self.v_plot_output:
                 display(self.fig)
         GUI.fig_ax = self.fig, self.fig.axes
 
     def coherence_vs_paramvals_plot(
         self,
         scan_value: str,
         scan_range: Tuple[float, float],
@@ -2081,32 +1603,28 @@
         scan_range:
             Sets the interval [ min, max ] through
             which plot_evals_vs_paramvals() will plot over.
         noise_channels:
             List of noise channels to be displayed
         """
         if not _HAS_WIDGET_BACKEND:
-            self.plot_output.clear_output(wait=True)
+            self.v_plot_output.clear_output(wait=True)
         scan_min, scan_max = scan_range
         np_list = np.linspace(scan_min, scan_max, self.active_defaults["num_sample"])
 
-        self.plot_output.outputs = tuple(
-            elem
-            for elem in self.plot_output.outputs
-            if "Label" not in elem["data"]["text/plain"]
-        )
+        self.v_plot_output.outputs = tuple(elem for elem in self.v_plot_output.outputs)
         if len(noise_channels["coherence_times"]) == 0:
             if _HAS_WIDGET_BACKEND:
                 self.fig.axes[0].clear()
-            error_label = Label(value="Please select at least one noise channel.")
-            with self.plot_output:
+            error_label = v.Text(children=["Must select at least one noise channel."])
+            with self.v_plot_output:
                 display(error_label)
             return
 
-        if self.plot_change_bool:
+        if self.plot_renewal_requested:
             if not t1_effective_tf and not t2_effective_tf:
                 self.fig, ax = self.active_qubit.plot_coherence_vs_paramvals(
                     param_name=scan_value,
                     param_vals=np_list,
                     noise_channels=noise_channels["coherence_times"],
                     common_noise_options=common_noise_options,
                 )
@@ -2136,18 +1654,18 @@
                 self.active_qubit.plot_t2_effective_vs_paramvals(
                     param_name=scan_value,
                     param_vals=np_list,
                     noise_channels=noise_channels["t2_eff"],
                     common_noise_options=common_noise_options,
                     fig_ax=(self.fig, ax[1]),
                 )
-            self.plot_change_bool = False
+            self.plot_renewal_requested = False
             if _HAS_WIDGET_BACKEND:
                 self.fig.canvas.header_visible = False
-                with self.plot_output:
+                with self.v_plot_output:
                     plt.show()
         else:
             for ax in self.fig.axes:
                 ax.clear()
             if not t1_effective_tf and not t2_effective_tf:
                 if len(noise_channels["coherence_times"]) > 1:
                     axes = np.array(self.fig.axes).reshape(
@@ -2192,10 +1710,10 @@
                     noise_channels=noise_channels["t2_eff"],
                     common_noise_options=common_noise_options,
                     fig_ax=(self.fig, self.fig.axes[1]),
                 )
         self.fig.set_figwidth(gui_defaults.FIG_WIDTH_INCHES)
         if not _HAS_WIDGET_BACKEND:
             plt.close("all")
-            with self.plot_output:
+            with self.v_plot_output:
                 display(self.fig)
         GUI.fig_ax = self.fig, self.fig.axes
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `scqubits-3.1.1/scqubits/utils/__init__.py` & `scqubits-3.2.0/scqubits/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `scqubits-3.1.1/scqubits/utils/cpu_switch.py` & `scqubits-3.2.0/scqubits/utils/cpu_switch.py`

 * *Files identical despite different names*

### Comparing `scqubits-3.1.1/scqubits/utils/misc.py` & `scqubits-3.2.0/scqubits/utils/misc.py`

 * *Files 11% similar despite different names*

```diff
@@ -12,21 +12,25 @@
 
 import ast
 import functools
 import platform
 import warnings
 
 from collections.abc import Sequence
+from distutils.version import StrictVersion
 from io import StringIO
 from typing import Any, Callable, Dict, Iterable, List, Optional, Tuple, Union
 
+import matplotlib
 import numpy as np
 import qutip as qt
 import scipy as sp
+from matplotlib import get_backend as get_matplotlib_backend
 
+import scqubits.settings
 from scqubits.settings import IN_IPYTHON
 
 if IN_IPYTHON:
     from tqdm.notebook import tqdm
 else:
     from tqdm import tqdm
 
@@ -93,27 +97,28 @@
     num_cpus:
         Number of CPUS/cores employed in underlying calculation.
     """
 
     def __init__(self, desc: str, num_cpus: int) -> None:
         self.desc = desc
         self.num_cpus = num_cpus
-        self.tqdm_bar: Optional[tqdm] = None
+        self.tqdm_bar = None
 
     def __enter__(self) -> None:
         self.tqdm_bar = tqdm(
             total=0,
-            disable=(self.num_cpus == 1),
+            disable=(self.num_cpus == 1) or scqubits.settings.PROGRESSBAR_DISABLED,
             leave=False,
             desc=self.desc,
             bar_format="{desc}",
         )
 
     def __exit__(self, *args) -> None:
-        self.tqdm_bar.close()
+        if self.tqdm_bar:
+            self.tqdm_bar.close()
 
 
 class Required:
     """Decorator class, ensuring that a given requirement or set of requirements is
     fulfilled.
 
     Parameters
@@ -122,45 +127,61 @@
         All bool conditions have to be True to pass. The provided str keys are used to
         display information on what condition is failing.
     """
 
     def __init__(self, **requirements) -> None:
         self.requirements_bools = list(requirements.values())
         self.requirements_names = list(requirements.keys())
+        self.missing_imports = [name for name in requirements if not requirements[name]]
 
     def __call__(self, func: Callable, *args, **kwargs) -> Callable:
         @functools.wraps(func)
         def decorated_func(*args, **kwargs):
             if all(self.requirements_bools):
                 return func(*args, **kwargs)
             else:
-                raise Exception(
-                    "ImportError: use of this method requires the optional package(s):"
-                    " {}. If you wish to use this functionality, the corresponding"
-                    " package(s) must be installed manually. (Installation via `conda"
-                    " install -c conda-forge <packagename>` or `pip install"
-                    " <packagename>` is recommended.)".format(self.requirements_names)
-                )
+                with warnings.catch_warnings():
+                    if self.missing_imports == ["ipyvuetify"]:
+                        warnings.warn(
+                            "Starting with v3.2, scqubits uses the optional package 'ipyuetify' for graphical "
+                            "user interfaces. To use this functionality, add the package via "
+                            "`conda install -c conda-forge ipyvuetify` or `pip install ipyvuetify`.\n"
+                            "For use with jupyter lab, additionally execute "
+                            "`jupyter labextension install jupyter-vuetify`.\n",
+                            category=Warning,
+                        )
+                    else:
+                        warnings.warn(
+                            "use of this method requires the optional package(s):"
+                            " {}. If you wish to use this functionality, the corresponding"
+                            " package(s) must be installed manually. (Installation via `conda"
+                            " install -c conda-forge <packagename>` or `pip install"
+                            " <packagename>` is recommended.)".format(
+                                self.requirements_names
+                            ),
+                            category=Warning,
+                        )
 
         return decorated_func
 
 
 def check_sync_status(func: Callable) -> Callable:
     @functools.wraps(func)
     def wrapper(self, *args, **kwargs):
-        if self._out_of_sync:
+        if self._out_of_sync and not self._out_of_sync_warning_issued:
             with warnings.catch_warnings():
                 warnings.simplefilter("always")
                 warnings.warn(
-                    "[scqubits] Some system parameters have been changed and"
+                    "[scqubits] Some quantum system parameters have been changed and"
                     " generated spectrum data could be outdated, potentially leading to"
                     " incorrect results. Spectral data can be refreshed via"
                     " <HilbertSpace>.generate_lookup() or <ParameterSweep>.run()",
                     Warning,
                 )
+            self._out_of_sync_warning_issued = True
         return func(self, *args, **kwargs)
 
     return wrapper
 
 
 def check_lookup_exists(func: Callable) -> Callable:
     @functools.wraps(func)
@@ -248,22 +269,36 @@
     short_str = ""
     for entry in the_tuple:
         short_str += str(entry) + ","
     return short_str[:-1]
 
 
 def to_list(obj: Any) -> List[Any]:
+    """
+    Converts object to a list: if the input is already a list, it will return the same list. If the input is
+    a numpy array, it will convert to a python list. Otherwise, it will return
+    the original object in a single-elemented python list.
+
+    Parameters
+    ----------
+    obj:
+        Specify the type of object that is being passed into the function
+
+    Returns
+    -------
+        a list of the object passed in
+    """
     if isinstance(obj, list):
         return obj
     if isinstance(obj, np.ndarray):
         return obj.tolist()
     return [obj]
 
 
-def about(print_info=True):
+def about(print_info=True) -> Optional[str]:
     """Prints or returns a string with basic information about
     scqubits as well as installed version of various packages
     that scqubits depends on.
 
     Parameters
     ----------
     print_info: bool
@@ -324,22 +359,30 @@
     if print_info:
         print(fs.getvalue())
         return None
     else:
         return fs.getvalue()
 
 
-def is_float_string(the_string: str) -> bool:
+def is_string_float(the_string: str) -> bool:
     try:
         float(the_string)
         return True
     except ValueError:
         return False
 
 
+def is_string_int(the_string: str) -> bool:
+    try:
+        int(the_string)
+        return True
+    except ValueError:
+        return False
+
+
 def list_intersection(list1: list, list2: list) -> list:
     return list(set(list1) & set(list2))
 
 
 def flatten_list(nested_list):
     """
     Flattens a list of lists once, not recursive.
@@ -353,30 +396,58 @@
     Returns
     -------
     Flattened list of objects
     """
     return functools.reduce(lambda a, b: a + b, nested_list)
 
 
-def flatten_list_recursive(S):
+def flatten_list_recursive(some_list: list) -> list:
     """
     Flattens a list of lists recursively.
 
     Parameters
     ----------
-
-    nested_list:
+    some_list:
         A list of lists, which can hold any class instance.
 
     Returns
     -------
     Flattened list of objects
     """
-    if S == []:
-        return S
-    if isinstance(S[0], list):
-        return flatten_list_recursive(S[0]) + flatten_list_recursive(S[1:])
-    return S[:1] + flatten_list_recursive(S[1:])
+    if some_list == []:
+        return some_list
+    if isinstance(some_list[0], list):
+        return flatten_list_recursive(some_list[0]) + flatten_list_recursive(
+            some_list[1:]
+        )
+    return some_list[:1] + flatten_list_recursive(some_list[1:])
 
 
 def number_of_lists_in_list(list_object: list) -> int:
+    """
+    Takes a list as an argument and returns the number of lists in that list. (Counts lists at root level only, no
+    recursion.)
+
+    Parameters
+    ----------
+    list_object:
+        List to be analyzed
+
+    Returns
+    -------
+    The number of lists in the list
+    """
     return sum([1 for element in list_object if type(element) == list])
+
+
+def check_matplotlib_compatibility():
+    if _HAS_WIDGET_BACKEND and StrictVersion(matplotlib.__version__) < StrictVersion(
+        "3.5.1"
+    ):
+        warnings.warn(
+            "The widget backend requires Matplotlib >=3.5.1 for proper functioning",
+            UserWarning,
+        )
+
+
+MATPLOTLIB_WIDGET_BACKEND = "module://ipympl.backend_nbagg"
+_HAS_WIDGET_BACKEND = get_matplotlib_backend() == MATPLOTLIB_WIDGET_BACKEND
```

### Comparing `scqubits-3.1.1/scqubits/utils/plot_defaults.py` & `scqubits-3.2.0/scqubits/utils/plot_defaults.py`

 * *Files identical despite different names*

### Comparing `scqubits-3.1.1/scqubits/utils/plot_utils.py` & `scqubits-3.2.0/scqubits/utils/plot_utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -19,16 +19,16 @@
 import numpy as np
 
 from matplotlib.axes import Axes
 from matplotlib.figure import Figure
 from numpy import ndarray
 
 from scqubits import settings as settings
-from scqubits.utils import plot_defaults as defaults
 from scqubits.settings import matplotlib_settings
+from scqubits.utils import plot_defaults as defaults
 
 if TYPE_CHECKING:
     from scqubits.core.storage import WaveFunction
 
 
 # A dictionary of plotting options that are directly passed to specific matplotlib's
 # plot commands.
@@ -45,15 +45,17 @@
     "imshow": ("interpolation",),
     "contourf": tuple(),  # empty for now
 }
 
 
 @mpl.rc_context(matplotlib_settings)
 def _extract_kwargs_options(
-    kwargs: Dict[str, Any], plot_type: str, direct_plot_options: Dict[str, Any] = None
+    kwargs: Dict[str, Any],
+    plot_type: str,
+    direct_plot_options: Optional[Dict[str, Any]] = None,
 ) -> Dict[str, Any]:
     """
     Select options from kwargs for a given plot_type and return them in a dictionary.
 
     Parameters
     ----------
     kwargs:
@@ -78,15 +80,15 @@
         if key in direct_plot_options[plot_type]:
             selected_options[key] = kwargs[key]
     return selected_options
 
 
 @mpl.rc_context(matplotlib_settings)
 def _process_options(
-    figure: Figure, axes: Axes, opts: Dict[str, Any] = None, **kwargs
+    figure: Figure, axes: Axes, opts: Optional[Dict[str, Any]] = None, **kwargs
 ) -> None:
     """
     Processes plotting options.
 
     Parameters
     ----------
     figure:
@@ -158,16 +160,19 @@
 
 @mpl.rc_context(matplotlib_settings)
 def scale_wavefunctions(
     wavefunc_list: List["WaveFunction"],
     potential_vals: np.ndarray,
     scaling: Optional[float],
 ) -> List["WaveFunction"]:
+    scale_factors = np.array(
+        [wavefunc.amplitude_scale_factor(potential_vals) for wavefunc in wavefunc_list]
+    )
     for wavefunc in wavefunc_list:
-        wavefunc.rescale_to_potential(potential_vals)
+        wavefunc.rescale(np.max(scale_factors))
     adaptive_scalefactor = scaling or defaults.set_wavefunction_scaling(
         wavefunc_list, potential_vals
     )
     for wavefunc in wavefunc_list:
         wavefunc.rescale(adaptive_scalefactor)
     return wavefunc_list
```

### Comparing `scqubits-3.1.1/scqubits/utils/plotting.py` & `scqubits-3.2.0/scqubits/utils/plotting.py`

 * *Files 1% similar despite different names*

```diff
@@ -20,24 +20,24 @@
 from matplotlib.figure import Figure
 from mpl_toolkits.axes_grid1 import make_axes_locatable
 
 import scqubits.core.constants as constants
 import scqubits.utils.misc as utils
 import scqubits.utils.plot_defaults as defaults
 
+from scqubits.settings import matplotlib_settings
 from scqubits.utils.plot_utils import (
     _extract_kwargs_options,
     _process_options,
     add_numbers_to_axes,
     color_normalize,
     plot_potential_to_axes,
     plot_wavefunction_to_axes,
     scale_wavefunctions,
 )
-from scqubits.settings import matplotlib_settings
 
 if TYPE_CHECKING:
     from scqubits.core.storage import SpectrumData, WaveFunction, WaveFunctionOnGrid
 
 try:
     from labellines import labelLines
 
@@ -361,17 +361,17 @@
     for axis, locs in [
         (axes.xaxis, np.arange(x_count)),
         (axes.yaxis, np.arange(y_count)),
     ]:
         axis.set_ticks(locs + 0.5, minor=True)
         axis.set(ticks=locs + 0.5, ticklabels=locs)
 
-    axes.tick_params(axis='x', pad=-5)
-    axes.tick_params(axis='y', pad=-5)
-    axes.tick_params(axis='z', pad=-2)
+    axes.tick_params(axis="x", pad=-5)
+    axes.tick_params(axis="y", pad=-5)
+    axes.tick_params(axis="z", pad=-2)
 
     _process_options(fig, axes, opts=defaults.matrix(), **kwargs)
 
     return fig, axes
 
 
 @mpl.rc_context(matplotlib_settings)
@@ -409,20 +409,26 @@
     modefunction = constants.MODE_FUNC_DICT[mode]
     zheight = modefunction(matrix).flatten()  # height of bars from matrix elements
 
     min_zheight, max_zheight, nrm = color_normalize(zheight, mode)
 
     if show_colorbar:
         # add colorbar with normalized range
-        fig.colorbar(
-            mpl.cm.ScalarMappable(norm=nrm, cmap=plt.cm.viridis),
-            ax=axes,
-            fraction=0.046,
-            pad=0.04,
-        )
+        if hasattr(axes, "colorbar"):  # update existing colorbar
+            axes.colorbar.update_normal(
+                mpl.cm.ScalarMappable(norm=nrm, cmap=plt.cm.viridis)
+            )
+        else:  # create new colorbar
+            cb = fig.colorbar(
+                mpl.cm.ScalarMappable(norm=nrm, cmap=plt.cm.viridis),
+                ax=axes,
+                fraction=0.046,
+                pad=0.04,
+            )
+            axes.colorbar = cb
     cax = axes.matshow(modefunction(matrix), cmap=plt.cm.viridis, interpolation=None)
 
     if show_numbers:
         fig_width, fig_height = fig.get_size_inches()
         box_width_inches = fig_width / matrix.shape[1]
         box_height_inches = fig_height / matrix.shape[0]
         font_size = min(box_width_inches, box_height_inches) * 11
@@ -572,17 +578,17 @@
     **kwargs:
         standard plotting option (see separate documentation)
 
     Returns
     -------
     matplotlib objects for further editing
     """
-    assert specdata.matrixelem_table is not None, (
-        "SpectrumData is missing matrix " "element data!"
-    )
+    assert (
+        specdata.matrixelem_table is not None
+    ), "SpectrumData is missing matrix element data!"
     fig, axes = kwargs.get("fig_ax") or plt.subplots()
     x_vals = specdata.param_vals
     modefunction = constants.MODE_FUNC_DICT[mode]
 
     if isinstance(select_elems, int):
         index_pairs = [
             (row, col) for row in range(select_elems) for col in range(row + 1)
```

### Comparing `scqubits-3.1.1/scqubits/utils/spectrum_utils.py` & `scqubits-3.2.0/scqubits/utils/spectrum_utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 #
 #    This source code is licensed under the BSD-style license found in the
 #    LICENSE file in the root directory of this source tree.
 ############################################################################
 
 import cmath
 
-from typing import TYPE_CHECKING, List, Optional, Tuple, Union
+from typing import TYPE_CHECKING, Callable, List, Optional, Tuple, Union
 
 import numpy as np
 import qutip as qt
 import scipy as sp
 
 from numpy import ndarray
 from qutip import Qobj
@@ -29,17 +29,17 @@
     from scqubits.core.qubit_base import QubitBaseClass
     from scqubits.io_utils.fileio_qutip import QutipEigenstates
 
 from scqubits.utils.typedefs import QuantumSys
 
 
 def eigsh_safe(*args, **kwargs):
-    """Wrapper method for scipy.sparse.linalg.eigsh
-    This ensures:
-    1. Always use the same "random" starting vector v0. Otherwise results show
+    """Wrapper method for `scipy.sparse.linalg.eigsh` which ensures the following.
+
+    1. Always use the same "random" starting vector v0. Otherwise, results show
        random behavior (small deviations between different runs, problem for pytests)
     2. Test for degenerate eigenvalues. If there are any, need to orthogonalize the
         eigenvectors properly."""
     mat_size = args[0].shape[0]
     kwargs["v0"] = settings.RANDOM_ARRAY[:mat_size]
 
     if kwargs.get("return_eigenvectors"):
@@ -73,15 +73,17 @@
     """
     ordered_evals_indices = evals.argsort()  # sort manually
     evals[:] = evals[ordered_evals_indices]
     evecs[:] = evecs[:, ordered_evals_indices]
     return evals, evecs
 
 
-def extract_phase(complex_array: np.ndarray, position: Optional[int] = None) -> float:
+def extract_phase(
+    complex_array: np.ndarray, position: Optional[Tuple[int, ...]] = None
+) -> float:
     """Extracts global phase from `complex_array` at given `position`. If position is
     not specified, the `position` is set as follows. Find the maximum between the
     leftmost point and the halfway point of the wavefunction. The position of that
     point is used to determine the phase factor to be eliminated.
 
     Parameters
     ----------
@@ -390,19 +392,19 @@
         [esys_mapdata[index][0] for index in range(paramvals_count)]
     )
     eigenstate_table = [esys_mapdata[index][1] for index in range(paramvals_count)]
     return eigenenergy_table, eigenstate_table
 
 
 def identity_wrap(
-    operator: Union[str, ndarray, Qobj],
+    operator: Union[str, ndarray, Qobj, Callable],
     subsystem: "QuantumSys",
     subsys_list: List["QuantumSys"],
     op_in_eigenbasis: bool = False,
-    evecs: ndarray = None,
+    evecs: Optional[ndarray] = None,
 ) -> Qobj:
     """Takes the `operator` belonging to `subsystem` and "wraps" it in identities.
     The full Hilbert space is taken to consist of all subsystems given as
     `subsys_list`. `subsystem` must be one element in that list. For each of the
     other subsystems in the list, an identity operator of the correct dimension is
     generated and inserted into the appropriate Kronecker product "sandwiching" the
     operator.
@@ -426,14 +428,21 @@
     Returns
     -------
         operator in the full Hilbert space (as specified by `subsystem_list`). This
         operator is expressed in the bare product basis consisting of the energy
         eigenstates of each subsystem (unless `operator` is provided as a `Qobj`,
         in which case no conversion takes place).
     """
+    if not isinstance(operator, qt.Qobj) and callable(operator):
+        try:
+            operator = operator(energy_esys=(None, evecs))
+        except TypeError:
+            operator = operator()
+        op_in_eigenbasis = True
+
     subsys_operator = convert_operator_to_qobj(
         operator, subsystem, op_in_eigenbasis, evecs  # type:ignore
     )
     operator_identitywrap_list = [
         qt.operators.qeye(the_subsys.truncated_dim) for the_subsys in subsys_list
     ]
     subsystem_index = subsys_list.index(subsystem)
```

### Comparing `scqubits-3.1.1/scqubits/utils/typedefs.py` & `scqubits-3.2.0/scqubits/utils/typedefs.py`

 * *Files identical despite different names*

### Comparing `scqubits-3.1.1/scqubits.egg-info/PKG-INFO` & `scqubits-3.2.0/scqubits.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: scqubits
-Version: 3.1.1
+Version: 3.2.0
 Summary: scqubits: superconducting qubits in Python
 Home-page: https://scqubits.readthedocs.io
 Author: Jens Koch, Peter Groszkowski
 Author-email: jens-koch@northwestern.edu, piotrekg@gmail.com
 License: BSD
 Keywords: superconducting qubits
 Platform: Linux
@@ -22,15 +22,14 @@
 Classifier: Operating System :: Unix
 Classifier: Operating System :: Microsoft :: Windows
 Requires-Python: >=3.7
 Provides-Extra: graphics
 Provides-Extra: explorer
 Provides-Extra: h5-support
 Provides-Extra: pathos
-Provides-Extra: fitting
 License-File: LICENSE
 
 
 scqubits is an open-source Python library for simulating superconducting qubits. It is
 meant to give the user a convenient way to obtain energy spectra of common
 superconducting qubits, plot energy levels as a function of external parameters,
 calculate matrix elements etc. The library further provides an interface to QuTiP,
```

### Comparing `scqubits-3.1.1/scqubits.egg-info/SOURCES.txt` & `scqubits-3.2.0/scqubits.egg-info/SOURCES.txt`

 * *Files 10% similar despite different names*

```diff
@@ -17,14 +17,15 @@
 scqubits/core/__init__.py
 scqubits/core/central_dispatch.py
 scqubits/core/circuit.py
 scqubits/core/circuit_utils.py
 scqubits/core/constants.py
 scqubits/core/cos2phi_qubit.py
 scqubits/core/descriptors.py
+scqubits/core/diag.py
 scqubits/core/discretization.py
 scqubits/core/flux_qubit.py
 scqubits/core/fluxonium.py
 scqubits/core/generic_qubit.py
 scqubits/core/hilbert_space.py
 scqubits/core/namedslots_array.py
 scqubits/core/noise.py
@@ -36,25 +37,29 @@
 scqubits/core/storage.py
 scqubits/core/sweeps.py
 scqubits/core/symbolic_circuit.py
 scqubits/core/transmon.py
 scqubits/core/units.py
 scqubits/core/zeropi.py
 scqubits/core/zeropi_full.py
-scqubits/core/qubit_img/cos2phi-qubit.jpg
-scqubits/core/qubit_img/fixed-transmon.jpg
-scqubits/core/qubit_img/flux-qubit.jpg
-scqubits/core/qubit_img/fluxonium.jpg
-scqubits/core/qubit_img/fullzeropi.jpg
-scqubits/core/qubit_img/kerr-oscillator.jpg
-scqubits/core/qubit_img/oscillator.jpg
-scqubits/core/qubit_img/tunable-transmon.jpg
-scqubits/core/qubit_img/zeropi.jpg
+scqubits/core/qubit_img/Bifluxon.jpg
+scqubits/core/qubit_img/Cos2PhiQubit.jpg
+scqubits/core/qubit_img/FluxQubit.jpg
+scqubits/core/qubit_img/Fluxonium.jpg
+scqubits/core/qubit_img/FullZeroPi.jpg
+scqubits/core/qubit_img/KerrOscillator.jpg
+scqubits/core/qubit_img/Oscillator.jpg
+scqubits/core/qubit_img/Snailmon.jpg
+scqubits/core/qubit_img/Transmon.jpg
+scqubits/core/qubit_img/TunableTransmon.jpg
+scqubits/core/qubit_img/ZeroPi.jpg
 scqubits/explorer/__init__.py
 scqubits/explorer/explorer_panels.py
+scqubits/explorer/explorer_settings.py
+scqubits/explorer/explorer_widget.py
 scqubits/io_utils/__init__.py
 scqubits/io_utils/fileio.py
 scqubits/io_utils/fileio_backends.py
 scqubits/io_utils/fileio_qutip.py
 scqubits/io_utils/fileio_serializers.py
 scqubits/tests/__init__.py
 scqubits/tests/conftest.py
@@ -89,30 +94,42 @@
 scqubits/tests/data/fluxonium_5.hdf5
 scqubits/tests/data/fluxqubit_1.hdf5
 scqubits/tests/data/fluxqubit_2.hdf5
 scqubits/tests/data/fluxqubit_4.hdf5
 scqubits/tests/data/fluxqubit_5.hdf5
 scqubits/tests/data/fullzeropi_1.hdf5
 scqubits/tests/data/fullzeropi_2.hdf5
+scqubits/tests/data/snailmon_1.hdf5
+scqubits/tests/data/snailmon_2.hdf5
+scqubits/tests/data/snailmon_4.hdf5
+scqubits/tests/data/snailmon_5.hdf5
 scqubits/tests/data/transmon_1.hdf5
 scqubits/tests/data/transmon_2.hdf5
 scqubits/tests/data/transmon_4.hdf5
 scqubits/tests/data/transmon_5.hdf5
 scqubits/tests/data/zeropi-test.hdf5
 scqubits/tests/data/zeropi_1.hdf5
 scqubits/tests/data/zeropi_2.hdf5
 scqubits/tests/data/zeropi_4.hdf5
 scqubits/tests/data/zeropi_5.hdf5
 scqubits/tests/data/zpifull-test.hdf5
 scqubits/ui/__init__.py
-scqubits/ui/explorer_widget.py
 scqubits/ui/gui.py
+scqubits/ui/gui_custom_widgets.py
 scqubits/ui/gui_defaults.py
+scqubits/ui/gui_navbar.py
+scqubits/ui/gui_setup.py
 scqubits/ui/hspace_widget.py
 scqubits/ui/qubit_widget.py
+scqubits/ui/icons/En.png
+scqubits/ui/icons/Me.png
+scqubits/ui/icons/MeS.png
+scqubits/ui/icons/T1.png
+scqubits/ui/icons/psi.png
+scqubits/ui/icons/scq-logo.png
 scqubits/utils/__init__.py
 scqubits/utils/cpu_switch.py
 scqubits/utils/misc.py
 scqubits/utils/plot_defaults.py
 scqubits/utils/plot_utils.py
 scqubits/utils/plotting.py
 scqubits/utils/spectrum_utils.py
```

### Comparing `scqubits-3.1.1/setup.py` & `scqubits-3.2.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -48,34 +48,33 @@
 """
 
 
 EXTRA_KWARGS = {}
 
 # version information about scqubits goes here
 MAJOR = 3
-MINOR = 1
-MICRO = 1
+MINOR = 2
+MICRO = 0
 ISRELEASED = True
 
 VERSION = "%d.%d.%d" % (MAJOR, MINOR, MICRO)
 
 CURRENT_DIR = os.path.dirname(os.path.abspath(__file__))
 with open(os.path.join(CURRENT_DIR, "requirements.txt")) as requirements:
     INSTALL_REQUIRES = requirements.read().splitlines()
 
 
 EXTRAS_REQUIRE = {
     "graphics": ["matplotlib-label-lines (>=0.3.6)"],
     "explorer": ["ipywidgets (>=7.5)"],
     "h5-support": ["h5py (>=2.10)"],
-    "pathos": ["pathos", "dill"],
-    "fitting": ["lmfit"],
+    "pathos": ["pathos", "dill"]
 }
 
-TESTS_REQUIRE = ["h5py (>=2.7.1)", "pathos", "dill", "ipywidgets", "pytest", "lmfit"]
+TESTS_REQUIRE = ["h5py (>=2.7.1)", "pathos", "dill", "ipywidgets", "pytest"]
 
 PACKAGES = [
     "scqubits",
     "scqubits/core",
     "scqubits/tests",
     "scqubits/utils",
     "scqubits/ui",
```

