# Comparing `tmp/siriuspy-2.73.0.tar.gz` & `tmp/siriuspy-2.74.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "siriuspy-2.73.0.tar", last modified: Thu Apr 20 19:20:58 2023, max compression
+gzip compressed data, was "siriuspy-2.74.0.tar", last modified: Mon May 15 11:31:28 2023, max compression
```

## Comparing `siriuspy-2.73.0.tar` & `siriuspy-2.74.0.tar`

### file list

```diff
@@ -1,387 +1,389 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-20 19:20:58.852560 siriuspy-2.73.0/
--rw-r--r--   0 runner    (1001) docker     (122)    34494 2023-04-20 19:20:44.000000 siriuspy-2.73.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (122)       90 2023-04-20 19:20:44.000000 siriuspy-2.73.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (122)     1423 2023-04-20 19:20:58.848559 siriuspy-2.73.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)      954 2023-04-20 19:20:44.000000 siriuspy-2.73.0/README.md
--rw-r--r--   0 runner    (1001) docker     (122)      128 2023-04-20 19:20:44.000000 siriuspy-2.73.0/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (122)       38 2023-04-20 19:20:58.852560 siriuspy-2.73.0/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (122)     1243 2023-04-20 19:20:44.000000 siriuspy-2.73.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-20 19:20:58.784550 siriuspy-2.73.0/siriuspy/
--rw-r--r--   0 runner    (1001) docker     (122)        7 2023-04-20 19:20:44.000000 siriuspy-2.73.0/siriuspy/VERSION
--rw-r--r--   0 runner    (1001) docker     (122)      497 2023-04-20 19:20:44.000000 siriuspy-2.73.0/siriuspy/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-20 19:20:58.788551 siriuspy-2.73.0/siriuspy/bsmp/
--rw-r--r--   0 runner    (1001) docker     (122)      422 2023-04-20 19:20:44.000000 siriuspy-2.73.0/siriuspy/bsmp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    15885 2023-04-20 19:20:44.000000 siriuspy-2.73.0/siriuspy/bsmp/commands.py
--rw-r--r--   0 runner    (1001) docker     (122)     1904 2023-04-20 19:20:44.000000 siriuspy-2.73.0/siriuspy/bsmp/constants.py
--rw-r--r--   0 runner    (1001) docker     (122)    11790 2023-04-20 19:20:44.000000 siriuspy-2.73.0/siriuspy/bsmp/entities.py
--rw-r--r--   0 runner    (1001) docker     (122)      610 2023-04-20 19:20:44.000000 siriuspy-2.73.0/siriuspy/bsmp/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (122)     8110 2023-04-20 19:20:44.000000 siriuspy-2.73.0/siriuspy/bsmp/serial.py
--rw-r--r--   0 runner    (1001) docker     (122)     1204 2023-04-20 19:20:44.000000 siriuspy-2.73.0/siriuspy/bsmp/types.py
--rw-r--r--   0 runner    (1001) docker     (122)     2992 2023-04-20 19:20:44.000000 siriuspy-2.73.0/siriuspy/callbacks.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-20 19:20:58.788551 siriuspy-2.73.0/siriuspy/clientarch/
--rw-r--r--   0 runner    (1001) docker     (122)      306 2023-04-20 19:20:44.000000 siriuspy-2.73.0/siriuspy/clientarch/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    13813 2023-04-20 19:20:44.000000 siriuspy-2.73.0/siriuspy/clientarch/client.py
--rw-r--r--   0 runner    (1001) docker     (122)     6392 2023-04-20 19:20:44.000000 siriuspy-2.73.0/siriuspy/clientarch/devices.py
--rw-r--r--   0 runner    (1001) docker     (122)      643 2023-04-20 19:20:44.000000 siriuspy-2.73.0/siriuspy/clientarch/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (122)    20400 2023-04-20 19:20:44.000000 siriuspy-2.73.0/siriuspy/clientarch/pvarch.py
--rw-r--r--   0 runner    (1001) docker     (122)     5003 2023-04-20 19:20:44.000000 siriuspy-2.73.0/siriuspy/clientarch/time.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-20 19:20:58.788551 siriuspy-2.73.0/siriuspy/clientconfigdb/
--rw-r--r--   0 runner    (1001) docker     (122)      227 2023-04-20 19:20:44.000000 siriuspy-2.73.0/siriuspy/clientconfigdb/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     3535 2023-04-20 19:20:44.000000 siriuspy-2.73.0/siriuspy/clientconfigdb/_templates.py
--rw-r--r--   0 runner    (1001) docker     (122)     9599 2023-04-20 19:20:44.000000 siriuspy-2.73.0/siriuspy/clientconfigdb/configdb_client.py
--rw-r--r--   0 runner    (1001) docker     (122)     5448 2023-04-20 19:20:44.000000 siriuspy-2.73.0/siriuspy/clientconfigdb/configdb_document.py
--rw-r--r--   0 runner    (1001) docker     (122)     4785 2023-04-20 19:20:44.000000 siriuspy-2.73.0/siriuspy/clientconfigdb/pvsconfig.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-20 19:20:58.792551 siriuspy-2.73.0/siriuspy/clientconfigdb/types/
--rw-r--r--   0 runner    (1001) docker     (122)      286 2023-04-20 19:20:44.000000 siriuspy-2.73.0/siriuspy/clientconfigdb/types/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    13746 2023-04-20 19:20:44.000000 siriuspy-2.73.0/siriuspy/clientconfigdb/types/as_corrloop_params.py
--rw-r--r--   0 runner    (1001) docker     (122)    57636 2023-04-20 19:20:44.000000 siriuspy-2.73.0/siriuspy/clientconfigdb/types/as_diagnostics.py
--rw-r--r--   0 runner    (1001) docker     (122)     6681 2023-04-20 19:20:44.000000 siriuspy-2.73.0/siriuspy/clientconfigdb/types/as_pwrstate.py
--rw-r--r--   0 runner    (1001) docker     (122)    34247 2023-04-20 19:20:44.000000 siriuspy-2.73.0/siriuspy/clientconfigdb/types/as_rf.py
--rw-r--r--   0 runner    (1001) docker     (122)     1135 2023-04-20 19:20:44.000000 siriuspy-2.73.0/siriuspy/clientconfigdb/types/bo_chromcorr_params.py
--rw-r--r--   0 runner    (1001) docker     (122)     3984 2023-04-20 19:20:44.000000 siriuspy-2.73.0/siriuspy/clientconfigdb/types/bo_normalized.py
--rw-r--r--   0 runner    (1001) docker     (122)     1135 2023-04-20 19:20:44.000000 siriuspy-2.73.0/siriuspy/clientconfigdb/types/bo_orbcorr_respm.py
--rw-r--r--   0 runner    (1001) docker     (122)      700 2023-04-20 19:20:44.000000 siriuspy-2.73.0/siriuspy/clientconfigdb/types/bo_orbit.py
--rw-r--r--   0 runner    (1001) docker     (122)     3042 2023-04-20 19:20:44.000000 siriuspy-2.73.0/siriuspy/clientconfigdb/types/bo_ramp.py
--rw-r--r--   0 runner    (1001) docker     (122)      975 2023-04-20 19:20:44.000000 siriuspy-2.73.0/siriuspy/clientconfigdb/types/bo_tunecorr_params.py
--rw-r--r--   0 runner    (1001) docker     (122)   122432 2023-04-20 19:20:44.000000 siriuspy-2.73.0/siriuspy/clientconfigdb/types/global_config.py
--rw-r--r--   0 runner    (1001) docker     (122)      735 2023-04-20 19:20:44.000000 siriuspy-2.73.0/siriuspy/clientconfigdb/types/si_bbadata.py
--rw-r--r--   0 runner    (1001) docker     (122)    18619 2023-04-20 19:20:44.000000 siriuspy-2.73.0/siriuspy/clientconfigdb/types/si_bbbproc.py
--rw-r--r--   0 runner    (1001) docker     (122)     1697 2023-04-20 19:20:44.000000 siriuspy-2.73.0/siriuspy/clientconfigdb/types/si_chromcorr_params.py
--rw-r--r--   0 runner    (1001) docker     (122)     1146 2023-04-20 19:20:44.000000 siriuspy-2.73.0/siriuspy/clientconfigdb/types/si_fastorbcorr_respm.py
--rw-r--r--   0 runner    (1001) docker     (122)     4741 2023-04-20 19:20:44.000000 siriuspy-2.73.0/siriuspy/clientconfigdb/types/si_fofb.py
--rw-r--r--   0 runner    (1001) docker     (122)      957 2023-04-20 19:20:44.000000 siriuspy-2.73.0/siriuspy/clientconfigdb/types/si_id.py
--rw-r--r--   0 runner    (1001) docker     (122)     1860 2023-04-20 19:20:44.000000 siriuspy-2.73.0/siriuspy/clientconfigdb/types/si_idff.py
--rw-r--r--   0 runner    (1001) docker     (122)     1136 2023-04-20 19:20:44.000000 siriuspy-2.73.0/siriuspy/clientconfigdb/types/si_orbcorr_respm.py
--rw-r--r--   0 runner    (1001) docker     (122)      701 2023-04-20 19:20:44.000000 siriuspy-2.73.0/siriuspy/clientconfigdb/types/si_orbit.py
--rw-r--r--   0 runner    (1001) docker     (122)     1290 2023-04-20 19:20:44.000000 siriuspy-2.73.0/siriuspy/clientconfigdb/types/si_tunecorr_params.py
--rw-r--r--   0 runner    (1001) docker     (122)     1738 2023-04-20 19:20:44.000000 siriuspy-2.73.0/siriuspy/clientconfigdb/types/tb_normalized.py
--rw-r--r--   0 runner    (1001) docker     (122)      969 2023-04-20 19:20:44.000000 siriuspy-2.73.0/siriuspy/clientconfigdb/types/tb_orbcorr_respm.py
--rw-r--r--   0 runner    (1001) docker     (122)      693 2023-04-20 19:20:44.000000 siriuspy-2.73.0/siriuspy/clientconfigdb/types/tb_orbit.py
--rw-r--r--   0 runner    (1001) docker     (122)     1651 2023-04-20 19:20:44.000000 siriuspy-2.73.0/siriuspy/clientconfigdb/types/tb_posang_respm.py
--rw-r--r--   0 runner    (1001) docker     (122)      969 2023-04-20 19:20:44.000000 siriuspy-2.73.0/siriuspy/clientconfigdb/types/ts_orbcorr_respm.py
--rw-r--r--   0 runner    (1001) docker     (122)      693 2023-04-20 19:20:44.000000 siriuspy-2.73.0/siriuspy/clientconfigdb/types/ts_orbit.py
--rw-r--r--   0 runner    (1001) docker     (122)     1721 2023-04-20 19:20:44.000000 siriuspy-2.73.0/siriuspy/clientconfigdb/types/ts_posang_respm.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-20 19:20:58.792551 siriuspy-2.73.0/siriuspy/clientweb/
--rw-r--r--   0 runner    (1001) docker     (122)       50 2023-04-20 19:20:44.000000 siriuspy-2.73.0/siriuspy/clientweb/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     5896 2023-04-20 19:20:44.000000 siriuspy-2.73.0/siriuspy/clientweb/implementation.py
--rw-r--r--   0 runner    (1001) docker     (122)     2236 2023-04-20 19:20:44.000000 siriuspy-2.73.0/siriuspy/csdev.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-20 19:20:58.792551 siriuspy-2.73.0/siriuspy/currinfo/
--rw-r--r--   0 runner    (1001) docker     (122)      144 2023-04-20 19:20:44.000000 siriuspy-2.73.0/siriuspy/currinfo/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     9620 2023-04-20 19:20:44.000000 siriuspy-2.73.0/siriuspy/currinfo/csdev.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-20 19:20:58.792551 siriuspy-2.73.0/siriuspy/currinfo/lifetime/
--rw-r--r--   0 runner    (1001) docker     (122)       72 2023-04-20 19:20:44.000000 siriuspy-2.73.0/siriuspy/currinfo/lifetime/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    12607 2023-04-20 19:20:44.000000 siriuspy-2.73.0/siriuspy/currinfo/lifetime/main.py
--rw-r--r--   0 runner    (1001) docker     (122)    23275 2023-04-20 19:20:44.000000 siriuspy-2.73.0/siriuspy/currinfo/main.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-20 19:20:58.792551 siriuspy-2.73.0/siriuspy/cycle/
--rw-r--r--   0 runner    (1001) docker     (122)      514 2023-04-20 19:20:44.000000 siriuspy-2.73.0/siriuspy/cycle/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)   104994 2023-04-20 19:20:44.000000 siriuspy-2.73.0/siriuspy/cycle/bo_cycle_data.py
--rw-r--r--   0 runner    (1001) docker     (122)    31135 2023-04-20 19:20:44.000000 siriuspy-2.73.0/siriuspy/cycle/conn.py
--rw-r--r--   0 runner    (1001) docker     (122)     9781 2023-04-20 19:20:44.000000 siriuspy-2.73.0/siriuspy/cycle/fc_cycle_data.py
--rw-r--r--   0 runner    (1001) docker     (122)     3286 2023-04-20 19:20:44.000000 siriuspy-2.73.0/siriuspy/cycle/li_cycle_data.py
--rw-r--r--   0 runner    (1001) docker     (122)    38408 2023-04-20 19:20:44.000000 siriuspy-2.73.0/siriuspy/cycle/main.py
--rw-r--r--   0 runner    (1001) docker     (122)     3567 2023-04-20 19:20:44.000000 siriuspy-2.73.0/siriuspy/cycle/util.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-20 19:20:58.796552 siriuspy-2.73.0/siriuspy/devices/
--rw-r--r--   0 runner    (1001) docker     (122)     1696 2023-04-20 19:20:44.000000 siriuspy-2.73.0/siriuspy/devices/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    48546 2023-04-20 19:20:44.000000 siriuspy-2.73.0/siriuspy/devices/bbb.py
--rw-r--r--   0 runner    (1001) docker     (122)    40979 2023-04-20 19:20:44.000000 siriuspy-2.73.0/siriuspy/devices/bpm.py
--rw-r--r--   0 runner    (1001) docker     (122)     7380 2023-04-20 19:20:44.000000 siriuspy-2.73.0/siriuspy/devices/currinfo.py
--rw-r--r--   0 runner    (1001) docker     (122)     2402 2023-04-20 19:20:44.000000 siriuspy-2.73.0/siriuspy/devices/dcct.py
--rw-r--r--   0 runner    (1001) docker     (122)    12731 2023-04-20 19:20:44.000000 siriuspy-2.73.0/siriuspy/devices/device.py
--rw-r--r--   0 runner    (1001) docker     (122)     6799 2023-04-20 19:20:44.000000 siriuspy-2.73.0/siriuspy/devices/dvf.py
--rw-r--r--   0 runner    (1001) docker     (122)    30814 2023-04-20 19:20:44.000000 siriuspy-2.73.0/siriuspy/devices/egun.py
--rw-r--r--   0 runner    (1001) docker     (122)     1743 2023-04-20 19:20:44.000000 siriuspy-2.73.0/siriuspy/devices/energy.py
--rw-r--r--   0 runner    (1001) docker     (122)    48527 2023-04-20 19:20:44.000000 siriuspy-2.73.0/siriuspy/devices/fofb.py
--rw-r--r--   0 runner    (1001) docker     (122)     2121 2023-04-20 19:20:44.000000 siriuspy-2.73.0/siriuspy/devices/ict.py
--rw-r--r--   0 runner    (1001) docker     (122)     4996 2023-04-20 19:20:44.000000 siriuspy-2.73.0/siriuspy/devices/idff.py
--rw-r--r--   0 runner    (1001) docker     (122)    17197 2023-04-20 19:20:44.000000 siriuspy-2.73.0/siriuspy/devices/ids.py
--rw-r--r--   0 runner    (1001) docker     (122)    20741 2023-04-20 19:20:44.000000 siriuspy-2.73.0/siriuspy/devices/injctrl.py
--rw-r--r--   0 runner    (1001) docker     (122)    36024 2023-04-20 19:20:44.000000 siriuspy-2.73.0/siriuspy/devices/injsys.py
--rw-r--r--   0 runner    (1001) docker     (122)     1630 2023-04-20 19:20:44.000000 siriuspy-2.73.0/siriuspy/devices/lienergy.py
--rw-r--r--   0 runner    (1001) docker     (122)     6948 2023-04-20 19:20:44.000000 siriuspy-2.73.0/siriuspy/devices/lillrf.py
--rw-r--r--   0 runner    (1001) docker     (122)      964 2023-04-20 19:20:44.000000 siriuspy-2.73.0/siriuspy/devices/machshift.py
--rw-r--r--   0 runner    (1001) docker     (122)     2290 2023-04-20 19:20:44.000000 siriuspy-2.73.0/siriuspy/devices/modltr.py
--rw-r--r--   0 runner    (1001) docker     (122)    36060 2023-04-20 19:20:44.000000 siriuspy-2.73.0/siriuspy/devices/orbit_interlock.py
--rw-r--r--   0 runner    (1001) docker     (122)     2427 2023-04-20 19:20:44.000000 siriuspy-2.73.0/siriuspy/devices/posang.py
--rw-r--r--   0 runner    (1001) docker     (122)     9576 2023-04-20 19:20:44.000000 siriuspy-2.73.0/siriuspy/devices/psconv.py
--rw-r--r--   0 runner    (1001) docker     (122)    12042 2023-04-20 19:20:44.000000 siriuspy-2.73.0/siriuspy/devices/pssofb.py
--rw-r--r--   0 runner    (1001) docker     (122)    19964 2023-04-20 19:20:44.000000 siriuspy-2.73.0/siriuspy/devices/pstesters.py
--rw-r--r--   0 runner    (1001) docker     (122)    28397 2023-04-20 19:20:44.000000 siriuspy-2.73.0/siriuspy/devices/pwrsupply.py
--rw-r--r--   0 runner    (1001) docker     (122)    35448 2023-04-20 19:20:44.000000 siriuspy-2.73.0/siriuspy/devices/rf.py
--rw-r--r--   0 runner    (1001) docker     (122)     3836 2023-04-20 19:20:44.000000 siriuspy-2.73.0/siriuspy/devices/screen.py
--rw-r--r--   0 runner    (1001) docker     (122)    22629 2023-04-20 19:20:44.000000 siriuspy-2.73.0/siriuspy/devices/sofb.py
--rw-r--r--   0 runner    (1001) docker     (122)     2606 2023-04-20 19:20:44.000000 siriuspy-2.73.0/siriuspy/devices/syncd.py
--rw-r--r--   0 runner    (1001) docker     (122)    17907 2023-04-20 19:20:44.000000 siriuspy-2.73.0/siriuspy/devices/timing.py
--rw-r--r--   0 runner    (1001) docker     (122)     5055 2023-04-20 19:20:44.000000 siriuspy-2.73.0/siriuspy/devices/tune.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-20 19:20:58.796552 siriuspy-2.73.0/siriuspy/diagbeam/
--rw-r--r--   0 runner    (1001) docker     (122)       30 2023-04-20 19:20:44.000000 siriuspy-2.73.0/siriuspy/diagbeam/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-20 19:20:58.796552 siriuspy-2.73.0/siriuspy/diagbeam/bpm/
--rw-r--r--   0 runner    (1001) docker     (122)       24 2023-04-20 19:20:44.000000 siriuspy-2.73.0/siriuspy/diagbeam/bpm/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    24052 2023-04-20 19:20:44.000000 siriuspy-2.73.0/siriuspy/diagbeam/bpm/csdev.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-20 19:20:58.796552 siriuspy-2.73.0/siriuspy/diagbeam/dcct/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-20 19:20:44.000000 siriuspy-2.73.0/siriuspy/diagbeam/dcct/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     8215 2023-04-20 19:20:44.000000 siriuspy-2.73.0/siriuspy/diagbeam/dcct/csdev.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-20 19:20:58.796552 siriuspy-2.73.0/siriuspy/diagbeam/ict/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-20 19:20:44.000000 siriuspy-2.73.0/siriuspy/diagbeam/ict/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     4878 2023-04-20 19:20:44.000000 siriuspy-2.73.0/siriuspy/diagbeam/ict/csdev.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-20 19:20:58.796552 siriuspy-2.73.0/siriuspy/diagbeam/screen/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-20 19:20:44.000000 siriuspy-2.73.0/siriuspy/diagbeam/screen/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    12756 2023-04-20 19:20:44.000000 siriuspy-2.73.0/siriuspy/diagbeam/screen/csdev.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-20 19:20:58.796552 siriuspy-2.73.0/siriuspy/diagbeam/slit/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-20 19:20:44.000000 siriuspy-2.73.0/siriuspy/diagbeam/slit/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     6750 2023-04-20 19:20:44.000000 siriuspy-2.73.0/siriuspy/diagbeam/slit/csdev.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-20 19:20:58.800552 siriuspy-2.73.0/siriuspy/diagsys/
--rw-r--r--   0 runner    (1001) docker     (122)       26 2023-04-20 19:20:44.000000 siriuspy-2.73.0/siriuspy/diagsys/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     1444 2023-04-20 19:20:44.000000 siriuspy-2.73.0/siriuspy/diagsys/app.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-20 19:20:58.800552 siriuspy-2.73.0/siriuspy/diagsys/lidiag/
--rw-r--r--   0 runner    (1001) docker     (122)       29 2023-04-20 19:20:44.000000 siriuspy-2.73.0/siriuspy/diagsys/lidiag/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     5193 2023-04-20 19:20:44.000000 siriuspy-2.73.0/siriuspy/diagsys/lidiag/csdev.py
--rw-r--r--   0 runner    (1001) docker     (122)     8168 2023-04-20 19:20:44.000000 siriuspy-2.73.0/siriuspy/diagsys/lidiag/main.py
--rw-r--r--   0 runner    (1001) docker     (122)     8774 2023-04-20 19:20:44.000000 siriuspy-2.73.0/siriuspy/diagsys/lidiag/pvs.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-20 19:20:58.800552 siriuspy-2.73.0/siriuspy/diagsys/psdiag/
--rw-r--r--   0 runner    (1001) docker     (122)       25 2023-04-20 19:20:44.000000 siriuspy-2.73.0/siriuspy/diagsys/psdiag/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     2556 2023-04-20 19:20:44.000000 siriuspy-2.73.0/siriuspy/diagsys/psdiag/csdev.py
--rw-r--r--   0 runner    (1001) docker     (122)     4299 2023-04-20 19:20:44.000000 siriuspy-2.73.0/siriuspy/diagsys/psdiag/main.py
--rw-r--r--   0 runner    (1001) docker     (122)     6705 2023-04-20 19:20:44.000000 siriuspy-2.73.0/siriuspy/diagsys/psdiag/pvs.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-20 19:20:58.800552 siriuspy-2.73.0/siriuspy/diagsys/pudiag/
--rw-r--r--   0 runner    (1001) docker     (122)       25 2023-04-20 19:20:44.000000 siriuspy-2.73.0/siriuspy/diagsys/pudiag/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     1418 2023-04-20 19:20:44.000000 siriuspy-2.73.0/siriuspy/diagsys/pudiag/csdev.py
--rw-r--r--   0 runner    (1001) docker     (122)     2871 2023-04-20 19:20:44.000000 siriuspy-2.73.0/siriuspy/diagsys/pudiag/main.py
--rw-r--r--   0 runner    (1001) docker     (122)     4099 2023-04-20 19:20:44.000000 siriuspy-2.73.0/siriuspy/diagsys/pudiag/pvs.py
--rw-r--r--   0 runner    (1001) docker     (122)     6824 2023-04-20 19:20:44.000000 siriuspy-2.73.0/siriuspy/diagsys/pvs.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-20 19:20:58.800552 siriuspy-2.73.0/siriuspy/diagsys/rfdiag/
--rw-r--r--   0 runner    (1001) docker     (122)       25 2023-04-20 19:20:44.000000 siriuspy-2.73.0/siriuspy/diagsys/rfdiag/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     2409 2023-04-20 19:20:44.000000 siriuspy-2.73.0/siriuspy/diagsys/rfdiag/csdev.py
--rw-r--r--   0 runner    (1001) docker     (122)     3783 2023-04-20 19:20:44.000000 siriuspy-2.73.0/siriuspy/diagsys/rfdiag/main.py
--rw-r--r--   0 runner    (1001) docker     (122)     4891 2023-04-20 19:20:44.000000 siriuspy-2.73.0/siriuspy/diagsys/rfdiag/pvs.py
--rw-r--r--   0 runner    (1001) docker     (122)     2135 2023-04-20 19:20:44.000000 siriuspy-2.73.0/siriuspy/envars.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-20 19:20:58.800552 siriuspy-2.73.0/siriuspy/epics/
--rw-r--r--   0 runner    (1001) docker     (122)      379 2023-04-20 19:20:44.000000 siriuspy-2.73.0/siriuspy/epics/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      624 2023-04-20 19:20:44.000000 siriuspy-2.73.0/siriuspy/epics/multiproc.py
--rw-r--r--   0 runner    (1001) docker     (122)     9097 2023-04-20 19:20:44.000000 siriuspy-2.73.0/siriuspy/epics/properties.py
--rw-r--r--   0 runner    (1001) docker     (122)      209 2023-04-20 19:20:44.000000 siriuspy-2.73.0/siriuspy/epics/pv.py
--rw-r--r--   0 runner    (1001) docker     (122)    29251 2023-04-20 19:20:44.000000 siriuspy-2.73.0/siriuspy/epics/pv_fake.py
--rw-r--r--   0 runner    (1001) docker     (122)     9170 2023-04-20 19:20:44.000000 siriuspy-2.73.0/siriuspy/epics/pv_time_serie.py
--rw-r--r--   0 runner    (1001) docker     (122)      100 2023-04-20 19:20:44.000000 siriuspy-2.73.0/siriuspy/epics/threading.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-20 19:20:58.800552 siriuspy-2.73.0/siriuspy/fofb/
--rw-r--r--   0 runner    (1001) docker     (122)       34 2023-04-20 19:20:44.000000 siriuspy-2.73.0/siriuspy/fofb/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    18873 2023-04-20 19:20:44.000000 siriuspy-2.73.0/siriuspy/fofb/csdev.py
--rw-r--r--   0 runner    (1001) docker     (122)    80150 2023-04-20 19:20:44.000000 siriuspy-2.73.0/siriuspy/fofb/main.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-20 19:20:58.800552 siriuspy-2.73.0/siriuspy/idff/
--rw-r--r--   0 runner    (1001) docker     (122)       44 2023-04-20 19:20:44.000000 siriuspy-2.73.0/siriuspy/idff/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     4539 2023-04-20 19:20:44.000000 siriuspy-2.73.0/siriuspy/idff/config.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-20 19:20:58.800552 siriuspy-2.73.0/siriuspy/injctrl/
--rw-r--r--   0 runner    (1001) docker     (122)       36 2023-04-20 19:20:44.000000 siriuspy-2.73.0/siriuspy/injctrl/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    15244 2023-04-20 19:20:44.000000 siriuspy-2.73.0/siriuspy/injctrl/bias_feedback.py
--rw-r--r--   0 runner    (1001) docker     (122)    26067 2023-04-20 19:20:44.000000 siriuspy-2.73.0/siriuspy/injctrl/csdev.py
--rw-r--r--   0 runner    (1001) docker     (122)    67948 2023-04-20 19:20:44.000000 siriuspy-2.73.0/siriuspy/injctrl/main.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-20 19:20:58.804553 siriuspy-2.73.0/siriuspy/machshift/
--rw-r--r--   0 runner    (1001) docker     (122)       32 2023-04-20 19:20:44.000000 siriuspy-2.73.0/siriuspy/machshift/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     1297 2023-04-20 19:20:44.000000 siriuspy-2.73.0/siriuspy/machshift/csdev.py
--rw-r--r--   0 runner    (1001) docker     (122)    77640 2023-04-20 19:20:44.000000 siriuspy-2.73.0/siriuspy/machshift/macreport.py
--rw-r--r--   0 runner    (1001) docker     (122)     8913 2023-04-20 19:20:44.000000 siriuspy-2.73.0/siriuspy/machshift/macschedule.py
--rw-r--r--   0 runner    (1001) docker     (122)     2237 2023-04-20 19:20:44.000000 siriuspy-2.73.0/siriuspy/machshift/main.py
--rw-r--r--   0 runner    (1001) docker     (122)     5429 2023-04-20 19:20:44.000000 siriuspy-2.73.0/siriuspy/machshift/test_macreport.py
--rw-r--r--   0 runner    (1001) docker     (122)     2012 2023-04-20 19:20:44.000000 siriuspy-2.73.0/siriuspy/machshift/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-20 19:20:58.804553 siriuspy-2.73.0/siriuspy/magnet/
--rw-r--r--   0 runner    (1001) docker     (122)       25 2023-04-20 19:20:44.000000 siriuspy-2.73.0/siriuspy/magnet/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     1126 2023-04-20 19:20:44.000000 siriuspy-2.73.0/siriuspy/magnet/data.py
--rw-r--r--   0 runner    (1001) docker     (122)     8736 2023-04-20 19:20:44.000000 siriuspy-2.73.0/siriuspy/magnet/excdata.py
--rw-r--r--   0 runner    (1001) docker     (122)     1390 2023-04-20 19:20:44.000000 siriuspy-2.73.0/siriuspy/magnet/factory.py
--rw-r--r--   0 runner    (1001) docker     (122)    15453 2023-04-20 19:20:44.000000 siriuspy-2.73.0/siriuspy/magnet/normalizer.py
--rw-r--r--   0 runner    (1001) docker     (122)     7185 2023-04-20 19:20:44.000000 siriuspy-2.73.0/siriuspy/magnet/util.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-20 19:20:58.804553 siriuspy-2.73.0/siriuspy/meas/
--rw-r--r--   0 runner    (1001) docker     (122)       41 2023-04-20 19:20:44.000000 siriuspy-2.73.0/siriuspy/meas/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    11826 2023-04-20 19:20:44.000000 siriuspy-2.73.0/siriuspy/meas/csdev.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-20 19:20:58.804553 siriuspy-2.73.0/siriuspy/meas/liemit/
--rw-r--r--   0 runner    (1001) docker     (122)       57 2023-04-20 19:20:44.000000 siriuspy-2.73.0/siriuspy/meas/liemit/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     1455 2023-04-20 19:20:44.000000 siriuspy-2.73.0/siriuspy/meas/liemit/csdev.py
--rw-r--r--   0 runner    (1001) docker     (122)    13017 2023-04-20 19:20:44.000000 siriuspy-2.73.0/siriuspy/meas/liemit/main.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-20 19:20:58.804553 siriuspy-2.73.0/siriuspy/meas/lienergy/
--rw-r--r--   0 runner    (1001) docker     (122)       80 2023-04-20 19:20:44.000000 siriuspy-2.73.0/siriuspy/meas/lienergy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     2821 2023-04-20 19:20:44.000000 siriuspy-2.73.0/siriuspy/meas/lienergy/csdev.py
--rw-r--r--   0 runner    (1001) docker     (122)     8714 2023-04-20 19:20:44.000000 siriuspy-2.73.0/siriuspy/meas/lienergy/main.py
--rw-r--r--   0 runner    (1001) docker     (122)    25137 2023-04-20 19:20:44.000000 siriuspy-2.73.0/siriuspy/meas/util.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-20 19:20:58.804553 siriuspy-2.73.0/siriuspy/namesys/
--rw-r--r--   0 runner    (1001) docker     (122)       82 2023-04-20 19:20:44.000000 siriuspy-2.73.0/siriuspy/namesys/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    15210 2023-04-20 19:20:44.000000 siriuspy-2.73.0/siriuspy/namesys/implementation.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-20 19:20:58.804553 siriuspy-2.73.0/siriuspy/optics/
--rw-r--r--   0 runner    (1001) docker     (122)       25 2023-04-20 19:20:44.000000 siriuspy-2.73.0/siriuspy/optics/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      363 2023-04-20 19:20:44.000000 siriuspy-2.73.0/siriuspy/optics/constants.py
--rw-r--r--   0 runner    (1001) docker     (122)     6906 2023-04-20 19:20:44.000000 siriuspy-2.73.0/siriuspy/optics/lattice_survey.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-20 19:20:58.804553 siriuspy-2.73.0/siriuspy/opticscorr/
--rw-r--r--   0 runner    (1001) docker     (122)       29 2023-04-20 19:20:44.000000 siriuspy-2.73.0/siriuspy/opticscorr/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    34878 2023-04-20 19:20:44.000000 siriuspy-2.73.0/siriuspy/opticscorr/base.py
--rw-r--r--   0 runner    (1001) docker     (122)    16096 2023-04-20 19:20:44.000000 siriuspy-2.73.0/siriuspy/opticscorr/chrom.py
--rw-r--r--   0 runner    (1001) docker     (122)    13454 2023-04-20 19:20:44.000000 siriuspy-2.73.0/siriuspy/opticscorr/csdev.py
--rw-r--r--   0 runner    (1001) docker     (122)    18765 2023-04-20 19:20:44.000000 siriuspy-2.73.0/siriuspy/opticscorr/opticscorr.py
--rw-r--r--   0 runner    (1001) docker     (122)     8006 2023-04-20 19:20:44.000000 siriuspy-2.73.0/siriuspy/opticscorr/tune.py
--rw-r--r--   0 runner    (1001) docker     (122)     1846 2023-04-20 19:20:44.000000 siriuspy-2.73.0/siriuspy/opticscorr/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-20 19:20:58.808554 siriuspy-2.73.0/siriuspy/oscilloscope/
--rw-r--r--   0 runner    (1001) docker     (122)      104 2023-04-20 19:20:44.000000 siriuspy-2.73.0/siriuspy/oscilloscope/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     6544 2023-04-20 19:20:44.000000 siriuspy-2.73.0/siriuspy/oscilloscope/keysight.py
--rw-r--r--   0 runner    (1001) docker     (122)     1180 2023-04-20 19:20:44.000000 siriuspy-2.73.0/siriuspy/oscilloscope/scopes.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-20 19:20:58.808554 siriuspy-2.73.0/siriuspy/posang/
--rw-r--r--   0 runner    (1001) docker     (122)       25 2023-04-20 19:20:44.000000 siriuspy-2.73.0/siriuspy/posang/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     4935 2023-04-20 19:20:44.000000 siriuspy-2.73.0/siriuspy/posang/csdev.py
--rw-r--r--   0 runner    (1001) docker     (122)    19747 2023-04-20 19:20:44.000000 siriuspy-2.73.0/siriuspy/posang/main.py
--rw-r--r--   0 runner    (1001) docker     (122)     1678 2023-04-20 19:20:44.000000 siriuspy-2.73.0/siriuspy/posang/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-20 19:20:58.808554 siriuspy-2.73.0/siriuspy/pwrsupply/
--rw-r--r--   0 runner    (1001) docker     (122)      132 2023-04-20 19:20:44.000000 siriuspy-2.73.0/siriuspy/pwrsupply/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     8950 2023-04-20 19:20:44.000000 siriuspy-2.73.0/siriuspy/pwrsupply/beaglebone.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-20 19:20:58.808554 siriuspy-2.73.0/siriuspy/pwrsupply/bsmp/
--rw-r--r--   0 runner    (1001) docker     (122)       48 2023-04-20 19:20:44.000000 siriuspy-2.73.0/siriuspy/pwrsupply/bsmp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    25156 2023-04-20 19:20:44.000000 siriuspy-2.73.0/siriuspy/pwrsupply/bsmp/commands.py
--rw-r--r--   0 runner    (1001) docker     (122)    19464 2023-04-20 19:20:44.000000 siriuspy-2.73.0/siriuspy/pwrsupply/bsmp/constants.py
--rw-r--r--   0 runner    (1001) docker     (122)    53763 2023-04-20 19:20:44.000000 siriuspy-2.73.0/siriuspy/pwrsupply/bsmp/entities.py
--rw-r--r--   0 runner    (1001) docker     (122)      850 2023-04-20 19:20:44.000000 siriuspy-2.73.0/siriuspy/pwrsupply/bsmp/factory.py
--rw-r--r--   0 runner    (1001) docker     (122)   150426 2023-04-20 19:20:44.000000 siriuspy-2.73.0/siriuspy/pwrsupply/csdev.py
--rw-r--r--   0 runner    (1001) docker     (122)     3624 2023-04-20 19:20:44.000000 siriuspy-2.73.0/siriuspy/pwrsupply/data.py
--rw-r--r--   0 runner    (1001) docker     (122)    10620 2023-04-20 19:20:44.000000 siriuspy-2.73.0/siriuspy/pwrsupply/factory.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-20 19:20:58.808554 siriuspy-2.73.0/siriuspy/pwrsupply/pructrl/
--rw-r--r--   0 runner    (1001) docker     (122)      841 2023-04-20 19:20:44.000000 siriuspy-2.73.0/siriuspy/pwrsupply/pructrl/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     3393 2023-04-20 19:20:44.000000 siriuspy-2.73.0/siriuspy/pwrsupply/pructrl/pru.py
--rw-r--r--   0 runner    (1001) docker     (122)    26340 2023-04-20 19:20:44.000000 siriuspy-2.73.0/siriuspy/pwrsupply/pructrl/prucontroller.py
--rw-r--r--   0 runner    (1001) docker     (122)     6133 2023-04-20 19:20:44.000000 siriuspy-2.73.0/siriuspy/pwrsupply/pructrl/prucparms.py
--rw-r--r--   0 runner    (1001) docker     (122)    10280 2023-04-20 19:20:44.000000 siriuspy-2.73.0/siriuspy/pwrsupply/pructrl/psdevstate.py
--rw-r--r--   0 runner    (1001) docker     (122)     7712 2023-04-20 19:20:44.000000 siriuspy-2.73.0/siriuspy/pwrsupply/pructrl/udc.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-20 19:20:58.808554 siriuspy-2.73.0/siriuspy/pwrsupply/psctrl/
--rw-r--r--   0 runner    (1001) docker     (122)      866 2023-04-20 19:20:44.000000 siriuspy-2.73.0/siriuspy/pwrsupply/psctrl/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     7884 2023-04-20 19:20:44.000000 siriuspy-2.73.0/siriuspy/pwrsupply/psctrl/pscontroller.py
--rw-r--r--   0 runner    (1001) docker     (122)     6262 2023-04-20 19:20:44.000000 siriuspy-2.73.0/siriuspy/pwrsupply/psctrl/pscreaders.py
--rw-r--r--   0 runner    (1001) docker     (122)     5502 2023-04-20 19:20:44.000000 siriuspy-2.73.0/siriuspy/pwrsupply/psctrl/pscstatus.py
--rw-r--r--   0 runner    (1001) docker     (122)    17064 2023-04-20 19:20:44.000000 siriuspy-2.73.0/siriuspy/pwrsupply/psctrl/pscwriters.py
--rw-r--r--   0 runner    (1001) docker     (122)    42124 2023-04-20 19:20:44.000000 siriuspy-2.73.0/siriuspy/pwrsupply/psctrl/psmodel.py
--rw-r--r--   0 runner    (1001) docker     (122)    33182 2023-04-20 19:20:44.000000 siriuspy-2.73.0/siriuspy/pwrsupply/pssofb.py
--rw-r--r--   0 runner    (1001) docker     (122)    12500 2023-04-20 19:20:44.000000 siriuspy-2.73.0/siriuspy/pwrsupply/siggen.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-20 19:20:58.816555 siriuspy-2.73.0/siriuspy/ramp/
--rw-r--r--   0 runner    (1001) docker     (122)       23 2023-04-20 19:20:44.000000 siriuspy-2.73.0/siriuspy/ramp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    28999 2023-04-20 19:20:44.000000 siriuspy-2.73.0/siriuspy/ramp/conn.py
--rw-r--r--   0 runner    (1001) docker     (122)      346 2023-04-20 19:20:44.000000 siriuspy-2.73.0/siriuspy/ramp/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (122)     3969 2023-04-20 19:20:44.000000 siriuspy-2.73.0/siriuspy/ramp/magnet.py
--rw-r--r--   0 runner    (1001) docker     (122)    45093 2023-04-20 19:20:44.000000 siriuspy-2.73.0/siriuspy/ramp/ramp.py
--rw-r--r--   0 runner    (1001) docker     (122)    29333 2023-04-20 19:20:44.000000 siriuspy-2.73.0/siriuspy/ramp/reconst_factory.py
--rwxr-xr-x   0 runner    (1001) docker     (122)     6985 2023-04-20 19:20:44.000000 siriuspy-2.73.0/siriuspy/ramp/test_reconst_factory.py
--rwxr-xr-x   0 runner    (1001) docker     (122)     4158 2023-04-20 19:20:44.000000 siriuspy-2.73.0/siriuspy/ramp/testwfm.py
--rw-r--r--   0 runner    (1001) docker     (122)     5584 2023-04-20 19:20:44.000000 siriuspy-2.73.0/siriuspy/ramp/util.py
--rw-r--r--   0 runner    (1001) docker     (122)    30145 2023-04-20 19:20:44.000000 siriuspy-2.73.0/siriuspy/ramp/waveform.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-20 19:20:58.820555 siriuspy-2.73.0/siriuspy/search/
--rw-r--r--   0 runner    (1001) docker     (122)      359 2023-04-20 19:20:44.000000 siriuspy-2.73.0/siriuspy/search/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     3537 2023-04-20 19:20:44.000000 siriuspy-2.73.0/siriuspy/search/bpms_search.py
--rw-r--r--   0 runner    (1001) docker     (122)     6612 2023-04-20 19:20:44.000000 siriuspy-2.73.0/siriuspy/search/hl_time_search.py
--rw-r--r--   0 runner    (1001) docker     (122)     4499 2023-04-20 19:20:44.000000 siriuspy-2.73.0/siriuspy/search/id_search.py
--rw-r--r--   0 runner    (1001) docker     (122)     4152 2023-04-20 19:20:44.000000 siriuspy-2.73.0/siriuspy/search/ioc_search.py
--rw-r--r--   0 runner    (1001) docker     (122)    16917 2023-04-20 19:20:44.000000 siriuspy-2.73.0/siriuspy/search/ll_time_search.py
--rw-r--r--   0 runner    (1001) docker     (122)     7219 2023-04-20 19:20:44.000000 siriuspy-2.73.0/siriuspy/search/ma_search.py
--rw-r--r--   0 runner    (1001) docker     (122)    23882 2023-04-20 19:20:44.000000 siriuspy-2.73.0/siriuspy/search/ps_search.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-20 19:20:58.824556 siriuspy-2.73.0/siriuspy/simul/
--rw-r--r--   0 runner    (1001) docker     (122)      311 2023-04-20 19:20:44.000000 siriuspy-2.73.0/siriuspy/simul/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     2202 2023-04-20 19:20:44.000000 siriuspy-2.73.0/siriuspy/simul/simfactory.py
--rw-r--r--   0 runner    (1001) docker     (122)     6298 2023-04-20 19:20:44.000000 siriuspy-2.73.0/siriuspy/simul/simps.py
--rw-r--r--   0 runner    (1001) docker     (122)     2324 2023-04-20 19:20:44.000000 siriuspy-2.73.0/siriuspy/simul/simpv.py
--rw-r--r--   0 runner    (1001) docker     (122)     7391 2023-04-20 19:20:44.000000 siriuspy-2.73.0/siriuspy/simul/simulation.py
--rw-r--r--   0 runner    (1001) docker     (122)     4266 2023-04-20 19:20:44.000000 siriuspy-2.73.0/siriuspy/simul/simulator.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-20 19:20:58.828556 siriuspy-2.73.0/siriuspy/sofb/
--rw-r--r--   0 runner    (1001) docker     (122)       78 2023-04-20 19:20:44.000000 siriuspy-2.73.0/siriuspy/sofb/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     4646 2023-04-20 19:20:44.000000 siriuspy-2.73.0/siriuspy/sofb/base_class.py
--rw-r--r--   0 runner    (1001) docker     (122)    28072 2023-04-20 19:20:44.000000 siriuspy-2.73.0/siriuspy/sofb/bpms.py
--rw-r--r--   0 runner    (1001) docker     (122)    32149 2023-04-20 19:20:44.000000 siriuspy-2.73.0/siriuspy/sofb/correctors.py
--rw-r--r--   0 runner    (1001) docker     (122)    47045 2023-04-20 19:20:44.000000 siriuspy-2.73.0/siriuspy/sofb/csdev.py
--rw-r--r--   0 runner    (1001) docker     (122)    45797 2023-04-20 19:20:44.000000 siriuspy-2.73.0/siriuspy/sofb/main.py
--rw-r--r--   0 runner    (1001) docker     (122)    12220 2023-04-20 19:20:44.000000 siriuspy-2.73.0/siriuspy/sofb/matrix.py
--rw-r--r--   0 runner    (1001) docker     (122)    39653 2023-04-20 19:20:44.000000 siriuspy-2.73.0/siriuspy/sofb/orbit.py
--rw-r--r--   0 runner    (1001) docker     (122)     3030 2023-04-20 19:20:44.000000 siriuspy-2.73.0/siriuspy/sofb/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-20 19:20:58.832557 siriuspy-2.73.0/siriuspy/stabinfo/
--rw-r--r--   0 runner    (1001) docker     (122)       38 2023-04-20 19:20:44.000000 siriuspy-2.73.0/siriuspy/stabinfo/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     3558 2023-04-20 19:20:44.000000 siriuspy-2.73.0/siriuspy/stabinfo/csdev.py
--rw-r--r--   0 runner    (1001) docker     (122)     7708 2023-04-20 19:20:44.000000 siriuspy-2.73.0/siriuspy/stabinfo/main.py
--rw-r--r--   0 runner    (1001) docker     (122)     8093 2023-04-20 19:20:44.000000 siriuspy-2.73.0/siriuspy/thread.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-20 19:20:58.832557 siriuspy-2.73.0/siriuspy/timesys/
--rw-r--r--   0 runner    (1001) docker     (122)       26 2023-04-20 19:20:44.000000 siriuspy-2.73.0/siriuspy/timesys/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    20220 2023-04-20 19:20:44.000000 siriuspy-2.73.0/siriuspy/timesys/csdev.py
--rw-r--r--   0 runner    (1001) docker     (122)    12705 2023-04-20 19:20:44.000000 siriuspy-2.73.0/siriuspy/timesys/hl_classes.py
--rw-r--r--   0 runner    (1001) docker     (122)    33256 2023-04-20 19:20:44.000000 siriuspy-2.73.0/siriuspy/timesys/ll_classes.py
--rw-r--r--   0 runner    (1001) docker     (122)     6015 2023-04-20 19:20:44.000000 siriuspy-2.73.0/siriuspy/timesys/plot_network.py
--rw-r--r--   0 runner    (1001) docker     (122)     5957 2023-04-20 19:20:44.000000 siriuspy-2.73.0/siriuspy/timesys/static_table.py
--rw-r--r--   0 runner    (1001) docker     (122)     8732 2023-04-20 19:20:44.000000 siriuspy-2.73.0/siriuspy/util.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-20 19:20:58.784550 siriuspy-2.73.0/siriuspy.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)     1423 2023-04-20 19:20:58.000000 siriuspy-2.73.0/siriuspy.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     9900 2023-04-20 19:20:58.000000 siriuspy-2.73.0/siriuspy.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-04-20 19:20:58.000000 siriuspy-2.73.0/siriuspy.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-04-20 19:20:58.000000 siriuspy-2.73.0/siriuspy.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (122)      128 2023-04-20 19:20:58.000000 siriuspy-2.73.0/siriuspy.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)       15 2023-04-20 19:20:58.000000 siriuspy-2.73.0/siriuspy.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-20 19:20:58.836557 siriuspy-2.73.0/tests/
--rw-r--r--   0 runner    (1001) docker     (122)      441 2023-04-20 19:20:44.000000 siriuspy-2.73.0/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-20 19:20:58.840558 siriuspy-2.73.0/tests/bsmp/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-20 19:20:44.000000 siriuspy-2.73.0/tests/bsmp/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (122)     5698 2023-04-20 19:20:44.000000 siriuspy-2.73.0/tests/bsmp/test_bsmp.py
--rwxr-xr-x   0 runner    (1001) docker     (122)    14788 2023-04-20 19:20:44.000000 siriuspy-2.73.0/tests/bsmp/test_commands.py
--rwxr-xr-x   0 runner    (1001) docker     (122)    13382 2023-04-20 19:20:44.000000 siriuspy-2.73.0/tests/bsmp/test_entities.py
--rwxr-xr-x   0 runner    (1001) docker     (122)     7719 2023-04-20 19:20:44.000000 siriuspy-2.73.0/tests/bsmp/test_serial.py
--rwxr-xr-x   0 runner    (1001) docker     (122)     1837 2023-04-20 19:20:44.000000 siriuspy-2.73.0/tests/bsmp/test_types.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-20 19:20:58.840558 siriuspy-2.73.0/tests/clientconfigdb/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-20 19:20:44.000000 siriuspy-2.73.0/tests/clientconfigdb/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (122)     2843 2023-04-20 19:20:44.000000 siriuspy-2.73.0/tests/clientconfigdb/test_configdb_client.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-20 19:20:58.840558 siriuspy-2.73.0/tests/clientweb/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-20 19:20:44.000000 siriuspy-2.73.0/tests/clientweb/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (122)    11633 2023-04-20 19:20:44.000000 siriuspy-2.73.0/tests/clientweb/test_implementation.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-20 19:20:58.840558 siriuspy-2.73.0/tests/currinfo/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-20 19:20:44.000000 siriuspy-2.73.0/tests/currinfo/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-20 19:20:58.840558 siriuspy-2.73.0/tests/currinfo/lifetime/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-20 19:20:44.000000 siriuspy-2.73.0/tests/currinfo/lifetime/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (122)     1908 2023-04-20 19:20:44.000000 siriuspy-2.73.0/tests/currinfo/lifetime/test_main.py
--rwxr-xr-x   0 runner    (1001) docker     (122)     6495 2023-04-20 19:20:44.000000 siriuspy-2.73.0/tests/currinfo/test_csdev.py
--rwxr-xr-x   0 runner    (1001) docker     (122)     2653 2023-04-20 19:20:44.000000 siriuspy-2.73.0/tests/currinfo/test_main.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-20 19:20:58.840558 siriuspy-2.73.0/tests/magnet/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-20 19:20:44.000000 siriuspy-2.73.0/tests/magnet/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (122)     2275 2023-04-20 19:20:44.000000 siriuspy-2.73.0/tests/magnet/test_factory.py
--rwxr-xr-x   0 runner    (1001) docker     (122)     2687 2023-04-20 19:20:44.000000 siriuspy-2.73.0/tests/magnet/tests_normalizer.py
--rwxr-xr-x   0 runner    (1001) docker     (122)     3618 2023-04-20 19:20:44.000000 siriuspy-2.73.0/tests/mock_servweb.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-20 19:20:58.840558 siriuspy-2.73.0/tests/namesys/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-20 19:20:44.000000 siriuspy-2.73.0/tests/namesys/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (122)     4896 2023-04-20 19:20:44.000000 siriuspy-2.73.0/tests/namesys/test_implementation.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-20 19:20:58.844559 siriuspy-2.73.0/tests/opticscorr/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-20 19:20:44.000000 siriuspy-2.73.0/tests/opticscorr/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     5490 2023-04-20 19:20:44.000000 siriuspy-2.73.0/tests/opticscorr/test_chrom.py
--rwxr-xr-x   0 runner    (1001) docker     (122)     4609 2023-04-20 19:20:44.000000 siriuspy-2.73.0/tests/opticscorr/test_csdev.py
--rwxr-xr-x   0 runner    (1001) docker     (122)    23381 2023-04-20 19:20:44.000000 siriuspy-2.73.0/tests/opticscorr/test_opticscorr.py
--rw-r--r--   0 runner    (1001) docker     (122)     5692 2023-04-20 19:20:44.000000 siriuspy-2.73.0/tests/opticscorr/test_tune.py
--rw-r--r--   0 runner    (1001) docker     (122)     1145 2023-04-20 19:20:44.000000 siriuspy-2.73.0/tests/opticscorr/test_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-20 19:20:58.844559 siriuspy-2.73.0/tests/posang/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-20 19:20:44.000000 siriuspy-2.73.0/tests/posang/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (122)     2872 2023-04-20 19:20:44.000000 siriuspy-2.73.0/tests/posang/test_csdev.py
--rwxr-xr-x   0 runner    (1001) docker     (122)     3164 2023-04-20 19:20:44.000000 siriuspy-2.73.0/tests/posang/test_main.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-20 19:20:58.844559 siriuspy-2.73.0/tests/pwrsupply/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-20 19:20:44.000000 siriuspy-2.73.0/tests/pwrsupply/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    18979 2023-04-20 19:20:44.000000 siriuspy-2.73.0/tests/pwrsupply/db.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-20 19:20:58.848559 siriuspy-2.73.0/tests/pwrsupply/pructrl/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-20 19:20:44.000000 siriuspy-2.73.0/tests/pwrsupply/pructrl/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (122)     2257 2023-04-20 19:20:44.000000 siriuspy-2.73.0/tests/pwrsupply/pructrl/test_pru.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-20 19:20:58.848559 siriuspy-2.73.0/tests/pwrsupply/psctrl/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-20 19:20:44.000000 siriuspy-2.73.0/tests/pwrsupply/psctrl/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     4853 2023-04-20 19:20:44.000000 siriuspy-2.73.0/tests/pwrsupply/psctrl/test_pscwriters.py
--rwxr-xr-x   0 runner    (1001) docker     (122)      166 2023-04-20 19:20:44.000000 siriuspy-2.73.0/tests/pwrsupply/test_beaglebone.py
--rwxr-xr-x   0 runner    (1001) docker     (122)       89 2023-04-20 19:20:44.000000 siriuspy-2.73.0/tests/pwrsupply/test_bsmp.py
--rwxr-xr-x   0 runner    (1001) docker     (122)     6439 2023-04-20 19:20:44.000000 siriuspy-2.73.0/tests/pwrsupply/test_csdev.py
--rwxr-xr-x   0 runner    (1001) docker     (122)     7331 2023-04-20 19:20:44.000000 siriuspy-2.73.0/tests/pwrsupply/test_data.py
--rwxr-xr-x   0 runner    (1001) docker     (122)     2323 2023-04-20 19:20:44.000000 siriuspy-2.73.0/tests/pwrsupply/test_siggen.py
--rw-r--r--   0 runner    (1001) docker     (122)     3146 2023-04-20 19:20:44.000000 siriuspy-2.73.0/tests/pwrsupply/variables.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-20 19:20:58.848559 siriuspy-2.73.0/tests/ramp/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-20 19:20:44.000000 siriuspy-2.73.0/tests/ramp/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (122)     5699 2023-04-20 19:20:44.000000 siriuspy-2.73.0/tests/ramp/test_magnet.py
--rwxr-xr-x   0 runner    (1001) docker     (122)     7235 2023-04-20 19:20:44.000000 siriuspy-2.73.0/tests/ramp/test_waveform.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-20 19:20:58.848559 siriuspy-2.73.0/tests/search/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-20 19:20:44.000000 siriuspy-2.73.0/tests/search/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (122)     2412 2023-04-20 19:20:44.000000 siriuspy-2.73.0/tests/search/test_hl_time_search.py
--rwxr-xr-x   0 runner    (1001) docker     (122)      559 2023-04-20 19:20:44.000000 siriuspy-2.73.0/tests/search/test_init.py
--rwxr-xr-x   0 runner    (1001) docker     (122)     3831 2023-04-20 19:20:44.000000 siriuspy-2.73.0/tests/search/test_ll_time_search.py
--rwxr-xr-x   0 runner    (1001) docker     (122)     6120 2023-04-20 19:20:44.000000 siriuspy-2.73.0/tests/search/test_ma_search.py
--rwxr-xr-x   0 runner    (1001) docker     (122)    13502 2023-04-20 19:20:44.000000 siriuspy-2.73.0/tests/search/test_ps_search.py
--rw-r--r--   0 runner    (1001) docker     (122)     3478 2023-04-20 19:20:44.000000 siriuspy-2.73.0/tests/test_callbacks.py
--rwxr-xr-x   0 runner    (1001) docker     (122)     1009 2023-04-20 19:20:44.000000 siriuspy-2.73.0/tests/test_csdev.py
--rwxr-xr-x   0 runner    (1001) docker     (122)     1605 2023-04-20 19:20:44.000000 siriuspy-2.73.0/tests/test_envars.py
--rwxr-xr-x   0 runner    (1001) docker     (122)    11533 2023-04-20 19:20:44.000000 siriuspy-2.73.0/tests/test_util.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-20 19:20:58.848559 siriuspy-2.73.0/tests/timesys/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-20 19:20:44.000000 siriuspy-2.73.0/tests/timesys/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (122)     4999 2023-04-20 19:20:44.000000 siriuspy-2.73.0/tests/timesys/test_csdev.py
--rw-r--r--   0 runner    (1001) docker     (122)      978 2023-04-20 19:20:44.000000 siriuspy-2.73.0/tests/timesys/test_plot_network.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-15 11:31:28.751122 siriuspy-2.74.0/
+-rw-r--r--   0 runner    (1001) docker     (122)    34494 2023-05-15 11:31:13.000000 siriuspy-2.74.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (122)       90 2023-05-15 11:31:13.000000 siriuspy-2.74.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (122)     1423 2023-05-15 11:31:28.751122 siriuspy-2.74.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)      954 2023-05-15 11:31:13.000000 siriuspy-2.74.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (122)      128 2023-05-15 11:31:13.000000 siriuspy-2.74.0/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       38 2023-05-15 11:31:28.751122 siriuspy-2.74.0/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (122)     1243 2023-05-15 11:31:13.000000 siriuspy-2.74.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-15 11:31:28.715121 siriuspy-2.74.0/siriuspy/
+-rw-r--r--   0 runner    (1001) docker     (122)        7 2023-05-15 11:31:13.000000 siriuspy-2.74.0/siriuspy/VERSION
+-rw-r--r--   0 runner    (1001) docker     (122)      497 2023-05-15 11:31:13.000000 siriuspy-2.74.0/siriuspy/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-15 11:31:28.715121 siriuspy-2.74.0/siriuspy/bsmp/
+-rw-r--r--   0 runner    (1001) docker     (122)      422 2023-05-15 11:31:13.000000 siriuspy-2.74.0/siriuspy/bsmp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    15885 2023-05-15 11:31:13.000000 siriuspy-2.74.0/siriuspy/bsmp/commands.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1904 2023-05-15 11:31:13.000000 siriuspy-2.74.0/siriuspy/bsmp/constants.py
+-rw-r--r--   0 runner    (1001) docker     (122)    11790 2023-05-15 11:31:13.000000 siriuspy-2.74.0/siriuspy/bsmp/entities.py
+-rw-r--r--   0 runner    (1001) docker     (122)      610 2023-05-15 11:31:13.000000 siriuspy-2.74.0/siriuspy/bsmp/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (122)     8110 2023-05-15 11:31:13.000000 siriuspy-2.74.0/siriuspy/bsmp/serial.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1204 2023-05-15 11:31:13.000000 siriuspy-2.74.0/siriuspy/bsmp/types.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2992 2023-05-15 11:31:13.000000 siriuspy-2.74.0/siriuspy/callbacks.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-15 11:31:28.715121 siriuspy-2.74.0/siriuspy/clientarch/
+-rw-r--r--   0 runner    (1001) docker     (122)      306 2023-05-15 11:31:13.000000 siriuspy-2.74.0/siriuspy/clientarch/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    13813 2023-05-15 11:31:13.000000 siriuspy-2.74.0/siriuspy/clientarch/client.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6392 2023-05-15 11:31:13.000000 siriuspy-2.74.0/siriuspy/clientarch/devices.py
+-rw-r--r--   0 runner    (1001) docker     (122)      643 2023-05-15 11:31:13.000000 siriuspy-2.74.0/siriuspy/clientarch/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (122)    20400 2023-05-15 11:31:13.000000 siriuspy-2.74.0/siriuspy/clientarch/pvarch.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5003 2023-05-15 11:31:13.000000 siriuspy-2.74.0/siriuspy/clientarch/time.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-15 11:31:28.715121 siriuspy-2.74.0/siriuspy/clientconfigdb/
+-rw-r--r--   0 runner    (1001) docker     (122)      227 2023-05-15 11:31:13.000000 siriuspy-2.74.0/siriuspy/clientconfigdb/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3535 2023-05-15 11:31:13.000000 siriuspy-2.74.0/siriuspy/clientconfigdb/_templates.py
+-rw-r--r--   0 runner    (1001) docker     (122)     9599 2023-05-15 11:31:13.000000 siriuspy-2.74.0/siriuspy/clientconfigdb/configdb_client.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5448 2023-05-15 11:31:13.000000 siriuspy-2.74.0/siriuspy/clientconfigdb/configdb_document.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4785 2023-05-15 11:31:13.000000 siriuspy-2.74.0/siriuspy/clientconfigdb/pvsconfig.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-15 11:31:28.719121 siriuspy-2.74.0/siriuspy/clientconfigdb/types/
+-rw-r--r--   0 runner    (1001) docker     (122)      286 2023-05-15 11:31:13.000000 siriuspy-2.74.0/siriuspy/clientconfigdb/types/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    13746 2023-05-15 11:31:13.000000 siriuspy-2.74.0/siriuspy/clientconfigdb/types/as_corrloop_params.py
+-rw-r--r--   0 runner    (1001) docker     (122)    57636 2023-05-15 11:31:13.000000 siriuspy-2.74.0/siriuspy/clientconfigdb/types/as_diagnostics.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6681 2023-05-15 11:31:13.000000 siriuspy-2.74.0/siriuspy/clientconfigdb/types/as_pwrstate.py
+-rw-r--r--   0 runner    (1001) docker     (122)    34247 2023-05-15 11:31:13.000000 siriuspy-2.74.0/siriuspy/clientconfigdb/types/as_rf.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1135 2023-05-15 11:31:13.000000 siriuspy-2.74.0/siriuspy/clientconfigdb/types/bo_chromcorr_params.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3984 2023-05-15 11:31:13.000000 siriuspy-2.74.0/siriuspy/clientconfigdb/types/bo_normalized.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1135 2023-05-15 11:31:13.000000 siriuspy-2.74.0/siriuspy/clientconfigdb/types/bo_orbcorr_respm.py
+-rw-r--r--   0 runner    (1001) docker     (122)      700 2023-05-15 11:31:13.000000 siriuspy-2.74.0/siriuspy/clientconfigdb/types/bo_orbit.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3042 2023-05-15 11:31:13.000000 siriuspy-2.74.0/siriuspy/clientconfigdb/types/bo_ramp.py
+-rw-r--r--   0 runner    (1001) docker     (122)      975 2023-05-15 11:31:13.000000 siriuspy-2.74.0/siriuspy/clientconfigdb/types/bo_tunecorr_params.py
+-rw-r--r--   0 runner    (1001) docker     (122)   122432 2023-05-15 11:31:13.000000 siriuspy-2.74.0/siriuspy/clientconfigdb/types/global_config.py
+-rw-r--r--   0 runner    (1001) docker     (122)      735 2023-05-15 11:31:13.000000 siriuspy-2.74.0/siriuspy/clientconfigdb/types/si_bbadata.py
+-rw-r--r--   0 runner    (1001) docker     (122)    18619 2023-05-15 11:31:13.000000 siriuspy-2.74.0/siriuspy/clientconfigdb/types/si_bbbproc.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1697 2023-05-15 11:31:13.000000 siriuspy-2.74.0/siriuspy/clientconfigdb/types/si_chromcorr_params.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1146 2023-05-15 11:31:13.000000 siriuspy-2.74.0/siriuspy/clientconfigdb/types/si_fastorbcorr_respm.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4741 2023-05-15 11:31:13.000000 siriuspy-2.74.0/siriuspy/clientconfigdb/types/si_fofb.py
+-rw-r--r--   0 runner    (1001) docker     (122)      957 2023-05-15 11:31:13.000000 siriuspy-2.74.0/siriuspy/clientconfigdb/types/si_id.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3181 2023-05-15 11:31:13.000000 siriuspy-2.74.0/siriuspy/clientconfigdb/types/si_idff.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1136 2023-05-15 11:31:13.000000 siriuspy-2.74.0/siriuspy/clientconfigdb/types/si_orbcorr_respm.py
+-rw-r--r--   0 runner    (1001) docker     (122)      701 2023-05-15 11:31:13.000000 siriuspy-2.74.0/siriuspy/clientconfigdb/types/si_orbit.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1290 2023-05-15 11:31:13.000000 siriuspy-2.74.0/siriuspy/clientconfigdb/types/si_tunecorr_params.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1738 2023-05-15 11:31:13.000000 siriuspy-2.74.0/siriuspy/clientconfigdb/types/tb_normalized.py
+-rw-r--r--   0 runner    (1001) docker     (122)      969 2023-05-15 11:31:13.000000 siriuspy-2.74.0/siriuspy/clientconfigdb/types/tb_orbcorr_respm.py
+-rw-r--r--   0 runner    (1001) docker     (122)      693 2023-05-15 11:31:13.000000 siriuspy-2.74.0/siriuspy/clientconfigdb/types/tb_orbit.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1651 2023-05-15 11:31:13.000000 siriuspy-2.74.0/siriuspy/clientconfigdb/types/tb_posang_respm.py
+-rw-r--r--   0 runner    (1001) docker     (122)      969 2023-05-15 11:31:13.000000 siriuspy-2.74.0/siriuspy/clientconfigdb/types/ts_orbcorr_respm.py
+-rw-r--r--   0 runner    (1001) docker     (122)      693 2023-05-15 11:31:13.000000 siriuspy-2.74.0/siriuspy/clientconfigdb/types/ts_orbit.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1721 2023-05-15 11:31:13.000000 siriuspy-2.74.0/siriuspy/clientconfigdb/types/ts_posang_respm.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-15 11:31:28.719121 siriuspy-2.74.0/siriuspy/clientweb/
+-rw-r--r--   0 runner    (1001) docker     (122)       50 2023-05-15 11:31:13.000000 siriuspy-2.74.0/siriuspy/clientweb/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5896 2023-05-15 11:31:13.000000 siriuspy-2.74.0/siriuspy/clientweb/implementation.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2236 2023-05-15 11:31:13.000000 siriuspy-2.74.0/siriuspy/csdev.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-15 11:31:28.719121 siriuspy-2.74.0/siriuspy/currinfo/
+-rw-r--r--   0 runner    (1001) docker     (122)      144 2023-05-15 11:31:13.000000 siriuspy-2.74.0/siriuspy/currinfo/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     9620 2023-05-15 11:31:13.000000 siriuspy-2.74.0/siriuspy/currinfo/csdev.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-15 11:31:28.719121 siriuspy-2.74.0/siriuspy/currinfo/lifetime/
+-rw-r--r--   0 runner    (1001) docker     (122)       72 2023-05-15 11:31:13.000000 siriuspy-2.74.0/siriuspy/currinfo/lifetime/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    12607 2023-05-15 11:31:13.000000 siriuspy-2.74.0/siriuspy/currinfo/lifetime/main.py
+-rw-r--r--   0 runner    (1001) docker     (122)    23275 2023-05-15 11:31:13.000000 siriuspy-2.74.0/siriuspy/currinfo/main.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-15 11:31:28.723122 siriuspy-2.74.0/siriuspy/cycle/
+-rw-r--r--   0 runner    (1001) docker     (122)      514 2023-05-15 11:31:13.000000 siriuspy-2.74.0/siriuspy/cycle/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)   104994 2023-05-15 11:31:13.000000 siriuspy-2.74.0/siriuspy/cycle/bo_cycle_data.py
+-rw-r--r--   0 runner    (1001) docker     (122)    31135 2023-05-15 11:31:13.000000 siriuspy-2.74.0/siriuspy/cycle/conn.py
+-rw-r--r--   0 runner    (1001) docker     (122)     9781 2023-05-15 11:31:13.000000 siriuspy-2.74.0/siriuspy/cycle/fc_cycle_data.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3286 2023-05-15 11:31:13.000000 siriuspy-2.74.0/siriuspy/cycle/li_cycle_data.py
+-rw-r--r--   0 runner    (1001) docker     (122)    38408 2023-05-15 11:31:13.000000 siriuspy-2.74.0/siriuspy/cycle/main.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3567 2023-05-15 11:31:13.000000 siriuspy-2.74.0/siriuspy/cycle/util.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-15 11:31:28.727121 siriuspy-2.74.0/siriuspy/devices/
+-rw-r--r--   0 runner    (1001) docker     (122)     1696 2023-05-15 11:31:13.000000 siriuspy-2.74.0/siriuspy/devices/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    48546 2023-05-15 11:31:13.000000 siriuspy-2.74.0/siriuspy/devices/bbb.py
+-rw-r--r--   0 runner    (1001) docker     (122)    41443 2023-05-15 11:31:13.000000 siriuspy-2.74.0/siriuspy/devices/bpm.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7380 2023-05-15 11:31:13.000000 siriuspy-2.74.0/siriuspy/devices/currinfo.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2402 2023-05-15 11:31:13.000000 siriuspy-2.74.0/siriuspy/devices/dcct.py
+-rw-r--r--   0 runner    (1001) docker     (122)    12731 2023-05-15 11:31:13.000000 siriuspy-2.74.0/siriuspy/devices/device.py
+-rw-r--r--   0 runner    (1001) docker     (122)     8382 2023-05-15 11:31:13.000000 siriuspy-2.74.0/siriuspy/devices/dvf.py
+-rw-r--r--   0 runner    (1001) docker     (122)    30814 2023-05-15 11:31:13.000000 siriuspy-2.74.0/siriuspy/devices/egun.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1743 2023-05-15 11:31:13.000000 siriuspy-2.74.0/siriuspy/devices/energy.py
+-rw-r--r--   0 runner    (1001) docker     (122)    48527 2023-05-15 11:31:13.000000 siriuspy-2.74.0/siriuspy/devices/fofb.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2121 2023-05-15 11:31:13.000000 siriuspy-2.74.0/siriuspy/devices/ict.py
+-rw-r--r--   0 runner    (1001) docker     (122)     9493 2023-05-15 11:31:13.000000 siriuspy-2.74.0/siriuspy/devices/idff.py
+-rw-r--r--   0 runner    (1001) docker     (122)    17596 2023-05-15 11:31:13.000000 siriuspy-2.74.0/siriuspy/devices/ids.py
+-rw-r--r--   0 runner    (1001) docker     (122)    20741 2023-05-15 11:31:13.000000 siriuspy-2.74.0/siriuspy/devices/injctrl.py
+-rw-r--r--   0 runner    (1001) docker     (122)    36024 2023-05-15 11:31:13.000000 siriuspy-2.74.0/siriuspy/devices/injsys.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1630 2023-05-15 11:31:13.000000 siriuspy-2.74.0/siriuspy/devices/lienergy.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6948 2023-05-15 11:31:13.000000 siriuspy-2.74.0/siriuspy/devices/lillrf.py
+-rw-r--r--   0 runner    (1001) docker     (122)      964 2023-05-15 11:31:13.000000 siriuspy-2.74.0/siriuspy/devices/machshift.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2290 2023-05-15 11:31:13.000000 siriuspy-2.74.0/siriuspy/devices/modltr.py
+-rw-r--r--   0 runner    (1001) docker     (122)    36060 2023-05-15 11:31:13.000000 siriuspy-2.74.0/siriuspy/devices/orbit_interlock.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2427 2023-05-15 11:31:13.000000 siriuspy-2.74.0/siriuspy/devices/posang.py
+-rw-r--r--   0 runner    (1001) docker     (122)     9576 2023-05-15 11:31:13.000000 siriuspy-2.74.0/siriuspy/devices/psconv.py
+-rw-r--r--   0 runner    (1001) docker     (122)    12042 2023-05-15 11:31:13.000000 siriuspy-2.74.0/siriuspy/devices/pssofb.py
+-rw-r--r--   0 runner    (1001) docker     (122)    19964 2023-05-15 11:31:13.000000 siriuspy-2.74.0/siriuspy/devices/pstesters.py
+-rw-r--r--   0 runner    (1001) docker     (122)    28397 2023-05-15 11:31:13.000000 siriuspy-2.74.0/siriuspy/devices/pwrsupply.py
+-rw-r--r--   0 runner    (1001) docker     (122)    35448 2023-05-15 11:31:13.000000 siriuspy-2.74.0/siriuspy/devices/rf.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3836 2023-05-15 11:31:13.000000 siriuspy-2.74.0/siriuspy/devices/screen.py
+-rw-r--r--   0 runner    (1001) docker     (122)    22629 2023-05-15 11:31:13.000000 siriuspy-2.74.0/siriuspy/devices/sofb.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2606 2023-05-15 11:31:13.000000 siriuspy-2.74.0/siriuspy/devices/syncd.py
+-rw-r--r--   0 runner    (1001) docker     (122)    17907 2023-05-15 11:31:13.000000 siriuspy-2.74.0/siriuspy/devices/timing.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5055 2023-05-15 11:31:13.000000 siriuspy-2.74.0/siriuspy/devices/tune.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-15 11:31:28.727121 siriuspy-2.74.0/siriuspy/diagbeam/
+-rw-r--r--   0 runner    (1001) docker     (122)       30 2023-05-15 11:31:13.000000 siriuspy-2.74.0/siriuspy/diagbeam/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-15 11:31:28.727121 siriuspy-2.74.0/siriuspy/diagbeam/bpm/
+-rw-r--r--   0 runner    (1001) docker     (122)       24 2023-05-15 11:31:13.000000 siriuspy-2.74.0/siriuspy/diagbeam/bpm/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    24052 2023-05-15 11:31:13.000000 siriuspy-2.74.0/siriuspy/diagbeam/bpm/csdev.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-15 11:31:28.727121 siriuspy-2.74.0/siriuspy/diagbeam/dcct/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-15 11:31:13.000000 siriuspy-2.74.0/siriuspy/diagbeam/dcct/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     8215 2023-05-15 11:31:13.000000 siriuspy-2.74.0/siriuspy/diagbeam/dcct/csdev.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-15 11:31:28.727121 siriuspy-2.74.0/siriuspy/diagbeam/ict/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-15 11:31:13.000000 siriuspy-2.74.0/siriuspy/diagbeam/ict/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4878 2023-05-15 11:31:13.000000 siriuspy-2.74.0/siriuspy/diagbeam/ict/csdev.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-15 11:31:28.727121 siriuspy-2.74.0/siriuspy/diagbeam/screen/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-15 11:31:13.000000 siriuspy-2.74.0/siriuspy/diagbeam/screen/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    12756 2023-05-15 11:31:13.000000 siriuspy-2.74.0/siriuspy/diagbeam/screen/csdev.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-15 11:31:28.727121 siriuspy-2.74.0/siriuspy/diagbeam/slit/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-15 11:31:13.000000 siriuspy-2.74.0/siriuspy/diagbeam/slit/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6750 2023-05-15 11:31:13.000000 siriuspy-2.74.0/siriuspy/diagbeam/slit/csdev.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-15 11:31:28.727121 siriuspy-2.74.0/siriuspy/diagsys/
+-rw-r--r--   0 runner    (1001) docker     (122)       26 2023-05-15 11:31:13.000000 siriuspy-2.74.0/siriuspy/diagsys/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1444 2023-05-15 11:31:13.000000 siriuspy-2.74.0/siriuspy/diagsys/app.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-15 11:31:28.727121 siriuspy-2.74.0/siriuspy/diagsys/lidiag/
+-rw-r--r--   0 runner    (1001) docker     (122)       29 2023-05-15 11:31:13.000000 siriuspy-2.74.0/siriuspy/diagsys/lidiag/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5193 2023-05-15 11:31:13.000000 siriuspy-2.74.0/siriuspy/diagsys/lidiag/csdev.py
+-rw-r--r--   0 runner    (1001) docker     (122)     8168 2023-05-15 11:31:13.000000 siriuspy-2.74.0/siriuspy/diagsys/lidiag/main.py
+-rw-r--r--   0 runner    (1001) docker     (122)     8774 2023-05-15 11:31:13.000000 siriuspy-2.74.0/siriuspy/diagsys/lidiag/pvs.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-15 11:31:28.727121 siriuspy-2.74.0/siriuspy/diagsys/psdiag/
+-rw-r--r--   0 runner    (1001) docker     (122)       25 2023-05-15 11:31:13.000000 siriuspy-2.74.0/siriuspy/diagsys/psdiag/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2556 2023-05-15 11:31:13.000000 siriuspy-2.74.0/siriuspy/diagsys/psdiag/csdev.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4299 2023-05-15 11:31:13.000000 siriuspy-2.74.0/siriuspy/diagsys/psdiag/main.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6705 2023-05-15 11:31:13.000000 siriuspy-2.74.0/siriuspy/diagsys/psdiag/pvs.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-15 11:31:28.727121 siriuspy-2.74.0/siriuspy/diagsys/pudiag/
+-rw-r--r--   0 runner    (1001) docker     (122)       25 2023-05-15 11:31:13.000000 siriuspy-2.74.0/siriuspy/diagsys/pudiag/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1418 2023-05-15 11:31:13.000000 siriuspy-2.74.0/siriuspy/diagsys/pudiag/csdev.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2871 2023-05-15 11:31:13.000000 siriuspy-2.74.0/siriuspy/diagsys/pudiag/main.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4099 2023-05-15 11:31:13.000000 siriuspy-2.74.0/siriuspy/diagsys/pudiag/pvs.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6824 2023-05-15 11:31:13.000000 siriuspy-2.74.0/siriuspy/diagsys/pvs.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-15 11:31:28.727121 siriuspy-2.74.0/siriuspy/diagsys/rfdiag/
+-rw-r--r--   0 runner    (1001) docker     (122)       25 2023-05-15 11:31:13.000000 siriuspy-2.74.0/siriuspy/diagsys/rfdiag/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2409 2023-05-15 11:31:13.000000 siriuspy-2.74.0/siriuspy/diagsys/rfdiag/csdev.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3783 2023-05-15 11:31:13.000000 siriuspy-2.74.0/siriuspy/diagsys/rfdiag/main.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4891 2023-05-15 11:31:13.000000 siriuspy-2.74.0/siriuspy/diagsys/rfdiag/pvs.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2135 2023-05-15 11:31:13.000000 siriuspy-2.74.0/siriuspy/envars.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-15 11:31:28.731121 siriuspy-2.74.0/siriuspy/epics/
+-rw-r--r--   0 runner    (1001) docker     (122)      379 2023-05-15 11:31:13.000000 siriuspy-2.74.0/siriuspy/epics/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      624 2023-05-15 11:31:13.000000 siriuspy-2.74.0/siriuspy/epics/multiproc.py
+-rw-r--r--   0 runner    (1001) docker     (122)     9097 2023-05-15 11:31:13.000000 siriuspy-2.74.0/siriuspy/epics/properties.py
+-rw-r--r--   0 runner    (1001) docker     (122)      209 2023-05-15 11:31:13.000000 siriuspy-2.74.0/siriuspy/epics/pv.py
+-rw-r--r--   0 runner    (1001) docker     (122)    29251 2023-05-15 11:31:13.000000 siriuspy-2.74.0/siriuspy/epics/pv_fake.py
+-rw-r--r--   0 runner    (1001) docker     (122)     9170 2023-05-15 11:31:13.000000 siriuspy-2.74.0/siriuspy/epics/pv_time_serie.py
+-rw-r--r--   0 runner    (1001) docker     (122)      100 2023-05-15 11:31:13.000000 siriuspy-2.74.0/siriuspy/epics/threading.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-15 11:31:28.731121 siriuspy-2.74.0/siriuspy/fofb/
+-rw-r--r--   0 runner    (1001) docker     (122)       34 2023-05-15 11:31:13.000000 siriuspy-2.74.0/siriuspy/fofb/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    18873 2023-05-15 11:31:13.000000 siriuspy-2.74.0/siriuspy/fofb/csdev.py
+-rw-r--r--   0 runner    (1001) docker     (122)    80150 2023-05-15 11:31:13.000000 siriuspy-2.74.0/siriuspy/fofb/main.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-15 11:31:28.731121 siriuspy-2.74.0/siriuspy/idff/
+-rw-r--r--   0 runner    (1001) docker     (122)       76 2023-05-15 11:31:13.000000 siriuspy-2.74.0/siriuspy/idff/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7459 2023-05-15 11:31:13.000000 siriuspy-2.74.0/siriuspy/idff/config.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2367 2023-05-15 11:31:13.000000 siriuspy-2.74.0/siriuspy/idff/csdev.py
+-rw-r--r--   0 runner    (1001) docker     (122)     8294 2023-05-15 11:31:13.000000 siriuspy-2.74.0/siriuspy/idff/main.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-15 11:31:28.731121 siriuspy-2.74.0/siriuspy/injctrl/
+-rw-r--r--   0 runner    (1001) docker     (122)       36 2023-05-15 11:31:13.000000 siriuspy-2.74.0/siriuspy/injctrl/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    15244 2023-05-15 11:31:13.000000 siriuspy-2.74.0/siriuspy/injctrl/bias_feedback.py
+-rw-r--r--   0 runner    (1001) docker     (122)    26067 2023-05-15 11:31:13.000000 siriuspy-2.74.0/siriuspy/injctrl/csdev.py
+-rw-r--r--   0 runner    (1001) docker     (122)    67948 2023-05-15 11:31:13.000000 siriuspy-2.74.0/siriuspy/injctrl/main.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-15 11:31:28.731121 siriuspy-2.74.0/siriuspy/machshift/
+-rw-r--r--   0 runner    (1001) docker     (122)       32 2023-05-15 11:31:13.000000 siriuspy-2.74.0/siriuspy/machshift/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1297 2023-05-15 11:31:13.000000 siriuspy-2.74.0/siriuspy/machshift/csdev.py
+-rw-r--r--   0 runner    (1001) docker     (122)    77640 2023-05-15 11:31:13.000000 siriuspy-2.74.0/siriuspy/machshift/macreport.py
+-rw-r--r--   0 runner    (1001) docker     (122)     8913 2023-05-15 11:31:13.000000 siriuspy-2.74.0/siriuspy/machshift/macschedule.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2237 2023-05-15 11:31:13.000000 siriuspy-2.74.0/siriuspy/machshift/main.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5429 2023-05-15 11:31:13.000000 siriuspy-2.74.0/siriuspy/machshift/test_macreport.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2012 2023-05-15 11:31:13.000000 siriuspy-2.74.0/siriuspy/machshift/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-15 11:31:28.731121 siriuspy-2.74.0/siriuspy/magnet/
+-rw-r--r--   0 runner    (1001) docker     (122)       25 2023-05-15 11:31:13.000000 siriuspy-2.74.0/siriuspy/magnet/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1126 2023-05-15 11:31:13.000000 siriuspy-2.74.0/siriuspy/magnet/data.py
+-rw-r--r--   0 runner    (1001) docker     (122)     8736 2023-05-15 11:31:13.000000 siriuspy-2.74.0/siriuspy/magnet/excdata.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1390 2023-05-15 11:31:13.000000 siriuspy-2.74.0/siriuspy/magnet/factory.py
+-rw-r--r--   0 runner    (1001) docker     (122)    15453 2023-05-15 11:31:13.000000 siriuspy-2.74.0/siriuspy/magnet/normalizer.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7185 2023-05-15 11:31:13.000000 siriuspy-2.74.0/siriuspy/magnet/util.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-15 11:31:28.731121 siriuspy-2.74.0/siriuspy/meas/
+-rw-r--r--   0 runner    (1001) docker     (122)       41 2023-05-15 11:31:13.000000 siriuspy-2.74.0/siriuspy/meas/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    11826 2023-05-15 11:31:13.000000 siriuspy-2.74.0/siriuspy/meas/csdev.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-15 11:31:28.735122 siriuspy-2.74.0/siriuspy/meas/liemit/
+-rw-r--r--   0 runner    (1001) docker     (122)       57 2023-05-15 11:31:13.000000 siriuspy-2.74.0/siriuspy/meas/liemit/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1455 2023-05-15 11:31:13.000000 siriuspy-2.74.0/siriuspy/meas/liemit/csdev.py
+-rw-r--r--   0 runner    (1001) docker     (122)    13017 2023-05-15 11:31:13.000000 siriuspy-2.74.0/siriuspy/meas/liemit/main.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-15 11:31:28.735122 siriuspy-2.74.0/siriuspy/meas/lienergy/
+-rw-r--r--   0 runner    (1001) docker     (122)       80 2023-05-15 11:31:13.000000 siriuspy-2.74.0/siriuspy/meas/lienergy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2821 2023-05-15 11:31:13.000000 siriuspy-2.74.0/siriuspy/meas/lienergy/csdev.py
+-rw-r--r--   0 runner    (1001) docker     (122)     8714 2023-05-15 11:31:13.000000 siriuspy-2.74.0/siriuspy/meas/lienergy/main.py
+-rw-r--r--   0 runner    (1001) docker     (122)    25137 2023-05-15 11:31:13.000000 siriuspy-2.74.0/siriuspy/meas/util.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-15 11:31:28.735122 siriuspy-2.74.0/siriuspy/namesys/
+-rw-r--r--   0 runner    (1001) docker     (122)       82 2023-05-15 11:31:13.000000 siriuspy-2.74.0/siriuspy/namesys/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    15210 2023-05-15 11:31:13.000000 siriuspy-2.74.0/siriuspy/namesys/implementation.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-15 11:31:28.735122 siriuspy-2.74.0/siriuspy/optics/
+-rw-r--r--   0 runner    (1001) docker     (122)       25 2023-05-15 11:31:13.000000 siriuspy-2.74.0/siriuspy/optics/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      363 2023-05-15 11:31:13.000000 siriuspy-2.74.0/siriuspy/optics/constants.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6906 2023-05-15 11:31:13.000000 siriuspy-2.74.0/siriuspy/optics/lattice_survey.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-15 11:31:28.735122 siriuspy-2.74.0/siriuspy/opticscorr/
+-rw-r--r--   0 runner    (1001) docker     (122)       29 2023-05-15 11:31:13.000000 siriuspy-2.74.0/siriuspy/opticscorr/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    34878 2023-05-15 11:31:13.000000 siriuspy-2.74.0/siriuspy/opticscorr/base.py
+-rw-r--r--   0 runner    (1001) docker     (122)    16096 2023-05-15 11:31:13.000000 siriuspy-2.74.0/siriuspy/opticscorr/chrom.py
+-rw-r--r--   0 runner    (1001) docker     (122)    13454 2023-05-15 11:31:13.000000 siriuspy-2.74.0/siriuspy/opticscorr/csdev.py
+-rw-r--r--   0 runner    (1001) docker     (122)    18765 2023-05-15 11:31:13.000000 siriuspy-2.74.0/siriuspy/opticscorr/opticscorr.py
+-rw-r--r--   0 runner    (1001) docker     (122)     8006 2023-05-15 11:31:13.000000 siriuspy-2.74.0/siriuspy/opticscorr/tune.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1846 2023-05-15 11:31:13.000000 siriuspy-2.74.0/siriuspy/opticscorr/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-15 11:31:28.735122 siriuspy-2.74.0/siriuspy/oscilloscope/
+-rw-r--r--   0 runner    (1001) docker     (122)      104 2023-05-15 11:31:13.000000 siriuspy-2.74.0/siriuspy/oscilloscope/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6691 2023-05-15 11:31:13.000000 siriuspy-2.74.0/siriuspy/oscilloscope/keysight.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1467 2023-05-15 11:31:13.000000 siriuspy-2.74.0/siriuspy/oscilloscope/scopes.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-15 11:31:28.735122 siriuspy-2.74.0/siriuspy/posang/
+-rw-r--r--   0 runner    (1001) docker     (122)       25 2023-05-15 11:31:13.000000 siriuspy-2.74.0/siriuspy/posang/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4935 2023-05-15 11:31:13.000000 siriuspy-2.74.0/siriuspy/posang/csdev.py
+-rw-r--r--   0 runner    (1001) docker     (122)    19747 2023-05-15 11:31:13.000000 siriuspy-2.74.0/siriuspy/posang/main.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1678 2023-05-15 11:31:13.000000 siriuspy-2.74.0/siriuspy/posang/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-15 11:31:28.735122 siriuspy-2.74.0/siriuspy/pwrsupply/
+-rw-r--r--   0 runner    (1001) docker     (122)      132 2023-05-15 11:31:13.000000 siriuspy-2.74.0/siriuspy/pwrsupply/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     8950 2023-05-15 11:31:13.000000 siriuspy-2.74.0/siriuspy/pwrsupply/beaglebone.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-15 11:31:28.739122 siriuspy-2.74.0/siriuspy/pwrsupply/bsmp/
+-rw-r--r--   0 runner    (1001) docker     (122)       48 2023-05-15 11:31:13.000000 siriuspy-2.74.0/siriuspy/pwrsupply/bsmp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    25156 2023-05-15 11:31:13.000000 siriuspy-2.74.0/siriuspy/pwrsupply/bsmp/commands.py
+-rw-r--r--   0 runner    (1001) docker     (122)    19464 2023-05-15 11:31:13.000000 siriuspy-2.74.0/siriuspy/pwrsupply/bsmp/constants.py
+-rw-r--r--   0 runner    (1001) docker     (122)    53763 2023-05-15 11:31:13.000000 siriuspy-2.74.0/siriuspy/pwrsupply/bsmp/entities.py
+-rw-r--r--   0 runner    (1001) docker     (122)      850 2023-05-15 11:31:13.000000 siriuspy-2.74.0/siriuspy/pwrsupply/bsmp/factory.py
+-rw-r--r--   0 runner    (1001) docker     (122)   150426 2023-05-15 11:31:13.000000 siriuspy-2.74.0/siriuspy/pwrsupply/csdev.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3624 2023-05-15 11:31:13.000000 siriuspy-2.74.0/siriuspy/pwrsupply/data.py
+-rw-r--r--   0 runner    (1001) docker     (122)    10620 2023-05-15 11:31:13.000000 siriuspy-2.74.0/siriuspy/pwrsupply/factory.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-15 11:31:28.739122 siriuspy-2.74.0/siriuspy/pwrsupply/pructrl/
+-rw-r--r--   0 runner    (1001) docker     (122)      841 2023-05-15 11:31:13.000000 siriuspy-2.74.0/siriuspy/pwrsupply/pructrl/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3393 2023-05-15 11:31:13.000000 siriuspy-2.74.0/siriuspy/pwrsupply/pructrl/pru.py
+-rw-r--r--   0 runner    (1001) docker     (122)    26340 2023-05-15 11:31:13.000000 siriuspy-2.74.0/siriuspy/pwrsupply/pructrl/prucontroller.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6133 2023-05-15 11:31:13.000000 siriuspy-2.74.0/siriuspy/pwrsupply/pructrl/prucparms.py
+-rw-r--r--   0 runner    (1001) docker     (122)    10280 2023-05-15 11:31:13.000000 siriuspy-2.74.0/siriuspy/pwrsupply/pructrl/psdevstate.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7712 2023-05-15 11:31:13.000000 siriuspy-2.74.0/siriuspy/pwrsupply/pructrl/udc.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-15 11:31:28.739122 siriuspy-2.74.0/siriuspy/pwrsupply/psctrl/
+-rw-r--r--   0 runner    (1001) docker     (122)      866 2023-05-15 11:31:13.000000 siriuspy-2.74.0/siriuspy/pwrsupply/psctrl/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7884 2023-05-15 11:31:13.000000 siriuspy-2.74.0/siriuspy/pwrsupply/psctrl/pscontroller.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6262 2023-05-15 11:31:13.000000 siriuspy-2.74.0/siriuspy/pwrsupply/psctrl/pscreaders.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5502 2023-05-15 11:31:13.000000 siriuspy-2.74.0/siriuspy/pwrsupply/psctrl/pscstatus.py
+-rw-r--r--   0 runner    (1001) docker     (122)    17064 2023-05-15 11:31:13.000000 siriuspy-2.74.0/siriuspy/pwrsupply/psctrl/pscwriters.py
+-rw-r--r--   0 runner    (1001) docker     (122)    42124 2023-05-15 11:31:13.000000 siriuspy-2.74.0/siriuspy/pwrsupply/psctrl/psmodel.py
+-rw-r--r--   0 runner    (1001) docker     (122)    33182 2023-05-15 11:31:13.000000 siriuspy-2.74.0/siriuspy/pwrsupply/pssofb.py
+-rw-r--r--   0 runner    (1001) docker     (122)    12500 2023-05-15 11:31:13.000000 siriuspy-2.74.0/siriuspy/pwrsupply/siggen.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-15 11:31:28.739122 siriuspy-2.74.0/siriuspy/ramp/
+-rw-r--r--   0 runner    (1001) docker     (122)       23 2023-05-15 11:31:13.000000 siriuspy-2.74.0/siriuspy/ramp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    28999 2023-05-15 11:31:13.000000 siriuspy-2.74.0/siriuspy/ramp/conn.py
+-rw-r--r--   0 runner    (1001) docker     (122)      346 2023-05-15 11:31:13.000000 siriuspy-2.74.0/siriuspy/ramp/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3969 2023-05-15 11:31:13.000000 siriuspy-2.74.0/siriuspy/ramp/magnet.py
+-rw-r--r--   0 runner    (1001) docker     (122)    45093 2023-05-15 11:31:13.000000 siriuspy-2.74.0/siriuspy/ramp/ramp.py
+-rw-r--r--   0 runner    (1001) docker     (122)    29333 2023-05-15 11:31:13.000000 siriuspy-2.74.0/siriuspy/ramp/reconst_factory.py
+-rwxr-xr-x   0 runner    (1001) docker     (122)     6985 2023-05-15 11:31:13.000000 siriuspy-2.74.0/siriuspy/ramp/test_reconst_factory.py
+-rwxr-xr-x   0 runner    (1001) docker     (122)     4158 2023-05-15 11:31:13.000000 siriuspy-2.74.0/siriuspy/ramp/testwfm.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5584 2023-05-15 11:31:13.000000 siriuspy-2.74.0/siriuspy/ramp/util.py
+-rw-r--r--   0 runner    (1001) docker     (122)    30145 2023-05-15 11:31:13.000000 siriuspy-2.74.0/siriuspy/ramp/waveform.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-15 11:31:28.743121 siriuspy-2.74.0/siriuspy/search/
+-rw-r--r--   0 runner    (1001) docker     (122)      359 2023-05-15 11:31:13.000000 siriuspy-2.74.0/siriuspy/search/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3537 2023-05-15 11:31:13.000000 siriuspy-2.74.0/siriuspy/search/bpms_search.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6612 2023-05-15 11:31:13.000000 siriuspy-2.74.0/siriuspy/search/hl_time_search.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4859 2023-05-15 11:31:13.000000 siriuspy-2.74.0/siriuspy/search/id_search.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4152 2023-05-15 11:31:13.000000 siriuspy-2.74.0/siriuspy/search/ioc_search.py
+-rw-r--r--   0 runner    (1001) docker     (122)    16917 2023-05-15 11:31:13.000000 siriuspy-2.74.0/siriuspy/search/ll_time_search.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7219 2023-05-15 11:31:13.000000 siriuspy-2.74.0/siriuspy/search/ma_search.py
+-rw-r--r--   0 runner    (1001) docker     (122)    23882 2023-05-15 11:31:13.000000 siriuspy-2.74.0/siriuspy/search/ps_search.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-15 11:31:28.743121 siriuspy-2.74.0/siriuspy/simul/
+-rw-r--r--   0 runner    (1001) docker     (122)      311 2023-05-15 11:31:13.000000 siriuspy-2.74.0/siriuspy/simul/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2202 2023-05-15 11:31:13.000000 siriuspy-2.74.0/siriuspy/simul/simfactory.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6298 2023-05-15 11:31:13.000000 siriuspy-2.74.0/siriuspy/simul/simps.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2324 2023-05-15 11:31:13.000000 siriuspy-2.74.0/siriuspy/simul/simpv.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7391 2023-05-15 11:31:13.000000 siriuspy-2.74.0/siriuspy/simul/simulation.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4266 2023-05-15 11:31:13.000000 siriuspy-2.74.0/siriuspy/simul/simulator.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-15 11:31:28.743121 siriuspy-2.74.0/siriuspy/sofb/
+-rw-r--r--   0 runner    (1001) docker     (122)       78 2023-05-15 11:31:13.000000 siriuspy-2.74.0/siriuspy/sofb/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4646 2023-05-15 11:31:13.000000 siriuspy-2.74.0/siriuspy/sofb/base_class.py
+-rw-r--r--   0 runner    (1001) docker     (122)    28072 2023-05-15 11:31:13.000000 siriuspy-2.74.0/siriuspy/sofb/bpms.py
+-rw-r--r--   0 runner    (1001) docker     (122)    32149 2023-05-15 11:31:13.000000 siriuspy-2.74.0/siriuspy/sofb/correctors.py
+-rw-r--r--   0 runner    (1001) docker     (122)    47045 2023-05-15 11:31:13.000000 siriuspy-2.74.0/siriuspy/sofb/csdev.py
+-rw-r--r--   0 runner    (1001) docker     (122)    45797 2023-05-15 11:31:13.000000 siriuspy-2.74.0/siriuspy/sofb/main.py
+-rw-r--r--   0 runner    (1001) docker     (122)    12220 2023-05-15 11:31:13.000000 siriuspy-2.74.0/siriuspy/sofb/matrix.py
+-rw-r--r--   0 runner    (1001) docker     (122)    39653 2023-05-15 11:31:13.000000 siriuspy-2.74.0/siriuspy/sofb/orbit.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3030 2023-05-15 11:31:13.000000 siriuspy-2.74.0/siriuspy/sofb/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-15 11:31:28.743121 siriuspy-2.74.0/siriuspy/stabinfo/
+-rw-r--r--   0 runner    (1001) docker     (122)       38 2023-05-15 11:31:13.000000 siriuspy-2.74.0/siriuspy/stabinfo/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3558 2023-05-15 11:31:13.000000 siriuspy-2.74.0/siriuspy/stabinfo/csdev.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7708 2023-05-15 11:31:13.000000 siriuspy-2.74.0/siriuspy/stabinfo/main.py
+-rw-r--r--   0 runner    (1001) docker     (122)     8093 2023-05-15 11:31:13.000000 siriuspy-2.74.0/siriuspy/thread.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-15 11:31:28.743121 siriuspy-2.74.0/siriuspy/timesys/
+-rw-r--r--   0 runner    (1001) docker     (122)       26 2023-05-15 11:31:13.000000 siriuspy-2.74.0/siriuspy/timesys/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    20220 2023-05-15 11:31:13.000000 siriuspy-2.74.0/siriuspy/timesys/csdev.py
+-rw-r--r--   0 runner    (1001) docker     (122)    12705 2023-05-15 11:31:13.000000 siriuspy-2.74.0/siriuspy/timesys/hl_classes.py
+-rw-r--r--   0 runner    (1001) docker     (122)    33256 2023-05-15 11:31:13.000000 siriuspy-2.74.0/siriuspy/timesys/ll_classes.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6015 2023-05-15 11:31:13.000000 siriuspy-2.74.0/siriuspy/timesys/plot_network.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5957 2023-05-15 11:31:13.000000 siriuspy-2.74.0/siriuspy/timesys/static_table.py
+-rw-r--r--   0 runner    (1001) docker     (122)     8732 2023-05-15 11:31:13.000000 siriuspy-2.74.0/siriuspy/util.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-15 11:31:28.715121 siriuspy-2.74.0/siriuspy.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)     1423 2023-05-15 11:31:28.000000 siriuspy-2.74.0/siriuspy.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     9945 2023-05-15 11:31:28.000000 siriuspy-2.74.0/siriuspy.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-05-15 11:31:28.000000 siriuspy-2.74.0/siriuspy.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-05-15 11:31:28.000000 siriuspy-2.74.0/siriuspy.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (122)      128 2023-05-15 11:31:28.000000 siriuspy-2.74.0/siriuspy.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       15 2023-05-15 11:31:28.000000 siriuspy-2.74.0/siriuspy.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-15 11:31:28.743121 siriuspy-2.74.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (122)      441 2023-05-15 11:31:13.000000 siriuspy-2.74.0/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-15 11:31:28.743121 siriuspy-2.74.0/tests/bsmp/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-15 11:31:13.000000 siriuspy-2.74.0/tests/bsmp/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (122)     5698 2023-05-15 11:31:13.000000 siriuspy-2.74.0/tests/bsmp/test_bsmp.py
+-rwxr-xr-x   0 runner    (1001) docker     (122)    14788 2023-05-15 11:31:13.000000 siriuspy-2.74.0/tests/bsmp/test_commands.py
+-rwxr-xr-x   0 runner    (1001) docker     (122)    13382 2023-05-15 11:31:13.000000 siriuspy-2.74.0/tests/bsmp/test_entities.py
+-rwxr-xr-x   0 runner    (1001) docker     (122)     7719 2023-05-15 11:31:13.000000 siriuspy-2.74.0/tests/bsmp/test_serial.py
+-rwxr-xr-x   0 runner    (1001) docker     (122)     1837 2023-05-15 11:31:13.000000 siriuspy-2.74.0/tests/bsmp/test_types.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-15 11:31:28.743121 siriuspy-2.74.0/tests/clientconfigdb/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-15 11:31:13.000000 siriuspy-2.74.0/tests/clientconfigdb/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (122)     2843 2023-05-15 11:31:13.000000 siriuspy-2.74.0/tests/clientconfigdb/test_configdb_client.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-15 11:31:28.747122 siriuspy-2.74.0/tests/clientweb/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-15 11:31:13.000000 siriuspy-2.74.0/tests/clientweb/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (122)    11633 2023-05-15 11:31:13.000000 siriuspy-2.74.0/tests/clientweb/test_implementation.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-15 11:31:28.747122 siriuspy-2.74.0/tests/currinfo/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-15 11:31:13.000000 siriuspy-2.74.0/tests/currinfo/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-15 11:31:28.747122 siriuspy-2.74.0/tests/currinfo/lifetime/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-15 11:31:13.000000 siriuspy-2.74.0/tests/currinfo/lifetime/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (122)     1908 2023-05-15 11:31:13.000000 siriuspy-2.74.0/tests/currinfo/lifetime/test_main.py
+-rwxr-xr-x   0 runner    (1001) docker     (122)     6495 2023-05-15 11:31:13.000000 siriuspy-2.74.0/tests/currinfo/test_csdev.py
+-rwxr-xr-x   0 runner    (1001) docker     (122)     2653 2023-05-15 11:31:13.000000 siriuspy-2.74.0/tests/currinfo/test_main.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-15 11:31:28.747122 siriuspy-2.74.0/tests/magnet/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-15 11:31:13.000000 siriuspy-2.74.0/tests/magnet/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (122)     2275 2023-05-15 11:31:13.000000 siriuspy-2.74.0/tests/magnet/test_factory.py
+-rwxr-xr-x   0 runner    (1001) docker     (122)     2687 2023-05-15 11:31:13.000000 siriuspy-2.74.0/tests/magnet/tests_normalizer.py
+-rwxr-xr-x   0 runner    (1001) docker     (122)     3618 2023-05-15 11:31:13.000000 siriuspy-2.74.0/tests/mock_servweb.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-15 11:31:28.747122 siriuspy-2.74.0/tests/namesys/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-15 11:31:13.000000 siriuspy-2.74.0/tests/namesys/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (122)     4896 2023-05-15 11:31:13.000000 siriuspy-2.74.0/tests/namesys/test_implementation.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-15 11:31:28.747122 siriuspy-2.74.0/tests/opticscorr/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-15 11:31:13.000000 siriuspy-2.74.0/tests/opticscorr/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5490 2023-05-15 11:31:13.000000 siriuspy-2.74.0/tests/opticscorr/test_chrom.py
+-rwxr-xr-x   0 runner    (1001) docker     (122)     4609 2023-05-15 11:31:13.000000 siriuspy-2.74.0/tests/opticscorr/test_csdev.py
+-rwxr-xr-x   0 runner    (1001) docker     (122)    23381 2023-05-15 11:31:13.000000 siriuspy-2.74.0/tests/opticscorr/test_opticscorr.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5692 2023-05-15 11:31:13.000000 siriuspy-2.74.0/tests/opticscorr/test_tune.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1145 2023-05-15 11:31:13.000000 siriuspy-2.74.0/tests/opticscorr/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-15 11:31:28.747122 siriuspy-2.74.0/tests/posang/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-15 11:31:13.000000 siriuspy-2.74.0/tests/posang/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (122)     2872 2023-05-15 11:31:13.000000 siriuspy-2.74.0/tests/posang/test_csdev.py
+-rwxr-xr-x   0 runner    (1001) docker     (122)     3164 2023-05-15 11:31:13.000000 siriuspy-2.74.0/tests/posang/test_main.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-15 11:31:28.747122 siriuspy-2.74.0/tests/pwrsupply/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-15 11:31:13.000000 siriuspy-2.74.0/tests/pwrsupply/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    18979 2023-05-15 11:31:13.000000 siriuspy-2.74.0/tests/pwrsupply/db.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-15 11:31:28.747122 siriuspy-2.74.0/tests/pwrsupply/pructrl/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-15 11:31:13.000000 siriuspy-2.74.0/tests/pwrsupply/pructrl/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (122)     2257 2023-05-15 11:31:13.000000 siriuspy-2.74.0/tests/pwrsupply/pructrl/test_pru.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-15 11:31:28.747122 siriuspy-2.74.0/tests/pwrsupply/psctrl/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-15 11:31:13.000000 siriuspy-2.74.0/tests/pwrsupply/psctrl/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4853 2023-05-15 11:31:13.000000 siriuspy-2.74.0/tests/pwrsupply/psctrl/test_pscwriters.py
+-rwxr-xr-x   0 runner    (1001) docker     (122)      166 2023-05-15 11:31:13.000000 siriuspy-2.74.0/tests/pwrsupply/test_beaglebone.py
+-rwxr-xr-x   0 runner    (1001) docker     (122)       89 2023-05-15 11:31:13.000000 siriuspy-2.74.0/tests/pwrsupply/test_bsmp.py
+-rwxr-xr-x   0 runner    (1001) docker     (122)     6439 2023-05-15 11:31:13.000000 siriuspy-2.74.0/tests/pwrsupply/test_csdev.py
+-rwxr-xr-x   0 runner    (1001) docker     (122)     7331 2023-05-15 11:31:13.000000 siriuspy-2.74.0/tests/pwrsupply/test_data.py
+-rwxr-xr-x   0 runner    (1001) docker     (122)     2323 2023-05-15 11:31:13.000000 siriuspy-2.74.0/tests/pwrsupply/test_siggen.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3146 2023-05-15 11:31:13.000000 siriuspy-2.74.0/tests/pwrsupply/variables.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-15 11:31:28.751122 siriuspy-2.74.0/tests/ramp/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-15 11:31:13.000000 siriuspy-2.74.0/tests/ramp/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (122)     5699 2023-05-15 11:31:13.000000 siriuspy-2.74.0/tests/ramp/test_magnet.py
+-rwxr-xr-x   0 runner    (1001) docker     (122)     7235 2023-05-15 11:31:13.000000 siriuspy-2.74.0/tests/ramp/test_waveform.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-15 11:31:28.751122 siriuspy-2.74.0/tests/search/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-15 11:31:13.000000 siriuspy-2.74.0/tests/search/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (122)     2412 2023-05-15 11:31:13.000000 siriuspy-2.74.0/tests/search/test_hl_time_search.py
+-rwxr-xr-x   0 runner    (1001) docker     (122)      559 2023-05-15 11:31:13.000000 siriuspy-2.74.0/tests/search/test_init.py
+-rwxr-xr-x   0 runner    (1001) docker     (122)     3831 2023-05-15 11:31:13.000000 siriuspy-2.74.0/tests/search/test_ll_time_search.py
+-rwxr-xr-x   0 runner    (1001) docker     (122)     6120 2023-05-15 11:31:13.000000 siriuspy-2.74.0/tests/search/test_ma_search.py
+-rwxr-xr-x   0 runner    (1001) docker     (122)    13502 2023-05-15 11:31:13.000000 siriuspy-2.74.0/tests/search/test_ps_search.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3478 2023-05-15 11:31:13.000000 siriuspy-2.74.0/tests/test_callbacks.py
+-rwxr-xr-x   0 runner    (1001) docker     (122)     1009 2023-05-15 11:31:13.000000 siriuspy-2.74.0/tests/test_csdev.py
+-rwxr-xr-x   0 runner    (1001) docker     (122)     1605 2023-05-15 11:31:13.000000 siriuspy-2.74.0/tests/test_envars.py
+-rwxr-xr-x   0 runner    (1001) docker     (122)    11533 2023-05-15 11:31:13.000000 siriuspy-2.74.0/tests/test_util.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-15 11:31:28.751122 siriuspy-2.74.0/tests/timesys/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-15 11:31:13.000000 siriuspy-2.74.0/tests/timesys/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (122)     4999 2023-05-15 11:31:13.000000 siriuspy-2.74.0/tests/timesys/test_csdev.py
+-rw-r--r--   0 runner    (1001) docker     (122)      978 2023-05-15 11:31:13.000000 siriuspy-2.74.0/tests/timesys/test_plot_network.py
```

### Comparing `siriuspy-2.73.0/LICENSE` & `siriuspy-2.74.0/LICENSE`

 * *Files identical despite different names*

### Comparing `siriuspy-2.73.0/PKG-INFO` & `siriuspy-2.74.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: siriuspy
-Version: 2.73.0
+Version: 2.74.0
 Summary: Development packages for Sirius
 Home-page: https://github.com/lnls-sirius/dev-packages
 Download-URL: https://github.com/lnls-sirius/dev-packages
 Author: lnls-sirius
 License: GNU GPLv3
 Classifier: Intended Audience :: Science/Research
 Classifier: Programming Language :: Python
```

### Comparing `siriuspy-2.73.0/README.md` & `siriuspy-2.74.0/README.md`

 * *Files identical despite different names*

### Comparing `siriuspy-2.73.0/setup.py` & `siriuspy-2.74.0/setup.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.73.0/siriuspy/bsmp/commands.py` & `siriuspy-2.74.0/siriuspy/bsmp/commands.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.73.0/siriuspy/bsmp/constants.py` & `siriuspy-2.74.0/siriuspy/bsmp/constants.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.73.0/siriuspy/bsmp/entities.py` & `siriuspy-2.74.0/siriuspy/bsmp/entities.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.73.0/siriuspy/bsmp/exceptions.py` & `siriuspy-2.74.0/siriuspy/bsmp/exceptions.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.73.0/siriuspy/bsmp/serial.py` & `siriuspy-2.74.0/siriuspy/bsmp/serial.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.73.0/siriuspy/bsmp/types.py` & `siriuspy-2.74.0/siriuspy/bsmp/types.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.73.0/siriuspy/callbacks.py` & `siriuspy-2.74.0/siriuspy/callbacks.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.73.0/siriuspy/clientarch/client.py` & `siriuspy-2.74.0/siriuspy/clientarch/client.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.73.0/siriuspy/clientarch/devices.py` & `siriuspy-2.74.0/siriuspy/clientarch/devices.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.73.0/siriuspy/clientarch/exceptions.py` & `siriuspy-2.74.0/siriuspy/clientarch/exceptions.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.73.0/siriuspy/clientarch/pvarch.py` & `siriuspy-2.74.0/siriuspy/clientarch/pvarch.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.73.0/siriuspy/clientarch/time.py` & `siriuspy-2.74.0/siriuspy/clientarch/time.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.73.0/siriuspy/clientconfigdb/_templates.py` & `siriuspy-2.74.0/siriuspy/clientconfigdb/_templates.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.73.0/siriuspy/clientconfigdb/configdb_client.py` & `siriuspy-2.74.0/siriuspy/clientconfigdb/configdb_client.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.73.0/siriuspy/clientconfigdb/configdb_document.py` & `siriuspy-2.74.0/siriuspy/clientconfigdb/configdb_document.py`

 * *Files 1% similar despite different names*

```diff
@@ -103,15 +103,15 @@
             name=self._name, discarded=discarded)
         self._value = self._configdbclient.get_config_value(
             name=self._name, discarded=discarded)
         self._synchronized = True
 
     def save(self, new_name=None):
         """Save configuration to ConfigServer."""
-        # if config is syncronyzed, it is not necessary to save an identical
+        # if config is syncronized, it is not necessary to save an identical
         # one in server
         if self.exist() and self._synchronized and not new_name:
             return
 
         # check if data format is ok
         if not self._configdbclient.check_valid_value(self._value):
             raise ValueError(
```

### Comparing `siriuspy-2.73.0/siriuspy/clientconfigdb/pvsconfig.py` & `siriuspy-2.74.0/siriuspy/clientconfigdb/pvsconfig.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.73.0/siriuspy/clientconfigdb/types/as_corrloop_params.py` & `siriuspy-2.74.0/siriuspy/clientconfigdb/types/as_corrloop_params.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.73.0/siriuspy/clientconfigdb/types/as_diagnostics.py` & `siriuspy-2.74.0/siriuspy/clientconfigdb/types/as_diagnostics.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.73.0/siriuspy/clientconfigdb/types/as_pwrstate.py` & `siriuspy-2.74.0/siriuspy/clientconfigdb/types/as_pwrstate.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.73.0/siriuspy/clientconfigdb/types/as_rf.py` & `siriuspy-2.74.0/siriuspy/clientconfigdb/types/as_rf.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.73.0/siriuspy/clientconfigdb/types/bo_chromcorr_params.py` & `siriuspy-2.74.0/siriuspy/clientconfigdb/types/bo_chromcorr_params.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.73.0/siriuspy/clientconfigdb/types/bo_normalized.py` & `siriuspy-2.74.0/siriuspy/clientconfigdb/types/bo_normalized.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.73.0/siriuspy/clientconfigdb/types/bo_orbcorr_respm.py` & `siriuspy-2.74.0/siriuspy/clientconfigdb/types/bo_orbcorr_respm.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.73.0/siriuspy/clientconfigdb/types/bo_orbit.py` & `siriuspy-2.74.0/siriuspy/clientconfigdb/types/bo_orbit.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.73.0/siriuspy/clientconfigdb/types/bo_ramp.py` & `siriuspy-2.74.0/siriuspy/clientconfigdb/types/bo_ramp.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.73.0/siriuspy/clientconfigdb/types/bo_tunecorr_params.py` & `siriuspy-2.74.0/siriuspy/clientconfigdb/types/bo_tunecorr_params.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.73.0/siriuspy/clientconfigdb/types/global_config.py` & `siriuspy-2.74.0/siriuspy/clientconfigdb/types/global_config.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.73.0/siriuspy/clientconfigdb/types/si_bbadata.py` & `siriuspy-2.74.0/siriuspy/clientconfigdb/types/si_bbadata.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.73.0/siriuspy/clientconfigdb/types/si_bbbproc.py` & `siriuspy-2.74.0/siriuspy/clientconfigdb/types/si_bbbproc.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.73.0/siriuspy/clientconfigdb/types/si_chromcorr_params.py` & `siriuspy-2.74.0/siriuspy/clientconfigdb/types/si_chromcorr_params.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.73.0/siriuspy/clientconfigdb/types/si_fastorbcorr_respm.py` & `siriuspy-2.74.0/siriuspy/clientconfigdb/types/si_fastorbcorr_respm.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.73.0/siriuspy/clientconfigdb/types/si_fofb.py` & `siriuspy-2.74.0/siriuspy/clientconfigdb/types/si_fofb.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.73.0/siriuspy/clientconfigdb/types/si_id.py` & `siriuspy-2.74.0/siriuspy/clientconfigdb/types/si_id.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.73.0/siriuspy/clientconfigdb/types/si_orbcorr_respm.py` & `siriuspy-2.74.0/siriuspy/clientconfigdb/types/si_orbcorr_respm.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.73.0/siriuspy/clientconfigdb/types/si_orbit.py` & `siriuspy-2.74.0/siriuspy/clientconfigdb/types/si_orbit.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.73.0/siriuspy/clientconfigdb/types/si_tunecorr_params.py` & `siriuspy-2.74.0/siriuspy/clientconfigdb/types/si_tunecorr_params.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.73.0/siriuspy/clientconfigdb/types/tb_normalized.py` & `siriuspy-2.74.0/siriuspy/clientconfigdb/types/tb_normalized.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.73.0/siriuspy/clientconfigdb/types/tb_orbcorr_respm.py` & `siriuspy-2.74.0/siriuspy/clientconfigdb/types/tb_orbcorr_respm.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.73.0/siriuspy/clientconfigdb/types/tb_orbit.py` & `siriuspy-2.74.0/siriuspy/clientconfigdb/types/tb_orbit.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.73.0/siriuspy/clientconfigdb/types/tb_posang_respm.py` & `siriuspy-2.74.0/siriuspy/clientconfigdb/types/tb_posang_respm.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.73.0/siriuspy/clientconfigdb/types/ts_orbcorr_respm.py` & `siriuspy-2.74.0/siriuspy/clientconfigdb/types/ts_orbcorr_respm.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.73.0/siriuspy/clientconfigdb/types/ts_orbit.py` & `siriuspy-2.74.0/siriuspy/clientconfigdb/types/ts_orbit.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.73.0/siriuspy/clientconfigdb/types/ts_posang_respm.py` & `siriuspy-2.74.0/siriuspy/clientconfigdb/types/ts_posang_respm.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.73.0/siriuspy/clientweb/implementation.py` & `siriuspy-2.74.0/siriuspy/clientweb/implementation.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.73.0/siriuspy/csdev.py` & `siriuspy-2.74.0/siriuspy/csdev.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.73.0/siriuspy/currinfo/csdev.py` & `siriuspy-2.74.0/siriuspy/currinfo/csdev.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.73.0/siriuspy/currinfo/lifetime/main.py` & `siriuspy-2.74.0/siriuspy/currinfo/lifetime/main.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.73.0/siriuspy/currinfo/main.py` & `siriuspy-2.74.0/siriuspy/currinfo/main.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.73.0/siriuspy/cycle/__init__.py` & `siriuspy-2.74.0/siriuspy/cycle/__init__.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.73.0/siriuspy/cycle/bo_cycle_data.py` & `siriuspy-2.74.0/siriuspy/cycle/bo_cycle_data.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.73.0/siriuspy/cycle/conn.py` & `siriuspy-2.74.0/siriuspy/cycle/conn.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.73.0/siriuspy/cycle/fc_cycle_data.py` & `siriuspy-2.74.0/siriuspy/cycle/fc_cycle_data.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.73.0/siriuspy/cycle/li_cycle_data.py` & `siriuspy-2.74.0/siriuspy/cycle/li_cycle_data.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.73.0/siriuspy/cycle/main.py` & `siriuspy-2.74.0/siriuspy/cycle/main.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.73.0/siriuspy/cycle/util.py` & `siriuspy-2.74.0/siriuspy/cycle/util.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.73.0/siriuspy/devices/__init__.py` & `siriuspy-2.74.0/siriuspy/devices/__init__.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.73.0/siriuspy/devices/bbb.py` & `siriuspy-2.74.0/siriuspy/devices/bbb.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.73.0/siriuspy/devices/bpm.py` & `siriuspy-2.74.0/siriuspy/devices/bpm.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,9 @@
-"""."""
+"""BPM devices."""
+
 import time as _time
 from threading import Event as _Flag
 import numpy as _np
 
 from .device import Device as _Device, Devices as _Devices, \
     ProptyDevice as _ProptyDevice
 from ..diagbeam.bpm.csdev import Const as _csbpm
@@ -10,17 +11,17 @@
 from ..namesys import SiriusPVName as _PVName
 
 
 class BPM(_Device):
     """BPM Device."""
 
     ACQSTATES_NOTOK = {
-            _csbpm.AcqStates.Error, _csbpm.AcqStates.No_Memory,
-            _csbpm.AcqStates.Too_Few_Samples,
-            _csbpm.AcqStates.Too_Many_Samples, _csbpm.AcqStates.Acq_Overflow}
+        _csbpm.AcqStates.Error, _csbpm.AcqStates.No_Memory,
+        _csbpm.AcqStates.Too_Few_Samples,
+        _csbpm.AcqStates.Too_Many_Samples, _csbpm.AcqStates.Acq_Overflow}
     ACQSTATES_STARTED = {
         _csbpm.AcqStates.Waiting, _csbpm.AcqStates.External_Trig,
         _csbpm.AcqStates.Data_Trig, _csbpm.AcqStates.Software_Trig,
         _csbpm.AcqStates.Acquiring}
     ACQSTATES_FINISHED = {_csbpm.AcqStates.Idle, _csbpm.AcqStates.Aborted}
     ACQSTATES_FINISHED |= ACQSTATES_NOTOK
 
@@ -883,15 +884,15 @@
             return prop.replace('GEN', 'PM')
         elif prop.startswith('ACQ'):
             return prop.replace('ACQ', 'ACQ_PM')
         return prop
 
 
 class FamBPMs(_Devices):
-    """."""
+    """Family of BPMs."""
 
     TIMEOUT = 10
     RFFEATT_MAX = 30
 
     class DEVICES:
         """."""
 
@@ -913,14 +914,15 @@
         devs = [
             BPM(dev, auto_mon=False, ispost_mortem=ispost_mortem)
             for dev in bpm_names]
 
         super().__init__(devname, devs)
         self._bpm_names = bpm_names
         self._csbpm = devs[0].csdata
+        self._initial_timestamps = None
 
         self._mturn_flags = dict()
         # NOTE: ACQCount-Mon need to be fixed on BPM's IOC
         # for bpm in devs:
         #     pvo = bpm.pv_object(bpm.get_propname('ACQCount-Mon'))
         #     pvo.auto_monitor = True
         #     self._mturn_flags[pvo.pvname] = _Flag()
@@ -1013,14 +1015,42 @@
         orbx = _np.array(orbx).T
         orby = _np.array(orby).T
 
         if not return_sum:
             return orbx, orby
         return orbx, orby, _np.array(possum).T
 
+    def get_mturn_timestamps(self, return_sum=False):
+        """Get Multiturn data timestamps.
+
+        Args:
+            return_sum (bool, optional): Whether or not to return BPMs sum
+                timestamps. Defaults to False.
+
+        Returns:
+            tsmps (numpy.ndarray, (160, N)): The i-th row has the timestamp of
+                the i-th bpm for the [horizontal, vertical, sum] signals
+                respectively. If return_sum is False, then N=2 instead of 3.
+
+        """
+        tsmps = _np.zeros((len(self._devices), 2+return_sum), dtype=float)
+        for i, bpm in enumerate(self._devices):
+            pvx = bpm.pv_object(bpm.get_propname('GEN_XArrayData'))
+            pvy = bpm.pv_object(bpm.get_propname('GEN_YArrayData'))
+            vax = pvx.get_timevars(timeout=self.TIMEOUT)
+            vay = pvy.get_timevars()
+            tsmps[i, 0] = pvx.timestamp if vax is None else vax['timestamp']
+            tsmps[i, 1] = pvy.timestamp if vay is None else vay['timestamp']
+            if not return_sum:
+                continue
+            pvs = bpm.pv_object(bpm.get_propname('GEN_SUMArrayData'))
+            vas = pvs.get_timevars()
+            tsmps[i, 2] = pvs.timestamp if vas is None else vas['timestamp']
+        return tsmps
+
     def get_sampling_frequency(self, rf_freq: float, acq_rate='') -> float:
         """Return the sampling frequency of the acquisition.
 
         Args:
             rf_freq (float): RF frequency.
             acq_rate (str, optional): acquisition rate. Defaults to ''.
             If empty string, it gets the configured acq. rate on BPMs
@@ -1203,27 +1233,29 @@
         """
         if mode not in ('direct', 'switching', 1, 3):
             raise ValueError('Value must be in ("direct", "switching", 1, 3).')
 
         for bpm in self._devices:
             bpm.switching_mode = mode
 
-    def mturn_update_initial_orbit(self, consider_sum=False):
+    def mturn_update_initial_timestamps(self, consider_sum=False):
         """Call this method before acquisition to get orbit for comparison."""
-        self._initial_orbs = self.get_mturn_orbit(return_sum=consider_sum)
+        self._initial_timestamps = self.get_mturn_timestamps(
+            return_sum=consider_sum)
 
     def mturn_reset_flags(self):
         """Reset Multiturn flags to wait for a new orbit update."""
         for flag in self._mturn_flags.values():
             flag.clear()
 
-    def mturn_reset_flags_and_update_initial_orbit(self, consider_sum=False):
+    def mturn_reset_flags_and_update_initial_timestamps(
+            self, consider_sum=False):
         """Set initial state to wait for orbit acquisition to start."""
         self.mturn_reset_flags()
-        self.mturn_update_initial_orbit(consider_sum)
+        self.mturn_update_initial_timestamps(consider_sum)
 
     def mturn_wait_update_flags(self, timeout=10):
         """Wait for all acquisition flags to be updated.
 
         Args:
             timeout (int, optional): Time to wait. Defaults to 10.
 
@@ -1237,93 +1269,73 @@
             t00 = _time.time()
             if not flag.wait(timeout=timeout):
                 return i + 1
             timeout -= _time.time() - t00
             timeout = max(timeout, 0)
         return 0
 
-    def mturn_wait_update_orbit(self, timeout=10, consider_sum=False) -> int:
-        """Call this method after acquisition to check if orbit was updated.
+    def mturn_wait_update_timestamps(
+            self, timeout=10, consider_sum=False) -> int:
+        """Call this method after acquisition to check if data was updated.
 
         For this method to work it is necessary to call
-            mturn_update_initial_orbit
+            mturn_update_initial_timestamps
         before the acquisition starts, so that a reference for comparison is
         created.
 
         Args:
             timeout (int, optional): Waiting timeout. Defaults to 10.
             consider_sum (bool, optional): Whether to also wait for sum signal
                 to be updated. Defaults to False.
 
         Returns:
             int: code describing what happened:
-                -4: unknown error;
-                -3: initial orbit was not acquired before acquisition;
-                -2: TypeError ocurred (maybe because some of them are None);
-                -1: Orbits have different sizes;
-                =0: Orbit updated.
-                >0: Index of the first BPM which did not update plus 1.
+                -1: initial timestamps were not defined;
+                =0: data updated.
+                >0: index of the first BPM which did not update plus 1.
 
         """
-        orbs0, self._initial_orbs = self._initial_orbs, None
-        if orbs0 is None:
-            return -3
+        if self._initial_timestamps is None:
+            return -1
+
+        tsmp0 = self._initial_timestamps
         while timeout > 0:
             t00 = _time.time()
-            orbs = self.get_mturn_orbit(return_sum=consider_sum)
-            typ = False
-            try:
-                sizes = [
-                    min(o.shape[0], o0.shape[0]) for o, o0 in zip(orbs, orbs0)]
-                continue_ = max(sizes) != min(sizes)
-                errs = _np.any([
-                    _np.all(_np.isclose(o[:s], o0[:s]), axis=0)
-                    for o, o0, s in zip(orbs, orbs0, sizes)], axis=0)
-                continue_ |= _np.any(errs)
-            except TypeError:
-                typ = True
-                continue_ = True
-            if not continue_:
+            tsmp = self.get_mturn_timestamps(return_sum=consider_sum)
+            updated = _np.all(_np.equal(tsmp, tsmp0), axis=1)
+            if _np.all(updated):
                 return 0
             _time.sleep(0.1)
             timeout -= _time.time() - t00
 
-        if typ:
-            return -1
-        elif max(sizes) != min(sizes):
-            return -2
-        elif _np.any(errs):
-            return int(errs.nonzero()[0][0])+1
-        return -4
+        return int(_np.nonzero(~updated)[0][0])+1
 
     def mturn_wait_update(self, timeout=10, consider_sum=False) -> int:
-        """Combine mturn_wait_update_flags and mturn_wait_update_orbit.
+        """Combine all methods to wait update data.
 
         Args:
             timeout (int, optional): Waiting timeout. Defaults to 10.
             consider_sum (bool, optional): Whether to also wait for sum signal
                 to be updated. Defaults to False.
 
         Returns:
             int: code describing what happened:
-                -4: unknown error;
-                -3: initial orbit was not acquired before acquisition;
-                -2: TypeError ocurred (maybe because some of them are None);
-                -1: Orbits have different sizes;
-                =0: Orbit updated.
-                >0: Index of the first BPM which did not update plus 1.
+                -1: initial timestamps were not defined;
+                =0: data updated.
+                >0: index of the first BPM which did not update plus 1.
 
         """
         t00 = _time.time()
         ret = self.mturn_wait_update_flags(timeout)
         if ret > 0:
             return ret
         timeout -= _time.time() - t00
 
-        return self.mturn_wait_update_orbit(timeout, consider_sum=consider_sum)
+        return self.mturn_wait_update_timestamps(
+            timeout, consider_sum=consider_sum)
 
     def _mturn_set_flag(self, pvname, **kwargs):
         _ = kwargs
         self._mturn_flags[pvname].set()
 
 
 class BPMLogicalTrigger(_ProptyDevice):
```

### Comparing `siriuspy-2.73.0/siriuspy/devices/currinfo.py` & `siriuspy-2.74.0/siriuspy/devices/currinfo.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.73.0/siriuspy/devices/dcct.py` & `siriuspy-2.74.0/siriuspy/devices/dcct.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.73.0/siriuspy/devices/device.py` & `siriuspy-2.74.0/siriuspy/devices/device.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.73.0/siriuspy/devices/egun.py` & `siriuspy-2.74.0/siriuspy/devices/egun.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.73.0/siriuspy/devices/energy.py` & `siriuspy-2.74.0/siriuspy/devices/energy.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.73.0/siriuspy/devices/fofb.py` & `siriuspy-2.74.0/siriuspy/devices/fofb.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.73.0/siriuspy/devices/ict.py` & `siriuspy-2.74.0/siriuspy/devices/ict.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.73.0/siriuspy/devices/ids.py` & `siriuspy-2.74.0/siriuspy/devices/ids.py`

 * *Files 4% similar despite different names*

```diff
@@ -108,28 +108,29 @@
 
     class DEVICES:
         """."""
 
         EPU50_10SB = 'SI-10SB:ID-EPU50'
         ALL = (EPU50_10SB, )
 
+    # NOTE: move this info to IDSearch?
     _idparam_fields = (
         'PERIOD',  # [mm]
         'PHASE_PARK',  # [mm]
         'GAP_PARK',  # [mm]
         )
 
     _dev2params = {
         DEVICES.EPU50_10SB:
-            _get_namedtuple('IDParameters',
-                _idparam_fields, (50.0, 0, 300.0)),
+            _get_namedtuple(
+                'IDParameters', _idparam_fields, (50.0, 0, 300.0)),
         }
 
     _short_shut_eye = 0.1  # [s]
-    _default_timeout = 5  # [s]
+    _default_timeout = 8  # [s]
 
     _properties = (
         'BeamLineCtrlEnbl-Sel', 'BeamLineCtrlEnbl-Sts',
         'EnblPwrAll-Cmd', 'PwrPhase-Mon', 'PwrGap-Mon',
         'EnblAndReleasePhase-Sel', 'EnblAndReleasePhase-Sts',
         'AllowedToChangePhase-Mon',
         'EnblAndReleaseGap-Sel', 'EnblAndReleaseGap-Sts',
@@ -181,28 +182,42 @@
 
     @property
     def phase_speed_max(self):
         """Return max phase speed readback [mm/s]."""
         return self['MaxPhaseSpeed-RB']
 
     @property
+    def phase_speed_max_lims(self):
+        """."""
+        ctrl = self.pv_ctrlvars('MaxPhaseSpeed-SP')
+        lims = [ctrl['lower_ctrl_limit'], ctrl['upper_ctrl_limit']]
+        return lims
+
+    @property
     def gap_speed(self):
         """Return gap speed readback [mm/s]."""
         return self['GapSpeed-RB']
 
     @property
     def gap_speed_mon(self):
         """Return gap speed monitor [mm/s]."""
         return self['GapSpeed-Mon']
 
     @property
     def gap_speed_max(self):
         """Return max gap speed readback [mm/s]."""
         return self['MaxGapSpeed-RB']
 
+    @property
+    def gap_speed_max_lims(self):
+        """."""
+        ctrl = self.pv_ctrlvars('MaxGapSpeed-SP')
+        lims = [ctrl['lower_ctrl_limit'], ctrl['upper_ctrl_limit']]
+        return lims
+
     # --- phase ---
 
     @property
     def phase(self):
         """Return EPU phase readback [mm]."""
         return self['Phase-RB']
 
@@ -308,84 +323,81 @@
             _time.sleep(min(EPU._short_shut_eye, timeout))
             if _time.time() - time_init > timeout:
                 return False
         return True
 
     # --- cmd_beamline and cmd_drive
 
-    def cmd_drive_turn_on(self, timeout=None):
+    def cmd_drive_turn_power_on(self, timeout=None):
         """Command turn phase and gap drives on."""
         if self.is_phase_drive_powered and self.is_gap_drive_powered:
             return True
         self['EnblPwrAll-Cmd'] = 1
-        props_values = {
-            'PwrPhase-Mon': 0,  # value compared to in 'not equal' operation
-            'PwrGap-Mon': 0,  # value compared to in 'not equal' operation
-            }
-        return self._wait(props_values, timeout=timeout, comp='ne')
+        props_values = {'PwrPhase-Mon': 1, 'PwrGap-Mon': 1}
+        return self._wait(props_values, timeout=timeout)
 
     def cmd_beamline_ctrl_enable(self, timeout=None):
         """Command enable bealine EPU control."""
-        return self._set_sp('BeamLineCtrlEnbl-Sel', 1, timeout)
+        return self._write_sp('BeamLineCtrlEnbl-Sel', 1, timeout)
 
     def cmd_beamline_ctrl_disable(self, timeout=None):
         """Command disable bealine EPU control."""
-        return self._set_sp('BeamLineCtrlEnbl-Sel', 0, timeout)
+        return self._write_sp('BeamLineCtrlEnbl-Sel', 0, timeout)
 
     # --- cmd_set ---
 
     def cmd_set_phase(self, phase, timeout=None):
         """Command to set EPU target phase for movement [mm]."""
-        return self._set_sp('Phase-SP', phase, timeout)
+        return self._write_sp('Phase-SP', phase, timeout)
 
     def cmd_set_gap(self, gap, timeout=None):
         """Command to set EPU target gap for movement [mm]."""
-        return self._set_sp('Gap-SP', gap, timeout)
+        return self._write_sp('Gap-SP', gap, timeout)
 
     def cmd_set_phase_speed(self, phase_speed, timeout=None):
         """Command to set EPU cruise phase speed for movement [mm/s]."""
-        return self._set_sp('PhaseSpeed-SP', phase_speed, timeout)
+        return self._write_sp('PhaseSpeed-SP', phase_speed, timeout)
 
     def cmd_set_gap_speed(self, gap_speed, timeout=None):
         """Command to set EPU cruise gap speed for movement [mm/s]."""
-        return self._set_sp('GapSpeed-SP', gap_speed, timeout)
+        return self._write_sp('GapSpeed-SP', gap_speed, timeout)
 
     def cmd_set_phase_speed_max(self, phase_speed_max, timeout=None):
         """Command to set EPU max cruise phase speed for movement [mm/s]."""
-        return self._set_sp('MaxPhaseSpeed-SP', phase_speed_max, timeout)
+        return self._write_sp('MaxPhaseSpeed-SP', phase_speed_max, timeout)
 
     def cmd_set_gap_speed_max(self, gap_speed_max, timeout=None):
         """Command to set EPU max cruise gap speed for movement [mm/s]."""
-        return self._set_sp('MaxGapSpeed-SP', gap_speed_max, timeout)
+        return self._write_sp('MaxGapSpeed-SP', gap_speed_max, timeout)
 
     # --- cmd_move disable/enable ---
 
     def cmd_move_phase_enable(self, timeout=None):
         """Command to release and enable EPU phase movement."""
-        # return self._set_sp('EnblAndReleasePhase-Sel', 1, timeout)
-        self['EnblAndReleasePhase-Sel'] = 1
-        return True
+        # self['EnblAndReleasePhase-Sel'] = 1
+        # return True
+        return self._write_sp('EnblAndReleasePhase-Sel', 1, timeout)
 
     def cmd_move_phase_disable(self, timeout=None):
         """Command to disable and break EPU phase movement."""
-        # return self._set_sp('EnblAndReleasePhase-Sel', 0, timeout)
-        self['EnblAndReleasePhase-Sel'] = 0
-        return True
+        # self['EnblAndReleasePhase-Sel'] = 0
+        # return True
+        return self._write_sp('EnblAndReleasePhase-Sel', 0, timeout)
 
     def cmd_move_gap_enable(self, timeout=None):
         """Command to release and enable EPU gap movement."""
-        # return self._set_sp('EnblAndReleaseGap-Sel', 1, timeout)
-        self['EnblAndReleaseGap-Sel'] = 1
-        return True
+        # self['EnblAndReleaseGap-Sel'] = 1
+        # return True
+        return self._write_sp('EnblAndReleaseGap-Sel', 1, timeout)
 
     def cmd_move_gap_disable(self, timeout=None):
         """Command to disable and break EPU gap movement."""
-        # return self._set_sp('EnblAndReleaseGap-Sel', 0, timeout)
-        self['EnblAndReleaseGap-Sel'] = 0
-        return True
+        # self['EnblAndReleaseGap-Sel'] = 0
+        # return True
+        return self._write_sp('EnblAndReleaseGap-Sel', 0, timeout)
 
     def cmd_move_enable(self, timeout=None):
         """Command to release and enable EPU phase and gap movements."""
         success = True
         success &= self.cmd_move_phase_enable(timeout=timeout)
         success &= self.cmd_move_gap_enable(timeout=timeout)
         return success
@@ -400,26 +412,27 @@
     # -- cmd_move
 
     def cmd_move_stop(self, timeout=None):
         """Command to interrupt and then enable phase and gap movements."""
         timeout = timeout or self._default_timeout
 
         # wait for not busy state
-        if self.cmd_wait_while_busy(timeout=timeout):
+        if not self.cmd_wait_while_busy(timeout=timeout):
             return False
 
         # send stop command
-        self['Stop-Cmd'] = 1
+        self.cmd_move_disable()
+        # self['Stop-Cmd'] = 1
 
         # check for successful stop
-        if self.cmd_wait_while_busy(timeout=timeout):
+        if not self.cmd_wait_while_busy(timeout=timeout):
             return False
         success = True
-        success &= super()._wait('Moving-Mon', 0, tiemout=timeout)
-        success &= super()._wait('IsBusy-Mon', 0, tiemout=timeout)
+        success &= super()._wait('Moving-Mon', 0, timeout=timeout)
+        success &= super()._wait('IsBusy-Mon', 0, timeout=timeout)
         if not success:
             return False
 
         # enable movement again
         return self.cmd_move_enable(timeout=timeout)
 
     def cmd_move_phase_start(self, timeout=None):
@@ -434,17 +447,17 @@
         """Command to set and start phase and gap movements."""
         # calc ETA
         dtime_phase = abs(phase - self.phase_mon) / self.phase_speed
         dtime_gap = abs(gap - self.gap_mon) / self.gap_speed
         dtime_max = max(dtime_phase, dtime_gap)
 
         # additional percentual in ETA
-        tol_gap = 0.002  # [mm]
-        tol_phase = 0.002  # [mm]
-        tol_dtime = 100  # [%]
+        tol_gap = 0.01  # [mm]
+        tol_phase = 0.01  # [mm]
+        tol_dtime = 300  # [%]
         tol_factor = (1 + tol_dtime/100)
         tol_total = tol_factor * dtime_max + 5
 
         # set target phase and gap
         if not self.cmd_set_phase(phase=phase, timeout=timeout):
             return False
         if not self.cmd_set_gap(gap=gap, timeout=timeout):
@@ -480,15 +493,15 @@
 
     # --- cmd_reset
 
     def cmd_device_reset(self, timeout=None):
         """Command to reset EPU to a standard movement state."""
         success = True
         success &= self.cmd_beamline_ctrl_disable(timeout=timeout)
-        success &= self.cmd_drive_turn_on(timeout=timeout)
+        success &= self.cmd_drive_turn_power_on(timeout=timeout)
         success &= self.cmd_move_enable(timeout=timeout)
         return success
 
     # --- private methods ---
 
     def _move_start(self, cmd_propty, timeout=None):
         """."""
@@ -499,27 +512,27 @@
             return False
 
         # send move command
         self[cmd_propty] = 1
 
         return True
 
-    def _set_sp(self, propties_sp, values, timeout=None):
+    def _write_sp(self, propties_sp, values, timeout=None):
         timeout = timeout or self._default_timeout
         if isinstance(propties_sp, str):
             propties_sp = (propties_sp, )
             values = (values, )
         success = True
         for propty_sp, value in zip(propties_sp, values):
-            if value == self[propty_sp]:
-                continue
+            propty_rb = propty_sp.replace('-SP', '-RB').replace('-Sel', '-Sts')
+            # if self[propty_rb] == value:
+            #     continue
             if not self.cmd_wait_while_busy(timeout=timeout):
                 return False
             self[propty_sp] = value
-            propty_rb = propty_sp.replace('-SP', '-RB').replace('-Sel', '-Sts')
             success &= super()._wait(
                 propty_rb, value, timeout=timeout, comp='eq')
         return success
 
     def _wait(self, props_values, timeout=None, comp='eq'):
         timeout = timeout or self._default_timeout
         success = True
```

### Comparing `siriuspy-2.73.0/siriuspy/devices/injctrl.py` & `siriuspy-2.74.0/siriuspy/devices/injctrl.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.73.0/siriuspy/devices/injsys.py` & `siriuspy-2.74.0/siriuspy/devices/injsys.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.73.0/siriuspy/devices/lienergy.py` & `siriuspy-2.74.0/siriuspy/devices/lienergy.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.73.0/siriuspy/devices/lillrf.py` & `siriuspy-2.74.0/siriuspy/devices/lillrf.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.73.0/siriuspy/devices/machshift.py` & `siriuspy-2.74.0/siriuspy/devices/machshift.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.73.0/siriuspy/devices/modltr.py` & `siriuspy-2.74.0/siriuspy/devices/modltr.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.73.0/siriuspy/devices/orbit_interlock.py` & `siriuspy-2.74.0/siriuspy/devices/orbit_interlock.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.73.0/siriuspy/devices/posang.py` & `siriuspy-2.74.0/siriuspy/devices/posang.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.73.0/siriuspy/devices/psconv.py` & `siriuspy-2.74.0/siriuspy/devices/psconv.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.73.0/siriuspy/devices/pssofb.py` & `siriuspy-2.74.0/siriuspy/devices/pssofb.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.73.0/siriuspy/devices/pstesters.py` & `siriuspy-2.74.0/siriuspy/devices/pstesters.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.73.0/siriuspy/devices/pwrsupply.py` & `siriuspy-2.74.0/siriuspy/devices/pwrsupply.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.73.0/siriuspy/devices/rf.py` & `siriuspy-2.74.0/siriuspy/devices/rf.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.73.0/siriuspy/devices/screen.py` & `siriuspy-2.74.0/siriuspy/devices/screen.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.73.0/siriuspy/devices/sofb.py` & `siriuspy-2.74.0/siriuspy/devices/sofb.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.73.0/siriuspy/devices/syncd.py` & `siriuspy-2.74.0/siriuspy/devices/syncd.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.73.0/siriuspy/devices/timing.py` & `siriuspy-2.74.0/siriuspy/devices/timing.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.73.0/siriuspy/devices/tune.py` & `siriuspy-2.74.0/siriuspy/devices/tune.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.73.0/siriuspy/diagbeam/bpm/csdev.py` & `siriuspy-2.74.0/siriuspy/diagbeam/bpm/csdev.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.73.0/siriuspy/diagbeam/dcct/csdev.py` & `siriuspy-2.74.0/siriuspy/diagbeam/dcct/csdev.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.73.0/siriuspy/diagbeam/ict/csdev.py` & `siriuspy-2.74.0/siriuspy/diagbeam/ict/csdev.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.73.0/siriuspy/diagbeam/screen/csdev.py` & `siriuspy-2.74.0/siriuspy/diagbeam/screen/csdev.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.73.0/siriuspy/diagbeam/slit/csdev.py` & `siriuspy-2.74.0/siriuspy/diagbeam/slit/csdev.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.73.0/siriuspy/diagsys/app.py` & `siriuspy-2.74.0/siriuspy/diagsys/app.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.73.0/siriuspy/diagsys/lidiag/csdev.py` & `siriuspy-2.74.0/siriuspy/diagsys/lidiag/csdev.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.73.0/siriuspy/diagsys/lidiag/main.py` & `siriuspy-2.74.0/siriuspy/diagsys/lidiag/main.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.73.0/siriuspy/diagsys/lidiag/pvs.py` & `siriuspy-2.74.0/siriuspy/diagsys/lidiag/pvs.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.73.0/siriuspy/diagsys/psdiag/csdev.py` & `siriuspy-2.74.0/siriuspy/diagsys/psdiag/csdev.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.73.0/siriuspy/diagsys/psdiag/main.py` & `siriuspy-2.74.0/siriuspy/diagsys/psdiag/main.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.73.0/siriuspy/diagsys/psdiag/pvs.py` & `siriuspy-2.74.0/siriuspy/diagsys/psdiag/pvs.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.73.0/siriuspy/diagsys/pudiag/csdev.py` & `siriuspy-2.74.0/siriuspy/diagsys/pudiag/csdev.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.73.0/siriuspy/diagsys/pudiag/main.py` & `siriuspy-2.74.0/siriuspy/diagsys/pudiag/main.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.73.0/siriuspy/diagsys/pudiag/pvs.py` & `siriuspy-2.74.0/siriuspy/diagsys/pudiag/pvs.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.73.0/siriuspy/diagsys/pvs.py` & `siriuspy-2.74.0/siriuspy/diagsys/pvs.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.73.0/siriuspy/diagsys/rfdiag/csdev.py` & `siriuspy-2.74.0/siriuspy/diagsys/rfdiag/csdev.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.73.0/siriuspy/diagsys/rfdiag/main.py` & `siriuspy-2.74.0/siriuspy/diagsys/rfdiag/main.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.73.0/siriuspy/diagsys/rfdiag/pvs.py` & `siriuspy-2.74.0/siriuspy/diagsys/rfdiag/pvs.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.73.0/siriuspy/envars.py` & `siriuspy-2.74.0/siriuspy/envars.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.73.0/siriuspy/epics/multiproc.py` & `siriuspy-2.74.0/siriuspy/epics/multiproc.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.73.0/siriuspy/epics/properties.py` & `siriuspy-2.74.0/siriuspy/epics/properties.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.73.0/siriuspy/epics/pv_fake.py` & `siriuspy-2.74.0/siriuspy/epics/pv_fake.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.73.0/siriuspy/epics/pv_time_serie.py` & `siriuspy-2.74.0/siriuspy/epics/pv_time_serie.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.73.0/siriuspy/fofb/csdev.py` & `siriuspy-2.74.0/siriuspy/fofb/csdev.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.73.0/siriuspy/fofb/main.py` & `siriuspy-2.74.0/siriuspy/fofb/main.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.73.0/siriuspy/injctrl/bias_feedback.py` & `siriuspy-2.74.0/siriuspy/injctrl/bias_feedback.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.73.0/siriuspy/injctrl/csdev.py` & `siriuspy-2.74.0/siriuspy/injctrl/csdev.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.73.0/siriuspy/injctrl/main.py` & `siriuspy-2.74.0/siriuspy/injctrl/main.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.73.0/siriuspy/machshift/csdev.py` & `siriuspy-2.74.0/siriuspy/machshift/csdev.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.73.0/siriuspy/machshift/macreport.py` & `siriuspy-2.74.0/siriuspy/machshift/macreport.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.73.0/siriuspy/machshift/macschedule.py` & `siriuspy-2.74.0/siriuspy/machshift/macschedule.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.73.0/siriuspy/machshift/main.py` & `siriuspy-2.74.0/siriuspy/machshift/main.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.73.0/siriuspy/machshift/test_macreport.py` & `siriuspy-2.74.0/siriuspy/machshift/test_macreport.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.73.0/siriuspy/machshift/utils.py` & `siriuspy-2.74.0/siriuspy/machshift/utils.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.73.0/siriuspy/magnet/data.py` & `siriuspy-2.74.0/siriuspy/magnet/data.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.73.0/siriuspy/magnet/excdata.py` & `siriuspy-2.74.0/siriuspy/magnet/excdata.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.73.0/siriuspy/magnet/factory.py` & `siriuspy-2.74.0/siriuspy/magnet/factory.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.73.0/siriuspy/magnet/normalizer.py` & `siriuspy-2.74.0/siriuspy/magnet/normalizer.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.73.0/siriuspy/magnet/util.py` & `siriuspy-2.74.0/siriuspy/magnet/util.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.73.0/siriuspy/meas/csdev.py` & `siriuspy-2.74.0/siriuspy/meas/csdev.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.73.0/siriuspy/meas/liemit/csdev.py` & `siriuspy-2.74.0/siriuspy/meas/liemit/csdev.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.73.0/siriuspy/meas/liemit/main.py` & `siriuspy-2.74.0/siriuspy/meas/liemit/main.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.73.0/siriuspy/meas/lienergy/csdev.py` & `siriuspy-2.74.0/siriuspy/meas/lienergy/csdev.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.73.0/siriuspy/meas/lienergy/main.py` & `siriuspy-2.74.0/siriuspy/meas/lienergy/main.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.73.0/siriuspy/meas/util.py` & `siriuspy-2.74.0/siriuspy/meas/util.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.73.0/siriuspy/namesys/implementation.py` & `siriuspy-2.74.0/siriuspy/namesys/implementation.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.73.0/siriuspy/optics/lattice_survey.py` & `siriuspy-2.74.0/siriuspy/optics/lattice_survey.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.73.0/siriuspy/opticscorr/base.py` & `siriuspy-2.74.0/siriuspy/opticscorr/base.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.73.0/siriuspy/opticscorr/chrom.py` & `siriuspy-2.74.0/siriuspy/opticscorr/chrom.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.73.0/siriuspy/opticscorr/csdev.py` & `siriuspy-2.74.0/siriuspy/opticscorr/csdev.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.73.0/siriuspy/opticscorr/opticscorr.py` & `siriuspy-2.74.0/siriuspy/opticscorr/opticscorr.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.73.0/siriuspy/opticscorr/tune.py` & `siriuspy-2.74.0/siriuspy/opticscorr/tune.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.73.0/siriuspy/opticscorr/utils.py` & `siriuspy-2.74.0/siriuspy/opticscorr/utils.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.73.0/siriuspy/oscilloscope/keysight.py` & `siriuspy-2.74.0/siriuspy/oscilloscope/keysight.py`

 * *Files 14% similar despite different names*

```diff
@@ -25,14 +25,15 @@
     import matplotlib.pyplot as plt
 
     scope = Keysight(scopesignal=ScopeSignals.SI_FILL_PATTERN)
     print(scope.scope_name)
     wavet, waved = scope.wfm_get_data()
     plt.plot(wavet, waved)
     plt.show()
+
     """
 
     def __init__(self, scope=None, scopesignal=None):
         """."""
         if scopesignal and isinstance(scopesignal, tuple):
             self.host = scopesignal[0]
             self.port = scopesignal[1]
@@ -118,14 +119,15 @@
         self.send_command(b":RUN\n", get_res=False)
         while len(dataraw) < datanum:
             dataraw = dataraw + self._socket.recv(datanum)
         dataraw = dataraw[0:-1]  # remove EOF char
 
         va1 = _np.array(list(dataraw)[0::2])
         va0 = _np.array(list(dataraw)[1::2])
+
         datay = ((va1 << 8) + va0 - 2**16*(va1 >> 7)) * yinc + yor
 
         datax = _np.arange(datay.size)*xinc
         return datax, datay, srate, bdw
 
     def wfm_get_data(self, channel=None):
         """Enable and get sccope waveform data."""
@@ -138,60 +140,68 @@
             self.wfm_config()
             tini = _time.time()
             print('Acquiring ' + self.chan)
             wavet, waved, srate1, bdw1 = self.wfm_acquire(channel)
             print('Total acquisition time:', _time.time() - tini)
             # self.send_command(b":WAVeform:STReaming ON\n", get_res=False)
         except Exception:
-            print("Unexpected error:", _sys.exc_info()[0])
-            print('Close connetion by exception')
+            print('Close connection by exception')
+            raise
+
         finally:
             self.close()
 
         return wavet, waved
 
     def stats_enable(self):
         """Enable scope measurement statistics info."""
         # Set bit order to MSB First
         self.send_command(b":MEASure:STATistics ON\n", get_res=False)
         self.send_command(b":MEASure:SENDvalid ON\n", get_res=False)
 
     def stats_acquire(self):
         """Return a dictionary of scope measurement statistics."""
         meas = self.send_command(b":MEASure:RESults?\n")
-        meas = meas.split(',')
-        data = dict()
-        for i in range(0, len(meas) - len(meas) % 8, 8):
-            datum = dict()
-            label = meas[i]
-            datum['current'] = float(meas[i+1])
-            datum['state'] = int(float(meas[i+2]))
-            datum['min'] = float(meas[i+3])
-            datum['max'] = float(meas[i+4])
-            datum['mean'] = float(meas[i+5])
-            datum['std_dev'] = float(meas[i+6])
-            datum['num_of_meas'] = int(float(meas[i+7]))
-            data[label] = datum
+        data = Keysight.process_stats_meas(meas)
         return data
 
     def stats_get_data(self):
         """."""
         self.connect()
         try:
             self.stats_enable()
             tini = _time.time()
             print('Acquiring ' + self.chan)
             data = self.stats_acquire()
             print('Total acquisition time:', _time.time() - tini)
         except Exception:
-            print("Unexpected error:", _sys.exc_info()[0])
-            print('Close connetion by exception')
+            print('Close connection by exception')
+            raise
         finally:
             self.close()
         return data
 
     def send_command(self, cmd, get_res=True):
         """."""
         self._socket.sendall(cmd)
         if get_res:
             return self._socket.recv(1024).decode('ascii')
         return
+
+    @staticmethod
+    def process_stats_meas(meas):
+        """Process stats measurents."""
+        # TODO: generalize or instantiate for each scope type
+        meas = meas.split(',')
+        data = dict()
+        for i in range(0, len(meas) - len(meas) % 8, 8):
+            datum = dict()
+            label = meas[i]
+            datum['current'] = float(meas[i+1])
+            datum['state'] = int(float(meas[i+2]))
+            datum['min'] = float(meas[i+3])
+            datum['max'] = float(meas[i+4])
+            datum['mean'] = float(meas[i+5])
+            datum['std_dev'] = float(meas[i+6])
+            datum['num_of_meas'] = int(float(meas[i+7]))
+            data[label] = datum
+        return data
```

### Comparing `siriuspy-2.73.0/siriuspy/posang/csdev.py` & `siriuspy-2.74.0/siriuspy/posang/csdev.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.73.0/siriuspy/posang/main.py` & `siriuspy-2.74.0/siriuspy/posang/main.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.73.0/siriuspy/posang/utils.py` & `siriuspy-2.74.0/siriuspy/posang/utils.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.73.0/siriuspy/pwrsupply/beaglebone.py` & `siriuspy-2.74.0/siriuspy/pwrsupply/beaglebone.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.73.0/siriuspy/pwrsupply/bsmp/commands.py` & `siriuspy-2.74.0/siriuspy/pwrsupply/bsmp/commands.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.73.0/siriuspy/pwrsupply/bsmp/constants.py` & `siriuspy-2.74.0/siriuspy/pwrsupply/bsmp/constants.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.73.0/siriuspy/pwrsupply/bsmp/entities.py` & `siriuspy-2.74.0/siriuspy/pwrsupply/bsmp/entities.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.73.0/siriuspy/pwrsupply/bsmp/factory.py` & `siriuspy-2.74.0/siriuspy/pwrsupply/bsmp/factory.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.73.0/siriuspy/pwrsupply/csdev.py` & `siriuspy-2.74.0/siriuspy/pwrsupply/csdev.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.73.0/siriuspy/pwrsupply/data.py` & `siriuspy-2.74.0/siriuspy/pwrsupply/data.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.73.0/siriuspy/pwrsupply/factory.py` & `siriuspy-2.74.0/siriuspy/pwrsupply/factory.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.73.0/siriuspy/pwrsupply/pructrl/__init__.py` & `siriuspy-2.74.0/siriuspy/pwrsupply/pructrl/__init__.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.73.0/siriuspy/pwrsupply/pructrl/pru.py` & `siriuspy-2.74.0/siriuspy/pwrsupply/pructrl/pru.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.73.0/siriuspy/pwrsupply/pructrl/prucontroller.py` & `siriuspy-2.74.0/siriuspy/pwrsupply/pructrl/prucontroller.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.73.0/siriuspy/pwrsupply/pructrl/prucparms.py` & `siriuspy-2.74.0/siriuspy/pwrsupply/pructrl/prucparms.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.73.0/siriuspy/pwrsupply/pructrl/psdevstate.py` & `siriuspy-2.74.0/siriuspy/pwrsupply/pructrl/psdevstate.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.73.0/siriuspy/pwrsupply/pructrl/udc.py` & `siriuspy-2.74.0/siriuspy/pwrsupply/pructrl/udc.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.73.0/siriuspy/pwrsupply/psctrl/__init__.py` & `siriuspy-2.74.0/siriuspy/pwrsupply/psctrl/__init__.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.73.0/siriuspy/pwrsupply/psctrl/pscontroller.py` & `siriuspy-2.74.0/siriuspy/pwrsupply/psctrl/pscontroller.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.73.0/siriuspy/pwrsupply/psctrl/pscreaders.py` & `siriuspy-2.74.0/siriuspy/pwrsupply/psctrl/pscreaders.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.73.0/siriuspy/pwrsupply/psctrl/pscstatus.py` & `siriuspy-2.74.0/siriuspy/pwrsupply/psctrl/pscstatus.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.73.0/siriuspy/pwrsupply/psctrl/pscwriters.py` & `siriuspy-2.74.0/siriuspy/pwrsupply/psctrl/pscwriters.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.73.0/siriuspy/pwrsupply/psctrl/psmodel.py` & `siriuspy-2.74.0/siriuspy/pwrsupply/psctrl/psmodel.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.73.0/siriuspy/pwrsupply/pssofb.py` & `siriuspy-2.74.0/siriuspy/pwrsupply/pssofb.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.73.0/siriuspy/pwrsupply/siggen.py` & `siriuspy-2.74.0/siriuspy/pwrsupply/siggen.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.73.0/siriuspy/ramp/conn.py` & `siriuspy-2.74.0/siriuspy/ramp/conn.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.73.0/siriuspy/ramp/magnet.py` & `siriuspy-2.74.0/siriuspy/ramp/magnet.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.73.0/siriuspy/ramp/ramp.py` & `siriuspy-2.74.0/siriuspy/ramp/ramp.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.73.0/siriuspy/ramp/reconst_factory.py` & `siriuspy-2.74.0/siriuspy/ramp/reconst_factory.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.73.0/siriuspy/ramp/test_reconst_factory.py` & `siriuspy-2.74.0/siriuspy/ramp/test_reconst_factory.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.73.0/siriuspy/ramp/testwfm.py` & `siriuspy-2.74.0/siriuspy/ramp/testwfm.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.73.0/siriuspy/ramp/util.py` & `siriuspy-2.74.0/siriuspy/ramp/util.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.73.0/siriuspy/ramp/waveform.py` & `siriuspy-2.74.0/siriuspy/ramp/waveform.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.73.0/siriuspy/search/bpms_search.py` & `siriuspy-2.74.0/siriuspy/search/bpms_search.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.73.0/siriuspy/search/hl_time_search.py` & `siriuspy-2.74.0/siriuspy/search/hl_time_search.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.73.0/siriuspy/search/id_search.py` & `siriuspy-2.74.0/siriuspy/search/id_search.py`

 * *Files 3% similar despite different names*

```diff
@@ -27,26 +27,30 @@
 
     _idname_2_idff = {
         'SI-06SB:ID-APU22': None,
         'SI-07SP:ID-APU22': None,
         'SI-08SB:ID-APU22': None,
         'SI-09SA:ID-APU22': None,
         'SI-10SB:ID-EPU50': {
-            'polarizations': ('horizontal', 'vertical', 'circular', ),
-            'kparameter': 'SI-10SB:ID-EPU:Gap-Mon',
+            'polarizations': (
+                'none', 'circularn', 'horizontal', 'circularp', 'vertical',
+                ),
+            'pparameter': 'SI-10SB:ID-EPU50:Phase-Mon',
+            'kparameter': 'SI-10SB:ID-EPU50:Gap-Mon',
             'ch1': 'SI-10SB:PS-CH-1:Current-SP',  # upstream
             'ch2': 'SI-10SB:PS-CH-2:Current-SP',  # downstream
             'cv1': 'SI-10SB:PS-CV-1:Current-SP',
             'cv2': 'SI-10SB:PS-CV-2:Current-SP',
             'qs1': 'SI-10SB:PS-QS-1:Current-SP',
             'qs2': 'SI-10SB:PS-QS-2:Current-SP',
         },
         'SI-11SP:ID-APU58': None,
         'SI-14SB:ID-WIG180': {
             'polarizations': ('horizontal', ),
+            'pparameter': None,
             'kparameter': 'SI-14SB:ID-WIG180:Gap-Mon',
             'ch1': 'SI-14SB:PS-CH-1:Current-SP',  # upstream
             'ch2': 'SI-14SB:PS-CH-2:Current-SP',  # downstream
         },
     }
 
     @staticmethod
@@ -89,14 +93,21 @@
 
     @staticmethod
     def conv_idname_2_idff(idname):
         """Return the IDFF dictionary for a given ID name."""
         return dict(IDSearch._idname_2_idff[idname])
 
     @staticmethod
+    def conv_idname_2_pparameter_propty(idname):
+        """."""
+        idff = IDSearch.conv_idname_2_idff(idname)
+        pvname = _SiriusPVName(idff['pparameter'])
+        return pvname.propty
+
+    @staticmethod
     def conv_idname_2_kparameter_propty(idname):
         """."""
         idff = IDSearch.conv_idname_2_idff(idname)
         pvname = _SiriusPVName(idff['kparameter'])
         return pvname.propty
 
     @staticmethod
```

### Comparing `siriuspy-2.73.0/siriuspy/search/ioc_search.py` & `siriuspy-2.74.0/siriuspy/search/ioc_search.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.73.0/siriuspy/search/ll_time_search.py` & `siriuspy-2.74.0/siriuspy/search/ll_time_search.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.73.0/siriuspy/search/ma_search.py` & `siriuspy-2.74.0/siriuspy/search/ma_search.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.73.0/siriuspy/search/ps_search.py` & `siriuspy-2.74.0/siriuspy/search/ps_search.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.73.0/siriuspy/simul/simfactory.py` & `siriuspy-2.74.0/siriuspy/simul/simfactory.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.73.0/siriuspy/simul/simps.py` & `siriuspy-2.74.0/siriuspy/simul/simps.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.73.0/siriuspy/simul/simpv.py` & `siriuspy-2.74.0/siriuspy/simul/simpv.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.73.0/siriuspy/simul/simulation.py` & `siriuspy-2.74.0/siriuspy/simul/simulation.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.73.0/siriuspy/simul/simulator.py` & `siriuspy-2.74.0/siriuspy/simul/simulator.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.73.0/siriuspy/sofb/base_class.py` & `siriuspy-2.74.0/siriuspy/sofb/base_class.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.73.0/siriuspy/sofb/bpms.py` & `siriuspy-2.74.0/siriuspy/sofb/bpms.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.73.0/siriuspy/sofb/correctors.py` & `siriuspy-2.74.0/siriuspy/sofb/correctors.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.73.0/siriuspy/sofb/csdev.py` & `siriuspy-2.74.0/siriuspy/sofb/csdev.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.73.0/siriuspy/sofb/main.py` & `siriuspy-2.74.0/siriuspy/sofb/main.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.73.0/siriuspy/sofb/matrix.py` & `siriuspy-2.74.0/siriuspy/sofb/matrix.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.73.0/siriuspy/sofb/orbit.py` & `siriuspy-2.74.0/siriuspy/sofb/orbit.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.73.0/siriuspy/sofb/utils.py` & `siriuspy-2.74.0/siriuspy/sofb/utils.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.73.0/siriuspy/stabinfo/csdev.py` & `siriuspy-2.74.0/siriuspy/stabinfo/csdev.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.73.0/siriuspy/stabinfo/main.py` & `siriuspy-2.74.0/siriuspy/stabinfo/main.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.73.0/siriuspy/thread.py` & `siriuspy-2.74.0/siriuspy/thread.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.73.0/siriuspy/timesys/csdev.py` & `siriuspy-2.74.0/siriuspy/timesys/csdev.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.73.0/siriuspy/timesys/hl_classes.py` & `siriuspy-2.74.0/siriuspy/timesys/hl_classes.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.73.0/siriuspy/timesys/ll_classes.py` & `siriuspy-2.74.0/siriuspy/timesys/ll_classes.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.73.0/siriuspy/timesys/plot_network.py` & `siriuspy-2.74.0/siriuspy/timesys/plot_network.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.73.0/siriuspy/timesys/static_table.py` & `siriuspy-2.74.0/siriuspy/timesys/static_table.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.73.0/siriuspy/util.py` & `siriuspy-2.74.0/siriuspy/util.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.73.0/siriuspy.egg-info/PKG-INFO` & `siriuspy-2.74.0/siriuspy.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: siriuspy
-Version: 2.73.0
+Version: 2.74.0
 Summary: Development packages for Sirius
 Home-page: https://github.com/lnls-sirius/dev-packages
 Download-URL: https://github.com/lnls-sirius/dev-packages
 Author: lnls-sirius
 License: GNU GPLv3
 Classifier: Intended Audience :: Science/Research
 Classifier: Programming Language :: Python
```

### Comparing `siriuspy-2.73.0/siriuspy.egg-info/SOURCES.txt` & `siriuspy-2.74.0/siriuspy.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -148,14 +148,16 @@
 siriuspy/epics/pv_time_serie.py
 siriuspy/epics/threading.py
 siriuspy/fofb/__init__.py
 siriuspy/fofb/csdev.py
 siriuspy/fofb/main.py
 siriuspy/idff/__init__.py
 siriuspy/idff/config.py
+siriuspy/idff/csdev.py
+siriuspy/idff/main.py
 siriuspy/injctrl/__init__.py
 siriuspy/injctrl/bias_feedback.py
 siriuspy/injctrl/csdev.py
 siriuspy/injctrl/main.py
 siriuspy/machshift/__init__.py
 siriuspy/machshift/csdev.py
 siriuspy/machshift/macreport.py
```

### Comparing `siriuspy-2.73.0/tests/bsmp/test_bsmp.py` & `siriuspy-2.74.0/tests/bsmp/test_bsmp.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.73.0/tests/bsmp/test_commands.py` & `siriuspy-2.74.0/tests/bsmp/test_commands.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.73.0/tests/bsmp/test_entities.py` & `siriuspy-2.74.0/tests/bsmp/test_entities.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.73.0/tests/bsmp/test_serial.py` & `siriuspy-2.74.0/tests/bsmp/test_serial.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.73.0/tests/bsmp/test_types.py` & `siriuspy-2.74.0/tests/bsmp/test_types.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.73.0/tests/clientconfigdb/test_configdb_client.py` & `siriuspy-2.74.0/tests/clientconfigdb/test_configdb_client.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.73.0/tests/clientweb/test_implementation.py` & `siriuspy-2.74.0/tests/clientweb/test_implementation.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.73.0/tests/currinfo/lifetime/test_main.py` & `siriuspy-2.74.0/tests/currinfo/lifetime/test_main.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.73.0/tests/currinfo/test_csdev.py` & `siriuspy-2.74.0/tests/currinfo/test_csdev.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.73.0/tests/currinfo/test_main.py` & `siriuspy-2.74.0/tests/currinfo/test_main.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.73.0/tests/magnet/test_factory.py` & `siriuspy-2.74.0/tests/magnet/test_factory.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.73.0/tests/magnet/tests_normalizer.py` & `siriuspy-2.74.0/tests/magnet/tests_normalizer.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.73.0/tests/mock_servweb.py` & `siriuspy-2.74.0/tests/mock_servweb.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.73.0/tests/namesys/test_implementation.py` & `siriuspy-2.74.0/tests/namesys/test_implementation.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.73.0/tests/opticscorr/test_chrom.py` & `siriuspy-2.74.0/tests/opticscorr/test_chrom.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.73.0/tests/opticscorr/test_csdev.py` & `siriuspy-2.74.0/tests/opticscorr/test_csdev.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.73.0/tests/opticscorr/test_opticscorr.py` & `siriuspy-2.74.0/tests/opticscorr/test_opticscorr.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.73.0/tests/opticscorr/test_tune.py` & `siriuspy-2.74.0/tests/opticscorr/test_tune.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.73.0/tests/opticscorr/test_utils.py` & `siriuspy-2.74.0/tests/opticscorr/test_utils.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.73.0/tests/posang/test_csdev.py` & `siriuspy-2.74.0/tests/posang/test_csdev.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.73.0/tests/posang/test_main.py` & `siriuspy-2.74.0/tests/posang/test_main.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.73.0/tests/pwrsupply/db.py` & `siriuspy-2.74.0/tests/pwrsupply/db.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.73.0/tests/pwrsupply/pructrl/test_pru.py` & `siriuspy-2.74.0/tests/pwrsupply/pructrl/test_pru.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.73.0/tests/pwrsupply/psctrl/test_pscwriters.py` & `siriuspy-2.74.0/tests/pwrsupply/psctrl/test_pscwriters.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.73.0/tests/pwrsupply/test_csdev.py` & `siriuspy-2.74.0/tests/pwrsupply/test_csdev.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.73.0/tests/pwrsupply/test_data.py` & `siriuspy-2.74.0/tests/pwrsupply/test_data.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.73.0/tests/pwrsupply/test_siggen.py` & `siriuspy-2.74.0/tests/pwrsupply/test_siggen.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.73.0/tests/pwrsupply/variables.py` & `siriuspy-2.74.0/tests/pwrsupply/variables.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.73.0/tests/ramp/test_magnet.py` & `siriuspy-2.74.0/tests/ramp/test_magnet.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.73.0/tests/ramp/test_waveform.py` & `siriuspy-2.74.0/tests/ramp/test_waveform.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.73.0/tests/search/test_hl_time_search.py` & `siriuspy-2.74.0/tests/search/test_hl_time_search.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.73.0/tests/search/test_init.py` & `siriuspy-2.74.0/tests/search/test_init.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.73.0/tests/search/test_ll_time_search.py` & `siriuspy-2.74.0/tests/search/test_ll_time_search.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.73.0/tests/search/test_ma_search.py` & `siriuspy-2.74.0/tests/search/test_ma_search.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.73.0/tests/search/test_ps_search.py` & `siriuspy-2.74.0/tests/search/test_ps_search.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.73.0/tests/test_callbacks.py` & `siriuspy-2.74.0/tests/test_callbacks.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.73.0/tests/test_csdev.py` & `siriuspy-2.74.0/tests/test_csdev.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.73.0/tests/test_envars.py` & `siriuspy-2.74.0/tests/test_envars.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.73.0/tests/test_util.py` & `siriuspy-2.74.0/tests/test_util.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.73.0/tests/timesys/test_csdev.py` & `siriuspy-2.74.0/tests/timesys/test_csdev.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.73.0/tests/timesys/test_plot_network.py` & `siriuspy-2.74.0/tests/timesys/test_plot_network.py`

 * *Files identical despite different names*

