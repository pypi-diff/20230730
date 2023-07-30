# Comparing `tmp/teneva_bm-0.5.0.tar.gz` & `tmp/teneva_bm-0.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "teneva_bm-0.5.0.tar", last modified: Thu Jul 27 18:27:58 2023, max compression
+gzip compressed data, was "teneva_bm-0.6.0.tar", last modified: Sun Jul 30 18:22:58 2023, max compression
```

## Comparing `teneva_bm-0.5.0.tar` & `teneva_bm-0.6.0.tar`

### file list

```diff
@@ -1,76 +1,79 @@
-drwxr-xr-x   0 andrei     (501) staff       (20)        0 2023-07-27 18:27:58.821829 teneva_bm-0.5.0/
--rw-r--r--   0 andrei     (501) staff       (20)     1090 2023-02-25 19:29:59.000000 teneva_bm-0.5.0/LICENSE.txt
--rw-r--r--   0 andrei     (501) staff       (20)       79 2023-07-27 07:17:23.000000 teneva_bm-0.5.0/MANIFEST.in
--rw-r--r--   0 andrei     (501) staff       (20)    18567 2023-07-27 18:27:58.822271 teneva_bm-0.5.0/PKG-INFO
--rw-r--r--   0 andrei     (501) staff       (20)    17306 2023-07-27 18:27:03.000000 teneva_bm-0.5.0/README.md
--rw-r--r--   0 andrei     (501) staff       (20)      899 2023-07-27 07:20:23.000000 teneva_bm-0.5.0/demo.py
--rw-r--r--   0 andrei     (501) staff       (20)       33 2023-06-19 10:36:15.000000 teneva_bm-0.5.0/requirements.txt
--rw-r--r--   0 andrei     (501) staff       (20)      107 2023-07-27 18:27:58.823494 teneva_bm-0.5.0/setup.cfg
--rw-r--r--   0 andrei     (501) staff       (20)     2518 2023-07-16 14:04:06.000000 teneva_bm-0.5.0/setup.py
-drwxr-xr-x   0 andrei     (501) staff       (20)        0 2023-07-27 18:27:58.784493 teneva_bm-0.5.0/teneva_bm/
--rw-r--r--   0 andrei     (501) staff       (20)      208 2023-07-27 18:26:56.000000 teneva_bm-0.5.0/teneva_bm/__init__.py
-drwxr-xr-x   0 andrei     (501) staff       (20)        0 2023-07-27 18:27:58.792385 teneva_bm-0.5.0/teneva_bm/agent/
--rw-r--r--   0 andrei     (501) staff       (20)      168 2023-07-27 13:43:14.000000 teneva_bm-0.5.0/teneva_bm/agent/__init__.py
--rw-r--r--   0 andrei     (501) staff       (20)     5812 2023-07-27 15:14:05.000000 teneva_bm-0.5.0/teneva_bm/agent/agent.py
--rw-r--r--   0 andrei     (501) staff       (20)     1818 2023-07-27 18:00:55.000000 teneva_bm-0.5.0/teneva_bm/agent/bm_agent_ant.py
--rw-r--r--   0 andrei     (501) staff       (20)     1868 2023-07-27 18:01:50.000000 teneva_bm-0.5.0/teneva_bm/agent/bm_agent_humanoid.py
--rw-r--r--   0 andrei     (501) staff       (20)     6836 2023-07-27 15:13:48.000000 teneva_bm-0.5.0/teneva_bm/agent/bm_agent_lake.py
--rw-r--r--   0 andrei     (501) staff       (20)     1831 2023-07-27 15:13:53.000000 teneva_bm-0.5.0/teneva_bm/agent/bm_agent_swimmer.py
--rw-r--r--   0 andrei     (501) staff       (20)     2113 2023-07-27 13:10:46.000000 teneva_bm-0.5.0/teneva_bm/agent/policy.py
--rw-r--r--   0 andrei     (501) staff       (20)    31229 2023-07-27 15:44:59.000000 teneva_bm-0.5.0/teneva_bm/bm.py
-drwxr-xr-x   0 andrei     (501) staff       (20)        0 2023-07-27 18:27:58.798770 teneva_bm-0.5.0/teneva_bm/func/
--rw-r--r--   0 andrei     (501) staff       (20)      516 2023-07-13 07:42:30.000000 teneva_bm-0.5.0/teneva_bm/func/__init__.py
--rw-r--r--   0 andrei     (501) staff       (20)     3606 2023-07-27 10:01:49.000000 teneva_bm-0.5.0/teneva_bm/func/bm_func_ackley.py
--rw-r--r--   0 andrei     (501) staff       (20)     2487 2023-07-27 10:01:53.000000 teneva_bm-0.5.0/teneva_bm/func/bm_func_alpine.py
--rw-r--r--   0 andrei     (501) staff       (20)     2526 2023-07-27 10:01:57.000000 teneva_bm-0.5.0/teneva_bm/func/bm_func_dixon.py
--rw-r--r--   0 andrei     (501) staff       (20)     2481 2023-07-27 10:02:00.000000 teneva_bm-0.5.0/teneva_bm/func/bm_func_exp.py
--rw-r--r--   0 andrei     (501) staff       (20)     2928 2023-07-27 10:02:04.000000 teneva_bm-0.5.0/teneva_bm/func/bm_func_griewank.py
--rw-r--r--   0 andrei     (501) staff       (20)     3519 2023-07-27 10:02:08.000000 teneva_bm-0.5.0/teneva_bm/func/bm_func_michalewicz.py
--rw-r--r--   0 andrei     (501) staff       (20)     2493 2023-07-27 10:02:11.000000 teneva_bm-0.5.0/teneva_bm/func/bm_func_piston.py
--rw-r--r--   0 andrei     (501) staff       (20)     2669 2023-07-27 10:02:15.000000 teneva_bm-0.5.0/teneva_bm/func/bm_func_qing.py
--rw-r--r--   0 andrei     (501) staff       (20)     3277 2023-07-27 10:02:21.000000 teneva_bm-0.5.0/teneva_bm/func/bm_func_rastrigin.py
--rw-r--r--   0 andrei     (501) staff       (20)     3334 2023-07-27 10:02:24.000000 teneva_bm-0.5.0/teneva_bm/func/bm_func_rosenbrock.py
--rw-r--r--   0 andrei     (501) staff       (20)     2187 2023-07-27 10:02:28.000000 teneva_bm-0.5.0/teneva_bm/func/bm_func_schaffer.py
--rw-r--r--   0 andrei     (501) staff       (20)     3335 2023-07-27 10:02:33.000000 teneva_bm-0.5.0/teneva_bm/func/bm_func_schwefel.py
-drwxr-xr-x   0 andrei     (501) staff       (20)        0 2023-07-27 18:27:58.800286 teneva_bm-0.5.0/teneva_bm/hs/
--rw-r--r--   0 andrei     (501) staff       (20)       78 2023-07-17 21:02:17.000000 teneva_bm-0.5.0/teneva_bm/hs/__init__.py
--rw-r--r--   0 andrei     (501) staff       (20)     1622 2023-07-27 10:24:15.000000 teneva_bm-0.5.0/teneva_bm/hs/bm_hs_func001.py
--rw-r--r--   0 andrei     (501) staff       (20)     2147 2023-07-27 10:24:20.000000 teneva_bm-0.5.0/teneva_bm/hs/bm_hs_func006.py
-drwxr-xr-x   0 andrei     (501) staff       (20)        0 2023-07-27 18:27:58.806077 teneva_bm-0.5.0/teneva_bm/hs/draft_constrained_functions/
--rw-r--r--   0 andrei     (501) staff       (20)      209 2023-07-17 20:25:36.000000 teneva_bm-0.5.0/teneva_bm/hs/draft_constrained_functions/__init__.py
--rw-r--r--   0 andrei     (501) staff       (20)     2272 2023-07-17 20:25:36.000000 teneva_bm-0.5.0/teneva_bm/hs/draft_constrained_functions/bm_hs007.py
--rw-r--r--   0 andrei     (501) staff       (20)     2459 2023-07-17 20:25:36.000000 teneva_bm-0.5.0/teneva_bm/hs/draft_constrained_functions/bm_hs008.py
--rw-r--r--   0 andrei     (501) staff       (20)     2318 2023-07-17 20:25:36.000000 teneva_bm-0.5.0/teneva_bm/hs/draft_constrained_functions/bm_hs009.py
--rw-r--r--   0 andrei     (501) staff       (20)     2266 2023-07-17 20:25:36.000000 teneva_bm-0.5.0/teneva_bm/hs/draft_constrained_functions/bm_hs010.py
--rw-r--r--   0 andrei     (501) staff       (20)     2251 2023-07-17 20:25:36.000000 teneva_bm-0.5.0/teneva_bm/hs/draft_constrained_functions/bm_hs011.py
--rw-r--r--   0 andrei     (501) staff       (20)     2376 2023-07-17 20:25:36.000000 teneva_bm-0.5.0/teneva_bm/hs/draft_constrained_functions/bm_hs012.py
-drwxr-xr-x   0 andrei     (501) staff       (20)        0 2023-07-27 18:27:58.812441 teneva_bm-0.5.0/teneva_bm/hs/draft_unconstrained_functions/
--rw-r--r--   0 andrei     (501) staff       (20)      209 2023-07-17 20:25:36.000000 teneva_bm-0.5.0/teneva_bm/hs/draft_unconstrained_functions/__init__.py
--rw-r--r--   0 andrei     (501) staff       (20)     1937 2023-07-17 20:25:36.000000 teneva_bm-0.5.0/teneva_bm/hs/draft_unconstrained_functions/bm_hs002.py
--rw-r--r--   0 andrei     (501) staff       (20)     1857 2023-07-17 20:25:36.000000 teneva_bm-0.5.0/teneva_bm/hs/draft_unconstrained_functions/bm_hs003.py
--rw-r--r--   0 andrei     (501) staff       (20)     1839 2023-07-17 20:25:36.000000 teneva_bm-0.5.0/teneva_bm/hs/draft_unconstrained_functions/bm_hs004.py
--rw-r--r--   0 andrei     (501) staff       (20)     2197 2023-07-17 20:25:36.000000 teneva_bm-0.5.0/teneva_bm/hs/draft_unconstrained_functions/bm_hs005.py
--rw-r--r--   0 andrei     (501) staff       (20)     2275 2023-07-17 20:25:36.000000 teneva_bm-0.5.0/teneva_bm/hs/draft_unconstrained_functions/bm_hs038.py
--rw-r--r--   0 andrei     (501) staff       (20)     1929 2023-07-17 20:25:36.000000 teneva_bm-0.5.0/teneva_bm/hs/draft_unconstrained_functions/bm_hs045.py
-drwxr-xr-x   0 andrei     (501) staff       (20)        0 2023-07-27 18:27:58.815366 teneva_bm-0.5.0/teneva_bm/oc/
--rw-r--r--   0 andrei     (501) staff       (20)       87 2023-07-13 07:42:11.000000 teneva_bm-0.5.0/teneva_bm/oc/__init__.py
--rw-r--r--   0 andrei     (501) staff       (20)     4166 2023-07-27 10:24:35.000000 teneva_bm-0.5.0/teneva_bm/oc/bm_oc_simple.py
--rw-r--r--   0 andrei     (501) staff       (20)     2265 2023-07-27 10:24:30.000000 teneva_bm-0.5.0/teneva_bm/oc/bm_oc_simple_constr.py
-drwxr-xr-x   0 andrei     (501) staff       (20)        0 2023-07-27 18:27:58.818583 teneva_bm-0.5.0/teneva_bm/qubo/
--rw-r--r--   0 andrei     (501) staff       (20)      166 2023-07-22 15:44:37.000000 teneva_bm-0.5.0/teneva_bm/qubo/__init__.py
--rw-r--r--   0 andrei     (501) staff       (20)     7023 2023-07-27 10:23:51.000000 teneva_bm-0.5.0/teneva_bm/qubo/bm_qubo_knap_det.py
--rw-r--r--   0 andrei     (501) staff       (20)     1861 2023-07-27 10:23:56.000000 teneva_bm-0.5.0/teneva_bm/qubo/bm_qubo_knap_quad.py
--rw-r--r--   0 andrei     (501) staff       (20)     2979 2023-07-27 10:24:01.000000 teneva_bm-0.5.0/teneva_bm/qubo/bm_qubo_maxcut.py
--rw-r--r--   0 andrei     (501) staff       (20)     2985 2023-07-27 10:24:04.000000 teneva_bm-0.5.0/teneva_bm/qubo/bm_qubo_mvc.py
--rw-r--r--   0 andrei     (501) staff       (20)     3386 2023-07-24 16:41:38.000000 teneva_bm-0.5.0/teneva_bm/teneva_bm_demo.py
-drwxr-xr-x   0 andrei     (501) staff       (20)        0 2023-07-27 18:27:58.821270 teneva_bm-0.5.0/teneva_bm/various/
--rw-r--r--   0 andrei     (501) staff       (20)      105 2023-07-13 07:41:21.000000 teneva_bm-0.5.0/teneva_bm/various/__init__.py
--rw-r--r--   0 andrei     (501) staff       (20)     7794 2023-07-27 11:58:55.000000 teneva_bm-0.5.0/teneva_bm/various/bm_matmul.py
--rw-r--r--   0 andrei     (501) staff       (20)    12653 2023-07-27 13:50:14.000000 teneva_bm-0.5.0/teneva_bm/various/bm_topopt.py
--rw-r--r--   0 andrei     (501) staff       (20)     1867 2023-07-27 10:23:32.000000 teneva_bm-0.5.0/teneva_bm/various/bm_wall_simple.py
-drwxr-xr-x   0 andrei     (501) staff       (20)        0 2023-07-27 18:27:58.787775 teneva_bm-0.5.0/teneva_bm.egg-info/
--rw-r--r--   0 andrei     (501) staff       (20)    18567 2023-07-27 18:27:58.000000 teneva_bm-0.5.0/teneva_bm.egg-info/PKG-INFO
--rw-r--r--   0 andrei     (501) staff       (20)     2179 2023-07-27 18:27:58.000000 teneva_bm-0.5.0/teneva_bm.egg-info/SOURCES.txt
--rw-r--r--   0 andrei     (501) staff       (20)        1 2023-07-27 18:27:58.000000 teneva_bm-0.5.0/teneva_bm.egg-info/dependency_links.txt
--rw-r--r--   0 andrei     (501) staff       (20)       33 2023-07-27 18:27:58.000000 teneva_bm-0.5.0/teneva_bm.egg-info/requires.txt
--rw-r--r--   0 andrei     (501) staff       (20)       10 2023-07-27 18:27:58.000000 teneva_bm-0.5.0/teneva_bm.egg-info/top_level.txt
+drwxr-xr-x   0 andrei     (501) staff       (20)        0 2023-07-30 18:22:58.554334 teneva_bm-0.6.0/
+-rw-r--r--   0 andrei     (501) staff       (20)     1090 2023-02-25 19:29:59.000000 teneva_bm-0.6.0/LICENSE.txt
+-rw-r--r--   0 andrei     (501) staff       (20)       79 2023-07-27 07:17:23.000000 teneva_bm-0.6.0/MANIFEST.in
+-rw-r--r--   0 andrei     (501) staff       (20)    19920 2023-07-30 18:22:58.554727 teneva_bm-0.6.0/PKG-INFO
+-rw-r--r--   0 andrei     (501) staff       (20)    18659 2023-07-30 18:22:24.000000 teneva_bm-0.6.0/README.md
+-rw-r--r--   0 andrei     (501) staff       (20)      899 2023-07-29 14:29:03.000000 teneva_bm-0.6.0/demo.py
+-rw-r--r--   0 andrei     (501) staff       (20)       33 2023-07-29 13:15:53.000000 teneva_bm-0.6.0/requirements.txt
+-rw-r--r--   0 andrei     (501) staff       (20)      107 2023-07-30 18:22:58.555926 teneva_bm-0.6.0/setup.cfg
+-rw-r--r--   0 andrei     (501) staff       (20)     2518 2023-07-16 14:04:06.000000 teneva_bm-0.6.0/setup.py
+drwxr-xr-x   0 andrei     (501) staff       (20)        0 2023-07-30 18:22:58.490528 teneva_bm-0.6.0/teneva_bm/
+-rw-r--r--   0 andrei     (501) staff       (20)      211 2023-07-30 18:22:18.000000 teneva_bm-0.6.0/teneva_bm/__init__.py
+drwxr-xr-x   0 andrei     (501) staff       (20)        0 2023-07-30 18:22:58.499773 teneva_bm-0.6.0/teneva_bm/agent/
+-rw-r--r--   0 andrei     (501) staff       (20)      319 2023-07-30 16:47:21.000000 teneva_bm-0.6.0/teneva_bm/agent/__init__.py
+-rw-r--r--   0 andrei     (501) staff       (20)     7232 2023-07-30 17:54:09.000000 teneva_bm-0.6.0/teneva_bm/agent/agent.py
+-rw-r--r--   0 andrei     (501) staff       (20)     2076 2023-07-30 16:06:42.000000 teneva_bm-0.6.0/teneva_bm/agent/bm_agent_ant.py
+-rw-r--r--   0 andrei     (501) staff       (20)     2092 2023-07-30 15:54:04.000000 teneva_bm-0.6.0/teneva_bm/agent/bm_agent_human.py
+-rw-r--r--   0 andrei     (501) staff       (20)     2139 2023-07-30 15:53:56.000000 teneva_bm-0.6.0/teneva_bm/agent/bm_agent_human_stand.py
+-rw-r--r--   0 andrei     (501) staff       (20)     6617 2023-07-30 18:20:22.000000 teneva_bm-0.6.0/teneva_bm/agent/bm_agent_lake.py
+-rw-r--r--   0 andrei     (501) staff       (20)     2136 2023-07-30 16:47:47.000000 teneva_bm-0.6.0/teneva_bm/agent/bm_agent_pend_inv.py
+-rw-r--r--   0 andrei     (501) staff       (20)     2185 2023-07-30 16:47:42.000000 teneva_bm-0.6.0/teneva_bm/agent/bm_agent_pend_inv_double.py
+-rw-r--r--   0 andrei     (501) staff       (20)     2288 2023-07-30 15:24:14.000000 teneva_bm-0.6.0/teneva_bm/agent/bm_agent_swimmer.py
+-rw-r--r--   0 andrei     (501) staff       (20)     3323 2023-07-30 15:46:50.000000 teneva_bm-0.6.0/teneva_bm/agent/policy.py
+-rw-r--r--   0 andrei     (501) staff       (20)    35039 2023-07-30 14:19:05.000000 teneva_bm-0.6.0/teneva_bm/bm.py
+drwxr-xr-x   0 andrei     (501) staff       (20)        0 2023-07-30 18:22:58.530348 teneva_bm-0.6.0/teneva_bm/func/
+-rw-r--r--   0 andrei     (501) staff       (20)      516 2023-07-13 07:42:30.000000 teneva_bm-0.6.0/teneva_bm/func/__init__.py
+-rw-r--r--   0 andrei     (501) staff       (20)     3548 2023-07-30 10:47:49.000000 teneva_bm-0.6.0/teneva_bm/func/bm_func_ackley.py
+-rw-r--r--   0 andrei     (501) staff       (20)     2301 2023-07-30 10:08:14.000000 teneva_bm-0.6.0/teneva_bm/func/bm_func_alpine.py
+-rw-r--r--   0 andrei     (501) staff       (20)     2430 2023-07-30 10:52:13.000000 teneva_bm-0.6.0/teneva_bm/func/bm_func_dixon.py
+-rw-r--r--   0 andrei     (501) staff       (20)     2295 2023-07-30 10:52:30.000000 teneva_bm-0.6.0/teneva_bm/func/bm_func_exp.py
+-rw-r--r--   0 andrei     (501) staff       (20)     2746 2023-07-30 10:13:15.000000 teneva_bm-0.6.0/teneva_bm/func/bm_func_griewank.py
+-rw-r--r--   0 andrei     (501) staff       (20)     3590 2023-07-30 10:53:24.000000 teneva_bm-0.6.0/teneva_bm/func/bm_func_michalewicz.py
+-rw-r--r--   0 andrei     (501) staff       (20)     2421 2023-07-30 10:17:40.000000 teneva_bm-0.6.0/teneva_bm/func/bm_func_piston.py
+-rw-r--r--   0 andrei     (501) staff       (20)     2478 2023-07-30 10:55:11.000000 teneva_bm-0.6.0/teneva_bm/func/bm_func_qing.py
+-rw-r--r--   0 andrei     (501) staff       (20)     3091 2023-07-30 10:19:45.000000 teneva_bm-0.6.0/teneva_bm/func/bm_func_rastrigin.py
+-rw-r--r--   0 andrei     (501) staff       (20)     3155 2023-07-30 10:56:44.000000 teneva_bm-0.6.0/teneva_bm/func/bm_func_rosenbrock.py
+-rw-r--r--   0 andrei     (501) staff       (20)     2129 2023-07-30 10:56:51.000000 teneva_bm-0.6.0/teneva_bm/func/bm_func_schaffer.py
+-rw-r--r--   0 andrei     (501) staff       (20)     3132 2023-07-30 10:22:30.000000 teneva_bm-0.6.0/teneva_bm/func/bm_func_schwefel.py
+drwxr-xr-x   0 andrei     (501) staff       (20)        0 2023-07-30 18:22:58.532446 teneva_bm-0.6.0/teneva_bm/hs/
+-rw-r--r--   0 andrei     (501) staff       (20)       78 2023-07-17 21:02:17.000000 teneva_bm-0.6.0/teneva_bm/hs/__init__.py
+-rw-r--r--   0 andrei     (501) staff       (20)     1755 2023-07-30 11:13:53.000000 teneva_bm-0.6.0/teneva_bm/hs/bm_hs_func001.py
+-rw-r--r--   0 andrei     (501) staff       (20)     2430 2023-07-30 11:26:02.000000 teneva_bm-0.6.0/teneva_bm/hs/bm_hs_func006.py
+drwxr-xr-x   0 andrei     (501) staff       (20)        0 2023-07-30 18:22:58.540284 teneva_bm-0.6.0/teneva_bm/hs/draft_constrained_functions/
+-rw-r--r--   0 andrei     (501) staff       (20)      209 2023-07-17 20:25:36.000000 teneva_bm-0.6.0/teneva_bm/hs/draft_constrained_functions/__init__.py
+-rw-r--r--   0 andrei     (501) staff       (20)     2272 2023-07-17 20:25:36.000000 teneva_bm-0.6.0/teneva_bm/hs/draft_constrained_functions/bm_hs007.py
+-rw-r--r--   0 andrei     (501) staff       (20)     2459 2023-07-17 20:25:36.000000 teneva_bm-0.6.0/teneva_bm/hs/draft_constrained_functions/bm_hs008.py
+-rw-r--r--   0 andrei     (501) staff       (20)     2318 2023-07-17 20:25:36.000000 teneva_bm-0.6.0/teneva_bm/hs/draft_constrained_functions/bm_hs009.py
+-rw-r--r--   0 andrei     (501) staff       (20)     2266 2023-07-17 20:25:36.000000 teneva_bm-0.6.0/teneva_bm/hs/draft_constrained_functions/bm_hs010.py
+-rw-r--r--   0 andrei     (501) staff       (20)     2251 2023-07-17 20:25:36.000000 teneva_bm-0.6.0/teneva_bm/hs/draft_constrained_functions/bm_hs011.py
+-rw-r--r--   0 andrei     (501) staff       (20)     2376 2023-07-17 20:25:36.000000 teneva_bm-0.6.0/teneva_bm/hs/draft_constrained_functions/bm_hs012.py
+drwxr-xr-x   0 andrei     (501) staff       (20)        0 2023-07-30 18:22:58.545703 teneva_bm-0.6.0/teneva_bm/hs/draft_unconstrained_functions/
+-rw-r--r--   0 andrei     (501) staff       (20)      209 2023-07-17 20:25:36.000000 teneva_bm-0.6.0/teneva_bm/hs/draft_unconstrained_functions/__init__.py
+-rw-r--r--   0 andrei     (501) staff       (20)     1937 2023-07-17 20:25:36.000000 teneva_bm-0.6.0/teneva_bm/hs/draft_unconstrained_functions/bm_hs002.py
+-rw-r--r--   0 andrei     (501) staff       (20)     1857 2023-07-17 20:25:36.000000 teneva_bm-0.6.0/teneva_bm/hs/draft_unconstrained_functions/bm_hs003.py
+-rw-r--r--   0 andrei     (501) staff       (20)     1839 2023-07-17 20:25:36.000000 teneva_bm-0.6.0/teneva_bm/hs/draft_unconstrained_functions/bm_hs004.py
+-rw-r--r--   0 andrei     (501) staff       (20)     2197 2023-07-17 20:25:36.000000 teneva_bm-0.6.0/teneva_bm/hs/draft_unconstrained_functions/bm_hs005.py
+-rw-r--r--   0 andrei     (501) staff       (20)     2275 2023-07-17 20:25:36.000000 teneva_bm-0.6.0/teneva_bm/hs/draft_unconstrained_functions/bm_hs038.py
+-rw-r--r--   0 andrei     (501) staff       (20)     1929 2023-07-17 20:25:36.000000 teneva_bm-0.6.0/teneva_bm/hs/draft_unconstrained_functions/bm_hs045.py
+drwxr-xr-x   0 andrei     (501) staff       (20)        0 2023-07-30 18:22:58.547925 teneva_bm-0.6.0/teneva_bm/odeoc/
+-rw-r--r--   0 andrei     (501) staff       (20)       99 2023-07-30 11:32:37.000000 teneva_bm-0.6.0/teneva_bm/odeoc/__init__.py
+-rw-r--r--   0 andrei     (501) staff       (20)     4237 2023-07-30 11:37:21.000000 teneva_bm-0.6.0/teneva_bm/odeoc/bm_odeoc_simple.py
+-rw-r--r--   0 andrei     (501) staff       (20)     2292 2023-07-30 11:37:44.000000 teneva_bm-0.6.0/teneva_bm/odeoc/bm_odeoc_simple_constr.py
+drwxr-xr-x   0 andrei     (501) staff       (20)        0 2023-07-30 18:22:58.551024 teneva_bm-0.6.0/teneva_bm/qubo/
+-rw-r--r--   0 andrei     (501) staff       (20)      166 2023-07-22 15:44:37.000000 teneva_bm-0.6.0/teneva_bm/qubo/__init__.py
+-rw-r--r--   0 andrei     (501) staff       (20)     7111 2023-07-30 11:04:30.000000 teneva_bm-0.6.0/teneva_bm/qubo/bm_qubo_knap_det.py
+-rw-r--r--   0 andrei     (501) staff       (20)     1834 2023-07-30 11:06:13.000000 teneva_bm-0.6.0/teneva_bm/qubo/bm_qubo_knap_quad.py
+-rw-r--r--   0 andrei     (501) staff       (20)     2967 2023-07-30 11:07:28.000000 teneva_bm-0.6.0/teneva_bm/qubo/bm_qubo_maxcut.py
+-rw-r--r--   0 andrei     (501) staff       (20)     2973 2023-07-30 11:08:28.000000 teneva_bm-0.6.0/teneva_bm/qubo/bm_qubo_mvc.py
+-rw-r--r--   0 andrei     (501) staff       (20)     3377 2023-07-29 14:31:04.000000 teneva_bm-0.6.0/teneva_bm/teneva_bm_demo.py
+drwxr-xr-x   0 andrei     (501) staff       (20)        0 2023-07-30 18:22:58.553751 teneva_bm-0.6.0/teneva_bm/various/
+-rw-r--r--   0 andrei     (501) staff       (20)      105 2023-07-13 07:41:21.000000 teneva_bm-0.6.0/teneva_bm/various/__init__.py
+-rw-r--r--   0 andrei     (501) staff       (20)     7790 2023-07-30 11:28:44.000000 teneva_bm-0.6.0/teneva_bm/various/bm_matmul.py
+-rw-r--r--   0 andrei     (501) staff       (20)    12645 2023-07-30 11:24:08.000000 teneva_bm-0.6.0/teneva_bm/various/bm_topopt.py
+-rw-r--r--   0 andrei     (501) staff       (20)     1867 2023-07-30 11:18:40.000000 teneva_bm-0.6.0/teneva_bm/various/bm_wall_simple.py
+drwxr-xr-x   0 andrei     (501) staff       (20)        0 2023-07-30 18:22:58.494135 teneva_bm-0.6.0/teneva_bm.egg-info/
+-rw-r--r--   0 andrei     (501) staff       (20)    19920 2023-07-30 18:22:58.000000 teneva_bm-0.6.0/teneva_bm.egg-info/PKG-INFO
+-rw-r--r--   0 andrei     (501) staff       (20)     2312 2023-07-30 18:22:58.000000 teneva_bm-0.6.0/teneva_bm.egg-info/SOURCES.txt
+-rw-r--r--   0 andrei     (501) staff       (20)        1 2023-07-30 18:22:58.000000 teneva_bm-0.6.0/teneva_bm.egg-info/dependency_links.txt
+-rw-r--r--   0 andrei     (501) staff       (20)       33 2023-07-30 18:22:58.000000 teneva_bm-0.6.0/teneva_bm.egg-info/requires.txt
+-rw-r--r--   0 andrei     (501) staff       (20)       10 2023-07-30 18:22:58.000000 teneva_bm-0.6.0/teneva_bm.egg-info/top_level.txt
```

### Comparing `teneva_bm-0.5.0/LICENSE.txt` & `teneva_bm-0.6.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `teneva_bm-0.5.0/PKG-INFO` & `teneva_bm-0.6.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: teneva_bm
-Version: 0.5.0
+Version: 0.6.0
 Summary: Benchmarks library, based on the software product teneva, for testing multivariate approximation and optimization methods
 Home-page: https://github.com/AndreiChertkov/teneva_bm
 Author: Andrei Chertkov
 Author-email: andre.chertkov@gmail.com
 License: MIT
 Project-URL: Source, https://github.com/AndreiChertkov/teneva_bm
 Keywords: benchmarks approximation optimization multidimensional array multivariate function low-rank representation tensor train format TT-decomposition
@@ -30,30 +30,30 @@
 ## Description
 
 Benchmarks library, based on the software product [teneva](https://github.com/AndreiChertkov/teneva), for testing multidimensional approximation and optimization methods. Our benchmarks include both multidimensional data arrays and discretized functions of many variables.
 
 
 ## Installation
 
-> Current version "0.5.0".
+> Current version "0.6.0".
 
-The package can be installed via pip: `pip install teneva_bm` (it requires the [Python](https://www.python.org) programming language of the version >= 3.8). It can be also downloaded from the repository [teneva_bm](https://github.com/AndreiChertkov/teneva_bm) and installed by `python setup.py install` command from the root folder of the project.
+The package can be installed via pip: `pip install teneva_bm` (it requires the [Python](https://www.python.org) programming language of the version 3.8 or 3.9). It can be also downloaded from the repository [teneva_bm](https://github.com/AndreiChertkov/teneva_bm) and installed by `python setup.py install` command from the root folder of the project.
 
-> Required python packages (see `requirements.txt`) [matplotlib](https://matplotlib.org/) (3.7.0+) and [teneva](https://github.com/AndreiChertkov/teneva) (0.14.2+) will be automatically installed during the installation of the main software product.
+> Required python packages (see `requirements.txt`) [matplotlib](https://matplotlib.org/) (3.7.0+) and [teneva](https://github.com/AndreiChertkov/teneva) (0.14.5+) will be automatically installed during the installation of the main software product.
 
-Some benchmarks require additional installation of specialized libraries. The corresponding instructions are given in the description of each benchmark (see `DESC` string in the python files with benchmarks). Installation of all required libraries for all benchmarks can be done with the following command:
+Some benchmarks require additional installation of specialized libraries. The corresponding instructions are given in the description of each benchmark (see `DESC` string in the python files with benchmarks). Installation of all required libraries for all benchmarks can be done with the following commands:
 
 - Collections `func`, `hs` and `various` do not require installation of additional libraries.
 
-- Сollections `oc` and `qubo` require installation of the following libraries:
+- Сollections `odeoc` and `qubo` require installation of the following libraries:
     ```bash
     pip install networkx==3.0 qubogen==0.1.1 gekko==1.0.6
     ```
 
-- Сollections `agent` and `agent_toe` require a rather complicated installation process of the `gym` and `mujoco` frameworks and related packages, so we have prepared a special python installation script [install_mujoco.py](https://github.com/AndreiChertkov/teneva_bm/blob/main/install_mujoco.py). Detailed instructions for using the script are presented in the file header.
+- Сollection `agent` require a rather complicated installation process of the `gym` and `mujoco` frameworks and related packages, so we have prepared a special python installation script [install_mujoco.py](https://github.com/AndreiChertkov/teneva_bm/blob/main/install_mujoco.py). Detailed instructions for using the script are presented in the file header.
 
 > To run benchmark optimization examples (see `demo_opti` folder), you should also install the [PROTES](https://github.com/anabatsh/PROTES) optimizer (`pip install protes==0.3.3`).
 
 
 ## Documentation and examples
 
 All benchmarks inherit from the `Bm` base class (`teneva_bm/bm.py`) and are located in the subfolders (collections of benchmarks) of `teneva_bm` folder. The corresponding python files contain a detailed description of the benchmarks, as well as a scripts for a demo run at the end of the files. You can get detailed information on the created benchmark using the `info` class method:
@@ -66,30 +66,28 @@
 
 You can run demos for all benchmarks at once with the command `python demo.py` from the root folder of the project (you can also specify the name of the benchmark as a script argument to run the demo for only one benchmark, e.g., `python demo.py bm_qubo_knap_det`). You can also use a function from the `teneva_bm` package to run all or only one demo:
 ```python
 from teneva_bm import teneva_bm_demo
 teneva_bm_demo('bm_qubo_knap_det', with_info=True)
 ```
 
-> We prepare some demo scripts with benchmark optimization examples in the `demo_opti` folder. To run these examples (e.g., `python demo_opti/demo_base.py`), you need to install the [PROTES](https://github.com/anabatsh/PROTES) optimizer (`pip install protes==0.3.3`).
-
-> We also present some examples in this [colab notebook](https://colab.research.google.com/drive/1z8LgqEARJziKub2dVB65CHkhcboc-fCH?usp=sharing).
+> We prepare some demo scripts with benchmark optimization examples in the `demo_opti` folder. To run these examples (e.g., `python demo_opti/base.py`), you need to install the [PROTES](https://github.com/anabatsh/PROTES) optimizer). We also present some examples in this [colab notebook](https://colab.research.google.com/drive/1z8LgqEARJziKub2dVB65CHkhcboc-fCH?usp=sharing).
 
 
 ## Available benchmarks
 
-- `agent` - the collection of problems from [gym](https://www.gymlibrary.dev/) framework, including [mujoco agents](https://www.gymlibrary.dev/environments/mujoco/index.html) based on the physics engine [mujoco](https://mujoco.org/) for faciliatating research and development in robotics, biomechanics, graphics and animation. The collection includes the following benchmarks: `BmAgentSwimmer`.
-    > Within the framework of this collection, explicit optimization of the entire set of actions (discrete or continuous) may be performed (i.e., `none` policy) or discrete Toeplitz policy may be used.
+- `agent` - the collection of problems from [gym](https://www.gymlibrary.dev/) framework, including [mujoco agents](https://www.gymlibrary.dev/environments/mujoco/index.html) based on the physics engine [mujoco](https://mujoco.org/) for faciliatating research and development in robotics, biomechanics, graphics and animation. The collection includes the following benchmarks: `BmAgentAnt`, `BmAgentHuman`, `BmAgentHumanStand`, `BmAgentLake`, `BmAgentPendInv`, `BmAgentPendInvDouble`, `BmAgentSwimmer`.
+    > Within the framework of this collection, explicit optimization of the entire set of actions (discrete or continuous) may be performed (if `direct` policy name is set) or discrete Toeplitz policy may be used (if `toeplitz` policy name is set; it is the default value); you can also set your own custom policy as an instance of the correct class (see `agent/policy.py` for details).
 
 - `func` - a collection of analytic functions of a real multidimensional argument. The collection includes the following benchmarks: `BmFuncAckley`, `BmFuncAlpine`, `BmFuncDixon`, `BmFuncExp`, `BmFuncGriewank`, `BmFuncMichalewicz`, `BmFuncPiston` (only `d=7` is supported), `BmFuncQing`, `BmFuncRastrigin`, `BmFuncRosenbrock`, `BmFuncSchaffer`, `BmFuncSchwefel`.
     > For almost all functions, the exact global minimum ("continuous x point", not multi-index) is known (see `bm.x_min_real` and `bm.y_min_real`). For a number of functions (`BmFuncAlpine`, `BmFuncExp`, `BmFuncGriewank`, `BmFuncMichalewicz`, `BmFuncQing`, `BmFuncRastrigin`, `BmFuncRosenbrock`, `BmFuncSchwefel`), a `bm.build_cores()` method is available that returns an exact representation of the function on the discrete grid used in the benchmark in the tensor train (TT) format as a list of 3D TT-cores. Note also that we apply small random shift of the grid limits for all functions, to make the optimization problem more difficult (because many functions have a minimum at the center point of the domain).
 
 - `hs` (draft!) - the [Hock & Schittkowski](http://apmonitor.com/wiki/index.php/Apps/HockSchittkowski) collection of benchmark functions, containing continuous analytic functions of small dimensions (2-5), some of which have given constraints. The collection includes the following benchmarks: `BmHsFunc001`, `BmHsFunc006`.
 
-- `oc` - a collection of optimal control problems described by ordinary differential equations with discrete binary control variable, some of the problems have explicit restrictions on the elements of the control vector. The collection includes the following benchmarks: `BmOcSimple`, `BmOcSimpleConstr`.
+- `odeoc` - a collection of optimal control problems described by ordinary differential equations, some of the problems have explicit restrictions on the elements of the control vector. The collection includes the following benchmarks: `BmOdeocSimple`, `BmOdeocSimpleConstr`.
 
 - `qubo` - a collection of quadratic unconstrained binary optimization (QUBO) problems; all benchmarks are discrete and have a mode size equals `2`. The collection includes the following benchmarks: `BmQuboKnapDet`, `BmQuboKnapQuad`, `BmQuboMaxcut`, `BmQuboMvc`.
     > The exact global minimum is known only for `BmQuboKnapDet` benchmark (note that this benchmark supports only dimensions `10`, `20`, `50`, `80` and `100`).
 
 - `various` - a collection of heterogeneous benchmarks that are not suitable for any other collection (note that in this case, we do not use the name of the collection in the name of the benchmarks, unlike all other sets). The collection includes the following benchmarks: `BmMatmul`, `BmTopopt` (draft!), `BmWallSimple`.
 
 
@@ -99,110 +97,117 @@
 
 ##### Benchmark initialization
 
 First, we create an instance of the desired benchmark class and manually call the `prep` method (optionally, we can also print detailed information about the benchmark):
 ```python
 import numpy as np
 from teneva_bm import *
-np.random.seed(42)
 
 bm = BmFuncAckley()
 bm.prep()
 print(bm.info())
 ```
 
 The class constructor of all benchmarks has the following optional arguments:
 
 - `d` - dimension of the benchmark's input (non-negative integer). For some benchmarks, this number is hardcoded (or depends on other specified auxiliary arguments), if another value is explicitly passed, an error message will be generated (e.g., the dimension for benchmark `various.bm_matmul` is determined automatically by the values of auxiliary arguments `size`, `rank` and `only2`). By default, some correct value is used (specified in the benchmark description).
 
 - `n` - number of possible discrete values for benchmark input variables, i.e., the mode size of the related tensor / multidimensional array (non-negative integer if all mode sizes are equal or a list of non-negative integers of the length `d`). For some benchmarks, this number is hardcoded (or depends on other specified auxiliary arguments), if another value is explicitly passed, an error message will be generated (e.g., in `qubo` collection all benchmarks should have `n = 2`). By default, some correct value is used (specified in the benchmark description).
 
-- `name` - the display name of the benchmark (string). By default, the name corresponding to the file/class name is used.
+- `name` - the display name of the benchmark (string). By default, the name corresponding to the file/class name (without `Bm` prefix) is used.
 
 - `desc` - the description of the benchmark (string). By default, a detailed description of the benchmark is used, provided in the corresponding python file.
 
 - `...other arguments...` - some benchmarks have additional optional arguments, which are described in the corresponding python files.
 
 ##### Setting advanced options
 
 Before calling the `bm.prep()` method, you can set a number of additional benchmark options:
 
 - `bm.set_seed(seed=42)` - with this function we can set a custom random seed. Note that we use `Random Generator` from numpy (i.e., `numpy.random.default_rng(seed)`) and for a fixed value of the seed, the behavior of the benchmark will always be the same, however, not all benchmarks depend on a seed.
 
-- `bm.set_grid_kind(kind='cheb')` - by default, we use the Chebyshev grid (`kind = 'cheb'`), but you can alternatively set it manually to use a uniform grid (`kind = 'uni'`).
+- `bm.set_grid_kind(kind='cheb')` - by default, we use the Chebyshev grid (`kind = 'cheb'`) for benchmarks corresponds to a function of a continuous argument, but you can alternatively set it manually to use a uniform grid (`kind = 'uni'`).
 
 - `bm.set_budget(m=None, m_cache=None, is_strict=True)` - optional method to set the computation buget `m`. If the number of requests to the benchmark (from calls to `bm.get` and `bm.get_poi` methods) exceeds the specified budget, then `None` will be returned. If the flag `is_strict` is disabled, then the request for the last batch will be allowed, after which the budget will be exceeded, otherwise this last batch will not be considered. Note that when the budget is exceeded, `None` will be returned both when requesting a single value and a batch of values. Also, in a similar way, you can set a limit on the use of the cache by `m_cache` parameter.
 
-- `bm.set_constr(penalty=1.E+42, eps=1.E-16, with_amplitude=True)` - if the benchmark has a constraint, then using this function you can set a `penalty` (for the requested points that do not satisfy the constraint, the value `penalty * constraint_value` will be returned) and a `eps` (threshold value to check that the constraint has been fulfilled). Note that we set the constraints as a function (`bm.constr`) that returns the value `constraint_value` (amplitude) of the constraint, and if the constraint is met, then the value must be non-positive, otherwise, the objective function is not calculated and a value proportional to the amplitude of the constraint is returned (if you disable flag `with_amplitude`, then just the value of the penalty will be returned). For the case of maximization task you should set negative `penalty` value.
+- `bm.set_constr(penalty=1.E+42, eps=1.E-16, with_amplitude=True)` - if the benchmark has a constraint, then using this function you can set a `penalty` (for the requested points that do not satisfy the constraint, the value `penalty * constraint_value` will be returned) and a `eps` (threshold value to check that the constraint has been fulfilled). Note that we set the constraints as a function (`bm.constr` / `bm.constr_batch`) that returns the value `constraint_value` (amplitude) of the constraint, and if the constraint is met, then the value must be non-positive, otherwise, the objective function is not calculated and a value proportional to the amplitude of the constraint is returned (if you disable flag `with_amplitude`, then just the value of the penalty will be returned). For the case of maximization task you should set negative `penalty` value.
 
 - `bm.set_max(i=None, x=None, y=None)` - if necessary, you can manually set the multi-index, the corresponding continuous point (for benchmarks, which relate to functions of a continuous argument), and the corresponding value for the exact global maximum of the function. The corresponding values will be further available in the benchmark as `bm.i_max_real`, `bm.x_max_real` and `bm.y_max_real` respectively. When the benchmark is initialized, this function is called automatically if the optimum is known.
 
 - `bm.set_min(i=None, x=None, y=None)` - the same as in the previous point, but for the global minimum.
 
-- `bm.set_log(with_log=False, cond='min-max', step=1000, prefix='bm', with_min=True, with_max=True)` - when calling this function with the `True` argument `with_log`, the log will be printed while requests to benchmark. You may set the log codition `cond` (`min`, `max`, `min-max` or `step`; e.g., in the case `min` the log will be presented each time the `min` value is updated), the log step (for condition `step`) and a string `prefix` for the log. You can also disable the display of current minimum values (`with_min`) or maximum values (`with_max`) in the log string.
+- `bm.set_log(log=False, cond='min-max', step=1000, prefix='bm', with_min=True, with_max=True)` - when calling this function with the `True` argument `log`, the log will be printed while requests to benchmark. You may set the log codition `cond` (`min`, `max`, `min-max` or `step`; e.g., in the case `min` the log will be presented each time the `min` value is updated), the log step (for condition `step`) and a string `prefix` for the log. You can also disable the display of current minimum values (`with_min`) or maximum values (`with_max`) in the log string. Note that you can provide as `log` argument some print-like function, e.g., `log=print`, in this case, printing will occur not to the console, but to the corresponding function.
 
-- `bm.set_cache(with_cache=False, cache=None, m_max=1.E+8)` - when calling this function with the `True` argument `with_cache`, the cache will be used, that is, all the values requested from the benchmark will be saved and when the same multi-indices are accessed again, the values will be retrieved from the cache instead of explicitly calculating the objective function. Additionally, you can optionally pass as an argument `cache` an already existing cache in the form of a dictionary (the keys are multi-indices in the form of tuples, and the values are the corresponding values of the objective function). We especially note that the cache is only used when querying benchmark values in discrete multi-indices; for requested continuous points, no cache will be used. It is also important to note that no cache will be used for matching multi-indices in the same requested batch of values. Optionally, you can set `m_max` argument that specifies the maximum cache size. If the size is exceeded, the cache will be cleared and a corresponding warning will be displayed.
+- `bm.set_cache(with_cache=False, cache=None, m_max=1.E+8)` - when calling this function with the `True` argument `with_cache`, the cache will be used, that is, all the values requested from the benchmark will be saved and when the same multi-indices are accessed again, the values will be retrieved from the cache instead of explicitly calculating the objective function. Additionally, you can optionally pass as an argument `cache` an already existing cache in the form of a dictionary (the keys are multi-indices in the form of tuples, and the values are the corresponding values of the objective function). We especially note that the cache is only used when querying benchmark values in discrete multi-indices; for requested continuous points, no cache will be used. It is also important to note that no cache will be used for matching multi-indices in the same requested batch of values. Optionally, you can set `m_max` argument that specifies the maximum cache size. If the size is exceeded, the cache will be cleared and a corresponding warning will be displayed to the log. Note that when the `bm.init` method is called, the cache is always reset to zero.
 
 - `bm.set_opts(...)` - for some benchmarks, this function may be called to set additional benchmark-specific options (please see the description of arguments in the relevant benchmark code file).
 
+> You can get all configuration options as a dictionary by the function `bm.get_config()`.
+
 ##### Computing benchmark values
 
 Now the benchmark is ready to go, and we can calculate its value in any requested discrete multi-index (a real number will be returned) or a list of its values for any requested batch of discrete multi-indices (1D numpy array of real numbers will be returned):
 ```python
 # Get value at multi-index i:
 i = np.ones(bm.d)
 print(bm[i]) # you can use the alias "bm.get(i)"
 
 # Get values for batch of multi-indices I:
 I = np.array([i, i+1, i+2])
 print(bm[I]) # you can use the alias "bm.get(I)"
 ```
 Note that the `get` method can be used instead of `[ ]` notation, for example, if it is necessary to pass somewhere a function that calculates benchmark values.
 
-Since the considered benchmark (`BmFuncAckley`) corresponds to a function of a continuous argument, above we calculated the values for the discretization of the function on a given grid. Additionally, we can calculate values at continuous points by analogy:
+Since the considered benchmark (`BmFuncAckley`) corresponds to a function of a continuous argument, above we calculated the values for the discretization of the function on a automatically selected grid. Additionally, we can calculate values at continuous points by analogy:
 ```python
 # Get value at point x:
 x = np.ones(bm.d) * 0.42
 print(bm(x)) # you can use the alias "bm.get_poi(x)"
 
 # Get values for batch of points X:
 X = np.array([x, x*0.3, x*1.1])
 print(bm(X)) # you can use the alias "bm.get_poi(X)"
 ```
 
-##### Data set generation
+##### Dataset generation
 
 For convenience, the benchmark also has functions that allow you to generate training and test data sets on a discrete grid:
 ```python
 # Generate random train dataset (from LHS):
 # I_trn is array of [500, bm.d] and y_trn is [500]
 I_trn, y_trn = bm.build_trn(500)
 
 # Generate random test dataset (from random choice):
 # I_tst is array of [100, bm.d] and y_tst of [100]
 I_tst, y_tst = bm.build_tst(100)
 ```
 
+> Note that, by default, the spent computational budget (see `bm.set_budget` function) and time spent does not change when the test dataset is generated (this is controlled by the default `skip_process` flag value in `bm.build_tst(m=0, skip_process=True)`), but is consumed when generating the training dataset (i.e., `bm.build_trn(m=0, skip_process=False)`).
+
 ##### Request history analysis
 
 During requests to the benchmark, that is, when calling functions `bm[]` (or `bm.get`), `bm()` (or `bm.get_poi`), `bm.build_trn` (if the flag `skip_process` is not set in the function arguments; it has a value `False` by default) and `bm.build_tst` (if `skip_process` is not set; it is `True` by default for this function), the following useful class parameters are updated:
 
 - `bm.m` - the total number of performed calculations of the benchmark value (if a cache is used, then the values taken from the cache are not taken into account in this variable).
 
 - `bm.m_cache` - the total number of cache hits performed instead of explicitly calculating benchmark values (if no cache is used, it is `0`).
 
 - `bm.time` - total time in seconds spent on calculating the benchmark values (the time spent on cache accesses is also taken into account).
 
+- `bm.time_full` - benchmark lifetime in seconds from the moment of initialization (i.e., the call to `bm.init` method).
+
 - `bm.y_list` - a list of all sequentially calculated benchmark values (results of cache accesses are also added to the list).
 
 - `bm.i_max`, `bm.x_max`, `bm.y_max` - a discrete multi-index, a continuous multi-dimensional point, and benchmark values corresponding to the maximum of all requested values. Note that for the case of a discrete function, the value of `x_max` will be `None`, and for the case of a continuous function, the values of `i_max` and `x_max` will correlate, while if requests were made for continuous points, then `x_max` will correspond to the exact position of the point, and `i_max` will be the nearest multi-index of the used discrete grid.
 
 - `bm.i_min`, `bm.x_min`, `bm.y_min` - same as in the previous point, but for the minimum value.
 
-The following function may be used to print the corresponding values: `print(bm.info_history())`.
+- `bm.i`, `bm.x`, `bm.y` - the last requested multi-index / point and the related computed benchmark's value.
+
+> The following function may be used to print the corresponding values: `print(bm.info_history())`. You can also get these values as a dictionary by the function `bm.get_history()`.
 
 ##### Notes
 
 - For some benchmarks (e.g., for all benchmarks from `agent` collection) the method `show` (present the current state, the state for provided input or the final state for the best found input) and `render` (present the animation for the current solution, the solution from the provided input or for the solution from the best found input) are available.
 
 
 ## Authors
```

### Comparing `teneva_bm-0.5.0/README.md` & `teneva_bm-0.6.0/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -4,30 +4,30 @@
 ## Description
 
 Benchmarks library, based on the software product [teneva](https://github.com/AndreiChertkov/teneva), for testing multidimensional approximation and optimization methods. Our benchmarks include both multidimensional data arrays and discretized functions of many variables.
 
 
 ## Installation
 
-> Current version "0.5.0".
+> Current version "0.6.0".
 
-The package can be installed via pip: `pip install teneva_bm` (it requires the [Python](https://www.python.org) programming language of the version >= 3.8). It can be also downloaded from the repository [teneva_bm](https://github.com/AndreiChertkov/teneva_bm) and installed by `python setup.py install` command from the root folder of the project.
+The package can be installed via pip: `pip install teneva_bm` (it requires the [Python](https://www.python.org) programming language of the version 3.8 or 3.9). It can be also downloaded from the repository [teneva_bm](https://github.com/AndreiChertkov/teneva_bm) and installed by `python setup.py install` command from the root folder of the project.
 
-> Required python packages (see `requirements.txt`) [matplotlib](https://matplotlib.org/) (3.7.0+) and [teneva](https://github.com/AndreiChertkov/teneva) (0.14.2+) will be automatically installed during the installation of the main software product.
+> Required python packages (see `requirements.txt`) [matplotlib](https://matplotlib.org/) (3.7.0+) and [teneva](https://github.com/AndreiChertkov/teneva) (0.14.5+) will be automatically installed during the installation of the main software product.
 
-Some benchmarks require additional installation of specialized libraries. The corresponding instructions are given in the description of each benchmark (see `DESC` string in the python files with benchmarks). Installation of all required libraries for all benchmarks can be done with the following command:
+Some benchmarks require additional installation of specialized libraries. The corresponding instructions are given in the description of each benchmark (see `DESC` string in the python files with benchmarks). Installation of all required libraries for all benchmarks can be done with the following commands:
 
 - Collections `func`, `hs` and `various` do not require installation of additional libraries.
 
-- Сollections `oc` and `qubo` require installation of the following libraries:
+- Сollections `odeoc` and `qubo` require installation of the following libraries:
     ```bash
     pip install networkx==3.0 qubogen==0.1.1 gekko==1.0.6
     ```
 
-- Сollections `agent` and `agent_toe` require a rather complicated installation process of the `gym` and `mujoco` frameworks and related packages, so we have prepared a special python installation script [install_mujoco.py](https://github.com/AndreiChertkov/teneva_bm/blob/main/install_mujoco.py). Detailed instructions for using the script are presented in the file header.
+- Сollection `agent` require a rather complicated installation process of the `gym` and `mujoco` frameworks and related packages, so we have prepared a special python installation script [install_mujoco.py](https://github.com/AndreiChertkov/teneva_bm/blob/main/install_mujoco.py). Detailed instructions for using the script are presented in the file header.
 
 > To run benchmark optimization examples (see `demo_opti` folder), you should also install the [PROTES](https://github.com/anabatsh/PROTES) optimizer (`pip install protes==0.3.3`).
 
 
 ## Documentation and examples
 
 All benchmarks inherit from the `Bm` base class (`teneva_bm/bm.py`) and are located in the subfolders (collections of benchmarks) of `teneva_bm` folder. The corresponding python files contain a detailed description of the benchmarks, as well as a scripts for a demo run at the end of the files. You can get detailed information on the created benchmark using the `info` class method:
@@ -40,30 +40,28 @@
 
 You can run demos for all benchmarks at once with the command `python demo.py` from the root folder of the project (you can also specify the name of the benchmark as a script argument to run the demo for only one benchmark, e.g., `python demo.py bm_qubo_knap_det`). You can also use a function from the `teneva_bm` package to run all or only one demo:
 ```python
 from teneva_bm import teneva_bm_demo
 teneva_bm_demo('bm_qubo_knap_det', with_info=True)
 ```
 
-> We prepare some demo scripts with benchmark optimization examples in the `demo_opti` folder. To run these examples (e.g., `python demo_opti/demo_base.py`), you need to install the [PROTES](https://github.com/anabatsh/PROTES) optimizer (`pip install protes==0.3.3`).
-
-> We also present some examples in this [colab notebook](https://colab.research.google.com/drive/1z8LgqEARJziKub2dVB65CHkhcboc-fCH?usp=sharing).
+> We prepare some demo scripts with benchmark optimization examples in the `demo_opti` folder. To run these examples (e.g., `python demo_opti/base.py`), you need to install the [PROTES](https://github.com/anabatsh/PROTES) optimizer). We also present some examples in this [colab notebook](https://colab.research.google.com/drive/1z8LgqEARJziKub2dVB65CHkhcboc-fCH?usp=sharing).
 
 
 ## Available benchmarks
 
-- `agent` - the collection of problems from [gym](https://www.gymlibrary.dev/) framework, including [mujoco agents](https://www.gymlibrary.dev/environments/mujoco/index.html) based on the physics engine [mujoco](https://mujoco.org/) for faciliatating research and development in robotics, biomechanics, graphics and animation. The collection includes the following benchmarks: `BmAgentSwimmer`.
-    > Within the framework of this collection, explicit optimization of the entire set of actions (discrete or continuous) may be performed (i.e., `none` policy) or discrete Toeplitz policy may be used.
+- `agent` - the collection of problems from [gym](https://www.gymlibrary.dev/) framework, including [mujoco agents](https://www.gymlibrary.dev/environments/mujoco/index.html) based on the physics engine [mujoco](https://mujoco.org/) for faciliatating research and development in robotics, biomechanics, graphics and animation. The collection includes the following benchmarks: `BmAgentAnt`, `BmAgentHuman`, `BmAgentHumanStand`, `BmAgentLake`, `BmAgentPendInv`, `BmAgentPendInvDouble`, `BmAgentSwimmer`.
+    > Within the framework of this collection, explicit optimization of the entire set of actions (discrete or continuous) may be performed (if `direct` policy name is set) or discrete Toeplitz policy may be used (if `toeplitz` policy name is set; it is the default value); you can also set your own custom policy as an instance of the correct class (see `agent/policy.py` for details).
 
 - `func` - a collection of analytic functions of a real multidimensional argument. The collection includes the following benchmarks: `BmFuncAckley`, `BmFuncAlpine`, `BmFuncDixon`, `BmFuncExp`, `BmFuncGriewank`, `BmFuncMichalewicz`, `BmFuncPiston` (only `d=7` is supported), `BmFuncQing`, `BmFuncRastrigin`, `BmFuncRosenbrock`, `BmFuncSchaffer`, `BmFuncSchwefel`.
     > For almost all functions, the exact global minimum ("continuous x point", not multi-index) is known (see `bm.x_min_real` and `bm.y_min_real`). For a number of functions (`BmFuncAlpine`, `BmFuncExp`, `BmFuncGriewank`, `BmFuncMichalewicz`, `BmFuncQing`, `BmFuncRastrigin`, `BmFuncRosenbrock`, `BmFuncSchwefel`), a `bm.build_cores()` method is available that returns an exact representation of the function on the discrete grid used in the benchmark in the tensor train (TT) format as a list of 3D TT-cores. Note also that we apply small random shift of the grid limits for all functions, to make the optimization problem more difficult (because many functions have a minimum at the center point of the domain).
 
 - `hs` (draft!) - the [Hock & Schittkowski](http://apmonitor.com/wiki/index.php/Apps/HockSchittkowski) collection of benchmark functions, containing continuous analytic functions of small dimensions (2-5), some of which have given constraints. The collection includes the following benchmarks: `BmHsFunc001`, `BmHsFunc006`.
 
-- `oc` - a collection of optimal control problems described by ordinary differential equations with discrete binary control variable, some of the problems have explicit restrictions on the elements of the control vector. The collection includes the following benchmarks: `BmOcSimple`, `BmOcSimpleConstr`.
+- `odeoc` - a collection of optimal control problems described by ordinary differential equations, some of the problems have explicit restrictions on the elements of the control vector. The collection includes the following benchmarks: `BmOdeocSimple`, `BmOdeocSimpleConstr`.
 
 - `qubo` - a collection of quadratic unconstrained binary optimization (QUBO) problems; all benchmarks are discrete and have a mode size equals `2`. The collection includes the following benchmarks: `BmQuboKnapDet`, `BmQuboKnapQuad`, `BmQuboMaxcut`, `BmQuboMvc`.
     > The exact global minimum is known only for `BmQuboKnapDet` benchmark (note that this benchmark supports only dimensions `10`, `20`, `50`, `80` and `100`).
 
 - `various` - a collection of heterogeneous benchmarks that are not suitable for any other collection (note that in this case, we do not use the name of the collection in the name of the benchmarks, unlike all other sets). The collection includes the following benchmarks: `BmMatmul`, `BmTopopt` (draft!), `BmWallSimple`.
 
 
@@ -73,110 +71,117 @@
 
 ##### Benchmark initialization
 
 First, we create an instance of the desired benchmark class and manually call the `prep` method (optionally, we can also print detailed information about the benchmark):
 ```python
 import numpy as np
 from teneva_bm import *
-np.random.seed(42)
 
 bm = BmFuncAckley()
 bm.prep()
 print(bm.info())
 ```
 
 The class constructor of all benchmarks has the following optional arguments:
 
 - `d` - dimension of the benchmark's input (non-negative integer). For some benchmarks, this number is hardcoded (or depends on other specified auxiliary arguments), if another value is explicitly passed, an error message will be generated (e.g., the dimension for benchmark `various.bm_matmul` is determined automatically by the values of auxiliary arguments `size`, `rank` and `only2`). By default, some correct value is used (specified in the benchmark description).
 
 - `n` - number of possible discrete values for benchmark input variables, i.e., the mode size of the related tensor / multidimensional array (non-negative integer if all mode sizes are equal or a list of non-negative integers of the length `d`). For some benchmarks, this number is hardcoded (or depends on other specified auxiliary arguments), if another value is explicitly passed, an error message will be generated (e.g., in `qubo` collection all benchmarks should have `n = 2`). By default, some correct value is used (specified in the benchmark description).
 
-- `name` - the display name of the benchmark (string). By default, the name corresponding to the file/class name is used.
+- `name` - the display name of the benchmark (string). By default, the name corresponding to the file/class name (without `Bm` prefix) is used.
 
 - `desc` - the description of the benchmark (string). By default, a detailed description of the benchmark is used, provided in the corresponding python file.
 
 - `...other arguments...` - some benchmarks have additional optional arguments, which are described in the corresponding python files.
 
 ##### Setting advanced options
 
 Before calling the `bm.prep()` method, you can set a number of additional benchmark options:
 
 - `bm.set_seed(seed=42)` - with this function we can set a custom random seed. Note that we use `Random Generator` from numpy (i.e., `numpy.random.default_rng(seed)`) and for a fixed value of the seed, the behavior of the benchmark will always be the same, however, not all benchmarks depend on a seed.
 
-- `bm.set_grid_kind(kind='cheb')` - by default, we use the Chebyshev grid (`kind = 'cheb'`), but you can alternatively set it manually to use a uniform grid (`kind = 'uni'`).
+- `bm.set_grid_kind(kind='cheb')` - by default, we use the Chebyshev grid (`kind = 'cheb'`) for benchmarks corresponds to a function of a continuous argument, but you can alternatively set it manually to use a uniform grid (`kind = 'uni'`).
 
 - `bm.set_budget(m=None, m_cache=None, is_strict=True)` - optional method to set the computation buget `m`. If the number of requests to the benchmark (from calls to `bm.get` and `bm.get_poi` methods) exceeds the specified budget, then `None` will be returned. If the flag `is_strict` is disabled, then the request for the last batch will be allowed, after which the budget will be exceeded, otherwise this last batch will not be considered. Note that when the budget is exceeded, `None` will be returned both when requesting a single value and a batch of values. Also, in a similar way, you can set a limit on the use of the cache by `m_cache` parameter.
 
-- `bm.set_constr(penalty=1.E+42, eps=1.E-16, with_amplitude=True)` - if the benchmark has a constraint, then using this function you can set a `penalty` (for the requested points that do not satisfy the constraint, the value `penalty * constraint_value` will be returned) and a `eps` (threshold value to check that the constraint has been fulfilled). Note that we set the constraints as a function (`bm.constr`) that returns the value `constraint_value` (amplitude) of the constraint, and if the constraint is met, then the value must be non-positive, otherwise, the objective function is not calculated and a value proportional to the amplitude of the constraint is returned (if you disable flag `with_amplitude`, then just the value of the penalty will be returned). For the case of maximization task you should set negative `penalty` value.
+- `bm.set_constr(penalty=1.E+42, eps=1.E-16, with_amplitude=True)` - if the benchmark has a constraint, then using this function you can set a `penalty` (for the requested points that do not satisfy the constraint, the value `penalty * constraint_value` will be returned) and a `eps` (threshold value to check that the constraint has been fulfilled). Note that we set the constraints as a function (`bm.constr` / `bm.constr_batch`) that returns the value `constraint_value` (amplitude) of the constraint, and if the constraint is met, then the value must be non-positive, otherwise, the objective function is not calculated and a value proportional to the amplitude of the constraint is returned (if you disable flag `with_amplitude`, then just the value of the penalty will be returned). For the case of maximization task you should set negative `penalty` value.
 
 - `bm.set_max(i=None, x=None, y=None)` - if necessary, you can manually set the multi-index, the corresponding continuous point (for benchmarks, which relate to functions of a continuous argument), and the corresponding value for the exact global maximum of the function. The corresponding values will be further available in the benchmark as `bm.i_max_real`, `bm.x_max_real` and `bm.y_max_real` respectively. When the benchmark is initialized, this function is called automatically if the optimum is known.
 
 - `bm.set_min(i=None, x=None, y=None)` - the same as in the previous point, but for the global minimum.
 
-- `bm.set_log(with_log=False, cond='min-max', step=1000, prefix='bm', with_min=True, with_max=True)` - when calling this function with the `True` argument `with_log`, the log will be printed while requests to benchmark. You may set the log codition `cond` (`min`, `max`, `min-max` or `step`; e.g., in the case `min` the log will be presented each time the `min` value is updated), the log step (for condition `step`) and a string `prefix` for the log. You can also disable the display of current minimum values (`with_min`) or maximum values (`with_max`) in the log string.
+- `bm.set_log(log=False, cond='min-max', step=1000, prefix='bm', with_min=True, with_max=True)` - when calling this function with the `True` argument `log`, the log will be printed while requests to benchmark. You may set the log codition `cond` (`min`, `max`, `min-max` or `step`; e.g., in the case `min` the log will be presented each time the `min` value is updated), the log step (for condition `step`) and a string `prefix` for the log. You can also disable the display of current minimum values (`with_min`) or maximum values (`with_max`) in the log string. Note that you can provide as `log` argument some print-like function, e.g., `log=print`, in this case, printing will occur not to the console, but to the corresponding function.
 
-- `bm.set_cache(with_cache=False, cache=None, m_max=1.E+8)` - when calling this function with the `True` argument `with_cache`, the cache will be used, that is, all the values requested from the benchmark will be saved and when the same multi-indices are accessed again, the values will be retrieved from the cache instead of explicitly calculating the objective function. Additionally, you can optionally pass as an argument `cache` an already existing cache in the form of a dictionary (the keys are multi-indices in the form of tuples, and the values are the corresponding values of the objective function). We especially note that the cache is only used when querying benchmark values in discrete multi-indices; for requested continuous points, no cache will be used. It is also important to note that no cache will be used for matching multi-indices in the same requested batch of values. Optionally, you can set `m_max` argument that specifies the maximum cache size. If the size is exceeded, the cache will be cleared and a corresponding warning will be displayed.
+- `bm.set_cache(with_cache=False, cache=None, m_max=1.E+8)` - when calling this function with the `True` argument `with_cache`, the cache will be used, that is, all the values requested from the benchmark will be saved and when the same multi-indices are accessed again, the values will be retrieved from the cache instead of explicitly calculating the objective function. Additionally, you can optionally pass as an argument `cache` an already existing cache in the form of a dictionary (the keys are multi-indices in the form of tuples, and the values are the corresponding values of the objective function). We especially note that the cache is only used when querying benchmark values in discrete multi-indices; for requested continuous points, no cache will be used. It is also important to note that no cache will be used for matching multi-indices in the same requested batch of values. Optionally, you can set `m_max` argument that specifies the maximum cache size. If the size is exceeded, the cache will be cleared and a corresponding warning will be displayed to the log. Note that when the `bm.init` method is called, the cache is always reset to zero.
 
 - `bm.set_opts(...)` - for some benchmarks, this function may be called to set additional benchmark-specific options (please see the description of arguments in the relevant benchmark code file).
 
+> You can get all configuration options as a dictionary by the function `bm.get_config()`.
+
 ##### Computing benchmark values
 
 Now the benchmark is ready to go, and we can calculate its value in any requested discrete multi-index (a real number will be returned) or a list of its values for any requested batch of discrete multi-indices (1D numpy array of real numbers will be returned):
 ```python
 # Get value at multi-index i:
 i = np.ones(bm.d)
 print(bm[i]) # you can use the alias "bm.get(i)"
 
 # Get values for batch of multi-indices I:
 I = np.array([i, i+1, i+2])
 print(bm[I]) # you can use the alias "bm.get(I)"
 ```
 Note that the `get` method can be used instead of `[ ]` notation, for example, if it is necessary to pass somewhere a function that calculates benchmark values.
 
-Since the considered benchmark (`BmFuncAckley`) corresponds to a function of a continuous argument, above we calculated the values for the discretization of the function on a given grid. Additionally, we can calculate values at continuous points by analogy:
+Since the considered benchmark (`BmFuncAckley`) corresponds to a function of a continuous argument, above we calculated the values for the discretization of the function on a automatically selected grid. Additionally, we can calculate values at continuous points by analogy:
 ```python
 # Get value at point x:
 x = np.ones(bm.d) * 0.42
 print(bm(x)) # you can use the alias "bm.get_poi(x)"
 
 # Get values for batch of points X:
 X = np.array([x, x*0.3, x*1.1])
 print(bm(X)) # you can use the alias "bm.get_poi(X)"
 ```
 
-##### Data set generation
+##### Dataset generation
 
 For convenience, the benchmark also has functions that allow you to generate training and test data sets on a discrete grid:
 ```python
 # Generate random train dataset (from LHS):
 # I_trn is array of [500, bm.d] and y_trn is [500]
 I_trn, y_trn = bm.build_trn(500)
 
 # Generate random test dataset (from random choice):
 # I_tst is array of [100, bm.d] and y_tst of [100]
 I_tst, y_tst = bm.build_tst(100)
 ```
 
+> Note that, by default, the spent computational budget (see `bm.set_budget` function) and time spent does not change when the test dataset is generated (this is controlled by the default `skip_process` flag value in `bm.build_tst(m=0, skip_process=True)`), but is consumed when generating the training dataset (i.e., `bm.build_trn(m=0, skip_process=False)`).
+
 ##### Request history analysis
 
 During requests to the benchmark, that is, when calling functions `bm[]` (or `bm.get`), `bm()` (or `bm.get_poi`), `bm.build_trn` (if the flag `skip_process` is not set in the function arguments; it has a value `False` by default) and `bm.build_tst` (if `skip_process` is not set; it is `True` by default for this function), the following useful class parameters are updated:
 
 - `bm.m` - the total number of performed calculations of the benchmark value (if a cache is used, then the values taken from the cache are not taken into account in this variable).
 
 - `bm.m_cache` - the total number of cache hits performed instead of explicitly calculating benchmark values (if no cache is used, it is `0`).
 
 - `bm.time` - total time in seconds spent on calculating the benchmark values (the time spent on cache accesses is also taken into account).
 
+- `bm.time_full` - benchmark lifetime in seconds from the moment of initialization (i.e., the call to `bm.init` method).
+
 - `bm.y_list` - a list of all sequentially calculated benchmark values (results of cache accesses are also added to the list).
 
 - `bm.i_max`, `bm.x_max`, `bm.y_max` - a discrete multi-index, a continuous multi-dimensional point, and benchmark values corresponding to the maximum of all requested values. Note that for the case of a discrete function, the value of `x_max` will be `None`, and for the case of a continuous function, the values of `i_max` and `x_max` will correlate, while if requests were made for continuous points, then `x_max` will correspond to the exact position of the point, and `i_max` will be the nearest multi-index of the used discrete grid.
 
 - `bm.i_min`, `bm.x_min`, `bm.y_min` - same as in the previous point, but for the minimum value.
 
-The following function may be used to print the corresponding values: `print(bm.info_history())`.
+- `bm.i`, `bm.x`, `bm.y` - the last requested multi-index / point and the related computed benchmark's value.
+
+> The following function may be used to print the corresponding values: `print(bm.info_history())`. You can also get these values as a dictionary by the function `bm.get_history()`.
 
 ##### Notes
 
 - For some benchmarks (e.g., for all benchmarks from `agent` collection) the method `show` (present the current state, the state for provided input or the final state for the best found input) and `render` (present the animation for the current solution, the solution from the provided input or for the solution from the best found input) are available.
 
 
 ## Authors
```

### Comparing `teneva_bm-0.5.0/demo.py` & `teneva_bm-0.6.0/demo.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 """Demo script for teneva_bm.
 
 Call it as "python demo.py" to run demo for all existing benchmarks or as
 "python demo.py bm_<name_of_collection>_<name_of_benchmark>" to run an example
 for a specific benchmark "<name_of_benchmark>" from the collection (folder)
-"<name_of_collection" (e.g., "python demo.py bm_qubo_knap_amba"). Note that the
+"<name_of_collection" (e.g., "python demo.py bm_qubo_knap_det"). Note that the
 code for the demo run is at the end of the corresponding benchmark file in the
 section "if __name__ == '__main__':".
 
-You can also run this script as ""python demo.py info" to present only info
-about existing collections and benchmarks.
+You can also run this script as ""python demo.py info" to present only short
+info about all existing collections and benchmarks.
 
 """
 import sys
 
 
 from teneva_bm import teneva_bm_demo
 
 
 if __name__ == '__main__':
     bm_use = sys.argv[1] if len(sys.argv) > 1 else None
 
-    only_info = (bm_use == 'info')
-    bm_use = None if bm_use and bm_use.lower() == 'info' else bm_use
+    only_info = bm_use and bm_use.lower() == 'info'
+    bm_use = None if only_info else bm_use
 
     teneva_bm_demo(bm_use, with_info=(bm_use is None), all=(not only_info))
```

### Comparing `teneva_bm-0.5.0/setup.py` & `teneva_bm-0.6.0/setup.py`

 * *Files identical despite different names*

### Comparing `teneva_bm-0.5.0/teneva_bm/agent/agent.py` & `teneva_bm-0.6.0/teneva_bm/agent/agent.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,38 +1,49 @@
+import matplotlib.pyplot as plt
 import numpy as np
-import os
 
 
 try:
     import cv2
     with_cv2 = True
 except Exception as e:
     with_cv2 = False
 
 
 try:
     import gym
-    with_gym = True
+    gym.logger.set_level(40)
     np.bool8 = bool
+    from gym.envs.toy_text import frozen_lake as gym_frozen_lake
+    with_gym = True
 except Exception as e:
     with_gym = False
 
 
+import warnings
+warnings.filterwarnings('ignore', category=DeprecationWarning,
+    module=r"importlib\.")
+warnings.filterwarnings('ignore', category=DeprecationWarning,
+    module=r"ipkernel")
+
+
 from teneva_bm import Bm
 from teneva_bm.agent.policy import Policy
 from teneva_bm.agent.policy import PolicyToeplitz
 
 
 class Agent(Bm):
-    def env_build(name, **args):
+    def make(name, **args):
         if with_gym:
             return gym.make(name, render_mode='rgb_array', **args)
 
-    def __init__(self, d=None, n=32, name='Agent-abstract-class', desc='',
-                 steps=1000, policy_name='none'):
+    frozen_lake = gym_frozen_lake if with_gym else None
+
+    def __init__(self, d=None, n=3, name='Agent-abstract-class', desc='',
+                 steps=1000, policy='toeplitz'):
         super().__init__(None, None, name, desc)
         self._n_raw = n # We'll set it later in "prep_bm" method
 
         if not with_cv2:
             msg = 'Need "cv2" module. For installation please see README.md'
             self.set_err(msg)
 
@@ -41,168 +52,223 @@
             self.set_err(msg)
 
         if d is not None:
             msg = 'Dimension number (d) should not be set manually'
             self.set_err(msg)
 
         self._steps = steps
-        self._policy_name = policy_name
+
+        if isinstance(policy, str):
+            self._policy_name = policy
+
+            if self._policy_name == 'direct':
+                self._policy = Policy()
+            elif self._policy_name == 'toeplitz':
+                self._policy = PolicyToeplitz()
+            else:
+                raise ValueError('Invalid policy name')
+
+        else:
+            self._policy_name = policy.name
+
+            self._policy = policy
 
         self._with_render = False
 
     @property
     def identity(self):
-        return ['_policy_name', 'n', '_steps']
+        return ['_steps', '_policy_name', 'n']
 
     @property
     def is_func(self):
-        return self._policy.is_func
+        return True
 
     @property
     def is_opti_max(self):
         return True
 
     @property
+    def _d_ac(self):
+        return len(self._env.action_space.low)
+
+    @property
+    def _d_st(self):
+        return len(self._env.observation_space.low)
+
+    @property
+    def _a_ac(self):
+        return np.array(self._env.action_space.low)
+
+    @property
+    def _a_st(self):
+        return np.array(self._env.observation_space.low)
+
+    @property
+    def _b_ac(self):
+        return np.array(self._env.action_space.high)
+
+    @property
+    def _b_st(self):
+        return np.array(self._env.observation_space.high)
+
+    @property
+    def _n_ac(self):
+        return None
+
+    @property
+    def _n_st(self):
+        return None
+
+    @property
     def _reward(self):
+        return self._rewards[-1] if len(self._rewards) else 0.
+
+    @property
+    def _reward_total(self):
         return np.sum(np.array(self._rewards)) if len(self._rewards) else 0.
 
     @property
     def _state(self):
-        return (self._states[-1] if len(self._states) else self._state0).copy()
+        return self._states[-1] if len(self._states) else self._state0
 
     def get_config(self):
         conf = super().get_config()
         conf['_steps'] = self._steps
         conf['_policy_name'] = self._policy_name
+        conf['_d_st'] = self._d_st
+        conf['_d_ac'] = self._d_ac
         return conf
 
     def info(self, footer=''):
         text = ''
 
-        text += 'Dimension of state space for agent       : '
-        v = self._d_st
-        text += f'{v}\n'
-
-        text += 'Dimension of action space for agent      : '
-        v = self._d_ac
-        text += f'{v}\n'
-
         text += 'Number of agent steps                    : '
         v = self._steps
         text += f'{v}\n'
 
         text += 'Used policy                              : '
         v = self._policy_name
         text += f'{v}\n'
 
+        text += 'Dimension of state space for agent       : '
+        v = self._d_st
+        text += f'{v}\n'
+
+        text += 'Dimension of action space for agent      : '
+        v = self._d_ac
+        text += f'{v}\n'
+
         return super().info(text+footer)
 
-    def prep_bm(self, env, policy=None, d_st=None, d_ac=None):
+    def prep_bm(self, env):
         if env is None:
             raise ValueError('Environment is not set')
         self._env = env
 
-        if d_st:
-            self._d_st = d_st
-            self._a_st = None
-            self._b_st = None
-        else:
-            self._d_st = len(self._env.observation_space.low)
-            self._a_st = list(self._env.observation_space.low)
-            self._b_st = list(self._env.observation_space.high)
-
-        if d_ac:
-            self._d_ac = d_ac
-            self._a_ac = None
-            self._b_ac = None
-        else:
-            self._d_ac = len(self._env.action_space.low)
-            self._a_ac = list(self._env.action_space.low)
-            self._b_ac = list(self._env.action_space.high)
-
-        if policy is not None:
-            self._policy = policy
-        elif self._policy_name == 'none':
-            self._policy = Policy(self._d_st, self._d_ac, self._steps)
-        elif self._policy_name == 'toeplitz':
-            self._policy = PolicyToeplitz(self._d_st, self._d_ac, self._steps)
-        else:
-            raise ValueError('Policy is not set')
-
-        self.set_size(self._policy.d, self._n_raw)
-        if self.is_func: # TODO !!!
-            self.set_grid(self._a_ac*self._steps, self._b_ac*self._steps)
-
+        self._policy.prep(self._steps,
+            self._d_st, self._n_st, self._a_st, self._b_st,
+            self._d_ac, self._n_ac, self._a_ac, self._b_ac)
+
+        self.set_dimension(self._policy.d)
+        self.set_size(self._n_raw)
+        if self.is_func:
+            self.set_grid(self._policy.a, self._policy.b)
         self._reset()
 
-    def render(self, fpath=None, i=None, best=True):
+    def render(self, fpath=None, i=None, best=True, fps=20.):
         self._with_render = True
         i, y = self.get_solution(i, best)
         self._with_render = False
 
         frames = self._frames
         frames = [cv2.cvtColor(frame, cv2.COLOR_RGB2BGR) for frame in frames]
         # frame = cv2.resize(frame,(512, 512))
 
         fpath = self.path_build(fpath, 'mp4')
         fourcc = cv2.VideoWriter_fourcc(*'mp4v')
-        out = cv2.VideoWriter(fpath, fourcc, 20.0, (frames[0].shape[:2]))
+        out = cv2.VideoWriter(fpath, fourcc, fps, (frames[0].shape[:2]))
         for frame in frames:
             out.write(frame)
         out.release()
 
+    def show(self, fpath=None, i=None, best=True):
+        i, y = self.get_solution(i, best)
+
+        try:
+            frame = self._env.render()
+        except Exception as e:
+            self._wrn('Can not render agent for image generation')
+
+        plt.imshow(frame)
+        plt.axis('off')
+
+        fpath = self.path_build(fpath, 'png')
+        plt.savefig(fpath, bbox_inches='tight') if fpath else plt.show()
+
     def target(self, params):
         self._policy.set(params)
         self._run()
-        return self._reward
+        return self._reward_total
 
-    def _gen_state0(self):
-        return np.zeros(self._d_st)
+    def _parse_action(self, action):
+        return action
+
+    def _parse_action_gym(self, action):
+        return action
+
+    def _parse_reward(self, reward):
+        return reward
 
     def _parse_state(self, state):
         return state
 
-    def _parse_reward(self, reward=0.):
-        return reward
+    def _parse_state_policy(self, state):
+        return state
 
-    def _reset(self, state0=None):
-        self._actions = []
-        self._frames = []
-        self._rewards = []
-        self._states = []
+    def _reset(self):
+        self._policy.reset()
+
+        state, info = self._env.reset(seed=self.seed)
 
         self._step = 0
-        self._state0 = self._gen_state0() if state0 is None else state0
-        self._state_prev = None
+        self._state0 = self._parse_state(state)
         self._done = False
 
-        __state, __info = self._env.reset(seed=self.seed)
-        self._set_state(self._state0)
+        self._actions = []
+        self._frames = []
+        self._rewards = []
+        self._states = []
 
     def _run(self):
         self._reset()
 
+        if self._with_render:
+            try:
+                self._frames.append(self._env.render())
+            except Exception as e:
+                self._wrn('Can not render agent for video generation')
+
         for step in range(self._steps):
             self._step = step
-            self._state_prev = self._state.copy()
 
-            action = self._policy(self._state, step)
-            if len(action) == 1:
-                action = action[0]
+            state = self._parse_state_policy(self._state)
+            action = self._policy(state)
+            action = self._parse_action(action)
+            self._actions.append(action)
 
-            state, reward, self._done = self._env.step(action)[:3]
+            action_gym = self._parse_action_gym(action)
+            state, reward, self._done = self._env.step(action_gym)[:3]
 
-            self._actions.append(action)
-            self._rewards.append(self._parse_reward(reward))
-            self._states.append(self._parse_state(state))
+            state = self._parse_state(state)
+            self._states.append(state)
+
+            reward = self._parse_reward(reward)
+            self._rewards.append(reward)
 
             if self._with_render:
                 try:
                     self._frames.append(self._env.render())
                 except Exception as e:
                     self._wrn('Can not render agent for video generation')
 
             if self._done:
                 break
-
-    def _set_state(self, state):
-        return
```

### Comparing `teneva_bm-0.5.0/teneva_bm/agent/bm_agent_ant.py` & `teneva_bm-0.6.0/teneva_bm/agent/bm_agent_ant.py`

 * *Files 26% similar despite different names*

```diff
@@ -2,62 +2,67 @@
 
 
 from teneva_bm.agent.agent import Agent
 
 
 
 DESC = """
-    Agent from myjoco environment "Ant". For details, see
+    Agent "Ant" from myjoco environment. For details, see
     https://mgoulao.github.io/gym-docs/environments/mujoco/ant/
-
-    By default ("policy_name" is 'none"), no policy is used. The Toeplitz
-    discrete policy may be also used (if "policy_name" is 'toeplitz"), see
-    https://github.com/jparkerholder/ASEBO/blob/master/asebo/policies.py
+    By default, the Toeplitz policy ("policy='toeplitz'") is used
+    (https://github.com/jparkerholder/ASEBO/blob/master/asebo/policies.py).
+    You can also set "direct" policy (direct optimization of agent's actions)
+    or own policy class instance (see "agent/policy.py" with a description of
+    the interface design details). The dimension is determined automatically
+    according to the properties of the agent and the used policy; the default
+    mode size is 3 and the number of agent's steps is 1000.
 """
 
 
 class BmAgentAnt(Agent):
-    def __init__(self, d=None, n=32, name='AgentAnt', desc=DESC,
-                 steps=1000, policy_name='none'):
-        super().__init__(d, n, name, desc, steps, policy_name)
-
-    def prep_bm(self, policy=None):
-        env = Agent.env_build('Ant-v4')
-        return super().prep_bm(env, policy)
-
-    def _set_state(self, state, x=0., y=0.):
-        return # TODO !!!
-        qpos = np.array([x, y] + list(state[:3]))
-        qvel = state[3:]
-        self._env.set_state(qpos, qvel)
+    def __init__(self, d=None, n=3, name='AgentAnt', desc=DESC,
+                 steps=1000, policy='toeplitz'):
+        super().__init__(d, n, name, desc, steps, policy)
+
+    def prep_bm(self):
+        env = Agent.make('Ant-v4')
+        return super().prep_bm(env)
 
 
 if __name__ == '__main__':
     np.random.seed(42)
 
-    bm = BmAgentAnt().prep()
+    bm = BmAgentAnt(steps=250).prep()
     print(bm.info())
 
     I_trn, y_trn = bm.build_trn(1.E+1)
     print(bm.info_history())
 
     text = 'Value at a random multi-index            :  '
     i = [np.random.choice(k) for k in bm.n]
     y = bm[i]
     text += f'{y:-10.3e}'
     print(text)
 
-    text = 'Generate video for a random multi-index  :  '
-    bm = BmAgentAnt(steps=200).prep()
+    text = 'Render for "direct" policy               :  '
+    bm = BmAgentAnt(steps=250, policy='direct').prep()
+    fpath = f'result/{bm.name}/render_direct'
     i = [np.random.choice(k) for k in bm.n]
     y = bm[i]
-    bm.render('result/BmAgentAnt_demo_none')
-    text += 'see "result/...demo_none.mp4'
+    bm.render(fpath)
+    text += f' see {fpath}'
     print(text)
 
-    text = 'Generate video for a random multi-index  :  '
-    bm = BmAgentAnt(steps=200, policy_name='toeplitz').prep()
+    text = 'Render for "toeplitz" policy             :  '
+    bm = BmAgentAnt(steps=250, policy='toeplitz').prep()
+    fpath = f'result/{bm.name}/render_toeplitz'
     i = [np.random.choice(k) for k in bm.n]
     y = bm[i]
-    bm.render('result/BmAgentAnt_demo_toeplitz')
-    text += 'see "result/...demo_toeplitz.mp4'
+    bm.render(fpath)
+    text += f' see {fpath}'
+    print(text)
+
+    text = 'Generate image for a random multi-index  :  '
+    fpath = f'result/{bm.name}/show'
+    bm.show(fpath)
+    text += f' see {fpath}'
     print(text)
```

### Comparing `teneva_bm-0.5.0/teneva_bm/agent/bm_agent_humanoid.py` & `teneva_bm-0.6.0/teneva_bm/agent/bm_agent_human.py`

 * *Files 20% similar despite different names*

```diff
@@ -2,62 +2,67 @@
 
 
 from teneva_bm.agent.agent import Agent
 
 
 
 DESC = """
-    Agent from myjoco environment "Humanoid". For details, see
-    https://mgoulao.github.io/gym-docs/environments/mujoco/humanoid/
-
-    By default ("policy_name" is 'none"), no policy is used. The Toeplitz
-    discrete policy may be also used (if "policy_name" is 'toeplitz"), see
-    https://github.com/jparkerholder/ASEBO/blob/master/asebo/policies.py
+    Agent "Humanoid" from myjoco environment. For details, see
+    https://mgoulao.github.io/gym-docs/environments/mujoco/Humanoid/
+    By default, the Toeplitz policy ("policy='toeplitz'") is used
+    (https://github.com/jparkerholder/ASEBO/blob/master/asebo/policies.py).
+    You can also set "direct" policy (direct optimization of agent's actions)
+    or own policy class instance (see "agent/policy.py" with a description of
+    the interface design details). The dimension is determined automatically
+    according to the properties of the agent and the used policy; the default
+    mode size is 3 and the number of agent's steps is 1000.
 """
 
 
-class BmAgentHumanoid(Agent):
-    def __init__(self, d=None, n=32, name='AgentHumanoid', desc=DESC,
-                 steps=1000, policy_name='none'):
-        super().__init__(d, n, name, desc, steps, policy_name)
-
-    def prep_bm(self, policy=None):
-        env = Agent.env_build('Humanoid-v4')
-        return super().prep_bm(env, policy)
-
-    def _set_state(self, state, x=0., y=0.):
-        return # TODO !!!
-        qpos = np.array([x, y] + list(state[:3]))
-        qvel = state[3:]
-        self._env.set_state(qpos, qvel)
+class BmAgentHuman(Agent):
+    def __init__(self, d=None, n=3, name='AgentHuman', desc=DESC,
+                 steps=1000, policy='toeplitz'):
+        super().__init__(d, n, name, desc, steps, policy)
+
+    def prep_bm(self):
+        env = Agent.make('Humanoid-v4')
+        return super().prep_bm(env)
 
 
 if __name__ == '__main__':
     np.random.seed(42)
 
-    bm = BmAgentHumanoid().prep()
+    bm = BmAgentHuman().prep()
     print(bm.info())
 
     I_trn, y_trn = bm.build_trn(1.E+1)
     print(bm.info_history())
 
     text = 'Value at a random multi-index            :  '
     i = [np.random.choice(k) for k in bm.n]
     y = bm[i]
     text += f'{y:-10.3e}'
     print(text)
 
-    text = 'Generate video for a random multi-index  :  '
-    bm = BmAgentHumanoid(steps=200).prep()
+    text = 'Render for "direct" policy               :  '
+    bm = BmAgentHuman(steps=250, policy='direct').prep()
+    fpath = f'result/{bm.name}/render_direct'
     i = [np.random.choice(k) for k in bm.n]
     y = bm[i]
-    bm.render('result/BmAgentHumanoid_demo_none')
-    text += 'see "result/...demo_none.mp4'
+    bm.render(fpath)
+    text += f' see {fpath}'
     print(text)
 
-    text = 'Generate video for a random multi-index  :  '
-    bm = BmAgentHumanoid(steps=200, policy_name='toeplitz').prep()
+    text = 'Render for "toeplitz" policy             :  '
+    bm = BmAgentHuman(steps=250, policy='toeplitz').prep()
+    fpath = f'result/{bm.name}/render_toeplitz'
     i = [np.random.choice(k) for k in bm.n]
     y = bm[i]
-    bm.render('result/BmAgentHumanoid_demo_toeplitz')
-    text += 'see "result/...demo_toeplitz.mp4'
+    bm.render(fpath)
+    text += f' see {fpath}'
+    print(text)
+
+    text = 'Generate image for a random multi-index  :  '
+    fpath = f'result/{bm.name}/show'
+    bm.show(fpath)
+    text += f' see {fpath}'
     print(text)
```

### Comparing `teneva_bm-0.5.0/teneva_bm/agent/bm_agent_swimmer.py` & `teneva_bm-0.6.0/teneva_bm/agent/bm_agent_swimmer.py`

 * *Files 18% similar despite different names*

```diff
@@ -2,61 +2,73 @@
 
 
 from teneva_bm.agent.agent import Agent
 
 
 
 DESC = """
-    Agent from myjoco environment "Swimmer". For details, see
+    Agent "Swimmer" from myjoco environment. For details, see
     https://mgoulao.github.io/gym-docs/environments/mujoco/swimmer
-
-    By default ("policy_name" is 'none"), no policy is used. The Toeplitz
-    discrete policy may be also used (if "policy_name" is 'toeplitz"), see
-    https://github.com/jparkerholder/ASEBO/blob/master/asebo/policies.py
+    By default, the Toeplitz policy ("policy='toeplitz'") is used
+    (https://github.com/jparkerholder/ASEBO/blob/master/asebo/policies.py).
+    You can also set "direct" policy (direct optimization of agent's actions)
+    or own policy class instance (see "agent/policy.py" with a description of
+    the interface design details). The dimension is determined automatically
+    according to the properties of the agent and the used policy; the default
+    mode size is 3 and the number of agent's steps is 1000.
 """
 
 
 class BmAgentSwimmer(Agent):
-    def __init__(self, d=None, n=32, name='AgentSwimmer', desc=DESC,
-                 steps=1000, policy_name='none'):
-        super().__init__(d, n, name, desc, steps, policy_name)
-
-    def prep_bm(self, policy=None):
-        env = Agent.env_build('Swimmer-v4')
-        return super().prep_bm(env, policy)
+    def __init__(self, d=None, n=3, name='AgentSwimmer', desc=DESC,
+                 steps=1000, policy='toeplitz'):
+        super().__init__(d, n, name, desc, steps, policy)
+
+    def prep_bm(self):
+        env = Agent.make('Swimmer-v4')
+        return super().prep_bm(env)
 
-    def _set_state(self, state, x=0., y=0.):
+    def _tmp_set_state(self, state, x=0., y=0.):
+        # Draft
         qpos = np.array([x, y] + list(state[:3]))
         qvel = state[3:]
         self._env.set_state(qpos, qvel)
 
 
 if __name__ == '__main__':
     np.random.seed(42)
 
-    bm = BmAgentSwimmer().prep()
+    bm = BmAgentSwimmer(steps=250).prep()
     print(bm.info())
 
     I_trn, y_trn = bm.build_trn(1.E+1)
     print(bm.info_history())
 
     text = 'Value at a random multi-index            :  '
     i = [np.random.choice(k) for k in bm.n]
     y = bm[i]
     text += f'{y:-10.3e}'
     print(text)
 
-    text = 'Generate video for a random multi-index  :  '
-    bm = BmAgentSwimmer(steps=200).prep()
+    text = 'Render for "direct" policy               :  '
+    bm = BmAgentSwimmer(steps=250, policy='direct').prep()
+    fpath = f'result/{bm.name}/render_direct'
     i = [np.random.choice(k) for k in bm.n]
     y = bm[i]
-    bm.render('result/BmAgentSwimmer_demo_none')
-    text += 'see "result/...demo_none.mp4'
+    bm.render(fpath)
+    text += f' see {fpath}'
     print(text)
 
-    text = 'Generate video for a random multi-index  :  '
-    bm = BmAgentSwimmer(steps=200, policy_name='toeplitz').prep()
+    text = 'Render for "toeplitz" policy             :  '
+    bm = BmAgentSwimmer(steps=250, policy='toeplitz').prep()
+    fpath = f'result/{bm.name}/render_toeplitz'
     i = [np.random.choice(k) for k in bm.n]
     y = bm[i]
-    bm.render('result/BmAgentSwimmer_demo_toeplitz')
-    text += 'see "result/...demo_toeplitz.mp4'
+    bm.render(fpath)
+    text += f' see {fpath}'
+    print(text)
+
+    text = 'Generate image for a random multi-index  :  '
+    fpath = f'result/{bm.name}/show'
+    bm.show(fpath)
+    text += f' see {fpath}'
     print(text)
```

### Comparing `teneva_bm-0.5.0/teneva_bm/bm.py` & `teneva_bm-0.6.0/teneva_bm/bm.py`

 * *Files 6% similar despite different names*

```diff
@@ -7,55 +7,56 @@
 from teneva_bm import __version__
 
 
 class Bm:
     def __init__(self, d=None, n=None, name='', desc=''):
         self.init()
 
+        self.set_log()
+
         self.set_seed()
 
-        self.set_size(d, n)
+        self.set_dimension(d)
+        self.set_size(n)
         self.set_constr()
 
         self.set_grid()
         self.set_grid_kind()
 
         self.set_name(name)
         self.set_desc(desc)
 
         self.set_opts()
         self.set_cache()
         self.set_budget()
 
-        self.set_min()
         self.set_max()
-
-        self.set_log()
+        self.set_min()
 
     def __call__(self, X):
         """Return a value or batch of values for provided x-point."""
         return self.get_poi(X)
 
     def __getitem__(self, I):
         """Return a value or batch of values for provided multi-index."""
         return self.get(I)
 
     @property
     def a0(self):
         """Return the lower grid size float value if it is constant."""
         if not self.is_a_equal:
             raise ValueError('Lower grid size is not constant, can`t get a0')
-        return self.a[0]
+        return self.a[0] if self.a is not None else None
 
     @property
     def b0(self):
         """Return the upper grid size float value if it is constant."""
         if not self.is_b_equal:
             raise ValueError('Upper grid size is not constant, can`t get b0')
-        return self.b[0]
+        return self.b[0] if self.b is not None else None
 
     @property
     def identity(self):
         """Returns a list of parameter names that define the benchmark."""
         return ['d', 'n']
 
     @property
@@ -107,15 +108,15 @@
         return not self.is_func
 
     @property
     def n0(self):
         """Return the mode size int value if it is constant."""
         if not self.is_n_equal:
             raise ValueError('Mode size is not constant, can`t get n0')
-        return self.n[0]
+        return self.n[0] if self.n is not None else None
 
     @property
     def time_full(self):
         """Full time of benchmark existence in seconds."""
         return tpc() - self.time_stamp_start
 
     @property
@@ -144,41 +145,57 @@
         return self.cores(X)
 
     def build_trn(self, m=0, skip_process=False):
         """Generate random (from LHS) train dataset of (index, value)."""
         if m < 1:
             return None, None
 
-        I_trn = self.sample_lhs(m)
+        I_trn = teneva.sample_lhs(self.n, m, seed=self.rand)
         y_trn = self.get(I_trn, skip_process)
 
         if y_trn is None:
             raise ValueError('The specified budget is exceeded')
 
         return I_trn, y_trn
 
     def build_tst(self, m=0, skip_process=True):
         """Generate random (from "choice") test dataset of (index, value)."""
         if m < 1:
             return None, None
 
-        I_tst = self.sample_random(m)
+        I_tst = teneva.sample_random(self.n, m, seed=self.rand)
         y_tst = self.get(I_tst, skip_process)
 
         if y_tst is None:
             raise ValueError('The specified budget is exceeded')
 
         return I_tst, y_tst
 
     def check(self):
         """Check that benchmark's configuration is valid."""
         if not self.is_prep:
             msg = 'Run "prep" method for BM before call it'
             self.set_err(msg)
 
+        if self.d is None:
+            msg = 'Dimension "d" should be set'
+            self.set_err(msg)
+
+        if self.n is None:
+            msg = 'Mode size "n" should be set'
+            self.set_err(msg)
+
+        if self.is_func and self.a is None:
+            msg = 'Lower grid limit "a" should be set for continuous function'
+            self.set_err(msg)
+
+        if self.is_func and self.b is None:
+            msg = 'Lower grid limit "b" should be set for continuous function'
+            self.set_err(msg)
+
         return self.check_err()
 
     def check_err(self):
         """Check that benchmark has not errors."""
         if len(self.err):
             msg = f'BM "{self.name}" is not ready'
             for e in self.err:
@@ -237,55 +254,55 @@
 
         return Y
 
     def cores_mul(self, X):
         """Helper function for the construction of the TT-cores."""
         return [x[None, :, None] for x in X]
 
-    def get(self, I, skip_process=False):
+    def get(self, I, skip_process=False, skip_cache=False):
         """Return a value or batch of values for provided multi-index."""
         t = tpc()
 
         self.check()
 
         I, X, is_batch = self.parse_input(I=I)
 
-        if self.with_cache:
+        if self.with_cache and not skip_cache:
             m = I.shape[0]
             ind = [k for k in range(m) if tuple(I[k]) not in self.cache]
 
             m_new = len(ind)
             dm_cache = m - m_new
 
             if self.budget_m_cache:
                 if self.budget_is_strict:
                     if self.m_cache + dm_cache > self.budget_m_cache:
-                        return None
+                        return self.process_last()
                 else:
                     if self.m_cache > self.budget_m_cache:
-                        return None
+                        return self.process_last()
 
             if m_new > 0:
                 Z = X[ind] if self.is_func else I[ind]
                 y_new = self.compute(Z, skip_process)
                 if y_new is None:
-                    return None
+                    return self.process_last()
 
                 for k in range(m_new):
                     self.cache[tuple(I[ind[k]])] = y_new[k]
 
             y = np.array([self.cache[tuple(i)] for i in I])
 
         else:
             dm_cache = 0
 
             Z = X if self.is_func else I
             y = self.compute(Z, skip_process)
             if y is None:
-                return None
+                return self.process_last()
 
         return self.process(I, X, y, dm_cache, t, is_batch, skip_process)
 
     def get_config(self):
         """Return a dict with configuration of the benchmark."""
         conf = {
             'd': self.d,
@@ -335,21 +352,21 @@
         return conf
 
     def get_history(self):
         """Return a dict with results of requests to the benchmark."""
         hist = {
             'm': self.m,
             'm_cache': self.m_cache,
-            'i_max': self.i_max,
-            'x_max': self.x_max,
+            'i_max': self.list_copy(self.i_max, 'int'),
+            'x_max': self.list_copy(self.x_max, 'float'),
             'y_max': self.y_max,
-            'i_min': self.i_min,
-            'x_min': self.x_min,
+            'i_min': self.list_copy(self.i_min, 'int'),
+            'x_min': self.list_copy(self.x_min, 'float'),
             'y_min': self.y_min,
-            'y_list': self.y_list,
+            'y_list': self.list_copy(self.y_list, 'float'),
             'time': self.time,
             'time_full': self.time_full,
             'err': '; '.join(self.err) if len(self.err) else '',
         }
 
         return hist
 
@@ -360,29 +377,29 @@
                 i = self.i_max if self.is_opti_max else self.i_min
             else:
                 i = self.i
 
         if i is None:
             raise ValueError('Input is not set')
 
-        y = self.get(i, skip_process=True)
+        y = self.get(i, skip_process=True, skip_cache=True)
 
         return i, y
 
     def get_poi(self, X, skip_process=False):
         """Return a value or batch of values for provided x-point."""
         t = tpc()
 
         self.check()
 
         I, X, is_batch = self.parse_input(X=X)
 
         y = self.compute(X, skip_process)
         if y is None:
-            return None
+            return self.process_last()
 
         return self.process(I, X, y, 0, t, is_batch, skip_process)
 
     def info(self, footer=''):
         """Returns a detailed description of the benchmark as text."""
         text = '-' * 78 + '\n' + 'BM: '
         text += self.name + ' ' * max(0, 36-len(self.name)) +  ' | '
@@ -531,14 +548,40 @@
             text += '>               Options'
             text += '\n'
             text += footer
 
         text += '=' * 78 + '\n'
         return text
 
+    def info_current(self, footer=''):
+        text = ''
+
+        if self.log_prefix:
+            text += self.log_prefix + ' > '
+
+        text += f'm {self.m:-7.1e}'
+        if self.with_cache:
+            text += f' [+ {self.m_cache:-7.1e}]'
+        text += ' | '
+
+        text += f't {self.time_full:-7.1e} | '
+
+        if self.log_with_min and self.y_min is not None:
+            text += f'min {self.y_min:-10.3e} | '
+
+        if self.log_with_max and self.y_max is not None:
+            text += f'max {self.y_max:-10.3e} | '
+
+        if footer:
+            text = text + footer
+
+        self.log_m_last = self.m
+
+        return text
+
     def info_history(self, footer=''):
         """Returns an information about the request history (text)."""
         text = ''
 
         text = '-' * 78 + '\n' + 'BM: '
         text += self.name + ' ' * max(0, 36-len(self.name)) +  ' | '
         text += f'DIMS = {self.d:-4d} | '
@@ -595,15 +638,14 @@
 
         text += '=' * 78 + '\n'
         return text
 
     def init(self):
         self.err = []
 
-        # Last solution:
         self.i = None
         self.x = None
         self.y = None
 
         self.is_y_max_new = False
         self.i_max = None
         self.x_max = None
@@ -618,67 +660,61 @@
 
         self.m = 0
         self.m_cache = 0
         self.time = 0.
 
         self.log_m_last = 0
 
-        self.is_prep = False
-
         self.time_stamp_start = tpc()
 
+        self.cache = {}
+
+        self.is_prep = False
+
     def list_convert(self, x, kind='float', eps=1.E-16):
         """Convert list of equal values to one number and back."""
         if x is None:
             return None
 
         if kind == 'int':
             if isinstance(x, (int, float)):
                 return np.array([x]*self.d, dtype=int)
-            return int(x[0]) if len(set(x))==1 else np.asanyarray(x, dtype=int)
+
+            if len(set(x)) == 1:
+                return int(x[0])
+            else:
+                return self.list_copy(x, 'int')
 
         elif kind == 'float':
             if isinstance(x, (int, float)):
                 return np.array([x]*self.d, dtype=float)
             for v in x:
                 if np.abs(v - x[0]) > eps:
-                    return np.asanyarray(x, dtype=float)
+                    return self.list_copy(x, 'float')
             return float(x[0])
 
         else:
             raise ValueError('Unsupported kind for list conversion')
 
-    def log(self, postfix='', out=False):
-        text = ''
-
-        if self.log_prefix:
-            text += self.log_prefix + ' > '
-
-        text += f'm {self.m:-7.1e}'
-        if self.with_cache:
-            text += f' [+ {self.m_cache:-7.1e}]'
-        text += ' | '
-
-        text += f't {self.time_full:-7.1e} | '
-
-        if self.log_with_min and self.y_min is not None:
-            text += f'min {self.y_min:-10.3e} | '
-
-        if self.log_with_max and self.y_max is not None:
-            text += f'max {self.y_max:-10.3e} | '
-
-        if postfix:
-            text = text + postfix
-
-        if out:
-            print(text)
+    def list_copy(self, x, kind=None):
+        """Copy list or array and return the new array."""
+        if x is None:
+            return None
 
-        self.log_m_last = self.m
+        if kind:
+            if kind == 'int':
+                x = np.asanyarray(x, dtype=int)
+            elif kind == 'float':
+                x = np.asanyarray(x, dtype=float)
+            else:
+                raise ValueError('Unsupported kind for list copy')
+        else:
+            x = np.asanyarray(x)
 
-        return text
+        return x.copy()
 
     def log_check(self):
         if not self.with_log:
             return False
 
         if self.log_cond == 'min':
             return self.is_y_min_new
@@ -761,92 +797,54 @@
         self.i = I[-1, :].copy() if I is not None else None
         self.x = X[-1, :].copy() if X is not None else None
         self.y = y[-1]
 
         ind = np.argmax(y)
         if self.y_max is None or self.y_max < y[ind]:
             self.is_y_max_new = True
-            self.i_max = I[ind, :] if I is not None else None
-            self.x_max = X[ind, :] if X is not None else None
+            self.i_max = I[ind, :].copy() if I is not None else None
+            self.x_max = X[ind, :].copy() if X is not None else None
             self.y_max = y[ind]
         else:
             self.is_y_max_new = False
 
 
         ind = np.argmin(y)
         if self.y_min is None or self.y_min > y[ind]:
             self.is_y_min_new = True
-            self.i_min = I[ind, :] if I is not None else None
-            self.x_min = X[ind, :] if X is not None else None
+            self.i_min = I[ind, :].copy() if I is not None else None
+            self.x_min = X[ind, :].copy() if X is not None else None
             self.y_min = y[ind]
         else:
             self.is_y_min_new = False
 
         if self.log_check():
-            print(self.log())
+            self.log(self.info_current())
 
         if self.cache_m_max and len(self.cache.keys()) > self.cache_m_max:
             self.cache = {}
             self.wrn('The maximum cache size has been exceeded. Cache cleared')
 
         return y if is_batch else y[0]
 
+    def process_last(self):
+        if self.with_log:
+            self.log(self.info_current('<<< DONE\n'))
+
     def recover(self, i=None, best=True):
         """Restores some benchmark-specific values."""
         raise NotImplementedError
         i, y = self.get_solution(i, best)
 
     def render(self, fpath=None, i=None, best=True):
         """Render the solution for benchmark."""
         raise NotImplementedError
         i, y = self.get_solution(i, best)
         fpath = self.path_build(fpath)
 
-    def sample_lhs(self, m):
-        """Generate LHS smaples (multi-indices).
-
-        Args:
-            m (int, float): number of samples.
-
-        Returns:
-            np.ndarray: generated multi-indices for the tensor in the form of
-            array of the shape [m, d], where d is the dimension of the tensor.
-
-        """
-        d = self.d
-        n = self.n
-        m = int(m)
-
-        I = np.empty((m, d), dtype=int)
-        for i, k in enumerate(n):
-            I1 = np.repeat(np.arange(k), m // k)
-            I2 = self.rand.choice(np.arange(k), m-len(I1), replace=False)
-            I[:, i] = np.concatenate([I1, I2])
-            self.rand.shuffle(I[:, i])
-
-        return I
-
-    def sample_random(self, m):
-        """Generate random smaples (multi-indices).
-
-        Args:
-            m (int, float): number of samples.
-
-        Returns:
-            np.ndarray: generated multi-indices for the tensor in the form of
-            array of the shape [m, d], where d is the dimension of the tensor.
-
-        """
-        n = self.n
-        m = int(m)
-
-        I = np.vstack([self.rand.choice(np.arange(k), m) for k in n]).T
-
-        return I
-
     def set_budget(self, m=None, m_cache=None, is_strict=True):
         """Set computation buget."""
         self.budget_m = int(m) if m else None
         self.budget_m_cache = int(m_cache) if m_cache else None
         self.budget_is_strict = is_strict
 
     def set_cache(self, with_cache=False, cache=None, m_max=1.E+8):
@@ -858,110 +856,191 @@
     def set_constr(self, penalty=1.E+42, eps=1.E-16, with_amplitude=True):
         """Set constraint options."""
         self.constr_penalty = penalty
         self.constr_eps = eps
         self.constr_with_amplitude = with_amplitude
 
     def set_desc(self, desc=''):
-        """Set text description of the problem."""
+        """Set text description of the benchmark."""
         self.desc = desc
 
+    def set_dimension(self, d=None):
+        """Set dimension (d)."""
+        self.d = None if d is None else int(d)
+
+        if getattr(self, 'n', None) is not None:
+            raise ValueError('Dimension shanged but "n" already set')
+        if getattr(self, 'a', None) is not None:
+            raise ValueError('Dimension shanged but "a" already set')
+        if getattr(self, 'b', None) is not None:
+            raise ValueError('Dimension shanged but "b" already set')
+
     def set_err(self, err=''):
         """Set the error text (can not import external module, etc.)."""
         self.err.append(err)
 
     def set_grid(self, a=None, b=None):
         """Set grid lower (a) and upper (b) limits for the function-like BM."""
         if (a is not None or b is not None) and not self.d:
             raise ValueError('Please, set dimension "d" before')
 
         self.a = teneva.grid_prep_opt(a, self.d)
         self.b = teneva.grid_prep_opt(b, self.d)
 
+        if self.a is not None and self.b is not None:
+            for k in range(self.d):
+                if self.a[k] >= self.b[k]:
+                    raise ValueError('Invalid grid limits (a >= b)')
+
     def set_grid_kind(self, kind='cheb'):
         """Set the kind of the grid ('cheb' or 'uni').
 
         Note:
             In some benchmarks, when setting the exact global optimum, it is
             used that the central multi-index for a grid with an odd number of
             nodes lies at the origin. When new types of grids appear, it should
             be taken into account.
 
         """
-        self.grid_kind = kind
-
-        if not self.grid_kind in ['uni', 'cheb']:
+        if not kind in ['uni', 'cheb']:
             msg = f'Invalid kind of the grid (should be "uni" or "cheb")'
             raise ValueError(msg)
 
-    def set_log(self, with_log=False, cond='min-max', step=1000, prefix='bm',
-                with_min=True, with_max=True):
-        """Set the log options."""
-        self.with_log = with_log
+        self.grid_kind = kind
+
+    def set_log(self, log=False, cond='min-max', step=1000, prefix='bm',
+                with_min=True, with_max=True, log_wrn=None):
+        """Set the log options. The "log" may be bool or print-like function."""
+        if log:
+            self.with_log = True
+            self.log = print if isinstance(log, bool) else log
+        else:
+            self.with_log = False
+            self.log = lambda text: None
+
+        if log_wrn:
+            self.log_wrn = log_wrn
+        else:
+            self.log_wrn = print
+
+        if not cond in ['min', 'max', 'min-max', 'step']:
+            raise ValueError(f'Invalid "log_cond" argument "{cond}"')
+
         self.log_cond = cond
         self.log_step = int(step) if step else None
         self.log_prefix = prefix
         self.log_with_min = with_min
         self.log_with_max = with_max
 
-        if not self.log_cond in ['min', 'max', 'min-max', 'step']:
-            raise ValueError(f'Invalid "log_cond" argument "{self.log_cond}"')
-
     def set_max(self, i=None, x=None, y=None):
         """Set exact (real) global maximum (index, point and related value)."""
         self.i_max_real = i
         self.x_max_real = x
         self.y_max_real = y
 
         if self.i_max_real is not None:
-            self.i_max_real = np.asanyarray(self.i_max_real, dtype=int)
+            self.i_max_real = self.list_copy(self.i_max_real, 'int')
         if self.x_max_real is not None:
-            self.x_max_real = np.asanyarray(self.x_max_real, dtype=float)
+            self.x_max_real = self.list_copy(self.x_max_real, 'float')
         if self.y_max_real is not None:
             self.y_max_real = float(self.y_max_real)
 
+        if self.i_max_real is not None:
+            if getattr(self, 'n', None) is None:
+                raise ValueError('Please set mode sizes before the max')
+
+            for k in range(self.d):
+                is_out_a = self.i_max_real[k] < 0
+                is_out_b = self.i_max_real[k] > self.n[k] - 1
+                if is_out_a or is_out_b:
+                    raise ValueError('The i_max is out of grid bounds')
+
+        if self.x_max_real is not None:
+            if not self.is_func:
+                raise ValueError('Can not set x_max for discrete function')
+            if getattr(self, 'a', None) is None:
+                raise ValueError('Please set lower grid limit before the max')
+            if getattr(self, 'b', None) is None:
+                raise ValueError('Please set upper grid limit before the max')
+
+            for k in range(self.d):
+                is_out_a = self.x_max_real[k] < self.a[k]
+                is_out_b = self.x_max_real[k] > self.b[k]
+                if is_out_a or is_out_b:
+                    raise ValueError('The x_max is out of grid bounds')
+
     def set_min(self, i=None, x=None, y=None):
         """Set exact (real) global minimum (index, point and related value)."""
         self.i_min_real = i
         self.x_min_real = x
         self.y_min_real = y
 
         if self.i_min_real is not None:
-            self.i_min_real = np.asanyarray(self.i_min_real, dtype=int)
+            self.i_min_real = self.list_copy(self.i_min_real, 'int')
         if self.x_min_real is not None:
-            self.x_min_real = np.asanyarray(self.x_min_real, dtype=float)
+            self.x_min_real = self.list_copy(self.x_min_real, 'float')
         if self.y_min_real is not None:
             self.y_min_real = float(self.y_min_real)
 
+        if self.i_min_real is not None:
+            if getattr(self, 'n', None) is None:
+                raise ValueError('Please set mode sizes before the min')
+
+            for k in range(self.d):
+                is_out_a = self.i_min_real[k] < 0
+                is_out_b = self.i_min_real[k] > self.n[k] - 1
+                if is_out_a or is_out_b:
+                    raise ValueError('The i_min is out of grid bounds')
+
+        if self.x_min_real is not None:
+            if not self.is_func:
+                raise ValueError('Can not set x_min for discrete function')
+            if getattr(self, 'a', None) is None:
+                raise ValueError('Please set lower grid limit before the min')
+            if getattr(self, 'b', None) is None:
+                raise ValueError('Please set upper grid limit before the min')
+
+            for k in range(self.d):
+                is_out_a = self.x_min_real[k] < self.a[k]
+                is_out_b = self.x_min_real[k] > self.b[k]
+                if is_out_a or is_out_b:
+                    raise ValueError('The x_min is out of grid bounds')
+
     def set_name(self, name=''):
-        """Set display name for the problem."""
+        """Set display name for the benchmark."""
         self.name = name
 
     def set_opts(self):
         """Set options specific to the benchmark."""
         return
 
     def set_seed(self, seed=42):
+        """Set random seed and inner generator of random numbers."""
         self.seed = seed
         self.rand = np.random.default_rng(self.seed)
 
-    def set_size(self, d=None, n=None):
-        """Set dimension (d) and sizes for all d-modes (n: int or list)."""
-        self.d = None if d is None else int(d)
-
+    def set_size(self, n=None):
+        """Set sizes for all d-modes (n should be int or list)."""
         if n is not None and not self.d:
             raise ValueError('Please, set dimension "d" before')
 
         self.n = teneva.grid_prep_opt(n, self.d, int)
 
-    def shift_grid(self, scale=25):
+    def shift_grid(self, scale=100., sign=1):
         """Apply random shift for the grid limits."""
-        shift = self.rand.normal(size=self.d) / scale
-        self.a = self.a - (self.b-self.a) * shift
-        self.b = self.b + (self.b-self.a) * shift
+        if self.a is None or self.b is None:
+            raise ValueError('Please, set grid before')
+
+        rand = np.random.default_rng(42)
+
+        a_shift = rand.uniform(0, (self.b-self.a) / scale, size=self.d)
+        b_shift = rand.uniform(0, (self.b-self.a) / scale, size=self.d)
+
+        self.a = self.a + a_shift * sign
+        self.b = self.b - b_shift * sign
 
     def show(self, fpath=None, i=None, best=True):
         """Present the state of the benchmark (image, graph, etc.)."""
         raise NotImplementedError
         i, y = self.get_solution(i, best)
         fpath = self.path_build(fpath)
 
@@ -970,9 +1049,8 @@
         return self.target_batch(x.reshape(1, -1))[0]
 
     def target_batch(self, X):
         """Function that computes values for a given batch of points/indices."""
         return np.array([self.target(x) for x in X])
 
     def wrn(self, text):
-        text = '!!! BM-WARNING | ' + text
-        print(text)
+        self.log_wrn('!!! BM-WARNING | ' + text)
```

### Comparing `teneva_bm-0.5.0/teneva_bm/func/__init__.py` & `teneva_bm-0.6.0/teneva_bm/func/__init__.py`

 * *Files identical despite different names*

### Comparing `teneva_bm-0.5.0/teneva_bm/func/bm_func_ackley.py` & `teneva_bm-0.6.0/teneva_bm/func/bm_func_ackley.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,40 +2,36 @@
 
 
 from teneva_bm import Bm
 
 
 DESC = """
     Analytical Ackley function (continuous).
-    The dimension and mode size may be any (default are d=50, n=15).
-    Default grid limits are [-32.768, 32.768]; the exact global minimum
-    is known: x = [0, ..., 0], y = 0.
-    See https://www.sfu.ca/~ssurjano/ackley.html for details.
-    See also the work Momin Jamil, Xin-She Yang. "A literature survey of
+    The dimension and mode size may be any (default are d=7, n=16).
+    Default grid limits are [-32.768, 32.768] (with small random shift);
+    the exact global minimum is known: x = [0, ..., 0], y = 0.
+    See the work Momin Jamil, Xin-She Yang. "A literature survey of
     benchmark functions for global optimization problems". Journal of
     Mathematical Modelling and Numerical Optimisation 2013; 4:150-194
     ("1. Ackley 1 Function"; Continuous, Differentiable, Non-separable,
     Scalable, Multimodal).
+    See also https://www.sfu.ca/~ssurjano/ackley.html for details.
 """
 
 
 class BmFuncAckley(Bm):
-    def __init__(self, d=50, n=15, name='FuncAckley', desc=DESC):
+    def __init__(self, d=7, n=16, name='FuncAckley', desc=DESC):
         super().__init__(d, n, name, desc)
 
         self.set_grid(-32.768, +32.768)
         self.shift_grid()
 
         self.set_min(x=[0.]*self.d, y=0.)
 
     @property
-    def identity(self):
-        return super().identity + ['seed']
-
-    @property
     def is_func(self):
         return True
 
     def get_config(self):
         conf = super().get_config()
         conf['_a'] = self._a
         conf['_b'] = self._b
```

### Comparing `teneva_bm-0.5.0/teneva_bm/func/bm_func_alpine.py` & `teneva_bm-0.6.0/teneva_bm/func/bm_func_alpine.py`

 * *Files 8% similar despite different names*

```diff
@@ -3,41 +3,35 @@
 
 
 from teneva_bm import Bm
 
 
 DESC = """
     Analytical Alpine function (continuous).
-    The dimension and mode size may be any (default are d=50, n=15).
-    Default grid limits are [-10, 10]; the exact global minimum
-    is known: x = [0, ..., 0], y = 0.
+    The dimension and mode size may be any (default are d=7, n=16).
+    Default grid limits are [-10, 10] (with small random shift);
+    the exact global minimum is known: x = [0, ..., 0], y = 0.
     See the work Momin Jamil, Xin-She Yang. "A literature survey of
     benchmark functions for global optimization problems". Journal of
     Mathematical Modelling and Numerical Optimisation 2013; 4:150-194
     ("6. Alpine 1 Function"; Continuous, Non-Differentiable, Separable,
     Non-Scalable, Multimodal).
-    Note that the method "build_cores" for construction of the function
-    in the TT-format on the discrete grid is available.
 """
 
 
 class BmFuncAlpine(Bm):
-    def __init__(self, d=50, n=15, name='FuncAlpine', desc=DESC):
+    def __init__(self, d=7, n=16, name='FuncAlpine', desc=DESC):
         super().__init__(d, n, name, desc)
 
         self.set_grid(-10., +10.)
         self.shift_grid()
 
         self.set_min(x=[0.]*self.d, y=0.)
 
     @property
-    def identity(self):
-        return super().identity + ['seed']
-
-    @property
     def is_func(self):
         return True
 
     @property
     def with_cores(self):
         return True
```

### Comparing `teneva_bm-0.5.0/teneva_bm/func/bm_func_dixon.py` & `teneva_bm-0.6.0/teneva_bm/func/bm_func_dixon.py`

 * *Files 6% similar despite different names*

```diff
@@ -2,44 +2,41 @@
 
 
 from teneva_bm import Bm
 
 
 DESC = """
     Analytical Dixon function (continuous).
-    The dimension and mode size may be any (default are d=50, n=15).
-    Default grid limits are [-10, 10]; the exact global minimum
-    is known: x_i = 2^{(2^i-2) / 2^i} (i = 1, ..., d), y = 0.  Note that
-    this function achieves a global minimum at more than one point.
-    See https://www.sfu.ca/~ssurjano/dixonpr.html for details.
-    See also the work Momin Jamil, Xin-She Yang. "A literature survey of
+    The dimension and mode size may be any (default are d=7, n=16).
+    Default grid limits are [-10, 10] (with small random shift);
+    the exact global minimum is known: x_i = 2^{(2^i-2) / 2^i}
+    (i = 1, ..., d), y = 0;  note that this function achieves a global
+    minimum at more than one point.
+    See the work Momin Jamil, Xin-She Yang. "A literature survey of
     benchmark functions for global optimization problems". Journal of
     Mathematical Modelling and Numerical Optimisation 2013; 4:150-194
     ("48. Dixon & Price Function"; Continuous, Differentiable,
     Non-Separable, Scalable, Unimodal).
+    See also https://www.sfu.ca/~ssurjano/dixonpr.html for details.
 """
 
 
 class BmFuncDixon(Bm):
-    def __init__(self, d=50, n=15, name='FuncDixon', desc=DESC):
+    def __init__(self, d=7, n=16, name='FuncDixon', desc=DESC):
         super().__init__(d, n, name, desc)
 
         self.set_grid(-10., +10.)
         self.shift_grid()
 
         x_min = [1.]
-        for _ in range(d-1): # TODO: check this formula one more time:
+        for _ in range(d-1):
             x_min.append(np.sqrt(x_min[-1]/2.))
         self.set_min(x=np.array(x_min), y=0.)
 
     @property
-    def identity(self):
-        return super().identity + ['seed']
-
-    @property
     def is_func(self):
         return True
 
     def target_batch(self, X):
         y1 = (X[:, 0] - 1)**2
 
         y2 = np.arange(2, self.d+1) * (2. * X[:, 1:]**2 - X[:, :-1])**2
```

### Comparing `teneva_bm-0.5.0/teneva_bm/func/bm_func_exp.py` & `teneva_bm-0.6.0/teneva_bm/func/bm_func_qing.py`

 * *Files 10% similar despite different names*

```diff
@@ -2,66 +2,62 @@
 import teneva
 
 
 from teneva_bm import Bm
 
 
 DESC = """
-    Analytical Exponential function (continuous).
-    The dimension and mode size may be any (default are d=50, n=15).
-    Default grid limits are [-1, 1]; the exact global minimum
-    is known: x = [0, ..., 0], y = -1.
+    Analytical Qing function (continuous).
+    The dimension and mode size may be any (default are d=7, n=16).
+    Default grid limits are [0, 500] (with small random shift; note
+    also that we limit this function to this domain instead of often
+    used [-500, 500] to make sure it has a single global minimum);
+    the exact global minimum is known: x_i = \sqrt{i}, y = 0.
     See the work Momin Jamil, Xin-She Yang. "A literature survey of
     benchmark functions for global optimization problems". Journal of
     Mathematical Modelling and Numerical Optimisation 2013; 4:150-194
-    ("54. Exponential Function"; Continuous, Differentiable,
-    Non-Separable, Scalable, Multimodal).
-    Note that the method "build_cores" for construction of the function
-    in the TT-format on the discrete grid is available.
+    ("98. Qing Function"; Continuous, Differentiable, Separable
+    Scalable, Multimodal).
 """
 
 
-class BmFuncExp(Bm):
-    def __init__(self, d=50, n=15, name='FuncExp', desc=DESC):
+class BmFuncQing(Bm):
+    def __init__(self, d=7, n=16, name='FuncQing', desc=DESC):
         super().__init__(d, n, name, desc)
 
-        self.set_grid(-1., +1.)
-        self.shift_grid()
+        self.set_grid(0., +500.)
+        self.shift_grid(sign=-1)
 
-        self.set_min(x=[0.]*self.d, y=-1.)
-
-    @property
-    def identity(self):
-        return super().identity + ['seed']
+        self.set_min(x=np.sqrt(np.arange(1, self.d+1)), y=0.)
 
     @property
     def is_func(self):
         return True
 
     @property
     def with_cores(self):
         return True
 
     def cores(self, X):
-        Y = self.cores_mul([np.exp(-0.5 * x**2) for x in X.T])
-        Y[-1] *= -1.
-        return Y
+        return self.cores_add([(x**2 - i)**2 for i, x in enumerate(X.T, 1)])
 
     def target_batch(self, X):
-        return -np.exp(-0.5 * np.sum(X**2, axis=1))
+        return np.sum((X**2 - np.arange(1, self.d+1))**2, axis=1)
 
     def _target_pt(self, x):
         """Draft."""
-        return -torch.exp(-0.5 * torch.sum(x**2))
+        d = torch.tensor(self.d)
+
+        return torch.sum((x**2 - torch.arange(1, d+1))**2)
 
 
 if __name__ == '__main__':
     np.random.seed(42)
 
-    bm = BmFuncExp().prep()
+    bm = BmFuncQing().prep()
     print(bm.info())
 
     I_trn, y_trn = bm.build_trn(1.E+4)
     print(bm.info_history())
 
     text = 'Value at a random multi-index            :  '
     i = [np.random.choice(k) for k in bm.n]
```

### Comparing `teneva_bm-0.5.0/teneva_bm/func/bm_func_griewank.py` & `teneva_bm-0.6.0/teneva_bm/func/bm_func_griewank.py`

 * *Files 7% similar despite different names*

```diff
@@ -3,42 +3,36 @@
 
 
 from teneva_bm import Bm
 
 
 DESC = """
     Analytical Griewank function (continuous).
-    The dimension and mode size may be any (default are d=50, n=15).
-    Default grid limits are [-100, 100]; the exact global minimum
-    is known: x = [0, ..., 0], y = 0.
-    See https://www.sfu.ca/~ssurjano/griewank.html for details.
-    See also the work Momin Jamil, Xin-She Yang. "A literature survey of
+    The dimension and mode size may be any (default are d=7, n=16).
+    Default grid limits are [-100, 100] (with small random shift);
+    the exact global minimum is known: x = [0, ..., 0], y = 0.
+    See the the work Momin Jamil, Xin-She Yang. "A literature survey of
     benchmark functions for global optimization problems". Journal of
     Mathematical Modelling and Numerical Optimisation 2013; 4:150-194
     ("59. Griewank Function"; Continuous, Differentiable, Non-Separable,
     Scalable, Multimodal).
-    Note that the method "build_cores" for construction of the function
-    in the TT-format on the discrete grid is available.
+    See also https://www.sfu.ca/~ssurjano/griewank.html for details.
 """
 
 
 class BmFuncGriewank(Bm):
-    def __init__(self, d=50, n=15, name='FuncGriewank', desc=DESC):
+    def __init__(self, d=7, n=16, name='FuncGriewank', desc=DESC):
         super().__init__(d, n, name, desc)
 
         self.set_grid(-100., +100.)
         self.shift_grid()
 
         self.set_min(x=[0.]*self.d, y=0.)
 
     @property
-    def identity(self):
-        return super().identity + ['seed']
-
-    @property
     def is_func(self):
         return True
 
     @property
     def with_cores(self):
         return True
```

### Comparing `teneva_bm-0.5.0/teneva_bm/func/bm_func_michalewicz.py` & `teneva_bm-0.6.0/teneva_bm/func/bm_func_michalewicz.py`

 * *Files 6% similar despite different names*

```diff
@@ -3,47 +3,42 @@
 
 
 from teneva_bm import Bm
 
 
 DESC = """
     Analytical Michalewicz function (continuous).
-    The dimension and mode size may be any (default are d=50, n=15).
-    Default grid limits are [0, pi]; the exact global minimum is known
-    only for the case of dimensions 2, 5, and 10; in this cases, only the
-    corresponding value of the function is known, but not the argument.
-    See https://www.sfu.ca/~ssurjano/michal.html for details.
-    See also Charlie Vanaret, Jean-Baptiste Gotteland, Nicolas Durand,
+    The dimension and mode size may be any (default are d=7, n=16).
+    Default grid limits are [0, pi] (with small random shift);
+    the exact global minimum is known only for the case of dimensions 2, 5,
+    and 10; in this cases, only the corresponding value of the function is
+    known, but not the argument (except the 2D case).
+    See Charlie Vanaret, Jean-Baptiste Gotteland, Nicolas Durand,
     Jean-Marc Alliot. "Certified global minima for a benchmark of difficult
     optimization problems". arXiv preprint arXiv:2003.09867 2020
     (the function has d! local minima, and it is multimodal).
-    Note that the method "build_cores" for construction of the function
-    in the TT-format on the discrete grid is available.
+    See also https://www.sfu.ca/~ssurjano/michal.html for details.
 """
 
 
 class BmFuncMichalewicz(Bm):
-    def __init__(self, d=50, n=15, name='FuncMichalewicz', desc=DESC):
+    def __init__(self, d=7, n=16, name='FuncMichalewicz', desc=DESC):
         super().__init__(d, n, name, desc)
 
         self.set_grid(0., np.pi)
         self.shift_grid()
 
         if self.d == 2:
             self.set_min(x=[2.20, 1.57], y=-1.8013)
         if self.d == 5:
             self.set_min(y=-4.687658)
         if self.d == 10:
             self.set_min(y=-9.66015)
 
     @property
-    def identity(self):
-        return super().identity + ['seed']
-
-    @property
     def is_func(self):
         return True
 
     @property
     def with_cores(self):
         return True
 
@@ -119,7 +114,14 @@
     print(text)
 
     text = 'TT-cores accuracy on train data          :  '
     Y = bm.build_cores()
     e = teneva.accuracy_on_data(Y, I_trn, y_trn)
     text += f'{e:-10.1e}'
     print(text)
+
+    text = 'Value at the minimum (real vs calc) 2D   :  '
+    bm = BmFuncMichalewicz(d=2).prep()
+    y_real = bm.y_min_real
+    y_calc = bm(bm.x_min_real)
+    text += f'{y_real:-10.3e}       /      {y_calc:-10.3e}'
+    print(text)
```

### Comparing `teneva_bm-0.5.0/teneva_bm/func/bm_func_piston.py` & `teneva_bm-0.6.0/teneva_bm/func/bm_func_piston.py`

 * *Files 4% similar despite different names*

```diff
@@ -3,39 +3,35 @@
 
 
 from teneva_bm import Bm
 
 
 DESC = """
     Analytical Piston function (continuous).
-    The dimension is 7 and the mode size may be any (default is n=15),
-    each mode has its own (substantially different) limits.
+    The dimension is 7 and the mode size may be any (default is n=16), each
+    mode has its own different limits (with small random shift).
     See Vitaly Zankin, Gleb Ryzhakov, Ivan Oseledets. "Gradient descent
     based D-optimal design for the least-squares polynomial approximation".
     arXiv preprint arXiv:1806.06631 2018 for details.
 """
 
 
 class BmFuncPiston(Bm):
-    def __init__(self, d=7, n=15, name='FuncPiston', desc=DESC):
+    def __init__(self, d=7, n=16, name='FuncPiston', desc=DESC):
         super().__init__(d, n, name, desc)
 
         if self.d != 7:
             self.set_err('Dimension should be "7"')
 
         self.set_grid(
             [30., 0.005, 0.002, 1000,  90000, 290, 340],
             [60., 0.020, 0.010, 5000, 110000, 296, 360])
         self.shift_grid()
 
     @property
-    def identity(self):
-        return super().identity + ['seed']
-
-    @property
     def is_func(self):
         return True
 
     def target_batch(self, X):
         _M  = X[:, 0]
         _S  = X[:, 1]
         _V0 = X[:, 2]
```

### Comparing `teneva_bm-0.5.0/teneva_bm/func/bm_func_qing.py` & `teneva_bm-0.6.0/teneva_bm/func/bm_func_exp.py`

 * *Files 14% similar despite different names*

```diff
@@ -2,68 +2,60 @@
 import teneva
 
 
 from teneva_bm import Bm
 
 
 DESC = """
-    Analytical Qing function (continuous).
-    The dimension and mode size may be any (default are d=50, n=15).
-    Default grid limits are [0, 500] (note that we limit this function
-    to this domain instead of often used [-500, 500] to make sure it has
-    a single global minimum); the exact global minimum
-    is known: x_i = \sqrt{i} (i = 1, ..., d), y = 0.
+    Analytical Exponential function (continuous).
+    The dimension and mode size may be any (default are d=7, n=16).
+    Default grid limits are [-1, 1] (with small random shift);
+    the exact global minimum is known: x = [0, ..., 0], y = -1.
     See the work Momin Jamil, Xin-She Yang. "A literature survey of
     benchmark functions for global optimization problems". Journal of
     Mathematical Modelling and Numerical Optimisation 2013; 4:150-194
-    ("98. Qing Function"; Continuous, Differentiable, Separable
-    Scalable, Multimodal).
-    Note that the method "build_cores" for construction of the function
-    in the TT-format on the discrete grid is available.
+    ("54. Exponential Function"; Continuous, Differentiable,
+    Non-Separable, Scalable, Multimodal).
 """
 
 
-class BmFuncQing(Bm):
-    def __init__(self, d=50, n=15, name='FuncQing', desc=DESC):
+class BmFuncExp(Bm):
+    def __init__(self, d=7, n=16, name='FuncExp', desc=DESC):
         super().__init__(d, n, name, desc)
 
-        self.set_grid(0., +500.)
+        self.set_grid(-1., +1.)
         self.shift_grid()
 
-        self.set_min(x=np.sqrt(np.arange(1, self.d+1)), y=0.)
-
-    @property
-    def identity(self):
-        return super().identity + ['seed']
+        self.set_min(x=[0.]*self.d, y=-1.)
 
     @property
     def is_func(self):
         return True
 
     @property
     def with_cores(self):
         return True
 
     def cores(self, X):
-        return self.cores_add([(x**2 - i)**2 for i, x in enumerate(X.T, 1)])
+        Y = self.cores_mul([np.exp(-0.5 * x**2) for x in X.T])
+        Y[-1] *= -1.
+        return Y
 
     def target_batch(self, X):
-        return np.sum((X**2 - np.arange(1, self.d+1))**2, axis=1)
+        return -np.exp(-0.5 * np.sum(X**2, axis=1))
 
     def _target_pt(self, x):
         """Draft."""
-        d = torch.tensor(self.d)
-
-        return torch.sum((x**2 - torch.arange(1, d+1))**2)
+        return -torch.exp(-0.5 * torch.sum(x**2))
 
 
 if __name__ == '__main__':
     np.random.seed(42)
 
-    bm = BmFuncQing().prep()
+    bm = BmFuncExp().prep()
     print(bm.info())
 
     I_trn, y_trn = bm.build_trn(1.E+4)
     print(bm.info_history())
 
     text = 'Value at a random multi-index            :  '
     i = [np.random.choice(k) for k in bm.n]
```

### Comparing `teneva_bm-0.5.0/teneva_bm/func/bm_func_rastrigin.py` & `teneva_bm-0.6.0/teneva_bm/func/bm_func_rastrigin.py`

 * *Files 5% similar despite different names*

```diff
@@ -3,40 +3,34 @@
 
 
 from teneva_bm import Bm
 
 
 DESC = """
     Analytical Rastrigin function (continuous).
-    The dimension and mode size may be any (default are d=50, n=15).
-    Default grid limits are [-5.12, 5.12]; the exact global minimum
-    is known: x = [0, ..., 0], y = 0.
-    See https://www.sfu.ca/~ssurjano/rastr.html for details.
-    See also the work Johannes M Dieterich, Bernd Hartke. "Empirical review
+    The dimension and mode size may be any (default are d=7, n=16).
+    Default grid limits are [-5.12, 5.12] (with small random shift);
+    the exact global minimum is known: x = [0, ..., 0], y = 0.
+    See the work Johannes M Dieterich, Bernd Hartke. "Empirical review
     of standard benchmark functions using evolutionary global optimization".
     Applied Mathematics 2012; 3:1552-1564.
-    Note that the method "build_cores" for construction of the function
-    in the TT-format on the discrete grid is available.
+    See also https://www.sfu.ca/~ssurjano/rastr.html for details.
 """
 
 
 class BmFuncRastrigin(Bm):
-    def __init__(self, d=50, n=15, name='FuncRastrigin', desc=DESC):
+    def __init__(self, d=7, n=16, name='FuncRastrigin', desc=DESC):
         super().__init__(d, n, name, desc)
 
         self.set_grid(-5.12, +5.12)
         self.shift_grid()
 
         self.set_min(x=[0.]*self.d, y=0.)
 
     @property
-    def identity(self):
-        return super().identity + ['seed']
-
-    @property
     def is_func(self):
         return True
 
     @property
     def with_cores(self):
         return True
```

### Comparing `teneva_bm-0.5.0/teneva_bm/func/bm_func_rosenbrock.py` & `teneva_bm-0.6.0/teneva_bm/func/bm_func_rosenbrock.py`

 * *Files 11% similar despite different names*

```diff
@@ -3,42 +3,36 @@
 
 
 from teneva_bm import Bm
 
 
 DESC = """
     Analytical Rosenbrock function (continuous).
-    The dimension and mode size may be any (default are d=50, n=15).
-    Default grid limits are [-2.048, 2.048]; the exact global minimum
-    is known: x = [1, ..., 1], y = 0.
-    See https://www.sfu.ca/~ssurjano/rosen.html for details.
-    See also the work Momin Jamil, Xin-She Yang. "A literature survey of
+    The dimension and mode size may be any (default are d=7, n=16).
+    Default grid limits are [-2.048, 2.048] (with small random shift);
+    the exact global minimum is known: x = [1, ..., 1], y = 0.
+    See the work Momin Jamil, Xin-She Yang. "A literature survey of
     benchmark functions for global optimization problems". Journal of
     Mathematical Modelling and Numerical Optimisation 2013; 4:150-194
     ("105. Rosenbrock Function"; Continuous, Differentiable,
     Non-Separable, Scalable, Unimodal).
-    Note that the method "build_cores" for construction of the function
-    in the TT-format on the discrete grid is available.
+    See also https://www.sfu.ca/~ssurjano/rosen.html for details.
 """
 
 
 class BmFuncRosenbrock(Bm):
-    def __init__(self, d=50, n=15, name='FuncRosenbrock', desc=DESC):
+    def __init__(self, d=7, n=16, name='FuncRosenbrock', desc=DESC):
         super().__init__(d, n, name, desc)
 
         self.set_grid(-2.048, +2.048)
-        self.shift_grid()
+        self.shift_grid(sign=-1)
 
         self.set_min(x=[1.]*self.d, y=0.)
 
     @property
-    def identity(self):
-        return super().identity + ['seed']
-
-    @property
     def is_func(self):
         return True
 
     @property
     def with_cores(self):
         return True
```

### Comparing `teneva_bm-0.5.0/teneva_bm/func/bm_func_schaffer.py` & `teneva_bm-0.6.0/teneva_bm/func/bm_func_schaffer.py`

 * *Files 8% similar despite different names*

```diff
@@ -3,39 +3,35 @@
 
 
 from teneva_bm import Bm
 
 
 DESC = """
     Analytical Schaffer function (continuous).
-    The dimension and mode size may be any (default are d=50, n=15).
-    Default grid limits are [-100, 100]; the exact global minimum
-    is known: x = [0, ..., 0], y = 0.
+    The dimension and mode size may be any (default are d=7, n=16).
+    Default grid limits are [-100, 100] (with small random shift);
+    the exact global minimum is known: x = [0, ..., 0], y = 0.
     See the work Momin Jamil, Xin-She Yang. "A literature survey of
     benchmark functions for global optimization problems". Journal of
     Mathematical Modelling and Numerical Optimisation 2013; 4:150-194
     ("136. Schaffer F6 Function"; Continuous, Differentiable,
     Non-Separable, Scalable, Multimodal).
 """
 
 
 class BmFuncSchaffer(Bm):
-    def __init__(self, d=50, n=15, name='FuncSchaffer', desc=DESC):
+    def __init__(self, d=7, n=16, name='FuncSchaffer', desc=DESC):
         super().__init__(d, n, name, desc)
 
         self.set_grid(-100., +100.)
         self.shift_grid()
 
         self.set_min(x=[0.]*self.d, y=0.)
 
     @property
-    def identity(self):
-        return super().identity + ['seed']
-
-    @property
     def is_func(self):
         return True
 
     def target_batch(self, X):
         Z = X[:, :-1]**2 + X[:, 1:]**2
         Y = 0.5 + (np.sin(np.sqrt(Z))**2 - 0.5) / (1. + 0.001 * Z)**2
         return np.sum(Y, axis=1)
```

### Comparing `teneva_bm-0.5.0/teneva_bm/func/bm_func_schwefel.py` & `teneva_bm-0.6.0/teneva_bm/func/bm_func_schwefel.py`

 * *Files 6% similar despite different names*

```diff
@@ -3,42 +3,36 @@
 
 
 from teneva_bm import Bm
 
 
 DESC = """
     Analytical Schwefel function (continuous).
-    The dimension and mode size may be any (default are d=50, n=15).
-    Default grid limits are [-500, 500]; the exact global minimum
-    is known: x = [420.9687, ..., 420.9687], y = 0.
-    See https://www.sfu.ca/~ssurjano/schwef.html for details.
-    See also the work Momin Jamil, Xin-She Yang. "A literature survey of
+    The dimension and mode size may be any (default are d=7, n=16).
+    Default grid limits are [-500, 500] (with small random shift);
+    the exact global minimum is known: x = 420.9687, y = 0.
+    See the work Momin Jamil, Xin-She Yang. "A literature survey of
     benchmark functions for global optimization problems". Journal of
     Mathematical Modelling and Numerical Optimisation 2013; 4:150-194
     ("128. Schwefel 2.26 Function"; Continuous, Differentiable,
     Separable, Scalable, Multimodal).
-    Note that the method "build_cores" for construction of the function
-    in the TT-format on the discrete grid is available.
+    See also https://www.sfu.ca/~ssurjano/schwef.html for details.
 """
 
 
 class BmFuncSchwefel(Bm):
-    def __init__(self, d=50, n=15, name='FuncSchwefel', desc=DESC):
+    def __init__(self, d=7, n=16, name='FuncSchwefel', desc=DESC):
         super().__init__(d, n, name, desc)
 
         self.set_grid(-500., +500.)
         self.shift_grid()
 
         self.set_min(x=[420.9687]*self.d, y=0.)
 
     @property
-    def identity(self):
-        return super().identity + ['seed']
-
-    @property
     def is_func(self):
         return True
 
     @property
     def with_cores(self):
         return True
```

### Comparing `teneva_bm-0.5.0/teneva_bm/hs/bm_hs_func001.py` & `teneva_bm-0.6.0/teneva_bm/hs/bm_hs_func001.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,33 +1,39 @@
 import numpy as np
 
 
 from teneva_bm import Bm
 
 
 DESC = """
-    The function 001 from the Hock & Schittkowski collection.
-    The dimension should be 2, and the mode size may be any (default is 21),
+    DRAFT!!! The function 001 from the Hock & Schittkowski collection.
+    The dimension should be 2, and the mode size may be any (default is 64),
     the default limits for function inputs are [-10, 10].
     The exact global minimum is known: x = [1, 1], y = 0.
 """
 
 
 class BmHsFunc001(Bm):
-    def __init__(self, d=2, n=21, name='HsFunc001', desc=DESC):
+    def __init__(self, d=2, n=64, name='HsFunc001', desc=DESC):
         super().__init__(d, n, name, desc)
 
         if self.d != 2:
             self.set_err('Dimension should be 2')
 
-        self.set_grid(-10., +10.) # TODO: do we need random shift?
+        self.set_grid(-10., +10.)
+        # self.shift_grid()
+        # TODO: do we need a random shift as in "func" collection???
 
         self.set_min(x=[1.]*self.d, y=0.)
 
     @property
+    def identity(self):
+        return ['n']
+
+    @property
     def is_func(self):
         return True
 
     def target_batch(self, X):
         return 100. * (X[:, 1] - X[:, 0]**2)**2 + (1. - X[:, 0])**2
```

### Comparing `teneva_bm-0.5.0/teneva_bm/hs/bm_hs_func006.py` & `teneva_bm-0.6.0/teneva_bm/hs/bm_hs_func006.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,35 +1,45 @@
 import numpy as np
 
 
 from teneva_bm import Bm
 
 
 DESC = """
-    The function 006 from the Hock & Schittkowski collection
+    DRAFT!!! The function 006 from the Hock & Schittkowski collection
     with the explicit constraint.
-    The dimension should be 2, and the mode size may be any (default is 21),
+    The dimension should be 2, and the mode size may be any (default is 64),
     the default limits for function inputs are [-10, 10].
     The exact global minimum is known: x = [1, 1], y = 0.
     Note that the default penalty for the constraint is "1.E+3"
     and the amplitude of the constraint is used.
 """
 
 
 class BmHsFunc006(Bm):
-    def __init__(self, d=2, n=21, name='HsFunc006', desc=DESC):
+    def __init__(self, d=2, n=64, name='HsFunc006', desc=DESC):
         super().__init__(d, n, name, desc)
 
-        self.set_grid(-10., +10.) # TODO: do we need random shift?
+        if self.d != 2:
+            self.set_err('Dimension should be 2')
+            
+        self.set_grid(-10., +10.)
+        # self.shift_grid()
+        # TODO: do we need a random shift as in "func" collection???
 
         self.set_min(x=[1.]*self.d, y=0.)
 
+        # TODO: is it ok, to set such constraint by default???
         self.set_constr(penalty=1.E+3, eps=1.E-2, with_amplitude=True)
 
     @property
+    def identity(self):
+        return ['n']
+
+    @property
     def is_func(self):
         return True
 
     @property
     def with_constr(self):
         return True
```

### Comparing `teneva_bm-0.5.0/teneva_bm/hs/draft_constrained_functions/bm_hs007.py` & `teneva_bm-0.6.0/teneva_bm/hs/draft_constrained_functions/bm_hs007.py`

 * *Files identical despite different names*

### Comparing `teneva_bm-0.5.0/teneva_bm/hs/draft_constrained_functions/bm_hs008.py` & `teneva_bm-0.6.0/teneva_bm/hs/draft_constrained_functions/bm_hs008.py`

 * *Files identical despite different names*

### Comparing `teneva_bm-0.5.0/teneva_bm/hs/draft_constrained_functions/bm_hs009.py` & `teneva_bm-0.6.0/teneva_bm/hs/draft_constrained_functions/bm_hs009.py`

 * *Files identical despite different names*

### Comparing `teneva_bm-0.5.0/teneva_bm/hs/draft_constrained_functions/bm_hs010.py` & `teneva_bm-0.6.0/teneva_bm/hs/draft_constrained_functions/bm_hs010.py`

 * *Files identical despite different names*

### Comparing `teneva_bm-0.5.0/teneva_bm/hs/draft_constrained_functions/bm_hs011.py` & `teneva_bm-0.6.0/teneva_bm/hs/draft_constrained_functions/bm_hs011.py`

 * *Files identical despite different names*

### Comparing `teneva_bm-0.5.0/teneva_bm/hs/draft_constrained_functions/bm_hs012.py` & `teneva_bm-0.6.0/teneva_bm/hs/draft_constrained_functions/bm_hs012.py`

 * *Files identical despite different names*

### Comparing `teneva_bm-0.5.0/teneva_bm/hs/draft_unconstrained_functions/bm_hs002.py` & `teneva_bm-0.6.0/teneva_bm/hs/draft_unconstrained_functions/bm_hs002.py`

 * *Files identical despite different names*

### Comparing `teneva_bm-0.5.0/teneva_bm/hs/draft_unconstrained_functions/bm_hs003.py` & `teneva_bm-0.6.0/teneva_bm/hs/draft_unconstrained_functions/bm_hs003.py`

 * *Files identical despite different names*

### Comparing `teneva_bm-0.5.0/teneva_bm/hs/draft_unconstrained_functions/bm_hs004.py` & `teneva_bm-0.6.0/teneva_bm/hs/draft_unconstrained_functions/bm_hs004.py`

 * *Files identical despite different names*

### Comparing `teneva_bm-0.5.0/teneva_bm/hs/draft_unconstrained_functions/bm_hs005.py` & `teneva_bm-0.6.0/teneva_bm/hs/draft_unconstrained_functions/bm_hs005.py`

 * *Files identical despite different names*

### Comparing `teneva_bm-0.5.0/teneva_bm/hs/draft_unconstrained_functions/bm_hs038.py` & `teneva_bm-0.6.0/teneva_bm/hs/draft_unconstrained_functions/bm_hs038.py`

 * *Files identical despite different names*

### Comparing `teneva_bm-0.5.0/teneva_bm/hs/draft_unconstrained_functions/bm_hs045.py` & `teneva_bm-0.6.0/teneva_bm/hs/draft_unconstrained_functions/bm_hs045.py`

 * *Files identical despite different names*

### Comparing `teneva_bm-0.5.0/teneva_bm/oc/bm_oc_simple.py` & `teneva_bm-0.6.0/teneva_bm/odeoc/bm_odeoc_simple.py`

 * *Files 4% similar despite different names*

```diff
@@ -15,33 +15,37 @@
     Discrete optimal control (OC) problem with simple 1D ODE "x**3 - i",
     where "x = x(t)" is a state variable, "x(0) = x_ini" and "i" is a
     binary control variable. The loss function for the optimal control
     problem is "0.5 * (x-x_ref)^2", where "x_ref" is a target value, and
     the maximum time value is "t_max". Note that for some control values
     the solver (gekko) fails, in this case we return the value "y_err".
     By default (see parameters of the "set_opts" function), "x_ini = 0.8",
-    "x_ref = 0.7", "t_max = 1" and "y_err = 1.E+50".
-    The dimension may be any (default is 50), and the mode size should be 2.
-    The benchmark needs "gekko==1.0.6" library (it is used for ODE solution).
+    "x_ref = 0.7", "t_max = 1" and "y_err = 1.E+50". The dimension may be
+    any (default is 100), and the mode size should be 2. The benchmark
+    needs "gekko==1.0.6" library (it is used for ODE solution).
 """
 
 
-class BmOcSimple(Bm):
-    def __init__(self, d=50, n=2, name='OcSimple', desc=DESC):
+class BmOdeocSimple(Bm):
+    def __init__(self, d=100, n=2, name='OdeocSimple', desc=DESC):
         super().__init__(d, n, name, desc)
 
         if not self.is_n_equal or self.n[0] != 2:
             self.set_err('Mode size (n) should be "2"')
 
         if not with_gekko:
             msg = 'Need "gekko" module. For installation please run '
             msg += '"pip install gekko==1.0.6"'
             self.set_err(msg)
 
     @property
+    def identity(self):
+        return ['d']
+
+    @property
     def is_tens(self):
         return True
 
     def get_config(self):
         conf = super().get_config()
         conf['_x_ini'] = self._x_ini
         conf['_x_ref'] = self._x_ref
@@ -117,15 +121,15 @@
         """Objective function for ODE solution."""
         return 0.5 * (x - self._x_ref)**2
 
 
 if __name__ == '__main__':
     np.random.seed(42)
 
-    bm = BmOcSimple().prep()
+    bm = BmOdeocSimple().prep()
     print(bm.info())
 
     I_trn, y_trn = bm.build_trn(1.E+2)
     print(bm.info_history())
 
     text = 'Value at a random multi-index     :  '
     i = [np.random.choice(k) for k in bm.n]
```

### Comparing `teneva_bm-0.5.0/teneva_bm/oc/bm_oc_simple_constr.py` & `teneva_bm-0.6.0/teneva_bm/odeoc/bm_odeoc_simple_constr.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 import numpy as np
 
 
-from teneva_bm.oc import BmOcSimple
+from teneva_bm.odeoc import BmOdeocSimple
 
 
 DESC = """
     Discrete optimal control (OC) problem with constraint of the special
-    form. This benchmark is the same as "BmOcSimple", except the constraint.
-    Please see the description of BmOcSimple for more details.
-    The dimension may be any (default is 50), and the mode size should be 2.
+    form. This benchmark is the same as "BmOdeocSimple", except the
+    constraint. Please see the description of BmOdeocSimple for more details.
+    The dimension may be any (default is 100), and the mode size should be 2.
     The benchmark needs "gekko==1.0.6" library (it is used for ODE solution).
-    Note that the default penalty for the constraint is "1.E+42"
-    and the amplitude of the constraint does not used.
+    Note that the default penalty for the constraint is "1.E+42" and the
+    amplitude of the constraint does not used.
 """
 
 
-class BmOcSimpleConstr(BmOcSimple):
-    def __init__(self, d=50, n=2, name='OcSimpleConstr', desc=DESC):
+class BmOdeocSimpleConstr(BmOdeocSimple):
+    def __init__(self, d=100, n=2, name='OdeocSimpleConstr', desc=DESC):
         super().__init__(d, n, name, desc)
 
-        self.set_constr(penalty=1.E+42, with_amplitude=True)
+        self.set_constr(penalty=1.E+42, with_amplitude=False)
 
     @property
     def with_constr(self):
         return True
 
     def constr(self, i):
         s = ''.join([str(k) for k in i])
@@ -38,15 +38,15 @@
 
         return 1. if condition_false else -1.
 
 
 if __name__ == '__main__':
     np.random.seed(42)
 
-    bm = BmOcSimpleConstr().prep()
+    bm = BmOdeocSimpleConstr().prep()
     print(bm.info())
 
     I_trn, y_trn = bm.build_trn(1.E+2)
     print(bm.info_history())
 
     text = 'Value at a random multi-index     :  '
     i = [np.random.choice(k) for k in bm.n]
```

### Comparing `teneva_bm-0.5.0/teneva_bm/qubo/bm_qubo_knap_det.py` & `teneva_bm-0.6.0/teneva_bm/qubo/bm_qubo_knap_det.py`

 * *Files 0% similar despite different names*

```diff
@@ -8,21 +8,21 @@
     Binary knapsack problem -1 * sum p_i x_i -> min s.t. sum w_i x_i < C with
     fixed weights w, profits p and the capacity C. The exact minimum is known
     (d=10: -295, d=20: -1024, d=50: -3103, d=80: -5183, d=100: -15170).
     We use the values of parameters from the work Dong et al. 2021 (problems
     k1-k5), where phase angle modulated bat algorithm (P-AMBA) was proposed
     for high dimensional binary optimization problems with application to
     antenna topology optimization. The dimension should be in 10, 20, 50, 80,
-    100, and the mode size should be 2. Note that the default penalty for the
-    constraint is "0".
+    100 (the default value is 100), and the mode size should be 2. Note that
+    the default penalty for the constraint is "0".
 """
 
 
 class BmQuboKnapDet(Bm):
-    def __init__(self, d=50, n=2, name='QuboKnapDet', desc=DESC):
+    def __init__(self, d=100, n=2, name='QuboKnapDet', desc=DESC):
         super().__init__(d, n, name, desc)
 
         if not self.is_n_equal or self.n0 != 2:
             self.set_err('Mode size (n) should be "2"')
 
         if self.d == 10:
             i = [0, 1, 1, 1, 0, 0, 0, 1, 1, 1]
@@ -55,14 +55,18 @@
 
         else:
             self.set_err('Dimension should be in 10, 20, 50, 80, 100')
 
         self.set_constr(penalty=0.)
 
     @property
+    def identity(self):
+        return ['d']
+
+    @property
     def is_tens(self):
         return True
 
     @property
     def with_constr(self):
         return True
```

### Comparing `teneva_bm-0.5.0/teneva_bm/qubo/bm_qubo_knap_quad.py` & `teneva_bm-0.6.0/teneva_bm/qubo/bm_qubo_knap_quad.py`

 * *Files 12% similar despite different names*

```diff
@@ -9,35 +9,34 @@
 
 
 from teneva_bm import Bm
 
 
 DESC = """
     Quadratic unconstrained binary optimization (QUBO) knapsack problem
-    represented as a discrete function.
-    The dimension may be any (default is 50), and the mode size should be 2.
-    The benchmark needs "qubogen==0.1.1" library.
+    represented as a discrete function. The dimension may be any (default is
+    100), and the mode size should be 2. It needs "qubogen==0.1.1" library.
 """
 
 
 class BmQuboKnapQuad(Bm):
-    def __init__(self, d=50, n=2, name='QuboKnapQuad', desc=DESC):
+    def __init__(self, d=100, n=2, name='QuboKnapQuad', desc=DESC):
         super().__init__(d, n, name, desc)
 
         if not self.is_n_equal or self.n0 != 2:
             self.set_err('Mode size (n) should be "2"')
 
         if not with_qubogen:
             msg = 'Need "qubogen" module. For installation please run '
             msg += '"pip install qubogen==0.1.1"'
             self.set_err(msg)
 
     @property
     def identity(self):
-        return super().identity + ['seed']
+        return ['d', 'seed']
 
     @property
     def is_tens(self):
         return True
 
     def prep_bm(self):
         v = np.diag(self.rand.random(self.d)) / 3.
```

### Comparing `teneva_bm-0.5.0/teneva_bm/qubo/bm_qubo_maxcut.py` & `teneva_bm-0.6.0/teneva_bm/qubo/bm_qubo_mvc.py`

 * *Files 4% similar despite different names*

```diff
@@ -15,23 +15,23 @@
     with_qubogen = False
 
 
 from teneva_bm import Bm
 
 
 DESC = """
-    Quadratic unconstrained binary optimization (QUBO) Max-Cut problem
-    represented as a discrete function.
-    The dimension may be any (default is 50), and the mode size should be 2.
-    The benchmark needs "networkx==3.0" and "qubogen==0.1.1" libraries.
+    Quadratic unconstrained binary optimization (QUBO) Minimum Vertex Cover
+    (MVC) problem represented as a discrete function. The dimension may be
+    any (default is 100), and the mode size should be 2. The benchmark needs
+    "networkx==3.0" and "qubogen==0.1.1" libraries.
 """
 
 
-class BmQuboMaxcut(Bm):
-    def __init__(self, d=50, n=2, name='QuboMaxcut', desc=DESC):
+class BmQuboMvc(Bm):
+    def __init__(self, d=100, n=2, name='QuboMVC', desc=DESC):
         super().__init__(d, n, name, desc)
 
         if not self.is_n_equal or self.n0 != 2:
             self.set_err('Mode size (n) should be "2"')
 
         if not with_networkx:
             msg = 'Need "networkx" module. For installation please run '
@@ -41,15 +41,15 @@
         if not with_qubogen:
             msg = 'Need "qubogen" module. For installation please run '
             msg += '"pip install qubogen==0.1.1"'
             self.set_err(msg)
 
     @property
     def identity(self):
-        return super().identity + ['seed']
+        return ['d', 'seed']
 
     @property
     def is_tens(self):
         return True
 
     def get_config(self):
         conf = super().get_config()
@@ -69,15 +69,15 @@
         d = self.d
         p = self._prob_con
         graph = nx.fast_gnp_random_graph(n=d, p=p, seed=self.seed)
         edges = np.array(list([list(e) for e in graph.edges]))
         n_nodes = len(np.unique(np.array(edges).flatten()))
 
         g = qubogen.Graph(edges=edges, n_nodes=n_nodes)
-        self._Q = qubogen.qubo_max_cut(g)
+        self._Q = qubogen.qubo_mvc(g)
 
     def set_opts(self, prob_con=0.5):
         """Setting options specific to the benchmark.
 
         There are no plans to manually change the default values.
 
         Args:
@@ -89,15 +89,15 @@
     def target_batch(self, I):
         return ((I @ self._Q) * I).sum(axis=1)
 
 
 if __name__ == '__main__':
     np.random.seed(42)
 
-    bm = BmQuboMaxcut().prep()
+    bm = BmQuboMvc().prep()
     print(bm.info())
 
     I_trn, y_trn = bm.build_trn(1.E+4)
     print(bm.info_history())
 
     text = 'Value at a random multi-index            :  '
     i = [np.random.choice(k) for k in bm.n]
```

### Comparing `teneva_bm-0.5.0/teneva_bm/qubo/bm_qubo_mvc.py` & `teneva_bm-0.6.0/teneva_bm/qubo/bm_qubo_maxcut.py`

 * *Files 4% similar despite different names*

```diff
@@ -15,23 +15,23 @@
     with_qubogen = False
 
 
 from teneva_bm import Bm
 
 
 DESC = """
-    Quadratic unconstrained binary optimization (QUBO) Minimum Vertex Cover
-    (MVC) problem represented as a discrete function.
-    The dimension may be any (default is 50), and the mode size should be 2.
-    The benchmark needs "networkx==3.0" and "qubogen==0.1.1" libraries.
+    Quadratic unconstrained binary optimization (QUBO) Max-Cut problem
+    represented as a discrete function. The dimension may be any (default
+    is 100), and the mode size should be 2. The benchmark needs
+    "networkx==3.0" and "qubogen==0.1.1" libraries.
 """
 
 
-class BmQuboMvc(Bm):
-    def __init__(self, d=50, n=2, name='QuboMVC', desc=DESC):
+class BmQuboMaxcut(Bm):
+    def __init__(self, d=100, n=2, name='QuboMaxcut', desc=DESC):
         super().__init__(d, n, name, desc)
 
         if not self.is_n_equal or self.n0 != 2:
             self.set_err('Mode size (n) should be "2"')
 
         if not with_networkx:
             msg = 'Need "networkx" module. For installation please run '
@@ -41,15 +41,15 @@
         if not with_qubogen:
             msg = 'Need "qubogen" module. For installation please run '
             msg += '"pip install qubogen==0.1.1"'
             self.set_err(msg)
 
     @property
     def identity(self):
-        return super().identity + ['seed']
+        return ['d', 'seed']
 
     @property
     def is_tens(self):
         return True
 
     def get_config(self):
         conf = super().get_config()
@@ -69,15 +69,15 @@
         d = self.d
         p = self._prob_con
         graph = nx.fast_gnp_random_graph(n=d, p=p, seed=self.seed)
         edges = np.array(list([list(e) for e in graph.edges]))
         n_nodes = len(np.unique(np.array(edges).flatten()))
 
         g = qubogen.Graph(edges=edges, n_nodes=n_nodes)
-        self._Q = qubogen.qubo_mvc(g)
+        self._Q = qubogen.qubo_max_cut(g)
 
     def set_opts(self, prob_con=0.5):
         """Setting options specific to the benchmark.
 
         There are no plans to manually change the default values.
 
         Args:
@@ -89,15 +89,15 @@
     def target_batch(self, I):
         return ((I @ self._Q) * I).sum(axis=1)
 
 
 if __name__ == '__main__':
     np.random.seed(42)
 
-    bm = BmQuboMvc().prep()
+    bm = BmQuboMaxcut().prep()
     print(bm.info())
 
     I_trn, y_trn = bm.build_trn(1.E+4)
     print(bm.info_history())
 
     text = 'Value at a random multi-index            :  '
     i = [np.random.choice(k) for k in bm.n]
```

### Comparing `teneva_bm-0.5.0/teneva_bm/teneva_bm_demo.py` & `teneva_bm-0.6.0/teneva_bm/teneva_bm_demo.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,20 +2,20 @@
 import re
 import subprocess
 
 
 def teneva_bm_demo(bm_use=None, with_info=True, all=False):
     """Demo script for teneva_bm.
 
-    Run demo for all existing benchmarks (if "bm_use" is None) or for a
-    specific benchmark (if "bm_use" is provided; e.g., "bm_qubo_knap_amba"). If
-    the flag "with_info" is set, then the stats for existing collections and
-    benchmarks will be also printed. Note that the code for the demo run of
-    benchmarks should be at the end of the corresponding benchmark file in the
-    section "if __name__ == '__main__':".
+    Run demo for all existing benchmarks (if "bm_use" is None and "all" is
+    True) or for a specific benchmark (if "bm_use" is provided). If the flag
+    "with_info" is set, then the stats for existing collections and benchmarks
+    will be also printed. Note that the code for the demo run of benchmarks
+    should be at the end of the corresponding benchmark file in the section
+    "if __name__ == '__main__':".
 
     """
     bms = {}
     found = False
 
     if bm_use:
         all = False
```

### Comparing `teneva_bm-0.5.0/teneva_bm/various/bm_matmul.py` & `teneva_bm-0.6.0/teneva_bm/various/bm_matmul.py`

 * *Files 0% similar despite different names*

```diff
@@ -15,20 +15,19 @@
     be set manually in the case if "size > 2" (e.g., for the "size = 3", the
     best known rank is "23"). The default mode size is "3", which relates to
     a standard matrix multiplication task; in this case, we are looking for a
     decomposition with factor matrix entries "-1, 0, 1". A mode size of "5"
     is also supported, which relates to the possible values "-2, -1, 0, 1, 2".
     If the "only2" flag is set during initialization, then only two factor
     matrices will be constructed, and the third matrix will be restored as a
-    solution to the corresponding system of linear equations.
-    The benchmark has also the method "recover", which returns the factor
-    matrices for the given multi-indices.
-    For more details, see the work Fawzi, A., et al. "Discovering faster
-    matrix multiplication algorithms with reinforcement learning." Nature
-    610.7930 (2022): 47-53.
+    solution to the corresponding system of linear equations. The benchmark
+    has also the method "recover", which returns the factor matrices for the
+    given multi-indices. For more details, see the work Fawzi, A., et al.
+    "Discovering faster matrix multiplication algorithms with reinforcement
+    learning." Nature 610.7930 (2022): 47-53.
 """
 
 
 class BmMatmul(Bm):
     def __init__(self, d=None, n=3, name='Matmul', desc=DESC, size=2, rank=7,
                  only2=False):
         T_real = _tensor_generate(size, size, size)
```

### Comparing `teneva_bm-0.5.0/teneva_bm/various/bm_topopt.py` & `teneva_bm-0.6.0/teneva_bm/various/bm_topopt.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,16 +4,17 @@
 from scipy.sparse.linalg import spsolve
 
 
 from teneva_bm import Bm
 
 
 DESC = """
-    Discrete Topology optimization task. This is a draft!!!
-    The dimension and mode size are defined from "nx" and "ny" parameters.
+    DRAFT!!! Discrete Topology optimization task.
+    The dimension is defined from "nx" and "ny" parameters and mode size
+    should be 2.
 """
 
 
 class BmTopopt(Bm):
     def __init__(self, d=None, n=2, name='BmTopopt', desc=DESC, nx=128, ny=32):
         super().__init__(nx*ny, n, name, desc)
 
@@ -393,10 +394,11 @@
     i3 = [np.random.choice(k) for k in bm.n]
     I = [i1, i2, i3]
     y = bm[I]
     text += '; '.join([f'{y_cur:-10.3e}' for y_cur in y])
     print(text)
 
     text = 'Generate image for a random multi-index  :  '
-    bm.show('result/BmTopopt_demo', np.array(i))
-    text += 'see "result" folder with png file'
+    fpath = f'result/{bm.name}/show'
+    bm.show(fpath)
+    text += f' see {fpath}'
     print(text)
```

### Comparing `teneva_bm-0.5.0/teneva_bm/various/bm_wall_simple.py` & `teneva_bm-0.6.0/teneva_bm/various/bm_wall_simple.py`

 * *Files identical despite different names*

### Comparing `teneva_bm-0.5.0/teneva_bm.egg-info/PKG-INFO` & `teneva_bm-0.6.0/teneva_bm.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: teneva-bm
-Version: 0.5.0
+Version: 0.6.0
 Summary: Benchmarks library, based on the software product teneva, for testing multivariate approximation and optimization methods
 Home-page: https://github.com/AndreiChertkov/teneva_bm
 Author: Andrei Chertkov
 Author-email: andre.chertkov@gmail.com
 License: MIT
 Project-URL: Source, https://github.com/AndreiChertkov/teneva_bm
 Keywords: benchmarks approximation optimization multidimensional array multivariate function low-rank representation tensor train format TT-decomposition
@@ -30,30 +30,30 @@
 ## Description
 
 Benchmarks library, based on the software product [teneva](https://github.com/AndreiChertkov/teneva), for testing multidimensional approximation and optimization methods. Our benchmarks include both multidimensional data arrays and discretized functions of many variables.
 
 
 ## Installation
 
-> Current version "0.5.0".
+> Current version "0.6.0".
 
-The package can be installed via pip: `pip install teneva_bm` (it requires the [Python](https://www.python.org) programming language of the version >= 3.8). It can be also downloaded from the repository [teneva_bm](https://github.com/AndreiChertkov/teneva_bm) and installed by `python setup.py install` command from the root folder of the project.
+The package can be installed via pip: `pip install teneva_bm` (it requires the [Python](https://www.python.org) programming language of the version 3.8 or 3.9). It can be also downloaded from the repository [teneva_bm](https://github.com/AndreiChertkov/teneva_bm) and installed by `python setup.py install` command from the root folder of the project.
 
-> Required python packages (see `requirements.txt`) [matplotlib](https://matplotlib.org/) (3.7.0+) and [teneva](https://github.com/AndreiChertkov/teneva) (0.14.2+) will be automatically installed during the installation of the main software product.
+> Required python packages (see `requirements.txt`) [matplotlib](https://matplotlib.org/) (3.7.0+) and [teneva](https://github.com/AndreiChertkov/teneva) (0.14.5+) will be automatically installed during the installation of the main software product.
 
-Some benchmarks require additional installation of specialized libraries. The corresponding instructions are given in the description of each benchmark (see `DESC` string in the python files with benchmarks). Installation of all required libraries for all benchmarks can be done with the following command:
+Some benchmarks require additional installation of specialized libraries. The corresponding instructions are given in the description of each benchmark (see `DESC` string in the python files with benchmarks). Installation of all required libraries for all benchmarks can be done with the following commands:
 
 - Collections `func`, `hs` and `various` do not require installation of additional libraries.
 
-- Сollections `oc` and `qubo` require installation of the following libraries:
+- Сollections `odeoc` and `qubo` require installation of the following libraries:
     ```bash
     pip install networkx==3.0 qubogen==0.1.1 gekko==1.0.6
     ```
 
-- Сollections `agent` and `agent_toe` require a rather complicated installation process of the `gym` and `mujoco` frameworks and related packages, so we have prepared a special python installation script [install_mujoco.py](https://github.com/AndreiChertkov/teneva_bm/blob/main/install_mujoco.py). Detailed instructions for using the script are presented in the file header.
+- Сollection `agent` require a rather complicated installation process of the `gym` and `mujoco` frameworks and related packages, so we have prepared a special python installation script [install_mujoco.py](https://github.com/AndreiChertkov/teneva_bm/blob/main/install_mujoco.py). Detailed instructions for using the script are presented in the file header.
 
 > To run benchmark optimization examples (see `demo_opti` folder), you should also install the [PROTES](https://github.com/anabatsh/PROTES) optimizer (`pip install protes==0.3.3`).
 
 
 ## Documentation and examples
 
 All benchmarks inherit from the `Bm` base class (`teneva_bm/bm.py`) and are located in the subfolders (collections of benchmarks) of `teneva_bm` folder. The corresponding python files contain a detailed description of the benchmarks, as well as a scripts for a demo run at the end of the files. You can get detailed information on the created benchmark using the `info` class method:
@@ -66,30 +66,28 @@
 
 You can run demos for all benchmarks at once with the command `python demo.py` from the root folder of the project (you can also specify the name of the benchmark as a script argument to run the demo for only one benchmark, e.g., `python demo.py bm_qubo_knap_det`). You can also use a function from the `teneva_bm` package to run all or only one demo:
 ```python
 from teneva_bm import teneva_bm_demo
 teneva_bm_demo('bm_qubo_knap_det', with_info=True)
 ```
 
-> We prepare some demo scripts with benchmark optimization examples in the `demo_opti` folder. To run these examples (e.g., `python demo_opti/demo_base.py`), you need to install the [PROTES](https://github.com/anabatsh/PROTES) optimizer (`pip install protes==0.3.3`).
-
-> We also present some examples in this [colab notebook](https://colab.research.google.com/drive/1z8LgqEARJziKub2dVB65CHkhcboc-fCH?usp=sharing).
+> We prepare some demo scripts with benchmark optimization examples in the `demo_opti` folder. To run these examples (e.g., `python demo_opti/base.py`), you need to install the [PROTES](https://github.com/anabatsh/PROTES) optimizer). We also present some examples in this [colab notebook](https://colab.research.google.com/drive/1z8LgqEARJziKub2dVB65CHkhcboc-fCH?usp=sharing).
 
 
 ## Available benchmarks
 
-- `agent` - the collection of problems from [gym](https://www.gymlibrary.dev/) framework, including [mujoco agents](https://www.gymlibrary.dev/environments/mujoco/index.html) based on the physics engine [mujoco](https://mujoco.org/) for faciliatating research and development in robotics, biomechanics, graphics and animation. The collection includes the following benchmarks: `BmAgentSwimmer`.
-    > Within the framework of this collection, explicit optimization of the entire set of actions (discrete or continuous) may be performed (i.e., `none` policy) or discrete Toeplitz policy may be used.
+- `agent` - the collection of problems from [gym](https://www.gymlibrary.dev/) framework, including [mujoco agents](https://www.gymlibrary.dev/environments/mujoco/index.html) based on the physics engine [mujoco](https://mujoco.org/) for faciliatating research and development in robotics, biomechanics, graphics and animation. The collection includes the following benchmarks: `BmAgentAnt`, `BmAgentHuman`, `BmAgentHumanStand`, `BmAgentLake`, `BmAgentPendInv`, `BmAgentPendInvDouble`, `BmAgentSwimmer`.
+    > Within the framework of this collection, explicit optimization of the entire set of actions (discrete or continuous) may be performed (if `direct` policy name is set) or discrete Toeplitz policy may be used (if `toeplitz` policy name is set; it is the default value); you can also set your own custom policy as an instance of the correct class (see `agent/policy.py` for details).
 
 - `func` - a collection of analytic functions of a real multidimensional argument. The collection includes the following benchmarks: `BmFuncAckley`, `BmFuncAlpine`, `BmFuncDixon`, `BmFuncExp`, `BmFuncGriewank`, `BmFuncMichalewicz`, `BmFuncPiston` (only `d=7` is supported), `BmFuncQing`, `BmFuncRastrigin`, `BmFuncRosenbrock`, `BmFuncSchaffer`, `BmFuncSchwefel`.
     > For almost all functions, the exact global minimum ("continuous x point", not multi-index) is known (see `bm.x_min_real` and `bm.y_min_real`). For a number of functions (`BmFuncAlpine`, `BmFuncExp`, `BmFuncGriewank`, `BmFuncMichalewicz`, `BmFuncQing`, `BmFuncRastrigin`, `BmFuncRosenbrock`, `BmFuncSchwefel`), a `bm.build_cores()` method is available that returns an exact representation of the function on the discrete grid used in the benchmark in the tensor train (TT) format as a list of 3D TT-cores. Note also that we apply small random shift of the grid limits for all functions, to make the optimization problem more difficult (because many functions have a minimum at the center point of the domain).
 
 - `hs` (draft!) - the [Hock & Schittkowski](http://apmonitor.com/wiki/index.php/Apps/HockSchittkowski) collection of benchmark functions, containing continuous analytic functions of small dimensions (2-5), some of which have given constraints. The collection includes the following benchmarks: `BmHsFunc001`, `BmHsFunc006`.
 
-- `oc` - a collection of optimal control problems described by ordinary differential equations with discrete binary control variable, some of the problems have explicit restrictions on the elements of the control vector. The collection includes the following benchmarks: `BmOcSimple`, `BmOcSimpleConstr`.
+- `odeoc` - a collection of optimal control problems described by ordinary differential equations, some of the problems have explicit restrictions on the elements of the control vector. The collection includes the following benchmarks: `BmOdeocSimple`, `BmOdeocSimpleConstr`.
 
 - `qubo` - a collection of quadratic unconstrained binary optimization (QUBO) problems; all benchmarks are discrete and have a mode size equals `2`. The collection includes the following benchmarks: `BmQuboKnapDet`, `BmQuboKnapQuad`, `BmQuboMaxcut`, `BmQuboMvc`.
     > The exact global minimum is known only for `BmQuboKnapDet` benchmark (note that this benchmark supports only dimensions `10`, `20`, `50`, `80` and `100`).
 
 - `various` - a collection of heterogeneous benchmarks that are not suitable for any other collection (note that in this case, we do not use the name of the collection in the name of the benchmarks, unlike all other sets). The collection includes the following benchmarks: `BmMatmul`, `BmTopopt` (draft!), `BmWallSimple`.
 
 
@@ -99,110 +97,117 @@
 
 ##### Benchmark initialization
 
 First, we create an instance of the desired benchmark class and manually call the `prep` method (optionally, we can also print detailed information about the benchmark):
 ```python
 import numpy as np
 from teneva_bm import *
-np.random.seed(42)
 
 bm = BmFuncAckley()
 bm.prep()
 print(bm.info())
 ```
 
 The class constructor of all benchmarks has the following optional arguments:
 
 - `d` - dimension of the benchmark's input (non-negative integer). For some benchmarks, this number is hardcoded (or depends on other specified auxiliary arguments), if another value is explicitly passed, an error message will be generated (e.g., the dimension for benchmark `various.bm_matmul` is determined automatically by the values of auxiliary arguments `size`, `rank` and `only2`). By default, some correct value is used (specified in the benchmark description).
 
 - `n` - number of possible discrete values for benchmark input variables, i.e., the mode size of the related tensor / multidimensional array (non-negative integer if all mode sizes are equal or a list of non-negative integers of the length `d`). For some benchmarks, this number is hardcoded (or depends on other specified auxiliary arguments), if another value is explicitly passed, an error message will be generated (e.g., in `qubo` collection all benchmarks should have `n = 2`). By default, some correct value is used (specified in the benchmark description).
 
-- `name` - the display name of the benchmark (string). By default, the name corresponding to the file/class name is used.
+- `name` - the display name of the benchmark (string). By default, the name corresponding to the file/class name (without `Bm` prefix) is used.
 
 - `desc` - the description of the benchmark (string). By default, a detailed description of the benchmark is used, provided in the corresponding python file.
 
 - `...other arguments...` - some benchmarks have additional optional arguments, which are described in the corresponding python files.
 
 ##### Setting advanced options
 
 Before calling the `bm.prep()` method, you can set a number of additional benchmark options:
 
 - `bm.set_seed(seed=42)` - with this function we can set a custom random seed. Note that we use `Random Generator` from numpy (i.e., `numpy.random.default_rng(seed)`) and for a fixed value of the seed, the behavior of the benchmark will always be the same, however, not all benchmarks depend on a seed.
 
-- `bm.set_grid_kind(kind='cheb')` - by default, we use the Chebyshev grid (`kind = 'cheb'`), but you can alternatively set it manually to use a uniform grid (`kind = 'uni'`).
+- `bm.set_grid_kind(kind='cheb')` - by default, we use the Chebyshev grid (`kind = 'cheb'`) for benchmarks corresponds to a function of a continuous argument, but you can alternatively set it manually to use a uniform grid (`kind = 'uni'`).
 
 - `bm.set_budget(m=None, m_cache=None, is_strict=True)` - optional method to set the computation buget `m`. If the number of requests to the benchmark (from calls to `bm.get` and `bm.get_poi` methods) exceeds the specified budget, then `None` will be returned. If the flag `is_strict` is disabled, then the request for the last batch will be allowed, after which the budget will be exceeded, otherwise this last batch will not be considered. Note that when the budget is exceeded, `None` will be returned both when requesting a single value and a batch of values. Also, in a similar way, you can set a limit on the use of the cache by `m_cache` parameter.
 
-- `bm.set_constr(penalty=1.E+42, eps=1.E-16, with_amplitude=True)` - if the benchmark has a constraint, then using this function you can set a `penalty` (for the requested points that do not satisfy the constraint, the value `penalty * constraint_value` will be returned) and a `eps` (threshold value to check that the constraint has been fulfilled). Note that we set the constraints as a function (`bm.constr`) that returns the value `constraint_value` (amplitude) of the constraint, and if the constraint is met, then the value must be non-positive, otherwise, the objective function is not calculated and a value proportional to the amplitude of the constraint is returned (if you disable flag `with_amplitude`, then just the value of the penalty will be returned). For the case of maximization task you should set negative `penalty` value.
+- `bm.set_constr(penalty=1.E+42, eps=1.E-16, with_amplitude=True)` - if the benchmark has a constraint, then using this function you can set a `penalty` (for the requested points that do not satisfy the constraint, the value `penalty * constraint_value` will be returned) and a `eps` (threshold value to check that the constraint has been fulfilled). Note that we set the constraints as a function (`bm.constr` / `bm.constr_batch`) that returns the value `constraint_value` (amplitude) of the constraint, and if the constraint is met, then the value must be non-positive, otherwise, the objective function is not calculated and a value proportional to the amplitude of the constraint is returned (if you disable flag `with_amplitude`, then just the value of the penalty will be returned). For the case of maximization task you should set negative `penalty` value.
 
 - `bm.set_max(i=None, x=None, y=None)` - if necessary, you can manually set the multi-index, the corresponding continuous point (for benchmarks, which relate to functions of a continuous argument), and the corresponding value for the exact global maximum of the function. The corresponding values will be further available in the benchmark as `bm.i_max_real`, `bm.x_max_real` and `bm.y_max_real` respectively. When the benchmark is initialized, this function is called automatically if the optimum is known.
 
 - `bm.set_min(i=None, x=None, y=None)` - the same as in the previous point, but for the global minimum.
 
-- `bm.set_log(with_log=False, cond='min-max', step=1000, prefix='bm', with_min=True, with_max=True)` - when calling this function with the `True` argument `with_log`, the log will be printed while requests to benchmark. You may set the log codition `cond` (`min`, `max`, `min-max` or `step`; e.g., in the case `min` the log will be presented each time the `min` value is updated), the log step (for condition `step`) and a string `prefix` for the log. You can also disable the display of current minimum values (`with_min`) or maximum values (`with_max`) in the log string.
+- `bm.set_log(log=False, cond='min-max', step=1000, prefix='bm', with_min=True, with_max=True)` - when calling this function with the `True` argument `log`, the log will be printed while requests to benchmark. You may set the log codition `cond` (`min`, `max`, `min-max` or `step`; e.g., in the case `min` the log will be presented each time the `min` value is updated), the log step (for condition `step`) and a string `prefix` for the log. You can also disable the display of current minimum values (`with_min`) or maximum values (`with_max`) in the log string. Note that you can provide as `log` argument some print-like function, e.g., `log=print`, in this case, printing will occur not to the console, but to the corresponding function.
 
-- `bm.set_cache(with_cache=False, cache=None, m_max=1.E+8)` - when calling this function with the `True` argument `with_cache`, the cache will be used, that is, all the values requested from the benchmark will be saved and when the same multi-indices are accessed again, the values will be retrieved from the cache instead of explicitly calculating the objective function. Additionally, you can optionally pass as an argument `cache` an already existing cache in the form of a dictionary (the keys are multi-indices in the form of tuples, and the values are the corresponding values of the objective function). We especially note that the cache is only used when querying benchmark values in discrete multi-indices; for requested continuous points, no cache will be used. It is also important to note that no cache will be used for matching multi-indices in the same requested batch of values. Optionally, you can set `m_max` argument that specifies the maximum cache size. If the size is exceeded, the cache will be cleared and a corresponding warning will be displayed.
+- `bm.set_cache(with_cache=False, cache=None, m_max=1.E+8)` - when calling this function with the `True` argument `with_cache`, the cache will be used, that is, all the values requested from the benchmark will be saved and when the same multi-indices are accessed again, the values will be retrieved from the cache instead of explicitly calculating the objective function. Additionally, you can optionally pass as an argument `cache` an already existing cache in the form of a dictionary (the keys are multi-indices in the form of tuples, and the values are the corresponding values of the objective function). We especially note that the cache is only used when querying benchmark values in discrete multi-indices; for requested continuous points, no cache will be used. It is also important to note that no cache will be used for matching multi-indices in the same requested batch of values. Optionally, you can set `m_max` argument that specifies the maximum cache size. If the size is exceeded, the cache will be cleared and a corresponding warning will be displayed to the log. Note that when the `bm.init` method is called, the cache is always reset to zero.
 
 - `bm.set_opts(...)` - for some benchmarks, this function may be called to set additional benchmark-specific options (please see the description of arguments in the relevant benchmark code file).
 
+> You can get all configuration options as a dictionary by the function `bm.get_config()`.
+
 ##### Computing benchmark values
 
 Now the benchmark is ready to go, and we can calculate its value in any requested discrete multi-index (a real number will be returned) or a list of its values for any requested batch of discrete multi-indices (1D numpy array of real numbers will be returned):
 ```python
 # Get value at multi-index i:
 i = np.ones(bm.d)
 print(bm[i]) # you can use the alias "bm.get(i)"
 
 # Get values for batch of multi-indices I:
 I = np.array([i, i+1, i+2])
 print(bm[I]) # you can use the alias "bm.get(I)"
 ```
 Note that the `get` method can be used instead of `[ ]` notation, for example, if it is necessary to pass somewhere a function that calculates benchmark values.
 
-Since the considered benchmark (`BmFuncAckley`) corresponds to a function of a continuous argument, above we calculated the values for the discretization of the function on a given grid. Additionally, we can calculate values at continuous points by analogy:
+Since the considered benchmark (`BmFuncAckley`) corresponds to a function of a continuous argument, above we calculated the values for the discretization of the function on a automatically selected grid. Additionally, we can calculate values at continuous points by analogy:
 ```python
 # Get value at point x:
 x = np.ones(bm.d) * 0.42
 print(bm(x)) # you can use the alias "bm.get_poi(x)"
 
 # Get values for batch of points X:
 X = np.array([x, x*0.3, x*1.1])
 print(bm(X)) # you can use the alias "bm.get_poi(X)"
 ```
 
-##### Data set generation
+##### Dataset generation
 
 For convenience, the benchmark also has functions that allow you to generate training and test data sets on a discrete grid:
 ```python
 # Generate random train dataset (from LHS):
 # I_trn is array of [500, bm.d] and y_trn is [500]
 I_trn, y_trn = bm.build_trn(500)
 
 # Generate random test dataset (from random choice):
 # I_tst is array of [100, bm.d] and y_tst of [100]
 I_tst, y_tst = bm.build_tst(100)
 ```
 
+> Note that, by default, the spent computational budget (see `bm.set_budget` function) and time spent does not change when the test dataset is generated (this is controlled by the default `skip_process` flag value in `bm.build_tst(m=0, skip_process=True)`), but is consumed when generating the training dataset (i.e., `bm.build_trn(m=0, skip_process=False)`).
+
 ##### Request history analysis
 
 During requests to the benchmark, that is, when calling functions `bm[]` (or `bm.get`), `bm()` (or `bm.get_poi`), `bm.build_trn` (if the flag `skip_process` is not set in the function arguments; it has a value `False` by default) and `bm.build_tst` (if `skip_process` is not set; it is `True` by default for this function), the following useful class parameters are updated:
 
 - `bm.m` - the total number of performed calculations of the benchmark value (if a cache is used, then the values taken from the cache are not taken into account in this variable).
 
 - `bm.m_cache` - the total number of cache hits performed instead of explicitly calculating benchmark values (if no cache is used, it is `0`).
 
 - `bm.time` - total time in seconds spent on calculating the benchmark values (the time spent on cache accesses is also taken into account).
 
+- `bm.time_full` - benchmark lifetime in seconds from the moment of initialization (i.e., the call to `bm.init` method).
+
 - `bm.y_list` - a list of all sequentially calculated benchmark values (results of cache accesses are also added to the list).
 
 - `bm.i_max`, `bm.x_max`, `bm.y_max` - a discrete multi-index, a continuous multi-dimensional point, and benchmark values corresponding to the maximum of all requested values. Note that for the case of a discrete function, the value of `x_max` will be `None`, and for the case of a continuous function, the values of `i_max` and `x_max` will correlate, while if requests were made for continuous points, then `x_max` will correspond to the exact position of the point, and `i_max` will be the nearest multi-index of the used discrete grid.
 
 - `bm.i_min`, `bm.x_min`, `bm.y_min` - same as in the previous point, but for the minimum value.
 
-The following function may be used to print the corresponding values: `print(bm.info_history())`.
+- `bm.i`, `bm.x`, `bm.y` - the last requested multi-index / point and the related computed benchmark's value.
+
+> The following function may be used to print the corresponding values: `print(bm.info_history())`. You can also get these values as a dictionary by the function `bm.get_history()`.
 
 ##### Notes
 
 - For some benchmarks (e.g., for all benchmarks from `agent` collection) the method `show` (present the current state, the state for provided input or the final state for the best found input) and `render` (present the animation for the current solution, the solution from the provided input or for the solution from the best found input) are available.
 
 
 ## Authors
```

### Comparing `teneva_bm-0.5.0/teneva_bm.egg-info/SOURCES.txt` & `teneva_bm-0.6.0/teneva_bm.egg-info/SOURCES.txt`

 * *Files 15% similar despite different names*

```diff
@@ -12,16 +12,19 @@
 teneva_bm.egg-info/SOURCES.txt
 teneva_bm.egg-info/dependency_links.txt
 teneva_bm.egg-info/requires.txt
 teneva_bm.egg-info/top_level.txt
 teneva_bm/agent/__init__.py
 teneva_bm/agent/agent.py
 teneva_bm/agent/bm_agent_ant.py
-teneva_bm/agent/bm_agent_humanoid.py
+teneva_bm/agent/bm_agent_human.py
+teneva_bm/agent/bm_agent_human_stand.py
 teneva_bm/agent/bm_agent_lake.py
+teneva_bm/agent/bm_agent_pend_inv.py
+teneva_bm/agent/bm_agent_pend_inv_double.py
 teneva_bm/agent/bm_agent_swimmer.py
 teneva_bm/agent/policy.py
 teneva_bm/func/__init__.py
 teneva_bm/func/bm_func_ackley.py
 teneva_bm/func/bm_func_alpine.py
 teneva_bm/func/bm_func_dixon.py
 teneva_bm/func/bm_func_exp.py
@@ -46,17 +49,17 @@
 teneva_bm/hs/draft_unconstrained_functions/__init__.py
 teneva_bm/hs/draft_unconstrained_functions/bm_hs002.py
 teneva_bm/hs/draft_unconstrained_functions/bm_hs003.py
 teneva_bm/hs/draft_unconstrained_functions/bm_hs004.py
 teneva_bm/hs/draft_unconstrained_functions/bm_hs005.py
 teneva_bm/hs/draft_unconstrained_functions/bm_hs038.py
 teneva_bm/hs/draft_unconstrained_functions/bm_hs045.py
-teneva_bm/oc/__init__.py
-teneva_bm/oc/bm_oc_simple.py
-teneva_bm/oc/bm_oc_simple_constr.py
+teneva_bm/odeoc/__init__.py
+teneva_bm/odeoc/bm_odeoc_simple.py
+teneva_bm/odeoc/bm_odeoc_simple_constr.py
 teneva_bm/qubo/__init__.py
 teneva_bm/qubo/bm_qubo_knap_det.py
 teneva_bm/qubo/bm_qubo_knap_quad.py
 teneva_bm/qubo/bm_qubo_maxcut.py
 teneva_bm/qubo/bm_qubo_mvc.py
 teneva_bm/various/__init__.py
 teneva_bm/various/bm_matmul.py
```

