# Comparing `tmp/ccsmeth-0.3.2.tar.gz` & `tmp/ccsmeth-0.3.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\ccsmeth-0.3.2.tar", last modified: Sun Sep 18 04:27:53 2022, max compression
+gzip compressed data, was "ccsmeth-0.3.3.tar", last modified: Mon May 15 11:32:43 2023, max compression
```

## Comparing `ccsmeth-0.3.2.tar` & `ccsmeth-0.3.3.tar`

### file list

```diff
@@ -1,40 +1,40 @@
-drwxrwxrwx   0        0        0        0 2022-09-18 04:27:53.000000 ccsmeth-0.3.2/
-drwxrwxrwx   0        0        0        0 2022-09-18 04:27:52.000000 ccsmeth-0.3.2/ccsmeth/
--rw-rw-rw-   0        0        0     9878 2022-09-12 06:23:49.000000 ccsmeth-0.3.2/ccsmeth/align_hifi_reads.py
--rw-rw-rw-   0        0        0     6040 2022-05-16 12:12:40.000000 ccsmeth-0.3.2/ccsmeth/call_hifi_reads.py
--rw-rw-rw-   0        0        0    30710 2022-09-10 15:59:27.000000 ccsmeth-0.3.2/ccsmeth/call_modifications.py
--rw-rw-rw-   0        0        0    32505 2022-09-18 04:23:06.000000 ccsmeth-0.3.2/ccsmeth/call_mods_freq_bam.py
--rw-rw-rw-   0        0        0    18444 2022-05-21 04:54:47.000000 ccsmeth-0.3.2/ccsmeth/call_mods_freq_txt.py
--rw-rw-rw-   0        0        0    54222 2022-09-18 04:23:06.000000 ccsmeth-0.3.2/ccsmeth/ccsmeth.py
--rw-rw-rw-   0        0        0     6908 2022-08-10 13:49:55.000000 ccsmeth-0.3.2/ccsmeth/dataloader.py
--rw-rw-rw-   0        0        0    31821 2022-08-10 11:33:05.000000 ccsmeth-0.3.2/ccsmeth/extract_features.py
--rw-rw-rw-   0        0        0     9782 2022-08-13 03:00:19.000000 ccsmeth-0.3.2/ccsmeth/models.py
--rw-rw-rw-   0        0        0    20305 2022-09-12 09:08:43.000000 ccsmeth-0.3.2/ccsmeth/train.py
--rw-rw-rw-   0        0        0    25192 2022-09-14 10:03:55.000000 ccsmeth-0.3.2/ccsmeth/train_multigpu.py
-drwxrwxrwx   0        0        0        0 2022-09-18 04:27:53.000000 ccsmeth-0.3.2/ccsmeth/utils/
--rw-rw-rw-   0        0        0     2801 2022-05-21 04:53:43.000000 ccsmeth-0.3.2/ccsmeth/utils/attention.py
--rw-rw-rw-   0        0        0      756 2022-08-11 09:36:05.000000 ccsmeth-0.3.2/ccsmeth/utils/constants_torch.py
--rw-rw-rw-   0        0        0     4077 2022-09-12 02:39:09.000000 ccsmeth-0.3.2/ccsmeth/utils/lookahead.py
--rw-rw-rw-   0        0        0    13974 2022-06-26 14:57:09.000000 ccsmeth-0.3.2/ccsmeth/utils/process_utils.py
--rw-rw-rw-   0        0        0     9051 2022-05-16 12:12:41.000000 ccsmeth-0.3.2/ccsmeth/utils/ranger2020.py
--rw-rw-rw-   0        0        0     2789 2022-05-16 12:12:41.000000 ccsmeth-0.3.2/ccsmeth/utils/ref_reader.py
--rw-rw-rw-   0        0        0      963 2022-05-16 12:12:41.000000 ccsmeth-0.3.2/ccsmeth/utils/sam2fastq_std.py
--rw-rw-rw-   0        0        0        0 2022-05-21 04:53:39.000000 ccsmeth-0.3.2/ccsmeth/utils/__init__.py
--rw-rw-rw-   0        0        0    15200 2022-09-14 12:58:07.000000 ccsmeth-0.3.2/ccsmeth/_bam2modbam.py
--rw-rw-rw-   0        0        0       18 2022-09-18 03:35:42.000000 ccsmeth-0.3.2/ccsmeth/_version.py
--rw-rw-rw-   0        0        0        0 2022-05-16 12:12:40.000000 ccsmeth-0.3.2/ccsmeth/__init__.py
-drwxrwxrwx   0        0        0        0 2022-09-18 04:27:53.000000 ccsmeth-0.3.2/ccsmeth.egg-info/
--rw-rw-rw-   0        0        0        1 2022-09-18 04:27:51.000000 ccsmeth-0.3.2/ccsmeth.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       50 2022-09-18 04:27:51.000000 ccsmeth-0.3.2/ccsmeth.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0        2 2022-09-18 04:27:51.000000 ccsmeth-0.3.2/ccsmeth.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0     2679 2022-09-18 04:27:51.000000 ccsmeth-0.3.2/ccsmeth.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      134 2022-09-18 04:27:51.000000 ccsmeth-0.3.2/ccsmeth.egg-info/requires.txt
--rw-rw-rw-   0        0        0      853 2022-09-18 04:27:52.000000 ccsmeth-0.3.2/ccsmeth.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        8 2022-09-18 04:27:51.000000 ccsmeth-0.3.2/ccsmeth.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1683 2022-05-21 04:55:01.000000 ccsmeth-0.3.2/LICENSE
--rw-rw-rw-   0        0        0       84 2022-08-16 11:17:57.000000 ccsmeth-0.3.2/MANIFEST.in
--rw-rw-rw-   0        0        0     2679 2022-09-18 04:27:53.000000 ccsmeth-0.3.2/PKG-INFO
--rw-rw-rw-   0        0        0     1240 2022-09-18 04:27:37.000000 ccsmeth-0.3.2/README.rst
--rw-rw-rw-   0        0        0      152 2022-08-11 07:52:06.000000 ccsmeth-0.3.2/requirements.txt
--rw-rw-rw-   0        0        0       86 2022-09-18 04:27:53.000000 ccsmeth-0.3.2/setup.cfg
--rw-rw-rw-   0        0        0     2017 2022-06-28 01:35:02.000000 ccsmeth-0.3.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-15 11:32:43.705074 ccsmeth-0.3.3/
+-rw-rw-rw-   0        0        0     1683 2023-03-22 03:41:13.000000 ccsmeth-0.3.3/LICENSE
+-rw-rw-rw-   0        0        0       84 2023-03-22 03:41:13.000000 ccsmeth-0.3.3/MANIFEST.in
+-rw-rw-rw-   0        0        0     2219 2023-05-15 11:32:43.705074 ccsmeth-0.3.3/PKG-INFO
+-rw-rw-rw-   0        0        0     1418 2023-05-10 16:47:48.000000 ccsmeth-0.3.3/README.rst
+drwxrwxrwx   0        0        0        0 2023-05-15 11:32:43.481213 ccsmeth-0.3.3/ccsmeth/
+-rw-rw-rw-   0        0        0        0 2022-05-16 12:12:40.000000 ccsmeth-0.3.3/ccsmeth/__init__.py
+-rw-rw-rw-   0        0        0    15200 2023-03-22 03:41:13.000000 ccsmeth-0.3.3/ccsmeth/_bam2modbam.py
+-rw-rw-rw-   0        0        0       18 2023-05-15 09:50:50.000000 ccsmeth-0.3.3/ccsmeth/_version.py
+-rw-rw-rw-   0        0        0     9878 2023-03-22 03:41:13.000000 ccsmeth-0.3.3/ccsmeth/align_hifi_reads.py
+-rw-rw-rw-   0        0        0     6040 2023-03-22 03:41:13.000000 ccsmeth-0.3.3/ccsmeth/call_hifi_reads.py
+-rw-rw-rw-   0        0        0    30718 2023-05-09 07:02:54.000000 ccsmeth-0.3.3/ccsmeth/call_modifications.py
+-rw-rw-rw-   0        0        0    37939 2023-05-09 07:03:05.000000 ccsmeth-0.3.3/ccsmeth/call_mods_freq_bam.py
+-rw-rw-rw-   0        0        0    18444 2023-03-22 03:41:14.000000 ccsmeth-0.3.3/ccsmeth/call_mods_freq_txt.py
+-rw-rw-rw-   0        0        0    54823 2023-05-09 07:02:13.000000 ccsmeth-0.3.3/ccsmeth/ccsmeth.py
+-rw-rw-rw-   0        0        0     6908 2023-03-22 03:41:14.000000 ccsmeth-0.3.3/ccsmeth/dataloader.py
+-rw-rw-rw-   0        0        0    31829 2023-05-09 07:02:43.000000 ccsmeth-0.3.3/ccsmeth/extract_features.py
+-rw-rw-rw-   0        0        0    10097 2023-04-26 02:27:23.000000 ccsmeth-0.3.3/ccsmeth/models.py
+-rw-rw-rw-   0        0        0    20305 2023-03-22 03:41:14.000000 ccsmeth-0.3.3/ccsmeth/train.py
+-rw-rw-rw-   0        0        0    25193 2023-04-23 13:09:00.000000 ccsmeth-0.3.3/ccsmeth/train_multigpu.py
+drwxrwxrwx   0        0        0        0 2023-05-15 11:32:43.690083 ccsmeth-0.3.3/ccsmeth/utils/
+-rw-rw-rw-   0        0        0        0 2022-05-21 04:53:39.000000 ccsmeth-0.3.3/ccsmeth/utils/__init__.py
+-rw-rw-rw-   0        0        0     2801 2023-03-22 03:41:14.000000 ccsmeth-0.3.3/ccsmeth/utils/attention.py
+-rw-rw-rw-   0        0        0      756 2023-03-22 03:41:14.000000 ccsmeth-0.3.3/ccsmeth/utils/constants_torch.py
+-rw-rw-rw-   0        0        0     4077 2023-03-22 03:41:14.000000 ccsmeth-0.3.3/ccsmeth/utils/lookahead.py
+-rw-rw-rw-   0        0        0    13974 2023-03-22 03:41:15.000000 ccsmeth-0.3.3/ccsmeth/utils/process_utils.py
+-rw-rw-rw-   0        0        0     9051 2022-05-16 12:12:41.000000 ccsmeth-0.3.3/ccsmeth/utils/ranger2020.py
+-rw-rw-rw-   0        0        0     2789 2022-05-16 12:12:41.000000 ccsmeth-0.3.3/ccsmeth/utils/ref_reader.py
+-rw-rw-rw-   0        0        0      963 2023-03-22 03:41:15.000000 ccsmeth-0.3.3/ccsmeth/utils/sam2fastq_std.py
+drwxrwxrwx   0        0        0        0 2023-05-15 11:32:43.592144 ccsmeth-0.3.3/ccsmeth.egg-info/
+-rw-rw-rw-   0        0        0     2219 2023-05-15 11:32:42.000000 ccsmeth-0.3.3/ccsmeth.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      853 2023-05-15 11:32:43.000000 ccsmeth-0.3.3/ccsmeth.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-15 11:32:42.000000 ccsmeth-0.3.3/ccsmeth.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       49 2023-05-15 11:32:42.000000 ccsmeth-0.3.3/ccsmeth.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0        2 2023-05-15 11:32:42.000000 ccsmeth-0.3.3/ccsmeth.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0      134 2023-05-15 11:32:42.000000 ccsmeth-0.3.3/ccsmeth.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2023-05-15 11:32:42.000000 ccsmeth-0.3.3/ccsmeth.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      152 2023-03-22 03:41:16.000000 ccsmeth-0.3.3/requirements.txt
+-rw-rw-rw-   0        0        0       86 2023-05-15 11:32:43.718069 ccsmeth-0.3.3/setup.cfg
+-rw-rw-rw-   0        0        0     2017 2023-03-22 03:41:17.000000 ccsmeth-0.3.3/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `ccsmeth-0.3.2/ccsmeth/align_hifi_reads.py` & `ccsmeth-0.3.3/ccsmeth/align_hifi_reads.py`

 * *Files identical despite different names*

### Comparing `ccsmeth-0.3.2/ccsmeth/call_hifi_reads.py` & `ccsmeth-0.3.3/ccsmeth/call_hifi_reads.py`

 * *Files identical despite different names*

### Comparing `ccsmeth-0.3.2/ccsmeth/call_modifications.py` & `ccsmeth-0.3.3/ccsmeth/call_modifications.py`

 * *Files 2% similar despite different names*

```diff
@@ -669,18 +669,18 @@
     p_extract.add_argument("--loginfo", type=str, default="no", required=False,
                            help="if printing more info of feature extraction on reads. "
                                 "yes or no, default no")
 
     p_extract_ref = parser.add_argument_group("EXTRACTION ALIGN_MODE")
     p_extract_ref.add_argument("--ref", type=str, required=False,
                                help="path to genome reference to be aligned, in fasta/fa format.")
-    p_extract_ref.add_argument("--mapq", type=int, default=10, required=False,
-                               help="MAPping Quality cutoff for selecting alignment items, default 10")
-    p_extract_ref.add_argument("--identity", type=float, default=0.70, required=False,
-                               help="identity cutoff for selecting alignment items, default 0.70")
+    p_extract_ref.add_argument("--mapq", type=int, default=1, required=False,
+                               help="MAPping Quality cutoff for selecting alignment items, default 1")
+    p_extract_ref.add_argument("--identity", type=float, default=0.0, required=False,
+                               help="identity cutoff for selecting alignment items, [0.0, 1.0], default 0.0")
     p_extract_ref.add_argument("--no_supplementary", action="store_true", default=False, required=False,
                                help="not use supplementary alignment")
     p_extract_ref.add_argument("--is_mapfea", type=str, default="no", required=False,
                                help="if extract mapping features, yes or no, default no")
     p_extract_ref.add_argument("--skip_unmapped", type=str, default="yes", required=False,
                                help="if skipping unmapped sites in reads, yes or no, default yes")
```

### Comparing `ccsmeth-0.3.2/ccsmeth/call_mods_freq_bam.py` & `ccsmeth-0.3.3/ccsmeth/call_mods_freq_bam.py`

 * *Files 13% similar despite different names*

```diff
@@ -12,14 +12,15 @@
 import numpy as np
 
 import multiprocessing as mp
 from multiprocessing import Queue
 from tqdm import tqdm
 import pysam
 import pybedtools
+import re
 
 from .utils.ref_reader import DNAReference
 from .utils.process_utils import compute_pct_identity
 from .utils.process_utils import is_file_empty
 from .utils.process_utils import index_bam_if_needed2
 from .utils.process_utils import get_motif_seqs
 from .utils.process_utils import complement_seq
@@ -96,61 +97,125 @@
 
 
 def _cal_mod_prob(ml_value):
     # WARN: if ori_prob exactly = 0.5, ml_value = floor(0.5*256) = 128
     # WARN: then if we use the following to convert ml_value to prob, the the new_prob = 0.5000001.
     # WARN: if we use the rule: label = 1 if prob>0.5 else 0, then the label of new_prob will be
     # WARN: different with the label of ori_prob
-    return round(ml_value / float(256) + 0.000001, 6)
+    return round(ml_value / float(256) + 0.000001, 6) if ml_value > 0 else 0
+
+
+# refer from PacBio https://github.com/PacificBiosciences/pb-CpG-tools under BSD 3-Clause Clear License
+def _get_mm_position_iters(mm_idxs):
+    base_count = 0
+    # base_counts = []
+    for idx in mm_idxs:
+        base_count += idx + 1
+        yield base_count
+        # base_counts.append(base_count)
+    # return base_counts
+
+
+# refer from PacBio https://github.com/PacificBiosciences/pb-CpG-tools under BSD 3-Clause Clear License
+def _get_all_modbase_positions(fwd_seq, modbase):
+    return [i.start() for i in re.finditer(modbase, fwd_seq)]
+
+
+def _get_moddict_in_tags(readitem, modbase="C", modification="m"):
+    mmtag, mltag = None, None
+    try:
+        mmtag = readitem.get_tag('MM')
+        mltag = readitem.get_tag('ML')
+    except KeyError:
+        pass
+    if mmtag is None or mltag is None:
+        return {}
+    else:
+        seq_fwdseq = readitem.get_forward_sequence()
+        seq_len = len(seq_fwdseq)
+        is_reverse = readitem.is_reverse
+
+        # parse MM/ML tags
+        mod_iters = None
+        for x in mmtag.split(';'):
+            if x.startswith(modbase + "+" + modification):
+                start_index = len(modbase) + 1 + len(modification)
+                if len(x) > start_index and x[start_index] in "?.":
+                    start_index += 1
+                if len(x) > start_index and x[start_index] == ",":
+                    start_index += 1
+                    mod_iters = _get_mm_position_iters([int(y) for y in x[start_index:].split(",")])
+                break
+        if mod_iters is None:
+            return {}
+        modbases_all = _get_all_modbase_positions(seq_fwdseq, modbase)
+        try:
+            modbases = [modbases_all[idx - 1] for idx in mod_iters]
+            assert len(modbases) == len(mltag)
+            moddict = dict()
+            for idx in range(len(modbases)):
+                mod_pos = modbases[idx]
+                if is_reverse:
+                    mod_pos = seq_len - 1 - mod_pos
+                moddict[mod_pos] = _cal_mod_prob(mltag[idx])
+            return moddict
+        except IndexError:
+            sys.stderr.write("[WARN] read {}: MM tag length does not match length of modbases "
+                             "in read!\n".format(readitem.query_name))
+            return {}
+        except AssertionError:
+            sys.stderr.write("[WARN] read {}: MM tag length != ML tag length!\n".format(readitem.query_name))
+            return {}
 
 
 def _get_moddict(readitem, modbase="C", modification="m"):
     """
 
     :param readitem:
     :return: moddict: query_pos(in alignment strand) 2 mod_probs([0,1])
     """
-    # mmtag, mltag = None, None
-    # try:
-    #     mmtag = readitem.get_tag('MM')
-    #     mltag = readitem.get_tag('ML')
-    #     seq_fwdseq = readitem.get_forward_sequence()
-    #     is_reverse = readitem.is_reverse
-    # except KeyError:
-    #     pass
-    # if mmtag is None or mltag is None:
-    #     return {}
 
-    # use .modified_bases instead of MM/ML tags to get moddict
+    # first try to use .modified_bases (pysam>=0.19.0) instead of MM/ML tags to get moddict
     modinfo = readitem.modified_bases
-    if modinfo is None:
-        return {}
-    modtuple = None
-    for modkey in modinfo.keys():
-        if modkey[0] == modbase and modkey[2] == modification:
-            modtuple = modinfo[modkey]
-            break
-    if modtuple is None:
-        return {}
-    moddict = dict(modtuple)
-    for modloc in moddict.keys():
-        moddict[modloc] = _cal_mod_prob(moddict[modloc])
-    return moddict
+    if not (modinfo is None or len(modinfo) == 0):
+        modtuple = None
+        for modkey in modinfo.keys():
+            if modkey[0] == modbase and modkey[2] == modification:
+                modtuple = modinfo[modkey]
+                break
+        if modtuple is None:
+            return {}
+        moddict = dict(modtuple)
+        for modloc in moddict.keys():
+            moddict[modloc] = _cal_mod_prob(moddict[modloc])
+        return moddict
+    else:
+        # case 1: the MM tag is "MM:Z:C+m?,..."?
+        # case 2: there are no MM/ML tags
+        return _get_moddict_in_tags(readitem, modbase, modification)
 
 
-def _cal_modfreq_in_count_mode(modprobs, prob_cf=0):
-    cnt_all, cnt_mod = 0, 0
+def _cal_modfreq_in_count_mode(modprobs, prob_cf=0, no_amb_cov=False):
+    cnt_all_filtered, cnt_mod = 0, 0
     for modprob in modprobs:
         if abs(modprob - (1 - modprob)) < prob_cf:
             continue
-        cnt_all += 1
+        cnt_all_filtered += 1
         if modprob > 0.5:
             cnt_mod += 1
-    modfreq = cnt_mod / float(cnt_all) if cnt_all > 0 else 0.
-    return cnt_all, cnt_mod, modfreq
+    modfreq = cnt_mod / float(cnt_all_filtered) if cnt_all_filtered > 0 else 0.
+    if no_amb_cov:
+        return cnt_all_filtered, cnt_mod, modfreq
+    else:
+        # WARN -- when prob_cf>0, cnt_mod/modfreq does not always equal len(modprobs)
+        # So:
+        if cnt_all_filtered != len(modprobs):
+            # adjust cnt_mod
+            cnt_mod = np.round(len(modprobs) * modfreq, 2)
+        return len(modprobs), cnt_mod, modfreq
 
 
 # from PacBio https://github.com/PacificBiosciences/pb-CpG-tools under BSD 3-Clause Clear License
 def _get_normalized_histo(probs, cov_cf=4, binsize=20):
     """
     Create the array data structure needed to apply the model, for a given site.
 
@@ -165,34 +230,67 @@
 
     hist = np.histogram(probs, bins=binsize, range=[0, 1])[0]
     norm = np.linalg.norm(hist)
     # divide hist by norm and add values to arr
     return np.round(hist / norm, 6)
 
 
-def _cal_modfreq_in_aggregate_mode(refposes, refposes_histos, model, seq_len=11):
+# try discretizing, similar idea from PacBio https://github.com/PacificBiosciences/pb-CpG-tools
+# under BSD 3-Clause Clear License
+def discretize_score(modprob, coverage):
+    """
+
+    """
+    # need to round up or round down modified read numbers based on score
+    # which allows a push towards 0/100 for adjusted score
+    if modprob > 0.66:
+        mod_reads = int(np.ceil(modprob * float(coverage)))
+    elif modprob <= 0.33:
+        mod_reads = int(np.floor(modprob * float(coverage)))
+    else:
+        mod_reads = round(coverage * modprob, 2)
+
+    unmod_reads = int(coverage) - mod_reads
+
+    if mod_reads == 0:
+        adjusted_score = 0.0
+    else:
+        adjusted_score = float(mod_reads) / (mod_reads + unmod_reads)
+
+    return mod_reads, unmod_reads, adjusted_score
+
+
+def _cal_modfreq_in_aggregate_mode(refposes, refposes_histos, model, seq_len=11, only_close=False):
 
     if len(refposes) == 0:
         return None
 
     from .utils.constants_torch import FloatTensor_cpu
 
     pad_len = seq_len // 2
     histos_mat = np.pad(np.stack(refposes_histos),
                         pad_width=((pad_len, pad_len), (0, 0)),
                         mode='constant', constant_values=0)
     histos_mat = np.swapaxes(sliding_window_view(histos_mat, seq_len, axis=0), 1, 2)
-    pos_mat = np.pad(refposes, pad_width=(pad_len, pad_len),
-                     mode='constant', constant_values=(refposes[0]-1000, refposes[-1]+1000))
-    pos_mat = sliding_window_view(pos_mat, seq_len)
-    pos_mat_center = np.repeat(refposes, seq_len).reshape((-1, seq_len))
-    pos_mat = np.absolute(np.subtract(pos_mat, pos_mat_center))
-    # no log2 is a litter better?
-    # pos_mat = np.round(1. / (np.log2(np.absolute(pos_mat) + 1) + 1), 6)
-    del pos_mat_center
+
+    if not only_close:
+        pos_mat = np.pad(refposes, pad_width=(pad_len, pad_len),
+                         mode='constant', constant_values=(refposes[0] - 1000, refposes[-1] + 1000))
+        pos_mat = sliding_window_view(pos_mat, seq_len)
+        pos_mat_center = np.repeat(refposes, seq_len).reshape((-1, seq_len))
+        pos_mat = np.absolute(np.subtract(pos_mat, pos_mat_center))
+        # no log2 is a litter better?
+        # pos_mat = np.round(1. / (np.log2(np.absolute(pos_mat) + 1) + 1), 6)
+        del pos_mat_center
+    else:
+        pos_mat = np.pad(refposes, pad_width=(pad_len + 1, pad_len),
+                         mode='constant', constant_values=(refposes[0] - 1000, refposes[-1] + 1000))
+        pos_mat = np.diff(pos_mat)
+        pos_mat = (pos_mat == 2).astype(int)
+        pos_mat = sliding_window_view(pos_mat, seq_len)
 
     probs = []
     batch_size = 1024
     for i in np.arange(0, len(histos_mat), batch_size):
         batch_s, batch_e = i, i + batch_size
         b_histos = np.array(histos_mat[batch_s:batch_e].copy())
         b_pos = np.array(pos_mat[batch_s:batch_e])
@@ -262,56 +360,68 @@
         if len(total_mods) > 0:
             if len(total_mods) >= args.cov_cf:
                 all_highcov_pos.append(refpos)
                 all_highcov_histos.append(_get_normalized_histo(total_mods, args.cov_cf, args.bin_size))
                 all_highcov_covs.append(len(total_mods))
             else:
                 all_lowcov_pos.append(refpos)
-                all_lowcov_mods.append(_cal_modfreq_in_count_mode(total_mods, args.prob_cf))
+                all_lowcov_mods.append(_cal_modfreq_in_count_mode(total_mods, args.prob_cf, args.no_amb_cov))
         if len(hp1_mods) > 0:
             if len(hp1_mods) >= args.cov_cf:
                 hp1_highcov_pos.append(refpos)
                 hp1_highcov_histos.append(_get_normalized_histo(hp1_mods, args.cov_cf, args.bin_size))
                 hp1_highcov_covs.append(len(hp1_mods))
             else:
                 hp1_lowcov_pos.append(refpos)
-                hp1_lowcov_mods.append(_cal_modfreq_in_count_mode(hp1_mods, args.prob_cf))
+                hp1_lowcov_mods.append(_cal_modfreq_in_count_mode(hp1_mods, args.prob_cf, args.no_amb_cov))
         if len(hp2_mods) > 0:
             if len(hp2_mods) >= args.cov_cf:
                 hp2_highcov_pos.append(refpos)
                 hp2_highcov_histos.append(_get_normalized_histo(hp2_mods, args.cov_cf, args.bin_size))
                 hp2_highcov_covs.append(len(hp2_mods))
             else:
                 hp2_lowcov_pos.append(refpos)
-                hp2_lowcov_mods.append(_cal_modfreq_in_count_mode(hp2_mods, args.prob_cf))
+                hp2_lowcov_mods.append(_cal_modfreq_in_count_mode(hp2_mods, args.prob_cf, args.no_amb_cov))
     for lowcov_idx in range(len(all_lowcov_pos)):
         refpos2result[all_lowcov_pos[lowcov_idx]][0] = all_lowcov_mods[lowcov_idx]
     for lowcov_idx in range(len(hp1_lowcov_pos)):
         refpos2result[hp1_lowcov_pos[lowcov_idx]][1] = hp1_lowcov_mods[lowcov_idx]
     for lowcov_idx in range(len(hp2_lowcov_pos)):
         refpos2result[hp2_lowcov_pos[lowcov_idx]][2] = hp2_lowcov_mods[lowcov_idx]
 
-    probs = _cal_modfreq_in_aggregate_mode(all_highcov_pos, all_highcov_histos, model, args.seq_len)
+    probs = _cal_modfreq_in_aggregate_mode(all_highcov_pos, all_highcov_histos, model, args.seq_len, args.only_close)
     for highcov_idx in range(len(all_highcov_pos)):
         modprob_tmp = probs[highcov_idx]
         cov_tmp = all_highcov_covs[highcov_idx]
-        cnt_mod = round(cov_tmp * modprob_tmp, 2)
-        refpos2result[all_highcov_pos[highcov_idx]][0] = (cov_tmp, cnt_mod, modprob_tmp)
-    probs = _cal_modfreq_in_aggregate_mode(hp1_highcov_pos, hp1_highcov_histos, model, args.seq_len)
+        if args.discrete:
+            d_cnt_mod, _, d_modprob_tmp = discretize_score(modprob_tmp, cov_tmp)
+            refpos2result[all_highcov_pos[highcov_idx]][0] = (cov_tmp, d_cnt_mod, d_modprob_tmp)
+        else:
+            cnt_mod = round(cov_tmp * modprob_tmp, 2)
+            refpos2result[all_highcov_pos[highcov_idx]][0] = (cov_tmp, cnt_mod, modprob_tmp)
+    probs = _cal_modfreq_in_aggregate_mode(hp1_highcov_pos, hp1_highcov_histos, model, args.seq_len, args.only_close)
     for highcov_idx in range(len(hp1_highcov_pos)):
         modprob_tmp = probs[highcov_idx]
         cov_tmp = hp1_highcov_covs[highcov_idx]
-        cnt_mod = round(cov_tmp * modprob_tmp, 2)
-        refpos2result[hp1_highcov_pos[highcov_idx]][1] = (cov_tmp, cnt_mod, modprob_tmp)
-    probs = _cal_modfreq_in_aggregate_mode(hp2_highcov_pos, hp2_highcov_histos, model, args.seq_len)
+        if args.discrete:
+            d_cnt_mod, _, d_modprob_tmp = discretize_score(modprob_tmp, cov_tmp)
+            refpos2result[hp1_highcov_pos[highcov_idx]][1] = (cov_tmp, d_cnt_mod, d_modprob_tmp)
+        else:
+            cnt_mod = round(cov_tmp * modprob_tmp, 2)
+            refpos2result[hp1_highcov_pos[highcov_idx]][1] = (cov_tmp, cnt_mod, modprob_tmp)
+    probs = _cal_modfreq_in_aggregate_mode(hp2_highcov_pos, hp2_highcov_histos, model, args.seq_len, args.only_close)
     for highcov_idx in range(len(hp2_highcov_pos)):
         modprob_tmp = probs[highcov_idx]
         cov_tmp = hp2_highcov_covs[highcov_idx]
-        cnt_mod = round(cov_tmp * modprob_tmp, 2)
-        refpos2result[hp2_highcov_pos[highcov_idx]][2] = (cov_tmp, cnt_mod, modprob_tmp)
+        if args.discrete:
+            d_cnt_mod, _, d_modprob_tmp = discretize_score(modprob_tmp, cov_tmp)
+            refpos2result[hp2_highcov_pos[highcov_idx]][2] = (cov_tmp, d_cnt_mod, d_modprob_tmp)
+        else:
+            cnt_mod = round(cov_tmp * modprob_tmp, 2)
+            refpos2result[hp2_highcov_pos[highcov_idx]][2] = (cov_tmp, cnt_mod, modprob_tmp)
 
     refpos_results = []
     for refpos in all_refposes:
         refpos_results.append((refpos, refpos2result[refpos][0], refpos2result[refpos][1],
                                refpos2result[refpos][2]))
     return refpos_results
 
@@ -325,17 +435,17 @@
             for modprob, hap in modinfo:
                 total_mods.append(modprob)
                 if not args.no_hap:
                     if hap == 1:
                         hp1_mods.append(modprob)
                     elif hap == 2:
                         hp2_mods.append(modprob)
-            info_all = _cal_modfreq_in_count_mode(total_mods, args.prob_cf) if len(total_mods) > 0 else None
-            info_hp1 = _cal_modfreq_in_count_mode(hp1_mods, args.prob_cf) if len(hp1_mods) > 0 else None
-            info_hp2 = _cal_modfreq_in_count_mode(hp2_mods, args.prob_cf) if len(hp2_mods) > 0 else None
+            info_all = _cal_modfreq_in_count_mode(total_mods, args.prob_cf, args.no_amb_cov) if len(total_mods) > 0 else None
+            info_hp1 = _cal_modfreq_in_count_mode(hp1_mods, args.prob_cf, args.no_amb_cov) if len(hp1_mods) > 0 else None
+            info_hp2 = _cal_modfreq_in_count_mode(hp2_mods, args.prob_cf, args.no_amb_cov) if len(hp2_mods) > 0 else None
             refpos_results.append((refpos, info_all, info_hp1, info_hp2))
     elif args.call_mode == "aggregate":
         refpos_results = _call_modfreq_of_one_region_aggregate_mode(refpos2modinfo, args)
     else:
         raise ValueError("wrong --call_mode")
 
     return refpos_results
@@ -553,15 +663,15 @@
             pysam.tabix_index(bedfile, force=True,
                               preset="bed",
                               keep_original=False)
     sys.stderr.write('write_process-{} finished\n'.format(os.getpid()))
 
 
 def call_mods_frequency_from_bamfile(args):
-    print("[main]call_freq_bam starts..")
+    sys.stderr.write("[main]call_freq_bam starts..\n")
     start = time.time()
 
     if args.call_mode == "aggregate" and not os.path.exists(args.aggre_model):
         raise ValueError("--aggre_model is not set right!")
 
     inputpath = _check_input_file(args.input_bam)
     index_bam_if_needed2(inputpath, args.threads)
@@ -574,16 +684,17 @@
 
     dnacontigs = DNAReference(args.ref).getcontigs()
     motifs = get_motif_seqs(args.motifs)
 
     motifs_filter = None
     if args.refsites_only or args.refsites_all:
         motifs_filter = motifs
-        print("[###] --refsites_only (or/and --refsites_all) is set as True, gonna keep only motifs({}) sites "
-              "of genome reference in the results".format(motifs_filter))
+        sys.stderr.write("[###] --refsites_only (or/and --refsites_all) is set as True, "
+                         "gonna keep only motifs({}) sites of genome reference in the "
+                         "results\n".format(motifs_filter))
 
     nproc = args.threads
     if nproc < 3:
         nproc = 3
     region_q = Queue()
     bed_q = Queue()
 
@@ -607,15 +718,15 @@
 
     for p in ps_gen:
         p.join()
     p_read.join()
     bed_q.put("kill")
     p_w.join()
 
-    print("[main]call_freq_bam costs %.1f seconds.." % (time.time() - start))
+    sys.stderr.write("[main]call_freq_bam costs %.1f seconds..\n" % (time.time() - start))
 
 
 def main():
     parser = argparse.ArgumentParser(description='calculate frequency of interested sites at genome level '
                                                  'from aligned.sorted.bam')
 
     parser.add_argument('--threads', action="store", type=int, required=False, default=5,
@@ -646,23 +757,26 @@
     scfb_callfreq.add_argument('--modtype', type=str, action="store", required=False, default="5mC",
                                choices=["5mC", ],
                                help='modification type, default 5mC.')
     scfb_callfreq.add_argument('--call_mode', type=str, action="store", required=False, default="count",
                                choices=["count", "aggregate"],
                                help='call mode: count, aggregate. default count.')
     scfb_callfreq.add_argument('--prob_cf', type=float, action="store", required=False, default=0.0,
-                               help='this is to remove ambiguous calls. '
+                               help='this is to remove ambiguous calls (only for count-mode now). '
                                'if abs(prob1-prob0)>=prob_cf, then we use the call. e.g., proc_cf=0 '
                                'means use all calls. range [0, 1], default 0.0.')
+    scfb_callfreq.add_argument('--no_amb_cov', action="store_true", required=False, default=False,
+                               help='when using prob_cf>0, DO NOT count ambiguous calls '
+                                    'for calculating reads coverage')
     scfb_callfreq.add_argument("--hap_tag", type=str, action="store", required=False, default="HP",
                                help="haplotype tag, default HP")
-    scfb_callfreq.add_argument("--mapq", type=int, default=10, required=False,
-                               help="MAPping Quality cutoff for selecting alignment items, default 10")
-    scfb_callfreq.add_argument("--identity", type=float, default=0.70, required=False,
-                               help="identity cutoff for selecting alignment items, default 0.70")
+    scfb_callfreq.add_argument("--mapq", type=int, default=1, required=False,
+                               help="MAPping Quality cutoff for selecting alignment items, default 1")
+    scfb_callfreq.add_argument("--identity", type=float, default=0.0, required=False,
+                               help="identity cutoff for selecting alignment items, [0.0, 1.0], default 0.0")
     scfb_callfreq.add_argument("--no_supplementary", action="store_true", default=False, required=False,
                                help="not use supplementary alignment")
     scfb_callfreq.add_argument("--motifs", action="store", type=str,
                                required=False, default='CG',
                                help='motif seq to be extracted, default: CG. '
                                     'can be multi motifs splited by comma '
                                     '(no space allowed in the input str), '
@@ -700,14 +814,18 @@
     scfb_aggre.add_argument('--hid_rnn', type=int, default=32, required=False,
                             help="BiRNN hidden_size, default 32")
     scfb_aggre.add_argument('--bin_size', type=int, action="store", required=False, default=20,
                             help="histogram bin size, default 20")
     scfb_aggre.add_argument('--cov_cf', action="store", type=int, required=False,
                             default=4, help="coverage cutoff, to consider if use aggregate model to "
                                             "re-predict the modstate of the site")
+    scfb_aggre.add_argument('--only_close', action="store_true", default=False, required=False,
+                            help="[EXPERIMENTAL]")
+    scfb_aggre.add_argument('--discrete', action="store_true", default=False, required=False,
+                            help="[EXPERIMENTAL]")
     scfb_aggre.add_argument('--tseed', type=int, default=1234,
                             help='random seed for torch')
 
     args = parser.parse_args()
 
     call_mods_frequency_from_bamfile(args)
```

### Comparing `ccsmeth-0.3.2/ccsmeth/call_mods_freq_txt.py` & `ccsmeth-0.3.3/ccsmeth/call_mods_freq_txt.py`

 * *Files identical despite different names*

### Comparing `ccsmeth-0.3.2/ccsmeth/ccsmeth.py` & `ccsmeth-0.3.3/ccsmeth/ccsmeth.py`

 * *Files 1% similar despite different names*

```diff
@@ -294,18 +294,18 @@
     scm_extract.add_argument("--loginfo", type=str, default="no", required=False,
                              help="if printing more info of feature extraction on reads. "
                                   "yes or no, default no")
 
     scm_extract_ref = sub_call_mods.add_argument_group("EXTRACTION ALIGN_MODE")
     scm_extract_ref.add_argument("--ref", type=str, required=False,
                                  help="path to genome reference to be aligned, in fasta/fa format.")
-    scm_extract_ref.add_argument("--mapq", type=int, default=10, required=False,
-                                 help="MAPping Quality cutoff for selecting alignment items, default 10")
-    scm_extract_ref.add_argument("--identity", type=float, default=0.70, required=False,
-                                 help="identity cutoff for selecting alignment items, default 0.70")
+    scm_extract_ref.add_argument("--mapq", type=int, default=1, required=False,
+                                 help="MAPping Quality cutoff for selecting alignment items, default 1")
+    scm_extract_ref.add_argument("--identity", type=float, default=0.0, required=False,
+                                 help="identity cutoff for selecting alignment items, [0.0, 1.0], default 0.0")
     scm_extract_ref.add_argument("--no_supplementary", action="store_true", default=False, required=False,
                                  help="not use supplementary alignment")
     scm_extract_ref.add_argument("--is_mapfea", type=str, default="no", required=False,
                                  help="if extract mapping features, yes or no, default no")
     scm_extract_ref.add_argument("--skip_unmapped", type=str, default="yes", required=False,
                                  help="if skipping unmapped sites in reads, yes or no, default yes")
 
@@ -371,18 +371,18 @@
     #                              "the PATH.")
     se_extract.add_argument("--holes_batch", type=int, default=50, required=False,
                             help="number of holes/hifi-reads in an batch to get/put in queues, default 50")
 
     se_extract_ref = sub_extract.add_argument_group("EXTRACTION ALIGN_MODE")
     se_extract_ref.add_argument("--ref", type=str, required=False,
                                 help="path to genome reference to be aligned, in fasta/fa format.")
-    se_extract_ref.add_argument("--mapq", type=int, default=10, required=False,
-                                help="MAPping Quality cutoff for selecting alignment items, default 10")
-    se_extract_ref.add_argument("--identity", type=float, default=0.70, required=False,
-                                help="identity cutoff for selecting alignment items, default 0.70")
+    se_extract_ref.add_argument("--mapq", type=int, default=1, required=False,
+                                help="MAPping Quality cutoff for selecting alignment items, default 1")
+    se_extract_ref.add_argument("--identity", type=float, default=0.0, required=False,
+                                help="identity cutoff for selecting alignment items, [0.0, 1.0], default 0.0")
     se_extract_ref.add_argument("--no_supplementary", action="store_true", default=False, required=False,
                                 help="not use supplementary alignment")
     se_extract_ref.add_argument("--is_mapfea", type=str, default="no", required=False,
                                 help="if extract mapping features, yes or no, default no")
     se_extract_ref.add_argument("--skip_unmapped", type=str, default="yes", required=False,
                                 help="if skipping unmapped sites in reads, yes or no, default yes")
 
@@ -479,23 +479,26 @@
     scfb_callfreq.add_argument('--modtype', type=str, action="store", required=False, default="5mC",
                                choices=["5mC", ],
                                help='modification type, default 5mC.')
     scfb_callfreq.add_argument('--call_mode', type=str, action="store", required=False, default="count",
                                choices=["count", "aggregate"],
                                help='call mode: count, aggregate. default count.')
     scfb_callfreq.add_argument('--prob_cf', type=float, action="store", required=False, default=0.0,
-                               help='this is to remove ambiguous calls. '
+                               help='this is to remove ambiguous calls (only for count-mode now). '
                                     'if abs(prob1-prob0)>=prob_cf, then we use the call. e.g., proc_cf=0 '
                                     'means use all calls. range [0, 1], default 0.0.')
+    scfb_callfreq.add_argument('--no_amb_cov', action="store_true", required=False, default=False,
+                               help='when using prob_cf>0, DO NOT count ambiguous calls '
+                                    'for calculating reads coverage')
     scfb_callfreq.add_argument("--hap_tag", type=str, action="store", required=False, default="HP",
                                help="haplotype tag, default HP")
-    scfb_callfreq.add_argument("--mapq", type=int, default=10, required=False,
-                               help="MAPping Quality cutoff for selecting alignment items, default 10")
-    scfb_callfreq.add_argument("--identity", type=float, default=0.70, required=False,
-                               help="identity cutoff for selecting alignment items, default 0.70")
+    scfb_callfreq.add_argument("--mapq", type=int, default=1, required=False,
+                               help="MAPping Quality cutoff for selecting alignment items, default 1")
+    scfb_callfreq.add_argument("--identity", type=float, default=0.0, required=False,
+                               help="identity cutoff for selecting alignment items, [0.0, 1.0], default 0.0")
     scfb_callfreq.add_argument("--no_supplementary", action="store_true", default=False, required=False,
                                help="not use supplementary alignment")
     scfb_callfreq.add_argument("--motifs", action="store", type=str,
                                required=False, default='CG',
                                help='motif seq to be extracted, default: CG. '
                                     'can be multi motifs splited by comma '
                                     '(no space allowed in the input str), '
@@ -533,14 +536,18 @@
     scfb_aggre.add_argument('--hid_rnn', type=int, default=32, required=False,
                             help="BiRNN hidden_size, default 32")
     scfb_aggre.add_argument('--bin_size', type=int, action="store", required=False, default=20,
                             help="histogram bin size, default 20")
     scfb_aggre.add_argument('--cov_cf', action="store", type=int, required=False,
                             default=4, help="coverage cutoff, to consider if use aggregate model to "
                                             "re-predict the modstate of the site")
+    scfb_aggre.add_argument('--only_close', action="store_true", default=False, required=False,
+                            help="[EXPERIMENTAL]")
+    scfb_aggre.add_argument('--discrete', action="store_true", default=False, required=False,
+                            help="[EXPERIMENTAL]")
     scfb_aggre.add_argument('--tseed', type=int, default=1234,
                             help='random seed for torch')
 
     sub_call_freqb.set_defaults(func=main_call_freqb)
 
     # sub_train =====================================================================================
     st_input = sub_train.add_argument_group("INPUT")
```

### Comparing `ccsmeth-0.3.2/ccsmeth/dataloader.py` & `ccsmeth-0.3.3/ccsmeth/dataloader.py`

 * *Files identical despite different names*

### Comparing `ccsmeth-0.3.2/ccsmeth/extract_features.py` & `ccsmeth-0.3.3/ccsmeth/extract_features.py`

 * *Files 1% similar despite different names*

```diff
@@ -692,18 +692,18 @@
     #                             "the PATH.")
     p_extract.add_argument("--holes_batch", type=int, default=50, required=False,
                            help="number of holes/hifi-reads in an batch to get/put in queues, default 50")
 
     p_extract_ref = parser.add_argument_group("EXTRACTION ALIGN_MODE")
     p_extract_ref.add_argument("--ref", type=str, required=False,
                                help="path to genome reference to be aligned, in fasta/fa format.")
-    p_extract_ref.add_argument("--mapq", type=int, default=10, required=False,
-                               help="MAPping Quality cutoff for selecting alignment items, default 10")
-    p_extract_ref.add_argument("--identity", type=float, default=0.70, required=False,
-                               help="identity cutoff for selecting alignment items, default 0.70")
+    p_extract_ref.add_argument("--mapq", type=int, default=1, required=False,
+                               help="MAPping Quality cutoff for selecting alignment items, default 1")
+    p_extract_ref.add_argument("--identity", type=float, default=0.0, required=False,
+                               help="identity cutoff for selecting alignment items, [0.0, 1.0], default 0.0")
     p_extract_ref.add_argument("--no_supplementary", action="store_true", default=False, required=False,
                                help="not use supplementary alignment")
     p_extract_ref.add_argument("--is_mapfea", type=str, default="no", required=False,
                                help="if extract mapping features, yes or no, default no")
     p_extract_ref.add_argument("--skip_unmapped", type=str, default="yes", required=False,
                                help="if skipping unmapped sites in reads, yes or no, default yes")
```

### Comparing `ccsmeth-0.3.2/ccsmeth/models.py` & `ccsmeth-0.3.3/ccsmeth/models.py`

 * *Files 2% similar despite different names*

```diff
@@ -41,30 +41,30 @@
             self.feas_ccs += 1
         if self.is_map:
             self.feas_ccs += 1
         if self.model_type == "attbilstm2s":
             self.rnn_cell = "lstm"
             self.rnn = nn.LSTM(embedding_size + self.feas_ccs, self.hidden_size, self.num_layers,
                                dropout=dropout_rate, batch_first=True, bidirectional=True)
-            self.rnn2 = nn.LSTM(embedding_size + self.feas_ccs, self.hidden_size, self.num_layers,
-                                dropout=dropout_rate, batch_first=True, bidirectional=True)
+            # self.rnn2 = nn.LSTM(embedding_size + self.feas_ccs, self.hidden_size, self.num_layers,
+            #                     dropout=dropout_rate, batch_first=True, bidirectional=True)
         elif self.model_type == "attbigru2s":
             self.rnn_cell = "gru"
             self.rnn = nn.GRU(embedding_size + self.feas_ccs, self.hidden_size, self.num_layers,
                               dropout=dropout_rate, batch_first=True, bidirectional=True)
-            self.rnn2 = nn.GRU(embedding_size + self.feas_ccs, self.hidden_size, self.num_layers,
-                               dropout=dropout_rate, batch_first=True, bidirectional=True)
+            # self.rnn2 = nn.GRU(embedding_size + self.feas_ccs, self.hidden_size, self.num_layers,
+            #                    dropout=dropout_rate, batch_first=True, bidirectional=True)
         else:
             raise ValueError("--model_type not set right!")
 
         self.dropout1 = nn.Dropout(p=dropout_rate)
         self.fc1 = nn.Linear(self.hidden_size * 2 * 2, self.num_classes)  # 2 for bidirection, another 2 for 2 strands
 
         self._att3 = Attention(self.hidden_size * 2, self.hidden_size * 2, self.hidden_size)
-        self._att3_2 = Attention(self.hidden_size * 2, self.hidden_size * 2, self.hidden_size)
+        # self._att3_2 = Attention(self.hidden_size * 2, self.hidden_size * 2, self.hidden_size)
 
         self.softmax = nn.Softmax(1)
 
     def get_model_type(self):
         return self.model_type
 
     def init_hidden(self, batch_size, num_layers, hidden_size):
@@ -114,14 +114,17 @@
             out1 = torch.cat((out1, maps), 2)  # (N, L, C)
             maps2 = torch.reshape(maps2, (-1, self.seq_len, 1)).float()
             out2 = torch.cat((out2, maps2), 2)  # (N, L, C)
 
         out1, n_states1 = self.rnn(out1, self.init_hidden(out1.size(0),
                                                           self.num_layers,
                                                           self.hidden_size))  # (N, L, nhid*2)
+        # out2, n_states2 = self.rnn2(out2, self.init_hidden(out2.size(0),
+        #                                                    self.num_layers,
+        #                                                    self.hidden_size))  # (N, L, nhid*2)
         out2, n_states2 = self.rnn(out2, self.init_hidden(out2.size(0),
                                                           self.num_layers,
                                                           self.hidden_size))  # (N, L, nhid*2)
 
         # attention_net3 ======
         # h_n: (num_layer * 2, N, nhid), h_0, c_0 -> h_n, c_n not affected by batch_first
         # h_n (last layer) = out[:, -1, :self.hidden_size] concats out1[:, 0, self.hidden_size:]
@@ -129,15 +132,16 @@
         h_n1 = h_n1.reshape(self.num_layers, 2, -1, self.hidden_size)[-1]  # last layer (2, N, nhid)
         h_n1 = h_n1.transpose(0, 1).reshape(-1, 1, 2 * self.hidden_size)
         out1, att_weights1 = self._att3(h_n1, out1)
 
         h_n2 = n_states2[0] if self.rnn_cell == "lstm" else n_states2
         h_n2 = h_n2.reshape(self.num_layers, 2, -1, self.hidden_size)[-1]  # last layer (2, N, nhid)
         h_n2 = h_n2.transpose(0, 1).reshape(-1, 1, 2 * self.hidden_size)
-        out2, att_weights2 = self._att3_2(h_n2, out2)
+        # out2, att_weights2 = self._att3_2(h_n2, out2)
+        out2, att_weights2 = self._att3(h_n2, out2)
 
         out = torch.cat((out1, out2), 1)
 
         out = self.dropout1(out)
         out = self.fc1(out)
 
         return out, self.softmax(out)
```

### Comparing `ccsmeth-0.3.2/ccsmeth/train.py` & `ccsmeth-0.3.3/ccsmeth/train.py`

 * *Files identical despite different names*

### Comparing `ccsmeth-0.3.2/ccsmeth/train_multigpu.py` & `ccsmeth-0.3.3/ccsmeth/train_multigpu.py`

 * *Files 0% similar despite different names*

```diff
@@ -129,15 +129,15 @@
         model.load_state_dict(model_dict)
 
     dist.barrier()
 
     model = model.cuda(local_rank)
     # DistributedDataParallel
     model = DDP(model, device_ids=[local_rank], output_device=local_rank,
-                find_unused_parameters=True)
+                find_unused_parameters=False)
 
     # 2. define dataloader
     print("training_process-{} reading data..".format(os.getpid()))
     if args.model_type in {"attbigru2s", "attbilstm2s"}:
         train_linenum = count_line_num(args.train_file, False)
         train_offsets = generate_offsets(args.train_file)
         train_dataset = FeaData3(args.train_file, train_offsets, train_linenum)
```

### Comparing `ccsmeth-0.3.2/ccsmeth/utils/attention.py` & `ccsmeth-0.3.3/ccsmeth/utils/attention.py`

 * *Files identical despite different names*

### Comparing `ccsmeth-0.3.2/ccsmeth/utils/constants_torch.py` & `ccsmeth-0.3.3/ccsmeth/utils/constants_torch.py`

 * *Files identical despite different names*

### Comparing `ccsmeth-0.3.2/ccsmeth/utils/lookahead.py` & `ccsmeth-0.3.3/ccsmeth/utils/lookahead.py`

 * *Files identical despite different names*

### Comparing `ccsmeth-0.3.2/ccsmeth/utils/process_utils.py` & `ccsmeth-0.3.3/ccsmeth/utils/process_utils.py`

 * *Files identical despite different names*

### Comparing `ccsmeth-0.3.2/ccsmeth/utils/ranger2020.py` & `ccsmeth-0.3.3/ccsmeth/utils/ranger2020.py`

 * *Files identical despite different names*

### Comparing `ccsmeth-0.3.2/ccsmeth/utils/ref_reader.py` & `ccsmeth-0.3.3/ccsmeth/utils/ref_reader.py`

 * *Files identical despite different names*

### Comparing `ccsmeth-0.3.2/ccsmeth/utils/sam2fastq_std.py` & `ccsmeth-0.3.3/ccsmeth/utils/sam2fastq_std.py`

 * *Files identical despite different names*

### Comparing `ccsmeth-0.3.2/ccsmeth/_bam2modbam.py` & `ccsmeth-0.3.3/ccsmeth/_bam2modbam.py`

 * *Files identical despite different names*

### Comparing `ccsmeth-0.3.2/ccsmeth.egg-info/SOURCES.txt` & `ccsmeth-0.3.3/ccsmeth.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ccsmeth-0.3.2/LICENSE` & `ccsmeth-0.3.3/LICENSE`

 * *Files identical despite different names*

### Comparing `ccsmeth-0.3.2/README.rst` & `ccsmeth-0.3.3/README.rst`

 * *Files 23% similar despite different names*

```diff
@@ -1,13 +1,22 @@
 ccsmeth
 ========
 
 
 Documentation
 -------------
+v0.3.3
+----------
+more robust operation for MM/ML tags
+
+update the call_mods model (v1 to v2), use shared params for both rnn and attention
+
+update aggregate model (v2 to v2p)
+
+
 v0.3.2
 ----------
 fix bug (0-pos CG in reverse strand) of call_freqb module
 
 add output check at the start of call_mods/call_freqb
 
 update aggregate model
```

### Comparing `ccsmeth-0.3.2/setup.py` & `ccsmeth-0.3.3/setup.py`

 * *Files identical despite different names*

