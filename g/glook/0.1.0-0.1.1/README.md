# Comparing `tmp/glook-0.1.0-py3-none-any.whl.zip` & `tmp/glook-0.1.1-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,14 +1,14 @@
-Zip file size: 16174 bytes, number of entries: 12
--rw-rw-rw-  2.0 fat     2776 b- defN 24-Apr-14 16:10 glook/GLook.py
+Zip file size: 16448 bytes, number of entries: 12
+-rw-rw-rw-  2.0 fat     3200 b- defN 24-Apr-16 17:28 glook/GLook.py
 -rw-rw-rw-  2.0 fat       51 b- defN 24-Mar-25 17:39 glook/__init__.py
 -rw-rw-rw-  2.0 fat      339 b- defN 24-Mar-25 18:24 glook/cli.py
 -rw-rw-rw-  2.0 fat     3698 b- defN 24-Apr-14 17:22 glook/pages/1_General_Data_Insights.py
 -rw-rw-rw-  2.0 fat    17728 b- defN 24-Apr-14 15:18 glook/pages/2_Univariate_Analysis.py
--rw-rw-rw-  2.0 fat     7771 b- defN 24-Apr-14 11:53 glook/pages/3_Bivariate_Analysis.py
--rw-rw-rw-  2.0 fat     7596 b- defN 24-Mar-28 17:23 glook/pages/4_Trivariate_Analysis.py
--rw-rw-rw-  2.0 fat     4078 b- defN 24-Apr-15 18:06 glook-0.1.0.dist-info/METADATA
--rw-rw-rw-  2.0 fat       92 b- defN 24-Apr-15 18:06 glook-0.1.0.dist-info/WHEEL
--rw-rw-rw-  2.0 fat       38 b- defN 24-Apr-15 18:05 glook-0.1.0.dist-info/entry_points.txt
--rw-rw-rw-  2.0 fat        6 b- defN 24-Apr-15 18:05 glook-0.1.0.dist-info/top_level.txt
--rw-rw-r--  2.0 fat      967 b- defN 24-Apr-15 18:06 glook-0.1.0.dist-info/RECORD
-12 files, 45140 bytes uncompressed, 14548 bytes compressed:  67.8%
+-rw-rw-rw-  2.0 fat     7813 b- defN 24-Apr-16 16:59 glook/pages/3_Bivariate_Analysis.py
+-rw-rw-rw-  2.0 fat     7647 b- defN 24-Apr-16 17:15 glook/pages/4_Trivariate_Analysis.py
+-rw-rw-rw-  2.0 fat     4053 b- defN 24-Apr-16 18:40 glook-0.1.1.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       92 b- defN 24-Apr-16 18:40 glook-0.1.1.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat       38 b- defN 24-Apr-16 18:40 glook-0.1.1.dist-info/entry_points.txt
+-rw-rw-rw-  2.0 fat        6 b- defN 24-Apr-16 18:40 glook-0.1.1.dist-info/top_level.txt
+-rw-rw-r--  2.0 fat      967 b- defN 24-Apr-16 18:40 glook-0.1.1.dist-info/RECORD
+12 files, 45632 bytes uncompressed, 14822 bytes compressed:  67.5%
```

## zipnote {}

```diff
@@ -15,23 +15,23 @@
 
 Filename: glook/pages/3_Bivariate_Analysis.py
 Comment: 
 
 Filename: glook/pages/4_Trivariate_Analysis.py
 Comment: 
 
-Filename: glook-0.1.0.dist-info/METADATA
+Filename: glook-0.1.1.dist-info/METADATA
 Comment: 
 
-Filename: glook-0.1.0.dist-info/WHEEL
+Filename: glook-0.1.1.dist-info/WHEEL
 Comment: 
 
-Filename: glook-0.1.0.dist-info/entry_points.txt
+Filename: glook-0.1.1.dist-info/entry_points.txt
 Comment: 
 
-Filename: glook-0.1.0.dist-info/top_level.txt
+Filename: glook-0.1.1.dist-info/top_level.txt
 Comment: 
 
-Filename: glook-0.1.0.dist-info/RECORD
+Filename: glook-0.1.1.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## glook/GLook.py

```diff
@@ -1,19 +1,31 @@
 # pip or conda to install openpyxl.
 # page 1
 import streamlit as st
 import pandas as pd
 import numpy as np
+st.set_page_config(
+	# page_title="ML-Automation", 
+	page_title="Auto - EDA", 
+	page_icon="👁️", 
+	layout="centered", 
+	initial_sidebar_state = "expanded",
+	menu_items={
+        'Get Help': 'https://github.com/gaurang157/glook/blob/main/README.md',
+        'Report a bug': "https://github.com/gaurang157/glook/issues",
+        'About': "# This is Auto EDA Library. This is an *extremely* cool app!"
+		}
+		)
 # import matplotlib.pyplot as plt
 # import matplotlib
 # matplotlib.use('TkAgg')
 if "shared" not in st.session_state:
 	st.session_state["shared"] = True
 
-st.title("G-Look Auto EDA")
+st.title("G-Look Auto EDA",)
 # st.write("`")
 gg = st.file_uploader("Input:", type=['csv', 'xlsx'])
 
 # df = None
 # if st.button("process", use_container_width=True):
 # 	try:
 # 		# Try reading as CSV
```

### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

## glook/pages/3_Bivariate_Analysis.py

```diff
@@ -164,15 +164,16 @@
     st.plotly_chart(fig)
     # Button to show the plot in full-screen mode
     if st.button("Show Full Screen"):
         fig.show()
     # Handle errors
 except Exception as e:
     st.error(e)
-    st.subheader("⚠️Please upload a file⚠️")
+    # st.subheader("⚠️Please upload a file⚠️")
+    st.warning("Select Proper Column")
 
 
 
 
 
 
 # Exclude non-numeric columns
```

## glook/pages/4_Trivariate_Analysis.py

```diff
@@ -199,13 +199,14 @@
         group_labels = ['X-Axis Column', 'Y-Axis Column', 'Z-Axis Column']
         fig = ff.create_distplot(hist_data, group_labels, bin_size=[.1, .25, .5])
         st.plotly_chart(fig, use_container_width=True)
 
 
 
     # Button to show the plot in full-screen mode
-    if st.button("Show Full Screen"):
+    if st.button("Show Full Screen in New Tab"):
         fig.show()
 
     
 except Exception as e:
+    st.warning("Select Proper Column")
     st.error(e)
```

## Comparing `glook-0.1.0.dist-info/METADATA` & `glook-0.1.1.dist-info/METADATA`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: glook
-Version: 0.1.0
+Version: 0.1.1
 Summary: Auto EDA.
 Home-page: https://github.com/gaurang157/glook
 Author: Gaurang Ingle
 Author-email: gaurang.ingle@gmail.com
 Maintainer: Gaurang Ingle, Sharat Chandra Manikonda
-Maintainer-email: gaurang.ingle@gmail.com, manikondasharat@gmail.com
+Maintainer-email: manikondasharat@gmail.com
 License: MIT
 Project-URL: Bug Reports, https://github.com/gaurang157/glook/issues
 Project-URL: Source, https://github.com/gaurang157/glook
 Project-URL: Documentation, https://github.com/gaurang157/glook/blob/main/README.md
 Project-URL: Say Thanks!, https://github.com/gaurang157/glook/issues/new?assignees=&labels=&template=thanks.yml
 Keywords: AutoEDA,Exploratory Data Analysis,Data Visualization,GUI,CLI,Python,Streamlit,CLI interface,UI interface
 Classifier: Programming Language :: Python :: 3
```

## Comparing `glook-0.1.0.dist-info/RECORD` & `glook-0.1.1.dist-info/RECORD`

 * *Files 19% similar despite different names*

```diff
@@ -1,12 +1,12 @@
-glook/GLook.py,sha256=8ppiVKtPyvA29zKzbQMNHzsM37EltchjN70XrB4AcvA,2776
+glook/GLook.py,sha256=qNCnTY0f4myhVXkZHf1mMgpN4yfHCaVXq4uz4uC85_s,3200
 glook/__init__.py,sha256=8NahmY4XQHJYMnFDvkZnHpjVBHwxrYrnDFlTTuyXbB0,51
 glook/cli.py,sha256=zBVCZyNNyRj_Zy4Tdnbrb1TrgRhEqAEEdZbk_vrLmi4,339
 glook/pages/1_General_Data_Insights.py,sha256=btHs2krtxH-H2MdX_x0hLnp8NR38dYvNnVdnNNjZosc,3698
 glook/pages/2_Univariate_Analysis.py,sha256=iQd1MsSFCdtIFU6coQBN-T9FWTVoVUA_Baf1evwjanA,17728
-glook/pages/3_Bivariate_Analysis.py,sha256=0fyPduQDUnlrfYk48YTV3JkxCaTxBjZANfzfPZMjllg,7771
-glook/pages/4_Trivariate_Analysis.py,sha256=Fhkmzqur1xBLPBviyI8kQeeFQbQYAhKwsOLw4E83Hs8,7596
-glook-0.1.0.dist-info/METADATA,sha256=F02QKdI8Q5kUturEubi2tjmP6_pRjwVRK9gA_2rZMhE,4078
-glook-0.1.0.dist-info/WHEEL,sha256=yQN5g4mg4AybRjkgi-9yy4iQEFibGQmlz78Pik5Or-A,92
-glook-0.1.0.dist-info/entry_points.txt,sha256=7q8WVzTgIl4vX4wJgctmfdJckoB5yPtI0p3hqAQSiFA,38
-glook-0.1.0.dist-info/top_level.txt,sha256=2wtpfrIqw9VT_LFDxpI77DArLrUaNjWxyClToM3P9WE,6
-glook-0.1.0.dist-info/RECORD,,
+glook/pages/3_Bivariate_Analysis.py,sha256=_eUSH35csf_Uljg9HvW7szmfXjrgNwrsVJA0gLMDNEA,7813
+glook/pages/4_Trivariate_Analysis.py,sha256=VPttBFaeegQUdCWH2OodwmX0Vn4B-4bnaLAKZErTgog,7647
+glook-0.1.1.dist-info/METADATA,sha256=ysJbUgPEpqfB8kCfB21NtQRtv0R86rTqpTuMuw7J2Ns,4053
+glook-0.1.1.dist-info/WHEEL,sha256=yQN5g4mg4AybRjkgi-9yy4iQEFibGQmlz78Pik5Or-A,92
+glook-0.1.1.dist-info/entry_points.txt,sha256=7q8WVzTgIl4vX4wJgctmfdJckoB5yPtI0p3hqAQSiFA,38
+glook-0.1.1.dist-info/top_level.txt,sha256=2wtpfrIqw9VT_LFDxpI77DArLrUaNjWxyClToM3P9WE,6
+glook-0.1.1.dist-info/RECORD,,
```

