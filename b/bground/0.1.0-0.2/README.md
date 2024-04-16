# Comparing `tmp/bground-0.1.0.tar.gz` & `tmp/bground-0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bground-0.1.0.tar", last modified: Sat Jun  3 22:08:10 2023, max compression
+gzip compressed data, was "bground-0.2.tar", last modified: Tue Apr 16 20:24:46 2024, max compression
```

## Comparing `bground-0.1.0.tar` & `bground-0.2.tar`

### file list

```diff
@@ -1,19 +1,20 @@
-drwxrwxrwx   0        0        0        0 2023-06-03 22:08:10.805137 bground-0.1.0/
--rw-rw-rw-   0        0        0     1093 2021-12-06 08:05:53.000000 bground-0.1.0/LICENCE
--rw-rw-rw-   0        0        0     1438 2023-06-03 22:08:10.803614 bground-0.1.0/PKG-INFO
--rw-rw-rw-   0        0        0      894 2023-06-03 22:03:35.000000 bground-0.1.0/README.md
--rw-rw-rw-   0        0        0      108 2021-08-03 08:03:10.000000 bground-0.1.0/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-06-03 22:08:10.805137 bground-0.1.0/setup.cfg
--rw-rw-rw-   0        0        0     1266 2022-09-13 06:31:08.000000 bground-0.1.0/setup.py
-drwxrwxrwx   0        0        0        0 2023-06-03 22:08:10.725491 bground-0.1.0/src/
-drwxrwxrwx   0        0        0        0 2023-06-03 22:08:10.792494 bground-0.1.0/src/bground/
--rw-rw-rw-   0        0        0      646 2023-05-31 07:50:35.000000 bground-0.1.0/src/bground/__init__.py
--rw-rw-rw-   0        0        0     4189 2023-05-28 16:35:34.000000 bground-0.1.0/src/bground/bdata.py
--rw-rw-rw-   0        0        0     4036 2023-05-30 17:11:54.000000 bground-0.1.0/src/bground/bfunc.py
--rw-rw-rw-   0        0        0    14413 2023-05-31 08:20:46.000000 bground-0.1.0/src/bground/iplot.py
--rw-rw-rw-   0        0        0     2746 2023-05-31 09:18:16.000000 bground-0.1.0/src/bground/ui.py
-drwxrwxrwx   0        0        0        0 2023-06-03 22:08:10.801119 bground-0.1.0/src/bground.egg-info/
--rw-rw-rw-   0        0        0     1438 2023-06-03 22:08:10.000000 bground-0.1.0/src/bground.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      286 2023-06-03 22:08:10.000000 bground-0.1.0/src/bground.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-03 22:08:10.000000 bground-0.1.0/src/bground.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        8 2023-06-03 22:08:10.000000 bground-0.1.0/src/bground.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-16 20:24:46.647208 bground-0.2/
+-rw-rw-rw-   0        0        0     1093 2021-12-06 08:05:54.000000 bground-0.2/LICENCE
+-rw-rw-rw-   0        0        0     2239 2024-04-16 20:24:46.633200 bground-0.2/PKG-INFO
+-rw-rw-rw-   0        0        0     1697 2024-04-16 20:08:17.000000 bground-0.2/README.md
+-rw-rw-rw-   0        0        0      108 2021-08-03 08:03:10.000000 bground-0.2/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-04-16 20:24:46.647208 bground-0.2/setup.cfg
+-rw-rw-rw-   0        0        0     1266 2022-09-13 06:31:08.000000 bground-0.2/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-16 20:24:46.633200 bground-0.2/src/
+drwxrwxrwx   0        0        0        0 2024-04-16 20:24:46.633200 bground-0.2/src/bground/
+-rw-rw-rw-   0        0        0      742 2024-04-15 16:26:10.000000 bground-0.2/src/bground/__init__.py
+-rw-rw-rw-   0        0        0     4224 2024-04-15 16:32:26.000000 bground-0.2/src/bground/bdata.py
+-rw-rw-rw-   0        0        0     4607 2024-04-15 16:33:50.000000 bground-0.2/src/bground/bfunc.py
+-rw-rw-rw-   0        0        0     4208 2024-04-16 15:43:46.000000 bground-0.2/src/bground/help.py
+-rw-rw-rw-   0        0        0    16954 2024-04-16 13:30:52.000000 bground-0.2/src/bground/iplot.py
+-rw-rw-rw-   0        0        0    20341 2024-04-16 12:15:06.000000 bground-0.2/src/bground/ui.py
+drwxrwxrwx   0        0        0        0 2024-04-16 20:24:46.633200 bground-0.2/src/bground.egg-info/
+-rw-rw-rw-   0        0        0     2239 2024-04-16 20:24:46.000000 bground-0.2/src/bground.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      306 2024-04-16 20:24:46.000000 bground-0.2/src/bground.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-16 20:24:46.000000 bground-0.2/src/bground.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        8 2024-04-16 20:24:46.000000 bground-0.2/src/bground.egg-info/top_level.txt
```

### Comparing `bground-0.1.0/LICENCE` & `bground-0.2/LICENCE`

 * *Files identical despite different names*

### Comparing `bground-0.1.0/PKG-INFO` & `bground-0.2/README.md`

 * *Files 22% similar despite different names*

```diff
@@ -1,39 +1,40 @@
-Metadata-Version: 2.1
-Name: bground
-Version: 0.1.0
-Summary: Interactive subtraction of background from XY-data
-Home-page: https://github.com/mirekslouf/bground/
-Author: Mirek Slouf
-Author-email: mirek.slouf@gmail.com
-License: MIT
-Project-URL: Documentation, https://mirekslouf.github.io/bground/
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.6
-Description-Content-Type: text/markdown
-License-File: LICENCE
-
-BGROUND :: interactive background subtraction
----------------------------------------------
-
-* BGROUND draws an interactive plot of XY-data.
-* The user can define and subtract backgound using mouse and keyboard.
-* XY-data is an arbitrary text file containing two columns: [X-data, Y-data].
+BGROUND :: semi-automated background subtraction
+------------------------------------------------
+
+* BGROUND performs semi-automated correction of background in XY-data.
+	- XY-data = usually a file with two columns - (X-data,Y-data)
+* How does it work?
+	- BGROUND reads XY-data and shows them in an interactive plot
+	- The user defines background points and backround types
+	- BGROUND does the rest (background calculation and subtraction)
+
+Installation
+------------
+* Requirement: Python with sci-modules: numpy, matplotlib, scipy, pandas
+* `pip install bground` = standard installation, no other packages needed
+
+Quick start
+-----------
+* Look at the
+  [worked example](https://www.dropbox.com/scl/fi/59og19il0qel4ajmg1io7/01_bground.nb.pdf?rlkey=aqdxrgn9jtaoounihiv2zhw7q&dl=0)
+  to see how BGROUND works.
+* Download
+  [complete examples with data](https://www.dropbox.com/scl/fo/08ougjp96dnwr1wqqm7be/AIStLY7i0yb80Yq3xKn1blw?rlkey=806nl015x93qte85feldycsxu&dl=0)
+  and try BGROUND yourself.
 
 Documentation, help and examples
 --------------------------------
 
 * [PyPI](https://pypi.org/project/bground) repository.
-* [GitHub](https://mirekslouf.github.io/bground) repository.
+* [GitHub](https://github.com/mirekslouf/bground) repository.
 * [GitHub Pages](https://mirekslouf.github.io/bground/)
   with [documentation](https://mirekslouf.github.io/bground/docs).
 
 Versions of BGROUND
 -------------------
 
 * Version 0.0.1 = an incomplete testing version
 * Version 0.0.2 = the basic algorithm works
 * Version 0.0.3 = a small improvement of code and docstrings
-* Version 0.1.0 = better arrangement of funcs in modules + semi-complete docs
-
+* Version 0.1 = OO-interface, better arrangement of funcs + semi-complete docs
+* Version 0.2 = improved OO-implementation + better UI (commands, saving, help)
```

### Comparing `bground-0.1.0/setup.py` & `bground-0.2/setup.py`

 * *Files identical despite different names*

### Comparing `bground-0.1.0/src/bground/bdata.py` & `bground-0.2/src/bground/bdata.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 '''
-Module bground.bdata
---------------------
+Module: bground.bdata
+---------------------
 The module defines three simple clasess.
 The classes keep data for definition of background.
 
 1. Class XYpoints = coordinates of the user-defined bakground points.
 2. Class XYcurve = two numpy arrays defining the whole calculated bkg curve.
 3. Class bkg = user defined background, containing
     - XYpoints object = the user-defined coordinates of bkg point
@@ -80,37 +80,38 @@
         Returns
         -------
         None.
         '''
         self.X = X
         self.Y = Y
 
-class bkg:
+class XYbackground:
     '''
     User-defined background.
     '''
     
     def __init__(self, basename, 
                  points = XYpoints([],[]), 
                  curve = XYcurve([],[]),
-                 itype = 'linear'):
+                 btype = 'linear'):
         '''
         Initialize background.
 
         Parameters
         ----------
         basename : str
             Basename of output file = filename without extension.
             The extension will be added automatically according to context.
         points : bdata.XYpoints object
             Coordinates of user-defined backround points.
         curve  : bdata.XYcurve object
             Backround curve = X,Y of all points of the calculated background.
-        itype : string; default is 'linear' 
-            Interpolation type = interpolation during backround calculation.
+        btype : string; default is 'linear' 
+            Background interpolation type
+            = interpolation during backround calculation.
             Implemented interpolation types: 'linear', 'quadratic', 'cubic'.
             
         Returns
         -------
         None; the result is the initialized object: bdata.bkg.
         
         Technical notes
@@ -122,8 +123,8 @@
           and the background in the main program must be initialized
           with empty objects XYpoints and XYcurve as well.
         * At the moment, I regard this as a Python mystery.
         '''
         self.basename = basename
         self.points   = points
         self.curve    = curve 
-        self.itype    = itype
+        self.btype    = btype
```

### Comparing `bground-0.1.0/src/bground/bfunc.py` & `bground-0.2/src/bground/bfunc.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,33 +1,46 @@
 '''
-Module bground.bfunc
---------------------
+Module: bground.bfunc
+---------------------
 Functions for background calculation.
 
-* The functions are usually called from bground.iplot module.
-* The bground.iplot module defines interactive plot and its events.
+* The functions are usually called by functions in bground.iplot module.
+* The bground.iplot module defines an interactive plot = the user interface.
 * This module defines functions that perform the real background calculation.
+
+Technical notes:
+
+* All functions in this module manipulate with bground.bdata.bkg object.
+    - The bkg object contains all info needed for background subtraction.
+* The last function works also with data = 2D-numpy array object.
+    - The 2D-numpy array = a 2-row array: [X,Y] => Y should be bkgr-corrected.
+    - The last function calculates a 3-row array: [X,Y,background-corrected-Y].
 '''
 
 import numpy as np
 from scipy import interpolate
+import matplotlib.pyplot as plt
+
 
 def sort_bkg_points(bkg):
     '''
     Sort background points according to their X-coordinate.
-    The background points are inserted as the whole bkg object.
     
     Parameters
     ----------
     bkg : bground.bdata.bkg object
-        A bkg object containing unsorted list of background points.
+        A bkg object containing (among other things)
+        an unsorted list of background points.
 
     Returns
     -------
-    None; the output is bkg object with sorted background points.
+    None
+        The result is the updated bkg object.
+        The updated object contains bkg.points sorted according to
+        their X-coordinate.
     '''
     # Sorting is based on the trick found on www
     # GoogleSearch: python sort two 1D arrays
     # https://stackoverflow.com/q/9007877
     X,Y = (bkg.points.X, bkg.points.Y)
     x,y = zip( *sorted( zip(X,Y) ) )
     bkg.points.X = list(x)
@@ -39,32 +52,35 @@
     = calculate interpolated background curve;
     the calculated background curve is saved within bkg object.
     
     Parameters
     ----------
     bkg : bground.bdata.bkg object
         Object containing the following items:
-            * basename = string, basename of output file(s)
-            * points = 3-column list: [PointType, X-coord, Y-coord]
-            * itype = type of interpolation for the calculation of bkground
+            
+        * basename = string, basename of output file(s)
+        * points = 3-column list: [PointType, X-coord, Y-coord]
+        * btype = a type of interpolation for the calculation of the bkground
     
     Returns
     -------
-    None; the result is the updated bkg object.
-        * bkg.X = calculated X-coordinates of the WHOLE background
+    None
+        The result is the updated bkg object.
+        
+        * bkg.X = calculated X-coordinates of the whole background
         * bkg.Y = calculated Y-coordinates of the WHOLE background
     '''
     # (1) Prepare background points = X,Y coordinates for interpolation
     X,Y = (bkg.points.X,bkg.points.Y)
     # (2) Interpolate background points = calculcate background curve
     try:
         # Interpolation = calculation of interpolation function F.
         # (F = interpolation object/function
         # (with which we easily calculate the interpolated data - see below
-        F = interpolate.interp1d(X,Y, kind=bkg.itype)
+        F = interpolate.interp1d(X,Y, kind=bkg.btype)
         Xmin = bkg.points.X[0]
         Xmax = bkg.points.X[-1]
         Xnew = data[0,(Xmin<=data[0])&(data[0]<=Xmax)]
         Ynew = F(Xnew)
         bkg.curve.X = Xnew
         bkg.curve.Y = Ynew
     except Exception as err:
@@ -105,7 +121,14 @@
     # (5) Subtract background from intensities between Xmin and Xmax
     data[2,bkg_range] = data[2,bkg_range] - bkg.curve.Y
     # (6) Set possible negative intensities after bkgr subtraction to zero
     data[2,data[2]<0] = 0
     # (7) Return modified data array
     # (the last column the array contains background-corrected intensities
     return(data)
+
+    
+    
+    
+    
+    
+
```

### Comparing `bground-0.1.0/src/bground/iplot.py` & `bground-0.2/src/bground/iplot.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,336 +1,397 @@
 '''
-Module bground.iplot
---------------------
-The module defines functions that can create an interactive plot.
-
-* The interactive plot is defined at two levels.
-* Level 1 = a general interactive plot = a plot linked with keypress events.
-* Level 2 = specific functions for the individual keypress events.
-* We define just keypress events, while mouse events = matplotlib defaults.
-* The default matplotlib mouse events are very good - no reason to change them.
+Module: bground.iplot
+---------------------
+The module defines functions that create an interactive plot.
+
+The interactive plot can be defined at three levels:
+    
+* Level 1 = function yielding the interactive plot = a plot linked with events.
+* Level 2 = functions for event types (key_press_event, close_event, etc.).
+* Level 3 = functions for individual events (such as specific keypress events).
+
+Simplifications and limitations:
+
+* We keep the (very reasonable) mouse events from Matplotlib UI.
+* We define *key_press_events*, by means of which we can do the whole job.
+* We can define additional simple events (here: *close_event* = on closing).
 '''
 
 import numpy as np
 import pandas as pd
 import matplotlib.pyplot as plt
 
 from bground import bdata, bfunc
 import warnings; warnings.filterwarnings("ignore")
 
-# Level 1: Define interactive plot -------------------------------------------- 
+# =============================================================================
+# Level 1: Create plot with events
 
-def create_plot(data, xlabel, ylabel='Intensity', xlim=[0,300], ylim=[0,300]):
+def interactive_plot(data, bkgr, ppar):
     '''
     Create plot from input data.
     
     This is a plot window, which will be made interactive later.
     In the rest of the program, the plot will be the program interface.
 
     Parameters
     ----------
     data : 2D numpy array
         Data for plotting; columns [X,Y].
-    xlabel : str
-        Label of X-axis.
-    ylabel : str, default is 'Intensity'
-        Label of Y-axis.
-    xlim : list or tuple (containing two values)
-        Lower and upper limit of X in the plot; the default is [0,300].
-    ylim : list or tuple (containing two values)
-        Lower and upper limit of Y in the plot; the default is [0,300].
+    bkgr : bground.bdata.XYbackground object
+        An object storing data for the background calculation.
+    ppar : bground.ui.PlotParameters object
+        An object with data for interactive plot + name of output file
     
     Returns
     -------
-    plt : maptplotlib.pyplot object
-        The line plot showing XY data.
+    fig,ax : maptplotlib.pyplot objects
+        The figure and axis of the interactive plot which shows XY-data.
+        
+    Technical notes
+    ---------------
+    The arguments/objects for this function (data, bkgr, ppar)
+    are usually defined by means of a simple OO-interface
+    before this function is called.
     '''
-    # Step 1 in defining an interactive plot
-    # = preparation of a standard plot, which will be made interactive later
-    initialize_plot_parameters()
-    X,Y = (data[0],data[1])
-    plt.gcf().canvas.set_window_title('Background definition')
-    plt.plot(X,Y, 'b-')
-    plt.xlim(xlim)
-    plt.ylim(ylim)
-    plt.xlabel(xlabel)
-    plt.ylabel(ylabel)
-    plt.tight_layout()
-    return(plt)
+    
+    # (0) Initialize
+    plt.close('all')  # Close all previous plots - to avoid mess in Jupyter
+    initialize_interactive_plot_parameters()
+    
+    # (1) Prepare the plot: fig,ax including window title
+    # (num argument below can take both integers and strings
+    fig,ax = plt.subplots(num='Background correction')
 
-def define_key_bindings(plt, data, bkgr, outfile):
-    '''
-    Define key bindings for plot = link plot with a callback function,
-    which links selected [keypress_events] with further functions.
+    # (2) Read XY data and create the plot
+    # Get XY data from the function argument data
+    X,Y = (data[0],data[1])
+    # Plot XY data
+    ax.plot(X,Y, 'b-')
+    # Set the remaining plot parameters
+    ax.set_xlim(ppar.xlim)
+    ax.set_ylim(ppar.ylim)
+    ax.set_xlabel(ppar.xlabel)
+    ax.set_ylabel(ppar.ylabel)
     
-    Parameters
-    ----------
-    plt : matplotlib.pyplot object
-        Prepared interactive XY-plot,
-        for which we want to define new [key_press_events].
-    data : 2D numpy array
-        XY-data (which are shown in plt),
-        which must be sent to functions after some [key_press_events].
-    bkgr : bdata.bkg object
-        Empty background object,
-        which must be sent to functions after some [key_press_events].
-    outfile : string
-        Name of the output file,
-        which must be sent to functions after some [key_press_events].
+    # (3) Connect the plot with event(s)
+    #   => link fig.canvas event(s) to a callback function(s).
+    # Here: two types of events:
+    #   key_press_event -> callback function = on_keypress.
+    #   close_event     -> callback function = on_close
+    # The callback function links the events to further user-defind funcs.
+    #   Note1: all is based on standard matplotlib function canvas.mpl_connect
+    #   Note2: the individual functions are defined below.
+    # Trick: If we need an event with multiple arguments => lambda functions.
+    #   GoogleSearch: python calback with multiple arguments 
     
-    Returns
-    -------
-    plt : maptplotlib.pyplot object
-        The line plot showing XY data with defined key-bindings.
-    '''
-    # Step 2 in defining interactive plot
-    # = link plt to a callback function (here: on_keypress),
-    #   which links selected [keypress_events] to further functions. 
-    # * Note1: all is based on standard matplotlib function canvas.mpl_connect
-    # * Note2: the individual functions are defined below in on_keypress func.
-    # ! Trick: we need an event with multiple arguments => lambda function
-    plt.gcf().canvas.mpl_connect('key_press_event',
-        lambda event: on_keypress(event, plt, data, bkgr, outfile))
-    # return plt object, in which key bindings were defined
-    return(plt)
+    # (3a) Connect plot with key_press_event (= when a key is pressed)
+    fig.canvas.mpl_connect('key_press_event',
+        lambda event: on_keypress(event, fig, ax, data, bkgr, ppar))
+    
+    # (3b) Connect plot with close_event (= when the window is closed)
+    fig.canvas.mpl_connect('close_event',
+        lambda event: on_close(event, ppar))
+    
+    # (4) Optimize the plot layout
+    plt.tight_layout()
+    
+    # (5) Return fig,ax
+    # (This is necessary, among others, fof Jupyter + %matplotlib widget
+    return(fig,ax)
 
-def on_keypress(event, plt, data, bkg, outfile):
+
+# =============================================================================
+# Level 2: Callback functions for all events
+
+def on_keypress(event, fig, ax, data, bkgr, ppar):
     '''
-    Definition of events for a plot.
-    Master callback procedure, which defines all keypress events.
+    Definition of key_press_events for a plot.
+    
+    The callback function, which defines all keypress events.
+    The functions for the individual keypress events are defined below.
     '''
     # Step 3 in defining interactive plot
     # = defining individual functions for specific pressed keys.
     # -----
     # Read pressed key and mouse coordinates
     key = event.key
     xm,ym = event.xdata,event.ydata
     # Mouse outside graph area - just print warning!
     if xm == None or ym == None:
-        print(f'Pressed {key:s}, mouse outside plot area - no action!')
+        if ppar.messages:
+            print(f'Key [{key}] mouse outside plot area - no action!')
     # Mouse inside graph area, run corresponding function.
     else:
-        print(f'Pressed {key:s}, mouse coordinates {xm:.2f},{ym:2f}.')
+        if ppar.messages:
+            print(f'Key [{key:s}] mouse [{xm:.1f},{ym:.1f}]', end=' ')
         # Functions run by means try-except
         # Reason: to ignore nonsense actions...
         # ...such as delete/draw points if no points are defined
         try:
-            if   key == '0': print_help(outfile)
-            elif key == '1': add_bkg_point(plt,data,bkg,xm,ym)
-            elif key == '2': delete_bkg_point(plt,bkg)
-            elif key == '3': delete_bkg_point_close_to_mouse(plt,bkg,xm,ym)
-            elif key == '4': replot_with_bkg_points(plt,data,bkg)
-            elif key == '5': replot_with_bkg(plt,data,bkg,'linear')
-            elif key == '6': replot_with_bkg(plt,data,bkg,'quadratic')
-            elif key == '7': replot_with_bkg(plt,data,bkg,'cubic')
-            elif key == 'a': print_bkg_points(bkg)
-            elif key == 'b': save_bkg_points(bkg)
-            elif key == 'c': load_bkg_points(plt,data,bkg)
-            elif key == 't': subtract_bkg_and_save(plt, outfile, data, bkg)
+            if   key == '1': add_bkg_point(plt,data,bkgr,ppar,xm,ym)
+            elif key == '2': del_bkg_point_close_to_mouse(plt,bkgr,ppar,xm,ym)
+            elif key == '3': replot_with_bkg_points(plt,data,bkgr,ppar)
+            elif key == '4': replot_with_bkg(plt,data,bkgr,ppar,'linear')
+            elif key == '5': replot_with_bkg(plt,data,bkgr,ppar,'quadratic')
+            elif key == '6': replot_with_bkg(plt,data,bkgr,ppar,'cubic')
+            elif key == 'a': load_bkg_points(plt,data,bkgr,ppar)
+            elif key == 'b': save_bkg_points(bkgr,ppar)
+            elif key == 't': subtract_bkg_and_save(plt, data, bkgr, ppar)
+            elif key == 's': save_PNG_image(ppar) 
+            elif ppar.messages: print() # for any other key just empty line
         except Exception:
             pass
 
-# Auxiliary functions (to Level 1 = defining ineractive plot) .................
 
-def initialize_plot_parameters():
+def on_close(event, ppar):
     '''
-    Initialize parameters for plotting.
-    '''
-    plt.rcParams.update({
-        'figure.figsize' : (6,4),
-        'figure.dpi' : 100,
-        'font.size' : 12})
+    Definition of on_close event of the plot.
+    
+    The simple callback function, which runs
+    when the interactive plot window is closed.
+    The function just prints some concluding remarks
+    and information about the output files.
+    '''
+    out_file1 = ppar.output_file
+    out_file2 = ppar.output_file + '.bkg'
+    out_file3 = ppar.output_file + '.png'
+    print()
+    print('The interactive plot was closed.')
+    print('If you followed the instructions on www,')
+    print('the outputs should be saved in the following files:')
+    print(f' - {out_file1} = TXT file with background-corrected XYdata')
+    print(f' - {out_file2} = BKG file containing background points')
+    print(f' - {out_file3} = PNG file showing the background')
 
-def print_ultrabrief_help():
-    '''
-    Print ultra-brief help in console window before activating the plot.
-    '''
-    print('Activate interactive plot window and press:')
-    print('0 = to print brief help in notebook/console window')
-    print('1 = to draw background point at current mouse position')
-    print('2 = to delete background point...')
-    print('---')
 
-# Level 2: Functions for individual events ------------------------------------
+# =============================================================================
+# Level 3: Functions for individual keypress events       
 
-def print_help(outfile):
-    '''
-    Function for pressed key = 0:
-    Print help for all pre-defined keys to console window.
+def add_bkg_point(plt, data, bkgr, ppar, xm, ym):
     '''
-    print()
-    print('==========================================================')
-    print('BGROUND :: Interactive background removal :: Brief help')
-    print('----------------------------------------------------------')
-    print('0 = print this help')
-    print('1 = add background point')
-    print('2 = delete background point - last one')
-    print('3 = delete background point - closest to mouse')
-    print('4 = re-draw plot with background points')
-    print('5 = re-draw plot with linear spline background')
-    print('6 = re-draw plot with quadratic spline background')
-    print('7 = re-draw plot with cubic spline background')
-    print('------')
-    print('a = background points :: print')
-    print('b = background points :: save to BKG-file') 
-    print('c = background points :: load from BKG-file')
-    print('(BKG-file = %s' % (outfile+'.bkg'))
-    print('------')
-    print('s = save current image as PNG (default matplotlib shortcut')
-    print('t = subtract current background & save data to TXT-file')
-    print('(TXT-file = %s' % outfile)
-    print('------')
-    print('All standard matplotlib tools and shortcuts work as well.')
-    print('See: https://matplotlib.org/stable/users/interactive.html')
-    print('===========================================================')
-       
-def add_bkg_point(plt, data, bkg, xm, ym):
-    '''
-    Function for pressed key = 1:
-    Add background point to at current mouse position.
-    More precisely: add background point at the XY-point,
+    Function for keypress = '1'.
+    
+    Add background point at current mouse position.
+    More precisely: add a background point at the the XY-curve,
     whose X-coordinate is the closest to the mouse X-coordinate.
     '''
     idx = find_nearest(data[0],xm)
     xm,ym = (data[0,idx],data[1,idx])
-    bkg.points.add_point(xm,ym)
+    bkgr.points.add_point(xm,ym)
     plt.plot(xm,ym,'r+')
     plt.draw()
+    if ppar.messages: print('background point added.')
     
-def delete_bkg_point(plt, bkg):
-    '''
-    Function for pressed key = 2:
-    Remove background point (the last inserted).
-    '''
-    xr = bkg.points.X.pop()
-    yr = bkg.points.Y.pop()
-    plt.plot(xr,yr, 'w+')
-    plt.draw()
 
-def delete_bkg_point_close_to_mouse(plt, bkg, xm, ym):
+def del_bkg_point_close_to_mouse(plt, bkgr, ppar, xm, ym):
     '''
-    Function for pressed key = 3:
-    Remove background point (the point closest to the mouse position).
-    More precisely: remove background point,
-    whose X-coordinate is the closest to the mouse X-coordinate.
+    Function for keypress = '2'.
     
+    Remove the background point close to mouse cursor position.
+    More precisely: remove the background point from the XY-curve,
+    whose X-coordinate is the closest to the mouse cursor X-coordinate.
     '''
     # a) Sort bkg points (sorted array is necessary for the next step)
-    bfunc.sort_bkg_points(bkg)
+    bfunc.sort_bkg_points(bkgr)
     # b) Find index of background point closest to the mouse X-position
-    idx = find_nearest(np.array(bkg.points.X), xm)
+    idx = find_nearest(np.array(bkgr.points.X), xm)
     # c) Remove element with given index from X,Y-lists (save coordinates)
-    xr = bkg.points.X.pop(idx)
-    yr = bkg.points.Y.pop(idx)
+    xr = bkgr.points.X.pop(idx)
+    yr = bkgr.points.Y.pop(idx)
     # d) Redraw removed element with background color
     plt.plot(xr,yr, 'w+')
     # e) Redraw plot
     plt.draw()
+    # f) Print message to stdout.
+    if ppar.messages: print('background point deleted.')
+
 
-def replot_with_bkg_points(plt, data, bkg):
+def replot_with_bkg_points(plt, data, bkgr, ppar, points_reloaded=False):
     '''
-    Function for pressed key = 4:
+    Function for keypress = '3'.
+    
     Re-draw plot with backround points.
+    Additional keyword parameter (points_reloaded=False),
+    is employed if the function is called from load_bkg_points function.
+    The load_bkg_points function uses its own short message
+    and sets points_reloaded=True to avoid additional confusing messaging.
     '''
     clear_plot()
     plt.plot(data[0],data[1],'b-')
-    plt.plot(bkg.points.X,bkg.points.Y,'r+')
+    plt.plot(bkgr.points.X,bkgr.points.Y,'r+')
     plt.draw()
+    if ppar.messages == True and points_reloaded == False:
+        # 
+        print('backround points re-drawn.')
 
-def replot_with_bkg(plt, data, bkg, itype):
+def replot_with_bkg(plt, data, bkgr, ppar, btype):
     '''
-    Function for pressed keys = 5,6,7:
+    Function for keypress = '4,5,6'.
+    
     Re-draw plot with backround points and background curve.
-    * Type of the curve is given by parameter itype.
-    * For key = 5/6/7. the function called with itype = linear/quadratic/cubic.
+    Type of the curve is given by parameter btype.
+    For key = 4/5/6 the function called with btype = linear/quadratic/cubic.
     '''
-    bfunc.sort_bkg_points(bkg)
-    bkg.itype = itype
-    bfunc.calculate_background(data, bkg)
+    # Sort background points + calculate background
+    bfunc.sort_bkg_points(bkgr)
+    bkgr.btype = btype
+    bfunc.calculate_background(data, bkgr)
+    # Clear plot + re-draw it with the background points
     clear_plot()
     plt.plot(data[0],data[1],'b-')
-    plt.plot(bkg.points.X,bkg.points.Y,'r+')
-    plt.plot(bkg.curve.X,bkg.curve.Y,'r:')
+    plt.plot(bkgr.points.X,bkgr.points.Y,'r+')
+    plt.plot(bkgr.curve.X,bkgr.curve.Y,'r:')
     plt.draw()
-    
-def subtract_bkg_and_save(plt, outfile, data, bkg):
-    '''
-    Function for pressed key = 8:
-    This is the final function which:
-        a) Recalculates recently defined background
-        b) Calculates background-corrected data = subtracts bkg from data
-        c) Saves the results to output file = TXT with 3 cols [X,Int,CInt]
-    '''
-    print('Subtract recently defined background and save results.')
-    print('a) Recalculating background...')
-    bfunc.calculate_background(data,bkg)
-    print('b) Subtracting background...')
-    data = bfunc.subtract_background(data,bkg)
-    print('c) Saving background to TXT-file...')
-    np.savetxt(
-        outfile, np.transpose(data), fmt=('%8.3f','%11.3e','%11.3e'),
-        header='Columns: X, Intensity, Background-corrected intensity')
-    print('File with backround-corrected intensities saved:')
-    print('[%s]' % outfile)
-    print('-----')
-
-def print_bkg_points(bkg):
-    '''
-    Function for pressed key = a:
-    Print background points in the console window.
-    '''
-    bfunc.sort_bkg_points(bkg)
-    df = bkg_to_df(bkg)
-    print('Current background points:')
-    print(df.to_string())
-    print('-----')
-
-def save_bkg_points(bkg):
-    '''
-    Function for pressed key = b:
-    Save background points to file.
-    (basename of output file is saved in bkg.basename).
-    '''
-    bfunc.sort_bkg_points(bkg)
-    output_filename = bkg.basename + '.bkg'
-    df = bkg_to_df(bkg)
-    with open(output_filename, 'w') as f:
-        f.write(df.to_string())
-        print('Background points saved to:')
-        print('[%s]' % output_filename)
-        print('-----')
-
-def load_bkg_points(plt, data, bkg):
-    '''
-    Function for pressed key = c:
-    Load background points from previously saved file
-    (basename of input file with background points saved in bkg.basename).
+    # Print a brief message on stdout if requested
+    if ppar.messages:
+        if bkgr.btype == 'linear':
+            print('linear background displayed.')
+        elif bkgr.btype == 'quadratic':
+            print('quadratic background displayed.')
+        elif bkgr.btype == 'cubic':
+            print('cubic background displayed.')
+
+
+def load_bkg_points(plt, data, bkgr, ppar):
+    '''
+    Function for keypress = 'a'.
+
+    Load background points from previously saved file.
+    Assumption: the file has been saved with save_bkg_points function,
+    which means that its name is fixed and known (bkgr.basename + '.bkg').
     '''
     # a) get input file with previously saved background points
     # (the filename is fixed to [output_file_name].bkg
     # (reason: inserting a name during an interactive plot session is a hassle
     # (solution: manual renaming of the BKG-file before running this program
-    input_filename = bkg.basename + '.bkg'
+    input_filename = bkgr.basename + '.bkg'
     # b) read input file to DataFrame
     df = pd.read_csv(input_filename, sep='\s+')
-    print(df)
     # c) initialize bkg object by means of above-read DataFrame
-    bkg.points = bdata.XYpoints(X = list(df.X), Y = list(df.Y))
-    bkg.itype='linear'
-    # d) print message & replot with currently loaded background
-    print('Background points read from file:')
-    print('[%s]' % input_filename)
-    print('-----')
-    replot_with_bkg_points(plt, data, bkg)
+    bkgr.points = bdata.XYpoints(X = list(df.X), Y = list(df.Y))
+    bkgr.btype='linear'
+    # d) print message if requested
+    if ppar.messages:
+        print(f'background points read from: [{input_filename}].')
+    # e) replot with currently loaded background
+    replot_with_bkg_points(plt, data, bkgr, ppar, points_reloaded=True)
+
+
+def save_bkg_points(bkgr, ppar):
+    '''
+    Function for keypress = 'b'.
+    
+    Save background points to file.
+    The output file name is bkgr.basename + extension 'bkg'.
+    '''
+    bfunc.sort_bkg_points(bkgr)
+    output_filename = bkgr.basename + '.bkg'
+    df = bkg_to_df(bkgr)
+    with open(output_filename, 'w') as f:
+        f.write(df.to_string())
+        if ppar.messages:
+            print(f'background points saved to: [{output_filename}].')
+    
+
+def subtract_bkg_and_save(plt, data, bkgr, ppar):
+    '''
+    Function for keypress 't'.
+    
+    This is the final function which:
+    
+    * Recalculates recently defined background
+    * Calculates background-corrected data = subtracts bkg from data
+    * Saves the results to TXT-file with 3 cols [X, Y, bkg-corrected-Y]
+    '''
+    # Subtract recently defined background and save results
+    # (a) Recalculate background
+    bfunc.calculate_background(data,bkgr)
+    # (b) Subtract background
+    data = bfunc.subtract_background(data,bkgr)
+    # (c) Save background-corrected data to TXT-file
+    # (we will use ppar object properties for this
+    # (ppar.output_file = output file name, ppar.xlabel = label of X-data...
+    my_file_header = (
+        f'Columns: {ppar.xlabel}, {ppar.ylabel}, ' +
+        f'background-corrected-{ppar.ylabel}\n' +
+        f'Background correction type: {bkgr.btype}')
+    np.savetxt(
+        ppar.output_file, np.transpose(data), fmt=('%8.3f','%11.3e','%11.3e'),
+        header=my_file_header)
+    if ppar.messages:
+        print(f'backround-corrected data saved to: [{ppar.output_file}].')
+
+
+def save_PNG_image(ppar):
+    '''
+    Function for keypress 's'.
     
-# Auxiliary functions (to level 2 = individual events) ........................
+    Special case - 's' is Matplotlib UI shortcut,
+    which saves PNG image of the plot.
+    As key_press_event 's' was NOT disconnected from the plot (intentionally),
+    the following two things are going to happen:
+    
+    * At first, the default event (saving as PNG) will take place.
+    * At second, this function prints a message on stdout (if requested).
+    '''
+    if ppar.messages:
+        print('plot saved to PNG; recommended name:', end='')
+        print(f'[{ppar.output_file+".png"}].')
+
+
+# =============================================================================
+# Level 4: Auxiliary functions for the interactive plot
+
+
+def initialize_interactive_plot_parameters():
+    '''
+    Initialize parameters of the interactive plot.
+    '''
+    plt.rcParams.update({
+        'figure.figsize' : (6,4),
+        'figure.dpi' : 100,
+        'font.size' : 12,
+        'lines.linewidth' : 1.0})
+
+
+def print_brief_help(ppar):
+    '''
+    Print ultra-brief help before activating the interactive plot.
+    
+    Parameters
+    ----------
+    ppar : 
+        It is used just to get the value of ppar.messages.
+        If ppar.messages == True, additional empty line is printed.
+        Reason: To separate the introductory help from the following messages.
+    
+    Returns
+    -------
+    None
+        The output is the brief help printed on stdout.
+    '''
+    print('(0) Click on the newly-opened window {Background correction},')
+    print('    which is a Matplotlib interative figure with extra shortcuts.')
+    print('(1) Use Matplotlib UI + keyboard shortcuts to define a background:')
+    print('    1,2 = add/delete a background point close to the mouse cursor')
+    print('    3,4,5,6 = show bkg points + linear/quadratic/cubic background')
+    print('(2) Save the results + close the window when you are done:')
+    print('    b = save the background points as a BKG-file (a = restore)')
+    print('    t = subtract the background & save the result as a TXT-file')
+    print('(3) Detailed help, complete documentation, and worked examples:')
+    print('    https://mirekslouf.github.io/bground/docs')
+    # Add an extra empty line if short messages to stdoud should be printed.
+    if ppar.messages: print()
+
 
 def find_nearest(arr, value):
     '''
-    Find index of the element with nearest value in 1D-array.
+    Auxiliary function:
+    Find the index of the element with the nearest {value} in 1D-array.
     
     Parameters
     ----------
     arr : 1D numpy array
         The array, in which we search the element with closest value.
         Important prerequisite: the array must be sorted.
     value : float
@@ -349,34 +410,40 @@
     # 2) finalization = consider special cases and return final value
     if idx > 0 and (
             idx == len(arr) or abs(value-arr[idx-1]) < abs(value-arr[idx])):
         return(idx-1)
     else:
         return(idx)
 
+
 def clear_plot():
     '''
-    Auxilliary function: clear plot before re-drawing.
-    Note: the functions keeps current labels and XY-limits of the plot.
+    Auxilliary function: clear interactive plot before re-drawing.
+    
+    Key feature of the function:
+    It keeps current labels and XY-limits of the plot.
     '''
     my_xlabel = plt.gca().get_xlabel()
     my_ylabel = plt.gca().get_ylabel()
     my_xlim = plt.xlim()
     my_ylim = plt.ylim()
     plt.cla()
     plt.xlabel(my_xlabel)
     plt.ylabel(my_ylabel)
     plt.xlim(my_xlim)
     plt.ylim(my_ylim)
+    
 
-def bkg_to_df(bkg):
+def bkg_to_df(bkgr):
     '''
-    Convert current background points to dataframe.
-    Reason: df can be used to print/save background points nicely.
+    Auxiliary function: Convert current background points to dataframe.
+    
+    Why this function?
+    => df can be used to save/restore background points nicely.
     '''
     # Convert bkg to DataFrame to get nicely formated output
     # (our trick: df.to_string & then print/save to file as string
     # (more straightforward: df.to_csv('something.txt', sep='\t')
     # (BUT the output with to_string has better-aligned columns
     df = pd.DataFrame(
-        np.transpose([bkg.points.X, bkg.points.Y]), columns=['X','Y'])
+        np.transpose([bkgr.points.X, bkgr.points.Y]), columns=['X','Y'])
     return(df)
```

### Comparing `bground-0.1.0/src/bground.egg-info/PKG-INFO` & `bground-0.2/PKG-INFO`

 * *Files 25% similar despite different names*

```diff
@@ -1,39 +1,56 @@
 Metadata-Version: 2.1
 Name: bground
-Version: 0.1.0
+Version: 0.2
 Summary: Interactive subtraction of background from XY-data
 Home-page: https://github.com/mirekslouf/bground/
 Author: Mirek Slouf
 Author-email: mirek.slouf@gmail.com
 License: MIT
 Project-URL: Documentation, https://mirekslouf.github.io/bground/
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENCE
 
-BGROUND :: interactive background subtraction
----------------------------------------------
+BGROUND :: semi-automated background subtraction
+------------------------------------------------
 
-* BGROUND draws an interactive plot of XY-data.
-* The user can define and subtract backgound using mouse and keyboard.
-* XY-data is an arbitrary text file containing two columns: [X-data, Y-data].
+* BGROUND performs semi-automated correction of background in XY-data.
+	- XY-data = usually a file with two columns - (X-data,Y-data)
+* How does it work?
+	- BGROUND reads XY-data and shows them in an interactive plot
+	- The user defines background points and backround types
+	- BGROUND does the rest (background calculation and subtraction)
+
+Installation
+------------
+* Requirement: Python with sci-modules: numpy, matplotlib, scipy, pandas
+* `pip install bground` = standard installation, no other packages needed
+
+Quick start
+-----------
+* Look at the
+  [worked example](https://www.dropbox.com/scl/fi/59og19il0qel4ajmg1io7/01_bground.nb.pdf?rlkey=aqdxrgn9jtaoounihiv2zhw7q&dl=0)
+  to see how BGROUND works.
+* Download
+  [complete examples with data](https://www.dropbox.com/scl/fo/08ougjp96dnwr1wqqm7be/AIStLY7i0yb80Yq3xKn1blw?rlkey=806nl015x93qte85feldycsxu&dl=0)
+  and try BGROUND yourself.
 
 Documentation, help and examples
 --------------------------------
 
 * [PyPI](https://pypi.org/project/bground) repository.
-* [GitHub](https://mirekslouf.github.io/bground) repository.
+* [GitHub](https://github.com/mirekslouf/bground) repository.
 * [GitHub Pages](https://mirekslouf.github.io/bground/)
   with [documentation](https://mirekslouf.github.io/bground/docs).
 
 Versions of BGROUND
 -------------------
 
 * Version 0.0.1 = an incomplete testing version
 * Version 0.0.2 = the basic algorithm works
 * Version 0.0.3 = a small improvement of code and docstrings
-* Version 0.1.0 = better arrangement of funcs in modules + semi-complete docs
-
+* Version 0.1 = OO-interface, better arrangement of funcs + semi-complete docs
+* Version 0.2 = improved OO-implementation + better UI (commands, saving, help)
```

