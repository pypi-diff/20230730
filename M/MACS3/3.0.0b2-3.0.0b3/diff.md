# Comparing `tmp/MACS3-3.0.0b2.tar.gz` & `tmp/MACS3-3.0.0b3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "MACS3-3.0.0b2.tar", last modified: Fri Jun 23 21:35:58 2023, max compression
+gzip compressed data, was "MACS3-3.0.0b3.tar", last modified: Sun Jul 30 16:49:27 2023, max compression
```

## Comparing `MACS3-3.0.0b2.tar` & `MACS3-3.0.0b3.tar`

### file list

```diff
@@ -1,363 +1,364 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 21:35:58.180009 MACS3-3.0.0b2/
--rw-r--r--   0 runner    (1001) docker     (123)    82248 2023-06-23 21:33:58.000000 MACS3-3.0.0b2/ChangeLog
--rw-r--r--   0 runner    (1001) docker     (123)     1526 2023-06-23 21:33:58.000000 MACS3-3.0.0b2/LICENSE
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 21:35:58.128005 MACS3-3.0.0b2/MACS3/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 21:35:58.128005 MACS3-3.0.0b2/MACS3/Commands/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-23 21:33:58.000000 MACS3-3.0.0b2/MACS3/Commands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1876 2023-06-23 21:33:58.000000 MACS3-3.0.0b2/MACS3/Commands/bdgbroadcall_cmd.py
--rw-r--r--   0 runner    (1001) docker     (123)     3403 2023-06-23 21:33:58.000000 MACS3-3.0.0b2/MACS3/Commands/bdgcmp_cmd.py
--rw-r--r--   0 runner    (1001) docker     (123)     4118 2023-06-23 21:33:58.000000 MACS3-3.0.0b2/MACS3/Commands/bdgdiff_cmd.py
--rw-r--r--   0 runner    (1001) docker     (123)     2105 2023-06-23 21:33:58.000000 MACS3-3.0.0b2/MACS3/Commands/bdgopt_cmd.py
--rw-r--r--   0 runner    (1001) docker     (123)     2491 2023-06-23 21:33:58.000000 MACS3-3.0.0b2/MACS3/Commands/bdgpeakcall_cmd.py
--rw-r--r--   0 runner    (1001) docker     (123)    17848 2023-06-23 21:33:58.000000 MACS3-3.0.0b2/MACS3/Commands/callpeak_cmd.py
--rw-r--r--   0 runner    (1001) docker     (123)    18078 2023-06-23 21:33:58.000000 MACS3-3.0.0b2/MACS3/Commands/callvar_cmd.py
--rw-r--r--   0 runner    (1001) docker     (123)     1632 2023-06-23 21:33:58.000000 MACS3-3.0.0b2/MACS3/Commands/cmbreps_cmd.py
--rw-r--r--   0 runner    (1001) docker     (123)     9693 2023-06-23 21:33:58.000000 MACS3-3.0.0b2/MACS3/Commands/diffpeak_cmd.py
--rw-r--r--   0 runner    (1001) docker     (123)     4563 2023-06-23 21:33:58.000000 MACS3-3.0.0b2/MACS3/Commands/filterdup_cmd.py
--rw-r--r--   0 runner    (1001) docker     (123)    28259 2023-06-23 21:33:58.000000 MACS3-3.0.0b2/MACS3/Commands/hmmratac_cmd.py
--rw-r--r--   0 runner    (1001) docker     (123)     3755 2023-06-23 21:33:58.000000 MACS3-3.0.0b2/MACS3/Commands/pileup_cmd.py
--rw-r--r--   0 runner    (1001) docker     (123)     4092 2023-06-23 21:33:58.000000 MACS3-3.0.0b2/MACS3/Commands/predictd_cmd.py
--rw-r--r--   0 runner    (1001) docker     (123)     3873 2023-06-23 21:33:58.000000 MACS3-3.0.0b2/MACS3/Commands/randsample_cmd.py
--rw-r--r--   0 runner    (1001) docker     (123)     3955 2023-06-23 21:33:58.000000 MACS3-3.0.0b2/MACS3/Commands/refinepeak_cmd.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 21:35:58.132005 MACS3-3.0.0b2/MACS3/IO/
--rw-r--r--   0 runner    (1001) docker     (123)    25603 2023-06-23 21:33:58.000000 MACS3-3.0.0b2/MACS3/IO/BAM.pyx
--rw-r--r--   0 runner    (1001) docker     (123)     2538 2023-06-23 21:33:58.000000 MACS3-3.0.0b2/MACS3/IO/BedGraphIO.pyx
--rw-r--r--   0 runner    (1001) docker     (123)    10381 2023-06-23 21:33:58.000000 MACS3-3.0.0b2/MACS3/IO/OutputWriter.py
--rw-r--r--   0 runner    (1001) docker     (123)    52515 2023-06-23 21:33:58.000000 MACS3-3.0.0b2/MACS3/IO/Parser.pyx
--rw-r--r--   0 runner    (1001) docker     (123)    54269 2023-06-23 21:33:58.000000 MACS3-3.0.0b2/MACS3/IO/PeakIO.pyx
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-23 21:33:58.000000 MACS3-3.0.0b2/MACS3/IO/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 21:35:58.136006 MACS3-3.0.0b2/MACS3/Signal/
--rw-r--r--   0 runner    (1001) docker     (123)    48049 2023-06-23 21:33:58.000000 MACS3-3.0.0b2/MACS3/Signal/BedGraph.pyx
--rw-r--r--   0 runner    (1001) docker     (123)    76301 2023-06-23 21:33:58.000000 MACS3-3.0.0b2/MACS3/Signal/CallPeakUnit.pyx
--rw-r--r--   0 runner    (1001) docker     (123)    21780 2023-06-23 21:33:58.000000 MACS3-3.0.0b2/MACS3/Signal/FixWidthTrack.pyx
--rw-r--r--   0 runner    (1001) docker     (123)    11209 2023-06-23 21:33:58.000000 MACS3-3.0.0b2/MACS3/Signal/HMMR_EM.pyx
--rw-r--r--   0 runner    (1001) docker     (123)     4209 2023-06-23 21:33:58.000000 MACS3-3.0.0b2/MACS3/Signal/HMMR_HMM.pyx
--rw-r--r--   0 runner    (1001) docker     (123)     7779 2023-06-23 21:33:58.000000 MACS3-3.0.0b2/MACS3/Signal/HMMR_Signal_Processing.pyx
--rw-r--r--   0 runner    (1001) docker     (123)    22046 2023-06-23 21:33:58.000000 MACS3-3.0.0b2/MACS3/Signal/PairedEndTrack.pyx
--rw-r--r--   0 runner    (1001) docker     (123)    17522 2023-06-23 21:33:58.000000 MACS3-3.0.0b2/MACS3/Signal/PeakDetect.pyx
--rw-r--r--   0 runner    (1001) docker     (123)    16813 2023-06-23 21:33:58.000000 MACS3-3.0.0b2/MACS3/Signal/PeakModel.pyx
--rw-r--r--   0 runner    (1001) docker     (123)    12726 2023-06-23 21:33:58.000000 MACS3-3.0.0b2/MACS3/Signal/PeakVariants.pyx
--rw-r--r--   0 runner    (1001) docker     (123)    23810 2023-06-23 21:33:58.000000 MACS3-3.0.0b2/MACS3/Signal/Pileup.pyx
--rw-r--r--   0 runner    (1001) docker     (123)     7898 2023-06-23 21:33:58.000000 MACS3-3.0.0b2/MACS3/Signal/PileupV2.pyx
--rw-r--r--   0 runner    (1001) docker     (123)    27685 2023-06-23 21:33:58.000000 MACS3-3.0.0b2/MACS3/Signal/PosReadsInfo.pyx
--rw-r--r--   0 runner    (1001) docker     (123)    24866 2023-06-23 21:33:58.000000 MACS3-3.0.0b2/MACS3/Signal/Prob.pyx
--rw-r--r--   0 runner    (1001) docker     (123)    35761 2023-06-23 21:33:58.000000 MACS3-3.0.0b2/MACS3/Signal/RACollection.pyx
--rw-r--r--   0 runner    (1001) docker     (123)    19506 2023-06-23 21:33:58.000000 MACS3-3.0.0b2/MACS3/Signal/ReadAlignment.pyx
--rw-r--r--   0 runner    (1001) docker     (123)    10155 2023-06-23 21:33:58.000000 MACS3-3.0.0b2/MACS3/Signal/Region.pyx
--rw-r--r--   0 runner    (1001) docker     (123)    58541 2023-06-23 21:33:58.000000 MACS3-3.0.0b2/MACS3/Signal/ScoreTrack.pyx
--rw-r--r--   0 runner    (1001) docker     (123)    13210 2023-06-23 21:33:58.000000 MACS3-3.0.0b2/MACS3/Signal/SignalProcessing.pyx
--rw-r--r--   0 runner    (1001) docker     (123)    12281 2023-06-23 21:33:58.000000 MACS3-3.0.0b2/MACS3/Signal/UnitigRACollection.pyx
--rw-r--r--   0 runner    (1001) docker     (123)    13764 2023-06-23 21:33:58.000000 MACS3-3.0.0b2/MACS3/Signal/VariantStat.pyx
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-23 21:33:58.000000 MACS3-3.0.0b2/MACS3/Signal/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13930 2023-06-23 21:33:58.000000 MACS3-3.0.0b2/MACS3/Signal/cPosValCalculation.c
--rw-r--r--   0 runner    (1001) docker     (123)     1786 2023-06-23 21:33:58.000000 MACS3-3.0.0b2/MACS3/Signal/cPosValCalculation.h
--rw-r--r--   0 runner    (1001) docker     (123)     1248 2023-06-23 21:33:58.000000 MACS3-3.0.0b2/MACS3/Signal/cPosValCalculation.pxd
--rw-r--r--   0 runner    (1001) docker     (123)     9826 2023-06-23 21:33:58.000000 MACS3-3.0.0b2/MACS3/Signal/swalign.c
--rw-r--r--   0 runner    (1001) docker     (123)     2358 2023-06-23 21:33:58.000000 MACS3-3.0.0b2/MACS3/Signal/swalign.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 21:35:58.136006 MACS3-3.0.0b2/MACS3/Utilities/
--rw-r--r--   0 runner    (1001) docker     (123)      661 2023-06-23 21:33:58.000000 MACS3-3.0.0b2/MACS3/Utilities/Constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     1079 2023-06-23 21:33:58.000000 MACS3-3.0.0b2/MACS3/Utilities/Logger.py
--rw-r--r--   0 runner    (1001) docker     (123)    31761 2023-06-23 21:33:58.000000 MACS3-3.0.0b2/MACS3/Utilities/OptValidator.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-23 21:33:58.000000 MACS3-3.0.0b2/MACS3/Utilities/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       49 2023-06-23 21:33:58.000000 MACS3-3.0.0b2/MACS3/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 21:35:58.140006 MACS3-3.0.0b2/MACS3/fermi-lite/
--rw-r--r--   0 runner    (1001) docker     (123)    19571 2023-06-23 21:33:58.000000 MACS3-3.0.0b2/MACS3/fermi-lite/bfc.c
--rw-r--r--   0 runner    (1001) docker     (123)     1181 2023-06-23 21:33:58.000000 MACS3-3.0.0b2/MACS3/fermi-lite/bseq.c
--rw-r--r--   0 runner    (1001) docker     (123)    12235 2023-06-23 21:33:58.000000 MACS3-3.0.0b2/MACS3/fermi-lite/bubble.c
--rw-r--r--   0 runner    (1001) docker     (123)     2271 2023-06-23 21:33:58.000000 MACS3-3.0.0b2/MACS3/fermi-lite/example.c
--rw-r--r--   0 runner    (1001) docker     (123)     5083 2023-06-23 21:33:58.000000 MACS3-3.0.0b2/MACS3/fermi-lite/fml.h
--rw-r--r--   0 runner    (1001) docker     (123)     3085 2023-06-23 21:33:58.000000 MACS3-3.0.0b2/MACS3/fermi-lite/htab.c
--rw-r--r--   0 runner    (1001) docker     (123)      622 2023-06-23 21:33:58.000000 MACS3-3.0.0b2/MACS3/fermi-lite/htab.h
--rw-r--r--   0 runner    (1001) docker     (123)      444 2023-06-23 21:33:58.000000 MACS3-3.0.0b2/MACS3/fermi-lite/internal.h
--rw-r--r--   0 runner    (1001) docker     (123)    21102 2023-06-23 21:33:58.000000 MACS3-3.0.0b2/MACS3/fermi-lite/khash.h
--rw-r--r--   0 runner    (1001) docker     (123)     2880 2023-06-23 21:33:58.000000 MACS3-3.0.0b2/MACS3/fermi-lite/kmer.h
--rw-r--r--   0 runner    (1001) docker     (123)     8739 2023-06-23 21:33:58.000000 MACS3-3.0.0b2/MACS3/fermi-lite/kseq.h
--rw-r--r--   0 runner    (1001) docker     (123)    10635 2023-06-23 21:33:58.000000 MACS3-3.0.0b2/MACS3/fermi-lite/ksort.h
--rw-r--r--   0 runner    (1001) docker     (123)     4437 2023-06-23 21:33:58.000000 MACS3-3.0.0b2/MACS3/fermi-lite/kstring.h
--rw-r--r--   0 runner    (1001) docker     (123)    12337 2023-06-23 21:33:58.000000 MACS3-3.0.0b2/MACS3/fermi-lite/ksw.c
--rw-r--r--   0 runner    (1001) docker     (123)     2485 2023-06-23 21:33:58.000000 MACS3-3.0.0b2/MACS3/fermi-lite/ksw.h
--rw-r--r--   0 runner    (1001) docker     (123)     1556 2023-06-23 21:33:58.000000 MACS3-3.0.0b2/MACS3/fermi-lite/kthread.c
--rw-r--r--   0 runner    (1001) docker     (123)     3289 2023-06-23 21:33:58.000000 MACS3-3.0.0b2/MACS3/fermi-lite/kvec.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 21:35:58.140006 MACS3-3.0.0b2/MACS3/fermi-lite/lib/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 21:35:58.144006 MACS3-3.0.0b2/MACS3/fermi-lite/lib/arm/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 21:35:58.164008 MACS3-3.0.0b2/MACS3/fermi-lite/lib/arm/neon/
--rw-r--r--   0 runner    (1001) docker     (123)     6276 2023-06-23 21:34:02.000000 MACS3-3.0.0b2/MACS3/fermi-lite/lib/arm/neon/aba.h
--rw-r--r--   0 runner    (1001) docker     (123)    10687 2023-06-23 21:34:02.000000 MACS3-3.0.0b2/MACS3/fermi-lite/lib/arm/neon/abd.h
--rw-r--r--   0 runner    (1001) docker     (123)     4266 2023-06-23 21:34:02.000000 MACS3-3.0.0b2/MACS3/fermi-lite/lib/arm/neon/abdl.h
--rw-r--r--   0 runner    (1001) docker     (123)    12280 2023-06-23 21:34:02.000000 MACS3-3.0.0b2/MACS3/fermi-lite/lib/arm/neon/abs.h
--rw-r--r--   0 runner    (1001) docker     (123)    18439 2023-06-23 21:34:02.000000 MACS3-3.0.0b2/MACS3/fermi-lite/lib/arm/neon/add.h
--rw-r--r--   0 runner    (1001) docker     (123)     3912 2023-06-23 21:34:02.000000 MACS3-3.0.0b2/MACS3/fermi-lite/lib/arm/neon/addl.h
--rw-r--r--   0 runner    (1001) docker     (123)     4141 2023-06-23 21:34:02.000000 MACS3-3.0.0b2/MACS3/fermi-lite/lib/arm/neon/addl_high.h
--rw-r--r--   0 runner    (1001) docker     (123)     8399 2023-06-23 21:34:02.000000 MACS3-3.0.0b2/MACS3/fermi-lite/lib/arm/neon/addlv.h
--rw-r--r--   0 runner    (1001) docker     (123)    10476 2023-06-23 21:34:02.000000 MACS3-3.0.0b2/MACS3/fermi-lite/lib/arm/neon/addv.h
--rw-r--r--   0 runner    (1001) docker     (123)     7501 2023-06-23 21:34:02.000000 MACS3-3.0.0b2/MACS3/fermi-lite/lib/arm/neon/addw.h
--rw-r--r--   0 runner    (1001) docker     (123)     6724 2023-06-23 21:34:02.000000 MACS3-3.0.0b2/MACS3/fermi-lite/lib/arm/neon/addw_high.h
--rw-r--r--   0 runner    (1001) docker     (123)    15830 2023-06-23 21:34:02.000000 MACS3-3.0.0b2/MACS3/fermi-lite/lib/arm/neon/and.h
--rw-r--r--   0 runner    (1001) docker     (123)    13752 2023-06-23 21:34:02.000000 MACS3-3.0.0b2/MACS3/fermi-lite/lib/arm/neon/bic.h
--rw-r--r--   0 runner    (1001) docker     (123)    14767 2023-06-23 21:34:02.000000 MACS3-3.0.0b2/MACS3/fermi-lite/lib/arm/neon/bsl.h
--rw-r--r--   0 runner    (1001) docker     (123)     4665 2023-06-23 21:34:02.000000 MACS3-3.0.0b2/MACS3/fermi-lite/lib/arm/neon/cagt.h
--rw-r--r--   0 runner    (1001) docker     (123)    21370 2023-06-23 21:34:02.000000 MACS3-3.0.0b2/MACS3/fermi-lite/lib/arm/neon/ceq.h
--rw-r--r--   0 runner    (1001) docker     (123)     9095 2023-06-23 21:34:02.000000 MACS3-3.0.0b2/MACS3/fermi-lite/lib/arm/neon/ceqz.h
--rw-r--r--   0 runner    (1001) docker     (123)    22658 2023-06-23 21:34:02.000000 MACS3-3.0.0b2/MACS3/fermi-lite/lib/arm/neon/cge.h
--rw-r--r--   0 runner    (1001) docker     (123)    11884 2023-06-23 21:34:02.000000 MACS3-3.0.0b2/MACS3/fermi-lite/lib/arm/neon/cgez.h
--rw-r--r--   0 runner    (1001) docker     (123)    22278 2023-06-23 21:34:02.000000 MACS3-3.0.0b2/MACS3/fermi-lite/lib/arm/neon/cgt.h
--rw-r--r--   0 runner    (1001) docker     (123)    11902 2023-06-23 21:34:02.000000 MACS3-3.0.0b2/MACS3/fermi-lite/lib/arm/neon/cgtz.h
--rw-r--r--   0 runner    (1001) docker     (123)    22658 2023-06-23 21:34:02.000000 MACS3-3.0.0b2/MACS3/fermi-lite/lib/arm/neon/cle.h
--rw-r--r--   0 runner    (1001) docker     (123)    11884 2023-06-23 21:34:02.000000 MACS3-3.0.0b2/MACS3/fermi-lite/lib/arm/neon/clez.h
--rw-r--r--   0 runner    (1001) docker     (123)     4854 2023-06-23 21:34:02.000000 MACS3-3.0.0b2/MACS3/fermi-lite/lib/arm/neon/cls.h
--rw-r--r--   0 runner    (1001) docker     (123)    22158 2023-06-23 21:34:02.000000 MACS3-3.0.0b2/MACS3/fermi-lite/lib/arm/neon/clt.h
--rw-r--r--   0 runner    (1001) docker     (123)     7771 2023-06-23 21:34:02.000000 MACS3-3.0.0b2/MACS3/fermi-lite/lib/arm/neon/cltz.h
--rw-r--r--   0 runner    (1001) docker     (123)    12387 2023-06-23 21:34:02.000000 MACS3-3.0.0b2/MACS3/fermi-lite/lib/arm/neon/clz.h
--rw-r--r--   0 runner    (1001) docker     (123)     4376 2023-06-23 21:34:02.000000 MACS3-3.0.0b2/MACS3/fermi-lite/lib/arm/neon/cnt.h
--rw-r--r--   0 runner    (1001) docker     (123)    11610 2023-06-23 21:34:02.000000 MACS3-3.0.0b2/MACS3/fermi-lite/lib/arm/neon/combine.h
--rw-r--r--   0 runner    (1001) docker     (123)     5174 2023-06-23 21:34:02.000000 MACS3-3.0.0b2/MACS3/fermi-lite/lib/arm/neon/create.h
--rw-r--r--   0 runner    (1001) docker     (123)    15180 2023-06-23 21:34:02.000000 MACS3-3.0.0b2/MACS3/fermi-lite/lib/arm/neon/cvt.h
--rw-r--r--   0 runner    (1001) docker     (123)     6420 2023-06-23 21:34:02.000000 MACS3-3.0.0b2/MACS3/fermi-lite/lib/arm/neon/dot.h
--rw-r--r--   0 runner    (1001) docker     (123)     7781 2023-06-23 21:34:02.000000 MACS3-3.0.0b2/MACS3/fermi-lite/lib/arm/neon/dot_lane.h
--rw-r--r--   0 runner    (1001) docker     (123)    21506 2023-06-23 21:34:02.000000 MACS3-3.0.0b2/MACS3/fermi-lite/lib/arm/neon/dup_lane.h
--rw-r--r--   0 runner    (1001) docker     (123)    15175 2023-06-23 21:34:02.000000 MACS3-3.0.0b2/MACS3/fermi-lite/lib/arm/neon/dup_n.h
--rw-r--r--   0 runner    (1001) docker     (123)    15830 2023-06-23 21:34:02.000000 MACS3-3.0.0b2/MACS3/fermi-lite/lib/arm/neon/eor.h
--rw-r--r--   0 runner    (1001) docker     (123)    39152 2023-06-23 21:34:02.000000 MACS3-3.0.0b2/MACS3/fermi-lite/lib/arm/neon/ext.h
--rw-r--r--   0 runner    (1001) docker     (123)     7901 2023-06-23 21:34:02.000000 MACS3-3.0.0b2/MACS3/fermi-lite/lib/arm/neon/get_high.h
--rw-r--r--   0 runner    (1001) docker     (123)    14459 2023-06-23 21:34:02.000000 MACS3-3.0.0b2/MACS3/fermi-lite/lib/arm/neon/get_lane.h
--rw-r--r--   0 runner    (1001) docker     (123)     8238 2023-06-23 21:34:02.000000 MACS3-3.0.0b2/MACS3/fermi-lite/lib/arm/neon/get_low.h
--rw-r--r--   0 runner    (1001) docker     (123)     9710 2023-06-23 21:34:02.000000 MACS3-3.0.0b2/MACS3/fermi-lite/lib/arm/neon/hadd.h
--rw-r--r--   0 runner    (1001) docker     (123)     9710 2023-06-23 21:34:02.000000 MACS3-3.0.0b2/MACS3/fermi-lite/lib/arm/neon/hsub.h
--rw-r--r--   0 runner    (1001) docker     (123)    11789 2023-06-23 21:34:02.000000 MACS3-3.0.0b2/MACS3/fermi-lite/lib/arm/neon/ld1.h
--rw-r--r--   0 runner    (1001) docker     (123)    16633 2023-06-23 21:34:02.000000 MACS3-3.0.0b2/MACS3/fermi-lite/lib/arm/neon/ld3.h
--rw-r--r--   0 runner    (1001) docker     (123)    15320 2023-06-23 21:34:02.000000 MACS3-3.0.0b2/MACS3/fermi-lite/lib/arm/neon/ld4.h
--rw-r--r--   0 runner    (1001) docker     (123)    19022 2023-06-23 21:34:02.000000 MACS3-3.0.0b2/MACS3/fermi-lite/lib/arm/neon/max.h
--rw-r--r--   0 runner    (1001) docker     (123)     6916 2023-06-23 21:34:02.000000 MACS3-3.0.0b2/MACS3/fermi-lite/lib/arm/neon/maxnm.h
--rw-r--r--   0 runner    (1001) docker     (123)     9895 2023-06-23 21:34:02.000000 MACS3-3.0.0b2/MACS3/fermi-lite/lib/arm/neon/maxv.h
--rw-r--r--   0 runner    (1001) docker     (123)    20487 2023-06-23 21:34:02.000000 MACS3-3.0.0b2/MACS3/fermi-lite/lib/arm/neon/min.h
--rw-r--r--   0 runner    (1001) docker     (123)     6916 2023-06-23 21:34:02.000000 MACS3-3.0.0b2/MACS3/fermi-lite/lib/arm/neon/minnm.h
--rw-r--r--   0 runner    (1001) docker     (123)    10751 2023-06-23 21:34:02.000000 MACS3-3.0.0b2/MACS3/fermi-lite/lib/arm/neon/minv.h
--rw-r--r--   0 runner    (1001) docker     (123)    16338 2023-06-23 21:34:02.000000 MACS3-3.0.0b2/MACS3/fermi-lite/lib/arm/neon/mla.h
--rw-r--r--   0 runner    (1001) docker     (123)    10252 2023-06-23 21:34:02.000000 MACS3-3.0.0b2/MACS3/fermi-lite/lib/arm/neon/mla_n.h
--rw-r--r--   0 runner    (1001) docker     (123)     5025 2023-06-23 21:34:02.000000 MACS3-3.0.0b2/MACS3/fermi-lite/lib/arm/neon/mlal.h
--rw-r--r--   0 runner    (1001) docker     (123)     5259 2023-06-23 21:34:02.000000 MACS3-3.0.0b2/MACS3/fermi-lite/lib/arm/neon/mlal_high.h
--rw-r--r--   0 runner    (1001) docker     (123)     4149 2023-06-23 21:34:02.000000 MACS3-3.0.0b2/MACS3/fermi-lite/lib/arm/neon/mlal_n.h
--rw-r--r--   0 runner    (1001) docker     (123)     7922 2023-06-23 21:34:02.000000 MACS3-3.0.0b2/MACS3/fermi-lite/lib/arm/neon/mls.h
--rw-r--r--   0 runner    (1001) docker     (123)     3888 2023-06-23 21:34:02.000000 MACS3-3.0.0b2/MACS3/fermi-lite/lib/arm/neon/mlsl.h
--rw-r--r--   0 runner    (1001) docker     (123)     4092 2023-06-23 21:34:02.000000 MACS3-3.0.0b2/MACS3/fermi-lite/lib/arm/neon/mlsl_high.h
--rw-r--r--   0 runner    (1001) docker     (123)     3110 2023-06-23 21:34:02.000000 MACS3-3.0.0b2/MACS3/fermi-lite/lib/arm/neon/mlsl_n.h
--rw-r--r--   0 runner    (1001) docker     (123)     6302 2023-06-23 21:34:02.000000 MACS3-3.0.0b2/MACS3/fermi-lite/lib/arm/neon/movl.h
--rw-r--r--   0 runner    (1001) docker     (123)     3784 2023-06-23 21:34:02.000000 MACS3-3.0.0b2/MACS3/fermi-lite/lib/arm/neon/movl_high.h
--rw-r--r--   0 runner    (1001) docker     (123)     5749 2023-06-23 21:34:02.000000 MACS3-3.0.0b2/MACS3/fermi-lite/lib/arm/neon/movn.h
--rw-r--r--   0 runner    (1001) docker     (123)     3905 2023-06-23 21:34:02.000000 MACS3-3.0.0b2/MACS3/fermi-lite/lib/arm/neon/movn_high.h
--rw-r--r--   0 runner    (1001) docker     (123)    16534 2023-06-23 21:34:02.000000 MACS3-3.0.0b2/MACS3/fermi-lite/lib/arm/neon/mul.h
--rw-r--r--   0 runner    (1001) docker     (123)    15323 2023-06-23 21:34:02.000000 MACS3-3.0.0b2/MACS3/fermi-lite/lib/arm/neon/mul_lane.h
--rw-r--r--   0 runner    (1001) docker     (123)    10970 2023-06-23 21:34:02.000000 MACS3-3.0.0b2/MACS3/fermi-lite/lib/arm/neon/mul_n.h
--rw-r--r--   0 runner    (1001) docker     (123)     7854 2023-06-23 21:34:02.000000 MACS3-3.0.0b2/MACS3/fermi-lite/lib/arm/neon/mull.h
--rw-r--r--   0 runner    (1001) docker     (123)     4044 2023-06-23 21:34:02.000000 MACS3-3.0.0b2/MACS3/fermi-lite/lib/arm/neon/mull_high.h
--rw-r--r--   0 runner    (1001) docker     (123)     5266 2023-06-23 21:34:02.000000 MACS3-3.0.0b2/MACS3/fermi-lite/lib/arm/neon/mull_n.h
--rw-r--r--   0 runner    (1001) docker     (123)    11934 2023-06-23 21:34:02.000000 MACS3-3.0.0b2/MACS3/fermi-lite/lib/arm/neon/mvn.h
--rw-r--r--   0 runner    (1001) docker     (123)    10654 2023-06-23 21:34:02.000000 MACS3-3.0.0b2/MACS3/fermi-lite/lib/arm/neon/neg.h
--rw-r--r--   0 runner    (1001) docker     (123)    14551 2023-06-23 21:34:02.000000 MACS3-3.0.0b2/MACS3/fermi-lite/lib/arm/neon/orn.h
--rw-r--r--   0 runner    (1001) docker     (123)    15798 2023-06-23 21:34:02.000000 MACS3-3.0.0b2/MACS3/fermi-lite/lib/arm/neon/orr.h
--rw-r--r--   0 runner    (1001) docker     (123)     6129 2023-06-23 21:34:02.000000 MACS3-3.0.0b2/MACS3/fermi-lite/lib/arm/neon/padal.h
--rw-r--r--   0 runner    (1001) docker     (123)     8877 2023-06-23 21:34:02.000000 MACS3-3.0.0b2/MACS3/fermi-lite/lib/arm/neon/padd.h
--rw-r--r--   0 runner    (1001) docker     (123)     7552 2023-06-23 21:34:02.000000 MACS3-3.0.0b2/MACS3/fermi-lite/lib/arm/neon/paddl.h
--rw-r--r--   0 runner    (1001) docker     (123)     7572 2023-06-23 21:34:02.000000 MACS3-3.0.0b2/MACS3/fermi-lite/lib/arm/neon/pmax.h
--rw-r--r--   0 runner    (1001) docker     (123)     7826 2023-06-23 21:34:02.000000 MACS3-3.0.0b2/MACS3/fermi-lite/lib/arm/neon/pmin.h
--rw-r--r--   0 runner    (1001) docker     (123)     7366 2023-06-23 21:34:02.000000 MACS3-3.0.0b2/MACS3/fermi-lite/lib/arm/neon/qabs.h
--rw-r--r--   0 runner    (1001) docker     (123)    15857 2023-06-23 21:34:02.000000 MACS3-3.0.0b2/MACS3/fermi-lite/lib/arm/neon/qadd.h
--rw-r--r--   0 runner    (1001) docker     (123)     4074 2023-06-23 21:34:02.000000 MACS3-3.0.0b2/MACS3/fermi-lite/lib/arm/neon/qdmulh.h
--rw-r--r--   0 runner    (1001) docker     (123)     4152 2023-06-23 21:34:02.000000 MACS3-3.0.0b2/MACS3/fermi-lite/lib/arm/neon/qdmull.h
--rw-r--r--   0 runner    (1001) docker     (123)     8266 2023-06-23 21:34:02.000000 MACS3-3.0.0b2/MACS3/fermi-lite/lib/arm/neon/qmovn.h
--rw-r--r--   0 runner    (1001) docker     (123)     4029 2023-06-23 21:34:02.000000 MACS3-3.0.0b2/MACS3/fermi-lite/lib/arm/neon/qmovn_high.h
--rw-r--r--   0 runner    (1001) docker     (123)     5196 2023-06-23 21:34:02.000000 MACS3-3.0.0b2/MACS3/fermi-lite/lib/arm/neon/qmovun.h
--rw-r--r--   0 runner    (1001) docker     (123)     8600 2023-06-23 21:34:02.000000 MACS3-3.0.0b2/MACS3/fermi-lite/lib/arm/neon/qneg.h
--rw-r--r--   0 runner    (1001) docker     (123)     5260 2023-06-23 21:34:02.000000 MACS3-3.0.0b2/MACS3/fermi-lite/lib/arm/neon/qrdmulh.h
--rw-r--r--   0 runner    (1001) docker     (123)     4088 2023-06-23 21:34:02.000000 MACS3-3.0.0b2/MACS3/fermi-lite/lib/arm/neon/qrdmulh_n.h
--rw-r--r--   0 runner    (1001) docker     (123)    19189 2023-06-23 21:34:02.000000 MACS3-3.0.0b2/MACS3/fermi-lite/lib/arm/neon/qshl.h
--rw-r--r--   0 runner    (1001) docker     (123)    15571 2023-06-23 21:34:02.000000 MACS3-3.0.0b2/MACS3/fermi-lite/lib/arm/neon/qsub.h
--rw-r--r--   0 runner    (1001) docker     (123)    17511 2023-06-23 21:34:02.000000 MACS3-3.0.0b2/MACS3/fermi-lite/lib/arm/neon/qtbl.h
--rw-r--r--   0 runner    (1001) docker     (123)    19270 2023-06-23 21:34:02.000000 MACS3-3.0.0b2/MACS3/fermi-lite/lib/arm/neon/qtbx.h
--rw-r--r--   0 runner    (1001) docker     (123)     6384 2023-06-23 21:34:02.000000 MACS3-3.0.0b2/MACS3/fermi-lite/lib/arm/neon/rbit.h
--rw-r--r--   0 runner    (1001) docker     (123)    95760 2023-06-23 21:34:02.000000 MACS3-3.0.0b2/MACS3/fermi-lite/lib/arm/neon/reinterpret.h
--rw-r--r--   0 runner    (1001) docker     (123)     4773 2023-06-23 21:34:02.000000 MACS3-3.0.0b2/MACS3/fermi-lite/lib/arm/neon/rev16.h
--rw-r--r--   0 runner    (1001) docker     (123)     8072 2023-06-23 21:34:02.000000 MACS3-3.0.0b2/MACS3/fermi-lite/lib/arm/neon/rev32.h
--rw-r--r--   0 runner    (1001) docker     (123)    11898 2023-06-23 21:34:02.000000 MACS3-3.0.0b2/MACS3/fermi-lite/lib/arm/neon/rev64.h
--rw-r--r--   0 runner    (1001) docker     (123)    16270 2023-06-23 21:34:02.000000 MACS3-3.0.0b2/MACS3/fermi-lite/lib/arm/neon/rhadd.h
--rw-r--r--   0 runner    (1001) docker     (123)     4269 2023-06-23 21:34:02.000000 MACS3-3.0.0b2/MACS3/fermi-lite/lib/arm/neon/rnd.h
--rw-r--r--   0 runner    (1001) docker     (123)    43945 2023-06-23 21:34:02.000000 MACS3-3.0.0b2/MACS3/fermi-lite/lib/arm/neon/rshl.h
--rw-r--r--   0 runner    (1001) docker     (123)    16744 2023-06-23 21:34:02.000000 MACS3-3.0.0b2/MACS3/fermi-lite/lib/arm/neon/rshr_n.h
--rw-r--r--   0 runner    (1001) docker     (123)     7379 2023-06-23 21:34:02.000000 MACS3-3.0.0b2/MACS3/fermi-lite/lib/arm/neon/rsra_n.h
--rw-r--r--   0 runner    (1001) docker     (123)    13789 2023-06-23 21:34:02.000000 MACS3-3.0.0b2/MACS3/fermi-lite/lib/arm/neon/set_lane.h
--rw-r--r--   0 runner    (1001) docker     (123)    35543 2023-06-23 21:34:02.000000 MACS3-3.0.0b2/MACS3/fermi-lite/lib/arm/neon/shl.h
--rw-r--r--   0 runner    (1001) docker     (123)    18134 2023-06-23 21:34:02.000000 MACS3-3.0.0b2/MACS3/fermi-lite/lib/arm/neon/shl_n.h
--rw-r--r--   0 runner    (1001) docker     (123)    19435 2023-06-23 21:34:02.000000 MACS3-3.0.0b2/MACS3/fermi-lite/lib/arm/neon/shr_n.h
--rw-r--r--   0 runner    (1001) docker     (123)     7090 2023-06-23 21:34:02.000000 MACS3-3.0.0b2/MACS3/fermi-lite/lib/arm/neon/sra_n.h
--rw-r--r--   0 runner    (1001) docker     (123)    10700 2023-06-23 21:34:02.000000 MACS3-3.0.0b2/MACS3/fermi-lite/lib/arm/neon/st1.h
--rw-r--r--   0 runner    (1001) docker     (123)    12450 2023-06-23 21:34:02.000000 MACS3-3.0.0b2/MACS3/fermi-lite/lib/arm/neon/st1_lane.h
--rw-r--r--   0 runner    (1001) docker     (123)    14527 2023-06-23 21:34:02.000000 MACS3-3.0.0b2/MACS3/fermi-lite/lib/arm/neon/st3.h
--rw-r--r--   0 runner    (1001) docker     (123)    16018 2023-06-23 21:34:02.000000 MACS3-3.0.0b2/MACS3/fermi-lite/lib/arm/neon/st4.h
--rw-r--r--   0 runner    (1001) docker     (123)    18645 2023-06-23 21:34:02.000000 MACS3-3.0.0b2/MACS3/fermi-lite/lib/arm/neon/sub.h
--rw-r--r--   0 runner    (1001) docker     (123)     3912 2023-06-23 21:34:02.000000 MACS3-3.0.0b2/MACS3/fermi-lite/lib/arm/neon/subl.h
--rw-r--r--   0 runner    (1001) docker     (123)     7418 2023-06-23 21:34:02.000000 MACS3-3.0.0b2/MACS3/fermi-lite/lib/arm/neon/subw.h
--rw-r--r--   0 runner    (1001) docker     (123)     8041 2023-06-23 21:34:02.000000 MACS3-3.0.0b2/MACS3/fermi-lite/lib/arm/neon/subw_high.h
--rw-r--r--   0 runner    (1001) docker     (123)     7749 2023-06-23 21:34:02.000000 MACS3-3.0.0b2/MACS3/fermi-lite/lib/arm/neon/tbl.h
--rw-r--r--   0 runner    (1001) docker     (123)     9121 2023-06-23 21:34:02.000000 MACS3-3.0.0b2/MACS3/fermi-lite/lib/arm/neon/tbx.h
--rw-r--r--   0 runner    (1001) docker     (123)     7435 2023-06-23 21:34:02.000000 MACS3-3.0.0b2/MACS3/fermi-lite/lib/arm/neon/trn.h
--rw-r--r--   0 runner    (1001) docker     (123)    14460 2023-06-23 21:34:02.000000 MACS3-3.0.0b2/MACS3/fermi-lite/lib/arm/neon/trn1.h
--rw-r--r--   0 runner    (1001) docker     (123)    14595 2023-06-23 21:34:02.000000 MACS3-3.0.0b2/MACS3/fermi-lite/lib/arm/neon/trn2.h
--rw-r--r--   0 runner    (1001) docker     (123)    17552 2023-06-23 21:34:02.000000 MACS3-3.0.0b2/MACS3/fermi-lite/lib/arm/neon/tst.h
--rw-r--r--   0 runner    (1001) docker     (123)    26581 2023-06-23 21:34:02.000000 MACS3-3.0.0b2/MACS3/fermi-lite/lib/arm/neon/types.h
--rw-r--r--   0 runner    (1001) docker     (123)     9465 2023-06-23 21:34:02.000000 MACS3-3.0.0b2/MACS3/fermi-lite/lib/arm/neon/uqadd.h
--rw-r--r--   0 runner    (1001) docker     (123)     7435 2023-06-23 21:34:02.000000 MACS3-3.0.0b2/MACS3/fermi-lite/lib/arm/neon/uzp.h
--rw-r--r--   0 runner    (1001) docker     (123)    20856 2023-06-23 21:34:02.000000 MACS3-3.0.0b2/MACS3/fermi-lite/lib/arm/neon/uzp1.h
--rw-r--r--   0 runner    (1001) docker     (123)    21036 2023-06-23 21:34:02.000000 MACS3-3.0.0b2/MACS3/fermi-lite/lib/arm/neon/uzp2.h
--rw-r--r--   0 runner    (1001) docker     (123)     7435 2023-06-23 21:34:02.000000 MACS3-3.0.0b2/MACS3/fermi-lite/lib/arm/neon/zip.h
--rw-r--r--   0 runner    (1001) docker     (123)    19744 2023-06-23 21:34:02.000000 MACS3-3.0.0b2/MACS3/fermi-lite/lib/arm/neon/zip1.h
--rw-r--r--   0 runner    (1001) docker     (123)    20392 2023-06-23 21:34:02.000000 MACS3-3.0.0b2/MACS3/fermi-lite/lib/arm/neon/zip2.h
--rw-r--r--   0 runner    (1001) docker     (123)     4351 2023-06-23 21:34:02.000000 MACS3-3.0.0b2/MACS3/fermi-lite/lib/arm/neon.h
--rw-r--r--   0 runner    (1001) docker     (123)     9846 2023-06-23 21:34:02.000000 MACS3-3.0.0b2/MACS3/fermi-lite/lib/check.h
--rw-r--r--   0 runner    (1001) docker     (123)     3119 2023-06-23 21:34:02.000000 MACS3-3.0.0b2/MACS3/fermi-lite/lib/debug-trap.h
--rw-r--r--   0 runner    (1001) docker     (123)    74181 2023-06-23 21:34:02.000000 MACS3-3.0.0b2/MACS3/fermi-lite/lib/hedley.h
--rw-r--r--   0 runner    (1001) docker     (123)    17805 2023-06-23 21:34:02.000000 MACS3-3.0.0b2/MACS3/fermi-lite/lib/simde-align.h
--rw-r--r--   0 runner    (1001) docker     (123)    16472 2023-06-23 21:34:02.000000 MACS3-3.0.0b2/MACS3/fermi-lite/lib/simde-arch.h
--rw-r--r--   0 runner    (1001) docker     (123)    32588 2023-06-23 21:34:02.000000 MACS3-3.0.0b2/MACS3/fermi-lite/lib/simde-common.h
--rw-r--r--   0 runner    (1001) docker     (123)    18585 2023-06-23 21:34:02.000000 MACS3-3.0.0b2/MACS3/fermi-lite/lib/simde-constify.h
--rw-r--r--   0 runner    (1001) docker     (123)     5065 2023-06-23 21:34:02.000000 MACS3-3.0.0b2/MACS3/fermi-lite/lib/simde-detect-clang.h
--rw-r--r--   0 runner    (1001) docker     (123)    18236 2023-06-23 21:34:02.000000 MACS3-3.0.0b2/MACS3/fermi-lite/lib/simde-diagnostic.h
--rw-r--r--   0 runner    (1001) docker     (123)    17861 2023-06-23 21:34:02.000000 MACS3-3.0.0b2/MACS3/fermi-lite/lib/simde-features.h
--rw-r--r--   0 runner    (1001) docker     (123)    57737 2023-06-23 21:34:02.000000 MACS3-3.0.0b2/MACS3/fermi-lite/lib/simde-math.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 21:35:58.168008 MACS3-3.0.0b2/MACS3/fermi-lite/lib/x86/
--rw-r--r--   0 runner    (1001) docker     (123)   195250 2023-06-23 21:34:02.000000 MACS3-3.0.0b2/MACS3/fermi-lite/lib/x86/avx.h
--rw-r--r--   0 runner    (1001) docker     (123)   194448 2023-06-23 21:34:02.000000 MACS3-3.0.0b2/MACS3/fermi-lite/lib/x86/avx2.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 21:35:58.180009 MACS3-3.0.0b2/MACS3/fermi-lite/lib/x86/avx512/
--rw-r--r--   0 runner    (1001) docker     (123)     8026 2023-06-23 21:34:02.000000 MACS3-3.0.0b2/MACS3/fermi-lite/lib/x86/avx512/2intersect.h
--rw-r--r--   0 runner    (1001) docker     (123)    17914 2023-06-23 21:34:02.000000 MACS3-3.0.0b2/MACS3/fermi-lite/lib/x86/avx512/abs.h
--rw-r--r--   0 runner    (1001) docker     (123)    21097 2023-06-23 21:34:02.000000 MACS3-3.0.0b2/MACS3/fermi-lite/lib/x86/avx512/add.h
--rw-r--r--   0 runner    (1001) docker     (123)    13194 2023-06-23 21:34:02.000000 MACS3-3.0.0b2/MACS3/fermi-lite/lib/x86/avx512/adds.h
--rw-r--r--   0 runner    (1001) docker     (123)     9570 2023-06-23 21:34:02.000000 MACS3-3.0.0b2/MACS3/fermi-lite/lib/x86/avx512/and.h
--rw-r--r--   0 runner    (1001) docker     (123)     7564 2023-06-23 21:34:02.000000 MACS3-3.0.0b2/MACS3/fermi-lite/lib/x86/avx512/andnot.h
--rw-r--r--   0 runner    (1001) docker     (123)     8799 2023-06-23 21:34:02.000000 MACS3-3.0.0b2/MACS3/fermi-lite/lib/x86/avx512/avg.h
--rw-r--r--   0 runner    (1001) docker     (123)     9480 2023-06-23 21:34:02.000000 MACS3-3.0.0b2/MACS3/fermi-lite/lib/x86/avx512/blend.h
--rw-r--r--   0 runner    (1001) docker     (123)    29208 2023-06-23 21:34:02.000000 MACS3-3.0.0b2/MACS3/fermi-lite/lib/x86/avx512/broadcast.h
--rw-r--r--   0 runner    (1001) docker     (123)     9094 2023-06-23 21:34:02.000000 MACS3-3.0.0b2/MACS3/fermi-lite/lib/x86/avx512/cast.h
--rw-r--r--   0 runner    (1001) docker     (123)    23105 2023-06-23 21:34:02.000000 MACS3-3.0.0b2/MACS3/fermi-lite/lib/x86/avx512/cmp.h
--rw-r--r--   0 runner    (1001) docker     (123)     5959 2023-06-23 21:34:02.000000 MACS3-3.0.0b2/MACS3/fermi-lite/lib/x86/avx512/cmpeq.h
--rw-r--r--   0 runner    (1001) docker     (123)     3401 2023-06-23 21:34:02.000000 MACS3-3.0.0b2/MACS3/fermi-lite/lib/x86/avx512/cmpge.h
--rw-r--r--   0 runner    (1001) docker     (123)     6256 2023-06-23 21:34:02.000000 MACS3-3.0.0b2/MACS3/fermi-lite/lib/x86/avx512/cmpgt.h
--rw-r--r--   0 runner    (1001) docker     (123)     3352 2023-06-23 21:34:02.000000 MACS3-3.0.0b2/MACS3/fermi-lite/lib/x86/avx512/cmple.h
--rw-r--r--   0 runner    (1001) docker     (123)     4012 2023-06-23 21:34:02.000000 MACS3-3.0.0b2/MACS3/fermi-lite/lib/x86/avx512/cmplt.h
--rw-r--r--   0 runner    (1001) docker     (123)     3008 2023-06-23 21:34:02.000000 MACS3-3.0.0b2/MACS3/fermi-lite/lib/x86/avx512/copysign.h
--rw-r--r--   0 runner    (1001) docker     (123)     3959 2023-06-23 21:34:02.000000 MACS3-3.0.0b2/MACS3/fermi-lite/lib/x86/avx512/cvt.h
--rw-r--r--   0 runner    (1001) docker     (123)    23453 2023-06-23 21:34:02.000000 MACS3-3.0.0b2/MACS3/fermi-lite/lib/x86/avx512/cvts.h
--rw-r--r--   0 runner    (1001) docker     (123)     5289 2023-06-23 21:34:02.000000 MACS3-3.0.0b2/MACS3/fermi-lite/lib/x86/avx512/div.h
--rw-r--r--   0 runner    (1001) docker     (123)     8810 2023-06-23 21:34:02.000000 MACS3-3.0.0b2/MACS3/fermi-lite/lib/x86/avx512/extract.h
--rw-r--r--   0 runner    (1001) docker     (123)     4563 2023-06-23 21:34:02.000000 MACS3-3.0.0b2/MACS3/fermi-lite/lib/x86/avx512/fmadd.h
--rw-r--r--   0 runner    (1001) docker     (123)     3601 2023-06-23 21:34:02.000000 MACS3-3.0.0b2/MACS3/fermi-lite/lib/x86/avx512/fmsub.h
--rw-r--r--   0 runner    (1001) docker     (123)     3620 2023-06-23 21:34:02.000000 MACS3-3.0.0b2/MACS3/fermi-lite/lib/x86/avx512/fnmadd.h
--rw-r--r--   0 runner    (1001) docker     (123)     3620 2023-06-23 21:34:02.000000 MACS3-3.0.0b2/MACS3/fermi-lite/lib/x86/avx512/fnmsub.h
--rw-r--r--   0 runner    (1001) docker     (123)     7801 2023-06-23 21:34:02.000000 MACS3-3.0.0b2/MACS3/fermi-lite/lib/x86/avx512/insert.h
--rw-r--r--   0 runner    (1001) docker     (123)     5919 2023-06-23 21:34:02.000000 MACS3-3.0.0b2/MACS3/fermi-lite/lib/x86/avx512/kshift.h
--rw-r--r--   0 runner    (1001) docker     (123)     2556 2023-06-23 21:34:02.000000 MACS3-3.0.0b2/MACS3/fermi-lite/lib/x86/avx512/load.h
--rw-r--r--   0 runner    (1001) docker     (123)     7347 2023-06-23 21:34:02.000000 MACS3-3.0.0b2/MACS3/fermi-lite/lib/x86/avx512/loadu.h
--rw-r--r--   0 runner    (1001) docker     (123)     7454 2023-06-23 21:34:02.000000 MACS3-3.0.0b2/MACS3/fermi-lite/lib/x86/avx512/lzcnt.h
--rw-r--r--   0 runner    (1001) docker     (123)     5652 2023-06-23 21:34:02.000000 MACS3-3.0.0b2/MACS3/fermi-lite/lib/x86/avx512/madd.h
--rw-r--r--   0 runner    (1001) docker     (123)     6089 2023-06-23 21:34:02.000000 MACS3-3.0.0b2/MACS3/fermi-lite/lib/x86/avx512/maddubs.h
--rw-r--r--   0 runner    (1001) docker     (123)    18597 2023-06-23 21:34:02.000000 MACS3-3.0.0b2/MACS3/fermi-lite/lib/x86/avx512/max.h
--rw-r--r--   0 runner    (1001) docker     (123)    18599 2023-06-23 21:34:02.000000 MACS3-3.0.0b2/MACS3/fermi-lite/lib/x86/avx512/min.h
--rw-r--r--   0 runner    (1001) docker     (123)    30273 2023-06-23 21:34:02.000000 MACS3-3.0.0b2/MACS3/fermi-lite/lib/x86/avx512/mov.h
--rw-r--r--   0 runner    (1001) docker     (123)    11926 2023-06-23 21:34:02.000000 MACS3-3.0.0b2/MACS3/fermi-lite/lib/x86/avx512/mov_mask.h
--rw-r--r--   0 runner    (1001) docker     (123)    15715 2023-06-23 21:34:02.000000 MACS3-3.0.0b2/MACS3/fermi-lite/lib/x86/avx512/movm.h
--rw-r--r--   0 runner    (1001) docker     (123)     9151 2023-06-23 21:34:02.000000 MACS3-3.0.0b2/MACS3/fermi-lite/lib/x86/avx512/mul.h
--rw-r--r--   0 runner    (1001) docker     (123)     2282 2023-06-23 21:34:02.000000 MACS3-3.0.0b2/MACS3/fermi-lite/lib/x86/avx512/mulhi.h
--rw-r--r--   0 runner    (1001) docker     (123)     2272 2023-06-23 21:34:02.000000 MACS3-3.0.0b2/MACS3/fermi-lite/lib/x86/avx512/mulhrs.h
--rw-r--r--   0 runner    (1001) docker     (123)     3842 2023-06-23 21:34:02.000000 MACS3-3.0.0b2/MACS3/fermi-lite/lib/x86/avx512/mullo.h
--rw-r--r--   0 runner    (1001) docker     (123)     2639 2023-06-23 21:34:02.000000 MACS3-3.0.0b2/MACS3/fermi-lite/lib/x86/avx512/negate.h
--rw-r--r--   0 runner    (1001) docker     (123)     7993 2023-06-23 21:34:02.000000 MACS3-3.0.0b2/MACS3/fermi-lite/lib/x86/avx512/or.h
--rw-r--r--   0 runner    (1001) docker     (123)     6819 2023-06-23 21:34:02.000000 MACS3-3.0.0b2/MACS3/fermi-lite/lib/x86/avx512/packs.h
--rw-r--r--   0 runner    (1001) docker     (123)     6833 2023-06-23 21:34:02.000000 MACS3-3.0.0b2/MACS3/fermi-lite/lib/x86/avx512/packus.h
--rw-r--r--   0 runner    (1001) docker     (123)    69829 2023-06-23 21:34:02.000000 MACS3-3.0.0b2/MACS3/fermi-lite/lib/x86/avx512/permutex2var.h
--rw-r--r--   0 runner    (1001) docker     (123)    49807 2023-06-23 21:34:02.000000 MACS3-3.0.0b2/MACS3/fermi-lite/lib/x86/avx512/permutexvar.h
--rw-r--r--   0 runner    (1001) docker     (123)     2638 2023-06-23 21:34:02.000000 MACS3-3.0.0b2/MACS3/fermi-lite/lib/x86/avx512/sad.h
--rw-r--r--   0 runner    (1001) docker     (123)    15045 2023-06-23 21:34:02.000000 MACS3-3.0.0b2/MACS3/fermi-lite/lib/x86/avx512/set.h
--rw-r--r--   0 runner    (1001) docker     (123)     9209 2023-06-23 21:34:02.000000 MACS3-3.0.0b2/MACS3/fermi-lite/lib/x86/avx512/set1.h
--rw-r--r--   0 runner    (1001) docker     (123)     3705 2023-06-23 21:34:02.000000 MACS3-3.0.0b2/MACS3/fermi-lite/lib/x86/avx512/set4.h
--rw-r--r--   0 runner    (1001) docker     (123)     2104 2023-06-23 21:34:02.000000 MACS3-3.0.0b2/MACS3/fermi-lite/lib/x86/avx512/setone.h
--rw-r--r--   0 runner    (1001) docker     (123)     4723 2023-06-23 21:34:02.000000 MACS3-3.0.0b2/MACS3/fermi-lite/lib/x86/avx512/setr.h
--rw-r--r--   0 runner    (1001) docker     (123)     3735 2023-06-23 21:34:02.000000 MACS3-3.0.0b2/MACS3/fermi-lite/lib/x86/avx512/setr4.h
--rw-r--r--   0 runner    (1001) docker     (123)     2924 2023-06-23 21:34:02.000000 MACS3-3.0.0b2/MACS3/fermi-lite/lib/x86/avx512/setzero.h
--rw-r--r--   0 runner    (1001) docker     (123)     7868 2023-06-23 21:34:02.000000 MACS3-3.0.0b2/MACS3/fermi-lite/lib/x86/avx512/shuffle.h
--rw-r--r--   0 runner    (1001) docker     (123)     8169 2023-06-23 21:34:02.000000 MACS3-3.0.0b2/MACS3/fermi-lite/lib/x86/avx512/sll.h
--rw-r--r--   0 runner    (1001) docker     (123)     6812 2023-06-23 21:34:02.000000 MACS3-3.0.0b2/MACS3/fermi-lite/lib/x86/avx512/slli.h
--rw-r--r--   0 runner    (1001) docker     (123)     2360 2023-06-23 21:34:02.000000 MACS3-3.0.0b2/MACS3/fermi-lite/lib/x86/avx512/sllv.h
--rw-r--r--   0 runner    (1001) docker     (123)     3977 2023-06-23 21:34:02.000000 MACS3-3.0.0b2/MACS3/fermi-lite/lib/x86/avx512/sqrt.h
--rw-r--r--   0 runner    (1001) docker     (123)     2684 2023-06-23 21:34:02.000000 MACS3-3.0.0b2/MACS3/fermi-lite/lib/x86/avx512/sra.h
--rw-r--r--   0 runner    (1001) docker     (123)     2340 2023-06-23 21:34:02.000000 MACS3-3.0.0b2/MACS3/fermi-lite/lib/x86/avx512/srai.h
--rw-r--r--   0 runner    (1001) docker     (123)     2271 2023-06-23 21:34:02.000000 MACS3-3.0.0b2/MACS3/fermi-lite/lib/x86/avx512/srav.h
--rw-r--r--   0 runner    (1001) docker     (123)     6928 2023-06-23 21:34:02.000000 MACS3-3.0.0b2/MACS3/fermi-lite/lib/x86/avx512/srl.h
--rw-r--r--   0 runner    (1001) docker     (123)     6593 2023-06-23 21:34:02.000000 MACS3-3.0.0b2/MACS3/fermi-lite/lib/x86/avx512/srli.h
--rw-r--r--   0 runner    (1001) docker     (123)     9460 2023-06-23 21:34:02.000000 MACS3-3.0.0b2/MACS3/fermi-lite/lib/x86/avx512/srlv.h
--rw-r--r--   0 runner    (1001) docker     (123)     3507 2023-06-23 21:34:02.000000 MACS3-3.0.0b2/MACS3/fermi-lite/lib/x86/avx512/store.h
--rw-r--r--   0 runner    (1001) docker     (123)     3429 2023-06-23 21:34:02.000000 MACS3-3.0.0b2/MACS3/fermi-lite/lib/x86/avx512/storeu.h
--rw-r--r--   0 runner    (1001) docker     (123)    10888 2023-06-23 21:34:02.000000 MACS3-3.0.0b2/MACS3/fermi-lite/lib/x86/avx512/sub.h
--rw-r--r--   0 runner    (1001) docker     (123)     7107 2023-06-23 21:34:02.000000 MACS3-3.0.0b2/MACS3/fermi-lite/lib/x86/avx512/subs.h
--rw-r--r--   0 runner    (1001) docker     (123)     6297 2023-06-23 21:34:02.000000 MACS3-3.0.0b2/MACS3/fermi-lite/lib/x86/avx512/test.h
--rw-r--r--   0 runner    (1001) docker     (123)    17809 2023-06-23 21:34:02.000000 MACS3-3.0.0b2/MACS3/fermi-lite/lib/x86/avx512/types.h
--rw-r--r--   0 runner    (1001) docker     (123)    13394 2023-06-23 21:34:02.000000 MACS3-3.0.0b2/MACS3/fermi-lite/lib/x86/avx512/unpackhi.h
--rw-r--r--   0 runner    (1001) docker     (123)     3886 2023-06-23 21:34:02.000000 MACS3-3.0.0b2/MACS3/fermi-lite/lib/x86/avx512/unpacklo.h
--rw-r--r--   0 runner    (1001) docker     (123)     8662 2023-06-23 21:34:02.000000 MACS3-3.0.0b2/MACS3/fermi-lite/lib/x86/avx512/xor.h
--rw-r--r--   0 runner    (1001) docker     (123)     2426 2023-06-23 21:34:02.000000 MACS3-3.0.0b2/MACS3/fermi-lite/lib/x86/avx512/xorsign.h
--rw-r--r--   0 runner    (1001) docker     (123)     3227 2023-06-23 21:34:02.000000 MACS3-3.0.0b2/MACS3/fermi-lite/lib/x86/avx512.h
--rw-r--r--   0 runner    (1001) docker     (123)    15656 2023-06-23 21:34:02.000000 MACS3-3.0.0b2/MACS3/fermi-lite/lib/x86/clmul.h
--rw-r--r--   0 runner    (1001) docker     (123)    21337 2023-06-23 21:34:02.000000 MACS3-3.0.0b2/MACS3/fermi-lite/lib/x86/fma.h
--rw-r--r--   0 runner    (1001) docker     (123)    31945 2023-06-23 21:34:02.000000 MACS3-3.0.0b2/MACS3/fermi-lite/lib/x86/gfni.h
--rw-r--r--   0 runner    (1001) docker     (123)    76602 2023-06-23 21:34:02.000000 MACS3-3.0.0b2/MACS3/fermi-lite/lib/x86/mmx.h
--rw-r--r--   0 runner    (1001) docker     (123)   144373 2023-06-23 21:34:02.000000 MACS3-3.0.0b2/MACS3/fermi-lite/lib/x86/sse.h
--rw-r--r--   0 runner    (1001) docker     (123)   241454 2023-06-23 21:34:02.000000 MACS3-3.0.0b2/MACS3/fermi-lite/lib/x86/sse2.h
--rw-r--r--   0 runner    (1001) docker     (123)    16133 2023-06-23 21:34:02.000000 MACS3-3.0.0b2/MACS3/fermi-lite/lib/x86/sse3.h
--rw-r--r--   0 runner    (1001) docker     (123)    75653 2023-06-23 21:34:02.000000 MACS3-3.0.0b2/MACS3/fermi-lite/lib/x86/sse4.1.h
--rw-r--r--   0 runner    (1001) docker     (123)    12626 2023-06-23 21:34:02.000000 MACS3-3.0.0b2/MACS3/fermi-lite/lib/x86/sse4.2.h
--rw-r--r--   0 runner    (1001) docker     (123)    35506 2023-06-23 21:34:02.000000 MACS3-3.0.0b2/MACS3/fermi-lite/lib/x86/ssse3.h
--rw-r--r--   0 runner    (1001) docker     (123)   398077 2023-06-23 21:34:02.000000 MACS3-3.0.0b2/MACS3/fermi-lite/lib/x86/svml.h
--rw-r--r--   0 runner    (1001) docker     (123)    17555 2023-06-23 21:33:58.000000 MACS3-3.0.0b2/MACS3/fermi-lite/mag.c
--rw-r--r--   0 runner    (1001) docker     (123)     1962 2023-06-23 21:33:58.000000 MACS3-3.0.0b2/MACS3/fermi-lite/mag.h
--rw-r--r--   0 runner    (1001) docker     (123)     7850 2023-06-23 21:33:58.000000 MACS3-3.0.0b2/MACS3/fermi-lite/misc.c
--rw-r--r--   0 runner    (1001) docker     (123)     8554 2023-06-23 21:33:58.000000 MACS3-3.0.0b2/MACS3/fermi-lite/mrope.c
--rw-r--r--   0 runner    (1001) docker     (123)     2694 2023-06-23 21:33:58.000000 MACS3-3.0.0b2/MACS3/fermi-lite/mrope.h
--rw-r--r--   0 runner    (1001) docker     (123)    13226 2023-06-23 21:33:58.000000 MACS3-3.0.0b2/MACS3/fermi-lite/rld0.c
--rw-r--r--   0 runner    (1001) docker     (123)     4296 2023-06-23 21:33:58.000000 MACS3-3.0.0b2/MACS3/fermi-lite/rld0.h
--rw-r--r--   0 runner    (1001) docker     (123)     4821 2023-06-23 21:33:58.000000 MACS3-3.0.0b2/MACS3/fermi-lite/rle.c
--rw-r--r--   0 runner    (1001) docker     (123)     1941 2023-06-23 21:33:58.000000 MACS3-3.0.0b2/MACS3/fermi-lite/rle.h
--rw-r--r--   0 runner    (1001) docker     (123)     6965 2023-06-23 21:33:58.000000 MACS3-3.0.0b2/MACS3/fermi-lite/rope.c
--rw-r--r--   0 runner    (1001) docker     (123)     1428 2023-06-23 21:33:58.000000 MACS3-3.0.0b2/MACS3/fermi-lite/rope.h
--rw-r--r--   0 runner    (1001) docker     (123)    15372 2023-06-23 21:33:58.000000 MACS3-3.0.0b2/MACS3/fermi-lite/unitig.c
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 21:35:58.128005 MACS3-3.0.0b2/MACS3.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     7613 2023-06-23 21:35:58.000000 MACS3-3.0.0b2/MACS3.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    11603 2023-06-23 21:35:58.000000 MACS3-3.0.0b2/MACS3.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-23 21:35:58.000000 MACS3-3.0.0b2/MACS3.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-06-23 21:35:58.000000 MACS3-3.0.0b2/MACS3.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-06-23 21:35:58.000000 MACS3-3.0.0b2/MACS3.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      396 2023-06-23 21:33:58.000000 MACS3-3.0.0b2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     7613 2023-06-23 21:35:58.180009 MACS3-3.0.0b2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     6721 2023-06-23 21:33:58.000000 MACS3-3.0.0b2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 21:35:58.180009 MACS3-3.0.0b2/bin/
--rw-r--r--   0 runner    (1001) docker     (123)    98279 2023-06-23 21:33:58.000000 MACS3-3.0.0b2/bin/macs3
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 21:35:58.180009 MACS3-3.0.0b2/docs/
--rw-r--r--   0 runner    (1001) docker     (123)     5815 2023-06-23 21:33:58.000000 MACS3-3.0.0b2/docs/INSTALL.md
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-23 21:33:58.000000 MACS3-3.0.0b2/docs/bdgbroadcall.md
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-23 21:33:58.000000 MACS3-3.0.0b2/docs/bdgcmp.md
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-23 21:33:58.000000 MACS3-3.0.0b2/docs/bdgdiff.md
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-23 21:33:58.000000 MACS3-3.0.0b2/docs/bdgopt.md
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-23 21:33:58.000000 MACS3-3.0.0b2/docs/bdgpeakcall.md
--rw-r--r--   0 runner    (1001) docker     (123)    16724 2023-06-23 21:33:58.000000 MACS3-3.0.0b2/docs/callpeak.md
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-23 21:33:58.000000 MACS3-3.0.0b2/docs/filterdup.md
--rw-r--r--   0 runner    (1001) docker     (123)     8564 2023-06-23 21:33:58.000000 MACS3-3.0.0b2/docs/hmmratac.md
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-23 21:33:58.000000 MACS3-3.0.0b2/docs/main.md
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-23 21:33:58.000000 MACS3-3.0.0b2/docs/pileup.md
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-23 21:33:58.000000 MACS3-3.0.0b2/docs/predictd.md
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-23 21:33:58.000000 MACS3-3.0.0b2/docs/qa.md
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-23 21:33:58.000000 MACS3-3.0.0b2/docs/randsample.md
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-23 21:33:58.000000 MACS3-3.0.0b2/docs/refinepeak.md
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-23 21:33:58.000000 MACS3-3.0.0b2/docs/testing_in_docker.md
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-23 21:33:58.000000 MACS3-3.0.0b2/docs/tutorial.md
--rw-r--r--   0 runner    (1001) docker     (123)     1942 2023-06-23 21:33:58.000000 MACS3-3.0.0b2/make_docker_base.sh
--rw-r--r--   0 runner    (1001) docker     (123)      125 2023-06-23 21:33:58.000000 MACS3-3.0.0b2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       82 2023-06-23 21:33:58.000000 MACS3-3.0.0b2/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-23 21:35:58.180009 MACS3-3.0.0b2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     9217 2023-06-23 21:33:58.000000 MACS3-3.0.0b2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 16:49:27.494857 MACS3-3.0.0b3/
+-rw-r--r--   0 runner    (1001) docker     (123)    82494 2023-07-30 16:47:10.000000 MACS3-3.0.0b3/ChangeLog
+-rw-r--r--   0 runner    (1001) docker     (123)     1526 2023-07-30 16:47:10.000000 MACS3-3.0.0b3/LICENSE
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 16:49:27.450857 MACS3-3.0.0b3/MACS3/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 16:49:27.454857 MACS3-3.0.0b3/MACS3/Commands/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-30 16:47:10.000000 MACS3-3.0.0b3/MACS3/Commands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1876 2023-07-30 16:47:10.000000 MACS3-3.0.0b3/MACS3/Commands/bdgbroadcall_cmd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3403 2023-07-30 16:47:10.000000 MACS3-3.0.0b3/MACS3/Commands/bdgcmp_cmd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4118 2023-07-30 16:47:10.000000 MACS3-3.0.0b3/MACS3/Commands/bdgdiff_cmd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2105 2023-07-30 16:47:10.000000 MACS3-3.0.0b3/MACS3/Commands/bdgopt_cmd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2491 2023-07-30 16:47:10.000000 MACS3-3.0.0b3/MACS3/Commands/bdgpeakcall_cmd.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17848 2023-07-30 16:47:10.000000 MACS3-3.0.0b3/MACS3/Commands/callpeak_cmd.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18078 2023-07-30 16:47:10.000000 MACS3-3.0.0b3/MACS3/Commands/callvar_cmd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1632 2023-07-30 16:47:10.000000 MACS3-3.0.0b3/MACS3/Commands/cmbreps_cmd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9693 2023-07-30 16:47:10.000000 MACS3-3.0.0b3/MACS3/Commands/diffpeak_cmd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4563 2023-07-30 16:47:10.000000 MACS3-3.0.0b3/MACS3/Commands/filterdup_cmd.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29326 2023-07-30 16:47:10.000000 MACS3-3.0.0b3/MACS3/Commands/hmmratac_cmd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3755 2023-07-30 16:47:10.000000 MACS3-3.0.0b3/MACS3/Commands/pileup_cmd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4092 2023-07-30 16:47:10.000000 MACS3-3.0.0b3/MACS3/Commands/predictd_cmd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3873 2023-07-30 16:47:10.000000 MACS3-3.0.0b3/MACS3/Commands/randsample_cmd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3955 2023-07-30 16:47:10.000000 MACS3-3.0.0b3/MACS3/Commands/refinepeak_cmd.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 16:49:27.454857 MACS3-3.0.0b3/MACS3/IO/
+-rw-r--r--   0 runner    (1001) docker     (123)    25603 2023-07-30 16:47:10.000000 MACS3-3.0.0b3/MACS3/IO/BAM.pyx
+-rw-r--r--   0 runner    (1001) docker     (123)     2538 2023-07-30 16:47:10.000000 MACS3-3.0.0b3/MACS3/IO/BedGraphIO.pyx
+-rw-r--r--   0 runner    (1001) docker     (123)    10381 2023-07-30 16:47:10.000000 MACS3-3.0.0b3/MACS3/IO/OutputWriter.py
+-rw-r--r--   0 runner    (1001) docker     (123)    52515 2023-07-30 16:47:10.000000 MACS3-3.0.0b3/MACS3/IO/Parser.pyx
+-rw-r--r--   0 runner    (1001) docker     (123)    54269 2023-07-30 16:47:10.000000 MACS3-3.0.0b3/MACS3/IO/PeakIO.pyx
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-30 16:47:10.000000 MACS3-3.0.0b3/MACS3/IO/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 16:49:27.458857 MACS3-3.0.0b3/MACS3/Signal/
+-rw-r--r--   0 runner    (1001) docker     (123)    48106 2023-07-30 16:47:10.000000 MACS3-3.0.0b3/MACS3/Signal/BedGraph.pyx
+-rw-r--r--   0 runner    (1001) docker     (123)    76301 2023-07-30 16:47:10.000000 MACS3-3.0.0b3/MACS3/Signal/CallPeakUnit.pyx
+-rw-r--r--   0 runner    (1001) docker     (123)    21780 2023-07-30 16:47:10.000000 MACS3-3.0.0b3/MACS3/Signal/FixWidthTrack.pyx
+-rw-r--r--   0 runner    (1001) docker     (123)    11209 2023-07-30 16:47:10.000000 MACS3-3.0.0b3/MACS3/Signal/HMMR_EM.pyx
+-rw-r--r--   0 runner    (1001) docker     (123)     4209 2023-07-30 16:47:10.000000 MACS3-3.0.0b3/MACS3/Signal/HMMR_HMM.pyx
+-rw-r--r--   0 runner    (1001) docker     (123)     8363 2023-07-30 16:47:10.000000 MACS3-3.0.0b3/MACS3/Signal/HMMR_Signal_Processing.pyx
+-rw-r--r--   0 runner    (1001) docker     (123)    22046 2023-07-30 16:47:10.000000 MACS3-3.0.0b3/MACS3/Signal/PairedEndTrack.pyx
+-rw-r--r--   0 runner    (1001) docker     (123)    17522 2023-07-30 16:47:10.000000 MACS3-3.0.0b3/MACS3/Signal/PeakDetect.pyx
+-rw-r--r--   0 runner    (1001) docker     (123)    16813 2023-07-30 16:47:10.000000 MACS3-3.0.0b3/MACS3/Signal/PeakModel.pyx
+-rw-r--r--   0 runner    (1001) docker     (123)    12726 2023-07-30 16:47:10.000000 MACS3-3.0.0b3/MACS3/Signal/PeakVariants.pyx
+-rw-r--r--   0 runner    (1001) docker     (123)    23810 2023-07-30 16:47:10.000000 MACS3-3.0.0b3/MACS3/Signal/Pileup.pyx
+-rw-r--r--   0 runner    (1001) docker     (123)     7898 2023-07-30 16:47:10.000000 MACS3-3.0.0b3/MACS3/Signal/PileupV2.pyx
+-rw-r--r--   0 runner    (1001) docker     (123)    27685 2023-07-30 16:47:10.000000 MACS3-3.0.0b3/MACS3/Signal/PosReadsInfo.pyx
+-rw-r--r--   0 runner    (1001) docker     (123)    24866 2023-07-30 16:47:10.000000 MACS3-3.0.0b3/MACS3/Signal/Prob.pyx
+-rw-r--r--   0 runner    (1001) docker     (123)    35761 2023-07-30 16:47:10.000000 MACS3-3.0.0b3/MACS3/Signal/RACollection.pyx
+-rw-r--r--   0 runner    (1001) docker     (123)    19506 2023-07-30 16:47:10.000000 MACS3-3.0.0b3/MACS3/Signal/ReadAlignment.pyx
+-rw-r--r--   0 runner    (1001) docker     (123)    10155 2023-07-30 16:47:10.000000 MACS3-3.0.0b3/MACS3/Signal/Region.pyx
+-rw-r--r--   0 runner    (1001) docker     (123)    58541 2023-07-30 16:47:10.000000 MACS3-3.0.0b3/MACS3/Signal/ScoreTrack.pyx
+-rw-r--r--   0 runner    (1001) docker     (123)    13210 2023-07-30 16:47:10.000000 MACS3-3.0.0b3/MACS3/Signal/SignalProcessing.pyx
+-rw-r--r--   0 runner    (1001) docker     (123)    12281 2023-07-30 16:47:10.000000 MACS3-3.0.0b3/MACS3/Signal/UnitigRACollection.pyx
+-rw-r--r--   0 runner    (1001) docker     (123)    13764 2023-07-30 16:47:10.000000 MACS3-3.0.0b3/MACS3/Signal/VariantStat.pyx
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-30 16:47:10.000000 MACS3-3.0.0b3/MACS3/Signal/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13930 2023-07-30 16:47:10.000000 MACS3-3.0.0b3/MACS3/Signal/cPosValCalculation.c
+-rw-r--r--   0 runner    (1001) docker     (123)     1786 2023-07-30 16:47:10.000000 MACS3-3.0.0b3/MACS3/Signal/cPosValCalculation.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1248 2023-07-30 16:47:10.000000 MACS3-3.0.0b3/MACS3/Signal/cPosValCalculation.pxd
+-rw-r--r--   0 runner    (1001) docker     (123)     9826 2023-07-30 16:47:10.000000 MACS3-3.0.0b3/MACS3/Signal/swalign.c
+-rw-r--r--   0 runner    (1001) docker     (123)     2358 2023-07-30 16:47:10.000000 MACS3-3.0.0b3/MACS3/Signal/swalign.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 16:49:27.458857 MACS3-3.0.0b3/MACS3/Utilities/
+-rw-r--r--   0 runner    (1001) docker     (123)      661 2023-07-30 16:47:10.000000 MACS3-3.0.0b3/MACS3/Utilities/Constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1079 2023-07-30 16:47:10.000000 MACS3-3.0.0b3/MACS3/Utilities/Logger.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31951 2023-07-30 16:47:10.000000 MACS3-3.0.0b3/MACS3/Utilities/OptValidator.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-30 16:47:10.000000 MACS3-3.0.0b3/MACS3/Utilities/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-07-30 16:47:10.000000 MACS3-3.0.0b3/MACS3/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 16:49:27.462857 MACS3-3.0.0b3/MACS3/fermi-lite/
+-rw-r--r--   0 runner    (1001) docker     (123)    19571 2023-07-30 16:47:10.000000 MACS3-3.0.0b3/MACS3/fermi-lite/bfc.c
+-rw-r--r--   0 runner    (1001) docker     (123)     1181 2023-07-30 16:47:10.000000 MACS3-3.0.0b3/MACS3/fermi-lite/bseq.c
+-rw-r--r--   0 runner    (1001) docker     (123)    12235 2023-07-30 16:47:10.000000 MACS3-3.0.0b3/MACS3/fermi-lite/bubble.c
+-rw-r--r--   0 runner    (1001) docker     (123)     2271 2023-07-30 16:47:10.000000 MACS3-3.0.0b3/MACS3/fermi-lite/example.c
+-rw-r--r--   0 runner    (1001) docker     (123)     5083 2023-07-30 16:47:10.000000 MACS3-3.0.0b3/MACS3/fermi-lite/fml.h
+-rw-r--r--   0 runner    (1001) docker     (123)     3085 2023-07-30 16:47:10.000000 MACS3-3.0.0b3/MACS3/fermi-lite/htab.c
+-rw-r--r--   0 runner    (1001) docker     (123)      622 2023-07-30 16:47:10.000000 MACS3-3.0.0b3/MACS3/fermi-lite/htab.h
+-rw-r--r--   0 runner    (1001) docker     (123)      444 2023-07-30 16:47:10.000000 MACS3-3.0.0b3/MACS3/fermi-lite/internal.h
+-rw-r--r--   0 runner    (1001) docker     (123)    21102 2023-07-30 16:47:10.000000 MACS3-3.0.0b3/MACS3/fermi-lite/khash.h
+-rw-r--r--   0 runner    (1001) docker     (123)     2880 2023-07-30 16:47:10.000000 MACS3-3.0.0b3/MACS3/fermi-lite/kmer.h
+-rw-r--r--   0 runner    (1001) docker     (123)     8739 2023-07-30 16:47:10.000000 MACS3-3.0.0b3/MACS3/fermi-lite/kseq.h
+-rw-r--r--   0 runner    (1001) docker     (123)    10635 2023-07-30 16:47:10.000000 MACS3-3.0.0b3/MACS3/fermi-lite/ksort.h
+-rw-r--r--   0 runner    (1001) docker     (123)     4437 2023-07-30 16:47:10.000000 MACS3-3.0.0b3/MACS3/fermi-lite/kstring.h
+-rw-r--r--   0 runner    (1001) docker     (123)    12337 2023-07-30 16:47:10.000000 MACS3-3.0.0b3/MACS3/fermi-lite/ksw.c
+-rw-r--r--   0 runner    (1001) docker     (123)     2485 2023-07-30 16:47:10.000000 MACS3-3.0.0b3/MACS3/fermi-lite/ksw.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1556 2023-07-30 16:47:10.000000 MACS3-3.0.0b3/MACS3/fermi-lite/kthread.c
+-rw-r--r--   0 runner    (1001) docker     (123)     3289 2023-07-30 16:47:10.000000 MACS3-3.0.0b3/MACS3/fermi-lite/kvec.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 16:49:27.462857 MACS3-3.0.0b3/MACS3/fermi-lite/lib/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 16:49:27.462857 MACS3-3.0.0b3/MACS3/fermi-lite/lib/arm/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 16:49:27.478857 MACS3-3.0.0b3/MACS3/fermi-lite/lib/arm/neon/
+-rw-r--r--   0 runner    (1001) docker     (123)     6276 2023-07-30 16:47:14.000000 MACS3-3.0.0b3/MACS3/fermi-lite/lib/arm/neon/aba.h
+-rw-r--r--   0 runner    (1001) docker     (123)    10687 2023-07-30 16:47:14.000000 MACS3-3.0.0b3/MACS3/fermi-lite/lib/arm/neon/abd.h
+-rw-r--r--   0 runner    (1001) docker     (123)     4266 2023-07-30 16:47:14.000000 MACS3-3.0.0b3/MACS3/fermi-lite/lib/arm/neon/abdl.h
+-rw-r--r--   0 runner    (1001) docker     (123)    12280 2023-07-30 16:47:14.000000 MACS3-3.0.0b3/MACS3/fermi-lite/lib/arm/neon/abs.h
+-rw-r--r--   0 runner    (1001) docker     (123)    18439 2023-07-30 16:47:14.000000 MACS3-3.0.0b3/MACS3/fermi-lite/lib/arm/neon/add.h
+-rw-r--r--   0 runner    (1001) docker     (123)     3912 2023-07-30 16:47:14.000000 MACS3-3.0.0b3/MACS3/fermi-lite/lib/arm/neon/addl.h
+-rw-r--r--   0 runner    (1001) docker     (123)     4141 2023-07-30 16:47:14.000000 MACS3-3.0.0b3/MACS3/fermi-lite/lib/arm/neon/addl_high.h
+-rw-r--r--   0 runner    (1001) docker     (123)     8399 2023-07-30 16:47:14.000000 MACS3-3.0.0b3/MACS3/fermi-lite/lib/arm/neon/addlv.h
+-rw-r--r--   0 runner    (1001) docker     (123)    10476 2023-07-30 16:47:14.000000 MACS3-3.0.0b3/MACS3/fermi-lite/lib/arm/neon/addv.h
+-rw-r--r--   0 runner    (1001) docker     (123)     7501 2023-07-30 16:47:14.000000 MACS3-3.0.0b3/MACS3/fermi-lite/lib/arm/neon/addw.h
+-rw-r--r--   0 runner    (1001) docker     (123)     6724 2023-07-30 16:47:14.000000 MACS3-3.0.0b3/MACS3/fermi-lite/lib/arm/neon/addw_high.h
+-rw-r--r--   0 runner    (1001) docker     (123)    15830 2023-07-30 16:47:14.000000 MACS3-3.0.0b3/MACS3/fermi-lite/lib/arm/neon/and.h
+-rw-r--r--   0 runner    (1001) docker     (123)    13752 2023-07-30 16:47:14.000000 MACS3-3.0.0b3/MACS3/fermi-lite/lib/arm/neon/bic.h
+-rw-r--r--   0 runner    (1001) docker     (123)    14767 2023-07-30 16:47:14.000000 MACS3-3.0.0b3/MACS3/fermi-lite/lib/arm/neon/bsl.h
+-rw-r--r--   0 runner    (1001) docker     (123)     4665 2023-07-30 16:47:14.000000 MACS3-3.0.0b3/MACS3/fermi-lite/lib/arm/neon/cagt.h
+-rw-r--r--   0 runner    (1001) docker     (123)    21370 2023-07-30 16:47:14.000000 MACS3-3.0.0b3/MACS3/fermi-lite/lib/arm/neon/ceq.h
+-rw-r--r--   0 runner    (1001) docker     (123)     9095 2023-07-30 16:47:14.000000 MACS3-3.0.0b3/MACS3/fermi-lite/lib/arm/neon/ceqz.h
+-rw-r--r--   0 runner    (1001) docker     (123)    22658 2023-07-30 16:47:14.000000 MACS3-3.0.0b3/MACS3/fermi-lite/lib/arm/neon/cge.h
+-rw-r--r--   0 runner    (1001) docker     (123)    11884 2023-07-30 16:47:14.000000 MACS3-3.0.0b3/MACS3/fermi-lite/lib/arm/neon/cgez.h
+-rw-r--r--   0 runner    (1001) docker     (123)    22278 2023-07-30 16:47:14.000000 MACS3-3.0.0b3/MACS3/fermi-lite/lib/arm/neon/cgt.h
+-rw-r--r--   0 runner    (1001) docker     (123)    11902 2023-07-30 16:47:14.000000 MACS3-3.0.0b3/MACS3/fermi-lite/lib/arm/neon/cgtz.h
+-rw-r--r--   0 runner    (1001) docker     (123)    22658 2023-07-30 16:47:14.000000 MACS3-3.0.0b3/MACS3/fermi-lite/lib/arm/neon/cle.h
+-rw-r--r--   0 runner    (1001) docker     (123)    11884 2023-07-30 16:47:14.000000 MACS3-3.0.0b3/MACS3/fermi-lite/lib/arm/neon/clez.h
+-rw-r--r--   0 runner    (1001) docker     (123)     4854 2023-07-30 16:47:14.000000 MACS3-3.0.0b3/MACS3/fermi-lite/lib/arm/neon/cls.h
+-rw-r--r--   0 runner    (1001) docker     (123)    22158 2023-07-30 16:47:14.000000 MACS3-3.0.0b3/MACS3/fermi-lite/lib/arm/neon/clt.h
+-rw-r--r--   0 runner    (1001) docker     (123)     7771 2023-07-30 16:47:14.000000 MACS3-3.0.0b3/MACS3/fermi-lite/lib/arm/neon/cltz.h
+-rw-r--r--   0 runner    (1001) docker     (123)    12387 2023-07-30 16:47:14.000000 MACS3-3.0.0b3/MACS3/fermi-lite/lib/arm/neon/clz.h
+-rw-r--r--   0 runner    (1001) docker     (123)     4376 2023-07-30 16:47:14.000000 MACS3-3.0.0b3/MACS3/fermi-lite/lib/arm/neon/cnt.h
+-rw-r--r--   0 runner    (1001) docker     (123)    11610 2023-07-30 16:47:14.000000 MACS3-3.0.0b3/MACS3/fermi-lite/lib/arm/neon/combine.h
+-rw-r--r--   0 runner    (1001) docker     (123)     5174 2023-07-30 16:47:14.000000 MACS3-3.0.0b3/MACS3/fermi-lite/lib/arm/neon/create.h
+-rw-r--r--   0 runner    (1001) docker     (123)    15180 2023-07-30 16:47:14.000000 MACS3-3.0.0b3/MACS3/fermi-lite/lib/arm/neon/cvt.h
+-rw-r--r--   0 runner    (1001) docker     (123)     6420 2023-07-30 16:47:14.000000 MACS3-3.0.0b3/MACS3/fermi-lite/lib/arm/neon/dot.h
+-rw-r--r--   0 runner    (1001) docker     (123)     7781 2023-07-30 16:47:14.000000 MACS3-3.0.0b3/MACS3/fermi-lite/lib/arm/neon/dot_lane.h
+-rw-r--r--   0 runner    (1001) docker     (123)    21506 2023-07-30 16:47:14.000000 MACS3-3.0.0b3/MACS3/fermi-lite/lib/arm/neon/dup_lane.h
+-rw-r--r--   0 runner    (1001) docker     (123)    15175 2023-07-30 16:47:14.000000 MACS3-3.0.0b3/MACS3/fermi-lite/lib/arm/neon/dup_n.h
+-rw-r--r--   0 runner    (1001) docker     (123)    15830 2023-07-30 16:47:14.000000 MACS3-3.0.0b3/MACS3/fermi-lite/lib/arm/neon/eor.h
+-rw-r--r--   0 runner    (1001) docker     (123)    39152 2023-07-30 16:47:14.000000 MACS3-3.0.0b3/MACS3/fermi-lite/lib/arm/neon/ext.h
+-rw-r--r--   0 runner    (1001) docker     (123)     7901 2023-07-30 16:47:14.000000 MACS3-3.0.0b3/MACS3/fermi-lite/lib/arm/neon/get_high.h
+-rw-r--r--   0 runner    (1001) docker     (123)    14459 2023-07-30 16:47:14.000000 MACS3-3.0.0b3/MACS3/fermi-lite/lib/arm/neon/get_lane.h
+-rw-r--r--   0 runner    (1001) docker     (123)     8238 2023-07-30 16:47:14.000000 MACS3-3.0.0b3/MACS3/fermi-lite/lib/arm/neon/get_low.h
+-rw-r--r--   0 runner    (1001) docker     (123)     9710 2023-07-30 16:47:14.000000 MACS3-3.0.0b3/MACS3/fermi-lite/lib/arm/neon/hadd.h
+-rw-r--r--   0 runner    (1001) docker     (123)     9710 2023-07-30 16:47:14.000000 MACS3-3.0.0b3/MACS3/fermi-lite/lib/arm/neon/hsub.h
+-rw-r--r--   0 runner    (1001) docker     (123)    11789 2023-07-30 16:47:14.000000 MACS3-3.0.0b3/MACS3/fermi-lite/lib/arm/neon/ld1.h
+-rw-r--r--   0 runner    (1001) docker     (123)    16633 2023-07-30 16:47:14.000000 MACS3-3.0.0b3/MACS3/fermi-lite/lib/arm/neon/ld3.h
+-rw-r--r--   0 runner    (1001) docker     (123)    15320 2023-07-30 16:47:14.000000 MACS3-3.0.0b3/MACS3/fermi-lite/lib/arm/neon/ld4.h
+-rw-r--r--   0 runner    (1001) docker     (123)    19022 2023-07-30 16:47:14.000000 MACS3-3.0.0b3/MACS3/fermi-lite/lib/arm/neon/max.h
+-rw-r--r--   0 runner    (1001) docker     (123)     6916 2023-07-30 16:47:14.000000 MACS3-3.0.0b3/MACS3/fermi-lite/lib/arm/neon/maxnm.h
+-rw-r--r--   0 runner    (1001) docker     (123)     9895 2023-07-30 16:47:14.000000 MACS3-3.0.0b3/MACS3/fermi-lite/lib/arm/neon/maxv.h
+-rw-r--r--   0 runner    (1001) docker     (123)    20487 2023-07-30 16:47:14.000000 MACS3-3.0.0b3/MACS3/fermi-lite/lib/arm/neon/min.h
+-rw-r--r--   0 runner    (1001) docker     (123)     6916 2023-07-30 16:47:14.000000 MACS3-3.0.0b3/MACS3/fermi-lite/lib/arm/neon/minnm.h
+-rw-r--r--   0 runner    (1001) docker     (123)    10751 2023-07-30 16:47:14.000000 MACS3-3.0.0b3/MACS3/fermi-lite/lib/arm/neon/minv.h
+-rw-r--r--   0 runner    (1001) docker     (123)    16338 2023-07-30 16:47:14.000000 MACS3-3.0.0b3/MACS3/fermi-lite/lib/arm/neon/mla.h
+-rw-r--r--   0 runner    (1001) docker     (123)    10252 2023-07-30 16:47:14.000000 MACS3-3.0.0b3/MACS3/fermi-lite/lib/arm/neon/mla_n.h
+-rw-r--r--   0 runner    (1001) docker     (123)     5025 2023-07-30 16:47:14.000000 MACS3-3.0.0b3/MACS3/fermi-lite/lib/arm/neon/mlal.h
+-rw-r--r--   0 runner    (1001) docker     (123)     5259 2023-07-30 16:47:14.000000 MACS3-3.0.0b3/MACS3/fermi-lite/lib/arm/neon/mlal_high.h
+-rw-r--r--   0 runner    (1001) docker     (123)     4149 2023-07-30 16:47:14.000000 MACS3-3.0.0b3/MACS3/fermi-lite/lib/arm/neon/mlal_n.h
+-rw-r--r--   0 runner    (1001) docker     (123)     7922 2023-07-30 16:47:14.000000 MACS3-3.0.0b3/MACS3/fermi-lite/lib/arm/neon/mls.h
+-rw-r--r--   0 runner    (1001) docker     (123)     3888 2023-07-30 16:47:14.000000 MACS3-3.0.0b3/MACS3/fermi-lite/lib/arm/neon/mlsl.h
+-rw-r--r--   0 runner    (1001) docker     (123)     4092 2023-07-30 16:47:14.000000 MACS3-3.0.0b3/MACS3/fermi-lite/lib/arm/neon/mlsl_high.h
+-rw-r--r--   0 runner    (1001) docker     (123)     3110 2023-07-30 16:47:14.000000 MACS3-3.0.0b3/MACS3/fermi-lite/lib/arm/neon/mlsl_n.h
+-rw-r--r--   0 runner    (1001) docker     (123)     6302 2023-07-30 16:47:14.000000 MACS3-3.0.0b3/MACS3/fermi-lite/lib/arm/neon/movl.h
+-rw-r--r--   0 runner    (1001) docker     (123)     3784 2023-07-30 16:47:14.000000 MACS3-3.0.0b3/MACS3/fermi-lite/lib/arm/neon/movl_high.h
+-rw-r--r--   0 runner    (1001) docker     (123)     5749 2023-07-30 16:47:14.000000 MACS3-3.0.0b3/MACS3/fermi-lite/lib/arm/neon/movn.h
+-rw-r--r--   0 runner    (1001) docker     (123)     3905 2023-07-30 16:47:14.000000 MACS3-3.0.0b3/MACS3/fermi-lite/lib/arm/neon/movn_high.h
+-rw-r--r--   0 runner    (1001) docker     (123)    16534 2023-07-30 16:47:14.000000 MACS3-3.0.0b3/MACS3/fermi-lite/lib/arm/neon/mul.h
+-rw-r--r--   0 runner    (1001) docker     (123)    15323 2023-07-30 16:47:14.000000 MACS3-3.0.0b3/MACS3/fermi-lite/lib/arm/neon/mul_lane.h
+-rw-r--r--   0 runner    (1001) docker     (123)    10970 2023-07-30 16:47:14.000000 MACS3-3.0.0b3/MACS3/fermi-lite/lib/arm/neon/mul_n.h
+-rw-r--r--   0 runner    (1001) docker     (123)     7854 2023-07-30 16:47:14.000000 MACS3-3.0.0b3/MACS3/fermi-lite/lib/arm/neon/mull.h
+-rw-r--r--   0 runner    (1001) docker     (123)     4044 2023-07-30 16:47:14.000000 MACS3-3.0.0b3/MACS3/fermi-lite/lib/arm/neon/mull_high.h
+-rw-r--r--   0 runner    (1001) docker     (123)     5266 2023-07-30 16:47:14.000000 MACS3-3.0.0b3/MACS3/fermi-lite/lib/arm/neon/mull_n.h
+-rw-r--r--   0 runner    (1001) docker     (123)    11934 2023-07-30 16:47:14.000000 MACS3-3.0.0b3/MACS3/fermi-lite/lib/arm/neon/mvn.h
+-rw-r--r--   0 runner    (1001) docker     (123)    10654 2023-07-30 16:47:14.000000 MACS3-3.0.0b3/MACS3/fermi-lite/lib/arm/neon/neg.h
+-rw-r--r--   0 runner    (1001) docker     (123)    14551 2023-07-30 16:47:14.000000 MACS3-3.0.0b3/MACS3/fermi-lite/lib/arm/neon/orn.h
+-rw-r--r--   0 runner    (1001) docker     (123)    15798 2023-07-30 16:47:14.000000 MACS3-3.0.0b3/MACS3/fermi-lite/lib/arm/neon/orr.h
+-rw-r--r--   0 runner    (1001) docker     (123)     6129 2023-07-30 16:47:14.000000 MACS3-3.0.0b3/MACS3/fermi-lite/lib/arm/neon/padal.h
+-rw-r--r--   0 runner    (1001) docker     (123)     8877 2023-07-30 16:47:14.000000 MACS3-3.0.0b3/MACS3/fermi-lite/lib/arm/neon/padd.h
+-rw-r--r--   0 runner    (1001) docker     (123)     7552 2023-07-30 16:47:14.000000 MACS3-3.0.0b3/MACS3/fermi-lite/lib/arm/neon/paddl.h
+-rw-r--r--   0 runner    (1001) docker     (123)     7572 2023-07-30 16:47:14.000000 MACS3-3.0.0b3/MACS3/fermi-lite/lib/arm/neon/pmax.h
+-rw-r--r--   0 runner    (1001) docker     (123)     7826 2023-07-30 16:47:14.000000 MACS3-3.0.0b3/MACS3/fermi-lite/lib/arm/neon/pmin.h
+-rw-r--r--   0 runner    (1001) docker     (123)     7366 2023-07-30 16:47:14.000000 MACS3-3.0.0b3/MACS3/fermi-lite/lib/arm/neon/qabs.h
+-rw-r--r--   0 runner    (1001) docker     (123)    15857 2023-07-30 16:47:14.000000 MACS3-3.0.0b3/MACS3/fermi-lite/lib/arm/neon/qadd.h
+-rw-r--r--   0 runner    (1001) docker     (123)     4074 2023-07-30 16:47:14.000000 MACS3-3.0.0b3/MACS3/fermi-lite/lib/arm/neon/qdmulh.h
+-rw-r--r--   0 runner    (1001) docker     (123)     4152 2023-07-30 16:47:14.000000 MACS3-3.0.0b3/MACS3/fermi-lite/lib/arm/neon/qdmull.h
+-rw-r--r--   0 runner    (1001) docker     (123)     8266 2023-07-30 16:47:14.000000 MACS3-3.0.0b3/MACS3/fermi-lite/lib/arm/neon/qmovn.h
+-rw-r--r--   0 runner    (1001) docker     (123)     4029 2023-07-30 16:47:14.000000 MACS3-3.0.0b3/MACS3/fermi-lite/lib/arm/neon/qmovn_high.h
+-rw-r--r--   0 runner    (1001) docker     (123)     5196 2023-07-30 16:47:14.000000 MACS3-3.0.0b3/MACS3/fermi-lite/lib/arm/neon/qmovun.h
+-rw-r--r--   0 runner    (1001) docker     (123)     8600 2023-07-30 16:47:14.000000 MACS3-3.0.0b3/MACS3/fermi-lite/lib/arm/neon/qneg.h
+-rw-r--r--   0 runner    (1001) docker     (123)     5260 2023-07-30 16:47:14.000000 MACS3-3.0.0b3/MACS3/fermi-lite/lib/arm/neon/qrdmulh.h
+-rw-r--r--   0 runner    (1001) docker     (123)     4088 2023-07-30 16:47:14.000000 MACS3-3.0.0b3/MACS3/fermi-lite/lib/arm/neon/qrdmulh_n.h
+-rw-r--r--   0 runner    (1001) docker     (123)    19189 2023-07-30 16:47:14.000000 MACS3-3.0.0b3/MACS3/fermi-lite/lib/arm/neon/qshl.h
+-rw-r--r--   0 runner    (1001) docker     (123)    15571 2023-07-30 16:47:14.000000 MACS3-3.0.0b3/MACS3/fermi-lite/lib/arm/neon/qsub.h
+-rw-r--r--   0 runner    (1001) docker     (123)    17511 2023-07-30 16:47:14.000000 MACS3-3.0.0b3/MACS3/fermi-lite/lib/arm/neon/qtbl.h
+-rw-r--r--   0 runner    (1001) docker     (123)    19270 2023-07-30 16:47:14.000000 MACS3-3.0.0b3/MACS3/fermi-lite/lib/arm/neon/qtbx.h
+-rw-r--r--   0 runner    (1001) docker     (123)     6384 2023-07-30 16:47:14.000000 MACS3-3.0.0b3/MACS3/fermi-lite/lib/arm/neon/rbit.h
+-rw-r--r--   0 runner    (1001) docker     (123)    95760 2023-07-30 16:47:14.000000 MACS3-3.0.0b3/MACS3/fermi-lite/lib/arm/neon/reinterpret.h
+-rw-r--r--   0 runner    (1001) docker     (123)     4773 2023-07-30 16:47:14.000000 MACS3-3.0.0b3/MACS3/fermi-lite/lib/arm/neon/rev16.h
+-rw-r--r--   0 runner    (1001) docker     (123)     8072 2023-07-30 16:47:14.000000 MACS3-3.0.0b3/MACS3/fermi-lite/lib/arm/neon/rev32.h
+-rw-r--r--   0 runner    (1001) docker     (123)    11898 2023-07-30 16:47:14.000000 MACS3-3.0.0b3/MACS3/fermi-lite/lib/arm/neon/rev64.h
+-rw-r--r--   0 runner    (1001) docker     (123)    16270 2023-07-30 16:47:14.000000 MACS3-3.0.0b3/MACS3/fermi-lite/lib/arm/neon/rhadd.h
+-rw-r--r--   0 runner    (1001) docker     (123)     4269 2023-07-30 16:47:14.000000 MACS3-3.0.0b3/MACS3/fermi-lite/lib/arm/neon/rnd.h
+-rw-r--r--   0 runner    (1001) docker     (123)    43945 2023-07-30 16:47:14.000000 MACS3-3.0.0b3/MACS3/fermi-lite/lib/arm/neon/rshl.h
+-rw-r--r--   0 runner    (1001) docker     (123)    16744 2023-07-30 16:47:14.000000 MACS3-3.0.0b3/MACS3/fermi-lite/lib/arm/neon/rshr_n.h
+-rw-r--r--   0 runner    (1001) docker     (123)     7379 2023-07-30 16:47:14.000000 MACS3-3.0.0b3/MACS3/fermi-lite/lib/arm/neon/rsra_n.h
+-rw-r--r--   0 runner    (1001) docker     (123)    13789 2023-07-30 16:47:14.000000 MACS3-3.0.0b3/MACS3/fermi-lite/lib/arm/neon/set_lane.h
+-rw-r--r--   0 runner    (1001) docker     (123)    35543 2023-07-30 16:47:14.000000 MACS3-3.0.0b3/MACS3/fermi-lite/lib/arm/neon/shl.h
+-rw-r--r--   0 runner    (1001) docker     (123)    18134 2023-07-30 16:47:14.000000 MACS3-3.0.0b3/MACS3/fermi-lite/lib/arm/neon/shl_n.h
+-rw-r--r--   0 runner    (1001) docker     (123)    19435 2023-07-30 16:47:14.000000 MACS3-3.0.0b3/MACS3/fermi-lite/lib/arm/neon/shr_n.h
+-rw-r--r--   0 runner    (1001) docker     (123)     7090 2023-07-30 16:47:14.000000 MACS3-3.0.0b3/MACS3/fermi-lite/lib/arm/neon/sra_n.h
+-rw-r--r--   0 runner    (1001) docker     (123)    10700 2023-07-30 16:47:14.000000 MACS3-3.0.0b3/MACS3/fermi-lite/lib/arm/neon/st1.h
+-rw-r--r--   0 runner    (1001) docker     (123)    12450 2023-07-30 16:47:14.000000 MACS3-3.0.0b3/MACS3/fermi-lite/lib/arm/neon/st1_lane.h
+-rw-r--r--   0 runner    (1001) docker     (123)    14527 2023-07-30 16:47:14.000000 MACS3-3.0.0b3/MACS3/fermi-lite/lib/arm/neon/st3.h
+-rw-r--r--   0 runner    (1001) docker     (123)    16018 2023-07-30 16:47:14.000000 MACS3-3.0.0b3/MACS3/fermi-lite/lib/arm/neon/st4.h
+-rw-r--r--   0 runner    (1001) docker     (123)    18645 2023-07-30 16:47:14.000000 MACS3-3.0.0b3/MACS3/fermi-lite/lib/arm/neon/sub.h
+-rw-r--r--   0 runner    (1001) docker     (123)     3912 2023-07-30 16:47:14.000000 MACS3-3.0.0b3/MACS3/fermi-lite/lib/arm/neon/subl.h
+-rw-r--r--   0 runner    (1001) docker     (123)     7418 2023-07-30 16:47:14.000000 MACS3-3.0.0b3/MACS3/fermi-lite/lib/arm/neon/subw.h
+-rw-r--r--   0 runner    (1001) docker     (123)     8041 2023-07-30 16:47:14.000000 MACS3-3.0.0b3/MACS3/fermi-lite/lib/arm/neon/subw_high.h
+-rw-r--r--   0 runner    (1001) docker     (123)     7749 2023-07-30 16:47:14.000000 MACS3-3.0.0b3/MACS3/fermi-lite/lib/arm/neon/tbl.h
+-rw-r--r--   0 runner    (1001) docker     (123)     9121 2023-07-30 16:47:14.000000 MACS3-3.0.0b3/MACS3/fermi-lite/lib/arm/neon/tbx.h
+-rw-r--r--   0 runner    (1001) docker     (123)     7435 2023-07-30 16:47:14.000000 MACS3-3.0.0b3/MACS3/fermi-lite/lib/arm/neon/trn.h
+-rw-r--r--   0 runner    (1001) docker     (123)    14460 2023-07-30 16:47:14.000000 MACS3-3.0.0b3/MACS3/fermi-lite/lib/arm/neon/trn1.h
+-rw-r--r--   0 runner    (1001) docker     (123)    14595 2023-07-30 16:47:14.000000 MACS3-3.0.0b3/MACS3/fermi-lite/lib/arm/neon/trn2.h
+-rw-r--r--   0 runner    (1001) docker     (123)    17552 2023-07-30 16:47:14.000000 MACS3-3.0.0b3/MACS3/fermi-lite/lib/arm/neon/tst.h
+-rw-r--r--   0 runner    (1001) docker     (123)    26581 2023-07-30 16:47:14.000000 MACS3-3.0.0b3/MACS3/fermi-lite/lib/arm/neon/types.h
+-rw-r--r--   0 runner    (1001) docker     (123)     9465 2023-07-30 16:47:14.000000 MACS3-3.0.0b3/MACS3/fermi-lite/lib/arm/neon/uqadd.h
+-rw-r--r--   0 runner    (1001) docker     (123)     7435 2023-07-30 16:47:14.000000 MACS3-3.0.0b3/MACS3/fermi-lite/lib/arm/neon/uzp.h
+-rw-r--r--   0 runner    (1001) docker     (123)    20856 2023-07-30 16:47:14.000000 MACS3-3.0.0b3/MACS3/fermi-lite/lib/arm/neon/uzp1.h
+-rw-r--r--   0 runner    (1001) docker     (123)    21036 2023-07-30 16:47:14.000000 MACS3-3.0.0b3/MACS3/fermi-lite/lib/arm/neon/uzp2.h
+-rw-r--r--   0 runner    (1001) docker     (123)     7435 2023-07-30 16:47:14.000000 MACS3-3.0.0b3/MACS3/fermi-lite/lib/arm/neon/zip.h
+-rw-r--r--   0 runner    (1001) docker     (123)    19744 2023-07-30 16:47:14.000000 MACS3-3.0.0b3/MACS3/fermi-lite/lib/arm/neon/zip1.h
+-rw-r--r--   0 runner    (1001) docker     (123)    20392 2023-07-30 16:47:14.000000 MACS3-3.0.0b3/MACS3/fermi-lite/lib/arm/neon/zip2.h
+-rw-r--r--   0 runner    (1001) docker     (123)     4351 2023-07-30 16:47:14.000000 MACS3-3.0.0b3/MACS3/fermi-lite/lib/arm/neon.h
+-rw-r--r--   0 runner    (1001) docker     (123)     9846 2023-07-30 16:47:14.000000 MACS3-3.0.0b3/MACS3/fermi-lite/lib/check.h
+-rw-r--r--   0 runner    (1001) docker     (123)     3119 2023-07-30 16:47:14.000000 MACS3-3.0.0b3/MACS3/fermi-lite/lib/debug-trap.h
+-rw-r--r--   0 runner    (1001) docker     (123)    74181 2023-07-30 16:47:14.000000 MACS3-3.0.0b3/MACS3/fermi-lite/lib/hedley.h
+-rw-r--r--   0 runner    (1001) docker     (123)    17805 2023-07-30 16:47:14.000000 MACS3-3.0.0b3/MACS3/fermi-lite/lib/simde-align.h
+-rw-r--r--   0 runner    (1001) docker     (123)    16472 2023-07-30 16:47:14.000000 MACS3-3.0.0b3/MACS3/fermi-lite/lib/simde-arch.h
+-rw-r--r--   0 runner    (1001) docker     (123)    32588 2023-07-30 16:47:14.000000 MACS3-3.0.0b3/MACS3/fermi-lite/lib/simde-common.h
+-rw-r--r--   0 runner    (1001) docker     (123)    18585 2023-07-30 16:47:14.000000 MACS3-3.0.0b3/MACS3/fermi-lite/lib/simde-constify.h
+-rw-r--r--   0 runner    (1001) docker     (123)     5065 2023-07-30 16:47:14.000000 MACS3-3.0.0b3/MACS3/fermi-lite/lib/simde-detect-clang.h
+-rw-r--r--   0 runner    (1001) docker     (123)    18236 2023-07-30 16:47:14.000000 MACS3-3.0.0b3/MACS3/fermi-lite/lib/simde-diagnostic.h
+-rw-r--r--   0 runner    (1001) docker     (123)    17861 2023-07-30 16:47:14.000000 MACS3-3.0.0b3/MACS3/fermi-lite/lib/simde-features.h
+-rw-r--r--   0 runner    (1001) docker     (123)    57737 2023-07-30 16:47:14.000000 MACS3-3.0.0b3/MACS3/fermi-lite/lib/simde-math.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 16:49:27.482858 MACS3-3.0.0b3/MACS3/fermi-lite/lib/x86/
+-rw-r--r--   0 runner    (1001) docker     (123)   195250 2023-07-30 16:47:14.000000 MACS3-3.0.0b3/MACS3/fermi-lite/lib/x86/avx.h
+-rw-r--r--   0 runner    (1001) docker     (123)   194448 2023-07-30 16:47:14.000000 MACS3-3.0.0b3/MACS3/fermi-lite/lib/x86/avx2.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 16:49:27.494857 MACS3-3.0.0b3/MACS3/fermi-lite/lib/x86/avx512/
+-rw-r--r--   0 runner    (1001) docker     (123)     8026 2023-07-30 16:47:14.000000 MACS3-3.0.0b3/MACS3/fermi-lite/lib/x86/avx512/2intersect.h
+-rw-r--r--   0 runner    (1001) docker     (123)    17914 2023-07-30 16:47:14.000000 MACS3-3.0.0b3/MACS3/fermi-lite/lib/x86/avx512/abs.h
+-rw-r--r--   0 runner    (1001) docker     (123)    21097 2023-07-30 16:47:14.000000 MACS3-3.0.0b3/MACS3/fermi-lite/lib/x86/avx512/add.h
+-rw-r--r--   0 runner    (1001) docker     (123)    13194 2023-07-30 16:47:14.000000 MACS3-3.0.0b3/MACS3/fermi-lite/lib/x86/avx512/adds.h
+-rw-r--r--   0 runner    (1001) docker     (123)     9570 2023-07-30 16:47:14.000000 MACS3-3.0.0b3/MACS3/fermi-lite/lib/x86/avx512/and.h
+-rw-r--r--   0 runner    (1001) docker     (123)     7564 2023-07-30 16:47:14.000000 MACS3-3.0.0b3/MACS3/fermi-lite/lib/x86/avx512/andnot.h
+-rw-r--r--   0 runner    (1001) docker     (123)     8799 2023-07-30 16:47:14.000000 MACS3-3.0.0b3/MACS3/fermi-lite/lib/x86/avx512/avg.h
+-rw-r--r--   0 runner    (1001) docker     (123)     9480 2023-07-30 16:47:14.000000 MACS3-3.0.0b3/MACS3/fermi-lite/lib/x86/avx512/blend.h
+-rw-r--r--   0 runner    (1001) docker     (123)    29208 2023-07-30 16:47:14.000000 MACS3-3.0.0b3/MACS3/fermi-lite/lib/x86/avx512/broadcast.h
+-rw-r--r--   0 runner    (1001) docker     (123)     9094 2023-07-30 16:47:14.000000 MACS3-3.0.0b3/MACS3/fermi-lite/lib/x86/avx512/cast.h
+-rw-r--r--   0 runner    (1001) docker     (123)    23105 2023-07-30 16:47:14.000000 MACS3-3.0.0b3/MACS3/fermi-lite/lib/x86/avx512/cmp.h
+-rw-r--r--   0 runner    (1001) docker     (123)     5959 2023-07-30 16:47:14.000000 MACS3-3.0.0b3/MACS3/fermi-lite/lib/x86/avx512/cmpeq.h
+-rw-r--r--   0 runner    (1001) docker     (123)     3401 2023-07-30 16:47:14.000000 MACS3-3.0.0b3/MACS3/fermi-lite/lib/x86/avx512/cmpge.h
+-rw-r--r--   0 runner    (1001) docker     (123)     6256 2023-07-30 16:47:14.000000 MACS3-3.0.0b3/MACS3/fermi-lite/lib/x86/avx512/cmpgt.h
+-rw-r--r--   0 runner    (1001) docker     (123)     3352 2023-07-30 16:47:14.000000 MACS3-3.0.0b3/MACS3/fermi-lite/lib/x86/avx512/cmple.h
+-rw-r--r--   0 runner    (1001) docker     (123)     4012 2023-07-30 16:47:14.000000 MACS3-3.0.0b3/MACS3/fermi-lite/lib/x86/avx512/cmplt.h
+-rw-r--r--   0 runner    (1001) docker     (123)     3008 2023-07-30 16:47:14.000000 MACS3-3.0.0b3/MACS3/fermi-lite/lib/x86/avx512/copysign.h
+-rw-r--r--   0 runner    (1001) docker     (123)     3959 2023-07-30 16:47:14.000000 MACS3-3.0.0b3/MACS3/fermi-lite/lib/x86/avx512/cvt.h
+-rw-r--r--   0 runner    (1001) docker     (123)    23453 2023-07-30 16:47:14.000000 MACS3-3.0.0b3/MACS3/fermi-lite/lib/x86/avx512/cvts.h
+-rw-r--r--   0 runner    (1001) docker     (123)     5289 2023-07-30 16:47:14.000000 MACS3-3.0.0b3/MACS3/fermi-lite/lib/x86/avx512/div.h
+-rw-r--r--   0 runner    (1001) docker     (123)     8810 2023-07-30 16:47:14.000000 MACS3-3.0.0b3/MACS3/fermi-lite/lib/x86/avx512/extract.h
+-rw-r--r--   0 runner    (1001) docker     (123)     4563 2023-07-30 16:47:14.000000 MACS3-3.0.0b3/MACS3/fermi-lite/lib/x86/avx512/fmadd.h
+-rw-r--r--   0 runner    (1001) docker     (123)     3601 2023-07-30 16:47:14.000000 MACS3-3.0.0b3/MACS3/fermi-lite/lib/x86/avx512/fmsub.h
+-rw-r--r--   0 runner    (1001) docker     (123)     3620 2023-07-30 16:47:14.000000 MACS3-3.0.0b3/MACS3/fermi-lite/lib/x86/avx512/fnmadd.h
+-rw-r--r--   0 runner    (1001) docker     (123)     3620 2023-07-30 16:47:14.000000 MACS3-3.0.0b3/MACS3/fermi-lite/lib/x86/avx512/fnmsub.h
+-rw-r--r--   0 runner    (1001) docker     (123)     7801 2023-07-30 16:47:14.000000 MACS3-3.0.0b3/MACS3/fermi-lite/lib/x86/avx512/insert.h
+-rw-r--r--   0 runner    (1001) docker     (123)     5919 2023-07-30 16:47:14.000000 MACS3-3.0.0b3/MACS3/fermi-lite/lib/x86/avx512/kshift.h
+-rw-r--r--   0 runner    (1001) docker     (123)     2556 2023-07-30 16:47:14.000000 MACS3-3.0.0b3/MACS3/fermi-lite/lib/x86/avx512/load.h
+-rw-r--r--   0 runner    (1001) docker     (123)     7347 2023-07-30 16:47:14.000000 MACS3-3.0.0b3/MACS3/fermi-lite/lib/x86/avx512/loadu.h
+-rw-r--r--   0 runner    (1001) docker     (123)     7454 2023-07-30 16:47:14.000000 MACS3-3.0.0b3/MACS3/fermi-lite/lib/x86/avx512/lzcnt.h
+-rw-r--r--   0 runner    (1001) docker     (123)     5652 2023-07-30 16:47:14.000000 MACS3-3.0.0b3/MACS3/fermi-lite/lib/x86/avx512/madd.h
+-rw-r--r--   0 runner    (1001) docker     (123)     6089 2023-07-30 16:47:14.000000 MACS3-3.0.0b3/MACS3/fermi-lite/lib/x86/avx512/maddubs.h
+-rw-r--r--   0 runner    (1001) docker     (123)    18597 2023-07-30 16:47:14.000000 MACS3-3.0.0b3/MACS3/fermi-lite/lib/x86/avx512/max.h
+-rw-r--r--   0 runner    (1001) docker     (123)    18599 2023-07-30 16:47:14.000000 MACS3-3.0.0b3/MACS3/fermi-lite/lib/x86/avx512/min.h
+-rw-r--r--   0 runner    (1001) docker     (123)    30273 2023-07-30 16:47:14.000000 MACS3-3.0.0b3/MACS3/fermi-lite/lib/x86/avx512/mov.h
+-rw-r--r--   0 runner    (1001) docker     (123)    11926 2023-07-30 16:47:14.000000 MACS3-3.0.0b3/MACS3/fermi-lite/lib/x86/avx512/mov_mask.h
+-rw-r--r--   0 runner    (1001) docker     (123)    15715 2023-07-30 16:47:14.000000 MACS3-3.0.0b3/MACS3/fermi-lite/lib/x86/avx512/movm.h
+-rw-r--r--   0 runner    (1001) docker     (123)     9151 2023-07-30 16:47:14.000000 MACS3-3.0.0b3/MACS3/fermi-lite/lib/x86/avx512/mul.h
+-rw-r--r--   0 runner    (1001) docker     (123)     2282 2023-07-30 16:47:14.000000 MACS3-3.0.0b3/MACS3/fermi-lite/lib/x86/avx512/mulhi.h
+-rw-r--r--   0 runner    (1001) docker     (123)     2272 2023-07-30 16:47:14.000000 MACS3-3.0.0b3/MACS3/fermi-lite/lib/x86/avx512/mulhrs.h
+-rw-r--r--   0 runner    (1001) docker     (123)     3842 2023-07-30 16:47:14.000000 MACS3-3.0.0b3/MACS3/fermi-lite/lib/x86/avx512/mullo.h
+-rw-r--r--   0 runner    (1001) docker     (123)     2639 2023-07-30 16:47:14.000000 MACS3-3.0.0b3/MACS3/fermi-lite/lib/x86/avx512/negate.h
+-rw-r--r--   0 runner    (1001) docker     (123)     7993 2023-07-30 16:47:14.000000 MACS3-3.0.0b3/MACS3/fermi-lite/lib/x86/avx512/or.h
+-rw-r--r--   0 runner    (1001) docker     (123)     6819 2023-07-30 16:47:14.000000 MACS3-3.0.0b3/MACS3/fermi-lite/lib/x86/avx512/packs.h
+-rw-r--r--   0 runner    (1001) docker     (123)     6833 2023-07-30 16:47:14.000000 MACS3-3.0.0b3/MACS3/fermi-lite/lib/x86/avx512/packus.h
+-rw-r--r--   0 runner    (1001) docker     (123)    69829 2023-07-30 16:47:14.000000 MACS3-3.0.0b3/MACS3/fermi-lite/lib/x86/avx512/permutex2var.h
+-rw-r--r--   0 runner    (1001) docker     (123)    49807 2023-07-30 16:47:14.000000 MACS3-3.0.0b3/MACS3/fermi-lite/lib/x86/avx512/permutexvar.h
+-rw-r--r--   0 runner    (1001) docker     (123)     2638 2023-07-30 16:47:14.000000 MACS3-3.0.0b3/MACS3/fermi-lite/lib/x86/avx512/sad.h
+-rw-r--r--   0 runner    (1001) docker     (123)    15045 2023-07-30 16:47:14.000000 MACS3-3.0.0b3/MACS3/fermi-lite/lib/x86/avx512/set.h
+-rw-r--r--   0 runner    (1001) docker     (123)     9209 2023-07-30 16:47:14.000000 MACS3-3.0.0b3/MACS3/fermi-lite/lib/x86/avx512/set1.h
+-rw-r--r--   0 runner    (1001) docker     (123)     3705 2023-07-30 16:47:14.000000 MACS3-3.0.0b3/MACS3/fermi-lite/lib/x86/avx512/set4.h
+-rw-r--r--   0 runner    (1001) docker     (123)     2104 2023-07-30 16:47:14.000000 MACS3-3.0.0b3/MACS3/fermi-lite/lib/x86/avx512/setone.h
+-rw-r--r--   0 runner    (1001) docker     (123)     4723 2023-07-30 16:47:14.000000 MACS3-3.0.0b3/MACS3/fermi-lite/lib/x86/avx512/setr.h
+-rw-r--r--   0 runner    (1001) docker     (123)     3735 2023-07-30 16:47:14.000000 MACS3-3.0.0b3/MACS3/fermi-lite/lib/x86/avx512/setr4.h
+-rw-r--r--   0 runner    (1001) docker     (123)     2924 2023-07-30 16:47:14.000000 MACS3-3.0.0b3/MACS3/fermi-lite/lib/x86/avx512/setzero.h
+-rw-r--r--   0 runner    (1001) docker     (123)     7868 2023-07-30 16:47:14.000000 MACS3-3.0.0b3/MACS3/fermi-lite/lib/x86/avx512/shuffle.h
+-rw-r--r--   0 runner    (1001) docker     (123)     8169 2023-07-30 16:47:14.000000 MACS3-3.0.0b3/MACS3/fermi-lite/lib/x86/avx512/sll.h
+-rw-r--r--   0 runner    (1001) docker     (123)     6812 2023-07-30 16:47:14.000000 MACS3-3.0.0b3/MACS3/fermi-lite/lib/x86/avx512/slli.h
+-rw-r--r--   0 runner    (1001) docker     (123)     2360 2023-07-30 16:47:14.000000 MACS3-3.0.0b3/MACS3/fermi-lite/lib/x86/avx512/sllv.h
+-rw-r--r--   0 runner    (1001) docker     (123)     3977 2023-07-30 16:47:14.000000 MACS3-3.0.0b3/MACS3/fermi-lite/lib/x86/avx512/sqrt.h
+-rw-r--r--   0 runner    (1001) docker     (123)     2684 2023-07-30 16:47:14.000000 MACS3-3.0.0b3/MACS3/fermi-lite/lib/x86/avx512/sra.h
+-rw-r--r--   0 runner    (1001) docker     (123)     2340 2023-07-30 16:47:14.000000 MACS3-3.0.0b3/MACS3/fermi-lite/lib/x86/avx512/srai.h
+-rw-r--r--   0 runner    (1001) docker     (123)     2271 2023-07-30 16:47:14.000000 MACS3-3.0.0b3/MACS3/fermi-lite/lib/x86/avx512/srav.h
+-rw-r--r--   0 runner    (1001) docker     (123)     6928 2023-07-30 16:47:14.000000 MACS3-3.0.0b3/MACS3/fermi-lite/lib/x86/avx512/srl.h
+-rw-r--r--   0 runner    (1001) docker     (123)     6593 2023-07-30 16:47:14.000000 MACS3-3.0.0b3/MACS3/fermi-lite/lib/x86/avx512/srli.h
+-rw-r--r--   0 runner    (1001) docker     (123)     9460 2023-07-30 16:47:14.000000 MACS3-3.0.0b3/MACS3/fermi-lite/lib/x86/avx512/srlv.h
+-rw-r--r--   0 runner    (1001) docker     (123)     3507 2023-07-30 16:47:14.000000 MACS3-3.0.0b3/MACS3/fermi-lite/lib/x86/avx512/store.h
+-rw-r--r--   0 runner    (1001) docker     (123)     3429 2023-07-30 16:47:14.000000 MACS3-3.0.0b3/MACS3/fermi-lite/lib/x86/avx512/storeu.h
+-rw-r--r--   0 runner    (1001) docker     (123)    10888 2023-07-30 16:47:14.000000 MACS3-3.0.0b3/MACS3/fermi-lite/lib/x86/avx512/sub.h
+-rw-r--r--   0 runner    (1001) docker     (123)     7107 2023-07-30 16:47:14.000000 MACS3-3.0.0b3/MACS3/fermi-lite/lib/x86/avx512/subs.h
+-rw-r--r--   0 runner    (1001) docker     (123)     6297 2023-07-30 16:47:14.000000 MACS3-3.0.0b3/MACS3/fermi-lite/lib/x86/avx512/test.h
+-rw-r--r--   0 runner    (1001) docker     (123)    17809 2023-07-30 16:47:14.000000 MACS3-3.0.0b3/MACS3/fermi-lite/lib/x86/avx512/types.h
+-rw-r--r--   0 runner    (1001) docker     (123)    13394 2023-07-30 16:47:14.000000 MACS3-3.0.0b3/MACS3/fermi-lite/lib/x86/avx512/unpackhi.h
+-rw-r--r--   0 runner    (1001) docker     (123)     3886 2023-07-30 16:47:14.000000 MACS3-3.0.0b3/MACS3/fermi-lite/lib/x86/avx512/unpacklo.h
+-rw-r--r--   0 runner    (1001) docker     (123)     8662 2023-07-30 16:47:14.000000 MACS3-3.0.0b3/MACS3/fermi-lite/lib/x86/avx512/xor.h
+-rw-r--r--   0 runner    (1001) docker     (123)     2426 2023-07-30 16:47:14.000000 MACS3-3.0.0b3/MACS3/fermi-lite/lib/x86/avx512/xorsign.h
+-rw-r--r--   0 runner    (1001) docker     (123)     3227 2023-07-30 16:47:14.000000 MACS3-3.0.0b3/MACS3/fermi-lite/lib/x86/avx512.h
+-rw-r--r--   0 runner    (1001) docker     (123)    15656 2023-07-30 16:47:14.000000 MACS3-3.0.0b3/MACS3/fermi-lite/lib/x86/clmul.h
+-rw-r--r--   0 runner    (1001) docker     (123)    21337 2023-07-30 16:47:14.000000 MACS3-3.0.0b3/MACS3/fermi-lite/lib/x86/fma.h
+-rw-r--r--   0 runner    (1001) docker     (123)    31945 2023-07-30 16:47:14.000000 MACS3-3.0.0b3/MACS3/fermi-lite/lib/x86/gfni.h
+-rw-r--r--   0 runner    (1001) docker     (123)    76602 2023-07-30 16:47:14.000000 MACS3-3.0.0b3/MACS3/fermi-lite/lib/x86/mmx.h
+-rw-r--r--   0 runner    (1001) docker     (123)   144373 2023-07-30 16:47:14.000000 MACS3-3.0.0b3/MACS3/fermi-lite/lib/x86/sse.h
+-rw-r--r--   0 runner    (1001) docker     (123)   241454 2023-07-30 16:47:14.000000 MACS3-3.0.0b3/MACS3/fermi-lite/lib/x86/sse2.h
+-rw-r--r--   0 runner    (1001) docker     (123)    16133 2023-07-30 16:47:14.000000 MACS3-3.0.0b3/MACS3/fermi-lite/lib/x86/sse3.h
+-rw-r--r--   0 runner    (1001) docker     (123)    75653 2023-07-30 16:47:14.000000 MACS3-3.0.0b3/MACS3/fermi-lite/lib/x86/sse4.1.h
+-rw-r--r--   0 runner    (1001) docker     (123)    12626 2023-07-30 16:47:14.000000 MACS3-3.0.0b3/MACS3/fermi-lite/lib/x86/sse4.2.h
+-rw-r--r--   0 runner    (1001) docker     (123)    35506 2023-07-30 16:47:14.000000 MACS3-3.0.0b3/MACS3/fermi-lite/lib/x86/ssse3.h
+-rw-r--r--   0 runner    (1001) docker     (123)   398077 2023-07-30 16:47:14.000000 MACS3-3.0.0b3/MACS3/fermi-lite/lib/x86/svml.h
+-rw-r--r--   0 runner    (1001) docker     (123)    17555 2023-07-30 16:47:10.000000 MACS3-3.0.0b3/MACS3/fermi-lite/mag.c
+-rw-r--r--   0 runner    (1001) docker     (123)     1962 2023-07-30 16:47:10.000000 MACS3-3.0.0b3/MACS3/fermi-lite/mag.h
+-rw-r--r--   0 runner    (1001) docker     (123)     7850 2023-07-30 16:47:10.000000 MACS3-3.0.0b3/MACS3/fermi-lite/misc.c
+-rw-r--r--   0 runner    (1001) docker     (123)     8554 2023-07-30 16:47:10.000000 MACS3-3.0.0b3/MACS3/fermi-lite/mrope.c
+-rw-r--r--   0 runner    (1001) docker     (123)     2694 2023-07-30 16:47:10.000000 MACS3-3.0.0b3/MACS3/fermi-lite/mrope.h
+-rw-r--r--   0 runner    (1001) docker     (123)    13226 2023-07-30 16:47:10.000000 MACS3-3.0.0b3/MACS3/fermi-lite/rld0.c
+-rw-r--r--   0 runner    (1001) docker     (123)     4296 2023-07-30 16:47:10.000000 MACS3-3.0.0b3/MACS3/fermi-lite/rld0.h
+-rw-r--r--   0 runner    (1001) docker     (123)     4821 2023-07-30 16:47:10.000000 MACS3-3.0.0b3/MACS3/fermi-lite/rle.c
+-rw-r--r--   0 runner    (1001) docker     (123)     1941 2023-07-30 16:47:10.000000 MACS3-3.0.0b3/MACS3/fermi-lite/rle.h
+-rw-r--r--   0 runner    (1001) docker     (123)     6965 2023-07-30 16:47:10.000000 MACS3-3.0.0b3/MACS3/fermi-lite/rope.c
+-rw-r--r--   0 runner    (1001) docker     (123)     1428 2023-07-30 16:47:10.000000 MACS3-3.0.0b3/MACS3/fermi-lite/rope.h
+-rw-r--r--   0 runner    (1001) docker     (123)    15372 2023-07-30 16:47:10.000000 MACS3-3.0.0b3/MACS3/fermi-lite/unitig.c
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 16:49:27.450857 MACS3-3.0.0b3/MACS3.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     7947 2023-07-30 16:49:27.000000 MACS3-3.0.0b3/MACS3.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    11622 2023-07-30 16:49:27.000000 MACS3-3.0.0b3/MACS3.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-30 16:49:27.000000 MACS3-3.0.0b3/MACS3.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       57 2023-07-30 16:49:27.000000 MACS3-3.0.0b3/MACS3.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-07-30 16:49:27.000000 MACS3-3.0.0b3/MACS3.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      432 2023-07-30 16:47:10.000000 MACS3-3.0.0b3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     7947 2023-07-30 16:49:27.494857 MACS3-3.0.0b3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     7055 2023-07-30 16:47:10.000000 MACS3-3.0.0b3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 16:49:27.494857 MACS3-3.0.0b3/bin/
+-rw-r--r--   0 runner    (1001) docker     (123)    99146 2023-07-30 16:47:10.000000 MACS3-3.0.0b3/bin/macs3
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 16:49:27.494857 MACS3-3.0.0b3/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)     5815 2023-07-30 16:47:10.000000 MACS3-3.0.0b3/docs/INSTALL.md
+-rw-r--r--   0 runner    (1001) docker     (123)     3081 2023-07-30 16:47:10.000000 MACS3-3.0.0b3/docs/bdgbroadcall.md
+-rw-r--r--   0 runner    (1001) docker     (123)     2709 2023-07-30 16:47:10.000000 MACS3-3.0.0b3/docs/bdgcmp.md
+-rw-r--r--   0 runner    (1001) docker     (123)     3470 2023-07-30 16:47:10.000000 MACS3-3.0.0b3/docs/bdgdiff.md
+-rw-r--r--   0 runner    (1001) docker     (123)     2578 2023-07-30 16:47:10.000000 MACS3-3.0.0b3/docs/bdgopt.md
+-rw-r--r--   0 runner    (1001) docker     (123)     2790 2023-07-30 16:47:10.000000 MACS3-3.0.0b3/docs/bdgpeakcall.md
+-rw-r--r--   0 runner    (1001) docker     (123)    16724 2023-07-30 16:47:10.000000 MACS3-3.0.0b3/docs/callpeak.md
+-rw-r--r--   0 runner    (1001) docker     (123)     5267 2023-07-30 16:47:10.000000 MACS3-3.0.0b3/docs/callvar.md
+-rw-r--r--   0 runner    (1001) docker     (123)     2505 2023-07-30 16:47:10.000000 MACS3-3.0.0b3/docs/cmbreps.md
+-rw-r--r--   0 runner    (1001) docker     (123)     3682 2023-07-30 16:47:10.000000 MACS3-3.0.0b3/docs/filterdup.md
+-rw-r--r--   0 runner    (1001) docker     (123)     8564 2023-07-30 16:47:10.000000 MACS3-3.0.0b3/docs/hmmratac.md
+-rw-r--r--   0 runner    (1001) docker     (123)     3282 2023-07-30 16:47:10.000000 MACS3-3.0.0b3/docs/pileup.md
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-30 16:47:10.000000 MACS3-3.0.0b3/docs/predictd.md
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-30 16:47:10.000000 MACS3-3.0.0b3/docs/qa.md
+-rw-r--r--   0 runner    (1001) docker     (123)     3441 2023-07-30 16:47:10.000000 MACS3-3.0.0b3/docs/randsample.md
+-rw-r--r--   0 runner    (1001) docker     (123)     2936 2023-07-30 16:47:10.000000 MACS3-3.0.0b3/docs/refinepeak.md
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-30 16:47:10.000000 MACS3-3.0.0b3/docs/testing_in_docker.md
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-30 16:47:10.000000 MACS3-3.0.0b3/docs/tutorial.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1942 2023-07-30 16:47:10.000000 MACS3-3.0.0b3/make_docker_base.sh
+-rw-r--r--   0 runner    (1001) docker     (123)      130 2023-07-30 16:47:10.000000 MACS3-3.0.0b3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       87 2023-07-30 16:47:10.000000 MACS3-3.0.0b3/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-30 16:49:27.494857 MACS3-3.0.0b3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     9222 2023-07-30 16:47:10.000000 MACS3-3.0.0b3/setup.py
```

### Comparing `MACS3-3.0.0b2/ChangeLog` & `MACS3-3.0.0b3/ChangeLog`

 * *Files 2% similar despite different names*

```diff
@@ -1,66 +1,73 @@
-2023-06-23  Tao Liu  <vladimir.liu@gmail.com>
-	MACS 3.0.0b2
+2023-07-28  Tao Liu  <vladimir.liu@gmail.com>
+	MACS 3.0.0b3
+
 	* New features in MACS3:
 
 	1) Speed/memory optimization.  Use the cykhash to replace python
 	dictionary. Use buffer (10MB) to read and parse input file (not
 	available for BAM file parser). And many optimization tweaks. We
 	added memory monitoring to the runtime messages.
 
-	2) Code cleanup. Reorganize source codes. 
-
-	3) Unit testing. 
-
-	4) R wrappers for MACS -- MACSr
+	2) Call variants in peak regions directly from BAM files. The
+	function was originally developed under code name SAPPER. Now
+	SAPPER has been merged into MACS. Also, `simde` has been added as
+	a submodule in order to support fermi-lite library under non-x64
+	architectures.
 
-	5) Switch to Github Action for CI, support multi-arch testing 
-	including x64, armv7, aarch64, s390x and ppc64le. 
-
-	6) MACS tag-shifting model has been refined. Now it will use a 
-	naive peak calling approach to find ALL possible paired peaks at +
-	and - strand, then use all of them to calculate the 
-	cross-correlation. (a related bug has been fix #442) 
-
-	7) Call variants in peak regions directly from BAM files. The 
-	function was originally developed under code name SAPPER. Now 
-	SAPPER has been merged into MACS. Also, `simde` has been added as 
-	a submodule in order to support fermi-lite library under non-x64 
-	architectures. 
-
-	8) BAI index and random access to BAM file now is supported. #449 
-	And user can use original BAM file (instead of the subset of BAM 
-	file as in SAPPER) in the `callvar` command. 
-
-	9) Support of Python > 3.10 #497 #498 
-	
-	10) HMMRATAC module is added. HMMRATAC is a dedicated software to
+	3) HMMRATAC module is added. HMMRATAC is a dedicated software to
 	analyze ATAC-seq data. The basic idea behind HMMRATAC is to digest
 	ATAC-seq data according to the fragment length of read pairs into
 	four signal tracks: short fragments, mononucleosomal fragments,
 	di-nucleosomal fragments and tri-nucleosomal fragments. Then
 	integrate the four tracks again using Hidden Markov Model to
 	consider three hidden states: open region, nucleosomal region, and
 	background region. The orginal paper was published in 2019 written
 	in JAVA, by Evan Tarbell. We implemented it in Python/Cython and
 	optimize the whole process using existing MACS functions and
 	hmmlearn. Now it can run much faster than the original JAVA
-	version. Note: evaluation of the peak calling results is underway.
+	version. Note: evaluation of the peak calling results is underway.	
+
+	4) Code cleanup. Reorganize source codes. 
+
+	5) Unit testing. 
+
+	6) R wrappers for MACS -- MACSr
+
+	7) Switch to Github Action for CI, support multi-arch testing
+	including x64, armv7, aarch64, s390x and ppc64le. We also test on
+	Mac OS 12.
+
+	8) MACS tag-shifting model has been refined. Now it will use a 
+	naive peak calling approach to find ALL possible paired peaks at +
+	and - strand, then use all of them to calculate the 
+	cross-correlation. (a related bug has been fix #442) 
+
+	9) BAI index and random access to BAM file now is supported. #449
+	And user can use original BAM file (instead of the subset of BAM
+	file as in SAPPER) in the `callvar` command.
+
+	10) Support of Python > 3.10 #497 #498 
 
 	11) The effective genome size parameters have been updated
 	according to deeptools. #508
 
-	12) Memory usage now will be displayed in the runtime message.
-	
-	13) Multiple updates regarding dependencies, anaconda built, CI/CD
+	12) Multiple updates regarding dependencies, anaconda built, CI/CD
 	process.
-	
+
+	13) Cython support to ~0.29. Cython 3 is not supported yet.
+
 	* Other:
 	1) Missing header line while no peaks can be called #501 #502
 
+	2) Note: different numpy, scipy, sklearn may give slightly
+	different results for hmmratac results. The current standard
+	results for automated testing in `/test` directory are from Numpy
+	1.25.1, Scipy 1.11.1, and sklearn 1.3.0.
+
 2020-04-11  Tao Liu  <vladimir.liu@gmail.com>
 	MACS version 2.2.7.1
 
 	* hotfix:
 
 	Add 'wheel' and 'pip' to pyproject.toml so that `pip install` can
 	work.
```

### Comparing `MACS3-3.0.0b2/LICENSE` & `MACS3-3.0.0b3/LICENSE`

 * *Files identical despite different names*

### Comparing `MACS3-3.0.0b2/MACS3/Commands/bdgbroadcall_cmd.py` & `MACS3-3.0.0b3/MACS3/Commands/bdgbroadcall_cmd.py`

 * *Files identical despite different names*

### Comparing `MACS3-3.0.0b2/MACS3/Commands/bdgcmp_cmd.py` & `MACS3-3.0.0b3/MACS3/Commands/bdgcmp_cmd.py`

 * *Files identical despite different names*

### Comparing `MACS3-3.0.0b2/MACS3/Commands/bdgdiff_cmd.py` & `MACS3-3.0.0b3/MACS3/Commands/bdgdiff_cmd.py`

 * *Files identical despite different names*

### Comparing `MACS3-3.0.0b2/MACS3/Commands/bdgopt_cmd.py` & `MACS3-3.0.0b3/MACS3/Commands/bdgopt_cmd.py`

 * *Files identical despite different names*

### Comparing `MACS3-3.0.0b2/MACS3/Commands/bdgpeakcall_cmd.py` & `MACS3-3.0.0b3/MACS3/Commands/bdgpeakcall_cmd.py`

 * *Files identical despite different names*

### Comparing `MACS3-3.0.0b2/MACS3/Commands/callpeak_cmd.py` & `MACS3-3.0.0b3/MACS3/Commands/callpeak_cmd.py`

 * *Files identical despite different names*

### Comparing `MACS3-3.0.0b2/MACS3/Commands/callvar_cmd.py` & `MACS3-3.0.0b3/MACS3/Commands/callvar_cmd.py`

 * *Files identical despite different names*

### Comparing `MACS3-3.0.0b2/MACS3/Commands/cmbreps_cmd.py` & `MACS3-3.0.0b3/MACS3/Commands/cmbreps_cmd.py`

 * *Files identical despite different names*

### Comparing `MACS3-3.0.0b2/MACS3/Commands/diffpeak_cmd.py` & `MACS3-3.0.0b3/MACS3/Commands/diffpeak_cmd.py`

 * *Files identical despite different names*

### Comparing `MACS3-3.0.0b2/MACS3/Commands/filterdup_cmd.py` & `MACS3-3.0.0b3/MACS3/Commands/filterdup_cmd.py`

 * *Files identical despite different names*

### Comparing `MACS3-3.0.0b2/MACS3/Commands/hmmratac_cmd.py` & `MACS3-3.0.0b3/MACS3/Commands/hmmratac_cmd.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Time-stamp: <2023-06-08 11:03:46 Tao Liu>
+# Time-stamp: <2023-07-28 12:10:12 Tao Liu>
 
 """Description: Main HMMR command
 
 This code is free software; you can redistribute it and/or modify it
 under the terms of the BSD License (see the file LICENSE included with
 the distribution).
 """
@@ -139,15 +139,15 @@
     options.info( f"#  Compute the weights for each fragment length for each of the four signal types")
     fl_dict = petrack.count_fraglengths()
     fl_list = list(fl_dict.keys())
     fl_list.sort()
 
     # now we will prepare the weights for each fragment length for
     # each of the four distributions based on the EM results
-    weight_mapping = generate_weight_mapping( fl_list, em_means, em_stddevs )
+    weight_mapping = generate_weight_mapping( fl_list, em_means, em_stddevs, min_frag_p = options.min_frag_p )
     
     options.info( f"#  Generate short, mono-, di-, and tri-nucleosomal signals")
     digested_atac_signals = generate_digested_signals( petrack, weight_mapping )
 
     # save three types of signals if needed
     if options.save_digested:
         fhd = open(short_bdgfile,"w")
@@ -185,26 +185,39 @@
     if options.cutoff_analysis_only:
         # we will run cutoff analysis only and quit
         options.info( f"#3 Generate cutoff analysis report from {petrack.total} fragments")
         options.info( f"#   Please review the cutoff analysis result in {cutoffanalysis_file}" )
 
         # Let MACS3 do the cutoff analysis to help decide the lower and upper cutoffs
         with open(cutoffanalysis_file, "w") as ofhd_cutoff:
-            ofhd_cutoff.write( fc_bdg.cutoff_analysis( min_length=minlen, max_gap=options.hmm_training_flanking ) )
+            ofhd_cutoff.write( fc_bdg.cutoff_analysis( min_length=minlen, max_gap=options.hmm_training_flanking, max_score = 1000 ) )
         #raise Exception("Cutoff analysis only.")
         sys.exit(1)
         
         
     #############################################
     # 3. Define training set by peak calling
     #############################################
 
     if options.hmm_file:
         # skip this step if hmm_file is given
         options.info( f"#3 Skip this step of looking for training set since a Hidden Markov Model file has been provided!")
+    elif options.hmm_training_regions: 
+        # if a training region file is provided - need to read in the bedfile and skip the peak calling step
+        options.info(f"#3 Read training regions from BED file: {options.hmm_training_regions}")
+        # from refinepeak_cmd.py:
+        peakio = open(options.hmm_training_regions,"rb")
+        peaks = PeakIO()
+        for l in peakio:
+            fs = l.rstrip().split()
+            peaks.add( chromosome=fs[0], start=int(fs[1]), end=int(fs[2])) #change based on what expected input file should contain
+        peakio.close()
+        training_regions = Regions()
+        training_regions.init_from_PeakIO( peaks )
+        options.info("#  Training regions have been read from bedfile")
     else:
         # Find regions with fold change within determined range to use as training sites.
         # Find regions with zscore values above certain cutoff to exclude from viterbi.
         # 
         options.info( f"#3 Look for training set from {petrack.total} fragments" )
         options.info( f"#  Call peak above within fold-change range of {options.hmm_lower} and {options.hmm_upper}." )
         options.info( f"#   The minimum length of the region is set as the average template/fragment length in the dataset: {minlen}" )
@@ -219,15 +232,15 @@
         options.info( f"#   if the choices of lower, upper and prescanning cutoff are appropriate." )
         options.info( f"#   Please read the message in the section 'Choices of cutoff values' by running" )
         options.info( f"#   `macs3 hmmratac -h` for detail." )
         options.info( f"#  ****" )
         
         # Let MACS3 do the cutoff analysis to help decide the lower and upper cutoffs
         with open(cutoffanalysis_file, "w") as ofhd_cutoff:
-            ofhd_cutoff.write( fc_bdg.cutoff_analysis( min_length=minlen, max_gap=options.hmm_training_flanking ) )
+            ofhd_cutoff.write( fc_bdg.cutoff_analysis( min_length=minlen, max_gap=options.hmm_training_flanking, max_score = 1000 ) )
             
         # we will check if anything left after filtering
         if peaks.total > options.hmm_maxTrain:
             peaks = peaks.randomly_pick( options.hmm_maxTrain, seed = options.hmm_randomSeed )
             options.info( f"#  We randomly pick {options.hmm_maxTrain} regions for training" )
         elif peaks.total == 0:
             options.error( f"# No training regions found. Please adjust the lower or upper cutoff." )
@@ -295,14 +308,19 @@
 
         # last one is the nuc state (note it may not be accurate though
         i_nucleosomal_region = list(set([0, 1, 2]) - set([i_open_region, i_background_region]))[0]
 
         # write hmm into model file
         options.info( f"#  Write HMM parameters into JSON: {hmm_modelfile}")
         hmm_model_save( hmm_modelfile, hmm_model, options.hmm_binsize, i_open_region, i_nucleosomal_region, i_background_region )
+        
+        # if --modelonly option provided, exit script after hmm model is saved 
+        if options.hmm_modelonly:
+            options.info( f"#  Complete - HMM model was saved, program exited (--modelonly option was provided) ")
+            sys.exit()
 
     # Now tell users the parameters of the HMM
     assignments = [ "", "", "" ]
     assignments[ i_open_region ]        = "open"
     assignments[ i_nucleosomal_region ] = "nuc"
     assignments[ i_background_region ]  = "bg"
```

### Comparing `MACS3-3.0.0b2/MACS3/Commands/pileup_cmd.py` & `MACS3-3.0.0b3/MACS3/Commands/pileup_cmd.py`

 * *Files identical despite different names*

### Comparing `MACS3-3.0.0b2/MACS3/Commands/predictd_cmd.py` & `MACS3-3.0.0b3/MACS3/Commands/predictd_cmd.py`

 * *Files identical despite different names*

### Comparing `MACS3-3.0.0b2/MACS3/Commands/randsample_cmd.py` & `MACS3-3.0.0b3/MACS3/Commands/randsample_cmd.py`

 * *Files identical despite different names*

### Comparing `MACS3-3.0.0b2/MACS3/Commands/refinepeak_cmd.py` & `MACS3-3.0.0b3/MACS3/Commands/refinepeak_cmd.py`

 * *Files identical despite different names*

### Comparing `MACS3-3.0.0b2/MACS3/IO/BAM.pyx` & `MACS3-3.0.0b3/MACS3/IO/BAM.pyx`

 * *Files identical despite different names*

### Comparing `MACS3-3.0.0b2/MACS3/IO/BedGraphIO.pyx` & `MACS3-3.0.0b3/MACS3/IO/BedGraphIO.pyx`

 * *Files identical despite different names*

### Comparing `MACS3-3.0.0b2/MACS3/IO/OutputWriter.py` & `MACS3-3.0.0b3/MACS3/IO/OutputWriter.py`

 * *Files identical despite different names*

### Comparing `MACS3-3.0.0b2/MACS3/IO/Parser.pyx` & `MACS3-3.0.0b3/MACS3/IO/Parser.pyx`

 * *Files identical despite different names*

### Comparing `MACS3-3.0.0b2/MACS3/IO/PeakIO.pyx` & `MACS3-3.0.0b3/MACS3/IO/PeakIO.pyx`

 * *Files identical despite different names*

### Comparing `MACS3-3.0.0b2/MACS3/Signal/BedGraph.pyx` & `MACS3-3.0.0b3/MACS3/Signal/BedGraph.pyx`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # cython: language_level=3
 # cython: profile=True
-# Time-stamp: <2023-06-08 10:52:59 Tao Liu>
+# Time-stamp: <2023-07-28 12:06:48 Tao Liu>
 
 """Module for BedGraph data class.
 
 This code is free software; you can redistribute it and/or modify it
 under the terms of the BSD License (see the file LICENSE included with
 the distribution).
 """
@@ -1127,15 +1127,15 @@
                 # meet the end of either bedGraphTrackI, simply exit
                 pass
 
         ret.finalize()
         #ret.merge_regions()
         return ret
 
-    cpdef str cutoff_analysis ( self, int32_t max_gap, int32_t min_length, int32_t steps = 100 ):
+    cpdef str cutoff_analysis ( self, int32_t max_gap, int32_t min_length, int32_t steps = 100, float32_t max_score = 1000 ):
         """
         Cutoff analysis function for bedGraphTrackI object.
     
         This function will try all possible cutoff values on the score column to call peaks. Then 
         will give a report of a number of metrics (number of peaks, total length of peaks, average
         length of peak) at varying score cutoffs. For each score cutoff, the function finds the 
         positions where the score exceeds the cutoff, then groups those positions into "peaks" 
@@ -1167,16 +1167,16 @@
             #dict cutoff_npeaks, cutoff_lpeaks
             float32_t s, midvalue
 
         chrs = self.get_chr_names()
 
         #midvalue = self.minvalue/2 + self.maxvalue/2
         #s = float(self.minvalue - midvalue)/steps
-        minv = self.minvalue
-        maxv = self.maxvalue
+        minv = max( 0, self.minvalue )
+        maxv = min( self.maxvalue, max_score )
 
         s = float(maxv - minv)/steps
 
         # a list of possible cutoff values from minv to maxv with step of s
         cutoff_list = [round(value, 3) for value in np.arange(minv, maxv, s)]
 
         cutoff_npeaks = [0] * len( cutoff_list )
@@ -1261,8 +1261,8 @@
     
     # Calculate the average change in slope
     avg_delta_slope = np.mean(delta_slopes)
     
     # Find all points where the change in slope is significantly larger than the average
     elbows = np.where(delta_slopes > avg_delta_slope + threshold)[0]
     
-    return elbows
+    return elbows
```

### Comparing `MACS3-3.0.0b2/MACS3/Signal/CallPeakUnit.pyx` & `MACS3-3.0.0b3/MACS3/Signal/CallPeakUnit.pyx`

 * *Files identical despite different names*

### Comparing `MACS3-3.0.0b2/MACS3/Signal/FixWidthTrack.pyx` & `MACS3-3.0.0b3/MACS3/Signal/FixWidthTrack.pyx`

 * *Files identical despite different names*

### Comparing `MACS3-3.0.0b2/MACS3/Signal/HMMR_EM.pyx` & `MACS3-3.0.0b3/MACS3/Signal/HMMR_EM.pyx`

 * *Files identical despite different names*

### Comparing `MACS3-3.0.0b2/MACS3/Signal/HMMR_HMM.pyx` & `MACS3-3.0.0b3/MACS3/Signal/HMMR_HMM.pyx`

 * *Files identical despite different names*

### Comparing `MACS3-3.0.0b2/MACS3/Signal/HMMR_Signal_Processing.pyx` & `MACS3-3.0.0b3/MACS3/Signal/HMMR_Signal_Processing.pyx`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # cython: language_level=3
 # cython: profile=True
-# Time-stamp: <2023-06-08 00:28:40 Tao Liu>
+# Time-stamp: <2023-07-28 12:14:57 Tao Liu>
 
 """Module description:
 
 This code is free software; you can redistribute it and/or modify it
 under the terms of the BSD License (see the file LICENSE included with
 the distribution).
 """
@@ -51,15 +51,15 @@
 # ------------------------------------
 # Classes
 # ------------------------------------
 # ------------------------------------
 # public functions
 # ------------------------------------
 
-cpdef list generate_weight_mapping( list fraglen_list, list means, list stddevs ):
+cpdef list generate_weight_mapping( list fraglen_list, list means, list stddevs, float min_frag_p = 0.001 ):
     """Generate weights for each fragment length in short, mono, di, and tri-signals track
 
     return: list of four dictionaries, with key as fraglen and value as the weight.
             ret[0] -- dictionary for short
             ret[1] -- dictionary for mono
             ret[2] -- dictionary for di
             ret[3] -- dictionary for tri
@@ -67,37 +67,44 @@
     cdef:
         list ret_mapping
         list variances
         int l
         float m_s, m_m, m_d, m_t
         float v_s, v_m, v_d, v_t
         float p_s, p_m, p_d, p_t
-        float w_s, w_m, w_d, w_t
         float s
         int i, j
     assert len(means) == 4
     assert len(stddevs) == 4
     [m_s, m_m, m_d, m_t] = means
     [v_s, v_m, v_d, v_t] = [ x**2 for x in stddevs ]
     ret_mapping = [ {}, {}, {}, {} ]
     for i in range( len(fraglen_list) ):
         l = fraglen_list[ i ]
         p_s = pnorm2( float(l), m_s, v_s )
         p_m = pnorm2( float(l), m_m, v_m )
         p_d = pnorm2( float(l), m_d, v_d )
         p_t = pnorm2( float(l), m_t, v_t )
         s = p_s + p_m + p_d + p_t
-        w_s = p_s / s
-        w_m = p_m / s
-        w_d = p_d / s
-        w_t = p_t / s
-        ret_mapping[ 0 ][ l ] = w_s
-        ret_mapping[ 1 ][ l ] = w_m
-        ret_mapping[ 2 ][ l ] = w_d
-        ret_mapping[ 3 ][ l ] = w_t
+        if p_s < min_frag_p and p_m < min_frag_p and p_d < min_frag_p and p_t < min_frag_p:
+            # we exclude the fragment which can't be assigned to
+            # short, mono, di-nuc, and tri-nuc (likelihood <
+            # min_frag_p, default:0.001) Normally this fragment is too
+            # large. We exclude these fragment by setting all weights
+            # to zero.
+            debug(f"The fragment length {l} can't be assigned to either distribution so will be excluded!")
+            ret_mapping[ 0 ][ l ] = 0
+            ret_mapping[ 1 ][ l ] = 0
+            ret_mapping[ 2 ][ l ] = 0
+            ret_mapping[ 3 ][ l ] = 0
+            continue
+        ret_mapping[ 0 ][ l ] = p_s / s
+        ret_mapping[ 1 ][ l ] = p_m / s
+        ret_mapping[ 2 ][ l ] = p_d / s
+        ret_mapping[ 3 ][ l ] = p_t / s
     return ret_mapping
 
 cpdef list generate_digested_signals( object petrack, list weight_mapping ):
     """Generate digested pileup signals (four tracks) using weight mapping 
 
     return: list of four signals in dictionary, with key as chromosome name and value as a p-v array.
             ret[0] -- dictionary for short
```

### Comparing `MACS3-3.0.0b2/MACS3/Signal/PairedEndTrack.pyx` & `MACS3-3.0.0b3/MACS3/Signal/PairedEndTrack.pyx`

 * *Files identical despite different names*

### Comparing `MACS3-3.0.0b2/MACS3/Signal/PeakDetect.pyx` & `MACS3-3.0.0b3/MACS3/Signal/PeakDetect.pyx`

 * *Files identical despite different names*

### Comparing `MACS3-3.0.0b2/MACS3/Signal/PeakModel.pyx` & `MACS3-3.0.0b3/MACS3/Signal/PeakModel.pyx`

 * *Files identical despite different names*

### Comparing `MACS3-3.0.0b2/MACS3/Signal/PeakVariants.pyx` & `MACS3-3.0.0b3/MACS3/Signal/PeakVariants.pyx`

 * *Files identical despite different names*

### Comparing `MACS3-3.0.0b2/MACS3/Signal/Pileup.pyx` & `MACS3-3.0.0b3/MACS3/Signal/Pileup.pyx`

 * *Files identical despite different names*

### Comparing `MACS3-3.0.0b2/MACS3/Signal/PileupV2.pyx` & `MACS3-3.0.0b3/MACS3/Signal/PileupV2.pyx`

 * *Files identical despite different names*

### Comparing `MACS3-3.0.0b2/MACS3/Signal/PosReadsInfo.pyx` & `MACS3-3.0.0b3/MACS3/Signal/PosReadsInfo.pyx`

 * *Files identical despite different names*

### Comparing `MACS3-3.0.0b2/MACS3/Signal/Prob.pyx` & `MACS3-3.0.0b3/MACS3/Signal/Prob.pyx`

 * *Files identical despite different names*

### Comparing `MACS3-3.0.0b2/MACS3/Signal/RACollection.pyx` & `MACS3-3.0.0b3/MACS3/Signal/RACollection.pyx`

 * *Files identical despite different names*

### Comparing `MACS3-3.0.0b2/MACS3/Signal/ReadAlignment.pyx` & `MACS3-3.0.0b3/MACS3/Signal/ReadAlignment.pyx`

 * *Files identical despite different names*

### Comparing `MACS3-3.0.0b2/MACS3/Signal/Region.pyx` & `MACS3-3.0.0b3/MACS3/Signal/Region.pyx`

 * *Files identical despite different names*

### Comparing `MACS3-3.0.0b2/MACS3/Signal/ScoreTrack.pyx` & `MACS3-3.0.0b3/MACS3/Signal/ScoreTrack.pyx`

 * *Files identical despite different names*

### Comparing `MACS3-3.0.0b2/MACS3/Signal/SignalProcessing.pyx` & `MACS3-3.0.0b3/MACS3/Signal/SignalProcessing.pyx`

 * *Files identical despite different names*

### Comparing `MACS3-3.0.0b2/MACS3/Signal/UnitigRACollection.pyx` & `MACS3-3.0.0b3/MACS3/Signal/UnitigRACollection.pyx`

 * *Files identical despite different names*

### Comparing `MACS3-3.0.0b2/MACS3/Signal/VariantStat.pyx` & `MACS3-3.0.0b3/MACS3/Signal/VariantStat.pyx`

 * *Files identical despite different names*

### Comparing `MACS3-3.0.0b2/MACS3/Signal/cPosValCalculation.c` & `MACS3-3.0.0b3/MACS3/Signal/cPosValCalculation.c`

 * *Files identical despite different names*

### Comparing `MACS3-3.0.0b2/MACS3/Signal/cPosValCalculation.h` & `MACS3-3.0.0b3/MACS3/Signal/cPosValCalculation.h`

 * *Files identical despite different names*

### Comparing `MACS3-3.0.0b2/MACS3/Signal/cPosValCalculation.pxd` & `MACS3-3.0.0b3/MACS3/Signal/cPosValCalculation.pxd`

 * *Files identical despite different names*

### Comparing `MACS3-3.0.0b2/MACS3/Signal/swalign.c` & `MACS3-3.0.0b3/MACS3/Signal/swalign.c`

 * *Files identical despite different names*

### Comparing `MACS3-3.0.0b2/MACS3/Signal/swalign.h` & `MACS3-3.0.0b3/MACS3/Signal/swalign.h`

 * *Files identical despite different names*

### Comparing `MACS3-3.0.0b2/MACS3/Utilities/Constants.py` & `MACS3-3.0.0b3/MACS3/Utilities/Constants.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-MACS_VERSION = "3.0.0b2"
+MACS_VERSION = "3.0.0b3"
 MAX_PAIRNUM = 1000
 MAX_LAMBDA  = 100000
 FESTEP      = 20
 BUFFER_SIZE = 100000                   # np array will increase at step of 1 million items
 READ_BUFFER_SIZE = 10000000            # 10M bytes for read buffer size
 N_MP = 2                               # Number of processers
```

### Comparing `MACS3-3.0.0b2/MACS3/Utilities/Logger.py` & `MACS3-3.0.0b3/MACS3/Utilities/Logger.py`

 * *Files identical despite different names*

### Comparing `MACS3-3.0.0b2/MACS3/Utilities/OptValidator.py` & `MACS3-3.0.0b3/MACS3/Utilities/OptValidator.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Time-stamp: <2022-06-10 10:24:34 Tao Liu>
+# Time-stamp: <2023-07-28 12:17:28 Tao Liu>
 
 """Module Description
 
 This code is free software; you can redistribute it and/or modify it
 under the terms of the BSD License (see the file LICENSE included with
 the distribution).
 """
@@ -806,14 +806,18 @@
         logger.error(" --means should not be negative! ")
         sys.exit( 1 )
     # em_stddev non-negative
     if sum( [ x < 0 for x in options.em_stddevs ] ):
         logger.error(" --stddev should not be negative! ")
         sys.exit( 1 )
 
+    # min_frag_p between 0 and 1
+    if options.min_frag_p <=0 or options.min_frag_p >= 1:
+        logger.error(" --min-frag-p should be larger than 0 and smaller than 1! ")
+        sys.exit( 1 )
 
     # HMM
     # hmm_states non-negative int, warn if not k=3
     #if options.hmm_states <=0:
     #    logger.error(" -s, --states must be an integer >= 0.")
     #    sys.exit( 1 )
     #elif options.hmm_states != 3 and options.hmm_states > 0 and options.store_peaks == False:
@@ -837,16 +841,16 @@
     
     # hmm_maxTrain non-negative
     if options.hmm_maxTrain <= 0:
         logger.error(" --maxTrain should be larger than 0!")
         sys.exit( 1 )
     
     # hmm_training_regions
-    #if options.hmm_training_regions:
-    #    options.argtxt += "# Using -t, --training input to train HMM instead of using fold change settings to select. \n"
+    if options.hmm_training_regions:
+       options.argtxt += "# Using -t, --training input to train HMM instead of using fold change settings to select. \n"
     
     # hmm_zscore non-negative
     #if options.hmm_zscore <0:
     #    logger.error(" -z, --zscore should not be negative!")
     #    sys.exit( 1 )
     
     # hmm_randomSeed
@@ -859,16 +863,16 @@
     #    sys.exit( 1 )
 
     # hmm_file
     #if options.hmm_file:
     #    options.argtxt += "# HMM training will be skipped, --model input used instead. \n"
 
     # hmm_modelonly
-    #if options.hmm_modelonly:
-    #    options.argtxt += "# Program will stop after generating model, which can be later applied with '--model'. \n"
+    if options.hmm_modelonly:
+       options.argtxt += "# Program will stop after generating model, which can be later applied with '--model'. \n"
 
 
     # Peak Calling
     if options.prescan_cutoff <= 1:
         logger.error(" In order to use -c or --prescan-cutoff, the cutoff must be larger than 1.")
         sys.exit( 1 )
```

### Comparing `MACS3-3.0.0b2/MACS3/fermi-lite/bfc.c` & `MACS3-3.0.0b3/MACS3/fermi-lite/bfc.c`

 * *Files identical despite different names*

### Comparing `MACS3-3.0.0b2/MACS3/fermi-lite/bseq.c` & `MACS3-3.0.0b3/MACS3/fermi-lite/bseq.c`

 * *Files identical despite different names*

### Comparing `MACS3-3.0.0b2/MACS3/fermi-lite/bubble.c` & `MACS3-3.0.0b3/MACS3/fermi-lite/bubble.c`

 * *Files identical despite different names*

### Comparing `MACS3-3.0.0b2/MACS3/fermi-lite/example.c` & `MACS3-3.0.0b3/MACS3/fermi-lite/example.c`

 * *Files identical despite different names*

### Comparing `MACS3-3.0.0b2/MACS3/fermi-lite/fml.h` & `MACS3-3.0.0b3/MACS3/fermi-lite/fml.h`

 * *Files identical despite different names*

### Comparing `MACS3-3.0.0b2/MACS3/fermi-lite/htab.c` & `MACS3-3.0.0b3/MACS3/fermi-lite/htab.c`

 * *Files identical despite different names*

### Comparing `MACS3-3.0.0b2/MACS3/fermi-lite/htab.h` & `MACS3-3.0.0b3/MACS3/fermi-lite/htab.h`

 * *Files identical despite different names*

### Comparing `MACS3-3.0.0b2/MACS3/fermi-lite/khash.h` & `MACS3-3.0.0b3/MACS3/fermi-lite/khash.h`

 * *Files identical despite different names*

### Comparing `MACS3-3.0.0b2/MACS3/fermi-lite/kmer.h` & `MACS3-3.0.0b3/MACS3/fermi-lite/kmer.h`

 * *Files identical despite different names*

### Comparing `MACS3-3.0.0b2/MACS3/fermi-lite/kseq.h` & `MACS3-3.0.0b3/MACS3/fermi-lite/kseq.h`

 * *Files identical despite different names*

### Comparing `MACS3-3.0.0b2/MACS3/fermi-lite/ksort.h` & `MACS3-3.0.0b3/MACS3/fermi-lite/ksort.h`

 * *Files identical despite different names*

### Comparing `MACS3-3.0.0b2/MACS3/fermi-lite/kstring.h` & `MACS3-3.0.0b3/MACS3/fermi-lite/kstring.h`

 * *Files identical despite different names*

### Comparing `MACS3-3.0.0b2/MACS3/fermi-lite/ksw.c` & `MACS3-3.0.0b3/MACS3/fermi-lite/ksw.c`

 * *Files identical despite different names*

### Comparing `MACS3-3.0.0b2/MACS3/fermi-lite/ksw.h` & `MACS3-3.0.0b3/MACS3/fermi-lite/ksw.h`

 * *Files identical despite different names*

### Comparing `MACS3-3.0.0b2/MACS3/fermi-lite/kthread.c` & `MACS3-3.0.0b3/MACS3/fermi-lite/kthread.c`

 * *Files identical despite different names*

### Comparing `MACS3-3.0.0b2/MACS3/fermi-lite/kvec.h` & `MACS3-3.0.0b3/MACS3/fermi-lite/kvec.h`

 * *Files identical despite different names*

### Comparing `MACS3-3.0.0b2/MACS3/fermi-lite/lib/arm/neon/aba.h` & `MACS3-3.0.0b3/MACS3/fermi-lite/lib/arm/neon/aba.h`

 * *Files identical despite different names*

### Comparing `MACS3-3.0.0b2/MACS3/fermi-lite/lib/arm/neon/abd.h` & `MACS3-3.0.0b3/MACS3/fermi-lite/lib/arm/neon/abd.h`

 * *Files identical despite different names*

### Comparing `MACS3-3.0.0b2/MACS3/fermi-lite/lib/arm/neon/abdl.h` & `MACS3-3.0.0b3/MACS3/fermi-lite/lib/arm/neon/abdl.h`

 * *Files identical despite different names*

### Comparing `MACS3-3.0.0b2/MACS3/fermi-lite/lib/arm/neon/abs.h` & `MACS3-3.0.0b3/MACS3/fermi-lite/lib/arm/neon/abs.h`

 * *Files identical despite different names*

### Comparing `MACS3-3.0.0b2/MACS3/fermi-lite/lib/arm/neon/add.h` & `MACS3-3.0.0b3/MACS3/fermi-lite/lib/arm/neon/add.h`

 * *Files identical despite different names*

### Comparing `MACS3-3.0.0b2/MACS3/fermi-lite/lib/arm/neon/addl.h` & `MACS3-3.0.0b3/MACS3/fermi-lite/lib/arm/neon/addl.h`

 * *Files identical despite different names*

### Comparing `MACS3-3.0.0b2/MACS3/fermi-lite/lib/arm/neon/addl_high.h` & `MACS3-3.0.0b3/MACS3/fermi-lite/lib/arm/neon/addl_high.h`

 * *Files identical despite different names*

### Comparing `MACS3-3.0.0b2/MACS3/fermi-lite/lib/arm/neon/addlv.h` & `MACS3-3.0.0b3/MACS3/fermi-lite/lib/arm/neon/addlv.h`

 * *Files identical despite different names*

### Comparing `MACS3-3.0.0b2/MACS3/fermi-lite/lib/arm/neon/addv.h` & `MACS3-3.0.0b3/MACS3/fermi-lite/lib/arm/neon/addv.h`

 * *Files identical despite different names*

### Comparing `MACS3-3.0.0b2/MACS3/fermi-lite/lib/arm/neon/addw.h` & `MACS3-3.0.0b3/MACS3/fermi-lite/lib/arm/neon/addw.h`

 * *Files identical despite different names*

### Comparing `MACS3-3.0.0b2/MACS3/fermi-lite/lib/arm/neon/addw_high.h` & `MACS3-3.0.0b3/MACS3/fermi-lite/lib/arm/neon/addw_high.h`

 * *Files identical despite different names*

### Comparing `MACS3-3.0.0b2/MACS3/fermi-lite/lib/arm/neon/and.h` & `MACS3-3.0.0b3/MACS3/fermi-lite/lib/arm/neon/and.h`

 * *Files identical despite different names*

### Comparing `MACS3-3.0.0b2/MACS3/fermi-lite/lib/arm/neon/bic.h` & `MACS3-3.0.0b3/MACS3/fermi-lite/lib/arm/neon/bic.h`

 * *Files identical despite different names*

### Comparing `MACS3-3.0.0b2/MACS3/fermi-lite/lib/arm/neon/bsl.h` & `MACS3-3.0.0b3/MACS3/fermi-lite/lib/arm/neon/bsl.h`

 * *Files identical despite different names*

### Comparing `MACS3-3.0.0b2/MACS3/fermi-lite/lib/arm/neon/cagt.h` & `MACS3-3.0.0b3/MACS3/fermi-lite/lib/arm/neon/cagt.h`

 * *Files identical despite different names*

### Comparing `MACS3-3.0.0b2/MACS3/fermi-lite/lib/arm/neon/ceq.h` & `MACS3-3.0.0b3/MACS3/fermi-lite/lib/arm/neon/ceq.h`

 * *Files identical despite different names*

### Comparing `MACS3-3.0.0b2/MACS3/fermi-lite/lib/arm/neon/ceqz.h` & `MACS3-3.0.0b3/MACS3/fermi-lite/lib/arm/neon/ceqz.h`

 * *Files identical despite different names*

### Comparing `MACS3-3.0.0b2/MACS3/fermi-lite/lib/arm/neon/cge.h` & `MACS3-3.0.0b3/MACS3/fermi-lite/lib/arm/neon/cge.h`

 * *Files identical despite different names*

### Comparing `MACS3-3.0.0b2/MACS3/fermi-lite/lib/arm/neon/cgez.h` & `MACS3-3.0.0b3/MACS3/fermi-lite/lib/arm/neon/cgez.h`

 * *Files identical despite different names*

### Comparing `MACS3-3.0.0b2/MACS3/fermi-lite/lib/arm/neon/cgt.h` & `MACS3-3.0.0b3/MACS3/fermi-lite/lib/arm/neon/cgt.h`

 * *Files identical despite different names*

### Comparing `MACS3-3.0.0b2/MACS3/fermi-lite/lib/arm/neon/cgtz.h` & `MACS3-3.0.0b3/MACS3/fermi-lite/lib/arm/neon/cgtz.h`

 * *Files identical despite different names*

### Comparing `MACS3-3.0.0b2/MACS3/fermi-lite/lib/arm/neon/cle.h` & `MACS3-3.0.0b3/MACS3/fermi-lite/lib/arm/neon/cle.h`

 * *Files identical despite different names*

### Comparing `MACS3-3.0.0b2/MACS3/fermi-lite/lib/arm/neon/clez.h` & `MACS3-3.0.0b3/MACS3/fermi-lite/lib/arm/neon/clez.h`

 * *Files identical despite different names*

### Comparing `MACS3-3.0.0b2/MACS3/fermi-lite/lib/arm/neon/cls.h` & `MACS3-3.0.0b3/MACS3/fermi-lite/lib/arm/neon/cls.h`

 * *Files identical despite different names*

### Comparing `MACS3-3.0.0b2/MACS3/fermi-lite/lib/arm/neon/clt.h` & `MACS3-3.0.0b3/MACS3/fermi-lite/lib/arm/neon/clt.h`

 * *Files identical despite different names*

### Comparing `MACS3-3.0.0b2/MACS3/fermi-lite/lib/arm/neon/cltz.h` & `MACS3-3.0.0b3/MACS3/fermi-lite/lib/arm/neon/cltz.h`

 * *Files identical despite different names*

### Comparing `MACS3-3.0.0b2/MACS3/fermi-lite/lib/arm/neon/clz.h` & `MACS3-3.0.0b3/MACS3/fermi-lite/lib/arm/neon/clz.h`

 * *Files identical despite different names*

### Comparing `MACS3-3.0.0b2/MACS3/fermi-lite/lib/arm/neon/cnt.h` & `MACS3-3.0.0b3/MACS3/fermi-lite/lib/arm/neon/cnt.h`

 * *Files identical despite different names*

### Comparing `MACS3-3.0.0b2/MACS3/fermi-lite/lib/arm/neon/combine.h` & `MACS3-3.0.0b3/MACS3/fermi-lite/lib/arm/neon/combine.h`

 * *Files identical despite different names*

### Comparing `MACS3-3.0.0b2/MACS3/fermi-lite/lib/arm/neon/create.h` & `MACS3-3.0.0b3/MACS3/fermi-lite/lib/arm/neon/create.h`

 * *Files identical despite different names*

### Comparing `MACS3-3.0.0b2/MACS3/fermi-lite/lib/arm/neon/cvt.h` & `MACS3-3.0.0b3/MACS3/fermi-lite/lib/arm/neon/cvt.h`

 * *Files identical despite different names*

### Comparing `MACS3-3.0.0b2/MACS3/fermi-lite/lib/arm/neon/dot.h` & `MACS3-3.0.0b3/MACS3/fermi-lite/lib/arm/neon/dot.h`

 * *Files identical despite different names*

### Comparing `MACS3-3.0.0b2/MACS3/fermi-lite/lib/arm/neon/dot_lane.h` & `MACS3-3.0.0b3/MACS3/fermi-lite/lib/arm/neon/dot_lane.h`

 * *Files identical despite different names*

### Comparing `MACS3-3.0.0b2/MACS3/fermi-lite/lib/arm/neon/dup_lane.h` & `MACS3-3.0.0b3/MACS3/fermi-lite/lib/arm/neon/dup_lane.h`

 * *Files identical despite different names*

### Comparing `MACS3-3.0.0b2/MACS3/fermi-lite/lib/arm/neon/dup_n.h` & `MACS3-3.0.0b3/MACS3/fermi-lite/lib/arm/neon/dup_n.h`

 * *Files identical despite different names*

### Comparing `MACS3-3.0.0b2/MACS3/fermi-lite/lib/arm/neon/eor.h` & `MACS3-3.0.0b3/MACS3/fermi-lite/lib/arm/neon/eor.h`

 * *Files identical despite different names*

### Comparing `MACS3-3.0.0b2/MACS3/fermi-lite/lib/arm/neon/ext.h` & `MACS3-3.0.0b3/MACS3/fermi-lite/lib/arm/neon/ext.h`

 * *Files identical despite different names*

### Comparing `MACS3-3.0.0b2/MACS3/fermi-lite/lib/arm/neon/get_high.h` & `MACS3-3.0.0b3/MACS3/fermi-lite/lib/arm/neon/get_high.h`

 * *Files identical despite different names*

### Comparing `MACS3-3.0.0b2/MACS3/fermi-lite/lib/arm/neon/get_lane.h` & `MACS3-3.0.0b3/MACS3/fermi-lite/lib/arm/neon/get_lane.h`

 * *Files identical despite different names*

### Comparing `MACS3-3.0.0b2/MACS3/fermi-lite/lib/arm/neon/get_low.h` & `MACS3-3.0.0b3/MACS3/fermi-lite/lib/arm/neon/get_low.h`

 * *Files identical despite different names*

### Comparing `MACS3-3.0.0b2/MACS3/fermi-lite/lib/arm/neon/hadd.h` & `MACS3-3.0.0b3/MACS3/fermi-lite/lib/arm/neon/hadd.h`

 * *Files identical despite different names*

### Comparing `MACS3-3.0.0b2/MACS3/fermi-lite/lib/arm/neon/hsub.h` & `MACS3-3.0.0b3/MACS3/fermi-lite/lib/arm/neon/hsub.h`

 * *Files identical despite different names*

### Comparing `MACS3-3.0.0b2/MACS3/fermi-lite/lib/arm/neon/ld1.h` & `MACS3-3.0.0b3/MACS3/fermi-lite/lib/arm/neon/ld1.h`

 * *Files identical despite different names*

### Comparing `MACS3-3.0.0b2/MACS3/fermi-lite/lib/arm/neon/ld3.h` & `MACS3-3.0.0b3/MACS3/fermi-lite/lib/arm/neon/ld3.h`

 * *Files identical despite different names*

### Comparing `MACS3-3.0.0b2/MACS3/fermi-lite/lib/arm/neon/ld4.h` & `MACS3-3.0.0b3/MACS3/fermi-lite/lib/arm/neon/ld4.h`

 * *Files identical despite different names*

### Comparing `MACS3-3.0.0b2/MACS3/fermi-lite/lib/arm/neon/max.h` & `MACS3-3.0.0b3/MACS3/fermi-lite/lib/arm/neon/max.h`

 * *Files identical despite different names*

### Comparing `MACS3-3.0.0b2/MACS3/fermi-lite/lib/arm/neon/maxnm.h` & `MACS3-3.0.0b3/MACS3/fermi-lite/lib/arm/neon/maxnm.h`

 * *Files identical despite different names*

### Comparing `MACS3-3.0.0b2/MACS3/fermi-lite/lib/arm/neon/maxv.h` & `MACS3-3.0.0b3/MACS3/fermi-lite/lib/arm/neon/maxv.h`

 * *Files identical despite different names*

### Comparing `MACS3-3.0.0b2/MACS3/fermi-lite/lib/arm/neon/min.h` & `MACS3-3.0.0b3/MACS3/fermi-lite/lib/arm/neon/min.h`

 * *Files identical despite different names*

### Comparing `MACS3-3.0.0b2/MACS3/fermi-lite/lib/arm/neon/minnm.h` & `MACS3-3.0.0b3/MACS3/fermi-lite/lib/arm/neon/minnm.h`

 * *Files identical despite different names*

### Comparing `MACS3-3.0.0b2/MACS3/fermi-lite/lib/arm/neon/minv.h` & `MACS3-3.0.0b3/MACS3/fermi-lite/lib/arm/neon/minv.h`

 * *Files identical despite different names*

### Comparing `MACS3-3.0.0b2/MACS3/fermi-lite/lib/arm/neon/mla.h` & `MACS3-3.0.0b3/MACS3/fermi-lite/lib/arm/neon/mla.h`

 * *Files identical despite different names*

### Comparing `MACS3-3.0.0b2/MACS3/fermi-lite/lib/arm/neon/mla_n.h` & `MACS3-3.0.0b3/MACS3/fermi-lite/lib/arm/neon/mla_n.h`

 * *Files identical despite different names*

### Comparing `MACS3-3.0.0b2/MACS3/fermi-lite/lib/arm/neon/mlal.h` & `MACS3-3.0.0b3/MACS3/fermi-lite/lib/arm/neon/mlal.h`

 * *Files identical despite different names*

### Comparing `MACS3-3.0.0b2/MACS3/fermi-lite/lib/arm/neon/mlal_high.h` & `MACS3-3.0.0b3/MACS3/fermi-lite/lib/arm/neon/mlal_high.h`

 * *Files identical despite different names*

### Comparing `MACS3-3.0.0b2/MACS3/fermi-lite/lib/arm/neon/mlal_n.h` & `MACS3-3.0.0b3/MACS3/fermi-lite/lib/arm/neon/mlal_n.h`

 * *Files identical despite different names*

### Comparing `MACS3-3.0.0b2/MACS3/fermi-lite/lib/arm/neon/mls.h` & `MACS3-3.0.0b3/MACS3/fermi-lite/lib/arm/neon/mls.h`

 * *Files identical despite different names*

### Comparing `MACS3-3.0.0b2/MACS3/fermi-lite/lib/arm/neon/mlsl.h` & `MACS3-3.0.0b3/MACS3/fermi-lite/lib/arm/neon/mlsl.h`

 * *Files identical despite different names*

### Comparing `MACS3-3.0.0b2/MACS3/fermi-lite/lib/arm/neon/mlsl_high.h` & `MACS3-3.0.0b3/MACS3/fermi-lite/lib/arm/neon/mlsl_high.h`

 * *Files identical despite different names*

### Comparing `MACS3-3.0.0b2/MACS3/fermi-lite/lib/arm/neon/mlsl_n.h` & `MACS3-3.0.0b3/MACS3/fermi-lite/lib/arm/neon/mlsl_n.h`

 * *Files identical despite different names*

### Comparing `MACS3-3.0.0b2/MACS3/fermi-lite/lib/arm/neon/movl.h` & `MACS3-3.0.0b3/MACS3/fermi-lite/lib/arm/neon/movl.h`

 * *Files identical despite different names*

### Comparing `MACS3-3.0.0b2/MACS3/fermi-lite/lib/arm/neon/movl_high.h` & `MACS3-3.0.0b3/MACS3/fermi-lite/lib/arm/neon/movl_high.h`

 * *Files identical despite different names*

### Comparing `MACS3-3.0.0b2/MACS3/fermi-lite/lib/arm/neon/movn.h` & `MACS3-3.0.0b3/MACS3/fermi-lite/lib/arm/neon/movn.h`

 * *Files identical despite different names*

### Comparing `MACS3-3.0.0b2/MACS3/fermi-lite/lib/arm/neon/movn_high.h` & `MACS3-3.0.0b3/MACS3/fermi-lite/lib/arm/neon/movn_high.h`

 * *Files identical despite different names*

### Comparing `MACS3-3.0.0b2/MACS3/fermi-lite/lib/arm/neon/mul.h` & `MACS3-3.0.0b3/MACS3/fermi-lite/lib/arm/neon/mul.h`

 * *Files identical despite different names*

### Comparing `MACS3-3.0.0b2/MACS3/fermi-lite/lib/arm/neon/mul_lane.h` & `MACS3-3.0.0b3/MACS3/fermi-lite/lib/arm/neon/mul_lane.h`

 * *Files identical despite different names*

### Comparing `MACS3-3.0.0b2/MACS3/fermi-lite/lib/arm/neon/mul_n.h` & `MACS3-3.0.0b3/MACS3/fermi-lite/lib/arm/neon/mul_n.h`

 * *Files identical despite different names*

### Comparing `MACS3-3.0.0b2/MACS3/fermi-lite/lib/arm/neon/mull.h` & `MACS3-3.0.0b3/MACS3/fermi-lite/lib/arm/neon/mull.h`

 * *Files identical despite different names*

### Comparing `MACS3-3.0.0b2/MACS3/fermi-lite/lib/arm/neon/mull_high.h` & `MACS3-3.0.0b3/MACS3/fermi-lite/lib/arm/neon/mull_high.h`

 * *Files identical despite different names*

### Comparing `MACS3-3.0.0b2/MACS3/fermi-lite/lib/arm/neon/mull_n.h` & `MACS3-3.0.0b3/MACS3/fermi-lite/lib/arm/neon/mull_n.h`

 * *Files identical despite different names*

### Comparing `MACS3-3.0.0b2/MACS3/fermi-lite/lib/arm/neon/mvn.h` & `MACS3-3.0.0b3/MACS3/fermi-lite/lib/arm/neon/mvn.h`

 * *Files identical despite different names*

### Comparing `MACS3-3.0.0b2/MACS3/fermi-lite/lib/arm/neon/neg.h` & `MACS3-3.0.0b3/MACS3/fermi-lite/lib/arm/neon/neg.h`

 * *Files identical despite different names*

### Comparing `MACS3-3.0.0b2/MACS3/fermi-lite/lib/arm/neon/orn.h` & `MACS3-3.0.0b3/MACS3/fermi-lite/lib/arm/neon/orn.h`

 * *Files identical despite different names*

### Comparing `MACS3-3.0.0b2/MACS3/fermi-lite/lib/arm/neon/orr.h` & `MACS3-3.0.0b3/MACS3/fermi-lite/lib/arm/neon/orr.h`

 * *Files identical despite different names*

### Comparing `MACS3-3.0.0b2/MACS3/fermi-lite/lib/arm/neon/padal.h` & `MACS3-3.0.0b3/MACS3/fermi-lite/lib/arm/neon/padal.h`

 * *Files identical despite different names*

### Comparing `MACS3-3.0.0b2/MACS3/fermi-lite/lib/arm/neon/padd.h` & `MACS3-3.0.0b3/MACS3/fermi-lite/lib/arm/neon/padd.h`

 * *Files identical despite different names*

### Comparing `MACS3-3.0.0b2/MACS3/fermi-lite/lib/arm/neon/paddl.h` & `MACS3-3.0.0b3/MACS3/fermi-lite/lib/arm/neon/paddl.h`

 * *Files identical despite different names*

### Comparing `MACS3-3.0.0b2/MACS3/fermi-lite/lib/arm/neon/pmax.h` & `MACS3-3.0.0b3/MACS3/fermi-lite/lib/arm/neon/pmax.h`

 * *Files identical despite different names*

### Comparing `MACS3-3.0.0b2/MACS3/fermi-lite/lib/arm/neon/pmin.h` & `MACS3-3.0.0b3/MACS3/fermi-lite/lib/arm/neon/pmin.h`

 * *Files identical despite different names*

### Comparing `MACS3-3.0.0b2/MACS3/fermi-lite/lib/arm/neon/qabs.h` & `MACS3-3.0.0b3/MACS3/fermi-lite/lib/arm/neon/qabs.h`

 * *Files identical despite different names*

### Comparing `MACS3-3.0.0b2/MACS3/fermi-lite/lib/arm/neon/qadd.h` & `MACS3-3.0.0b3/MACS3/fermi-lite/lib/arm/neon/qadd.h`

 * *Files identical despite different names*

### Comparing `MACS3-3.0.0b2/MACS3/fermi-lite/lib/arm/neon/qdmulh.h` & `MACS3-3.0.0b3/MACS3/fermi-lite/lib/arm/neon/qdmulh.h`

 * *Files identical despite different names*

### Comparing `MACS3-3.0.0b2/MACS3/fermi-lite/lib/arm/neon/qdmull.h` & `MACS3-3.0.0b3/MACS3/fermi-lite/lib/arm/neon/qdmull.h`

 * *Files identical despite different names*

### Comparing `MACS3-3.0.0b2/MACS3/fermi-lite/lib/arm/neon/qmovn.h` & `MACS3-3.0.0b3/MACS3/fermi-lite/lib/arm/neon/qmovn.h`

 * *Files identical despite different names*

### Comparing `MACS3-3.0.0b2/MACS3/fermi-lite/lib/arm/neon/qmovn_high.h` & `MACS3-3.0.0b3/MACS3/fermi-lite/lib/arm/neon/qmovn_high.h`

 * *Files identical despite different names*

### Comparing `MACS3-3.0.0b2/MACS3/fermi-lite/lib/arm/neon/qmovun.h` & `MACS3-3.0.0b3/MACS3/fermi-lite/lib/arm/neon/qmovun.h`

 * *Files identical despite different names*

### Comparing `MACS3-3.0.0b2/MACS3/fermi-lite/lib/arm/neon/qneg.h` & `MACS3-3.0.0b3/MACS3/fermi-lite/lib/arm/neon/qneg.h`

 * *Files identical despite different names*

### Comparing `MACS3-3.0.0b2/MACS3/fermi-lite/lib/arm/neon/qrdmulh.h` & `MACS3-3.0.0b3/MACS3/fermi-lite/lib/arm/neon/qrdmulh.h`

 * *Files identical despite different names*

### Comparing `MACS3-3.0.0b2/MACS3/fermi-lite/lib/arm/neon/qrdmulh_n.h` & `MACS3-3.0.0b3/MACS3/fermi-lite/lib/arm/neon/qrdmulh_n.h`

 * *Files identical despite different names*

### Comparing `MACS3-3.0.0b2/MACS3/fermi-lite/lib/arm/neon/qshl.h` & `MACS3-3.0.0b3/MACS3/fermi-lite/lib/arm/neon/qshl.h`

 * *Files identical despite different names*

### Comparing `MACS3-3.0.0b2/MACS3/fermi-lite/lib/arm/neon/qsub.h` & `MACS3-3.0.0b3/MACS3/fermi-lite/lib/arm/neon/qsub.h`

 * *Files identical despite different names*

### Comparing `MACS3-3.0.0b2/MACS3/fermi-lite/lib/arm/neon/qtbl.h` & `MACS3-3.0.0b3/MACS3/fermi-lite/lib/arm/neon/qtbl.h`

 * *Files identical despite different names*

### Comparing `MACS3-3.0.0b2/MACS3/fermi-lite/lib/arm/neon/qtbx.h` & `MACS3-3.0.0b3/MACS3/fermi-lite/lib/arm/neon/qtbx.h`

 * *Files identical despite different names*

### Comparing `MACS3-3.0.0b2/MACS3/fermi-lite/lib/arm/neon/rbit.h` & `MACS3-3.0.0b3/MACS3/fermi-lite/lib/arm/neon/rbit.h`

 * *Files identical despite different names*

### Comparing `MACS3-3.0.0b2/MACS3/fermi-lite/lib/arm/neon/reinterpret.h` & `MACS3-3.0.0b3/MACS3/fermi-lite/lib/arm/neon/reinterpret.h`

 * *Files identical despite different names*

### Comparing `MACS3-3.0.0b2/MACS3/fermi-lite/lib/arm/neon/rev16.h` & `MACS3-3.0.0b3/MACS3/fermi-lite/lib/arm/neon/rev16.h`

 * *Files identical despite different names*

### Comparing `MACS3-3.0.0b2/MACS3/fermi-lite/lib/arm/neon/rev32.h` & `MACS3-3.0.0b3/MACS3/fermi-lite/lib/arm/neon/rev32.h`

 * *Files identical despite different names*

### Comparing `MACS3-3.0.0b2/MACS3/fermi-lite/lib/arm/neon/rev64.h` & `MACS3-3.0.0b3/MACS3/fermi-lite/lib/arm/neon/rev64.h`

 * *Files identical despite different names*

### Comparing `MACS3-3.0.0b2/MACS3/fermi-lite/lib/arm/neon/rhadd.h` & `MACS3-3.0.0b3/MACS3/fermi-lite/lib/arm/neon/rhadd.h`

 * *Files identical despite different names*

### Comparing `MACS3-3.0.0b2/MACS3/fermi-lite/lib/arm/neon/rnd.h` & `MACS3-3.0.0b3/MACS3/fermi-lite/lib/arm/neon/rnd.h`

 * *Files identical despite different names*

### Comparing `MACS3-3.0.0b2/MACS3/fermi-lite/lib/arm/neon/rshl.h` & `MACS3-3.0.0b3/MACS3/fermi-lite/lib/arm/neon/rshl.h`

 * *Files identical despite different names*

### Comparing `MACS3-3.0.0b2/MACS3/fermi-lite/lib/arm/neon/rshr_n.h` & `MACS3-3.0.0b3/MACS3/fermi-lite/lib/arm/neon/rshr_n.h`

 * *Files identical despite different names*

### Comparing `MACS3-3.0.0b2/MACS3/fermi-lite/lib/arm/neon/rsra_n.h` & `MACS3-3.0.0b3/MACS3/fermi-lite/lib/arm/neon/rsra_n.h`

 * *Files identical despite different names*

### Comparing `MACS3-3.0.0b2/MACS3/fermi-lite/lib/arm/neon/set_lane.h` & `MACS3-3.0.0b3/MACS3/fermi-lite/lib/arm/neon/set_lane.h`

 * *Files identical despite different names*

### Comparing `MACS3-3.0.0b2/MACS3/fermi-lite/lib/arm/neon/shl.h` & `MACS3-3.0.0b3/MACS3/fermi-lite/lib/arm/neon/shl.h`

 * *Files identical despite different names*

### Comparing `MACS3-3.0.0b2/MACS3/fermi-lite/lib/arm/neon/shl_n.h` & `MACS3-3.0.0b3/MACS3/fermi-lite/lib/arm/neon/shl_n.h`

 * *Files identical despite different names*

### Comparing `MACS3-3.0.0b2/MACS3/fermi-lite/lib/arm/neon/shr_n.h` & `MACS3-3.0.0b3/MACS3/fermi-lite/lib/arm/neon/shr_n.h`

 * *Files identical despite different names*

### Comparing `MACS3-3.0.0b2/MACS3/fermi-lite/lib/arm/neon/sra_n.h` & `MACS3-3.0.0b3/MACS3/fermi-lite/lib/arm/neon/sra_n.h`

 * *Files identical despite different names*

### Comparing `MACS3-3.0.0b2/MACS3/fermi-lite/lib/arm/neon/st1.h` & `MACS3-3.0.0b3/MACS3/fermi-lite/lib/arm/neon/st1.h`

 * *Files identical despite different names*

### Comparing `MACS3-3.0.0b2/MACS3/fermi-lite/lib/arm/neon/st1_lane.h` & `MACS3-3.0.0b3/MACS3/fermi-lite/lib/arm/neon/st1_lane.h`

 * *Files identical despite different names*

### Comparing `MACS3-3.0.0b2/MACS3/fermi-lite/lib/arm/neon/st3.h` & `MACS3-3.0.0b3/MACS3/fermi-lite/lib/arm/neon/st3.h`

 * *Files identical despite different names*

### Comparing `MACS3-3.0.0b2/MACS3/fermi-lite/lib/arm/neon/st4.h` & `MACS3-3.0.0b3/MACS3/fermi-lite/lib/arm/neon/st4.h`

 * *Files identical despite different names*

### Comparing `MACS3-3.0.0b2/MACS3/fermi-lite/lib/arm/neon/sub.h` & `MACS3-3.0.0b3/MACS3/fermi-lite/lib/arm/neon/sub.h`

 * *Files identical despite different names*

### Comparing `MACS3-3.0.0b2/MACS3/fermi-lite/lib/arm/neon/subl.h` & `MACS3-3.0.0b3/MACS3/fermi-lite/lib/arm/neon/subl.h`

 * *Files identical despite different names*

### Comparing `MACS3-3.0.0b2/MACS3/fermi-lite/lib/arm/neon/subw.h` & `MACS3-3.0.0b3/MACS3/fermi-lite/lib/arm/neon/subw.h`

 * *Files identical despite different names*

### Comparing `MACS3-3.0.0b2/MACS3/fermi-lite/lib/arm/neon/subw_high.h` & `MACS3-3.0.0b3/MACS3/fermi-lite/lib/arm/neon/subw_high.h`

 * *Files identical despite different names*

### Comparing `MACS3-3.0.0b2/MACS3/fermi-lite/lib/arm/neon/tbl.h` & `MACS3-3.0.0b3/MACS3/fermi-lite/lib/arm/neon/tbl.h`

 * *Files identical despite different names*

### Comparing `MACS3-3.0.0b2/MACS3/fermi-lite/lib/arm/neon/tbx.h` & `MACS3-3.0.0b3/MACS3/fermi-lite/lib/arm/neon/tbx.h`

 * *Files identical despite different names*

### Comparing `MACS3-3.0.0b2/MACS3/fermi-lite/lib/arm/neon/trn.h` & `MACS3-3.0.0b3/MACS3/fermi-lite/lib/arm/neon/trn.h`

 * *Files identical despite different names*

### Comparing `MACS3-3.0.0b2/MACS3/fermi-lite/lib/arm/neon/trn1.h` & `MACS3-3.0.0b3/MACS3/fermi-lite/lib/arm/neon/trn1.h`

 * *Files identical despite different names*

### Comparing `MACS3-3.0.0b2/MACS3/fermi-lite/lib/arm/neon/trn2.h` & `MACS3-3.0.0b3/MACS3/fermi-lite/lib/arm/neon/trn2.h`

 * *Files identical despite different names*

### Comparing `MACS3-3.0.0b2/MACS3/fermi-lite/lib/arm/neon/tst.h` & `MACS3-3.0.0b3/MACS3/fermi-lite/lib/arm/neon/tst.h`

 * *Files identical despite different names*

### Comparing `MACS3-3.0.0b2/MACS3/fermi-lite/lib/arm/neon/types.h` & `MACS3-3.0.0b3/MACS3/fermi-lite/lib/arm/neon/types.h`

 * *Files identical despite different names*

### Comparing `MACS3-3.0.0b2/MACS3/fermi-lite/lib/arm/neon/uqadd.h` & `MACS3-3.0.0b3/MACS3/fermi-lite/lib/arm/neon/uqadd.h`

 * *Files identical despite different names*

### Comparing `MACS3-3.0.0b2/MACS3/fermi-lite/lib/arm/neon/uzp.h` & `MACS3-3.0.0b3/MACS3/fermi-lite/lib/arm/neon/uzp.h`

 * *Files identical despite different names*

### Comparing `MACS3-3.0.0b2/MACS3/fermi-lite/lib/arm/neon/uzp1.h` & `MACS3-3.0.0b3/MACS3/fermi-lite/lib/arm/neon/uzp1.h`

 * *Files identical despite different names*

### Comparing `MACS3-3.0.0b2/MACS3/fermi-lite/lib/arm/neon/uzp2.h` & `MACS3-3.0.0b3/MACS3/fermi-lite/lib/arm/neon/uzp2.h`

 * *Files identical despite different names*

### Comparing `MACS3-3.0.0b2/MACS3/fermi-lite/lib/arm/neon/zip.h` & `MACS3-3.0.0b3/MACS3/fermi-lite/lib/arm/neon/zip.h`

 * *Files identical despite different names*

### Comparing `MACS3-3.0.0b2/MACS3/fermi-lite/lib/arm/neon/zip1.h` & `MACS3-3.0.0b3/MACS3/fermi-lite/lib/arm/neon/zip1.h`

 * *Files identical despite different names*

### Comparing `MACS3-3.0.0b2/MACS3/fermi-lite/lib/arm/neon/zip2.h` & `MACS3-3.0.0b3/MACS3/fermi-lite/lib/arm/neon/zip2.h`

 * *Files identical despite different names*

### Comparing `MACS3-3.0.0b2/MACS3/fermi-lite/lib/arm/neon.h` & `MACS3-3.0.0b3/MACS3/fermi-lite/lib/arm/neon.h`

 * *Files identical despite different names*

### Comparing `MACS3-3.0.0b2/MACS3/fermi-lite/lib/check.h` & `MACS3-3.0.0b3/MACS3/fermi-lite/lib/check.h`

 * *Files identical despite different names*

### Comparing `MACS3-3.0.0b2/MACS3/fermi-lite/lib/debug-trap.h` & `MACS3-3.0.0b3/MACS3/fermi-lite/lib/debug-trap.h`

 * *Files identical despite different names*

### Comparing `MACS3-3.0.0b2/MACS3/fermi-lite/lib/hedley.h` & `MACS3-3.0.0b3/MACS3/fermi-lite/lib/hedley.h`

 * *Files identical despite different names*

### Comparing `MACS3-3.0.0b2/MACS3/fermi-lite/lib/simde-align.h` & `MACS3-3.0.0b3/MACS3/fermi-lite/lib/simde-align.h`

 * *Files identical despite different names*

### Comparing `MACS3-3.0.0b2/MACS3/fermi-lite/lib/simde-arch.h` & `MACS3-3.0.0b3/MACS3/fermi-lite/lib/simde-arch.h`

 * *Files identical despite different names*

### Comparing `MACS3-3.0.0b2/MACS3/fermi-lite/lib/simde-common.h` & `MACS3-3.0.0b3/MACS3/fermi-lite/lib/simde-common.h`

 * *Files identical despite different names*

### Comparing `MACS3-3.0.0b2/MACS3/fermi-lite/lib/simde-constify.h` & `MACS3-3.0.0b3/MACS3/fermi-lite/lib/simde-constify.h`

 * *Files identical despite different names*

### Comparing `MACS3-3.0.0b2/MACS3/fermi-lite/lib/simde-detect-clang.h` & `MACS3-3.0.0b3/MACS3/fermi-lite/lib/simde-detect-clang.h`

 * *Files identical despite different names*

### Comparing `MACS3-3.0.0b2/MACS3/fermi-lite/lib/simde-diagnostic.h` & `MACS3-3.0.0b3/MACS3/fermi-lite/lib/simde-diagnostic.h`

 * *Files identical despite different names*

### Comparing `MACS3-3.0.0b2/MACS3/fermi-lite/lib/simde-features.h` & `MACS3-3.0.0b3/MACS3/fermi-lite/lib/simde-features.h`

 * *Files identical despite different names*

### Comparing `MACS3-3.0.0b2/MACS3/fermi-lite/lib/simde-math.h` & `MACS3-3.0.0b3/MACS3/fermi-lite/lib/simde-math.h`

 * *Files identical despite different names*

### Comparing `MACS3-3.0.0b2/MACS3/fermi-lite/lib/x86/avx.h` & `MACS3-3.0.0b3/MACS3/fermi-lite/lib/x86/avx.h`

 * *Files identical despite different names*

### Comparing `MACS3-3.0.0b2/MACS3/fermi-lite/lib/x86/avx2.h` & `MACS3-3.0.0b3/MACS3/fermi-lite/lib/x86/avx2.h`

 * *Files identical despite different names*

### Comparing `MACS3-3.0.0b2/MACS3/fermi-lite/lib/x86/avx512/2intersect.h` & `MACS3-3.0.0b3/MACS3/fermi-lite/lib/x86/avx512/2intersect.h`

 * *Files identical despite different names*

### Comparing `MACS3-3.0.0b2/MACS3/fermi-lite/lib/x86/avx512/abs.h` & `MACS3-3.0.0b3/MACS3/fermi-lite/lib/x86/avx512/abs.h`

 * *Files identical despite different names*

### Comparing `MACS3-3.0.0b2/MACS3/fermi-lite/lib/x86/avx512/add.h` & `MACS3-3.0.0b3/MACS3/fermi-lite/lib/x86/avx512/add.h`

 * *Files identical despite different names*

### Comparing `MACS3-3.0.0b2/MACS3/fermi-lite/lib/x86/avx512/adds.h` & `MACS3-3.0.0b3/MACS3/fermi-lite/lib/x86/avx512/adds.h`

 * *Files identical despite different names*

### Comparing `MACS3-3.0.0b2/MACS3/fermi-lite/lib/x86/avx512/and.h` & `MACS3-3.0.0b3/MACS3/fermi-lite/lib/x86/avx512/and.h`

 * *Files identical despite different names*

### Comparing `MACS3-3.0.0b2/MACS3/fermi-lite/lib/x86/avx512/andnot.h` & `MACS3-3.0.0b3/MACS3/fermi-lite/lib/x86/avx512/andnot.h`

 * *Files identical despite different names*

### Comparing `MACS3-3.0.0b2/MACS3/fermi-lite/lib/x86/avx512/avg.h` & `MACS3-3.0.0b3/MACS3/fermi-lite/lib/x86/avx512/avg.h`

 * *Files identical despite different names*

### Comparing `MACS3-3.0.0b2/MACS3/fermi-lite/lib/x86/avx512/blend.h` & `MACS3-3.0.0b3/MACS3/fermi-lite/lib/x86/avx512/blend.h`

 * *Files identical despite different names*

### Comparing `MACS3-3.0.0b2/MACS3/fermi-lite/lib/x86/avx512/broadcast.h` & `MACS3-3.0.0b3/MACS3/fermi-lite/lib/x86/avx512/broadcast.h`

 * *Files identical despite different names*

### Comparing `MACS3-3.0.0b2/MACS3/fermi-lite/lib/x86/avx512/cast.h` & `MACS3-3.0.0b3/MACS3/fermi-lite/lib/x86/avx512/cast.h`

 * *Files identical despite different names*

### Comparing `MACS3-3.0.0b2/MACS3/fermi-lite/lib/x86/avx512/cmp.h` & `MACS3-3.0.0b3/MACS3/fermi-lite/lib/x86/avx512/cmp.h`

 * *Files identical despite different names*

### Comparing `MACS3-3.0.0b2/MACS3/fermi-lite/lib/x86/avx512/cmpeq.h` & `MACS3-3.0.0b3/MACS3/fermi-lite/lib/x86/avx512/cmpeq.h`

 * *Files identical despite different names*

### Comparing `MACS3-3.0.0b2/MACS3/fermi-lite/lib/x86/avx512/cmpge.h` & `MACS3-3.0.0b3/MACS3/fermi-lite/lib/x86/avx512/cmpge.h`

 * *Files identical despite different names*

### Comparing `MACS3-3.0.0b2/MACS3/fermi-lite/lib/x86/avx512/cmpgt.h` & `MACS3-3.0.0b3/MACS3/fermi-lite/lib/x86/avx512/cmpgt.h`

 * *Files identical despite different names*

### Comparing `MACS3-3.0.0b2/MACS3/fermi-lite/lib/x86/avx512/cmple.h` & `MACS3-3.0.0b3/MACS3/fermi-lite/lib/x86/avx512/cmple.h`

 * *Files identical despite different names*

### Comparing `MACS3-3.0.0b2/MACS3/fermi-lite/lib/x86/avx512/cmplt.h` & `MACS3-3.0.0b3/MACS3/fermi-lite/lib/x86/avx512/cmplt.h`

 * *Files identical despite different names*

### Comparing `MACS3-3.0.0b2/MACS3/fermi-lite/lib/x86/avx512/copysign.h` & `MACS3-3.0.0b3/MACS3/fermi-lite/lib/x86/avx512/copysign.h`

 * *Files identical despite different names*

### Comparing `MACS3-3.0.0b2/MACS3/fermi-lite/lib/x86/avx512/cvt.h` & `MACS3-3.0.0b3/MACS3/fermi-lite/lib/x86/avx512/cvt.h`

 * *Files identical despite different names*

### Comparing `MACS3-3.0.0b2/MACS3/fermi-lite/lib/x86/avx512/cvts.h` & `MACS3-3.0.0b3/MACS3/fermi-lite/lib/x86/avx512/cvts.h`

 * *Files identical despite different names*

### Comparing `MACS3-3.0.0b2/MACS3/fermi-lite/lib/x86/avx512/div.h` & `MACS3-3.0.0b3/MACS3/fermi-lite/lib/x86/avx512/div.h`

 * *Files identical despite different names*

### Comparing `MACS3-3.0.0b2/MACS3/fermi-lite/lib/x86/avx512/extract.h` & `MACS3-3.0.0b3/MACS3/fermi-lite/lib/x86/avx512/extract.h`

 * *Files identical despite different names*

### Comparing `MACS3-3.0.0b2/MACS3/fermi-lite/lib/x86/avx512/fmadd.h` & `MACS3-3.0.0b3/MACS3/fermi-lite/lib/x86/avx512/fmadd.h`

 * *Files identical despite different names*

### Comparing `MACS3-3.0.0b2/MACS3/fermi-lite/lib/x86/avx512/fmsub.h` & `MACS3-3.0.0b3/MACS3/fermi-lite/lib/x86/avx512/fmsub.h`

 * *Files identical despite different names*

### Comparing `MACS3-3.0.0b2/MACS3/fermi-lite/lib/x86/avx512/fnmadd.h` & `MACS3-3.0.0b3/MACS3/fermi-lite/lib/x86/avx512/fnmadd.h`

 * *Files identical despite different names*

### Comparing `MACS3-3.0.0b2/MACS3/fermi-lite/lib/x86/avx512/fnmsub.h` & `MACS3-3.0.0b3/MACS3/fermi-lite/lib/x86/avx512/fnmsub.h`

 * *Files identical despite different names*

### Comparing `MACS3-3.0.0b2/MACS3/fermi-lite/lib/x86/avx512/insert.h` & `MACS3-3.0.0b3/MACS3/fermi-lite/lib/x86/avx512/insert.h`

 * *Files identical despite different names*

### Comparing `MACS3-3.0.0b2/MACS3/fermi-lite/lib/x86/avx512/kshift.h` & `MACS3-3.0.0b3/MACS3/fermi-lite/lib/x86/avx512/kshift.h`

 * *Files identical despite different names*

### Comparing `MACS3-3.0.0b2/MACS3/fermi-lite/lib/x86/avx512/load.h` & `MACS3-3.0.0b3/MACS3/fermi-lite/lib/x86/avx512/load.h`

 * *Files identical despite different names*

### Comparing `MACS3-3.0.0b2/MACS3/fermi-lite/lib/x86/avx512/loadu.h` & `MACS3-3.0.0b3/MACS3/fermi-lite/lib/x86/avx512/loadu.h`

 * *Files identical despite different names*

### Comparing `MACS3-3.0.0b2/MACS3/fermi-lite/lib/x86/avx512/lzcnt.h` & `MACS3-3.0.0b3/MACS3/fermi-lite/lib/x86/avx512/lzcnt.h`

 * *Files identical despite different names*

### Comparing `MACS3-3.0.0b2/MACS3/fermi-lite/lib/x86/avx512/madd.h` & `MACS3-3.0.0b3/MACS3/fermi-lite/lib/x86/avx512/madd.h`

 * *Files identical despite different names*

### Comparing `MACS3-3.0.0b2/MACS3/fermi-lite/lib/x86/avx512/maddubs.h` & `MACS3-3.0.0b3/MACS3/fermi-lite/lib/x86/avx512/maddubs.h`

 * *Files identical despite different names*

### Comparing `MACS3-3.0.0b2/MACS3/fermi-lite/lib/x86/avx512/max.h` & `MACS3-3.0.0b3/MACS3/fermi-lite/lib/x86/avx512/max.h`

 * *Files identical despite different names*

### Comparing `MACS3-3.0.0b2/MACS3/fermi-lite/lib/x86/avx512/min.h` & `MACS3-3.0.0b3/MACS3/fermi-lite/lib/x86/avx512/min.h`

 * *Files identical despite different names*

### Comparing `MACS3-3.0.0b2/MACS3/fermi-lite/lib/x86/avx512/mov.h` & `MACS3-3.0.0b3/MACS3/fermi-lite/lib/x86/avx512/mov.h`

 * *Files identical despite different names*

### Comparing `MACS3-3.0.0b2/MACS3/fermi-lite/lib/x86/avx512/mov_mask.h` & `MACS3-3.0.0b3/MACS3/fermi-lite/lib/x86/avx512/mov_mask.h`

 * *Files identical despite different names*

### Comparing `MACS3-3.0.0b2/MACS3/fermi-lite/lib/x86/avx512/movm.h` & `MACS3-3.0.0b3/MACS3/fermi-lite/lib/x86/avx512/movm.h`

 * *Files identical despite different names*

### Comparing `MACS3-3.0.0b2/MACS3/fermi-lite/lib/x86/avx512/mul.h` & `MACS3-3.0.0b3/MACS3/fermi-lite/lib/x86/avx512/mul.h`

 * *Files identical despite different names*

### Comparing `MACS3-3.0.0b2/MACS3/fermi-lite/lib/x86/avx512/mulhi.h` & `MACS3-3.0.0b3/MACS3/fermi-lite/lib/x86/avx512/mulhi.h`

 * *Files identical despite different names*

### Comparing `MACS3-3.0.0b2/MACS3/fermi-lite/lib/x86/avx512/mulhrs.h` & `MACS3-3.0.0b3/MACS3/fermi-lite/lib/x86/avx512/mulhrs.h`

 * *Files identical despite different names*

### Comparing `MACS3-3.0.0b2/MACS3/fermi-lite/lib/x86/avx512/mullo.h` & `MACS3-3.0.0b3/MACS3/fermi-lite/lib/x86/avx512/mullo.h`

 * *Files identical despite different names*

### Comparing `MACS3-3.0.0b2/MACS3/fermi-lite/lib/x86/avx512/negate.h` & `MACS3-3.0.0b3/MACS3/fermi-lite/lib/x86/avx512/negate.h`

 * *Files identical despite different names*

### Comparing `MACS3-3.0.0b2/MACS3/fermi-lite/lib/x86/avx512/or.h` & `MACS3-3.0.0b3/MACS3/fermi-lite/lib/x86/avx512/or.h`

 * *Files identical despite different names*

### Comparing `MACS3-3.0.0b2/MACS3/fermi-lite/lib/x86/avx512/packs.h` & `MACS3-3.0.0b3/MACS3/fermi-lite/lib/x86/avx512/packs.h`

 * *Files identical despite different names*

### Comparing `MACS3-3.0.0b2/MACS3/fermi-lite/lib/x86/avx512/packus.h` & `MACS3-3.0.0b3/MACS3/fermi-lite/lib/x86/avx512/packus.h`

 * *Files identical despite different names*

### Comparing `MACS3-3.0.0b2/MACS3/fermi-lite/lib/x86/avx512/permutex2var.h` & `MACS3-3.0.0b3/MACS3/fermi-lite/lib/x86/avx512/permutex2var.h`

 * *Files identical despite different names*

### Comparing `MACS3-3.0.0b2/MACS3/fermi-lite/lib/x86/avx512/permutexvar.h` & `MACS3-3.0.0b3/MACS3/fermi-lite/lib/x86/avx512/permutexvar.h`

 * *Files identical despite different names*

### Comparing `MACS3-3.0.0b2/MACS3/fermi-lite/lib/x86/avx512/sad.h` & `MACS3-3.0.0b3/MACS3/fermi-lite/lib/x86/avx512/sad.h`

 * *Files identical despite different names*

### Comparing `MACS3-3.0.0b2/MACS3/fermi-lite/lib/x86/avx512/set.h` & `MACS3-3.0.0b3/MACS3/fermi-lite/lib/x86/avx512/set.h`

 * *Files identical despite different names*

### Comparing `MACS3-3.0.0b2/MACS3/fermi-lite/lib/x86/avx512/set1.h` & `MACS3-3.0.0b3/MACS3/fermi-lite/lib/x86/avx512/set1.h`

 * *Files identical despite different names*

### Comparing `MACS3-3.0.0b2/MACS3/fermi-lite/lib/x86/avx512/set4.h` & `MACS3-3.0.0b3/MACS3/fermi-lite/lib/x86/avx512/set4.h`

 * *Files identical despite different names*

### Comparing `MACS3-3.0.0b2/MACS3/fermi-lite/lib/x86/avx512/setone.h` & `MACS3-3.0.0b3/MACS3/fermi-lite/lib/x86/avx512/setone.h`

 * *Files identical despite different names*

### Comparing `MACS3-3.0.0b2/MACS3/fermi-lite/lib/x86/avx512/setr.h` & `MACS3-3.0.0b3/MACS3/fermi-lite/lib/x86/avx512/setr.h`

 * *Files identical despite different names*

### Comparing `MACS3-3.0.0b2/MACS3/fermi-lite/lib/x86/avx512/setr4.h` & `MACS3-3.0.0b3/MACS3/fermi-lite/lib/x86/avx512/setr4.h`

 * *Files identical despite different names*

### Comparing `MACS3-3.0.0b2/MACS3/fermi-lite/lib/x86/avx512/setzero.h` & `MACS3-3.0.0b3/MACS3/fermi-lite/lib/x86/avx512/setzero.h`

 * *Files identical despite different names*

### Comparing `MACS3-3.0.0b2/MACS3/fermi-lite/lib/x86/avx512/shuffle.h` & `MACS3-3.0.0b3/MACS3/fermi-lite/lib/x86/avx512/shuffle.h`

 * *Files identical despite different names*

### Comparing `MACS3-3.0.0b2/MACS3/fermi-lite/lib/x86/avx512/sll.h` & `MACS3-3.0.0b3/MACS3/fermi-lite/lib/x86/avx512/sll.h`

 * *Files identical despite different names*

### Comparing `MACS3-3.0.0b2/MACS3/fermi-lite/lib/x86/avx512/slli.h` & `MACS3-3.0.0b3/MACS3/fermi-lite/lib/x86/avx512/slli.h`

 * *Files identical despite different names*

### Comparing `MACS3-3.0.0b2/MACS3/fermi-lite/lib/x86/avx512/sllv.h` & `MACS3-3.0.0b3/MACS3/fermi-lite/lib/x86/avx512/sllv.h`

 * *Files identical despite different names*

### Comparing `MACS3-3.0.0b2/MACS3/fermi-lite/lib/x86/avx512/sqrt.h` & `MACS3-3.0.0b3/MACS3/fermi-lite/lib/x86/avx512/sqrt.h`

 * *Files identical despite different names*

### Comparing `MACS3-3.0.0b2/MACS3/fermi-lite/lib/x86/avx512/sra.h` & `MACS3-3.0.0b3/MACS3/fermi-lite/lib/x86/avx512/sra.h`

 * *Files identical despite different names*

### Comparing `MACS3-3.0.0b2/MACS3/fermi-lite/lib/x86/avx512/srai.h` & `MACS3-3.0.0b3/MACS3/fermi-lite/lib/x86/avx512/srai.h`

 * *Files identical despite different names*

### Comparing `MACS3-3.0.0b2/MACS3/fermi-lite/lib/x86/avx512/srav.h` & `MACS3-3.0.0b3/MACS3/fermi-lite/lib/x86/avx512/srav.h`

 * *Files identical despite different names*

### Comparing `MACS3-3.0.0b2/MACS3/fermi-lite/lib/x86/avx512/srl.h` & `MACS3-3.0.0b3/MACS3/fermi-lite/lib/x86/avx512/srl.h`

 * *Files identical despite different names*

### Comparing `MACS3-3.0.0b2/MACS3/fermi-lite/lib/x86/avx512/srli.h` & `MACS3-3.0.0b3/MACS3/fermi-lite/lib/x86/avx512/srli.h`

 * *Files identical despite different names*

### Comparing `MACS3-3.0.0b2/MACS3/fermi-lite/lib/x86/avx512/srlv.h` & `MACS3-3.0.0b3/MACS3/fermi-lite/lib/x86/avx512/srlv.h`

 * *Files identical despite different names*

### Comparing `MACS3-3.0.0b2/MACS3/fermi-lite/lib/x86/avx512/store.h` & `MACS3-3.0.0b3/MACS3/fermi-lite/lib/x86/avx512/store.h`

 * *Files identical despite different names*

### Comparing `MACS3-3.0.0b2/MACS3/fermi-lite/lib/x86/avx512/storeu.h` & `MACS3-3.0.0b3/MACS3/fermi-lite/lib/x86/avx512/storeu.h`

 * *Files identical despite different names*

### Comparing `MACS3-3.0.0b2/MACS3/fermi-lite/lib/x86/avx512/sub.h` & `MACS3-3.0.0b3/MACS3/fermi-lite/lib/x86/avx512/sub.h`

 * *Files identical despite different names*

### Comparing `MACS3-3.0.0b2/MACS3/fermi-lite/lib/x86/avx512/subs.h` & `MACS3-3.0.0b3/MACS3/fermi-lite/lib/x86/avx512/subs.h`

 * *Files identical despite different names*

### Comparing `MACS3-3.0.0b2/MACS3/fermi-lite/lib/x86/avx512/test.h` & `MACS3-3.0.0b3/MACS3/fermi-lite/lib/x86/avx512/test.h`

 * *Files identical despite different names*

### Comparing `MACS3-3.0.0b2/MACS3/fermi-lite/lib/x86/avx512/types.h` & `MACS3-3.0.0b3/MACS3/fermi-lite/lib/x86/avx512/types.h`

 * *Files identical despite different names*

### Comparing `MACS3-3.0.0b2/MACS3/fermi-lite/lib/x86/avx512/unpackhi.h` & `MACS3-3.0.0b3/MACS3/fermi-lite/lib/x86/avx512/unpackhi.h`

 * *Files identical despite different names*

### Comparing `MACS3-3.0.0b2/MACS3/fermi-lite/lib/x86/avx512/unpacklo.h` & `MACS3-3.0.0b3/MACS3/fermi-lite/lib/x86/avx512/unpacklo.h`

 * *Files identical despite different names*

### Comparing `MACS3-3.0.0b2/MACS3/fermi-lite/lib/x86/avx512/xor.h` & `MACS3-3.0.0b3/MACS3/fermi-lite/lib/x86/avx512/xor.h`

 * *Files identical despite different names*

### Comparing `MACS3-3.0.0b2/MACS3/fermi-lite/lib/x86/avx512/xorsign.h` & `MACS3-3.0.0b3/MACS3/fermi-lite/lib/x86/avx512/xorsign.h`

 * *Files identical despite different names*

### Comparing `MACS3-3.0.0b2/MACS3/fermi-lite/lib/x86/avx512.h` & `MACS3-3.0.0b3/MACS3/fermi-lite/lib/x86/avx512.h`

 * *Files identical despite different names*

### Comparing `MACS3-3.0.0b2/MACS3/fermi-lite/lib/x86/clmul.h` & `MACS3-3.0.0b3/MACS3/fermi-lite/lib/x86/clmul.h`

 * *Files identical despite different names*

### Comparing `MACS3-3.0.0b2/MACS3/fermi-lite/lib/x86/fma.h` & `MACS3-3.0.0b3/MACS3/fermi-lite/lib/x86/fma.h`

 * *Files identical despite different names*

### Comparing `MACS3-3.0.0b2/MACS3/fermi-lite/lib/x86/gfni.h` & `MACS3-3.0.0b3/MACS3/fermi-lite/lib/x86/gfni.h`

 * *Files identical despite different names*

### Comparing `MACS3-3.0.0b2/MACS3/fermi-lite/lib/x86/mmx.h` & `MACS3-3.0.0b3/MACS3/fermi-lite/lib/x86/mmx.h`

 * *Files identical despite different names*

### Comparing `MACS3-3.0.0b2/MACS3/fermi-lite/lib/x86/sse.h` & `MACS3-3.0.0b3/MACS3/fermi-lite/lib/x86/sse.h`

 * *Files identical despite different names*

### Comparing `MACS3-3.0.0b2/MACS3/fermi-lite/lib/x86/sse2.h` & `MACS3-3.0.0b3/MACS3/fermi-lite/lib/x86/sse2.h`

 * *Files identical despite different names*

### Comparing `MACS3-3.0.0b2/MACS3/fermi-lite/lib/x86/sse3.h` & `MACS3-3.0.0b3/MACS3/fermi-lite/lib/x86/sse3.h`

 * *Files identical despite different names*

### Comparing `MACS3-3.0.0b2/MACS3/fermi-lite/lib/x86/sse4.1.h` & `MACS3-3.0.0b3/MACS3/fermi-lite/lib/x86/sse4.1.h`

 * *Files identical despite different names*

### Comparing `MACS3-3.0.0b2/MACS3/fermi-lite/lib/x86/sse4.2.h` & `MACS3-3.0.0b3/MACS3/fermi-lite/lib/x86/sse4.2.h`

 * *Files identical despite different names*

### Comparing `MACS3-3.0.0b2/MACS3/fermi-lite/lib/x86/ssse3.h` & `MACS3-3.0.0b3/MACS3/fermi-lite/lib/x86/ssse3.h`

 * *Files identical despite different names*

### Comparing `MACS3-3.0.0b2/MACS3/fermi-lite/lib/x86/svml.h` & `MACS3-3.0.0b3/MACS3/fermi-lite/lib/x86/svml.h`

 * *Files identical despite different names*

### Comparing `MACS3-3.0.0b2/MACS3/fermi-lite/mag.c` & `MACS3-3.0.0b3/MACS3/fermi-lite/mag.c`

 * *Files identical despite different names*

### Comparing `MACS3-3.0.0b2/MACS3/fermi-lite/mag.h` & `MACS3-3.0.0b3/MACS3/fermi-lite/mag.h`

 * *Files identical despite different names*

### Comparing `MACS3-3.0.0b2/MACS3/fermi-lite/misc.c` & `MACS3-3.0.0b3/MACS3/fermi-lite/misc.c`

 * *Files identical despite different names*

### Comparing `MACS3-3.0.0b2/MACS3/fermi-lite/mrope.c` & `MACS3-3.0.0b3/MACS3/fermi-lite/mrope.c`

 * *Files identical despite different names*

### Comparing `MACS3-3.0.0b2/MACS3/fermi-lite/mrope.h` & `MACS3-3.0.0b3/MACS3/fermi-lite/mrope.h`

 * *Files identical despite different names*

### Comparing `MACS3-3.0.0b2/MACS3/fermi-lite/rld0.c` & `MACS3-3.0.0b3/MACS3/fermi-lite/rld0.c`

 * *Files identical despite different names*

### Comparing `MACS3-3.0.0b2/MACS3/fermi-lite/rld0.h` & `MACS3-3.0.0b3/MACS3/fermi-lite/rld0.h`

 * *Files identical despite different names*

### Comparing `MACS3-3.0.0b2/MACS3/fermi-lite/rle.c` & `MACS3-3.0.0b3/MACS3/fermi-lite/rle.c`

 * *Files identical despite different names*

### Comparing `MACS3-3.0.0b2/MACS3/fermi-lite/rle.h` & `MACS3-3.0.0b3/MACS3/fermi-lite/rle.h`

 * *Files identical despite different names*

### Comparing `MACS3-3.0.0b2/MACS3/fermi-lite/rope.c` & `MACS3-3.0.0b3/MACS3/fermi-lite/rope.c`

 * *Files identical despite different names*

### Comparing `MACS3-3.0.0b2/MACS3/fermi-lite/rope.h` & `MACS3-3.0.0b3/MACS3/fermi-lite/rope.h`

 * *Files identical despite different names*

### Comparing `MACS3-3.0.0b2/MACS3/fermi-lite/unitig.c` & `MACS3-3.0.0b3/MACS3/fermi-lite/unitig.c`

 * *Files identical despite different names*

### Comparing `MACS3-3.0.0b2/MACS3.egg-info/PKG-INFO` & `MACS3-3.0.0b3/MACS3.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: MACS3
-Version: 3.0.0b2
+Version: 3.0.0b3
 Summary: Model Based Analysis for ChIP-Seq data
 Home-page: http://github.com/macs3-project/MACS/
 Author: Tao Liu
 Author-email: vladimir.liu@gmail.com
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
@@ -20,15 +20,15 @@
 Classifier: Programming Language :: Cython
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # MACS: Model-based Analysis for ChIP-Seq
 
-![Status](https://img.shields.io/pypi/status/macs3.svg) ![License](https://img.shields.io/github/license/macs3-project/MACS) ![Programming languages](https://img.shields.io/github/languages/top/macs3-project/MACS) ![CI x64](https://github.com/macs3-project/MACS/workflows/CI%20x64/badge.svg) ![CI non x64](https://github.com/macs3-project/MACS/workflows/CI%20non%20x64,%20python%203.7/badge.svg)
+![Status](https://img.shields.io/pypi/status/macs3.svg) ![License](https://img.shields.io/github/license/macs3-project/MACS) ![Programming languages](https://img.shields.io/github/languages/top/macs3-project/MACS) ![CI x64](https://github.com/macs3-project/MACS/workflows/CI%20x64/badge.svg) ![CI non x64](https://github.com/macs3-project/MACS/workflows/CI%20non%20x64,%20python%203.7/badge.svg) ![CI MacOS 12](https://github.com/macs3-project/MACS/workflows/CI%20MacOS%2012/badge.svg)
 
 [![PyPI download](https://img.shields.io/pypi/dm/macs3?label=pypi%20downloads)](https://pypistats.org/packages/macs3) [![Bioconda download](https://img.shields.io/conda/dn/bioconda/macs3?label=bioconda%20downloads)](https://anaconda.org/bioconda/macs3)
 
 Latest Release:
 * Github: [![Github Release](https://img.shields.io/github/v/release/macs3-project/MACS)](https://github.com/macs3-project/MACS/releases)
 * PyPI: [![PyPI Release](https://img.shields.io/pypi/v/macs3.svg) ![PyPI Python Version](https://img.shields.io/pypi/pyversions/MACS3) ![PyPI Format](https://img.shields.io/pypi/format/macs3)](https://pypi.org/project/macs3/)
 * Bioconda: [![Bioconda Release](https://img.shields.io/conda/v/bioconda/macs3) ![Bioconda Platform](https://img.shields.io/conda/pn/bioconda/macs3)](https://anaconda.org/bioconda/macs3)
@@ -54,30 +54,37 @@
 
 **Please note that current MACS3 is still in beta stage. However, we
 utilize Github Action to implement the CI (Continous Integration) to
 make sure that the main branch passes unit testing on certain
 functions and subcommands to reproduce the correct outputs. We will
 add more new features in the future.**
 
-## Recent Changes for MACS (3.0.0b2)
+## Recent Changes for MACS (3.0.0b3)
 
-### 3.0.0b2
-    The second beta version of MACS3, with HMMRATAC feature refined.
+### 3.0.0b3
+    The third beta version of MACS3, addressing Cython issue and with
+    two HMMRATAC options added.
 	   
-	* New features from beta1:
+	* New features from beta2:
 
-	1) HMMRATAC module fixes
+	1) HMMRATAC module
     
-       Cutoff analysis function added
-       Description regarding it has been added
-    
-    2) Memory monitoring in the runtime message
-    
-    3) testing for s390x, armv7 and power64le is back. However, we turned off the function to check if the `hmmratac` results from non-x86 architectures are the same as the standard results, because in order to let the testing run, we need to use old python libraries (scipy and sklearn) through the distribution of Debian/Linux bullseye.
+       --modelonly option: only generate HMM model and quit
+       
+       -t or --training: customized training regions can be provided
+	   through this option.
+	   
+	   --min-frag-p: exclude fragments with abnormal fragment length while generating four
+       signal tracks. #577 Check `macs3 hmmratac -h`.
     
+    2) testing for Mac OS12 is added. 
+
+	3) We require Cython 0.29.*. The new Cython3 will break our
+	codes. We will adopt Cython3 later. #574
+
 ## Install
 
 The common way to install MACS is through
 [PYPI](https://pypi.org/project/macs3/)) or
 [conda](https://anaconda.org/bioconda/macs3). Please check the
 [INSTALL](./docs/INSTALL.md) document for detail.
 
@@ -85,14 +92,20 @@
 architectures:
 
  * x86_64
  * aarch64
  * armv7
  * ppc64le
  * s390x 
+ * Apple chips
+
+In general, you can install through PyPI as `pip install macs3`. 
+To use virtual environment is highly recommended. Or you can install
+after unzipping the released package downloaded from Github, then
+use `pip install .` command.
 
 ## Usage
 
 Example for regular peak calling on TF ChIP-seq:
 
 `macs3 callpeak -t ChIP.bam -c Control.bam -f BAM -g hs -n test -B -q 0.01`
```

### Comparing `MACS3-3.0.0b2/MACS3.egg-info/SOURCES.txt` & `MACS3-3.0.0b3/MACS3.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -330,17 +330,18 @@
 docs/INSTALL.md
 docs/bdgbroadcall.md
 docs/bdgcmp.md
 docs/bdgdiff.md
 docs/bdgopt.md
 docs/bdgpeakcall.md
 docs/callpeak.md
+docs/callvar.md
+docs/cmbreps.md
 docs/filterdup.md
 docs/hmmratac.md
-docs/main.md
 docs/pileup.md
 docs/predictd.md
 docs/qa.md
 docs/randsample.md
 docs/refinepeak.md
 docs/testing_in_docker.md
 docs/tutorial.md
```

### Comparing `MACS3-3.0.0b2/PKG-INFO` & `MACS3-3.0.0b3/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: MACS3
-Version: 3.0.0b2
+Version: 3.0.0b3
 Summary: Model Based Analysis for ChIP-Seq data
 Home-page: http://github.com/macs3-project/MACS/
 Author: Tao Liu
 Author-email: vladimir.liu@gmail.com
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
@@ -20,15 +20,15 @@
 Classifier: Programming Language :: Cython
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # MACS: Model-based Analysis for ChIP-Seq
 
-![Status](https://img.shields.io/pypi/status/macs3.svg) ![License](https://img.shields.io/github/license/macs3-project/MACS) ![Programming languages](https://img.shields.io/github/languages/top/macs3-project/MACS) ![CI x64](https://github.com/macs3-project/MACS/workflows/CI%20x64/badge.svg) ![CI non x64](https://github.com/macs3-project/MACS/workflows/CI%20non%20x64,%20python%203.7/badge.svg)
+![Status](https://img.shields.io/pypi/status/macs3.svg) ![License](https://img.shields.io/github/license/macs3-project/MACS) ![Programming languages](https://img.shields.io/github/languages/top/macs3-project/MACS) ![CI x64](https://github.com/macs3-project/MACS/workflows/CI%20x64/badge.svg) ![CI non x64](https://github.com/macs3-project/MACS/workflows/CI%20non%20x64,%20python%203.7/badge.svg) ![CI MacOS 12](https://github.com/macs3-project/MACS/workflows/CI%20MacOS%2012/badge.svg)
 
 [![PyPI download](https://img.shields.io/pypi/dm/macs3?label=pypi%20downloads)](https://pypistats.org/packages/macs3) [![Bioconda download](https://img.shields.io/conda/dn/bioconda/macs3?label=bioconda%20downloads)](https://anaconda.org/bioconda/macs3)
 
 Latest Release:
 * Github: [![Github Release](https://img.shields.io/github/v/release/macs3-project/MACS)](https://github.com/macs3-project/MACS/releases)
 * PyPI: [![PyPI Release](https://img.shields.io/pypi/v/macs3.svg) ![PyPI Python Version](https://img.shields.io/pypi/pyversions/MACS3) ![PyPI Format](https://img.shields.io/pypi/format/macs3)](https://pypi.org/project/macs3/)
 * Bioconda: [![Bioconda Release](https://img.shields.io/conda/v/bioconda/macs3) ![Bioconda Platform](https://img.shields.io/conda/pn/bioconda/macs3)](https://anaconda.org/bioconda/macs3)
@@ -54,30 +54,37 @@
 
 **Please note that current MACS3 is still in beta stage. However, we
 utilize Github Action to implement the CI (Continous Integration) to
 make sure that the main branch passes unit testing on certain
 functions and subcommands to reproduce the correct outputs. We will
 add more new features in the future.**
 
-## Recent Changes for MACS (3.0.0b2)
+## Recent Changes for MACS (3.0.0b3)
 
-### 3.0.0b2
-    The second beta version of MACS3, with HMMRATAC feature refined.
+### 3.0.0b3
+    The third beta version of MACS3, addressing Cython issue and with
+    two HMMRATAC options added.
 	   
-	* New features from beta1:
+	* New features from beta2:
 
-	1) HMMRATAC module fixes
+	1) HMMRATAC module
     
-       Cutoff analysis function added
-       Description regarding it has been added
-    
-    2) Memory monitoring in the runtime message
-    
-    3) testing for s390x, armv7 and power64le is back. However, we turned off the function to check if the `hmmratac` results from non-x86 architectures are the same as the standard results, because in order to let the testing run, we need to use old python libraries (scipy and sklearn) through the distribution of Debian/Linux bullseye.
+       --modelonly option: only generate HMM model and quit
+       
+       -t or --training: customized training regions can be provided
+	   through this option.
+	   
+	   --min-frag-p: exclude fragments with abnormal fragment length while generating four
+       signal tracks. #577 Check `macs3 hmmratac -h`.
     
+    2) testing for Mac OS12 is added. 
+
+	3) We require Cython 0.29.*. The new Cython3 will break our
+	codes. We will adopt Cython3 later. #574
+
 ## Install
 
 The common way to install MACS is through
 [PYPI](https://pypi.org/project/macs3/)) or
 [conda](https://anaconda.org/bioconda/macs3). Please check the
 [INSTALL](./docs/INSTALL.md) document for detail.
 
@@ -85,14 +92,20 @@
 architectures:
 
  * x86_64
  * aarch64
  * armv7
  * ppc64le
  * s390x 
+ * Apple chips
+
+In general, you can install through PyPI as `pip install macs3`. 
+To use virtual environment is highly recommended. Or you can install
+after unzipping the released package downloaded from Github, then
+use `pip install .` command.
 
 ## Usage
 
 Example for regular peak calling on TF ChIP-seq:
 
 `macs3 callpeak -t ChIP.bam -c Control.bam -f BAM -g hs -n test -B -q 0.01`
```

### Comparing `MACS3-3.0.0b2/README.md` & `MACS3-3.0.0b3/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # MACS: Model-based Analysis for ChIP-Seq
 
-![Status](https://img.shields.io/pypi/status/macs3.svg) ![License](https://img.shields.io/github/license/macs3-project/MACS) ![Programming languages](https://img.shields.io/github/languages/top/macs3-project/MACS) ![CI x64](https://github.com/macs3-project/MACS/workflows/CI%20x64/badge.svg) ![CI non x64](https://github.com/macs3-project/MACS/workflows/CI%20non%20x64,%20python%203.7/badge.svg)
+![Status](https://img.shields.io/pypi/status/macs3.svg) ![License](https://img.shields.io/github/license/macs3-project/MACS) ![Programming languages](https://img.shields.io/github/languages/top/macs3-project/MACS) ![CI x64](https://github.com/macs3-project/MACS/workflows/CI%20x64/badge.svg) ![CI non x64](https://github.com/macs3-project/MACS/workflows/CI%20non%20x64,%20python%203.7/badge.svg) ![CI MacOS 12](https://github.com/macs3-project/MACS/workflows/CI%20MacOS%2012/badge.svg)
 
 [![PyPI download](https://img.shields.io/pypi/dm/macs3?label=pypi%20downloads)](https://pypistats.org/packages/macs3) [![Bioconda download](https://img.shields.io/conda/dn/bioconda/macs3?label=bioconda%20downloads)](https://anaconda.org/bioconda/macs3)
 
 Latest Release:
 * Github: [![Github Release](https://img.shields.io/github/v/release/macs3-project/MACS)](https://github.com/macs3-project/MACS/releases)
 * PyPI: [![PyPI Release](https://img.shields.io/pypi/v/macs3.svg) ![PyPI Python Version](https://img.shields.io/pypi/pyversions/MACS3) ![PyPI Format](https://img.shields.io/pypi/format/macs3)](https://pypi.org/project/macs3/)
 * Bioconda: [![Bioconda Release](https://img.shields.io/conda/v/bioconda/macs3) ![Bioconda Platform](https://img.shields.io/conda/pn/bioconda/macs3)](https://anaconda.org/bioconda/macs3)
@@ -30,30 +30,37 @@
 
 **Please note that current MACS3 is still in beta stage. However, we
 utilize Github Action to implement the CI (Continous Integration) to
 make sure that the main branch passes unit testing on certain
 functions and subcommands to reproduce the correct outputs. We will
 add more new features in the future.**
 
-## Recent Changes for MACS (3.0.0b2)
+## Recent Changes for MACS (3.0.0b3)
 
-### 3.0.0b2
-    The second beta version of MACS3, with HMMRATAC feature refined.
+### 3.0.0b3
+    The third beta version of MACS3, addressing Cython issue and with
+    two HMMRATAC options added.
 	   
-	* New features from beta1:
+	* New features from beta2:
 
-	1) HMMRATAC module fixes
+	1) HMMRATAC module
     
-       Cutoff analysis function added
-       Description regarding it has been added
-    
-    2) Memory monitoring in the runtime message
-    
-    3) testing for s390x, armv7 and power64le is back. However, we turned off the function to check if the `hmmratac` results from non-x86 architectures are the same as the standard results, because in order to let the testing run, we need to use old python libraries (scipy and sklearn) through the distribution of Debian/Linux bullseye.
+       --modelonly option: only generate HMM model and quit
+       
+       -t or --training: customized training regions can be provided
+	   through this option.
+	   
+	   --min-frag-p: exclude fragments with abnormal fragment length while generating four
+       signal tracks. #577 Check `macs3 hmmratac -h`.
     
+    2) testing for Mac OS12 is added. 
+
+	3) We require Cython 0.29.*. The new Cython3 will break our
+	codes. We will adopt Cython3 later. #574
+
 ## Install
 
 The common way to install MACS is through
 [PYPI](https://pypi.org/project/macs3/)) or
 [conda](https://anaconda.org/bioconda/macs3). Please check the
 [INSTALL](./docs/INSTALL.md) document for detail.
 
@@ -61,14 +68,20 @@
 architectures:
 
  * x86_64
  * aarch64
  * armv7
  * ppc64le
  * s390x 
+ * Apple chips
+
+In general, you can install through PyPI as `pip install macs3`. 
+To use virtual environment is highly recommended. Or you can install
+after unzipping the released package downloaded from Github, then
+use `pip install .` command.
 
 ## Usage
 
 Example for regular peak calling on TF ChIP-seq:
 
 `macs3 callpeak -t ChIP.bam -c Control.bam -f BAM -g hs -n test -B -q 0.01`
```

### Comparing `MACS3-3.0.0b2/bin/macs3` & `MACS3-3.0.0b3/bin/macs3`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 #!/usr/bin/env python
-# Time-stamp: <2023-06-23 12:59:17 Tao Liu>
+# Time-stamp: <2023-07-28 12:14:37 Tao Liu>
 
 """Description: MACS v3 main executable.
 
 This code is free software; you can redistribute it and/or modify it
 under the terms of the BSD License (see the file LICENSE included with
 the distribution).
 """
@@ -916,14 +916,17 @@
                            default = False )
     group_em.add_argument( "--means", dest = "em_means", type = float, nargs = 4,
                             help = "Comma separated list of initial mean values for the fragment distribution for short fragments, mono-, di-, and tri-nucleosomal fragments. Default: 50 200 400 600",
                             default = [50, 200, 400, 600] )
     group_em.add_argument( "--stddevs", dest = "em_stddevs", type = float, nargs = 4,
                             help = "Comma separated list of initial standard deviation values for fragment distribution for short fragments, mono-, di-, and tri-nucleosomal fragments. Default: 20 20 20 20",
                             default = [20, 20, 20, 20] )
+    group_em.add_argument( "--min-frag-p", dest = "min_frag_p", type = float,
+                           help = "We will exclude the abnormal fragments that can't be assigned to any of the four signal tracks. After we use EM to find the means and stddevs of the four distributions, we will calculate the likelihood that a given fragment length fit any of the four using normal distribution. The criteria we will use is that if a fragment length has less than MIN_FRAG_P probability to be like either of short, mono, di, or tri-nuc fragment, we will exclude it while generating the four signal tracks for later HMM training and prediction. The value should be between 0 and 1. Larger the value, more abnormal fragments will be allowed. So if you want to include more 'ideal' fragments, make this value smaller. Default = 0.001",
+                           default = 0.001 )
     # group for HMM
     group_hmm = argparser_hmmratac.add_argument_group( "Hidden Markov Model arguments" )
     #group_hmm.add_argument( "-s", "--states", dest = "hmm_states", type = int,
     #                        help = "Number of States in the model. Default = 3. If not k=3, recommend NOT calling peaks, use bedgraph. This option is named as `--kmeans` in HMMRATAC since it will also control the number of clusters in the k-means clustering process to decide the initial emissions for HMM training.",
     #                        default = 3 )
     group_hmm.add_argument( "--binsize", dest = "hmm_binsize", type = int,
                             help = "Size of the bins to split the pileup signals for training and decoding with Hidden Markov Model. Must >= 1. Smaller the binsize, higher the resolution of the results, slower the process. Default = 10",
@@ -936,26 +939,26 @@
                             default = 10 )
     group_hmm.add_argument( "--maxTrain", dest = "hmm_maxTrain", type = int,
                             help = "Maximum number of training regions to use. After we identify the training regions between `-l` and `-u`, the lower and upper cutoffs, we will randomly pick this number of regions for training. Default: 1000",
                             default = 1000 )
     group_hmm.add_argument( "--training-flanking", dest = "hmm_training_flanking", type = int, required = False,
                             help = "Training regions will be expanded to both side with this number of basepairs. The purpose is to include more background regions. Default: 1000",
                             default = 1000 )
-    #group_hmm.add_argument( "-t", "--training", dest = "hmm_training_regions", type = str, required = False, 
-    #                        help = "Filename of training regions (previously was BED_file) to use for training HMM, instead of using foldchange settings to select. Default: NA" )
+    group_hmm.add_argument( "-t", "--training", dest = "hmm_training_regions", type = str, required = False, 
+                           help = "Filename of training regions (previously was BED_file) to use for training HMM, instead of using foldchange settings to select. Default: NA" )
     #group_hmm.add_argument( "-z", "--zscore", dest = "hmm_zscore", type = int,
     #                        help = "Zscored read depth to mask during Viterbi decoding. Default: 100",
     #                        default = 100 )
     #group_hmm.add_argument( "--window", dest = "hmm_window", type = int,
     #                        help = "Size of the bins to split the genome into for Viterbi decoding. To save memory, the genome is split into WINDOW long bins and viterbi decoding occurs across each bin. Default = 25000000. Note: For machines with limited memory, it is recommended to reduce the size of the bins.",
     #                        default = 25000000 )
     group_hmm.add_argument( "--model", dest = "hmm_file", type = str, required = False, 
                             help = "A JSON file generated from previous HMMRATAC run to use instead of creating new one. When provided, HMM training will be skipped. Default: NA" )
-    #group_hmm.add_argument( "--modelonly", dest = "hmm_modelonly", action = "store_true", default = False,
-    #                        help = "Stop the program after generating model. Use this option to generate HMM model ONLY, which can be later applied with `--model`. Default: False")
+    group_hmm.add_argument( "--modelonly", dest = "hmm_modelonly", action = "store_true", default = False,
+                           help = "Stop the program after generating model. Use this option to generate HMM model ONLY, which can be later applied with `--model`. Default: False")
 
     # group for peak calling arguments
     group_call = argparser_hmmratac.add_argument_group( "Peak calling/HMM decoding arguments" )
     group_call.add_argument( "-c", "--prescan-cutoff", dest = "prescan_cutoff", type = float,
                              help = "The fold change cutoff for prescanning candidate regions in the whole dataset. Then we will use HMM to predict/decode states on these candidate regions. Higher the prescan cutoff, fewer regions will be considered. Must > 1. This is an important parameter for decoding so please read. The purpose of this parameter is to EXCLUDE those chromatin regions having noises/random enrichment so we can have a large number of possible regions to predict the HMM states. It's highly recommended to run the `--cutoff-analysis-only` first to decide the lower cutoff `-l`, the upper cutoff `-u`, and the pre-scanning cutoff `-c`. The pre-scanning cutoff should be the cutoff close to the BOTTOM of the cutoff analysis result that can capture large number of possible peaks with normal length (average length 500-1000bps). In most cases, please do not pick a cutoff too low that capture almost all the background noises from the data. Default: 1.2",
                              default = 1.2 )
```

### Comparing `MACS3-3.0.0b2/docs/INSTALL.md` & `MACS3-3.0.0b3/docs/INSTALL.md`

 * *Files identical despite different names*

### Comparing `MACS3-3.0.0b2/docs/callpeak.md` & `MACS3-3.0.0b3/docs/callpeak.md`

 * *Files identical despite different names*

### Comparing `MACS3-3.0.0b2/docs/hmmratac.md` & `MACS3-3.0.0b3/docs/hmmratac.md`

 * *Files identical despite different names*

### Comparing `MACS3-3.0.0b2/make_docker_base.sh` & `MACS3-3.0.0b3/make_docker_base.sh`

 * *Files identical despite different names*

### Comparing `MACS3-3.0.0b2/setup.py` & `MACS3-3.0.0b3/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -34,16 +34,16 @@
               'Programming Language :: Python :: 3.9',
               'Programming Language :: Python :: 3.10',
               'Programming Language :: Python :: 3.11',
               'Programming Language :: Cython', ]
 
 install_requires = [ "numpy>=1.19",
                      "hmmlearn>=0.3",
-                     "cykhash>=2.0",
-                     "Cython>=0.29" ]
+                     "cykhash>=2.0,<3.0",
+                     "Cython~=0.29" ]
 
 tests_requires = [ 'pytest' ]
 
 
 def main():
     if sys.version_info < (3,8):
         sys.stderr.write("CRITICAL: Python version must >= 3.8!\n")
```

