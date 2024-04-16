# Comparing `tmp/panda_server-0.3.3.tar.gz` & `tmp/panda_server-0.3.4.tar.gz`

## Comparing `panda_server-0.3.3.tar` & `panda_server-0.3.4.tar`

### file list

```diff
@@ -1,207 +1,207 @@
--rw-r--r--   0        0        0      461 2020-02-02 00:00:00.000000 panda_server-0.3.3/.pre-commit-config.yaml
--rw-r--r--   0        0        0    81265 2020-02-02 00:00:00.000000 panda_server-0.3.3/ChangeLog.txt
--rw-r--r--   0        0        0     4406 2020-02-02 00:00:00.000000 panda_server-0.3.3/Dockerfile
--rw-r--r--   0        0        0     2039 2020-02-02 00:00:00.000000 panda_server-0.3.3/INSTALL.md
--rw-r--r--   0        0        0     1598 2020-02-02 00:00:00.000000 panda_server-0.3.3/INSTALL_ATLAS.md
--rw-r--r--   0        0        0       64 2020-02-02 00:00:00.000000 panda_server-0.3.3/MANIFEST.in
--rw-r--r--   0        0        0       26 2020-02-02 00:00:00.000000 panda_server-0.3.3/PandaPkgInfo.py
--rw-r--r--   0        0        0     1255 2020-02-02 00:00:00.000000 panda_server-0.3.3/panda-server.spec
--rw-r--r--   0        0        0     4795 2020-02-02 00:00:00.000000 panda_server-0.3.3/package/hatch_build.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 panda_server-0.3.3/pandaserver/__init__.py
--rw-r--r--   0        0        0       99 2020-02-02 00:00:00.000000 panda_server-0.3.3/pandaserver/brokerage/ErrorCode.py
--rw-r--r--   0        0        0    16370 2020-02-02 00:00:00.000000 panda_server-0.3.3/pandaserver/brokerage/SiteMapper.py
--rwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 panda_server-0.3.3/pandaserver/brokerage/__init__.py
--rwxr-xr-x   0        0        0    85928 2020-02-02 00:00:00.000000 panda_server-0.3.3/pandaserver/brokerage/broker.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 panda_server-0.3.3/pandaserver/config/__init__.py
--rw-r--r--   0        0        0      491 2020-02-02 00:00:00.000000 panda_server-0.3.3/pandaserver/config/config_utils.py
--rw-r--r--   0        0        0      551 2020-02-02 00:00:00.000000 panda_server-0.3.3/pandaserver/config/daemon_config.py
--rwxr-xr-x   0        0        0     6900 2020-02-02 00:00:00.000000 panda_server-0.3.3/pandaserver/config/panda_config.py
--rw-r--r--   0        0        0     2435 2020-02-02 00:00:00.000000 panda_server-0.3.3/pandaserver/configurator/Carbon.py
--rw-r--r--   0        0        0    38070 2020-02-02 00:00:00.000000 panda_server-0.3.3/pandaserver/configurator/Configurator.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 panda_server-0.3.3/pandaserver/configurator/__init__.py
--rw-r--r--   0        0        0     1906 2020-02-02 00:00:00.000000 panda_server-0.3.3/pandaserver/configurator/aux.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 panda_server-0.3.3/pandaserver/daemons/__init__.py
--rw-r--r--   0        0        0     3022 2020-02-02 00:00:00.000000 panda_server-0.3.3/pandaserver/daemons/master.py
--rw-r--r--   0        0        0     2363 2020-02-02 00:00:00.000000 panda_server-0.3.3/pandaserver/daemons/master_systemd.py
--rw-r--r--   0        0        0    25423 2020-02-02 00:00:00.000000 panda_server-0.3.3/pandaserver/daemons/utils.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 panda_server-0.3.3/pandaserver/daemons/scripts/__init__.py
--rw-r--r--   0        0        0     8804 2020-02-02 00:00:00.000000 panda_server-0.3.3/pandaserver/daemons/scripts/add_main.py
--rw-r--r--   0        0        0    13604 2020-02-02 00:00:00.000000 panda_server-0.3.3/pandaserver/daemons/scripts/add_sub.py
--rw-r--r--   0        0        0     1288 2020-02-02 00:00:00.000000 panda_server-0.3.3/pandaserver/daemons/scripts/cache_pilots.py
--rw-r--r--   0        0        0    11242 2020-02-02 00:00:00.000000 panda_server-0.3.3/pandaserver/daemons/scripts/cache_schedconfig.py
--rw-r--r--   0        0        0     1455 2020-02-02 00:00:00.000000 panda_server-0.3.3/pandaserver/daemons/scripts/carbon.py
--rw-r--r--   0        0        0     3308 2020-02-02 00:00:00.000000 panda_server-0.3.3/pandaserver/daemons/scripts/configurator.py
--rw-r--r--   0        0        0    63605 2020-02-02 00:00:00.000000 panda_server-0.3.3/pandaserver/daemons/scripts/copyArchive.py
--rw-r--r--   0        0        0    53989 2020-02-02 00:00:00.000000 panda_server-0.3.3/pandaserver/daemons/scripts/datasetManager.py
--rw-r--r--   0        0        0      490 2020-02-02 00:00:00.000000 panda_server-0.3.3/pandaserver/daemons/scripts/dummy_test.py
--rw-r--r--   0        0        0     4703 2020-02-02 00:00:00.000000 panda_server-0.3.3/pandaserver/daemons/scripts/evpPD2P.py
--rw-r--r--   0        0        0    41997 2020-02-02 00:00:00.000000 panda_server-0.3.3/pandaserver/daemons/scripts/metric_collector.py
--rw-r--r--   0        0        0     2330 2020-02-02 00:00:00.000000 panda_server-0.3.3/pandaserver/daemons/scripts/panda_activeusers_query.py
--rw-r--r--   0        0        0     3305 2020-02-02 00:00:00.000000 panda_server-0.3.3/pandaserver/daemons/scripts/pilotStreaming.py
--rw-r--r--   0        0        0     5392 2020-02-02 00:00:00.000000 panda_server-0.3.3/pandaserver/daemons/scripts/process_workflow_files_daemon.py
--rw-r--r--   0        0        0     5063 2020-02-02 00:00:00.000000 panda_server-0.3.3/pandaserver/daemons/scripts/recover_lost_files_daemon.py
--rw-r--r--   0        0        0    15357 2020-02-02 00:00:00.000000 panda_server-0.3.3/pandaserver/daemons/scripts/task_evaluator.py
--rw-r--r--   0        0        0     1933 2020-02-02 00:00:00.000000 panda_server-0.3.3/pandaserver/daemons/scripts/tmpwatch.py
--rw-r--r--   0        0        0     3019 2020-02-02 00:00:00.000000 panda_server-0.3.3/pandaserver/daemons/scripts/worker_synchronization.py
--rw-r--r--   0        0        0    54210 2020-02-02 00:00:00.000000 panda_server-0.3.3/pandaserver/dataservice/AdderAtlasPlugin.py
--rw-r--r--   0        0        0      343 2020-02-02 00:00:00.000000 panda_server-0.3.3/pandaserver/dataservice/AdderDummyPlugin.py
--rw-r--r--   0        0        0    42448 2020-02-02 00:00:00.000000 panda_server-0.3.3/pandaserver/dataservice/AdderGen.py
--rw-r--r--   0        0        0      301 2020-02-02 00:00:00.000000 panda_server-0.3.3/pandaserver/dataservice/AdderPluginBase.py
--rw-r--r--   0        0        0     1074 2020-02-02 00:00:00.000000 panda_server-0.3.3/pandaserver/dataservice/AdderResult.py
--rw-r--r--   0        0        0     5999 2020-02-02 00:00:00.000000 panda_server-0.3.3/pandaserver/dataservice/AdderSimplePlugin.py
--rw-r--r--   0        0        0    13140 2020-02-02 00:00:00.000000 panda_server-0.3.3/pandaserver/dataservice/DataServiceUtils.py
--rwxr-xr-x   0        0        0      390 2020-02-02 00:00:00.000000 panda_server-0.3.3/pandaserver/dataservice/ErrorCode.py
--rw-r--r--   0        0        0     1664 2020-02-02 00:00:00.000000 panda_server-0.3.3/pandaserver/dataservice/ProcessLimiter.py
--rw-r--r--   0        0        0    10594 2020-02-02 00:00:00.000000 panda_server-0.3.3/pandaserver/dataservice/RecoverLostFilesCore.py
--rwxr-xr-x   0        0        0     8820 2020-02-02 00:00:00.000000 panda_server-0.3.3/pandaserver/dataservice/Setupper.py
--rwxr-xr-x   0        0        0   111777 2020-02-02 00:00:00.000000 panda_server-0.3.3/pandaserver/dataservice/SetupperAtlasPlugin.py
--rw-r--r--   0        0        0      638 2020-02-02 00:00:00.000000 panda_server-0.3.3/pandaserver/dataservice/SetupperDummyPlugin.py
--rw-r--r--   0        0        0     1285 2020-02-02 00:00:00.000000 panda_server-0.3.3/pandaserver/dataservice/SetupperPluginBase.py
--rwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 panda_server-0.3.3/pandaserver/dataservice/__init__.py
--rwxr-xr-x   0        0        0     2553 2020-02-02 00:00:00.000000 panda_server-0.3.3/pandaserver/dataservice/activator.py
--rwxr-xr-x   0        0        0    10782 2020-02-02 00:00:00.000000 panda_server-0.3.3/pandaserver/dataservice/closer.py
--rw-r--r--   0        0        0     3183 2020-02-02 00:00:00.000000 panda_server-0.3.3/pandaserver/dataservice/closer_atlas_plugin.py
--rwxr-xr-x   0        0        0    39928 2020-02-02 00:00:00.000000 panda_server-0.3.3/pandaserver/dataservice/ddm.py
--rw-r--r--   0        0        0     3104 2020-02-02 00:00:00.000000 panda_server-0.3.3/pandaserver/dataservice/ddm_handler.py
--rw-r--r--   0        0        0    35028 2020-02-02 00:00:00.000000 panda_server-0.3.3/pandaserver/dataservice/dyn_data_distributer.py
--rw-r--r--   0        0        0     3589 2020-02-02 00:00:00.000000 panda_server-0.3.3/pandaserver/dataservice/event_lookup_client_ei.py
--rw-r--r--   0        0        0    10398 2020-02-02 00:00:00.000000 panda_server-0.3.3/pandaserver/dataservice/event_picker.py
--rwxr-xr-x   0        0        0     7248 2020-02-02 00:00:00.000000 panda_server-0.3.3/pandaserver/dataservice/finisher.py
--rwxr-xr-x   0        0        0     2317 2020-02-02 00:00:00.000000 panda_server-0.3.3/pandaserver/dataservice/forkSetupper.py
--rw-r--r--   0        0        0     1030 2020-02-02 00:00:00.000000 panda_server-0.3.3/pandaserver/jobdispatcher/DispatcherUtils.py
--rwxr-xr-x   0        0        0      249 2020-02-02 00:00:00.000000 panda_server-0.3.3/pandaserver/jobdispatcher/ErrorCode.py
--rwxr-xr-x   0        0        0    58971 2020-02-02 00:00:00.000000 panda_server-0.3.3/pandaserver/jobdispatcher/JobDispatcher.py
--rwxr-xr-x   0        0        0    16520 2020-02-02 00:00:00.000000 panda_server-0.3.3/pandaserver/jobdispatcher/Protocol.py
--rwxr-xr-x   0        0        0     9377 2020-02-02 00:00:00.000000 panda_server-0.3.3/pandaserver/jobdispatcher/Watcher.py
--rwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 panda_server-0.3.3/pandaserver/jobdispatcher/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 panda_server-0.3.3/pandaserver/proxycache/__init__.py
--rw-r--r--   0        0        0     9933 2020-02-02 00:00:00.000000 panda_server-0.3.3/pandaserver/proxycache/panda_proxy_cache.py
--rw-r--r--   0        0        0       77 2020-02-02 00:00:00.000000 panda_server-0.3.3/pandaserver/server/.gacl
--rwxr-xr-x   0        0        0    11763 2020-02-02 00:00:00.000000 panda_server-0.3.3/pandaserver/server/panda.py
--rw-r--r--   0        0        0     5528 2020-02-02 00:00:00.000000 panda_server-0.3.3/pandaserver/srvcore/CoreUtils.py
--rwxr-xr-x   0        0        0     4014 2020-02-02 00:00:00.000000 panda_server-0.3.3/pandaserver/srvcore/MailUtils.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 panda_server-0.3.3/pandaserver/srvcore/__init__.py
--rw-r--r--   0        0        0     3446 2020-02-02 00:00:00.000000 panda_server-0.3.3/pandaserver/srvcore/allowed_methods.py
--rw-r--r--   0        0        0     4169 2020-02-02 00:00:00.000000 panda_server-0.3.3/pandaserver/srvcore/oidc_utils.py
--rw-r--r--   0        0        0     6640 2020-02-02 00:00:00.000000 panda_server-0.3.3/pandaserver/srvcore/panda_request.py
--rw-r--r--   0        0        0     1190 2020-02-02 00:00:00.000000 panda_server-0.3.3/pandaserver/srvcore/srv_msg_utils.py
--rw-r--r--   0        0        0      734 2020-02-02 00:00:00.000000 panda_server-0.3.3/pandaserver/taskbuffer/CloudSpec.py
--rw-r--r--   0        0        0     2449 2020-02-02 00:00:00.000000 panda_server-0.3.3/pandaserver/taskbuffer/CloudTaskSpec.py
--rw-r--r--   0        0        0    18693 2020-02-02 00:00:00.000000 panda_server-0.3.3/pandaserver/taskbuffer/ConBridge.py
--rwxr-xr-x   0        0        0     2583 2020-02-02 00:00:00.000000 panda_server-0.3.3/pandaserver/taskbuffer/DBProxyPool.py
--rwxr-xr-x   0        0        0     3568 2020-02-02 00:00:00.000000 panda_server-0.3.3/pandaserver/taskbuffer/DatasetSpec.py
--rw-r--r--   0        0        0     4014 2020-02-02 00:00:00.000000 panda_server-0.3.3/pandaserver/taskbuffer/DdmSpec.py
--rwxr-xr-x   0        0        0     1746 2020-02-02 00:00:00.000000 panda_server-0.3.3/pandaserver/taskbuffer/ErrorCode.py
--rw-r--r--   0        0        0    10956 2020-02-02 00:00:00.000000 panda_server-0.3.3/pandaserver/taskbuffer/EventServiceUtils.py
--rwxr-xr-x   0        0        0     8466 2020-02-02 00:00:00.000000 panda_server-0.3.3/pandaserver/taskbuffer/FileSpec.py
--rw-r--r--   0        0        0     7148 2020-02-02 00:00:00.000000 panda_server-0.3.3/pandaserver/taskbuffer/GlobalShares.py
--rw-r--r--   0        0        0     2777 2020-02-02 00:00:00.000000 panda_server-0.3.3/pandaserver/taskbuffer/HarvesterMetricsSpec.py
--rw-r--r--   0        0        0     2472 2020-02-02 00:00:00.000000 panda_server-0.3.3/pandaserver/taskbuffer/Initializer.py
--rwxr-xr-x   0        0        0    27241 2020-02-02 00:00:00.000000 panda_server-0.3.3/pandaserver/taskbuffer/JobSpec.py
--rw-r--r--   0        0        0     6057 2020-02-02 00:00:00.000000 panda_server-0.3.3/pandaserver/taskbuffer/JobUtils.py
--rw-r--r--   0        0        0     3912 2020-02-02 00:00:00.000000 panda_server-0.3.3/pandaserver/taskbuffer/NucleusSpec.py
--rw-r--r--   0        0        0  1267473 2020-02-02 00:00:00.000000 panda_server-0.3.3/pandaserver/taskbuffer/OraDBProxy.py
--rw-r--r--   0        0        0      238 2020-02-02 00:00:00.000000 panda_server-0.3.3/pandaserver/taskbuffer/PanDAMsgProcessor.py
--rw-r--r--   0        0        0      476 2020-02-02 00:00:00.000000 panda_server-0.3.3/pandaserver/taskbuffer/PandaDBSchemaInfo.py
--rw-r--r--   0        0        0      634 2020-02-02 00:00:00.000000 panda_server-0.3.3/pandaserver/taskbuffer/PickleFileSpec.py
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 panda_server-0.3.3/pandaserver/taskbuffer/PickleJobSpec.py
--rw-r--r--   0        0        0      982 2020-02-02 00:00:00.000000 panda_server-0.3.3/pandaserver/taskbuffer/PrioUtil.py
--rw-r--r--   0        0        0     3314 2020-02-02 00:00:00.000000 panda_server-0.3.3/pandaserver/taskbuffer/ProcessGroups.py
--rw-r--r--   0        0        0     3688 2020-02-02 00:00:00.000000 panda_server-0.3.3/pandaserver/taskbuffer/ResourceSpec.py
--rw-r--r--   0        0        0     1099 2020-02-02 00:00:00.000000 panda_server-0.3.3/pandaserver/taskbuffer/SQLDumper.py
--rw-r--r--   0        0        0     1828 2020-02-02 00:00:00.000000 panda_server-0.3.3/pandaserver/taskbuffer/SQLManager.py
--rw-r--r--   0        0        0     7088 2020-02-02 00:00:00.000000 panda_server-0.3.3/pandaserver/taskbuffer/SiteSpec.py
--rw-r--r--   0        0        0      206 2020-02-02 00:00:00.000000 panda_server-0.3.3/pandaserver/taskbuffer/SupErrors.py
--rwxr-xr-x   0        0        0   143625 2020-02-02 00:00:00.000000 panda_server-0.3.3/pandaserver/taskbuffer/TaskBuffer.py
--rw-r--r--   0        0        0     5157 2020-02-02 00:00:00.000000 panda_server-0.3.3/pandaserver/taskbuffer/TaskBufferInterface.py
--rwxr-xr-x   0        0        0    26885 2020-02-02 00:00:00.000000 panda_server-0.3.3/pandaserver/taskbuffer/Utils.py
--rw-r--r--   0        0        0     3983 2020-02-02 00:00:00.000000 panda_server-0.3.3/pandaserver/taskbuffer/WorkerSpec.py
--rw-r--r--   0        0        0    17651 2020-02-02 00:00:00.000000 panda_server-0.3.3/pandaserver/taskbuffer/WrappedCursor.py
--rw-r--r--   0        0        0     3179 2020-02-02 00:00:00.000000 panda_server-0.3.3/pandaserver/taskbuffer/WrappedPickle.py
--rw-r--r--   0        0        0      482 2020-02-02 00:00:00.000000 panda_server-0.3.3/pandaserver/taskbuffer/WrappedPostgresConn.py
--rwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 panda_server-0.3.3/pandaserver/taskbuffer/__init__.py
--rw-r--r--   0        0        0    18729 2020-02-02 00:00:00.000000 panda_server-0.3.3/pandaserver/taskbuffer/retryModule.py
--rw-r--r--   0        0        0     5738 2020-02-02 00:00:00.000000 panda_server-0.3.3/pandaserver/taskbuffer/task_split_rules.py
--rw-r--r--   0        0        0    12538 2020-02-02 00:00:00.000000 panda_server-0.3.3/pandaserver/taskbuffer/workflow_processor.py
--rw-r--r--   0        0        0     1475 2020-02-02 00:00:00.000000 panda_server-0.3.3/pandaserver/test/SchemaChecker.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 panda_server-0.3.3/pandaserver/test/__init__.py
--rw-r--r--   0        0        0     1044 2020-02-02 00:00:00.000000 panda_server-0.3.3/pandaserver/test/banUser.py
--rwxr-xr-x   0        0        0      643 2020-02-02 00:00:00.000000 panda_server-0.3.3/pandaserver/test/boostPrio.py
--rwxr-xr-x   0        0        0     1225 2020-02-02 00:00:00.000000 panda_server-0.3.3/pandaserver/test/boostUser.py
--rwxr-xr-x   0        0        0      665 2020-02-02 00:00:00.000000 panda_server-0.3.3/pandaserver/test/callbackDDM.py
--rw-r--r--   0        0        0     2409 2020-02-02 00:00:00.000000 panda_server-0.3.3/pandaserver/test/daod_on_demand.py
--rwxr-xr-x   0        0        0    10154 2020-02-02 00:00:00.000000 panda_server-0.3.3/pandaserver/test/finishJob.py
--rw-r--r--   0        0        0      228 2020-02-02 00:00:00.000000 panda_server-0.3.3/pandaserver/test/finishTaskJEDI.py
--rwxr-xr-x   0        0        0     1238 2020-02-02 00:00:00.000000 panda_server-0.3.3/pandaserver/test/getJobs.py
--rwxr-xr-x   0        0        0     2032 2020-02-02 00:00:00.000000 panda_server-0.3.3/pandaserver/test/killJob.py
--rwxr-xr-x   0        0        0     3023 2020-02-02 00:00:00.000000 panda_server-0.3.3/pandaserver/test/killJobLowPrio.py
--rwxr-xr-x   0        0        0     1670 2020-02-02 00:00:00.000000 panda_server-0.3.3/pandaserver/test/killJobsInTask.py
--rwxr-xr-x   0        0        0      557 2020-02-02 00:00:00.000000 panda_server-0.3.3/pandaserver/test/killProdJobs.py
--rwxr-xr-x   0        0        0     2314 2020-02-02 00:00:00.000000 panda_server-0.3.3/pandaserver/test/killTask.py
--rwxr-xr-x   0        0        0      241 2020-02-02 00:00:00.000000 panda_server-0.3.3/pandaserver/test/killTaskJEDI.py
--rw-r--r--   0        0        0     2452 2020-02-02 00:00:00.000000 panda_server-0.3.3/pandaserver/test/killUser.py
--rwxr-xr-x   0        0        0      341 2020-02-02 00:00:00.000000 panda_server-0.3.3/pandaserver/test/reassignJobs.py
--rw-r--r--   0        0        0     2318 2020-02-02 00:00:00.000000 panda_server-0.3.3/pandaserver/test/reassignSite.py
--rw-r--r--   0        0        0     3346 2020-02-02 00:00:00.000000 panda_server-0.3.3/pandaserver/test/reassignTask.py
--rwxr-xr-x   0        0        0     1070 2020-02-02 00:00:00.000000 panda_server-0.3.3/pandaserver/test/reassignWaiting.py
--rw-r--r--   0        0        0      144 2020-02-02 00:00:00.000000 panda_server-0.3.3/pandaserver/test/recoverLostFiles.py
--rw-r--r--   0        0        0     1776 2020-02-02 00:00:00.000000 panda_server-0.3.3/pandaserver/test/reloadInputDS.py
--rw-r--r--   0        0        0      623 2020-02-02 00:00:00.000000 panda_server-0.3.3/pandaserver/test/sendCommandToJob.py
--rwxr-xr-x   0        0        0      936 2020-02-02 00:00:00.000000 panda_server-0.3.3/pandaserver/test/setDebugMode.py
--rwxr-xr-x   0        0        0      826 2020-02-02 00:00:00.000000 panda_server-0.3.3/pandaserver/test/setPriority.py
--rwxr-xr-x   0        0        0     1726 2020-02-02 00:00:00.000000 panda_server-0.3.3/pandaserver/test/testEvgen.py
--rwxr-xr-x   0        0        0     1700 2020-02-02 00:00:00.000000 panda_server-0.3.3/pandaserver/test/testEvgen17.py
--rwxr-xr-x   0        0        0     2446 2020-02-02 00:00:00.000000 panda_server-0.3.3/pandaserver/test/testG4sim.py
--rw-r--r--   0        0        0     2599 2020-02-02 00:00:00.000000 panda_server-0.3.3/pandaserver/test/testG4sim17.py
--rw-r--r--   0        0        0     1801 2020-02-02 00:00:00.000000 panda_server-0.3.3/pandaserver/test/testGetCriteriaForGlobalShares.py
--rw-r--r--   0        0        0     5059 2020-02-02 00:00:00.000000 panda_server-0.3.3/pandaserver/test/testGlobalShares.py
--rw-r--r--   0        0        0    12073 2020-02-02 00:00:00.000000 panda_server-0.3.3/pandaserver/test/testJobFlowATLAS.py
--rwxr-xr-x   0        0        0     3540 2020-02-02 00:00:00.000000 panda_server-0.3.3/pandaserver/test/testReco.py
--rw-r--r--   0        0        0     3054 2020-02-02 00:00:00.000000 panda_server-0.3.3/pandaserver/test/testSimulReco14.py
--rwxr-xr-x   0        0        0      708 2020-02-02 00:00:00.000000 panda_server-0.3.3/pandaserver/test/testSiteMap.py
--rw-r--r--   0        0        0      407 2020-02-02 00:00:00.000000 panda_server-0.3.3/pandaserver/test/testUpdateWorkerPilotStatus.py
--rw-r--r--   0        0        0     1179 2020-02-02 00:00:00.000000 panda_server-0.3.3/pandaserver/test/testutils.py
--rw-r--r--   0        0        0      396 2020-02-02 00:00:00.000000 panda_server-0.3.3/pandaserver/test/alice/README.txt
--rw-r--r--   0        0        0      196 2020-02-02 00:00:00.000000 panda_server-0.3.3/pandaserver/test/alice/mysetup
--rw-r--r--   0        0        0     1252 2020-02-02 00:00:00.000000 panda_server-0.3.3/pandaserver/test/alice/titan_testScript_ec2_alice_1.py
--rw-r--r--   0        0        0     1301 2020-02-02 00:00:00.000000 panda_server-0.3.3/pandaserver/test/alice/titan_testScript_ec2_alice_2.py
--rw-r--r--   0        0        0      222 2020-02-02 00:00:00.000000 panda_server-0.3.3/pandaserver/test/lsst/README.txt
--rw-r--r--   0        0        0     4773 2020-02-02 00:00:00.000000 panda_server-0.3.3/pandaserver/test/lsst/lsstSubmit.py
--rw-r--r--   0        0        0     4880 2020-02-02 00:00:00.000000 panda_server-0.3.3/pandaserver/test/lsst/lsstSubmitMERGEtest.py
--rw-r--r--   0        0        0     1683 2020-02-02 00:00:00.000000 panda_server-0.3.3/pandaserver/test/lsst/lsstSubmitPhosim332.py
--rw-r--r--   0        0        0     1069 2020-02-02 00:00:00.000000 panda_server-0.3.3/pandaserver/test/lsst/prepare-client-tarball-from-bigpanda-server.sh
--rwxr-xr-x   0        0        0    80304 2020-02-02 00:00:00.000000 panda_server-0.3.3/pandaserver/userinterface/Client.py
--rw-r--r--   0        0        0    91604 2020-02-02 00:00:00.000000 panda_server-0.3.3/pandaserver/userinterface/UserIF.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 panda_server-0.3.3/pandaserver/userinterface/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 panda_server-0.3.3/pandaserver/workflow/__init__.py
--rw-r--r--   0        0        0     4848 2020-02-02 00:00:00.000000 panda_server-0.3.3/pandaserver/workflow/pcwl_test.py
--rw-r--r--   0        0        0    14436 2020-02-02 00:00:00.000000 panda_server-0.3.3/pandaserver/workflow/pcwl_utils.py
--rw-r--r--   0        0        0     1957 2020-02-02 00:00:00.000000 panda_server-0.3.3/pandaserver/workflow/psnakemake_container.json
--rw-r--r--   0        0        0     1823 2020-02-02 00:00:00.000000 panda_server-0.3.3/pandaserver/workflow/psnakemake_task.json
--rw-r--r--   0        0        0     2090 2020-02-02 00:00:00.000000 panda_server-0.3.3/pandaserver/workflow/psnakemake_test.py
--rw-r--r--   0        0        0    39025 2020-02-02 00:00:00.000000 panda_server-0.3.3/pandaserver/workflow/workflow_utils.py
--rw-r--r--   0        0        0       50 2020-02-02 00:00:00.000000 panda_server-0.3.3/pandaserver/workflow/snakeparser/__init__.py
--rw-r--r--   0        0        0     1750 2020-02-02 00:00:00.000000 panda_server-0.3.3/pandaserver/workflow/snakeparser/extensions.py
--rw-r--r--   0        0        0     1696 2020-02-02 00:00:00.000000 panda_server-0.3.3/pandaserver/workflow/snakeparser/log.py
--rw-r--r--   0        0        0       78 2020-02-02 00:00:00.000000 panda_server-0.3.3/pandaserver/workflow/snakeparser/names.py
--rw-r--r--   0        0        0    13843 2020-02-02 00:00:00.000000 panda_server-0.3.3/pandaserver/workflow/snakeparser/parser.py
--rw-r--r--   0        0        0      643 2020-02-02 00:00:00.000000 panda_server-0.3.3/pandaserver/workflow/snakeparser/utils.py
--rw-r--r--   0        0        0      633 2020-02-02 00:00:00.000000 panda_server-0.3.3/templates/conda_meta.yaml.template
--rw-r--r--   0        0        0     5109 2020-02-02 00:00:00.000000 panda_server-0.3.3/templates/panda_server-httpd-FastCGI.conf.rpmnew.template
--rw-r--r--   0        0        0     3534 2020-02-02 00:00:00.000000 panda_server-0.3.3/templates/panda_server-httpd.conf.rpmnew.template
--rw-r--r--   0        0        0     6035 2020-02-02 00:00:00.000000 panda_server-0.3.3/templates/panda_server.cfg.rpmnew.template
--rwxr-xr-x   0        0        0    15351 2020-02-02 00:00:00.000000 panda_server-0.3.3/templates/bin/panda_server-makeSlsXml.exe.template
--rwxr-xr-x   0        0        0      745 2020-02-02 00:00:00.000000 panda_server-0.3.3/templates/bin/panda_server-vomsrenew.exe.template
--rw-r--r--   0        0        0     2862 2020-02-02 00:00:00.000000 panda_server-0.3.3/templates/init.d/panda_daemon.exe.template
--rw-r--r--   0        0        0     6668 2020-02-02 00:00:00.000000 panda_server-0.3.3/templates/init.d/panda_httpd.exe.template
--rwxr-xr-x   0        0        0     1547 2020-02-02 00:00:00.000000 panda_server-0.3.3/templates/init.d/panda_server.exe.template
--rw-r--r--   0        0        0      618 2020-02-02 00:00:00.000000 panda_server-0.3.3/templates/logrotate.d/panda_server.logrotate.template
--rw-r--r--   0        0        0     2619 2020-02-02 00:00:00.000000 panda_server-0.3.3/templates/sysconfig/panda_server.sysconfig.rpmnew.template
--rw-r--r--   0        0        0      780 2020-02-02 00:00:00.000000 panda_server-0.3.3/templates/sysconfig/panda_server_env.systemd.rpmnew.template
--rw-r--r--   0        0        0      463 2020-02-02 00:00:00.000000 panda_server-0.3.3/templates/systemd/panda.service.template
--rw-r--r--   0        0        0      495 2020-02-02 00:00:00.000000 panda_server-0.3.3/templates/systemd/panda_daemon.service.template
--rw-r--r--   0        0        0      392 2020-02-02 00:00:00.000000 panda_server-0.3.3/templates/systemd/panda_httpd.service.template
--rw-r--r--   0        0        0    11358 2020-02-02 00:00:00.000000 panda_server-0.3.3/LICENSE.txt
--rw-r--r--   0        0        0      394 2020-02-02 00:00:00.000000 panda_server-0.3.3/README.md
--rw-r--r--   0        0        0     2118 2020-02-02 00:00:00.000000 panda_server-0.3.3/pyproject.toml
--rw-r--r--   0        0        0     1929 2020-02-02 00:00:00.000000 panda_server-0.3.3/PKG-INFO
+-rw-r--r--   0        0        0      461 2020-02-02 00:00:00.000000 panda_server-0.3.4/.pre-commit-config.yaml
+-rw-r--r--   0        0        0    81265 2020-02-02 00:00:00.000000 panda_server-0.3.4/ChangeLog.txt
+-rw-r--r--   0        0        0     4406 2020-02-02 00:00:00.000000 panda_server-0.3.4/Dockerfile
+-rw-r--r--   0        0        0     2039 2020-02-02 00:00:00.000000 panda_server-0.3.4/INSTALL.md
+-rw-r--r--   0        0        0     1598 2020-02-02 00:00:00.000000 panda_server-0.3.4/INSTALL_ATLAS.md
+-rw-r--r--   0        0        0       64 2020-02-02 00:00:00.000000 panda_server-0.3.4/MANIFEST.in
+-rw-r--r--   0        0        0       26 2020-02-02 00:00:00.000000 panda_server-0.3.4/PandaPkgInfo.py
+-rw-r--r--   0        0        0     1255 2020-02-02 00:00:00.000000 panda_server-0.3.4/panda-server.spec
+-rw-r--r--   0        0        0     4795 2020-02-02 00:00:00.000000 panda_server-0.3.4/package/hatch_build.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 panda_server-0.3.4/pandaserver/__init__.py
+-rw-r--r--   0        0        0       99 2020-02-02 00:00:00.000000 panda_server-0.3.4/pandaserver/brokerage/ErrorCode.py
+-rw-r--r--   0        0        0    16370 2020-02-02 00:00:00.000000 panda_server-0.3.4/pandaserver/brokerage/SiteMapper.py
+-rwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 panda_server-0.3.4/pandaserver/brokerage/__init__.py
+-rwxr-xr-x   0        0        0    85928 2020-02-02 00:00:00.000000 panda_server-0.3.4/pandaserver/brokerage/broker.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 panda_server-0.3.4/pandaserver/config/__init__.py
+-rw-r--r--   0        0        0      491 2020-02-02 00:00:00.000000 panda_server-0.3.4/pandaserver/config/config_utils.py
+-rw-r--r--   0        0        0      551 2020-02-02 00:00:00.000000 panda_server-0.3.4/pandaserver/config/daemon_config.py
+-rwxr-xr-x   0        0        0     6900 2020-02-02 00:00:00.000000 panda_server-0.3.4/pandaserver/config/panda_config.py
+-rw-r--r--   0        0        0     2435 2020-02-02 00:00:00.000000 panda_server-0.3.4/pandaserver/configurator/Carbon.py
+-rw-r--r--   0        0        0    38070 2020-02-02 00:00:00.000000 panda_server-0.3.4/pandaserver/configurator/Configurator.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 panda_server-0.3.4/pandaserver/configurator/__init__.py
+-rw-r--r--   0        0        0     1906 2020-02-02 00:00:00.000000 panda_server-0.3.4/pandaserver/configurator/aux.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 panda_server-0.3.4/pandaserver/daemons/__init__.py
+-rw-r--r--   0        0        0     3022 2020-02-02 00:00:00.000000 panda_server-0.3.4/pandaserver/daemons/master.py
+-rw-r--r--   0        0        0     2363 2020-02-02 00:00:00.000000 panda_server-0.3.4/pandaserver/daemons/master_systemd.py
+-rw-r--r--   0        0        0    25423 2020-02-02 00:00:00.000000 panda_server-0.3.4/pandaserver/daemons/utils.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 panda_server-0.3.4/pandaserver/daemons/scripts/__init__.py
+-rw-r--r--   0        0        0     8804 2020-02-02 00:00:00.000000 panda_server-0.3.4/pandaserver/daemons/scripts/add_main.py
+-rw-r--r--   0        0        0    13604 2020-02-02 00:00:00.000000 panda_server-0.3.4/pandaserver/daemons/scripts/add_sub.py
+-rw-r--r--   0        0        0     1288 2020-02-02 00:00:00.000000 panda_server-0.3.4/pandaserver/daemons/scripts/cache_pilots.py
+-rw-r--r--   0        0        0    11242 2020-02-02 00:00:00.000000 panda_server-0.3.4/pandaserver/daemons/scripts/cache_schedconfig.py
+-rw-r--r--   0        0        0     1455 2020-02-02 00:00:00.000000 panda_server-0.3.4/pandaserver/daemons/scripts/carbon.py
+-rw-r--r--   0        0        0     3308 2020-02-02 00:00:00.000000 panda_server-0.3.4/pandaserver/daemons/scripts/configurator.py
+-rw-r--r--   0        0        0    63605 2020-02-02 00:00:00.000000 panda_server-0.3.4/pandaserver/daemons/scripts/copyArchive.py
+-rw-r--r--   0        0        0    53989 2020-02-02 00:00:00.000000 panda_server-0.3.4/pandaserver/daemons/scripts/datasetManager.py
+-rw-r--r--   0        0        0      490 2020-02-02 00:00:00.000000 panda_server-0.3.4/pandaserver/daemons/scripts/dummy_test.py
+-rw-r--r--   0        0        0     4703 2020-02-02 00:00:00.000000 panda_server-0.3.4/pandaserver/daemons/scripts/evpPD2P.py
+-rw-r--r--   0        0        0    41997 2020-02-02 00:00:00.000000 panda_server-0.3.4/pandaserver/daemons/scripts/metric_collector.py
+-rw-r--r--   0        0        0     2330 2020-02-02 00:00:00.000000 panda_server-0.3.4/pandaserver/daemons/scripts/panda_activeusers_query.py
+-rw-r--r--   0        0        0     3305 2020-02-02 00:00:00.000000 panda_server-0.3.4/pandaserver/daemons/scripts/pilotStreaming.py
+-rw-r--r--   0        0        0     5392 2020-02-02 00:00:00.000000 panda_server-0.3.4/pandaserver/daemons/scripts/process_workflow_files_daemon.py
+-rw-r--r--   0        0        0     5063 2020-02-02 00:00:00.000000 panda_server-0.3.4/pandaserver/daemons/scripts/recover_lost_files_daemon.py
+-rw-r--r--   0        0        0    15357 2020-02-02 00:00:00.000000 panda_server-0.3.4/pandaserver/daemons/scripts/task_evaluator.py
+-rw-r--r--   0        0        0     1933 2020-02-02 00:00:00.000000 panda_server-0.3.4/pandaserver/daemons/scripts/tmpwatch.py
+-rw-r--r--   0        0        0     3019 2020-02-02 00:00:00.000000 panda_server-0.3.4/pandaserver/daemons/scripts/worker_synchronization.py
+-rw-r--r--   0        0        0    54210 2020-02-02 00:00:00.000000 panda_server-0.3.4/pandaserver/dataservice/AdderAtlasPlugin.py
+-rw-r--r--   0        0        0      343 2020-02-02 00:00:00.000000 panda_server-0.3.4/pandaserver/dataservice/AdderDummyPlugin.py
+-rw-r--r--   0        0        0    42448 2020-02-02 00:00:00.000000 panda_server-0.3.4/pandaserver/dataservice/AdderGen.py
+-rw-r--r--   0        0        0      301 2020-02-02 00:00:00.000000 panda_server-0.3.4/pandaserver/dataservice/AdderPluginBase.py
+-rw-r--r--   0        0        0     1074 2020-02-02 00:00:00.000000 panda_server-0.3.4/pandaserver/dataservice/AdderResult.py
+-rw-r--r--   0        0        0     5999 2020-02-02 00:00:00.000000 panda_server-0.3.4/pandaserver/dataservice/AdderSimplePlugin.py
+-rw-r--r--   0        0        0    13140 2020-02-02 00:00:00.000000 panda_server-0.3.4/pandaserver/dataservice/DataServiceUtils.py
+-rwxr-xr-x   0        0        0      390 2020-02-02 00:00:00.000000 panda_server-0.3.4/pandaserver/dataservice/ErrorCode.py
+-rw-r--r--   0        0        0     1664 2020-02-02 00:00:00.000000 panda_server-0.3.4/pandaserver/dataservice/ProcessLimiter.py
+-rw-r--r--   0        0        0    10594 2020-02-02 00:00:00.000000 panda_server-0.3.4/pandaserver/dataservice/RecoverLostFilesCore.py
+-rwxr-xr-x   0        0        0     8820 2020-02-02 00:00:00.000000 panda_server-0.3.4/pandaserver/dataservice/Setupper.py
+-rwxr-xr-x   0        0        0   111777 2020-02-02 00:00:00.000000 panda_server-0.3.4/pandaserver/dataservice/SetupperAtlasPlugin.py
+-rw-r--r--   0        0        0      638 2020-02-02 00:00:00.000000 panda_server-0.3.4/pandaserver/dataservice/SetupperDummyPlugin.py
+-rw-r--r--   0        0        0     1285 2020-02-02 00:00:00.000000 panda_server-0.3.4/pandaserver/dataservice/SetupperPluginBase.py
+-rwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 panda_server-0.3.4/pandaserver/dataservice/__init__.py
+-rwxr-xr-x   0        0        0     2553 2020-02-02 00:00:00.000000 panda_server-0.3.4/pandaserver/dataservice/activator.py
+-rwxr-xr-x   0        0        0    10782 2020-02-02 00:00:00.000000 panda_server-0.3.4/pandaserver/dataservice/closer.py
+-rw-r--r--   0        0        0     3183 2020-02-02 00:00:00.000000 panda_server-0.3.4/pandaserver/dataservice/closer_atlas_plugin.py
+-rwxr-xr-x   0        0        0    39928 2020-02-02 00:00:00.000000 panda_server-0.3.4/pandaserver/dataservice/ddm.py
+-rw-r--r--   0        0        0     3104 2020-02-02 00:00:00.000000 panda_server-0.3.4/pandaserver/dataservice/ddm_handler.py
+-rw-r--r--   0        0        0    35028 2020-02-02 00:00:00.000000 panda_server-0.3.4/pandaserver/dataservice/dyn_data_distributer.py
+-rw-r--r--   0        0        0     3589 2020-02-02 00:00:00.000000 panda_server-0.3.4/pandaserver/dataservice/event_lookup_client_ei.py
+-rw-r--r--   0        0        0    10398 2020-02-02 00:00:00.000000 panda_server-0.3.4/pandaserver/dataservice/event_picker.py
+-rwxr-xr-x   0        0        0     7248 2020-02-02 00:00:00.000000 panda_server-0.3.4/pandaserver/dataservice/finisher.py
+-rwxr-xr-x   0        0        0     2317 2020-02-02 00:00:00.000000 panda_server-0.3.4/pandaserver/dataservice/forkSetupper.py
+-rw-r--r--   0        0        0     1030 2020-02-02 00:00:00.000000 panda_server-0.3.4/pandaserver/jobdispatcher/DispatcherUtils.py
+-rwxr-xr-x   0        0        0      249 2020-02-02 00:00:00.000000 panda_server-0.3.4/pandaserver/jobdispatcher/ErrorCode.py
+-rwxr-xr-x   0        0        0    58971 2020-02-02 00:00:00.000000 panda_server-0.3.4/pandaserver/jobdispatcher/JobDispatcher.py
+-rwxr-xr-x   0        0        0    16520 2020-02-02 00:00:00.000000 panda_server-0.3.4/pandaserver/jobdispatcher/Protocol.py
+-rwxr-xr-x   0        0        0     9377 2020-02-02 00:00:00.000000 panda_server-0.3.4/pandaserver/jobdispatcher/Watcher.py
+-rwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 panda_server-0.3.4/pandaserver/jobdispatcher/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 panda_server-0.3.4/pandaserver/proxycache/__init__.py
+-rw-r--r--   0        0        0     9933 2020-02-02 00:00:00.000000 panda_server-0.3.4/pandaserver/proxycache/panda_proxy_cache.py
+-rw-r--r--   0        0        0       77 2020-02-02 00:00:00.000000 panda_server-0.3.4/pandaserver/server/.gacl
+-rwxr-xr-x   0        0        0    11763 2020-02-02 00:00:00.000000 panda_server-0.3.4/pandaserver/server/panda.py
+-rw-r--r--   0        0        0     5528 2020-02-02 00:00:00.000000 panda_server-0.3.4/pandaserver/srvcore/CoreUtils.py
+-rwxr-xr-x   0        0        0     4014 2020-02-02 00:00:00.000000 panda_server-0.3.4/pandaserver/srvcore/MailUtils.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 panda_server-0.3.4/pandaserver/srvcore/__init__.py
+-rw-r--r--   0        0        0     3446 2020-02-02 00:00:00.000000 panda_server-0.3.4/pandaserver/srvcore/allowed_methods.py
+-rw-r--r--   0        0        0     4169 2020-02-02 00:00:00.000000 panda_server-0.3.4/pandaserver/srvcore/oidc_utils.py
+-rw-r--r--   0        0        0     6640 2020-02-02 00:00:00.000000 panda_server-0.3.4/pandaserver/srvcore/panda_request.py
+-rw-r--r--   0        0        0     1190 2020-02-02 00:00:00.000000 panda_server-0.3.4/pandaserver/srvcore/srv_msg_utils.py
+-rw-r--r--   0        0        0      734 2020-02-02 00:00:00.000000 panda_server-0.3.4/pandaserver/taskbuffer/CloudSpec.py
+-rw-r--r--   0        0        0     2449 2020-02-02 00:00:00.000000 panda_server-0.3.4/pandaserver/taskbuffer/CloudTaskSpec.py
+-rw-r--r--   0        0        0    18693 2020-02-02 00:00:00.000000 panda_server-0.3.4/pandaserver/taskbuffer/ConBridge.py
+-rwxr-xr-x   0        0        0     2583 2020-02-02 00:00:00.000000 panda_server-0.3.4/pandaserver/taskbuffer/DBProxyPool.py
+-rwxr-xr-x   0        0        0     3568 2020-02-02 00:00:00.000000 panda_server-0.3.4/pandaserver/taskbuffer/DatasetSpec.py
+-rw-r--r--   0        0        0     4014 2020-02-02 00:00:00.000000 panda_server-0.3.4/pandaserver/taskbuffer/DdmSpec.py
+-rwxr-xr-x   0        0        0     1746 2020-02-02 00:00:00.000000 panda_server-0.3.4/pandaserver/taskbuffer/ErrorCode.py
+-rw-r--r--   0        0        0    10956 2020-02-02 00:00:00.000000 panda_server-0.3.4/pandaserver/taskbuffer/EventServiceUtils.py
+-rwxr-xr-x   0        0        0     8466 2020-02-02 00:00:00.000000 panda_server-0.3.4/pandaserver/taskbuffer/FileSpec.py
+-rw-r--r--   0        0        0     7148 2020-02-02 00:00:00.000000 panda_server-0.3.4/pandaserver/taskbuffer/GlobalShares.py
+-rw-r--r--   0        0        0     2777 2020-02-02 00:00:00.000000 panda_server-0.3.4/pandaserver/taskbuffer/HarvesterMetricsSpec.py
+-rw-r--r--   0        0        0     2472 2020-02-02 00:00:00.000000 panda_server-0.3.4/pandaserver/taskbuffer/Initializer.py
+-rwxr-xr-x   0        0        0    27241 2020-02-02 00:00:00.000000 panda_server-0.3.4/pandaserver/taskbuffer/JobSpec.py
+-rw-r--r--   0        0        0     5861 2020-02-02 00:00:00.000000 panda_server-0.3.4/pandaserver/taskbuffer/JobUtils.py
+-rw-r--r--   0        0        0     3912 2020-02-02 00:00:00.000000 panda_server-0.3.4/pandaserver/taskbuffer/NucleusSpec.py
+-rw-r--r--   0        0        0  1268991 2020-02-02 00:00:00.000000 panda_server-0.3.4/pandaserver/taskbuffer/OraDBProxy.py
+-rw-r--r--   0        0        0      238 2020-02-02 00:00:00.000000 panda_server-0.3.4/pandaserver/taskbuffer/PanDAMsgProcessor.py
+-rw-r--r--   0        0        0      476 2020-02-02 00:00:00.000000 panda_server-0.3.4/pandaserver/taskbuffer/PandaDBSchemaInfo.py
+-rw-r--r--   0        0        0      634 2020-02-02 00:00:00.000000 panda_server-0.3.4/pandaserver/taskbuffer/PickleFileSpec.py
+-rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 panda_server-0.3.4/pandaserver/taskbuffer/PickleJobSpec.py
+-rw-r--r--   0        0        0      982 2020-02-02 00:00:00.000000 panda_server-0.3.4/pandaserver/taskbuffer/PrioUtil.py
+-rw-r--r--   0        0        0     3314 2020-02-02 00:00:00.000000 panda_server-0.3.4/pandaserver/taskbuffer/ProcessGroups.py
+-rw-r--r--   0        0        0     5299 2020-02-02 00:00:00.000000 panda_server-0.3.4/pandaserver/taskbuffer/ResourceSpec.py
+-rw-r--r--   0        0        0     1099 2020-02-02 00:00:00.000000 panda_server-0.3.4/pandaserver/taskbuffer/SQLDumper.py
+-rw-r--r--   0        0        0     1828 2020-02-02 00:00:00.000000 panda_server-0.3.4/pandaserver/taskbuffer/SQLManager.py
+-rw-r--r--   0        0        0     6889 2020-02-02 00:00:00.000000 panda_server-0.3.4/pandaserver/taskbuffer/SiteSpec.py
+-rw-r--r--   0        0        0      206 2020-02-02 00:00:00.000000 panda_server-0.3.4/pandaserver/taskbuffer/SupErrors.py
+-rwxr-xr-x   0        0        0   143604 2020-02-02 00:00:00.000000 panda_server-0.3.4/pandaserver/taskbuffer/TaskBuffer.py
+-rw-r--r--   0        0        0     5157 2020-02-02 00:00:00.000000 panda_server-0.3.4/pandaserver/taskbuffer/TaskBufferInterface.py
+-rwxr-xr-x   0        0        0    26885 2020-02-02 00:00:00.000000 panda_server-0.3.4/pandaserver/taskbuffer/Utils.py
+-rw-r--r--   0        0        0     3983 2020-02-02 00:00:00.000000 panda_server-0.3.4/pandaserver/taskbuffer/WorkerSpec.py
+-rw-r--r--   0        0        0    17651 2020-02-02 00:00:00.000000 panda_server-0.3.4/pandaserver/taskbuffer/WrappedCursor.py
+-rw-r--r--   0        0        0     3179 2020-02-02 00:00:00.000000 panda_server-0.3.4/pandaserver/taskbuffer/WrappedPickle.py
+-rw-r--r--   0        0        0      482 2020-02-02 00:00:00.000000 panda_server-0.3.4/pandaserver/taskbuffer/WrappedPostgresConn.py
+-rwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 panda_server-0.3.4/pandaserver/taskbuffer/__init__.py
+-rw-r--r--   0        0        0    18729 2020-02-02 00:00:00.000000 panda_server-0.3.4/pandaserver/taskbuffer/retryModule.py
+-rw-r--r--   0        0        0     5738 2020-02-02 00:00:00.000000 panda_server-0.3.4/pandaserver/taskbuffer/task_split_rules.py
+-rw-r--r--   0        0        0    12538 2020-02-02 00:00:00.000000 panda_server-0.3.4/pandaserver/taskbuffer/workflow_processor.py
+-rw-r--r--   0        0        0     1475 2020-02-02 00:00:00.000000 panda_server-0.3.4/pandaserver/test/SchemaChecker.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 panda_server-0.3.4/pandaserver/test/__init__.py
+-rw-r--r--   0        0        0     1044 2020-02-02 00:00:00.000000 panda_server-0.3.4/pandaserver/test/banUser.py
+-rwxr-xr-x   0        0        0      643 2020-02-02 00:00:00.000000 panda_server-0.3.4/pandaserver/test/boostPrio.py
+-rwxr-xr-x   0        0        0     1225 2020-02-02 00:00:00.000000 panda_server-0.3.4/pandaserver/test/boostUser.py
+-rwxr-xr-x   0        0        0      665 2020-02-02 00:00:00.000000 panda_server-0.3.4/pandaserver/test/callbackDDM.py
+-rw-r--r--   0        0        0     2409 2020-02-02 00:00:00.000000 panda_server-0.3.4/pandaserver/test/daod_on_demand.py
+-rwxr-xr-x   0        0        0    10154 2020-02-02 00:00:00.000000 panda_server-0.3.4/pandaserver/test/finishJob.py
+-rw-r--r--   0        0        0      228 2020-02-02 00:00:00.000000 panda_server-0.3.4/pandaserver/test/finishTaskJEDI.py
+-rwxr-xr-x   0        0        0     1238 2020-02-02 00:00:00.000000 panda_server-0.3.4/pandaserver/test/getJobs.py
+-rwxr-xr-x   0        0        0     2032 2020-02-02 00:00:00.000000 panda_server-0.3.4/pandaserver/test/killJob.py
+-rwxr-xr-x   0        0        0     3023 2020-02-02 00:00:00.000000 panda_server-0.3.4/pandaserver/test/killJobLowPrio.py
+-rwxr-xr-x   0        0        0     1670 2020-02-02 00:00:00.000000 panda_server-0.3.4/pandaserver/test/killJobsInTask.py
+-rwxr-xr-x   0        0        0      557 2020-02-02 00:00:00.000000 panda_server-0.3.4/pandaserver/test/killProdJobs.py
+-rwxr-xr-x   0        0        0     2314 2020-02-02 00:00:00.000000 panda_server-0.3.4/pandaserver/test/killTask.py
+-rwxr-xr-x   0        0        0      241 2020-02-02 00:00:00.000000 panda_server-0.3.4/pandaserver/test/killTaskJEDI.py
+-rw-r--r--   0        0        0     2452 2020-02-02 00:00:00.000000 panda_server-0.3.4/pandaserver/test/killUser.py
+-rwxr-xr-x   0        0        0      341 2020-02-02 00:00:00.000000 panda_server-0.3.4/pandaserver/test/reassignJobs.py
+-rw-r--r--   0        0        0     2318 2020-02-02 00:00:00.000000 panda_server-0.3.4/pandaserver/test/reassignSite.py
+-rw-r--r--   0        0        0     3346 2020-02-02 00:00:00.000000 panda_server-0.3.4/pandaserver/test/reassignTask.py
+-rwxr-xr-x   0        0        0     1070 2020-02-02 00:00:00.000000 panda_server-0.3.4/pandaserver/test/reassignWaiting.py
+-rw-r--r--   0        0        0      144 2020-02-02 00:00:00.000000 panda_server-0.3.4/pandaserver/test/recoverLostFiles.py
+-rw-r--r--   0        0        0     1776 2020-02-02 00:00:00.000000 panda_server-0.3.4/pandaserver/test/reloadInputDS.py
+-rw-r--r--   0        0        0      623 2020-02-02 00:00:00.000000 panda_server-0.3.4/pandaserver/test/sendCommandToJob.py
+-rwxr-xr-x   0        0        0      936 2020-02-02 00:00:00.000000 panda_server-0.3.4/pandaserver/test/setDebugMode.py
+-rwxr-xr-x   0        0        0      826 2020-02-02 00:00:00.000000 panda_server-0.3.4/pandaserver/test/setPriority.py
+-rwxr-xr-x   0        0        0     1726 2020-02-02 00:00:00.000000 panda_server-0.3.4/pandaserver/test/testEvgen.py
+-rwxr-xr-x   0        0        0     1700 2020-02-02 00:00:00.000000 panda_server-0.3.4/pandaserver/test/testEvgen17.py
+-rwxr-xr-x   0        0        0     2446 2020-02-02 00:00:00.000000 panda_server-0.3.4/pandaserver/test/testG4sim.py
+-rw-r--r--   0        0        0     2599 2020-02-02 00:00:00.000000 panda_server-0.3.4/pandaserver/test/testG4sim17.py
+-rw-r--r--   0        0        0     1801 2020-02-02 00:00:00.000000 panda_server-0.3.4/pandaserver/test/testGetCriteriaForGlobalShares.py
+-rw-r--r--   0        0        0     5059 2020-02-02 00:00:00.000000 panda_server-0.3.4/pandaserver/test/testGlobalShares.py
+-rw-r--r--   0        0        0    12073 2020-02-02 00:00:00.000000 panda_server-0.3.4/pandaserver/test/testJobFlowATLAS.py
+-rwxr-xr-x   0        0        0     3540 2020-02-02 00:00:00.000000 panda_server-0.3.4/pandaserver/test/testReco.py
+-rw-r--r--   0        0        0     3054 2020-02-02 00:00:00.000000 panda_server-0.3.4/pandaserver/test/testSimulReco14.py
+-rwxr-xr-x   0        0        0      708 2020-02-02 00:00:00.000000 panda_server-0.3.4/pandaserver/test/testSiteMap.py
+-rw-r--r--   0        0        0      407 2020-02-02 00:00:00.000000 panda_server-0.3.4/pandaserver/test/testUpdateWorkerPilotStatus.py
+-rw-r--r--   0        0        0     1179 2020-02-02 00:00:00.000000 panda_server-0.3.4/pandaserver/test/testutils.py
+-rw-r--r--   0        0        0      396 2020-02-02 00:00:00.000000 panda_server-0.3.4/pandaserver/test/alice/README.txt
+-rw-r--r--   0        0        0      196 2020-02-02 00:00:00.000000 panda_server-0.3.4/pandaserver/test/alice/mysetup
+-rw-r--r--   0        0        0     1252 2020-02-02 00:00:00.000000 panda_server-0.3.4/pandaserver/test/alice/titan_testScript_ec2_alice_1.py
+-rw-r--r--   0        0        0     1301 2020-02-02 00:00:00.000000 panda_server-0.3.4/pandaserver/test/alice/titan_testScript_ec2_alice_2.py
+-rw-r--r--   0        0        0      222 2020-02-02 00:00:00.000000 panda_server-0.3.4/pandaserver/test/lsst/README.txt
+-rw-r--r--   0        0        0     4773 2020-02-02 00:00:00.000000 panda_server-0.3.4/pandaserver/test/lsst/lsstSubmit.py
+-rw-r--r--   0        0        0     4880 2020-02-02 00:00:00.000000 panda_server-0.3.4/pandaserver/test/lsst/lsstSubmitMERGEtest.py
+-rw-r--r--   0        0        0     1683 2020-02-02 00:00:00.000000 panda_server-0.3.4/pandaserver/test/lsst/lsstSubmitPhosim332.py
+-rw-r--r--   0        0        0     1069 2020-02-02 00:00:00.000000 panda_server-0.3.4/pandaserver/test/lsst/prepare-client-tarball-from-bigpanda-server.sh
+-rwxr-xr-x   0        0        0    80304 2020-02-02 00:00:00.000000 panda_server-0.3.4/pandaserver/userinterface/Client.py
+-rw-r--r--   0        0        0    91604 2020-02-02 00:00:00.000000 panda_server-0.3.4/pandaserver/userinterface/UserIF.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 panda_server-0.3.4/pandaserver/userinterface/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 panda_server-0.3.4/pandaserver/workflow/__init__.py
+-rw-r--r--   0        0        0     4848 2020-02-02 00:00:00.000000 panda_server-0.3.4/pandaserver/workflow/pcwl_test.py
+-rw-r--r--   0        0        0    14436 2020-02-02 00:00:00.000000 panda_server-0.3.4/pandaserver/workflow/pcwl_utils.py
+-rw-r--r--   0        0        0     1957 2020-02-02 00:00:00.000000 panda_server-0.3.4/pandaserver/workflow/psnakemake_container.json
+-rw-r--r--   0        0        0     1823 2020-02-02 00:00:00.000000 panda_server-0.3.4/pandaserver/workflow/psnakemake_task.json
+-rw-r--r--   0        0        0     2090 2020-02-02 00:00:00.000000 panda_server-0.3.4/pandaserver/workflow/psnakemake_test.py
+-rw-r--r--   0        0        0    39025 2020-02-02 00:00:00.000000 panda_server-0.3.4/pandaserver/workflow/workflow_utils.py
+-rw-r--r--   0        0        0       50 2020-02-02 00:00:00.000000 panda_server-0.3.4/pandaserver/workflow/snakeparser/__init__.py
+-rw-r--r--   0        0        0     1750 2020-02-02 00:00:00.000000 panda_server-0.3.4/pandaserver/workflow/snakeparser/extensions.py
+-rw-r--r--   0        0        0     1696 2020-02-02 00:00:00.000000 panda_server-0.3.4/pandaserver/workflow/snakeparser/log.py
+-rw-r--r--   0        0        0       78 2020-02-02 00:00:00.000000 panda_server-0.3.4/pandaserver/workflow/snakeparser/names.py
+-rw-r--r--   0        0        0    13843 2020-02-02 00:00:00.000000 panda_server-0.3.4/pandaserver/workflow/snakeparser/parser.py
+-rw-r--r--   0        0        0      643 2020-02-02 00:00:00.000000 panda_server-0.3.4/pandaserver/workflow/snakeparser/utils.py
+-rw-r--r--   0        0        0      633 2020-02-02 00:00:00.000000 panda_server-0.3.4/templates/conda_meta.yaml.template
+-rw-r--r--   0        0        0     5109 2020-02-02 00:00:00.000000 panda_server-0.3.4/templates/panda_server-httpd-FastCGI.conf.rpmnew.template
+-rw-r--r--   0        0        0     3534 2020-02-02 00:00:00.000000 panda_server-0.3.4/templates/panda_server-httpd.conf.rpmnew.template
+-rw-r--r--   0        0        0     6035 2020-02-02 00:00:00.000000 panda_server-0.3.4/templates/panda_server.cfg.rpmnew.template
+-rwxr-xr-x   0        0        0    15351 2020-02-02 00:00:00.000000 panda_server-0.3.4/templates/bin/panda_server-makeSlsXml.exe.template
+-rwxr-xr-x   0        0        0      745 2020-02-02 00:00:00.000000 panda_server-0.3.4/templates/bin/panda_server-vomsrenew.exe.template
+-rw-r--r--   0        0        0     2862 2020-02-02 00:00:00.000000 panda_server-0.3.4/templates/init.d/panda_daemon.exe.template
+-rw-r--r--   0        0        0     6668 2020-02-02 00:00:00.000000 panda_server-0.3.4/templates/init.d/panda_httpd.exe.template
+-rwxr-xr-x   0        0        0     1547 2020-02-02 00:00:00.000000 panda_server-0.3.4/templates/init.d/panda_server.exe.template
+-rw-r--r--   0        0        0      618 2020-02-02 00:00:00.000000 panda_server-0.3.4/templates/logrotate.d/panda_server.logrotate.template
+-rw-r--r--   0        0        0     2619 2020-02-02 00:00:00.000000 panda_server-0.3.4/templates/sysconfig/panda_server.sysconfig.rpmnew.template
+-rw-r--r--   0        0        0      780 2020-02-02 00:00:00.000000 panda_server-0.3.4/templates/sysconfig/panda_server_env.systemd.rpmnew.template
+-rw-r--r--   0        0        0      463 2020-02-02 00:00:00.000000 panda_server-0.3.4/templates/systemd/panda.service.template
+-rw-r--r--   0        0        0      495 2020-02-02 00:00:00.000000 panda_server-0.3.4/templates/systemd/panda_daemon.service.template
+-rw-r--r--   0        0        0      392 2020-02-02 00:00:00.000000 panda_server-0.3.4/templates/systemd/panda_httpd.service.template
+-rw-r--r--   0        0        0    11358 2020-02-02 00:00:00.000000 panda_server-0.3.4/LICENSE.txt
+-rw-r--r--   0        0        0      394 2020-02-02 00:00:00.000000 panda_server-0.3.4/README.md
+-rw-r--r--   0        0        0     2118 2020-02-02 00:00:00.000000 panda_server-0.3.4/pyproject.toml
+-rw-r--r--   0        0        0     1929 2020-02-02 00:00:00.000000 panda_server-0.3.4/PKG-INFO
```

### Comparing `panda_server-0.3.3/ChangeLog.txt` & `panda_server-0.3.4/ChangeLog.txt`

 * *Files identical despite different names*

### Comparing `panda_server-0.3.3/Dockerfile` & `panda_server-0.3.4/Dockerfile`

 * *Files identical despite different names*

### Comparing `panda_server-0.3.3/INSTALL.md` & `panda_server-0.3.4/INSTALL.md`

 * *Files identical despite different names*

### Comparing `panda_server-0.3.3/INSTALL_ATLAS.md` & `panda_server-0.3.4/INSTALL_ATLAS.md`

 * *Files identical despite different names*

### Comparing `panda_server-0.3.3/panda-server.spec` & `panda_server-0.3.4/panda-server.spec`

 * *Files identical despite different names*

### Comparing `panda_server-0.3.3/package/hatch_build.py` & `panda_server-0.3.4/package/hatch_build.py`

 * *Files identical despite different names*

### Comparing `panda_server-0.3.3/pandaserver/brokerage/SiteMapper.py` & `panda_server-0.3.4/pandaserver/brokerage/SiteMapper.py`

 * *Files identical despite different names*

### Comparing `panda_server-0.3.3/pandaserver/brokerage/broker.py` & `panda_server-0.3.4/pandaserver/brokerage/broker.py`

 * *Files identical despite different names*

### Comparing `panda_server-0.3.3/pandaserver/config/daemon_config.py` & `panda_server-0.3.4/pandaserver/config/daemon_config.py`

 * *Files identical despite different names*

### Comparing `panda_server-0.3.3/pandaserver/config/panda_config.py` & `panda_server-0.3.4/pandaserver/config/panda_config.py`

 * *Files identical despite different names*

### Comparing `panda_server-0.3.3/pandaserver/configurator/Carbon.py` & `panda_server-0.3.4/pandaserver/configurator/Carbon.py`

 * *Files identical despite different names*

### Comparing `panda_server-0.3.3/pandaserver/configurator/Configurator.py` & `panda_server-0.3.4/pandaserver/configurator/Configurator.py`

 * *Files identical despite different names*

### Comparing `panda_server-0.3.3/pandaserver/configurator/aux.py` & `panda_server-0.3.4/pandaserver/configurator/aux.py`

 * *Files identical despite different names*

### Comparing `panda_server-0.3.3/pandaserver/daemons/master.py` & `panda_server-0.3.4/pandaserver/daemons/master.py`

 * *Files identical despite different names*

### Comparing `panda_server-0.3.3/pandaserver/daemons/master_systemd.py` & `panda_server-0.3.4/pandaserver/daemons/master_systemd.py`

 * *Files identical despite different names*

### Comparing `panda_server-0.3.3/pandaserver/daemons/utils.py` & `panda_server-0.3.4/pandaserver/daemons/utils.py`

 * *Files identical despite different names*

### Comparing `panda_server-0.3.3/pandaserver/daemons/scripts/add_main.py` & `panda_server-0.3.4/pandaserver/daemons/scripts/add_main.py`

 * *Files identical despite different names*

### Comparing `panda_server-0.3.3/pandaserver/daemons/scripts/add_sub.py` & `panda_server-0.3.4/pandaserver/daemons/scripts/add_sub.py`

 * *Files identical despite different names*

### Comparing `panda_server-0.3.3/pandaserver/daemons/scripts/cache_pilots.py` & `panda_server-0.3.4/pandaserver/daemons/scripts/cache_pilots.py`

 * *Files identical despite different names*

### Comparing `panda_server-0.3.3/pandaserver/daemons/scripts/cache_schedconfig.py` & `panda_server-0.3.4/pandaserver/daemons/scripts/cache_schedconfig.py`

 * *Files identical despite different names*

### Comparing `panda_server-0.3.3/pandaserver/daemons/scripts/carbon.py` & `panda_server-0.3.4/pandaserver/daemons/scripts/carbon.py`

 * *Files identical despite different names*

### Comparing `panda_server-0.3.3/pandaserver/daemons/scripts/configurator.py` & `panda_server-0.3.4/pandaserver/daemons/scripts/configurator.py`

 * *Files identical despite different names*

### Comparing `panda_server-0.3.3/pandaserver/daemons/scripts/copyArchive.py` & `panda_server-0.3.4/pandaserver/daemons/scripts/copyArchive.py`

 * *Files identical despite different names*

### Comparing `panda_server-0.3.3/pandaserver/daemons/scripts/datasetManager.py` & `panda_server-0.3.4/pandaserver/daemons/scripts/datasetManager.py`

 * *Files identical despite different names*

### Comparing `panda_server-0.3.3/pandaserver/daemons/scripts/evpPD2P.py` & `panda_server-0.3.4/pandaserver/daemons/scripts/evpPD2P.py`

 * *Files identical despite different names*

### Comparing `panda_server-0.3.3/pandaserver/daemons/scripts/metric_collector.py` & `panda_server-0.3.4/pandaserver/daemons/scripts/metric_collector.py`

 * *Files identical despite different names*

### Comparing `panda_server-0.3.3/pandaserver/daemons/scripts/panda_activeusers_query.py` & `panda_server-0.3.4/pandaserver/daemons/scripts/panda_activeusers_query.py`

 * *Files identical despite different names*

### Comparing `panda_server-0.3.3/pandaserver/daemons/scripts/pilotStreaming.py` & `panda_server-0.3.4/pandaserver/daemons/scripts/pilotStreaming.py`

 * *Files identical despite different names*

### Comparing `panda_server-0.3.3/pandaserver/daemons/scripts/process_workflow_files_daemon.py` & `panda_server-0.3.4/pandaserver/daemons/scripts/process_workflow_files_daemon.py`

 * *Files identical despite different names*

### Comparing `panda_server-0.3.3/pandaserver/daemons/scripts/recover_lost_files_daemon.py` & `panda_server-0.3.4/pandaserver/daemons/scripts/recover_lost_files_daemon.py`

 * *Files identical despite different names*

### Comparing `panda_server-0.3.3/pandaserver/daemons/scripts/task_evaluator.py` & `panda_server-0.3.4/pandaserver/daemons/scripts/task_evaluator.py`

 * *Files identical despite different names*

### Comparing `panda_server-0.3.3/pandaserver/daemons/scripts/tmpwatch.py` & `panda_server-0.3.4/pandaserver/daemons/scripts/tmpwatch.py`

 * *Files identical despite different names*

### Comparing `panda_server-0.3.3/pandaserver/daemons/scripts/worker_synchronization.py` & `panda_server-0.3.4/pandaserver/daemons/scripts/worker_synchronization.py`

 * *Files identical despite different names*

### Comparing `panda_server-0.3.3/pandaserver/dataservice/AdderAtlasPlugin.py` & `panda_server-0.3.4/pandaserver/dataservice/AdderAtlasPlugin.py`

 * *Files identical despite different names*

### Comparing `panda_server-0.3.3/pandaserver/dataservice/AdderGen.py` & `panda_server-0.3.4/pandaserver/dataservice/AdderGen.py`

 * *Files identical despite different names*

### Comparing `panda_server-0.3.3/pandaserver/dataservice/AdderResult.py` & `panda_server-0.3.4/pandaserver/dataservice/AdderResult.py`

 * *Files identical despite different names*

### Comparing `panda_server-0.3.3/pandaserver/dataservice/AdderSimplePlugin.py` & `panda_server-0.3.4/pandaserver/dataservice/AdderSimplePlugin.py`

 * *Files identical despite different names*

### Comparing `panda_server-0.3.3/pandaserver/dataservice/DataServiceUtils.py` & `panda_server-0.3.4/pandaserver/dataservice/DataServiceUtils.py`

 * *Files identical despite different names*

### Comparing `panda_server-0.3.3/pandaserver/dataservice/ProcessLimiter.py` & `panda_server-0.3.4/pandaserver/dataservice/ProcessLimiter.py`

 * *Files identical despite different names*

### Comparing `panda_server-0.3.3/pandaserver/dataservice/RecoverLostFilesCore.py` & `panda_server-0.3.4/pandaserver/dataservice/RecoverLostFilesCore.py`

 * *Files identical despite different names*

### Comparing `panda_server-0.3.3/pandaserver/dataservice/Setupper.py` & `panda_server-0.3.4/pandaserver/dataservice/Setupper.py`

 * *Files identical despite different names*

### Comparing `panda_server-0.3.3/pandaserver/dataservice/SetupperAtlasPlugin.py` & `panda_server-0.3.4/pandaserver/dataservice/SetupperAtlasPlugin.py`

 * *Files identical despite different names*

### Comparing `panda_server-0.3.3/pandaserver/dataservice/SetupperDummyPlugin.py` & `panda_server-0.3.4/pandaserver/dataservice/SetupperDummyPlugin.py`

 * *Files identical despite different names*

### Comparing `panda_server-0.3.3/pandaserver/dataservice/SetupperPluginBase.py` & `panda_server-0.3.4/pandaserver/dataservice/SetupperPluginBase.py`

 * *Files identical despite different names*

### Comparing `panda_server-0.3.3/pandaserver/dataservice/activator.py` & `panda_server-0.3.4/pandaserver/dataservice/activator.py`

 * *Files identical despite different names*

### Comparing `panda_server-0.3.3/pandaserver/dataservice/closer.py` & `panda_server-0.3.4/pandaserver/dataservice/closer.py`

 * *Files identical despite different names*

### Comparing `panda_server-0.3.3/pandaserver/dataservice/closer_atlas_plugin.py` & `panda_server-0.3.4/pandaserver/dataservice/closer_atlas_plugin.py`

 * *Files identical despite different names*

### Comparing `panda_server-0.3.3/pandaserver/dataservice/ddm.py` & `panda_server-0.3.4/pandaserver/dataservice/ddm.py`

 * *Files identical despite different names*

### Comparing `panda_server-0.3.3/pandaserver/dataservice/ddm_handler.py` & `panda_server-0.3.4/pandaserver/dataservice/ddm_handler.py`

 * *Files identical despite different names*

### Comparing `panda_server-0.3.3/pandaserver/dataservice/dyn_data_distributer.py` & `panda_server-0.3.4/pandaserver/dataservice/dyn_data_distributer.py`

 * *Files identical despite different names*

### Comparing `panda_server-0.3.3/pandaserver/dataservice/event_lookup_client_ei.py` & `panda_server-0.3.4/pandaserver/dataservice/event_lookup_client_ei.py`

 * *Files identical despite different names*

### Comparing `panda_server-0.3.3/pandaserver/dataservice/event_picker.py` & `panda_server-0.3.4/pandaserver/dataservice/event_picker.py`

 * *Files identical despite different names*

### Comparing `panda_server-0.3.3/pandaserver/dataservice/finisher.py` & `panda_server-0.3.4/pandaserver/dataservice/finisher.py`

 * *Files identical despite different names*

### Comparing `panda_server-0.3.3/pandaserver/dataservice/forkSetupper.py` & `panda_server-0.3.4/pandaserver/dataservice/forkSetupper.py`

 * *Files identical despite different names*

### Comparing `panda_server-0.3.3/pandaserver/jobdispatcher/DispatcherUtils.py` & `panda_server-0.3.4/pandaserver/jobdispatcher/DispatcherUtils.py`

 * *Files identical despite different names*

### Comparing `panda_server-0.3.3/pandaserver/jobdispatcher/JobDispatcher.py` & `panda_server-0.3.4/pandaserver/jobdispatcher/JobDispatcher.py`

 * *Files identical despite different names*

### Comparing `panda_server-0.3.3/pandaserver/jobdispatcher/Protocol.py` & `panda_server-0.3.4/pandaserver/jobdispatcher/Protocol.py`

 * *Files identical despite different names*

### Comparing `panda_server-0.3.3/pandaserver/jobdispatcher/Watcher.py` & `panda_server-0.3.4/pandaserver/jobdispatcher/Watcher.py`

 * *Files identical despite different names*

### Comparing `panda_server-0.3.3/pandaserver/proxycache/panda_proxy_cache.py` & `panda_server-0.3.4/pandaserver/proxycache/panda_proxy_cache.py`

 * *Files identical despite different names*

### Comparing `panda_server-0.3.3/pandaserver/server/panda.py` & `panda_server-0.3.4/pandaserver/server/panda.py`

 * *Files identical despite different names*

### Comparing `panda_server-0.3.3/pandaserver/srvcore/CoreUtils.py` & `panda_server-0.3.4/pandaserver/srvcore/CoreUtils.py`

 * *Files identical despite different names*

### Comparing `panda_server-0.3.3/pandaserver/srvcore/MailUtils.py` & `panda_server-0.3.4/pandaserver/srvcore/MailUtils.py`

 * *Files identical despite different names*

### Comparing `panda_server-0.3.3/pandaserver/srvcore/allowed_methods.py` & `panda_server-0.3.4/pandaserver/srvcore/allowed_methods.py`

 * *Files identical despite different names*

### Comparing `panda_server-0.3.3/pandaserver/srvcore/oidc_utils.py` & `panda_server-0.3.4/pandaserver/srvcore/oidc_utils.py`

 * *Files identical despite different names*

### Comparing `panda_server-0.3.3/pandaserver/srvcore/panda_request.py` & `panda_server-0.3.4/pandaserver/srvcore/panda_request.py`

 * *Files identical despite different names*

### Comparing `panda_server-0.3.3/pandaserver/srvcore/srv_msg_utils.py` & `panda_server-0.3.4/pandaserver/srvcore/srv_msg_utils.py`

 * *Files identical despite different names*

### Comparing `panda_server-0.3.3/pandaserver/taskbuffer/CloudSpec.py` & `panda_server-0.3.4/pandaserver/taskbuffer/CloudSpec.py`

 * *Files identical despite different names*

### Comparing `panda_server-0.3.3/pandaserver/taskbuffer/CloudTaskSpec.py` & `panda_server-0.3.4/pandaserver/taskbuffer/CloudTaskSpec.py`

 * *Files identical despite different names*

### Comparing `panda_server-0.3.3/pandaserver/taskbuffer/ConBridge.py` & `panda_server-0.3.4/pandaserver/taskbuffer/ConBridge.py`

 * *Files identical despite different names*

### Comparing `panda_server-0.3.3/pandaserver/taskbuffer/DBProxyPool.py` & `panda_server-0.3.4/pandaserver/taskbuffer/DBProxyPool.py`

 * *Files identical despite different names*

### Comparing `panda_server-0.3.3/pandaserver/taskbuffer/DatasetSpec.py` & `panda_server-0.3.4/pandaserver/taskbuffer/DatasetSpec.py`

 * *Files identical despite different names*

### Comparing `panda_server-0.3.3/pandaserver/taskbuffer/DdmSpec.py` & `panda_server-0.3.4/pandaserver/taskbuffer/DdmSpec.py`

 * *Files identical despite different names*

### Comparing `panda_server-0.3.3/pandaserver/taskbuffer/ErrorCode.py` & `panda_server-0.3.4/pandaserver/taskbuffer/ErrorCode.py`

 * *Files identical despite different names*

### Comparing `panda_server-0.3.3/pandaserver/taskbuffer/EventServiceUtils.py` & `panda_server-0.3.4/pandaserver/taskbuffer/EventServiceUtils.py`

 * *Files identical despite different names*

### Comparing `panda_server-0.3.3/pandaserver/taskbuffer/FileSpec.py` & `panda_server-0.3.4/pandaserver/taskbuffer/FileSpec.py`

 * *Files identical despite different names*

### Comparing `panda_server-0.3.3/pandaserver/taskbuffer/GlobalShares.py` & `panda_server-0.3.4/pandaserver/taskbuffer/GlobalShares.py`

 * *Files identical despite different names*

### Comparing `panda_server-0.3.3/pandaserver/taskbuffer/HarvesterMetricsSpec.py` & `panda_server-0.3.4/pandaserver/taskbuffer/HarvesterMetricsSpec.py`

 * *Files identical despite different names*

### Comparing `panda_server-0.3.3/pandaserver/taskbuffer/Initializer.py` & `panda_server-0.3.4/pandaserver/taskbuffer/Initializer.py`

 * *Files identical despite different names*

### Comparing `panda_server-0.3.3/pandaserver/taskbuffer/JobSpec.py` & `panda_server-0.3.4/pandaserver/taskbuffer/JobSpec.py`

 * *Files identical despite different names*

### Comparing `panda_server-0.3.3/pandaserver/taskbuffer/JobUtils.py` & `panda_server-0.3.4/pandaserver/taskbuffer/JobUtils.py`

 * *Files 2% similar despite different names*

```diff
@@ -22,22 +22,14 @@
 
 job_labels = [ANALY_PS, PROD_PS]
 
 # priority of tasks to jumbo over others
 priorityTasksToJumpOver = 1500
 
 
-def translate_resourcetype_to_cores(resource_type, cores_queue):
-    # resolve the multiplying core factor
-    if "MCORE" in resource_type:
-        return cores_queue
-    else:
-        return 1
-
-
 def translate_prodsourcelabel_to_jobtype(queue_type, prodsourcelabel):
     if prodsourcelabel in analy_sources:
         return ANALY_PS
 
     if prodsourcelabel in prod_sources:
         return PROD_PS
```

### Comparing `panda_server-0.3.3/pandaserver/taskbuffer/NucleusSpec.py` & `panda_server-0.3.4/pandaserver/taskbuffer/NucleusSpec.py`

 * *Files identical despite different names*

### Comparing `panda_server-0.3.3/pandaserver/taskbuffer/OraDBProxy.py` & `panda_server-0.3.4/pandaserver/taskbuffer/OraDBProxy.py`

 * *Files 0% similar despite different names*

```diff
@@ -39,15 +39,19 @@
 )
 from pandaserver.taskbuffer.CloudTaskSpec import CloudTaskSpec
 from pandaserver.taskbuffer.DatasetSpec import DatasetSpec
 from pandaserver.taskbuffer.DdmSpec import DdmSpec
 from pandaserver.taskbuffer.FileSpec import FileSpec
 from pandaserver.taskbuffer.HarvesterMetricsSpec import HarvesterMetricsSpec
 from pandaserver.taskbuffer.JobSpec import JobSpec, push_status_changes
-from pandaserver.taskbuffer.ResourceSpec import ResourceSpec
+from pandaserver.taskbuffer.ResourceSpec import (
+    BASIC_RESOURCE_TYPE,
+    ResourceSpec,
+    ResourceSpecMapper,
+)
 from pandaserver.taskbuffer.SupErrors import SupErrors
 from pandaserver.taskbuffer.Utils import create_shards
 from pandaserver.taskbuffer.WorkerSpec import WorkerSpec
 from pandaserver.taskbuffer.WrappedCursor import WrappedCursor
 
 try:
     import idds.common.constants
@@ -152,27 +156,29 @@
         # global share variables
         self.tree = None  # Pointer to the root of the global shares tree
         self.leave_shares = None  # Pointer to the list with leave shares
         self.__t_update_shares = None  # Timestamp when the shares were last updated
         self.__hs_distribution = None  # HS06s distribution of sites
         self.__t_update_distribution = None  # Timestamp when the HS06s distribution was last updated
 
+        # resource type mapper
+        # if you want to use it, you need to call __reload_resource_spec_mapper first
+        self.__resource_spec_mapper = None
+        self.__t_update_resource_type_mapper = None
+
         # priority boost
         self.job_prio_boost_dict = None
         self.job_prio_boost_dict_update_time = None
 
         # keep type
         self.__orig_type = type
 
         # mb proxy
         self.mb_proxy_dict = None
 
-        # self.__reload_shares()
-        # self.__reload_hs_distribution()
-
     # connect to DB
     def connect(
         self,
         dbhost=panda_config.dbhost,
         dbpasswd=panda_config.dbpasswd,
         dbuser=panda_config.dbuser,
         dbname=panda_config.dbname,
@@ -16805,15 +16811,15 @@
                     _logger.info(f"{methodName} set merge site to {newSiteName}")
                     break
         # return
         return
 
     # set score site to ES job
     def setScoreSiteToEs(self, jobSpec, methodName, comment):
-        _logger.debug(f"{methodName} looking for SCORE site")
+        _logger.debug(f"{methodName} looking for single-core site")
 
         # get score PQ in the nucleus associated to the site to run the small ES job
         sqlSN = "SELECT /* use_json_type */ ps2.panda_site_name "
         sqlSN += "FROM ATLAS_PANDA.panda_site ps1, ATLAS_PANDA.panda_site ps2, ATLAS_PANDA.schedconfig_json sc "
         sqlSN += "WHERE ps1.panda_site_name=:site AND ps1.site_name=ps2.site_name AND sc.panda_queue=ps2.panda_site_name "
         sqlSN += "AND (sc.data.corecount IS NULL OR sc.data.corecount=1 OR sc.data.capability=:capability) "
         sqlSN += "AND (sc.data.jobseed IS NULL OR sc.data.jobseed<>'std') "
@@ -16863,17 +16869,17 @@
                 maxNumPilot = nPilots
                 jobSpec.computingSite = tmp_panda_site_name
                 jobSpec.coreCount = 1
                 jobSpec.minRamCount = 0
                 jobSpec.resource_type = self.get_resource_type_job(jobSpec)
                 newSiteName = jobSpec.computingSite
         if newSiteName is not None:
-            _logger.info(f"{methodName} set SCORE site to {newSiteName}")
+            _logger.info(f"{methodName} set single-core site to {newSiteName}")
         else:
-            _logger.info(f"{methodName} no SCORE site for {jobSpec.computingSite}")
+            _logger.info(f"{methodName} no single-core site for {jobSpec.computingSite}")
         # return
         return
 
     # change task priority
     def changeTaskPriorityPanda(self, jediTaskID, newPriority):
         comment = " /* DBProxy.changeTaskPriorityPanda */"
         methodName = comment.split(" ")[-2].split(".")[-1]
@@ -22668,14 +22674,26 @@
             # roll back
             self._rollback()
             type, value, traceback = sys.exc_info()
             _logger.error(f"{comment}: {sql} {var_map}")
             _logger.error(f"{comment}: {type} {value}")
             return -1
 
+    def __reload_resource_spec_mapper(self):
+        # update once per hour only
+        if self.__t_update_resource_type_mapper and self.__t_update_resource_type_mapper > datetime.datetime.now() - datetime.timedelta(hours=1):
+            return
+
+        # get the resource types from the DB and make the ResourceSpecMapper object
+        resource_types = self.load_resource_types()
+        if resource_types:
+            self.__resource_spec_mapper = ResourceSpecMapper(resource_types)
+            self.__t_update_resource_type_mapper = datetime.datetime.now()
+        return
+
     def load_resource_types(self, formatting="spec"):
         """
         Load the resource type table to memory
         """
         comment = " /* JediDBProxy.load_resource_types */"
         method_name = comment.split(" ")[-2].split(".")[-1]
         tmp_log = LogWrapper(_logger, method_name)
@@ -22868,65 +22886,82 @@
         except Exception:
             # roll back
             self._rollback()
             self.dumpErrorMessage(tmpLog, methodName)
             return False, "database error"
 
     # update stat of workers with jobtype breakdown
-    def reportWorkerStats_jobtype(self, harvesterID, siteName, paramsList):
+    def reportWorkerStats_jobtype(self, harvesterID, siteName, parameter_list):
         comment = " /* DBProxy.reportWorkerStats_jobtype */"
-        methodName = comment.split(" ")[-2].split(".")[-1]
-        tmpLog = LogWrapper(
+        method_name = comment.split(" ")[-2].split(".")[-1]
+        tmp_log = LogWrapper(
             _logger,
-            methodName + f" < harvesterID={harvesterID} siteName={siteName} >",
+            f"{method_name} < harvesterID={harvesterID} siteName={siteName} >",
         )
-        tmpLog.debug("start")
-        tmpLog.debug(f"params={str(paramsList)}")
+        tmp_log.debug("start")
+        tmp_log.debug(f"params={str(parameter_list)}")
         try:
             # load new site data
-            paramsList = json.loads(paramsList)
+            parameter_list = json.loads(parameter_list)
             # set autocommit on
             self.conn.begin()
-            # delete old site data
-            sqlDel = "DELETE FROM ATLAS_PANDA.Harvester_Worker_Stats "
-            sqlDel += "WHERE harvester_ID=:harvesterID AND computingSite=:siteName "
-            varMap = dict()
-            varMap[":harvesterID"] = harvesterID
-            varMap[":siteName"] = siteName
-            self.cur.execute(sqlDel + comment, varMap)
+
+            # lock the site data rows
+            var_map = dict()
+            var_map[":harvesterID"] = harvesterID
+            var_map[":siteName"] = siteName
+            sql_lock = "SELECT harvester_ID, computingSite FROM ATLAS_PANDA.Harvester_Worker_Stats "
+            sql_lock += "WHERE harvester_ID=:harvesterID AND computingSite=:siteName FOR UPDATE NOWAIT "
+            try:
+                self.cur.execute(sql_lock + comment, var_map)
+            except Exception:
+                self._rollback()
+                message = "rows locked by another update"
+                tmp_log.debug(message)
+                tmp_log.debug("done")
+                return False, message
+
+            # delete them
+            sql_delete = "DELETE FROM ATLAS_PANDA.Harvester_Worker_Stats "
+            sql_delete += "WHERE harvester_ID=:harvesterID AND computingSite=:siteName "
+            self.cur.execute(sql_delete + comment, var_map)
+
             # insert new site data
-            sqlI = "INSERT INTO ATLAS_PANDA.Harvester_Worker_Stats (harvester_ID, computingSite, jobType, resourceType, status, n_workers, lastUpdate) "
-            sqlI += "VALUES (:harvester_ID, :siteName, :jobType, :resourceType, :status, :n_workers, CURRENT_DATE) "
+            sql_insert = "INSERT INTO ATLAS_PANDA.Harvester_Worker_Stats (harvester_ID, computingSite, jobType, resourceType, status, n_workers, lastUpdate) "
+            sql_insert += "VALUES (:harvester_ID, :siteName, :jobType, :resourceType, :status, :n_workers, CURRENT_DATE) "
 
-            for jobType in paramsList:
-                jt_params = paramsList[jobType]
+            var_map_list = []
+            for jobType in parameter_list:
+                jt_params = parameter_list[jobType]
                 for resourceType in jt_params:
                     params = jt_params[resourceType]
                     if resourceType == "Undefined":
                         continue
                     for status in params:
                         n_workers = params[status]
-                        varMap = dict()
-                        varMap[":harvester_ID"] = harvesterID
-                        varMap[":siteName"] = siteName
-                        varMap[":status"] = status
-                        varMap[":jobType"] = jobType
-                        varMap[":resourceType"] = resourceType
-                        varMap[":n_workers"] = n_workers
-                        self.cur.execute(sqlI + comment, varMap)
-            # commit
+                        var_map = {
+                            ":harvester_ID": harvesterID,
+                            ":siteName": siteName,
+                            ":status": status,
+                            ":jobType": jobType,
+                            ":resourceType": resourceType,
+                            ":n_workers": n_workers,
+                        }
+                        var_map_list.append(var_map)
+
+            self.cur.executemany(sql_insert + comment, var_map_list)
+
             if not self._commit():
                 raise RuntimeError("Commit error")
-            # return
-            tmpLog.debug("done")
+
+            tmp_log.debug("done")
             return True, "OK"
-        except Exception:
-            # roll back
+        except Exception as e:
             self._rollback()
-            self.dumpErrorMessage(tmpLog, methodName)
+            self.dumpErrorMessage(tmp_log, method_name)
             return False, "database error"
 
     # get stat of workers
     def getWorkerStats(self):
         comment = " /* DBProxy.getWorkerStats */"
         methodName = comment.split(" ")[-2].split(".")[-1]
         tmpLog = LogWrapper(_logger)
@@ -23408,48 +23443,47 @@
         :param queue: name of the queue
         :param worker_stats: queue worker stats
         :return:
         """
 
         comment = " /* DBProxy.ups_new_worker_distribution */"
         method_name = comment.split(" ")[-2].split(".")[-1]
-        tmpLog = LogWrapper(_logger, f"{method_name}-{queue}")
-        tmpLog.debug("start")
+        tmp_log = LogWrapper(_logger, f"{method_name}-{queue}")
+        tmp_log.debug("start")
         n_cores_running = 0
         workers_queued = {}
         n_cores_queued = 0
         harvester_ids_temp = list(worker_stats)
 
-        # HIMEM resource types group
         HIMEM = "HIMEM"
-        HIMEM_RTS = ["SCORE_HIMEM", "MCORE_HIMEM"]
+        self.__reload_resource_spec_mapper()
 
         # get the configuration for maximum workers of each type
         pq_data_des = self.get_config_for_pq(queue)
         resource_type_limits = {}
         queue_type = "production"
         if not pq_data_des:
-            tmpLog.debug("Error retrieving queue configuration from DB, limits can not be applied")
+            tmp_log.debug("Error retrieving queue configuration from DB, limits can not be applied")
         else:
             try:
                 resource_type_limits = pq_data_des["uconfig"]["resource_type_limits"]
             except KeyError:
-                tmpLog.debug("No resource type limits")
+                tmp_log.debug("No resource type limits")
                 pass
             try:
                 queue_type = pq_data_des["type"]
             except KeyError:
-                tmpLog.error("No queue type")
+                tmp_log.error("No queue type")
                 pass
             try:
                 cores_queue = pq_data_des["corecount"]
                 if not cores_queue:
                     cores_queue = 1
             except KeyError:
-                tmpLog.error("No corecount")
+                tmp_log.error("No corecount")
                 pass
 
         # Retrieve the assigned harvester instance and submit UPS commands only to this instance. We have had multiple
         # cases of test instances submitting to large queues in classic pull mode and not following commands.
         try:
             assigned_harvester_id = pq_data_des["harvester"]
         except KeyErrorException:
@@ -23466,31 +23500,31 @@
                 if "ACT" not in harvester_id and "test_fbarreir" not in harvester_id and "cern_cloud" not in harvester_id:
                     harvester_ids.append(harvester_id)
 
         for harvester_id in harvester_ids:
             for job_type in worker_stats[harvester_id]:
                 workers_queued.setdefault(job_type, {})
                 for resource_type in worker_stats[harvester_id][job_type]:
-                    core_factor = JobUtils.translate_resourcetype_to_cores(resource_type, cores_queue)
+                    core_factor = self.__resource_spec_mapper.translate_resourcetype_to_cores(resource_type, cores_queue)
                     try:
                         n_cores_running = n_cores_running + worker_stats[harvester_id][job_type][resource_type]["running"] * core_factor
 
                         # This limit is in #JOBS or #WORKERS
                         if resource_type in resource_type_limits:
                             resource_type_limits[resource_type] = (
                                 resource_type_limits[resource_type] - worker_stats[harvester_id][job_type][resource_type]["running"]
                             )
-                            tmpLog.debug(f"Limit for rt {resource_type} down to {resource_type_limits[resource_type]}")
+                            tmp_log.debug(f"Limit for rt {resource_type} down to {resource_type_limits[resource_type]}")
 
                         # This limit is in #CORES, since it mixes single and multi core jobs
-                        if resource_type in HIMEM_RTS and HIMEM in resource_type_limits:
+                        if self.__resource_spec_mapper.is_high_memory(resource_type) and HIMEM in resource_type_limits:
                             resource_type_limits[HIMEM] = (
                                 resource_type_limits[HIMEM] - worker_stats[harvester_id][job_type][resource_type]["running"] * core_factor
                             )
-                            tmpLog.debug(f"Limit for rt group {HIMEM} down to {resource_type_limits[HIMEM]}")
+                            tmp_log.debug(f"Limit for rt group {HIMEM} down to {resource_type_limits[HIMEM]}")
 
                     except KeyError:
                         pass
 
                     try:  # submitted
                         workers_queued[job_type].setdefault(resource_type, 0)
                         workers_queued[job_type][resource_type] = (
@@ -23505,33 +23539,33 @@
                         workers_queued[job_type][resource_type] = (
                             workers_queued[job_type][resource_type] + worker_stats[harvester_id][job_type][resource_type]["ready"]
                         )
                         n_cores_queued = n_cores_queued + worker_stats[harvester_id][job_type][resource_type]["ready"] * core_factor
                     except KeyError:
                         pass
 
-        tmpLog.debug(f"Queue {queue} queued worker overview: {workers_queued}")
+        tmp_log.debug(f"Queue {queue} queued worker overview: {workers_queued}")
 
         # For queues that need more pressure towards reaching a target
         n_cores_running_fake = 0
         try:
             if pq_data_des["status"] in [
                 "online",
                 "brokeroff",
             ]:  # don't flood test sites with workers
                 n_cores_running_fake = pq_data_des["params"]["ups_core_target"]
-                tmpLog.debug(f"Using ups_core_target {n_cores_running_fake} for queue {queue}")
-        except KeyError:  # no value defined in AGIS
+                tmp_log.debug(f"Using ups_core_target {n_cores_running_fake} for queue {queue}")
+        except KeyError:  # no value defined in CRIC
             pass
 
         n_cores_running = max(n_cores_running, n_cores_running_fake)
 
         n_cores_target = max(int(n_cores_running * 0.4), 75 * cores_queue)
         n_cores_to_submit = max(n_cores_target - n_cores_queued, 5 * cores_queue)
-        tmpLog.debug(f"IN CORES: nrunning {n_cores_running}, ntarget {n_cores_target}, nqueued {n_cores_queued}. We need to process {n_cores_to_submit} cores")
+        tmp_log.debug(f"IN CORES: nrunning {n_cores_running}, ntarget {n_cores_target}, nqueued {n_cores_queued}. We need to process {n_cores_to_submit} cores")
 
         # Get the sorted global shares
         sorted_shares = self.get_sorted_leaves()
 
         # Run over the activated jobs by gshare & priority, and substract them from the queued
         # A negative value for queued will mean more pilots of that resource type are missing
         for share in sorted_shares:
@@ -23541,83 +23575,83 @@
                   WHERE jobstatus = 'activated'
                      AND computingsite=:queue
                      AND gshare=:gshare
                   ORDER BY currentpriority DESC
                   """
             self.cur.execute(sql + comment, var_map)
             activated_jobs = self.cur.fetchall()
-            tmpLog.debug(f"Processing share: {share.name}. Got {len(activated_jobs)} activated jobs")
+            tmp_log.debug(f"Processing share: {share.name}. Got {len(activated_jobs)} activated jobs")
             for gshare, prodsourcelabel, resource_type in activated_jobs:
-                core_factor = JobUtils.translate_resourcetype_to_cores(resource_type, cores_queue)
+                core_factor = self.__resource_spec_mapper.translate_resourcetype_to_cores(resource_type, cores_queue)
 
                 # translate prodsourcelabel to a subset of job types, typically 'user' and 'managed'
                 job_type = JobUtils.translate_prodsourcelabel_to_jobtype(queue_type, prodsourcelabel)
                 # if we reached the limit for the resource type, skip the job
                 if resource_type in resource_type_limits and resource_type_limits[resource_type] <= 0:
-                    # tmpLog.debug('Reached resource type limit for {0}'.format(resource_type))
+                    # tmp_log.debug('Reached resource type limit for {0}'.format(resource_type))
                     continue
 
                 # if we reached the limit for the HIMEM resource type group, skip the job
-                if resource_type in HIMEM_RTS and HIMEM in resource_type_limits and resource_type_limits[HIMEM] <= 0:
-                    # tmpLog.debug('Reached resource type limit for {0}'.format(resource_type))
+                if self.__resource_spec_mapper.is_high_memory(resource_type) and HIMEM in resource_type_limits and resource_type_limits[HIMEM] <= 0:
+                    # tmp_log.debug('Reached resource type limit for {0}'.format(resource_type))
                     continue
 
                 workers_queued.setdefault(job_type, {})
                 workers_queued[job_type].setdefault(resource_type, 0)
                 workers_queued[job_type][resource_type] = workers_queued[job_type][resource_type] - 1
                 if workers_queued[job_type][resource_type] <= 0:
                     # we've gone over the jobs that already have a queued worker, now we go for new workers
                     n_cores_to_submit = n_cores_to_submit - core_factor
 
                 # We reached the number of workers needed
                 if n_cores_to_submit <= 0:
-                    tmpLog.debug("Reached cores needed (inner)")
+                    tmp_log.debug("Reached cores needed (inner)")
                     break
 
             # We reached the number of workers needed
             if n_cores_to_submit <= 0:
-                tmpLog.debug("Reached cores needed (outer)")
+                tmp_log.debug("Reached cores needed (outer)")
                 break
 
-        tmpLog.debug(f"workers_queued: {workers_queued}")
+        tmp_log.debug(f"workers_queued: {workers_queued}")
 
         new_workers = {}
         for job_type in workers_queued:
             new_workers.setdefault(job_type, {})
             for resource_type in workers_queued[job_type]:
                 if workers_queued[job_type][resource_type] >= 0:
                     # we have too many workers queued already, don't submit more
                     new_workers[job_type][resource_type] = 0
                 elif workers_queued[job_type][resource_type] < 0:
                     # we don't have enough workers for this resource type
                     new_workers[job_type][resource_type] = -workers_queued[job_type][resource_type] + 1
 
-        # We should still submit a SCORE worker, even if there are no activated jobs to avoid queue deactivation
+        # We should still submit a basic worker, even if there are no activated jobs to avoid queue deactivation
         workers = False
         for job_type in new_workers:
             for resource_type in new_workers[job_type]:
                 if new_workers[job_type][resource_type] > 0:
                     workers = True
                     break
         if not workers:
-            new_workers["managed"] = {"SCORE": 1}
+            new_workers["managed"] = {BASIC_RESOURCE_TYPE: 1}
 
         # In case multiple harvester instances are serving a panda queue, split workers evenly between them
         new_workers_per_harvester = {}
         for harvester_id in harvester_ids:
             new_workers_per_harvester.setdefault(harvester_id, {})
             for job_type in new_workers:
                 new_workers_per_harvester[harvester_id].setdefault(job_type, {})
                 for resource_type in new_workers[job_type]:
                     new_workers_per_harvester[harvester_id][job_type][resource_type] = int(
                         math.ceil(new_workers[job_type][resource_type] * 1.0 / len(harvester_ids))
                     )
 
-        tmpLog.debug(f"Workers to submit: {new_workers_per_harvester}")
-        tmpLog.debug("done")
+        tmp_log.debug(f"Workers to submit: {new_workers_per_harvester}")
+        tmp_log.debug("done")
         return new_workers_per_harvester
 
     # get active consumers
     def getActiveConsumers(self, jediTaskID, jobsetID, myPandaID):
         comment = " /* DBProxy.getActiveConsumers */"
         methodName = comment.split(" ")[-2].split(".")[-1]
         methodName += f" < jediTaskID={jediTaskID} jobsetID={jobsetID} PandaID={myPandaID} >"
```

### Comparing `panda_server-0.3.3/pandaserver/taskbuffer/PickleFileSpec.py` & `panda_server-0.3.4/pandaserver/taskbuffer/PickleFileSpec.py`

 * *Files identical despite different names*

### Comparing `panda_server-0.3.3/pandaserver/taskbuffer/PickleJobSpec.py` & `panda_server-0.3.4/pandaserver/taskbuffer/PickleJobSpec.py`

 * *Files identical despite different names*

### Comparing `panda_server-0.3.3/pandaserver/taskbuffer/PrioUtil.py` & `panda_server-0.3.4/pandaserver/taskbuffer/PrioUtil.py`

 * *Files identical despite different names*

### Comparing `panda_server-0.3.3/pandaserver/taskbuffer/ProcessGroups.py` & `panda_server-0.3.4/pandaserver/taskbuffer/ProcessGroups.py`

 * *Files identical despite different names*

### Comparing `panda_server-0.3.3/pandaserver/taskbuffer/SQLDumper.py` & `panda_server-0.3.4/pandaserver/taskbuffer/SQLDumper.py`

 * *Files identical despite different names*

### Comparing `panda_server-0.3.3/pandaserver/taskbuffer/SQLManager.py` & `panda_server-0.3.4/pandaserver/taskbuffer/SQLManager.py`

 * *Files identical despite different names*

### Comparing `panda_server-0.3.3/pandaserver/taskbuffer/SiteSpec.py` & `panda_server-0.3.4/pandaserver/taskbuffer/SiteSpec.py`

 * *Files 5% similar despite different names*

```diff
@@ -78,22 +78,14 @@
 
     # check if direct IO is used when tasks allow it
     def isDirectIO(self):
         if self.direct_access_lan is True:
             return True
         return False
 
-    # get resource type
-    def getResourceType(self):
-        if self.type == "analysis":
-            return "ANALY"
-        if self.coreCount > 1:
-            return "MCORE"
-        return "SCORE"
-
     # check what type of jobs are allowed
     def getJobSeed(self):
         tmpVal = self.jobseed
         if tmpVal is None:
             return "std"
         return tmpVal
 
@@ -153,15 +145,15 @@
     # get number of simulated events for dynamic number of events
     def get_n_sim_events(self):
         tmpVal = self.getValueFromCatchall("nSimEvents")
         if tmpVal is None:
             return None
         return int(tmpVal)
 
-    # get minimum of remainig events for jumbo jobs
+    # get minimum of remaining events for jumbo jobs
     def getMinEventsForJumbo(self):
         tmpVal = self.getValueFromCatchall("minEventsForJumbo")
         if tmpVal is None:
             return None
         return int(tmpVal)
 
     # check if opportunistic
```

### Comparing `panda_server-0.3.3/pandaserver/taskbuffer/TaskBuffer.py` & `panda_server-0.3.4/pandaserver/taskbuffer/TaskBuffer.py`

 * *Files 0% similar despite different names*

```diff
@@ -3576,15 +3576,15 @@
         # release DB proxy
         self.proxyPool.putProxy(proxy)
         # return
         return res
 
     def getResourceTypes(self):
         """
-        Get resource types (SCORE, MCORE, SCORE_HIMEM, MCORE_HIMEM) and their definitions
+        Get resource types (SCORE, MCORE, ...) and their definitions
         """
         # get DB proxy
         proxy = self.proxyPool.getProxy()
         # exec
         res = proxy.load_resource_types(formatting="dict")
         # release DB proxy
         self.proxyPool.putProxy(proxy)
```

### Comparing `panda_server-0.3.3/pandaserver/taskbuffer/TaskBufferInterface.py` & `panda_server-0.3.4/pandaserver/taskbuffer/TaskBufferInterface.py`

 * *Files identical despite different names*

### Comparing `panda_server-0.3.3/pandaserver/taskbuffer/Utils.py` & `panda_server-0.3.4/pandaserver/taskbuffer/Utils.py`

 * *Files identical despite different names*

### Comparing `panda_server-0.3.3/pandaserver/taskbuffer/WorkerSpec.py` & `panda_server-0.3.4/pandaserver/taskbuffer/WorkerSpec.py`

 * *Files identical despite different names*

### Comparing `panda_server-0.3.3/pandaserver/taskbuffer/WrappedCursor.py` & `panda_server-0.3.4/pandaserver/taskbuffer/WrappedCursor.py`

 * *Files identical despite different names*

### Comparing `panda_server-0.3.3/pandaserver/taskbuffer/WrappedPickle.py` & `panda_server-0.3.4/pandaserver/taskbuffer/WrappedPickle.py`

 * *Files identical despite different names*

### Comparing `panda_server-0.3.3/pandaserver/taskbuffer/retryModule.py` & `panda_server-0.3.4/pandaserver/taskbuffer/retryModule.py`

 * *Files identical despite different names*

### Comparing `panda_server-0.3.3/pandaserver/taskbuffer/task_split_rules.py` & `panda_server-0.3.4/pandaserver/taskbuffer/task_split_rules.py`

 * *Files identical despite different names*

### Comparing `panda_server-0.3.3/pandaserver/taskbuffer/workflow_processor.py` & `panda_server-0.3.4/pandaserver/taskbuffer/workflow_processor.py`

 * *Files identical despite different names*

### Comparing `panda_server-0.3.3/pandaserver/test/SchemaChecker.py` & `panda_server-0.3.4/pandaserver/test/SchemaChecker.py`

 * *Files identical despite different names*

### Comparing `panda_server-0.3.3/pandaserver/test/banUser.py` & `panda_server-0.3.4/pandaserver/test/banUser.py`

 * *Files identical despite different names*

### Comparing `panda_server-0.3.3/pandaserver/test/boostPrio.py` & `panda_server-0.3.4/pandaserver/test/boostPrio.py`

 * *Files identical despite different names*

### Comparing `panda_server-0.3.3/pandaserver/test/boostUser.py` & `panda_server-0.3.4/pandaserver/test/boostUser.py`

 * *Files identical despite different names*

### Comparing `panda_server-0.3.3/pandaserver/test/callbackDDM.py` & `panda_server-0.3.4/pandaserver/test/callbackDDM.py`

 * *Files identical despite different names*

### Comparing `panda_server-0.3.3/pandaserver/test/daod_on_demand.py` & `panda_server-0.3.4/pandaserver/test/daod_on_demand.py`

 * *Files identical despite different names*

### Comparing `panda_server-0.3.3/pandaserver/test/finishJob.py` & `panda_server-0.3.4/pandaserver/test/finishJob.py`

 * *Files identical despite different names*

### Comparing `panda_server-0.3.3/pandaserver/test/getJobs.py` & `panda_server-0.3.4/pandaserver/test/getJobs.py`

 * *Files identical despite different names*

### Comparing `panda_server-0.3.3/pandaserver/test/killJob.py` & `panda_server-0.3.4/pandaserver/test/killJob.py`

 * *Files identical despite different names*

### Comparing `panda_server-0.3.3/pandaserver/test/killJobLowPrio.py` & `panda_server-0.3.4/pandaserver/test/killJobLowPrio.py`

 * *Files identical despite different names*

### Comparing `panda_server-0.3.3/pandaserver/test/killJobsInTask.py` & `panda_server-0.3.4/pandaserver/test/killJobsInTask.py`

 * *Files identical despite different names*

### Comparing `panda_server-0.3.3/pandaserver/test/killProdJobs.py` & `panda_server-0.3.4/pandaserver/test/killProdJobs.py`

 * *Files identical despite different names*

### Comparing `panda_server-0.3.3/pandaserver/test/killTask.py` & `panda_server-0.3.4/pandaserver/test/killTask.py`

 * *Files identical despite different names*

### Comparing `panda_server-0.3.3/pandaserver/test/killUser.py` & `panda_server-0.3.4/pandaserver/test/killUser.py`

 * *Files identical despite different names*

### Comparing `panda_server-0.3.3/pandaserver/test/reassignSite.py` & `panda_server-0.3.4/pandaserver/test/reassignSite.py`

 * *Files identical despite different names*

### Comparing `panda_server-0.3.3/pandaserver/test/reassignTask.py` & `panda_server-0.3.4/pandaserver/test/reassignTask.py`

 * *Files identical despite different names*

### Comparing `panda_server-0.3.3/pandaserver/test/reassignWaiting.py` & `panda_server-0.3.4/pandaserver/test/reassignWaiting.py`

 * *Files identical despite different names*

### Comparing `panda_server-0.3.3/pandaserver/test/reloadInputDS.py` & `panda_server-0.3.4/pandaserver/test/reloadInputDS.py`

 * *Files identical despite different names*

### Comparing `panda_server-0.3.3/pandaserver/test/sendCommandToJob.py` & `panda_server-0.3.4/pandaserver/test/sendCommandToJob.py`

 * *Files identical despite different names*

### Comparing `panda_server-0.3.3/pandaserver/test/setDebugMode.py` & `panda_server-0.3.4/pandaserver/test/setDebugMode.py`

 * *Files identical despite different names*

### Comparing `panda_server-0.3.3/pandaserver/test/setPriority.py` & `panda_server-0.3.4/pandaserver/test/setPriority.py`

 * *Files identical despite different names*

### Comparing `panda_server-0.3.3/pandaserver/test/testEvgen.py` & `panda_server-0.3.4/pandaserver/test/testEvgen.py`

 * *Files identical despite different names*

### Comparing `panda_server-0.3.3/pandaserver/test/testEvgen17.py` & `panda_server-0.3.4/pandaserver/test/testEvgen17.py`

 * *Files identical despite different names*

### Comparing `panda_server-0.3.3/pandaserver/test/testG4sim.py` & `panda_server-0.3.4/pandaserver/test/testG4sim.py`

 * *Files identical despite different names*

### Comparing `panda_server-0.3.3/pandaserver/test/testG4sim17.py` & `panda_server-0.3.4/pandaserver/test/testG4sim17.py`

 * *Files identical despite different names*

### Comparing `panda_server-0.3.3/pandaserver/test/testGetCriteriaForGlobalShares.py` & `panda_server-0.3.4/pandaserver/test/testGetCriteriaForGlobalShares.py`

 * *Files identical despite different names*

### Comparing `panda_server-0.3.3/pandaserver/test/testGlobalShares.py` & `panda_server-0.3.4/pandaserver/test/testGlobalShares.py`

 * *Files identical despite different names*

### Comparing `panda_server-0.3.3/pandaserver/test/testJobFlowATLAS.py` & `panda_server-0.3.4/pandaserver/test/testJobFlowATLAS.py`

 * *Files identical despite different names*

### Comparing `panda_server-0.3.3/pandaserver/test/testReco.py` & `panda_server-0.3.4/pandaserver/test/testReco.py`

 * *Files identical despite different names*

### Comparing `panda_server-0.3.3/pandaserver/test/testSimulReco14.py` & `panda_server-0.3.4/pandaserver/test/testSimulReco14.py`

 * *Files identical despite different names*

### Comparing `panda_server-0.3.3/pandaserver/test/testSiteMap.py` & `panda_server-0.3.4/pandaserver/test/testSiteMap.py`

 * *Files identical despite different names*

### Comparing `panda_server-0.3.3/pandaserver/test/testutils.py` & `panda_server-0.3.4/pandaserver/test/testutils.py`

 * *Files identical despite different names*

### Comparing `panda_server-0.3.3/pandaserver/test/alice/titan_testScript_ec2_alice_1.py` & `panda_server-0.3.4/pandaserver/test/alice/titan_testScript_ec2_alice_1.py`

 * *Files identical despite different names*

### Comparing `panda_server-0.3.3/pandaserver/test/alice/titan_testScript_ec2_alice_2.py` & `panda_server-0.3.4/pandaserver/test/alice/titan_testScript_ec2_alice_2.py`

 * *Files identical despite different names*

### Comparing `panda_server-0.3.3/pandaserver/test/lsst/lsstSubmit.py` & `panda_server-0.3.4/pandaserver/test/lsst/lsstSubmit.py`

 * *Files identical despite different names*

### Comparing `panda_server-0.3.3/pandaserver/test/lsst/lsstSubmitMERGEtest.py` & `panda_server-0.3.4/pandaserver/test/lsst/lsstSubmitMERGEtest.py`

 * *Files identical despite different names*

### Comparing `panda_server-0.3.3/pandaserver/test/lsst/lsstSubmitPhosim332.py` & `panda_server-0.3.4/pandaserver/test/lsst/lsstSubmitPhosim332.py`

 * *Files identical despite different names*

### Comparing `panda_server-0.3.3/pandaserver/test/lsst/prepare-client-tarball-from-bigpanda-server.sh` & `panda_server-0.3.4/pandaserver/test/lsst/prepare-client-tarball-from-bigpanda-server.sh`

 * *Files identical despite different names*

### Comparing `panda_server-0.3.3/pandaserver/userinterface/Client.py` & `panda_server-0.3.4/pandaserver/userinterface/Client.py`

 * *Files identical despite different names*

### Comparing `panda_server-0.3.3/pandaserver/userinterface/UserIF.py` & `panda_server-0.3.4/pandaserver/userinterface/UserIF.py`

 * *Files identical despite different names*

### Comparing `panda_server-0.3.3/pandaserver/workflow/pcwl_test.py` & `panda_server-0.3.4/pandaserver/workflow/pcwl_test.py`

 * *Files identical despite different names*

### Comparing `panda_server-0.3.3/pandaserver/workflow/pcwl_utils.py` & `panda_server-0.3.4/pandaserver/workflow/pcwl_utils.py`

 * *Files identical despite different names*

### Comparing `panda_server-0.3.3/pandaserver/workflow/psnakemake_container.json` & `panda_server-0.3.4/pandaserver/workflow/psnakemake_container.json`

 * *Files identical despite different names*

### Comparing `panda_server-0.3.3/pandaserver/workflow/psnakemake_task.json` & `panda_server-0.3.4/pandaserver/workflow/psnakemake_task.json`

 * *Files identical despite different names*

### Comparing `panda_server-0.3.3/pandaserver/workflow/psnakemake_test.py` & `panda_server-0.3.4/pandaserver/workflow/psnakemake_test.py`

 * *Files identical despite different names*

### Comparing `panda_server-0.3.3/pandaserver/workflow/workflow_utils.py` & `panda_server-0.3.4/pandaserver/workflow/workflow_utils.py`

 * *Files identical despite different names*

### Comparing `panda_server-0.3.3/pandaserver/workflow/snakeparser/extensions.py` & `panda_server-0.3.4/pandaserver/workflow/snakeparser/extensions.py`

 * *Files identical despite different names*

### Comparing `panda_server-0.3.3/pandaserver/workflow/snakeparser/log.py` & `panda_server-0.3.4/pandaserver/workflow/snakeparser/log.py`

 * *Files identical despite different names*

### Comparing `panda_server-0.3.3/pandaserver/workflow/snakeparser/parser.py` & `panda_server-0.3.4/pandaserver/workflow/snakeparser/parser.py`

 * *Files identical despite different names*

### Comparing `panda_server-0.3.3/pandaserver/workflow/snakeparser/utils.py` & `panda_server-0.3.4/pandaserver/workflow/snakeparser/utils.py`

 * *Files identical despite different names*

### Comparing `panda_server-0.3.3/templates/conda_meta.yaml.template` & `panda_server-0.3.4/templates/conda_meta.yaml.template`

 * *Files identical despite different names*

### Comparing `panda_server-0.3.3/templates/panda_server-httpd-FastCGI.conf.rpmnew.template` & `panda_server-0.3.4/templates/panda_server-httpd-FastCGI.conf.rpmnew.template`

 * *Files identical despite different names*

### Comparing `panda_server-0.3.3/templates/panda_server-httpd.conf.rpmnew.template` & `panda_server-0.3.4/templates/panda_server-httpd.conf.rpmnew.template`

 * *Files identical despite different names*

### Comparing `panda_server-0.3.3/templates/panda_server.cfg.rpmnew.template` & `panda_server-0.3.4/templates/panda_server.cfg.rpmnew.template`

 * *Files identical despite different names*

### Comparing `panda_server-0.3.3/templates/bin/panda_server-makeSlsXml.exe.template` & `panda_server-0.3.4/templates/bin/panda_server-makeSlsXml.exe.template`

 * *Files identical despite different names*

### Comparing `panda_server-0.3.3/templates/bin/panda_server-vomsrenew.exe.template` & `panda_server-0.3.4/templates/bin/panda_server-vomsrenew.exe.template`

 * *Files identical despite different names*

### Comparing `panda_server-0.3.3/templates/init.d/panda_daemon.exe.template` & `panda_server-0.3.4/templates/init.d/panda_daemon.exe.template`

 * *Files identical despite different names*

### Comparing `panda_server-0.3.3/templates/init.d/panda_httpd.exe.template` & `panda_server-0.3.4/templates/init.d/panda_httpd.exe.template`

 * *Files identical despite different names*

### Comparing `panda_server-0.3.3/templates/init.d/panda_server.exe.template` & `panda_server-0.3.4/templates/init.d/panda_server.exe.template`

 * *Files identical despite different names*

### Comparing `panda_server-0.3.3/templates/logrotate.d/panda_server.logrotate.template` & `panda_server-0.3.4/templates/logrotate.d/panda_server.logrotate.template`

 * *Files identical despite different names*

### Comparing `panda_server-0.3.3/templates/sysconfig/panda_server.sysconfig.rpmnew.template` & `panda_server-0.3.4/templates/sysconfig/panda_server.sysconfig.rpmnew.template`

 * *Files identical despite different names*

### Comparing `panda_server-0.3.3/templates/sysconfig/panda_server_env.systemd.rpmnew.template` & `panda_server-0.3.4/templates/sysconfig/panda_server_env.systemd.rpmnew.template`

 * *Files identical despite different names*

### Comparing `panda_server-0.3.3/LICENSE.txt` & `panda_server-0.3.4/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `panda_server-0.3.3/pyproject.toml` & `panda_server-0.3.4/pyproject.toml`

 * *Files identical despite different names*

### Comparing `panda_server-0.3.3/PKG-INFO` & `panda_server-0.3.4/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: panda-server
-Version: 0.3.3
+Version: 0.3.4
 Summary: PanDA Server Package
 Project-URL: Homepage, https://panda-wms.readthedocs.io/en/latest/
 Author-email: PanDA Team <panda-support@cern.ch>
 License: Apache-2.0
 License-File: LICENSE.txt
 Requires-Python: >=3.8
 Requires-Dist: cwl-utils>=0.13
```

