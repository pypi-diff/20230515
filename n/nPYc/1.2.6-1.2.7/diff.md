# Comparing `tmp/nPYc-1.2.6.tar.gz` & `tmp/nPYc-1.2.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nPYc-1.2.6.tar", last modified: Tue Aug 10 12:39:14 2021, max compression
+gzip compressed data, was "nPYc-1.2.7.tar", last modified: Mon Mar 13 15:59:49 2023, max compression
```

## Comparing `nPYc-1.2.6.tar` & `nPYc-1.2.7.tar`

### file list

```diff
@@ -1,165 +1,165 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-08-10 12:39:14.646822 nPYc-1.2.6/
--rw-r--r--   0 runner    (1001) docker     (121)     1080 2021-08-10 12:33:39.000000 nPYc-1.2.6/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (121)      148 2021-08-10 12:33:39.000000 nPYc-1.2.6/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)     2508 2021-08-10 12:39:14.646822 nPYc-1.2.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     4018 2021-08-10 12:33:39.000000 nPYc-1.2.6/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-08-10 12:39:14.622822 nPYc-1.2.6/nPYc/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-08-10 12:39:14.626822 nPYc-1.2.6/nPYc/StudyDesigns/
--rw-r--r--   0 runner    (1001) docker     (121)      245 2021-08-10 12:33:40.000000 nPYc-1.2.6/nPYc/StudyDesigns/Abbreviations.csv
--rw-r--r--   0 runner    (1001) docker     (121)     4416 2021-08-10 12:33:40.000000 nPYc-1.2.6/nPYc/StudyDesigns/AssayParameters.json
--rw-r--r--   0 runner    (1001) docker     (121)      205 2021-08-10 12:33:40.000000 nPYc-1.2.6/nPYc/StudyDesigns/AssayParametersSchema.json
--rw-r--r--   0 runner    (1001) docker     (121)     1165 2021-08-10 12:33:40.000000 nPYc-1.2.6/nPYc/StudyDesigns/BI-LISA_analyteGroups.json
--rw-r--r--   0 runner    (1001) docker     (121)     1287 2021-08-10 12:33:40.000000 nPYc-1.2.6/nPYc/StudyDesigns/BI-LISA_reference_groups.json
--rw-r--r--   0 runner    (1001) docker     (121)     7669 2021-08-10 12:33:40.000000 nPYc-1.2.6/nPYc/StudyDesigns/BI-LISA_reference_ranges.json
--rw-r--r--   0 runner    (1001) docker     (121)    79621 2021-08-10 12:33:40.000000 nPYc-1.2.6/nPYc/StudyDesigns/BI-LISAref.csv
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-08-10 12:39:14.622822 nPYc-1.2.6/nPYc/StudyDesigns/BlankISATAB/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-08-10 12:39:14.626822 nPYc-1.2.6/nPYc/StudyDesigns/BlankISATAB/blank-ms/
--rw-r--r--   0 runner    (1001) docker     (121)     1319 2021-08-10 12:33:40.000000 nPYc-1.2.6/nPYc/StudyDesigns/BlankISATAB/blank-ms/a_npc-test-study_metabolite_profiling_mass_spectrometry.txt
--rw-r--r--   0 runner    (1001) docker     (121)     4105 2021-08-10 12:33:40.000000 nPYc-1.2.6/nPYc/StudyDesigns/BlankISATAB/blank-ms/i_Investigation.txt
--rw-r--r--   0 runner    (1001) docker     (121)      470 2021-08-10 12:33:40.000000 nPYc-1.2.6/nPYc/StudyDesigns/BlankISATAB/blank-ms/s_NPC-Test-Study.txt
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-08-10 12:39:14.626822 nPYc-1.2.6/nPYc/StudyDesigns/BlankISATAB/blank-nmr/
--rw-r--r--   0 runner    (1001) docker     (121)      747 2021-08-10 12:33:40.000000 nPYc-1.2.6/nPYc/StudyDesigns/BlankISATAB/blank-nmr/a_npc-test-study_metabolite_profiling_NMR_spectroscopy.txt
--rw-r--r--   0 runner    (1001) docker     (121)     4030 2021-08-10 12:33:40.000000 nPYc-1.2.6/nPYc/StudyDesigns/BlankISATAB/blank-nmr/i_Investigation.txt
--rw-r--r--   0 runner    (1001) docker     (121)      424 2021-08-10 12:33:40.000000 nPYc-1.2.6/nPYc/StudyDesigns/BlankISATAB/blank-nmr/s_NPC-Test-Study.txt
--rw-r--r--   0 runner    (1001) docker     (121)     1329 2021-08-10 12:33:40.000000 nPYc-1.2.6/nPYc/StudyDesigns/DilutionSeries.csv
--rw-r--r--   0 runner    (1001) docker     (121)    10162 2021-08-10 12:33:40.000000 nPYc-1.2.6/nPYc/StudyDesigns/ExactMasses.csv
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-08-10 12:39:14.626822 nPYc-1.2.6/nPYc/StudyDesigns/ISATABFieldMappings/
--rw-r--r--   0 runner    (1001) docker     (121)      688 2021-08-10 12:33:40.000000 nPYc-1.2.6/nPYc/StudyDesigns/ISATABFieldMappings/MSFields.json
--rw-r--r--   0 runner    (1001) docker     (121)      334 2021-08-10 12:33:40.000000 nPYc-1.2.6/nPYc/StudyDesigns/ISATABFieldMappings/NMRFields.json
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-08-10 12:39:14.626822 nPYc-1.2.6/nPYc/StudyDesigns/SOP/
--rw-r--r--   0 runner    (1001) docker     (121)     8762 2021-08-10 12:33:40.000000 nPYc-1.2.6/nPYc/StudyDesigns/SOP/AminoAcidMS.json
--rw-r--r--   0 runner    (1001) docker     (121)     1698 2021-08-10 12:33:40.000000 nPYc-1.2.6/nPYc/StudyDesigns/SOP/BrukerBI-LISA.json
--rw-r--r--   0 runner    (1001) docker     (121)     1716 2021-08-10 12:33:40.000000 nPYc-1.2.6/nPYc/StudyDesigns/SOP/BrukerBI-QUANT-PS.json
--rw-r--r--   0 runner    (1001) docker     (121)     1711 2021-08-10 12:33:40.000000 nPYc-1.2.6/nPYc/StudyDesigns/SOP/BrukerQuant-UR.json
--rw-r--r--   0 runner    (1001) docker     (121)      599 2021-08-10 12:33:40.000000 nPYc-1.2.6/nPYc/StudyDesigns/SOP/Generic.json
--rw-r--r--   0 runner    (1001) docker     (121)     4567 2021-08-10 12:33:40.000000 nPYc-1.2.6/nPYc/StudyDesigns/SOP/GenericMS.json
--rw-r--r--   0 runner    (1001) docker     (121)     2671 2021-08-10 12:33:40.000000 nPYc-1.2.6/nPYc/StudyDesigns/SOP/GenericNMRblood.json
--rw-r--r--   0 runner    (1001) docker     (121)     2644 2021-08-10 12:33:40.000000 nPYc-1.2.6/nPYc/StudyDesigns/SOP/GenericNMRurine.json
--rw-r--r--   0 runner    (1001) docker     (121)     2473 2021-08-10 12:33:40.000000 nPYc-1.2.6/nPYc/StudyDesigns/SOP/NMR1Djresblood.json
--rw-r--r--   0 runner    (1001) docker     (121)     2468 2021-08-10 12:33:40.000000 nPYc-1.2.6/nPYc/StudyDesigns/SOP/NMR1Djresurine.json
--rw-r--r--   0 runner    (1001) docker     (121)    10044 2021-08-10 12:33:40.000000 nPYc-1.2.6/nPYc/StudyDesigns/SOP/OxylipinMS.json
--rwxr-xr-x   0 runner    (1001) docker     (121)     5865 2021-08-10 12:33:40.000000 nPYc-1.2.6/nPYc/StudyDesigns/SOP/TryptophanMS.json
--rw-r--r--   0 runner    (1001) docker     (121)      625 2021-08-10 12:33:40.000000 nPYc-1.2.6/nPYc/StudyDesigns/colours.json
--rw-r--r--   0 runner    (1001) docker     (121)     1334 2021-08-10 12:33:40.000000 nPYc-1.2.6/nPYc/StudyDesigns/urine_quant_b_reference_groups.json
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-08-10 12:39:14.630822 nPYc-1.2.6/nPYc/Templates/
--rw-r--r--   0 runner    (1001) docker     (121)     5079 2021-08-10 12:33:40.000000 nPYc-1.2.6/nPYc/Templates/ID_request_MS.html
--rw-r--r--   0 runner    (1001) docker     (121)      912 2021-08-10 12:33:40.000000 nPYc-1.2.6/nPYc/Templates/MS_BatchCorrectionAssessmentReport.html
--rw-r--r--   0 runner    (1001) docker     (121)     2093 2021-08-10 12:33:40.000000 nPYc-1.2.6/nPYc/Templates/MS_BatchCorrectionSummaryReport.html
--rw-r--r--   0 runner    (1001) docker     (121)     1870 2021-08-10 12:33:40.000000 nPYc-1.2.6/nPYc/Templates/MS_CorrelationToDilutionReport.html
--rw-r--r--   0 runner    (1001) docker     (121)     1821 2021-08-10 12:33:40.000000 nPYc-1.2.6/nPYc/Templates/MS_FeatureSelectionReport.html
--rw-r--r--   0 runner    (1001) docker     (121)     4632 2021-08-10 12:33:40.000000 nPYc-1.2.6/nPYc/Templates/MS_FeatureSummaryReport.html
--rw-r--r--   0 runner    (1001) docker     (121)     4386 2021-08-10 12:33:40.000000 nPYc-1.2.6/nPYc/Templates/MS_FinalSummaryReport.html
--rw-r--r--   0 runner    (1001) docker     (121)     3432 2021-08-10 12:33:40.000000 nPYc-1.2.6/nPYc/Templates/MS_FinalSummaryReport_Abridged.html
--rw-r--r--   0 runner    (1001) docker     (121)     4955 2021-08-10 12:33:40.000000 nPYc-1.2.6/nPYc/Templates/MS_peakPantheR_FinalSummaryReport.html
--rw-r--r--   0 runner    (1001) docker     (121)     2518 2021-08-10 12:33:40.000000 nPYc-1.2.6/nPYc/Templates/NMR_FinalSummaryReport.html
--rw-r--r--   0 runner    (1001) docker     (121)     2176 2021-08-10 12:33:40.000000 nPYc-1.2.6/nPYc/Templates/NMR_QCSummaryReport.html
--rw-r--r--   0 runner    (1001) docker     (121)     8972 2021-08-10 12:33:40.000000 nPYc-1.2.6/nPYc/Templates/NPC_MultivariateReport.html
--rw-r--r--   0 runner    (1001) docker     (121)     4154 2021-08-10 12:33:40.000000 nPYc-1.2.6/nPYc/Templates/Targeted_FeatureSummaryReport.html
--rw-r--r--   0 runner    (1001) docker     (121)     4319 2021-08-10 12:33:40.000000 nPYc-1.2.6/nPYc/Templates/Targeted_FinalReportMS.html
--rw-r--r--   0 runner    (1001) docker     (121)     4882 2021-08-10 12:33:40.000000 nPYc-1.2.6/nPYc/Templates/Targeted_FinalReportNMR.html
--rw-r--r--   0 runner    (1001) docker     (121)     1824 2021-08-10 12:33:40.000000 nPYc-1.2.6/nPYc/Templates/Targeted_MergeLOQReport.html
--rw-r--r--   0 runner    (1001) docker     (121)       34 2021-08-10 12:33:40.000000 nPYc-1.2.6/nPYc/Templates/base_QC.html
--rw-r--r--   0 runner    (1001) docker     (121)     1348 2021-08-10 12:33:40.000000 nPYc-1.2.6/nPYc/Templates/base_generic.html
--rw-r--r--   0 runner    (1001) docker     (121)      826 2021-08-10 12:33:40.000000 nPYc-1.2.6/nPYc/Templates/featureDistributionReport.html
--rw-r--r--   0 runner    (1001) docker     (121)     3032 2021-08-10 12:33:40.000000 nPYc-1.2.6/nPYc/Templates/generateReportBILISA.html
--rw-r--r--   0 runner    (1001) docker     (121)     2201 2021-08-10 12:33:40.000000 nPYc-1.2.6/nPYc/Templates/generateReportBIQuantUR.html
--rw-r--r--   0 runner    (1001) docker     (121)    11797 2021-08-10 12:33:40.000000 nPYc-1.2.6/nPYc/Templates/generateReportTargeted.html
--rw-r--r--   0 runner    (1001) docker     (121)      246 2021-08-10 12:33:40.000000 nPYc-1.2.6/nPYc/Templates/generateSampleReport.html
--rw-r--r--   0 runner    (1001) docker     (121)     7291 2021-08-10 12:33:40.000000 nPYc-1.2.6/nPYc/Templates/npc-main.css
--rw-r--r--   0 runner    (1001) docker     (121)      775 2021-08-10 12:33:40.000000 nPYc-1.2.6/nPYc/Templates/pcaReport.html
--rw-r--r--   0 runner    (1001) docker     (121)     1941 2021-08-10 12:33:40.000000 nPYc-1.2.6/nPYc/Templates/sampleReportChunk.html
--rw-r--r--   0 runner    (1001) docker     (121)    18396 2021-08-10 12:33:40.000000 nPYc-1.2.6/nPYc/Templates/toolbox_logo.png
--rw-r--r--   0 runner    (1001) docker     (121)      567 2021-08-10 12:33:40.000000 nPYc-1.2.6/nPYc/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      161 2021-08-10 12:33:40.000000 nPYc-1.2.6/nPYc/_toolboxPath.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-08-10 12:39:14.630822 nPYc-1.2.6/nPYc/batchAndROCorrection/
--rw-r--r--   0 runner    (1001) docker     (121)       92 2021-08-10 12:33:40.000000 nPYc-1.2.6/nPYc/batchAndROCorrection/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (121)    11506 2021-08-10 12:33:40.000000 nPYc-1.2.6/nPYc/batchAndROCorrection/_batchAndROCorrection.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-08-10 12:39:14.630822 nPYc-1.2.6/nPYc/enumerations/
--rw-r--r--   0 runner    (1001) docker     (121)      528 2021-08-10 12:33:40.000000 nPYc-1.2.6/nPYc/enumerations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     5792 2021-08-10 12:33:40.000000 nPYc-1.2.6/nPYc/enumerations/_enumerations.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-08-10 12:39:14.630822 nPYc-1.2.6/nPYc/multivariate/
--rw-r--r--   0 runner    (1001) docker     (121)      593 2021-08-10 12:33:40.000000 nPYc-1.2.6/nPYc/multivariate/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     3569 2021-08-10 12:33:40.000000 nPYc-1.2.6/nPYc/multivariate/exploratoryAnalysisPCA.py
--rw-r--r--   0 runner    (1001) docker     (121)     4128 2021-08-10 12:33:40.000000 nPYc-1.2.6/nPYc/multivariate/multivariateUtilities.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-08-10 12:39:14.634822 nPYc-1.2.6/nPYc/objects/
--rw-r--r--   0 runner    (1001) docker     (121)      214 2021-08-10 12:33:40.000000 nPYc-1.2.6/nPYc/objects/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)   114092 2021-08-10 12:33:40.000000 nPYc-1.2.6/nPYc/objects/_dataset.py
--rw-r--r--   0 runner    (1001) docker     (121)   125993 2021-08-10 12:33:40.000000 nPYc-1.2.6/nPYc/objects/_msDataset.py
--rw-r--r--   0 runner    (1001) docker     (121)    28555 2021-08-10 12:33:40.000000 nPYc-1.2.6/nPYc/objects/_nmrDataset.py
--rw-r--r--   0 runner    (1001) docker     (121)   247448 2021-08-10 12:33:40.000000 nPYc-1.2.6/nPYc/objects/_targetedDataset.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-08-10 12:39:14.638822 nPYc-1.2.6/nPYc/plotting/
--rw-r--r--   0 runner    (1001) docker     (121)     3297 2021-08-10 12:33:40.000000 nPYc-1.2.6/nPYc/plotting/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     2991 2021-08-10 12:33:40.000000 nPYc-1.2.6/nPYc/plotting/_correlationSpectroscopy.py
--rw-r--r--   0 runner    (1001) docker     (121)     3779 2021-08-10 12:33:40.000000 nPYc-1.2.6/nPYc/plotting/_jointplotRSDvCorrelation.py
--rw-r--r--   0 runner    (1001) docker     (121)    40743 2021-08-10 12:33:40.000000 nPYc-1.2.6/nPYc/plotting/_multivariatePlotting.py
--rw-r--r--   0 runner    (1001) docker     (121)    14168 2021-08-10 12:33:40.000000 nPYc-1.2.6/nPYc/plotting/_nmrPlotting.py
--rw-r--r--   0 runner    (1001) docker     (121)    10498 2021-08-10 12:33:40.000000 nPYc-1.2.6/nPYc/plotting/_plotBatchAndROCorrection.py
--rw-r--r--   0 runner    (1001) docker     (121)     3425 2021-08-10 12:33:40.000000 nPYc-1.2.6/nPYc/plotting/_plotDiscreteLoadings.py
--rw-r--r--   0 runner    (1001) docker     (121)     5715 2021-08-10 12:33:40.000000 nPYc-1.2.6/nPYc/plotting/_plotFeatureAccuracyPrecision.py
--rw-r--r--   0 runner    (1001) docker     (121)    10732 2021-08-10 12:33:40.000000 nPYc-1.2.6/nPYc/plotting/_plotFeatureLOQ.py
--rw-r--r--   0 runner    (1001) docker     (121)     5749 2021-08-10 12:33:40.000000 nPYc-1.2.6/nPYc/plotting/_plotFeatureRanges.py
--rw-r--r--   0 runner    (1001) docker     (121)     5090 2021-08-10 12:33:40.000000 nPYc-1.2.6/nPYc/plotting/_plotIonMap.py
--rw-r--r--   0 runner    (1001) docker     (121)    17340 2021-08-10 12:33:40.000000 nPYc-1.2.6/nPYc/plotting/_plotLOQFeatureViolin.py
--rw-r--r--   0 runner    (1001) docker     (121)    18942 2021-08-10 12:33:40.000000 nPYc-1.2.6/nPYc/plotting/_plotLOQRunOrder.py
--rw-r--r--   0 runner    (1001) docker     (121)     5391 2021-08-10 12:33:40.000000 nPYc-1.2.6/nPYc/plotting/_plotNMRbaseline.py
--rw-r--r--   0 runner    (1001) docker     (121)     3631 2021-08-10 12:33:40.000000 nPYc-1.2.6/nPYc/plotting/_plotNMRcalibration.py
--rw-r--r--   0 runner    (1001) docker     (121)     4466 2021-08-10 12:33:40.000000 nPYc-1.2.6/nPYc/plotting/_plotNMRsolvent.py
--rw-r--r--   0 runner    (1001) docker     (121)     9075 2021-08-10 12:33:40.000000 nPYc-1.2.6/nPYc/plotting/_plotRSDs.py
--rw-r--r--   0 runner    (1001) docker     (121)     8042 2021-08-10 12:33:40.000000 nPYc-1.2.6/nPYc/plotting/_plotSpectralVariance.py
--rw-r--r--   0 runner    (1001) docker     (121)    12005 2021-08-10 12:33:40.000000 nPYc-1.2.6/nPYc/plotting/_plotTIC.py
--rw-r--r--   0 runner    (1001) docker     (121)     3229 2021-08-10 12:33:40.000000 nPYc-1.2.6/nPYc/plotting/_plotTargeted.py
--rw-r--r--   0 runner    (1001) docker     (121)     3510 2021-08-10 12:33:40.000000 nPYc-1.2.6/nPYc/plotting/_plotTargetedFeatureDistribution.py
--rw-r--r--   0 runner    (1001) docker     (121)     9853 2021-08-10 12:33:40.000000 nPYc-1.2.6/nPYc/plotting/_plotVariableScatter.py
--rw-r--r--   0 runner    (1001) docker     (121)    17882 2021-08-10 12:33:40.000000 nPYc-1.2.6/nPYc/plotting/_plotting.py
--rw-r--r--   0 runner    (1001) docker     (121)      875 2021-08-10 12:33:40.000000 nPYc-1.2.6/nPYc/plotting/_rangeFrameLocator.py
--rw-r--r--   0 runner    (1001) docker     (121)     1671 2021-08-10 12:33:40.000000 nPYc-1.2.6/nPYc/plotting/_violinPlot.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-08-10 12:39:14.642822 nPYc-1.2.6/nPYc/reports/
--rw-r--r--   0 runner    (1001) docker     (121)      794 2021-08-10 12:33:40.000000 nPYc-1.2.6/nPYc/reports/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    20642 2021-08-10 12:33:40.000000 nPYc-1.2.6/nPYc/reports/_finalReportPeakPantheR.py
--rw-r--r--   0 runner    (1001) docker     (121)     3129 2021-08-10 12:33:40.000000 nPYc-1.2.6/nPYc/reports/_generateBasicPCAReport.py
--rw-r--r--   0 runner    (1001) docker     (121)     3070 2021-08-10 12:33:40.000000 nPYc-1.2.6/nPYc/reports/_generateFeatureDistributionReport.py
--rw-r--r--   0 runner    (1001) docker     (121)    86395 2021-08-10 12:33:40.000000 nPYc-1.2.6/nPYc/reports/_generateReportMS.py
--rw-r--r--   0 runner    (1001) docker     (121)    14173 2021-08-10 12:33:40.000000 nPYc-1.2.6/nPYc/reports/_generateReportNMR.py
--rw-r--r--   0 runner    (1001) docker     (121)    59107 2021-08-10 12:33:40.000000 nPYc-1.2.6/nPYc/reports/_generateReportTargeted.py
--rw-r--r--   0 runner    (1001) docker     (121)    10134 2021-08-10 12:33:40.000000 nPYc-1.2.6/nPYc/reports/_generateSampleReport.py
--rw-r--r--   0 runner    (1001) docker     (121)    20602 2021-08-10 12:33:40.000000 nPYc-1.2.6/nPYc/reports/featureID.py
--rw-r--r--   0 runner    (1001) docker     (121)     6569 2021-08-10 12:33:40.000000 nPYc-1.2.6/nPYc/reports/generateReport.py
--rw-r--r--   0 runner    (1001) docker     (121)       73 2021-08-10 12:33:40.000000 nPYc-1.2.6/nPYc/reports/metadata.py
--rw-r--r--   0 runner    (1001) docker     (121)    33781 2021-08-10 12:33:40.000000 nPYc-1.2.6/nPYc/reports/multivariateReport.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-08-10 12:39:14.646822 nPYc-1.2.6/nPYc/utilities/
--rw-r--r--   0 runner    (1001) docker     (121)      531 2021-08-10 12:33:40.000000 nPYc-1.2.6/nPYc/utilities/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1230 2021-08-10 12:33:40.000000 nPYc-1.2.6/nPYc/utilities/_addReferenceRanges.py
--rw-r--r--   0 runner    (1001) docker     (121)     2920 2021-08-10 12:33:40.000000 nPYc-1.2.6/nPYc/utilities/_buildSpectrumFromQIfeature.py
--rw-r--r--   0 runner    (1001) docker     (121)     5309 2021-08-10 12:33:40.000000 nPYc-1.2.6/nPYc/utilities/_calibratePPMscale.py
--rw-r--r--   0 runner    (1001) docker     (121)     1172 2021-08-10 12:33:40.000000 nPYc-1.2.6/nPYc/utilities/_checkInRange.py
--rw-r--r--   0 runner    (1001) docker     (121)      674 2021-08-10 12:33:40.000000 nPYc-1.2.6/nPYc/utilities/_conditionalJoin.py
--rw-r--r--   0 runner    (1001) docker     (121)     1959 2021-08-10 12:33:40.000000 nPYc-1.2.6/nPYc/utilities/_filters.py
--rw-r--r--   0 runner    (1001) docker     (121)    13536 2021-08-10 12:33:40.000000 nPYc-1.2.6/nPYc/utilities/_fitPeak.py
--rw-r--r--   0 runner    (1001) docker     (121)     2949 2021-08-10 12:33:40.000000 nPYc-1.2.6/nPYc/utilities/_getMetadataFromBrukerNMR.py
--rw-r--r--   0 runner    (1001) docker     (121)     2017 2021-08-10 12:33:40.000000 nPYc-1.2.6/nPYc/utilities/_getMetadataFromWatersRaw.py
--rw-r--r--   0 runner    (1001) docker     (121)     2504 2021-08-10 12:33:40.000000 nPYc-1.2.6/nPYc/utilities/_getMetadataFrommzML.py
--rw-r--r--   0 runner    (1001) docker     (121)     6715 2021-08-10 12:33:40.000000 nPYc-1.2.6/nPYc/utilities/_importBrukerSpectrum.py
--rw-r--r--   0 runner    (1001) docker     (121)     2253 2021-08-10 12:33:40.000000 nPYc-1.2.6/nPYc/utilities/_internal.py
--rw-r--r--   0 runner    (1001) docker     (121)     1666 2021-08-10 12:33:40.000000 nPYc-1.2.6/nPYc/utilities/_lineWidth.py
--rw-r--r--   0 runner    (1001) docker     (121)     3816 2021-08-10 12:33:40.000000 nPYc-1.2.6/nPYc/utilities/_massSpectrumBuilder.py
--rw-r--r--   0 runner    (1001) docker     (121)     3300 2021-08-10 12:33:40.000000 nPYc-1.2.6/nPYc/utilities/_nmr.py
--rw-r--r--   0 runner    (1001) docker     (121)     1494 2021-08-10 12:33:40.000000 nPYc-1.2.6/nPYc/utilities/_npc_sampleledger.py
--rw-r--r--   0 runner    (1001) docker     (121)     6295 2021-08-10 12:33:40.000000 nPYc-1.2.6/nPYc/utilities/_readBrukerXML.py
--rwxr-xr-x   0 runner    (1001) docker     (121)     7347 2021-08-10 12:33:40.000000 nPYc-1.2.6/nPYc/utilities/extractParams.py
--rw-r--r--   0 runner    (1001) docker     (121)      766 2021-08-10 12:33:40.000000 nPYc-1.2.6/nPYc/utilities/generic.py
--rw-r--r--   0 runner    (1001) docker     (121)     5096 2021-08-10 12:33:40.000000 nPYc-1.2.6/nPYc/utilities/ms.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-08-10 12:39:14.646822 nPYc-1.2.6/nPYc/utilities/normalisation/
--rw-r--r--   0 runner    (1001) docker     (121)      948 2021-08-10 12:33:40.000000 nPYc-1.2.6/nPYc/utilities/normalisation/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     2916 2021-08-10 12:33:40.000000 nPYc-1.2.6/nPYc/utilities/normalisation/_normaliserABC.py
--rw-r--r--   0 runner    (1001) docker     (121)     1194 2021-08-10 12:33:40.000000 nPYc-1.2.6/nPYc/utilities/normalisation/_nullNormaliser.py
--rw-r--r--   0 runner    (1001) docker     (121)     4175 2021-08-10 12:33:40.000000 nPYc-1.2.6/nPYc/utilities/normalisation/_probabilisticQuotientNormaliser.py
--rw-r--r--   0 runner    (1001) docker     (121)     1930 2021-08-10 12:33:40.000000 nPYc-1.2.6/nPYc/utilities/normalisation/_totalAreaNormaliser.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-08-10 12:39:14.626822 nPYc-1.2.6/nPYc.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     2508 2021-08-10 12:39:14.000000 nPYc-1.2.6/nPYc.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     5538 2021-08-10 12:39:14.000000 nPYc-1.2.6/nPYc.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2021-08-10 12:39:14.000000 nPYc-1.2.6/nPYc.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2021-08-10 12:39:14.000000 nPYc-1.2.6/nPYc.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (121)      271 2021-08-10 12:39:14.000000 nPYc-1.2.6/nPYc.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)        5 2021-08-10 12:39:14.000000 nPYc-1.2.6/nPYc.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)       38 2021-08-10 12:39:14.646822 nPYc-1.2.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     2776 2021-08-10 12:33:40.000000 nPYc-1.2.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-13 15:59:49.102905 nPYc-1.2.7/
+-rw-r--r--   0 runner    (1001) docker     (123)     1080 2023-03-13 15:55:02.000000 nPYc-1.2.7/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-03-13 15:55:02.000000 nPYc-1.2.7/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     2218 2023-03-13 15:59:49.102905 nPYc-1.2.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4018 2023-03-13 15:55:02.000000 nPYc-1.2.7/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-13 15:59:49.078905 nPYc-1.2.7/nPYc/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-13 15:59:49.082905 nPYc-1.2.7/nPYc/StudyDesigns/
+-rw-r--r--   0 runner    (1001) docker     (123)      245 2023-03-13 15:55:02.000000 nPYc-1.2.7/nPYc/StudyDesigns/Abbreviations.csv
+-rw-r--r--   0 runner    (1001) docker     (123)     4416 2023-03-13 15:55:02.000000 nPYc-1.2.7/nPYc/StudyDesigns/AssayParameters.json
+-rw-r--r--   0 runner    (1001) docker     (123)      205 2023-03-13 15:55:02.000000 nPYc-1.2.7/nPYc/StudyDesigns/AssayParametersSchema.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1165 2023-03-13 15:55:02.000000 nPYc-1.2.7/nPYc/StudyDesigns/BI-LISA_analyteGroups.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1287 2023-03-13 15:55:02.000000 nPYc-1.2.7/nPYc/StudyDesigns/BI-LISA_reference_groups.json
+-rw-r--r--   0 runner    (1001) docker     (123)     7669 2023-03-13 15:55:02.000000 nPYc-1.2.7/nPYc/StudyDesigns/BI-LISA_reference_ranges.json
+-rw-r--r--   0 runner    (1001) docker     (123)    79621 2023-03-13 15:55:02.000000 nPYc-1.2.7/nPYc/StudyDesigns/BI-LISAref.csv
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-13 15:59:49.078905 nPYc-1.2.7/nPYc/StudyDesigns/BlankISATAB/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-13 15:59:49.082905 nPYc-1.2.7/nPYc/StudyDesigns/BlankISATAB/blank-ms/
+-rw-r--r--   0 runner    (1001) docker     (123)     1319 2023-03-13 15:55:02.000000 nPYc-1.2.7/nPYc/StudyDesigns/BlankISATAB/blank-ms/a_npc-test-study_metabolite_profiling_mass_spectrometry.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     4105 2023-03-13 15:55:02.000000 nPYc-1.2.7/nPYc/StudyDesigns/BlankISATAB/blank-ms/i_Investigation.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      470 2023-03-13 15:55:02.000000 nPYc-1.2.7/nPYc/StudyDesigns/BlankISATAB/blank-ms/s_NPC-Test-Study.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-13 15:59:49.082905 nPYc-1.2.7/nPYc/StudyDesigns/BlankISATAB/blank-nmr/
+-rw-r--r--   0 runner    (1001) docker     (123)      747 2023-03-13 15:55:02.000000 nPYc-1.2.7/nPYc/StudyDesigns/BlankISATAB/blank-nmr/a_npc-test-study_metabolite_profiling_NMR_spectroscopy.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     4030 2023-03-13 15:55:02.000000 nPYc-1.2.7/nPYc/StudyDesigns/BlankISATAB/blank-nmr/i_Investigation.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      424 2023-03-13 15:55:02.000000 nPYc-1.2.7/nPYc/StudyDesigns/BlankISATAB/blank-nmr/s_NPC-Test-Study.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1329 2023-03-13 15:55:02.000000 nPYc-1.2.7/nPYc/StudyDesigns/DilutionSeries.csv
+-rw-r--r--   0 runner    (1001) docker     (123)    10162 2023-03-13 15:55:02.000000 nPYc-1.2.7/nPYc/StudyDesigns/ExactMasses.csv
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-13 15:59:49.082905 nPYc-1.2.7/nPYc/StudyDesigns/ISATABFieldMappings/
+-rw-r--r--   0 runner    (1001) docker     (123)      688 2023-03-13 15:55:02.000000 nPYc-1.2.7/nPYc/StudyDesigns/ISATABFieldMappings/MSFields.json
+-rw-r--r--   0 runner    (1001) docker     (123)      334 2023-03-13 15:55:02.000000 nPYc-1.2.7/nPYc/StudyDesigns/ISATABFieldMappings/NMRFields.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-13 15:59:49.086905 nPYc-1.2.7/nPYc/StudyDesigns/SOP/
+-rw-r--r--   0 runner    (1001) docker     (123)     8762 2023-03-13 15:55:02.000000 nPYc-1.2.7/nPYc/StudyDesigns/SOP/AminoAcidMS.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1698 2023-03-13 15:55:02.000000 nPYc-1.2.7/nPYc/StudyDesigns/SOP/BrukerBI-LISA.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1716 2023-03-13 15:55:02.000000 nPYc-1.2.7/nPYc/StudyDesigns/SOP/BrukerBI-QUANT-PS.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1711 2023-03-13 15:55:02.000000 nPYc-1.2.7/nPYc/StudyDesigns/SOP/BrukerQuant-UR.json
+-rw-r--r--   0 runner    (1001) docker     (123)      599 2023-03-13 15:55:02.000000 nPYc-1.2.7/nPYc/StudyDesigns/SOP/Generic.json
+-rw-r--r--   0 runner    (1001) docker     (123)     4567 2023-03-13 15:55:02.000000 nPYc-1.2.7/nPYc/StudyDesigns/SOP/GenericMS.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2671 2023-03-13 15:55:02.000000 nPYc-1.2.7/nPYc/StudyDesigns/SOP/GenericNMRblood.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2644 2023-03-13 15:55:02.000000 nPYc-1.2.7/nPYc/StudyDesigns/SOP/GenericNMRurine.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2473 2023-03-13 15:55:02.000000 nPYc-1.2.7/nPYc/StudyDesigns/SOP/NMR1Djresblood.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2468 2023-03-13 15:55:02.000000 nPYc-1.2.7/nPYc/StudyDesigns/SOP/NMR1Djresurine.json
+-rw-r--r--   0 runner    (1001) docker     (123)    10044 2023-03-13 15:55:02.000000 nPYc-1.2.7/nPYc/StudyDesigns/SOP/OxylipinMS.json
+-rwxr-xr-x   0 runner    (1001) docker     (123)     5865 2023-03-13 15:55:02.000000 nPYc-1.2.7/nPYc/StudyDesigns/SOP/TryptophanMS.json
+-rw-r--r--   0 runner    (1001) docker     (123)      625 2023-03-13 15:55:02.000000 nPYc-1.2.7/nPYc/StudyDesigns/colours.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1334 2023-03-13 15:55:02.000000 nPYc-1.2.7/nPYc/StudyDesigns/urine_quant_b_reference_groups.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-13 15:59:49.090905 nPYc-1.2.7/nPYc/Templates/
+-rw-r--r--   0 runner    (1001) docker     (123)     5079 2023-03-13 15:55:02.000000 nPYc-1.2.7/nPYc/Templates/ID_request_MS.html
+-rw-r--r--   0 runner    (1001) docker     (123)      912 2023-03-13 15:55:02.000000 nPYc-1.2.7/nPYc/Templates/MS_BatchCorrectionAssessmentReport.html
+-rw-r--r--   0 runner    (1001) docker     (123)     2093 2023-03-13 15:55:02.000000 nPYc-1.2.7/nPYc/Templates/MS_BatchCorrectionSummaryReport.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1870 2023-03-13 15:55:02.000000 nPYc-1.2.7/nPYc/Templates/MS_CorrelationToDilutionReport.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1821 2023-03-13 15:55:02.000000 nPYc-1.2.7/nPYc/Templates/MS_FeatureSelectionReport.html
+-rw-r--r--   0 runner    (1001) docker     (123)     4632 2023-03-13 15:55:02.000000 nPYc-1.2.7/nPYc/Templates/MS_FeatureSummaryReport.html
+-rw-r--r--   0 runner    (1001) docker     (123)     4386 2023-03-13 15:55:02.000000 nPYc-1.2.7/nPYc/Templates/MS_FinalSummaryReport.html
+-rw-r--r--   0 runner    (1001) docker     (123)     3432 2023-03-13 15:55:02.000000 nPYc-1.2.7/nPYc/Templates/MS_FinalSummaryReport_Abridged.html
+-rw-r--r--   0 runner    (1001) docker     (123)     4955 2023-03-13 15:55:02.000000 nPYc-1.2.7/nPYc/Templates/MS_peakPantheR_FinalSummaryReport.html
+-rw-r--r--   0 runner    (1001) docker     (123)     2518 2023-03-13 15:55:02.000000 nPYc-1.2.7/nPYc/Templates/NMR_FinalSummaryReport.html
+-rw-r--r--   0 runner    (1001) docker     (123)     2176 2023-03-13 15:55:02.000000 nPYc-1.2.7/nPYc/Templates/NMR_QCSummaryReport.html
+-rw-r--r--   0 runner    (1001) docker     (123)     8972 2023-03-13 15:55:02.000000 nPYc-1.2.7/nPYc/Templates/NPC_MultivariateReport.html
+-rw-r--r--   0 runner    (1001) docker     (123)     4154 2023-03-13 15:55:02.000000 nPYc-1.2.7/nPYc/Templates/Targeted_FeatureSummaryReport.html
+-rw-r--r--   0 runner    (1001) docker     (123)     4319 2023-03-13 15:55:02.000000 nPYc-1.2.7/nPYc/Templates/Targeted_FinalReportMS.html
+-rw-r--r--   0 runner    (1001) docker     (123)     4882 2023-03-13 15:55:02.000000 nPYc-1.2.7/nPYc/Templates/Targeted_FinalReportNMR.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1824 2023-03-13 15:55:02.000000 nPYc-1.2.7/nPYc/Templates/Targeted_MergeLOQReport.html
+-rw-r--r--   0 runner    (1001) docker     (123)       34 2023-03-13 15:55:02.000000 nPYc-1.2.7/nPYc/Templates/base_QC.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1348 2023-03-13 15:55:02.000000 nPYc-1.2.7/nPYc/Templates/base_generic.html
+-rw-r--r--   0 runner    (1001) docker     (123)      826 2023-03-13 15:55:02.000000 nPYc-1.2.7/nPYc/Templates/featureDistributionReport.html
+-rw-r--r--   0 runner    (1001) docker     (123)     3032 2023-03-13 15:55:02.000000 nPYc-1.2.7/nPYc/Templates/generateReportBILISA.html
+-rw-r--r--   0 runner    (1001) docker     (123)     2201 2023-03-13 15:55:02.000000 nPYc-1.2.7/nPYc/Templates/generateReportBIQuantUR.html
+-rw-r--r--   0 runner    (1001) docker     (123)    11797 2023-03-13 15:55:02.000000 nPYc-1.2.7/nPYc/Templates/generateReportTargeted.html
+-rw-r--r--   0 runner    (1001) docker     (123)      246 2023-03-13 15:55:02.000000 nPYc-1.2.7/nPYc/Templates/generateSampleReport.html
+-rw-r--r--   0 runner    (1001) docker     (123)     7291 2023-03-13 15:55:02.000000 nPYc-1.2.7/nPYc/Templates/npc-main.css
+-rw-r--r--   0 runner    (1001) docker     (123)      775 2023-03-13 15:55:02.000000 nPYc-1.2.7/nPYc/Templates/pcaReport.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1941 2023-03-13 15:55:02.000000 nPYc-1.2.7/nPYc/Templates/sampleReportChunk.html
+-rw-r--r--   0 runner    (1001) docker     (123)    18396 2023-03-13 15:55:02.000000 nPYc-1.2.7/nPYc/Templates/toolbox_logo.png
+-rw-r--r--   0 runner    (1001) docker     (123)      569 2023-03-13 15:55:02.000000 nPYc-1.2.7/nPYc/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      161 2023-03-13 15:55:02.000000 nPYc-1.2.7/nPYc/_toolboxPath.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-13 15:59:49.090905 nPYc-1.2.7/nPYc/batchAndROCorrection/
+-rw-r--r--   0 runner    (1001) docker     (123)       92 2023-03-13 15:55:02.000000 nPYc-1.2.7/nPYc/batchAndROCorrection/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    12001 2023-03-13 15:55:02.000000 nPYc-1.2.7/nPYc/batchAndROCorrection/_batchAndROCorrection.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-13 15:59:49.090905 nPYc-1.2.7/nPYc/enumerations/
+-rw-r--r--   0 runner    (1001) docker     (123)      528 2023-03-13 15:55:02.000000 nPYc-1.2.7/nPYc/enumerations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5792 2023-03-13 15:55:02.000000 nPYc-1.2.7/nPYc/enumerations/_enumerations.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-13 15:59:49.090905 nPYc-1.2.7/nPYc/multivariate/
+-rw-r--r--   0 runner    (1001) docker     (123)      593 2023-03-13 15:55:02.000000 nPYc-1.2.7/nPYc/multivariate/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3569 2023-03-13 15:55:02.000000 nPYc-1.2.7/nPYc/multivariate/exploratoryAnalysisPCA.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4128 2023-03-13 15:55:02.000000 nPYc-1.2.7/nPYc/multivariate/multivariateUtilities.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-13 15:59:49.090905 nPYc-1.2.7/nPYc/objects/
+-rw-r--r--   0 runner    (1001) docker     (123)      214 2023-03-13 15:55:02.000000 nPYc-1.2.7/nPYc/objects/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    95647 2023-03-13 15:55:02.000000 nPYc-1.2.7/nPYc/objects/_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)   133407 2023-03-13 15:55:02.000000 nPYc-1.2.7/nPYc/objects/_msDataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18000 2023-03-13 15:55:02.000000 nPYc-1.2.7/nPYc/objects/_nmrDataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)   247448 2023-03-13 15:55:02.000000 nPYc-1.2.7/nPYc/objects/_targetedDataset.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-13 15:59:49.094905 nPYc-1.2.7/nPYc/plotting/
+-rw-r--r--   0 runner    (1001) docker     (123)     3297 2023-03-13 15:55:02.000000 nPYc-1.2.7/nPYc/plotting/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2991 2023-03-13 15:55:02.000000 nPYc-1.2.7/nPYc/plotting/_correlationSpectroscopy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3779 2023-03-13 15:55:02.000000 nPYc-1.2.7/nPYc/plotting/_jointplotRSDvCorrelation.py
+-rw-r--r--   0 runner    (1001) docker     (123)    40818 2023-03-13 15:55:02.000000 nPYc-1.2.7/nPYc/plotting/_multivariatePlotting.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14168 2023-03-13 15:55:02.000000 nPYc-1.2.7/nPYc/plotting/_nmrPlotting.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10498 2023-03-13 15:55:02.000000 nPYc-1.2.7/nPYc/plotting/_plotBatchAndROCorrection.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3425 2023-03-13 15:55:02.000000 nPYc-1.2.7/nPYc/plotting/_plotDiscreteLoadings.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5715 2023-03-13 15:55:02.000000 nPYc-1.2.7/nPYc/plotting/_plotFeatureAccuracyPrecision.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10732 2023-03-13 15:55:02.000000 nPYc-1.2.7/nPYc/plotting/_plotFeatureLOQ.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5749 2023-03-13 15:55:02.000000 nPYc-1.2.7/nPYc/plotting/_plotFeatureRanges.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5090 2023-03-13 15:55:02.000000 nPYc-1.2.7/nPYc/plotting/_plotIonMap.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17340 2023-03-13 15:55:02.000000 nPYc-1.2.7/nPYc/plotting/_plotLOQFeatureViolin.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18942 2023-03-13 15:55:02.000000 nPYc-1.2.7/nPYc/plotting/_plotLOQRunOrder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5391 2023-03-13 15:55:02.000000 nPYc-1.2.7/nPYc/plotting/_plotNMRbaseline.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3631 2023-03-13 15:55:02.000000 nPYc-1.2.7/nPYc/plotting/_plotNMRcalibration.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4466 2023-03-13 15:55:02.000000 nPYc-1.2.7/nPYc/plotting/_plotNMRsolvent.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9075 2023-03-13 15:55:02.000000 nPYc-1.2.7/nPYc/plotting/_plotRSDs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8042 2023-03-13 15:55:02.000000 nPYc-1.2.7/nPYc/plotting/_plotSpectralVariance.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12005 2023-03-13 15:55:02.000000 nPYc-1.2.7/nPYc/plotting/_plotTIC.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3229 2023-03-13 15:55:02.000000 nPYc-1.2.7/nPYc/plotting/_plotTargeted.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3510 2023-03-13 15:55:02.000000 nPYc-1.2.7/nPYc/plotting/_plotTargetedFeatureDistribution.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9853 2023-03-13 15:55:02.000000 nPYc-1.2.7/nPYc/plotting/_plotVariableScatter.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17882 2023-03-13 15:55:02.000000 nPYc-1.2.7/nPYc/plotting/_plotting.py
+-rw-r--r--   0 runner    (1001) docker     (123)      875 2023-03-13 15:55:02.000000 nPYc-1.2.7/nPYc/plotting/_rangeFrameLocator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1671 2023-03-13 15:55:02.000000 nPYc-1.2.7/nPYc/plotting/_violinPlot.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-13 15:59:49.098905 nPYc-1.2.7/nPYc/reports/
+-rw-r--r--   0 runner    (1001) docker     (123)      794 2023-03-13 15:55:02.000000 nPYc-1.2.7/nPYc/reports/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20642 2023-03-13 15:55:02.000000 nPYc-1.2.7/nPYc/reports/_finalReportPeakPantheR.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3129 2023-03-13 15:55:02.000000 nPYc-1.2.7/nPYc/reports/_generateBasicPCAReport.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3070 2023-03-13 15:55:02.000000 nPYc-1.2.7/nPYc/reports/_generateFeatureDistributionReport.py
+-rw-r--r--   0 runner    (1001) docker     (123)    86395 2023-03-13 15:55:02.000000 nPYc-1.2.7/nPYc/reports/_generateReportMS.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14173 2023-03-13 15:55:02.000000 nPYc-1.2.7/nPYc/reports/_generateReportNMR.py
+-rw-r--r--   0 runner    (1001) docker     (123)    59107 2023-03-13 15:55:02.000000 nPYc-1.2.7/nPYc/reports/_generateReportTargeted.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10134 2023-03-13 15:55:02.000000 nPYc-1.2.7/nPYc/reports/_generateSampleReport.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20685 2023-03-13 15:55:02.000000 nPYc-1.2.7/nPYc/reports/featureID.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6569 2023-03-13 15:55:02.000000 nPYc-1.2.7/nPYc/reports/generateReport.py
+-rw-r--r--   0 runner    (1001) docker     (123)       73 2023-03-13 15:55:02.000000 nPYc-1.2.7/nPYc/reports/metadata.py
+-rw-r--r--   0 runner    (1001) docker     (123)    33781 2023-03-13 15:55:02.000000 nPYc-1.2.7/nPYc/reports/multivariateReport.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-13 15:59:49.102905 nPYc-1.2.7/nPYc/utilities/
+-rw-r--r--   0 runner    (1001) docker     (123)      531 2023-03-13 15:55:02.000000 nPYc-1.2.7/nPYc/utilities/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1230 2023-03-13 15:55:02.000000 nPYc-1.2.7/nPYc/utilities/_addReferenceRanges.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2920 2023-03-13 15:55:02.000000 nPYc-1.2.7/nPYc/utilities/_buildSpectrumFromQIfeature.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5309 2023-03-13 15:55:02.000000 nPYc-1.2.7/nPYc/utilities/_calibratePPMscale.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1172 2023-03-13 15:55:02.000000 nPYc-1.2.7/nPYc/utilities/_checkInRange.py
+-rw-r--r--   0 runner    (1001) docker     (123)      674 2023-03-13 15:55:02.000000 nPYc-1.2.7/nPYc/utilities/_conditionalJoin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1959 2023-03-13 15:55:02.000000 nPYc-1.2.7/nPYc/utilities/_filters.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13536 2023-03-13 15:55:02.000000 nPYc-1.2.7/nPYc/utilities/_fitPeak.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2949 2023-03-13 15:55:02.000000 nPYc-1.2.7/nPYc/utilities/_getMetadataFromBrukerNMR.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2017 2023-03-13 15:55:02.000000 nPYc-1.2.7/nPYc/utilities/_getMetadataFromWatersRaw.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2504 2023-03-13 15:55:02.000000 nPYc-1.2.7/nPYc/utilities/_getMetadataFrommzML.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6715 2023-03-13 15:55:02.000000 nPYc-1.2.7/nPYc/utilities/_importBrukerSpectrum.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2253 2023-03-13 15:55:02.000000 nPYc-1.2.7/nPYc/utilities/_internal.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1666 2023-03-13 15:55:02.000000 nPYc-1.2.7/nPYc/utilities/_lineWidth.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3816 2023-03-13 15:55:02.000000 nPYc-1.2.7/nPYc/utilities/_massSpectrumBuilder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3300 2023-03-13 15:55:02.000000 nPYc-1.2.7/nPYc/utilities/_nmr.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1494 2023-03-13 15:55:02.000000 nPYc-1.2.7/nPYc/utilities/_npc_sampleledger.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6295 2023-03-13 15:55:02.000000 nPYc-1.2.7/nPYc/utilities/_readBrukerXML.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     7347 2023-03-13 15:55:02.000000 nPYc-1.2.7/nPYc/utilities/extractParams.py
+-rw-r--r--   0 runner    (1001) docker     (123)      766 2023-03-13 15:55:02.000000 nPYc-1.2.7/nPYc/utilities/generic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5096 2023-03-13 15:55:02.000000 nPYc-1.2.7/nPYc/utilities/ms.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-13 15:59:49.102905 nPYc-1.2.7/nPYc/utilities/normalisation/
+-rw-r--r--   0 runner    (1001) docker     (123)      948 2023-03-13 15:55:02.000000 nPYc-1.2.7/nPYc/utilities/normalisation/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2916 2023-03-13 15:55:02.000000 nPYc-1.2.7/nPYc/utilities/normalisation/_normaliserABC.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1194 2023-03-13 15:55:02.000000 nPYc-1.2.7/nPYc/utilities/normalisation/_nullNormaliser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4175 2023-03-13 15:55:02.000000 nPYc-1.2.7/nPYc/utilities/normalisation/_probabilisticQuotientNormaliser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1930 2023-03-13 15:55:02.000000 nPYc-1.2.7/nPYc/utilities/normalisation/_totalAreaNormaliser.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-13 15:59:49.078905 nPYc-1.2.7/nPYc.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2218 2023-03-13 15:59:49.000000 nPYc-1.2.7/nPYc.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5538 2023-03-13 15:59:49.000000 nPYc-1.2.7/nPYc.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-13 15:59:49.000000 nPYc-1.2.7/nPYc.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-13 15:55:55.000000 nPYc-1.2.7/nPYc.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      249 2023-03-13 15:59:49.000000 nPYc-1.2.7/nPYc.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-03-13 15:59:49.000000 nPYc-1.2.7/nPYc.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-13 15:59:49.102905 nPYc-1.2.7/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2895 2023-03-13 15:55:02.000000 nPYc-1.2.7/setup.py
```

### Comparing `nPYc-1.2.6/LICENSE.md` & `nPYc-1.2.7/LICENSE.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 MIT License
 
-Copyright (c) 2021 National Phenome Centre
+Copyright (c) 2022 National Phenome Centre
 
 Permission is hereby granted, free of charge, to any person obtaining a copy
 of this software and associated documentation files (the "Software"), to deal
 in the Software without restriction, including without limitation the rights
 to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 copies of the Software, and to permit persons to whom the Software is
 furnished to do so, subject to the following conditions:
```

### Comparing `nPYc-1.2.6/PKG-INFO` & `nPYc-1.2.7/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,55 +1,58 @@
 Metadata-Version: 2.1
 Name: nPYc
-Version: 1.2.6
+Version: 1.2.7
 Summary: National Phenome Centre toolbox
 Home-page: https://github.com/phenomecentre/npyc-toolbox
 Author: National Phenome Centre
 Author-email: phenomecentre@imperial.ac.uk
 License: MIT
-Description: 		Toolbox for preprocessing of metabolic profiling datasets
-        		---------------------------------------------------------
-        
-        		.. image:: https://travis-ci.org/phenomecentre/nPYc-Toolbox.svg?branch=master
-        		   :target: https://travis-ci.org/phenomecentre/nPYc-Toolbox
-        		   :alt: Travis CI build status
-        
-        		.. image:: https://readthedocs.org/projects/npyc-toolbox/badge/?version=latest
-        		   :target: http://npyc-toolbox.readthedocs.io/en/latest/?badge=latest
-        		   :alt: Documentation Status
-        
-        		.. image:: https://codecov.io/gh/phenomecentre/nPYc-Toolbox/branch/master/graph/badge.svg
-        		   :target: https://codecov.io/gh/phenomecentre/nPYc-Toolbox
-        		   :alt: Test coverage
-        
-        		|
-        
-        		The nPYc toolbox offers functions for the import, preprocessing, and QC of metabolic profiling datasets.
-        
-        		Documentation can be found on `Read the Docs <http://npyc-toolbox.readthedocs.io/en/latest/?badge=latest>`_.
-        
-        		Imports
-        		 - Peak-picked LC-MS data (XCMS, Progenesis QI, *&* Metaboscape)
-        		 - Raw NMR spectra (Bruker format)
-        		 - Targeted datasets (TargetLynx, Bruker BI-LISA, *&* BI-Quant-Ur)
-        
-        		Provides
-        		 - Batch *&* drift correction for LC-MS datasets
-        		 - Feature filtering by RSD *&* linearity of response
-        		 - Calculation of spectral line-width in NMR
-        		 - PCA of datasets
-        		 - Visualisation of datasets
-        
-        		Exports
-        		 - Basic tabular csv
-        		 - `ISA-TAB <http://isa-tools.org>`_
-        
-        		The nPYc toolbox is `developed <https://github.com/phenomecentre/npyc-toolbox>`_ by the informatics team at `The National Phenome Centre <http://phenomecentre.org/>`_ at `Imperial College London <http://imperial.ac.uk/>`_.
-        		
 Platform: UNKNOWN
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Topic :: Scientific/Engineering :: Bio-Informatics
 Description-Content-Type: text/markdown
+License-File: LICENSE.md
+
+		Toolbox for preprocessing of metabolic profiling datasets
+		---------------------------------------------------------
+
+		.. image:: https://travis-ci.org/phenomecentre/nPYc-Toolbox.svg?branch=master
+		   :target: https://travis-ci.org/phenomecentre/nPYc-Toolbox
+		   :alt: Travis CI build status
+
+		.. image:: https://readthedocs.org/projects/npyc-toolbox/badge/?version=latest
+		   :target: http://npyc-toolbox.readthedocs.io/en/latest/?badge=latest
+		   :alt: Documentation Status
+
+		.. image:: https://codecov.io/gh/phenomecentre/nPYc-Toolbox/branch/master/graph/badge.svg
+		   :target: https://codecov.io/gh/phenomecentre/nPYc-Toolbox
+		   :alt: Test coverage
+
+		|
+
+		The nPYc toolbox offers functions for the import, preprocessing, and QC of metabolic profiling datasets.
+
+		Documentation can be found on `Read the Docs <http://npyc-toolbox.readthedocs.io/en/latest/?badge=latest>`_.
+
+		Imports
+		 - Peak-picked LC-MS data (XCMS, Progenesis QI, *&* Metaboscape)
+		 - Raw NMR spectra (Bruker format)
+		 - Targeted datasets (TargetLynx, Bruker BI-LISA, *&* BI-Quant-Ur)
+
+		Provides
+		 - Batch *&* drift correction for LC-MS datasets
+		 - Feature filtering by RSD *&* linearity of response
+		 - Calculation of spectral line-width in NMR
+		 - PCA of datasets
+		 - Visualisation of datasets
+
+		Exports
+		 - Basic tabular csv
+		 - `ISA-TAB <http://isa-tools.org>`_
+
+		The nPYc toolbox is `developed <https://github.com/phenomecentre/npyc-toolbox>`_ by the informatics team at `The National Phenome Centre <http://phenomecentre.org/>`_ at `Imperial College London <http://imperial.ac.uk/>`_.
+		
+
```

### Comparing `nPYc-1.2.6/README.md` & `nPYc-1.2.7/README.md`

 * *Files identical despite different names*

### Comparing `nPYc-1.2.6/nPYc/StudyDesigns/AssayParameters.json` & `nPYc-1.2.7/nPYc/StudyDesigns/AssayParameters.json`

 * *Files identical despite different names*

### Comparing `nPYc-1.2.6/nPYc/StudyDesigns/BI-LISA_analyteGroups.json` & `nPYc-1.2.7/nPYc/StudyDesigns/BI-LISA_analyteGroups.json`

 * *Files identical despite different names*

### Comparing `nPYc-1.2.6/nPYc/StudyDesigns/BI-LISA_reference_groups.json` & `nPYc-1.2.7/nPYc/StudyDesigns/BI-LISA_reference_groups.json`

 * *Files identical despite different names*

### Comparing `nPYc-1.2.6/nPYc/StudyDesigns/BI-LISA_reference_ranges.json` & `nPYc-1.2.7/nPYc/StudyDesigns/BI-LISA_reference_ranges.json`

 * *Files identical despite different names*

### Comparing `nPYc-1.2.6/nPYc/StudyDesigns/BI-LISAref.csv` & `nPYc-1.2.7/nPYc/StudyDesigns/BI-LISAref.csv`

 * *Files identical despite different names*

### Comparing `nPYc-1.2.6/nPYc/StudyDesigns/BlankISATAB/blank-ms/a_npc-test-study_metabolite_profiling_mass_spectrometry.txt` & `nPYc-1.2.7/nPYc/StudyDesigns/BlankISATAB/blank-ms/a_npc-test-study_metabolite_profiling_mass_spectrometry.txt`

 * *Files identical despite different names*

### Comparing `nPYc-1.2.6/nPYc/StudyDesigns/BlankISATAB/blank-ms/i_Investigation.txt` & `nPYc-1.2.7/nPYc/StudyDesigns/BlankISATAB/blank-ms/i_Investigation.txt`

 * *Files identical despite different names*

### Comparing `nPYc-1.2.6/nPYc/StudyDesigns/BlankISATAB/blank-nmr/a_npc-test-study_metabolite_profiling_NMR_spectroscopy.txt` & `nPYc-1.2.7/nPYc/StudyDesigns/BlankISATAB/blank-nmr/a_npc-test-study_metabolite_profiling_NMR_spectroscopy.txt`

 * *Files identical despite different names*

### Comparing `nPYc-1.2.6/nPYc/StudyDesigns/BlankISATAB/blank-nmr/i_Investigation.txt` & `nPYc-1.2.7/nPYc/StudyDesigns/BlankISATAB/blank-nmr/i_Investigation.txt`

 * *Files identical despite different names*

### Comparing `nPYc-1.2.6/nPYc/StudyDesigns/DilutionSeries.csv` & `nPYc-1.2.7/nPYc/StudyDesigns/DilutionSeries.csv`

 * *Files identical despite different names*

### Comparing `nPYc-1.2.6/nPYc/StudyDesigns/ExactMasses.csv` & `nPYc-1.2.7/nPYc/StudyDesigns/ExactMasses.csv`

 * *Files identical despite different names*

### Comparing `nPYc-1.2.6/nPYc/StudyDesigns/ISATABFieldMappings/MSFields.json` & `nPYc-1.2.7/nPYc/StudyDesigns/ISATABFieldMappings/MSFields.json`

 * *Files identical despite different names*

### Comparing `nPYc-1.2.6/nPYc/StudyDesigns/SOP/AminoAcidMS.json` & `nPYc-1.2.7/nPYc/StudyDesigns/SOP/AminoAcidMS.json`

 * *Files identical despite different names*

### Comparing `nPYc-1.2.6/nPYc/StudyDesigns/SOP/BrukerBI-LISA.json` & `nPYc-1.2.7/nPYc/StudyDesigns/SOP/BrukerBI-LISA.json`

 * *Files identical despite different names*

### Comparing `nPYc-1.2.6/nPYc/StudyDesigns/SOP/BrukerBI-QUANT-PS.json` & `nPYc-1.2.7/nPYc/StudyDesigns/SOP/BrukerBI-QUANT-PS.json`

 * *Files identical despite different names*

### Comparing `nPYc-1.2.6/nPYc/StudyDesigns/SOP/BrukerQuant-UR.json` & `nPYc-1.2.7/nPYc/StudyDesigns/SOP/BrukerQuant-UR.json`

 * *Files identical despite different names*

### Comparing `nPYc-1.2.6/nPYc/StudyDesigns/SOP/Generic.json` & `nPYc-1.2.7/nPYc/StudyDesigns/SOP/Generic.json`

 * *Files identical despite different names*

### Comparing `nPYc-1.2.6/nPYc/StudyDesigns/SOP/GenericMS.json` & `nPYc-1.2.7/nPYc/StudyDesigns/SOP/GenericMS.json`

 * *Files identical despite different names*

### Comparing `nPYc-1.2.6/nPYc/StudyDesigns/SOP/GenericNMRblood.json` & `nPYc-1.2.7/nPYc/StudyDesigns/SOP/GenericNMRblood.json`

 * *Files identical despite different names*

### Comparing `nPYc-1.2.6/nPYc/StudyDesigns/SOP/GenericNMRurine.json` & `nPYc-1.2.7/nPYc/StudyDesigns/SOP/GenericNMRurine.json`

 * *Files identical despite different names*

### Comparing `nPYc-1.2.6/nPYc/StudyDesigns/SOP/NMR1Djresblood.json` & `nPYc-1.2.7/nPYc/StudyDesigns/SOP/NMR1Djresblood.json`

 * *Files identical despite different names*

### Comparing `nPYc-1.2.6/nPYc/StudyDesigns/SOP/NMR1Djresurine.json` & `nPYc-1.2.7/nPYc/StudyDesigns/SOP/NMR1Djresurine.json`

 * *Files identical despite different names*

### Comparing `nPYc-1.2.6/nPYc/StudyDesigns/SOP/OxylipinMS.json` & `nPYc-1.2.7/nPYc/StudyDesigns/SOP/OxylipinMS.json`

 * *Files identical despite different names*

### Comparing `nPYc-1.2.6/nPYc/StudyDesigns/SOP/TryptophanMS.json` & `nPYc-1.2.7/nPYc/StudyDesigns/SOP/TryptophanMS.json`

 * *Files identical despite different names*

### Comparing `nPYc-1.2.6/nPYc/StudyDesigns/colours.json` & `nPYc-1.2.7/nPYc/StudyDesigns/colours.json`

 * *Files identical despite different names*

### Comparing `nPYc-1.2.6/nPYc/StudyDesigns/urine_quant_b_reference_groups.json` & `nPYc-1.2.7/nPYc/StudyDesigns/urine_quant_b_reference_groups.json`

 * *Files identical despite different names*

### Comparing `nPYc-1.2.6/nPYc/Templates/ID_request_MS.html` & `nPYc-1.2.7/nPYc/Templates/ID_request_MS.html`

 * *Files identical despite different names*

### Comparing `nPYc-1.2.6/nPYc/Templates/MS_BatchCorrectionAssessmentReport.html` & `nPYc-1.2.7/nPYc/Templates/MS_BatchCorrectionAssessmentReport.html`

 * *Files identical despite different names*

### Comparing `nPYc-1.2.6/nPYc/Templates/MS_BatchCorrectionSummaryReport.html` & `nPYc-1.2.7/nPYc/Templates/MS_BatchCorrectionSummaryReport.html`

 * *Files identical despite different names*

### Comparing `nPYc-1.2.6/nPYc/Templates/MS_CorrelationToDilutionReport.html` & `nPYc-1.2.7/nPYc/Templates/MS_CorrelationToDilutionReport.html`

 * *Files identical despite different names*

### Comparing `nPYc-1.2.6/nPYc/Templates/MS_FeatureSelectionReport.html` & `nPYc-1.2.7/nPYc/Templates/MS_FeatureSelectionReport.html`

 * *Files identical despite different names*

### Comparing `nPYc-1.2.6/nPYc/Templates/MS_FeatureSummaryReport.html` & `nPYc-1.2.7/nPYc/Templates/MS_FeatureSummaryReport.html`

 * *Files identical despite different names*

### Comparing `nPYc-1.2.6/nPYc/Templates/MS_FinalSummaryReport.html` & `nPYc-1.2.7/nPYc/Templates/MS_FinalSummaryReport.html`

 * *Files identical despite different names*

### Comparing `nPYc-1.2.6/nPYc/Templates/MS_FinalSummaryReport_Abridged.html` & `nPYc-1.2.7/nPYc/Templates/MS_FinalSummaryReport_Abridged.html`

 * *Files identical despite different names*

### Comparing `nPYc-1.2.6/nPYc/Templates/MS_peakPantheR_FinalSummaryReport.html` & `nPYc-1.2.7/nPYc/Templates/MS_peakPantheR_FinalSummaryReport.html`

 * *Files identical despite different names*

### Comparing `nPYc-1.2.6/nPYc/Templates/NMR_FinalSummaryReport.html` & `nPYc-1.2.7/nPYc/Templates/NMR_FinalSummaryReport.html`

 * *Files identical despite different names*

### Comparing `nPYc-1.2.6/nPYc/Templates/NMR_QCSummaryReport.html` & `nPYc-1.2.7/nPYc/Templates/NMR_QCSummaryReport.html`

 * *Files identical despite different names*

### Comparing `nPYc-1.2.6/nPYc/Templates/NPC_MultivariateReport.html` & `nPYc-1.2.7/nPYc/Templates/NPC_MultivariateReport.html`

 * *Files identical despite different names*

### Comparing `nPYc-1.2.6/nPYc/Templates/Targeted_FeatureSummaryReport.html` & `nPYc-1.2.7/nPYc/Templates/Targeted_FeatureSummaryReport.html`

 * *Files identical despite different names*

### Comparing `nPYc-1.2.6/nPYc/Templates/Targeted_FinalReportMS.html` & `nPYc-1.2.7/nPYc/Templates/Targeted_FinalReportMS.html`

 * *Files identical despite different names*

### Comparing `nPYc-1.2.6/nPYc/Templates/Targeted_FinalReportNMR.html` & `nPYc-1.2.7/nPYc/Templates/Targeted_FinalReportNMR.html`

 * *Files identical despite different names*

### Comparing `nPYc-1.2.6/nPYc/Templates/Targeted_MergeLOQReport.html` & `nPYc-1.2.7/nPYc/Templates/Targeted_MergeLOQReport.html`

 * *Files identical despite different names*

### Comparing `nPYc-1.2.6/nPYc/Templates/base_generic.html` & `nPYc-1.2.7/nPYc/Templates/base_generic.html`

 * *Files identical despite different names*

### Comparing `nPYc-1.2.6/nPYc/Templates/featureDistributionReport.html` & `nPYc-1.2.7/nPYc/Templates/featureDistributionReport.html`

 * *Files identical despite different names*

### Comparing `nPYc-1.2.6/nPYc/Templates/generateReportBILISA.html` & `nPYc-1.2.7/nPYc/Templates/generateReportBILISA.html`

 * *Files identical despite different names*

### Comparing `nPYc-1.2.6/nPYc/Templates/generateReportBIQuantUR.html` & `nPYc-1.2.7/nPYc/Templates/generateReportBIQuantUR.html`

 * *Files identical despite different names*

### Comparing `nPYc-1.2.6/nPYc/Templates/generateReportTargeted.html` & `nPYc-1.2.7/nPYc/Templates/generateReportTargeted.html`

 * *Files identical despite different names*

### Comparing `nPYc-1.2.6/nPYc/Templates/npc-main.css` & `nPYc-1.2.7/nPYc/Templates/npc-main.css`

 * *Files identical despite different names*

### Comparing `nPYc-1.2.6/nPYc/Templates/pcaReport.html` & `nPYc-1.2.7/nPYc/Templates/pcaReport.html`

 * *Files identical despite different names*

### Comparing `nPYc-1.2.6/nPYc/Templates/sampleReportChunk.html` & `nPYc-1.2.7/nPYc/Templates/sampleReportChunk.html`

 * *Files identical despite different names*

### Comparing `nPYc-1.2.6/nPYc/Templates/toolbox_logo.png` & `nPYc-1.2.7/nPYc/Templates/toolbox_logo.png`

 * *Files identical despite different names*

### Comparing `nPYc-1.2.6/nPYc/__init__.py` & `nPYc-1.2.7/nPYc/__init__.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,11 +1,13 @@
 """
 The `nPYc-Toolbox <https://github.com/phenomecentre/nPYc-Toolbox>`_ defines objects for representing, and implements functions to manipulate and display, metabolic profiling datasets.
 """
-__version__ = '1.2.6'
+
+__version__ = '1.2.7'
+
 
 from . import enumerations
 from .objects import Dataset, MSDataset, NMRDataset, TargetedDataset
 from . import utilities
 from . import plotting
 from . import reports
 from . import batchAndROCorrection
```

### Comparing `nPYc-1.2.6/nPYc/batchAndROCorrection/_batchAndROCorrection.py` & `nPYc-1.2.7/nPYc/batchAndROCorrection/_batchAndROCorrection.py`

 * *Files 8% similar despite different names*

```diff
@@ -14,53 +14,56 @@
 import sys
 import copy
 from datetime import datetime, timedelta
 from ..objects._msDataset import MSDataset
 from ..enumerations import AssayRole, SampleType
 
 
-def correctMSdataset(data, window=11, method='LOWESS', align='median', parallelise=True, excludeFailures=True):
+def correctMSdataset(data, window=11, method='LOWESS', align='median', parallelise=True, excludeFailures=True, correctionSampleType=SampleType.StudyPool):
 	"""
 	Conduct run-order correction and batch alignment on the :py:class:`~nPYc.objects.MSDataset` instance *data*, returning a new instance with corrected intensity values.
 
 	Sample are seperated into batches acording to the *'Correction Batch'* column in *data.sampleMetadata*.
 
 	:param data: MSDataset object with measurements to be corrected
 	:type data: MSDataset
 	:param int window: When calculating trends, consider this many reference samples, centred on the current position
 	:param str method: Correction method, one of 'LOWESS' (default), 'SavitzkyGolay' or None for no correction
 	:param str align: Average calculation of batch and feature intensity for correction, one of 'median' (default) or 'mean'
 	:param bool parallelise: If ``True``, use multiple cores
 	:param bool excludeFailures: If ``True``, remove features where a correct fit could not be calculated from the dataset
+	:param enum correctionSampleType: Which SampleType to use for the correction, default SampleType.StudyPool
 	:return: Duplicate of *data*, with run-order correction applied
 	:rtype: MSDataset
 	"""
 	import copy
 
 	# Check inputs
 	if not isinstance(data, MSDataset):
 		raise TypeError("data must be a MSDataset instance")
 	if not isinstance(window, int) & (window>0):
 		raise TypeError('window must be a positive integer')
 	if method is not None:
 		if not isinstance(method, str) & (method in {'LOWESS', 'SavitzkyGolay'}):
 			raise ValueError('method must be == LOWESS or SavitzkyGolay')
-	if not isinstance(align, str) & (align in {'mean', 'median'}):
-		raise ValueError('align must be == mean or median')
+	if not isinstance(align, str) & (align in {'mean', 'median', 'no'}):
+		raise ValueError('align must be == mean, median or no')
 	if not isinstance(parallelise, bool):
 		raise TypeError("parallelise must be a boolean")
 	if not isinstance(excludeFailures, bool):
 		raise TypeError("excludeFailures must be a boolean")
+	if not isinstance(correctionSampleType,SampleType):
+		raise TypeError("correctionType must be a SampleType")
 
 	with warnings.catch_warnings():
 		warnings.simplefilter('ignore', category=RuntimeWarning)
 
 		correctedP = _batchCorrectionHead(data.intensityData,
 									 data.sampleMetadata['Run Order'].values,
-									 (data.sampleMetadata['SampleType'].values == SampleType.StudyPool) & (data.sampleMetadata['AssayRole'].values == AssayRole.PrecisionReference),
+									 (data.sampleMetadata['SampleType'].values == correctionSampleType) & (data.sampleMetadata['AssayRole'].values == AssayRole.PrecisionReference),
 									 data.sampleMetadata['Correction Batch'].values,
 									 window=window,
 									 method=method,
 									 align=align,
 									 parallelise=parallelise)
 
 	correctedData = copy.deepcopy(data)
@@ -97,16 +100,16 @@
 	if not isinstance(batchList, numpy.ndarray):
 		raise TypeError('batchList must be a numpy array')
 	if not isinstance(window, int) & (window>0):
 		raise TypeError('window must be a positive integer')
 	if method is not None:
 		if not isinstance(method, str) & (method in {'LOWESS', 'SavitzkyGolay'}):
 			raise ValueError('method must be == LOWESS or SavitzkyGolay')	
-	if not isinstance(align, str) & (align in {'mean', 'median'}):
-			raise ValueError('align must be == mean or median')
+	if not isinstance(align, str) & (align in {'mean', 'median', 'no'}):
+			raise ValueError('align must be == mean, median or no')
 	if not isinstance(parallelise, bool):
 		raise TypeError('parallelise must be True or False')
 	if not isinstance(savePlots, bool):
 		raise TypeError('savePlots must be True or False')
 
 	# Store paramaters in a dict to avoid arg lists going out of control
 	parameters = dict()
@@ -201,16 +204,16 @@
 		batches = list(set(batchList))
 
 		# Get overall average intensity
 		if parameters['align'] == 'mean':
 			featureAverage = numpy.mean(feature[QCsamples])
 		elif parameters['align'] == 'median':
 			featureAverage = numpy.median(feature[QCsamples])
-		else:
-			return numpy.zeros_like(data)
+		#else:
+			#return numpy.zeros_like(data)
 				
 		# Iterate over batches.
 		for batch in batches:
 			# Skip the NaN batch
 			if not numpy.isnan(batch):
 
 				batchMask = numpy.squeeze(numpy.asarray(batchList == batch, 'bool'))
@@ -226,19 +229,19 @@
 																			parameters)
 
 				# Correct batch average to overall feature average
 				if parameters['align'] == 'mean':
 					batchMean = numpy.mean(feature[batchMask & QCsamples])
 				elif parameters['align'] == 'median':
 					batchMean = numpy.median(feature[batchMask & QCsamples])
-				else:
-					batchMean = numpy.nan_like(feature[batchMask])
-
-				feature[batchMask] = numpy.divide(feature[batchMask], batchMean)
-				feature[batchMask] = numpy.multiply(feature[batchMask], featureAverage)
+				#else:
+				#	batchMean = numpy.nan_like(feature[batchMask])
+				if parameters['align'] != 'no':
+					feature[batchMask] = numpy.divide(feature[batchMask], batchMean)
+					feature[batchMask] = numpy.multiply(feature[batchMask], featureAverage)
 				
 #				# If negative data mark for exclusion (occurs when too many QCsamples have intensity==0)
 #				if sum(feature[batchMask]<0) != 0:  # CJS 240816
 #					exclude = exclude + '; negativeData=' + str(sum(feature[batchMask]<0))
 
 #		results.append((i, feature, fit, exclude))  # CJS 240816
 		results.append((i, feature, fit))
@@ -254,33 +257,35 @@
 	# Break the QCs out of the dataset
 	QCdata = data[referenceSamples]
 	QCrunorder = runOrder[referenceSamples]
 
 	# Select model
 	# Optimisation of window would happen here.
 	window = parameters['window']
+	align = parameters['align']
 	if parameters['method'] == 'LOWESS':
 		(data, fit) = doLOESScorrection(QCdata, 
 										QCrunorder, 
 										data, 
-										runOrder, 
+										runOrder,
+										align=align,
 										window=window)
 	elif parameters['method'] == 'SavitzkyGolay':
 		(data, fit) = doSavitzkyGolayCorrection(QCdata, 
 												QCrunorder, 
 												data, 
 												runOrder, 
 												window=window)
 
 	# Potentially exclude features with poor fits that retuned NaN &c here.
 	
 	return (data, fit)
 
 
-def doLOESScorrection(QCdata, QCrunorder, data, runorder, window=11):
+def doLOESScorrection(QCdata, QCrunorder, data, runorder, align='median', window=11):
 	"""
 	Fit a LOWESS regression to the data.
 	"""
 	# Convert window number of samples to fraction of the dataset:
 	noSamples = QCrunorder.shape
 
 	if noSamples == 0:
@@ -297,17 +302,20 @@
 		# Divide by fit, then rescale to batch median
 		fit = numpy.interp(runorder, z[:,0], z[:,1])
 	
 		# Fit can go negative if too many adjacent QC samples == 0; set any negative fit values to zero
 		fit[fit < 0] = 0
 
 		corrected = numpy.divide(data, fit)
-		corrected = numpy.multiply(corrected, numpy.median(QCdata))
+		if align == 'median':
+			corrected = numpy.multiply(corrected, numpy.median(QCdata))
+		elif align == 'mean':
+			corrected = numpy.multiply(corrected, numpy.mean(QCdata))
 
-	return (corrected, fit)
+	return corrected, fit
 
 
 def doSavitzkyGolayCorrection(QCdata, QCrunorder, data, runorder, window=11, polyOrder=3):
 	"""
 	Fit a Savitzky-Golay curve to the data.
 	"""
 	# Sort the array
@@ -319,15 +327,15 @@
 	z = savgol_filter(QCdataSorted, window, polyOrder)
 
 	fit = numpy.interp(runorder, sortedRO2, z)
 
 	corrected = numpy.divide(data, fit)
 	corrected = numpy.multiply(corrected, numpy.median(QCdata))
 
-	return (corrected, fit)
+	return corrected, fit
 
 
 def optimiseCorrection(feature, optimise):
 	"""
 	Optimise the window function my mimising the output of `optimise(data)`
 	"""
 	pass
```

### Comparing `nPYc-1.2.6/nPYc/enumerations/__init__.py` & `nPYc-1.2.7/nPYc/enumerations/__init__.py`

 * *Files identical despite different names*

### Comparing `nPYc-1.2.6/nPYc/enumerations/_enumerations.py` & `nPYc-1.2.7/nPYc/enumerations/_enumerations.py`

 * *Files identical despite different names*

### Comparing `nPYc-1.2.6/nPYc/multivariate/__init__.py` & `nPYc-1.2.7/nPYc/multivariate/__init__.py`

 * *Files identical despite different names*

### Comparing `nPYc-1.2.6/nPYc/multivariate/exploratoryAnalysisPCA.py` & `nPYc-1.2.7/nPYc/multivariate/exploratoryAnalysisPCA.py`

 * *Files identical despite different names*

### Comparing `nPYc-1.2.6/nPYc/multivariate/multivariateUtilities.py` & `nPYc-1.2.7/nPYc/multivariate/multivariateUtilities.py`

 * *Files identical despite different names*

### Comparing `nPYc-1.2.6/nPYc/objects/_dataset.py` & `nPYc-1.2.7/nPYc/objects/_dataset.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 import scipy
 import numpy
 import pandas
 import os
-import isatools.isatab as isatab
 import json
 import inspect
 import re
 from ..enumerations import VariableType, DatasetLevel, SampleType, AssayRole
 from ..utilities.generic import removeDuplicateColumns
 from .._toolboxPath import toolboxPath
 from datetime import datetime
@@ -1119,15 +1118,14 @@
 		Load additional metadata and map it in to the :py:attr:`sampleMetadata` table.
 
 		Possible options:
 
 		* **'Basic CSV'** Joins the :py:attr:`sampleMetadata` table with the data in the ``csv`` file at *filePath=*, matching on the 'Sample File Name' column in both (see :doc:`samplemetadata`).
 		* **'Filenames'** Parses sample information out of the filenames, based on the named capture groups in the regex passed in *filenamespec*
 		* **'Raw Data'** Extract analytical parameters from raw data files
-		* **'ISATAB'** ISATAB study designs
 
 		:param str descriptionFormat: Format of metadata to be added
 		:param str filePath: Path to the additional data to be added
 		:raises NotImplementedError: if the descriptionFormat is not understood
 		"""
 
 		"""
@@ -1139,16 +1137,14 @@
 			self._matchBasicCSV(filePath)
 		elif descriptionFormat == 'NPC LIMS':
 			self._matchDatasetToLIMS(filePath)
 		elif descriptionFormat == 'NPC Subject Info':
 			self._matchDatasetToSubjectInfo(filePath)
 		elif descriptionFormat == 'Raw Data':
 			self._getSampleMetadataFromRawData(filePath, filetype)
-		elif descriptionFormat == 'ISATAB':
-			self._matchDatasetToISATAB(filePath, **kwargs)
 		elif descriptionFormat == 'Filenames':
 			self._getSampleMetadataFromFilename(kwargs['filenameSpec'])
 		else:
 			raise NotImplementedError
 
 	def addFeatureInfo(self, filePath=None, descriptionFormat=None, featureId=None, **kwargs):
 		"""
@@ -1613,270 +1609,14 @@
 		if 'SampleType' in sampleMetadata.columns:
 			for stype in SampleType:
 				sampleMetadata.loc[sampleMetadata['SampleType'].values == str(stype), 'SampleType'] = stype
 
 		return (objectName, intensityData, featureMetadata, sampleMetadata)
 
 
-	def _matchDatasetToISATAB(self, pathToISATABFile, filenameSpec=None, studyID = 1, assayID=1, assay='MS'):
-		"""
-		Match the Sample IDs in :py:attr:`sampleMetadata` to the subject and assay information in the ISATAB File.
-
-		The column *Sampling ID* in :py:attr:`sampleMetadata` is matched to *Sample Name* in the *ISATAB Study* sheet
-
-		:param str pathToISATABFile: path to the ISATAB File
-		:param int studyID: the Study index in the ISATAB File
-		:param int assayID: the Assay index in the ISATAB File
-		:param str assay: the assay type 'MS' or 'NMR'
-		"""
-
-
-		#if 'Dilution' in self.sampleMetadata.columns:
-		#	self.sampleMetadata.drop(['Dilution'], axis=1, inplace=True)
-
-		if not (assay in ['MS','NMR']):
-			raise ValueError('assay should be either \'MS\' or \'NMR\'')
-
-		# Load ISATAB file
-		with open(os.path.join(pathToISATABFile,'i_Investigation.txt')) as fp:
-			isa_tab_record = isatab.load(fp)
-
-		# subject info === study
-		# limsFile info === assay
-		study1 = isa_tab_record.studies[studyID - 1]  # get the 1st study
-		study_filename = study1.filename
-		subjectInfo = pandas.read_csv(os.path.join(pathToISATABFile, study_filename), sep='\t')
-		# We're only interested in these fields so keep them
-		subjectInfo = subjectInfo[
-			['Source Name', 'Characteristics[age]', 'Characteristics[gender]', 'Date', 'Comment[study name]',
-			 'Characteristics[organism]', 'Characteristics[material role]', 'Characteristics[material type]',
-			 'Sample Name']]
-		# rename Characteristics[material role] to Status
-		subjectInfo.rename(columns={'Characteristics[material role]': 'Status'}, inplace=True)
-		# rename these fields to something similar to excel sheet
-		subjectInfo.rename(columns={'Source Name': 'Subject ID'}, inplace=True)
-		subjectInfo.rename(columns={'Characteristics[age]': 'Age'}, inplace=True)
-		subjectInfo.rename(columns={'Characteristics[gender]': 'Gender'}, inplace=True)
-		subjectInfo.rename(columns={'Date': 'Sampling Date'}, inplace=True)
-		subjectInfo.rename(columns={'Characteristics[organism]': 'Organism'}, inplace=True)
-		subjectInfo.rename(columns={'Characteristics[material type]': 'Material Type'}, inplace=True)
-		subjectInfo.rename(columns={'Comment[study name]': 'Study'}, inplace=True)
-		# subjectInfo.rename(columns={'Characteristics[dilution factor]': 'Dilution'}, inplace=True)
-		# Enforce string type on Subject ID and Sampling ID columns
-		subjectInfo['Subject ID'] = subjectInfo['Subject ID'].astype('str')
-		subjectInfo['Sample Name'] = subjectInfo['Sample Name'].astype('str')
-
-		assay1 = study1.assays[assayID - 1]  # get the assay
-		assay_filename = assay1.filename
-		# Read in ISATAB file
-		# The reason it's called limsFile is because this object is used in other modules such as reports
-		limsFile = pandas.read_csv(os.path.join(pathToISATABFile, assay_filename), sep='\t')
-
-		if not self.__validateColumns(limsFile, assay):
-			warnings.warn("One or more required fields are missing in your Assay table, results maybe unreliable!")
-
-		# rename Sample Name column to Sampling ID
-		if any(limsFile.columns.str.match('Sample Name')):
-			limsFile.rename(columns={'Sample Name': 'Sampling ID'}, inplace=True)
-
-
-		#rename fields according to assay type
-		if assay == 'NMR':
-			with open(os.path.join(toolboxPath(), 'StudyDesigns', 'ISATABFieldMappings','NMRFields.json')) as data_file:
-				nmrFieldDict = json.load(data_file)
-				limsFile.rename(columns = nmrFieldDict, inplace=True)
-				self.Attributes['Log'].append([datetime.now(), 'NMR Assay field names have been mapped into NPC field names' ])
-		else:
-			with open(os.path.join(toolboxPath(), 'StudyDesigns', 'ISATABFieldMappings','MSFields.json')) as data_file:
-				msFieldDict = json.load(data_file)
-				limsFile.rename(columns=msFieldDict, inplace=True)
-				self.Attributes['Log'].append([datetime.now(), 'MS Assay field names have been mapped into NPC field names' ])
-
-		#remove fields inserted by ISATAB and only keep the fields we're interested in
-		if assay == 'MS':
-			limsFile = limsFile[['Sampling ID','Assay data name','Dilution','Run Order','Acquisition Date','Acquisition Time','Instrument','Chromatography','Ionisation','Batch','Sample batch','Plate','Well','Correction Batch','Detector']]
-		else:
-			limsFile = limsFile[['Sampling ID','Assay data name','Run Order','Acquisition Date','Acquisition Time','Instrument','Batch','Sample batch']]
-
-
-		#self.Attributes['DataPath'] = limsFile['Data Path'][0]
-
-		#merge the two fields 'Acquisition Date','Acquisition Time' into one field 'Acquired Time'
-		#a few lines down we make sure 'Acquired Time' is a proper date/time field that pandas is happy with!
-		limsFile['Acquired Time'] = limsFile[['Acquisition Date', 'Acquisition Time']].apply(lambda x: ' '.join(x), axis=1)
-		limsFile.drop(['Acquisition Date', 'Acquisition Time'], axis=1, inplace=True)
-		self.Attributes['Log'].append([datetime.now(), '\'Acquisition Date\', \'Acquisition Time\' read from ISATAB have been merged into \'Acquired Time\' and removed' ])
-
-		# retrieve the material role or Sample Type or Status of each sample in the assay
-		# one way to do this is by merging the assay and study based on sample name!
-		self.limsFile = pandas.merge(limsFile, subjectInfo, left_on='Sampling ID', right_on='Sample Name')
-		# Remove duplicate columns (these will be appended with _x or _y)
-		self.limsFile = removeDuplicateColumns(self.limsFile)
-
-		# this is becuase when NMR metadata is read from raw data, it already contains a field 'Acquired Time'
-		# remove this field so we don't confuse it with the one read from isatab
-		# Log it!
-		if any(self.sampleMetadata.columns.str.match('Acquired Time')):
-			self.sampleMetadata.drop('Acquired Time', axis=1, inplace=True)
-			self.Attributes['Log'].append(
-				[datetime.now(), 'Acquired Time has been read from ISATAB instead of raw data'])
-
-		# this is becuase when NMR metadata is read from raw data, it already contains a field 'Run Order'
-		# remove this field so we don't confuse it with the one read from isatab
-		if any(self.sampleMetadata.columns.str.match('Run Order')):
-			self.sampleMetadata.drop('Run Order', axis=1, inplace=True)
-			self.Attributes['Log'].append([datetime.now(), 'Run Order has been read from ISATAB instead of raw data'])
-
-		# Prepare data
-		self.sampleMetadata.loc[:, 'Sample Base Name'] = self.sampleMetadata['Sample File Name']
-		self.sampleMetadata.loc[:, 'Sample Base Name Normalised'] = self.sampleMetadata['Sample Base Name'].str.lower()
-
-		# Enforce string type on 'Sampling ID'
-		sampleIDmask = pandas.isnull(self.limsFile['Sampling ID']) == False
-		self.limsFile.loc[sampleIDmask, 'Sampling ID'] = self.limsFile.loc[sampleIDmask, 'Sampling ID'].astype('str')
-		self.limsFile.loc[:, 'Assay data name Normalised'] = self.limsFile['Assay data name'].str.lower()
-
-		# Match limsFile to sampleMetdata for samples with data PRESENT
-		self.sampleMetadata = pandas.merge(self.limsFile,self.sampleMetadata, left_on='Assay data name Normalised', right_on='Sample Base Name Normalised', how='right', sort=False)
-		self.sampleMetadata = removeDuplicateColumns(self.sampleMetadata)
-		#
-		if 'Exclusion Details' not in self.sampleMetadata:
-			self.sampleMetadata['Exclusion Details'] = ''
-
-		# Complete/create set of boolean columns describing the data in each row for sampleMetadata
-		#self.sampleMetadata.loc[:,'Study Sample'] = self.sampleMetadata['Sampling ID'].notnull().astype(bool)
-		self.sampleMetadata.loc[:,'Study Sample'] = self.sampleMetadata['Status'].str.match('Sample', na=False).astype(bool)
-		self.sampleMetadata.loc[:,'Long-Term Reference'] = self.sampleMetadata['Status'].str.match('Long Term Reference', na=False).astype(bool)
-		self.sampleMetadata.loc[:,'Study Reference'] = self.sampleMetadata['Status'].str.match('Study Reference', na=False).astype(bool)
-		self.sampleMetadata.loc[:,'Method Reference'] = self.sampleMetadata['Status'].str.match('Method Reference', na=False).astype(bool)
-		self.sampleMetadata.loc[:,'Dilution Series'] = self.sampleMetadata['Status'].str.match('Dilution Series', na=False).astype(bool)
-		#why is this repeated?
-		#self.sampleMetadata.loc[:,'Study Sample'] = self.sampleMetadata['Study Sample'].where((self.sampleMetadata['Long-Term Reference'] | self.sampleMetadata['Study Reference']) == False, other=False)
-		self.sampleMetadata.loc[:,'LIMS Marked Missing'] = self.sampleMetadata['Status'].str.match('Missing', na=False).astype(bool)
-
-		# Complete/create set of boolean columns describing the data in each row for sampleMetadata
-		self.sampleMetadata.loc[:,'Data Present'] = self.sampleMetadata['Sample File Name'].str.match('.+', na=False)
-		self.sampleMetadata.loc[:,'LIMS Present'] = self.sampleMetadata['Assay data name'].str.match('.+', na=False, case=False)
-		self.sampleMetadata.loc[:,'LIMS Marked Missing'] = self.sampleMetadata['Status'].str.match('Missing', na=False)
-		self.sampleMetadata['Study Sample'].where((self.sampleMetadata['Study Sample'] & (self.sampleMetadata['LIMS Present'] == False)) == False, False, inplace=True)
-		#check with Jake/Caroline
-		self.sampleMetadata['Skipped'] = None
-
-		# Explicity convert datetime format
-		self.sampleMetadata['Acquired Time'] = self.sampleMetadata['Acquired Time'].apply(pandas.to_datetime,dayfirst=True)
-		self.sampleMetadata['Acquired Time'] = self.sampleMetadata['Acquired Time']
-
-		#automatically mark samples that have no 'Acquired Time' for exclusion
-		if sum(self.sampleMetadata['Acquired Time'].isnull()) > 0:
-			self.excludeSamples(self.sampleMetadata[self.sampleMetadata['Acquired Time'].notnull()==False]['Sample File Name'], on='Sample File Name', message='Acquired time missing')
-			self.Attributes['Log'].append([datetime.now(), 'One or more samples have been marked for exclusion because their Acquisition Date/Time values are missing'])
-			warnings.warn('One or more samples have been marked for exclusion because their Acquisition Date/Time values are missing!')
-
-		##
-		# If AssayRole or SampleType columns are present parse strings into enums
-		##
-		"""
-		self.sampleMetadata['AssayRole'] = AssayRole.Assay
-		if 'AssayRole' in self.sampleMetadata.columns:
-			for role in AssayRole:
-				self.sampleMetadata.loc[self.sampleMetadata['AssayRole'].values == role.name, 'AssayRole'] = role
-
-		self.sampleMetadata['SampleType'] = SampleType.StudySample
-		if 'SampleType' in self.sampleMetadata.columns:
-			for stype in SampleType:
-				self.sampleMetadata.loc[self.sampleMetadata['SampleType'].values == stype.name, 'SampleType'] = stype
-		"""
-		self.sampleMetadata['AssayRole'] = AssayRole.Assay
-		self.sampleMetadata.loc[self.sampleMetadata['Study Reference'].values, 'AssayRole'] = AssayRole.PrecisionReference
-		#self.sampleMetadata.loc[self.sampleMetadata['Batch Termini'].values, 'AssayRole'] = AssayRole.PrecisionReference
-		self.sampleMetadata.loc[self.sampleMetadata['Long-Term Reference'].values, 'AssayRole'] = AssayRole.PrecisionReference
-		self.sampleMetadata.loc[self.sampleMetadata['Method Reference'].values, 'AssayRole'] = AssayRole.PrecisionReference
-		self.sampleMetadata.loc[self.sampleMetadata['Dilution Series'].values, 'AssayRole'] = AssayRole.LinearityReference
-
-		self.sampleMetadata['SampleType'] = SampleType.StudySample
-		self.sampleMetadata.loc[self.sampleMetadata['Study Reference'].values, 'SampleType'] = SampleType.StudyPool
-		#self.sampleMetadata.loc[self.sampleMetadata['Batch Termini'].values, 'SampleType'] = SampleType.StudyPool
-		self.sampleMetadata.loc[self.sampleMetadata['Long-Term Reference'].values, 'SampleType'] = SampleType.ExternalReference
-		self.sampleMetadata.loc[self.sampleMetadata['Method Reference'].values, 'SampleType'] = SampleType.MethodReference
-		self.sampleMetadata.loc[self.sampleMetadata['Dilution Series'].values, 'SampleType'] = SampleType.StudyPool
-
-		# Remove duplicate columns (these will be appended with _x or _y)
-		self.sampleMetadata = removeDuplicateColumns(self.sampleMetadata)
-
-		# Find samples present in LIMS but not acquired - replace the deepcopy from python with pandas, to avoid error
-		# when the dataframe is empty
-		lims_butnotacq = self.limsFile.loc[self.limsFile['Assay data name Normalised'].isin(self.sampleMetadata['Sample Base Name Normalised'])==False,:]
-		self.sampleAbsentMetadata = lims_butnotacq.copy(deep=True)
-
-		# Complete/create set of boolean columns describing the data in each row for sampleAbsentMetadata
-		self.sampleAbsentMetadata.loc[:,'Study Sample'] = self.sampleAbsentMetadata['Status'].str.match('Sample', na=False).astype(bool)
-		self.sampleAbsentMetadata.loc[:,'Long-Term Reference'] = self.sampleAbsentMetadata['Status'].str.match('Long Term Reference', na=False).astype(bool)
-		self.sampleAbsentMetadata.loc[:,'Study Reference'] = self.sampleAbsentMetadata['Status'].str.match('Study Reference', na=False).astype(bool)
-		self.sampleAbsentMetadata.loc[:,'Method Reference'] = self.sampleAbsentMetadata['Status'].str.match('Method Reference', na=False).astype(bool)
-		self.sampleAbsentMetadata.loc[:,'Dilution Series'] = self.sampleAbsentMetadata['Status'].str.match('Dilution Series', na=False).astype(bool)
-		self.sampleAbsentMetadata.loc[:,'LIMS Marked Missing'] = self.sampleAbsentMetadata['Status'].str.match('Missing', na=False).astype(bool)
-
-		# Remove duplicate columns (these will be appended with _x or _y)
-		#self.sampleAbsentMetadata = removeDuplicateColumns(self.sampleAbsentMetadata)
-
-		#This should be done in a better way
-		self.sampleAbsentMetadata['AssayRole'] = AssayRole.Assay
-		self.sampleAbsentMetadata.loc[self.sampleAbsentMetadata['Study Reference'].values, 'AssayRole'] = AssayRole.PrecisionReference
-		#self.sampleMetadata.loc[self.sampleMetadata['Batch Termini'].values, 'AssayRole'] = AssayRole.PrecisionReference
-		self.sampleAbsentMetadata.loc[self.sampleAbsentMetadata['Long-Term Reference'].values, 'AssayRole'] = AssayRole.PrecisionReference
-		self.sampleAbsentMetadata.loc[self.sampleAbsentMetadata['Method Reference'].values, 'AssayRole'] = AssayRole.PrecisionReference
-		self.sampleAbsentMetadata.loc[self.sampleAbsentMetadata['Dilution Series'].values, 'AssayRole'] = AssayRole.LinearityReference
-
-
-		self.sampleAbsentMetadata['SampleType'] = SampleType.StudySample
-		self.sampleAbsentMetadata.loc[self.sampleAbsentMetadata['Study Reference'].values, 'SampleType'] = SampleType.StudyPool
-		#self.sampleMetadata.loc[self.sampleMetadata['Batch Termini'].values, 'SampleType'] = SampleType.StudyPool
-		self.sampleAbsentMetadata.loc[self.sampleAbsentMetadata['Long-Term Reference'].values, 'SampleType'] = SampleType.ExternalReference
-		self.sampleAbsentMetadata.loc[self.sampleAbsentMetadata['Method Reference'].values, 'SampleType'] = SampleType.MethodReference
-		self.sampleAbsentMetadata.loc[self.sampleAbsentMetadata['Dilution Series'].values, 'SampleType'] = SampleType.StudyPool
-
-		# Save biological parameters (for multivariate QC)
-		self.Attributes['Analytical Measurements'] = self.sampleMetadata.columns
-		self.Attributes['Log'].append([datetime.now(), 'ISATAB sample IDs matched from %s' % (pathToISATABFile)])
-
-		# subject info === study
-		# limsFile info === assay
-
-		# Create one overall samplingInfo sheet - combine subjectInfo and samplingEvents for samples present in samplingEvents
-		self.samplingInfo = pandas.merge(self.limsFile, subjectInfo, left_on='Sampling ID', right_on='Sample Name', how='left', sort=False)
-
-		# Remove duplicate columns (these will be appended with _x or _y)
-		self.samplingInfo = removeDuplicateColumns(self.samplingInfo)
-
-		# make sure these fields are of type string
-		self.samplingInfo['Subject ID'] = self.samplingInfo['Subject ID'].astype('str')
-		self.samplingInfo['Sample Name'] = self.samplingInfo['Sample Name'].astype('str')
-
-		self.sampleAbsentMetadata['SubjectInfoData'] = False
-		self.sampleAbsentMetadata.loc[self.sampleAbsentMetadata['Subject ID'].notnull(), 'SubjectInfoData'] = True
-
-
-		self.sampleMetadata['SubjectInfoData'] = False
-		self.sampleMetadata.loc[self.sampleMetadata['Subject ID'].notnull(), 'SubjectInfoData'] = True
-
-		"""
-		# Find subjects present in sampleInfo only
-		self.samplingInfo['inLIMS'] = False
-		tempP = [ numpy.sum(a == self.sampleMetadata['Sampling ID'] ) for a in self.samplingInfo['Sampling ID']]
-		tempA = [ numpy.sum(a == self.sampleAbsentMetadata['Sampling ID'] ) for a in self.samplingInfo['Sampling ID']]
-		for t in range(self.samplingInfo.shape[0]):
-				if ((tempP[t] != 0) | (tempA[t] != 0)):
-						self.samplingInfo.loc[t,'inLIMS'] = True
-		self.subjectAbsentMetadata = self.samplingInfo[self.samplingInfo['inLIMS']==False]
-
-		# Save biological parameters (for multivariate QC)
-		self.Attributes['Biological Measurements'] = self.samplingInfo.columns.drop('inLIMS')
-		"""
-		self.Attributes['Biological Measurements'] = self.samplingInfo.columns
-		self.Attributes['Log'].append([datetime.now(), 'Subject information matched from ISATAB %s' % (pathToISATABFile)])
 
 
 	def excludeSamples(self, sampleList, on='Sample File Name', message='User Excluded'):
 		"""
 		Sets the :py:attr:`sampleMask` for the samples listed in *sampleList* to ``False`` to mask them from the dataset.
 
 		:param list sampleList: A list of sample IDs to be excluded
@@ -1966,47 +1706,28 @@
 
 		else:
 			raise ValueError('Unknown VariableType.')
 
 		return notFound
 
 
-	def exportDataset(self, destinationPath='.', saveFormat='CSV', isaDetailsDict = {}, withExclusions=True, escapeDelimiters=False, filterMetadata=True):
+	def exportDataset(self, destinationPath='.', saveFormat='CSV', withExclusions=True, escapeDelimiters=False, filterMetadata=True):
 		"""
 		Export dataset object in a variety of formats for import in other software, the export is named according to the :py:attr:`name` attribute of the Dataset object.
 
 		Possible save formats are:
 
 		* **CSV** Basic CSV output, :py:attr:`featureMetadata`, :py:attr:`sampleMetadata` and :py:attr:`intensityData` are written to three separate CSV files in *desitinationPath*
 		* **UnifiedCSV** Exports :py:attr:`featureMetadata`, :py:attr:`sampleMetadata` and :py:attr:`intensityData` concatenated into a single CSV file
-		* **ISATAB** Exports the sampleMetadata in the `ISATAB <http://isa-tools.org>`_ format
 
 		:param str destinationPath: Save data into the directory specified here
 		:param str format: File format for saved data, defaults to CSV.
-		:param dict detailsDict: Contains several key: value pairs required to for exporting ISATAB.
 
-		detailsDict should have the format:
-		detailsDict = {
-			'investigation_identifier' : "i1",
-			'investigation_title' : "Give it a title",
-			'investigation_description' : "Add a description",
-			'investigation_submission_date' : "2016-11-03",
-			'investigation_public_release_date' : "2016-11-03",
-			'first_name' : "Noureddin",
-			'last_name' : "Sadawi",
-			'affiliation' : "University",
-			'study_filename' : "my_ms_study",
-			'study_material_type' : "Serum",
-			'study_identifier' : "s1",
-			'study_title' : "Give the study a title",
-			'study_description' : "Add study description",
-			'study_submission_date' : "2016-11-03",
-			'study_public_release_date' : "2016-11-03",
-			'assay_filename' : "my_ms_assay"
-		}
+
+
 
 		:param bool withExclusions: If ``True`` mask features and samples will be excluded
 		:param bool escapeDelimiters: If ``True`` remove characters commonly used as delimiters in csv files from metadata
 		:param bool filterMetadata: If ``True`` does not export the sampleMetadata and featureMetadata columns listed in self.Attributes['sampleMetadataNotExported'] and self.Attributes['featureMetadataNotExported']
 		:raises ValueError: if *saveFormat* is not understood
 		"""
 		# Validate inputs
@@ -2042,16 +1763,14 @@
 
 		if saveFormat == 'CSV':
 			destinationPath = os.path.join(destinationPath, exportDataset.name)
 			exportDataset._exportCSV(destinationPath, escapeDelimiters=escapeDelimiters)
 		elif saveFormat == 'UnifiedCSV':
 			destinationPath = os.path.join(destinationPath, exportDataset.name)
 			exportDataset._exportUnifiedCSV(destinationPath, escapeDelimiters=escapeDelimiters)
-		elif saveFormat == 'ISATAB':
-			exportDataset._exportISATAB(destinationPath, isaDetailsDict)
 		else:
 			raise ValueError('Save format \'%s\' not understood.' % saveFormat)
 
 		self.Attributes['Log'].append([datetime.now(), "%s format export made to %s\n" % (saveFormat, self.saveDir)])
 
 
 	def _exportCSV(self, destinationPath, escapeDelimiters=False):
@@ -2095,24 +1814,14 @@
 							   encoding='utf-8')
 
 		# Export intensity data
 		numpy.savetxt(destinationPath + '_intensityData.csv',
 					  self.intensityData, delimiter=",")
 
 
-	def _exportISATAB(self, destinationPath, isaDetailsDict, assay='MS'):
-		"""
-		Export the dataset's metadata to the directory *destinationPath* as ISATAB
-
-		:param str destinationPath: Path to a directory in which the output will be saved
-		:param bool escapeDelimiters: Remove characters commonly used as delimiters in csv files from metadata
-		:raises IOError: If writing one of the files fails
-		"""
-		raise NotImplementedError
-
 
 	def _exportUnifiedCSV(self, destinationPath, escapeDelimiters=True):
 		"""
 		Export the dataset to the directory *destinationPath* as a combined CSV file containing intensity data, and feature and sample metadata
 			*destinationPath*_combinedData.csv.csv
 
 		:param str destinationPath: Path to a directory in which the output will be saved
```

### Comparing `nPYc-1.2.6/nPYc/objects/_msDataset.py` & `nPYc-1.2.7/nPYc/objects/_msDataset.py`

 * *Files 5% similar despite different names*

```diff
@@ -33,18 +33,36 @@
 
 	Objects can be initialised from a variety of common data formats, currently peak-picked data from Progenesis QI or XCMS, and targeted Biocrates datasets.
 
 	* Progenesis QI
 		QI import operates on csv files exported *via* the 'Export Compound Measurements' menu option in QI. Import requires the presence of both normalised and raw datasets, but will only import the raw meaturenents.
 
 	* XCMS
-		XCMS import operates on the csv files generated by XCMS with the peakTable() method. By default, the csv is expected to have 14 columns of feature parameters, with the intensity values for the first sample coming on the 15 column. However, the number of columns to skip is dataset dependent and can be set with the (e ``noFeatureParams=`` keyword argument.
+		XCMS import operates on the csv files generated by XCMS with the peakTable() method. By default, the csv is expected to have 14 columns of feature parameters, with the intensity values for the first sample coming on the 15 column. However, the number of columns to skip is dataset dependent and can be set with the ``noFeatureParams=`` keyword argument.
+		This method assumes that the retention time value in the XCMS exported peak list is specified in seconds.
+
+	* XCMSOnline
+		XCMS Online download output supplies an unannotated and an annotated xlsx file stored by default in "XCMS results" folder.
+		By default, the table is expected to have 10 columns of feature parameters, with the intensity values for the first sample coming on the 11th column.
+		However, the number of columns to skip is dataset dependent and can be set with the (e ``noFeatureParams=`` keyword argument.
+
+	* MZmine
+		MZmine2: import operates on csv files exported via the 'Export to CSV' file' menu option. Field separator should be comma "," and all export elements should be chosen for export.
+		MZmine3: choose 'Export feature list' -> 'CSV (legacy MZmine 2)' menu option. Field separator should be comma "," and all export elements should be chosen for export.
+
+	* MS-DIAL
+		MS-DIAL import operates on the .txt (MSP) files exported via the 'Export -> Alignment result' menu option. Export options to choose are preferably 'Raw data matrix (Area)' or 'Raw data matrix (Height)'.
+		This method will also import the accompanying experimental metadata information such as File Type, Injection Order and Batch ID.
 
 	* Biocrates
 		Operates on spreadsheets exported from Biocrates MetIDQ. By default loads data from the sheet named 'Data Export', this may be overridden with the ``sheetName=`` argument, If the number of sample metadata columns differes from the default, this can be overridden with the ``noSampleParams=`` argument.
+
+	* nPYc
+		nPYc import operates on the csv file generated using nPYc exportDataset function ('combinedData' file). This reimport function is meant for further filtering or normalisation without having to run whole process again.
+		Note that metadata does not need to be imported again.
 	"""
 
 	def __init__(self, datapath, fileType='xcms', sop='GenericMS', **kwargs):
 		"""
 		Basic initialisation.
 		"""
 
@@ -69,39 +87,58 @@
 											 'correlationToDilutionFilter': False,
 											 'artifactualFilter': False, 'blankFilter': False}
 		self.Attributes['filterParameters'] = {'rsdThreshold': None, 'corrMethod': None, 'corrThreshold': None,
 											   'varianceRatio': None, 'blankThreshold': None,
 											   'overlapThresholdArtifactual': None, 'corrThresholdArtifactual': None,
 											   'deltaMzArtifactual': None}
 
-		# Load the QI output file
+		# Load the output file
 		fileType = fileType.lower()
 		if fileType == 'qi':
 			self._loadQIDataset(datapath)
 			self.Attributes['FeatureExtractionSoftware'] = 'Progenesis QI'
 			self.VariableType = VariableType.Discrete
+		elif fileType == 'mzmine':
+			self._loadMZmineDataset(datapath)
+			self.Attributes['FeatureExtractionSoftware'] = 'MZmine'
+			self.VariableType = VariableType.Discrete
+		elif fileType == 'msdial':
+			self._loadMSDIALDataset(datapath)
+			self.Attributes['FeatureExtractionSoftware'] = 'MS-DIAL'
+			self.VariableType = VariableType.Discrete
 		elif fileType == 'csv':
 			self._loadCSVImport(datapath, **kwargs)
 			self.Attributes['FeatureExtractionSoftware'] = 'Unknown'
 			if 'variableType' not in kwargs:
 				self.VariableType = VariableType.Discrete
 			else:
 				self.VariableType = kwargs['variableType']
 		elif fileType == 'xcms':
 			self._loadXCMSDataset(datapath, **kwargs)
 			self.Attributes['FeatureExtractionSoftware'] = 'XCMS'
 			self.VariableType = VariableType.Discrete
+		elif fileType == 'xcmsonline':
+			self._loadXCMSonlineDataset(datapath, **kwargs)
+			self.Attributes['FeatureExtractionSoftware'] = 'XCMSonline'
+			self.VariableType = VariableType.Discrete
 		elif fileType == 'biocrates':
 			self._loadBiocratesDataset(datapath, **kwargs)
 			self.Attributes['FeatureExtractionSoftware'] = 'Biocrates'
 			self.VariableType = VariableType.Discrete
 		elif fileType == 'metaboscape':
 			self._loadMetaboscapeDataset(datapath, **kwargs)
 			self.Attributes['FeatureExtractionSoftware'] = 'Metaboscape'
 			self.VariableType = VariableType.Discrete
+		elif fileType == 'npyc':
+			self._loadnPYcImport(datapath, **kwargs)
+			self.Attributes['FeatureExtractionSoftware'] = 'Unknown'
+			if 'variableType' not in kwargs:
+				self.VariableType = VariableType.Discrete
+			else:
+				self.VariableType = kwargs['variableType']
 		elif fileType == 'csv export':
 			(self.name, self.intensityData, self.featureMetadata, self.sampleMetadata) = self._initialiseFromCSV(
 				datapath)
 			if 'm/z' in self.featureMetadata.columns:
 				self.featureMetadata['m/z'] = self.featureMetadata['m/z'].apply(pandas.to_numeric, errors='ignore')
 			if 'Retention Time' in self.featureMetadata.columns:
 				self.featureMetadata['Retention Time'] = self.featureMetadata['Retention Time'].apply(pandas.to_numeric,
@@ -109,14 +146,15 @@
 			self.VariableType = VariableType.Discrete
 		elif fileType == 'empty':
 			# Lets us build an empty object for testing &c
 			pass
 		else:
 			raise NotImplementedError
 
+		self._intensityData = self._intensityData.astype(float)
 		self.featureMetadata['Exclusion Details'] = None
 		self.featureMetadata['User Excluded'] = False
 		self.featureMetadata[['rsdFilter', 'varianceRatioFilter', 'correlationToDilutionFilter', 'blankFilter',
 							  'artifactualFilter']] = pandas.DataFrame([[True, True, True, True, True]],
 																	   index=self.featureMetadata.index)
 
 		self.featureMetadata[['rsdSP', 'rsdSS/rsdSP', 'correlationToDilution', 'blankValue']] \
@@ -471,15 +509,15 @@
 										   ', '.join("{!s}={!r}".format(key, val) for (key, val) in kwargs.items()))])
 
 	def saveFeatureMask(self):
 		"""
 		Updates featureMask and saves as 'Passing Selection' in self.featureMetadata
 		"""
 
-		# Updates featureMask       
+		# Updates featureMask
 		self.updateMasks(filterSamples=False, filterFeatures=True)
 
 		# Save featureMask as 'Passing Selection' column in self.featureMetadata
 		self.featureMetadata['Passing Selection'] = self.featureMask
 
 		# Reset featureMask
 		self.initialiseMasks()
@@ -557,14 +595,166 @@
 		self.sampleMetadata['SampleType'] = None  # SampleType.StudySample
 		self.sampleMetadata['Dilution'] = 100
 		self.sampleMetadata['Metadata Available'] = False
 		self.sampleMetadata['Exclusion Details'] = None
 
 		self.Attributes['Log'].append([datetime.now(), 'Progenesis QI dataset loaded from %s' % (path)])
 
+	def _loadMZmineDataset(self, path):
+
+		# First import full table
+		dataT = pandas.read_csv(path, index_col=None)
+
+		# Raise error if MZmine3 csv format was chosen
+		if dataT.columns[0] == 'id':
+			raise NotImplementedError('MZmine3 export format not supported, choose legacy MZmine 2 export option')
+
+		# Read values as subset
+		values = dataT.filter(like="Peak area", axis=1)
+		self._intensityData = values.values.transpose()
+
+		# Get the sample names as the only metadata we have
+		sampleMetadata = dict()
+		sampleMetadata['Sample File Name'] = [name.replace('Peak area', '').rstrip() for name in list(values.columns.values)]
+
+		# Build feature name by combination of rt and m/z
+		feature_names = [str(round(row['row retention time'], 2)) + '_' + str(round(row['row m/z'], 4)) + 'm/z' for idx, row in dataT.iterrows()]
+
+		# Check for duplicated feature Names and append a '_1', etc if these exist
+		countNames = numpy.unique(feature_names, return_counts=True)
+		if max(countNames[1]) > 1:
+			for duplicatedIdx in numpy.where(countNames[1] > 1)[0]:
+				duplicatedFeature = countNames[0][duplicatedIdx]
+				featuresToModifyIdx = numpy.where(feature_names == duplicatedFeature)[0]
+				suffixCount = 1
+				for duplicatedfeatureIdx in featuresToModifyIdx:
+					feature_names[duplicatedfeatureIdx] = feature_names[duplicatedfeatureIdx] + '_' + str(suffixCount)
+					suffixCount += 1
+
+		# Calculate more feature metadata
+		peak_durations = dataT.filter(like="duration time", axis=1).mean(skipna=True, axis=1).round(3)
+		RT_min = dataT.filter(like="RT start", axis=1).replace(0,999999).min(skipna=True, axis=1).round(3)
+		RT_max = dataT.filter(like="RT end", axis=1).max(skipna=True, axis=1).round(3)
+
+		# Peak info
+		featureMetadata = dict()
+		featureMetadata['Feature Name'] = feature_names
+		featureMetadata['m/z'] = dataT['row m/z'].values
+		featureMetadata['Retention Time'] = dataT['row retention time'].values
+		featureMetadata['Retention Time - Minimum'] = RT_min
+		featureMetadata['Retention Time - Maximum'] = RT_max
+		featureMetadata['Peak Width'] = peak_durations
+
+		self.featureMetadata = pandas.DataFrame(numpy.vstack([featureMetadata[c] for c in featureMetadata.keys()]).T,
+												columns=featureMetadata.keys())
+		# keep the default empty sampleMetadata (column names) and fill it
+		for c in sampleMetadata.keys():
+			self.sampleMetadata[c] = sampleMetadata[c]
+
+		self.featureMetadata['Retention Time'] = self.featureMetadata['Retention Time'].astype(float)
+		self.featureMetadata['m/z'] = self.featureMetadata['m/z'].astype(float)
+
+		# self.initialiseMasks()
+
+		self.sampleMetadata['AssayRole'] = None  # AssayRole.Assay
+		self.sampleMetadata['SampleType'] = None  # SampleType.StudySample
+		self.sampleMetadata['Dilution'] = 100
+		self.sampleMetadata['Metadata Available'] = False
+		self.sampleMetadata['Exclusion Details'] = None
+
+		self.Attributes['Log'].append([datetime.now(), 'MZmine dataset loaded from %s' % (path)])
+
+	def _loadMSDIALDataset(self, path):
+
+		# Get index positions for MS-DIALs data blocks
+		dataT = pandas.read_csv(path, delimiter="\t", index_col=None, header=[0], nrows=1)
+
+		startIndex = dataT.columns.get_loc("Class") + 1
+		endIndex = dataT.columns.get_loc("NA")
+
+		dataSize = endIndex - startIndex
+
+		# Now read for real
+		dataT = pandas.read_csv(path, delimiter="\t", header=4)
+		values = dataT.iloc[:, startIndex:startIndex + dataSize]
+		self._intensityData = values.values.transpose()
+
+		# Get the sample names as the only metadata we have
+		sampleMetadata = dict()
+		sampleMetadata['Sample File Name'] = [name for name in list(values.columns.values)]
+
+		# Build feature name by combination of rt and m/z
+		feature_names = [str(round(row['Average Rt(min)'], 2)) + '_' + str(round(row['Average Mz'], 4)) + 'm/z' for idx, row in dataT.iterrows()]
+
+		# Check for duplicated feature Names and append a '_1', etc if these exist
+		countNames = numpy.unique(feature_names, return_counts=True)
+		if max(countNames[1]) > 1:
+			for duplicatedIdx in numpy.where(countNames[1] > 1)[0]:
+				duplicatedFeature = countNames[0][duplicatedIdx]
+				featuresToModifyIdx = numpy.where(feature_names == duplicatedFeature)[0]
+				suffixCount = 1
+				for duplicatedfeatureIdx in featuresToModifyIdx:
+					feature_names[duplicatedfeatureIdx] = feature_names[duplicatedfeatureIdx] + '_' + str(suffixCount)
+					suffixCount += 1
+
+		# Peak info
+		featureMetadata = dict()
+		featureMetadata['Feature Name'] = feature_names
+		featureMetadata['m/z'] = dataT['Average Mz'].values
+		featureMetadata['Retention Time'] = dataT['Average Rt(min)'].values
+		featureMetadata['Isotope Distribution'] = dataT['MS1 isotopic spectrum'].values
+		featureMetadata['Adducts'] = dataT['Adduct type'].values
+
+		self.featureMetadata = pandas.DataFrame(numpy.vstack([featureMetadata[c] for c in featureMetadata.keys()]).T,
+												columns=featureMetadata.keys())
+		# keep the default empty sampleMetadata (column names) and fill it
+		for c in sampleMetadata.keys():
+			self.sampleMetadata[c] = sampleMetadata[c]
+
+		self.featureMetadata['Retention Time'] = self.featureMetadata['Retention Time'].astype(float)
+		self.featureMetadata['m/z'] = self.featureMetadata['m/z'].astype(float)
+
+		# self.initialiseMasks()
+
+		# Import only metadata information
+		metadataT = pandas.read_csv(path, delimiter="\t", index_col=None, header=[0], nrows=3)
+		file_types = metadataT.iloc[0, startIndex:startIndex + dataSize]
+		injection_order = metadataT.iloc[1, startIndex:startIndex + dataSize].astype('int64').reset_index(drop=True)
+		batch_id = metadataT.iloc[2, startIndex:startIndex + dataSize].astype('int64').reset_index(drop=True)
+		assay_roles = []
+		sample_types = []
+
+		# Extract as much metadata as possible
+		for i in file_types:
+			if i == "Sample":
+				assay_roles.append('Assay')
+				sample_types.append('Study Sample')
+			elif i == "Standard":
+				assay_roles.append('Precision Reference')
+				sample_types.append('External Reference')
+			elif i == "QC":
+				assay_roles.append('Precision Reference') # assuming it is an undiluted pool
+				sample_types.append('Study Pool')
+			elif i == "Blank":
+				assay_roles.append('Assay')
+				sample_types.append('Procedural Blank')
+			else:
+				assay_roles.append(None)
+				sample_types.append(None)
+		self.sampleMetadata['AssayRole'] = assay_roles
+		self.sampleMetadata['SampleType'] = sample_types
+
+		self.sampleMetadata['Run Order'] = injection_order
+		self.sampleMetadata['Correction Batch'] = batch_id
+		self.sampleMetadata['Dilution'] = 100
+		self.sampleMetadata['Metadata Available'] = True
+		self.sampleMetadata['Exclusion Details'] = None
+
+		self.Attributes['Log'].append([datetime.now(), 'MS-DIAL dataset loaded from %s' % (path)])
+
 	def _loadCSVImport(self, path, noFeatureParams=1, variableType='Discrete'):
 
 		if variableType not in ['Discrete', 'Continuum', 'Profile', 'Spectrum']:
 			raise ValueError('Feature type must either be Discrete or Continuum')
 		# temporary here as not fully implemented
 		if variableType in ['Continuum', 'Profile', 'Spectrum']:
 			raise NotImplementedError
@@ -652,16 +842,27 @@
 
 		# for when peakTable methods is used directly instead of diffreport
 		# If no feature name is present, assume peakTable was used to derive the dataset and adjust accordingly
 		# If the try fails,
 		if 'name' not in dataT.columns:
 			try:
 				# build feature name by combination of rt and m/z
-				feature_names = [str(round(row['rt'], 2)) + '_' + str(round(row['mz'], 4)) + 'm/z' for idx, row in
-								 dataT.iterrows()]
+				feature_names = numpy.array([str(round(row['rt'], 2)) + '_' + str(round(row['mz'], 4)) + 'm/z' for idx, row in
+								 dataT.iterrows()])
+				# Check for duplicated feature Names and append a '_1', etc if these exist
+				countNames = numpy.unique(feature_names, return_counts=True)
+				if max(countNames[1]) > 1:
+					for duplicatedIdx in numpy.where(countNames[1] > 1)[0]:
+						duplicatedFeature = countNames[0][duplicatedIdx]
+						featuresToModifyIdx = numpy.where(feature_names == duplicatedFeature)[0]
+						suffixCount = 1
+						for duplicatedfeatureIdx in featuresToModifyIdx:
+							feature_names[duplicatedfeatureIdx] = feature_names[duplicatedfeatureIdx] + '_' + str(suffixCount)
+							suffixCount += 1
+
 				# insert feature name
 				dataT.insert(0, 'name', feature_names)
 				# rename mz to mzmed like in diffreport
 				dataT.rename(columns={'mz': 'mzmed', 'rt': 'rtmed'}, inplace=True)
 			except:
 				raise ValueError('XCMS data frame should be obtained with either peakTable or diffreport methods')
 
@@ -696,14 +897,95 @@
 		fileNameAndExtension = self.sampleMetadata['Sample File Name'].apply(os.path.splitext)
 		self.sampleMetadata['Sample File Name'] = [x[0] for x in fileNameAndExtension]
 
 		# self.initialiseMasks()
 
 		self.Attributes['Log'].append([datetime.now(), 'XCMS dataset loaded from %s' % (path)])
 
+	def _loadXCMSOnlineDataset(self, path, noFeatureParams=10):
+
+		# Import into dataframe
+		# XCMSonline result xlsx file must be manually converted to csv first (delimiter = ",") as pandas.read_excel cannot deal with large excel files such as these
+		dataT = pandas.read_csv(path, index_col=False)
+
+		# Find start of data
+		startIndex = noFeatureParams
+		# Find end of data. If annotated result file was used, it contains three extra columns that need to be excluded but not dropped ("isotopes", "adduct", "pcgroup")
+		if 'isotopes' in dataT.columns:
+			endIndex = dataT.columns.get_loc('isotopes')
+		else:
+			endIndex = len(dataT.columns)
+
+		dataSize = endIndex - startIndex
+
+		# Now read for real
+		values = dataT.iloc[:, startIndex:]
+		self._intensityData = values.values.transpose()
+
+		# Get the sample names as the only metadata we have
+		sampleMetadata = dict()
+		sampleMetadata['Sample File Name'] = [name for name in list(values.columns.values)]
+
+		# Peak info
+		featureMetadata = dict()
+
+		# By default, no feature name is present, thus assume peakTable was used to derive the dataset and adjust accordingly
+		# If the try fails,
+		if 'name' not in dataT.columns:
+			try:
+				# build feature name by combination of rt and m/z
+				# rename mzmed to mz and rtmed to rt for once
+				dataT.rename(columns={'mzmed': 'mz', 'rtmed': 'rt'}, inplace=True)
+				feature_names = [str(round(row['rt'], 2)) + '_' + str(round(row['mz'], 4)) + 'm/z' for idx, row in
+								 dataT.iterrows()]
+				# insert feature name
+				dataT.insert(0, 'name', feature_names)
+				# backname mz and rt like in diffreport
+				dataT.rename(columns={'mz': 'mzmed', 'rt': 'rtmed'}, inplace=True)
+			except:
+				raise ValueError('XCMSonline result data frame should be obtained with either peakTable or diffreport methods, check processing settings in XCMSonline')
+
+		featureMetadata['Feature Name'] = dataT['name'].values
+		featureMetadata['m/z'] = dataT['mzmed'].values
+		featureMetadata['Retention Time'] = dataT['rtmed'].values
+		featureMetadata['m/z - Minimum'] = dataT['mzmin'].values
+		featureMetadata['m/z - Maximum'] = dataT['mzmax'].values
+		featureMetadata['Retention Time - Minimum'] = dataT['rtmin'].values
+		featureMetadata['Retention Time - Maximum'] = dataT['rtmax'].values
+		# If the annotated result file was used, let us also collect adduct values
+		if 'adduct' in dataT.columns:
+			featureMetadata['Adducts'] = dataT['adduct'].values
+
+		self.featureMetadata = pandas.DataFrame(numpy.vstack([featureMetadata[c] for c in featureMetadata.keys()]).T,
+												columns=featureMetadata.keys())
+		self.sampleMetadata = pandas.DataFrame(
+			numpy.concatenate([sampleMetadata[c] for c in sampleMetadata.keys()], axis=0),
+			columns=sampleMetadata.keys())
+
+		# Put Feature Names first
+		name = self.featureMetadata['Feature Name']
+		self.featureMetadata.drop(labels=['Feature Name'], axis=1, inplace=True)
+		self.featureMetadata.insert(0, 'Feature Name', name)
+
+		self.featureMetadata['Retention Time'] = self.featureMetadata['Retention Time'].astype(float)
+		self.featureMetadata['m/z'] = self.featureMetadata['m/z'].astype(float)
+
+		self.sampleMetadata['AssayRole'] = None  # AssayRole.Assay
+		self.sampleMetadata['SampleType'] = None  # SampleType.StudySample
+		self.sampleMetadata['Dilution'] = 100
+		self.sampleMetadata['Metadata Available'] = False
+		self.sampleMetadata['Exclusion Details'] = None
+
+		fileNameAndExtension = self.sampleMetadata['Sample File Name'].apply(os.path.splitext)
+		self.sampleMetadata['Sample File Name'] = [x[0] for x in fileNameAndExtension]
+
+		# self.initialiseMasks()
+
+		self.Attributes['Log'].append([datetime.now(), 'XCMSonline dataset loaded from %s' % (path)])
+
 	def _loadBiocratesDataset(self, path, noSampleParams=15, sheetName='Data Export'):
 
 		# Read in data
 		dataT = pandas.read_excel(path, sheet_name=sheetName, skiprows=[0])
 
 		##
 		# Intensity matrix
@@ -859,14 +1141,103 @@
 		self.sampleMetadata = sampleMetadata
 		self.featureMetadata = featureMetadata
 
 		# self.initialiseMasks()
 
 		self.Attributes['Log'].append([datetime.now(), 'Metaboscape dataset loaded from %s' % (path)])
 
+	def _loadnPYcImport(self, path, noFeatureParams=6, variableType='Discrete'):
+
+		if variableType not in ['Discrete', 'Continuum', 'Profile', 'Spectrum']:
+			raise ValueError('Feature type must either be Discrete or Continuum')
+		# temporary here as not fully implemented
+		if variableType in ['Continuum', 'Profile', 'Spectrum']:
+			raise NotImplementedError
+
+		# Import into dataframe
+		dataT = pandas.read_csv(path, index_col=False)
+
+		# Find start of data
+		startIndex = noFeatureParams
+		endIndex = len(dataT.columns)
+		# Starting row of features depends on dataset, therefore find start of first feature which is always named '0'
+		startRow = dataT[dataT.iloc[:,0] == '0'].index[0]
+
+		# Now read for real
+		values = dataT.iloc[startRow:, startIndex:]
+		self._intensityData = values.values
+
+		# Get the sample names as the only metadata we have
+		sampleMetadata = dict()
+		sampleMetadata['Sample File Name'] = [name for name in list(dataT.loc[startRow:, 'Sample File Name'])]
+
+		# Peak info
+		featureMetadata = dict()
+		# Feature Names, m/z and Retention Time are set as rows 0,1,2 - others are dependent on original dataset and software used for preprocessing
+		feature_names = dataT.iloc[0,startIndex:]
+		featureMetadata['Feature Name'] = feature_names
+		mz_values = dataT.iloc[1,startIndex:]
+		featureMetadata['m/z'] = mz_values
+		rt_values = dataT.iloc[2,startIndex:]
+		featureMetadata['Retention Time'] = rt_values
+		# Check if other metadata is part of import file
+		if dataT.iloc[:,0].isin(['m/z - Minimum']).any():
+			metadataRow = dataT[dataT.iloc[:,0] == 'm/z - Minimum'].index[0]
+			featureMetadata['m/z - Minimum'] = dataT.iloc[metadataRow,startIndex:]
+		if dataT.iloc[:,0].isin(['m/z - Maximum']).any():
+			metadataRow = dataT[dataT.iloc[:,0] == 'm/z - Maximum'].index[0]
+			featureMetadata['m/z - Maximum'] = dataT.iloc[metadataRow,startIndex:]
+		if dataT.iloc[:,0].isin(['Retention Time - Minimum']).any():
+			metadataRow = dataT[dataT.iloc[:,0] == 'Retention Time - Minimum'].index[0]
+			featureMetadata['Retention Time - Minimum'] = dataT.iloc[metadataRow,startIndex:]
+		if dataT.iloc[:,0].isin(['Retention Time - Maximum']).any():
+			metadataRow = dataT[dataT.iloc[:,0] == 'Retention Time - Maximum'].index[0]
+			featureMetadata['Retention Time - Maximum'] = dataT.iloc[metadataRow,startIndex:]
+		if dataT.iloc[:,0].isin(['Peak Width']).any():
+			metadataRow = dataT[dataT.iloc[:,0] == 'Peak Width'].index[0]
+			featureMetadata['Peak Width'] = dataT.iloc[metadataRow,startIndex:]
+		if dataT.iloc[:,0].isin(['Isotope Distribution']).any():
+			metadataRow = dataT[dataT.iloc[:,0] == 'Isotope Distribution'].index[0]
+			featureMetadata['Isotope Distribution'] = dataT.iloc[metadataRow,startIndex:]
+		if dataT.iloc[:,0].isin(['Adducts']).any():
+			metadataRow = dataT[dataT.iloc[:,0] == 'Adducts'].index[0]
+			featureMetadata['Adducts'] = dataT.iloc[metadataRow,startIndex:]
+		if dataT.iloc[:,0].isin(['Class']).any():
+			metadataRow = dataT[dataT.iloc[:,0] == 'Class'].index[0]
+			featureMetadata['Class'] = dataT.iloc[metadataRow,startIndex:]
+		if dataT.iloc[:,0].isin(['LOD (μM)']).any():
+			metadataRow = dataT[dataT.iloc[:,0] == 'LOD (μM)'].index[0]
+			featureMetadata['LOD (μM)'] = dataT.iloc[metadataRow,startIndex:]
+
+		self.featureMetadata = pandas.DataFrame(numpy.vstack([featureMetadata[c] for c in featureMetadata.keys()]).T,
+												columns=featureMetadata.keys())
+		self.sampleMetadata = pandas.DataFrame(
+			numpy.concatenate([sampleMetadata[c] for c in sampleMetadata.keys()], axis=0),
+			columns=sampleMetadata.keys())
+
+		# Put Feature Names first
+		name = self.featureMetadata['Feature Name']
+		self.featureMetadata.drop(labels=['Feature Name'], axis=1, inplace=True)
+		self.featureMetadata.insert(0, 'Feature Name', name)
+
+		self.sampleMetadata['AssayRole'] = dataT.loc[startRow:, 'AssayRole']
+		self.sampleMetadata['SampleType'] = dataT.loc[startRow:, 'SampleType']
+		self.sampleMetadata['Run Order'] = dataT.loc[startRow:, 'Run Order'].astype('int64')
+		self.sampleMetadata['Dilution'] = 100 # Dilution is not stored to nPYc export
+		self.sampleMetadata['Metadata Available'] = True # No new import of metadata needed
+
+		self.sampleMetadata['Exclusion Details'] = None
+
+		fileNameAndExtension = self.sampleMetadata['Sample File Name'].apply(os.path.splitext)
+		self.sampleMetadata['Sample File Name'] = [x[0] for x in fileNameAndExtension]
+
+		# self.initialiseMasks()
+
+		self.Attributes['Log'].append([datetime.now(), 'nPYc dataset loaded from %s' % (path)])
+
 	def _getSampleMetadataFromRawData(self, rawDataPath, filetype="Waters .raw"):
 		"""
 		Pull metadata out of raw experiment files.
 		"""
 		# Validate inputs
 		if not os.path.isdir(rawDataPath):
 			raise ValueError('No directory found at %s' % (rawDataPath))
@@ -1401,225 +1772,14 @@
 		self.featureMetadata.loc[:, ['rsdFilter', 'varianceRatioFilter', 'correlationToDilutionFilter', 'blankFilter',
 									 'artifactualFilter']] = True
 
 		self.featureMetadata.loc[:, ['rsdSP', 'rsdSS/rsdSP', 'correlationToDilution', 'blankValue']] = numpy.nan
 		self.featureMetadata.loc[:, 'User Excluded'] = False
 		self.featureMetadata.loc[:, 'Exclusion Details'] = None
 
-	def _exportISATAB(self, destinationPath, detailsDict):
-		"""
-		Export the dataset's metadata to the directory *destinationPath* as ISATAB
-		detailsDict should have the format:
-		detailsDict = {
-			'investigation_identifier' : "i1",
-			'investigation_title' : "Give it a title",
-			'investigation_description' : "Add a description",
-			'investigation_submission_date' : "2016-11-03",
-			'investigation_public_release_date' : "2016-11-03",
-			'first_name' : "Noureddin",
-			'last_name' : "Sadawi",
-			'affiliation' : "University",
-			'study_filename' : "my_ms_study",
-			'study_material_type' : "Serum",
-			'study_identifier' : "s1",
-			'study_title' : "Give the study a title",
-			'study_description' : "Add study description",
-			'study_submission_date' : "2016-11-03",
-			'study_public_release_date' : "2016-11-03",
-			'assay_filename' : "my_ms_assay"
-		}
-
-		:param str destinationPath: Path to a directory in which the output will be saved
-		:param dict detailsDict: Contains several key: value pairs required to for ISATAB
-		:raises IOError: If writing one of the files fails
-		"""
-
-		from isatools.model import Investigation, Study, Assay, OntologyAnnotation, OntologySource, Person, Publication, \
-			Protocol, Source
-		from isatools.model import Comment, Sample, Characteristic, Process, Material, DataFile, ParameterValue, plink
-		from isatools import isatab
-		import isaExplorer as ie
-
-		investigation = Investigation()
-
-		investigation.identifier = detailsDict['investigation_identifier']
-		investigation.title = detailsDict['investigation_title']
-		investigation.description = detailsDict['investigation_description']
-		investigation.submission_date = detailsDict['investigation_submission_date']  # use today if not specified
-		investigation.public_release_date = detailsDict['investigation_public_release_date']
-		study = Study(filename='s_' + detailsDict['study_filename'] + '.txt')
-		study.identifier = detailsDict['study_identifier']
-		study.title = detailsDict['study_title']
-		study.description = detailsDict['study_description']
-		study.submission_date = detailsDict['study_submission_date']
-		study.public_release_date = detailsDict['study_public_release_date']
-		investigation.studies.append(study)
-		obi = OntologySource(name='OBI', description="Ontology for Biomedical Investigations")
-		investigation.ontology_source_references.append(obi)
-		intervention_design = OntologyAnnotation(term_source=obi)
-		intervention_design.term = "intervention design"
-		intervention_design.term_accession = "http://purl.obolibrary.org/obo/OBI_0000115"
-		study.design_descriptors.append(intervention_design)
-
-		# Other instance variables common to both Investigation and Study objects include 'contacts' and 'publications',
-		# each with lists of corresponding Person and Publication objects.
-
-		contact = Person(first_name=detailsDict['first_name'], last_name=detailsDict['last_name'],
-						 affiliation=detailsDict['affiliation'], roles=[OntologyAnnotation(term='submitter')])
-		study.contacts.append(contact)
-		publication = Publication(title="Experiments with Data", author_list="Auther 1, Author 2")
-		publication.pubmed_id = "12345678"
-		publication.status = OntologyAnnotation(term="published")
-		study.publications.append(publication)
-
-		# To create the study graph that corresponds to the contents of the study table file (the s_*.txt file), we need
-		# to create a process sequence. To do this we use the Process class and attach it to the Study object's
-		# 'process_sequence' list instance variable. Each process must be linked with a Protocol object that is attached to
-		# a Study object's 'protocols' list instance variable. The sample collection Process object usually has as input
-		# a Source material and as output a Sample material.
-
-		sample_collection_protocol = Protocol(id_="sample collection", name="sample collection",
-											  protocol_type=OntologyAnnotation(term="sample collection"))
-		aliquoting_protocol = Protocol(id_="aliquoting", name="aliquoting",
-									   protocol_type=OntologyAnnotation(term="aliquoting"))
-
-		for index, row in self.sampleMetadata.iterrows():
-			src_name = row['Sample File Name']
-			source = Source(name=src_name)
-
-			source.comments.append(Comment(name='Study Name', value=row['Study']))
-			study.sources.append(source)
-
-			sample_name = src_name
-
-			# sample_name = 'sample_'+str(index)
-			sample = Sample(name=sample_name, derives_from=[source])
-			# check if field exists first
-			status = row['Status'] if 'Status' in self.sampleMetadata.columns else 'N/A'
-			characteristic_material_type = Characteristic(category=OntologyAnnotation(term="material type"),
-														  value=status)
-			sample.characteristics.append(characteristic_material_type)
-
-			# characteristic_material_role = Characteristic(category=OntologyAnnotation(term="material role"), value=row['SampleType'])
-			# sample.characteristics.append(characteristic_material_role)
-
-			# check if field exists first
-			age = row['Age'] if 'Age' in self.sampleMetadata.columns else 'N/A'
-			characteristic_age = Characteristic(category=OntologyAnnotation(term="Age"), value=age, unit='Year')
-			sample.characteristics.append(characteristic_age)
-			# check if field exists first
-			gender = row['Gender'] if 'Gender' in self.sampleMetadata.columns else 'N/A'
-			characteristic_gender = Characteristic(category=OntologyAnnotation(term="Gender"), value=gender)
-			sample.characteristics.append(characteristic_gender)
-
-			ncbitaxon = OntologySource(name='NCBITaxon', description="NCBI Taxonomy")
-			characteristic_organism = Characteristic(category=OntologyAnnotation(term="Organism"),
-													 value=OntologyAnnotation(term="Homo Sapiens",
-																			  term_source=ncbitaxon,
-																			  term_accession="http://purl.bioontology.org/ontology/NCBITAXON/9606"))
-			sample.characteristics.append(characteristic_organism)
-			# check if field exists first
-			sampling_date = row['Sampling Date'] if not pandas.isnull(row['Sampling Date']) else None
-			sample_collection_process = Process(id_='sam_coll_proc', executes_protocol=sample_collection_protocol,
-												date_=sampling_date)
-			aliquoting_process = Process(id_='sam_coll_proc', executes_protocol=aliquoting_protocol,
-										 date_=sampling_date)
-
-			sample_collection_process.inputs = [source]
-			aliquoting_process.outputs = [sample]
-
-			# links processes
-			plink(sample_collection_process, aliquoting_process)
-
-			study.process_sequence.append(sample_collection_process)
-			study.process_sequence.append(aliquoting_process)
-
-			study.samples.append(sample)
-
-		study.protocols.append(sample_collection_protocol)
-		study.protocols.append(aliquoting_protocol)
-
-		### Add MS Assay ###
-		ms_assay = Assay(filename='a_' + detailsDict['assay_filename'] + '.txt',
-						 measurement_type=OntologyAnnotation(term="metabolite profiling"),
-						 technology_type=OntologyAnnotation(term="mass spectrometry"))
-		extraction_protocol = Protocol(name='extraction', protocol_type=OntologyAnnotation(term="material extraction"))
-
-		study.protocols.append(extraction_protocol)
-		ms_protocol = Protocol(name='mass spectrometry', protocol_type=OntologyAnnotation(term="MS Assay"))
-		ms_protocol.add_param('Run Order')
-		ms_protocol.add_param('Instrument')
-		ms_protocol.add_param('Sample Batch')
-		ms_protocol.add_param('Acquisition Batch')
-
-		study.protocols.append(ms_protocol)
-
-		# for index, row in sampleMetadata.iterrows():
-		for index, sample in enumerate(study.samples):
-			row = self.sampleMetadata.loc[self.sampleMetadata['Sample File Name'].astype(str) == sample.name]
-
-			# create an extraction process that executes the extraction protocol
-			extraction_process = Process(executes_protocol=extraction_protocol)
-
-			# extraction process takes as input a sample, and produces an extract material as output
-			sample_name = sample.name
-			sample = Sample(name=sample_name, derives_from=[source])
-
-			extraction_process.inputs.append(sample)
-			material = Material(name="extract-{}".format(index))
-			material.type = "Extract Name"
-			extraction_process.outputs.append(material)
-
-			# create a ms process that executes the nmr protocol
-			ms_process = Process(executes_protocol=ms_protocol, date_=datetime.isoformat(
-				datetime.strptime(str(row['Acquired Time'].values[0]), '%Y-%m-%d %H:%M:%S')))
-
-			ms_process.name = "assay-name-{}".format(index)
-			ms_process.inputs.append(extraction_process.outputs[0])
-			# nmr process usually has an output data file
-			# check if field exists first
-			assay_data_name = row['Assay data name'].values[
-				0] if 'Assay data name' in self.sampleMetadata.columns else 'N/A'
-			datafile = DataFile(filename=assay_data_name, label="MS Assay Name", generated_from=[sample])
-			ms_process.outputs.append(datafile)
-
-			# nmr_process.parameter_values.append(ParameterValue(category='Run Order',value=str(i)))
-			ms_process.parameter_values = [
-				ParameterValue(category=ms_protocol.get_param('Run Order'), value=row['Run Order'].values[0])]
-			# check if field exists first
-			instrument = row['Instrument'].values[0] if 'Instrument' in self.sampleMetadata.columns else 'N/A'
-			ms_process.parameter_values.append(
-				ParameterValue(category=ms_protocol.get_param('Instrument'), value=instrument))
-			# check if field exists first
-			sbatch = row['Sample batch'].values[0] if 'Sample batch' in self.sampleMetadata.columns else 'N/A'
-			ms_process.parameter_values.append(
-				ParameterValue(category=ms_protocol.get_param('Sample Batch'), value=sbatch))
-
-			ms_process.parameter_values.append(
-				ParameterValue(category=ms_protocol.get_param('Acquisition Batch'), value=row['Batch'].values[0]))
-
-			# ensure Processes are linked forward and backward
-			plink(extraction_process, ms_process)
-			# make sure the extract, data file, and the processes are attached to the assay
-			ms_assay.samples.append(sample)
-			ms_assay.data_files.append(datafile)
-			ms_assay.other_material.append(material)
-			ms_assay.process_sequence.append(extraction_process)
-			ms_assay.process_sequence.append(ms_process)
-			ms_assay.measurement_type = OntologyAnnotation(term="metabolite profiling")
-			ms_assay.technology_type = OntologyAnnotation(term="mass spectrometry")
-
-		# attach the assay to the study
-		study.assays.append(ms_assay)
-
-		if os.path.exists(os.path.join(destinationPath, 'i_Investigation.txt')):
-			ie.appendStudytoISA(study, destinationPath)
-		else:
-			isatab.dump(isa_obj=investigation, output_path=destinationPath)
-
 	def validateObject(self, verbose=True, raiseError=False, raiseWarning=True):
 		"""
 		Checks that all the attributes specified in the class definition are present and of the required class and/or values.
 
 		Returns 4 boolean: is the object a *Dataset* < a *basic MSDataset* < has the object *parameters for QC* < *has the object sample metadata*.
 
 		To employ all class methods, the most inclusive (*has the object sample metadata*) must be successful:
@@ -2081,15 +2241,16 @@
 				failure = 'Check self.filePath is a str:\tFailure, \'self.filePath\' is ' + str(type(self.filePath))
 				failureListBasic = conditionTest(condition, success, failure, failureListBasic, verbose, raiseError,
 												 raiseWarning, exception=TypeError(failure))
 			# end self.filePath
 
 			## self._intensityData
 			# Use _intensityData as size reference for all future tables
-			if (self._intensityData.all() != numpy.array(None).all()):
+			# if (self._intensityData.all() != numpy.array(None).all()):
+			if self._intensityData.shape != ():
 				refNumSamples = self._intensityData.shape[0]
 				refNumFeatures = self._intensityData.shape[1]
 				if verbose:
 					print('---- self._intensityData used as size reference ----')
 					print('\t' + str(refNumSamples) + ' samples, ' + str(refNumFeatures) + ' features')
 			# end self._intensityData
```

### Comparing `nPYc-1.2.6/nPYc/objects/_targetedDataset.py` & `nPYc-1.2.7/nPYc/objects/_targetedDataset.py`

 * *Files identical despite different names*

### Comparing `nPYc-1.2.6/nPYc/plotting/__init__.py` & `nPYc-1.2.7/nPYc/plotting/__init__.py`

 * *Files identical despite different names*

### Comparing `nPYc-1.2.6/nPYc/plotting/_correlationSpectroscopy.py` & `nPYc-1.2.7/nPYc/plotting/_correlationSpectroscopy.py`

 * *Files identical despite different names*

### Comparing `nPYc-1.2.6/nPYc/plotting/_jointplotRSDvCorrelation.py` & `nPYc-1.2.7/nPYc/plotting/_jointplotRSDvCorrelation.py`

 * *Files identical despite different names*

### Comparing `nPYc-1.2.6/nPYc/plotting/_multivariatePlotting.py` & `nPYc-1.2.7/nPYc/plotting/_multivariatePlotting.py`

 * *Files 0% similar despite different names*

```diff
@@ -472,14 +472,15 @@
 	for i in numpy.arange(0,nc):
 
 		cVect = pcaModel.loadings[i, :]
 		orig_cmap = plt.cm.RdYlBu_r # Red for high, Blue for negative, and we will have a very neutral yellow for 0
 		maxval = numpy.max([numpy.abs(numpy.max(cVect)), numpy.abs(numpy.min(cVect))])
 		maxcol = maxval#numpy.max(cVect) # grab the maximum
 		mincol = -maxval#numpy.min(cVect) # Grab the minimum
+		#name = 'new_%s' % i
 		new_cmap = _shiftedColorMap(orig_cmap, start=0, midpoint=1 - maxcol/(maxcol + numpy.abs(mincol)), stop=1, name='new')
 
 		fig, ax = plt.subplots(figsize=figureSize, dpi=dpi)
 
 		if ((msData.VariableType.name == 'Discrete') & (hasattr(msData.featureMetadata, 'Retention Time'))):
 
 			# To set the alpha of each point to be associated with the weight of the loading, generate an array where each row corresponds to a feature, the
@@ -1121,10 +1122,11 @@
 
 		cdict['red'].append((si, r, r))
 		cdict['green'].append((si, g, g))
 		cdict['blue'].append((si, b, b))
 		cdict['alpha'].append((si, a, a))
 
 	newcmap = matplotlib.colors.LinearSegmentedColormap(name, cdict)
-	plt.register_cmap(cmap=newcmap)
+	matplotlib.colormaps.register(newcmap,force=True)
+	#plt.register_cmap(cmap=newcmap)
 
 	return newcmap
```

### Comparing `nPYc-1.2.6/nPYc/plotting/_nmrPlotting.py` & `nPYc-1.2.7/nPYc/plotting/_nmrPlotting.py`

 * *Files identical despite different names*

### Comparing `nPYc-1.2.6/nPYc/plotting/_plotBatchAndROCorrection.py` & `nPYc-1.2.7/nPYc/plotting/_plotBatchAndROCorrection.py`

 * *Files identical despite different names*

### Comparing `nPYc-1.2.6/nPYc/plotting/_plotDiscreteLoadings.py` & `nPYc-1.2.7/nPYc/plotting/_plotDiscreteLoadings.py`

 * *Files identical despite different names*

### Comparing `nPYc-1.2.6/nPYc/plotting/_plotFeatureAccuracyPrecision.py` & `nPYc-1.2.7/nPYc/plotting/_plotFeatureAccuracyPrecision.py`

 * *Files identical despite different names*

### Comparing `nPYc-1.2.6/nPYc/plotting/_plotFeatureLOQ.py` & `nPYc-1.2.7/nPYc/plotting/_plotFeatureLOQ.py`

 * *Files identical despite different names*

### Comparing `nPYc-1.2.6/nPYc/plotting/_plotFeatureRanges.py` & `nPYc-1.2.7/nPYc/plotting/_plotFeatureRanges.py`

 * *Files identical despite different names*

### Comparing `nPYc-1.2.6/nPYc/plotting/_plotIonMap.py` & `nPYc-1.2.7/nPYc/plotting/_plotIonMap.py`

 * *Files identical despite different names*

### Comparing `nPYc-1.2.6/nPYc/plotting/_plotLOQFeatureViolin.py` & `nPYc-1.2.7/nPYc/plotting/_plotLOQFeatureViolin.py`

 * *Files identical despite different names*

### Comparing `nPYc-1.2.6/nPYc/plotting/_plotLOQRunOrder.py` & `nPYc-1.2.7/nPYc/plotting/_plotLOQRunOrder.py`

 * *Files identical despite different names*

### Comparing `nPYc-1.2.6/nPYc/plotting/_plotNMRbaseline.py` & `nPYc-1.2.7/nPYc/plotting/_plotNMRbaseline.py`

 * *Files identical despite different names*

### Comparing `nPYc-1.2.6/nPYc/plotting/_plotNMRcalibration.py` & `nPYc-1.2.7/nPYc/plotting/_plotNMRcalibration.py`

 * *Files identical despite different names*

### Comparing `nPYc-1.2.6/nPYc/plotting/_plotNMRsolvent.py` & `nPYc-1.2.7/nPYc/plotting/_plotNMRsolvent.py`

 * *Files identical despite different names*

### Comparing `nPYc-1.2.6/nPYc/plotting/_plotRSDs.py` & `nPYc-1.2.7/nPYc/plotting/_plotRSDs.py`

 * *Files identical despite different names*

### Comparing `nPYc-1.2.6/nPYc/plotting/_plotSpectralVariance.py` & `nPYc-1.2.7/nPYc/plotting/_plotSpectralVariance.py`

 * *Files identical despite different names*

### Comparing `nPYc-1.2.6/nPYc/plotting/_plotTIC.py` & `nPYc-1.2.7/nPYc/plotting/_plotTIC.py`

 * *Files identical despite different names*

### Comparing `nPYc-1.2.6/nPYc/plotting/_plotTargeted.py` & `nPYc-1.2.7/nPYc/plotting/_plotTargeted.py`

 * *Files identical despite different names*

### Comparing `nPYc-1.2.6/nPYc/plotting/_plotTargetedFeatureDistribution.py` & `nPYc-1.2.7/nPYc/plotting/_plotTargetedFeatureDistribution.py`

 * *Files identical despite different names*

### Comparing `nPYc-1.2.6/nPYc/plotting/_plotVariableScatter.py` & `nPYc-1.2.7/nPYc/plotting/_plotVariableScatter.py`

 * *Files identical despite different names*

### Comparing `nPYc-1.2.6/nPYc/plotting/_plotting.py` & `nPYc-1.2.7/nPYc/plotting/_plotting.py`

 * *Files identical despite different names*

### Comparing `nPYc-1.2.6/nPYc/plotting/_rangeFrameLocator.py` & `nPYc-1.2.7/nPYc/plotting/_rangeFrameLocator.py`

 * *Files identical despite different names*

### Comparing `nPYc-1.2.6/nPYc/plotting/_violinPlot.py` & `nPYc-1.2.7/nPYc/plotting/_violinPlot.py`

 * *Files identical despite different names*

### Comparing `nPYc-1.2.6/nPYc/reports/__init__.py` & `nPYc-1.2.7/nPYc/reports/__init__.py`

 * *Files identical despite different names*

### Comparing `nPYc-1.2.6/nPYc/reports/_finalReportPeakPantheR.py` & `nPYc-1.2.7/nPYc/reports/_finalReportPeakPantheR.py`

 * *Files identical despite different names*

### Comparing `nPYc-1.2.6/nPYc/reports/_generateBasicPCAReport.py` & `nPYc-1.2.7/nPYc/reports/_generateBasicPCAReport.py`

 * *Files identical despite different names*

### Comparing `nPYc-1.2.6/nPYc/reports/_generateFeatureDistributionReport.py` & `nPYc-1.2.7/nPYc/reports/_generateFeatureDistributionReport.py`

 * *Files identical despite different names*

### Comparing `nPYc-1.2.6/nPYc/reports/_generateReportMS.py` & `nPYc-1.2.7/nPYc/reports/_generateReportMS.py`

 * *Files identical despite different names*

### Comparing `nPYc-1.2.6/nPYc/reports/_generateReportNMR.py` & `nPYc-1.2.7/nPYc/reports/_generateReportNMR.py`

 * *Files identical despite different names*

### Comparing `nPYc-1.2.6/nPYc/reports/_generateReportTargeted.py` & `nPYc-1.2.7/nPYc/reports/_generateReportTargeted.py`

 * *Files identical despite different names*

### Comparing `nPYc-1.2.6/nPYc/reports/_generateSampleReport.py` & `nPYc-1.2.7/nPYc/reports/_generateSampleReport.py`

 * *Files identical despite different names*

### Comparing `nPYc-1.2.6/nPYc/reports/featureID.py` & `nPYc-1.2.7/nPYc/reports/featureID.py`

 * *Files 2% similar despite different names*

```diff
@@ -262,19 +262,20 @@
 	intCorrs = _vcorrcoef((msData.intensityData[sampleMask,:]), numpy.transpose(msData.intensityData[sampleMask, featureNo]))
 
 	# Null out excluded features
 	intCorrs[msData.featureMask == False] = 0
 	intCorrs[numpy.isnan(intCorrs)] = 0
 
 	color = sns.color_palette()[1]
-	grid = sns.JointGrid(msData.featureMetadata[intCorrs > msData.Attributes['corrThreshold']]['m/z'].values, msData.featureMetadata[intCorrs > msData.Attributes['corrThreshold']]['Retention Time'].values,
-					space=1, size=6, ratio=50,
+	grid = sns.JointGrid(pandas.DataFrame(data={'m/z':msData.featureMetadata[intCorrs > msData.Attributes['corrThreshold']]['m/z'].values,'Retention Time':msData.featureMetadata[intCorrs > msData.Attributes['corrThreshold']]['Retention Time'].values}),
+					space=1, height=6, ratio=50, x='Retention Time', y='m/z',
 					xlim=(msData.featureMetadata['m/z'].min(), msData.featureMetadata['m/z'].max()),
 					ylim=(msData.featureMetadata['Retention Time'].min(), msData.featureMetadata['Retention Time'].max()))
-	grid.plot_joint(plt.scatter, color=color, alpha=.8)
+
+	grid.plot_joint(sns.scatterplot, color=color, alpha=.8)
 	grid.plot_marginals(sns.rugplot, color=color)
 
 	grid.set_axis_labels('m/z', 'Retention Time')
 
 	# sns.despine(trim=True)
 	plt.tight_layout()
 	plt.savefig(item['RelatedFigure'], format=msData.Attributes['figureFormat'], dpi=msData.Attributes['dpi'])
```

### Comparing `nPYc-1.2.6/nPYc/reports/generateReport.py` & `nPYc-1.2.7/nPYc/reports/generateReport.py`

 * *Files identical despite different names*

### Comparing `nPYc-1.2.6/nPYc/reports/multivariateReport.py` & `nPYc-1.2.7/nPYc/reports/multivariateReport.py`

 * *Files identical despite different names*

### Comparing `nPYc-1.2.6/nPYc/utilities/__init__.py` & `nPYc-1.2.7/nPYc/utilities/__init__.py`

 * *Files identical despite different names*

### Comparing `nPYc-1.2.6/nPYc/utilities/_addReferenceRanges.py` & `nPYc-1.2.7/nPYc/utilities/_addReferenceRanges.py`

 * *Files identical despite different names*

### Comparing `nPYc-1.2.6/nPYc/utilities/_buildSpectrumFromQIfeature.py` & `nPYc-1.2.7/nPYc/utilities/_buildSpectrumFromQIfeature.py`

 * *Files identical despite different names*

### Comparing `nPYc-1.2.6/nPYc/utilities/_calibratePPMscale.py` & `nPYc-1.2.7/nPYc/utilities/_calibratePPMscale.py`

 * *Files identical despite different names*

### Comparing `nPYc-1.2.6/nPYc/utilities/_checkInRange.py` & `nPYc-1.2.7/nPYc/utilities/_checkInRange.py`

 * *Files identical despite different names*

### Comparing `nPYc-1.2.6/nPYc/utilities/_conditionalJoin.py` & `nPYc-1.2.7/nPYc/utilities/_conditionalJoin.py`

 * *Files identical despite different names*

### Comparing `nPYc-1.2.6/nPYc/utilities/_filters.py` & `nPYc-1.2.7/nPYc/utilities/_filters.py`

 * *Files identical despite different names*

### Comparing `nPYc-1.2.6/nPYc/utilities/_fitPeak.py` & `nPYc-1.2.7/nPYc/utilities/_fitPeak.py`

 * *Files identical despite different names*

### Comparing `nPYc-1.2.6/nPYc/utilities/_getMetadataFromBrukerNMR.py` & `nPYc-1.2.7/nPYc/utilities/_getMetadataFromBrukerNMR.py`

 * *Files identical despite different names*

### Comparing `nPYc-1.2.6/nPYc/utilities/_getMetadataFromWatersRaw.py` & `nPYc-1.2.7/nPYc/utilities/_getMetadataFromWatersRaw.py`

 * *Files identical despite different names*

### Comparing `nPYc-1.2.6/nPYc/utilities/_getMetadataFrommzML.py` & `nPYc-1.2.7/nPYc/utilities/_getMetadataFrommzML.py`

 * *Files identical despite different names*

### Comparing `nPYc-1.2.6/nPYc/utilities/_importBrukerSpectrum.py` & `nPYc-1.2.7/nPYc/utilities/_importBrukerSpectrum.py`

 * *Files identical despite different names*

### Comparing `nPYc-1.2.6/nPYc/utilities/_internal.py` & `nPYc-1.2.7/nPYc/utilities/_internal.py`

 * *Files identical despite different names*

### Comparing `nPYc-1.2.6/nPYc/utilities/_lineWidth.py` & `nPYc-1.2.7/nPYc/utilities/_lineWidth.py`

 * *Files identical despite different names*

### Comparing `nPYc-1.2.6/nPYc/utilities/_massSpectrumBuilder.py` & `nPYc-1.2.7/nPYc/utilities/_massSpectrumBuilder.py`

 * *Files identical despite different names*

### Comparing `nPYc-1.2.6/nPYc/utilities/_nmr.py` & `nPYc-1.2.7/nPYc/utilities/_nmr.py`

 * *Files identical despite different names*

### Comparing `nPYc-1.2.6/nPYc/utilities/_npc_sampleledger.py` & `nPYc-1.2.7/nPYc/utilities/_npc_sampleledger.py`

 * *Files identical despite different names*

### Comparing `nPYc-1.2.6/nPYc/utilities/_readBrukerXML.py` & `nPYc-1.2.7/nPYc/utilities/_readBrukerXML.py`

 * *Files identical despite different names*

### Comparing `nPYc-1.2.6/nPYc/utilities/extractParams.py` & `nPYc-1.2.7/nPYc/utilities/extractParams.py`

 * *Files identical despite different names*

### Comparing `nPYc-1.2.6/nPYc/utilities/generic.py` & `nPYc-1.2.7/nPYc/utilities/generic.py`

 * *Files identical despite different names*

### Comparing `nPYc-1.2.6/nPYc/utilities/ms.py` & `nPYc-1.2.7/nPYc/utilities/ms.py`

 * *Files identical despite different names*

### Comparing `nPYc-1.2.6/nPYc/utilities/normalisation/__init__.py` & `nPYc-1.2.7/nPYc/utilities/normalisation/__init__.py`

 * *Files identical despite different names*

### Comparing `nPYc-1.2.6/nPYc/utilities/normalisation/_normaliserABC.py` & `nPYc-1.2.7/nPYc/utilities/normalisation/_normaliserABC.py`

 * *Files identical despite different names*

### Comparing `nPYc-1.2.6/nPYc/utilities/normalisation/_nullNormaliser.py` & `nPYc-1.2.7/nPYc/utilities/normalisation/_nullNormaliser.py`

 * *Files identical despite different names*

### Comparing `nPYc-1.2.6/nPYc/utilities/normalisation/_probabilisticQuotientNormaliser.py` & `nPYc-1.2.7/nPYc/utilities/normalisation/_probabilisticQuotientNormaliser.py`

 * *Files identical despite different names*

### Comparing `nPYc-1.2.6/nPYc/utilities/normalisation/_totalAreaNormaliser.py` & `nPYc-1.2.7/nPYc/utilities/normalisation/_totalAreaNormaliser.py`

 * *Files identical despite different names*

### Comparing `nPYc-1.2.6/nPYc.egg-info/PKG-INFO` & `nPYc-1.2.7/nPYc.egg-info/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,55 +1,58 @@
 Metadata-Version: 2.1
 Name: nPYc
-Version: 1.2.6
+Version: 1.2.7
 Summary: National Phenome Centre toolbox
 Home-page: https://github.com/phenomecentre/npyc-toolbox
 Author: National Phenome Centre
 Author-email: phenomecentre@imperial.ac.uk
 License: MIT
-Description: 		Toolbox for preprocessing of metabolic profiling datasets
-        		---------------------------------------------------------
-        
-        		.. image:: https://travis-ci.org/phenomecentre/nPYc-Toolbox.svg?branch=master
-        		   :target: https://travis-ci.org/phenomecentre/nPYc-Toolbox
-        		   :alt: Travis CI build status
-        
-        		.. image:: https://readthedocs.org/projects/npyc-toolbox/badge/?version=latest
-        		   :target: http://npyc-toolbox.readthedocs.io/en/latest/?badge=latest
-        		   :alt: Documentation Status
-        
-        		.. image:: https://codecov.io/gh/phenomecentre/nPYc-Toolbox/branch/master/graph/badge.svg
-        		   :target: https://codecov.io/gh/phenomecentre/nPYc-Toolbox
-        		   :alt: Test coverage
-        
-        		|
-        
-        		The nPYc toolbox offers functions for the import, preprocessing, and QC of metabolic profiling datasets.
-        
-        		Documentation can be found on `Read the Docs <http://npyc-toolbox.readthedocs.io/en/latest/?badge=latest>`_.
-        
-        		Imports
-        		 - Peak-picked LC-MS data (XCMS, Progenesis QI, *&* Metaboscape)
-        		 - Raw NMR spectra (Bruker format)
-        		 - Targeted datasets (TargetLynx, Bruker BI-LISA, *&* BI-Quant-Ur)
-        
-        		Provides
-        		 - Batch *&* drift correction for LC-MS datasets
-        		 - Feature filtering by RSD *&* linearity of response
-        		 - Calculation of spectral line-width in NMR
-        		 - PCA of datasets
-        		 - Visualisation of datasets
-        
-        		Exports
-        		 - Basic tabular csv
-        		 - `ISA-TAB <http://isa-tools.org>`_
-        
-        		The nPYc toolbox is `developed <https://github.com/phenomecentre/npyc-toolbox>`_ by the informatics team at `The National Phenome Centre <http://phenomecentre.org/>`_ at `Imperial College London <http://imperial.ac.uk/>`_.
-        		
 Platform: UNKNOWN
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Topic :: Scientific/Engineering :: Bio-Informatics
 Description-Content-Type: text/markdown
+License-File: LICENSE.md
+
+		Toolbox for preprocessing of metabolic profiling datasets
+		---------------------------------------------------------
+
+		.. image:: https://travis-ci.org/phenomecentre/nPYc-Toolbox.svg?branch=master
+		   :target: https://travis-ci.org/phenomecentre/nPYc-Toolbox
+		   :alt: Travis CI build status
+
+		.. image:: https://readthedocs.org/projects/npyc-toolbox/badge/?version=latest
+		   :target: http://npyc-toolbox.readthedocs.io/en/latest/?badge=latest
+		   :alt: Documentation Status
+
+		.. image:: https://codecov.io/gh/phenomecentre/nPYc-Toolbox/branch/master/graph/badge.svg
+		   :target: https://codecov.io/gh/phenomecentre/nPYc-Toolbox
+		   :alt: Test coverage
+
+		|
+
+		The nPYc toolbox offers functions for the import, preprocessing, and QC of metabolic profiling datasets.
+
+		Documentation can be found on `Read the Docs <http://npyc-toolbox.readthedocs.io/en/latest/?badge=latest>`_.
+
+		Imports
+		 - Peak-picked LC-MS data (XCMS, Progenesis QI, *&* Metaboscape)
+		 - Raw NMR spectra (Bruker format)
+		 - Targeted datasets (TargetLynx, Bruker BI-LISA, *&* BI-Quant-Ur)
+
+		Provides
+		 - Batch *&* drift correction for LC-MS datasets
+		 - Feature filtering by RSD *&* linearity of response
+		 - Calculation of spectral line-width in NMR
+		 - PCA of datasets
+		 - Visualisation of datasets
+
+		Exports
+		 - Basic tabular csv
+		 - `ISA-TAB <http://isa-tools.org>`_
+
+		The nPYc toolbox is `developed <https://github.com/phenomecentre/npyc-toolbox>`_ by the informatics team at `The National Phenome Centre <http://phenomecentre.org/>`_ at `Imperial College London <http://imperial.ac.uk/>`_.
+		
+
```

### Comparing `nPYc-1.2.6/nPYc.egg-info/SOURCES.txt` & `nPYc-1.2.7/nPYc.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `nPYc-1.2.6/setup.py` & `nPYc-1.2.7/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,28 +1,33 @@
 from setuptools import setup, find_packages
 
 setup(name='nPYc',
-	version='1.2.6',
+	version='1.2.7',
 	description='National Phenome Centre toolbox',
 	url='https://github.com/phenomecentre/npyc-toolbox',
 	author='National Phenome Centre',
 	author_email='phenomecentre@imperial.ac.uk',
 	license='MIT',
 	packages=find_packages(),
 	install_requires=[
 		'cycler>=0.10.0',
 		'iPython>=6.3.1',
-		'isaExplorer>=0.1',
-		'isatools>=0.9.3',
-		'Jinja2>=2.10',
+		#'isaExplorer>=0.1',
+		#'isatools>=0.9.3',
+		'Jinja2>=3.0.1',
 		'lmfit>=0.9.7',
-		'matplotlib>=2.2.2',
-		'networkx>=2.1',
-		'numpy>=1.14.2',
-		'pandas>=0.23.0',
+		#'markupsafe==2.0.1',
+		'matplotlib==3.5.2',
+		'networkx>=2.5.1',
+		#'numpy>=1.14.2',
+		#'pandas>=0.23.0',
+		'numpy~=1.23.3',
+		'openpyxl',
+        #'jsonschema~=3.2.0',
+        'pandas~=1.5.0',
 		'plotly>=3.1.0',
 		'pyChemometrics>=0.1',
 		'scikit-learn>=0.19.1',
 		'scipy>=1.1.0',
 		'seaborn>=0.8.1',
 		'setuptools>=39.1.0',
 		'statsmodels>=0.9.0'
```

