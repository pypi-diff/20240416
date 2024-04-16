# Comparing `tmp/pyuniprotkb-0.3.0.tar.gz` & `tmp/pyuniprotkb-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyuniprotkb-0.3.0.tar", last modified: Mon Apr 15 20:33:24 2024, max compression
+gzip compressed data, was "pyuniprotkb-0.4.0.tar", last modified: Tue Apr 16 16:09:57 2024, max compression
```

## Comparing `pyuniprotkb-0.3.0.tar` & `pyuniprotkb-0.4.0.tar`

### file list

```diff
@@ -1,35 +1,35 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 20:33:24.622710 pyuniprotkb-0.3.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1547 2024-04-15 20:33:13.000000 pyuniprotkb-0.3.0/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1067 2024-04-15 20:33:13.000000 pyuniprotkb-0.3.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      348 2024-04-15 20:33:13.000000 pyuniprotkb-0.3.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     4574 2024-04-15 20:33:24.622710 pyuniprotkb-0.3.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3832 2024-04-15 20:33:13.000000 pyuniprotkb-0.3.0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      327 2024-04-15 20:33:13.000000 pyuniprotkb-0.3.0/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 20:33:24.618710 pyuniprotkb-0.3.0/pyuniprot/
--rw-r--r--   0 runner    (1001) docker     (127)       62 2024-04-15 20:33:13.000000 pyuniprotkb-0.3.0/pyuniprot/CC.py
--rw-r--r--   0 runner    (1001) docker     (127)      816 2024-04-15 20:33:13.000000 pyuniprotkb-0.3.0/pyuniprot/DB.py
--rw-r--r--   0 runner    (1001) docker     (127)     9087 2024-04-15 20:33:13.000000 pyuniprotkb-0.3.0/pyuniprot/UniRef.py
--rw-r--r--   0 runner    (1001) docker     (127)    25902 2024-04-15 20:33:13.000000 pyuniprotkb-0.3.0/pyuniprot/Uniprot.py
--rw-r--r--   0 runner    (1001) docker     (127)      242 2024-04-15 20:33:13.000000 pyuniprotkb-0.3.0/pyuniprot/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-15 20:33:13.000000 pyuniprotkb-0.3.0/pyuniprot/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 20:33:24.618710 pyuniprotkb-0.3.0/pyuniprot/utils/
--rw-r--r--   0 runner    (1001) docker     (127)      122 2024-04-15 20:33:13.000000 pyuniprotkb-0.3.0/pyuniprot/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9824 2024-04-15 20:33:13.000000 pyuniprotkb-0.3.0/pyuniprot/utils/isoforms.py
--rw-r--r--   0 runner    (1001) docker     (127)       22 2024-04-15 20:33:13.000000 pyuniprotkb-0.3.0/pyuniprot/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 20:33:24.618710 pyuniprotkb-0.3.0/pyuniprotkb.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     4574 2024-04-15 20:33:24.000000 pyuniprotkb-0.3.0/pyuniprotkb.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      600 2024-04-15 20:33:24.000000 pyuniprotkb-0.3.0/pyuniprotkb.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-15 20:33:24.000000 pyuniprotkb-0.3.0/pyuniprotkb.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       70 2024-04-15 20:33:24.000000 pyuniprotkb-0.3.0/pyuniprotkb.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       16 2024-04-15 20:33:24.000000 pyuniprotkb-0.3.0/pyuniprotkb.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       23 2024-04-15 20:33:13.000000 pyuniprotkb-0.3.0/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)      116 2024-04-15 20:33:13.000000 pyuniprotkb-0.3.0/requirements_dev.txt
--rw-r--r--   0 runner    (1001) docker     (127)      246 2024-04-15 20:33:24.622710 pyuniprotkb-0.3.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1220 2024-04-15 20:33:13.000000 pyuniprotkb-0.3.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 20:33:24.618710 pyuniprotkb-0.3.0/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-15 20:33:13.000000 pyuniprotkb-0.3.0/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      320 2024-04-15 20:33:13.000000 pyuniprotkb-0.3.0/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (127)     3977 2024-04-15 20:33:13.000000 pyuniprotkb-0.3.0/tests/test_isoforms.py
--rw-r--r--   0 runner    (1001) docker     (127)     2940 2024-04-15 20:33:13.000000 pyuniprotkb-0.3.0/tests/test_uniprot.py
--rw-r--r--   0 runner    (1001) docker     (127)     4702 2024-04-15 20:33:13.000000 pyuniprotkb-0.3.0/tests/test_uniref.py
--rw-r--r--   0 runner    (1001) docker     (127)      286 2024-04-15 20:33:13.000000 pyuniprotkb-0.3.0/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 16:09:57.469540 pyuniprotkb-0.4.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1584 2024-04-16 16:09:49.000000 pyuniprotkb-0.4.0/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1067 2024-04-16 16:09:49.000000 pyuniprotkb-0.4.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      348 2024-04-16 16:09:49.000000 pyuniprotkb-0.4.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     4574 2024-04-16 16:09:57.469540 pyuniprotkb-0.4.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3832 2024-04-16 16:09:49.000000 pyuniprotkb-0.4.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      327 2024-04-16 16:09:49.000000 pyuniprotkb-0.4.0/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 16:09:57.465540 pyuniprotkb-0.4.0/pyuniprot/
+-rw-r--r--   0 runner    (1001) docker     (127)       62 2024-04-16 16:09:49.000000 pyuniprotkb-0.4.0/pyuniprot/CC.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2375 2024-04-16 16:09:49.000000 pyuniprotkb-0.4.0/pyuniprot/DB.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9087 2024-04-16 16:09:49.000000 pyuniprotkb-0.4.0/pyuniprot/UniRef.py
+-rw-r--r--   0 runner    (1001) docker     (127)    30664 2024-04-16 16:09:49.000000 pyuniprotkb-0.4.0/pyuniprot/Uniprot.py
+-rw-r--r--   0 runner    (1001) docker     (127)      242 2024-04-16 16:09:49.000000 pyuniprotkb-0.4.0/pyuniprot/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-16 16:09:49.000000 pyuniprotkb-0.4.0/pyuniprot/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 16:09:57.465540 pyuniprotkb-0.4.0/pyuniprot/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)      122 2024-04-16 16:09:49.000000 pyuniprotkb-0.4.0/pyuniprot/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9824 2024-04-16 16:09:49.000000 pyuniprotkb-0.4.0/pyuniprot/utils/isoforms.py
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-04-16 16:09:49.000000 pyuniprotkb-0.4.0/pyuniprot/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 16:09:57.469540 pyuniprotkb-0.4.0/pyuniprotkb.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4574 2024-04-16 16:09:57.000000 pyuniprotkb-0.4.0/pyuniprotkb.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      600 2024-04-16 16:09:57.000000 pyuniprotkb-0.4.0/pyuniprotkb.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-16 16:09:57.000000 pyuniprotkb-0.4.0/pyuniprotkb.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       70 2024-04-16 16:09:57.000000 pyuniprotkb-0.4.0/pyuniprotkb.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       16 2024-04-16 16:09:57.000000 pyuniprotkb-0.4.0/pyuniprotkb.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       23 2024-04-16 16:09:49.000000 pyuniprotkb-0.4.0/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      116 2024-04-16 16:09:49.000000 pyuniprotkb-0.4.0/requirements_dev.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      246 2024-04-16 16:09:57.469540 pyuniprotkb-0.4.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1220 2024-04-16 16:09:49.000000 pyuniprotkb-0.4.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 16:09:57.469540 pyuniprotkb-0.4.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-16 16:09:49.000000 pyuniprotkb-0.4.0/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      320 2024-04-16 16:09:49.000000 pyuniprotkb-0.4.0/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3977 2024-04-16 16:09:49.000000 pyuniprotkb-0.4.0/tests/test_isoforms.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4045 2024-04-16 16:09:49.000000 pyuniprotkb-0.4.0/tests/test_uniprot.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4702 2024-04-16 16:09:49.000000 pyuniprotkb-0.4.0/tests/test_uniref.py
+-rw-r--r--   0 runner    (1001) docker     (127)      286 2024-04-16 16:09:49.000000 pyuniprotkb-0.4.0/tox.ini
```

### Comparing `pyuniprotkb-0.3.0/.pre-commit-config.yaml` & `pyuniprotkb-0.4.0/.pre-commit-config.yaml`

 * *Files 4% similar despite different names*

```diff
@@ -11,15 +11,15 @@
       - id: end-of-file-fixer
         exclude: tests/test_files
       - id: forbid-new-submodules
       - id: trailing-whitespace
         exclude: tests/test_files
 
   - repo: https://github.com/psf/black
-    rev: 24.3.0
+    rev: 24.4.0
     hooks:
       - id: black
         language_version: python3.10
 
   - repo: https://github.com/PyCQA/flake8
     rev: 7.0.0
     hooks:
@@ -32,14 +32,15 @@
           ]
         exclude: tests/test_files
 
   - repo: https://github.com/PyCQA/isort
     rev: 5.13.2
     hooks:
       - id: isort
+        args: ["--profile", "black"]
         files: \.py$
 
   - repo: https://github.com/pre-commit/mirrors-mypy
     rev: v1.9.0
     hooks:
       - id: mypy
         exclude: tests/data
```

### Comparing `pyuniprotkb-0.3.0/LICENSE` & `pyuniprotkb-0.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pyuniprotkb-0.3.0/PKG-INFO` & `pyuniprotkb-0.4.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyuniprotkb
-Version: 0.3.0
+Version: 0.4.0
 Summary: A python package to retrieve bioinformatics given Uniprot IDs.
 Home-page: https://github.com/Ruibin-Liu/pyuniprot
 Author: Ruibin Liu
 Author-email: ruibinliuphd@gmail.com
 Project-URL: Bug Tracker, https://github.com/Ruibin-Liu/pyuniprot/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `pyuniprotkb-0.3.0/README.md` & `pyuniprotkb-0.4.0/README.md`

 * *Files identical despite different names*

### Comparing `pyuniprotkb-0.3.0/pyuniprot/UniRef.py` & `pyuniprotkb-0.4.0/pyuniprot/UniRef.py`

 * *Files identical despite different names*

### Comparing `pyuniprotkb-0.3.0/pyuniprot/Uniprot.py` & `pyuniprotkb-0.4.0/pyuniprot/Uniprot.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 import urllib.request
 from collections import defaultdict
 from dataclasses import dataclass
 from datetime import date, datetime
 from pathlib import Path
 from typing import Union
 
-from .DB import HGNC, PANTHER, PDB, SeqRange
+from .DB import CCDS, EMBL, GO, HGNC, PANTHER, PDB, PIR, Reactome, RefSeq, SeqRange
 
 
 @dataclass
 class ID:
     """Entry name and length"""
 
     entry_name: str
@@ -155,14 +155,55 @@
     weight: int
     crc_checksum_value: str
     crc_bits: int
 
 
 UNIPROT = Union[ID, AC, DT, DE, GN, OSCX, RNPCXATL, CC, DR, PE, KW, FT, SQ]
 
+GO_TYPE = {
+    "C": "Cellular Component",
+    "F": "Molecular Fucntion",
+    "P": "Biological Process",
+}
+GO_SOURCE = {
+    # experimental evidence codess
+    "EXP": "Experiment",  # usually peer-reviewed publication
+    "IDA": "Direct Assay",
+    "IPI": "Physical Interaction",
+    "IMP": "Mutant Phenotype",
+    "IGI": "Genetic Interaction",
+    "IEP": "Epression Pattern",
+    "HTP": "High Throughput Pxperiment",
+    "HDA": "High Throughput Direct Assay",
+    "HMP": "High Throughput Mutant Phenotype",
+    "HGI": "High Throughput Genetic Interaction",
+    "HEP": "High Throughputf Expression Pattern",
+    # phylogenetically-inferred annotations
+    "IBA": "Biological aspect of Ancestor",
+    "IBD": "Biological aspect of Descendant",
+    "IKR": "Key Residues",
+    "IRD": "Rapid Divergence",
+    # computational analysis evidence codes
+    "ISS": "Sequence or structural Similarity",
+    "ISO": "Sequence Orthology",
+    "ISA": "Sequence Alignment",
+    "ISM": "Sequence Model",
+    "IGC": "Genomic Context",
+    "RCA": "Reviewed Computational Analysis",
+    # author statement evidence codes
+    "TAS": "Traceable Author Statement",
+    "NAS": "Non-traceable Author Statement",
+    # curator statement evidence codes
+    "IC": "Curator",
+    "ND": "No biological Data available",
+    # electronic annotation evidence code
+    "IEA": "Electronic Annotation",
+}
+"""From https://geneontology.org/docs/guide-go-evidence-codes"""
+
 
 class Uniprot:
     """The python object representing all information of a Uniprot txt file."""
 
     def __init__(
         self,
         uniprot_id: str,
@@ -552,14 +593,88 @@
                                 family_name,
                                 family_occurrence,
                                 subfamily_id,
                                 subfamily_name,
                                 subfamily_occurrence,
                             )
                         )
+                    elif db_name == "EMBL":
+                        nucleotide_sequence_id: str = db_content[0].strip()
+                        protein_sequence_id: str = db_content[1].strip()
+                        molecule_type: str = db_content[2].strip()
+                        status: str = db_content[3].strip()
+                        db_reference[db_name].append(
+                            EMBL(
+                                nucleotide_sequence_id,
+                                protein_sequence_id,
+                                molecule_type,
+                                status,
+                            )
+                        )
+                    elif db_name == "CCDS":
+                        ccds_id: str = db_content[0].strip()
+                        isoform: str = db_content[1].split("[")[-1].strip("]")
+                        db_reference[db_name].append(
+                            CCDS(
+                                ccds_id,
+                                isoform,
+                            )
+                        )
+                    elif db_name == "PIR":
+                        uid: str = db_content[0].strip()
+                        entry: str = db_content[1].strip()
+                        db_reference[db_name].append(
+                            PIR(
+                                uid,
+                                entry,
+                            )
+                        )
+                    elif db_name == "GO":
+                        accession_number: str = db_content[0].split(":")[-1]
+                        aspect_term = db_content[1].strip().split(":")
+                        aspect: str = aspect_term[0]
+                        aspect = GO_TYPE[aspect]
+                        term: str = aspect_term[1]
+                        infer = db_content[2].strip().split(":")
+                        inferred_from: str = infer[0]
+                        inferred_from = GO_SOURCE[inferred_from]
+                        source: str = infer[1]
+                        db_reference[db_name].append(
+                            GO(
+                                accession_number,
+                                aspect,
+                                term,
+                                inferred_from,
+                                source,
+                            )
+                        )
+                    elif db_name == "Reactome":
+                        id: str = db_content[0].strip()
+                        pathway: str = db_content[1].strip()
+                        db_reference[db_name].append(
+                            Reactome(
+                                id,
+                                pathway,
+                            )
+                        )
+                    elif db_name == "RefSeq":
+                        protein_sequence_id = db_content[0].strip()
+                        items = db_content[1].strip().split()
+                        nucleotide_sequence_id = items[0]
+                        if len(items) > 1:
+                            isoform = items[1].strip("[").strip("]")
+                        else:
+                            isoform = ""
+                        db_reference[db_name].append(
+                            RefSeq(
+                                protein_sequence_id,
+                                nucleotide_sequence_id,
+                                isoform,
+                            )
+                        )
                     else:
                         db_reference[db_name].append(tuple(db_content))
                     line = u_file.readline()
                 content_dict["DR"] = DR(db_reference)
                 continue
             elif line.startswith("PE"):
                 protein_existence: str = line[5:-2]
@@ -581,15 +696,15 @@
                     record_name: str = line[2:20].strip()
                     if record_name != "":
                         one_record: dict[str, str | int | SeqRange | None] = {}
                         site_or_range: str | int | SeqRange | None = None
                         seq_ids: list[str] = [
                             seq_id for seq_id in line[20:].strip().split("..")
                         ]
-                        isoform: str = self.uniprot_id
+                        isoform = self.uniprot_id
                         if ":" in seq_ids[0]:
                             isoform = seq_ids[0].split(":")[0]
                         if len(seq_ids) == 1:
                             name: str = "at_site"
                             try:
                                 site_or_range = int(seq_ids[0].split(":")[-1])
                             except ValueError:
@@ -617,16 +732,14 @@
                         while record_name_like == "":
                             if "/" in line:
                                 one_record_lines += line[19:-1]
                             else:
                                 one_record_lines += line[21:-1]
                             line = u_file.readline()
                             record_name_like = line[2:20].strip()
-                        # if record_name == 'VAR_SEQ':
-                        #     print(one_record_lines)
                         attrs: list[str] = one_record_lines.rstrip().split("  /")
                         for attr in attrs[1:]:
                             attr_name, attr_content = attr.strip().split('="')
                             one_record[attr_name] = attr_content.strip('"')
                         feature_tables[record_name].append(one_record)
                 content_dict["FT"] = FT(feature_tables)
                 continue
@@ -643,11 +756,9 @@
                     line = u_file.readline()
                 content_dict["SQ"] = SQ(
                     sequence, length, weight, crc_checksum_value, crc_bits
                 )
                 break
 
             line = u_file.readline()
-        # print(line)
 
         self._category_lines = content_dict
-        # print(self.category_lines["FT"].feature_tables)
```

### Comparing `pyuniprotkb-0.3.0/pyuniprot/utils/isoforms.py` & `pyuniprotkb-0.4.0/pyuniprot/utils/isoforms.py`

 * *Files identical despite different names*

### Comparing `pyuniprotkb-0.3.0/pyuniprotkb.egg-info/PKG-INFO` & `pyuniprotkb-0.4.0/pyuniprotkb.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyuniprotkb
-Version: 0.3.0
+Version: 0.4.0
 Summary: A python package to retrieve bioinformatics given Uniprot IDs.
 Home-page: https://github.com/Ruibin-Liu/pyuniprot
 Author: Ruibin Liu
 Author-email: ruibinliuphd@gmail.com
 Project-URL: Bug Tracker, https://github.com/Ruibin-Liu/pyuniprot/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `pyuniprotkb-0.3.0/pyuniprotkb.egg-info/SOURCES.txt` & `pyuniprotkb-0.4.0/pyuniprotkb.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pyuniprotkb-0.3.0/setup.py` & `pyuniprotkb-0.4.0/setup.py`

 * *Files identical despite different names*

### Comparing `pyuniprotkb-0.3.0/tests/test_isoforms.py` & `pyuniprotkb-0.4.0/tests/test_isoforms.py`

 * *Files identical despite different names*

### Comparing `pyuniprotkb-0.3.0/tests/test_uniref.py` & `pyuniprotkb-0.4.0/tests/test_uniref.py`

 * *Files identical despite different names*

