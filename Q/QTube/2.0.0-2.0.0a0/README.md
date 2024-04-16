# Comparing `tmp/QTube-2.0.0.tar.gz` & `tmp/qtube-2.0.0a0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "QTube-2.0.0.tar", last modified: Tue Apr  9 21:13:56 2024, max compression
+gzip compressed data, was "qtube-2.0.0a0.tar", last modified: Tue Apr 16 15:15:36 2024, max compression
```

## Comparing `QTube-2.0.0.tar` & `qtube-2.0.0a0.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxrwxrwx   0        0        0        0 2024-04-09 21:13:56.933931 QTube-2.0.0/
--rw-rw-rw-   0        0        0     1098 2024-03-22 12:34:17.000000 QTube-2.0.0/LICENSE.txt
--rw-rw-rw-   0        0        0    15168 2024-04-09 21:13:56.930929 QTube-2.0.0/PKG-INFO
-drwxrwxrwx   0        0        0        0 2024-04-09 21:13:56.676252 QTube-2.0.0/QTube/
-drwxrwxrwx   0        0        0        0 2024-04-09 21:13:56.783471 QTube-2.0.0/QTube/scripts/
--rw-rw-rw-   0        0        0        0 2024-04-09 11:51:19.000000 QTube-2.0.0/QTube/scripts/__init__.py
--rw-rw-rw-   0        0        0    26126 2024-04-09 21:13:43.000000 QTube-2.0.0/QTube/scripts/qtube.py
--rw-rw-rw-   0        0        0    89918 2024-03-19 09:48:04.000000 QTube-2.0.0/QTube/scripts/tests.py
-drwxrwxrwx   0        0        0        0 2024-04-09 21:13:56.827362 QTube-2.0.0/QTube/utils/
--rw-rw-rw-   0        0        0        0 2024-03-27 18:35:16.000000 QTube-2.0.0/QTube/utils/__init__.py
--rw-rw-rw-   0        0        0    11137 2024-04-09 15:58:26.000000 QTube-2.0.0/QTube/utils/checks.py
--rw-rw-rw-   0        0        0     6833 2024-03-19 09:46:30.000000 QTube-2.0.0/QTube/utils/helpers.py
--rw-rw-rw-   0        0        0     7421 2024-03-19 09:46:53.000000 QTube-2.0.0/QTube/utils/parsing.py
-drwxrwxrwx   0        0        0        0 2024-04-09 21:13:56.901928 QTube-2.0.0/QTube/utils/youtube/
--rw-rw-rw-   0        0        0     1558 2024-03-19 09:40:23.000000 QTube-2.0.0/QTube/utils/youtube/captions.py
--rw-rw-rw-   0        0        0     3233 2024-03-19 09:41:06.000000 QTube-2.0.0/QTube/utils/youtube/channels.py
--rw-rw-rw-   0        0        0     3090 2024-03-19 09:41:48.000000 QTube-2.0.0/QTube/utils/youtube/playlists.py
--rw-rw-rw-   0        0        0    11641 2024-03-19 09:44:03.000000 QTube-2.0.0/QTube/utils/youtube/videos.py
-drwxrwxrwx   0        0        0        0 2024-04-09 21:13:56.919930 QTube-2.0.0/QTube.egg-info/
--rw-rw-rw-   0        0        0    15168 2024-04-09 21:13:56.000000 QTube-2.0.0/QTube.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      512 2024-04-09 21:13:56.000000 QTube-2.0.0/QTube.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-09 21:13:56.000000 QTube-2.0.0/QTube.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       51 2024-04-09 21:13:56.000000 QTube-2.0.0/QTube.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0      159 2024-04-09 21:13:56.000000 QTube-2.0.0/QTube.egg-info/requires.txt
--rw-rw-rw-   0        0        0        6 2024-04-09 21:13:56.000000 QTube-2.0.0/QTube.egg-info/top_level.txt
--rw-rw-rw-   0        0        0    12514 2024-03-19 11:00:50.000000 QTube-2.0.0/README.md
--rw-rw-rw-   0        0        0     1444 2024-04-09 21:00:35.000000 QTube-2.0.0/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-04-09 21:13:56.934931 QTube-2.0.0/setup.cfg
--rw-rw-rw-   0        0        0      649 2024-04-09 17:05:50.000000 QTube-2.0.0/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-16 15:15:36.953742 qtube-2.0.0a0/
+-rw-rw-rw-   0        0        0     1098 2024-03-22 12:34:17.000000 qtube-2.0.0a0/LICENSE.txt
+-rw-rw-rw-   0        0        0    15737 2024-04-16 15:15:36.951741 qtube-2.0.0a0/PKG-INFO
+drwxrwxrwx   0        0        0        0 2024-04-16 15:15:36.817595 qtube-2.0.0a0/QTube/
+drwxrwxrwx   0        0        0        0 2024-04-16 15:15:36.886562 qtube-2.0.0a0/QTube/scripts/
+-rw-rw-rw-   0        0        0        0 2024-04-09 11:51:19.000000 qtube-2.0.0a0/QTube/scripts/__init__.py
+-rw-rw-rw-   0        0        0    26111 2024-04-16 14:02:35.000000 qtube-2.0.0a0/QTube/scripts/qtube.py
+-rw-rw-rw-   0        0        0    89918 2024-03-19 09:48:04.000000 qtube-2.0.0a0/QTube/scripts/tests.py
+drwxrwxrwx   0        0        0        0 2024-04-16 15:15:36.911564 qtube-2.0.0a0/QTube/utils/
+-rw-rw-rw-   0        0        0        0 2024-03-27 18:35:16.000000 qtube-2.0.0a0/QTube/utils/__init__.py
+-rw-rw-rw-   0        0        0    11137 2024-04-09 15:58:26.000000 qtube-2.0.0a0/QTube/utils/checks.py
+-rw-rw-rw-   0        0        0     6833 2024-03-19 09:46:30.000000 qtube-2.0.0a0/QTube/utils/helpers.py
+-rw-rw-rw-   0        0        0     7421 2024-03-19 09:46:53.000000 qtube-2.0.0a0/QTube/utils/parsing.py
+drwxrwxrwx   0        0        0        0 2024-04-16 15:15:36.934564 qtube-2.0.0a0/QTube/utils/youtube/
+-rw-rw-rw-   0        0        0     1558 2024-03-19 09:40:23.000000 qtube-2.0.0a0/QTube/utils/youtube/captions.py
+-rw-rw-rw-   0        0        0     3233 2024-03-19 09:41:06.000000 qtube-2.0.0a0/QTube/utils/youtube/channels.py
+-rw-rw-rw-   0        0        0     3090 2024-03-19 09:41:48.000000 qtube-2.0.0a0/QTube/utils/youtube/playlists.py
+-rw-rw-rw-   0        0        0    11641 2024-03-19 09:44:03.000000 qtube-2.0.0a0/QTube/utils/youtube/videos.py
+drwxrwxrwx   0        0        0        0 2024-04-16 15:15:36.937741 qtube-2.0.0a0/QTube.egg-info/
+-rw-rw-rw-   0        0        0    15737 2024-04-16 15:15:36.000000 qtube-2.0.0a0/QTube.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      512 2024-04-16 15:15:36.000000 qtube-2.0.0a0/QTube.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-16 15:15:36.000000 qtube-2.0.0a0/QTube.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       51 2024-04-16 15:15:36.000000 qtube-2.0.0a0/QTube.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0      159 2024-04-16 15:15:36.000000 qtube-2.0.0a0/QTube.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        6 2024-04-16 15:15:36.000000 qtube-2.0.0a0/QTube.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0    13081 2024-04-11 04:37:59.000000 qtube-2.0.0a0/README.md
+-rw-rw-rw-   0        0        0     1450 2024-04-16 15:14:47.000000 qtube-2.0.0a0/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-04-16 15:15:36.953742 qtube-2.0.0a0/setup.cfg
+-rw-rw-rw-   0        0        0      655 2024-04-16 15:14:53.000000 qtube-2.0.0a0/setup.py
```

### Comparing `QTube-2.0.0/LICENSE.txt` & `qtube-2.0.0a0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `QTube-2.0.0/PKG-INFO` & `qtube-2.0.0a0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: QTube
-Version: 2.0.0
+Version: 2.0.0a0
 Summary: Automatically add Youtube videos to a playlist.
 Home-page: https://github.com/Killian42/QTube
 Author: Killian Lebreton
 Author-email: Killian Lebreton <killian.lebreton35@gmail.com>
 Maintainer-email: Killian Lebreton <killian.lebreton35@gmail.com>
 License: MIT License
         
@@ -51,23 +51,24 @@
 Requires-Dist: protobuf>=4.25.1
 Requires-Dist: pytube>=15.0.0
 Requires-Dist: Requests>=2.31.0
 Requires-Dist: setuptools>=68.2.2
 
 <h1 align="center">
    <br>
-   <a href="https://github.com/Killian42/QTube/releases/latest"><img src="logo.png" alt="QTube" width="500"></a>
+   <a href="https://github.com/Killian42/QTube/releases/latest"><img src="https://i.postimg.cc/wMLMYv3M/logo.png" alt="QTube" width="500"></a>
    <br>
 </h1>
 
 <h3 align="center">Automatically add Youtube videos to a playlist.</h3>
 
 <p align="center">
    <a href="https://www.repostatus.org/#active"><img src="https://www.repostatus.org/badges/latest/active.svg" alt="Project Status: Active – The project has reached a stable, usable state and is being actively developed." /></a>
    <a href="https://github.com/Killian42/QTube/releases/latest"><img src="https://img.shields.io/github/v/release/Killian42/QTube" alt="Latest Version"></a>
+   <a href="https://pypi.org/project/QTube/"><img src="https://img.shields.io/pypi/dm/QTube.svg?label=PyPI%20downloads" alt="PyPi Downloads"></a>
    <a href="https://github.com/Killian42/QTube/issues"><img src="https://img.shields.io/github/issues/Killian42/QTube" alt="Open Issues"></a>
    <a href="https://github.com/Killian42/QTube/issues?q=is%3Aissue+is%3Aclosed"><img src="https://img.shields.io/github/issues-closed/Killian42/QTube?color=sucess" alt="Closed Issues"></a>
    <a href="https://opensource.org/licenses/MIT"><img src="https://img.shields.io/badge/license-MIT-green" alt="License"></a>
    <a href="https://github.com/psf/black"><img src="https://img.shields.io/badge/code%20style-black-000000.svg" alt="Code style: black"></a>
    <a href="https://github.com/Killian42/QTube"><img src="https://img.shields.io/github/languages/code-size/Killian42/QTube" alt="Code Size"></a>
 </p>
 
@@ -100,23 +101,23 @@
 * Upload date filtering
 * Shorts filtering
 * Duplicate checking
 
 ## How to use
 Before using this software, you first need to get a Youtube API key and create a web app to get a client secrets file (that should look like [this](docs/client_secrets_template.json)). This [Corey Schafer video](https://www.youtube.com/watch?v=vQQEaSnQ_bs) goes through the process step by step.
 
-Once that's done, either clone this repository or download the ZIP archive. Then, copy and rename the [user parameters template](docs/user_params_template.json) file to *user_params.json*. Modify it so that it fits your needs (more information on how in the [following table](#user-defined-parameters) and in the [examples section](#examples)).
+Once that's done, download this project or install the package with [PyPI](https://pypi.org/project/QTube/). Then, copy the [user parameters template](docs/user_params_template.json) file to the main QTube directory and rename it to *user_params.json*. Modify it so that it fits your needs (more information on how in the [following table](#user-defined-parameters) and in the [examples section](#examples)).
 
-Verify that you have all of the dependencies installed (see the [requirements](requirements.txt) file).
+Verify that you have all of the dependencies installed (see the [requirements](requirements.txt) file or the [TOML](pyproject.toml) file).
 
-Finally, execute the [run.py](QTube/run.py) file to start the software.
+Finally, execute the [qtube.py](QTube/scripts/qtube.py) file to start the software, either by running the file directly or by using the CLI ***qtube*** in the main directory.
 
 I would recommend creating a task to execute the program regularly (like once a day).
 
-For more versatile uses, you can also use command line arguments with the [run.py](QTube/run.py) file. Enable this option by setting the parameter `override_json` to *True* in your JSON user parameters file. Provided command line arguments will then override what is in your JSON user parameters file.
+For more versatile uses, you can also use command line arguments with the [qtube.py](QTube/scripts/qtube.py) file. Enable this option by setting the parameter `override_json` to *True* in your JSON user parameters file. Provided command line arguments will then override what is in your JSON user parameters file. This is especially useful to manage different types of videos and put them in dedicated playlists (music playlist, gaming playlist, ect...).
 
 ### User-defined parameters
 |Parameter|Optional|Description|Possible values|
 |--|:--:|:--:|:--:|
 |`required_in_channel_name`|Yes|Words that must be in channel names, typically channel names themselves. Videos from channels not containing any of the words of this list in their name will not be added.|Any string|
 |`banned_in_channel_name`|Yes|Words that must not be in channel names, typically channel names themselves. Videos from channels containing any of the words of this list in their name will not be added.|Any string|
 |`include_extra_channels`|No|Determines whether to include channels the user is not subscribed to.|boolean|
@@ -146,15 +147,15 @@
 |`override_json`|No|Allow command line arguments to override user_params.json parameters.|boolean|
 |`verbosity`|No|Controls how much information is shown in the terminal. Options can be combined, so that selecting each option gives the same result as selecting *all*. <br>1: Everything is shown.<br>2: Nothing is shown.<br>3: Only information regarding function execution is shown.<br>4: Only information regarding credentials is shown (loading, retrieving and saving).<br>5: Only information regarding added videos is shown (number, channel names and video titles).|<br>*all*<sup> 1 </sup>, <br>*none*<sup> 2 </sup> , <br>*func*<sup> 3 </sup>, <br>*credentials*<sup> 4 </sup> ,<br>*videos*<sup> 5 </sup>.|
 
 All parameters are case-sensitive by default and if you do not want to use an optional parameter, replace its value with *null* or delete the entry.
 
 For further information about each parameter, check the note associated with the [release](https://github.com/Killian42/QTube/releases) they were introduced in.
 ### Requirements
-See the [requirements](requirements.txt) file.
+See the [requirements](requirements.txt) file or the [TOML](pyproject.toml) file.
 
 ## Examples
 This section presents examples of user parameters json files for concrete use-cases.
 * <a href="#example-1---every-videos-from-subscribed-channels">Every videos from subscribed channels</a>
 * <a href="#example-2---higher-quality-videos">Higher quality videos</a>
 * <a href="#example-3---specific-video-series-from-a-creator">Video series from a creator</a>
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: QTube Version: 2.0.0 Summary: Automatically add
+Metadata-Version: 2.1 Name: QTube Version: 2.0.0a0 Summary: Automatically add
 Youtube videos to a playlist. Home-page: https://github.com/Killian42/QTube
 Author: Killian Lebreton Author-email: Killian Lebreton
 gmail.com> Maintainer-email: Killian Lebreton
 gmail.com> License: MIT License Copyright (c) [2024] [Killian Lebreton]
 Permission is hereby granted, free of charge, to any person obtaining a copy of
 this software and associated documentation files (the "Software"), to deal in
 the Software without restriction, including without limitation the rights to
@@ -32,16 +32,16 @@
 protobuf>=4.25.1 Requires-Dist: pytube>=15.0.0 Requires-Dist: Requests>=2.31.0
 Requires-Dist: setuptools>=68.2.2
                                     ************
                                     _[[_QQ_TT_uu_bb_ee_]]
                                      ************
            ******** AAuuttoommaattiiccaallllyy aadddd YYoouuttuubbee vviiddeeooss ttoo aa ppllaayylliisstt.. ********
 _[_P_r_o_j_e_c_t_ _S_t_a_t_u_s_:_ _A_c_t_i_v_e_ _â___ _T_h_e_ _p_r_o_j_e_c_t_ _h_a_s_ _r_e_a_c_h_e_d_ _a_ _s_t_a_b_l_e_,_ _u_s_a_b_l_e_ _s_t_a_t_e_ _a_n_d
-   _i_s_ _b_e_i_n_g_ _a_c_t_i_v_e_l_y_ _d_e_v_e_l_o_p_e_d_._]_[_L_a_t_e_s_t_ _V_e_r_s_i_o_n_]_[_O_p_e_n_ _I_s_s_u_e_s_]_[_C_l_o_s_e_d_ _I_s_s_u_e_s_]
-                    _[_L_i_c_e_n_s_e_]_[_C_o_d_e_ _s_t_y_l_e_:_ _b_l_a_c_k_]_[_C_o_d_e_ _S_i_z_e_]
+  _i_s_ _b_e_i_n_g_ _a_c_t_i_v_e_l_y_ _d_e_v_e_l_o_p_e_d_._]_[_L_a_t_e_s_t_ _V_e_r_s_i_o_n_]_[_P_y_P_i_ _D_o_w_n_l_o_a_d_s_]_[_O_p_e_n_ _I_s_s_u_e_s_]
+            _[_C_l_o_s_e_d_ _I_s_s_u_e_s_]_[_L_i_c_e_n_s_e_]_[_C_o_d_e_ _s_t_y_l_e_:_ _b_l_a_c_k_]_[_C_o_d_e_ _S_i_z_e_]
     _A_b_o_u_t â¢ _F_e_a_t_u_r_e_s â¢ _H_o_w_ _T_o_ _U_s_e â¢ _E_x_a_m_p_l_e_s â¢ _F_A_Q â¢ _C_o_n_t_a_c_t â¢
                           _A_c_k_n_o_w_l_e_d_g_m_e_n_t_s â¢ _L_i_c_e_n_s_e
 ## About The reason for the existence of this software is Youtube's seemingly
 random behavior when it comes to notifying people that a new video has been
 published (late or missing notifications, useless notification bell, videos not
 appearing in the subscription tab, ...). With this software, you can set a
 number of rules that determine which videos are added to a dedicated playlist,
@@ -50,31 +50,35 @@
 features are available: * Channel name filtering * Title filtering *
 Description filtering * Tags filtering * Language filtering * Caption filtering
 * Duration filtering * Quality filtering * Upload date filtering * Shorts
 filtering * Duplicate checking ## How to use Before using this software, you
 first need to get a Youtube API key and create a web app to get a client
 secrets file (that should look like [this](docs/client_secrets_template.json)).
 This [Corey Schafer video](https://www.youtube.com/watch?v=vQQEaSnQ_bs) goes
-through the process step by step. Once that's done, either clone this
-repository or download the ZIP archive. Then, copy and rename the [user
-parameters template](docs/user_params_template.json) file to
-*user_params.json*. Modify it so that it fits your needs (more information on
-how in the [following table](#user-defined-parameters) and in the [examples
-section](#examples)). Verify that you have all of the dependencies installed
-(see the [requirements](requirements.txt) file). Finally, execute the [run.py]
-(QTube/run.py) file to start the software. I would recommend creating a task to
-execute the program regularly (like once a day). For more versatile uses, you
-can also use command line arguments with the [run.py](QTube/run.py) file.
-Enable this option by setting the parameter `override_json` to *True* in your
-JSON user parameters file. Provided command line arguments will then override
-what is in your JSON user parameters file. ### User-defined parameters
-|Parameter|Optional|Description|Possible values| |--|:--:|:--:|:--:
-| |`required_in_channel_name`|Yes|Words that must be in channel names,
-typically channel names themselves. Videos from channels not containing any of
-the words of this list in their name will not be added.|Any string|
+through the process step by step. Once that's done, download this project or
+install the package with [PyPI](https://pypi.org/project/QTube/). Then, copy
+the [user parameters template](docs/user_params_template.json) file to the main
+QTube directory and rename it to *user_params.json*. Modify it so that it fits
+your needs (more information on how in the [following table](#user-defined-
+parameters) and in the [examples section](#examples)). Verify that you have all
+of the dependencies installed (see the [requirements](requirements.txt) file or
+the [TOML](pyproject.toml) file). Finally, execute the [qtube.py](QTube/
+scripts/qtube.py) file to start the software, either by running the file
+directly or by using the CLI ***qtube*** in the main directory. I would
+recommend creating a task to execute the program regularly (like once a day).
+For more versatile uses, you can also use command line arguments with the
+[qtube.py](QTube/scripts/qtube.py) file. Enable this option by setting the
+parameter `override_json` to *True* in your JSON user parameters file. Provided
+command line arguments will then override what is in your JSON user parameters
+file. This is especially useful to manage different types of videos and put
+them in dedicated playlists (music playlist, gaming playlist, ect...). ###
+User-defined parameters |Parameter|Optional|Description|Possible values| |--|:-
+-:|:--:|:--:| |`required_in_channel_name`|Yes|Words that must be in channel
+names, typically channel names themselves. Videos from channels not containing
+any of the words of this list in their name will not be added.|Any string|
 |`banned_in_channel_name`|Yes|Words that must not be in channel names,
 typically channel names themselves. Videos from channels containing any of the
 words of this list in their name will not be added.|Any string|
 |`include_extra_channels`|No|Determines whether to include channels the user is
 not subscribed to.|boolean| |`extra_channel_handles`|Yes|Handles of additional
 channels to be checked. Handles are found at the end of a channel's URL:
 `https://www.youtube.com/@*handle*`|Any channel handle|
@@ -132,44 +136,44 @@
 *none* 2 ,
 *func* 3 ,
 *credentials* 4 ,
 *videos* 5 .| All parameters are case-sensitive by default and if you do not
 want to use an optional parameter, replace its value with *null* or delete the
 entry. For further information about each parameter, check the note associated
 with the [release](https://github.com/Killian42/QTube/releases) they were
-introduced in. ### Requirements See the [requirements](requirements.txt) file.
-## Examples This section presents examples of user parameters json files for
-concrete use-cases. * _E_v_e_r_y_ _v_i_d_e_o_s_ _f_r_o_m_ _s_u_b_s_c_r_i_b_e_d_ _c_h_a_n_n_e_l_s * _H_i_g_h_e_r_ _q_u_a_l_i_t_y
-_v_i_d_e_o_s * _V_i_d_e_o_ _s_e_r_i_e_s_ _f_r_o_m_ _a_ _c_r_e_a_t_o_r ### Example 1 - Every videos from
-subscribed channels The following *user_params.json* file would add every new
-videos from channels you are subcribed to. ``` { "required_in_channel_name":
-null, "banned_in_channel_name": null, "include_extra_channels": false,
-"extra_channel_handles": null, "required_in_title": null, "banned_in_title":
-null, "ignore_title_emojis": false, "ignore_title_punctuation": false,
-"ignore_title_case": false, "required_in_description": null,
-"banned_in_description": null, "required_tags": null, "banned_tags": null,
-"preferred_languages": null, "require_captions":false, "caption_options": null,
-"allowed_durations": null, "lowest_definition": null, "lowest_resolution":
-null, "lowest_framerate": null, "preferred_dimensions": null,
-"preferred_projections": null, "run_frequency":"daily", "keep_shorts": true,
-"keep_duplicates": false, "upload_playlist_ID": "your_playlist_ID",
-"override_json":false, "verbosity": ["credentials","videos"] } ``` ### Example
-2 - Higher quality videos The following *user_params.json* file would only add
-videos with good quality. ``` { "required_in_channel_name": null,
-"banned_in_channel_name": null, "include_extra_channels": false,
-"extra_channel_handles": null, "required_in_title": null, "banned_in_title":
-null, "ignore_title_emojis": false, "ignore_title_punctuation": false,
-"ignore_title_case": false, "required_in_description": null,
-"banned_in_description": null, "required_tags": null, "banned_tags": null,
-"preferred_languages": null, "require_captions":false, "caption_options": null,
-"allowed_durations": null, "lowest_definition": "HD", "lowest_resolution":
-"1080p", "lowest_framerate": 60, "preferred_dimensions": ["2D"],
-"preferred_projections": ["rectangular"], "run_frequency":"daily",
-"keep_shorts": true, "keep_duplicates": false, "upload_playlist_ID":
+introduced in. ### Requirements See the [requirements](requirements.txt) file
+or the [TOML](pyproject.toml) file. ## Examples This section presents examples
+of user parameters json files for concrete use-cases. * _E_v_e_r_y_ _v_i_d_e_o_s_ _f_r_o_m
+_s_u_b_s_c_r_i_b_e_d_ _c_h_a_n_n_e_l_s * _H_i_g_h_e_r_ _q_u_a_l_i_t_y_ _v_i_d_e_o_s * _V_i_d_e_o_ _s_e_r_i_e_s_ _f_r_o_m_ _a_ _c_r_e_a_t_o_r ###
+Example 1 - Every videos from subscribed channels The following
+*user_params.json* file would add every new videos from channels you are
+subcribed to. ``` { "required_in_channel_name": null, "banned_in_channel_name":
+null, "include_extra_channels": false, "extra_channel_handles": null,
+"required_in_title": null, "banned_in_title": null, "ignore_title_emojis":
+false, "ignore_title_punctuation": false, "ignore_title_case": false,
+"required_in_description": null, "banned_in_description": null,
+"required_tags": null, "banned_tags": null, "preferred_languages": null,
+"require_captions":false, "caption_options": null, "allowed_durations": null,
+"lowest_definition": null, "lowest_resolution": null, "lowest_framerate": null,
+"preferred_dimensions": null, "preferred_projections": null, "run_frequency":
+"daily", "keep_shorts": true, "keep_duplicates": false, "upload_playlist_ID":
 "your_playlist_ID", "override_json":false, "verbosity":
+["credentials","videos"] } ``` ### Example 2 - Higher quality videos The
+following *user_params.json* file would only add videos with good quality. ```
+{ "required_in_channel_name": null, "banned_in_channel_name": null,
+"include_extra_channels": false, "extra_channel_handles": null,
+"required_in_title": null, "banned_in_title": null, "ignore_title_emojis":
+false, "ignore_title_punctuation": false, "ignore_title_case": false,
+"required_in_description": null, "banned_in_description": null,
+"required_tags": null, "banned_tags": null, "preferred_languages": null,
+"require_captions":false, "caption_options": null, "allowed_durations": null,
+"lowest_definition": "HD", "lowest_resolution": "1080p", "lowest_framerate":
+60, "preferred_dimensions": ["2D"], "preferred_projections": ["rectangular"],
+"run_frequency":"daily", "keep_shorts": true, "keep_duplicates": false,
+"upload_playlist_ID": "your_playlist_ID", "override_json":false, "verbosity":
 ["credentials","videos"] } ``` ### Example 3 - Specific video series from a
 creator The following *user_params.json* file would only add the *$1 vs.*
 MrBeast videos. ``` { "required_in_channel_name": ["MrBeast"],
 "banned_in_channel_name": null, "include_extra_channels": false,
 "extra_channel_handles": null, "required_in_title": ["$1 vs."],
 "banned_in_title": null, "ignore_title_emojis": true,
 "ignore_title_punctuation": false, "ignore_title_case": true,
```

### Comparing `QTube-2.0.0/QTube/scripts/qtube.py` & `qtube-2.0.0a0/QTube/scripts/qtube.py`

 * *Files 1% similar despite different names*

```diff
@@ -665,15 +665,15 @@
         vid_ID: vid_info for vid_ID, vid_info in videos.items() if vid_info["to add"]
     }
 
     ## Adding selected videos to a playlist
     playlist_title = QTube.utils.youtube.playlists.get_playlists_titles(
         youtube, [playlist_ID]
     )[0]
-    if videos_to_add is not None:  # Checks if there are actually videos to add
+    if len(videos_to_add)!=0:  # Checks if there are actually videos to add
         QTube.utils.helpers.print2(
             f"The following videos will be added to the {playlist_title} playlist:",
             ["all", "videos"],
             verb,
         )
         for vid_ID, vid_info in videos_to_add.items():
             QTube.utils.helpers.handle_http_errors(
@@ -687,15 +687,15 @@
             QTube.utils.helpers.print2(
                 f"From {vid_info['channel name']}, the video named: {vid_info['original title']} has been added.",
                 ["all", "videos"],
                 verb,
             )
     else:
         QTube.utils.helpers.print2(
-            f"No videos from yesterday to add to the {playlist_title} playlist.",
+            f"No new videos to add to the {playlist_title} playlist.",
             ["all", "videos"],
             verb,
         )
 
 
 if __name__ == "__main__":
     main()
```

### Comparing `QTube-2.0.0/QTube/scripts/tests.py` & `qtube-2.0.0a0/QTube/scripts/tests.py`

 * *Files identical despite different names*

### Comparing `QTube-2.0.0/QTube/utils/checks.py` & `qtube-2.0.0a0/QTube/utils/checks.py`

 * *Files identical despite different names*

### Comparing `QTube-2.0.0/QTube/utils/helpers.py` & `qtube-2.0.0a0/QTube/utils/helpers.py`

 * *Files identical despite different names*

### Comparing `QTube-2.0.0/QTube/utils/parsing.py` & `qtube-2.0.0a0/QTube/utils/parsing.py`

 * *Files identical despite different names*

### Comparing `QTube-2.0.0/QTube/utils/youtube/captions.py` & `qtube-2.0.0a0/QTube/utils/youtube/captions.py`

 * *Files identical despite different names*

### Comparing `QTube-2.0.0/QTube/utils/youtube/channels.py` & `qtube-2.0.0a0/QTube/utils/youtube/channels.py`

 * *Files identical despite different names*

### Comparing `QTube-2.0.0/QTube/utils/youtube/playlists.py` & `qtube-2.0.0a0/QTube/utils/youtube/playlists.py`

 * *Files identical despite different names*

### Comparing `QTube-2.0.0/QTube/utils/youtube/videos.py` & `qtube-2.0.0a0/QTube/utils/youtube/videos.py`

 * *Files identical despite different names*

### Comparing `QTube-2.0.0/QTube.egg-info/PKG-INFO` & `qtube-2.0.0a0/QTube.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: QTube
-Version: 2.0.0
+Version: 2.0.0a0
 Summary: Automatically add Youtube videos to a playlist.
 Home-page: https://github.com/Killian42/QTube
 Author: Killian Lebreton
 Author-email: Killian Lebreton <killian.lebreton35@gmail.com>
 Maintainer-email: Killian Lebreton <killian.lebreton35@gmail.com>
 License: MIT License
         
@@ -51,23 +51,24 @@
 Requires-Dist: protobuf>=4.25.1
 Requires-Dist: pytube>=15.0.0
 Requires-Dist: Requests>=2.31.0
 Requires-Dist: setuptools>=68.2.2
 
 <h1 align="center">
    <br>
-   <a href="https://github.com/Killian42/QTube/releases/latest"><img src="logo.png" alt="QTube" width="500"></a>
+   <a href="https://github.com/Killian42/QTube/releases/latest"><img src="https://i.postimg.cc/wMLMYv3M/logo.png" alt="QTube" width="500"></a>
    <br>
 </h1>
 
 <h3 align="center">Automatically add Youtube videos to a playlist.</h3>
 
 <p align="center">
    <a href="https://www.repostatus.org/#active"><img src="https://www.repostatus.org/badges/latest/active.svg" alt="Project Status: Active – The project has reached a stable, usable state and is being actively developed." /></a>
    <a href="https://github.com/Killian42/QTube/releases/latest"><img src="https://img.shields.io/github/v/release/Killian42/QTube" alt="Latest Version"></a>
+   <a href="https://pypi.org/project/QTube/"><img src="https://img.shields.io/pypi/dm/QTube.svg?label=PyPI%20downloads" alt="PyPi Downloads"></a>
    <a href="https://github.com/Killian42/QTube/issues"><img src="https://img.shields.io/github/issues/Killian42/QTube" alt="Open Issues"></a>
    <a href="https://github.com/Killian42/QTube/issues?q=is%3Aissue+is%3Aclosed"><img src="https://img.shields.io/github/issues-closed/Killian42/QTube?color=sucess" alt="Closed Issues"></a>
    <a href="https://opensource.org/licenses/MIT"><img src="https://img.shields.io/badge/license-MIT-green" alt="License"></a>
    <a href="https://github.com/psf/black"><img src="https://img.shields.io/badge/code%20style-black-000000.svg" alt="Code style: black"></a>
    <a href="https://github.com/Killian42/QTube"><img src="https://img.shields.io/github/languages/code-size/Killian42/QTube" alt="Code Size"></a>
 </p>
 
@@ -100,23 +101,23 @@
 * Upload date filtering
 * Shorts filtering
 * Duplicate checking
 
 ## How to use
 Before using this software, you first need to get a Youtube API key and create a web app to get a client secrets file (that should look like [this](docs/client_secrets_template.json)). This [Corey Schafer video](https://www.youtube.com/watch?v=vQQEaSnQ_bs) goes through the process step by step.
 
-Once that's done, either clone this repository or download the ZIP archive. Then, copy and rename the [user parameters template](docs/user_params_template.json) file to *user_params.json*. Modify it so that it fits your needs (more information on how in the [following table](#user-defined-parameters) and in the [examples section](#examples)).
+Once that's done, download this project or install the package with [PyPI](https://pypi.org/project/QTube/). Then, copy the [user parameters template](docs/user_params_template.json) file to the main QTube directory and rename it to *user_params.json*. Modify it so that it fits your needs (more information on how in the [following table](#user-defined-parameters) and in the [examples section](#examples)).
 
-Verify that you have all of the dependencies installed (see the [requirements](requirements.txt) file).
+Verify that you have all of the dependencies installed (see the [requirements](requirements.txt) file or the [TOML](pyproject.toml) file).
 
-Finally, execute the [run.py](QTube/run.py) file to start the software.
+Finally, execute the [qtube.py](QTube/scripts/qtube.py) file to start the software, either by running the file directly or by using the CLI ***qtube*** in the main directory.
 
 I would recommend creating a task to execute the program regularly (like once a day).
 
-For more versatile uses, you can also use command line arguments with the [run.py](QTube/run.py) file. Enable this option by setting the parameter `override_json` to *True* in your JSON user parameters file. Provided command line arguments will then override what is in your JSON user parameters file.
+For more versatile uses, you can also use command line arguments with the [qtube.py](QTube/scripts/qtube.py) file. Enable this option by setting the parameter `override_json` to *True* in your JSON user parameters file. Provided command line arguments will then override what is in your JSON user parameters file. This is especially useful to manage different types of videos and put them in dedicated playlists (music playlist, gaming playlist, ect...).
 
 ### User-defined parameters
 |Parameter|Optional|Description|Possible values|
 |--|:--:|:--:|:--:|
 |`required_in_channel_name`|Yes|Words that must be in channel names, typically channel names themselves. Videos from channels not containing any of the words of this list in their name will not be added.|Any string|
 |`banned_in_channel_name`|Yes|Words that must not be in channel names, typically channel names themselves. Videos from channels containing any of the words of this list in their name will not be added.|Any string|
 |`include_extra_channels`|No|Determines whether to include channels the user is not subscribed to.|boolean|
@@ -146,15 +147,15 @@
 |`override_json`|No|Allow command line arguments to override user_params.json parameters.|boolean|
 |`verbosity`|No|Controls how much information is shown in the terminal. Options can be combined, so that selecting each option gives the same result as selecting *all*. <br>1: Everything is shown.<br>2: Nothing is shown.<br>3: Only information regarding function execution is shown.<br>4: Only information regarding credentials is shown (loading, retrieving and saving).<br>5: Only information regarding added videos is shown (number, channel names and video titles).|<br>*all*<sup> 1 </sup>, <br>*none*<sup> 2 </sup> , <br>*func*<sup> 3 </sup>, <br>*credentials*<sup> 4 </sup> ,<br>*videos*<sup> 5 </sup>.|
 
 All parameters are case-sensitive by default and if you do not want to use an optional parameter, replace its value with *null* or delete the entry.
 
 For further information about each parameter, check the note associated with the [release](https://github.com/Killian42/QTube/releases) they were introduced in.
 ### Requirements
-See the [requirements](requirements.txt) file.
+See the [requirements](requirements.txt) file or the [TOML](pyproject.toml) file.
 
 ## Examples
 This section presents examples of user parameters json files for concrete use-cases.
 * <a href="#example-1---every-videos-from-subscribed-channels">Every videos from subscribed channels</a>
 * <a href="#example-2---higher-quality-videos">Higher quality videos</a>
 * <a href="#example-3---specific-video-series-from-a-creator">Video series from a creator</a>
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: QTube Version: 2.0.0 Summary: Automatically add
+Metadata-Version: 2.1 Name: QTube Version: 2.0.0a0 Summary: Automatically add
 Youtube videos to a playlist. Home-page: https://github.com/Killian42/QTube
 Author: Killian Lebreton Author-email: Killian Lebreton
 gmail.com> Maintainer-email: Killian Lebreton
 gmail.com> License: MIT License Copyright (c) [2024] [Killian Lebreton]
 Permission is hereby granted, free of charge, to any person obtaining a copy of
 this software and associated documentation files (the "Software"), to deal in
 the Software without restriction, including without limitation the rights to
@@ -32,16 +32,16 @@
 protobuf>=4.25.1 Requires-Dist: pytube>=15.0.0 Requires-Dist: Requests>=2.31.0
 Requires-Dist: setuptools>=68.2.2
                                     ************
                                     _[[_QQ_TT_uu_bb_ee_]]
                                      ************
            ******** AAuuttoommaattiiccaallllyy aadddd YYoouuttuubbee vviiddeeooss ttoo aa ppllaayylliisstt.. ********
 _[_P_r_o_j_e_c_t_ _S_t_a_t_u_s_:_ _A_c_t_i_v_e_ _â___ _T_h_e_ _p_r_o_j_e_c_t_ _h_a_s_ _r_e_a_c_h_e_d_ _a_ _s_t_a_b_l_e_,_ _u_s_a_b_l_e_ _s_t_a_t_e_ _a_n_d
-   _i_s_ _b_e_i_n_g_ _a_c_t_i_v_e_l_y_ _d_e_v_e_l_o_p_e_d_._]_[_L_a_t_e_s_t_ _V_e_r_s_i_o_n_]_[_O_p_e_n_ _I_s_s_u_e_s_]_[_C_l_o_s_e_d_ _I_s_s_u_e_s_]
-                    _[_L_i_c_e_n_s_e_]_[_C_o_d_e_ _s_t_y_l_e_:_ _b_l_a_c_k_]_[_C_o_d_e_ _S_i_z_e_]
+  _i_s_ _b_e_i_n_g_ _a_c_t_i_v_e_l_y_ _d_e_v_e_l_o_p_e_d_._]_[_L_a_t_e_s_t_ _V_e_r_s_i_o_n_]_[_P_y_P_i_ _D_o_w_n_l_o_a_d_s_]_[_O_p_e_n_ _I_s_s_u_e_s_]
+            _[_C_l_o_s_e_d_ _I_s_s_u_e_s_]_[_L_i_c_e_n_s_e_]_[_C_o_d_e_ _s_t_y_l_e_:_ _b_l_a_c_k_]_[_C_o_d_e_ _S_i_z_e_]
     _A_b_o_u_t â¢ _F_e_a_t_u_r_e_s â¢ _H_o_w_ _T_o_ _U_s_e â¢ _E_x_a_m_p_l_e_s â¢ _F_A_Q â¢ _C_o_n_t_a_c_t â¢
                           _A_c_k_n_o_w_l_e_d_g_m_e_n_t_s â¢ _L_i_c_e_n_s_e
 ## About The reason for the existence of this software is Youtube's seemingly
 random behavior when it comes to notifying people that a new video has been
 published (late or missing notifications, useless notification bell, videos not
 appearing in the subscription tab, ...). With this software, you can set a
 number of rules that determine which videos are added to a dedicated playlist,
@@ -50,31 +50,35 @@
 features are available: * Channel name filtering * Title filtering *
 Description filtering * Tags filtering * Language filtering * Caption filtering
 * Duration filtering * Quality filtering * Upload date filtering * Shorts
 filtering * Duplicate checking ## How to use Before using this software, you
 first need to get a Youtube API key and create a web app to get a client
 secrets file (that should look like [this](docs/client_secrets_template.json)).
 This [Corey Schafer video](https://www.youtube.com/watch?v=vQQEaSnQ_bs) goes
-through the process step by step. Once that's done, either clone this
-repository or download the ZIP archive. Then, copy and rename the [user
-parameters template](docs/user_params_template.json) file to
-*user_params.json*. Modify it so that it fits your needs (more information on
-how in the [following table](#user-defined-parameters) and in the [examples
-section](#examples)). Verify that you have all of the dependencies installed
-(see the [requirements](requirements.txt) file). Finally, execute the [run.py]
-(QTube/run.py) file to start the software. I would recommend creating a task to
-execute the program regularly (like once a day). For more versatile uses, you
-can also use command line arguments with the [run.py](QTube/run.py) file.
-Enable this option by setting the parameter `override_json` to *True* in your
-JSON user parameters file. Provided command line arguments will then override
-what is in your JSON user parameters file. ### User-defined parameters
-|Parameter|Optional|Description|Possible values| |--|:--:|:--:|:--:
-| |`required_in_channel_name`|Yes|Words that must be in channel names,
-typically channel names themselves. Videos from channels not containing any of
-the words of this list in their name will not be added.|Any string|
+through the process step by step. Once that's done, download this project or
+install the package with [PyPI](https://pypi.org/project/QTube/). Then, copy
+the [user parameters template](docs/user_params_template.json) file to the main
+QTube directory and rename it to *user_params.json*. Modify it so that it fits
+your needs (more information on how in the [following table](#user-defined-
+parameters) and in the [examples section](#examples)). Verify that you have all
+of the dependencies installed (see the [requirements](requirements.txt) file or
+the [TOML](pyproject.toml) file). Finally, execute the [qtube.py](QTube/
+scripts/qtube.py) file to start the software, either by running the file
+directly or by using the CLI ***qtube*** in the main directory. I would
+recommend creating a task to execute the program regularly (like once a day).
+For more versatile uses, you can also use command line arguments with the
+[qtube.py](QTube/scripts/qtube.py) file. Enable this option by setting the
+parameter `override_json` to *True* in your JSON user parameters file. Provided
+command line arguments will then override what is in your JSON user parameters
+file. This is especially useful to manage different types of videos and put
+them in dedicated playlists (music playlist, gaming playlist, ect...). ###
+User-defined parameters |Parameter|Optional|Description|Possible values| |--|:-
+-:|:--:|:--:| |`required_in_channel_name`|Yes|Words that must be in channel
+names, typically channel names themselves. Videos from channels not containing
+any of the words of this list in their name will not be added.|Any string|
 |`banned_in_channel_name`|Yes|Words that must not be in channel names,
 typically channel names themselves. Videos from channels containing any of the
 words of this list in their name will not be added.|Any string|
 |`include_extra_channels`|No|Determines whether to include channels the user is
 not subscribed to.|boolean| |`extra_channel_handles`|Yes|Handles of additional
 channels to be checked. Handles are found at the end of a channel's URL:
 `https://www.youtube.com/@*handle*`|Any channel handle|
@@ -132,44 +136,44 @@
 *none* 2 ,
 *func* 3 ,
 *credentials* 4 ,
 *videos* 5 .| All parameters are case-sensitive by default and if you do not
 want to use an optional parameter, replace its value with *null* or delete the
 entry. For further information about each parameter, check the note associated
 with the [release](https://github.com/Killian42/QTube/releases) they were
-introduced in. ### Requirements See the [requirements](requirements.txt) file.
-## Examples This section presents examples of user parameters json files for
-concrete use-cases. * _E_v_e_r_y_ _v_i_d_e_o_s_ _f_r_o_m_ _s_u_b_s_c_r_i_b_e_d_ _c_h_a_n_n_e_l_s * _H_i_g_h_e_r_ _q_u_a_l_i_t_y
-_v_i_d_e_o_s * _V_i_d_e_o_ _s_e_r_i_e_s_ _f_r_o_m_ _a_ _c_r_e_a_t_o_r ### Example 1 - Every videos from
-subscribed channels The following *user_params.json* file would add every new
-videos from channels you are subcribed to. ``` { "required_in_channel_name":
-null, "banned_in_channel_name": null, "include_extra_channels": false,
-"extra_channel_handles": null, "required_in_title": null, "banned_in_title":
-null, "ignore_title_emojis": false, "ignore_title_punctuation": false,
-"ignore_title_case": false, "required_in_description": null,
-"banned_in_description": null, "required_tags": null, "banned_tags": null,
-"preferred_languages": null, "require_captions":false, "caption_options": null,
-"allowed_durations": null, "lowest_definition": null, "lowest_resolution":
-null, "lowest_framerate": null, "preferred_dimensions": null,
-"preferred_projections": null, "run_frequency":"daily", "keep_shorts": true,
-"keep_duplicates": false, "upload_playlist_ID": "your_playlist_ID",
-"override_json":false, "verbosity": ["credentials","videos"] } ``` ### Example
-2 - Higher quality videos The following *user_params.json* file would only add
-videos with good quality. ``` { "required_in_channel_name": null,
-"banned_in_channel_name": null, "include_extra_channels": false,
-"extra_channel_handles": null, "required_in_title": null, "banned_in_title":
-null, "ignore_title_emojis": false, "ignore_title_punctuation": false,
-"ignore_title_case": false, "required_in_description": null,
-"banned_in_description": null, "required_tags": null, "banned_tags": null,
-"preferred_languages": null, "require_captions":false, "caption_options": null,
-"allowed_durations": null, "lowest_definition": "HD", "lowest_resolution":
-"1080p", "lowest_framerate": 60, "preferred_dimensions": ["2D"],
-"preferred_projections": ["rectangular"], "run_frequency":"daily",
-"keep_shorts": true, "keep_duplicates": false, "upload_playlist_ID":
+introduced in. ### Requirements See the [requirements](requirements.txt) file
+or the [TOML](pyproject.toml) file. ## Examples This section presents examples
+of user parameters json files for concrete use-cases. * _E_v_e_r_y_ _v_i_d_e_o_s_ _f_r_o_m
+_s_u_b_s_c_r_i_b_e_d_ _c_h_a_n_n_e_l_s * _H_i_g_h_e_r_ _q_u_a_l_i_t_y_ _v_i_d_e_o_s * _V_i_d_e_o_ _s_e_r_i_e_s_ _f_r_o_m_ _a_ _c_r_e_a_t_o_r ###
+Example 1 - Every videos from subscribed channels The following
+*user_params.json* file would add every new videos from channels you are
+subcribed to. ``` { "required_in_channel_name": null, "banned_in_channel_name":
+null, "include_extra_channels": false, "extra_channel_handles": null,
+"required_in_title": null, "banned_in_title": null, "ignore_title_emojis":
+false, "ignore_title_punctuation": false, "ignore_title_case": false,
+"required_in_description": null, "banned_in_description": null,
+"required_tags": null, "banned_tags": null, "preferred_languages": null,
+"require_captions":false, "caption_options": null, "allowed_durations": null,
+"lowest_definition": null, "lowest_resolution": null, "lowest_framerate": null,
+"preferred_dimensions": null, "preferred_projections": null, "run_frequency":
+"daily", "keep_shorts": true, "keep_duplicates": false, "upload_playlist_ID":
 "your_playlist_ID", "override_json":false, "verbosity":
+["credentials","videos"] } ``` ### Example 2 - Higher quality videos The
+following *user_params.json* file would only add videos with good quality. ```
+{ "required_in_channel_name": null, "banned_in_channel_name": null,
+"include_extra_channels": false, "extra_channel_handles": null,
+"required_in_title": null, "banned_in_title": null, "ignore_title_emojis":
+false, "ignore_title_punctuation": false, "ignore_title_case": false,
+"required_in_description": null, "banned_in_description": null,
+"required_tags": null, "banned_tags": null, "preferred_languages": null,
+"require_captions":false, "caption_options": null, "allowed_durations": null,
+"lowest_definition": "HD", "lowest_resolution": "1080p", "lowest_framerate":
+60, "preferred_dimensions": ["2D"], "preferred_projections": ["rectangular"],
+"run_frequency":"daily", "keep_shorts": true, "keep_duplicates": false,
+"upload_playlist_ID": "your_playlist_ID", "override_json":false, "verbosity":
 ["credentials","videos"] } ``` ### Example 3 - Specific video series from a
 creator The following *user_params.json* file would only add the *$1 vs.*
 MrBeast videos. ``` { "required_in_channel_name": ["MrBeast"],
 "banned_in_channel_name": null, "include_extra_channels": false,
 "extra_channel_handles": null, "required_in_title": ["$1 vs."],
 "banned_in_title": null, "ignore_title_emojis": true,
 "ignore_title_punctuation": false, "ignore_title_case": true,
```

### Comparing `QTube-2.0.0/QTube.egg-info/SOURCES.txt` & `qtube-2.0.0a0/QTube.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `QTube-2.0.0/README.md` & `qtube-2.0.0a0/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -1,18 +1,19 @@
 <h1 align="center">
    <br>
-   <a href="https://github.com/Killian42/QTube/releases/latest"><img src="logo.png" alt="QTube" width="500"></a>
+   <a href="https://github.com/Killian42/QTube/releases/latest"><img src="https://i.postimg.cc/wMLMYv3M/logo.png" alt="QTube" width="500"></a>
    <br>
 </h1>
 
 <h3 align="center">Automatically add Youtube videos to a playlist.</h3>
 
 <p align="center">
    <a href="https://www.repostatus.org/#active"><img src="https://www.repostatus.org/badges/latest/active.svg" alt="Project Status: Active – The project has reached a stable, usable state and is being actively developed." /></a>
    <a href="https://github.com/Killian42/QTube/releases/latest"><img src="https://img.shields.io/github/v/release/Killian42/QTube" alt="Latest Version"></a>
+   <a href="https://pypi.org/project/QTube/"><img src="https://img.shields.io/pypi/dm/QTube.svg?label=PyPI%20downloads" alt="PyPi Downloads"></a>
    <a href="https://github.com/Killian42/QTube/issues"><img src="https://img.shields.io/github/issues/Killian42/QTube" alt="Open Issues"></a>
    <a href="https://github.com/Killian42/QTube/issues?q=is%3Aissue+is%3Aclosed"><img src="https://img.shields.io/github/issues-closed/Killian42/QTube?color=sucess" alt="Closed Issues"></a>
    <a href="https://opensource.org/licenses/MIT"><img src="https://img.shields.io/badge/license-MIT-green" alt="License"></a>
    <a href="https://github.com/psf/black"><img src="https://img.shields.io/badge/code%20style-black-000000.svg" alt="Code style: black"></a>
    <a href="https://github.com/Killian42/QTube"><img src="https://img.shields.io/github/languages/code-size/Killian42/QTube" alt="Code Size"></a>
 </p>
 
@@ -45,23 +46,23 @@
 * Upload date filtering
 * Shorts filtering
 * Duplicate checking
 
 ## How to use
 Before using this software, you first need to get a Youtube API key and create a web app to get a client secrets file (that should look like [this](docs/client_secrets_template.json)). This [Corey Schafer video](https://www.youtube.com/watch?v=vQQEaSnQ_bs) goes through the process step by step.
 
-Once that's done, either clone this repository or download the ZIP archive. Then, copy and rename the [user parameters template](docs/user_params_template.json) file to *user_params.json*. Modify it so that it fits your needs (more information on how in the [following table](#user-defined-parameters) and in the [examples section](#examples)).
+Once that's done, download this project or install the package with [PyPI](https://pypi.org/project/QTube/). Then, copy the [user parameters template](docs/user_params_template.json) file to the main QTube directory and rename it to *user_params.json*. Modify it so that it fits your needs (more information on how in the [following table](#user-defined-parameters) and in the [examples section](#examples)).
 
-Verify that you have all of the dependencies installed (see the [requirements](requirements.txt) file).
+Verify that you have all of the dependencies installed (see the [requirements](requirements.txt) file or the [TOML](pyproject.toml) file).
 
-Finally, execute the [run.py](QTube/run.py) file to start the software.
+Finally, execute the [qtube.py](QTube/scripts/qtube.py) file to start the software, either by running the file directly or by using the CLI ***qtube*** in the main directory.
 
 I would recommend creating a task to execute the program regularly (like once a day).
 
-For more versatile uses, you can also use command line arguments with the [run.py](QTube/run.py) file. Enable this option by setting the parameter `override_json` to *True* in your JSON user parameters file. Provided command line arguments will then override what is in your JSON user parameters file.
+For more versatile uses, you can also use command line arguments with the [qtube.py](QTube/scripts/qtube.py) file. Enable this option by setting the parameter `override_json` to *True* in your JSON user parameters file. Provided command line arguments will then override what is in your JSON user parameters file. This is especially useful to manage different types of videos and put them in dedicated playlists (music playlist, gaming playlist, ect...).
 
 ### User-defined parameters
 |Parameter|Optional|Description|Possible values|
 |--|:--:|:--:|:--:|
 |`required_in_channel_name`|Yes|Words that must be in channel names, typically channel names themselves. Videos from channels not containing any of the words of this list in their name will not be added.|Any string|
 |`banned_in_channel_name`|Yes|Words that must not be in channel names, typically channel names themselves. Videos from channels containing any of the words of this list in their name will not be added.|Any string|
 |`include_extra_channels`|No|Determines whether to include channels the user is not subscribed to.|boolean|
@@ -91,15 +92,15 @@
 |`override_json`|No|Allow command line arguments to override user_params.json parameters.|boolean|
 |`verbosity`|No|Controls how much information is shown in the terminal. Options can be combined, so that selecting each option gives the same result as selecting *all*. <br>1: Everything is shown.<br>2: Nothing is shown.<br>3: Only information regarding function execution is shown.<br>4: Only information regarding credentials is shown (loading, retrieving and saving).<br>5: Only information regarding added videos is shown (number, channel names and video titles).|<br>*all*<sup> 1 </sup>, <br>*none*<sup> 2 </sup> , <br>*func*<sup> 3 </sup>, <br>*credentials*<sup> 4 </sup> ,<br>*videos*<sup> 5 </sup>.|
 
 All parameters are case-sensitive by default and if you do not want to use an optional parameter, replace its value with *null* or delete the entry.
 
 For further information about each parameter, check the note associated with the [release](https://github.com/Killian42/QTube/releases) they were introduced in.
 ### Requirements
-See the [requirements](requirements.txt) file.
+See the [requirements](requirements.txt) file or the [TOML](pyproject.toml) file.
 
 ## Examples
 This section presents examples of user parameters json files for concrete use-cases.
 * <a href="#example-1---every-videos-from-subscribed-channels">Every videos from subscribed channels</a>
 * <a href="#example-2---higher-quality-videos">Higher quality videos</a>
 * <a href="#example-3---specific-video-series-from-a-creator">Video series from a creator</a>
```

#### html2text {}

```diff
@@ -1,14 +1,14 @@
                                     ************
                                     _[[_QQ_TT_uu_bb_ee_]]
                                      ************
            ******** AAuuttoommaattiiccaallllyy aadddd YYoouuttuubbee vviiddeeooss ttoo aa ppllaayylliisstt.. ********
 _[_P_r_o_j_e_c_t_ _S_t_a_t_u_s_:_ _A_c_t_i_v_e_ _â___ _T_h_e_ _p_r_o_j_e_c_t_ _h_a_s_ _r_e_a_c_h_e_d_ _a_ _s_t_a_b_l_e_,_ _u_s_a_b_l_e_ _s_t_a_t_e_ _a_n_d
-   _i_s_ _b_e_i_n_g_ _a_c_t_i_v_e_l_y_ _d_e_v_e_l_o_p_e_d_._]_[_L_a_t_e_s_t_ _V_e_r_s_i_o_n_]_[_O_p_e_n_ _I_s_s_u_e_s_]_[_C_l_o_s_e_d_ _I_s_s_u_e_s_]
-                    _[_L_i_c_e_n_s_e_]_[_C_o_d_e_ _s_t_y_l_e_:_ _b_l_a_c_k_]_[_C_o_d_e_ _S_i_z_e_]
+  _i_s_ _b_e_i_n_g_ _a_c_t_i_v_e_l_y_ _d_e_v_e_l_o_p_e_d_._]_[_L_a_t_e_s_t_ _V_e_r_s_i_o_n_]_[_P_y_P_i_ _D_o_w_n_l_o_a_d_s_]_[_O_p_e_n_ _I_s_s_u_e_s_]
+            _[_C_l_o_s_e_d_ _I_s_s_u_e_s_]_[_L_i_c_e_n_s_e_]_[_C_o_d_e_ _s_t_y_l_e_:_ _b_l_a_c_k_]_[_C_o_d_e_ _S_i_z_e_]
     _A_b_o_u_t â¢ _F_e_a_t_u_r_e_s â¢ _H_o_w_ _T_o_ _U_s_e â¢ _E_x_a_m_p_l_e_s â¢ _F_A_Q â¢ _C_o_n_t_a_c_t â¢
                           _A_c_k_n_o_w_l_e_d_g_m_e_n_t_s â¢ _L_i_c_e_n_s_e
 ## About The reason for the existence of this software is Youtube's seemingly
 random behavior when it comes to notifying people that a new video has been
 published (late or missing notifications, useless notification bell, videos not
 appearing in the subscription tab, ...). With this software, you can set a
 number of rules that determine which videos are added to a dedicated playlist,
@@ -17,31 +17,35 @@
 features are available: * Channel name filtering * Title filtering *
 Description filtering * Tags filtering * Language filtering * Caption filtering
 * Duration filtering * Quality filtering * Upload date filtering * Shorts
 filtering * Duplicate checking ## How to use Before using this software, you
 first need to get a Youtube API key and create a web app to get a client
 secrets file (that should look like [this](docs/client_secrets_template.json)).
 This [Corey Schafer video](https://www.youtube.com/watch?v=vQQEaSnQ_bs) goes
-through the process step by step. Once that's done, either clone this
-repository or download the ZIP archive. Then, copy and rename the [user
-parameters template](docs/user_params_template.json) file to
-*user_params.json*. Modify it so that it fits your needs (more information on
-how in the [following table](#user-defined-parameters) and in the [examples
-section](#examples)). Verify that you have all of the dependencies installed
-(see the [requirements](requirements.txt) file). Finally, execute the [run.py]
-(QTube/run.py) file to start the software. I would recommend creating a task to
-execute the program regularly (like once a day). For more versatile uses, you
-can also use command line arguments with the [run.py](QTube/run.py) file.
-Enable this option by setting the parameter `override_json` to *True* in your
-JSON user parameters file. Provided command line arguments will then override
-what is in your JSON user parameters file. ### User-defined parameters
-|Parameter|Optional|Description|Possible values| |--|:--:|:--:|:--:
-| |`required_in_channel_name`|Yes|Words that must be in channel names,
-typically channel names themselves. Videos from channels not containing any of
-the words of this list in their name will not be added.|Any string|
+through the process step by step. Once that's done, download this project or
+install the package with [PyPI](https://pypi.org/project/QTube/). Then, copy
+the [user parameters template](docs/user_params_template.json) file to the main
+QTube directory and rename it to *user_params.json*. Modify it so that it fits
+your needs (more information on how in the [following table](#user-defined-
+parameters) and in the [examples section](#examples)). Verify that you have all
+of the dependencies installed (see the [requirements](requirements.txt) file or
+the [TOML](pyproject.toml) file). Finally, execute the [qtube.py](QTube/
+scripts/qtube.py) file to start the software, either by running the file
+directly or by using the CLI ***qtube*** in the main directory. I would
+recommend creating a task to execute the program regularly (like once a day).
+For more versatile uses, you can also use command line arguments with the
+[qtube.py](QTube/scripts/qtube.py) file. Enable this option by setting the
+parameter `override_json` to *True* in your JSON user parameters file. Provided
+command line arguments will then override what is in your JSON user parameters
+file. This is especially useful to manage different types of videos and put
+them in dedicated playlists (music playlist, gaming playlist, ect...). ###
+User-defined parameters |Parameter|Optional|Description|Possible values| |--|:-
+-:|:--:|:--:| |`required_in_channel_name`|Yes|Words that must be in channel
+names, typically channel names themselves. Videos from channels not containing
+any of the words of this list in their name will not be added.|Any string|
 |`banned_in_channel_name`|Yes|Words that must not be in channel names,
 typically channel names themselves. Videos from channels containing any of the
 words of this list in their name will not be added.|Any string|
 |`include_extra_channels`|No|Determines whether to include channels the user is
 not subscribed to.|boolean| |`extra_channel_handles`|Yes|Handles of additional
 channels to be checked. Handles are found at the end of a channel's URL:
 `https://www.youtube.com/@*handle*`|Any channel handle|
@@ -99,44 +103,44 @@
 *none* 2 ,
 *func* 3 ,
 *credentials* 4 ,
 *videos* 5 .| All parameters are case-sensitive by default and if you do not
 want to use an optional parameter, replace its value with *null* or delete the
 entry. For further information about each parameter, check the note associated
 with the [release](https://github.com/Killian42/QTube/releases) they were
-introduced in. ### Requirements See the [requirements](requirements.txt) file.
-## Examples This section presents examples of user parameters json files for
-concrete use-cases. * _E_v_e_r_y_ _v_i_d_e_o_s_ _f_r_o_m_ _s_u_b_s_c_r_i_b_e_d_ _c_h_a_n_n_e_l_s * _H_i_g_h_e_r_ _q_u_a_l_i_t_y
-_v_i_d_e_o_s * _V_i_d_e_o_ _s_e_r_i_e_s_ _f_r_o_m_ _a_ _c_r_e_a_t_o_r ### Example 1 - Every videos from
-subscribed channels The following *user_params.json* file would add every new
-videos from channels you are subcribed to. ``` { "required_in_channel_name":
-null, "banned_in_channel_name": null, "include_extra_channels": false,
-"extra_channel_handles": null, "required_in_title": null, "banned_in_title":
-null, "ignore_title_emojis": false, "ignore_title_punctuation": false,
-"ignore_title_case": false, "required_in_description": null,
-"banned_in_description": null, "required_tags": null, "banned_tags": null,
-"preferred_languages": null, "require_captions":false, "caption_options": null,
-"allowed_durations": null, "lowest_definition": null, "lowest_resolution":
-null, "lowest_framerate": null, "preferred_dimensions": null,
-"preferred_projections": null, "run_frequency":"daily", "keep_shorts": true,
-"keep_duplicates": false, "upload_playlist_ID": "your_playlist_ID",
-"override_json":false, "verbosity": ["credentials","videos"] } ``` ### Example
-2 - Higher quality videos The following *user_params.json* file would only add
-videos with good quality. ``` { "required_in_channel_name": null,
-"banned_in_channel_name": null, "include_extra_channels": false,
-"extra_channel_handles": null, "required_in_title": null, "banned_in_title":
-null, "ignore_title_emojis": false, "ignore_title_punctuation": false,
-"ignore_title_case": false, "required_in_description": null,
-"banned_in_description": null, "required_tags": null, "banned_tags": null,
-"preferred_languages": null, "require_captions":false, "caption_options": null,
-"allowed_durations": null, "lowest_definition": "HD", "lowest_resolution":
-"1080p", "lowest_framerate": 60, "preferred_dimensions": ["2D"],
-"preferred_projections": ["rectangular"], "run_frequency":"daily",
-"keep_shorts": true, "keep_duplicates": false, "upload_playlist_ID":
+introduced in. ### Requirements See the [requirements](requirements.txt) file
+or the [TOML](pyproject.toml) file. ## Examples This section presents examples
+of user parameters json files for concrete use-cases. * _E_v_e_r_y_ _v_i_d_e_o_s_ _f_r_o_m
+_s_u_b_s_c_r_i_b_e_d_ _c_h_a_n_n_e_l_s * _H_i_g_h_e_r_ _q_u_a_l_i_t_y_ _v_i_d_e_o_s * _V_i_d_e_o_ _s_e_r_i_e_s_ _f_r_o_m_ _a_ _c_r_e_a_t_o_r ###
+Example 1 - Every videos from subscribed channels The following
+*user_params.json* file would add every new videos from channels you are
+subcribed to. ``` { "required_in_channel_name": null, "banned_in_channel_name":
+null, "include_extra_channels": false, "extra_channel_handles": null,
+"required_in_title": null, "banned_in_title": null, "ignore_title_emojis":
+false, "ignore_title_punctuation": false, "ignore_title_case": false,
+"required_in_description": null, "banned_in_description": null,
+"required_tags": null, "banned_tags": null, "preferred_languages": null,
+"require_captions":false, "caption_options": null, "allowed_durations": null,
+"lowest_definition": null, "lowest_resolution": null, "lowest_framerate": null,
+"preferred_dimensions": null, "preferred_projections": null, "run_frequency":
+"daily", "keep_shorts": true, "keep_duplicates": false, "upload_playlist_ID":
 "your_playlist_ID", "override_json":false, "verbosity":
+["credentials","videos"] } ``` ### Example 2 - Higher quality videos The
+following *user_params.json* file would only add videos with good quality. ```
+{ "required_in_channel_name": null, "banned_in_channel_name": null,
+"include_extra_channels": false, "extra_channel_handles": null,
+"required_in_title": null, "banned_in_title": null, "ignore_title_emojis":
+false, "ignore_title_punctuation": false, "ignore_title_case": false,
+"required_in_description": null, "banned_in_description": null,
+"required_tags": null, "banned_tags": null, "preferred_languages": null,
+"require_captions":false, "caption_options": null, "allowed_durations": null,
+"lowest_definition": "HD", "lowest_resolution": "1080p", "lowest_framerate":
+60, "preferred_dimensions": ["2D"], "preferred_projections": ["rectangular"],
+"run_frequency":"daily", "keep_shorts": true, "keep_duplicates": false,
+"upload_playlist_ID": "your_playlist_ID", "override_json":false, "verbosity":
 ["credentials","videos"] } ``` ### Example 3 - Specific video series from a
 creator The following *user_params.json* file would only add the *$1 vs.*
 MrBeast videos. ``` { "required_in_channel_name": ["MrBeast"],
 "banned_in_channel_name": null, "include_extra_channels": false,
 "extra_channel_handles": null, "required_in_title": ["$1 vs."],
 "banned_in_title": null, "ignore_title_emojis": true,
 "ignore_title_punctuation": false, "ignore_title_case": true,
```

### Comparing `QTube-2.0.0/pyproject.toml` & `qtube-2.0.0a0/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 
 [project]
 name = "QTube"
-version = "2.0.0"
+version = "2.0.0-alpha"
 requires-python = ">=3.8"
 authors = [
     { name = "Killian Lebreton", email = "killian.lebreton35@gmail.com" },
 ]
 maintainers = [
     { name = "Killian Lebreton", email = "killian.lebreton35@gmail.com" },
 ]
```

### Comparing `QTube-2.0.0/setup.py` & `qtube-2.0.0a0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup
 
 with open("README.md", "r") as f:
     long_description = f.read()
 
 setup(
     name="QTube",
-    version="2.0.0",
+    version="2.0.0-alpha",
     description="Automatically add Youtube videos to a playlist.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     license="MIT",
     author="Killian Lebreton",
     author_email="killian.lebreton35@gmail.com",
     url="https://github.com/Killian42/QTube",
```

