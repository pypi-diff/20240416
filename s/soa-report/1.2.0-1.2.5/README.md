# Comparing `tmp/soa_report-1.2.0-py3-none-any.whl.zip` & `tmp/soa_report-1.2.5-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,50 +1,59 @@
-Zip file size: 82757 bytes, number of entries: 48
+Zip file size: 97134 bytes, number of entries: 57
 -rw-r--r--  2.0 unx        0 b- defN 24-Jan-19 09:54 old_modules/__init__.py
 -rw-r--r--  2.0 unx     3343 b- defN 24-Jan-19 09:54 old_modules/soa_run_eps.py
 -rw-r--r--  2.0 unx     1201 b- defN 24-Jan-19 09:54 old_modules/test_soa_report.py
 -rw-r--r--  2.0 unx     2051 b- defN 24-Jan-19 09:54 old_modules/test_soa_report_filter.py
 -rw-r--r--  2.0 unx        0 b- defN 23-May-23 12:11 scripts/__init__.py
--rw-r--r--  2.0 unx       18 b- defN 24-Jan-19 09:54 soa_report/__init__.py
--rw-r--r--  2.0 unx     5914 b- defN 24-Jan-19 09:54 soa_report/scenario_reporter_cmd.py
+-rw-r--r--  2.0 unx       18 b- defN 24-Apr-16 08:50 soa_report/__init__.py
+-rw-r--r--  2.0 unx     5908 b- defN 24-Apr-16 08:50 soa_report/scenario_reporter_cmd.py
 -rw-r--r--  2.0 unx     5986 b- defN 24-Jan-19 09:54 soa_report/segmentation_reporter_cmd.py
 -rw-r--r--  2.0 unx        0 b- defN 23-May-23 12:11 soa_report/commons/__init__.py
 -rw-r--r--  2.0 unx     1840 b- defN 23-May-23 12:11 soa_report/commons/env_variables.py
 -rw-r--r--  2.0 unx     3883 b- defN 24-Jan-19 09:54 soa_report/commons/matplotlib_utils.py
 -rw-r--r--  2.0 unx     1023 b- defN 24-Jan-19 09:54 soa_report/commons/my_log.py
--rw-r--r--  2.0 unx    18853 b- defN 24-Jan-19 09:54 soa_report/commons/plots_utils.py
+-rw-r--r--  2.0 unx    20419 b- defN 24-Apr-16 08:50 soa_report/commons/plots_utils.py
 -rw-r--r--  2.0 unx     2390 b- defN 24-Jan-19 09:54 soa_report/commons/power_pwr.py
 -rw-r--r--  2.0 unx     7623 b- defN 24-Jan-19 09:54 soa_report/commons/rst_report.py
 -rw-r--r--  2.0 unx      663 b- defN 23-May-23 12:11 soa_report/commons/spice_kernel_utils.py
 -rw-r--r--  2.0 unx     1397 b- defN 23-May-23 12:11 soa_report/juice/__init__.py
--rw-r--r--  2.0 unx    46949 b- defN 24-Jan-19 09:54 soa_report/juice/scenario_reporter.py
--rw-r--r--  2.0 unx    53057 b- defN 24-Jan-19 09:54 soa_report/juice/segmentation_reporter.py
+-rw-r--r--  2.0 unx    40326 b- defN 24-Apr-16 08:50 soa_report/juice/scenario_reporter.py
+-rw-r--r--  2.0 unx    54475 b- defN 24-Apr-16 08:50 soa_report/juice/segmentation_reporter.py
 -rw-r--r--  2.0 unx        0 b- defN 23-May-23 12:11 soa_report/juice/eps_data/__init__.py
+-rw-r--r--  2.0 unx     6469 b- defN 24-Apr-16 08:50 soa_report/juice/eps_data/brf.py
 -rw-r--r--  2.0 unx     8277 b- defN 24-Jan-19 09:54 soa_report/juice/eps_data/data_rate_avg.py
--rw-r--r--  2.0 unx     4510 b- defN 24-Jan-19 09:54 soa_report/juice/eps_data/df_data_latency.py
+-rw-r--r--  2.0 unx     1799 b- defN 24-Apr-16 08:50 soa_report/juice/eps_data/df_brf.py
+-rw-r--r--  2.0 unx     3903 b- defN 24-Apr-16 08:50 soa_report/juice/eps_data/df_data_latency.py
 -rw-r--r--  2.0 unx     6453 b- defN 24-Jan-19 09:54 soa_report/juice/eps_data/df_data_rate_avg.py
--rw-r--r--  2.0 unx     1803 b- defN 24-Jan-19 09:54 soa_report/juice/eps_data/df_power_avg.py
--rw-r--r--  2.0 unx     8830 b- defN 24-Jan-19 09:54 soa_report/juice/eps_data/ds_latency.py
+-rw-r--r--  2.0 unx     1802 b- defN 24-Apr-16 08:50 soa_report/juice/eps_data/df_power_avg.py
+-rw-r--r--  2.0 unx     8852 b- defN 24-Apr-16 08:50 soa_report/juice/eps_data/ds_latency.py
+-rw-r--r--  2.0 unx     7602 b- defN 24-Apr-16 08:50 soa_report/juice/eps_data/ds_transfers.py
 -rw-r--r--  2.0 unx      431 b- defN 24-Jan-19 09:54 soa_report/juice/eps_data/epsoutput.py
--rw-r--r--  2.0 unx     8802 b- defN 24-Jan-19 09:54 soa_report/juice/eps_data/power_avg.py
+-rw-r--r--  2.0 unx     2589 b- defN 24-Apr-16 08:50 soa_report/juice/eps_data/file_latency.py
+-rw-r--r--  2.0 unx     7622 b- defN 24-Apr-16 08:50 soa_report/juice/eps_data/power_avg.py
 -rw-r--r--  2.0 unx        0 b- defN 23-May-23 12:11 soa_report/juice/report/__init__.py
--rw-r--r--  2.0 unx    20763 b- defN 24-Jan-19 09:54 soa_report/juice/report/soa_report_basics.py
+-rw-r--r--  2.0 unx    21329 b- defN 24-Apr-16 08:50 soa_report/juice/report/soa_report_basics.py
 -rw-r--r--  2.0 unx     3851 b- defN 23-May-23 12:11 soa_report/juice/report/soa_report_summary.py
 -rw-r--r--  2.0 unx        0 b- defN 23-May-23 12:11 soa_report/juice/segmentation/__init__.py
 -rw-r--r--  2.0 unx     9035 b- defN 24-Jan-19 09:54 soa_report/juice/segmentation/power_metrics.py
 -rw-r--r--  2.0 unx        0 b- defN 23-May-23 12:11 soa_report/juice/soa/__init__.py
 -rw-r--r--  2.0 unx     8997 b- defN 24-Jan-19 09:54 soa_report/juice/soa/power_metrics.py
+-rw-r--r--  2.0 unx    15117 b- defN 24-Apr-16 08:50 soa_report/juice/soa/scenario_compare.py
+-rw-r--r--  2.0 unx    19652 b- defN 24-Apr-16 08:50 soa_report/juice/soa/soa_report_basics.py
 -rw-r--r--  2.0 unx    15613 b- defN 23-May-23 12:11 soa_report/juice/templates/custom-reference.docx
 -rw-r--r--  2.0 unx    13276 b- defN 23-May-23 12:11 soa_report/juice/templates/default_rst2pdf.style
 -rw-r--r--  2.0 unx     5704 b- defN 24-Jan-19 09:54 soa_report/templates/Segmentation_Reporter_Configuration_file.json
 -rw-r--r--  2.0 unx        0 b- defN 23-May-23 12:11 soa_report/templates/__init__.py
--rw-r--r--  2.0 unx     2554 b- defN 24-Jan-19 09:54 soa_report/templates/scenario_reporter.json
+-rw-r--r--  2.0 unx     2331 b- defN 24-Apr-16 08:50 soa_report/templates/scenario_reporter.json
+-rw-r--r--  2.0 unx        0 b- defN 24-Apr-16 08:50 soa_report/utest/__init__.py
+-rw-r--r--  2.0 unx     1279 b- defN 24-Apr-16 08:50 soa_report/utest/utest_epsdata_brf_handling.py
 -rw-r--r--  2.0 unx        0 b- defN 23-May-23 12:11 test/__init__.py
 -rw-r--r--  2.0 unx     1732 b- defN 24-Jan-19 09:54 test/test_scenario_report_e2e.py
 -rw-r--r--  2.0 unx     1775 b- defN 24-Jan-19 09:54 test/test_segmentation_report_e2e.py
--rw-r--r--  2.0 unx     3577 b- defN 24-Jan-19 09:54 test/test_segmentation_report_e2e_not_osve.py
--rw-r--r--  2.0 unx      426 b- defN 24-Apr-15 15:02 soa_report-1.2.0.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 24-Apr-15 15:02 soa_report-1.2.0.dist-info/WHEEL
--rw-r--r--  2.0 unx      142 b- defN 24-Apr-15 15:02 soa_report-1.2.0.dist-info/entry_points.txt
--rw-r--r--  2.0 unx       36 b- defN 24-Apr-15 15:02 soa_report-1.2.0.dist-info/top_level.txt
--rw-rw-r--  2.0 unx     4408 b- defN 24-Apr-15 15:02 soa_report-1.2.0.dist-info/RECORD
-48 files, 287278 bytes uncompressed, 75573 bytes compressed:  73.7%
+-rw-r--r--  2.0 unx     2066 b- defN 24-Apr-16 08:50 test/test_segmentation_report_e2e_not_osve.py
+-rw-r--r--  2.0 unx     2314 b- defN 24-Apr-16 08:50 test/test_segmentation_report_e2e_overwrite.py
+-rw-r--r--  2.0 unx      426 b- defN 24-Apr-16 10:55 soa_report-1.2.5.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 24-Apr-16 10:55 soa_report-1.2.5.dist-info/WHEEL
+-rw-r--r--  2.0 unx      142 b- defN 24-Apr-16 10:55 soa_report-1.2.5.dist-info/entry_points.txt
+-rw-r--r--  2.0 unx       36 b- defN 24-Apr-16 10:55 soa_report-1.2.5.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx     5270 b- defN 24-Apr-16 10:55 soa_report-1.2.5.dist-info/RECORD
+57 files, 338382 bytes uncompressed, 88566 bytes compressed:  73.8%
```

## zipnote {}

```diff
@@ -54,32 +54,44 @@
 
 Filename: soa_report/juice/segmentation_reporter.py
 Comment: 
 
 Filename: soa_report/juice/eps_data/__init__.py
 Comment: 
 
+Filename: soa_report/juice/eps_data/brf.py
+Comment: 
+
 Filename: soa_report/juice/eps_data/data_rate_avg.py
 Comment: 
 
+Filename: soa_report/juice/eps_data/df_brf.py
+Comment: 
+
 Filename: soa_report/juice/eps_data/df_data_latency.py
 Comment: 
 
 Filename: soa_report/juice/eps_data/df_data_rate_avg.py
 Comment: 
 
 Filename: soa_report/juice/eps_data/df_power_avg.py
 Comment: 
 
 Filename: soa_report/juice/eps_data/ds_latency.py
 Comment: 
 
+Filename: soa_report/juice/eps_data/ds_transfers.py
+Comment: 
+
 Filename: soa_report/juice/eps_data/epsoutput.py
 Comment: 
 
+Filename: soa_report/juice/eps_data/file_latency.py
+Comment: 
+
 Filename: soa_report/juice/eps_data/power_avg.py
 Comment: 
 
 Filename: soa_report/juice/report/__init__.py
 Comment: 
 
 Filename: soa_report/juice/report/soa_report_basics.py
@@ -96,14 +108,20 @@
 
 Filename: soa_report/juice/soa/__init__.py
 Comment: 
 
 Filename: soa_report/juice/soa/power_metrics.py
 Comment: 
 
+Filename: soa_report/juice/soa/scenario_compare.py
+Comment: 
+
+Filename: soa_report/juice/soa/soa_report_basics.py
+Comment: 
+
 Filename: soa_report/juice/templates/custom-reference.docx
 Comment: 
 
 Filename: soa_report/juice/templates/default_rst2pdf.style
 Comment: 
 
 Filename: soa_report/templates/Segmentation_Reporter_Configuration_file.json
@@ -111,35 +129,44 @@
 
 Filename: soa_report/templates/__init__.py
 Comment: 
 
 Filename: soa_report/templates/scenario_reporter.json
 Comment: 
 
+Filename: soa_report/utest/__init__.py
+Comment: 
+
+Filename: soa_report/utest/utest_epsdata_brf_handling.py
+Comment: 
+
 Filename: test/__init__.py
 Comment: 
 
 Filename: test/test_scenario_report_e2e.py
 Comment: 
 
 Filename: test/test_segmentation_report_e2e.py
 Comment: 
 
 Filename: test/test_segmentation_report_e2e_not_osve.py
 Comment: 
 
-Filename: soa_report-1.2.0.dist-info/METADATA
+Filename: test/test_segmentation_report_e2e_overwrite.py
+Comment: 
+
+Filename: soa_report-1.2.5.dist-info/METADATA
 Comment: 
 
-Filename: soa_report-1.2.0.dist-info/WHEEL
+Filename: soa_report-1.2.5.dist-info/WHEEL
 Comment: 
 
-Filename: soa_report-1.2.0.dist-info/entry_points.txt
+Filename: soa_report-1.2.5.dist-info/entry_points.txt
 Comment: 
 
-Filename: soa_report-1.2.0.dist-info/top_level.txt
+Filename: soa_report-1.2.5.dist-info/top_level.txt
 Comment: 
 
-Filename: soa_report-1.2.0.dist-info/RECORD
+Filename: soa_report-1.2.5.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## soa_report/__init__.py

```diff
@@ -1 +1 @@
-version = "1.2.0"
+version = "1.2.5"
```

## soa_report/scenario_reporter_cmd.py

```diff
@@ -142,15 +142,15 @@
 
     if 'request' in list(x_dic.keys()):
 
         simu = x_dic['request']
 
         set_request_parameters(simu)
 
-        p = SoaReportFilter(x_dic, simu, working_dir)
+        p = SoaReportFilter(x_dic, working_dir)
         p.create_report()
 
     else:
 
         logging.error('request section missing in configuration file: {}'.format(cfg_file))
         logging.error('This configuration file is not a valid configuration file, please check it!')
         sys.exit()
```

## soa_report/commons/plots_utils.py

```diff
@@ -37,15 +37,14 @@
     if len(instruments) > 0:
         new_parameters = []
         for k in parameters:
 
             for inst in instruments:
 
                 if k.startswith(inst):
-
                     new_parameters.append(k)
 
         parameters = new_parameters
 
     if plot_ax_start is None and plot_ax_end is None:
         (plot_ax_start, plot_ax_end) = (df['datetime (UTC)'][0], df['datetime (UTC)'].iloc[-1])
 
@@ -102,15 +101,14 @@
     if len(instruments) > 0:
         new_parameters = []
         for k in parameters:
 
             for inst in instruments:
 
                 if k.startswith(inst):
-
                     new_parameters.append(k)
 
         parameters = new_parameters
 
     if plot_ax_start is None and plot_ax_end is None:
         (plot_ax_start, plot_ax_end) = (df['datetime (UTC)'][0], df['datetime (UTC)'].iloc[-1])
 
@@ -136,25 +134,24 @@
         if key in df.keys() and ':%' not in key:
             ax1.plot(df['datetime (UTC)'], df[key], linewidth=line_width, label=short_key)
             # ax2.plot(df['timedelta (seconds)'], df[key], linewidth=line_width)
 
         if ':%' in key:
 
             if key in df.keys():
-
                 ax1.set_ylim(0, 100)
                 ax1.set_ylabel(key)
                 ax1.plot(df['datetime (UTC)'], df[key], linewidth=line_width, label=key)
                 t_0, t_final = df['datetime (UTC)'][0], df['datetime (UTC)'].iloc[-1]
-                pos_x_anotate = t_0 + (t_final - t_0)/5
+                pos_x_anotate = t_0 + (t_final - t_0) / 5
                 ax1.plot([t_0, t_final], [80, 80], 'r--')
                 ax1.plot([t_0, t_final], [70, 70], 'g--')
                 # annotate(BATTERY_DOD_SOFT_LIMIT)
                 ax1.annotate('BATTERY_CAPACITY = {} [Watts]'.format(battery_capacity),
-                              xy=(t_0, 5), xytext=(pos_x_anotate, 5), color='r')
+                             xy=(t_0, 5), xytext=(pos_x_anotate, 5), color='r')
                 ax1.annotate('BATTERY_DOD_HARD_LIMIT = 80%', xy=(t_0, 80), xytext=(pos_x_anotate, 81), color='r')
                 ax1.annotate('BATTERY_DOD_SOFT_LIMIT = 70%', xy=(t_0, 70), xytext=(pos_x_anotate, 71), color='g')
 
     ax1.set_ylim(bottom=0)
 
     include_phase_area_df(df, ax1, my_periods)
     matplotlib_utils.add_unified_legend_box(ax1)
@@ -190,15 +187,14 @@
     if len(instruments) > 0:
         new_parameters = []
         for k in parameters:
 
             for inst in instruments:
 
                 if k.startswith(inst):
-
                     new_parameters.append(k)
 
         parameters = new_parameters
 
     if plot_ax_start is None and plot_ax_end is None:
         (plot_ax_start, plot_ax_end) = (df['datetime (UTC)'][0], df['datetime (UTC)'].iloc[-1])
 
@@ -226,20 +222,19 @@
         if key in df.keys() and ':%' not in key:
             ax1.plot(df['datetime (UTC)'], df[key], linewidth=line_width, label=short_key)
             # ax2.plot(df['timedelta (seconds)'], df[key], linewidth=line_width)
 
         if ':%' in key:
 
             if key in df.keys():
-
                 par1.set_ylim(0, 110)
                 par1.set_ylabel(key)
                 par1.plot(df['datetime (UTC)'], df[key], linewidth=line_width, label=key)
                 t_0, t_final = df['datetime (UTC)'][0], df['datetime (UTC)'].iloc[-1]
-                pos_x_anotate = t_0 + (t_final - t_0)/5
+                pos_x_anotate = t_0 + (t_final - t_0) / 5
                 par1.plot([t_0, t_final], [20, 20], 'r--')
                 par1.plot([t_0, t_final], [30, 30], 'g--')
                 par1.plot([t_0, t_final], [100, 100], 'k--')
                 par1.annotate('BATTERY_CAPACITY = {} [Watts]'.format(battery_capacity),
                               xy=(t_0, 101), xytext=(pos_x_anotate, 101), color='k')
                 par1.annotate('BATTERY_DOD_HARD_LIMIT = 20%', xy=(t_0, 20), xytext=(pos_x_anotate, 21), color='r')
                 par1.annotate('BATTERY_DOD_SOFT_LIMIT = 30%', xy=(t_0, 30), xytext=(pos_x_anotate, 31), color='g')
@@ -298,56 +293,103 @@
         matplotlib_utils.set_plot_options(plt, input_path, fig_name=fig_name, option=option)
 
         plt.close()
 
 
 def create_plot_latency_presentation(df_l, input_path, option='png',
                                      fig_name='plot_latency_presentation',
-                                     y_label='Days', my_periods='', antenna_label='HGA'):
+                                     y_label='Days', my_periods='', antenna_label='LINK',
+                                     selected_keys=[]):
     """
     Creates a specific maplotlib graph
 
     :param df_l: input dataframe
     :param input_path: path of the working directory
     :param option: plot option; plot display the plot.
     :param fig_name: Name of the graph and corresponding image.
     :param y_label: y axis label
-    :param my_periods: period to be plot
+    :param my_periods: list of window periods
     :param antenna_label: label use to filter antenna values
+    :param selected_keys: list of selected key; Default is empty, and then all keys are selected
     """
 
-    latency_days = [k for k in df_l.keys() if antenna_label in k]  # and 'Maximum' in k]
+    latency_day_keys = [k for k in df_l.keys() if antenna_label in k]
+    if selected_keys:
+        latency_day_keys = selected_keys
 
-    plt.figure('fig_name', figsize=(12, 8))  # figsize=(16, 10)) =1200)
+    plt.figure('fig_name', figsize=(12, 8))
 
     ax1 = plt.subplot(111)
     ax1.set_ylabel(y_label)
 
-    for key in latency_days:
-        short_key = key
+    for key in latency_day_keys:
+
+        short_key = key.split(':')[1]
         if 'SSMM ' in key:
             short_key = key.split(':')[0].split('SSMM ')[1]
-        if 'Maximum' in key:
-            short_key = key.replace('Maximum', 'Total_Latency')
         if key in df_l.keys():
-            ax1.plot(df_l['datetime (UTC)'], df_l[key], label=short_key)
+            if len(df_l['datetime (UTC)']) < 3:
+                ax1.plot(df_l['datetime (UTC)'], df_l[key], label=short_key, marker='+')
+            else:
+                ax1.plot(df_l['datetime (UTC)'], df_l[key], label=short_key)
 
-    ax1.set_ylim(bottom=0)  # , top=5)
+    ax1.set_ylim(bottom=0)
 
     box = ax1.get_position()
     ax1.set_position([box.x0, box.y0, box.width * 0.85, box.height])
-    ax1.legend(bbox_to_anchor=(1.05, 1), loc=2, borderaxespad=0.)
+    ax1.legend(bbox_to_anchor=(1.01, 1), loc=2, borderaxespad=0., title=antenna_label)
 
     include_phase_area_df(df_l, ax1, my_periods)
 
     matplotlib_utils.set_plot_options(plt, input_path, fig_name=fig_name, option=option)
 
     plt.close()
 
 
+def create_plot_files_latency(dico, input_path, option='png',
+                              fig_name='plot_latency_presentation',
+                              y_label='Days', my_periods=[]):
+    """
+    Creates a specific maplotlib graph
+
+    :param dico: input dico
+    :param input_path: path of the working directory
+    :param option: plot option; plot display the plot.
+    :param fig_name: Name of the graph and corresponding image.
+    :param y_label: y axis label
+    :param my_periods: list of window periods
+    """
+
+    plt.figure('fig_name', figsize=(12, 8))
+
+    ax1 = plt.subplot(111)
+    ax1.set_ylabel(y_label)
+
+    for key in dico.keys():
+
+        short_key = key.replace('SSMM SSMM', 'SSMM')
+
+        if len(dico[key]['datetime (UTC)']) < 3:
+            ax1.plot(dico[key]['datetime (UTC)'], dico[key]['latency'], label=short_key, marker='+')
+        else:
+            ax1.plot(dico[key]['datetime (UTC)'], dico[key]['latency'], label=short_key)
+
+    ax1.set_ylim(bottom=0)
+
+    box = ax1.get_position()
+    ax1.set_position([box.x0, box.y0, box.width * 0.85, box.height])
+    ax1.legend(bbox_to_anchor=(1.01, 1), loc=2, borderaxespad=0., title='File Latency')
+
+    include_phase_area_df(dico, ax1, my_periods)
+
+    matplotlib_utils.set_plot_options(plt, input_path, fig_name=fig_name, option=option)
+
+    plt.close()
+
+
 def create_advanced_plot_ssmm_vs_max(df_a, input_path, option='png',
                                      fig_name='fig', y_label='Gbits', my_periods=[]):
     """
     Creates SSMM plot
 
     :param my_periods: list of window periods
     :param y_label: label of y axis
@@ -376,15 +418,15 @@
         if key in df_a.keys():
             ax1.plot(df_a['datetime (UTC)'], df_a[key], label=short_key)
 
     ax1.set_ylim(bottom=0)
 
     box = ax1.get_position()
     ax1.set_position([box.x0, box.y0, box.width * 0.85, box.height])
-    ax1.legend(bbox_to_anchor=(1.05, 1), loc=2, borderaxespad=0.)
+    ax1.legend(bbox_to_anchor=(1.01, 1), loc=2, borderaxespad=0.)
 
     include_phase_area_df(df_a, ax1, my_periods)
 
     matplotlib_utils.set_plot_options(plt, input_path, fig_name=fig_name, option=option)
 
     plt.close()
 
@@ -534,12 +576,11 @@
     :param my_periods: list of datetime period
     :return:
     """
 
     # Default background color
     ax.patch.set_facecolor('mintcream')  # ('aliceblue') # ('palegreen') mistyrose
 
-    if not df_a.empty:
-        for i in range(len(my_periods)):
-            if i % 2 == 0:
-                ax.fill_between([my_periods[i][0], my_periods[i][1]], 0,
-                                [ax.get_ylim()[1], ax.get_ylim()[1]], facecolor='navajowhite', interpolate=True)
+    for i in range(len(my_periods)):
+        if i % 2 == 0:
+            ax.fill_between([my_periods[i][0], my_periods[i][1]], 0,
+                            [ax.get_ylim()[1], ax.get_ylim()[1]], facecolor='navajowhite', interpolate=True)
```

## soa_report/juice/scenario_reporter.py

```diff
@@ -23,21 +23,21 @@
     get_power_profiles_metrics, get_energy_profiles_metrics, \
     get_power_profiles_metrics_percent
 from soa_report.juice.eps_data.df_data_latency import DfDataLatency
 from soa_report.juice.eps_data.df_power_avg import DfPowerAverage
 from soa_report.juice.eps_data.data_rate_avg import DataRateAverage
 from soa_report.juice.eps_data.ds_latency import DsLatency
 from soa_report.juice.eps_data.power_avg import PowerAverage
-import soa_report.juice.report.soa_report_basics as soa_report_basics
+import soa_report.juice.soa.soa_report_basics as soa_report_basics
 import soa_report.commons.plots_utils as plots_utils
 
 AVAILABLE_POWER_DEF = """
 The available is:
 
-    Available = JUICE + total_instruments + total_available_lost + total_available_stored_in_batt - total_bat_used
+    Available = JUICE + total_instrument + total_available_lost + total_available_stored_in_batt - total_bat_used
 
     where:
 
     * `Available`: Energy available from solar panels for platform, instruments, and charged battery;
     * `JUICE`: Energy used by the JUICE Platform including NAVCAM and RADEM;
     * `total_instruments`: Energy used by instruments;
     * `total_available_lost`: Available energy not used and therefore lost (not needed by platform/instruments and battery recharge);
@@ -48,16 +48,17 @@
 
 
 class SoaReportFilter(soa_report_basics.SoaReportBasics):
     """
     This class allows to report EPS simulation Metrics
     """
 
-    def __init__(self, x, simu, working_dir):
+    def __init__(self, x, working_dir):
 
+        simu = x['request']
         o_simu = namedtuple('Struct', simu.keys())(*simu.values())
 
         partitions_times = [tds.str2datetime(t) for t in o_simu.partition_times]
 
         soa_report_basics.SoaReportBasics.__init__(self, partitions_times, o_simu.add_start_end_scenario)
 
         self.simu = o_simu
@@ -79,69 +80,17 @@
 
         :param x: config parameter object
         :param simu: simulation parameters (OSVE, EPS)
         :param working_dir: working directory
         :return: eps_cfg_parameters: configuration parameters
         """
 
-        import spiceypy as spi
-
-        from osve_wrapper.osve_advanced_wrapper import run_osve
-        from collections import namedtuple
-
         eps_cfg_parameters = None
 
         run_simu = False
-        if hasattr(simu, 'run_simu'):
-            run_simu = simu.run_simu
-
-        if 'osve' in list(x.keys()):
-
-            # Reduce simulation period to the start/end of partitions
-            if simu.add_start_end_scenario:
-
-                x['osve']['start_timeline'] = None
-                x['osve']['end_timeline'] = None
-
-                # Enforce OSVE  to cut Top ITL
-                x['osve']['no_ptr_cut'] = False
-
-            else:
-
-                if len(self.my_date_partition) == 0:
-
-                    x['osve']['start_timeline'] = None
-                    x['osve']['end_timeline'] = None
-
-                    if 'no_ptr_cut' not in x['osve']:
-                        x['osve']['no_ptr_cut'] = False  # OSVE cutting to Top ITL by default
-
-                elif len(self.my_date_partition) == 1:
-
-                    logging.error('partition_times require at least two time when add_start_end_scenario is False (0)')
-                    logging.error('Please review your setting for partition time')
-                    sys.exit()
-
-                else:
-
-                    x['osve']['start_timeline'] = None
-                    x['osve']['end_timeline'] = None
-
-                    x['osve']['filterStartTime'] = self.my_date_partition[0].isoformat()
-                    x['osve']['filterEndTime'] = self.my_date_partition[-1].isoformat()
-
-            o_x_osve = namedtuple('Struct', x['osve'].keys())(*x['osve'].values())
-
-            for experiment_type in simu.experiment_types:
-
-                osve_working_directory = os.path.join(working_dir, o_x_osve.scenario)
-                if run_simu:
-                    eps_cfg_parameters, spice_kernel_md_path = \
-                        run_osve(osve_working_directory, o_x_osve, experiment_type)
-                    spi.furnsh(spice_kernel_md_path)
 
         if not run_simu:
 
             if hasattr(simu, 'battery_capacity_if_sim_not_run'):
                 self.battery_capacity_if_sim_not_run = simu.battery_capacity_if_sim_not_run
                 logging.info('Osve not run; Battery_capacity set to battery_capacity_if_sim_not_run '
                              'configuration parameter: {}'.format(simu.battery_capacity_if_sim_not_run))
@@ -163,195 +112,165 @@
         3) fill report
         4) generate rst, html and docx report
         """
 
         simu = self.simu
         root_path = self.root_path
 
-        (scenario_path, root_path, output_dir, self.plots_path) = \
-            self.set_up_parameters(simu.scenario, root_path, simu.output_dir)
-        experiment_types = simu.experiment_types
+        (root_path, output_dir, self.plots_path) = \
+            self.set_up_parameters(root_path, simu.output_dir)
 
         proc_report = RstReport(self.plots_path, out='rst', output_path=output_dir)
         objective = 'Generate Summary Report'
         if hasattr(simu, 'report_title'):
-            objective = simu.report_title + f': {self.simu.scenario}'
+            objective = simu.report_title
         proc_report.print_summary_intro(objective)
 
-        if experiment_types != ["instrument"]:
-            logging.warning('experiment type must be set to "instrument"')
-
-        self.fill_report(proc_report, scenario_path, experiment_types, output_dir)
+        self.fill_report(proc_report, root_path, output_dir)
 
         proc_report.rst_to_html()
 
         here = os.getcwd()
         os.chdir(output_dir)
         proc_report.pandoc_html_to_docx(docx_style_file=get_template_docx())
         os.chdir(here)
 
         if hasattr(simu, 'report_file_name'):
             proc_report.rename_report(simu.report_file_name, just_rename=True)
 
-    def fill_report(self, proc_report, scenario_path, experiment_types, output_dir, n_level=1):
+    def fill_report(self, proc_report, eps_output_dir, output_dir, n_level=1):
         """
         Fill Sequential report
 
         For each experiment type
             1) Load and parse data_avg, power_avg and DS_latency
             2) Set partitions
             3) Report DS, SSMM, downlink Summary
             4) if requested report Power and Energy summary
             5) add DS, SSMM, downlink Summary for each partition
             6) if requested report Power and Energy summary for each partition
 
         :param proc_report: report object
-        :param scenario_path: scenario root directory
-        :param experiment_types:  list of experiment types  ['instrument_type', 'segment_type', 'target', 'all']
+        :param eps_output_dir: eps output directory path
         :param output_dir: output directory path
         :param n_level: title section baseline number
         """
 
         proc_report.insert_page_break()
 
         eps_cfg_parameters = self.eps_cfg_parameters
 
-        dv_exp_type = {}
-        ds_exp_type = {}
-        df_pow_exp_type = {}
-        for experiment_type in experiment_types:
-
-            proc_report.insert_page_break()
-            proc_report.write_head(n_level, experiment_type.capitalize())
-
-            experiment_type_dir = os.path.join(scenario_path, experiment_type)
-            eps_output_dir = os.path.join(experiment_type_dir, 'eps_output')
-            data_avg = os.path.join(eps_output_dir, 'data_rate_avg.out')
-            ds_latency = os.path.join(eps_output_dir, 'DS_latency.out')
-            if self.simu.include_power_metrics:
-                power_avg = os.path.join(eps_output_dir, 'power_avg.out')
-
-            read_start = None
-            if not self.simu.add_start_end_scenario and len(self.my_date_partition) != 0:
-                read_start = self.my_date_partition[0]
-
-            dv = dv_exp_type[experiment_type] = DataRateAverage(data_avg, read_start=read_start)
-            self.set_partition_period(dv.start, dv.end, self.simu.add_start_end_scenario)
-            my_periods = [[x, self.my_date_partition[i + 1]] for i, x in enumerate(self.my_date_partition[:-1])]
-            dv.df = dv.df[dv.df['datetime (UTC)'] >= my_periods[0][0]]
-            dv.df = dv.df[dv.df['datetime (UTC)'] <= my_periods[-1][-1]]
-            dv.df.reindex()
-            data_frames = self.get_periods(dv)
-
-            ds = ds_exp_type[experiment_type] = load_ds_latency_dataframe(ds_latency)
-            # filter ds.df = ds.df[ds.df['datetime (UTC)'] >= my_periods[0][0]]
-            # filter ds.df = ds.df[ds.df['datetime (UTC)'] >= my_periods[-1][-1]]
-            # filter ds.df.reindex()
-
-            if self.simu.include_power_metrics:
-                df_power = df_pow_exp_type[experiment_type] = \
-                    load_power_avg_dataframe(power_avg, eps_cfg_parameters, read_start=read_start,
-                                             bat_capacity=self.battery_capacity_if_sim_not_run)
-                df_power.df = df_power.df[df_power.df['datetime (UTC)'] >= my_periods[0][0]]
-                df_power.df = df_power.df[df_power.df['datetime (UTC)'] <= my_periods[-1][-1]]
-                df_power.df.reindex()
-                df_power_frames = self.get_periods(df_power)
-
-            # Report Data Budget Summary
-            soa_report_basics.report_summary_table_data_avg_periods(n_level + 1, data_frames, proc_report)
-
-            if self.simu.include_power_metrics:
-                add_power_status_summary(n_level + 1, proc_report, df_power, AVAILABLE_POWER_DEF)
-
-            proc_report.insert_page_break()
-            proc_report.write_head(n_level, experiment_type.capitalize() + ' Details per Experiment and Periods')
-
-            self.generated_dv_summary(n_level + 1, dv, data_frames, proc_report, experiment_type, my_periods)
-
-            self.generated_dvs_and_dvs_vs_downlink(n_level + 1, proc_report, data_frames, experiment_type)
-
-            # dv.df is the dataframe for the entire simulation;
-            # data_frames a list ad dataframe for each partition_period
-            self.generated_dv_accumulated_per_experiment(n_level + 1, proc_report, dv.df, experiment_type, my_periods)
-
-            # Instantaneous data rate per instrument
-            if self.simu.include_instantaneous_data_rate_per_experiment:
-                self.add_instantaneous_data_rate_per_experiment(
-                    n_level + 1, proc_report, dv.df, experiment_type, my_periods)
-
-            # SSMM Status per instrument
-            if self.simu.include_ssmm_status_per_instruments:
-                self.add_ssmm_status_per_instrument(n_level + 1, proc_report, dv.df, experiment_type,
-                                                    my_periods)  # no pkt store for non instrument
-
-            # Downlink Status
-            if self.simu.include_downlink_status_per_instruments:
-                self.add_downlink_status_per_instrument(n_level + 1, proc_report, dv.df, experiment_type, my_periods)
+        proc_report.insert_page_break()
 
-            self.add_latency_report_juice(n_level + 1, proc_report, ds, experiment_type, my_periods)
+        data_avg = os.path.join(eps_output_dir, 'data_rate_avg.out')
+        ds_latency = os.path.join(eps_output_dir, 'DS_latency.out')
+        if self.simu.include_power_metrics:
+            power_avg = os.path.join(eps_output_dir, 'power_avg.out')
+
+        read_start = None
+        if not self.simu.add_start_end_scenario and len(self.my_date_partition) != 0:
+            read_start = self.my_date_partition[0]
+
+        dv = DataRateAverage(data_avg, read_start=read_start)
+        my_periods = self.set_partition_period(dv.start, dv.end, self.simu.add_start_end_scenario)
+
+        dv.df = dv.df[dv.df['datetime (UTC)'] >= my_periods[0][0]]
+        dv.df = dv.df[dv.df['datetime (UTC)'] <= my_periods[-1][-1]]
+        dv.df.reindex()
+        data_frames = self.get_periods(dv)
+
+        ds_latency = load_ds_latency_dataframe(ds_latency)
+
+        if self.simu.include_power_metrics:
+            df_power = load_power_avg_dataframe(power_avg, eps_cfg_parameters, read_start=read_start,
+                                                bat_capacity=self.battery_capacity_if_sim_not_run)
+            df_power.df = df_power.df[df_power.df['datetime (UTC)'] >= my_periods[0][0]]
+            df_power.df = df_power.df[df_power.df['datetime (UTC)'] <= my_periods[-1][-1]]
+            df_power.df.reindex()
+            df_power_frames = self.get_periods(df_power)
 
-            if self.simu.include_power_metrics:
+        # Report Data Budget Summary
+        soa_report_basics.report_summary_table_data_avg_periods(n_level + 1, data_frames, proc_report)
 
-                if hasattr(self.simu, 'include_power_metrics_partition_details'):
-                    add_pwr_metrics_details = self.simu.include_power_metrics_partition_details
-                else:
-                    add_pwr_metrics_details = 0
+        if self.simu.include_power_metrics:
+            add_power_status_summary(n_level + 1, proc_report, df_power, AVAILABLE_POWER_DEF)
+
+        proc_report.insert_page_break()
+        proc_report.write_head(n_level, 'Details per Periods')
+
+        self.generated_dv_summary(n_level + 1, dv, data_frames, proc_report, my_periods)
+
+        self.generated_dvs_and_dvs_vs_downlink(n_level + 1, proc_report, data_frames)
+
+        # dv.df is the dataframe for the entire simulation;
+        # data_frames a list ad dataframe for each partition_period
+        self.generated_dv_accumulated_per_experiment(n_level + 1, proc_report, dv.df, my_periods)
+
+        # Instantaneous data rate per instrument
+        if self.simu.include_instantaneous_data_rate_per_experiment:
+            self.add_instantaneous_data_rate_per_experiment(
+                n_level + 1, proc_report, dv.df, my_periods)
+
+        # SSMM Status per instrument
+        if self.simu.include_ssmm_status_per_instruments:
+            self.add_ssmm_status_per_instrument(n_level + 1, proc_report, dv.df,
+                                                my_periods)  # no pkt store for non instrument
 
-                self.add_power_status_per_experiment(n_level + 1, proc_report, df_power, df_power_frames,
-                                                     experiment_type,
-                                                     my_periods,
-                                                     self.plots_path, my_periods[0][0], my_periods[-1][-1],
-                                                     eps_cfg_parameters=eps_cfg_parameters,
-                                                     include_power_metrics_partition_details=add_pwr_metrics_details,
-                                                     include_plot_experiment_power=False)
-
-        # proc_report.insert_page_break()
-        # proc_report.write_head(n_level, "ANNEX")
-        #
-        # self.report_resources_info(n_level + 1, proc_report, scenario_path, output_dir)
-        # if self.eps_cfg_parameters is not None:
-        #     proc_report.insert_page_break()
-        #     self.report_spice_kernel_info(n_level + 1, proc_report)
-        # else:
-        #     logging.info('OSVE not processed')
+        # Downlink Status
+        if self.simu.include_downlink_status_per_instruments:
+            self.add_downlink_status_per_instrument(n_level + 1, proc_report, dv.df, my_periods)
+
+        self.add_latency_report_juice(n_level + 1, proc_report, ds_latency, my_periods)
+
+        if self.simu.include_power_metrics:
+
+            if hasattr(self.simu, 'include_power_metrics_partition_details'):
+                add_pwr_metrics_details = self.simu.include_power_metrics_partition_details
+            else:
+                add_pwr_metrics_details = 0
+
+            self.add_power_status_per_experiment(n_level + 1, proc_report, df_power, df_power_frames,
+                                                 my_periods,
+                                                 self.plots_path, my_periods[0][0], my_periods[-1][-1],
+                                                 include_power_metrics_partition_details=add_pwr_metrics_details,
+                                                 include_plot_experiment_power=False)
 
         proc_report.print_summary_end()
 
     def generated_dv_per_experiment_vs_downlink_capacity(self, proc_report, dic_sum_accum,
-                                                         experiment_type, my_period='',
+                                                         my_period='',
                                                          total_downlink_capacity=0, title='Generated DV'):
         """
-        Generate rst table including Data volume generated in Gbits for all instruments.
+        Generate rst table including Data volume generated in Gbits for all instrument.
 
         The % of generated dv versus downlink capacity is added in last column
         - if the input total_downlink_capacity=0, then last column is removed
 
         - a pie chart showing generated DV per experiment against total generated DV is added at the end of subsection.
 
         :param proc_report:
         :param dic_sum_accum:
-        :param experiment_type:
         :param my_period:
         :param total_downlink_capacity:
         :param title:
         :return:
         """
 
         if 'NAVCAM' not in dic_sum_accum.keys():
             dic_sum_accum['NAVCAM'] = 0
             logging.warning('Experiment NAVCAM not included in simulation; Set to 0')
 
-        title = '{} per {} [{}]'.format(title, experiment_type, my_period)
+        title = f'{title} per instrument [{my_period}]'
 
-        text_table = ('\n\nThe table bellow provides for each {} in [{}]: \n\n'
+        text_table = (f'\n\nThe table bellow provides for each instrument in [{my_period.replace("_", ", ")}]: \n\n'
                       '* Generated DV in Gbits;\n\n'
                       '* Percentage Generated DV against Total generated in Gbits\n\n'
-                      ).format(experiment_type, my_period.replace('_', ', '))
+                      )
 
-        metric_header = [experiment_type, 'Generated DV (Gbits)', '[%] Generated DV']
+        metric_header = ['Instrument', 'Generated DV (Gbits)', '[%] Generated DV']
 
         total_dv_generated = sum(dic_sum_accum.values())
 
         if total_downlink_capacity:
             text_table += '* Percentage Generated DV against Total Downlink Capacity in Gbits\n\n'
             text_table += '* Percentage Generated DV against Science downlink Capacity in Gbits\n\n'
 
@@ -417,38 +336,37 @@
         if len(metrics) > 0:
             proc_report.print_rst_table(metrics)
 
         for ch in [':', 'T', '-', '=']:
             my_period = my_period.replace(ch, '').replace(' ', '_')
 
         my_period_label = my_period.replace('otal_', 'Total')
-        plot_name = experiment_type + '_' + my_period_label
+        plot_name = f'instrument_{my_period_label}'
         plot_file_path = create_plot_pie(self.plots_path, plot_name, percent, min_values=0.01,
                                          colors=colors)
         plot_file_path = os.path.join('plots', os.path.basename(plot_file_path))
         figure = [plot_file_path]
 
         for fig in figure:
             fig = os.path.expandvars(fig)
             proc_report.rst_insert_figure(fig, title=title, text='')
 
-    def generated_dvs_and_dvs_vs_downlink(self, n_level, proc_report, dfs, experiment_type):
+    def generated_dvs_and_dvs_vs_downlink(self, n_level, proc_report, dfs):
         """
-        Generates rst table including Data volume generated in Gbits for all instruments
+        Generates rst table including Data volume generated in Gbits for all instrument
         - Generate a subsection with a table including the Generated dv for the entire simulation
         - if there are more than on period/partition, add a subsection with on table per partition
 
-        :param n_level: headking level number
+        :param n_level: head level number
         :param proc_report:
         :param dfs: dictionary including a subset of dataframes; keys are labels <start>_<end>
-        :param experiment_type:
         :return:
         """
 
-        proc_report.print_summary_section(n_level, 'Generated DV vs Downlink per {}'.format(experiment_type))
+        proc_report.print_summary_section(n_level, 'Generated DV vs Downlink per instrument')
 
         dico_total = {}
         for key in dfs.keys():
             dic_sum_accum = dfs[key].get_total_accum_data_volume()
             for k in dic_sum_accum.keys():
                 if k not in dico_total.keys():
                     dico_total[k] = dic_sum_accum[k]
@@ -460,252 +378,226 @@
 
         date_format = '%Y-%m-%dT%H:%M:%S'
         total_window = 'Total = {}_{}'.format(datetime.datetime.strftime(self.my_date_partition[0], date_format),
                                               datetime.datetime.strftime(self.my_date_partition[-1], date_format))
 
         proc_report.print_summary_section(n_level + 1, 'Total Periods')
         self.generated_dv_per_experiment_vs_downlink_capacity(
-            proc_report, dico_total, experiment_type, total_window, total_downlink_capacity=sum(values),
+            proc_report, dico_total, total_window, total_downlink_capacity=sum(values),
             title='Generated DV vs Downlink')
 
         if len(dfs.keys()) > 1:
 
             for key in sorted(dfs.keys()):
                 proc_report.print_summary_section(n_level + 1, 'Sub-periods [{}]'.format(key))
 
                 dic_sum_accum = dfs[key].get_total_accum_data_volume()
                 total_downlink = dfs[key].get_total_downlink()
                 self.generated_dv_per_experiment_vs_downlink_capacity(
-                    proc_report, dic_sum_accum, experiment_type + '_vs_Downlink', key,
+                    proc_report, dic_sum_accum, 'instrument_vs_Downlink', key,
                     total_downlink_capacity=total_downlink, title='Generated DV vs Downlink')
 
-    def add_latency_report_juice(self, n_level, proc_report, ds, experiment_type, my_periods,
-                                 objective_summary=''):
+    def add_latency_report_juice(self, n_level, proc_report, ds, my_periods, objective_summary=''):
         """
-        Generate rst table including Data volume generated in Gbits for all instruments
+        Generate rst table including Data volume generated in Gbits for all instrument
 
         :param n_level: Report header level
         :param proc_report: report object
         :param ds: ds latency dataframe
-        :param experiment_type: experiment type (i.e. instrument, target)
         :param my_periods: curent period [start, end]
         :param objective_summary: text summary
         :return:
         """
 
         if ds.df is None:
 
             logging.info('There is no latency; Latency file empty')
 
         else:
 
-            dfs = self.get_periods(ds, DfDataLatency)
-
             title = 'Data Latency'
             logging.debug(title)
 
             text = """The table bellow provides for each packet store:
                       \n * Latency: The Maximum latency in days
                       \n * Average: The mean value of the latency in days
                       \n * Instrument: instrument name\n\n"""
 
-            sub_phases_header = ['Metric'] + [s.replace('_', ' ') for s in sorted(dfs.keys())] + ['All']
-            metrics = [sub_phases_header]
-            values = [max(dfs[k].get_max_latency().values()) for k in sorted(dfs.keys())]
-            metrics.append(['Maximum latency in days'] + values + [max(values)])
-            values = [round(np.mean(list(dfs[k].get_mean_latency().values())), 2) for k in sorted(dfs.keys())]
-            metrics.append(['Average latency in days'] + values + [round(np.mean(values), 2)])
+            keys = sorted([k for k in ds.df.keys() if 'time' not in k and 'Maximum' not in k])
+
+            sub_phases_header = ['Metric'] + [s.replace('_', ' ') for s in keys]
+            metrics = [sub_phases_header,
+                       ['Maximum latency in days'] + [ds.df[k].max() for k in keys],
+                       ['Average latency in days'] + [round(ds.df[k].mean(), 2) for k in keys]]
 
             if len(metrics[0]) > 4:
                 metrics = np.array(metrics).T.tolist()
 
             proc_report.print_summary_section(n_level, title, objective_summary=text, metrics=metrics, figure=[])
 
-            # sub_phases_header = [experiment_type.capitalize(), 'Mean latency [Days]', 'Max latency [Days]']
-            # latency_days = [k for k in ds.df.keys() if 'B-LINK' in k]  # and 'Maximum' in k]
+            for label in ['KAB_LINK', 'XB_LINK']:
+                fig_name = f'data_latency_{label}_instrument'
+                key_label = [k for k in keys if label in k]
+                plots_utils.create_plot_latency_presentation(ds.df, self.plots_path, option='png',
+                                                             antenna_label=label, fig_name=fig_name,
+                                                             y_label='Days', my_periods=my_periods,
+                                                             selected_keys=key_label)
+                plot_file_path = os.path.join('plots', os.path.basename(fig_name + '.png'))
+                proc_report.rst_insert_figure(plot_file_path, title='Data Latency', text=objective_summary)
 
-            # for k in sorted(dfs.keys()):
-            #     title = 'Sub-period per {} [{}]'.format(experiment_type, k)
-            #     metrics = [sub_phases_header]
-            #     mean_latency = dfs[k].get_mean_latency()
-            #     max_latency = dfs[k].get_max_latency()
-            #     # print mean_latency
-            #     # print max_latency
-            #     for l in mean_latency.keys():
-            #         if 'Maximum' in l:
-            #             to_end = [l, round(mean_latency[l], 2), round(max_latency[l], 2)]
-            #         else:
-            #             metrics.append([l, round(mean_latency[l], 2), round(max_latency[l], 2)])
-            #             # metrics.append([l, round(mean_latency[l], 10), round(max_latency[l], 10)])
-            #
-            #     proc_report.print_summary_section(n_level + 1, title, objective_summary=text, metrics=metrics,
-            #                                       figure=[])
-
-            fig_name = 'data_latency_' + experiment_type
-            plots_utils.create_plot_latency_presentation(ds.df, self.plots_path, option='png',
-                                                         fig_name=fig_name, y_label='Days', my_periods=my_periods)
-            plot_file_path = os.path.join('plots', os.path.basename(fig_name + '.png'))
-            proc_report.rst_insert_figure(plot_file_path, title='Data Latency', text=objective_summary)
-
-    def add_instantaneous_data_rate_per_experiment(self, n_level, proc_report, df, experiment_type, my_periods):
+    def add_instantaneous_data_rate_per_experiment(self, n_level, proc_report, df, my_periods):
         """
         Add Datarate Generation per instrument subsection in the report
 
         :param n_level: Report header level
         :param proc_report: report object
         :param df: data_avg dataframe
-        :param experiment_type: experiment type (i.e. instrument, target)
         :param my_periods: current windows time
         """
 
-        proc_report.print_summary_section(n_level, 'Datarate Generation per {}'.format(experiment_type))
+        proc_report.print_summary_section(n_level, 'Data rate Generation per instrument')
 
-        fig_name = 'plot_datarate_generation_{}'.format(experiment_type)
+        fig_name = 'plot_datarate_generation_instrument'
 
         list_of_experiments = [k for k in df.keys() if 'Upload' in k]
 
         plots_utils.create_advanced_plot_1ax_2ay(df, self.plots_path, list_of_experiments,
                                                  option='png', fig_name=fig_name, my_periods=my_periods,
                                                  y_label='kbits / sec')
 
         fig_path = os.path.join('plots', fig_name + '.png')
-        proc_report.rst_insert_figure(fig_path, title='Datarate Generation for {}'.format(experiment_type), text='')
+        proc_report.rst_insert_figure(fig_path, title='Datarate Generation for instrument', text='')
 
         for k in list_of_experiments:
-            fig_name = 'plot_datarate_generation_{}_{}'.format(experiment_type, k.split(':')[0])
+            fig_name = f'plot_datarate_generation_instrument_{k.split(":")[0]}'
             plots_utils.create_advanced_plot_1ax_2ay(df, self.plots_path, [k], option='png',
                                                      fig_name=fig_name, my_periods=my_periods, y_label='kbits / sec')
 
             proc_report.rst_insert_figure(os.path.join('plots', fig_name + '.png'),
                                           title='{} Datarate Generation'.format(k.split(':')[0]),
                                           text='')
 
-    def add_ssmm_status_per_instrument(self, n_level, proc_report, df, experiment_type, my_periods):
+    def add_ssmm_status_per_instrument(self, n_level, proc_report, df, my_periods):
         """
         Add SSMM packet store status per experiment subsection in the report
 
         :param n_level: Report header level
         :param proc_report: report object
         :param df: data_avg dataframe
-        :param experiment_type: experiment type (i.e. instrument, target)
         :param my_periods: current windows time
         """
 
-        proc_report.print_summary_section(n_level, 'SSMM Status per {}'.format(experiment_type))
+        proc_report.print_summary_section(n_level, 'SSMM Status per instrument')
 
-        fig_name = 'plot_ssmm_pkstore_{}'.format(experiment_type)
+        fig_name = 'plot_ssmm_pkstore_instrument'
 
         list_of_experiments = [k for k in df.keys() if 'Memory' in k]
 
         plots_utils.create_advanced_plot_1ax_2ay(df, self.plots_path, list_of_experiments,
                                                  option='png', fig_name=fig_name, my_periods=my_periods,
                                                  y_label='Gbits')
 
         proc_report.rst_insert_figure(os.path.join('plots', fig_name + '.png'),
-                                      title='SSMM Packet Store [Gbits] for {}'.format(experiment_type),
+                                      title='SSMM Packet Store [Gbits] for instrument',
                                       text='')
 
         for k in list_of_experiments:
 
-            fig_name = 'plot_sssm_pkstore_{}_{}'.format(experiment_type, k.split(':')[0].replace(' ', '_'))
+            fig_name = f'plot_sssm_pkstore_instrument_{k.split(":")[0].replace(" ", "_")}'
             plots_utils.create_advanced_plot_1ax_2ay(df, self.plots_path, [k], option='png',
                                                      fig_name=fig_name, my_periods=my_periods, y_label='Gbits')
 
             if df[k].max() > 0:
 
                 proc_report.rst_insert_figure(os.path.join('plots', fig_name + '.png'),
                                               title='{} SSMM Packet Store [Gbits]'.format(k.split(':')[0]),
                                               text='')
 
             else:
                 proc_report.write_text('\n{} SSMM Packet Store = 0 [Gbits] (always empty)\n'.format(k.split(':')[0]))
 
-    def add_downlink_status_per_instrument(self, n_level, proc_report, df, experiment_type, my_periods):
+    def add_downlink_status_per_instrument(self, n_level, proc_report, df, my_periods):
         """
         Add packet store downlink status per experiment subsection in the report
 
         :param n_level: Report header level
         :param proc_report: report object
         :param df: data_avg dataframe
-        :param experiment_type: experiment type (i.e. instrument, target)
         """
 
-        proc_report.print_summary_section(n_level, 'Downlink Status per {}'.format(experiment_type))
+        proc_report.print_summary_section(n_level, 'Downlink Status per instrument')
 
-        fig_name = 'plot_downlink_{}'.format(experiment_type)
+        fig_name = 'plot_downlink_instrument'
 
         list_of_experiments = [k for k in df.keys() if 'Downlink' in k or 'Download' in k]
 
         plots_utils.create_advanced_plot_1ax_2ay(df, self.plots_path, list_of_experiments,
                                                  option='png', fig_name=fig_name, my_periods=my_periods,
                                                  y_label='Gbits')
 
         proc_report.rst_insert_figure(os.path.join('plots', fig_name + '.png'),
-                                      title='Downlink [Gbits] for {}'.format(experiment_type),
+                                      title='Downlink [Gbits]',
                                       text='')
 
         for k in list_of_experiments:
-            fig_name = 'plot_downlink_{}_{}'.format(experiment_type, k.split(':')[0].replace(' ', '_'))
+            fig_name = f'plot_downlink_instrument_{k.replace(":", "").replace("_", "").replace("-", "")}'
             plots_utils.create_advanced_plot_1ax_2ay(df, self.plots_path, [k], option='png',
                                                      fig_name=fig_name, my_periods=my_periods, y_label='Gbits')
 
             if df[k].max() > 0:
 
                 proc_report.rst_insert_figure(os.path.join('plots', fig_name + '.png'),
                                               title='{} Downlink [Gbits]'.format(k.split(':')[0]),
                                               text='')
 
             else:
                 proc_report.write_text('\n{} SSMM Packet Store = 0 [Gbits] (always empty)\n'.format(k.split(':')[0]))
 
-    def add_power_status_per_experiment(self, n_level, proc_report, df_power, df_power_frames, experiment_type,
+    def add_power_status_per_experiment(self, n_level, proc_report, df_power, df_power_frames,
                                         my_periods, plots_dir, start, end, objective_summary='',
-                                        eps_cfg_parameters=None,
                                         include_power_metrics_partition_details=False,
                                         include_plot_experiment_power=False):
         """
         Add power per experiment subsection in the report
 
         :param n_level: Report header level
         :param proc_report: report object
         :param df_power: df power dataframe
         :param df_power_frames: df power dataframe for current period
-        :param experiment_type: experiment type (i.e. instrument, target)
         :param my_periods: current period [start, end]
         :param plots_dir: path to plot directory
         :param start: absolute stat time
         :param end: absolute end time
         :param objective_summary: text summary
-        :param eps_cfg_parameters: epd.cfg parameters
         :param include_plot_experiment_power: flag to add power info; False by default
         :param include_power_metrics_partition_details: flag to add sub-periods details;
             False by default to reduce report size.
         """
 
         if df_power.df is None:
 
             logging.info('There is no power_avg; file empty')
 
         else:
 
             dfs = df_power_frames
 
-            proc_report.write_head(n_level, 'Power Status per {}'.format(experiment_type))
+            proc_report.write_head(n_level, 'Power Status per instrument')
 
             title = 'Power Average'
             logging.debug(title)
 
             bat_percent = [label for label in df_power.df.keys() if '%' in label]
             inst_platform = \
                 ['Available:Watts', 'Available_power_for_science:Watts', 'Batt. DoD:Watts', 'Batt.:Watts',
                  'XB_LINK:Watts', 'KAB_LINK:Watts', 'NAVCAM:Watts', 'RADEM:Watts', 'SSMM:Watts', 'JUICE_platform:Watts',
                  'JUICE:Watts', 'Batt_discharges:Watts']
-            no_instruments = bat_percent + inst_platform
+            no_instrument = bat_percent + inst_platform
             inst_experiment = [label for label in df_power.df.keys() if
-                               label not in no_instruments and "Watts" in label]
+                               label not in no_instrument and "Watts" in label]
             inst_platform = [label for label in inst_platform if label in df_power.df.keys()]
 
             proc_report.write_head(n_level + 1, 'Total Periods ')
             proc_report.write_head(n_level + 2, 'Power Status')
 
             import copy
             my_df_power = copy.copy(df_power)
@@ -714,77 +606,77 @@
             tmp_experiment = calculate_power_status(df_power_total.df, inst_filter=inst_experiment)
             tmp_bat_per = calculate_power_status(df_power_total.df, inst_filter=bat_percent)
 
             proc_report.print_rst_table(get_power_profiles_metrics(tmp_platform))
             proc_report.print_rst_table(get_power_profiles_metrics(tmp_experiment))
             proc_report.print_rst_table(get_power_profiles_metrics_percent(tmp_bat_per))
 
-            fig_name = 'Power_{}'.format(experiment_type)
+            fig_name = 'Power_instrument'
             plots_utils.create_plot_power_avg(df_power.df, plots_dir, fig_name=fig_name,
-                                              instruments=['Available:Watts', 'total_instruments:Watts',
+                                              instruments=['Available:Watts', 'total_instrument:Watts',
                                                            'JUICE_platform:Watts',
                                                            'Batt_discharges:Watts'],
                                               my_periods=my_periods)
 
             proc_report.rst_insert_figure(os.path.join('plots', fig_name + '.png'),
                                           title='Power Status',
                                           text='')
 
-            fig_name = 'Power_RF_{}'.format(experiment_type)
+            fig_name = 'Power_RF_instrument'
             plots_utils.create_plot_power_avg(df_power.df, plots_dir, fig_name=fig_name,
                                               instruments=['XB_LINK:Watts', 'KAB_LINK:Watts'],
                                               my_periods=my_periods)
 
             proc_report.rst_insert_figure(os.path.join('plots', fig_name + '.png'),
                                           title='Power Status RF',
                                           text='')
 
-            fig_name = 'Power_used{}'.format(experiment_type)
+            fig_name = 'Power_used_instrument'
             plots_utils.create_plot_power_avg(df_power.df, plots_dir, fig_name=fig_name,
                                               instruments=['total_bat_used:Watts',
                                                            'total_available_not_used_stored_in_batt:Watts',
                                                            'total_available_lost:Watts'],
                                               my_periods=my_periods)
 
             proc_report.rst_insert_figure(os.path.join('plots', fig_name + '.png'),
                                           title='Power Status Used',
                                           text='')
 
             proc_report.rst_insert_figure(os.path.join('plots', fig_name + '.png'),
                                           title='Science Power',
                                           text='')
 
-            fig_name = 'plot_power_batt_dod_{}'.format(experiment_type)
+            fig_name = 'plot_power_batt_dod_instrument'
             plots_utils.create_plot_bat_dod(df_power, plots_dir, fig_name=fig_name,
                                             instruments=['Batt. DoD:Watts', 'Batt. DoD:%'],
                                             my_periods=my_periods, y_label='Batt. DoD:Watts')
 
             proc_report.rst_insert_figure(os.path.join('plots', fig_name + '.png'),
-                                          title='Power Batt DoD for {}'.format(experiment_type),
+                                          title='Power Batt DoD',
                                           text='')
 
-            fig_name = 'plot_power_batt_status_{}'.format(experiment_type)
+            fig_name = 'plot_power_batt_status_instrument'
             plots_utils.create_plot_bat_status(df_power, plots_dir, fig_name=fig_name,
                                                instruments=['Batt.:Watts', 'Batt.:%'],
                                                my_periods=my_periods, y_label='Batt.:Watts')
 
             proc_report.rst_insert_figure(os.path.join('plots', fig_name + '.png'),
-                                          title='Power Batt Status for {}'.format(experiment_type),
+                                          title='Power Batt Status',
                                           text='')
 
             proc_report.write_head(n_level + 2, 'Power  Accum')
 
             for inst in inst_experiment:
-                fig_name = 'plot_power_avg_{}_{}'.format(experiment_type, inst.split(':')[0])
+                fig_name = f'plot_power_avg_instrument_{inst.split(":")[0]}'
                 plots_utils.create_plot_power_avg(df_power.df, plots_dir, fig_name=fig_name,
                                                   instruments=[inst],
                                                   my_periods=my_periods)
 
                 proc_report.rst_insert_figure(os.path.join('plots', fig_name + '.png'),
-                                              title='Power Average for {}:{}'.format(experiment_type, inst),
+                                              title=f'Power Average for instrument: {inst}',
                                               text='')
 
             proc_report.write_head(n_level + 2, 'Energy Status')
 
             proc_report.write_text(AVAILABLE_POWER_DEF)
 
             metrics = get_energy_profiles_metrics(tmp_platform)
@@ -793,34 +685,34 @@
             metrics = get_energy_profiles_metrics(tmp_experiment)
             proc_report.print_rst_table(metrics)
 
             percent = {}
             for [k, val_start, val_end, val_delta] in metrics:
                 if 'SEGMENT' not in k and 'otal' not in k:
                     percent[k] = float(val_delta)
-                elif k.startswith('total_instruments'):
+                elif k.startswith('total_instrument'):
                     total_percent = float(val_delta)
 
             if total_percent > 0:
 
                 for k, val in percent.items():
                     percent[k] = round(val / total_percent * 100, ndigits=2)
 
-                fig_name = 'pie_energy_{}'.format(experiment_type)
+                fig_name = 'pie_energy_instrument'
                 plots_utils.create_plot_pie(plots_dir, fig_name, percent, min_values=0.01, colors=colors)
                 proc_report.rst_insert_figure(os.path.join('plots', fig_name + '.png'),
                                               title='science Instrument: Energy Sharing',
                                               text='')
             else:
 
                 logging.warning('no instrument consumption during this periods')
 
             proc_report.write_head(n_level + 2, 'Energy Accum')
 
-            fig_name = 'plot_energy_accum_{}'.format(experiment_type)
+            fig_name = 'plot_energy_accum_instrument'
             plots_utils.create_plot_power_avg(df_power.df, plots_dir, fig_name=fig_name,
                                               instruments=['Available_energy_accum:Wh',
                                                            'total_platform_and_science_energy_accum:Wh',
                                                            'total_available_stored_in_batt_energy_accum:Wh',
                                                            'total_available_lost_energy_accum:Wh',
                                                            'total_bat_used_energy_accum:Wh'],
                                               my_periods=my_periods, y_label='Energy (Wh)')
@@ -828,48 +720,47 @@
             proc_report.rst_insert_figure(os.path.join('plots', fig_name + '.png'),
                                           title='Energy Accum',
                                           text='')
 
             for inst in inst_experiment:
 
                 inst_key = inst.replace(':Watts', "_energy_accum:Wh")
-                fig_name = 'plot_energy_accum_{}_{}'.format(experiment_type, inst.split(':')[0])
+                fig_name = f'plot_energy_accum_instrument_{inst.split(":")[0]}'
                 plots_utils.create_plot_power_avg(df_power.df, plots_dir, fig_name=fig_name,
                                                   instruments=[inst_key], y_label='Energy [Wh]',
                                                   my_periods=my_periods)
 
                 if df_power.df[inst_key].max() > 0:
 
                     proc_report.rst_insert_figure(os.path.join('plots', fig_name + '.png'),
-                                                  title='Accumulate Energy for {}:{}'.format(experiment_type,
-                                                                                             inst_key),
+                                                  title=f'Accumulate Energy for instrument:{inst_key}',
                                                   text='')
                 else:
 
                     proc_report.write_text('\n {} = 0 [Wh] (always empty).\n'.format(inst_key))
 
             if include_power_metrics_partition_details:
 
                 if len(my_periods) == 1:
                     logging.info('There is only one period!; So need to add partition details')
                     return 0
 
                 for k in sorted(dfs.keys()):
 
-                    title = 'Sub-period per {} [{}]'.format(experiment_type, k)
+                    title = f'Sub-period per instrument [{k}]'
 
                     proc_report.write_head(n_level + 1, title)
 
                     proc_report.write_head(n_level + 2, 'Power')
 
-                    fig_name = 'plot_power_available_{}_{}'.format(experiment_type,
-                                                                   k.replace(':', '').replace('_', '').replace('-', ''))
+                    fig_name = f'plot_power_available_instrument_' \
+                               f'{k.replace(":", "").replace("_", "").replace("-", "")}'
 
                     plots_utils.create_plot_power_avg(dfs[k].df, plots_dir, fig_name=fig_name,
-                                                      instruments=['Available:Watts', 'total_instruments:Watts',
+                                                      instruments=['Available:Watts', 'total_instrument:Watts',
                                                                    'JUICE_platform:Watts'],
                                                       my_periods=my_periods)
 
                     proc_report.rst_insert_figure(os.path.join('plots', fig_name + '.png'),
                                                   title='Power Status',
                                                   text='')
 
@@ -879,23 +770,23 @@
 
                     proc_report.print_rst_table(get_power_profiles_metrics(tmp_platform))
                     proc_report.print_rst_table(get_power_profiles_metrics(tmp_experiment))
                     proc_report.print_rst_table(get_power_profiles_metrics_percent(tmp_bat_per))
 
                     if include_plot_experiment_power:
                         for inst in inst_experiment:
-                            fig_name = 'plot_power_avg_{}_{}_{}'.format(
-                                experiment_type, inst, k.replace(':', '').replace('_', '').replace('-', ''))
+                            fig_name = f'plot_power_avg_{inst}_' \
+                                       f'{k.replace(":", "").replace("_", "").replace("-", "")}'
 
                             plots_utils.create_plot_power_avg(dfs[k].df, plots_dir, fig_name=fig_name,
                                                               instruments=[inst],
                                                               my_periods=my_periods)
 
                             proc_report.rst_insert_figure(os.path.join('plots', fig_name + '.png'),
-                                                          title=f'Power Average for {experiment_type}:{inst}',
+                                                          title=f'Power Average for instrument: {inst}',
                                                           text='')
 
                     proc_report.write_head(n_level + 2, 'Energy Status')
 
                     proc_report.write_text(AVAILABLE_POWER_DEF)
 
                     metrics = get_energy_profiles_metrics(tmp_platform)
@@ -904,38 +795,38 @@
                     metrics = get_energy_profiles_metrics(tmp_experiment)
                     proc_report.print_rst_table(metrics)
 
                     percent = {}
                     for val, val_start, val_end, val_delta in metrics:
                         if 'SEGMENT' not in k and 'otal' not in val:
                             percent[val] = float(val_delta)
-                        elif val.startswith('total_instruments'):
+                        elif val.startswith('total_instrument'):
                             total_percent = float(val_delta)
                     for key, val in percent.items():
                         percent[key] = round(val / total_percent * 100, ndigits=2)
 
-                    fig_name = 'pie_energy_{}{}'.format(experiment_type,
-                                                        k.replace(':', '').replace('_', '').replace('-', ''))
+                    fig_name = f'pie_energy_instrument_{k.replace(":", "").replace("_", "").replace("-", "")}'
+
                     plots_utils.create_plot_pie(plots_dir, fig_name, percent, min_values=0.01, colors=colors)
                     proc_report.rst_insert_figure(os.path.join('plots', fig_name + '.png'),
                                                   title='science Instrument: Energy Sharing',
                                                   text='')
 
                     for inst in inst_experiment:
 
                         inst_key = inst.replace(':Watts', "_energy_accum:Wh")
-                        fig_name = 'plot_energy_accum_{}_{}'.format(experiment_type, inst.split(':')[0])
+                        fig_name = f'plot_energy_accum_instrument_{inst.split(":")[0]}'
                         plots_utils.create_plot_power_avg(dfs[k].df, plots_dir, fig_name=fig_name,
                                                           instruments=[inst_key], y_label='Energy [Wh]',
                                                           my_periods=my_periods)
 
                         if df_power.df[inst_key].max() > 0:
 
                             proc_report.rst_insert_figure(os.path.join('plots', fig_name + '.png'),
-                                                          title=f'Accumulate Energy for {experiment_type}:{inst_key}',
+                                                          title=f'Accumulate Energy for instrument:{inst_key}',
                                                           text='')
                         else:
 
                             proc_report.write_text('\n {} = 0 [Wh] (always empty).\n'.format(inst_key))
 
 
 def load_power_avg_dataframe(power_avg, eps_cfg_parameters, read_start=None, bat_capacity=None):
```

## soa_report/juice/segmentation_reporter.py

```diff
@@ -2,36 +2,34 @@
 Created on March 2019
 
 @author: Claudio Munoz Crego (ESAC)
 
 This Module allows to report soa_report subsection including plots
 """
 
+import datetime
+import logging
 import os
 import sys
-import logging
-import datetime
-import numpy as np
-
 from collections import namedtuple
 
-import esac_juice_pyutils.commons.tds as tds
+import numpy as np
 
-from soa_report.commons.rst_report import RstReport
+import esac_juice_pyutils.commons.tds as tds
+import soa_report.commons.plots_utils as plots_utils
+import soa_report.juice.report.soa_report_basics as report_basics
 from soa_report.commons.plots_utils import create_plot_pie
-from soa_report.juice.segmentation.power_metrics import add_power_status_summary, calculate_power_status, \
-    get_power_profiles_metrics, get_energy_profiles_metrics, get_power_profiles_metrics_percent
+from soa_report.commons.rst_report import RstReport
+from soa_report.juice.eps_data.data_rate_avg import DataRateAverage
 from soa_report.juice.eps_data.df_data_rate_avg import DfDataRateAverage
-from soa_report.juice.eps_data.df_data_latency import DfDataLatency
 from soa_report.juice.eps_data.df_power_avg import DfPowerAverage
-from soa_report.juice.eps_data.data_rate_avg import DataRateAverage
 from soa_report.juice.eps_data.ds_latency import DsLatency
 from soa_report.juice.eps_data.power_avg import PowerAverage
-import soa_report.juice.report.soa_report_basics as report_basics
-import soa_report.commons.plots_utils as plots_utils
+from soa_report.juice.segmentation.power_metrics import add_power_status_summary, calculate_power_status, \
+    get_power_profiles_metrics, get_energy_profiles_metrics, get_power_profiles_metrics_percent
 
 
 class SoaReportFilter(report_basics.SoaReportBasics):
     """
     This class allows to report EPS simulation Metrics
     """
 
@@ -67,26 +65,26 @@
         :param x: config parameter object
         :param simu: simulation parameters (OSVE, EPS)
         :param working_dir: working directory
         :return: eps_cfg_parameters: configuration parameters
         """
 
         import spiceypy as spi
-
-        from osve_wrapper.osve_advanced_wrapper import run_osve
         from collections import namedtuple
 
         eps_cfg_parameters = None
 
         run_simu = True
         if hasattr(simu, 'run_simu'):
             run_simu = simu.run_simu
 
         if run_simu:
 
+            from osve_wrapper.osve_advanced_wrapper import run_osve
+
             if 'osve' not in list(x.keys()):
                 logging.error('"osve" section not defined in configuration file; Please check')
                 logging.error('"osve" is required if run_simu is true/1 or not specified in configuration file')
                 sys.exit(0)
 
             # Reduce simulation period to the start/end of partitions
             if simu.add_start_end_scenario:
@@ -223,14 +221,15 @@
                 proc_report.write_head(n_level, experiment_type.capitalize())
                 n_level += 1
 
             experiment_type_dir = os.path.join(scenario_path, experiment_type)
             eps_output_dir = os.path.join(experiment_type_dir, 'eps_output')
             data_avg = os.path.join(eps_output_dir, 'data_rate_avg.out')
             ds_latency = os.path.join(eps_output_dir, 'DS_latency.out')
+            ds_transfers = os.path.join(eps_output_dir, 'DS_transfers.out')
             if self.simu.include_power_metrics:
                 power_avg = os.path.join(eps_output_dir, 'power_avg.out')
 
             read_start = None
             if not self.simu.add_start_end_scenario and len(self.my_date_partition) != 0:
                 read_start = self.my_date_partition[0]
 
@@ -240,19 +239,17 @@
             ds = ds_exp_type[experiment_type] = load_ds_latency_dataframe(ds_latency)
 
             if self.simu.include_power_metrics:
                 df_power = df_pow_exp_type[experiment_type] = \
                     load_power_avg_dataframe(power_avg, eps_cfg_parameters, read_start=read_start,
                                              bat_capacity=self.battery_capacity_if_sim_not_run)
 
-            self.set_partition_period(dv0.start, dv0.end, self.simu.add_start_end_scenario)
+            my_periods = self.set_partition_period(dv0.start, dv0.end, self.simu.add_start_end_scenario)
             data_frames = self.get_periods(dv)
 
-            my_periods = [[x, self.my_date_partition[i + 1]] for i, x in enumerate(self.my_date_partition[:-1])]
-
             # Report Data Volume budget summary
             report_basics.report_summary_table_data_avg_periods(n_level, data_frames, proc_report,
                                                                 title='Data Volume budget summary')
 
             proc_report.insert_page_break()
 
             # Report estimated data volume generated per science experiment
@@ -321,20 +318,20 @@
 
             # Instantaneous data rate per instrument
             if self.simu.include_instantaneous_data_rate_per_experiment:
                 self.add_instantaneous_data_rate_per_experiment(
                     n_level, proc_report, dv.df, experiment_type, my_periods)
 
             # Report Data Latency
-            self.add_latency_report_juice(n_level, proc_report, ds, experiment_type, my_periods)
+            self.add_latency_report_juice(n_level, proc_report, ds, dv, experiment_type, my_periods)
 
             # Report Power and Energy (Not for now at least for segmentation) if requested only
             if self.simu.include_power_metrics:
                 self.add_power_metrics_if_requested(n_level, proc_report, df_power, experiment_type,
-                                                my_periods, eps_cfg_parameters)
+                                                    my_periods, eps_cfg_parameters)
 
         proc_report.insert_page_break()
         proc_report.write_head(n_level, "ANNEX")
 
         self.report_resources_info(n_level, proc_report, scenario_path, output_dir)
         if self.eps_cfg_parameters is not None:
             proc_report.insert_page_break()
@@ -460,15 +457,15 @@
 
     def generated_dvs_and_dvs_vs_downlink(self, n_level, proc_report, dfs, experiment_type):
         """
         Generates rst table including Data volume generated in Gbits for all instruments
         - Generate a subsection with a table including the Generated dv for the entire simulation
         - if there are more than on period/partition, add a subsection with on table per partition
 
-        :param n_level: headking level number
+        :param n_level: level number
         :param proc_report:
         :param dfs: dictionary including a subset of dataframes; keys are labels <start>_<end>
         :param experiment_type:
         :return:
         """
 
         dico_total = {}
@@ -499,81 +496,102 @@
 
                 dic_sum_accum = dfs[key].get_total_accum_data_volume()
                 total_downlink = dfs[key].get_total_downlink()
                 self.generated_dv_per_experiment_vs_downlink_capacity(
                     proc_report, dic_sum_accum, experiment_type + '_vs_Downlink', key,
                     total_downlink_capacity=total_downlink, title='Generated DV vs Downlink')
 
-    def add_latency_report_juice(self, n_level, proc_report, ds, experiment_type, my_periods,
+    def add_latency_report_juice(self, n_level, proc_report, ds, dv, experiment_type, my_periods,
                                  objective_summary=''):
         """
         Generate rst table including Data volume generated in Gbits for all instruments
 
+        1) First get DS_latency from any experiment using selective downlink (any _STORE:ACCUM) within data_rate_avg
+        2) set table metrics taking into account 1) replacing the means and max values for selective downlink experiments (if needed)
+        3) create latency plot for experiment not using selective downlink
+        4) create latency plot for experiment using selective downlink
+
         :param n_level: Report header level
         :param proc_report: report object
-        :param ds: ds latency dataframe
+        :param ds: ds_latency dataframe
+        :param dv: data_rate_avg dataframe
         :param experiment_type: experiment type (i.e. instrument, target)
         :param my_periods: curent period [start, end]
         :param objective_summary: text summary
         :return:
         """
 
         if ds.df is None:
 
             logging.info('There is no latency; Latency file empty')
 
         else:
 
-            dfs = self.get_periods(ds, DfDataLatency)
-
             title = 'Data Latency'
             logging.debug(title)
 
             text = """The table bellow provides for each packet store:
                       \n * Latency: The Maximum latency in days
                       \n * Average: The mean value of the latency in days
                       \n * Instrument: instrument name\n\n"""
 
-            sub_phases_header = ['Metric'] + [s.replace('_', ' ') for s in sorted(dfs.keys())] + ['All']
-            metrics = [sub_phases_header]
-            values = [max(dfs[k].get_max_latency().values()) for k in sorted(dfs.keys())]
-            metrics.append(['Maximum latency in days'] + values + [max(values)])
-            values = [round(np.mean(list(dfs[k].get_mean_latency().values())), 2) for k in sorted(dfs.keys())]
-            metrics.append(['Average latency in days'] + values + [round(np.mean(values), 2)])
+            keys = sorted([k for k in ds.df.keys() if 'time' not in k and 'KAB' in k and 'SSMM' in k])
+
+            key_latency_files = [k for k in keys if k.endswith('_DOWNLINK')]
+            key_latency = [k for k in keys if not k.endswith('_DOWNLINK')]
+
+            # 1) Get DS_latency from any experiment using selective downlink
+            key_stores = [k for k in dv.df.keys() if k.endswith('_STORE:Accum')]
+
+            from soa_report.juice.eps_data.file_latency import get_file_latency
+            ds_file_store = {}
+            for k in key_stores:
+                key = k.split('_STORE:Accum')[0]
+                if key not in ds_file_store.keys():
+                    ds_file_store[key] = {}
+
+                ds_file_store[key]['datetime (UTC)'], ds_file_store[key]['latency'], ds_file_store[key]['sizes'] = \
+                    get_file_latency(dv.df, f"{key}_STORE:Accum", f"{key}_DOWNLINK:Accum")
+
+            sub_phases_header = ['Metric'] + [s.split(':')[-1] for s in key_latency] \
+                                + [s.split(' ')[-1] for s in ds_file_store.keys()]
+            metrics = [sub_phases_header,
+                       ['Maximum latency in days'] +
+                       [ds.df[k].max() for k in key_latency] +
+                       [np.max(ds_file_store[k]['latency']) for k in ds_file_store.keys()],
+                       ['Average latency in days'] +
+                       [round(ds.df[k].mean(), 2) for k in key_latency] +
+                       [round(np.mean(ds_file_store[k]['latency']), 2) for k in ds_file_store.keys()]]
 
             if len(metrics[0]) > 4:
                 metrics = np.array(metrics).T.tolist()
 
             proc_report.print_summary_section(n_level, title, objective_summary=text, metrics=metrics, figure=[])
 
-            sub_phases_header = [experiment_type.capitalize(), 'Mean latency [Days]', 'Max latency [Days]']
-            latency_days = [k for k in ds.df.keys() if 'B-LINK' in k]  # and 'Maximum' in k]
-
-            # for k in sorted(dfs.keys()):
-            #     title = 'Sub-period per {} [{}]'.format(experiment_type, k)
-            #     metrics = [sub_phases_header]
-            #     mean_latency = dfs[k].get_mean_latency()
-            #     max_latency = dfs[k].get_max_latency()
-            #     # print mean_latency
-            #     # print max_latency
-            #     for l in mean_latency.keys():
-            #         if 'Maximum' in l:
-            #             to_end = [l, round(mean_latency[l], 2), round(max_latency[l], 2)]
-            #         else:
-            #             metrics.append([l, round(mean_latency[l], 2), round(max_latency[l], 2)])
-            #             # metrics.append([l, round(mean_latency[l], 10), round(max_latency[l], 10)])
-            #
-            #     proc_report.print_summary_section(n_level + 1, title, objective_summary=text, metrics=metrics,
-            #                                       figure=[])
-
-            fig_name = 'data_latency_' + experiment_type
-            plots_utils.create_plot_latency_presentation(ds.df, self.plots_path, option='png',
-                                                         fig_name=fig_name, y_label='Days', my_periods=my_periods)
+            for label in ['KAB_LINK']:
+                fig_name = f'data_latency_{label}_{experiment_type}'
+                plots_utils.create_plot_latency_presentation(ds.df, self.plots_path, option='png',
+                                                             antenna_label=label, fig_name=fig_name,
+                                                             y_label='Days', my_periods=my_periods,
+                                                             selected_keys=key_latency)
+                plot_file_path = os.path.join('plots', os.path.basename(fig_name + '.png'))
+                proc_report.rst_insert_figure(plot_file_path, title='Data Latency', text=objective_summary)
+
+                fig_name = f'data_latency_file_from_ds_{label}_{experiment_type}'
+                plots_utils.create_plot_latency_presentation(ds.df, self.plots_path, option='png',
+                                                             antenna_label=label, fig_name=fig_name,
+                                                             y_label='Days', my_periods=my_periods,
+                                                             selected_keys=key_latency_files)
+
+            fig_name = f'data_files_latency_from_dv_{experiment_type}'
+            plots_utils.create_plot_files_latency(ds_file_store, self.plots_path, option='png',
+                                                  fig_name=fig_name, my_periods=my_periods,
+                                                  y_label='Days')
             plot_file_path = os.path.join('plots', os.path.basename(fig_name + '.png'))
-            proc_report.rst_insert_figure(plot_file_path, title='Data Latency', text=objective_summary)
+            proc_report.rst_insert_figure(plot_file_path, title='Data Files Latency', text=objective_summary)
 
     def add_instantaneous_data_rate_per_experiment(self, n_level, proc_report, df, experiment_type, my_periods):
         """
         Add Data rate Generation per instrument subsection in the report
 
         :param n_level: Report header level
         :param proc_report: report object
@@ -637,15 +655,15 @@
                                                      fig_name=fig_name, my_periods=my_periods, y_label='Gbits')
 
             proc_report.rst_insert_figure(os.path.join('plots', fig_name + '.png'),
                                           title='{} SSMM Packet Store [Gbits]'.format(k.split(':')[0]),
                                           text='')
 
     def generated_overwrite_all_periods(self, n_level, proc_report, dfs, experiment_type, overwrite_periods,
-                                    date_format='%Y-%m-%dT%H:%M:%S'):
+                                        date_format='%Y-%m-%dT%H:%M:%S'):
         """
         Generates rst table including Data volume generated in Gbits for all instruments
 
         - Generate a subsection with a table including the Generated dv for the entire simulation
         - if there are more than on period/partition, add a subsection with on table per partition
 
         :param n_level: Report header level
@@ -1065,15 +1083,15 @@
     """
 
     df_power = PowerAverage(power_avg, eps_cfg_parameters, read_start, bat_capacity)
 
     return df_power
 
 
-def load_ds_latency_dataframe(ds_latency):
+def load_ds_latency_dataframe(ds_latency, ):
     """
     Get ds_latency data frame
     :param ds_latency: data latency file path
     :return: ds: ds_latency dataframe
     """
 
     ds = DsLatency(ds_latency)
```

## soa_report/juice/eps_data/df_data_latency.py

```diff
@@ -114,26 +114,7 @@
     def get_total_latency_accum(self):
         """
         Return the values in Gbit of Total Latency (X-band + K-band) at the end of scenario
         :return: total_Latency:
         """
 
         return self.df['Total_Latency'].sum()
-
-
-# def get_latency_accum(df, antenna_label='HGA'):
-#     """
-#     Build a data frame including eps downlink profiles
-#
-#     :param df: panda data frame including X_band_Downlink,K_band_Downlink and Total_Downlink
-#     :param antenna_label: label use to filter antenna values
-#     :return: dico
-#     """
-#
-#     dico = {'Total_Latency': [0]}
-#     col_label = '{}:Maximum'.format(antenna_label)
-#
-#     for i in range(len(df['datetime (UTC)']) - 1):
-#         ant_total_latency = df[col_label][i + 1] + df[col_label][i + 1]
-#         dico['Total_Latency'].append(ant_total_latency)
-#
-#     return dico
```

## soa_report/juice/eps_data/df_power_avg.py

```diff
@@ -15,15 +15,15 @@
     def __init__(self, df, start_date_time, end_date_time):
 
         self.df = self.get_data_frame_period(df, start_date_time, end_date_time)
 
         self.__get_eps_output_report_time_step__()
 
         self.start = self.df['datetime (UTC)'][0]
-        self.end = self.df['datetime (UTC)'].iat[-1]  # iat faster than iloc if you only whant value
+        self.end = self.df['datetime (UTC)'].iat[-1]  # iat faster than iloc if you only want value
 
     def __get_eps_output_report_time_step__(self):
         """
         Calculates the eps output report time step in seconds.
         """
 
         self.report_time_step = (self.df['datetime (UTC)'][1]
```

## soa_report/juice/eps_data/ds_latency.py

```diff
@@ -15,41 +15,28 @@
 from esac_juice_pyutils.commons import tds
 from soa_report.juice.eps_data.epsoutput import EpsOutput
 from soa_report.juice.eps_data.df_data_latency import DfDataLatency
 
 
 class DsLatency(DfDataLatency):
     """
-    This class allows to handle (read, write) DS_latency file produced by bepiColombo SOA Tool
+    This class allows to handle (read, write) DS_latency file
     """
 
-    def __init__(self, input_file_path, read_start=None, experiment_to_ignore=[]):
+    def __init__(self, input_file_path, read_start=None, experiment_to_ignore=[], read_stop=None):
 
-        # self.df = self.get_data_frame_extended(input_file_path, experiment_to_ignore=[])
-        self.df = self.get_data_frame(input_file_path, read_start, experiment_to_ignore)
+        self.df = self.get_data_frame(input_file_path,
+                                      read_start=read_start,
+                                      experiment_to_ignore=experiment_to_ignore,
+                                      read_stop=read_stop)
 
         if self.df is not None:
-
-            self.__get_eps_output_report_time_step__()
-
             self.start = pandas.to_datetime(self.df['datetime (UTC)'][0])
             self.end = pandas.to_datetime(self.df['datetime (UTC)'].iloc[-1])
 
-    def __get_eps_output_report_time_step__(self):
-        """
-        Calculates the eps output report time step in seconds.
-        """
-
-        self.report_time_step = (self.df['datetime (UTC)'][1]
-                                 - self.df['datetime (UTC)'][0]).total_seconds()
-
-        self.Kbits_sec_to_Gbits_dt = self.report_time_step / 1000 / 1000
-
-        logging.debug('eps output report_time_step = {} seconds'.format(self.report_time_step))
-
     def read(self, input_file_path):
         """
         Read event file
 
         :param input_file_path: path of the input data_rate_avg.out file
         :return EpsOutput Object
         """
@@ -87,21 +74,22 @@
                             list_of_values.append(float(ele))
                         else:
                             list_of_values.append(ele)
                     data_out.data_value.append(list_of_values)
 
         return data_out
 
-    def get_data_frame(self, input_file_path, read_start=None, experiment_to_ignore=[]):
+    def get_data_frame(self, input_file_path, read_start=None, read_stop=None, experiment_to_ignore=[]):
         """
         Return eps data_latency as pandas frames
 
         :param input_file_path:
         :param read_start: Allow to specify the first time to read
         :param experiment_to_ignore: list of experiment to ignore
+        :param read_stop: Allow to specify the final time to read
         :return: df: panda data frame
         """
 
         import pandas as pd
 
         data_out = self.read(input_file_path)
 
@@ -110,33 +98,32 @@
         for j in range(len(data_out.data_title[0])):
             df_keys.append(data_out.data_title[0][j] + ':' + data_out.data_title[1][j])
 
         # Fill data frame dictionary
         df_dictionary = {}
         for i in range(len(df_keys)):
             df_dictionary[df_keys[i]] = []
-            # print df_keys[i]
+
             for line in data_out.data_value:
+
                 # Remove undefined values +, - are set to 'NaN
                 if line[i] == '+' or line[i] == '-':
                     line[i] = np.nan
                 df_dictionary[df_keys[i]].append(line[i])
 
         ref_date = data_out.start_utc
         logging.debug('reference start time = {}'.format(ref_date))
 
         if not df_dictionary:
-
             logging.info('There is no latency; Latency file empty: {}'.format(input_file_path))
             return None
 
         if ':Elapsed time' in df_dictionary.keys():
 
             if len(df_dictionary['Elapsed time:ddd_hh:mm:ss']) == 0:
-
                 logging.info('There is no latency; Latency file empty: {}'.format(input_file_path))
                 return None
 
             df_dictionary['Elapsed time'] = df_dictionary.pop('Elapsed time:ddd_hh:mm:ss')
 
             # Check if relative first start time for latency is not 000_00:00:00
             # and in affirmative case insert this corresponding values
@@ -197,38 +184,45 @@
             df_dictionary = {k: v for k, v in df_dictionary.items() if not k.startswith(f"{experiment}:")}
 
         df = pd.DataFrame(df_dictionary)
 
         if read_start:
             df = df[df['datetime (UTC)'] >= read_start]
             df.reset_index(drop=True, inplace=True)
+        if read_stop:
+            df = df[df['datetime (UTC)'] <= read_stop]
+            df.reset_index(drop=True, inplace=True)
 
         return df
 
-    def get_data_frame_extended(self, input_file_path):
+    def get_data_frame_extended(self, input_file_path, read_start=None, read_stop=None, experiment_to_ignore=[]):
         """
         Return extended eps data_latency as pandas frames
         :param input_file_path:
+        :param read_start: Allow to specify the first time to read
+        :param read_stop: Allow to specify the final time to read
+        :param experiment_to_ignore: list of experiment to ignore
         :return: df: panda data frame
         """
 
-        df_ds_latency = self.get_data_frame(input_file_path)
+        df = self.get_data_frame(input_file_path, read_start=read_start, read_stop=read_stop,
+                                 experiment_to_ignore=experiment_to_ignore)
 
-        if df_ds_latency is None:
+        if df is None:
             return None
 
-        dico = get_latency_accum(df_ds_latency)
-        # print '\n', dico.keys()
+        dico = get_latency_accum(df)
+
         for dp in dico.keys():
-            df_ds_latency[dp] = dico[dp]
+            df[dp] = dico[dp]
 
-        return df_ds_latency
+        return df
 
 
-def get_latency_accum(df, antenna_label='HGA'):
+def get_latency_accum(df, antenna_label='KAB_LINK'):
     """
     Build a data frame including eps downlink profiles
 
     :param df: panda data frame including X_band_Downlink,K_band_Downlink and Total_Downlink
     :param antenna_label: label use to filter antenna values
     :return: dico
     """
```

## soa_report/juice/eps_data/power_avg.py

```diff
@@ -27,15 +27,17 @@
     This class allows to handle (read, write) power_avg file produced by bepiColombo SOA Tool
     """
 
     def __init__(self, input_file_path, eps_cfg_parameters=None, read_start=None, bat_capacity=None):
 
         self.battery_capacity = None
 
-        self.df = self.get_data_frame_extended(input_file_path, eps_cfg_parameters, read_start, bat_capacity)
+        self.df = self.get_data_frame_extended(input_file_path,
+                                               read_start=read_start,
+                                               bat_capacity=bat_capacity)
 
         if self.df is not None:
             self.__get_eps_output_report_time_step__()
 
             self.start = pandas.to_datetime(self.df['datetime (UTC)'][0])
             self.end = pandas.to_datetime(self.df['datetime (UTC)'].iloc[-1])
 
@@ -68,15 +70,14 @@
         if not os.path.exists(input_file_path):
             logging.error('{} file {} does not exist'.format('Juice SOA power average', input_file_path))
 
         data_out = EpsOutput(os.path.basename(input_file_path))
 
         f = open(input_file_path, 'r')
         for line in f.read().splitlines():
-            # event_mask = re.match(r'^([0-9T\-:]{19})\s*([0-9\.]{6,20})',line,re.M|re.I)
 
             if line.startswith('#'):  # reading file header
                 line = line[1:].lstrip()
                 metadata_header = line.split(':')[0]
                 if ':' in line:
                     header_value = line.split(':')[1]
                     if 'Ref_date:' in line:
@@ -120,15 +121,15 @@
         df_keys = []
         for j in range(len(data_out.data_title[0])):
             df_keys.append(data_out.data_title[0][j]
                            + ':' + data_out.data_title[1][j].replace('(', '').replace(')', ''))
         df_dictionary = {}
         for i in range(len(df_keys)):
             df_dictionary[df_keys[i]] = []
-            # print df_keys[i]
+
             for line in data_out.data_value:
                 df_dictionary[df_keys[i]].append(line[i])
 
         ref_date = data_out.start_utc
         logging.debug('reference start time = {}'.format(ref_date))
 
         if 'Elapsed time:ddd_hh:mm:ss' in df_dictionary.keys():
@@ -175,70 +176,47 @@
 
             logging.error('Please check eps file files format: {}'.format(input_file_path))
             sys.exit()
 
         df = pd.DataFrame(df_dictionary)
         return df
 
-    def get_data_frame_extended(self, input_file_path, eps_cfg_parameters=None, read_start=None, bat_capacity=None):
+    def get_data_frame_extended(self, input_file_path, read_start=None, bat_capacity=None, read_stop=None):
         """
         Return extended eps data_latency as pandas frames
 
         :param input_file_path:
         :param read_start: Allow to specify the first time to read
+        :param read_stop: Allow to specify the final time to read
+        :param bat_capacity: number of Watts
         :return: df: panda data frame
         """
 
         df = self.get_data_frame(input_file_path)
-        n = len(df)
 
         if df is None:
             return None
 
-        if eps_cfg_parameters:
-
-            if eps_cfg_parameters['POWER_MODEL']:
-
-                if eps_cfg_parameters['POWER_MODEL']['BATTERY_CAPACITY']:
-
-                    bat_cap = eps_cfg_parameters['POWER_MODEL']['BATTERY_CAPACITY'][0][0]
-                    # bat_cap = eps_cfg_parameters['POWER_MODEL']['BATTERY_CAPACITY']
-
-                    for key in df.keys():
-
-                        if 'Batt. DoD:%' in key:
-
-                            # df['Batt.:Watts'] = (100 - df['Batt. DoD:%']) / 100 * bat_cap
-                            df['Batt.:%'] = 100 - df['Batt. DoD:%']
-                            # df['Batt. DoD:Watts'] = df['Batt. DoD:%'] / 100 * bat_cap
-                            self.battery_capacity = bat_cap
-        elif bat_capacity:
+        if bat_capacity:
 
             bat_cap = bat_capacity
 
-            # My understanding is Batt. DoD:% means
-            # - Batt . DoD:% status (like SSMM status) that sum of Power discharge - Sum Power charge
-            # - Batt DoD % power discharge (like data/rate) would be Sum of positive increment of DoD:% are equivalent to discharge
-            # - Batt DoD Watts =
-
             if 'Batt. DoD:%' in list(df.keys()):
 
-                batt_status = df['Batt. DoD:%']
-                power_discharges = np.array([0.0] * n)
-                power_charges = np.array([0.0] * n)
-
-                # df['Batt.:Watts'] = (100 - df['Batt. DoD:%']) / 100 * bat_cap
                 df['Batt.:%'] = 100 - df['Batt. DoD:%']
-                # df['Batt. DoD:Watts'] = df['Batt. DoD:%'] / 100 * bat_cap
+
                 self.battery_capacity = bat_cap
 
         # Platform is PLATFORM in segmentation and JUICE in scenario
         if 'JUICE:Watts' in list(df.keys()):
             df = get_extra_df_scenarios(df, self.battery_capacity, df['Batt.:%'])
         else:
             df = get_extra_df_segmentation(df)
 
         if read_start:
             df = df[df['datetime (UTC)'] >= read_start]
             df.reset_index(drop=True, inplace=True)
+        if read_stop:
+            df = df[df['datetime (UTC)'] <= read_stop]
+            df.reset_index(drop=True, inplace=True)
 
         return df
```

## soa_report/juice/report/soa_report_basics.py

```diff
@@ -105,32 +105,46 @@
 
         if len(self.my_date_partition) == 0:
             self.my_date_partition.append(scenario_start)
             self.my_date_partition.append(scenario_end)
             logging.warning('No date partition provided; We will used the total window (start, end) = ({}, {})'.format(
                 scenario_start, scenario_end))
 
+            my_periods = [[scenario_start, scenario_end]]
+
         else:
 
-            for t in self.my_date_partition:
+            my_periods = [[x, self.my_date_partition[i + 1]] for i, x in enumerate(self.my_date_partition[:-1])]
+
+            for p in my_periods:
 
-                if t < scenario_start or t > scenario_end:
-                    logging.warning('{} time subset is out of scenario period [{}, {}]'.format(
-                        t, scenario_start, scenario_end))
+                [e, s] = p
+
+                if e < scenario_start or s > scenario_end:
+                    logging.error(f'[{datetime.datetime.strftime(s, "%Y-%m-%dT%H:%M:%S")}, '
+                                  f'{datetime.datetime.strftime(e, "%Y-%m-%dT%H:%M:%S")}], '
+                                  f'time subset is out of scenario period '
+                                  f'[{scenario_start}, {scenario_end}]; removed')
+                    logging.error('Please review the request periods')
+                    sys.exit()
 
         my_date_partition_str = []
         for period in self.my_date_partition:
             my_date_partition_str.append(datetime.datetime.strftime(period, '%Y-%m-%dT%H:%M:%S.%f'))
 
         logging.info('my_date_partition_0 = {}'.format(my_date_partition_str))
 
+        return my_periods
+
     def get_periods(self, dv, df_type=DfDataRateAverage, my_date_partition=None):
         """
         Defines data_frames subset
 
+        :param my_date_partition:
+        :param df_type:
         :param dv: pandas dataframe for the whole scenario
         :return: list of pandas dataframe corresponding to a given subset if periods
         """
 
         if my_date_partition is None:
             my_date_partition = self.my_date_partition
```

## soa_report/templates/scenario_reporter.json

### Pretty-printed

 * *Similarity: 0.9424603174603176%*

 * *Differences: {"'request'": "{'root_path': './08Sep2022-140545/eps_output', delete: ['scenario', "*

 * *              "'experiment_types']}",*

 * * "'request_parameter_descriptions'": "{'root_path': 'path of directory eps_output directory', "*

 * *                                     "delete: ['scenario', 'experiment_types']}"}*

```diff
@@ -1,41 +1,35 @@
 {
     "config_for_command_line_tool": "scenario_reporter",
     "request": {
         "add_start_end_scenario": 0,
         "battery_capacity_if_sim_not_run": 4946,
-        "experiment_types": [
-            "instrument"
-        ],
         "include_downlink_status_per_instruments": 1,
         "include_instantaneous_data_rate_per_experiment": 1,
         "include_power_metrics": 1,
         "include_power_metrics_partition_details": 1,
         "include_ssmm_status_per_instruments": 1,
         "output_dir": "output",
         "partition_times": [
             "2031-08-09T22:00:00",
             "2031-08-10T00:00:00"
         ],
         "report_file_name": "report_08Sep2022_140545",
         "report_title": "Summary Report 08Sep2022-140545",
-        "root_path": "./",
-        "scenario": "08Sep2022-140545"
+        "root_path": "./08Sep2022-140545/eps_output"
     },
     "request_parameter_descriptions": {
         "add_start_end_scenario": "This flag must be set to 0/1 to allow/avoid the inclusion of periods from/util start/end eps_package window",
         "battery_capacity_if_sim_not_run": "Allows to set the battery capacity in case OSVE sim not run",
-        "experiment_types": "list of experiment type [instrument]; only instrument is supported",
         "include_downlink_status_per_instruments": "[Optional] Flag to enforce/avoid inclusion of donwlink status per experiment; default True/0",
         "include_instantaneous_data_rate_per_experiment": "Flag to enforce/avoid inclusion instantaneous data rate per experiment metrics; default is 1/true",
         "include_power_metrics": "Flag to enforce/avoid inclusion of power metrics; default is 1/true",
         "include_power_metrics_partition_details": "[Optional] Flag to enforce/avoid inclusion of power metric partition; default is 0/false to reduce report size; take into account only if include_power_metrics=1/true",
         "include_ssmm_status_per_instruments": "[Optional] Flag to enforce/avoid inclusion of SSMM status per experiment; default True/0",
         "output_dir": "path of output dir (which must exist); by default soa_report_output within eps_package directory",
         "overwrite_periods": "This allow to overwrite sub-periods distributing the corresponding DV in per experiment in % (only for target experiment types)",
         "partition_times": "list of time requested within (time format: YYYY-mm-ddTHH:MM:SS)",
         "report_file_name": "[Optional] Report file Name; default is 'report'",
         "report_title": "Report title",
-        "root_path": "path of directory where eps_package is located ",
-        "scenario": "Name of the eps_package (directory)"
+        "root_path": "path of directory eps_output directory"
     }
 }
```

## test/test_segmentation_report_e2e_not_osve.py

```diff
@@ -6,16 +6,14 @@
 This Module allows run the Segmentation reporter for several cases
 
 All the data are available on test_data_set directory
 
 1) Generate segmentation report from ref test_case TDS/crema_5_0
 The result is compared against a previous run (here the rst report)
 
-2) Generate segmentation report from ref test_case TDS/overwrite_with_2_experiments
-The result is compared against a previous run (here the rst report)
 
 """
 
 import os
 import logging
 import unittest
 
@@ -37,21 +35,23 @@
         Here we do not run osve but only check the reporting part.
         This test is used for CI/DL purpose
         """
 
         test_data_set = '../TDS/crema_5_0'
 
         here = os.getcwd()
-        print(f'here:{here}')
+        print(f'here: {here}')
         os.chdir(test_data_set)
         working_dir = os.getcwd()
 
         config_file = 'Reporter_Config_e2e_test.json'
 
         cfg = load_to_dic(config_file)
+        cfg['request']['run_simu'] = 0  # no run
+        cfg['env_var'] = {}  # Environment var need to be set to local host for osve run, not needed!
         output_ref = cfg['request']["output_dir"]
 
         report_name = 'report'
         if "report_file_name" in cfg['request'].keys():
             report_name = cfg['request']['report_file_name']
 
         report_name_tmp = report_name + '_tmp'
@@ -66,51 +66,7 @@
         self.assertListEqual(tmp_values, tmp_ref)
 
         for f_tmp in os.listdir():
             if report_name_tmp in f_tmp:
                 os.remove(f_tmp)
 
         os.chdir(here)
-
-    def test_segmentation_report_overwrite_with_2_experiments(self,):
-        """
-        Test (case e) check Segmentation report generated as expected
-        this exercise the overwrite period functionality with 2 experiments TARGETS, and EXPERIMENT_TYPE
-
-        Here we do not run osve but only check the reporting part.
-        This test is used for CI/DL purpose
-        """
-
-        test_data_set = '../TDS/overwrite_with_2_experiments'
-
-        here = os.getcwd()
-        print(here)
-        os.chdir(test_data_set)
-        working_dir = os.getcwd()
-
-        config_file = 'config_json_2_claudio.json'
-
-        cfg = load_to_dic(config_file)
-        output_ref = cfg['request']["output_dir"] = 'output_generate_segmentation_for_e2e_test'
-        cfg['request']['run_simu'] = 0
-
-        report_name = 'report'
-        if "report_file_name" in cfg['request'].keys():
-            report_name = cfg['request']['report_file_name']
-
-        report_name_tmp = report_name + '_tmp'
-        cfg['request']['report_file_name'] = report_name_tmp
-        cfg['request']['run_simu'] = False
-
-        segmentation_reporter.run(config_file, cfg, working_dir)
-
-        tmp_values = list(open(os.path.join(output_ref, f'{report_name_tmp}.rst'), 'r'))
-        tmp_ref = list(open(os.path.join(output_ref, f'{report_name}.rst'), 'r'))
-
-        self.assertListEqual(tmp_values, tmp_ref)
-
-        for f_tmp in os.listdir():
-            if report_name_tmp in f_tmp:
-                os.remove(f_tmp)
-
-        os.chdir(here)
-
```

## Comparing `soa_report-1.2.0.dist-info/RECORD` & `soa_report-1.2.5.dist-info/RECORD`

 * *Files 16% similar despite different names*

```diff
@@ -1,48 +1,57 @@
 old_modules/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 old_modules/soa_run_eps.py,sha256=HD5A1yjQbR0xyXrMxlFYFgaSGrXD72AJXtCpvCw3HcE,3343
 old_modules/test_soa_report.py,sha256=Rh7V9oDX_-2EHoDClNGlkeUw-cP5DIuP7n6U4unxoOQ,1201
 old_modules/test_soa_report_filter.py,sha256=uOetxOeaboVyYbvl5oDuN2NBcdQkdTC9XGTgGW35KqM,2051
 scripts/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
-soa_report/__init__.py,sha256=-XvoSdwL-0go8ZX6VN74e-D6dwG0z-0p7vL5MO0Sz5s,18
-soa_report/scenario_reporter_cmd.py,sha256=0mZSf4lbhlNHodhbo6KxI-6KYaMlm29X3GdVovX1MHI,5914
+soa_report/__init__.py,sha256=sdJx4-9BZbQ5298uEp1eU9RE6AXslda5v-aSs-OjEPE,18
+soa_report/scenario_reporter_cmd.py,sha256=CzSVssLBT2J7dx5j90Z6zH07bpQ7CJqRVWbHOdOSL0Q,5908
 soa_report/segmentation_reporter_cmd.py,sha256=H6awmsCnB7lmhAcxVb3K-qvdb2K5cCnp8Iau4EHN6Oo,5986
 soa_report/commons/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 soa_report/commons/env_variables.py,sha256=TpLD0fXlfYwsljg9khfVk0362qpnJZkVt-E7lns6YKs,1840
 soa_report/commons/matplotlib_utils.py,sha256=d3-cfuZpOlq3Xt3oEDGHhhckXwUo-D2EC2ZSAiwqGy8,3883
 soa_report/commons/my_log.py,sha256=YBjkZh_rDC9AVuD6Lrk0CDlGc3gYK4MsBO4Vb77CFd0,1023
-soa_report/commons/plots_utils.py,sha256=mwdzIdbmsh1BNrgZMQWPeXvjkWvKeQtH9RdBHd4lFZM,18853
+soa_report/commons/plots_utils.py,sha256=dpG66NqL_EemDCPe9L1pWw2-qqMYdakWDNkGDb-VU8E,20419
 soa_report/commons/power_pwr.py,sha256=5pe9wT0leTIJAUuqvdAP9b6ruHRniqiJj3k8dtJwiaM,2390
 soa_report/commons/rst_report.py,sha256=XIryINT8Nd_H_yPspapCBVCUAaocrciDqqXR5PQAMDc,7623
 soa_report/commons/spice_kernel_utils.py,sha256=15aAU-adSsrg9ccQ2AgmCj6xirGd4baPor51mgKwB2I,663
 soa_report/juice/__init__.py,sha256=gA5Ljo1XFoBK_Sc7nH7MHyfwRoI5ojp3PiOBaAhkkI8,1397
-soa_report/juice/scenario_reporter.py,sha256=_Eeh8MttzGWwoq3_ihemkOH5saP8WFKgdV9cSWfO8B4,46949
-soa_report/juice/segmentation_reporter.py,sha256=xcJegf0OSdwcQmu19-3X9I0vqbzEpqMyQbW-pabPpdw,53057
+soa_report/juice/scenario_reporter.py,sha256=JNSDHgwd03SP0-bDocX9Ktm1edyVLj8xiw0Zo2KKq-U,40326
+soa_report/juice/segmentation_reporter.py,sha256=al0sgMp4odLzbuvegsbTYhWNsYyU1U_muI2H5C-t0dw,54475
 soa_report/juice/eps_data/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
+soa_report/juice/eps_data/brf.py,sha256=2p0rBSCtcXXZchiJIijdpS23Oq6qmN8GsJF4QTcSjmc,6469
 soa_report/juice/eps_data/data_rate_avg.py,sha256=kh22c25HubMNzxX3dZgO1iETzaxZK-XhzBt2hy3V4E4,8277
-soa_report/juice/eps_data/df_data_latency.py,sha256=CNbTMugTQ2F3YIScQ7im6MUbXmy33lyhAU0OKrCR5vw,4510
+soa_report/juice/eps_data/df_brf.py,sha256=rm45OcBWtM-UMcUliWvORvVhyBT0KEcm7jZRYL3mt7s,1799
+soa_report/juice/eps_data/df_data_latency.py,sha256=8ingDgMVzwu5Xc_ZWQpdSiEKmh7Wbq3auwINFXh-8wM,3903
 soa_report/juice/eps_data/df_data_rate_avg.py,sha256=Lj6tNTpQEFlPkj_t4JXrYZuSo_xegM6YyyKJKQOtulc,6453
-soa_report/juice/eps_data/df_power_avg.py,sha256=fWVZtgiBCb58YrgJ0tOCgiL0jNmcUrCIxthmSBlXxSc,1803
-soa_report/juice/eps_data/ds_latency.py,sha256=2ne3ROthsgm7HnZXGHbse6HX9z6kyiNXmu1NyDxToJk,8830
+soa_report/juice/eps_data/df_power_avg.py,sha256=xFcSGVCfPrPu4QpJuWaKMtqpfhPTSoYlX_Pfi-GQhtk,1802
+soa_report/juice/eps_data/ds_latency.py,sha256=gX5YhdlaM0XJrIHYFKkWotGR3dy8muPB2fstNYSfr0Y,8852
+soa_report/juice/eps_data/ds_transfers.py,sha256=4YRguvPUnDuMH2Vd1VIKZlozO2Mm9xQY91KWD5tVE18,7602
 soa_report/juice/eps_data/epsoutput.py,sha256=2ORezN3WaQiPQLbTz8fZgzvRwl5mSq88iwKlUSQP18g,431
-soa_report/juice/eps_data/power_avg.py,sha256=r3txi1WrAnmFCHQBeocKA9VOOFJCtWUhTVfvpPCB8mY,8802
+soa_report/juice/eps_data/file_latency.py,sha256=pIfwulEFT0mFpUh4skgUa2QzFGSjMgo9iMazLMch1_U,2589
+soa_report/juice/eps_data/power_avg.py,sha256=69e9bmAo0vrUPT4iqyjlqLJ9XRr_cJWIRgaBcnCKHhQ,7622
 soa_report/juice/report/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
-soa_report/juice/report/soa_report_basics.py,sha256=Wpbm105vBI92ysX6M5lZoWHvQSOBjo7hiY-sVRFVOyg,20763
+soa_report/juice/report/soa_report_basics.py,sha256=rHjG-wgVx6vtIVDFCtVCCRK830FlhKyVYugTgFPn9Yw,21329
 soa_report/juice/report/soa_report_summary.py,sha256=YFIaqEOpwOTWy4JneBMDlxI9YeLaN5rSab5Q_h9E998,3851
 soa_report/juice/segmentation/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 soa_report/juice/segmentation/power_metrics.py,sha256=HTDcBgR0p8fnYAti2FER1XzVwu2RN5gI3rAkReCESco,9035
 soa_report/juice/soa/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 soa_report/juice/soa/power_metrics.py,sha256=7vSgg0rIfG76EzFhI8Cjwm9hPvUoHwOYAPPqcj6JuPM,8997
+soa_report/juice/soa/scenario_compare.py,sha256=7oKFnHx3oL8ttCRwY8kyIxRwa5I6UYwsO6NN28_Rd0Q,15117
+soa_report/juice/soa/soa_report_basics.py,sha256=ZjThsrL57VkUJ6m_zrs-3OcuSZLcAicmDf-ZGGusgQg,19652
 soa_report/juice/templates/custom-reference.docx,sha256=GkMl7zGrSVn2xnlWJIsL3ETpGpjI7x304K_-sTLA8e8,15613
 soa_report/juice/templates/default_rst2pdf.style,sha256=tx6rkhphrlWTMUvqzE8J45ggo6qF8QeJIQMY3PMGlew,13276
 soa_report/templates/Segmentation_Reporter_Configuration_file.json,sha256=_wNqeGMPYa2tsI9KIFEquRKWKKJDHktHEd0NV1UGFEs,5704
 soa_report/templates/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
-soa_report/templates/scenario_reporter.json,sha256=OeLdn15V5nSNh89SU-mI8kIx6sMvH3K1uFUY_SXnwpI,2554
+soa_report/templates/scenario_reporter.json,sha256=KSJp4f-6orsxS7kDZdZPaVobnUcoxsm0lfhoETgOZnA,2331
+soa_report/utest/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
+soa_report/utest/utest_epsdata_brf_handling.py,sha256=scozxmta1k0TJVHwoPXKMbaSbO1llwhQrec4_AEDB9k,1279
 test/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 test/test_scenario_report_e2e.py,sha256=DFDrjPO19VqiCwwhUk7ouuoMaOeeHaHIaHL8945hDCw,1732
 test/test_segmentation_report_e2e.py,sha256=m8vSQ9F-sC9uRTnJpm29gezuTLoHpoFD4T2du-dgttI,1775
-test/test_segmentation_report_e2e_not_osve.py,sha256=rdUI7HceMzx-Kri6A8nkqJcf9YR3EzZxTk0uqj7iokQ,3577
-soa_report-1.2.0.dist-info/METADATA,sha256=eTVp0yMbA5MdT7jzFcU4HDyGjG6NslZs8BbZX-xctUk,426
-soa_report-1.2.0.dist-info/WHEEL,sha256=GJ7t_kWBFywbagK5eo9IoUwLW6oyOeTKmQ-9iHFVNxQ,92
-soa_report-1.2.0.dist-info/entry_points.txt,sha256=sZ-5oqjYM4E7xZzBh3yiRYcIF_SyrdDpvWJp3ShRv1A,142
-soa_report-1.2.0.dist-info/top_level.txt,sha256=685eAaVwl4LSXeAxzXXodt0TQ9jJLFwF3-Aa2h6v1cw,36
-soa_report-1.2.0.dist-info/RECORD,,
+test/test_segmentation_report_e2e_not_osve.py,sha256=1lW6zfsJ4DHK4bCLGqpGwdctNhn3uzQwzT-EPi3z2do,2066
+test/test_segmentation_report_e2e_overwrite.py,sha256=b0foloFNO4JXyVeBX6S3exCnFZ0zIfDMlVzRLZWJj-o,2314
+soa_report-1.2.5.dist-info/METADATA,sha256=nSSlGfltc-UsT8OdmA4sASC5A-VeDrK1MYNnthTVBsQ,426
+soa_report-1.2.5.dist-info/WHEEL,sha256=GJ7t_kWBFywbagK5eo9IoUwLW6oyOeTKmQ-9iHFVNxQ,92
+soa_report-1.2.5.dist-info/entry_points.txt,sha256=sZ-5oqjYM4E7xZzBh3yiRYcIF_SyrdDpvWJp3ShRv1A,142
+soa_report-1.2.5.dist-info/top_level.txt,sha256=685eAaVwl4LSXeAxzXXodt0TQ9jJLFwF3-Aa2h6v1cw,36
+soa_report-1.2.5.dist-info/RECORD,,
```

