# Comparing `tmp/siriuspy-2.78.0.tar.gz` & `tmp/siriuspy-2.79.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "siriuspy-2.78.0.tar", last modified: Mon Jul 17 20:43:58 2023, max compression
+gzip compressed data, was "siriuspy-2.79.0.tar", last modified: Sun Jul 30 14:45:12 2023, max compression
```

## Comparing `siriuspy-2.78.0.tar` & `siriuspy-2.79.0.tar`

### file list

```diff
@@ -1,396 +1,399 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-17 20:43:58.525197 siriuspy-2.78.0/
--rw-r--r--   0 runner    (1001) docker     (122)    34494 2023-07-17 20:43:48.000000 siriuspy-2.78.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (122)       90 2023-07-17 20:43:48.000000 siriuspy-2.78.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (122)     1423 2023-07-17 20:43:58.525197 siriuspy-2.78.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)      954 2023-07-17 20:43:48.000000 siriuspy-2.78.0/README.md
--rw-r--r--   0 runner    (1001) docker     (122)      128 2023-07-17 20:43:48.000000 siriuspy-2.78.0/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (122)       38 2023-07-17 20:43:58.525197 siriuspy-2.78.0/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (122)     1243 2023-07-17 20:43:48.000000 siriuspy-2.78.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-17 20:43:58.497197 siriuspy-2.78.0/siriuspy/
--rw-r--r--   0 runner    (1001) docker     (122)        7 2023-07-17 20:43:48.000000 siriuspy-2.78.0/siriuspy/VERSION
--rw-r--r--   0 runner    (1001) docker     (122)      515 2023-07-17 20:43:48.000000 siriuspy-2.78.0/siriuspy/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-17 20:43:58.497197 siriuspy-2.78.0/siriuspy/bsmp/
--rw-r--r--   0 runner    (1001) docker     (122)      422 2023-07-17 20:43:48.000000 siriuspy-2.78.0/siriuspy/bsmp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    15885 2023-07-17 20:43:48.000000 siriuspy-2.78.0/siriuspy/bsmp/commands.py
--rw-r--r--   0 runner    (1001) docker     (122)     1904 2023-07-17 20:43:48.000000 siriuspy-2.78.0/siriuspy/bsmp/constants.py
--rw-r--r--   0 runner    (1001) docker     (122)    11790 2023-07-17 20:43:48.000000 siriuspy-2.78.0/siriuspy/bsmp/entities.py
--rw-r--r--   0 runner    (1001) docker     (122)      610 2023-07-17 20:43:48.000000 siriuspy-2.78.0/siriuspy/bsmp/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (122)     8110 2023-07-17 20:43:48.000000 siriuspy-2.78.0/siriuspy/bsmp/serial.py
--rw-r--r--   0 runner    (1001) docker     (122)     1204 2023-07-17 20:43:48.000000 siriuspy-2.78.0/siriuspy/bsmp/types.py
--rw-r--r--   0 runner    (1001) docker     (122)     2992 2023-07-17 20:43:48.000000 siriuspy-2.78.0/siriuspy/callbacks.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-17 20:43:58.501197 siriuspy-2.78.0/siriuspy/clientarch/
--rw-r--r--   0 runner    (1001) docker     (122)      306 2023-07-17 20:43:48.000000 siriuspy-2.78.0/siriuspy/clientarch/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    13813 2023-07-17 20:43:48.000000 siriuspy-2.78.0/siriuspy/clientarch/client.py
--rw-r--r--   0 runner    (1001) docker     (122)     6392 2023-07-17 20:43:48.000000 siriuspy-2.78.0/siriuspy/clientarch/devices.py
--rw-r--r--   0 runner    (1001) docker     (122)      643 2023-07-17 20:43:48.000000 siriuspy-2.78.0/siriuspy/clientarch/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (122)    20400 2023-07-17 20:43:48.000000 siriuspy-2.78.0/siriuspy/clientarch/pvarch.py
--rw-r--r--   0 runner    (1001) docker     (122)     5003 2023-07-17 20:43:48.000000 siriuspy-2.78.0/siriuspy/clientarch/time.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-17 20:43:58.501197 siriuspy-2.78.0/siriuspy/clientconfigdb/
--rw-r--r--   0 runner    (1001) docker     (122)      227 2023-07-17 20:43:48.000000 siriuspy-2.78.0/siriuspy/clientconfigdb/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     3345 2023-07-17 20:43:48.000000 siriuspy-2.78.0/siriuspy/clientconfigdb/_templates.py
--rw-r--r--   0 runner    (1001) docker     (122)     9599 2023-07-17 20:43:48.000000 siriuspy-2.78.0/siriuspy/clientconfigdb/configdb_client.py
--rw-r--r--   0 runner    (1001) docker     (122)     5448 2023-07-17 20:43:48.000000 siriuspy-2.78.0/siriuspy/clientconfigdb/configdb_document.py
--rw-r--r--   0 runner    (1001) docker     (122)     4785 2023-07-17 20:43:48.000000 siriuspy-2.78.0/siriuspy/clientconfigdb/pvsconfig.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-17 20:43:58.501197 siriuspy-2.78.0/siriuspy/clientconfigdb/types/
--rw-r--r--   0 runner    (1001) docker     (122)      286 2023-07-17 20:43:48.000000 siriuspy-2.78.0/siriuspy/clientconfigdb/types/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    13746 2023-07-17 20:43:48.000000 siriuspy-2.78.0/siriuspy/clientconfigdb/types/as_corrloop_params.py
--rw-r--r--   0 runner    (1001) docker     (122)    57620 2023-07-17 20:43:48.000000 siriuspy-2.78.0/siriuspy/clientconfigdb/types/as_diagnostics.py
--rw-r--r--   0 runner    (1001) docker     (122)     6681 2023-07-17 20:43:48.000000 siriuspy-2.78.0/siriuspy/clientconfigdb/types/as_pwrstate.py
--rw-r--r--   0 runner    (1001) docker     (122)    34247 2023-07-17 20:43:48.000000 siriuspy-2.78.0/siriuspy/clientconfigdb/types/as_rf.py
--rw-r--r--   0 runner    (1001) docker     (122)     1135 2023-07-17 20:43:48.000000 siriuspy-2.78.0/siriuspy/clientconfigdb/types/bo_chromcorr_params.py
--rw-r--r--   0 runner    (1001) docker     (122)     3984 2023-07-17 20:43:48.000000 siriuspy-2.78.0/siriuspy/clientconfigdb/types/bo_normalized.py
--rw-r--r--   0 runner    (1001) docker     (122)     1135 2023-07-17 20:43:48.000000 siriuspy-2.78.0/siriuspy/clientconfigdb/types/bo_orbcorr_respm.py
--rw-r--r--   0 runner    (1001) docker     (122)      700 2023-07-17 20:43:48.000000 siriuspy-2.78.0/siriuspy/clientconfigdb/types/bo_orbit.py
--rw-r--r--   0 runner    (1001) docker     (122)     3042 2023-07-17 20:43:48.000000 siriuspy-2.78.0/siriuspy/clientconfigdb/types/bo_ramp.py
--rw-r--r--   0 runner    (1001) docker     (122)      975 2023-07-17 20:43:48.000000 siriuspy-2.78.0/siriuspy/clientconfigdb/types/bo_tunecorr_params.py
--rw-r--r--   0 runner    (1001) docker     (122)   123005 2023-07-17 20:43:48.000000 siriuspy-2.78.0/siriuspy/clientconfigdb/types/global_config.py
--rw-r--r--   0 runner    (1001) docker     (122)      735 2023-07-17 20:43:48.000000 siriuspy-2.78.0/siriuspy/clientconfigdb/types/si_bbadata.py
--rw-r--r--   0 runner    (1001) docker     (122)    18619 2023-07-17 20:43:48.000000 siriuspy-2.78.0/siriuspy/clientconfigdb/types/si_bbbproc.py
--rw-r--r--   0 runner    (1001) docker     (122)     1697 2023-07-17 20:43:48.000000 siriuspy-2.78.0/siriuspy/clientconfigdb/types/si_chromcorr_params.py
--rw-r--r--   0 runner    (1001) docker     (122)     1146 2023-07-17 20:43:48.000000 siriuspy-2.78.0/siriuspy/clientconfigdb/types/si_fastorbcorr_respm.py
--rw-r--r--   0 runner    (1001) docker     (122)     4741 2023-07-17 20:43:48.000000 siriuspy-2.78.0/siriuspy/clientconfigdb/types/si_fofb.py
--rw-r--r--   0 runner    (1001) docker     (122)      957 2023-07-17 20:43:48.000000 siriuspy-2.78.0/siriuspy/clientconfigdb/types/si_id.py
--rw-r--r--   0 runner    (1001) docker     (122)     3181 2023-07-17 20:43:48.000000 siriuspy-2.78.0/siriuspy/clientconfigdb/types/si_idff.py
--rw-r--r--   0 runner    (1001) docker     (122)     1136 2023-07-17 20:43:48.000000 siriuspy-2.78.0/siriuspy/clientconfigdb/types/si_orbcorr_respm.py
--rw-r--r--   0 runner    (1001) docker     (122)      701 2023-07-17 20:43:48.000000 siriuspy-2.78.0/siriuspy/clientconfigdb/types/si_orbit.py
--rw-r--r--   0 runner    (1001) docker     (122)     1290 2023-07-17 20:43:48.000000 siriuspy-2.78.0/siriuspy/clientconfigdb/types/si_tunecorr_params.py
--rw-r--r--   0 runner    (1001) docker     (122)     1738 2023-07-17 20:43:48.000000 siriuspy-2.78.0/siriuspy/clientconfigdb/types/tb_normalized.py
--rw-r--r--   0 runner    (1001) docker     (122)      969 2023-07-17 20:43:48.000000 siriuspy-2.78.0/siriuspy/clientconfigdb/types/tb_orbcorr_respm.py
--rw-r--r--   0 runner    (1001) docker     (122)      693 2023-07-17 20:43:48.000000 siriuspy-2.78.0/siriuspy/clientconfigdb/types/tb_orbit.py
--rw-r--r--   0 runner    (1001) docker     (122)     1651 2023-07-17 20:43:48.000000 siriuspy-2.78.0/siriuspy/clientconfigdb/types/tb_posang_respm.py
--rw-r--r--   0 runner    (1001) docker     (122)      969 2023-07-17 20:43:48.000000 siriuspy-2.78.0/siriuspy/clientconfigdb/types/ts_orbcorr_respm.py
--rw-r--r--   0 runner    (1001) docker     (122)      693 2023-07-17 20:43:48.000000 siriuspy-2.78.0/siriuspy/clientconfigdb/types/ts_orbit.py
--rw-r--r--   0 runner    (1001) docker     (122)     1721 2023-07-17 20:43:48.000000 siriuspy-2.78.0/siriuspy/clientconfigdb/types/ts_posang_respm.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-17 20:43:58.501197 siriuspy-2.78.0/siriuspy/clientweb/
--rw-r--r--   0 runner    (1001) docker     (122)       50 2023-07-17 20:43:48.000000 siriuspy-2.78.0/siriuspy/clientweb/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     5896 2023-07-17 20:43:48.000000 siriuspy-2.78.0/siriuspy/clientweb/implementation.py
--rw-r--r--   0 runner    (1001) docker     (122)     2236 2023-07-17 20:43:48.000000 siriuspy-2.78.0/siriuspy/csdev.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-17 20:43:58.501197 siriuspy-2.78.0/siriuspy/currinfo/
--rw-r--r--   0 runner    (1001) docker     (122)      144 2023-07-17 20:43:48.000000 siriuspy-2.78.0/siriuspy/currinfo/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     9620 2023-07-17 20:43:48.000000 siriuspy-2.78.0/siriuspy/currinfo/csdev.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-17 20:43:58.501197 siriuspy-2.78.0/siriuspy/currinfo/lifetime/
--rw-r--r--   0 runner    (1001) docker     (122)       72 2023-07-17 20:43:48.000000 siriuspy-2.78.0/siriuspy/currinfo/lifetime/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    12607 2023-07-17 20:43:48.000000 siriuspy-2.78.0/siriuspy/currinfo/lifetime/main.py
--rw-r--r--   0 runner    (1001) docker     (122)    23275 2023-07-17 20:43:48.000000 siriuspy-2.78.0/siriuspy/currinfo/main.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-17 20:43:58.505197 siriuspy-2.78.0/siriuspy/cycle/
--rw-r--r--   0 runner    (1001) docker     (122)      514 2023-07-17 20:43:48.000000 siriuspy-2.78.0/siriuspy/cycle/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)   104994 2023-07-17 20:43:48.000000 siriuspy-2.78.0/siriuspy/cycle/bo_cycle_data.py
--rw-r--r--   0 runner    (1001) docker     (122)    31135 2023-07-17 20:43:48.000000 siriuspy-2.78.0/siriuspy/cycle/conn.py
--rw-r--r--   0 runner    (1001) docker     (122)     9781 2023-07-17 20:43:48.000000 siriuspy-2.78.0/siriuspy/cycle/fc_cycle_data.py
--rw-r--r--   0 runner    (1001) docker     (122)     3286 2023-07-17 20:43:48.000000 siriuspy-2.78.0/siriuspy/cycle/li_cycle_data.py
--rw-r--r--   0 runner    (1001) docker     (122)    38408 2023-07-17 20:43:48.000000 siriuspy-2.78.0/siriuspy/cycle/main.py
--rw-r--r--   0 runner    (1001) docker     (122)     3574 2023-07-17 20:43:48.000000 siriuspy-2.78.0/siriuspy/cycle/util.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-17 20:43:58.505197 siriuspy-2.78.0/siriuspy/devices/
--rw-r--r--   0 runner    (1001) docker     (122)     1764 2023-07-17 20:43:48.000000 siriuspy-2.78.0/siriuspy/devices/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    48546 2023-07-17 20:43:48.000000 siriuspy-2.78.0/siriuspy/devices/bbb.py
--rw-r--r--   0 runner    (1001) docker     (122)     2786 2023-07-17 20:43:48.000000 siriuspy-2.78.0/siriuspy/devices/blctrl.py
--rw-r--r--   0 runner    (1001) docker     (122)    41475 2023-07-17 20:43:48.000000 siriuspy-2.78.0/siriuspy/devices/bpm.py
--rw-r--r--   0 runner    (1001) docker     (122)     7380 2023-07-17 20:43:48.000000 siriuspy-2.78.0/siriuspy/devices/currinfo.py
--rw-r--r--   0 runner    (1001) docker     (122)     2402 2023-07-17 20:43:48.000000 siriuspy-2.78.0/siriuspy/devices/dcct.py
--rw-r--r--   0 runner    (1001) docker     (122)    13949 2023-07-17 20:43:48.000000 siriuspy-2.78.0/siriuspy/devices/device.py
--rw-r--r--   0 runner    (1001) docker     (122)    16525 2023-07-17 20:43:48.000000 siriuspy-2.78.0/siriuspy/devices/dvf.py
--rw-r--r--   0 runner    (1001) docker     (122)    30814 2023-07-17 20:43:48.000000 siriuspy-2.78.0/siriuspy/devices/egun.py
--rw-r--r--   0 runner    (1001) docker     (122)     1743 2023-07-17 20:43:48.000000 siriuspy-2.78.0/siriuspy/devices/energy.py
--rw-r--r--   0 runner    (1001) docker     (122)    51622 2023-07-17 20:43:48.000000 siriuspy-2.78.0/siriuspy/devices/fofb.py
--rw-r--r--   0 runner    (1001) docker     (122)     2121 2023-07-17 20:43:48.000000 siriuspy-2.78.0/siriuspy/devices/ict.py
--rw-r--r--   0 runner    (1001) docker     (122)    10051 2023-07-17 20:43:48.000000 siriuspy-2.78.0/siriuspy/devices/idff.py
--rw-r--r--   0 runner    (1001) docker     (122)    21328 2023-07-17 20:43:48.000000 siriuspy-2.78.0/siriuspy/devices/ids.py
--rw-r--r--   0 runner    (1001) docker     (122)    20759 2023-07-17 20:43:48.000000 siriuspy-2.78.0/siriuspy/devices/injctrl.py
--rw-r--r--   0 runner    (1001) docker     (122)    38127 2023-07-17 20:43:48.000000 siriuspy-2.78.0/siriuspy/devices/injsys.py
--rw-r--r--   0 runner    (1001) docker     (122)     1630 2023-07-17 20:43:48.000000 siriuspy-2.78.0/siriuspy/devices/lienergy.py
--rw-r--r--   0 runner    (1001) docker     (122)     6948 2023-07-17 20:43:48.000000 siriuspy-2.78.0/siriuspy/devices/lillrf.py
--rw-r--r--   0 runner    (1001) docker     (122)      964 2023-07-17 20:43:48.000000 siriuspy-2.78.0/siriuspy/devices/machshift.py
--rw-r--r--   0 runner    (1001) docker     (122)     2290 2023-07-17 20:43:48.000000 siriuspy-2.78.0/siriuspy/devices/modltr.py
--rw-r--r--   0 runner    (1001) docker     (122)    36060 2023-07-17 20:43:48.000000 siriuspy-2.78.0/siriuspy/devices/orbit_interlock.py
--rw-r--r--   0 runner    (1001) docker     (122)     2427 2023-07-17 20:43:48.000000 siriuspy-2.78.0/siriuspy/devices/posang.py
--rw-r--r--   0 runner    (1001) docker     (122)    10195 2023-07-17 20:43:48.000000 siriuspy-2.78.0/siriuspy/devices/psconv.py
--rw-r--r--   0 runner    (1001) docker     (122)    12184 2023-07-17 20:43:48.000000 siriuspy-2.78.0/siriuspy/devices/pssofb.py
--rw-r--r--   0 runner    (1001) docker     (122)    20070 2023-07-17 20:43:48.000000 siriuspy-2.78.0/siriuspy/devices/pstesters.py
--rw-r--r--   0 runner    (1001) docker     (122)    30064 2023-07-17 20:43:48.000000 siriuspy-2.78.0/siriuspy/devices/pwrsupply.py
--rw-r--r--   0 runner    (1001) docker     (122)    35448 2023-07-17 20:43:48.000000 siriuspy-2.78.0/siriuspy/devices/rf.py
--rw-r--r--   0 runner    (1001) docker     (122)     3836 2023-07-17 20:43:48.000000 siriuspy-2.78.0/siriuspy/devices/screen.py
--rw-r--r--   0 runner    (1001) docker     (122)    22629 2023-07-17 20:43:48.000000 siriuspy-2.78.0/siriuspy/devices/sofb.py
--rw-r--r--   0 runner    (1001) docker     (122)     2652 2023-07-17 20:43:48.000000 siriuspy-2.78.0/siriuspy/devices/syncd.py
--rw-r--r--   0 runner    (1001) docker     (122)    17907 2023-07-17 20:43:48.000000 siriuspy-2.78.0/siriuspy/devices/timing.py
--rw-r--r--   0 runner    (1001) docker     (122)     5055 2023-07-17 20:43:48.000000 siriuspy-2.78.0/siriuspy/devices/tune.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-17 20:43:58.505197 siriuspy-2.78.0/siriuspy/diagbeam/
--rw-r--r--   0 runner    (1001) docker     (122)       30 2023-07-17 20:43:48.000000 siriuspy-2.78.0/siriuspy/diagbeam/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-17 20:43:58.505197 siriuspy-2.78.0/siriuspy/diagbeam/bpm/
--rw-r--r--   0 runner    (1001) docker     (122)       24 2023-07-17 20:43:48.000000 siriuspy-2.78.0/siriuspy/diagbeam/bpm/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    24052 2023-07-17 20:43:48.000000 siriuspy-2.78.0/siriuspy/diagbeam/bpm/csdev.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-17 20:43:58.505197 siriuspy-2.78.0/siriuspy/diagbeam/dcct/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-17 20:43:48.000000 siriuspy-2.78.0/siriuspy/diagbeam/dcct/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     8215 2023-07-17 20:43:48.000000 siriuspy-2.78.0/siriuspy/diagbeam/dcct/csdev.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-17 20:43:58.509197 siriuspy-2.78.0/siriuspy/diagbeam/ict/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-17 20:43:48.000000 siriuspy-2.78.0/siriuspy/diagbeam/ict/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     4878 2023-07-17 20:43:48.000000 siriuspy-2.78.0/siriuspy/diagbeam/ict/csdev.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-17 20:43:58.509197 siriuspy-2.78.0/siriuspy/diagbeam/screen/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-17 20:43:48.000000 siriuspy-2.78.0/siriuspy/diagbeam/screen/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    12756 2023-07-17 20:43:48.000000 siriuspy-2.78.0/siriuspy/diagbeam/screen/csdev.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-17 20:43:58.509197 siriuspy-2.78.0/siriuspy/diagbeam/slit/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-17 20:43:48.000000 siriuspy-2.78.0/siriuspy/diagbeam/slit/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     6750 2023-07-17 20:43:48.000000 siriuspy-2.78.0/siriuspy/diagbeam/slit/csdev.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-17 20:43:58.509197 siriuspy-2.78.0/siriuspy/diagsys/
--rw-r--r--   0 runner    (1001) docker     (122)       26 2023-07-17 20:43:48.000000 siriuspy-2.78.0/siriuspy/diagsys/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     1484 2023-07-17 20:43:48.000000 siriuspy-2.78.0/siriuspy/diagsys/app.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-17 20:43:58.509197 siriuspy-2.78.0/siriuspy/diagsys/lidiag/
--rw-r--r--   0 runner    (1001) docker     (122)       29 2023-07-17 20:43:48.000000 siriuspy-2.78.0/siriuspy/diagsys/lidiag/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     5193 2023-07-17 20:43:48.000000 siriuspy-2.78.0/siriuspy/diagsys/lidiag/csdev.py
--rw-r--r--   0 runner    (1001) docker     (122)     8168 2023-07-17 20:43:48.000000 siriuspy-2.78.0/siriuspy/diagsys/lidiag/main.py
--rw-r--r--   0 runner    (1001) docker     (122)     8774 2023-07-17 20:43:48.000000 siriuspy-2.78.0/siriuspy/diagsys/lidiag/pvs.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-17 20:43:58.509197 siriuspy-2.78.0/siriuspy/diagsys/psdiag/
--rw-r--r--   0 runner    (1001) docker     (122)       25 2023-07-17 20:43:48.000000 siriuspy-2.78.0/siriuspy/diagsys/psdiag/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     2699 2023-07-17 20:43:48.000000 siriuspy-2.78.0/siriuspy/diagsys/psdiag/csdev.py
--rw-r--r--   0 runner    (1001) docker     (122)     4582 2023-07-17 20:43:48.000000 siriuspy-2.78.0/siriuspy/diagsys/psdiag/main.py
--rw-r--r--   0 runner    (1001) docker     (122)     7692 2023-07-17 20:43:48.000000 siriuspy-2.78.0/siriuspy/diagsys/psdiag/pvs.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-17 20:43:58.509197 siriuspy-2.78.0/siriuspy/diagsys/pudiag/
--rw-r--r--   0 runner    (1001) docker     (122)       25 2023-07-17 20:43:48.000000 siriuspy-2.78.0/siriuspy/diagsys/pudiag/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     1418 2023-07-17 20:43:48.000000 siriuspy-2.78.0/siriuspy/diagsys/pudiag/csdev.py
--rw-r--r--   0 runner    (1001) docker     (122)     2871 2023-07-17 20:43:48.000000 siriuspy-2.78.0/siriuspy/diagsys/pudiag/main.py
--rw-r--r--   0 runner    (1001) docker     (122)     4099 2023-07-17 20:43:48.000000 siriuspy-2.78.0/siriuspy/diagsys/pudiag/pvs.py
--rw-r--r--   0 runner    (1001) docker     (122)     6792 2023-07-17 20:43:48.000000 siriuspy-2.78.0/siriuspy/diagsys/pvs.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-17 20:43:58.509197 siriuspy-2.78.0/siriuspy/diagsys/rfdiag/
--rw-r--r--   0 runner    (1001) docker     (122)       25 2023-07-17 20:43:48.000000 siriuspy-2.78.0/siriuspy/diagsys/rfdiag/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     2409 2023-07-17 20:43:48.000000 siriuspy-2.78.0/siriuspy/diagsys/rfdiag/csdev.py
--rw-r--r--   0 runner    (1001) docker     (122)     3783 2023-07-17 20:43:48.000000 siriuspy-2.78.0/siriuspy/diagsys/rfdiag/main.py
--rw-r--r--   0 runner    (1001) docker     (122)     4891 2023-07-17 20:43:48.000000 siriuspy-2.78.0/siriuspy/diagsys/rfdiag/pvs.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-17 20:43:58.509197 siriuspy-2.78.0/siriuspy/dvfimgproc/
--rw-r--r--   0 runner    (1001) docker     (122)       39 2023-07-17 20:43:48.000000 siriuspy-2.78.0/siriuspy/dvfimgproc/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     7692 2023-07-17 20:43:48.000000 siriuspy-2.78.0/siriuspy/dvfimgproc/csdev.py
--rw-r--r--   0 runner    (1001) docker     (122)    15295 2023-07-17 20:43:48.000000 siriuspy-2.78.0/siriuspy/dvfimgproc/main.py
--rw-r--r--   0 runner    (1001) docker     (122)     7082 2023-07-17 20:43:48.000000 siriuspy-2.78.0/siriuspy/dvfimgproc/meas.py
--rw-r--r--   0 runner    (1001) docker     (122)     2135 2023-07-17 20:43:48.000000 siriuspy-2.78.0/siriuspy/envars.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-17 20:43:58.509197 siriuspy-2.78.0/siriuspy/epics/
--rw-r--r--   0 runner    (1001) docker     (122)      379 2023-07-17 20:43:48.000000 siriuspy-2.78.0/siriuspy/epics/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      624 2023-07-17 20:43:48.000000 siriuspy-2.78.0/siriuspy/epics/multiproc.py
--rw-r--r--   0 runner    (1001) docker     (122)     9097 2023-07-17 20:43:48.000000 siriuspy-2.78.0/siriuspy/epics/properties.py
--rw-r--r--   0 runner    (1001) docker     (122)      209 2023-07-17 20:43:48.000000 siriuspy-2.78.0/siriuspy/epics/pv.py
--rw-r--r--   0 runner    (1001) docker     (122)    29251 2023-07-17 20:43:48.000000 siriuspy-2.78.0/siriuspy/epics/pv_fake.py
--rw-r--r--   0 runner    (1001) docker     (122)     9170 2023-07-17 20:43:48.000000 siriuspy-2.78.0/siriuspy/epics/pv_time_serie.py
--rw-r--r--   0 runner    (1001) docker     (122)      100 2023-07-17 20:43:48.000000 siriuspy-2.78.0/siriuspy/epics/threading.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-17 20:43:58.509197 siriuspy-2.78.0/siriuspy/fofb/
--rw-r--r--   0 runner    (1001) docker     (122)       34 2023-07-17 20:43:48.000000 siriuspy-2.78.0/siriuspy/fofb/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    19263 2023-07-17 20:43:48.000000 siriuspy-2.78.0/siriuspy/fofb/csdev.py
--rw-r--r--   0 runner    (1001) docker     (122)    77425 2023-07-17 20:43:48.000000 siriuspy-2.78.0/siriuspy/fofb/main.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-17 20:43:58.509197 siriuspy-2.78.0/siriuspy/idff/
--rw-r--r--   0 runner    (1001) docker     (122)       76 2023-07-17 20:43:48.000000 siriuspy-2.78.0/siriuspy/idff/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     7315 2023-07-17 20:43:48.000000 siriuspy-2.78.0/siriuspy/idff/config.py
--rw-r--r--   0 runner    (1001) docker     (122)     3408 2023-07-17 20:43:48.000000 siriuspy-2.78.0/siriuspy/idff/csdev.py
--rw-r--r--   0 runner    (1001) docker     (122)    14175 2023-07-17 20:43:48.000000 siriuspy-2.78.0/siriuspy/idff/main.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-17 20:43:58.509197 siriuspy-2.78.0/siriuspy/injctrl/
--rw-r--r--   0 runner    (1001) docker     (122)       36 2023-07-17 20:43:48.000000 siriuspy-2.78.0/siriuspy/injctrl/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    15253 2023-07-17 20:43:48.000000 siriuspy-2.78.0/siriuspy/injctrl/bias_feedback.py
--rw-r--r--   0 runner    (1001) docker     (122)    24732 2023-07-17 20:43:48.000000 siriuspy-2.78.0/siriuspy/injctrl/csdev.py
--rw-r--r--   0 runner    (1001) docker     (122)    70114 2023-07-17 20:43:48.000000 siriuspy-2.78.0/siriuspy/injctrl/main.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-17 20:43:58.513197 siriuspy-2.78.0/siriuspy/machshift/
--rw-r--r--   0 runner    (1001) docker     (122)       32 2023-07-17 20:43:48.000000 siriuspy-2.78.0/siriuspy/machshift/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     1297 2023-07-17 20:43:48.000000 siriuspy-2.78.0/siriuspy/machshift/csdev.py
--rw-r--r--   0 runner    (1001) docker     (122)     6903 2023-07-17 20:43:48.000000 siriuspy-2.78.0/siriuspy/machshift/gensumm_macreport.py
--rw-r--r--   0 runner    (1001) docker     (122)    78928 2023-07-17 20:43:48.000000 siriuspy-2.78.0/siriuspy/machshift/macreport.py
--rw-r--r--   0 runner    (1001) docker     (122)     9197 2023-07-17 20:43:48.000000 siriuspy-2.78.0/siriuspy/machshift/macschedule.py
--rw-r--r--   0 runner    (1001) docker     (122)     2237 2023-07-17 20:43:48.000000 siriuspy-2.78.0/siriuspy/machshift/main.py
--rw-r--r--   0 runner    (1001) docker     (122)     2539 2023-07-17 20:43:48.000000 siriuspy-2.78.0/siriuspy/machshift/savedata_macreport.py
--rw-r--r--   0 runner    (1001) docker     (122)     2012 2023-07-17 20:43:48.000000 siriuspy-2.78.0/siriuspy/machshift/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-17 20:43:58.513197 siriuspy-2.78.0/siriuspy/magnet/
--rw-r--r--   0 runner    (1001) docker     (122)       25 2023-07-17 20:43:48.000000 siriuspy-2.78.0/siriuspy/magnet/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     1126 2023-07-17 20:43:48.000000 siriuspy-2.78.0/siriuspy/magnet/data.py
--rw-r--r--   0 runner    (1001) docker     (122)     8736 2023-07-17 20:43:48.000000 siriuspy-2.78.0/siriuspy/magnet/excdata.py
--rw-r--r--   0 runner    (1001) docker     (122)     1390 2023-07-17 20:43:48.000000 siriuspy-2.78.0/siriuspy/magnet/factory.py
--rw-r--r--   0 runner    (1001) docker     (122)    15453 2023-07-17 20:43:48.000000 siriuspy-2.78.0/siriuspy/magnet/normalizer.py
--rw-r--r--   0 runner    (1001) docker     (122)     7185 2023-07-17 20:43:48.000000 siriuspy-2.78.0/siriuspy/magnet/util.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-17 20:43:58.513197 siriuspy-2.78.0/siriuspy/meas/
--rw-r--r--   0 runner    (1001) docker     (122)       41 2023-07-17 20:43:48.000000 siriuspy-2.78.0/siriuspy/meas/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    11826 2023-07-17 20:43:48.000000 siriuspy-2.78.0/siriuspy/meas/csdev.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-17 20:43:58.513197 siriuspy-2.78.0/siriuspy/meas/liemit/
--rw-r--r--   0 runner    (1001) docker     (122)       57 2023-07-17 20:43:48.000000 siriuspy-2.78.0/siriuspy/meas/liemit/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     1455 2023-07-17 20:43:48.000000 siriuspy-2.78.0/siriuspy/meas/liemit/csdev.py
--rw-r--r--   0 runner    (1001) docker     (122)    13017 2023-07-17 20:43:48.000000 siriuspy-2.78.0/siriuspy/meas/liemit/main.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-17 20:43:58.513197 siriuspy-2.78.0/siriuspy/meas/lienergy/
--rw-r--r--   0 runner    (1001) docker     (122)       80 2023-07-17 20:43:48.000000 siriuspy-2.78.0/siriuspy/meas/lienergy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     2821 2023-07-17 20:43:48.000000 siriuspy-2.78.0/siriuspy/meas/lienergy/csdev.py
--rw-r--r--   0 runner    (1001) docker     (122)     8714 2023-07-17 20:43:48.000000 siriuspy-2.78.0/siriuspy/meas/lienergy/main.py
--rw-r--r--   0 runner    (1001) docker     (122)    25137 2023-07-17 20:43:48.000000 siriuspy-2.78.0/siriuspy/meas/util.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-17 20:43:58.513197 siriuspy-2.78.0/siriuspy/namesys/
--rw-r--r--   0 runner    (1001) docker     (122)       82 2023-07-17 20:43:48.000000 siriuspy-2.78.0/siriuspy/namesys/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    15210 2023-07-17 20:43:48.000000 siriuspy-2.78.0/siriuspy/namesys/implementation.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-17 20:43:58.513197 siriuspy-2.78.0/siriuspy/optics/
--rw-r--r--   0 runner    (1001) docker     (122)       25 2023-07-17 20:43:48.000000 siriuspy-2.78.0/siriuspy/optics/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      363 2023-07-17 20:43:48.000000 siriuspy-2.78.0/siriuspy/optics/constants.py
--rw-r--r--   0 runner    (1001) docker     (122)     8749 2023-07-17 20:43:48.000000 siriuspy-2.78.0/siriuspy/optics/lattice_survey.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-17 20:43:58.513197 siriuspy-2.78.0/siriuspy/opticscorr/
--rw-r--r--   0 runner    (1001) docker     (122)       29 2023-07-17 20:43:48.000000 siriuspy-2.78.0/siriuspy/opticscorr/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    34878 2023-07-17 20:43:48.000000 siriuspy-2.78.0/siriuspy/opticscorr/base.py
--rw-r--r--   0 runner    (1001) docker     (122)    16096 2023-07-17 20:43:48.000000 siriuspy-2.78.0/siriuspy/opticscorr/chrom.py
--rw-r--r--   0 runner    (1001) docker     (122)    13454 2023-07-17 20:43:48.000000 siriuspy-2.78.0/siriuspy/opticscorr/csdev.py
--rw-r--r--   0 runner    (1001) docker     (122)    18765 2023-07-17 20:43:48.000000 siriuspy-2.78.0/siriuspy/opticscorr/opticscorr.py
--rw-r--r--   0 runner    (1001) docker     (122)     8006 2023-07-17 20:43:48.000000 siriuspy-2.78.0/siriuspy/opticscorr/tune.py
--rw-r--r--   0 runner    (1001) docker     (122)     1846 2023-07-17 20:43:48.000000 siriuspy-2.78.0/siriuspy/opticscorr/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-17 20:43:58.513197 siriuspy-2.78.0/siriuspy/oscilloscope/
--rw-r--r--   0 runner    (1001) docker     (122)      104 2023-07-17 20:43:48.000000 siriuspy-2.78.0/siriuspy/oscilloscope/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     6974 2023-07-17 20:43:48.000000 siriuspy-2.78.0/siriuspy/oscilloscope/keysight.py
--rw-r--r--   0 runner    (1001) docker     (122)     1467 2023-07-17 20:43:48.000000 siriuspy-2.78.0/siriuspy/oscilloscope/scopes.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-17 20:43:58.513197 siriuspy-2.78.0/siriuspy/posang/
--rw-r--r--   0 runner    (1001) docker     (122)       25 2023-07-17 20:43:48.000000 siriuspy-2.78.0/siriuspy/posang/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     4935 2023-07-17 20:43:48.000000 siriuspy-2.78.0/siriuspy/posang/csdev.py
--rw-r--r--   0 runner    (1001) docker     (122)    19747 2023-07-17 20:43:48.000000 siriuspy-2.78.0/siriuspy/posang/main.py
--rw-r--r--   0 runner    (1001) docker     (122)     1678 2023-07-17 20:43:48.000000 siriuspy-2.78.0/siriuspy/posang/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-17 20:43:58.517197 siriuspy-2.78.0/siriuspy/pwrsupply/
--rw-r--r--   0 runner    (1001) docker     (122)      132 2023-07-17 20:43:48.000000 siriuspy-2.78.0/siriuspy/pwrsupply/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     8950 2023-07-17 20:43:48.000000 siriuspy-2.78.0/siriuspy/pwrsupply/beaglebone.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-17 20:43:58.517197 siriuspy-2.78.0/siriuspy/pwrsupply/bsmp/
--rw-r--r--   0 runner    (1001) docker     (122)       48 2023-07-17 20:43:48.000000 siriuspy-2.78.0/siriuspy/pwrsupply/bsmp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    25156 2023-07-17 20:43:48.000000 siriuspy-2.78.0/siriuspy/pwrsupply/bsmp/commands.py
--rw-r--r--   0 runner    (1001) docker     (122)    19464 2023-07-17 20:43:48.000000 siriuspy-2.78.0/siriuspy/pwrsupply/bsmp/constants.py
--rw-r--r--   0 runner    (1001) docker     (122)    53763 2023-07-17 20:43:48.000000 siriuspy-2.78.0/siriuspy/pwrsupply/bsmp/entities.py
--rw-r--r--   0 runner    (1001) docker     (122)      850 2023-07-17 20:43:48.000000 siriuspy-2.78.0/siriuspy/pwrsupply/bsmp/factory.py
--rw-r--r--   0 runner    (1001) docker     (122)   150566 2023-07-17 20:43:48.000000 siriuspy-2.78.0/siriuspy/pwrsupply/csdev.py
--rw-r--r--   0 runner    (1001) docker     (122)     3624 2023-07-17 20:43:48.000000 siriuspy-2.78.0/siriuspy/pwrsupply/data.py
--rw-r--r--   0 runner    (1001) docker     (122)    10629 2023-07-17 20:43:48.000000 siriuspy-2.78.0/siriuspy/pwrsupply/factory.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-17 20:43:58.517197 siriuspy-2.78.0/siriuspy/pwrsupply/pructrl/
--rw-r--r--   0 runner    (1001) docker     (122)      841 2023-07-17 20:43:48.000000 siriuspy-2.78.0/siriuspy/pwrsupply/pructrl/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     3393 2023-07-17 20:43:48.000000 siriuspy-2.78.0/siriuspy/pwrsupply/pructrl/pru.py
--rw-r--r--   0 runner    (1001) docker     (122)    25723 2023-07-17 20:43:48.000000 siriuspy-2.78.0/siriuspy/pwrsupply/pructrl/prucontroller.py
--rw-r--r--   0 runner    (1001) docker     (122)     6133 2023-07-17 20:43:48.000000 siriuspy-2.78.0/siriuspy/pwrsupply/pructrl/prucparms.py
--rw-r--r--   0 runner    (1001) docker     (122)    10280 2023-07-17 20:43:48.000000 siriuspy-2.78.0/siriuspy/pwrsupply/pructrl/psdevstate.py
--rw-r--r--   0 runner    (1001) docker     (122)     7712 2023-07-17 20:43:48.000000 siriuspy-2.78.0/siriuspy/pwrsupply/pructrl/udc.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-17 20:43:58.517197 siriuspy-2.78.0/siriuspy/pwrsupply/psctrl/
--rw-r--r--   0 runner    (1001) docker     (122)      866 2023-07-17 20:43:48.000000 siriuspy-2.78.0/siriuspy/pwrsupply/psctrl/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     7884 2023-07-17 20:43:48.000000 siriuspy-2.78.0/siriuspy/pwrsupply/psctrl/pscontroller.py
--rw-r--r--   0 runner    (1001) docker     (122)     6262 2023-07-17 20:43:48.000000 siriuspy-2.78.0/siriuspy/pwrsupply/psctrl/pscreaders.py
--rw-r--r--   0 runner    (1001) docker     (122)     5502 2023-07-17 20:43:48.000000 siriuspy-2.78.0/siriuspy/pwrsupply/psctrl/pscstatus.py
--rw-r--r--   0 runner    (1001) docker     (122)    17064 2023-07-17 20:43:48.000000 siriuspy-2.78.0/siriuspy/pwrsupply/psctrl/pscwriters.py
--rw-r--r--   0 runner    (1001) docker     (122)    42124 2023-07-17 20:43:48.000000 siriuspy-2.78.0/siriuspy/pwrsupply/psctrl/psmodel.py
--rw-r--r--   0 runner    (1001) docker     (122)    34142 2023-07-17 20:43:48.000000 siriuspy-2.78.0/siriuspy/pwrsupply/pssofb.py
--rw-r--r--   0 runner    (1001) docker     (122)    12500 2023-07-17 20:43:48.000000 siriuspy-2.78.0/siriuspy/pwrsupply/siggen.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-17 20:43:58.517197 siriuspy-2.78.0/siriuspy/ramp/
--rw-r--r--   0 runner    (1001) docker     (122)       23 2023-07-17 20:43:48.000000 siriuspy-2.78.0/siriuspy/ramp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    28999 2023-07-17 20:43:48.000000 siriuspy-2.78.0/siriuspy/ramp/conn.py
--rw-r--r--   0 runner    (1001) docker     (122)      346 2023-07-17 20:43:48.000000 siriuspy-2.78.0/siriuspy/ramp/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (122)     3969 2023-07-17 20:43:48.000000 siriuspy-2.78.0/siriuspy/ramp/magnet.py
--rw-r--r--   0 runner    (1001) docker     (122)    45093 2023-07-17 20:43:48.000000 siriuspy-2.78.0/siriuspy/ramp/ramp.py
--rw-r--r--   0 runner    (1001) docker     (122)    29333 2023-07-17 20:43:48.000000 siriuspy-2.78.0/siriuspy/ramp/reconst_factory.py
--rwxr-xr-x   0 runner    (1001) docker     (122)     6985 2023-07-17 20:43:48.000000 siriuspy-2.78.0/siriuspy/ramp/test_reconst_factory.py
--rwxr-xr-x   0 runner    (1001) docker     (122)     4158 2023-07-17 20:43:48.000000 siriuspy-2.78.0/siriuspy/ramp/testwfm.py
--rw-r--r--   0 runner    (1001) docker     (122)     5584 2023-07-17 20:43:48.000000 siriuspy-2.78.0/siriuspy/ramp/util.py
--rw-r--r--   0 runner    (1001) docker     (122)    30145 2023-07-17 20:43:48.000000 siriuspy-2.78.0/siriuspy/ramp/waveform.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-17 20:43:58.517197 siriuspy-2.78.0/siriuspy/search/
--rw-r--r--   0 runner    (1001) docker     (122)      359 2023-07-17 20:43:48.000000 siriuspy-2.78.0/siriuspy/search/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     3537 2023-07-17 20:43:48.000000 siriuspy-2.78.0/siriuspy/search/bpms_search.py
--rw-r--r--   0 runner    (1001) docker     (122)     6632 2023-07-17 20:43:48.000000 siriuspy-2.78.0/siriuspy/search/hl_time_search.py
--rw-r--r--   0 runner    (1001) docker     (122)     5566 2023-07-17 20:43:48.000000 siriuspy-2.78.0/siriuspy/search/id_search.py
--rw-r--r--   0 runner    (1001) docker     (122)     4152 2023-07-17 20:43:48.000000 siriuspy-2.78.0/siriuspy/search/ioc_search.py
--rw-r--r--   0 runner    (1001) docker     (122)    16917 2023-07-17 20:43:48.000000 siriuspy-2.78.0/siriuspy/search/ll_time_search.py
--rw-r--r--   0 runner    (1001) docker     (122)     7219 2023-07-17 20:43:48.000000 siriuspy-2.78.0/siriuspy/search/ma_search.py
--rw-r--r--   0 runner    (1001) docker     (122)    23882 2023-07-17 20:43:48.000000 siriuspy-2.78.0/siriuspy/search/ps_search.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-17 20:43:58.521197 siriuspy-2.78.0/siriuspy/simul/
--rw-r--r--   0 runner    (1001) docker     (122)      311 2023-07-17 20:43:48.000000 siriuspy-2.78.0/siriuspy/simul/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     2202 2023-07-17 20:43:48.000000 siriuspy-2.78.0/siriuspy/simul/simfactory.py
--rw-r--r--   0 runner    (1001) docker     (122)     6298 2023-07-17 20:43:48.000000 siriuspy-2.78.0/siriuspy/simul/simps.py
--rw-r--r--   0 runner    (1001) docker     (122)     2324 2023-07-17 20:43:48.000000 siriuspy-2.78.0/siriuspy/simul/simpv.py
--rw-r--r--   0 runner    (1001) docker     (122)     7391 2023-07-17 20:43:48.000000 siriuspy-2.78.0/siriuspy/simul/simulation.py
--rw-r--r--   0 runner    (1001) docker     (122)     4266 2023-07-17 20:43:48.000000 siriuspy-2.78.0/siriuspy/simul/simulator.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-17 20:43:58.521197 siriuspy-2.78.0/siriuspy/sofb/
--rw-r--r--   0 runner    (1001) docker     (122)       78 2023-07-17 20:43:48.000000 siriuspy-2.78.0/siriuspy/sofb/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     4869 2023-07-17 20:43:48.000000 siriuspy-2.78.0/siriuspy/sofb/base_class.py
--rw-r--r--   0 runner    (1001) docker     (122)    28072 2023-07-17 20:43:48.000000 siriuspy-2.78.0/siriuspy/sofb/bpms.py
--rw-r--r--   0 runner    (1001) docker     (122)    32010 2023-07-17 20:43:48.000000 siriuspy-2.78.0/siriuspy/sofb/correctors.py
--rw-r--r--   0 runner    (1001) docker     (122)    47062 2023-07-17 20:43:48.000000 siriuspy-2.78.0/siriuspy/sofb/csdev.py
--rw-r--r--   0 runner    (1001) docker     (122)    46398 2023-07-17 20:43:48.000000 siriuspy-2.78.0/siriuspy/sofb/main.py
--rw-r--r--   0 runner    (1001) docker     (122)    11841 2023-07-17 20:43:48.000000 siriuspy-2.78.0/siriuspy/sofb/matrix.py
--rw-r--r--   0 runner    (1001) docker     (122)    36357 2023-07-17 20:43:48.000000 siriuspy-2.78.0/siriuspy/sofb/orbit.py
--rw-r--r--   0 runner    (1001) docker     (122)     3030 2023-07-17 20:43:48.000000 siriuspy-2.78.0/siriuspy/sofb/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-17 20:43:58.521197 siriuspy-2.78.0/siriuspy/stabinfo/
--rw-r--r--   0 runner    (1001) docker     (122)       38 2023-07-17 20:43:48.000000 siriuspy-2.78.0/siriuspy/stabinfo/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     3558 2023-07-17 20:43:48.000000 siriuspy-2.78.0/siriuspy/stabinfo/csdev.py
--rw-r--r--   0 runner    (1001) docker     (122)     7708 2023-07-17 20:43:48.000000 siriuspy-2.78.0/siriuspy/stabinfo/main.py
--rw-r--r--   0 runner    (1001) docker     (122)     8598 2023-07-17 20:43:48.000000 siriuspy-2.78.0/siriuspy/thread.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-17 20:43:58.521197 siriuspy-2.78.0/siriuspy/timesys/
--rw-r--r--   0 runner    (1001) docker     (122)       26 2023-07-17 20:43:48.000000 siriuspy-2.78.0/siriuspy/timesys/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    20220 2023-07-17 20:43:48.000000 siriuspy-2.78.0/siriuspy/timesys/csdev.py
--rw-r--r--   0 runner    (1001) docker     (122)    12705 2023-07-17 20:43:48.000000 siriuspy-2.78.0/siriuspy/timesys/hl_classes.py
--rw-r--r--   0 runner    (1001) docker     (122)    33264 2023-07-17 20:43:48.000000 siriuspy-2.78.0/siriuspy/timesys/ll_classes.py
--rw-r--r--   0 runner    (1001) docker     (122)     6015 2023-07-17 20:43:48.000000 siriuspy-2.78.0/siriuspy/timesys/plot_network.py
--rw-r--r--   0 runner    (1001) docker     (122)     5957 2023-07-17 20:43:48.000000 siriuspy-2.78.0/siriuspy/timesys/static_table.py
--rw-r--r--   0 runner    (1001) docker     (122)     8732 2023-07-17 20:43:48.000000 siriuspy-2.78.0/siriuspy/util.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-17 20:43:58.497197 siriuspy-2.78.0/siriuspy.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)     1423 2023-07-17 20:43:58.000000 siriuspy-2.78.0/siriuspy.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)    10133 2023-07-17 20:43:58.000000 siriuspy-2.78.0/siriuspy.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-07-17 20:43:58.000000 siriuspy-2.78.0/siriuspy.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-07-17 20:43:58.000000 siriuspy-2.78.0/siriuspy.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (122)      128 2023-07-17 20:43:58.000000 siriuspy-2.78.0/siriuspy.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)       15 2023-07-17 20:43:58.000000 siriuspy-2.78.0/siriuspy.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-17 20:43:58.521197 siriuspy-2.78.0/tests/
--rw-r--r--   0 runner    (1001) docker     (122)      441 2023-07-17 20:43:48.000000 siriuspy-2.78.0/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-17 20:43:58.521197 siriuspy-2.78.0/tests/bsmp/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-17 20:43:48.000000 siriuspy-2.78.0/tests/bsmp/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (122)     5698 2023-07-17 20:43:48.000000 siriuspy-2.78.0/tests/bsmp/test_bsmp.py
--rwxr-xr-x   0 runner    (1001) docker     (122)    14788 2023-07-17 20:43:48.000000 siriuspy-2.78.0/tests/bsmp/test_commands.py
--rwxr-xr-x   0 runner    (1001) docker     (122)    13382 2023-07-17 20:43:48.000000 siriuspy-2.78.0/tests/bsmp/test_entities.py
--rwxr-xr-x   0 runner    (1001) docker     (122)     7719 2023-07-17 20:43:48.000000 siriuspy-2.78.0/tests/bsmp/test_serial.py
--rwxr-xr-x   0 runner    (1001) docker     (122)     1837 2023-07-17 20:43:48.000000 siriuspy-2.78.0/tests/bsmp/test_types.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-17 20:43:58.521197 siriuspy-2.78.0/tests/clientconfigdb/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-17 20:43:48.000000 siriuspy-2.78.0/tests/clientconfigdb/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (122)     2843 2023-07-17 20:43:48.000000 siriuspy-2.78.0/tests/clientconfigdb/test_configdb_client.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-17 20:43:58.521197 siriuspy-2.78.0/tests/clientweb/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-17 20:43:48.000000 siriuspy-2.78.0/tests/clientweb/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (122)    11633 2023-07-17 20:43:48.000000 siriuspy-2.78.0/tests/clientweb/test_implementation.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-17 20:43:58.521197 siriuspy-2.78.0/tests/currinfo/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-17 20:43:48.000000 siriuspy-2.78.0/tests/currinfo/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-17 20:43:58.521197 siriuspy-2.78.0/tests/currinfo/lifetime/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-17 20:43:48.000000 siriuspy-2.78.0/tests/currinfo/lifetime/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (122)     1908 2023-07-17 20:43:48.000000 siriuspy-2.78.0/tests/currinfo/lifetime/test_main.py
--rwxr-xr-x   0 runner    (1001) docker     (122)     6495 2023-07-17 20:43:48.000000 siriuspy-2.78.0/tests/currinfo/test_csdev.py
--rwxr-xr-x   0 runner    (1001) docker     (122)     2653 2023-07-17 20:43:48.000000 siriuspy-2.78.0/tests/currinfo/test_main.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-17 20:43:58.521197 siriuspy-2.78.0/tests/magnet/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-17 20:43:48.000000 siriuspy-2.78.0/tests/magnet/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (122)     2275 2023-07-17 20:43:48.000000 siriuspy-2.78.0/tests/magnet/test_factory.py
--rwxr-xr-x   0 runner    (1001) docker     (122)     2687 2023-07-17 20:43:48.000000 siriuspy-2.78.0/tests/magnet/tests_normalizer.py
--rwxr-xr-x   0 runner    (1001) docker     (122)     3618 2023-07-17 20:43:48.000000 siriuspy-2.78.0/tests/mock_servweb.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-17 20:43:58.521197 siriuspy-2.78.0/tests/namesys/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-17 20:43:48.000000 siriuspy-2.78.0/tests/namesys/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (122)     4896 2023-07-17 20:43:48.000000 siriuspy-2.78.0/tests/namesys/test_implementation.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-17 20:43:58.525197 siriuspy-2.78.0/tests/opticscorr/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-17 20:43:48.000000 siriuspy-2.78.0/tests/opticscorr/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     5490 2023-07-17 20:43:48.000000 siriuspy-2.78.0/tests/opticscorr/test_chrom.py
--rwxr-xr-x   0 runner    (1001) docker     (122)     4609 2023-07-17 20:43:48.000000 siriuspy-2.78.0/tests/opticscorr/test_csdev.py
--rwxr-xr-x   0 runner    (1001) docker     (122)    23381 2023-07-17 20:43:48.000000 siriuspy-2.78.0/tests/opticscorr/test_opticscorr.py
--rw-r--r--   0 runner    (1001) docker     (122)     5692 2023-07-17 20:43:48.000000 siriuspy-2.78.0/tests/opticscorr/test_tune.py
--rw-r--r--   0 runner    (1001) docker     (122)     1145 2023-07-17 20:43:48.000000 siriuspy-2.78.0/tests/opticscorr/test_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-17 20:43:58.525197 siriuspy-2.78.0/tests/posang/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-17 20:43:48.000000 siriuspy-2.78.0/tests/posang/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (122)     2872 2023-07-17 20:43:48.000000 siriuspy-2.78.0/tests/posang/test_csdev.py
--rwxr-xr-x   0 runner    (1001) docker     (122)     3164 2023-07-17 20:43:48.000000 siriuspy-2.78.0/tests/posang/test_main.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-17 20:43:58.525197 siriuspy-2.78.0/tests/pwrsupply/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-17 20:43:48.000000 siriuspy-2.78.0/tests/pwrsupply/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    18979 2023-07-17 20:43:48.000000 siriuspy-2.78.0/tests/pwrsupply/db.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-17 20:43:58.525197 siriuspy-2.78.0/tests/pwrsupply/pructrl/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-17 20:43:48.000000 siriuspy-2.78.0/tests/pwrsupply/pructrl/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (122)     2257 2023-07-17 20:43:48.000000 siriuspy-2.78.0/tests/pwrsupply/pructrl/test_pru.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-17 20:43:58.525197 siriuspy-2.78.0/tests/pwrsupply/psctrl/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-17 20:43:48.000000 siriuspy-2.78.0/tests/pwrsupply/psctrl/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     4853 2023-07-17 20:43:48.000000 siriuspy-2.78.0/tests/pwrsupply/psctrl/test_pscwriters.py
--rwxr-xr-x   0 runner    (1001) docker     (122)      166 2023-07-17 20:43:48.000000 siriuspy-2.78.0/tests/pwrsupply/test_beaglebone.py
--rwxr-xr-x   0 runner    (1001) docker     (122)       89 2023-07-17 20:43:48.000000 siriuspy-2.78.0/tests/pwrsupply/test_bsmp.py
--rwxr-xr-x   0 runner    (1001) docker     (122)     6439 2023-07-17 20:43:48.000000 siriuspy-2.78.0/tests/pwrsupply/test_csdev.py
--rwxr-xr-x   0 runner    (1001) docker     (122)     7331 2023-07-17 20:43:48.000000 siriuspy-2.78.0/tests/pwrsupply/test_data.py
--rwxr-xr-x   0 runner    (1001) docker     (122)     2323 2023-07-17 20:43:48.000000 siriuspy-2.78.0/tests/pwrsupply/test_siggen.py
--rw-r--r--   0 runner    (1001) docker     (122)     3146 2023-07-17 20:43:48.000000 siriuspy-2.78.0/tests/pwrsupply/variables.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-17 20:43:58.525197 siriuspy-2.78.0/tests/ramp/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-17 20:43:48.000000 siriuspy-2.78.0/tests/ramp/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (122)     5699 2023-07-17 20:43:48.000000 siriuspy-2.78.0/tests/ramp/test_magnet.py
--rwxr-xr-x   0 runner    (1001) docker     (122)     7235 2023-07-17 20:43:48.000000 siriuspy-2.78.0/tests/ramp/test_waveform.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-17 20:43:58.525197 siriuspy-2.78.0/tests/search/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-17 20:43:48.000000 siriuspy-2.78.0/tests/search/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (122)     2412 2023-07-17 20:43:48.000000 siriuspy-2.78.0/tests/search/test_hl_time_search.py
--rwxr-xr-x   0 runner    (1001) docker     (122)      559 2023-07-17 20:43:48.000000 siriuspy-2.78.0/tests/search/test_init.py
--rwxr-xr-x   0 runner    (1001) docker     (122)     3831 2023-07-17 20:43:48.000000 siriuspy-2.78.0/tests/search/test_ll_time_search.py
--rwxr-xr-x   0 runner    (1001) docker     (122)     6120 2023-07-17 20:43:48.000000 siriuspy-2.78.0/tests/search/test_ma_search.py
--rwxr-xr-x   0 runner    (1001) docker     (122)    13502 2023-07-17 20:43:48.000000 siriuspy-2.78.0/tests/search/test_ps_search.py
--rw-r--r--   0 runner    (1001) docker     (122)     3478 2023-07-17 20:43:48.000000 siriuspy-2.78.0/tests/test_callbacks.py
--rwxr-xr-x   0 runner    (1001) docker     (122)     1009 2023-07-17 20:43:48.000000 siriuspy-2.78.0/tests/test_csdev.py
--rwxr-xr-x   0 runner    (1001) docker     (122)     1605 2023-07-17 20:43:48.000000 siriuspy-2.78.0/tests/test_envars.py
--rwxr-xr-x   0 runner    (1001) docker     (122)    11533 2023-07-17 20:43:48.000000 siriuspy-2.78.0/tests/test_util.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-17 20:43:58.525197 siriuspy-2.78.0/tests/timesys/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-17 20:43:48.000000 siriuspy-2.78.0/tests/timesys/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (122)     4999 2023-07-17 20:43:48.000000 siriuspy-2.78.0/tests/timesys/test_csdev.py
--rw-r--r--   0 runner    (1001) docker     (122)      978 2023-07-17 20:43:48.000000 siriuspy-2.78.0/tests/timesys/test_plot_network.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-30 14:45:12.893647 siriuspy-2.79.0/
+-rw-r--r--   0 runner    (1001) docker     (122)    34494 2023-07-30 14:45:00.000000 siriuspy-2.79.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (122)       90 2023-07-30 14:45:00.000000 siriuspy-2.79.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (122)     1423 2023-07-30 14:45:12.893647 siriuspy-2.79.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)      954 2023-07-30 14:45:00.000000 siriuspy-2.79.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (122)      128 2023-07-30 14:45:00.000000 siriuspy-2.79.0/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       38 2023-07-30 14:45:12.893647 siriuspy-2.79.0/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (122)     1243 2023-07-30 14:45:00.000000 siriuspy-2.79.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-30 14:45:12.853647 siriuspy-2.79.0/siriuspy/
+-rw-r--r--   0 runner    (1001) docker     (122)        7 2023-07-30 14:45:00.000000 siriuspy-2.79.0/siriuspy/VERSION
+-rw-r--r--   0 runner    (1001) docker     (122)      515 2023-07-30 14:45:00.000000 siriuspy-2.79.0/siriuspy/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-30 14:45:12.857647 siriuspy-2.79.0/siriuspy/bsmp/
+-rw-r--r--   0 runner    (1001) docker     (122)      422 2023-07-30 14:45:00.000000 siriuspy-2.79.0/siriuspy/bsmp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    15885 2023-07-30 14:45:00.000000 siriuspy-2.79.0/siriuspy/bsmp/commands.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1904 2023-07-30 14:45:00.000000 siriuspy-2.79.0/siriuspy/bsmp/constants.py
+-rw-r--r--   0 runner    (1001) docker     (122)    11790 2023-07-30 14:45:00.000000 siriuspy-2.79.0/siriuspy/bsmp/entities.py
+-rw-r--r--   0 runner    (1001) docker     (122)      610 2023-07-30 14:45:00.000000 siriuspy-2.79.0/siriuspy/bsmp/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (122)     8110 2023-07-30 14:45:00.000000 siriuspy-2.79.0/siriuspy/bsmp/serial.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1204 2023-07-30 14:45:00.000000 siriuspy-2.79.0/siriuspy/bsmp/types.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2992 2023-07-30 14:45:00.000000 siriuspy-2.79.0/siriuspy/callbacks.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-30 14:45:12.857647 siriuspy-2.79.0/siriuspy/clientarch/
+-rw-r--r--   0 runner    (1001) docker     (122)      306 2023-07-30 14:45:00.000000 siriuspy-2.79.0/siriuspy/clientarch/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    13813 2023-07-30 14:45:00.000000 siriuspy-2.79.0/siriuspy/clientarch/client.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6392 2023-07-30 14:45:00.000000 siriuspy-2.79.0/siriuspy/clientarch/devices.py
+-rw-r--r--   0 runner    (1001) docker     (122)      643 2023-07-30 14:45:00.000000 siriuspy-2.79.0/siriuspy/clientarch/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (122)    20400 2023-07-30 14:45:00.000000 siriuspy-2.79.0/siriuspy/clientarch/pvarch.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5003 2023-07-30 14:45:00.000000 siriuspy-2.79.0/siriuspy/clientarch/time.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-30 14:45:12.857647 siriuspy-2.79.0/siriuspy/clientconfigdb/
+-rw-r--r--   0 runner    (1001) docker     (122)      227 2023-07-30 14:45:00.000000 siriuspy-2.79.0/siriuspy/clientconfigdb/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3345 2023-07-30 14:45:00.000000 siriuspy-2.79.0/siriuspy/clientconfigdb/_templates.py
+-rw-r--r--   0 runner    (1001) docker     (122)     9599 2023-07-30 14:45:00.000000 siriuspy-2.79.0/siriuspy/clientconfigdb/configdb_client.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5448 2023-07-30 14:45:00.000000 siriuspy-2.79.0/siriuspy/clientconfigdb/configdb_document.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4785 2023-07-30 14:45:00.000000 siriuspy-2.79.0/siriuspy/clientconfigdb/pvsconfig.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-30 14:45:12.865647 siriuspy-2.79.0/siriuspy/clientconfigdb/types/
+-rw-r--r--   0 runner    (1001) docker     (122)      286 2023-07-30 14:45:00.000000 siriuspy-2.79.0/siriuspy/clientconfigdb/types/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    13746 2023-07-30 14:45:00.000000 siriuspy-2.79.0/siriuspy/clientconfigdb/types/as_corrloop_params.py
+-rw-r--r--   0 runner    (1001) docker     (122)    49080 2023-07-30 14:45:00.000000 siriuspy-2.79.0/siriuspy/clientconfigdb/types/as_diagnostics.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6681 2023-07-30 14:45:00.000000 siriuspy-2.79.0/siriuspy/clientconfigdb/types/as_pwrstate.py
+-rw-r--r--   0 runner    (1001) docker     (122)    34247 2023-07-30 14:45:00.000000 siriuspy-2.79.0/siriuspy/clientconfigdb/types/as_rf.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1135 2023-07-30 14:45:00.000000 siriuspy-2.79.0/siriuspy/clientconfigdb/types/bo_chromcorr_params.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3984 2023-07-30 14:45:00.000000 siriuspy-2.79.0/siriuspy/clientconfigdb/types/bo_normalized.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1135 2023-07-30 14:45:00.000000 siriuspy-2.79.0/siriuspy/clientconfigdb/types/bo_orbcorr_respm.py
+-rw-r--r--   0 runner    (1001) docker     (122)      700 2023-07-30 14:45:00.000000 siriuspy-2.79.0/siriuspy/clientconfigdb/types/bo_orbit.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3042 2023-07-30 14:45:00.000000 siriuspy-2.79.0/siriuspy/clientconfigdb/types/bo_ramp.py
+-rw-r--r--   0 runner    (1001) docker     (122)      975 2023-07-30 14:45:00.000000 siriuspy-2.79.0/siriuspy/clientconfigdb/types/bo_tunecorr_params.py
+-rw-r--r--   0 runner    (1001) docker     (122)   124502 2023-07-30 14:45:00.000000 siriuspy-2.79.0/siriuspy/clientconfigdb/types/global_config.py
+-rw-r--r--   0 runner    (1001) docker     (122)      735 2023-07-30 14:45:00.000000 siriuspy-2.79.0/siriuspy/clientconfigdb/types/si_bbadata.py
+-rw-r--r--   0 runner    (1001) docker     (122)    18619 2023-07-30 14:45:00.000000 siriuspy-2.79.0/siriuspy/clientconfigdb/types/si_bbbproc.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1697 2023-07-30 14:45:00.000000 siriuspy-2.79.0/siriuspy/clientconfigdb/types/si_chromcorr_params.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1146 2023-07-30 14:45:00.000000 siriuspy-2.79.0/siriuspy/clientconfigdb/types/si_fastorbcorr_respm.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4741 2023-07-30 14:45:00.000000 siriuspy-2.79.0/siriuspy/clientconfigdb/types/si_fofb.py
+-rw-r--r--   0 runner    (1001) docker     (122)      957 2023-07-30 14:45:00.000000 siriuspy-2.79.0/siriuspy/clientconfigdb/types/si_id.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3181 2023-07-30 14:45:00.000000 siriuspy-2.79.0/siriuspy/clientconfigdb/types/si_idff.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1136 2023-07-30 14:45:00.000000 siriuspy-2.79.0/siriuspy/clientconfigdb/types/si_orbcorr_respm.py
+-rw-r--r--   0 runner    (1001) docker     (122)      701 2023-07-30 14:45:00.000000 siriuspy-2.79.0/siriuspy/clientconfigdb/types/si_orbit.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1290 2023-07-30 14:45:00.000000 siriuspy-2.79.0/siriuspy/clientconfigdb/types/si_tunecorr_params.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1738 2023-07-30 14:45:00.000000 siriuspy-2.79.0/siriuspy/clientconfigdb/types/tb_normalized.py
+-rw-r--r--   0 runner    (1001) docker     (122)      969 2023-07-30 14:45:00.000000 siriuspy-2.79.0/siriuspy/clientconfigdb/types/tb_orbcorr_respm.py
+-rw-r--r--   0 runner    (1001) docker     (122)      693 2023-07-30 14:45:00.000000 siriuspy-2.79.0/siriuspy/clientconfigdb/types/tb_orbit.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1651 2023-07-30 14:45:00.000000 siriuspy-2.79.0/siriuspy/clientconfigdb/types/tb_posang_respm.py
+-rw-r--r--   0 runner    (1001) docker     (122)      969 2023-07-30 14:45:00.000000 siriuspy-2.79.0/siriuspy/clientconfigdb/types/ts_orbcorr_respm.py
+-rw-r--r--   0 runner    (1001) docker     (122)      693 2023-07-30 14:45:00.000000 siriuspy-2.79.0/siriuspy/clientconfigdb/types/ts_orbit.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1721 2023-07-30 14:45:00.000000 siriuspy-2.79.0/siriuspy/clientconfigdb/types/ts_posang_respm.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-30 14:45:12.865647 siriuspy-2.79.0/siriuspy/clientweb/
+-rw-r--r--   0 runner    (1001) docker     (122)       50 2023-07-30 14:45:00.000000 siriuspy-2.79.0/siriuspy/clientweb/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5896 2023-07-30 14:45:00.000000 siriuspy-2.79.0/siriuspy/clientweb/implementation.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2236 2023-07-30 14:45:00.000000 siriuspy-2.79.0/siriuspy/csdev.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-30 14:45:12.865647 siriuspy-2.79.0/siriuspy/currinfo/
+-rw-r--r--   0 runner    (1001) docker     (122)      144 2023-07-30 14:45:00.000000 siriuspy-2.79.0/siriuspy/currinfo/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     9620 2023-07-30 14:45:00.000000 siriuspy-2.79.0/siriuspy/currinfo/csdev.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-30 14:45:12.865647 siriuspy-2.79.0/siriuspy/currinfo/lifetime/
+-rw-r--r--   0 runner    (1001) docker     (122)       72 2023-07-30 14:45:00.000000 siriuspy-2.79.0/siriuspy/currinfo/lifetime/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    12607 2023-07-30 14:45:00.000000 siriuspy-2.79.0/siriuspy/currinfo/lifetime/main.py
+-rw-r--r--   0 runner    (1001) docker     (122)    23275 2023-07-30 14:45:00.000000 siriuspy-2.79.0/siriuspy/currinfo/main.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-30 14:45:12.865647 siriuspy-2.79.0/siriuspy/cycle/
+-rw-r--r--   0 runner    (1001) docker     (122)      514 2023-07-30 14:45:00.000000 siriuspy-2.79.0/siriuspy/cycle/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)   104994 2023-07-30 14:45:00.000000 siriuspy-2.79.0/siriuspy/cycle/bo_cycle_data.py
+-rw-r--r--   0 runner    (1001) docker     (122)    31135 2023-07-30 14:45:00.000000 siriuspy-2.79.0/siriuspy/cycle/conn.py
+-rw-r--r--   0 runner    (1001) docker     (122)     9781 2023-07-30 14:45:00.000000 siriuspy-2.79.0/siriuspy/cycle/fc_cycle_data.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3286 2023-07-30 14:45:00.000000 siriuspy-2.79.0/siriuspy/cycle/li_cycle_data.py
+-rw-r--r--   0 runner    (1001) docker     (122)    38408 2023-07-30 14:45:00.000000 siriuspy-2.79.0/siriuspy/cycle/main.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3574 2023-07-30 14:45:00.000000 siriuspy-2.79.0/siriuspy/cycle/util.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-30 14:45:12.869647 siriuspy-2.79.0/siriuspy/devices/
+-rw-r--r--   0 runner    (1001) docker     (122)     1969 2023-07-30 14:45:00.000000 siriuspy-2.79.0/siriuspy/devices/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4172 2023-07-30 14:45:00.000000 siriuspy-2.79.0/siriuspy/devices/afc_acq_core.py
+-rw-r--r--   0 runner    (1001) docker     (122)    48546 2023-07-30 14:45:00.000000 siriuspy-2.79.0/siriuspy/devices/bbb.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2786 2023-07-30 14:45:00.000000 siriuspy-2.79.0/siriuspy/devices/blctrl.py
+-rw-r--r--   0 runner    (1001) docker     (122)    40718 2023-07-30 14:45:00.000000 siriuspy-2.79.0/siriuspy/devices/bpm.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7380 2023-07-30 14:45:00.000000 siriuspy-2.79.0/siriuspy/devices/currinfo.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2402 2023-07-30 14:45:00.000000 siriuspy-2.79.0/siriuspy/devices/dcct.py
+-rw-r--r--   0 runner    (1001) docker     (122)    13949 2023-07-30 14:45:00.000000 siriuspy-2.79.0/siriuspy/devices/device.py
+-rw-r--r--   0 runner    (1001) docker     (122)    19400 2023-07-30 14:45:00.000000 siriuspy-2.79.0/siriuspy/devices/dvf.py
+-rw-r--r--   0 runner    (1001) docker     (122)    30814 2023-07-30 14:45:00.000000 siriuspy-2.79.0/siriuspy/devices/egun.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1743 2023-07-30 14:45:00.000000 siriuspy-2.79.0/siriuspy/devices/energy.py
+-rw-r--r--   0 runner    (1001) docker     (122)    51455 2023-07-30 14:45:00.000000 siriuspy-2.79.0/siriuspy/devices/fofb.py
+-rw-r--r--   0 runner    (1001) docker     (122)    46088 2023-07-30 14:45:00.000000 siriuspy-2.79.0/siriuspy/devices/fofb_acq.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2121 2023-07-30 14:45:00.000000 siriuspy-2.79.0/siriuspy/devices/ict.py
+-rw-r--r--   0 runner    (1001) docker     (122)    10051 2023-07-30 14:45:00.000000 siriuspy-2.79.0/siriuspy/devices/idff.py
+-rw-r--r--   0 runner    (1001) docker     (122)    21328 2023-07-30 14:45:00.000000 siriuspy-2.79.0/siriuspy/devices/ids.py
+-rw-r--r--   0 runner    (1001) docker     (122)    20759 2023-07-30 14:45:00.000000 siriuspy-2.79.0/siriuspy/devices/injctrl.py
+-rw-r--r--   0 runner    (1001) docker     (122)    38127 2023-07-30 14:45:00.000000 siriuspy-2.79.0/siriuspy/devices/injsys.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1630 2023-07-30 14:45:00.000000 siriuspy-2.79.0/siriuspy/devices/lienergy.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6948 2023-07-30 14:45:00.000000 siriuspy-2.79.0/siriuspy/devices/lillrf.py
+-rw-r--r--   0 runner    (1001) docker     (122)      964 2023-07-30 14:45:00.000000 siriuspy-2.79.0/siriuspy/devices/machshift.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2290 2023-07-30 14:45:00.000000 siriuspy-2.79.0/siriuspy/devices/modltr.py
+-rw-r--r--   0 runner    (1001) docker     (122)    36084 2023-07-30 14:45:00.000000 siriuspy-2.79.0/siriuspy/devices/orbit_interlock.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2427 2023-07-30 14:45:00.000000 siriuspy-2.79.0/siriuspy/devices/posang.py
+-rw-r--r--   0 runner    (1001) docker     (122)    10195 2023-07-30 14:45:00.000000 siriuspy-2.79.0/siriuspy/devices/psconv.py
+-rw-r--r--   0 runner    (1001) docker     (122)    12184 2023-07-30 14:45:00.000000 siriuspy-2.79.0/siriuspy/devices/pssofb.py
+-rw-r--r--   0 runner    (1001) docker     (122)    20070 2023-07-30 14:45:00.000000 siriuspy-2.79.0/siriuspy/devices/pstesters.py
+-rw-r--r--   0 runner    (1001) docker     (122)    30064 2023-07-30 14:45:00.000000 siriuspy-2.79.0/siriuspy/devices/pwrsupply.py
+-rw-r--r--   0 runner    (1001) docker     (122)    35448 2023-07-30 14:45:00.000000 siriuspy-2.79.0/siriuspy/devices/rf.py
+-rw-r--r--   0 runner    (1001) docker     (122)     8522 2023-07-30 14:45:00.000000 siriuspy-2.79.0/siriuspy/devices/scraper.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3836 2023-07-30 14:45:00.000000 siriuspy-2.79.0/siriuspy/devices/screen.py
+-rw-r--r--   0 runner    (1001) docker     (122)    25271 2023-07-30 14:45:00.000000 siriuspy-2.79.0/siriuspy/devices/sofb.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2652 2023-07-30 14:45:00.000000 siriuspy-2.79.0/siriuspy/devices/syncd.py
+-rw-r--r--   0 runner    (1001) docker     (122)    17907 2023-07-30 14:45:00.000000 siriuspy-2.79.0/siriuspy/devices/timing.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5055 2023-07-30 14:45:00.000000 siriuspy-2.79.0/siriuspy/devices/tune.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-30 14:45:12.869647 siriuspy-2.79.0/siriuspy/diagbeam/
+-rw-r--r--   0 runner    (1001) docker     (122)       30 2023-07-30 14:45:00.000000 siriuspy-2.79.0/siriuspy/diagbeam/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-30 14:45:12.869647 siriuspy-2.79.0/siriuspy/diagbeam/bpm/
+-rw-r--r--   0 runner    (1001) docker     (122)       24 2023-07-30 14:45:00.000000 siriuspy-2.79.0/siriuspy/diagbeam/bpm/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    24054 2023-07-30 14:45:00.000000 siriuspy-2.79.0/siriuspy/diagbeam/bpm/csdev.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-30 14:45:12.869647 siriuspy-2.79.0/siriuspy/diagbeam/dcct/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-30 14:45:00.000000 siriuspy-2.79.0/siriuspy/diagbeam/dcct/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     8215 2023-07-30 14:45:00.000000 siriuspy-2.79.0/siriuspy/diagbeam/dcct/csdev.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-30 14:45:12.869647 siriuspy-2.79.0/siriuspy/diagbeam/ict/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-30 14:45:00.000000 siriuspy-2.79.0/siriuspy/diagbeam/ict/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4878 2023-07-30 14:45:00.000000 siriuspy-2.79.0/siriuspy/diagbeam/ict/csdev.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-30 14:45:12.869647 siriuspy-2.79.0/siriuspy/diagbeam/screen/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-30 14:45:00.000000 siriuspy-2.79.0/siriuspy/diagbeam/screen/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    12756 2023-07-30 14:45:00.000000 siriuspy-2.79.0/siriuspy/diagbeam/screen/csdev.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-30 14:45:12.869647 siriuspy-2.79.0/siriuspy/diagbeam/slit/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-30 14:45:00.000000 siriuspy-2.79.0/siriuspy/diagbeam/slit/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6750 2023-07-30 14:45:00.000000 siriuspy-2.79.0/siriuspy/diagbeam/slit/csdev.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-30 14:45:12.869647 siriuspy-2.79.0/siriuspy/diagsys/
+-rw-r--r--   0 runner    (1001) docker     (122)       26 2023-07-30 14:45:00.000000 siriuspy-2.79.0/siriuspy/diagsys/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1484 2023-07-30 14:45:00.000000 siriuspy-2.79.0/siriuspy/diagsys/app.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-30 14:45:12.869647 siriuspy-2.79.0/siriuspy/diagsys/lidiag/
+-rw-r--r--   0 runner    (1001) docker     (122)       29 2023-07-30 14:45:00.000000 siriuspy-2.79.0/siriuspy/diagsys/lidiag/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5193 2023-07-30 14:45:00.000000 siriuspy-2.79.0/siriuspy/diagsys/lidiag/csdev.py
+-rw-r--r--   0 runner    (1001) docker     (122)     8168 2023-07-30 14:45:00.000000 siriuspy-2.79.0/siriuspy/diagsys/lidiag/main.py
+-rw-r--r--   0 runner    (1001) docker     (122)     8774 2023-07-30 14:45:00.000000 siriuspy-2.79.0/siriuspy/diagsys/lidiag/pvs.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-30 14:45:12.873647 siriuspy-2.79.0/siriuspy/diagsys/psdiag/
+-rw-r--r--   0 runner    (1001) docker     (122)       25 2023-07-30 14:45:00.000000 siriuspy-2.79.0/siriuspy/diagsys/psdiag/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2699 2023-07-30 14:45:00.000000 siriuspy-2.79.0/siriuspy/diagsys/psdiag/csdev.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4582 2023-07-30 14:45:00.000000 siriuspy-2.79.0/siriuspy/diagsys/psdiag/main.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7692 2023-07-30 14:45:00.000000 siriuspy-2.79.0/siriuspy/diagsys/psdiag/pvs.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-30 14:45:12.873647 siriuspy-2.79.0/siriuspy/diagsys/pudiag/
+-rw-r--r--   0 runner    (1001) docker     (122)       25 2023-07-30 14:45:00.000000 siriuspy-2.79.0/siriuspy/diagsys/pudiag/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1418 2023-07-30 14:45:00.000000 siriuspy-2.79.0/siriuspy/diagsys/pudiag/csdev.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2871 2023-07-30 14:45:00.000000 siriuspy-2.79.0/siriuspy/diagsys/pudiag/main.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4099 2023-07-30 14:45:00.000000 siriuspy-2.79.0/siriuspy/diagsys/pudiag/pvs.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6792 2023-07-30 14:45:00.000000 siriuspy-2.79.0/siriuspy/diagsys/pvs.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-30 14:45:12.873647 siriuspy-2.79.0/siriuspy/diagsys/rfdiag/
+-rw-r--r--   0 runner    (1001) docker     (122)       25 2023-07-30 14:45:00.000000 siriuspy-2.79.0/siriuspy/diagsys/rfdiag/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2409 2023-07-30 14:45:00.000000 siriuspy-2.79.0/siriuspy/diagsys/rfdiag/csdev.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3783 2023-07-30 14:45:00.000000 siriuspy-2.79.0/siriuspy/diagsys/rfdiag/main.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4891 2023-07-30 14:45:00.000000 siriuspy-2.79.0/siriuspy/diagsys/rfdiag/pvs.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-30 14:45:12.873647 siriuspy-2.79.0/siriuspy/dvfimgproc/
+-rw-r--r--   0 runner    (1001) docker     (122)       39 2023-07-30 14:45:00.000000 siriuspy-2.79.0/siriuspy/dvfimgproc/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7692 2023-07-30 14:45:00.000000 siriuspy-2.79.0/siriuspy/dvfimgproc/csdev.py
+-rw-r--r--   0 runner    (1001) docker     (122)    15295 2023-07-30 14:45:00.000000 siriuspy-2.79.0/siriuspy/dvfimgproc/main.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7082 2023-07-30 14:45:00.000000 siriuspy-2.79.0/siriuspy/dvfimgproc/meas.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2135 2023-07-30 14:45:00.000000 siriuspy-2.79.0/siriuspy/envars.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-30 14:45:12.873647 siriuspy-2.79.0/siriuspy/epics/
+-rw-r--r--   0 runner    (1001) docker     (122)      379 2023-07-30 14:45:00.000000 siriuspy-2.79.0/siriuspy/epics/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      624 2023-07-30 14:45:00.000000 siriuspy-2.79.0/siriuspy/epics/multiproc.py
+-rw-r--r--   0 runner    (1001) docker     (122)     9097 2023-07-30 14:45:00.000000 siriuspy-2.79.0/siriuspy/epics/properties.py
+-rw-r--r--   0 runner    (1001) docker     (122)      209 2023-07-30 14:45:00.000000 siriuspy-2.79.0/siriuspy/epics/pv.py
+-rw-r--r--   0 runner    (1001) docker     (122)    29251 2023-07-30 14:45:00.000000 siriuspy-2.79.0/siriuspy/epics/pv_fake.py
+-rw-r--r--   0 runner    (1001) docker     (122)     9170 2023-07-30 14:45:00.000000 siriuspy-2.79.0/siriuspy/epics/pv_time_serie.py
+-rw-r--r--   0 runner    (1001) docker     (122)      100 2023-07-30 14:45:00.000000 siriuspy-2.79.0/siriuspy/epics/threading.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-30 14:45:12.873647 siriuspy-2.79.0/siriuspy/fofb/
+-rw-r--r--   0 runner    (1001) docker     (122)       34 2023-07-30 14:45:00.000000 siriuspy-2.79.0/siriuspy/fofb/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    19263 2023-07-30 14:45:00.000000 siriuspy-2.79.0/siriuspy/fofb/csdev.py
+-rw-r--r--   0 runner    (1001) docker     (122)    77425 2023-07-30 14:45:00.000000 siriuspy-2.79.0/siriuspy/fofb/main.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-30 14:45:12.873647 siriuspy-2.79.0/siriuspy/idff/
+-rw-r--r--   0 runner    (1001) docker     (122)       76 2023-07-30 14:45:00.000000 siriuspy-2.79.0/siriuspy/idff/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7315 2023-07-30 14:45:00.000000 siriuspy-2.79.0/siriuspy/idff/config.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3408 2023-07-30 14:45:00.000000 siriuspy-2.79.0/siriuspy/idff/csdev.py
+-rw-r--r--   0 runner    (1001) docker     (122)    14175 2023-07-30 14:45:00.000000 siriuspy-2.79.0/siriuspy/idff/main.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-30 14:45:12.873647 siriuspy-2.79.0/siriuspy/injctrl/
+-rw-r--r--   0 runner    (1001) docker     (122)       36 2023-07-30 14:45:00.000000 siriuspy-2.79.0/siriuspy/injctrl/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    15253 2023-07-30 14:45:00.000000 siriuspy-2.79.0/siriuspy/injctrl/bias_feedback.py
+-rw-r--r--   0 runner    (1001) docker     (122)    24732 2023-07-30 14:45:00.000000 siriuspy-2.79.0/siriuspy/injctrl/csdev.py
+-rw-r--r--   0 runner    (1001) docker     (122)    70114 2023-07-30 14:45:00.000000 siriuspy-2.79.0/siriuspy/injctrl/main.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-30 14:45:12.877647 siriuspy-2.79.0/siriuspy/machshift/
+-rw-r--r--   0 runner    (1001) docker     (122)       32 2023-07-30 14:45:00.000000 siriuspy-2.79.0/siriuspy/machshift/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1297 2023-07-30 14:45:00.000000 siriuspy-2.79.0/siriuspy/machshift/csdev.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6903 2023-07-30 14:45:00.000000 siriuspy-2.79.0/siriuspy/machshift/gensumm_macreport.py
+-rw-r--r--   0 runner    (1001) docker     (122)    78928 2023-07-30 14:45:00.000000 siriuspy-2.79.0/siriuspy/machshift/macreport.py
+-rw-r--r--   0 runner    (1001) docker     (122)     9197 2023-07-30 14:45:00.000000 siriuspy-2.79.0/siriuspy/machshift/macschedule.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2237 2023-07-30 14:45:00.000000 siriuspy-2.79.0/siriuspy/machshift/main.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2539 2023-07-30 14:45:00.000000 siriuspy-2.79.0/siriuspy/machshift/savedata_macreport.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2012 2023-07-30 14:45:00.000000 siriuspy-2.79.0/siriuspy/machshift/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-30 14:45:12.877647 siriuspy-2.79.0/siriuspy/magnet/
+-rw-r--r--   0 runner    (1001) docker     (122)       25 2023-07-30 14:45:00.000000 siriuspy-2.79.0/siriuspy/magnet/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1126 2023-07-30 14:45:00.000000 siriuspy-2.79.0/siriuspy/magnet/data.py
+-rw-r--r--   0 runner    (1001) docker     (122)     8736 2023-07-30 14:45:00.000000 siriuspy-2.79.0/siriuspy/magnet/excdata.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1390 2023-07-30 14:45:00.000000 siriuspy-2.79.0/siriuspy/magnet/factory.py
+-rw-r--r--   0 runner    (1001) docker     (122)    15453 2023-07-30 14:45:00.000000 siriuspy-2.79.0/siriuspy/magnet/normalizer.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7185 2023-07-30 14:45:00.000000 siriuspy-2.79.0/siriuspy/magnet/util.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-30 14:45:12.877647 siriuspy-2.79.0/siriuspy/meas/
+-rw-r--r--   0 runner    (1001) docker     (122)       41 2023-07-30 14:45:00.000000 siriuspy-2.79.0/siriuspy/meas/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    11826 2023-07-30 14:45:00.000000 siriuspy-2.79.0/siriuspy/meas/csdev.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-30 14:45:12.877647 siriuspy-2.79.0/siriuspy/meas/liemit/
+-rw-r--r--   0 runner    (1001) docker     (122)       57 2023-07-30 14:45:00.000000 siriuspy-2.79.0/siriuspy/meas/liemit/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1455 2023-07-30 14:45:00.000000 siriuspy-2.79.0/siriuspy/meas/liemit/csdev.py
+-rw-r--r--   0 runner    (1001) docker     (122)    13017 2023-07-30 14:45:00.000000 siriuspy-2.79.0/siriuspy/meas/liemit/main.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-30 14:45:12.877647 siriuspy-2.79.0/siriuspy/meas/lienergy/
+-rw-r--r--   0 runner    (1001) docker     (122)       80 2023-07-30 14:45:00.000000 siriuspy-2.79.0/siriuspy/meas/lienergy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2821 2023-07-30 14:45:00.000000 siriuspy-2.79.0/siriuspy/meas/lienergy/csdev.py
+-rw-r--r--   0 runner    (1001) docker     (122)     8714 2023-07-30 14:45:00.000000 siriuspy-2.79.0/siriuspy/meas/lienergy/main.py
+-rw-r--r--   0 runner    (1001) docker     (122)    25137 2023-07-30 14:45:00.000000 siriuspy-2.79.0/siriuspy/meas/util.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-30 14:45:12.877647 siriuspy-2.79.0/siriuspy/namesys/
+-rw-r--r--   0 runner    (1001) docker     (122)       82 2023-07-30 14:45:00.000000 siriuspy-2.79.0/siriuspy/namesys/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    15210 2023-07-30 14:45:00.000000 siriuspy-2.79.0/siriuspy/namesys/implementation.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-30 14:45:12.877647 siriuspy-2.79.0/siriuspy/optics/
+-rw-r--r--   0 runner    (1001) docker     (122)       25 2023-07-30 14:45:00.000000 siriuspy-2.79.0/siriuspy/optics/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      363 2023-07-30 14:45:00.000000 siriuspy-2.79.0/siriuspy/optics/constants.py
+-rw-r--r--   0 runner    (1001) docker     (122)     8749 2023-07-30 14:45:00.000000 siriuspy-2.79.0/siriuspy/optics/lattice_survey.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-30 14:45:12.877647 siriuspy-2.79.0/siriuspy/opticscorr/
+-rw-r--r--   0 runner    (1001) docker     (122)       29 2023-07-30 14:45:00.000000 siriuspy-2.79.0/siriuspy/opticscorr/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    34878 2023-07-30 14:45:00.000000 siriuspy-2.79.0/siriuspy/opticscorr/base.py
+-rw-r--r--   0 runner    (1001) docker     (122)    16096 2023-07-30 14:45:00.000000 siriuspy-2.79.0/siriuspy/opticscorr/chrom.py
+-rw-r--r--   0 runner    (1001) docker     (122)    13454 2023-07-30 14:45:00.000000 siriuspy-2.79.0/siriuspy/opticscorr/csdev.py
+-rw-r--r--   0 runner    (1001) docker     (122)    18765 2023-07-30 14:45:00.000000 siriuspy-2.79.0/siriuspy/opticscorr/opticscorr.py
+-rw-r--r--   0 runner    (1001) docker     (122)     8006 2023-07-30 14:45:00.000000 siriuspy-2.79.0/siriuspy/opticscorr/tune.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1846 2023-07-30 14:45:00.000000 siriuspy-2.79.0/siriuspy/opticscorr/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-30 14:45:12.877647 siriuspy-2.79.0/siriuspy/oscilloscope/
+-rw-r--r--   0 runner    (1001) docker     (122)      104 2023-07-30 14:45:00.000000 siriuspy-2.79.0/siriuspy/oscilloscope/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7003 2023-07-30 14:45:00.000000 siriuspy-2.79.0/siriuspy/oscilloscope/keysight.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1467 2023-07-30 14:45:00.000000 siriuspy-2.79.0/siriuspy/oscilloscope/scopes.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-30 14:45:12.877647 siriuspy-2.79.0/siriuspy/posang/
+-rw-r--r--   0 runner    (1001) docker     (122)       25 2023-07-30 14:45:00.000000 siriuspy-2.79.0/siriuspy/posang/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4935 2023-07-30 14:45:00.000000 siriuspy-2.79.0/siriuspy/posang/csdev.py
+-rw-r--r--   0 runner    (1001) docker     (122)    19747 2023-07-30 14:45:00.000000 siriuspy-2.79.0/siriuspy/posang/main.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1678 2023-07-30 14:45:00.000000 siriuspy-2.79.0/siriuspy/posang/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-30 14:45:12.881647 siriuspy-2.79.0/siriuspy/pwrsupply/
+-rw-r--r--   0 runner    (1001) docker     (122)      132 2023-07-30 14:45:00.000000 siriuspy-2.79.0/siriuspy/pwrsupply/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     8950 2023-07-30 14:45:00.000000 siriuspy-2.79.0/siriuspy/pwrsupply/beaglebone.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-30 14:45:12.881647 siriuspy-2.79.0/siriuspy/pwrsupply/bsmp/
+-rw-r--r--   0 runner    (1001) docker     (122)       48 2023-07-30 14:45:00.000000 siriuspy-2.79.0/siriuspy/pwrsupply/bsmp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    25156 2023-07-30 14:45:00.000000 siriuspy-2.79.0/siriuspy/pwrsupply/bsmp/commands.py
+-rw-r--r--   0 runner    (1001) docker     (122)    19464 2023-07-30 14:45:00.000000 siriuspy-2.79.0/siriuspy/pwrsupply/bsmp/constants.py
+-rw-r--r--   0 runner    (1001) docker     (122)    53763 2023-07-30 14:45:00.000000 siriuspy-2.79.0/siriuspy/pwrsupply/bsmp/entities.py
+-rw-r--r--   0 runner    (1001) docker     (122)      850 2023-07-30 14:45:00.000000 siriuspy-2.79.0/siriuspy/pwrsupply/bsmp/factory.py
+-rw-r--r--   0 runner    (1001) docker     (122)   150566 2023-07-30 14:45:00.000000 siriuspy-2.79.0/siriuspy/pwrsupply/csdev.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3624 2023-07-30 14:45:00.000000 siriuspy-2.79.0/siriuspy/pwrsupply/data.py
+-rw-r--r--   0 runner    (1001) docker     (122)    10629 2023-07-30 14:45:00.000000 siriuspy-2.79.0/siriuspy/pwrsupply/factory.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-30 14:45:12.881647 siriuspy-2.79.0/siriuspy/pwrsupply/pructrl/
+-rw-r--r--   0 runner    (1001) docker     (122)      841 2023-07-30 14:45:00.000000 siriuspy-2.79.0/siriuspy/pwrsupply/pructrl/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3393 2023-07-30 14:45:00.000000 siriuspy-2.79.0/siriuspy/pwrsupply/pructrl/pru.py
+-rw-r--r--   0 runner    (1001) docker     (122)    25723 2023-07-30 14:45:00.000000 siriuspy-2.79.0/siriuspy/pwrsupply/pructrl/prucontroller.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6133 2023-07-30 14:45:00.000000 siriuspy-2.79.0/siriuspy/pwrsupply/pructrl/prucparms.py
+-rw-r--r--   0 runner    (1001) docker     (122)    10280 2023-07-30 14:45:00.000000 siriuspy-2.79.0/siriuspy/pwrsupply/pructrl/psdevstate.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7712 2023-07-30 14:45:00.000000 siriuspy-2.79.0/siriuspy/pwrsupply/pructrl/udc.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-30 14:45:12.881647 siriuspy-2.79.0/siriuspy/pwrsupply/psctrl/
+-rw-r--r--   0 runner    (1001) docker     (122)      866 2023-07-30 14:45:00.000000 siriuspy-2.79.0/siriuspy/pwrsupply/psctrl/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7884 2023-07-30 14:45:00.000000 siriuspy-2.79.0/siriuspy/pwrsupply/psctrl/pscontroller.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6262 2023-07-30 14:45:00.000000 siriuspy-2.79.0/siriuspy/pwrsupply/psctrl/pscreaders.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5502 2023-07-30 14:45:00.000000 siriuspy-2.79.0/siriuspy/pwrsupply/psctrl/pscstatus.py
+-rw-r--r--   0 runner    (1001) docker     (122)    17064 2023-07-30 14:45:00.000000 siriuspy-2.79.0/siriuspy/pwrsupply/psctrl/pscwriters.py
+-rw-r--r--   0 runner    (1001) docker     (122)    42124 2023-07-30 14:45:00.000000 siriuspy-2.79.0/siriuspy/pwrsupply/psctrl/psmodel.py
+-rw-r--r--   0 runner    (1001) docker     (122)    34142 2023-07-30 14:45:00.000000 siriuspy-2.79.0/siriuspy/pwrsupply/pssofb.py
+-rw-r--r--   0 runner    (1001) docker     (122)    12500 2023-07-30 14:45:00.000000 siriuspy-2.79.0/siriuspy/pwrsupply/siggen.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-30 14:45:12.881647 siriuspy-2.79.0/siriuspy/ramp/
+-rw-r--r--   0 runner    (1001) docker     (122)       23 2023-07-30 14:45:00.000000 siriuspy-2.79.0/siriuspy/ramp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    28999 2023-07-30 14:45:00.000000 siriuspy-2.79.0/siriuspy/ramp/conn.py
+-rw-r--r--   0 runner    (1001) docker     (122)      346 2023-07-30 14:45:00.000000 siriuspy-2.79.0/siriuspy/ramp/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3969 2023-07-30 14:45:00.000000 siriuspy-2.79.0/siriuspy/ramp/magnet.py
+-rw-r--r--   0 runner    (1001) docker     (122)    45093 2023-07-30 14:45:00.000000 siriuspy-2.79.0/siriuspy/ramp/ramp.py
+-rw-r--r--   0 runner    (1001) docker     (122)    29333 2023-07-30 14:45:00.000000 siriuspy-2.79.0/siriuspy/ramp/reconst_factory.py
+-rwxr-xr-x   0 runner    (1001) docker     (122)     6985 2023-07-30 14:45:00.000000 siriuspy-2.79.0/siriuspy/ramp/test_reconst_factory.py
+-rwxr-xr-x   0 runner    (1001) docker     (122)     4158 2023-07-30 14:45:00.000000 siriuspy-2.79.0/siriuspy/ramp/testwfm.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5584 2023-07-30 14:45:00.000000 siriuspy-2.79.0/siriuspy/ramp/util.py
+-rw-r--r--   0 runner    (1001) docker     (122)    30145 2023-07-30 14:45:00.000000 siriuspy-2.79.0/siriuspy/ramp/waveform.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-30 14:45:12.885647 siriuspy-2.79.0/siriuspy/search/
+-rw-r--r--   0 runner    (1001) docker     (122)      359 2023-07-30 14:45:00.000000 siriuspy-2.79.0/siriuspy/search/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3537 2023-07-30 14:45:00.000000 siriuspy-2.79.0/siriuspy/search/bpms_search.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6903 2023-07-30 14:45:00.000000 siriuspy-2.79.0/siriuspy/search/hl_time_search.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5566 2023-07-30 14:45:00.000000 siriuspy-2.79.0/siriuspy/search/id_search.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4152 2023-07-30 14:45:00.000000 siriuspy-2.79.0/siriuspy/search/ioc_search.py
+-rw-r--r--   0 runner    (1001) docker     (122)    17480 2023-07-30 14:45:00.000000 siriuspy-2.79.0/siriuspy/search/ll_time_search.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7219 2023-07-30 14:45:00.000000 siriuspy-2.79.0/siriuspy/search/ma_search.py
+-rw-r--r--   0 runner    (1001) docker     (122)    23882 2023-07-30 14:45:00.000000 siriuspy-2.79.0/siriuspy/search/ps_search.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-30 14:45:12.885647 siriuspy-2.79.0/siriuspy/simul/
+-rw-r--r--   0 runner    (1001) docker     (122)      311 2023-07-30 14:45:00.000000 siriuspy-2.79.0/siriuspy/simul/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2202 2023-07-30 14:45:00.000000 siriuspy-2.79.0/siriuspy/simul/simfactory.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6298 2023-07-30 14:45:00.000000 siriuspy-2.79.0/siriuspy/simul/simps.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2324 2023-07-30 14:45:00.000000 siriuspy-2.79.0/siriuspy/simul/simpv.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7391 2023-07-30 14:45:00.000000 siriuspy-2.79.0/siriuspy/simul/simulation.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4266 2023-07-30 14:45:00.000000 siriuspy-2.79.0/siriuspy/simul/simulator.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-30 14:45:12.889647 siriuspy-2.79.0/siriuspy/sofb/
+-rw-r--r--   0 runner    (1001) docker     (122)       78 2023-07-30 14:45:00.000000 siriuspy-2.79.0/siriuspy/sofb/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4869 2023-07-30 14:45:00.000000 siriuspy-2.79.0/siriuspy/sofb/base_class.py
+-rw-r--r--   0 runner    (1001) docker     (122)    28072 2023-07-30 14:45:00.000000 siriuspy-2.79.0/siriuspy/sofb/bpms.py
+-rw-r--r--   0 runner    (1001) docker     (122)    32010 2023-07-30 14:45:00.000000 siriuspy-2.79.0/siriuspy/sofb/correctors.py
+-rw-r--r--   0 runner    (1001) docker     (122)    47062 2023-07-30 14:45:00.000000 siriuspy-2.79.0/siriuspy/sofb/csdev.py
+-rw-r--r--   0 runner    (1001) docker     (122)    46398 2023-07-30 14:45:00.000000 siriuspy-2.79.0/siriuspy/sofb/main.py
+-rw-r--r--   0 runner    (1001) docker     (122)    11841 2023-07-30 14:45:00.000000 siriuspy-2.79.0/siriuspy/sofb/matrix.py
+-rw-r--r--   0 runner    (1001) docker     (122)    36357 2023-07-30 14:45:00.000000 siriuspy-2.79.0/siriuspy/sofb/orbit.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3030 2023-07-30 14:45:00.000000 siriuspy-2.79.0/siriuspy/sofb/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-30 14:45:12.889647 siriuspy-2.79.0/siriuspy/stabinfo/
+-rw-r--r--   0 runner    (1001) docker     (122)       38 2023-07-30 14:45:00.000000 siriuspy-2.79.0/siriuspy/stabinfo/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3558 2023-07-30 14:45:00.000000 siriuspy-2.79.0/siriuspy/stabinfo/csdev.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7708 2023-07-30 14:45:00.000000 siriuspy-2.79.0/siriuspy/stabinfo/main.py
+-rw-r--r--   0 runner    (1001) docker     (122)     8598 2023-07-30 14:45:00.000000 siriuspy-2.79.0/siriuspy/thread.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-30 14:45:12.889647 siriuspy-2.79.0/siriuspy/timesys/
+-rw-r--r--   0 runner    (1001) docker     (122)       26 2023-07-30 14:45:00.000000 siriuspy-2.79.0/siriuspy/timesys/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    20485 2023-07-30 14:45:00.000000 siriuspy-2.79.0/siriuspy/timesys/csdev.py
+-rw-r--r--   0 runner    (1001) docker     (122)    12705 2023-07-30 14:45:00.000000 siriuspy-2.79.0/siriuspy/timesys/hl_classes.py
+-rw-r--r--   0 runner    (1001) docker     (122)    33336 2023-07-30 14:45:00.000000 siriuspy-2.79.0/siriuspy/timesys/ll_classes.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6015 2023-07-30 14:45:00.000000 siriuspy-2.79.0/siriuspy/timesys/plot_network.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5957 2023-07-30 14:45:00.000000 siriuspy-2.79.0/siriuspy/timesys/static_table.py
+-rw-r--r--   0 runner    (1001) docker     (122)     8732 2023-07-30 14:45:00.000000 siriuspy-2.79.0/siriuspy/util.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-30 14:45:12.857647 siriuspy-2.79.0/siriuspy.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)     1423 2023-07-30 14:45:12.000000 siriuspy-2.79.0/siriuspy.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)    10223 2023-07-30 14:45:12.000000 siriuspy-2.79.0/siriuspy.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-07-30 14:45:12.000000 siriuspy-2.79.0/siriuspy.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-07-30 14:45:12.000000 siriuspy-2.79.0/siriuspy.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (122)      128 2023-07-30 14:45:12.000000 siriuspy-2.79.0/siriuspy.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       15 2023-07-30 14:45:12.000000 siriuspy-2.79.0/siriuspy.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-30 14:45:12.889647 siriuspy-2.79.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (122)      441 2023-07-30 14:45:00.000000 siriuspy-2.79.0/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-30 14:45:12.889647 siriuspy-2.79.0/tests/bsmp/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-30 14:45:00.000000 siriuspy-2.79.0/tests/bsmp/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (122)     5698 2023-07-30 14:45:00.000000 siriuspy-2.79.0/tests/bsmp/test_bsmp.py
+-rwxr-xr-x   0 runner    (1001) docker     (122)    14788 2023-07-30 14:45:00.000000 siriuspy-2.79.0/tests/bsmp/test_commands.py
+-rwxr-xr-x   0 runner    (1001) docker     (122)    13382 2023-07-30 14:45:00.000000 siriuspy-2.79.0/tests/bsmp/test_entities.py
+-rwxr-xr-x   0 runner    (1001) docker     (122)     7719 2023-07-30 14:45:00.000000 siriuspy-2.79.0/tests/bsmp/test_serial.py
+-rwxr-xr-x   0 runner    (1001) docker     (122)     1837 2023-07-30 14:45:00.000000 siriuspy-2.79.0/tests/bsmp/test_types.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-30 14:45:12.889647 siriuspy-2.79.0/tests/clientconfigdb/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-30 14:45:00.000000 siriuspy-2.79.0/tests/clientconfigdb/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (122)     2843 2023-07-30 14:45:00.000000 siriuspy-2.79.0/tests/clientconfigdb/test_configdb_client.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-30 14:45:12.889647 siriuspy-2.79.0/tests/clientweb/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-30 14:45:00.000000 siriuspy-2.79.0/tests/clientweb/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (122)    11633 2023-07-30 14:45:00.000000 siriuspy-2.79.0/tests/clientweb/test_implementation.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-30 14:45:12.889647 siriuspy-2.79.0/tests/currinfo/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-30 14:45:00.000000 siriuspy-2.79.0/tests/currinfo/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-30 14:45:12.889647 siriuspy-2.79.0/tests/currinfo/lifetime/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-30 14:45:00.000000 siriuspy-2.79.0/tests/currinfo/lifetime/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (122)     1908 2023-07-30 14:45:00.000000 siriuspy-2.79.0/tests/currinfo/lifetime/test_main.py
+-rwxr-xr-x   0 runner    (1001) docker     (122)     6495 2023-07-30 14:45:00.000000 siriuspy-2.79.0/tests/currinfo/test_csdev.py
+-rwxr-xr-x   0 runner    (1001) docker     (122)     2653 2023-07-30 14:45:00.000000 siriuspy-2.79.0/tests/currinfo/test_main.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-30 14:45:12.889647 siriuspy-2.79.0/tests/magnet/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-30 14:45:00.000000 siriuspy-2.79.0/tests/magnet/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (122)     2275 2023-07-30 14:45:00.000000 siriuspy-2.79.0/tests/magnet/test_factory.py
+-rwxr-xr-x   0 runner    (1001) docker     (122)     2687 2023-07-30 14:45:00.000000 siriuspy-2.79.0/tests/magnet/tests_normalizer.py
+-rwxr-xr-x   0 runner    (1001) docker     (122)     3618 2023-07-30 14:45:00.000000 siriuspy-2.79.0/tests/mock_servweb.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-30 14:45:12.889647 siriuspy-2.79.0/tests/namesys/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-30 14:45:00.000000 siriuspy-2.79.0/tests/namesys/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (122)     4896 2023-07-30 14:45:00.000000 siriuspy-2.79.0/tests/namesys/test_implementation.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-30 14:45:12.893647 siriuspy-2.79.0/tests/opticscorr/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-30 14:45:00.000000 siriuspy-2.79.0/tests/opticscorr/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5490 2023-07-30 14:45:00.000000 siriuspy-2.79.0/tests/opticscorr/test_chrom.py
+-rwxr-xr-x   0 runner    (1001) docker     (122)     4609 2023-07-30 14:45:00.000000 siriuspy-2.79.0/tests/opticscorr/test_csdev.py
+-rwxr-xr-x   0 runner    (1001) docker     (122)    23381 2023-07-30 14:45:00.000000 siriuspy-2.79.0/tests/opticscorr/test_opticscorr.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5692 2023-07-30 14:45:00.000000 siriuspy-2.79.0/tests/opticscorr/test_tune.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1145 2023-07-30 14:45:00.000000 siriuspy-2.79.0/tests/opticscorr/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-30 14:45:12.893647 siriuspy-2.79.0/tests/posang/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-30 14:45:00.000000 siriuspy-2.79.0/tests/posang/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (122)     2872 2023-07-30 14:45:00.000000 siriuspy-2.79.0/tests/posang/test_csdev.py
+-rwxr-xr-x   0 runner    (1001) docker     (122)     3164 2023-07-30 14:45:00.000000 siriuspy-2.79.0/tests/posang/test_main.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-30 14:45:12.893647 siriuspy-2.79.0/tests/pwrsupply/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-30 14:45:00.000000 siriuspy-2.79.0/tests/pwrsupply/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    18979 2023-07-30 14:45:00.000000 siriuspy-2.79.0/tests/pwrsupply/db.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-30 14:45:12.893647 siriuspy-2.79.0/tests/pwrsupply/pructrl/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-30 14:45:00.000000 siriuspy-2.79.0/tests/pwrsupply/pructrl/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (122)     2257 2023-07-30 14:45:00.000000 siriuspy-2.79.0/tests/pwrsupply/pructrl/test_pru.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-30 14:45:12.893647 siriuspy-2.79.0/tests/pwrsupply/psctrl/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-30 14:45:00.000000 siriuspy-2.79.0/tests/pwrsupply/psctrl/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4853 2023-07-30 14:45:00.000000 siriuspy-2.79.0/tests/pwrsupply/psctrl/test_pscwriters.py
+-rwxr-xr-x   0 runner    (1001) docker     (122)      166 2023-07-30 14:45:00.000000 siriuspy-2.79.0/tests/pwrsupply/test_beaglebone.py
+-rwxr-xr-x   0 runner    (1001) docker     (122)       89 2023-07-30 14:45:00.000000 siriuspy-2.79.0/tests/pwrsupply/test_bsmp.py
+-rwxr-xr-x   0 runner    (1001) docker     (122)     6439 2023-07-30 14:45:00.000000 siriuspy-2.79.0/tests/pwrsupply/test_csdev.py
+-rwxr-xr-x   0 runner    (1001) docker     (122)     7331 2023-07-30 14:45:00.000000 siriuspy-2.79.0/tests/pwrsupply/test_data.py
+-rwxr-xr-x   0 runner    (1001) docker     (122)     2323 2023-07-30 14:45:00.000000 siriuspy-2.79.0/tests/pwrsupply/test_siggen.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3146 2023-07-30 14:45:00.000000 siriuspy-2.79.0/tests/pwrsupply/variables.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-30 14:45:12.893647 siriuspy-2.79.0/tests/ramp/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-30 14:45:00.000000 siriuspy-2.79.0/tests/ramp/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (122)     5699 2023-07-30 14:45:00.000000 siriuspy-2.79.0/tests/ramp/test_magnet.py
+-rwxr-xr-x   0 runner    (1001) docker     (122)     7235 2023-07-30 14:45:00.000000 siriuspy-2.79.0/tests/ramp/test_waveform.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-30 14:45:12.893647 siriuspy-2.79.0/tests/search/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-30 14:45:00.000000 siriuspy-2.79.0/tests/search/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (122)     2433 2023-07-30 14:45:00.000000 siriuspy-2.79.0/tests/search/test_hl_time_search.py
+-rwxr-xr-x   0 runner    (1001) docker     (122)      559 2023-07-30 14:45:00.000000 siriuspy-2.79.0/tests/search/test_init.py
+-rwxr-xr-x   0 runner    (1001) docker     (122)     3886 2023-07-30 14:45:00.000000 siriuspy-2.79.0/tests/search/test_ll_time_search.py
+-rwxr-xr-x   0 runner    (1001) docker     (122)     6120 2023-07-30 14:45:00.000000 siriuspy-2.79.0/tests/search/test_ma_search.py
+-rwxr-xr-x   0 runner    (1001) docker     (122)    13502 2023-07-30 14:45:00.000000 siriuspy-2.79.0/tests/search/test_ps_search.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3478 2023-07-30 14:45:00.000000 siriuspy-2.79.0/tests/test_callbacks.py
+-rwxr-xr-x   0 runner    (1001) docker     (122)     1009 2023-07-30 14:45:00.000000 siriuspy-2.79.0/tests/test_csdev.py
+-rwxr-xr-x   0 runner    (1001) docker     (122)     1605 2023-07-30 14:45:00.000000 siriuspy-2.79.0/tests/test_envars.py
+-rwxr-xr-x   0 runner    (1001) docker     (122)    11533 2023-07-30 14:45:00.000000 siriuspy-2.79.0/tests/test_util.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-30 14:45:12.893647 siriuspy-2.79.0/tests/timesys/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-30 14:45:00.000000 siriuspy-2.79.0/tests/timesys/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (122)     5018 2023-07-30 14:45:00.000000 siriuspy-2.79.0/tests/timesys/test_csdev.py
+-rw-r--r--   0 runner    (1001) docker     (122)      978 2023-07-30 14:45:00.000000 siriuspy-2.79.0/tests/timesys/test_plot_network.py
```

### Comparing `siriuspy-2.78.0/LICENSE` & `siriuspy-2.79.0/LICENSE`

 * *Files identical despite different names*

### Comparing `siriuspy-2.78.0/PKG-INFO` & `siriuspy-2.79.0/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: siriuspy
-Version: 2.78.0
+Version: 2.79.0
 Summary: Development packages for Sirius
 Home-page: https://github.com/lnls-sirius/dev-packages
 Download-URL: https://github.com/lnls-sirius/dev-packages
 Author: lnls-sirius
 License: GNU GPLv3
 Classifier: Intended Audience :: Science/Research
 Classifier: Programming Language :: Python
```

### Comparing `siriuspy-2.78.0/README.md` & `siriuspy-2.79.0/README.md`

 * *Files identical despite different names*

### Comparing `siriuspy-2.78.0/setup.py` & `siriuspy-2.79.0/setup.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.78.0/siriuspy/__init__.py` & `siriuspy-2.79.0/siriuspy/__init__.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.78.0/siriuspy/bsmp/commands.py` & `siriuspy-2.79.0/siriuspy/bsmp/commands.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.78.0/siriuspy/bsmp/constants.py` & `siriuspy-2.79.0/siriuspy/bsmp/constants.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.78.0/siriuspy/bsmp/entities.py` & `siriuspy-2.79.0/siriuspy/bsmp/entities.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.78.0/siriuspy/bsmp/exceptions.py` & `siriuspy-2.79.0/siriuspy/bsmp/exceptions.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.78.0/siriuspy/bsmp/serial.py` & `siriuspy-2.79.0/siriuspy/bsmp/serial.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.78.0/siriuspy/bsmp/types.py` & `siriuspy-2.79.0/siriuspy/bsmp/types.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.78.0/siriuspy/callbacks.py` & `siriuspy-2.79.0/siriuspy/callbacks.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.78.0/siriuspy/clientarch/client.py` & `siriuspy-2.79.0/siriuspy/clientarch/client.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.78.0/siriuspy/clientarch/devices.py` & `siriuspy-2.79.0/siriuspy/clientarch/devices.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.78.0/siriuspy/clientarch/exceptions.py` & `siriuspy-2.79.0/siriuspy/clientarch/exceptions.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.78.0/siriuspy/clientarch/pvarch.py` & `siriuspy-2.79.0/siriuspy/clientarch/pvarch.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.78.0/siriuspy/clientarch/time.py` & `siriuspy-2.79.0/siriuspy/clientarch/time.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.78.0/siriuspy/clientconfigdb/_templates.py` & `siriuspy-2.79.0/siriuspy/clientconfigdb/_templates.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.78.0/siriuspy/clientconfigdb/configdb_client.py` & `siriuspy-2.79.0/siriuspy/clientconfigdb/configdb_client.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.78.0/siriuspy/clientconfigdb/configdb_document.py` & `siriuspy-2.79.0/siriuspy/clientconfigdb/configdb_document.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.78.0/siriuspy/clientconfigdb/pvsconfig.py` & `siriuspy-2.79.0/siriuspy/clientconfigdb/pvsconfig.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.78.0/siriuspy/clientconfigdb/types/as_corrloop_params.py` & `siriuspy-2.79.0/siriuspy/clientconfigdb/types/as_corrloop_params.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.78.0/siriuspy/clientconfigdb/types/as_diagnostics.py` & `siriuspy-2.79.0/siriuspy/clientconfigdb/types/as_diagnostics.py`

 * *Files 19% similar despite different names*

```diff
@@ -9,14 +9,18 @@
         'config_type_name': module_name,
         'value': _dcopy(_template_dict),
         'check': False
     }
     return _dict
 
 
+AFC_ACQCORE_NR_PHY_TRIGGER = 8
+AFC_ACQCORE_NR_LOG_TRIGGER = 24
+
+
 _li_diags = [
     # Screens
     ['LA-BI:PRF1:CAM:AcquireTime', 0.001, 0],
     ['LA-BI:PRF1:CAM:Gain', 0, 0],
     ['LA-BI:PRF1:CAL:CentroidThreshold', 0, 0],
     ['LA-BI:PRF1:ROI:MinX_', 0, 0],
     ['LA-BI:PRF1:ROI:MinY_', 0, 0],
@@ -103,15 +107,15 @@
     'IA-16RaBPM:TI-AMCFPGAEVR:',
     'IA-17RaBPM:TI-AMCFPGAEVR:',
     'IA-18RaBPM:TI-AMCFPGAEVR:',
     'IA-19RaBPM:TI-AMCFPGAEVR:',
     'IA-20RaBPM:TI-AMCFPGAEVR:',
     'IA-20RaBPMTL:TI-AMCFPGAEVR:',
     ]
-_amcfpgaevr_amcs = ['AMC3', 'AMC4', 'AMC6', 'AMC7']
+_amcfpgaevr_amcs = ['AMC3', 'AMC6']
 _amcfpgaevr_propts = [
     ['State-Sel', 1, 0.0],
     ['Src-Sel', 3, 0.0],
     ['Dir-Sel', 0, 0.0],
     ['Evt-SP', 0, 0.0],
     ['WidthRaw-SP', 1, 0.0],
     ['Polarity-Sel', 0, 0.0],
@@ -369,238 +373,14 @@
     [':RFFEPidBDTd-SP', 2.0, 0.0],
     [':RFFEHeaterAC-SP', 0.0, 0.0],
     [':RFFEHeaterBD-SP', 0.0, 0.0],
     [':ADC0RstModes-Sel', 1, 0.0],
     [':ADC1RstModes-Sel', 1, 0.0],
     [':ADC2RstModes-Sel', 1, 0.0],
     [':ADC3RstModes-Sel', 1, 0.0],
-    [':TRIGGER0Dir-Sel', 1, 0.0],
-    [':TRIGGER0DirPol-Sel', 1, 0.0],
-    [':TRIGGER0RcvLen-SP', 1, 0.0],
-    [':TRIGGER0TrnLen-SP', 1, 0.0],
-    [':TRIGGER1Dir-Sel', 1, 0.0],
-    [':TRIGGER1DirPol-Sel', 1, 0.0],
-    [':TRIGGER1RcvLen-SP', 1, 0.0],
-    [':TRIGGER1TrnLen-SP', 1, 0.0],
-    [':TRIGGER2Dir-Sel', 0, 0.0],
-    [':TRIGGER2DirPol-Sel', 1, 0.0],
-    [':TRIGGER2RcvLen-SP', 1, 0.0],
-    [':TRIGGER2TrnLen-SP', 1, 0.0],
-    [':TRIGGER3Dir-Sel', 0, 0.0],
-    [':TRIGGER3DirPol-Sel', 1, 0.0],
-    [':TRIGGER3RcvLen-SP', 1, 0.0],
-    [':TRIGGER3TrnLen-SP', 1, 0.0],
-    [':TRIGGER4Dir-Sel', 1, 0.0],
-    [':TRIGGER4DirPol-Sel', 1, 0.0],
-    [':TRIGGER4RcvLen-SP', 1, 0.0],
-    [':TRIGGER4TrnLen-SP', 1, 0.0],
-    [':TRIGGER5Dir-Sel', 1, 0.0],
-    [':TRIGGER5DirPol-Sel', 1, 0.0],
-    [':TRIGGER5RcvLen-SP', 1, 0.0],
-    [':TRIGGER5TrnLen-SP', 1, 0.0],
-    [':TRIGGER6Dir-Sel', 1, 0.0],
-    [':TRIGGER6DirPol-Sel', 1, 0.0],
-    [':TRIGGER6RcvLen-SP', 1, 0.0],
-    [':TRIGGER6TrnLen-SP', 1, 0.0],
-    [':TRIGGER7Dir-Sel', 1, 0.0],
-    [':TRIGGER7DirPol-Sel', 1, 0.0],
-    [':TRIGGER7RcvLen-SP', 1, 0.0],
-    [':TRIGGER7TrnLen-SP', 1, 0.0],
-    [':TRIGGER0RcvInSel-SP', 0, 0.0],
-    [':TRIGGER0RcvSrc-Sel', 0, 0.0],
-    [':TRIGGER0TrnOutSel-SP', 0, 0.0],
-    [':TRIGGER0TrnSrc-Sel', 0, 0.0],
-    [':TRIGGER1RcvInSel-SP', 0, 0.0],
-    [':TRIGGER1RcvSrc-Sel', 0, 0.0],
-    [':TRIGGER1TrnOutSel-SP', 0, 0.0],
-    [':TRIGGER1TrnSrc-Sel', 0, 0.0],
-    [':TRIGGER2RcvInSel-SP', 0, 0.0],
-    [':TRIGGER2RcvSrc-Sel', 0, 0.0],
-    [':TRIGGER2TrnOutSel-SP', 0, 0.0],
-    [':TRIGGER2TrnSrc-Sel', 0, 0.0],
-    [':TRIGGER3RcvInSel-SP', 0, 0.0],
-    [':TRIGGER3RcvSrc-Sel', 0, 0.0],
-    [':TRIGGER3TrnOutSel-SP', 0, 0.0],
-    [':TRIGGER3TrnSrc-Sel', 0, 0.0],
-    [':TRIGGER4RcvInSel-SP', 0, 0.0],
-    [':TRIGGER4RcvSrc-Sel', 0, 0.0],
-    [':TRIGGER4TrnOutSel-SP', 0, 0.0],
-    [':TRIGGER4TrnSrc-Sel', 0, 0.0],
-    [':TRIGGER5RcvInSel-SP', 0, 0.0],
-    [':TRIGGER5RcvSrc-Sel', 0, 0.0],
-    [':TRIGGER5TrnOutSel-SP', 0, 0.0],
-    [':TRIGGER5TrnSrc-Sel', 0, 0.0],
-    [':TRIGGER6RcvInSel-SP', 0, 0.0],
-    [':TRIGGER6RcvSrc-Sel', 0, 0.0],
-    [':TRIGGER6TrnOutSel-SP', 0, 0.0],
-    [':TRIGGER6TrnSrc-Sel', 0, 0.0],
-    [':TRIGGER7RcvInSel-SP', 0, 0.0],
-    [':TRIGGER7RcvSrc-Sel', 0, 0.0],
-    [':TRIGGER7TrnOutSel-SP', 0, 0.0],
-    [':TRIGGER7TrnSrc-Sel', 0, 0.0],
-    [':TRIGGER8RcvInSel-SP', 0, 0.0],
-    [':TRIGGER8RcvSrc-Sel', 0, 0.0],
-    [':TRIGGER8TrnOutSel-SP', 0, 0.0],
-    [':TRIGGER8TrnSrc-Sel', 0, 0.0],
-    [':TRIGGER9RcvInSel-SP', 0, 0.0],
-    [':TRIGGER9RcvSrc-Sel', 0, 0.0],
-    [':TRIGGER9TrnOutSel-SP', 0, 0.0],
-    [':TRIGGER9TrnSrc-Sel', 0, 0.0],
-    [':TRIGGER10RcvInSel-SP', 0, 0.0],
-    [':TRIGGER10RcvSrc-Sel', 0, 0.0],
-    [':TRIGGER10TrnOutSel-SP', 0, 0.0],
-    [':TRIGGER10TrnSrc-Sel', 0, 0.0],
-    [':TRIGGER11RcvInSel-SP', 0, 0.0],
-    [':TRIGGER11RcvSrc-Sel', 0, 0.0],
-    [':TRIGGER11TrnOutSel-SP', 0, 0.0],
-    [':TRIGGER11TrnSrc-Sel', 0, 0.0],
-    [':TRIGGER12RcvInSel-SP', 0, 0.0],
-    [':TRIGGER12RcvSrc-Sel', 0, 0.0],
-    [':TRIGGER12TrnOutSel-SP', 0, 0.0],
-    [':TRIGGER12TrnSrc-Sel', 0, 0.0],
-    [':TRIGGER13RcvInSel-SP', 0, 0.0],
-    [':TRIGGER13RcvSrc-Sel', 0, 0.0],
-    [':TRIGGER13TrnOutSel-SP', 0, 0.0],
-    [':TRIGGER13TrnSrc-Sel', 0, 0.0],
-    [':TRIGGER14RcvInSel-SP', 0, 0.0],
-    [':TRIGGER14RcvSrc-Sel', 0, 0.0],
-    [':TRIGGER14TrnOutSel-SP', 0, 0.0],
-    [':TRIGGER14TrnSrc-Sel', 0, 0.0],
-    [':TRIGGER15RcvInSel-SP', 0, 0.0],
-    [':TRIGGER15RcvSrc-Sel', 0, 0.0],
-    [':TRIGGER15TrnOutSel-SP', 0, 0.0],
-    [':TRIGGER15TrnSrc-Sel', 0, 0.0],
-    [':TRIGGER16RcvInSel-SP', 0, 0.0],
-    [':TRIGGER16RcvSrc-Sel', 0, 0.0],
-    [':TRIGGER16TrnOutSel-SP', 0, 0.0],
-    [':TRIGGER16TrnSrc-Sel', 0, 0.0],
-    [':TRIGGER17RcvInSel-SP', 0, 0.0],
-    [':TRIGGER17RcvSrc-Sel', 0, 0.0],
-    [':TRIGGER17TrnOutSel-SP', 0, 0.0],
-    [':TRIGGER17TrnSrc-Sel', 0, 0.0],
-    [':TRIGGER18RcvInSel-SP', 1, 0.0],
-    [':TRIGGER18RcvSrc-Sel', 1, 0.0],
-    [':TRIGGER18TrnOutSel-SP', 0, 0.0],
-    [':TRIGGER18TrnSrc-Sel', 0, 0.0],
-    [':TRIGGER19RcvInSel-SP', 0, 0.0],
-    [':TRIGGER19RcvSrc-Sel', 0, 0.0],
-    [':TRIGGER19TrnOutSel-SP', 0, 0.0],
-    [':TRIGGER19TrnSrc-Sel', 0, 0.0],
-    [':TRIGGER20RcvInSel-SP', 0, 0.0],
-    [':TRIGGER20RcvSrc-Sel', 0, 0.0],
-    [':TRIGGER20TrnOutSel-SP', 0, 0.0],
-    [':TRIGGER20TrnSrc-Sel', 0, 0.0],
-    [':TRIGGER21RcvInSel-SP', 0, 0.0],
-    [':TRIGGER21RcvSrc-Sel', 0, 0.0],
-    [':TRIGGER21TrnOutSel-SP', 0, 0.0],
-    [':TRIGGER21TrnSrc-Sel', 0, 0.0],
-    [':TRIGGER22RcvInSel-SP', 0, 0.0],
-    [':TRIGGER22RcvSrc-Sel', 0, 0.0],
-    [':TRIGGER22TrnOutSel-SP', 0, 0.0],
-    [':TRIGGER22TrnSrc-Sel', 0, 0.0],
-    [':TRIGGER23RcvInSel-SP', 0, 0.0],
-    [':TRIGGER23RcvSrc-Sel', 0, 0.0],
-    [':TRIGGER23TrnOutSel-SP', 0, 0.0],
-    [':TRIGGER23TrnSrc-Sel', 0, 0.0],
-    [':TRIGGER_PM0RcvInSel-SP', 0, 0.0],
-    [':TRIGGER_PM0RcvSrc-Sel', 0, 0.0],
-    [':TRIGGER_PM0TrnOutSel-SP', 0, 0.0],
-    [':TRIGGER_PM0TrnSrc-Sel', 0, 0.0],
-    [':TRIGGER_PM1RcvInSel-SP', 0, 0.0],
-    [':TRIGGER_PM1RcvSrc-Sel', 0, 0.0],
-    [':TRIGGER_PM1TrnOutSel-SP', 0, 0.0],
-    [':TRIGGER_PM1TrnSrc-Sel', 0, 0.0],
-    [':TRIGGER_PM2RcvInSel-SP', 0, 0.0],
-    [':TRIGGER_PM2RcvSrc-Sel', 0, 0.0],
-    [':TRIGGER_PM2TrnOutSel-SP', 0, 0.0],
-    [':TRIGGER_PM2TrnSrc-Sel', 0, 0.0],
-    [':TRIGGER_PM3RcvInSel-SP', 0, 0.0],
-    [':TRIGGER_PM3RcvSrc-Sel', 0, 0.0],
-    [':TRIGGER_PM3TrnOutSel-SP', 0, 0.0],
-    [':TRIGGER_PM3TrnSrc-Sel', 0, 0.0],
-    [':TRIGGER_PM4RcvInSel-SP', 0, 0.0],
-    [':TRIGGER_PM4RcvSrc-Sel', 0, 0.0],
-    [':TRIGGER_PM4TrnOutSel-SP', 0, 0.0],
-    [':TRIGGER_PM4TrnSrc-Sel', 0, 0.0],
-    [':TRIGGER_PM5RcvInSel-SP', 0, 0.0],
-    [':TRIGGER_PM5RcvSrc-Sel', 0, 0.0],
-    [':TRIGGER_PM5TrnOutSel-SP', 0, 0.0],
-    [':TRIGGER_PM5TrnSrc-Sel', 0, 0.0],
-    [':TRIGGER_PM6RcvInSel-SP', 0, 0.0],
-    [':TRIGGER_PM6RcvSrc-Sel', 0, 0.0],
-    [':TRIGGER_PM6TrnOutSel-SP', 0, 0.0],
-    [':TRIGGER_PM6TrnSrc-Sel', 0, 0.0],
-    [':TRIGGER_PM7RcvInSel-SP', 0, 0.0],
-    [':TRIGGER_PM7RcvSrc-Sel', 0, 0.0],
-    [':TRIGGER_PM7TrnOutSel-SP', 0, 0.0],
-    [':TRIGGER_PM7TrnSrc-Sel', 0, 0.0],
-    [':TRIGGER_PM8RcvInSel-SP', 0, 0.0],
-    [':TRIGGER_PM8RcvSrc-Sel', 0, 0.0],
-    [':TRIGGER_PM8TrnOutSel-SP', 0, 0.0],
-    [':TRIGGER_PM8TrnSrc-Sel', 0, 0.0],
-    [':TRIGGER_PM9RcvInSel-SP', 0, 0.0],
-    [':TRIGGER_PM9RcvSrc-Sel', 0, 0.0],
-    [':TRIGGER_PM9TrnOutSel-SP', 0, 0.0],
-    [':TRIGGER_PM9TrnSrc-Sel', 0, 0.0],
-    [':TRIGGER_PM10RcvInSel-SP', 0, 0.0],
-    [':TRIGGER_PM10RcvSrc-Sel', 0, 0.0],
-    [':TRIGGER_PM10TrnOutSel-SP', 0, 0.0],
-    [':TRIGGER_PM10TrnSrc-Sel', 0, 0.0],
-    [':TRIGGER_PM11RcvInSel-SP', 0, 0.0],
-    [':TRIGGER_PM11RcvSrc-Sel', 0, 0.0],
-    [':TRIGGER_PM11TrnOutSel-SP', 0, 0.0],
-    [':TRIGGER_PM11TrnSrc-Sel', 0, 0.0],
-    [':TRIGGER_PM12RcvInSel-SP', 0, 0.0],
-    [':TRIGGER_PM12RcvSrc-Sel', 0, 0.0],
-    [':TRIGGER_PM12TrnOutSel-SP', 0, 0.0],
-    [':TRIGGER_PM12TrnSrc-Sel', 0, 0.0],
-    [':TRIGGER_PM13RcvInSel-SP', 0, 0.0],
-    [':TRIGGER_PM13RcvSrc-Sel', 0, 0.0],
-    [':TRIGGER_PM13TrnOutSel-SP', 0, 0.0],
-    [':TRIGGER_PM13TrnSrc-Sel', 0, 0.0],
-    [':TRIGGER_PM14RcvInSel-SP', 0, 0.0],
-    [':TRIGGER_PM14RcvSrc-Sel', 0, 0.0],
-    [':TRIGGER_PM14TrnOutSel-SP', 0, 0.0],
-    [':TRIGGER_PM14TrnSrc-Sel', 0, 0.0],
-    [':TRIGGER_PM15RcvInSel-SP', 0, 0.0],
-    [':TRIGGER_PM15RcvSrc-Sel', 0, 0.0],
-    [':TRIGGER_PM15TrnOutSel-SP', 0, 0.0],
-    [':TRIGGER_PM15TrnSrc-Sel', 0, 0.0],
-    [':TRIGGER_PM16RcvInSel-SP', 0, 0.0],
-    [':TRIGGER_PM16RcvSrc-Sel', 0, 0.0],
-    [':TRIGGER_PM16TrnOutSel-SP', 0, 0.0],
-    [':TRIGGER_PM16TrnSrc-Sel', 0, 0.0],
-    [':TRIGGER_PM17RcvInSel-SP', 0, 0.0],
-    [':TRIGGER_PM17RcvSrc-Sel', 0, 0.0],
-    [':TRIGGER_PM17TrnOutSel-SP', 0, 0.0],
-    [':TRIGGER_PM17TrnSrc-Sel', 0, 0.0],
-    [':TRIGGER_PM18RcvInSel-SP', 0, 0.0],
-    [':TRIGGER_PM18RcvSrc-Sel', 0, 0.0],
-    [':TRIGGER_PM18TrnOutSel-SP', 0, 0.0],
-    [':TRIGGER_PM18TrnSrc-Sel', 0, 0.0],
-    [':TRIGGER_PM19RcvInSel-SP', 0, 0.0],
-    [':TRIGGER_PM19RcvSrc-Sel', 0, 0.0],
-    [':TRIGGER_PM19TrnOutSel-SP', 0, 0.0],
-    [':TRIGGER_PM19TrnSrc-Sel', 0, 0.0],
-    [':TRIGGER_PM20RcvInSel-SP', 0, 0.0],
-    [':TRIGGER_PM20RcvSrc-Sel', 0, 0.0],
-    [':TRIGGER_PM20TrnOutSel-SP', 0, 0.0],
-    [':TRIGGER_PM20TrnSrc-Sel', 0, 0.0],
-    [':TRIGGER_PM21RcvInSel-SP', 0, 0.0],
-    [':TRIGGER_PM21RcvSrc-Sel', 0, 0.0],
-    [':TRIGGER_PM21TrnOutSel-SP', 0, 0.0],
-    [':TRIGGER_PM21TrnSrc-Sel', 0, 0.0],
-    [':TRIGGER_PM22RcvInSel-SP', 0, 0.0],
-    [':TRIGGER_PM22RcvSrc-Sel', 0, 0.0],
-    [':TRIGGER_PM22TrnOutSel-SP', 0, 0.0],
-    [':TRIGGER_PM22TrnSrc-Sel', 0, 0.0],
-    [':TRIGGER_PM23RcvInSel-SP', 0, 0.0],
-    [':TRIGGER_PM23RcvSrc-Sel', 0, 0.0],
-    [':TRIGGER_PM23TrnOutSel-SP', 0, 0.0],
-    [':TRIGGER_PM23TrnSrc-Sel', 0, 0.0],
     [':ACQChannel-Sel', 0, 0.0],
     [':ACQSamplesPre-SP', 100, 0.0],
     [':ACQSamplesPost-SP', 50, 0.0],
     [':ACQTrigger-Sel', 1, 0.0],
     [':ACQShots-SP', 1, 0.0],
     [':ACQTriggerRep-Sel', 0, 0.0],
     [':ACQBPMMode-Sel', 1, 0.0],
@@ -640,14 +420,29 @@
     [':SwDirGainC-SP', 1.0, 0.0],
     [':SwDirGainD-SP', 1.0, 0.0],
     [':SwInvGainA-SP', 1.0, 0.0],
     [':SwInvGainB-SP', 1.0, 0.0],
     [':SwInvGainC-SP', 1.0, 0.0],
     [':SwInvGainD-SP', 1.0, 0.0],
 ]
+for phy_trig in range(AFC_ACQCORE_NR_PHY_TRIGGER):
+    _bpm_propts.extend([
+        [f':TRIGGER{phy_trig}Dir-Sel', 0, 0.0],
+        [f':TRIGGER{phy_trig}DirPol-Sel', 0, 0.0],
+        [f':TRIGGER{phy_trig}RcvLen-SP', 0, 0.0],
+        [f':TRIGGER{phy_trig}TrnLen-SP', 0, 0.0],
+    ])
+for acq_core in ['', '_PM']:
+    for log_trig in range(AFC_ACQCORE_NR_LOG_TRIGGER):
+        _bpm_propts.extend([
+            [f':TRIGGER{acq_core}{log_trig}RcvInSel-SP', 0, 0.0],
+            [f':TRIGGER{acq_core}{log_trig}RcvSrc-Sel', 0, 0.0],
+            [f':TRIGGER{acq_core}{log_trig}TrnOutSel-SP', 0, 0.0],
+            [f':TRIGGER{acq_core}{log_trig}TrnSrc-Sel', 0, 0.0],
+        ])
 _bpm_pvs = list()
 for dev in _bpms:
     for ppt, val, dly in _bpm_propts:
         _bpm_pvs.append([dev+ppt, val, dly])
 
 _scrns = [
     'TB-01:DI-{0:s}-1',
@@ -1431,48 +1226,30 @@
     'IA-15RaBPM:BS-FOFBCtrl',
     'IA-16RaBPM:BS-FOFBCtrl',
     'IA-17RaBPM:BS-FOFBCtrl',
     'IA-18RaBPM:BS-FOFBCtrl',
     'IA-19RaBPM:BS-FOFBCtrl',
     'IA-20RaBPM:BS-FOFBCtrl',
 ]
-_fofb_propts = [
-    [':TRIGGER0Dir-Sel', 1, 0.0],
-    [':TRIGGER0DirPol-Sel', 1, 0.0],
-    [':TRIGGER0RcvLen-SP', 1, 0.0],
-    [':TRIGGER0TrnLen-SP', 1, 0.0],
-    [':TRIGGER1Dir-Sel', 1, 0.0],
-    [':TRIGGER1DirPol-Sel', 1, 0.0],
-    [':TRIGGER1RcvLen-SP', 1, 0.0],
-    [':TRIGGER1TrnLen-SP', 1, 0.0],
-    [':TRIGGER2Dir-Sel', 0, 0.0],
-    [':TRIGGER2DirPol-Sel', 1, 0.0],
-    [':TRIGGER2RcvLen-SP', 1, 0.0],
-    [':TRIGGER2TrnLen-SP', 1, 0.0],
-    [':TRIGGER3Dir-Sel', 0, 0.0],
-    [':TRIGGER3DirPol-Sel', 1, 0.0],
-    [':TRIGGER3RcvLen-SP', 1, 0.0],
-    [':TRIGGER3TrnLen-SP', 1, 0.0],
-    [':TRIGGER4Dir-Sel', 1, 0.0],
-    [':TRIGGER4DirPol-Sel', 1, 0.0],
-    [':TRIGGER4RcvLen-SP', 1, 0.0],
-    [':TRIGGER4TrnLen-SP', 1, 0.0],
-    [':TRIGGER5Dir-Sel', 1, 0.0],
-    [':TRIGGER5DirPol-Sel', 1, 0.0],
-    [':TRIGGER5RcvLen-SP', 1, 0.0],
-    [':TRIGGER5TrnLen-SP', 1, 0.0],
-    [':TRIGGER6Dir-Sel', 1, 0.0],
-    [':TRIGGER6DirPol-Sel', 1, 0.0],
-    [':TRIGGER6RcvLen-SP', 1, 0.0],
-    [':TRIGGER6TrnLen-SP', 1, 0.0],
-    [':TRIGGER7Dir-Sel', 1, 0.0],
-    [':TRIGGER7DirPol-Sel', 1, 0.0],
-    [':TRIGGER7RcvLen-SP', 1, 0.0],
-    [':TRIGGER7TrnLen-SP', 1, 0.0],
-    ]
+_fofb_propts = list()
+for phy_trig in range(AFC_ACQCORE_NR_PHY_TRIGGER):
+    _fofb_propts.extend([
+        [f':TRIGGER{phy_trig}Dir-Sel', 0, 0.0],
+        [f':TRIGGER{phy_trig}DirPol-Sel', 0, 0.0],
+        [f':TRIGGER{phy_trig}RcvLen-SP', 0, 0.0],
+        [f':TRIGGER{phy_trig}TrnLen-SP', 0, 0.0],
+    ])
+for acq_core in ['_LAMP', '_SYSID']:
+    for log_trig in range(AFC_ACQCORE_NR_LOG_TRIGGER):
+        _fofb_propts.extend([
+            [f':TRIGGER{acq_core}{log_trig}RcvInSel-SP', 0, 0.0],
+            [f':TRIGGER{acq_core}{log_trig}RcvSrc-Sel', 0, 0.0],
+            [f':TRIGGER{acq_core}{log_trig}TrnOutSel-SP', 0, 0.0],
+            [f':TRIGGER{acq_core}{log_trig}TrnSrc-Sel', 0, 0.0],
+        ])
 _fofb_pvs = list()
 for dev in _fofbctrls:
     for ppt, val, dly in _fofb_propts:
         _fofb_pvs.append([dev+ppt, val, dly])
 
 
 # When using this type of configuration to set the machine,
```

### Comparing `siriuspy-2.78.0/siriuspy/clientconfigdb/types/as_pwrstate.py` & `siriuspy-2.79.0/siriuspy/clientconfigdb/types/as_pwrstate.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.78.0/siriuspy/clientconfigdb/types/as_rf.py` & `siriuspy-2.79.0/siriuspy/clientconfigdb/types/as_rf.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.78.0/siriuspy/clientconfigdb/types/bo_chromcorr_params.py` & `siriuspy-2.79.0/siriuspy/clientconfigdb/types/bo_chromcorr_params.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.78.0/siriuspy/clientconfigdb/types/bo_normalized.py` & `siriuspy-2.79.0/siriuspy/clientconfigdb/types/bo_normalized.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.78.0/siriuspy/clientconfigdb/types/bo_orbcorr_respm.py` & `siriuspy-2.79.0/siriuspy/clientconfigdb/types/bo_orbcorr_respm.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.78.0/siriuspy/clientconfigdb/types/bo_orbit.py` & `siriuspy-2.79.0/siriuspy/clientconfigdb/types/bo_orbit.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.78.0/siriuspy/clientconfigdb/types/bo_ramp.py` & `siriuspy-2.79.0/siriuspy/clientconfigdb/types/bo_ramp.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.78.0/siriuspy/clientconfigdb/types/bo_tunecorr_params.py` & `siriuspy-2.79.0/siriuspy/clientconfigdb/types/bo_tunecorr_params.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.78.0/siriuspy/clientconfigdb/types/global_config.py` & `siriuspy-2.79.0/siriuspy/clientconfigdb/types/global_config.py`

 * *Files 0% similar despite different names*

```diff
@@ -353,14 +353,15 @@
     ['BO-Fam:TI-BPM:WidthRaw-SP', 0, 0.0],
     ['BO-Fam:TI-BPM:NrPulses-SP', 0, 0.0],
     ['BO-Fam:TI-BPM:Polarity-Sel', 0, 0.0],
     ['BO-Fam:TI-BPM:Src-Sel', 0, 0.0],
     ['BO-Fam:TI-BPM:State-Sel', 0, 0.0],
     ['BO-Fam:TI-BPM:DeltaDelayRaw-SP', 30*[0, ], 0],
     ['BO-Fam:TI-BPM:LowLvlLock-Sel', 0, 0.0],
+    ['BO-Fam:TI-BPM:Direction-Sel', 0, 0.0],
 
     ['BO-Glob:TI-LLRF-Gen:DelayRaw-SP', 0, 0],
     ['BO-Glob:TI-LLRF-Gen:WidthRaw-SP', 0, 0.0],
     ['BO-Glob:TI-LLRF-Gen:NrPulses-SP', 0, 0.0],
     ['BO-Glob:TI-LLRF-Gen:Polarity-Sel', 0, 0.0],
     ['BO-Glob:TI-LLRF-Gen:Src-Sel', 0, 0.0],
     ['BO-Glob:TI-LLRF-Gen:State-Sel', 0, 0.0],
@@ -389,14 +390,15 @@
     ['BO-Glob:TI-Mags-Corrs:WidthRaw-SP', 0, 0.0],
     ['BO-Glob:TI-Mags-Corrs:NrPulses-SP', 0, 0.0],
     ['BO-Glob:TI-Mags-Corrs:Polarity-Sel', 0, 0.0],
     ['BO-Glob:TI-Mags-Corrs:Src-Sel', 0, 0.0],
     # ['BO-Glob:TI-Mags-Corrs:State-Sel', 0, 0.0],
     ['BO-Glob:TI-Mags-Corrs:DeltaDelayRaw-SP', 30*[0, ], 0],
     ['BO-Glob:TI-Mags-Corrs:LowLvlLock-Sel', 0, 0.0],
+    ['BO-Glob:TI-Mags-Corrs:Direction-Sel', 0, 0.0],
 
     ['BO-Glob:TI-Mags-Fams:DelayRaw-SP', 0, 0],
     ['BO-Glob:TI-Mags-Fams:WidthRaw-SP', 0, 0.0],
     ['BO-Glob:TI-Mags-Fams:NrPulses-SP', 0, 0.0],
     ['BO-Glob:TI-Mags-Fams:Polarity-Sel', 0, 0.0],
     ['BO-Glob:TI-Mags-Fams:Src-Sel', 0, 0.0],
     # ['BO-Glob:TI-Mags-Fams:State-Sel', 0, 0.0],
@@ -615,41 +617,65 @@
     ['SI-Fam:TI-BPM:WidthRaw-SP', 0, 0.0],
     ['SI-Fam:TI-BPM:NrPulses-SP', 0, 0.0],
     ['SI-Fam:TI-BPM:Polarity-Sel', 0, 0.0],
     ['SI-Fam:TI-BPM:Src-Sel', 0, 0.0],
     ['SI-Fam:TI-BPM:State-Sel', 0, 0.0],
     ['SI-Fam:TI-BPM:DeltaDelayRaw-SP', 30*[0, ], 0],
     ['SI-Fam:TI-BPM:LowLvlLock-Sel', 0, 0.0],
+    ['SI-Fam:TI-BPM:Direction-Sel', 0, 0.0],
 
     ['SI-Fam:TI-BPM-PsMtn:DelayRaw-SP', 0, 0],
     ['SI-Fam:TI-BPM-PsMtn:WidthRaw-SP', 0, 0.0],
     ['SI-Fam:TI-BPM-PsMtn:NrPulses-SP', 0, 0.0],
     ['SI-Fam:TI-BPM-PsMtn:Polarity-Sel', 0, 0.0],
     ['SI-Fam:TI-BPM-PsMtn:Src-Sel', 0, 0.0],
     ['SI-Fam:TI-BPM-PsMtn:State-Sel', 0, 0.0],
     ['SI-Fam:TI-BPM-PsMtn:DeltaDelayRaw-SP', 30*[0, ], 0],
     ['SI-Fam:TI-BPM-PsMtn:LowLvlLock-Sel', 0, 0.0],
+    ['SI-Fam:TI-BPM-PsMtn:Direction-Sel', 0, 0.0],
+
+    ['AS-Fam:TI-BPM-MonitClk:DelayRaw-SP', 0, 0],
+    ['AS-Fam:TI-BPM-MonitClk:WidthRaw-SP', 0, 0.0],
+    ['AS-Fam:TI-BPM-MonitClk:NrPulses-SP', 0, 0.0],
+    ['AS-Fam:TI-BPM-MonitClk:Polarity-Sel', 0, 0.0],
+    ['AS-Fam:TI-BPM-MonitClk:Src-Sel', 0, 0.0],
+    ['AS-Fam:TI-BPM-MonitClk:State-Sel', 0, 0.0],
+    ['AS-Fam:TI-BPM-MonitClk:DeltaDelayRaw-SP', 30*[0, ], 0],
+    ['AS-Fam:TI-BPM-MonitClk:LowLvlLock-Sel', 0, 0.0],
+    ['AS-Fam:TI-BPM-MonitClk:Direction-Sel', 0, 0.0],
+
+    ['SI-Fam:TI-BPM-OrbIntlk:DelayRaw-SP', 0, 0],
+    ['SI-Fam:TI-BPM-OrbIntlk:WidthRaw-SP', 0, 0.0],
+    ['SI-Fam:TI-BPM-OrbIntlk:NrPulses-SP', 0, 0.0],
+    ['SI-Fam:TI-BPM-OrbIntlk:Polarity-Sel', 0, 0.0],
+    ['SI-Fam:TI-BPM-OrbIntlk:Src-Sel', 0, 0.0],
+    ['SI-Fam:TI-BPM-OrbIntlk:State-Sel', 0, 0.0],
+    ['SI-Fam:TI-BPM-OrbIntlk:DeltaDelayRaw-SP', 30*[0, ], 0],
+    ['SI-Fam:TI-BPM-OrbIntlk:LowLvlLock-Sel', 0, 0.0],
+    ['SI-Fam:TI-BPM-OrbIntlk:Direction-Sel', 1, 0.0],
 
     ['SI-Fam:TI-FOFB:DelayRaw-SP', 0, 0],
     ['SI-Fam:TI-FOFB:WidthRaw-SP', 0, 0.0],
     ['SI-Fam:TI-FOFB:NrPulses-SP', 0, 0.0],
     ['SI-Fam:TI-FOFB:Polarity-Sel', 0, 0.0],
     ['SI-Fam:TI-FOFB:Src-Sel', 0, 0.0],
     ['SI-Fam:TI-FOFB:State-Sel', 0, 0.0],
     ['SI-Fam:TI-FOFB:DeltaDelayRaw-SP', 30*[0, ], 0],
     ['SI-Fam:TI-FOFB:LowLvlLock-Sel', 0, 0.0],
+    ['SI-Fam:TI-FOFB:Direction-Sel', 0, 0.0],
 
     ['SI-01:TI-Mags-FFCorrs:DelayRaw-SP', 0, 0],
     ['SI-01:TI-Mags-FFCorrs:WidthRaw-SP', 0, 0.0],
     ['SI-01:TI-Mags-FFCorrs:NrPulses-SP', 0, 0.0],
     ['SI-01:TI-Mags-FFCorrs:Polarity-Sel', 0, 0.0],
     ['SI-01:TI-Mags-FFCorrs:Src-Sel', 0, 0.0],
     ['SI-01:TI-Mags-FFCorrs:State-Sel', 0, 0.0],
     ['SI-01:TI-Mags-FFCorrs:DeltaDelayRaw-SP', 30*[0, ], 0],
     ['SI-01:TI-Mags-FFCorrs:LowLvlLock-Sel', 0, 0.0],
+    ['SI-01:TI-Mags-FFCorrs:Direction-Sel', 0, 0.0],
 
     ['SI-Glob:TI-BbBProcH-Fid:DelayRaw-SP', 0, 0],
     ['SI-Glob:TI-BbBProcH-Fid:WidthRaw-SP', 0, 0.0],
     ['SI-Glob:TI-BbBProcH-Fid:NrPulses-SP', 0, 0.0],
     ['SI-Glob:TI-BbBProcH-Fid:Polarity-Sel', 0, 0.0],
     ['SI-Glob:TI-BbBProcH-Fid:RFDelayType-Sel', 0, 0.0],
     ['SI-Glob:TI-BbBProcH-Fid:Src-Sel', 0, 0.0],
@@ -771,14 +797,15 @@
     ['SI-Glob:TI-Mags-Corrs:WidthRaw-SP', 0, 0.0],
     ['SI-Glob:TI-Mags-Corrs:NrPulses-SP', 0, 0.0],
     ['SI-Glob:TI-Mags-Corrs:Polarity-Sel', 0, 0.0],
     ['SI-Glob:TI-Mags-Corrs:Src-Sel', 0, 0.0],
     ['SI-Glob:TI-Mags-Corrs:State-Sel', 0, 0.0],
     ['SI-Glob:TI-Mags-Corrs:DeltaDelayRaw-SP', 30*[0, ], 0],
     ['SI-Glob:TI-Mags-Corrs:LowLvlLock-Sel', 0, 0.0],
+    ['SI-Glob:TI-Mags-Corrs:Direction-Sel', 0, 0.0],
 
     ['SI-Glob:TI-Mags-Quads:DelayRaw-SP', 0, 0],
     ['SI-Glob:TI-Mags-Quads:WidthRaw-SP', 0, 0.0],
     ['SI-Glob:TI-Mags-Quads:NrPulses-SP', 0, 0.0],
     ['SI-Glob:TI-Mags-Quads:Polarity-Sel', 0, 0.0],
     ['SI-Glob:TI-Mags-Quads:Src-Sel', 0, 0.0],
     ['SI-Glob:TI-Mags-Quads:State-Sel', 0, 0.0],
@@ -789,14 +816,15 @@
     ['SI-Glob:TI-Mags-QTrims:WidthRaw-SP', 0, 0.0],
     ['SI-Glob:TI-Mags-QTrims:NrPulses-SP', 0, 0.0],
     ['SI-Glob:TI-Mags-QTrims:Polarity-Sel', 0, 0.0],
     ['SI-Glob:TI-Mags-QTrims:Src-Sel', 0, 0.0],
     ['SI-Glob:TI-Mags-QTrims:State-Sel', 0, 0.0],
     ['SI-Glob:TI-Mags-QTrims:DeltaDelayRaw-SP', 30*[0, ], 0],
     ['SI-Glob:TI-Mags-QTrims:LowLvlLock-Sel', 0, 0.0],
+    ['SI-Glob:TI-Mags-QTrims:Direction-Sel', 0, 0.0],
 
     ['SI-Glob:TI-Mags-Sexts:DelayRaw-SP', 0, 0],
     ['SI-Glob:TI-Mags-Sexts:WidthRaw-SP', 0, 0.0],
     ['SI-Glob:TI-Mags-Sexts:NrPulses-SP', 0, 0.0],
     ['SI-Glob:TI-Mags-Sexts:Polarity-Sel', 0, 0.0],
     ['SI-Glob:TI-Mags-Sexts:Src-Sel', 0, 0.0],
     ['SI-Glob:TI-Mags-Sexts:State-Sel', 0, 0.0],
@@ -807,14 +835,15 @@
     ['SI-Glob:TI-Mags-Skews:WidthRaw-SP', 0, 0.0],
     ['SI-Glob:TI-Mags-Skews:NrPulses-SP', 0, 0.0],
     ['SI-Glob:TI-Mags-Skews:Polarity-Sel', 0, 0.0],
     ['SI-Glob:TI-Mags-Skews:Src-Sel', 0, 0.0],
     ['SI-Glob:TI-Mags-Skews:State-Sel', 0, 0.0],
     ['SI-Glob:TI-Mags-Skews:DeltaDelayRaw-SP', 30*[0, ], 0],
     ['SI-Glob:TI-Mags-Skews:LowLvlLock-Sel', 0, 0.0],
+    ['SI-Glob:TI-Mags-Skews:Direction-Sel', 0, 0.0],
 
     # NOTE: This trigger is not present yet in timing IOC:
     # ['SI-Glob:TI-StrkCam-Trig1:DelayRaw-SP', 0, 0],
     # ['SI-Glob:TI-StrkCam-Trig1:WidthRaw-SP', 0, 0.0],
     # ['SI-Glob:TI-StrkCam-Trig1:NrPulses-SP', 0, 0.0],
     # ['SI-Glob:TI-StrkCam-Trig1:Polarity-Sel', 0, 0.0],
     # ['SI-Glob:TI-StrkCam-Trig1:RFDelayType-Sel', 0, 0.0],
@@ -846,14 +875,15 @@
     ['TB-Fam:TI-BPM:WidthRaw-SP', 0, 0.0],
     ['TB-Fam:TI-BPM:NrPulses-SP', 0, 0.0],
     ['TB-Fam:TI-BPM:Polarity-Sel', 0, 0.0],
     ['TB-Fam:TI-BPM:Src-Sel', 0, 0.0],
     ['TB-Fam:TI-BPM:State-Sel', 0, 0.0],
     ['TB-Fam:TI-BPM:DeltaDelayRaw-SP', 30*[0, ], 0],
     ['TB-Fam:TI-BPM:LowLvlLock-Sel', 0, 0.0],
+    ['TB-Fam:TI-BPM:Direction-Sel', 0, 0.0],
 
     ['TB-Fam:TI-ICT-Digit:DelayRaw-SP', 0, 0],
     ['TB-Fam:TI-ICT-Digit:WidthRaw-SP', 0, 0.0],
     ['TB-Fam:TI-ICT-Digit:NrPulses-SP', 0, 0.0],
     ['TB-Fam:TI-ICT-Digit:Polarity-Sel', 0, 0.0],
     ['TB-Fam:TI-ICT-Digit:Src-Sel', 0, 0.0],
     ['TB-Fam:TI-ICT-Digit:State-Sel', 0, 0.0],
@@ -929,14 +959,15 @@
     ['TS-Fam:TI-BPM:WidthRaw-SP', 0, 0.0],
     ['TS-Fam:TI-BPM:NrPulses-SP', 0, 0.0],
     ['TS-Fam:TI-BPM:Polarity-Sel', 0, 0.0],
     ['TS-Fam:TI-BPM:Src-Sel', 0, 0.0],
     ['TS-Fam:TI-BPM:State-Sel', 0, 0.0],
     ['TS-Fam:TI-BPM:DeltaDelayRaw-SP', 30*[0, ], 0],
     ['TS-Fam:TI-BPM:LowLvlLock-Sel', 0, 0.0],
+    ['TS-Fam:TI-BPM:Direction-Sel', 0, 0.0],
 
     ['TS-Fam:TI-ICT-Digit:DelayRaw-SP', 0, 0],
     ['TS-Fam:TI-ICT-Digit:WidthRaw-SP', 0, 0.0],
     ['TS-Fam:TI-ICT-Digit:NrPulses-SP', 0, 0.0],
     ['TS-Fam:TI-ICT-Digit:Polarity-Sel', 0, 0.0],
     ['TS-Fam:TI-ICT-Digit:Src-Sel', 0, 0.0],
     ['TS-Fam:TI-ICT-Digit:State-Sel', 0, 0.0],
```

### Comparing `siriuspy-2.78.0/siriuspy/clientconfigdb/types/si_bbadata.py` & `siriuspy-2.79.0/siriuspy/clientconfigdb/types/si_bbadata.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.78.0/siriuspy/clientconfigdb/types/si_bbbproc.py` & `siriuspy-2.79.0/siriuspy/clientconfigdb/types/si_bbbproc.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.78.0/siriuspy/clientconfigdb/types/si_chromcorr_params.py` & `siriuspy-2.79.0/siriuspy/clientconfigdb/types/si_chromcorr_params.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.78.0/siriuspy/clientconfigdb/types/si_fastorbcorr_respm.py` & `siriuspy-2.79.0/siriuspy/clientconfigdb/types/si_fastorbcorr_respm.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.78.0/siriuspy/clientconfigdb/types/si_fofb.py` & `siriuspy-2.79.0/siriuspy/clientconfigdb/types/si_fofb.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.78.0/siriuspy/clientconfigdb/types/si_id.py` & `siriuspy-2.79.0/siriuspy/clientconfigdb/types/si_id.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.78.0/siriuspy/clientconfigdb/types/si_idff.py` & `siriuspy-2.79.0/siriuspy/clientconfigdb/types/si_idff.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.78.0/siriuspy/clientconfigdb/types/si_orbcorr_respm.py` & `siriuspy-2.79.0/siriuspy/clientconfigdb/types/si_orbcorr_respm.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.78.0/siriuspy/clientconfigdb/types/si_orbit.py` & `siriuspy-2.79.0/siriuspy/clientconfigdb/types/si_orbit.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.78.0/siriuspy/clientconfigdb/types/si_tunecorr_params.py` & `siriuspy-2.79.0/siriuspy/clientconfigdb/types/si_tunecorr_params.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.78.0/siriuspy/clientconfigdb/types/tb_normalized.py` & `siriuspy-2.79.0/siriuspy/clientconfigdb/types/tb_normalized.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.78.0/siriuspy/clientconfigdb/types/tb_orbcorr_respm.py` & `siriuspy-2.79.0/siriuspy/clientconfigdb/types/tb_orbcorr_respm.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.78.0/siriuspy/clientconfigdb/types/tb_orbit.py` & `siriuspy-2.79.0/siriuspy/clientconfigdb/types/tb_orbit.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.78.0/siriuspy/clientconfigdb/types/tb_posang_respm.py` & `siriuspy-2.79.0/siriuspy/clientconfigdb/types/tb_posang_respm.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.78.0/siriuspy/clientconfigdb/types/ts_orbcorr_respm.py` & `siriuspy-2.79.0/siriuspy/clientconfigdb/types/ts_orbcorr_respm.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.78.0/siriuspy/clientconfigdb/types/ts_orbit.py` & `siriuspy-2.79.0/siriuspy/clientconfigdb/types/ts_orbit.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.78.0/siriuspy/clientconfigdb/types/ts_posang_respm.py` & `siriuspy-2.79.0/siriuspy/clientconfigdb/types/ts_posang_respm.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.78.0/siriuspy/clientweb/implementation.py` & `siriuspy-2.79.0/siriuspy/clientweb/implementation.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.78.0/siriuspy/csdev.py` & `siriuspy-2.79.0/siriuspy/csdev.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.78.0/siriuspy/currinfo/csdev.py` & `siriuspy-2.79.0/siriuspy/currinfo/csdev.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.78.0/siriuspy/currinfo/lifetime/main.py` & `siriuspy-2.79.0/siriuspy/currinfo/lifetime/main.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.78.0/siriuspy/currinfo/main.py` & `siriuspy-2.79.0/siriuspy/currinfo/main.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.78.0/siriuspy/cycle/__init__.py` & `siriuspy-2.79.0/siriuspy/cycle/__init__.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.78.0/siriuspy/cycle/bo_cycle_data.py` & `siriuspy-2.79.0/siriuspy/cycle/bo_cycle_data.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.78.0/siriuspy/cycle/conn.py` & `siriuspy-2.79.0/siriuspy/cycle/conn.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.78.0/siriuspy/cycle/fc_cycle_data.py` & `siriuspy-2.79.0/siriuspy/cycle/fc_cycle_data.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.78.0/siriuspy/cycle/li_cycle_data.py` & `siriuspy-2.79.0/siriuspy/cycle/li_cycle_data.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.78.0/siriuspy/cycle/main.py` & `siriuspy-2.79.0/siriuspy/cycle/main.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.78.0/siriuspy/cycle/util.py` & `siriuspy-2.79.0/siriuspy/cycle/util.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.78.0/siriuspy/devices/__init__.py` & `siriuspy-2.79.0/siriuspy/devices/__init__.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,19 +1,22 @@
 """Devices subpackage."""
 
+from .afc_acq_core import AFCPhysicalTrigger, AFCACQLogicalTrigger
 from .bbb import BunchbyBunch
-from .bpm import BPM, FamBPMs, BPMLogicalTrigger
+from .bpm import BPM, FamBPMs
 from .currinfo import CurrInfoTranspEff, CurrInfoLinear, \
     CurrInfoBO, CurrInfoSI, CurrInfoAS
 from .dcct import DCCT
 from .device import Device, DeviceApp, Devices, DeviceNC
 from .egun import EGBias, EGFilament, EGHVPS, EGTriggerPS, EGPulsePS, EGun
 from .energy import Energy
 from .fofb import FOFBCtrlDCC, BPMDCC, FOFBCtrlRef, FamFOFBControllers, \
     FamFastCorrs, HLFOFB
+from .fofb_acq import FOFBCtrlSysId, FOFBPSSysId, FamFOFBSysId, \
+    FOFBCtrlLamp, FOFBPSLamp, FamFOFBLamp
 from .ict import ICT, TranspEff
 from .ids import APU, WIG, PAPU, EPU
 from .idff import IDFF, WIGIDFF, PAPUIDFF, EPUIDFF, APUIDFF
 from .injctrl import InjCtrl
 from .injsys import PUMagsStandbyHandler, BOPSRampStandbyHandler, \
     BORFRampStandbyHandler, InjSysStandbyHandler, LinacStandbyHandler, \
     InjSysPUModeHandler
@@ -32,13 +35,14 @@
 from .sofb import SOFB
 from .syncd import DevicesSync
 from .timing import EVG, Event, Trigger, HLTiming
 from .tune import TuneFrac, TuneProc, Tune, TuneCorr
 from .dvf import DVF, DVFImgProc
 from .lienergy import LIEnergy
 from .blctrl import BLPPSCtrl
+from .scraper import ScraperH, ScraperV
 
 
 del device, bpm, dcct, egun, ict, lillrf, modltr
 del pwrsupply, posang, psconv, pssofb, rf, injsys, injctrl
 del screen, tune, sofb, timing, syncd, energy
-del ids, currinfo, bbb, machshift, dvf, lienergy, blctrl
+del ids, currinfo, bbb, machshift, dvf, lienergy, blctrl, scraper
```

### Comparing `siriuspy-2.78.0/siriuspy/devices/bbb.py` & `siriuspy-2.79.0/siriuspy/devices/bbb.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.78.0/siriuspy/devices/blctrl.py` & `siriuspy-2.79.0/siriuspy/devices/blctrl.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.78.0/siriuspy/devices/bpm.py` & `siriuspy-2.79.0/siriuspy/devices/bpm.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 """BPM devices."""
 
 import time as _time
 from threading import Event as _Flag
 import numpy as _np
 
-from .device import Device as _Device, Devices as _Devices, \
-    ProptyDevice as _ProptyDevice
+from .device import Device as _Device, Devices as _Devices
 from ..diagbeam.bpm.csdev import Const as _csbpm
 from ..search import BPMSearch as _BPMSearch
 from ..namesys import SiriusPVName as _PVName
 
 
 class BPM(_Device):
     """BPM Device."""
@@ -80,17 +79,14 @@
         )
 
     CONV_NM2UM = 1e-3  # [nm] --> [um]
 
     def __init__(self, devname, auto_monitor_mon=True, ispost_mortem=False):
         """."""
         # call base class constructor
-        if not _BPMSearch.is_valid_devname(devname):
-            raise ValueError(devname + ' is not a valid BPM or PBPM name.')
-
         self._ispost_mortem = ispost_mortem
         properties = {self.get_propname(p) for p in BPM._properties}
 
         if _BPMSearch.is_photon_bpm(devname):
             properties -= {'RFFEAtt-SP', 'RFFEAtt-RB'}
         properties = list(properties)
 
@@ -884,35 +880,47 @@
             return prop.replace('GEN', 'PM')
         elif prop.startswith('ACQ'):
             return prop.replace('ACQ', 'ACQ_PM')
         return prop
 
 
 class FamBPMs(_Devices):
-    """Family of BPMs."""
+    """Family of BPMs.
+
+    Parameters
+    ----------
+        devname (str, optional)
+            Device name. If not provided, defaults to DEVICES.SI.
+            Determine the list of BPM names.
+        bpmnames ((list, tuple), optional)
+            BPM names list. If provided, it takes priority over 'devname'
+            parameter. Defaults to None.
+        ispost_mortem (bool, optional)
+            Whether to control PM acquisition core. Defaults to False.
+    """
 
     TIMEOUT = 10
     RFFEATT_MAX = 30
 
     class DEVICES:
         """."""
 
         SI = 'SI-Fam:DI-BPM'
         BO = 'BO-Fam:DI-BPM'
         ALL = (BO, SI)
 
-    def __init__(self, devname=None, ispost_mortem=False):
+    def __init__(self, devname=None, bpmnames=None, ispost_mortem=False):
         """."""
         if devname is None:
             devname = self.DEVICES.SI
         if devname not in self.DEVICES.ALL:
             raise ValueError('Wrong value for devname')
 
         devname = _PVName(devname)
-        bpm_names = _BPMSearch.get_names(
+        bpm_names = bpmnames or _BPMSearch.get_names(
             filters={'sec': devname.sec, 'dev': devname.dev})
         self._ispost_mortem = ispost_mortem
         devs = [
             BPM(dev, auto_monitor_mon=False, ispost_mortem=ispost_mortem)
             for dev in bpm_names]
 
         super().__init__(devname, devs)
@@ -1091,34 +1099,43 @@
             acq_rate='FAcq', repeat=True, external=True) -> int:
         """Configure acquisition for BPMs.
 
         Args:
             nr_points_after (int): number of points after trigger.
             nr_points_before (int): number of points after trigger.
                 Defaults to 0.
-            acq_rate (str, optional): Acquisition rate ('TbT', 'FOFB',
-                'FAcq'). Defaults to 'FAcq'.
+            acq_rate (str, optional): Acquisition rate ('TbT', 'TbTPha',
+                'FOFB', 'FOFBPha', 'FAcq', 'ADC', 'ADCSwp').
+                Defaults to 'FAcq'.
             repeat (bool, optional): Whether or not acquisition should be
                 repetitive. Defaults to True.
             external (bool, optional): Whether or not external trigger should
                 be used. Defaults to True.
 
         Returns:
             int: code describing what happened:
                 =0: BPMs are ready.
                 <0: Index of the first BPM which did not stop last acq. plus 1.
                 >0: Index of the first BPM which is not ready for acq. plus 1.
 
         """
         if acq_rate.lower().startswith('facq'):
             acq_rate = self._csbpm.AcqChan.FAcq
+        elif acq_rate.lower().startswith('fofbpha'):
+            acq_rate = self._csbpm.AcqChan.FOFBPha
         elif acq_rate.lower().startswith('fofb'):
             acq_rate = self._csbpm.AcqChan.FOFB
+        elif acq_rate.lower().startswith('tbtpha'):
+            acq_rate = self._csbpm.AcqChan.TbTPha
         elif acq_rate.lower().startswith('tbt'):
             acq_rate = self._csbpm.AcqChan.TbT
+        elif acq_rate.lower().startswith('adcswp'):
+            acq_rate = self._csbpm.AcqChan.ADCSwp
+        elif acq_rate.lower().startswith('adc'):
+            acq_rate = self._csbpm.AcqChan.ADC
         else:
             raise ValueError(acq_rate + ' is not a valid acquisition rate.')
 
         if repeat:
             repeat = self._csbpm.AcqRepeat.Repetitive
         else:
             repeat = self._csbpm.AcqRepeat.Normal
@@ -1332,64 +1349,7 @@
 
         return self.mturn_wait_update_timestamps(
             timeout, consider_sum=consider_sum)
 
     def _mturn_set_flag(self, pvname, **kwargs):
         _ = kwargs
         self._mturn_flags[pvname].set()
-
-
-class BPMLogicalTrigger(_ProptyDevice):
-    """BPM Logical Trigger device."""
-
-    _properties = (
-        'RcvSrc-Sel', 'RcvSrc-Sts',
-        'RcvInSel-SP', 'RcvInSel-RB',
-        'TrnSrc-Sel', 'TrnSrc-Sts',
-        'TrnOutSel-SP', 'TrnOutSel-RB',
-    )
-
-    def __init__(self, bpmname, index):
-        """Init."""
-        if not _BPMSearch.is_valid_devname(bpmname):
-            raise NotImplementedError(bpmname)
-        if not 0 <= int(index) <= 23:
-            raise NotImplementedError(index)
-        super().__init__(
-            bpmname, 'TRIGGER'+str(index),
-            properties=BPMLogicalTrigger._properties)
-
-    @property
-    def receiver_source(self):
-        """Receiver source."""
-        return self['RcvSrc-Sts']
-
-    @receiver_source.setter
-    def receiver_source(self, value):
-        self['RcvSrc-Sel'] = value
-
-    @property
-    def receiver_in_sel(self):
-        """Receiver in selection."""
-        return self['RcvInSel-RB']
-
-    @receiver_in_sel.setter
-    def receiver_in_sel(self, value):
-        self['RcvInSel-SP'] = value
-
-    @property
-    def transmitter_source(self):
-        """Transmitter source."""
-        return self['TrnSrc-Sts']
-
-    @transmitter_source.setter
-    def transmitter_source(self, value):
-        self['TrnSrc-Sel'] = value
-
-    @property
-    def transmitter_out_sel(self):
-        """Transmitter out selection."""
-        return self['TrnOutSel-RB']
-
-    @transmitter_out_sel.setter
-    def transmitter_out_sel(self, value):
-        self['TrnOutSel-SP'] = value
```

### Comparing `siriuspy-2.78.0/siriuspy/devices/currinfo.py` & `siriuspy-2.79.0/siriuspy/devices/currinfo.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.78.0/siriuspy/devices/dcct.py` & `siriuspy-2.79.0/siriuspy/devices/dcct.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.78.0/siriuspy/devices/device.py` & `siriuspy-2.79.0/siriuspy/devices/device.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.78.0/siriuspy/devices/dvf.py` & `siriuspy-2.79.0/siriuspy/devices/timing.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,556 +1,624 @@
-"""DVF devices."""
+"""."""
+import time as _time
 
 import numpy as _np
 
 from mathphys.functions import get_namedtuple as _get_namedtuple
-from mathphys.imgproc import Image2D_Fit as _Image2D_Fit
-from mathphys.imgproc import FitGaussianScipy as _FitGaussianScipy
 
-from .device import DeviceNC as _DeviceNC
-
-
-class DVF(_DeviceNC):
-    """Beam Visualization Device ("Dispositivo de Visualização de Feixe")."""
-
-    class DEVICES:
-        """Devices names."""
-        CAX_DVF1 = 'CAX:A:BASLER01'
-        CAX_DVF2 = 'CAX:B:BASLER01'
-        ALL = (CAX_DVF1, CAX_DVF2)
-
-    _default_timeout = 10  # [s]
-
-    _dvfparam_fields = (
-        'MAX_INTENSITY_NR_BITS',
-        'ACQUISITION_TIME_MIN',  # [s]
-        'ACQUISITION_TIME_DEFAULT',  # [s]
-        'EXPOSURE_TIME_DEFAULT',  # [s]
-        'IMAGE_SIZE_Y',  # [pixel]
-        'IMAGE_SIZE_X',  # [pixel]
-        'IMAGE_PIXEL_SIZE',  # [um]
-        'OPTICS_MAGNIFICATION_FACTOR',  # source to image
-    )
-
-    _dev2params = {
-        DEVICES.CAX_DVF1:
-            _get_namedtuple(
-                'DVFParameters',
-                _dvfparam_fields, (16, 0.5, 0.5, 0.005, 2064, 3088, 2.4, 5.0)),
-        DEVICES.CAX_DVF2:
-            _get_namedtuple(
-                'DVFParameters',
-                _dvfparam_fields, (16, 0.5, 0.5, 0.005, 2064, 3088, 2.4, 5.0)),
-        }
+from .device import Device as _Device, ProptyDevice as _ProptyDevice, \
+    Devices as _Devices
+from ..timesys.csdev import ETypes as _ETypes, Const as _TIConst, \
+    get_hl_trigger_database as _get_hl_trigger_database
+from ..search import HLTimeSearch as _HLTimeSearch
+from ..util import get_bit as _get_bit
+
+
+class EVG(_Device):
+    """Device EVG."""
+
+    DEVNAME = 'AS-RaMO:TI-EVG'
+    StateMachine = _get_namedtuple('StateMachine', (
+        'Initializing', 'Stopped', 'Continuous', 'Injection',
+        'Preparing_Continuous', 'Preparing_Injection',
+        'Restarting_Continuous'))
 
     _properties = (
-        'cam1:MaxSizeX_RBV', 'cam1:MaxSizeY_RBV',
-        'cam1:ArrayCallbacks', 'cam1:ArrayCallbacks_RBV',
-        'cam1:AcquireTime', 'cam1:AcquireTime_RBV',
-        'cam1:AcquirePeriod', 'cam1:AcquirePeriod_RBV',
-        'cam1:Acquire', 'cam1:Acquire_RBV',
-        'cam1:ImageMode', 'cam1:ImageMode_RBV',
-        'cam1:Gain', 'cam1:Gain_RBV',
-        'cam1:GainAuto', 'cam1:GainAuto_RBV',
-        'cam1:DataType', 'cam1:DataType_RBV',
-        'cam1:PixelFormat', 'cam1:PixelFormat_RBV',
-        'cam1:PixelSize', 'cam1:PixelSize_RBV',
-        'cam1:SizeX_RBV', 'cam1:SizeY_RBV',
-        'cam1:Temperature',
-        'cam1:FAILURES_RBV', 'cam1:COMPLETED_RBV',
-        'ROI1:NDArrayPort', 'ROI1:NDArrayPort_RBV',
-        'ROI1:EnableCallbacks', 'ROI1:EnableCallbacks_RBV',
-        'ROI1:MinX', 'ROI1:MinX_RBV',
-        'ROI1:MinY', 'ROI1:MinY_RBV',
-        'ROI1:SizeX', 'ROI1:SizeX_RBV',
-        'ROI1:SizeY', 'ROI1:SizeY_RBV',
-        'ROI1:EnableX', 'ROI1:EnableX_RBV',
-        'ROI1:EnableY', 'ROI1:EnableY_RBV',
-        'ROI1:ArrayCallbacks', 'ROI1:ArrayCallbacks_RBV',
-        'image1:NDArrayPort', 'image1:NDArrayPort_RBV',
-        'image1:EnableCallbacks', 'image1:EnableCallbacks_RBV',
-        'image1:ArraySize0_RBV', 'image1:ArraySize1_RBV',
-        'image1:ArrayData',
-        'ffmstream1:EnableCallbacks', 'ffmstream1:EnableCallbacks_RBV',
-        'Trans1:EnableCallbacks', 'Trans1:EnableCallbacks_RBV',
-        'HDF1:EnableCallbacks', 'HDF1:EnableCallbacks_RBV',
-        )
+        'InjectionEvt-Sel', 'InjectionEvt-Sts', 'UpdateEvt-Cmd',
+        'ContinuousEvt-Sel', 'ContinuousEvt-Sts', 'STATEMACHINE',
+        'RepeatBucketList-SP', 'RepeatBucketList-RB',
+        'BucketList-SP', 'BucketList-RB', 'BucketList-Mon',
+        'BucketListLen-Mon', 'TotalInjCount-Mon', 'InjCount-Mon',
+        'BucketListSyncStatus-Mon')
 
-    def __init__(self, devname, *args, **kwargs):
-        """Init."""
-        # check if device exists
-        if devname not in DVF.DEVICES.ALL:
-            raise NotImplementedError(devname)
-        # call base class constructor
-        super().__init__(devname, properties=self._properties, *args, **kwargs)
+    def __init__(self):
+        """."""
+        super().__init__(EVG.DEVNAME, properties=EVG._properties)
 
     @property
-    def parameters(self):
-        """Return DVF parameters."""
-        return DVF._dev2params[self.devname]
+    def nrpulses(self):
+        """Number of pulses to repeat Bucket List."""
+        return self['RepeatBucketList-RB']
 
-    @property
-    def intensity_saturation_value(self):
-        """Image intensity saturation value."""
-        pixel_format_to_num_bits = {0: 8, 1: 12}  # 0: 'Mono8, 1: 'Mono12
-        data_type_to_num_bits = {0: 8, 1: 16} # 0: 'UInt8', 1: 'UInt16'
-        used_bits = pixel_format_to_num_bits[self.pixel_format]
-        max_bits = data_type_to_num_bits[self.data_type]
-        max_intensity = (1 << used_bits) - 1
-        if used_bits <= max_bits:
-            # Shift intensity to align with most-significant bits
-            max_intensity <<= max_bits - used_bits
-        elif used_bits > max_bits:
-            # Clip to maximum value allowed by the data type
-            max_intensity = (1 << max_bits) - 1
-        return max_intensity
+    @nrpulses.setter
+    def nrpulses(self, value):
+        """Set number of pulses to repeat Bucket List."""
+        self['RepeatBucketList-SP'] = value
 
     @property
-    def exposure_time(self):
-        """Camera exposure time [s]."""
-        return self['cam1:AcquireTime']
-
-    @exposure_time.setter
-    def exposure_time(self, value):
-        """Camera exposure time [s]."""
-        value = max(value, 0)
-        self['cam1:AcquireTime'] = value
+    def bucketlist_len(self):
+        """Bucket List Length."""
+        value = self['BucketListLen-Mon']
+        return int(value) if value is not None else None
 
     @property
-    def acquisition_time(self):
-        """Camera acquisition time [s]."""
-        return self['cam1:AcquirePeriod']
-
-    @acquisition_time.setter
-    def acquisition_time(self, value):
-        """Camera acquisition time [s]."""
-        params = self.parameters
-        value = max(value, params.ACQUISITION_TIME_MIN)
-        self['cam1:AcquirePeriod'] = value
+    def bucketlist_mon(self):
+        """Implemented Bucket List."""
+        return self['BucketList-Mon'][:self.bucketlist_len]
 
     @property
-    def acquisition_status(self):
-        """Return IOC acquisition status."""
-        return self['cam1:Acquire']
+    def bucketlist(self):
+        """Last setpoint accepted for Bucket List."""
+        return self['BucketList-RB'][:self.bucketlist_len]
 
-    @property
-    def cam_max_sizex(self):
-        """Camera max second dimension size (pixels)."""
-        return self['cam1:MaxSizeX_RBV']
+    @bucketlist.setter
+    def bucketlist(self, value):
+        """Set Bucket List."""
+        self['BucketList-SP'] = _np.array(value, dtype=int)
 
     @property
-    def cam_max_sizey(self):
-        """Camera max first dimension size (pixels)."""
-        return self['cam1:MaxSizeY_RBV']
+    def bucketlist_sync(self):
+        """Bucket list syncronized status."""
+        return self['BucketListSyncStatus-Mon']
 
     @property
-    def cam_sizex(self):
-        """Camera second dimension size (pixels)."""
-        return self['cam1:SizeX_RBV']
+    def continuous_state(self):
+        """."""
+        return bool(self['ContinuousEvt-Sts'])
 
-    @property
-    def cam_sizey(self):
-        """Camera first dimension size (pixels)."""
-        return self['cam1:SizeY_RBV']
+    @continuous_state.setter
+    def continuous_state(self, value):
+        """."""
+        new_val = bool(value)
+        if self.continuous_state != new_val:
+            self['ContinuousEvt-Sel'] = int(new_val)
 
     @property
-    def roi_minx(self):
+    def state_machine(self):
         """."""
-        return self['ROI1:MinX_RBV']
+        return self['STATEMACHINE']
 
-    @roi_minx.setter
-    def roi_minx(self, value):
+    @property
+    def state_machine_str(self):
         """."""
-        self['ROI1:MinX'] = int(value)
+        return self.StateMachine._fields[self.state_machine]
 
     @property
-    def roi_miny(self):
+    def injection_state(self):
         """."""
-        return self['ROI1:MinY_RBV']
+        return bool(self['InjectionEvt-Sts'])
 
-    @roi_miny.setter
-    def roi_miny(self, value):
+    @injection_state.setter
+    def injection_state(self, value):
         """."""
-        self['ROI1:MinY'] = int(value)
+        new_val = bool(value)
+        if self.injection_state != new_val:
+            self['InjectionEvt-Sel'] = int(new_val)
 
     @property
-    def image_sizex(self):
-        """Image second dimension size (pixels)."""
-        return self['image1:ArraySize0_RBV']
+    def injection_count_total(self):
+        """."""
+        return self['TotalInjCount-Mon']
 
     @property
-    def image_sizey(self):
-        """Image first dimension size (pixels)."""
-        return self['image1:ArraySize1_RBV']
+    def injection_count(self):
+        """."""
+        return self['InjCount-Mon']
 
-    @property
-    def image(self):
-        """Return DVF image formatted as a (sizey, sizex) numpy matrix."""
-        shape = (self.image_sizey, self.image_sizex)
-        data = self['image1:ArrayData']
-        image = _np.reshape(data, shape)
-        return image
+    def fill_bucketlist(self, stop, start=1, step=30, timeout=10):
+        """Fill bucket list."""
+        if (step > 0) and (start > stop):
+            stop += 864
+        if (step < 0) and (stop > start):
+            stop -= 864
+        value = _np.arange(start, stop, step)
+        value = (value-1) % 864 + 1
+        self.bucketlist = value
+        rb_value = _np.zeros(864)
+        rb_value[:len(value)] = value
+        return self._wait('BucketList-RB', rb_value, timeout=timeout)
 
-    @property
-    def image_pixel_size(self):
-        """Image pixel size [um]."""
-        params = self.parameters
-        return params.IMAGE_PIXEL_SIZE
+    def wait_injection_finish(self, timeout=10):
+        """."""
+        return self._wait(propty='InjectionEvt-Sts', value=0, timeout=timeout)
 
-    @property
-    def optics_magnification_factor(self):
-        """Source to image magnification factor."""
-        params = self.parameters
-        return params.OPTICS_MAGNIFICATION_FACTOR
+    def cmd_update_events(self, timeout=10):
+        """."""
+        val = self.continuous_state
+        self['UpdateEvt-Cmd'] = 1
+        _time.sleep(0.1)
+        return self._wait(
+            propty='ContinuousEvt-Sts', value=val, timeout=timeout)
 
-    @property
-    def conv_pixel_2_srcsize(self):
-        """Pixel to source size convertion factor."""
-        pixel_size = self.image_pixel_size
-        mag_factor = self.optics_magnefication_factor
-        pixel2srcsize = pixel_size / mag_factor
-        return pixel2srcsize
+    def cmd_turn_on_injection(self, timeout=10, wait_rb=False):
+        """."""
+        self.injection_state = 1
+        pv2wait = 'InjectionEvt-' + ('Sts' if wait_rb else 'Sel')
+        return self._wait(propty=pv2wait, value=1, timeout=timeout)
 
-    @property
-    def gain(self):
-        """Return camera gain."""
-        return self['cam1:Gain_RBV']
+    def cmd_turn_off_injection(self, timeout=10, wait_rb=False):
+        """."""
+        self.injection_state = 0
+        pv2wait = 'InjectionEvt-' + ('Sts' if wait_rb else 'Sel')
+        return self._wait(propty=pv2wait, value=0, timeout=timeout)
 
-    @gain.setter
-    def gain(self, value):
-        """Set camera gain."""
-        self['cam1:Gain'] = value
+    def cmd_turn_on_continuous(self, timeout=10, wait_rb=False):
+        """."""
+        self.continuous_state = 1
+        pv2wait = 'ContinuousEvt-' + ('Sts' if wait_rb else 'Sel')
+        return self._wait(propty=pv2wait, value=1, timeout=timeout)
 
-    @property
-    def gain_auto(self):
-        """Return camera gain auto."""
-        return self['cam1:GainAuto_RBV']
+    def cmd_turn_off_continuous(self, timeout=10, wait_rb=False):
+        """."""
+        self.continuous_state = 0
+        pv2wait = 'ContinuousEvt-' + ('Sts' if wait_rb else 'Sel')
+        return self._wait(propty=pv2wait, value=0, timeout=timeout)
 
-    @gain.setter
-    def gain_auto(self, value):
-        """Set camera gain auto."""
-        self['cam1:GainAuto'] = value
+    def set_nrpulses(self, value, timeout=10):
+        """Set and wait number of pulses."""
+        self['RepeatBucketList-SP'] = value
+        return self._wait('RepeatBucketList-RB', value, timeout=timeout)
 
-    @property
-    def pixel_format(self):
-        """Return camera pixel format."""
-        return self['cam1:PixelFormat_RBV']
 
-    @pixel_format.setter
-    def pixel_format(self, value):
-        """Set camera pixel format."""
-        self['cam1:PixelFormat'] = value
+class Event(_ProptyDevice):
+    """Device Timing Event."""
 
-    @property
-    def data_type(self):
-        """Return camera data type."""
-        return self['cam1:DataType_RBV']
+    _properties = (
+        'Delay-SP', 'Delay-RB', 'DelayRaw-SP', 'DelayRaw-RB',
+        'DelayType-Sel', 'DelayType-Sts', 'Mode-Sel', 'Mode-Sts',
+        'Code-Mon', 'ExtTrig-Cmd',
+        )
 
-    @data_type.setter
-    def data_type(self, value):
-        """Set camera data type."""
-        self['cam1:DataType'] = value
+    MODES = _ETypes.EVT_MODES
+    DELAYTYPES = ('Incr', 'Fixed')
+
+    def __init__(self, evtname):
+        """."""
+        super().__init__(
+            EVG.DEVNAME, evtname, properties=Event._properties)
 
     @property
-    def pixel_size(self):
-        """Return camera pixel size."""
-        return self['cam1:PixelSize_RBV']
+    def mode(self):
+        """."""
+        return self['Mode-Sts']
 
-    @pixel_size.setter
-    def pixel_size(self, value):
-        """Set camera pixel size."""
-        self['cam1:PixelSize'] = value
+    @mode.setter
+    def mode(self, value):
+        self._enum_setter('Mode-Sel', value, Event.MODES)
 
     @property
-    def cam_temperature(self):
-        """Return camera temperature"""
-        return self['cam1:Temperature']
+    def mode_str(self):
+        """."""
+        mode = self['Mode-Sts']
+        if mode is not None:
+            return Event.MODES[mode]
+        return None
 
     @property
-    def cam_frames_completed(self):
-        """Return number of acquisition frames completed."""
-        return self['cam1:COMPLETED_RBV']
+    def code(self):
+        """."""
+        return self['Code-Mon']
 
     @property
-    def cam_frames_failures(self):
-        """Return number of acquisition frames failures."""
-        return self['cam1:FAILURES_RBV']
+    def delay_type(self):
+        """."""
+        return self['DelayType-Sts']
 
-    def cmd_reset(self, timeout=None):
-        """Reset DVF to a standard configuration."""
-        props_values = {
-            'cam1:ArrayCallbacks': 1,  # Enable passing array
-            'cam1:ImageMode': 2,  # Continuous
-            'cam1:PixelFormat': 1,  # Mono12
-            'cam1:DataType': 1,  # UInt16 (maybe unnecessary)
-            'ROI1:NDArrayPort': 'CAMPORT',  # Take img from camport
-            'ROI1:EnableCallbacks': 1,  # Enable getting from NDArrayPort
-            'ROI1:MinX': 0,  # [pixel]
-            'ROI1:MinY': 0,  # [pixel]
-            'ROI1:SizeX': self.cam_max_sizex,  # [pixel]
-            'ROI1:SizeY': self.cam_max_sizey,  # [pixel]
-            'ROI1:EnableX': 1,  # Enable
-            'ROI1:EnableY': 1,  # Enable
-            'ROI1:ArrayCallbacks': 1,  # Enable passing array
-            'image1:NDArrayPort': 'ROI1',  # image1 takes img from ROI1
-            'image1:EnableCallbacks': 1,  # Enable
-            'ffmstream1:EnableCallbacks': 0,  # Disable
-            'HDF1:EnableCallbacks': 0,  # Disable
-            'Trans1:EnableCallbacks': 0,  # Disable
-        }
+    @delay_type.setter
+    def delay_type(self, value):
+        self._enum_setter('DelayType-Sel', value, Event.DELAYTYPES)
 
-        # set properties
-        for propty, value in props_values.items():
-            self[propty] = value
+    @property
+    def delay_type_str(self):
+        """."""
+        dlytyp = self['DelayType-Sts']
+        if dlytyp is not None:
+            return Event.DELAYTYPES[dlytyp]
+        return None
 
-        # check readback values
-        for propty, value in props_values.items():
-            if not self._wait(propty + '_RBV', value, timeout=timeout):
-                return False
+    @property
+    def delay(self):
+        """."""
+        return self['Delay-RB']
 
-        # configure image acquisition parameters
-        params = self.parameters
-        self.exposure_time = params.EXPOSURE_TIME_DEFAULT
-        self.acquisition_time = params.ACQUISITION_TIME_DEFAULT
-        return True
+    @delay.setter
+    def delay(self, value):
+        self['Delay-SP'] = value
 
-    def cmd_acquire_on(self, timeout=None):
-        """Tune IOC image acquisition on."""
-        return self._set_and_wait('cam1:Acquire', 1, timeout=timeout)
+    @property
+    def delay_raw(self):
+        """."""
+        return self['DelayRaw-RB']
 
-    def cmd_acquire_off(self, timeout=None):
-        """Tune IOC image acquisition off."""
-        return self._set_and_wait('cam1:Acquire', 0, timeout=timeout)
+    @delay_raw.setter
+    def delay_raw(self, value):
+        self['DelayRaw-SP'] = int(value)
 
-    @staticmethod
-    def conv_devname2parameters(devname):
+    def cmd_external_trigger(self):
         """."""
-        return DVF._dev2params[devname]
+        self['ExtTrig-Cmd'] = 1
+        return True
 
-    def _set_and_wait(self, propty, value, timeout=None):
+    @property
+    def is_in_inj_table(self):
         """."""
-        timeout = timeout or self._default_timeout
-        self[propty] = value
-        return self._wait(propty + '_RBV', value, timeout=timeout)
+        return self.mode_str in Event.MODES[1:4]
 
 
-class DVFImgProc(DVF):
-    """."""
+class Trigger(_Device):
+    """Device trigger."""
 
-    _properties = DVF._properties + (
-        'ImgIntensityMax-Mon', 'ImgIntensityMin-Mon',
-        'ImgIntensitySum-Mon', 'ImgIsSaturated-Mon',
-        'ImgIsWithBeam-Mon',
-        'ImgIsWithBeamThreshold-SP', 'ImgIsWithBeamThreshold-RB',
-
-        'ImgROIX-RB', 'ImgROIX-SP',
-        'ImgROIXCenter-Mon', 'ImgROIXFWHM-Mon',
-        'ImgROIY-RB', 'ImgROIY-SP',
-        'ImgROIYCenter-Mon', 'ImgROIYFWHM-Mon',
-
-        'ImgLog-Mon',
-        'ImgROIUpdateWithFWHM-Sel', 'ImgROIUpdateWithFWHM-Sts',
-        'ImgROIYUpdateWithFWHMFactor-RB', 'ImgROIYUpdateWithFWHMFactor-SP',
-        'ImgROIXUpdateWithFWHMFactor-RB', 'ImgROIXUpdateWithFWHMFactor-SP',
-
-        'ImgROIXFitMean-Mon', 'ImgROIXFitSigma-Mon',
-        'ImgROIXFitAmplitude-Mon', 'ImgROIXFitError-Mon',
-        'ImgROIYFitMean-Mon', 'ImgROIYFitSigma-Mon',
-        'ImgROIYFitAmplitude-Mon', 'ImgROIYFitError-Mon',
-        'ImgFitAngle-Mon',
-        'ImgFitSigma1-Mon', 'ImgFitSigma2-Mon',
-        'ImgFitProcTime-Mon',
-        'ImgFitAngleUseCMomSVD-Sel', 'ImgFitAngleUseCMomSVD-Sts',
-        'ImgDVFStatus-Mon', 'ImgDVFStatusLabels-Cte',
-        )
+    STATES = ('Dsbl', 'Enbl')
+    LOCKLL = ('Unlocked', 'Locked')
+    POLARITIES = ('Normal', 'Inverse')
 
-    def __init__(self, devname, *args, **kwargs):
-        """."""
-        super().__init__(devname=devname, *args, **kwargs)
-        self._fitgaussian = _FitGaussianScipy()
+    def __init__(self, trigname):
+        """Init."""
+        self._database = _get_hl_trigger_database(trigname)
+        self._properties = tuple(self._database)
+        self._source_options = self._database['Src-Sel']['enums']
+        super().__init__(trigname, properties=self._properties)
 
     @property
-    def intensity_min(self):
-        """Image min intensity."""
-        return self['ImgIntensityMin-Mon']
+    def status(self):
+        """Status."""
+        return self['Status-Mon']
 
     @property
-    def intensity_max(self):
-        """Image max intensity."""
-        return self['ImgIntensityMax-Mon']
+    def status_str(self):
+        """Status string."""
+        value = self.status
+        strs = [d for i, d in enumerate(_TIConst.HLTrigStatusLabels)
+                if _get_bit(value, i)]
+        return ', '.join(strs) if strs else 'Ok'
 
     @property
-    def intensity_sum(self):
-        """Image sum intensity."""
-        return self['ImgIntensitySum-Mon']
+    def status_labels(self):
+        """Return Status labels of trigger.
+
+        Returns:
+            list: labels describing the possible statuses of the trigger.
+
+        """
+        pvo = self.pv_object('StatusLabels-Cte')
+        return pvo.get(as_string=True).split('\n')
 
     @property
-    def is_saturated(self):
-        """Whether image is saturated."""
-        return self['ImgIsSaturated-Mon']
+    def state(self):
+        """State."""
+        return self['State-Sts']
+
+    @state.setter
+    def state(self, value):
+        self._enum_setter('State-Sel', value, Trigger.STATES)
 
     @property
-    def is_with_beam(self):
-        """Whether image is with beam."""
-        return self['ImgIsWithBeam-Mon']
+    def state_str(self):
+        """State string."""
+        return Trigger.STATES[self['State-Sts']]
 
     @property
-    def is_with_beam_threashold(self):
-        """Get image is with beam threashold."""
-        return self['ImgIsWithBeamThreshold-RB']
+    def lock_low_level(self):
+        """Lock low level status."""
+        return self['LowLvlLock-Sts']
 
-    @is_with_beam_threashold.setter
-    def is_with_beam_threashold(self, value):
-        """Set image is with beam threashold."""
-        self['ImgIsWithBeamThreshold-SP'] = value
+    @lock_low_level.setter
+    def lock_low_level(self, value):
+        self._enum_setter('LowLvlLock-Sel', value, Trigger.LOCKLL)
 
     @property
-    def roiy(self):
-        """."""
-        return self['ImgROIY-RB']
-
-    @roiy.setter
-    def roiy(self, value):
-        """."""
-        self['ImgROIY-SP'] = value
+    def lock_low_level_str(self):
+        """Lock low level status string."""
+        return Trigger.LOCKLL[self['LowLvlLock-Sts']]
 
     @property
-    def roix(self):
-        """."""
-        return self['ImgROIX-RB']
+    def controlled_channels(self):
+        """Return channels controlled by this trigger.
 
-    @roix.setter
-    def roix(self, value):
-        """."""
-        self['ImgROIX-SP'] = value
+        Returns:
+            list: names of the controlled channels.
 
-    @property
-    def roiy_center(self):
-        """."""
-        return self['ImgROIYCenter-Mon']
+        """
+        pvo = self.pv_object('CtrldChannels-Cte')
+        return pvo.get(as_string=True).split('\n')
 
     @property
-    def roix_center(self):
-        """."""
-        return self['ImgROIXCenter-Mon']
+    def low_level_triggers(self):
+        """Return low level triggers controlled by this trigger.
+
+        Returns:
+            list: names of the controlled low level triggers.
+
+        """
+        pvo = self.pv_object('LowLvlTriggers-Cte')
+        return pvo.get(as_string=True).split('\n')
 
     @property
-    def roiy_fwhm(self):
-        """."""
-        return self['ImgROIYFWHM-Mon']
+    def source(self):
+        """Source."""
+        return self['Src-Sts']
+
+    @source.setter
+    def source(self, value):
+        self._enum_setter('Src-Sel', value, self._source_options)
 
     @property
-    def roix_fwhm(self):
-        """."""
-        return self['ImgROIXFWHM-Mon']
+    def source_str(self):
+        """Source string."""
+        if self['Src-Sts'] is not None:
+            return self._source_options[self['Src-Sts']]
+        return
 
     @property
-    def roiy_fit_amplitude(self):
-        """."""
-        return self['ImgROIYFitAmplitude-Mon']
+    def source_options(self):
+        """Source options."""
+        return self._source_options
 
     @property
-    def roix_fit_amplitude(self):
-        """."""
-        return self['ImgROIXFitAmplitude-Mon']
+    def duration(self):
+        """Duration."""
+        return self['Duration-RB']
+
+    @duration.setter
+    def duration(self, value):
+        self['Duration-SP'] = value
 
     @property
-    def roiy_fit_mean(self):
-        """."""
-        return self['ImgROIYFitMean-Mon']
+    def width_raw(self):
+        """Width of one pulse in hardware units."""
+        return self['WidthRaw-RB']
+
+    @width_raw.setter
+    def width_raw(self, value):
+        self['WidthRaw-SP'] = value
 
     @property
-    def roix_fit_mean(self):
-        """."""
-        return self['ImgROIXFitMean-Mon']
+    def polarity(self):
+        """Polarity."""
+        return self['Polarity-Sts']
+
+    @polarity.setter
+    def polarity(self, value):
+        self._enum_setter('Polarity-Sel', value, Trigger.POLARITIES)
 
     @property
-    def roiy_fit_sigma(self):
-        """."""
-        return self['ImgROIYFitSigma-Mon']
+    def polarity_str(self):
+        """Polarity string."""
+        return Trigger.POLARITIES[self['Polarity-Sts']]
 
     @property
-    def roix_fit_sigma(self):
-        """."""
-        return self['ImgROIXFitSigma-Mon']
+    def nr_pulses(self):
+        """Nr. of pulses."""
+        return self['NrPulses-RB']
+
+    @nr_pulses.setter
+    def nr_pulses(self, value):
+        self['NrPulses-SP'] = value
 
     @property
-    def roiy_fit_error(self):
-        """."""
-        return self['ImgROIYFitError-Mon']
+    def delay(self):
+        """Delay."""
+        return self['Delay-RB']
+
+    @delay.setter
+    def delay(self, value):
+        self['Delay-SP'] = value
 
     @property
-    def roix_fit_error(self):
-        """."""
-        return self['ImgROIXFitError-Mon']
+    def total_delay(self):
+        """Total delay."""
+        return self['TotalDelay-Mon']
 
     @property
-    def roiy_fwhm_factor(self):
-        """."""
-        return self['ImgROIYUpdateWithFWHMFactor-RB']
+    def delta_delay(self):
+        """Return delta delay array.
 
-    @roiy_fwhm_factor.setter
-    def roiy_fwhm_factor(self, value):
-        """."""
-        self['ImgROIYUpdateWithFWHMFactor-SP'] = value
+        Returns:
+            numpy.ndarray: delta delays.
 
-    @property
-    def roix_fwhm_factor(self):
-        """."""
-        return self['ImgROIXUpdateWithFWHMFactor-RB']
+        """
+        return self['DeltaDelay-RB']
 
-    @roix_fwhm_factor.setter
-    def roix_fwhm_factor(self, value):
-        """."""
-        self['ImgROIXUpdateWithFWHMFactor-SP'] = value
+    @delta_delay.setter
+    def delta_delay(self, value):
+        if not isinstance(value, (_np.ndarray, list, tuple)):
+            raise TypeError('Value must be a numpy.ndarray, list or tuple.')
+
+        value = _np.array(value)
+        size = self.delta_delay.size
+        if value.size != size:
+            raise TypeError(f'Size of value must be {size:d}.')
+        self['DeltaDelay-SP'] = value
 
     @property
-    def roi_update_with_fwhm(self):
-        """."""
-        return bool(self['ImgROIUpdateWithFWHM-Sts'])
+    def delay_raw(self):
+        """Delay raw."""
+        return self['DelayRaw-RB']
 
-    @roi_update_with_fwhm.setter
-    def roi_update_with_fwhm(self, value):
-        """."""
-        self['ImgROIUpdateWithFWHM-Sel'] = bool(value)
+    @delay_raw.setter
+    def delay_raw(self, value):
+        self['DelayRaw-SP'] = value
 
     @property
-    def fit_angle(self):
-        """."""
-        return self['ImgFitAngle-Mon']
+    def total_delay_raw(self):
+        """Total delay raw."""
+        return self['TotalDelayRaw-Mon']
 
     @property
-    def fit_sigma1(self):
-        """."""
-        return self['ImgFitSigma1-Mon']
+    def delta_delay_raw(self):
+        """Return delta delay raw array.
 
-    @property
-    def fit_sigma2(self):
-        """."""
-        return self['ImgFitSigma2-Mon']
+        Returns:
+            numpy.ndarray: delta delays raw.
 
-    @property
-    def fit_proctime(self):
-        """Return image processing time [ms]."""
-        return self['ImgFitProcTime-Mon']
+        """
+        return self['DeltaDelayRaw-RB']
 
-    @property
-    def fit_angle_use_cmom_svd(self):
-        """."""
-        return self['ImgFitAngleUseCMomSVD-Sts']
+    @delta_delay_raw.setter
+    def delta_delay_raw(self, value):
+        if not isinstance(value, (_np.ndarray, list, tuple)):
+            raise TypeError('Value must be a numpy.ndarray, list or tuple.')
 
-    @fit_angle_use_cmom_svd.setter
-    def fit_angle_use_cmom_svd(self, value):
-        """."""
-        self['ImgFitAngleUseCMomSVD-Sel'] = bool(value)
+        value = _np.array(value)
+        size = self.delta_delay_raw.size
+        if value.size != size:
+            raise TypeError(f'Size of value must be {size:d}.')
+        self['DeltaDelayRaw-SP'] = value
 
     @property
-    def log(self):
+    def is_in_inj_table(self):
+        """Is in Injection table."""
+        return self['InInjTable-Mon']
+
+    def cmd_enable(self, timeout=3):
+        """Command enable."""
+        self.state = 1
+        return self._wait('State-Sts', 1, timeout)
+
+    def cmd_disable(self, timeout=3):
+        """Command disable."""
+        self.state = 0
+        return self._wait('State-Sts', 0, timeout)
+
+    def cmd_lock_low_level(self, timeout=3):
+        """Lock low level IOCs state."""
+        self.lock_low_level = 1
+        return self._wait('LowLvlLock-Sts', 1, timeout)
+
+    def cmd_unlock_low_level(self, timeout=3):
+        """Unlock low level IOCs state."""
+        self.lock_low_level = 0
+        return self._wait('LowLvlLock-Sts', 0, timeout)
+
+
+class HLTiming(_Devices):
+    """."""
+
+    SEARCH = _HLTimeSearch
+
+    def __init__(self):
         """."""
-        return self['ImgLog-Mon']
+        self.evg = EVG()
+        evs = self.SEARCH.get_configurable_hl_events()
+        self.events = {ev: Event(ev) for ev in evs.keys()}
+        self.triggers = {t: Trigger(t) for t in self.SEARCH.get_hl_triggers()}
+        devs = [self.evg, ]
+        devs += list(self.events.values())
+        devs += list(self.triggers.values())
+        super().__init__('AS-Glob:TI-HLTiming', devs)
+
+    def get_mapping_events2triggers(self) -> dict:
+        """."""
+        map_ = {tn: tr.source_str for tn, tr in self.triggers.items()}
+        inv_map = {ev: list() for ev in set(map_.values())}
+        for tn, ev in map_.items():
+            inv_map[ev].append(tn)
+        return inv_map
+
+    def get_mapping_injtable2events(self) -> dict:
+        """."""
+        map_evt2table = {n: o.mode_str for n, o in self.events.items()}
+        map_table2evt = {}
+        for k, v in map_evt2table.items():
+            map_table2evt[v] = map_table2evt.get(v, []) + [k]
+        return map_table2evt
+
+    def change_triggers_source(
+            self, trigs, new_src='Linac', printlog=True) -> list:
+        """."""
+        notchanged = list()
+        for tn in trigs:
+            tr = self.triggers[tn]
+
+            if new_src not in tr.source_options:
+                if printlog:
+                    print(
+                        f'{tn:25s} -> No Change: {new_src:s}'
+                        ' is not an option.')
+                notchanged.append(tn)
+                continue
+
+            dly_newsrc = 0
+            if new_src in self.events:
+                dly_newsrc = self.events[new_src].delay_raw
+
+            dly_oldsrc = 0
+            old_src = tr.source_str
+            if old_src in self.events:
+                dly_oldsrc = self.events[old_src].delay_raw
+
+            dly = tr.delay_raw
+            delta_dly = dly_oldsrc
+            delta_dly -= dly_newsrc
+            dly += delta_dly
+            if dly < 0:
+                notchanged.append(tn)
+                if printlog:
+                    print(f'{tn:25s} -> No Change: total delay not constant!')
+                continue
+
+            tr.delay_raw = dly
+            tr.source = new_src
+            if printlog:
+                print(f'{tn:25s} -> Change OK: .')
+        return notchanged
+
+    def change_event_delay(self, new_dly, event='Linac', printlog=True):
+        """."""
+        if event not in self.events:
+            if printlog:
+                print(f'{event} is not a valid event!')
+            return False
+        new_dly = int(new_dly)
+        old_dly = self.events[event].delay_raw
+        dlt_dly = old_dly - new_dly
+
+        trigs = self.get_mapping_events2triggers()[event]
+        for trn in trigs:
+            dly = self.triggers[trn].delay_raw + dlt_dly
+            if dly < 0:
+                if printlog:
+                    print(f'cannot change delay: {trn:s} would change!')
+                return False
 
-    def create_image2dfit(self):
-        """Return a Image2DFit object with current image as data."""
-        imgfit2d = _Image2D_Fit(
-            data=self.image, fitgauss=self._fitgaussian,
-            roix=self.roix, roiy=self.roiy)
-        return imgfit2d
+        for trn in trigs:
+            self.triggers[trn].delay_raw += dlt_dly
+        self.events[event].delay_raw = new_dly
+        if printlog:
+            print('Delay changed!')
+        return True
+
+    def print_injtable_mapping(self, only_enabled=False):
+        """."""
+        map_evt2trig = self.get_mapping_events2triggers()
+        map_table2evt = self.get_mapping_injtable2events()
+        tabs = {'Continuous', 'Injection', 'OneShot'}
+        tabs &= map_table2evt.keys()
+        tabs = sorted(tabs)
+
+        dlys = []
+        for tab in tabs:
+            for evt in map_table2evt[tab]:
+                for name in map_evt2trig.get(evt, []):
+                    obj = self.triggers[name]
+                    if only_enabled and not obj.enabled:
+                        continue
+                    dlys.append([obj.total_delay, name, evt, tab])
+        dlys = sorted(dlys)
+
+        tmpl = ' {:^30s} |' * len(tabs)
+        print(('{:^12s} |' + tmpl).format('Delay [ms]', *tabs))
+        print('-'*(12+33*len(tabs) + 2))
+        for dly, trg, evt, tab in dlys:
+            stgs = [''] * len(tabs)
+            stgs[tabs.index(tab)] = trg
+            print(('{:>12.6f} |' + tmpl).format(dly/1e3, *stgs))
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `siriuspy-2.78.0/siriuspy/devices/egun.py` & `siriuspy-2.79.0/siriuspy/devices/egun.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.78.0/siriuspy/devices/energy.py` & `siriuspy-2.79.0/siriuspy/devices/energy.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.78.0/siriuspy/devices/fofb.py` & `siriuspy-2.79.0/siriuspy/devices/fofb.py`

 * *Files 5% similar despite different names*

```diff
@@ -6,29 +6,31 @@
 
 from ..namesys import SiriusPVName as _PVName
 from ..search import BPMSearch as _BPMSearch, PSSearch as _PSSearch
 from ..fofb.csdev import HLFOFBConst as _Const, NR_BPM
 
 from .device import Device as _Device, ProptyDevice as _ProptyDevice, \
     Devices as _Devices
-from .bpm import BPMLogicalTrigger
+from .afc_acq_core import AFCACQLogicalTrigger
 from .timing import Event
 from .pwrsupply import PowerSupplyFC
 from .psconv import StrengthConv
 
 
-class _FOFBCtrlBase:
+class FOFBCtrlBase:
     """FOFB Ctrl base."""
 
     _devices = {
         f'SI{i:02d}': f'IA-{i:02d}RaBPM:BS-FOFBCtrl' for i in range(1, 21)}
     DEVICES = _get_namedtuple('DEVICES', *zip(*_devices.items()))
 
 
-class FOFBCtrlRef(_Device, _FOFBCtrlBase):
+# ---------------- ref device  ----------------
+
+class FOFBCtrlRef(_Device, FOFBCtrlBase):
     """FOFB reference orbit controller device."""
 
     _properties = (
         'RefOrbX-SP', 'RefOrbX-RB',
         'RefOrbY-SP', 'RefOrbY-RB',
         'MaxOrbDistortion-SP', 'MaxOrbDistortion-RB',
         'MaxOrbDistortionEnbl-Sel', 'MaxOrbDistortionEnbl-Sts',
@@ -37,18 +39,14 @@
         'LoopIntlk-Mon', 'LoopIntlkReset-Cmd',
         'SYSIDPRBSFOFBAccEn-Sel', 'SYSIDPRBSFOFBAccEn-Sts',
         'SYSIDPRBSBPMPosEn-Sel', 'SYSIDPRBSBPMPosEn-Sts',
     )
 
     def __init__(self, devname):
         """Init."""
-        # check if device exists
-        if devname not in self.DEVICES:
-            raise NotImplementedError(devname)
-
         # call base class constructor
         super().__init__(
             devname, properties=FOFBCtrlRef._properties, auto_monitor_mon=True)
 
     @property
     def refx(self):
         """Reference orbit X."""
@@ -140,14 +138,16 @@
 
     def cmd_reset(self):
         """Reset interlocks."""
         self['LoopIntlkReset-Cmd'] = 1
         return True
 
 
+# ---------------- DCC devices ----------------
+
 class _DCCDevice(_ProptyDevice):
     """FOFB Diamond communication controller device."""
 
     DEF_TIMEOUT = 1
     DEF_FMC_BPMCNT = NR_BPM
     DEF_P2P_BPMCNT = 8
 
@@ -211,28 +211,26 @@
         if not self.connected:
             return False
         cnt = self.DEF_FMC_BPMCNT if 'FMC' in self.dccname \
             else self.DEF_P2P_BPMCNT
         return self['BPMCnt-Mon'] == cnt
 
 
-class FOFBCtrlDCC(_DCCDevice, _FOFBCtrlBase):
+class FOFBCtrlDCC(_DCCDevice, FOFBCtrlBase):
     """FOFBCtrl DCC device."""
 
     class PROPDEVICES:
         """DCC devices."""
 
         FMC = 'DCCFMC'
         P2P = 'DCCP2P'
         ALL = (FMC, P2P)
 
     def __init__(self, devname, dccname):
         """Init."""
-        if devname not in self.DEVICES:
-            raise NotImplementedError(devname)
         if dccname not in self.PROPDEVICES.ALL:
             raise NotImplementedError(dccname)
         super().__init__(devname, dccname)
 
     @property
     def linkpartners(self):
         """Return linked partners."""
@@ -243,20 +241,19 @@
 
 
 class BPMDCC(_DCCDevice):
     """BPM DCC device."""
 
     def __init__(self, devname):
         """Init."""
-        # Temporarily remove this check to control new 10SB BPMs
-        # if not _BPMSearch.is_valid_devname(devname):
-        #     raise NotImplementedError(devname)
         super().__init__(devname, 'DCCP2P')
 
 
+# ---------------- Fam devices ----------------
+
 class FamFOFBControllers(_Devices):
     """Family of FOFBCtrl and related BPM devices."""
 
     DEF_TIMEOUT = 10  # [s]
     DEF_DCC_TIMEFRAMELEN = 5000
     DEF_BPMTRIG_RCVSRC = 0
     DEF_BPMTRIG_RCVIN = 5
@@ -275,30 +272,30 @@
         # FOFBCtrl Refs and DCCs
         bpmids = _np.array(
             [self.FOFBCTRL_BPMID_OFFSET - 1 + i for i in range(1, 21)])
         lpcw = _np.roll(bpmids, 1)
         lpaw = _np.roll(bpmids, -1)
         self._ctl_ids, self._ctl_part = dict(), dict()
         self._ctl_refs, self._ctl_dccs = dict(), dict()
-        for idx, ctl in enumerate(_FOFBCtrlBase.DEVICES):
+        for idx, ctl in enumerate(FOFBCtrlBase.DEVICES):
             self._ctl_ids[ctl] = bpmids[idx]
             self._ctl_part[ctl] = {lpcw[idx], lpaw[idx]}
             self._ctl_refs[ctl] = FOFBCtrlRef(ctl)
             for dcc in FOFBCtrlDCC.PROPDEVICES.ALL:
                 self._ctl_dccs[ctl + ':' + dcc] = FOFBCtrlDCC(ctl, dcc)
         # BPM DCCs and triggers
         self._bpmnames = _BPMSearch.get_names({'sec': 'SI', 'dev': 'BPM'})
         bpmids = [((i + 1) // 2) * 2 % 160 for i in range(NR_BPM)]
         self._bpm_dccs, self._bpm_trgs, self._bpm_ids = dict(), dict(), dict()
         for idx, bpm in enumerate(self._bpmnames):
             self._bpm_ids[bpm] = bpmids[idx]
             self._bpm_dccs[bpm] = BPMDCC(bpm)
             for trig in self.BPM_TRIGS_IDS:
                 trigname = bpm + ':TRIGGER' + str(trig)
-                self._bpm_trgs[trigname] = BPMLogicalTrigger(bpm, trig)
+                self._bpm_trgs[trigname] = AFCACQLogicalTrigger(bpm, trig)
         bpm2dsbl = [
             'SI-'+sub+':DI-BPM-'+idx
             for sub in ['06SB', '07SP', '08SB', '09SA', '10SB', '11SP', '12SB']
             for idx in ['1', '2']
         ]
         self._bpmdcc2dsbl = dict()
         for bpm in bpm2dsbl:
@@ -328,15 +325,15 @@
     @property
     def bpmdccdevs(self):
         """BPMDCC device list."""
         return self._bpm_dccs
 
     @property
     def bpmtrigdevs(self):
-        """BPMLogicalTrigger device list."""
+        """AFCACQLogicalTrigger device list."""
         return self._bpm_trgs
 
     @property
     def fofbevtdev(self):
         """FOFBS Event device."""
         return self._evt_fofb
 
@@ -1080,14 +1077,16 @@
                 not isinstance(indices, (list, tuple, _np.ndarray)):
             indices = [indices, ]
         if indices is None:
             indices = [i for i in range(len(self._psnames))]
         return [self._psdevs[i] for i in indices]
 
 
+# ----------------  HL device  ----------------
+
 class HLFOFB(_Device):
     """Control high level FOFB IOC."""
 
     class DEVICES:
         """Devices names."""
 
         SI = 'SI-Glob:AP-FOFB'
```

### Comparing `siriuspy-2.78.0/siriuspy/devices/ict.py` & `siriuspy-2.79.0/siriuspy/devices/ict.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.78.0/siriuspy/devices/idff.py` & `siriuspy-2.79.0/siriuspy/devices/idff.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.78.0/siriuspy/devices/ids.py` & `siriuspy-2.79.0/siriuspy/devices/ids.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.78.0/siriuspy/devices/injctrl.py` & `siriuspy-2.79.0/siriuspy/devices/injctrl.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.78.0/siriuspy/devices/injsys.py` & `siriuspy-2.79.0/siriuspy/devices/injsys.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.78.0/siriuspy/devices/lienergy.py` & `siriuspy-2.79.0/siriuspy/devices/lienergy.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.78.0/siriuspy/devices/lillrf.py` & `siriuspy-2.79.0/siriuspy/devices/lillrf.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.78.0/siriuspy/devices/machshift.py` & `siriuspy-2.79.0/siriuspy/devices/machshift.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.78.0/siriuspy/devices/modltr.py` & `siriuspy-2.79.0/siriuspy/devices/modltr.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.78.0/siriuspy/devices/orbit_interlock.py` & `siriuspy-2.79.0/siriuspy/devices/orbit_interlock.py`

 * *Files 0% similar despite different names*

```diff
@@ -84,14 +84,15 @@
         return cls.__BPM_UPSTREAM
 
     def __init__(self):
         """Init."""
         self._oper = {
             'mean': self._mean,
             'diff': self._diff,
+            'min': min,
         }
 
     @staticmethod
     def get_down_up_bpms(bpmname):
         """Return down and up BPM names for bpmname."""
         index = BaseOrbitIntlk.BPM_NAMES.index(bpmname)
         down = BaseOrbitIntlk.BPM_DOWNSTREAM[index]
```

### Comparing `siriuspy-2.78.0/siriuspy/devices/posang.py` & `siriuspy-2.79.0/siriuspy/devices/posang.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.78.0/siriuspy/devices/psconv.py` & `siriuspy-2.79.0/siriuspy/devices/psconv.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.78.0/siriuspy/devices/pssofb.py` & `siriuspy-2.79.0/siriuspy/devices/pssofb.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.78.0/siriuspy/devices/pstesters.py` & `siriuspy-2.79.0/siriuspy/devices/pstesters.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.78.0/siriuspy/devices/pwrsupply.py` & `siriuspy-2.79.0/siriuspy/devices/pwrsupply.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.78.0/siriuspy/devices/rf.py` & `siriuspy-2.79.0/siriuspy/devices/rf.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.78.0/siriuspy/devices/screen.py` & `siriuspy-2.79.0/siriuspy/devices/screen.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.78.0/siriuspy/devices/sofb.py` & `siriuspy-2.79.0/siriuspy/devices/sofb.py`

 * *Files 7% similar despite different names*

```diff
@@ -38,15 +38,15 @@
 
 
 class TLSOFB(_Device):
     """SOFB Device."""
 
     _properties = (
         'TrigAcqChan-Sel', 'TrigAcqChan-Sts', 'OrbStatus-Mon',
-        'RespMat-SP', 'RespMat-RB', 'InvRespMat-Mon',
+        'RespMat-SP', 'RespMat-RB', 'RespMat-Mon', 'InvRespMat-Mon',
         'KickCH-Mon', 'KickCV-Mon',
         'DeltaKickCH-Mon', 'DeltaKickCV-Mon',
         'DeltaKickCH-SP', 'DeltaKickCV-SP',
         'MaxDeltaKickCH-RB', 'MaxDeltaKickCV-RB',
         'MaxDeltaKickCH-SP', 'MaxDeltaKickCV-SP',
         'ManCorrGainCH-SP', 'ManCorrGainCV-SP',
         'ManCorrGainCH-RB', 'ManCorrGainCV-RB',
@@ -102,25 +102,29 @@
     @trigchannel.setter
     def trigchannel(self, value):
         self._enum_setter(
             'TrigAcqChan-Sel', value, self._data.TrigAcqChan)
 
     @property
     def respmat(self):
-        """."""
+        """Raw response matrix."""
         return self['RespMat-RB'].reshape(self._data.nr_bpms*2, -1)
 
     @respmat.setter
     def respmat(self, mat):
-        """."""
         self['RespMat-SP'] = _np.array(mat).ravel()
 
     @property
+    def respmat_mon(self):
+        """Applied response matrix."""
+        return self['RespMat-Mon'].reshape(self._data.nr_bpms*2, -1)
+
+    @property
     def invrespmat(self):
-        """."""
+        """Inverse response matrix."""
         return self['InvRespMat-Mon'].reshape(-1, self._data.nr_bpms*2)
 
     @property
     def trigchannel_str(self):
         """."""
         return self._data.TrigAcqChan._fields[self['TrigAcqChan-Sts']]
 
@@ -584,14 +588,20 @@
         'DeltaKickRF-Mon', 'DeltaKickRF-SP',
         'MaxDeltaKickRF-RB', 'MaxDeltaKickRF-SP',
         'ManCorrGainRF-SP', 'ManCorrGainRF-RB',
         'MeasRespMatKickRF-SP', 'MeasRespMatKickRF-RB',
         'RFEnbl-Sel', 'RFEnbl-Sts',
         'SlowOrbX-Mon', 'SlowOrbY-Mon',
         'LoopState-Sts', 'LoopState-Sel',
+        'LoopPIDKpCH-SP', 'LoopPIDKiCH-SP', 'LoopPIDKdCH-SP',
+        'LoopPIDKpCH-RB', 'LoopPIDKiCH-RB', 'LoopPIDKdCH-RB',
+        'LoopPIDKpCV-SP', 'LoopPIDKiCV-SP', 'LoopPIDKdCV-SP',
+        'LoopPIDKpCV-RB', 'LoopPIDKiCV-RB', 'LoopPIDKdCV-RB',
+        'LoopPIDKpRF-SP', 'LoopPIDKiRF-SP', 'LoopPIDKdRF-SP',
+        'LoopPIDKpRF-RB', 'LoopPIDKiRF-RB', 'LoopPIDKdRF-RB',
         'DriveFreqDivisor-SP', 'DriveFreqDivisor-RB', 'DriveFrequency-Mon',
         'DriveNrCycles-SP', 'DriveNrCycles-RB', 'DriveDuration-Mon',
         'DriveAmplitude-SP', 'DriveAmplitude-RB',
         'DrivePhase-SP', 'DrivePhase-RB',
         'DriveCorrIndex-SP', 'DriveCorrIndex-RB',
         'DriveBPMIndex-SP', 'DriveBPMIndex-RB',
         'DriveType-Sel', 'DriveType-Sts',
@@ -631,14 +641,95 @@
         ret = self._wait('SOFBMode-Sts', mode, timeout=timeout)
         if not ret:
             return False
         _time.sleep(0.6)  # Status PV updates at 2Hz
         return self.wait_orb_status_ok(timeout=timeout)
 
     @property
+    def loop_pid_ch_kp(self):
+        """Loop PID Kp parameter for CH."""
+        return self['LoopPIDKpCH-RB']
+
+    @loop_pid_ch_kp.setter
+    def loop_pid_ch_kp(self, value):
+        self['LoopPIDKpCH-SP'] = value
+
+    @property
+    def loop_pid_ch_ki(self):
+        """Loop PID Ki parameter for CH."""
+        return self['LoopPIDKiCH-RB']
+
+    @loop_pid_ch_ki.setter
+    def loop_pid_ch_ki(self, value):
+        self['LoopPIDKiCH-SP'] = value
+
+    @property
+    def loop_pid_ch_kd(self):
+        """Loop PID Kd parameter for CH."""
+        return self['LoopPIDKdCH-RB']
+
+    @loop_pid_ch_kd.setter
+    def loop_pid_ch_kd(self, value):
+        self['LoopPIDKdCH-SP'] = value
+
+    @property
+    def loop_pid_cv_kp(self):
+        """Loop PID Kp parameter for CV."""
+        return self['LoopPIDKpCV-RB']
+
+    @loop_pid_cv_kp.setter
+    def loop_pid_cv_kp(self, value):
+        self['LoopPIDKpCV-SP'] = value
+
+    @property
+    def loop_pid_cv_ki(self):
+        """Loop PID Ki parameter for CV."""
+        return self['LoopPIDKiCV-RB']
+
+    @loop_pid_cv_ki.setter
+    def loop_pid_cv_ki(self, value):
+        self['LoopPIDKiCV-SP'] = value
+
+    @property
+    def loop_pid_cv_kd(self):
+        """Loop PID Kd parameter for CV."""
+        return self['LoopPIDKdCV-RB']
+
+    @loop_pid_cv_kd.setter
+    def loop_pid_cv_kd(self, value):
+        self['LoopPIDKdCV-SP'] = value
+
+    @property
+    def loop_pid_rf_kp(self):
+        """Loop PID Kp parameter for RF."""
+        return self['LoopPIDKpRF-RB']
+
+    @loop_pid_rf_kp.setter
+    def loop_pid_rf_kp(self, value):
+        self['LoopPIDKpRF-SP'] = value
+
+    @property
+    def loop_pid_rf_ki(self):
+        """Loop PID Ki parameter for RF."""
+        return self['LoopPIDKiRF-RB']
+
+    @loop_pid_rf_ki.setter
+    def loop_pid_rf_ki(self, value):
+        self['LoopPIDKiRF-SP'] = value
+
+    @property
+    def loop_pid_rf_kd(self):
+        """Loop PID Kd parameter for RF."""
+        return self['LoopPIDKdRF-RB']
+
+    @loop_pid_rf_kd.setter
+    def loop_pid_rf_kd(self, value):
+        self['LoopPIDKdRF-SP'] = value
+
+    @property
     def drivests(self):
         """."""
         return self['DriveState-Sts']
 
     @property
     def drivetype(self):
         """."""
```

### Comparing `siriuspy-2.78.0/siriuspy/devices/syncd.py` & `siriuspy-2.79.0/siriuspy/devices/syncd.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.78.0/siriuspy/devices/timing.py` & `siriuspy-2.79.0/siriuspy/devices/dvf.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,624 +1,637 @@
-"""."""
-import time as _time
+"""DVF devices."""
 
 import numpy as _np
 
 from mathphys.functions import get_namedtuple as _get_namedtuple
+from mathphys.imgproc import Image2D_Fit as _Image2D_Fit
+from mathphys.imgproc import FitGaussianScipy as _FitGaussianScipy
 
-from .device import Device as _Device, ProptyDevice as _ProptyDevice, \
-    Devices as _Devices
-from ..timesys.csdev import ETypes as _ETypes, Const as _TIConst, \
-    get_hl_trigger_database as _get_hl_trigger_database
-from ..search import HLTimeSearch as _HLTimeSearch
-from ..util import get_bit as _get_bit
-
-
-class EVG(_Device):
-    """Device EVG."""
-
-    DEVNAME = 'AS-RaMO:TI-EVG'
-    StateMachine = _get_namedtuple('StateMachine', (
-        'Initializing', 'Stopped', 'Continuous', 'Injection',
-        'Preparing_Continuous', 'Preparing_Injection',
-        'Restarting_Continuous'))
+from .device import DeviceNC as _DeviceNC
+
+
+class DVF(_DeviceNC):
+    """Beam Visualization Device ("Dispositivo de Visualização de Feixe")."""
+
+    class DEVICES:
+        """Devices names."""
+        CAX_DVF1 = 'CAX:A:BASLER01'
+        CAX_DVF2 = 'CAX:B:BASLER01'
+        ALL = (CAX_DVF1, CAX_DVF2)
+
+    _default_timeout = 10  # [s]
+
+    _dvfparam_fields = (
+        'MAX_INTENSITY_NR_BITS',
+        'ACQUISITION_TIME_MIN',  # [s]
+        'ACQUISITION_TIME_DEFAULT',  # [s]
+        'EXPOSURE_TIME_DEFAULT',  # [s]
+        'IMAGE_SIZE_Y',  # [pixel]
+        'IMAGE_SIZE_X',  # [pixel]
+        'IMAGE_PIXEL_SIZE',  # [um]
+        'OPTICS_MAGNIFICATION_FACTOR',  # source to image
+    )
+
+    _dev2params = {
+        DEVICES.CAX_DVF1:
+            _get_namedtuple(
+                'DVFParameters',
+                _dvfparam_fields, (16, 0.5, 0.5, 0.005, 2064, 3088, 2.4, 5.0)),
+        DEVICES.CAX_DVF2:
+            _get_namedtuple(
+                'DVFParameters',
+                _dvfparam_fields, (16, 0.5, 0.5, 0.005, 2064, 3088, 2.4, 5.0)),
+        }
 
     _properties = (
-        'InjectionEvt-Sel', 'InjectionEvt-Sts', 'UpdateEvt-Cmd',
-        'ContinuousEvt-Sel', 'ContinuousEvt-Sts', 'STATEMACHINE',
-        'RepeatBucketList-SP', 'RepeatBucketList-RB',
-        'BucketList-SP', 'BucketList-RB', 'BucketList-Mon',
-        'BucketListLen-Mon', 'TotalInjCount-Mon', 'InjCount-Mon',
-        'BucketListSyncStatus-Mon')
+        'cam1:MaxSizeX_RBV', 'cam1:MaxSizeY_RBV',
+        'cam1:SizeX_RBV', 'cam1:SizeY_RBV',
+        'cam1:Width', 'cam1:Width_RBV',
+        'cam1:Height', 'cam1:Height_RBV',
+        'cam1:OffsetX', 'cam1:OffsetX_RBV',
+        'cam1:OffsetY', 'cam1:OffsetY_RBV',
+        'cam1:CenterX', 'cam1:CenterX_RBV',
+        'cam1:CenterY', 'cam1:CenterY_RBV',
+        'cam1:ArrayCallbacks', 'cam1:ArrayCallbacks_RBV',
+        'cam1:AcquireTime', 'cam1:AcquireTime_RBV',
+        'cam1:AcquirePeriod', 'cam1:AcquirePeriod_RBV',
+        'cam1:Acquire', 'cam1:Acquire_RBV',
+        'cam1:ImageMode', 'cam1:ImageMode_RBV',
+        'cam1:Gain', 'cam1:Gain_RBV',
+        'cam1:GainAuto', 'cam1:GainAuto_RBV',
+        'cam1:DataType', 'cam1:DataType_RBV',
+        'cam1:PixelFormat', 'cam1:PixelFormat_RBV',
+        'cam1:PixelSize', 'cam1:PixelSize_RBV',
+        'cam1:Temperature',
+        'cam1:FAILURES_RBV', 'cam1:COMPLETED_RBV',
+        'image1:NDArrayPort', 'image1:NDArrayPort_RBV',
+        'image1:EnableCallbacks', 'image1:EnableCallbacks_RBV',
+        'image1:ArraySize0_RBV', 'image1:ArraySize1_RBV',
+        'image1:ArrayData',
+        'ROI1:NDArrayPort', 'ROI1:NDArrayPort_RBV',
+        'ROI1:EnableCallbacks', 'ROI1:EnableCallbacks_RBV',
+        'ROI1:MinX', 'ROI1:MinX_RBV',
+        'ROI1:MinY', 'ROI1:MinY_RBV',
+        'ROI1:SizeX', 'ROI1:SizeX_RBV',
+        'ROI1:SizeY', 'ROI1:SizeY_RBV',
+        'ROI1:EnableX', 'ROI1:EnableX_RBV',
+        'ROI1:EnableY', 'ROI1:EnableY_RBV',
+        'ROI1:ArrayCallbacks', 'ROI1:ArrayCallbacks_RBV',
+        'ffmstream1:EnableCallbacks', 'ffmstream1:EnableCallbacks_RBV',
+        'Trans1:EnableCallbacks', 'Trans1:EnableCallbacks_RBV',
+        'HDF1:EnableCallbacks', 'HDF1:EnableCallbacks_RBV',
+        )
 
-    def __init__(self):
-        """."""
-        super().__init__(EVG.DEVNAME, properties=EVG._properties)
+    def __init__(self, devname, *args, **kwargs):
+        """Init."""
+        # check if device exists
+        if devname not in DVF.DEVICES.ALL:
+            raise NotImplementedError(devname)
+        # call base class constructor
+        super().__init__(devname, properties=self._properties, *args, **kwargs)
 
     @property
-    def nrpulses(self):
-        """Number of pulses to repeat Bucket List."""
-        return self['RepeatBucketList-RB']
-
-    @nrpulses.setter
-    def nrpulses(self, value):
-        """Set number of pulses to repeat Bucket List."""
-        self['RepeatBucketList-SP'] = value
+    def parameters(self):
+        """Return DVF parameters."""
+        return DVF._dev2params[self.devname]
 
     @property
-    def bucketlist_len(self):
-        """Bucket List Length."""
-        value = self['BucketListLen-Mon']
-        return int(value) if value is not None else None
+    def intensity_saturation_value(self):
+        """Image intensity saturation value."""
+        pixel_format_to_num_bits = {0: 8, 1: 12}  # 0: 'Mono8, 1: 'Mono12
+        data_type_to_num_bits = {0: 8, 1: 16} # 0: 'UInt8', 1: 'UInt16'
+        used_bits = pixel_format_to_num_bits[self.pixel_format]
+        max_bits = data_type_to_num_bits[self.data_type]
+        max_intensity = (1 << used_bits) - 1
+        if used_bits <= max_bits:
+            # Shift intensity to align with most-significant bits
+            max_intensity <<= max_bits - used_bits
+        elif used_bits > max_bits:
+            # Clip to maximum value allowed by the data type
+            max_intensity = (1 << max_bits) - 1
+        return max_intensity
 
     @property
-    def bucketlist_mon(self):
-        """Implemented Bucket List."""
-        return self['BucketList-Mon'][:self.bucketlist_len]
+    def exposure_time(self):
+        """Camera exposure time [s]."""
+        return self['cam1:AcquireTime']
+
+    @exposure_time.setter
+    def exposure_time(self, value):
+        """Camera exposure time [s]."""
+        value = max(value, 0)
+        self['cam1:AcquireTime'] = value
 
     @property
-    def bucketlist(self):
-        """Last setpoint accepted for Bucket List."""
-        return self['BucketList-RB'][:self.bucketlist_len]
+    def acquisition_time(self):
+        """Camera acquisition time [s]."""
+        return self['cam1:AcquirePeriod']
 
-    @bucketlist.setter
-    def bucketlist(self, value):
-        """Set Bucket List."""
-        self['BucketList-SP'] = _np.array(value, dtype=int)
+    @acquisition_time.setter
+    def acquisition_time(self, value):
+        """Camera acquisition time [s]."""
+        params = self.parameters
+        value = max(value, params.ACQUISITION_TIME_MIN)
+        self['cam1:AcquirePeriod'] = value
 
     @property
-    def bucketlist_sync(self):
-        """Bucket list syncronized status."""
-        return self['BucketListSyncStatus-Mon']
+    def acquisition_status(self):
+        """Return IOC acquisition status."""
+        return self['cam1:Acquire']
 
     @property
-    def continuous_state(self):
-        """."""
-        return bool(self['ContinuousEvt-Sts'])
+    def cam_max_sizex(self):
+        """Camera max second dimension size [pixel]."""
+        return self['cam1:MaxSizeX_RBV']
 
-    @continuous_state.setter
-    def continuous_state(self, value):
-        """."""
-        new_val = bool(value)
-        if self.continuous_state != new_val:
-            self['ContinuousEvt-Sel'] = int(new_val)
+    @property
+    def cam_max_sizey(self):
+        """Camera max first dimension size [pixel]."""
+        return self['cam1:MaxSizeY_RBV']
 
     @property
-    def state_machine(self):
-        """."""
-        return self['STATEMACHINE']
+    def cam_sizex(self):
+        """Camera second dimension size [pixel]."""
+        return self['cam1:SizeX_RBV']
 
     @property
-    def state_machine_str(self):
-        """."""
-        return self.StateMachine._fields[self.state_machine]
+    def cam_sizey(self):
+        """Camera first dimension size [pixel]."""
+        return self['cam1:SizeY_RBV']
 
     @property
-    def injection_state(self):
-        """."""
-        return bool(self['InjectionEvt-Sts'])
+    def cam_width(self):
+        """Camera image X width [pixels]."""
+        # NOTE: the same as cam_sizex
+        return self['cam1:Width_RBV']
 
-    @injection_state.setter
-    def injection_state(self, value):
-        """."""
-        new_val = bool(value)
-        if self.injection_state != new_val:
-            self['InjectionEvt-Sel'] = int(new_val)
+    @cam_width.setter
+    def cam_width(self, value):
+        """Set camera image X width [pixel]."""
+        # NOTE: acquisition has to be turned off and on for
+        # this to take effect on ROI and image1 modules
+        value = int(value)
+        if 0 < value <= self.cam_max_sizex:
+            self['cam1:Width'] = value
+        else:
+            raise ValueError('Invalid width value!')
 
     @property
-    def injection_count_total(self):
-        """."""
-        return self['TotalInjCount-Mon']
+    def cam_height(self):
+        """Camera image Y height [pixels]."""
+        # NOTE: the same as cam_sizey
+        return self['cam1:Height_RBV']
 
-    @property
-    def injection_count(self):
-        """."""
-        return self['InjCount-Mon']
+    @cam_height.setter
+    def cam_height(self, value):
+        """Set camera image Y height [pixel]."""
+        # NOTE: acquisition has to be turned off and on for
+        # this to take effect on ROI and image1 modules
+        value = int(value)
+        if 0 < value <= self.cam_max_sizey:
+            self['cam1:Height'] = value
+        else:
+            raise ValueError('Invalid width value!')
 
-    def fill_bucketlist(self, stop, start=1, step=30, timeout=10):
-        """Fill bucket list."""
-        if (step > 0) and (start > stop):
-            stop += 864
-        if (step < 0) and (stop > start):
-            stop -= 864
-        value = _np.arange(start, stop, step)
-        value = (value-1) % 864 + 1
-        self.bucketlist = value
-        rb_value = _np.zeros(864)
-        rb_value[:len(value)] = value
-        return self._wait('BucketList-RB', rb_value, timeout=timeout)
+    @property
+    def cam_offsetx(self):
+        """Camera image X offset [pixels]."""
+        return self['cam1:OffsetX_RBV']
 
-    def wait_injection_finish(self, timeout=10):
-        """."""
-        return self._wait(propty='InjectionEvt-Sts', value=0, timeout=timeout)
+    @cam_offsetx.setter
+    def cam_offsetx(self, value):
+        """Set camera image X offset [pixel]."""
+        value = int(value)
+        if 0 <= value < self.cam_max_sizex:
+            self['cam1:OffsetX'] = value
+            # NOTE: if offset is invalid, there is, offset + width exceeds
+            # cam image max size, then setpoint is neglected by DVF IOC
+        else:
+            raise ValueError('Invalid offsetx value!')
 
-    def cmd_update_events(self, timeout=10):
-        """."""
-        val = self.continuous_state
-        self['UpdateEvt-Cmd'] = 1
-        _time.sleep(0.1)
-        return self._wait(
-            propty='ContinuousEvt-Sts', value=val, timeout=timeout)
+    @property
+    def cam_offsety(self):
+        """Camera image Y offset [pixels]."""
+        return self['cam1:OffsetY_RBV']
 
-    def cmd_turn_on_injection(self, timeout=10, wait_rb=False):
-        """."""
-        self.injection_state = 1
-        pv2wait = 'InjectionEvt-' + ('Sts' if wait_rb else 'Sel')
-        return self._wait(propty=pv2wait, value=1, timeout=timeout)
+    @cam_offsety.setter
+    def cam_offsety(self, value):
+        """Set camera image Y offset [pixel]."""
+        value = int(value)
+        if 0 <= value < self.cam_max_sizey:
+            self['cam1:OffsetY'] = value
+            # NOTE: if offset is invalid, there is, offset + height exceeds
+            # cam image max size, then setpoint is neglected by DVF IOC
+        else:
+            raise ValueError('Invalid offsety value!')
 
-    def cmd_turn_off_injection(self, timeout=10, wait_rb=False):
+    @property
+    def roi_minx(self):
         """."""
-        self.injection_state = 0
-        pv2wait = 'InjectionEvt-' + ('Sts' if wait_rb else 'Sel')
-        return self._wait(propty=pv2wait, value=0, timeout=timeout)
+        return self['ROI1:MinX_RBV']
 
-    def cmd_turn_on_continuous(self, timeout=10, wait_rb=False):
+    @roi_minx.setter
+    def roi_minx(self, value):
         """."""
-        self.continuous_state = 1
-        pv2wait = 'ContinuousEvt-' + ('Sts' if wait_rb else 'Sel')
-        return self._wait(propty=pv2wait, value=1, timeout=timeout)
+        self['ROI1:MinX'] = int(value)
 
-    def cmd_turn_off_continuous(self, timeout=10, wait_rb=False):
+    @property
+    def roi_miny(self):
         """."""
-        self.continuous_state = 0
-        pv2wait = 'ContinuousEvt-' + ('Sts' if wait_rb else 'Sel')
-        return self._wait(propty=pv2wait, value=0, timeout=timeout)
-
-    def set_nrpulses(self, value, timeout=10):
-        """Set and wait number of pulses."""
-        self['RepeatBucketList-SP'] = value
-        return self._wait('RepeatBucketList-RB', value, timeout=timeout)
-
-
-class Event(_ProptyDevice):
-    """Device Timing Event."""
+        return self['ROI1:MinY_RBV']
 
-    _properties = (
-        'Delay-SP', 'Delay-RB', 'DelayRaw-SP', 'DelayRaw-RB',
-        'DelayType-Sel', 'DelayType-Sts', 'Mode-Sel', 'Mode-Sts',
-        'Code-Mon', 'ExtTrig-Cmd',
-        )
-
-    MODES = _ETypes.EVT_MODES
-    DELAYTYPES = ('Incr', 'Fixed')
-
-    def __init__(self, evtname):
+    @roi_miny.setter
+    def roi_miny(self, value):
         """."""
-        super().__init__(
-            EVG.DEVNAME, evtname, properties=Event._properties)
+        self['ROI1:MinY'] = int(value)
 
     @property
-    def mode(self):
-        """."""
-        return self['Mode-Sts']
-
-    @mode.setter
-    def mode(self, value):
-        self._enum_setter('Mode-Sel', value, Event.MODES)
+    def image_sizex(self):
+        """Image second dimension size [pixel]."""
+        return self['image1:ArraySize0_RBV']
 
     @property
-    def mode_str(self):
-        """."""
-        mode = self['Mode-Sts']
-        if mode is not None:
-            return Event.MODES[mode]
-        return None
+    def image_sizey(self):
+        """Image first dimension size [pixel]."""
+        return self['image1:ArraySize1_RBV']
 
     @property
-    def code(self):
-        """."""
-        return self['Code-Mon']
+    def image(self):
+        """Return DVF image formatted as a (sizey, sizex) numpy matrix."""
+        shape = (self.image_sizey, self.image_sizex)
+        data = self['image1:ArrayData']
+        image = _np.reshape(data, shape)
+        return image
 
     @property
-    def delay_type(self):
-        """."""
-        return self['DelayType-Sts']
+    def image_pixel_size(self):
+        """Image pixel size [um]."""
+        params = self.parameters
+        return params.IMAGE_PIXEL_SIZE
 
-    @delay_type.setter
-    def delay_type(self, value):
-        self._enum_setter('DelayType-Sel', value, Event.DELAYTYPES)
+    @property
+    def optics_magnification_factor(self):
+        """Source to image magnification factor."""
+        params = self.parameters
+        return params.OPTICS_MAGNIFICATION_FACTOR
 
     @property
-    def delay_type_str(self):
-        """."""
-        dlytyp = self['DelayType-Sts']
-        if dlytyp is not None:
-            return Event.DELAYTYPES[dlytyp]
-        return None
+    def conv_pixel_2_srcsize(self):
+        """Pixel to source size convertion factor."""
+        pixel_size = self.image_pixel_size
+        mag_factor = self.optics_magnefication_factor
+        pixel2srcsize = pixel_size / mag_factor
+        return pixel2srcsize
 
     @property
-    def delay(self):
-        """."""
-        return self['Delay-RB']
+    def gain(self):
+        """Return camera gain."""
+        return self['cam1:Gain_RBV']
 
-    @delay.setter
-    def delay(self, value):
-        self['Delay-SP'] = value
+    @gain.setter
+    def gain(self, value):
+        """Set camera gain."""
+        self['cam1:Gain'] = value
 
     @property
-    def delay_raw(self):
-        """."""
-        return self['DelayRaw-RB']
-
-    @delay_raw.setter
-    def delay_raw(self, value):
-        self['DelayRaw-SP'] = int(value)
+    def gain_auto(self):
+        """Return camera gain auto."""
+        return self['cam1:GainAuto_RBV']
 
-    def cmd_external_trigger(self):
-        """."""
-        self['ExtTrig-Cmd'] = 1
-        return True
+    @gain.setter
+    def gain_auto(self, value):
+        """Set camera gain auto."""
+        self['cam1:GainAuto'] = value
 
     @property
-    def is_in_inj_table(self):
-        """."""
-        return self.mode_str in Event.MODES[1:4]
+    def pixel_format(self):
+        """Return camera pixel format."""
+        return self['cam1:PixelFormat_RBV']
 
+    @pixel_format.setter
+    def pixel_format(self, value):
+        """Set camera pixel format."""
+        self['cam1:PixelFormat'] = value
 
-class Trigger(_Device):
-    """Device trigger."""
+    @property
+    def data_type(self):
+        """Return camera data type."""
+        return self['cam1:DataType_RBV']
 
-    STATES = ('Dsbl', 'Enbl')
-    LOCKLL = ('Unlocked', 'Locked')
-    POLARITIES = ('Normal', 'Inverse')
+    @data_type.setter
+    def data_type(self, value):
+        """Set camera data type."""
+        self['cam1:DataType'] = value
 
-    def __init__(self, trigname):
-        """Init."""
-        self._database = _get_hl_trigger_database(trigname)
-        self._properties = tuple(self._database)
-        self._source_options = self._database['Src-Sel']['enums']
-        super().__init__(trigname, properties=self._properties)
+    @property
+    def pixel_size(self):
+        """Return camera pixel size."""
+        return self['cam1:PixelSize_RBV']
+
+    @pixel_size.setter
+    def pixel_size(self, value):
+        """Set camera pixel size."""
+        self['cam1:PixelSize'] = value
 
     @property
-    def status(self):
-        """Status."""
-        return self['Status-Mon']
+    def cam_temperature(self):
+        """Return camera temperature"""
+        return self['cam1:Temperature']
 
     @property
-    def status_str(self):
-        """Status string."""
-        value = self.status
-        strs = [d for i, d in enumerate(_TIConst.HLTrigStatusLabels)
-                if _get_bit(value, i)]
-        return ', '.join(strs) if strs else 'Ok'
+    def cam_frames_completed(self):
+        """Return number of acquisition frames completed."""
+        return self['cam1:COMPLETED_RBV']
 
     @property
-    def status_labels(self):
-        """Return Status labels of trigger.
+    def cam_frames_failures(self):
+        """Return number of acquisition frames failures."""
+        return self['cam1:FAILURES_RBV']
 
-        Returns:
-            list: labels describing the possible statuses of the trigger.
+    def cmd_reset(self, timeout=None):
+        """Reset DVF to a standard configuration."""
+        props_values = {
+            'cam1:ArrayCallbacks': 1,  # Enable passing array
+            'cam1:ImageMode': 2,  # Continuous
+            'cam1:PixelFormat': 1,  # Mono12
+            'cam1:DataType': 1,  # UInt16 (maybe unnecessary)
+            'ROI1:NDArrayPort': 'CAMPORT',  # Take img from camport
+            'ROI1:EnableCallbacks': 1,  # Enable getting from NDArrayPort
+            'ROI1:MinX': 0,  # [pixel]
+            'ROI1:MinY': 0,  # [pixel]
+            'ROI1:SizeX': self.cam_max_sizex,  # [pixel]
+            'ROI1:SizeY': self.cam_max_sizey,  # [pixel]
+            'ROI1:EnableX': 1,  # Enable
+            'ROI1:EnableY': 1,  # Enable
+            'ROI1:ArrayCallbacks': 1,  # Enable passing array
+            'image1:NDArrayPort': 'ROI1',  # image1 takes img from ROI1
+            'image1:EnableCallbacks': 1,  # Enable
+            'ffmstream1:EnableCallbacks': 0,  # Disable
+            'HDF1:EnableCallbacks': 0,  # Disable
+            'Trans1:EnableCallbacks': 0,  # Disable
+        }
 
-        """
-        pvo = self.pv_object('StatusLabels-Cte')
-        return pvo.get(as_string=True).split('\n')
+        # set properties
+        for propty, value in props_values.items():
+            self[propty] = value
 
-    @property
-    def state(self):
-        """State."""
-        return self['State-Sts']
+        # check readback values
+        for propty, value in props_values.items():
+            if not self._wait(propty + '_RBV', value, timeout=timeout):
+                return False
 
-    @state.setter
-    def state(self, value):
-        self._enum_setter('State-Sel', value, Trigger.STATES)
+        # configure image acquisition parameters
+        params = self.parameters
+        self.exposure_time = params.EXPOSURE_TIME_DEFAULT
+        self.acquisition_time = params.ACQUISITION_TIME_DEFAULT
+        return True
 
-    @property
-    def state_str(self):
-        """State string."""
-        return Trigger.STATES[self['State-Sts']]
+    def cmd_acquire_on(self, timeout=None):
+        """Tune IOC image acquisition on."""
+        return self._set_and_wait('cam1:Acquire', 1, timeout=timeout)
 
-    @property
-    def lock_low_level(self):
-        """Lock low level status."""
-        return self['LowLvlLock-Sts']
+    def cmd_acquire_off(self, timeout=None):
+        """Tune IOC image acquisition off."""
+        return self._set_and_wait('cam1:Acquire', 0, timeout=timeout)
 
-    @lock_low_level.setter
-    def lock_low_level(self, value):
-        self._enum_setter('LowLvlLock-Sel', value, Trigger.LOCKLL)
+    def cmd_set_cam_roi(self, offsetx, offsety, width, height, timeout=None):
+        """Set cam image region of interest and reset aquisition."""
+        self.cmd_acquire_off(timeout=timeout)
+        self.cam_offsetx = offsetx
+        self.cam_offsety = offsety
+        self.cam_width = width
+        self.cam_height = height
+        self.cmd_acquire_on(timeout=timeout)
 
-    @property
-    def lock_low_level_str(self):
-        """Lock low level status string."""
-        return Trigger.LOCKLL[self['LowLvlLock-Sts']]
+    @staticmethod
+    def conv_devname2parameters(devname):
+        """."""
+        return DVF._dev2params[devname]
 
-    @property
-    def controlled_channels(self):
-        """Return channels controlled by this trigger.
+    def _set_and_wait(self, propty, value, timeout=None):
+        """."""
+        timeout = timeout or self._default_timeout
+        self[propty] = value
+        return self._wait(propty + '_RBV', value, timeout=timeout)
 
-        Returns:
-            list: names of the controlled channels.
 
-        """
-        pvo = self.pv_object('CtrldChannels-Cte')
-        return pvo.get(as_string=True).split('\n')
+class DVFImgProc(DVF):
+    """."""
 
-    @property
-    def low_level_triggers(self):
-        """Return low level triggers controlled by this trigger.
+    _properties = DVF._properties + (
+        'ImgIntensityMax-Mon', 'ImgIntensityMin-Mon',
+        'ImgIntensitySum-Mon', 'ImgIsSaturated-Mon',
+        'ImgIsWithBeam-Mon',
+        'ImgIsWithBeamThreshold-SP', 'ImgIsWithBeamThreshold-RB',
+
+        'ImgROIX-RB', 'ImgROIX-SP',
+        'ImgROIXCenter-Mon', 'ImgROIXFWHM-Mon',
+        'ImgROIY-RB', 'ImgROIY-SP',
+        'ImgROIYCenter-Mon', 'ImgROIYFWHM-Mon',
+
+        'ImgLog-Mon',
+        'ImgROIUpdateWithFWHM-Sel', 'ImgROIUpdateWithFWHM-Sts',
+        'ImgROIYUpdateWithFWHMFactor-RB', 'ImgROIYUpdateWithFWHMFactor-SP',
+        'ImgROIXUpdateWithFWHMFactor-RB', 'ImgROIXUpdateWithFWHMFactor-SP',
+
+        'ImgROIXFitMean-Mon', 'ImgROIXFitSigma-Mon',
+        'ImgROIXFitAmplitude-Mon', 'ImgROIXFitError-Mon',
+        'ImgROIYFitMean-Mon', 'ImgROIYFitSigma-Mon',
+        'ImgROIYFitAmplitude-Mon', 'ImgROIYFitError-Mon',
+        'ImgFitAngle-Mon',
+        'ImgFitSigma1-Mon', 'ImgFitSigma2-Mon',
+        'ImgFitProcTime-Mon',
+        'ImgFitAngleUseCMomSVD-Sel', 'ImgFitAngleUseCMomSVD-Sts',
+        'ImgDVFStatus-Mon', 'ImgDVFStatusLabels-Cte',
+        )
 
-        Returns:
-            list: names of the controlled low level triggers.
+    def __init__(self, devname, *args, **kwargs):
+        """."""
+        super().__init__(devname=devname, *args, **kwargs)
+        self._fitgaussian = _FitGaussianScipy()
 
-        """
-        pvo = self.pv_object('LowLvlTriggers-Cte')
-        return pvo.get(as_string=True).split('\n')
+    @property
+    def intensity_min(self):
+        """Image min intensity."""
+        return self['ImgIntensityMin-Mon']
 
     @property
-    def source(self):
-        """Source."""
-        return self['Src-Sts']
+    def intensity_max(self):
+        """Image max intensity."""
+        return self['ImgIntensityMax-Mon']
 
-    @source.setter
-    def source(self, value):
-        self._enum_setter('Src-Sel', value, self._source_options)
+    @property
+    def intensity_sum(self):
+        """Image sum intensity."""
+        return self['ImgIntensitySum-Mon']
 
     @property
-    def source_str(self):
-        """Source string."""
-        if self['Src-Sts'] is not None:
-            return self._source_options[self['Src-Sts']]
-        return
+    def is_saturated(self):
+        """Whether image is saturated."""
+        return self['ImgIsSaturated-Mon']
 
     @property
-    def source_options(self):
-        """Source options."""
-        return self._source_options
+    def is_with_beam(self):
+        """Whether image is with beam."""
+        return self['ImgIsWithBeam-Mon']
 
     @property
-    def duration(self):
-        """Duration."""
-        return self['Duration-RB']
+    def is_with_beam_threashold(self):
+        """Get image is with beam threashold."""
+        return self['ImgIsWithBeamThreshold-RB']
 
-    @duration.setter
-    def duration(self, value):
-        self['Duration-SP'] = value
+    @is_with_beam_threashold.setter
+    def is_with_beam_threashold(self, value):
+        """Set image is with beam threashold."""
+        self['ImgIsWithBeamThreshold-SP'] = value
 
     @property
-    def width_raw(self):
-        """Width of one pulse in hardware units."""
-        return self['WidthRaw-RB']
+    def roiy(self):
+        """."""
+        return self['ImgROIY-RB']
 
-    @width_raw.setter
-    def width_raw(self, value):
-        self['WidthRaw-SP'] = value
+    @roiy.setter
+    def roiy(self, value):
+        """."""
+        self['ImgROIY-SP'] = value
 
     @property
-    def polarity(self):
-        """Polarity."""
-        return self['Polarity-Sts']
+    def roix(self):
+        """."""
+        return self['ImgROIX-RB']
 
-    @polarity.setter
-    def polarity(self, value):
-        self._enum_setter('Polarity-Sel', value, Trigger.POLARITIES)
+    @roix.setter
+    def roix(self, value):
+        """."""
+        self['ImgROIX-SP'] = value
 
     @property
-    def polarity_str(self):
-        """Polarity string."""
-        return Trigger.POLARITIES[self['Polarity-Sts']]
+    def roiy_center(self):
+        """."""
+        return self['ImgROIYCenter-Mon']
 
     @property
-    def nr_pulses(self):
-        """Nr. of pulses."""
-        return self['NrPulses-RB']
-
-    @nr_pulses.setter
-    def nr_pulses(self, value):
-        self['NrPulses-SP'] = value
+    def roix_center(self):
+        """."""
+        return self['ImgROIXCenter-Mon']
 
     @property
-    def delay(self):
-        """Delay."""
-        return self['Delay-RB']
-
-    @delay.setter
-    def delay(self, value):
-        self['Delay-SP'] = value
+    def roiy_fwhm(self):
+        """."""
+        return self['ImgROIYFWHM-Mon']
 
     @property
-    def total_delay(self):
-        """Total delay."""
-        return self['TotalDelay-Mon']
+    def roix_fwhm(self):
+        """."""
+        return self['ImgROIXFWHM-Mon']
 
     @property
-    def delta_delay(self):
-        """Return delta delay array.
-
-        Returns:
-            numpy.ndarray: delta delays.
-
-        """
-        return self['DeltaDelay-RB']
-
-    @delta_delay.setter
-    def delta_delay(self, value):
-        if not isinstance(value, (_np.ndarray, list, tuple)):
-            raise TypeError('Value must be a numpy.ndarray, list or tuple.')
+    def roiy_fit_amplitude(self):
+        """."""
+        return self['ImgROIYFitAmplitude-Mon']
 
-        value = _np.array(value)
-        size = self.delta_delay.size
-        if value.size != size:
-            raise TypeError(f'Size of value must be {size:d}.')
-        self['DeltaDelay-SP'] = value
+    @property
+    def roix_fit_amplitude(self):
+        """."""
+        return self['ImgROIXFitAmplitude-Mon']
 
     @property
-    def delay_raw(self):
-        """Delay raw."""
-        return self['DelayRaw-RB']
+    def roiy_fit_mean(self):
+        """."""
+        return self['ImgROIYFitMean-Mon']
 
-    @delay_raw.setter
-    def delay_raw(self, value):
-        self['DelayRaw-SP'] = value
+    @property
+    def roix_fit_mean(self):
+        """."""
+        return self['ImgROIXFitMean-Mon']
 
     @property
-    def total_delay_raw(self):
-        """Total delay raw."""
-        return self['TotalDelayRaw-Mon']
+    def roiy_fit_sigma(self):
+        """."""
+        return self['ImgROIYFitSigma-Mon']
 
     @property
-    def delta_delay_raw(self):
-        """Return delta delay raw array.
+    def roix_fit_sigma(self):
+        """."""
+        return self['ImgROIXFitSigma-Mon']
 
-        Returns:
-            numpy.ndarray: delta delays raw.
+    @property
+    def roiy_fit_error(self):
+        """."""
+        return self['ImgROIYFitError-Mon']
 
-        """
-        return self['DeltaDelayRaw-RB']
+    @property
+    def roix_fit_error(self):
+        """."""
+        return self['ImgROIXFitError-Mon']
 
-    @delta_delay_raw.setter
-    def delta_delay_raw(self, value):
-        if not isinstance(value, (_np.ndarray, list, tuple)):
-            raise TypeError('Value must be a numpy.ndarray, list or tuple.')
+    @property
+    def roiy_fwhm_factor(self):
+        """."""
+        return self['ImgROIYUpdateWithFWHMFactor-RB']
 
-        value = _np.array(value)
-        size = self.delta_delay_raw.size
-        if value.size != size:
-            raise TypeError(f'Size of value must be {size:d}.')
-        self['DeltaDelayRaw-SP'] = value
+    @roiy_fwhm_factor.setter
+    def roiy_fwhm_factor(self, value):
+        """."""
+        self['ImgROIYUpdateWithFWHMFactor-SP'] = value
 
     @property
-    def is_in_inj_table(self):
-        """Is in Injection table."""
-        return self['InInjTable-Mon']
+    def roix_fwhm_factor(self):
+        """."""
+        return self['ImgROIXUpdateWithFWHMFactor-RB']
 
-    def cmd_enable(self, timeout=3):
-        """Command enable."""
-        self.state = 1
-        return self._wait('State-Sts', 1, timeout)
+    @roix_fwhm_factor.setter
+    def roix_fwhm_factor(self, value):
+        """."""
+        self['ImgROIXUpdateWithFWHMFactor-SP'] = value
 
-    def cmd_disable(self, timeout=3):
-        """Command disable."""
-        self.state = 0
-        return self._wait('State-Sts', 0, timeout)
+    @property
+    def roi_update_with_fwhm(self):
+        """."""
+        return bool(self['ImgROIUpdateWithFWHM-Sts'])
 
-    def cmd_lock_low_level(self, timeout=3):
-        """Lock low level IOCs state."""
-        self.lock_low_level = 1
-        return self._wait('LowLvlLock-Sts', 1, timeout)
+    @roi_update_with_fwhm.setter
+    def roi_update_with_fwhm(self, value):
+        """."""
+        self['ImgROIUpdateWithFWHM-Sel'] = bool(value)
 
-    def cmd_unlock_low_level(self, timeout=3):
-        """Unlock low level IOCs state."""
-        self.lock_low_level = 0
-        return self._wait('LowLvlLock-Sts', 0, timeout)
+    @property
+    def fit_angle(self):
+        """."""
+        return self['ImgFitAngle-Mon']
 
+    @property
+    def fit_sigma1(self):
+        """."""
+        return self['ImgFitSigma1-Mon']
 
-class HLTiming(_Devices):
-    """."""
+    @property
+    def fit_sigma2(self):
+        """."""
+        return self['ImgFitSigma2-Mon']
 
-    SEARCH = _HLTimeSearch
+    @property
+    def fit_proctime(self):
+        """Return image processing time [ms]."""
+        return self['ImgFitProcTime-Mon']
 
-    def __init__(self):
+    @property
+    def fit_angle_use_cmom_svd(self):
         """."""
-        self.evg = EVG()
-        evs = self.SEARCH.get_configurable_hl_events()
-        self.events = {ev: Event(ev) for ev in evs.keys()}
-        self.triggers = {t: Trigger(t) for t in self.SEARCH.get_hl_triggers()}
-        devs = [self.evg, ]
-        devs += list(self.events.values())
-        devs += list(self.triggers.values())
-        super().__init__('AS-Glob:TI-HLTiming', devs)
-
-    def get_mapping_events2triggers(self) -> dict:
-        """."""
-        map_ = {tn: tr.source_str for tn, tr in self.triggers.items()}
-        inv_map = {ev: list() for ev in set(map_.values())}
-        for tn, ev in map_.items():
-            inv_map[ev].append(tn)
-        return inv_map
-
-    def get_mapping_injtable2events(self) -> dict:
-        """."""
-        map_evt2table = {n: o.mode_str for n, o in self.events.items()}
-        map_table2evt = {}
-        for k, v in map_evt2table.items():
-            map_table2evt[v] = map_table2evt.get(v, []) + [k]
-        return map_table2evt
-
-    def change_triggers_source(
-            self, trigs, new_src='Linac', printlog=True) -> list:
-        """."""
-        notchanged = list()
-        for tn in trigs:
-            tr = self.triggers[tn]
-
-            if new_src not in tr.source_options:
-                if printlog:
-                    print(
-                        f'{tn:25s} -> No Change: {new_src:s}'
-                        ' is not an option.')
-                notchanged.append(tn)
-                continue
-
-            dly_newsrc = 0
-            if new_src in self.events:
-                dly_newsrc = self.events[new_src].delay_raw
-
-            dly_oldsrc = 0
-            old_src = tr.source_str
-            if old_src in self.events:
-                dly_oldsrc = self.events[old_src].delay_raw
-
-            dly = tr.delay_raw
-            delta_dly = dly_oldsrc
-            delta_dly -= dly_newsrc
-            dly += delta_dly
-            if dly < 0:
-                notchanged.append(tn)
-                if printlog:
-                    print(f'{tn:25s} -> No Change: total delay not constant!')
-                continue
-
-            tr.delay_raw = dly
-            tr.source = new_src
-            if printlog:
-                print(f'{tn:25s} -> Change OK: .')
-        return notchanged
-
-    def change_event_delay(self, new_dly, event='Linac', printlog=True):
-        """."""
-        if event not in self.events:
-            if printlog:
-                print(f'{event} is not a valid event!')
-            return False
-        new_dly = int(new_dly)
-        old_dly = self.events[event].delay_raw
-        dlt_dly = old_dly - new_dly
-
-        trigs = self.get_mapping_events2triggers()[event]
-        for trn in trigs:
-            dly = self.triggers[trn].delay_raw + dlt_dly
-            if dly < 0:
-                if printlog:
-                    print(f'cannot change delay: {trn:s} would change!')
-                return False
+        return self['ImgFitAngleUseCMomSVD-Sts']
 
-        for trn in trigs:
-            self.triggers[trn].delay_raw += dlt_dly
-        self.events[event].delay_raw = new_dly
-        if printlog:
-            print('Delay changed!')
-        return True
+    @fit_angle_use_cmom_svd.setter
+    def fit_angle_use_cmom_svd(self, value):
+        """."""
+        self['ImgFitAngleUseCMomSVD-Sel'] = bool(value)
 
-    def print_injtable_mapping(self, only_enabled=False):
+    @property
+    def log(self):
         """."""
-        map_evt2trig = self.get_mapping_events2triggers()
-        map_table2evt = self.get_mapping_injtable2events()
-        tabs = {'Continuous', 'Injection', 'OneShot'}
-        tabs &= map_table2evt.keys()
-        tabs = sorted(tabs)
-
-        dlys = []
-        for tab in tabs:
-            for evt in map_table2evt[tab]:
-                for name in map_evt2trig.get(evt, []):
-                    obj = self.triggers[name]
-                    if only_enabled and not obj.enabled:
-                        continue
-                    dlys.append([obj.total_delay, name, evt, tab])
-        dlys = sorted(dlys)
-
-        tmpl = ' {:^30s} |' * len(tabs)
-        print(('{:^12s} |' + tmpl).format('Delay [ms]', *tabs))
-        print('-'*(12+33*len(tabs) + 2))
-        for dly, trg, evt, tab in dlys:
-            stgs = [''] * len(tabs)
-            stgs[tabs.index(tab)] = trg
-            print(('{:>12.6f} |' + tmpl).format(dly/1e3, *stgs))
+        return self['ImgLog-Mon']
+
+    def create_image2dfit(self):
+        """Return a Image2DFit object with current image as data."""
+        imgfit2d = _Image2D_Fit(
+            data=self.image, fitgauss=self._fitgaussian,
+            roix=self.roix, roiy=self.roiy)
+        return imgfit2d
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `siriuspy-2.78.0/siriuspy/devices/tune.py` & `siriuspy-2.79.0/siriuspy/devices/tune.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.78.0/siriuspy/diagbeam/bpm/csdev.py` & `siriuspy-2.79.0/siriuspy/diagbeam/bpm/csdev.py`

 * *Files 1% similar despite different names*

```diff
@@ -293,18 +293,18 @@
         """."""
         dbase = {
             'MonitEnable-Sel': {
                 'type': 'enum', 'enums': Const.MonitEnbl._fields, 'value': 3},
             'MonitEnable-Sts': {
                 'type': 'enum', 'enums': Const.MonitEnbl._fields, 'value': 3},
             'MONITUpdtTime-SP': {
-                'type': 'float', 'value': 0, 'low': 0.05, 'high': 1.0,
+                'type': 'float', 'value': 0, 'low': 0.001, 'high': 1.0,
                 'unit': 's'},
             'MONITUpdtTime-RB': {
-                'type': 'float', 'value': 0, 'low': 0.05, 'high': 1.0,
+                'type': 'float', 'value': 0, 'low': 0.001, 'high': 1.0,
                 'unit': 's'},
             }
         return {prefix + k: v for k, v in dbase.items()}
 
     @staticmethod
     def get_offsets_database(prefix=''):
         """."""
```

### Comparing `siriuspy-2.78.0/siriuspy/diagbeam/dcct/csdev.py` & `siriuspy-2.79.0/siriuspy/diagbeam/dcct/csdev.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.78.0/siriuspy/diagbeam/ict/csdev.py` & `siriuspy-2.79.0/siriuspy/diagbeam/ict/csdev.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.78.0/siriuspy/diagbeam/screen/csdev.py` & `siriuspy-2.79.0/siriuspy/diagbeam/screen/csdev.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.78.0/siriuspy/diagbeam/slit/csdev.py` & `siriuspy-2.79.0/siriuspy/diagbeam/slit/csdev.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.78.0/siriuspy/diagsys/app.py` & `siriuspy-2.79.0/siriuspy/diagsys/app.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.78.0/siriuspy/diagsys/lidiag/csdev.py` & `siriuspy-2.79.0/siriuspy/diagsys/lidiag/csdev.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.78.0/siriuspy/diagsys/lidiag/main.py` & `siriuspy-2.79.0/siriuspy/diagsys/lidiag/main.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.78.0/siriuspy/diagsys/lidiag/pvs.py` & `siriuspy-2.79.0/siriuspy/diagsys/lidiag/pvs.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.78.0/siriuspy/diagsys/psdiag/csdev.py` & `siriuspy-2.79.0/siriuspy/diagsys/psdiag/csdev.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.78.0/siriuspy/diagsys/psdiag/main.py` & `siriuspy-2.79.0/siriuspy/diagsys/psdiag/main.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.78.0/siriuspy/diagsys/psdiag/pvs.py` & `siriuspy-2.79.0/siriuspy/diagsys/psdiag/pvs.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.78.0/siriuspy/diagsys/pudiag/csdev.py` & `siriuspy-2.79.0/siriuspy/diagsys/pudiag/csdev.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.78.0/siriuspy/diagsys/pudiag/main.py` & `siriuspy-2.79.0/siriuspy/diagsys/pudiag/main.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.78.0/siriuspy/diagsys/pudiag/pvs.py` & `siriuspy-2.79.0/siriuspy/diagsys/pudiag/pvs.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.78.0/siriuspy/diagsys/pvs.py` & `siriuspy-2.79.0/siriuspy/diagsys/pvs.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.78.0/siriuspy/diagsys/rfdiag/csdev.py` & `siriuspy-2.79.0/siriuspy/diagsys/rfdiag/csdev.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.78.0/siriuspy/diagsys/rfdiag/main.py` & `siriuspy-2.79.0/siriuspy/diagsys/rfdiag/main.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.78.0/siriuspy/diagsys/rfdiag/pvs.py` & `siriuspy-2.79.0/siriuspy/diagsys/rfdiag/pvs.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.78.0/siriuspy/dvfimgproc/csdev.py` & `siriuspy-2.79.0/siriuspy/dvfimgproc/csdev.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.78.0/siriuspy/dvfimgproc/main.py` & `siriuspy-2.79.0/siriuspy/dvfimgproc/main.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.78.0/siriuspy/dvfimgproc/meas.py` & `siriuspy-2.79.0/siriuspy/dvfimgproc/meas.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.78.0/siriuspy/envars.py` & `siriuspy-2.79.0/siriuspy/envars.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.78.0/siriuspy/epics/multiproc.py` & `siriuspy-2.79.0/siriuspy/epics/multiproc.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.78.0/siriuspy/epics/properties.py` & `siriuspy-2.79.0/siriuspy/epics/properties.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.78.0/siriuspy/epics/pv_fake.py` & `siriuspy-2.79.0/siriuspy/epics/pv_fake.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.78.0/siriuspy/epics/pv_time_serie.py` & `siriuspy-2.79.0/siriuspy/epics/pv_time_serie.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.78.0/siriuspy/fofb/csdev.py` & `siriuspy-2.79.0/siriuspy/fofb/csdev.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.78.0/siriuspy/fofb/main.py` & `siriuspy-2.79.0/siriuspy/fofb/main.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.78.0/siriuspy/idff/config.py` & `siriuspy-2.79.0/siriuspy/idff/config.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.78.0/siriuspy/idff/csdev.py` & `siriuspy-2.79.0/siriuspy/idff/csdev.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.78.0/siriuspy/idff/main.py` & `siriuspy-2.79.0/siriuspy/idff/main.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.78.0/siriuspy/injctrl/bias_feedback.py` & `siriuspy-2.79.0/siriuspy/injctrl/bias_feedback.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.78.0/siriuspy/injctrl/csdev.py` & `siriuspy-2.79.0/siriuspy/injctrl/csdev.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.78.0/siriuspy/injctrl/main.py` & `siriuspy-2.79.0/siriuspy/injctrl/main.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.78.0/siriuspy/machshift/csdev.py` & `siriuspy-2.79.0/siriuspy/machshift/csdev.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.78.0/siriuspy/machshift/gensumm_macreport.py` & `siriuspy-2.79.0/siriuspy/machshift/gensumm_macreport.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.78.0/siriuspy/machshift/macreport.py` & `siriuspy-2.79.0/siriuspy/machshift/macreport.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.78.0/siriuspy/machshift/macschedule.py` & `siriuspy-2.79.0/siriuspy/machshift/macschedule.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.78.0/siriuspy/machshift/main.py` & `siriuspy-2.79.0/siriuspy/machshift/main.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.78.0/siriuspy/machshift/savedata_macreport.py` & `siriuspy-2.79.0/siriuspy/machshift/savedata_macreport.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.78.0/siriuspy/machshift/utils.py` & `siriuspy-2.79.0/siriuspy/machshift/utils.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.78.0/siriuspy/magnet/data.py` & `siriuspy-2.79.0/siriuspy/magnet/data.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.78.0/siriuspy/magnet/excdata.py` & `siriuspy-2.79.0/siriuspy/magnet/excdata.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.78.0/siriuspy/magnet/factory.py` & `siriuspy-2.79.0/siriuspy/magnet/factory.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.78.0/siriuspy/magnet/normalizer.py` & `siriuspy-2.79.0/siriuspy/magnet/normalizer.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.78.0/siriuspy/magnet/util.py` & `siriuspy-2.79.0/siriuspy/magnet/util.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.78.0/siriuspy/meas/csdev.py` & `siriuspy-2.79.0/siriuspy/meas/csdev.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.78.0/siriuspy/meas/liemit/csdev.py` & `siriuspy-2.79.0/siriuspy/meas/liemit/csdev.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.78.0/siriuspy/meas/liemit/main.py` & `siriuspy-2.79.0/siriuspy/meas/liemit/main.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.78.0/siriuspy/meas/lienergy/csdev.py` & `siriuspy-2.79.0/siriuspy/meas/lienergy/csdev.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.78.0/siriuspy/meas/lienergy/main.py` & `siriuspy-2.79.0/siriuspy/meas/lienergy/main.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.78.0/siriuspy/meas/util.py` & `siriuspy-2.79.0/siriuspy/meas/util.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.78.0/siriuspy/namesys/implementation.py` & `siriuspy-2.79.0/siriuspy/namesys/implementation.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.78.0/siriuspy/optics/lattice_survey.py` & `siriuspy-2.79.0/siriuspy/optics/lattice_survey.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.78.0/siriuspy/opticscorr/base.py` & `siriuspy-2.79.0/siriuspy/opticscorr/base.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.78.0/siriuspy/opticscorr/chrom.py` & `siriuspy-2.79.0/siriuspy/opticscorr/chrom.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.78.0/siriuspy/opticscorr/csdev.py` & `siriuspy-2.79.0/siriuspy/opticscorr/csdev.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.78.0/siriuspy/opticscorr/opticscorr.py` & `siriuspy-2.79.0/siriuspy/opticscorr/opticscorr.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.78.0/siriuspy/opticscorr/tune.py` & `siriuspy-2.79.0/siriuspy/opticscorr/tune.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.78.0/siriuspy/opticscorr/utils.py` & `siriuspy-2.79.0/siriuspy/opticscorr/utils.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.78.0/siriuspy/oscilloscope/keysight.py` & `siriuspy-2.79.0/siriuspy/oscilloscope/keysight.py`

 * *Files 1% similar despite different names*

```diff
@@ -127,14 +127,15 @@
         self.send_command(b":RUN\n", get_res=False)
         while len(dataraw) < datanum:
             dataraw = dataraw + self._socket.recv(datanum)
         dataraw = dataraw[0:-1]  # remove EOF char
 
         va1 = _np.array(list(dataraw)[0::2])
         va0 = _np.array(list(dataraw)[1::2])
+        va1 = va1[:va0.size]
 
         datay = ((va1 << 8) + va0 - 2**16*(va1 >> 7)) * yinc + yor
 
         datax = _np.arange(datay.size)*xinc
         return datax, datay, srate, bdw
 
     def wfm_get_data(self, channel=None, wait_trigger=False):
```

### Comparing `siriuspy-2.78.0/siriuspy/oscilloscope/scopes.py` & `siriuspy-2.79.0/siriuspy/oscilloscope/scopes.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.78.0/siriuspy/posang/csdev.py` & `siriuspy-2.79.0/siriuspy/posang/csdev.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.78.0/siriuspy/posang/main.py` & `siriuspy-2.79.0/siriuspy/posang/main.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.78.0/siriuspy/posang/utils.py` & `siriuspy-2.79.0/siriuspy/posang/utils.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.78.0/siriuspy/pwrsupply/beaglebone.py` & `siriuspy-2.79.0/siriuspy/pwrsupply/beaglebone.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.78.0/siriuspy/pwrsupply/bsmp/commands.py` & `siriuspy-2.79.0/siriuspy/pwrsupply/bsmp/commands.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.78.0/siriuspy/pwrsupply/bsmp/constants.py` & `siriuspy-2.79.0/siriuspy/pwrsupply/bsmp/constants.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.78.0/siriuspy/pwrsupply/bsmp/entities.py` & `siriuspy-2.79.0/siriuspy/pwrsupply/bsmp/entities.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.78.0/siriuspy/pwrsupply/bsmp/factory.py` & `siriuspy-2.79.0/siriuspy/pwrsupply/bsmp/factory.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.78.0/siriuspy/pwrsupply/csdev.py` & `siriuspy-2.79.0/siriuspy/pwrsupply/csdev.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.78.0/siriuspy/pwrsupply/data.py` & `siriuspy-2.79.0/siriuspy/pwrsupply/data.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.78.0/siriuspy/pwrsupply/factory.py` & `siriuspy-2.79.0/siriuspy/pwrsupply/factory.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.78.0/siriuspy/pwrsupply/pructrl/__init__.py` & `siriuspy-2.79.0/siriuspy/pwrsupply/pructrl/__init__.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.78.0/siriuspy/pwrsupply/pructrl/pru.py` & `siriuspy-2.79.0/siriuspy/pwrsupply/pructrl/pru.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.78.0/siriuspy/pwrsupply/pructrl/prucontroller.py` & `siriuspy-2.79.0/siriuspy/pwrsupply/pructrl/prucontroller.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.78.0/siriuspy/pwrsupply/pructrl/prucparms.py` & `siriuspy-2.79.0/siriuspy/pwrsupply/pructrl/prucparms.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.78.0/siriuspy/pwrsupply/pructrl/psdevstate.py` & `siriuspy-2.79.0/siriuspy/pwrsupply/pructrl/psdevstate.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.78.0/siriuspy/pwrsupply/pructrl/udc.py` & `siriuspy-2.79.0/siriuspy/pwrsupply/pructrl/udc.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.78.0/siriuspy/pwrsupply/psctrl/__init__.py` & `siriuspy-2.79.0/siriuspy/pwrsupply/psctrl/__init__.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.78.0/siriuspy/pwrsupply/psctrl/pscontroller.py` & `siriuspy-2.79.0/siriuspy/pwrsupply/psctrl/pscontroller.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.78.0/siriuspy/pwrsupply/psctrl/pscreaders.py` & `siriuspy-2.79.0/siriuspy/pwrsupply/psctrl/pscreaders.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.78.0/siriuspy/pwrsupply/psctrl/pscstatus.py` & `siriuspy-2.79.0/siriuspy/pwrsupply/psctrl/pscstatus.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.78.0/siriuspy/pwrsupply/psctrl/pscwriters.py` & `siriuspy-2.79.0/siriuspy/pwrsupply/psctrl/pscwriters.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.78.0/siriuspy/pwrsupply/psctrl/psmodel.py` & `siriuspy-2.79.0/siriuspy/pwrsupply/psctrl/psmodel.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.78.0/siriuspy/pwrsupply/pssofb.py` & `siriuspy-2.79.0/siriuspy/pwrsupply/pssofb.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.78.0/siriuspy/pwrsupply/siggen.py` & `siriuspy-2.79.0/siriuspy/pwrsupply/siggen.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.78.0/siriuspy/ramp/conn.py` & `siriuspy-2.79.0/siriuspy/ramp/conn.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.78.0/siriuspy/ramp/magnet.py` & `siriuspy-2.79.0/siriuspy/ramp/magnet.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.78.0/siriuspy/ramp/ramp.py` & `siriuspy-2.79.0/siriuspy/ramp/ramp.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.78.0/siriuspy/ramp/reconst_factory.py` & `siriuspy-2.79.0/siriuspy/ramp/reconst_factory.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.78.0/siriuspy/ramp/test_reconst_factory.py` & `siriuspy-2.79.0/siriuspy/ramp/test_reconst_factory.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.78.0/siriuspy/ramp/testwfm.py` & `siriuspy-2.79.0/siriuspy/ramp/testwfm.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.78.0/siriuspy/ramp/util.py` & `siriuspy-2.79.0/siriuspy/ramp/util.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.78.0/siriuspy/ramp/waveform.py` & `siriuspy-2.79.0/siriuspy/ramp/waveform.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.78.0/siriuspy/search/bpms_search.py` & `siriuspy-2.79.0/siriuspy/search/bpms_search.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.78.0/siriuspy/search/hl_time_search.py` & `siriuspy-2.79.0/siriuspy/search/hl_time_search.py`

 * *Files 6% similar despite different names*

```diff
@@ -103,14 +103,21 @@
     def has_delay_type(cls, hl_trigger):
         """Return True if hl_trigger has property delayType."""
         cls._init()
         ll_chans = cls.get_ll_trigger_names(hl_trigger)
         return all([_LLSearch.has_delay_type(name) for name in ll_chans])
 
     @classmethod
+    def has_direction(cls, hl_trigger):
+        """Return True if hl_trigger has property direction."""
+        cls._init()
+        ll_chans = cls.get_ll_trigger_names(hl_trigger)
+        return all([_LLSearch.has_direction(name) for name in ll_chans])
+
+    @classmethod
     def has_clock(cls, hl_trigger):
         """Return True if hl_trigger can listen to Clocks from EVG."""
         cls._init()
         ll_chans = cls.get_ll_trigger_names(hl_trigger)
         return all([_LLSearch.has_clock(name) for name in ll_chans])
 
     @classmethod
```

### Comparing `siriuspy-2.78.0/siriuspy/search/id_search.py` & `siriuspy-2.79.0/siriuspy/search/id_search.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.78.0/siriuspy/search/ioc_search.py` & `siriuspy-2.79.0/siriuspy/search/ioc_search.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.78.0/siriuspy/search/ll_time_search.py` & `siriuspy-2.79.0/siriuspy/search/ll_time_search.py`

 * *Files 2% similar despite different names*

```diff
@@ -108,14 +108,15 @@
         for conn1, conns in conns_.items():
             for conn2 in conns:
                 dic_[conn2] = conn1
     del dev, conns_, dic_, conn1, conns, conn2  # cleanning class namespace.
 
     _conn_from_evg = dict()
     _conn_twds_evg = dict()
+    _crates_mapping = dict()
     _top_chain_devs = set()
     _final_receiver_devs = set()
     _all_devices = set()
     _trig_src_devs = set()
     _fout_devs = set()
     _evg_devs = set()
     _lock = _Lock()
@@ -310,14 +311,28 @@
             bool: True or False.
 
         """
         name = _PVName(ll_trigger)
         return name.dev in {'EVR', 'EVE'} and name.propty.startswith('OUT')
 
     @classmethod
+    def has_direction(cls, ll_trigger):
+        """Check whether a low level trigger has direction property.
+
+        Args:
+            ll_trigger (SiriusPVName): Trigger name.
+
+        Returns:
+            bool: True or False.
+
+        """
+        name = _PVName(ll_trigger)
+        return 'AMCFPGAEVR' == name.dev
+
+    @classmethod
     def get_trigger_name(cls, channel):
         """Get name of the trigger associated with channel."""
         chan_tree = cls.get_device_tree(channel)
         for up_chan in chan_tree:
             if up_chan.device_name in cls._trig_src_devs:
                 return up_chan
 
@@ -333,14 +348,20 @@
     def get_evg_channel(cls, channel):
         """Get name of the EVG channel associated with channel."""
         chan_tree = cls.get_device_tree(channel)
         for up_chan in chan_tree:
             if up_chan.device_name in cls._evg_devs:
                 return up_chan
 
+    @classmethod
+    def get_crates_mapping(cls):
+        """Return crates to devices mapping."""
+        cls._get_timedata()
+        return cls._crates_mapping
+
     # --- private methods ---
 
     @classmethod
     def _add_entry_to_map(cls, which_map, conn, ele1, ele2):
         if which_map.lower().startswith('from'):
             mapp = cls._conn_from_evg
         else:
@@ -430,14 +451,15 @@
             crate, dev, *_ = line.split()
             dev = _PVName(dev)
             if crate not in mapping and dev.dev == 'AMCFPGAEVR':
                 crates[crate] = dev
                 mapping[crates[crate]] = list()
             else:
                 mapping[crates[crate]].append(dev)
+        cls._crates_mapping = mapping
         return mapping
 
     @classmethod
     def _add_udc_info(cls):
         """Add the information of bbb to PS to timing map."""
         data = _PSSearch.get_udc_dict()
         conn_dict = {udc: [x[0] for x in bsmps] for udc, bsmps in data.items()}
```

### Comparing `siriuspy-2.78.0/siriuspy/search/ma_search.py` & `siriuspy-2.79.0/siriuspy/search/ma_search.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.78.0/siriuspy/search/ps_search.py` & `siriuspy-2.79.0/siriuspy/search/ps_search.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.78.0/siriuspy/simul/simfactory.py` & `siriuspy-2.79.0/siriuspy/simul/simfactory.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.78.0/siriuspy/simul/simps.py` & `siriuspy-2.79.0/siriuspy/simul/simps.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.78.0/siriuspy/simul/simpv.py` & `siriuspy-2.79.0/siriuspy/simul/simpv.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.78.0/siriuspy/simul/simulation.py` & `siriuspy-2.79.0/siriuspy/simul/simulation.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.78.0/siriuspy/simul/simulator.py` & `siriuspy-2.79.0/siriuspy/simul/simulator.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.78.0/siriuspy/sofb/base_class.py` & `siriuspy-2.79.0/siriuspy/sofb/base_class.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.78.0/siriuspy/sofb/bpms.py` & `siriuspy-2.79.0/siriuspy/sofb/bpms.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.78.0/siriuspy/sofb/correctors.py` & `siriuspy-2.79.0/siriuspy/sofb/correctors.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.78.0/siriuspy/sofb/csdev.py` & `siriuspy-2.79.0/siriuspy/sofb/csdev.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.78.0/siriuspy/sofb/main.py` & `siriuspy-2.79.0/siriuspy/sofb/main.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.78.0/siriuspy/sofb/matrix.py` & `siriuspy-2.79.0/siriuspy/sofb/matrix.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.78.0/siriuspy/sofb/orbit.py` & `siriuspy-2.79.0/siriuspy/sofb/orbit.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.78.0/siriuspy/sofb/utils.py` & `siriuspy-2.79.0/siriuspy/sofb/utils.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.78.0/siriuspy/stabinfo/csdev.py` & `siriuspy-2.79.0/siriuspy/stabinfo/csdev.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.78.0/siriuspy/stabinfo/main.py` & `siriuspy-2.79.0/siriuspy/stabinfo/main.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.78.0/siriuspy/thread.py` & `siriuspy-2.79.0/siriuspy/thread.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.78.0/siriuspy/timesys/csdev.py` & `siriuspy-2.79.0/siriuspy/timesys/csdev.py`

 * *Files 2% similar despite different names*

```diff
@@ -17,14 +17,15 @@
 
     EVT_MODES = ('Disable', 'Continuous', 'Injection', 'OneShot', 'External')
     TRIG_SRC_LL = (
         'Dsbl', 'Trigger', 'Clock0', 'Clock1', 'Clock2',
         'Clock3', 'Clock4', 'Clock5', 'Clock6', 'Clock7')
     LOCKLL = ('Unlocked', 'Locked')
     DLYTYP = ('Manual', 'Auto')
+    DIRECTION = ('Receive', 'Transmit')
     ININJTAB = ('No', 'Yes')
     RFOUT = ('OFF', '5RF/2', '5RF/4', 'RF', 'RF/2', 'RF/4')
 
 
 _et = ETypes  # syntactic sugar
 
 
@@ -44,15 +45,16 @@
     EvtModes = _csdev.Const.register('EvtModes', _et.EVT_MODES)
     EvtDlyTyp = _csdev.Const.register('EvtDlyTyp', _et.FIXED_INCR)
     ClockStates = _csdev.Const.register('ClockStates', _et.DSBL_ENBL)
     TrigStates = _csdev.Const.register('TrigStates', _et.DSBL_ENBL)
     TrigPol = _csdev.Const.register('TrigPol', _et.NORM_INV)
     LowLvlLock = _csdev.Const.register('LowLvlLock', _et.LOCKLL)
     TrigDlyTyp = _csdev.Const.register('TrigDlyTyp', _et.DLYTYP)
-    InInjTab = _csdev.Const.register('TrigDlyTyp', _et.ININJTAB)
+    TrigDir = _csdev.Const.register('TrigDir', _et.DIRECTION)
+    InInjTab = _csdev.Const.register('InInjTab', _et.ININJTAB)
     TrigSrcLL = _csdev.Const.register('TrigSrcLL', _et.TRIG_SRC_LL)
     HLTrigStatusLabels = (
         'All PVs connected',
         'Device Enabled',
         'Fout Enabled',
         'EVG Enabled',
         'Network Ok',
@@ -585,19 +587,23 @@
 
     dic_ = {'type': 'enum', 'enums': _et.LOCKLL, 'value': 0}
     dbase['LowLvlLock-Sts'] = _dcopy(dic_)
     dbase['LowLvlLock-Sel'] = dic_
 
     dic_ = {'type': 'enum', 'enums': _et.DLYTYP}
     dic_.update(trig_db['RFDelayType'])
-    dbase['RFDelayType-Sts'] = _dcopy(dic_)
-    dbase['RFDelayType-Sel'] = dic_
-    if not _HLTimeSearch.has_delay_type(hl_trigger):
-        dbase.pop('RFDelayType-Sts')
-        dbase.pop('RFDelayType-Sel')
+    if _HLTimeSearch.has_delay_type(hl_trigger):
+        dbase['RFDelayType-Sts'] = _dcopy(dic_)
+        dbase['RFDelayType-Sel'] = dic_
+
+    dic_ = {'type': 'enum', 'enums': _et.DIRECTION}
+    dic_.update(trig_db.get('Direction', dict()))
+    if _HLTimeSearch.has_direction(hl_trigger):
+        dbase['Direction-Sel'] = _dcopy(dic_)
+        dbase['Direction-Sts'] = dic_
 
     dbase['Status-Mon'] = {'type': 'int', 'value': 0b1111111111}
     dbase['InInjTable-Mon'] = {
         'type': 'enum', 'enums': _et.ININJTAB, 'value': 0}
 
     dbase['StatusLabels-Cte'] = {
         'type': 'char', 'count': 1000,
```

### Comparing `siriuspy-2.78.0/siriuspy/timesys/hl_classes.py` & `siriuspy-2.79.0/siriuspy/timesys/hl_classes.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.78.0/siriuspy/timesys/ll_classes.py` & `siriuspy-2.79.0/siriuspy/timesys/ll_classes.py`

 * *Files 1% similar despite different names*

```diff
@@ -372,16 +372,14 @@
         if self.channel.propty.startswith('OUT'):
             intrg = _LLSearch.get_channel_internal_trigger_pvname(self.channel)
             intrg = int(intrg.propty[-2:])  # get internal trigger number
             self._config_ok_values['SrcTrig'] = intrg
             # Stop using FineDelay and RF Delay to ease consistency:
             self._config_ok_values['FineDelay'] = 0
             self._config_ok_values['RFDelay'] = 0
-        elif self.channel.propty.startswith(('FMC', 'CRT')):
-            self._config_ok_values['Dir'] = 0
 
     def write(self, prop, value):
         # keep this info for recalculating Width whenever necessary
         if prop == 'Duration':
             self._duration = value
         elif prop == 'WidthRaw':
             pul = self._config_ok_values.get('NrPulses') or 1
@@ -439,26 +437,27 @@
             'Polarity': _partial(self._set_simple, 'Polarity'),
             'NrPulses': self._set_nrpulses,
             'Delay': _partial(self._set_delay, raw=False),
             'DelayRaw': _partial(self._set_delay, raw=True),
             'RFDelayType': _partial(self._set_simple, 'RFDelayType'),
             'RFDelayType': self._set_rfdelaytype,
             'LowLvlLock': self._set_locked,
+            'Direction': _partial(self._set_simple, 'Dir'),
             }
         return map_
 
     def _define_dict_for_update(self):
         map_ = {
             'State': _partial(self._get_simple, 'State'),
             'Evt': _partial(self._process_source, 'Evt'),
             'Width': _partial(self._get_duration_pulses, 'Width'),
             'Polarity': _partial(self._get_simple, 'Polarity'),
             'NrPulses': _partial(self._get_duration_pulses, 'NrPulses'),
             'Delay': _partial(self._get_delay, 'Delay'),
-            'Dir': _partial(self._get_simple, 'Dir'),
+            'Dir': _partial(self._get_simple, 'Dir', hl_prop='Direction'),
             'Src': _partial(self._process_source, 'Src'),
             'SrcTrig': _partial(self._process_source, 'SrcTrig'),
             'RFDelay': _partial(self._get_delay, 'RFDelay'),
             'FineDelay': _partial(self._get_delay, 'FineDelay'),
             'RFDelayType': _partial(self._get_simple, 'RFDelayType'),
             'DevEnbl': _partial(self._get_status, 'DevEnbl'),
             'Network': _partial(self._get_status, 'Network'),
@@ -486,14 +485,16 @@
             'TotalDelay': _partial(self._get_delay, 'Delay'),
             'TotalDelayRaw': _partial(self._get_delay, 'Delay'),
             'Src': _partial(self._process_source, ''),
             'RFDelayType': _partial(self._get_simple, 'RFDelayType'),
             'Status': _partial(self._get_status, ''),
             'InInjTable': _partial(self._get_status, ''),
             'LowLvlLock': lambda is_sp: {'LowLvlLock': self.locked},
+            'Direction': _partial(
+                self._get_simple, 'Dir', hl_prop='Direction'),
             }
         return map_
 
     def _get_status(self, prop, is_sp, value=None):
         dic_ = dict()
         dic_['DevEnbl'] = self._get_from_pvs(is_sp, 'DevEnbl', def_val=0)
         dic_['EVGDevEnbl'] = self._get_from_pvs(is_sp, 'EVGDevEnbl', def_val=0)
```

### Comparing `siriuspy-2.78.0/siriuspy/timesys/plot_network.py` & `siriuspy-2.79.0/siriuspy/timesys/plot_network.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.78.0/siriuspy/timesys/static_table.py` & `siriuspy-2.79.0/siriuspy/timesys/static_table.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.78.0/siriuspy/util.py` & `siriuspy-2.79.0/siriuspy/util.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.78.0/siriuspy.egg-info/PKG-INFO` & `siriuspy-2.79.0/siriuspy.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: siriuspy
-Version: 2.78.0
+Version: 2.79.0
 Summary: Development packages for Sirius
 Home-page: https://github.com/lnls-sirius/dev-packages
 Download-URL: https://github.com/lnls-sirius/dev-packages
 Author: lnls-sirius
 License: GNU GPLv3
 Classifier: Intended Audience :: Science/Research
 Classifier: Programming Language :: Python
```

### Comparing `siriuspy-2.78.0/siriuspy.egg-info/SOURCES.txt` & `siriuspy-2.79.0/siriuspy.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -76,24 +76,26 @@
 siriuspy/cycle/bo_cycle_data.py
 siriuspy/cycle/conn.py
 siriuspy/cycle/fc_cycle_data.py
 siriuspy/cycle/li_cycle_data.py
 siriuspy/cycle/main.py
 siriuspy/cycle/util.py
 siriuspy/devices/__init__.py
+siriuspy/devices/afc_acq_core.py
 siriuspy/devices/bbb.py
 siriuspy/devices/blctrl.py
 siriuspy/devices/bpm.py
 siriuspy/devices/currinfo.py
 siriuspy/devices/dcct.py
 siriuspy/devices/device.py
 siriuspy/devices/dvf.py
 siriuspy/devices/egun.py
 siriuspy/devices/energy.py
 siriuspy/devices/fofb.py
+siriuspy/devices/fofb_acq.py
 siriuspy/devices/ict.py
 siriuspy/devices/idff.py
 siriuspy/devices/ids.py
 siriuspy/devices/injctrl.py
 siriuspy/devices/injsys.py
 siriuspy/devices/lienergy.py
 siriuspy/devices/lillrf.py
@@ -102,14 +104,15 @@
 siriuspy/devices/orbit_interlock.py
 siriuspy/devices/posang.py
 siriuspy/devices/psconv.py
 siriuspy/devices/pssofb.py
 siriuspy/devices/pstesters.py
 siriuspy/devices/pwrsupply.py
 siriuspy/devices/rf.py
+siriuspy/devices/scraper.py
 siriuspy/devices/screen.py
 siriuspy/devices/sofb.py
 siriuspy/devices/syncd.py
 siriuspy/devices/timing.py
 siriuspy/devices/tune.py
 siriuspy/diagbeam/__init__.py
 siriuspy/diagbeam/bpm/__init__.py
```

### Comparing `siriuspy-2.78.0/tests/bsmp/test_bsmp.py` & `siriuspy-2.79.0/tests/bsmp/test_bsmp.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.78.0/tests/bsmp/test_commands.py` & `siriuspy-2.79.0/tests/bsmp/test_commands.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.78.0/tests/bsmp/test_entities.py` & `siriuspy-2.79.0/tests/bsmp/test_entities.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.78.0/tests/bsmp/test_serial.py` & `siriuspy-2.79.0/tests/bsmp/test_serial.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.78.0/tests/bsmp/test_types.py` & `siriuspy-2.79.0/tests/bsmp/test_types.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.78.0/tests/clientconfigdb/test_configdb_client.py` & `siriuspy-2.79.0/tests/clientconfigdb/test_configdb_client.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.78.0/tests/clientweb/test_implementation.py` & `siriuspy-2.79.0/tests/clientweb/test_implementation.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.78.0/tests/currinfo/lifetime/test_main.py` & `siriuspy-2.79.0/tests/currinfo/lifetime/test_main.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.78.0/tests/currinfo/test_csdev.py` & `siriuspy-2.79.0/tests/currinfo/test_csdev.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.78.0/tests/currinfo/test_main.py` & `siriuspy-2.79.0/tests/currinfo/test_main.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.78.0/tests/magnet/test_factory.py` & `siriuspy-2.79.0/tests/magnet/test_factory.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.78.0/tests/magnet/tests_normalizer.py` & `siriuspy-2.79.0/tests/magnet/tests_normalizer.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.78.0/tests/mock_servweb.py` & `siriuspy-2.79.0/tests/mock_servweb.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.78.0/tests/namesys/test_implementation.py` & `siriuspy-2.79.0/tests/namesys/test_implementation.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.78.0/tests/opticscorr/test_chrom.py` & `siriuspy-2.79.0/tests/opticscorr/test_chrom.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.78.0/tests/opticscorr/test_csdev.py` & `siriuspy-2.79.0/tests/opticscorr/test_csdev.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.78.0/tests/opticscorr/test_opticscorr.py` & `siriuspy-2.79.0/tests/opticscorr/test_opticscorr.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.78.0/tests/opticscorr/test_tune.py` & `siriuspy-2.79.0/tests/opticscorr/test_tune.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.78.0/tests/opticscorr/test_utils.py` & `siriuspy-2.79.0/tests/opticscorr/test_utils.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.78.0/tests/posang/test_csdev.py` & `siriuspy-2.79.0/tests/posang/test_csdev.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.78.0/tests/posang/test_main.py` & `siriuspy-2.79.0/tests/posang/test_main.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.78.0/tests/pwrsupply/db.py` & `siriuspy-2.79.0/tests/pwrsupply/db.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.78.0/tests/pwrsupply/pructrl/test_pru.py` & `siriuspy-2.79.0/tests/pwrsupply/pructrl/test_pru.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.78.0/tests/pwrsupply/psctrl/test_pscwriters.py` & `siriuspy-2.79.0/tests/pwrsupply/psctrl/test_pscwriters.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.78.0/tests/pwrsupply/test_csdev.py` & `siriuspy-2.79.0/tests/pwrsupply/test_csdev.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.78.0/tests/pwrsupply/test_data.py` & `siriuspy-2.79.0/tests/pwrsupply/test_data.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.78.0/tests/pwrsupply/test_siggen.py` & `siriuspy-2.79.0/tests/pwrsupply/test_siggen.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.78.0/tests/pwrsupply/variables.py` & `siriuspy-2.79.0/tests/pwrsupply/variables.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.78.0/tests/ramp/test_magnet.py` & `siriuspy-2.79.0/tests/ramp/test_magnet.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.78.0/tests/ramp/test_waveform.py` & `siriuspy-2.79.0/tests/ramp/test_waveform.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.78.0/tests/search/test_hl_time_search.py` & `siriuspy-2.79.0/tests/search/test_hl_time_search.py`

 * *Files 1% similar despite different names*

```diff
@@ -32,14 +32,15 @@
         'get_hl_trigger_sources',
         'get_hl_trigger_prop_value',
         'get_hl_trigger_prop_limits',
         'get_hl_trigger_interface',
         'get_ll_trigger_names',
         'get_hl_from_ll_triggers',
         'has_delay_type',
+        'has_direction',
         'has_clock',
         'check_hl_triggers_consistency',
         'reset',
     )
 
     def get_hl_triggers(self):
         """Test get_hl_triggers."""
@@ -71,15 +72,15 @@
         # TODO: implement test!
         pass
 
     def get_ll_trigger_names(self):
         """Test get_ll_trigger_names."""
         # TODO: implement test!
         pass
-    
+
     def get_hl_from_triggers(self):
         """Test get_hl_from_ll_triggers."""
         # TODO: implement test!
         pass
 
     def has_delay_type(self):
         """Test has_delay_type."""
```

### Comparing `siriuspy-2.78.0/tests/search/test_init.py` & `siriuspy-2.79.0/tests/search/test_init.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.78.0/tests/search/test_ll_time_search.py` & `siriuspy-2.79.0/tests/search/test_ll_time_search.py`

 * *Files 3% similar despite different names*

```diff
@@ -48,17 +48,19 @@
         'get_connections_twds_evg',
         'get_top_chain_senders',
         'get_final_receivers',
         'get_relations_from_evg',
         'get_relations_twds_evg',
         'has_clock',
         'has_delay_type',
+        'has_direction',
         'get_trigger_name',
         'get_fout_channel',
         'get_evg_channel',
+        'get_crates_mapping',
     )
 
     def test_public_interface(self):
         """Test class public interface."""
         valid = util.check_public_interface_namespace(
             ll_time_search.LLTimeSearch, TestLLTimeSearch.public_interface)
         self.assertTrue(valid)
```

### Comparing `siriuspy-2.78.0/tests/search/test_ma_search.py` & `siriuspy-2.79.0/tests/search/test_ma_search.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.78.0/tests/search/test_ps_search.py` & `siriuspy-2.79.0/tests/search/test_ps_search.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.78.0/tests/test_callbacks.py` & `siriuspy-2.79.0/tests/test_callbacks.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.78.0/tests/test_csdev.py` & `siriuspy-2.79.0/tests/test_csdev.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.78.0/tests/test_envars.py` & `siriuspy-2.79.0/tests/test_envars.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.78.0/tests/test_util.py` & `siriuspy-2.79.0/tests/test_util.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.78.0/tests/timesys/test_csdev.py` & `siriuspy-2.79.0/tests/timesys/test_csdev.py`

 * *Files 1% similar despite different names*

```diff
@@ -181,14 +181,15 @@
         'EvtModes',
         'EvtDlyTyp',
         'ClockStates',
         'TrigStates',
         'TrigPol',
         'LowLvlLock',
         'TrigDlyTyp',
+        'TrigDir',
         'InInjTab',
         'TrigSrcLL',
         'EvtHL2LLMap',
         'EvtLL2HLMap',
         'EvtLL',
         'ClkHL2LLMap',
         'ClkLL2HLMap',
```

### Comparing `siriuspy-2.78.0/tests/timesys/test_plot_network.py` & `siriuspy-2.79.0/tests/timesys/test_plot_network.py`

 * *Files identical despite different names*

