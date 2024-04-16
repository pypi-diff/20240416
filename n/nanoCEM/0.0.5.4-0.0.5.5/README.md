# Comparing `tmp/nanoCEM-0.0.5.4.tar.gz` & `tmp/nanoCEM-0.0.5.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/nanoCEM-0.0.5.4.tar", last modified: Wed Mar  6 04:58:25 2024, max compression
+gzip compressed data, was "dist/nanoCEM-0.0.5.5.tar", last modified: Tue Apr 16 07:30:24 2024, max compression
```

## Comparing `nanoCEM-0.0.5.4.tar` & `nanoCEM-0.0.5.5.tar`

### file list

```diff
@@ -1,36 +1,37 @@
-drwxrwxr-x   0 zhguo     (1000) zhguo     (1000)        0 2024-03-06 04:58:25.716647 nanoCEM-0.0.5.4/
--rw-rw-r--   0 zhguo     (1000) zhguo     (1000)     1087 2023-05-31 12:16:43.000000 nanoCEM-0.0.5.4/LICENSE
--rw-rw-r--   0 zhguo     (1000) zhguo     (1000)     2464 2024-03-06 04:58:25.716647 nanoCEM-0.0.5.4/PKG-INFO
--rw-rw-r--   0 zhguo     (1000) zhguo     (1000)     1838 2024-03-06 04:56:58.000000 nanoCEM-0.0.5.4/README.md
-drwxrwxr-x   0 zhguo     (1000) zhguo     (1000)        0 2024-03-06 04:58:25.716647 nanoCEM-0.0.5.4/nanoCEM/
--rw-rw-r--   0 zhguo     (1000) zhguo     (1000)    15015 2024-03-06 04:32:24.000000 nanoCEM-0.0.5.4/nanoCEM/CE_magnifier_test.py
--rw-rw-r--   0 zhguo     (1000) zhguo     (1000)     5416 2023-12-21 04:37:40.000000 nanoCEM-0.0.5.4/nanoCEM/NEW_TRAINER.py
--rw-rw-r--   0 zhguo     (1000) zhguo     (1000)       56 2023-06-14 11:15:11.000000 nanoCEM-0.0.5.4/nanoCEM/__init__.py
--rw-rw-r--   0 zhguo     (1000) zhguo     (1000)     4547 2023-12-10 10:36:58.000000 nanoCEM-0.0.5.4/nanoCEM/alignment_feature_camera.py
--rw-rw-r--   0 zhguo     (1000) zhguo     (1000)     3941 2024-03-05 05:12:42.000000 nanoCEM-0.0.5.4/nanoCEM/alignment_magnifier
--rw-rw-r--   0 zhguo     (1000) zhguo     (1000)    14541 2024-03-05 04:48:45.000000 nanoCEM-0.0.5.4/nanoCEM/cem_utils.py
--rwxrwxr-x   0 zhguo     (1000) zhguo     (1000)    10832 2024-03-06 04:39:12.000000 nanoCEM-0.0.5.4/nanoCEM/current_events_magnifier
--rw-rw-r--   0 zhguo     (1000) zhguo     (1000)     5903 2024-03-04 13:42:45.000000 nanoCEM-0.0.5.4/nanoCEM/de_novo.py
--rw-rw-r--   0 zhguo     (1000) zhguo     (1000)     3137 2023-12-15 14:01:45.000000 nanoCEM-0.0.5.4/nanoCEM/density_2d.py
--rw-rw-r--   0 zhguo     (1000) zhguo     (1000)     4083 2024-02-22 02:44:17.000000 nanoCEM-0.0.5.4/nanoCEM/extract_sub_fast5_from_bam
--rw-rw-r--   0 zhguo     (1000) zhguo     (1000)     1868 2023-07-24 04:48:56.000000 nanoCEM-0.0.5.4/nanoCEM/extract_sub_fastq_from_bam
-drwxrwxr-x   0 zhguo     (1000) zhguo     (1000)        0 2024-03-06 04:58:25.716647 nanoCEM-0.0.5.4/nanoCEM/f5c_result_rna/
--rw-rw-r--   0 zhguo     (1000) zhguo     (1000)        0 2024-01-29 04:01:24.000000 nanoCEM-0.0.5.4/nanoCEM/f5c_result_rna/__init__.py
--rw-rw-r--   0 zhguo     (1000) zhguo     (1000)      318 2024-01-29 04:02:07.000000 nanoCEM-0.0.5.4/nanoCEM/f5c_result_rna/test.py
--rw-rw-r--   0 zhguo     (1000) zhguo     (1000)     2160 2024-03-04 13:42:45.000000 nanoCEM-0.0.5.4/nanoCEM/kmer_test.py
--rw-rw-r--   0 zhguo     (1000) zhguo     (1000)     1988 2024-02-23 07:56:30.000000 nanoCEM-0.0.5.4/nanoCEM/kmer_test_pr.py
--rw-rw-r--   0 zhguo     (1000) zhguo     (1000)     3600 2024-03-04 13:42:45.000000 nanoCEM-0.0.5.4/nanoCEM/machine_learning_trainer.py
--rw-rw-r--   0 zhguo     (1000) zhguo     (1000)     4427 2024-02-02 06:02:13.000000 nanoCEM-0.0.5.4/nanoCEM/normalization.py
--rw-rw-r--   0 zhguo     (1000) zhguo     (1000)    11200 2024-02-23 10:21:22.000000 nanoCEM-0.0.5.4/nanoCEM/plot.py
--rw-rw-r--   0 zhguo     (1000) zhguo     (1000)    10455 2024-02-23 09:17:31.000000 nanoCEM-0.0.5.4/nanoCEM/read_f5c_eventalign.py
--rw-rw-r--   0 zhguo     (1000) zhguo     (1000)     6683 2024-02-28 09:35:51.000000 nanoCEM-0.0.5.4/nanoCEM/read_f5c_resquiggle.py
--rw-rw-r--   0 zhguo     (1000) zhguo     (1000)     6867 2024-02-26 09:56:01.000000 nanoCEM-0.0.5.4/nanoCEM/read_move_table.py
--rw-rw-r--   0 zhguo     (1000) zhguo     (1000)    13342 2024-02-26 08:39:30.000000 nanoCEM-0.0.5.4/nanoCEM/read_tombo_resquiggle.py
-drwxrwxr-x   0 zhguo     (1000) zhguo     (1000)        0 2024-03-06 04:58:25.716647 nanoCEM-0.0.5.4/nanoCEM.egg-info/
--rw-rw-r--   0 zhguo     (1000) zhguo     (1000)     2464 2024-03-06 04:58:25.000000 nanoCEM-0.0.5.4/nanoCEM.egg-info/PKG-INFO
--rw-rw-r--   0 zhguo     (1000) zhguo     (1000)      791 2024-03-06 04:58:25.000000 nanoCEM-0.0.5.4/nanoCEM.egg-info/SOURCES.txt
--rw-rw-r--   0 zhguo     (1000) zhguo     (1000)        1 2024-03-06 04:58:25.000000 nanoCEM-0.0.5.4/nanoCEM.egg-info/dependency_links.txt
--rw-rw-r--   0 zhguo     (1000) zhguo     (1000)      178 2024-03-06 04:58:25.000000 nanoCEM-0.0.5.4/nanoCEM.egg-info/requires.txt
--rw-rw-r--   0 zhguo     (1000) zhguo     (1000)        8 2024-03-06 04:58:25.000000 nanoCEM-0.0.5.4/nanoCEM.egg-info/top_level.txt
--rw-rw-r--   0 zhguo     (1000) zhguo     (1000)       38 2024-03-06 04:58:25.716647 nanoCEM-0.0.5.4/setup.cfg
--rw-rw-r--   0 zhguo     (1000) zhguo     (1000)     1291 2024-03-06 04:57:47.000000 nanoCEM-0.0.5.4/setup.py
+drwxrwxr-x   0 zhguo     (1000) zhguo     (1000)        0 2024-04-16 07:30:24.822410 nanoCEM-0.0.5.5/
+-rw-rw-r--   0 zhguo     (1000) zhguo     (1000)     1087 2023-05-31 12:16:43.000000 nanoCEM-0.0.5.5/LICENSE
+-rw-rw-r--   0 zhguo     (1000) zhguo     (1000)     2730 2024-04-16 07:30:24.822410 nanoCEM-0.0.5.5/PKG-INFO
+-rw-rw-r--   0 zhguo     (1000) zhguo     (1000)     2100 2024-03-07 07:08:59.000000 nanoCEM-0.0.5.5/README.md
+drwxrwxr-x   0 zhguo     (1000) zhguo     (1000)        0 2024-04-16 07:30:24.822410 nanoCEM-0.0.5.5/nanoCEM/
+-rw-rw-r--   0 zhguo     (1000) zhguo     (1000)    15651 2024-04-16 07:22:23.000000 nanoCEM-0.0.5.5/nanoCEM/CE_magnifier_test.py
+-rw-rw-r--   0 zhguo     (1000) zhguo     (1000)     5416 2023-12-21 04:37:40.000000 nanoCEM-0.0.5.5/nanoCEM/NEW_TRAINER.py
+-rw-rw-r--   0 zhguo     (1000) zhguo     (1000)       56 2023-06-14 11:15:11.000000 nanoCEM-0.0.5.5/nanoCEM/__init__.py
+-rw-rw-r--   0 zhguo     (1000) zhguo     (1000)     4547 2023-12-10 10:36:58.000000 nanoCEM-0.0.5.5/nanoCEM/alignment_feature_camera.py
+-rw-rw-r--   0 zhguo     (1000) zhguo     (1000)    10849 2024-04-16 04:27:47.000000 nanoCEM-0.0.5.5/nanoCEM/alignment_magnifier
+-rw-rw-r--   0 zhguo     (1000) zhguo     (1000)    14695 2024-04-15 10:30:11.000000 nanoCEM-0.0.5.5/nanoCEM/cem_utils.py
+-rwxrwxr-x   0 zhguo     (1000) zhguo     (1000)    10801 2024-04-13 03:51:24.000000 nanoCEM-0.0.5.5/nanoCEM/current_events_magnifier
+-rw-rw-r--   0 zhguo     (1000) zhguo     (1000)     5903 2024-03-27 13:32:46.000000 nanoCEM-0.0.5.5/nanoCEM/de_novo.py
+-rw-rw-r--   0 zhguo     (1000) zhguo     (1000)     3137 2023-12-15 14:01:45.000000 nanoCEM-0.0.5.5/nanoCEM/density_2d.py
+-rw-rw-r--   0 zhguo     (1000) zhguo     (1000)     4083 2024-02-22 02:44:17.000000 nanoCEM-0.0.5.5/nanoCEM/extract_sub_fast5_from_bam
+-rw-rw-r--   0 zhguo     (1000) zhguo     (1000)     1868 2023-07-24 04:48:56.000000 nanoCEM-0.0.5.5/nanoCEM/extract_sub_fastq_from_bam
+drwxrwxr-x   0 zhguo     (1000) zhguo     (1000)        0 2024-04-16 07:30:24.822410 nanoCEM-0.0.5.5/nanoCEM/f5c_result_rna/
+-rw-rw-r--   0 zhguo     (1000) zhguo     (1000)        0 2024-01-29 04:01:24.000000 nanoCEM-0.0.5.5/nanoCEM/f5c_result_rna/__init__.py
+-rw-rw-r--   0 zhguo     (1000) zhguo     (1000)      318 2024-01-29 04:02:07.000000 nanoCEM-0.0.5.5/nanoCEM/f5c_result_rna/test.py
+-rw-rw-r--   0 zhguo     (1000) zhguo     (1000)     2160 2024-03-27 13:32:46.000000 nanoCEM-0.0.5.5/nanoCEM/kmer_test.py
+-rw-rw-r--   0 zhguo     (1000) zhguo     (1000)     1988 2024-02-23 07:56:30.000000 nanoCEM-0.0.5.5/nanoCEM/kmer_test_pr.py
+-rw-rw-r--   0 zhguo     (1000) zhguo     (1000)     3600 2024-03-27 13:32:45.000000 nanoCEM-0.0.5.5/nanoCEM/machine_learning_trainer.py
+-rw-rw-r--   0 zhguo     (1000) zhguo     (1000)     4427 2024-03-27 13:32:45.000000 nanoCEM-0.0.5.5/nanoCEM/normalization.py
+-rw-rw-r--   0 zhguo     (1000) zhguo     (1000)    11200 2024-02-23 10:21:22.000000 nanoCEM-0.0.5.5/nanoCEM/plot.py
+-rw-rw-r--   0 zhguo     (1000) zhguo     (1000)    10253 2024-04-16 02:28:14.000000 nanoCEM-0.0.5.5/nanoCEM/read_f5c_eventalign.py
+-rw-rw-r--   0 zhguo     (1000) zhguo     (1000)     6811 2024-04-16 02:48:18.000000 nanoCEM-0.0.5.5/nanoCEM/read_f5c_resquiggle.py
+-rw-rw-r--   0 zhguo     (1000) zhguo     (1000)     6866 2024-04-16 02:51:06.000000 nanoCEM-0.0.5.5/nanoCEM/read_move_table.py
+-rw-rw-r--   0 zhguo     (1000) zhguo     (1000)    13342 2024-02-26 08:39:30.000000 nanoCEM-0.0.5.5/nanoCEM/read_tombo_resquiggle.py
+-rw-rw-r--   0 zhguo     (1000) zhguo     (1000)     8548 2024-04-09 09:41:06.000000 nanoCEM-0.0.5.5/nanoCEM/squigualiser_utils.py
+drwxrwxr-x   0 zhguo     (1000) zhguo     (1000)        0 2024-04-16 07:30:24.822410 nanoCEM-0.0.5.5/nanoCEM.egg-info/
+-rw-rw-r--   0 zhguo     (1000) zhguo     (1000)     2730 2024-04-16 07:30:24.000000 nanoCEM-0.0.5.5/nanoCEM.egg-info/PKG-INFO
+-rw-rw-r--   0 zhguo     (1000) zhguo     (1000)      821 2024-04-16 07:30:24.000000 nanoCEM-0.0.5.5/nanoCEM.egg-info/SOURCES.txt
+-rw-rw-r--   0 zhguo     (1000) zhguo     (1000)        1 2024-04-16 07:30:24.000000 nanoCEM-0.0.5.5/nanoCEM.egg-info/dependency_links.txt
+-rw-rw-r--   0 zhguo     (1000) zhguo     (1000)      178 2024-04-16 07:30:24.000000 nanoCEM-0.0.5.5/nanoCEM.egg-info/requires.txt
+-rw-rw-r--   0 zhguo     (1000) zhguo     (1000)        8 2024-04-16 07:30:24.000000 nanoCEM-0.0.5.5/nanoCEM.egg-info/top_level.txt
+-rw-rw-r--   0 zhguo     (1000) zhguo     (1000)       38 2024-04-16 07:30:24.822410 nanoCEM-0.0.5.5/setup.cfg
+-rw-rw-r--   0 zhguo     (1000) zhguo     (1000)     1295 2024-04-16 07:30:08.000000 nanoCEM-0.0.5.5/setup.py
```

### Comparing `nanoCEM-0.0.5.4/LICENSE` & `nanoCEM-0.0.5.5/LICENSE`

 * *Files identical despite different names*

### Comparing `nanoCEM-0.0.5.4/PKG-INFO` & `nanoCEM-0.0.5.5/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 Metadata-Version: 2.1
 Name: nanoCEM
-Version: 0.0.5.4
+Version: 0.0.5.5
 Summary: A simple tool designed to visualize the features that distinguish between two groups of ONT data at the site level.                It supports 4 re-squiggle program(tombo resquiggle/f5c resquiggle/f5c eventalign/move_table).
 Home-page: https://github.com/lrslab/nanoCEM
 Author: GUO Zhihao
 Author-email: qhuozhihao@icloud.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
-Requires-Python: >=3.7,<=3.11
+Requires-Python: >=3.7.0,<=3.11.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # nanoCEM ![logo](docs/logo_tiny.png "nanoCEM")
 <a href="https://pypi.python.org/pypi/nanoCEM" rel="pypi">![PyPI](https://img.shields.io/pypi/v/nanoCEM?color=green) </a>
 <a href="https://opensource.org/license/mit/" rel="license">![License](https://img.shields.io/pypi/l/nanoCEM?color=orange)</a>
 
@@ -42,15 +42,23 @@
     docker pull zhihaguo/nanocem_env
     
 To check the version of nanoCEM, run:
 
     pip list | grep nanoCEM
 
 
- **Notes:** Additionally, we do not rely on any re-squiggle or eventalign packages. We only need their index files for the sequencing data.
+## Solutions for some potential environment problem
+Although it does not affect the functionality, the issue of possible missing header files caused by **samtools** installation by conda can be resolved with the following command.
+
+    conda install -c conda-forge ncurses
+
+The potential **vbz** format compression issue when reading **fast5** files.
+
+    conda install -c bioconda ont_vbz_hdf_plugin
+
 
 
 ## Data release
 For the data we used and related commands in our paper, please view our [wiki](https://github.com/lrslab/nanoCEM/wiki/Data-release-and-commands)
 
 ## Documents
 Full documentation is available at https://nanocem.readthedocs.io/
```

#### html2text {}

```diff
@@ -1,16 +1,16 @@
-Metadata-Version: 2.1 Name: nanoCEM Version: 0.0.5.4 Summary: A simple tool
+Metadata-Version: 2.1 Name: nanoCEM Version: 0.0.5.5 Summary: A simple tool
 designed to visualize the features that distinguish between two groups of ONT
 data at the site level. It supports 4 re-squiggle program(tombo resquiggle/f5c
 resquiggle/f5c eventalign/move_table). Home-page: https://github.com/lrslab/
 nanoCEM Author: GUO Zhihao Author-email: qhuozhihao@icloud.com Classifier:
 Programming Language :: Python :: 3 Classifier: License :: OSI Approved :: MIT
 License Classifier: Operating System :: OS Independent Requires-Python:
->=3.7,<=3.11 Description-Content-Type: text/markdown License-File: LICENSE #
-nanoCEM ![logo](docs/logo_tiny.png "nanoCEM") _!_[_P_y_P_I_]_(_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/
+>=3.7.0,<=3.11.7 Description-Content-Type: text/markdown License-File: LICENSE
+# nanoCEM ![logo](docs/logo_tiny.png "nanoCEM") _!_[_P_y_P_I_]_(_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/
 _p_y_p_i_/_v_/_n_a_n_o_C_E_M_?_c_o_l_o_r_=_g_r_e_e_n_)_ _!_[_L_i_c_e_n_s_e_]_(_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_p_y_p_i_/_l_/
 _n_a_n_o_C_E_M_?_c_o_l_o_r_=_o_r_a_n_g_e_) The nanopore current events magnifier (`nanoCEM`) is a
 python command line to facilitate the analysis of DNA/RNA modification sites by
 visualizing statistical features of current events. NanoCEM can be used to
 showcase high confidence sites and observe the difference based on the
 modification sample and the low or no modification sample. It supports two re-
 squiggle pipeline(`Tombo` and `f5c`) and support `R9` and `R10`. If you want to
@@ -18,13 +18,16 @@
 hiruna72/squigualiser) is recommended. ## Installation Before pip install, make
 sure you have installed the `samtools`(>=1.16) , `f5c`(>=1.4), `slow5tools`
 (>=1.1.0) and `minimap2`(>=2.17), conda install samtools=1.16 minimap2 f5c=1.4
 slow5tools -c conda-forge -c bioconda To install the latest nanoCEM pip install
 nanoCEM And install from the resource git clone https://github.com/lrslab/
 nanoCEM.git cd nanoCEM/ pip install . To install nanoCEM from docker, docker
 pull zhihaguo/nanocem_env To check the version of nanoCEM, run: pip list | grep
-nanoCEM **Notes:** Additionally, we do not rely on any re-squiggle or
-eventalign packages. We only need their index files for the sequencing data. ##
-Data release For the data we used and related commands in our paper, please
-view our [wiki](https://github.com/lrslab/nanoCEM/wiki/Data-release-and-
-commands) ## Documents Full documentation is available at https://
+nanoCEM ## Solutions for some potential environment problem Although it does
+not affect the functionality, the issue of possible missing header files caused
+by **samtools** installation by conda can be resolved with the following
+command. conda install -c conda-forge ncurses The potential **vbz** format
+compression issue when reading **fast5** files. conda install -c bioconda
+ont_vbz_hdf_plugin ## Data release For the data we used and related commands in
+our paper, please view our [wiki](https://github.com/lrslab/nanoCEM/wiki/Data-
+release-and-commands) ## Documents Full documentation is available at https://
 nanocem.readthedocs.io/ ## Workflow ![workflow](docs/Workflow.png)
```

### Comparing `nanoCEM-0.0.5.4/README.md` & `nanoCEM-0.0.5.5/README.md`

 * *Files 14% similar despite different names*

```diff
@@ -28,15 +28,23 @@
     docker pull zhihaguo/nanocem_env
     
 To check the version of nanoCEM, run:
 
     pip list | grep nanoCEM
 
 
- **Notes:** Additionally, we do not rely on any re-squiggle or eventalign packages. We only need their index files for the sequencing data.
+## Solutions for some potential environment problem
+Although it does not affect the functionality, the issue of possible missing header files caused by **samtools** installation by conda can be resolved with the following command.
+
+    conda install -c conda-forge ncurses
+
+The potential **vbz** format compression issue when reading **fast5** files.
+
+    conda install -c bioconda ont_vbz_hdf_plugin
+
 
 
 ## Data release
 For the data we used and related commands in our paper, please view our [wiki](https://github.com/lrslab/nanoCEM/wiki/Data-release-and-commands)
 
 ## Documents
 Full documentation is available at https://nanocem.readthedocs.io/
```

#### html2text {}

```diff
@@ -10,13 +10,16 @@
 hiruna72/squigualiser) is recommended. ## Installation Before pip install, make
 sure you have installed the `samtools`(>=1.16) , `f5c`(>=1.4), `slow5tools`
 (>=1.1.0) and `minimap2`(>=2.17), conda install samtools=1.16 minimap2 f5c=1.4
 slow5tools -c conda-forge -c bioconda To install the latest nanoCEM pip install
 nanoCEM And install from the resource git clone https://github.com/lrslab/
 nanoCEM.git cd nanoCEM/ pip install . To install nanoCEM from docker, docker
 pull zhihaguo/nanocem_env To check the version of nanoCEM, run: pip list | grep
-nanoCEM **Notes:** Additionally, we do not rely on any re-squiggle or
-eventalign packages. We only need their index files for the sequencing data. ##
-Data release For the data we used and related commands in our paper, please
-view our [wiki](https://github.com/lrslab/nanoCEM/wiki/Data-release-and-
-commands) ## Documents Full documentation is available at https://
+nanoCEM ## Solutions for some potential environment problem Although it does
+not affect the functionality, the issue of possible missing header files caused
+by **samtools** installation by conda can be resolved with the following
+command. conda install -c conda-forge ncurses The potential **vbz** format
+compression issue when reading **fast5** files. conda install -c bioconda
+ont_vbz_hdf_plugin ## Data release For the data we used and related commands in
+our paper, please view our [wiki](https://github.com/lrslab/nanoCEM/wiki/Data-
+release-and-commands) ## Documents Full documentation is available at https://
 nanocem.readthedocs.io/ ## Workflow ![workflow](docs/Workflow.png)
```

### Comparing `nanoCEM-0.0.5.4/nanoCEM/CE_magnifier_test.py` & `nanoCEM-0.0.5.5/nanoCEM/CE_magnifier_test.py`

 * *Files 6% similar despite different names*

```diff
@@ -57,15 +57,15 @@
     add_public_argument(parser_f5c)
 
     parser_f5c = subparsers.add_parser('f5c_re', help='tackle f5c re-squiggle')
     parser_f5c.add_argument("-i", "--input", required=True,
                             help="blow5_path")
     parser_f5c.add_argument('-c', "--control",
                             help="control_blow5_path")
-    parser_f5c.add_argument('--base_shift', action='store_true', help='Turn on the base shift')
+    parser_f5c.add_argument('--base_shift',choices=['auto',0,-1,-2,-3,-4,-5,-6,-7,-8], default='auto', help='base shift option')
     parser_f5c.add_argument('--pore', choices=['r9', 'r10','rna004'], help='Select pore type', default='r9')
     add_public_argument(parser_f5c)
 
     parser_f5c = subparsers.add_parser('move_table', help='tackle move_table from basecaller')
     parser_f5c.add_argument("-i", "--input", required=True,
                             help="blow5_path")
     parser_f5c.add_argument('-c', "--control",
@@ -98,32 +98,39 @@
     #                     subsample_ratio=1,
     #                     ref="../example/data/23S_rRNA.fasta", rna=True)
     # parser.set_defaults(function='move_table', chrom="17", pos=43281378, len=10, strand='+', cpu=8,norm=True,
     #                                         input='../example/dna/hg38_chr17_43281378/WGS_r941/basecall',
     #                                         control='../example/dna/hg38_chr17_43281378/scWGA_941/basecall', output='move_result_dna',
     #                     subsample_ratio=1,sig_move_offset=4,kmer_length=5,
     #                     ref="../example/dna/hg38_17.fa", rna=False)
-    # parser.set_defaults(function='f5c_ev', chrom="17", pos=43281925, len=10, strand='+', cpu=8,base_shift=True,norm=True,
-    #                     input='../example/dna/hg38_chr17_43281378/WGS_r941/file',
-    #                     control='../example/dna/hg38_chr17_43281378/scWGA_941/file', output='f5c_result_dna_ev',
+    # parser.set_defaults(function='f5c_re', chrom="17", pos=43281378, len=10, strand='-', cpu=8,base_shift='auto',norm=True,
+    #                     input='../example/dna/hg38_chr17_43281378/WGS_r941/file',kmer_size=3,
+    #                     control='../example/dna/hg38_chr17_43281378/scWGA_941/file', output='f5c_result_dna_re',
     #                     subsample_ratio=1,rna=False,
     #                     ref="../example/dna/hg38_17.fa", pore='r9')
+    # parser.set_defaults(function='f5c_re', chrom="17", pos=39976063, len=10, strand='-', cpu=8, base_shift='auto',
+    #                     norm=True,
+    #                     input='../example/dna/hg38_chr17_43281378/WGS_r941/file', kmer_size=3,
+    #                     control='../example/dna/hg38_chr17_43281378/scWGA_941/file', output='f5c_result_dna_re_re',
+    #                     subsample_ratio=1, rna=False,
+    #                     ref="../example/dna/hg38_17_rev.fa", pore='r9')
+
     # parser.set_defaults(function='f5c_re', chrom="NR_103073.1", pos=2524, len=10, strand='+', cpu=8,base_shift=True,norm=True,
     #                     input='/hdd_data/download/23s_rRNA_A2030/wt/file',
     #                     control='/hdd_data/download/23s_rRNA_A2030/ivt/file', output='f5c_result_rna_re_2524',
     #                     subsample_ratio=1,rna=True,
     #                     ref="../example/data/23S_rRNA.fasta", pore='r9')
-    # parser.set_defaults(function='f5c', chrom="NR_103073.1", pos=875, len=10, strand='-', cpu=8,norm=True,base_shift=True,pore='r9',
-    #                     input='../example/data/wt/file', control='../example/data/ivt/file', output='f5c_result_rna_re',
-    #                     subsample_ratio=1,
+    # parser.set_defaults(function='f5c_re', chrom="NR_103073.1", pos=875, len=10, strand='-', cpu=8,norm=True,base_shift='auto',pore='r9',
+    #                     input='../example/data/wt/file', control='../example/data/ivt/file', output='f5c_result_rna_re_re',
+    #                     subsample_ratio=1,kmer_size=3,
     #                     ref="../example/data/reverse/23S_rRNA_re.fasta", rna=True)
-    parser.set_defaults(function='f5c_ev', chrom="NR_103073.1", pos=2251, len=5, strand='+', cpu=8,norm=True,base_shift=False,pore='r9',
-                        input='../example/data/wt/file', control='../example/data/ivt/file', output='f5c_result_rna_ev_2251',
-                        subsample_ratio=1,
-                        ref="../example/data/23S_rRNA.fasta", rna=True)
+    # parser.set_defaults(function='f5c_ev', chrom="NR_103073.1", pos=2251, len=5, strand='+', cpu=8,norm=True,base_shift='auto',pore='r9',
+    #                     input='../example/data/wt/file', control='../example/data/ivt/file', output='f5c_result_rna_ev_2251',kmer_size=3,
+    #                     subsample_ratio=1,
+    #                     ref="../example/data/23S_rRNA.fasta", rna=True)
     return parser
 
 if __name__ == '__main__':
     # Parse the arguments
     parser = init_parser()
     args = parser.parse_args()
     # args check
@@ -218,29 +225,29 @@
 
             df = pd.concat([df_wt, df_ivt])
         except:
             single_mode =True
         if args.control is None:
             single_mode =True
     else:
-        raise  RuntimeError("Wrong option")
+        raise  RuntimeError("Wrong option, select from tombo, move_table, f5c_ev, f5c_re")
     if single_mode:
         df = df_wt
         df_wt['Group'] = 'Single'
         title = title + '   Sample:' + str(aligned_num_wt)
     else:
         df = pd.concat([df_wt, df_ivt])
         title = title + '   Sample:' + str(aligned_num_wt) + '  Control:' + str(aligned_num_ivt)
         category = pd.api.types.CategoricalDtype(categories=['Sample', "Control"], ordered=True)
         df['Group'] = df['Group'].astype(category)
 
     # save result table
     df_copy = copy.deepcopy(df)
     df_copy['Position'] = df_copy['Position'].astype(int) + 1
-    df_copy.to_csv(results_path + '/current_feature.csv', index=None)
+    df_copy.to_csv(results_path + '/current_feature.csv', index=False)
     print("Feature file saved  in " + results_path + '/current_feature.csv')
     # draw current feature
     current_plot(df, results_path, args.pos, base_list, title,filter=True)
     if not single_mode:
         if args.kmer_size is None:
             args.kmer_size = 3
         # draw PCA
```

### Comparing `nanoCEM-0.0.5.4/nanoCEM/NEW_TRAINER.py` & `nanoCEM-0.0.5.5/nanoCEM/NEW_TRAINER.py`

 * *Files identical despite different names*

### Comparing `nanoCEM-0.0.5.4/nanoCEM/alignment_feature_camera.py` & `nanoCEM-0.0.5.5/nanoCEM/alignment_feature_camera.py`

 * *Files identical despite different names*

### Comparing `nanoCEM-0.0.5.4/nanoCEM/cem_utils.py` & `nanoCEM-0.0.5.5/nanoCEM/cem_utils.py`

 * *Files 5% similar despite different names*

```diff
@@ -3,25 +3,36 @@
 from collections import OrderedDict
 import subprocess
 import numpy as np
 import pandas as pd
 from tqdm import tqdm
 import multiprocessing
 import warnings
+
 warnings.filterwarnings("ignore", category=FutureWarning)
 from scipy import stats
 import copy
 
 ker_model_size ={
     'r9+RNA': 5,
     'r9+DNA': 6,
     'r10+DNA': 9,
     'rna004+RNA': 9
 }
 
+base_shift_dict ={
+    'r9RNA+': -1,
+    'r9RNA-': -3,
+    'r9DNA+': -2,
+    'r9DNA-': -3,
+    'r10DNA+': -2,
+    'r10DNA-': -6,
+    'rna004+RNA': 9
+}
+
 def caculate_base_shift_size(kmer_model,strand):
     def is_odd(number):
         if number % 2 == 0:
             return False
         else:
             return True
     if kmer_model<=1:
@@ -381,7 +392,8 @@
     new_df.columns = ['Position', 'P value(-log10)','Norm_differ']
     return new_df
 
 # fasta=read_fasta_to_dic("../example/data/23S_rRNA.fasta")
 # for key,value in fasta.items():
 #     fasta[key]=reverse_fasta(value)
 # save_fasta_dict(fasta,'../example/data/23S_rRNA_re.fasta')
+
```

### Comparing `nanoCEM-0.0.5.4/nanoCEM/current_events_magnifier` & `nanoCEM-0.0.5.5/nanoCEM/alignment_magnifier`

 * *Files 1% similar despite different names*

```diff
@@ -19,15 +19,15 @@
         parser_input.add_argument("--strand", default="+", help="Strand of your interest")
         parser_input.add_argument('-r', "--ref", required=True, help="fasta file")
         parser_input.add_argument('-t', "--cpu", default=4, type=int, help="num of process")
         parser_input.add_argument('--norm', action='store_true', help='Turn on the normalization mode')
         parser_input.add_argument('-s', "--subsample_ratio", default=1, type=float,
                                   help="Subsample ratio to select reads")
         parser_input.add_argument('--rna', action='store_true', help='Turn on the RNA mode')
-        parser_input.add_argument('--kmer_size', choices=[3,5,7],default=3, type=int,  help="kmer size for PCA and MANOVA analysis")
+        parser_input.add_argument('--kmer_size', choices=[3,5,7],default=3, help="kmer size for PCA and MANOVA analysis")
         parser_input.add_argument('-o', "--output", default="nanoCEM_result", help="output_file")
 
     # Define the argument parser
     parser = argparse.ArgumentParser(
         description='A sample tool designed to visualize the features that distinguish between two groups of ONT data at the site level. It supports two re-squiggle pipeline(Tombo and f5c).')
     subparsers = parser.add_subparsers(dest='function')
 
@@ -37,14 +37,16 @@
                               help='The attribute group to extract the training data from. e.g. RawGenomeCorrected_000')
     parser_tombo.add_argument('--basecall_subgroup', default='BaseCalled_template',
                               help='Basecall subgroup Nanoraw resquiggle into. Default is BaseCalled_template')
     parser_tombo.add_argument('-i', "--input_fast5", required=True,
                               help="input_fast5_file")
     parser_tombo.add_argument('-c', "--control_fast5",
                               help="control_fast5_file")
+    # parser_tombo.add_argument('-b', "--bam", help="bam file to help index to speed up")
+
 
     add_public_argument(parser_tombo)
 
     # f5c subparser
     parser_f5c = subparsers.add_parser('f5c_ev', help='tackle f5c eventalign')
     parser_f5c.add_argument("-i", "--input", required=True,
                             help="blow5_path")
@@ -55,15 +57,15 @@
     add_public_argument(parser_f5c)
 
     parser_f5c = subparsers.add_parser('f5c_re', help='tackle f5c re-squiggle')
     parser_f5c.add_argument("-i", "--input", required=True,
                             help="blow5_path")
     parser_f5c.add_argument('-c', "--control",
                             help="control_blow5_path")
-    parser_f5c.add_argument('--base_shift', action='store_true', help='Turn on the base shift')
+    parser_f5c.add_argument('--base_shift',choices=['auto',0,-1,-2,-3,-4,-5,-6,-7,-8], default='auto', help='base shift option')
     parser_f5c.add_argument('--pore', choices=['r9', 'r10','rna004'], help='Select pore type', default='r9')
     add_public_argument(parser_f5c)
 
     parser_f5c = subparsers.add_parser('move_table', help='tackle move_table from basecaller')
     parser_f5c.add_argument("-i", "--input", required=True,
                             help="blow5_path")
     parser_f5c.add_argument('-c', "--control",
@@ -144,14 +146,15 @@
         df_wt['Group'] = 'Sample'
         try:
             df_ivt, aligned_num_ivt = read_basecall_bam(args.control, args.pos, args.ref, args.len, args.chrom, args.strand, args.sig_move_offset, args.kmer_length,
                                                     subsample_ratio, args.norm, str(args.cpu),
                                                     args.rna)
             df_ivt['Group'] = 'Control'
 
+
         except Exception as e:
             print(e)
             single_mode = True
         if args.control is None:
             single_mode = True
     elif args.function == 'f5c_re':
         from nanoCEM.read_f5c_resquiggle import read_blow5
@@ -168,37 +171,35 @@
 
             df = pd.concat([df_wt, df_ivt])
         except:
             single_mode =True
         if args.control is None:
             single_mode =True
     else:
-        raise  RuntimeError("Wrong option")
+        raise  RuntimeError("Wrong option, select from tombo, move_table, f5c_ev, f5c_re")
     if single_mode:
         df = df_wt
         df_wt['Group'] = 'Single'
         title = title + '   Sample:' + str(aligned_num_wt)
     else:
         df = pd.concat([df_wt, df_ivt])
         title = title + '   Sample:' + str(aligned_num_wt) + '  Control:' + str(aligned_num_ivt)
         category = pd.api.types.CategoricalDtype(categories=['Sample', "Control"], ordered=True)
         df['Group'] = df['Group'].astype(category)
 
     # save result table
     df_copy = copy.deepcopy(df)
     df_copy['Position'] = df_copy['Position'].astype(int) + 1
-    df_copy.to_csv(results_path + '/current_feature.csv', index=None)
+    df_copy.to_csv(results_path + '/current_feature.csv', index=False)
     print("Feature file saved  in " + results_path + '/current_feature.csv')
     # draw current feature
     current_plot(df, results_path, args.pos, base_list, title,filter=True)
     if not single_mode:
         if args.kmer_size is None:
             args.kmer_size = 3
-        if args.kmer_size > args.len:
-            raise RuntimeError("kmer_size is larger than windows size, please re-choose len of kmer_size")
         # draw PCA
         kmer_size = args.kmer_size
         # df_copy.loc[:, 'Position'] = df_copy['Position'].astype(int)
         feature_matrix, label = extract_kmer_feature(df_copy,kmer_size, args.pos + 1)
         plot_PCA(feature_matrix, label, results_path)
         # draw p_value
         new_df = calculate_MANOVA_result( args.pos+1,df_copy,args.len,500,args.len,kmer_size)
```

### Comparing `nanoCEM-0.0.5.4/nanoCEM/de_novo.py` & `nanoCEM-0.0.5.5/nanoCEM/de_novo.py`

 * *Files identical despite different names*

### Comparing `nanoCEM-0.0.5.4/nanoCEM/density_2d.py` & `nanoCEM-0.0.5.5/nanoCEM/density_2d.py`

 * *Files identical despite different names*

### Comparing `nanoCEM-0.0.5.4/nanoCEM/extract_sub_fast5_from_bam` & `nanoCEM-0.0.5.5/nanoCEM/extract_sub_fast5_from_bam`

 * *Files identical despite different names*

### Comparing `nanoCEM-0.0.5.4/nanoCEM/extract_sub_fastq_from_bam` & `nanoCEM-0.0.5.5/nanoCEM/extract_sub_fastq_from_bam`

 * *Files identical despite different names*

### Comparing `nanoCEM-0.0.5.4/nanoCEM/kmer_test.py` & `nanoCEM-0.0.5.5/nanoCEM/kmer_test.py`

 * *Files identical despite different names*

### Comparing `nanoCEM-0.0.5.4/nanoCEM/kmer_test_pr.py` & `nanoCEM-0.0.5.5/nanoCEM/kmer_test_pr.py`

 * *Files identical despite different names*

### Comparing `nanoCEM-0.0.5.4/nanoCEM/machine_learning_trainer.py` & `nanoCEM-0.0.5.5/nanoCEM/machine_learning_trainer.py`

 * *Files identical despite different names*

### Comparing `nanoCEM-0.0.5.4/nanoCEM/normalization.py` & `nanoCEM-0.0.5.5/nanoCEM/normalization.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 import numpy as np
-OUTLIER_THRESH = 3.0
+OUTLIER_THRESH = 5.0
 MAX_POINTS_FOR_THEIL_SEN = 1000
 
 def normalize_signal_with_lim(raw_signal, lower_lim=-OUTLIER_THRESH, upper_lim=OUTLIER_THRESH):
     # shift = np.median(signal)
     # # note factor to scale MAD to SD
     # scale = np.median(np.absolute(signal - shift)) * 1.4826
     # norm_signal = (signal - shift) / scale
```

### Comparing `nanoCEM-0.0.5.4/nanoCEM/plot.py` & `nanoCEM-0.0.5.5/nanoCEM/plot.py`

 * *Files identical despite different names*

### Comparing `nanoCEM-0.0.5.4/nanoCEM/read_f5c_eventalign.py` & `nanoCEM-0.0.5.5/nanoCEM/read_f5c_eventalign.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,27 +1,29 @@
 import re
 import numpy as np
 import pandas as pd
 import pyslow5
 import pysam
 from tqdm import tqdm
 from nanoCEM.normalization import normalize_signal,normalize_signal_with_lim
-from nanoCEM.cem_utils import generate_bam_file,identify_file_path,generate_paf_file_eventalign
+from nanoCEM.cem_utils import generate_bam_file,identify_file_path,generate_paf_file_eventalign,base_shift_dict
 # from nanoCEM.plot import draw_signal
 # import os
 # import argparse
 score_dict={}
 nucleotide_type=None
 
 def extract_feature(line,strand,position,windows_length,base_shift=2,norm=True):
     global nucleotide_type
     pbar.update(1)
     read_id = line[0]
-    if read_id == '0a017d09-5c09-456d-8875-635f4c2c1380':
-        print(1)
+    # if read_id == '0a017d09-5c09-456d-8875-635f4c2c1380':
+    #     print(1)
+    if line[4] != strand:
+        return None
     # tackle moves tag
     moves_string = line[14]
     moves_string = re.sub('ss:Z:', '', moves_string)
     moves_string = re.sub('D', 'D,', moves_string)
     moves_string = re.sub('I', 'I,', moves_string)
     # print(moves_string)
     moves = re.split(r',+', moves_string)
@@ -66,47 +68,40 @@
 
     signal = signal[start_index:end_index]
     if norm:
         signal, shift, scale = normalize_signal_with_lim(signal)
     event_starts = event_length.cumsum()
     event_starts = np.insert(event_starts, 0, 0)[:-1]
 
-
-    # index query and reference map index
-    if nucleotide_type == 'RNA' :
-        # signal = np.flip(signal)
-        # event_length = np.flip(event_length)
-        ref_start = line[8]
-        start_position = np.max([line[8], position - windows_length]) - ref_start
-        end_position = np.min([line[7], position + windows_length]) - ref_start
-
-    else:
-        ref_start = line[7]
-        start_position = np.max([line[7], position - windows_length]) - ref_start
-        end_position = np.min([line[8], position + windows_length]) - ref_start
-
     # base shift
-    if (nucleotide_type == 'RNA' and strand == '+') or (nucleotide_type == 'DNA' and strand == '-'):
-        end_pos = line[10] - start_position - 1 + base_shift
-        start_pos = line[10] - end_position - 1 + base_shift
+    ref_start = np.min([line[7],line[8]])
+    ref_end = np.max([line[7], line[8]])
+    ref_start = ref_start - base_shift
+    ref_end = ref_end - base_shift
+    start_position = np.max([ref_start, position - windows_length]) - ref_start
+    end_position = np.min([ref_end, position + windows_length]) - ref_start
 
+    # index query and reference map index
+    if (nucleotide_type == 'RNA' and strand=='+') or (nucleotide_type == 'DNA' and strand=='-'):
+        end_pos = line[10] - start_position - 1
+        start_pos = line[10] - end_position - 1
     else:
-        end_pos = end_position - base_shift
-        start_pos = start_position - base_shift
+        end_pos = end_position
+        start_pos = start_position
 
     end_pos = np.min([end_pos, line[10] - 1])
     # extract raw signal by event length and event start
     total_feature_per_reads = []
     raw_signal_every = [signal[event_starts[x]:event_starts[x] + event_length[x]] for x in
                         range(start_pos,end_pos+1)]
-    if (nucleotide_type == 'RNA' and strand == '+') or (nucleotide_type == 'DNA' and strand == '-'):
+    if (nucleotide_type == 'RNA' and strand=='+') or (nucleotide_type == 'DNA' and strand=='-'):
         raw_signal_every.reverse()
     # calculate mean median and dwell time
     for i, element in enumerate(raw_signal_every):
-        if len(element)==0:
+        if len(element) == 0:
             continue
         temp = [read_id,np.mean(element), np.std(element), np.median(element), len(element), str(start_position+ref_start+i)]
         total_feature_per_reads.append(temp)
     return total_feature_per_reads
 
 def extract_pairs_pos(bam_file,position,length,chromosome,strand):
 
@@ -114,45 +109,40 @@
     for read in bam_file.fetch(chromosome,position-length, position+length+1):
         if read.is_supplementary or read.is_secondary:
             continue
         if strand == '+' and read.is_reverse:
             continue
         if strand == '-' and not read.is_reverse:
             continue
-        if read.qname == 'db71b047-e073-42cf-833b-a3ccdd9459b3':
-            print(1)
+        # if read.qname == 'db71b047-e073-42cf-833b-a3ccdd9459b3':
+        #     print(1)
         start_position=read.reference_start
         end_position=read.reference_end
         if position < start_position or position > end_position:
             continue
         # unit
         temp={}
         temp['ref_length'] = read.reference_length
         result_dict[read.qname] = temp
     return result_dict
 
-
-
-def read_blow5(path,position,reference,length,chrom,strand,pore,subsample_ratio=1,base_shift=True,norm=True,cpu=4,rna=True):
+def read_blow5(path,position,reference,length,chrom,strand,pore,subsample_ratio=1,base_shift='auto',norm=True,cpu=4,rna=True):
     global s5,pbar
     slow5_file = path + ".blow5"
     fastq_file = path + ".fastq"
     identify_file_path(fastq_file)
     identify_file_path(slow5_file)
-
-    if base_shift:
-        if rna or (pore == 'r9' and not rna):
-            base_shift = 2
-        else:
-            base_shift = 4
+    if rna:
+        nucleotide_type = "RNA"
     else:
-        base_shift = 0
-    if strand =='-' and not rna and pore == 'r9':
-        base_shift = 3
-
+        nucleotide_type = 'DNA'
+    if base_shift == 'auto':
+        base_shift = base_shift_dict[pore+nucleotide_type+strand]
+    else:
+        base_shift = base_shift
     fastq_file, bam_file = generate_bam_file(fastq_file, reference, cpu, subsample_ratio)
     paf_file = generate_paf_file_eventalign(fastq_file,slow5_file,bam_file,reference,pore,rna,cpu)
 
     bam_file = pysam.AlignmentFile(bam_file,'rb')
 
     info_dict = extract_pairs_pos(bam_file,position,length,chrom,strand)
     if info_dict == {}:
```

### Comparing `nanoCEM-0.0.5.4/nanoCEM/read_f5c_resquiggle.py` & `nanoCEM-0.0.5.5/nanoCEM/read_f5c_resquiggle.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,22 +1,25 @@
 import re
 import numpy as np
 import pandas as pd
-import pyslow5
 import pysam
+import pyslow5
 from tqdm import tqdm
-from nanoCEM.normalization import normalize_signal,normalize_signal_with_lim
-from nanoCEM.cem_utils import generate_bam_file,identify_file_path,generate_paf_file_resquiggle,ker_model_size,caculate_base_shift_size
+
+from nanoCEM.cem_utils import generate_bam_file, identify_file_path, generate_paf_file_resquiggle, base_shift_dict,ker_model_size
+from nanoCEM.normalization import normalize_signal_with_lim
 # from nanoCEM.plot import draw_signal
-from nanoCEM.read_move_table import  extract_pairs_pos
+from nanoCEM.read_move_table import extract_pairs_pos
+
 # import os
 # import argparse
-score_dict={}
-nucleotide_type=None
-def extract_feature(line,strand,kmer_model,base_shift,norm=True):
+score_dict = {}
+nucleotide_type = None
+
+def extract_feature(line,kmer_model,strand,base_shift, norm=True):
     global nucleotide_type
     pbar.update(1)
     read_id = line[0]
     # if read_id =='94c4929a-8630-4fd0-89d5-21f6bc399165':
     #     print(1)
     if read_id not in info_dict:
         return None
@@ -27,73 +30,72 @@
     moves_string = re.sub('I', 'I,', moves_string)
     # print(moves_string)
     moves = re.split(r',+', moves_string)
     moves = moves[:-1]
     # extract index and generate event_length and event_start
     insertion = 0
     event_length = []
-    for i,item in enumerate(moves):
+    for i, item in enumerate(moves):
         if 'D' in item:
             deletion = int(item[:-1])
             for i in range(deletion):
                 event_length.append(0)
         elif 'I' in item:
-            if i == 0 :
+            if i == 0:
                 continue
             else:
                 return None
         elif '=' in item:
             return None
         else:
             event_length.append(int(item))
     # build event_length from move table
-    read = s5.get_read(read_id, aux=["read_number", "start_mux"],pA=True)
+    read = s5.get_read(read_id, aux=["read_number", "start_mux"], pA=True)
     start_index = line[2]
     end_index = line[3]
     event_length = np.array(event_length)
 
     # identify RNA or DNA
     if nucleotide_type is None:
-        if line[7]>line[8]:
-            nucleotide_type='RNA'
+        if line[7] > line[8]:
+            nucleotide_type = 'RNA'
         else:
-            nucleotide_type='DNA'
+            nucleotide_type = 'DNA'
     #  assert len_raw_signal in paf and blow5
     try:
-        assert end_index-start_index == np.sum(event_length)
+        assert end_index - start_index == np.sum(event_length)
         assert read['len_raw_signal'] == line[1]
 
     except Exception:
         print("Warning: 1 read's length of signal is not equal between blow5 and paf")
         return None
 
     signal = read['signal']
 
     # create event start and flip all table
     signal = signal[start_index:end_index]
     event_starts = event_length.cumsum()
     event_starts = np.insert(event_starts, 0, 0)[:-1]
     if norm:
-        signal,_,_ = normalize_signal_with_lim(signal)
+        signal, _, _ = normalize_signal_with_lim(signal)
 
     # index query and reference
-    aligned_pair=info_dict[read_id]['pairs']
+    aligned_pair = info_dict[read_id]['pairs']
     qlen = info_dict[read_id]['query_length']
     # assert len(event_length) + kmer_model - 1 == qlen
 
     # correct index about DNA and RNA
-    if (nucleotide_type == 'RNA' and strand == '+') or (nucleotide_type == 'DNA' and strand == '-'):
+    if (nucleotide_type == 'RNA' and strand=='+') or (nucleotide_type == 'DNA' and strand=='-'):
         aligned_pair[0] = qlen - aligned_pair[0] - 1
-        aligned_pair[0] = aligned_pair[0] - kmer_model + 1
-
-    if base_shift != 0:
-        aligned_pair[1] = aligned_pair[1] + base_shift
+        aligned_pair[1] = aligned_pair[1] - kmer_model - base_shift + 1
+    else:
+        aligned_pair[1] = aligned_pair[1] - base_shift
 
-    aligned_pair = aligned_pair[(aligned_pair[0]>=0)&(aligned_pair[0]<len(event_length))]
-    if aligned_pair.shape[0]==0:
+    aligned_pair = aligned_pair[(aligned_pair[0] >= 0) & (aligned_pair[0] < len(event_length))]
+    if aligned_pair.shape[0] == 0:
         return None
     read_pos = aligned_pair[0].values
     ref_pos = aligned_pair[1].values
 
     # extract raw signal by event length and event start
     total_feature_per_reads = []
     try:
@@ -104,69 +106,70 @@
     except Exception as e:
         print(e)
         return None
     # calculate mean median and dwell time
     for i, element in enumerate(raw_signal_every):
         if event_length[read_pos[i]] == 0:
             continue
-        temp = [read_id,np.mean(element), np.std(element), np.median(element), event_length[read_pos[i]],ref_pos[i]]
+        temp = [read_id, np.mean(element), np.std(element), np.median(element), event_length[read_pos[i]], ref_pos[i]]
         total_feature_per_reads.append(temp)
     return total_feature_per_reads
 
 
-def read_blow5(path,position,reference,length,chrom,strand,pore,subsample_ratio=1,base_shift=True,norm=True,cpu=4,rna=True):
-    global s5,pbar,info_dict
+def read_blow5(path, position, reference, length, chrom, strand, pore, subsample_ratio=1, base_shift=True, norm=True,
+               cpu=4, rna=True):
+    global s5, pbar, info_dict
     slow5_file = path + ".blow5"
     fastq_file = path + ".fastq"
     identify_file_path(fastq_file)
     identify_file_path(slow5_file)
 
     if rna:
-        nucleotide_type='RNA'
+        nucleotide_type = 'RNA'
     else:
-        nucleotide_type='DNA'
+        nucleotide_type = 'DNA'
     kmer_model = ker_model_size[pore+'+'+nucleotide_type]
-    if base_shift:
-        base_shift = caculate_base_shift_size(kmer_model,strand)
+    if base_shift == 'auto':
+        base_shift = base_shift_dict[pore + nucleotide_type + strand]
     else:
-        base_shift = 0
+        base_shift = base_shift
 
     fastq_file, bam_file = generate_bam_file(fastq_file, reference, cpu, subsample_ratio)
-    paf_file = generate_paf_file_resquiggle(fastq_file,slow5_file,pore,rna,cpu)
-    bam_file = pysam.AlignmentFile(bam_file,'rb')
-    info_dict = extract_pairs_pos(bam_file,position,length+base_shift,chrom,strand)
+    paf_file = generate_paf_file_resquiggle(fastq_file, slow5_file, pore, rna, cpu)
+    bam_file = pysam.AlignmentFile(bam_file, 'rb')
+    info_dict = extract_pairs_pos(bam_file, position, length + abs(kmer_model), chrom, strand)
     if info_dict == {}:
         raise RuntimeError("There is no read aligned on this position")
     info_df = pd.DataFrame(list(info_dict.keys()))
 
     s5 = pyslow5.Open(slow5_file, 'r')
-    df=pd.read_csv(paf_file,sep='\t',header=None)
-    df=pd.merge(df,info_df,how='inner',on=0)
+    df = pd.read_csv(paf_file, sep='\t', header=None)
+    df = pd.merge(df, info_df, how='inner', on=0)
     if df.shape[0] == 0:
         raise RuntimeError("cannot found the record from bam in your paf file. Please check your f5c command ... ")
     if df.shape[0] / info_df.shape[0] < 0.8:
-        print('There are '+str(info_df.shape[0]-df.shape[0])+" reads not found in your paf file ...")
+        print('There are ' + str(info_df.shape[0] - df.shape[0]) + " reads not found in your paf file ...")
     pbar = tqdm(total=df.shape[0], position=0, leave=True)
-    df["feature"] = df.apply(extract_feature,kmer_model=kmer_model,base_shift=base_shift,strand=strand,norm=norm,axis=1)
+    df["feature"] = df.apply(extract_feature,kmer_model=kmer_model, strand = strand,base_shift=base_shift, norm=norm, axis=1)
     pbar.close()
 
     df.dropna(inplace=True)
     num_aligned = df.shape[0]
-    if subsample_ratio<1:
-        df=df.sample(frac=subsample_ratio)
-    final_feature=[]
+    if subsample_ratio < 1:
+        df = df.sample(frac=subsample_ratio)
+    final_feature = []
     for item in df["feature"]:
         final_feature.extend(item)
-    final_feature=pd.DataFrame(final_feature)
-    final_feature.columns=['Read ID','Mean','STD','Median','Dwell time','Position']
-    final_feature = final_feature[(final_feature['Position']>=position-length)&(final_feature['Position']<=position+length)]
+    final_feature = pd.DataFrame(final_feature)
+    final_feature.columns = ['Read ID', 'Mean', 'STD', 'Median', 'Dwell time', 'Position']
+    final_feature = final_feature[
+        (final_feature['Position'] >= position - length) & (final_feature['Position'] <= position + length)]
 
     final_feature['Position'] = final_feature['Position'].astype(int).astype(str)
     print('Extracted ', num_aligned, ' aligned reads from blow5 files')
 
     # if num_aligned>50:
     #     dwell_filter_pctls = (0.5, 99.5)
     #     dwell_min, dwell_max = np.percentile(final_feature['Dwell time'].values, dwell_filter_pctls)
     #     final_feature = final_feature[(final_feature['Dwell time'] > dwell_min) & (final_feature['Dwell time'] < dwell_max)]
 
-    return final_feature,num_aligned,nucleotide_type
-
+    return final_feature, num_aligned, nucleotide_type
```

### Comparing `nanoCEM-0.0.5.4/nanoCEM/read_move_table.py` & `nanoCEM-0.0.5.5/nanoCEM/read_move_table.py`

 * *Files 0% similar despite different names*

```diff
@@ -76,15 +76,14 @@
     except Exception:
         print("Warning: 1 read's length of event is not equal between bam and paf file")
         return None
     # correct index about DNA and RNA
     if (nucleotide_type == 'RNA' and strand == '+') or (nucleotide_type == 'DNA' and strand == '-'):
         aligned_pair[0] = qlen - aligned_pair[0] - 1
 
-
     if aligned_pair.shape[0]==0:
         return None
     read_pos = aligned_pair[0].values
     ref_pos = aligned_pair[1].values
 
     # extract raw signal by event length and event start
     total_feature_per_reads = []
```

### Comparing `nanoCEM-0.0.5.4/nanoCEM/read_tombo_resquiggle.py` & `nanoCEM-0.0.5.5/nanoCEM/read_tombo_resquiggle.py`

 * *Files identical despite different names*

### Comparing `nanoCEM-0.0.5.4/nanoCEM.egg-info/PKG-INFO` & `nanoCEM-0.0.5.5/nanoCEM.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 Metadata-Version: 2.1
 Name: nanoCEM
-Version: 0.0.5.4
+Version: 0.0.5.5
 Summary: A simple tool designed to visualize the features that distinguish between two groups of ONT data at the site level.                It supports 4 re-squiggle program(tombo resquiggle/f5c resquiggle/f5c eventalign/move_table).
 Home-page: https://github.com/lrslab/nanoCEM
 Author: GUO Zhihao
 Author-email: qhuozhihao@icloud.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
-Requires-Python: >=3.7,<=3.11
+Requires-Python: >=3.7.0,<=3.11.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # nanoCEM ![logo](docs/logo_tiny.png "nanoCEM")
 <a href="https://pypi.python.org/pypi/nanoCEM" rel="pypi">![PyPI](https://img.shields.io/pypi/v/nanoCEM?color=green) </a>
 <a href="https://opensource.org/license/mit/" rel="license">![License](https://img.shields.io/pypi/l/nanoCEM?color=orange)</a>
 
@@ -42,15 +42,23 @@
     docker pull zhihaguo/nanocem_env
     
 To check the version of nanoCEM, run:
 
     pip list | grep nanoCEM
 
 
- **Notes:** Additionally, we do not rely on any re-squiggle or eventalign packages. We only need their index files for the sequencing data.
+## Solutions for some potential environment problem
+Although it does not affect the functionality, the issue of possible missing header files caused by **samtools** installation by conda can be resolved with the following command.
+
+    conda install -c conda-forge ncurses
+
+The potential **vbz** format compression issue when reading **fast5** files.
+
+    conda install -c bioconda ont_vbz_hdf_plugin
+
 
 
 ## Data release
 For the data we used and related commands in our paper, please view our [wiki](https://github.com/lrslab/nanoCEM/wiki/Data-release-and-commands)
 
 ## Documents
 Full documentation is available at https://nanocem.readthedocs.io/
```

#### html2text {}

```diff
@@ -1,16 +1,16 @@
-Metadata-Version: 2.1 Name: nanoCEM Version: 0.0.5.4 Summary: A simple tool
+Metadata-Version: 2.1 Name: nanoCEM Version: 0.0.5.5 Summary: A simple tool
 designed to visualize the features that distinguish between two groups of ONT
 data at the site level. It supports 4 re-squiggle program(tombo resquiggle/f5c
 resquiggle/f5c eventalign/move_table). Home-page: https://github.com/lrslab/
 nanoCEM Author: GUO Zhihao Author-email: qhuozhihao@icloud.com Classifier:
 Programming Language :: Python :: 3 Classifier: License :: OSI Approved :: MIT
 License Classifier: Operating System :: OS Independent Requires-Python:
->=3.7,<=3.11 Description-Content-Type: text/markdown License-File: LICENSE #
-nanoCEM ![logo](docs/logo_tiny.png "nanoCEM") _!_[_P_y_P_I_]_(_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/
+>=3.7.0,<=3.11.7 Description-Content-Type: text/markdown License-File: LICENSE
+# nanoCEM ![logo](docs/logo_tiny.png "nanoCEM") _!_[_P_y_P_I_]_(_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/
 _p_y_p_i_/_v_/_n_a_n_o_C_E_M_?_c_o_l_o_r_=_g_r_e_e_n_)_ _!_[_L_i_c_e_n_s_e_]_(_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_p_y_p_i_/_l_/
 _n_a_n_o_C_E_M_?_c_o_l_o_r_=_o_r_a_n_g_e_) The nanopore current events magnifier (`nanoCEM`) is a
 python command line to facilitate the analysis of DNA/RNA modification sites by
 visualizing statistical features of current events. NanoCEM can be used to
 showcase high confidence sites and observe the difference based on the
 modification sample and the low or no modification sample. It supports two re-
 squiggle pipeline(`Tombo` and `f5c`) and support `R9` and `R10`. If you want to
@@ -18,13 +18,16 @@
 hiruna72/squigualiser) is recommended. ## Installation Before pip install, make
 sure you have installed the `samtools`(>=1.16) , `f5c`(>=1.4), `slow5tools`
 (>=1.1.0) and `minimap2`(>=2.17), conda install samtools=1.16 minimap2 f5c=1.4
 slow5tools -c conda-forge -c bioconda To install the latest nanoCEM pip install
 nanoCEM And install from the resource git clone https://github.com/lrslab/
 nanoCEM.git cd nanoCEM/ pip install . To install nanoCEM from docker, docker
 pull zhihaguo/nanocem_env To check the version of nanoCEM, run: pip list | grep
-nanoCEM **Notes:** Additionally, we do not rely on any re-squiggle or
-eventalign packages. We only need their index files for the sequencing data. ##
-Data release For the data we used and related commands in our paper, please
-view our [wiki](https://github.com/lrslab/nanoCEM/wiki/Data-release-and-
-commands) ## Documents Full documentation is available at https://
+nanoCEM ## Solutions for some potential environment problem Although it does
+not affect the functionality, the issue of possible missing header files caused
+by **samtools** installation by conda can be resolved with the following
+command. conda install -c conda-forge ncurses The potential **vbz** format
+compression issue when reading **fast5** files. conda install -c bioconda
+ont_vbz_hdf_plugin ## Data release For the data we used and related commands in
+our paper, please view our [wiki](https://github.com/lrslab/nanoCEM/wiki/Data-
+release-and-commands) ## Documents Full documentation is available at https://
 nanocem.readthedocs.io/ ## Workflow ![workflow](docs/Workflow.png)
```

### Comparing `nanoCEM-0.0.5.4/nanoCEM.egg-info/SOURCES.txt` & `nanoCEM-0.0.5.5/nanoCEM.egg-info/SOURCES.txt`

 * *Files 7% similar despite different names*

```diff
@@ -17,14 +17,15 @@
 nanoCEM/machine_learning_trainer.py
 nanoCEM/normalization.py
 nanoCEM/plot.py
 nanoCEM/read_f5c_eventalign.py
 nanoCEM/read_f5c_resquiggle.py
 nanoCEM/read_move_table.py
 nanoCEM/read_tombo_resquiggle.py
+nanoCEM/squigualiser_utils.py
 nanoCEM.egg-info/PKG-INFO
 nanoCEM.egg-info/SOURCES.txt
 nanoCEM.egg-info/dependency_links.txt
 nanoCEM.egg-info/requires.txt
 nanoCEM.egg-info/top_level.txt
 nanoCEM/f5c_result_rna/__init__.py
 nanoCEM/f5c_result_rna/test.py
```

### Comparing `nanoCEM-0.0.5.4/setup.py` & `nanoCEM-0.0.5.5/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setup(
     name="nanoCEM",
-    version="0.0.5.4",
+    version="0.0.5.5",
     author="GUO Zhihao",
     author_email="qhuozhihao@icloud.com",
     description='A simple tool designed to visualize the features that distinguish between two groups of ONT data at the site level.\
                 It supports 4 re-squiggle program(tombo resquiggle/f5c resquiggle/f5c eventalign/move_table).',
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/lrslab/nanoCEM",
     packages=find_packages(),
     classifiers=[
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent",
     ],
-    python_requires='>=3.7,<=3.11',
+    python_requires='>=3.7.0,<=3.11.7',
     install_requires=[
         'h5py>=3.8.0',
         'numpy>=1.23.0',
         'pandas>=1.5.0',
         'plotnine==0.12.4',
         'tqdm>=4.62.0',
         "pysam>=0.21.0",
```

