# Comparing `tmp/europarser-0.1.7.tar.gz` & `tmp/europarser-0.1.8.tar.gz`

## Comparing `europarser-0.1.7.tar` & `europarser-0.1.8.tar`

### file list

```diff
@@ -1,43 +1,44 @@
--rw-r--r--   0        0        0       71 2020-02-02 00:00:00.000000 europarser-0.1.7/.dockerignore
--rw-r--r--   0        0        0     1416 2020-02-02 00:00:00.000000 europarser-0.1.7/Dockerfile
--rw-r--r--   0        0        0     2953 2020-02-02 00:00:00.000000 europarser-0.1.7/README_en.md
--rw-r--r--   0        0        0     1032 2020-02-02 00:00:00.000000 europarser-0.1.7/docker_log.conf
--rw-r--r--   0        0        0     1080 2020-02-02 00:00:00.000000 europarser-0.1.7/log.conf
--rw-r--r--   0        0        0     2365 2020-02-02 00:00:00.000000 europarser-0.1.7/pyinstaller.py
--rwxr-xr-x   0        0        0     2203 2020-02-02 00:00:00.000000 europarser-0.1.7/start_europarser.sh
--rw-r--r--   0        0        0     1376 2020-02-02 00:00:00.000000 europarser-0.1.7/.github/workflows/docker-publish.yml
--rw-r--r--   0        0        0     3536 2020-02-02 00:00:00.000000 europarser-0.1.7/.github/workflows/hatch-build-and-publish.yml
--rw-r--r--   0        0        0      135 2020-02-02 00:00:00.000000 europarser-0.1.7/src/europarser/__about__.py
--rw-r--r--   0        0        0      320 2020-02-02 00:00:00.000000 europarser-0.1.7/src/europarser/__init__.py
--rw-r--r--   0        0        0     2322 2020-02-02 00:00:00.000000 europarser-0.1.7/src/europarser/daniel_light.py
--rw-r--r--   0        0        0     2485 2020-02-02 00:00:00.000000 europarser-0.1.7/src/europarser/endpoint.py
--rw-r--r--   0        0        0       93 2020-02-02 00:00:00.000000 europarser-0.1.7/src/europarser/lang_detect.py
--rw-r--r--   0        0        0     1544 2020-02-02 00:00:00.000000 europarser-0.1.7/src/europarser/main.py
--rw-r--r--   0        0        0     2238 2020-02-02 00:00:00.000000 europarser-0.1.7/src/europarser/models.py
--rw-r--r--   0        0        0     2725 2020-02-02 00:00:00.000000 europarser-0.1.7/src/europarser/pipeline.py
--rw-r--r--   0        0        0     8705 2020-02-02 00:00:00.000000 europarser-0.1.7/src/europarser/pivot.py
--rw-r--r--   0        0        0    13243 2020-02-02 00:00:00.000000 europarser-0.1.7/src/europarser/utils.py
--rw-r--r--   0        0        0      153 2020-02-02 00:00:00.000000 europarser-0.1.7/src/europarser/api/__init__.py
--rw-r--r--   0        0        0     3888 2020-02-02 00:00:00.000000 europarser-0.1.7/src/europarser/api/api.py
--rw-r--r--   0        0        0      430 2020-02-02 00:00:00.000000 europarser-0.1.7/src/europarser/api/utils.py
--rw-r--r--   0        0        0      750 2020-02-02 00:00:00.000000 europarser-0.1.7/src/europarser/api/static/basic.min.css
--rw-r--r--   0        0        0     9830 2020-02-02 00:00:00.000000 europarser-0.1.7/src/europarser/api/static/dropzone.min.css
--rw-r--r--   0        0        0   114649 2020-02-02 00:00:00.000000 europarser-0.1.7/src/europarser/api/static/dropzone.min.js
--rw-r--r--   0        0        0    39237 2020-02-02 00:00:00.000000 europarser-0.1.7/src/europarser/api/static/favicon.ico
--rw-r--r--   0        0        0    14776 2020-02-02 00:00:00.000000 europarser-0.1.7/src/europarser/api/templates/main.html
--rw-r--r--   0        0        0      113 2020-02-02 00:00:00.000000 europarser-0.1.7/src/europarser/transformers/__init__.py
--rw-r--r--   0        0        0      659 2020-02-02 00:00:00.000000 europarser-0.1.7/src/europarser/transformers/to_csv.py
--rw-r--r--   0        0        0     1895 2020-02-02 00:00:00.000000 europarser-0.1.7/src/europarser/transformers/to_gephi.py
--rw-r--r--   0        0        0      975 2020-02-02 00:00:00.000000 europarser-0.1.7/src/europarser/transformers/to_iramuteq.py
--rw-r--r--   0        0        0      708 2020-02-02 00:00:00.000000 europarser-0.1.7/src/europarser/transformers/to_json.py
--rw-r--r--   0        0        0     4095 2020-02-02 00:00:00.000000 europarser-0.1.7/src/europarser/transformers/to_markdown.py
--rw-r--r--   0        0        0    18209 2020-02-02 00:00:00.000000 europarser-0.1.7/src/europarser/transformers/to_stats.py
--rw-r--r--   0        0        0     1662 2020-02-02 00:00:00.000000 europarser-0.1.7/src/europarser/transformers/to_txm.py
--rw-r--r--   0        0        0     2824 2020-02-02 00:00:00.000000 europarser-0.1.7/src/europarser/transformers/transformer.py
--rw-r--r--   0        0        0      961 2020-02-02 00:00:00.000000 europarser-0.1.7/tests/api_tester.py
--rw-r--r--   0        0        0     2347 2020-02-02 00:00:00.000000 europarser-0.1.7/.gitignore
--rw-r--r--   0        0        0       99 2020-02-02 00:00:00.000000 europarser-0.1.7/.hgignore
--rw-r--r--   0        0        0    34503 2020-02-02 00:00:00.000000 europarser-0.1.7/LICENSE.txt
--rw-r--r--   0        0        0     3198 2020-02-02 00:00:00.000000 europarser-0.1.7/README.md
--rw-r--r--   0        0        0     2365 2020-02-02 00:00:00.000000 europarser-0.1.7/pyproject.toml
--rw-r--r--   0        0        0     4643 2020-02-02 00:00:00.000000 europarser-0.1.7/PKG-INFO
+-rw-r--r--   0        0        0       71 2020-02-02 00:00:00.000000 europarser-0.1.8/.dockerignore
+-rw-r--r--   0        0        0     1416 2020-02-02 00:00:00.000000 europarser-0.1.8/Dockerfile
+-rw-r--r--   0        0        0     2953 2020-02-02 00:00:00.000000 europarser-0.1.8/README_en.md
+-rw-r--r--   0        0        0     1032 2020-02-02 00:00:00.000000 europarser-0.1.8/docker_log.conf
+-rw-r--r--   0        0        0     1080 2020-02-02 00:00:00.000000 europarser-0.1.8/log.conf
+-rw-r--r--   0        0        0     2365 2020-02-02 00:00:00.000000 europarser-0.1.8/pyinstaller.py
+-rwxr-xr-x   0        0        0     2203 2020-02-02 00:00:00.000000 europarser-0.1.8/start_europarser.sh
+-rw-r--r--   0        0        0     1376 2020-02-02 00:00:00.000000 europarser-0.1.8/.github/workflows/docker-publish.yml
+-rw-r--r--   0        0        0     3536 2020-02-02 00:00:00.000000 europarser-0.1.8/.github/workflows/hatch-build-and-publish.yml
+-rw-r--r--   0        0        0      135 2020-02-02 00:00:00.000000 europarser-0.1.8/src/europarser/__about__.py
+-rw-r--r--   0        0        0      320 2020-02-02 00:00:00.000000 europarser-0.1.8/src/europarser/__init__.py
+-rw-r--r--   0        0        0     2322 2020-02-02 00:00:00.000000 europarser-0.1.8/src/europarser/daniel_light.py
+-rw-r--r--   0        0        0     2485 2020-02-02 00:00:00.000000 europarser-0.1.8/src/europarser/endpoint.py
+-rw-r--r--   0        0        0       93 2020-02-02 00:00:00.000000 europarser-0.1.8/src/europarser/lang_detect.py
+-rw-r--r--   0        0        0     1553 2020-02-02 00:00:00.000000 europarser-0.1.8/src/europarser/main.py
+-rw-r--r--   0        0        0     2256 2020-02-02 00:00:00.000000 europarser-0.1.8/src/europarser/models.py
+-rw-r--r--   0        0        0     2820 2020-02-02 00:00:00.000000 europarser-0.1.8/src/europarser/pipeline.py
+-rw-r--r--   0        0        0     8705 2020-02-02 00:00:00.000000 europarser-0.1.8/src/europarser/pivot.py
+-rw-r--r--   0        0        0    13243 2020-02-02 00:00:00.000000 europarser-0.1.8/src/europarser/utils.py
+-rw-r--r--   0        0        0      153 2020-02-02 00:00:00.000000 europarser-0.1.8/src/europarser/api/__init__.py
+-rw-r--r--   0        0        0     3908 2020-02-02 00:00:00.000000 europarser-0.1.8/src/europarser/api/api.py
+-rw-r--r--   0        0        0      607 2020-02-02 00:00:00.000000 europarser-0.1.8/src/europarser/api/utils.py
+-rw-r--r--   0        0        0      750 2020-02-02 00:00:00.000000 europarser-0.1.8/src/europarser/api/static/basic.min.css
+-rw-r--r--   0        0        0     9830 2020-02-02 00:00:00.000000 europarser-0.1.8/src/europarser/api/static/dropzone.min.css
+-rw-r--r--   0        0        0   114649 2020-02-02 00:00:00.000000 europarser-0.1.8/src/europarser/api/static/dropzone.min.js
+-rw-r--r--   0        0        0    39237 2020-02-02 00:00:00.000000 europarser-0.1.8/src/europarser/api/static/favicon.ico
+-rw-r--r--   0        0        0    15134 2020-02-02 00:00:00.000000 europarser-0.1.8/src/europarser/api/templates/main.html
+-rw-r--r--   0        0        0      113 2020-02-02 00:00:00.000000 europarser-0.1.8/src/europarser/transformers/__init__.py
+-rw-r--r--   0        0        0      659 2020-02-02 00:00:00.000000 europarser-0.1.8/src/europarser/transformers/to_csv.py
+-rw-r--r--   0        0        0      825 2020-02-02 00:00:00.000000 europarser-0.1.8/src/europarser/transformers/to_excel.py
+-rw-r--r--   0        0        0     1895 2020-02-02 00:00:00.000000 europarser-0.1.8/src/europarser/transformers/to_gephi.py
+-rw-r--r--   0        0        0      975 2020-02-02 00:00:00.000000 europarser-0.1.8/src/europarser/transformers/to_iramuteq.py
+-rw-r--r--   0        0        0      708 2020-02-02 00:00:00.000000 europarser-0.1.8/src/europarser/transformers/to_json.py
+-rw-r--r--   0        0        0     4095 2020-02-02 00:00:00.000000 europarser-0.1.8/src/europarser/transformers/to_markdown.py
+-rw-r--r--   0        0        0    18209 2020-02-02 00:00:00.000000 europarser-0.1.8/src/europarser/transformers/to_stats.py
+-rw-r--r--   0        0        0     1662 2020-02-02 00:00:00.000000 europarser-0.1.8/src/europarser/transformers/to_txm.py
+-rw-r--r--   0        0        0     2824 2020-02-02 00:00:00.000000 europarser-0.1.8/src/europarser/transformers/transformer.py
+-rw-r--r--   0        0        0      961 2020-02-02 00:00:00.000000 europarser-0.1.8/tests/api_tester.py
+-rw-r--r--   0        0        0     2347 2020-02-02 00:00:00.000000 europarser-0.1.8/.gitignore
+-rw-r--r--   0        0        0       99 2020-02-02 00:00:00.000000 europarser-0.1.8/.hgignore
+-rw-r--r--   0        0        0    34503 2020-02-02 00:00:00.000000 europarser-0.1.8/LICENSE.txt
+-rw-r--r--   0        0        0     3198 2020-02-02 00:00:00.000000 europarser-0.1.8/README.md
+-rw-r--r--   0        0        0     2365 2020-02-02 00:00:00.000000 europarser-0.1.8/pyproject.toml
+-rw-r--r--   0        0        0     4643 2020-02-02 00:00:00.000000 europarser-0.1.8/PKG-INFO
```

### Comparing `europarser-0.1.7/Dockerfile` & `europarser-0.1.8/Dockerfile`

 * *Files identical despite different names*

### Comparing `europarser-0.1.7/README_en.md` & `europarser-0.1.8/README_en.md`

 * *Files identical despite different names*

### Comparing `europarser-0.1.7/docker_log.conf` & `europarser-0.1.8/docker_log.conf`

 * *Files identical despite different names*

### Comparing `europarser-0.1.7/log.conf` & `europarser-0.1.8/log.conf`

 * *Files identical despite different names*

### Comparing `europarser-0.1.7/pyinstaller.py` & `europarser-0.1.8/pyinstaller.py`

 * *Files identical despite different names*

### Comparing `europarser-0.1.7/start_europarser.sh` & `europarser-0.1.8/start_europarser.sh`

 * *Files identical despite different names*

### Comparing `europarser-0.1.7/.github/workflows/docker-publish.yml` & `europarser-0.1.8/.github/workflows/docker-publish.yml`

 * *Files identical despite different names*

### Comparing `europarser-0.1.7/.github/workflows/hatch-build-and-publish.yml` & `europarser-0.1.8/.github/workflows/hatch-build-and-publish.yml`

 * *Files identical despite different names*

### Comparing `europarser-0.1.7/src/europarser/daniel_light.py` & `europarser-0.1.8/src/europarser/daniel_light.py`

 * *Files identical despite different names*

### Comparing `europarser-0.1.7/src/europarser/endpoint.py` & `europarser-0.1.8/src/europarser/endpoint.py`

 * *Files identical despite different names*

### Comparing `europarser-0.1.7/src/europarser/main.py` & `europarser-0.1.8/src/europarser/main.py`

 * *Files 1% similar despite different names*

```diff
@@ -32,15 +32,15 @@
             with open(folder / f'{result.filename}', 'wb') as f:
                 f.write(result.data)
 
 
 
 if __name__ == '__main__':
     folder = Path('/home/marceau/Nextcloud/eurocollectes/15-18')
-    outputs = ["json", "txm", "iramuteq", "csv", "stats", "processed_stats", "plots", "markdown"]
+    outputs = ["json", "txm", "iramuteq", "csv", "excel", "stats", "processed_stats", "plots", "markdown"]
     # outputs = ["json", "stats", "processed_stats", "plots"]
     params = Params(
         minimal_support_kw=5,
         minimal_support_authors=2,
         minimal_support_journals=8,
         minimal_support_dates=3,
     )
```

### Comparing `europarser-0.1.7/src/europarser/models.py` & `europarser-0.1.8/src/europarser/models.py`

 * *Files 3% similar despite different names*

```diff
@@ -37,16 +37,16 @@
         return hash((self.journal, self.date, self.titre))
 
     @field_serializer('keywords')
     def serialize_keywords(self, kw: Set[str]):
         return ', '.join(kw)
 
 
-OutputFormat = Literal["csv", "json", "txt", "xml", "zip"]
-Output = Literal["json", "txm", "iramuteq", "gephi", "csv", "stats", "processed_stats", "plots", "markdown"]
+OutputFormat = Literal["csv", "excel", "json", "txt", "xml", "zip"]
+Output = Literal["json", "txm", "iramuteq", "gephi", "csv", "excel", "stats", "processed_stats", "plots", "markdown"]
 
 
 class TransformerOutput(BaseModel):
     data: Union[str, bytes, None]
     output: OutputFormat
     filename: str
```

### Comparing `europarser-0.1.7/src/europarser/pipeline.py` & `europarser-0.1.8/src/europarser/pipeline.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,27 +2,29 @@
 
 import concurrent.futures
 
 from tqdm.auto import tqdm
 
 from .models import Output, FileToTransform, TransformerOutput, Params
 from .transformers.to_csv import CSVTransformer
+from .transformers.to_excel import ExcelTransformer
 from .transformers.to_iramuteq import IramuteqTransformer
 from .transformers.to_json import JSONTransformer
 from .transformers.to_markdown import MarkdownTransformer
 from .pivot import PivotTransformer
 from .transformers.to_txm import TXMTransformer
 from .transformers.to_stats import StatsTransformer
 
 transformer_factory = {
     "json": JSONTransformer().transform,
     "txm": TXMTransformer().transform,
     "iramuteq": IramuteqTransformer().transform,
     "gephi": None,
     "csv": CSVTransformer().transform,
+    "excel": ExcelTransformer().transform,
     "stats": "get_stats",
     "processed_stats": "get_processed_stats",
     "plots": "get_plots",
     "markdown": MarkdownTransformer().transform
 }
 
 stats_outputs = {"stats", "processed_stats", "plots", "markdown"}
```

### Comparing `europarser-0.1.7/src/europarser/pivot.py` & `europarser-0.1.8/src/europarser/pivot.py`

 * *Files identical despite different names*

### Comparing `europarser-0.1.7/src/europarser/utils.py` & `europarser-0.1.8/src/europarser/utils.py`

 * *Files identical despite different names*

### Comparing `europarser-0.1.7/src/europarser/api/api.py` & `europarser-0.1.8/src/europarser/api/api.py`

 * *Files 1% similar despite different names*

```diff
@@ -28,14 +28,15 @@
 
 class Outputs(str, Enum):
     json = "json"
     txm = "txm"
     iramuteq = "iramuteq"
     gephi = "gephi"
     csv = "csv"
+    excel = "excel"
     stats = "stats"
     processed_stats = "processed_stats"
     plots = "plots"
     markdown = "markdown"
 
 
 @app.get("/", response_class=HTMLResponse)
```

### Comparing `europarser-0.1.7/src/europarser/api/static/basic.min.css` & `europarser-0.1.8/src/europarser/api/static/basic.min.css`

 * *Files identical despite different names*

### Comparing `europarser-0.1.7/src/europarser/api/static/dropzone.min.css` & `europarser-0.1.8/src/europarser/api/static/dropzone.min.css`

 * *Files identical despite different names*

### Comparing `europarser-0.1.7/src/europarser/api/static/dropzone.min.js` & `europarser-0.1.8/src/europarser/api/static/dropzone.min.js`

 * *Files identical despite different names*

### Comparing `europarser-0.1.7/src/europarser/api/static/favicon.ico` & `europarser-0.1.8/src/europarser/api/static/favicon.ico`

 * *Files identical despite different names*

### Comparing `europarser-0.1.7/src/europarser/api/templates/main.html` & `europarser-0.1.8/src/europarser/api/templates/main.html`

 * *Files 2% similar despite different names*

```diff
@@ -139,14 +139,18 @@
                         for="json">JSON</label>
                 </div>
                 <div class="myDivInput">
                     <input type="checkbox" id="csv" name="output" value="csv" class="myInput"> <label
                         for="csv">CSV</label>
                 </div>
                 <div class="myDivInput">
+                    <input type="checkbox" id="excel" name="output" value="excel" class="myInput"> <label
+                        for="excel">Excel</label>
+                </div>
+                <div class="myDivInput">
                     <input type="checkbox" id="markdown" name="output" value="markdown" class="myInput"> <label
                         for="markdown">Markdown</label>
                 </div>
 
                 <h3 style="font-weight: 100">Statistiques</h3>
 
                 <div class="myDivInput">
@@ -279,14 +283,17 @@
                 }
                 if (document.getElementById('json').checked) {
                     formData.append("output", "json");
                 }
                 if (document.getElementById('csv').checked) {
                     formData.append("output", "csv");
                 }
+                if (document.getElementById('excel').checked) {
+                    formData.append("output", "excel");
+                }
                 if (document.getElementById('stats').checked) {
                     formData.append("output", "stats");
                 }
                 if (document.getElementById('processed_stats').checked) {
                     formData.append("output", "processed_stats");
                     checked = true;
                 }
```

#### html2text {}

```diff
@@ -1,13 +1,14 @@
 ************ CCoonnvveerrttiisssseeuurr EEuurroopprreessssee ************
 **** CCoonnvveerrttiisssseezz ddeess HHTTMMLLss EEuurroopprreessssee vveerrss dd''aauuttrreess ffoorrmmaattss ****
 ??IRAMUTEQ
 ??TXM (XML)
 ??JSON
 ??CSV
+??Excel
 ??Markdown
 ******** SSttaattiissttiiqquueess ********
 ??Statistiques
 ??Statistiques traitées
 ??Graphiques
 ******** PPaarraamm?èttrreess ********
 ??Filter les mots clés n'apparaissant que dans un seul article
```

### Comparing `europarser-0.1.7/src/europarser/transformers/to_csv.py` & `europarser-0.1.8/src/europarser/transformers/to_csv.py`

 * *Files identical despite different names*

### Comparing `europarser-0.1.7/src/europarser/transformers/to_gephi.py` & `europarser-0.1.8/src/europarser/transformers/to_gephi.py`

 * *Files identical despite different names*

### Comparing `europarser-0.1.7/src/europarser/transformers/to_iramuteq.py` & `europarser-0.1.8/src/europarser/transformers/to_iramuteq.py`

 * *Files identical despite different names*

### Comparing `europarser-0.1.7/src/europarser/transformers/to_json.py` & `europarser-0.1.8/src/europarser/transformers/to_json.py`

 * *Files identical despite different names*

### Comparing `europarser-0.1.7/src/europarser/transformers/to_markdown.py` & `europarser-0.1.8/src/europarser/transformers/to_markdown.py`

 * *Files identical despite different names*

### Comparing `europarser-0.1.7/src/europarser/transformers/to_stats.py` & `europarser-0.1.8/src/europarser/transformers/to_stats.py`

 * *Files identical despite different names*

### Comparing `europarser-0.1.7/src/europarser/transformers/to_txm.py` & `europarser-0.1.8/src/europarser/transformers/to_txm.py`

 * *Files identical despite different names*

### Comparing `europarser-0.1.7/src/europarser/transformers/transformer.py` & `europarser-0.1.8/src/europarser/transformers/transformer.py`

 * *Files identical despite different names*

### Comparing `europarser-0.1.7/tests/api_tester.py` & `europarser-0.1.8/tests/api_tester.py`

 * *Files identical despite different names*

### Comparing `europarser-0.1.7/.gitignore` & `europarser-0.1.8/.gitignore`

 * *Files identical despite different names*

### Comparing `europarser-0.1.7/LICENSE.txt` & `europarser-0.1.8/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `europarser-0.1.7/README.md` & `europarser-0.1.8/README.md`

 * *Files identical despite different names*

### Comparing `europarser-0.1.7/pyproject.toml` & `europarser-0.1.8/pyproject.toml`

 * *Files identical despite different names*

### Comparing `europarser-0.1.7/PKG-INFO` & `europarser-0.1.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: europarser
-Version: 0.1.7
+Version: 0.1.8
 Project-URL: Documentation, https://github.com/CERES-sorbonne/europarser#readme
 Project-URL: Issues, https://github.com/CERES-sorbonne/europarser/issues
 Project-URL: Source, https://github.com/CERES-sorbonne/europarser
 Author-email: Marceau <pypi@marceau-h.fr>
 License-Expression: AGPL-3.0-or-later
 License-File: LICENSE.txt
 Classifier: Development Status :: 4 - Beta
```

