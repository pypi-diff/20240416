# Comparing `tmp/git-sim-0.3.3.tar.gz` & `tmp/git_sim-0.3.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "git-sim-0.3.3.tar", last modified: Wed Jul  5 01:52:36 2023, max compression
+gzip compressed data, was "git_sim-0.3.4.tar", last modified: Tue Apr 16 17:25:10 2024, max compression
```

## Comparing `git-sim-0.3.3.tar` & `git_sim-0.3.4.tar`

### file list

```diff
@@ -1,45 +1,48 @@
-drwxrwxrwx   0        0        0        0 2023-07-05 01:52:36.529848 git-sim-0.3.3/
--rw-rw-rw-   0        0        0    18431 2023-03-09 07:57:29.000000 git-sim-0.3.3/LICENSE
--rw-rw-rw-   0        0        0       26 2023-03-09 07:57:17.000000 git-sim-0.3.3/MANIFEST.in
--rw-rw-rw-   0        0        0    25490 2023-07-05 01:52:36.528497 git-sim-0.3.3/PKG-INFO
--rw-rw-rw-   0        0        0    24683 2023-06-12 02:56:27.000000 git-sim-0.3.3/README.md
-drwxrwxrwx   0        0        0        0 2023-07-05 01:52:36.520305 git-sim-0.3.3/git_sim/
--rw-rw-rw-   0        0        0       23 2023-07-05 01:51:56.000000 git-sim-0.3.3/git_sim/__init__.py
--rw-rw-rw-   0        0        0     8333 2023-04-21 20:23:21.000000 git-sim-0.3.3/git_sim/__main__.py
--rw-rw-rw-   0        0        0     2852 2023-04-21 20:10:26.000000 git-sim-0.3.3/git_sim/add.py
--rw-rw-rw-   0        0        0     3680 2023-04-21 20:23:21.000000 git-sim-0.3.3/git_sim/animations.py
--rw-rw-rw-   0        0        0     1511 2023-04-21 20:10:26.000000 git-sim-0.3.3/git_sim/branch.py
--rw-rw-rw-   0        0        0     4415 2023-04-21 20:10:26.000000 git-sim-0.3.3/git_sim/checkout.py
--rw-rw-rw-   0        0        0     2302 2023-04-21 20:10:26.000000 git-sim-0.3.3/git_sim/cherrypick.py
--rw-rw-rw-   0        0        0     3921 2023-04-21 20:23:21.000000 git-sim-0.3.3/git_sim/clean.py
--rw-rw-rw-   0        0        0     2974 2023-04-21 20:10:26.000000 git-sim-0.3.3/git_sim/clone.py
--rw-rw-rw-   0        0        0     8586 2023-04-21 20:23:21.000000 git-sim-0.3.3/git_sim/commands.py
--rw-rw-rw-   0        0        0     3175 2023-04-21 20:10:26.000000 git-sim-0.3.3/git_sim/commit.py
--rw-rw-rw-   0        0        0      572 2023-04-21 21:10:02.000000 git-sim-0.3.3/git_sim/enums.py
--rw-rw-rw-   0        0        0     2842 2023-04-21 20:10:26.000000 git-sim-0.3.3/git_sim/fetch.py
--rw-rw-rw-   0        0        0    46330 2023-06-12 02:56:27.000000 git-sim-0.3.3/git_sim/git_sim_base_command.py
--rw-rw-rw-   0        0        0     1415 2023-06-06 18:37:54.000000 git-sim-0.3.3/git_sim/log.py
--rw-rw-rw-   0        0        0    63319 2023-03-09 07:57:17.000000 git-sim-0.3.3/git_sim/logo.png
--rw-rw-rw-   0        0        0     7258 2023-06-12 02:56:27.000000 git-sim-0.3.3/git_sim/merge.py
--rw-rw-rw-   0        0        0     2937 2023-04-21 20:23:21.000000 git-sim-0.3.3/git_sim/mv.py
--rw-rw-rw-   0        0        0     3844 2023-04-21 20:10:26.000000 git-sim-0.3.3/git_sim/pull.py
--rw-rw-rw-   0        0        0     7226 2023-04-21 21:10:02.000000 git-sim-0.3.3/git_sim/push.py
--rw-rw-rw-   0        0        0     6057 2023-04-21 20:23:21.000000 git-sim-0.3.3/git_sim/rebase.py
--rw-rw-rw-   0        0        0     5042 2023-04-21 20:10:26.000000 git-sim-0.3.3/git_sim/reset.py
--rw-rw-rw-   0        0        0     2467 2023-04-21 20:10:26.000000 git-sim-0.3.3/git_sim/restore.py
--rw-rw-rw-   0        0        0     5607 2023-04-21 20:23:21.000000 git-sim-0.3.3/git_sim/revert.py
--rw-rw-rw-   0        0        0     4541 2023-04-21 20:23:21.000000 git-sim-0.3.3/git_sim/rm.py
--rw-rw-rw-   0        0        0     1566 2023-07-05 01:51:10.000000 git-sim-0.3.3/git_sim/settings.py
--rw-rw-rw-   0        0        0     6505 2023-04-21 20:10:26.000000 git-sim-0.3.3/git_sim/stash.py
--rw-rw-rw-   0        0        0      829 2023-04-21 20:10:26.000000 git-sim-0.3.3/git_sim/status.py
--rw-rw-rw-   0        0        0     4413 2023-04-21 20:10:26.000000 git-sim-0.3.3/git_sim/switch.py
--rw-rw-rw-   0        0        0     1469 2023-04-21 20:10:26.000000 git-sim-0.3.3/git_sim/tag.py
-drwxrwxrwx   0        0        0        0 2023-07-05 01:52:36.528497 git-sim-0.3.3/git_sim.egg-info/
--rw-rw-rw-   0        0        0    25490 2023-07-05 01:52:36.000000 git-sim-0.3.3/git_sim.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      770 2023-07-05 01:52:36.000000 git-sim-0.3.3/git_sim.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-05 01:52:36.000000 git-sim-0.3.3/git_sim.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       84 2023-07-05 01:52:36.000000 git-sim-0.3.3/git_sim.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       73 2023-07-05 01:52:36.000000 git-sim-0.3.3/git_sim.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2023-07-05 01:52:36.000000 git-sim-0.3.3/git_sim.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-07-05 01:52:36.529848 git-sim-0.3.3/setup.cfg
--rw-rw-rw-   0        0        0     1477 2023-07-05 01:48:30.000000 git-sim-0.3.3/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-16 17:25:10.799986 git_sim-0.3.4/
+-rw-rw-rw-   0        0        0    18431 2024-04-09 04:56:41.000000 git_sim-0.3.4/LICENSE
+-rw-rw-rw-   0        0        0       26 2023-03-09 07:57:17.000000 git_sim-0.3.4/MANIFEST.in
+-rw-rw-rw-   0        0        0    27375 2024-04-16 17:25:10.798982 git_sim-0.3.4/PKG-INFO
+-rw-rw-rw-   0        0        0    26213 2024-04-16 17:03:29.000000 git_sim-0.3.4/README.md
+-rw-rw-rw-   0        0        0     1366 2024-03-21 02:51:06.000000 git_sim-0.3.4/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-04-16 17:25:10.799986 git_sim-0.3.4/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-04-16 17:25:10.765385 git_sim-0.3.4/src/
+drwxrwxrwx   0        0        0        0 2024-04-16 17:25:10.784572 git_sim-0.3.4/src/git_sim/
+-rw-rw-rw-   0        0        0       23 2024-04-16 17:06:39.000000 git_sim-0.3.4/src/git_sim/__init__.py
+-rw-rw-rw-   0        0        0     9438 2024-04-16 17:03:29.000000 git_sim-0.3.4/src/git_sim/__main__.py
+-rw-rw-rw-   0        0        0     2895 2024-04-16 17:03:29.000000 git_sim-0.3.4/src/git_sim/add.py
+-rw-rw-rw-   0        0        0     3680 2023-12-24 03:27:50.000000 git_sim-0.3.4/src/git_sim/animations.py
+-rw-rw-rw-   0        0        0     1582 2024-04-16 17:03:29.000000 git_sim-0.3.4/src/git_sim/branch.py
+-rw-rw-rw-   0        0        0     4483 2024-04-16 17:03:29.000000 git_sim-0.3.4/src/git_sim/checkout.py
+-rw-rw-rw-   0        0        0     2352 2024-04-16 17:03:29.000000 git_sim-0.3.4/src/git_sim/cherrypick.py
+-rw-rw-rw-   0        0        0     3990 2024-04-16 17:03:29.000000 git_sim-0.3.4/src/git_sim/clean.py
+-rw-rw-rw-   0        0        0     3458 2024-04-16 17:03:29.000000 git_sim-0.3.4/src/git_sim/clone.py
+-rw-rw-rw-   0        0        0    10740 2024-04-16 17:03:29.000000 git_sim-0.3.4/src/git_sim/commands.py
+-rw-rw-rw-   0        0        0     3683 2024-04-16 17:03:29.000000 git_sim-0.3.4/src/git_sim/commit.py
+-rw-rw-rw-   0        0        0    10056 2024-04-16 17:03:29.000000 git_sim-0.3.4/src/git_sim/config.py
+-rw-rw-rw-   0        0        0      720 2024-04-16 17:03:29.000000 git_sim-0.3.4/src/git_sim/enums.py
+-rw-rw-rw-   0        0        0     2884 2024-04-16 17:03:29.000000 git_sim-0.3.4/src/git_sim/fetch.py
+-rw-rw-rw-   0        0        0    49049 2024-04-16 17:03:29.000000 git_sim-0.3.4/src/git_sim/git_sim_base_command.py
+-rw-rw-rw-   0        0        0    11319 2024-04-16 17:03:29.000000 git_sim-0.3.4/src/git_sim/init.py
+-rw-rw-rw-   0        0        0     1458 2024-04-16 17:03:29.000000 git_sim-0.3.4/src/git_sim/log.py
+-rw-rw-rw-   0        0        0     7300 2024-04-16 17:03:29.000000 git_sim-0.3.4/src/git_sim/merge.py
+-rw-rw-rw-   0        0        0     2978 2024-04-16 17:03:29.000000 git_sim-0.3.4/src/git_sim/mv.py
+-rw-rw-rw-   0        0        0     3886 2024-04-16 17:03:29.000000 git_sim-0.3.4/src/git_sim/pull.py
+-rw-rw-rw-   0        0        0     7386 2024-04-16 17:03:29.000000 git_sim-0.3.4/src/git_sim/push.py
+-rw-rw-rw-   0        0        0     6095 2024-04-16 17:03:29.000000 git_sim-0.3.4/src/git_sim/rebase.py
+-rw-rw-rw-   0        0        0    15809 2024-04-16 17:03:29.000000 git_sim-0.3.4/src/git_sim/remote.py
+-rw-rw-rw-   0        0        0     5043 2024-04-16 17:03:29.000000 git_sim-0.3.4/src/git_sim/reset.py
+-rw-rw-rw-   0        0        0     2848 2024-04-16 17:03:29.000000 git_sim-0.3.4/src/git_sim/restore.py
+-rw-rw-rw-   0        0        0     5605 2024-04-16 17:03:29.000000 git_sim-0.3.4/src/git_sim/revert.py
+-rw-rw-rw-   0        0        0     4578 2024-04-16 17:03:29.000000 git_sim-0.3.4/src/git_sim/rm.py
+-rw-rw-rw-   0        0        0     1663 2024-04-16 17:03:29.000000 git_sim-0.3.4/src/git_sim/settings.py
+-rw-rw-rw-   0        0        0     7571 2024-04-16 17:03:29.000000 git_sim-0.3.4/src/git_sim/stash.py
+-rw-rw-rw-   0        0        0      901 2024-04-16 17:03:29.000000 git_sim-0.3.4/src/git_sim/status.py
+-rw-rw-rw-   0        0        0     5383 2024-04-16 17:03:29.000000 git_sim-0.3.4/src/git_sim/switch.py
+-rw-rw-rw-   0        0        0     3568 2024-04-16 17:03:29.000000 git_sim-0.3.4/src/git_sim/tag.py
+drwxrwxrwx   0        0        0        0 2024-04-16 17:25:10.798982 git_sim-0.3.4/src/git_sim.egg-info/
+-rw-rw-rw-   0        0        0    27375 2024-04-16 17:25:10.000000 git_sim-0.3.4/src/git_sim.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      963 2024-04-16 17:25:10.000000 git_sim-0.3.4/src/git_sim.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-16 17:25:10.000000 git_sim-0.3.4/src/git_sim.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       49 2024-04-16 17:25:10.000000 git_sim-0.3.4/src/git_sim.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0      116 2024-04-16 17:25:10.000000 git_sim-0.3.4/src/git_sim.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2024-04-16 17:25:10.000000 git_sim-0.3.4/src/git_sim.egg-info/top_level.txt
```

### Comparing `git-sim-0.3.3/LICENSE` & `git_sim-0.3.4/LICENSE`

 * *Files identical despite different names*

### Comparing `git-sim-0.3.3/PKG-INFO` & `git_sim-0.3.4/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,23 +1,34 @@
 Metadata-Version: 2.1
 Name: git-sim
-Version: 0.3.3
+Version: 0.3.4
 Summary: Simulate Git commands on your own repos by generating an image (default) or video visualization depicting the command's behavior.
-Home-page: https://initialcommit.com/tools/git-sim
-Author: Jacob Stopak
-Author-email: jacob@initialcommit.io
+Author-email: Jacob Stopak <jacob@initialcommit.io>
+License: GPL-2.0
 Project-URL: Homepage, https://initialcommit.com/tools/git-sim
 Project-URL: Source, https://github.com/initialcommit-com/git-sim
-Keywords: git sim simulation simulate git-simulate git-simulation git-sim manim animation gitanimation image video dryrun dry-run
+Keywords: git,sim,simulation,simulate,git-simulate,git-simulation,git-sim,manim,animation,gitanimation,image,video,dryrun,dry-run
 Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License
+Classifier: License :: OSI Approved :: GNU General Public License v2 (GPLv2)
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: git-dummy
+Requires-Dist: gitpython
+Requires-Dist: manim
+Requires-Dist: opencv-python-headless
+Requires-Dist: pydantic_settings
+Requires-Dist: typer
+Requires-Dist: fonttools
+Provides-Extra: dev
+Requires-Dist: black; extra == "dev"
+Requires-Dist: numpy; extra == "dev"
+Requires-Dist: pillow; extra == "dev"
+Requires-Dist: pytest; extra == "dev"
 
 # git-sim
 ![git-sim-logo-with-tagline-1440x376p45](https://user-images.githubusercontent.com/49353917/232990611-58d0693f-69c0-45c8-b51d-cd540793d18c.gif)
 
 [![GitHub license](https://img.shields.io/github/license/initialcommit-com/git-sim)](https://github.com/initialcommit-com/git-sim/blob/main/LICENSE)
 [![GitHub tag](https://img.shields.io/github/v/release/initialcommit-com/git-sim)](https://img.shields.io/github/v/release/initialcommit-com/git-sim)
 [![Downloads](https://static.pepy.tech/badge/git-sim)](https://pepy.tech/project/git-sim)
@@ -30,26 +41,33 @@
 
 Command syntax is based directly on Git's command-line syntax, so using git-sim is as familiar as possible.
 
 Example: `$ git-sim merge <branch>`
 <br/><br/>
 ![git-sim-merge_04-22-23_21-04-32_cropped](https://user-images.githubusercontent.com/49353917/233821875-a7bb640d-10be-4433-a8fb-bd25646eeff4.jpg)
 
+Check out the [git-sim release blog post](https://initialcommit.com/blog/git-sim) for the full scoop!
+
+## Support git-sim
+Git-Sim is Free and Open-Source Software (FOSS). Your support will help me work on it (and other Git projects) full time!
+- [Sponsor Git-Sim on GitHub](https://github.com/sponsors/initialcommit-com)
+- [Support Git-Sim via Patreon](https://patreon.com/user?u=92322459)
+
 ## Use cases
 - Visualize Git commands to understand their effects on your repo before actually running them
 - Prevent unexpected working directory and repository states by simulating before running
 - Share visualizations (jpg/png image or mp4/webm video) of your Git commands with your team, or the world
 - Save visualizations as a part of your team documentation to document workflow and prevent recurring issues
 - Create static Git diagrams (jpg/png) or dynamic animated videos (mp4/webm) to speed up content creation
 - Help visual learners understand how Git commands work
 - Combine with bundled command [git-dummy](https://github.com/initialcommit-com/git-dummy) to generate a dummy Git repo and then simulate operations on it
 
 ## Features
 - Run a one-liner git-sim command in the terminal to generate a custom Git command visualization (.jpg) from your repo
-- Supported commands: `log`, `status`, `add`, `restore`, `commit`, `stash`, `branch`, `tag`, `reset`, `revert`, `merge`, `rebase`, `cherry-pick`, `switch`, `checkout`, `fetch`, `pull`, `push`, `clone`, `rm`, `mv`, `clean`
+- Supported commands: `add`, `branch`, `checkout`, `cherry-pick`, `clean`, `clone`, `commit`, `config`, `fetch`, `init`, `log`, `merge`, `mv`, `pull`, `push`, `rebase`, `remote`, `reset`, `restore`, `revert`, `rm`, `stash`, `status`, `switch`, `tag`
 - Generate an animated video (.mp4) instead of a static image using the `--animate` flag (note: significant performance slowdown, it is recommended to use `--low-quality` to speed up testing and remove when ready to generate presentation-quality video)
 - Color commits by parameter, such as author with the `--color-by=author` option
 - Choose between dark mode (default) and light mode
 - Specify output formats of either jpg, png, mp4, or webm
 - Combine with bundled command [git-dummy](https://github.com/initialcommit-com/git-dummy) to generate a dummy Git repo and then simulate operations on it
 - Animation only: Add custom branded intro/outro sequences if desired
 - Animation only: Speed up or slow down animation speed as desired
@@ -141,15 +159,16 @@
 
 ## Requirements
 * Python 3.7 or greater
 * Pip (Package manager for Python)
 * [Manim (Community version)](https://www.manim.community/)
 
 ## Commands
-Basic usage is similar to Git itself - `git-sim` takes a familiar set of subcommands including "log", "status", "add", "restore", "commit", "stash", "branch", "tag", "reset", "revert", "merge", "rebase", "cherry-pick", "switch", "checkout", "fetch", "pull", "push", "clone", "rm", "mv", "clean" along with corresponding options.
+Basic usage is similar to Git itself - `git-sim` takes a familiar set of subcommands including "add", "branch", "checkout", "cherry-pick", "clean", "clone", "commit", "config", "fetch", "init", "log", "merge", "mv", "pull", "push", "rebase", "remote", "reset", "restore", "revert", "rm", "stash", "status", "switch", "tag" along with corresponding options.
+
 
 ```console
 $ git-sim [global options] <subcommand> [subcommand options]
 ```
 
 The `[global options]` apply to the overarching `git-sim` simulation itself, including:
 
@@ -176,159 +195,134 @@
 `--speed=n`: Set the multiple of animation speed of the output simulation, `n` can be an integer or float, default is 1.5.  
 `--low-quality`: Render the animation in low quality to speed up creation time, recommended for non-presentation use.  
 `--show-intro`: Add an intro sequence with custom logo and title.  
 `--show-outro`: Add an outro sequence with custom logo and text.  
 `--title=title`: Custom title to display at the beginning of the animation.  
 `--logo=logo.png`: The path to a custom logo to use in the animation intro/outro.  
 `--outro-top-text`: Custom text to display above the logo during the outro.  
-`--outro-bottom-text`: Custom text to display below the logo during the outro.
+`--outro-bottom-text`: Custom text to display below the logo during the outro.  
+`--font`: Font family used to display rendered text.
 
 The `[subcommand options]` are like regular Git options specific to the specified subcommand (see below for a full list).
 
 The following is a list of Git commands that can be simulated and their corresponding options/flags.
 
-### git log
-Usage: `git-sim log [-n <number>] [--all]`
-
-- Simulated output will show the most recent 5 commits on the active branch by default
-- Use `-n <number>` to set number of commits to display from each branch head
-- Set `--all` to display all local branches in the log output
-
-![git-sim-log_01-05-23_22-02-39](https://user-images.githubusercontent.com/49353917/210940300-aadd14c6-72ab-4529-a1be-b494ed5dd4c9.jpg)
-
-### git status
-Usage: `git-sim status`
-
-- Simulated output will show the state of the working directory, staging area, and untracked files
-- Note that simulated output will also show the most recent 5 commits on the active branch
-
-![git-sim-status_01-05-23_22-06-28](https://user-images.githubusercontent.com/49353917/210940685-735665e2-fa12-4043-979c-54c295b13800.jpg)
-
 ### git add
 Usage: `git-sim add <file 1> <file 2> ... <file n>`
 
 - Specify one or more `<file>` as a *modified* working directory file, or an untracked file
 - Simulated output will show files being moved to the staging area
 - Note that simulated output will also show the most recent 5 commits on the active branch
 
 ![git-sim-add_01-05-23_22-07-40](https://user-images.githubusercontent.com/49353917/210940814-7e8dc318-6116-4e56-b415-bc547401a56a.jpg)
 
-### git restore
-Usage: `git-sim restore <file 1> <file 2> ... <file n>`
+### git branch
+Usage: `git-sim branch <new branch name>`
 
-- Specify one or more `<file>` as a *modified* working directory file, or staged file
-- Simulated output will show files being moved back to the working directory or discarded changes
+- Specify `<new branch name>` as the name of the new branch to simulate creation of
+- Simulated output will show the newly create branch ref along with most recent 5 commits on the active branch
+
+![git-sim-branch_01-05-23_22-13-17](https://user-images.githubusercontent.com/49353917/210941509-2a42a7a4-2168-4f62-913f-3f6fe74a0684.jpg)
+
+### git checkout
+Usage: `git-sim checkout [-b] <branch>`
+
+- Checks out `<branch>` into the working directory, i.e. moves `HEAD` to the specified `<branch>`
+- The `-b` flag creates a new branch with the specified name `<branch>` and checks it out, assuming it doesn't already exist
+
+![git-sim-checkout_04-09-23_21-46-04](https://user-images.githubusercontent.com/49353917/230827836-e9f23a0e-2576-4716-b2fb-6327d3cf9b22.jpg)
+
+### git cherry-pick
+Usage: `git-sim cherry-pick <commit>`
+
+- Specify `<commit>` as a ref (branch name/tag) or commit ID to cherry-pick onto the active branch
+- Supports editing the cherry-picked commit message with: `$ git-sim cherry-pick <commit> -e "Edited commit message"`
+
+![git-sim-cherry-pick_01-05-23_22-23-08](https://user-images.githubusercontent.com/49353917/210942811-fa5155b1-4c6f-4afc-bea2-d39b4cd594aa.jpg)
+
+### git clean
+Usage: `git-sim clean`
+
+- Simulated output will show untracked files being deleted
+- Since this is just a simulation, no need to specify `-i`, `-n`, `-f` as in regular Git
 - Note that simulated output will also show the most recent 5 commits on the active branch
 
-![git-sim-restore_01-05-23_22-09-14](https://user-images.githubusercontent.com/49353917/210941009-e6bf7271-ce9b-4e41-9a0b-24cc4b8d3b15.jpg)
+![git-sim-clean_04-09-23_22-05-54](https://user-images.githubusercontent.com/49353917/230830043-779e7230-f439-461a-a408-b19b263e86e4.jpg)
+
+### git clone
+Usage: `git-sim clone <url>`
+
+- Clone the remote repo from `<url>` (web URL or filesystem path) to a new folder in the current directory
+- Output will report if clone operation is successful and show log of local clone
+
+![git-sim-clone_04-09-23_21-51-53](https://user-images.githubusercontent.com/49353917/230828521-80c8d2d1-2a31-46bb-aeed-746f0441c86e.jpg)
 
 ### git commit
 Usage: `git-sim commit -m "Commit message"`
 
 - Simulated output will show the new commit added to the tip of the active branch
 - Specify a commit message with the `-m` option
 - HEAD and the active branch will be moved to the new commit
 - Simulated output will show files in the staging area being included in the new commit
 - Supports amending the last commit with: `$ git-sim commit --amend -m "Amended commit message"`
 
 ![git-sim-commit_01-05-23_22-10-21](https://user-images.githubusercontent.com/49353917/210941149-d83677a1-3ab7-4880-bc0f-871b1f150087.jpg)
 
-### git stash
-Usage: `git-sim stash [push|pop|apply] <file>`
-
-- Specify one or more `<file>` as a *modified* working directory file, or staged file
-- If no `<file>` is specified, all available files will be included
-- Simulated output will show files being moved in/out of the Git stash
-- Note that simulated output will also show the most recent 5 commits on the active branch
-
-![git-sim-stash_01-05-23_22-11-18](https://user-images.githubusercontent.com/49353917/210941254-69c80b63-5c06-411a-a36a-1454b2906ee8.jpg)
+### git config
+Usage: `git-sim config [--list] <section.option> <value>`
 
-### git branch
-Usage: `git-sim branch <new branch name>`
+- Simulated output describes the specified configuration change
+- Use `--list` or `-l` to display all configuration
 
-- Specify `<new branch name>` as the name of the new branch to simulate creation of
-- Simulated output will show the newly create branch ref along with most recent 5 commits on the active branch
-
-![git-sim-branch_01-05-23_22-13-17](https://user-images.githubusercontent.com/49353917/210941509-2a42a7a4-2168-4f62-913f-3f6fe74a0684.jpg)
+![git-sim-config_04-16-24_08-34-34](https://github.com/initialcommit-com/git-sim/assets/49353917/c123e7a7-1fff-4f5c-b4a2-1e34ea2a4d80)
 
-### git tag
-Usage: `git-sim tag <new tag name>`
+### git fetch
+Usage: `git-sim fetch <remote> <branch>`
 
-- Specify `<new tag name>` as the name of the new tag to simulate creation of
-- Simulated output will show the newly create tag ref along with most recent 5 commits on the active branch
+- Fetches the specified `<branch>` from the specified `<remote>` to the local repo
 
-![git-sim-tag_01-05-23_22-14-18](https://user-images.githubusercontent.com/49353917/210941647-79376ff7-2941-42b3-964a-b1d3a404a4fe.jpg)
+![git-sim-fetch_04-09-23_21-47-59](https://user-images.githubusercontent.com/49353917/230828090-acae8979-4097-43a8-96ea-525890e0e0a8.jpg)
 
-### git reset
-Usage: `git-sim reset <reset-to> [--mixed|--soft|--hard]`
+### git init
+Usage: `git-sim init`
 
-- Specify `<reset-to>` as any commit id, branch name, tag, or other ref to simulate reset to from the current HEAD (default: `HEAD`)
-- As with a normal git reset command, default reset mode is `--mixed`, but can be specified using `--soft`, `--hard`, or `--mixed`
-- Simulated output will show branch/HEAD resets and resulting state of the working directory, staging area, and whether any file changes would be deleted by running the actual command
+- Simulated output describes the initialized `.git/` directory and it's contents
 
-![git-sim-reset_01-05-23_22-15-49](https://user-images.githubusercontent.com/49353917/210941835-80f032d2-4f06-4032-8dd0-98c8a2569049.jpg)
+![git-sim-init_04-16-24_08-34-47](https://github.com/initialcommit-com/git-sim/assets/49353917/2abb1a4a-3022-4353-a828-2d337baa8383)
 
-### git revert
-Usage: `git-sim revert <to-revert>`
+### git log
+Usage: `git-sim log [-n <number>] [--all]`
 
-- Specify `<to-revert>` as any commit id, branch name, tag, or other ref to simulate revert for
-- Simulated output will show the new commit which reverts the changes from `<to-revert>`
-- Simulated output will include the next 4 most recent commits on the active branch
+- Simulated output will show the most recent 5 commits on the active branch by default
+- Use `-n <number>` to set number of commits to display from each branch head
+- Set `--all` to display all local branches in the log output
 
-![git-sim-revert_01-05-23_22-16-59](https://user-images.githubusercontent.com/49353917/210941979-6db8b55c-2881-41d8-9e2e-6263b1dece13.jpg)
+![git-sim-log_01-05-23_22-02-39](https://user-images.githubusercontent.com/49353917/210940300-aadd14c6-72ab-4529-a1be-b494ed5dd4c9.jpg)
 
 ### git merge
 Usage: `git-sim merge <branch> [-m "Commit message"] [--no-ff]`
 
 - Specify `<branch>` as the branch name to merge into the active branch
 - If desired, specify a commit message with the `-m` option
 - Simulated output will depict a fast-forward merge if possible
 - Otherwise, a three-way merge will be depicted
 - To force a merge commit when a fast-forward is possible, use `--no-ff`
 - If merge fails due to merge conflicts, the conflicting files are displayed
 
 ![git-sim-merge_01-05-23_09-44-46](https://user-images.githubusercontent.com/49353917/210942030-c7229488-571a-4943-a1f4-c6e4a0c8ccf3.jpg)
 
-### git rebase
-Usage: `git-sim rebase <new-base>`
-
-- Specify `<new-base>` as the branch name to rebase the active branch onto
-
-![git-sim-rebase_01-05-23_09-53-34](https://user-images.githubusercontent.com/49353917/210942598-4ff8d1e6-464d-48f3-afb9-f46f7ec4828c.jpg)
-
-### git cherry-pick
-Usage: `git-sim cherry-pick <commit>`
-
-- Specify `<commit>` as a ref (branch name/tag) or commit ID to cherry-pick onto the active branch
-- Supports editing the cherry-picked commit message with: `$ git-sim cherry-pick <commit> -e "Edited commit message"`
-
-![git-sim-cherry-pick_01-05-23_22-23-08](https://user-images.githubusercontent.com/49353917/210942811-fa5155b1-4c6f-4afc-bea2-d39b4cd594aa.jpg)
-
-### git switch
-Usage: `git-sim switch [-c] <branch>`
-
-- Switches the checked-out branch to `<branch>`, i.e. moves `HEAD` to the specified `<branch>`
-- The `-c` flag creates a new branch with the specified name `<branch>` and switches to it, assuming it doesn't already exist
-
-![git-sim-switch_04-09-23_21-42-43](https://user-images.githubusercontent.com/49353917/230827783-a8740ace-b66f-4cac-b94e-5d101d27e0b5.jpg)
-
-### git checkout
-Usage: `git-sim checkout [-b] <branch>`
-
-- Checks out `<branch>` into the working directory, i.e. moves `HEAD` to the specified `<branch>`
-- The `-b` flag creates a new branch with the specified name `<branch>` and checks it out, assuming it doesn't already exist
-
-![git-sim-checkout_04-09-23_21-46-04](https://user-images.githubusercontent.com/49353917/230827836-e9f23a0e-2576-4716-b2fb-6327d3cf9b22.jpg)
-
-### git fetch
-Usage: `git-sim fetch <remote> <branch>`
+### git mv
+Usage: `git-sim mv <file> <new file>`
 
-- Fetches the specified `<branch>` from the specified `<remote>` to the local repo
+- Specify `<file>` as file to update name/path
+- Specify `<new file>` as new name/path of file 
+- Simulated output will show the name/path of the file being updated 
+- Note that simulated output will also show the most recent 5 commits on the active branch
 
-![git-sim-fetch_04-09-23_21-47-59](https://user-images.githubusercontent.com/49353917/230828090-acae8979-4097-43a8-96ea-525890e0e0a8.jpg)
+![git-sim-mv_04-09-23_22-05-13](https://user-images.githubusercontent.com/49353917/230829978-0a64dbe2-d974-4cef-9c6e-ed26e987342f.jpg)
 
 ### git pull
 Usage: `git-sim pull [<remote> <branch>]`
 
 - Pulls the specified `<branch>` from the specified `<remote>` to the local repo
 - If `<remote>` and `<branch>` are not specified, the active branch is pulled from the default remote
 - If merge conflicts occur, they are displayed in a table
@@ -340,49 +334,98 @@
 
 - Pushes the specified `<branch>` to the specified `<remote>` and displays the local result
 - If `<remote>` and `<branch>` are not specified, the active branch is pushed to the default remote
 - If the push fails due to remote changes that don't exist in the local repo, a message is included telling the user to pull first, along with color coding which commits need to be pulled
 
 ![git-sim-push_04-21-23_13-41-57](https://user-images.githubusercontent.com/49353917/233731005-51fd7887-ae14-4ceb-a5d5-e5aed79e9fd8.jpg)
 
-### git clone
-Usage: `git-sim clone <url>`
+### git rebase
+Usage: `git-sim rebase <new-base>`
 
-- Clone the remote repo from `<url>` (web URL or filesystem path) to a new folder in the current directory
-- Output will report if clone operation is successful and show log of local clone
+- Specify `<new-base>` as the branch name to rebase the active branch onto
 
-![git-sim-clone_04-09-23_21-51-53](https://user-images.githubusercontent.com/49353917/230828521-80c8d2d1-2a31-46bb-aeed-746f0441c86e.jpg)
+![git-sim-rebase_01-05-23_09-53-34](https://user-images.githubusercontent.com/49353917/210942598-4ff8d1e6-464d-48f3-afb9-f46f7ec4828c.jpg)
+
+### git remote
+Usage: `git-sim remote [add|rename|remove|get-url|set-url] [<remote>] [<url>]`
+
+- Simulated output will show remotes being added, renamed, removed, modified as indicated
+- Running `git-sim remote` with no options will list all existing remotes and their details  
+
+![git-sim-remote_04-16-24_08-40-37](https://github.com/initialcommit-com/git-sim/assets/49353917/ebaff04c-d5b6-4691-97b3-60bb502ba444)
+
+### git reset
+Usage: `git-sim reset <reset-to> [--mixed|--soft|--hard]`
+
+- Specify `<reset-to>` as any commit id, branch name, tag, or other ref to simulate reset to from the current HEAD (default: `HEAD`)
+- As with a normal git reset command, default reset mode is `--mixed`, but can be specified using `--soft`, `--hard`, or `--mixed`
+- Simulated output will show branch/HEAD resets and resulting state of the working directory, staging area, and whether any file changes would be deleted by running the actual command
+
+![git-sim-reset_01-05-23_22-15-49](https://user-images.githubusercontent.com/49353917/210941835-80f032d2-4f06-4032-8dd0-98c8a2569049.jpg)
+
+### git restore
+Usage: `git-sim restore <file 1> <file 2> ... <file n>`
+
+- Specify one or more `<file>` as a *modified* working directory file, or staged file
+- Simulated output will show files being moved back to the working directory or discarded changes
+- Note that simulated output will also show the most recent 5 commits on the active branch
+
+![git-sim-restore_01-05-23_22-09-14](https://user-images.githubusercontent.com/49353917/210941009-e6bf7271-ce9b-4e41-9a0b-24cc4b8d3b15.jpg)
+
+### git revert
+Usage: `git-sim revert <to-revert>`
+
+- Specify `<to-revert>` as any commit id, branch name, tag, or other ref to simulate revert for
+- Simulated output will show the new commit which reverts the changes from `<to-revert>`
+- Simulated output will include the next 4 most recent commits on the active branch
+
+![git-sim-revert_01-05-23_22-16-59](https://user-images.githubusercontent.com/49353917/210941979-6db8b55c-2881-41d8-9e2e-6263b1dece13.jpg)
 
 ### git rm
 Usage: `git-sim rm <file 1> <file 2> ... <file n>`
 
 - Specify one or more `<file>` as a *tracked* file
 - Simulated output will show files being removed from Git tracking
 - Note that simulated output will also show the most recent 5 commits on the active branch
 
 ![git-sim-rm_04-09-23_22-01-29](https://user-images.githubusercontent.com/49353917/230829899-f5d688ea-bc8e-46f9-a54a-55d251c8915d.jpg)
 
-### git mv
-Usage: `git-sim mv <file> <new file>`
+### git stash
+Usage: `git-sim stash [push|pop|apply] <file>`
 
-- Specify `<file>` as file to update name/path
-- Specify `<new file>` as new name/path of file 
-- Simulated output will show the name/path of the file being updated 
+- Specify one or more `<file>` as a *modified* working directory file, or staged file
+- If no `<file>` is specified, all available files will be included
+- Simulated output will show files being moved in/out of the Git stash
 - Note that simulated output will also show the most recent 5 commits on the active branch
 
-![git-sim-mv_04-09-23_22-05-13](https://user-images.githubusercontent.com/49353917/230829978-0a64dbe2-d974-4cef-9c6e-ed26e987342f.jpg)
+![git-sim-stash_01-05-23_22-11-18](https://user-images.githubusercontent.com/49353917/210941254-69c80b63-5c06-411a-a36a-1454b2906ee8.jpg)
 
-### git clean
-Usage: `git-sim clean`
+### git status
+Usage: `git-sim status`
 
-- Simulated output will show untracked files being deleted
-- Since this is just a simulation, no need to specify `-i`, `-n`, `-f` as in regular Git
+- Simulated output will show the state of the working directory, staging area, and untracked files
 - Note that simulated output will also show the most recent 5 commits on the active branch
 
-![git-sim-clean_04-09-23_22-05-54](https://user-images.githubusercontent.com/49353917/230830043-779e7230-f439-461a-a408-b19b263e86e4.jpg)
+![git-sim-status_01-05-23_22-06-28](https://user-images.githubusercontent.com/49353917/210940685-735665e2-fa12-4043-979c-54c295b13800.jpg)
+
+### git switch
+Usage: `git-sim switch [-c] <branch>`
+
+- Switches the checked-out branch to `<branch>`, i.e. moves `HEAD` to the specified `<branch>`
+- The `-c` flag creates a new branch with the specified name `<branch>` and switches to it, assuming it doesn't already exist
+
+![git-sim-switch_04-09-23_21-42-43](https://user-images.githubusercontent.com/49353917/230827783-a8740ace-b66f-4cac-b94e-5d101d27e0b5.jpg)
+
+### git tag
+Usage: `git-sim tag <new tag name>`
+
+- Specify `<new tag name>` as the name of the new tag to simulate creation of
+- Simulated output will show the newly create tag ref along with most recent 5 commits on the active branch
+
+![git-sim-tag_01-05-23_22-14-18](https://user-images.githubusercontent.com/49353917/210941647-79376ff7-2941-42b3-964a-b1d3a404a4fe.jpg)
 
 ## Video animation examples
 ```console
 $ git-sim --animate reset HEAD^
 ```
 
 https://user-images.githubusercontent.com/49353917/210943230-f38d879b-bb0d-4d42-a196-f24efb9e351a.mp4
```

### Comparing `git-sim-0.3.3/README.md` & `git_sim-0.3.4/src/git_sim.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,7 +1,35 @@
+Metadata-Version: 2.1
+Name: git-sim
+Version: 0.3.4
+Summary: Simulate Git commands on your own repos by generating an image (default) or video visualization depicting the command's behavior.
+Author-email: Jacob Stopak <jacob@initialcommit.io>
+License: GPL-2.0
+Project-URL: Homepage, https://initialcommit.com/tools/git-sim
+Project-URL: Source, https://github.com/initialcommit-com/git-sim
+Keywords: git,sim,simulation,simulate,git-simulate,git-simulation,git-sim,manim,animation,gitanimation,image,video,dryrun,dry-run
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: GNU General Public License v2 (GPLv2)
+Classifier: Operating System :: OS Independent
+Requires-Python: >=3.7
+Description-Content-Type: text/markdown
+License-File: LICENSE
+Requires-Dist: git-dummy
+Requires-Dist: gitpython
+Requires-Dist: manim
+Requires-Dist: opencv-python-headless
+Requires-Dist: pydantic_settings
+Requires-Dist: typer
+Requires-Dist: fonttools
+Provides-Extra: dev
+Requires-Dist: black; extra == "dev"
+Requires-Dist: numpy; extra == "dev"
+Requires-Dist: pillow; extra == "dev"
+Requires-Dist: pytest; extra == "dev"
+
 # git-sim
 ![git-sim-logo-with-tagline-1440x376p45](https://user-images.githubusercontent.com/49353917/232990611-58d0693f-69c0-45c8-b51d-cd540793d18c.gif)
 
 [![GitHub license](https://img.shields.io/github/license/initialcommit-com/git-sim)](https://github.com/initialcommit-com/git-sim/blob/main/LICENSE)
 [![GitHub tag](https://img.shields.io/github/v/release/initialcommit-com/git-sim)](https://img.shields.io/github/v/release/initialcommit-com/git-sim)
 [![Downloads](https://static.pepy.tech/badge/git-sim)](https://pepy.tech/project/git-sim)
 [![Contributors](https://img.shields.io/github/contributors/initialcommit-com/git-sim)](https://github.com/initialcommit-com/git-sim/graphs/contributors)
@@ -13,26 +41,33 @@
 
 Command syntax is based directly on Git's command-line syntax, so using git-sim is as familiar as possible.
 
 Example: `$ git-sim merge <branch>`
 <br/><br/>
 ![git-sim-merge_04-22-23_21-04-32_cropped](https://user-images.githubusercontent.com/49353917/233821875-a7bb640d-10be-4433-a8fb-bd25646eeff4.jpg)
 
+Check out the [git-sim release blog post](https://initialcommit.com/blog/git-sim) for the full scoop!
+
+## Support git-sim
+Git-Sim is Free and Open-Source Software (FOSS). Your support will help me work on it (and other Git projects) full time!
+- [Sponsor Git-Sim on GitHub](https://github.com/sponsors/initialcommit-com)
+- [Support Git-Sim via Patreon](https://patreon.com/user?u=92322459)
+
 ## Use cases
 - Visualize Git commands to understand their effects on your repo before actually running them
 - Prevent unexpected working directory and repository states by simulating before running
 - Share visualizations (jpg/png image or mp4/webm video) of your Git commands with your team, or the world
 - Save visualizations as a part of your team documentation to document workflow and prevent recurring issues
 - Create static Git diagrams (jpg/png) or dynamic animated videos (mp4/webm) to speed up content creation
 - Help visual learners understand how Git commands work
 - Combine with bundled command [git-dummy](https://github.com/initialcommit-com/git-dummy) to generate a dummy Git repo and then simulate operations on it
 
 ## Features
 - Run a one-liner git-sim command in the terminal to generate a custom Git command visualization (.jpg) from your repo
-- Supported commands: `log`, `status`, `add`, `restore`, `commit`, `stash`, `branch`, `tag`, `reset`, `revert`, `merge`, `rebase`, `cherry-pick`, `switch`, `checkout`, `fetch`, `pull`, `push`, `clone`, `rm`, `mv`, `clean`
+- Supported commands: `add`, `branch`, `checkout`, `cherry-pick`, `clean`, `clone`, `commit`, `config`, `fetch`, `init`, `log`, `merge`, `mv`, `pull`, `push`, `rebase`, `remote`, `reset`, `restore`, `revert`, `rm`, `stash`, `status`, `switch`, `tag`
 - Generate an animated video (.mp4) instead of a static image using the `--animate` flag (note: significant performance slowdown, it is recommended to use `--low-quality` to speed up testing and remove when ready to generate presentation-quality video)
 - Color commits by parameter, such as author with the `--color-by=author` option
 - Choose between dark mode (default) and light mode
 - Specify output formats of either jpg, png, mp4, or webm
 - Combine with bundled command [git-dummy](https://github.com/initialcommit-com/git-dummy) to generate a dummy Git repo and then simulate operations on it
 - Animation only: Add custom branded intro/outro sequences if desired
 - Animation only: Speed up or slow down animation speed as desired
@@ -124,15 +159,16 @@
 
 ## Requirements
 * Python 3.7 or greater
 * Pip (Package manager for Python)
 * [Manim (Community version)](https://www.manim.community/)
 
 ## Commands
-Basic usage is similar to Git itself - `git-sim` takes a familiar set of subcommands including "log", "status", "add", "restore", "commit", "stash", "branch", "tag", "reset", "revert", "merge", "rebase", "cherry-pick", "switch", "checkout", "fetch", "pull", "push", "clone", "rm", "mv", "clean" along with corresponding options.
+Basic usage is similar to Git itself - `git-sim` takes a familiar set of subcommands including "add", "branch", "checkout", "cherry-pick", "clean", "clone", "commit", "config", "fetch", "init", "log", "merge", "mv", "pull", "push", "rebase", "remote", "reset", "restore", "revert", "rm", "stash", "status", "switch", "tag" along with corresponding options.
+
 
 ```console
 $ git-sim [global options] <subcommand> [subcommand options]
 ```
 
 The `[global options]` apply to the overarching `git-sim` simulation itself, including:
 
@@ -159,159 +195,134 @@
 `--speed=n`: Set the multiple of animation speed of the output simulation, `n` can be an integer or float, default is 1.5.  
 `--low-quality`: Render the animation in low quality to speed up creation time, recommended for non-presentation use.  
 `--show-intro`: Add an intro sequence with custom logo and title.  
 `--show-outro`: Add an outro sequence with custom logo and text.  
 `--title=title`: Custom title to display at the beginning of the animation.  
 `--logo=logo.png`: The path to a custom logo to use in the animation intro/outro.  
 `--outro-top-text`: Custom text to display above the logo during the outro.  
-`--outro-bottom-text`: Custom text to display below the logo during the outro.
+`--outro-bottom-text`: Custom text to display below the logo during the outro.  
+`--font`: Font family used to display rendered text.
 
 The `[subcommand options]` are like regular Git options specific to the specified subcommand (see below for a full list).
 
 The following is a list of Git commands that can be simulated and their corresponding options/flags.
 
-### git log
-Usage: `git-sim log [-n <number>] [--all]`
-
-- Simulated output will show the most recent 5 commits on the active branch by default
-- Use `-n <number>` to set number of commits to display from each branch head
-- Set `--all` to display all local branches in the log output
-
-![git-sim-log_01-05-23_22-02-39](https://user-images.githubusercontent.com/49353917/210940300-aadd14c6-72ab-4529-a1be-b494ed5dd4c9.jpg)
-
-### git status
-Usage: `git-sim status`
-
-- Simulated output will show the state of the working directory, staging area, and untracked files
-- Note that simulated output will also show the most recent 5 commits on the active branch
-
-![git-sim-status_01-05-23_22-06-28](https://user-images.githubusercontent.com/49353917/210940685-735665e2-fa12-4043-979c-54c295b13800.jpg)
-
 ### git add
 Usage: `git-sim add <file 1> <file 2> ... <file n>`
 
 - Specify one or more `<file>` as a *modified* working directory file, or an untracked file
 - Simulated output will show files being moved to the staging area
 - Note that simulated output will also show the most recent 5 commits on the active branch
 
 ![git-sim-add_01-05-23_22-07-40](https://user-images.githubusercontent.com/49353917/210940814-7e8dc318-6116-4e56-b415-bc547401a56a.jpg)
 
-### git restore
-Usage: `git-sim restore <file 1> <file 2> ... <file n>`
+### git branch
+Usage: `git-sim branch <new branch name>`
 
-- Specify one or more `<file>` as a *modified* working directory file, or staged file
-- Simulated output will show files being moved back to the working directory or discarded changes
+- Specify `<new branch name>` as the name of the new branch to simulate creation of
+- Simulated output will show the newly create branch ref along with most recent 5 commits on the active branch
+
+![git-sim-branch_01-05-23_22-13-17](https://user-images.githubusercontent.com/49353917/210941509-2a42a7a4-2168-4f62-913f-3f6fe74a0684.jpg)
+
+### git checkout
+Usage: `git-sim checkout [-b] <branch>`
+
+- Checks out `<branch>` into the working directory, i.e. moves `HEAD` to the specified `<branch>`
+- The `-b` flag creates a new branch with the specified name `<branch>` and checks it out, assuming it doesn't already exist
+
+![git-sim-checkout_04-09-23_21-46-04](https://user-images.githubusercontent.com/49353917/230827836-e9f23a0e-2576-4716-b2fb-6327d3cf9b22.jpg)
+
+### git cherry-pick
+Usage: `git-sim cherry-pick <commit>`
+
+- Specify `<commit>` as a ref (branch name/tag) or commit ID to cherry-pick onto the active branch
+- Supports editing the cherry-picked commit message with: `$ git-sim cherry-pick <commit> -e "Edited commit message"`
+
+![git-sim-cherry-pick_01-05-23_22-23-08](https://user-images.githubusercontent.com/49353917/210942811-fa5155b1-4c6f-4afc-bea2-d39b4cd594aa.jpg)
+
+### git clean
+Usage: `git-sim clean`
+
+- Simulated output will show untracked files being deleted
+- Since this is just a simulation, no need to specify `-i`, `-n`, `-f` as in regular Git
 - Note that simulated output will also show the most recent 5 commits on the active branch
 
-![git-sim-restore_01-05-23_22-09-14](https://user-images.githubusercontent.com/49353917/210941009-e6bf7271-ce9b-4e41-9a0b-24cc4b8d3b15.jpg)
+![git-sim-clean_04-09-23_22-05-54](https://user-images.githubusercontent.com/49353917/230830043-779e7230-f439-461a-a408-b19b263e86e4.jpg)
+
+### git clone
+Usage: `git-sim clone <url>`
+
+- Clone the remote repo from `<url>` (web URL or filesystem path) to a new folder in the current directory
+- Output will report if clone operation is successful and show log of local clone
+
+![git-sim-clone_04-09-23_21-51-53](https://user-images.githubusercontent.com/49353917/230828521-80c8d2d1-2a31-46bb-aeed-746f0441c86e.jpg)
 
 ### git commit
 Usage: `git-sim commit -m "Commit message"`
 
 - Simulated output will show the new commit added to the tip of the active branch
 - Specify a commit message with the `-m` option
 - HEAD and the active branch will be moved to the new commit
 - Simulated output will show files in the staging area being included in the new commit
 - Supports amending the last commit with: `$ git-sim commit --amend -m "Amended commit message"`
 
 ![git-sim-commit_01-05-23_22-10-21](https://user-images.githubusercontent.com/49353917/210941149-d83677a1-3ab7-4880-bc0f-871b1f150087.jpg)
 
-### git stash
-Usage: `git-sim stash [push|pop|apply] <file>`
-
-- Specify one or more `<file>` as a *modified* working directory file, or staged file
-- If no `<file>` is specified, all available files will be included
-- Simulated output will show files being moved in/out of the Git stash
-- Note that simulated output will also show the most recent 5 commits on the active branch
-
-![git-sim-stash_01-05-23_22-11-18](https://user-images.githubusercontent.com/49353917/210941254-69c80b63-5c06-411a-a36a-1454b2906ee8.jpg)
+### git config
+Usage: `git-sim config [--list] <section.option> <value>`
 
-### git branch
-Usage: `git-sim branch <new branch name>`
-
-- Specify `<new branch name>` as the name of the new branch to simulate creation of
-- Simulated output will show the newly create branch ref along with most recent 5 commits on the active branch
+- Simulated output describes the specified configuration change
+- Use `--list` or `-l` to display all configuration
 
-![git-sim-branch_01-05-23_22-13-17](https://user-images.githubusercontent.com/49353917/210941509-2a42a7a4-2168-4f62-913f-3f6fe74a0684.jpg)
+![git-sim-config_04-16-24_08-34-34](https://github.com/initialcommit-com/git-sim/assets/49353917/c123e7a7-1fff-4f5c-b4a2-1e34ea2a4d80)
 
-### git tag
-Usage: `git-sim tag <new tag name>`
+### git fetch
+Usage: `git-sim fetch <remote> <branch>`
 
-- Specify `<new tag name>` as the name of the new tag to simulate creation of
-- Simulated output will show the newly create tag ref along with most recent 5 commits on the active branch
+- Fetches the specified `<branch>` from the specified `<remote>` to the local repo
 
-![git-sim-tag_01-05-23_22-14-18](https://user-images.githubusercontent.com/49353917/210941647-79376ff7-2941-42b3-964a-b1d3a404a4fe.jpg)
+![git-sim-fetch_04-09-23_21-47-59](https://user-images.githubusercontent.com/49353917/230828090-acae8979-4097-43a8-96ea-525890e0e0a8.jpg)
 
-### git reset
-Usage: `git-sim reset <reset-to> [--mixed|--soft|--hard]`
+### git init
+Usage: `git-sim init`
 
-- Specify `<reset-to>` as any commit id, branch name, tag, or other ref to simulate reset to from the current HEAD (default: `HEAD`)
-- As with a normal git reset command, default reset mode is `--mixed`, but can be specified using `--soft`, `--hard`, or `--mixed`
-- Simulated output will show branch/HEAD resets and resulting state of the working directory, staging area, and whether any file changes would be deleted by running the actual command
+- Simulated output describes the initialized `.git/` directory and it's contents
 
-![git-sim-reset_01-05-23_22-15-49](https://user-images.githubusercontent.com/49353917/210941835-80f032d2-4f06-4032-8dd0-98c8a2569049.jpg)
+![git-sim-init_04-16-24_08-34-47](https://github.com/initialcommit-com/git-sim/assets/49353917/2abb1a4a-3022-4353-a828-2d337baa8383)
 
-### git revert
-Usage: `git-sim revert <to-revert>`
+### git log
+Usage: `git-sim log [-n <number>] [--all]`
 
-- Specify `<to-revert>` as any commit id, branch name, tag, or other ref to simulate revert for
-- Simulated output will show the new commit which reverts the changes from `<to-revert>`
-- Simulated output will include the next 4 most recent commits on the active branch
+- Simulated output will show the most recent 5 commits on the active branch by default
+- Use `-n <number>` to set number of commits to display from each branch head
+- Set `--all` to display all local branches in the log output
 
-![git-sim-revert_01-05-23_22-16-59](https://user-images.githubusercontent.com/49353917/210941979-6db8b55c-2881-41d8-9e2e-6263b1dece13.jpg)
+![git-sim-log_01-05-23_22-02-39](https://user-images.githubusercontent.com/49353917/210940300-aadd14c6-72ab-4529-a1be-b494ed5dd4c9.jpg)
 
 ### git merge
 Usage: `git-sim merge <branch> [-m "Commit message"] [--no-ff]`
 
 - Specify `<branch>` as the branch name to merge into the active branch
 - If desired, specify a commit message with the `-m` option
 - Simulated output will depict a fast-forward merge if possible
 - Otherwise, a three-way merge will be depicted
 - To force a merge commit when a fast-forward is possible, use `--no-ff`
 - If merge fails due to merge conflicts, the conflicting files are displayed
 
 ![git-sim-merge_01-05-23_09-44-46](https://user-images.githubusercontent.com/49353917/210942030-c7229488-571a-4943-a1f4-c6e4a0c8ccf3.jpg)
 
-### git rebase
-Usage: `git-sim rebase <new-base>`
-
-- Specify `<new-base>` as the branch name to rebase the active branch onto
-
-![git-sim-rebase_01-05-23_09-53-34](https://user-images.githubusercontent.com/49353917/210942598-4ff8d1e6-464d-48f3-afb9-f46f7ec4828c.jpg)
-
-### git cherry-pick
-Usage: `git-sim cherry-pick <commit>`
-
-- Specify `<commit>` as a ref (branch name/tag) or commit ID to cherry-pick onto the active branch
-- Supports editing the cherry-picked commit message with: `$ git-sim cherry-pick <commit> -e "Edited commit message"`
-
-![git-sim-cherry-pick_01-05-23_22-23-08](https://user-images.githubusercontent.com/49353917/210942811-fa5155b1-4c6f-4afc-bea2-d39b4cd594aa.jpg)
-
-### git switch
-Usage: `git-sim switch [-c] <branch>`
-
-- Switches the checked-out branch to `<branch>`, i.e. moves `HEAD` to the specified `<branch>`
-- The `-c` flag creates a new branch with the specified name `<branch>` and switches to it, assuming it doesn't already exist
-
-![git-sim-switch_04-09-23_21-42-43](https://user-images.githubusercontent.com/49353917/230827783-a8740ace-b66f-4cac-b94e-5d101d27e0b5.jpg)
-
-### git checkout
-Usage: `git-sim checkout [-b] <branch>`
-
-- Checks out `<branch>` into the working directory, i.e. moves `HEAD` to the specified `<branch>`
-- The `-b` flag creates a new branch with the specified name `<branch>` and checks it out, assuming it doesn't already exist
-
-![git-sim-checkout_04-09-23_21-46-04](https://user-images.githubusercontent.com/49353917/230827836-e9f23a0e-2576-4716-b2fb-6327d3cf9b22.jpg)
-
-### git fetch
-Usage: `git-sim fetch <remote> <branch>`
+### git mv
+Usage: `git-sim mv <file> <new file>`
 
-- Fetches the specified `<branch>` from the specified `<remote>` to the local repo
+- Specify `<file>` as file to update name/path
+- Specify `<new file>` as new name/path of file 
+- Simulated output will show the name/path of the file being updated 
+- Note that simulated output will also show the most recent 5 commits on the active branch
 
-![git-sim-fetch_04-09-23_21-47-59](https://user-images.githubusercontent.com/49353917/230828090-acae8979-4097-43a8-96ea-525890e0e0a8.jpg)
+![git-sim-mv_04-09-23_22-05-13](https://user-images.githubusercontent.com/49353917/230829978-0a64dbe2-d974-4cef-9c6e-ed26e987342f.jpg)
 
 ### git pull
 Usage: `git-sim pull [<remote> <branch>]`
 
 - Pulls the specified `<branch>` from the specified `<remote>` to the local repo
 - If `<remote>` and `<branch>` are not specified, the active branch is pulled from the default remote
 - If merge conflicts occur, they are displayed in a table
@@ -323,49 +334,98 @@
 
 - Pushes the specified `<branch>` to the specified `<remote>` and displays the local result
 - If `<remote>` and `<branch>` are not specified, the active branch is pushed to the default remote
 - If the push fails due to remote changes that don't exist in the local repo, a message is included telling the user to pull first, along with color coding which commits need to be pulled
 
 ![git-sim-push_04-21-23_13-41-57](https://user-images.githubusercontent.com/49353917/233731005-51fd7887-ae14-4ceb-a5d5-e5aed79e9fd8.jpg)
 
-### git clone
-Usage: `git-sim clone <url>`
+### git rebase
+Usage: `git-sim rebase <new-base>`
 
-- Clone the remote repo from `<url>` (web URL or filesystem path) to a new folder in the current directory
-- Output will report if clone operation is successful and show log of local clone
+- Specify `<new-base>` as the branch name to rebase the active branch onto
 
-![git-sim-clone_04-09-23_21-51-53](https://user-images.githubusercontent.com/49353917/230828521-80c8d2d1-2a31-46bb-aeed-746f0441c86e.jpg)
+![git-sim-rebase_01-05-23_09-53-34](https://user-images.githubusercontent.com/49353917/210942598-4ff8d1e6-464d-48f3-afb9-f46f7ec4828c.jpg)
+
+### git remote
+Usage: `git-sim remote [add|rename|remove|get-url|set-url] [<remote>] [<url>]`
+
+- Simulated output will show remotes being added, renamed, removed, modified as indicated
+- Running `git-sim remote` with no options will list all existing remotes and their details  
+
+![git-sim-remote_04-16-24_08-40-37](https://github.com/initialcommit-com/git-sim/assets/49353917/ebaff04c-d5b6-4691-97b3-60bb502ba444)
+
+### git reset
+Usage: `git-sim reset <reset-to> [--mixed|--soft|--hard]`
+
+- Specify `<reset-to>` as any commit id, branch name, tag, or other ref to simulate reset to from the current HEAD (default: `HEAD`)
+- As with a normal git reset command, default reset mode is `--mixed`, but can be specified using `--soft`, `--hard`, or `--mixed`
+- Simulated output will show branch/HEAD resets and resulting state of the working directory, staging area, and whether any file changes would be deleted by running the actual command
+
+![git-sim-reset_01-05-23_22-15-49](https://user-images.githubusercontent.com/49353917/210941835-80f032d2-4f06-4032-8dd0-98c8a2569049.jpg)
+
+### git restore
+Usage: `git-sim restore <file 1> <file 2> ... <file n>`
+
+- Specify one or more `<file>` as a *modified* working directory file, or staged file
+- Simulated output will show files being moved back to the working directory or discarded changes
+- Note that simulated output will also show the most recent 5 commits on the active branch
+
+![git-sim-restore_01-05-23_22-09-14](https://user-images.githubusercontent.com/49353917/210941009-e6bf7271-ce9b-4e41-9a0b-24cc4b8d3b15.jpg)
+
+### git revert
+Usage: `git-sim revert <to-revert>`
+
+- Specify `<to-revert>` as any commit id, branch name, tag, or other ref to simulate revert for
+- Simulated output will show the new commit which reverts the changes from `<to-revert>`
+- Simulated output will include the next 4 most recent commits on the active branch
+
+![git-sim-revert_01-05-23_22-16-59](https://user-images.githubusercontent.com/49353917/210941979-6db8b55c-2881-41d8-9e2e-6263b1dece13.jpg)
 
 ### git rm
 Usage: `git-sim rm <file 1> <file 2> ... <file n>`
 
 - Specify one or more `<file>` as a *tracked* file
 - Simulated output will show files being removed from Git tracking
 - Note that simulated output will also show the most recent 5 commits on the active branch
 
 ![git-sim-rm_04-09-23_22-01-29](https://user-images.githubusercontent.com/49353917/230829899-f5d688ea-bc8e-46f9-a54a-55d251c8915d.jpg)
 
-### git mv
-Usage: `git-sim mv <file> <new file>`
+### git stash
+Usage: `git-sim stash [push|pop|apply] <file>`
 
-- Specify `<file>` as file to update name/path
-- Specify `<new file>` as new name/path of file 
-- Simulated output will show the name/path of the file being updated 
+- Specify one or more `<file>` as a *modified* working directory file, or staged file
+- If no `<file>` is specified, all available files will be included
+- Simulated output will show files being moved in/out of the Git stash
 - Note that simulated output will also show the most recent 5 commits on the active branch
 
-![git-sim-mv_04-09-23_22-05-13](https://user-images.githubusercontent.com/49353917/230829978-0a64dbe2-d974-4cef-9c6e-ed26e987342f.jpg)
+![git-sim-stash_01-05-23_22-11-18](https://user-images.githubusercontent.com/49353917/210941254-69c80b63-5c06-411a-a36a-1454b2906ee8.jpg)
 
-### git clean
-Usage: `git-sim clean`
+### git status
+Usage: `git-sim status`
 
-- Simulated output will show untracked files being deleted
-- Since this is just a simulation, no need to specify `-i`, `-n`, `-f` as in regular Git
+- Simulated output will show the state of the working directory, staging area, and untracked files
 - Note that simulated output will also show the most recent 5 commits on the active branch
 
-![git-sim-clean_04-09-23_22-05-54](https://user-images.githubusercontent.com/49353917/230830043-779e7230-f439-461a-a408-b19b263e86e4.jpg)
+![git-sim-status_01-05-23_22-06-28](https://user-images.githubusercontent.com/49353917/210940685-735665e2-fa12-4043-979c-54c295b13800.jpg)
+
+### git switch
+Usage: `git-sim switch [-c] <branch>`
+
+- Switches the checked-out branch to `<branch>`, i.e. moves `HEAD` to the specified `<branch>`
+- The `-c` flag creates a new branch with the specified name `<branch>` and switches to it, assuming it doesn't already exist
+
+![git-sim-switch_04-09-23_21-42-43](https://user-images.githubusercontent.com/49353917/230827783-a8740ace-b66f-4cac-b94e-5d101d27e0b5.jpg)
+
+### git tag
+Usage: `git-sim tag <new tag name>`
+
+- Specify `<new tag name>` as the name of the new tag to simulate creation of
+- Simulated output will show the newly create tag ref along with most recent 5 commits on the active branch
+
+![git-sim-tag_01-05-23_22-14-18](https://user-images.githubusercontent.com/49353917/210941647-79376ff7-2941-42b3-964a-b1d3a404a4fe.jpg)
 
 ## Video animation examples
 ```console
 $ git-sim --animate reset HEAD^
 ```
 
 https://user-images.githubusercontent.com/49353917/210943230-f38d879b-bb0d-4d42-a196-f24efb9e351a.mp4
```

### Comparing `git-sim-0.3.3/git_sim/__main__.py` & `git_sim-0.3.4/src/git_sim/__main__.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,27 +1,38 @@
+import contextlib
 import datetime
 import os
 import pathlib
 import sys
 import time
+from pathlib import Path
 
 import typer
+import manim as m
+
+from fontTools.ttLib import TTFont
 
 import git_sim.commands
 from git_sim.settings import (
     ColorByOptions,
     StyleOptions,
     ImgFormat,
     VideoFormat,
     settings,
 )
 
 app = typer.Typer(context_settings={"help_option_names": ["-h", "--help"]})
 
 
+def get_font_name(font_path):
+    """Get the name of a font from its .ttf file."""
+    font = TTFont(font_path)
+    return font["name"].getName(4, 3, 1, 1033).toUnicode()
+
+
 def version_callback(value: bool) -> None:
     if value:
         print(f"git-sim version {git_sim.__version__}")
         raise typer.Exit()
 
 
 @app.callback(no_args_is_help=True)
@@ -44,15 +55,14 @@
     ),
     img_format: ImgFormat = typer.Option(
         settings.img_format,
         help="Output format for the image files.",
     ),
     light_mode: bool = typer.Option(
         settings.light_mode,
-        "--light-mode",
         help="Enable light-mode with white background",
     ),
     transparent_bg: bool = typer.Option(
         settings.transparent_bg,
         "--transparent-bg",
         help="Make background transparent",
     ),
@@ -153,14 +163,22 @@
         help="Show the version of git-sim and exit",
         callback=version_callback,
     ),
     style: StyleOptions = typer.Option(
         settings.style.value,
         help="Graphical style of the output image or animated video",
     ),
+    font: str = typer.Option(
+        settings.font,
+        help="Font family used to display rendered text",
+    ),
+    show_command_as_title: bool = typer.Option(
+        settings.show_command_as_title,
+        help="Use the simulated git command as the title of the output image or animated video",
+    ),
 ):
     import git
     from manim import WHITE, config
 
     settings.animate = animate
     settings.n = n
     settings.auto_open = auto_open
@@ -185,14 +203,24 @@
     settings.quiet = quiet
     settings.invert_branches = invert_branches
     settings.hide_merged_branches = hide_merged_branches
     settings.all = all
     settings.color_by = color_by
     settings.highlight_commit_messages = highlight_commit_messages
     settings.style = style
+    settings.show_command_as_title = show_command_as_title
+
+    # If font is a path, define the context that will be used when using Manim.
+    if Path(font).exists():
+        font_path = Path(font)
+        settings.font_context = m.register_font(font_path)
+        settings.font = get_font_name(font_path)
+    else:
+        settings.font_context = contextlib.nullcontext()
+        settings.font = font
 
     try:
         if sys.platform == "linux" or sys.platform == "darwin":
             repo_name = git.repo.Repo(
                 search_parent_directories=True
             ).working_tree_dir.split("/")[-1]
         elif sys.platform == "win32":
@@ -223,21 +251,24 @@
 app.command()(git_sim.commands.add)
 app.command()(git_sim.commands.branch)
 app.command()(git_sim.commands.checkout)
 app.command()(git_sim.commands.cherry_pick)
 app.command()(git_sim.commands.clean)
 app.command()(git_sim.commands.clone)
 app.command()(git_sim.commands.commit)
+app.command()(git_sim.commands.config)
 app.command()(git_sim.commands.fetch)
+app.command()(git_sim.commands.init)
 app.command()(git_sim.commands.log)
 app.command()(git_sim.commands.merge)
 app.command()(git_sim.commands.mv)
 app.command()(git_sim.commands.pull)
 app.command()(git_sim.commands.push)
 app.command()(git_sim.commands.rebase)
+app.command()(git_sim.commands.remote)
 app.command()(git_sim.commands.reset)
 app.command()(git_sim.commands.restore)
 app.command()(git_sim.commands.revert)
 app.command()(git_sim.commands.rm)
 app.command()(git_sim.commands.stash)
 app.command()(git_sim.commands.status)
 app.command()(git_sim.commands.switch)
```

### Comparing `git-sim-0.3.3/git_sim/add.py` & `git_sim-0.3.4/src/git_sim/add.py`

 * *Files 5% similar despite different names*

```diff
@@ -25,26 +25,27 @@
         for file in self.files:
             if file not in [x.a_path for x in self.repo.index.diff(None)] + [
                 z for z in self.repo.untracked_files
             ]:
                 print(f"git-sim error: No modified file with name: '{file}'")
                 sys.exit()
 
+        self.cmd += f"{type(self).__name__.lower()} {' '.join(self.files)}"
+
     def construct(self):
         if not settings.stdout and not settings.output_only_path and not settings.quiet:
-            print(
-                f"{settings.INFO_STRING} {type(self).__name__.lower()} {' '.join(self.files)}"
-            )
+            print(f"{settings.INFO_STRING} {self.cmd}")
 
         self.show_intro()
         self.parse_commits()
         self.recenter_frame()
         self.scale_frame()
         self.vsplit_frame()
         self.setup_and_draw_zones()
+        self.show_command_as_title()
         self.fadeout()
         self.show_outro()
 
     def populate_zones(
         self,
         firstColumnFileNames,
         secondColumnFileNames,
```

### Comparing `git-sim-0.3.3/git_sim/animations.py` & `git_sim-0.3.4/src/git_sim/animations.py`

 * *Files identical despite different names*

### Comparing `git-sim-0.3.3/git_sim/branch.py` & `git_sim-0.3.4/src/git_sim/branch.py`

 * *Files 3% similar despite different names*

```diff
@@ -4,27 +4,28 @@
 from git_sim.settings import settings
 
 
 class Branch(GitSimBaseCommand):
     def __init__(self, name: str):
         super().__init__()
         self.name = name
+        self.cmd += f"{type(self).__name__.lower()} {self.name}"
 
     def construct(self):
         if not settings.stdout and not settings.output_only_path and not settings.quiet:
-            print(f"{settings.INFO_STRING} {type(self).__name__.lower()} {self.name}")
+            print(f"{settings.INFO_STRING} {self.cmd}")
 
         self.show_intro()
         self.parse_commits()
         self.parse_all()
         self.center_frame_on_commit(self.get_commit())
 
         branchText = m.Text(
             self.name,
-            font="Monospace",
+            font=self.font,
             font_size=20,
             color=self.fontColor,
         )
         branchRec = m.Rectangle(
             color=m.GREEN,
             fill_color=m.GREEN,
             fill_opacity=0.25,
@@ -44,9 +45,10 @@
 
         self.toFadeOut.add(branchRec, branchText)
         self.drawnRefs[self.name] = fullbranch
 
         self.recenter_frame()
         self.scale_frame()
         self.color_by()
+        self.show_command_as_title()
         self.fadeout()
         self.show_outro()
```

### Comparing `git-sim-0.3.3/git_sim/checkout.py` & `git_sim-0.3.4/src/git_sim/checkout.py`

 * *Files 1% similar despite different names*

```diff
@@ -56,19 +56,21 @@
             self.selected_branches.append(self.branch)
 
         try:
             self.selected_branches.append(self.repo.active_branch.name)
         except TypeError:
             pass
 
+        self.cmd += (
+            f"{type(self).__name__.lower()}{' -b' if self.b else ''} {self.branch}"
+        )
+
     def construct(self):
         if not settings.stdout and not settings.output_only_path and not settings.quiet:
-            print(
-                f"{settings.INFO_STRING } {type(self).__name__.lower()}{' -b' if self.b else ''} {self.branch}"
-            )
+            print(f"{settings.INFO_STRING} {self.cmd}")
 
         self.show_intro()
         head_commit = self.get_commit()
 
         # using -b flag, create new branch label and exit
         if self.b:
             self.parse_commits(head_commit)
@@ -114,8 +116,9 @@
                 self.recenter_frame()
                 self.scale_frame()
                 self.reset_head(branch_commit.hexsha)
                 self.reset_branch(head_commit.hexsha)
 
         self.color_by()
         self.fadeout()
+        self.show_command_as_title()
         self.show_outro()
```

### Comparing `git-sim-0.3.3/git_sim/cherrypick.py` & `git_sim-0.3.4/src/git_sim/cherrypick.py`

 * *Files 3% similar despite different names*

```diff
@@ -27,20 +27,21 @@
             self.selected_branches.append(self.commit)
 
         try:
             self.selected_branches.append(self.repo.active_branch.name)
         except TypeError:
             pass
 
+        self.cmd += f"cherry-pick {self.commit}" + (
+            (' -e "' + self.edit + '"') if self.edit else ""
+        )
+
     def construct(self):
         if not settings.stdout and not settings.output_only_path and not settings.quiet:
-            print(
-                f"{settings.INFO_STRING} cherry-pick {self.commit}"
-                + ((' -e "' + self.edit + '"') if self.edit else "")
-            )
+            print(f"{settings.INFO_STRING} {self.cmd}")
 
         if self.repo.active_branch.name in self.repo.git.branch(
             "--contains", self.commit
         ):
             print(
                 "git-sim error: Commit '"
                 + self.commit
@@ -62,9 +63,10 @@
             self.edit if self.edit else cherry_picked_commit.message,
         )
         self.draw_arrow_between_commits(cherry_picked_commit.hexsha, "abcdef")
         self.recenter_frame()
         self.scale_frame()
         self.reset_head_branch("abcdef")
         self.color_by(offset=2)
+        self.show_command_as_title()
         self.fadeout()
         self.show_outro()
```

### Comparing `git-sim-0.3.3/git_sim/clean.py` & `git_sim-0.3.4/src/git_sim/clean.py`

 * *Files 5% similar despite different names*

```diff
@@ -17,28 +17,31 @@
         self.n = self.n_default
 
         try:
             self.selected_branches.append(self.repo.active_branch.name)
         except TypeError:
             pass
 
+        self.cmd += f"{type(self).__name__.lower()}"
+
     def construct(self):
         if not settings.stdout and not settings.output_only_path and not settings.quiet:
-            print(f"{settings.INFO_STRING} {type(self).__name__.lower()}")
+            print(f"{settings.INFO_STRING} {self.cmd}")
 
         self.show_intro()
         self.parse_commits()
         self.recenter_frame()
         self.scale_frame()
         self.vsplit_frame()
         self.setup_and_draw_zones(
             first_column_name="Untracked files",
             second_column_name="----",
             third_column_name="Deleted files",
         )
+        self.show_command_as_title()
         self.fadeout()
         self.show_outro()
 
     def create_zone_text(
         self,
         firstColumnFileNames,
         secondColumnFileNames,
@@ -54,15 +57,15 @@
         thirdColumnTitle,
         horizontal2,
     ):
         for i, f in enumerate(firstColumnFileNames):
             text = (
                 m.Text(
                     self.trim_path(f),
-                    font="Monospace",
+                    font=self.font,
                     font_size=24,
                     color=self.fontColor,
                 )
                 .move_to(
                     (firstColumnTitle.get_center()[0], horizontal2.get_center()[1], 0)
                 )
                 .shift(m.DOWN * 0.5 * (i + 1))
@@ -70,15 +73,15 @@
             firstColumnFiles.add(text)
             firstColumnFilesDict[f] = text
 
         for j, f in enumerate(secondColumnFileNames):
             text = (
                 m.Text(
                     self.trim_path(f),
-                    font="Monospace",
+                    font=self.font,
                     font_size=24,
                     color=self.fontColor,
                 )
                 .move_to(
                     (secondColumnTitle.get_center()[0], horizontal2.get_center()[1], 0)
                 )
                 .shift(m.DOWN * 0.5 * (j + 1))
@@ -90,15 +93,15 @@
             text = (
                 m.MarkupText(
                     "<span strikethrough='true' strikethrough_color='"
                     + self.fontColor
                     + "'>"
                     + self.trim_path(f)
                     + "</span>",
-                    font="Monospace",
+                    font=self.font,
                     font_size=24,
                     color=self.fontColor,
                 )
                 .move_to(
                     (thirdColumnTitle.get_center()[0], horizontal2.get_center()[1], 0)
                 )
                 .shift(m.DOWN * 0.5 * (h + 1))
```

### Comparing `git-sim-0.3.3/git_sim/clone.py` & `git_sim-0.3.4/src/git_sim/clone.py`

 * *Files 13% similar despite different names*

```diff
@@ -15,36 +15,44 @@
 
 
 class Clone(GitSimBaseCommand):
     # Override since 'clone' subcommand shouldn't require repo to exist
     def init_repo(self):
         pass
 
-    def __init__(self, url: str):
+    def __init__(self, url: str, path: str):
         super().__init__()
         self.url = url
+        self.path = path
         settings.max_branches_per_commit = 2
+        self.cmd += f"{type(self).__name__.lower()} {self.url + ('' if self.path == '.' else ' ' + self.path)}"
 
     def construct(self):
         if not settings.stdout and not settings.output_only_path and not settings.quiet:
-            print(f"{settings.INFO_STRING } {type(self).__name__.lower()} {self.url}")
+            print(f"{settings.INFO_STRING} {self.cmd}")
 
         self.show_intro()
 
         # Configure paths to make local clone to run networked commands in
         repo_name = re.search(r"/([^/]+)/?$", self.url)
         if repo_name:
             repo_name = repo_name.group(1)
             if repo_name.endswith(".git"):
                 repo_name = repo_name[:-4]
+        elif self.url == "." or self.url == "./" or self.url == ".\\":
+            repo_name = os.path.split(os.getcwd())[1]
         else:
             print(
                 f"git-sim error: Invalid repo URL, please confirm repo URL and try again"
             )
             sys.exit(1)
+
+        if self.url == os.path.join(self.path, repo_name):
+            print(f"git-sim error: Cannot clone into same path, please try again")
+            sys.exit(1)
         new_dir = os.path.join(tempfile.gettempdir(), "git_sim", repo_name)
 
         # Create local clone of local repo
         try:
             self.repo = git.Repo.clone_from(self.url, new_dir, no_hardlinks=True)
         except git.GitCommandError as e:
             print(
@@ -54,36 +62,37 @@
 
         head_commit = self.get_commit()
         self.parse_commits(head_commit)
         self.recenter_frame()
         self.scale_frame()
         self.add_details(repo_name)
         self.color_by()
+        self.show_command_as_title()
         self.fadeout()
         self.show_outro()
 
         # Unlink the program from the filesystem
         self.repo.git.clear_cache()
 
         # Delete the local clones
         shutil.rmtree(new_dir, onerror=self.del_rw)
 
     def add_details(self, repo_name):
         text1 = m.Text(
-            f"Successfully cloned from {self.url} into ./{repo_name}",
-            font="Monospace",
+            f"Successfully cloned from {self.url} into {repo_name if self.path == '.' else self.path}",
+            font=self.font,
             font_size=20,
             color=self.fontColor,
             weight=m.BOLD,
         )
         text1.move_to([self.camera.frame.get_center()[0], 4, 0])
 
         text2 = m.Text(
             f"Cloned repo log:",
-            font="Monospace",
+            font=self.font,
             font_size=20,
             color=self.fontColor,
             weight=m.BOLD,
         )
         text2.move_to(text1.get_center()).shift(m.DOWN / 2)
 
         self.toFadeOut.add(text1)
```

### Comparing `git-sim-0.3.3/git_sim/commands.py` & `git_sim-0.3.4/src/git_sim/commands.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,24 +1,25 @@
 from __future__ import annotations
 
 import typer
 
 from typing import List, TYPE_CHECKING
 
-from git_sim.enums import ResetMode, StashSubCommand
 from git_sim.settings import settings
+from git_sim.enums import ResetMode, StashSubCommand, RemoteSubCommand
 
 if TYPE_CHECKING:
     from manim import Scene
 
 
 def handle_animations(scene: Scene) -> None:
     from git_sim.animations import handle_animations as _handle_animations
 
-    return _handle_animations(scene)
+    with settings.font_context:
+        return _handle_animations(scene)
 
 
 def add(
     files: List[str] = typer.Argument(
         default=None,
         help="The names of one or more files to add to Git's staging area",
     )
@@ -86,18 +87,22 @@
 
 
 def clone(
     url: str = typer.Argument(
         ...,
         help="The web URL or filesystem path of the Git repo to clone",
     ),
+    path: str = typer.Argument(
+        default=".",
+        help="The web URL or filesystem path of the Git repo to clone",
+    ),
 ):
     from git_sim.clone import Clone
 
-    scene = Clone(url=url)
+    scene = Clone(url=url, path=path)
     handle_animations(scene=scene)
 
 
 def commit(
     message: str = typer.Option(
         "New commit",
         "--message",
@@ -112,14 +117,32 @@
     from git_sim.commit import Commit
 
     settings.hide_first_tag = True
     scene = Commit(message=message, amend=amend)
     handle_animations(scene=scene)
 
 
+def config(
+    l: bool = typer.Option(
+        False,
+        "-l",
+        "--list",
+        help="List existing local repo config settings",
+    ),
+    settings: List[str] = typer.Argument(
+        default=None,
+        help="The names and values of one or more config settings to set",
+    ),
+):
+    from git_sim.config import Config
+
+    scene = Config(l=l, settings=settings)
+    handle_animations(scene=scene)
+
+
 def fetch(
     remote: str = typer.Argument(
         default=None,
         help="The name of the remote to fetch from",
     ),
     branch: str = typer.Argument(
         default=None,
@@ -128,14 +151,21 @@
 ):
     from git_sim.fetch import Fetch
 
     scene = Fetch(remote=remote, branch=branch)
     handle_animations(scene=scene)
 
 
+def init():
+    from git_sim.init import Init
+
+    scene = Init()
+    handle_animations(scene=scene)
+
+
 def log(
     ctx: typer.Context,
     n: int = typer.Option(
         None,
         "-n",
         help="Number of commits to display from branch heads",
     ),
@@ -212,18 +242,23 @@
         default=None,
         help="The name of the remote to push to",
     ),
     branch: str = typer.Argument(
         default=None,
         help="The name of the branch to push",
     ),
+    set_upstream: bool = typer.Option(
+        False,
+        "--set-upstream",
+        help="Map the local branch to the specified upstream branch",
+    ),
 ):
     from git_sim.push import Push
 
-    scene = Push(remote=remote, branch=branch)
+    scene = Push(remote=remote, branch=branch, set_upstream=set_upstream)
     handle_animations(scene=scene)
 
 
 def rebase(
     branch: str = typer.Argument(
         ...,
         help="The branch to simulate rebasing the checked-out commit onto",
@@ -231,14 +266,34 @@
 ):
     from git_sim.rebase import Rebase
 
     scene = Rebase(branch=branch)
     handle_animations(scene=scene)
 
 
+def remote(
+    command: RemoteSubCommand = typer.Argument(
+        default=None,
+        help="Remote subcommand (add, rename, remove, get-url, set-url)",
+    ),
+    remote: str = typer.Argument(
+        default=None,
+        help="The name of the remote",
+    ),
+    url_or_path: str = typer.Argument(
+        default=None,
+        help="The url or path to the remote",
+    ),
+):
+    from git_sim.remote import Remote
+
+    scene = Remote(command=command, remote=remote, url_or_path=url_or_path)
+    handle_animations(scene=scene)
+
+
 def reset(
     commit: str = typer.Argument(
         default="HEAD",
         help="The ref (branch/tag), or commit ID to simulate reset to",
     ),
     mode: ResetMode = typer.Option(
         default="mixed",
@@ -264,20 +319,25 @@
     handle_animations(scene=scene)
 
 
 def restore(
     files: List[str] = typer.Argument(
         default=None,
         help="The names of one or more files to restore",
-    )
+    ),
+    staged: bool = typer.Option(
+        False,
+        "--staged",
+        help="Restore staged file to working directory",
+    ),
 ):
     from git_sim.restore import Restore
 
     settings.hide_first_tag = True
-    scene = Restore(files=files)
+    scene = Restore(files=files, staged=staged)
     handle_animations(scene=scene)
 
 
 def revert(
     commit: str = typer.Argument(
         default="HEAD",
         help="The ref (branch/tag), or commit ID to simulate revert",
@@ -308,19 +368,23 @@
         default=None,
         help="Stash subcommand (push, pop, apply)",
     ),
     files: List[str] = typer.Argument(
         default=None,
         help="The name of the file to stash changes for",
     ),
+    stash_index: str = typer.Argument(
+        default="0",
+        help="Stash index",
+    ),
 ):
     from git_sim.stash import Stash
 
     settings.hide_first_tag = True
-    scene = Stash(files=files, command=command)
+    scene = Stash(files=files, command=command, stash_index=stash_index)
     handle_animations(scene=scene)
 
 
 def status():
     from git_sim.status import Status
 
     settings.hide_first_tag = True
@@ -336,24 +400,38 @@
         help="The name of the branch to switch to",
     ),
     c: bool = typer.Option(
         False,
         "-c",
         help="Create the specified branch if it doesn't already exist",
     ),
+    detach: bool = typer.Option(
+        False,
+        "--detach",
+        help="Allow switch resulting in detached HEAD state",
+    ),
 ):
     from git_sim.switch import Switch
 
-    scene = Switch(branch=branch, c=c)
+    scene = Switch(branch=branch, c=c, detach=detach)
     handle_animations(scene=scene)
 
 
 def tag(
     name: str = typer.Argument(
         ...,
-        help="The name of the new tag",
-    )
+        help="The name of the tag",
+    ),
+    commit: str = typer.Argument(
+        default=None,
+        help="The commit to tag",
+    ),
+    d: bool = typer.Option(
+        False,
+        "-d",
+        help="Delete the specified tag",
+    ),
 ):
     from git_sim.tag import Tag
 
-    scene = Tag(name=name)
+    scene = Tag(name=name, commit=commit, d=d)
     handle_animations(scene=scene)
```

### Comparing `git-sim-0.3.3/git_sim/commit.py` & `git_sim-0.3.4/src/git_sim/commit.py`

 * *Files 4% similar despite different names*

```diff
@@ -26,22 +26,24 @@
 
         if self.amend and self.message == "New commit":
             print(
                 "git-sim error: The --amend flag must be used with the -m flag to specify the amended commit message."
             )
             sys.exit(1)
 
+        self.cmd += (
+            f"{type(self).__name__.lower()} {'--amend ' if self.amend else ''}"
+            + '-m "'
+            + self.message
+            + '"'
+        )
+
     def construct(self):
         if not settings.stdout and not settings.output_only_path and not settings.quiet:
-            print(
-                f"{settings.INFO_STRING } {type(self).__name__.lower()} {'--amend ' if self.amend else ''}"
-                + '-m "'
-                + self.message
-                + '"'
-            )
+            print(f"{settings.INFO_STRING} {self.cmd}")
 
         self.show_intro()
         head_commit = self.get_commit()
 
         if self.amend:
             tree = self.repo.tree()
             amended = git.Commit.create_from_tree(
@@ -69,18 +71,19 @@
         self.scale_frame()
 
         if not self.amend:
             self.reset_head_branch("abcdef")
             self.vsplit_frame()
             self.setup_and_draw_zones(
                 first_column_name="Working directory",
-                second_column_name="Staging area",
+                second_column_name="Staged files",
                 third_column_name="New commit",
             )
 
+        self.show_command_as_title()
         self.fadeout()
         self.show_outro()
 
     def populate_zones(
         self,
         firstColumnFileNames,
         secondColumnFileNames,
@@ -89,14 +92,23 @@
         secondColumnArrowMap={},
         thirdColumnArrowMap={},
     ):
         for x in self.repo.index.diff(None):
             if "git-sim_media" not in x.a_path:
                 firstColumnFileNames.add(x.a_path)
 
-        for y in self.repo.index.diff("HEAD"):
-            if "git-sim_media" not in y.a_path:
-                secondColumnFileNames.add(y.a_path)
-                thirdColumnFileNames.add(y.a_path)
-                secondColumnArrowMap[y.a_path] = m.Arrow(
-                    stroke_width=3, color=self.fontColor
-                )
+        if self.head_exists():
+            for y in self.repo.index.diff("HEAD"):
+                if "git-sim_media" not in y.a_path:
+                    secondColumnFileNames.add(y.a_path)
+                    thirdColumnFileNames.add(y.a_path)
+                    secondColumnArrowMap[y.a_path] = m.Arrow(
+                        stroke_width=3, color=self.fontColor
+                    )
+        else:
+            for y in self.repo.index.diff(None, staged=True):
+                if "git-sim_media" not in y.a_path:
+                    secondColumnFileNames.add(y.a_path)
+                    thirdColumnFileNames.add(y.a_path)
+                    secondColumnArrowMap[y.a_path] = m.Arrow(
+                        stroke_width=3, color=self.fontColor
+                    )
```

### Comparing `git-sim-0.3.3/git_sim/enums.py` & `git_sim-0.3.4/src/git_sim/enums.py`

 * *Files 8% similar despite different names*

```diff
@@ -4,20 +4,14 @@
 class ResetMode(Enum):
     DEFAULT = "mixed"
     SOFT = "soft"
     MIXED = "mixed"
     HARD = "hard"
 
 
-class StashSubCommand(Enum):
-    POP = "pop"
-    APPLY = "apply"
-    PUSH = "push"
-
-
 class ColorByOptions(Enum):
     AUTHOR = "author"
     BRANCH = "branch"
     NOTLOCAL1 = "notlocal1"
     NOTLOCAL2 = "notlocal2"
 
 
@@ -30,7 +24,21 @@
     MP4 = "mp4"
     WEBM = "webm"
 
 
 class ImgFormat(str, Enum):
     JPG = "jpg"
     PNG = "png"
+
+
+class StashSubCommand(Enum):
+    POP = "pop"
+    APPLY = "apply"
+    PUSH = "push"
+
+
+class RemoteSubCommand(Enum):
+    ADD = "add"
+    RENAME = "rename"
+    REMOVE = "remove"
+    GET_URL = "get-url"
+    SET_URL = "set-url"
```

### Comparing `git-sim-0.3.3/git_sim/fetch.py` & `git_sim-0.3.4/src/git_sim/fetch.py`

 * *Files 2% similar despite different names*

```diff
@@ -20,19 +20,19 @@
         self.branch = branch
         settings.max_branches_per_commit = 2
 
         if self.remote and self.remote not in self.repo.remotes:
             print("git-sim error: no remote with name '" + self.remote + "'")
             sys.exit(1)
 
+        self.cmd += f"{type(self).__name__.lower()} {self.remote if self.remote else ''} {self.branch if self.branch else ''}"
+
     def construct(self):
         if not settings.stdout and not settings.output_only_path and not settings.quiet:
-            print(
-                f"{settings.INFO_STRING } {type(self).__name__.lower()} {self.remote if self.remote else ''} {self.branch if self.branch else ''}"
-            )
+            print(f"{settings.INFO_STRING} {self.cmd}")
 
         if not self.remote:
             self.remote = "origin"
         if not self.branch:
             self.branch = self.repo.active_branch.name
 
         self.show_intro()
@@ -75,11 +75,12 @@
         else:
             commit = self.get_commit(self.branch)
         self.parse_commits(commit)
 
         self.recenter_frame()
         self.scale_frame()
         self.color_by()
+        self.show_command_as_title()
         self.fadeout()
         self.show_outro()
         self.repo.git.clear_cache()
         shutil.rmtree(new_dir, onerror=self.del_rw)
```

### Comparing `git-sim-0.3.3/git_sim/git_sim_base_command.py` & `git_sim-0.3.4/src/git_sim/git_sim_base_command.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,23 +14,27 @@
 from git_sim.enums import ColorByOptions, StyleOptions
 from git_sim.settings import settings
 
 
 class GitSimBaseCommand(m.MovingCameraScene):
     def __init__(self):
         super().__init__()
+        self.cmd = "git "
         self.init_repo()
 
+        self.font = settings.font
         self.fontColor = m.BLACK if settings.light_mode else m.WHITE
         self.drawnCommits = {}
         self.drawnRefs = {}
+        self.drawnRefsByCommit = {}
         self.drawnCommitIds = {}
         self.toFadeOut = m.Group()
         self.prevRef = None
         self.topref = None
+        self.topelement = None
         self.n_default = settings.n_default
         self.n = settings.n
         self.n_orig = self.n
         self.n_dark_commits = 0
         self.selected_branches = []
         self.zone_title_offset = 2.6 if platform.system() == "Windows" else 2.6
         self.arrow_map = []
@@ -95,15 +99,17 @@
         print(f"{settings.INFO_STRING} {type(self).__name__.lower()}")
         self.show_intro()
         self.parse_commits()
         self.fadeout()
         self.show_outro()
 
     def get_commit(self, sha_or_ref="HEAD"):
-        return self.repo.commit(sha_or_ref)
+        if self.head_exists():
+            return self.repo.commit(sha_or_ref)
+        return "dark"
 
     def get_default_commits(self):
         defaultCommits = [self.get_commit()]
         for x in range(self.n_default - 1):
             defaultCommits.append(defaultCommits[-1].parents[0])
         return defaultCommits
 
@@ -111,14 +117,17 @@
         self,
         commit=None,
         i=0,
         prevCircle=None,
         shift=numpy.array([0.0, 0.0, 0.0]),
         make_branches_remote=False,
     ):
+        if not self.head_exists():
+            commit = self.create_dark_commit()
+
         commit = commit or self.get_commit()
 
         if commit != "dark":
             isNewCommit = commit.hexsha not in self.drawnCommits
         else:
             isNewCommit = True
 
@@ -183,15 +192,15 @@
 
     def show_intro(self):
         if settings.animate and settings.show_intro:
             self.add(self.logo)
 
             initialCommitText = m.Text(
                 settings.title,
-                font="Monospace",
+                font=self.font,
                 font_size=36,
                 color=self.fontColor,
             ).to_edge(m.UP, buff=1)
             self.add(initialCommitText)
             self.wait(2)
             self.play(m.FadeOut(initialCommitText))
             self.play(
@@ -211,23 +220,23 @@
         if settings.animate and settings.show_outro:
             self.play(m.Restore(self.camera.frame))
 
             self.play(self.logo.animate.scale(4).set_x(0).set_y(0))
 
             outroTopText = m.Text(
                 settings.outro_top_text,
-                font="Monospace",
+                font=self.font,
                 font_size=36,
                 color=self.fontColor,
             ).to_edge(m.UP, buff=1)
             self.play(m.AddTextLetterByLetter(outroTopText))
 
             outroBottomText = m.Text(
                 settings.outro_bottom_text,
-                font="Monospace",
+                font=self.font,
                 font_size=36,
                 color=self.fontColor,
             ).to_edge(m.DOWN, buff=1)
             self.play(m.AddTextLetterByLetter(outroBottomText))
 
             self.wait(3)
 
@@ -338,15 +347,15 @@
         if commit != "dark":
             self.drawnCommitIds[commit.hexsha] = commitId
 
         message = m.Text(
             "\n".join(
                 commitMessage[j : j + 20] for j in range(0, len(commitMessage), 20)
             )[:100],
-            font="Monospace",
+            font=self.font,
             font_size=20 if settings.highlight_commit_messages else 14,
             color=self.fontColor,
             weight=m.BOLD
             if settings.highlight_commit_messages
             or settings.style == StyleOptions.THICK
             else m.NORMAL,
         ).next_to(circle, m.DOWN)
@@ -399,24 +408,24 @@
         return [b for b in branches if b.name not in exclude]
 
     def build_commit_id_and_message(self, commit, i):
         hide_refs = False
         if commit == "dark":
             commitId = m.Text(
                 "",
-                font="Monospace",
+                font=self.font,
                 font_size=20,
                 color=self.fontColor,
                 weight=self.font_weight,
             )
             commitMessage = ""
         else:
             commitId = m.Text(
                 commit.hexsha[0:6],
-                font="Monospace",
+                font=self.font,
                 font_size=20,
                 color=self.fontColor,
                 weight=self.font_weight,
             )
             commitMessage = commit.message.split("\n")[0][:40].replace("\n", " ")
         return commitId, commitMessage, commit, hide_refs
 
@@ -429,29 +438,30 @@
             headbox.height = 0.4
             if settings.highlight_commit_messages:
                 headbox.next_to(self.drawnCommits[commit.hexsha], m.UP)
             else:
                 headbox.next_to(commitId, m.UP)
             headText = m.Text(
                 "HEAD",
-                font="Monospace",
+                font=self.font,
                 font_size=20,
                 color=self.fontColor,
                 weight=self.font_weight,
             ).move_to(headbox.get_center())
 
             head = m.VGroup(headbox, headText)
 
             if settings.animate:
                 self.play(m.Create(head), run_time=1 / settings.speed)
             else:
                 self.add(head)
 
             self.toFadeOut.add(head)
             self.drawnRefs["HEAD"] = head
+            self.add_ref_to_drawn_refs_by_commit(commit.hexsha, head)
             self.prevRef = head
 
             if i == 0 and self.first_parse:
                 self.topref = self.prevRef
 
     def draw_branch(self, commit, i, make_branches_remote=False):
         x = 0
@@ -463,32 +473,29 @@
         )
 
         for selected_branch in self.selected_branches:
             branches.insert(0, branches.pop(branches.index(selected_branch)))
 
         for branch in branches:
             if (
-                branch not in remote_tracking_branches # local branch
+                branch not in remote_tracking_branches  # local branch
                 and commit.hexsha == self.repo.heads[branch].commit.hexsha
             ) or (
-                branch in remote_tracking_branches # remote tracking branch
+                branch in remote_tracking_branches  # remote tracking branch
                 and commit.hexsha == remote_tracking_branches[branch]
             ):
                 text = (
                     (make_branches_remote + "/" + branch)
-                    if (
-                        make_branches_remote
-                        and branch not in remote_tracking_branches 
-                    )
+                    if (make_branches_remote and branch not in remote_tracking_branches)
                     else branch
                 )
 
                 branchText = m.Text(
                     text,
-                    font="Monospace",
+                    font=self.font,
                     font_size=20,
                     color=self.fontColor,
                     weight=self.font_weight,
                 )
                 branchRec = m.Rectangle(
                     color=m.GREEN,
                     fill_color=m.GREEN,
@@ -507,14 +514,15 @@
                 if settings.animate:
                     self.play(m.Create(fullbranch), run_time=1 / settings.speed)
                 else:
                     self.add(fullbranch)
 
                 self.toFadeOut.add(fullbranch)
                 self.drawnRefs[branch] = fullbranch
+                self.add_ref_to_drawn_refs_by_commit(commit.hexsha, fullbranch)
 
                 if i == 0 and self.first_parse:
                     self.topref = self.prevRef
 
                 x += 1
                 if x >= settings.max_branches_per_commit:
                     return
@@ -526,15 +534,15 @@
             return
 
         for tag in self.repo.tags:
             try:
                 if commit.hexsha == tag.commit.hexsha:
                     tagText = m.Text(
                         tag.name,
-                        font="Monospace",
+                        font=self.font,
                         font_size=20,
                         color=self.fontColor,
                         weight=self.font_weight,
                     )
                     tagRec = m.Rectangle(
                         color=m.YELLOW,
                         fill_color=m.YELLOW,
@@ -555,15 +563,16 @@
                             m.Create(fulltag),
                             run_time=1 / settings.speed,
                         )
                     else:
                         self.add(fulltag)
 
                     self.toFadeOut.add(fulltag)
-                    self.drawnRefs[tag] = fulltag
+                    self.drawnRefs[tag.name] = fulltag
+                    self.add_ref_to_drawn_refs_by_commit(commit.hexsha, fulltag)
 
                     if i == 0 and self.first_parse:
                         self.topref = self.prevRef
 
                     x += 1
                     if x >= settings.max_tags_per_commit:
                         return
@@ -587,30 +596,32 @@
                 run_time=1 / settings.speed,
             )
         else:
             self.camera.frame.move_to(self.toFadeOut.get_center())
 
     def scale_frame(self):
         if settings.animate:
-            self.play(
-                self.camera.frame.animate.scale_to_fit_width(
-                    self.toFadeOut.get_width() * 1.1
-                ),
-                run_time=1 / settings.speed,
-            )
-            if self.toFadeOut.get_height() >= self.camera.frame.get_height():
+            if self.toFadeOut.get_width() > self.camera.frame.get_width():
+                self.play(
+                    self.camera.frame.animate.scale_to_fit_width(
+                        self.toFadeOut.get_width() * 1.1
+                    ),
+                    run_time=1 / settings.speed,
+                )
+            if self.toFadeOut.get_height() > self.camera.frame.get_height():
                 self.play(
                     self.camera.frame.animate.scale_to_fit_height(
                         self.toFadeOut.get_height() * 1.25
                     ),
                     run_time=1 / settings.speed,
                 )
         else:
-            self.camera.frame.scale_to_fit_width(self.toFadeOut.get_width() * 1.1)
-            if self.toFadeOut.get_height() >= self.camera.frame.get_height():
+            if self.toFadeOut.get_width() > self.camera.frame.get_width():
+                self.camera.frame.scale_to_fit_width(self.toFadeOut.get_width() * 1.1)
+            if self.toFadeOut.get_height() > self.camera.frame.get_height():
                 self.camera.frame.scale_to_fit_height(
                     self.toFadeOut.get_height() * 1.25
                 )
 
     def vsplit_frame(self):
         if settings.animate:
             self.play(
@@ -621,55 +632,58 @@
         else:
             self.camera.frame.scale_to_fit_height(self.camera.frame.get_height() * 2)
 
         try:
             if settings.animate:
                 self.play(
                     self.toFadeOut.animate.align_to(self.camera.frame, m.UP).shift(
-                        m.DOWN * 0.75
+                        m.DOWN * 2.25
                     )
                 )
             else:
-                self.toFadeOut.align_to(self.camera.frame, m.UP).shift(m.DOWN * 0.75)
+                self.toFadeOut.align_to(self.camera.frame, m.UP).shift(m.DOWN * 2.25)
         except ValueError:
             pass
 
     def setup_and_draw_zones(
         self,
         first_column_name="Untracked files",
-        second_column_name="Working directory mods",
-        third_column_name="Staging area",
+        second_column_name="Modified files",
+        third_column_name="Staged files",
         reverse=False,
     ):
+        if self.check_all_dark():
+            self.zone_title_offset = 2.0 if platform.system() == "Windows" else 2.0
+
         horizontal = m.Line(
             (
                 self.camera.frame.get_left()[0],
                 self.camera.frame.get_center()[1],
                 0,
             ),
             (
                 self.camera.frame.get_right()[0],
                 self.camera.frame.get_center()[1],
                 0,
             ),
             color=self.fontColor,
-        ).shift(m.UP * 2.5)
+        ).shift(m.UP * 1.75)
         horizontal2 = m.Line(
             (
                 self.camera.frame.get_left()[0],
                 self.camera.frame.get_center()[1],
                 0,
             ),
             (
                 self.camera.frame.get_right()[0],
                 self.camera.frame.get_center()[1],
                 0,
             ),
             color=self.fontColor,
-        ).shift(m.UP * 1.5)
+        ).shift(m.UP * 0.75)
         vert1 = m.DashedLine(
             (
                 self.camera.frame.get_left()[0],
                 self.camera.frame.get_bottom()[1],
                 0,
             ),
             (self.camera.frame.get_left()[0], horizontal.get_start()[1], 0),
@@ -687,40 +701,41 @@
             color=self.fontColor,
         ).shift(m.LEFT * 8)
 
         if reverse:
             first_column_name = "Staging area"
             third_column_name = "Deleted changes"
 
+        title_v_shift = abs(horizontal2.get_start()[1] - horizontal.get_start()[1]) / 2
         firstColumnTitle = (
             m.Text(
                 first_column_name,
-                font="Monospace",
+                font=self.font,
                 font_size=28,
                 color=self.fontColor,
                 weight=m.BOLD,
             )
-            .move_to((vert1.get_center()[0] - 4, 0, 0))
-            .shift(m.UP * self.zone_title_offset)
+            .move_to((vert1.get_center()[0] - 4, horizontal.get_start()[1], 0))
+            .shift(m.DOWN * title_v_shift)
         )
         secondColumnTitle = (
             m.Text(
                 second_column_name,
-                font="Monospace",
+                font=self.font,
                 font_size=28,
                 color=self.fontColor,
                 weight=m.BOLD,
             )
             .move_to(self.camera.frame.get_center())
             .align_to(firstColumnTitle, m.UP)
         )
         thirdColumnTitle = (
             m.Text(
                 third_column_name,
-                font="Monospace",
+                font=self.font,
                 font_size=28,
                 color=self.fontColor,
                 weight=m.BOLD,
             )
             .move_to((vert2.get_center()[0] + 4, 0, 0))
             .align_to(firstColumnTitle, m.UP)
         )
@@ -916,24 +931,30 @@
                     thirdColumnFileNames.add(y)
 
         for z in self.repo.untracked_files:
             if "git-sim_media" not in z:
                 firstColumnFileNames.add(z)
 
     def center_frame_on_commit(self, commit):
+        if not commit or commit == "dark":
+            return
+
         if settings.animate:
             self.play(
                 self.camera.frame.animate.move_to(
                     self.drawnCommits[commit.hexsha].get_center()
                 )
             )
         else:
             self.camera.frame.move_to(self.drawnCommits[commit.hexsha].get_center())
 
     def reset_head_branch(self, hexsha, shift=numpy.array([0.0, 0.0, 0.0])):
+        if not self.head_exists():
+            return
+
         if settings.animate:
             self.play(
                 self.drawnRefs["HEAD"].animate.move_to(
                     (
                         self.drawnCommits[hexsha].get_center()[0] + shift[0],
                         self.drawnCommits[hexsha].get_center()[1] + 1.4 + shift[1],
                         0,
@@ -1034,49 +1055,52 @@
         circle = m.Circle(
             stroke_color=color,
             stroke_width=self.commit_stroke_width,
             fill_color=color,
             fill_opacity=self.ref_fill_opacity,
         )
         circle.height = 1
-        circle.next_to(
-            self.drawnCommits[child.hexsha],
-            m.LEFT if settings.reverse else m.RIGHT,
-            buff=1.5,
-        )
+        if child != "dark":
+            circle.next_to(
+                self.drawnCommits[child.hexsha],
+                m.LEFT if settings.reverse else m.RIGHT,
+                buff=1.5,
+            )
+
         circle.shift(shift)
 
-        start = circle.get_center()
-        end = self.drawnCommits[child.hexsha].get_center()
-        arrow = m.Arrow(
-            start,
-            end,
-            color=self.fontColor,
-            stroke_width=self.arrow_stroke_width,
-            tip_shape=self.arrow_tip_shape,
-            max_stroke_width_to_length_ratio=1000,
-        )
-        length = numpy.linalg.norm(start - end) - (1.5 if start[1] == end[1] else 3)
-        arrow.set_length(length)
+        if child != "dark":
+            start = circle.get_center()
+            end = self.drawnCommits[child.hexsha].get_center()
+            arrow = m.Arrow(
+                start,
+                end,
+                color=self.fontColor,
+                stroke_width=self.arrow_stroke_width,
+                tip_shape=self.arrow_tip_shape,
+                max_stroke_width_to_length_ratio=1000,
+            )
+            length = numpy.linalg.norm(start - end) - (1.5 if start[1] == end[1] else 3)
+            arrow.set_length(length)
 
         commitId = m.Text(
             "abcdef",
-            font="Monospace",
+            font=self.font,
             font_size=20,
             color=self.fontColor,
             weight=self.font_weight,
         ).next_to(circle, m.UP)
         self.toFadeOut.add(commitId)
 
         commitMessage = commitMessage.split("\n")[0][:40].replace("\n", " ")
         message = m.Text(
             "\n".join(
                 commitMessage[j : j + 20] for j in range(0, len(commitMessage), 20)
             )[:100],
-            font="Monospace",
+            font=self.font,
             font_size=14,
             color=self.fontColor,
             weight=self.font_weight,
         ).next_to(circle, m.DOWN)
         self.toFadeOut.add(message)
 
         if settings.animate:
@@ -1090,15 +1114,15 @@
         else:
             self.camera.frame.move_to(circle.get_center())
             self.add(circle, commitId, message)
 
         self.drawnCommits["abcdef"] = circle
         self.toFadeOut.add(circle)
 
-        if draw_arrow:
+        if draw_arrow and child != "dark":
             if settings.animate:
                 self.play(m.Create(arrow), run_time=1 / settings.speed)
             else:
                 self.add(arrow)
             self.arrows.append(arrow)
             self.toFadeOut.add(arrow)
 
@@ -1121,15 +1145,15 @@
     def get_nondark_commits(self):
         nondark_commits = []
         return nondark_commits
 
     def draw_ref(self, commit, top, i=0, text="HEAD", color=m.BLUE):
         refText = m.Text(
             text,
-            font="Monospace",
+            font=self.font,
             font_size=20,
             color=self.fontColor,
             weight=self.font_weight,
         )
         refbox = m.Rectangle(
             color=color,
             fill_color=color,
@@ -1163,15 +1187,18 @@
         )
         refRec.next_to(self.prevRef, m.UP)
         self.add(refRec)
         self.toFadeOut.add(refRec)
         self.prevRef = refRec
 
     def trim_path(self, path):
-        return (path[:15] + "..." + path[-15:]) if len(path) > 30 else path
+        return f"{path[:15]}...{path[-15:]}" if len(path) > 33 else path
+
+    def trim_cmd(self, path, length=30):
+        return f"{path[:length]}..." if len(path) > (length + 3) else path
 
     def get_remote_tracking_branches(self):
         remote_refs = [remote.refs for remote in self.repo.remotes]
         remote_tracking_branches = {}
         for reflist in remote_refs:
             for ref in reflist:
                 if "HEAD" not in ref.name and ref.name not in remote_tracking_branches:
@@ -1194,15 +1221,15 @@
         thirdColumnTitle,
         horizontal2,
     ):
         for i, f in enumerate(firstColumnFileNames):
             text = (
                 m.Text(
                     self.trim_path(f),
-                    font="Monospace",
+                    font=self.font,
                     font_size=24,
                     color=self.fontColor,
                 )
                 .move_to(
                     (firstColumnTitle.get_center()[0], horizontal2.get_center()[1], 0)
                 )
                 .shift(m.DOWN * 0.5 * (i + 1))
@@ -1210,15 +1237,15 @@
             firstColumnFiles.add(text)
             firstColumnFilesDict[f] = text
 
         for j, f in enumerate(secondColumnFileNames):
             text = (
                 m.Text(
                     self.trim_path(f),
-                    font="Monospace",
+                    font=self.font,
                     font_size=24,
                     color=self.fontColor,
                 )
                 .move_to(
                     (secondColumnTitle.get_center()[0], horizontal2.get_center()[1], 0)
                 )
                 .shift(m.DOWN * 0.5 * (j + 1))
@@ -1226,15 +1253,15 @@
             secondColumnFiles.add(text)
             secondColumnFilesDict[f] = text
 
         for h, f in enumerate(thirdColumnFileNames):
             text = (
                 m.Text(
                     self.trim_path(f),
-                    font="Monospace",
+                    font=self.font,
                     font_size=24,
                     color=self.fontColor,
                 )
                 .move_to(
                     (thirdColumnTitle.get_center()[0], horizontal2.get_center()[1], 0)
                 )
                 .shift(m.DOWN * 0.5 * (h + 1))
@@ -1248,15 +1275,15 @@
                 self.author_groups.keys(),
                 key=lambda k: len(self.author_groups[k]),
                 reverse=True,
             )
             for i, author in enumerate(sorted_authors):
                 authorText = m.Text(
                     f"{author[:15]} ({str(len(self.author_groups[author]))})",
-                    font="Monospace",
+                    font=self.font,
                     font_size=36,
                     color=self.colors[int(i % 11)],
                     weight=self.font_weight,
                 )
                 authorText.move_to(
                     [(-5 - offset) if settings.reverse else (5 + offset), -i, 0]
                 )
@@ -1290,18 +1317,68 @@
 
     def add_group_to_author_groups(self, author, group):
         if author not in self.author_groups:
             self.author_groups[author] = [group]
         else:
             self.author_groups[author].append(group)
 
+    def show_command_as_title(self):
+        if settings.show_command_as_title:
+            titleText = m.Text(
+                self.trim_cmd(self.cmd),
+                font=self.font,
+                font_size=36,
+                color=self.fontColor,
+            )
+            top = 0
+            for element in self.toFadeOut:
+                if element.get_top()[1] > top:
+                    top = element.get_top()[1]
+            titleText.move_to(
+                (
+                    self.camera.frame.get_x(),
+                    top + titleText.height * 2,
+                    0,
+                )
+            )
+            ul = m.Underline(
+                titleText,
+                color=self.fontColor,
+            )
+            self.toFadeOut.add(titleText, ul)
+            self.scale_frame()
+            if settings.animate:
+                self.play(m.AddTextLetterByLetter(titleText), m.Create(ul))
+            else:
+                self.add(titleText, ul)
+
     def del_rw(self, action, name, exc):
         os.chmod(name, stat.S_IWRITE)
         os.remove(name)
 
+    def head_exists(self):
+        try:
+            hc = self.repo.head.commit
+        except ValueError:
+            return False
+        return True
+
+    def check_all_dark(self):
+        if not self.drawnCommits:
+            return True
+        return False
+
+    def add_ref_to_drawn_refs_by_commit(self, hexsha, ref):
+        try:
+            self.drawnRefsByCommit[hexsha].append(ref)
+        except KeyError:
+            self.drawnRefsByCommit[hexsha] = [
+                ref,
+            ]
+
 
 class DottedLine(m.Line):
     def __init__(self, *args, dot_spacing=0.4, dot_kwargs={}, **kwargs):
         m.Line.__init__(self, *args, **kwargs)
         n_dots = int(self.get_length() / dot_spacing) + 1
         dot_spacing = self.get_length() / (n_dots - 1)
         unit_vector = self.get_unit_vector()
```

### Comparing `git-sim-0.3.3/git_sim/log.py` & `git_sim-0.3.4/src/git_sim/log.py`

 * *Files 7% similar despite different names*

```diff
@@ -28,20 +28,21 @@
         self.all = all
 
         try:
             self.selected_branches.append(self.repo.active_branch.name)
         except TypeError:
             pass
 
+        self.cmd += f"{type(self).__name__.lower()}{' --all' if self.all_subcommand else ''}{' -n ' + str(self.n) if self.n_subcommand else ''}"
+
     def construct(self):
         if not settings.stdout and not settings.output_only_path and not settings.quiet:
-            print(
-                f"{settings.INFO_STRING} {type(self).__name__.lower()}{' --all' if self.all_subcommand else ''}{' -n ' + str(self.n) if self.n_subcommand else ''}"
-            )
+            print(f"{settings.INFO_STRING} {self.cmd}")
         self.show_intro()
         self.parse_commits()
         self.parse_all()
         self.recenter_frame()
         self.scale_frame()
         self.color_by()
+        self.show_command_as_title()
         self.fadeout()
         self.show_outro()
```

### Comparing `git-sim-0.3.3/git_sim/merge.py` & `git_sim-0.3.4/src/git_sim/merge.py`

 * *Files 2% similar despite different names*

```diff
@@ -34,19 +34,19 @@
             self.selected_branches.append(self.branch)
 
         try:
             self.selected_branches.append(self.repo.active_branch.name)
         except TypeError:
             pass
 
+        self.cmd += f"{type(self).__name__.lower()} {self.branch} {'--no-ff' if self.no_ff else ''}"
+
     def construct(self):
         if not settings.stdout and not settings.output_only_path and not settings.quiet:
-            print(
-                f"{settings.INFO_STRING } {type(self).__name__.lower()} {self.branch} {'--no-ff' if self.no_ff else ''}"
-            )
+            print(f"{settings.INFO_STRING} {self.cmd}")
 
         if self.repo.active_branch.name in self.repo.git.branch(
             "--contains", self.branch
         ):
             print(
                 "git-sim error: Branch '"
                 + self.branch
@@ -147,14 +147,15 @@
                 self.draw_arrow_between_commits("abcdef", branch_commit.hexsha)
                 self.draw_arrow_between_commits("abcdef", head_commit.hexsha)
                 self.recenter_frame()
                 self.scale_frame()
                 self.reset_head_branch("abcdef")
                 self.color_by(offset=2)
 
+        self.show_command_as_title()
         self.fadeout()
         self.show_outro()
 
         # Unlink the program from the filesystem
         self.repo.git.clear_cache()
 
         # Delete the local clone
```

### Comparing `git-sim-0.3.3/git_sim/mv.py` & `git_sim-0.3.4/src/git_sim/mv.py`

 * *Files 4% similar despite different names*

```diff
@@ -25,31 +25,32 @@
 
             try:
                 self.repo.git.ls_files("--error-unmatch", self.file)
             except:
                 print(f"git-sim error: No tracked file with name: '{file}'")
                 sys.exit()
 
+        self.cmd += f"{type(self).__name__.lower()} {self.file} {self.new_file}"
+
     def construct(self):
         if not settings.stdout and not settings.output_only_path and not settings.quiet:
-            print(
-                f"{settings.INFO_STRING} {type(self).__name__.lower()} {self.file} {self.new_file}"
-            )
+            print(f"{settings.INFO_STRING} {self.cmd}")
 
         self.show_intro()
         self.parse_commits()
         self.recenter_frame()
         self.scale_frame()
         self.vsplit_frame()
         self.setup_and_draw_zones(
             first_column_name="Working directory",
             second_column_name="Staging area",
             third_column_name="Renamed files",
         )
         self.rename_moved_file()
+        self.show_command_as_title()
         self.fadeout()
         self.show_outro()
 
     def populate_zones(
         self,
         firstColumnFileNames,
         secondColumnFileNames,
@@ -71,15 +72,15 @@
 
         thirdColumnFileNames.add(self.file)
 
     def rename_moved_file(self):
         for file in self.thirdColumnFiles:
             new_file = m.Text(
                 self.trim_path(self.new_file),
-                font="Monospace",
+                font=self.font,
                 font_size=24,
                 color=self.fontColor,
             )
             new_file.move_to(file.get_center())
             if settings.animate:
                 self.play(m.FadeOut(file), run_time=1 / settings.speed)
                 self.toFadeOut.remove(file)
```

### Comparing `git-sim-0.3.3/git_sim/pull.py` & `git_sim-0.3.4/src/git_sim/pull.py`

 * *Files 2% similar despite different names*

```diff
@@ -21,19 +21,19 @@
         self.branch = branch
         settings.max_branches_per_commit = 2
 
         if self.remote and self.remote not in self.repo.remotes:
             print("git-sim error: no remote with name '" + self.remote + "'")
             sys.exit(1)
 
+        self.cmd += f"{type(self).__name__.lower()} {self.remote if self.remote else ''} {self.branch if self.branch else ''}"
+
     def construct(self):
         if not settings.stdout and not settings.output_only_path and not settings.quiet:
-            print(
-                f"{settings.INFO_STRING } {type(self).__name__.lower()} {self.remote if self.remote else ''} {self.branch if self.branch else ''}"
-            )
+            print(f"{settings.INFO_STRING} {self.cmd}")
 
         self.show_intro()
 
         # Configure paths to make local clone to run networked commands in
         git_root = self.repo.git.rev_parse("--show-toplevel")
         repo_name = os.path.basename(self.repo.working_dir)
         new_dir = os.path.join(tempfile.gettempdir(), "git_sim", repo_name)
@@ -83,14 +83,15 @@
                     f"git-sim error: git pull failed for unhandled reason: {e.stdout}"
                 )
                 self.repo.git.clear_cache()
                 shutil.rmtree(new_dir, onerror=self.del_rw)
                 sys.exit(1)
 
         self.color_by()
+        self.show_command_as_title()
         self.fadeout()
         self.show_outro()
 
         # Unlink the program from the filesystem
         self.repo.git.clear_cache()
 
         # Delete the local clone
```

### Comparing `git-sim-0.3.3/git_sim/push.py` & `git_sim-0.3.4/src/git_sim/push.py`

 * *Files 13% similar despite different names*

```diff
@@ -12,29 +12,32 @@
 
 from git_sim.git_sim_base_command import GitSimBaseCommand
 from git_sim.settings import settings
 from git_sim.enums import ColorByOptions
 
 
 class Push(GitSimBaseCommand):
-    def __init__(self, remote: str = None, branch: str = None):
+    def __init__(
+        self, remote: str = None, branch: str = None, set_upstream: bool = False
+    ):
         super().__init__()
         self.remote = remote
         self.branch = branch
+        self.set_upstream = set_upstream
         settings.max_branches_per_commit = 2
 
         if self.remote and self.remote not in self.repo.remotes:
             print("git-sim error: no remote with name '" + self.remote + "'")
             sys.exit(1)
 
+        self.cmd += f"{type(self).__name__.lower()} {'--set-upstream ' if self.set_upstream else ''}{self.remote if self.remote else ''} {self.branch if self.branch else ''}"
+
     def construct(self):
         if not settings.stdout and not settings.output_only_path and not settings.quiet:
-            print(
-                f"{settings.INFO_STRING } {type(self).__name__.lower()} {self.remote if self.remote else ''} {self.branch if self.branch else ''}"
-            )
+            print(f"{settings.INFO_STRING} {self.cmd}")
 
         self.show_intro()
 
         # Configure paths to make local clone to run networked commands in
         git_root = self.repo.git.rev_parse("--show-toplevel")
         repo_name = os.path.basename(self.repo.working_dir)
         new_dir = os.path.join(tempfile.gettempdir(), "git_sim", repo_name)
@@ -98,14 +101,15 @@
         else:
             self.parse_commits(head_commit)
 
         self.recenter_frame()
         self.scale_frame()
         self.failed_push(push_result)
         self.color_by()
+        self.show_command_as_title()
         self.fadeout()
         self.show_outro()
 
         # Unlink the program from the filesystem
         self.repo.git.clear_cache()
         if self.orig_repo:
             self.orig_repo.git.clear_cache()
@@ -115,80 +119,80 @@
         shutil.rmtree(new_dir2, onerror=self.del_rw)
 
     def failed_push(self, push_result):
         texts = []
         if push_result == 1:
             text1 = m.Text(
                 f"'git push' failed since the remote repo has commits that don't exist locally.",
-                font="Monospace",
+                font=self.font,
                 font_size=20,
                 color=self.fontColor,
                 weight=m.BOLD,
             )
             text1.move_to([self.camera.frame.get_center()[0], 5, 0])
 
             text2 = m.Text(
                 f"Run 'git pull' (or 'git-sim pull' to simulate first) and then try again.",
-                font="Monospace",
+                font=self.font,
                 font_size=20,
                 color=self.fontColor,
                 weight=m.BOLD,
             )
             text2.move_to(text1.get_center()).shift(m.DOWN / 2)
 
             text3 = m.Text(
                 f"Gold commits exist in remote repo, but not locally (need to be pulled).",
-                font="Monospace",
+                font=self.font,
                 font_size=20,
                 color=m.GOLD,
                 weight=m.BOLD,
             )
             text3.move_to(text2.get_center()).shift(m.DOWN / 2)
 
             text4 = m.Text(
                 f"Red commits exist in both local and remote repos.",
-                font="Monospace",
+                font=self.font,
                 font_size=20,
                 color=m.RED,
                 weight=m.BOLD,
             )
             text4.move_to(text3.get_center()).shift(m.DOWN / 2)
             texts = [text1, text2, text3, text4]
 
         elif push_result == 2:
             text1 = m.Text(
                 f"'git push' failed since the tip of your current branch is behind the remote.",
-                font="Monospace",
+                font=self.font,
                 font_size=20,
                 color=self.fontColor,
                 weight=m.BOLD,
             )
             text1.move_to([self.camera.frame.get_center()[0], 5, 0])
 
             text2 = m.Text(
                 f"Run 'git pull' (or 'git-sim pull' to simulate first) and then try again.",
-                font="Monospace",
+                font=self.font,
                 font_size=20,
                 color=self.fontColor,
                 weight=m.BOLD,
             )
             text2.move_to(text1.get_center()).shift(m.DOWN / 2)
 
             text3 = m.Text(
                 f"Gold commits are ahead of your current branch tip (need to be pulled).",
-                font="Monospace",
+                font=self.font,
                 font_size=20,
                 color=m.GOLD,
                 weight=m.BOLD,
             )
             text3.move_to(text2.get_center()).shift(m.DOWN / 2)
 
             text4 = m.Text(
                 f"Red commits are up to date in both local and remote branches.",
-                font="Monospace",
+                font=self.font,
                 font_size=20,
                 color=m.RED,
                 weight=m.BOLD,
             )
             text4.move_to(text3.get_center()).shift(m.DOWN / 2)
             texts = [text1, text2, text3, text4]
```

### Comparing `git-sim-0.3.3/git_sim/rebase.py` & `git_sim-0.3.4/src/git_sim/rebase.py`

 * *Files 2% similar despite different names*

```diff
@@ -27,19 +27,19 @@
             self.selected_branches.append(self.branch)
 
         try:
             self.selected_branches.append(self.repo.active_branch.name)
         except TypeError:
             pass
 
+        self.cmd += f"{type(self).__name__.lower()} {self.branch}"
+
     def construct(self):
         if not settings.stdout and not settings.output_only_path and not settings.quiet:
-            print(
-                f"{settings.INFO_STRING } {type(self).__name__.lower()} {self.branch}"
-            )
+            print(f"{settings.INFO_STRING} {self.cmd}")
 
         if self.branch in self.repo.git.branch(
             "--contains", self.repo.active_branch.name
         ):
             print(
                 "git-sim error: Branch '"
                 + self.repo.active_branch.name
@@ -97,14 +97,15 @@
             parent = self.setup_and_draw_parent(parent, message)
             self.draw_arrow_between_commits(tr.hexsha, parent)
 
         self.recenter_frame()
         self.scale_frame()
         self.reset_head_branch(parent)
         self.color_by(offset=2 * len(to_rebase))
+        self.show_command_as_title()
         self.fadeout()
         self.show_outro()
 
     def setup_and_draw_parent(
         self,
         child,
         commitMessage="New commit",
@@ -145,26 +146,26 @@
                 or chr(ord(letter) + 1).isdigit()
             )
             else letter
             for letter in child[:6]
         )
         commitId = m.Text(
             sha if commitMessage != "..." else "...",
-            font="Monospace",
+            font=self.font,
             font_size=20,
             color=self.fontColor,
         ).next_to(circle, m.UP)
         self.toFadeOut.add(commitId)
 
         commitMessage = commitMessage[:40].replace("\n", " ")
         message = m.Text(
             "\n".join(
                 commitMessage[j : j + 20] for j in range(0, len(commitMessage), 20)
             )[:100],
-            font="Monospace",
+            font=self.font,
             font_size=14,
             color=self.fontColor,
         ).next_to(circle, m.DOWN)
         self.toFadeOut.add(message)
 
         if settings.animate:
             self.play(
```

### Comparing `git-sim-0.3.3/git_sim/reset.py` & `git_sim-0.3.4/src/git_sim/reset.py`

 * *Files 6% similar despite different names*

```diff
@@ -37,59 +37,58 @@
         if hard:
             self.mode = ResetMode.HARD
         if mixed:
             self.mode = ResetMode.MIXED
         if soft:
             self.mode = ResetMode.SOFT
 
+        self.cmd += f"{type(self).__name__.lower()}{' --' + self.mode.value if self.mode != ResetMode.DEFAULT else ''} {self.commit}"
+
     def construct(self):
         if not settings.stdout and not settings.output_only_path and not settings.quiet:
-            print(
-                f"{settings.INFO_STRING } {type(self).__name__.lower()}{' --' + self.mode.value if self.mode != ResetMode.DEFAULT else ''} {self.commit}",
-            )
+            print(f"{settings.INFO_STRING} {self.cmd}")
 
         self.show_intro()
         self.parse_commits()
         self.recenter_frame()
         self.scale_frame()
         self.reset_head_branch(self.resetTo.hexsha)
         self.vsplit_frame()
         self.setup_and_draw_zones(first_column_name="Changes deleted from")
+        self.show_command_as_title()
         self.fadeout()
         self.show_outro()
 
     def build_commit_id_and_message(self, commit, i):
         hide_refs = False
         if commit == "dark":
-            commitId = m.Text("", font="Monospace", font_size=20, color=self.fontColor)
+            commitId = m.Text("", font=self.font, font_size=20, color=self.fontColor)
             commitMessage = ""
         elif i == 3 and self.resetTo.hexsha not in [
             c.hexsha for c in self.get_default_commits()
         ]:
-            commitId = m.Text(
-                "...", font="Monospace", font_size=20, color=self.fontColor
-            )
+            commitId = m.Text("...", font=self.font, font_size=20, color=self.fontColor)
             commitMessage = "..."
             hide_refs = True
         elif i == 4 and self.resetTo.hexsha not in [
             c.hexsha for c in self.get_default_commits()
         ]:
             commitId = m.Text(
                 self.resetTo.hexsha[:6],
-                font="Monospace",
+                font=self.font,
                 font_size=20,
                 color=self.fontColor,
             )
             commitMessage = self.resetTo.message.split("\n")[0][:40].replace("\n", " ")
             commit = self.resetTo
             hide_refs = True
         else:
             commitId = m.Text(
                 commit.hexsha[:6],
-                font="Monospace",
+                font=self.font,
                 font_size=20,
                 color=self.fontColor,
             )
             commitMessage = commit.message.split("\n")[0][:40].replace("\n", " ")
 
         if (
             commit != "dark"
```

### Comparing `git-sim-0.3.3/git_sim/restore.py` & `git_sim-0.3.4/src/git_sim/restore.py`

 * *Files 9% similar despite different names*

```diff
@@ -4,44 +4,52 @@
 from typing import List
 
 from git_sim.git_sim_base_command import GitSimBaseCommand
 from git_sim.settings import settings
 
 
 class Restore(GitSimBaseCommand):
-    def __init__(self, files: List[str]):
+    def __init__(self, files: List[str], staged: bool):
         super().__init__()
         self.files = files
+        self.staged = staged
         settings.hide_merged_branches = True
         self.n = self.n_default
 
         try:
             self.selected_branches.append(self.repo.active_branch.name)
         except TypeError:
             pass
 
-        for file in self.files:
-            if file not in [x.a_path for x in self.repo.index.diff(None)] + [
-                y.a_path for y in self.repo.index.diff("HEAD")
-            ]:
-                print(f"git-sim error: No modified or staged file with name: '{file}'")
-                sys.exit()
+        if not self.staged:
+            for file in self.files:
+                if file not in [x.a_path for x in self.repo.index.diff(None)]:
+                    print(f"git-sim error: No modified file with name: '{file}'")
+                    sys.exit()
+        else:
+            for file in self.files:
+                if file not in [y.a_path for y in self.repo.index.diff("HEAD")]:
+                    print(
+                        f"git-sim error: No modified or staged file with name: '{file}'"
+                    )
+                    sys.exit()
+
+        self.cmd += f"{type(self).__name__.lower()}{' --staged' if self.staged else ''} {' '.join(self.files)}"
 
     def construct(self):
         if not settings.stdout and not settings.output_only_path and not settings.quiet:
-            print(
-                f"{settings.INFO_STRING } {type(self).__name__.lower()} {' '.join(self.files)}"
-            )
+            print(f"{settings.INFO_STRING} {self.cmd}")
 
         self.show_intro()
         self.parse_commits()
         self.recenter_frame()
         self.scale_frame()
         self.vsplit_frame()
         self.setup_and_draw_zones(reverse=True)
+        self.show_command_as_title()
         self.fadeout()
         self.show_outro()
 
     def populate_zones(
         self,
         firstColumnFileNames,
         secondColumnFileNames,
```

### Comparing `git-sim-0.3.3/git_sim/revert.py` & `git_sim-0.3.4/src/git_sim/revert.py`

 * *Files 4% similar despite different names*

```diff
@@ -30,64 +30,63 @@
         self.zone_title_offset += 0.1
 
         try:
             self.selected_branches.append(self.repo.active_branch.name)
         except TypeError:
             pass
 
+        self.cmd += f"{type(self).__name__.lower()} {self.commit}"
+
     def construct(self):
         if not settings.stdout and not settings.output_only_path and not settings.quiet:
-            print(
-                f"{settings.INFO_STRING } {type(self).__name__.lower()} {self.commit}"
-            )
+            print(f"{settings.INFO_STRING} {self.cmd}")
 
         self.show_intro()
         self.parse_commits()
         self.center_frame_on_commit(self.get_commit())
         self.setup_and_draw_revert_commit()
         self.recenter_frame()
         self.scale_frame()
         self.reset_head_branch("abcdef")
         self.vsplit_frame()
         self.setup_and_draw_zones(
             first_column_name="----",
             second_column_name="Changes reverted from",
             third_column_name="----",
         )
+        self.show_command_as_title()
         self.fadeout()
         self.show_outro()
 
     def build_commit_id_and_message(self, commit, i):
         hide_refs = False
         if commit == "dark":
-            commitId = m.Text("", font="Monospace", font_size=20, color=self.fontColor)
+            commitId = m.Text("", font=self.font, font_size=20, color=self.fontColor)
             commitMessage = ""
         elif i == 2 and self.revert.hexsha not in [
             commit.hexsha for commit in self.get_default_commits()
         ]:
-            commitId = m.Text(
-                "...", font="Monospace", font_size=20, color=self.fontColor
-            )
+            commitId = m.Text("...", font=self.font, font_size=20, color=self.fontColor)
             commitMessage = "..."
             hide_refs = True
         elif i == 3 and self.revert.hexsha not in [
             commit.hexsha for commit in self.get_default_commits()
         ]:
             commitId = m.Text(
                 self.revert.hexsha[:6],
-                font="Monospace",
+                font=self.font,
                 font_size=20,
                 color=self.fontColor,
             )
             commitMessage = self.revert.message.split("\n")[0][:40].replace("\n", " ")
             hide_refs = True
         else:
             commitId = m.Text(
                 commit.hexsha[:6],
-                font="Monospace",
+                font=self.font,
                 font_size=20,
                 color=self.fontColor,
             )
             commitMessage = commit.message.split("\n")[0][:40].replace("\n", " ")
         return commitId, commitMessage, commit, hide_refs
 
     def setup_and_draw_revert_commit(self):
@@ -114,25 +113,25 @@
             tip_shape=self.arrow_tip_shape,
             max_stroke_width_to_length_ratio=1000,
         )
         length = numpy.linalg.norm(start - end) - (1.5 if start[1] == end[1] else 3)
         arrow.set_length(length)
 
         commitId = m.Text(
-            "abcdef", font="Monospace", font_size=20, color=self.fontColor
+            "abcdef", font=self.font, font_size=20, color=self.fontColor
         ).next_to(circle, m.UP)
         self.toFadeOut.add(commitId)
 
         commitMessage = "Revert " + self.revert.hexsha[0:6]
         commitMessage = commitMessage[:40].replace("\n", " ")
         message = m.Text(
             "\n".join(
                 commitMessage[j : j + 20] for j in range(0, len(commitMessage), 20)
             )[:100],
-            font="Monospace",
+            font=self.font,
             font_size=14,
             color=self.fontColor,
         ).next_to(circle, m.DOWN)
         self.toFadeOut.add(message)
 
         if settings.animate:
             self.play(
```

### Comparing `git-sim-0.3.3/git_sim/rm.py` & `git_sim-0.3.4/src/git_sim/rm.py`

 * *Files 8% similar despite different names*

```diff
@@ -25,30 +25,31 @@
         for file in self.files:
             try:
                 self.repo.git.ls_files("--error-unmatch", file)
             except:
                 print(f"git-sim error: No tracked file with name: '{file}'")
                 sys.exit()
 
+        self.cmd += f"{type(self).__name__.lower()} {' '.join(self.files)}"
+
     def construct(self):
         if not settings.stdout and not settings.output_only_path and not settings.quiet:
-            print(
-                f"{settings.INFO_STRING} {type(self).__name__.lower()} {' '.join(self.files)}"
-            )
+            print(f"{settings.INFO_STRING} {self.cmd}")
 
         self.show_intro()
         self.parse_commits()
         self.recenter_frame()
         self.scale_frame()
         self.vsplit_frame()
         self.setup_and_draw_zones(
             first_column_name="Working directory",
             second_column_name="Staging area",
             third_column_name="Removed files",
         )
+        self.show_command_as_title()
         self.fadeout()
         self.show_outro()
 
     def create_zone_text(
         self,
         firstColumnFileNames,
         secondColumnFileNames,
@@ -64,15 +65,15 @@
         thirdColumnTitle,
         horizontal2,
     ):
         for i, f in enumerate(firstColumnFileNames):
             text = (
                 m.Text(
                     self.trim_path(f),
-                    font="Monospace",
+                    font=self.font,
                     font_size=24,
                     color=self.fontColor,
                 )
                 .move_to(
                     (firstColumnTitle.get_center()[0], horizontal2.get_center()[1], 0)
                 )
                 .shift(m.DOWN * 0.5 * (i + 1))
@@ -80,15 +81,15 @@
             firstColumnFiles.add(text)
             firstColumnFilesDict[f] = text
 
         for j, f in enumerate(secondColumnFileNames):
             text = (
                 m.Text(
                     self.trim_path(f),
-                    font="Monospace",
+                    font=self.font,
                     font_size=24,
                     color=self.fontColor,
                 )
                 .move_to(
                     (secondColumnTitle.get_center()[0], horizontal2.get_center()[1], 0)
                 )
                 .shift(m.DOWN * 0.5 * (j + 1))
@@ -100,15 +101,15 @@
             text = (
                 m.MarkupText(
                     "<span strikethrough='true' strikethrough_color='"
                     + self.fontColor
                     + "'>"
                     + self.trim_path(f)
                     + "</span>",
-                    font="Monospace",
+                    font=self.font,
                     font_size=24,
                     color=self.fontColor,
                 )
                 .move_to(
                     (thirdColumnTitle.get_center()[0], horizontal2.get_center()[1], 0)
                 )
                 .shift(m.DOWN * 0.5 * (h + 1))
```

### Comparing `git-sim-0.3.3/git_sim/settings.py` & `git_sim-0.3.4/src/git_sim/settings.py`

 * *Files 8% similar despite different names*

```diff
@@ -11,15 +11,15 @@
     animate: bool = False
     auto_open: bool = True
     n_default: int = 5
     n: int = 5
     files: Union[List[pathlib.Path], None] = None
     hide_first_tag: bool = False
     img_format: ImgFormat = ImgFormat.JPG
-    INFO_STRING: str = "Simulating: git"
+    INFO_STRING: str = "Simulating:"
     light_mode: bool = False
     transparent_bg: bool = False
     logo: pathlib.Path = pathlib.Path(__file__).parent.resolve() / "logo.png"
     low_quality: bool = False
     max_branches_per_commit: int = 1
     max_tags_per_commit: int = 1
     media_dir: pathlib.Path = pathlib.Path().cwd()
@@ -36,13 +36,16 @@
     quiet: bool = False
     invert_branches: bool = False
     hide_merged_branches: bool = False
     all: bool = False
     color_by: Union[ColorByOptions, None] = None
     highlight_commit_messages: bool = False
     style: Union[StyleOptions, None] = StyleOptions.CLEAN
+    font: str = "Monospace"
+    font_context: bool = False
+    show_command_as_title: bool = True
 
     class Config:
         env_prefix = "git_sim_"
 
 
 settings = Settings()
```

### Comparing `git-sim-0.3.3/git_sim/stash.py` & `git_sim-0.3.4/src/git_sim/stash.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,27 +1,33 @@
+import re
 import sys
 from enum import Enum
 import manim as m
 
 from typing import List
 
 from git_sim.enums import StashSubCommand
 from git_sim.git_sim_base_command import GitSimBaseCommand
 from git_sim.settings import settings
 
 
 class Stash(GitSimBaseCommand):
-    def __init__(self, files: List[str], command: StashSubCommand):
+    def __init__(self, files: List[str], command: StashSubCommand, stash_index: int):
         super().__init__()
         self.files = files
         self.no_files = True if not self.files else False
         self.command = command
         settings.hide_merged_branches = True
         self.n = self.n_default
 
+        self.stash_index = self.parse_stash_format(stash_index)
+        if self.stash_index is None:
+            print("git-sim error: specify stash index as either integer or stash@{i}")
+            sys.exit()
+
         try:
             self.selected_branches.append(self.repo.active_branch.name)
         except TypeError:
             pass
 
         if self.command in [StashSubCommand.PUSH, None]:
             for file in self.files:
@@ -40,33 +46,34 @@
         elif self.files:
             if (
                 not settings.stdout
                 and not settings.output_only_path
                 and not settings.quiet
             ):
                 print(
-                    "Files are not required in apply/pop subcommand. Ignoring the file list....."
+                    "Files are not required in apply/pop subcommand. Ignoring the file list..."
                 )
 
+        self.cmd += f"{type(self).__name__.lower()} {self.command.value if self.command else ''} {' '.join(self.files) if not self.no_files else ''}"
+
     def construct(self):
         if not settings.stdout and not settings.output_only_path and not settings.quiet:
-            print(
-                f"{settings.INFO_STRING } {type(self).__name__.lower()} {self.command.value if self.command else ''} {' '.join(self.files) if not self.no_files else ''}"
-            )
+            print(f"{settings.INFO_STRING} {self.cmd}")
 
         self.show_intro()
         self.parse_commits()
         self.recenter_frame()
         self.scale_frame()
         self.vsplit_frame()
         self.setup_and_draw_zones(
             first_column_name="Working directory",
             second_column_name="Staging area",
             third_column_name="Stashed changes",
         )
+        self.show_command_as_title()
         self.fadeout()
         self.show_outro()
 
     def create_zone_text(
         self,
         firstColumnFileNames,
         secondColumnFileNames,
@@ -82,15 +89,15 @@
         thirdColumnTitle,
         horizontal2,
     ):
         for i, f in enumerate(firstColumnFileNames):
             text = (
                 m.Text(
                     self.trim_path(f),
-                    font="Monospace",
+                    font=self.font,
                     font_size=24,
                     color=self.fontColor,
                 )
                 .move_to(
                     (firstColumnTitle.get_center()[0], horizontal2.get_center()[1], 0)
                 )
                 .shift(m.DOWN * 0.5 * (i + 1))
@@ -98,15 +105,15 @@
             firstColumnFiles.add(text)
             firstColumnFilesDict[f] = text
 
         for j, f in enumerate(secondColumnFileNames):
             text = (
                 m.Text(
                     self.trim_path(f),
-                    font="Monospace",
+                    font=self.font,
                     font_size=24,
                     color=self.fontColor,
                 )
                 .move_to(
                     (secondColumnTitle.get_center()[0], horizontal2.get_center()[1], 0)
                 )
                 .shift(m.DOWN * 0.5 * (j + 1))
@@ -120,15 +127,15 @@
                     "<span strikethrough='true' strikethrough_color='"
                     + self.fontColor
                     + "'>"
                     + self.trim_path(f)
                     + "</span>"
                     if self.command == StashSubCommand.POP
                     else self.trim_path(f),
-                    font="Monospace",
+                    font=self.font,
                     font_size=24,
                     color=self.fontColor,
                 )
                 .move_to(
                     (thirdColumnTitle.get_center()[0], horizontal2.get_center()[1], 0)
                 )
                 .shift(m.DOWN * 0.5 * (h + 1))
@@ -142,27 +149,31 @@
         secondColumnFileNames,
         thirdColumnFileNames,
         firstColumnArrowMap={},
         secondColumnArrowMap={},
         thirdColumnArrowMap={},
     ):
         if self.command in [StashSubCommand.POP, StashSubCommand.APPLY]:
-            for x in self.repo.index.diff(None):
-                thirdColumnFileNames.add(x.a_path)
-                firstColumnFileNames.add(x.a_path)
-                thirdColumnArrowMap[x.a_path] = m.Arrow(
-                    stroke_width=3, color=self.fontColor
+            try:
+                stashedFileNames = self.repo.git.stash(
+                    "show", "--name-only", self.stash_index
                 )
-
-            for y in self.repo.index.diff("HEAD"):
-                firstColumnFileNames.add(y.a_path)
-                thirdColumnFileNames.add(y.a_path)
-                thirdColumnArrowMap[y.a_path] = m.Arrow(
-                    stroke_width=3, color=self.fontColor
+                stashedFileNames = stashedFileNames.split("\n")
+            except:
+                print(
+                    f"git-sim error: No stash entry with index {self.stashIndex} exists in stash"
                 )
+                sys.exit()
+            for s in stashedFileNames:
+                thirdColumnFileNames.add(s)
+                firstColumnFileNames.add(s)
+                thirdColumnArrowMap[s] = m.Arrow(stroke_width=3, color=self.fontColor)
+                firstColumnFileNames.add(s)
+                thirdColumnFileNames.add(s)
+                thirdColumnArrowMap[s] = m.Arrow(stroke_width=3, color=self.fontColor)
 
         else:
             for x in self.repo.index.diff(None):
                 firstColumnFileNames.add(x.a_path)
                 for file in self.files:
                     if file == x.a_path:
                         thirdColumnFileNames.add(x.a_path)
@@ -174,7 +185,18 @@
                 secondColumnFileNames.add(y.a_path)
                 for file in self.files:
                     if file == y.a_path:
                         thirdColumnFileNames.add(y.a_path)
                         secondColumnArrowMap[y.a_path] = m.Arrow(
                             stroke_width=3, color=self.fontColor
                         )
+
+    def parse_stash_format(self, s):
+        # Regular expression to match either a plain integer or stash@{integer}
+        match = re.match(r"^(?:stash@\{(\d+)\}|\b(\d+)\b)$", s)
+        if match:
+            # match.group(1) is the integer in the stash@{integer} format
+            # match.group(2) is the integer if it's just a plain number
+            # One of these groups will be None, the other will have our number as a string
+            number_str = match.group(1) or match.group(2)
+            return int(number_str)
+        return None
```

### Comparing `git-sim-0.3.3/git_sim/status.py` & `git_sim-0.3.4/src/git_sim/status.py`

 * *Files 26% similar despite different names*

```diff
@@ -7,19 +7,21 @@
         super().__init__()
         try:
             self.selected_branches.append(self.repo.active_branch.name)
         except TypeError:
             pass
         settings.hide_merged_branches = True
         self.n = self.n_default
+        self.cmd += f"{type(self).__name__.lower()}"
 
     def construct(self):
         if not settings.stdout and not settings.output_only_path and not settings.quiet:
-            print(f"{settings.INFO_STRING } {type(self).__name__.lower()}")
+            print(f"{settings.INFO_STRING} {self.cmd}")
         self.show_intro()
         self.parse_commits()
         self.recenter_frame()
         self.scale_frame()
         self.vsplit_frame()
         self.setup_and_draw_zones()
+        self.show_command_as_title()
         self.fadeout()
         self.show_outro()
```

### Comparing `git-sim-0.3.3/git_sim/switch.py` & `git_sim-0.3.4/src/git_sim/switch.py`

 * *Files 23% similar despite different names*

```diff
@@ -6,69 +6,88 @@
 import numpy
 
 from git_sim.git_sim_base_command import GitSimBaseCommand
 from git_sim.settings import settings
 
 
 class Switch(GitSimBaseCommand):
-    def __init__(self, branch: str, c: bool):
+    def __init__(self, branch: str, c: bool, detach: bool):
         super().__init__()
         self.branch = branch
         self.c = c
+        self.detach = detach
 
         if self.c:
             if self.branch in self.repo.heads:
                 print(
                     "git-sim error: can't create new branch '"
                     + self.branch
                     + "', it already exists"
                 )
                 sys.exit(1)
+            if detach:
+                print("git-sim error: can't use both '-c' and '--detach' flags")
+                sys.exit(1)
         else:
             try:
                 git.repo.fun.rev_parse(self.repo, self.branch)
             except git.exc.BadName:
                 print(
                     "git-sim error: '"
                     + self.branch
                     + "' is not a valid Git ref or identifier."
                 )
                 sys.exit(1)
 
-            if self.branch == self.repo.active_branch.name:
+            if (
+                not self.repo.head.is_detached
+                and self.branch == self.repo.active_branch.name
+            ):
                 print("git-sim error: already on branch '" + self.branch + "'")
                 sys.exit(1)
 
+            if not self.detach:
+                if self.branch not in self.repo.heads:
+                    print("git-sim error: include --detach to allow detached HEAD")
+                    sys.exit(1)
+
             self.is_ancestor = False
             self.is_descendant = False
 
             # branch being switched to is behind HEAD
-            if self.repo.active_branch.name in self.repo.git.branch(
-                "--contains", self.branch
-            ):
+            branch_names = self.repo.git.branch("--contains", self.branch)
+            branch_names = branch_names.split("\n")
+            for i, bn in enumerate(branch_names):
+                branch_names[i] = bn.strip("*").strip()
+            branch_hexshas = [
+                self.repo.branches[branch].commit.hexsha for branch in branch_names
+            ]
+            if self.repo.head.commit.hexsha in branch_hexshas:
                 self.is_ancestor = True
+
             # HEAD is behind branch being switched to
             elif self.branch in self.repo.git.branch(
-                "--contains", self.repo.active_branch.name
+                "--contains", self.repo.head.commit.hexsha
             ):
                 self.is_descendant = True
 
         if self.branch in [branch.name for branch in self.repo.heads]:
             self.selected_branches.append(self.branch)
 
         try:
-            self.selected_branches.append(self.repo.active_branch.name)
+            if not self.repo.head.is_detached:
+                self.selected_branches.append(self.repo.active_branch.name)
         except TypeError:
             pass
 
+        self.cmd += f"{type(self).__name__.lower()}{' -c' if self.c else ''}{' --detach' if self.detach else ''} {self.branch}"
+
     def construct(self):
         if not settings.stdout and not settings.output_only_path and not settings.quiet:
-            print(
-                f"{settings.INFO_STRING } {type(self).__name__.lower()}{' -c' if self.c else ''} {self.branch}"
-            )
+            print(f"{settings.INFO_STRING} {self.cmd}")
 
         self.show_intro()
         head_commit = self.get_commit()
 
         # using -c flag, create new branch label and exit
         if self.c:
             self.parse_commits(head_commit)
@@ -100,22 +119,24 @@
             elif self.is_descendant:
                 self.parse_commits(branch_commit)
                 reset_head_to = branch_commit.hexsha
                 self.recenter_frame()
                 self.scale_frame()
                 if "HEAD" in self.drawnRefs:
                     self.reset_head(reset_head_to)
-                    self.reset_branch(head_commit.hexsha)
+                    if not self.repo.head.is_detached:
+                        self.reset_branch(head_commit.hexsha)
                 else:
                     self.draw_ref(branch_commit, self.topref)
             else:
                 self.parse_commits(head_commit)
                 self.parse_commits(branch_commit, shift=4 * m.DOWN)
                 self.center_frame_on_commit(branch_commit)
                 self.recenter_frame()
                 self.scale_frame()
                 self.reset_head(branch_commit.hexsha)
                 self.reset_branch(head_commit.hexsha)
 
         self.color_by()
+        self.show_command_as_title()
         self.fadeout()
         self.show_outro()
```

### Comparing `git-sim-0.3.3/git_sim.egg-info/PKG-INFO` & `git_sim-0.3.4/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,24 +1,7 @@
-Metadata-Version: 2.1
-Name: git-sim
-Version: 0.3.3
-Summary: Simulate Git commands on your own repos by generating an image (default) or video visualization depicting the command's behavior.
-Home-page: https://initialcommit.com/tools/git-sim
-Author: Jacob Stopak
-Author-email: jacob@initialcommit.io
-Project-URL: Homepage, https://initialcommit.com/tools/git-sim
-Project-URL: Source, https://github.com/initialcommit-com/git-sim
-Keywords: git sim simulation simulate git-simulate git-simulation git-sim manim animation gitanimation image video dryrun dry-run
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.7
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 # git-sim
 ![git-sim-logo-with-tagline-1440x376p45](https://user-images.githubusercontent.com/49353917/232990611-58d0693f-69c0-45c8-b51d-cd540793d18c.gif)
 
 [![GitHub license](https://img.shields.io/github/license/initialcommit-com/git-sim)](https://github.com/initialcommit-com/git-sim/blob/main/LICENSE)
 [![GitHub tag](https://img.shields.io/github/v/release/initialcommit-com/git-sim)](https://img.shields.io/github/v/release/initialcommit-com/git-sim)
 [![Downloads](https://static.pepy.tech/badge/git-sim)](https://pepy.tech/project/git-sim)
 [![Contributors](https://img.shields.io/github/contributors/initialcommit-com/git-sim)](https://github.com/initialcommit-com/git-sim/graphs/contributors)
@@ -30,26 +13,33 @@
 
 Command syntax is based directly on Git's command-line syntax, so using git-sim is as familiar as possible.
 
 Example: `$ git-sim merge <branch>`
 <br/><br/>
 ![git-sim-merge_04-22-23_21-04-32_cropped](https://user-images.githubusercontent.com/49353917/233821875-a7bb640d-10be-4433-a8fb-bd25646eeff4.jpg)
 
+Check out the [git-sim release blog post](https://initialcommit.com/blog/git-sim) for the full scoop!
+
+## Support git-sim
+Git-Sim is Free and Open-Source Software (FOSS). Your support will help me work on it (and other Git projects) full time!
+- [Sponsor Git-Sim on GitHub](https://github.com/sponsors/initialcommit-com)
+- [Support Git-Sim via Patreon](https://patreon.com/user?u=92322459)
+
 ## Use cases
 - Visualize Git commands to understand their effects on your repo before actually running them
 - Prevent unexpected working directory and repository states by simulating before running
 - Share visualizations (jpg/png image or mp4/webm video) of your Git commands with your team, or the world
 - Save visualizations as a part of your team documentation to document workflow and prevent recurring issues
 - Create static Git diagrams (jpg/png) or dynamic animated videos (mp4/webm) to speed up content creation
 - Help visual learners understand how Git commands work
 - Combine with bundled command [git-dummy](https://github.com/initialcommit-com/git-dummy) to generate a dummy Git repo and then simulate operations on it
 
 ## Features
 - Run a one-liner git-sim command in the terminal to generate a custom Git command visualization (.jpg) from your repo
-- Supported commands: `log`, `status`, `add`, `restore`, `commit`, `stash`, `branch`, `tag`, `reset`, `revert`, `merge`, `rebase`, `cherry-pick`, `switch`, `checkout`, `fetch`, `pull`, `push`, `clone`, `rm`, `mv`, `clean`
+- Supported commands: `add`, `branch`, `checkout`, `cherry-pick`, `clean`, `clone`, `commit`, `config`, `fetch`, `init`, `log`, `merge`, `mv`, `pull`, `push`, `rebase`, `remote`, `reset`, `restore`, `revert`, `rm`, `stash`, `status`, `switch`, `tag`
 - Generate an animated video (.mp4) instead of a static image using the `--animate` flag (note: significant performance slowdown, it is recommended to use `--low-quality` to speed up testing and remove when ready to generate presentation-quality video)
 - Color commits by parameter, such as author with the `--color-by=author` option
 - Choose between dark mode (default) and light mode
 - Specify output formats of either jpg, png, mp4, or webm
 - Combine with bundled command [git-dummy](https://github.com/initialcommit-com/git-dummy) to generate a dummy Git repo and then simulate operations on it
 - Animation only: Add custom branded intro/outro sequences if desired
 - Animation only: Speed up or slow down animation speed as desired
@@ -141,15 +131,16 @@
 
 ## Requirements
 * Python 3.7 or greater
 * Pip (Package manager for Python)
 * [Manim (Community version)](https://www.manim.community/)
 
 ## Commands
-Basic usage is similar to Git itself - `git-sim` takes a familiar set of subcommands including "log", "status", "add", "restore", "commit", "stash", "branch", "tag", "reset", "revert", "merge", "rebase", "cherry-pick", "switch", "checkout", "fetch", "pull", "push", "clone", "rm", "mv", "clean" along with corresponding options.
+Basic usage is similar to Git itself - `git-sim` takes a familiar set of subcommands including "add", "branch", "checkout", "cherry-pick", "clean", "clone", "commit", "config", "fetch", "init", "log", "merge", "mv", "pull", "push", "rebase", "remote", "reset", "restore", "revert", "rm", "stash", "status", "switch", "tag" along with corresponding options.
+
 
 ```console
 $ git-sim [global options] <subcommand> [subcommand options]
 ```
 
 The `[global options]` apply to the overarching `git-sim` simulation itself, including:
 
@@ -176,159 +167,134 @@
 `--speed=n`: Set the multiple of animation speed of the output simulation, `n` can be an integer or float, default is 1.5.  
 `--low-quality`: Render the animation in low quality to speed up creation time, recommended for non-presentation use.  
 `--show-intro`: Add an intro sequence with custom logo and title.  
 `--show-outro`: Add an outro sequence with custom logo and text.  
 `--title=title`: Custom title to display at the beginning of the animation.  
 `--logo=logo.png`: The path to a custom logo to use in the animation intro/outro.  
 `--outro-top-text`: Custom text to display above the logo during the outro.  
-`--outro-bottom-text`: Custom text to display below the logo during the outro.
+`--outro-bottom-text`: Custom text to display below the logo during the outro.  
+`--font`: Font family used to display rendered text.
 
 The `[subcommand options]` are like regular Git options specific to the specified subcommand (see below for a full list).
 
 The following is a list of Git commands that can be simulated and their corresponding options/flags.
 
-### git log
-Usage: `git-sim log [-n <number>] [--all]`
-
-- Simulated output will show the most recent 5 commits on the active branch by default
-- Use `-n <number>` to set number of commits to display from each branch head
-- Set `--all` to display all local branches in the log output
-
-![git-sim-log_01-05-23_22-02-39](https://user-images.githubusercontent.com/49353917/210940300-aadd14c6-72ab-4529-a1be-b494ed5dd4c9.jpg)
-
-### git status
-Usage: `git-sim status`
-
-- Simulated output will show the state of the working directory, staging area, and untracked files
-- Note that simulated output will also show the most recent 5 commits on the active branch
-
-![git-sim-status_01-05-23_22-06-28](https://user-images.githubusercontent.com/49353917/210940685-735665e2-fa12-4043-979c-54c295b13800.jpg)
-
 ### git add
 Usage: `git-sim add <file 1> <file 2> ... <file n>`
 
 - Specify one or more `<file>` as a *modified* working directory file, or an untracked file
 - Simulated output will show files being moved to the staging area
 - Note that simulated output will also show the most recent 5 commits on the active branch
 
 ![git-sim-add_01-05-23_22-07-40](https://user-images.githubusercontent.com/49353917/210940814-7e8dc318-6116-4e56-b415-bc547401a56a.jpg)
 
-### git restore
-Usage: `git-sim restore <file 1> <file 2> ... <file n>`
+### git branch
+Usage: `git-sim branch <new branch name>`
 
-- Specify one or more `<file>` as a *modified* working directory file, or staged file
-- Simulated output will show files being moved back to the working directory or discarded changes
+- Specify `<new branch name>` as the name of the new branch to simulate creation of
+- Simulated output will show the newly create branch ref along with most recent 5 commits on the active branch
+
+![git-sim-branch_01-05-23_22-13-17](https://user-images.githubusercontent.com/49353917/210941509-2a42a7a4-2168-4f62-913f-3f6fe74a0684.jpg)
+
+### git checkout
+Usage: `git-sim checkout [-b] <branch>`
+
+- Checks out `<branch>` into the working directory, i.e. moves `HEAD` to the specified `<branch>`
+- The `-b` flag creates a new branch with the specified name `<branch>` and checks it out, assuming it doesn't already exist
+
+![git-sim-checkout_04-09-23_21-46-04](https://user-images.githubusercontent.com/49353917/230827836-e9f23a0e-2576-4716-b2fb-6327d3cf9b22.jpg)
+
+### git cherry-pick
+Usage: `git-sim cherry-pick <commit>`
+
+- Specify `<commit>` as a ref (branch name/tag) or commit ID to cherry-pick onto the active branch
+- Supports editing the cherry-picked commit message with: `$ git-sim cherry-pick <commit> -e "Edited commit message"`
+
+![git-sim-cherry-pick_01-05-23_22-23-08](https://user-images.githubusercontent.com/49353917/210942811-fa5155b1-4c6f-4afc-bea2-d39b4cd594aa.jpg)
+
+### git clean
+Usage: `git-sim clean`
+
+- Simulated output will show untracked files being deleted
+- Since this is just a simulation, no need to specify `-i`, `-n`, `-f` as in regular Git
 - Note that simulated output will also show the most recent 5 commits on the active branch
 
-![git-sim-restore_01-05-23_22-09-14](https://user-images.githubusercontent.com/49353917/210941009-e6bf7271-ce9b-4e41-9a0b-24cc4b8d3b15.jpg)
+![git-sim-clean_04-09-23_22-05-54](https://user-images.githubusercontent.com/49353917/230830043-779e7230-f439-461a-a408-b19b263e86e4.jpg)
+
+### git clone
+Usage: `git-sim clone <url>`
+
+- Clone the remote repo from `<url>` (web URL or filesystem path) to a new folder in the current directory
+- Output will report if clone operation is successful and show log of local clone
+
+![git-sim-clone_04-09-23_21-51-53](https://user-images.githubusercontent.com/49353917/230828521-80c8d2d1-2a31-46bb-aeed-746f0441c86e.jpg)
 
 ### git commit
 Usage: `git-sim commit -m "Commit message"`
 
 - Simulated output will show the new commit added to the tip of the active branch
 - Specify a commit message with the `-m` option
 - HEAD and the active branch will be moved to the new commit
 - Simulated output will show files in the staging area being included in the new commit
 - Supports amending the last commit with: `$ git-sim commit --amend -m "Amended commit message"`
 
 ![git-sim-commit_01-05-23_22-10-21](https://user-images.githubusercontent.com/49353917/210941149-d83677a1-3ab7-4880-bc0f-871b1f150087.jpg)
 
-### git stash
-Usage: `git-sim stash [push|pop|apply] <file>`
-
-- Specify one or more `<file>` as a *modified* working directory file, or staged file
-- If no `<file>` is specified, all available files will be included
-- Simulated output will show files being moved in/out of the Git stash
-- Note that simulated output will also show the most recent 5 commits on the active branch
-
-![git-sim-stash_01-05-23_22-11-18](https://user-images.githubusercontent.com/49353917/210941254-69c80b63-5c06-411a-a36a-1454b2906ee8.jpg)
+### git config
+Usage: `git-sim config [--list] <section.option> <value>`
 
-### git branch
-Usage: `git-sim branch <new branch name>`
-
-- Specify `<new branch name>` as the name of the new branch to simulate creation of
-- Simulated output will show the newly create branch ref along with most recent 5 commits on the active branch
+- Simulated output describes the specified configuration change
+- Use `--list` or `-l` to display all configuration
 
-![git-sim-branch_01-05-23_22-13-17](https://user-images.githubusercontent.com/49353917/210941509-2a42a7a4-2168-4f62-913f-3f6fe74a0684.jpg)
+![git-sim-config_04-16-24_08-34-34](https://github.com/initialcommit-com/git-sim/assets/49353917/c123e7a7-1fff-4f5c-b4a2-1e34ea2a4d80)
 
-### git tag
-Usage: `git-sim tag <new tag name>`
+### git fetch
+Usage: `git-sim fetch <remote> <branch>`
 
-- Specify `<new tag name>` as the name of the new tag to simulate creation of
-- Simulated output will show the newly create tag ref along with most recent 5 commits on the active branch
+- Fetches the specified `<branch>` from the specified `<remote>` to the local repo
 
-![git-sim-tag_01-05-23_22-14-18](https://user-images.githubusercontent.com/49353917/210941647-79376ff7-2941-42b3-964a-b1d3a404a4fe.jpg)
+![git-sim-fetch_04-09-23_21-47-59](https://user-images.githubusercontent.com/49353917/230828090-acae8979-4097-43a8-96ea-525890e0e0a8.jpg)
 
-### git reset
-Usage: `git-sim reset <reset-to> [--mixed|--soft|--hard]`
+### git init
+Usage: `git-sim init`
 
-- Specify `<reset-to>` as any commit id, branch name, tag, or other ref to simulate reset to from the current HEAD (default: `HEAD`)
-- As with a normal git reset command, default reset mode is `--mixed`, but can be specified using `--soft`, `--hard`, or `--mixed`
-- Simulated output will show branch/HEAD resets and resulting state of the working directory, staging area, and whether any file changes would be deleted by running the actual command
+- Simulated output describes the initialized `.git/` directory and it's contents
 
-![git-sim-reset_01-05-23_22-15-49](https://user-images.githubusercontent.com/49353917/210941835-80f032d2-4f06-4032-8dd0-98c8a2569049.jpg)
+![git-sim-init_04-16-24_08-34-47](https://github.com/initialcommit-com/git-sim/assets/49353917/2abb1a4a-3022-4353-a828-2d337baa8383)
 
-### git revert
-Usage: `git-sim revert <to-revert>`
+### git log
+Usage: `git-sim log [-n <number>] [--all]`
 
-- Specify `<to-revert>` as any commit id, branch name, tag, or other ref to simulate revert for
-- Simulated output will show the new commit which reverts the changes from `<to-revert>`
-- Simulated output will include the next 4 most recent commits on the active branch
+- Simulated output will show the most recent 5 commits on the active branch by default
+- Use `-n <number>` to set number of commits to display from each branch head
+- Set `--all` to display all local branches in the log output
 
-![git-sim-revert_01-05-23_22-16-59](https://user-images.githubusercontent.com/49353917/210941979-6db8b55c-2881-41d8-9e2e-6263b1dece13.jpg)
+![git-sim-log_01-05-23_22-02-39](https://user-images.githubusercontent.com/49353917/210940300-aadd14c6-72ab-4529-a1be-b494ed5dd4c9.jpg)
 
 ### git merge
 Usage: `git-sim merge <branch> [-m "Commit message"] [--no-ff]`
 
 - Specify `<branch>` as the branch name to merge into the active branch
 - If desired, specify a commit message with the `-m` option
 - Simulated output will depict a fast-forward merge if possible
 - Otherwise, a three-way merge will be depicted
 - To force a merge commit when a fast-forward is possible, use `--no-ff`
 - If merge fails due to merge conflicts, the conflicting files are displayed
 
 ![git-sim-merge_01-05-23_09-44-46](https://user-images.githubusercontent.com/49353917/210942030-c7229488-571a-4943-a1f4-c6e4a0c8ccf3.jpg)
 
-### git rebase
-Usage: `git-sim rebase <new-base>`
-
-- Specify `<new-base>` as the branch name to rebase the active branch onto
-
-![git-sim-rebase_01-05-23_09-53-34](https://user-images.githubusercontent.com/49353917/210942598-4ff8d1e6-464d-48f3-afb9-f46f7ec4828c.jpg)
-
-### git cherry-pick
-Usage: `git-sim cherry-pick <commit>`
-
-- Specify `<commit>` as a ref (branch name/tag) or commit ID to cherry-pick onto the active branch
-- Supports editing the cherry-picked commit message with: `$ git-sim cherry-pick <commit> -e "Edited commit message"`
-
-![git-sim-cherry-pick_01-05-23_22-23-08](https://user-images.githubusercontent.com/49353917/210942811-fa5155b1-4c6f-4afc-bea2-d39b4cd594aa.jpg)
-
-### git switch
-Usage: `git-sim switch [-c] <branch>`
-
-- Switches the checked-out branch to `<branch>`, i.e. moves `HEAD` to the specified `<branch>`
-- The `-c` flag creates a new branch with the specified name `<branch>` and switches to it, assuming it doesn't already exist
-
-![git-sim-switch_04-09-23_21-42-43](https://user-images.githubusercontent.com/49353917/230827783-a8740ace-b66f-4cac-b94e-5d101d27e0b5.jpg)
-
-### git checkout
-Usage: `git-sim checkout [-b] <branch>`
-
-- Checks out `<branch>` into the working directory, i.e. moves `HEAD` to the specified `<branch>`
-- The `-b` flag creates a new branch with the specified name `<branch>` and checks it out, assuming it doesn't already exist
-
-![git-sim-checkout_04-09-23_21-46-04](https://user-images.githubusercontent.com/49353917/230827836-e9f23a0e-2576-4716-b2fb-6327d3cf9b22.jpg)
-
-### git fetch
-Usage: `git-sim fetch <remote> <branch>`
+### git mv
+Usage: `git-sim mv <file> <new file>`
 
-- Fetches the specified `<branch>` from the specified `<remote>` to the local repo
+- Specify `<file>` as file to update name/path
+- Specify `<new file>` as new name/path of file 
+- Simulated output will show the name/path of the file being updated 
+- Note that simulated output will also show the most recent 5 commits on the active branch
 
-![git-sim-fetch_04-09-23_21-47-59](https://user-images.githubusercontent.com/49353917/230828090-acae8979-4097-43a8-96ea-525890e0e0a8.jpg)
+![git-sim-mv_04-09-23_22-05-13](https://user-images.githubusercontent.com/49353917/230829978-0a64dbe2-d974-4cef-9c6e-ed26e987342f.jpg)
 
 ### git pull
 Usage: `git-sim pull [<remote> <branch>]`
 
 - Pulls the specified `<branch>` from the specified `<remote>` to the local repo
 - If `<remote>` and `<branch>` are not specified, the active branch is pulled from the default remote
 - If merge conflicts occur, they are displayed in a table
@@ -340,49 +306,98 @@
 
 - Pushes the specified `<branch>` to the specified `<remote>` and displays the local result
 - If `<remote>` and `<branch>` are not specified, the active branch is pushed to the default remote
 - If the push fails due to remote changes that don't exist in the local repo, a message is included telling the user to pull first, along with color coding which commits need to be pulled
 
 ![git-sim-push_04-21-23_13-41-57](https://user-images.githubusercontent.com/49353917/233731005-51fd7887-ae14-4ceb-a5d5-e5aed79e9fd8.jpg)
 
-### git clone
-Usage: `git-sim clone <url>`
+### git rebase
+Usage: `git-sim rebase <new-base>`
 
-- Clone the remote repo from `<url>` (web URL or filesystem path) to a new folder in the current directory
-- Output will report if clone operation is successful and show log of local clone
+- Specify `<new-base>` as the branch name to rebase the active branch onto
 
-![git-sim-clone_04-09-23_21-51-53](https://user-images.githubusercontent.com/49353917/230828521-80c8d2d1-2a31-46bb-aeed-746f0441c86e.jpg)
+![git-sim-rebase_01-05-23_09-53-34](https://user-images.githubusercontent.com/49353917/210942598-4ff8d1e6-464d-48f3-afb9-f46f7ec4828c.jpg)
+
+### git remote
+Usage: `git-sim remote [add|rename|remove|get-url|set-url] [<remote>] [<url>]`
+
+- Simulated output will show remotes being added, renamed, removed, modified as indicated
+- Running `git-sim remote` with no options will list all existing remotes and their details  
+
+![git-sim-remote_04-16-24_08-40-37](https://github.com/initialcommit-com/git-sim/assets/49353917/ebaff04c-d5b6-4691-97b3-60bb502ba444)
+
+### git reset
+Usage: `git-sim reset <reset-to> [--mixed|--soft|--hard]`
+
+- Specify `<reset-to>` as any commit id, branch name, tag, or other ref to simulate reset to from the current HEAD (default: `HEAD`)
+- As with a normal git reset command, default reset mode is `--mixed`, but can be specified using `--soft`, `--hard`, or `--mixed`
+- Simulated output will show branch/HEAD resets and resulting state of the working directory, staging area, and whether any file changes would be deleted by running the actual command
+
+![git-sim-reset_01-05-23_22-15-49](https://user-images.githubusercontent.com/49353917/210941835-80f032d2-4f06-4032-8dd0-98c8a2569049.jpg)
+
+### git restore
+Usage: `git-sim restore <file 1> <file 2> ... <file n>`
+
+- Specify one or more `<file>` as a *modified* working directory file, or staged file
+- Simulated output will show files being moved back to the working directory or discarded changes
+- Note that simulated output will also show the most recent 5 commits on the active branch
+
+![git-sim-restore_01-05-23_22-09-14](https://user-images.githubusercontent.com/49353917/210941009-e6bf7271-ce9b-4e41-9a0b-24cc4b8d3b15.jpg)
+
+### git revert
+Usage: `git-sim revert <to-revert>`
+
+- Specify `<to-revert>` as any commit id, branch name, tag, or other ref to simulate revert for
+- Simulated output will show the new commit which reverts the changes from `<to-revert>`
+- Simulated output will include the next 4 most recent commits on the active branch
+
+![git-sim-revert_01-05-23_22-16-59](https://user-images.githubusercontent.com/49353917/210941979-6db8b55c-2881-41d8-9e2e-6263b1dece13.jpg)
 
 ### git rm
 Usage: `git-sim rm <file 1> <file 2> ... <file n>`
 
 - Specify one or more `<file>` as a *tracked* file
 - Simulated output will show files being removed from Git tracking
 - Note that simulated output will also show the most recent 5 commits on the active branch
 
 ![git-sim-rm_04-09-23_22-01-29](https://user-images.githubusercontent.com/49353917/230829899-f5d688ea-bc8e-46f9-a54a-55d251c8915d.jpg)
 
-### git mv
-Usage: `git-sim mv <file> <new file>`
+### git stash
+Usage: `git-sim stash [push|pop|apply] <file>`
 
-- Specify `<file>` as file to update name/path
-- Specify `<new file>` as new name/path of file 
-- Simulated output will show the name/path of the file being updated 
+- Specify one or more `<file>` as a *modified* working directory file, or staged file
+- If no `<file>` is specified, all available files will be included
+- Simulated output will show files being moved in/out of the Git stash
 - Note that simulated output will also show the most recent 5 commits on the active branch
 
-![git-sim-mv_04-09-23_22-05-13](https://user-images.githubusercontent.com/49353917/230829978-0a64dbe2-d974-4cef-9c6e-ed26e987342f.jpg)
+![git-sim-stash_01-05-23_22-11-18](https://user-images.githubusercontent.com/49353917/210941254-69c80b63-5c06-411a-a36a-1454b2906ee8.jpg)
 
-### git clean
-Usage: `git-sim clean`
+### git status
+Usage: `git-sim status`
 
-- Simulated output will show untracked files being deleted
-- Since this is just a simulation, no need to specify `-i`, `-n`, `-f` as in regular Git
+- Simulated output will show the state of the working directory, staging area, and untracked files
 - Note that simulated output will also show the most recent 5 commits on the active branch
 
-![git-sim-clean_04-09-23_22-05-54](https://user-images.githubusercontent.com/49353917/230830043-779e7230-f439-461a-a408-b19b263e86e4.jpg)
+![git-sim-status_01-05-23_22-06-28](https://user-images.githubusercontent.com/49353917/210940685-735665e2-fa12-4043-979c-54c295b13800.jpg)
+
+### git switch
+Usage: `git-sim switch [-c] <branch>`
+
+- Switches the checked-out branch to `<branch>`, i.e. moves `HEAD` to the specified `<branch>`
+- The `-c` flag creates a new branch with the specified name `<branch>` and switches to it, assuming it doesn't already exist
+
+![git-sim-switch_04-09-23_21-42-43](https://user-images.githubusercontent.com/49353917/230827783-a8740ace-b66f-4cac-b94e-5d101d27e0b5.jpg)
+
+### git tag
+Usage: `git-sim tag <new tag name>`
+
+- Specify `<new tag name>` as the name of the new tag to simulate creation of
+- Simulated output will show the newly create tag ref along with most recent 5 commits on the active branch
+
+![git-sim-tag_01-05-23_22-14-18](https://user-images.githubusercontent.com/49353917/210941647-79376ff7-2941-42b3-964a-b1d3a404a4fe.jpg)
 
 ## Video animation examples
 ```console
 $ git-sim --animate reset HEAD^
 ```
 
 https://user-images.githubusercontent.com/49353917/210943230-f38d879b-bb0d-4d42-a196-f24efb9e351a.mp4
```

