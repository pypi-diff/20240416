# Comparing `tmp/dataverse-1.0.6.dev0-py3-none-any.whl.zip` & `tmp/dataverse-1.0.6.dev1-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,8 +1,8 @@
-Zip file size: 88235 bytes, number of entries: 75
+Zip file size: 88283 bytes, number of entries: 75
 -rw-r--r--  2.0 unx        0 b- defN 24-Mar-06 12:20 dataverse/__init__.py
 -rw-r--r--  2.0 unx        0 b- defN 24-Mar-06 12:20 dataverse/api/__init__.py
 -rw-r--r--  2.0 unx      413 b- defN 24-Mar-06 12:20 dataverse/api/cli.py
 -rw-r--r--  2.0 unx     1350 b- defN 24-Mar-06 12:20 dataverse/api/emr.py
 -rw-r--r--  2.0 unx       30 b- defN 24-Mar-06 12:20 dataverse/config/__init__.py
 -rw-r--r--  2.0 unx     8394 b- defN 24-Apr-16 17:08 dataverse/config/interface.py
 -rw-r--r--  2.0 unx      133 b- defN 24-Mar-06 12:20 dataverse/etl/__init__.py
@@ -62,16 +62,16 @@
 -rw-r--r--  2.0 unx     1036 b- defN 24-Mar-06 12:20 dataverse/utils/analyze/python.py
 -rw-r--r--  2.0 unx     1603 b- defN 24-Mar-06 12:20 dataverse/utils/api/__init__.py
 -rw-r--r--  2.0 unx    68144 b- defN 24-Apr-04 11:07 dataverse/utils/api/aws.py
 -rw-r--r--  2.0 unx      151 b- defN 24-Mar-06 12:20 dataverse/utils/format/__init__.py
 -rw-r--r--  2.0 unx     3319 b- defN 24-Apr-01 01:17 dataverse/utils/format/huggingface.py
 -rw-r--r--  2.0 unx      144 b- defN 24-Mar-06 12:20 dataverse/utils/format/ufl.py
 -rw-r--r--  2.0 unx      110 b- defN 24-Mar-06 12:20 dataverse/utils/setting/__init__.py
--rw-r--r--  2.0 unx     7852 b- defN 24-Apr-16 17:04 dataverse/utils/setting/system.py
+-rw-r--r--  2.0 unx     8081 b- defN 24-Apr-16 17:27 dataverse/utils/setting/system.py
 -rw-r--r--  2.0 unx     6019 b- defN 24-Mar-06 12:20 dataverse/utils/setting/user.py
--rw-r--r--  2.0 unx    11357 b- defN 24-Apr-16 17:11 dataverse-1.0.6.dev0.dist-info/LICENSE
--rw-r--r--  2.0 unx      730 b- defN 24-Apr-16 17:11 dataverse-1.0.6.dev0.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 24-Apr-16 17:11 dataverse-1.0.6.dev0.dist-info/WHEEL
--rw-r--r--  2.0 unx       53 b- defN 24-Apr-16 17:11 dataverse-1.0.6.dev0.dist-info/entry_points.txt
--rw-r--r--  2.0 unx       10 b- defN 24-Apr-16 17:11 dataverse-1.0.6.dev0.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx     6644 b- defN 24-Apr-16 17:11 dataverse-1.0.6.dev0.dist-info/RECORD
-75 files, 259086 bytes uncompressed, 77535 bytes compressed:  70.1%
+-rw-r--r--  2.0 unx    11357 b- defN 24-Apr-16 17:29 dataverse-1.0.6.dev1.dist-info/LICENSE
+-rw-r--r--  2.0 unx      726 b- defN 24-Apr-16 17:29 dataverse-1.0.6.dev1.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 24-Apr-16 17:29 dataverse-1.0.6.dev1.dist-info/WHEEL
+-rw-r--r--  2.0 unx       53 b- defN 24-Apr-16 17:29 dataverse-1.0.6.dev1.dist-info/entry_points.txt
+-rw-r--r--  2.0 unx       10 b- defN 24-Apr-16 17:29 dataverse-1.0.6.dev1.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx     6644 b- defN 24-Apr-16 17:29 dataverse-1.0.6.dev1.dist-info/RECORD
+75 files, 259311 bytes uncompressed, 77583 bytes compressed:  70.1%
```

## zipnote {}

```diff
@@ -201,26 +201,26 @@
 
 Filename: dataverse/utils/setting/system.py
 Comment: 
 
 Filename: dataverse/utils/setting/user.py
 Comment: 
 
-Filename: dataverse-1.0.6.dev0.dist-info/LICENSE
+Filename: dataverse-1.0.6.dev1.dist-info/LICENSE
 Comment: 
 
-Filename: dataverse-1.0.6.dev0.dist-info/METADATA
+Filename: dataverse-1.0.6.dev1.dist-info/METADATA
 Comment: 
 
-Filename: dataverse-1.0.6.dev0.dist-info/WHEEL
+Filename: dataverse-1.0.6.dev1.dist-info/WHEEL
 Comment: 
 
-Filename: dataverse-1.0.6.dev0.dist-info/entry_points.txt
+Filename: dataverse-1.0.6.dev1.dist-info/entry_points.txt
 Comment: 
 
-Filename: dataverse-1.0.6.dev0.dist-info/top_level.txt
+Filename: dataverse-1.0.6.dev1.dist-info/top_level.txt
 Comment: 
 
-Filename: dataverse-1.0.6.dev0.dist-info/RECORD
+Filename: dataverse-1.0.6.dev1.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## dataverse/utils/setting/system.py

```diff
@@ -98,16 +98,18 @@
 
         # if there is no relevant bucket, create one
         bucket = f'dataverse-{self.MAGIC_NUMBER}-{uuid.uuid1()}'
         aws_s3_create_bucket(bucket)
 
         return bucket
 
-    def _default_setting(self, default_value, given_value=None):
-        return default_value if given_value is None else given_value
+    def _default_setting(self, name, default_value, given_value=None):
+        result = default_value if given_value is None else given_value
+        self.system_setting[name] = result
+        return result
     
     def default_setting(self):
         """
         Reset the system setting to default
 
         Default setting:
         - `MAGIC_NUMBER`: magic number for dataverse
@@ -119,34 +121,35 @@
         """
         self.system_setting = {}
 
         # MAGIC NUMBER
         # dv - Dataverse
         # 42 - (The Hitchhiker's Guide to the Galaxy)
         #      The Answer to the Ultimate Question of Life, the Universe, and Everything
-        self.MAGIC_NUMBER = self._default_setting("dv42", self.MAGIC_NUMBER)
+        self.MAGIC_NUMBER = self._default_setting("MAGIC_NUMBER", "dv42", self.MAGIC_NUMBER)
 
         # DATAVERSE
-        self.DATAVERSE_HOME = self._default_setting(os.path.dirname(dataverse.__file__), self.DATAVERSE_HOME)
+        self.DATAVERSE_HOME = self._default_setting("DATAVERSE_HOME", os.path.dirname(dataverse.__file__), self.DATAVERSE_HOME)
 
         # HARD CODED DEFAULT SETTING
-        self.CACHE_DIR = self._default_setting(Path.home().as_posix(), self.CACHE_DIR)
-        self.IS_CLI = self._default_setting(False, self.IS_CLI)
+        self.CACHE_DIR = self._default_setting("CACHE_DIR", Path.home().as_posix(), self.CACHE_DIR)
+        self.IS_CLI = self._default_setting("IS_CLI", False, self.IS_CLI)
 
         # AWS SETTING
-        self.AWS_BUCKET = self._default_setting(self._get_aws_bucket(), self.AWS_BUCKET)
+        self.AWS_BUCKET = self._default_setting("AWS_BUCKET", self._get_aws_bucket(), self.AWS_BUCKET)
 
         # SPARK VERSION
-        self.SPARK_VERSION = self._default_setting(pyspark.__version__, self.SPARK_VERSION)
+        self.SPARK_VERSION = self._default_setting("SPARK_VERSION", pyspark.__version__, self.SPARK_VERSION)
 
         # HADOOP VERSION
         if not self.HADOOP_VERSION:
             jars = Path(pyspark.__file__).parent / "jars"
             hadoop_jar = list(jars.glob("hadoop-client-runtime*.jar"))
             self.HADOOP_VERSION = re.findall(r"\d+\.\d+\.\d+", hadoop_jar[0].name)[-1]
+        self.system_setting["HADOOP_VERSION"] = self.HADOOP_VERSION
 
         # TODO: add more default setting here
         ...
 
     def update_by_env(self):
         """
         Update the system setting by env variable
```

## Comparing `dataverse-1.0.6.dev0.dist-info/LICENSE` & `dataverse-1.0.6.dev1.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `dataverse-1.0.6.dev0.dist-info/METADATA` & `dataverse-1.0.6.dev1.dist-info/METADATA`

 * *Files 2% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 Metadata-Version: 2.1
 Name: dataverse
-Version: 1.0.6.dev0
+Version: 1.0.6.dev1
 Summary: An open-source simplifies ETL workflow with Python based on Spark
 Author: Dataverse Team
 Author-email: dataverse@upstage.ai
 License: Apache License 2.0
 License-File: LICENSE
 Requires-Dist: requests
 Requires-Dist: numpy
 Requires-Dist: pandas
 Requires-Dist: fasttext-wheel
 Requires-Dist: omegaconf
-Requires-Dist: pyarrow (==14.0.1)
+Requires-Dist: pyarrow ==14.0.1
 Requires-Dist: datasets
 Requires-Dist: pyspark
 Requires-Dist: scipy
 Requires-Dist: trafilatura
 Requires-Dist: html2text
 Requires-Dist: faker
 Requires-Dist: awscli
 Requires-Dist: boto3
-Requires-Dist: pre-commit (==3.6.0)
+Requires-Dist: pre-commit ==3.6.0
 Requires-Dist: botocore
 Requires-Dist: rsa
 Requires-Dist: s3transfer
 Requires-Dist: isort
 Requires-Dist: pytest
```

## Comparing `dataverse-1.0.6.dev0.dist-info/RECORD` & `dataverse-1.0.6.dev1.dist-info/RECORD`

 * *Files 2% similar despite different names*

```diff
@@ -61,15 +61,15 @@
 dataverse/utils/analyze/python.py,sha256=nchHNEbl-Iqm23VhICYLUnJJDUxCp6FjNTOP2HiPv1w,1036
 dataverse/utils/api/__init__.py,sha256=pgAJdND7egHR1gWshxXPqJgNjq5w0j5-Rk5Sjp-j4Ws,1603
 dataverse/utils/api/aws.py,sha256=e9SEtzfvMtuu3AnOVty3c5wGJlqbAlAWTrTcI0eK7nQ,68144
 dataverse/utils/format/__init__.py,sha256=kPoH1GQBG_nvIHtxtjRVqQJWt2x40W5OEcbQq22R6pU,151
 dataverse/utils/format/huggingface.py,sha256=sqfXx_6cM0OHSD0Ldx0j0I0uRWY1bSCPLfTsBBavopg,3319
 dataverse/utils/format/ufl.py,sha256=fIBYyV5Rue-kkBHLSO8h4rRhi01G_B7jPU0HZpZb5_s,144
 dataverse/utils/setting/__init__.py,sha256=v7-MJJgJgK3c9IZ6V-TfJKjjrMffxhpKKjmwzIWgAQ0,110
-dataverse/utils/setting/system.py,sha256=yl3ErLxffUH1_EWfoP_HfrkSK_ha6BDYLEZqGaFpPUM,7852
+dataverse/utils/setting/system.py,sha256=tlh1Wu3DFkOE5aWK8AAvWg4Z9Dih72BMmY0QHAYhDHs,8081
 dataverse/utils/setting/user.py,sha256=TJfVJbAgeViMxvNgH-1Xt-5fRCmxRzLWLe1MQRnprjI,6019
-dataverse-1.0.6.dev0.dist-info/LICENSE,sha256=xx0jnfkXJvxRnG63LTGOxlggYnIysveWIZ6H3PNdCrQ,11357
-dataverse-1.0.6.dev0.dist-info/METADATA,sha256=EM8h5J3mh-FGbIexpynD-YLCpGtHHQLERAoXYDROq48,730
-dataverse-1.0.6.dev0.dist-info/WHEEL,sha256=2wepM1nk4DS4eFpYrW1TTqPcoGNfHhhO_i5m4cOimbo,92
-dataverse-1.0.6.dev0.dist-info/entry_points.txt,sha256=2JG3fmkHIRftHHC4pKRQb9TT0cl8jKkjwzw-6I03hqw,53
-dataverse-1.0.6.dev0.dist-info/top_level.txt,sha256=DQthQD-a7flZ1h_SzQ_2X0ZD9T4hl_K8UW43H1y_t6k,10
-dataverse-1.0.6.dev0.dist-info/RECORD,,
+dataverse-1.0.6.dev1.dist-info/LICENSE,sha256=xx0jnfkXJvxRnG63LTGOxlggYnIysveWIZ6H3PNdCrQ,11357
+dataverse-1.0.6.dev1.dist-info/METADATA,sha256=pnsBB8e6A7gxY2GrQRRPR92KPCZ5uN2mtMNmc9NGoLA,726
+dataverse-1.0.6.dev1.dist-info/WHEEL,sha256=yQN5g4mg4AybRjkgi-9yy4iQEFibGQmlz78Pik5Or-A,92
+dataverse-1.0.6.dev1.dist-info/entry_points.txt,sha256=2JG3fmkHIRftHHC4pKRQb9TT0cl8jKkjwzw-6I03hqw,53
+dataverse-1.0.6.dev1.dist-info/top_level.txt,sha256=DQthQD-a7flZ1h_SzQ_2X0ZD9T4hl_K8UW43H1y_t6k,10
+dataverse-1.0.6.dev1.dist-info/RECORD,,
```

