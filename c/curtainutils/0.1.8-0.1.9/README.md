# Comparing `tmp/curtainutils-0.1.8.tar.gz` & `tmp/curtainutils-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "curtainutils-0.1.8.tar", max compression
+gzip compressed data, was "curtainutils-0.1.9.tar", max compression
```

## Comparing `curtainutils-0.1.8.tar` & `curtainutils-0.1.9.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0        0 2023-09-12 15:15:05.573182 curtainutils-0.1.8/curtainutils/__init__.py
--rw-r--r--   0        0        0    12511 2023-11-06 12:44:21.495664 curtainutils-0.1.8/curtainutils/client.py
--rw-r--r--   0        0        0    10171 2023-11-12 21:05:28.582773 curtainutils-0.1.8/curtainutils/common.py
--rw-r--r--   0        0        0     6952 2024-01-12 13:28:23.732241 curtainutils-0.1.8/curtainutils/diann.py
--rw-r--r--   0        0        0     4994 2024-01-12 13:27:36.075152 curtainutils-0.1.8/curtainutils/msfragger.py
--rw-r--r--   0        0        0     4644 2024-01-12 13:28:23.727235 curtainutils-0.1.8/curtainutils/spectronaut.py
--rw-r--r--   0        0        0     1098 2023-09-10 15:58:15.517718 curtainutils-0.1.8/LICENSE
--rw-r--r--   0        0        0      699 2024-01-12 13:29:19.789133 curtainutils-0.1.8/pyproject.toml
--rw-r--r--   0        0        0     4498 2023-11-02 16:39:57.932650 curtainutils-0.1.8/README.md
--rw-r--r--   0        0        0     5192 1970-01-01 00:00:00.000000 curtainutils-0.1.8/PKG-INFO
+-rw-r--r--   0        0        0        0 2023-09-12 15:15:05.573182 curtainutils-0.1.9/curtainutils/__init__.py
+-rw-r--r--   0        0        0    12511 2023-11-06 12:44:21.495664 curtainutils-0.1.9/curtainutils/client.py
+-rw-r--r--   0        0        0    10171 2023-11-12 21:05:28.582773 curtainutils-0.1.9/curtainutils/common.py
+-rw-r--r--   0        0        0     7168 2024-02-04 19:48:21.501431 curtainutils-0.1.9/curtainutils/diann.py
+-rw-r--r--   0        0        0     5276 2024-02-04 19:48:21.517006 curtainutils-0.1.9/curtainutils/msfragger.py
+-rw-r--r--   0        0        0     4834 2024-02-04 19:48:21.525518 curtainutils-0.1.9/curtainutils/spectronaut.py
+-rw-r--r--   0        0        0     1098 2023-09-10 15:58:15.517718 curtainutils-0.1.9/LICENSE
+-rw-r--r--   0        0        0      699 2024-02-04 19:49:13.066249 curtainutils-0.1.9/pyproject.toml
+-rw-r--r--   0        0        0     4498 2023-11-02 16:39:57.932650 curtainutils-0.1.9/README.md
+-rw-r--r--   0        0        0     5192 1970-01-01 00:00:00.000000 curtainutils-0.1.9/PKG-INFO
```

### Comparing `curtainutils-0.1.8/curtainutils/client.py` & `curtainutils-0.1.9/curtainutils/client.py`

 * *Files identical despite different names*

### Comparing `curtainutils-0.1.8/curtainutils/common.py` & `curtainutils-0.1.9/curtainutils/common.py`

 * *Files identical despite different names*

### Comparing `curtainutils-0.1.8/curtainutils/diann.py` & `curtainutils-0.1.9/curtainutils/diann.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,56 +4,57 @@
 import pandas as pd
 from uniprotparser.betaparser import UniprotParser, UniprotSequence
 from sequal.sequence import Sequence
 def lambda_function_for_diann_ptm_single_site(row: pd.Series, modified_seq_col: str, entry_col: str, fasta_df: pd.DataFrame, modification_of_interests: str) -> pd.Series:
     seq = Sequence(row[modified_seq_col])
     stripped_seq = seq.to_stripped_string()
     print(f"Processing {row[modified_seq_col]}")
-    for i in seq:
-        if len(i.mods) > 0:
-            for mod in i.mods:
-                if mod.value == modification_of_interests:
-                    row["Position.in.peptide"] = i.position
-                    row["Residue"] = i.value
-                    row["Variant"] = row["Protein.Group"]
-                    matched_acc_row = fasta_df[fasta_df["Entry"].str.contains(row[entry_col])]
-                    if len(matched_acc_row) > 0:
-                        for i2, row2 in matched_acc_row.iterrows():
-                            seq = row2["Sequence"]
-                            peptide_seq = stripped_seq
-                            try:
-                                peptide_position = seq.index(peptide_seq)
-                            except ValueError:
-                                peptide_position = seq.replace("I", "L").index(
-                                    peptide_seq.replace("I", "L"))
-                                row["Comment"] = "I replaced by L"
-                            if peptide_position >= -1:
+    if row[entry_col] in fasta_df["Entry"].values:
+        for i in seq:
+            if len(i.mods) > 0:
+                for mod in i.mods:
+                    if mod.value == modification_of_interests:
+                        row["Position.in.peptide"] = i.position
+                        row["Residue"] = i.value
+                        row["Variant"] = row["Protein.Group"]
+                        matched_acc_row = fasta_df[fasta_df["Entry"].str.contains(row[entry_col])]
+                        if len(matched_acc_row) > 0:
+                            for i2, row2 in matched_acc_row.iterrows():
+                                seq = row2["Sequence"]
+                                peptide_seq = stripped_seq
+                                try:
+                                    peptide_position = seq.index(peptide_seq)
+                                except ValueError:
+                                    peptide_position = seq.replace("I", "L").index(
+                                        peptide_seq.replace("I", "L"))
+                                    row["Comment"] = "I replaced by L"
+                                if peptide_position >= -1:
 
-                                position_in_protein = i.position + peptide_position
-                                row["Position"] = position_in_protein
-                                row["Variant"] = row2["Entry"]
-                                sequence_window = ""
-                                if row["Position"] - 1 - 10 >= 0:
-                                    sequence_window += seq[row["Position"] - 1 - 10:row["Position"] - 1]
-                                else:
-                                    sequence_window += seq[:row["Position"] - 1]
-                                    if len(sequence_window) < 10:
-                                        sequence_window = "_" * (10 - len(sequence_window)) + sequence_window
-                                sequence_window += seq[row["Position"] - 1]
-                                if row["Position"] + 10 <= len(seq):
-                                    sequence_window += seq[row["Position"]:row["Position"] + 10]
-                                else:
-                                    sequence_window += seq[row["Position"]:]
-                                    if len(sequence_window) < 21:
-                                        sequence_window += "_" * (21 - len(sequence_window))
-                                if "Protein names" in row2:
-                                    row["Protein.Name"] = row2["Protein names"]
-                                row["Sequence.window"] = sequence_window
-                                break
-                    break
+                                    position_in_protein = i.position + peptide_position
+                                    row["Position"] = position_in_protein
+                                    row["Variant"] = row2["Entry"]
+                                    sequence_window = ""
+                                    if row["Position"] - 1 - 10 >= 0:
+                                        sequence_window += seq[row["Position"] - 1 - 10:row["Position"] - 1]
+                                    else:
+                                        sequence_window += seq[:row["Position"] - 1]
+                                        if len(sequence_window) < 10:
+                                            sequence_window = "_" * (10 - len(sequence_window)) + sequence_window
+                                    sequence_window += seq[row["Position"] - 1]
+                                    if row["Position"] + 10 <= len(seq):
+                                        sequence_window += seq[row["Position"]:row["Position"] + 10]
+                                    else:
+                                        sequence_window += seq[row["Position"]:]
+                                        if len(sequence_window) < 21:
+                                            sequence_window += "_" * (21 - len(sequence_window))
+                                    if "Protein names" in row2:
+                                        row["Protein.Name"] = row2["Protein names"]
+                                    row["Sequence.window"] = sequence_window
+                                    break
+                        break
     return row
 
 def process_diann_ptm(pr_file_path: str, report_file_path: str, output_file: str, modification_of_interests: str = "UniMod:21", columns: str = "accession,id,sequence,protein_name"):
     df = pd.read_csv(pr_file_path, sep="\t")
     localization_score_col = "PTM.Site.Confidence"
     modified_seq_col = "Modified.Sequence"
     index_col = "Precursor.Id"
```

### Comparing `curtainutils-0.1.8/curtainutils/msfragger.py` & `curtainutils-0.1.9/curtainutils/msfragger.py`

 * *Files 3% similar despite different names*

```diff
@@ -13,80 +13,82 @@
     match = reg_positon_residue.search(row[index_col])
     print(f"Processing {row[index_col]}")
     if match:
         position = int(match.group(2))
         row["Position"] = position
         row["Residue"] = match.group(1)
         row["Peptide_Sequence"] = row[peptide_col].split(";")[0]
-        matched_acc_row = fasta_df[fasta_df["Entry"].str.contains(row["PrimaryID"])]
-        if len(matched_acc_row) > 0:
-            if not parse_from_peptide_col:
-                for i2, row2 in matched_acc_row.iterrows():
-                    seq = row2["Sequence"]
-
-                    peptide_seq = row["Peptide_Sequence"].split(";")[0].upper()
-                    try:
-                        peptide_position = seq.index(peptide_seq)
-                    except ValueError:
-                        peptide_position = seq.replace("I", "L").index(
-                            peptide_seq.replace("I", "L"))
-                        row["Comment"] = "I replaced by L"
-                    if peptide_position >= -1:
-
-                        position_in_peptide = position - peptide_position
-                        row["Position.in.peptide"] = position_in_peptide
-                        row["Variant"] = row2["Entry"]
-                        sequence_window = ""
-                        if row["Position"] - 1 - 10 >= 0:
-                            sequence_window += seq[row["Position"] - 1 - 10:row["Position"] - 1]
-                        else:
-                            sequence_window += seq[:row["Position"] - 1]
-                            if len(sequence_window) < 10:
-                                sequence_window = "_" * (10 - len(sequence_window)) + sequence_window
-                        sequence_window += seq[row["Position"] - 1]
-                        if row["Position"] + 10 <= len(seq):
-                            sequence_window += seq[row["Position"]:row["Position"] + 10]
-                        else:
-                            sequence_window += seq[row["Position"]:]
-                            if len(sequence_window) < 21:
-                                sequence_window += "_" * (21 - len(sequence_window))
-
-                        row["Sequence.window"] = sequence_window
-                        if "Protein names" in row2:
-                            row["Protein.Name"] = row2["Protein names"]
-                        break
-            else:
-                # get index of character in lower case
-                for i, aa in enumerate(row["Peptide_Sequence"]):
-                    if aa.islower() and row["Residue"] == aa.upper():
-                        row["Position.in.peptide"] = i + 1
-                        break
+        if row["PrimaryID"] in fasta_df["Entry"].values:
+            matched_acc_row = fasta_df[fasta_df["Entry"].str.contains(row["PrimaryID"])]
+
+            if len(matched_acc_row) > 0:
+                if not parse_from_peptide_col:
+                    for i2, row2 in matched_acc_row.iterrows():
+                        seq = row2["Sequence"]
+
+                        peptide_seq = row["Peptide_Sequence"].split(";")[0].upper()
+                        try:
+                            peptide_position = seq.index(peptide_seq)
+                        except ValueError:
+                            peptide_position = seq.replace("I", "L").index(
+                                peptide_seq.replace("I", "L"))
+                            row["Comment"] = "I replaced by L"
+                        if peptide_position >= -1:
+
+                            position_in_peptide = position - peptide_position
+                            row["Position.in.peptide"] = position_in_peptide
+                            row["Variant"] = row2["Entry"]
+                            sequence_window = ""
+                            if row["Position"] - 1 - 10 >= 0:
+                                sequence_window += seq[row["Position"] - 1 - 10:row["Position"] - 1]
+                            else:
+                                sequence_window += seq[:row["Position"] - 1]
+                                if len(sequence_window) < 10:
+                                    sequence_window = "_" * (10 - len(sequence_window)) + sequence_window
+                            sequence_window += seq[row["Position"] - 1]
+                            if row["Position"] + 10 <= len(seq):
+                                sequence_window += seq[row["Position"]:row["Position"] + 10]
+                            else:
+                                sequence_window += seq[row["Position"]:]
+                                if len(sequence_window) < 21:
+                                    sequence_window += "_" * (21 - len(sequence_window))
+
+                            row["Sequence.window"] = sequence_window
+                            if "Protein names" in row2:
+                                row["Protein.Name"] = row2["Protein names"]
+                            break
+                else:
+                    # get index of character in lower case
+                    for i, aa in enumerate(row["Peptide_Sequence"]):
+                        if aa.islower() and row["Residue"] == aa.upper():
+                            row["Position.in.peptide"] = i + 1
+                            break
 
     return row
 
 
 def process_msfragger_ptm_single_site(file_path: str, index_col: str, peptide_col: str, output_file: str, fasta_file: str = "", get_position_from_peptide_column: bool = False, columns: str = "accession,id,sequence,protein_name"):
     df = pd.read_csv(file_path, sep="\t")
-
+    print(df.shape)
     df["PrimaryID"] = df[index_col].apply(lambda x: str(UniprotSequence(x, parse_acc=True)) if UniprotSequence(x, parse_acc=True).accession else x)
     if fasta_file:
         fasta_df = read_fasta(fasta_file)
     else:
         parser = UniprotParser(columns=columns, include_isoform=True)
         fasta_df = []
-        for i in parser.parse(df["PrimaryID"].unique().tolist()):
+        for i in parser.parse(df["PrimaryID"].unique().tolist(), 500):
             fasta_df.append(pd.read_csv(io.StringIO(i), sep="\t"))
         if len(fasta_df) == 1:
             fasta_df = fasta_df[0]
         else:
             fasta_df = pd.concat(fasta_df, ignore_index=True)
-
+    print(df.shape)
     df = df.apply(lambda x: lambda_function_for_msfragger_ptm_single_site(x, index_col, peptide_col, fasta_df, get_position_from_peptide_column),
                   axis=1)
-
+    print(df.shape)
 
     df.to_csv(output_file, sep="\t", index=False)
 
 
 @click.command()
 @click.option("--file_path", "-f", help="Path to the file to be processed")
 @click.option("--index_col", "-i", help="Name of the index column", default="Index")
```

### Comparing `curtainutils-0.1.8/curtainutils/spectronaut.py` & `curtainutils-0.1.9/curtainutils/spectronaut.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,49 +6,50 @@
 import re
 from curtainutils.common import read_fasta
 reg_pattern = re.compile("_\w(\d+)_")
 protein_name_pattern = re.compile("(\w+_\w+)")
 def lambda_function_for_spectronaut_ptm(row: pd.Series, index_col: str, peptide_col: str, fasta_df: pd.DataFrame) -> pd.Series:
     d = row[index_col].split("_")
     row["Position"] = int(d[-2][1:])
-    matched_acc_row = fasta_df[fasta_df["Entry"].str.contains(row["UniprotID"])]
-    reformat_seq = row[peptide_col].split(";")[0].upper()
-    if len(matched_acc_row) > 0:
-        for i2, row2 in matched_acc_row.iterrows():
-            row2["PeptideSequence"] = reformat_seq[:len(reformat_seq)-2]
-            seq = row2["Sequence"]
-            try:
-                peptide_position = seq.index(row2["PeptideSequence"])
-            except ValueError:
-                peptide_position = seq.replace("I", "L").index(
-                    row2["PeptideSequence"].replace("I", "L"))
-                row["Comment"] = "I replaced by L"
-            if peptide_position >= -1:
-                if "Protein names" in row2:
-                    row["Protein.Name"] = row2["Protein names"]
-                position_in_peptide = row["Position"] - peptide_position
-                row["Position.in.peptide"] = position_in_peptide
-                row["Variant"] = row2["Entry"]
-                sequence_window = ""
-                if row["Position"] - 1 - 10 >= 0:
-                    sequence_window += seq[row["Position"] - 1 - 10:row["Position"] - 1]
-                else:
-                    sequence_window += seq[:row["Position"] - 1]
-                    if len(sequence_window) < 10:
-                        sequence_window = "_" * (10 - len(sequence_window)) + sequence_window
-                sequence_window += seq[row["Position"] - 1]
-                if row["Position"] + 10 <= len(seq):
-                    sequence_window += seq[row["Position"]:row["Position"] + 10]
-                else:
-                    sequence_window += seq[row["Position"]:]
-                    if len(sequence_window) < 21:
-                        sequence_window += "_" * (21 - len(sequence_window))
+    if row["UniprotID"] in fasta_df["Entry"].values:
+        matched_acc_row = fasta_df[fasta_df["Entry"].str.contains(row["UniprotID"])]
+        reformat_seq = row[peptide_col].split(";")[0].upper()
+        if len(matched_acc_row) > 0:
+            for i2, row2 in matched_acc_row.iterrows():
+                row2["PeptideSequence"] = reformat_seq[:len(reformat_seq)-2]
+                seq = row2["Sequence"]
+                try:
+                    peptide_position = seq.index(row2["PeptideSequence"])
+                except ValueError:
+                    peptide_position = seq.replace("I", "L").index(
+                        row2["PeptideSequence"].replace("I", "L"))
+                    row["Comment"] = "I replaced by L"
+                if peptide_position >= -1:
+                    if "Protein names" in row2:
+                        row["Protein.Name"] = row2["Protein names"]
+                    position_in_peptide = row["Position"] - peptide_position
+                    row["Position.in.peptide"] = position_in_peptide
+                    row["Variant"] = row2["Entry"]
+                    sequence_window = ""
+                    if row["Position"] - 1 - 10 >= 0:
+                        sequence_window += seq[row["Position"] - 1 - 10:row["Position"] - 1]
+                    else:
+                        sequence_window += seq[:row["Position"] - 1]
+                        if len(sequence_window) < 10:
+                            sequence_window = "_" * (10 - len(sequence_window)) + sequence_window
+                    sequence_window += seq[row["Position"] - 1]
+                    if row["Position"] + 10 <= len(seq):
+                        sequence_window += seq[row["Position"]:row["Position"] + 10]
+                    else:
+                        sequence_window += seq[row["Position"]:]
+                        if len(sequence_window) < 21:
+                            sequence_window += "_" * (21 - len(sequence_window))
 
-                row["Sequence.window"] = sequence_window
-                break
+                    row["Sequence.window"] = sequence_window
+                    break
     return row
 
 @click.command()
 @click.option("--file_path", "-f", help="Path to the file to be processed")
 @click.option("--index_col", "-i", help="Name of the index column", default="PTM_collapse_key")
 @click.option("--peptide_col", "-p", help="Name of the peptide column", default="PEP.StrippedSequence")
 @click.option("--output_file", "-o", help="Path to the output file")
```

### Comparing `curtainutils-0.1.8/LICENSE` & `curtainutils-0.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `curtainutils-0.1.8/pyproject.toml` & `curtainutils-0.1.9/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "curtainutils"
-version = "0.1.8"
+version = "0.1.9"
 description = "A utility package that can be used to upload data to a curtain backend server."
 authors = ["Toan Phung <toan.phung@proteo.info>"]
 readme = "README.md"
 license = "MIT"
 
 [tool.poetry.dependencies]
 python = "^3.9"
```

### Comparing `curtainutils-0.1.8/README.md` & `curtainutils-0.1.9/README.md`

 * *Files identical despite different names*

### Comparing `curtainutils-0.1.8/PKG-INFO` & `curtainutils-0.1.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: curtainutils
-Version: 0.1.8
+Version: 0.1.9
 Summary: A utility package that can be used to upload data to a curtain backend server.
 License: MIT
 Author: Toan Phung
 Author-email: toan.phung@proteo.info
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

