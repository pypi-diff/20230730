# Comparing `tmp/pyDecision-4.0.9.tar.gz` & `tmp/pyDecision-4.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\pyDecision-4.0.9.tar", last modified: Tue Jul 25 22:42:25 2023, max compression
+gzip compressed data, was "dist\pyDecision-4.1.4.tar", last modified: Sat Jul 29 23:14:07 2023, max compression
```

## Comparing `pyDecision-4.0.9.tar` & `pyDecision-4.1.4.tar`

### file list

```diff
@@ -1,82 +1,85 @@
-drwxrwxrwx   0        0        0        0 2023-07-25 22:42:25.000000 pyDecision-4.0.9/
--rw-rw-rw-   0        0        0      659 2022-03-01 20:02:45.000000 pyDecision-4.0.9/LICENSE
--rw-rw-rw-   0        0        0    16271 2023-07-25 22:42:25.000000 pyDecision-4.0.9/PKG-INFO
--rw-rw-rw-   0        0        0    15858 2023-07-25 22:42:06.000000 pyDecision-4.0.9/README.md
-drwxrwxrwx   0        0        0        0 2023-07-25 22:42:25.000000 pyDecision-4.0.9/pyDecision/
--rw-rw-rw-   0        0        0        1 2022-03-01 07:37:35.000000 pyDecision-4.0.9/pyDecision/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-25 22:42:25.000000 pyDecision-4.0.9/pyDecision/algorithm/
--rw-rw-rw-   0        0        0     2379 2023-07-23 16:35:36.000000 pyDecision-4.0.9/pyDecision/algorithm/__init__.py
--rw-rw-rw-   0        0        0     1079 2023-07-21 17:12:59.000000 pyDecision-4.0.9/pyDecision/algorithm/ahp.py
--rw-rw-rw-   0        0        0     2591 2023-07-21 17:32:54.000000 pyDecision-4.0.9/pyDecision/algorithm/aras.py
--rw-rw-rw-   0        0        0     2147 2023-07-21 20:21:53.000000 pyDecision-4.0.9/pyDecision/algorithm/borda.py
--rw-rw-rw-   0        0        0     1548 2023-07-21 17:33:22.000000 pyDecision-4.0.9/pyDecision/algorithm/bwm.py
--rw-rw-rw-   0        0        0      862 2023-07-18 00:52:46.000000 pyDecision-4.0.9/pyDecision/algorithm/cilos.py
--rw-rw-rw-   0        0        0     2762 2023-07-22 02:44:56.000000 pyDecision-4.0.9/pyDecision/algorithm/cocoso.py
--rw-rw-rw-   0        0        0     2754 2023-07-21 17:33:49.000000 pyDecision-4.0.9/pyDecision/algorithm/codas.py
--rw-rw-rw-   0        0        0     2870 2023-07-23 17:00:58.000000 pyDecision-4.0.9/pyDecision/algorithm/copeland.py
--rw-rw-rw-   0        0        0     2471 2023-07-21 17:34:03.000000 pyDecision-4.0.9/pyDecision/algorithm/copras.py
--rw-rw-rw-   0        0        0     2347 2023-07-23 16:38:01.000000 pyDecision-4.0.9/pyDecision/algorithm/cradis.py
--rw-rw-rw-   0        0        0     1121 2021-04-26 20:45:47.000000 pyDecision-4.0.9/pyDecision/algorithm/critic.py
--rw-rw-rw-   0        0        0     3204 2021-02-02 00:46:00.000000 pyDecision-4.0.9/pyDecision/algorithm/dematel.py
--rw-rw-rw-   0        0        0     9331 2020-01-14 19:04:25.000000 pyDecision-4.0.9/pyDecision/algorithm/e_i.py
--rw-rw-rw-   0        0        0     9548 2020-01-13 23:26:00.000000 pyDecision-4.0.9/pyDecision/algorithm/e_i_s.py
--rw-rw-rw-   0        0        0     9225 2020-01-13 23:30:51.000000 pyDecision-4.0.9/pyDecision/algorithm/e_i_v.py
--rw-rw-rw-   0        0        0    16907 2023-07-21 20:38:15.000000 pyDecision-4.0.9/pyDecision/algorithm/e_ii.py
--rw-rw-rw-   0        0        0    13823 2020-01-13 22:04:18.000000 pyDecision-4.0.9/pyDecision/algorithm/e_iii.py
--rw-rw-rw-   0        0        0    14298 2023-07-21 19:41:40.000000 pyDecision-4.0.9/pyDecision/algorithm/e_iv.py
--rw-rw-rw-   0        0        0    14611 2020-08-10 21:53:58.000000 pyDecision-4.0.9/pyDecision/algorithm/e_tri_b.py
--rw-rw-rw-   0        0        0     2711 2023-07-21 20:33:16.000000 pyDecision-4.0.9/pyDecision/algorithm/edas.py
--rw-rw-rw-   0        0        0      925 2023-07-19 01:09:53.000000 pyDecision-4.0.9/pyDecision/algorithm/entropy.py
--rw-rw-rw-   0        0        0     1655 2022-09-01 20:46:10.000000 pyDecision-4.0.9/pyDecision/algorithm/fuzzy_ahp.py
--rw-rw-rw-   0        0        0     3321 2023-07-25 15:17:23.000000 pyDecision-4.0.9/pyDecision/algorithm/fuzzy_aras.py
--rw-rw-rw-   0        0        0     4545 2023-07-21 17:31:44.000000 pyDecision-4.0.9/pyDecision/algorithm/fuzzy_copras.py
--rw-rw-rw-   0        0        0     3930 2021-02-02 01:12:46.000000 pyDecision-4.0.9/pyDecision/algorithm/fuzzy_dematel.py
--rw-rw-rw-   0        0        0     5042 2023-07-21 18:03:22.000000 pyDecision-4.0.9/pyDecision/algorithm/fuzzy_edas.py
--rw-rw-rw-   0        0        0     3706 2023-07-21 18:11:21.000000 pyDecision-4.0.9/pyDecision/algorithm/fuzzy_moora.py
--rw-rw-rw-   0        0        0     4098 2023-07-21 18:13:14.000000 pyDecision-4.0.9/pyDecision/algorithm/fuzzy_ocra.py
--rw-rw-rw-   0        0        0     4086 2023-07-21 18:17:14.000000 pyDecision-4.0.9/pyDecision/algorithm/fuzzy_topsis.py
--rw-rw-rw-   0        0        0     5994 2023-07-21 18:18:25.000000 pyDecision-4.0.9/pyDecision/algorithm/fuzzy_vikor.py
--rw-rw-rw-   0        0        0     2553 2023-07-22 02:46:58.000000 pyDecision-4.0.9/pyDecision/algorithm/gra.py
--rw-rw-rw-   0        0        0     2617 2023-07-25 20:31:22.000000 pyDecision-4.0.9/pyDecision/algorithm/idocriw.py
--rw-rw-rw-   0        0        0     2585 2023-07-21 18:06:06.000000 pyDecision-4.0.9/pyDecision/algorithm/mabac.py
--rw-rw-rw-   0        0        0     2575 2023-07-23 16:39:11.000000 pyDecision-4.0.9/pyDecision/algorithm/mairca.py
--rw-rw-rw-   0        0        0     3048 2023-07-21 18:09:18.000000 pyDecision-4.0.9/pyDecision/algorithm/marcos.py
--rw-rw-rw-   0        0        0     3766 2023-07-22 02:46:58.000000 pyDecision-4.0.9/pyDecision/algorithm/maut.py
--rw-rw-rw-   0        0        0      965 2023-07-21 18:10:23.000000 pyDecision-4.0.9/pyDecision/algorithm/merec.py
--rw-rw-rw-   0        0        0     2541 2023-07-21 18:10:51.000000 pyDecision-4.0.9/pyDecision/algorithm/moora.py
--rw-rw-rw-   0        0        0     2549 2023-07-21 18:12:07.000000 pyDecision-4.0.9/pyDecision/algorithm/moosra.py
--rw-rw-rw-   0        0        0     4968 2023-07-22 01:50:19.000000 pyDecision-4.0.9/pyDecision/algorithm/multimoora.py
--rw-rw-rw-   0        0        0     2477 2023-07-21 23:26:24.000000 pyDecision-4.0.9/pyDecision/algorithm/ocra.py
--rw-rw-rw-   0        0        0     8518 2020-01-13 22:39:45.000000 pyDecision-4.0.9/pyDecision/algorithm/p_i.py
--rw-rw-rw-   0        0        0     5891 2023-07-21 19:40:41.000000 pyDecision-4.0.9/pyDecision/algorithm/p_ii.py
--rw-rw-rw-   0        0        0     8323 2021-01-28 15:26:38.000000 pyDecision-4.0.9/pyDecision/algorithm/p_iii.py
--rw-rw-rw-   0        0        0     8547 2023-07-21 19:39:42.000000 pyDecision-4.0.9/pyDecision/algorithm/p_iv.py
--rw-rw-rw-   0        0        0     6472 2023-07-21 19:39:01.000000 pyDecision-4.0.9/pyDecision/algorithm/p_v.py
--rw-rw-rw-   0        0        0     9380 2023-07-21 19:37:53.000000 pyDecision-4.0.9/pyDecision/algorithm/p_vi.py
--rw-rw-rw-   0        0        0     7337 2021-01-27 21:21:21.000000 pyDecision-4.0.9/pyDecision/algorithm/p_xgaia.py
--rw-rw-rw-   0        0        0     2139 2023-07-23 16:40:26.000000 pyDecision-4.0.9/pyDecision/algorithm/piv.py
--rw-rw-rw-   0        0        0     2184 2023-07-21 18:14:04.000000 pyDecision-4.0.9/pyDecision/algorithm/psi.py
--rw-rw-rw-   0        0        0     2434 2023-07-22 02:08:59.000000 pyDecision-4.0.9/pyDecision/algorithm/rov.py
--rw-rw-rw-   0        0        0     2130 2023-07-21 18:14:55.000000 pyDecision-4.0.9/pyDecision/algorithm/saw.py
--rw-rw-rw-   0        0        0     2344 2023-07-21 18:15:17.000000 pyDecision-4.0.9/pyDecision/algorithm/smart.py
--rw-rw-rw-   0        0        0     2867 2023-07-21 18:15:39.000000 pyDecision-4.0.9/pyDecision/algorithm/todim.py
--rw-rw-rw-   0        0        0     2600 2023-07-21 18:16:04.000000 pyDecision-4.0.9/pyDecision/algorithm/topsis.py
--rw-rw-rw-   0        0        0     3703 2023-07-22 03:11:26.000000 pyDecision-4.0.9/pyDecision/algorithm/vikor.py
--rw-rw-rw-   0        0        0     4242 2023-07-25 13:24:23.000000 pyDecision-4.0.9/pyDecision/algorithm/waspas.py
--rw-rw-rw-   0        0        0     2643 2023-07-21 18:23:36.000000 pyDecision-4.0.9/pyDecision/algorithm/wings.py
-drwxrwxrwx   0        0        0        0 2023-07-25 22:42:25.000000 pyDecision-4.0.9/pyDecision/compare/
--rw-rw-rw-   0        0        0       94 2023-07-25 21:52:02.000000 pyDecision-4.0.9/pyDecision/compare/__init__.py
--rw-rw-rw-   0        0        0    18196 2023-07-25 22:02:05.000000 pyDecision-4.0.9/pyDecision/compare/compare.py
-drwxrwxrwx   0        0        0        0 2023-07-25 22:42:25.000000 pyDecision-4.0.9/pyDecision/util/
--rw-rw-rw-   0        0        0     3151 2023-07-25 21:32:57.000000 pyDecision-4.0.9/pyDecision/util/LLM.py
--rw-rw-rw-   0        0        0      138 2023-07-25 21:52:24.000000 pyDecision-4.0.9/pyDecision/util/__init__.py
--rw-rw-rw-   0        0        0     6266 2023-07-21 21:06:34.000000 pyDecision-4.0.9/pyDecision/util/ga.py
--rw-rw-rw-   0        0        0     6113 2023-07-25 20:17:38.000000 pyDecision-4.0.9/pyDecision/util/gwo.py
-drwxrwxrwx   0        0        0        0 2023-07-25 22:42:25.000000 pyDecision-4.0.9/pyDecision.egg-info/
--rw-rw-rw-   0        0        0    16271 2023-07-25 22:42:24.000000 pyDecision-4.0.9/pyDecision.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     2199 2023-07-25 22:42:24.000000 pyDecision-4.0.9/pyDecision.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-25 22:42:24.000000 pyDecision-4.0.9/pyDecision.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       50 2023-07-25 22:42:24.000000 pyDecision-4.0.9/pyDecision.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2023-07-25 22:42:24.000000 pyDecision-4.0.9/pyDecision.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-07-25 22:42:25.000000 pyDecision-4.0.9/setup.cfg
--rw-rw-rw-   0        0        0      662 2023-07-25 22:42:10.000000 pyDecision-4.0.9/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-29 23:14:07.000000 pyDecision-4.1.4/
+-rw-rw-rw-   0        0        0      659 2022-03-01 20:02:45.000000 pyDecision-4.1.4/LICENSE
+-rw-rw-rw-   0        0        0    16931 2023-07-29 23:14:07.000000 pyDecision-4.1.4/PKG-INFO
+-rw-rw-rw-   0        0        0    16511 2023-07-29 22:26:13.000000 pyDecision-4.1.4/README.md
+drwxrwxrwx   0        0        0        0 2023-07-29 23:14:07.000000 pyDecision-4.1.4/pyDecision/
+-rw-rw-rw-   0        0        0        1 2022-03-01 07:37:35.000000 pyDecision-4.1.4/pyDecision/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-29 23:14:07.000000 pyDecision-4.1.4/pyDecision/algorithm/
+-rw-rw-rw-   0        0        0     2503 2023-07-29 23:13:09.000000 pyDecision-4.1.4/pyDecision/algorithm/__init__.py
+-rw-rw-rw-   0        0        0     1079 2023-07-21 17:12:59.000000 pyDecision-4.1.4/pyDecision/algorithm/ahp.py
+-rw-rw-rw-   0        0        0     2591 2023-07-21 17:32:54.000000 pyDecision-4.1.4/pyDecision/algorithm/aras.py
+-rw-rw-rw-   0        0        0     2147 2023-07-21 20:21:53.000000 pyDecision-4.1.4/pyDecision/algorithm/borda.py
+-rw-rw-rw-   0        0        0     1548 2023-07-21 17:33:22.000000 pyDecision-4.1.4/pyDecision/algorithm/bwm.py
+-rw-rw-rw-   0        0        0      862 2023-07-18 00:52:46.000000 pyDecision-4.1.4/pyDecision/algorithm/cilos.py
+-rw-rw-rw-   0        0        0     2762 2023-07-22 02:44:56.000000 pyDecision-4.1.4/pyDecision/algorithm/cocoso.py
+-rw-rw-rw-   0        0        0     2754 2023-07-21 17:33:49.000000 pyDecision-4.1.4/pyDecision/algorithm/codas.py
+-rw-rw-rw-   0        0        0     2870 2023-07-23 17:00:58.000000 pyDecision-4.1.4/pyDecision/algorithm/copeland.py
+-rw-rw-rw-   0        0        0     2471 2023-07-21 17:34:03.000000 pyDecision-4.1.4/pyDecision/algorithm/copras.py
+-rw-rw-rw-   0        0        0     2347 2023-07-23 16:38:01.000000 pyDecision-4.1.4/pyDecision/algorithm/cradis.py
+-rw-rw-rw-   0        0        0     1121 2021-04-26 20:45:47.000000 pyDecision-4.1.4/pyDecision/algorithm/critic.py
+-rw-rw-rw-   0        0        0     3204 2021-02-02 00:46:00.000000 pyDecision-4.1.4/pyDecision/algorithm/dematel.py
+-rw-rw-rw-   0        0        0     9331 2020-01-14 19:04:25.000000 pyDecision-4.1.4/pyDecision/algorithm/e_i.py
+-rw-rw-rw-   0        0        0     9548 2020-01-13 23:26:00.000000 pyDecision-4.1.4/pyDecision/algorithm/e_i_s.py
+-rw-rw-rw-   0        0        0     9225 2020-01-13 23:30:51.000000 pyDecision-4.1.4/pyDecision/algorithm/e_i_v.py
+-rw-rw-rw-   0        0        0    16907 2023-07-21 20:38:15.000000 pyDecision-4.1.4/pyDecision/algorithm/e_ii.py
+-rw-rw-rw-   0        0        0    13823 2020-01-13 22:04:18.000000 pyDecision-4.1.4/pyDecision/algorithm/e_iii.py
+-rw-rw-rw-   0        0        0    14298 2023-07-21 19:41:40.000000 pyDecision-4.1.4/pyDecision/algorithm/e_iv.py
+-rw-rw-rw-   0        0        0    14611 2020-08-10 21:53:58.000000 pyDecision-4.1.4/pyDecision/algorithm/e_tri_b.py
+-rw-rw-rw-   0        0        0     2711 2023-07-21 20:33:16.000000 pyDecision-4.1.4/pyDecision/algorithm/edas.py
+-rw-rw-rw-   0        0        0      925 2023-07-19 01:09:53.000000 pyDecision-4.1.4/pyDecision/algorithm/entropy.py
+-rw-rw-rw-   0        0        0     1655 2022-09-01 20:46:10.000000 pyDecision-4.1.4/pyDecision/algorithm/fuzzy_ahp.py
+-rw-rw-rw-   0        0        0     3321 2023-07-25 15:17:23.000000 pyDecision-4.1.4/pyDecision/algorithm/fuzzy_aras.py
+-rw-rw-rw-   0        0        0     4545 2023-07-21 17:31:44.000000 pyDecision-4.1.4/pyDecision/algorithm/fuzzy_copras.py
+-rw-rw-rw-   0        0        0     3930 2021-02-02 01:12:46.000000 pyDecision-4.1.4/pyDecision/algorithm/fuzzy_dematel.py
+-rw-rw-rw-   0        0        0     5042 2023-07-21 18:03:22.000000 pyDecision-4.1.4/pyDecision/algorithm/fuzzy_edas.py
+-rw-rw-rw-   0        0        0     3706 2023-07-21 18:11:21.000000 pyDecision-4.1.4/pyDecision/algorithm/fuzzy_moora.py
+-rw-rw-rw-   0        0        0     4098 2023-07-21 18:13:14.000000 pyDecision-4.1.4/pyDecision/algorithm/fuzzy_ocra.py
+-rw-rw-rw-   0        0        0     4086 2023-07-21 18:17:14.000000 pyDecision-4.1.4/pyDecision/algorithm/fuzzy_topsis.py
+-rw-rw-rw-   0        0        0     5994 2023-07-21 18:18:25.000000 pyDecision-4.1.4/pyDecision/algorithm/fuzzy_vikor.py
+-rw-rw-rw-   0        0        0     2553 2023-07-22 02:46:58.000000 pyDecision-4.1.4/pyDecision/algorithm/gra.py
+-rw-rw-rw-   0        0        0     2617 2023-07-25 20:31:22.000000 pyDecision-4.1.4/pyDecision/algorithm/idocriw.py
+-rw-rw-rw-   0        0        0     2585 2023-07-21 18:06:06.000000 pyDecision-4.1.4/pyDecision/algorithm/mabac.py
+-rw-rw-rw-   0        0        0     2388 2023-07-28 22:31:36.000000 pyDecision-4.1.4/pyDecision/algorithm/macbeth.py
+-rw-rw-rw-   0        0        0     2575 2023-07-23 16:39:11.000000 pyDecision-4.1.4/pyDecision/algorithm/mairca.py
+-rw-rw-rw-   0        0        0     3048 2023-07-21 18:09:18.000000 pyDecision-4.1.4/pyDecision/algorithm/marcos.py
+-rw-rw-rw-   0        0        0     3766 2023-07-22 02:46:58.000000 pyDecision-4.1.4/pyDecision/algorithm/maut.py
+-rw-rw-rw-   0        0        0      965 2023-07-21 18:10:23.000000 pyDecision-4.1.4/pyDecision/algorithm/merec.py
+-rw-rw-rw-   0        0        0     2541 2023-07-21 18:10:51.000000 pyDecision-4.1.4/pyDecision/algorithm/moora.py
+-rw-rw-rw-   0        0        0     2549 2023-07-21 18:12:07.000000 pyDecision-4.1.4/pyDecision/algorithm/moosra.py
+-rw-rw-rw-   0        0        0     4968 2023-07-22 01:50:19.000000 pyDecision-4.1.4/pyDecision/algorithm/multimoora.py
+-rw-rw-rw-   0        0        0     2477 2023-07-21 23:26:24.000000 pyDecision-4.1.4/pyDecision/algorithm/ocra.py
+-rw-rw-rw-   0        0        0     2553 2023-07-28 23:58:56.000000 pyDecision-4.1.4/pyDecision/algorithm/oreste.py
+-rw-rw-rw-   0        0        0     8518 2020-01-13 22:39:45.000000 pyDecision-4.1.4/pyDecision/algorithm/p_i.py
+-rw-rw-rw-   0        0        0     5891 2023-07-21 19:40:41.000000 pyDecision-4.1.4/pyDecision/algorithm/p_ii.py
+-rw-rw-rw-   0        0        0     8323 2021-01-28 15:26:38.000000 pyDecision-4.1.4/pyDecision/algorithm/p_iii.py
+-rw-rw-rw-   0        0        0     8547 2023-07-21 19:39:42.000000 pyDecision-4.1.4/pyDecision/algorithm/p_iv.py
+-rw-rw-rw-   0        0        0     6472 2023-07-21 19:39:01.000000 pyDecision-4.1.4/pyDecision/algorithm/p_v.py
+-rw-rw-rw-   0        0        0     9380 2023-07-21 19:37:53.000000 pyDecision-4.1.4/pyDecision/algorithm/p_vi.py
+-rw-rw-rw-   0        0        0     7337 2021-01-27 21:21:21.000000 pyDecision-4.1.4/pyDecision/algorithm/p_xgaia.py
+-rw-rw-rw-   0        0        0     2139 2023-07-23 16:40:26.000000 pyDecision-4.1.4/pyDecision/algorithm/piv.py
+-rw-rw-rw-   0        0        0     2184 2023-07-21 18:14:04.000000 pyDecision-4.1.4/pyDecision/algorithm/psi.py
+-rw-rw-rw-   0        0        0     5228 2023-07-29 11:05:11.000000 pyDecision-4.1.4/pyDecision/algorithm/regime.py
+-rw-rw-rw-   0        0        0     2434 2023-07-22 02:08:59.000000 pyDecision-4.1.4/pyDecision/algorithm/rov.py
+-rw-rw-rw-   0        0        0     2130 2023-07-21 18:14:55.000000 pyDecision-4.1.4/pyDecision/algorithm/saw.py
+-rw-rw-rw-   0        0        0     2344 2023-07-21 18:15:17.000000 pyDecision-4.1.4/pyDecision/algorithm/smart.py
+-rw-rw-rw-   0        0        0     2867 2023-07-21 18:15:39.000000 pyDecision-4.1.4/pyDecision/algorithm/todim.py
+-rw-rw-rw-   0        0        0     2600 2023-07-21 18:16:04.000000 pyDecision-4.1.4/pyDecision/algorithm/topsis.py
+-rw-rw-rw-   0        0        0     3703 2023-07-22 03:11:26.000000 pyDecision-4.1.4/pyDecision/algorithm/vikor.py
+-rw-rw-rw-   0        0        0     4242 2023-07-25 13:24:23.000000 pyDecision-4.1.4/pyDecision/algorithm/waspas.py
+-rw-rw-rw-   0        0        0     2643 2023-07-21 18:23:36.000000 pyDecision-4.1.4/pyDecision/algorithm/wings.py
+drwxrwxrwx   0        0        0        0 2023-07-29 23:14:07.000000 pyDecision-4.1.4/pyDecision/compare/
+-rw-rw-rw-   0        0        0       94 2023-07-25 21:52:02.000000 pyDecision-4.1.4/pyDecision/compare/__init__.py
+-rw-rw-rw-   0        0        0    18822 2023-07-29 22:20:55.000000 pyDecision-4.1.4/pyDecision/compare/compare.py
+drwxrwxrwx   0        0        0        0 2023-07-29 23:14:07.000000 pyDecision-4.1.4/pyDecision/util/
+-rw-rw-rw-   0        0        0     3151 2023-07-25 21:32:57.000000 pyDecision-4.1.4/pyDecision/util/LLM.py
+-rw-rw-rw-   0        0        0      138 2023-07-25 21:52:24.000000 pyDecision-4.1.4/pyDecision/util/__init__.py
+-rw-rw-rw-   0        0        0     6266 2023-07-21 21:06:34.000000 pyDecision-4.1.4/pyDecision/util/ga.py
+-rw-rw-rw-   0        0        0     6113 2023-07-25 20:17:38.000000 pyDecision-4.1.4/pyDecision/util/gwo.py
+drwxrwxrwx   0        0        0        0 2023-07-29 23:14:07.000000 pyDecision-4.1.4/pyDecision.egg-info/
+-rw-rw-rw-   0        0        0    16931 2023-07-29 23:14:06.000000 pyDecision-4.1.4/pyDecision.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     2293 2023-07-29 23:14:07.000000 pyDecision-4.1.4/pyDecision.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-29 23:14:06.000000 pyDecision-4.1.4/pyDecision.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       50 2023-07-29 23:14:06.000000 pyDecision-4.1.4/pyDecision.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2023-07-29 23:14:06.000000 pyDecision-4.1.4/pyDecision.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-29 23:14:07.000000 pyDecision-4.1.4/setup.cfg
+-rw-rw-rw-   0        0        0      662 2023-07-29 23:13:26.000000 pyDecision-4.1.4/setup.py
```

### Comparing `pyDecision-4.0.9/LICENSE` & `pyDecision-4.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `pyDecision-4.0.9/PKG-INFO` & `pyDecision-4.1.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 Metadata-Version: 2.1
 Name: pyDecision
-Version: 4.0.9
+Version: 4.1.4
 Summary: A MCDA Library
 Home-page: https://github.com/Valdecy/pyDecisions
 Author: Valdecy Pereira
 Author-email: valdecy.pereira@gmail.com
 License: GNU
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # pyDecision
 
 ## Introduction
 
-A python library with the following MCDA methods: **AHP** (Analytic Hierarchy Process); **Fuzzy AHP**; **ARAS** (Additive Ratio ASsessment); **Fuzzy ARAS**; **Borda**; **BWM** (Best-Worst Method); **CILOS** (Criterion Impact LOSs); **CoCoSo** (COmbined COmpromise SOlution); **CODAS** (Combinative Distance-based Assessment); **Copeland**; **COPRAS** (Complex PRoportional Assessment); **Fuzzy COPRAS**; **CRADIS** (Compromise Ranking of Alternatives from Distance to Ideal Solution); **CRITIC** (CRiteria Importance Through Intercriteria Correlation); **DEMATEL** (DEcision MAking Trial and Evaluation Laboratory); **Fuzzy DEMATEL**; **EDAS** (Evaluation based on Distance from Average Solution); **Fuzzy EDAS**; **Entropy**; **ELECTRE** (I, I_s, I_v, II, III, IV, Tri-B); **GRA** (Grey Relational Analysis); **IDOCRIW** (Integrated Determination of Objective CRIteria Weights); **MABAC** (Multi-Attributive Border Approximation area Comparison); **MAIRCA** (Multi-Attributive Ideal-Real Comparative Analysis); **MARCOS** (Measurement of Alternatives and Ranking according to COmpromise Solution); **MAUT** (Multi-attribute Utility Theory); **MEREC** (MEthod based on the Removal Effects of Criteria); **MOORA** (Multi-Objective Optimization on the basis of Ratio Analysis); **Fuzzy MOORA**; **MOOSRA** (Multi-Objective Optimisation on the Basis of Simple Ratio Analysis);  **MULTIMOORA** (Multi-Objective Optimization on the basis of Ratio Analisys Multiplicative Form); **OCRA** (Operational Competitiveness RAting); **Fuzzy OCRA** ; **PROMETHEE** (I, II, III, IV, V, VI, Gaia); **SAW** (Simple Additive Weighting); **SMART** (Simple Multi-Attribute Rating Technique); **TODIM** (TOmada de Decisao Interativa e Multicriterio - Interactive and Multicriteria Decision Making); **PIV** (Proximity Indexed Value); **PSI** (Preference Selection Index); **ROV** (Range Of Value); **TOPSIS** (Technique for Order of Preference by Similarity to Ideal Solution); **Fuzzy TOPSIS**; **VIKOR** (VIseKriterijumska Optimizacija I Kompromisno Resenje); **Fuzzy VIKOR**; **WINGS** (Weighted Influence Non-linear Gauge System); **WSM** (Weighted Sum Model); **WPM** (Weighted Product Model); **WASPAS** (Weighted Aggregates Sum Product Assessment).
+A python library with the following MCDA methods: **AHP** (Analytic Hierarchy Process); **Fuzzy AHP**; **ARAS** (Additive Ratio ASsessment); **Fuzzy ARAS**; **Borda**; **BWM** (Best-Worst Method); **CILOS** (Criterion Impact LOSs); **CoCoSo** (COmbined COmpromise SOlution); **CODAS** (Combinative Distance-based Assessment); **Copeland**; **COPRAS** (Complex PRoportional Assessment); **Fuzzy COPRAS**; **CRADIS** (Compromise Ranking of Alternatives from Distance to Ideal Solution); **CRITIC** (CRiteria Importance Through Intercriteria Correlation); **DEMATEL** (DEcision MAking Trial and Evaluation Laboratory); **Fuzzy DEMATEL**; **EDAS** (Evaluation based on Distance from Average Solution); **Fuzzy EDAS**; **Entropy**; **ELECTRE** (I, I_s, I_v, II, III, IV, Tri-B); **GRA** (Grey Relational Analysis); **IDOCRIW** (Integrated Determination of Objective CRIteria Weights); **MABAC** (Multi-Attributive Border Approximation area Comparison); **MACBETH** (Measuring Attractiveness by a Categorical Based Evaluation TecHnique); **MAIRCA** (Multi-Attributive Ideal-Real Comparative Analysis); **MARCOS** (Measurement of Alternatives and Ranking according to COmpromise Solution); **MAUT** (Multi-attribute Utility Theory); **MEREC** (MEthod based on the Removal Effects of Criteria); **MOORA** (Multi-Objective Optimization on the basis of Ratio Analysis); **Fuzzy MOORA**; **MOOSRA** (Multi-Objective Optimisation on the Basis of Simple Ratio Analysis);  **MULTIMOORA** (Multi-Objective Optimization on the basis of Ratio Analisys Multiplicative Form); **OCRA** (Operational Competitiveness RAting); **Fuzzy OCRA** ; **ORESTE** (Organisation Rangement Et SynThÃ¨sE de donnÃ©es relationnelles); **PROMETHEE** (I, II, III, IV, V, VI, Gaia); **SAW** (Simple Additive Weighting); **SMART** (Simple Multi-Attribute Rating Technique); **TODIM** (TOmada de Decisao Interativa e Multicriterio - Interactive and Multicriteria Decision Making); **PIV** (Proximity Indexed Value); **PSI** (Preference Selection Index); **Regime**; **ROV** (Range Of Value); **TOPSIS** (Technique for Order of Preference by Similarity to Ideal Solution); **Fuzzy TOPSIS**; **VIKOR** (VIseKriterijumska Optimizacija I Kompromisno Resenje); **Fuzzy VIKOR**; **WINGS** (Weighted Influence Non-linear Gauge System); **WSM** (Weighted Sum Model); **WPM** (Weighted Product Model); **WASPAS** (Weighted Aggregates Sum Product Assessment).
 
 pyDecision offers an array of features including the **comparison of ranking alternatives** and **comparison of criterion weights** from various methods. The library is also fully integrated with **chatGPT**, elevating result interpretation through AI. Additionally, pyDecision provides the flexibility to import results from custom methods or those not yet implemented in the library for swift comparison.
 
 ## Usage
 
 1. Install
 ```bash
@@ -75,48 +75,51 @@
 - CODAS ([ Colab Demo ](https://colab.research.google.com/drive/1hm7__urqFeBHM6nVQJcBzGPF72DFuoLr?usp=sharing)) ( [ Paper ](https://EconPapers.repec.org/RePEc:cys:ecocyb:v:50:y:2016:i:3:p:25-44))
 - Copeland ([ Colab Demo ](https://colab.research.google.com/drive/1ObP3AkQAzoCxT6et5Qkyk1trlER7mcdH?usp=sharing)) ( [ Paper ](https://link.springer.com/article/10.1007/bf01212012))
 - COPRAS ([ Colab Demo ](https://colab.research.google.com/drive/1TZJtSjXqwYEwuL7-wfLcPQ8ZBtDq3lth?usp=sharing)) ( [ Paper ](https://doi.org/10.3846/20294913.2012.762953))
 - Fuzzy COPRAS ([ Colab Demo ](https://colab.research.google.com/drive/1AIGgxBkmcA6YHKx06VeYcGf2EV8dPffW?usp=sharing)) ( [ Paper ](https://doi.org/10.1007/s00500-021-05762-w))
 - CRADIS ([ Colab Demo ](https://colab.research.google.com/drive/1p7AQmPIOsZFxaypqMsiRIWW8mIvDtoLi?usp=sharing)) ( [ Paper ](https://doi.org/10.1007%2Fs10668-021-01902-2))
 - CRITIC ([ Colab Demo ](https://colab.research.google.com/drive/1D5SaBHa1-Eo_KYSXHkFjsHYu29M21l_F?usp=sharing)) ( [ Paper ](https://doi.org/10.1016/0305-0548(94)00059-H))
 - DEMATEL ([ Colab Demo ](https://colab.research.google.com/drive/1T04qEft9uwTyQx--gADN6V_vUrT21Xo6?usp=sharing)) ( [ Paper ](https://doi.org/10.1155/2018/3696457))
-- Fuzzy DEMATEL ([ Colab Demo ](https://colab.research.google.com/drive/15e9dMDROr3cxjbWRXg3_t4TScuQtQDpR?usp=sharing)) ( [ Paper ](http://dx.doi.org/10.1016/j.eswa.2005.12.005))
+- Fuzzy DEMATEL ([ Colab Demo ](https://colab.research.google.com/drive/15e9dMDROr3cxjbWRXg3_t4TScuQtQDpR?usp=sharing)) ( [ Paper ](https://www.mdpi.com/2071-1050/9/11/2083))
 - EDAS ([ Colab Demo ](https://colab.research.google.com/drive/1xsMdwH-IH-zvOW-1kv6ztQnKGt7p5JnY?usp=sharing)) ( [ Paper ](https://doi.org/10.15388/Informatica.2015.57))
 - Fuzzy EDAS ([ Colab Demo ](https://colab.research.google.com/drive/1kw2LwztNAU9Asjj6BvBmvk11wvk8R3V6?usp=sharing)) ( [ Paper ](https://doi.org/10.1007/978-981-32-9072-3_63))
 - Entropy ([ Colab Demo ](https://colab.research.google.com/drive/1LOCef2KFxoV2qUEQRi4DqfzrgnMgtwT9?usp=sharing)) ( [ Paper ](https://people.math.harvard.edu/~ctm/home/text/others/shannon/entropy/entropy.pdf))
 - ELECTRE I     ([ Colab Demo ](https://colab.research.google.com/drive/1KFqRPBRyv-fxiu2B1y7VNkP5pCCbILF1?usp=sharing)) ( [ Paper ](https://github.com/Valdecy/Datasets/blob/master/MCDA/E01.pdf))
 - ELECTRE I_s   ([ Colab Demo ](https://colab.research.google.com/drive/1ngxsQPh2QULjd1_AifFofbukq5zIOePd?usp=sharing)) ( [ Paper ](http://dx.doi.org/10.1007/978-1-4757-5057-7_3))
 - ELECTRE I_v   ([ Colab Demo ](https://colab.research.google.com/drive/1moonq95gqXqmbRe2KvgqbN2IfowJ12C-?usp=sharing)) ( [ Paper ](http://dx.doi.org/10.1007/978-1-4757-5057-7_3))
 - ELECTRE II    ([ Colab Demo ](https://colab.research.google.com/drive/1UeAjICH6_tjVr3O9H-fC65HHYMVZgTKc?usp=sharing)) ( [ Paper ](http://dx.doi.org/10.1007/978-1-4757-5057-7_3))
 - ELECTRE III   ([ Colab Demo ](https://colab.research.google.com/drive/1smeD5ZoPgBnAAUyooAXSrkxHgqZPmUC9?usp=sharing)) ( [ Paper ](https://github.com/Valdecy/Datasets/raw/master/MCDA/E03.pdf))
 - ELECTRE IV    ([ Colab Demo ](https://colab.research.google.com/drive/178x062yC-Es6lstEiFaFprbMsTJZwnC-?usp=sharing)) ( [ Paper ](http://dx.doi.org/10.1007/978-1-4757-5057-7_3))
 - ELECTRE Tri-B ([ Colab Demo ](https://colab.research.google.com/drive/1hu0fJcxdBAiEDrVngmKQfpINpjTF-osE?usp=sharing)) ( [ Paper ](https://drive.google.com/file/d/1oWOI_sX3EEYdRbavoBTT7vUmPII1yPgE/view?usp=sharing))
 - GRA ([ Colab Demo ](https://colab.research.google.com/drive/1aMMI0Cuo5kpzTDefqEwJhf0wWpBOP_JL?usp=sharing)) ( [ Paper ](https://doi.org/10.1016/S0167-6911(82)80025-X))
 - IDOCRIW ([ Colab Demo ](https://colab.research.google.com/drive/1zt8uPFZGcHaSnpiT7tDnrDjvs0pK_7vS?usp=sharing)) ( [ Paper ](https://link.springer.com/chapter/10.1007/978-3-030-15009-9_19))
 - MABAC ([ Colab Demo ](https://colab.research.google.com/drive/1BMqO-HnBXdcOZfZoULpx1H4MLPoUGucJ?usp=sharing)) ( [ Paper ](https://doi.org/10.1016/j.eswa.2014.11.057))
+- MACBETH ([ Colab Demo ](https://colab.research.google.com/drive/1GqM9uPgbaWCGyj4l-XjkoifY2JJoVyf2?usp=sharing)) ( [ Paper ](https://link.springer.com/chapter/10.1007/978-3-030-15009-9_16))
 - MAIRCA ([ Colab Demo ](https://colab.research.google.com/drive/1gfqgrBAFGVygwm1j3lTjfy5wTsLgT_j5?usp=sharing)) ( [ Paper ](https://www.tandfonline.com/doi/full/10.1080/1331677X.2018.1506706))
 - MARCOS ([ Colab Demo ](https://colab.research.google.com/drive/13MI2Qrakm5VzHN3r5O2RqggCzQwRxCs-?usp=sharing)) ( [ Paper ](https://www.sciencedirect.com/science/article/abs/pii/S0360835219307004))
 - MAUT ([ Colab Demo ](https://colab.research.google.com/drive/1qm3ARgQm68GUK2irGiCB-B49vnVHazB7?usp=sharing)) ( [ Paper ](https://apps.dtic.mil/sti/pdfs/AD0770576.pdf))
 - MEREC ([ Colab Demo ](https://colab.research.google.com/drive/1XE3AIzS84w-gw_1MEtV7xvkU1Gj_tRPd?usp=sharing)) ( [ Paper ](https://www.mdpi.com/2073-8994/13/4/525))
 - MOORA ([ Colab Demo ](https://colab.research.google.com/drive/1FpKl0QAdwGgCVvLYsRHvMWhz7yOp17B5?usp=sharing)) ( [ Paper ](https://www.researchgate.net/publication/228345226_The_MOORA_method_and_its_application_to_privatization_in_a_transition_economy))
 - Fuzzy MOORA ([ Colab Demo ](https://colab.research.google.com/drive/1ydHzGeA8WBVY5Gyu8K7Oq6kofQ5XbK3P?usp=sharing)) ( [ Paper ](https://pdfs.semanticscholar.org/6d33/ca3f14c9ed44d23742fd4e9cf94cebcaf148.pdf))
 - MOOSRA ([ Colab Demo ](https://colab.research.google.com/drive/1KYyA4f3OsipPA5e63Ja4A0OGmHvNY6dj?usp=sharing)) ( [ Paper ](https://ijret.org/volumes/2014v03/i15/IJRET20140315105.pdf))
 - MULTIMOORA ([ Colab Demo ](https://colab.research.google.com/drive/1JAT8qqHPNoFfMV6a-CzF6BgRwtcUF3-e?usp=sharing)) ( [ Paper ](https://journals.vilniustech.lt/index.php/TEDE/article/view/5832/5078))
 - OCRA ([ Colab Demo ](https://colab.research.google.com/drive/1yQ41lOdjhiANtD1SOXoxA7gVim7A4X4P?usp=sharing)) ( [ Paper ](https://www.researchgate.net/publication/272362515_Selection_of_non-conventional_machining_processes_using_the_OCRA_method))
 - Fuzzy OCRA ([ Colab Demo ](https://colab.research.google.com/drive/1SniY4RLsR6jR9SnI3AR9k0wGlBWH6Pm8?usp=sharing)) ( [ Paper ](http://dx.doi.org/10.5755/j01.ee.30.5.20546))
+- ORESTE ([ Colab Demo ]()) ( [ Paper ](https://link.springer.com/chapter/10.1007/978-3-030-15009-9_3))
 - PROMETHEE I    ([ Colab Demo ](https://colab.research.google.com/drive/1WsagC7-Y_5X-Xl90pMz8YwUkKfxf2vol?usp=sharing)) ( [ Paper ](https://www.cin.ufpe.br/~if703/aulas/promethee.pdf))
 - PROMETHEE II   ([ Colab Demo ](https://colab.research.google.com/drive/143TUtTBy9y6gW0kMVAfhANBhuw1bKvBB?usp=sharing)) ( [ Paper ](https://www.cin.ufpe.br/~if703/aulas/promethee.pdf))
 - PROMETHEE III  ([ Colab Demo ](https://colab.research.google.com/drive/11DBaEBBT8B-B3poXubvZ41HELOHok0Rz?usp=sharing)) ( [ Paper ](http://dx.doi.org/10.1007/978-3-030-15009-9_5
 ))
 - PROMETHEE IV   ([ Colab Demo ](https://colab.research.google.com/drive/1X2evE6pIf4F7qiKjt1fSU2PqT-NaA5sJ?usp=sharing)) ( [ Paper ](http://dx.doi.org/10.1007/978-3-319-11949-6_14))
 - PROMETHEE V    ([ Colab Demo ](https://colab.research.google.com/drive/1IaZCCtq5m8vBBxrBLMCp6xB5U2j8ZNRc?usp=sharing)) ( [ Paper ](https://www.cin.ufpe.br/~if703/aulas/promethee.pdf))
 - PROMETHEE VI   ([ Colab Demo ](https://colab.research.google.com/drive/14QdhifGitj4GK-QijRr1vj_dmGU2Pfh4?usp=sharing)) ( [ Paper ](https://www.cin.ufpe.br/~if703/aulas/promethee.pdf))
 - PROMETHEE Gaia ([ Colab Demo ](https://colab.research.google.com/drive/1lj7IRKXcuRjrpoBp_KmQn_3sI3P_Qxju?usp=sharing)) ( [ Paper ](https://www.cin.ufpe.br/~if703/aulas/promethee.pdf))
 - PIV ([ Colab Demo ](https://colab.research.google.com/drive/1PwJoBqYn1O2s22MqC9euP89Uyv4sedS0?usp=sharing)) ( [ Paper ](https://www.sciencedirect.com/science/article/abs/pii/S0360835218301360))
 - PSI ([ Colab Demo ](https://colab.research.google.com/drive/1u9tN8cYl2mx6KK6yLW2oz6fuVoy8xcCI?usp=sharing)) ( [ Paper ](https://www.sciencedirect.com/science/article/abs/pii/S0261306909006396))
+- Regime ([ Colab Demo ](https://colab.research.google.com/drive/1jcAcjAS92rxvE2urhc6HPixvzJ60HqEg?usp=sharing)) ( [ Paper ](https://link.springer.com/chapter/10.1007/978-3-030-15009-9_2))
 - ROV ([ Colab Demo ](https://colab.research.google.com/drive/1sQAPCem0pcS29uf6-n4TpncXMXNx9JDh?usp=sharing)) ( [ Paper ](https://doi.org/10.5267/j.dsl.2015.12.001))
 - SAW ([ Colab Demo ](https://colab.research.google.com/drive/1R4cIsu0jBP9-6zwww_bNxEEnVGrhnS2d?usp=sharing)) ( [ Paper ](https://media.neliti.com/media/publications/326766-simple-additive-weighting-saw-method-in-f8f093e8.pdf))
 - SMART ([ Colab Demo ](https://colab.research.google.com/drive/1K93HXHBR_v2da95Hh_CB6AmTCqta-k3D?usp=sharing)) ( [ Paper ](https://doi.org/10.1007/978-1-4612-3982-6_4))
 - TODIM ([ Colab Demo ](https://colab.research.google.com/drive/1EQqhhBQHHb8HT0TfuuVeFA2kwezsQYT1?usp=sharing)) ( [ Paper ](https://www.sciencedirect.com/science/article/abs/pii/S0377221707010740))
 - TOPSIS ([ Colab Demo ](https://colab.research.google.com/drive/1s87DC5_oa9GvgVe98oAP1UIhduac09CB?usp=sharing)) ( [ Paper ](https://doi.org/10.1057/jors.1987.44))
 - Fuzzy TOPSIS ([ Colab Demo ](https://colab.research.google.com/drive/1eKx7AOYrnG-kZcsBt28rMEtCrUO-j3J-?usp=sharing)) ( [ Paper ](https://doi.org/10.1016/j.procs.2016.07.088))
 - VIKOR ([ Colab Demo ](https://colab.research.google.com/drive/1egZiTNvI2eE-tyJ2m85MM6B3-qhiSjPG?usp=sharing)) ( [ Paper ](https://doi.org/10.1007/978-981-33-4745-8_8))
```

### Comparing `pyDecision-4.0.9/README.md` & `pyDecision-4.1.4/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # pyDecision
 
 ## Introduction
 
-A python library with the following MCDA methods: **AHP** (Analytic Hierarchy Process); **Fuzzy AHP**; **ARAS** (Additive Ratio ASsessment); **Fuzzy ARAS**; **Borda**; **BWM** (Best-Worst Method); **CILOS** (Criterion Impact LOSs); **CoCoSo** (COmbined COmpromise SOlution); **CODAS** (Combinative Distance-based Assessment); **Copeland**; **COPRAS** (Complex PRoportional Assessment); **Fuzzy COPRAS**; **CRADIS** (Compromise Ranking of Alternatives from Distance to Ideal Solution); **CRITIC** (CRiteria Importance Through Intercriteria Correlation); **DEMATEL** (DEcision MAking Trial and Evaluation Laboratory); **Fuzzy DEMATEL**; **EDAS** (Evaluation based on Distance from Average Solution); **Fuzzy EDAS**; **Entropy**; **ELECTRE** (I, I_s, I_v, II, III, IV, Tri-B); **GRA** (Grey Relational Analysis); **IDOCRIW** (Integrated Determination of Objective CRIteria Weights); **MABAC** (Multi-Attributive Border Approximation area Comparison); **MAIRCA** (Multi-Attributive Ideal-Real Comparative Analysis); **MARCOS** (Measurement of Alternatives and Ranking according to COmpromise Solution); **MAUT** (Multi-attribute Utility Theory); **MEREC** (MEthod based on the Removal Effects of Criteria); **MOORA** (Multi-Objective Optimization on the basis of Ratio Analysis); **Fuzzy MOORA**; **MOOSRA** (Multi-Objective Optimisation on the Basis of Simple Ratio Analysis);  **MULTIMOORA** (Multi-Objective Optimization on the basis of Ratio Analisys Multiplicative Form); **OCRA** (Operational Competitiveness RAting); **Fuzzy OCRA** ; **PROMETHEE** (I, II, III, IV, V, VI, Gaia); **SAW** (Simple Additive Weighting); **SMART** (Simple Multi-Attribute Rating Technique); **TODIM** (TOmada de Decisao Interativa e Multicriterio - Interactive and Multicriteria Decision Making); **PIV** (Proximity Indexed Value); **PSI** (Preference Selection Index); **ROV** (Range Of Value); **TOPSIS** (Technique for Order of Preference by Similarity to Ideal Solution); **Fuzzy TOPSIS**; **VIKOR** (VIseKriterijumska Optimizacija I Kompromisno Resenje); **Fuzzy VIKOR**; **WINGS** (Weighted Influence Non-linear Gauge System); **WSM** (Weighted Sum Model); **WPM** (Weighted Product Model); **WASPAS** (Weighted Aggregates Sum Product Assessment).
+A python library with the following MCDA methods: **AHP** (Analytic Hierarchy Process); **Fuzzy AHP**; **ARAS** (Additive Ratio ASsessment); **Fuzzy ARAS**; **Borda**; **BWM** (Best-Worst Method); **CILOS** (Criterion Impact LOSs); **CoCoSo** (COmbined COmpromise SOlution); **CODAS** (Combinative Distance-based Assessment); **Copeland**; **COPRAS** (Complex PRoportional Assessment); **Fuzzy COPRAS**; **CRADIS** (Compromise Ranking of Alternatives from Distance to Ideal Solution); **CRITIC** (CRiteria Importance Through Intercriteria Correlation); **DEMATEL** (DEcision MAking Trial and Evaluation Laboratory); **Fuzzy DEMATEL**; **EDAS** (Evaluation based on Distance from Average Solution); **Fuzzy EDAS**; **Entropy**; **ELECTRE** (I, I_s, I_v, II, III, IV, Tri-B); **GRA** (Grey Relational Analysis); **IDOCRIW** (Integrated Determination of Objective CRIteria Weights); **MABAC** (Multi-Attributive Border Approximation area Comparison); **MACBETH** (Measuring Attractiveness by a Categorical Based Evaluation TecHnique); **MAIRCA** (Multi-Attributive Ideal-Real Comparative Analysis); **MARCOS** (Measurement of Alternatives and Ranking according to COmpromise Solution); **MAUT** (Multi-attribute Utility Theory); **MEREC** (MEthod based on the Removal Effects of Criteria); **MOORA** (Multi-Objective Optimization on the basis of Ratio Analysis); **Fuzzy MOORA**; **MOOSRA** (Multi-Objective Optimisation on the Basis of Simple Ratio Analysis);  **MULTIMOORA** (Multi-Objective Optimization on the basis of Ratio Analisys Multiplicative Form); **OCRA** (Operational Competitiveness RAting); **Fuzzy OCRA** ; **ORESTE** (Organisation Rangement Et SynThèsE de données relationnelles); **PROMETHEE** (I, II, III, IV, V, VI, Gaia); **SAW** (Simple Additive Weighting); **SMART** (Simple Multi-Attribute Rating Technique); **TODIM** (TOmada de Decisao Interativa e Multicriterio - Interactive and Multicriteria Decision Making); **PIV** (Proximity Indexed Value); **PSI** (Preference Selection Index); **Regime**; **ROV** (Range Of Value); **TOPSIS** (Technique for Order of Preference by Similarity to Ideal Solution); **Fuzzy TOPSIS**; **VIKOR** (VIseKriterijumska Optimizacija I Kompromisno Resenje); **Fuzzy VIKOR**; **WINGS** (Weighted Influence Non-linear Gauge System); **WSM** (Weighted Sum Model); **WPM** (Weighted Product Model); **WASPAS** (Weighted Aggregates Sum Product Assessment).
 
 pyDecision offers an array of features including the **comparison of ranking alternatives** and **comparison of criterion weights** from various methods. The library is also fully integrated with **chatGPT**, elevating result interpretation through AI. Additionally, pyDecision provides the flexibility to import results from custom methods or those not yet implemented in the library for swift comparison.
 
 ## Usage
 
 1. Install
 ```bash
@@ -64,48 +64,51 @@
 - CODAS ([ Colab Demo ](https://colab.research.google.com/drive/1hm7__urqFeBHM6nVQJcBzGPF72DFuoLr?usp=sharing)) ( [ Paper ](https://EconPapers.repec.org/RePEc:cys:ecocyb:v:50:y:2016:i:3:p:25-44))
 - Copeland ([ Colab Demo ](https://colab.research.google.com/drive/1ObP3AkQAzoCxT6et5Qkyk1trlER7mcdH?usp=sharing)) ( [ Paper ](https://link.springer.com/article/10.1007/bf01212012))
 - COPRAS ([ Colab Demo ](https://colab.research.google.com/drive/1TZJtSjXqwYEwuL7-wfLcPQ8ZBtDq3lth?usp=sharing)) ( [ Paper ](https://doi.org/10.3846/20294913.2012.762953))
 - Fuzzy COPRAS ([ Colab Demo ](https://colab.research.google.com/drive/1AIGgxBkmcA6YHKx06VeYcGf2EV8dPffW?usp=sharing)) ( [ Paper ](https://doi.org/10.1007/s00500-021-05762-w))
 - CRADIS ([ Colab Demo ](https://colab.research.google.com/drive/1p7AQmPIOsZFxaypqMsiRIWW8mIvDtoLi?usp=sharing)) ( [ Paper ](https://doi.org/10.1007%2Fs10668-021-01902-2))
 - CRITIC ([ Colab Demo ](https://colab.research.google.com/drive/1D5SaBHa1-Eo_KYSXHkFjsHYu29M21l_F?usp=sharing)) ( [ Paper ](https://doi.org/10.1016/0305-0548(94)00059-H))
 - DEMATEL ([ Colab Demo ](https://colab.research.google.com/drive/1T04qEft9uwTyQx--gADN6V_vUrT21Xo6?usp=sharing)) ( [ Paper ](https://doi.org/10.1155/2018/3696457))
-- Fuzzy DEMATEL ([ Colab Demo ](https://colab.research.google.com/drive/15e9dMDROr3cxjbWRXg3_t4TScuQtQDpR?usp=sharing)) ( [ Paper ](http://dx.doi.org/10.1016/j.eswa.2005.12.005))
+- Fuzzy DEMATEL ([ Colab Demo ](https://colab.research.google.com/drive/15e9dMDROr3cxjbWRXg3_t4TScuQtQDpR?usp=sharing)) ( [ Paper ](https://www.mdpi.com/2071-1050/9/11/2083))
 - EDAS ([ Colab Demo ](https://colab.research.google.com/drive/1xsMdwH-IH-zvOW-1kv6ztQnKGt7p5JnY?usp=sharing)) ( [ Paper ](https://doi.org/10.15388/Informatica.2015.57))
 - Fuzzy EDAS ([ Colab Demo ](https://colab.research.google.com/drive/1kw2LwztNAU9Asjj6BvBmvk11wvk8R3V6?usp=sharing)) ( [ Paper ](https://doi.org/10.1007/978-981-32-9072-3_63))
 - Entropy ([ Colab Demo ](https://colab.research.google.com/drive/1LOCef2KFxoV2qUEQRi4DqfzrgnMgtwT9?usp=sharing)) ( [ Paper ](https://people.math.harvard.edu/~ctm/home/text/others/shannon/entropy/entropy.pdf))
 - ELECTRE I     ([ Colab Demo ](https://colab.research.google.com/drive/1KFqRPBRyv-fxiu2B1y7VNkP5pCCbILF1?usp=sharing)) ( [ Paper ](https://github.com/Valdecy/Datasets/blob/master/MCDA/E01.pdf))
 - ELECTRE I_s   ([ Colab Demo ](https://colab.research.google.com/drive/1ngxsQPh2QULjd1_AifFofbukq5zIOePd?usp=sharing)) ( [ Paper ](http://dx.doi.org/10.1007/978-1-4757-5057-7_3))
 - ELECTRE I_v   ([ Colab Demo ](https://colab.research.google.com/drive/1moonq95gqXqmbRe2KvgqbN2IfowJ12C-?usp=sharing)) ( [ Paper ](http://dx.doi.org/10.1007/978-1-4757-5057-7_3))
 - ELECTRE II    ([ Colab Demo ](https://colab.research.google.com/drive/1UeAjICH6_tjVr3O9H-fC65HHYMVZgTKc?usp=sharing)) ( [ Paper ](http://dx.doi.org/10.1007/978-1-4757-5057-7_3))
 - ELECTRE III   ([ Colab Demo ](https://colab.research.google.com/drive/1smeD5ZoPgBnAAUyooAXSrkxHgqZPmUC9?usp=sharing)) ( [ Paper ](https://github.com/Valdecy/Datasets/raw/master/MCDA/E03.pdf))
 - ELECTRE IV    ([ Colab Demo ](https://colab.research.google.com/drive/178x062yC-Es6lstEiFaFprbMsTJZwnC-?usp=sharing)) ( [ Paper ](http://dx.doi.org/10.1007/978-1-4757-5057-7_3))
 - ELECTRE Tri-B ([ Colab Demo ](https://colab.research.google.com/drive/1hu0fJcxdBAiEDrVngmKQfpINpjTF-osE?usp=sharing)) ( [ Paper ](https://drive.google.com/file/d/1oWOI_sX3EEYdRbavoBTT7vUmPII1yPgE/view?usp=sharing))
 - GRA ([ Colab Demo ](https://colab.research.google.com/drive/1aMMI0Cuo5kpzTDefqEwJhf0wWpBOP_JL?usp=sharing)) ( [ Paper ](https://doi.org/10.1016/S0167-6911(82)80025-X))
 - IDOCRIW ([ Colab Demo ](https://colab.research.google.com/drive/1zt8uPFZGcHaSnpiT7tDnrDjvs0pK_7vS?usp=sharing)) ( [ Paper ](https://link.springer.com/chapter/10.1007/978-3-030-15009-9_19))
 - MABAC ([ Colab Demo ](https://colab.research.google.com/drive/1BMqO-HnBXdcOZfZoULpx1H4MLPoUGucJ?usp=sharing)) ( [ Paper ](https://doi.org/10.1016/j.eswa.2014.11.057))
+- MACBETH ([ Colab Demo ](https://colab.research.google.com/drive/1GqM9uPgbaWCGyj4l-XjkoifY2JJoVyf2?usp=sharing)) ( [ Paper ](https://link.springer.com/chapter/10.1007/978-3-030-15009-9_16))
 - MAIRCA ([ Colab Demo ](https://colab.research.google.com/drive/1gfqgrBAFGVygwm1j3lTjfy5wTsLgT_j5?usp=sharing)) ( [ Paper ](https://www.tandfonline.com/doi/full/10.1080/1331677X.2018.1506706))
 - MARCOS ([ Colab Demo ](https://colab.research.google.com/drive/13MI2Qrakm5VzHN3r5O2RqggCzQwRxCs-?usp=sharing)) ( [ Paper ](https://www.sciencedirect.com/science/article/abs/pii/S0360835219307004))
 - MAUT ([ Colab Demo ](https://colab.research.google.com/drive/1qm3ARgQm68GUK2irGiCB-B49vnVHazB7?usp=sharing)) ( [ Paper ](https://apps.dtic.mil/sti/pdfs/AD0770576.pdf))
 - MEREC ([ Colab Demo ](https://colab.research.google.com/drive/1XE3AIzS84w-gw_1MEtV7xvkU1Gj_tRPd?usp=sharing)) ( [ Paper ](https://www.mdpi.com/2073-8994/13/4/525))
 - MOORA ([ Colab Demo ](https://colab.research.google.com/drive/1FpKl0QAdwGgCVvLYsRHvMWhz7yOp17B5?usp=sharing)) ( [ Paper ](https://www.researchgate.net/publication/228345226_The_MOORA_method_and_its_application_to_privatization_in_a_transition_economy))
 - Fuzzy MOORA ([ Colab Demo ](https://colab.research.google.com/drive/1ydHzGeA8WBVY5Gyu8K7Oq6kofQ5XbK3P?usp=sharing)) ( [ Paper ](https://pdfs.semanticscholar.org/6d33/ca3f14c9ed44d23742fd4e9cf94cebcaf148.pdf))
 - MOOSRA ([ Colab Demo ](https://colab.research.google.com/drive/1KYyA4f3OsipPA5e63Ja4A0OGmHvNY6dj?usp=sharing)) ( [ Paper ](https://ijret.org/volumes/2014v03/i15/IJRET20140315105.pdf))
 - MULTIMOORA ([ Colab Demo ](https://colab.research.google.com/drive/1JAT8qqHPNoFfMV6a-CzF6BgRwtcUF3-e?usp=sharing)) ( [ Paper ](https://journals.vilniustech.lt/index.php/TEDE/article/view/5832/5078))
 - OCRA ([ Colab Demo ](https://colab.research.google.com/drive/1yQ41lOdjhiANtD1SOXoxA7gVim7A4X4P?usp=sharing)) ( [ Paper ](https://www.researchgate.net/publication/272362515_Selection_of_non-conventional_machining_processes_using_the_OCRA_method))
 - Fuzzy OCRA ([ Colab Demo ](https://colab.research.google.com/drive/1SniY4RLsR6jR9SnI3AR9k0wGlBWH6Pm8?usp=sharing)) ( [ Paper ](http://dx.doi.org/10.5755/j01.ee.30.5.20546))
+- ORESTE ([ Colab Demo ]()) ( [ Paper ](https://link.springer.com/chapter/10.1007/978-3-030-15009-9_3))
 - PROMETHEE I    ([ Colab Demo ](https://colab.research.google.com/drive/1WsagC7-Y_5X-Xl90pMz8YwUkKfxf2vol?usp=sharing)) ( [ Paper ](https://www.cin.ufpe.br/~if703/aulas/promethee.pdf))
 - PROMETHEE II   ([ Colab Demo ](https://colab.research.google.com/drive/143TUtTBy9y6gW0kMVAfhANBhuw1bKvBB?usp=sharing)) ( [ Paper ](https://www.cin.ufpe.br/~if703/aulas/promethee.pdf))
 - PROMETHEE III  ([ Colab Demo ](https://colab.research.google.com/drive/11DBaEBBT8B-B3poXubvZ41HELOHok0Rz?usp=sharing)) ( [ Paper ](http://dx.doi.org/10.1007/978-3-030-15009-9_5
 ))
 - PROMETHEE IV   ([ Colab Demo ](https://colab.research.google.com/drive/1X2evE6pIf4F7qiKjt1fSU2PqT-NaA5sJ?usp=sharing)) ( [ Paper ](http://dx.doi.org/10.1007/978-3-319-11949-6_14))
 - PROMETHEE V    ([ Colab Demo ](https://colab.research.google.com/drive/1IaZCCtq5m8vBBxrBLMCp6xB5U2j8ZNRc?usp=sharing)) ( [ Paper ](https://www.cin.ufpe.br/~if703/aulas/promethee.pdf))
 - PROMETHEE VI   ([ Colab Demo ](https://colab.research.google.com/drive/14QdhifGitj4GK-QijRr1vj_dmGU2Pfh4?usp=sharing)) ( [ Paper ](https://www.cin.ufpe.br/~if703/aulas/promethee.pdf))
 - PROMETHEE Gaia ([ Colab Demo ](https://colab.research.google.com/drive/1lj7IRKXcuRjrpoBp_KmQn_3sI3P_Qxju?usp=sharing)) ( [ Paper ](https://www.cin.ufpe.br/~if703/aulas/promethee.pdf))
 - PIV ([ Colab Demo ](https://colab.research.google.com/drive/1PwJoBqYn1O2s22MqC9euP89Uyv4sedS0?usp=sharing)) ( [ Paper ](https://www.sciencedirect.com/science/article/abs/pii/S0360835218301360))
 - PSI ([ Colab Demo ](https://colab.research.google.com/drive/1u9tN8cYl2mx6KK6yLW2oz6fuVoy8xcCI?usp=sharing)) ( [ Paper ](https://www.sciencedirect.com/science/article/abs/pii/S0261306909006396))
+- Regime ([ Colab Demo ](https://colab.research.google.com/drive/1jcAcjAS92rxvE2urhc6HPixvzJ60HqEg?usp=sharing)) ( [ Paper ](https://link.springer.com/chapter/10.1007/978-3-030-15009-9_2))
 - ROV ([ Colab Demo ](https://colab.research.google.com/drive/1sQAPCem0pcS29uf6-n4TpncXMXNx9JDh?usp=sharing)) ( [ Paper ](https://doi.org/10.5267/j.dsl.2015.12.001))
 - SAW ([ Colab Demo ](https://colab.research.google.com/drive/1R4cIsu0jBP9-6zwww_bNxEEnVGrhnS2d?usp=sharing)) ( [ Paper ](https://media.neliti.com/media/publications/326766-simple-additive-weighting-saw-method-in-f8f093e8.pdf))
 - SMART ([ Colab Demo ](https://colab.research.google.com/drive/1K93HXHBR_v2da95Hh_CB6AmTCqta-k3D?usp=sharing)) ( [ Paper ](https://doi.org/10.1007/978-1-4612-3982-6_4))
 - TODIM ([ Colab Demo ](https://colab.research.google.com/drive/1EQqhhBQHHb8HT0TfuuVeFA2kwezsQYT1?usp=sharing)) ( [ Paper ](https://www.sciencedirect.com/science/article/abs/pii/S0377221707010740))
 - TOPSIS ([ Colab Demo ](https://colab.research.google.com/drive/1s87DC5_oa9GvgVe98oAP1UIhduac09CB?usp=sharing)) ( [ Paper ](https://doi.org/10.1057/jors.1987.44))
 - Fuzzy TOPSIS ([ Colab Demo ](https://colab.research.google.com/drive/1eKx7AOYrnG-kZcsBt28rMEtCrUO-j3J-?usp=sharing)) ( [ Paper ](https://doi.org/10.1016/j.procs.2016.07.088))
 - VIKOR ([ Colab Demo ](https://colab.research.google.com/drive/1egZiTNvI2eE-tyJ2m85MM6B3-qhiSjPG?usp=sharing)) ( [ Paper ](https://doi.org/10.1007/978-981-33-4745-8_8))
```

### Comparing `pyDecision-4.0.9/pyDecision/algorithm/__init__.py` & `pyDecision-4.1.4/pyDecision/algorithm/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -27,31 +27,34 @@
 from .fuzzy_moora   import fuzzy_moora_method
 from .fuzzy_ocra    import fuzzy_ocra_method
 from .fuzzy_topsis  import fuzzy_topsis_method
 from .fuzzy_vikor   import fuzzy_vikor_method
 from .gra           import gra_method
 from .idocriw       import idocriw_method
 from .mabac         import mabac_method
+from .macbeth       import macbeth_method
 from .mairca        import mairca_method
 from .marcos        import marcos_method
 from .maut          import maut_method
 from .merec         import merec_method
 from .moora         import moora_method
 from .moosra        import moosra_method
 from .multimoora    import multimoora_method  
 from .ocra          import ocra_method
+from .oreste        import oreste_method
 from .p_i           import promethee_i
 from .p_ii          import promethee_ii
 from .p_iii         import promethee_iii
 from .p_iv          import promethee_iv
 from .p_v           import promethee_v
 from .p_vi          import promethee_vi
 from .p_xgaia       import promethee_gaia
 from .piv           import piv_method
 from .psi           import psi_method
+from .regime        import regime_method
 from .rov           import rov_method
 from .saw           import saw_method
 from .smart         import smart_method
 from .todim         import todim_method
 from .topsis        import topsis_method
 from .vikor         import vikor_method, ranking
 from .waspas        import waspas_method
```

### Comparing `pyDecision-4.0.9/pyDecision/algorithm/ahp.py` & `pyDecision-4.1.4/pyDecision/algorithm/ahp.py`

 * *Files identical despite different names*

### Comparing `pyDecision-4.0.9/pyDecision/algorithm/aras.py` & `pyDecision-4.1.4/pyDecision/algorithm/aras.py`

 * *Files identical despite different names*

### Comparing `pyDecision-4.0.9/pyDecision/algorithm/borda.py` & `pyDecision-4.1.4/pyDecision/algorithm/borda.py`

 * *Files identical despite different names*

### Comparing `pyDecision-4.0.9/pyDecision/algorithm/bwm.py` & `pyDecision-4.1.4/pyDecision/algorithm/bwm.py`

 * *Files identical despite different names*

### Comparing `pyDecision-4.0.9/pyDecision/algorithm/cilos.py` & `pyDecision-4.1.4/pyDecision/algorithm/cilos.py`

 * *Files identical despite different names*

### Comparing `pyDecision-4.0.9/pyDecision/algorithm/cocoso.py` & `pyDecision-4.1.4/pyDecision/algorithm/cocoso.py`

 * *Files identical despite different names*

### Comparing `pyDecision-4.0.9/pyDecision/algorithm/codas.py` & `pyDecision-4.1.4/pyDecision/algorithm/codas.py`

 * *Files identical despite different names*

### Comparing `pyDecision-4.0.9/pyDecision/algorithm/copeland.py` & `pyDecision-4.1.4/pyDecision/algorithm/copeland.py`

 * *Files identical despite different names*

### Comparing `pyDecision-4.0.9/pyDecision/algorithm/copras.py` & `pyDecision-4.1.4/pyDecision/algorithm/copras.py`

 * *Files identical despite different names*

### Comparing `pyDecision-4.0.9/pyDecision/algorithm/cradis.py` & `pyDecision-4.1.4/pyDecision/algorithm/cradis.py`

 * *Files identical despite different names*

### Comparing `pyDecision-4.0.9/pyDecision/algorithm/critic.py` & `pyDecision-4.1.4/pyDecision/algorithm/critic.py`

 * *Files identical despite different names*

### Comparing `pyDecision-4.0.9/pyDecision/algorithm/dematel.py` & `pyDecision-4.1.4/pyDecision/algorithm/dematel.py`

 * *Files identical despite different names*

### Comparing `pyDecision-4.0.9/pyDecision/algorithm/e_i.py` & `pyDecision-4.1.4/pyDecision/algorithm/e_i.py`

 * *Files identical despite different names*

### Comparing `pyDecision-4.0.9/pyDecision/algorithm/e_i_s.py` & `pyDecision-4.1.4/pyDecision/algorithm/e_i_s.py`

 * *Files identical despite different names*

### Comparing `pyDecision-4.0.9/pyDecision/algorithm/e_i_v.py` & `pyDecision-4.1.4/pyDecision/algorithm/e_i_v.py`

 * *Files identical despite different names*

### Comparing `pyDecision-4.0.9/pyDecision/algorithm/e_ii.py` & `pyDecision-4.1.4/pyDecision/algorithm/e_ii.py`

 * *Files identical despite different names*

### Comparing `pyDecision-4.0.9/pyDecision/algorithm/e_iii.py` & `pyDecision-4.1.4/pyDecision/algorithm/e_iii.py`

 * *Files identical despite different names*

### Comparing `pyDecision-4.0.9/pyDecision/algorithm/e_iv.py` & `pyDecision-4.1.4/pyDecision/algorithm/e_iv.py`

 * *Files identical despite different names*

### Comparing `pyDecision-4.0.9/pyDecision/algorithm/e_tri_b.py` & `pyDecision-4.1.4/pyDecision/algorithm/e_tri_b.py`

 * *Files identical despite different names*

### Comparing `pyDecision-4.0.9/pyDecision/algorithm/edas.py` & `pyDecision-4.1.4/pyDecision/algorithm/edas.py`

 * *Files identical despite different names*

### Comparing `pyDecision-4.0.9/pyDecision/algorithm/entropy.py` & `pyDecision-4.1.4/pyDecision/algorithm/entropy.py`

 * *Files identical despite different names*

### Comparing `pyDecision-4.0.9/pyDecision/algorithm/fuzzy_ahp.py` & `pyDecision-4.1.4/pyDecision/algorithm/fuzzy_ahp.py`

 * *Files identical despite different names*

### Comparing `pyDecision-4.0.9/pyDecision/algorithm/fuzzy_aras.py` & `pyDecision-4.1.4/pyDecision/algorithm/fuzzy_aras.py`

 * *Files identical despite different names*

### Comparing `pyDecision-4.0.9/pyDecision/algorithm/fuzzy_copras.py` & `pyDecision-4.1.4/pyDecision/algorithm/fuzzy_copras.py`

 * *Files identical despite different names*

### Comparing `pyDecision-4.0.9/pyDecision/algorithm/fuzzy_dematel.py` & `pyDecision-4.1.4/pyDecision/algorithm/fuzzy_dematel.py`

 * *Files identical despite different names*

### Comparing `pyDecision-4.0.9/pyDecision/algorithm/fuzzy_edas.py` & `pyDecision-4.1.4/pyDecision/algorithm/fuzzy_edas.py`

 * *Files identical despite different names*

### Comparing `pyDecision-4.0.9/pyDecision/algorithm/fuzzy_moora.py` & `pyDecision-4.1.4/pyDecision/algorithm/fuzzy_moora.py`

 * *Files identical despite different names*

### Comparing `pyDecision-4.0.9/pyDecision/algorithm/fuzzy_ocra.py` & `pyDecision-4.1.4/pyDecision/algorithm/fuzzy_ocra.py`

 * *Files identical despite different names*

### Comparing `pyDecision-4.0.9/pyDecision/algorithm/fuzzy_topsis.py` & `pyDecision-4.1.4/pyDecision/algorithm/fuzzy_topsis.py`

 * *Files identical despite different names*

### Comparing `pyDecision-4.0.9/pyDecision/algorithm/fuzzy_vikor.py` & `pyDecision-4.1.4/pyDecision/algorithm/fuzzy_vikor.py`

 * *Files identical despite different names*

### Comparing `pyDecision-4.0.9/pyDecision/algorithm/gra.py` & `pyDecision-4.1.4/pyDecision/algorithm/gra.py`

 * *Files identical despite different names*

### Comparing `pyDecision-4.0.9/pyDecision/algorithm/idocriw.py` & `pyDecision-4.1.4/pyDecision/algorithm/idocriw.py`

 * *Files identical despite different names*

### Comparing `pyDecision-4.0.9/pyDecision/algorithm/mabac.py` & `pyDecision-4.1.4/pyDecision/algorithm/mabac.py`

 * *Files identical despite different names*

### Comparing `pyDecision-4.0.9/pyDecision/algorithm/mairca.py` & `pyDecision-4.1.4/pyDecision/algorithm/mairca.py`

 * *Files identical despite different names*

### Comparing `pyDecision-4.0.9/pyDecision/algorithm/marcos.py` & `pyDecision-4.1.4/pyDecision/algorithm/marcos.py`

 * *Files identical despite different names*

### Comparing `pyDecision-4.0.9/pyDecision/algorithm/maut.py` & `pyDecision-4.1.4/pyDecision/algorithm/maut.py`

 * *Files identical despite different names*

### Comparing `pyDecision-4.0.9/pyDecision/algorithm/merec.py` & `pyDecision-4.1.4/pyDecision/algorithm/merec.py`

 * *Files identical despite different names*

### Comparing `pyDecision-4.0.9/pyDecision/algorithm/moora.py` & `pyDecision-4.1.4/pyDecision/algorithm/moora.py`

 * *Files identical despite different names*

### Comparing `pyDecision-4.0.9/pyDecision/algorithm/moosra.py` & `pyDecision-4.1.4/pyDecision/algorithm/moosra.py`

 * *Files identical despite different names*

### Comparing `pyDecision-4.0.9/pyDecision/algorithm/multimoora.py` & `pyDecision-4.1.4/pyDecision/algorithm/multimoora.py`

 * *Files identical despite different names*

### Comparing `pyDecision-4.0.9/pyDecision/algorithm/ocra.py` & `pyDecision-4.1.4/pyDecision/algorithm/ocra.py`

 * *Files identical despite different names*

### Comparing `pyDecision-4.0.9/pyDecision/algorithm/p_i.py` & `pyDecision-4.1.4/pyDecision/algorithm/p_i.py`

 * *Files identical despite different names*

### Comparing `pyDecision-4.0.9/pyDecision/algorithm/p_ii.py` & `pyDecision-4.1.4/pyDecision/algorithm/p_ii.py`

 * *Files identical despite different names*

### Comparing `pyDecision-4.0.9/pyDecision/algorithm/p_iii.py` & `pyDecision-4.1.4/pyDecision/algorithm/p_iii.py`

 * *Files identical despite different names*

### Comparing `pyDecision-4.0.9/pyDecision/algorithm/p_iv.py` & `pyDecision-4.1.4/pyDecision/algorithm/p_iv.py`

 * *Files identical despite different names*

### Comparing `pyDecision-4.0.9/pyDecision/algorithm/p_v.py` & `pyDecision-4.1.4/pyDecision/algorithm/p_v.py`

 * *Files identical despite different names*

### Comparing `pyDecision-4.0.9/pyDecision/algorithm/p_vi.py` & `pyDecision-4.1.4/pyDecision/algorithm/p_vi.py`

 * *Files identical despite different names*

### Comparing `pyDecision-4.0.9/pyDecision/algorithm/p_xgaia.py` & `pyDecision-4.1.4/pyDecision/algorithm/p_xgaia.py`

 * *Files identical despite different names*

### Comparing `pyDecision-4.0.9/pyDecision/algorithm/piv.py` & `pyDecision-4.1.4/pyDecision/algorithm/piv.py`

 * *Files identical despite different names*

### Comparing `pyDecision-4.0.9/pyDecision/algorithm/psi.py` & `pyDecision-4.1.4/pyDecision/algorithm/psi.py`

 * *Files identical despite different names*

### Comparing `pyDecision-4.0.9/pyDecision/algorithm/rov.py` & `pyDecision-4.1.4/pyDecision/algorithm/rov.py`

 * *Files identical despite different names*

### Comparing `pyDecision-4.0.9/pyDecision/algorithm/saw.py` & `pyDecision-4.1.4/pyDecision/algorithm/saw.py`

 * *Files identical despite different names*

### Comparing `pyDecision-4.0.9/pyDecision/algorithm/smart.py` & `pyDecision-4.1.4/pyDecision/algorithm/smart.py`

 * *Files identical despite different names*

### Comparing `pyDecision-4.0.9/pyDecision/algorithm/todim.py` & `pyDecision-4.1.4/pyDecision/algorithm/todim.py`

 * *Files identical despite different names*

### Comparing `pyDecision-4.0.9/pyDecision/algorithm/topsis.py` & `pyDecision-4.1.4/pyDecision/algorithm/topsis.py`

 * *Files identical despite different names*

### Comparing `pyDecision-4.0.9/pyDecision/algorithm/vikor.py` & `pyDecision-4.1.4/pyDecision/algorithm/vikor.py`

 * *Files identical despite different names*

### Comparing `pyDecision-4.0.9/pyDecision/algorithm/waspas.py` & `pyDecision-4.1.4/pyDecision/algorithm/waspas.py`

 * *Files identical despite different names*

### Comparing `pyDecision-4.0.9/pyDecision/algorithm/wings.py` & `pyDecision-4.1.4/pyDecision/algorithm/wings.py`

 * *Files identical despite different names*

### Comparing `pyDecision-4.0.9/pyDecision/compare/compare.py` & `pyDecision-4.1.4/pyDecision/compare/compare.py`

 * *Files 1% similar despite different names*

```diff
@@ -23,21 +23,23 @@
 from pyDecision.algorithm.codas        import codas_method
 from pyDecision.algorithm.copeland     import copeland_method
 from pyDecision.algorithm.copras       import copras_method
 from pyDecision.algorithm.cradis       import cradis_method
 from pyDecision.algorithm.edas         import edas_method
 from pyDecision.algorithm.gra          import gra_method
 from pyDecision.algorithm.mabac        import mabac_method
+from pyDecision.algorithm.macbeth      import macbeth_method
 from pyDecision.algorithm.mairca       import mairca_method
 from pyDecision.algorithm.marcos       import marcos_method
 from pyDecision.algorithm.maut         import maut_method
 from pyDecision.algorithm.moora        import moora_method
 from pyDecision.algorithm.moosra       import moosra_method
 from pyDecision.algorithm.multimoora   import multimoora_method
 from pyDecision.algorithm.ocra         import ocra_method
+from pyDecision.algorithm.oreste       import oreste_method
 from pyDecision.algorithm.piv          import piv_method
 from pyDecision.algorithm.p_ii         import promethee_ii
 from pyDecision.algorithm.p_iv         import promethee_iv
 from pyDecision.algorithm.psi          import psi_method
 from pyDecision.algorithm.rov          import rov_method
 from pyDecision.algorithm.saw          import saw_method
 from pyDecision.algorithm.todim        import todim_method
@@ -135,17 +137,17 @@
             X[:,j] = w
             j      = j + 1
             print('MEREC: Done!')
     X = pd.DataFrame(X, index = ['g'+str(i+1) for i in range(0, X.shape[0])], columns = methods_list)    
     return X
 
 # Function: Compare Ranks Crisp
-def compare_ranks_crisp(dataset, weights, criterion_type, utility_functions = [], custom_methods = [], custom_ranks = [], methods_list = [], L = 0.5, lmbd = 0.02, epsilon = 0.5, step_size = 1, teta = 1, strategy_coefficient = 0.5, Q = [], S = [], P = [], F = [], lambda_value = 0.5):
+def compare_ranks_crisp(dataset, weights, criterion_type, utility_functions = [], custom_methods = [], custom_ranks = [], methods_list = [], L = 0.5, lmbd = 0.02, epsilon = 0.5, step_size = 1, teta = 1, strategy_coefficient = 0.5, Q = [], S = [], P = [], F = [], lambda_value = 0.5, alpha = 0.4):
     if ('all' in methods_list):
-        methods_list = ['aras', 'borda', 'cocoso', 'codas', 'copras', 'cradis', 'edas', 'gra', 'mabac', 'mairca', 'marcos', 'maut', 'moora', 'moosra', 'multimoora', 'ocra', 'piv', 'promethee_ii', 'promethee_iv', 'psi', 'rov', 'saw', 'todim', 'topsis', 'vikor', 'wsm', 'wpm', 'waspas']
+        methods_list = ['aras', 'borda', 'cocoso', 'codas', 'copras', 'cradis', 'edas', 'gra', 'mabac', 'macbeth', 'mairca', 'marcos', 'maut', 'moora', 'moosra', 'multimoora', 'ocra', 'oreste', 'piv', 'promethee_ii', 'promethee_iv', 'psi', 'rov', 'saw', 'todim', 'topsis', 'vikor', 'wsm', 'wpm', 'waspas']
     if (len(custom_methods) > 0):
         methods_list = custom_methods + methods_list 
     graph   = False
     verbose = False
     X       = np.zeros((dataset.shape[0], len(methods_list)))
     j       = 0
     for i in range(0, len(custom_ranks)):
@@ -199,14 +201,19 @@
             j      = j + 1
             print('GRA: Done!')
         if (method == 'mabac' or method == 'all'):
             rank   = mabac_method(dataset, criterion_type, graph, verbose)
             X[:,j] = rank
             j      = j + 1
             print('MABAC: Done!')
+        if (method == 'macbeth' or method == 'all'):
+            rank   = macbeth_method(dataset, weights, criterion_type, graph, verbose)
+            X[:,j] = rank
+            j      = j + 1
+            print('MACBETH: Done!')
         if (method == 'mairca' or method == 'all'):
             rank   = mairca_method(dataset, weights, criterion_type, graph, verbose)
             X[:,j] = rank
             j      = j + 1
             print('MAIRCA: Done!')
         if (method == 'marcos' or method == 'all'):
             rank   = marcos_method(dataset, weights, criterion_type, graph, verbose)
@@ -234,14 +241,19 @@
             j      = j + 1
             print('MULTIMOORA: Done!')
         if (method == 'ocra' or method == 'all'):
             rank   = ocra_method(dataset, weights, criterion_type, graph, verbose)
             X[:,j] = rank
             j      = j + 1
             print('OCRA: Done!')
+        if (method == 'oreste' or method == 'all'):
+            rank   = oreste_method(dataset, weights, criterion_type, alpha, graph, verbose)
+            X[:,j] = -rank
+            j      = j + 1
+            print('ORESTE: Done!')
         if (method == 'piv' or method == 'all'):
             rank   = piv_method(dataset, weights, criterion_type, graph, verbose)
             X[:,j] = rank
             j      = j + 1
             print('PIV: Done!')
         if (method == 'promethee_ii' or method == 'all'):
             data_adj = np.copy(dataset)
@@ -366,8 +378,8 @@
     ranked = np.zeros_like(X)
     for i in range(0, X.shape[1]):
         ranked[:, i] = X.shape[0] + 1 - rankdata(X[:, i], method = 'max')
     X      = pd.DataFrame(X, index = ['a'+str(i+1) for i in range(0, X.shape[0])], columns = methods_list)    
     ranked = pd.DataFrame(ranked, index = ['a'+str(i+1) for i in range(0, X.shape[0])], columns = methods_list)
     return X, ranked
 
-###############################################################################
+###############################################################################
```

### Comparing `pyDecision-4.0.9/pyDecision/util/LLM.py` & `pyDecision-4.1.4/pyDecision/util/LLM.py`

 * *Files identical despite different names*

### Comparing `pyDecision-4.0.9/pyDecision/util/ga.py` & `pyDecision-4.1.4/pyDecision/util/ga.py`

 * *Files identical despite different names*

### Comparing `pyDecision-4.0.9/pyDecision/util/gwo.py` & `pyDecision-4.1.4/pyDecision/util/gwo.py`

 * *Files identical despite different names*

### Comparing `pyDecision-4.0.9/pyDecision.egg-info/PKG-INFO` & `pyDecision-4.1.4/pyDecision.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 Metadata-Version: 2.1
 Name: pyDecision
-Version: 4.0.9
+Version: 4.1.4
 Summary: A MCDA Library
 Home-page: https://github.com/Valdecy/pyDecisions
 Author: Valdecy Pereira
 Author-email: valdecy.pereira@gmail.com
 License: GNU
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # pyDecision
 
 ## Introduction
 
-A python library with the following MCDA methods: **AHP** (Analytic Hierarchy Process); **Fuzzy AHP**; **ARAS** (Additive Ratio ASsessment); **Fuzzy ARAS**; **Borda**; **BWM** (Best-Worst Method); **CILOS** (Criterion Impact LOSs); **CoCoSo** (COmbined COmpromise SOlution); **CODAS** (Combinative Distance-based Assessment); **Copeland**; **COPRAS** (Complex PRoportional Assessment); **Fuzzy COPRAS**; **CRADIS** (Compromise Ranking of Alternatives from Distance to Ideal Solution); **CRITIC** (CRiteria Importance Through Intercriteria Correlation); **DEMATEL** (DEcision MAking Trial and Evaluation Laboratory); **Fuzzy DEMATEL**; **EDAS** (Evaluation based on Distance from Average Solution); **Fuzzy EDAS**; **Entropy**; **ELECTRE** (I, I_s, I_v, II, III, IV, Tri-B); **GRA** (Grey Relational Analysis); **IDOCRIW** (Integrated Determination of Objective CRIteria Weights); **MABAC** (Multi-Attributive Border Approximation area Comparison); **MAIRCA** (Multi-Attributive Ideal-Real Comparative Analysis); **MARCOS** (Measurement of Alternatives and Ranking according to COmpromise Solution); **MAUT** (Multi-attribute Utility Theory); **MEREC** (MEthod based on the Removal Effects of Criteria); **MOORA** (Multi-Objective Optimization on the basis of Ratio Analysis); **Fuzzy MOORA**; **MOOSRA** (Multi-Objective Optimisation on the Basis of Simple Ratio Analysis);  **MULTIMOORA** (Multi-Objective Optimization on the basis of Ratio Analisys Multiplicative Form); **OCRA** (Operational Competitiveness RAting); **Fuzzy OCRA** ; **PROMETHEE** (I, II, III, IV, V, VI, Gaia); **SAW** (Simple Additive Weighting); **SMART** (Simple Multi-Attribute Rating Technique); **TODIM** (TOmada de Decisao Interativa e Multicriterio - Interactive and Multicriteria Decision Making); **PIV** (Proximity Indexed Value); **PSI** (Preference Selection Index); **ROV** (Range Of Value); **TOPSIS** (Technique for Order of Preference by Similarity to Ideal Solution); **Fuzzy TOPSIS**; **VIKOR** (VIseKriterijumska Optimizacija I Kompromisno Resenje); **Fuzzy VIKOR**; **WINGS** (Weighted Influence Non-linear Gauge System); **WSM** (Weighted Sum Model); **WPM** (Weighted Product Model); **WASPAS** (Weighted Aggregates Sum Product Assessment).
+A python library with the following MCDA methods: **AHP** (Analytic Hierarchy Process); **Fuzzy AHP**; **ARAS** (Additive Ratio ASsessment); **Fuzzy ARAS**; **Borda**; **BWM** (Best-Worst Method); **CILOS** (Criterion Impact LOSs); **CoCoSo** (COmbined COmpromise SOlution); **CODAS** (Combinative Distance-based Assessment); **Copeland**; **COPRAS** (Complex PRoportional Assessment); **Fuzzy COPRAS**; **CRADIS** (Compromise Ranking of Alternatives from Distance to Ideal Solution); **CRITIC** (CRiteria Importance Through Intercriteria Correlation); **DEMATEL** (DEcision MAking Trial and Evaluation Laboratory); **Fuzzy DEMATEL**; **EDAS** (Evaluation based on Distance from Average Solution); **Fuzzy EDAS**; **Entropy**; **ELECTRE** (I, I_s, I_v, II, III, IV, Tri-B); **GRA** (Grey Relational Analysis); **IDOCRIW** (Integrated Determination of Objective CRIteria Weights); **MABAC** (Multi-Attributive Border Approximation area Comparison); **MACBETH** (Measuring Attractiveness by a Categorical Based Evaluation TecHnique); **MAIRCA** (Multi-Attributive Ideal-Real Comparative Analysis); **MARCOS** (Measurement of Alternatives and Ranking according to COmpromise Solution); **MAUT** (Multi-attribute Utility Theory); **MEREC** (MEthod based on the Removal Effects of Criteria); **MOORA** (Multi-Objective Optimization on the basis of Ratio Analysis); **Fuzzy MOORA**; **MOOSRA** (Multi-Objective Optimisation on the Basis of Simple Ratio Analysis);  **MULTIMOORA** (Multi-Objective Optimization on the basis of Ratio Analisys Multiplicative Form); **OCRA** (Operational Competitiveness RAting); **Fuzzy OCRA** ; **ORESTE** (Organisation Rangement Et SynThÃ¨sE de donnÃ©es relationnelles); **PROMETHEE** (I, II, III, IV, V, VI, Gaia); **SAW** (Simple Additive Weighting); **SMART** (Simple Multi-Attribute Rating Technique); **TODIM** (TOmada de Decisao Interativa e Multicriterio - Interactive and Multicriteria Decision Making); **PIV** (Proximity Indexed Value); **PSI** (Preference Selection Index); **Regime**; **ROV** (Range Of Value); **TOPSIS** (Technique for Order of Preference by Similarity to Ideal Solution); **Fuzzy TOPSIS**; **VIKOR** (VIseKriterijumska Optimizacija I Kompromisno Resenje); **Fuzzy VIKOR**; **WINGS** (Weighted Influence Non-linear Gauge System); **WSM** (Weighted Sum Model); **WPM** (Weighted Product Model); **WASPAS** (Weighted Aggregates Sum Product Assessment).
 
 pyDecision offers an array of features including the **comparison of ranking alternatives** and **comparison of criterion weights** from various methods. The library is also fully integrated with **chatGPT**, elevating result interpretation through AI. Additionally, pyDecision provides the flexibility to import results from custom methods or those not yet implemented in the library for swift comparison.
 
 ## Usage
 
 1. Install
 ```bash
@@ -75,48 +75,51 @@
 - CODAS ([ Colab Demo ](https://colab.research.google.com/drive/1hm7__urqFeBHM6nVQJcBzGPF72DFuoLr?usp=sharing)) ( [ Paper ](https://EconPapers.repec.org/RePEc:cys:ecocyb:v:50:y:2016:i:3:p:25-44))
 - Copeland ([ Colab Demo ](https://colab.research.google.com/drive/1ObP3AkQAzoCxT6et5Qkyk1trlER7mcdH?usp=sharing)) ( [ Paper ](https://link.springer.com/article/10.1007/bf01212012))
 - COPRAS ([ Colab Demo ](https://colab.research.google.com/drive/1TZJtSjXqwYEwuL7-wfLcPQ8ZBtDq3lth?usp=sharing)) ( [ Paper ](https://doi.org/10.3846/20294913.2012.762953))
 - Fuzzy COPRAS ([ Colab Demo ](https://colab.research.google.com/drive/1AIGgxBkmcA6YHKx06VeYcGf2EV8dPffW?usp=sharing)) ( [ Paper ](https://doi.org/10.1007/s00500-021-05762-w))
 - CRADIS ([ Colab Demo ](https://colab.research.google.com/drive/1p7AQmPIOsZFxaypqMsiRIWW8mIvDtoLi?usp=sharing)) ( [ Paper ](https://doi.org/10.1007%2Fs10668-021-01902-2))
 - CRITIC ([ Colab Demo ](https://colab.research.google.com/drive/1D5SaBHa1-Eo_KYSXHkFjsHYu29M21l_F?usp=sharing)) ( [ Paper ](https://doi.org/10.1016/0305-0548(94)00059-H))
 - DEMATEL ([ Colab Demo ](https://colab.research.google.com/drive/1T04qEft9uwTyQx--gADN6V_vUrT21Xo6?usp=sharing)) ( [ Paper ](https://doi.org/10.1155/2018/3696457))
-- Fuzzy DEMATEL ([ Colab Demo ](https://colab.research.google.com/drive/15e9dMDROr3cxjbWRXg3_t4TScuQtQDpR?usp=sharing)) ( [ Paper ](http://dx.doi.org/10.1016/j.eswa.2005.12.005))
+- Fuzzy DEMATEL ([ Colab Demo ](https://colab.research.google.com/drive/15e9dMDROr3cxjbWRXg3_t4TScuQtQDpR?usp=sharing)) ( [ Paper ](https://www.mdpi.com/2071-1050/9/11/2083))
 - EDAS ([ Colab Demo ](https://colab.research.google.com/drive/1xsMdwH-IH-zvOW-1kv6ztQnKGt7p5JnY?usp=sharing)) ( [ Paper ](https://doi.org/10.15388/Informatica.2015.57))
 - Fuzzy EDAS ([ Colab Demo ](https://colab.research.google.com/drive/1kw2LwztNAU9Asjj6BvBmvk11wvk8R3V6?usp=sharing)) ( [ Paper ](https://doi.org/10.1007/978-981-32-9072-3_63))
 - Entropy ([ Colab Demo ](https://colab.research.google.com/drive/1LOCef2KFxoV2qUEQRi4DqfzrgnMgtwT9?usp=sharing)) ( [ Paper ](https://people.math.harvard.edu/~ctm/home/text/others/shannon/entropy/entropy.pdf))
 - ELECTRE I     ([ Colab Demo ](https://colab.research.google.com/drive/1KFqRPBRyv-fxiu2B1y7VNkP5pCCbILF1?usp=sharing)) ( [ Paper ](https://github.com/Valdecy/Datasets/blob/master/MCDA/E01.pdf))
 - ELECTRE I_s   ([ Colab Demo ](https://colab.research.google.com/drive/1ngxsQPh2QULjd1_AifFofbukq5zIOePd?usp=sharing)) ( [ Paper ](http://dx.doi.org/10.1007/978-1-4757-5057-7_3))
 - ELECTRE I_v   ([ Colab Demo ](https://colab.research.google.com/drive/1moonq95gqXqmbRe2KvgqbN2IfowJ12C-?usp=sharing)) ( [ Paper ](http://dx.doi.org/10.1007/978-1-4757-5057-7_3))
 - ELECTRE II    ([ Colab Demo ](https://colab.research.google.com/drive/1UeAjICH6_tjVr3O9H-fC65HHYMVZgTKc?usp=sharing)) ( [ Paper ](http://dx.doi.org/10.1007/978-1-4757-5057-7_3))
 - ELECTRE III   ([ Colab Demo ](https://colab.research.google.com/drive/1smeD5ZoPgBnAAUyooAXSrkxHgqZPmUC9?usp=sharing)) ( [ Paper ](https://github.com/Valdecy/Datasets/raw/master/MCDA/E03.pdf))
 - ELECTRE IV    ([ Colab Demo ](https://colab.research.google.com/drive/178x062yC-Es6lstEiFaFprbMsTJZwnC-?usp=sharing)) ( [ Paper ](http://dx.doi.org/10.1007/978-1-4757-5057-7_3))
 - ELECTRE Tri-B ([ Colab Demo ](https://colab.research.google.com/drive/1hu0fJcxdBAiEDrVngmKQfpINpjTF-osE?usp=sharing)) ( [ Paper ](https://drive.google.com/file/d/1oWOI_sX3EEYdRbavoBTT7vUmPII1yPgE/view?usp=sharing))
 - GRA ([ Colab Demo ](https://colab.research.google.com/drive/1aMMI0Cuo5kpzTDefqEwJhf0wWpBOP_JL?usp=sharing)) ( [ Paper ](https://doi.org/10.1016/S0167-6911(82)80025-X))
 - IDOCRIW ([ Colab Demo ](https://colab.research.google.com/drive/1zt8uPFZGcHaSnpiT7tDnrDjvs0pK_7vS?usp=sharing)) ( [ Paper ](https://link.springer.com/chapter/10.1007/978-3-030-15009-9_19))
 - MABAC ([ Colab Demo ](https://colab.research.google.com/drive/1BMqO-HnBXdcOZfZoULpx1H4MLPoUGucJ?usp=sharing)) ( [ Paper ](https://doi.org/10.1016/j.eswa.2014.11.057))
+- MACBETH ([ Colab Demo ](https://colab.research.google.com/drive/1GqM9uPgbaWCGyj4l-XjkoifY2JJoVyf2?usp=sharing)) ( [ Paper ](https://link.springer.com/chapter/10.1007/978-3-030-15009-9_16))
 - MAIRCA ([ Colab Demo ](https://colab.research.google.com/drive/1gfqgrBAFGVygwm1j3lTjfy5wTsLgT_j5?usp=sharing)) ( [ Paper ](https://www.tandfonline.com/doi/full/10.1080/1331677X.2018.1506706))
 - MARCOS ([ Colab Demo ](https://colab.research.google.com/drive/13MI2Qrakm5VzHN3r5O2RqggCzQwRxCs-?usp=sharing)) ( [ Paper ](https://www.sciencedirect.com/science/article/abs/pii/S0360835219307004))
 - MAUT ([ Colab Demo ](https://colab.research.google.com/drive/1qm3ARgQm68GUK2irGiCB-B49vnVHazB7?usp=sharing)) ( [ Paper ](https://apps.dtic.mil/sti/pdfs/AD0770576.pdf))
 - MEREC ([ Colab Demo ](https://colab.research.google.com/drive/1XE3AIzS84w-gw_1MEtV7xvkU1Gj_tRPd?usp=sharing)) ( [ Paper ](https://www.mdpi.com/2073-8994/13/4/525))
 - MOORA ([ Colab Demo ](https://colab.research.google.com/drive/1FpKl0QAdwGgCVvLYsRHvMWhz7yOp17B5?usp=sharing)) ( [ Paper ](https://www.researchgate.net/publication/228345226_The_MOORA_method_and_its_application_to_privatization_in_a_transition_economy))
 - Fuzzy MOORA ([ Colab Demo ](https://colab.research.google.com/drive/1ydHzGeA8WBVY5Gyu8K7Oq6kofQ5XbK3P?usp=sharing)) ( [ Paper ](https://pdfs.semanticscholar.org/6d33/ca3f14c9ed44d23742fd4e9cf94cebcaf148.pdf))
 - MOOSRA ([ Colab Demo ](https://colab.research.google.com/drive/1KYyA4f3OsipPA5e63Ja4A0OGmHvNY6dj?usp=sharing)) ( [ Paper ](https://ijret.org/volumes/2014v03/i15/IJRET20140315105.pdf))
 - MULTIMOORA ([ Colab Demo ](https://colab.research.google.com/drive/1JAT8qqHPNoFfMV6a-CzF6BgRwtcUF3-e?usp=sharing)) ( [ Paper ](https://journals.vilniustech.lt/index.php/TEDE/article/view/5832/5078))
 - OCRA ([ Colab Demo ](https://colab.research.google.com/drive/1yQ41lOdjhiANtD1SOXoxA7gVim7A4X4P?usp=sharing)) ( [ Paper ](https://www.researchgate.net/publication/272362515_Selection_of_non-conventional_machining_processes_using_the_OCRA_method))
 - Fuzzy OCRA ([ Colab Demo ](https://colab.research.google.com/drive/1SniY4RLsR6jR9SnI3AR9k0wGlBWH6Pm8?usp=sharing)) ( [ Paper ](http://dx.doi.org/10.5755/j01.ee.30.5.20546))
+- ORESTE ([ Colab Demo ]()) ( [ Paper ](https://link.springer.com/chapter/10.1007/978-3-030-15009-9_3))
 - PROMETHEE I    ([ Colab Demo ](https://colab.research.google.com/drive/1WsagC7-Y_5X-Xl90pMz8YwUkKfxf2vol?usp=sharing)) ( [ Paper ](https://www.cin.ufpe.br/~if703/aulas/promethee.pdf))
 - PROMETHEE II   ([ Colab Demo ](https://colab.research.google.com/drive/143TUtTBy9y6gW0kMVAfhANBhuw1bKvBB?usp=sharing)) ( [ Paper ](https://www.cin.ufpe.br/~if703/aulas/promethee.pdf))
 - PROMETHEE III  ([ Colab Demo ](https://colab.research.google.com/drive/11DBaEBBT8B-B3poXubvZ41HELOHok0Rz?usp=sharing)) ( [ Paper ](http://dx.doi.org/10.1007/978-3-030-15009-9_5
 ))
 - PROMETHEE IV   ([ Colab Demo ](https://colab.research.google.com/drive/1X2evE6pIf4F7qiKjt1fSU2PqT-NaA5sJ?usp=sharing)) ( [ Paper ](http://dx.doi.org/10.1007/978-3-319-11949-6_14))
 - PROMETHEE V    ([ Colab Demo ](https://colab.research.google.com/drive/1IaZCCtq5m8vBBxrBLMCp6xB5U2j8ZNRc?usp=sharing)) ( [ Paper ](https://www.cin.ufpe.br/~if703/aulas/promethee.pdf))
 - PROMETHEE VI   ([ Colab Demo ](https://colab.research.google.com/drive/14QdhifGitj4GK-QijRr1vj_dmGU2Pfh4?usp=sharing)) ( [ Paper ](https://www.cin.ufpe.br/~if703/aulas/promethee.pdf))
 - PROMETHEE Gaia ([ Colab Demo ](https://colab.research.google.com/drive/1lj7IRKXcuRjrpoBp_KmQn_3sI3P_Qxju?usp=sharing)) ( [ Paper ](https://www.cin.ufpe.br/~if703/aulas/promethee.pdf))
 - PIV ([ Colab Demo ](https://colab.research.google.com/drive/1PwJoBqYn1O2s22MqC9euP89Uyv4sedS0?usp=sharing)) ( [ Paper ](https://www.sciencedirect.com/science/article/abs/pii/S0360835218301360))
 - PSI ([ Colab Demo ](https://colab.research.google.com/drive/1u9tN8cYl2mx6KK6yLW2oz6fuVoy8xcCI?usp=sharing)) ( [ Paper ](https://www.sciencedirect.com/science/article/abs/pii/S0261306909006396))
+- Regime ([ Colab Demo ](https://colab.research.google.com/drive/1jcAcjAS92rxvE2urhc6HPixvzJ60HqEg?usp=sharing)) ( [ Paper ](https://link.springer.com/chapter/10.1007/978-3-030-15009-9_2))
 - ROV ([ Colab Demo ](https://colab.research.google.com/drive/1sQAPCem0pcS29uf6-n4TpncXMXNx9JDh?usp=sharing)) ( [ Paper ](https://doi.org/10.5267/j.dsl.2015.12.001))
 - SAW ([ Colab Demo ](https://colab.research.google.com/drive/1R4cIsu0jBP9-6zwww_bNxEEnVGrhnS2d?usp=sharing)) ( [ Paper ](https://media.neliti.com/media/publications/326766-simple-additive-weighting-saw-method-in-f8f093e8.pdf))
 - SMART ([ Colab Demo ](https://colab.research.google.com/drive/1K93HXHBR_v2da95Hh_CB6AmTCqta-k3D?usp=sharing)) ( [ Paper ](https://doi.org/10.1007/978-1-4612-3982-6_4))
 - TODIM ([ Colab Demo ](https://colab.research.google.com/drive/1EQqhhBQHHb8HT0TfuuVeFA2kwezsQYT1?usp=sharing)) ( [ Paper ](https://www.sciencedirect.com/science/article/abs/pii/S0377221707010740))
 - TOPSIS ([ Colab Demo ](https://colab.research.google.com/drive/1s87DC5_oa9GvgVe98oAP1UIhduac09CB?usp=sharing)) ( [ Paper ](https://doi.org/10.1057/jors.1987.44))
 - Fuzzy TOPSIS ([ Colab Demo ](https://colab.research.google.com/drive/1eKx7AOYrnG-kZcsBt28rMEtCrUO-j3J-?usp=sharing)) ( [ Paper ](https://doi.org/10.1016/j.procs.2016.07.088))
 - VIKOR ([ Colab Demo ](https://colab.research.google.com/drive/1egZiTNvI2eE-tyJ2m85MM6B3-qhiSjPG?usp=sharing)) ( [ Paper ](https://doi.org/10.1007/978-981-33-4745-8_8))
```

### Comparing `pyDecision-4.0.9/pyDecision.egg-info/SOURCES.txt` & `pyDecision-4.1.4/pyDecision.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -37,31 +37,34 @@
 pyDecision/algorithm/fuzzy_moora.py
 pyDecision/algorithm/fuzzy_ocra.py
 pyDecision/algorithm/fuzzy_topsis.py
 pyDecision/algorithm/fuzzy_vikor.py
 pyDecision/algorithm/gra.py
 pyDecision/algorithm/idocriw.py
 pyDecision/algorithm/mabac.py
+pyDecision/algorithm/macbeth.py
 pyDecision/algorithm/mairca.py
 pyDecision/algorithm/marcos.py
 pyDecision/algorithm/maut.py
 pyDecision/algorithm/merec.py
 pyDecision/algorithm/moora.py
 pyDecision/algorithm/moosra.py
 pyDecision/algorithm/multimoora.py
 pyDecision/algorithm/ocra.py
+pyDecision/algorithm/oreste.py
 pyDecision/algorithm/p_i.py
 pyDecision/algorithm/p_ii.py
 pyDecision/algorithm/p_iii.py
 pyDecision/algorithm/p_iv.py
 pyDecision/algorithm/p_v.py
 pyDecision/algorithm/p_vi.py
 pyDecision/algorithm/p_xgaia.py
 pyDecision/algorithm/piv.py
 pyDecision/algorithm/psi.py
+pyDecision/algorithm/regime.py
 pyDecision/algorithm/rov.py
 pyDecision/algorithm/saw.py
 pyDecision/algorithm/smart.py
 pyDecision/algorithm/todim.py
 pyDecision/algorithm/topsis.py
 pyDecision/algorithm/vikor.py
 pyDecision/algorithm/waspas.py
```

### Comparing `pyDecision-4.0.9/setup.py` & `pyDecision-4.1.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from pathlib import Path
 
 this_directory = Path(__file__).parent
 long_description = (this_directory / 'README.md').read_text()
 
 setup(
     name='pyDecision',
-    version='4.0.9',
+    version='4.1.4',
     license='GNU',
     author='Valdecy Pereira',
     author_email='valdecy.pereira@gmail.com',
     url='https://github.com/Valdecy/pyDecisions',
     packages=find_packages(),
     install_requires=[
         'matplotlib',
```

