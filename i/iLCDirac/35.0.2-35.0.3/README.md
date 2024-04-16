# Comparing `tmp/iLCDirac-35.0.2.tar.gz` & `tmp/ilcdirac-35.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "iLCDirac-35.0.2.tar", last modified: Fri Mar 15 15:01:06 2024, max compression
+gzip compressed data, was "ilcdirac-35.0.3.tar", last modified: Tue Apr 16 15:47:28 2024, max compression
```

## Comparing `iLCDirac-35.0.2.tar` & `ilcdirac-35.0.3.tar`

### file list

```diff
@@ -1,481 +1,481 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-15 15:01:06.567158 iLCDirac-35.0.2/
--rw-rw-rw-   0 root         (0) root         (0)    32452 2024-03-15 15:00:47.000000 iLCDirac-35.0.2/LICENSE
--rw-rw-rw-   0 root         (0) root         (0)      142 2024-03-15 15:00:47.000000 iLCDirac-35.0.2/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     2175 2024-03-15 15:01:06.567158 iLCDirac-35.0.2/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)      241 2024-03-15 15:00:47.000000 iLCDirac-35.0.2/README.md
--rw-rw-rw-   0 root         (0) root         (0)      463 2024-03-15 15:00:47.000000 iLCDirac-35.0.2/pyproject.toml
--rw-rw-rw-   0 root         (0) root         (0)      361 2024-03-15 15:00:47.000000 iLCDirac-35.0.2/pytest.ini
--rw-rw-rw-   0 root         (0) root         (0)    85926 2024-03-15 15:00:47.000000 iLCDirac-35.0.2/release.notes
--rw-rw-rw-   0 root         (0) root         (0)    27753 2024-03-15 15:00:47.000000 iLCDirac-35.0.2/releases.cfg
--rw-rw-rw-   0 root         (0) root         (0)     4389 2024-03-15 15:01:06.569158 iLCDirac-35.0.2/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)      276 2024-03-15 15:00:47.000000 iLCDirac-35.0.2/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-15 15:01:06.451159 iLCDirac-35.0.2/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-15 15:01:06.454159 iLCDirac-35.0.2/src/ILCDIRAC/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-15 15:01:06.455159 iLCDirac-35.0.2/src/ILCDIRAC/CalibrationSystem/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-15 15:01:06.455159 iLCDirac-35.0.2/src/ILCDIRAC/CalibrationSystem/Agent/
--rw-rw-rw-   0 root         (0) root         (0)    10978 2024-03-15 15:00:47.000000 iLCDirac-35.0.2/src/ILCDIRAC/CalibrationSystem/Agent/CalibrationAgent.py
--rw-rw-rw-   0 root         (0) root         (0)     1013 2024-03-15 15:00:47.000000 iLCDirac-35.0.2/src/ILCDIRAC/CalibrationSystem/Agent/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-15 15:01:06.456159 iLCDirac-35.0.2/src/ILCDIRAC/CalibrationSystem/Client/
--rw-rw-rw-   0 root         (0) root         (0)     6343 2024-03-15 15:00:47.000000 iLCDirac-35.0.2/src/ILCDIRAC/CalibrationSystem/Client/CalibrationClient.py
--rw-rw-rw-   0 root         (0) root         (0)     1013 2024-03-15 15:00:47.000000 iLCDirac-35.0.2/src/ILCDIRAC/CalibrationSystem/Client/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      527 2024-03-15 15:00:47.000000 iLCDirac-35.0.2/src/ILCDIRAC/CalibrationSystem/ConfigTemplate.cfg
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-15 15:01:06.457159 iLCDirac-35.0.2/src/ILCDIRAC/CalibrationSystem/Service/
--rw-rw-rw-   0 root         (0) root         (0)    36181 2024-03-15 15:00:47.000000 iLCDirac-35.0.2/src/ILCDIRAC/CalibrationSystem/Service/CalibrationHandler.py
--rw-rw-rw-   0 root         (0) root         (0)    44494 2024-03-15 15:00:47.000000 iLCDirac-35.0.2/src/ILCDIRAC/CalibrationSystem/Service/CalibrationRun.py
--rw-rw-rw-   0 root         (0) root         (0)     5951 2024-03-15 15:00:47.000000 iLCDirac-35.0.2/src/ILCDIRAC/CalibrationSystem/Service/DetectorSettings.py
--rw-rw-rw-   0 root         (0) root         (0)     1013 2024-03-15 15:00:47.000000 iLCDirac-35.0.2/src/ILCDIRAC/CalibrationSystem/Service/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     3971 2024-03-15 15:00:47.000000 iLCDirac-35.0.2/src/ILCDIRAC/CalibrationSystem/TODO
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-15 15:01:06.459159 iLCDirac-35.0.2/src/ILCDIRAC/CalibrationSystem/Test/
--rw-rw-rw-   0 root         (0) root         (0)    14462 2024-03-15 15:00:47.000000 iLCDirac-35.0.2/src/ILCDIRAC/CalibrationSystem/Test/Test_CalibrationAgent.py
--rw-rw-rw-   0 root         (0) root         (0)     2255 2024-03-15 15:00:47.000000 iLCDirac-35.0.2/src/ILCDIRAC/CalibrationSystem/Test/Test_CalibrationClient.py
--rw-rw-rw-   0 root         (0) root         (0)    51085 2024-03-15 15:00:47.000000 iLCDirac-35.0.2/src/ILCDIRAC/CalibrationSystem/Test/Test_CalibrationService.py
--rw-rw-rw-   0 root         (0) root         (0)     2037 2024-03-15 15:00:47.000000 iLCDirac-35.0.2/src/ILCDIRAC/CalibrationSystem/Test/Test_Util_fileutils.py
--rw-rw-rw-   0 root         (0) root         (0)     9201 2024-03-15 15:00:47.000000 iLCDirac-35.0.2/src/ILCDIRAC/CalibrationSystem/Test/Test_Util_functions.py
--rw-rw-rw-   0 root         (0) root         (0)     1013 2024-03-15 15:00:47.000000 iLCDirac-35.0.2/src/ILCDIRAC/CalibrationSystem/Test/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-15 15:01:06.460159 iLCDirac-35.0.2/src/ILCDIRAC/CalibrationSystem/Utilities/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-15 15:01:06.463159 iLCDirac-35.0.2/src/ILCDIRAC/CalibrationSystem/Utilities/Python_Read_Scripts/
--rw-rw-rw-   0 root         (0) root         (0)     3152 2024-03-15 15:00:47.000000 iLCDirac-35.0.2/src/ILCDIRAC/CalibrationSystem/Utilities/Python_Read_Scripts/ECal_Digi_Extract.py
--rw-rw-rw-   0 root         (0) root         (0)     1811 2024-03-15 15:00:47.000000 iLCDirac-35.0.2/src/ILCDIRAC/CalibrationSystem/Utilities/Python_Read_Scripts/EM_Extract.py
--rw-rw-rw-   0 root         (0) root         (0)     1494 2024-03-15 15:00:47.000000 iLCDirac-35.0.2/src/ILCDIRAC/CalibrationSystem/Utilities/Python_Read_Scripts/Extract_GeVToMIP.py
--rw-rw-rw-   0 root         (0) root         (0)      945 2024-03-15 15:00:47.000000 iLCDirac-35.0.2/src/ILCDIRAC/CalibrationSystem/Utilities/Python_Read_Scripts/Extract_SimCaloHitMIPMPV.py
--rw-rw-rw-   0 root         (0) root         (0)     2867 2024-03-15 15:00:47.000000 iLCDirac-35.0.2/src/ILCDIRAC/CalibrationSystem/Utilities/Python_Read_Scripts/Final_Calibration.py
--rw-rw-rw-   0 root         (0) root         (0)     2682 2024-03-15 15:00:47.000000 iLCDirac-35.0.2/src/ILCDIRAC/CalibrationSystem/Utilities/Python_Read_Scripts/Final_Calibration.py.orig
--rw-rw-rw-   0 root         (0) root         (0)     2388 2024-03-15 15:00:47.000000 iLCDirac-35.0.2/src/ILCDIRAC/CalibrationSystem/Utilities/Python_Read_Scripts/HCal_Digi_Extract.py
--rw-rw-rw-   0 root         (0) root         (0)     1456 2024-03-15 15:00:47.000000 iLCDirac-35.0.2/src/ILCDIRAC/CalibrationSystem/Utilities/Python_Read_Scripts/HCal_Direction_Corrections_Extract.py
--rw-rw-rw-   0 root         (0) root         (0)     1487 2024-03-15 15:00:47.000000 iLCDirac-35.0.2/src/ILCDIRAC/CalibrationSystem/Utilities/Python_Read_Scripts/HCal_Ring_Digi_Extract.py
--rw-rw-rw-   0 root         (0) root         (0)     3967 2024-03-15 15:00:47.000000 iLCDirac-35.0.2/src/ILCDIRAC/CalibrationSystem/Utilities/Python_Read_Scripts/HCal_Ring_Gear_Information.py
--rw-rw-rw-   0 root         (0) root         (0)     4968 2024-03-15 15:00:47.000000 iLCDirac-35.0.2/src/ILCDIRAC/CalibrationSystem/Utilities/Python_Read_Scripts/Had_Extract.py
--rw-rw-rw-   0 root         (0) root         (0)      220 2024-03-15 15:00:47.000000 iLCDirac-35.0.2/src/ILCDIRAC/CalibrationSystem/Utilities/Python_Read_Scripts/Helper_Functions.py
--rw-rw-rw-   0 root         (0) root         (0)     3579 2024-03-15 15:00:47.000000 iLCDirac-35.0.2/src/ILCDIRAC/CalibrationSystem/Utilities/Python_Read_Scripts/Python_Read_Scripts.tgz
--rw-rw-rw-   0 root         (0) root         (0)     1013 2024-03-15 15:00:47.000000 iLCDirac-35.0.2/src/ILCDIRAC/CalibrationSystem/Utilities/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-15 15:01:06.464159 iLCDirac-35.0.2/src/ILCDIRAC/CalibrationSystem/Utilities/auxiliaryFiles/
--rw-rw-rw-   0 root         (0) root         (0)     1765 2024-03-15 15:00:47.000000 iLCDirac-35.0.2/src/ILCDIRAC/CalibrationSystem/Utilities/auxiliaryFiles/parameterListMarlinSteeringFile.txt
--rw-rw-rw-   0 root         (0) root         (0)     3928 2024-03-15 15:00:47.000000 iLCDirac-35.0.2/src/ILCDIRAC/CalibrationSystem/Utilities/auxiliaryFiles/pfoAnalysis.xml
--rw-rw-rw-   0 root         (0) root         (0)     1484 2024-03-15 15:00:47.000000 iLCDirac-35.0.2/src/ILCDIRAC/CalibrationSystem/Utilities/fileutils.py
--rw-rw-rw-   0 root         (0) root         (0)    12301 2024-03-15 15:00:47.000000 iLCDirac-35.0.2/src/ILCDIRAC/CalibrationSystem/Utilities/functions.py
--rw-rw-rw-   0 root         (0) root         (0)     4433 2024-03-15 15:00:47.000000 iLCDirac-35.0.2/src/ILCDIRAC/CalibrationSystem/Utilities/mergePandoraLikelihoodData.py
--rw-rw-rw-   0 root         (0) root         (0)     1668 2024-03-15 15:00:47.000000 iLCDirac-35.0.2/src/ILCDIRAC/CalibrationSystem/Utilities/objectFactory.py
--rw-rw-rw-   0 root         (0) root         (0)     1013 2024-03-15 15:00:47.000000 iLCDirac-35.0.2/src/ILCDIRAC/CalibrationSystem/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     2943 2024-03-15 15:00:47.000000 iLCDirac-35.0.2/src/ILCDIRAC/CalibrationSystem/dev_create_events.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-15 15:01:06.464159 iLCDirac-35.0.2/src/ILCDIRAC/Core/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-15 15:01:06.472159 iLCDirac-35.0.2/src/ILCDIRAC/Core/Utilities/
--rw-rw-rw-   0 root         (0) root         (0)     3755 2024-03-15 15:00:47.000000 iLCDirac-35.0.2/src/ILCDIRAC/Core/Utilities/CheckAndGetProdProxy.py
--rw-rw-rw-   0 root         (0) root         (0)     1767 2024-03-15 15:00:47.000000 iLCDirac-35.0.2/src/ILCDIRAC/Core/Utilities/CheckXMLValidity.py
--rw-rw-rw-   0 root         (0) root         (0)    15260 2024-03-15 15:00:47.000000 iLCDirac-35.0.2/src/ILCDIRAC/Core/Utilities/CombinedSoftwareInstallation.py
--rw-rw-rw-   0 root         (0) root         (0)     1903 2024-03-15 15:00:47.000000 iLCDirac-35.0.2/src/ILCDIRAC/Core/Utilities/Configuration.py
--rw-rw-rw-   0 root         (0) root         (0)    18781 2024-03-15 15:00:47.000000 iLCDirac-35.0.2/src/ILCDIRAC/Core/Utilities/DetectOS.py
--rw-rw-rw-   0 root         (0) root         (0)     4861 2024-03-15 15:00:47.000000 iLCDirac-35.0.2/src/ILCDIRAC/Core/Utilities/FileUtils.py
--rw-rw-rw-   0 root         (0) root         (0)     9749 2024-03-15 15:00:47.000000 iLCDirac-35.0.2/src/ILCDIRAC/Core/Utilities/FilenameEncoder.py
--rw-rw-rw-   0 root         (0) root         (0)     2767 2024-03-15 15:00:47.000000 iLCDirac-35.0.2/src/ILCDIRAC/Core/Utilities/FindSteeringFileDir.py
--rw-rw-rw-   0 root         (0) root         (0)     4110 2024-03-15 15:00:47.000000 iLCDirac-35.0.2/src/ILCDIRAC/Core/Utilities/GeneratorModels.py
--rw-rw-rw-   0 root         (0) root         (0)    17917 2024-03-15 15:00:47.000000 iLCDirac-35.0.2/src/ILCDIRAC/Core/Utilities/HTML.py
--rw-rw-rw-   0 root         (0) root         (0)     6866 2024-03-15 15:00:47.000000 iLCDirac-35.0.2/src/ILCDIRAC/Core/Utilities/InputDataResolution.py
--rw-rw-rw-   0 root         (0) root         (0)     4246 2024-03-15 15:00:47.000000 iLCDirac-35.0.2/src/ILCDIRAC/Core/Utilities/InputFilesUtilities.py
--rw-rw-rw-   0 root         (0) root         (0)     5535 2024-03-15 15:00:47.000000 iLCDirac-35.0.2/src/ILCDIRAC/Core/Utilities/InstalledFiles.py
--rw-rw-rw-   0 root         (0) root         (0)     2805 2024-03-15 15:00:47.000000 iLCDirac-35.0.2/src/ILCDIRAC/Core/Utilities/JobPathResolution.py
--rw-rw-rw-   0 root         (0) root         (0)     2311 2024-03-15 15:00:47.000000 iLCDirac-35.0.2/src/ILCDIRAC/Core/Utilities/LFNPathUtilities.py
--rw-rw-rw-   0 root         (0) root         (0)     7040 2024-03-15 15:00:47.000000 iLCDirac-35.0.2/src/ILCDIRAC/Core/Utilities/MarlinXML.py
--rw-rw-rw-   0 root         (0) root         (0)     3285 2024-03-15 15:00:47.000000 iLCDirac-35.0.2/src/ILCDIRAC/Core/Utilities/OutputDataPolicy.py
--rw-rw-rw-   0 root         (0) root         (0)     3601 2024-03-15 15:00:47.000000 iLCDirac-35.0.2/src/ILCDIRAC/Core/Utilities/OverlayFiles.py
--rw-rw-rw-   0 root         (0) root         (0)     2856 2024-03-15 15:00:47.000000 iLCDirac-35.0.2/src/ILCDIRAC/Core/Utilities/PrepareLibs.py
--rw-rw-rw-   0 root         (0) root         (0)    38627 2024-03-15 15:00:47.000000 iLCDirac-35.0.2/src/ILCDIRAC/Core/Utilities/PrepareOptionFiles.py
--rw-rw-rw-   0 root         (0) root         (0)     7483 2024-03-15 15:00:47.000000 iLCDirac-35.0.2/src/ILCDIRAC/Core/Utilities/ProcessList.py
--rw-rw-rw-   0 root         (0) root         (0)    11004 2024-03-15 15:00:47.000000 iLCDirac-35.0.2/src/ILCDIRAC/Core/Utilities/ProductionData.py
--rw-rw-rw-   0 root         (0) root         (0)     3993 2024-03-15 15:00:47.000000 iLCDirac-35.0.2/src/ILCDIRAC/Core/Utilities/RemoveSoft.py
--rw-rw-rw-   0 root         (0) root         (0)     2690 2024-03-15 15:00:47.000000 iLCDirac-35.0.2/src/ILCDIRAC/Core/Utilities/ResolveDependencies.py
--rw-rw-rw-   0 root         (0) root         (0)     4689 2024-03-15 15:00:47.000000 iLCDirac-35.0.2/src/ILCDIRAC/Core/Utilities/ResolveSE.py
--rw-rw-rw-   0 root         (0) root         (0)     1804 2024-03-15 15:00:47.000000 iLCDirac-35.0.2/src/ILCDIRAC/Core/Utilities/Splitting.py
--rw-rw-rw-   0 root         (0) root         (0)    21977 2024-03-15 15:00:47.000000 iLCDirac-35.0.2/src/ILCDIRAC/Core/Utilities/TARsoft.py
--rw-rw-rw-   0 root         (0) root         (0)     2868 2024-03-15 15:00:47.000000 iLCDirac-35.0.2/src/ILCDIRAC/Core/Utilities/Utilities.py
--rw-rw-rw-   0 root         (0) root         (0)     1898 2024-03-15 15:00:47.000000 iLCDirac-35.0.2/src/ILCDIRAC/Core/Utilities/WasteCPU.py
--rw-rw-rw-   0 root         (0) root         (0)    41912 2024-03-15 15:00:47.000000 iLCDirac-35.0.2/src/ILCDIRAC/Core/Utilities/WhizardOptions.py
--rw-rw-rw-   0 root         (0) root         (0)     1100 2024-03-15 15:00:47.000000 iLCDirac-35.0.2/src/ILCDIRAC/Core/Utilities/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     6604 2024-03-15 15:00:47.000000 iLCDirac-35.0.2/src/ILCDIRAC/Core/Utilities/resolvePathsAndNames.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-15 15:01:06.478159 iLCDirac-35.0.2/src/ILCDIRAC/Core/Utilities/tests/
--rw-rw-rw-   0 root         (0) root         (0)     6226 2024-03-15 15:00:47.000000 iLCDirac-35.0.2/src/ILCDIRAC/Core/Utilities/tests/Test_CheckAndGetProd.py
--rw-rw-rw-   0 root         (0) root         (0)    32396 2024-03-15 15:00:47.000000 iLCDirac-35.0.2/src/ILCDIRAC/Core/Utilities/tests/Test_CombinedSoftwareInstallation.py
--rw-rw-rw-   0 root         (0) root         (0)     2440 2024-03-15 15:00:47.000000 iLCDirac-35.0.2/src/ILCDIRAC/Core/Utilities/tests/Test_Configuration.py
--rw-rw-rw-   0 root         (0) root         (0)    23878 2024-03-15 15:00:47.000000 iLCDirac-35.0.2/src/ILCDIRAC/Core/Utilities/tests/Test_DetectOS.py
--rw-rw-rw-   0 root         (0) root         (0)    17273 2024-03-15 15:00:47.000000 iLCDirac-35.0.2/src/ILCDIRAC/Core/Utilities/tests/Test_FileUtils.py
--rw-rw-rw-   0 root         (0) root         (0)    16707 2024-03-15 15:00:47.000000 iLCDirac-35.0.2/src/ILCDIRAC/Core/Utilities/tests/Test_FilenameEncoder.py
--rw-rw-rw-   0 root         (0) root         (0)     4872 2024-03-15 15:00:47.000000 iLCDirac-35.0.2/src/ILCDIRAC/Core/Utilities/tests/Test_FindSteeringFileDir.py
--rw-rw-rw-   0 root         (0) root         (0)    10164 2024-03-15 15:00:47.000000 iLCDirac-35.0.2/src/ILCDIRAC/Core/Utilities/tests/Test_InputDataResolution.py
--rw-rw-rw-   0 root         (0) root         (0)     7506 2024-03-15 15:00:47.000000 iLCDirac-35.0.2/src/ILCDIRAC/Core/Utilities/tests/Test_InputFilesUtilities.py
--rw-rw-rw-   0 root         (0) root         (0)     2277 2024-03-15 15:00:47.000000 iLCDirac-35.0.2/src/ILCDIRAC/Core/Utilities/tests/Test_LFNPathUtilities.py
--rw-rw-rw-   0 root         (0) root         (0)    18959 2024-03-15 15:00:47.000000 iLCDirac-35.0.2/src/ILCDIRAC/Core/Utilities/tests/Test_OutputDataPolicy.py
--rw-rw-rw-   0 root         (0) root         (0)     2654 2024-03-15 15:00:47.000000 iLCDirac-35.0.2/src/ILCDIRAC/Core/Utilities/tests/Test_OverlayFiles.py
--rw-rw-rw-   0 root         (0) root         (0)     6803 2024-03-15 15:00:47.000000 iLCDirac-35.0.2/src/ILCDIRAC/Core/Utilities/tests/Test_PrepareLibs.py
--rw-rw-rw-   0 root         (0) root         (0)    26585 2024-03-15 15:00:47.000000 iLCDirac-35.0.2/src/ILCDIRAC/Core/Utilities/tests/Test_PrepareMarlinXML.py
--rw-rw-rw-   0 root         (0) root         (0)    86014 2024-03-15 15:00:47.000000 iLCDirac-35.0.2/src/ILCDIRAC/Core/Utilities/tests/Test_PrepareOptionsFiles.py
--rw-rw-rw-   0 root         (0) root         (0)    14816 2024-03-15 15:00:47.000000 iLCDirac-35.0.2/src/ILCDIRAC/Core/Utilities/tests/Test_ProcessList.py
--rw-rw-rw-   0 root         (0) root         (0)     6220 2024-03-15 15:00:47.000000 iLCDirac-35.0.2/src/ILCDIRAC/Core/Utilities/tests/Test_ProductionData.py
--rw-rw-rw-   0 root         (0) root         (0)     4230 2024-03-15 15:00:47.000000 iLCDirac-35.0.2/src/ILCDIRAC/Core/Utilities/tests/Test_ProductionOutputData.py
--rw-rw-rw-   0 root         (0) root         (0)    11294 2024-03-15 15:00:47.000000 iLCDirac-35.0.2/src/ILCDIRAC/Core/Utilities/tests/Test_ResolvePathsandNames.py
--rw-rw-rw-   0 root         (0) root         (0)     9475 2024-03-15 15:00:47.000000 iLCDirac-35.0.2/src/ILCDIRAC/Core/Utilities/tests/Test_ResolveSEs.py
--rw-rw-rw-   0 root         (0) root         (0)     2278 2024-03-15 15:00:47.000000 iLCDirac-35.0.2/src/ILCDIRAC/Core/Utilities/tests/Test_Splitting.py
--rw-rw-rw-   0 root         (0) root         (0)    72966 2024-03-15 15:00:47.000000 iLCDirac-35.0.2/src/ILCDIRAC/Core/Utilities/tests/Test_TARsoft.py
--rw-rw-rw-   0 root         (0) root         (0)     3214 2024-03-15 15:00:47.000000 iLCDirac-35.0.2/src/ILCDIRAC/Core/Utilities/tests/Test_Utilities.py
--rw-rw-rw-   0 root         (0) root         (0)     2480 2024-03-15 15:00:47.000000 iLCDirac-35.0.2/src/ILCDIRAC/Core/Utilities/tests/Test_WasteCPU.py
--rw-rw-rw-   0 root         (0) root         (0)    26730 2024-03-15 15:00:47.000000 iLCDirac-35.0.2/src/ILCDIRAC/Core/Utilities/tests/Test_WhizardOptions.py
--rw-rw-rw-   0 root         (0) root         (0)     1180 2024-03-15 15:00:47.000000 iLCDirac-35.0.2/src/ILCDIRAC/Core/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-15 15:01:06.482159 iLCDirac-35.0.2/src/ILCDIRAC/Core/scripts/
--rw-rw-rw-   0 root         (0) root         (0)     1086 2024-03-15 15:00:47.000000 iLCDirac-35.0.2/src/ILCDIRAC/Core/scripts/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     2720 2024-03-15 15:00:47.000000 iLCDirac-35.0.2/src/ILCDIRAC/Core/scripts/createJavaTarBall.sh
--rwxrwxrwx   0 root         (0) root         (0)     3224 2024-03-15 15:00:47.000000 iLCDirac-35.0.2/src/ILCDIRAC/Core/scripts/createLCIOTarBall.sh
--rwxrwxrwx   0 root         (0) root         (0)     6151 2024-03-15 15:00:47.000000 iLCDirac-35.0.2/src/ILCDIRAC/Core/scripts/createMarlinTarBall.sh
--rwxrwxrwx   0 root         (0) root         (0)     6706 2024-03-15 15:00:47.000000 iLCDirac-35.0.2/src/ILCDIRAC/Core/scripts/createMokkaTarBall.sh
--rwxrwxrwx   0 root         (0) root         (0)     3200 2024-03-15 15:00:47.000000 iLCDirac-35.0.2/src/ILCDIRAC/Core/scripts/createSlicPandoraTarBall.sh
--rwxrwxrwx   0 root         (0) root         (0)     2307 2024-03-15 15:00:47.000000 iLCDirac-35.0.2/src/ILCDIRAC/Core/scripts/createTarBallForProgram.sh
--rwxrwxrwx   0 root         (0) root         (0)     9197 2024-03-15 15:00:47.000000 iLCDirac-35.0.2/src/ILCDIRAC/Core/scripts/dirac-architecture
--rw-rw-rw-   0 root         (0) root         (0)    16949 2024-03-15 15:00:47.000000 iLCDirac-35.0.2/src/ILCDIRAC/Core/scripts/dirac_ilc_add_cvmfs_software.py
--rw-rw-rw-   0 root         (0) root         (0)    10488 2024-03-15 15:00:47.000000 iLCDirac-35.0.2/src/ILCDIRAC/Core/scripts/dirac_ilc_add_software.py
--rw-rw-rw-   0 root         (0) root         (0)     9764 2024-03-15 15:00:47.000000 iLCDirac-35.0.2/src/ILCDIRAC/Core/scripts/dirac_ilc_add_user.py
--rw-rw-rw-   0 root         (0) root         (0)    16381 2024-03-15 15:00:47.000000 iLCDirac-35.0.2/src/ILCDIRAC/Core/scripts/dirac_ilc_add_whizard.py
--rw-rw-rw-   0 root         (0) root         (0)     3905 2024-03-15 15:00:47.000000 iLCDirac-35.0.2/src/ILCDIRAC/Core/scripts/dirac_ilc_list_users.py
--rw-rw-rw-   0 root         (0) root         (0)     1573 2024-03-15 15:00:47.000000 iLCDirac-35.0.2/src/ILCDIRAC/Core/scripts/ilcdirac-install.sh
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-15 15:01:06.482159 iLCDirac-35.0.2/src/ILCDIRAC/DataManagementSystem/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-15 15:01:06.483158 iLCDirac-35.0.2/src/ILCDIRAC/DataManagementSystem/Agent/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-15 15:01:06.483158 iLCDirac-35.0.2/src/ILCDIRAC/DataManagementSystem/Agent/RequestOperations/
--rw-rw-rw-   0 root         (0) root         (0)     4676 2024-03-15 15:00:47.000000 iLCDirac-35.0.2/src/ILCDIRAC/DataManagementSystem/Agent/RequestOperations/LogUpload.py
--rw-rw-rw-   0 root         (0) root         (0)     1115 2024-03-15 15:00:47.000000 iLCDirac-35.0.2/src/ILCDIRAC/DataManagementSystem/Agent/RequestOperations/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1103 2024-03-15 15:00:47.000000 iLCDirac-35.0.2/src/ILCDIRAC/DataManagementSystem/Agent/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1108 2024-03-15 15:00:47.000000 iLCDirac-35.0.2/src/ILCDIRAC/DataManagementSystem/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-15 15:01:06.484159 iLCDirac-35.0.2/src/ILCDIRAC/FrameworkSystem/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-15 15:01:06.484159 iLCDirac-35.0.2/src/ILCDIRAC/FrameworkSystem/Agent/
--rw-rw-rw-   0 root         (0) root         (0)     1013 2024-03-15 15:00:47.000000 iLCDirac-35.0.2/src/ILCDIRAC/FrameworkSystem/Agent/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)       11 2024-03-15 15:00:47.000000 iLCDirac-35.0.2/src/ILCDIRAC/FrameworkSystem/ConfigTemplate.cfg
--rw-rw-rw-   0 root         (0) root         (0)     1013 2024-03-15 15:00:47.000000 iLCDirac-35.0.2/src/ILCDIRAC/FrameworkSystem/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-15 15:01:06.485159 iLCDirac-35.0.2/src/ILCDIRAC/ILCTransformationSystem/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-15 15:01:06.486158 iLCDirac-35.0.2/src/ILCDIRAC/ILCTransformationSystem/Agent/
--rw-rw-rw-   0 root         (0) root         (0)    25777 2024-03-15 15:00:47.000000 iLCDirac-35.0.2/src/ILCDIRAC/ILCTransformationSystem/Agent/FileStatusTransformationAgent.py
--rw-rw-rw-   0 root         (0) root         (0)     9996 2024-03-15 15:00:47.000000 iLCDirac-35.0.2/src/ILCDIRAC/ILCTransformationSystem/Agent/TarTheLogsAgent.py
--rw-rw-rw-   0 root         (0) root         (0)     5395 2024-03-15 15:00:47.000000 iLCDirac-35.0.2/src/ILCDIRAC/ILCTransformationSystem/Agent/TransformationPlugin.py
--rw-rw-rw-   0 root         (0) root         (0)     1072 2024-03-15 15:00:47.000000 iLCDirac-35.0.2/src/ILCDIRAC/ILCTransformationSystem/Agent/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-15 15:01:06.486158 iLCDirac-35.0.2/src/ILCDIRAC/ILCTransformationSystem/Client/
--rw-rw-rw-   0 root         (0) root         (0)     1934 2024-03-15 15:00:47.000000 iLCDirac-35.0.2/src/ILCDIRAC/ILCTransformationSystem/Client/Transformation.py
--rw-rw-rw-   0 root         (0) root         (0)     1079 2024-03-15 15:00:47.000000 iLCDirac-35.0.2/src/ILCDIRAC/ILCTransformationSystem/Client/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      441 2024-03-15 15:00:47.000000 iLCDirac-35.0.2/src/ILCDIRAC/ILCTransformationSystem/ConfigTemplate.cfg
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-15 15:01:06.488159 iLCDirac-35.0.2/src/ILCDIRAC/ILCTransformationSystem/Tests/
--rw-rw-rw-   0 root         (0) root         (0)    35437 2024-03-15 15:00:47.000000 iLCDirac-35.0.2/src/ILCDIRAC/ILCTransformationSystem/Tests/Test_FileStatusTransformationAgent.py
--rw-rw-rw-   0 root         (0) root         (0)    14308 2024-03-15 15:00:47.000000 iLCDirac-35.0.2/src/ILCDIRAC/ILCTransformationSystem/Tests/Test_ReleaseHelper.py
--rw-rw-rw-   0 root         (0) root         (0)    19604 2024-03-15 15:00:47.000000 iLCDirac-35.0.2/src/ILCDIRAC/ILCTransformationSystem/Tests/Test_TransformationPlugin.py
--rw-rw-rw-   0 root         (0) root         (0)    13782 2024-03-15 15:00:47.000000 iLCDirac-35.0.2/src/ILCDIRAC/ILCTransformationSystem/Tests/Test_createMovingTransformation.py
--rw-rw-rw-   0 root         (0) root         (0)    30921 2024-03-15 15:00:47.000000 iLCDirac-35.0.2/src/ILCDIRAC/ILCTransformationSystem/Tests/Test_diracClicMakeProductions.py
--rw-rw-rw-   0 root         (0) root         (0)    28121 2024-03-15 15:00:47.000000 iLCDirac-35.0.2/src/ILCDIRAC/ILCTransformationSystem/Tests/Test_diracFccMakeProductions.py
--rw-rw-rw-   0 root         (0) root         (0)     7554 2024-03-15 15:00:47.000000 iLCDirac-35.0.2/src/ILCDIRAC/ILCTransformationSystem/Tests/test_diracIlcAddTasks.py
--rw-rw-rw-   0 root         (0) root         (0)     2889 2024-03-15 15:00:47.000000 iLCDirac-35.0.2/src/ILCDIRAC/ILCTransformationSystem/Tests/test_utilities.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-15 15:01:06.489158 iLCDirac-35.0.2/src/ILCDIRAC/ILCTransformationSystem/Utilities/
--rw-rw-rw-   0 root         (0) root         (0)     5456 2024-03-15 15:00:47.000000 iLCDirac-35.0.2/src/ILCDIRAC/ILCTransformationSystem/Utilities/DataParameters.py
--rw-rw-rw-   0 root         (0) root         (0)     6462 2024-03-15 15:00:47.000000 iLCDirac-35.0.2/src/ILCDIRAC/ILCTransformationSystem/Utilities/ReleaseHelper.py
--rw-rw-rw-   0 root         (0) root         (0)     3263 2024-03-15 15:00:47.000000 iLCDirac-35.0.2/src/ILCDIRAC/ILCTransformationSystem/Utilities/Utilities.py
--rw-rw-rw-   0 root         (0) root         (0)     1074 2024-03-15 15:00:47.000000 iLCDirac-35.0.2/src/ILCDIRAC/ILCTransformationSystem/Utilities/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1071 2024-03-15 15:00:47.000000 iLCDirac-35.0.2/src/ILCDIRAC/ILCTransformationSystem/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-15 15:01:06.493158 iLCDirac-35.0.2/src/ILCDIRAC/ILCTransformationSystem/scripts/
--rw-rw-rw-   0 root         (0) root         (0)     1075 2024-03-15 15:00:47.000000 iLCDirac-35.0.2/src/ILCDIRAC/ILCTransformationSystem/scripts/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    49305 2024-03-15 15:00:47.000000 iLCDirac-35.0.2/src/ILCDIRAC/ILCTransformationSystem/scripts/dirac_clic_make_productions.py
--rw-rw-rw-   0 root         (0) root         (0)    49823 2024-03-15 15:00:47.000000 iLCDirac-35.0.2/src/ILCDIRAC/ILCTransformationSystem/scripts/dirac_fcc_make_productions.py
--rw-rw-rw-   0 root         (0) root         (0)     6173 2024-03-15 15:00:47.000000 iLCDirac-35.0.2/src/ILCDIRAC/ILCTransformationSystem/scripts/dirac_ilc_add_tasks_to_prod.py
--rw-rw-rw-   0 root         (0) root         (0)     3311 2024-03-15 15:00:47.000000 iLCDirac-35.0.2/src/ILCDIRAC/ILCTransformationSystem/scripts/dirac_ilc_filestatus_transformation.py
--rw-rw-rw-   0 root         (0) root         (0)    13681 2024-03-15 15:00:47.000000 iLCDirac-35.0.2/src/ILCDIRAC/ILCTransformationSystem/scripts/dirac_ilc_get_info.py
--rw-rw-rw-   0 root         (0) root         (0)     7259 2024-03-15 15:00:47.000000 iLCDirac-35.0.2/src/ILCDIRAC/ILCTransformationSystem/scripts/dirac_ilc_get_prod_log.py
--rwxrwxrwx   0 root         (0) root         (0)     9899 2024-03-15 15:00:47.000000 iLCDirac-35.0.2/src/ILCDIRAC/ILCTransformationSystem/scripts/dirac_ilc_make_ddsimtarball.py
--rw-rw-rw-   0 root         (0) root         (0)     4618 2024-03-15 15:00:47.000000 iLCDirac-35.0.2/src/ILCDIRAC/ILCTransformationSystem/scripts/dirac_ilc_moving_transformation.py
--rw-rw-rw-   0 root         (0) root         (0)    18138 2024-03-15 15:00:47.000000 iLCDirac-35.0.2/src/ILCDIRAC/ILCTransformationSystem/scripts/dirac_ilc_production_summary.py
--rw-rw-rw-   0 root         (0) root         (0)     3481 2024-03-15 15:00:47.000000 iLCDirac-35.0.2/src/ILCDIRAC/ILCTransformationSystem/scripts/dirac_ilc_replication_transformation.py
--rw-rw-rw-   0 root         (0) root         (0)    12061 2024-03-15 15:00:47.000000 iLCDirac-35.0.2/src/ILCDIRAC/ILCTransformationSystem/scripts/dirac_ilc_upload_gen_files.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-15 15:01:06.493158 iLCDirac-35.0.2/src/ILCDIRAC/Interfaces/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-15 15:01:06.493158 iLCDirac-35.0.2/src/ILCDIRAC/Interfaces/API/
--rw-rw-rw-   0 root         (0) root         (0)    13839 2024-03-15 15:00:47.000000 iLCDirac-35.0.2/src/ILCDIRAC/Interfaces/API/DiracILC.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-15 15:01:06.448159 iLCDirac-35.0.2/src/ILCDIRAC/Interfaces/API/Examples/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-15 15:01:06.494158 iLCDirac-35.0.2/src/ILCDIRAC/Interfaces/API/Examples/SIDChain/
--rw-rw-rw-   0 root         (0) root         (0)       77 2024-03-15 15:00:47.000000 iLCDirac-35.0.2/src/ILCDIRAC/Interfaces/API/Examples/SIDChain/alias.properties
--rw-rw-rw-   0 root         (0) root         (0)     1890 2024-03-15 15:00:47.000000 iLCDirac-35.0.2/src/ILCDIRAC/Interfaces/API/Examples/SIDChain/bannedSites.py
--rw-rw-rw-   0 root         (0) root         (0)     9474 2024-03-15 15:00:47.000000 iLCDirac-35.0.2/src/ILCDIRAC/Interfaces/API/Examples/SIDChain/defaultPrePandoraLcsim.xml
--rw-rw-rw-   0 root         (0) root         (0)    10942 2024-03-15 15:00:47.000000 iLCDirac-35.0.2/src/ILCDIRAC/Interfaces/API/Examples/SIDChain/defaultPrePandoraLcsimOverlay.xml
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-15 15:01:06.495159 iLCDirac-35.0.2/src/ILCDIRAC/Interfaces/API/Examples/SIDChain/fileLists/
--rw-rw-rw-   0 root         (0) root         (0)     1202 2024-03-15 15:00:47.000000 iLCDirac-35.0.2/src/ILCDIRAC/Interfaces/API/Examples/SIDChain/fileLists/testSimList.py
--rw-rw-rw-   0 root         (0) root         (0)     1196 2024-03-15 15:00:47.000000 iLCDirac-35.0.2/src/ILCDIRAC/Interfaces/API/Examples/SIDChain/fileLists/testStdhepList.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-15 15:01:06.507158 iLCDirac-35.0.2/src/ILCDIRAC/Interfaces/API/Examples/SIDChain/slicMacros/
--rw-rw-rw-   0 root         (0) root         (0)       42 2024-03-15 15:00:47.000000 iLCDirac-35.0.2/src/ILCDIRAC/Interfaces/API/Examples/SIDChain/slicMacros/default.mac
--rw-rw-rw-   0 root         (0) root         (0)       80 2024-03-15 15:00:47.000000 iLCDirac-35.0.2/src/ILCDIRAC/Interfaces/API/Examples/SIDChain/slicMacros/defaultClicCrossingAngle.mac
--rw-rw-rw-   0 root         (0) root         (0)      324 2024-03-15 15:00:47.000000 iLCDirac-35.0.2/src/ILCDIRAC/Interfaces/API/Examples/SIDChain/slicMacros/e-_100gev_theta5-175.mac
--rw-rw-rw-   0 root         (0) root         (0)      323 2024-03-15 15:00:47.000000 iLCDirac-35.0.2/src/ILCDIRAC/Interfaces/API/Examples/SIDChain/slicMacros/e-_10gev_theta5-175.mac
--rw-rw-rw-   0 root         (0) root         (0)      327 2024-03-15 15:00:47.000000 iLCDirac-35.0.2/src/ILCDIRAC/Interfaces/API/Examples/SIDChain/slicMacros/gamma_100gev_theta5-175.mac
--rw-rw-rw-   0 root         (0) root         (0)      326 2024-03-15 15:00:47.000000 iLCDirac-35.0.2/src/ILCDIRAC/Interfaces/API/Examples/SIDChain/slicMacros/gamma_10gev_theta5-175.mac
--rw-rw-rw-   0 root         (0) root         (0)      325 2024-03-15 15:00:47.000000 iLCDirac-35.0.2/src/ILCDIRAC/Interfaces/API/Examples/SIDChain/slicMacros/mu-_100gev_theta10.mac
--rw-rw-rw-   0 root         (0) root         (0)      325 2024-03-15 15:00:47.000000 iLCDirac-35.0.2/src/ILCDIRAC/Interfaces/API/Examples/SIDChain/slicMacros/mu-_100gev_theta20.mac
--rw-rw-rw-   0 root         (0) root         (0)      325 2024-03-15 15:00:47.000000 iLCDirac-35.0.2/src/ILCDIRAC/Interfaces/API/Examples/SIDChain/slicMacros/mu-_100gev_theta30.mac
--rw-rw-rw-   0 root         (0) root         (0)      325 2024-03-15 15:00:47.000000 iLCDirac-35.0.2/src/ILCDIRAC/Interfaces/API/Examples/SIDChain/slicMacros/mu-_100gev_theta40.mac
--rw-rw-rw-   0 root         (0) root         (0)      325 2024-03-15 15:00:47.000000 iLCDirac-35.0.2/src/ILCDIRAC/Interfaces/API/Examples/SIDChain/slicMacros/mu-_100gev_theta5-175.mac
--rw-rw-rw-   0 root         (0) root         (0)      325 2024-03-15 15:00:47.000000 iLCDirac-35.0.2/src/ILCDIRAC/Interfaces/API/Examples/SIDChain/slicMacros/mu-_100gev_theta50.mac
--rw-rw-rw-   0 root         (0) root         (0)      325 2024-03-15 15:00:47.000000 iLCDirac-35.0.2/src/ILCDIRAC/Interfaces/API/Examples/SIDChain/slicMacros/mu-_100gev_theta60.mac
--rw-rw-rw-   0 root         (0) root         (0)      325 2024-03-15 15:00:47.000000 iLCDirac-35.0.2/src/ILCDIRAC/Interfaces/API/Examples/SIDChain/slicMacros/mu-_100gev_theta70.mac
--rw-rw-rw-   0 root         (0) root         (0)      325 2024-03-15 15:00:47.000000 iLCDirac-35.0.2/src/ILCDIRAC/Interfaces/API/Examples/SIDChain/slicMacros/mu-_100gev_theta80.mac
--rw-rw-rw-   0 root         (0) root         (0)      325 2024-03-15 15:00:47.000000 iLCDirac-35.0.2/src/ILCDIRAC/Interfaces/API/Examples/SIDChain/slicMacros/mu-_100gev_theta90.mac
--rw-rw-rw-   0 root         (0) root         (0)      324 2024-03-15 15:00:47.000000 iLCDirac-35.0.2/src/ILCDIRAC/Interfaces/API/Examples/SIDChain/slicMacros/mu-_10gev_theta10.mac
--rw-rw-rw-   0 root         (0) root         (0)      324 2024-03-15 15:00:47.000000 iLCDirac-35.0.2/src/ILCDIRAC/Interfaces/API/Examples/SIDChain/slicMacros/mu-_10gev_theta20.mac
--rw-rw-rw-   0 root         (0) root         (0)      324 2024-03-15 15:00:47.000000 iLCDirac-35.0.2/src/ILCDIRAC/Interfaces/API/Examples/SIDChain/slicMacros/mu-_10gev_theta30.mac
--rw-rw-rw-   0 root         (0) root         (0)      324 2024-03-15 15:00:47.000000 iLCDirac-35.0.2/src/ILCDIRAC/Interfaces/API/Examples/SIDChain/slicMacros/mu-_10gev_theta40.mac
--rw-rw-rw-   0 root         (0) root         (0)      324 2024-03-15 15:00:47.000000 iLCDirac-35.0.2/src/ILCDIRAC/Interfaces/API/Examples/SIDChain/slicMacros/mu-_10gev_theta5-175.mac
--rw-rw-rw-   0 root         (0) root         (0)      324 2024-03-15 15:00:47.000000 iLCDirac-35.0.2/src/ILCDIRAC/Interfaces/API/Examples/SIDChain/slicMacros/mu-_10gev_theta50.mac
--rw-rw-rw-   0 root         (0) root         (0)      324 2024-03-15 15:00:47.000000 iLCDirac-35.0.2/src/ILCDIRAC/Interfaces/API/Examples/SIDChain/slicMacros/mu-_10gev_theta60.mac
--rw-rw-rw-   0 root         (0) root         (0)      324 2024-03-15 15:00:47.000000 iLCDirac-35.0.2/src/ILCDIRAC/Interfaces/API/Examples/SIDChain/slicMacros/mu-_10gev_theta70.mac
--rw-rw-rw-   0 root         (0) root         (0)      324 2024-03-15 15:00:47.000000 iLCDirac-35.0.2/src/ILCDIRAC/Interfaces/API/Examples/SIDChain/slicMacros/mu-_10gev_theta80.mac
--rw-rw-rw-   0 root         (0) root         (0)      324 2024-03-15 15:00:47.000000 iLCDirac-35.0.2/src/ILCDIRAC/Interfaces/API/Examples/SIDChain/slicMacros/mu-_10gev_theta90.mac
--rw-rw-rw-   0 root         (0) root         (0)      325 2024-03-15 15:00:47.000000 iLCDirac-35.0.2/src/ILCDIRAC/Interfaces/API/Examples/SIDChain/slicMacros/mu-_200gev_theta10.mac
--rw-rw-rw-   0 root         (0) root         (0)      325 2024-03-15 15:00:47.000000 iLCDirac-35.0.2/src/ILCDIRAC/Interfaces/API/Examples/SIDChain/slicMacros/mu-_200gev_theta20.mac
--rw-rw-rw-   0 root         (0) root         (0)      325 2024-03-15 15:00:47.000000 iLCDirac-35.0.2/src/ILCDIRAC/Interfaces/API/Examples/SIDChain/slicMacros/mu-_200gev_theta30.mac
--rw-rw-rw-   0 root         (0) root         (0)      325 2024-03-15 15:00:47.000000 iLCDirac-35.0.2/src/ILCDIRAC/Interfaces/API/Examples/SIDChain/slicMacros/mu-_200gev_theta40.mac
--rw-rw-rw-   0 root         (0) root         (0)      325 2024-03-15 15:00:47.000000 iLCDirac-35.0.2/src/ILCDIRAC/Interfaces/API/Examples/SIDChain/slicMacros/mu-_200gev_theta50.mac
--rw-rw-rw-   0 root         (0) root         (0)      325 2024-03-15 15:00:47.000000 iLCDirac-35.0.2/src/ILCDIRAC/Interfaces/API/Examples/SIDChain/slicMacros/mu-_200gev_theta60.mac
--rw-rw-rw-   0 root         (0) root         (0)      325 2024-03-15 15:00:47.000000 iLCDirac-35.0.2/src/ILCDIRAC/Interfaces/API/Examples/SIDChain/slicMacros/mu-_200gev_theta70.mac
--rw-rw-rw-   0 root         (0) root         (0)      325 2024-03-15 15:00:47.000000 iLCDirac-35.0.2/src/ILCDIRAC/Interfaces/API/Examples/SIDChain/slicMacros/mu-_200gev_theta80.mac
--rw-rw-rw-   0 root         (0) root         (0)      325 2024-03-15 15:00:47.000000 iLCDirac-35.0.2/src/ILCDIRAC/Interfaces/API/Examples/SIDChain/slicMacros/mu-_200gev_theta90.mac
--rw-rw-rw-   0 root         (0) root         (0)      324 2024-03-15 15:00:47.000000 iLCDirac-35.0.2/src/ILCDIRAC/Interfaces/API/Examples/SIDChain/slicMacros/mu-_50gev_theta10.mac
--rw-rw-rw-   0 root         (0) root         (0)      324 2024-03-15 15:00:47.000000 iLCDirac-35.0.2/src/ILCDIRAC/Interfaces/API/Examples/SIDChain/slicMacros/mu-_50gev_theta20.mac
--rw-rw-rw-   0 root         (0) root         (0)      324 2024-03-15 15:00:47.000000 iLCDirac-35.0.2/src/ILCDIRAC/Interfaces/API/Examples/SIDChain/slicMacros/mu-_50gev_theta30.mac
--rw-rw-rw-   0 root         (0) root         (0)      324 2024-03-15 15:00:47.000000 iLCDirac-35.0.2/src/ILCDIRAC/Interfaces/API/Examples/SIDChain/slicMacros/mu-_50gev_theta40.mac
--rw-rw-rw-   0 root         (0) root         (0)      324 2024-03-15 15:00:47.000000 iLCDirac-35.0.2/src/ILCDIRAC/Interfaces/API/Examples/SIDChain/slicMacros/mu-_50gev_theta50.mac
--rw-rw-rw-   0 root         (0) root         (0)      324 2024-03-15 15:00:47.000000 iLCDirac-35.0.2/src/ILCDIRAC/Interfaces/API/Examples/SIDChain/slicMacros/mu-_50gev_theta60.mac
--rw-rw-rw-   0 root         (0) root         (0)      324 2024-03-15 15:00:47.000000 iLCDirac-35.0.2/src/ILCDIRAC/Interfaces/API/Examples/SIDChain/slicMacros/mu-_50gev_theta70.mac
--rw-rw-rw-   0 root         (0) root         (0)      324 2024-03-15 15:00:47.000000 iLCDirac-35.0.2/src/ILCDIRAC/Interfaces/API/Examples/SIDChain/slicMacros/mu-_50gev_theta80.mac
--rw-rw-rw-   0 root         (0) root         (0)      324 2024-03-15 15:00:47.000000 iLCDirac-35.0.2/src/ILCDIRAC/Interfaces/API/Examples/SIDChain/slicMacros/mu-_50gev_theta90.mac
--rw-rw-rw-   0 root         (0) root         (0)      325 2024-03-15 15:00:47.000000 iLCDirac-35.0.2/src/ILCDIRAC/Interfaces/API/Examples/SIDChain/slicMacros/pi-_100gev_theta5-175.mac
--rw-rw-rw-   0 root         (0) root         (0)      324 2024-03-15 15:00:47.000000 iLCDirac-35.0.2/src/ILCDIRAC/Interfaces/API/Examples/SIDChain/slicMacros/pi-_10gev_theta5-175.mac
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-15 15:01:06.507158 iLCDirac-35.0.2/src/ILCDIRAC/Interfaces/API/Examples/SiDProduction/
--rw-rw-rw-   0 root         (0) root         (0)     8766 2024-03-15 15:00:47.000000 iLCDirac-35.0.2/src/ILCDIRAC/Interfaces/API/Examples/SiDProduction/sid_dbd_sim_production_default.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-15 15:01:06.510158 iLCDirac-35.0.2/src/ILCDIRAC/Interfaces/API/NewInterface/
--rw-rw-rw-   0 root         (0) root         (0)    27099 2024-03-15 15:00:47.000000 iLCDirac-35.0.2/src/ILCDIRAC/Interfaces/API/NewInterface/Application.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-15 15:01:06.519158 iLCDirac-35.0.2/src/ILCDIRAC/Interfaces/API/NewInterface/Applications/
--rw-rw-rw-   0 root         (0) root         (0)     6108 2024-03-15 15:00:47.000000 iLCDirac-35.0.2/src/ILCDIRAC/Interfaces/API/NewInterface/Applications/Babayaga.py
--rw-rw-rw-   0 root         (0) root         (0)     6024 2024-03-15 15:00:47.000000 iLCDirac-35.0.2/src/ILCDIRAC/Interfaces/API/NewInterface/Applications/Bhlumi.py
--rw-rw-rw-   0 root         (0) root         (0)     3135 2024-03-15 15:00:47.000000 iLCDirac-35.0.2/src/ILCDIRAC/Interfaces/API/NewInterface/Applications/Calibration.py
--rw-rw-rw-   0 root         (0) root         (0)     3757 2024-03-15 15:00:47.000000 iLCDirac-35.0.2/src/ILCDIRAC/Interfaces/API/NewInterface/Applications/CheckCollections.py
--rw-rw-rw-   0 root         (0) root         (0)     2335 2024-03-15 15:00:47.000000 iLCDirac-35.0.2/src/ILCDIRAC/Interfaces/API/NewInterface/Applications/CheckWNs.py
--rw-rw-rw-   0 root         (0) root         (0)    10462 2024-03-15 15:00:47.000000 iLCDirac-35.0.2/src/ILCDIRAC/Interfaces/API/NewInterface/Applications/DDSim.py
--rw-rw-rw-   0 root         (0) root         (0)    14016 2024-03-15 15:00:47.000000 iLCDirac-35.0.2/src/ILCDIRAC/Interfaces/API/NewInterface/Applications/DelphesApp.py
--rw-rw-rw-   0 root         (0) root         (0)    35946 2024-03-15 15:00:47.000000 iLCDirac-35.0.2/src/ILCDIRAC/Interfaces/API/NewInterface/Applications/Fcc.py
--rw-rw-rw-   0 root         (0) root         (0)    13940 2024-03-15 15:00:47.000000 iLCDirac-35.0.2/src/ILCDIRAC/Interfaces/API/NewInterface/Applications/GaudiApp.py
--rw-rw-rw-   0 root         (0) root         (0)     6521 2024-03-15 15:00:47.000000 iLCDirac-35.0.2/src/ILCDIRAC/Interfaces/API/NewInterface/Applications/GenericApplication.py
--rw-rw-rw-   0 root         (0) root         (0)     3885 2024-03-15 15:00:47.000000 iLCDirac-35.0.2/src/ILCDIRAC/Interfaces/API/NewInterface/Applications/GetSRMFile.py
--rw-rw-rw-   0 root         (0) root         (0)     6008 2024-03-15 15:00:47.000000 iLCDirac-35.0.2/src/ILCDIRAC/Interfaces/API/NewInterface/Applications/KKMC.py
--rw-rw-rw-   0 root         (0) root         (0)     9573 2024-03-15 15:00:47.000000 iLCDirac-35.0.2/src/ILCDIRAC/Interfaces/API/NewInterface/Applications/LCSIM.py
--rw-rw-rw-   0 root         (0) root         (0)    10161 2024-03-15 15:00:47.000000 iLCDirac-35.0.2/src/ILCDIRAC/Interfaces/API/NewInterface/Applications/Marlin.py
--rw-rw-rw-   0 root         (0) root         (0)     8281 2024-03-15 15:00:47.000000 iLCDirac-35.0.2/src/ILCDIRAC/Interfaces/API/NewInterface/Applications/Mokka.py
--rw-rw-rw-   0 root         (0) root         (0)    16303 2024-03-15 15:00:47.000000 iLCDirac-35.0.2/src/ILCDIRAC/Interfaces/API/NewInterface/Applications/OverlayInput.py
--rw-rw-rw-   0 root         (0) root         (0)     3918 2024-03-15 15:00:47.000000 iLCDirac-35.0.2/src/ILCDIRAC/Interfaces/API/NewInterface/Applications/PostGenSelection.py
--rw-rw-rw-   0 root         (0) root         (0)     3312 2024-03-15 15:00:47.000000 iLCDirac-35.0.2/src/ILCDIRAC/Interfaces/API/NewInterface/Applications/Pythia.py
--rw-rw-rw-   0 root         (0) root         (0)     2090 2024-03-15 15:00:47.000000 iLCDirac-35.0.2/src/ILCDIRAC/Interfaces/API/NewInterface/Applications/RootMacro.py
--rw-rw-rw-   0 root         (0) root         (0)     2461 2024-03-15 15:00:47.000000 iLCDirac-35.0.2/src/ILCDIRAC/Interfaces/API/NewInterface/Applications/RootScript.py
--rw-rw-rw-   0 root         (0) root         (0)     3752 2024-03-15 15:00:47.000000 iLCDirac-35.0.2/src/ILCDIRAC/Interfaces/API/NewInterface/Applications/SLCIOConcatenate.py
--rw-rw-rw-   0 root         (0) root         (0)     4434 2024-03-15 15:00:47.000000 iLCDirac-35.0.2/src/ILCDIRAC/Interfaces/API/NewInterface/Applications/SLCIOSplit.py
--rw-rw-rw-   0 root         (0) root         (0)     6174 2024-03-15 15:00:47.000000 iLCDirac-35.0.2/src/ILCDIRAC/Interfaces/API/NewInterface/Applications/SLIC.py
--rw-rw-rw-   0 root         (0) root         (0)     6089 2024-03-15 15:00:47.000000 iLCDirac-35.0.2/src/ILCDIRAC/Interfaces/API/NewInterface/Applications/SLICPandora.py
--rw-rw-rw-   0 root         (0) root         (0)     5479 2024-03-15 15:00:47.000000 iLCDirac-35.0.2/src/ILCDIRAC/Interfaces/API/NewInterface/Applications/StdHepSplit.py
--rw-rw-rw-   0 root         (0) root         (0)     6957 2024-03-15 15:00:47.000000 iLCDirac-35.0.2/src/ILCDIRAC/Interfaces/API/NewInterface/Applications/StdhepCut.py
--rw-rw-rw-   0 root         (0) root         (0)     1782 2024-03-15 15:00:47.000000 iLCDirac-35.0.2/src/ILCDIRAC/Interfaces/API/NewInterface/Applications/StdhepCutJava.py
--rw-rw-rw-   0 root         (0) root         (0)     3921 2024-03-15 15:00:47.000000 iLCDirac-35.0.2/src/ILCDIRAC/Interfaces/API/NewInterface/Applications/Tomato.py
--rw-rw-rw-   0 root         (0) root         (0)    17277 2024-03-15 15:00:47.000000 iLCDirac-35.0.2/src/ILCDIRAC/Interfaces/API/NewInterface/Applications/Whizard.py
--rw-rw-rw-   0 root         (0) root         (0)    12788 2024-03-15 15:00:47.000000 iLCDirac-35.0.2/src/ILCDIRAC/Interfaces/API/NewInterface/Applications/Whizard2.py
--rw-rw-rw-   0 root         (0) root         (0)     4441 2024-03-15 15:00:47.000000 iLCDirac-35.0.2/src/ILCDIRAC/Interfaces/API/NewInterface/Applications/_Root.py
--rw-rw-rw-   0 root         (0) root         (0)     5185 2024-03-15 15:00:47.000000 iLCDirac-35.0.2/src/ILCDIRAC/Interfaces/API/NewInterface/Applications/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-15 15:01:06.521158 iLCDirac-35.0.2/src/ILCDIRAC/Interfaces/API/NewInterface/Examples/
--rw-rw-rw-   0 root         (0) root         (0)     2838 2024-03-15 15:00:47.000000 iLCDirac-35.0.2/src/ILCDIRAC/Interfaces/API/NewInterface/Examples/ConditionalOverlay.py
--rw-rw-rw-   0 root         (0) root         (0)     2672 2024-03-15 15:00:47.000000 iLCDirac-35.0.2/src/ILCDIRAC/Interfaces/API/NewInterface/Examples/FullILDChain.py
--rw-rw-rw-   0 root         (0) root         (0)    19620 2024-03-15 15:00:47.000000 iLCDirac-35.0.2/src/ILCDIRAC/Interfaces/API/NewInterface/Examples/ILDProductionChainDBD.py
--rw-rw-rw-   0 root         (0) root         (0)    22235 2024-03-15 15:00:47.000000 iLCDirac-35.0.2/src/ILCDIRAC/Interfaces/API/NewInterface/Examples/ILDProductionChainOpt2017.py
--rw-rw-rw-   0 root         (0) root         (0)     2078 2024-03-15 15:00:47.000000 iLCDirac-35.0.2/src/ILCDIRAC/Interfaces/API/NewInterface/Examples/MarlinExample.py
--rw-rw-rw-   0 root         (0) root         (0)     2841 2024-03-15 15:00:47.000000 iLCDirac-35.0.2/src/ILCDIRAC/Interfaces/API/NewInterface/Examples/MokkaMarlinOverlayMarlin.py
--rw-rw-rw-   0 root         (0) root         (0)     2993 2024-03-15 15:00:47.000000 iLCDirac-35.0.2/src/ILCDIRAC/Interfaces/API/NewInterface/Examples/ParametricJobExample.py
--rw-rw-rw-   0 root         (0) root         (0)     4254 2024-03-15 15:00:47.000000 iLCDirac-35.0.2/src/ILCDIRAC/Interfaces/API/NewInterface/Examples/ReplicationAkiya.py
--rw-rw-rw-   0 root         (0) root         (0)     9864 2024-03-15 15:00:47.000000 iLCDirac-35.0.2/src/ILCDIRAC/Interfaces/API/NewInterface/Examples/SIDProductionChain.py
--rw-rw-rw-   0 root         (0) root         (0)    24484 2024-03-15 15:00:47.000000 iLCDirac-35.0.2/src/ILCDIRAC/Interfaces/API/NewInterface/ILDProductionJobDBD.py
--rw-rw-rw-   0 root         (0) root         (0)    26292 2024-03-15 15:00:47.000000 iLCDirac-35.0.2/src/ILCDIRAC/Interfaces/API/NewInterface/ILDProductionJobOpt2017.py
--rw-rw-rw-   0 root         (0) root         (0)    15111 2024-03-15 15:00:47.000000 iLCDirac-35.0.2/src/ILCDIRAC/Interfaces/API/NewInterface/Job.py
--rw-rw-rw-   0 root         (0) root         (0)     3097 2024-03-15 15:00:47.000000 iLCDirac-35.0.2/src/ILCDIRAC/Interfaces/API/NewInterface/LCApplication.py
--rw-rw-rw-   0 root         (0) root         (0)     2402 2024-03-15 15:00:47.000000 iLCDirac-35.0.2/src/ILCDIRAC/Interfaces/API/NewInterface/LCUtilityApplication.py
--rw-rw-rw-   0 root         (0) root         (0)    42099 2024-03-15 15:00:47.000000 iLCDirac-35.0.2/src/ILCDIRAC/Interfaces/API/NewInterface/ProductionJob.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-15 15:01:06.523158 iLCDirac-35.0.2/src/ILCDIRAC/Interfaces/API/NewInterface/Productions/
--rw-rw-rw-   0 root         (0) root         (0)    28003 2024-03-15 15:00:47.000000 iLCDirac-35.0.2/src/ILCDIRAC/Interfaces/API/NewInterface/Productions/CLICProductionChain.py
--rw-rw-rw-   0 root         (0) root         (0)    29734 2024-03-15 15:00:47.000000 iLCDirac-35.0.2/src/ILCDIRAC/Interfaces/API/NewInterface/Productions/CLICProductionChain_hzqq_420.py
--rwxrwxrwx   0 root         (0) root         (0)    35686 2024-03-15 15:00:47.000000 iLCDirac-35.0.2/src/ILCDIRAC/Interfaces/API/NewInterface/Productions/ProductionChainTest.py
--rw-rw-rw-   0 root         (0) root         (0)    13131 2024-03-15 15:00:47.000000 iLCDirac-35.0.2/src/ILCDIRAC/Interfaces/API/NewInterface/Productions/SIDProductionChain.py
--rw-rw-rw-   0 root         (0) root         (0)    12330 2024-03-15 15:00:47.000000 iLCDirac-35.0.2/src/ILCDIRAC/Interfaces/API/NewInterface/SIDProductionJob.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-15 15:01:06.531158 iLCDirac-35.0.2/src/ILCDIRAC/Interfaces/API/NewInterface/Tests/
--rw-rw-rw-   0 root         (0) root         (0)     7876 2024-03-15 15:00:47.000000 iLCDirac-35.0.2/src/ILCDIRAC/Interfaces/API/NewInterface/Tests/Test_Application.py
--rw-rw-rw-   0 root         (0) root         (0)     9657 2024-03-15 15:00:47.000000 iLCDirac-35.0.2/src/ILCDIRAC/Interfaces/API/NewInterface/Tests/Test_Babayaga.py
--rw-rw-rw-   0 root         (0) root         (0)     9427 2024-03-15 15:00:47.000000 iLCDirac-35.0.2/src/ILCDIRAC/Interfaces/API/NewInterface/Tests/Test_Bhlumi.py
--rw-rw-rw-   0 root         (0) root         (0)     2416 2024-03-15 15:00:47.000000 iLCDirac-35.0.2/src/ILCDIRAC/Interfaces/API/NewInterface/Tests/Test_Calibration.py
--rw-rw-rw-   0 root         (0) root         (0)     4672 2024-03-15 15:00:47.000000 iLCDirac-35.0.2/src/ILCDIRAC/Interfaces/API/NewInterface/Tests/Test_CheckCollections.py
--rw-rw-rw-   0 root         (0) root         (0)     2878 2024-03-15 15:00:47.000000 iLCDirac-35.0.2/src/ILCDIRAC/Interfaces/API/NewInterface/Tests/Test_CheckWNs.py
--rw-rw-rw-   0 root         (0) root         (0)    18299 2024-03-15 15:00:47.000000 iLCDirac-35.0.2/src/ILCDIRAC/Interfaces/API/NewInterface/Tests/Test_DDSim.py
--rw-rw-rw-   0 root         (0) root         (0)    20338 2024-03-15 15:00:47.000000 iLCDirac-35.0.2/src/ILCDIRAC/Interfaces/API/NewInterface/Tests/Test_DelphesApp.py
--rw-rw-rw-   0 root         (0) root         (0)    41414 2024-03-15 15:00:47.000000 iLCDirac-35.0.2/src/ILCDIRAC/Interfaces/API/NewInterface/Tests/Test_Fcc.py
--rw-rw-rw-   0 root         (0) root         (0)    16986 2024-03-15 15:00:47.000000 iLCDirac-35.0.2/src/ILCDIRAC/Interfaces/API/NewInterface/Tests/Test_GaudiApp.py
--rw-rw-rw-   0 root         (0) root         (0)     5930 2024-03-15 15:00:47.000000 iLCDirac-35.0.2/src/ILCDIRAC/Interfaces/API/NewInterface/Tests/Test_GenericApplication.py
--rw-rw-rw-   0 root         (0) root         (0)     4218 2024-03-15 15:00:47.000000 iLCDirac-35.0.2/src/ILCDIRAC/Interfaces/API/NewInterface/Tests/Test_GetSRMFile.py
--rw-rw-rw-   0 root         (0) root         (0)    13745 2024-03-15 15:00:47.000000 iLCDirac-35.0.2/src/ILCDIRAC/Interfaces/API/NewInterface/Tests/Test_Job.py
--rw-rw-rw-   0 root         (0) root         (0)     8888 2024-03-15 15:00:47.000000 iLCDirac-35.0.2/src/ILCDIRAC/Interfaces/API/NewInterface/Tests/Test_KKMC.py
--rw-rw-rw-   0 root         (0) root         (0)    12305 2024-03-15 15:00:47.000000 iLCDirac-35.0.2/src/ILCDIRAC/Interfaces/API/NewInterface/Tests/Test_LCSIM.py
--rw-rw-rw-   0 root         (0) root         (0)     8309 2024-03-15 15:00:47.000000 iLCDirac-35.0.2/src/ILCDIRAC/Interfaces/API/NewInterface/Tests/Test_Marlin.py
--rw-rw-rw-   0 root         (0) root         (0)     6492 2024-03-15 15:00:47.000000 iLCDirac-35.0.2/src/ILCDIRAC/Interfaces/API/NewInterface/Tests/Test_Mokka.py
--rw-rw-rw-   0 root         (0) root         (0)    14537 2024-03-15 15:00:47.000000 iLCDirac-35.0.2/src/ILCDIRAC/Interfaces/API/NewInterface/Tests/Test_OverlayInput.py
--rw-rw-rw-   0 root         (0) root         (0)     4767 2024-03-15 15:00:47.000000 iLCDirac-35.0.2/src/ILCDIRAC/Interfaces/API/NewInterface/Tests/Test_PostGenSelection.py
--rw-rw-rw-   0 root         (0) root         (0)    75909 2024-03-15 15:00:47.000000 iLCDirac-35.0.2/src/ILCDIRAC/Interfaces/API/NewInterface/Tests/Test_ProductionJob.py
--rw-rw-rw-   0 root         (0) root         (0)     4830 2024-03-15 15:00:47.000000 iLCDirac-35.0.2/src/ILCDIRAC/Interfaces/API/NewInterface/Tests/Test_Pythia.py
--rw-rw-rw-   0 root         (0) root         (0)     4533 2024-03-15 15:00:47.000000 iLCDirac-35.0.2/src/ILCDIRAC/Interfaces/API/NewInterface/Tests/Test_SLCIOConcatenate.py
--rw-rw-rw-   0 root         (0) root         (0)     4798 2024-03-15 15:00:47.000000 iLCDirac-35.0.2/src/ILCDIRAC/Interfaces/API/NewInterface/Tests/Test_SLCIOSplit.py
--rw-rw-rw-   0 root         (0) root         (0)     6232 2024-03-15 15:00:47.000000 iLCDirac-35.0.2/src/ILCDIRAC/Interfaces/API/NewInterface/Tests/Test_SLIC.py
--rw-rw-rw-   0 root         (0) root         (0)     7551 2024-03-15 15:00:47.000000 iLCDirac-35.0.2/src/ILCDIRAC/Interfaces/API/NewInterface/Tests/Test_SLICPandora.py
--rw-rw-rw-   0 root         (0) root         (0)     5077 2024-03-15 15:00:47.000000 iLCDirac-35.0.2/src/ILCDIRAC/Interfaces/API/NewInterface/Tests/Test_StdHepSplit.py
--rw-rw-rw-   0 root         (0) root         (0)     6829 2024-03-15 15:00:47.000000 iLCDirac-35.0.2/src/ILCDIRAC/Interfaces/API/NewInterface/Tests/Test_StdhepCut.py
--rw-rw-rw-   0 root         (0) root         (0)     4763 2024-03-15 15:00:47.000000 iLCDirac-35.0.2/src/ILCDIRAC/Interfaces/API/NewInterface/Tests/Test_Tomato.py
--rw-rw-rw-   0 root         (0) root         (0)    22726 2024-03-15 15:00:47.000000 iLCDirac-35.0.2/src/ILCDIRAC/Interfaces/API/NewInterface/Tests/Test_UserJob.py
--rw-rw-rw-   0 root         (0) root         (0)    20865 2024-03-15 15:00:47.000000 iLCDirac-35.0.2/src/ILCDIRAC/Interfaces/API/NewInterface/Tests/Test_Whizard.py
--rw-rw-rw-   0 root         (0) root         (0)    13044 2024-03-15 15:00:47.000000 iLCDirac-35.0.2/src/ILCDIRAC/Interfaces/API/NewInterface/Tests/Test_Whizard2.py
--rw-rw-rw-   0 root         (0) root         (0)     4169 2024-03-15 15:00:47.000000 iLCDirac-35.0.2/src/ILCDIRAC/Interfaces/API/NewInterface/Tests/Test__Root.py
--rw-rw-rw-   0 root         (0) root         (0)     1128 2024-03-15 15:00:47.000000 iLCDirac-35.0.2/src/ILCDIRAC/Interfaces/API/NewInterface/Tests/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     9860 2024-03-15 15:00:47.000000 iLCDirac-35.0.2/src/ILCDIRAC/Interfaces/API/NewInterface/UserJob.py
--rw-rw-rw-   0 root         (0) root         (0)     1129 2024-03-15 15:00:47.000000 iLCDirac-35.0.2/src/ILCDIRAC/Interfaces/API/NewInterface/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-15 15:01:06.532158 iLCDirac-35.0.2/src/ILCDIRAC/Interfaces/API/Test/
--rw-rw-rw-   0 root         (0) root         (0)    20995 2024-03-15 15:00:47.000000 iLCDirac-35.0.2/src/ILCDIRAC/Interfaces/API/Test/Test_DiracILC.py
--rw-rw-rw-   0 root         (0) root         (0)     1132 2024-03-15 15:00:47.000000 iLCDirac-35.0.2/src/ILCDIRAC/Interfaces/API/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-15 15:01:06.532158 iLCDirac-35.0.2/src/ILCDIRAC/Interfaces/Tests/
--rw-rw-rw-   0 root         (0) root         (0)     2622 2024-03-15 15:00:47.000000 iLCDirac-35.0.2/src/ILCDIRAC/Interfaces/Tests/Test_JobHelpers.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-15 15:01:06.533158 iLCDirac-35.0.2/src/ILCDIRAC/Interfaces/Utilities/
--rw-rw-rw-   0 root         (0) root         (0)     4727 2024-03-15 15:00:47.000000 iLCDirac-35.0.2/src/ILCDIRAC/Interfaces/Utilities/DDInterfaceMixin.py
--rw-rw-rw-   0 root         (0) root         (0)     1680 2024-03-15 15:00:47.000000 iLCDirac-35.0.2/src/ILCDIRAC/Interfaces/Utilities/JobHelpers.py
--rw-rw-rw-   0 root         (0) root         (0)    15312 2024-03-15 15:00:47.000000 iLCDirac-35.0.2/src/ILCDIRAC/Interfaces/Utilities/SplitMixin.py
--rw-rw-rw-   0 root         (0) root         (0)     1013 2024-03-15 15:00:47.000000 iLCDirac-35.0.2/src/ILCDIRAC/Interfaces/Utilities/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1116 2024-03-15 15:00:47.000000 iLCDirac-35.0.2/src/ILCDIRAC/Interfaces/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-15 15:01:06.535158 iLCDirac-35.0.2/src/ILCDIRAC/Interfaces/scripts/
--rwxrwxrwx   0 root         (0) root         (0)     2975 2024-03-15 15:00:47.000000 iLCDirac-35.0.2/src/ILCDIRAC/Interfaces/scripts/TestAndProbeSites.py
--rw-rw-rw-   0 root         (0) root         (0)     1073 2024-03-15 15:00:47.000000 iLCDirac-35.0.2/src/ILCDIRAC/Interfaces/scripts/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     7669 2024-03-15 15:00:47.000000 iLCDirac-35.0.2/src/ILCDIRAC/Interfaces/scripts/dirac_ilc_find_in_FC.py
--rw-rw-rw-   0 root         (0) root         (0)     3483 2024-03-15 15:00:47.000000 iLCDirac-35.0.2/src/ILCDIRAC/Interfaces/scripts/dirac_ilc_show_software.py
--rw-rw-rw-   0 root         (0) root         (0)     2581 2024-03-15 15:00:47.000000 iLCDirac-35.0.2/src/ILCDIRAC/Interfaces/scripts/dirac_repo_create_lfn_list.py
--rw-rw-rw-   0 root         (0) root         (0)     3033 2024-03-15 15:00:47.000000 iLCDirac-35.0.2/src/ILCDIRAC/Interfaces/scripts/dirac_repo_retrieve_jobs_output.py
--rw-rw-rw-   0 root         (0) root         (0)     2341 2024-03-15 15:00:47.000000 iLCDirac-35.0.2/src/ILCDIRAC/Interfaces/scripts/dirac_repo_retrieve_jobs_output_data.py
--rwxrwxrwx   0 root         (0) root         (0)     3634 2024-03-15 15:00:47.000000 iLCDirac-35.0.2/src/ILCDIRAC/Interfaces/scripts/ilcdirac_version.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-15 15:01:06.536158 iLCDirac-35.0.2/src/ILCDIRAC/OverlaySystem/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-15 15:01:06.536158 iLCDirac-35.0.2/src/ILCDIRAC/OverlaySystem/Agent/
--rw-rw-rw-   0 root         (0) root         (0)     2638 2024-03-15 15:00:47.000000 iLCDirac-35.0.2/src/ILCDIRAC/OverlaySystem/Agent/ResetCounters.py
--rw-rw-rw-   0 root         (0) root         (0)     1088 2024-03-15 15:00:47.000000 iLCDirac-35.0.2/src/ILCDIRAC/OverlaySystem/Agent/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-15 15:01:06.537158 iLCDirac-35.0.2/src/ILCDIRAC/OverlaySystem/Client/
--rw-rw-rw-   0 root         (0) root         (0)     1399 2024-03-15 15:00:47.000000 iLCDirac-35.0.2/src/ILCDIRAC/OverlaySystem/Client/OverlaySystemClient.py
--rw-rw-rw-   0 root         (0) root         (0)     1088 2024-03-15 15:00:47.000000 iLCDirac-35.0.2/src/ILCDIRAC/OverlaySystem/Client/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      221 2024-03-15 15:00:47.000000 iLCDirac-35.0.2/src/ILCDIRAC/OverlaySystem/ConfigTemplate.cfg
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-15 15:01:06.537158 iLCDirac-35.0.2/src/ILCDIRAC/OverlaySystem/DB/
--rw-rw-rw-   0 root         (0) root         (0)     6953 2024-03-15 15:00:47.000000 iLCDirac-35.0.2/src/ILCDIRAC/OverlaySystem/DB/OverlayDB.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-15 15:01:06.537158 iLCDirac-35.0.2/src/ILCDIRAC/OverlaySystem/DB/Test/
--rw-rw-rw-   0 root         (0) root         (0)     9389 2024-03-15 15:00:47.000000 iLCDirac-35.0.2/src/ILCDIRAC/OverlaySystem/DB/Test/Test_OverlayDB.py
--rw-rw-rw-   0 root         (0) root         (0)     1062 2024-03-15 15:00:47.000000 iLCDirac-35.0.2/src/ILCDIRAC/OverlaySystem/DB/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-15 15:01:06.538158 iLCDirac-35.0.2/src/ILCDIRAC/OverlaySystem/Service/
--rw-rw-rw-   0 root         (0) root         (0)     2462 2024-03-15 15:00:47.000000 iLCDirac-35.0.2/src/ILCDIRAC/OverlaySystem/Service/OverlayHandler.py
--rw-rw-rw-   0 root         (0) root         (0)     1072 2024-03-15 15:00:47.000000 iLCDirac-35.0.2/src/ILCDIRAC/OverlaySystem/Service/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1118 2024-03-15 15:00:47.000000 iLCDirac-35.0.2/src/ILCDIRAC/OverlaySystem/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-15 15:01:06.538158 iLCDirac-35.0.2/src/ILCDIRAC/Workflow/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-15 15:01:06.550158 iLCDirac-35.0.2/src/ILCDIRAC/Workflow/Modules/
--rw-rw-rw-   0 root         (0) root         (0)     4515 2024-03-15 15:00:47.000000 iLCDirac-35.0.2/src/ILCDIRAC/Workflow/Modules/AnalyseWN.py
--rw-rw-rw-   0 root         (0) root         (0)     5524 2024-03-15 15:00:47.000000 iLCDirac-35.0.2/src/ILCDIRAC/Workflow/Modules/ApplicationScript.py
--rw-rw-rw-   0 root         (0) root         (0)     7489 2024-03-15 15:00:47.000000 iLCDirac-35.0.2/src/ILCDIRAC/Workflow/Modules/BabayagaAnalysis.py
--rw-rw-rw-   0 root         (0) root         (0)     8870 2024-03-15 15:00:47.000000 iLCDirac-35.0.2/src/ILCDIRAC/Workflow/Modules/BhlumiAnalysis.py
--rw-rw-rw-   0 root         (0) root         (0)    23026 2024-03-15 15:00:47.000000 iLCDirac-35.0.2/src/ILCDIRAC/Workflow/Modules/Calibration.py
--rw-rw-rw-   0 root         (0) root         (0)     5789 2024-03-15 15:00:47.000000 iLCDirac-35.0.2/src/ILCDIRAC/Workflow/Modules/CheckCollections.py
--rw-rw-rw-   0 root         (0) root         (0)     2452 2024-03-15 15:00:47.000000 iLCDirac-35.0.2/src/ILCDIRAC/Workflow/Modules/ComputeOutputDataList.py
--rw-rw-rw-   0 root         (0) root         (0)     3146 2024-03-15 15:00:47.000000 iLCDirac-35.0.2/src/ILCDIRAC/Workflow/Modules/DBDGenRegisterOutputData.py
--rw-rw-rw-   0 root         (0) root         (0)    16673 2024-03-15 15:00:47.000000 iLCDirac-35.0.2/src/ILCDIRAC/Workflow/Modules/DDSimAnalysis.py
--rw-rw-rw-   0 root         (0) root         (0)     9184 2024-03-15 15:00:47.000000 iLCDirac-35.0.2/src/ILCDIRAC/Workflow/Modules/DelphesAppModule.py
--rw-rw-rw-   0 root         (0) root         (0)     1894 2024-03-15 15:00:47.000000 iLCDirac-35.0.2/src/ILCDIRAC/Workflow/Modules/DummyModule.py
--rw-rw-rw-   0 root         (0) root         (0)     6809 2024-03-15 15:00:47.000000 iLCDirac-35.0.2/src/ILCDIRAC/Workflow/Modules/FailoverRequest.py
--rw-rw-rw-   0 root         (0) root         (0)    19926 2024-03-15 15:00:47.000000 iLCDirac-35.0.2/src/ILCDIRAC/Workflow/Modules/FccAnalysis.py
--rw-rw-rw-   0 root         (0) root         (0)     8792 2024-03-15 15:00:47.000000 iLCDirac-35.0.2/src/ILCDIRAC/Workflow/Modules/GaudiAppModule.py
--rw-rw-rw-   0 root         (0) root         (0)     4454 2024-03-15 15:00:47.000000 iLCDirac-35.0.2/src/ILCDIRAC/Workflow/Modules/GetSRMFile.py
--rw-rw-rw-   0 root         (0) root         (0)     6156 2024-03-15 15:00:47.000000 iLCDirac-35.0.2/src/ILCDIRAC/Workflow/Modules/ILDRegisterOutputData.py
--rw-rw-rw-   0 root         (0) root         (0)     7234 2024-03-15 15:00:47.000000 iLCDirac-35.0.2/src/ILCDIRAC/Workflow/Modules/KKMCAnalysis.py
--rw-rw-rw-   0 root         (0) root         (0)     5057 2024-03-15 15:00:47.000000 iLCDirac-35.0.2/src/ILCDIRAC/Workflow/Modules/LCIOConcatenate.py
--rw-rw-rw-   0 root         (0) root         (0)     8078 2024-03-15 15:00:47.000000 iLCDirac-35.0.2/src/ILCDIRAC/Workflow/Modules/LCIOSplit.py
--rw-rw-rw-   0 root         (0) root         (0)    13096 2024-03-15 15:00:47.000000 iLCDirac-35.0.2/src/ILCDIRAC/Workflow/Modules/LCSIMAnalysis.py
--rw-rw-rw-   0 root         (0) root         (0)    18950 2024-03-15 15:00:47.000000 iLCDirac-35.0.2/src/ILCDIRAC/Workflow/Modules/MarlinAnalysis.py
--rw-rw-rw-   0 root         (0) root         (0)    31351 2024-03-15 15:00:47.000000 iLCDirac-35.0.2/src/ILCDIRAC/Workflow/Modules/ModuleBase.py
--rw-rw-rw-   0 root         (0) root         (0)    26082 2024-03-15 15:00:47.000000 iLCDirac-35.0.2/src/ILCDIRAC/Workflow/Modules/MokkaAnalysis.py
--rw-rw-rw-   0 root         (0) root         (0)     5266 2024-03-15 15:00:47.000000 iLCDirac-35.0.2/src/ILCDIRAC/Workflow/Modules/MoveInFC.py
--rw-rw-rw-   0 root         (0) root         (0)    33871 2024-03-15 15:00:47.000000 iLCDirac-35.0.2/src/ILCDIRAC/Workflow/Modules/OverlayInput.py
--rw-rw-rw-   0 root         (0) root         (0)     7960 2024-03-15 15:00:47.000000 iLCDirac-35.0.2/src/ILCDIRAC/Workflow/Modules/PostGenSelection.py
--rw-rw-rw-   0 root         (0) root         (0)     8182 2024-03-15 15:00:47.000000 iLCDirac-35.0.2/src/ILCDIRAC/Workflow/Modules/PythiaAnalysis.py
--rw-rw-rw-   0 root         (0) root         (0)     5743 2024-03-15 15:00:47.000000 iLCDirac-35.0.2/src/ILCDIRAC/Workflow/Modules/RegisterOutputData.py
--rw-rw-rw-   0 root         (0) root         (0)     3640 2024-03-15 15:00:47.000000 iLCDirac-35.0.2/src/ILCDIRAC/Workflow/Modules/RemoveInputData.py
--rw-rw-rw-   0 root         (0) root         (0)     2095 2024-03-15 15:00:47.000000 iLCDirac-35.0.2/src/ILCDIRAC/Workflow/Modules/ReportErrors.py
--rw-rw-rw-   0 root         (0) root         (0)     5915 2024-03-15 15:00:47.000000 iLCDirac-35.0.2/src/ILCDIRAC/Workflow/Modules/RootExecutableAnalysis.py
--rw-rw-rw-   0 root         (0) root         (0)     5740 2024-03-15 15:00:47.000000 iLCDirac-35.0.2/src/ILCDIRAC/Workflow/Modules/RootMacroAnalysis.py
--rw-rw-rw-   0 root         (0) root         (0)     4935 2024-03-15 15:00:47.000000 iLCDirac-35.0.2/src/ILCDIRAC/Workflow/Modules/SIDRegisterOutputData.py
--rw-rw-rw-   0 root         (0) root         (0)    11639 2024-03-15 15:00:47.000000 iLCDirac-35.0.2/src/ILCDIRAC/Workflow/Modules/SLICAnalysis.py
--rw-rw-rw-   0 root         (0) root         (0)    11192 2024-03-15 15:00:47.000000 iLCDirac-35.0.2/src/ILCDIRAC/Workflow/Modules/SLICPandoraAnalysis.py
--rw-rw-rw-   0 root         (0) root         (0)     4044 2024-03-15 15:00:47.000000 iLCDirac-35.0.2/src/ILCDIRAC/Workflow/Modules/StdHepConverter.py
--rw-rw-rw-   0 root         (0) root         (0)     9340 2024-03-15 15:00:47.000000 iLCDirac-35.0.2/src/ILCDIRAC/Workflow/Modules/StdHepCut.py
--rw-rw-rw-   0 root         (0) root         (0)     3020 2024-03-15 15:00:47.000000 iLCDirac-35.0.2/src/ILCDIRAC/Workflow/Modules/StdHepCutJava.py
--rw-rw-rw-   0 root         (0) root         (0)     8569 2024-03-15 15:00:47.000000 iLCDirac-35.0.2/src/ILCDIRAC/Workflow/Modules/StdHepSplit.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-15 15:01:06.557158 iLCDirac-35.0.2/src/ILCDIRAC/Workflow/Modules/Test/
--rw-rw-rw-   0 root         (0) root         (0)     2311 2024-03-15 15:00:47.000000 iLCDirac-35.0.2/src/ILCDIRAC/Workflow/Modules/Test/MakeRequest.py
--rw-rw-rw-   0 root         (0) root         (0)    12596 2024-03-15 15:00:47.000000 iLCDirac-35.0.2/src/ILCDIRAC/Workflow/Modules/Test/Test_BabayagaAnalysis.py
--rw-rw-rw-   0 root         (0) root         (0)    13750 2024-03-15 15:00:47.000000 iLCDirac-35.0.2/src/ILCDIRAC/Workflow/Modules/Test/Test_BhlumiAnalysis.py
--rw-rw-rw-   0 root         (0) root         (0)    14814 2024-03-15 15:00:47.000000 iLCDirac-35.0.2/src/ILCDIRAC/Workflow/Modules/Test/Test_Calibration.py
--rw-rw-rw-   0 root         (0) root         (0)    45457 2024-03-15 15:00:47.000000 iLCDirac-35.0.2/src/ILCDIRAC/Workflow/Modules/Test/Test_DDSimWorkflow.py
--rw-rw-rw-   0 root         (0) root         (0)    20933 2024-03-15 15:00:47.000000 iLCDirac-35.0.2/src/ILCDIRAC/Workflow/Modules/Test/Test_DelphesAppModule.py
--rw-rw-rw-   0 root         (0) root         (0)    28578 2024-03-15 15:00:47.000000 iLCDirac-35.0.2/src/ILCDIRAC/Workflow/Modules/Test/Test_FccAnalysis.py
--rw-rw-rw-   0 root         (0) root         (0)    20006 2024-03-15 15:00:47.000000 iLCDirac-35.0.2/src/ILCDIRAC/Workflow/Modules/Test/Test_GaudiAppModule.py
--rw-rw-rw-   0 root         (0) root         (0)    11611 2024-03-15 15:00:47.000000 iLCDirac-35.0.2/src/ILCDIRAC/Workflow/Modules/Test/Test_KKMCAnalysis.py
--rw-rw-rw-   0 root         (0) root         (0)    45397 2024-03-15 15:00:47.000000 iLCDirac-35.0.2/src/ILCDIRAC/Workflow/Modules/Test/Test_MarlinAnalysis.py
--rw-rw-rw-   0 root         (0) root         (0)    43848 2024-03-15 15:00:47.000000 iLCDirac-35.0.2/src/ILCDIRAC/Workflow/Modules/Test/Test_ModuleBase.py
--rw-rw-rw-   0 root         (0) root         (0)    41500 2024-03-15 15:00:47.000000 iLCDirac-35.0.2/src/ILCDIRAC/Workflow/Modules/Test/Test_OverlayInput.py
--rw-rw-rw-   0 root         (0) root         (0)    10867 2024-03-15 15:00:47.000000 iLCDirac-35.0.2/src/ILCDIRAC/Workflow/Modules/Test/Test_RegisterOutputData.py
--rw-rw-rw-   0 root         (0) root         (0)     2626 2024-03-15 15:00:47.000000 iLCDirac-35.0.2/src/ILCDIRAC/Workflow/Modules/Test/Test_ReportErrors.py
--rw-rw-rw-   0 root         (0) root         (0)     8844 2024-03-15 15:00:47.000000 iLCDirac-35.0.2/src/ILCDIRAC/Workflow/Modules/Test/Test_RootExecutableAnalysis.py
--rw-rw-rw-   0 root         (0) root         (0)    28021 2024-03-15 15:00:47.000000 iLCDirac-35.0.2/src/ILCDIRAC/Workflow/Modules/Test/Test_SLICPandoraAnalysis.py
--rw-rw-rw-   0 root         (0) root         (0)     3462 2024-03-15 15:00:47.000000 iLCDirac-35.0.2/src/ILCDIRAC/Workflow/Modules/Test/Test_SlicPandora.py
--rw-rw-rw-   0 root         (0) root         (0)    19461 2024-03-15 15:00:47.000000 iLCDirac-35.0.2/src/ILCDIRAC/Workflow/Modules/Test/Test_StdHepCut.py
--rw-rw-rw-   0 root         (0) root         (0)    14457 2024-03-15 15:00:47.000000 iLCDirac-35.0.2/src/ILCDIRAC/Workflow/Modules/Test/Test_StdHepSplit.py
--rw-rw-rw-   0 root         (0) root         (0)    12973 2024-03-15 15:00:47.000000 iLCDirac-35.0.2/src/ILCDIRAC/Workflow/Modules/Test/Test_UploadLogFile.py
--rw-rw-rw-   0 root         (0) root         (0)    10007 2024-03-15 15:00:47.000000 iLCDirac-35.0.2/src/ILCDIRAC/Workflow/Modules/Test/Test_UploadOutputData.py
--rw-rw-rw-   0 root         (0) root         (0)    32143 2024-03-15 15:00:47.000000 iLCDirac-35.0.2/src/ILCDIRAC/Workflow/Modules/Test/Test_UserJobFinalization.py
--rw-rw-rw-   0 root         (0) root         (0)    14235 2024-03-15 15:00:47.000000 iLCDirac-35.0.2/src/ILCDIRAC/Workflow/Modules/Test/Test_Whizard2Workflow.py
--rw-rw-rw-   0 root         (0) root         (0)    67243 2024-03-15 15:00:47.000000 iLCDirac-35.0.2/src/ILCDIRAC/Workflow/Modules/Test/Test_WhizardAnalysis.py
--rw-rw-rw-   0 root         (0) root         (0)    86847 2024-03-15 15:00:47.000000 iLCDirac-35.0.2/src/ILCDIRAC/Workflow/Modules/Test/Test_WorkflowModuleRequests.py
--rw-rw-rw-   0 root         (0) root         (0)     6505 2024-03-15 15:00:47.000000 iLCDirac-35.0.2/src/ILCDIRAC/Workflow/Modules/TomatoAnalysis.py
--rw-rw-rw-   0 root         (0) root         (0)    17704 2024-03-15 15:00:47.000000 iLCDirac-35.0.2/src/ILCDIRAC/Workflow/Modules/UploadLogFile.py
--rw-rw-rw-   0 root         (0) root         (0)    15076 2024-03-15 15:00:47.000000 iLCDirac-35.0.2/src/ILCDIRAC/Workflow/Modules/UploadOutputData.py
--rw-rw-rw-   0 root         (0) root         (0)    17792 2024-03-15 15:00:47.000000 iLCDirac-35.0.2/src/ILCDIRAC/Workflow/Modules/UserJobFinalization.py
--rw-rw-rw-   0 root         (0) root         (0)    10190 2024-03-15 15:00:47.000000 iLCDirac-35.0.2/src/ILCDIRAC/Workflow/Modules/Whizard2Analysis.py
--rw-rw-rw-   0 root         (0) root         (0)    22938 2024-03-15 15:00:47.000000 iLCDirac-35.0.2/src/ILCDIRAC/Workflow/Modules/WhizardAnalysis.py
--rw-rw-rw-   0 root         (0) root         (0)     1130 2024-03-15 15:00:47.000000 iLCDirac-35.0.2/src/ILCDIRAC/Workflow/Modules/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-15 15:01:06.558158 iLCDirac-35.0.2/src/ILCDIRAC/Workflow/Utilities/
--rw-rw-rw-   0 root         (0) root         (0)     3265 2024-03-15 15:00:47.000000 iLCDirac-35.0.2/src/ILCDIRAC/Workflow/Utilities/CompactMixin.py
--rw-rw-rw-   0 root         (0) root         (0)     5501 2024-03-15 15:00:47.000000 iLCDirac-35.0.2/src/ILCDIRAC/Workflow/Utilities/DD4hepMixin.py
--rw-rw-rw-   0 root         (0) root         (0)     2714 2024-03-15 15:00:47.000000 iLCDirac-35.0.2/src/ILCDIRAC/Workflow/Utilities/RootMixin.py
--rw-rw-rw-   0 root         (0) root         (0)     1066 2024-03-15 15:00:47.000000 iLCDirac-35.0.2/src/ILCDIRAC/Workflow/Utilities/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1167 2024-03-15 15:00:47.000000 iLCDirac-35.0.2/src/ILCDIRAC/Workflow/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-15 15:01:06.558158 iLCDirac-35.0.2/src/ILCDIRAC/WorkloadManagementSystem/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-15 15:01:06.559158 iLCDirac-35.0.2/src/ILCDIRAC/WorkloadManagementSystem/Agent/
--rw-rw-rw-   0 root         (0) root         (0)    24475 2024-03-15 15:00:47.000000 iLCDirac-35.0.2/src/ILCDIRAC/WorkloadManagementSystem/Agent/JobResetAgent.py
--rw-rw-rw-   0 root         (0) root         (0)     1013 2024-03-15 15:00:47.000000 iLCDirac-35.0.2/src/ILCDIRAC/WorkloadManagementSystem/Agent/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-15 15:01:06.559158 iLCDirac-35.0.2/src/ILCDIRAC/WorkloadManagementSystem/Client/
--rw-rw-rw-   0 root         (0) root         (0)    15894 2024-03-15 15:00:47.000000 iLCDirac-35.0.2/src/ILCDIRAC/WorkloadManagementSystem/Client/DownloadInputData.py
--rw-rw-rw-   0 root         (0) root         (0)     1083 2024-03-15 15:00:47.000000 iLCDirac-35.0.2/src/ILCDIRAC/WorkloadManagementSystem/Client/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      498 2024-03-15 15:00:47.000000 iLCDirac-35.0.2/src/ILCDIRAC/WorkloadManagementSystem/ConfigTemplate.cfg
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-15 15:01:06.560158 iLCDirac-35.0.2/src/ILCDIRAC/WorkloadManagementSystem/Executor/
--rw-rw-rw-   0 root         (0) root         (0)     5646 2024-03-15 15:00:47.000000 iLCDirac-35.0.2/src/ILCDIRAC/WorkloadManagementSystem/Executor/SoftwareVersions.py
--rw-rw-rw-   0 root         (0) root         (0)     1082 2024-03-15 15:00:47.000000 iLCDirac-35.0.2/src/ILCDIRAC/WorkloadManagementSystem/Executor/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-15 15:01:06.561158 iLCDirac-35.0.2/src/ILCDIRAC/WorkloadManagementSystem/Tests/
--rw-rw-rw-   0 root         (0) root         (0)    13587 2024-03-15 15:00:47.000000 iLCDirac-35.0.2/src/ILCDIRAC/WorkloadManagementSystem/Tests/Test_Client_DownloadInputData.py
--rw-rw-rw-   0 root         (0) root         (0)    31624 2024-03-15 15:00:47.000000 iLCDirac-35.0.2/src/ILCDIRAC/WorkloadManagementSystem/Tests/Test_JobResetAgent.py
--rw-rw-rw-   0 root         (0) root         (0)     3345 2024-03-15 15:00:47.000000 iLCDirac-35.0.2/src/ILCDIRAC/WorkloadManagementSystem/Tests/Test_SoftwareVersions.py
--rw-rw-rw-   0 root         (0) root         (0)     1083 2024-03-15 15:00:47.000000 iLCDirac-35.0.2/src/ILCDIRAC/WorkloadManagementSystem/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     2395 2024-03-15 15:00:47.000000 iLCDirac-35.0.2/src/ILCDIRAC/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-15 15:01:06.563158 iLCDirac-35.0.2/src/iLCDirac.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2175 2024-03-15 15:01:06.000000 iLCDirac-35.0.2/src/iLCDirac.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)    25074 2024-03-15 15:01:06.000000 iLCDirac-35.0.2/src/iLCDirac.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-03-15 15:01:06.000000 iLCDirac-35.0.2/src/iLCDirac.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)     2121 2024-03-15 15:01:06.000000 iLCDirac-35.0.2/src/iLCDirac.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-03-15 15:01:05.000000 iLCDirac-35.0.2/src/iLCDirac.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)      297 2024-03-15 15:01:06.000000 iLCDirac-35.0.2/src/iLCDirac.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        9 2024-03-15 15:01:06.000000 iLCDirac-35.0.2/src/iLCDirac.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-16 15:47:28.393816 ilcdirac-35.0.3/
+-rw-rw-rw-   0 root         (0) root         (0)    32452 2024-04-16 15:47:11.000000 ilcdirac-35.0.3/LICENSE
+-rw-rw-rw-   0 root         (0) root         (0)      142 2024-04-16 15:47:11.000000 ilcdirac-35.0.3/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     2178 2024-04-16 15:47:28.393816 ilcdirac-35.0.3/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)      241 2024-04-16 15:47:11.000000 ilcdirac-35.0.3/README.md
+-rw-rw-rw-   0 root         (0) root         (0)      463 2024-04-16 15:47:11.000000 ilcdirac-35.0.3/pyproject.toml
+-rw-rw-rw-   0 root         (0) root         (0)      361 2024-04-16 15:47:11.000000 ilcdirac-35.0.3/pytest.ini
+-rw-rw-rw-   0 root         (0) root         (0)    86194 2024-04-16 15:47:11.000000 ilcdirac-35.0.3/release.notes
+-rw-rw-rw-   0 root         (0) root         (0)    27753 2024-04-16 15:47:11.000000 ilcdirac-35.0.3/releases.cfg
+-rw-rw-rw-   0 root         (0) root         (0)     4392 2024-04-16 15:47:28.394816 ilcdirac-35.0.3/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)      276 2024-04-16 15:47:11.000000 ilcdirac-35.0.3/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-16 15:47:28.283817 ilcdirac-35.0.3/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-16 15:47:28.286817 ilcdirac-35.0.3/src/ILCDIRAC/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-16 15:47:28.286817 ilcdirac-35.0.3/src/ILCDIRAC/CalibrationSystem/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-16 15:47:28.287817 ilcdirac-35.0.3/src/ILCDIRAC/CalibrationSystem/Agent/
+-rw-rw-rw-   0 root         (0) root         (0)    10978 2024-04-16 15:47:11.000000 ilcdirac-35.0.3/src/ILCDIRAC/CalibrationSystem/Agent/CalibrationAgent.py
+-rw-rw-rw-   0 root         (0) root         (0)     1013 2024-04-16 15:47:11.000000 ilcdirac-35.0.3/src/ILCDIRAC/CalibrationSystem/Agent/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-16 15:47:28.287817 ilcdirac-35.0.3/src/ILCDIRAC/CalibrationSystem/Client/
+-rw-rw-rw-   0 root         (0) root         (0)     6343 2024-04-16 15:47:11.000000 ilcdirac-35.0.3/src/ILCDIRAC/CalibrationSystem/Client/CalibrationClient.py
+-rw-rw-rw-   0 root         (0) root         (0)     1013 2024-04-16 15:47:11.000000 ilcdirac-35.0.3/src/ILCDIRAC/CalibrationSystem/Client/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      527 2024-04-16 15:47:11.000000 ilcdirac-35.0.3/src/ILCDIRAC/CalibrationSystem/ConfigTemplate.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-16 15:47:28.288817 ilcdirac-35.0.3/src/ILCDIRAC/CalibrationSystem/Service/
+-rw-rw-rw-   0 root         (0) root         (0)    36181 2024-04-16 15:47:11.000000 ilcdirac-35.0.3/src/ILCDIRAC/CalibrationSystem/Service/CalibrationHandler.py
+-rw-rw-rw-   0 root         (0) root         (0)    44494 2024-04-16 15:47:11.000000 ilcdirac-35.0.3/src/ILCDIRAC/CalibrationSystem/Service/CalibrationRun.py
+-rw-rw-rw-   0 root         (0) root         (0)     5951 2024-04-16 15:47:11.000000 ilcdirac-35.0.3/src/ILCDIRAC/CalibrationSystem/Service/DetectorSettings.py
+-rw-rw-rw-   0 root         (0) root         (0)     1013 2024-04-16 15:47:11.000000 ilcdirac-35.0.3/src/ILCDIRAC/CalibrationSystem/Service/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     3971 2024-04-16 15:47:11.000000 ilcdirac-35.0.3/src/ILCDIRAC/CalibrationSystem/TODO
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-16 15:47:28.290817 ilcdirac-35.0.3/src/ILCDIRAC/CalibrationSystem/Test/
+-rw-rw-rw-   0 root         (0) root         (0)    14462 2024-04-16 15:47:11.000000 ilcdirac-35.0.3/src/ILCDIRAC/CalibrationSystem/Test/Test_CalibrationAgent.py
+-rw-rw-rw-   0 root         (0) root         (0)     2255 2024-04-16 15:47:11.000000 ilcdirac-35.0.3/src/ILCDIRAC/CalibrationSystem/Test/Test_CalibrationClient.py
+-rw-rw-rw-   0 root         (0) root         (0)    51085 2024-04-16 15:47:11.000000 ilcdirac-35.0.3/src/ILCDIRAC/CalibrationSystem/Test/Test_CalibrationService.py
+-rw-rw-rw-   0 root         (0) root         (0)     2037 2024-04-16 15:47:11.000000 ilcdirac-35.0.3/src/ILCDIRAC/CalibrationSystem/Test/Test_Util_fileutils.py
+-rw-rw-rw-   0 root         (0) root         (0)     9201 2024-04-16 15:47:11.000000 ilcdirac-35.0.3/src/ILCDIRAC/CalibrationSystem/Test/Test_Util_functions.py
+-rw-rw-rw-   0 root         (0) root         (0)     1013 2024-04-16 15:47:11.000000 ilcdirac-35.0.3/src/ILCDIRAC/CalibrationSystem/Test/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-16 15:47:28.291817 ilcdirac-35.0.3/src/ILCDIRAC/CalibrationSystem/Utilities/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-16 15:47:28.294817 ilcdirac-35.0.3/src/ILCDIRAC/CalibrationSystem/Utilities/Python_Read_Scripts/
+-rw-rw-rw-   0 root         (0) root         (0)     3152 2024-04-16 15:47:11.000000 ilcdirac-35.0.3/src/ILCDIRAC/CalibrationSystem/Utilities/Python_Read_Scripts/ECal_Digi_Extract.py
+-rw-rw-rw-   0 root         (0) root         (0)     1811 2024-04-16 15:47:11.000000 ilcdirac-35.0.3/src/ILCDIRAC/CalibrationSystem/Utilities/Python_Read_Scripts/EM_Extract.py
+-rw-rw-rw-   0 root         (0) root         (0)     1494 2024-04-16 15:47:11.000000 ilcdirac-35.0.3/src/ILCDIRAC/CalibrationSystem/Utilities/Python_Read_Scripts/Extract_GeVToMIP.py
+-rw-rw-rw-   0 root         (0) root         (0)      945 2024-04-16 15:47:11.000000 ilcdirac-35.0.3/src/ILCDIRAC/CalibrationSystem/Utilities/Python_Read_Scripts/Extract_SimCaloHitMIPMPV.py
+-rw-rw-rw-   0 root         (0) root         (0)     2867 2024-04-16 15:47:11.000000 ilcdirac-35.0.3/src/ILCDIRAC/CalibrationSystem/Utilities/Python_Read_Scripts/Final_Calibration.py
+-rw-rw-rw-   0 root         (0) root         (0)     2682 2024-04-16 15:47:11.000000 ilcdirac-35.0.3/src/ILCDIRAC/CalibrationSystem/Utilities/Python_Read_Scripts/Final_Calibration.py.orig
+-rw-rw-rw-   0 root         (0) root         (0)     2388 2024-04-16 15:47:11.000000 ilcdirac-35.0.3/src/ILCDIRAC/CalibrationSystem/Utilities/Python_Read_Scripts/HCal_Digi_Extract.py
+-rw-rw-rw-   0 root         (0) root         (0)     1456 2024-04-16 15:47:11.000000 ilcdirac-35.0.3/src/ILCDIRAC/CalibrationSystem/Utilities/Python_Read_Scripts/HCal_Direction_Corrections_Extract.py
+-rw-rw-rw-   0 root         (0) root         (0)     1487 2024-04-16 15:47:11.000000 ilcdirac-35.0.3/src/ILCDIRAC/CalibrationSystem/Utilities/Python_Read_Scripts/HCal_Ring_Digi_Extract.py
+-rw-rw-rw-   0 root         (0) root         (0)     3967 2024-04-16 15:47:11.000000 ilcdirac-35.0.3/src/ILCDIRAC/CalibrationSystem/Utilities/Python_Read_Scripts/HCal_Ring_Gear_Information.py
+-rw-rw-rw-   0 root         (0) root         (0)     4968 2024-04-16 15:47:11.000000 ilcdirac-35.0.3/src/ILCDIRAC/CalibrationSystem/Utilities/Python_Read_Scripts/Had_Extract.py
+-rw-rw-rw-   0 root         (0) root         (0)      220 2024-04-16 15:47:11.000000 ilcdirac-35.0.3/src/ILCDIRAC/CalibrationSystem/Utilities/Python_Read_Scripts/Helper_Functions.py
+-rw-rw-rw-   0 root         (0) root         (0)     3579 2024-04-16 15:47:11.000000 ilcdirac-35.0.3/src/ILCDIRAC/CalibrationSystem/Utilities/Python_Read_Scripts/Python_Read_Scripts.tgz
+-rw-rw-rw-   0 root         (0) root         (0)     1013 2024-04-16 15:47:11.000000 ilcdirac-35.0.3/src/ILCDIRAC/CalibrationSystem/Utilities/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-16 15:47:28.295817 ilcdirac-35.0.3/src/ILCDIRAC/CalibrationSystem/Utilities/auxiliaryFiles/
+-rw-rw-rw-   0 root         (0) root         (0)     1765 2024-04-16 15:47:11.000000 ilcdirac-35.0.3/src/ILCDIRAC/CalibrationSystem/Utilities/auxiliaryFiles/parameterListMarlinSteeringFile.txt
+-rw-rw-rw-   0 root         (0) root         (0)     3928 2024-04-16 15:47:11.000000 ilcdirac-35.0.3/src/ILCDIRAC/CalibrationSystem/Utilities/auxiliaryFiles/pfoAnalysis.xml
+-rw-rw-rw-   0 root         (0) root         (0)     1484 2024-04-16 15:47:11.000000 ilcdirac-35.0.3/src/ILCDIRAC/CalibrationSystem/Utilities/fileutils.py
+-rw-rw-rw-   0 root         (0) root         (0)    12301 2024-04-16 15:47:11.000000 ilcdirac-35.0.3/src/ILCDIRAC/CalibrationSystem/Utilities/functions.py
+-rw-rw-rw-   0 root         (0) root         (0)     4433 2024-04-16 15:47:11.000000 ilcdirac-35.0.3/src/ILCDIRAC/CalibrationSystem/Utilities/mergePandoraLikelihoodData.py
+-rw-rw-rw-   0 root         (0) root         (0)     1668 2024-04-16 15:47:11.000000 ilcdirac-35.0.3/src/ILCDIRAC/CalibrationSystem/Utilities/objectFactory.py
+-rw-rw-rw-   0 root         (0) root         (0)     1013 2024-04-16 15:47:11.000000 ilcdirac-35.0.3/src/ILCDIRAC/CalibrationSystem/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2943 2024-04-16 15:47:11.000000 ilcdirac-35.0.3/src/ILCDIRAC/CalibrationSystem/dev_create_events.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-16 15:47:28.295817 ilcdirac-35.0.3/src/ILCDIRAC/Core/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-16 15:47:28.303817 ilcdirac-35.0.3/src/ILCDIRAC/Core/Utilities/
+-rw-rw-rw-   0 root         (0) root         (0)     3755 2024-04-16 15:47:11.000000 ilcdirac-35.0.3/src/ILCDIRAC/Core/Utilities/CheckAndGetProdProxy.py
+-rw-rw-rw-   0 root         (0) root         (0)     1767 2024-04-16 15:47:11.000000 ilcdirac-35.0.3/src/ILCDIRAC/Core/Utilities/CheckXMLValidity.py
+-rw-rw-rw-   0 root         (0) root         (0)    15260 2024-04-16 15:47:11.000000 ilcdirac-35.0.3/src/ILCDIRAC/Core/Utilities/CombinedSoftwareInstallation.py
+-rw-rw-rw-   0 root         (0) root         (0)     1903 2024-04-16 15:47:11.000000 ilcdirac-35.0.3/src/ILCDIRAC/Core/Utilities/Configuration.py
+-rw-rw-rw-   0 root         (0) root         (0)    18781 2024-04-16 15:47:11.000000 ilcdirac-35.0.3/src/ILCDIRAC/Core/Utilities/DetectOS.py
+-rw-rw-rw-   0 root         (0) root         (0)     4861 2024-04-16 15:47:11.000000 ilcdirac-35.0.3/src/ILCDIRAC/Core/Utilities/FileUtils.py
+-rw-rw-rw-   0 root         (0) root         (0)     9749 2024-04-16 15:47:11.000000 ilcdirac-35.0.3/src/ILCDIRAC/Core/Utilities/FilenameEncoder.py
+-rw-rw-rw-   0 root         (0) root         (0)     2767 2024-04-16 15:47:11.000000 ilcdirac-35.0.3/src/ILCDIRAC/Core/Utilities/FindSteeringFileDir.py
+-rw-rw-rw-   0 root         (0) root         (0)     4110 2024-04-16 15:47:11.000000 ilcdirac-35.0.3/src/ILCDIRAC/Core/Utilities/GeneratorModels.py
+-rw-rw-rw-   0 root         (0) root         (0)    17917 2024-04-16 15:47:11.000000 ilcdirac-35.0.3/src/ILCDIRAC/Core/Utilities/HTML.py
+-rw-rw-rw-   0 root         (0) root         (0)     6866 2024-04-16 15:47:11.000000 ilcdirac-35.0.3/src/ILCDIRAC/Core/Utilities/InputDataResolution.py
+-rw-rw-rw-   0 root         (0) root         (0)     4246 2024-04-16 15:47:11.000000 ilcdirac-35.0.3/src/ILCDIRAC/Core/Utilities/InputFilesUtilities.py
+-rw-rw-rw-   0 root         (0) root         (0)     5550 2024-04-16 15:47:11.000000 ilcdirac-35.0.3/src/ILCDIRAC/Core/Utilities/InstalledFiles.py
+-rw-rw-rw-   0 root         (0) root         (0)     2805 2024-04-16 15:47:11.000000 ilcdirac-35.0.3/src/ILCDIRAC/Core/Utilities/JobPathResolution.py
+-rw-rw-rw-   0 root         (0) root         (0)     2311 2024-04-16 15:47:11.000000 ilcdirac-35.0.3/src/ILCDIRAC/Core/Utilities/LFNPathUtilities.py
+-rw-rw-rw-   0 root         (0) root         (0)     7040 2024-04-16 15:47:11.000000 ilcdirac-35.0.3/src/ILCDIRAC/Core/Utilities/MarlinXML.py
+-rw-rw-rw-   0 root         (0) root         (0)     3285 2024-04-16 15:47:11.000000 ilcdirac-35.0.3/src/ILCDIRAC/Core/Utilities/OutputDataPolicy.py
+-rw-rw-rw-   0 root         (0) root         (0)     3601 2024-04-16 15:47:11.000000 ilcdirac-35.0.3/src/ILCDIRAC/Core/Utilities/OverlayFiles.py
+-rw-rw-rw-   0 root         (0) root         (0)     2856 2024-04-16 15:47:11.000000 ilcdirac-35.0.3/src/ILCDIRAC/Core/Utilities/PrepareLibs.py
+-rw-rw-rw-   0 root         (0) root         (0)    38627 2024-04-16 15:47:11.000000 ilcdirac-35.0.3/src/ILCDIRAC/Core/Utilities/PrepareOptionFiles.py
+-rw-rw-rw-   0 root         (0) root         (0)     7483 2024-04-16 15:47:11.000000 ilcdirac-35.0.3/src/ILCDIRAC/Core/Utilities/ProcessList.py
+-rw-rw-rw-   0 root         (0) root         (0)    11004 2024-04-16 15:47:11.000000 ilcdirac-35.0.3/src/ILCDIRAC/Core/Utilities/ProductionData.py
+-rw-rw-rw-   0 root         (0) root         (0)     3993 2024-04-16 15:47:11.000000 ilcdirac-35.0.3/src/ILCDIRAC/Core/Utilities/RemoveSoft.py
+-rw-rw-rw-   0 root         (0) root         (0)     2690 2024-04-16 15:47:11.000000 ilcdirac-35.0.3/src/ILCDIRAC/Core/Utilities/ResolveDependencies.py
+-rw-rw-rw-   0 root         (0) root         (0)     4689 2024-04-16 15:47:11.000000 ilcdirac-35.0.3/src/ILCDIRAC/Core/Utilities/ResolveSE.py
+-rw-rw-rw-   0 root         (0) root         (0)     1804 2024-04-16 15:47:11.000000 ilcdirac-35.0.3/src/ILCDIRAC/Core/Utilities/Splitting.py
+-rw-rw-rw-   0 root         (0) root         (0)    21977 2024-04-16 15:47:11.000000 ilcdirac-35.0.3/src/ILCDIRAC/Core/Utilities/TARsoft.py
+-rw-rw-rw-   0 root         (0) root         (0)     2868 2024-04-16 15:47:11.000000 ilcdirac-35.0.3/src/ILCDIRAC/Core/Utilities/Utilities.py
+-rw-rw-rw-   0 root         (0) root         (0)     1898 2024-04-16 15:47:11.000000 ilcdirac-35.0.3/src/ILCDIRAC/Core/Utilities/WasteCPU.py
+-rw-rw-rw-   0 root         (0) root         (0)    41912 2024-04-16 15:47:11.000000 ilcdirac-35.0.3/src/ILCDIRAC/Core/Utilities/WhizardOptions.py
+-rw-rw-rw-   0 root         (0) root         (0)     1100 2024-04-16 15:47:11.000000 ilcdirac-35.0.3/src/ILCDIRAC/Core/Utilities/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     6604 2024-04-16 15:47:11.000000 ilcdirac-35.0.3/src/ILCDIRAC/Core/Utilities/resolvePathsAndNames.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-16 15:47:28.309817 ilcdirac-35.0.3/src/ILCDIRAC/Core/Utilities/tests/
+-rw-rw-rw-   0 root         (0) root         (0)     6226 2024-04-16 15:47:11.000000 ilcdirac-35.0.3/src/ILCDIRAC/Core/Utilities/tests/Test_CheckAndGetProd.py
+-rw-rw-rw-   0 root         (0) root         (0)    32396 2024-04-16 15:47:11.000000 ilcdirac-35.0.3/src/ILCDIRAC/Core/Utilities/tests/Test_CombinedSoftwareInstallation.py
+-rw-rw-rw-   0 root         (0) root         (0)     2440 2024-04-16 15:47:11.000000 ilcdirac-35.0.3/src/ILCDIRAC/Core/Utilities/tests/Test_Configuration.py
+-rw-rw-rw-   0 root         (0) root         (0)    23878 2024-04-16 15:47:11.000000 ilcdirac-35.0.3/src/ILCDIRAC/Core/Utilities/tests/Test_DetectOS.py
+-rw-rw-rw-   0 root         (0) root         (0)    17273 2024-04-16 15:47:11.000000 ilcdirac-35.0.3/src/ILCDIRAC/Core/Utilities/tests/Test_FileUtils.py
+-rw-rw-rw-   0 root         (0) root         (0)    16707 2024-04-16 15:47:11.000000 ilcdirac-35.0.3/src/ILCDIRAC/Core/Utilities/tests/Test_FilenameEncoder.py
+-rw-rw-rw-   0 root         (0) root         (0)     4872 2024-04-16 15:47:11.000000 ilcdirac-35.0.3/src/ILCDIRAC/Core/Utilities/tests/Test_FindSteeringFileDir.py
+-rw-rw-rw-   0 root         (0) root         (0)    10164 2024-04-16 15:47:11.000000 ilcdirac-35.0.3/src/ILCDIRAC/Core/Utilities/tests/Test_InputDataResolution.py
+-rw-rw-rw-   0 root         (0) root         (0)     7506 2024-04-16 15:47:11.000000 ilcdirac-35.0.3/src/ILCDIRAC/Core/Utilities/tests/Test_InputFilesUtilities.py
+-rw-rw-rw-   0 root         (0) root         (0)     2277 2024-04-16 15:47:11.000000 ilcdirac-35.0.3/src/ILCDIRAC/Core/Utilities/tests/Test_LFNPathUtilities.py
+-rw-rw-rw-   0 root         (0) root         (0)    18959 2024-04-16 15:47:11.000000 ilcdirac-35.0.3/src/ILCDIRAC/Core/Utilities/tests/Test_OutputDataPolicy.py
+-rw-rw-rw-   0 root         (0) root         (0)     2654 2024-04-16 15:47:11.000000 ilcdirac-35.0.3/src/ILCDIRAC/Core/Utilities/tests/Test_OverlayFiles.py
+-rw-rw-rw-   0 root         (0) root         (0)     6803 2024-04-16 15:47:11.000000 ilcdirac-35.0.3/src/ILCDIRAC/Core/Utilities/tests/Test_PrepareLibs.py
+-rw-rw-rw-   0 root         (0) root         (0)    26585 2024-04-16 15:47:11.000000 ilcdirac-35.0.3/src/ILCDIRAC/Core/Utilities/tests/Test_PrepareMarlinXML.py
+-rw-rw-rw-   0 root         (0) root         (0)    86014 2024-04-16 15:47:11.000000 ilcdirac-35.0.3/src/ILCDIRAC/Core/Utilities/tests/Test_PrepareOptionsFiles.py
+-rw-rw-rw-   0 root         (0) root         (0)    14816 2024-04-16 15:47:11.000000 ilcdirac-35.0.3/src/ILCDIRAC/Core/Utilities/tests/Test_ProcessList.py
+-rw-rw-rw-   0 root         (0) root         (0)     6220 2024-04-16 15:47:11.000000 ilcdirac-35.0.3/src/ILCDIRAC/Core/Utilities/tests/Test_ProductionData.py
+-rw-rw-rw-   0 root         (0) root         (0)     4230 2024-04-16 15:47:11.000000 ilcdirac-35.0.3/src/ILCDIRAC/Core/Utilities/tests/Test_ProductionOutputData.py
+-rw-rw-rw-   0 root         (0) root         (0)    11294 2024-04-16 15:47:11.000000 ilcdirac-35.0.3/src/ILCDIRAC/Core/Utilities/tests/Test_ResolvePathsandNames.py
+-rw-rw-rw-   0 root         (0) root         (0)     9475 2024-04-16 15:47:11.000000 ilcdirac-35.0.3/src/ILCDIRAC/Core/Utilities/tests/Test_ResolveSEs.py
+-rw-rw-rw-   0 root         (0) root         (0)     2278 2024-04-16 15:47:11.000000 ilcdirac-35.0.3/src/ILCDIRAC/Core/Utilities/tests/Test_Splitting.py
+-rw-rw-rw-   0 root         (0) root         (0)    72966 2024-04-16 15:47:11.000000 ilcdirac-35.0.3/src/ILCDIRAC/Core/Utilities/tests/Test_TARsoft.py
+-rw-rw-rw-   0 root         (0) root         (0)     3214 2024-04-16 15:47:11.000000 ilcdirac-35.0.3/src/ILCDIRAC/Core/Utilities/tests/Test_Utilities.py
+-rw-rw-rw-   0 root         (0) root         (0)     2480 2024-04-16 15:47:11.000000 ilcdirac-35.0.3/src/ILCDIRAC/Core/Utilities/tests/Test_WasteCPU.py
+-rw-rw-rw-   0 root         (0) root         (0)    26730 2024-04-16 15:47:11.000000 ilcdirac-35.0.3/src/ILCDIRAC/Core/Utilities/tests/Test_WhizardOptions.py
+-rw-rw-rw-   0 root         (0) root         (0)     1180 2024-04-16 15:47:11.000000 ilcdirac-35.0.3/src/ILCDIRAC/Core/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-16 15:47:28.313817 ilcdirac-35.0.3/src/ILCDIRAC/Core/scripts/
+-rw-rw-rw-   0 root         (0) root         (0)     1086 2024-04-16 15:47:11.000000 ilcdirac-35.0.3/src/ILCDIRAC/Core/scripts/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2720 2024-04-16 15:47:11.000000 ilcdirac-35.0.3/src/ILCDIRAC/Core/scripts/createJavaTarBall.sh
+-rwxrwxrwx   0 root         (0) root         (0)     3224 2024-04-16 15:47:11.000000 ilcdirac-35.0.3/src/ILCDIRAC/Core/scripts/createLCIOTarBall.sh
+-rwxrwxrwx   0 root         (0) root         (0)     6151 2024-04-16 15:47:11.000000 ilcdirac-35.0.3/src/ILCDIRAC/Core/scripts/createMarlinTarBall.sh
+-rwxrwxrwx   0 root         (0) root         (0)     6706 2024-04-16 15:47:11.000000 ilcdirac-35.0.3/src/ILCDIRAC/Core/scripts/createMokkaTarBall.sh
+-rwxrwxrwx   0 root         (0) root         (0)     3200 2024-04-16 15:47:11.000000 ilcdirac-35.0.3/src/ILCDIRAC/Core/scripts/createSlicPandoraTarBall.sh
+-rwxrwxrwx   0 root         (0) root         (0)     2307 2024-04-16 15:47:11.000000 ilcdirac-35.0.3/src/ILCDIRAC/Core/scripts/createTarBallForProgram.sh
+-rwxrwxrwx   0 root         (0) root         (0)     9197 2024-04-16 15:47:11.000000 ilcdirac-35.0.3/src/ILCDIRAC/Core/scripts/dirac-architecture
+-rw-rw-rw-   0 root         (0) root         (0)    16952 2024-04-16 15:47:11.000000 ilcdirac-35.0.3/src/ILCDIRAC/Core/scripts/dirac_ilc_add_cvmfs_software.py
+-rw-rw-rw-   0 root         (0) root         (0)    10488 2024-04-16 15:47:11.000000 ilcdirac-35.0.3/src/ILCDIRAC/Core/scripts/dirac_ilc_add_software.py
+-rw-rw-rw-   0 root         (0) root         (0)     9764 2024-04-16 15:47:11.000000 ilcdirac-35.0.3/src/ILCDIRAC/Core/scripts/dirac_ilc_add_user.py
+-rw-rw-rw-   0 root         (0) root         (0)    16381 2024-04-16 15:47:11.000000 ilcdirac-35.0.3/src/ILCDIRAC/Core/scripts/dirac_ilc_add_whizard.py
+-rw-rw-rw-   0 root         (0) root         (0)     3905 2024-04-16 15:47:11.000000 ilcdirac-35.0.3/src/ILCDIRAC/Core/scripts/dirac_ilc_list_users.py
+-rw-rw-rw-   0 root         (0) root         (0)     1573 2024-04-16 15:47:11.000000 ilcdirac-35.0.3/src/ILCDIRAC/Core/scripts/ilcdirac-install.sh
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-16 15:47:28.313817 ilcdirac-35.0.3/src/ILCDIRAC/DataManagementSystem/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-16 15:47:28.313817 ilcdirac-35.0.3/src/ILCDIRAC/DataManagementSystem/Agent/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-16 15:47:28.314817 ilcdirac-35.0.3/src/ILCDIRAC/DataManagementSystem/Agent/RequestOperations/
+-rw-rw-rw-   0 root         (0) root         (0)     4676 2024-04-16 15:47:11.000000 ilcdirac-35.0.3/src/ILCDIRAC/DataManagementSystem/Agent/RequestOperations/LogUpload.py
+-rw-rw-rw-   0 root         (0) root         (0)     1115 2024-04-16 15:47:11.000000 ilcdirac-35.0.3/src/ILCDIRAC/DataManagementSystem/Agent/RequestOperations/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1103 2024-04-16 15:47:11.000000 ilcdirac-35.0.3/src/ILCDIRAC/DataManagementSystem/Agent/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1108 2024-04-16 15:47:11.000000 ilcdirac-35.0.3/src/ILCDIRAC/DataManagementSystem/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-16 15:47:28.314817 ilcdirac-35.0.3/src/ILCDIRAC/FrameworkSystem/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-16 15:47:28.314817 ilcdirac-35.0.3/src/ILCDIRAC/FrameworkSystem/Agent/
+-rw-rw-rw-   0 root         (0) root         (0)     1013 2024-04-16 15:47:11.000000 ilcdirac-35.0.3/src/ILCDIRAC/FrameworkSystem/Agent/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)       11 2024-04-16 15:47:11.000000 ilcdirac-35.0.3/src/ILCDIRAC/FrameworkSystem/ConfigTemplate.cfg
+-rw-rw-rw-   0 root         (0) root         (0)     1013 2024-04-16 15:47:11.000000 ilcdirac-35.0.3/src/ILCDIRAC/FrameworkSystem/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-16 15:47:28.315817 ilcdirac-35.0.3/src/ILCDIRAC/ILCTransformationSystem/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-16 15:47:28.316817 ilcdirac-35.0.3/src/ILCDIRAC/ILCTransformationSystem/Agent/
+-rw-rw-rw-   0 root         (0) root         (0)    25777 2024-04-16 15:47:11.000000 ilcdirac-35.0.3/src/ILCDIRAC/ILCTransformationSystem/Agent/FileStatusTransformationAgent.py
+-rw-rw-rw-   0 root         (0) root         (0)     9996 2024-04-16 15:47:11.000000 ilcdirac-35.0.3/src/ILCDIRAC/ILCTransformationSystem/Agent/TarTheLogsAgent.py
+-rw-rw-rw-   0 root         (0) root         (0)     5395 2024-04-16 15:47:11.000000 ilcdirac-35.0.3/src/ILCDIRAC/ILCTransformationSystem/Agent/TransformationPlugin.py
+-rw-rw-rw-   0 root         (0) root         (0)     1072 2024-04-16 15:47:11.000000 ilcdirac-35.0.3/src/ILCDIRAC/ILCTransformationSystem/Agent/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-16 15:47:28.316817 ilcdirac-35.0.3/src/ILCDIRAC/ILCTransformationSystem/Client/
+-rw-rw-rw-   0 root         (0) root         (0)     1934 2024-04-16 15:47:11.000000 ilcdirac-35.0.3/src/ILCDIRAC/ILCTransformationSystem/Client/Transformation.py
+-rw-rw-rw-   0 root         (0) root         (0)     1079 2024-04-16 15:47:11.000000 ilcdirac-35.0.3/src/ILCDIRAC/ILCTransformationSystem/Client/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      441 2024-04-16 15:47:11.000000 ilcdirac-35.0.3/src/ILCDIRAC/ILCTransformationSystem/ConfigTemplate.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-16 15:47:28.318817 ilcdirac-35.0.3/src/ILCDIRAC/ILCTransformationSystem/Tests/
+-rw-rw-rw-   0 root         (0) root         (0)    35437 2024-04-16 15:47:11.000000 ilcdirac-35.0.3/src/ILCDIRAC/ILCTransformationSystem/Tests/Test_FileStatusTransformationAgent.py
+-rw-rw-rw-   0 root         (0) root         (0)    14308 2024-04-16 15:47:11.000000 ilcdirac-35.0.3/src/ILCDIRAC/ILCTransformationSystem/Tests/Test_ReleaseHelper.py
+-rw-rw-rw-   0 root         (0) root         (0)    19604 2024-04-16 15:47:11.000000 ilcdirac-35.0.3/src/ILCDIRAC/ILCTransformationSystem/Tests/Test_TransformationPlugin.py
+-rw-rw-rw-   0 root         (0) root         (0)    13782 2024-04-16 15:47:11.000000 ilcdirac-35.0.3/src/ILCDIRAC/ILCTransformationSystem/Tests/Test_createMovingTransformation.py
+-rw-rw-rw-   0 root         (0) root         (0)    30921 2024-04-16 15:47:11.000000 ilcdirac-35.0.3/src/ILCDIRAC/ILCTransformationSystem/Tests/Test_diracClicMakeProductions.py
+-rw-rw-rw-   0 root         (0) root         (0)    28121 2024-04-16 15:47:11.000000 ilcdirac-35.0.3/src/ILCDIRAC/ILCTransformationSystem/Tests/Test_diracFccMakeProductions.py
+-rw-rw-rw-   0 root         (0) root         (0)     7554 2024-04-16 15:47:11.000000 ilcdirac-35.0.3/src/ILCDIRAC/ILCTransformationSystem/Tests/test_diracIlcAddTasks.py
+-rw-rw-rw-   0 root         (0) root         (0)     2889 2024-04-16 15:47:11.000000 ilcdirac-35.0.3/src/ILCDIRAC/ILCTransformationSystem/Tests/test_utilities.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-16 15:47:28.319817 ilcdirac-35.0.3/src/ILCDIRAC/ILCTransformationSystem/Utilities/
+-rw-rw-rw-   0 root         (0) root         (0)     5456 2024-04-16 15:47:11.000000 ilcdirac-35.0.3/src/ILCDIRAC/ILCTransformationSystem/Utilities/DataParameters.py
+-rw-rw-rw-   0 root         (0) root         (0)     6462 2024-04-16 15:47:11.000000 ilcdirac-35.0.3/src/ILCDIRAC/ILCTransformationSystem/Utilities/ReleaseHelper.py
+-rw-rw-rw-   0 root         (0) root         (0)     3263 2024-04-16 15:47:11.000000 ilcdirac-35.0.3/src/ILCDIRAC/ILCTransformationSystem/Utilities/Utilities.py
+-rw-rw-rw-   0 root         (0) root         (0)     1074 2024-04-16 15:47:11.000000 ilcdirac-35.0.3/src/ILCDIRAC/ILCTransformationSystem/Utilities/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1071 2024-04-16 15:47:11.000000 ilcdirac-35.0.3/src/ILCDIRAC/ILCTransformationSystem/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-16 15:47:28.322817 ilcdirac-35.0.3/src/ILCDIRAC/ILCTransformationSystem/scripts/
+-rw-rw-rw-   0 root         (0) root         (0)     1075 2024-04-16 15:47:11.000000 ilcdirac-35.0.3/src/ILCDIRAC/ILCTransformationSystem/scripts/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    49305 2024-04-16 15:47:11.000000 ilcdirac-35.0.3/src/ILCDIRAC/ILCTransformationSystem/scripts/dirac_clic_make_productions.py
+-rw-rw-rw-   0 root         (0) root         (0)    49891 2024-04-16 15:47:11.000000 ilcdirac-35.0.3/src/ILCDIRAC/ILCTransformationSystem/scripts/dirac_fcc_make_productions.py
+-rw-rw-rw-   0 root         (0) root         (0)     6173 2024-04-16 15:47:11.000000 ilcdirac-35.0.3/src/ILCDIRAC/ILCTransformationSystem/scripts/dirac_ilc_add_tasks_to_prod.py
+-rw-rw-rw-   0 root         (0) root         (0)     3311 2024-04-16 15:47:11.000000 ilcdirac-35.0.3/src/ILCDIRAC/ILCTransformationSystem/scripts/dirac_ilc_filestatus_transformation.py
+-rw-rw-rw-   0 root         (0) root         (0)    13681 2024-04-16 15:47:11.000000 ilcdirac-35.0.3/src/ILCDIRAC/ILCTransformationSystem/scripts/dirac_ilc_get_info.py
+-rw-rw-rw-   0 root         (0) root         (0)     7259 2024-04-16 15:47:11.000000 ilcdirac-35.0.3/src/ILCDIRAC/ILCTransformationSystem/scripts/dirac_ilc_get_prod_log.py
+-rwxrwxrwx   0 root         (0) root         (0)     9899 2024-04-16 15:47:11.000000 ilcdirac-35.0.3/src/ILCDIRAC/ILCTransformationSystem/scripts/dirac_ilc_make_ddsimtarball.py
+-rw-rw-rw-   0 root         (0) root         (0)     4618 2024-04-16 15:47:11.000000 ilcdirac-35.0.3/src/ILCDIRAC/ILCTransformationSystem/scripts/dirac_ilc_moving_transformation.py
+-rw-rw-rw-   0 root         (0) root         (0)    18138 2024-04-16 15:47:11.000000 ilcdirac-35.0.3/src/ILCDIRAC/ILCTransformationSystem/scripts/dirac_ilc_production_summary.py
+-rw-rw-rw-   0 root         (0) root         (0)     3481 2024-04-16 15:47:11.000000 ilcdirac-35.0.3/src/ILCDIRAC/ILCTransformationSystem/scripts/dirac_ilc_replication_transformation.py
+-rw-rw-rw-   0 root         (0) root         (0)    12061 2024-04-16 15:47:11.000000 ilcdirac-35.0.3/src/ILCDIRAC/ILCTransformationSystem/scripts/dirac_ilc_upload_gen_files.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-16 15:47:28.323817 ilcdirac-35.0.3/src/ILCDIRAC/Interfaces/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-16 15:47:28.323817 ilcdirac-35.0.3/src/ILCDIRAC/Interfaces/API/
+-rw-rw-rw-   0 root         (0) root         (0)    13839 2024-04-16 15:47:11.000000 ilcdirac-35.0.3/src/ILCDIRAC/Interfaces/API/DiracILC.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-16 15:47:28.279817 ilcdirac-35.0.3/src/ILCDIRAC/Interfaces/API/Examples/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-16 15:47:28.324817 ilcdirac-35.0.3/src/ILCDIRAC/Interfaces/API/Examples/SIDChain/
+-rw-rw-rw-   0 root         (0) root         (0)       77 2024-04-16 15:47:11.000000 ilcdirac-35.0.3/src/ILCDIRAC/Interfaces/API/Examples/SIDChain/alias.properties
+-rw-rw-rw-   0 root         (0) root         (0)     1890 2024-04-16 15:47:11.000000 ilcdirac-35.0.3/src/ILCDIRAC/Interfaces/API/Examples/SIDChain/bannedSites.py
+-rw-rw-rw-   0 root         (0) root         (0)     9474 2024-04-16 15:47:11.000000 ilcdirac-35.0.3/src/ILCDIRAC/Interfaces/API/Examples/SIDChain/defaultPrePandoraLcsim.xml
+-rw-rw-rw-   0 root         (0) root         (0)    10942 2024-04-16 15:47:11.000000 ilcdirac-35.0.3/src/ILCDIRAC/Interfaces/API/Examples/SIDChain/defaultPrePandoraLcsimOverlay.xml
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-16 15:47:28.325817 ilcdirac-35.0.3/src/ILCDIRAC/Interfaces/API/Examples/SIDChain/fileLists/
+-rw-rw-rw-   0 root         (0) root         (0)     1202 2024-04-16 15:47:11.000000 ilcdirac-35.0.3/src/ILCDIRAC/Interfaces/API/Examples/SIDChain/fileLists/testSimList.py
+-rw-rw-rw-   0 root         (0) root         (0)     1196 2024-04-16 15:47:11.000000 ilcdirac-35.0.3/src/ILCDIRAC/Interfaces/API/Examples/SIDChain/fileLists/testStdhepList.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-16 15:47:28.336817 ilcdirac-35.0.3/src/ILCDIRAC/Interfaces/API/Examples/SIDChain/slicMacros/
+-rw-rw-rw-   0 root         (0) root         (0)       42 2024-04-16 15:47:11.000000 ilcdirac-35.0.3/src/ILCDIRAC/Interfaces/API/Examples/SIDChain/slicMacros/default.mac
+-rw-rw-rw-   0 root         (0) root         (0)       80 2024-04-16 15:47:11.000000 ilcdirac-35.0.3/src/ILCDIRAC/Interfaces/API/Examples/SIDChain/slicMacros/defaultClicCrossingAngle.mac
+-rw-rw-rw-   0 root         (0) root         (0)      324 2024-04-16 15:47:11.000000 ilcdirac-35.0.3/src/ILCDIRAC/Interfaces/API/Examples/SIDChain/slicMacros/e-_100gev_theta5-175.mac
+-rw-rw-rw-   0 root         (0) root         (0)      323 2024-04-16 15:47:11.000000 ilcdirac-35.0.3/src/ILCDIRAC/Interfaces/API/Examples/SIDChain/slicMacros/e-_10gev_theta5-175.mac
+-rw-rw-rw-   0 root         (0) root         (0)      327 2024-04-16 15:47:11.000000 ilcdirac-35.0.3/src/ILCDIRAC/Interfaces/API/Examples/SIDChain/slicMacros/gamma_100gev_theta5-175.mac
+-rw-rw-rw-   0 root         (0) root         (0)      326 2024-04-16 15:47:11.000000 ilcdirac-35.0.3/src/ILCDIRAC/Interfaces/API/Examples/SIDChain/slicMacros/gamma_10gev_theta5-175.mac
+-rw-rw-rw-   0 root         (0) root         (0)      325 2024-04-16 15:47:11.000000 ilcdirac-35.0.3/src/ILCDIRAC/Interfaces/API/Examples/SIDChain/slicMacros/mu-_100gev_theta10.mac
+-rw-rw-rw-   0 root         (0) root         (0)      325 2024-04-16 15:47:11.000000 ilcdirac-35.0.3/src/ILCDIRAC/Interfaces/API/Examples/SIDChain/slicMacros/mu-_100gev_theta20.mac
+-rw-rw-rw-   0 root         (0) root         (0)      325 2024-04-16 15:47:11.000000 ilcdirac-35.0.3/src/ILCDIRAC/Interfaces/API/Examples/SIDChain/slicMacros/mu-_100gev_theta30.mac
+-rw-rw-rw-   0 root         (0) root         (0)      325 2024-04-16 15:47:11.000000 ilcdirac-35.0.3/src/ILCDIRAC/Interfaces/API/Examples/SIDChain/slicMacros/mu-_100gev_theta40.mac
+-rw-rw-rw-   0 root         (0) root         (0)      325 2024-04-16 15:47:11.000000 ilcdirac-35.0.3/src/ILCDIRAC/Interfaces/API/Examples/SIDChain/slicMacros/mu-_100gev_theta5-175.mac
+-rw-rw-rw-   0 root         (0) root         (0)      325 2024-04-16 15:47:11.000000 ilcdirac-35.0.3/src/ILCDIRAC/Interfaces/API/Examples/SIDChain/slicMacros/mu-_100gev_theta50.mac
+-rw-rw-rw-   0 root         (0) root         (0)      325 2024-04-16 15:47:11.000000 ilcdirac-35.0.3/src/ILCDIRAC/Interfaces/API/Examples/SIDChain/slicMacros/mu-_100gev_theta60.mac
+-rw-rw-rw-   0 root         (0) root         (0)      325 2024-04-16 15:47:11.000000 ilcdirac-35.0.3/src/ILCDIRAC/Interfaces/API/Examples/SIDChain/slicMacros/mu-_100gev_theta70.mac
+-rw-rw-rw-   0 root         (0) root         (0)      325 2024-04-16 15:47:11.000000 ilcdirac-35.0.3/src/ILCDIRAC/Interfaces/API/Examples/SIDChain/slicMacros/mu-_100gev_theta80.mac
+-rw-rw-rw-   0 root         (0) root         (0)      325 2024-04-16 15:47:11.000000 ilcdirac-35.0.3/src/ILCDIRAC/Interfaces/API/Examples/SIDChain/slicMacros/mu-_100gev_theta90.mac
+-rw-rw-rw-   0 root         (0) root         (0)      324 2024-04-16 15:47:11.000000 ilcdirac-35.0.3/src/ILCDIRAC/Interfaces/API/Examples/SIDChain/slicMacros/mu-_10gev_theta10.mac
+-rw-rw-rw-   0 root         (0) root         (0)      324 2024-04-16 15:47:11.000000 ilcdirac-35.0.3/src/ILCDIRAC/Interfaces/API/Examples/SIDChain/slicMacros/mu-_10gev_theta20.mac
+-rw-rw-rw-   0 root         (0) root         (0)      324 2024-04-16 15:47:11.000000 ilcdirac-35.0.3/src/ILCDIRAC/Interfaces/API/Examples/SIDChain/slicMacros/mu-_10gev_theta30.mac
+-rw-rw-rw-   0 root         (0) root         (0)      324 2024-04-16 15:47:11.000000 ilcdirac-35.0.3/src/ILCDIRAC/Interfaces/API/Examples/SIDChain/slicMacros/mu-_10gev_theta40.mac
+-rw-rw-rw-   0 root         (0) root         (0)      324 2024-04-16 15:47:11.000000 ilcdirac-35.0.3/src/ILCDIRAC/Interfaces/API/Examples/SIDChain/slicMacros/mu-_10gev_theta5-175.mac
+-rw-rw-rw-   0 root         (0) root         (0)      324 2024-04-16 15:47:11.000000 ilcdirac-35.0.3/src/ILCDIRAC/Interfaces/API/Examples/SIDChain/slicMacros/mu-_10gev_theta50.mac
+-rw-rw-rw-   0 root         (0) root         (0)      324 2024-04-16 15:47:11.000000 ilcdirac-35.0.3/src/ILCDIRAC/Interfaces/API/Examples/SIDChain/slicMacros/mu-_10gev_theta60.mac
+-rw-rw-rw-   0 root         (0) root         (0)      324 2024-04-16 15:47:11.000000 ilcdirac-35.0.3/src/ILCDIRAC/Interfaces/API/Examples/SIDChain/slicMacros/mu-_10gev_theta70.mac
+-rw-rw-rw-   0 root         (0) root         (0)      324 2024-04-16 15:47:11.000000 ilcdirac-35.0.3/src/ILCDIRAC/Interfaces/API/Examples/SIDChain/slicMacros/mu-_10gev_theta80.mac
+-rw-rw-rw-   0 root         (0) root         (0)      324 2024-04-16 15:47:11.000000 ilcdirac-35.0.3/src/ILCDIRAC/Interfaces/API/Examples/SIDChain/slicMacros/mu-_10gev_theta90.mac
+-rw-rw-rw-   0 root         (0) root         (0)      325 2024-04-16 15:47:11.000000 ilcdirac-35.0.3/src/ILCDIRAC/Interfaces/API/Examples/SIDChain/slicMacros/mu-_200gev_theta10.mac
+-rw-rw-rw-   0 root         (0) root         (0)      325 2024-04-16 15:47:11.000000 ilcdirac-35.0.3/src/ILCDIRAC/Interfaces/API/Examples/SIDChain/slicMacros/mu-_200gev_theta20.mac
+-rw-rw-rw-   0 root         (0) root         (0)      325 2024-04-16 15:47:11.000000 ilcdirac-35.0.3/src/ILCDIRAC/Interfaces/API/Examples/SIDChain/slicMacros/mu-_200gev_theta30.mac
+-rw-rw-rw-   0 root         (0) root         (0)      325 2024-04-16 15:47:11.000000 ilcdirac-35.0.3/src/ILCDIRAC/Interfaces/API/Examples/SIDChain/slicMacros/mu-_200gev_theta40.mac
+-rw-rw-rw-   0 root         (0) root         (0)      325 2024-04-16 15:47:11.000000 ilcdirac-35.0.3/src/ILCDIRAC/Interfaces/API/Examples/SIDChain/slicMacros/mu-_200gev_theta50.mac
+-rw-rw-rw-   0 root         (0) root         (0)      325 2024-04-16 15:47:11.000000 ilcdirac-35.0.3/src/ILCDIRAC/Interfaces/API/Examples/SIDChain/slicMacros/mu-_200gev_theta60.mac
+-rw-rw-rw-   0 root         (0) root         (0)      325 2024-04-16 15:47:11.000000 ilcdirac-35.0.3/src/ILCDIRAC/Interfaces/API/Examples/SIDChain/slicMacros/mu-_200gev_theta70.mac
+-rw-rw-rw-   0 root         (0) root         (0)      325 2024-04-16 15:47:11.000000 ilcdirac-35.0.3/src/ILCDIRAC/Interfaces/API/Examples/SIDChain/slicMacros/mu-_200gev_theta80.mac
+-rw-rw-rw-   0 root         (0) root         (0)      325 2024-04-16 15:47:11.000000 ilcdirac-35.0.3/src/ILCDIRAC/Interfaces/API/Examples/SIDChain/slicMacros/mu-_200gev_theta90.mac
+-rw-rw-rw-   0 root         (0) root         (0)      324 2024-04-16 15:47:11.000000 ilcdirac-35.0.3/src/ILCDIRAC/Interfaces/API/Examples/SIDChain/slicMacros/mu-_50gev_theta10.mac
+-rw-rw-rw-   0 root         (0) root         (0)      324 2024-04-16 15:47:11.000000 ilcdirac-35.0.3/src/ILCDIRAC/Interfaces/API/Examples/SIDChain/slicMacros/mu-_50gev_theta20.mac
+-rw-rw-rw-   0 root         (0) root         (0)      324 2024-04-16 15:47:11.000000 ilcdirac-35.0.3/src/ILCDIRAC/Interfaces/API/Examples/SIDChain/slicMacros/mu-_50gev_theta30.mac
+-rw-rw-rw-   0 root         (0) root         (0)      324 2024-04-16 15:47:11.000000 ilcdirac-35.0.3/src/ILCDIRAC/Interfaces/API/Examples/SIDChain/slicMacros/mu-_50gev_theta40.mac
+-rw-rw-rw-   0 root         (0) root         (0)      324 2024-04-16 15:47:11.000000 ilcdirac-35.0.3/src/ILCDIRAC/Interfaces/API/Examples/SIDChain/slicMacros/mu-_50gev_theta50.mac
+-rw-rw-rw-   0 root         (0) root         (0)      324 2024-04-16 15:47:11.000000 ilcdirac-35.0.3/src/ILCDIRAC/Interfaces/API/Examples/SIDChain/slicMacros/mu-_50gev_theta60.mac
+-rw-rw-rw-   0 root         (0) root         (0)      324 2024-04-16 15:47:11.000000 ilcdirac-35.0.3/src/ILCDIRAC/Interfaces/API/Examples/SIDChain/slicMacros/mu-_50gev_theta70.mac
+-rw-rw-rw-   0 root         (0) root         (0)      324 2024-04-16 15:47:11.000000 ilcdirac-35.0.3/src/ILCDIRAC/Interfaces/API/Examples/SIDChain/slicMacros/mu-_50gev_theta80.mac
+-rw-rw-rw-   0 root         (0) root         (0)      324 2024-04-16 15:47:11.000000 ilcdirac-35.0.3/src/ILCDIRAC/Interfaces/API/Examples/SIDChain/slicMacros/mu-_50gev_theta90.mac
+-rw-rw-rw-   0 root         (0) root         (0)      325 2024-04-16 15:47:11.000000 ilcdirac-35.0.3/src/ILCDIRAC/Interfaces/API/Examples/SIDChain/slicMacros/pi-_100gev_theta5-175.mac
+-rw-rw-rw-   0 root         (0) root         (0)      324 2024-04-16 15:47:11.000000 ilcdirac-35.0.3/src/ILCDIRAC/Interfaces/API/Examples/SIDChain/slicMacros/pi-_10gev_theta5-175.mac
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-16 15:47:28.336817 ilcdirac-35.0.3/src/ILCDIRAC/Interfaces/API/Examples/SiDProduction/
+-rw-rw-rw-   0 root         (0) root         (0)     8766 2024-04-16 15:47:11.000000 ilcdirac-35.0.3/src/ILCDIRAC/Interfaces/API/Examples/SiDProduction/sid_dbd_sim_production_default.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-16 15:47:28.339817 ilcdirac-35.0.3/src/ILCDIRAC/Interfaces/API/NewInterface/
+-rw-rw-rw-   0 root         (0) root         (0)    27099 2024-04-16 15:47:11.000000 ilcdirac-35.0.3/src/ILCDIRAC/Interfaces/API/NewInterface/Application.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-16 15:47:28.347817 ilcdirac-35.0.3/src/ILCDIRAC/Interfaces/API/NewInterface/Applications/
+-rw-rw-rw-   0 root         (0) root         (0)     6108 2024-04-16 15:47:11.000000 ilcdirac-35.0.3/src/ILCDIRAC/Interfaces/API/NewInterface/Applications/Babayaga.py
+-rw-rw-rw-   0 root         (0) root         (0)     6024 2024-04-16 15:47:11.000000 ilcdirac-35.0.3/src/ILCDIRAC/Interfaces/API/NewInterface/Applications/Bhlumi.py
+-rw-rw-rw-   0 root         (0) root         (0)     3135 2024-04-16 15:47:11.000000 ilcdirac-35.0.3/src/ILCDIRAC/Interfaces/API/NewInterface/Applications/Calibration.py
+-rw-rw-rw-   0 root         (0) root         (0)     3757 2024-04-16 15:47:11.000000 ilcdirac-35.0.3/src/ILCDIRAC/Interfaces/API/NewInterface/Applications/CheckCollections.py
+-rw-rw-rw-   0 root         (0) root         (0)     2335 2024-04-16 15:47:11.000000 ilcdirac-35.0.3/src/ILCDIRAC/Interfaces/API/NewInterface/Applications/CheckWNs.py
+-rw-rw-rw-   0 root         (0) root         (0)    10491 2024-04-16 15:47:11.000000 ilcdirac-35.0.3/src/ILCDIRAC/Interfaces/API/NewInterface/Applications/DDSim.py
+-rw-rw-rw-   0 root         (0) root         (0)    14016 2024-04-16 15:47:11.000000 ilcdirac-35.0.3/src/ILCDIRAC/Interfaces/API/NewInterface/Applications/DelphesApp.py
+-rw-rw-rw-   0 root         (0) root         (0)    35946 2024-04-16 15:47:11.000000 ilcdirac-35.0.3/src/ILCDIRAC/Interfaces/API/NewInterface/Applications/Fcc.py
+-rw-rw-rw-   0 root         (0) root         (0)    13940 2024-04-16 15:47:11.000000 ilcdirac-35.0.3/src/ILCDIRAC/Interfaces/API/NewInterface/Applications/GaudiApp.py
+-rw-rw-rw-   0 root         (0) root         (0)     6521 2024-04-16 15:47:11.000000 ilcdirac-35.0.3/src/ILCDIRAC/Interfaces/API/NewInterface/Applications/GenericApplication.py
+-rw-rw-rw-   0 root         (0) root         (0)     3885 2024-04-16 15:47:11.000000 ilcdirac-35.0.3/src/ILCDIRAC/Interfaces/API/NewInterface/Applications/GetSRMFile.py
+-rw-rw-rw-   0 root         (0) root         (0)     6008 2024-04-16 15:47:11.000000 ilcdirac-35.0.3/src/ILCDIRAC/Interfaces/API/NewInterface/Applications/KKMC.py
+-rw-rw-rw-   0 root         (0) root         (0)     9573 2024-04-16 15:47:11.000000 ilcdirac-35.0.3/src/ILCDIRAC/Interfaces/API/NewInterface/Applications/LCSIM.py
+-rw-rw-rw-   0 root         (0) root         (0)    10161 2024-04-16 15:47:11.000000 ilcdirac-35.0.3/src/ILCDIRAC/Interfaces/API/NewInterface/Applications/Marlin.py
+-rw-rw-rw-   0 root         (0) root         (0)     8281 2024-04-16 15:47:11.000000 ilcdirac-35.0.3/src/ILCDIRAC/Interfaces/API/NewInterface/Applications/Mokka.py
+-rw-rw-rw-   0 root         (0) root         (0)    16303 2024-04-16 15:47:11.000000 ilcdirac-35.0.3/src/ILCDIRAC/Interfaces/API/NewInterface/Applications/OverlayInput.py
+-rw-rw-rw-   0 root         (0) root         (0)     3918 2024-04-16 15:47:11.000000 ilcdirac-35.0.3/src/ILCDIRAC/Interfaces/API/NewInterface/Applications/PostGenSelection.py
+-rw-rw-rw-   0 root         (0) root         (0)     3312 2024-04-16 15:47:11.000000 ilcdirac-35.0.3/src/ILCDIRAC/Interfaces/API/NewInterface/Applications/Pythia.py
+-rw-rw-rw-   0 root         (0) root         (0)     2090 2024-04-16 15:47:11.000000 ilcdirac-35.0.3/src/ILCDIRAC/Interfaces/API/NewInterface/Applications/RootMacro.py
+-rw-rw-rw-   0 root         (0) root         (0)     2461 2024-04-16 15:47:11.000000 ilcdirac-35.0.3/src/ILCDIRAC/Interfaces/API/NewInterface/Applications/RootScript.py
+-rw-rw-rw-   0 root         (0) root         (0)     3752 2024-04-16 15:47:11.000000 ilcdirac-35.0.3/src/ILCDIRAC/Interfaces/API/NewInterface/Applications/SLCIOConcatenate.py
+-rw-rw-rw-   0 root         (0) root         (0)     4434 2024-04-16 15:47:11.000000 ilcdirac-35.0.3/src/ILCDIRAC/Interfaces/API/NewInterface/Applications/SLCIOSplit.py
+-rw-rw-rw-   0 root         (0) root         (0)     6174 2024-04-16 15:47:11.000000 ilcdirac-35.0.3/src/ILCDIRAC/Interfaces/API/NewInterface/Applications/SLIC.py
+-rw-rw-rw-   0 root         (0) root         (0)     6089 2024-04-16 15:47:11.000000 ilcdirac-35.0.3/src/ILCDIRAC/Interfaces/API/NewInterface/Applications/SLICPandora.py
+-rw-rw-rw-   0 root         (0) root         (0)     5479 2024-04-16 15:47:11.000000 ilcdirac-35.0.3/src/ILCDIRAC/Interfaces/API/NewInterface/Applications/StdHepSplit.py
+-rw-rw-rw-   0 root         (0) root         (0)     6957 2024-04-16 15:47:11.000000 ilcdirac-35.0.3/src/ILCDIRAC/Interfaces/API/NewInterface/Applications/StdhepCut.py
+-rw-rw-rw-   0 root         (0) root         (0)     1782 2024-04-16 15:47:11.000000 ilcdirac-35.0.3/src/ILCDIRAC/Interfaces/API/NewInterface/Applications/StdhepCutJava.py
+-rw-rw-rw-   0 root         (0) root         (0)     3921 2024-04-16 15:47:11.000000 ilcdirac-35.0.3/src/ILCDIRAC/Interfaces/API/NewInterface/Applications/Tomato.py
+-rw-rw-rw-   0 root         (0) root         (0)    17277 2024-04-16 15:47:11.000000 ilcdirac-35.0.3/src/ILCDIRAC/Interfaces/API/NewInterface/Applications/Whizard.py
+-rw-rw-rw-   0 root         (0) root         (0)    12788 2024-04-16 15:47:11.000000 ilcdirac-35.0.3/src/ILCDIRAC/Interfaces/API/NewInterface/Applications/Whizard2.py
+-rw-rw-rw-   0 root         (0) root         (0)     4441 2024-04-16 15:47:11.000000 ilcdirac-35.0.3/src/ILCDIRAC/Interfaces/API/NewInterface/Applications/_Root.py
+-rw-rw-rw-   0 root         (0) root         (0)     5185 2024-04-16 15:47:11.000000 ilcdirac-35.0.3/src/ILCDIRAC/Interfaces/API/NewInterface/Applications/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-16 15:47:28.349817 ilcdirac-35.0.3/src/ILCDIRAC/Interfaces/API/NewInterface/Examples/
+-rw-rw-rw-   0 root         (0) root         (0)     2838 2024-04-16 15:47:11.000000 ilcdirac-35.0.3/src/ILCDIRAC/Interfaces/API/NewInterface/Examples/ConditionalOverlay.py
+-rw-rw-rw-   0 root         (0) root         (0)     2672 2024-04-16 15:47:11.000000 ilcdirac-35.0.3/src/ILCDIRAC/Interfaces/API/NewInterface/Examples/FullILDChain.py
+-rw-rw-rw-   0 root         (0) root         (0)    19620 2024-04-16 15:47:11.000000 ilcdirac-35.0.3/src/ILCDIRAC/Interfaces/API/NewInterface/Examples/ILDProductionChainDBD.py
+-rw-rw-rw-   0 root         (0) root         (0)    22235 2024-04-16 15:47:11.000000 ilcdirac-35.0.3/src/ILCDIRAC/Interfaces/API/NewInterface/Examples/ILDProductionChainOpt2017.py
+-rw-rw-rw-   0 root         (0) root         (0)     2078 2024-04-16 15:47:11.000000 ilcdirac-35.0.3/src/ILCDIRAC/Interfaces/API/NewInterface/Examples/MarlinExample.py
+-rw-rw-rw-   0 root         (0) root         (0)     2841 2024-04-16 15:47:11.000000 ilcdirac-35.0.3/src/ILCDIRAC/Interfaces/API/NewInterface/Examples/MokkaMarlinOverlayMarlin.py
+-rw-rw-rw-   0 root         (0) root         (0)     2993 2024-04-16 15:47:11.000000 ilcdirac-35.0.3/src/ILCDIRAC/Interfaces/API/NewInterface/Examples/ParametricJobExample.py
+-rw-rw-rw-   0 root         (0) root         (0)     4254 2024-04-16 15:47:11.000000 ilcdirac-35.0.3/src/ILCDIRAC/Interfaces/API/NewInterface/Examples/ReplicationAkiya.py
+-rw-rw-rw-   0 root         (0) root         (0)     9864 2024-04-16 15:47:11.000000 ilcdirac-35.0.3/src/ILCDIRAC/Interfaces/API/NewInterface/Examples/SIDProductionChain.py
+-rw-rw-rw-   0 root         (0) root         (0)    24484 2024-04-16 15:47:11.000000 ilcdirac-35.0.3/src/ILCDIRAC/Interfaces/API/NewInterface/ILDProductionJobDBD.py
+-rw-rw-rw-   0 root         (0) root         (0)    26292 2024-04-16 15:47:11.000000 ilcdirac-35.0.3/src/ILCDIRAC/Interfaces/API/NewInterface/ILDProductionJobOpt2017.py
+-rw-rw-rw-   0 root         (0) root         (0)    15111 2024-04-16 15:47:11.000000 ilcdirac-35.0.3/src/ILCDIRAC/Interfaces/API/NewInterface/Job.py
+-rw-rw-rw-   0 root         (0) root         (0)     3097 2024-04-16 15:47:11.000000 ilcdirac-35.0.3/src/ILCDIRAC/Interfaces/API/NewInterface/LCApplication.py
+-rw-rw-rw-   0 root         (0) root         (0)     2402 2024-04-16 15:47:11.000000 ilcdirac-35.0.3/src/ILCDIRAC/Interfaces/API/NewInterface/LCUtilityApplication.py
+-rw-rw-rw-   0 root         (0) root         (0)    42197 2024-04-16 15:47:11.000000 ilcdirac-35.0.3/src/ILCDIRAC/Interfaces/API/NewInterface/ProductionJob.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-16 15:47:28.350817 ilcdirac-35.0.3/src/ILCDIRAC/Interfaces/API/NewInterface/Productions/
+-rw-rw-rw-   0 root         (0) root         (0)    28003 2024-04-16 15:47:11.000000 ilcdirac-35.0.3/src/ILCDIRAC/Interfaces/API/NewInterface/Productions/CLICProductionChain.py
+-rw-rw-rw-   0 root         (0) root         (0)    29734 2024-04-16 15:47:11.000000 ilcdirac-35.0.3/src/ILCDIRAC/Interfaces/API/NewInterface/Productions/CLICProductionChain_hzqq_420.py
+-rwxrwxrwx   0 root         (0) root         (0)    35686 2024-04-16 15:47:11.000000 ilcdirac-35.0.3/src/ILCDIRAC/Interfaces/API/NewInterface/Productions/ProductionChainTest.py
+-rw-rw-rw-   0 root         (0) root         (0)    13131 2024-04-16 15:47:11.000000 ilcdirac-35.0.3/src/ILCDIRAC/Interfaces/API/NewInterface/Productions/SIDProductionChain.py
+-rw-rw-rw-   0 root         (0) root         (0)    12330 2024-04-16 15:47:11.000000 ilcdirac-35.0.3/src/ILCDIRAC/Interfaces/API/NewInterface/SIDProductionJob.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-16 15:47:28.358816 ilcdirac-35.0.3/src/ILCDIRAC/Interfaces/API/NewInterface/Tests/
+-rw-rw-rw-   0 root         (0) root         (0)     7876 2024-04-16 15:47:11.000000 ilcdirac-35.0.3/src/ILCDIRAC/Interfaces/API/NewInterface/Tests/Test_Application.py
+-rw-rw-rw-   0 root         (0) root         (0)     9657 2024-04-16 15:47:11.000000 ilcdirac-35.0.3/src/ILCDIRAC/Interfaces/API/NewInterface/Tests/Test_Babayaga.py
+-rw-rw-rw-   0 root         (0) root         (0)     9427 2024-04-16 15:47:11.000000 ilcdirac-35.0.3/src/ILCDIRAC/Interfaces/API/NewInterface/Tests/Test_Bhlumi.py
+-rw-rw-rw-   0 root         (0) root         (0)     2416 2024-04-16 15:47:11.000000 ilcdirac-35.0.3/src/ILCDIRAC/Interfaces/API/NewInterface/Tests/Test_Calibration.py
+-rw-rw-rw-   0 root         (0) root         (0)     4672 2024-04-16 15:47:11.000000 ilcdirac-35.0.3/src/ILCDIRAC/Interfaces/API/NewInterface/Tests/Test_CheckCollections.py
+-rw-rw-rw-   0 root         (0) root         (0)     2878 2024-04-16 15:47:11.000000 ilcdirac-35.0.3/src/ILCDIRAC/Interfaces/API/NewInterface/Tests/Test_CheckWNs.py
+-rw-rw-rw-   0 root         (0) root         (0)    18299 2024-04-16 15:47:11.000000 ilcdirac-35.0.3/src/ILCDIRAC/Interfaces/API/NewInterface/Tests/Test_DDSim.py
+-rw-rw-rw-   0 root         (0) root         (0)    20338 2024-04-16 15:47:11.000000 ilcdirac-35.0.3/src/ILCDIRAC/Interfaces/API/NewInterface/Tests/Test_DelphesApp.py
+-rw-rw-rw-   0 root         (0) root         (0)    41414 2024-04-16 15:47:11.000000 ilcdirac-35.0.3/src/ILCDIRAC/Interfaces/API/NewInterface/Tests/Test_Fcc.py
+-rw-rw-rw-   0 root         (0) root         (0)    16975 2024-04-16 15:47:11.000000 ilcdirac-35.0.3/src/ILCDIRAC/Interfaces/API/NewInterface/Tests/Test_GaudiApp.py
+-rw-rw-rw-   0 root         (0) root         (0)     5930 2024-04-16 15:47:11.000000 ilcdirac-35.0.3/src/ILCDIRAC/Interfaces/API/NewInterface/Tests/Test_GenericApplication.py
+-rw-rw-rw-   0 root         (0) root         (0)     4218 2024-04-16 15:47:11.000000 ilcdirac-35.0.3/src/ILCDIRAC/Interfaces/API/NewInterface/Tests/Test_GetSRMFile.py
+-rw-rw-rw-   0 root         (0) root         (0)    13745 2024-04-16 15:47:11.000000 ilcdirac-35.0.3/src/ILCDIRAC/Interfaces/API/NewInterface/Tests/Test_Job.py
+-rw-rw-rw-   0 root         (0) root         (0)     8888 2024-04-16 15:47:11.000000 ilcdirac-35.0.3/src/ILCDIRAC/Interfaces/API/NewInterface/Tests/Test_KKMC.py
+-rw-rw-rw-   0 root         (0) root         (0)    12305 2024-04-16 15:47:11.000000 ilcdirac-35.0.3/src/ILCDIRAC/Interfaces/API/NewInterface/Tests/Test_LCSIM.py
+-rw-rw-rw-   0 root         (0) root         (0)     8309 2024-04-16 15:47:11.000000 ilcdirac-35.0.3/src/ILCDIRAC/Interfaces/API/NewInterface/Tests/Test_Marlin.py
+-rw-rw-rw-   0 root         (0) root         (0)     6492 2024-04-16 15:47:11.000000 ilcdirac-35.0.3/src/ILCDIRAC/Interfaces/API/NewInterface/Tests/Test_Mokka.py
+-rw-rw-rw-   0 root         (0) root         (0)    14537 2024-04-16 15:47:11.000000 ilcdirac-35.0.3/src/ILCDIRAC/Interfaces/API/NewInterface/Tests/Test_OverlayInput.py
+-rw-rw-rw-   0 root         (0) root         (0)     4767 2024-04-16 15:47:11.000000 ilcdirac-35.0.3/src/ILCDIRAC/Interfaces/API/NewInterface/Tests/Test_PostGenSelection.py
+-rw-rw-rw-   0 root         (0) root         (0)    75909 2024-04-16 15:47:11.000000 ilcdirac-35.0.3/src/ILCDIRAC/Interfaces/API/NewInterface/Tests/Test_ProductionJob.py
+-rw-rw-rw-   0 root         (0) root         (0)     4830 2024-04-16 15:47:11.000000 ilcdirac-35.0.3/src/ILCDIRAC/Interfaces/API/NewInterface/Tests/Test_Pythia.py
+-rw-rw-rw-   0 root         (0) root         (0)     4533 2024-04-16 15:47:11.000000 ilcdirac-35.0.3/src/ILCDIRAC/Interfaces/API/NewInterface/Tests/Test_SLCIOConcatenate.py
+-rw-rw-rw-   0 root         (0) root         (0)     4798 2024-04-16 15:47:11.000000 ilcdirac-35.0.3/src/ILCDIRAC/Interfaces/API/NewInterface/Tests/Test_SLCIOSplit.py
+-rw-rw-rw-   0 root         (0) root         (0)     6232 2024-04-16 15:47:11.000000 ilcdirac-35.0.3/src/ILCDIRAC/Interfaces/API/NewInterface/Tests/Test_SLIC.py
+-rw-rw-rw-   0 root         (0) root         (0)     7551 2024-04-16 15:47:11.000000 ilcdirac-35.0.3/src/ILCDIRAC/Interfaces/API/NewInterface/Tests/Test_SLICPandora.py
+-rw-rw-rw-   0 root         (0) root         (0)     5077 2024-04-16 15:47:11.000000 ilcdirac-35.0.3/src/ILCDIRAC/Interfaces/API/NewInterface/Tests/Test_StdHepSplit.py
+-rw-rw-rw-   0 root         (0) root         (0)     6829 2024-04-16 15:47:11.000000 ilcdirac-35.0.3/src/ILCDIRAC/Interfaces/API/NewInterface/Tests/Test_StdhepCut.py
+-rw-rw-rw-   0 root         (0) root         (0)     4763 2024-04-16 15:47:11.000000 ilcdirac-35.0.3/src/ILCDIRAC/Interfaces/API/NewInterface/Tests/Test_Tomato.py
+-rw-rw-rw-   0 root         (0) root         (0)    22726 2024-04-16 15:47:11.000000 ilcdirac-35.0.3/src/ILCDIRAC/Interfaces/API/NewInterface/Tests/Test_UserJob.py
+-rw-rw-rw-   0 root         (0) root         (0)    20865 2024-04-16 15:47:11.000000 ilcdirac-35.0.3/src/ILCDIRAC/Interfaces/API/NewInterface/Tests/Test_Whizard.py
+-rw-rw-rw-   0 root         (0) root         (0)    13044 2024-04-16 15:47:11.000000 ilcdirac-35.0.3/src/ILCDIRAC/Interfaces/API/NewInterface/Tests/Test_Whizard2.py
+-rw-rw-rw-   0 root         (0) root         (0)     4169 2024-04-16 15:47:11.000000 ilcdirac-35.0.3/src/ILCDIRAC/Interfaces/API/NewInterface/Tests/Test__Root.py
+-rw-rw-rw-   0 root         (0) root         (0)     1128 2024-04-16 15:47:11.000000 ilcdirac-35.0.3/src/ILCDIRAC/Interfaces/API/NewInterface/Tests/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     9860 2024-04-16 15:47:11.000000 ilcdirac-35.0.3/src/ILCDIRAC/Interfaces/API/NewInterface/UserJob.py
+-rw-rw-rw-   0 root         (0) root         (0)     1129 2024-04-16 15:47:11.000000 ilcdirac-35.0.3/src/ILCDIRAC/Interfaces/API/NewInterface/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-16 15:47:28.358816 ilcdirac-35.0.3/src/ILCDIRAC/Interfaces/API/Test/
+-rw-rw-rw-   0 root         (0) root         (0)    20995 2024-04-16 15:47:11.000000 ilcdirac-35.0.3/src/ILCDIRAC/Interfaces/API/Test/Test_DiracILC.py
+-rw-rw-rw-   0 root         (0) root         (0)     1132 2024-04-16 15:47:11.000000 ilcdirac-35.0.3/src/ILCDIRAC/Interfaces/API/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-16 15:47:28.359816 ilcdirac-35.0.3/src/ILCDIRAC/Interfaces/Tests/
+-rw-rw-rw-   0 root         (0) root         (0)     2622 2024-04-16 15:47:11.000000 ilcdirac-35.0.3/src/ILCDIRAC/Interfaces/Tests/Test_JobHelpers.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-16 15:47:28.360817 ilcdirac-35.0.3/src/ILCDIRAC/Interfaces/Utilities/
+-rw-rw-rw-   0 root         (0) root         (0)     4727 2024-04-16 15:47:11.000000 ilcdirac-35.0.3/src/ILCDIRAC/Interfaces/Utilities/DDInterfaceMixin.py
+-rw-rw-rw-   0 root         (0) root         (0)     1680 2024-04-16 15:47:11.000000 ilcdirac-35.0.3/src/ILCDIRAC/Interfaces/Utilities/JobHelpers.py
+-rw-rw-rw-   0 root         (0) root         (0)    15312 2024-04-16 15:47:11.000000 ilcdirac-35.0.3/src/ILCDIRAC/Interfaces/Utilities/SplitMixin.py
+-rw-rw-rw-   0 root         (0) root         (0)     1013 2024-04-16 15:47:11.000000 ilcdirac-35.0.3/src/ILCDIRAC/Interfaces/Utilities/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1116 2024-04-16 15:47:11.000000 ilcdirac-35.0.3/src/ILCDIRAC/Interfaces/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-16 15:47:28.362816 ilcdirac-35.0.3/src/ILCDIRAC/Interfaces/scripts/
+-rwxrwxrwx   0 root         (0) root         (0)     2975 2024-04-16 15:47:11.000000 ilcdirac-35.0.3/src/ILCDIRAC/Interfaces/scripts/TestAndProbeSites.py
+-rw-rw-rw-   0 root         (0) root         (0)     1073 2024-04-16 15:47:11.000000 ilcdirac-35.0.3/src/ILCDIRAC/Interfaces/scripts/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     7669 2024-04-16 15:47:11.000000 ilcdirac-35.0.3/src/ILCDIRAC/Interfaces/scripts/dirac_ilc_find_in_FC.py
+-rw-rw-rw-   0 root         (0) root         (0)     3483 2024-04-16 15:47:11.000000 ilcdirac-35.0.3/src/ILCDIRAC/Interfaces/scripts/dirac_ilc_show_software.py
+-rw-rw-rw-   0 root         (0) root         (0)     2581 2024-04-16 15:47:11.000000 ilcdirac-35.0.3/src/ILCDIRAC/Interfaces/scripts/dirac_repo_create_lfn_list.py
+-rw-rw-rw-   0 root         (0) root         (0)     3033 2024-04-16 15:47:11.000000 ilcdirac-35.0.3/src/ILCDIRAC/Interfaces/scripts/dirac_repo_retrieve_jobs_output.py
+-rw-rw-rw-   0 root         (0) root         (0)     2341 2024-04-16 15:47:11.000000 ilcdirac-35.0.3/src/ILCDIRAC/Interfaces/scripts/dirac_repo_retrieve_jobs_output_data.py
+-rwxrwxrwx   0 root         (0) root         (0)     3634 2024-04-16 15:47:11.000000 ilcdirac-35.0.3/src/ILCDIRAC/Interfaces/scripts/ilcdirac_version.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-16 15:47:28.362816 ilcdirac-35.0.3/src/ILCDIRAC/OverlaySystem/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-16 15:47:28.362816 ilcdirac-35.0.3/src/ILCDIRAC/OverlaySystem/Agent/
+-rw-rw-rw-   0 root         (0) root         (0)     2638 2024-04-16 15:47:11.000000 ilcdirac-35.0.3/src/ILCDIRAC/OverlaySystem/Agent/ResetCounters.py
+-rw-rw-rw-   0 root         (0) root         (0)     1088 2024-04-16 15:47:11.000000 ilcdirac-35.0.3/src/ILCDIRAC/OverlaySystem/Agent/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-16 15:47:28.363817 ilcdirac-35.0.3/src/ILCDIRAC/OverlaySystem/Client/
+-rw-rw-rw-   0 root         (0) root         (0)     1399 2024-04-16 15:47:11.000000 ilcdirac-35.0.3/src/ILCDIRAC/OverlaySystem/Client/OverlaySystemClient.py
+-rw-rw-rw-   0 root         (0) root         (0)     1088 2024-04-16 15:47:11.000000 ilcdirac-35.0.3/src/ILCDIRAC/OverlaySystem/Client/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      221 2024-04-16 15:47:11.000000 ilcdirac-35.0.3/src/ILCDIRAC/OverlaySystem/ConfigTemplate.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-16 15:47:28.363817 ilcdirac-35.0.3/src/ILCDIRAC/OverlaySystem/DB/
+-rw-rw-rw-   0 root         (0) root         (0)     6953 2024-04-16 15:47:11.000000 ilcdirac-35.0.3/src/ILCDIRAC/OverlaySystem/DB/OverlayDB.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-16 15:47:28.364817 ilcdirac-35.0.3/src/ILCDIRAC/OverlaySystem/DB/Test/
+-rw-rw-rw-   0 root         (0) root         (0)     9389 2024-04-16 15:47:11.000000 ilcdirac-35.0.3/src/ILCDIRAC/OverlaySystem/DB/Test/Test_OverlayDB.py
+-rw-rw-rw-   0 root         (0) root         (0)     1062 2024-04-16 15:47:11.000000 ilcdirac-35.0.3/src/ILCDIRAC/OverlaySystem/DB/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-16 15:47:28.364817 ilcdirac-35.0.3/src/ILCDIRAC/OverlaySystem/Service/
+-rw-rw-rw-   0 root         (0) root         (0)     2462 2024-04-16 15:47:11.000000 ilcdirac-35.0.3/src/ILCDIRAC/OverlaySystem/Service/OverlayHandler.py
+-rw-rw-rw-   0 root         (0) root         (0)     1072 2024-04-16 15:47:11.000000 ilcdirac-35.0.3/src/ILCDIRAC/OverlaySystem/Service/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1118 2024-04-16 15:47:11.000000 ilcdirac-35.0.3/src/ILCDIRAC/OverlaySystem/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-16 15:47:28.364817 ilcdirac-35.0.3/src/ILCDIRAC/Workflow/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-16 15:47:28.376816 ilcdirac-35.0.3/src/ILCDIRAC/Workflow/Modules/
+-rw-rw-rw-   0 root         (0) root         (0)     4515 2024-04-16 15:47:11.000000 ilcdirac-35.0.3/src/ILCDIRAC/Workflow/Modules/AnalyseWN.py
+-rw-rw-rw-   0 root         (0) root         (0)     5524 2024-04-16 15:47:11.000000 ilcdirac-35.0.3/src/ILCDIRAC/Workflow/Modules/ApplicationScript.py
+-rw-rw-rw-   0 root         (0) root         (0)     7489 2024-04-16 15:47:11.000000 ilcdirac-35.0.3/src/ILCDIRAC/Workflow/Modules/BabayagaAnalysis.py
+-rw-rw-rw-   0 root         (0) root         (0)     8870 2024-04-16 15:47:11.000000 ilcdirac-35.0.3/src/ILCDIRAC/Workflow/Modules/BhlumiAnalysis.py
+-rw-rw-rw-   0 root         (0) root         (0)    23026 2024-04-16 15:47:11.000000 ilcdirac-35.0.3/src/ILCDIRAC/Workflow/Modules/Calibration.py
+-rw-rw-rw-   0 root         (0) root         (0)     5789 2024-04-16 15:47:11.000000 ilcdirac-35.0.3/src/ILCDIRAC/Workflow/Modules/CheckCollections.py
+-rw-rw-rw-   0 root         (0) root         (0)     2452 2024-04-16 15:47:11.000000 ilcdirac-35.0.3/src/ILCDIRAC/Workflow/Modules/ComputeOutputDataList.py
+-rw-rw-rw-   0 root         (0) root         (0)     3146 2024-04-16 15:47:11.000000 ilcdirac-35.0.3/src/ILCDIRAC/Workflow/Modules/DBDGenRegisterOutputData.py
+-rw-rw-rw-   0 root         (0) root         (0)    16673 2024-04-16 15:47:11.000000 ilcdirac-35.0.3/src/ILCDIRAC/Workflow/Modules/DDSimAnalysis.py
+-rw-rw-rw-   0 root         (0) root         (0)     9184 2024-04-16 15:47:11.000000 ilcdirac-35.0.3/src/ILCDIRAC/Workflow/Modules/DelphesAppModule.py
+-rw-rw-rw-   0 root         (0) root         (0)     1894 2024-04-16 15:47:11.000000 ilcdirac-35.0.3/src/ILCDIRAC/Workflow/Modules/DummyModule.py
+-rw-rw-rw-   0 root         (0) root         (0)     6809 2024-04-16 15:47:11.000000 ilcdirac-35.0.3/src/ILCDIRAC/Workflow/Modules/FailoverRequest.py
+-rw-rw-rw-   0 root         (0) root         (0)    19926 2024-04-16 15:47:11.000000 ilcdirac-35.0.3/src/ILCDIRAC/Workflow/Modules/FccAnalysis.py
+-rw-rw-rw-   0 root         (0) root         (0)     8792 2024-04-16 15:47:11.000000 ilcdirac-35.0.3/src/ILCDIRAC/Workflow/Modules/GaudiAppModule.py
+-rw-rw-rw-   0 root         (0) root         (0)     4454 2024-04-16 15:47:11.000000 ilcdirac-35.0.3/src/ILCDIRAC/Workflow/Modules/GetSRMFile.py
+-rw-rw-rw-   0 root         (0) root         (0)     6156 2024-04-16 15:47:11.000000 ilcdirac-35.0.3/src/ILCDIRAC/Workflow/Modules/ILDRegisterOutputData.py
+-rw-rw-rw-   0 root         (0) root         (0)     7234 2024-04-16 15:47:11.000000 ilcdirac-35.0.3/src/ILCDIRAC/Workflow/Modules/KKMCAnalysis.py
+-rw-rw-rw-   0 root         (0) root         (0)     5057 2024-04-16 15:47:11.000000 ilcdirac-35.0.3/src/ILCDIRAC/Workflow/Modules/LCIOConcatenate.py
+-rw-rw-rw-   0 root         (0) root         (0)     8078 2024-04-16 15:47:11.000000 ilcdirac-35.0.3/src/ILCDIRAC/Workflow/Modules/LCIOSplit.py
+-rw-rw-rw-   0 root         (0) root         (0)    13096 2024-04-16 15:47:11.000000 ilcdirac-35.0.3/src/ILCDIRAC/Workflow/Modules/LCSIMAnalysis.py
+-rw-rw-rw-   0 root         (0) root         (0)    18950 2024-04-16 15:47:11.000000 ilcdirac-35.0.3/src/ILCDIRAC/Workflow/Modules/MarlinAnalysis.py
+-rw-rw-rw-   0 root         (0) root         (0)    31351 2024-04-16 15:47:11.000000 ilcdirac-35.0.3/src/ILCDIRAC/Workflow/Modules/ModuleBase.py
+-rw-rw-rw-   0 root         (0) root         (0)    26082 2024-04-16 15:47:11.000000 ilcdirac-35.0.3/src/ILCDIRAC/Workflow/Modules/MokkaAnalysis.py
+-rw-rw-rw-   0 root         (0) root         (0)     5266 2024-04-16 15:47:11.000000 ilcdirac-35.0.3/src/ILCDIRAC/Workflow/Modules/MoveInFC.py
+-rw-rw-rw-   0 root         (0) root         (0)    33871 2024-04-16 15:47:11.000000 ilcdirac-35.0.3/src/ILCDIRAC/Workflow/Modules/OverlayInput.py
+-rw-rw-rw-   0 root         (0) root         (0)     7960 2024-04-16 15:47:11.000000 ilcdirac-35.0.3/src/ILCDIRAC/Workflow/Modules/PostGenSelection.py
+-rw-rw-rw-   0 root         (0) root         (0)     8182 2024-04-16 15:47:11.000000 ilcdirac-35.0.3/src/ILCDIRAC/Workflow/Modules/PythiaAnalysis.py
+-rw-rw-rw-   0 root         (0) root         (0)     5743 2024-04-16 15:47:11.000000 ilcdirac-35.0.3/src/ILCDIRAC/Workflow/Modules/RegisterOutputData.py
+-rw-rw-rw-   0 root         (0) root         (0)     3640 2024-04-16 15:47:11.000000 ilcdirac-35.0.3/src/ILCDIRAC/Workflow/Modules/RemoveInputData.py
+-rw-rw-rw-   0 root         (0) root         (0)     2095 2024-04-16 15:47:11.000000 ilcdirac-35.0.3/src/ILCDIRAC/Workflow/Modules/ReportErrors.py
+-rw-rw-rw-   0 root         (0) root         (0)     5915 2024-04-16 15:47:11.000000 ilcdirac-35.0.3/src/ILCDIRAC/Workflow/Modules/RootExecutableAnalysis.py
+-rw-rw-rw-   0 root         (0) root         (0)     5740 2024-04-16 15:47:11.000000 ilcdirac-35.0.3/src/ILCDIRAC/Workflow/Modules/RootMacroAnalysis.py
+-rw-rw-rw-   0 root         (0) root         (0)     4935 2024-04-16 15:47:11.000000 ilcdirac-35.0.3/src/ILCDIRAC/Workflow/Modules/SIDRegisterOutputData.py
+-rw-rw-rw-   0 root         (0) root         (0)    11639 2024-04-16 15:47:11.000000 ilcdirac-35.0.3/src/ILCDIRAC/Workflow/Modules/SLICAnalysis.py
+-rw-rw-rw-   0 root         (0) root         (0)    11192 2024-04-16 15:47:11.000000 ilcdirac-35.0.3/src/ILCDIRAC/Workflow/Modules/SLICPandoraAnalysis.py
+-rw-rw-rw-   0 root         (0) root         (0)     4044 2024-04-16 15:47:11.000000 ilcdirac-35.0.3/src/ILCDIRAC/Workflow/Modules/StdHepConverter.py
+-rw-rw-rw-   0 root         (0) root         (0)     9340 2024-04-16 15:47:11.000000 ilcdirac-35.0.3/src/ILCDIRAC/Workflow/Modules/StdHepCut.py
+-rw-rw-rw-   0 root         (0) root         (0)     3020 2024-04-16 15:47:11.000000 ilcdirac-35.0.3/src/ILCDIRAC/Workflow/Modules/StdHepCutJava.py
+-rw-rw-rw-   0 root         (0) root         (0)     8569 2024-04-16 15:47:11.000000 ilcdirac-35.0.3/src/ILCDIRAC/Workflow/Modules/StdHepSplit.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-16 15:47:28.383816 ilcdirac-35.0.3/src/ILCDIRAC/Workflow/Modules/Test/
+-rw-rw-rw-   0 root         (0) root         (0)     2311 2024-04-16 15:47:11.000000 ilcdirac-35.0.3/src/ILCDIRAC/Workflow/Modules/Test/MakeRequest.py
+-rw-rw-rw-   0 root         (0) root         (0)    12596 2024-04-16 15:47:11.000000 ilcdirac-35.0.3/src/ILCDIRAC/Workflow/Modules/Test/Test_BabayagaAnalysis.py
+-rw-rw-rw-   0 root         (0) root         (0)    13750 2024-04-16 15:47:11.000000 ilcdirac-35.0.3/src/ILCDIRAC/Workflow/Modules/Test/Test_BhlumiAnalysis.py
+-rw-rw-rw-   0 root         (0) root         (0)    14814 2024-04-16 15:47:11.000000 ilcdirac-35.0.3/src/ILCDIRAC/Workflow/Modules/Test/Test_Calibration.py
+-rw-rw-rw-   0 root         (0) root         (0)    45457 2024-04-16 15:47:11.000000 ilcdirac-35.0.3/src/ILCDIRAC/Workflow/Modules/Test/Test_DDSimWorkflow.py
+-rw-rw-rw-   0 root         (0) root         (0)    20933 2024-04-16 15:47:11.000000 ilcdirac-35.0.3/src/ILCDIRAC/Workflow/Modules/Test/Test_DelphesAppModule.py
+-rw-rw-rw-   0 root         (0) root         (0)    28578 2024-04-16 15:47:11.000000 ilcdirac-35.0.3/src/ILCDIRAC/Workflow/Modules/Test/Test_FccAnalysis.py
+-rw-rw-rw-   0 root         (0) root         (0)    20006 2024-04-16 15:47:11.000000 ilcdirac-35.0.3/src/ILCDIRAC/Workflow/Modules/Test/Test_GaudiAppModule.py
+-rw-rw-rw-   0 root         (0) root         (0)    11611 2024-04-16 15:47:11.000000 ilcdirac-35.0.3/src/ILCDIRAC/Workflow/Modules/Test/Test_KKMCAnalysis.py
+-rw-rw-rw-   0 root         (0) root         (0)    45397 2024-04-16 15:47:11.000000 ilcdirac-35.0.3/src/ILCDIRAC/Workflow/Modules/Test/Test_MarlinAnalysis.py
+-rw-rw-rw-   0 root         (0) root         (0)    43848 2024-04-16 15:47:11.000000 ilcdirac-35.0.3/src/ILCDIRAC/Workflow/Modules/Test/Test_ModuleBase.py
+-rw-rw-rw-   0 root         (0) root         (0)    41500 2024-04-16 15:47:11.000000 ilcdirac-35.0.3/src/ILCDIRAC/Workflow/Modules/Test/Test_OverlayInput.py
+-rw-rw-rw-   0 root         (0) root         (0)    10867 2024-04-16 15:47:11.000000 ilcdirac-35.0.3/src/ILCDIRAC/Workflow/Modules/Test/Test_RegisterOutputData.py
+-rw-rw-rw-   0 root         (0) root         (0)     2626 2024-04-16 15:47:11.000000 ilcdirac-35.0.3/src/ILCDIRAC/Workflow/Modules/Test/Test_ReportErrors.py
+-rw-rw-rw-   0 root         (0) root         (0)     8844 2024-04-16 15:47:11.000000 ilcdirac-35.0.3/src/ILCDIRAC/Workflow/Modules/Test/Test_RootExecutableAnalysis.py
+-rw-rw-rw-   0 root         (0) root         (0)    28021 2024-04-16 15:47:11.000000 ilcdirac-35.0.3/src/ILCDIRAC/Workflow/Modules/Test/Test_SLICPandoraAnalysis.py
+-rw-rw-rw-   0 root         (0) root         (0)     3462 2024-04-16 15:47:11.000000 ilcdirac-35.0.3/src/ILCDIRAC/Workflow/Modules/Test/Test_SlicPandora.py
+-rw-rw-rw-   0 root         (0) root         (0)    19461 2024-04-16 15:47:11.000000 ilcdirac-35.0.3/src/ILCDIRAC/Workflow/Modules/Test/Test_StdHepCut.py
+-rw-rw-rw-   0 root         (0) root         (0)    14457 2024-04-16 15:47:11.000000 ilcdirac-35.0.3/src/ILCDIRAC/Workflow/Modules/Test/Test_StdHepSplit.py
+-rw-rw-rw-   0 root         (0) root         (0)    12973 2024-04-16 15:47:11.000000 ilcdirac-35.0.3/src/ILCDIRAC/Workflow/Modules/Test/Test_UploadLogFile.py
+-rw-rw-rw-   0 root         (0) root         (0)    10007 2024-04-16 15:47:11.000000 ilcdirac-35.0.3/src/ILCDIRAC/Workflow/Modules/Test/Test_UploadOutputData.py
+-rw-rw-rw-   0 root         (0) root         (0)    32143 2024-04-16 15:47:11.000000 ilcdirac-35.0.3/src/ILCDIRAC/Workflow/Modules/Test/Test_UserJobFinalization.py
+-rw-rw-rw-   0 root         (0) root         (0)    16170 2024-04-16 15:47:11.000000 ilcdirac-35.0.3/src/ILCDIRAC/Workflow/Modules/Test/Test_Whizard2Workflow.py
+-rw-rw-rw-   0 root         (0) root         (0)    67243 2024-04-16 15:47:11.000000 ilcdirac-35.0.3/src/ILCDIRAC/Workflow/Modules/Test/Test_WhizardAnalysis.py
+-rw-rw-rw-   0 root         (0) root         (0)    86847 2024-04-16 15:47:11.000000 ilcdirac-35.0.3/src/ILCDIRAC/Workflow/Modules/Test/Test_WorkflowModuleRequests.py
+-rw-rw-rw-   0 root         (0) root         (0)     6505 2024-04-16 15:47:11.000000 ilcdirac-35.0.3/src/ILCDIRAC/Workflow/Modules/TomatoAnalysis.py
+-rw-rw-rw-   0 root         (0) root         (0)    17704 2024-04-16 15:47:11.000000 ilcdirac-35.0.3/src/ILCDIRAC/Workflow/Modules/UploadLogFile.py
+-rw-rw-rw-   0 root         (0) root         (0)    15076 2024-04-16 15:47:11.000000 ilcdirac-35.0.3/src/ILCDIRAC/Workflow/Modules/UploadOutputData.py
+-rw-rw-rw-   0 root         (0) root         (0)    17792 2024-04-16 15:47:11.000000 ilcdirac-35.0.3/src/ILCDIRAC/Workflow/Modules/UserJobFinalization.py
+-rw-rw-rw-   0 root         (0) root         (0)    13300 2024-04-16 15:47:11.000000 ilcdirac-35.0.3/src/ILCDIRAC/Workflow/Modules/Whizard2Analysis.py
+-rw-rw-rw-   0 root         (0) root         (0)    22938 2024-04-16 15:47:11.000000 ilcdirac-35.0.3/src/ILCDIRAC/Workflow/Modules/WhizardAnalysis.py
+-rw-rw-rw-   0 root         (0) root         (0)     1130 2024-04-16 15:47:11.000000 ilcdirac-35.0.3/src/ILCDIRAC/Workflow/Modules/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-16 15:47:28.384817 ilcdirac-35.0.3/src/ILCDIRAC/Workflow/Utilities/
+-rw-rw-rw-   0 root         (0) root         (0)     3265 2024-04-16 15:47:11.000000 ilcdirac-35.0.3/src/ILCDIRAC/Workflow/Utilities/CompactMixin.py
+-rw-rw-rw-   0 root         (0) root         (0)     5501 2024-04-16 15:47:11.000000 ilcdirac-35.0.3/src/ILCDIRAC/Workflow/Utilities/DD4hepMixin.py
+-rw-rw-rw-   0 root         (0) root         (0)     2714 2024-04-16 15:47:11.000000 ilcdirac-35.0.3/src/ILCDIRAC/Workflow/Utilities/RootMixin.py
+-rw-rw-rw-   0 root         (0) root         (0)     1066 2024-04-16 15:47:11.000000 ilcdirac-35.0.3/src/ILCDIRAC/Workflow/Utilities/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1167 2024-04-16 15:47:11.000000 ilcdirac-35.0.3/src/ILCDIRAC/Workflow/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-16 15:47:28.384817 ilcdirac-35.0.3/src/ILCDIRAC/WorkloadManagementSystem/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-16 15:47:28.385816 ilcdirac-35.0.3/src/ILCDIRAC/WorkloadManagementSystem/Agent/
+-rw-rw-rw-   0 root         (0) root         (0)    24475 2024-04-16 15:47:11.000000 ilcdirac-35.0.3/src/ILCDIRAC/WorkloadManagementSystem/Agent/JobResetAgent.py
+-rw-rw-rw-   0 root         (0) root         (0)     1013 2024-04-16 15:47:11.000000 ilcdirac-35.0.3/src/ILCDIRAC/WorkloadManagementSystem/Agent/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-16 15:47:28.385816 ilcdirac-35.0.3/src/ILCDIRAC/WorkloadManagementSystem/Client/
+-rw-rw-rw-   0 root         (0) root         (0)    15894 2024-04-16 15:47:11.000000 ilcdirac-35.0.3/src/ILCDIRAC/WorkloadManagementSystem/Client/DownloadInputData.py
+-rw-rw-rw-   0 root         (0) root         (0)     1083 2024-04-16 15:47:11.000000 ilcdirac-35.0.3/src/ILCDIRAC/WorkloadManagementSystem/Client/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      498 2024-04-16 15:47:11.000000 ilcdirac-35.0.3/src/ILCDIRAC/WorkloadManagementSystem/ConfigTemplate.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-16 15:47:28.386816 ilcdirac-35.0.3/src/ILCDIRAC/WorkloadManagementSystem/Executor/
+-rw-rw-rw-   0 root         (0) root         (0)     5646 2024-04-16 15:47:11.000000 ilcdirac-35.0.3/src/ILCDIRAC/WorkloadManagementSystem/Executor/SoftwareVersions.py
+-rw-rw-rw-   0 root         (0) root         (0)     1082 2024-04-16 15:47:11.000000 ilcdirac-35.0.3/src/ILCDIRAC/WorkloadManagementSystem/Executor/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-16 15:47:28.387817 ilcdirac-35.0.3/src/ILCDIRAC/WorkloadManagementSystem/Tests/
+-rw-rw-rw-   0 root         (0) root         (0)    13587 2024-04-16 15:47:11.000000 ilcdirac-35.0.3/src/ILCDIRAC/WorkloadManagementSystem/Tests/Test_Client_DownloadInputData.py
+-rw-rw-rw-   0 root         (0) root         (0)    31624 2024-04-16 15:47:11.000000 ilcdirac-35.0.3/src/ILCDIRAC/WorkloadManagementSystem/Tests/Test_JobResetAgent.py
+-rw-rw-rw-   0 root         (0) root         (0)     3345 2024-04-16 15:47:11.000000 ilcdirac-35.0.3/src/ILCDIRAC/WorkloadManagementSystem/Tests/Test_SoftwareVersions.py
+-rw-rw-rw-   0 root         (0) root         (0)     1083 2024-04-16 15:47:11.000000 ilcdirac-35.0.3/src/ILCDIRAC/WorkloadManagementSystem/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2395 2024-04-16 15:47:11.000000 ilcdirac-35.0.3/src/ILCDIRAC/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-16 15:47:28.389816 ilcdirac-35.0.3/src/iLCDirac.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2178 2024-04-16 15:47:28.000000 ilcdirac-35.0.3/src/iLCDirac.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)    25074 2024-04-16 15:47:28.000000 ilcdirac-35.0.3/src/iLCDirac.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-04-16 15:47:28.000000 ilcdirac-35.0.3/src/iLCDirac.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)     2121 2024-04-16 15:47:28.000000 ilcdirac-35.0.3/src/iLCDirac.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-04-16 15:47:27.000000 ilcdirac-35.0.3/src/iLCDirac.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)      300 2024-04-16 15:47:28.000000 ilcdirac-35.0.3/src/iLCDirac.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        9 2024-04-16 15:47:28.000000 ilcdirac-35.0.3/src/iLCDirac.egg-info/top_level.txt
```

### Comparing `iLCDirac-35.0.2/LICENSE` & `ilcdirac-35.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `iLCDirac-35.0.2/PKG-INFO` & `ilcdirac-35.0.3/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: iLCDirac
-Version: 35.0.2
+Version: 35.0.3
 Summary: iLCDirac is the iLC/CLIC/FCC extension of DIRAC
 Home-page: https://gitlab.cern.ch/clicdp/ilcdirac/ilcdirac.git
 Maintainer: Andre Sailer
 Maintainer-email: ilcdirac-support@cern.ch
 License: GPL-3.0-only
 Project-URL: Bug Tracker, https://its.cern.ch/jira/browse/ILCDIRAC
 Project-URL: Documentation, https://ilcdirac-doc.web.cern.ch/
@@ -13,15 +13,15 @@
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Topic :: Scientific/Engineering
 Classifier: Topic :: System :: Distributed Computing
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
-Requires-Dist: DIRAC~=8.0
+Requires-Dist: DIRAC>=8.0.41
 Requires-Dist: requests
 Requires-Dist: six
 Provides-Extra: server
 Requires-Dist: DIRAC[server]; extra == "server"
 Requires-Dist: psutil; extra == "server"
 Requires-Dist: suds-jurko; extra == "server"
 Provides-Extra: testing
```

### Comparing `iLCDirac-35.0.2/release.notes` & `ilcdirac-35.0.3/release.notes`

 * *Files 0% similar despite different names*

```diff
@@ -1,7 +1,18 @@
+[35.0.3]
+
+*ILCTransformation
+
+FIX: (!498) dirac-ilc-add-cvmfs-software has the dry run now working properly.
+
+*Workflow
+
+NEW: (!498) Whizard2 parses log files extracting luminosity, cross section and efficiency.
+NEW: (!498) Steering files for CLD are added to Gaudi.
+
 [35.0.2]
 Release date: 2024-03-15
 
 *Workflow
 
 FIX: (!497) DelphesPythia8_EDM4HEP now works correctly with LHE input files.
```

### Comparing `iLCDirac-35.0.2/releases.cfg` & `ilcdirac-35.0.3/releases.cfg`

 * *Files identical despite different names*

### Comparing `iLCDirac-35.0.2/setup.cfg` & `ilcdirac-35.0.3/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -22,15 +22,15 @@
 
 [options]
 python_requires = >=3.9
 package_dir = 
 	=src
 packages = find:
 install_requires = 
-	DIRAC ~= 8.0
+	DIRAC >= 8.0.41
 	requests
 	six
 zip_safe = False
 include_package_data = True
 
 [options.package_data]
 * = ConfigTemplate.cfg, *.sql
```

### Comparing `iLCDirac-35.0.2/src/ILCDIRAC/CalibrationSystem/Agent/CalibrationAgent.py` & `ilcdirac-35.0.3/src/ILCDIRAC/CalibrationSystem/Agent/CalibrationAgent.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-35.0.2/src/ILCDIRAC/CalibrationSystem/Agent/__init__.py` & `ilcdirac-35.0.3/src/ILCDIRAC/CalibrationSystem/Agent/__init__.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-35.0.2/src/ILCDIRAC/CalibrationSystem/Client/CalibrationClient.py` & `ilcdirac-35.0.3/src/ILCDIRAC/CalibrationSystem/Client/CalibrationClient.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-35.0.2/src/ILCDIRAC/CalibrationSystem/Client/__init__.py` & `ilcdirac-35.0.3/src/ILCDIRAC/CalibrationSystem/Client/__init__.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-35.0.2/src/ILCDIRAC/CalibrationSystem/ConfigTemplate.cfg` & `ilcdirac-35.0.3/src/ILCDIRAC/CalibrationSystem/ConfigTemplate.cfg`

 * *Files identical despite different names*

### Comparing `iLCDirac-35.0.2/src/ILCDIRAC/CalibrationSystem/Service/CalibrationHandler.py` & `ilcdirac-35.0.3/src/ILCDIRAC/CalibrationSystem/Service/CalibrationHandler.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-35.0.2/src/ILCDIRAC/CalibrationSystem/Service/CalibrationRun.py` & `ilcdirac-35.0.3/src/ILCDIRAC/CalibrationSystem/Service/CalibrationRun.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-35.0.2/src/ILCDIRAC/CalibrationSystem/Service/DetectorSettings.py` & `ilcdirac-35.0.3/src/ILCDIRAC/CalibrationSystem/Service/DetectorSettings.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-35.0.2/src/ILCDIRAC/CalibrationSystem/Service/__init__.py` & `ilcdirac-35.0.3/src/ILCDIRAC/CalibrationSystem/Service/__init__.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-35.0.2/src/ILCDIRAC/CalibrationSystem/TODO` & `ilcdirac-35.0.3/src/ILCDIRAC/CalibrationSystem/TODO`

 * *Files identical despite different names*

### Comparing `iLCDirac-35.0.2/src/ILCDIRAC/CalibrationSystem/Test/Test_CalibrationAgent.py` & `ilcdirac-35.0.3/src/ILCDIRAC/CalibrationSystem/Test/Test_CalibrationAgent.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-35.0.2/src/ILCDIRAC/CalibrationSystem/Test/Test_CalibrationClient.py` & `ilcdirac-35.0.3/src/ILCDIRAC/CalibrationSystem/Test/Test_CalibrationClient.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-35.0.2/src/ILCDIRAC/CalibrationSystem/Test/Test_CalibrationService.py` & `ilcdirac-35.0.3/src/ILCDIRAC/CalibrationSystem/Test/Test_CalibrationService.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-35.0.2/src/ILCDIRAC/CalibrationSystem/Test/Test_Util_fileutils.py` & `ilcdirac-35.0.3/src/ILCDIRAC/CalibrationSystem/Test/Test_Util_fileutils.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-35.0.2/src/ILCDIRAC/CalibrationSystem/Test/Test_Util_functions.py` & `ilcdirac-35.0.3/src/ILCDIRAC/CalibrationSystem/Test/Test_Util_functions.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-35.0.2/src/ILCDIRAC/CalibrationSystem/Test/__init__.py` & `ilcdirac-35.0.3/src/ILCDIRAC/CalibrationSystem/Test/__init__.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-35.0.2/src/ILCDIRAC/CalibrationSystem/Utilities/Python_Read_Scripts/ECal_Digi_Extract.py` & `ilcdirac-35.0.3/src/ILCDIRAC/CalibrationSystem/Utilities/Python_Read_Scripts/ECal_Digi_Extract.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-35.0.2/src/ILCDIRAC/CalibrationSystem/Utilities/Python_Read_Scripts/EM_Extract.py` & `ilcdirac-35.0.3/src/ILCDIRAC/CalibrationSystem/Utilities/Python_Read_Scripts/EM_Extract.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-35.0.2/src/ILCDIRAC/CalibrationSystem/Utilities/Python_Read_Scripts/Extract_GeVToMIP.py` & `ilcdirac-35.0.3/src/ILCDIRAC/CalibrationSystem/Utilities/Python_Read_Scripts/Extract_GeVToMIP.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-35.0.2/src/ILCDIRAC/CalibrationSystem/Utilities/Python_Read_Scripts/Extract_SimCaloHitMIPMPV.py` & `ilcdirac-35.0.3/src/ILCDIRAC/CalibrationSystem/Utilities/Python_Read_Scripts/Extract_SimCaloHitMIPMPV.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-35.0.2/src/ILCDIRAC/CalibrationSystem/Utilities/Python_Read_Scripts/Final_Calibration.py` & `ilcdirac-35.0.3/src/ILCDIRAC/CalibrationSystem/Utilities/Python_Read_Scripts/Final_Calibration.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-35.0.2/src/ILCDIRAC/CalibrationSystem/Utilities/Python_Read_Scripts/Final_Calibration.py.orig` & `ilcdirac-35.0.3/src/ILCDIRAC/CalibrationSystem/Utilities/Python_Read_Scripts/Final_Calibration.py.orig`

 * *Files identical despite different names*

### Comparing `iLCDirac-35.0.2/src/ILCDIRAC/CalibrationSystem/Utilities/Python_Read_Scripts/HCal_Digi_Extract.py` & `ilcdirac-35.0.3/src/ILCDIRAC/CalibrationSystem/Utilities/Python_Read_Scripts/HCal_Digi_Extract.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-35.0.2/src/ILCDIRAC/CalibrationSystem/Utilities/Python_Read_Scripts/HCal_Direction_Corrections_Extract.py` & `ilcdirac-35.0.3/src/ILCDIRAC/CalibrationSystem/Utilities/Python_Read_Scripts/HCal_Direction_Corrections_Extract.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-35.0.2/src/ILCDIRAC/CalibrationSystem/Utilities/Python_Read_Scripts/HCal_Ring_Digi_Extract.py` & `ilcdirac-35.0.3/src/ILCDIRAC/CalibrationSystem/Utilities/Python_Read_Scripts/HCal_Ring_Digi_Extract.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-35.0.2/src/ILCDIRAC/CalibrationSystem/Utilities/Python_Read_Scripts/HCal_Ring_Gear_Information.py` & `ilcdirac-35.0.3/src/ILCDIRAC/CalibrationSystem/Utilities/Python_Read_Scripts/HCal_Ring_Gear_Information.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-35.0.2/src/ILCDIRAC/CalibrationSystem/Utilities/Python_Read_Scripts/Had_Extract.py` & `ilcdirac-35.0.3/src/ILCDIRAC/CalibrationSystem/Utilities/Python_Read_Scripts/Had_Extract.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-35.0.2/src/ILCDIRAC/CalibrationSystem/Utilities/Python_Read_Scripts/Python_Read_Scripts.tgz` & `ilcdirac-35.0.3/src/ILCDIRAC/CalibrationSystem/Utilities/Python_Read_Scripts/Python_Read_Scripts.tgz`

 * *Files identical despite different names*

### Comparing `iLCDirac-35.0.2/src/ILCDIRAC/CalibrationSystem/Utilities/__init__.py` & `ilcdirac-35.0.3/src/ILCDIRAC/CalibrationSystem/Utilities/__init__.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-35.0.2/src/ILCDIRAC/CalibrationSystem/Utilities/auxiliaryFiles/parameterListMarlinSteeringFile.txt` & `ilcdirac-35.0.3/src/ILCDIRAC/CalibrationSystem/Utilities/auxiliaryFiles/parameterListMarlinSteeringFile.txt`

 * *Files identical despite different names*

### Comparing `iLCDirac-35.0.2/src/ILCDIRAC/CalibrationSystem/Utilities/auxiliaryFiles/pfoAnalysis.xml` & `ilcdirac-35.0.3/src/ILCDIRAC/CalibrationSystem/Utilities/auxiliaryFiles/pfoAnalysis.xml`

 * *Files identical despite different names*

### Comparing `iLCDirac-35.0.2/src/ILCDIRAC/CalibrationSystem/Utilities/fileutils.py` & `ilcdirac-35.0.3/src/ILCDIRAC/CalibrationSystem/Utilities/fileutils.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-35.0.2/src/ILCDIRAC/CalibrationSystem/Utilities/functions.py` & `ilcdirac-35.0.3/src/ILCDIRAC/CalibrationSystem/Utilities/functions.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-35.0.2/src/ILCDIRAC/CalibrationSystem/Utilities/mergePandoraLikelihoodData.py` & `ilcdirac-35.0.3/src/ILCDIRAC/CalibrationSystem/Utilities/mergePandoraLikelihoodData.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-35.0.2/src/ILCDIRAC/CalibrationSystem/Utilities/objectFactory.py` & `ilcdirac-35.0.3/src/ILCDIRAC/CalibrationSystem/Utilities/objectFactory.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-35.0.2/src/ILCDIRAC/CalibrationSystem/__init__.py` & `ilcdirac-35.0.3/src/ILCDIRAC/CalibrationSystem/__init__.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-35.0.2/src/ILCDIRAC/CalibrationSystem/dev_create_events.py` & `ilcdirac-35.0.3/src/ILCDIRAC/CalibrationSystem/dev_create_events.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-35.0.2/src/ILCDIRAC/Core/Utilities/CheckAndGetProdProxy.py` & `ilcdirac-35.0.3/src/ILCDIRAC/Core/Utilities/CheckAndGetProdProxy.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-35.0.2/src/ILCDIRAC/Core/Utilities/CheckXMLValidity.py` & `ilcdirac-35.0.3/src/ILCDIRAC/Core/Utilities/CheckXMLValidity.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-35.0.2/src/ILCDIRAC/Core/Utilities/CombinedSoftwareInstallation.py` & `ilcdirac-35.0.3/src/ILCDIRAC/Core/Utilities/CombinedSoftwareInstallation.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-35.0.2/src/ILCDIRAC/Core/Utilities/Configuration.py` & `ilcdirac-35.0.3/src/ILCDIRAC/Core/Utilities/Configuration.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-35.0.2/src/ILCDIRAC/Core/Utilities/DetectOS.py` & `ilcdirac-35.0.3/src/ILCDIRAC/Core/Utilities/DetectOS.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-35.0.2/src/ILCDIRAC/Core/Utilities/FileUtils.py` & `ilcdirac-35.0.3/src/ILCDIRAC/Core/Utilities/FileUtils.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-35.0.2/src/ILCDIRAC/Core/Utilities/FilenameEncoder.py` & `ilcdirac-35.0.3/src/ILCDIRAC/Core/Utilities/FilenameEncoder.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-35.0.2/src/ILCDIRAC/Core/Utilities/FindSteeringFileDir.py` & `ilcdirac-35.0.3/src/ILCDIRAC/Core/Utilities/FindSteeringFileDir.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-35.0.2/src/ILCDIRAC/Core/Utilities/GeneratorModels.py` & `ilcdirac-35.0.3/src/ILCDIRAC/Core/Utilities/GeneratorModels.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-35.0.2/src/ILCDIRAC/Core/Utilities/HTML.py` & `ilcdirac-35.0.3/src/ILCDIRAC/Core/Utilities/HTML.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-35.0.2/src/ILCDIRAC/Core/Utilities/InputDataResolution.py` & `ilcdirac-35.0.3/src/ILCDIRAC/Core/Utilities/InputDataResolution.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-35.0.2/src/ILCDIRAC/Core/Utilities/InputFilesUtilities.py` & `ilcdirac-35.0.3/src/ILCDIRAC/Core/Utilities/InputFilesUtilities.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-35.0.2/src/ILCDIRAC/Core/Utilities/InstalledFiles.py` & `ilcdirac-35.0.3/src/ILCDIRAC/Core/Utilities/InstalledFiles.py`

 * *Files 3% similar despite different names*

```diff
@@ -83,19 +83,20 @@
            "ild_00.gear",
            "ild_00_steering.xml",
            "ild_00.steer",
            "cuts_quarks_1400.txt", "cuts_taus_1400.txt",
            "cuts_h_gammaZ_1400.txt", "cuts_h_gammagamma_1400.txt",
            "cuts_h_mumu_3000.txt", 
            "card_IDEA.tcl", "edm4hep_IDEA.tcl",
-           "geant_fullsim_fccee_lar_pgun.py", 
            "k4simdelphesalg_pythia.py",
-           "pythia.py",
            "DECAY.dec",
            "evt.pdl",
+           "cld_steer.py",
+           "fcc_steer.py",
+           "CLDReconstruction.py",
            ]
   if myfile in files:
     return S_OK()
   elif configversion is None or platform is None:
     return S_ERROR("File %s is not available locally nor in the software installation." % myfile)
   else:
     return _checkInCVMFS(myfile, platform, configversion)
@@ -110,15 +111,15 @@
   configPath = Operations().getValue("/AvailableTarBalls/%(platform)s/%(app)s/%(version)s/CVMFSPath" %
                                          dict(version=version,
                                                platform=platform,
                                                app=app.lower(),
                                              ),
                                       "")
   if not configPath:
-    return S_ERROR("Cannot get CVMFSPath for this ILDConfig version: %s " % version)
+    return S_ERROR("Cannot get CVMFSPath for this Config version: %s " % version)
 
   # check if cvmfs exists on this machine, if not we guess the person knows what they are doing
   if not os.path.exists("/cvmfs"):
     LOG.warn("CMVFS does not exist on this machine, cannot check for file existance.")
     return S_OK()
 
   if os.path.exists(os.path.join(configPath, cFile)):
```

### Comparing `iLCDirac-35.0.2/src/ILCDIRAC/Core/Utilities/JobPathResolution.py` & `ilcdirac-35.0.3/src/ILCDIRAC/Core/Utilities/JobPathResolution.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-35.0.2/src/ILCDIRAC/Core/Utilities/LFNPathUtilities.py` & `ilcdirac-35.0.3/src/ILCDIRAC/Core/Utilities/LFNPathUtilities.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-35.0.2/src/ILCDIRAC/Core/Utilities/MarlinXML.py` & `ilcdirac-35.0.3/src/ILCDIRAC/Core/Utilities/MarlinXML.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-35.0.2/src/ILCDIRAC/Core/Utilities/OutputDataPolicy.py` & `ilcdirac-35.0.3/src/ILCDIRAC/Core/Utilities/OutputDataPolicy.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-35.0.2/src/ILCDIRAC/Core/Utilities/OverlayFiles.py` & `ilcdirac-35.0.3/src/ILCDIRAC/Core/Utilities/OverlayFiles.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-35.0.2/src/ILCDIRAC/Core/Utilities/PrepareLibs.py` & `ilcdirac-35.0.3/src/ILCDIRAC/Core/Utilities/PrepareLibs.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-35.0.2/src/ILCDIRAC/Core/Utilities/PrepareOptionFiles.py` & `ilcdirac-35.0.3/src/ILCDIRAC/Core/Utilities/PrepareOptionFiles.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-35.0.2/src/ILCDIRAC/Core/Utilities/ProcessList.py` & `ilcdirac-35.0.3/src/ILCDIRAC/Core/Utilities/ProcessList.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-35.0.2/src/ILCDIRAC/Core/Utilities/ProductionData.py` & `ilcdirac-35.0.3/src/ILCDIRAC/Core/Utilities/ProductionData.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-35.0.2/src/ILCDIRAC/Core/Utilities/RemoveSoft.py` & `ilcdirac-35.0.3/src/ILCDIRAC/Core/Utilities/RemoveSoft.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-35.0.2/src/ILCDIRAC/Core/Utilities/ResolveDependencies.py` & `ilcdirac-35.0.3/src/ILCDIRAC/Core/Utilities/ResolveDependencies.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-35.0.2/src/ILCDIRAC/Core/Utilities/ResolveSE.py` & `ilcdirac-35.0.3/src/ILCDIRAC/Core/Utilities/ResolveSE.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-35.0.2/src/ILCDIRAC/Core/Utilities/Splitting.py` & `ilcdirac-35.0.3/src/ILCDIRAC/Core/Utilities/Splitting.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-35.0.2/src/ILCDIRAC/Core/Utilities/TARsoft.py` & `ilcdirac-35.0.3/src/ILCDIRAC/Core/Utilities/TARsoft.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-35.0.2/src/ILCDIRAC/Core/Utilities/Utilities.py` & `ilcdirac-35.0.3/src/ILCDIRAC/Core/Utilities/Utilities.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-35.0.2/src/ILCDIRAC/Core/Utilities/WasteCPU.py` & `ilcdirac-35.0.3/src/ILCDIRAC/Core/Utilities/WasteCPU.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-35.0.2/src/ILCDIRAC/Core/Utilities/WhizardOptions.py` & `ilcdirac-35.0.3/src/ILCDIRAC/Core/Utilities/WhizardOptions.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-35.0.2/src/ILCDIRAC/Core/Utilities/__init__.py` & `ilcdirac-35.0.3/src/ILCDIRAC/Core/Utilities/__init__.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-35.0.2/src/ILCDIRAC/Core/Utilities/resolvePathsAndNames.py` & `ilcdirac-35.0.3/src/ILCDIRAC/Core/Utilities/resolvePathsAndNames.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-35.0.2/src/ILCDIRAC/Core/Utilities/tests/Test_CheckAndGetProd.py` & `ilcdirac-35.0.3/src/ILCDIRAC/Core/Utilities/tests/Test_CheckAndGetProd.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-35.0.2/src/ILCDIRAC/Core/Utilities/tests/Test_CombinedSoftwareInstallation.py` & `ilcdirac-35.0.3/src/ILCDIRAC/Core/Utilities/tests/Test_CombinedSoftwareInstallation.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-35.0.2/src/ILCDIRAC/Core/Utilities/tests/Test_Configuration.py` & `ilcdirac-35.0.3/src/ILCDIRAC/Core/Utilities/tests/Test_Configuration.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-35.0.2/src/ILCDIRAC/Core/Utilities/tests/Test_DetectOS.py` & `ilcdirac-35.0.3/src/ILCDIRAC/Core/Utilities/tests/Test_DetectOS.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-35.0.2/src/ILCDIRAC/Core/Utilities/tests/Test_FileUtils.py` & `ilcdirac-35.0.3/src/ILCDIRAC/Core/Utilities/tests/Test_FileUtils.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-35.0.2/src/ILCDIRAC/Core/Utilities/tests/Test_FilenameEncoder.py` & `ilcdirac-35.0.3/src/ILCDIRAC/Core/Utilities/tests/Test_FilenameEncoder.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-35.0.2/src/ILCDIRAC/Core/Utilities/tests/Test_FindSteeringFileDir.py` & `ilcdirac-35.0.3/src/ILCDIRAC/Core/Utilities/tests/Test_FindSteeringFileDir.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-35.0.2/src/ILCDIRAC/Core/Utilities/tests/Test_InputDataResolution.py` & `ilcdirac-35.0.3/src/ILCDIRAC/Core/Utilities/tests/Test_InputDataResolution.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-35.0.2/src/ILCDIRAC/Core/Utilities/tests/Test_InputFilesUtilities.py` & `ilcdirac-35.0.3/src/ILCDIRAC/Core/Utilities/tests/Test_InputFilesUtilities.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-35.0.2/src/ILCDIRAC/Core/Utilities/tests/Test_LFNPathUtilities.py` & `ilcdirac-35.0.3/src/ILCDIRAC/Core/Utilities/tests/Test_LFNPathUtilities.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-35.0.2/src/ILCDIRAC/Core/Utilities/tests/Test_OutputDataPolicy.py` & `ilcdirac-35.0.3/src/ILCDIRAC/Core/Utilities/tests/Test_OutputDataPolicy.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-35.0.2/src/ILCDIRAC/Core/Utilities/tests/Test_OverlayFiles.py` & `ilcdirac-35.0.3/src/ILCDIRAC/Core/Utilities/tests/Test_OverlayFiles.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-35.0.2/src/ILCDIRAC/Core/Utilities/tests/Test_PrepareLibs.py` & `ilcdirac-35.0.3/src/ILCDIRAC/Core/Utilities/tests/Test_PrepareLibs.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-35.0.2/src/ILCDIRAC/Core/Utilities/tests/Test_PrepareMarlinXML.py` & `ilcdirac-35.0.3/src/ILCDIRAC/Core/Utilities/tests/Test_PrepareMarlinXML.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-35.0.2/src/ILCDIRAC/Core/Utilities/tests/Test_PrepareOptionsFiles.py` & `ilcdirac-35.0.3/src/ILCDIRAC/Core/Utilities/tests/Test_PrepareOptionsFiles.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-35.0.2/src/ILCDIRAC/Core/Utilities/tests/Test_ProcessList.py` & `ilcdirac-35.0.3/src/ILCDIRAC/Core/Utilities/tests/Test_ProcessList.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-35.0.2/src/ILCDIRAC/Core/Utilities/tests/Test_ProductionData.py` & `ilcdirac-35.0.3/src/ILCDIRAC/Core/Utilities/tests/Test_ProductionData.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-35.0.2/src/ILCDIRAC/Core/Utilities/tests/Test_ProductionOutputData.py` & `ilcdirac-35.0.3/src/ILCDIRAC/Core/Utilities/tests/Test_ProductionOutputData.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-35.0.2/src/ILCDIRAC/Core/Utilities/tests/Test_ResolvePathsandNames.py` & `ilcdirac-35.0.3/src/ILCDIRAC/Core/Utilities/tests/Test_ResolvePathsandNames.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-35.0.2/src/ILCDIRAC/Core/Utilities/tests/Test_ResolveSEs.py` & `ilcdirac-35.0.3/src/ILCDIRAC/Core/Utilities/tests/Test_ResolveSEs.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-35.0.2/src/ILCDIRAC/Core/Utilities/tests/Test_Splitting.py` & `ilcdirac-35.0.3/src/ILCDIRAC/Core/Utilities/tests/Test_Splitting.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-35.0.2/src/ILCDIRAC/Core/Utilities/tests/Test_TARsoft.py` & `ilcdirac-35.0.3/src/ILCDIRAC/Core/Utilities/tests/Test_TARsoft.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-35.0.2/src/ILCDIRAC/Core/Utilities/tests/Test_Utilities.py` & `ilcdirac-35.0.3/src/ILCDIRAC/Core/Utilities/tests/Test_Utilities.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-35.0.2/src/ILCDIRAC/Core/Utilities/tests/Test_WasteCPU.py` & `ilcdirac-35.0.3/src/ILCDIRAC/Core/Utilities/tests/Test_WasteCPU.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-35.0.2/src/ILCDIRAC/Core/Utilities/tests/Test_WhizardOptions.py` & `ilcdirac-35.0.3/src/ILCDIRAC/Core/Utilities/tests/Test_WhizardOptions.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-35.0.2/src/ILCDIRAC/Core/__init__.py` & `ilcdirac-35.0.3/src/ILCDIRAC/Core/__init__.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-35.0.2/src/ILCDIRAC/Core/scripts/__init__.py` & `ilcdirac-35.0.3/src/ILCDIRAC/Core/scripts/__init__.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-35.0.2/src/ILCDIRAC/Core/scripts/createJavaTarBall.sh` & `ilcdirac-35.0.3/src/ILCDIRAC/Core/scripts/createJavaTarBall.sh`

 * *Files identical despite different names*

### Comparing `iLCDirac-35.0.2/src/ILCDIRAC/Core/scripts/createLCIOTarBall.sh` & `ilcdirac-35.0.3/src/ILCDIRAC/Core/scripts/createLCIOTarBall.sh`

 * *Files identical despite different names*

### Comparing `iLCDirac-35.0.2/src/ILCDIRAC/Core/scripts/createMarlinTarBall.sh` & `ilcdirac-35.0.3/src/ILCDIRAC/Core/scripts/createMarlinTarBall.sh`

 * *Files identical despite different names*

### Comparing `iLCDirac-35.0.2/src/ILCDIRAC/Core/scripts/createMokkaTarBall.sh` & `ilcdirac-35.0.3/src/ILCDIRAC/Core/scripts/createMokkaTarBall.sh`

 * *Files identical despite different names*

### Comparing `iLCDirac-35.0.2/src/ILCDIRAC/Core/scripts/createSlicPandoraTarBall.sh` & `ilcdirac-35.0.3/src/ILCDIRAC/Core/scripts/createSlicPandoraTarBall.sh`

 * *Files identical despite different names*

### Comparing `iLCDirac-35.0.2/src/ILCDIRAC/Core/scripts/createTarBallForProgram.sh` & `ilcdirac-35.0.3/src/ILCDIRAC/Core/scripts/createTarBallForProgram.sh`

 * *Files identical despite different names*

### Comparing `iLCDirac-35.0.2/src/ILCDIRAC/Core/scripts/dirac-architecture` & `ilcdirac-35.0.3/src/ILCDIRAC/Core/scripts/dirac-architecture`

 * *Files identical despite different names*

### Comparing `iLCDirac-35.0.2/src/ILCDIRAC/Core/scripts/dirac_ilc_add_cvmfs_software.py` & `ilcdirac-35.0.3/src/ILCDIRAC/Core/scripts/dirac_ilc_add_cvmfs_software.py`

 * *Files 0% similar despite different names*

```diff
@@ -163,15 +163,15 @@
 
     Script.registerSwitch("Q:", "DBSlice=", "Path to Mokka DB Slice", self.setDBSlice)
     Script.registerSwitch('', 'MarlinPandoraVersion=', 'Version of MarlinPandora, needed for '
                           'pandora_calibration_scripts', self._setMPV)
     Script.registerSwitch('', 'PandoraAnalysisVersion=', 'Version of PandoraAnalysis, needed for '
                           'pandora_calibration_scripts', self._setPAV)
 
-    Script.registerSwitch("N", "dry-run", "DryRun: do not commit to CS", self.dryRun)
+    Script.registerSwitch("N", "dry-run", "DryRun: do not commit to CS", self.setDryrun)
 
     Script.setUsageMessage('\n'.join([__doc__.split('\n')[1],
                                          '\nUsage:',
                                          '  %s [option|cfgfile] ...\n' % Script.scriptName]))
 
 
 class CVMFSAdder(object):
```

### Comparing `iLCDirac-35.0.2/src/ILCDIRAC/Core/scripts/dirac_ilc_add_software.py` & `ilcdirac-35.0.3/src/ILCDIRAC/Core/scripts/dirac_ilc_add_software.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-35.0.2/src/ILCDIRAC/Core/scripts/dirac_ilc_add_user.py` & `ilcdirac-35.0.3/src/ILCDIRAC/Core/scripts/dirac_ilc_add_user.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-35.0.2/src/ILCDIRAC/Core/scripts/dirac_ilc_add_whizard.py` & `ilcdirac-35.0.3/src/ILCDIRAC/Core/scripts/dirac_ilc_add_whizard.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-35.0.2/src/ILCDIRAC/Core/scripts/dirac_ilc_list_users.py` & `ilcdirac-35.0.3/src/ILCDIRAC/Core/scripts/dirac_ilc_list_users.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-35.0.2/src/ILCDIRAC/Core/scripts/ilcdirac-install.sh` & `ilcdirac-35.0.3/src/ILCDIRAC/Core/scripts/ilcdirac-install.sh`

 * *Files identical despite different names*

### Comparing `iLCDirac-35.0.2/src/ILCDIRAC/DataManagementSystem/Agent/RequestOperations/LogUpload.py` & `ilcdirac-35.0.3/src/ILCDIRAC/DataManagementSystem/Agent/RequestOperations/LogUpload.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-35.0.2/src/ILCDIRAC/DataManagementSystem/Agent/RequestOperations/__init__.py` & `ilcdirac-35.0.3/src/ILCDIRAC/DataManagementSystem/Agent/RequestOperations/__init__.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-35.0.2/src/ILCDIRAC/DataManagementSystem/Agent/__init__.py` & `ilcdirac-35.0.3/src/ILCDIRAC/DataManagementSystem/Agent/__init__.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-35.0.2/src/ILCDIRAC/DataManagementSystem/__init__.py` & `ilcdirac-35.0.3/src/ILCDIRAC/DataManagementSystem/__init__.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-35.0.2/src/ILCDIRAC/FrameworkSystem/Agent/__init__.py` & `ilcdirac-35.0.3/src/ILCDIRAC/FrameworkSystem/Agent/__init__.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-35.0.2/src/ILCDIRAC/FrameworkSystem/__init__.py` & `ilcdirac-35.0.3/src/ILCDIRAC/FrameworkSystem/__init__.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-35.0.2/src/ILCDIRAC/ILCTransformationSystem/Agent/FileStatusTransformationAgent.py` & `ilcdirac-35.0.3/src/ILCDIRAC/ILCTransformationSystem/Agent/FileStatusTransformationAgent.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-35.0.2/src/ILCDIRAC/ILCTransformationSystem/Agent/TarTheLogsAgent.py` & `ilcdirac-35.0.3/src/ILCDIRAC/ILCTransformationSystem/Agent/TarTheLogsAgent.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-35.0.2/src/ILCDIRAC/ILCTransformationSystem/Agent/TransformationPlugin.py` & `ilcdirac-35.0.3/src/ILCDIRAC/ILCTransformationSystem/Agent/TransformationPlugin.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-35.0.2/src/ILCDIRAC/ILCTransformationSystem/Agent/__init__.py` & `ilcdirac-35.0.3/src/ILCDIRAC/ILCTransformationSystem/Agent/__init__.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-35.0.2/src/ILCDIRAC/ILCTransformationSystem/Client/Transformation.py` & `ilcdirac-35.0.3/src/ILCDIRAC/ILCTransformationSystem/Client/Transformation.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-35.0.2/src/ILCDIRAC/ILCTransformationSystem/Client/__init__.py` & `ilcdirac-35.0.3/src/ILCDIRAC/ILCTransformationSystem/Client/__init__.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-35.0.2/src/ILCDIRAC/ILCTransformationSystem/Tests/Test_FileStatusTransformationAgent.py` & `ilcdirac-35.0.3/src/ILCDIRAC/ILCTransformationSystem/Tests/Test_FileStatusTransformationAgent.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-35.0.2/src/ILCDIRAC/ILCTransformationSystem/Tests/Test_ReleaseHelper.py` & `ilcdirac-35.0.3/src/ILCDIRAC/ILCTransformationSystem/Tests/Test_ReleaseHelper.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-35.0.2/src/ILCDIRAC/ILCTransformationSystem/Tests/Test_TransformationPlugin.py` & `ilcdirac-35.0.3/src/ILCDIRAC/ILCTransformationSystem/Tests/Test_TransformationPlugin.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-35.0.2/src/ILCDIRAC/ILCTransformationSystem/Tests/Test_createMovingTransformation.py` & `ilcdirac-35.0.3/src/ILCDIRAC/ILCTransformationSystem/Tests/Test_createMovingTransformation.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-35.0.2/src/ILCDIRAC/ILCTransformationSystem/Tests/Test_diracClicMakeProductions.py` & `ilcdirac-35.0.3/src/ILCDIRAC/ILCTransformationSystem/Tests/Test_diracClicMakeProductions.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-35.0.2/src/ILCDIRAC/ILCTransformationSystem/Tests/Test_diracFccMakeProductions.py` & `ilcdirac-35.0.3/src/ILCDIRAC/ILCTransformationSystem/Tests/Test_diracFccMakeProductions.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-35.0.2/src/ILCDIRAC/ILCTransformationSystem/Tests/test_diracIlcAddTasks.py` & `ilcdirac-35.0.3/src/ILCDIRAC/ILCTransformationSystem/Tests/test_diracIlcAddTasks.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-35.0.2/src/ILCDIRAC/ILCTransformationSystem/Tests/test_utilities.py` & `ilcdirac-35.0.3/src/ILCDIRAC/ILCTransformationSystem/Tests/test_utilities.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-35.0.2/src/ILCDIRAC/ILCTransformationSystem/Utilities/DataParameters.py` & `ilcdirac-35.0.3/src/ILCDIRAC/ILCTransformationSystem/Utilities/DataParameters.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-35.0.2/src/ILCDIRAC/ILCTransformationSystem/Utilities/ReleaseHelper.py` & `ilcdirac-35.0.3/src/ILCDIRAC/ILCTransformationSystem/Utilities/ReleaseHelper.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-35.0.2/src/ILCDIRAC/ILCTransformationSystem/Utilities/Utilities.py` & `ilcdirac-35.0.3/src/ILCDIRAC/ILCTransformationSystem/Utilities/Utilities.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-35.0.2/src/ILCDIRAC/ILCTransformationSystem/Utilities/__init__.py` & `ilcdirac-35.0.3/src/ILCDIRAC/ILCTransformationSystem/Utilities/__init__.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-35.0.2/src/ILCDIRAC/ILCTransformationSystem/__init__.py` & `ilcdirac-35.0.3/src/ILCDIRAC/ILCTransformationSystem/__init__.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-35.0.2/src/ILCDIRAC/ILCTransformationSystem/scripts/__init__.py` & `ilcdirac-35.0.3/src/ILCDIRAC/ILCTransformationSystem/scripts/__init__.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-35.0.2/src/ILCDIRAC/ILCTransformationSystem/scripts/dirac_clic_make_productions.py` & `ilcdirac-35.0.3/src/ILCDIRAC/ILCTransformationSystem/scripts/dirac_clic_make_productions.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-35.0.2/src/ILCDIRAC/ILCTransformationSystem/scripts/dirac_fcc_make_productions.py` & `ilcdirac-35.0.3/src/ILCDIRAC/ILCTransformationSystem/scripts/dirac_fcc_make_productions.py`

 * *Files 0% similar despite different names*

```diff
@@ -695,14 +695,15 @@
     self._setApplicationOptions('KKMC', kkmcee, task.applicationOptions)
     return kkmcee
 
   def createWhizard2Application(self, task):
     """create Whizard2 Application."""
     from ILCDIRAC.Interfaces.API.NewInterface.Applications import Whizard2
     whiz = Whizard2()
+    whiz._decayProc = ['proc']
     whiz.setVersion(self.softwareVersion)
     whiz.setNumberOfEvents(task.eventsPerJob)
     whiz.setSinFile(task.genFile)
     whiz.setEvtType(task.meta['EvtType'])
     whiz.setEnergy(task.meta['Energy'])
     whiz.datatype = 'stdhep'
     self._setApplicationOptions('whizard2', whiz, task.applicationOptions)
@@ -770,15 +771,15 @@
     """create DDSim Application."""
     from ILCDIRAC.Interfaces.API.NewInterface.Applications import DDSim
     ddsim = DDSim()
     ddsim.setVersion(self.softwareVersion)
     ddsim.setDetectorModel(self.detectorModel)
     ddsim.setNumberOfEvents(task.eventsPerJob)
     ddsim.setEnergy(task.meta['Energy'])
-    self._setApplicationOptions('DDSim', ddsim, task.applicationOptions)
+    self._setApplicationOptions('ddsim', ddsim, task.applicationOptions)
     ddsim.datatype = 'sim'
     return ddsim
 
   def createGenerationProduction(self, task):
     """Create generation production."""
     prodName = task.getProdName(self.machine, 'gen', self.additionalName)
     parameterDict = task.parameterDict
@@ -1024,14 +1025,15 @@
     """return production job instance with some parameters set."""
     from ILCDIRAC.Interfaces.API.NewInterface.ProductionJob import ProductionJob
     prodJob = ProductionJob()
     prodJob.setLogLevel(self.productionLogLevel)
     prodJob.setProdGroup(self.prodGroup)
     prodJob.setOutputSE(self.outputSE)
     prodJob.basepath = self.basepath
+    prodJob.campaign = self.campaign
     prodJob.dryrun = self._flags.dryRun
     prodJob.maxFCFoldersToCheck = 1
     return prodJob
 
   def _setApplicationOptions(self, appName, app, optionsDict=None):
     """set options for given application.
```

### Comparing `iLCDirac-35.0.2/src/ILCDIRAC/ILCTransformationSystem/scripts/dirac_ilc_add_tasks_to_prod.py` & `ilcdirac-35.0.3/src/ILCDIRAC/ILCTransformationSystem/scripts/dirac_ilc_add_tasks_to_prod.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-35.0.2/src/ILCDIRAC/ILCTransformationSystem/scripts/dirac_ilc_filestatus_transformation.py` & `ilcdirac-35.0.3/src/ILCDIRAC/ILCTransformationSystem/scripts/dirac_ilc_filestatus_transformation.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-35.0.2/src/ILCDIRAC/ILCTransformationSystem/scripts/dirac_ilc_get_info.py` & `ilcdirac-35.0.3/src/ILCDIRAC/ILCTransformationSystem/scripts/dirac_ilc_get_info.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-35.0.2/src/ILCDIRAC/ILCTransformationSystem/scripts/dirac_ilc_get_prod_log.py` & `ilcdirac-35.0.3/src/ILCDIRAC/ILCTransformationSystem/scripts/dirac_ilc_get_prod_log.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-35.0.2/src/ILCDIRAC/ILCTransformationSystem/scripts/dirac_ilc_make_ddsimtarball.py` & `ilcdirac-35.0.3/src/ILCDIRAC/ILCTransformationSystem/scripts/dirac_ilc_make_ddsimtarball.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-35.0.2/src/ILCDIRAC/ILCTransformationSystem/scripts/dirac_ilc_moving_transformation.py` & `ilcdirac-35.0.3/src/ILCDIRAC/ILCTransformationSystem/scripts/dirac_ilc_moving_transformation.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-35.0.2/src/ILCDIRAC/ILCTransformationSystem/scripts/dirac_ilc_production_summary.py` & `ilcdirac-35.0.3/src/ILCDIRAC/ILCTransformationSystem/scripts/dirac_ilc_production_summary.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-35.0.2/src/ILCDIRAC/ILCTransformationSystem/scripts/dirac_ilc_replication_transformation.py` & `ilcdirac-35.0.3/src/ILCDIRAC/ILCTransformationSystem/scripts/dirac_ilc_replication_transformation.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-35.0.2/src/ILCDIRAC/ILCTransformationSystem/scripts/dirac_ilc_upload_gen_files.py` & `ilcdirac-35.0.3/src/ILCDIRAC/ILCTransformationSystem/scripts/dirac_ilc_upload_gen_files.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-35.0.2/src/ILCDIRAC/Interfaces/API/DiracILC.py` & `ilcdirac-35.0.3/src/ILCDIRAC/Interfaces/API/DiracILC.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-35.0.2/src/ILCDIRAC/Interfaces/API/Examples/SIDChain/bannedSites.py` & `ilcdirac-35.0.3/src/ILCDIRAC/Interfaces/API/Examples/SIDChain/bannedSites.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-35.0.2/src/ILCDIRAC/Interfaces/API/Examples/SIDChain/defaultPrePandoraLcsim.xml` & `ilcdirac-35.0.3/src/ILCDIRAC/Interfaces/API/Examples/SIDChain/defaultPrePandoraLcsim.xml`

 * *Files identical despite different names*

### Comparing `iLCDirac-35.0.2/src/ILCDIRAC/Interfaces/API/Examples/SIDChain/defaultPrePandoraLcsimOverlay.xml` & `ilcdirac-35.0.3/src/ILCDIRAC/Interfaces/API/Examples/SIDChain/defaultPrePandoraLcsimOverlay.xml`

 * *Files identical despite different names*

### Comparing `iLCDirac-35.0.2/src/ILCDIRAC/Interfaces/API/Examples/SIDChain/fileLists/testSimList.py` & `ilcdirac-35.0.3/src/ILCDIRAC/Interfaces/API/Examples/SIDChain/fileLists/testSimList.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-35.0.2/src/ILCDIRAC/Interfaces/API/Examples/SIDChain/fileLists/testStdhepList.py` & `ilcdirac-35.0.3/src/ILCDIRAC/Interfaces/API/Examples/SIDChain/fileLists/testStdhepList.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-35.0.2/src/ILCDIRAC/Interfaces/API/Examples/SiDProduction/sid_dbd_sim_production_default.py` & `ilcdirac-35.0.3/src/ILCDIRAC/Interfaces/API/Examples/SiDProduction/sid_dbd_sim_production_default.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-35.0.2/src/ILCDIRAC/Interfaces/API/NewInterface/Application.py` & `ilcdirac-35.0.3/src/ILCDIRAC/Interfaces/API/NewInterface/Application.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-35.0.2/src/ILCDIRAC/Interfaces/API/NewInterface/Applications/Babayaga.py` & `ilcdirac-35.0.3/src/ILCDIRAC/Interfaces/API/NewInterface/Applications/Babayaga.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-35.0.2/src/ILCDIRAC/Interfaces/API/NewInterface/Applications/Bhlumi.py` & `ilcdirac-35.0.3/src/ILCDIRAC/Interfaces/API/NewInterface/Applications/Bhlumi.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-35.0.2/src/ILCDIRAC/Interfaces/API/NewInterface/Applications/Calibration.py` & `ilcdirac-35.0.3/src/ILCDIRAC/Interfaces/API/NewInterface/Applications/Calibration.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-35.0.2/src/ILCDIRAC/Interfaces/API/NewInterface/Applications/CheckCollections.py` & `ilcdirac-35.0.3/src/ILCDIRAC/Interfaces/API/NewInterface/Applications/CheckCollections.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-35.0.2/src/ILCDIRAC/Interfaces/API/NewInterface/Applications/CheckWNs.py` & `ilcdirac-35.0.3/src/ILCDIRAC/Interfaces/API/NewInterface/Applications/CheckWNs.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-35.0.2/src/ILCDIRAC/Interfaces/API/NewInterface/Applications/DDSim.py` & `ilcdirac-35.0.3/src/ILCDIRAC/Interfaces/API/NewInterface/Applications/DDSim.py`

 * *Files 1% similar despite different names*

```diff
@@ -77,14 +77,15 @@
     self.extraParticles = []
     super(DDSim, self).__init__(paramdict)
     # Those 5 need to come after default constructor
     self._modulename = 'DDSimAnalysis'
     self._moduledescription = 'Module to run DDSim'
     self.appname = 'ddsim'
     self.datatype = 'SIM'
+    self._extension = 'root'
     self._paramsToExclude.extend(["outputDstPath", "outputRecPath", "OutputDstFile", "OutputRecFile"])
     self._ops = Operations()
 
   @property
   def detectortype(self):
     """detectorType needed for transformations."""
     return self.detectorModel
```

### Comparing `iLCDirac-35.0.2/src/ILCDIRAC/Interfaces/API/NewInterface/Applications/DelphesApp.py` & `ilcdirac-35.0.3/src/ILCDIRAC/Interfaces/API/NewInterface/Applications/DelphesApp.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-35.0.2/src/ILCDIRAC/Interfaces/API/NewInterface/Applications/Fcc.py` & `ilcdirac-35.0.3/src/ILCDIRAC/Interfaces/API/NewInterface/Applications/Fcc.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-35.0.2/src/ILCDIRAC/Interfaces/API/NewInterface/Applications/GaudiApp.py` & `ilcdirac-35.0.3/src/ILCDIRAC/Interfaces/API/NewInterface/Applications/GaudiApp.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-35.0.2/src/ILCDIRAC/Interfaces/API/NewInterface/Applications/GenericApplication.py` & `ilcdirac-35.0.3/src/ILCDIRAC/Interfaces/API/NewInterface/Applications/GenericApplication.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-35.0.2/src/ILCDIRAC/Interfaces/API/NewInterface/Applications/GetSRMFile.py` & `ilcdirac-35.0.3/src/ILCDIRAC/Interfaces/API/NewInterface/Applications/GetSRMFile.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-35.0.2/src/ILCDIRAC/Interfaces/API/NewInterface/Applications/KKMC.py` & `ilcdirac-35.0.3/src/ILCDIRAC/Interfaces/API/NewInterface/Applications/KKMC.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-35.0.2/src/ILCDIRAC/Interfaces/API/NewInterface/Applications/LCSIM.py` & `ilcdirac-35.0.3/src/ILCDIRAC/Interfaces/API/NewInterface/Applications/LCSIM.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-35.0.2/src/ILCDIRAC/Interfaces/API/NewInterface/Applications/Marlin.py` & `ilcdirac-35.0.3/src/ILCDIRAC/Interfaces/API/NewInterface/Applications/Marlin.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-35.0.2/src/ILCDIRAC/Interfaces/API/NewInterface/Applications/Mokka.py` & `ilcdirac-35.0.3/src/ILCDIRAC/Interfaces/API/NewInterface/Applications/Mokka.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-35.0.2/src/ILCDIRAC/Interfaces/API/NewInterface/Applications/OverlayInput.py` & `ilcdirac-35.0.3/src/ILCDIRAC/Interfaces/API/NewInterface/Applications/OverlayInput.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-35.0.2/src/ILCDIRAC/Interfaces/API/NewInterface/Applications/PostGenSelection.py` & `ilcdirac-35.0.3/src/ILCDIRAC/Interfaces/API/NewInterface/Applications/PostGenSelection.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-35.0.2/src/ILCDIRAC/Interfaces/API/NewInterface/Applications/Pythia.py` & `ilcdirac-35.0.3/src/ILCDIRAC/Interfaces/API/NewInterface/Applications/Pythia.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-35.0.2/src/ILCDIRAC/Interfaces/API/NewInterface/Applications/RootMacro.py` & `ilcdirac-35.0.3/src/ILCDIRAC/Interfaces/API/NewInterface/Applications/RootMacro.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-35.0.2/src/ILCDIRAC/Interfaces/API/NewInterface/Applications/RootScript.py` & `ilcdirac-35.0.3/src/ILCDIRAC/Interfaces/API/NewInterface/Applications/RootScript.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-35.0.2/src/ILCDIRAC/Interfaces/API/NewInterface/Applications/SLCIOConcatenate.py` & `ilcdirac-35.0.3/src/ILCDIRAC/Interfaces/API/NewInterface/Applications/SLCIOConcatenate.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-35.0.2/src/ILCDIRAC/Interfaces/API/NewInterface/Applications/SLCIOSplit.py` & `ilcdirac-35.0.3/src/ILCDIRAC/Interfaces/API/NewInterface/Applications/SLCIOSplit.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-35.0.2/src/ILCDIRAC/Interfaces/API/NewInterface/Applications/SLIC.py` & `ilcdirac-35.0.3/src/ILCDIRAC/Interfaces/API/NewInterface/Applications/SLIC.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-35.0.2/src/ILCDIRAC/Interfaces/API/NewInterface/Applications/SLICPandora.py` & `ilcdirac-35.0.3/src/ILCDIRAC/Interfaces/API/NewInterface/Applications/SLICPandora.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-35.0.2/src/ILCDIRAC/Interfaces/API/NewInterface/Applications/StdHepSplit.py` & `ilcdirac-35.0.3/src/ILCDIRAC/Interfaces/API/NewInterface/Applications/StdHepSplit.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-35.0.2/src/ILCDIRAC/Interfaces/API/NewInterface/Applications/StdhepCut.py` & `ilcdirac-35.0.3/src/ILCDIRAC/Interfaces/API/NewInterface/Applications/StdhepCut.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-35.0.2/src/ILCDIRAC/Interfaces/API/NewInterface/Applications/StdhepCutJava.py` & `ilcdirac-35.0.3/src/ILCDIRAC/Interfaces/API/NewInterface/Applications/StdhepCutJava.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-35.0.2/src/ILCDIRAC/Interfaces/API/NewInterface/Applications/Tomato.py` & `ilcdirac-35.0.3/src/ILCDIRAC/Interfaces/API/NewInterface/Applications/Tomato.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-35.0.2/src/ILCDIRAC/Interfaces/API/NewInterface/Applications/Whizard.py` & `ilcdirac-35.0.3/src/ILCDIRAC/Interfaces/API/NewInterface/Applications/Whizard.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-35.0.2/src/ILCDIRAC/Interfaces/API/NewInterface/Applications/Whizard2.py` & `ilcdirac-35.0.3/src/ILCDIRAC/Interfaces/API/NewInterface/Applications/Whizard2.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-35.0.2/src/ILCDIRAC/Interfaces/API/NewInterface/Applications/_Root.py` & `ilcdirac-35.0.3/src/ILCDIRAC/Interfaces/API/NewInterface/Applications/_Root.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-35.0.2/src/ILCDIRAC/Interfaces/API/NewInterface/Applications/__init__.py` & `ilcdirac-35.0.3/src/ILCDIRAC/Interfaces/API/NewInterface/Applications/__init__.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-35.0.2/src/ILCDIRAC/Interfaces/API/NewInterface/Examples/ConditionalOverlay.py` & `ilcdirac-35.0.3/src/ILCDIRAC/Interfaces/API/NewInterface/Examples/ConditionalOverlay.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-35.0.2/src/ILCDIRAC/Interfaces/API/NewInterface/Examples/FullILDChain.py` & `ilcdirac-35.0.3/src/ILCDIRAC/Interfaces/API/NewInterface/Examples/FullILDChain.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-35.0.2/src/ILCDIRAC/Interfaces/API/NewInterface/Examples/ILDProductionChainDBD.py` & `ilcdirac-35.0.3/src/ILCDIRAC/Interfaces/API/NewInterface/Examples/ILDProductionChainDBD.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-35.0.2/src/ILCDIRAC/Interfaces/API/NewInterface/Examples/ILDProductionChainOpt2017.py` & `ilcdirac-35.0.3/src/ILCDIRAC/Interfaces/API/NewInterface/Examples/ILDProductionChainOpt2017.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-35.0.2/src/ILCDIRAC/Interfaces/API/NewInterface/Examples/MarlinExample.py` & `ilcdirac-35.0.3/src/ILCDIRAC/Interfaces/API/NewInterface/Examples/MarlinExample.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-35.0.2/src/ILCDIRAC/Interfaces/API/NewInterface/Examples/MokkaMarlinOverlayMarlin.py` & `ilcdirac-35.0.3/src/ILCDIRAC/Interfaces/API/NewInterface/Examples/MokkaMarlinOverlayMarlin.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-35.0.2/src/ILCDIRAC/Interfaces/API/NewInterface/Examples/ParametricJobExample.py` & `ilcdirac-35.0.3/src/ILCDIRAC/Interfaces/API/NewInterface/Examples/ParametricJobExample.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-35.0.2/src/ILCDIRAC/Interfaces/API/NewInterface/Examples/ReplicationAkiya.py` & `ilcdirac-35.0.3/src/ILCDIRAC/Interfaces/API/NewInterface/Examples/ReplicationAkiya.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-35.0.2/src/ILCDIRAC/Interfaces/API/NewInterface/Examples/SIDProductionChain.py` & `ilcdirac-35.0.3/src/ILCDIRAC/Interfaces/API/NewInterface/Examples/SIDProductionChain.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-35.0.2/src/ILCDIRAC/Interfaces/API/NewInterface/ILDProductionJobDBD.py` & `ilcdirac-35.0.3/src/ILCDIRAC/Interfaces/API/NewInterface/ILDProductionJobDBD.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-35.0.2/src/ILCDIRAC/Interfaces/API/NewInterface/ILDProductionJobOpt2017.py` & `ilcdirac-35.0.3/src/ILCDIRAC/Interfaces/API/NewInterface/ILDProductionJobOpt2017.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-35.0.2/src/ILCDIRAC/Interfaces/API/NewInterface/Job.py` & `ilcdirac-35.0.3/src/ILCDIRAC/Interfaces/API/NewInterface/Job.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-35.0.2/src/ILCDIRAC/Interfaces/API/NewInterface/LCApplication.py` & `ilcdirac-35.0.3/src/ILCDIRAC/Interfaces/API/NewInterface/LCApplication.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-35.0.2/src/ILCDIRAC/Interfaces/API/NewInterface/LCUtilityApplication.py` & `ilcdirac-35.0.3/src/ILCDIRAC/Interfaces/API/NewInterface/LCUtilityApplication.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-35.0.2/src/ILCDIRAC/Interfaces/API/NewInterface/ProductionJob.py` & `ilcdirac-35.0.3/src/ILCDIRAC/Interfaces/API/NewInterface/ProductionJob.py`

 * *Files 0% similar despite different names*

```diff
@@ -91,14 +91,15 @@
     self.evttype = ''
     self.datatype = ''
     self.energycat = ''
     self.detector = ''
     self.currtrans = None
     self.description = ''
     self.generator = None
+    self.campaign = ''
 
     self.finalpaths = []
     self.finalMetaDict = defaultdict(dict)
     self.prodMetaDict = {}
     self.finalMetaDictNonSearch = {}
     self.metadict_external = {}
     self.specialFinalMetaData = {}
@@ -800,14 +801,15 @@
       self.prodparameters['Generator'] = self.generator
       if self.vo != 'fcc': # for fcc we no longer include the generator inside the file path
         currentPathList.append(self.generator)
         generatorPath = os.path.join(*currentPathList)
         self.finalMetaDict[generatorPath] = {'Generator': self.generator}
 
     if self.vo == 'fcc':
+      self.finalMetaDict[self.basepath] = {"Campaign": str(self.campaign)}
       self.configureFCCOutputPath(path, application, currentPathList)
 
     if self.vo == 'ilc':
       self.configureILCOutputPath(path, application, currentPathList)
 
     res = self._updateProdParameters(application)
     if not res['OK']:
```

### Comparing `iLCDirac-35.0.2/src/ILCDIRAC/Interfaces/API/NewInterface/Productions/CLICProductionChain.py` & `ilcdirac-35.0.3/src/ILCDIRAC/Interfaces/API/NewInterface/Productions/CLICProductionChain.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-35.0.2/src/ILCDIRAC/Interfaces/API/NewInterface/Productions/CLICProductionChain_hzqq_420.py` & `ilcdirac-35.0.3/src/ILCDIRAC/Interfaces/API/NewInterface/Productions/CLICProductionChain_hzqq_420.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-35.0.2/src/ILCDIRAC/Interfaces/API/NewInterface/Productions/ProductionChainTest.py` & `ilcdirac-35.0.3/src/ILCDIRAC/Interfaces/API/NewInterface/Productions/ProductionChainTest.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-35.0.2/src/ILCDIRAC/Interfaces/API/NewInterface/Productions/SIDProductionChain.py` & `ilcdirac-35.0.3/src/ILCDIRAC/Interfaces/API/NewInterface/Productions/SIDProductionChain.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-35.0.2/src/ILCDIRAC/Interfaces/API/NewInterface/SIDProductionJob.py` & `ilcdirac-35.0.3/src/ILCDIRAC/Interfaces/API/NewInterface/SIDProductionJob.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-35.0.2/src/ILCDIRAC/Interfaces/API/NewInterface/Tests/Test_Application.py` & `ilcdirac-35.0.3/src/ILCDIRAC/Interfaces/API/NewInterface/Tests/Test_Application.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-35.0.2/src/ILCDIRAC/Interfaces/API/NewInterface/Tests/Test_Babayaga.py` & `ilcdirac-35.0.3/src/ILCDIRAC/Interfaces/API/NewInterface/Tests/Test_Babayaga.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-35.0.2/src/ILCDIRAC/Interfaces/API/NewInterface/Tests/Test_Bhlumi.py` & `ilcdirac-35.0.3/src/ILCDIRAC/Interfaces/API/NewInterface/Tests/Test_Bhlumi.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-35.0.2/src/ILCDIRAC/Interfaces/API/NewInterface/Tests/Test_Calibration.py` & `ilcdirac-35.0.3/src/ILCDIRAC/Interfaces/API/NewInterface/Tests/Test_Calibration.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-35.0.2/src/ILCDIRAC/Interfaces/API/NewInterface/Tests/Test_CheckCollections.py` & `ilcdirac-35.0.3/src/ILCDIRAC/Interfaces/API/NewInterface/Tests/Test_CheckCollections.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-35.0.2/src/ILCDIRAC/Interfaces/API/NewInterface/Tests/Test_CheckWNs.py` & `ilcdirac-35.0.3/src/ILCDIRAC/Interfaces/API/NewInterface/Tests/Test_CheckWNs.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-35.0.2/src/ILCDIRAC/Interfaces/API/NewInterface/Tests/Test_DDSim.py` & `ilcdirac-35.0.3/src/ILCDIRAC/Interfaces/API/NewInterface/Tests/Test_DDSim.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-35.0.2/src/ILCDIRAC/Interfaces/API/NewInterface/Tests/Test_DelphesApp.py` & `ilcdirac-35.0.3/src/ILCDIRAC/Interfaces/API/NewInterface/Tests/Test_DelphesApp.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-35.0.2/src/ILCDIRAC/Interfaces/API/NewInterface/Tests/Test_Fcc.py` & `ilcdirac-35.0.3/src/ILCDIRAC/Interfaces/API/NewInterface/Tests/Test_Fcc.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-35.0.2/src/ILCDIRAC/Interfaces/API/NewInterface/Tests/Test_GaudiApp.py` & `ilcdirac-35.0.3/src/ILCDIRAC/Interfaces/API/NewInterface/Tests/Test_GaudiApp.py`

 * *Files 0% similar despite different names*

```diff
@@ -356,15 +356,15 @@
     self.assertNotIn('Process', self.gaudi.prodparameters)
 
   def test_checkconsistency_okaysteeringfile(self):
     self.gaudi.version = '134'
     self.gaudi.detectorModel = 'mymodel.det'
     self.gaudi.outputFile = 'myoutput.file'
     self.gaudi._jobtype = 'User'
-    self.gaudi.steeringFile = 'geant_fullsim_fccee_lar_pgun.py'
+    self.gaudi.steeringFile = 'CLDReconstruction.py'
     assertDiracSucceeds(self.gaudi._checkConsistency(Mock()), self)
     self.assertNotIn({'outputFile': '@{OutputFile}', 'outputPath': '@{OutputPath}',
                         'outputDataSE': '@{OutputSE}'}, self.gaudi._listofoutput)
     self.assertNotIn('nbevts', self.gaudi.prodparameters)
     self.assertNotIn('Process', self.gaudi.prodparameters)
 
   @patch("DIRAC.Core.Workflow.Parameter.ParameterCollection.getParametersNames", new=Mock(return_value={"a":1, "b":2, "c":3}))
```

### Comparing `iLCDirac-35.0.2/src/ILCDIRAC/Interfaces/API/NewInterface/Tests/Test_GenericApplication.py` & `ilcdirac-35.0.3/src/ILCDIRAC/Interfaces/API/NewInterface/Tests/Test_GenericApplication.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-35.0.2/src/ILCDIRAC/Interfaces/API/NewInterface/Tests/Test_GetSRMFile.py` & `ilcdirac-35.0.3/src/ILCDIRAC/Interfaces/API/NewInterface/Tests/Test_GetSRMFile.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-35.0.2/src/ILCDIRAC/Interfaces/API/NewInterface/Tests/Test_Job.py` & `ilcdirac-35.0.3/src/ILCDIRAC/Interfaces/API/NewInterface/Tests/Test_Job.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-35.0.2/src/ILCDIRAC/Interfaces/API/NewInterface/Tests/Test_KKMC.py` & `ilcdirac-35.0.3/src/ILCDIRAC/Interfaces/API/NewInterface/Tests/Test_KKMC.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-35.0.2/src/ILCDIRAC/Interfaces/API/NewInterface/Tests/Test_LCSIM.py` & `ilcdirac-35.0.3/src/ILCDIRAC/Interfaces/API/NewInterface/Tests/Test_LCSIM.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-35.0.2/src/ILCDIRAC/Interfaces/API/NewInterface/Tests/Test_Marlin.py` & `ilcdirac-35.0.3/src/ILCDIRAC/Interfaces/API/NewInterface/Tests/Test_Marlin.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-35.0.2/src/ILCDIRAC/Interfaces/API/NewInterface/Tests/Test_Mokka.py` & `ilcdirac-35.0.3/src/ILCDIRAC/Interfaces/API/NewInterface/Tests/Test_Mokka.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-35.0.2/src/ILCDIRAC/Interfaces/API/NewInterface/Tests/Test_OverlayInput.py` & `ilcdirac-35.0.3/src/ILCDIRAC/Interfaces/API/NewInterface/Tests/Test_OverlayInput.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-35.0.2/src/ILCDIRAC/Interfaces/API/NewInterface/Tests/Test_PostGenSelection.py` & `ilcdirac-35.0.3/src/ILCDIRAC/Interfaces/API/NewInterface/Tests/Test_PostGenSelection.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-35.0.2/src/ILCDIRAC/Interfaces/API/NewInterface/Tests/Test_ProductionJob.py` & `ilcdirac-35.0.3/src/ILCDIRAC/Interfaces/API/NewInterface/Tests/Test_ProductionJob.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-35.0.2/src/ILCDIRAC/Interfaces/API/NewInterface/Tests/Test_Pythia.py` & `ilcdirac-35.0.3/src/ILCDIRAC/Interfaces/API/NewInterface/Tests/Test_Pythia.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-35.0.2/src/ILCDIRAC/Interfaces/API/NewInterface/Tests/Test_SLCIOConcatenate.py` & `ilcdirac-35.0.3/src/ILCDIRAC/Interfaces/API/NewInterface/Tests/Test_SLCIOConcatenate.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-35.0.2/src/ILCDIRAC/Interfaces/API/NewInterface/Tests/Test_SLCIOSplit.py` & `ilcdirac-35.0.3/src/ILCDIRAC/Interfaces/API/NewInterface/Tests/Test_SLCIOSplit.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-35.0.2/src/ILCDIRAC/Interfaces/API/NewInterface/Tests/Test_SLIC.py` & `ilcdirac-35.0.3/src/ILCDIRAC/Interfaces/API/NewInterface/Tests/Test_SLIC.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-35.0.2/src/ILCDIRAC/Interfaces/API/NewInterface/Tests/Test_SLICPandora.py` & `ilcdirac-35.0.3/src/ILCDIRAC/Interfaces/API/NewInterface/Tests/Test_SLICPandora.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-35.0.2/src/ILCDIRAC/Interfaces/API/NewInterface/Tests/Test_StdHepSplit.py` & `ilcdirac-35.0.3/src/ILCDIRAC/Interfaces/API/NewInterface/Tests/Test_StdHepSplit.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-35.0.2/src/ILCDIRAC/Interfaces/API/NewInterface/Tests/Test_StdhepCut.py` & `ilcdirac-35.0.3/src/ILCDIRAC/Interfaces/API/NewInterface/Tests/Test_StdhepCut.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-35.0.2/src/ILCDIRAC/Interfaces/API/NewInterface/Tests/Test_Tomato.py` & `ilcdirac-35.0.3/src/ILCDIRAC/Interfaces/API/NewInterface/Tests/Test_Tomato.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-35.0.2/src/ILCDIRAC/Interfaces/API/NewInterface/Tests/Test_UserJob.py` & `ilcdirac-35.0.3/src/ILCDIRAC/Interfaces/API/NewInterface/Tests/Test_UserJob.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-35.0.2/src/ILCDIRAC/Interfaces/API/NewInterface/Tests/Test_Whizard.py` & `ilcdirac-35.0.3/src/ILCDIRAC/Interfaces/API/NewInterface/Tests/Test_Whizard.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-35.0.2/src/ILCDIRAC/Interfaces/API/NewInterface/Tests/Test_Whizard2.py` & `ilcdirac-35.0.3/src/ILCDIRAC/Interfaces/API/NewInterface/Tests/Test_Whizard2.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-35.0.2/src/ILCDIRAC/Interfaces/API/NewInterface/Tests/Test__Root.py` & `ilcdirac-35.0.3/src/ILCDIRAC/Interfaces/API/NewInterface/Tests/Test__Root.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-35.0.2/src/ILCDIRAC/Interfaces/API/NewInterface/Tests/__init__.py` & `ilcdirac-35.0.3/src/ILCDIRAC/Interfaces/API/NewInterface/Tests/__init__.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-35.0.2/src/ILCDIRAC/Interfaces/API/NewInterface/UserJob.py` & `ilcdirac-35.0.3/src/ILCDIRAC/Interfaces/API/NewInterface/UserJob.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-35.0.2/src/ILCDIRAC/Interfaces/API/NewInterface/__init__.py` & `ilcdirac-35.0.3/src/ILCDIRAC/Interfaces/API/NewInterface/__init__.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-35.0.2/src/ILCDIRAC/Interfaces/API/Test/Test_DiracILC.py` & `ilcdirac-35.0.3/src/ILCDIRAC/Interfaces/API/Test/Test_DiracILC.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-35.0.2/src/ILCDIRAC/Interfaces/API/__init__.py` & `ilcdirac-35.0.3/src/ILCDIRAC/Interfaces/API/__init__.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-35.0.2/src/ILCDIRAC/Interfaces/Tests/Test_JobHelpers.py` & `ilcdirac-35.0.3/src/ILCDIRAC/Interfaces/Tests/Test_JobHelpers.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-35.0.2/src/ILCDIRAC/Interfaces/Utilities/DDInterfaceMixin.py` & `ilcdirac-35.0.3/src/ILCDIRAC/Interfaces/Utilities/DDInterfaceMixin.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-35.0.2/src/ILCDIRAC/Interfaces/Utilities/JobHelpers.py` & `ilcdirac-35.0.3/src/ILCDIRAC/Interfaces/Utilities/JobHelpers.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-35.0.2/src/ILCDIRAC/Interfaces/Utilities/SplitMixin.py` & `ilcdirac-35.0.3/src/ILCDIRAC/Interfaces/Utilities/SplitMixin.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-35.0.2/src/ILCDIRAC/Interfaces/Utilities/__init__.py` & `ilcdirac-35.0.3/src/ILCDIRAC/Interfaces/Utilities/__init__.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-35.0.2/src/ILCDIRAC/Interfaces/__init__.py` & `ilcdirac-35.0.3/src/ILCDIRAC/Interfaces/__init__.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-35.0.2/src/ILCDIRAC/Interfaces/scripts/TestAndProbeSites.py` & `ilcdirac-35.0.3/src/ILCDIRAC/Interfaces/scripts/TestAndProbeSites.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-35.0.2/src/ILCDIRAC/Interfaces/scripts/__init__.py` & `ilcdirac-35.0.3/src/ILCDIRAC/Interfaces/scripts/__init__.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-35.0.2/src/ILCDIRAC/Interfaces/scripts/dirac_ilc_find_in_FC.py` & `ilcdirac-35.0.3/src/ILCDIRAC/Interfaces/scripts/dirac_ilc_find_in_FC.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-35.0.2/src/ILCDIRAC/Interfaces/scripts/dirac_ilc_show_software.py` & `ilcdirac-35.0.3/src/ILCDIRAC/Interfaces/scripts/dirac_ilc_show_software.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-35.0.2/src/ILCDIRAC/Interfaces/scripts/dirac_repo_create_lfn_list.py` & `ilcdirac-35.0.3/src/ILCDIRAC/Interfaces/scripts/dirac_repo_create_lfn_list.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-35.0.2/src/ILCDIRAC/Interfaces/scripts/dirac_repo_retrieve_jobs_output.py` & `ilcdirac-35.0.3/src/ILCDIRAC/Interfaces/scripts/dirac_repo_retrieve_jobs_output.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-35.0.2/src/ILCDIRAC/Interfaces/scripts/dirac_repo_retrieve_jobs_output_data.py` & `ilcdirac-35.0.3/src/ILCDIRAC/Interfaces/scripts/dirac_repo_retrieve_jobs_output_data.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-35.0.2/src/ILCDIRAC/Interfaces/scripts/ilcdirac_version.py` & `ilcdirac-35.0.3/src/ILCDIRAC/Interfaces/scripts/ilcdirac_version.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-35.0.2/src/ILCDIRAC/OverlaySystem/Agent/ResetCounters.py` & `ilcdirac-35.0.3/src/ILCDIRAC/OverlaySystem/Agent/ResetCounters.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-35.0.2/src/ILCDIRAC/OverlaySystem/Agent/__init__.py` & `ilcdirac-35.0.3/src/ILCDIRAC/OverlaySystem/Agent/__init__.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-35.0.2/src/ILCDIRAC/OverlaySystem/Client/OverlaySystemClient.py` & `ilcdirac-35.0.3/src/ILCDIRAC/OverlaySystem/Client/OverlaySystemClient.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-35.0.2/src/ILCDIRAC/OverlaySystem/Client/__init__.py` & `ilcdirac-35.0.3/src/ILCDIRAC/OverlaySystem/Client/__init__.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-35.0.2/src/ILCDIRAC/OverlaySystem/DB/OverlayDB.py` & `ilcdirac-35.0.3/src/ILCDIRAC/OverlaySystem/DB/OverlayDB.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-35.0.2/src/ILCDIRAC/OverlaySystem/DB/Test/Test_OverlayDB.py` & `ilcdirac-35.0.3/src/ILCDIRAC/OverlaySystem/DB/Test/Test_OverlayDB.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-35.0.2/src/ILCDIRAC/OverlaySystem/DB/__init__.py` & `ilcdirac-35.0.3/src/ILCDIRAC/OverlaySystem/DB/__init__.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-35.0.2/src/ILCDIRAC/OverlaySystem/Service/OverlayHandler.py` & `ilcdirac-35.0.3/src/ILCDIRAC/OverlaySystem/Service/OverlayHandler.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-35.0.2/src/ILCDIRAC/OverlaySystem/Service/__init__.py` & `ilcdirac-35.0.3/src/ILCDIRAC/OverlaySystem/Service/__init__.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-35.0.2/src/ILCDIRAC/OverlaySystem/__init__.py` & `ilcdirac-35.0.3/src/ILCDIRAC/OverlaySystem/__init__.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-35.0.2/src/ILCDIRAC/Workflow/Modules/AnalyseWN.py` & `ilcdirac-35.0.3/src/ILCDIRAC/Workflow/Modules/AnalyseWN.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-35.0.2/src/ILCDIRAC/Workflow/Modules/ApplicationScript.py` & `ilcdirac-35.0.3/src/ILCDIRAC/Workflow/Modules/ApplicationScript.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-35.0.2/src/ILCDIRAC/Workflow/Modules/BabayagaAnalysis.py` & `ilcdirac-35.0.3/src/ILCDIRAC/Workflow/Modules/BabayagaAnalysis.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-35.0.2/src/ILCDIRAC/Workflow/Modules/BhlumiAnalysis.py` & `ilcdirac-35.0.3/src/ILCDIRAC/Workflow/Modules/BhlumiAnalysis.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-35.0.2/src/ILCDIRAC/Workflow/Modules/Calibration.py` & `ilcdirac-35.0.3/src/ILCDIRAC/Workflow/Modules/Calibration.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-35.0.2/src/ILCDIRAC/Workflow/Modules/CheckCollections.py` & `ilcdirac-35.0.3/src/ILCDIRAC/Workflow/Modules/CheckCollections.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-35.0.2/src/ILCDIRAC/Workflow/Modules/ComputeOutputDataList.py` & `ilcdirac-35.0.3/src/ILCDIRAC/Workflow/Modules/ComputeOutputDataList.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-35.0.2/src/ILCDIRAC/Workflow/Modules/DBDGenRegisterOutputData.py` & `ilcdirac-35.0.3/src/ILCDIRAC/Workflow/Modules/DBDGenRegisterOutputData.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-35.0.2/src/ILCDIRAC/Workflow/Modules/DDSimAnalysis.py` & `ilcdirac-35.0.3/src/ILCDIRAC/Workflow/Modules/DDSimAnalysis.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-35.0.2/src/ILCDIRAC/Workflow/Modules/DelphesAppModule.py` & `ilcdirac-35.0.3/src/ILCDIRAC/Workflow/Modules/DelphesAppModule.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-35.0.2/src/ILCDIRAC/Workflow/Modules/DummyModule.py` & `ilcdirac-35.0.3/src/ILCDIRAC/Workflow/Modules/DummyModule.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-35.0.2/src/ILCDIRAC/Workflow/Modules/FailoverRequest.py` & `ilcdirac-35.0.3/src/ILCDIRAC/Workflow/Modules/FailoverRequest.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-35.0.2/src/ILCDIRAC/Workflow/Modules/FccAnalysis.py` & `ilcdirac-35.0.3/src/ILCDIRAC/Workflow/Modules/FccAnalysis.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-35.0.2/src/ILCDIRAC/Workflow/Modules/GaudiAppModule.py` & `ilcdirac-35.0.3/src/ILCDIRAC/Workflow/Modules/GaudiAppModule.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-35.0.2/src/ILCDIRAC/Workflow/Modules/GetSRMFile.py` & `ilcdirac-35.0.3/src/ILCDIRAC/Workflow/Modules/GetSRMFile.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-35.0.2/src/ILCDIRAC/Workflow/Modules/ILDRegisterOutputData.py` & `ilcdirac-35.0.3/src/ILCDIRAC/Workflow/Modules/ILDRegisterOutputData.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-35.0.2/src/ILCDIRAC/Workflow/Modules/KKMCAnalysis.py` & `ilcdirac-35.0.3/src/ILCDIRAC/Workflow/Modules/KKMCAnalysis.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-35.0.2/src/ILCDIRAC/Workflow/Modules/LCIOConcatenate.py` & `ilcdirac-35.0.3/src/ILCDIRAC/Workflow/Modules/LCIOConcatenate.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-35.0.2/src/ILCDIRAC/Workflow/Modules/LCIOSplit.py` & `ilcdirac-35.0.3/src/ILCDIRAC/Workflow/Modules/LCIOSplit.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-35.0.2/src/ILCDIRAC/Workflow/Modules/LCSIMAnalysis.py` & `ilcdirac-35.0.3/src/ILCDIRAC/Workflow/Modules/LCSIMAnalysis.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-35.0.2/src/ILCDIRAC/Workflow/Modules/MarlinAnalysis.py` & `ilcdirac-35.0.3/src/ILCDIRAC/Workflow/Modules/MarlinAnalysis.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-35.0.2/src/ILCDIRAC/Workflow/Modules/ModuleBase.py` & `ilcdirac-35.0.3/src/ILCDIRAC/Workflow/Modules/ModuleBase.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-35.0.2/src/ILCDIRAC/Workflow/Modules/MokkaAnalysis.py` & `ilcdirac-35.0.3/src/ILCDIRAC/Workflow/Modules/MokkaAnalysis.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-35.0.2/src/ILCDIRAC/Workflow/Modules/MoveInFC.py` & `ilcdirac-35.0.3/src/ILCDIRAC/Workflow/Modules/MoveInFC.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-35.0.2/src/ILCDIRAC/Workflow/Modules/OverlayInput.py` & `ilcdirac-35.0.3/src/ILCDIRAC/Workflow/Modules/OverlayInput.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-35.0.2/src/ILCDIRAC/Workflow/Modules/PostGenSelection.py` & `ilcdirac-35.0.3/src/ILCDIRAC/Workflow/Modules/PostGenSelection.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-35.0.2/src/ILCDIRAC/Workflow/Modules/PythiaAnalysis.py` & `ilcdirac-35.0.3/src/ILCDIRAC/Workflow/Modules/PythiaAnalysis.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-35.0.2/src/ILCDIRAC/Workflow/Modules/RegisterOutputData.py` & `ilcdirac-35.0.3/src/ILCDIRAC/Workflow/Modules/RegisterOutputData.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-35.0.2/src/ILCDIRAC/Workflow/Modules/RemoveInputData.py` & `ilcdirac-35.0.3/src/ILCDIRAC/Workflow/Modules/RemoveInputData.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-35.0.2/src/ILCDIRAC/Workflow/Modules/ReportErrors.py` & `ilcdirac-35.0.3/src/ILCDIRAC/Workflow/Modules/ReportErrors.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-35.0.2/src/ILCDIRAC/Workflow/Modules/RootExecutableAnalysis.py` & `ilcdirac-35.0.3/src/ILCDIRAC/Workflow/Modules/RootExecutableAnalysis.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-35.0.2/src/ILCDIRAC/Workflow/Modules/RootMacroAnalysis.py` & `ilcdirac-35.0.3/src/ILCDIRAC/Workflow/Modules/RootMacroAnalysis.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-35.0.2/src/ILCDIRAC/Workflow/Modules/SIDRegisterOutputData.py` & `ilcdirac-35.0.3/src/ILCDIRAC/Workflow/Modules/SIDRegisterOutputData.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-35.0.2/src/ILCDIRAC/Workflow/Modules/SLICAnalysis.py` & `ilcdirac-35.0.3/src/ILCDIRAC/Workflow/Modules/SLICAnalysis.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-35.0.2/src/ILCDIRAC/Workflow/Modules/SLICPandoraAnalysis.py` & `ilcdirac-35.0.3/src/ILCDIRAC/Workflow/Modules/SLICPandoraAnalysis.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-35.0.2/src/ILCDIRAC/Workflow/Modules/StdHepConverter.py` & `ilcdirac-35.0.3/src/ILCDIRAC/Workflow/Modules/StdHepConverter.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-35.0.2/src/ILCDIRAC/Workflow/Modules/StdHepCut.py` & `ilcdirac-35.0.3/src/ILCDIRAC/Workflow/Modules/StdHepCut.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-35.0.2/src/ILCDIRAC/Workflow/Modules/StdHepCutJava.py` & `ilcdirac-35.0.3/src/ILCDIRAC/Workflow/Modules/StdHepCutJava.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-35.0.2/src/ILCDIRAC/Workflow/Modules/StdHepSplit.py` & `ilcdirac-35.0.3/src/ILCDIRAC/Workflow/Modules/StdHepSplit.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-35.0.2/src/ILCDIRAC/Workflow/Modules/Test/MakeRequest.py` & `ilcdirac-35.0.3/src/ILCDIRAC/Workflow/Modules/Test/MakeRequest.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-35.0.2/src/ILCDIRAC/Workflow/Modules/Test/Test_BabayagaAnalysis.py` & `ilcdirac-35.0.3/src/ILCDIRAC/Workflow/Modules/Test/Test_BabayagaAnalysis.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-35.0.2/src/ILCDIRAC/Workflow/Modules/Test/Test_BhlumiAnalysis.py` & `ilcdirac-35.0.3/src/ILCDIRAC/Workflow/Modules/Test/Test_BhlumiAnalysis.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-35.0.2/src/ILCDIRAC/Workflow/Modules/Test/Test_Calibration.py` & `ilcdirac-35.0.3/src/ILCDIRAC/Workflow/Modules/Test/Test_Calibration.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-35.0.2/src/ILCDIRAC/Workflow/Modules/Test/Test_DDSimWorkflow.py` & `ilcdirac-35.0.3/src/ILCDIRAC/Workflow/Modules/Test/Test_DDSimWorkflow.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-35.0.2/src/ILCDIRAC/Workflow/Modules/Test/Test_DelphesAppModule.py` & `ilcdirac-35.0.3/src/ILCDIRAC/Workflow/Modules/Test/Test_DelphesAppModule.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-35.0.2/src/ILCDIRAC/Workflow/Modules/Test/Test_FccAnalysis.py` & `ilcdirac-35.0.3/src/ILCDIRAC/Workflow/Modules/Test/Test_FccAnalysis.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-35.0.2/src/ILCDIRAC/Workflow/Modules/Test/Test_GaudiAppModule.py` & `ilcdirac-35.0.3/src/ILCDIRAC/Workflow/Modules/Test/Test_GaudiAppModule.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-35.0.2/src/ILCDIRAC/Workflow/Modules/Test/Test_KKMCAnalysis.py` & `ilcdirac-35.0.3/src/ILCDIRAC/Workflow/Modules/Test/Test_KKMCAnalysis.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-35.0.2/src/ILCDIRAC/Workflow/Modules/Test/Test_MarlinAnalysis.py` & `ilcdirac-35.0.3/src/ILCDIRAC/Workflow/Modules/Test/Test_MarlinAnalysis.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-35.0.2/src/ILCDIRAC/Workflow/Modules/Test/Test_ModuleBase.py` & `ilcdirac-35.0.3/src/ILCDIRAC/Workflow/Modules/Test/Test_ModuleBase.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-35.0.2/src/ILCDIRAC/Workflow/Modules/Test/Test_OverlayInput.py` & `ilcdirac-35.0.3/src/ILCDIRAC/Workflow/Modules/Test/Test_OverlayInput.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-35.0.2/src/ILCDIRAC/Workflow/Modules/Test/Test_RegisterOutputData.py` & `ilcdirac-35.0.3/src/ILCDIRAC/Workflow/Modules/Test/Test_RegisterOutputData.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-35.0.2/src/ILCDIRAC/Workflow/Modules/Test/Test_ReportErrors.py` & `ilcdirac-35.0.3/src/ILCDIRAC/Workflow/Modules/Test/Test_ReportErrors.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-35.0.2/src/ILCDIRAC/Workflow/Modules/Test/Test_RootExecutableAnalysis.py` & `ilcdirac-35.0.3/src/ILCDIRAC/Workflow/Modules/Test/Test_RootExecutableAnalysis.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-35.0.2/src/ILCDIRAC/Workflow/Modules/Test/Test_SLICPandoraAnalysis.py` & `ilcdirac-35.0.3/src/ILCDIRAC/Workflow/Modules/Test/Test_SLICPandoraAnalysis.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-35.0.2/src/ILCDIRAC/Workflow/Modules/Test/Test_SlicPandora.py` & `ilcdirac-35.0.3/src/ILCDIRAC/Workflow/Modules/Test/Test_SlicPandora.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-35.0.2/src/ILCDIRAC/Workflow/Modules/Test/Test_StdHepCut.py` & `ilcdirac-35.0.3/src/ILCDIRAC/Workflow/Modules/Test/Test_StdHepCut.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-35.0.2/src/ILCDIRAC/Workflow/Modules/Test/Test_StdHepSplit.py` & `ilcdirac-35.0.3/src/ILCDIRAC/Workflow/Modules/Test/Test_StdHepSplit.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-35.0.2/src/ILCDIRAC/Workflow/Modules/Test/Test_UploadLogFile.py` & `ilcdirac-35.0.3/src/ILCDIRAC/Workflow/Modules/Test/Test_UploadLogFile.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-35.0.2/src/ILCDIRAC/Workflow/Modules/Test/Test_UploadOutputData.py` & `ilcdirac-35.0.3/src/ILCDIRAC/Workflow/Modules/Test/Test_UploadOutputData.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-35.0.2/src/ILCDIRAC/Workflow/Modules/Test/Test_UserJobFinalization.py` & `ilcdirac-35.0.3/src/ILCDIRAC/Workflow/Modules/Test/Test_UserJobFinalization.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-35.0.2/src/ILCDIRAC/Workflow/Modules/Test/Test_Whizard2Workflow.py` & `ilcdirac-35.0.3/src/ILCDIRAC/Workflow/Modules/Test/Test_Whizard2Workflow.py`

 * *Files 10% similar despite different names*

```diff
@@ -94,15 +94,16 @@
   @patch("%s.getEnvironmentScript" % MODULE_NAME, new=Mock(return_value=S_OK("setup.sh")))
   @patch("%s.shellCall" % MODULE_NAME, new=Mock(return_value=S_OK((0, "AllGood"))))
   def test_Whizard2_runIt_success(self):
     """Whizard2.runit ................................................................................."""
     self.whiz.platform = 'Windows'
     self.whiz.applicationLog = self.logFileName
     # side effect for Script, userlibs, log, logAfter
-    with patch("os.path.exists", new=Mock(side_effect=[False, False, False, True])):
+    with patch("os.path.exists", new=Mock(side_effect=[False, False, False, True])),\
+      patch.object(self.whiz, "_analyseTheLog", new=Mock(return_value=S_OK())):
       res = self.whiz.runIt()
     print(res)
     assertDiracSucceeds(res, self)
 
   @patch("%s.getEnvironmentScript" % MODULE_NAME, new=Mock(return_value=S_OK("setup.sh")))
   @patch("%s.shellCall" % MODULE_NAME, new=Mock(return_value=S_OK((0, "AllGood"))))
   def test_Whizard2_runIt_failure_LogFile(self):
@@ -179,15 +180,16 @@
   def test_Whizard2_runIt_success_sinFile(self, pName, pValue, pExpected, pUnExpected=None):
     """Whizard.runit success with steeringFile........................................................."""
     self.whiz.platform = "Windows"
     self.whiz.applicationLog = self.logFileName
     self.whiz.whizard2SinFile = "whizard instructions"
     setattr(self.whiz, pName, pValue)
     # side effect for Steering1, Steering2, Script, userlib, log, logAfter
-    with patch("os.path.exists", new=Mock(side_effect=[False, False, False, True])):
+    with patch("os.path.exists", new=Mock(side_effect=[False, False, False, True])), \
+      patch.object(self.whiz, "_analyseTheLog", new=Mock(return_value=S_OK())):
       res = self.whiz.runIt()
     assertDiracSucceeds(res, self)
     self.assertEqual(self.whiz.whizard2SinFile, "whizard instructions")
     self.assertIn("whizard instructions", open("Whizard2__Steer_.sin").read())
     if not pUnExpected:
       self.assertIn(pExpected, open("Whizard2__Steer_.sin").read())
     else:
@@ -233,14 +235,23 @@
     gLogger.setLevel("ERROR")
     self.whiz.workflow_commons = dict(IS_PROD=True, PRODUCTION_ID=6666, JOB_ID=123)
     self.whiz.OutputFile = 'events.stdhep'
     self.whiz.resolveInputVariables()
     self.whiz.applicationSpecificInputs()
     self.assertEqual(self.whiz.randomSeed, 6666123)
 
+  def test_Whizard2_ASI_RandomSeedchange_Prod(self):
+    """Whizard.applicationSpecificInputs: check changing of randomseed in production..................."""
+    gLogger.setLevel("ERROR")
+    self.whiz.workflow_commons = dict(IS_PROD=True, PRODUCTION_ID=0, JOB_ID=12345 + 4294967295)
+    self.whiz.OutputFile = 'events.stdhep'
+    self.whiz.resolveInputVariables()
+    self.whiz.applicationSpecificInputs()
+    self.assertEqual(self.whiz.randomSeed, 12345)
+
   @patch.dict(os.environ, {"JOBID": "12345"})
   def test_Whizard2_ASI_RandomSeed_Set(self):
     """Whizard.applicationSpecificInputs: check setting of default randomseed in user jobs............"""
     gLogger.setLevel("ERROR")
     self.whiz = Whizard2Analysis()
     self.whiz.workflow_commons = dict()
     self.whiz.resolveInputVariables()
@@ -295,14 +306,34 @@
     pathMock.path.join = os.path.join
     pathMock.path.exists.return_value = localFile
     with patch('%s.os' % MODULE_NAME, new=pathMock), \
          patch('%s.extractTarball' % MODULE_NAME, return_value=S_OK()):
       ret = self.whiz.resolveIntegratedProcess()
     self.assertEqual(ret['OK'], success)
 
+  strings = ["corr. to luminosity [fb-1] =   1.2792E+02", """|-----------------------------------------------------------------------------|
+  17      69993  7.8172284E-02  1.32E-04    0.17    0.45   19.12    0.41   7
+|=============================================================================|""", "Events: actual unweighting efficiency =  15.15 %"]
+  @parameterized.expand([(True, "", strings[0] + strings[1] + strings[2], False),
+                        (True, "", strings[0] + strings[1] + strings[2], True),
+                        (False, "luminosity not found", strings[1] + strings[2], False),
+                        (False, "cross section not found", strings[0] + strings[2], False),
+                        (False, "efficiency not found", strings[0] + strings[1], False),
+                       ])
+  def test_Whizard2__analyseTheLog(self, success, error, applog, info):
+    """Whizard._analyseTheLog;......................................................................."""
+    self.whiz.applicationLog = ""
+    if info:
+      self.whiz.workflow_commons = {'Info': {}}
+    with patch('%s.open' % MODULE_NAME, mock_open(read_data=applog), create=True):
+      res = self.whiz._analyseTheLog()
+    if success:
+      assertDiracSucceeds(res, self)
+    else:
+      self.assertIn(error, res['Message'])
 
 def runTests():
   """Runs our tests."""
   suite = unittest.defaultTestLoader.loadTestsFromTestCase(TestWhizard2Analysis)
   suite.addTest(unittest.defaultTestLoader.loadTestsFromTestCase(TestWhizard2AnalysisRunit))
   suite.addTest(unittest.defaultTestLoader.loadTestsFromTestCase(TestWhizard2AnalysisASI))
   testResult = unittest.TextTestRunner(verbosity=2).run(suite)
```

### Comparing `iLCDirac-35.0.2/src/ILCDIRAC/Workflow/Modules/Test/Test_WhizardAnalysis.py` & `ilcdirac-35.0.3/src/ILCDIRAC/Workflow/Modules/Test/Test_WhizardAnalysis.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-35.0.2/src/ILCDIRAC/Workflow/Modules/Test/Test_WorkflowModuleRequests.py` & `ilcdirac-35.0.3/src/ILCDIRAC/Workflow/Modules/Test/Test_WorkflowModuleRequests.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-35.0.2/src/ILCDIRAC/Workflow/Modules/TomatoAnalysis.py` & `ilcdirac-35.0.3/src/ILCDIRAC/Workflow/Modules/TomatoAnalysis.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-35.0.2/src/ILCDIRAC/Workflow/Modules/UploadLogFile.py` & `ilcdirac-35.0.3/src/ILCDIRAC/Workflow/Modules/UploadLogFile.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-35.0.2/src/ILCDIRAC/Workflow/Modules/UploadOutputData.py` & `ilcdirac-35.0.3/src/ILCDIRAC/Workflow/Modules/UploadOutputData.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-35.0.2/src/ILCDIRAC/Workflow/Modules/UserJobFinalization.py` & `ilcdirac-35.0.3/src/ILCDIRAC/Workflow/Modules/UserJobFinalization.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-35.0.2/src/ILCDIRAC/Workflow/Modules/WhizardAnalysis.py` & `ilcdirac-35.0.3/src/ILCDIRAC/Workflow/Modules/WhizardAnalysis.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-35.0.2/src/ILCDIRAC/Workflow/Modules/__init__.py` & `ilcdirac-35.0.3/src/ILCDIRAC/Workflow/Modules/__init__.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-35.0.2/src/ILCDIRAC/Workflow/Utilities/CompactMixin.py` & `ilcdirac-35.0.3/src/ILCDIRAC/Workflow/Utilities/CompactMixin.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-35.0.2/src/ILCDIRAC/Workflow/Utilities/DD4hepMixin.py` & `ilcdirac-35.0.3/src/ILCDIRAC/Workflow/Utilities/DD4hepMixin.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-35.0.2/src/ILCDIRAC/Workflow/Utilities/RootMixin.py` & `ilcdirac-35.0.3/src/ILCDIRAC/Workflow/Utilities/RootMixin.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-35.0.2/src/ILCDIRAC/Workflow/Utilities/__init__.py` & `ilcdirac-35.0.3/src/ILCDIRAC/Workflow/Utilities/__init__.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-35.0.2/src/ILCDIRAC/Workflow/__init__.py` & `ilcdirac-35.0.3/src/ILCDIRAC/Workflow/__init__.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-35.0.2/src/ILCDIRAC/WorkloadManagementSystem/Agent/JobResetAgent.py` & `ilcdirac-35.0.3/src/ILCDIRAC/WorkloadManagementSystem/Agent/JobResetAgent.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-35.0.2/src/ILCDIRAC/WorkloadManagementSystem/Agent/__init__.py` & `ilcdirac-35.0.3/src/ILCDIRAC/WorkloadManagementSystem/Agent/__init__.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-35.0.2/src/ILCDIRAC/WorkloadManagementSystem/Client/DownloadInputData.py` & `ilcdirac-35.0.3/src/ILCDIRAC/WorkloadManagementSystem/Client/DownloadInputData.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-35.0.2/src/ILCDIRAC/WorkloadManagementSystem/Client/__init__.py` & `ilcdirac-35.0.3/src/ILCDIRAC/WorkloadManagementSystem/Client/__init__.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-35.0.2/src/ILCDIRAC/WorkloadManagementSystem/Executor/SoftwareVersions.py` & `ilcdirac-35.0.3/src/ILCDIRAC/WorkloadManagementSystem/Executor/SoftwareVersions.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-35.0.2/src/ILCDIRAC/WorkloadManagementSystem/Executor/__init__.py` & `ilcdirac-35.0.3/src/ILCDIRAC/WorkloadManagementSystem/Executor/__init__.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-35.0.2/src/ILCDIRAC/WorkloadManagementSystem/Tests/Test_Client_DownloadInputData.py` & `ilcdirac-35.0.3/src/ILCDIRAC/WorkloadManagementSystem/Tests/Test_Client_DownloadInputData.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-35.0.2/src/ILCDIRAC/WorkloadManagementSystem/Tests/Test_JobResetAgent.py` & `ilcdirac-35.0.3/src/ILCDIRAC/WorkloadManagementSystem/Tests/Test_JobResetAgent.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-35.0.2/src/ILCDIRAC/WorkloadManagementSystem/Tests/Test_SoftwareVersions.py` & `ilcdirac-35.0.3/src/ILCDIRAC/WorkloadManagementSystem/Tests/Test_SoftwareVersions.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-35.0.2/src/ILCDIRAC/WorkloadManagementSystem/__init__.py` & `ilcdirac-35.0.3/src/ILCDIRAC/WorkloadManagementSystem/__init__.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-35.0.2/src/ILCDIRAC/__init__.py` & `ilcdirac-35.0.3/src/ILCDIRAC/__init__.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-35.0.2/src/iLCDirac.egg-info/PKG-INFO` & `ilcdirac-35.0.3/src/iLCDirac.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: iLCDirac
-Version: 35.0.2
+Version: 35.0.3
 Summary: iLCDirac is the iLC/CLIC/FCC extension of DIRAC
 Home-page: https://gitlab.cern.ch/clicdp/ilcdirac/ilcdirac.git
 Maintainer: Andre Sailer
 Maintainer-email: ilcdirac-support@cern.ch
 License: GPL-3.0-only
 Project-URL: Bug Tracker, https://its.cern.ch/jira/browse/ILCDIRAC
 Project-URL: Documentation, https://ilcdirac-doc.web.cern.ch/
@@ -13,15 +13,15 @@
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Topic :: Scientific/Engineering
 Classifier: Topic :: System :: Distributed Computing
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
-Requires-Dist: DIRAC~=8.0
+Requires-Dist: DIRAC>=8.0.41
 Requires-Dist: requests
 Requires-Dist: six
 Provides-Extra: server
 Requires-Dist: DIRAC[server]; extra == "server"
 Requires-Dist: psutil; extra == "server"
 Requires-Dist: suds-jurko; extra == "server"
 Provides-Extra: testing
```

### Comparing `iLCDirac-35.0.2/src/iLCDirac.egg-info/SOURCES.txt` & `ilcdirac-35.0.3/src/iLCDirac.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `iLCDirac-35.0.2/src/iLCDirac.egg-info/entry_points.txt` & `ilcdirac-35.0.3/src/iLCDirac.egg-info/entry_points.txt`

 * *Files identical despite different names*

