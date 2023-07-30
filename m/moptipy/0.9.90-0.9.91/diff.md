# Comparing `tmp/moptipy-0.9.90.tar.gz` & `tmp/moptipy-0.9.91.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "moptipy-0.9.90.tar", last modified: Fri Jul 28 11:03:09 2023, max compression
+gzip compressed data, was "moptipy-0.9.91.tar", last modified: Sun Jul 30 05:02:51 2023, max compression
```

## Comparing `moptipy-0.9.90.tar` & `moptipy-0.9.91.tar`

### file list

```diff
@@ -1,259 +1,259 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 11:03:09.306593 moptipy-0.9.90/
--rw-r--r--   0 runner    (1001) docker     (123)   195321 2023-07-28 11:03:09.306593 moptipy-0.9.90/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)   186686 2023-07-28 10:39:11.000000 moptipy-0.9.90/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 11:03:09.274593 moptipy-0.9.90/moptipy/
--rw-r--r--   0 runner    (1001) docker     (123)      914 2023-07-28 10:39:11.000000 moptipy-0.9.90/moptipy/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 11:03:09.274593 moptipy-0.9.90/moptipy/algorithms/
--rw-r--r--   0 runner    (1001) docker     (123)      644 2023-07-28 10:39:11.000000 moptipy-0.9.90/moptipy/algorithms/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5478 2023-07-28 10:39:11.000000 moptipy-0.9.90/moptipy/algorithms/luby_restarts.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 11:03:09.278593 moptipy-0.9.90/moptipy/algorithms/mo/
--rw-r--r--   0 runner    (1001) docker     (123)       76 2023-07-28 10:39:11.000000 moptipy-0.9.90/moptipy/algorithms/mo/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2828 2023-07-28 10:39:11.000000 moptipy-0.9.90/moptipy/algorithms/mo/morls.py
--rw-r--r--   0 runner    (1001) docker     (123)    13469 2023-07-28 10:39:11.000000 moptipy-0.9.90/moptipy/algorithms/mo/nsga2.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 11:03:09.278593 moptipy-0.9.90/moptipy/algorithms/modules/
--rw-r--r--   0 runner    (1001) docker     (123)       44 2023-07-28 10:39:11.000000 moptipy-0.9.90/moptipy/algorithms/modules/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4725 2023-07-28 10:39:11.000000 moptipy-0.9.90/moptipy/algorithms/modules/selection.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 11:03:09.278593 moptipy-0.9.90/moptipy/algorithms/modules/selections/
--rw-r--r--   0 runner    (1001) docker     (123)     1569 2023-07-28 10:39:11.000000 moptipy-0.9.90/moptipy/algorithms/modules/selections/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3922 2023-07-28 10:39:11.000000 moptipy-0.9.90/moptipy/algorithms/modules/selections/best.py
--rw-r--r--   0 runner    (1001) docker     (123)    16741 2023-07-28 10:39:11.000000 moptipy-0.9.90/moptipy/algorithms/modules/selections/fitness_proportionate_sus.py
--rw-r--r--   0 runner    (1001) docker     (123)     1936 2023-07-28 10:39:11.000000 moptipy-0.9.90/moptipy/algorithms/modules/selections/random_without_repl.py
--rw-r--r--   0 runner    (1001) docker     (123)     5049 2023-07-28 10:39:11.000000 moptipy-0.9.90/moptipy/algorithms/modules/selections/tournament_with_repl.py
--rw-r--r--   0 runner    (1001) docker     (123)     7708 2023-07-28 10:39:11.000000 moptipy-0.9.90/moptipy/algorithms/modules/selections/tournament_without_repl.py
--rw-r--r--   0 runner    (1001) docker     (123)     9080 2023-07-28 10:39:11.000000 moptipy-0.9.90/moptipy/algorithms/modules/temperature_schedule.py
--rw-r--r--   0 runner    (1001) docker     (123)     2663 2023-07-28 10:39:11.000000 moptipy-0.9.90/moptipy/algorithms/random_sampling.py
--rw-r--r--   0 runner    (1001) docker     (123)     2539 2023-07-28 10:39:11.000000 moptipy-0.9.90/moptipy/algorithms/random_walk.py
--rw-r--r--   0 runner    (1001) docker     (123)     3041 2023-07-28 10:39:11.000000 moptipy-0.9.90/moptipy/algorithms/restarts.py
--rw-r--r--   0 runner    (1001) docker     (123)     2383 2023-07-28 10:39:11.000000 moptipy-0.9.90/moptipy/algorithms/single_random_sample.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 11:03:09.278593 moptipy-0.9.90/moptipy/algorithms/so/
--rw-r--r--   0 runner    (1001) docker     (123)       77 2023-07-28 10:39:11.000000 moptipy-0.9.90/moptipy/algorithms/so/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11249 2023-07-28 10:39:11.000000 moptipy-0.9.90/moptipy/algorithms/so/ea.py
--rw-r--r--   0 runner    (1001) docker     (123)    15618 2023-07-28 10:39:11.000000 moptipy-0.9.90/moptipy/algorithms/so/fea1plus1.py
--rw-r--r--   0 runner    (1001) docker     (123)     4942 2023-07-28 10:39:11.000000 moptipy-0.9.90/moptipy/algorithms/so/fitness.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 11:03:09.278593 moptipy-0.9.90/moptipy/algorithms/so/fitnesses/
--rw-r--r--   0 runner    (1001) docker     (123)      330 2023-07-28 10:39:11.000000 moptipy-0.9.90/moptipy/algorithms/so/fitnesses/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2089 2023-07-28 10:39:11.000000 moptipy-0.9.90/moptipy/algorithms/so/fitnesses/direct.py
--rw-r--r--   0 runner    (1001) docker     (123)    14412 2023-07-28 10:39:11.000000 moptipy-0.9.90/moptipy/algorithms/so/fitnesses/ffa.py
--rw-r--r--   0 runner    (1001) docker     (123)     3677 2023-07-28 10:39:11.000000 moptipy-0.9.90/moptipy/algorithms/so/fitnesses/rank.py
--rw-r--r--   0 runner    (1001) docker     (123)     3661 2023-07-28 10:39:11.000000 moptipy-0.9.90/moptipy/algorithms/so/fitnesses/rank_and_iteration.py
--rw-r--r--   0 runner    (1001) docker     (123)    13406 2023-07-28 10:39:11.000000 moptipy-0.9.90/moptipy/algorithms/so/general_ea.py
--rw-r--r--   0 runner    (1001) docker     (123)    15063 2023-07-28 10:39:11.000000 moptipy-0.9.90/moptipy/algorithms/so/general_ma.py
--rw-r--r--   0 runner    (1001) docker     (123)     5119 2023-07-28 10:39:11.000000 moptipy-0.9.90/moptipy/algorithms/so/greedy_2plus1_ea_mod.py
--rw-r--r--   0 runner    (1001) docker     (123)     4764 2023-07-28 10:39:11.000000 moptipy-0.9.90/moptipy/algorithms/so/hill_climber.py
--rw-r--r--   0 runner    (1001) docker     (123)     4751 2023-07-28 10:39:11.000000 moptipy-0.9.90/moptipy/algorithms/so/hill_climber_with_restarts.py
--rw-r--r--   0 runner    (1001) docker     (123)    12010 2023-07-28 10:39:11.000000 moptipy-0.9.90/moptipy/algorithms/so/ma.py
--rw-r--r--   0 runner    (1001) docker     (123)    10176 2023-07-28 10:39:11.000000 moptipy-0.9.90/moptipy/algorithms/so/marls.py
--rw-r--r--   0 runner    (1001) docker     (123)    17933 2023-07-28 10:39:11.000000 moptipy-0.9.90/moptipy/algorithms/so/ppa.py
--rw-r--r--   0 runner    (1001) docker     (123)     2077 2023-07-28 10:39:11.000000 moptipy-0.9.90/moptipy/algorithms/so/record.py
--rw-r--r--   0 runner    (1001) docker     (123)     5413 2023-07-28 10:39:11.000000 moptipy-0.9.90/moptipy/algorithms/so/rls.py
--rw-r--r--   0 runner    (1001) docker     (123)     6497 2023-07-28 10:39:11.000000 moptipy-0.9.90/moptipy/algorithms/so/simulated_annealing.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 11:03:09.282593 moptipy-0.9.90/moptipy/algorithms/so/vector/
--rw-r--r--   0 runner    (1001) docker     (123)      422 2023-07-28 10:39:11.000000 moptipy-0.9.90/moptipy/algorithms/so/vector/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13842 2023-07-28 10:39:11.000000 moptipy-0.9.90/moptipy/algorithms/so/vector/cmaes_lib.py
--rw-r--r--   0 runner    (1001) docker     (123)     5210 2023-07-28 10:39:11.000000 moptipy-0.9.90/moptipy/algorithms/so/vector/pdfo.py
--rw-r--r--   0 runner    (1001) docker     (123)    14930 2023-07-28 10:39:11.000000 moptipy-0.9.90/moptipy/algorithms/so/vector/scipy.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 11:03:09.282593 moptipy-0.9.90/moptipy/algorithms/so/vector/surrogate/
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-07-28 10:39:11.000000 moptipy-0.9.90/moptipy/algorithms/so/vector/surrogate/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4889 2023-07-28 10:39:11.000000 moptipy-0.9.90/moptipy/algorithms/so/vector/surrogate/_processes.py
--rw-r--r--   0 runner    (1001) docker     (123)    11287 2023-07-28 10:39:11.000000 moptipy-0.9.90/moptipy/algorithms/so/vector/surrogate/rbf_interpolation.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 11:03:09.282593 moptipy-0.9.90/moptipy/api/
--rw-r--r--   0 runner    (1001) docker     (123)     9431 2023-07-28 10:39:11.000000 moptipy-0.9.90/moptipy/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13048 2023-07-28 10:39:11.000000 moptipy-0.9.90/moptipy/api/_mo_process_no_ss.py
--rw-r--r--   0 runner    (1001) docker     (123)     4944 2023-07-28 10:39:11.000000 moptipy-0.9.90/moptipy/api/_mo_process_no_ss_log.py
--rw-r--r--   0 runner    (1001) docker     (123)     7804 2023-07-28 10:39:11.000000 moptipy-0.9.90/moptipy/api/_mo_process_ss.py
--rw-r--r--   0 runner    (1001) docker     (123)     5470 2023-07-28 10:39:11.000000 moptipy-0.9.90/moptipy/api/_mo_process_ss_log.py
--rw-r--r--   0 runner    (1001) docker     (123)    25213 2023-07-28 10:39:11.000000 moptipy-0.9.90/moptipy/api/_process_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     2911 2023-07-28 10:39:11.000000 moptipy-0.9.90/moptipy/api/_process_no_ss.py
--rw-r--r--   0 runner    (1001) docker     (123)     5148 2023-07-28 10:39:11.000000 moptipy-0.9.90/moptipy/api/_process_no_ss_log.py
--rw-r--r--   0 runner    (1001) docker     (123)     6331 2023-07-28 10:39:11.000000 moptipy-0.9.90/moptipy/api/_process_ss.py
--rw-r--r--   0 runner    (1001) docker     (123)     5839 2023-07-28 10:39:11.000000 moptipy-0.9.90/moptipy/api/_process_ss_log.py
--rw-r--r--   0 runner    (1001) docker     (123)     8661 2023-07-28 10:39:11.000000 moptipy-0.9.90/moptipy/api/algorithm.py
--rw-r--r--   0 runner    (1001) docker     (123)     2121 2023-07-28 10:39:11.000000 moptipy-0.9.90/moptipy/api/component.py
--rw-r--r--   0 runner    (1001) docker     (123)     3509 2023-07-28 10:39:11.000000 moptipy-0.9.90/moptipy/api/encoding.py
--rw-r--r--   0 runner    (1001) docker     (123)    15675 2023-07-28 10:39:11.000000 moptipy-0.9.90/moptipy/api/execution.py
--rw-r--r--   0 runner    (1001) docker     (123)    21741 2023-07-28 10:39:11.000000 moptipy-0.9.90/moptipy/api/experiment.py
--rw-r--r--   0 runner    (1001) docker     (123)     7761 2023-07-28 10:39:11.000000 moptipy-0.9.90/moptipy/api/logging.py
--rw-r--r--   0 runner    (1001) docker     (123)     1816 2023-07-28 10:39:11.000000 moptipy-0.9.90/moptipy/api/mo_algorithm.py
--rw-r--r--   0 runner    (1001) docker     (123)     4664 2023-07-28 10:39:11.000000 moptipy-0.9.90/moptipy/api/mo_archive.py
--rw-r--r--   0 runner    (1001) docker     (123)    13483 2023-07-28 10:39:11.000000 moptipy-0.9.90/moptipy/api/mo_execution.py
--rw-r--r--   0 runner    (1001) docker     (123)    13366 2023-07-28 10:39:11.000000 moptipy-0.9.90/moptipy/api/mo_problem.py
--rw-r--r--   0 runner    (1001) docker     (123)     5010 2023-07-28 10:39:11.000000 moptipy-0.9.90/moptipy/api/mo_process.py
--rw-r--r--   0 runner    (1001) docker     (123)     2296 2023-07-28 10:39:11.000000 moptipy-0.9.90/moptipy/api/mo_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     3914 2023-07-28 10:39:11.000000 moptipy-0.9.90/moptipy/api/objective.py
--rw-r--r--   0 runner    (1001) docker     (123)     9671 2023-07-28 10:39:11.000000 moptipy-0.9.90/moptipy/api/operators.py
--rw-r--r--   0 runner    (1001) docker     (123)    23790 2023-07-28 10:39:11.000000 moptipy-0.9.90/moptipy/api/process.py
--rw-r--r--   0 runner    (1001) docker     (123)    10572 2023-07-28 10:39:11.000000 moptipy-0.9.90/moptipy/api/space.py
--rw-r--r--   0 runner    (1001) docker     (123)    26534 2023-07-28 10:39:11.000000 moptipy-0.9.90/moptipy/api/subprocesses.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 11:03:09.286593 moptipy-0.9.90/moptipy/evaluation/
--rw-r--r--   0 runner    (1001) docker     (123)     5612 2023-07-28 10:39:11.000000 moptipy-0.9.90/moptipy/evaluation/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2733 2023-07-28 10:39:11.000000 moptipy-0.9.90/moptipy/evaluation/_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    18666 2023-07-28 10:39:11.000000 moptipy-0.9.90/moptipy/evaluation/axis_ranger.py
--rw-r--r--   0 runner    (1001) docker     (123)     9253 2023-07-28 10:39:11.000000 moptipy-0.9.90/moptipy/evaluation/base.py
--rw-r--r--   0 runner    (1001) docker     (123)    15363 2023-07-28 10:39:11.000000 moptipy-0.9.90/moptipy/evaluation/ecdf.py
--rw-r--r--   0 runner    (1001) docker     (123)    32492 2023-07-28 10:39:11.000000 moptipy-0.9.90/moptipy/evaluation/end_results.py
--rw-r--r--   0 runner    (1001) docker     (123)    52395 2023-07-28 10:39:11.000000 moptipy-0.9.90/moptipy/evaluation/end_statistics.py
--rw-r--r--   0 runner    (1001) docker     (123)    16418 2023-07-28 10:39:11.000000 moptipy-0.9.90/moptipy/evaluation/ert.py
--rw-r--r--   0 runner    (1001) docker     (123)     2898 2023-07-28 10:39:11.000000 moptipy-0.9.90/moptipy/evaluation/ertecdf.py
--rw-r--r--   0 runner    (1001) docker     (123)    10790 2023-07-28 10:39:11.000000 moptipy-0.9.90/moptipy/evaluation/ioh_analyzer.py
--rw-r--r--   0 runner    (1001) docker     (123)    28993 2023-07-28 10:39:11.000000 moptipy-0.9.90/moptipy/evaluation/log_parser.py
--rw-r--r--   0 runner    (1001) docker     (123)    16617 2023-07-28 10:39:11.000000 moptipy-0.9.90/moptipy/evaluation/plot_ecdf.py
--rw-r--r--   0 runner    (1001) docker     (123)    16630 2023-07-28 10:39:11.000000 moptipy-0.9.90/moptipy/evaluation/plot_end_results.py
--rw-r--r--   0 runner    (1001) docker     (123)    16614 2023-07-28 10:39:11.000000 moptipy-0.9.90/moptipy/evaluation/plot_end_statistics_over_parameter.py
--rw-r--r--   0 runner    (1001) docker     (123)    14202 2023-07-28 10:39:11.000000 moptipy-0.9.90/moptipy/evaluation/plot_ert.py
--rw-r--r--   0 runner    (1001) docker     (123)    17812 2023-07-28 10:39:11.000000 moptipy-0.9.90/moptipy/evaluation/plot_progress.py
--rw-r--r--   0 runner    (1001) docker     (123)    16630 2023-07-28 10:39:11.000000 moptipy-0.9.90/moptipy/evaluation/progress.py
--rw-r--r--   0 runner    (1001) docker     (123)    18748 2023-07-28 10:39:11.000000 moptipy-0.9.90/moptipy/evaluation/stat_run.py
--rw-r--r--   0 runner    (1001) docker     (123)    16330 2023-07-28 10:39:11.000000 moptipy-0.9.90/moptipy/evaluation/statistics.py
--rw-r--r--   0 runner    (1001) docker     (123)     9863 2023-07-28 10:39:11.000000 moptipy-0.9.90/moptipy/evaluation/styler.py
--rw-r--r--   0 runner    (1001) docker     (123)    30136 2023-07-28 10:39:11.000000 moptipy-0.9.90/moptipy/evaluation/tabulate_end_results.py
--rw-r--r--   0 runner    (1001) docker     (123)    18068 2023-07-28 10:39:11.000000 moptipy-0.9.90/moptipy/evaluation/tabulate_result_tests.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 11:03:09.286593 moptipy-0.9.90/moptipy/examples/
--rw-r--r--   0 runner    (1001) docker     (123)       53 2023-07-28 10:39:11.000000 moptipy-0.9.90/moptipy/examples/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 11:03:09.286593 moptipy-0.9.90/moptipy/examples/bitstrings/
--rw-r--r--   0 runner    (1001) docker     (123)     1496 2023-07-28 10:39:11.000000 moptipy-0.9.90/moptipy/examples/bitstrings/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2747 2023-07-28 10:39:11.000000 moptipy-0.9.90/moptipy/examples/bitstrings/bitstring_problem.py
--rw-r--r--   0 runner    (1001) docker     (123)     2856 2023-07-28 10:39:11.000000 moptipy-0.9.90/moptipy/examples/bitstrings/ising1d.py
--rw-r--r--   0 runner    (1001) docker     (123)     4199 2023-07-28 10:39:11.000000 moptipy-0.9.90/moptipy/examples/bitstrings/jump.py
--rw-r--r--   0 runner    (1001) docker     (123)     1793 2023-07-28 10:39:11.000000 moptipy-0.9.90/moptipy/examples/bitstrings/leadingones.py
--rw-r--r--   0 runner    (1001) docker     (123)     2230 2023-07-28 10:39:11.000000 moptipy-0.9.90/moptipy/examples/bitstrings/onemax.py
--rw-r--r--   0 runner    (1001) docker     (123)     1707 2023-07-28 10:39:11.000000 moptipy-0.9.90/moptipy/examples/bitstrings/trap.py
--rw-r--r--   0 runner    (1001) docker     (123)    20111 2023-07-28 10:39:11.000000 moptipy-0.9.90/moptipy/examples/bitstrings/w_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     1772 2023-07-28 10:39:11.000000 moptipy-0.9.90/moptipy/examples/bitstrings/zeromax.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 11:03:09.290593 moptipy-0.9.90/moptipy/examples/jssp/
--rw-r--r--   0 runner    (1001) docker     (123)     5588 2023-07-28 10:39:11.000000 moptipy-0.9.90/moptipy/examples/jssp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      270 2023-07-28 10:39:11.000000 moptipy-0.9.90/moptipy/examples/jssp/demo.txt
--rw-r--r--   0 runner    (1001) docker     (123)    12554 2023-07-28 10:39:11.000000 moptipy-0.9.90/moptipy/examples/jssp/demo_examples.py
--rw-r--r--   0 runner    (1001) docker     (123)    32963 2023-07-28 10:39:11.000000 moptipy-0.9.90/moptipy/examples/jssp/evaluation.py
--rw-r--r--   0 runner    (1001) docker     (123)    14957 2023-07-28 10:39:11.000000 moptipy-0.9.90/moptipy/examples/jssp/experiment.py
--rw-r--r--   0 runner    (1001) docker     (123)     4952 2023-07-28 10:39:11.000000 moptipy-0.9.90/moptipy/examples/jssp/gantt.py
--rw-r--r--   0 runner    (1001) docker     (123)    12912 2023-07-28 10:39:11.000000 moptipy-0.9.90/moptipy/examples/jssp/gantt_space.py
--rw-r--r--   0 runner    (1001) docker     (123)    26490 2023-07-28 10:39:11.000000 moptipy-0.9.90/moptipy/examples/jssp/instance.py
--rw-r--r--   0 runner    (1001) docker     (123)    29210 2023-07-28 10:39:11.000000 moptipy-0.9.90/moptipy/examples/jssp/instance_selector.py
--rw-r--r--   0 runner    (1001) docker     (123)   819206 2023-07-28 10:39:11.000000 moptipy-0.9.90/moptipy/examples/jssp/instances.txt
--rw-r--r--   0 runner    (1001) docker     (123)     2263 2023-07-28 10:39:11.000000 moptipy-0.9.90/moptipy/examples/jssp/makespan.py
--rw-r--r--   0 runner    (1001) docker     (123)     7412 2023-07-28 10:39:11.000000 moptipy-0.9.90/moptipy/examples/jssp/ob_encoding.py
--rw-r--r--   0 runner    (1001) docker     (123)    12512 2023-07-28 10:39:11.000000 moptipy-0.9.90/moptipy/examples/jssp/plot_gantt_chart.py
--rw-r--r--   0 runner    (1001) docker     (123)    19016 2023-07-28 10:39:11.000000 moptipy-0.9.90/moptipy/examples/jssp/plots.py
--rw-r--r--   0 runner    (1001) docker     (123)    22178 2023-07-28 10:39:11.000000 moptipy-0.9.90/moptipy/examples/jssp/spaces_sizes.py
--rw-r--r--   0 runner    (1001) docker     (123)     2524 2023-07-28 10:39:11.000000 moptipy-0.9.90/moptipy/examples/jssp/worktime.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 11:03:09.294593 moptipy-0.9.90/moptipy/examples/vectors/
--rw-r--r--   0 runner    (1001) docker     (123)       64 2023-07-28 10:39:11.000000 moptipy-0.9.90/moptipy/examples/vectors/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1947 2023-07-28 10:39:11.000000 moptipy-0.9.90/moptipy/examples/vectors/ackley.py
--rw-r--r--   0 runner    (1001) docker     (123)     1140 2023-07-28 10:39:11.000000 moptipy-0.9.90/moptipy/examples/vectors/sphere.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 11:03:09.294593 moptipy-0.9.90/moptipy/mo/
--rw-r--r--   0 runner    (1001) docker     (123)       67 2023-07-28 10:39:11.000000 moptipy-0.9.90/moptipy/mo/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 11:03:09.294593 moptipy-0.9.90/moptipy/mo/archive/
--rw-r--r--   0 runner    (1001) docker     (123)       68 2023-07-28 10:39:11.000000 moptipy-0.9.90/moptipy/mo/archive/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9662 2023-07-28 10:39:11.000000 moptipy-0.9.90/moptipy/mo/archive/keep_farthest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 11:03:09.294593 moptipy-0.9.90/moptipy/mo/problem/
--rw-r--r--   0 runner    (1001) docker     (123)       77 2023-07-28 10:39:11.000000 moptipy-0.9.90/moptipy/mo/problem/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13784 2023-07-28 10:39:11.000000 moptipy-0.9.90/moptipy/mo/problem/basic_mo_problem.py
--rw-r--r--   0 runner    (1001) docker     (123)    14774 2023-07-28 10:39:11.000000 moptipy-0.9.90/moptipy/mo/problem/weighted_sum.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 11:03:09.294593 moptipy-0.9.90/moptipy/mock/
--rw-r--r--   0 runner    (1001) docker     (123)       67 2023-07-28 10:39:11.000000 moptipy-0.9.90/moptipy/mock/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    34742 2023-07-28 10:39:11.000000 moptipy-0.9.90/moptipy/mock/components.py
--rw-r--r--   0 runner    (1001) docker     (123)    11157 2023-07-28 10:39:11.000000 moptipy-0.9.90/moptipy/mock/end_results.py
--rw-r--r--   0 runner    (1001) docker     (123)     2339 2023-07-28 10:39:11.000000 moptipy-0.9.90/moptipy/mock/mo_problem.py
--rw-r--r--   0 runner    (1001) docker     (123)     8442 2023-07-28 10:39:11.000000 moptipy-0.9.90/moptipy/mock/objective.py
--rw-r--r--   0 runner    (1001) docker     (123)    15121 2023-07-28 10:39:11.000000 moptipy-0.9.90/moptipy/mock/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 11:03:09.294593 moptipy-0.9.90/moptipy/operators/
--rw-r--r--   0 runner    (1001) docker     (123)      611 2023-07-28 10:39:11.000000 moptipy-0.9.90/moptipy/operators/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 11:03:09.298593 moptipy-0.9.90/moptipy/operators/bitstrings/
--rw-r--r--   0 runner    (1001) docker     (123)     1100 2023-07-28 10:39:11.000000 moptipy-0.9.90/moptipy/operators/bitstrings/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      744 2023-07-28 10:39:11.000000 moptipy-0.9.90/moptipy/operators/bitstrings/op0_random.py
--rw-r--r--   0 runner    (1001) docker     (123)      947 2023-07-28 10:39:11.000000 moptipy-0.9.90/moptipy/operators/bitstrings/op1_flip1.py
--rw-r--r--   0 runner    (1001) docker     (123)     3758 2023-07-28 10:39:11.000000 moptipy-0.9.90/moptipy/operators/bitstrings/op1_flip_m.py
--rw-r--r--   0 runner    (1001) docker     (123)     3662 2023-07-28 10:39:11.000000 moptipy-0.9.90/moptipy/operators/bitstrings/op1_m_over_n_flip.py
--rw-r--r--   0 runner    (1001) docker     (123)     4225 2023-07-28 10:39:11.000000 moptipy-0.9.90/moptipy/operators/bitstrings/op2_uniform.py
--rw-r--r--   0 runner    (1001) docker     (123)     3153 2023-07-28 10:39:11.000000 moptipy-0.9.90/moptipy/operators/op0_forward.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 11:03:09.298593 moptipy-0.9.90/moptipy/operators/ordered_choices/
--rw-r--r--   0 runner    (1001) docker     (123)      229 2023-07-28 10:39:11.000000 moptipy-0.9.90/moptipy/operators/ordered_choices/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1914 2023-07-28 10:39:11.000000 moptipy-0.9.90/moptipy/operators/ordered_choices/op0_choose_and_shuffle.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 11:03:09.298593 moptipy-0.9.90/moptipy/operators/permutations/
--rw-r--r--   0 runner    (1001) docker     (123)     2290 2023-07-28 10:39:11.000000 moptipy-0.9.90/moptipy/operators/permutations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1893 2023-07-28 10:39:11.000000 moptipy-0.9.90/moptipy/operators/permutations/op0_shuffle.py
--rw-r--r--   0 runner    (1001) docker     (123)     9893 2023-07-28 10:39:11.000000 moptipy-0.9.90/moptipy/operators/permutations/op1_insert1.py
--rw-r--r--   0 runner    (1001) docker     (123)     5251 2023-07-28 10:39:11.000000 moptipy-0.9.90/moptipy/operators/permutations/op1_swap2.py
--rw-r--r--   0 runner    (1001) docker     (123)    27917 2023-07-28 10:39:11.000000 moptipy-0.9.90/moptipy/operators/permutations/op1_swap_exactly_n.py
--rw-r--r--   0 runner    (1001) docker     (123)     5469 2023-07-28 10:39:11.000000 moptipy-0.9.90/moptipy/operators/permutations/op1_swap_try_n.py
--rw-r--r--   0 runner    (1001) docker     (123)     5348 2023-07-28 10:39:11.000000 moptipy-0.9.90/moptipy/operators/permutations/op1_swapn.py
--rw-r--r--   0 runner    (1001) docker     (123)     6104 2023-07-28 10:39:11.000000 moptipy-0.9.90/moptipy/operators/permutations/op2_gap.py
--rw-r--r--   0 runner    (1001) docker     (123)     6287 2023-07-28 10:39:11.000000 moptipy-0.9.90/moptipy/operators/permutations/op2_ox2.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 11:03:09.298593 moptipy-0.9.90/moptipy/operators/signed_permutations/
--rw-r--r--   0 runner    (1001) docker     (123)      532 2023-07-28 10:39:11.000000 moptipy-0.9.90/moptipy/operators/signed_permutations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2111 2023-07-28 10:39:11.000000 moptipy-0.9.90/moptipy/operators/signed_permutations/op0_shuffle_and_flip.py
--rw-r--r--   0 runner    (1001) docker     (123)     3453 2023-07-28 10:39:11.000000 moptipy-0.9.90/moptipy/operators/signed_permutations/op1_swap_2_or_flip.py
--rw-r--r--   0 runner    (1001) docker     (123)     5370 2023-07-28 10:39:11.000000 moptipy-0.9.90/moptipy/operators/tools.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 11:03:09.298593 moptipy-0.9.90/moptipy/operators/vectors/
--rw-r--r--   0 runner    (1001) docker     (123)       35 2023-07-28 10:39:11.000000 moptipy-0.9.90/moptipy/operators/vectors/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1695 2023-07-28 10:39:11.000000 moptipy-0.9.90/moptipy/operators/vectors/op0_uniform.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 10:39:11.000000 moptipy-0.9.90/moptipy/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 11:03:09.298593 moptipy-0.9.90/moptipy/spaces/
--rw-r--r--   0 runner    (1001) docker     (123)     1678 2023-07-28 10:39:11.000000 moptipy-0.9.90/moptipy/spaces/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2451 2023-07-28 10:39:11.000000 moptipy-0.9.90/moptipy/spaces/bitstrings.py
--rw-r--r--   0 runner    (1001) docker     (123)     5112 2023-07-28 10:39:11.000000 moptipy-0.9.90/moptipy/spaces/intspace.py
--rw-r--r--   0 runner    (1001) docker     (123)     4826 2023-07-28 10:39:11.000000 moptipy-0.9.90/moptipy/spaces/nparrayspace.py
--rw-r--r--   0 runner    (1001) docker     (123)    11154 2023-07-28 10:39:11.000000 moptipy-0.9.90/moptipy/spaces/ordered_choices.py
--rw-r--r--   0 runner    (1001) docker     (123)    10767 2023-07-28 10:39:11.000000 moptipy-0.9.90/moptipy/spaces/permutations.py
--rw-r--r--   0 runner    (1001) docker     (123)    13231 2023-07-28 10:39:11.000000 moptipy-0.9.90/moptipy/spaces/signed_permutations.py
--rw-r--r--   0 runner    (1001) docker     (123)    10649 2023-07-28 10:39:11.000000 moptipy-0.9.90/moptipy/spaces/vectorspace.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 11:03:09.302593 moptipy-0.9.90/moptipy/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      493 2023-07-28 10:39:11.000000 moptipy-0.9.90/moptipy/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10867 2023-07-28 10:39:11.000000 moptipy-0.9.90/moptipy/tests/algorithm.py
--rw-r--r--   0 runner    (1001) docker     (123)     5052 2023-07-28 10:39:11.000000 moptipy-0.9.90/moptipy/tests/component.py
--rw-r--r--   0 runner    (1001) docker     (123)     4294 2023-07-28 10:39:11.000000 moptipy-0.9.90/moptipy/tests/encoding.py
--rw-r--r--   0 runner    (1001) docker     (123)     4397 2023-07-28 10:39:11.000000 moptipy-0.9.90/moptipy/tests/fitness.py
--rw-r--r--   0 runner    (1001) docker     (123)     9686 2023-07-28 10:39:11.000000 moptipy-0.9.90/moptipy/tests/mo_algorithm.py
--rw-r--r--   0 runner    (1001) docker     (123)     7780 2023-07-28 10:39:11.000000 moptipy-0.9.90/moptipy/tests/mo_archive_pruner.py
--rw-r--r--   0 runner    (1001) docker     (123)     7865 2023-07-28 10:39:11.000000 moptipy-0.9.90/moptipy/tests/mo_problem.py
--rw-r--r--   0 runner    (1001) docker     (123)     6360 2023-07-28 10:39:11.000000 moptipy-0.9.90/moptipy/tests/objective.py
--rw-r--r--   0 runner    (1001) docker     (123)    23227 2023-07-28 10:39:11.000000 moptipy-0.9.90/moptipy/tests/on_bitstrings.py
--rw-r--r--   0 runner    (1001) docker     (123)     9276 2023-07-28 10:39:11.000000 moptipy-0.9.90/moptipy/tests/on_jssp.py
--rw-r--r--   0 runner    (1001) docker     (123)     4519 2023-07-28 10:39:11.000000 moptipy-0.9.90/moptipy/tests/on_ordered_choices.py
--rw-r--r--   0 runner    (1001) docker     (123)    10891 2023-07-28 10:39:11.000000 moptipy-0.9.90/moptipy/tests/on_permutations.py
--rw-r--r--   0 runner    (1001) docker     (123)     6552 2023-07-28 10:39:11.000000 moptipy-0.9.90/moptipy/tests/on_signed_permutations.py
--rw-r--r--   0 runner    (1001) docker     (123)     8028 2023-07-28 10:39:11.000000 moptipy-0.9.90/moptipy/tests/on_vectors.py
--rw-r--r--   0 runner    (1001) docker     (123)     3280 2023-07-28 10:39:11.000000 moptipy-0.9.90/moptipy/tests/op0.py
--rw-r--r--   0 runner    (1001) docker     (123)     4017 2023-07-28 10:39:11.000000 moptipy-0.9.90/moptipy/tests/op1.py
--rw-r--r--   0 runner    (1001) docker     (123)     5107 2023-07-28 10:39:11.000000 moptipy-0.9.90/moptipy/tests/op1_with_step_size.py
--rw-r--r--   0 runner    (1001) docker     (123)     4666 2023-07-28 10:39:11.000000 moptipy-0.9.90/moptipy/tests/op2.py
--rw-r--r--   0 runner    (1001) docker     (123)     8870 2023-07-28 10:39:11.000000 moptipy-0.9.90/moptipy/tests/selection.py
--rw-r--r--   0 runner    (1001) docker     (123)     4692 2023-07-28 10:39:11.000000 moptipy-0.9.90/moptipy/tests/space.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 11:03:09.306593 moptipy-0.9.90/moptipy/utils/
--rw-r--r--   0 runner    (1001) docker     (123)       47 2023-07-28 10:39:11.000000 moptipy-0.9.90/moptipy/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      995 2023-07-28 10:39:11.000000 moptipy-0.9.90/moptipy/utils/cache.py
--rw-r--r--   0 runner    (1001) docker     (123)      727 2023-07-28 10:39:11.000000 moptipy-0.9.90/moptipy/utils/console.py
--rw-r--r--   0 runner    (1001) docker     (123)     7454 2023-07-28 10:39:11.000000 moptipy-0.9.90/moptipy/utils/formatted_string.py
--rw-r--r--   0 runner    (1001) docker     (123)     3799 2023-07-28 10:39:11.000000 moptipy-0.9.90/moptipy/utils/help.py
--rw-r--r--   0 runner    (1001) docker     (123)     4861 2023-07-28 10:39:11.000000 moptipy-0.9.90/moptipy/utils/html.py
--rw-r--r--   0 runner    (1001) docker     (123)    12820 2023-07-28 10:39:11.000000 moptipy-0.9.90/moptipy/utils/lang.py
--rw-r--r--   0 runner    (1001) docker     (123)     5269 2023-07-28 10:39:11.000000 moptipy-0.9.90/moptipy/utils/latex.py
--rw-r--r--   0 runner    (1001) docker     (123)    24422 2023-07-28 10:39:11.000000 moptipy-0.9.90/moptipy/utils/logger.py
--rw-r--r--   0 runner    (1001) docker     (123)     4756 2023-07-28 10:39:11.000000 moptipy-0.9.90/moptipy/utils/markdown.py
--rw-r--r--   0 runner    (1001) docker     (123)    17374 2023-07-28 10:39:11.000000 moptipy-0.9.90/moptipy/utils/math.py
--rw-r--r--   0 runner    (1001) docker     (123)    24206 2023-07-28 10:39:11.000000 moptipy-0.9.90/moptipy/utils/nputils.py
--rw-r--r--   0 runner    (1001) docker     (123)    19384 2023-07-28 10:39:11.000000 moptipy-0.9.90/moptipy/utils/number_renderer.py
--rw-r--r--   0 runner    (1001) docker     (123)     9738 2023-07-28 10:39:11.000000 moptipy-0.9.90/moptipy/utils/path.py
--rw-r--r--   0 runner    (1001) docker     (123)    15949 2023-07-28 10:39:11.000000 moptipy-0.9.90/moptipy/utils/plot_defaults.py
--rw-r--r--   0 runner    (1001) docker     (123)    28468 2023-07-28 10:39:11.000000 moptipy-0.9.90/moptipy/utils/plot_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    11740 2023-07-28 10:39:11.000000 moptipy-0.9.90/moptipy/utils/strings.py
--rw-r--r--   0 runner    (1001) docker     (123)    15463 2023-07-28 10:39:11.000000 moptipy-0.9.90/moptipy/utils/sys_info.py
--rw-r--r--   0 runner    (1001) docker     (123)    21203 2023-07-28 10:39:11.000000 moptipy-0.9.90/moptipy/utils/table.py
--rw-r--r--   0 runner    (1001) docker     (123)     4209 2023-07-28 10:39:11.000000 moptipy-0.9.90/moptipy/utils/temp.py
--rw-r--r--   0 runner    (1001) docker     (123)     7943 2023-07-28 10:39:11.000000 moptipy-0.9.90/moptipy/utils/text_format.py
--rw-r--r--   0 runner    (1001) docker     (123)    11078 2023-07-28 10:39:11.000000 moptipy-0.9.90/moptipy/utils/types.py
--rw-r--r--   0 runner    (1001) docker     (123)      162 2023-07-28 10:39:11.000000 moptipy-0.9.90/moptipy/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 11:03:09.274593 moptipy-0.9.90/moptipy.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)   195321 2023-07-28 11:03:09.000000 moptipy-0.9.90/moptipy.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     7685 2023-07-28 11:03:09.000000 moptipy-0.9.90/moptipy.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 11:03:09.000000 moptipy-0.9.90/moptipy.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 11:03:09.000000 moptipy-0.9.90/moptipy.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      149 2023-07-28 11:03:09.000000 moptipy-0.9.90/moptipy.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-07-28 11:03:09.000000 moptipy-0.9.90/moptipy.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       88 2023-07-28 10:39:11.000000 moptipy-0.9.90/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     2531 2023-07-28 11:03:09.306593 moptipy-0.9.90/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1655 2023-07-28 10:39:11.000000 moptipy-0.9.90/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 11:03:09.306593 moptipy-0.9.90/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     2929 2023-07-28 10:39:11.000000 moptipy-0.9.90/tests/test_examples_from_readme_md.py
--rw-r--r--   0 runner    (1001) docker     (123)     1749 2023-07-28 10:39:11.000000 moptipy-0.9.90/tests/test_examples_in_examples_directory.py
--rw-r--r--   0 runner    (1001) docker     (123)    14386 2023-07-28 10:39:11.000000 moptipy-0.9.90/tests/test_links_in_documentation.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 05:02:51.440920 moptipy-0.9.91/
+-rw-r--r--   0 runner    (1001) docker     (123)   195321 2023-07-30 05:02:51.444920 moptipy-0.9.91/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)   186686 2023-07-30 04:38:25.000000 moptipy-0.9.91/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 05:02:51.412920 moptipy-0.9.91/moptipy/
+-rw-r--r--   0 runner    (1001) docker     (123)      914 2023-07-30 04:38:25.000000 moptipy-0.9.91/moptipy/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 05:02:51.412920 moptipy-0.9.91/moptipy/algorithms/
+-rw-r--r--   0 runner    (1001) docker     (123)      644 2023-07-30 04:38:25.000000 moptipy-0.9.91/moptipy/algorithms/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5478 2023-07-30 04:38:25.000000 moptipy-0.9.91/moptipy/algorithms/luby_restarts.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 05:02:51.412920 moptipy-0.9.91/moptipy/algorithms/mo/
+-rw-r--r--   0 runner    (1001) docker     (123)       76 2023-07-30 04:38:25.000000 moptipy-0.9.91/moptipy/algorithms/mo/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2828 2023-07-30 04:38:25.000000 moptipy-0.9.91/moptipy/algorithms/mo/morls.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13469 2023-07-30 04:38:25.000000 moptipy-0.9.91/moptipy/algorithms/mo/nsga2.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 05:02:51.412920 moptipy-0.9.91/moptipy/algorithms/modules/
+-rw-r--r--   0 runner    (1001) docker     (123)       44 2023-07-30 04:38:25.000000 moptipy-0.9.91/moptipy/algorithms/modules/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4725 2023-07-30 04:38:25.000000 moptipy-0.9.91/moptipy/algorithms/modules/selection.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 05:02:51.416920 moptipy-0.9.91/moptipy/algorithms/modules/selections/
+-rw-r--r--   0 runner    (1001) docker     (123)     1569 2023-07-30 04:38:25.000000 moptipy-0.9.91/moptipy/algorithms/modules/selections/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3922 2023-07-30 04:38:25.000000 moptipy-0.9.91/moptipy/algorithms/modules/selections/best.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16741 2023-07-30 04:38:25.000000 moptipy-0.9.91/moptipy/algorithms/modules/selections/fitness_proportionate_sus.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1936 2023-07-30 04:38:25.000000 moptipy-0.9.91/moptipy/algorithms/modules/selections/random_without_repl.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5049 2023-07-30 04:38:25.000000 moptipy-0.9.91/moptipy/algorithms/modules/selections/tournament_with_repl.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7708 2023-07-30 04:38:25.000000 moptipy-0.9.91/moptipy/algorithms/modules/selections/tournament_without_repl.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9080 2023-07-30 04:38:25.000000 moptipy-0.9.91/moptipy/algorithms/modules/temperature_schedule.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2663 2023-07-30 04:38:25.000000 moptipy-0.9.91/moptipy/algorithms/random_sampling.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2539 2023-07-30 04:38:25.000000 moptipy-0.9.91/moptipy/algorithms/random_walk.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3041 2023-07-30 04:38:25.000000 moptipy-0.9.91/moptipy/algorithms/restarts.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2383 2023-07-30 04:38:25.000000 moptipy-0.9.91/moptipy/algorithms/single_random_sample.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 05:02:51.416920 moptipy-0.9.91/moptipy/algorithms/so/
+-rw-r--r--   0 runner    (1001) docker     (123)       77 2023-07-30 04:38:25.000000 moptipy-0.9.91/moptipy/algorithms/so/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11249 2023-07-30 04:38:25.000000 moptipy-0.9.91/moptipy/algorithms/so/ea.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15618 2023-07-30 04:38:25.000000 moptipy-0.9.91/moptipy/algorithms/so/fea1plus1.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4942 2023-07-30 04:38:25.000000 moptipy-0.9.91/moptipy/algorithms/so/fitness.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 05:02:51.416920 moptipy-0.9.91/moptipy/algorithms/so/fitnesses/
+-rw-r--r--   0 runner    (1001) docker     (123)      330 2023-07-30 04:38:25.000000 moptipy-0.9.91/moptipy/algorithms/so/fitnesses/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2089 2023-07-30 04:38:25.000000 moptipy-0.9.91/moptipy/algorithms/so/fitnesses/direct.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14412 2023-07-30 04:38:25.000000 moptipy-0.9.91/moptipy/algorithms/so/fitnesses/ffa.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3677 2023-07-30 04:38:25.000000 moptipy-0.9.91/moptipy/algorithms/so/fitnesses/rank.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3661 2023-07-30 04:38:25.000000 moptipy-0.9.91/moptipy/algorithms/so/fitnesses/rank_and_iteration.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13399 2023-07-30 04:38:25.000000 moptipy-0.9.91/moptipy/algorithms/so/general_ea.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15063 2023-07-30 04:38:25.000000 moptipy-0.9.91/moptipy/algorithms/so/general_ma.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5119 2023-07-30 04:38:25.000000 moptipy-0.9.91/moptipy/algorithms/so/greedy_2plus1_ea_mod.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4764 2023-07-30 04:38:25.000000 moptipy-0.9.91/moptipy/algorithms/so/hill_climber.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4751 2023-07-30 04:38:25.000000 moptipy-0.9.91/moptipy/algorithms/so/hill_climber_with_restarts.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12010 2023-07-30 04:38:25.000000 moptipy-0.9.91/moptipy/algorithms/so/ma.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10176 2023-07-30 04:38:25.000000 moptipy-0.9.91/moptipy/algorithms/so/marls.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17933 2023-07-30 04:38:25.000000 moptipy-0.9.91/moptipy/algorithms/so/ppa.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2077 2023-07-30 04:38:25.000000 moptipy-0.9.91/moptipy/algorithms/so/record.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5413 2023-07-30 04:38:25.000000 moptipy-0.9.91/moptipy/algorithms/so/rls.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6497 2023-07-30 04:38:25.000000 moptipy-0.9.91/moptipy/algorithms/so/simulated_annealing.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 05:02:51.416920 moptipy-0.9.91/moptipy/algorithms/so/vector/
+-rw-r--r--   0 runner    (1001) docker     (123)      422 2023-07-30 04:38:25.000000 moptipy-0.9.91/moptipy/algorithms/so/vector/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13844 2023-07-30 04:38:25.000000 moptipy-0.9.91/moptipy/algorithms/so/vector/cmaes_lib.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5210 2023-07-30 04:38:25.000000 moptipy-0.9.91/moptipy/algorithms/so/vector/pdfo.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14930 2023-07-30 04:38:25.000000 moptipy-0.9.91/moptipy/algorithms/so/vector/scipy.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 05:02:51.420920 moptipy-0.9.91/moptipy/algorithms/so/vector/surrogate/
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-07-30 04:38:25.000000 moptipy-0.9.91/moptipy/algorithms/so/vector/surrogate/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4889 2023-07-30 04:38:25.000000 moptipy-0.9.91/moptipy/algorithms/so/vector/surrogate/_processes.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11287 2023-07-30 04:38:25.000000 moptipy-0.9.91/moptipy/algorithms/so/vector/surrogate/rbf_interpolation.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 05:02:51.420920 moptipy-0.9.91/moptipy/api/
+-rw-r--r--   0 runner    (1001) docker     (123)     9431 2023-07-30 04:38:25.000000 moptipy-0.9.91/moptipy/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13048 2023-07-30 04:38:25.000000 moptipy-0.9.91/moptipy/api/_mo_process_no_ss.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4944 2023-07-30 04:38:25.000000 moptipy-0.9.91/moptipy/api/_mo_process_no_ss_log.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7804 2023-07-30 04:38:25.000000 moptipy-0.9.91/moptipy/api/_mo_process_ss.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5470 2023-07-30 04:38:25.000000 moptipy-0.9.91/moptipy/api/_mo_process_ss_log.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25213 2023-07-30 04:38:25.000000 moptipy-0.9.91/moptipy/api/_process_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2911 2023-07-30 04:38:25.000000 moptipy-0.9.91/moptipy/api/_process_no_ss.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5148 2023-07-30 04:38:25.000000 moptipy-0.9.91/moptipy/api/_process_no_ss_log.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6331 2023-07-30 04:38:25.000000 moptipy-0.9.91/moptipy/api/_process_ss.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5839 2023-07-30 04:38:25.000000 moptipy-0.9.91/moptipy/api/_process_ss_log.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8661 2023-07-30 04:38:25.000000 moptipy-0.9.91/moptipy/api/algorithm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2121 2023-07-30 04:38:25.000000 moptipy-0.9.91/moptipy/api/component.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3509 2023-07-30 04:38:25.000000 moptipy-0.9.91/moptipy/api/encoding.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15675 2023-07-30 04:38:25.000000 moptipy-0.9.91/moptipy/api/execution.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21741 2023-07-30 04:38:25.000000 moptipy-0.9.91/moptipy/api/experiment.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7761 2023-07-30 04:38:25.000000 moptipy-0.9.91/moptipy/api/logging.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1816 2023-07-30 04:38:25.000000 moptipy-0.9.91/moptipy/api/mo_algorithm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4664 2023-07-30 04:38:25.000000 moptipy-0.9.91/moptipy/api/mo_archive.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13483 2023-07-30 04:38:25.000000 moptipy-0.9.91/moptipy/api/mo_execution.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13366 2023-07-30 04:38:25.000000 moptipy-0.9.91/moptipy/api/mo_problem.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5010 2023-07-30 04:38:25.000000 moptipy-0.9.91/moptipy/api/mo_process.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2296 2023-07-30 04:38:25.000000 moptipy-0.9.91/moptipy/api/mo_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3914 2023-07-30 04:38:25.000000 moptipy-0.9.91/moptipy/api/objective.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9671 2023-07-30 04:38:25.000000 moptipy-0.9.91/moptipy/api/operators.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23790 2023-07-30 04:38:25.000000 moptipy-0.9.91/moptipy/api/process.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10572 2023-07-30 04:38:25.000000 moptipy-0.9.91/moptipy/api/space.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26534 2023-07-30 04:38:25.000000 moptipy-0.9.91/moptipy/api/subprocesses.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 05:02:51.424920 moptipy-0.9.91/moptipy/evaluation/
+-rw-r--r--   0 runner    (1001) docker     (123)     5612 2023-07-30 04:38:25.000000 moptipy-0.9.91/moptipy/evaluation/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2733 2023-07-30 04:38:25.000000 moptipy-0.9.91/moptipy/evaluation/_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18666 2023-07-30 04:38:25.000000 moptipy-0.9.91/moptipy/evaluation/axis_ranger.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29593 2023-07-30 04:38:25.000000 moptipy-0.9.91/moptipy/evaluation/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17841 2023-07-30 04:38:25.000000 moptipy-0.9.91/moptipy/evaluation/ecdf.py
+-rw-r--r--   0 runner    (1001) docker     (123)    39653 2023-07-30 04:38:25.000000 moptipy-0.9.91/moptipy/evaluation/end_results.py
+-rw-r--r--   0 runner    (1001) docker     (123)    56172 2023-07-30 04:38:25.000000 moptipy-0.9.91/moptipy/evaluation/end_statistics.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18087 2023-07-30 04:38:25.000000 moptipy-0.9.91/moptipy/evaluation/ert.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2909 2023-07-30 04:38:25.000000 moptipy-0.9.91/moptipy/evaluation/ertecdf.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10790 2023-07-30 04:38:25.000000 moptipy-0.9.91/moptipy/evaluation/ioh_analyzer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30768 2023-07-30 04:38:25.000000 moptipy-0.9.91/moptipy/evaluation/log_parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16617 2023-07-30 04:38:25.000000 moptipy-0.9.91/moptipy/evaluation/plot_ecdf.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16630 2023-07-30 04:38:25.000000 moptipy-0.9.91/moptipy/evaluation/plot_end_results.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16614 2023-07-30 04:38:25.000000 moptipy-0.9.91/moptipy/evaluation/plot_end_statistics_over_parameter.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14202 2023-07-30 04:38:25.000000 moptipy-0.9.91/moptipy/evaluation/plot_ert.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17812 2023-07-30 04:38:25.000000 moptipy-0.9.91/moptipy/evaluation/plot_progress.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17196 2023-07-30 04:38:25.000000 moptipy-0.9.91/moptipy/evaluation/progress.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21325 2023-07-30 04:38:25.000000 moptipy-0.9.91/moptipy/evaluation/stat_run.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16841 2023-07-30 04:38:25.000000 moptipy-0.9.91/moptipy/evaluation/statistics.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9863 2023-07-30 04:38:25.000000 moptipy-0.9.91/moptipy/evaluation/styler.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30136 2023-07-30 04:38:25.000000 moptipy-0.9.91/moptipy/evaluation/tabulate_end_results.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18068 2023-07-30 04:38:25.000000 moptipy-0.9.91/moptipy/evaluation/tabulate_result_tests.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 05:02:51.424920 moptipy-0.9.91/moptipy/examples/
+-rw-r--r--   0 runner    (1001) docker     (123)       53 2023-07-30 04:38:25.000000 moptipy-0.9.91/moptipy/examples/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 05:02:51.428920 moptipy-0.9.91/moptipy/examples/bitstrings/
+-rw-r--r--   0 runner    (1001) docker     (123)     1496 2023-07-30 04:38:25.000000 moptipy-0.9.91/moptipy/examples/bitstrings/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2747 2023-07-30 04:38:25.000000 moptipy-0.9.91/moptipy/examples/bitstrings/bitstring_problem.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2856 2023-07-30 04:38:25.000000 moptipy-0.9.91/moptipy/examples/bitstrings/ising1d.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4199 2023-07-30 04:38:25.000000 moptipy-0.9.91/moptipy/examples/bitstrings/jump.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1793 2023-07-30 04:38:25.000000 moptipy-0.9.91/moptipy/examples/bitstrings/leadingones.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2230 2023-07-30 04:38:25.000000 moptipy-0.9.91/moptipy/examples/bitstrings/onemax.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1707 2023-07-30 04:38:25.000000 moptipy-0.9.91/moptipy/examples/bitstrings/trap.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20111 2023-07-30 04:38:25.000000 moptipy-0.9.91/moptipy/examples/bitstrings/w_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1772 2023-07-30 04:38:25.000000 moptipy-0.9.91/moptipy/examples/bitstrings/zeromax.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 05:02:51.428920 moptipy-0.9.91/moptipy/examples/jssp/
+-rw-r--r--   0 runner    (1001) docker     (123)     5588 2023-07-30 04:38:25.000000 moptipy-0.9.91/moptipy/examples/jssp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      270 2023-07-30 04:38:25.000000 moptipy-0.9.91/moptipy/examples/jssp/demo.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    12554 2023-07-30 04:38:25.000000 moptipy-0.9.91/moptipy/examples/jssp/demo_examples.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32963 2023-07-30 04:38:25.000000 moptipy-0.9.91/moptipy/examples/jssp/evaluation.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14957 2023-07-30 04:38:25.000000 moptipy-0.9.91/moptipy/examples/jssp/experiment.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4952 2023-07-30 04:38:25.000000 moptipy-0.9.91/moptipy/examples/jssp/gantt.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12912 2023-07-30 04:38:25.000000 moptipy-0.9.91/moptipy/examples/jssp/gantt_space.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26490 2023-07-30 04:38:25.000000 moptipy-0.9.91/moptipy/examples/jssp/instance.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29210 2023-07-30 04:38:25.000000 moptipy-0.9.91/moptipy/examples/jssp/instance_selector.py
+-rw-r--r--   0 runner    (1001) docker     (123)   819206 2023-07-30 04:38:25.000000 moptipy-0.9.91/moptipy/examples/jssp/instances.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2263 2023-07-30 04:38:25.000000 moptipy-0.9.91/moptipy/examples/jssp/makespan.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7412 2023-07-30 04:38:25.000000 moptipy-0.9.91/moptipy/examples/jssp/ob_encoding.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12512 2023-07-30 04:38:25.000000 moptipy-0.9.91/moptipy/examples/jssp/plot_gantt_chart.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19016 2023-07-30 04:38:25.000000 moptipy-0.9.91/moptipy/examples/jssp/plots.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22178 2023-07-30 04:38:25.000000 moptipy-0.9.91/moptipy/examples/jssp/spaces_sizes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2524 2023-07-30 04:38:25.000000 moptipy-0.9.91/moptipy/examples/jssp/worktime.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 05:02:51.428920 moptipy-0.9.91/moptipy/examples/vectors/
+-rw-r--r--   0 runner    (1001) docker     (123)       64 2023-07-30 04:38:25.000000 moptipy-0.9.91/moptipy/examples/vectors/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1947 2023-07-30 04:38:25.000000 moptipy-0.9.91/moptipy/examples/vectors/ackley.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1140 2023-07-30 04:38:25.000000 moptipy-0.9.91/moptipy/examples/vectors/sphere.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 05:02:51.428920 moptipy-0.9.91/moptipy/mo/
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2023-07-30 04:38:25.000000 moptipy-0.9.91/moptipy/mo/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 05:02:51.432920 moptipy-0.9.91/moptipy/mo/archive/
+-rw-r--r--   0 runner    (1001) docker     (123)       68 2023-07-30 04:38:25.000000 moptipy-0.9.91/moptipy/mo/archive/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9662 2023-07-30 04:38:25.000000 moptipy-0.9.91/moptipy/mo/archive/keep_farthest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 05:02:51.432920 moptipy-0.9.91/moptipy/mo/problem/
+-rw-r--r--   0 runner    (1001) docker     (123)       77 2023-07-30 04:38:25.000000 moptipy-0.9.91/moptipy/mo/problem/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13784 2023-07-30 04:38:25.000000 moptipy-0.9.91/moptipy/mo/problem/basic_mo_problem.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14774 2023-07-30 04:38:25.000000 moptipy-0.9.91/moptipy/mo/problem/weighted_sum.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 05:02:51.432920 moptipy-0.9.91/moptipy/mock/
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2023-07-30 04:38:25.000000 moptipy-0.9.91/moptipy/mock/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    34741 2023-07-30 04:38:25.000000 moptipy-0.9.91/moptipy/mock/components.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11346 2023-07-30 04:38:25.000000 moptipy-0.9.91/moptipy/mock/end_results.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2339 2023-07-30 04:38:25.000000 moptipy-0.9.91/moptipy/mock/mo_problem.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8442 2023-07-30 04:38:25.000000 moptipy-0.9.91/moptipy/mock/objective.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15121 2023-07-30 04:38:25.000000 moptipy-0.9.91/moptipy/mock/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 05:02:51.432920 moptipy-0.9.91/moptipy/operators/
+-rw-r--r--   0 runner    (1001) docker     (123)      611 2023-07-30 04:38:25.000000 moptipy-0.9.91/moptipy/operators/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 05:02:51.432920 moptipy-0.9.91/moptipy/operators/bitstrings/
+-rw-r--r--   0 runner    (1001) docker     (123)     1100 2023-07-30 04:38:25.000000 moptipy-0.9.91/moptipy/operators/bitstrings/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      744 2023-07-30 04:38:25.000000 moptipy-0.9.91/moptipy/operators/bitstrings/op0_random.py
+-rw-r--r--   0 runner    (1001) docker     (123)      947 2023-07-30 04:38:25.000000 moptipy-0.9.91/moptipy/operators/bitstrings/op1_flip1.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3758 2023-07-30 04:38:25.000000 moptipy-0.9.91/moptipy/operators/bitstrings/op1_flip_m.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3662 2023-07-30 04:38:25.000000 moptipy-0.9.91/moptipy/operators/bitstrings/op1_m_over_n_flip.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4225 2023-07-30 04:38:25.000000 moptipy-0.9.91/moptipy/operators/bitstrings/op2_uniform.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3153 2023-07-30 04:38:25.000000 moptipy-0.9.91/moptipy/operators/op0_forward.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 05:02:51.432920 moptipy-0.9.91/moptipy/operators/ordered_choices/
+-rw-r--r--   0 runner    (1001) docker     (123)      229 2023-07-30 04:38:25.000000 moptipy-0.9.91/moptipy/operators/ordered_choices/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1914 2023-07-30 04:38:25.000000 moptipy-0.9.91/moptipy/operators/ordered_choices/op0_choose_and_shuffle.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 05:02:51.432920 moptipy-0.9.91/moptipy/operators/permutations/
+-rw-r--r--   0 runner    (1001) docker     (123)     2290 2023-07-30 04:38:25.000000 moptipy-0.9.91/moptipy/operators/permutations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1893 2023-07-30 04:38:25.000000 moptipy-0.9.91/moptipy/operators/permutations/op0_shuffle.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9893 2023-07-30 04:38:25.000000 moptipy-0.9.91/moptipy/operators/permutations/op1_insert1.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5251 2023-07-30 04:38:25.000000 moptipy-0.9.91/moptipy/operators/permutations/op1_swap2.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27917 2023-07-30 04:38:25.000000 moptipy-0.9.91/moptipy/operators/permutations/op1_swap_exactly_n.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5469 2023-07-30 04:38:25.000000 moptipy-0.9.91/moptipy/operators/permutations/op1_swap_try_n.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5348 2023-07-30 04:38:25.000000 moptipy-0.9.91/moptipy/operators/permutations/op1_swapn.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6104 2023-07-30 04:38:25.000000 moptipy-0.9.91/moptipy/operators/permutations/op2_gap.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6287 2023-07-30 04:38:25.000000 moptipy-0.9.91/moptipy/operators/permutations/op2_ox2.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 05:02:51.436920 moptipy-0.9.91/moptipy/operators/signed_permutations/
+-rw-r--r--   0 runner    (1001) docker     (123)      532 2023-07-30 04:38:25.000000 moptipy-0.9.91/moptipy/operators/signed_permutations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2111 2023-07-30 04:38:25.000000 moptipy-0.9.91/moptipy/operators/signed_permutations/op0_shuffle_and_flip.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3453 2023-07-30 04:38:25.000000 moptipy-0.9.91/moptipy/operators/signed_permutations/op1_swap_2_or_flip.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5370 2023-07-30 04:38:25.000000 moptipy-0.9.91/moptipy/operators/tools.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 05:02:51.436920 moptipy-0.9.91/moptipy/operators/vectors/
+-rw-r--r--   0 runner    (1001) docker     (123)       35 2023-07-30 04:38:25.000000 moptipy-0.9.91/moptipy/operators/vectors/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1695 2023-07-30 04:38:25.000000 moptipy-0.9.91/moptipy/operators/vectors/op0_uniform.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-30 04:38:25.000000 moptipy-0.9.91/moptipy/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 05:02:51.436920 moptipy-0.9.91/moptipy/spaces/
+-rw-r--r--   0 runner    (1001) docker     (123)     1678 2023-07-30 04:38:25.000000 moptipy-0.9.91/moptipy/spaces/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2451 2023-07-30 04:38:25.000000 moptipy-0.9.91/moptipy/spaces/bitstrings.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5112 2023-07-30 04:38:25.000000 moptipy-0.9.91/moptipy/spaces/intspace.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4826 2023-07-30 04:38:25.000000 moptipy-0.9.91/moptipy/spaces/nparrayspace.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11154 2023-07-30 04:38:25.000000 moptipy-0.9.91/moptipy/spaces/ordered_choices.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10767 2023-07-30 04:38:25.000000 moptipy-0.9.91/moptipy/spaces/permutations.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13231 2023-07-30 04:38:25.000000 moptipy-0.9.91/moptipy/spaces/signed_permutations.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10649 2023-07-30 04:38:25.000000 moptipy-0.9.91/moptipy/spaces/vectorspace.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 05:02:51.440920 moptipy-0.9.91/moptipy/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      493 2023-07-30 04:38:25.000000 moptipy-0.9.91/moptipy/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10867 2023-07-30 04:38:25.000000 moptipy-0.9.91/moptipy/tests/algorithm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5052 2023-07-30 04:38:25.000000 moptipy-0.9.91/moptipy/tests/component.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4294 2023-07-30 04:38:25.000000 moptipy-0.9.91/moptipy/tests/encoding.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4397 2023-07-30 04:38:25.000000 moptipy-0.9.91/moptipy/tests/fitness.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9686 2023-07-30 04:38:25.000000 moptipy-0.9.91/moptipy/tests/mo_algorithm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7780 2023-07-30 04:38:25.000000 moptipy-0.9.91/moptipy/tests/mo_archive_pruner.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7865 2023-07-30 04:38:25.000000 moptipy-0.9.91/moptipy/tests/mo_problem.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6360 2023-07-30 04:38:25.000000 moptipy-0.9.91/moptipy/tests/objective.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23227 2023-07-30 04:38:25.000000 moptipy-0.9.91/moptipy/tests/on_bitstrings.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9276 2023-07-30 04:38:25.000000 moptipy-0.9.91/moptipy/tests/on_jssp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4519 2023-07-30 04:38:25.000000 moptipy-0.9.91/moptipy/tests/on_ordered_choices.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10891 2023-07-30 04:38:25.000000 moptipy-0.9.91/moptipy/tests/on_permutations.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6552 2023-07-30 04:38:25.000000 moptipy-0.9.91/moptipy/tests/on_signed_permutations.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8028 2023-07-30 04:38:25.000000 moptipy-0.9.91/moptipy/tests/on_vectors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3280 2023-07-30 04:38:25.000000 moptipy-0.9.91/moptipy/tests/op0.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4017 2023-07-30 04:38:25.000000 moptipy-0.9.91/moptipy/tests/op1.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5107 2023-07-30 04:38:25.000000 moptipy-0.9.91/moptipy/tests/op1_with_step_size.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4666 2023-07-30 04:38:25.000000 moptipy-0.9.91/moptipy/tests/op2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8870 2023-07-30 04:38:25.000000 moptipy-0.9.91/moptipy/tests/selection.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4692 2023-07-30 04:38:25.000000 moptipy-0.9.91/moptipy/tests/space.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 05:02:51.440920 moptipy-0.9.91/moptipy/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-07-30 04:38:25.000000 moptipy-0.9.91/moptipy/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      995 2023-07-30 04:38:25.000000 moptipy-0.9.91/moptipy/utils/cache.py
+-rw-r--r--   0 runner    (1001) docker     (123)      727 2023-07-30 04:38:25.000000 moptipy-0.9.91/moptipy/utils/console.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7454 2023-07-30 04:38:25.000000 moptipy-0.9.91/moptipy/utils/formatted_string.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3799 2023-07-30 04:38:25.000000 moptipy-0.9.91/moptipy/utils/help.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4861 2023-07-30 04:38:25.000000 moptipy-0.9.91/moptipy/utils/html.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12820 2023-07-30 04:38:25.000000 moptipy-0.9.91/moptipy/utils/lang.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5269 2023-07-30 04:38:25.000000 moptipy-0.9.91/moptipy/utils/latex.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24426 2023-07-30 04:38:25.000000 moptipy-0.9.91/moptipy/utils/logger.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4756 2023-07-30 04:38:25.000000 moptipy-0.9.91/moptipy/utils/markdown.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17374 2023-07-30 04:38:25.000000 moptipy-0.9.91/moptipy/utils/math.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24206 2023-07-30 04:38:25.000000 moptipy-0.9.91/moptipy/utils/nputils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19384 2023-07-30 04:38:25.000000 moptipy-0.9.91/moptipy/utils/number_renderer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9738 2023-07-30 04:38:25.000000 moptipy-0.9.91/moptipy/utils/path.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15949 2023-07-30 04:38:25.000000 moptipy-0.9.91/moptipy/utils/plot_defaults.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28468 2023-07-30 04:38:25.000000 moptipy-0.9.91/moptipy/utils/plot_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11740 2023-07-30 04:38:25.000000 moptipy-0.9.91/moptipy/utils/strings.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15463 2023-07-30 04:38:25.000000 moptipy-0.9.91/moptipy/utils/sys_info.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21203 2023-07-30 04:38:25.000000 moptipy-0.9.91/moptipy/utils/table.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4209 2023-07-30 04:38:25.000000 moptipy-0.9.91/moptipy/utils/temp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7943 2023-07-30 04:38:25.000000 moptipy-0.9.91/moptipy/utils/text_format.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11078 2023-07-30 04:38:25.000000 moptipy-0.9.91/moptipy/utils/types.py
+-rw-r--r--   0 runner    (1001) docker     (123)      162 2023-07-30 04:38:25.000000 moptipy-0.9.91/moptipy/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 05:02:51.412920 moptipy-0.9.91/moptipy.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)   195321 2023-07-30 05:02:51.000000 moptipy-0.9.91/moptipy.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     7685 2023-07-30 05:02:51.000000 moptipy-0.9.91/moptipy.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-30 05:02:51.000000 moptipy-0.9.91/moptipy.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-30 05:02:51.000000 moptipy-0.9.91/moptipy.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      149 2023-07-30 05:02:51.000000 moptipy-0.9.91/moptipy.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-07-30 05:02:51.000000 moptipy-0.9.91/moptipy.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       88 2023-07-30 04:38:25.000000 moptipy-0.9.91/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     2531 2023-07-30 05:02:51.444920 moptipy-0.9.91/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1655 2023-07-30 04:38:25.000000 moptipy-0.9.91/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 05:02:51.440920 moptipy-0.9.91/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     2929 2023-07-30 04:38:25.000000 moptipy-0.9.91/tests/test_examples_from_readme_md.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1749 2023-07-30 04:38:25.000000 moptipy-0.9.91/tests/test_examples_in_examples_directory.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14386 2023-07-30 04:38:25.000000 moptipy-0.9.91/tests/test_links_in_documentation.py
```

### Comparing `moptipy-0.9.90/PKG-INFO` & `moptipy-0.9.91/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 00000000: 4d65 7461 6461 7461 2d56 6572 7369 6f6e  Metadata-Version
 00000010: 3a20 322e 310a 4e61 6d65 3a20 6d6f 7074  : 2.1.Name: mopt
 00000020: 6970 790a 5665 7273 696f 6e3a 2030 2e39  ipy.Version: 0.9
-00000030: 2e39 300a 5375 6d6d 6172 793a 2041 2070  .90.Summary: A p
+00000030: 2e39 310a 5375 6d6d 6172 793a 2041 2070  .91.Summary: A p
 00000040: 6163 6b61 6765 2066 6f72 206d 6574 6168  ackage for metah
 00000050: 6575 7269 7374 6963 206f 7074 696d 697a  euristic optimiz
 00000060: 6174 696f 6e20 696e 2050 7974 686f 6e2e  ation in Python.
 00000070: 0a48 6f6d 652d 7061 6765 3a20 6874 7470  .Home-page: http
 00000080: 733a 2f2f 7468 6f6d 6173 7765 6973 652e  s://thomasweise.
 00000090: 6769 7468 7562 2e69 6f2f 6d6f 7074 6970  github.io/moptip
 000000a0: 790a 4175 7468 6f72 3a20 5468 6f6d 6173  y.Author: Thomas
```

### Comparing `moptipy-0.9.90/README.md` & `moptipy-0.9.91/README.md`

 * *Files identical despite different names*

### Comparing `moptipy-0.9.90/moptipy/__init__.py` & `moptipy-0.9.91/moptipy/__init__.py`

 * *Files identical despite different names*

### Comparing `moptipy-0.9.90/moptipy/algorithms/__init__.py` & `moptipy-0.9.91/moptipy/algorithms/__init__.py`

 * *Files identical despite different names*

### Comparing `moptipy-0.9.90/moptipy/algorithms/luby_restarts.py` & `moptipy-0.9.91/moptipy/algorithms/luby_restarts.py`

 * *Files identical despite different names*

### Comparing `moptipy-0.9.90/moptipy/algorithms/mo/morls.py` & `moptipy-0.9.91/moptipy/algorithms/mo/morls.py`

 * *Files identical despite different names*

### Comparing `moptipy-0.9.90/moptipy/algorithms/mo/nsga2.py` & `moptipy-0.9.91/moptipy/algorithms/mo/nsga2.py`

 * *Files identical despite different names*

### Comparing `moptipy-0.9.90/moptipy/algorithms/modules/selection.py` & `moptipy-0.9.91/moptipy/algorithms/modules/selection.py`

 * *Files identical despite different names*

### Comparing `moptipy-0.9.90/moptipy/algorithms/modules/selections/__init__.py` & `moptipy-0.9.91/moptipy/algorithms/modules/selections/__init__.py`

 * *Files identical despite different names*

### Comparing `moptipy-0.9.90/moptipy/algorithms/modules/selections/best.py` & `moptipy-0.9.91/moptipy/algorithms/modules/selections/best.py`

 * *Files identical despite different names*

### Comparing `moptipy-0.9.90/moptipy/algorithms/modules/selections/fitness_proportionate_sus.py` & `moptipy-0.9.91/moptipy/algorithms/modules/selections/fitness_proportionate_sus.py`

 * *Files identical despite different names*

### Comparing `moptipy-0.9.90/moptipy/algorithms/modules/selections/random_without_repl.py` & `moptipy-0.9.91/moptipy/algorithms/modules/selections/random_without_repl.py`

 * *Files identical despite different names*

### Comparing `moptipy-0.9.90/moptipy/algorithms/modules/selections/tournament_with_repl.py` & `moptipy-0.9.91/moptipy/algorithms/modules/selections/tournament_with_repl.py`

 * *Files identical despite different names*

### Comparing `moptipy-0.9.90/moptipy/algorithms/modules/selections/tournament_without_repl.py` & `moptipy-0.9.91/moptipy/algorithms/modules/selections/tournament_without_repl.py`

 * *Files identical despite different names*

### Comparing `moptipy-0.9.90/moptipy/algorithms/modules/temperature_schedule.py` & `moptipy-0.9.91/moptipy/algorithms/modules/temperature_schedule.py`

 * *Files identical despite different names*

### Comparing `moptipy-0.9.90/moptipy/algorithms/random_sampling.py` & `moptipy-0.9.91/moptipy/algorithms/random_sampling.py`

 * *Files identical despite different names*

### Comparing `moptipy-0.9.90/moptipy/algorithms/random_walk.py` & `moptipy-0.9.91/moptipy/algorithms/random_walk.py`

 * *Files identical despite different names*

### Comparing `moptipy-0.9.90/moptipy/algorithms/restarts.py` & `moptipy-0.9.91/moptipy/algorithms/restarts.py`

 * *Files identical despite different names*

### Comparing `moptipy-0.9.90/moptipy/algorithms/single_random_sample.py` & `moptipy-0.9.91/moptipy/algorithms/single_random_sample.py`

 * *Files identical despite different names*

### Comparing `moptipy-0.9.90/moptipy/algorithms/so/ea.py` & `moptipy-0.9.91/moptipy/algorithms/so/ea.py`

 * *Files identical despite different names*

### Comparing `moptipy-0.9.90/moptipy/algorithms/so/fea1plus1.py` & `moptipy-0.9.91/moptipy/algorithms/so/fea1plus1.py`

 * *Files identical despite different names*

### Comparing `moptipy-0.9.90/moptipy/algorithms/so/fitness.py` & `moptipy-0.9.91/moptipy/algorithms/so/fitness.py`

 * *Files identical despite different names*

### Comparing `moptipy-0.9.90/moptipy/algorithms/so/fitnesses/direct.py` & `moptipy-0.9.91/moptipy/algorithms/so/fitnesses/direct.py`

 * *Files identical despite different names*

### Comparing `moptipy-0.9.90/moptipy/algorithms/so/fitnesses/ffa.py` & `moptipy-0.9.91/moptipy/algorithms/so/fitnesses/ffa.py`

 * *Files identical despite different names*

### Comparing `moptipy-0.9.90/moptipy/algorithms/so/fitnesses/rank.py` & `moptipy-0.9.91/moptipy/algorithms/so/fitnesses/rank.py`

 * *Files identical despite different names*

### Comparing `moptipy-0.9.90/moptipy/algorithms/so/fitnesses/rank_and_iteration.py` & `moptipy-0.9.91/moptipy/algorithms/so/fitnesses/rank_and_iteration.py`

 * *Files identical despite different names*

### Comparing `moptipy-0.9.90/moptipy/algorithms/so/general_ea.py` & `moptipy-0.9.91/moptipy/algorithms/so/general_ea.py`

 * *Files 0% similar despite different names*

```diff
@@ -64,15 +64,15 @@
 from moptipy.api.operators import Op0, Op1, Op2
 from moptipy.api.process import Process
 from moptipy.utils.logger import KeyValueLogSection
 from moptipy.utils.strings import PART_SEPARATOR
 
 
 class _Record(FRecord):
-    """Same as :class:`FRecord`, but with a secret selection marker."""
+    """Same as `FRecord`, but with a secret selection marker."""
 
     def __init__(self, x, f: int | float, selected: bool = False):
         """
         Create the record.
 
         :param x: the data structure for a point in the search space
         :param f: the corresponding objective value
```

### Comparing `moptipy-0.9.90/moptipy/algorithms/so/general_ma.py` & `moptipy-0.9.91/moptipy/algorithms/so/general_ma.py`

 * *Files identical despite different names*

### Comparing `moptipy-0.9.90/moptipy/algorithms/so/greedy_2plus1_ea_mod.py` & `moptipy-0.9.91/moptipy/algorithms/so/greedy_2plus1_ea_mod.py`

 * *Files identical despite different names*

### Comparing `moptipy-0.9.90/moptipy/algorithms/so/hill_climber.py` & `moptipy-0.9.91/moptipy/algorithms/so/hill_climber.py`

 * *Files identical despite different names*

### Comparing `moptipy-0.9.90/moptipy/algorithms/so/hill_climber_with_restarts.py` & `moptipy-0.9.91/moptipy/algorithms/so/hill_climber_with_restarts.py`

 * *Files identical despite different names*

### Comparing `moptipy-0.9.90/moptipy/algorithms/so/ma.py` & `moptipy-0.9.91/moptipy/algorithms/so/ma.py`

 * *Files identical despite different names*

### Comparing `moptipy-0.9.90/moptipy/algorithms/so/marls.py` & `moptipy-0.9.91/moptipy/algorithms/so/marls.py`

 * *Files identical despite different names*

### Comparing `moptipy-0.9.90/moptipy/algorithms/so/ppa.py` & `moptipy-0.9.91/moptipy/algorithms/so/ppa.py`

 * *Files identical despite different names*

### Comparing `moptipy-0.9.90/moptipy/algorithms/so/record.py` & `moptipy-0.9.91/moptipy/algorithms/so/record.py`

 * *Files identical despite different names*

### Comparing `moptipy-0.9.90/moptipy/algorithms/so/rls.py` & `moptipy-0.9.91/moptipy/algorithms/so/rls.py`

 * *Files identical despite different names*

### Comparing `moptipy-0.9.90/moptipy/algorithms/so/simulated_annealing.py` & `moptipy-0.9.91/moptipy/algorithms/so/simulated_annealing.py`

 * *Files identical despite different names*

### Comparing `moptipy-0.9.90/moptipy/algorithms/so/vector/cmaes_lib.py` & `moptipy-0.9.91/moptipy/algorithms/so/vector/cmaes_lib.py`

 * *Files 0% similar despite different names*

```diff
@@ -64,15 +64,15 @@
 
     :param cma: the algorithm instance
     :param f: the objective function
     :param should_terminate: the termination criterion
     :param solutions: the internal list to store the solutions
     :param run_criterion: the stopper for a run
     :returns: the number of consumed FEs if the run was terminated by
-      `run_criterion`, `-1` otherwise
+        `run_criterion`, `-1` otherwise
     """
     fes: int = 0
     pop_size: Final[int] = cma.population_size
 
     # now we load a lot of fast call function pointers
     ask: Final[Callable[[], np.ndarray]] = cma.ask
     append: Final[Callable[[
```

### Comparing `moptipy-0.9.90/moptipy/algorithms/so/vector/pdfo.py` & `moptipy-0.9.91/moptipy/algorithms/so/vector/pdfo.py`

 * *Files identical despite different names*

### Comparing `moptipy-0.9.90/moptipy/algorithms/so/vector/scipy.py` & `moptipy-0.9.91/moptipy/algorithms/so/vector/scipy.py`

 * *Files identical despite different names*

### Comparing `moptipy-0.9.90/moptipy/algorithms/so/vector/surrogate/_processes.py` & `moptipy-0.9.91/moptipy/algorithms/so/vector/surrogate/_processes.py`

 * *Files identical despite different names*

### Comparing `moptipy-0.9.90/moptipy/algorithms/so/vector/surrogate/rbf_interpolation.py` & `moptipy-0.9.91/moptipy/algorithms/so/vector/surrogate/rbf_interpolation.py`

 * *Files identical despite different names*

### Comparing `moptipy-0.9.90/moptipy/api/__init__.py` & `moptipy-0.9.91/moptipy/api/__init__.py`

 * *Files identical despite different names*

### Comparing `moptipy-0.9.90/moptipy/api/_mo_process_no_ss.py` & `moptipy-0.9.91/moptipy/api/_mo_process_no_ss.py`

 * *Files identical despite different names*

### Comparing `moptipy-0.9.90/moptipy/api/_mo_process_no_ss_log.py` & `moptipy-0.9.91/moptipy/api/_mo_process_no_ss_log.py`

 * *Files identical despite different names*

### Comparing `moptipy-0.9.90/moptipy/api/_mo_process_ss.py` & `moptipy-0.9.91/moptipy/api/_mo_process_ss.py`

 * *Files identical despite different names*

### Comparing `moptipy-0.9.90/moptipy/api/_mo_process_ss_log.py` & `moptipy-0.9.91/moptipy/api/_mo_process_ss_log.py`

 * *Files identical despite different names*

### Comparing `moptipy-0.9.90/moptipy/api/_process_base.py` & `moptipy-0.9.91/moptipy/api/_process_base.py`

 * *Files identical despite different names*

### Comparing `moptipy-0.9.90/moptipy/api/_process_no_ss.py` & `moptipy-0.9.91/moptipy/api/_process_no_ss.py`

 * *Files identical despite different names*

### Comparing `moptipy-0.9.90/moptipy/api/_process_no_ss_log.py` & `moptipy-0.9.91/moptipy/api/_process_no_ss_log.py`

 * *Files identical despite different names*

### Comparing `moptipy-0.9.90/moptipy/api/_process_ss.py` & `moptipy-0.9.91/moptipy/api/_process_ss.py`

 * *Files identical despite different names*

### Comparing `moptipy-0.9.90/moptipy/api/_process_ss_log.py` & `moptipy-0.9.91/moptipy/api/_process_ss_log.py`

 * *Files identical despite different names*

### Comparing `moptipy-0.9.90/moptipy/api/algorithm.py` & `moptipy-0.9.91/moptipy/api/algorithm.py`

 * *Files identical despite different names*

### Comparing `moptipy-0.9.90/moptipy/api/component.py` & `moptipy-0.9.91/moptipy/api/component.py`

 * *Files identical despite different names*

### Comparing `moptipy-0.9.90/moptipy/api/encoding.py` & `moptipy-0.9.91/moptipy/api/encoding.py`

 * *Files identical despite different names*

### Comparing `moptipy-0.9.90/moptipy/api/execution.py` & `moptipy-0.9.91/moptipy/api/execution.py`

 * *Files identical despite different names*

### Comparing `moptipy-0.9.90/moptipy/api/experiment.py` & `moptipy-0.9.91/moptipy/api/experiment.py`

 * *Files identical despite different names*

### Comparing `moptipy-0.9.90/moptipy/api/logging.py` & `moptipy-0.9.91/moptipy/api/logging.py`

 * *Files identical despite different names*

### Comparing `moptipy-0.9.90/moptipy/api/mo_algorithm.py` & `moptipy-0.9.91/moptipy/api/mo_algorithm.py`

 * *Files identical despite different names*

### Comparing `moptipy-0.9.90/moptipy/api/mo_archive.py` & `moptipy-0.9.91/moptipy/api/mo_archive.py`

 * *Files identical despite different names*

### Comparing `moptipy-0.9.90/moptipy/api/mo_execution.py` & `moptipy-0.9.91/moptipy/api/mo_execution.py`

 * *Files identical despite different names*

### Comparing `moptipy-0.9.90/moptipy/api/mo_problem.py` & `moptipy-0.9.91/moptipy/api/mo_problem.py`

 * *Files identical despite different names*

### Comparing `moptipy-0.9.90/moptipy/api/mo_process.py` & `moptipy-0.9.91/moptipy/api/mo_process.py`

 * *Files identical despite different names*

### Comparing `moptipy-0.9.90/moptipy/api/mo_utils.py` & `moptipy-0.9.91/moptipy/api/mo_utils.py`

 * *Files identical despite different names*

### Comparing `moptipy-0.9.90/moptipy/api/objective.py` & `moptipy-0.9.91/moptipy/api/objective.py`

 * *Files identical despite different names*

### Comparing `moptipy-0.9.90/moptipy/api/operators.py` & `moptipy-0.9.91/moptipy/api/operators.py`

 * *Files identical despite different names*

### Comparing `moptipy-0.9.90/moptipy/api/process.py` & `moptipy-0.9.91/moptipy/api/process.py`

 * *Files identical despite different names*

### Comparing `moptipy-0.9.90/moptipy/api/space.py` & `moptipy-0.9.91/moptipy/api/space.py`

 * *Files identical despite different names*

### Comparing `moptipy-0.9.90/moptipy/api/subprocesses.py` & `moptipy-0.9.91/moptipy/api/subprocesses.py`

 * *Files identical despite different names*

### Comparing `moptipy-0.9.90/moptipy/evaluation/__init__.py` & `moptipy-0.9.91/moptipy/evaluation/__init__.py`

 * *Files identical despite different names*

### Comparing `moptipy-0.9.90/moptipy/evaluation/_utils.py` & `moptipy-0.9.91/moptipy/evaluation/_utils.py`

 * *Files identical despite different names*

### Comparing `moptipy-0.9.90/moptipy/evaluation/axis_ranger.py` & `moptipy-0.9.91/moptipy/evaluation/axis_ranger.py`

 * *Files identical despite different names*

### Comparing `moptipy-0.9.90/moptipy/evaluation/base.py` & `moptipy-0.9.91/moptipy/tests/on_jssp.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,294 +1,236 @@
-"""Some internal helper functions and base classes."""
+"""Perform tests on the Job Shop Scheduling Problem."""
 
-from dataclasses import dataclass
-from math import inf
-from typing import Any, Final
-
-from moptipy.utils.nputils import rand_seed_check
-from moptipy.utils.strings import sanitize_name
-from moptipy.utils.types import check_int_range, type_error
-
-#: The key for the total number of runs.
-KEY_N: Final[str] = "n"
-
-#: The unit of the time axis if time is measured in milliseconds.
-TIME_UNIT_MILLIS: Final[str] = "ms"
-#: The unit of the time axis of time is measured in FEs
-TIME_UNIT_FES: Final[str] = "FEs"
-
-#: The name of the raw objective values data.
-F_NAME_RAW: Final[str] = "plainF"
-#: The name of the scaled objective values data.
-F_NAME_SCALED: Final[str] = "scaledF"
-#: The name of the normalized objective values data.
-F_NAME_NORMALIZED: Final[str] = "normalizedF"
-
-
-def check_time_unit(time_unit: Any) -> str:
-    """
-    Check that the time unit is OK.
-
-    :param time_unit: the time unit
-    :return: the time unit string
-
-    >>> check_time_unit("FEs")
-    'FEs'
-    >>> check_time_unit("ms")
-    'ms'
-    >>> try:
-    ...     check_time_unit(1)
-    ... except TypeError as te:
-    ...     print(te)
-    time_unit should be an instance of str but is int, namely '1'.
-    >>> try:
-    ...     check_time_unit("blabedibla")
-    ... except ValueError as ve:
-    ...     print(ve)
-    Invalid time unit 'blabedibla', only 'FEs' and 'ms' are permitted.
-    """
-    if not isinstance(time_unit, str):
-        raise type_error(time_unit, "time_unit", str)
-    if time_unit in (TIME_UNIT_FES, TIME_UNIT_MILLIS):
-        return time_unit
-    raise ValueError(
-        f"Invalid time unit {time_unit!r}, only {TIME_UNIT_FES!r} "
-        f"and {TIME_UNIT_MILLIS!r} are permitted.")
-
-
-def check_f_name(f_name: Any) -> str:
-    """
-    Check whether an objective value name is valid.
-
-    :param f_name: the name of the objective function dimension
-    :return: the name of the objective function dimension
-
-    >>> check_f_name("plainF")
-    'plainF'
-    >>> check_f_name("scaledF")
-    'scaledF'
-    >>> check_f_name("normalizedF")
-    'normalizedF'
-    >>> try:
-    ...     check_f_name(1.0)
-    ... except TypeError as te:
-    ...     print(te)
-    f_name should be an instance of str but is float, namely '1.0'.
-    >>> try:
-    ...     check_f_name("oops")
-    ... except ValueError as ve:
-    ...     print(ve)
-    Invalid f name 'oops', only 'plainF', 'scaledF', and 'normalizedF' \
-are permitted.
-    """
-    if not isinstance(f_name, str):
-        raise type_error(f_name, "f_name", str)
-    if f_name in (F_NAME_RAW, F_NAME_SCALED, F_NAME_NORMALIZED):
-        return f_name
-    raise ValueError(
-        f"Invalid f name {f_name!r}, only {F_NAME_RAW!r}, "
-        f"{F_NAME_SCALED!r}, and {F_NAME_NORMALIZED!r} are permitted.")
-
-
-@dataclass(frozen=True, init=False, order=True)
-class PerRunData:
-    """
-    An immutable record of information over a single run.
-
-    >>> p = PerRunData("a", "i", 234)
-    >>> print(p.instance)
-    i
-    >>> print(p.algorithm)
-    a
-    >>> print(p.rand_seed)
-    234
-    """
-
-    #: The algorithm that was applied.
-    algorithm: str
-
-    #: The problem instance that was solved.
-    instance: str
-
-    #: The seed of the random number generator.
-    rand_seed: int
-
-    def __init__(self, algorithm: str, instance: str, rand_seed: int):
-        """
-        Create a per-run data record.
-
-        :param str algorithm: the algorithm name
-        :param str instance: the instance name
-        :param int rand_seed: the random seed
-        """
-        if not isinstance(algorithm, str):
-            raise type_error(algorithm, "algorithm", str)
-        if algorithm != sanitize_name(algorithm):
-            raise ValueError(f"Invalid algorithm name {algorithm!r}.")
-        object.__setattr__(self, "algorithm", algorithm)
-
-        if not isinstance(instance, str):
-            raise type_error(instance, "instance", str)
-        if instance != sanitize_name(instance):
-            raise ValueError(f"Invalid instance name {instance!r}.")
-        object.__setattr__(self, "instance", instance)
-        object.__setattr__(self, "rand_seed", rand_seed_check(rand_seed))
-
-
-@dataclass(frozen=True, init=False, order=True)
-class MultiRunData:
-    """
-    A class that represents statistics over a set of runs.
-
-    If one algorithm*instance is used, then `algorithm` and `instance` are
-    defined. Otherwise, only the parameter which is the same over all recorded
-    runs is defined.
-
-    >>> p = MultiRunData("a", "i", 3)
-    >>> print(p.instance)
-    i
-    >>> print(p.algorithm)
-    a
-    >>> print(p.n)
-    3
-    """
-
-    #: The algorithm that was applied, if the same over all runs.
-    algorithm: str | None
-    #: The problem instance that was solved, if the same over all runs.
-    instance: str | None
-    #: The number of runs over which the statistic information is computed.
-    n: int
-
-    def __init__(self, algorithm: str | None, instance: str | None, n: int):
-        """
-        Create the dataset of an experiment-setup combination.
-
-        :param algorithm: the algorithm name, if all runs are with the same
-            algorithm
-        :param instance: the instance name, if all runs are on the same
-            instance
-        :param n: the total number of runs
-        """
-        if (algorithm is not None) and \
-                (algorithm != sanitize_name(algorithm)):
-            raise ValueError(f"Invalid algorithm {algorithm!r}.")
-        object.__setattr__(self, "algorithm", algorithm)
-
-        if (instance is not None) and (instance != sanitize_name(instance)):
-            raise ValueError(f"Invalid instance {instance!r}.")
-        object.__setattr__(self, "instance", instance)
-        object.__setattr__(self, "n", check_int_range(n, "n", 1))
-
-
-@dataclass(frozen=True, init=False, order=True)
-class MultiRun2DData(MultiRunData):
-    """
-    A multi-run data based on one time and one objective dimension.
-
-    >>> p = MultiRun2DData("a", "i", 3, TIME_UNIT_FES, F_NAME_SCALED)
-    >>> print(p.instance)
-    i
-    >>> print(p.algorithm)
-    a
-    >>> print(p.n)
-    3
-    >>> print(p.time_unit)
-    FEs
-    >>> print(p.f_name)
-    scaledF
-    """
-
-    #: The unit of the time axis.
-    time_unit: str
-    #: the name of the objective value axis.
-    f_name: str
-
-    def __init__(self, algorithm: str | None, instance: str | None, n: int,
-                 time_unit: str, f_name: str):
-        """
-        Create multi-run data based on one time and one objective dimension.
-
-        :param algorithm: the algorithm name, if all runs are with the same
-            algorithm
-        :param instance: the instance name, if all runs are on the same
-            instance
-        :param n: the total number of runs
-        :param time_unit: the time unit
-        :param f_name: the objective dimension name
-        """
-        super().__init__(algorithm, instance, n)
-        object.__setattr__(self, "time_unit", check_time_unit(time_unit))
-        object.__setattr__(self, "f_name", check_f_name(f_name))
-
-
-def get_instance(obj: PerRunData | MultiRunData) -> str | None:
-    """
-    Get the instance of a given object.
-
-    :param obj: the object
-    :return: the instance string, or `None` if no instance is specified
-
-    >>> p1 = MultiRunData("a", "i1", 3)
-    >>> print(get_instance(p1))
-    i1
-    >>> p2 = PerRunData("a", "i2", 31)
-    >>> print(get_instance(p2))
-    i2
-    """
-    return obj.instance
-
-
-def get_algorithm(obj: PerRunData | MultiRunData) -> str | None:
-    """
-    Get the algorithm of a given object.
-
-    :param obj: the object
-    :return: the algorithm string, or `None` if no algorithm is specified
-
-    >>> p1 = MultiRunData("a1", "i1", 3)
-    >>> print(get_algorithm(p1))
-    a1
-    >>> p2 = PerRunData("a2", "i2", 31)
-    >>> print(get_algorithm(p2))
-    a2
-    """
-    return obj.algorithm
-
-
-def sort_key(obj: PerRunData | MultiRunData) -> \
-        tuple[str, str, str, int, int, str, str, float]:
-    """
-    Get a default sort key for the given object.
-
-    The sort key is a tuple with well-defined field elements that should
-    allow for a default and consistent sorting over many different elements of
-    the experiment evaluation data API. Sorting should work also for lists
-    containing elements of different classes.
-
-    :param obj: the object
-    :return: the sort key
-
-    >>> p1 = MultiRunData("a1", "i1", 3)
-    >>> p2 = PerRunData("a2", "i2", 31)
-    >>> print(sort_key(p1) < sort_key(p2))
-    True
-    >>> print(sort_key(p1) >= sort_key(p2))
-    False
-    >>> p3 = MultiRun2DData("a", "i", 3, TIME_UNIT_FES, F_NAME_SCALED)
-    >>> print(sort_key(p3) < sort_key(p1))
-    True
-    >>> print(sort_key(p3) >= sort_key(p1))
-    False
-    """
-    goal_f = getattr(obj, "goal_f") if hasattr(obj, "goal_f") else None
-    if goal_f is None:
-        goal_f = inf
-
-    return obj.__class__.__name__, \
-        "" if obj.algorithm is None else obj.algorithm, \
-        "" if obj.instance is None else obj.instance, \
-        obj.n if isinstance(obj, MultiRunData) else 0, \
-        obj.rand_seed if isinstance(obj, PerRunData) else 0, \
-        obj.time_unit if isinstance(obj, MultiRun2DData) else "", \
-        obj.f_name if isinstance(obj, MultiRun2DData) else "", \
-        goal_f
+from typing import Any, Callable, Final, Iterable, cast
+
+from numpy.random import Generator, default_rng
+
+from moptipy.api.algorithm import Algorithm
+from moptipy.api.mo_algorithm import MOAlgorithm
+from moptipy.api.mo_problem import MOProblem
+from moptipy.api.objective import Objective
+from moptipy.examples.jssp.gantt import Gantt
+from moptipy.examples.jssp.gantt_space import GanttSpace
+from moptipy.examples.jssp.instance import Instance
+from moptipy.examples.jssp.makespan import Makespan
+from moptipy.examples.jssp.ob_encoding import OperationBasedEncoding
+from moptipy.examples.jssp.worktime import Worktime
+from moptipy.mo.problem.weighted_sum import WeightedSum
+from moptipy.operators.permutations.op0_shuffle import Op0Shuffle
+from moptipy.spaces.permutations import Permutations
+from moptipy.tests.algorithm import validate_algorithm
+from moptipy.tests.mo_algorithm import validate_mo_algorithm
+from moptipy.tests.objective import validate_objective
+from moptipy.utils.types import type_error
+
+
+def jssp_instances_for_tests() -> Iterable[str]:
+    """
+    Get a sequence of JSSP instances to test on.
+
+    :returns: an iterable of JSSP instance names
+    """
+    r = default_rng()
+    ri = r.integers
+    insts: list[str] = [
+        "demo", "ft06", "ft10", f"abz{ri(5, 10)}", f"dmu{ri(10, 81)}",
+        f"orb0{ri(1, 10)}", f"swv{ri(10, 21)}", f"ta{ri(10, 65)}",
+        f"ta{ri(65, 70)}", f"ta{ri(70, 75)}", f"yn{ri(1, 5)}"]
+    r.shuffle(cast(list, insts))
+    return insts
+
+
+def make_gantt_valid(inst: Instance) -> Callable[[Generator, Gantt], Gantt]:
+    """
+    Make a function that creates valid Gantt charts.
+
+    :param inst: the JSSP instance
+    :returns: a function that can make gantt charts valid
+    """
+    pr = Permutations.with_repetitions(inst.jobs, inst.machines)
+    op0 = Op0Shuffle(pr)
+    oe = OperationBasedEncoding(inst)
+
+    def __make_valid(prnd: Generator, x: Gantt, ppr=pr,
+                     pop0=op0, poe=oe) -> Gantt:
+        xx = ppr.create()
+        pop0.op0(prnd, xx)
+        poe.decode(xx, x)
+        return x
+
+    return __make_valid
+
+
+def validate_algorithm_on_1_jssp(
+        algorithm: Algorithm | Callable[
+            [Instance, Permutations, Objective], Algorithm],
+        instance: str | None = None, max_fes: int = 100,
+        required_result: int | None = None,
+        post: Callable[[Algorithm, int], Any] | None = None) -> None:
+    """
+    Check the validity of a black-box algorithm on the JSSP.
+
+    :param algorithm: the algorithm or algorithm factory
+    :param instance: the instance name, or `None` to randomly pick one
+    :param max_fes: the maximum number of FEs
+    :param required_result: the optional required result quality
+    :param post: a check to run after each execution of the algorithm,
+        receiving the algorithm and the number of consumed FEs as parameter
+    """
+    if not (isinstance(algorithm, Algorithm) or callable(algorithm)):
+        raise type_error(algorithm, "algorithm", Algorithm, True)
+    if instance is None:
+        instance = str(default_rng().choice(Instance.list_resources()))
+    if not isinstance(instance, str):
+        raise type_error(instance, "JSSP instance name", (str, None))
+    inst = Instance.from_resource(instance)
+    if not isinstance(inst, Instance):
+        raise type_error(inst, f"loaded JSSP instance {instance!r}", Instance)
+    if (post is not None) and (not callable(post)):
+        raise type_error(post, "post", None, call=True)
+
+    search_space = Permutations.with_repetitions(inst.jobs,
+                                                 inst.machines)
+    solution_space = GanttSpace(inst)
+    encoding = OperationBasedEncoding(inst)
+    objective = Makespan(inst)
+    if callable(algorithm):
+        algorithm = algorithm(inst, search_space, objective)
+    if not isinstance(algorithm, Algorithm):
+        raise type_error(algorithm, "algorithm", Algorithm, call=True)
+
+    goal: int
+    if required_result is None:
+        lb: int = objective.lower_bound()
+        ub: int = objective.upper_bound()
+        goal = max(lb + 1, min(ub - 1, int(0.5 + (lb + (0.96 * (ub - lb))))))
+    else:
+        goal = required_result
+
+    validate_algorithm(algorithm=algorithm,
+                       solution_space=solution_space,
+                       objective=objective,
+                       search_space=search_space,
+                       encoding=encoding,
+                       max_fes=max_fes,
+                       required_result=goal,
+                       post=post)
+
+
+def validate_algorithm_on_jssp(
+        algorithm: Callable[[Instance, Permutations,
+                             Objective], Algorithm],
+        max_fes: int = 100,
+        post: Callable[[Algorithm, int], Any] | None = None) -> None:
+    """
+    Validate an algorithm on a set of JSSP instances.
+
+    :param algorithm: the algorithm factory
+    :param max_fes: the maximum FEs
+    :param post: a check to run after each execution of the algorithm,
+        receiving the algorithm and the number of consumed FEs as parameter
+    """
+    for i in jssp_instances_for_tests():
+        validate_algorithm_on_1_jssp(algorithm, i, max_fes=max_fes, post=post)
+
+
+def validate_objective_on_1_jssp(
+        objective: Objective | Callable[[Instance], Objective],
+        instance: str | None = None,
+        is_deterministic: bool = True) -> None:
+    """
+    Validate an objective function on 1 JSSP instance.
+
+    :param objective: the objective function or a factory creating it
+    :param instance: the instance name
+    :param is_deterministic: is the objective function deterministic?
+    """
+    if instance is None:
+        instance = str(default_rng().choice(Instance.list_resources()))
+    if not isinstance(instance, str):
+        raise type_error(instance, "JSSP instance name", (str, None))
+    inst = Instance.from_resource(instance)
+    if not isinstance(inst, Instance):
+        raise type_error(inst, f"loaded JSSP instance {instance!r}", Instance)
+
+    if callable(objective):
+        objective = objective(inst)
+
+    validate_objective(
+        objective=objective,
+        solution_space=GanttSpace(inst),
+        make_solution_space_element_valid=make_gantt_valid(inst),
+        is_deterministic=is_deterministic)
+
+
+def validate_objective_on_jssp(
+        objective: Objective | Callable[[Instance], Objective],
+        is_deterministic: bool = True) -> None:
+    """
+    Validate an objective function on JSSP instances.
+
+    :param objective: the objective function or a factory creating it
+    :param is_deterministic: is the objective function deterministic?
+    """
+    for i in jssp_instances_for_tests():
+        validate_objective_on_1_jssp(objective, i, is_deterministic)
+
+
+def validate_mo_algorithm_on_1_jssp(
+        algorithm: MOAlgorithm | Callable[
+            [Instance, Permutations, MOProblem], MOAlgorithm],
+        instance: str | None = None, max_fes: int = 100) -> None:
+    """
+    Check the validity of a black-box multi-objective algorithm on the JSSP.
+
+    :param algorithm: the algorithm or algorithm factory
+    :param instance: the instance name, or `None` to randomly pick one
+    :param max_fes: the maximum number of FEs
+    """
+    if not (isinstance(algorithm, MOAlgorithm) or callable(algorithm)):
+        raise type_error(algorithm, "algorithm", MOAlgorithm, True)
+
+    random: Final[Generator] = default_rng()
+    if instance is None:
+        instance = str(random.choice(Instance.list_resources()))
+    if not isinstance(instance, str):
+        raise type_error(instance, "JSSP instance name", (str, None))
+    inst = Instance.from_resource(instance)
+    if not isinstance(inst, Instance):
+        raise type_error(inst, "loaded JSSP instance '{instance}'", Instance)
+
+    search_space = Permutations.with_repetitions(inst.jobs,
+                                                 inst.machines)
+    solution_space = GanttSpace(inst)
+    encoding = OperationBasedEncoding(inst)
+
+    weights: Final[list[int | float]] = [float(random.uniform(0.01, 10)),
+                                         float(random.uniform(0.01, 10))] \
+        if random.integers(2) <= 0 else \
+        [1 + int(random.integers(1 << random.integers(40))),
+         1 + int(random.integers(1 << random.integers(40)))]
+    problem: Final[MOProblem] = WeightedSum(
+        [Makespan(inst), Worktime(inst)], weights)
+
+    if callable(algorithm):
+        algorithm = algorithm(inst, search_space, problem)
+    if not isinstance(algorithm, MOAlgorithm):
+        raise type_error(algorithm, "algorithm", MOAlgorithm, call=True)
+
+    validate_mo_algorithm(algorithm=algorithm,
+                          solution_space=solution_space,
+                          problem=problem,
+                          search_space=search_space,
+                          encoding=encoding,
+                          max_fes=max_fes)
+
+
+def validate_mo_algorithm_on_jssp(
+        algorithm: Callable[
+            [Instance, Permutations, MOProblem], MOAlgorithm]) -> None:
+    """
+    Validate a multi-objective algorithm on a set of JSSP instances.
+
+    :param algorithm: the algorithm factory
+    """
+    for i in jssp_instances_for_tests():
+        validate_mo_algorithm_on_1_jssp(algorithm, i, 100)
```

### Comparing `moptipy-0.9.90/moptipy/evaluation/ecdf.py` & `moptipy-0.9.91/moptipy/evaluation/ecdf.py`

 * *Files 14% similar despite different names*

```diff
@@ -35,75 +35,87 @@
 
 from dataclasses import dataclass
 from math import inf, isfinite
 from typing import Any, Callable, Final, Iterable
 
 import numpy as np
 
-import moptipy.api.logging as lg
-import moptipy.utils.nputils as npu
+from moptipy.api.logging import (
+    KEY_ALGORITHM,
+    KEY_GOAL_F,
+)
 from moptipy.evaluation._utils import _get_goal_reach_index
 from moptipy.evaluation.base import (
     F_NAME_NORMALIZED,
     F_NAME_SCALED,
+    KEY_ENCODING,
     KEY_N,
+    KEY_OBJECTIVE_FUNCTION,
     MultiRun2DData,
 )
 from moptipy.evaluation.progress import Progress
 from moptipy.utils.console import logger
 from moptipy.utils.lang import Lang
 from moptipy.utils.logger import (
     COMMENT_CHAR,
     CSV_SEPARATOR,
     KEY_VALUE_SEPARATOR,
 )
+from moptipy.utils.nputils import is_all_finite
 from moptipy.utils.path import Path
 from moptipy.utils.strings import num_to_str
 from moptipy.utils.types import check_int_range, type_error
 
 #: The number of instances.
 KEY_N_INSTS: Final[str] = f"{KEY_N}Insts"
 #: The objective dimension name.
 KEY_F_NAME: Final[str] = "fName"
 
 
-@dataclass(frozen=True, init=False, order=True)
+@dataclass(frozen=True, init=False, order=False, eq=False)
 class Ecdf(MultiRun2DData):
     """The ECDF data."""
 
     #: The ECDF data function
     ecdf: np.ndarray
     #: The number of instances over which the ERT-ECDF is computed.
     n_insts: int
     #: The goal value, or None if different goals were used for different
     #: instances
     goal_f: int | float | None
 
     def __init__(self,
                  algorithm: str | None,
+                 objective: str | None,
+                 encoding: str | None,
                  n: int,
                  n_insts: int,
                  time_unit: str,
                  f_name: str,
                  goal_f: int | float | None,
                  ecdf: np.ndarray):
         """
         Create the ECDF function.
 
         :param algorithm: the algorithm name, if all runs are with the same
             algorithm
+        :param objective: the objective name, if all runs are on the same
+            objective function, `None` otherwise
+        :param encoding: the encoding name, if all runs are on the same
+            encoding and an encoding was actually used, `None` otherwise
         :param n: the total number of runs
         :param n_insts: the total number of instances
         :param time_unit: the time unit
         :param f_name: the objective dimension name
         :param goal_f: the goal value, or `None` if different goals were used
             for different instances
         :param numpy.ndarray ecdf: the ert-ecdf matrix
         """
-        super().__init__(algorithm, None, n, time_unit, f_name)
+        super().__init__(algorithm, None, objective, encoding, n,
+                         time_unit, f_name)
         object.__setattr__(
             self, "n_insts", check_int_range(n_insts, "n_insts", 1, self.n))
 
         if goal_f is not None:
             if not isinstance(goal_f, int | float):
                 raise type_error(goal_f, "goal_f", (int, float))
             if not isfinite(goal_f):
@@ -115,23 +127,23 @@
         ecdf.flags.writeable = False
 
         time: Final[np.ndarray] = ecdf[:, 0]
         ll = time.size
         if ll < 2:
             raise ValueError("Must have at least two points in "
                              f"ecdf curve , but encountered {ll}.")
-        if not npu.is_all_finite(time[:-1]):
+        if not is_all_finite(time[:-1]):
             raise ValueError("Non-last Ert-based time-values must be finite, "
                              f"but encountered {time}.")
         if np.any(time[1:] <= time[:-1]):
             raise ValueError("Time data must be strictly increasing,"
                              f"but encountered {time}.")
 
         prb: Final[np.ndarray] = ecdf[:, 1]
-        if not npu.is_all_finite(prb):
+        if not is_all_finite(prb):
             raise ValueError(
                 f"All ECDF values must be finite, but encountered {prb}.")
         if (ll > 2) and np.any(prb[1:-1] <= prb[:-2]):
             raise ValueError("ECDF data must be strictly increasing,"
                              f"but encountered {prb}.")
         if prb[0] < 0:
             raise ValueError(f"First ECDF element cannot be {prb[0]}.")
@@ -151,45 +163,61 @@
         """
         Get the time key.
 
         :return: the time key
         """
         return self.time_unit
 
+    def _tuple(self) -> tuple[Any, ...]:
+        """
+        Get the tuple representation of this object used in comparisons.
+
+        :return: the comparison-relevant data of this object in a tuple
+        """
+        return (self.__class__.__name__,
+                "" if self.algorithm is None else self.algorithm,
+                "" if self.instance is None else self.instance,
+                "" if self.objective is None else self.objective,
+                "" if self.encoding is None else self.encoding,
+                self.n, -1, self.time_unit, self.f_name,
+                inf if self.goal_f is None else self.goal_f,
+                self.n_insts)
+
     def to_csv(self, file: str,
                put_header: bool = True) -> Path:
         """
         Store a :class:`Ecdf` record in a CSV file.
 
         :param file: the file to generate
         :param put_header: should we put a header with meta-data?
         :return: the fully resolved file name
         """
         path: Final[Path] = Path.path(file)
         logger(f"Writing ECDF to CSV file {path!r}.")
 
         with path.open_for_write() as out:
             sep: Final[str] = CSV_SEPARATOR
+            write: Final[Callable[[str], int]] = out.write
             if put_header:
                 kv: Final[str] = KEY_VALUE_SEPARATOR
                 cmt: Final[str] = COMMENT_CHAR
                 if self.algorithm is not None:
-                    out.write(
-                        f"{cmt} {lg.KEY_ALGORITHM}{kv}{self.algorithm}\n")
-                out.write(
-                    f"{cmt} {KEY_N}{kv}{self.n}\n")
-                out.write(
-                    f"{cmt} {KEY_N_INSTS}{kv}{self.n_insts}\n")
-                out.write(
-                    f"{cmt} {KEY_F_NAME}{kv}{self.f_name}\n")
+                    write(f"{cmt} {KEY_ALGORITHM}{kv}{self.algorithm}\n")
+                write(f"{cmt} {KEY_N}{kv}{self.n}\n")
+                write(f"{cmt} {KEY_N_INSTS}{kv}{self.n_insts}\n")
+                write(f"{cmt} {KEY_F_NAME}{kv}{self.f_name}\n")
                 if self.goal_f is not None:
-                    out.write(
-                        f"{cmt} {lg.KEY_GOAL_F}{kv}{self.goal_f}\n")
+                    write(f"{cmt} {KEY_GOAL_F}{kv}{self.goal_f}\n")
+                if self.objective is not None:
+                    write(f"{cmt} {KEY_OBJECTIVE_FUNCTION}"
+                          f"{kv}{self.objective}\n")
+                if self.encoding is not None:
+                    write(f"{cmt} {KEY_ENCODING}{kv}{self.encoding}\n")
 
-            out.write(f"{self._time_key()}{sep}ecdf\n")
+            write(f"{self._time_key()}{sep}ecdf\n")
             for v in self.ecdf:
                 out.write(
                     f"{num_to_str(v[0])}{sep}{num_to_str(v[1])}\n")
 
         logger(f"Done writing ECDF to CSV file {path!r}.")
 
         path.enforce_file()
@@ -245,29 +273,37 @@
         :return: the Ecdf record
         :rtype: Ecdf
         """
         if not isinstance(source, Iterable):
             raise type_error(source, "source", Iterable)
 
         algorithm: str | None = None
+        objective: str | None = None
+        encoding: str | None = None
         time_unit: str | None = None
         f_name: str | None = None
         inst_runs: dict[str, list[Progress]] = {}
         n: int = 0
 
         for progress in source:
             if not isinstance(progress, Progress):
                 raise type_error(progress, "progress", Progress)
             if n <= 0:
                 algorithm = progress.algorithm
                 time_unit = progress.time_unit
+                objective = progress.objective
+                encoding = progress.encoding
                 f_name = progress.f_name
             else:
                 if algorithm != progress.algorithm:
                     algorithm = None
+                if objective != progress.objective:
+                    objective = None
+                if encoding != progress.encoding:
+                    encoding = None
                 if time_unit != progress.time_unit:
                     raise ValueError(
                         f"Cannot mix time units {time_unit} "
                         f"and {progress.time_unit}.")
                 if f_name != progress.f_name:
                     raise ValueError(f"Cannot mix f-names {f_name} "
                                      f"and {progress.f_name}.")
@@ -318,17 +354,16 @@
                         raise ValueError(f"Invalid ert {t}.")
                     times.append(t)
                 elif not (t >= inf):
                     raise ValueError(f"Invalid ert {t}.")
         del inst_runs
 
         if len(times) <= 0:
-            return cls(algorithm, n, n_insts, time_unit,
-                       f_name, same_goal_f,
-                       np.array([[0, 0], [inf, 0]]))
+            return cls(algorithm, objective, encoding, n, n_insts, time_unit,
+                       f_name, same_goal_f, np.array([[0, 0], [inf, 0]]))
 
         times.sort()
         time: list[float] = [0]
         ecdf: list[float] = [0]
         success: int = 0
         div: Final[int] = cls._get_div(n, n_insts)
         ll: int = 0
@@ -340,65 +375,76 @@
                 ll += 1
             else:
                 ecdf[ll] = success / div
 
         time.append(inf)
         ecdf.append(ecdf[ll])
 
-        return cls(algorithm, n, n_insts,
-                   time_unit, f_name,
-                   same_goal_f,
-                   np.column_stack((np.array(time),
-                                    np.array(ecdf))))
+        return cls(algorithm, objective, encoding, n, n_insts,
+                   time_unit, f_name, same_goal_f,
+                   np.column_stack((np.array(time), np.array(ecdf))))
 
     @classmethod
     def from_progresses(
             cls: type["Ecdf"],
             source: Iterable[Progress], consumer: Callable[["Ecdf"], Any],
             f_goal: int | float | Callable
                         | Iterable[int | float | Callable] | None = None,
-            join_all_algorithms: bool = False) -> None:
+            join_all_algorithms: bool = False,
+            join_all_objectives: bool = False,
+            join_all_encodings: bool = False) -> None:
         """
         Compute one or multiple ECDFs from a stream of end results.
 
         :param source: the set of progress instances
         :param f_goal: one or multiple goal values
         :param consumer: the destination to which the new records will be
             passed, can be the `append` method of a :class:`list`
-        :param join_all_algorithms: should the Ert-Ecdf be aggregated over all
+        :param join_all_algorithms: should the Ecdf be aggregated over all
             algorithms
+        :param join_all_objectives: should the Ecdf be aggregated over all
+            objective functions
+        :param join_all_encodings: should the Ecdf be aggregated over all
+            encodings
         """
         if not isinstance(source, Iterable):
             raise type_error(source, "source", Iterable)
         if not callable(consumer):
             raise type_error(consumer, "consumer", call=True)
         if not isinstance(join_all_algorithms, bool):
             raise type_error(join_all_algorithms,
                              "join_all_algorithms", bool)
+        if not isinstance(join_all_objectives, bool):
+            raise type_error(join_all_objectives,
+                             "join_all_objectives", bool)
+        if not isinstance(join_all_encodings, bool):
+            raise type_error(join_all_encodings,
+                             "join_all_encodings", bool)
         if not isinstance(f_goal, Iterable):
             f_goal = [f_goal]
 
-        sorter: dict[str, list[Progress]] = {}
+        sorter: dict[tuple[str, str, str], list[Progress]] = {}
         for er in source:
             if not isinstance(er, Progress):
                 raise type_error(er, "progress", Progress)
-            key = er.algorithm
+            key = ("" if join_all_algorithms else er.algorithm,
+                   "" if join_all_objectives else er.objective,
+                   "" if join_all_encodings else (
+                       "" if er.encoding is None else er.encoding))
             if key in sorter:
                 lst = sorter[key]
             else:
                 lst = []
                 sorter[key] = lst
             lst.append(er)
 
         if len(sorter) <= 0:
             raise ValueError("source must not be empty")
 
-        keyz = list(sorter.keys())
-        keyz.sort()
-
+        keyz = sorted(sorter.keys())
         for goal in f_goal:
             use_default_goal = goal is None
             for key in keyz:
                 consumer(cls.create(sorter[key], goal, use_default_goal))
 
 
 def get_goal(ecdf: Ecdf) -> int | float | None:
```

### Comparing `moptipy-0.9.90/moptipy/evaluation/end_results.py` & `moptipy-0.9.91/moptipy/evaluation/end_results.py`

 * *Files 12% similar despite different names*

```diff
@@ -40,14 +40,16 @@
 from moptipy.evaluation._utils import (
     _check_max_time_millis,
 )
 from moptipy.evaluation.base import (
     F_NAME_NORMALIZED,
     F_NAME_RAW,
     F_NAME_SCALED,
+    KEY_ENCODING,
+    KEY_OBJECTIVE_FUNCTION,
     PerRunData,
 )
 from moptipy.evaluation.log_parser import SetupAndStateParser
 from moptipy.utils.console import logger
 from moptipy.utils.help import argparser
 from moptipy.utils.logger import CSV_SEPARATOR
 from moptipy.utils.math import try_float_div, try_int
@@ -59,27 +61,26 @@
     sanitize_names,
     str_to_intfloat,
     str_to_intfloatnone,
     str_to_intnone,
 )
 from moptipy.utils.types import check_int_range, check_to_int_range, type_error
 
-#: The internal CSV header
-_HEADER: Final[str] = (f"{KEY_ALGORITHM}{CSV_SEPARATOR}"
-                       f"{KEY_INSTANCE}{CSV_SEPARATOR}"
-                       f"{KEY_RAND_SEED}{CSV_SEPARATOR}"
-                       f"{KEY_BEST_F}{CSV_SEPARATOR}"
-                       f"{KEY_LAST_IMPROVEMENT_FE}{CSV_SEPARATOR}"
-                       f"{KEY_LAST_IMPROVEMENT_TIME_MILLIS}"
-                       f"{CSV_SEPARATOR}"
-                       f"{KEY_TOTAL_FES}{CSV_SEPARATOR}"
-                       f"{KEY_TOTAL_TIME_MILLIS}{CSV_SEPARATOR}"
-                       f"{KEY_GOAL_F}{CSV_SEPARATOR}"
-                       f"{KEY_MAX_FES}{CSV_SEPARATOR}"
-                       f"{KEY_MAX_TIME_MILLIS}\n")
+#: The internal CSV header, part 1
+_HEADER_1: Final[str] = (f"{KEY_ALGORITHM}{CSV_SEPARATOR}"
+                         f"{KEY_INSTANCE}{CSV_SEPARATOR}"
+                         f"{KEY_OBJECTIVE_FUNCTION}")
+#: The internal CSV header, part 2
+_HEADER_2: Final[str] = (f"{CSV_SEPARATOR}{KEY_RAND_SEED}{CSV_SEPARATOR}"
+                         f"{KEY_BEST_F}{CSV_SEPARATOR}"
+                         f"{KEY_LAST_IMPROVEMENT_FE}{CSV_SEPARATOR}"
+                         f"{KEY_LAST_IMPROVEMENT_TIME_MILLIS}"
+                         f"{CSV_SEPARATOR}"
+                         f"{KEY_TOTAL_FES}{CSV_SEPARATOR}"
+                         f"{KEY_TOTAL_TIME_MILLIS}")
 
 
 def __get_goal_f(e: "EndResult") -> int | float:
     """
     Get the goal_f.
 
     :param e: the end result
@@ -156,15 +157,15 @@
     F_NAME_NORMALIZED: __get_f_norm,
     KEY_MAX_FES: __get_max_fes,
     KEY_MAX_TIME_MILLIS: __get_max_time_millis,
 }
 _GETTERS[KEY_BEST_F] = _GETTERS[F_NAME_RAW]
 
 
-@dataclass(frozen=True, init=False, order=True)
+@dataclass(frozen=True, init=False, order=False, eq=False)
 class EndResult(PerRunData):
     """
     An immutable end result record of one run of one algorithm on one problem.
 
     This record provides the information of the outcome of one application of
     one algorithm to one problem instance in an immutable way.
     """
@@ -192,42 +193,47 @@
 
     #: The (optional) maximum runtime.
     max_time_millis: int | None
 
     def __init__(self,
                  algorithm: str,
                  instance: str,
+                 objective: str,
+                 encoding: str | None,
                  rand_seed: int,
                  best_f: int | float,
                  last_improvement_fe: int,
                  last_improvement_time_millis: int,
                  total_fes: int,
                  total_time_millis: int,
                  goal_f: int | float | None,
                  max_fes: int | None,
                  max_time_millis: int | None):
         """
         Create a consistent instance of :class:`EndResult`.
 
         :param algorithm: the algorithm name
         :param instance: the instance name
+        :param objective: the name of the objective function
+        :param encoding: the name of the encoding that was used, if any, or
+            `None` if no encoding was used
         :param rand_seed: the random seed
         :param best_f: the best reached objective value
         :param last_improvement_fe: the FE when best_f was reached
         :param last_improvement_time_millis: the time when best_f was reached
         :param total_fes: the total FEs
         :param total_time_millis: the total runtime
         :param goal_f: the goal objective value, if provide
         :param max_fes: the optional maximum FEs
         :param max_time_millis: the optional maximum runtime
 
         :raises TypeError: if any parameter has a wrong type
         :raises ValueError: if the parameter values are inconsistent
         """
-        super().__init__(algorithm, instance, rand_seed)
+        super().__init__(algorithm, instance, objective, encoding, rand_seed)
         object.__setattr__(self, "best_f", try_int(best_f))
         object.__setattr__(
             self, "last_improvement_fe", check_int_range(
                 last_improvement_fe, "last_improvement_fe",
                 1, 1_000_000_000_000_000))
         object.__setattr__(
             self, "last_improvement_time_millis", check_int_range(
@@ -255,14 +261,33 @@
             check_int_range(
                 max_time_millis, "max_time_millis", 1, 100_000_000_000)
             _check_max_time_millis(max_time_millis,
                                    total_fes,
                                    total_time_millis)
         object.__setattr__(self, "max_time_millis", max_time_millis)
 
+    def _tuple(self) -> tuple[Any, ...]:
+        """
+        Get the tuple representation of this object used in comparisons.
+
+        :return: the comparison-relevant data of this object in a tuple
+        """
+        return (self.__class__.__name__,
+                "" if self.algorithm is None else self.algorithm,
+                "" if self.instance is None else self.instance,
+                "" if self.objective is None else self.objective,
+                "" if self.encoding is None else self.encoding,
+                1, self.rand_seed, "", "",
+                inf if self.goal_f is None else self.goal_f,
+                inf if self.max_fes is None else self.max_fes,
+                inf if self.max_time_millis is None else self.max_time_millis,
+                self.best_f, self.last_improvement_fe,
+                self.last_improvement_time_millis, self.total_fes,
+                self.total_time_millis)
+
     def success(self) -> bool:
         """
         Check if a run is successful.
 
         This method returns `True` if and only if `goal_f` is defined and
         `best_f <= goal_f` (and `False` otherwise).
 
@@ -416,29 +441,65 @@
         :param file: the path
         :return: the path of the file that was written
         """
         path: Final[Path] = Path.path(file)
         logger(f"Writing end results to CSV file {path!r}.")
         Path.path(os.path.dirname(path)).ensure_dir_exists()
 
+        sorted_results: Final[list[EndResult]] = sorted(results)
+        needs_encoding: bool = False
+        needs_max_fes: bool = False
+        needs_max_ms: bool = False
+        needs_goal_f: bool = False
+        for er in sorted_results:
+            if er.encoding is not None:
+                needs_encoding = True
+            if er.max_fes is not None:
+                needs_max_fes = True
+            if er.max_time_millis is not None:
+                needs_max_ms = True
+            if (er.goal_f is not None) and (isfinite(er.goal_f)):
+                needs_goal_f = True
+
         with path.open_for_write() as out:
-            out.write(_HEADER)
+            write: Final[Callable[[str], int]] = out.write
+            write(_HEADER_1)
+            if needs_encoding:
+                write(f"{CSV_SEPARATOR}{KEY_ENCODING}")
+            write(_HEADER_2)
+            if needs_goal_f:
+                write(f"{CSV_SEPARATOR}{KEY_GOAL_F}")
+            if needs_max_fes:
+                write(f"{CSV_SEPARATOR}{KEY_MAX_FES}")
+            if needs_max_ms:
+                write(f"{CSV_SEPARATOR}{KEY_MAX_TIME_MILLIS}")
+            write("\n")
+
             for e in results:
-                out.write(
-                    f"{e.algorithm}{CSV_SEPARATOR}"
-                    f"{e.instance}{CSV_SEPARATOR}"
-                    f"{hex(e.rand_seed)}{CSV_SEPARATOR}"
-                    f"{num_to_str(e.best_f)}{CSV_SEPARATOR}"
-                    f"{e.last_improvement_fe}{CSV_SEPARATOR}"
-                    f"{e.last_improvement_time_millis}{CSV_SEPARATOR}"
-                    f"{e.total_fes}{CSV_SEPARATOR}"
-                    f"{e.total_time_millis}{CSV_SEPARATOR}"
-                    f"{intfloatnone_to_str(e.goal_f)}{CSV_SEPARATOR}"
-                    f"{intnone_to_str(e.max_fes)}{CSV_SEPARATOR}"
-                    f"{intnone_to_str(e.max_time_millis)}\n")
+                write(f"{e.algorithm}{CSV_SEPARATOR}"
+                      f"{e.instance}{CSV_SEPARATOR}"
+                      f"{e.objective}")
+                if needs_encoding:
+                    write(CSV_SEPARATOR)
+                    if e.encoding is not None:
+                        write(e.encoding)
+                write(f"{CSV_SEPARATOR}{hex(e.rand_seed)}{CSV_SEPARATOR}"
+                      f"{num_to_str(e.best_f)}{CSV_SEPARATOR}"
+                      f"{e.last_improvement_fe}{CSV_SEPARATOR}"
+                      f"{e.last_improvement_time_millis}{CSV_SEPARATOR}"
+                      f"{e.total_fes}{CSV_SEPARATOR}"
+                      f"{e.total_time_millis}")
+                if needs_goal_f:
+                    write(f"{CSV_SEPARATOR}{intfloatnone_to_str(e.goal_f)}")
+                if needs_max_fes:
+                    write(f"{CSV_SEPARATOR}{intnone_to_str(e.max_fes)}")
+                if needs_max_ms:
+                    write(
+                        f"{CSV_SEPARATOR}{intnone_to_str(e.max_time_millis)}")
+                write("\n")
 
         logger(f"Done writing end results to CSV file {path!r}.")
         return path
 
     @staticmethod
     def from_csv(file: str, consumer: Callable[["EndResult"], Any],
                  filterer: Callable[["EndResult"], bool]
@@ -453,39 +514,138 @@
         """
         if not callable(consumer):
             raise type_error(consumer, "consumer", call=True)
         path: Final[Path] = Path.file(file)
         logger(f"Now reading CSV file {path!r}.")
 
         with path.open_for_read() as rd:
-            header = rd.readlines(1)
-            if (header is None) or (len(header) <= 0):
+            header_rows: list[str] = rd.readlines(1)
+            if (header_rows is None) or (len(header_rows) <= 0):
                 raise ValueError(f"No line in file {file!r}.")
-            if header[0] != _HEADER:
+            header = header_rows[0]
+            if not isinstance(header, str):
+                raise type_error(header, f"{file!r}[0]", str)
+            header = header.strip()
+            if not header.startswith(_HEADER_1):
+                raise ValueError(f"header of {file!r} should start with "
+                                 f"{_HEADER_1!r} but is {header!r}")
+
+            idx_algorithm: int = -1
+            idx_instance: int = -1
+            idx_objective: int = -1
+            idx_encoding: int = -1
+            idx_seed: int = -1
+            idx_li_fe: int = -1
+            idx_li_ms: int = -1
+            idx_best_f: int = -1
+            idx_tt_fe: int = -1
+            idx_tt_ms: int = -1
+            idx_goal_f: int = -1
+            idx_max_fes: int = -1
+            idx_max_ms: int = -1
+
+            for i, cell in enumerate(header.split(CSV_SEPARATOR)):
+                if cell == KEY_ALGORITHM:
+                    idx_algorithm = i
+                elif cell == KEY_INSTANCE:
+                    idx_instance = i
+                elif cell == KEY_OBJECTIVE_FUNCTION:
+                    idx_objective = i
+                elif cell == KEY_ENCODING:
+                    idx_encoding = i
+                elif cell == KEY_RAND_SEED:
+                    idx_seed = i
+                elif cell == KEY_LAST_IMPROVEMENT_FE:
+                    idx_li_fe = i
+                elif cell == KEY_LAST_IMPROVEMENT_TIME_MILLIS:
+                    idx_li_ms = i
+                elif cell == KEY_BEST_F:
+                    idx_best_f = i
+                elif cell == KEY_TOTAL_FES:
+                    idx_tt_fe = i
+                elif cell == KEY_TOTAL_TIME_MILLIS:
+                    idx_tt_ms = i
+                elif cell == KEY_GOAL_F:
+                    idx_goal_f = i
+                elif cell == KEY_MAX_FES:
+                    idx_max_fes = i
+                elif cell == KEY_MAX_TIME_MILLIS:
+                    idx_max_ms = i
+                else:
+                    raise ValueError(
+                        f"Unknown key {cell!r} at index {i} in header "
+                        f"{header!r} of file {file!r}.")
+
+            if idx_algorithm < 0:
+                raise ValueError(
+                    f"Missing key {KEY_ALGORITHM!r} in header "
+                    f"{header!r} of file {file!r}.")
+            if idx_instance < 0:
+                raise ValueError(
+                    f"Missing key {KEY_INSTANCE!r} in header "
+                    f"{header!r} of file {file!r}.")
+            if idx_objective < 0:
+                raise ValueError(
+                    f"Missing key {KEY_OBJECTIVE_FUNCTION!r} in header "
+                    f"{header!r} of file {file!r}.")
+            if idx_seed < 0:
+                raise ValueError(
+                    f"Missing key {KEY_RAND_SEED!r} in "
+                    f"header {header!r} of file {file!r}.")
+            if idx_li_fe < 0:
+                raise ValueError(
+                    f"Missing key {KEY_LAST_IMPROVEMENT_FE!r} in header "
+                    f"{header!r} of file {file!r}.")
+            if idx_li_ms < 0:
+                raise ValueError(
+                    f"Missing key {KEY_LAST_IMPROVEMENT_TIME_MILLIS!r} in "
+                    f"header {header!r} of file {file!r}.")
+            if idx_best_f < 0:
+                raise ValueError(
+                    f"Missing key {KEY_BEST_F!r} in header "
+                    f"{header!r} of file {file!r}.")
+            if idx_tt_fe < 0:
+                raise ValueError(
+                    f"Missing key {KEY_TOTAL_FES!r} in "
+                    f"header {header!r} of file {file!r}.")
+            if idx_tt_ms < 0:
                 raise ValueError(
-                    f"Header {header[0]!r} in {path!r} should be {_HEADER!r}.")
+                    f"Missing key {KEY_TOTAL_TIME_MILLIS!r} in "
+                    f"header {header!r} of file {file!r}.")
 
             while True:
                 lines = rd.readlines(100)
                 if (lines is None) or (len(lines) <= 0):
                     break
                 for line in lines:
                     splt = line.strip().split(CSV_SEPARATOR)
+                    encoding: str | None
+                    if idx_encoding < 0:
+                        encoding = None
+                    else:
+                        encoding = splt[idx_encoding].strip()
+                        if len(encoding) <= 0:
+                            encoding = None
                     er = EndResult(
-                        splt[0].strip(),  # algorithm
-                        splt[1].strip(),  # instance
-                        int((splt[2])[2:], 16),  # rand seed
-                        str_to_intfloat(splt[3]),  # best_f
-                        int(splt[4]),  # last_improvement_fe
-                        int(splt[5]),  # last_improvement_time_millis
-                        int(splt[6]),  # total_fes
-                        int(splt[7]),  # total_time_millis
-                        str_to_intfloatnone(splt[8]),  # goal_f
-                        str_to_intnone(splt[9]),  # max_fes
-                        str_to_intnone(splt[10]))  # max_time_millis
+                        splt[idx_algorithm].strip(),  # algorithm
+                        splt[idx_instance].strip(),  # instance
+                        splt[idx_objective].strip(),  # objective
+                        encoding,  # encoding
+                        int((splt[idx_seed])[2:], 16),  # rand seed
+                        str_to_intfloat(splt[idx_best_f]),  # best_f
+                        int(splt[idx_li_fe]),  # last_improvement_fe
+                        int(splt[idx_li_ms]),  # last_improvement_time_millis
+                        int(splt[idx_tt_fe]),  # total_fes
+                        int(splt[idx_tt_ms]),  # total_time_millis
+                        None if idx_goal_f < 0 else
+                        str_to_intfloatnone(splt[idx_goal_f]),  # goal_f
+                        None if idx_max_fes < 0 else
+                        str_to_intnone(splt[idx_max_fes]),  # max_fes
+                        None if idx_max_ms < 0 else
+                        str_to_intnone(splt[idx_max_ms]))  # max_time_millis
                     if filterer(er):
                         consumer(er)
 
         logger(f"Done reading CSV file {path!r}.")
 
 
 class _InnerLogParser(SetupAndStateParser):
@@ -501,14 +661,16 @@
         if not callable(consumer):
             raise type_error(consumer, "consumer", call=True)
         self.__consumer: Final[Callable[[EndResult], Any]] = consumer
 
     def process(self) -> None:
         self.__consumer(EndResult(self.algorithm,
                                   self.instance,
+                                  self.objective,
+                                  self.encoding,
                                   self.rand_seed,
                                   self.best_f,
                                   self.last_improvement_fe,
                                   self.last_improvement_time_millis,
                                   self.total_fes,
                                   self.total_time_millis,
                                   self.goal_f,
@@ -591,14 +753,16 @@
                 ul_fes = ul_fes - 1
             stop_fes = max(stop_fes, cast(int, min(
                 ul_fes, self.__limit_fes)))
 
         self.__consumer(EndResult(
             algorithm=self.algorithm,
             instance=self.instance,
+            objective=self.objective,
+            encoding=self.encoding,
             rand_seed=self.rand_seed,
             best_f=self.__stop_f,
             last_improvement_fe=self.__stop_li_fe,
             last_improvement_time_millis=self.__stop_li_ms,
             total_fes=stop_fes,
             total_time_millis=stop_ms,
             goal_f=_join_goals(self.__limit_f_n, self.goal_f, max),
```

### Comparing `moptipy-0.9.90/moptipy/evaluation/end_statistics.py` & `moptipy-0.9.91/moptipy/evaluation/end_statistics.py`

 * *Files 4% similar despite different names*

```diff
@@ -10,20 +10,35 @@
 """
 import argparse
 import os.path
 from dataclasses import dataclass
 from math import ceil, inf
 from typing import Any, Callable, Final, Iterable, Union
 
-import moptipy.api.logging as log
-from moptipy.evaluation._utils import _check_max_time_millis
+from moptipy.api.logging import (
+    KEY_ALGORITHM,
+    KEY_BEST_F,
+    KEY_GOAL_F,
+    KEY_INSTANCE,
+    KEY_LAST_IMPROVEMENT_FE,
+    KEY_LAST_IMPROVEMENT_TIME_MILLIS,
+    KEY_MAX_FES,
+    KEY_MAX_TIME_MILLIS,
+    KEY_TOTAL_FES,
+    KEY_TOTAL_TIME_MILLIS,
+)
+from moptipy.evaluation._utils import (
+    _check_max_time_millis,
+)
 from moptipy.evaluation.base import (
     F_NAME_RAW,
     F_NAME_SCALED,
+    KEY_ENCODING,
     KEY_N,
+    KEY_OBJECTIVE_FUNCTION,
     MultiRunData,
 )
 from moptipy.evaluation.end_results import EndResult
 from moptipy.evaluation.statistics import (
     CSV_COLS,
     EMPTY_CSV_ROW,
     KEY_STDDEV,
@@ -34,15 +49,15 @@
 from moptipy.utils.logger import CSV_SEPARATOR, SCOPE_SEPARATOR
 from moptipy.utils.math import try_int, try_int_div
 from moptipy.utils.path import Path
 from moptipy.utils.strings import num_to_str, sanitize_name, str_to_intfloat
 from moptipy.utils.types import check_int_range, type_error, type_name_of
 
 #: The key for the best F.
-KEY_BEST_F_SCALED: Final[str] = log.KEY_BEST_F + "scaled"
+KEY_BEST_F_SCALED: Final[str] = KEY_BEST_F + "scaled"
 #: The key for the number of successful runs.
 KEY_N_SUCCESS: Final[str] = "successN"
 #: The key for the success FEs.
 KEY_SUCCESS_FES: Final[str] = "successFEs"
 #: The key for the success time millis.
 KEY_SUCCESS_TIME_MILLIS: Final[str] = "successTimeMillis"
 #: The key for the ERT in FEs.
@@ -52,41 +67,41 @@
 
 #: the internal getters that can work directly
 _GETTERS_0: Final[dict[str, Callable[["EndStatistics"],
                                      int | float | None]]] = {
     KEY_N_SUCCESS: lambda s: s.n_success,
     KEY_ERT_FES: lambda s: s.ert_fes,
     KEY_ERT_TIME_MILLIS: lambda s: s.ert_time_millis,
-    log.KEY_GOAL_F: lambda s: s.goal_f if isinstance(s.goal_f,
-                                                     int | float) else None,
-    log.KEY_MAX_TIME_MILLIS: lambda s: s.max_time_millis
+    KEY_GOAL_F: lambda s: s.goal_f if isinstance(s.goal_f,
+                                                 int | float) else None,
+    KEY_MAX_TIME_MILLIS: lambda s: s.max_time_millis
     if isinstance(s.max_time_millis, int | float) else None,
-    log.KEY_MAX_FES: lambda s: s.max_fes
+    KEY_MAX_FES: lambda s: s.max_fes
     if isinstance(s.max_fes, int | float) else None,
 }
 
 #: the internal getters that access end statistics
 _GETTERS_1: Final[dict[
     str, Callable[["EndStatistics"], int | float | Statistics | None]]] = {
-    log.KEY_LAST_IMPROVEMENT_FE: lambda s: s.last_improvement_fe,
-    log.KEY_LAST_IMPROVEMENT_TIME_MILLIS:
+    KEY_LAST_IMPROVEMENT_FE: lambda s: s.last_improvement_fe,
+    KEY_LAST_IMPROVEMENT_TIME_MILLIS:
         lambda s: s.last_improvement_time_millis,
-    log.KEY_TOTAL_FES: lambda s: s.total_fes,
-    log.KEY_TOTAL_TIME_MILLIS: lambda s: s.total_time_millis,
+    KEY_TOTAL_FES: lambda s: s.total_fes,
+    KEY_TOTAL_TIME_MILLIS: lambda s: s.total_time_millis,
     F_NAME_RAW: lambda s: s.best_f,
     F_NAME_SCALED: lambda s: s.best_f_scaled,
-    log.KEY_MAX_TIME_MILLIS: lambda s: s.max_time_millis,
-    log.KEY_MAX_FES: lambda s: s.max_fes,
-    log.KEY_GOAL_F: lambda s: s.goal_f,
+    KEY_MAX_TIME_MILLIS: lambda s: s.max_time_millis,
+    KEY_MAX_FES: lambda s: s.max_fes,
+    KEY_GOAL_F: lambda s: s.goal_f,
 }
-_GETTERS_1[log.KEY_BEST_F] = _GETTERS_1[F_NAME_RAW]
+_GETTERS_1[KEY_BEST_F] = _GETTERS_1[F_NAME_RAW]
 _GETTERS_1[KEY_BEST_F_SCALED] = _GETTERS_1[F_NAME_SCALED]
 
 
-@dataclass(frozen=True, init=False, order=True)
+@dataclass(frozen=True, init=False, order=False, eq=False)
 class EndStatistics(MultiRunData):
     """
     Statistics over end results of one or multiple algorithm*instance setups.
 
     If one algorithm*instance is used, then `algorithm` and `instance` are
     defined. Otherwise, only the parameter which is the same over all recorded
     runs is defined.
@@ -122,14 +137,16 @@
     max_fes: Statistics | int | None
     #: The budget in milliseconds, if every run had one; None otherwise.
     max_time_millis: Statistics | int | None
 
     def __init__(self,
                  algorithm: str | None,
                  instance: str | None,
+                 objective: str | None,
+                 encoding: str | None,
                  n: int,
                  best_f: Statistics,
                  last_improvement_fe: Statistics,
                  last_improvement_time_millis: Statistics,
                  total_fes: Statistics,
                  total_time_millis: Statistics,
                  goal_f: float | int | Statistics | None,
@@ -144,14 +161,18 @@
         """
         Create the end statistics of an experiment-setup combination.
 
         :param algorithm: the algorithm name, if all runs are with the same
             algorithm
         :param instance: the instance name, if all runs are on the same
             instance
+        :param objective: the objective name, if all runs are on the same
+            objective function, `None` otherwise
+        :param encoding: the encoding name, if all runs are on the same
+            encoding and an encoding was actually used, `None` otherwise
         :param n: the total number of runs
         :param best_f: statistics about the best achieved result
         :param last_improvement_fe: statistics about the last improvement FE
         :param last_improvement_time_millis: statistics about the last
             improvement time
         :param total_fes: statistics about the total FEs
         :param total_time_millis: statistics about the total runtime in
@@ -175,17 +196,17 @@
         :param ert_fes: if `goal_f` is always defined, then this is the
             empirically estimated running time to solve the problem in FEs if
             `n_success>0` and `inf` otherwise
         :param ert_time_millis: if `goal_f` is always defined, then this is
             the empirically estimated running time to solve the problem in
             milliseconds if `n_success>0` and `inf` otherwise
         :param max_fes: the budget in FEs, if any
-        :param max_time_millis: the budget in term of milliseconds
+        :param max_time_millis: the budget in terms of milliseconds
         """
-        super().__init__(algorithm, instance, n)
+        super().__init__(algorithm, instance, objective, encoding, n)
 
         if not isinstance(best_f, Statistics):
             raise type_error(best_f, "best_f", Statistics)
         object.__setattr__(self, "best_f", best_f)
 
         if not isinstance(last_improvement_fe, Statistics):
             raise type_error(last_improvement_fe, "last_improvement_fe",
@@ -427,26 +448,34 @@
         success_fes: list[int] | None = []
         success_times: list[int] | None = []
 
         fes: int = 0
         time: int = 0
         algorithm: str | None = None
         instance: str | None = None
+        objective: str | None = None
+        encoding: str | None = None
 
         for er in source:
             if not isinstance(er, EndResult):
                 raise type_error(er, "end result", EndResult)
             if n == 0:
                 algorithm = er.algorithm
                 instance = er.instance
+                objective = er.objective
+                encoding = er.encoding
             else:
                 if algorithm != er.algorithm:
                     algorithm = None
                 if instance != er.instance:
                     instance = None
+                if objective != er.objective:
+                    objective = None
+                if encoding != er.encoding:
+                    encoding = None
             n += 1
             best_f.append(er.best_f)
             last_improvement_fe.append(er.last_improvement_fe)
             last_improvement_time_millis.append(
                 er.last_improvement_time_millis)
             total_fes.append(er.total_fes)
             total_time_millis.append(er.total_time_millis)
@@ -493,14 +522,16 @@
                     time += er.total_time_millis
         if n <= 0:
             raise ValueError("There must be at least one end result record.")
 
         return EndStatistics(
             algorithm,
             instance,
+            objective,
+            encoding,
             n,
             Statistics.create(best_f),
             Statistics.create(last_improvement_fe),
             Statistics.create(last_improvement_time_millis),
             Statistics.create(total_fes),
             Statistics.create(total_time_millis),
             None if (goal_f is None)
@@ -522,47 +553,61 @@
             else (max_time_millis[0] if max_time_same
                   else Statistics.create(max_time_millis)))
 
     @staticmethod
     def from_end_results(source: Iterable[EndResult],
                          consumer: Callable[["EndStatistics"], Any],
                          join_all_algorithms: bool = False,
-                         join_all_instances: bool = False) -> None:
+                         join_all_instances: bool = False,
+                         join_all_objectives: bool = False,
+                         join_all_encodings: bool = False) -> None:
         """
         Aggregate statistics over a stream of end results.
 
         :param source: the stream of end results
         :param consumer: the destination to which the new records will be
             sent, can be the `append` method of a :class:`list`
         :param join_all_algorithms: should the statistics be aggregated
             over all algorithms
         :param join_all_instances: should the statistics be aggregated
             over all algorithms
+        :param join_all_objectives: should the statistics be aggregated over
+            all objectives?
+        :param join_all_encodings: should statistics be aggregated over all
+            encodings
         """
         if not isinstance(source, Iterable):
             raise type_error(source, "source", Iterable)
         if not callable(consumer):
             raise type_error(consumer, "consumer", call=True)
         if not isinstance(join_all_algorithms, bool):
             raise type_error(join_all_algorithms,
                              "join_all_algorithms", bool)
         if not isinstance(join_all_instances, bool):
             raise type_error(join_all_instances, "join_all_instances", bool)
+        if not isinstance(join_all_objectives, bool):
+            raise type_error(join_all_objectives, "join_all_objectives", bool)
+        if not isinstance(join_all_encodings, bool):
+            raise type_error(join_all_encodings, "join_all_encodings", bool)
 
-        if join_all_algorithms and join_all_instances:
+        if (join_all_algorithms and join_all_instances
+                and join_all_objectives and join_all_encodings):
             consumer(EndStatistics.create(source))
             return
 
-        sorter: dict[tuple[str, str], list[EndResult]] = {}
+        sorter: dict[tuple[str, str, str, str], list[EndResult]] = {}
         for er in source:
             if not isinstance(er, EndResult):
                 raise type_error(source, "end results from source",
                                  EndResult)
             key = ("" if join_all_algorithms else er.algorithm,
-                   "" if join_all_instances else er.instance)
+                   "" if join_all_instances else er.instance,
+                   "" if join_all_objectives else er.objective,
+                   "" if join_all_encodings else (
+                       "" if er.encoding is None else er.encoding))
             if key in sorter:
                 lst = sorter[key]
             else:
                 lst = []
                 sorter[key] = lst
             lst.append(er)
 
@@ -589,108 +634,122 @@
         """
         path: Final[Path] = Path.path(file)
         logger(f"Writing end result statistics to CSV file {path!r}.")
         Path.path(os.path.dirname(path)).ensure_dir_exists()
 
         has_algorithm: bool = False  # 1
         has_instance: bool = False  # 2
-        has_goal_f: int = 0  # 4
-        has_best_f_scaled: bool = False  # 8
-        has_n_success: bool = False  # 16
-        has_success_fes: bool = False  # 32
-        has_success_time_millis: bool = False  # 64
-        has_ert_fes: bool = False  # 128
-        has_ert_time_millis: bool = False  # 256
-        has_max_fes: int = 0  # 512
-        has_max_time_millis: int = 0  # 1024
-        checker: int = 2047
+        has_objective: bool = False  # 4
+        has_encoding: bool = False  # 8
+        has_goal_f: int = 0  # 16
+        has_best_f_scaled: bool = False  # 32
+        has_n_success: bool = False  # 64
+        has_success_fes: bool = False  # 128
+        has_success_time_millis: bool = False  # 256
+        has_ert_fes: bool = False  # 512
+        has_ert_time_millis: bool = False  # 1024
+        has_max_fes: int = 0  # 2048
+        has_max_time_millis: int = 0  # 4096
+        checker: int = 8191
 
         if isinstance(data, EndStatistics):
             data = [data]
 
         for es in data:
             if es.algorithm is not None:
                 has_algorithm = True
                 checker &= ~1
             if es.instance is not None:
                 has_instance = True
                 checker &= ~2
+            if es.objective is not None:
+                has_objective = True
+                checker &= ~4
+            if es.encoding is not None:
+                has_encoding = True
+                checker &= ~8
             if es.goal_f is not None:
                 if isinstance(es.goal_f, Statistics) \
                         and (es.goal_f.maximum > es.goal_f.minimum):
                     has_goal_f = 2
-                    checker &= ~4
+                    checker &= ~16
                 elif has_goal_f == 0:
                     has_goal_f = 1
             if es.best_f_scaled is not None:
                 has_best_f_scaled = True
-                checker &= ~8
+                checker &= ~32
             if es.n_success is not None:
                 has_n_success = True
-                checker &= ~8
+                checker &= ~64
             if es.success_fes is not None:
                 has_success_fes = True
-                checker &= ~32
+                checker &= ~128
             if es.success_time_millis is not None:
                 has_success_time_millis = True
-                checker &= ~64
+                checker &= ~256
             if es.ert_fes is not None:
                 has_ert_fes = True
-                checker &= ~128
+                checker &= ~512
             if es.ert_time_millis is not None:
                 has_ert_time_millis = True
-                checker &= ~256
+                checker &= ~1024
             if es.max_fes is not None:
                 if isinstance(es.max_fes, Statistics) \
                         and (es.max_fes.maximum > es.max_fes.minimum):
                     has_max_fes = 2
-                    checker &= ~512
+                    checker &= ~2048
                 elif has_max_fes == 0:
                     has_max_fes = 1
             if es.max_time_millis is not None:
                 if isinstance(es.max_time_millis, Statistics) \
                         and (es.max_time_millis.maximum
                              > es.max_time_millis.minimum):
                     has_max_time_millis = 2
-                    checker &= ~1024
+                    checker &= ~4096
                 elif has_max_time_millis == 0:
                     has_max_time_millis = 1
             if checker == 0:
                 break
 
         with path.open_for_write() as out:
             wrt: Final[Callable] = out.write
             sep: Final[str] = CSV_SEPARATOR
             if has_algorithm:
-                wrt(log.KEY_ALGORITHM)
+                wrt(KEY_ALGORITHM)
                 wrt(sep)
             if has_instance:
-                wrt(log.KEY_INSTANCE)
+                wrt(KEY_INSTANCE)
+                wrt(sep)
+            if has_objective:
+                wrt(KEY_OBJECTIVE_FUNCTION)
+                wrt(sep)
+            if has_encoding:
+                wrt(KEY_ENCODING)
                 wrt(sep)
 
             def h(p) -> None:
                 wrt(sep.join(Statistics.csv_col_names(p)))
 
             wrt(KEY_N)
             wrt(sep)
-            h(log.KEY_BEST_F)
+            h(KEY_BEST_F)
             wrt(sep)
-            h(log.KEY_LAST_IMPROVEMENT_FE)
+            h(KEY_LAST_IMPROVEMENT_FE)
             wrt(sep)
-            h(log.KEY_LAST_IMPROVEMENT_TIME_MILLIS)
+            h(KEY_LAST_IMPROVEMENT_TIME_MILLIS)
             wrt(sep)
-            h(log.KEY_TOTAL_FES)
+            h(KEY_TOTAL_FES)
             wrt(sep)
-            h(log.KEY_TOTAL_TIME_MILLIS)
+            h(KEY_TOTAL_TIME_MILLIS)
             if has_goal_f == 1:
                 wrt(sep)
-                wrt(log.KEY_GOAL_F)
+                wrt(KEY_GOAL_F)
             elif has_goal_f == 2:
                 wrt(sep)
-                h(log.KEY_GOAL_F)
+                h(KEY_GOAL_F)
             if has_best_f_scaled:
                 wrt(sep)
                 h(KEY_BEST_F_SCALED)
             if has_n_success:
                 wrt(sep)
                 wrt(KEY_N_SUCCESS)
             if has_success_fes:
@@ -703,38 +762,46 @@
                 wrt(sep)
                 wrt(KEY_ERT_FES)
             if has_ert_time_millis:
                 wrt(sep)
                 wrt(KEY_ERT_TIME_MILLIS)
             if has_max_fes == 1:
                 wrt(sep)
-                wrt(log.KEY_MAX_FES)
+                wrt(KEY_MAX_FES)
             elif has_max_fes == 2:
                 wrt(sep)
-                h(log.KEY_MAX_FES)
+                h(KEY_MAX_FES)
             if has_max_time_millis == 1:
                 wrt(sep)
-                wrt(log.KEY_MAX_TIME_MILLIS)
+                wrt(KEY_MAX_TIME_MILLIS)
             elif has_max_time_millis == 2:
                 wrt(sep)
-                h(log.KEY_MAX_TIME_MILLIS)
+                h(KEY_MAX_TIME_MILLIS)
             out.write("\n")
 
             csv: Final[Callable] = Statistics.value_to_csv
             num: Final[Callable] = num_to_str
 
             for er in data:
                 if has_algorithm:
                     if er.algorithm is not None:
                         wrt(er.algorithm)
                     wrt(sep)
                 if has_instance:
                     if er.instance is not None:
                         wrt(er.instance)
                     wrt(sep)
+                if has_objective:
+                    if er.objective is not None:
+                        wrt(er.objective)
+                    wrt(sep)
+                if has_encoding:
+                    if er.encoding is not None:
+                        wrt(er.encoding)
+                    wrt(sep)
                 wrt(str(er.n))
                 wrt(sep)
                 wrt(er.best_f.to_csv())
                 wrt(sep)
                 wrt(er.last_improvement_fe.to_csv())
                 wrt(sep)
                 wrt(er.last_improvement_time_millis.to_csv())
@@ -841,39 +908,45 @@
             header: Final[list[str]] = [ss.strip()
                                         for ss in headerstr.split(sep)]
             if len(header) <= 3:
                 raise ValueError(
                     f"Invalid header {headerstr!r} in file {file!r}.")
 
             idx = 0
-            has_algorithm: bool
-            if header[0] == log.KEY_ALGORITHM:
+            has_algorithm: bool = False
+            if header[0] == KEY_ALGORITHM:
                 has_algorithm = True
                 idx = 1
-            else:
-                has_algorithm = False
 
-            has_instance: bool
-            if header[idx] == log.KEY_INSTANCE:
+            has_instance: bool = False
+            if header[idx] == KEY_INSTANCE:
                 has_instance = True
                 idx += 1
-            else:
-                has_instance = False
+
+            has_objective: bool = False
+            if header[idx] == KEY_OBJECTIVE_FUNCTION:
+                has_objective = True
+                idx += 1
+
+            has_encoding: bool = False
+            if header[idx] == KEY_ENCODING:
+                has_encoding = True
+                idx += 1
 
             csv: Final[Callable] = Statistics.csv_col_names
 
             if header[idx] != KEY_N:
                 raise ValueError(
                     f"Expected to find {KEY_N!r} at index {idx} "
                     f"in header {headerstr!r} of file {path!r}.")
             idx += 1
 
-            for key in [log.KEY_BEST_F, log.KEY_LAST_IMPROVEMENT_FE,
-                        log.KEY_LAST_IMPROVEMENT_TIME_MILLIS,
-                        log.KEY_TOTAL_FES, log.KEY_TOTAL_TIME_MILLIS]:
+            for key in [KEY_BEST_F, KEY_LAST_IMPROVEMENT_FE,
+                        KEY_LAST_IMPROVEMENT_TIME_MILLIS,
+                        KEY_TOTAL_FES, KEY_TOTAL_TIME_MILLIS]:
                 if csv(key) != header[idx:(idx + CSV_COLS)]:
                     raise ValueError(
                         f"Expected to find '{key}.*' keys from index "
                         f"{idx} on in header "
                         f"{headerstr!r} of file {path!r}, expected "
                         f"{csv(key)} but got {header[idx:(idx + CSV_COLS)]}.")
                 idx += CSV_COLS
@@ -884,22 +957,22 @@
             has_success_fes: bool = False
             has_success_time: bool = False
             has_ert_fes: bool = False
             has_ert_time: bool = False
             has_max_fes: int = 0
             has_max_time: int = 0
             while idx <= len(header):
-                if header[idx] == log.KEY_GOAL_F:
+                if header[idx] == KEY_GOAL_F:
                     has_goal_f = 1
                     idx += 1
-                elif header[idx].startswith(log.KEY_GOAL_F):
+                elif header[idx].startswith(KEY_GOAL_F):
                     has_goal_f = 2
-                    if csv(log.KEY_GOAL_F) != header[idx:(idx + CSV_COLS)]:
+                    if csv(KEY_GOAL_F) != header[idx:(idx + CSV_COLS)]:
                         raise ValueError(
-                            f"Expected to find '{log.KEY_GOAL_F}.*' keys from "
+                            f"Expected to find '{KEY_GOAL_F}.*' keys from "
                             f"index {idx} on in header "
                             f"{headerstr!r} of file {path!r}.")
                     idx += CSV_COLS
 
                 if idx >= len(header):
                     break
 
@@ -958,37 +1031,37 @@
                 if header[idx] == KEY_ERT_TIME_MILLIS:
                     has_ert_time = True
                     idx += 1
 
                 if idx >= len(header):
                     break
 
-                if header[idx] == log.KEY_MAX_FES:
+                if header[idx] == KEY_MAX_FES:
                     has_max_fes = 1
                     idx += 1
-                elif header[idx].startswith(log.KEY_MAX_FES):
+                elif header[idx].startswith(KEY_MAX_FES):
                     has_max_fes = 2
-                    if csv(log.KEY_MAX_FES) != header[idx:(idx + CSV_COLS)]:
+                    if csv(KEY_MAX_FES) != header[idx:(idx + CSV_COLS)]:
                         raise ValueError(
-                            f"Expected to find '{log.KEY_MAX_FES}.*' keys"
+                            f"Expected to find '{KEY_MAX_FES}.*' keys"
                             f" from index {idx} on in header "
                             f"{headerstr!r} of file {path!r}.")
                     idx += CSV_COLS
 
                 if idx >= len(header):
                     break
 
-                if header[idx] == log.KEY_MAX_TIME_MILLIS:
+                if header[idx] == KEY_MAX_TIME_MILLIS:
                     has_max_time = 1
                     idx += 1
-                elif header[idx].startswith(log.KEY_MAX_TIME_MILLIS):
+                elif header[idx].startswith(KEY_MAX_TIME_MILLIS):
                     has_max_time = 2
-                    if csv(log.KEY_MAX_FES) != header[idx:(idx + CSV_COLS)]:
+                    if csv(KEY_MAX_FES) != header[idx:(idx + CSV_COLS)]:
                         raise ValueError(
-                            f"Expected to find '{log.KEY_MAX_TIME_MILLIS}.*' "
+                            f"Expected to find '{KEY_MAX_TIME_MILLIS}.*' "
                             f"keys from index {idx} on in header "
                             f"{headerstr!r} of file {path!r}.")
                     idx += CSV_COLS
 
                 break
 
             if len(header) > idx:
@@ -1000,34 +1073,44 @@
                 lines = rd.readlines(100)
                 if (lines is None) or (len(lines) <= 0):
                     break
                 for line in lines:
                     row = [ss.strip() for ss in line.strip().split(sep)]
 
                     idx = 0
-                    algo: str | None = None
-                    inst: str | None = None
+                    algorithm: str | None = None
+                    instance: str | None = None
+                    objective: str | None = None
+                    encoding: str | None = None
                     n: int
                     goal_f: None | int | float | Statistics = None
                     best_f_scaled: Statistics | None = None
                     n_success: int | None = None
                     success_fes: Statistics | None = None
                     success_time: Statistics | None = None
                     ert_fes: int | float | None = None
                     ert_time: int | float | None = None
                     max_fes: int | Statistics | None = None
                     max_time: int | Statistics | None = None
 
                     try:
                         if has_algorithm:
-                            algo = sanitize_name(row[0])
+                            algorithm = sanitize_name(row[0])
                             idx += 1
 
                         if has_instance:
-                            inst = sanitize_name(row[idx])
+                            instance = sanitize_name(row[idx])
+                            idx += 1
+
+                        if has_objective:
+                            objective = sanitize_name(row[idx])
+                            idx += 1
+
+                        if has_encoding:
+                            encoding = sanitize_name(row[idx])
                             idx += 1
 
                         n = int(row[idx])
                         idx += 1
 
                         best_f: Statistics = Statistics.from_csv(
                             n, row[idx:(idx + CSV_COLS)])
@@ -1108,18 +1191,19 @@
                         raise ValueError(
                             f"Invalid row {line!r} in file {path!r}.") from be
 
                     if len(row) != idx:
                         raise ValueError("Invalid number of columns in row "
                                          f"{line!r} in file {path!r}.")
                     consumer(EndStatistics(
-                        algo, inst, n, best_f, last_improv_fe,
-                        last_improv_time, total_fes, total_time, goal_f,
-                        best_f_scaled, n_success, success_fes, success_time,
-                        ert_fes, ert_time, max_fes, max_time))
+                        algorithm, instance, objective, encoding, n, best_f,
+                        last_improv_fe, last_improv_time, total_fes,
+                        total_time, goal_f, best_f_scaled, n_success,
+                        success_fes, success_time, ert_fes, ert_time, max_fes,
+                        max_time))
 
         logger("Finished reading end result statistics from CSV "
                f"file {path!r}.")
 
     @staticmethod
     def getter(dimension: str) -> Callable[["EndStatistics"],
                                            int | float | None]:
@@ -1206,14 +1290,24 @@
              " are not separated by algorithm but all algorithms are treated "
              "as one", action="store_true")
     parser.add_argument(
         "--join_instances",
         help="compute statistics over all instances, i.e., the statistics"
              " are not separated by instance but all instances are treated "
              "as one", action="store_true")
+    parser.add_argument(
+        "--join_objectives",
+        help="compute statistics over all objective functions, i.e., the "
+             "statistics are not separated by objective functions but all "
+             "objectives functions are treated as one", action="store_true")
+    parser.add_argument(
+        "--join_encodings",
+        help="compute statistics over all encodings, i.e., the statistics"
+             " are not separated by encodings but all encodings are treated "
+             "as one", action="store_true")
     args: Final[argparse.Namespace] = parser.parse_args()
 
     src_path: Final[Path] = args.source
     end_results: Final[list[EndResult]] = []
     if src_path.is_file():
         logger(f"{src_path!r} identifies file, load as end-results csv")
         EndResult.from_csv(src_path, end_results.append)
@@ -1221,9 +1315,11 @@
         logger(f"{src_path!r} identifies directory, load it as log files")
         EndResult.from_logs(src_path, end_results.append)
 
     end_stats: Final[list[EndStatistics]] = []
     EndStatistics.from_end_results(
         source=end_results, consumer=end_stats.append,
         join_all_algorithms=args.join_algorithms,
-        join_all_instances=args.join_instances)
+        join_all_instances=args.join_instances,
+        join_all_objectives=args.join_objectives,
+        join_all_encodings=args.join_encodings)
     EndStatistics.to_csv(end_stats, args.dest)
```

### Comparing `moptipy-0.9.90/moptipy/evaluation/ert.py` & `moptipy-0.9.91/moptipy/evaluation/ert.py`

 * *Files 6% similar despite different names*

```diff
@@ -32,31 +32,36 @@
 
 from dataclasses import dataclass
 from math import inf, isfinite
 from typing import Any, Callable, Final, Iterable, cast
 
 import numpy as np
 
-import moptipy.api.logging as lg
-import moptipy.utils.nputils as npu
+from moptipy.api.logging import (
+    KEY_ALGORITHM,
+    KEY_INSTANCE,
+)
 from moptipy.evaluation._utils import _get_goal_reach_index
 from moptipy.evaluation.base import (
     F_NAME_NORMALIZED,
     F_NAME_RAW,
     F_NAME_SCALED,
+    KEY_ENCODING,
     KEY_N,
+    KEY_OBJECTIVE_FUNCTION,
     MultiRun2DData,
 )
 from moptipy.evaluation.progress import Progress
 from moptipy.utils.console import logger
 from moptipy.utils.logger import (
     COMMENT_CHAR,
     CSV_SEPARATOR,
     KEY_VALUE_SEPARATOR,
 )
+from moptipy.utils.nputils import DEFAULT_FLOAT, DEFAULT_INT, is_all_finite
 from moptipy.utils.path import Path
 from moptipy.utils.strings import num_to_str
 from moptipy.utils.types import type_error
 
 
 def compute_single_ert(source: Iterable[Progress],
                        goal_f: int | float) -> float:
@@ -78,18 +83,18 @@
     :param goal_f: the goal objective value
     :return: the ERT
 
     >>> from moptipy.evaluation.progress import Progress as Pr
     >>> from numpy import array as a
     >>> f = "plainF"
     >>> t = "FEs"
-    >>> r = [Pr("a", "i", 1, a([1, 4, 8]), t, a([10, 8, 5]), f),
-    ...      Pr("a", "i", 2, a([1, 3, 6]), t, a([9, 7, 4]), f),
-    ...      Pr("a", "i", 3, a([1, 2, 7, 9]), t, a([8, 7, 6, 3]), f),
-    ...      Pr("a", "i", 4, a([1, 12]), t, a([9, 3]), f)]
+    >>> r = [Pr("a", "i", "f", "e", 1, a([1, 4, 8]), t, a([10, 8, 5]), f),
+    ...      Pr("a", "i", "f", "e", 2, a([1, 3, 6]), t, a([9, 7, 4]), f),
+    ...      Pr("a", "i", "f", "e", 3, a([1, 2, 7, 9]), t, a([8, 7, 6, 3]), f),
+    ...      Pr("a", "i", "f", "e", 4, a([1, 12]), t, a([9, 3]), f)]
     >>> print(compute_single_ert(r, 11))
     1.0
     >>> print(compute_single_ert(r, 10))
     1.0
     >>> print(compute_single_ert(r, 9.5))  # (4 + 1 + 1 + 1) / 4 = 1.75
     1.75
     >>> print(compute_single_ert(r, 9))  # (4 + 1 + 1 + 1) / 4 = 1.75
@@ -135,57 +140,64 @@
     if time_sum <= 0:
         raise ValueError(f"Time sum cannot be {time_sum}.")
     if n_success <= 0:
         return inf
     return time_sum / n_success
 
 
-@dataclass(frozen=True, init=False, order=True)
+@dataclass(frozen=True, init=False, order=False, eq=False)
 class Ert(MultiRun2DData):
     """Estimate the Expected Running Time (ERT)."""
 
     #: The ert function
     ert: np.ndarray
 
     def __init__(self,
                  algorithm: str | None,
                  instance: str | None,
+                 objective: str | None,
+                 encoding: str | None,
                  n: int,
                  time_unit: str,
                  f_name: str,
                  ert: np.ndarray):
         """
         Create the Ert function.
 
         :param algorithm: the algorithm name, if all runs are with the same
             algorithm
         :param instance: the instance name, if all runs are on the same
             instance
+        :param objective: the objective name, if all runs are on the same
+            objective function, `None` otherwise
+        :param encoding: the encoding name, if all runs are on the same
+            encoding and an encoding was actually used, `None` otherwise
         :param n: the total number of runs
         :param time_unit: the time unit
         :param f_name: the objective dimension name
         :param ert: the ert matrix
         """
-        super().__init__(algorithm, instance, n, time_unit, f_name)
+        super().__init__(algorithm, instance, objective, encoding, n,
+                         time_unit, f_name)
         if not isinstance(ert, np.ndarray):
             raise type_error(ert, "ert", np.ndarray)
         ert.flags.writeable = False
 
         f: Final[np.ndarray] = ert[:, 0]
-        if not npu.is_all_finite(f):
+        if not is_all_finite(f):
             raise ValueError(
                 f"Ert x-axis must be all finite, but encountered {f}.")
         ll = f.size
         if (ll > 1) and np.any(f[1:] <= f[:-1]):
             raise ValueError("f data must be strictly increasing,"
                              f"but encountered {f}.")
 
         t: Final[np.ndarray] = ert[:, 1]
         if np.isfinite(t[0]) or (np.isposinf(t[0])):
-            if not npu.is_all_finite(t[1:]):
+            if not is_all_finite(t[1:]):
                 raise ValueError(
                     "non-first ert y-axis elements must be all finite.")
             if np.any(t[1:] >= t[:-1]):
                 raise ValueError("t data must be strictly decreasing,"
                                  f"but encountered {t}.")
         else:
             raise ValueError(
@@ -202,29 +214,31 @@
         :return: the fully resolved file name
         """
         path: Final[Path] = Path.path(file)
         logger(f"Writing ERT to CSV file {path!r}.")
 
         with path.open_for_write() as out:
             sep: Final[str] = CSV_SEPARATOR
+            write: Callable[[str], int] = out.write
             if put_header:
                 kv: Final[str] = KEY_VALUE_SEPARATOR
                 cmt: Final[str] = COMMENT_CHAR
                 if self.algorithm is not None:
-                    out.write(
-                        f"{cmt} {lg.KEY_ALGORITHM}{kv}{self.algorithm}\n")
+                    write(f"{cmt} {KEY_ALGORITHM}{kv}{self.algorithm}\n")
                 if self.instance is not None:
-                    out.write(
-                        f"{cmt} {lg.KEY_INSTANCE}{kv}{self.instance}\n")
-                out.write(
-                    f"{cmt} {KEY_N}{kv}{self.n}\n")
-            out.write(f"{self.f_name}{sep}ert[{self.time_unit}]\n")
+                    write(f"{cmt} {KEY_INSTANCE}{kv}{self.instance}\n")
+                if self.objective is not None:
+                    write(f"{cmt} {KEY_OBJECTIVE_FUNCTION}{kv}"
+                          f"{self.objective}\n")
+                if self.encoding is not None:
+                    write(f"{cmt} {KEY_ENCODING}{kv}{self.encoding}\n")
+                write(f"{cmt} {KEY_N}{kv}{self.n}\n")
+            write(f"{self.f_name}{sep}ert[{self.time_unit}]\n")
             for v in self.ert:
-                out.write(
-                    f"{num_to_str(v[0])}{sep}{num_to_str(v[1])}\n")
+                write(f"{num_to_str(v[0])}{sep}{num_to_str(v[1])}\n")
 
         logger(f"Done writing ERT to CSV file {path!r}.")
 
         path.enforce_file()
         return path
 
     @staticmethod
@@ -251,35 +265,43 @@
                 raise ValueError("f_lower_bound must be finite "
                                  f"but is {f_lower_bound}.")
             lower_bound = f_lower_bound
             f_lower_bound = None
 
         algorithm: str | None = None
         instance: str | None = None
+        objective: str | None = None
+        encoding: str | None = None
         time_unit: str | None = None
         f_name: str | None = None
         f_list: list[np.ndarray] = []
         n: int = 0
 
         prgs: Final[list[Progress]] = cast(list[Progress], source) \
             if isinstance(source, list) else list(source)
 
         for progress in prgs:
             if not isinstance(progress, Progress):
                 raise type_error(progress, "progress input", Progress)
             if n <= 0:
                 algorithm = progress.algorithm
                 instance = progress.instance
+                objective = progress.objective
+                encoding = progress.encoding
                 time_unit = progress.time_unit
                 f_name = progress.f_name
             else:
                 if algorithm != progress.algorithm:
                     algorithm = None
                 if instance != progress.instance:
                     instance = None
+                if objective != progress.objective:
+                    objective = None
+                if encoding != progress.encoding:
+                    encoding = None
                 if time_unit != progress.time_unit:
                     raise ValueError(
                         f"Cannot mix time units {time_unit} "
                         f"and {progress.time_unit}.")
                 if f_name != progress.f_name:
                     raise ValueError(f"Cannot mix f-names {f_name} "
                                      f"and {progress.f_name}.")
@@ -317,16 +339,16 @@
         x = np.unique(x)
         if has_lb:
             x = x[x >= lower_bound]
         base_len: Final[int] = x.size
 
         # prepare for backward iteration over arrays
         indices = np.array([(ppr.f.size - 1) for ppr in prgs],
-                           dtype=npu.DEFAULT_INT)
-        y = np.empty(base_len, dtype=npu.DEFAULT_FLOAT)
+                           dtype=DEFAULT_INT)
+        y = np.empty(base_len, dtype=DEFAULT_FLOAT)
 
         for out_index in range(base_len):
             f_lim = x[out_index]
             found = 0
             time_sum: int = 0
             for r_idx, pr in enumerate(prgs):
                 idx = indices[r_idx]
@@ -345,71 +367,79 @@
 
             # compute ert value: infinite if no run meets condition
             y[out_index] = inf if (found <= 0) else time_sum / found
 
         # convert the two arrays into one matrix
         ert = np.concatenate((x, y)).reshape((base_len, 2), order="F")
 
-        return Ert(algorithm, instance, n,
+        return Ert(algorithm, instance, objective, encoding, n,
                    time_unit, f_name, ert)
 
     @staticmethod
     def from_progresses(source: Iterable[Progress],
                         consumer: Callable[["Ert"], Any],
                         f_lower_bound: float | None = None,
                         use_default_lower_bounds: bool = True,
                         join_all_algorithms: bool = False,
-                        join_all_instances: bool = False) -> None:
+                        join_all_instances: bool = False,
+                        join_all_objectives: bool = False,
+                        join_all_encodings: bool = False) -> None:
         """
         Compute one or multiple ERTs from a stream of end results.
 
         :param source: the set of progress instances
         :param f_lower_bound: the lower bound for the objective value
         :param use_default_lower_bounds: should we use the default lower
             bounds
         :param consumer: the destination to which the new records will be
             passed, can be the `append` method of a :class:`list`
         :param join_all_algorithms: should the Ert be aggregated over all
             algorithms
         :param join_all_instances: should the Ert be aggregated over all
             algorithms
+        :param join_all_objectives: should the statistics be aggregated over
+            all objective functions?
+        :param join_all_encodings: should the statistics be aggregated over
+            all encodings?
         """
         if not isinstance(source, Iterable):
             raise type_error(source, "source", Iterable)
         if not callable(consumer):
             raise type_error(consumer, "consumer", call=True)
         if not isinstance(join_all_algorithms, bool):
             raise type_error(join_all_algorithms, "join_all_algorithms", bool)
         if not isinstance(join_all_instances, bool):
             raise type_error(join_all_instances, "join_all_instances", bool)
 
-        if join_all_algorithms and join_all_instances:
+        if (join_all_algorithms and join_all_instances and join_all_objectives
+                and join_all_encodings):
             consumer(Ert.create(source, f_lower_bound,
                                 use_default_lower_bounds))
             return
 
-        sorter: dict[str, list[Progress]] = {}
+        sorter: dict[tuple[str, str, str, str], list[Progress]] = {}
         for er in source:
             if not isinstance(er, Progress):
                 raise type_error(er, "progress source", Progress)
-            key = er.instance if join_all_algorithms else \
-                er.algorithm if join_all_instances else \
-                f"{er.algorithm}/{er.instance}"
+            key = ("" if join_all_algorithms else er.algorithm,
+                   "" if join_all_instances else er.instance,
+                   "" if join_all_objectives else er.objective,
+                   "" if join_all_encodings else (
+                       "" if er.encoding is None else er.encoding))
             if key in sorter:
                 lst = sorter[key]
             else:
                 lst = []
                 sorter[key] = lst
             lst.append(er)
 
         if len(sorter) <= 0:
             raise ValueError("source must not be empty")
 
         if len(sorter) > 1:
-            keyz = list(sorter.keys())
-            keyz.sort()
+            keyz = sorted(sorter.keys())
             for key in keyz:
                 consumer(Ert.create(sorter[key], f_lower_bound,
                                     use_default_lower_bounds))
         else:
             consumer(Ert.create(next(iter(sorter.values())), f_lower_bound,
                                 use_default_lower_bounds))
```

### Comparing `moptipy-0.9.90/moptipy/evaluation/ertecdf.py` & `moptipy-0.9.91/moptipy/evaluation/ertecdf.py`

 * *Files 3% similar despite different names*

```diff
@@ -28,15 +28,15 @@
 from dataclasses import dataclass
 
 from moptipy.evaluation.ecdf import Ecdf
 from moptipy.evaluation.ert import compute_single_ert
 from moptipy.evaluation.progress import Progress
 
 
-@dataclass(frozen=True, init=False, order=True)
+@dataclass(frozen=True, init=False, order=False, eq=False)
 class ErtEcdf(Ecdf):
     """The ERT-ECDF."""
 
     def time_label(self) -> str:
         """
         Get the time axis label.
```

### Comparing `moptipy-0.9.90/moptipy/evaluation/ioh_analyzer.py` & `moptipy-0.9.91/moptipy/evaluation/ioh_analyzer.py`

 * *Files identical despite different names*

### Comparing `moptipy-0.9.90/moptipy/evaluation/log_parser.py` & `moptipy-0.9.91/moptipy/evaluation/log_parser.py`

 * *Files 4% similar despite different names*

```diff
@@ -36,14 +36,16 @@
     KEY_MAX_FES,
     KEY_MAX_TIME_MILLIS,
     KEY_NAME,
     KEY_RAND_SEED,
     KEY_TOTAL_FES,
     KEY_TOTAL_TIME_MILLIS,
     SCOPE_ALGORITHM,
+    SCOPE_ENCODING,
+    SCOPE_OBJECTIVE_FUNCTION,
     SCOPE_PROCESS,
     SECTION_FINAL_STATE,
     SECTION_SETUP,
 )
 from moptipy.evaluation._utils import _check_max_time_millis
 from moptipy.utils.console import logger
 from moptipy.utils.logger import (
@@ -72,14 +74,20 @@
 _FULL_KEY_GOAL_F: Final[str] = f"{SCOPE_PROCESS}{SCOPE_SEPARATOR}{KEY_GOAL_F}"
 #: the random seed
 _FULL_KEY_RAND_SEED: Final[str] = \
     f"{SCOPE_PROCESS}{SCOPE_SEPARATOR}{KEY_RAND_SEED}"
 #: the full algorithm name key
 _FULL_KEY_ALGORITHM: Final[str] = \
     f"{SCOPE_ALGORITHM}{SCOPE_SEPARATOR}{KEY_NAME}"
+#: the full objective function name key
+_FULL_KEY_OBJECTIVE: Final[str] = \
+    f"{SCOPE_OBJECTIVE_FUNCTION}{SCOPE_SEPARATOR}{KEY_NAME}"
+#: the full encoding name key
+_FULL_KEY_ENCODING: Final[str] = \
+    f"{SCOPE_ENCODING}{SCOPE_SEPARATOR}{KEY_NAME}"
 
 
 class LogParser:
     """
     A log parser can parse a log file and separate the sections.
 
     The log parser is designed to load data from text files generated
@@ -529,22 +537,38 @@
     This parser processes the `SETUP` and `STATE` sections of a log file and
     stores the performance-related information in member variables.
     """
 
     def __init__(self):
         """Create the basic data parser."""
         super().__init__()
+        #: the total consumed runtime, in objective function evaluations
         self.total_fes: int | None = None
+        #: the total consumed runtime in milliseconds
         self.total_time_millis: int | None = None
+        #: the best objective function value encountered
         self.best_f: int | float | None = None
+        #: the objective function evaluation when the last improvement
+        #: happened, in milliseconds
         self.last_improvement_fe: int | None = None
+        #: the time step when the last improvement happened, in milliseconds
         self.last_improvement_time_millis: int | None = None
+        #: the goal objective value, if any
         self.goal_f: int | float | None = None
+        #: the maximum permitted number of objective function evaluations,
+        #: if any
         self.max_fes: int | None = None
+        #: the maximum runtime limit in milliseconds, if any
         self.max_time_millis: int | None = None
+        #: The name of the objective to which the current log file belongs.
+        self.objective: str | None = None
+        #: The name of the encoding to which the current log file belongs.
+        self.encoding: str | None = None
+        #: the internal state, an OR mask: 1=after setup section, 2=after
+        #: state section, 4=in setup section, 8=in state section
         self.__state: int = 0
 
     def start_file(self, path: Path) -> bool:
         """
         Begin parsing the file identified by `path`.
 
         :param path: the path identifying the file
@@ -581,14 +605,16 @@
                 f"{SECTION_SETUP!r} section.")
         if self.rand_seed is None:
             raise ValueError("rand_seed is missing.")
         if self.algorithm is None:
             raise ValueError("algorithm is missing.")
         if self.instance is None:
             raise ValueError("instance is missing.")
+        if self.objective is None:
+            raise ValueError("objective is missing.")
         if self.total_fes is None:
             raise ValueError("total_fes is missing.")
         if self.total_time_millis is None:
             raise ValueError("total_time_millis is missing.")
         if self.best_f is None:
             raise ValueError("best_f is missing.")
         if self.last_improvement_fe is None:
@@ -601,14 +627,16 @@
         self.total_time_millis = None
         self.best_f = None
         self.last_improvement_fe = None
         self.last_improvement_time_millis = None
         self.goal_f = None
         self.max_fes = None
         self.max_time_millis = None
+        self.objective = None
+        self.encoding = None
         self.__state = 0
         return super().end_file()
 
     def needs_more_lines(self) -> bool:
         """
         Check whether we need to process more lines.
 
@@ -692,14 +720,24 @@
                 # file names
                 if a.casefold() == self.algorithm.casefold():
                     self.algorithm = a  # rely on name from log file
                 else:  # ok, case was not the issue - raise error
                     raise ValueError(
                         f"algorithm name from file name is {self.algorithm!r}"
                         f", but key {_FULL_KEY_ALGORITHM!r} gives {a!r}.")
+        else:
+            raise ValueError(f"key {_FULL_KEY_ALGORITHM!r} missing in file!")
+
+        if _FULL_KEY_OBJECTIVE in data:
+            self.objective = data[_FULL_KEY_OBJECTIVE]
+        else:
+            raise ValueError(f"key {_FULL_KEY_OBJECTIVE!r} missing in file!")
+
+        self.encoding = data[_FULL_KEY_ENCODING] \
+            if _FULL_KEY_ENCODING in data else None
 
         seed_check = rand_seed_check(int(data[_FULL_KEY_RAND_SEED]))
         if self.rand_seed is None:
             self.rand_seed = seed_check
         elif seed_check != self.rand_seed:
             raise ValueError(
                 f"Found seed {seed_check} in log file, but file name "
```

### Comparing `moptipy-0.9.90/moptipy/evaluation/plot_ecdf.py` & `moptipy-0.9.91/moptipy/evaluation/plot_ecdf.py`

 * *Files identical despite different names*

### Comparing `moptipy-0.9.90/moptipy/evaluation/plot_end_results.py` & `moptipy-0.9.91/moptipy/evaluation/plot_end_results.py`

 * *Files identical despite different names*

### Comparing `moptipy-0.9.90/moptipy/evaluation/plot_end_statistics_over_parameter.py` & `moptipy-0.9.91/moptipy/evaluation/plot_end_statistics_over_parameter.py`

 * *Files identical despite different names*

### Comparing `moptipy-0.9.90/moptipy/evaluation/plot_ert.py` & `moptipy-0.9.91/moptipy/evaluation/plot_ert.py`

 * *Files identical despite different names*

### Comparing `moptipy-0.9.90/moptipy/evaluation/plot_progress.py` & `moptipy-0.9.91/moptipy/evaluation/plot_progress.py`

 * *Files identical despite different names*

### Comparing `moptipy-0.9.90/moptipy/evaluation/progress.py` & `moptipy-0.9.91/moptipy/evaluation/progress.py`

 * *Files 2% similar despite different names*

```diff
@@ -25,14 +25,16 @@
     PROGRESS_FES,
     PROGRESS_TIME_MILLIS,
     SECTION_PROGRESS,
 )
 from moptipy.evaluation.base import (
     F_NAME_RAW,
     F_NAME_SCALED,
+    KEY_ENCODING,
+    KEY_OBJECTIVE_FUNCTION,
     TIME_UNIT_FES,
     TIME_UNIT_MILLIS,
     PerRunData,
     check_f_name,
     check_time_unit,
 )
 from moptipy.evaluation.log_parser import SetupAndStateParser
@@ -44,15 +46,15 @@
 )
 from moptipy.utils.nputils import is_all_finite, is_np_float, is_np_int
 from moptipy.utils.path import Path
 from moptipy.utils.strings import num_to_str, str_to_intfloat
 from moptipy.utils.types import type_error
 
 
-@dataclass(frozen=True, init=False, order=True)
+@dataclass(frozen=True, init=False, order=False, eq=False)
 class Progress(PerRunData):
     """An immutable record of progress information over a single run."""
 
     #: The time axis data.
     time: np.ndarray
 
     #: The unit of the time axis.
@@ -68,37 +70,42 @@
     #: If :attr:`f_name` is `F_NAME_SCALED` or `F_NAME_NORMALIZED`.
     #: then this value has been used to normalize the data.
     f_standard: int | float | None
 
     def __init__(self,
                  algorithm: str,
                  instance: str,
+                 objective: str,
+                 encoding: str | None,
                  rand_seed: int,
                  time: np.ndarray,
                  time_unit: str,
                  f: np.ndarray,
                  f_name: str,
                  f_standard: int | float | None = None,
                  only_improvements: bool = True):
         """
         Create a consistent instance of :class:`EndResult`.
 
         :param algorithm: the algorithm name
         :param instance: the instance name
+        :param objective: the name of the objective function
+        :param encoding: the name of the encoding that was used, if any, or
+            `None` if no encoding was used
         :param rand_seed: the random seed
         :param time: the time axis data
         :param time_unit: the unit of the time axis
         :param f: the objective value axis data
         :param f_name: the name of the objective value axis data
         :param f_standard: the value used to standardize of the objective
             value dimension
         :param only_improvements: enforce that f-values should be
             improving and time values increasing
         """
-        super().__init__(algorithm, instance, rand_seed)
+        super().__init__(algorithm, instance, objective, encoding, rand_seed)
 
         if not isinstance(time, np.ndarray):
             raise type_error(time, "time data", np.ndarray)
         time.flags.writeable = False
         if len(time.shape) != 1:
             raise ValueError("time array must be one-dimensional, but "
                              f"has shape {time.shape}.")
@@ -117,15 +124,15 @@
                 raise ValueError("time data must be monotonously"
                                  f"increasing, but encountered {time}.")
 
         object.__setattr__(self, "time", time)
         object.__setattr__(self, "time_unit", check_time_unit(time_unit))
 
         mintime = 1 if time_unit == TIME_UNIT_FES else 0
-        if any(time < mintime):
+        if np.any(time < mintime):
             raise ValueError(f"No time value can be less than {mintime} if"
                              f" time unit is {time_unit}.")
 
         if not isinstance(f, np.ndarray):
             raise type_error(f, "f data", np.ndarray)
         f.flags.writeable = False
         if len(f.shape) != 1:
@@ -206,29 +213,29 @@
         :return: the fully resolved file name
         """
         path: Final[Path] = Path.path(file)
         logger(f"Writing progress object to CSV file {path!r}.")
 
         with path.open_for_write() as out:
             sep: Final[str] = CSV_SEPARATOR
+            write: Final[Callable[[str], int]] = out.write
             if put_header:
                 kv: Final[str] = KEY_VALUE_SEPARATOR
                 cmt: Final[str] = COMMENT_CHAR
-                out.write(
-                    f"{cmt} {KEY_ALGORITHM}{kv}{self.algorithm}\n")
-                out.write(
-                    f"{cmt} {KEY_INSTANCE}{kv}{self.instance}\n")
-                out.write(f"{cmt} {KEY_RAND_SEED}{kv}"
-                          f"{hex(self.rand_seed)}\n")
+                write(f"{cmt} {KEY_ALGORITHM}{kv}{self.algorithm}\n")
+                write(f"{cmt} {KEY_INSTANCE}{kv}{self.instance}\n")
+                write(f"{cmt} {KEY_OBJECTIVE_FUNCTION}{kv}{self.objective}\n")
+                if self.encoding is not None:
+                    write(f"{cmt} {KEY_ENCODING}{kv}{self.objective}\n")
+                write(f"{cmt} {KEY_RAND_SEED}{kv}{hex(self.rand_seed)}\n")
                 if self.f_standard is not None:
-                    out.write(
-                        f"{cmt} {KEY_GOAL_F}{kv}{self.f_standard}\n")
-            out.write(f"{self.time_unit}{sep}{self.f_name}\n")
+                    write(f"{cmt} {KEY_GOAL_F}{kv}{self.f_standard}\n")
+            write(f"{self.time_unit}{sep}{self.f_name}\n")
             for i, t in enumerate(self.time):
-                out.write(f"{t}{sep}{num_to_str(self.f[i])}\n")
+                write(f"{t}{sep}{num_to_str(self.f[i])}\n")
 
         logger(f"Done writing progress object to CSV file {path!r}.")
 
         path.enforce_file()
         return path
 
 
@@ -313,14 +320,16 @@
         else:
             ff = np.array([(f - f_standard) / f_standard
                            for f in self.__f_collector])
         self.__f_collector.clear()
 
         self.__consumer(Progress(self.algorithm,
                                  self.instance,
+                                 self.objective,
+                                 self.encoding,
                                  self.rand_seed,
                                  np.array(self.__t_collector),
                                  self.__time_unit,
                                  ff,
                                  self.__f_name,
                                  f_standard,
                                  self.__only_improvements))
```

### Comparing `moptipy-0.9.90/moptipy/evaluation/stat_run.py` & `moptipy-0.9.91/moptipy/evaluation/stat_run.py`

 * *Files 15% similar despite different names*

```diff
@@ -131,144 +131,156 @@
     values: Final[np.ndarray] = np.zeros(stat_dim, DEFAULT_FLOAT)
     pos: Final[np.ndarray] = np.array([len(x) - 1 for x in x_raw], DEFAULT_INT)
 
     return __apply_fun(x_unique, x_raw, y_raw, stat_func, out_len,
                        dest_y, stat_dim, values, pos)
 
 
-@numba.njit(parallel=True)
+@numba.njit(cache=True, inline="always", fastmath=False, boundscheck=False,
+            parallel=True)
 def __stat_arith_mean(data: np.ndarray) -> np.number:
     """
     Compute the arithmetic mean.
 
     :param data: the data
     :return: the arithmetic mean
     """
     return data.mean()
 
 
-@numba.njit(parallel=True)
+@numba.njit(cache=True, inline="always", fastmath=False, boundscheck=False,
+            parallel=True)
 def __stat_geo_mean(data: np.ndarray) -> np.number:
     """
     Compute the geometric mean.
 
     :param data: the data
     :return: the geometric mean
     """
     return np.exp(np.mean(np.log(data)))
 
 
-@numba.njit(parallel=True)
+@numba.njit(cache=True, inline="always", fastmath=False, boundscheck=False,
+            parallel=True)
 def __stat_min(data: np.ndarray) -> np.number:
     """
     Compute the minimum.
 
     :param data: the data
     :return: the minimum
     """
     return data.min()
 
 
-@numba.njit(parallel=True)
+@numba.njit(cache=True, inline="always", fastmath=False, boundscheck=False,
+            parallel=True)
 def __stat_max(data: np.ndarray) -> np.number:
     """
     Compute the maximum.
 
     :param data: the data
     :return: the maximum
     """
     return data.max()
 
 
-@numba.njit
+@numba.njit(cache=True, inline="always", fastmath=False, boundscheck=False,
+            parallel=True)
 def __stat_median(data: np.ndarray) -> np.ndarray:
     """
     Compute the median.
 
     :param data: the data
     :return: the median
     """
     return np.median(data)
 
 
-@numba.njit(parallel=True)
+@numba.njit(cache=True, inline="always", fastmath=False, boundscheck=False,
+            parallel=True)
 def __stat_sd(data: np.ndarray) -> np.number:
     """
     Compute the standard deviation.
 
     :param data: the data
     :return: the standard deviation
     """
     return data.std()
 
 
-@numba.njit(parallel=True)
+@numba.njit(cache=True, inline="always", fastmath=False, boundscheck=False,
+            parallel=True)
 def __stat_mean_minus_sd(data: np.ndarray) -> np.number:
     """
     Compute the arithmetic mean minus the standard deviation.
 
     :param data: the data
     :return: the arithmetic mean minus the standard deviation
     """
     return data.mean() - data.std()
 
 
-@numba.njit(parallel=True)
+@numba.njit(cache=True, inline="always", fastmath=False, boundscheck=False,
+            parallel=True)
 def __stat_mean_plus_sd(data: np.ndarray) -> np.number:
     """
     Compute the arithmetic mean plus the standard deviation.
 
     :param data: the data
     :return: the arithmetic mean plus the standard deviation
     """
     return data.mean() + data.std()
 
 
-@numba.njit
+@numba.njit(cache=True, inline="always", fastmath=False, boundscheck=False,
+            parallel=True)
 def __stat_quantile_10(data: np.ndarray) -> np.ndarray:
     """
     Compute the 10% quantile.
 
     :param data: the data
     :return: the 10% quantile
     """
     length: Final[int] = len(data)
     if (length > 10) and ((length % 10) == 1):
         data.sort()
         return data[(length - 1) // 10]
     return np.quantile(data, 0.1)
 
 
-@numba.njit
+@numba.njit(cache=True, inline="always", fastmath=False, boundscheck=False,
+            parallel=True)
 def __stat_quantile_90(data: np.ndarray) -> np.ndarray:
     """
     Compute the 90% quantile.
 
     :param data: the data
     :return: the 90% quantile
     """
     length: Final[int] = len(data)
     if (length > 10) and ((length % 10) == 1):
         data.sort()
         return data[(9 * (length - 1)) // 10]
     return np.quantile(data, 0.9)
 
 
-@numba.njit
+@numba.njit(cache=True, inline="always", fastmath=False, boundscheck=False,
+            parallel=True)
 def __stat_quantile_159(data: np.ndarray) -> np.ndarray:
     """
     Compute the 15.9% quantile, which equals mean-sd in normal distributions.
 
     :param data: the data
     :return: the 15.9% quantile
     """
     return np.quantile(data, __Q159)
 
 
-@numba.njit
+@numba.njit(cache=True, inline="always", fastmath=False, boundscheck=False,
+            parallel=True)
 def __stat_quantile_841(data: np.ndarray) -> np.ndarray:
     """
     Compute the 84.1% quantile, which equals mean+sd in normal distributions.
 
     :param data: the data
     :return: the 84.1% quantile
     """
@@ -315,45 +327,52 @@
     STAT_Q10: __stat_quantile_10,
     STAT_Q90: __stat_quantile_90,
     STAT_Q159: __stat_quantile_159,
     STAT_Q841: __stat_quantile_841,
 }
 
 
-@dataclass(frozen=True, init=False, order=True)
+@dataclass(frozen=True, init=False, order=False, eq=False)
 class StatRun(MultiRun2DData):
     """A time-value statistic over a set of runs."""
 
     #: The name of this statistic.
     stat_name: str
     #: The time-dependent statistic.
     stat: np.ndarray
 
     def __init__(self,
                  algorithm: str | None,
                  instance: str | None,
+                 objective: str | None,
+                 encoding: str | None,
                  n: int,
                  time_unit: str,
                  f_name: str,
                  stat_name: str,
                  stat: np.ndarray):
         """
         Create the time-based statistics of an algorithm-setup combination.
 
         :param algorithm: the algorithm name, if all runs are
             with the same algorithm
         :param instance: the instance name, if all runs are
             on the same instance
+        :param objective: the objective name, if all runs are on the same
+            objective function, `None` otherwise
+        :param encoding: the encoding name, if all runs are on the same
+            encoding and an encoding was actually used, `None` otherwise
         :param n: the total number of runs
         :param time_unit: the time unit
         :param f_name: the objective dimension name
         :param stat_name: the name of the statistic
         :param stat: the statistic itself
         """
-        super().__init__(algorithm, instance, n, time_unit, f_name)
+        super().__init__(algorithm, instance, objective, encoding, n,
+                         time_unit, f_name)
 
         if not isinstance(stat_name, str):
             raise type_error(stat_name, "stat_name", str)
         object.__setattr__(self, "stat_name", stat_name)
         if not isinstance(stat, np.ndarray):
             raise type_error(stat, "statistic data", np.ndarray)
         stat.flags.writeable = False
@@ -385,33 +404,41 @@
         if not isinstance(statistics, Iterable):
             raise type_error(statistics, "statistics", Iterable)
         if not callable(consumer):
             raise type_error(consumer, "consumer", call=True)
 
         algorithm: str | None = None
         instance: str | None = None
+        objective: str | None = None
+        encoding: str | None = None
         time_unit: str | None = None
         f_name: str | None = None
         time: list[np.ndarray] = []
         f: list[np.ndarray] = []
         n: int = 0
 
         for progress in source:
             if not isinstance(progress, Progress):
                 raise type_error(progress, "stat run data source", Progress)
             if n <= 0:
                 algorithm = progress.algorithm
                 instance = progress.instance
+                objective = progress.objective
+                encoding = progress.encoding
                 time_unit = progress.time_unit
                 f_name = progress.f_name
             else:
                 if algorithm != progress.algorithm:
                     algorithm = None
                 if instance != progress.instance:
                     instance = None
+                if objective != progress.objective:
+                    objective = None
+                if encoding != progress.encoding:
+                    encoding = None
                 if time_unit != progress.time_unit:
                     raise ValueError(
                         f"Cannot mix time units {time_unit} "
                         f"and {progress.time_unit}.")
                 if f_name != progress.f_name:
                     raise ValueError(f"Cannot mix f-names {f_name} "
                                      f"and {progress.f_name}.")
@@ -434,59 +461,74 @@
 
         count = 0
         for name in statistics:
             if not isinstance(name, str):
                 raise type_error(name, "statistic name", str)
             if name not in _FUNC_MAP:
                 raise ValueError(f"Unknown statistic name {name!r}.")
-            consumer(StatRun(algorithm, instance, n, time_unit, f_name, name,
+            consumer(StatRun(algorithm, instance, objective, encoding, n,
+                             time_unit, f_name, name,
                              _apply_fun(x_unique, time, f, _FUNC_MAP[name])))
             count += 1
 
         if count <= 0:
             raise ValueError("No statistic names provided.")
 
     @staticmethod
     def from_progress(source: Iterable[Progress],
                       statistics: str | Iterable[str],
                       consumer: Callable[["StatRun"], Any],
                       join_all_algorithms: bool = False,
-                      join_all_instances: bool = False) -> None:
+                      join_all_instances: bool = False,
+                      join_all_objectives: bool = False,
+                      join_all_encodings: bool = False) -> None:
         """
         Aggregate statist runs over a stream of progress data.
 
         :param source: the stream of progress data
         :param statistics: the statistics that should be computed per group
         :param consumer: the destination to which the new stat runs will be
             passed, can be the `append` method of a :class:`list`
         :param join_all_algorithms: should the statistics be aggregated
             over all algorithms
         :param join_all_instances: should the statistics be aggregated
             over all algorithms
+        :param join_all_objectives: should the statistics be aggregated over
+            all objective functions?
+        :param join_all_encodings: should the statistics be aggregated over
+            all encodings?
         """
         if not isinstance(source, Iterable):
             raise type_error(source, "source", Iterable)
         if isinstance(statistics, str):
             statistics = [statistics]
         if not isinstance(statistics, Iterable):
             raise type_error(statistics, "statistics", Iterable)
         if not callable(consumer):
             raise type_error(consumer, "consumer", call=True)
         if not isinstance(join_all_algorithms, bool):
             raise type_error(join_all_algorithms, "join_all_algorithms", bool)
         if not isinstance(join_all_instances, bool):
             raise type_error(join_all_instances, "join_all_instances", bool)
+        if not isinstance(join_all_objectives, bool):
+            raise type_error(join_all_objectives, "join_all_objectives", bool)
+        if not isinstance(join_all_encodings, bool):
+            raise type_error(join_all_encodings, "join_all_encodings", bool)
 
-        sorter: dict[str, list[Progress]] = {}
+        sorter: dict[tuple[str, str, str, str, str, str], list[Progress]] = {}
         for prog in source:
             if not isinstance(prog, Progress):
                 raise type_error(prog, "progress source", Progress)
-            a: str = "" if join_all_algorithms else prog.algorithm
-            i: str = "" if join_all_instances else prog.instance
-            key: str = f"{a}/{i}/{prog.time_unit}/{prog.f_name}"
+            key = ("" if join_all_algorithms else prog.algorithm,
+                   "" if join_all_instances else prog.instance,
+                   "" if join_all_objectives else prog.objective,
+                   "" if join_all_encodings else (
+                       "" if prog.encoding is None else prog.encoding),
+                   prog.time_unit, prog.f_name)
+
             if key in sorter:
                 lst = sorter[key]
             else:
                 lst = []
                 sorter[key] = lst
             lst.append(prog)
```

### Comparing `moptipy-0.9.90/moptipy/evaluation/statistics.py` & `moptipy-0.9.91/moptipy/evaluation/statistics.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 """A simple and immutable basic statistics record."""
 
 import statistics
 from dataclasses import dataclass
-from math import gcd, inf, isfinite, sqrt
+from math import gcd, inf, isfinite, nextafter, sqrt
 from typing import Callable, Final, Iterable, cast
 
 from moptipy.utils.logger import CSV_SEPARATOR, SCOPE_SEPARATOR
 from moptipy.utils.math import (
     DBL_INT_LIMIT_P,
     try_int,
     try_int_div,
@@ -17,15 +17,14 @@
     str_to_intfloat,
     str_to_intfloatnone,
 )
 from moptipy.utils.types import check_int_range, type_error
 
 #: The limit until which we simplify geometric mean data.
 _INT_ROOT_LIMIT: Final[int] = int(sqrt(DBL_INT_LIMIT_P))
-_ULP: Final[float] = 1 - (2 ** (-53))
 
 #: The minimum value key.
 KEY_MINIMUM: Final[str] = "min"
 #: The median value key.
 KEY_MEDIAN: Final[str] = "med"
 #: The arithmetic mean value key.
 KEY_MEAN_ARITH: Final[str] = "mean"
@@ -50,15 +49,15 @@
     KEY_MEAN_ARITH: lambda s: s.mean_arith,
     KEY_MEAN_GEOM: lambda s: s.mean_geom,
     KEY_MAXIMUM: lambda s: s.maximum,
     KEY_STDDEV: lambda s: s.stddev,
 }
 
 
-@dataclass(frozen=True, init=False, order=True)
+@dataclass(frozen=True, init=False, order=True, eq=True)
 class Statistics:
     """An immutable record with statistics of one quantity."""
 
     #: The minimum.
     minimum: int | float
     #: The median.
     median: int | float
@@ -162,23 +161,25 @@
                 if mean_geom != minimum:
                     raise ValueError(f"mean_geom ({mean_geom}) must equal "
                                      f"minimum ({minimum}) if n=1.")
             else:
                 if mean_geom < minimum:
                     raise ValueError(
                         f"mean_geom ({mean_geom}) must be >= "
-                        f"minimum ({minimum}) if n>1.")
+                        f"minimum ({minimum}) if (n={n})>1.")
                 if mean_geom > mean_arith:
                     raise ValueError(
                         f"mean_geom ({mean_geom}) must be <= "
-                        f"mean_arith ({mean_arith}) if n>1.")
-                if (mean_geom >= mean_arith) and (minimum < maximum):
+                        f"mean_arith ({mean_arith}) if (n={n})>1.")
+                if ((mean_geom >= mean_arith) and (minimum < maximum)
+                        and (((maximum - minimum) / (max(  # precision
+                            abs(maximum), abs(minimum)))) > 0.01)):
                     raise ValueError(
                         f"mean_geom ({mean_geom}) must be < "
-                        f"mean_arith ({mean_arith}) if n>1 and "
+                        f"mean_arith ({mean_arith}) if (n={n})>1 and "
                         f"minimum ({minimum}) < maximum ({maximum}).")
 
         if not isinstance(stddev, int | float):
             raise type_error(stddev, "stddev", (int, float))
         if isinstance(stddev, float) and (not isfinite(stddev)):
             raise ValueError(f"stddev must be finite, but is {stddev}.")
 
@@ -313,38 +314,43 @@
 
                 var: int | float  # the container for the variance
                 var = try_int_div(int_sum_sqr - int_sum2, n - 1) \
                     if i_n == 1 else \
                     ((int_sum_sqr - (int_sum2 / i_n)) / (n - 1))
 
                 stddev = try_int(sqrt(var))
+                if (stddev == 0) and (minimum < maximum):
+                    stddev = statistics.stdev(source)
 
             if minimum > 0:  # geometric mean only defined for all-positive
                 if int_prod == 0:
                     mean_geom = 0  # geometric mean is 0 if product is 0
                 else:  # if not, geom_mean = prod ** (1/n)
                     mean_geom = try_int_root(int_prod, n, True)
-                    if mean_geom is None:
+                    if (mean_geom is None) or ((minimum < maximum) and (
+                            mean_geom >= mean_arith)):
                         mean_geom = statistics.geometric_mean(source)
         else:  # ok, we do not have only integer-like values
             mean_arith = try_int(statistics.mean(source))
             if minimum > 0:
                 mean_geom = try_int(statistics.geometric_mean(source))
             if n > 1:
                 stddev = try_int(statistics.stdev(source))
 
         if mean_geom is not None:
             # Deal with errors that may have arisen due to
             # numerical imprecision.
-            if (mean_geom < minimum) \
-                    and ((mean_geom / _ULP) >= (minimum * _ULP)):
+            if (mean_geom < minimum) and (nextafter(
+                    mean_geom, inf) >= nextafter(minimum, -inf)):
                 mean_geom = minimum
-            if (mean_geom > maximum) \
-                    and ((maximum / _ULP) >= (mean_geom * _ULP)):
-                mean_geom = maximum
+            upper_limit = mean_arith if (n > 1) else maximum
+            if (mean_geom > upper_limit) and ((nextafter(
+                    upper_limit, inf) >= nextafter(mean_geom, -inf)) or (
+                    (0.9999999999999 * mean_geom) <= upper_limit)):
+                mean_geom = upper_limit
 
         return Statistics(n=n,
                           minimum=minimum,
                           median=statistics.median(source),
                           mean_arith=mean_arith,
                           mean_geom=mean_geom,
                           maximum=maximum,
```

### Comparing `moptipy-0.9.90/moptipy/evaluation/styler.py` & `moptipy-0.9.91/moptipy/evaluation/styler.py`

 * *Files identical despite different names*

### Comparing `moptipy-0.9.90/moptipy/evaluation/tabulate_end_results.py` & `moptipy-0.9.91/moptipy/evaluation/tabulate_end_results.py`

 * *Files identical despite different names*

### Comparing `moptipy-0.9.90/moptipy/evaluation/tabulate_result_tests.py` & `moptipy-0.9.91/moptipy/evaluation/tabulate_result_tests.py`

 * *Files identical despite different names*

### Comparing `moptipy-0.9.90/moptipy/examples/bitstrings/__init__.py` & `moptipy-0.9.91/moptipy/examples/bitstrings/__init__.py`

 * *Files identical despite different names*

### Comparing `moptipy-0.9.90/moptipy/examples/bitstrings/bitstring_problem.py` & `moptipy-0.9.91/moptipy/examples/bitstrings/bitstring_problem.py`

 * *Files identical despite different names*

### Comparing `moptipy-0.9.90/moptipy/examples/bitstrings/ising1d.py` & `moptipy-0.9.91/moptipy/examples/bitstrings/ising1d.py`

 * *Files identical despite different names*

### Comparing `moptipy-0.9.90/moptipy/examples/bitstrings/jump.py` & `moptipy-0.9.91/moptipy/examples/bitstrings/jump.py`

 * *Files identical despite different names*

### Comparing `moptipy-0.9.90/moptipy/examples/bitstrings/leadingones.py` & `moptipy-0.9.91/moptipy/examples/bitstrings/leadingones.py`

 * *Files identical despite different names*

### Comparing `moptipy-0.9.90/moptipy/examples/bitstrings/onemax.py` & `moptipy-0.9.91/moptipy/examples/bitstrings/onemax.py`

 * *Files identical despite different names*

### Comparing `moptipy-0.9.90/moptipy/examples/bitstrings/trap.py` & `moptipy-0.9.91/moptipy/examples/bitstrings/trap.py`

 * *Files identical despite different names*

### Comparing `moptipy-0.9.90/moptipy/examples/bitstrings/w_model.py` & `moptipy-0.9.91/moptipy/examples/bitstrings/w_model.py`

 * *Files identical despite different names*

### Comparing `moptipy-0.9.90/moptipy/examples/bitstrings/zeromax.py` & `moptipy-0.9.91/moptipy/examples/bitstrings/zeromax.py`

 * *Files identical despite different names*

### Comparing `moptipy-0.9.90/moptipy/examples/jssp/__init__.py` & `moptipy-0.9.91/moptipy/examples/jssp/__init__.py`

 * *Files identical despite different names*

### Comparing `moptipy-0.9.90/moptipy/examples/jssp/demo_examples.py` & `moptipy-0.9.91/moptipy/examples/jssp/demo_examples.py`

 * *Files identical despite different names*

### Comparing `moptipy-0.9.90/moptipy/examples/jssp/evaluation.py` & `moptipy-0.9.91/moptipy/examples/jssp/evaluation.py`

 * *Files identical despite different names*

### Comparing `moptipy-0.9.90/moptipy/examples/jssp/experiment.py` & `moptipy-0.9.91/moptipy/examples/jssp/experiment.py`

 * *Files identical despite different names*

### Comparing `moptipy-0.9.90/moptipy/examples/jssp/gantt.py` & `moptipy-0.9.91/moptipy/examples/jssp/gantt.py`

 * *Files identical despite different names*

### Comparing `moptipy-0.9.90/moptipy/examples/jssp/gantt_space.py` & `moptipy-0.9.91/moptipy/examples/jssp/gantt_space.py`

 * *Files identical despite different names*

### Comparing `moptipy-0.9.90/moptipy/examples/jssp/instance.py` & `moptipy-0.9.91/moptipy/examples/jssp/instance.py`

 * *Files identical despite different names*

### Comparing `moptipy-0.9.90/moptipy/examples/jssp/instance_selector.py` & `moptipy-0.9.91/moptipy/examples/jssp/instance_selector.py`

 * *Files identical despite different names*

### Comparing `moptipy-0.9.90/moptipy/examples/jssp/instances.txt` & `moptipy-0.9.91/moptipy/examples/jssp/instances.txt`

 * *Files identical despite different names*

### Comparing `moptipy-0.9.90/moptipy/examples/jssp/makespan.py` & `moptipy-0.9.91/moptipy/examples/jssp/makespan.py`

 * *Files identical despite different names*

### Comparing `moptipy-0.9.90/moptipy/examples/jssp/ob_encoding.py` & `moptipy-0.9.91/moptipy/examples/jssp/ob_encoding.py`

 * *Files identical despite different names*

### Comparing `moptipy-0.9.90/moptipy/examples/jssp/plot_gantt_chart.py` & `moptipy-0.9.91/moptipy/examples/jssp/plot_gantt_chart.py`

 * *Files identical despite different names*

### Comparing `moptipy-0.9.90/moptipy/examples/jssp/plots.py` & `moptipy-0.9.91/moptipy/examples/jssp/plots.py`

 * *Files identical despite different names*

### Comparing `moptipy-0.9.90/moptipy/examples/jssp/spaces_sizes.py` & `moptipy-0.9.91/moptipy/examples/jssp/spaces_sizes.py`

 * *Files identical despite different names*

### Comparing `moptipy-0.9.90/moptipy/examples/jssp/worktime.py` & `moptipy-0.9.91/moptipy/examples/jssp/worktime.py`

 * *Files identical despite different names*

### Comparing `moptipy-0.9.90/moptipy/examples/vectors/ackley.py` & `moptipy-0.9.91/moptipy/examples/vectors/ackley.py`

 * *Files identical despite different names*

### Comparing `moptipy-0.9.90/moptipy/examples/vectors/sphere.py` & `moptipy-0.9.91/moptipy/examples/vectors/sphere.py`

 * *Files identical despite different names*

### Comparing `moptipy-0.9.90/moptipy/mo/archive/keep_farthest.py` & `moptipy-0.9.91/moptipy/mo/archive/keep_farthest.py`

 * *Files identical despite different names*

### Comparing `moptipy-0.9.90/moptipy/mo/problem/basic_mo_problem.py` & `moptipy-0.9.91/moptipy/mo/problem/basic_mo_problem.py`

 * *Files identical despite different names*

### Comparing `moptipy-0.9.90/moptipy/mo/problem/weighted_sum.py` & `moptipy-0.9.91/moptipy/mo/problem/weighted_sum.py`

 * *Files identical despite different names*

### Comparing `moptipy-0.9.90/moptipy/mock/components.py` & `moptipy-0.9.91/moptipy/mock/components.py`

 * *Files 1% similar despite different names*

```diff
@@ -426,15 +426,15 @@
         not_allowed: Final[set[str | float]] = \
             _make_not_allowed(forbidden)
         names: list[str] = []
         strengths: list[float] = []
         jitters: list[float] = []
         complexities: list[float] = []
 
-        prefixes: Final[tuple[str, ...]] = ("aco", "bobyqa", "cma-es", "de",
+        prefixes: Final[tuple[str, ...]] = ("aco", "bobyqa", "cmaes", "de",
                                             "ea", "eda", "ga", "gp", "hc",
                                             "ma", "pso", "rs", "rw", "sa",
                                             "umda")
         suffixes: Final[tuple[str, ...]] = ("1swap", "2swap", "µ")
 
         max_name_len: int = int(max(2, ceil(n / 6)))
         trials: int = 0
@@ -544,23 +544,23 @@
         return tuple(result)
 
 
 @dataclass(frozen=True, init=False, order=True)
 class BasePerformance:
     """An algorithm applied to a problem instance description record."""
 
-    #: The algorithm.
+    #: the algorithm.
     algorithm: Algorithm
-    #: The problem instance
+    #: the problem instance
     instance: Instance
-    #: The base performance, in (0, 1), larger values are worst
+    #: the base performance, in (0, 1), larger values are worst
     performance: float
-    #: The performance jitter, in (0, 1), larger values are worst
+    #: the performance jitter, in (0, 1), larger values are worst
     jitter: float
-    #: The time per FE, in (0, 1), larger values are worst
+    #: the time per FE, in (0, 1), larger values are worst
     speed: float
 
     def __init__(self,
                  algorithm: Algorithm,
                  instance: Instance,
                  performance: float,
                  jitter: float,
```

### Comparing `moptipy-0.9.90/moptipy/mock/end_results.py` & `moptipy-0.9.91/moptipy/mock/end_results.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 """Compute the end result of one mock run."""
 
 from dataclasses import dataclass
-from math import ceil, inf
+from math import ceil
 from typing import Final
 
 from numpy.random import Generator
 
 from moptipy.evaluation.end_results import EndResult
 from moptipy.mock.components import (
     Algorithm,
@@ -29,60 +29,60 @@
     :param max_fes: the maximum number of FEs
     :param max_time_millis: the maximum time
     :returns: the end result record
     """
     if not isinstance(performance, BasePerformance):
         raise type_error(performance, "performance", BasePerformance)
 
-    limit_time: int | float = inf
-    limit_fes: int | float = inf
+    limit_time: int = 1_000_000_000_000
+    limit_fes: int = 1_000_000_000_000
     if max_time_millis is not None:
         limit_time = check_int_range(
-            max_time_millis, "max_time_millis", 11, 1_000_000_000_000_000)
+            max_time_millis, "max_time_millis", 11, 1_000_000_000_000)
     if max_fes is not None:
         limit_fes = check_int_range(
-            max_fes, "max_fes", 11, 1_000_000_000_000_000)
+            max_fes, "max_fes", 11, 1_000_000_000_000)
 
     # The random number generator is determined by the seed.
     random: Final[Generator] = rand_generator(seed)
 
     # The speed also has some slight jitter.
     jitter: Final[float] = performance.jitter
     speed: float = -1
     while (speed <= 0) or (speed >= 1):
         speed = random.normal(loc=performance.speed, scale=0.01 * jitter)
 
     # total_time ~ total_fes * (performance.speed ** 3)
     total_time: int
     total_fes: int
     trials: int
-    if max_time_millis:
+    if max_time_millis is not None:
         total_time = int(max_time_millis + abs(random.normal(
             loc=0, scale=5 * jitter)))
         total_fes = -1
         trials = 0
         while ((total_fes <= 100) or (total_fes > limit_fes)) \
                 and (trials < 10000):
             trials += 1
             total_fes = int(random.normal(
                 loc=max(10.0, total_time / (speed ** 3)),
                 scale=max(100.0, 200.0 / speed)))
         if trials >= 10000:
             total_fes = int(min(limit_fes, 10000.0))
     else:
-        total_fes = max_fes if max_fes else 1_000_000
+        total_fes = max_fes if max_fes is not None else 1_000_000
         total_time = -1
         trials = 0
         while ((total_time <= 10) or (total_time > limit_time)) \
                 and (trials < 10000):
             total_time = int(random.normal(
                 loc=max(10.0, total_fes * (speed ** 3)),
                 scale=max(10.0, 100.0 / speed)))
         if trials >= 10000:
-            total_time = int(min(limit_time, 10000.0))
+            total_time = int(min(limit_time, 10000))
 
     # We now look for the vicinity of the local optimum that will be found.
     # We use the quality to determine which attractor to use.
     # Then we will sample a solution between the next lower and next higher
     # attractor, again using the jitter and quality.
 
     # First, add some jitter to the quality.
@@ -92,15 +92,20 @@
 
     # Second, find the right attractor and remember it in base.
     att: Final[tuple[int, ...]] = performance.instance.attractors
     attn: Final[int] = len(att)
     att_index: int = -1
     best: Final[int] = performance.instance.best
     worst: Final[int] = performance.instance.worst
+    att_trials: int = 1000
     while (att_index < 0) or (att_index >= (attn - 1)):
+        att_trials -= 1
+        if att_trials <= 0:
+            att_index = attn // 2
+            break
         att_index = int(random.normal(loc=attn * (qual ** 1.7),
                                       scale=jitter ** 0.9))
     base: Final[int] = att[att_index]
 
     # Third, choose the ends of the intervals in which we can jitter.
     jit_end: int = min(int(base + 0.6 * (att[att_index + 1] - base)), worst)
     jit_start: int = base
@@ -134,14 +139,15 @@
             or (last_improvement_time >= total_time):
         last_improvement_time = int(random.normal(
             loc=total_time * fact, scale=total_time * 0.05 * jitter))
 
     res: Final[EndResult] = EndResult(
         algorithm=performance.algorithm.name,
         instance=performance.instance.name,
+        objective="f", encoding="e",
         rand_seed=seed,
         best_f=best_f,
         last_improvement_fe=last_improvement_fe,
         last_improvement_time_millis=last_improvement_time,
         total_fes=total_fes,
         total_time_millis=total_time,
         goal_f=performance.instance.best,
```

### Comparing `moptipy-0.9.90/moptipy/mock/mo_problem.py` & `moptipy-0.9.91/moptipy/mock/mo_problem.py`

 * *Files identical despite different names*

### Comparing `moptipy-0.9.90/moptipy/mock/objective.py` & `moptipy-0.9.91/moptipy/mock/objective.py`

 * *Files identical despite different names*

### Comparing `moptipy-0.9.90/moptipy/mock/utils.py` & `moptipy-0.9.91/moptipy/mock/utils.py`

 * *Files identical despite different names*

### Comparing `moptipy-0.9.90/moptipy/operators/__init__.py` & `moptipy-0.9.91/moptipy/operators/__init__.py`

 * *Files identical despite different names*

### Comparing `moptipy-0.9.90/moptipy/operators/bitstrings/__init__.py` & `moptipy-0.9.91/moptipy/operators/bitstrings/__init__.py`

 * *Files identical despite different names*

### Comparing `moptipy-0.9.90/moptipy/operators/bitstrings/op0_random.py` & `moptipy-0.9.91/moptipy/operators/bitstrings/op0_random.py`

 * *Files identical despite different names*

### Comparing `moptipy-0.9.90/moptipy/operators/bitstrings/op1_flip1.py` & `moptipy-0.9.91/moptipy/operators/bitstrings/op1_flip1.py`

 * *Files identical despite different names*

### Comparing `moptipy-0.9.90/moptipy/operators/bitstrings/op1_flip_m.py` & `moptipy-0.9.91/moptipy/operators/bitstrings/op1_flip_m.py`

 * *Files identical despite different names*

### Comparing `moptipy-0.9.90/moptipy/operators/bitstrings/op1_m_over_n_flip.py` & `moptipy-0.9.91/moptipy/operators/bitstrings/op1_m_over_n_flip.py`

 * *Files identical despite different names*

### Comparing `moptipy-0.9.90/moptipy/operators/bitstrings/op2_uniform.py` & `moptipy-0.9.91/moptipy/operators/bitstrings/op2_uniform.py`

 * *Files identical despite different names*

### Comparing `moptipy-0.9.90/moptipy/operators/op0_forward.py` & `moptipy-0.9.91/moptipy/operators/op0_forward.py`

 * *Files identical despite different names*

### Comparing `moptipy-0.9.90/moptipy/operators/ordered_choices/op0_choose_and_shuffle.py` & `moptipy-0.9.91/moptipy/operators/ordered_choices/op0_choose_and_shuffle.py`

 * *Files identical despite different names*

### Comparing `moptipy-0.9.90/moptipy/operators/permutations/__init__.py` & `moptipy-0.9.91/moptipy/operators/permutations/__init__.py`

 * *Files identical despite different names*

### Comparing `moptipy-0.9.90/moptipy/operators/permutations/op0_shuffle.py` & `moptipy-0.9.91/moptipy/operators/permutations/op0_shuffle.py`

 * *Files identical despite different names*

### Comparing `moptipy-0.9.90/moptipy/operators/permutations/op1_insert1.py` & `moptipy-0.9.91/moptipy/operators/permutations/op1_insert1.py`

 * *Files identical despite different names*

### Comparing `moptipy-0.9.90/moptipy/operators/permutations/op1_swap2.py` & `moptipy-0.9.91/moptipy/operators/permutations/op1_swap2.py`

 * *Files identical despite different names*

### Comparing `moptipy-0.9.90/moptipy/operators/permutations/op1_swap_exactly_n.py` & `moptipy-0.9.91/moptipy/operators/permutations/op1_swap_exactly_n.py`

 * *Files identical despite different names*

### Comparing `moptipy-0.9.90/moptipy/operators/permutations/op1_swap_try_n.py` & `moptipy-0.9.91/moptipy/operators/permutations/op1_swap_try_n.py`

 * *Files identical despite different names*

### Comparing `moptipy-0.9.90/moptipy/operators/permutations/op1_swapn.py` & `moptipy-0.9.91/moptipy/operators/permutations/op1_swapn.py`

 * *Files identical despite different names*

### Comparing `moptipy-0.9.90/moptipy/operators/permutations/op2_gap.py` & `moptipy-0.9.91/moptipy/operators/permutations/op2_gap.py`

 * *Files identical despite different names*

### Comparing `moptipy-0.9.90/moptipy/operators/permutations/op2_ox2.py` & `moptipy-0.9.91/moptipy/operators/permutations/op2_ox2.py`

 * *Files identical despite different names*

### Comparing `moptipy-0.9.90/moptipy/operators/signed_permutations/__init__.py` & `moptipy-0.9.91/moptipy/operators/signed_permutations/__init__.py`

 * *Files identical despite different names*

### Comparing `moptipy-0.9.90/moptipy/operators/signed_permutations/op0_shuffle_and_flip.py` & `moptipy-0.9.91/moptipy/operators/signed_permutations/op0_shuffle_and_flip.py`

 * *Files identical despite different names*

### Comparing `moptipy-0.9.90/moptipy/operators/signed_permutations/op1_swap_2_or_flip.py` & `moptipy-0.9.91/moptipy/operators/signed_permutations/op1_swap_2_or_flip.py`

 * *Files identical despite different names*

### Comparing `moptipy-0.9.90/moptipy/operators/tools.py` & `moptipy-0.9.91/moptipy/operators/tools.py`

 * *Files identical despite different names*

### Comparing `moptipy-0.9.90/moptipy/operators/vectors/op0_uniform.py` & `moptipy-0.9.91/moptipy/operators/vectors/op0_uniform.py`

 * *Files identical despite different names*

### Comparing `moptipy-0.9.90/moptipy/spaces/__init__.py` & `moptipy-0.9.91/moptipy/spaces/__init__.py`

 * *Files identical despite different names*

### Comparing `moptipy-0.9.90/moptipy/spaces/bitstrings.py` & `moptipy-0.9.91/moptipy/spaces/bitstrings.py`

 * *Files identical despite different names*

### Comparing `moptipy-0.9.90/moptipy/spaces/intspace.py` & `moptipy-0.9.91/moptipy/spaces/intspace.py`

 * *Files identical despite different names*

### Comparing `moptipy-0.9.90/moptipy/spaces/nparrayspace.py` & `moptipy-0.9.91/moptipy/spaces/nparrayspace.py`

 * *Files identical despite different names*

### Comparing `moptipy-0.9.90/moptipy/spaces/ordered_choices.py` & `moptipy-0.9.91/moptipy/spaces/ordered_choices.py`

 * *Files identical despite different names*

### Comparing `moptipy-0.9.90/moptipy/spaces/permutations.py` & `moptipy-0.9.91/moptipy/spaces/permutations.py`

 * *Files identical despite different names*

### Comparing `moptipy-0.9.90/moptipy/spaces/signed_permutations.py` & `moptipy-0.9.91/moptipy/spaces/signed_permutations.py`

 * *Files identical despite different names*

### Comparing `moptipy-0.9.90/moptipy/spaces/vectorspace.py` & `moptipy-0.9.91/moptipy/spaces/vectorspace.py`

 * *Files identical despite different names*

### Comparing `moptipy-0.9.90/moptipy/tests/algorithm.py` & `moptipy-0.9.91/moptipy/tests/algorithm.py`

 * *Files identical despite different names*

### Comparing `moptipy-0.9.90/moptipy/tests/component.py` & `moptipy-0.9.91/moptipy/tests/component.py`

 * *Files identical despite different names*

### Comparing `moptipy-0.9.90/moptipy/tests/encoding.py` & `moptipy-0.9.91/moptipy/tests/encoding.py`

 * *Files identical despite different names*

### Comparing `moptipy-0.9.90/moptipy/tests/fitness.py` & `moptipy-0.9.91/moptipy/tests/fitness.py`

 * *Files identical despite different names*

### Comparing `moptipy-0.9.90/moptipy/tests/mo_algorithm.py` & `moptipy-0.9.91/moptipy/tests/mo_algorithm.py`

 * *Files identical despite different names*

### Comparing `moptipy-0.9.90/moptipy/tests/mo_archive_pruner.py` & `moptipy-0.9.91/moptipy/tests/mo_archive_pruner.py`

 * *Files identical despite different names*

### Comparing `moptipy-0.9.90/moptipy/tests/mo_problem.py` & `moptipy-0.9.91/moptipy/tests/mo_problem.py`

 * *Files identical despite different names*

### Comparing `moptipy-0.9.90/moptipy/tests/objective.py` & `moptipy-0.9.91/moptipy/tests/objective.py`

 * *Files identical despite different names*

### Comparing `moptipy-0.9.90/moptipy/tests/on_bitstrings.py` & `moptipy-0.9.91/moptipy/tests/on_bitstrings.py`

 * *Files identical despite different names*

### Comparing `moptipy-0.9.90/moptipy/tests/on_ordered_choices.py` & `moptipy-0.9.91/moptipy/tests/on_ordered_choices.py`

 * *Files identical despite different names*

### Comparing `moptipy-0.9.90/moptipy/tests/on_permutations.py` & `moptipy-0.9.91/moptipy/tests/on_permutations.py`

 * *Files identical despite different names*

### Comparing `moptipy-0.9.90/moptipy/tests/on_signed_permutations.py` & `moptipy-0.9.91/moptipy/tests/on_signed_permutations.py`

 * *Files identical despite different names*

### Comparing `moptipy-0.9.90/moptipy/tests/on_vectors.py` & `moptipy-0.9.91/moptipy/tests/on_vectors.py`

 * *Files identical despite different names*

### Comparing `moptipy-0.9.90/moptipy/tests/op0.py` & `moptipy-0.9.91/moptipy/tests/op0.py`

 * *Files identical despite different names*

### Comparing `moptipy-0.9.90/moptipy/tests/op1.py` & `moptipy-0.9.91/moptipy/tests/op1.py`

 * *Files identical despite different names*

### Comparing `moptipy-0.9.90/moptipy/tests/op1_with_step_size.py` & `moptipy-0.9.91/moptipy/tests/op1_with_step_size.py`

 * *Files identical despite different names*

### Comparing `moptipy-0.9.90/moptipy/tests/op2.py` & `moptipy-0.9.91/moptipy/tests/op2.py`

 * *Files identical despite different names*

### Comparing `moptipy-0.9.90/moptipy/tests/selection.py` & `moptipy-0.9.91/moptipy/tests/selection.py`

 * *Files identical despite different names*

### Comparing `moptipy-0.9.90/moptipy/tests/space.py` & `moptipy-0.9.91/moptipy/tests/space.py`

 * *Files identical despite different names*

### Comparing `moptipy-0.9.90/moptipy/utils/cache.py` & `moptipy-0.9.91/moptipy/utils/cache.py`

 * *Files identical despite different names*

### Comparing `moptipy-0.9.90/moptipy/utils/console.py` & `moptipy-0.9.91/moptipy/utils/console.py`

 * *Files identical despite different names*

### Comparing `moptipy-0.9.90/moptipy/utils/formatted_string.py` & `moptipy-0.9.91/moptipy/utils/formatted_string.py`

 * *Files identical despite different names*

### Comparing `moptipy-0.9.90/moptipy/utils/help.py` & `moptipy-0.9.91/moptipy/utils/help.py`

 * *Files identical despite different names*

### Comparing `moptipy-0.9.90/moptipy/utils/html.py` & `moptipy-0.9.91/moptipy/utils/html.py`

 * *Files identical despite different names*

### Comparing `moptipy-0.9.90/moptipy/utils/lang.py` & `moptipy-0.9.91/moptipy/utils/lang.py`

 * *Files identical despite different names*

### Comparing `moptipy-0.9.90/moptipy/utils/latex.py` & `moptipy-0.9.91/moptipy/utils/latex.py`

 * *Files identical despite different names*

### Comparing `moptipy-0.9.90/moptipy/utils/logger.py` & `moptipy-0.9.91/moptipy/utils/logger.py`

 * *Files 0% similar despite different names*

```diff
@@ -108,15 +108,15 @@
 
     def _error(self, message: str) -> None:
         """
         Raise a :class:`ValueError` with context information.
 
         :param message: the message elements to merge
         :raises ValueError: an error with the message and some context
-        information
+            information
         """
         raise ValueError(f"{message} in logger {self.__log_name!r}."
                          if self.__section is None else
                          f"{message} in section {self.__section!r} "
                          f"of logger {self.__log_name!r}.")
 
     def __exit__(self, exception_type, exception_value, traceback) -> None:
```

### Comparing `moptipy-0.9.90/moptipy/utils/markdown.py` & `moptipy-0.9.91/moptipy/utils/markdown.py`

 * *Files identical despite different names*

### Comparing `moptipy-0.9.90/moptipy/utils/math.py` & `moptipy-0.9.91/moptipy/utils/math.py`

 * *Files identical despite different names*

### Comparing `moptipy-0.9.90/moptipy/utils/nputils.py` & `moptipy-0.9.91/moptipy/utils/nputils.py`

 * *Files identical despite different names*

### Comparing `moptipy-0.9.90/moptipy/utils/number_renderer.py` & `moptipy-0.9.91/moptipy/utils/number_renderer.py`

 * *Files identical despite different names*

### Comparing `moptipy-0.9.90/moptipy/utils/path.py` & `moptipy-0.9.91/moptipy/utils/path.py`

 * *Files identical despite different names*

### Comparing `moptipy-0.9.90/moptipy/utils/plot_defaults.py` & `moptipy-0.9.91/moptipy/utils/plot_defaults.py`

 * *Files identical despite different names*

### Comparing `moptipy-0.9.90/moptipy/utils/plot_utils.py` & `moptipy-0.9.91/moptipy/utils/plot_utils.py`

 * *Files identical despite different names*

### Comparing `moptipy-0.9.90/moptipy/utils/strings.py` & `moptipy-0.9.91/moptipy/utils/strings.py`

 * *Files identical despite different names*

### Comparing `moptipy-0.9.90/moptipy/utils/sys_info.py` & `moptipy-0.9.91/moptipy/utils/sys_info.py`

 * *Files identical despite different names*

### Comparing `moptipy-0.9.90/moptipy/utils/table.py` & `moptipy-0.9.91/moptipy/utils/table.py`

 * *Files identical despite different names*

### Comparing `moptipy-0.9.90/moptipy/utils/temp.py` & `moptipy-0.9.91/moptipy/utils/temp.py`

 * *Files identical despite different names*

### Comparing `moptipy-0.9.90/moptipy/utils/text_format.py` & `moptipy-0.9.91/moptipy/utils/text_format.py`

 * *Files identical despite different names*

### Comparing `moptipy-0.9.90/moptipy/utils/types.py` & `moptipy-0.9.91/moptipy/utils/types.py`

 * *Files identical despite different names*

### Comparing `moptipy-0.9.90/moptipy.egg-info/PKG-INFO` & `moptipy-0.9.91/moptipy.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 00000000: 4d65 7461 6461 7461 2d56 6572 7369 6f6e  Metadata-Version
 00000010: 3a20 322e 310a 4e61 6d65 3a20 6d6f 7074  : 2.1.Name: mopt
 00000020: 6970 790a 5665 7273 696f 6e3a 2030 2e39  ipy.Version: 0.9
-00000030: 2e39 300a 5375 6d6d 6172 793a 2041 2070  .90.Summary: A p
+00000030: 2e39 310a 5375 6d6d 6172 793a 2041 2070  .91.Summary: A p
 00000040: 6163 6b61 6765 2066 6f72 206d 6574 6168  ackage for metah
 00000050: 6575 7269 7374 6963 206f 7074 696d 697a  euristic optimiz
 00000060: 6174 696f 6e20 696e 2050 7974 686f 6e2e  ation in Python.
 00000070: 0a48 6f6d 652d 7061 6765 3a20 6874 7470  .Home-page: http
 00000080: 733a 2f2f 7468 6f6d 6173 7765 6973 652e  s://thomasweise.
 00000090: 6769 7468 7562 2e69 6f2f 6d6f 7074 6970  github.io/moptip
 000000a0: 790a 4175 7468 6f72 3a20 5468 6f6d 6173  y.Author: Thomas
```

### Comparing `moptipy-0.9.90/moptipy.egg-info/SOURCES.txt` & `moptipy-0.9.91/moptipy.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `moptipy-0.9.90/setup.cfg` & `moptipy-0.9.91/setup.cfg`

 * *Files identical despite different names*

### Comparing `moptipy-0.9.90/setup.py` & `moptipy-0.9.91/setup.py`

 * *Files identical despite different names*

### Comparing `moptipy-0.9.90/tests/test_examples_from_readme_md.py` & `moptipy-0.9.91/tests/test_examples_from_readme_md.py`

 * *Files identical despite different names*

### Comparing `moptipy-0.9.90/tests/test_examples_in_examples_directory.py` & `moptipy-0.9.91/tests/test_examples_in_examples_directory.py`

 * *Files identical despite different names*

### Comparing `moptipy-0.9.90/tests/test_links_in_documentation.py` & `moptipy-0.9.91/tests/test_links_in_documentation.py`

 * *Files identical despite different names*

