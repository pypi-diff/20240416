# Comparing `tmp/track2p-0.5.0.tar.gz` & `tmp/track2p-0.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "track2p-0.5.0.tar", last modified: Fri Mar 22 14:44:31 2024, max compression
+gzip compressed data, was "track2p-0.5.1.tar", last modified: Tue Apr 16 15:14:01 2024, max compression
```

## Comparing `track2p-0.5.0.tar` & `track2p-0.5.1.tar`

### file list

```diff
@@ -1,49 +1,48 @@
-drwxr-xr-x   0 manonmantez   (501) staff       (20)        0 2024-03-22 14:44:31.973271 track2p-0.5.0/
--rw-r--r--   0 manonmantez   (501) staff       (20)    35149 2024-02-12 15:58:33.000000 track2p-0.5.0/LICENSE
--rw-r--r--   0 manonmantez   (501) staff       (20)     4308 2024-03-22 14:44:31.972951 track2p-0.5.0/PKG-INFO
--rw-r--r--   0 manonmantez   (501) staff       (20)     3910 2024-03-22 13:46:13.000000 track2p-0.5.0/README.md
--rw-r--r--   0 manonmantez   (501) staff       (20)       38 2024-03-22 14:44:31.973331 track2p-0.5.0/setup.cfg
--rw-r--r--   0 manonmantez   (501) staff       (20)      565 2024-03-22 14:40:51.000000 track2p-0.5.0/setup.py
-drwxr-xr-x   0 manonmantez   (501) staff       (20)        0 2024-03-22 14:44:31.963176 track2p-0.5.0/track2p/
--rw-r--r--   0 manonmantez   (501) staff       (20)       48 2024-02-22 09:56:18.000000 track2p-0.5.0/track2p/__init__.py
--rw-r--r--   0 manonmantez   (501) staff       (20)      417 2024-02-21 12:46:39.000000 track2p-0.5.0/track2p/__main__.py
-drwxr-xr-x   0 manonmantez   (501) staff       (20)        0 2024-03-22 14:44:31.967462 track2p-0.5.0/track2p/gui/
--rw-r--r--   0 manonmantez   (501) staff       (20)        0 2024-02-21 13:37:36.000000 track2p-0.5.0/track2p/gui/__init__.py
--rw-r--r--   0 manonmantez   (501) staff       (20)     6753 2024-02-29 09:44:51.000000 track2p-0.5.0/track2p/gui/cell_plot.py
--rw-r--r--   0 manonmantez   (501) staff       (20)     6512 2024-02-28 15:48:00.000000 track2p-0.5.0/track2p/gui/fluo_plot.py
--rw-r--r--   0 manonmantez   (501) staff       (20)     1965 2024-03-22 14:24:14.000000 track2p-0.5.0/track2p/gui/import_wd.py
--rw-r--r--   0 manonmantez   (501) staff       (20)    14151 2024-03-22 14:40:51.000000 track2p-0.5.0/track2p/gui/main_wd.py
--rw-r--r--   0 manonmantez   (501) staff       (20)    15242 2024-03-22 14:40:51.000000 track2p-0.5.0/track2p/gui/raster_wd.py
--rw-r--r--   0 manonmantez   (501) staff       (20)     8261 2024-03-06 14:04:13.000000 track2p-0.5.0/track2p/gui/roi_plot.py
--rw-r--r--   0 manonmantez   (501) staff       (20)      372 2024-02-20 14:31:45.000000 track2p-0.5.0/track2p/gui/run_gui.py
--rw-r--r--   0 manonmantez   (501) staff       (20)     8984 2024-03-22 14:40:51.000000 track2p-0.5.0/track2p/gui/t2p_wd.py
-drwxr-xr-x   0 manonmantez   (501) staff       (20)        0 2024-03-22 14:44:31.968779 track2p-0.5.0/track2p/io/
--rw-r--r--   0 manonmantez   (501) staff       (20)        0 2024-02-21 13:37:36.000000 track2p-0.5.0/track2p/io/__init__.py
--rw-r--r--   0 manonmantez   (501) staff       (20)     1781 2024-03-22 13:46:13.000000 track2p-0.5.0/track2p/io/loaders.py
--rw-r--r--   0 manonmantez   (501) staff       (20)     4309 2024-03-22 13:46:13.000000 track2p-0.5.0/track2p/io/s2p_loaders.py
--rw-r--r--   0 manonmantez   (501) staff       (20)      773 2024-02-12 11:04:52.000000 track2p-0.5.0/track2p/io/savers.py
--rw-r--r--   0 manonmantez   (501) staff       (20)      252 2024-01-09 12:56:24.000000 track2p-0.5.0/track2p/io/utils.py
-drwxr-xr-x   0 manonmantez   (501) staff       (20)        0 2024-03-22 14:44:31.969750 track2p-0.5.0/track2p/match/
--rw-r--r--   0 manonmantez   (501) staff       (20)        0 2024-02-21 13:37:36.000000 track2p-0.5.0/track2p/match/__init__.py
--rw-r--r--   0 manonmantez   (501) staff       (20)     4471 2024-01-09 12:56:24.000000 track2p-0.5.0/track2p/match/loop.py
--rw-r--r--   0 manonmantez   (501) staff       (20)     5890 2024-03-01 14:53:03.000000 track2p-0.5.0/track2p/match/utils.py
-drwxr-xr-x   0 manonmantez   (501) staff       (20)        0 2024-03-22 14:44:31.970241 track2p-0.5.0/track2p/ops/
--rw-r--r--   0 manonmantez   (501) staff       (20)        0 2024-02-21 13:37:36.000000 track2p-0.5.0/track2p/ops/__init__.py
--rw-r--r--   0 manonmantez   (501) staff       (20)     2904 2024-02-12 15:58:23.000000 track2p-0.5.0/track2p/ops/default.py
-drwxr-xr-x   0 manonmantez   (501) staff       (20)        0 2024-03-22 14:44:31.971420 track2p-0.5.0/track2p/plot/
--rw-r--r--   0 manonmantez   (501) staff       (20)        0 2024-02-21 13:37:36.000000 track2p-0.5.0/track2p/plot/__init__.py
--rw-r--r--   0 manonmantez   (501) staff       (20)    15369 2024-02-12 11:04:52.000000 track2p-0.5.0/track2p/plot/output.py
--rw-r--r--   0 manonmantez   (501) staff       (20)      926 2024-02-12 11:04:52.000000 track2p-0.5.0/track2p/plot/progress.py
--rw-r--r--   0 manonmantez   (501) staff       (20)     1859 2024-02-12 11:04:52.000000 track2p-0.5.0/track2p/plot/utils.py
-drwxr-xr-x   0 manonmantez   (501) staff       (20)        0 2024-03-22 14:44:31.972423 track2p-0.5.0/track2p/register/
--rw-r--r--   0 manonmantez   (501) staff       (20)        0 2024-02-21 13:37:36.000000 track2p-0.5.0/track2p/register/__init__.py
--rw-r--r--   0 manonmantez   (501) staff       (20)     1348 2024-01-10 11:16:47.000000 track2p-0.5.0/track2p/register/elastix.py
--rw-r--r--   0 manonmantez   (501) staff       (20)     4054 2024-01-09 12:56:24.000000 track2p-0.5.0/track2p/register/loop.py
--rw-r--r--   0 manonmantez   (501) staff       (20)     2345 2024-01-09 12:56:24.000000 track2p-0.5.0/track2p/register/utils.py
--rw-r--r--   0 manonmantez   (501) staff       (20)     3521 2024-03-20 14:50:27.000000 track2p-0.5.0/track2p/t2p.py
-drwxr-xr-x   0 manonmantez   (501) staff       (20)        0 2024-03-22 14:44:31.964231 track2p-0.5.0/track2p.egg-info/
--rw-r--r--   0 manonmantez   (501) staff       (20)     4308 2024-03-22 14:44:31.000000 track2p-0.5.0/track2p.egg-info/PKG-INFO
--rw-r--r--   0 manonmantez   (501) staff       (20)      884 2024-03-22 14:44:31.000000 track2p-0.5.0/track2p.egg-info/SOURCES.txt
--rw-r--r--   0 manonmantez   (501) staff       (20)        1 2024-03-22 14:44:31.000000 track2p-0.5.0/track2p.egg-info/dependency_links.txt
--rw-r--r--   0 manonmantez   (501) staff       (20)      149 2024-03-22 14:44:31.000000 track2p-0.5.0/track2p.egg-info/requires.txt
--rw-r--r--   0 manonmantez   (501) staff       (20)        8 2024-03-22 14:44:31.000000 track2p-0.5.0/track2p.egg-info/top_level.txt
+drwxr-xr-x   0 manonmantez   (501) staff       (20)        0 2024-04-16 15:14:01.009960 track2p-0.5.1/
+-rw-r--r--   0 manonmantez   (501) staff       (20)    35149 2024-02-12 15:58:33.000000 track2p-0.5.1/LICENSE
+-rw-r--r--   0 manonmantez   (501) staff       (20)     5073 2024-04-16 15:14:01.009626 track2p-0.5.1/PKG-INFO
+-rw-r--r--   0 manonmantez   (501) staff       (20)     4646 2024-04-16 14:56:02.000000 track2p-0.5.1/README.md
+-rw-r--r--   0 manonmantez   (501) staff       (20)       38 2024-04-16 15:14:01.010021 track2p-0.5.1/setup.cfg
+-rw-r--r--   0 manonmantez   (501) staff       (20)      591 2024-04-16 15:13:05.000000 track2p-0.5.1/setup.py
+drwxr-xr-x   0 manonmantez   (501) staff       (20)        0 2024-04-16 15:14:01.000571 track2p-0.5.1/track2p/
+-rw-r--r--   0 manonmantez   (501) staff       (20)       48 2024-02-22 09:56:18.000000 track2p-0.5.1/track2p/__init__.py
+-rw-r--r--   0 manonmantez   (501) staff       (20)      417 2024-02-21 12:46:39.000000 track2p-0.5.1/track2p/__main__.py
+drwxr-xr-x   0 manonmantez   (501) staff       (20)        0 2024-04-16 15:14:01.004501 track2p-0.5.1/track2p/gui/
+-rw-r--r--   0 manonmantez   (501) staff       (20)        0 2024-02-21 13:37:36.000000 track2p-0.5.1/track2p/gui/__init__.py
+-rw-r--r--   0 manonmantez   (501) staff       (20)     8413 2024-04-16 14:56:02.000000 track2p-0.5.1/track2p/gui/cell_plot.py
+-rw-r--r--   0 manonmantez   (501) staff       (20)     6456 2024-04-16 14:56:02.000000 track2p-0.5.1/track2p/gui/fluo_plot.py
+-rw-r--r--   0 manonmantez   (501) staff       (20)     2622 2024-04-16 14:56:02.000000 track2p-0.5.1/track2p/gui/import_wd.py
+-rw-r--r--   0 manonmantez   (501) staff       (20)    22751 2024-04-16 14:56:02.000000 track2p-0.5.1/track2p/gui/main_wd.py
+-rw-r--r--   0 manonmantez   (501) staff       (20)    15418 2024-04-16 14:56:02.000000 track2p-0.5.1/track2p/gui/raster_wd.py
+-rw-r--r--   0 manonmantez   (501) staff       (20)     8677 2024-04-16 14:56:02.000000 track2p-0.5.1/track2p/gui/roi_plot.py
+-rw-r--r--   0 manonmantez   (501) staff       (20)    10427 2024-04-16 14:56:02.000000 track2p-0.5.1/track2p/gui/t2p_wd.py
+drwxr-xr-x   0 manonmantez   (501) staff       (20)        0 2024-04-16 15:14:01.005757 track2p-0.5.1/track2p/io/
+-rw-r--r--   0 manonmantez   (501) staff       (20)        0 2024-02-21 13:37:36.000000 track2p-0.5.1/track2p/io/__init__.py
+-rw-r--r--   0 manonmantez   (501) staff       (20)     1726 2024-04-16 14:56:02.000000 track2p-0.5.1/track2p/io/loaders.py
+-rw-r--r--   0 manonmantez   (501) staff       (20)     4238 2024-04-16 14:56:02.000000 track2p-0.5.1/track2p/io/s2p_loaders.py
+-rw-r--r--   0 manonmantez   (501) staff       (20)      773 2024-02-12 11:04:52.000000 track2p-0.5.1/track2p/io/savers.py
+-rw-r--r--   0 manonmantez   (501) staff       (20)      252 2024-01-09 12:56:24.000000 track2p-0.5.1/track2p/io/utils.py
+drwxr-xr-x   0 manonmantez   (501) staff       (20)        0 2024-04-16 15:14:01.006576 track2p-0.5.1/track2p/match/
+-rw-r--r--   0 manonmantez   (501) staff       (20)        0 2024-02-21 13:37:36.000000 track2p-0.5.1/track2p/match/__init__.py
+-rw-r--r--   0 manonmantez   (501) staff       (20)     4471 2024-01-09 12:56:24.000000 track2p-0.5.1/track2p/match/loop.py
+-rw-r--r--   0 manonmantez   (501) staff       (20)     5807 2024-04-16 14:56:02.000000 track2p-0.5.1/track2p/match/utils.py
+drwxr-xr-x   0 manonmantez   (501) staff       (20)        0 2024-04-16 15:14:01.006976 track2p-0.5.1/track2p/ops/
+-rw-r--r--   0 manonmantez   (501) staff       (20)        0 2024-02-21 13:37:36.000000 track2p-0.5.1/track2p/ops/__init__.py
+-rw-r--r--   0 manonmantez   (501) staff       (20)     3348 2024-04-16 14:56:02.000000 track2p-0.5.1/track2p/ops/default.py
+drwxr-xr-x   0 manonmantez   (501) staff       (20)        0 2024-04-16 15:14:01.007909 track2p-0.5.1/track2p/plot/
+-rw-r--r--   0 manonmantez   (501) staff       (20)        0 2024-02-21 13:37:36.000000 track2p-0.5.1/track2p/plot/__init__.py
+-rw-r--r--   0 manonmantez   (501) staff       (20)    15443 2024-04-16 14:56:02.000000 track2p-0.5.1/track2p/plot/output.py
+-rw-r--r--   0 manonmantez   (501) staff       (20)      926 2024-02-12 11:04:52.000000 track2p-0.5.1/track2p/plot/progress.py
+-rw-r--r--   0 manonmantez   (501) staff       (20)     1859 2024-02-12 11:04:52.000000 track2p-0.5.1/track2p/plot/utils.py
+drwxr-xr-x   0 manonmantez   (501) staff       (20)        0 2024-04-16 15:14:01.009057 track2p-0.5.1/track2p/register/
+-rw-r--r--   0 manonmantez   (501) staff       (20)        0 2024-02-21 13:37:36.000000 track2p-0.5.1/track2p/register/__init__.py
+-rw-r--r--   0 manonmantez   (501) staff       (20)     1348 2024-01-10 11:16:47.000000 track2p-0.5.1/track2p/register/elastix.py
+-rw-r--r--   0 manonmantez   (501) staff       (20)     4054 2024-01-09 12:56:24.000000 track2p-0.5.1/track2p/register/loop.py
+-rw-r--r--   0 manonmantez   (501) staff       (20)     2345 2024-01-09 12:56:24.000000 track2p-0.5.1/track2p/register/utils.py
+-rw-r--r--   0 manonmantez   (501) staff       (20)     9791 2024-04-16 14:56:02.000000 track2p-0.5.1/track2p/t2p.py
+drwxr-xr-x   0 manonmantez   (501) staff       (20)        0 2024-04-16 15:14:01.001743 track2p-0.5.1/track2p.egg-info/
+-rw-r--r--   0 manonmantez   (501) staff       (20)     5073 2024-04-16 15:14:00.000000 track2p-0.5.1/track2p.egg-info/PKG-INFO
+-rw-r--r--   0 manonmantez   (501) staff       (20)      861 2024-04-16 15:14:00.000000 track2p-0.5.1/track2p.egg-info/SOURCES.txt
+-rw-r--r--   0 manonmantez   (501) staff       (20)        1 2024-04-16 15:14:00.000000 track2p-0.5.1/track2p.egg-info/dependency_links.txt
+-rw-r--r--   0 manonmantez   (501) staff       (20)      163 2024-04-16 15:14:00.000000 track2p-0.5.1/track2p.egg-info/requires.txt
+-rw-r--r--   0 manonmantez   (501) staff       (20)        8 2024-04-16 15:14:00.000000 track2p-0.5.1/track2p.egg-info/top_level.txt
```

### Comparing `track2p-0.5.0/LICENSE` & `track2p-0.5.1/LICENSE`

 * *Files identical despite different names*

### Comparing `track2p-0.5.0/PKG-INFO` & `track2p-0.5.1/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 Metadata-Version: 2.1
 Name: track2p
-Version: 0.5.0
+Version: 0.5.1
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: numpy==1.23.5
 Requires-Dist: matplotlib==3.5.3
 Requires-Dist: scikit-image==0.20.0
 Requires-Dist: itk-elastix==0.19.1
 Requires-Dist: PyQt5==5.15.10
 Requires-Dist: qtpy==2.4.1
 Requires-Dist: tqdm==4.66.2
 Requires-Dist: scikit-learn==1.4.0
 Requires-Dist: openTSNE==1.0.1
+Requires-Dist: pandas==1.5.3
 
 # track2p
 Cell tracking for longitudinal calcium imaging recordings.
 
 [![PyPI version](https://img.shields.io/pypi/v/track2p)](https://pypi.org/project/track2p/)
 [![All time downloads](https://static.pepy.tech/badge/track2p)](https://pepy.tech/project/track2p)
 [![Monthly downloads](https://img.shields.io/pypi/dm/track2p)](https://pypi.org/project/track2p/)
@@ -50,51 +51,59 @@
 python -m track2p
 ```
 
 This opens a GUI allowing the user to launch the algorithm and visualise the results interactively.
 
 (For instructions on running track2p without the GUI see the 'Run via script' under the 'Usage' section)
 
+Note: For common installation issues see [documentation](https://github.com/juremaj/track2p/blob/main/docs/installation.md).
+
 # Usage
 
 ## Run through GUI
 
 After activating the GUI through `python -m track2p` the user should navigate to the 'Run' tab on the top left of the window and select 'Run algorithm' from the dropdown menu. This will open a pop-up window that will allow the user to set the paths to suite2p datasets and to set the algorithm parameters. Once these have been set the user can click on 'Run', which will launch the track2p algorithm, with the progress being printed in the window below.
 
-When the algorithm is finished, another pop-up window will appear, asking the user if they want to visualise the outputs in the GUI (for more information see section below).
+When the algorithm is finished, another pop-up window will appear, asking the user if they want to visualise the outputs in the GUI.
+
+For more details on how to run the algorithm through the GUI see [documentation](https://github.com/juremaj/track2p/blob/main/docs/gui.md) and for more description of paramters see documentation [here](https://github.com/juremaj/track2p/blob/main/docs/parameters.md).
 
 ## GUI visualisation
 
 
 The GUI supports both visualisation after algorithm run (as described above), as well as visualising previously processed data. The latter can be done by navigating to File -> Load processed data on the top left of the GUI.
 
 
 ![gui_mainwindow.png](docs/media/plots/gui_mainwindow.png)
 
 Briefly the GUI allows the user to visualise the mean field of view on all days, with the ROIs of all matched cells visualised. The user can then interactively select a cell by clicking on the ROI on the mean image. This will display a zoomed-in view of this cell across all days on the right, and the extracted fluorescence time series below.
 
+For more details on how to use the GUI for visualising track2p results see [documentation](https://github.com/juremaj/track2p/blob/main/docs/gui.md).
+
 ## Run via script
 
 To run via script you can use the `run_track2p.py` script in the root of this repo as a template. It is exactly the same as running thrugh the gui, only that the paths and the parameters are defined within the script (for more on parameters etc. see documentation). When running make sure you are running it within the track2p environment, for example:
 
 ```
 conda activate track2p
 python -m run_track2p
 ```
 
 # Outputs
 
-All the outputs of the script will be saved in a `track2p` folder created within the `track_ops.save_path` directory specified by the user when running the algorithm. For an introduction on how to use the outputs for further downstream analysis we provide a useful demo notebook `demo_t2p_outlput.ipynb` in the root of this repository. Note: You will need to additionally install jupyter for this to work. For example:
+All the outputs of the script will be saved in a `track2p` folder created within the `track_ops.save_path` directory specified by the user when running the algorithm. For an introduction on how to use the outputs for further downstream analysis we provide a useful demo notebook `demo_t2p_output.ipynb` in the root of this repository. Note: You will need to additionally install jupyter for this to work. For example:
 
 ```
 conda install conda-forge::jupyterlab
 ```
 
+For more information see documentation relating to track2p [viusalisations](https://github.com/juremaj/track2p/blob/main/docs/visualisations.md) and [outputs](https://github.com/juremaj/track2p/blob/main/docs/outputs.md).
+
 # Reference
 
 For now if you use the algorithm please reference the Cosyne abstract:
 
-  **Majnik, J., Zangila, S., Cossart, R. & Platel, J. C. (2024). _Emergence of state modulation in a developing circuit_. COSYNE Abstract.**
+  **Majnik, J., Zangila, S., Cossart, R. & Platel, J. C. (2024). _Emergence of state modulation in a developing cortical circuit_. COSYNE Abstract.**
 
   
 
 You can also see the YouTube recording of the talk for a reference use-case in neocortical development: [Link to video (starting at 47:20)](https://youtu.be/Tr97HwgQ9ik?t=2839)
```

### Comparing `track2p-0.5.0/README.md` & `track2p-0.5.1/README.md`

 * *Files 16% similar despite different names*

```diff
@@ -35,51 +35,59 @@
 python -m track2p
 ```
 
 This opens a GUI allowing the user to launch the algorithm and visualise the results interactively.
 
 (For instructions on running track2p without the GUI see the 'Run via script' under the 'Usage' section)
 
+Note: For common installation issues see [documentation](https://github.com/juremaj/track2p/blob/main/docs/installation.md).
+
 # Usage
 
 ## Run through GUI
 
 After activating the GUI through `python -m track2p` the user should navigate to the 'Run' tab on the top left of the window and select 'Run algorithm' from the dropdown menu. This will open a pop-up window that will allow the user to set the paths to suite2p datasets and to set the algorithm parameters. Once these have been set the user can click on 'Run', which will launch the track2p algorithm, with the progress being printed in the window below.
 
-When the algorithm is finished, another pop-up window will appear, asking the user if they want to visualise the outputs in the GUI (for more information see section below).
+When the algorithm is finished, another pop-up window will appear, asking the user if they want to visualise the outputs in the GUI.
+
+For more details on how to run the algorithm through the GUI see [documentation](https://github.com/juremaj/track2p/blob/main/docs/gui.md) and for more description of paramters see documentation [here](https://github.com/juremaj/track2p/blob/main/docs/parameters.md).
 
 ## GUI visualisation
 
 
 The GUI supports both visualisation after algorithm run (as described above), as well as visualising previously processed data. The latter can be done by navigating to File -> Load processed data on the top left of the GUI.
 
 
 ![gui_mainwindow.png](docs/media/plots/gui_mainwindow.png)
 
 Briefly the GUI allows the user to visualise the mean field of view on all days, with the ROIs of all matched cells visualised. The user can then interactively select a cell by clicking on the ROI on the mean image. This will display a zoomed-in view of this cell across all days on the right, and the extracted fluorescence time series below.
 
+For more details on how to use the GUI for visualising track2p results see [documentation](https://github.com/juremaj/track2p/blob/main/docs/gui.md).
+
 ## Run via script
 
 To run via script you can use the `run_track2p.py` script in the root of this repo as a template. It is exactly the same as running thrugh the gui, only that the paths and the parameters are defined within the script (for more on parameters etc. see documentation). When running make sure you are running it within the track2p environment, for example:
 
 ```
 conda activate track2p
 python -m run_track2p
 ```
 
 # Outputs
 
-All the outputs of the script will be saved in a `track2p` folder created within the `track_ops.save_path` directory specified by the user when running the algorithm. For an introduction on how to use the outputs for further downstream analysis we provide a useful demo notebook `demo_t2p_outlput.ipynb` in the root of this repository. Note: You will need to additionally install jupyter for this to work. For example:
+All the outputs of the script will be saved in a `track2p` folder created within the `track_ops.save_path` directory specified by the user when running the algorithm. For an introduction on how to use the outputs for further downstream analysis we provide a useful demo notebook `demo_t2p_output.ipynb` in the root of this repository. Note: You will need to additionally install jupyter for this to work. For example:
 
 ```
 conda install conda-forge::jupyterlab
 ```
 
+For more information see documentation relating to track2p [viusalisations](https://github.com/juremaj/track2p/blob/main/docs/visualisations.md) and [outputs](https://github.com/juremaj/track2p/blob/main/docs/outputs.md).
+
 # Reference
 
 For now if you use the algorithm please reference the Cosyne abstract:
 
-  **Majnik, J., Zangila, S., Cossart, R. & Platel, J. C. (2024). _Emergence of state modulation in a developing circuit_. COSYNE Abstract.**
+  **Majnik, J., Zangila, S., Cossart, R. & Platel, J. C. (2024). _Emergence of state modulation in a developing cortical circuit_. COSYNE Abstract.**
 
   
 
 You can also see the YouTube recording of the talk for a reference use-case in neocortical development: [Link to video (starting at 47:20)](https://youtu.be/Tr97HwgQ9ik?t=2839)
```

### Comparing `track2p-0.5.0/setup.py` & `track2p-0.5.1/setup.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,23 +1,24 @@
 from setuptools import find_packages, setup
 
 with open('README.md', 'r') as f:
     long_description = f.read()
 
 setup(
     name='track2p',
-    version='0.5.0',
+    version='0.5.1',
     packages=find_packages(),
     install_requires=[
         'numpy==1.23.5',
         'matplotlib==3.5.3',
         'scikit-image==0.20.0',
         'itk-elastix==0.19.1',
         'PyQt5==5.15.10',
         'qtpy==2.4.1',
         'tqdm==4.66.2',
         'scikit-learn==1.4.0',
-        'openTSNE==1.0.1'
+        'openTSNE==1.0.1',
+        'pandas==1.5.3',
         ],
     long_description=long_description,
     long_description_content_type='text/markdown'
     )
```

### Comparing `track2p-0.5.0/track2p/gui/cell_plot.py` & `track2p-0.5.1/track2p/gui/cell_plot.py`

 * *Files 18% similar despite different names*

```diff
@@ -7,26 +7,27 @@
 
 class CellPlotWidget(FigureCanvas):
     '''This class is used to view and interact with the mean image of each recording (day). There is one instance of this class per recording. The instance of this class is created in the MainWindow class.
     It also allows to select a cell and display its fluorescence and zooms across days. The cell selected signal is emitted when a cell is selected.'''
     cell_selected = Signal(int)
 
     def __init__(self, tab=None, ops=None, stat_t2p=None, f_t2p=None, colors=None, update_selection_callback=None,
-                 all_fluorescence=None, all_stat_t2p=None, all_ops=None):
+                 all_f_t2p=None, all_stat_t2p=None, all_ops=None, initial_colors=None):
         """It initializes the class attributes and connects certain events to their respective handlers. It also creates the figure and the axes to display the mean image of the recording."""
         self.fig, self.ax_image = plt.subplots(1, 1) 
         self.fig.set_facecolor('black')
         super().__init__(self.fig)
         self.ops = ops
         self.stat_t2p = stat_t2p
         self.f_t2p = f_t2p
-        self.all_fluorescence = all_fluorescence
+        self.all_fluorescence = all_f_t2p
         self.all_stat_t2p=all_stat_t2p
         self.all_ops=all_ops
         self.colors = colors
+        self.initial_colors=initial_colors
         self.selected_cell_index = None
         self.mpl_connect('button_press_event', self.on_mouse_press)
         self.update_selection_callback = update_selection_callback
         self.nb_cells= len(self.stat_t2p)
         self.plot_cells()
         self.initialize_interactions()
         
@@ -39,38 +40,65 @@
         match_mean_img=skimage.exposure.match_histograms(self.ops['meanImg'], l_mean_img, channel_axis=None)
         self.ax_image.imshow(match_mean_img, cmap='gray')
         
         for cell in range(self.nb_cells):
             bin_mask = np.zeros_like(self.ops['meanImg']) #create a binary mask with the same shape as the mean image of the recording
             bin_mask[self.stat_t2p[cell]['ypix'], self.stat_t2p[cell]['xpix']] = 1
             color_cell=self.colors[cell]
+           
             self.ax_image.contour(bin_mask, levels=[0.5], colors=[color_cell], linewidths=1) 
         self.ax_image.axis('off')
         print(f'time for plotting cells on mean image for recording : {time.time()-start}')
         self.draw()
-
-
+        
            
+    def underline_cell_remix(self,selected_cell_index,vector_curation):
+        
+        for cell in range(self.nb_cells):
+            if cell == selected_cell_index:
+                bin_mask = np.zeros_like(self.ops['meanImg'])
+                if vector_curation[selected_cell_index] in [3,4]:
+                    bin_mask[self.stat_t2p[cell]['ypix'], self.stat_t2p[cell]['xpix']] = 1 
+                    color_cell = (0.4, 0.4, 0.4)
+                    self.colors[cell]=(0.4, 0.4, 0.4)
+                   # color_cell = (0.0, 0.0, 0.0)
+                   # self.colors[cell]=(0.0, 0.0, 0.0) #update colors of plor and fluo  
+                    
+                if vector_curation[selected_cell_index]==2:
+                    bin_mask[self.stat_t2p[cell]['ypix'], self.stat_t2p[cell]['xpix']] = 1 
+                    color_cell =(0.78, 0.78, 0.78)
+                    self.colors[cell]=(0.78, 0.78, 0.78)
+                   # color_cell = (0.4, 0.4, 0.4)
+                   # self.colors[cell]=(0.4, 0.4, 0.4) #update colors of plor and fluo 
+                if vector_curation[selected_cell_index]==1: 
+                    bin_mask[self.stat_t2p[cell]['ypix'], self.stat_t2p[cell]['xpix']] = 1 
+                    color_cell=self.initial_colors[cell]
+                    self.colors[cell]=self.initial_colors[cell] #update colors of plor and fluo  
+                self.ax_image.contour(bin_mask, levels=[0.5], colors=[color_cell], linewidths=1)
+                self.ax_image.contour(bin_mask, levels=[0.5], colors=[color_cell], linewidths=3) #update mean image 
+        self.draw() 
+    
+   
+        
     def underline_cell(self,selected_cell_index):
         """It underlines the selected cell by increasing the linewidth of the contour of the cell"""
         for cell in range(self.nb_cells):
             if cell == selected_cell_index:
                 bin_mask = np.zeros_like(self.ops['meanImg']) 
                 bin_mask[self.stat_t2p[cell]['ypix'], self.stat_t2p[cell]['xpix']] = 1 
                 color_cell=self.colors[cell]
                 self.ax_image.contour(bin_mask, levels=[0.5], colors=[color_cell], linewidths=3)
         self.draw() 
     
     def remove_previous_underline(self):
         """It removes the underline of the previously selected cell by decreasing the linewidth of the contour of the cell."""
         for collection in self.ax_image.collections:
-            collection.set_linewidth(1)   
-        self.draw() # important, don't forget it ! (update the plot)
-                
-    
+            collection.set_linewidth(1)
+         # important, don't forget it ! (update the plot)
+            
     def initialize_interactions(self):
         """This method is used to initialize user interactions with the mean image. It connects the scroll event to the on_scroll method and records the initial xlim and ylim of the mean image."""
         self.cid_scroll = self.fig.canvas.mpl_connect('scroll_event', self.on_scroll)
         self.initial_xlim = self.ax_image.get_xlim()
         self.initial_ylim = self.ax_image.get_ylim()
 
     def on_scroll(self, event):
@@ -101,11 +129,12 @@
             x, y = event.xdata, event.ydata
             for j, cell_info in enumerate(self.stat_t2p):
                 ypix = cell_info['ypix'] #ypix are the y coordinates of the pixels of the cell
                 xpix = cell_info['xpix'] #xpix are the x coordinates of the pixels of the cell
                 if np.any((xpix == int(x)) & (ypix == int(y))):
                     self.selected_cell_index = j
                     self.update_selection_callback(j)
-                    print(f"Cell selected: {j + 1}", flush=True)
+                    print(f"Cell selected: {j}", flush=True)
                     break
         print(f'time taken for updating: {time.time()-start}')
         
+
```

### Comparing `track2p-0.5.0/track2p/gui/fluo_plot.py` & `track2p-0.5.1/track2p/gui/fluo_plot.py`

 * *Files 14% similar despite different names*

```diff
@@ -7,18 +7,18 @@
 import matplotlib.patches as patches
 from PyQt5 import QtCore
 
 
 
 class FluorescencePlotWidget(FigureCanvas):
     """this class is used to display the fluorescence of the selected cell across days. It also allows to select a region of interest (ROI) on the fluorescence plot and zoom in on the selected ROI"""
-    def __init__(self, all_fluorescence=None, all_ops=None, colors=None, all_stat_t2p=None):
+    def __init__(self, all_f_t2p=None, all_ops=None, colors=None, all_stat_t2p=None):
         self.fig, self.ax_fluorescence = plt.subplots(1, 1)
         super().__init__(self.fig)
-        self.all_fluorescence = all_fluorescence
+        self.all_f_t2p = all_f_t2p
         self.all_ops=all_ops
         self.fig.set_facecolor('black')
         self.colors = colors
         self.all_stat_t2p= all_stat_t2p
         
         self.rect = patches.Rectangle((0,0), 1, 1, color='white', linewidth=2) 
         
@@ -79,45 +79,45 @@
             self.ax_fluorescence.set_xlim(self.x0, self.x1)
             self.ax_fluorescence.set_ylim(self.y0, self.y1)
             self.rect.set_visible(False) 
             self.point.set_visible(False)
             self.fig.canvas.draw()
 
 
-    def display_all_fluorescence(self, selected_cell_index):
+    def display_all_f_t2p(self, selected_cell_index):
         """it plots the fluroescence of the selected cell across days where each curve being a different day (the curve at the top of the plot is the first day)"""
         
-        if self.all_fluorescence is not None and selected_cell_index is not None:
+        if self.all_f_t2p is not None and selected_cell_index is not None:
             self.ax_fluorescence.clear()
             self.ax_fluorescence.set_facecolor('black')
             self.ax_fluorescence.tick_params(axis='x', colors='white') 
             self.ax_fluorescence.tick_params(axis='y', colors='white')  
             self.ax_fluorescence.xaxis.label.set_color('white') 
             self.ax_fluorescence.yaxis.label.set_color('white')
             self.ax_fluorescence.spines['bottom'].set_color('#666') 
         
             
-            for i, fluorescence_data in list(enumerate(reversed(self.all_fluorescence))):
+            for i, fluorescence_data in list(enumerate(reversed(self.all_f_t2p))):
                 fluorescence_zscore = zscore(fluorescence_data, axis=1, ddof=1) #zscore is used to normalize the fluorescence data
                 offset = i * 12 #
                 y_values = fluorescence_zscore[selected_cell_index, :] + offset 
                 color = self.colors[selected_cell_index] 
                 #create a gradient of colors for the curves (the darkest shade is for the last day and the lightest shade is for the first day)
                 if i == 0:
                     color = color 
                 else:
                     h, l, s = colorsys.rgb_to_hls(*color)  
                     l_range = 1 - (l + 0.05)  
-                    l_add = l_range/len(self.all_fluorescence) 
+                    l_add = l_range/len(self.all_f_t2p) 
                     
                     adjusted_luminosity = l + (l_add *i) 
                     color = colorsys.hls_to_rgb(h, adjusted_luminosity, s)
                 ops=self.all_ops[i]
                 fs = ops['fs']
-                tstamps = np.arange(0,self.all_fluorescence[i].shape[1])/fs
+                tstamps = np.arange(0,self.all_f_t2p[i].shape[1])/fs
                 if len(tstamps) != len(y_values):
                     raise ValueError(f"tstamps and y_values must have the same length, but have lengths {len(tstamps)} and {len(y_values)}")
                 self.ax_fluorescence.plot(tstamps,y_values, label=f'Curve {i + 1}', color= color)
             
             self.ax_fluorescence.set_yticklabels([])
             self.ax_fluorescence.get_yaxis().set_visible(False)
             self.ax_fluorescence.set_xlabel('Seconds')
```

### Comparing `track2p-0.5.0/track2p/gui/raster_wd.py` & `track2p-0.5.1/track2p/gui/raster_wd.py`

 * *Files 2% similar despite different names*

```diff
@@ -94,22 +94,23 @@
             self.vmax.setVisible(False)         
             
             label_run= QLabel("Run the analysis:")
             field_run=QPushButton("Run")
             field_run.clicked.connect(self.generate_raster_plt)
             layout.addRow(label_run,field_run)
             
-            label_save= QLabel("Location where you want to save the figures:")
+            label_save= QLabel("Save the figure:")
             field_save = QPushButton("Save")
             field_save.clicked.connect(self.get_output_save_path)
             layout.addRow(label_save,field_save)
             
             label_output_path= QLabel("The figure has been saved here:")
             self.field_output_path=QLabel()
             layout.addRow(label_output_path,self.field_output_path)
+            
             self.view=QGraphicsView(self) #QGraphicsView is a subclass of QWidget
             
             splitter = QSplitter(Qt.Horizontal)            
             right_widget = QWidget()
             right_widget.setLayout(layout)
             splitter.addWidget(right_widget)
             splitter.addWidget(self.view)
@@ -129,31 +130,35 @@
             else:
                 self.advanced_options_group.setVisible(False)
                 self.bin.setVisible(False)
                 self.vmin.setVisible(False)
                 self.vmax.setVisible(False)
                 
         def load_directory_contents(self):
-            load_directory= QFileDialog.getExistingDirectory(self, "Select Directory")
-            if load_directory:
+            self.load_directory= QFileDialog.getExistingDirectory(self, "Select Directory")
+            if self.load_directory:
                 #self.savedirectory=savedirectory
-                self.field_imp_path.setText(f'{load_directory}')
+                self.field_imp_path.setText(f'{self.load_directory}')
             #self.storedPlane = int(self.fieldPlane.text())
-            self.main_window.loadFiles(load_directory,plane=int(self.field_plane.text()))
-            self.all_f_t2p= self.main_window.all_fluorescence
+            plane=int(self.field_plane.text())
+            value=1
+            self.main_window.loadFiles(self.load_directory,plane,value)
+            self.all_f_t2p= self.main_window.all_f_t2p
             self.all_stat_t2p= self.main_window.all_stat_t2p
             for i in range(len(self.all_stat_t2p)):
                 self.day_choice.addItem(str(i + 1))
         
         def get_output_save_path(self):
-            save_path= QFileDialog.getExistingDirectory(self, "Select Directory")
-            if save_path:
-                self.field_output_path.setText(f'{save_path}')
-                filename=os.path.join(save_path,'rasterplot_{}_plane{}.pdf'.format(self.raster_type,str(self.field_plane.text())))
-                plt.savefig(filename)
+            #save_path= QFileDialog.getExistingDirectory(self, "Select Directory")
+            #if save_path:
+            raster_folder = os.path.join(self.load_directory,'track2p', 'raster')
+            os.makedirs(raster_folder, exist_ok=True)
+            self.field_output_path.setText(f'{raster_folder}')
+            filename=os.path.join(raster_folder,'rasterplot_{}_plane{}.pdf'.format(self.raster_type,str(self.field_plane.text())))
+            plt.savefig(filename)
                 
         def get_checkbox_choice(self):
             vmin=float(self.vmin.text())
             vmax=float(self.vmax.text())
             print(vmin)
             print(vmax)
             if self.checkbox1.isChecked():
```

### Comparing `track2p-0.5.0/track2p/gui/roi_plot.py` & `track2p-0.5.1/track2p/gui/roi_plot.py`

 * *Files 4% similar despite different names*

```diff
@@ -6,119 +6,125 @@
 
 
 class ZoomPlotWidget(FigureCanvas):
     """It is used to display the roi of the selected cell across days with each zoom being a different day. 
     The roi is centered on the median coordinates of the selected cell. The mean image of the recording is used to create the zooms. 
     The probability of the cell being a cell and the index of the cell in the suite2p files associated with each recording (day) are also displayed under the zooms."""
     
-    def __init__(self,  all_ops=None, all_stat_t2p=None, colors=None, all_is_cell=None,t2p_match_mat_allday =None):
-        nb_plot=len(all_is_cell)
+    def __init__(self,  all_ops=None, all_stat_t2p=None, colors=None, all_iscell_t2p=None,t2p_match_mat_allday =None,track_ops=None):
+        nb_plot=len(all_iscell_t2p)
         self.fig, self.ax_zoom = plt.subplots(1, nb_plot, figsize = (10*nb_plot, nb_plot), gridspec_kw={'width_ratios': [1] * nb_plot},facecolor='black')
         super().__init__(self.fig)
+        self.track_ops=track_ops
         self.all_ops = all_ops
         self.all_stat_t2p = all_stat_t2p
         self.colors = colors
-        self.all_is_cell=all_is_cell
+        self.all_is_cell=all_iscell_t2p
         self.t2p_match_mat_allday =t2p_match_mat_allday 
+        self.roi_dict={} 
 
     def display_zooms(self, selected_cell_index):
         """It is called when the application is opened and a cell is selected."""
-        roi_dict={} #it is used to store the roi and the median coordinates of the selected cell for each recording (day)
+        self.roi_dict={} #it is used to store the roi and the median coordinates of the selected cell for each recording (day)
         if self.all_ops is not None and self.all_stat_t2p is not None and self.all_is_cell is not None:
             for i in range(len(self.all_ops)):
-                wind = 40
+                wind = 20
                 mean_img = self.all_ops[i]['meanImg']
                 stat_t2p = self.all_stat_t2p[i]
                 median_coord = stat_t2p[selected_cell_index]['med']
                 #if the median coordinates of the selected cell are close to the edges of the mean image, the roi is cropped to avoid an index out of range error
                 if (int(median_coord[0]) + wind) > mean_img.shape[0] and (median_coord[1] + wind) > mean_img.shape[1]:   
                     out_x = (int(median_coord[0]) + wind) - mean_img.shape[0]
                     out_y = (int(median_coord[1]) + wind) - mean_img.shape[1]
                     new_coordinate_x = int(median_coord[0]) - out_x
                     new_coordinate_y = int(median_coord[1]) - out_y
                     roi = mean_img[new_coordinate_x-wind:new_coordinate_x+wind, new_coordinate_y-wind:new_coordinate_y+wind]
                     median_coord[1]= new_coordinate_y
                     median_coord[0]=new_coordinate_x
-                    roi_dict[i] = (roi, median_coord)
+                    self.roi_dict[i] = (roi, median_coord)
                 elif (int(median_coord[0]) + wind) > mean_img.shape[0]: 
                     out_x = (int(median_coord[0]) + wind) - mean_img.shape[0]
                     new_coordinate_x = int(median_coord[0]) - out_x
                     roi = mean_img[new_coordinate_x-wind:new_coordinate_x+wind, int(median_coord[1])-wind:int(median_coord[1])+wind]
                     median_coord[0]=new_coordinate_x
-                    roi_dict[i] = (roi, median_coord)
+                    self.roi_dict[i] = (roi, median_coord)
                 elif (int(median_coord[1]) + wind) > mean_img.shape[1]: 
                     out_y = (int(median_coord[1]) + wind) - mean_img.shape[1]
                     new_coordinate_y = int(median_coord[1]) - out_y
                     roi = mean_img[int(median_coord[0])-wind:int(median_coord[0])+wind, new_coordinate_y-wind:new_coordinate_y+wind]
                     median_coord[1]= new_coordinate_y
-                    roi_dict[i] = (roi, median_coord)
+                    self.roi_dict[i] = (roi, median_coord)
                 elif (int(median_coord[0]) + wind)  > mean_img.shape[0] and (median_coord[1] - wind) <0:   
                     out_x = (int(median_coord[0]) + wind) - mean_img.shape[0]
                     out_y= 0 - (int(median_coord[1]) - wind) 
                     new_coordinate_x= int (median_coord[0]) - out_x
                     new_coordinate_y= int (median_coord[1]) + out_y
                     roi = mean_img[new_coordinate_x-wind:new_coordinate_x+wind, new_coordinate_y-wind:new_coordinate_y+wind]
                     median_coord[1]= new_coordinate_y
                     median_coord[0]=new_coordinate_x
-                    roi_dict[i] = (roi, median_coord)
+                    self.roi_dict[i] = (roi, median_coord)
                 elif (median_coord[1] - wind) <0:   
                     out_y= 0 - (int(median_coord[1]) - wind) 
                     new_coordinate_y= int (median_coord[1]) + out_y
                     roi= mean_img[int(median_coord[0])-wind:int(median_coord[0])+wind, new_coordinate_y-wind:new_coordinate_y+wind]
                     median_coord[1]= new_coordinate_y
-                    roi_dict[i] = (roi, median_coord)
+                    self.roi_dict[i] = (roi, median_coord)
                 elif (int(median_coord[0]) - wind) <0:
                     out_x = 0 - (int(median_coord[0]) - wind)
                     new_coordinate_x= int (median_coord[0]) + out_x
                     roi= mean_img[new_coordinate_x-wind:new_coordinate_x+wind, int(median_coord[1])-wind:int(median_coord[1])+wind]
                     median_coord[0]=new_coordinate_x
-                    roi_dict[i] = (roi, median_coord)
+                    self.roi_dict[i] = (roi, median_coord)
                 elif (int(median_coord[0]) - wind) <0 and (median_coord[1] + wind) > mean_img.shape[1]:   
                     out_x = 0 - (int(median_coord[0]) - wind)
                     out_y= (int(median_coord[1]) + wind) - mean_img.shape[1]
                     new_coordinate_x= int (median_coord[0]) + out_x
                     new_coordinate_y= int (median_coord[1]) - out_y
                     roi = mean_img[new_coordinate_x-wind:new_coordinate_x+wind, new_coordinate_y-wind:new_coordinate_y+wind]
                     median_coord[0]=new_coordinate_x
                     median_coord[1]= new_coordinate_y
-                    roi_dict[i] = (roi, median_coord)
+                    self.roi_dict[i] = (roi, median_coord)
                 elif (int(median_coord[0]) - wind) <0  and (median_coord[1] - wind) <0: 
                     out_x = 0 - (int(median_coord[0]) - wind)
                     out_y= 0 - (int(median_coord[1]) - wind) 
                     new_coordinate_x= int (median_coord[0]) + out_x
                     new_coordinate_y= int (median_coord[1]) + out_y
                     roi = mean_img[new_coordinate_x-wind:new_coordinate_x+wind, new_coordinate_y-wind:new_coordinate_y+wind] 
                     median_coord[0]=new_coordinate_x
                     median_coord[1]= new_coordinate_y
-                    roi_dict[i] = (roi, median_coord)
+                    self.roi_dict[i] = (roi, median_coord)
                 else: 
                     roi = mean_img[int(median_coord[0])-wind:int(median_coord[0])+wind, int(median_coord[1])-wind:int(median_coord[1])+wind]
-                    roi_dict[i] = (roi, median_coord)
+                    self.roi_dict[i] = (roi, median_coord)
             
-            for i, (roi, median_coord) in enumerate(roi_dict.items()):
+            for i, (roi, median_coord) in enumerate(self.roi_dict.items()):
                 iscell=self.all_is_cell[i]
-                indices_lignes_1 = np.where(iscell[:,0]==1)[0]
-                match_index=self.t2p_match_mat_allday[selected_cell_index,i]
-                #print(match_index)
-                true_index=indices_lignes_1[match_index]
-                #print(true_index)
+                if self.track_ops.iscell_thr==None:
+                    indices_lignes_1 = np.where(iscell[:,0]==1)[0]
+                    match_index=self.t2p_match_mat_allday[selected_cell_index,i]
+                    true_index=indices_lignes_1[match_index]
+                else:
+                    indices_lignes_1= np.where(iscell[:,1]>self.track_ops.iscell_thr)[0]
+                    match_index=self.t2p_match_mat_allday[selected_cell_index,i]
+                    true_index=indices_lignes_1[match_index]
+                
                 prob=round(iscell[true_index,1],2)
                 stat_t2p = self.all_stat_t2p[i]
                 ypix=stat_t2p[selected_cell_index]['ypix']
                 xpix=stat_t2p[selected_cell_index]['xpix']
                 ax = self.ax_zoom[i]
                 color = self.colors[selected_cell_index]
-                median_values= list(roi_dict.values())[i][1] #median coordinates of the selected cell
+                median_values= list(self.roi_dict.values())[i][1] #median coordinates of the selected cell
                 mask=np.zeros((2*wind,2*wind))
                 mask[ypix-median_values[0]+wind,xpix-median_values[1]+wind]=1
                 ax.clear()
                 ax.contour(mask,levels=[0.5], colors=[color],linewidths=2)
                 
-                l_roi=list(roi_dict.values())[-1][0] 
-                match_roi=skimage.exposure.match_histograms(list(roi_dict.values())[i][0], l_roi, channel_axis=None)
+                l_roi=list(self.roi_dict.values())[-1][0] 
+                match_roi=skimage.exposure.match_histograms(list(self.roi_dict.values())[i][0], l_roi, channel_axis=None)
                 
                 ax.imshow(match_roi, cmap='gray')
                 ax.set_title(f'Day {i + 1}', color='white', fontsize=10)
                 ax.text(0.5, -0.2, f'i: {true_index}', color='white', fontsize=10, ha='center', va='center', transform=ax.transAxes)
                 ax.text(0.5, -0.4, f'p: {prob}', color='white', fontsize=10, ha='center', va='center', transform=ax.transAxes)
 
                 ax.axis('off')
```

### Comparing `track2p-0.5.0/track2p/gui/t2p_wd.py` & `track2p-0.5.1/track2p/gui/t2p_wd.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,13 +1,15 @@
 
 import os
-from PyQt5.QtWidgets import QVBoxLayout, QWidget,  QHBoxLayout, QPushButton, QFileDialog, QLineEdit, QLabel, QFormLayout, QListWidget, QMessageBox,QListWidgetItem, QInputDialog,QCheckBox,QSizePolicy
+from PyQt5.QtWidgets import QVBoxLayout, QWidget,  QHBoxLayout, QPushButton, QFileDialog, QLineEdit, QLabel, QFormLayout, QListWidget, QMessageBox,QListWidgetItem, QInputDialog,QCheckBox,QSizePolicy,QComboBox,QDialog
 from PyQt5.QtCore import Qt
 from track2p.t2p import run_t2p
 from track2p.ops.default import DefaultTrackOps
+
+
 import sys 
 #from track2p.gui.terminal_gui import MultiStream, ConsoleOutput
 
 
 class NewWindow(QWidget):
         """it is used to set the parameters of the track2p algorithm. 
     It is called when the user clicks on the run track2p algorithm button in the main window. 
@@ -16,14 +18,15 @@
     The user can also save the parameters and run the track2p algorithm."""
         def __init__(self, mainWindow):
             super(NewWindow,self).__init__()
             self.main_window = mainWindow
             layout = QFormLayout()
             self.setLayout(layout)
             self.stored_plane=None 
+            self.track_ops = DefaultTrackOps()
             self.file_paths = {}
             
         
             label_imp_button=QLabel(" Import the directory containing subfolders of different recordings for the same subject:")
             self.importButton = QPushButton("Import", self)
             self.importButton.clicked.connect(self.importDirectory)
             layout.addRow(label_imp_button,self.importButton)
@@ -87,25 +90,30 @@
             
             label_save_path= QLabel("Here is the path to access the track2P folder:")
             label_save_path.setSizePolicy(QSizePolicy.Fixed, QSizePolicy.Fixed)
             self.save_path=QLabel()
             self.save_path.setSizePolicy(QSizePolicy.Fixed, QSizePolicy.Fixed)
             layout.addRow(label_save_path,self.save_path)
             
-        
+            label_save_s2p= QLabel("Save the outputs in suite2p format (containing cells tracked on all days):")
+            self.checkbox3 = QCheckBox(self)
+            #self.checkbox3.stateChanged.connect(self.save_in_s2p_format)
+            layout.addRow(label_save_s2p,self.checkbox3)
+            
+
             self.run_button = QPushButton("Run", self)
             self.run_button.clicked.connect(self.run)
             layout.addRow("Run the algorithm:", self.run_button)
             
             terminal_intruction=QLabel("To monitor the progress of the algorith see outputs in the terminal where the GUI was launched from")
             layout.addRow(terminal_intruction)
      
     
 ############################################################################################################################################################################
-
+        
         def display_iscell(self,state):
             if state == Qt.Checked:
                 self.is_cell_thr.setVisible(True)
             else:
                 self.is_cell_thr.setVisible(False)
 
         def run(self):
@@ -113,35 +121,39 @@
             self.is_cell= self.is_cell_thr.text()
             self.reg_channel= self.reg_chan.text()
             self.save_track2p_path= self.savedirectory
             self.stored_all_ds_path = []
             for i in range(self.paths_list.count()):
                 self.stored_all_ds_path.append(self.paths_list.item(i).data(Qt.UserRole))
             print("All parameters have been recorded ! The track2p algorithm is running...")
-            track_ops = DefaultTrackOps() #Initializes the track_ops object with the default parameters
-            track_ops.all_ds_path= self.stored_all_ds_path
-            print(f'track_ops.all_ds_path : {track_ops.all_ds_path}')
-            track_ops.save_path = self.save_track2p_path
-            track_ops.reg_chan=int(self.reg_channel)
+           # self.track_ops = DefaultTrackOps() #Initializes the self.track_ops object with the default parameters
+            self.track_ops.all_ds_path= self.stored_all_ds_path
+            #print(f'self.track_ops.all_ds_path : {self.track_ops.all_ds_path}')
+            self.track_ops.save_path = self.save_track2p_path
+            self.track_ops.reg_chan=int(self.reg_channel)
             if self.checkbox1.isChecked():
-                track_ops.iscell_thr=None
+                self.track_ops.iscell_thr=None
             if self.checkbox2.isChecked():
-                track_ops.iscell_thr=float(self.is_cell)
-            run_t2p(track_ops)
+                self.track_ops.iscell_thr=float(self.is_cell)
+            if self.checkbox3.isChecked():
+                self.track_ops.save_in_s2p_format=True
+            run_t2p(self.track_ops)
             self.askQuestion()
- 
 
+        # In your askQuestion method:
         def askQuestion(self):
             reply = QMessageBox.question(self, "", "Run completed successfully!\nDo you want to launch the gui?", QMessageBox.Yes | QMessageBox.No, QMessageBox.No)
 
             if reply == QMessageBox.Yes:
-                text, ok = QInputDialog.getText(self, '', 'Enter your plane:')
-                if ok:
-                    self.storedPlane=int(text)
-                    self.main_window.loadFiles(self.save_track2p_path, plane=self.storedPlane)
+                dialog = ComboBoxDialog(self)
+                if dialog.exec_():
+                    plane, comboBoxResult = dialog.getResults()
+                    self.storedPlane = int(plane)
+                    comboBoxResult = int(comboBoxResult)
+                    self.main_window.loadFiles(self.save_track2p_path, plane=self.storedPlane, combobox_value=comboBoxResult)
                     self.close()
             if reply == QMessageBox.No:
                 pass
         
         def saveDirectory(self):
             savedirectory= QFileDialog.getExistingDirectory(self, "Select Directory")
             if savedirectory:
@@ -154,28 +166,55 @@
                 self.label_dir.setText(f'{directory}')
                 self.computer_file_list.clear()
                 files= os.listdir(directory)
                 for file in sorted(files):
                     full_path = os.path.join(directory, file)
                     item=QListWidgetItem(file)
                     item.setData(Qt.UserRole, full_path)
-                   # print(f'file_name={item.text()}')
-                    #print(f'full_path={item.data(Qt.UserRole)}')
                     self.computer_file_list.addItem(item)
 
 
         def moveFileToBox(self):
             selectedItems = self.computer_file_list.selectedItems()
             for item in selectedItems:
                 self.computer_file_list.takeItem(self.computer_file_list.row(item))
                 self.paths_list.addItem(item)
-            #for i in range(self.boxFileListWidget.count()):
-              #  print(self.boxFileListWidget.item(i).text())
-              # print(self.boxFileListWidget.item(i).data(Qt.UserRole))
+       
 
         def moveFileToComputer(self):
             selectedItems = self.paths_list.selectedItems()
             for item in selectedItems:
                 self.paths_list.takeItem(self.paths_list.row(item))
                 self.computer_file_list.addItem(item)
                 
 
+class ComboBoxDialog(QDialog):
+    def __init__(self, parent=None):
+        super(ComboBoxDialog, self).__init__(parent)
+        self.parent=parent
+        self.layout = QFormLayout(self)
+
+        # Add a label
+        label_plane= QLabel("Choose the plane to analyze:")
+        self.field_plane=QLineEdit()
+        self.field_plane.setText('0')
+        self.field_plane.setFixedWidth(50)
+        self.layout.addRow(label_plane,self.field_plane)
+        
+
+        label_combobox= QLabel("not_cell_count_over_days :")
+        self.comboBox = QComboBox(self)
+        for i in range(len(self.parent.stored_all_ds_path)):
+            self.comboBox.addItem(str(i + 1))
+        self.layout.addRow(label_combobox,self.comboBox)
+        # Add a "OK" button
+        self.okButton = QPushButton("OK", self)
+        self.okButton.clicked.connect(self.accept)
+        self.layout.addRow(self.okButton)
+        
+        self.setLayout(self.layout)
+    
+    def getResults(self):
+        return self.field_plane.text(), self.comboBox.currentText()
+        
+        
+
```

### Comparing `track2p-0.5.0/track2p/io/loaders.py` & `track2p-0.5.1/track2p/io/loaders.py`

 * *Files 12% similar despite different names*

```diff
@@ -8,18 +8,16 @@
     stat = np.load(track_ops_path + f'/suite2p/plane{plane_idx}/stat.npy', allow_pickle=True)
     iscell = np.load(track_ops_path + f'/suite2p/plane{plane_idx}/iscell.npy', allow_pickle=True)
     # filter based on track_ops.iscell_thr
     len_stat_allcell = len(stat)
     
     if track_ops.iscell_thr==None:
         stat = stat[iscell[:,0] ==1]
-        print("manually")
     else:
         stat= stat[iscell[:,1]>track_ops.iscell_thr]
-        print("probability")
     len_stat_iscell = len(stat)
     print(f'Loading ROIs for plane{plane_idx} in dataset {track_ops_path.split("/")[-2]}')
     print(f'Chose {len_stat_iscell}/{len_stat_allcell} ROIs, based on s2p iscell threshold {track_ops.iscell_thr} (see track_ops.iscell_thr)')
     # make a stat_summary dictionary
     stat_summary = {
         'len_stat_allcell': len_stat_allcell,
         'len_stat_iscell': len_stat_iscell,
```

### Comparing `track2p-0.5.0/track2p/io/s2p_loaders.py` & `track2p-0.5.1/track2p/io/s2p_loaders.py`

 * *Files 2% similar despite different names*

```diff
@@ -65,18 +65,16 @@
     for (i, ds_path) in enumerate(track_ops.all_ds_path):
         ds_stat_iscell = []
         for j in range(track_ops.nplanes):
             stat = np.load(os.path.join(ds_path, 'suite2p', f'plane{j}', 'stat.npy'), allow_pickle=True)
             iscell = np.load(os.path.join(ds_path, 'suite2p', f'plane{j}', 'iscell.npy'), allow_pickle=True)
             if track_ops.iscell_thr==None:
                 stat_iscell = stat[iscell[:,0]==1]
-                print("manually")
             else: 
                 stat_iscell = stat[iscell[:,1]>track_ops.iscell_thr]
-                print("probability")
             ds_stat_iscell.append(stat_iscell)
         all_ds_stat_iscell.append(ds_stat_iscell)
 
     return all_ds_stat_iscell
 
 def load_all_ds_ops(track_ops):
     all_ds_ops = []
```

### Comparing `track2p-0.5.0/track2p/io/savers.py` & `track2p-0.5.1/track2p/io/savers.py`

 * *Files identical despite different names*

### Comparing `track2p-0.5.0/track2p/match/loop.py` & `track2p-0.5.1/track2p/match/loop.py`

 * *Files identical despite different names*

### Comparing `track2p-0.5.0/track2p/match/utils.py` & `track2p-0.5.1/track2p/match/utils.py`

 * *Files 4% similar despite different names*

```diff
@@ -9,16 +9,14 @@
     for i in range(all_roi.shape[2]):
         roi = all_roi[:,:,i]
         labels = measure.label(roi)
         features = measure.regionprops(labels)
         try:
             centroids.append(features[0].centroid)
         except IndexError:
-            print('IndexError in get_centroids')
-            print('roi index', i)
             centroids.append([0, 0])
 
     return np.array(centroids)
 
 def get_cent_dist_mat(all_roi_ref, all_roi_reg):
     # compute distances
     centroids_ref = get_centroids(all_roi_ref)
```

### Comparing `track2p-0.5.0/track2p/ops/default.py` & `track2p-0.5.1/track2p/ops/default.py`

 * *Files 12% similar despite different names*

```diff
@@ -25,14 +25,22 @@
 
         # do not change these
         self.show_roi_reg_output = False # this is slow because plt.contour is slow and also very memory intensive(it can easily crash) but the visualisation is nice for presentations (for example by increasing self.iscell_thr)
 
         # plotting parameters
         self.win_size = 48 # window size for visualising matched ROIs across days (crop of mean image)
         self.sat_perc = 99.9 # percentile to saturate image at (only affects visualisation not the registration/matching)
+        
+        self.colors = None # save color after curation
+        self.vector_curation=None #save the status of the ROIs after curation
+        self.init_colors=None #save the initial colors of the ROIs (before curation)
+        self.curated_cells=None #save the index of the curated cells
+        
+        
+        self.save_in_s2p_format = False # save the output in suite2p format (this is useful for downstream analysis with suite2p)
 
         # make the output directories when initialising the object
         
     def init_save_paths(self):
         self.save_path = os.path.join(self.save_path, 'track2p/')
         self.save_path_fig = os.path.join(self.save_path, 'fig/')
         make_dir(self.save_path)
```

### Comparing `track2p-0.5.0/track2p/plot/output.py` & `track2p-0.5.1/track2p/plot/output.py`

 * *Files 2% similar despite different names*

```diff
@@ -172,14 +172,15 @@
     plt.close(fig)
 
 
 def plot_thr_met_hist(all_ds_thr_met, all_ds_thr, track_ops):
     fig, axs = plt.subplots(track_ops.nplanes, len(all_ds_thr_met), figsize=(6*len(all_ds_thr_met), 6*track_ops.nplanes), sharey=True, sharex=True)
     for i in range(len(all_ds_thr_met)):
         for j in range(track_ops.nplanes):
+            axs = np.array([axs]) if type(axs) is not np.ndarray else axs
             this_ax = axs[i] if track_ops.nplanes==1 else axs[j][i]
             n_reg_roi = len(all_ds_thr_met[i][j])
             n_abovethr_roi = np.sum(all_ds_thr_met[i][j]>all_ds_thr[i][j])
             this_ax.hist(all_ds_thr_met[i][j], bins=20)
             this_ax.axvline(all_ds_thr[i][j], color='grey', linestyle='--')
             # label the line with 'otsu threshold'
             this_ax.text(all_ds_thr[i][j]+0.02, this_ax.get_ylim()[1]*0.9, f'{track_ops.thr_method} thr.: {all_ds_thr[i][j]:.2f}')
```

### Comparing `track2p-0.5.0/track2p/plot/progress.py` & `track2p-0.5.1/track2p/plot/progress.py`

 * *Files identical despite different names*

### Comparing `track2p-0.5.0/track2p/plot/utils.py` & `track2p-0.5.1/track2p/plot/utils.py`

 * *Files identical despite different names*

### Comparing `track2p-0.5.0/track2p/register/elastix.py` & `track2p-0.5.1/track2p/register/elastix.py`

 * *Files identical despite different names*

### Comparing `track2p-0.5.0/track2p/register/loop.py` & `track2p-0.5.1/track2p/register/loop.py`

 * *Files identical despite different names*

### Comparing `track2p-0.5.0/track2p/register/utils.py` & `track2p-0.5.1/track2p/register/utils.py`

 * *Files identical despite different names*

### Comparing `track2p-0.5.0/track2p.egg-info/PKG-INFO` & `track2p-0.5.1/track2p.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 Metadata-Version: 2.1
 Name: track2p
-Version: 0.5.0
+Version: 0.5.1
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: numpy==1.23.5
 Requires-Dist: matplotlib==3.5.3
 Requires-Dist: scikit-image==0.20.0
 Requires-Dist: itk-elastix==0.19.1
 Requires-Dist: PyQt5==5.15.10
 Requires-Dist: qtpy==2.4.1
 Requires-Dist: tqdm==4.66.2
 Requires-Dist: scikit-learn==1.4.0
 Requires-Dist: openTSNE==1.0.1
+Requires-Dist: pandas==1.5.3
 
 # track2p
 Cell tracking for longitudinal calcium imaging recordings.
 
 [![PyPI version](https://img.shields.io/pypi/v/track2p)](https://pypi.org/project/track2p/)
 [![All time downloads](https://static.pepy.tech/badge/track2p)](https://pepy.tech/project/track2p)
 [![Monthly downloads](https://img.shields.io/pypi/dm/track2p)](https://pypi.org/project/track2p/)
@@ -50,51 +51,59 @@
 python -m track2p
 ```
 
 This opens a GUI allowing the user to launch the algorithm and visualise the results interactively.
 
 (For instructions on running track2p without the GUI see the 'Run via script' under the 'Usage' section)
 
+Note: For common installation issues see [documentation](https://github.com/juremaj/track2p/blob/main/docs/installation.md).
+
 # Usage
 
 ## Run through GUI
 
 After activating the GUI through `python -m track2p` the user should navigate to the 'Run' tab on the top left of the window and select 'Run algorithm' from the dropdown menu. This will open a pop-up window that will allow the user to set the paths to suite2p datasets and to set the algorithm parameters. Once these have been set the user can click on 'Run', which will launch the track2p algorithm, with the progress being printed in the window below.
 
-When the algorithm is finished, another pop-up window will appear, asking the user if they want to visualise the outputs in the GUI (for more information see section below).
+When the algorithm is finished, another pop-up window will appear, asking the user if they want to visualise the outputs in the GUI.
+
+For more details on how to run the algorithm through the GUI see [documentation](https://github.com/juremaj/track2p/blob/main/docs/gui.md) and for more description of paramters see documentation [here](https://github.com/juremaj/track2p/blob/main/docs/parameters.md).
 
 ## GUI visualisation
 
 
 The GUI supports both visualisation after algorithm run (as described above), as well as visualising previously processed data. The latter can be done by navigating to File -> Load processed data on the top left of the GUI.
 
 
 ![gui_mainwindow.png](docs/media/plots/gui_mainwindow.png)
 
 Briefly the GUI allows the user to visualise the mean field of view on all days, with the ROIs of all matched cells visualised. The user can then interactively select a cell by clicking on the ROI on the mean image. This will display a zoomed-in view of this cell across all days on the right, and the extracted fluorescence time series below.
 
+For more details on how to use the GUI for visualising track2p results see [documentation](https://github.com/juremaj/track2p/blob/main/docs/gui.md).
+
 ## Run via script
 
 To run via script you can use the `run_track2p.py` script in the root of this repo as a template. It is exactly the same as running thrugh the gui, only that the paths and the parameters are defined within the script (for more on parameters etc. see documentation). When running make sure you are running it within the track2p environment, for example:
 
 ```
 conda activate track2p
 python -m run_track2p
 ```
 
 # Outputs
 
-All the outputs of the script will be saved in a `track2p` folder created within the `track_ops.save_path` directory specified by the user when running the algorithm. For an introduction on how to use the outputs for further downstream analysis we provide a useful demo notebook `demo_t2p_outlput.ipynb` in the root of this repository. Note: You will need to additionally install jupyter for this to work. For example:
+All the outputs of the script will be saved in a `track2p` folder created within the `track_ops.save_path` directory specified by the user when running the algorithm. For an introduction on how to use the outputs for further downstream analysis we provide a useful demo notebook `demo_t2p_output.ipynb` in the root of this repository. Note: You will need to additionally install jupyter for this to work. For example:
 
 ```
 conda install conda-forge::jupyterlab
 ```
 
+For more information see documentation relating to track2p [viusalisations](https://github.com/juremaj/track2p/blob/main/docs/visualisations.md) and [outputs](https://github.com/juremaj/track2p/blob/main/docs/outputs.md).
+
 # Reference
 
 For now if you use the algorithm please reference the Cosyne abstract:
 
-  **Majnik, J., Zangila, S., Cossart, R. & Platel, J. C. (2024). _Emergence of state modulation in a developing circuit_. COSYNE Abstract.**
+  **Majnik, J., Zangila, S., Cossart, R. & Platel, J. C. (2024). _Emergence of state modulation in a developing cortical circuit_. COSYNE Abstract.**
 
   
 
 You can also see the YouTube recording of the talk for a reference use-case in neocortical development: [Link to video (starting at 47:20)](https://youtu.be/Tr97HwgQ9ik?t=2839)
```

### Comparing `track2p-0.5.0/track2p.egg-info/SOURCES.txt` & `track2p-0.5.1/track2p.egg-info/SOURCES.txt`

 * *Files 5% similar despite different names*

```diff
@@ -12,15 +12,14 @@
 track2p/gui/__init__.py
 track2p/gui/cell_plot.py
 track2p/gui/fluo_plot.py
 track2p/gui/import_wd.py
 track2p/gui/main_wd.py
 track2p/gui/raster_wd.py
 track2p/gui/roi_plot.py
-track2p/gui/run_gui.py
 track2p/gui/t2p_wd.py
 track2p/io/__init__.py
 track2p/io/loaders.py
 track2p/io/s2p_loaders.py
 track2p/io/savers.py
 track2p/io/utils.py
 track2p/match/__init__.py
```

