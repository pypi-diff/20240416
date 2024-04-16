# Comparing `tmp/pysysq-0.1.1.tar.gz` & `tmp/pysysq-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pysysq-0.1.1.tar", last modified: Sat Apr  6 21:04:35 2024, max compression
+gzip compressed data, was "pysysq-0.1.2.tar", last modified: Mon Apr 15 19:59:44 2024, max compression
```

## Comparing `pysysq-0.1.1.tar` & `pysysq-0.1.2.tar`

### file list

```diff
@@ -1,118 +1,117 @@
-drwxrwxr-x   0 ajith     (1000) ajith     (1000)        0 2024-04-06 21:04:35.811643 pysysq-0.1.1/
--rw-rw-r--   0 ajith     (1000) ajith     (1000)     3113 2024-03-31 20:14:07.000000 pysysq-0.1.1/.gitignore
--rw-rw-r--   0 ajith     (1000) ajith     (1000)     1073 2024-03-31 20:14:07.000000 pysysq-0.1.1/LICENSE
--rw-r--r--   0 ajith     (1000) ajith     (1000)    11852 2024-04-06 21:04:35.811643 pysysq-0.1.1/PKG-INFO
--rw-rw-r--   0 ajith     (1000) ajith     (1000)   607908 2024-03-31 20:14:07.000000 pysysq-0.1.1/PysysQ.ipynb
--rw-rw-r--   0 ajith     (1000) ajith     (1000)     9238 2024-04-06 20:27:59.000000 pysysq-0.1.1/README.md
--rw-rw-r--   0 ajith     (1000) ajith     (1000)        0 2024-04-01 14:12:34.000000 pysysq-0.1.1/__init__.py
--rw-rw-r--   0 ajith     (1000) ajith     (1000)     1403 2024-04-06 21:04:30.000000 pysysq-0.1.1/pyproject.toml
--rw-rw-r--   0 ajith     (1000) ajith     (1000)      384 2024-03-31 20:14:07.000000 pysysq-0.1.1/requirements.txt
--rw-rw-r--   0 ajith     (1000) ajith     (1000)       38 2024-04-06 21:04:35.811643 pysysq-0.1.1/setup.cfg
-drwxrwxr-x   0 ajith     (1000) ajith     (1000)        0 2024-04-06 21:04:35.799642 pysysq-0.1.1/src/
-drwxrwxr-x   0 ajith     (1000) ajith     (1000)        0 2024-04-06 21:04:35.803643 pysysq-0.1.1/src/pysysq/
--rw-rw-r--   0 ajith     (1000) ajith     (1000)      188 2024-03-31 20:14:07.000000 pysysq-0.1.1/src/pysysq/__init__.py
--rw-rw-r--   0 ajith     (1000) ajith     (1000)      493 2024-03-31 20:20:58.000000 pysysq-0.1.1/src/pysysq/__main__.py
--rw-rw-r--   0 ajith     (1000) ajith     (1000)      465 2024-04-06 21:04:35.000000 pysysq-0.1.1/src/pysysq/_version.py
--rw-rw-r--   0 ajith     (1000) ajith     (1000)     2138 2024-03-31 20:14:07.000000 pysysq-0.1.1/src/pysysq/logging.conf
-drwxrwxr-x   0 ajith     (1000) ajith     (1000)        0 2024-04-06 21:04:35.803643 pysysq-0.1.1/src/pysysq/sq_base/
--rw-rw-r--   0 ajith     (1000) ajith     (1000)      475 2024-03-31 20:14:07.000000 pysysq-0.1.1/src/pysysq/sq_base/__init__.py
-drwxrwxr-x   0 ajith     (1000) ajith     (1000)        0 2024-04-06 21:04:35.803643 pysysq-0.1.1/src/pysysq/sq_base/sq_clock/
--rw-rw-r--   0 ajith     (1000) ajith     (1000)       30 2024-03-31 20:14:07.000000 pysysq-0.1.1/src/pysysq/sq_base/sq_clock/__init__.py
--rw-rw-r--   0 ajith     (1000) ajith     (1000)     1117 2024-04-06 09:26:43.000000 pysysq-0.1.1/src/pysysq/sq_base/sq_clock/sq_clock.py
-drwxrwxr-x   0 ajith     (1000) ajith     (1000)        0 2024-04-06 21:04:35.803643 pysysq-0.1.1/src/pysysq/sq_base/sq_event/
--rw-rw-r--   0 ajith     (1000) ajith     (1000)      127 2024-03-31 20:14:07.000000 pysysq-0.1.1/src/pysysq/sq_base/sq_event/__init__.py
--rw-rw-r--   0 ajith     (1000) ajith     (1000)      843 2024-03-31 20:14:07.000000 pysysq-0.1.1/src/pysysq/sq_base/sq_event/sq_event.py
--rw-rw-r--   0 ajith     (1000) ajith     (1000)     1965 2024-03-31 20:14:07.000000 pysysq-0.1.1/src/pysysq/sq_base/sq_event/sq_event_manager.py
--rw-rw-r--   0 ajith     (1000) ajith     (1000)     1183 2024-03-31 20:14:07.000000 pysysq-0.1.1/src/pysysq/sq_base/sq_event/sq_event_queue.py
-drwxrwxr-x   0 ajith     (1000) ajith     (1000)        0 2024-04-06 21:04:35.807643 pysysq-0.1.1/src/pysysq/sq_base/sq_factory/
--rw-rw-r--   0 ajith     (1000) ajith     (1000)       81 2024-04-06 10:06:37.000000 pysysq-0.1.1/src/pysysq/sq_base/sq_factory/__init__.py
--rw-rw-r--   0 ajith     (1000) ajith     (1000)     1973 2024-04-06 13:21:28.000000 pysysq-0.1.1/src/pysysq/sq_base/sq_factory/sq_factory.py
--rw-rw-r--   0 ajith     (1000) ajith     (1000)      443 2024-04-06 20:59:49.000000 pysysq-0.1.1/src/pysysq/sq_base/sq_factory/sq_helper_factory.py
-drwxrwxr-x   0 ajith     (1000) ajith     (1000)        0 2024-04-06 21:04:35.807643 pysysq-0.1.1/src/pysysq/sq_base/sq_filter/
--rw-rw-r--   0 ajith     (1000) ajith     (1000)       34 2024-04-01 14:12:25.000000 pysysq-0.1.1/src/pysysq/sq_base/sq_filter/__init__.py
--rw-rw-r--   0 ajith     (1000) ajith     (1000)     1446 2024-04-01 22:28:07.000000 pysysq-0.1.1/src/pysysq/sq_base/sq_filter/sq_filter.py
-drwxrwxr-x   0 ajith     (1000) ajith     (1000)        0 2024-04-06 21:04:35.807643 pysysq-0.1.1/src/pysysq/sq_base/sq_logger/
--rw-rw-r--   0 ajith     (1000) ajith     (1000)       32 2024-03-31 20:14:07.000000 pysysq-0.1.1/src/pysysq/sq_base/sq_logger/__init__.py
--rw-rw-r--   0 ajith     (1000) ajith     (1000)      892 2024-03-31 20:14:07.000000 pysysq-0.1.1/src/pysysq/sq_base/sq_logger/sq_logger.py
-drwxrwxr-x   0 ajith     (1000) ajith     (1000)        0 2024-04-06 21:04:35.807643 pysysq-0.1.1/src/pysysq/sq_base/sq_merger/
--rw-rw-r--   0 ajith     (1000) ajith     (1000)       31 2024-03-31 20:14:07.000000 pysysq-0.1.1/src/pysysq/sq_base/sq_merger/__init__.py
--rw-rw-r--   0 ajith     (1000) ajith     (1000)     1585 2024-04-01 14:12:25.000000 pysysq-0.1.1/src/pysysq/sq_base/sq_merger/sq_merger.py
-drwxrwxr-x   0 ajith     (1000) ajith     (1000)        0 2024-04-06 21:04:35.807643 pysysq-0.1.1/src/pysysq/sq_base/sq_mux_demux/
--rw-rw-r--   0 ajith     (1000) ajith     (1000)       59 2024-04-06 10:07:28.000000 pysysq-0.1.1/src/pysysq/sq_base/sq_mux_demux/__init__.py
--rw-rw-r--   0 ajith     (1000) ajith     (1000)     2168 2024-04-01 22:28:07.000000 pysysq-0.1.1/src/pysysq/sq_base/sq_mux_demux/sq_demux.py
--rw-rw-r--   0 ajith     (1000) ajith     (1000)     1982 2024-04-01 22:28:07.000000 pysysq-0.1.1/src/pysysq/sq_base/sq_mux_demux/sq_mux.py
--rw-rw-r--   0 ajith     (1000) ajith     (1000)     7027 2024-04-06 10:07:17.000000 pysysq-0.1.1/src/pysysq/sq_base/sq_object.py
-drwxrwxr-x   0 ajith     (1000) ajith     (1000)        0 2024-04-06 21:04:35.807643 pysysq-0.1.1/src/pysysq/sq_base/sq_packet/
--rw-rw-r--   0 ajith     (1000) ajith     (1000)      109 2024-03-31 20:14:07.000000 pysysq-0.1.1/src/pysysq/sq_base/sq_packet/__init__.py
--rw-rw-r--   0 ajith     (1000) ajith     (1000)      132 2024-03-31 20:14:07.000000 pysysq-0.1.1/src/pysysq/sq_base/sq_packet/sq_metadata.py
--rw-rw-r--   0 ajith     (1000) ajith     (1000)      328 2024-03-31 20:14:07.000000 pysysq-0.1.1/src/pysysq/sq_base/sq_packet/sq_packet.py
--rw-rw-r--   0 ajith     (1000) ajith     (1000)      157 2024-03-31 20:14:07.000000 pysysq-0.1.1/src/pysysq/sq_base/sq_packet/sq_packet_info.py
-drwxrwxr-x   0 ajith     (1000) ajith     (1000)        0 2024-04-06 21:04:35.807643 pysysq-0.1.1/src/pysysq/sq_base/sq_pkt_gen/
--rw-rw-r--   0 ajith     (1000) ajith     (1000)       44 2024-04-06 10:07:36.000000 pysysq-0.1.1/src/pysysq/sq_base/sq_pkt_gen/__init__.py
--rw-rw-r--   0 ajith     (1000) ajith     (1000)     1728 2024-04-01 22:28:07.000000 pysysq-0.1.1/src/pysysq/sq_base/sq_pkt_gen/sq_pkt_gen.py
-drwxrwxr-x   0 ajith     (1000) ajith     (1000)        0 2024-04-06 21:04:35.807643 pysysq-0.1.1/src/pysysq/sq_base/sq_pkt_gen/states/
--rw-rw-r--   0 ajith     (1000) ajith     (1000)      250 2024-04-01 14:46:29.000000 pysysq-0.1.1/src/pysysq/sq_base/sq_pkt_gen/states/__init__.py
--rw-rw-r--   0 ajith     (1000) ajith     (1000)      410 2024-04-06 20:36:42.000000 pysysq-0.1.1/src/pysysq/sq_base/sq_pkt_gen/states/sq_generator_state.py
--rw-rw-r--   0 ajith     (1000) ajith     (1000)      616 2024-04-01 14:46:29.000000 pysysq-0.1.1/src/pysysq/sq_base/sq_pkt_gen/states/sq_generator_state_factory.py
--rw-rw-r--   0 ajith     (1000) ajith     (1000)      584 2024-04-01 14:46:29.000000 pysysq-0.1.1/src/pysysq/sq_base/sq_pkt_gen/states/sq_pkt_generator_gen_state.py
--rw-rw-r--   0 ajith     (1000) ajith     (1000)      830 2024-04-06 20:17:41.000000 pysysq-0.1.1/src/pysysq/sq_base/sq_pkt_gen/states/sq_pkt_generator_queuing_state.py
-drwxrwxr-x   0 ajith     (1000) ajith     (1000)        0 2024-04-06 21:04:35.807643 pysysq-0.1.1/src/pysysq/sq_base/sq_pkt_processor/
--rw-rw-r--   0 ajith     (1000) ajith     (1000)       48 2024-04-06 10:07:43.000000 pysysq-0.1.1/src/pysysq/sq_base/sq_pkt_processor/__init__.py
--rw-rw-r--   0 ajith     (1000) ajith     (1000)     3279 2024-04-06 20:39:45.000000 pysysq-0.1.1/src/pysysq/sq_base/sq_pkt_processor/sq_pkt_processor.py
-drwxrwxr-x   0 ajith     (1000) ajith     (1000)        0 2024-04-06 21:04:35.807643 pysysq-0.1.1/src/pysysq/sq_base/sq_pkt_processor/states/
--rw-rw-r--   0 ajith     (1000) ajith     (1000)       96 2024-04-06 20:39:45.000000 pysysq-0.1.1/src/pysysq/sq_base/sq_pkt_processor/states/__init__.py
--rw-rw-r--   0 ajith     (1000) ajith     (1000)     1101 2024-04-01 14:56:54.000000 pysysq-0.1.1/src/pysysq/sq_base/sq_pkt_processor/states/sq_pkt_proc_complete.py
--rw-rw-r--   0 ajith     (1000) ajith     (1000)     1326 2024-04-01 14:56:54.000000 pysysq-0.1.1/src/pysysq/sq_base/sq_pkt_processor/states/sq_pkt_proc_idle.py
--rw-rw-r--   0 ajith     (1000) ajith     (1000)      787 2024-04-01 14:56:54.000000 pysysq-0.1.1/src/pysysq/sq_base/sq_pkt_processor/states/sq_pkt_proc_processing.py
--rw-rw-r--   0 ajith     (1000) ajith     (1000)      470 2024-04-01 14:56:54.000000 pysysq-0.1.1/src/pysysq/sq_base/sq_pkt_processor/states/sq_pkt_processor_state.py
--rw-rw-r--   0 ajith     (1000) ajith     (1000)      729 2024-03-31 20:14:07.000000 pysysq-0.1.1/src/pysysq/sq_base/sq_pkt_processor/states/sq_state_factory.py
-drwxrwxr-x   0 ajith     (1000) ajith     (1000)        0 2024-04-06 21:04:35.807643 pysysq-0.1.1/src/pysysq/sq_base/sq_pkt_sink/
--rw-rw-r--   0 ajith     (1000) ajith     (1000)       34 2024-03-31 20:14:07.000000 pysysq-0.1.1/src/pysysq/sq_base/sq_pkt_sink/__init__.py
--rw-rw-r--   0 ajith     (1000) ajith     (1000)     1216 2024-04-01 20:12:38.000000 pysysq-0.1.1/src/pysysq/sq_base/sq_pkt_sink/sq_pkt_sink.py
-drwxrwxr-x   0 ajith     (1000) ajith     (1000)        0 2024-04-06 21:04:35.807643 pysysq-0.1.1/src/pysysq/sq_base/sq_plugin/
--rw-rw-r--   0 ajith     (1000) ajith     (1000)       77 2024-04-01 22:28:07.000000 pysysq-0.1.1/src/pysysq/sq_base/sq_plugin/__init__.py
-drwxrwxr-x   0 ajith     (1000) ajith     (1000)        0 2024-04-06 21:04:35.807643 pysysq-0.1.1/src/pysysq/sq_base/sq_plugin/default/
--rw-rw-r--   0 ajith     (1000) ajith     (1000)       87 2024-04-06 20:59:49.000000 pysysq-0.1.1/src/pysysq/sq_base/sq_plugin/default/__init__.py
--rw-rw-r--   0 ajith     (1000) ajith     (1000)     3060 2024-04-06 21:04:30.000000 pysysq-0.1.1/src/pysysq/sq_base/sq_plugin/default/sq_default_plugin.py
--rw-rw-r--   0 ajith     (1000) ajith     (1000)      980 2024-04-06 10:06:10.000000 pysysq-0.1.1/src/pysysq/sq_base/sq_plugin/sq_helper.py
--rw-rw-r--   0 ajith     (1000) ajith     (1000)      112 2024-04-06 10:04:40.000000 pysysq-0.1.1/src/pysysq/sq_base/sq_plugin/sq_plugin.py
--rw-rw-r--   0 ajith     (1000) ajith     (1000)      632 2024-04-06 20:59:49.000000 pysysq-0.1.1/src/pysysq/sq_base/sq_plugin/sq_plugin_loader.py
-drwxrwxr-x   0 ajith     (1000) ajith     (1000)        0 2024-04-06 21:04:35.807643 pysysq-0.1.1/src/pysysq/sq_base/sq_queue/
--rw-rw-r--   0 ajith     (1000) ajith     (1000)       73 2024-03-31 20:14:07.000000 pysysq-0.1.1/src/pysysq/sq_base/sq_queue/__init__.py
--rw-rw-r--   0 ajith     (1000) ajith     (1000)      418 2024-03-31 20:14:07.000000 pysysq-0.1.1/src/pysysq/sq_base/sq_queue/sq_queue.py
--rw-rw-r--   0 ajith     (1000) ajith     (1000)     1826 2024-04-01 20:12:38.000000 pysysq-0.1.1/src/pysysq/sq_base/sq_queue/sq_single_queue.py
-drwxrwxr-x   0 ajith     (1000) ajith     (1000)        0 2024-04-06 21:04:35.811643 pysysq-0.1.1/src/pysysq/sq_base/sq_sim_setup_generator/
--rw-rw-r--   0 ajith     (1000) ajith     (1000)       43 2024-03-31 20:14:07.000000 pysysq-0.1.1/src/pysysq/sq_base/sq_sim_setup_generator/__init__.py
-drwxrwxr-x   0 ajith     (1000) ajith     (1000)        0 2024-04-06 21:04:35.811643 pysysq-0.1.1/src/pysysq/sq_base/sq_sim_setup_generator/config/
--rw-rw-r--   0 ajith     (1000) ajith     (1000)     2856 2024-04-06 20:08:42.000000 pysysq-0.1.1/src/pysysq/sq_base/sq_sim_setup_generator/config/input.json
--rw-rw-r--   0 ajith     (1000) ajith     (1000)     1961 2024-04-06 20:14:46.000000 pysysq-0.1.1/src/pysysq/sq_base/sq_sim_setup_generator/sq_code_gen_model.py
--rw-rw-r--   0 ajith     (1000) ajith     (1000)     1461 2024-04-06 10:02:05.000000 pysysq-0.1.1/src/pysysq/sq_base/sq_sim_setup_generator/sq_sim_data_gen_ctx.py
--rw-rw-r--   0 ajith     (1000) ajith     (1000)     7114 2024-04-06 20:08:42.000000 pysysq-0.1.1/src/pysysq/sq_base/sq_sim_setup_generator/sq_sim_data_gen_strategy.py
--rw-rw-r--   0 ajith     (1000) ajith     (1000)      312 2024-04-06 10:02:05.000000 pysysq-0.1.1/src/pysysq/sq_base/sq_sim_setup_generator/sq_sim_data_model.py
--rw-rw-r--   0 ajith     (1000) ajith     (1000)     1669 2024-04-06 10:02:05.000000 pysysq-0.1.1/src/pysysq/sq_base/sq_sim_setup_generator/sq_sim_setup_gen.py
-drwxrwxr-x   0 ajith     (1000) ajith     (1000)        0 2024-04-06 21:04:35.811643 pysysq-0.1.1/src/pysysq/sq_base/sq_sim_setup_generator/templates/
--rw-rw-r--   0 ajith     (1000) ajith     (1000)     1901 2024-04-06 13:11:59.000000 pysysq-0.1.1/src/pysysq/sq_base/sq_sim_setup_generator/templates/sim_setup.py.j2
-drwxrwxr-x   0 ajith     (1000) ajith     (1000)        0 2024-04-06 21:04:35.811643 pysysq-0.1.1/src/pysysq/sq_base/sq_simulator/
--rw-rw-r--   0 ajith     (1000) ajith     (1000)       37 2024-03-31 20:14:07.000000 pysysq-0.1.1/src/pysysq/sq_base/sq_simulator/__init__.py
--rw-rw-r--   0 ajith     (1000) ajith     (1000)     1330 2024-04-01 20:12:38.000000 pysysq-0.1.1/src/pysysq/sq_base/sq_simulator/sq_simulator.py
-drwxrwxr-x   0 ajith     (1000) ajith     (1000)        0 2024-04-06 21:04:35.811643 pysysq-0.1.1/src/pysysq/sq_base/sq_splitter/
--rw-rw-r--   0 ajith     (1000) ajith     (1000)       36 2024-03-31 20:14:07.000000 pysysq-0.1.1/src/pysysq/sq_base/sq_splitter/__init__.py
--rw-rw-r--   0 ajith     (1000) ajith     (1000)     1517 2024-04-01 20:12:38.000000 pysysq-0.1.1/src/pysysq/sq_base/sq_splitter/sq_splitter.py
-drwxrwxr-x   0 ajith     (1000) ajith     (1000)        0 2024-04-06 21:04:35.811643 pysysq-0.1.1/src/pysysq/sq_base/sq_statistics/
--rw-rw-r--   0 ajith     (1000) ajith     (1000)       74 2024-03-31 20:14:07.000000 pysysq-0.1.1/src/pysysq/sq_base/sq_statistics/__init__.py
--rw-rw-r--   0 ajith     (1000) ajith     (1000)     2371 2024-03-31 20:14:07.000000 pysysq-0.1.1/src/pysysq/sq_base/sq_statistics/sq_plotter.py
--rw-rw-r--   0 ajith     (1000) ajith     (1000)     1172 2024-03-31 20:14:07.000000 pysysq-0.1.1/src/pysysq/sq_base/sq_statistics/sq_statistics.py
--rw-rw-r--   0 ajith     (1000) ajith     (1000)      431 2024-03-31 20:14:07.000000 pysysq-0.1.1/src/pysysq/sq_base/sq_time_base.py
-drwxrwxr-x   0 ajith     (1000) ajith     (1000)        0 2024-04-06 21:04:35.811643 pysysq-0.1.1/src/pysysq.egg-info/
--rw-r--r--   0 ajith     (1000) ajith     (1000)    11852 2024-04-06 21:04:35.000000 pysysq-0.1.1/src/pysysq.egg-info/PKG-INFO
--rw-rw-r--   0 ajith     (1000) ajith     (1000)     3770 2024-04-06 21:04:35.000000 pysysq-0.1.1/src/pysysq.egg-info/SOURCES.txt
--rw-rw-r--   0 ajith     (1000) ajith     (1000)        1 2024-04-06 21:04:35.000000 pysysq-0.1.1/src/pysysq.egg-info/dependency_links.txt
--rw-rw-r--   0 ajith     (1000) ajith     (1000)      384 2024-04-06 21:04:35.000000 pysysq-0.1.1/src/pysysq.egg-info/requires.txt
--rw-rw-r--   0 ajith     (1000) ajith     (1000)        7 2024-04-06 21:04:35.000000 pysysq-0.1.1/src/pysysq.egg-info/top_level.txt
-drwxrwxr-x   0 ajith     (1000) ajith     (1000)        0 2024-04-06 21:04:35.803643 pysysq-0.1.1/tests/
-drwxrwxr-x   0 ajith     (1000) ajith     (1000)        0 2024-04-06 21:04:35.811643 pysysq-0.1.1/tests/unittests/
--rw-rw-r--   0 ajith     (1000) ajith     (1000)        0 2024-03-31 20:14:07.000000 pysysq-0.1.1/tests/unittests/__init__.py
--rw-rw-r--   0 ajith     (1000) ajith     (1000)     2392 2024-03-31 20:14:07.000000 pysysq-0.1.1/tests/unittests/test_sq_demux.py
--rw-rw-r--   0 ajith     (1000) ajith     (1000)     2366 2024-03-31 20:14:07.000000 pysysq-0.1.1/tests/unittests/test_sq_mux.py
--rw-rw-r--   0 ajith     (1000) ajith     (1000)     3201 2024-03-31 20:14:07.000000 pysysq-0.1.1/tests/unittests/test_sq_object.py
--rw-rw-r--   0 ajith     (1000) ajith     (1000)     2768 2024-03-31 20:14:07.000000 pysysq-0.1.1/tests/unittests/test_sq_pkt_processor.py
+drwxrwxr-x   0 ajith     (1000) ajith     (1000)        0 2024-04-15 19:59:44.614289 pysysq-0.1.2/
+-rw-rw-r--   0 ajith     (1000) ajith     (1000)     3113 2024-03-31 20:14:07.000000 pysysq-0.1.2/.gitignore
+-rw-rw-r--   0 ajith     (1000) ajith     (1000)     1073 2024-03-31 20:14:07.000000 pysysq-0.1.2/LICENSE
+-rw-r--r--   0 ajith     (1000) ajith     (1000)    11852 2024-04-15 19:59:44.614289 pysysq-0.1.2/PKG-INFO
+-rw-rw-r--   0 ajith     (1000) ajith     (1000)   607908 2024-03-31 20:14:07.000000 pysysq-0.1.2/PysysQ.ipynb
+-rw-rw-r--   0 ajith     (1000) ajith     (1000)     9238 2024-04-06 20:27:59.000000 pysysq-0.1.2/README.md
+-rw-rw-r--   0 ajith     (1000) ajith     (1000)        0 2024-04-01 14:12:34.000000 pysysq-0.1.2/__init__.py
+-rw-rw-r--   0 ajith     (1000) ajith     (1000)     1403 2024-04-15 19:59:29.000000 pysysq-0.1.2/pyproject.toml
+-rw-rw-r--   0 ajith     (1000) ajith     (1000)      384 2024-03-31 20:14:07.000000 pysysq-0.1.2/requirements.txt
+-rw-rw-r--   0 ajith     (1000) ajith     (1000)       38 2024-04-15 19:59:44.614289 pysysq-0.1.2/setup.cfg
+drwxrwxr-x   0 ajith     (1000) ajith     (1000)        0 2024-04-15 19:59:44.586289 pysysq-0.1.2/src/
+drwxrwxr-x   0 ajith     (1000) ajith     (1000)        0 2024-04-15 19:59:44.594289 pysysq-0.1.2/src/pysysq/
+-rw-rw-r--   0 ajith     (1000) ajith     (1000)      188 2024-03-31 20:14:07.000000 pysysq-0.1.2/src/pysysq/__init__.py
+-rw-rw-r--   0 ajith     (1000) ajith     (1000)      493 2024-03-31 20:20:58.000000 pysysq-0.1.2/src/pysysq/__main__.py
+-rw-rw-r--   0 ajith     (1000) ajith     (1000)      467 2024-04-15 19:59:44.000000 pysysq-0.1.2/src/pysysq/_version.py
+-rw-rw-r--   0 ajith     (1000) ajith     (1000)     2138 2024-03-31 20:14:07.000000 pysysq-0.1.2/src/pysysq/logging.conf
+drwxrwxr-x   0 ajith     (1000) ajith     (1000)        0 2024-04-15 19:59:44.594289 pysysq-0.1.2/src/pysysq/sq_base/
+-rw-rw-r--   0 ajith     (1000) ajith     (1000)      475 2024-03-31 20:14:07.000000 pysysq-0.1.2/src/pysysq/sq_base/__init__.py
+drwxrwxr-x   0 ajith     (1000) ajith     (1000)        0 2024-04-15 19:59:44.594289 pysysq-0.1.2/src/pysysq/sq_base/sq_clock/
+-rw-rw-r--   0 ajith     (1000) ajith     (1000)       30 2024-03-31 20:14:07.000000 pysysq-0.1.2/src/pysysq/sq_base/sq_clock/__init__.py
+-rw-rw-r--   0 ajith     (1000) ajith     (1000)     1117 2024-04-06 09:26:43.000000 pysysq-0.1.2/src/pysysq/sq_base/sq_clock/sq_clock.py
+drwxrwxr-x   0 ajith     (1000) ajith     (1000)        0 2024-04-15 19:59:44.598289 pysysq-0.1.2/src/pysysq/sq_base/sq_event/
+-rw-rw-r--   0 ajith     (1000) ajith     (1000)      127 2024-03-31 20:14:07.000000 pysysq-0.1.2/src/pysysq/sq_base/sq_event/__init__.py
+-rw-rw-r--   0 ajith     (1000) ajith     (1000)      843 2024-03-31 20:14:07.000000 pysysq-0.1.2/src/pysysq/sq_base/sq_event/sq_event.py
+-rw-rw-r--   0 ajith     (1000) ajith     (1000)     1965 2024-03-31 20:14:07.000000 pysysq-0.1.2/src/pysysq/sq_base/sq_event/sq_event_manager.py
+-rw-rw-r--   0 ajith     (1000) ajith     (1000)     1183 2024-03-31 20:14:07.000000 pysysq-0.1.2/src/pysysq/sq_base/sq_event/sq_event_queue.py
+drwxrwxr-x   0 ajith     (1000) ajith     (1000)        0 2024-04-15 19:59:44.598289 pysysq-0.1.2/src/pysysq/sq_base/sq_factory/
+-rw-rw-r--   0 ajith     (1000) ajith     (1000)       81 2024-04-06 10:06:37.000000 pysysq-0.1.2/src/pysysq/sq_base/sq_factory/__init__.py
+-rw-rw-r--   0 ajith     (1000) ajith     (1000)     1973 2024-04-06 13:21:28.000000 pysysq-0.1.2/src/pysysq/sq_base/sq_factory/sq_factory.py
+-rw-rw-r--   0 ajith     (1000) ajith     (1000)      443 2024-04-06 20:59:49.000000 pysysq-0.1.2/src/pysysq/sq_base/sq_factory/sq_helper_factory.py
+drwxrwxr-x   0 ajith     (1000) ajith     (1000)        0 2024-04-15 19:59:44.598289 pysysq-0.1.2/src/pysysq/sq_base/sq_filter/
+-rw-rw-r--   0 ajith     (1000) ajith     (1000)       34 2024-04-01 14:12:25.000000 pysysq-0.1.2/src/pysysq/sq_base/sq_filter/__init__.py
+-rw-rw-r--   0 ajith     (1000) ajith     (1000)     1446 2024-04-01 22:28:07.000000 pysysq-0.1.2/src/pysysq/sq_base/sq_filter/sq_filter.py
+drwxrwxr-x   0 ajith     (1000) ajith     (1000)        0 2024-04-15 19:59:44.598289 pysysq-0.1.2/src/pysysq/sq_base/sq_logger/
+-rw-rw-r--   0 ajith     (1000) ajith     (1000)       32 2024-03-31 20:14:07.000000 pysysq-0.1.2/src/pysysq/sq_base/sq_logger/__init__.py
+-rw-rw-r--   0 ajith     (1000) ajith     (1000)      892 2024-03-31 20:14:07.000000 pysysq-0.1.2/src/pysysq/sq_base/sq_logger/sq_logger.py
+drwxrwxr-x   0 ajith     (1000) ajith     (1000)        0 2024-04-15 19:59:44.598289 pysysq-0.1.2/src/pysysq/sq_base/sq_merger/
+-rw-rw-r--   0 ajith     (1000) ajith     (1000)       31 2024-03-31 20:14:07.000000 pysysq-0.1.2/src/pysysq/sq_base/sq_merger/__init__.py
+-rw-rw-r--   0 ajith     (1000) ajith     (1000)     1585 2024-04-01 14:12:25.000000 pysysq-0.1.2/src/pysysq/sq_base/sq_merger/sq_merger.py
+drwxrwxr-x   0 ajith     (1000) ajith     (1000)        0 2024-04-15 19:59:44.598289 pysysq-0.1.2/src/pysysq/sq_base/sq_mux_demux/
+-rw-rw-r--   0 ajith     (1000) ajith     (1000)       59 2024-04-06 10:07:28.000000 pysysq-0.1.2/src/pysysq/sq_base/sq_mux_demux/__init__.py
+-rw-rw-r--   0 ajith     (1000) ajith     (1000)     2168 2024-04-01 22:28:07.000000 pysysq-0.1.2/src/pysysq/sq_base/sq_mux_demux/sq_demux.py
+-rw-rw-r--   0 ajith     (1000) ajith     (1000)     1982 2024-04-01 22:28:07.000000 pysysq-0.1.2/src/pysysq/sq_base/sq_mux_demux/sq_mux.py
+-rw-rw-r--   0 ajith     (1000) ajith     (1000)     7027 2024-04-06 10:07:17.000000 pysysq-0.1.2/src/pysysq/sq_base/sq_object.py
+drwxrwxr-x   0 ajith     (1000) ajith     (1000)        0 2024-04-15 19:59:44.602289 pysysq-0.1.2/src/pysysq/sq_base/sq_packet/
+-rw-rw-r--   0 ajith     (1000) ajith     (1000)       68 2024-04-15 18:02:36.000000 pysysq-0.1.2/src/pysysq/sq_base/sq_packet/__init__.py
+-rw-rw-r--   0 ajith     (1000) ajith     (1000)      132 2024-03-31 20:14:07.000000 pysysq-0.1.2/src/pysysq/sq_base/sq_packet/sq_metadata.py
+-rw-rw-r--   0 ajith     (1000) ajith     (1000)      104 2024-04-15 19:03:53.000000 pysysq-0.1.2/src/pysysq/sq_base/sq_packet/sq_packet.py
+drwxrwxr-x   0 ajith     (1000) ajith     (1000)        0 2024-04-15 19:59:44.602289 pysysq-0.1.2/src/pysysq/sq_base/sq_pkt_gen/
+-rw-rw-r--   0 ajith     (1000) ajith     (1000)       44 2024-04-06 10:07:36.000000 pysysq-0.1.2/src/pysysq/sq_base/sq_pkt_gen/__init__.py
+-rw-rw-r--   0 ajith     (1000) ajith     (1000)     1728 2024-04-01 22:28:07.000000 pysysq-0.1.2/src/pysysq/sq_base/sq_pkt_gen/sq_pkt_gen.py
+drwxrwxr-x   0 ajith     (1000) ajith     (1000)        0 2024-04-15 19:59:44.602289 pysysq-0.1.2/src/pysysq/sq_base/sq_pkt_gen/states/
+-rw-rw-r--   0 ajith     (1000) ajith     (1000)      250 2024-04-01 14:46:29.000000 pysysq-0.1.2/src/pysysq/sq_base/sq_pkt_gen/states/__init__.py
+-rw-rw-r--   0 ajith     (1000) ajith     (1000)      410 2024-04-06 20:36:42.000000 pysysq-0.1.2/src/pysysq/sq_base/sq_pkt_gen/states/sq_generator_state.py
+-rw-rw-r--   0 ajith     (1000) ajith     (1000)      616 2024-04-01 14:46:29.000000 pysysq-0.1.2/src/pysysq/sq_base/sq_pkt_gen/states/sq_generator_state_factory.py
+-rw-rw-r--   0 ajith     (1000) ajith     (1000)      584 2024-04-01 14:46:29.000000 pysysq-0.1.2/src/pysysq/sq_base/sq_pkt_gen/states/sq_pkt_generator_gen_state.py
+-rw-rw-r--   0 ajith     (1000) ajith     (1000)      830 2024-04-06 20:17:41.000000 pysysq-0.1.2/src/pysysq/sq_base/sq_pkt_gen/states/sq_pkt_generator_queuing_state.py
+drwxrwxr-x   0 ajith     (1000) ajith     (1000)        0 2024-04-15 19:59:44.602289 pysysq-0.1.2/src/pysysq/sq_base/sq_pkt_processor/
+-rw-rw-r--   0 ajith     (1000) ajith     (1000)       48 2024-04-06 10:07:43.000000 pysysq-0.1.2/src/pysysq/sq_base/sq_pkt_processor/__init__.py
+-rw-rw-r--   0 ajith     (1000) ajith     (1000)     3279 2024-04-06 20:39:45.000000 pysysq-0.1.2/src/pysysq/sq_base/sq_pkt_processor/sq_pkt_processor.py
+drwxrwxr-x   0 ajith     (1000) ajith     (1000)        0 2024-04-15 19:59:44.606289 pysysq-0.1.2/src/pysysq/sq_base/sq_pkt_processor/states/
+-rw-rw-r--   0 ajith     (1000) ajith     (1000)       96 2024-04-06 20:39:45.000000 pysysq-0.1.2/src/pysysq/sq_base/sq_pkt_processor/states/__init__.py
+-rw-rw-r--   0 ajith     (1000) ajith     (1000)     1101 2024-04-01 14:56:54.000000 pysysq-0.1.2/src/pysysq/sq_base/sq_pkt_processor/states/sq_pkt_proc_complete.py
+-rw-rw-r--   0 ajith     (1000) ajith     (1000)     1326 2024-04-01 14:56:54.000000 pysysq-0.1.2/src/pysysq/sq_base/sq_pkt_processor/states/sq_pkt_proc_idle.py
+-rw-rw-r--   0 ajith     (1000) ajith     (1000)      787 2024-04-01 14:56:54.000000 pysysq-0.1.2/src/pysysq/sq_base/sq_pkt_processor/states/sq_pkt_proc_processing.py
+-rw-rw-r--   0 ajith     (1000) ajith     (1000)      470 2024-04-01 14:56:54.000000 pysysq-0.1.2/src/pysysq/sq_base/sq_pkt_processor/states/sq_pkt_processor_state.py
+-rw-rw-r--   0 ajith     (1000) ajith     (1000)      729 2024-03-31 20:14:07.000000 pysysq-0.1.2/src/pysysq/sq_base/sq_pkt_processor/states/sq_state_factory.py
+drwxrwxr-x   0 ajith     (1000) ajith     (1000)        0 2024-04-15 19:59:44.606289 pysysq-0.1.2/src/pysysq/sq_base/sq_pkt_sink/
+-rw-rw-r--   0 ajith     (1000) ajith     (1000)       34 2024-03-31 20:14:07.000000 pysysq-0.1.2/src/pysysq/sq_base/sq_pkt_sink/__init__.py
+-rw-rw-r--   0 ajith     (1000) ajith     (1000)     1181 2024-04-15 17:58:00.000000 pysysq-0.1.2/src/pysysq/sq_base/sq_pkt_sink/sq_pkt_sink.py
+drwxrwxr-x   0 ajith     (1000) ajith     (1000)        0 2024-04-15 19:59:44.606289 pysysq-0.1.2/src/pysysq/sq_base/sq_plugin/
+-rw-rw-r--   0 ajith     (1000) ajith     (1000)       77 2024-04-01 22:28:07.000000 pysysq-0.1.2/src/pysysq/sq_base/sq_plugin/__init__.py
+drwxrwxr-x   0 ajith     (1000) ajith     (1000)        0 2024-04-15 19:59:44.606289 pysysq-0.1.2/src/pysysq/sq_base/sq_plugin/default/
+-rw-rw-r--   0 ajith     (1000) ajith     (1000)       87 2024-04-06 20:59:49.000000 pysysq-0.1.2/src/pysysq/sq_base/sq_plugin/default/__init__.py
+-rw-rw-r--   0 ajith     (1000) ajith     (1000)     3139 2024-04-15 19:03:53.000000 pysysq-0.1.2/src/pysysq/sq_base/sq_plugin/default/sq_default_plugin.py
+-rw-rw-r--   0 ajith     (1000) ajith     (1000)      221 2024-04-15 19:03:53.000000 pysysq-0.1.2/src/pysysq/sq_base/sq_plugin/default/sq_generic_packet.py
+-rw-rw-r--   0 ajith     (1000) ajith     (1000)      157 2024-03-31 20:14:07.000000 pysysq-0.1.2/src/pysysq/sq_base/sq_plugin/default/sq_packet_info.py
+-rw-rw-r--   0 ajith     (1000) ajith     (1000)      980 2024-04-06 10:06:10.000000 pysysq-0.1.2/src/pysysq/sq_base/sq_plugin/sq_helper.py
+-rw-rw-r--   0 ajith     (1000) ajith     (1000)      112 2024-04-06 10:04:40.000000 pysysq-0.1.2/src/pysysq/sq_base/sq_plugin/sq_plugin.py
+-rw-rw-r--   0 ajith     (1000) ajith     (1000)      632 2024-04-06 20:59:49.000000 pysysq-0.1.2/src/pysysq/sq_base/sq_plugin/sq_plugin_loader.py
+drwxrwxr-x   0 ajith     (1000) ajith     (1000)        0 2024-04-15 19:59:44.606289 pysysq-0.1.2/src/pysysq/sq_base/sq_queue/
+-rw-rw-r--   0 ajith     (1000) ajith     (1000)       73 2024-03-31 20:14:07.000000 pysysq-0.1.2/src/pysysq/sq_base/sq_queue/__init__.py
+-rw-rw-r--   0 ajith     (1000) ajith     (1000)      383 2024-04-15 17:58:00.000000 pysysq-0.1.2/src/pysysq/sq_base/sq_queue/sq_queue.py
+-rw-rw-r--   0 ajith     (1000) ajith     (1000)     1826 2024-04-01 20:12:38.000000 pysysq-0.1.2/src/pysysq/sq_base/sq_queue/sq_single_queue.py
+drwxrwxr-x   0 ajith     (1000) ajith     (1000)        0 2024-04-15 19:59:44.610289 pysysq-0.1.2/src/pysysq/sq_base/sq_sim_setup_generator/
+-rw-rw-r--   0 ajith     (1000) ajith     (1000)       43 2024-03-31 20:14:07.000000 pysysq-0.1.2/src/pysysq/sq_base/sq_sim_setup_generator/__init__.py
+drwxrwxr-x   0 ajith     (1000) ajith     (1000)        0 2024-04-15 19:59:44.610289 pysysq-0.1.2/src/pysysq/sq_base/sq_sim_setup_generator/config/
+-rw-rw-r--   0 ajith     (1000) ajith     (1000)     2856 2024-04-06 20:08:42.000000 pysysq-0.1.2/src/pysysq/sq_base/sq_sim_setup_generator/config/input.json
+-rw-rw-r--   0 ajith     (1000) ajith     (1000)     1961 2024-04-06 20:14:46.000000 pysysq-0.1.2/src/pysysq/sq_base/sq_sim_setup_generator/sq_code_gen_model.py
+-rw-rw-r--   0 ajith     (1000) ajith     (1000)     1461 2024-04-06 10:02:05.000000 pysysq-0.1.2/src/pysysq/sq_base/sq_sim_setup_generator/sq_sim_data_gen_ctx.py
+-rw-rw-r--   0 ajith     (1000) ajith     (1000)     7114 2024-04-06 20:08:42.000000 pysysq-0.1.2/src/pysysq/sq_base/sq_sim_setup_generator/sq_sim_data_gen_strategy.py
+-rw-rw-r--   0 ajith     (1000) ajith     (1000)      312 2024-04-06 10:02:05.000000 pysysq-0.1.2/src/pysysq/sq_base/sq_sim_setup_generator/sq_sim_data_model.py
+-rw-rw-r--   0 ajith     (1000) ajith     (1000)     1669 2024-04-06 10:02:05.000000 pysysq-0.1.2/src/pysysq/sq_base/sq_sim_setup_generator/sq_sim_setup_gen.py
+drwxrwxr-x   0 ajith     (1000) ajith     (1000)        0 2024-04-15 19:59:44.610289 pysysq-0.1.2/src/pysysq/sq_base/sq_sim_setup_generator/templates/
+-rw-rw-r--   0 ajith     (1000) ajith     (1000)     1901 2024-04-06 13:11:59.000000 pysysq-0.1.2/src/pysysq/sq_base/sq_sim_setup_generator/templates/sim_setup.py.j2
+drwxrwxr-x   0 ajith     (1000) ajith     (1000)        0 2024-04-15 19:59:44.610289 pysysq-0.1.2/src/pysysq/sq_base/sq_simulator/
+-rw-rw-r--   0 ajith     (1000) ajith     (1000)       37 2024-03-31 20:14:07.000000 pysysq-0.1.2/src/pysysq/sq_base/sq_simulator/__init__.py
+-rw-rw-r--   0 ajith     (1000) ajith     (1000)     1330 2024-04-01 20:12:38.000000 pysysq-0.1.2/src/pysysq/sq_base/sq_simulator/sq_simulator.py
+drwxrwxr-x   0 ajith     (1000) ajith     (1000)        0 2024-04-15 19:59:44.610289 pysysq-0.1.2/src/pysysq/sq_base/sq_splitter/
+-rw-rw-r--   0 ajith     (1000) ajith     (1000)       36 2024-03-31 20:14:07.000000 pysysq-0.1.2/src/pysysq/sq_base/sq_splitter/__init__.py
+-rw-rw-r--   0 ajith     (1000) ajith     (1000)     1517 2024-04-01 20:12:38.000000 pysysq-0.1.2/src/pysysq/sq_base/sq_splitter/sq_splitter.py
+drwxrwxr-x   0 ajith     (1000) ajith     (1000)        0 2024-04-15 19:59:44.610289 pysysq-0.1.2/src/pysysq/sq_base/sq_statistics/
+-rw-rw-r--   0 ajith     (1000) ajith     (1000)       74 2024-03-31 20:14:07.000000 pysysq-0.1.2/src/pysysq/sq_base/sq_statistics/__init__.py
+-rw-rw-r--   0 ajith     (1000) ajith     (1000)     2371 2024-03-31 20:14:07.000000 pysysq-0.1.2/src/pysysq/sq_base/sq_statistics/sq_plotter.py
+-rw-rw-r--   0 ajith     (1000) ajith     (1000)     1172 2024-03-31 20:14:07.000000 pysysq-0.1.2/src/pysysq/sq_base/sq_statistics/sq_statistics.py
+-rw-rw-r--   0 ajith     (1000) ajith     (1000)      431 2024-03-31 20:14:07.000000 pysysq-0.1.2/src/pysysq/sq_base/sq_time_base.py
+drwxrwxr-x   0 ajith     (1000) ajith     (1000)        0 2024-04-15 19:59:44.614289 pysysq-0.1.2/src/pysysq.egg-info/
+-rw-r--r--   0 ajith     (1000) ajith     (1000)    11852 2024-04-15 19:59:44.000000 pysysq-0.1.2/src/pysysq.egg-info/PKG-INFO
+-rw-rw-r--   0 ajith     (1000) ajith     (1000)     3761 2024-04-15 19:59:44.000000 pysysq-0.1.2/src/pysysq.egg-info/SOURCES.txt
+-rw-rw-r--   0 ajith     (1000) ajith     (1000)        1 2024-04-15 19:59:44.000000 pysysq-0.1.2/src/pysysq.egg-info/dependency_links.txt
+-rw-rw-r--   0 ajith     (1000) ajith     (1000)      384 2024-04-15 19:59:44.000000 pysysq-0.1.2/src/pysysq.egg-info/requires.txt
+-rw-rw-r--   0 ajith     (1000) ajith     (1000)        7 2024-04-15 19:59:44.000000 pysysq-0.1.2/src/pysysq.egg-info/top_level.txt
+drwxrwxr-x   0 ajith     (1000) ajith     (1000)        0 2024-04-15 19:59:44.586289 pysysq-0.1.2/tests/
+drwxrwxr-x   0 ajith     (1000) ajith     (1000)        0 2024-04-15 19:59:44.614289 pysysq-0.1.2/tests/unittests/
+-rw-rw-r--   0 ajith     (1000) ajith     (1000)        0 2024-03-31 20:14:07.000000 pysysq-0.1.2/tests/unittests/__init__.py
+-rw-rw-r--   0 ajith     (1000) ajith     (1000)     2794 2024-04-15 19:40:28.000000 pysysq-0.1.2/tests/unittests/test_sq_demux.py
+-rw-rw-r--   0 ajith     (1000) ajith     (1000)     2705 2024-04-15 19:40:28.000000 pysysq-0.1.2/tests/unittests/test_sq_mux.py
```

### Comparing `pysysq-0.1.1/.gitignore` & `pysysq-0.1.2/.gitignore`

 * *Files identical despite different names*

### Comparing `pysysq-0.1.1/LICENSE` & `pysysq-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `pysysq-0.1.1/PKG-INFO` & `pysysq-0.1.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pysysq
-Version: 0.1.1
+Version: 0.1.2
 Summary: A system functional flow simulation framework using Queuing Theory
 Author-email: Ajith Padman <ajith.padman@gmail.com>
 License: MIT License
         
         Copyright (c) [2024] [Ajith Padman]
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `pysysq-0.1.1/PysysQ.ipynb` & `pysysq-0.1.2/PysysQ.ipynb`

 * *Files identical despite different names*

### Comparing `pysysq-0.1.1/README.md` & `pysysq-0.1.2/README.md`

 * *Files identical despite different names*

### Comparing `pysysq-0.1.1/pyproject.toml` & `pysysq-0.1.2/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [build-system]
 requires = ["setuptools", "setuptools-scm"]
 build-backend = "setuptools.build_meta"
 
 
 [project]
 name = "pysysq"
-version = "0.1.1"
+version = "0.1.2"
 authors =[
     {name = "Ajith Padman", email = "ajith.padman@gmail.com"}
 ]
 description= "A system functional flow simulation framework using Queuing Theory"
 readme = "README.md"
 license = {file = "LICENSE"}
 dependencies = [
```

### Comparing `pysysq-0.1.1/src/pysysq/logging.conf` & `pysysq-0.1.2/src/pysysq/logging.conf`

 * *Files identical despite different names*

### Comparing `pysysq-0.1.1/src/pysysq/sq_base/sq_clock/sq_clock.py` & `pysysq-0.1.2/src/pysysq/sq_base/sq_clock/sq_clock.py`

 * *Files identical despite different names*

### Comparing `pysysq-0.1.1/src/pysysq/sq_base/sq_event/sq_event.py` & `pysysq-0.1.2/src/pysysq/sq_base/sq_event/sq_event.py`

 * *Files identical despite different names*

### Comparing `pysysq-0.1.1/src/pysysq/sq_base/sq_event/sq_event_manager.py` & `pysysq-0.1.2/src/pysysq/sq_base/sq_event/sq_event_manager.py`

 * *Files identical despite different names*

### Comparing `pysysq-0.1.1/src/pysysq/sq_base/sq_event/sq_event_queue.py` & `pysysq-0.1.2/src/pysysq/sq_base/sq_event/sq_event_queue.py`

 * *Files identical despite different names*

### Comparing `pysysq-0.1.1/src/pysysq/sq_base/sq_factory/sq_factory.py` & `pysysq-0.1.2/src/pysysq/sq_base/sq_factory/sq_factory.py`

 * *Files identical despite different names*

### Comparing `pysysq-0.1.1/src/pysysq/sq_base/sq_filter/sq_filter.py` & `pysysq-0.1.2/src/pysysq/sq_base/sq_filter/sq_filter.py`

 * *Files identical despite different names*

### Comparing `pysysq-0.1.1/src/pysysq/sq_base/sq_logger/sq_logger.py` & `pysysq-0.1.2/src/pysysq/sq_base/sq_logger/sq_logger.py`

 * *Files identical despite different names*

### Comparing `pysysq-0.1.1/src/pysysq/sq_base/sq_merger/sq_merger.py` & `pysysq-0.1.2/src/pysysq/sq_base/sq_merger/sq_merger.py`

 * *Files identical despite different names*

### Comparing `pysysq-0.1.1/src/pysysq/sq_base/sq_mux_demux/sq_demux.py` & `pysysq-0.1.2/src/pysysq/sq_base/sq_mux_demux/sq_demux.py`

 * *Files identical despite different names*

### Comparing `pysysq-0.1.1/src/pysysq/sq_base/sq_mux_demux/sq_mux.py` & `pysysq-0.1.2/src/pysysq/sq_base/sq_mux_demux/sq_mux.py`

 * *Files identical despite different names*

### Comparing `pysysq-0.1.1/src/pysysq/sq_base/sq_object.py` & `pysysq-0.1.2/src/pysysq/sq_base/sq_object.py`

 * *Files identical despite different names*

### Comparing `pysysq-0.1.1/src/pysysq/sq_base/sq_pkt_gen/sq_pkt_gen.py` & `pysysq-0.1.2/src/pysysq/sq_base/sq_pkt_gen/sq_pkt_gen.py`

 * *Files identical despite different names*

### Comparing `pysysq-0.1.1/src/pysysq/sq_base/sq_pkt_gen/states/sq_generator_state_factory.py` & `pysysq-0.1.2/src/pysysq/sq_base/sq_pkt_gen/states/sq_generator_state_factory.py`

 * *Files identical despite different names*

### Comparing `pysysq-0.1.1/src/pysysq/sq_base/sq_pkt_gen/states/sq_pkt_generator_gen_state.py` & `pysysq-0.1.2/src/pysysq/sq_base/sq_pkt_gen/states/sq_pkt_generator_gen_state.py`

 * *Files identical despite different names*

### Comparing `pysysq-0.1.1/src/pysysq/sq_base/sq_pkt_gen/states/sq_pkt_generator_queuing_state.py` & `pysysq-0.1.2/src/pysysq/sq_base/sq_pkt_gen/states/sq_pkt_generator_queuing_state.py`

 * *Files identical despite different names*

### Comparing `pysysq-0.1.1/src/pysysq/sq_base/sq_pkt_processor/sq_pkt_processor.py` & `pysysq-0.1.2/src/pysysq/sq_base/sq_pkt_processor/sq_pkt_processor.py`

 * *Files identical despite different names*

### Comparing `pysysq-0.1.1/src/pysysq/sq_base/sq_pkt_processor/states/sq_pkt_proc_complete.py` & `pysysq-0.1.2/src/pysysq/sq_base/sq_pkt_processor/states/sq_pkt_proc_complete.py`

 * *Files identical despite different names*

### Comparing `pysysq-0.1.1/src/pysysq/sq_base/sq_pkt_processor/states/sq_pkt_proc_idle.py` & `pysysq-0.1.2/src/pysysq/sq_base/sq_pkt_processor/states/sq_pkt_proc_idle.py`

 * *Files identical despite different names*

### Comparing `pysysq-0.1.1/src/pysysq/sq_base/sq_pkt_processor/states/sq_pkt_proc_processing.py` & `pysysq-0.1.2/src/pysysq/sq_base/sq_pkt_processor/states/sq_pkt_proc_processing.py`

 * *Files identical despite different names*

### Comparing `pysysq-0.1.1/src/pysysq/sq_base/sq_pkt_processor/states/sq_state_factory.py` & `pysysq-0.1.2/src/pysysq/sq_base/sq_pkt_processor/states/sq_state_factory.py`

 * *Files identical despite different names*

### Comparing `pysysq-0.1.1/src/pysysq/sq_base/sq_pkt_sink/sq_pkt_sink.py` & `pysysq-0.1.2/src/pysysq/sq_base/sq_pkt_sink/sq_pkt_sink.py`

 * *Files 11% similar despite different names*

```diff
@@ -20,13 +20,13 @@
 
     def process_packet(self, evt: SQEvent):
         super().process_packet(evt)
         if evt.owner is self.clk:
             curr_pkt = self.input_q.pop()
             self.tick += 1
             if curr_pkt is not None:
-                self.logger.info(f' Terminated the Packet {curr_pkt} path of the packet {curr_pkt.path} ')
+                self.logger.info(f' Terminated the Packet {curr_pkt} ')
             else:
                 self.logger.info(f' No Packet to Terminate')
         else:
             if evt.name != f'{self.name}_start':
                 self.logger.error(f'Ignoring Events other than Clock Events {evt}')
```

### Comparing `pysysq-0.1.1/src/pysysq/sq_base/sq_plugin/default/sq_default_plugin.py` & `pysysq-0.1.2/src/pysysq/sq_base/sq_plugin/default/sq_default_plugin.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 from typing import Generator, List, Union
 import numpy as np
 from ...sq_packet import SQPacket, SQMetadata
 from ...sq_queue import SQQueue
 from ...sq_event import SQEvent
 from ..sq_helper import SQHelper
-from ...sq_packet import SQPacketInfo
+from .sq_packet_info import SQPacketInfo
+from .sq_generic_packet import SQGenericPacket
 from ...sq_time_base import SQTimeBase
 
 
 def register(helper_factory):
     helper_factory.register(name="default", factory=SQDefaultHelper)
 
 
@@ -29,19 +30,19 @@
         pkts = []
         no_of_pkts = int(np.abs(np.random.normal(self.no_pkts_mean, self.no_pkts_sd, None)))
         pkt_sizes = [int(x) for x in np.abs(np.random.normal(self.pkt_size_mean, self.pkt_size_sd, no_of_pkts))]
         pkt_classes = np.random.choice(self.classes, no_of_pkts)
         pkt_priorities = np.random.randint(self.priorities[0], self.priorities[1], no_of_pkts)
         pkt_info: SQPacketInfo = SQPacketInfo(no_of_pkts, pkt_sizes, pkt_classes, pkt_priorities)
         for p in range(pkt_info.no_of_pkts):
-            pkt = SQPacket(id=self.pkt_id,
-                           size=pkt_info.pkt_sizes[p],
-                           class_name=pkt_info.pkt_classes[p],
-                           priority=pkt_info.pkt_priorities[p],
-                           generation_time=SQTimeBase.get_current_sim_time())
+            pkt = SQGenericPacket(id=self.pkt_id,
+                                  size=pkt_info.pkt_sizes[p],
+                                  class_name=pkt_info.pkt_classes[p],
+                                  priority=pkt_info.pkt_priorities[p],
+                                  timestamp=SQTimeBase.get_current_sim_time())
             self.pkt_id += 1
             pkts.append(pkt)
         yield pkts
 
     def get_processing_cycles(self, pkt: SQPacket) -> int:
         np.random.seed(pkt.size)
         return np.random.randint(1, 10)
```

### Comparing `pysysq-0.1.1/src/pysysq/sq_base/sq_plugin/sq_helper.py` & `pysysq-0.1.2/src/pysysq/sq_base/sq_plugin/sq_helper.py`

 * *Files identical despite different names*

### Comparing `pysysq-0.1.1/src/pysysq/sq_base/sq_plugin/sq_plugin_loader.py` & `pysysq-0.1.2/src/pysysq/sq_base/sq_plugin/sq_plugin_loader.py`

 * *Files identical despite different names*

### Comparing `pysysq-0.1.1/src/pysysq/sq_base/sq_queue/sq_single_queue.py` & `pysysq-0.1.2/src/pysysq/sq_base/sq_queue/sq_single_queue.py`

 * *Files identical despite different names*

### Comparing `pysysq-0.1.1/src/pysysq/sq_base/sq_sim_setup_generator/config/input.json` & `pysysq-0.1.2/src/pysysq/sq_base/sq_sim_setup_generator/config/input.json`

 * *Files identical despite different names*

### Comparing `pysysq-0.1.1/src/pysysq/sq_base/sq_sim_setup_generator/sq_code_gen_model.py` & `pysysq-0.1.2/src/pysysq/sq_base/sq_sim_setup_generator/sq_code_gen_model.py`

 * *Files identical despite different names*

### Comparing `pysysq-0.1.1/src/pysysq/sq_base/sq_sim_setup_generator/sq_sim_data_gen_ctx.py` & `pysysq-0.1.2/src/pysysq/sq_base/sq_sim_setup_generator/sq_sim_data_gen_ctx.py`

 * *Files identical despite different names*

### Comparing `pysysq-0.1.1/src/pysysq/sq_base/sq_sim_setup_generator/sq_sim_data_gen_strategy.py` & `pysysq-0.1.2/src/pysysq/sq_base/sq_sim_setup_generator/sq_sim_data_gen_strategy.py`

 * *Files identical despite different names*

### Comparing `pysysq-0.1.1/src/pysysq/sq_base/sq_sim_setup_generator/sq_sim_setup_gen.py` & `pysysq-0.1.2/src/pysysq/sq_base/sq_sim_setup_generator/sq_sim_setup_gen.py`

 * *Files identical despite different names*

### Comparing `pysysq-0.1.1/src/pysysq/sq_base/sq_sim_setup_generator/templates/sim_setup.py.j2` & `pysysq-0.1.2/src/pysysq/sq_base/sq_sim_setup_generator/templates/sim_setup.py.j2`

 * *Files identical despite different names*

### Comparing `pysysq-0.1.1/src/pysysq/sq_base/sq_simulator/sq_simulator.py` & `pysysq-0.1.2/src/pysysq/sq_base/sq_simulator/sq_simulator.py`

 * *Files identical despite different names*

### Comparing `pysysq-0.1.1/src/pysysq/sq_base/sq_splitter/sq_splitter.py` & `pysysq-0.1.2/src/pysysq/sq_base/sq_splitter/sq_splitter.py`

 * *Files identical despite different names*

### Comparing `pysysq-0.1.1/src/pysysq/sq_base/sq_statistics/sq_plotter.py` & `pysysq-0.1.2/src/pysysq/sq_base/sq_statistics/sq_plotter.py`

 * *Files identical despite different names*

### Comparing `pysysq-0.1.1/src/pysysq/sq_base/sq_statistics/sq_statistics.py` & `pysysq-0.1.2/src/pysysq/sq_base/sq_statistics/sq_statistics.py`

 * *Files identical despite different names*

### Comparing `pysysq-0.1.1/src/pysysq.egg-info/PKG-INFO` & `pysysq-0.1.2/src/pysysq.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pysysq
-Version: 0.1.1
+Version: 0.1.2
 Summary: A system functional flow simulation framework using Queuing Theory
 Author-email: Ajith Padman <ajith.padman@gmail.com>
 License: MIT License
         
         Copyright (c) [2024] [Ajith Padman]
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `pysysq-0.1.1/src/pysysq.egg-info/SOURCES.txt` & `pysysq-0.1.2/src/pysysq.egg-info/SOURCES.txt`

 * *Files 7% similar despite different names*

```diff
@@ -34,15 +34,14 @@
 src/pysysq/sq_base/sq_merger/sq_merger.py
 src/pysysq/sq_base/sq_mux_demux/__init__.py
 src/pysysq/sq_base/sq_mux_demux/sq_demux.py
 src/pysysq/sq_base/sq_mux_demux/sq_mux.py
 src/pysysq/sq_base/sq_packet/__init__.py
 src/pysysq/sq_base/sq_packet/sq_metadata.py
 src/pysysq/sq_base/sq_packet/sq_packet.py
-src/pysysq/sq_base/sq_packet/sq_packet_info.py
 src/pysysq/sq_base/sq_pkt_gen/__init__.py
 src/pysysq/sq_base/sq_pkt_gen/sq_pkt_gen.py
 src/pysysq/sq_base/sq_pkt_gen/states/__init__.py
 src/pysysq/sq_base/sq_pkt_gen/states/sq_generator_state.py
 src/pysysq/sq_base/sq_pkt_gen/states/sq_generator_state_factory.py
 src/pysysq/sq_base/sq_pkt_gen/states/sq_pkt_generator_gen_state.py
 src/pysysq/sq_base/sq_pkt_gen/states/sq_pkt_generator_queuing_state.py
@@ -58,14 +57,16 @@
 src/pysysq/sq_base/sq_pkt_sink/sq_pkt_sink.py
 src/pysysq/sq_base/sq_plugin/__init__.py
 src/pysysq/sq_base/sq_plugin/sq_helper.py
 src/pysysq/sq_base/sq_plugin/sq_plugin.py
 src/pysysq/sq_base/sq_plugin/sq_plugin_loader.py
 src/pysysq/sq_base/sq_plugin/default/__init__.py
 src/pysysq/sq_base/sq_plugin/default/sq_default_plugin.py
+src/pysysq/sq_base/sq_plugin/default/sq_generic_packet.py
+src/pysysq/sq_base/sq_plugin/default/sq_packet_info.py
 src/pysysq/sq_base/sq_queue/__init__.py
 src/pysysq/sq_base/sq_queue/sq_queue.py
 src/pysysq/sq_base/sq_queue/sq_single_queue.py
 src/pysysq/sq_base/sq_sim_setup_generator/__init__.py
 src/pysysq/sq_base/sq_sim_setup_generator/sq_code_gen_model.py
 src/pysysq/sq_base/sq_sim_setup_generator/sq_sim_data_gen_ctx.py
 src/pysysq/sq_base/sq_sim_setup_generator/sq_sim_data_gen_strategy.py
@@ -78,10 +79,8 @@
 src/pysysq/sq_base/sq_splitter/__init__.py
 src/pysysq/sq_base/sq_splitter/sq_splitter.py
 src/pysysq/sq_base/sq_statistics/__init__.py
 src/pysysq/sq_base/sq_statistics/sq_plotter.py
 src/pysysq/sq_base/sq_statistics/sq_statistics.py
 tests/unittests/__init__.py
 tests/unittests/test_sq_demux.py
-tests/unittests/test_sq_mux.py
-tests/unittests/test_sq_object.py
-tests/unittests/test_sq_pkt_processor.py
+tests/unittests/test_sq_mux.py
```

