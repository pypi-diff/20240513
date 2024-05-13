# Comparing `tmp/steam-sdk-2024.5.1.tar.gz` & `tmp/steam-sdk-2024.5.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "steam-sdk-2024.5.1.tar", last modified: Mon May 13 09:44:36 2024, max compression
+gzip compressed data, was "steam-sdk-2024.5.2.tar", last modified: Mon May 13 10:13:26 2024, max compression
```

## Comparing `steam-sdk-2024.5.1.tar` & `steam-sdk-2024.5.2.tar`

### file list

```diff
@@ -1,216 +1,216 @@
-drwxrwxrwx   0        0        0        0 2024-05-13 09:44:36.457732 steam-sdk-2024.5.1/
--rw-rw-rw-   0        0        0      264 2023-06-07 14:48:24.000000 steam-sdk-2024.5.1/MANIFEST.in
--rw-rw-rw-   0        0        0     5753 2024-05-13 09:44:36.452731 steam-sdk-2024.5.1/PKG-INFO
--rw-rw-rw-   0        0        0       42 2024-05-13 09:44:36.457732 steam-sdk-2024.5.1/setup.cfg
--rw-rw-rw-   0        0        0     1668 2024-05-13 09:41:29.000000 steam-sdk-2024.5.1/setup.py
-drwxrwxrwx   0        0        0        0 2024-05-13 09:44:34.761264 steam-sdk-2024.5.1/steam_sdk/
--rw-rw-rw-   0        0        0        0 2022-02-23 07:50:41.000000 steam-sdk-2024.5.1/steam_sdk/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-13 09:44:34.826025 steam-sdk-2024.5.1/steam_sdk/analyses/
--rw-rw-rw-   0        0        0    37589 2024-04-19 11:58:44.000000 steam-sdk-2024.5.1/steam_sdk/analyses/AnalysisEvent.py
--rw-rw-rw-   0        0        0    30954 2024-04-26 11:34:23.000000 steam-sdk-2024.5.1/steam_sdk/analyses/AnalysisEventLHC.py
--rw-rw-rw-   0        0        0   135646 2024-05-13 09:25:29.000000 steam-sdk-2024.5.1/steam_sdk/analyses/AnalysisSTEAM.py
--rw-rw-rw-   0        0        0        0 2022-02-23 07:50:41.000000 steam-sdk-2024.5.1/steam_sdk/analyses/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-13 09:44:34.828025 steam-sdk-2024.5.1/steam_sdk/analyses/custom_analyses/
--rw-rw-rw-   0        0        0        0 2022-02-23 07:50:41.000000 steam-sdk-2024.5.1/steam_sdk/analyses/custom_analyses/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-13 09:44:34.845026 steam-sdk-2024.5.1/steam_sdk/analyses/custom_analyses/analysis_short_circuit_LEDET_1/
--rw-rw-rw-   0        0        0        0 2022-02-23 07:50:41.000000 steam-sdk-2024.5.1/steam_sdk/analyses/custom_analyses/analysis_short_circuit_LEDET_1/__init__.py
--rw-rw-rw-   0        0        0    23388 2024-01-12 14:29:22.000000 steam-sdk-2024.5.1/steam_sdk/analyses/custom_analyses/analysis_short_circuit_LEDET_1/analysis_short_circuit_LEDET_1.py
-drwxrwxrwx   0        0        0        0 2024-05-13 09:44:34.926555 steam-sdk-2024.5.1/steam_sdk/analyses/custom_analyses/analysis_short_circuit_LEDET_1/utils/
--rw-rw-rw-   0        0        0        0 2022-02-23 07:50:41.000000 steam-sdk-2024.5.1/steam_sdk/analyses/custom_analyses/analysis_short_circuit_LEDET_1/utils/__init__.py
--rw-rw-rw-   0        0        0    16777 2024-01-12 14:32:10.000000 steam-sdk-2024.5.1/steam_sdk/analyses/custom_analyses/analysis_short_circuit_LEDET_1/utils/calculate_short_parameters.py
--rw-rw-rw-   0        0        0     2820 2024-01-12 14:32:10.000000 steam-sdk-2024.5.1/steam_sdk/analyses/custom_analyses/analysis_short_circuit_LEDET_1/utils/copy_input_files.py
--rw-rw-rw-   0        0        0     6761 2024-01-12 14:32:10.000000 steam-sdk-2024.5.1/steam_sdk/analyses/custom_analyses/analysis_short_circuit_LEDET_1/utils/set_common_parameters.py
--rw-rw-rw-   0        0        0    95432 2024-01-12 14:32:10.000000 steam-sdk-2024.5.1/steam_sdk/analyses/custom_analyses/analysis_short_circuit_LEDET_1/utils/set_magnet_specific_parameters.py
--rw-rw-rw-   0        0        0     2672 2024-01-12 14:32:10.000000 steam-sdk-2024.5.1/steam_sdk/analyses/custom_analyses/analysis_short_circuit_LEDET_1/utils/set_short_circuit_analysis_parameters.py
--rw-rw-rw-   0        0        0     2361 2024-01-12 14:29:35.000000 steam-sdk-2024.5.1/steam_sdk/analyses/custom_analyses/analysis_short_circuit_LEDET_1/utils/set_simulations_to_prepare_run.py
-drwxrwxrwx   0        0        0        0 2024-05-13 09:44:34.943653 steam-sdk-2024.5.1/steam_sdk/analyses/custom_analyses/co_simulation_QH_PyBBQ_LEDET_1/
--rw-rw-rw-   0        0        0        0 2022-02-23 07:50:41.000000 steam-sdk-2024.5.1/steam_sdk/analyses/custom_analyses/co_simulation_QH_PyBBQ_LEDET_1/__init__.py
--rw-rw-rw-   0        0        0    22357 2024-03-11 05:39:28.000000 steam-sdk-2024.5.1/steam_sdk/analyses/custom_analyses/co_simulation_QH_PyBBQ_LEDET_1/co_simulation_QH_PyBBQ_LEDET_1.py
-drwxrwxrwx   0        0        0        0 2024-05-13 09:44:34.978855 steam-sdk-2024.5.1/steam_sdk/analyses/custom_analyses/co_simulation_QH_PyBBQ_LEDET_1/utils/
--rw-rw-rw-   0        0        0        0 2022-09-26 06:59:06.000000 steam-sdk-2024.5.1/steam_sdk/analyses/custom_analyses/co_simulation_QH_PyBBQ_LEDET_1/utils/__init__.py
--rw-rw-rw-   0        0        0     5330 2024-01-12 14:32:10.000000 steam-sdk-2024.5.1/steam_sdk/analyses/custom_analyses/co_simulation_QH_PyBBQ_LEDET_1/utils/calculate_quench_propagation_velocity.py
--rw-rw-rw-   0        0        0     4450 2024-01-12 14:32:10.000000 steam-sdk-2024.5.1/steam_sdk/analyses/custom_analyses/co_simulation_QH_PyBBQ_LEDET_1/utils/create_conductor_analysis_file.py
--rw-rw-rw-   0        0        0     2844 2024-01-12 14:32:10.000000 steam-sdk-2024.5.1/steam_sdk/analyses/custom_analyses/co_simulation_QH_PyBBQ_LEDET_1/utils/create_magnet_analysis_file.py
-drwxrwxrwx   0        0        0        0 2024-05-13 09:44:34.996963 steam-sdk-2024.5.1/steam_sdk/analyses/custom_analyses/co_simulation_QH_PyBBQ_LEDET_MBRD_validation_1/
--rw-rw-rw-   0        0        0        0 2022-09-26 06:59:06.000000 steam-sdk-2024.5.1/steam_sdk/analyses/custom_analyses/co_simulation_QH_PyBBQ_LEDET_MBRD_validation_1/__init__.py
--rw-rw-rw-   0        0        0    29436 2024-03-11 05:39:28.000000 steam-sdk-2024.5.1/steam_sdk/analyses/custom_analyses/co_simulation_QH_PyBBQ_LEDET_MBRD_validation_1/co_simulation_QH_PyBBQ_LEDET_MBRD_validation_1.py
-drwxrwxrwx   0        0        0        0 2024-05-13 09:44:35.024223 steam-sdk-2024.5.1/steam_sdk/analyses/custom_analyses/co_simulation_QH_PyBBQ_LEDET_MBRD_validation_1/utils/
--rw-rw-rw-   0        0        0        0 2022-09-26 06:59:06.000000 steam-sdk-2024.5.1/steam_sdk/analyses/custom_analyses/co_simulation_QH_PyBBQ_LEDET_MBRD_validation_1/utils/__init__.py
--rw-rw-rw-   0        0        0     5330 2024-01-12 14:32:09.000000 steam-sdk-2024.5.1/steam_sdk/analyses/custom_analyses/co_simulation_QH_PyBBQ_LEDET_MBRD_validation_1/utils/calculate_quench_propagation_velocity.py
--rw-rw-rw-   0        0        0     4627 2024-01-12 14:32:10.000000 steam-sdk-2024.5.1/steam_sdk/analyses/custom_analyses/co_simulation_QH_PyBBQ_LEDET_MBRD_validation_1/utils/create_conductor_analysis_file.py
--rw-rw-rw-   0        0        0     4775 2024-01-12 14:32:10.000000 steam-sdk-2024.5.1/steam_sdk/analyses/custom_analyses/co_simulation_QH_PyBBQ_LEDET_MBRD_validation_1/utils/create_magnet_analysis_file.py
-drwxrwxrwx   0        0        0        0 2024-05-13 09:44:35.036318 steam-sdk-2024.5.1/steam_sdk/analyses/custom_analyses/custom_function_test_1/
--rw-rw-rw-   0        0        0        0 2022-02-23 07:50:41.000000 steam-sdk-2024.5.1/steam_sdk/analyses/custom_analyses/custom_function_test_1/__init__.py
--rw-rw-rw-   0        0        0     1307 2022-09-10 00:27:54.000000 steam-sdk-2024.5.1/steam_sdk/analyses/custom_analyses/custom_function_test_1/custom_function_test_1.py
-drwxrwxrwx   0        0        0        0 2024-05-13 09:44:35.170647 steam-sdk-2024.5.1/steam_sdk/builders/
--rw-rw-rw-   0        0        0    13175 2024-03-13 09:34:54.000000 steam-sdk-2024.5.1/steam_sdk/builders/BuilderAPDL_CT.py
--rw-rw-rw-   0        0        0     4805 2024-03-22 08:53:57.000000 steam-sdk-2024.5.1/steam_sdk/builders/BuilderCosim.py
--rw-rw-rw-   0        0        0    17741 2024-02-07 15:54:14.000000 steam-sdk-2024.5.1/steam_sdk/builders/BuilderFiQuS.py
--rw-rw-rw-   0        0        0   160440 2024-04-17 14:10:37.000000 steam-sdk-2024.5.1/steam_sdk/builders/BuilderLEDET.py
--rw-rw-rw-   0        0        0    53471 2024-05-08 10:36:11.000000 steam-sdk-2024.5.1/steam_sdk/builders/BuilderModel.py
--rw-rw-rw-   0        0        0    12686 2024-03-13 11:10:16.000000 steam-sdk-2024.5.1/steam_sdk/builders/BuilderProteCCT.py
--rw-rw-rw-   0        0        0     6749 2022-08-22 11:29:04.000000 steam-sdk-2024.5.1/steam_sdk/builders/BuilderPyBBQ.py
--rw-rw-rw-   0        0        0    12487 2024-04-11 22:26:08.000000 steam-sdk-2024.5.1/steam_sdk/builders/BuilderPySIGMA.py
--rw-rw-rw-   0        0        0    57747 2024-05-07 07:59:18.000000 steam-sdk-2024.5.1/steam_sdk/builders/BuilderTFM.py
--rw-rw-rw-   0        0        0    11689 2023-01-18 09:46:00.000000 steam-sdk-2024.5.1/steam_sdk/builders/SelfMutualInductanceCalculation.py
--rw-rw-rw-   0        0        0     7941 2022-12-06 11:41:34.000000 steam-sdk-2024.5.1/steam_sdk/builders/Solenoids.py
--rw-rw-rw-   0        0        0        0 2022-02-23 07:50:41.000000 steam-sdk-2024.5.1/steam_sdk/builders/__init__.py
--rw-rw-rw-   0        0        0     8352 2023-02-02 15:39:34.000000 steam-sdk-2024.5.1/steam_sdk/builders/geometricFunctions.py
-drwxrwxrwx   0        0        0        0 2024-05-13 09:44:35.171647 steam-sdk-2024.5.1/steam_sdk/configs/
--rw-rw-rw-   0        0        0        0 2022-02-23 07:50:41.000000 steam-sdk-2024.5.1/steam_sdk/configs/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-13 09:44:35.192266 steam-sdk-2024.5.1/steam_sdk/configs/tools_defaults/
-drwxrwxrwx   0        0        0        0 2024-05-13 09:44:35.194279 steam-sdk-2024.5.1/steam_sdk/configs/tools_defaults/LEDET/
--rw-rw-rw-   0        0        0        0 2022-02-23 07:50:41.000000 steam-sdk-2024.5.1/steam_sdk/configs/tools_defaults/LEDET/__init__.py
--rw-rw-rw-   0        0        0     1426 2022-02-23 07:50:41.000000 steam-sdk-2024.5.1/steam_sdk/configs/tools_defaults/ToolDefaultReader.py
--rw-rw-rw-   0        0        0        0 2022-02-23 07:50:41.000000 steam-sdk-2024.5.1/steam_sdk/configs/tools_defaults/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-13 09:44:35.197267 steam-sdk-2024.5.1/steam_sdk/cosims/
--rw-rw-rw-   0        0        0    26984 2024-04-29 06:28:52.000000 steam-sdk-2024.5.1/steam_sdk/cosims/CoSimPyCoSim.py
--rw-rw-rw-   0        0        0        0 2022-02-23 07:50:41.000000 steam-sdk-2024.5.1/steam_sdk/cosims/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-13 09:44:35.534129 steam-sdk-2024.5.1/steam_sdk/data/
--rw-rw-rw-   0        0        0     1684 2024-03-21 12:23:41.000000 steam-sdk-2024.5.1/steam_sdk/data/DataAPDLCTOptions.py
--rw-rw-rw-   0        0        0    13001 2024-05-08 10:18:52.000000 steam-sdk-2024.5.1/steam_sdk/data/DataAnalysis.py
--rw-rw-rw-   0        0        0      414 2024-03-06 09:01:34.000000 steam-sdk-2024.5.1/steam_sdk/data/DataCoSim.py
--rw-rw-rw-   0        0        0     9303 2024-04-08 06:18:59.000000 steam-sdk-2024.5.1/steam_sdk/data/DataConductor.py
--rw-rw-rw-   0        0        0      308 2024-04-19 11:58:44.000000 steam-sdk-2024.5.1/steam_sdk/data/DataDakota.py
--rw-rw-rw-   0        0        0     2987 2024-03-21 12:23:41.000000 steam-sdk-2024.5.1/steam_sdk/data/DataEventCircuit.py
--rw-rw-rw-   0        0        0     4636 2024-03-21 12:23:41.000000 steam-sdk-2024.5.1/steam_sdk/data/DataEventMagnet.py
--rw-rw-rw-   0        0        0    87484 2024-05-13 08:12:26.000000 steam-sdk-2024.5.1/steam_sdk/data/DataFiQuS.py
--rw-rw-rw-   0        0        0     7309 2024-03-21 12:23:41.000000 steam-sdk-2024.5.1/steam_sdk/data/DataFiQuSOptions.py
--rw-rw-rw-   0        0        0    16769 2024-04-08 06:18:59.000000 steam-sdk-2024.5.1/steam_sdk/data/DataLEDET.py
--rw-rw-rw-   0        0        0     9528 2024-03-21 12:23:41.000000 steam-sdk-2024.5.1/steam_sdk/data/DataLEDETOptions.py
--rw-rw-rw-   0        0        0     5377 2024-05-07 07:59:18.000000 steam-sdk-2024.5.1/steam_sdk/data/DataModelCircuit.py
--rw-rw-rw-   0        0        0     5216 2024-03-21 12:23:41.000000 steam-sdk-2024.5.1/steam_sdk/data/DataModelCommon.py
--rw-rw-rw-   0        0        0     6621 2024-03-21 12:23:41.000000 steam-sdk-2024.5.1/steam_sdk/data/DataModelConductor.py
--rw-rw-rw-   0        0        0    12150 2024-04-29 06:28:52.000000 steam-sdk-2024.5.1/steam_sdk/data/DataModelCosim.py
--rw-rw-rw-   0        0        0     8020 2024-03-21 12:23:41.000000 steam-sdk-2024.5.1/steam_sdk/data/DataModelMagnet.py
--rw-rw-rw-   0        0        0     6491 2024-04-19 11:58:44.000000 steam-sdk-2024.5.1/steam_sdk/data/DataModelParsimDakota.py
--rw-rw-rw-   0        0        0     3008 2024-04-08 08:00:24.000000 steam-sdk-2024.5.1/steam_sdk/data/DataParsimConductor.py
--rw-rw-rw-   0        0        0      625 2024-05-08 10:18:52.000000 steam-sdk-2024.5.1/steam_sdk/data/DataPlot.py
--rw-rw-rw-   0        0        0     2130 2024-03-21 12:23:41.000000 steam-sdk-2024.5.1/steam_sdk/data/DataProteCCT.py
--rw-rw-rw-   0        0        0     2956 2024-03-21 12:23:41.000000 steam-sdk-2024.5.1/steam_sdk/data/DataProteCCTOptions.py
--rw-rw-rw-   0        0        0     2595 2024-03-21 12:23:41.000000 steam-sdk-2024.5.1/steam_sdk/data/DataPyBBQ.py
--rw-rw-rw-   0        0        0     1508 2024-03-21 12:23:41.000000 steam-sdk-2024.5.1/steam_sdk/data/DataPyBBQOptions.py
--rw-rw-rw-   0        0        0      766 2024-04-17 14:10:37.000000 steam-sdk-2024.5.1/steam_sdk/data/DataPyCoSim.py
--rw-rw-rw-   0        0        0     6552 2024-03-21 12:23:41.000000 steam-sdk-2024.5.1/steam_sdk/data/DataPySIGMA.py
--rw-rw-rw-   0        0        0     2228 2024-03-21 12:23:41.000000 steam-sdk-2024.5.1/steam_sdk/data/DataPySIGMAOptions.py
--rw-rw-rw-   0        0        0      236 2024-02-01 12:22:22.000000 steam-sdk-2024.5.1/steam_sdk/data/DataRoxieParams.py
--rw-rw-rw-   0        0        0     9824 2024-03-21 12:23:41.000000 steam-sdk-2024.5.1/steam_sdk/data/DataRoxieParser.py
--rw-rw-rw-   0        0        0    12733 2024-05-06 07:29:15.000000 steam-sdk-2024.5.1/steam_sdk/data/DataSettings.py
--rw-rw-rw-   0        0        0     3263 2024-03-21 12:23:41.000000 steam-sdk-2024.5.1/steam_sdk/data/DataSignal.py
--rw-rw-rw-   0        0        0     6024 2024-05-07 07:59:18.000000 steam-sdk-2024.5.1/steam_sdk/data/DataTFM.py
--rw-rw-rw-   0        0        0    18457 2023-11-20 11:26:58.000000 steam-sdk-2024.5.1/steam_sdk/data/DictionaryLEDET.py
--rw-rw-rw-   0        0        0     4482 2022-08-23 08:56:30.000000 steam-sdk-2024.5.1/steam_sdk/data/DictionaryProteCCT.py
--rw-rw-rw-   0        0        0     2902 2022-09-28 09:57:32.000000 steam-sdk-2024.5.1/steam_sdk/data/DictionaryPyBBQ.py
--rw-rw-rw-   0        0        0    30456 2024-04-08 06:18:59.000000 steam-sdk-2024.5.1/steam_sdk/data/TemplateLEDET.py
--rw-rw-rw-   0        0        0     7903 2022-03-30 17:37:43.000000 steam-sdk-2024.5.1/steam_sdk/data/TemplateProteCCT.py
--rw-rw-rw-   0        0        0        0 2022-02-23 07:50:41.000000 steam-sdk-2024.5.1/steam_sdk/data/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-13 09:44:35.641370 steam-sdk-2024.5.1/steam_sdk/drivers/
--rw-rw-rw-   0        0        0     3739 2024-01-31 11:21:01.000000 steam-sdk-2024.5.1/steam_sdk/drivers/DriverANSYS.py
--rw-rw-rw-   0        0        0    13733 2024-04-26 11:34:23.000000 steam-sdk-2024.5.1/steam_sdk/drivers/DriverAnalysis.py
--rw-rw-rw-   0        0        0     7448 2024-04-15 08:30:14.000000 steam-sdk-2024.5.1/steam_sdk/drivers/DriverDakota.py
--rw-rw-rw-   0        0        0     4278 2024-05-06 07:29:15.000000 steam-sdk-2024.5.1/steam_sdk/drivers/DriverFiQuS.py
--rw-rw-rw-   0        0        0     4301 2024-05-13 08:12:26.000000 steam-sdk-2024.5.1/steam_sdk/drivers/DriverLEDET.py
--rw-rw-rw-   0        0        0     1894 2024-03-20 11:29:04.000000 steam-sdk-2024.5.1/steam_sdk/drivers/DriverPSPICE.py
--rw-rw-rw-   0        0        0     2275 2024-04-19 11:54:24.000000 steam-sdk-2024.5.1/steam_sdk/drivers/DriverProteCCT.py
--rw-rw-rw-   0        0        0     2219 2022-06-02 08:33:55.000000 steam-sdk-2024.5.1/steam_sdk/drivers/DriverPyBBQ.py
--rw-rw-rw-   0        0        0      517 2024-02-21 14:45:24.000000 steam-sdk-2024.5.1/steam_sdk/drivers/DriverPySIGMA.py
--rw-rw-rw-   0        0        0     1983 2024-03-13 14:05:47.000000 steam-sdk-2024.5.1/steam_sdk/drivers/DriverXYCE.py
--rw-rw-rw-   0        0        0        0 2022-02-23 07:50:41.000000 steam-sdk-2024.5.1/steam_sdk/drivers/__init__.py
--rw-rw-rw-   0        0        0      723 2024-01-30 11:37:38.000000 steam-sdk-2024.5.1/steam_sdk/drivers/to_DELETE.py
-drwxrwxrwx   0        0        0        0 2024-05-13 09:44:35.941622 steam-sdk-2024.5.1/steam_sdk/parsers/
--rw-rw-rw-   0        0        0     4984 2022-08-22 11:29:04.000000 steam-sdk-2024.5.1/steam_sdk/parsers/CSD_Reader.py
--rw-rw-rw-   0        0        0      315 2023-10-17 12:06:12.000000 steam-sdk-2024.5.1/steam_sdk/parsers/ParserCOMSOLToTxt.py
--rw-rw-rw-   0        0        0    14173 2024-04-17 08:17:01.000000 steam-sdk-2024.5.1/steam_sdk/parsers/ParserCOSIM.py
--rw-rw-rw-   0        0        0     2290 2022-06-24 07:36:06.000000 steam-sdk-2024.5.1/steam_sdk/parsers/ParserCond2d.py
--rw-rw-rw-   0        0        0     1024 2023-10-17 12:06:12.000000 steam-sdk-2024.5.1/steam_sdk/parsers/ParserCsd.py
--rw-rw-rw-   0        0        0     6302 2024-04-17 11:47:52.000000 steam-sdk-2024.5.1/steam_sdk/parsers/ParserCsv.py
--rw-rw-rw-   0        0        0     2729 2024-04-19 11:58:44.000000 steam-sdk-2024.5.1/steam_sdk/parsers/ParserDakota.py
--rw-rw-rw-   0        0        0     8536 2023-02-02 15:29:22.000000 steam-sdk-2024.5.1/steam_sdk/parsers/ParserExcel.py
--rw-rw-rw-   0        0        0     2614 2024-03-19 10:59:46.000000 steam-sdk-2024.5.1/steam_sdk/parsers/ParserFiQuS.py
--rw-rw-rw-   0        0        0     3760 2024-04-17 14:10:36.000000 steam-sdk-2024.5.1/steam_sdk/parsers/ParserFile.py
--rw-rw-rw-   0        0        0    30071 2024-05-06 07:29:15.000000 steam-sdk-2024.5.1/steam_sdk/parsers/ParserLEDET.py
--rw-rw-rw-   0        0        0    18391 2024-05-06 07:29:15.000000 steam-sdk-2024.5.1/steam_sdk/parsers/ParserMap2d.py
--rw-rw-rw-   0        0        0    15085 2024-04-17 12:14:12.000000 steam-sdk-2024.5.1/steam_sdk/parsers/ParserMat.py
--rw-rw-rw-   0        0        0    65009 2024-04-12 12:06:03.000000 steam-sdk-2024.5.1/steam_sdk/parsers/ParserPSPICE.py
--rw-rw-rw-   0        0        0     4706 2023-10-17 12:06:12.000000 steam-sdk-2024.5.1/steam_sdk/parsers/ParserPdf.py
--rw-rw-rw-   0        0        0     6765 2024-03-13 13:40:54.000000 steam-sdk-2024.5.1/steam_sdk/parsers/ParserProteCCT.py
--rw-rw-rw-   0        0        0     1758 2023-10-17 12:06:12.000000 steam-sdk-2024.5.1/steam_sdk/parsers/ParserPyBBQ.py
--rw-rw-rw-   0        0        0     1663 2024-04-17 08:08:09.000000 steam-sdk-2024.5.1/steam_sdk/parsers/ParserPyCoSim.py
--rw-rw-rw-   0        0        0     4061 2024-04-11 22:26:08.000000 steam-sdk-2024.5.1/steam_sdk/parsers/ParserPySIGMA.py
--rw-rw-rw-   0        0        0   155447 2024-04-16 07:32:37.000000 steam-sdk-2024.5.1/steam_sdk/parsers/ParserRoxie.py
--rw-rw-rw-   0        0        0    11746 2024-04-12 13:06:00.000000 steam-sdk-2024.5.1/steam_sdk/parsers/ParserTdms.py
--rw-rw-rw-   0        0        0    58167 2024-05-06 07:29:15.000000 steam-sdk-2024.5.1/steam_sdk/parsers/ParserXYCE.py
--rw-rw-rw-   0        0        0     7770 2024-04-18 11:38:14.000000 steam-sdk-2024.5.1/steam_sdk/parsers/ParserYAML.py
--rw-rw-rw-   0        0        0        0 2022-02-23 07:50:41.000000 steam-sdk-2024.5.1/steam_sdk/parsers/__init__.py
--rw-rw-rw-   0        0        0      929 2024-03-21 13:47:53.000000 steam-sdk-2024.5.1/steam_sdk/parsers/utils_ParserCircuits.py
--rw-rw-rw-   0        0        0     9687 2024-04-29 06:28:52.000000 steam-sdk-2024.5.1/steam_sdk/parsers/utils_ParserCosims.py
-drwxrwxrwx   0        0        0        0 2024-05-13 09:44:35.999923 steam-sdk-2024.5.1/steam_sdk/parsims/
--rw-rw-rw-   0        0        0    66858 2024-04-16 07:32:37.000000 steam-sdk-2024.5.1/steam_sdk/parsims/ParsimConductor.py
--rw-rw-rw-   0        0        0     4619 2024-04-15 08:30:14.000000 steam-sdk-2024.5.1/steam_sdk/parsims/ParsimDakota.py
--rw-rw-rw-   0        0        0    90102 2024-02-16 08:41:13.000000 steam-sdk-2024.5.1/steam_sdk/parsims/ParsimEventCircuit.py
--rw-rw-rw-   0        0        0    48261 2024-03-18 14:18:48.000000 steam-sdk-2024.5.1/steam_sdk/parsims/ParsimEventMagnet.py
--rw-rw-rw-   0        0        0        0 2022-02-23 07:50:41.000000 steam-sdk-2024.5.1/steam_sdk/parsims/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-13 09:44:36.017527 steam-sdk-2024.5.1/steam_sdk/parsims/translation_dicts/
--rw-rw-rw-   0        0        0     2351 2024-04-08 08:04:39.000000 steam-sdk-2024.5.1/steam_sdk/parsims/translation_dicts/conductor_column_names.yaml
--rw-rw-rw-   0        0        0     2016 2023-05-09 19:16:09.000000 steam-sdk-2024.5.1/steam_sdk/parsims/translation_dicts/event_column_names.yaml
-drwxrwxrwx   0        0        0        0 2024-05-13 09:44:36.066815 steam-sdk-2024.5.1/steam_sdk/plotters/
--rw-rw-rw-   0        0        0    29312 2023-07-13 14:20:54.000000 steam-sdk-2024.5.1/steam_sdk/plotters/PlotterAnalysis.py
--rw-rw-rw-   0        0        0     8480 2024-05-08 10:18:52.000000 steam-sdk-2024.5.1/steam_sdk/plotters/PlotterGriddedData.py
--rw-rw-rw-   0        0        0    20627 2024-05-06 07:29:15.000000 steam-sdk-2024.5.1/steam_sdk/plotters/PlotterMap2d.py
--rw-rw-rw-   0        0        0    39519 2024-04-16 07:32:37.000000 steam-sdk-2024.5.1/steam_sdk/plotters/PlotterModel.py
--rw-rw-rw-   0        0        0    22987 2022-12-06 11:41:34.000000 steam-sdk-2024.5.1/steam_sdk/plotters/PlotterParametric.py
--rw-rw-rw-   0        0        0    13246 2024-03-25 10:52:36.000000 steam-sdk-2024.5.1/steam_sdk/plotters/PlotterRoxie.py
--rw-rw-rw-   0        0        0        0 2022-02-23 07:50:41.000000 steam-sdk-2024.5.1/steam_sdk/plotters/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-13 09:44:36.068814 steam-sdk-2024.5.1/steam_sdk/postprocs/
--rw-rw-rw-   0        0        0    15676 2024-05-08 10:18:52.000000 steam-sdk-2024.5.1/steam_sdk/postprocs/PostprocsMetrics.py
--rw-rw-rw-   0        0        0        0 2022-09-14 13:30:58.000000 steam-sdk-2024.5.1/steam_sdk/postprocs/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-13 09:44:36.391945 steam-sdk-2024.5.1/steam_sdk/utils/
--rw-rw-rw-   0        0        0     2679 2023-03-13 09:01:17.000000 steam-sdk-2024.5.1/steam_sdk/utils/MTF_reading_functions.py
--rw-rw-rw-   0        0        0      204 2024-04-16 07:32:37.000000 steam-sdk-2024.5.1/steam_sdk/utils/MatrixOperations.py
--rw-rw-rw-   0        0        0    15002 2024-01-12 14:37:06.000000 steam-sdk-2024.5.1/steam_sdk/utils/ModifyModelData.py
--rw-rw-rw-   0        0        0     3201 2024-04-08 06:18:59.000000 steam-sdk-2024.5.1/steam_sdk/utils/ModifyModelDataMagnet.py
--rw-rw-rw-   0        0        0     2770 2024-04-08 06:18:59.000000 steam-sdk-2024.5.1/steam_sdk/utils/ModifyModelDataconductor.py
--rw-rw-rw-   0        0        0      313 2022-03-01 14:21:51.000000 steam-sdk-2024.5.1/steam_sdk/utils/NumpyEncoder.py
--rw-rw-rw-   0        0        0     5730 2023-06-20 09:25:09.000000 steam-sdk-2024.5.1/steam_sdk/utils/ParserRoxieHelpers.py
--rw-rw-rw-   0        0        0        0 2022-02-23 07:50:41.000000 steam-sdk-2024.5.1/steam_sdk/utils/__init__.py
--rw-rw-rw-   0        0        0     5806 2024-03-27 10:23:11.000000 steam-sdk-2024.5.1/steam_sdk/utils/attribute_model.py
--rw-rw-rw-   0        0        0      686 2022-06-12 12:41:34.000000 steam-sdk-2024.5.1/steam_sdk/utils/clean_NaN_from_signal.py
--rw-rw-rw-   0        0        0    12832 2023-10-02 06:56:47.000000 steam-sdk-2024.5.1/steam_sdk/utils/compare_simulations.py
--rw-rw-rw-   0        0        0     3837 2023-02-03 13:26:48.000000 steam-sdk-2024.5.1/steam_sdk/utils/compare_two_parameters.py
--rw-rw-rw-   0        0        0     1650 2024-04-11 23:08:34.000000 steam-sdk-2024.5.1/steam_sdk/utils/correct_RRR_NIST.py
--rw-rw-rw-   0        0        0      227 2024-01-10 14:12:29.000000 steam-sdk-2024.5.1/steam_sdk/utils/delete_if_existing.py
--rw-rw-rw-   0        0        0     1135 2024-04-17 08:22:42.000000 steam-sdk-2024.5.1/steam_sdk/utils/find_delete_files.py
--rw-rw-rw-   0        0        0     1204 2024-03-22 11:11:51.000000 steam-sdk-2024.5.1/steam_sdk/utils/get_attribute_type.py
--rw-rw-rw-   0        0        0      167 2022-06-11 12:54:31.000000 steam-sdk-2024.5.1/steam_sdk/utils/isNaN.py
--rw-rw-rw-   0        0        0      691 2024-04-11 22:26:08.000000 steam-sdk-2024.5.1/steam_sdk/utils/make_folder_if_not_existing.py
--rw-rw-rw-   0        0        0      928 2023-09-25 12:01:38.000000 steam-sdk-2024.5.1/steam_sdk/utils/make_json_schema.py
--rw-rw-rw-   0        0        0     4512 2022-05-02 08:49:48.000000 steam-sdk-2024.5.1/steam_sdk/utils/misc.py
--rw-rw-rw-   0        0        0     1878 2023-11-21 15:44:37.000000 steam-sdk-2024.5.1/steam_sdk/utils/overwrite_files.py
--rw-rw-rw-   0        0        0    11408 2024-01-10 12:09:33.000000 steam-sdk-2024.5.1/steam_sdk/utils/overwrite_output_to_reference_files.py
--rw-rw-rw-   0        0        0     3555 2023-06-13 10:45:51.000000 steam-sdk-2024.5.1/steam_sdk/utils/parse_str_to_list.py
--rw-rw-rw-   0        0        0     1596 2024-04-15 10:55:27.000000 steam-sdk-2024.5.1/steam_sdk/utils/read_settings_file.py
--rw-rw-rw-   0        0        0     3365 2023-12-06 09:10:21.000000 steam-sdk-2024.5.1/steam_sdk/utils/reformat_figure.py
--rw-rw-rw-   0        0        0      388 2022-04-11 18:20:26.000000 steam-sdk-2024.5.1/steam_sdk/utils/rgetattr.py
--rw-rw-rw-   0        0        0      460 2023-01-07 20:16:27.000000 steam-sdk-2024.5.1/steam_sdk/utils/rhasattr.py
--rw-rw-rw-   0        0        0      383 2022-04-11 18:20:26.000000 steam-sdk-2024.5.1/steam_sdk/utils/sgetattr.py
--rw-rw-rw-   0        0        0      863 2022-02-23 07:50:41.000000 steam-sdk-2024.5.1/steam_sdk/utils/tic_toc.py
--rw-rw-rw-   0        0        0      168 2022-06-07 19:34:59.000000 steam-sdk-2024.5.1/steam_sdk/utils/unique.py
--rw-rw-rw-   0        0        0     7005 2023-05-12 14:38:34.000000 steam-sdk-2024.5.1/steam_sdk/utils/utils_PC.py
-drwxrwxrwx   0        0        0        0 2024-05-13 09:44:36.410513 steam-sdk-2024.5.1/steam_sdk/viewers/
--rw-rw-rw-   0        0        0    39140 2024-02-23 08:10:26.000000 steam-sdk-2024.5.1/steam_sdk/viewers/Viewer.py
--rw-rw-rw-   0        0        0        0 2022-02-23 07:50:41.000000 steam-sdk-2024.5.1/steam_sdk/viewers/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-13 09:44:36.426586 steam-sdk-2024.5.1/steam_sdk/wrappers/
--rw-rw-rw-   0        0        0        0 2022-02-23 07:50:41.000000 steam-sdk-2024.5.1/steam_sdk/wrappers/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-13 09:44:36.428582 steam-sdk-2024.5.1/steam_sdk/wrappers/java/
-drwxrwxrwx   0        0        0        0 2024-05-13 09:44:36.432586 steam-sdk-2024.5.1/steam_sdk/wrappers/java/SING/
--rw-rw-rw-   0        0        0        0 2022-02-23 07:50:41.000000 steam-sdk-2024.5.1/steam_sdk/wrappers/java/SING/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-13 09:44:36.436658 steam-sdk-2024.5.1/steam_sdk/wrappers/java/SING/jars/
--rw-rw-rw-   0        0        0        0 2022-02-23 07:50:41.000000 steam-sdk-2024.5.1/steam_sdk/wrappers/java/SING/jars/__init__.py
--rw-rw-rw-   0        0        0        0 2022-02-23 07:50:41.000000 steam-sdk-2024.5.1/steam_sdk/wrappers/java/__init__.py
--rw-rw-rw-   0        0        0     1830 2024-01-10 12:13:04.000000 steam-sdk-2024.5.1/steam_sdk/wrappers/wrapper_yaml.py
-drwxrwxrwx   0        0        0        0 2024-05-13 09:44:36.437660 steam-sdk-2024.5.1/steam_sdk.egg-info/
--rw-rw-rw-   0        0        0     5753 2024-05-13 09:44:34.000000 steam-sdk-2024.5.1/steam_sdk.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     7888 2024-05-13 09:44:34.000000 steam-sdk-2024.5.1/steam_sdk.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-13 09:44:34.000000 steam-sdk-2024.5.1/steam_sdk.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0     1745 2024-05-13 09:44:34.000000 steam-sdk-2024.5.1/steam_sdk.egg-info/requires.txt
--rw-rw-rw-   0        0        0       16 2024-05-13 09:44:34.000000 steam-sdk-2024.5.1/steam_sdk.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-13 10:13:26.404884 steam-sdk-2024.5.2/
+-rw-rw-rw-   0        0        0      264 2023-06-07 14:48:24.000000 steam-sdk-2024.5.2/MANIFEST.in
+-rw-rw-rw-   0        0        0     5753 2024-05-13 10:13:26.402882 steam-sdk-2024.5.2/PKG-INFO
+-rw-rw-rw-   0        0        0       42 2024-05-13 10:13:26.404884 steam-sdk-2024.5.2/setup.cfg
+-rw-rw-rw-   0        0        0     1668 2024-05-13 10:12:09.000000 steam-sdk-2024.5.2/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-13 10:13:26.095886 steam-sdk-2024.5.2/steam_sdk/
+-rw-rw-rw-   0        0        0        0 2022-02-23 07:50:41.000000 steam-sdk-2024.5.2/steam_sdk/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-13 10:13:26.141883 steam-sdk-2024.5.2/steam_sdk/analyses/
+-rw-rw-rw-   0        0        0    37589 2024-04-19 11:58:44.000000 steam-sdk-2024.5.2/steam_sdk/analyses/AnalysisEvent.py
+-rw-rw-rw-   0        0        0    30954 2024-04-26 11:34:23.000000 steam-sdk-2024.5.2/steam_sdk/analyses/AnalysisEventLHC.py
+-rw-rw-rw-   0        0        0   135654 2024-05-13 10:08:33.000000 steam-sdk-2024.5.2/steam_sdk/analyses/AnalysisSTEAM.py
+-rw-rw-rw-   0        0        0        0 2022-02-23 07:50:41.000000 steam-sdk-2024.5.2/steam_sdk/analyses/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-13 10:13:26.143893 steam-sdk-2024.5.2/steam_sdk/analyses/custom_analyses/
+-rw-rw-rw-   0        0        0        0 2022-02-23 07:50:41.000000 steam-sdk-2024.5.2/steam_sdk/analyses/custom_analyses/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-13 10:13:26.146883 steam-sdk-2024.5.2/steam_sdk/analyses/custom_analyses/analysis_short_circuit_LEDET_1/
+-rw-rw-rw-   0        0        0        0 2022-02-23 07:50:41.000000 steam-sdk-2024.5.2/steam_sdk/analyses/custom_analyses/analysis_short_circuit_LEDET_1/__init__.py
+-rw-rw-rw-   0        0        0    23388 2024-01-12 14:29:22.000000 steam-sdk-2024.5.2/steam_sdk/analyses/custom_analyses/analysis_short_circuit_LEDET_1/analysis_short_circuit_LEDET_1.py
+drwxrwxrwx   0        0        0        0 2024-05-13 10:13:26.156888 steam-sdk-2024.5.2/steam_sdk/analyses/custom_analyses/analysis_short_circuit_LEDET_1/utils/
+-rw-rw-rw-   0        0        0        0 2022-02-23 07:50:41.000000 steam-sdk-2024.5.2/steam_sdk/analyses/custom_analyses/analysis_short_circuit_LEDET_1/utils/__init__.py
+-rw-rw-rw-   0        0        0    16777 2024-01-12 14:32:10.000000 steam-sdk-2024.5.2/steam_sdk/analyses/custom_analyses/analysis_short_circuit_LEDET_1/utils/calculate_short_parameters.py
+-rw-rw-rw-   0        0        0     2820 2024-01-12 14:32:10.000000 steam-sdk-2024.5.2/steam_sdk/analyses/custom_analyses/analysis_short_circuit_LEDET_1/utils/copy_input_files.py
+-rw-rw-rw-   0        0        0     6761 2024-01-12 14:32:10.000000 steam-sdk-2024.5.2/steam_sdk/analyses/custom_analyses/analysis_short_circuit_LEDET_1/utils/set_common_parameters.py
+-rw-rw-rw-   0        0        0    95432 2024-01-12 14:32:10.000000 steam-sdk-2024.5.2/steam_sdk/analyses/custom_analyses/analysis_short_circuit_LEDET_1/utils/set_magnet_specific_parameters.py
+-rw-rw-rw-   0        0        0     2672 2024-01-12 14:32:10.000000 steam-sdk-2024.5.2/steam_sdk/analyses/custom_analyses/analysis_short_circuit_LEDET_1/utils/set_short_circuit_analysis_parameters.py
+-rw-rw-rw-   0        0        0     2361 2024-01-12 14:29:35.000000 steam-sdk-2024.5.2/steam_sdk/analyses/custom_analyses/analysis_short_circuit_LEDET_1/utils/set_simulations_to_prepare_run.py
+drwxrwxrwx   0        0        0        0 2024-05-13 10:13:26.158883 steam-sdk-2024.5.2/steam_sdk/analyses/custom_analyses/co_simulation_QH_PyBBQ_LEDET_1/
+-rw-rw-rw-   0        0        0        0 2022-02-23 07:50:41.000000 steam-sdk-2024.5.2/steam_sdk/analyses/custom_analyses/co_simulation_QH_PyBBQ_LEDET_1/__init__.py
+-rw-rw-rw-   0        0        0    22357 2024-03-11 05:39:28.000000 steam-sdk-2024.5.2/steam_sdk/analyses/custom_analyses/co_simulation_QH_PyBBQ_LEDET_1/co_simulation_QH_PyBBQ_LEDET_1.py
+drwxrwxrwx   0        0        0        0 2024-05-13 10:13:26.166882 steam-sdk-2024.5.2/steam_sdk/analyses/custom_analyses/co_simulation_QH_PyBBQ_LEDET_1/utils/
+-rw-rw-rw-   0        0        0        0 2022-09-26 06:59:06.000000 steam-sdk-2024.5.2/steam_sdk/analyses/custom_analyses/co_simulation_QH_PyBBQ_LEDET_1/utils/__init__.py
+-rw-rw-rw-   0        0        0     5330 2024-01-12 14:32:10.000000 steam-sdk-2024.5.2/steam_sdk/analyses/custom_analyses/co_simulation_QH_PyBBQ_LEDET_1/utils/calculate_quench_propagation_velocity.py
+-rw-rw-rw-   0        0        0     4450 2024-01-12 14:32:10.000000 steam-sdk-2024.5.2/steam_sdk/analyses/custom_analyses/co_simulation_QH_PyBBQ_LEDET_1/utils/create_conductor_analysis_file.py
+-rw-rw-rw-   0        0        0     2844 2024-01-12 14:32:10.000000 steam-sdk-2024.5.2/steam_sdk/analyses/custom_analyses/co_simulation_QH_PyBBQ_LEDET_1/utils/create_magnet_analysis_file.py
+drwxrwxrwx   0        0        0        0 2024-05-13 10:13:26.169882 steam-sdk-2024.5.2/steam_sdk/analyses/custom_analyses/co_simulation_QH_PyBBQ_LEDET_MBRD_validation_1/
+-rw-rw-rw-   0        0        0        0 2022-09-26 06:59:06.000000 steam-sdk-2024.5.2/steam_sdk/analyses/custom_analyses/co_simulation_QH_PyBBQ_LEDET_MBRD_validation_1/__init__.py
+-rw-rw-rw-   0        0        0    29436 2024-03-11 05:39:28.000000 steam-sdk-2024.5.2/steam_sdk/analyses/custom_analyses/co_simulation_QH_PyBBQ_LEDET_MBRD_validation_1/co_simulation_QH_PyBBQ_LEDET_MBRD_validation_1.py
+drwxrwxrwx   0        0        0        0 2024-05-13 10:13:26.175882 steam-sdk-2024.5.2/steam_sdk/analyses/custom_analyses/co_simulation_QH_PyBBQ_LEDET_MBRD_validation_1/utils/
+-rw-rw-rw-   0        0        0        0 2022-09-26 06:59:06.000000 steam-sdk-2024.5.2/steam_sdk/analyses/custom_analyses/co_simulation_QH_PyBBQ_LEDET_MBRD_validation_1/utils/__init__.py
+-rw-rw-rw-   0        0        0     5330 2024-01-12 14:32:09.000000 steam-sdk-2024.5.2/steam_sdk/analyses/custom_analyses/co_simulation_QH_PyBBQ_LEDET_MBRD_validation_1/utils/calculate_quench_propagation_velocity.py
+-rw-rw-rw-   0        0        0     4627 2024-01-12 14:32:10.000000 steam-sdk-2024.5.2/steam_sdk/analyses/custom_analyses/co_simulation_QH_PyBBQ_LEDET_MBRD_validation_1/utils/create_conductor_analysis_file.py
+-rw-rw-rw-   0        0        0     4775 2024-01-12 14:32:10.000000 steam-sdk-2024.5.2/steam_sdk/analyses/custom_analyses/co_simulation_QH_PyBBQ_LEDET_MBRD_validation_1/utils/create_magnet_analysis_file.py
+drwxrwxrwx   0        0        0        0 2024-05-13 10:13:26.179894 steam-sdk-2024.5.2/steam_sdk/analyses/custom_analyses/custom_function_test_1/
+-rw-rw-rw-   0        0        0        0 2022-02-23 07:50:41.000000 steam-sdk-2024.5.2/steam_sdk/analyses/custom_analyses/custom_function_test_1/__init__.py
+-rw-rw-rw-   0        0        0     1307 2022-09-10 00:27:54.000000 steam-sdk-2024.5.2/steam_sdk/analyses/custom_analyses/custom_function_test_1/custom_function_test_1.py
+drwxrwxrwx   0        0        0        0 2024-05-13 10:13:26.198882 steam-sdk-2024.5.2/steam_sdk/builders/
+-rw-rw-rw-   0        0        0    13175 2024-03-13 09:34:54.000000 steam-sdk-2024.5.2/steam_sdk/builders/BuilderAPDL_CT.py
+-rw-rw-rw-   0        0        0     4805 2024-03-22 08:53:57.000000 steam-sdk-2024.5.2/steam_sdk/builders/BuilderCosim.py
+-rw-rw-rw-   0        0        0    17741 2024-02-07 15:54:14.000000 steam-sdk-2024.5.2/steam_sdk/builders/BuilderFiQuS.py
+-rw-rw-rw-   0        0        0   160440 2024-04-17 14:10:37.000000 steam-sdk-2024.5.2/steam_sdk/builders/BuilderLEDET.py
+-rw-rw-rw-   0        0        0    53471 2024-05-08 10:36:11.000000 steam-sdk-2024.5.2/steam_sdk/builders/BuilderModel.py
+-rw-rw-rw-   0        0        0    12686 2024-03-13 11:10:16.000000 steam-sdk-2024.5.2/steam_sdk/builders/BuilderProteCCT.py
+-rw-rw-rw-   0        0        0     6749 2022-08-22 11:29:04.000000 steam-sdk-2024.5.2/steam_sdk/builders/BuilderPyBBQ.py
+-rw-rw-rw-   0        0        0    12487 2024-04-11 22:26:08.000000 steam-sdk-2024.5.2/steam_sdk/builders/BuilderPySIGMA.py
+-rw-rw-rw-   0        0        0    57747 2024-05-07 07:59:18.000000 steam-sdk-2024.5.2/steam_sdk/builders/BuilderTFM.py
+-rw-rw-rw-   0        0        0    11689 2023-01-18 09:46:00.000000 steam-sdk-2024.5.2/steam_sdk/builders/SelfMutualInductanceCalculation.py
+-rw-rw-rw-   0        0        0     7941 2022-12-06 11:41:34.000000 steam-sdk-2024.5.2/steam_sdk/builders/Solenoids.py
+-rw-rw-rw-   0        0        0        0 2022-02-23 07:50:41.000000 steam-sdk-2024.5.2/steam_sdk/builders/__init__.py
+-rw-rw-rw-   0        0        0     8352 2023-02-02 15:39:34.000000 steam-sdk-2024.5.2/steam_sdk/builders/geometricFunctions.py
+drwxrwxrwx   0        0        0        0 2024-05-13 10:13:26.199884 steam-sdk-2024.5.2/steam_sdk/configs/
+-rw-rw-rw-   0        0        0        0 2022-02-23 07:50:41.000000 steam-sdk-2024.5.2/steam_sdk/configs/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-13 10:13:26.200881 steam-sdk-2024.5.2/steam_sdk/configs/tools_defaults/
+drwxrwxrwx   0        0        0        0 2024-05-13 10:13:26.201884 steam-sdk-2024.5.2/steam_sdk/configs/tools_defaults/LEDET/
+-rw-rw-rw-   0        0        0        0 2022-02-23 07:50:41.000000 steam-sdk-2024.5.2/steam_sdk/configs/tools_defaults/LEDET/__init__.py
+-rw-rw-rw-   0        0        0     1426 2022-02-23 07:50:41.000000 steam-sdk-2024.5.2/steam_sdk/configs/tools_defaults/ToolDefaultReader.py
+-rw-rw-rw-   0        0        0        0 2022-02-23 07:50:41.000000 steam-sdk-2024.5.2/steam_sdk/configs/tools_defaults/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-13 10:13:26.203900 steam-sdk-2024.5.2/steam_sdk/cosims/
+-rw-rw-rw-   0        0        0    26984 2024-04-29 06:28:52.000000 steam-sdk-2024.5.2/steam_sdk/cosims/CoSimPyCoSim.py
+-rw-rw-rw-   0        0        0        0 2022-02-23 07:50:41.000000 steam-sdk-2024.5.2/steam_sdk/cosims/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-13 10:13:26.263884 steam-sdk-2024.5.2/steam_sdk/data/
+-rw-rw-rw-   0        0        0     1684 2024-03-21 12:23:41.000000 steam-sdk-2024.5.2/steam_sdk/data/DataAPDLCTOptions.py
+-rw-rw-rw-   0        0        0    13001 2024-05-08 10:18:52.000000 steam-sdk-2024.5.2/steam_sdk/data/DataAnalysis.py
+-rw-rw-rw-   0        0        0      414 2024-03-06 09:01:34.000000 steam-sdk-2024.5.2/steam_sdk/data/DataCoSim.py
+-rw-rw-rw-   0        0        0     9303 2024-04-08 06:18:59.000000 steam-sdk-2024.5.2/steam_sdk/data/DataConductor.py
+-rw-rw-rw-   0        0        0      308 2024-04-19 11:58:44.000000 steam-sdk-2024.5.2/steam_sdk/data/DataDakota.py
+-rw-rw-rw-   0        0        0     2987 2024-03-21 12:23:41.000000 steam-sdk-2024.5.2/steam_sdk/data/DataEventCircuit.py
+-rw-rw-rw-   0        0        0     4636 2024-03-21 12:23:41.000000 steam-sdk-2024.5.2/steam_sdk/data/DataEventMagnet.py
+-rw-rw-rw-   0        0        0    87484 2024-05-13 08:12:26.000000 steam-sdk-2024.5.2/steam_sdk/data/DataFiQuS.py
+-rw-rw-rw-   0        0        0     7309 2024-03-21 12:23:41.000000 steam-sdk-2024.5.2/steam_sdk/data/DataFiQuSOptions.py
+-rw-rw-rw-   0        0        0    16769 2024-04-08 06:18:59.000000 steam-sdk-2024.5.2/steam_sdk/data/DataLEDET.py
+-rw-rw-rw-   0        0        0     9528 2024-03-21 12:23:41.000000 steam-sdk-2024.5.2/steam_sdk/data/DataLEDETOptions.py
+-rw-rw-rw-   0        0        0     5377 2024-05-07 07:59:18.000000 steam-sdk-2024.5.2/steam_sdk/data/DataModelCircuit.py
+-rw-rw-rw-   0        0        0     5216 2024-03-21 12:23:41.000000 steam-sdk-2024.5.2/steam_sdk/data/DataModelCommon.py
+-rw-rw-rw-   0        0        0     6621 2024-03-21 12:23:41.000000 steam-sdk-2024.5.2/steam_sdk/data/DataModelConductor.py
+-rw-rw-rw-   0        0        0    12150 2024-04-29 06:28:52.000000 steam-sdk-2024.5.2/steam_sdk/data/DataModelCosim.py
+-rw-rw-rw-   0        0        0     8020 2024-03-21 12:23:41.000000 steam-sdk-2024.5.2/steam_sdk/data/DataModelMagnet.py
+-rw-rw-rw-   0        0        0     6491 2024-04-19 11:58:44.000000 steam-sdk-2024.5.2/steam_sdk/data/DataModelParsimDakota.py
+-rw-rw-rw-   0        0        0     3008 2024-04-08 08:00:24.000000 steam-sdk-2024.5.2/steam_sdk/data/DataParsimConductor.py
+-rw-rw-rw-   0        0        0      625 2024-05-08 10:18:52.000000 steam-sdk-2024.5.2/steam_sdk/data/DataPlot.py
+-rw-rw-rw-   0        0        0     2130 2024-03-21 12:23:41.000000 steam-sdk-2024.5.2/steam_sdk/data/DataProteCCT.py
+-rw-rw-rw-   0        0        0     2956 2024-03-21 12:23:41.000000 steam-sdk-2024.5.2/steam_sdk/data/DataProteCCTOptions.py
+-rw-rw-rw-   0        0        0     2595 2024-03-21 12:23:41.000000 steam-sdk-2024.5.2/steam_sdk/data/DataPyBBQ.py
+-rw-rw-rw-   0        0        0     1508 2024-03-21 12:23:41.000000 steam-sdk-2024.5.2/steam_sdk/data/DataPyBBQOptions.py
+-rw-rw-rw-   0        0        0      766 2024-04-17 14:10:37.000000 steam-sdk-2024.5.2/steam_sdk/data/DataPyCoSim.py
+-rw-rw-rw-   0        0        0     6552 2024-03-21 12:23:41.000000 steam-sdk-2024.5.2/steam_sdk/data/DataPySIGMA.py
+-rw-rw-rw-   0        0        0     2228 2024-03-21 12:23:41.000000 steam-sdk-2024.5.2/steam_sdk/data/DataPySIGMAOptions.py
+-rw-rw-rw-   0        0        0      236 2024-02-01 12:22:22.000000 steam-sdk-2024.5.2/steam_sdk/data/DataRoxieParams.py
+-rw-rw-rw-   0        0        0     9824 2024-03-21 12:23:41.000000 steam-sdk-2024.5.2/steam_sdk/data/DataRoxieParser.py
+-rw-rw-rw-   0        0        0    12733 2024-05-06 07:29:15.000000 steam-sdk-2024.5.2/steam_sdk/data/DataSettings.py
+-rw-rw-rw-   0        0        0     3263 2024-03-21 12:23:41.000000 steam-sdk-2024.5.2/steam_sdk/data/DataSignal.py
+-rw-rw-rw-   0        0        0     6024 2024-05-07 07:59:18.000000 steam-sdk-2024.5.2/steam_sdk/data/DataTFM.py
+-rw-rw-rw-   0        0        0    18457 2023-11-20 11:26:58.000000 steam-sdk-2024.5.2/steam_sdk/data/DictionaryLEDET.py
+-rw-rw-rw-   0        0        0     4482 2022-08-23 08:56:30.000000 steam-sdk-2024.5.2/steam_sdk/data/DictionaryProteCCT.py
+-rw-rw-rw-   0        0        0     2902 2022-09-28 09:57:32.000000 steam-sdk-2024.5.2/steam_sdk/data/DictionaryPyBBQ.py
+-rw-rw-rw-   0        0        0    30456 2024-04-08 06:18:59.000000 steam-sdk-2024.5.2/steam_sdk/data/TemplateLEDET.py
+-rw-rw-rw-   0        0        0     7903 2022-03-30 17:37:43.000000 steam-sdk-2024.5.2/steam_sdk/data/TemplateProteCCT.py
+-rw-rw-rw-   0        0        0        0 2022-02-23 07:50:41.000000 steam-sdk-2024.5.2/steam_sdk/data/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-13 10:13:26.279890 steam-sdk-2024.5.2/steam_sdk/drivers/
+-rw-rw-rw-   0        0        0     3739 2024-01-31 11:21:01.000000 steam-sdk-2024.5.2/steam_sdk/drivers/DriverANSYS.py
+-rw-rw-rw-   0        0        0    13733 2024-04-26 11:34:23.000000 steam-sdk-2024.5.2/steam_sdk/drivers/DriverAnalysis.py
+-rw-rw-rw-   0        0        0     7448 2024-04-15 08:30:14.000000 steam-sdk-2024.5.2/steam_sdk/drivers/DriverDakota.py
+-rw-rw-rw-   0        0        0     4278 2024-05-06 07:29:15.000000 steam-sdk-2024.5.2/steam_sdk/drivers/DriverFiQuS.py
+-rw-rw-rw-   0        0        0     4301 2024-05-13 08:12:26.000000 steam-sdk-2024.5.2/steam_sdk/drivers/DriverLEDET.py
+-rw-rw-rw-   0        0        0     1894 2024-03-20 11:29:04.000000 steam-sdk-2024.5.2/steam_sdk/drivers/DriverPSPICE.py
+-rw-rw-rw-   0        0        0     2275 2024-04-19 11:54:24.000000 steam-sdk-2024.5.2/steam_sdk/drivers/DriverProteCCT.py
+-rw-rw-rw-   0        0        0     2219 2022-06-02 08:33:55.000000 steam-sdk-2024.5.2/steam_sdk/drivers/DriverPyBBQ.py
+-rw-rw-rw-   0        0        0      517 2024-02-21 14:45:24.000000 steam-sdk-2024.5.2/steam_sdk/drivers/DriverPySIGMA.py
+-rw-rw-rw-   0        0        0     1983 2024-03-13 14:05:47.000000 steam-sdk-2024.5.2/steam_sdk/drivers/DriverXYCE.py
+-rw-rw-rw-   0        0        0        0 2022-02-23 07:50:41.000000 steam-sdk-2024.5.2/steam_sdk/drivers/__init__.py
+-rw-rw-rw-   0        0        0      723 2024-01-30 11:37:38.000000 steam-sdk-2024.5.2/steam_sdk/drivers/to_DELETE.py
+drwxrwxrwx   0        0        0        0 2024-05-13 10:13:26.318883 steam-sdk-2024.5.2/steam_sdk/parsers/
+-rw-rw-rw-   0        0        0     4984 2022-08-22 11:29:04.000000 steam-sdk-2024.5.2/steam_sdk/parsers/CSD_Reader.py
+-rw-rw-rw-   0        0        0      315 2023-10-17 12:06:12.000000 steam-sdk-2024.5.2/steam_sdk/parsers/ParserCOMSOLToTxt.py
+-rw-rw-rw-   0        0        0    14173 2024-04-17 08:17:01.000000 steam-sdk-2024.5.2/steam_sdk/parsers/ParserCOSIM.py
+-rw-rw-rw-   0        0        0     2290 2022-06-24 07:36:06.000000 steam-sdk-2024.5.2/steam_sdk/parsers/ParserCond2d.py
+-rw-rw-rw-   0        0        0     1024 2023-10-17 12:06:12.000000 steam-sdk-2024.5.2/steam_sdk/parsers/ParserCsd.py
+-rw-rw-rw-   0        0        0     6302 2024-04-17 11:47:52.000000 steam-sdk-2024.5.2/steam_sdk/parsers/ParserCsv.py
+-rw-rw-rw-   0        0        0     2729 2024-04-19 11:58:44.000000 steam-sdk-2024.5.2/steam_sdk/parsers/ParserDakota.py
+-rw-rw-rw-   0        0        0     8536 2023-02-02 15:29:22.000000 steam-sdk-2024.5.2/steam_sdk/parsers/ParserExcel.py
+-rw-rw-rw-   0        0        0     2614 2024-03-19 10:59:46.000000 steam-sdk-2024.5.2/steam_sdk/parsers/ParserFiQuS.py
+-rw-rw-rw-   0        0        0     3760 2024-04-17 14:10:36.000000 steam-sdk-2024.5.2/steam_sdk/parsers/ParserFile.py
+-rw-rw-rw-   0        0        0    30071 2024-05-06 07:29:15.000000 steam-sdk-2024.5.2/steam_sdk/parsers/ParserLEDET.py
+-rw-rw-rw-   0        0        0    18391 2024-05-06 07:29:15.000000 steam-sdk-2024.5.2/steam_sdk/parsers/ParserMap2d.py
+-rw-rw-rw-   0        0        0    15085 2024-04-17 12:14:12.000000 steam-sdk-2024.5.2/steam_sdk/parsers/ParserMat.py
+-rw-rw-rw-   0        0        0    65009 2024-04-12 12:06:03.000000 steam-sdk-2024.5.2/steam_sdk/parsers/ParserPSPICE.py
+-rw-rw-rw-   0        0        0     4706 2023-10-17 12:06:12.000000 steam-sdk-2024.5.2/steam_sdk/parsers/ParserPdf.py
+-rw-rw-rw-   0        0        0     6765 2024-03-13 13:40:54.000000 steam-sdk-2024.5.2/steam_sdk/parsers/ParserProteCCT.py
+-rw-rw-rw-   0        0        0     1758 2023-10-17 12:06:12.000000 steam-sdk-2024.5.2/steam_sdk/parsers/ParserPyBBQ.py
+-rw-rw-rw-   0        0        0     1663 2024-04-17 08:08:09.000000 steam-sdk-2024.5.2/steam_sdk/parsers/ParserPyCoSim.py
+-rw-rw-rw-   0        0        0     4061 2024-04-11 22:26:08.000000 steam-sdk-2024.5.2/steam_sdk/parsers/ParserPySIGMA.py
+-rw-rw-rw-   0        0        0   155447 2024-04-16 07:32:37.000000 steam-sdk-2024.5.2/steam_sdk/parsers/ParserRoxie.py
+-rw-rw-rw-   0        0        0    11746 2024-04-12 13:06:00.000000 steam-sdk-2024.5.2/steam_sdk/parsers/ParserTdms.py
+-rw-rw-rw-   0        0        0    58167 2024-05-06 07:29:15.000000 steam-sdk-2024.5.2/steam_sdk/parsers/ParserXYCE.py
+-rw-rw-rw-   0        0        0     7770 2024-04-18 11:38:14.000000 steam-sdk-2024.5.2/steam_sdk/parsers/ParserYAML.py
+-rw-rw-rw-   0        0        0        0 2022-02-23 07:50:41.000000 steam-sdk-2024.5.2/steam_sdk/parsers/__init__.py
+-rw-rw-rw-   0        0        0      929 2024-03-21 13:47:53.000000 steam-sdk-2024.5.2/steam_sdk/parsers/utils_ParserCircuits.py
+-rw-rw-rw-   0        0        0     9687 2024-04-29 06:28:52.000000 steam-sdk-2024.5.2/steam_sdk/parsers/utils_ParserCosims.py
+drwxrwxrwx   0        0        0        0 2024-05-13 10:13:26.329883 steam-sdk-2024.5.2/steam_sdk/parsims/
+-rw-rw-rw-   0        0        0    66858 2024-04-16 07:32:37.000000 steam-sdk-2024.5.2/steam_sdk/parsims/ParsimConductor.py
+-rw-rw-rw-   0        0        0     4619 2024-04-15 08:30:14.000000 steam-sdk-2024.5.2/steam_sdk/parsims/ParsimDakota.py
+-rw-rw-rw-   0        0        0    90102 2024-02-16 08:41:13.000000 steam-sdk-2024.5.2/steam_sdk/parsims/ParsimEventCircuit.py
+-rw-rw-rw-   0        0        0    48261 2024-03-18 14:18:48.000000 steam-sdk-2024.5.2/steam_sdk/parsims/ParsimEventMagnet.py
+-rw-rw-rw-   0        0        0        0 2022-02-23 07:50:41.000000 steam-sdk-2024.5.2/steam_sdk/parsims/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-13 10:13:26.331883 steam-sdk-2024.5.2/steam_sdk/parsims/translation_dicts/
+-rw-rw-rw-   0        0        0     2351 2024-04-08 08:04:39.000000 steam-sdk-2024.5.2/steam_sdk/parsims/translation_dicts/conductor_column_names.yaml
+-rw-rw-rw-   0        0        0     2016 2023-05-09 19:16:09.000000 steam-sdk-2024.5.2/steam_sdk/parsims/translation_dicts/event_column_names.yaml
+drwxrwxrwx   0        0        0        0 2024-05-13 10:13:26.341883 steam-sdk-2024.5.2/steam_sdk/plotters/
+-rw-rw-rw-   0        0        0    29312 2023-07-13 14:20:54.000000 steam-sdk-2024.5.2/steam_sdk/plotters/PlotterAnalysis.py
+-rw-rw-rw-   0        0        0     8480 2024-05-08 10:18:52.000000 steam-sdk-2024.5.2/steam_sdk/plotters/PlotterGriddedData.py
+-rw-rw-rw-   0        0        0    20627 2024-05-06 07:29:15.000000 steam-sdk-2024.5.2/steam_sdk/plotters/PlotterMap2d.py
+-rw-rw-rw-   0        0        0    39519 2024-04-16 07:32:37.000000 steam-sdk-2024.5.2/steam_sdk/plotters/PlotterModel.py
+-rw-rw-rw-   0        0        0    22987 2022-12-06 11:41:34.000000 steam-sdk-2024.5.2/steam_sdk/plotters/PlotterParametric.py
+-rw-rw-rw-   0        0        0    13246 2024-03-25 10:52:36.000000 steam-sdk-2024.5.2/steam_sdk/plotters/PlotterRoxie.py
+-rw-rw-rw-   0        0        0        0 2022-02-23 07:50:41.000000 steam-sdk-2024.5.2/steam_sdk/plotters/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-13 10:13:26.343883 steam-sdk-2024.5.2/steam_sdk/postprocs/
+-rw-rw-rw-   0        0        0    15676 2024-05-08 10:18:52.000000 steam-sdk-2024.5.2/steam_sdk/postprocs/PostprocsMetrics.py
+-rw-rw-rw-   0        0        0        0 2022-09-14 13:30:58.000000 steam-sdk-2024.5.2/steam_sdk/postprocs/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-13 10:13:26.382883 steam-sdk-2024.5.2/steam_sdk/utils/
+-rw-rw-rw-   0        0        0     2679 2023-03-13 09:01:17.000000 steam-sdk-2024.5.2/steam_sdk/utils/MTF_reading_functions.py
+-rw-rw-rw-   0        0        0      204 2024-04-16 07:32:37.000000 steam-sdk-2024.5.2/steam_sdk/utils/MatrixOperations.py
+-rw-rw-rw-   0        0        0    15002 2024-01-12 14:37:06.000000 steam-sdk-2024.5.2/steam_sdk/utils/ModifyModelData.py
+-rw-rw-rw-   0        0        0     3201 2024-04-08 06:18:59.000000 steam-sdk-2024.5.2/steam_sdk/utils/ModifyModelDataMagnet.py
+-rw-rw-rw-   0        0        0     2770 2024-04-08 06:18:59.000000 steam-sdk-2024.5.2/steam_sdk/utils/ModifyModelDataconductor.py
+-rw-rw-rw-   0        0        0      313 2022-03-01 14:21:51.000000 steam-sdk-2024.5.2/steam_sdk/utils/NumpyEncoder.py
+-rw-rw-rw-   0        0        0     5730 2023-06-20 09:25:09.000000 steam-sdk-2024.5.2/steam_sdk/utils/ParserRoxieHelpers.py
+-rw-rw-rw-   0        0        0        0 2022-02-23 07:50:41.000000 steam-sdk-2024.5.2/steam_sdk/utils/__init__.py
+-rw-rw-rw-   0        0        0     5806 2024-03-27 10:23:11.000000 steam-sdk-2024.5.2/steam_sdk/utils/attribute_model.py
+-rw-rw-rw-   0        0        0      686 2022-06-12 12:41:34.000000 steam-sdk-2024.5.2/steam_sdk/utils/clean_NaN_from_signal.py
+-rw-rw-rw-   0        0        0    12832 2023-10-02 06:56:47.000000 steam-sdk-2024.5.2/steam_sdk/utils/compare_simulations.py
+-rw-rw-rw-   0        0        0     3837 2023-02-03 13:26:48.000000 steam-sdk-2024.5.2/steam_sdk/utils/compare_two_parameters.py
+-rw-rw-rw-   0        0        0     1650 2024-04-11 23:08:34.000000 steam-sdk-2024.5.2/steam_sdk/utils/correct_RRR_NIST.py
+-rw-rw-rw-   0        0        0      227 2024-01-10 14:12:29.000000 steam-sdk-2024.5.2/steam_sdk/utils/delete_if_existing.py
+-rw-rw-rw-   0        0        0     1135 2024-04-17 08:22:42.000000 steam-sdk-2024.5.2/steam_sdk/utils/find_delete_files.py
+-rw-rw-rw-   0        0        0     1204 2024-03-22 11:11:51.000000 steam-sdk-2024.5.2/steam_sdk/utils/get_attribute_type.py
+-rw-rw-rw-   0        0        0      167 2022-06-11 12:54:31.000000 steam-sdk-2024.5.2/steam_sdk/utils/isNaN.py
+-rw-rw-rw-   0        0        0      691 2024-04-11 22:26:08.000000 steam-sdk-2024.5.2/steam_sdk/utils/make_folder_if_not_existing.py
+-rw-rw-rw-   0        0        0      928 2023-09-25 12:01:38.000000 steam-sdk-2024.5.2/steam_sdk/utils/make_json_schema.py
+-rw-rw-rw-   0        0        0     4512 2022-05-02 08:49:48.000000 steam-sdk-2024.5.2/steam_sdk/utils/misc.py
+-rw-rw-rw-   0        0        0     1878 2023-11-21 15:44:37.000000 steam-sdk-2024.5.2/steam_sdk/utils/overwrite_files.py
+-rw-rw-rw-   0        0        0    11408 2024-01-10 12:09:33.000000 steam-sdk-2024.5.2/steam_sdk/utils/overwrite_output_to_reference_files.py
+-rw-rw-rw-   0        0        0     3555 2023-06-13 10:45:51.000000 steam-sdk-2024.5.2/steam_sdk/utils/parse_str_to_list.py
+-rw-rw-rw-   0        0        0     1596 2024-04-15 10:55:27.000000 steam-sdk-2024.5.2/steam_sdk/utils/read_settings_file.py
+-rw-rw-rw-   0        0        0     3365 2023-12-06 09:10:21.000000 steam-sdk-2024.5.2/steam_sdk/utils/reformat_figure.py
+-rw-rw-rw-   0        0        0      388 2022-04-11 18:20:26.000000 steam-sdk-2024.5.2/steam_sdk/utils/rgetattr.py
+-rw-rw-rw-   0        0        0      460 2023-01-07 20:16:27.000000 steam-sdk-2024.5.2/steam_sdk/utils/rhasattr.py
+-rw-rw-rw-   0        0        0      383 2022-04-11 18:20:26.000000 steam-sdk-2024.5.2/steam_sdk/utils/sgetattr.py
+-rw-rw-rw-   0        0        0      863 2022-02-23 07:50:41.000000 steam-sdk-2024.5.2/steam_sdk/utils/tic_toc.py
+-rw-rw-rw-   0        0        0      168 2022-06-07 19:34:59.000000 steam-sdk-2024.5.2/steam_sdk/utils/unique.py
+-rw-rw-rw-   0        0        0     7005 2023-05-12 14:38:34.000000 steam-sdk-2024.5.2/steam_sdk/utils/utils_PC.py
+drwxrwxrwx   0        0        0        0 2024-05-13 10:13:26.385882 steam-sdk-2024.5.2/steam_sdk/viewers/
+-rw-rw-rw-   0        0        0    39140 2024-02-23 08:10:26.000000 steam-sdk-2024.5.2/steam_sdk/viewers/Viewer.py
+-rw-rw-rw-   0        0        0        0 2022-02-23 07:50:41.000000 steam-sdk-2024.5.2/steam_sdk/viewers/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-13 10:13:26.387883 steam-sdk-2024.5.2/steam_sdk/wrappers/
+-rw-rw-rw-   0        0        0        0 2022-02-23 07:50:41.000000 steam-sdk-2024.5.2/steam_sdk/wrappers/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-13 10:13:26.388883 steam-sdk-2024.5.2/steam_sdk/wrappers/java/
+drwxrwxrwx   0        0        0        0 2024-05-13 10:13:26.389882 steam-sdk-2024.5.2/steam_sdk/wrappers/java/SING/
+-rw-rw-rw-   0        0        0        0 2022-02-23 07:50:41.000000 steam-sdk-2024.5.2/steam_sdk/wrappers/java/SING/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-13 10:13:26.390883 steam-sdk-2024.5.2/steam_sdk/wrappers/java/SING/jars/
+-rw-rw-rw-   0        0        0        0 2022-02-23 07:50:41.000000 steam-sdk-2024.5.2/steam_sdk/wrappers/java/SING/jars/__init__.py
+-rw-rw-rw-   0        0        0        0 2022-02-23 07:50:41.000000 steam-sdk-2024.5.2/steam_sdk/wrappers/java/__init__.py
+-rw-rw-rw-   0        0        0     1830 2024-01-10 12:13:04.000000 steam-sdk-2024.5.2/steam_sdk/wrappers/wrapper_yaml.py
+drwxrwxrwx   0        0        0        0 2024-05-13 10:13:26.391890 steam-sdk-2024.5.2/steam_sdk.egg-info/
+-rw-rw-rw-   0        0        0     5753 2024-05-13 10:13:25.000000 steam-sdk-2024.5.2/steam_sdk.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     7888 2024-05-13 10:13:26.000000 steam-sdk-2024.5.2/steam_sdk.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-13 10:13:25.000000 steam-sdk-2024.5.2/steam_sdk.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0     1745 2024-05-13 10:13:25.000000 steam-sdk-2024.5.2/steam_sdk.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       16 2024-05-13 10:13:25.000000 steam-sdk-2024.5.2/steam_sdk.egg-info/top_level.txt
```

### Comparing `steam-sdk-2024.5.1/PKG-INFO` & `steam-sdk-2024.5.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 Metadata-Version: 2.1
 Name: steam-sdk
-Version: 2024.5.1
+Version: 2024.5.2
 Summary: Source code for APIs for STEAM tools.
 Home-page: https://gitlab.cern.ch/steam/steam_sdk
 Author: STEAM Team
 Author-email: steam-team@cern.ch
-Keywords: SDK,STEAM,CERN,API
+Keywords: STEAM,SDK,CERN,API
 Classifier: Programming Language :: Python :: 3.11
 Requires-Python: >=3.11
 Description-Content-Type: text/markdown
 Requires-Dist: gmsh==4.11.1
 Requires-Dist: matplotlib==3.8.3
 Requires-Dist: Jinja2==3.1.3
 Requires-Dist: numpy==1.26.4
```

### Comparing `steam-sdk-2024.5.1/setup.py` & `steam-sdk-2024.5.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -33,15 +33,15 @@
 
 build_require = ["setuptools==69.2.0"]
 
 all_requirements = required + docs_require + tests_require + build_require
 
 setup(
     name="steam-sdk",
-    version="2024.5.1",
+    version="2024.5.2",
     author="STEAM Team",
     author_email="steam-team@cern.ch",
     description="Source code for APIs for STEAM tools.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://gitlab.cern.ch/steam/steam_sdk",
     keywords={"STEAM", "API", "SDK", "CERN"},
```

### Comparing `steam-sdk-2024.5.1/steam_sdk/analyses/AnalysisEvent.py` & `steam-sdk-2024.5.2/steam_sdk/analyses/AnalysisEvent.py`

 * *Files identical despite different names*

### Comparing `steam-sdk-2024.5.1/steam_sdk/analyses/AnalysisEventLHC.py` & `steam-sdk-2024.5.2/steam_sdk/analyses/AnalysisEventLHC.py`

 * *Files identical despite different names*

### Comparing `steam-sdk-2024.5.1/steam_sdk/analyses/AnalysisSTEAM.py` & `steam-sdk-2024.5.2/steam_sdk/analyses/AnalysisSTEAM.py`

 * *Files 0% similar despite different names*

```diff
@@ -989,15 +989,15 @@
         """
         Set up a APDL_CT model in the local APDL_CT working folder
         Note: The sim_number is assigned to the subfolder name, not to the file name
         """
         verbose = verbose if verbose is not None else self.verbose  # if verbose is not defined, take its value from self
 
         local_model_folder = os.path.join(self.settings.local_ANSYS_folder, simulation_name, str(sim_number))
-        BM.buildAPDL_CT(sim_name=simulation_name, sim_number='', output_path=local_model_folder, flag_plot_all=flag_plot_all, verbose=verbose)
+        BM.buildAPDL_CT(sim_name=simulation_name, sim_number=sim_number, output_path=local_model_folder, flag_plot_all=flag_plot_all, verbose=verbose)
 
         # Add simulation number to the list
         self.list_sims.append(sim_number)
 
         return BM
 
     def setup_sim_COSIM(self, BM: BuilderCosim, simulation_name, sim_number, verbose: bool = None):
```

### Comparing `steam-sdk-2024.5.1/steam_sdk/analyses/custom_analyses/analysis_short_circuit_LEDET_1/analysis_short_circuit_LEDET_1.py` & `steam-sdk-2024.5.2/steam_sdk/analyses/custom_analyses/analysis_short_circuit_LEDET_1/analysis_short_circuit_LEDET_1.py`

 * *Files identical despite different names*

### Comparing `steam-sdk-2024.5.1/steam_sdk/analyses/custom_analyses/analysis_short_circuit_LEDET_1/utils/calculate_short_parameters.py` & `steam-sdk-2024.5.2/steam_sdk/analyses/custom_analyses/analysis_short_circuit_LEDET_1/utils/calculate_short_parameters.py`

 * *Files identical despite different names*

### Comparing `steam-sdk-2024.5.1/steam_sdk/analyses/custom_analyses/analysis_short_circuit_LEDET_1/utils/copy_input_files.py` & `steam-sdk-2024.5.2/steam_sdk/analyses/custom_analyses/analysis_short_circuit_LEDET_1/utils/copy_input_files.py`

 * *Files identical despite different names*

### Comparing `steam-sdk-2024.5.1/steam_sdk/analyses/custom_analyses/analysis_short_circuit_LEDET_1/utils/set_common_parameters.py` & `steam-sdk-2024.5.2/steam_sdk/analyses/custom_analyses/analysis_short_circuit_LEDET_1/utils/set_common_parameters.py`

 * *Files identical despite different names*

### Comparing `steam-sdk-2024.5.1/steam_sdk/analyses/custom_analyses/analysis_short_circuit_LEDET_1/utils/set_magnet_specific_parameters.py` & `steam-sdk-2024.5.2/steam_sdk/analyses/custom_analyses/analysis_short_circuit_LEDET_1/utils/set_magnet_specific_parameters.py`

 * *Files identical despite different names*

### Comparing `steam-sdk-2024.5.1/steam_sdk/analyses/custom_analyses/analysis_short_circuit_LEDET_1/utils/set_short_circuit_analysis_parameters.py` & `steam-sdk-2024.5.2/steam_sdk/analyses/custom_analyses/analysis_short_circuit_LEDET_1/utils/set_short_circuit_analysis_parameters.py`

 * *Files identical despite different names*

### Comparing `steam-sdk-2024.5.1/steam_sdk/analyses/custom_analyses/analysis_short_circuit_LEDET_1/utils/set_simulations_to_prepare_run.py` & `steam-sdk-2024.5.2/steam_sdk/analyses/custom_analyses/analysis_short_circuit_LEDET_1/utils/set_simulations_to_prepare_run.py`

 * *Files identical despite different names*

### Comparing `steam-sdk-2024.5.1/steam_sdk/analyses/custom_analyses/co_simulation_QH_PyBBQ_LEDET_1/co_simulation_QH_PyBBQ_LEDET_1.py` & `steam-sdk-2024.5.2/steam_sdk/analyses/custom_analyses/co_simulation_QH_PyBBQ_LEDET_1/co_simulation_QH_PyBBQ_LEDET_1.py`

 * *Files identical despite different names*

### Comparing `steam-sdk-2024.5.1/steam_sdk/analyses/custom_analyses/co_simulation_QH_PyBBQ_LEDET_1/utils/calculate_quench_propagation_velocity.py` & `steam-sdk-2024.5.2/steam_sdk/analyses/custom_analyses/co_simulation_QH_PyBBQ_LEDET_1/utils/calculate_quench_propagation_velocity.py`

 * *Files identical despite different names*

### Comparing `steam-sdk-2024.5.1/steam_sdk/analyses/custom_analyses/co_simulation_QH_PyBBQ_LEDET_1/utils/create_conductor_analysis_file.py` & `steam-sdk-2024.5.2/steam_sdk/analyses/custom_analyses/co_simulation_QH_PyBBQ_LEDET_1/utils/create_conductor_analysis_file.py`

 * *Files identical despite different names*

### Comparing `steam-sdk-2024.5.1/steam_sdk/analyses/custom_analyses/co_simulation_QH_PyBBQ_LEDET_1/utils/create_magnet_analysis_file.py` & `steam-sdk-2024.5.2/steam_sdk/analyses/custom_analyses/co_simulation_QH_PyBBQ_LEDET_1/utils/create_magnet_analysis_file.py`

 * *Files identical despite different names*

### Comparing `steam-sdk-2024.5.1/steam_sdk/analyses/custom_analyses/co_simulation_QH_PyBBQ_LEDET_MBRD_validation_1/co_simulation_QH_PyBBQ_LEDET_MBRD_validation_1.py` & `steam-sdk-2024.5.2/steam_sdk/analyses/custom_analyses/co_simulation_QH_PyBBQ_LEDET_MBRD_validation_1/co_simulation_QH_PyBBQ_LEDET_MBRD_validation_1.py`

 * *Files identical despite different names*

### Comparing `steam-sdk-2024.5.1/steam_sdk/analyses/custom_analyses/co_simulation_QH_PyBBQ_LEDET_MBRD_validation_1/utils/calculate_quench_propagation_velocity.py` & `steam-sdk-2024.5.2/steam_sdk/analyses/custom_analyses/co_simulation_QH_PyBBQ_LEDET_MBRD_validation_1/utils/calculate_quench_propagation_velocity.py`

 * *Files identical despite different names*

### Comparing `steam-sdk-2024.5.1/steam_sdk/analyses/custom_analyses/co_simulation_QH_PyBBQ_LEDET_MBRD_validation_1/utils/create_conductor_analysis_file.py` & `steam-sdk-2024.5.2/steam_sdk/analyses/custom_analyses/co_simulation_QH_PyBBQ_LEDET_MBRD_validation_1/utils/create_conductor_analysis_file.py`

 * *Files identical despite different names*

### Comparing `steam-sdk-2024.5.1/steam_sdk/analyses/custom_analyses/co_simulation_QH_PyBBQ_LEDET_MBRD_validation_1/utils/create_magnet_analysis_file.py` & `steam-sdk-2024.5.2/steam_sdk/analyses/custom_analyses/co_simulation_QH_PyBBQ_LEDET_MBRD_validation_1/utils/create_magnet_analysis_file.py`

 * *Files identical despite different names*

### Comparing `steam-sdk-2024.5.1/steam_sdk/analyses/custom_analyses/custom_function_test_1/custom_function_test_1.py` & `steam-sdk-2024.5.2/steam_sdk/analyses/custom_analyses/custom_function_test_1/custom_function_test_1.py`

 * *Files identical despite different names*

### Comparing `steam-sdk-2024.5.1/steam_sdk/builders/BuilderAPDL_CT.py` & `steam-sdk-2024.5.2/steam_sdk/builders/BuilderAPDL_CT.py`

 * *Files identical despite different names*

### Comparing `steam-sdk-2024.5.1/steam_sdk/builders/BuilderCosim.py` & `steam-sdk-2024.5.2/steam_sdk/builders/BuilderCosim.py`

 * *Files identical despite different names*

### Comparing `steam-sdk-2024.5.1/steam_sdk/builders/BuilderFiQuS.py` & `steam-sdk-2024.5.2/steam_sdk/builders/BuilderFiQuS.py`

 * *Files identical despite different names*

### Comparing `steam-sdk-2024.5.1/steam_sdk/builders/BuilderLEDET.py` & `steam-sdk-2024.5.2/steam_sdk/builders/BuilderLEDET.py`

 * *Files identical despite different names*

### Comparing `steam-sdk-2024.5.1/steam_sdk/builders/BuilderModel.py` & `steam-sdk-2024.5.2/steam_sdk/builders/BuilderModel.py`

 * *Files identical despite different names*

### Comparing `steam-sdk-2024.5.1/steam_sdk/builders/BuilderProteCCT.py` & `steam-sdk-2024.5.2/steam_sdk/builders/BuilderProteCCT.py`

 * *Files identical despite different names*

### Comparing `steam-sdk-2024.5.1/steam_sdk/builders/BuilderPyBBQ.py` & `steam-sdk-2024.5.2/steam_sdk/builders/BuilderPyBBQ.py`

 * *Files identical despite different names*

### Comparing `steam-sdk-2024.5.1/steam_sdk/builders/BuilderPySIGMA.py` & `steam-sdk-2024.5.2/steam_sdk/builders/BuilderPySIGMA.py`

 * *Files identical despite different names*

### Comparing `steam-sdk-2024.5.1/steam_sdk/builders/BuilderTFM.py` & `steam-sdk-2024.5.2/steam_sdk/builders/BuilderTFM.py`

 * *Files identical despite different names*

### Comparing `steam-sdk-2024.5.1/steam_sdk/builders/SelfMutualInductanceCalculation.py` & `steam-sdk-2024.5.2/steam_sdk/builders/SelfMutualInductanceCalculation.py`

 * *Files identical despite different names*

### Comparing `steam-sdk-2024.5.1/steam_sdk/builders/Solenoids.py` & `steam-sdk-2024.5.2/steam_sdk/builders/Solenoids.py`

 * *Files identical despite different names*

### Comparing `steam-sdk-2024.5.1/steam_sdk/builders/geometricFunctions.py` & `steam-sdk-2024.5.2/steam_sdk/builders/geometricFunctions.py`

 * *Files identical despite different names*

### Comparing `steam-sdk-2024.5.1/steam_sdk/configs/tools_defaults/ToolDefaultReader.py` & `steam-sdk-2024.5.2/steam_sdk/configs/tools_defaults/ToolDefaultReader.py`

 * *Files identical despite different names*

### Comparing `steam-sdk-2024.5.1/steam_sdk/cosims/CoSimPyCoSim.py` & `steam-sdk-2024.5.2/steam_sdk/cosims/CoSimPyCoSim.py`

 * *Files identical despite different names*

### Comparing `steam-sdk-2024.5.1/steam_sdk/data/DataAPDLCTOptions.py` & `steam-sdk-2024.5.2/steam_sdk/data/DataAPDLCTOptions.py`

 * *Files identical despite different names*

### Comparing `steam-sdk-2024.5.1/steam_sdk/data/DataAnalysis.py` & `steam-sdk-2024.5.2/steam_sdk/data/DataAnalysis.py`

 * *Files identical despite different names*

### Comparing `steam-sdk-2024.5.1/steam_sdk/data/DataConductor.py` & `steam-sdk-2024.5.2/steam_sdk/data/DataConductor.py`

 * *Files identical despite different names*

### Comparing `steam-sdk-2024.5.1/steam_sdk/data/DataEventCircuit.py` & `steam-sdk-2024.5.2/steam_sdk/data/DataEventCircuit.py`

 * *Files identical despite different names*

### Comparing `steam-sdk-2024.5.1/steam_sdk/data/DataEventMagnet.py` & `steam-sdk-2024.5.2/steam_sdk/data/DataEventMagnet.py`

 * *Files identical despite different names*

### Comparing `steam-sdk-2024.5.1/steam_sdk/data/DataFiQuS.py` & `steam-sdk-2024.5.2/steam_sdk/data/DataFiQuS.py`

 * *Files identical despite different names*

### Comparing `steam-sdk-2024.5.1/steam_sdk/data/DataFiQuSOptions.py` & `steam-sdk-2024.5.2/steam_sdk/data/DataFiQuSOptions.py`

 * *Files identical despite different names*

### Comparing `steam-sdk-2024.5.1/steam_sdk/data/DataLEDET.py` & `steam-sdk-2024.5.2/steam_sdk/data/DataLEDET.py`

 * *Files identical despite different names*

### Comparing `steam-sdk-2024.5.1/steam_sdk/data/DataLEDETOptions.py` & `steam-sdk-2024.5.2/steam_sdk/data/DataLEDETOptions.py`

 * *Files identical despite different names*

### Comparing `steam-sdk-2024.5.1/steam_sdk/data/DataModelCircuit.py` & `steam-sdk-2024.5.2/steam_sdk/data/DataModelCircuit.py`

 * *Files identical despite different names*

### Comparing `steam-sdk-2024.5.1/steam_sdk/data/DataModelCommon.py` & `steam-sdk-2024.5.2/steam_sdk/data/DataModelCommon.py`

 * *Files identical despite different names*

### Comparing `steam-sdk-2024.5.1/steam_sdk/data/DataModelConductor.py` & `steam-sdk-2024.5.2/steam_sdk/data/DataModelConductor.py`

 * *Files identical despite different names*

### Comparing `steam-sdk-2024.5.1/steam_sdk/data/DataModelCosim.py` & `steam-sdk-2024.5.2/steam_sdk/data/DataModelCosim.py`

 * *Files identical despite different names*

### Comparing `steam-sdk-2024.5.1/steam_sdk/data/DataModelMagnet.py` & `steam-sdk-2024.5.2/steam_sdk/data/DataModelMagnet.py`

 * *Files identical despite different names*

### Comparing `steam-sdk-2024.5.1/steam_sdk/data/DataModelParsimDakota.py` & `steam-sdk-2024.5.2/steam_sdk/data/DataModelParsimDakota.py`

 * *Files identical despite different names*

### Comparing `steam-sdk-2024.5.1/steam_sdk/data/DataParsimConductor.py` & `steam-sdk-2024.5.2/steam_sdk/data/DataParsimConductor.py`

 * *Files identical despite different names*

### Comparing `steam-sdk-2024.5.1/steam_sdk/data/DataPlot.py` & `steam-sdk-2024.5.2/steam_sdk/data/DataPlot.py`

 * *Files identical despite different names*

### Comparing `steam-sdk-2024.5.1/steam_sdk/data/DataProteCCT.py` & `steam-sdk-2024.5.2/steam_sdk/data/DataProteCCT.py`

 * *Files identical despite different names*

### Comparing `steam-sdk-2024.5.1/steam_sdk/data/DataProteCCTOptions.py` & `steam-sdk-2024.5.2/steam_sdk/data/DataProteCCTOptions.py`

 * *Files identical despite different names*

### Comparing `steam-sdk-2024.5.1/steam_sdk/data/DataPyBBQ.py` & `steam-sdk-2024.5.2/steam_sdk/data/DataPyBBQ.py`

 * *Files identical despite different names*

### Comparing `steam-sdk-2024.5.1/steam_sdk/data/DataPyBBQOptions.py` & `steam-sdk-2024.5.2/steam_sdk/data/DataPyBBQOptions.py`

 * *Files identical despite different names*

### Comparing `steam-sdk-2024.5.1/steam_sdk/data/DataPyCoSim.py` & `steam-sdk-2024.5.2/steam_sdk/data/DataPyCoSim.py`

 * *Files identical despite different names*

### Comparing `steam-sdk-2024.5.1/steam_sdk/data/DataPySIGMA.py` & `steam-sdk-2024.5.2/steam_sdk/data/DataPySIGMA.py`

 * *Files identical despite different names*

### Comparing `steam-sdk-2024.5.1/steam_sdk/data/DataPySIGMAOptions.py` & `steam-sdk-2024.5.2/steam_sdk/data/DataPySIGMAOptions.py`

 * *Files identical despite different names*

### Comparing `steam-sdk-2024.5.1/steam_sdk/data/DataRoxieParser.py` & `steam-sdk-2024.5.2/steam_sdk/data/DataRoxieParser.py`

 * *Files identical despite different names*

### Comparing `steam-sdk-2024.5.1/steam_sdk/data/DataSettings.py` & `steam-sdk-2024.5.2/steam_sdk/data/DataSettings.py`

 * *Files identical despite different names*

### Comparing `steam-sdk-2024.5.1/steam_sdk/data/DataSignal.py` & `steam-sdk-2024.5.2/steam_sdk/data/DataSignal.py`

 * *Files identical despite different names*

### Comparing `steam-sdk-2024.5.1/steam_sdk/data/DataTFM.py` & `steam-sdk-2024.5.2/steam_sdk/data/DataTFM.py`

 * *Files identical despite different names*

### Comparing `steam-sdk-2024.5.1/steam_sdk/data/DictionaryLEDET.py` & `steam-sdk-2024.5.2/steam_sdk/data/DictionaryLEDET.py`

 * *Files identical despite different names*

### Comparing `steam-sdk-2024.5.1/steam_sdk/data/DictionaryProteCCT.py` & `steam-sdk-2024.5.2/steam_sdk/data/DictionaryProteCCT.py`

 * *Files identical despite different names*

### Comparing `steam-sdk-2024.5.1/steam_sdk/data/DictionaryPyBBQ.py` & `steam-sdk-2024.5.2/steam_sdk/data/DictionaryPyBBQ.py`

 * *Files identical despite different names*

### Comparing `steam-sdk-2024.5.1/steam_sdk/data/TemplateLEDET.py` & `steam-sdk-2024.5.2/steam_sdk/data/TemplateLEDET.py`

 * *Files identical despite different names*

### Comparing `steam-sdk-2024.5.1/steam_sdk/data/TemplateProteCCT.py` & `steam-sdk-2024.5.2/steam_sdk/data/TemplateProteCCT.py`

 * *Files identical despite different names*

### Comparing `steam-sdk-2024.5.1/steam_sdk/drivers/DriverANSYS.py` & `steam-sdk-2024.5.2/steam_sdk/drivers/DriverANSYS.py`

 * *Files identical despite different names*

### Comparing `steam-sdk-2024.5.1/steam_sdk/drivers/DriverAnalysis.py` & `steam-sdk-2024.5.2/steam_sdk/drivers/DriverAnalysis.py`

 * *Files identical despite different names*

### Comparing `steam-sdk-2024.5.1/steam_sdk/drivers/DriverDakota.py` & `steam-sdk-2024.5.2/steam_sdk/drivers/DriverDakota.py`

 * *Files identical despite different names*

### Comparing `steam-sdk-2024.5.1/steam_sdk/drivers/DriverFiQuS.py` & `steam-sdk-2024.5.2/steam_sdk/drivers/DriverFiQuS.py`

 * *Files identical despite different names*

### Comparing `steam-sdk-2024.5.1/steam_sdk/drivers/DriverLEDET.py` & `steam-sdk-2024.5.2/steam_sdk/drivers/DriverLEDET.py`

 * *Files identical despite different names*

### Comparing `steam-sdk-2024.5.1/steam_sdk/drivers/DriverPSPICE.py` & `steam-sdk-2024.5.2/steam_sdk/drivers/DriverPSPICE.py`

 * *Files identical despite different names*

### Comparing `steam-sdk-2024.5.1/steam_sdk/drivers/DriverProteCCT.py` & `steam-sdk-2024.5.2/steam_sdk/drivers/DriverProteCCT.py`

 * *Files identical despite different names*

### Comparing `steam-sdk-2024.5.1/steam_sdk/drivers/DriverPyBBQ.py` & `steam-sdk-2024.5.2/steam_sdk/drivers/DriverPyBBQ.py`

 * *Files identical despite different names*

### Comparing `steam-sdk-2024.5.1/steam_sdk/drivers/DriverPySIGMA.py` & `steam-sdk-2024.5.2/steam_sdk/drivers/DriverPySIGMA.py`

 * *Files identical despite different names*

### Comparing `steam-sdk-2024.5.1/steam_sdk/drivers/DriverXYCE.py` & `steam-sdk-2024.5.2/steam_sdk/drivers/DriverXYCE.py`

 * *Files identical despite different names*

### Comparing `steam-sdk-2024.5.1/steam_sdk/drivers/to_DELETE.py` & `steam-sdk-2024.5.2/steam_sdk/drivers/to_DELETE.py`

 * *Files identical despite different names*

### Comparing `steam-sdk-2024.5.1/steam_sdk/parsers/CSD_Reader.py` & `steam-sdk-2024.5.2/steam_sdk/parsers/CSD_Reader.py`

 * *Files identical despite different names*

### Comparing `steam-sdk-2024.5.1/steam_sdk/parsers/ParserCOSIM.py` & `steam-sdk-2024.5.2/steam_sdk/parsers/ParserCOSIM.py`

 * *Files identical despite different names*

### Comparing `steam-sdk-2024.5.1/steam_sdk/parsers/ParserCond2d.py` & `steam-sdk-2024.5.2/steam_sdk/parsers/ParserCond2d.py`

 * *Files identical despite different names*

### Comparing `steam-sdk-2024.5.1/steam_sdk/parsers/ParserCsd.py` & `steam-sdk-2024.5.2/steam_sdk/parsers/ParserCsd.py`

 * *Files identical despite different names*

### Comparing `steam-sdk-2024.5.1/steam_sdk/parsers/ParserCsv.py` & `steam-sdk-2024.5.2/steam_sdk/parsers/ParserCsv.py`

 * *Files identical despite different names*

### Comparing `steam-sdk-2024.5.1/steam_sdk/parsers/ParserDakota.py` & `steam-sdk-2024.5.2/steam_sdk/parsers/ParserDakota.py`

 * *Files identical despite different names*

### Comparing `steam-sdk-2024.5.1/steam_sdk/parsers/ParserExcel.py` & `steam-sdk-2024.5.2/steam_sdk/parsers/ParserExcel.py`

 * *Files identical despite different names*

### Comparing `steam-sdk-2024.5.1/steam_sdk/parsers/ParserFiQuS.py` & `steam-sdk-2024.5.2/steam_sdk/parsers/ParserFiQuS.py`

 * *Files identical despite different names*

### Comparing `steam-sdk-2024.5.1/steam_sdk/parsers/ParserFile.py` & `steam-sdk-2024.5.2/steam_sdk/parsers/ParserFile.py`

 * *Files identical despite different names*

### Comparing `steam-sdk-2024.5.1/steam_sdk/parsers/ParserLEDET.py` & `steam-sdk-2024.5.2/steam_sdk/parsers/ParserLEDET.py`

 * *Files identical despite different names*

### Comparing `steam-sdk-2024.5.1/steam_sdk/parsers/ParserMap2d.py` & `steam-sdk-2024.5.2/steam_sdk/parsers/ParserMap2d.py`

 * *Files identical despite different names*

### Comparing `steam-sdk-2024.5.1/steam_sdk/parsers/ParserMat.py` & `steam-sdk-2024.5.2/steam_sdk/parsers/ParserMat.py`

 * *Files identical despite different names*

### Comparing `steam-sdk-2024.5.1/steam_sdk/parsers/ParserPSPICE.py` & `steam-sdk-2024.5.2/steam_sdk/parsers/ParserPSPICE.py`

 * *Files identical despite different names*

### Comparing `steam-sdk-2024.5.1/steam_sdk/parsers/ParserPdf.py` & `steam-sdk-2024.5.2/steam_sdk/parsers/ParserPdf.py`

 * *Files identical despite different names*

### Comparing `steam-sdk-2024.5.1/steam_sdk/parsers/ParserProteCCT.py` & `steam-sdk-2024.5.2/steam_sdk/parsers/ParserProteCCT.py`

 * *Files identical despite different names*

### Comparing `steam-sdk-2024.5.1/steam_sdk/parsers/ParserPyBBQ.py` & `steam-sdk-2024.5.2/steam_sdk/parsers/ParserPyBBQ.py`

 * *Files identical despite different names*

### Comparing `steam-sdk-2024.5.1/steam_sdk/parsers/ParserPyCoSim.py` & `steam-sdk-2024.5.2/steam_sdk/parsers/ParserPyCoSim.py`

 * *Files identical despite different names*

### Comparing `steam-sdk-2024.5.1/steam_sdk/parsers/ParserPySIGMA.py` & `steam-sdk-2024.5.2/steam_sdk/parsers/ParserPySIGMA.py`

 * *Files identical despite different names*

### Comparing `steam-sdk-2024.5.1/steam_sdk/parsers/ParserRoxie.py` & `steam-sdk-2024.5.2/steam_sdk/parsers/ParserRoxie.py`

 * *Files identical despite different names*

### Comparing `steam-sdk-2024.5.1/steam_sdk/parsers/ParserTdms.py` & `steam-sdk-2024.5.2/steam_sdk/parsers/ParserTdms.py`

 * *Files identical despite different names*

### Comparing `steam-sdk-2024.5.1/steam_sdk/parsers/ParserXYCE.py` & `steam-sdk-2024.5.2/steam_sdk/parsers/ParserXYCE.py`

 * *Files identical despite different names*

### Comparing `steam-sdk-2024.5.1/steam_sdk/parsers/ParserYAML.py` & `steam-sdk-2024.5.2/steam_sdk/parsers/ParserYAML.py`

 * *Files identical despite different names*

### Comparing `steam-sdk-2024.5.1/steam_sdk/parsers/utils_ParserCircuits.py` & `steam-sdk-2024.5.2/steam_sdk/parsers/utils_ParserCircuits.py`

 * *Files identical despite different names*

### Comparing `steam-sdk-2024.5.1/steam_sdk/parsers/utils_ParserCosims.py` & `steam-sdk-2024.5.2/steam_sdk/parsers/utils_ParserCosims.py`

 * *Files identical despite different names*

### Comparing `steam-sdk-2024.5.1/steam_sdk/parsims/ParsimConductor.py` & `steam-sdk-2024.5.2/steam_sdk/parsims/ParsimConductor.py`

 * *Files identical despite different names*

### Comparing `steam-sdk-2024.5.1/steam_sdk/parsims/ParsimDakota.py` & `steam-sdk-2024.5.2/steam_sdk/parsims/ParsimDakota.py`

 * *Files identical despite different names*

### Comparing `steam-sdk-2024.5.1/steam_sdk/parsims/ParsimEventCircuit.py` & `steam-sdk-2024.5.2/steam_sdk/parsims/ParsimEventCircuit.py`

 * *Files identical despite different names*

### Comparing `steam-sdk-2024.5.1/steam_sdk/parsims/ParsimEventMagnet.py` & `steam-sdk-2024.5.2/steam_sdk/parsims/ParsimEventMagnet.py`

 * *Files identical despite different names*

### Comparing `steam-sdk-2024.5.1/steam_sdk/parsims/translation_dicts/conductor_column_names.yaml` & `steam-sdk-2024.5.2/steam_sdk/parsims/translation_dicts/conductor_column_names.yaml`

 * *Files identical despite different names*

### Comparing `steam-sdk-2024.5.1/steam_sdk/parsims/translation_dicts/event_column_names.yaml` & `steam-sdk-2024.5.2/steam_sdk/parsims/translation_dicts/event_column_names.yaml`

 * *Files identical despite different names*

### Comparing `steam-sdk-2024.5.1/steam_sdk/plotters/PlotterAnalysis.py` & `steam-sdk-2024.5.2/steam_sdk/plotters/PlotterAnalysis.py`

 * *Files identical despite different names*

### Comparing `steam-sdk-2024.5.1/steam_sdk/plotters/PlotterGriddedData.py` & `steam-sdk-2024.5.2/steam_sdk/plotters/PlotterGriddedData.py`

 * *Files identical despite different names*

### Comparing `steam-sdk-2024.5.1/steam_sdk/plotters/PlotterMap2d.py` & `steam-sdk-2024.5.2/steam_sdk/plotters/PlotterMap2d.py`

 * *Files identical despite different names*

### Comparing `steam-sdk-2024.5.1/steam_sdk/plotters/PlotterModel.py` & `steam-sdk-2024.5.2/steam_sdk/plotters/PlotterModel.py`

 * *Files identical despite different names*

### Comparing `steam-sdk-2024.5.1/steam_sdk/plotters/PlotterParametric.py` & `steam-sdk-2024.5.2/steam_sdk/plotters/PlotterParametric.py`

 * *Files identical despite different names*

### Comparing `steam-sdk-2024.5.1/steam_sdk/plotters/PlotterRoxie.py` & `steam-sdk-2024.5.2/steam_sdk/plotters/PlotterRoxie.py`

 * *Files identical despite different names*

### Comparing `steam-sdk-2024.5.1/steam_sdk/postprocs/PostprocsMetrics.py` & `steam-sdk-2024.5.2/steam_sdk/postprocs/PostprocsMetrics.py`

 * *Files identical despite different names*

### Comparing `steam-sdk-2024.5.1/steam_sdk/utils/MTF_reading_functions.py` & `steam-sdk-2024.5.2/steam_sdk/utils/MTF_reading_functions.py`

 * *Files identical despite different names*

### Comparing `steam-sdk-2024.5.1/steam_sdk/utils/ModifyModelData.py` & `steam-sdk-2024.5.2/steam_sdk/utils/ModifyModelData.py`

 * *Files identical despite different names*

### Comparing `steam-sdk-2024.5.1/steam_sdk/utils/ModifyModelDataMagnet.py` & `steam-sdk-2024.5.2/steam_sdk/utils/ModifyModelDataMagnet.py`

 * *Files identical despite different names*

### Comparing `steam-sdk-2024.5.1/steam_sdk/utils/ModifyModelDataconductor.py` & `steam-sdk-2024.5.2/steam_sdk/utils/ModifyModelDataconductor.py`

 * *Files identical despite different names*

### Comparing `steam-sdk-2024.5.1/steam_sdk/utils/ParserRoxieHelpers.py` & `steam-sdk-2024.5.2/steam_sdk/utils/ParserRoxieHelpers.py`

 * *Files identical despite different names*

### Comparing `steam-sdk-2024.5.1/steam_sdk/utils/attribute_model.py` & `steam-sdk-2024.5.2/steam_sdk/utils/attribute_model.py`

 * *Files identical despite different names*

### Comparing `steam-sdk-2024.5.1/steam_sdk/utils/clean_NaN_from_signal.py` & `steam-sdk-2024.5.2/steam_sdk/utils/clean_NaN_from_signal.py`

 * *Files identical despite different names*

### Comparing `steam-sdk-2024.5.1/steam_sdk/utils/compare_simulations.py` & `steam-sdk-2024.5.2/steam_sdk/utils/compare_simulations.py`

 * *Files identical despite different names*

### Comparing `steam-sdk-2024.5.1/steam_sdk/utils/compare_two_parameters.py` & `steam-sdk-2024.5.2/steam_sdk/utils/compare_two_parameters.py`

 * *Files identical despite different names*

### Comparing `steam-sdk-2024.5.1/steam_sdk/utils/correct_RRR_NIST.py` & `steam-sdk-2024.5.2/steam_sdk/utils/correct_RRR_NIST.py`

 * *Files identical despite different names*

### Comparing `steam-sdk-2024.5.1/steam_sdk/utils/find_delete_files.py` & `steam-sdk-2024.5.2/steam_sdk/utils/find_delete_files.py`

 * *Files identical despite different names*

### Comparing `steam-sdk-2024.5.1/steam_sdk/utils/get_attribute_type.py` & `steam-sdk-2024.5.2/steam_sdk/utils/get_attribute_type.py`

 * *Files identical despite different names*

### Comparing `steam-sdk-2024.5.1/steam_sdk/utils/make_folder_if_not_existing.py` & `steam-sdk-2024.5.2/steam_sdk/utils/make_folder_if_not_existing.py`

 * *Files identical despite different names*

### Comparing `steam-sdk-2024.5.1/steam_sdk/utils/make_json_schema.py` & `steam-sdk-2024.5.2/steam_sdk/utils/make_json_schema.py`

 * *Files identical despite different names*

### Comparing `steam-sdk-2024.5.1/steam_sdk/utils/misc.py` & `steam-sdk-2024.5.2/steam_sdk/utils/misc.py`

 * *Files identical despite different names*

### Comparing `steam-sdk-2024.5.1/steam_sdk/utils/overwrite_files.py` & `steam-sdk-2024.5.2/steam_sdk/utils/overwrite_files.py`

 * *Files identical despite different names*

### Comparing `steam-sdk-2024.5.1/steam_sdk/utils/overwrite_output_to_reference_files.py` & `steam-sdk-2024.5.2/steam_sdk/utils/overwrite_output_to_reference_files.py`

 * *Files identical despite different names*

### Comparing `steam-sdk-2024.5.1/steam_sdk/utils/parse_str_to_list.py` & `steam-sdk-2024.5.2/steam_sdk/utils/parse_str_to_list.py`

 * *Files identical despite different names*

### Comparing `steam-sdk-2024.5.1/steam_sdk/utils/read_settings_file.py` & `steam-sdk-2024.5.2/steam_sdk/utils/read_settings_file.py`

 * *Files identical despite different names*

### Comparing `steam-sdk-2024.5.1/steam_sdk/utils/reformat_figure.py` & `steam-sdk-2024.5.2/steam_sdk/utils/reformat_figure.py`

 * *Files identical despite different names*

### Comparing `steam-sdk-2024.5.1/steam_sdk/utils/tic_toc.py` & `steam-sdk-2024.5.2/steam_sdk/utils/tic_toc.py`

 * *Files identical despite different names*

### Comparing `steam-sdk-2024.5.1/steam_sdk/utils/utils_PC.py` & `steam-sdk-2024.5.2/steam_sdk/utils/utils_PC.py`

 * *Files identical despite different names*

### Comparing `steam-sdk-2024.5.1/steam_sdk/viewers/Viewer.py` & `steam-sdk-2024.5.2/steam_sdk/viewers/Viewer.py`

 * *Files identical despite different names*

### Comparing `steam-sdk-2024.5.1/steam_sdk/wrappers/wrapper_yaml.py` & `steam-sdk-2024.5.2/steam_sdk/wrappers/wrapper_yaml.py`

 * *Files identical despite different names*

### Comparing `steam-sdk-2024.5.1/steam_sdk.egg-info/PKG-INFO` & `steam-sdk-2024.5.2/steam_sdk.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 Metadata-Version: 2.1
 Name: steam-sdk
-Version: 2024.5.1
+Version: 2024.5.2
 Summary: Source code for APIs for STEAM tools.
 Home-page: https://gitlab.cern.ch/steam/steam_sdk
 Author: STEAM Team
 Author-email: steam-team@cern.ch
-Keywords: SDK,STEAM,CERN,API
+Keywords: STEAM,SDK,CERN,API
 Classifier: Programming Language :: Python :: 3.11
 Requires-Python: >=3.11
 Description-Content-Type: text/markdown
 Requires-Dist: gmsh==4.11.1
 Requires-Dist: matplotlib==3.8.3
 Requires-Dist: Jinja2==3.1.3
 Requires-Dist: numpy==1.26.4
```

### Comparing `steam-sdk-2024.5.1/steam_sdk.egg-info/SOURCES.txt` & `steam-sdk-2024.5.2/steam_sdk.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `steam-sdk-2024.5.1/steam_sdk.egg-info/requires.txt` & `steam-sdk-2024.5.2/steam_sdk.egg-info/requires.txt`

 * *Files identical despite different names*

