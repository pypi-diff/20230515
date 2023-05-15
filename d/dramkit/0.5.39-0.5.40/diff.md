# Comparing `tmp/dramkit-0.5.39.tar.gz` & `tmp/dramkit-0.5.40.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dramkit-0.5.39.tar", last modified: Fri May  5 14:54:02 2023, max compression
+gzip compressed data, was "dramkit-0.5.40.tar", last modified: Mon May 15 06:26:58 2023, max compression
```

## Comparing `dramkit-0.5.39.tar` & `dramkit-0.5.40.tar`

### file list

```diff
@@ -1,187 +1,188 @@
-drwxrwxrwx   0        0        0        0 2023-05-05 14:54:02.598603 dramkit-0.5.39/
--rw-rw-rw-   0        0        0     1072 2023-02-25 10:45:19.000000 dramkit-0.5.39/LICENSE
--rw-rw-rw-   0        0        0     1095 2023-05-05 14:54:02.597605 dramkit-0.5.39/PKG-INFO
--rw-rw-rw-   0        0        0      795 2022-05-06 14:18:52.000000 dramkit-0.5.39/README.md
-drwxrwxrwx   0        0        0        0 2023-05-05 14:54:02.478895 dramkit-0.5.39/dramkit/
--rw-rw-rw-   0        0        0      999 2023-04-24 03:43:26.000000 dramkit-0.5.39/dramkit/__init__.py
--rw-rw-rw-   0        0        0      662 2023-05-05 14:53:39.000000 dramkit-0.5.39/dramkit/_pkg_info.py
-drwxrwxrwx   0        0        0        0 2023-05-05 14:54:02.514800 dramkit-0.5.39/dramkit/_tmp/
--rw-rw-rw-   0        0        0     6600 2021-12-24 09:25:22.000000 dramkit-0.5.39/dramkit/_tmp/CRR.py
--rw-rw-rw-   0        0        0     1844 2022-08-02 09:50:33.000000 dramkit-0.5.39/dramkit/_tmp/CtrlPreTS.py
--rw-rw-rw-   0        0        0      515 2022-01-09 09:11:34.000000 dramkit-0.5.39/dramkit/_tmp/NPairSum.py
--rw-rw-rw-   0        0        0     3672 2021-12-24 09:25:22.000000 dramkit-0.5.39/dramkit/_tmp/PIDtest.py
--rw-rw-rw-   0        0        0     2316 2021-12-24 09:25:22.000000 dramkit-0.5.39/dramkit/_tmp/PIDtest2.py
--rw-rw-rw-   0        0        0     6152 2021-12-24 09:25:22.000000 dramkit-0.5.39/dramkit/_tmp/VMD.py
--rw-rw-rw-   0        0        0       25 2021-12-24 09:25:22.000000 dramkit-0.5.39/dramkit/_tmp/__init__.py
--rw-rw-rw-   0        0        0     2182 2021-12-24 09:25:22.000000 dramkit-0.5.39/dramkit/_tmp/cca_test.py
--rw-rw-rw-   0        0        0     1768 2021-12-24 09:25:22.000000 dramkit-0.5.39/dramkit/_tmp/dtw_test.py
--rw-rw-rw-   0        0        0    10656 2021-12-24 09:25:22.000000 dramkit-0.5.39/dramkit/_tmp/explore.py
--rw-rw-rw-   0        0        0     2857 2021-12-24 09:25:22.000000 dramkit-0.5.39/dramkit/_tmp/gini.py
--rw-rw-rw-   0        0        0      899 2021-12-24 09:25:22.000000 dramkit-0.5.39/dramkit/_tmp/merge_sort.py
--rw-rw-rw-   0        0        0      910 2021-12-24 09:25:22.000000 dramkit-0.5.39/dramkit/_tmp/mouse_move.py
--rw-rw-rw-   0        0        0     1600 2021-12-24 09:25:22.000000 dramkit-0.5.39/dramkit/_tmp/mpc_test1.py
--rw-rw-rw-   0        0        0     7521 2021-12-24 09:25:22.000000 dramkit-0.5.39/dramkit/_tmp/options_Implied_volatility.py
--rw-rw-rw-   0        0        0      501 2021-12-24 09:25:22.000000 dramkit-0.5.39/dramkit/_tmp/pf_test.py
--rw-rw-rw-   0        0        0     4142 2021-12-24 09:25:22.000000 dramkit-0.5.39/dramkit/_tmp/plot_test.py
--rw-rw-rw-   0        0        0     1567 2022-05-06 11:02:39.000000 dramkit-0.5.39/dramkit/_tmp/plot_test2.py
--rw-rw-rw-   0        0        0     2618 2022-07-06 06:24:15.000000 dramkit-0.5.39/dramkit/_tmp/simple_smooth.py
--rw-rw-rw-   0        0        0     1057 2023-03-17 03:20:46.000000 dramkit-0.5.39/dramkit/_tmp/test_async_washs.py
--rw-rw-rw-   0        0        0     1720 2023-04-03 01:16:22.000000 dramkit-0.5.39/dramkit/_tmp/test_await_timeout.py
--rw-rw-rw-   0        0        0      747 2021-12-24 09:25:22.000000 dramkit-0.5.39/dramkit/_tmp/test_backtrader.py
--rw-rw-rw-   0        0        0     1917 2023-02-16 09:04:46.000000 dramkit-0.5.39/dramkit/_tmp/test_chatgpt_v1.py
--rw-rw-rw-   0        0        0      657 2021-12-24 09:25:22.000000 dramkit-0.5.39/dramkit/_tmp/test_code.py
--rw-rw-rw-   0        0        0     3629 2022-04-13 14:32:40.000000 dramkit-0.5.39/dramkit/_tmp/test_find_peaks.py
--rw-rw-rw-   0        0        0      585 2023-01-29 09:46:43.000000 dramkit-0.5.39/dramkit/_tmp/test_get_var_name.py
--rw-rw-rw-   0        0        0     1263 2022-06-22 06:15:28.000000 dramkit-0.5.39/dramkit/_tmp/test_grading.py
--rw-rw-rw-   0        0        0     2193 2021-12-24 09:25:22.000000 dramkit-0.5.39/dramkit/_tmp/test_lr.py
--rw-rw-rw-   0        0        0     1154 2023-01-13 09:20:58.000000 dramkit-0.5.39/dramkit/_tmp/test_maxsort.py
--rw-rw-rw-   0        0        0      466 2023-04-06 07:48:43.000000 dramkit-0.5.39/dramkit/_tmp/test_multiprocessing.py
--rw-rw-rw-   0        0        0      318 2022-01-26 13:43:15.000000 dramkit-0.5.39/dramkit/_tmp/test_ocr.py
--rw-rw-rw-   0        0        0     1791 2022-04-22 14:45:04.000000 dramkit-0.5.39/dramkit/_tmp/test_pywechat.py
--rw-rw-rw-   0        0        0     3046 2022-09-12 10:04:35.000000 dramkit-0.5.39/dramkit/_tmp/test_tree.py
--rw-rw-rw-   0        0        0     1154 2023-03-08 08:28:22.000000 dramkit-0.5.39/dramkit/_tmp/test_tree2.py
--rw-rw-rw-   0        0        0     1590 2022-09-06 13:36:18.000000 dramkit-0.5.39/dramkit/_tmp/test_wechat_work.py
--rw-rw-rw-   0        0        0     4876 2021-12-24 09:25:22.000000 dramkit-0.5.39/dramkit/_tmp/tfDNNCls_test.py
--rw-rw-rw-   0        0        0     2832 2021-12-24 09:25:22.000000 dramkit-0.5.39/dramkit/_tmp/tmp.py
--rw-rw-rw-   0        0        0     1323 2023-03-28 09:21:10.000000 dramkit-0.5.39/dramkit/_tmp/tmp_args.py
--rw-rw-rw-   0        0        0     5409 2021-12-24 09:25:22.000000 dramkit-0.5.39/dramkit/_tmp/transformer_pytorch.py
--rw-rw-rw-   0        0        0     4675 2022-07-06 06:13:38.000000 dramkit-0.5.39/dramkit/_tmp/utils_SignalDec.py
--rw-rw-rw-   0        0        0    10430 2022-05-06 10:45:29.000000 dramkit-0.5.39/dramkit/_tmp/utils_TimeSeries.py
--rw-rw-rw-   0        0        0     3190 2022-05-06 10:38:49.000000 dramkit-0.5.39/dramkit/_tmp/utils_lottery.py
--rw-rw-rw-   0        0        0     3295 2021-12-24 09:25:22.000000 dramkit-0.5.39/dramkit/_tmp/utils_rl.py
--rw-rw-rw-   0        0        0     2178 2021-12-24 09:25:22.000000 dramkit-0.5.39/dramkit/_tmp/utils_rl2.py
--rw-rw-rw-   0        0        0     4310 2021-12-24 09:25:22.000000 dramkit-0.5.39/dramkit/_tmp/utils_rl3.py
--rw-rw-rw-   0        0        0     4703 2021-12-24 09:25:22.000000 dramkit-0.5.39/dramkit/_tmp/utils_rl4.py
--rw-rw-rw-   0        0        0    10517 2021-12-24 09:25:22.000000 dramkit-0.5.39/dramkit/_tmp/utils_rl5.py
--rw-rw-rw-   0        0        0    10095 2021-12-24 09:25:22.000000 dramkit-0.5.39/dramkit/_tmp/utils_rl6.py
--rw-rw-rw-   0        0        0     5426 2021-12-24 09:25:22.000000 dramkit-0.5.39/dramkit/_tmp/utils_rl7.py
--rw-rw-rw-   0        0        0     2959 2021-12-24 09:25:22.000000 dramkit-0.5.39/dramkit/_tmp/utils_sem.py
-drwxrwxrwx   0        0        0        0 2023-05-05 14:54:02.515796 dramkit-0.5.39/dramkit/backpacks/
--rw-rw-rw-   0        0        0       25 2021-12-24 09:25:22.000000 dramkit-0.5.39/dramkit/backpacks/__init__.py
--rw-rw-rw-   0        0        0     7101 2022-05-01 13:07:37.000000 dramkit-0.5.39/dramkit/backpacks/backpack01_float_dy.py
--rw-rw-rw-   0        0        0     6771 2022-05-01 13:50:22.000000 dramkit-0.5.39/dramkit/backpacks/backpack01_int_dy.py
-drwxrwxrwx   0        0        0        0 2023-05-05 14:54:02.535746 dramkit-0.5.39/dramkit/chncal/
--rw-rw-rw-   0        0        0      730 2023-05-04 13:48:09.000000 dramkit-0.5.39/dramkit/chncal/__init__.py
--rw-rw-rw-   0        0        0    21004 2023-05-04 13:48:09.000000 dramkit-0.5.39/dramkit/chncal/apis.py
--rw-rw-rw-   0        0        0    69806 2023-05-04 13:48:09.000000 dramkit-0.5.39/dramkit/chncal/constants.py
--rw-rw-rw-   0        0        0     8480 2023-05-04 13:48:09.000000 dramkit-0.5.39/dramkit/chncal/constants_fate.py
--rw-rw-rw-   0        0        0  9509384 2023-05-04 13:48:09.000000 dramkit-0.5.39/dramkit/chncal/constants_hko.py
--rw-rw-rw-   0        0        0  3955489 2023-05-04 13:48:09.000000 dramkit-0.5.39/dramkit/chncal/constants_trade_dates.py
--rw-rw-rw-   0        0        0     2501 2023-05-04 13:48:09.000000 dramkit-0.5.39/dramkit/chncal/constants_wuxing.py
--rw-rw-rw-   0        0        0     8342 2023-05-04 13:48:09.000000 dramkit-0.5.39/dramkit/chncal/constants_zodiac_marry.py
--rw-rw-rw-   0        0        0     4570 2023-05-04 13:48:09.000000 dramkit-0.5.39/dramkit/chncal/solar_terms.py
--rw-rw-rw-   0        0        0     6723 2023-04-24 06:40:29.000000 dramkit-0.5.39/dramkit/cryptotools.py
--rw-rw-rw-   0        0        0    33510 2023-04-19 02:53:20.000000 dramkit-0.5.39/dramkit/datetimetools.py
-drwxrwxrwx   0        0        0        0 2023-05-05 14:54:02.550727 dramkit-0.5.39/dramkit/datsci/
--rw-rw-rw-   0        0        0       65 2022-05-06 02:08:55.000000 dramkit-0.5.39/dramkit/datsci/__init__.py
--rw-rw-rw-   0        0        0     2865 2023-03-22 07:56:05.000000 dramkit-0.5.39/dramkit/datsci/_utils_ann.py
--rw-rw-rw-   0        0        0     2090 2022-05-05 14:04:35.000000 dramkit-0.5.39/dramkit/datsci/activate_funcs.py
--rw-rw-rw-   0        0        0    19078 2023-03-22 07:56:56.000000 dramkit-0.5.39/dramkit/datsci/ahp.py
--rw-rw-rw-   0        0        0     2992 2023-03-22 07:58:04.000000 dramkit-0.5.39/dramkit/datsci/ahp_sim_ri.py
--rw-rw-rw-   0        0        0    10071 2022-05-19 06:37:13.000000 dramkit-0.5.39/dramkit/datsci/apriori.py
--rw-rw-rw-   0        0        0     4362 2022-05-06 06:17:24.000000 dramkit-0.5.39/dramkit/datsci/curvature.py
--rw-rw-rw-   0        0        0     6966 2023-03-22 07:59:58.000000 dramkit-0.5.39/dramkit/datsci/elm_cls.py
--rw-rw-rw-   0        0        0     8216 2023-03-22 08:00:46.000000 dramkit-0.5.39/dramkit/datsci/elm_reg.py
--rw-rw-rw-   0        0        0     3697 2022-06-25 18:21:15.000000 dramkit-0.5.39/dramkit/datsci/entropy_weight.py
--rw-rw-rw-   0        0        0    50059 2023-03-22 08:02:24.000000 dramkit-0.5.39/dramkit/datsci/find_maxmin.py
--rw-rw-rw-   0        0        0     7229 2023-03-22 08:06:26.000000 dramkit-0.5.39/dramkit/datsci/freq_item_set.py
--rw-rw-rw-   0        0        0     6219 2023-03-22 07:59:12.000000 dramkit-0.5.39/dramkit/datsci/lr.py
--rw-rw-rw-   0        0        0    19374 2023-04-25 08:42:22.000000 dramkit-0.5.39/dramkit/datsci/preprocess.py
--rw-rw-rw-   0        0        0    41389 2023-03-23 13:45:46.000000 dramkit-0.5.39/dramkit/datsci/stats.py
--rw-rw-rw-   0        0        0    36092 2023-03-22 08:04:05.000000 dramkit-0.5.39/dramkit/datsci/time_series.py
--rw-rw-rw-   0        0        0     3451 2022-06-25 18:24:48.000000 dramkit-0.5.39/dramkit/datsci/topsis.py
--rw-rw-rw-   0        0        0    23324 2022-10-17 06:00:47.000000 dramkit-0.5.39/dramkit/datsci/utils_lgb.py
--rw-rw-rw-   0        0        0     6843 2022-09-09 05:44:56.000000 dramkit-0.5.39/dramkit/datsci/utils_ml.py
-drwxrwxrwx   0        0        0        0 2023-05-05 14:54:02.556711 dramkit-0.5.39/dramkit/find_addends/
--rw-rw-rw-   0        0        0       25 2021-12-24 09:25:22.000000 dramkit-0.5.39/dramkit/find_addends/__init__.py
--rw-rw-rw-   0        0        0     3433 2023-03-22 08:18:35.000000 dramkit-0.5.39/dramkit/find_addends/find_addends_backpack01float.py
--rw-rw-rw-   0        0        0     2149 2022-05-01 08:15:22.000000 dramkit-0.5.39/dramkit/find_addends/find_addends_backpack01int.py
--rw-rw-rw-   0        0        0    12658 2023-03-22 08:17:39.000000 dramkit-0.5.39/dramkit/find_addends/find_addends_bigfirst.py
--rw-rw-rw-   0        0        0     4500 2023-03-22 08:17:06.000000 dramkit-0.5.39/dramkit/find_addends/find_addends_recu.py
--rw-rw-rw-   0        0        0     9576 2023-03-22 08:16:00.000000 dramkit-0.5.39/dramkit/find_addends/find_addends_smlfirst.py
--rw-rw-rw-   0        0        0     3988 2022-04-30 16:29:18.000000 dramkit-0.5.39/dramkit/find_addends/find_addends_utils.py
--rw-rw-rw-   0        0        0   115682 2023-04-30 09:54:45.000000 dramkit-0.5.39/dramkit/gentools.py
--rw-rw-rw-   0        0        0      735 2022-08-04 06:40:11.000000 dramkit-0.5.39/dramkit/install_check.py
--rw-rw-rw-   0        0        0    67031 2023-04-29 02:36:33.000000 dramkit-0.5.39/dramkit/iotools.py
-drwxrwxrwx   0        0        0        0 2023-05-05 14:54:02.559703 dramkit-0.5.39/dramkit/logtools/
--rw-rw-rw-   0        0        0      139 2023-05-01 07:34:20.000000 dramkit-0.5.39/dramkit/logtools/__init__.py
--rw-rw-rw-   0        0        0     2566 2023-02-08 04:11:46.000000 dramkit-0.5.39/dramkit/logtools/logger_general.py
--rw-rw-rw-   0        0        0     3597 2023-02-07 03:04:57.000000 dramkit-0.5.39/dramkit/logtools/logger_rotating.py
--rw-rw-rw-   0        0        0     2880 2023-02-07 03:04:39.000000 dramkit-0.5.39/dramkit/logtools/logger_timedrotating.py
--rw-rw-rw-   0        0        0     4214 2023-02-28 10:31:30.000000 dramkit-0.5.39/dramkit/logtools/utils_logger.py
-drwxrwxrwx   0        0        0        0 2023-05-05 14:54:02.561698 dramkit-0.5.39/dramkit/openai/
--rw-rw-rw-   0        0        0      203 2023-04-24 02:54:37.000000 dramkit-0.5.39/dramkit/openai/__init__.py
--rw-rw-rw-   0        0        0     5656 2023-04-25 16:34:10.000000 dramkit-0.5.39/dramkit/openai/aiedu_chat.py
--rw-rw-rw-   0        0        0    16820 2023-04-26 14:09:48.000000 dramkit-0.5.39/dramkit/openai/openai_chat.py
--rw-rw-rw-   0        0        0     4461 2023-04-25 02:00:24.000000 dramkit-0.5.39/dramkit/openai/openai_chat_hs.py
-drwxrwxrwx   0        0        0        0 2023-05-05 14:54:02.570674 dramkit-0.5.39/dramkit/optimizer/
--rw-rw-rw-   0        0        0       25 2021-12-24 09:25:22.000000 dramkit-0.5.39/dramkit/optimizer/__init__.py
--rw-rw-rw-   0        0        0     9712 2023-03-22 08:26:32.000000 dramkit-0.5.39/dramkit/optimizer/alo.py
--rw-rw-rw-   0        0        0     3141 2022-05-02 02:31:44.000000 dramkit-0.5.39/dramkit/optimizer/base_funcs.py
--rw-rw-rw-   0        0        0     7428 2023-03-22 08:35:00.000000 dramkit-0.5.39/dramkit/optimizer/boa.py
--rw-rw-rw-   0        0        0     8863 2023-03-22 08:34:30.000000 dramkit-0.5.39/dramkit/optimizer/cs.py
--rw-rw-rw-   0        0        0    13415 2023-03-22 08:33:50.000000 dramkit-0.5.39/dramkit/optimizer/ga.py
--rw-rw-rw-   0        0        0     8701 2023-03-22 08:33:17.000000 dramkit-0.5.39/dramkit/optimizer/gwo.py
--rw-rw-rw-   0        0        0     9311 2023-03-22 08:32:10.000000 dramkit-0.5.39/dramkit/optimizer/hcpsoboa.py
--rw-rw-rw-   0        0        0     9929 2023-03-22 08:31:27.000000 dramkit-0.5.39/dramkit/optimizer/hho.py
--rw-rw-rw-   0        0        0     8817 2023-03-22 08:30:38.000000 dramkit-0.5.39/dramkit/optimizer/hpsoboa.py
--rw-rw-rw-   0        0        0     8889 2023-03-22 08:29:43.000000 dramkit-0.5.39/dramkit/optimizer/pso.py
--rw-rw-rw-   0        0        0     5222 2022-05-02 02:18:28.000000 dramkit-0.5.39/dramkit/optimizer/utils_heuristic.py
--rw-rw-rw-   0        0        0     7334 2023-03-22 08:27:35.000000 dramkit-0.5.39/dramkit/optimizer/woa.py
-drwxrwxrwx   0        0        0        0 2023-05-05 14:54:02.575660 dramkit-0.5.39/dramkit/other/
--rw-rw-rw-   0        0        0     3856 2023-04-30 10:22:45.000000 dramkit-0.5.39/dramkit/other/_Linux_notes.py
--rw-rw-rw-   0        0        0     2871 2023-04-19 03:27:58.000000 dramkit-0.5.39/dramkit/other/_Python_notes.py
--rw-rw-rw-   0        0        0     4777 2023-04-24 08:14:04.000000 dramkit-0.5.39/dramkit/other/_Vim_notes.py
--rw-rw-rw-   0        0        0      164 2022-08-25 01:46:27.000000 dramkit-0.5.39/dramkit/other/__init__.py
--rw-rw-rw-   0        0        0     7988 2022-10-27 06:38:44.000000 dramkit-0.5.39/dramkit/other/langconv.py
--rw-rw-rw-   0        0        0     8353 2022-12-10 15:26:10.000000 dramkit-0.5.39/dramkit/other/othertools.py
--rw-rw-rw-   0        0        0     1804 2023-03-22 08:36:51.000000 dramkit-0.5.39/dramkit/other/replace_endblank.py
--rw-rw-rw-   0        0        0   143066 2022-08-25 01:37:20.000000 dramkit-0.5.39/dramkit/other/zh_wiki.py
-drwxrwxrwx   0        0        0        0 2023-05-05 14:54:02.578652 dramkit-0.5.39/dramkit/plottools/
--rw-rw-rw-   0        0        0      112 2022-05-04 14:50:04.000000 dramkit-0.5.39/dramkit/plottools/__init__.py
--rw-rw-rw-   0        0        0     4400 2022-01-09 07:36:22.000000 dramkit-0.5.39/dramkit/plottools/plot_barline.py
--rw-rw-rw-   0        0        0    48559 2023-04-22 13:09:27.000000 dramkit-0.5.39/dramkit/plottools/plot_common.py
--rw-rw-rw-   0        0        0     9033 2022-06-25 18:36:48.000000 dramkit-0.5.39/dramkit/plottools/plot_histdist.py
--rw-rw-rw-   0        0        0     2145 2023-03-04 13:10:35.000000 dramkit-0.5.39/dramkit/plottools/plot_scatter.py
--rw-rw-rw-   0        0        0     5120 2023-03-21 14:27:12.000000 dramkit-0.5.39/dramkit/plottools/utils_plot.py
-drwxrwxrwx   0        0        0        0 2023-05-05 14:54:02.580651 dramkit-0.5.39/dramkit/pystyles/
--rw-rw-rw-   0        0        0       25 2021-12-25 16:04:07.000000 dramkit-0.5.39/dramkit/pystyles/__init__.py
--rw-rw-rw-   0        0        0     8021 2022-04-30 13:24:37.000000 dramkit-0.5.39/dramkit/pystyles/dramkit_style.py
-drwxrwxrwx   0        0        0        0 2023-05-05 14:54:02.584641 dramkit-0.5.39/dramkit/sorts/
--rw-rw-rw-   0        0        0       25 2021-12-24 09:25:22.000000 dramkit-0.5.39/dramkit/sorts/__init__.py
--rw-rw-rw-   0        0        0     1302 2022-01-09 08:45:28.000000 dramkit-0.5.39/dramkit/sorts/bubble_sort.py
--rw-rw-rw-   0        0        0     1426 2022-01-09 08:51:55.000000 dramkit-0.5.39/dramkit/sorts/bucket_sort.py
--rw-rw-rw-   0        0        0     4742 2022-01-09 08:10:56.000000 dramkit-0.5.39/dramkit/sorts/insert_sort.py
--rw-rw-rw-   0        0        0     4833 2022-01-09 09:23:30.000000 dramkit-0.5.39/dramkit/sorts/insert_sort_bin.py
--rw-rw-rw-   0        0        0     1339 2022-01-09 08:55:14.000000 dramkit-0.5.39/dramkit/sorts/quick_sort.py
-drwxrwxrwx   0        0        0        0 2023-05-05 14:54:02.589623 dramkit-0.5.39/dramkit/speedup/
--rw-rw-rw-   0        0        0       25 2021-12-24 09:25:22.000000 dramkit-0.5.39/dramkit/speedup/__init__.py
--rw-rw-rw-   0        0        0     1231 2023-04-14 13:02:46.000000 dramkit-0.5.39/dramkit/speedup/_mp_test1.py
--rw-rw-rw-   0        0        0      886 2023-04-14 13:17:44.000000 dramkit-0.5.39/dramkit/speedup/_mp_test2.py
--rw-rw-rw-   0        0        0      684 2023-04-14 13:14:44.000000 dramkit-0.5.39/dramkit/speedup/_mp_test3.py
--rw-rw-rw-   0        0        0     3384 2023-04-14 13:25:51.000000 dramkit-0.5.39/dramkit/speedup/iotools_tmp.py
--rw-rw-rw-   0        0        0     3754 2023-04-12 08:17:22.000000 dramkit-0.5.39/dramkit/speedup/multi_process_concurrent.py
--rw-rw-rw-   0        0        0     7888 2023-04-07 08:59:34.000000 dramkit-0.5.39/dramkit/speedup/multi_thread.py
-drwxrwxrwx   0        0        0        0 2023-05-05 14:54:02.594610 dramkit-0.5.39/dramkit/sqltools/
--rw-rw-rw-   0        0        0     2495 2023-02-23 05:15:08.000000 dramkit-0.5.39/dramkit/sqltools/_Hive_notes.py
--rw-rw-rw-   0        0        0    30416 2023-04-11 01:33:28.000000 dramkit-0.5.39/dramkit/sqltools/_MySQL_notes.py
--rw-rw-rw-   0        0        0     6849 2023-03-07 09:26:53.000000 dramkit-0.5.39/dramkit/sqltools/_Oracle_notes.py
--rw-rw-rw-   0        0        0      160 2023-05-01 12:57:19.000000 dramkit-0.5.39/dramkit/sqltools/__init__.py
--rw-rw-rw-   0        0        0    19770 2023-02-15 09:03:04.000000 dramkit-0.5.39/dramkit/sqltools/cxoracle.py
--rw-rw-rw-   0        0        0    25908 2023-02-24 11:31:13.000000 dramkit-0.5.39/dramkit/sqltools/py_hive.py
--rw-rw-rw-   0        0        0    50395 2023-02-24 11:32:46.000000 dramkit-0.5.39/dramkit/sqltools/py_mysql.py
--rw-rw-rw-   0        0        0    18391 2023-03-22 02:56:24.000000 dramkit-0.5.39/dramkit/sqltools/sql_alchemy.py
-drwxrwxrwx   0        0        0        0 2023-05-05 14:54:02.595610 dramkit-0.5.39/dramkit/webtools/
--rw-rw-rw-   0        0        0       25 2021-12-24 09:25:22.000000 dramkit-0.5.39/dramkit/webtools/__init__.py
--rw-rw-rw-   0        0        0     5337 2022-06-25 18:37:55.000000 dramkit-0.5.39/dramkit/webtools/utils_html.py
-drwxrwxrwx   0        0        0        0 2023-05-05 14:54:02.596604 dramkit-0.5.39/dramkit/wechat/
--rw-rw-rw-   0        0        0       58 2022-09-06 14:04:57.000000 dramkit-0.5.39/dramkit/wechat/__init__.py
--rw-rw-rw-   0        0        0     7473 2022-10-28 03:03:37.000000 dramkit-0.5.39/dramkit/wechat/qywechat.py
-drwxrwxrwx   0        0        0        0 2023-05-05 14:54:02.481886 dramkit-0.5.39/dramkit.egg-info/
--rw-rw-rw-   0        0        0     1095 2023-05-05 14:54:02.000000 dramkit-0.5.39/dramkit.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     4852 2023-05-05 14:54:02.000000 dramkit-0.5.39/dramkit.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-05 14:54:02.000000 dramkit-0.5.39/dramkit.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       66 2023-05-05 14:54:02.000000 dramkit-0.5.39/dramkit.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2023-05-05 14:54:02.000000 dramkit-0.5.39/dramkit.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-05 14:54:02.599596 dramkit-0.5.39/setup.cfg
--rw-rw-rw-   0        0        0     1944 2023-05-01 12:58:33.000000 dramkit-0.5.39/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-15 06:26:58.323759 dramkit-0.5.40/
+-rw-rw-rw-   0        0        0     1072 2023-02-25 10:45:19.000000 dramkit-0.5.40/LICENSE
+-rw-rw-rw-   0        0        0     1095 2023-05-15 06:26:58.322778 dramkit-0.5.40/PKG-INFO
+-rw-rw-rw-   0        0        0      795 2022-05-06 14:18:52.000000 dramkit-0.5.40/README.md
+drwxrwxrwx   0        0        0        0 2023-05-15 06:26:57.885763 dramkit-0.5.40/dramkit/
+-rw-rw-rw-   0        0        0      999 2023-04-24 03:43:26.000000 dramkit-0.5.40/dramkit/__init__.py
+-rw-rw-rw-   0        0        0      662 2023-05-15 06:26:21.000000 dramkit-0.5.40/dramkit/_pkg_info.py
+drwxrwxrwx   0        0        0        0 2023-05-15 06:26:58.021761 dramkit-0.5.40/dramkit/_tmp/
+-rw-rw-rw-   0        0        0     6600 2021-12-24 09:25:22.000000 dramkit-0.5.40/dramkit/_tmp/CRR.py
+-rw-rw-rw-   0        0        0     1844 2022-08-02 09:50:33.000000 dramkit-0.5.40/dramkit/_tmp/CtrlPreTS.py
+-rw-rw-rw-   0        0        0      515 2022-01-09 09:11:34.000000 dramkit-0.5.40/dramkit/_tmp/NPairSum.py
+-rw-rw-rw-   0        0        0     3672 2021-12-24 09:25:22.000000 dramkit-0.5.40/dramkit/_tmp/PIDtest.py
+-rw-rw-rw-   0        0        0     2316 2021-12-24 09:25:22.000000 dramkit-0.5.40/dramkit/_tmp/PIDtest2.py
+-rw-rw-rw-   0        0        0     6152 2021-12-24 09:25:22.000000 dramkit-0.5.40/dramkit/_tmp/VMD.py
+-rw-rw-rw-   0        0        0       25 2021-12-24 09:25:22.000000 dramkit-0.5.40/dramkit/_tmp/__init__.py
+-rw-rw-rw-   0        0        0     2182 2021-12-24 09:25:22.000000 dramkit-0.5.40/dramkit/_tmp/cca_test.py
+-rw-rw-rw-   0        0        0     1768 2021-12-24 09:25:22.000000 dramkit-0.5.40/dramkit/_tmp/dtw_test.py
+-rw-rw-rw-   0        0        0    10656 2021-12-24 09:25:22.000000 dramkit-0.5.40/dramkit/_tmp/explore.py
+-rw-rw-rw-   0        0        0     2857 2021-12-24 09:25:22.000000 dramkit-0.5.40/dramkit/_tmp/gini.py
+-rw-rw-rw-   0        0        0      899 2021-12-24 09:25:22.000000 dramkit-0.5.40/dramkit/_tmp/merge_sort.py
+-rw-rw-rw-   0        0        0      910 2021-12-24 09:25:22.000000 dramkit-0.5.40/dramkit/_tmp/mouse_move.py
+-rw-rw-rw-   0        0        0     1600 2021-12-24 09:25:22.000000 dramkit-0.5.40/dramkit/_tmp/mpc_test1.py
+-rw-rw-rw-   0        0        0     7521 2021-12-24 09:25:22.000000 dramkit-0.5.40/dramkit/_tmp/options_Implied_volatility.py
+-rw-rw-rw-   0        0        0      501 2021-12-24 09:25:22.000000 dramkit-0.5.40/dramkit/_tmp/pf_test.py
+-rw-rw-rw-   0        0        0     4142 2021-12-24 09:25:22.000000 dramkit-0.5.40/dramkit/_tmp/plot_test.py
+-rw-rw-rw-   0        0        0     1567 2022-05-06 11:02:39.000000 dramkit-0.5.40/dramkit/_tmp/plot_test2.py
+-rw-rw-rw-   0        0        0     2618 2022-07-06 06:24:15.000000 dramkit-0.5.40/dramkit/_tmp/simple_smooth.py
+-rw-rw-rw-   0        0        0     1057 2023-03-17 03:20:46.000000 dramkit-0.5.40/dramkit/_tmp/test_async_washs.py
+-rw-rw-rw-   0        0        0     1720 2023-04-03 01:16:22.000000 dramkit-0.5.40/dramkit/_tmp/test_await_timeout.py
+-rw-rw-rw-   0        0        0      747 2021-12-24 09:25:22.000000 dramkit-0.5.40/dramkit/_tmp/test_backtrader.py
+-rw-rw-rw-   0        0        0     1917 2023-02-16 09:04:46.000000 dramkit-0.5.40/dramkit/_tmp/test_chatgpt_v1.py
+-rw-rw-rw-   0        0        0      657 2021-12-24 09:25:22.000000 dramkit-0.5.40/dramkit/_tmp/test_code.py
+-rw-rw-rw-   0        0        0     3629 2022-04-13 14:32:40.000000 dramkit-0.5.40/dramkit/_tmp/test_find_peaks.py
+-rw-rw-rw-   0        0        0      585 2023-01-29 09:46:43.000000 dramkit-0.5.40/dramkit/_tmp/test_get_var_name.py
+-rw-rw-rw-   0        0        0     1263 2022-06-22 06:15:28.000000 dramkit-0.5.40/dramkit/_tmp/test_grading.py
+-rw-rw-rw-   0        0        0     2193 2021-12-24 09:25:22.000000 dramkit-0.5.40/dramkit/_tmp/test_lr.py
+-rw-rw-rw-   0        0        0     1154 2023-01-13 09:20:58.000000 dramkit-0.5.40/dramkit/_tmp/test_maxsort.py
+-rw-rw-rw-   0        0        0      466 2023-04-06 07:48:43.000000 dramkit-0.5.40/dramkit/_tmp/test_multiprocessing.py
+-rw-rw-rw-   0        0        0      318 2022-01-26 13:43:15.000000 dramkit-0.5.40/dramkit/_tmp/test_ocr.py
+-rw-rw-rw-   0        0        0     1791 2022-04-22 14:45:04.000000 dramkit-0.5.40/dramkit/_tmp/test_pywechat.py
+-rw-rw-rw-   0        0        0     3046 2022-09-12 10:04:35.000000 dramkit-0.5.40/dramkit/_tmp/test_tree.py
+-rw-rw-rw-   0        0        0     1154 2023-03-08 08:28:22.000000 dramkit-0.5.40/dramkit/_tmp/test_tree2.py
+-rw-rw-rw-   0        0        0     1590 2022-09-06 13:36:18.000000 dramkit-0.5.40/dramkit/_tmp/test_wechat_work.py
+-rw-rw-rw-   0        0        0     4876 2021-12-24 09:25:22.000000 dramkit-0.5.40/dramkit/_tmp/tfDNNCls_test.py
+-rw-rw-rw-   0        0        0     2832 2021-12-24 09:25:22.000000 dramkit-0.5.40/dramkit/_tmp/tmp.py
+-rw-rw-rw-   0        0        0     1323 2023-03-28 09:21:10.000000 dramkit-0.5.40/dramkit/_tmp/tmp_args.py
+-rw-rw-rw-   0        0        0     5409 2021-12-24 09:25:22.000000 dramkit-0.5.40/dramkit/_tmp/transformer_pytorch.py
+-rw-rw-rw-   0        0        0     4675 2022-07-06 06:13:38.000000 dramkit-0.5.40/dramkit/_tmp/utils_SignalDec.py
+-rw-rw-rw-   0        0        0    10430 2022-05-06 10:45:29.000000 dramkit-0.5.40/dramkit/_tmp/utils_TimeSeries.py
+-rw-rw-rw-   0        0        0     3190 2022-05-06 10:38:49.000000 dramkit-0.5.40/dramkit/_tmp/utils_lottery.py
+-rw-rw-rw-   0        0        0     3295 2021-12-24 09:25:22.000000 dramkit-0.5.40/dramkit/_tmp/utils_rl.py
+-rw-rw-rw-   0        0        0     2178 2021-12-24 09:25:22.000000 dramkit-0.5.40/dramkit/_tmp/utils_rl2.py
+-rw-rw-rw-   0        0        0     4310 2021-12-24 09:25:22.000000 dramkit-0.5.40/dramkit/_tmp/utils_rl3.py
+-rw-rw-rw-   0        0        0     4703 2021-12-24 09:25:22.000000 dramkit-0.5.40/dramkit/_tmp/utils_rl4.py
+-rw-rw-rw-   0        0        0    10517 2021-12-24 09:25:22.000000 dramkit-0.5.40/dramkit/_tmp/utils_rl5.py
+-rw-rw-rw-   0        0        0    10095 2021-12-24 09:25:22.000000 dramkit-0.5.40/dramkit/_tmp/utils_rl6.py
+-rw-rw-rw-   0        0        0     5426 2021-12-24 09:25:22.000000 dramkit-0.5.40/dramkit/_tmp/utils_rl7.py
+-rw-rw-rw-   0        0        0     2959 2021-12-24 09:25:22.000000 dramkit-0.5.40/dramkit/_tmp/utils_sem.py
+drwxrwxrwx   0        0        0        0 2023-05-15 06:26:58.029777 dramkit-0.5.40/dramkit/backpacks/
+-rw-rw-rw-   0        0        0       25 2021-12-24 09:25:22.000000 dramkit-0.5.40/dramkit/backpacks/__init__.py
+-rw-rw-rw-   0        0        0     7101 2022-05-01 13:07:37.000000 dramkit-0.5.40/dramkit/backpacks/backpack01_float_dy.py
+-rw-rw-rw-   0        0        0     6771 2022-05-01 13:50:22.000000 dramkit-0.5.40/dramkit/backpacks/backpack01_int_dy.py
+drwxrwxrwx   0        0        0        0 2023-05-15 06:26:58.071775 dramkit-0.5.40/dramkit/chncal/
+-rw-rw-rw-   0        0        0      730 2023-05-12 02:03:24.000000 dramkit-0.5.40/dramkit/chncal/__init__.py
+-rw-rw-rw-   0        0        0    21004 2023-05-12 02:03:24.000000 dramkit-0.5.40/dramkit/chncal/apis.py
+-rw-rw-rw-   0        0        0    69806 2023-05-12 02:03:24.000000 dramkit-0.5.40/dramkit/chncal/constants.py
+-rw-rw-rw-   0        0        0     8480 2023-05-12 02:03:24.000000 dramkit-0.5.40/dramkit/chncal/constants_fate.py
+-rw-rw-rw-   0        0        0  9509384 2023-05-12 02:03:24.000000 dramkit-0.5.40/dramkit/chncal/constants_hko.py
+-rw-rw-rw-   0        0        0  3958798 2023-05-12 02:03:24.000000 dramkit-0.5.40/dramkit/chncal/constants_trade_dates.py
+-rw-rw-rw-   0        0        0     2501 2023-05-12 02:03:24.000000 dramkit-0.5.40/dramkit/chncal/constants_wuxing.py
+-rw-rw-rw-   0        0        0     8342 2023-05-12 02:03:24.000000 dramkit-0.5.40/dramkit/chncal/constants_zodiac_marry.py
+-rw-rw-rw-   0        0        0     4570 2023-05-12 02:03:24.000000 dramkit-0.5.40/dramkit/chncal/solar_terms.py
+-rw-rw-rw-   0        0        0     6723 2023-04-24 06:40:29.000000 dramkit-0.5.40/dramkit/cryptotools.py
+-rw-rw-rw-   0        0        0    34313 2023-05-11 01:22:24.000000 dramkit-0.5.40/dramkit/datetimetools.py
+drwxrwxrwx   0        0        0        0 2023-05-15 06:26:58.123780 dramkit-0.5.40/dramkit/datsci/
+-rw-rw-rw-   0        0        0       65 2022-05-06 02:08:55.000000 dramkit-0.5.40/dramkit/datsci/__init__.py
+-rw-rw-rw-   0        0        0     2865 2023-03-22 07:56:05.000000 dramkit-0.5.40/dramkit/datsci/_utils_ann.py
+-rw-rw-rw-   0        0        0     2090 2022-05-05 14:04:35.000000 dramkit-0.5.40/dramkit/datsci/activate_funcs.py
+-rw-rw-rw-   0        0        0    19078 2023-03-22 07:56:56.000000 dramkit-0.5.40/dramkit/datsci/ahp.py
+-rw-rw-rw-   0        0        0     2992 2023-03-22 07:58:04.000000 dramkit-0.5.40/dramkit/datsci/ahp_sim_ri.py
+-rw-rw-rw-   0        0        0    10071 2022-05-19 06:37:13.000000 dramkit-0.5.40/dramkit/datsci/apriori.py
+-rw-rw-rw-   0        0        0     4362 2022-05-06 06:17:24.000000 dramkit-0.5.40/dramkit/datsci/curvature.py
+-rw-rw-rw-   0        0        0     6966 2023-03-22 07:59:58.000000 dramkit-0.5.40/dramkit/datsci/elm_cls.py
+-rw-rw-rw-   0        0        0     8216 2023-03-22 08:00:46.000000 dramkit-0.5.40/dramkit/datsci/elm_reg.py
+-rw-rw-rw-   0        0        0     3697 2022-06-25 18:21:15.000000 dramkit-0.5.40/dramkit/datsci/entropy_weight.py
+-rw-rw-rw-   0        0        0    50084 2023-05-10 02:47:36.000000 dramkit-0.5.40/dramkit/datsci/find_maxmin.py
+-rw-rw-rw-   0        0        0     7229 2023-03-22 08:06:26.000000 dramkit-0.5.40/dramkit/datsci/freq_item_set.py
+-rw-rw-rw-   0        0        0     6219 2023-03-22 07:59:12.000000 dramkit-0.5.40/dramkit/datsci/lr.py
+-rw-rw-rw-   0        0        0    19374 2023-04-25 08:42:22.000000 dramkit-0.5.40/dramkit/datsci/preprocess.py
+-rw-rw-rw-   0        0        0    41389 2023-03-23 13:45:46.000000 dramkit-0.5.40/dramkit/datsci/stats.py
+-rw-rw-rw-   0        0        0    36092 2023-03-22 08:04:05.000000 dramkit-0.5.40/dramkit/datsci/time_series.py
+-rw-rw-rw-   0        0        0     3451 2022-06-25 18:24:48.000000 dramkit-0.5.40/dramkit/datsci/topsis.py
+-rw-rw-rw-   0        0        0    23324 2022-10-17 06:00:47.000000 dramkit-0.5.40/dramkit/datsci/utils_lgb.py
+-rw-rw-rw-   0        0        0     6843 2022-09-09 05:44:56.000000 dramkit-0.5.40/dramkit/datsci/utils_ml.py
+-rw-rw-rw-   0        0        0    21037 2023-05-11 01:05:22.000000 dramkit-0.5.40/dramkit/datsci/zigzag.py
+drwxrwxrwx   0        0        0        0 2023-05-15 06:26:58.141776 dramkit-0.5.40/dramkit/find_addends/
+-rw-rw-rw-   0        0        0       25 2021-12-24 09:25:22.000000 dramkit-0.5.40/dramkit/find_addends/__init__.py
+-rw-rw-rw-   0        0        0     3433 2023-03-22 08:18:35.000000 dramkit-0.5.40/dramkit/find_addends/find_addends_backpack01float.py
+-rw-rw-rw-   0        0        0     2149 2022-05-01 08:15:22.000000 dramkit-0.5.40/dramkit/find_addends/find_addends_backpack01int.py
+-rw-rw-rw-   0        0        0    12658 2023-03-22 08:17:39.000000 dramkit-0.5.40/dramkit/find_addends/find_addends_bigfirst.py
+-rw-rw-rw-   0        0        0     4500 2023-03-22 08:17:06.000000 dramkit-0.5.40/dramkit/find_addends/find_addends_recu.py
+-rw-rw-rw-   0        0        0     9576 2023-03-22 08:16:00.000000 dramkit-0.5.40/dramkit/find_addends/find_addends_smlfirst.py
+-rw-rw-rw-   0        0        0     3988 2022-04-30 16:29:18.000000 dramkit-0.5.40/dramkit/find_addends/find_addends_utils.py
+-rw-rw-rw-   0        0        0   119309 2023-05-10 06:51:27.000000 dramkit-0.5.40/dramkit/gentools.py
+-rw-rw-rw-   0        0        0      735 2022-08-04 06:40:11.000000 dramkit-0.5.40/dramkit/install_check.py
+-rw-rw-rw-   0        0        0    67227 2023-05-12 02:56:43.000000 dramkit-0.5.40/dramkit/iotools.py
+drwxrwxrwx   0        0        0        0 2023-05-15 06:26:58.155760 dramkit-0.5.40/dramkit/logtools/
+-rw-rw-rw-   0        0        0      139 2023-05-01 07:34:20.000000 dramkit-0.5.40/dramkit/logtools/__init__.py
+-rw-rw-rw-   0        0        0     2566 2023-02-08 04:11:46.000000 dramkit-0.5.40/dramkit/logtools/logger_general.py
+-rw-rw-rw-   0        0        0     3597 2023-02-07 03:04:57.000000 dramkit-0.5.40/dramkit/logtools/logger_rotating.py
+-rw-rw-rw-   0        0        0     2880 2023-02-07 03:04:39.000000 dramkit-0.5.40/dramkit/logtools/logger_timedrotating.py
+-rw-rw-rw-   0        0        0     4214 2023-02-28 10:31:30.000000 dramkit-0.5.40/dramkit/logtools/utils_logger.py
+drwxrwxrwx   0        0        0        0 2023-05-15 06:26:58.166773 dramkit-0.5.40/dramkit/openai/
+-rw-rw-rw-   0        0        0      203 2023-04-24 02:54:37.000000 dramkit-0.5.40/dramkit/openai/__init__.py
+-rw-rw-rw-   0        0        0     5656 2023-04-25 16:34:10.000000 dramkit-0.5.40/dramkit/openai/aiedu_chat.py
+-rw-rw-rw-   0        0        0    16999 2023-05-08 02:26:05.000000 dramkit-0.5.40/dramkit/openai/openai_chat.py
+-rw-rw-rw-   0        0        0     4461 2023-04-25 02:00:24.000000 dramkit-0.5.40/dramkit/openai/openai_chat_hs.py
+drwxrwxrwx   0        0        0        0 2023-05-15 06:26:58.199760 dramkit-0.5.40/dramkit/optimizer/
+-rw-rw-rw-   0        0        0       25 2021-12-24 09:25:22.000000 dramkit-0.5.40/dramkit/optimizer/__init__.py
+-rw-rw-rw-   0        0        0     9712 2023-03-22 08:26:32.000000 dramkit-0.5.40/dramkit/optimizer/alo.py
+-rw-rw-rw-   0        0        0     3141 2022-05-02 02:31:44.000000 dramkit-0.5.40/dramkit/optimizer/base_funcs.py
+-rw-rw-rw-   0        0        0     7428 2023-03-22 08:35:00.000000 dramkit-0.5.40/dramkit/optimizer/boa.py
+-rw-rw-rw-   0        0        0     8863 2023-03-22 08:34:30.000000 dramkit-0.5.40/dramkit/optimizer/cs.py
+-rw-rw-rw-   0        0        0    13415 2023-03-22 08:33:50.000000 dramkit-0.5.40/dramkit/optimizer/ga.py
+-rw-rw-rw-   0        0        0     8701 2023-03-22 08:33:17.000000 dramkit-0.5.40/dramkit/optimizer/gwo.py
+-rw-rw-rw-   0        0        0     9311 2023-03-22 08:32:10.000000 dramkit-0.5.40/dramkit/optimizer/hcpsoboa.py
+-rw-rw-rw-   0        0        0     9929 2023-03-22 08:31:27.000000 dramkit-0.5.40/dramkit/optimizer/hho.py
+-rw-rw-rw-   0        0        0     8817 2023-03-22 08:30:38.000000 dramkit-0.5.40/dramkit/optimizer/hpsoboa.py
+-rw-rw-rw-   0        0        0     8889 2023-03-22 08:29:43.000000 dramkit-0.5.40/dramkit/optimizer/pso.py
+-rw-rw-rw-   0        0        0     5222 2022-05-02 02:18:28.000000 dramkit-0.5.40/dramkit/optimizer/utils_heuristic.py
+-rw-rw-rw-   0        0        0     7334 2023-03-22 08:27:35.000000 dramkit-0.5.40/dramkit/optimizer/woa.py
+drwxrwxrwx   0        0        0        0 2023-05-15 06:26:58.219759 dramkit-0.5.40/dramkit/other/
+-rw-rw-rw-   0        0        0     3856 2023-04-30 10:22:45.000000 dramkit-0.5.40/dramkit/other/_Linux_notes.py
+-rw-rw-rw-   0        0        0     2871 2023-04-19 03:27:58.000000 dramkit-0.5.40/dramkit/other/_Python_notes.py
+-rw-rw-rw-   0        0        0     4777 2023-04-24 08:14:04.000000 dramkit-0.5.40/dramkit/other/_Vim_notes.py
+-rw-rw-rw-   0        0        0      164 2022-08-25 01:46:27.000000 dramkit-0.5.40/dramkit/other/__init__.py
+-rw-rw-rw-   0        0        0     7988 2022-10-27 06:38:44.000000 dramkit-0.5.40/dramkit/other/langconv.py
+-rw-rw-rw-   0        0        0     8353 2022-12-10 15:26:10.000000 dramkit-0.5.40/dramkit/other/othertools.py
+-rw-rw-rw-   0        0        0     1804 2023-03-22 08:36:51.000000 dramkit-0.5.40/dramkit/other/replace_endblank.py
+-rw-rw-rw-   0        0        0   143066 2022-08-25 01:37:20.000000 dramkit-0.5.40/dramkit/other/zh_wiki.py
+drwxrwxrwx   0        0        0        0 2023-05-15 06:26:58.236759 dramkit-0.5.40/dramkit/plottools/
+-rw-rw-rw-   0        0        0      112 2022-05-04 14:50:04.000000 dramkit-0.5.40/dramkit/plottools/__init__.py
+-rw-rw-rw-   0        0        0     4400 2022-01-09 07:36:22.000000 dramkit-0.5.40/dramkit/plottools/plot_barline.py
+-rw-rw-rw-   0        0        0    48559 2023-04-22 13:09:27.000000 dramkit-0.5.40/dramkit/plottools/plot_common.py
+-rw-rw-rw-   0        0        0     9033 2022-06-25 18:36:48.000000 dramkit-0.5.40/dramkit/plottools/plot_histdist.py
+-rw-rw-rw-   0        0        0     2145 2023-03-04 13:10:35.000000 dramkit-0.5.40/dramkit/plottools/plot_scatter.py
+-rw-rw-rw-   0        0        0     5120 2023-03-21 14:27:12.000000 dramkit-0.5.40/dramkit/plottools/utils_plot.py
+drwxrwxrwx   0        0        0        0 2023-05-15 06:26:58.242760 dramkit-0.5.40/dramkit/pystyles/
+-rw-rw-rw-   0        0        0       25 2021-12-25 16:04:07.000000 dramkit-0.5.40/dramkit/pystyles/__init__.py
+-rw-rw-rw-   0        0        0     8021 2022-04-30 13:24:37.000000 dramkit-0.5.40/dramkit/pystyles/dramkit_style.py
+drwxrwxrwx   0        0        0        0 2023-05-15 06:26:58.259760 dramkit-0.5.40/dramkit/sorts/
+-rw-rw-rw-   0        0        0       25 2021-12-24 09:25:22.000000 dramkit-0.5.40/dramkit/sorts/__init__.py
+-rw-rw-rw-   0        0        0     1302 2022-01-09 08:45:28.000000 dramkit-0.5.40/dramkit/sorts/bubble_sort.py
+-rw-rw-rw-   0        0        0     1426 2022-01-09 08:51:55.000000 dramkit-0.5.40/dramkit/sorts/bucket_sort.py
+-rw-rw-rw-   0        0        0     4742 2022-01-09 08:10:56.000000 dramkit-0.5.40/dramkit/sorts/insert_sort.py
+-rw-rw-rw-   0        0        0     4833 2022-01-09 09:23:30.000000 dramkit-0.5.40/dramkit/sorts/insert_sort_bin.py
+-rw-rw-rw-   0        0        0     1339 2022-01-09 08:55:14.000000 dramkit-0.5.40/dramkit/sorts/quick_sort.py
+drwxrwxrwx   0        0        0        0 2023-05-15 06:26:58.280759 dramkit-0.5.40/dramkit/speedup/
+-rw-rw-rw-   0        0        0       25 2021-12-24 09:25:22.000000 dramkit-0.5.40/dramkit/speedup/__init__.py
+-rw-rw-rw-   0        0        0     1231 2023-04-14 13:02:46.000000 dramkit-0.5.40/dramkit/speedup/_mp_test1.py
+-rw-rw-rw-   0        0        0      886 2023-04-14 13:17:44.000000 dramkit-0.5.40/dramkit/speedup/_mp_test2.py
+-rw-rw-rw-   0        0        0      684 2023-04-14 13:14:44.000000 dramkit-0.5.40/dramkit/speedup/_mp_test3.py
+-rw-rw-rw-   0        0        0     3384 2023-04-14 13:25:51.000000 dramkit-0.5.40/dramkit/speedup/iotools_tmp.py
+-rw-rw-rw-   0        0        0     3754 2023-04-12 08:17:22.000000 dramkit-0.5.40/dramkit/speedup/multi_process_concurrent.py
+-rw-rw-rw-   0        0        0     7888 2023-04-07 08:59:34.000000 dramkit-0.5.40/dramkit/speedup/multi_thread.py
+drwxrwxrwx   0        0        0        0 2023-05-15 06:26:58.304762 dramkit-0.5.40/dramkit/sqltools/
+-rw-rw-rw-   0        0        0     2495 2023-02-23 05:15:08.000000 dramkit-0.5.40/dramkit/sqltools/_Hive_notes.py
+-rw-rw-rw-   0        0        0    30416 2023-04-11 01:33:28.000000 dramkit-0.5.40/dramkit/sqltools/_MySQL_notes.py
+-rw-rw-rw-   0        0        0     6849 2023-03-07 09:26:53.000000 dramkit-0.5.40/dramkit/sqltools/_Oracle_notes.py
+-rw-rw-rw-   0        0        0      160 2023-05-01 12:57:19.000000 dramkit-0.5.40/dramkit/sqltools/__init__.py
+-rw-rw-rw-   0        0        0    20285 2023-05-06 13:49:07.000000 dramkit-0.5.40/dramkit/sqltools/cxoracle.py
+-rw-rw-rw-   0        0        0    25908 2023-02-24 11:31:13.000000 dramkit-0.5.40/dramkit/sqltools/py_hive.py
+-rw-rw-rw-   0        0        0    50966 2023-05-06 13:23:21.000000 dramkit-0.5.40/dramkit/sqltools/py_mysql.py
+-rw-rw-rw-   0        0        0    18391 2023-03-22 02:56:24.000000 dramkit-0.5.40/dramkit/sqltools/sql_alchemy.py
+drwxrwxrwx   0        0        0        0 2023-05-15 06:26:58.311773 dramkit-0.5.40/dramkit/webtools/
+-rw-rw-rw-   0        0        0       25 2021-12-24 09:25:22.000000 dramkit-0.5.40/dramkit/webtools/__init__.py
+-rw-rw-rw-   0        0        0     5337 2022-06-25 18:37:55.000000 dramkit-0.5.40/dramkit/webtools/utils_html.py
+drwxrwxrwx   0        0        0        0 2023-05-15 06:26:58.319760 dramkit-0.5.40/dramkit/wechat/
+-rw-rw-rw-   0        0        0       58 2022-09-06 14:04:57.000000 dramkit-0.5.40/dramkit/wechat/__init__.py
+-rw-rw-rw-   0        0        0     7473 2022-10-28 03:03:37.000000 dramkit-0.5.40/dramkit/wechat/qywechat.py
+drwxrwxrwx   0        0        0        0 2023-05-15 06:26:57.898763 dramkit-0.5.40/dramkit.egg-info/
+-rw-rw-rw-   0        0        0     1095 2023-05-15 06:26:53.000000 dramkit-0.5.40/dramkit.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     4877 2023-05-15 06:26:56.000000 dramkit-0.5.40/dramkit.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-15 06:26:53.000000 dramkit-0.5.40/dramkit.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       66 2023-05-15 06:26:53.000000 dramkit-0.5.40/dramkit.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2023-05-15 06:26:53.000000 dramkit-0.5.40/dramkit.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-15 06:26:58.323759 dramkit-0.5.40/setup.cfg
+-rw-rw-rw-   0        0        0     1944 2023-05-01 12:58:33.000000 dramkit-0.5.40/setup.py
```

### Comparing `dramkit-0.5.39/LICENSE` & `dramkit-0.5.40/LICENSE`

 * *Files identical despite different names*

### Comparing `dramkit-0.5.39/PKG-INFO` & `dramkit-0.5.40/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dramkit
-Version: 0.5.39
+Version: 0.5.40
 Summary: DramKit is a toolbox.
 Home-page: https://github.com/Genlovy-Hoo/dramkit/
 Author: Genlovy Hoo, YueYong Hu
 Author-email: genlovhyy@163.com
 License: MIT
 Platform: any
 Description-Content-Type: text/markdown
```

### Comparing `dramkit-0.5.39/README.md` & `dramkit-0.5.40/README.md`

 * *Files identical despite different names*

### Comparing `dramkit-0.5.39/dramkit/__init__.py` & `dramkit-0.5.40/dramkit/__init__.py`

 * *Files identical despite different names*

### Comparing `dramkit-0.5.39/dramkit/_pkg_info.py` & `dramkit-0.5.40/dramkit/_pkg_info.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 pkg_info = {
     '__pkgname__': 'dramkit',
-    '__version__': '0.5.39',
+    '__version__': '0.5.40',
     '__license__': 'MIT',
     '__url__': 'https://github.com/Genlovy-Hoo/dramkit/',
     '__urls__':
         {'pypi': 'https://pypi.org/project/dramkit/',
          'github': 'https://github.com/Genlovy-Hoo/dramkit/',
 		 'document': 'http://www.glhyy.cn/dramkit/doc/html/index.html'
         },
```

### Comparing `dramkit-0.5.39/dramkit/_tmp/CRR.py` & `dramkit-0.5.40/dramkit/_tmp/CRR.py`

 * *Files identical despite different names*

### Comparing `dramkit-0.5.39/dramkit/_tmp/CtrlPreTS.py` & `dramkit-0.5.40/dramkit/_tmp/CtrlPreTS.py`

 * *Files identical despite different names*

### Comparing `dramkit-0.5.39/dramkit/_tmp/NPairSum.py` & `dramkit-0.5.40/dramkit/_tmp/NPairSum.py`

 * *Files identical despite different names*

### Comparing `dramkit-0.5.39/dramkit/_tmp/PIDtest.py` & `dramkit-0.5.40/dramkit/_tmp/PIDtest.py`

 * *Files identical despite different names*

### Comparing `dramkit-0.5.39/dramkit/_tmp/PIDtest2.py` & `dramkit-0.5.40/dramkit/_tmp/PIDtest2.py`

 * *Files identical despite different names*

### Comparing `dramkit-0.5.39/dramkit/_tmp/VMD.py` & `dramkit-0.5.40/dramkit/_tmp/VMD.py`

 * *Files identical despite different names*

### Comparing `dramkit-0.5.39/dramkit/_tmp/cca_test.py` & `dramkit-0.5.40/dramkit/_tmp/cca_test.py`

 * *Files identical despite different names*

### Comparing `dramkit-0.5.39/dramkit/_tmp/dtw_test.py` & `dramkit-0.5.40/dramkit/_tmp/dtw_test.py`

 * *Files identical despite different names*

### Comparing `dramkit-0.5.39/dramkit/_tmp/explore.py` & `dramkit-0.5.40/dramkit/_tmp/explore.py`

 * *Files identical despite different names*

### Comparing `dramkit-0.5.39/dramkit/_tmp/gini.py` & `dramkit-0.5.40/dramkit/_tmp/gini.py`

 * *Files identical despite different names*

### Comparing `dramkit-0.5.39/dramkit/_tmp/merge_sort.py` & `dramkit-0.5.40/dramkit/_tmp/merge_sort.py`

 * *Files identical despite different names*

### Comparing `dramkit-0.5.39/dramkit/_tmp/mouse_move.py` & `dramkit-0.5.40/dramkit/_tmp/mouse_move.py`

 * *Files identical despite different names*

### Comparing `dramkit-0.5.39/dramkit/_tmp/mpc_test1.py` & `dramkit-0.5.40/dramkit/_tmp/mpc_test1.py`

 * *Files identical despite different names*

### Comparing `dramkit-0.5.39/dramkit/_tmp/options_Implied_volatility.py` & `dramkit-0.5.40/dramkit/_tmp/options_Implied_volatility.py`

 * *Files identical despite different names*

### Comparing `dramkit-0.5.39/dramkit/_tmp/plot_test.py` & `dramkit-0.5.40/dramkit/_tmp/plot_test.py`

 * *Files identical despite different names*

### Comparing `dramkit-0.5.39/dramkit/_tmp/plot_test2.py` & `dramkit-0.5.40/dramkit/_tmp/plot_test2.py`

 * *Files identical despite different names*

### Comparing `dramkit-0.5.39/dramkit/_tmp/simple_smooth.py` & `dramkit-0.5.40/dramkit/_tmp/simple_smooth.py`

 * *Files identical despite different names*

### Comparing `dramkit-0.5.39/dramkit/_tmp/test_async_washs.py` & `dramkit-0.5.40/dramkit/_tmp/test_async_washs.py`

 * *Files identical despite different names*

### Comparing `dramkit-0.5.39/dramkit/_tmp/test_await_timeout.py` & `dramkit-0.5.40/dramkit/_tmp/test_await_timeout.py`

 * *Files identical despite different names*

### Comparing `dramkit-0.5.39/dramkit/_tmp/test_backtrader.py` & `dramkit-0.5.40/dramkit/_tmp/test_backtrader.py`

 * *Files identical despite different names*

### Comparing `dramkit-0.5.39/dramkit/_tmp/test_chatgpt_v1.py` & `dramkit-0.5.40/dramkit/_tmp/test_chatgpt_v1.py`

 * *Files identical despite different names*

### Comparing `dramkit-0.5.39/dramkit/_tmp/test_code.py` & `dramkit-0.5.40/dramkit/_tmp/test_code.py`

 * *Files identical despite different names*

### Comparing `dramkit-0.5.39/dramkit/_tmp/test_find_peaks.py` & `dramkit-0.5.40/dramkit/_tmp/test_find_peaks.py`

 * *Files identical despite different names*

### Comparing `dramkit-0.5.39/dramkit/_tmp/test_get_var_name.py` & `dramkit-0.5.40/dramkit/_tmp/test_get_var_name.py`

 * *Files identical despite different names*

### Comparing `dramkit-0.5.39/dramkit/_tmp/test_grading.py` & `dramkit-0.5.40/dramkit/_tmp/test_grading.py`

 * *Files identical despite different names*

### Comparing `dramkit-0.5.39/dramkit/_tmp/test_lr.py` & `dramkit-0.5.40/dramkit/_tmp/test_lr.py`

 * *Files identical despite different names*

### Comparing `dramkit-0.5.39/dramkit/_tmp/test_maxsort.py` & `dramkit-0.5.40/dramkit/_tmp/test_maxsort.py`

 * *Files identical despite different names*

### Comparing `dramkit-0.5.39/dramkit/_tmp/test_pywechat.py` & `dramkit-0.5.40/dramkit/_tmp/test_pywechat.py`

 * *Files identical despite different names*

### Comparing `dramkit-0.5.39/dramkit/_tmp/test_tree.py` & `dramkit-0.5.40/dramkit/_tmp/test_tree.py`

 * *Files identical despite different names*

### Comparing `dramkit-0.5.39/dramkit/_tmp/test_tree2.py` & `dramkit-0.5.40/dramkit/_tmp/test_tree2.py`

 * *Files identical despite different names*

### Comparing `dramkit-0.5.39/dramkit/_tmp/test_wechat_work.py` & `dramkit-0.5.40/dramkit/_tmp/test_wechat_work.py`

 * *Files identical despite different names*

### Comparing `dramkit-0.5.39/dramkit/_tmp/tfDNNCls_test.py` & `dramkit-0.5.40/dramkit/_tmp/tfDNNCls_test.py`

 * *Files identical despite different names*

### Comparing `dramkit-0.5.39/dramkit/_tmp/tmp.py` & `dramkit-0.5.40/dramkit/_tmp/tmp.py`

 * *Files identical despite different names*

### Comparing `dramkit-0.5.39/dramkit/_tmp/tmp_args.py` & `dramkit-0.5.40/dramkit/_tmp/tmp_args.py`

 * *Files identical despite different names*

### Comparing `dramkit-0.5.39/dramkit/_tmp/transformer_pytorch.py` & `dramkit-0.5.40/dramkit/_tmp/transformer_pytorch.py`

 * *Files identical despite different names*

### Comparing `dramkit-0.5.39/dramkit/_tmp/utils_SignalDec.py` & `dramkit-0.5.40/dramkit/_tmp/utils_SignalDec.py`

 * *Files identical despite different names*

### Comparing `dramkit-0.5.39/dramkit/_tmp/utils_TimeSeries.py` & `dramkit-0.5.40/dramkit/_tmp/utils_TimeSeries.py`

 * *Files identical despite different names*

### Comparing `dramkit-0.5.39/dramkit/_tmp/utils_lottery.py` & `dramkit-0.5.40/dramkit/_tmp/utils_lottery.py`

 * *Files identical despite different names*

### Comparing `dramkit-0.5.39/dramkit/_tmp/utils_rl.py` & `dramkit-0.5.40/dramkit/_tmp/utils_rl.py`

 * *Files identical despite different names*

### Comparing `dramkit-0.5.39/dramkit/_tmp/utils_rl2.py` & `dramkit-0.5.40/dramkit/_tmp/utils_rl2.py`

 * *Files identical despite different names*

### Comparing `dramkit-0.5.39/dramkit/_tmp/utils_rl3.py` & `dramkit-0.5.40/dramkit/_tmp/utils_rl3.py`

 * *Files identical despite different names*

### Comparing `dramkit-0.5.39/dramkit/_tmp/utils_rl4.py` & `dramkit-0.5.40/dramkit/_tmp/utils_rl4.py`

 * *Files identical despite different names*

### Comparing `dramkit-0.5.39/dramkit/_tmp/utils_rl5.py` & `dramkit-0.5.40/dramkit/_tmp/utils_rl5.py`

 * *Files identical despite different names*

### Comparing `dramkit-0.5.39/dramkit/_tmp/utils_rl6.py` & `dramkit-0.5.40/dramkit/_tmp/utils_rl6.py`

 * *Files identical despite different names*

### Comparing `dramkit-0.5.39/dramkit/_tmp/utils_rl7.py` & `dramkit-0.5.40/dramkit/_tmp/utils_rl7.py`

 * *Files identical despite different names*

### Comparing `dramkit-0.5.39/dramkit/_tmp/utils_sem.py` & `dramkit-0.5.40/dramkit/_tmp/utils_sem.py`

 * *Files identical despite different names*

### Comparing `dramkit-0.5.39/dramkit/backpacks/backpack01_float_dy.py` & `dramkit-0.5.40/dramkit/backpacks/backpack01_float_dy.py`

 * *Files identical despite different names*

### Comparing `dramkit-0.5.39/dramkit/backpacks/backpack01_int_dy.py` & `dramkit-0.5.40/dramkit/backpacks/backpack01_int_dy.py`

 * *Files identical despite different names*

### Comparing `dramkit-0.5.39/dramkit/chncal/__init__.py` & `dramkit-0.5.40/dramkit/chncal/__init__.py`

 * *Files identical despite different names*

### Comparing `dramkit-0.5.39/dramkit/chncal/apis.py` & `dramkit-0.5.40/dramkit/chncal/apis.py`

 * *Files identical despite different names*

### Comparing `dramkit-0.5.39/dramkit/chncal/constants.py` & `dramkit-0.5.40/dramkit/chncal/constants.py`

 * *Files identical despite different names*

### Comparing `dramkit-0.5.39/dramkit/chncal/constants_fate.py` & `dramkit-0.5.40/dramkit/chncal/constants_fate.py`

 * *Files identical despite different names*

### Comparing `dramkit-0.5.39/dramkit/chncal/constants_hko.py` & `dramkit-0.5.40/dramkit/chncal/constants_hko.py`

 * *Files identical despite different names*

### Comparing `dramkit-0.5.39/dramkit/chncal/constants_trade_dates.py` & `dramkit-0.5.40/dramkit/chncal/constants_trade_dates.py`

 * *Files 0% similar despite different names*

```diff
@@ -6086,14 +6086,22 @@
     ("CFFEX", datetime.date(year=2023, month=4, day=28)): 1,
     ("CFFEX", datetime.date(year=2023, month=4, day=29)): 0,
     ("CFFEX", datetime.date(year=2023, month=4, day=30)): 0,
     ("CFFEX", datetime.date(year=2023, month=5, day=1)): 0,
     ("CFFEX", datetime.date(year=2023, month=5, day=2)): 0,
     ("CFFEX", datetime.date(year=2023, month=5, day=3)): 0,
     ("CFFEX", datetime.date(year=2023, month=5, day=4)): 1,
+    ("CFFEX", datetime.date(year=2023, month=5, day=5)): 1,
+    ("CFFEX", datetime.date(year=2023, month=5, day=6)): 0,
+    ("CFFEX", datetime.date(year=2023, month=5, day=7)): 0,
+    ("CFFEX", datetime.date(year=2023, month=5, day=8)): 1,
+    ("CFFEX", datetime.date(year=2023, month=5, day=9)): 1,
+    ("CFFEX", datetime.date(year=2023, month=5, day=10)): 1,
+    ("CFFEX", datetime.date(year=2023, month=5, day=11)): 1,
+    ("CFFEX", datetime.date(year=2023, month=5, day=12)): 1,
     ("CZCE", datetime.date(year=1990, month=10, day=12)): 1,
     ("CZCE", datetime.date(year=1990, month=10, day=13)): 0,
     ("CZCE", datetime.date(year=1990, month=10, day=14)): 0,
     ("CZCE", datetime.date(year=1990, month=10, day=15)): 1,
     ("CZCE", datetime.date(year=1990, month=10, day=16)): 1,
     ("CZCE", datetime.date(year=1990, month=10, day=17)): 1,
     ("CZCE", datetime.date(year=1990, month=10, day=18)): 1,
@@ -17978,14 +17986,22 @@
     ("CZCE", datetime.date(year=2023, month=4, day=28)): 1,
     ("CZCE", datetime.date(year=2023, month=4, day=29)): 0,
     ("CZCE", datetime.date(year=2023, month=4, day=30)): 0,
     ("CZCE", datetime.date(year=2023, month=5, day=1)): 0,
     ("CZCE", datetime.date(year=2023, month=5, day=2)): 0,
     ("CZCE", datetime.date(year=2023, month=5, day=3)): 0,
     ("CZCE", datetime.date(year=2023, month=5, day=4)): 1,
+    ("CZCE", datetime.date(year=2023, month=5, day=5)): 1,
+    ("CZCE", datetime.date(year=2023, month=5, day=6)): 0,
+    ("CZCE", datetime.date(year=2023, month=5, day=7)): 0,
+    ("CZCE", datetime.date(year=2023, month=5, day=8)): 1,
+    ("CZCE", datetime.date(year=2023, month=5, day=9)): 1,
+    ("CZCE", datetime.date(year=2023, month=5, day=10)): 1,
+    ("CZCE", datetime.date(year=2023, month=5, day=11)): 1,
+    ("CZCE", datetime.date(year=2023, month=5, day=12)): 1,
     ("DCE", datetime.date(year=1993, month=3, day=1)): 1,
     ("DCE", datetime.date(year=1993, month=3, day=2)): 1,
     ("DCE", datetime.date(year=1993, month=3, day=3)): 1,
     ("DCE", datetime.date(year=1993, month=3, day=4)): 1,
     ("DCE", datetime.date(year=1993, month=3, day=5)): 1,
     ("DCE", datetime.date(year=1993, month=3, day=6)): 0,
     ("DCE", datetime.date(year=1993, month=3, day=7)): 0,
@@ -28999,14 +29015,22 @@
     ("DCE", datetime.date(year=2023, month=4, day=28)): 1,
     ("DCE", datetime.date(year=2023, month=4, day=29)): 0,
     ("DCE", datetime.date(year=2023, month=4, day=30)): 0,
     ("DCE", datetime.date(year=2023, month=5, day=1)): 0,
     ("DCE", datetime.date(year=2023, month=5, day=2)): 0,
     ("DCE", datetime.date(year=2023, month=5, day=3)): 0,
     ("DCE", datetime.date(year=2023, month=5, day=4)): 1,
+    ("DCE", datetime.date(year=2023, month=5, day=5)): 1,
+    ("DCE", datetime.date(year=2023, month=5, day=6)): 0,
+    ("DCE", datetime.date(year=2023, month=5, day=7)): 0,
+    ("DCE", datetime.date(year=2023, month=5, day=8)): 1,
+    ("DCE", datetime.date(year=2023, month=5, day=9)): 1,
+    ("DCE", datetime.date(year=2023, month=5, day=10)): 1,
+    ("DCE", datetime.date(year=2023, month=5, day=11)): 1,
+    ("DCE", datetime.date(year=2023, month=5, day=12)): 1,
     ("INE", datetime.date(year=2017, month=5, day=23)): 1,
     ("INE", datetime.date(year=2017, month=5, day=24)): 1,
     ("INE", datetime.date(year=2017, month=5, day=25)): 1,
     ("INE", datetime.date(year=2017, month=5, day=26)): 1,
     ("INE", datetime.date(year=2017, month=5, day=27)): 0,
     ("INE", datetime.date(year=2017, month=5, day=28)): 0,
     ("INE", datetime.date(year=2017, month=5, day=29)): 0,
@@ -31171,14 +31195,22 @@
     ("INE", datetime.date(year=2023, month=4, day=28)): 1,
     ("INE", datetime.date(year=2023, month=4, day=29)): 0,
     ("INE", datetime.date(year=2023, month=4, day=30)): 0,
     ("INE", datetime.date(year=2023, month=5, day=1)): 0,
     ("INE", datetime.date(year=2023, month=5, day=2)): 0,
     ("INE", datetime.date(year=2023, month=5, day=3)): 0,
     ("INE", datetime.date(year=2023, month=5, day=4)): 1,
+    ("INE", datetime.date(year=2023, month=5, day=5)): 1,
+    ("INE", datetime.date(year=2023, month=5, day=6)): 0,
+    ("INE", datetime.date(year=2023, month=5, day=7)): 0,
+    ("INE", datetime.date(year=2023, month=5, day=8)): 1,
+    ("INE", datetime.date(year=2023, month=5, day=9)): 1,
+    ("INE", datetime.date(year=2023, month=5, day=10)): 1,
+    ("INE", datetime.date(year=2023, month=5, day=11)): 1,
+    ("INE", datetime.date(year=2023, month=5, day=12)): 1,
     ("SHFE", datetime.date(year=1991, month=5, day=28)): 1,
     ("SHFE", datetime.date(year=1991, month=5, day=29)): 1,
     ("SHFE", datetime.date(year=1991, month=5, day=30)): 1,
     ("SHFE", datetime.date(year=1991, month=5, day=31)): 1,
     ("SHFE", datetime.date(year=1991, month=6, day=1)): 0,
     ("SHFE", datetime.date(year=1991, month=6, day=2)): 0,
     ("SHFE", datetime.date(year=1991, month=6, day=3)): 1,
@@ -42835,14 +42867,22 @@
     ("SHFE", datetime.date(year=2023, month=4, day=28)): 1,
     ("SHFE", datetime.date(year=2023, month=4, day=29)): 0,
     ("SHFE", datetime.date(year=2023, month=4, day=30)): 0,
     ("SHFE", datetime.date(year=2023, month=5, day=1)): 0,
     ("SHFE", datetime.date(year=2023, month=5, day=2)): 0,
     ("SHFE", datetime.date(year=2023, month=5, day=3)): 0,
     ("SHFE", datetime.date(year=2023, month=5, day=4)): 1,
+    ("SHFE", datetime.date(year=2023, month=5, day=5)): 1,
+    ("SHFE", datetime.date(year=2023, month=5, day=6)): 0,
+    ("SHFE", datetime.date(year=2023, month=5, day=7)): 0,
+    ("SHFE", datetime.date(year=2023, month=5, day=8)): 1,
+    ("SHFE", datetime.date(year=2023, month=5, day=9)): 1,
+    ("SHFE", datetime.date(year=2023, month=5, day=10)): 1,
+    ("SHFE", datetime.date(year=2023, month=5, day=11)): 1,
+    ("SHFE", datetime.date(year=2023, month=5, day=12)): 1,
     ("SSE", datetime.date(year=1990, month=12, day=19)): 1,
     ("SSE", datetime.date(year=1990, month=12, day=20)): 1,
     ("SSE", datetime.date(year=1990, month=12, day=21)): 1,
     ("SSE", datetime.date(year=1990, month=12, day=22)): 0,
     ("SSE", datetime.date(year=1990, month=12, day=23)): 0,
     ("SSE", datetime.date(year=1990, month=12, day=24)): 1,
     ("SSE", datetime.date(year=1990, month=12, day=25)): 1,
@@ -54660,14 +54700,22 @@
     ("SSE", datetime.date(year=2023, month=4, day=28)): 1,
     ("SSE", datetime.date(year=2023, month=4, day=29)): 0,
     ("SSE", datetime.date(year=2023, month=4, day=30)): 0,
     ("SSE", datetime.date(year=2023, month=5, day=1)): 0,
     ("SSE", datetime.date(year=2023, month=5, day=2)): 0,
     ("SSE", datetime.date(year=2023, month=5, day=3)): 0,
     ("SSE", datetime.date(year=2023, month=5, day=4)): 1,
+    ("SSE", datetime.date(year=2023, month=5, day=5)): 1,
+    ("SSE", datetime.date(year=2023, month=5, day=6)): 0,
+    ("SSE", datetime.date(year=2023, month=5, day=7)): 0,
+    ("SSE", datetime.date(year=2023, month=5, day=8)): 1,
+    ("SSE", datetime.date(year=2023, month=5, day=9)): 1,
+    ("SSE", datetime.date(year=2023, month=5, day=10)): 1,
+    ("SSE", datetime.date(year=2023, month=5, day=11)): 1,
+    ("SSE", datetime.date(year=2023, month=5, day=12)): 1,
     ("SZSE", datetime.date(year=1991, month=7, day=3)): 1,
     ("SZSE", datetime.date(year=1991, month=7, day=4)): 1,
     ("SZSE", datetime.date(year=1991, month=7, day=5)): 1,
     ("SZSE", datetime.date(year=1991, month=7, day=6)): 0,
     ("SZSE", datetime.date(year=1991, month=7, day=7)): 0,
     ("SZSE", datetime.date(year=1991, month=7, day=8)): 1,
     ("SZSE", datetime.date(year=1991, month=7, day=9)): 1,
@@ -66289,8 +66337,16 @@
     ("SZSE", datetime.date(year=2023, month=4, day=28)): 1,
     ("SZSE", datetime.date(year=2023, month=4, day=29)): 0,
     ("SZSE", datetime.date(year=2023, month=4, day=30)): 0,
     ("SZSE", datetime.date(year=2023, month=5, day=1)): 0,
     ("SZSE", datetime.date(year=2023, month=5, day=2)): 0,
     ("SZSE", datetime.date(year=2023, month=5, day=3)): 0,
     ("SZSE", datetime.date(year=2023, month=5, day=4)): 1,
+    ("SZSE", datetime.date(year=2023, month=5, day=5)): 1,
+    ("SZSE", datetime.date(year=2023, month=5, day=6)): 0,
+    ("SZSE", datetime.date(year=2023, month=5, day=7)): 0,
+    ("SZSE", datetime.date(year=2023, month=5, day=8)): 1,
+    ("SZSE", datetime.date(year=2023, month=5, day=9)): 1,
+    ("SZSE", datetime.date(year=2023, month=5, day=10)): 1,
+    ("SZSE", datetime.date(year=2023, month=5, day=11)): 1,
+    ("SZSE", datetime.date(year=2023, month=5, day=12)): 1,
 }
```

### Comparing `dramkit-0.5.39/dramkit/chncal/constants_wuxing.py` & `dramkit-0.5.40/dramkit/chncal/constants_wuxing.py`

 * *Files identical despite different names*

### Comparing `dramkit-0.5.39/dramkit/chncal/constants_zodiac_marry.py` & `dramkit-0.5.40/dramkit/chncal/constants_zodiac_marry.py`

 * *Files identical despite different names*

### Comparing `dramkit-0.5.39/dramkit/chncal/solar_terms.py` & `dramkit-0.5.40/dramkit/chncal/solar_terms.py`

 * *Files identical despite different names*

### Comparing `dramkit-0.5.39/dramkit/cryptotools.py` & `dramkit-0.5.40/dramkit/cryptotools.py`

 * *Files identical despite different names*

### Comparing `dramkit-0.5.39/dramkit/datetimetools.py` & `dramkit-0.5.40/dramkit/datetimetools.py`

 * *Files 1% similar despite different names*

```diff
@@ -673,14 +673,36 @@
         date = today_date()
     day = x2datetime(date)
     next_month = day.replace(day=28) + datetime.timedelta(days=4)
     month_end = next_month - datetime.timedelta(days=next_month.day)
     return copy_format(month_end, date)
 
 
+def get_next_nmonth_start_end(date=None, n=1):
+    if pd.isnull(date):
+        date = today_date()
+    day = x2datetime(date)
+    y, m = day.year, day.month
+    y, m = get_2part_next(y, m, 12, n)
+    month_start = pd.to_datetime('%s-%s-01'%(y, m))
+    next_month = month_start.replace(day=28) + datetime.timedelta(days=4)
+    month_end = next_month - datetime.timedelta(days=next_month.day)
+    return copy_format(month_start, date), copy_format(month_end, date)
+
+
+def get_next_nquarter_start_end(date=None, n=1):
+    if pd.isnull(date):
+        date = today_date()
+    day = x2datetime(date)
+    y, q = day.year, day.quarter
+    y, q = get_2part_next(y, q, 4, n)
+    start, end = get_quarter_start_end_by_yq(y, q, '')
+    return copy_format(start, date), copy_format(end, date)
+
+
 def get_date_format(date,
                     joiners=[' ', '-', '/', '*', '#', '@', '.', '_']
                     ):
     '''
     判断日期格式位，返回日期位数和连接符
 
     Parameters
```

### Comparing `dramkit-0.5.39/dramkit/datsci/_utils_ann.py` & `dramkit-0.5.40/dramkit/datsci/_utils_ann.py`

 * *Files identical despite different names*

### Comparing `dramkit-0.5.39/dramkit/datsci/activate_funcs.py` & `dramkit-0.5.40/dramkit/datsci/activate_funcs.py`

 * *Files identical despite different names*

### Comparing `dramkit-0.5.39/dramkit/datsci/ahp.py` & `dramkit-0.5.40/dramkit/datsci/ahp.py`

 * *Files identical despite different names*

### Comparing `dramkit-0.5.39/dramkit/datsci/ahp_sim_ri.py` & `dramkit-0.5.40/dramkit/datsci/ahp_sim_ri.py`

 * *Files identical despite different names*

### Comparing `dramkit-0.5.39/dramkit/datsci/apriori.py` & `dramkit-0.5.40/dramkit/datsci/apriori.py`

 * *Files identical despite different names*

### Comparing `dramkit-0.5.39/dramkit/datsci/curvature.py` & `dramkit-0.5.40/dramkit/datsci/curvature.py`

 * *Files identical despite different names*

### Comparing `dramkit-0.5.39/dramkit/datsci/elm_cls.py` & `dramkit-0.5.40/dramkit/datsci/elm_cls.py`

 * *Files identical despite different names*

### Comparing `dramkit-0.5.39/dramkit/datsci/elm_reg.py` & `dramkit-0.5.40/dramkit/datsci/elm_reg.py`

 * *Files identical despite different names*

### Comparing `dramkit-0.5.39/dramkit/datsci/entropy_weight.py` & `dramkit-0.5.40/dramkit/datsci/entropy_weight.py`

 * *Files identical despite different names*

### Comparing `dramkit-0.5.39/dramkit/datsci/find_maxmin.py` & `dramkit-0.5.40/dramkit/datsci/find_maxmin.py`

 * *Files 0% similar despite different names*

```diff
@@ -72,23 +72,24 @@
     if series.isna().sum() > 0:        
         if skip_nan:
             logger_show('发现无效值，可能导致结果错误！', logger, 'warn')
         else:
             raise ValueError('发现无效值，请先处理！')
 
     # 序列名和索引名
-    series.name = 'series'
+    if series.name is None:
+        series.name = 'series'
     if series.index.name is None:
         series.index.name = 'idx'
 
     df = pd.DataFrame(series)
     col = df.columns[0]
     df.reset_index(inplace=True)
     
-    # plot_series(df, {'series': '.-k'}, title='原始数据', grids=True)
+    # plot_series(df, {col: '.-k'}, title='原始数据', grids=True)
 
     # 所有转折点
     df['dif'] = df[col].diff()
     df['dif_big'] = (df['dif'] > 0).astype(int)
     df['dif_sml'] = -1 * (df['dif'] < 0).astype(int)
     ktmp = 1
     while ktmp < df.shape[0] and df.loc[df.index[ktmp], 'dif'] == 0:
@@ -1083,15 +1084,15 @@
     # '''
     # 50ETF日线行情------------------------------------------------------------
     fpath = '../_test/510500.SH_daily_qfq.csv'
     his_data = load_csv(fpath)
     his_data.set_index('date', drop=False, inplace=True)
 
     # N = his_data.shape[0]
-    N = 5000
+    N = 200
     col = 'close'
     df = his_data.iloc[-N:, :].copy()
 
     # t_min = None
     t_min = 3
     df['label'] = find_maxmin(df[col], t_min=t_min)
 
@@ -1101,15 +1102,15 @@
     if OK:
         print('极值点排列正确！')
     else:
         print('极值点排列错误:', e)
     # '''
 
     #%%
-    # '''
+    '''
     # 上证50分钟行情------------------------------------------------------------
     his_data = load_index_joinquant('000016', '1min')
     his_data['time'] = his_data['time'].apply(lambda x:
                     x.replace('-', '').replace(':', '').replace(' ', '')[:-2])
     his_data.set_index('time', drop=False, inplace=True)
     his_data['ma'] = his_data['close'].rolling(20).mean()
```

### Comparing `dramkit-0.5.39/dramkit/datsci/freq_item_set.py` & `dramkit-0.5.40/dramkit/datsci/freq_item_set.py`

 * *Files identical despite different names*

### Comparing `dramkit-0.5.39/dramkit/datsci/lr.py` & `dramkit-0.5.40/dramkit/datsci/lr.py`

 * *Files identical despite different names*

### Comparing `dramkit-0.5.39/dramkit/datsci/preprocess.py` & `dramkit-0.5.40/dramkit/datsci/preprocess.py`

 * *Files identical despite different names*

### Comparing `dramkit-0.5.39/dramkit/datsci/stats.py` & `dramkit-0.5.40/dramkit/datsci/stats.py`

 * *Files identical despite different names*

### Comparing `dramkit-0.5.39/dramkit/datsci/time_series.py` & `dramkit-0.5.40/dramkit/datsci/time_series.py`

 * *Files identical despite different names*

### Comparing `dramkit-0.5.39/dramkit/datsci/topsis.py` & `dramkit-0.5.40/dramkit/datsci/topsis.py`

 * *Files identical despite different names*

### Comparing `dramkit-0.5.39/dramkit/datsci/utils_lgb.py` & `dramkit-0.5.40/dramkit/datsci/utils_lgb.py`

 * *Files identical despite different names*

### Comparing `dramkit-0.5.39/dramkit/datsci/utils_ml.py` & `dramkit-0.5.40/dramkit/datsci/utils_ml.py`

 * *Files identical despite different names*

### Comparing `dramkit-0.5.39/dramkit/find_addends/find_addends_backpack01float.py` & `dramkit-0.5.40/dramkit/find_addends/find_addends_backpack01float.py`

 * *Files identical despite different names*

### Comparing `dramkit-0.5.39/dramkit/find_addends/find_addends_backpack01int.py` & `dramkit-0.5.40/dramkit/find_addends/find_addends_backpack01int.py`

 * *Files identical despite different names*

### Comparing `dramkit-0.5.39/dramkit/find_addends/find_addends_bigfirst.py` & `dramkit-0.5.40/dramkit/find_addends/find_addends_bigfirst.py`

 * *Files identical despite different names*

### Comparing `dramkit-0.5.39/dramkit/find_addends/find_addends_recu.py` & `dramkit-0.5.40/dramkit/find_addends/find_addends_recu.py`

 * *Files identical despite different names*

### Comparing `dramkit-0.5.39/dramkit/find_addends/find_addends_smlfirst.py` & `dramkit-0.5.40/dramkit/find_addends/find_addends_smlfirst.py`

 * *Files identical despite different names*

### Comparing `dramkit-0.5.39/dramkit/find_addends/find_addends_utils.py` & `dramkit-0.5.40/dramkit/find_addends/find_addends_utils.py`

 * *Files identical despite different names*

### Comparing `dramkit-0.5.39/dramkit/gentools.py` & `dramkit-0.5.40/dramkit/gentools.py`

 * *Files 2% similar despite different names*

```diff
@@ -305,15 +305,17 @@
                     timeout_show_str=timeout_show_str,
                     kill_when_timeout=kill_when_timeout,
                     **kwargs)
         return timeouter
     return transfunc
         
         
-def try_repeat_run(n_max_run=3, logger=None, sleep_seconds=0,
+def try_repeat_run(n_max_run=3,
+                   logger=None,
+                   sleep_seconds=0,
                    force_rep=False):
     '''
     | 作为装饰器尝试多次运行指定函数
     | 使用场景：第一次运行可能出错，需要再次运行(比如取数据时第一次可能连接超时，需要再取一次)
     
     Parameters
     ----------
@@ -355,42 +357,60 @@
         @wraps(func)
         def repeater(*args, **kwargs):
             '''尝试多次运行func'''
             if not force_rep:
                 n_run, ok = 0, False
                 while not ok and n_run < n_max_run:
                     n_run += 1
-                    # logger_show('第%s次运行`%s`...'%(n_run, func.__name__),
-                    #             logger, 'info')
+                    # if isnull(logger) and 'logger' in kwargs:
+                    #     logger_show('第%s次运行`%s`...'%(n_run, func.__name__),
+                    #                 kwargs['logger'], 'info')
+                    # else:
+                    #     logger_show('第%s次运行`%s`...'%(n_run, func.__name__),
+                    #                 logger, 'info')
                     try:
                         result = func(*args, **kwargs)
                         return result
                     except:
                         if n_run == n_max_run:
-                            logger_show(traceback.format_exc(), logger)
-                            logger_show('`%s`运行失败，共运行了%s次。'%(func.__name__, n_run),
-                                        logger, 'error')                            
+                            if isnull(logger) and 'logger' in kwargs:
+                                logger_show(traceback.format_exc(), kwargs['logger'])
+                                logger_show('`%s`运行失败，共运行了%s次。'%(func.__name__, n_run),
+                                            kwargs['logger'], 'error')
+                            else:
+                                logger_show(traceback.format_exc(), logger)
+                                logger_show('`%s`运行失败，共运行了%s次。'%(func.__name__, n_run),
+                                            logger, 'error')                            
                             return
                         else:
                             if sleep_seconds > 0:
                                 time.sleep(sleep_seconds)
                             else:
                                 pass
             else:
                 n_run = 0
                 while n_run < n_max_run:
                     n_run += 1
                     try:
                         result = func(*args, **kwargs)
-                        logger_show('`%s`第%s运行：成功。'%(func.__name__, n_run),
-                                    logger, 'info')
+                        if isnull(logger) and 'logger' in kwargs:
+                            logger_show('`%s`第%s运行：成功。'%(func.__name__, n_run),
+                                        kwargs['logger'], 'info')
+                        else:
+                            logger_show('`%s`第%s运行：成功。'%(func.__name__, n_run),
+                                        logger, 'info')
                     except:
-                        logger_show(traceback.format_exc(), logger)
-                        logger_show('`%s`第%s运行：失败。'%(func.__name__, n_run),
-                                    logger, 'error')
+                        if isnull(logger) and 'logger' in kwargs:
+                            logger_show(traceback.format_exc(), kwargs['logger'])
+                            logger_show('`%s`第%s运行：失败。'%(func.__name__, n_run),
+                                        kwargs['logger'], 'error')
+                        else:
+                            logger_show(traceback.format_exc(), logger)
+                            logger_show('`%s`第%s运行：失败。'%(func.__name__, n_run),
+                                        logger, 'error')
                         result = None
                     if sleep_seconds > 0:
                         time.sleep(sleep_seconds)
                 return result
         return repeater
     return transfunc
 
@@ -2739,14 +2759,15 @@
     TODO
     ----
     - idcols唯一性检查
     - 填充时选择交易日或工作日参数设置
     - idx_cols中有nan时检查和处理
     - 其他参数/变量规范重写
     - 日期格式不写死，根据tcol列转化
+    - 日期生成函数自定义，比如可以日频、月频、小时频率等
     '''
     vcols = check_list_arg(vcols, allow_none=True)
     idcols = check_list_arg(idcols)
     if isnull(vcols):
         vcols = [x for x in df.columns if not x in idcols+[tcol]]
     if df.shape[0] == 0:
         return pd.DataFrame(columns=[tcol]+idcols+vcols)
@@ -2769,18 +2790,52 @@
     df = df.fillna(method='ffill')#.fillna(method='bfill')
     df = df.stack(level=idcols).reset_index()
     df = df.replace({'__tmp_None_tmp__': np.nan})
     df = df.sort_values(idcols+[tcol])
     return df
 
 
-def get_first_appear_index(series, values, ascending=False,
-                           return_iloc=False):
-    '''获取values中的值在series中第一次出现时的索引'''
-    raise NotImplementedError
+def get_first_appear(series, func_cond,
+                     reverse=False,
+                     return_iloc=False):
+    '''
+    | 获取满足func_cond(x)为True的值在series中第一次出现时的索引
+    | 若reverse为True，则是最后一次出现
+    | 若return_iloc为True，则返回行号和值，否则返回索引和值
+    '''
+    assert callable(func_cond)
+    # df = pd.DataFrame({'s': series})
+    # df['ok'] = df['s'].apply(lambda x: func_cond(x)).astype(int)
+    # if return_iloc:
+    #     df = df.reset_index(drop=True)
+    # idx = -1 if reverse else 0
+    # try:
+    #     return df[df['ok'] == 1].index[idx], df[df['ok'] == 1]['ok'].iloc[idx]
+    # except:
+    #     return None, None
+    if not reverse:
+        n, k, find = len(series), 0, False
+        while k < n and not find:
+            find = func_cond(series.iloc[k])
+            if find:
+                if return_iloc:
+                    return k, series.iloc[k]
+                return series.index[k], series.iloc[k]
+            k += 1
+        return None, None
+    else:
+        k, find = len(series)-1, False
+        while k > -1 and not find:
+            find = func_cond(series.iloc[k])
+            if find:
+                if return_iloc:
+                    return k, series.iloc[k]
+                return series.index[k], series.iloc[k]
+            k -= 1
+        return None, None
 
 
 def get_appear_order(series, ascending=True):
     '''
     标注series (`pandas.Series` , 离散值)中重复元素是第几次出现，
     
     返回为 `pandas.Series`，ascending设置返回结果是否按出现次序升序排列
@@ -2887,14 +2942,45 @@
     '''计算df的每个index出现的次数'''
     df_index = pd.DataFrame({'index_': df.index})
     df_index['count'] = count_values(df_index, 'index_')
     df_index.index = df_index['index_']
     return df_index['count']
 
 
+def get_all_turns(series):
+    '''获取序列series中所有的转折点，返回series中-1位低点，1位高点'''
+    s = series.copy()
+    if s.name is None:
+        s.name = 'series'
+    if s.index.name is None:
+        s.index.name = 'idx'
+    df = pd.DataFrame(s)
+    col = df.columns[0]
+    df.reset_index(inplace=True)
+    
+    df['dif'] = df[col].diff()
+    df['dif_big'] = (df['dif'] > 0).astype(int)
+    df['dif_sml'] = -1 * (df['dif'] < 0).astype(int)
+    ktmp = 1
+    while ktmp < df.shape[0] and df.loc[df.index[ktmp], 'dif'] == 0:
+        ktmp += 1
+    if df.loc[df.index[ktmp], 'dif'] > 0:
+        df.loc[df.index[0], 'dif_sml'] = -1
+    elif df.loc[df.index[ktmp], 'dif'] < 0:
+        df.loc[df.index[0], 'dif_big'] = 1
+    df['label'] = df['dif_big'] + df['dif_sml']
+    label_ = replace_repeat_pd(df['label'][::-1], 1, 0)
+    label_ = replace_repeat_pd(label_, -1, 0)
+    df['label'] = label_[::-1]
+    
+    df.set_index(s.index.name, inplace=True)
+    
+    return df['label']
+
+
 def group_shift():
     '''分组shift，待实现'''
     raise NotImplementedError
     
     
 def rolling_corr(df, col1, col2, *args, **kwargs):
     '''滚动相关性（2个变量）'''
```

### Comparing `dramkit-0.5.39/dramkit/install_check.py` & `dramkit-0.5.40/dramkit/install_check.py`

 * *Files identical despite different names*

### Comparing `dramkit-0.5.39/dramkit/iotools.py` & `dramkit-0.5.40/dramkit/iotools.py`

 * *Files 1% similar despite different names*

```diff
@@ -705,19 +705,25 @@
 
 def archive_df(df_old, df_new, idcols=None,
                del_dup_cols=None, rep_keep='new',
                sort_cols=None, ascendings=True,
                old_ftype=None, new_ftype=None,
                save_ftype=None, save_path=None,
                kwargs_read_old={}, kwargs_read_new={},
-               kwargs_save={}, method='merge',
+               kwargs_save={'index': None},
+               method='merge',
                logger=None):
     '''
     合并df_new和df_old，再排序、去重、写入csv或excel
     '''
+    if isnull(save_path):
+        if isinstance(df_old, str):
+            save_path = df_old
+        elif isinstance(df_new, str):
+            save_path = df_new
     if isinstance(df_new, str):
         df_new = load_df_pd(df_new, ftype=new_ftype,
                             logger=logger,
                             **kwargs_read_new)
     if isinstance(df_old, str):
         if os.path.exists(df_old):
             if isnull(df_new) or df_new.shape[0] < 1:
```

### Comparing `dramkit-0.5.39/dramkit/logtools/logger_general.py` & `dramkit-0.5.40/dramkit/logtools/logger_general.py`

 * *Files identical despite different names*

### Comparing `dramkit-0.5.39/dramkit/logtools/logger_rotating.py` & `dramkit-0.5.40/dramkit/logtools/logger_rotating.py`

 * *Files identical despite different names*

### Comparing `dramkit-0.5.39/dramkit/logtools/logger_timedrotating.py` & `dramkit-0.5.40/dramkit/logtools/logger_timedrotating.py`

 * *Files identical despite different names*

### Comparing `dramkit-0.5.39/dramkit/logtools/utils_logger.py` & `dramkit-0.5.40/dramkit/logtools/utils_logger.py`

 * *Files identical despite different names*

### Comparing `dramkit-0.5.39/dramkit/openai/aiedu_chat.py` & `dramkit-0.5.40/dramkit/openai/aiedu_chat.py`

 * *Files identical despite different names*

### Comparing `dramkit-0.5.39/dramkit/openai/openai_chat.py` & `dramkit-0.5.40/dramkit/openai/openai_chat.py`

 * *Files 1% similar despite different names*

```diff
@@ -17,15 +17,24 @@
 from dramkit.iotools import load_yml, get_parent_path, load_json, write_json, make_file_dir
 from dramkit.datetimetools import datetime_now
 from dramkit.cryptotools import en_aes_cbc, de_aes_cbc
 
 
 API_KEY = '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'
 
-QUIT_WORDS = ['quit', 'bye', 'good bye', 'goodbye', '拜拜', '再见']
+QUIT_WORDS = ['quit',
+              'exit',
+              'bye',
+              'good bye',
+              'goodbye',
+              '拜拜',
+              '再见',
+              '退出',
+              '结束',
+              '结束对话']
 N_TRY = 1 # 重试次数
 
 CON = True # 是否允许连续对话
 N_MAX_CON = 20 # 连续对话信息保留的最大轮数
 MAX_PROMPT_LEN = 1500
```

### Comparing `dramkit-0.5.39/dramkit/openai/openai_chat_hs.py` & `dramkit-0.5.40/dramkit/openai/openai_chat_hs.py`

 * *Files identical despite different names*

### Comparing `dramkit-0.5.39/dramkit/optimizer/alo.py` & `dramkit-0.5.40/dramkit/optimizer/alo.py`

 * *Files identical despite different names*

### Comparing `dramkit-0.5.39/dramkit/optimizer/base_funcs.py` & `dramkit-0.5.40/dramkit/optimizer/base_funcs.py`

 * *Files identical despite different names*

### Comparing `dramkit-0.5.39/dramkit/optimizer/boa.py` & `dramkit-0.5.40/dramkit/optimizer/boa.py`

 * *Files identical despite different names*

### Comparing `dramkit-0.5.39/dramkit/optimizer/cs.py` & `dramkit-0.5.40/dramkit/optimizer/cs.py`

 * *Files identical despite different names*

### Comparing `dramkit-0.5.39/dramkit/optimizer/ga.py` & `dramkit-0.5.40/dramkit/optimizer/ga.py`

 * *Files identical despite different names*

### Comparing `dramkit-0.5.39/dramkit/optimizer/gwo.py` & `dramkit-0.5.40/dramkit/optimizer/gwo.py`

 * *Files identical despite different names*

### Comparing `dramkit-0.5.39/dramkit/optimizer/hcpsoboa.py` & `dramkit-0.5.40/dramkit/optimizer/hcpsoboa.py`

 * *Files identical despite different names*

### Comparing `dramkit-0.5.39/dramkit/optimizer/hho.py` & `dramkit-0.5.40/dramkit/optimizer/hho.py`

 * *Files identical despite different names*

### Comparing `dramkit-0.5.39/dramkit/optimizer/hpsoboa.py` & `dramkit-0.5.40/dramkit/optimizer/hpsoboa.py`

 * *Files identical despite different names*

### Comparing `dramkit-0.5.39/dramkit/optimizer/pso.py` & `dramkit-0.5.40/dramkit/optimizer/pso.py`

 * *Files identical despite different names*

### Comparing `dramkit-0.5.39/dramkit/optimizer/utils_heuristic.py` & `dramkit-0.5.40/dramkit/optimizer/utils_heuristic.py`

 * *Files identical despite different names*

### Comparing `dramkit-0.5.39/dramkit/optimizer/woa.py` & `dramkit-0.5.40/dramkit/optimizer/woa.py`

 * *Files identical despite different names*

### Comparing `dramkit-0.5.39/dramkit/other/_Linux_notes.py` & `dramkit-0.5.40/dramkit/other/_Linux_notes.py`

 * *Files identical despite different names*

### Comparing `dramkit-0.5.39/dramkit/other/_Python_notes.py` & `dramkit-0.5.40/dramkit/other/_Python_notes.py`

 * *Files identical despite different names*

### Comparing `dramkit-0.5.39/dramkit/other/_Vim_notes.py` & `dramkit-0.5.40/dramkit/other/_Vim_notes.py`

 * *Files identical despite different names*

### Comparing `dramkit-0.5.39/dramkit/other/langconv.py` & `dramkit-0.5.40/dramkit/other/langconv.py`

 * *Files identical despite different names*

### Comparing `dramkit-0.5.39/dramkit/other/othertools.py` & `dramkit-0.5.40/dramkit/other/othertools.py`

 * *Files identical despite different names*

### Comparing `dramkit-0.5.39/dramkit/other/replace_endblank.py` & `dramkit-0.5.40/dramkit/other/replace_endblank.py`

 * *Files identical despite different names*

### Comparing `dramkit-0.5.39/dramkit/other/zh_wiki.py` & `dramkit-0.5.40/dramkit/other/zh_wiki.py`

 * *Files identical despite different names*

### Comparing `dramkit-0.5.39/dramkit/plottools/plot_barline.py` & `dramkit-0.5.40/dramkit/plottools/plot_barline.py`

 * *Files identical despite different names*

### Comparing `dramkit-0.5.39/dramkit/plottools/plot_common.py` & `dramkit-0.5.40/dramkit/plottools/plot_common.py`

 * *Files identical despite different names*

### Comparing `dramkit-0.5.39/dramkit/plottools/plot_histdist.py` & `dramkit-0.5.40/dramkit/plottools/plot_histdist.py`

 * *Files identical despite different names*

### Comparing `dramkit-0.5.39/dramkit/plottools/plot_scatter.py` & `dramkit-0.5.40/dramkit/plottools/plot_scatter.py`

 * *Files identical despite different names*

### Comparing `dramkit-0.5.39/dramkit/plottools/utils_plot.py` & `dramkit-0.5.40/dramkit/plottools/utils_plot.py`

 * *Files identical despite different names*

### Comparing `dramkit-0.5.39/dramkit/pystyles/dramkit_style.py` & `dramkit-0.5.40/dramkit/pystyles/dramkit_style.py`

 * *Files identical despite different names*

### Comparing `dramkit-0.5.39/dramkit/sorts/bubble_sort.py` & `dramkit-0.5.40/dramkit/sorts/bubble_sort.py`

 * *Files identical despite different names*

### Comparing `dramkit-0.5.39/dramkit/sorts/bucket_sort.py` & `dramkit-0.5.40/dramkit/sorts/bucket_sort.py`

 * *Files identical despite different names*

### Comparing `dramkit-0.5.39/dramkit/sorts/insert_sort.py` & `dramkit-0.5.40/dramkit/sorts/insert_sort.py`

 * *Files identical despite different names*

### Comparing `dramkit-0.5.39/dramkit/sorts/insert_sort_bin.py` & `dramkit-0.5.40/dramkit/sorts/insert_sort_bin.py`

 * *Files identical despite different names*

### Comparing `dramkit-0.5.39/dramkit/sorts/quick_sort.py` & `dramkit-0.5.40/dramkit/sorts/quick_sort.py`

 * *Files identical despite different names*

### Comparing `dramkit-0.5.39/dramkit/speedup/_mp_test1.py` & `dramkit-0.5.40/dramkit/speedup/_mp_test1.py`

 * *Files identical despite different names*

### Comparing `dramkit-0.5.39/dramkit/speedup/_mp_test2.py` & `dramkit-0.5.40/dramkit/speedup/_mp_test2.py`

 * *Files identical despite different names*

### Comparing `dramkit-0.5.39/dramkit/speedup/_mp_test3.py` & `dramkit-0.5.40/dramkit/speedup/_mp_test3.py`

 * *Files identical despite different names*

### Comparing `dramkit-0.5.39/dramkit/speedup/iotools_tmp.py` & `dramkit-0.5.40/dramkit/speedup/iotools_tmp.py`

 * *Files identical despite different names*

### Comparing `dramkit-0.5.39/dramkit/speedup/multi_process_concurrent.py` & `dramkit-0.5.40/dramkit/speedup/multi_process_concurrent.py`

 * *Files identical despite different names*

### Comparing `dramkit-0.5.39/dramkit/speedup/multi_thread.py` & `dramkit-0.5.40/dramkit/speedup/multi_thread.py`

 * *Files identical despite different names*

### Comparing `dramkit-0.5.39/dramkit/sqltools/_Hive_notes.py` & `dramkit-0.5.40/dramkit/sqltools/_Hive_notes.py`

 * *Files identical despite different names*

### Comparing `dramkit-0.5.39/dramkit/sqltools/_MySQL_notes.py` & `dramkit-0.5.40/dramkit/sqltools/_MySQL_notes.py`

 * *Files identical despite different names*

### Comparing `dramkit-0.5.39/dramkit/sqltools/_Oracle_notes.py` & `dramkit-0.5.40/dramkit/sqltools/_Oracle_notes.py`

 * *Files identical despite different names*

### Comparing `dramkit-0.5.39/dramkit/sqltools/cxoracle.py` & `dramkit-0.5.40/dramkit/sqltools/cxoracle.py`

 * *Files 3% similar despite different names*

```diff
@@ -49,14 +49,17 @@
     
     def get_fields(self, tb_name):
         return get_fields(self.conn, tb_name)
     
     def has_table(self, tb_name):
         return has_table(self.conn, tb_name)
     
+    def clear_data(self, tb_name):
+        return clear_data(self.conn, tb_name)
+    
     def drop_table(self, tb_name, purge=True):
         return drop_table(self.conn, tb_name, purge=purge)
     
     def get_create_table_sql(self, tb_name):
         return get_create_table_sql(self.conn, tb_name)
     
     def create_table(self, tb_name, cols_info,
@@ -149,14 +152,21 @@
                  WHERE table_name = UPPER('{}')
               '''.format(tb_name)
     fields_info = execute_sql(conn, sql_str, to_df=True)
     fields = fields_info['COLUMN_NAME'].tolist()
     return fields, fields_info
 
 
+def clear_data(conn, tb_name):
+    '''清空表中数据'''
+    sql = 'TRUNCATE TABLE {}'.format(tb_name)
+    # sql = 'DELETE FROM {}'.format(tb_name)
+    execute_sql(conn, sql, to_df=False)
+
+
 def has_table(conn, tb_name):
     sql = "SELECT COUNT(*) n FROM user_tables WHERE table_name=UPPER('{}')".format(tb_name)
     n = execute_sql(conn, sql, to_df=False)[0][0]
     if n > 0:
         return True
     return False
 
@@ -344,14 +354,15 @@
         cx_oracle.connect数据库连接对象
     tb_name : str
         存入的表名
     act_type : str
         | 存入方式：
         |     若为'ignore_tb'，则当表已经存在时不进行任何操作
         |     若为'new'，则新建表（若原表已存在，则会先删除再重建）
+        |     若为'clear'，则先清空已存在数据（若原表已存在）
         |     若为'insert'，则直接插入
         |     若为'replace'，则将已存在的数据更新，不存在的行和列都新插入
         |     若为'insert_ignore'，则已有的行不更新，不存在的行新插入
         |     若为'insert_newcols'（谨慎使用），则对已存在的列同直接insert（但是遇到已存在的行时不会报错，可能会丢失数据），有新列则插入新列内容
         |     若为'insert_ignore_newcols'，则对已存在的列同直接insert_ignore，有新列则插入新列内容
     cols : None, list
         需要存入的数据列
@@ -384,15 +395,15 @@
     ...                     'value': [66, 7, 8, 9],
     ...                     'VALUE2': [10, 11, 12, 13],
     ...                     'VALUE3': ['10a', '11b', 12, '13']})
     >>> df_to_sql(df, conn, tb_name, act_type='new', idcols=idcols)
     >>> df_to_sql(df1, conn, tb_name, act_type='replace', idcols=idcols)
     '''
     
-    assert act_type in ['ignore_tb', 'new', 'insert', 'insert_ignore', 'replace',
+    assert act_type in ['ignore_tb', 'new', 'clear', 'insert', 'insert_ignore', 'replace',
                         'insert_newcols', 'insert_ignore_newcols']
     if act_type == 'ignore_tb' and has_table(conn, tb_name):
         return
     
     # 待入库字段检查
     cols = check_list_arg(cols, allow_none=True)
     # 字段名称统一处理为大写
@@ -418,14 +429,18 @@
 
     cur_ = conn.cursor()
 
     cols_info, dtype, ph, cols_info_dict = get_cols_info_df(
         df, cols=cols, col_types=change_dict_key(col_types, lambda x: x.upper()),
         **kwargs_cols)
 
+    # 清空表
+    if act_type == 'clear':
+        if has_table(conn, tb_name):
+            clear_data(conn, tb_name)
     # 表不存在则新建
     idcols = check_list_arg(idcols, allow_none=True)
     idcols = [x.upper() for x in idcols] if not isnull(idcols) else idcols
     force = True if act_type == 'new' else False
     create_table(conn, tb_name, cols_info.split(', '),
                  idcols=idcols, force=force)
     
@@ -448,15 +463,15 @@
         raise ValueError('待存入数据中必须包含所有唯一值字段！')
         
     # TODO: idcols和idcols_即已有唯一索引字段不符合的情况处理
     assert list_eq(idcols, idcols_, order=False), '`idcols`必须和表唯一值索引相同'
     
     # 数据更新
     values = df.values.tolist()
-    if isnull(idcols) or act_type == 'new':        
+    if isnull(idcols) or act_type in ['new', 'clear']:        
         cur_.executemany('INSERT INTO {a} ({b}) VALUES ({c})'.format(
                              a=tb_name, b=','.join(cols), c=ph),
                          values)
     elif act_type == 'insert':
         # 批量插入新数据
         try:
             cur_.executemany('INSERT INTO {a} ({b}) VALUES ({c})'.format(
```

### Comparing `dramkit-0.5.39/dramkit/sqltools/py_hive.py` & `dramkit-0.5.40/dramkit/sqltools/py_hive.py`

 * *Files identical despite different names*

### Comparing `dramkit-0.5.39/dramkit/sqltools/py_mysql.py` & `dramkit-0.5.40/dramkit/sqltools/py_mysql.py`

 * *Files 1% similar despite different names*

```diff
@@ -242,17 +242,18 @@
         res = copy(self)
         conn_args = self.__db_conn_args.copy()
         conn_args.update({'client_flag': CLIENT.MULTI_STATEMENTS})
         res.conn = get_conn(**conn_args)
         return res
     
     def has_table(self, tb_name, db_name=None):
-        tbs = self.show_tables(db_name=db_name)
-        return tb_name.lower() in [x.lower() for x in tbs]
-        
+        # tbs = self.show_tables(db_name=db_name)
+        # return tb_name.lower() in [x.lower() for x in tbs]
+        return self.execute_sql('SHOW TABLES LIKE "{}"'.format(tb_name), db_name=db_name).shape[0] > 0
+
         
 def _check_list_arg(arg, allow_none=True):
     if allow_none:
         assert isinstance(arg, (type(None), str, list, tuple))
     else:
         assert isinstance(arg, (str, list, tuple))
     if isinstance(arg, str):
@@ -289,16 +290,17 @@
         res = pd.DataFrame(res, columns=cols)
     cur.close()
     conn.commit()
     return res
 
 
 def has_table(conn, tb_name, db_name=None):
-    tbs = show_tables(conn, db_name=db_name)
-    return tb_name.lower() in [x.lower() for x in tbs]
+    # tbs = show_tables(conn, db_name=db_name)
+    # return tb_name.lower() in [x.lower() for x in tbs]
+    return execute_sql(conn, 'SHOW TABLES LIKE "{}"'.format(tb_name), db_name=db_name).shape[0] > 0
 
 
 def get_fields(conn, tb_name, db_name=None):
     '''获取表字段名列表'''
     sql_str = 'DESC {};'.format(tb_name)
     fields_info = execute_sql(conn, sql_str,
                               db_name=db_name, to_df=True)
@@ -824,14 +826,15 @@
         pymysql.connect数据库连接对象
     tb_name : str
         存入的表名
     act_type : str
         | 存入方式：
         |     若为'ignore_tb'，则当表已经存在时不进行任何操作
         |     若为'new'，则新建表（若原表已存在，则会先删除再重建）
+        |     若为'clear'，则先清空原表数据（若原表已存在）
         |     若为'insert'，则直接插入
         |     若为'replace'，则将已存在的数据更新，不存在的行和列都新插入
         |     若为'insert_ignore'，则已有的行不更新，不存在的行新插入
         |     若为'insert_newcols'（谨慎使用），则对已存在的列同直接insert（但是遇到已存在的行时不会报错，可能会丢失数据），有新列则插入新列内容
         |     若为'insert_ignore_newcols'，则对已存在的列同直接insert_ignore，有新列则插入新列内容
     cols : None, list
         需要存入的数据列
@@ -932,15 +935,15 @@
         return
     
     idcols = _check_list_arg(idcols)
     if isnull(idcols):
         act_type = 'insert' if act_type != 'new' else 'new'
     
     # 清除原数据或直接新增数据
-    if act_type in ['new', 'insert', 'insert_ignore']:
+    if act_type in ['new', 'clear', 'insert', 'insert_ignore']:
         df_to_sql_by_row(df, conn, tb_name, act_type=act_type,
                          db_name=db_name, cols=cols, idcols=idcols,
                          col_types=col_types, na_val=na_val,
                          inf_val=inf_val, _inf_val=_inf_val,
                          logger=logger, **kwargs_cols)
         return
     
@@ -1068,15 +1071,15 @@
     Note
     ----
     判断数据是否存在时是根据主键或唯一索引来的，
     因此当待插入数据字段只是已存在数据字段的一部分时，
     此函数应慎用'replace'（可能导致原有数据变成Null）
     '''
     
-    assert act_type in ['ignore_tb', 'new', 'insert', 'replace', 'insert_ignore']
+    assert act_type in ['ignore_tb', 'new', 'clear', 'insert', 'replace', 'insert_ignore']
     if act_type == 'ignore_tb' and has_table(conn, tb_name, db_name=db_name):
         return
     
     # 待入库字段检查
     cols = _check_list_arg(cols)
     # 字段名称统一处理为大写
     df = df.rename(columns={x: x.upper() for x in df.columns})
@@ -1101,14 +1104,20 @@
         cur.execute('CREATE DATABASE IF NOT EXISTS {};'.format(db_name))
         cur.execute('USE {};'.format(db_name))
 
     cols_info, dtype, ph, cols_info_dict = get_cols_info_df(
         df, cols=cols, col_types=change_dict_key(col_types, lambda x: x.upper()),
         **kwargs_cols)
 
+    # 清空表
+    if act_type == 'clear':
+        n = cur.execute('SHOW TABLES LIKE "{}";'.format(tb_name))
+        if n > 0:
+            cur.execute('TRUNCATE TABLE {};'.format(tb_name))
+            # cur.execute('DELETE FROM {};'.format(tb_name))
     # 表不存在则新建
     if act_type == 'new':
         cur.execute('DROP TABLE IF EXISTS {};'.format(tb_name))
     idcols = _check_list_arg(idcols)
     if isnull(idcols):
         cur.execute('CREATE TABLE IF NOT EXISTS {a}({b});'.format(
                      a=tb_name, b=cols_info))
@@ -1135,15 +1144,15 @@
         cur.execute('ALTER TABLE {} ADD {};'.format(
             tb_name, cols_info_dict[col][0]))
     # 所有字段
     all_fields = list(set(fields + cols_loss))
     
     # 数据更新
     values = df.values.tolist()
-    if act_type == 'new' or isnull(idcols):
+    if act_type in ['new', 'clear'] or isnull(idcols):
         cur.executemany('INSERT INTO {a} ({b}) VALUES ({c});'.format(
                         a=tb_name, b=','.join(cols), c=ph),
                         values)
     elif act_type == 'insert':
         # 批量插入新数据
         try:
             cur.executemany('INSERT INTO {a} ({b}) VALUES ({c});'.format(
```

### Comparing `dramkit-0.5.39/dramkit/sqltools/sql_alchemy.py` & `dramkit-0.5.40/dramkit/sqltools/sql_alchemy.py`

 * *Files identical despite different names*

### Comparing `dramkit-0.5.39/dramkit/webtools/utils_html.py` & `dramkit-0.5.40/dramkit/webtools/utils_html.py`

 * *Files identical despite different names*

### Comparing `dramkit-0.5.39/dramkit/wechat/qywechat.py` & `dramkit-0.5.40/dramkit/wechat/qywechat.py`

 * *Files identical despite different names*

### Comparing `dramkit-0.5.39/dramkit.egg-info/PKG-INFO` & `dramkit-0.5.40/dramkit.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dramkit
-Version: 0.5.39
+Version: 0.5.40
 Summary: DramKit is a toolbox.
 Home-page: https://github.com/Genlovy-Hoo/dramkit/
 Author: Genlovy Hoo, YueYong Hu
 Author-email: genlovhyy@163.com
 License: MIT
 Platform: any
 Description-Content-Type: text/markdown
```

### Comparing `dramkit-0.5.39/dramkit.egg-info/SOURCES.txt` & `dramkit-0.5.40/dramkit.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -90,14 +90,15 @@
 dramkit/datsci/lr.py
 dramkit/datsci/preprocess.py
 dramkit/datsci/stats.py
 dramkit/datsci/time_series.py
 dramkit/datsci/topsis.py
 dramkit/datsci/utils_lgb.py
 dramkit/datsci/utils_ml.py
+dramkit/datsci/zigzag.py
 dramkit/find_addends/__init__.py
 dramkit/find_addends/find_addends_backpack01float.py
 dramkit/find_addends/find_addends_backpack01int.py
 dramkit/find_addends/find_addends_bigfirst.py
 dramkit/find_addends/find_addends_recu.py
 dramkit/find_addends/find_addends_smlfirst.py
 dramkit/find_addends/find_addends_utils.py
```

### Comparing `dramkit-0.5.39/setup.py` & `dramkit-0.5.40/setup.py`

 * *Files identical despite different names*

