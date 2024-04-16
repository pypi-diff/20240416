# Comparing `tmp/picnic-bio-1.0.0b2.tar.gz` & `tmp/picnic_bio-1.0.0b3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "picnic-bio-1.0.0b2.tar", last modified: Thu Dec 14 10:49:03 2023, max compression
+gzip compressed data, was "picnic_bio-1.0.0b3.tar", last modified: Tue Apr 16 07:06:22 2024, max compression
```

## Comparing `picnic-bio-1.0.0b2.tar` & `picnic_bio-1.0.0b3.tar`

### file list

```diff
@@ -1,44 +1,44 @@
-drwxr-xr-x   0 maxim      (502) staff       (20)        0 2023-12-14 10:49:03.116653 picnic-bio-1.0.0b2/
--rw-r--r--   0 maxim      (502) staff       (20)     1514 2023-10-11 14:32:47.000000 picnic-bio-1.0.0b2/LICENSE
--rw-r--r--   0 maxim      (502) staff       (20)     8094 2023-12-14 10:49:03.116163 picnic-bio-1.0.0b2/PKG-INFO
--rw-r--r--   0 maxim      (502) staff       (20)     9947 2023-12-14 09:56:30.000000 picnic-bio-1.0.0b2/README.md
-drwxr-xr-x   0 maxim      (502) staff       (20)        0 2023-12-14 10:49:03.114883 picnic-bio-1.0.0b2/picnic_bio.egg-info/
--rw-r--r--   0 maxim      (502) staff       (20)     8094 2023-12-14 10:49:03.000000 picnic-bio-1.0.0b2/picnic_bio.egg-info/PKG-INFO
--rw-r--r--   0 maxim      (502) staff       (20)     1132 2023-12-14 10:49:03.000000 picnic-bio-1.0.0b2/picnic_bio.egg-info/SOURCES.txt
--rw-r--r--   0 maxim      (502) staff       (20)        1 2023-12-14 10:49:03.000000 picnic-bio-1.0.0b2/picnic_bio.egg-info/dependency_links.txt
--rw-r--r--   0 maxim      (502) staff       (20)       48 2023-12-14 10:49:03.000000 picnic-bio-1.0.0b2/picnic_bio.egg-info/entry_points.txt
--rw-r--r--   0 maxim      (502) staff       (20)      103 2023-12-14 10:49:03.000000 picnic-bio-1.0.0b2/picnic_bio.egg-info/requires.txt
--rw-r--r--   0 maxim      (502) staff       (20)       11 2023-12-14 10:49:03.000000 picnic-bio-1.0.0b2/picnic_bio.egg-info/top_level.txt
--rw-r--r--   0 maxim      (502) staff       (20)      182 2023-10-11 14:32:47.000000 picnic-bio-1.0.0b2/pyproject.toml
--rw-r--r--   0 maxim      (502) staff       (20)      528 2023-12-14 10:49:03.118096 picnic-bio-1.0.0b2/setup.cfg
--rw-r--r--   0 maxim      (502) staff       (20)     2180 2023-12-14 09:56:30.000000 picnic-bio-1.0.0b2/setup.py
-drwxr-xr-x   0 maxim      (502) staff       (20)        0 2023-12-14 10:49:03.055968 picnic-bio-1.0.0b2/src/
--rw-r--r--   0 maxim      (502) staff       (20)        0 2023-10-11 14:32:47.000000 picnic-bio-1.0.0b2/src/__init__.py
--rw-r--r--   0 maxim      (502) staff       (20)      591 2023-12-12 10:02:21.000000 picnic-bio-1.0.0b2/src/exceptions.py
-drwxr-xr-x   0 maxim      (502) staff       (20)        0 2023-12-14 10:49:03.060777 picnic-bio-1.0.0b2/src/features/
--rw-r--r--   0 maxim      (502) staff       (20)        0 2023-10-11 14:32:47.000000 picnic-bio-1.0.0b2/src/features/__init__.py
--rw-r--r--   0 maxim      (502) staff       (20)     1470 2023-10-11 14:32:47.000000 picnic-bio-1.0.0b2/src/features/calculation_disorder.py
--rw-r--r--   0 maxim      (502) staff       (20)     2310 2023-12-12 10:02:21.000000 picnic-bio-1.0.0b2/src/features/goterms.py
--rw-r--r--   0 maxim      (502) staff       (20)      918 2023-10-11 14:32:47.000000 picnic-bio-1.0.0b2/src/features/sequence_complexity.py
--rw-r--r--   0 maxim      (502) staff       (20)     2571 2023-10-11 14:32:47.000000 picnic-bio-1.0.0b2/src/features/sequence_distance.py
--rw-r--r--   0 maxim      (502) staff       (20)     8465 2023-10-11 14:32:47.000000 picnic-bio-1.0.0b2/src/features/sequence_structure_AF2.py
-drwxr-xr-x   0 maxim      (502) staff       (20)        0 2023-12-14 10:49:03.061532 picnic-bio-1.0.0b2/src/files/
--rw-r--r--   0 maxim      (502) staff       (20)      178 2023-10-11 14:32:47.000000 picnic-bio-1.0.0b2/src/files/__init__.py
-drwxr-xr-x   0 maxim      (502) staff       (20)        0 2023-12-14 10:49:03.085378 picnic-bio-1.0.0b2/src/files/go/
--rw-r--r--   0 maxim      (502) staff       (20)   628505 2023-08-14 14:33:27.000000 picnic-bio-1.0.0b2/src/files/go/bp_2500_freq.txt
--rw-r--r--   0 maxim      (502) staff       (20)  3146152 2023-08-14 14:33:27.000000 picnic-bio-1.0.0b2/src/files/go/bp_2500_freq_all.json
--rw-r--r--   0 maxim      (502) staff       (20)    91947 2023-08-14 14:33:27.000000 picnic-bio-1.0.0b2/src/files/go/cc_2000_freq.txt
--rw-r--r--   0 maxim      (502) staff       (20)   263088 2023-08-14 14:33:27.000000 picnic-bio-1.0.0b2/src/files/go/cc_2000_freq_all.json
--rw-r--r--   0 maxim      (502) staff       (20)   245749 2023-08-14 14:33:27.000000 picnic-bio-1.0.0b2/src/files/go/mf_2500_freq.txt
--rw-r--r--   0 maxim      (502) staff       (20)   869522 2023-08-14 14:33:28.000000 picnic-bio-1.0.0b2/src/files/go/mf_2500_freq_all.json
-drwxr-xr-x   0 maxim      (502) staff       (20)        0 2023-12-14 10:49:03.099486 picnic-bio-1.0.0b2/src/files/models_llps/
--rw-r--r--   0 maxim      (502) staff       (20)      157 2023-08-14 14:33:28.000000 picnic-bio-1.0.0b2/src/files/models_llps/keys_llps_withgonocc_retrained_newgo_18.txt
--rw-r--r--   0 maxim      (502) staff       (20)      674 2023-08-14 14:33:28.000000 picnic-bio-1.0.0b2/src/files/models_llps/keys_llps_withoutgocattrue_92.txt
--rw-r--r--   0 maxim      (502) staff       (20)   968164 2023-08-14 14:33:28.000000 picnic-bio-1.0.0b2/src/files/models_llps/modelpipe_depth6class1_id_2_llps_withgonocc_retrained_newgo18.sav
--rw-r--r--   0 maxim      (502) staff       (20)  2346792 2023-08-14 14:33:28.000000 picnic-bio-1.0.0b2/src/files/models_llps/modelpipe_depth7class1_id_92_llps_withoutgo_24-02.sav
--rw-r--r--   0 maxim      (502) staff       (20)     4505 2023-10-12 14:21:39.000000 picnic-bio-1.0.0b2/src/main.py
-drwxr-xr-x   0 maxim      (502) staff       (20)        0 2023-12-14 10:49:03.113452 picnic-bio-1.0.0b2/src/prediction/
--rw-r--r--   0 maxim      (502) staff       (20)        0 2023-10-11 14:32:47.000000 picnic-bio-1.0.0b2/src/prediction/__init__.py
--rw-r--r--   0 maxim      (502) staff       (20)     2501 2023-10-11 14:32:47.000000 picnic-bio-1.0.0b2/src/prediction/calculation_pipeline.py
--rw-r--r--   0 maxim      (502) staff       (20)     3294 2023-10-11 14:32:47.000000 picnic-bio-1.0.0b2/src/prediction/create_model.py
--rw-r--r--   0 maxim      (502) staff       (20)     3955 2023-10-11 14:32:47.000000 picnic-bio-1.0.0b2/src/prediction/inference_model.py
+drwxr-xr-x   0 maxim      (502) staff       (20)        0 2024-04-16 07:06:22.212587 picnic_bio-1.0.0b3/
+-rw-r--r--   0 maxim      (502) staff       (20)     1514 2023-10-11 14:32:47.000000 picnic_bio-1.0.0b3/LICENSE
+-rw-r--r--   0 maxim      (502) staff       (20)     9662 2024-04-16 07:06:22.212250 picnic_bio-1.0.0b3/PKG-INFO
+-rw-r--r--   0 maxim      (502) staff       (20)    11501 2024-04-16 07:05:26.000000 picnic_bio-1.0.0b3/README.md
+drwxr-xr-x   0 maxim      (502) staff       (20)        0 2024-04-16 07:06:22.211485 picnic_bio-1.0.0b3/picnic_bio.egg-info/
+-rw-r--r--   0 maxim      (502) staff       (20)     9662 2024-04-16 07:06:22.000000 picnic_bio-1.0.0b3/picnic_bio.egg-info/PKG-INFO
+-rw-r--r--   0 maxim      (502) staff       (20)     1132 2024-04-16 07:06:22.000000 picnic_bio-1.0.0b3/picnic_bio.egg-info/SOURCES.txt
+-rw-r--r--   0 maxim      (502) staff       (20)        1 2024-04-16 07:06:22.000000 picnic_bio-1.0.0b3/picnic_bio.egg-info/dependency_links.txt
+-rw-r--r--   0 maxim      (502) staff       (20)       48 2024-04-16 07:06:22.000000 picnic_bio-1.0.0b3/picnic_bio.egg-info/entry_points.txt
+-rw-r--r--   0 maxim      (502) staff       (20)      103 2024-04-16 07:06:22.000000 picnic_bio-1.0.0b3/picnic_bio.egg-info/requires.txt
+-rw-r--r--   0 maxim      (502) staff       (20)       11 2024-04-16 07:06:22.000000 picnic_bio-1.0.0b3/picnic_bio.egg-info/top_level.txt
+-rw-r--r--   0 maxim      (502) staff       (20)      182 2023-10-11 14:32:47.000000 picnic_bio-1.0.0b3/pyproject.toml
+-rw-r--r--   0 maxim      (502) staff       (20)      528 2024-04-16 07:06:22.213392 picnic_bio-1.0.0b3/setup.cfg
+-rw-r--r--   0 maxim      (502) staff       (20)     2228 2024-04-16 06:01:58.000000 picnic_bio-1.0.0b3/setup.py
+drwxr-xr-x   0 maxim      (502) staff       (20)        0 2024-04-16 07:06:22.158036 picnic_bio-1.0.0b3/src/
+-rw-r--r--   0 maxim      (502) staff       (20)        0 2023-10-11 14:32:47.000000 picnic_bio-1.0.0b3/src/__init__.py
+-rw-r--r--   0 maxim      (502) staff       (20)     2607 2024-04-16 05:56:10.000000 picnic_bio-1.0.0b3/src/exceptions.py
+drwxr-xr-x   0 maxim      (502) staff       (20)        0 2024-04-16 07:06:22.163647 picnic_bio-1.0.0b3/src/features/
+-rw-r--r--   0 maxim      (502) staff       (20)        0 2023-10-11 14:32:47.000000 picnic_bio-1.0.0b3/src/features/__init__.py
+-rw-r--r--   0 maxim      (502) staff       (20)     1470 2024-01-24 08:48:42.000000 picnic_bio-1.0.0b3/src/features/calculation_disorder.py
+-rw-r--r--   0 maxim      (502) staff       (20)     2339 2024-01-17 16:35:26.000000 picnic_bio-1.0.0b3/src/features/goterms.py
+-rw-r--r--   0 maxim      (502) staff       (20)      918 2023-10-11 14:32:47.000000 picnic_bio-1.0.0b3/src/features/sequence_complexity.py
+-rw-r--r--   0 maxim      (502) staff       (20)     2571 2023-10-11 14:32:47.000000 picnic_bio-1.0.0b3/src/features/sequence_distance.py
+-rw-r--r--   0 maxim      (502) staff       (20)     8898 2024-04-16 06:01:58.000000 picnic_bio-1.0.0b3/src/features/sequence_structure_AF2.py
+drwxr-xr-x   0 maxim      (502) staff       (20)        0 2024-04-16 07:06:22.164604 picnic_bio-1.0.0b3/src/files/
+-rw-r--r--   0 maxim      (502) staff       (20)      285 2024-01-17 16:35:26.000000 picnic_bio-1.0.0b3/src/files/__init__.py
+drwxr-xr-x   0 maxim      (502) staff       (20)        0 2024-04-16 07:06:22.186647 picnic_bio-1.0.0b3/src/files/go/
+-rw-r--r--   0 maxim      (502) staff       (20)   628505 2023-08-14 14:33:27.000000 picnic_bio-1.0.0b3/src/files/go/bp_2500_freq.txt
+-rw-r--r--   0 maxim      (502) staff       (20)  3146152 2023-08-14 14:33:27.000000 picnic_bio-1.0.0b3/src/files/go/bp_2500_freq_all.json
+-rw-r--r--   0 maxim      (502) staff       (20)    91947 2023-08-14 14:33:27.000000 picnic_bio-1.0.0b3/src/files/go/cc_2000_freq.txt
+-rw-r--r--   0 maxim      (502) staff       (20)   263088 2023-08-14 14:33:27.000000 picnic_bio-1.0.0b3/src/files/go/cc_2000_freq_all.json
+-rw-r--r--   0 maxim      (502) staff       (20)   245749 2023-08-14 14:33:27.000000 picnic_bio-1.0.0b3/src/files/go/mf_2500_freq.txt
+-rw-r--r--   0 maxim      (502) staff       (20)   869522 2023-08-14 14:33:28.000000 picnic_bio-1.0.0b3/src/files/go/mf_2500_freq_all.json
+drwxr-xr-x   0 maxim      (502) staff       (20)        0 2024-04-16 07:06:22.200686 picnic_bio-1.0.0b3/src/files/models_llps/
+-rw-r--r--   0 maxim      (502) staff       (20)      157 2023-08-14 14:33:28.000000 picnic_bio-1.0.0b3/src/files/models_llps/keys_llps_withgonocc_retrained_newgo_18.txt
+-rw-r--r--   0 maxim      (502) staff       (20)      674 2023-08-14 14:33:28.000000 picnic_bio-1.0.0b3/src/files/models_llps/keys_llps_withoutgocattrue_92.txt
+-rw-r--r--   0 maxim      (502) staff       (20)   968164 2023-08-14 14:33:28.000000 picnic_bio-1.0.0b3/src/files/models_llps/modelpipe_depth6class1_id_2_llps_withgonocc_retrained_newgo18.sav
+-rw-r--r--   0 maxim      (502) staff       (20)  2346792 2023-08-14 14:33:28.000000 picnic_bio-1.0.0b3/src/files/models_llps/modelpipe_depth7class1_id_92_llps_withoutgo_24-02.sav
+-rw-r--r--   0 maxim      (502) staff       (20)     4517 2024-04-16 05:59:31.000000 picnic_bio-1.0.0b3/src/main.py
+drwxr-xr-x   0 maxim      (502) staff       (20)        0 2024-04-16 07:06:22.210725 picnic_bio-1.0.0b3/src/prediction/
+-rw-r--r--   0 maxim      (502) staff       (20)        0 2023-10-11 14:32:47.000000 picnic_bio-1.0.0b3/src/prediction/__init__.py
+-rw-r--r--   0 maxim      (502) staff       (20)     2508 2024-04-16 05:59:31.000000 picnic_bio-1.0.0b3/src/prediction/calculation_pipeline.py
+-rw-r--r--   0 maxim      (502) staff       (20)     3294 2023-10-11 14:32:47.000000 picnic_bio-1.0.0b3/src/prediction/create_model.py
+-rw-r--r--   0 maxim      (502) staff       (20)     8295 2024-04-16 05:59:31.000000 picnic_bio-1.0.0b3/src/prediction/inference_model.py
```

### Comparing `picnic-bio-1.0.0b2/LICENSE` & `picnic_bio-1.0.0b3/LICENSE`

 * *Files identical despite different names*

### Comparing `picnic-bio-1.0.0b2/README.md` & `picnic_bio-1.0.0b3/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 
 # Installation instructions
 
 A binary installer for the latest released version is available at the Python Package Index (PyPI).
 
 ## Requirements
 
-* Python version 3.10+
+* Python versions >=3.9,<3.12
 * Download and unpack IUPred2A
   * Add IUPred2A to PYTHONPATH
 * Download and unpack STRIDE
   * Add STRIDE binary to your system PATH
 
 
 ## Install external requirements
@@ -57,33 +57,35 @@
 $ tar -zxf iupred2a.tar.gz
 $ cd iupred2a
 $ export PYTHONPATH="$PWD"
 ```
 
 ## PICNIC is available on PyPI
 
+PICNIC officially supports Python versions >=3.9,<3.12.
+
 ```shell
-$ python -m pip install picnic_bio
+$ python3 --version
+Python 3.11.5
+$ python3 -m pip install picnic_bio
 ```
 
-PICNIC officially supports Python 3.10+.
-
 ## PICNIC is also installable from source
 
 ```shell
 $ git clone git@git.mpi-cbg.de:atplab/picnic.git
 ```
 
 Once you have a copy of the source, you can embed it in your own Python package, or install it into your site-packages easily
 
 ```shell
 $ cd picnic
 $ python3 -m venv picnic-env
-$source picnic-env/bin/activate
-(venv) $ python -m pip install .
+$ source picnic-env/bin/activate
+(picnic-env) $ python -m pip install .
 ```
 
 ## How to install PICNIC using Conda?
 
 There isn't any binary installer available on Conda yet. Though it is possible to install PICNIC within a virtual Conda environment.
 
 Please note that in a conda environment you have to pre-install catboost, before installing picnic-bio itself, otherwise the installation will fail when compiling the catboost package from source code. Also it is recommended to use and set up [conda-forge](https://conda-forge.org/docs/user/introduction.html) to fetch pre-compiled versions of catboost.
@@ -91,75 +93,121 @@
 Please also note that catboost=1.2.2 is incompatible with Python 3.12. The maintainers of catboost are working towards a fix right now.
 
 We have documented how to get around the catboost installation issue.
 
 ```shell
 $ conda config --add channels conda-forge
 $ conda config --set channel_priority strict
-$ conda create -n myenv python=[3.10, 3.11] catboost=1.2.2
+$ conda create -n myenv python=[3.9, 3.10, 3.11] catboost=1.2.2
 $ conda activate myenv
 (myenv) $ python -m pip install picnic_bio
 ```
 
 # How to use?
 
 ## Usage - Using PICNIC from command line
 
 ```
-$ picnic <is_automated> <path_af> <uniprot_id> <is_go> --path_fasta_file <file>
+$ picnic <is_automated> <path_af> <protein_id> <is_go> --path_fasta_file <file>
 
 usage: PICNIC [-h] [--path_fasta_file PATH_FASTA_FILE]
-              is_automated path_af uniprot_id is_go
+              is_automated path_af protein_id is_go
 
 PICNIC (Proteins Involved in CoNdensates In Cells) is a machine learning-based
 model that predicts proteins involved in biomolecular condensates.
 
 positional arguments:
   is_automated          True if automated pipeline (works for proteins with
                         length < 1400 aa, with precalculated Alphafold2 model,
                         deposited to UniprotKB), else manual pipeline
-                        (uniprot_id, Alphafold2 model(s) and fasta file are
+                        (protein_id, Alphafold2 model(s) and fasta file are
                         needed to be provided as input)
   path_af               directory with pdb files, created by Alphafold2 for
                         the protein in the format. For smaller proteins ( <
                         1400 aa length) AlphaFold2 provides one model, that
-                        should be named: AF-uniprot_id-F1-v{j}.pdb, where j is
+                        should be named: AF-protein_id-F1-v{j}.pdb, where j is
                         a version number. In case of large proteins Alphafold2
                         provides more than one file, and all of them should be
                         stored in one directory and named: 'AF-
-                        uniprot_id-F{i}-v{j}.pdb', where i is a number of
+                        protein_id-F{i}-v{j}.pdb', where i is a number of
                         model, j is a version number.
-  uniprot_id            protein identifier in UniprotKB (should correspond to
-                        the name 'uniprot_id' for Alphafold2 models, stored in
+  protein_id            protein identifier in UniprotKB (should correspond to
+                        the name 'protein_id' for Alphafold2 models, stored in
                         directory_af_models)
   is_go                 boolean flag; if 'True', picnic_go score (picnic
                         version with Gene Ontology features) will be
                         calculated, Gene Ontology terms are retrieved in this
-                        case from UniprotKB by uniprot_id identifier;
+                        case from UniprotKB by protein_id identifier;
                         otherwise default picnic score will be printed
                         (without Gene Ontology annotation)
 
 options:
   -h, --help            show this help message and exit
   --path_fasta_file PATH_FASTA_FILE
                         directory with sequence file in fasta format
 ```
 
 ## Examples
 
-Run automated pipeline:
+Run automated pipeline for a given UniProt Id:
 ```shell
 $ picnic True notebooks/test_files/Q99720/ Q99720 True
 ```
-Run manual pipeline:
+Run manual pipeline for a given UniProt Id:
 ```shell
 $ picnic False 'notebooks/test_files/O95613/' 'O95613' False --path_fasta_file 'notebooks/test_files/O95613/O95613.fasta.txt'
 ```
+Run manual pipeline for your own protein sequence called MY_PROTEIN, which has no reference to UniProt:
+```shell
+$ picnic False 'notebooks/test_files/MY_PROTEIN/' 'MY_PROTEIN' False --path_fasta_file 'notebooks/test_files/MY_PROTEIN/my_protein.fasta'
+```
 Examples of using PICNIC are shown in a jupyter-notebook in notebooks folder.
 
+## How to run the provided Jupyter notebook?
+
+Examples of how to use and run PICNIC are shown in a provided Jupyter notebook. The notebook can be found under the
+**notebooks** folder.
+
+### What is Jupyter Notebook?
+
+Please read documentation [here](https://saturncloud.io/blog/how-to-launch-jupyter-notebook-from-your-terminal/#what-is-jupyter-notebook).
+
+
+### How to create a virtual environment and install all required Python packages.
+
+Create a virtual environment by executing the command venv:
+```shell
+$ python -m venv /path/to/new/virtual/environment
+# e.g.
+$ python -m venv my_jupyter_env
+```
+
+Then install the classic Jupyter Notebook with:
+```shell
+$ source my_jupyter_env/bin/activate
+
+$ pip install notebook
+```
+Also install picnic-bio from source in the same virtual environment...
+```shell
+$ pip install .
+```
+
+### How to Launch Jupyter Notebook from Your Terminal?
+
+In your terminal source the previously created virtual environment...
+```shell
+$ source my_jupyter_env/bin/activate
+```
+Launch Jupyter Notebook...
+```shell
+$ jupyter notebook
+```
+Open the example notebook called 'picnic_examples.ipynb' under the notebooks folder.  
+
 # Link to paper
 
 [DOI: 10.1101/2023.06.01.543229](https://www.biorxiv.org/content/10.1101/2023.06.01.543229v2)
 
 # Development
 
 ## Getting started
@@ -207,15 +255,15 @@
 ```
 export COMPOSE_DOCKER_CLI_BUILD=1
 ```
 
 ## Building your Docker images
 
 ```shell
-$ docker build . -f Dockerfile -t atplab/picnic-service
+$ docker build --build-arg="PYTHON_VERSION=3.10.13" . -f Dockerfile -t atplab/picnic-service
 ```
 
 ### Run your image as a container
 
 ```shell
 $ docker run atplab/picnic-service
 
@@ -249,16 +297,16 @@
 ```shell
 (venv) % cd /<path-to-project-root-folder>/picnic
 
 (venv) % pip install .
 
 # Type in the picnic command to found out if the installation was successfully
 (venv) % picnic                                                                            
-usage: PICNIC [-h] [--path_fasta_file PATH_FASTA_FILE] is_automated path_af uniprot_id is_go
-PICNIC: error: the following arguments are required: is_automated, path_af, uniprot_id, is_go
+usage: PICNIC [-h] [--path_fasta_file PATH_FASTA_FILE] is_automated path_af protein_id is_go
+PICNIC: error: the following arguments are required: is_automated, path_af, protein_id, is_go
 ```
 
 ### How to build the PICNIC package from the project root directory?
 
 Run the following command from the root directory to build the package. This will create a dist 
 folder where the wheel distribution is built along with a zip file.
 ```shell
@@ -283,9 +331,8 @@
 ```
 
 
 ### How to deactivate the virtual environment?
 
 ```shell
 (packaging) $ deactivate
-```
-
+```
```

### Comparing `picnic-bio-1.0.0b2/picnic_bio.egg-info/SOURCES.txt` & `picnic_bio-1.0.0b3/picnic_bio.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `picnic-bio-1.0.0b2/setup.cfg` & `picnic_bio-1.0.0b3/setup.cfg`

 * *Files identical despite different names*

### Comparing `picnic-bio-1.0.0b2/setup.py` & `picnic_bio-1.0.0b3/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -5,15 +5,15 @@
     for line in fh:
         if line.startswith("# Development"):
             break
         long_description += line
 
 setuptools.setup(
     name="picnic-bio",
-    version="1.0.0-beta2",
+    version="1.0.0-beta3",
     author="Anna Hadarovich <hadarovi@mpi-cbg.de>, Maxim Scheremetjew <schereme@mpi-cbg.de>",
     author_email="picnic@cd-code.org",
     description="PICNIC (Proteins Involved in CoNdensates In Cells) is a machine learning-based model that predicts proteins involved in biomolecular condensates.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://picnic.cd-code.org/",
     project_urls={
@@ -27,22 +27,23 @@
         "Development Status :: 4 - Beta",
         "Intended Audience :: Science/Research",
         "License :: OSI Approved :: BSD License",
         "Topic :: Scientific/Engineering :: Bio-Informatics",
         "Programming Language :: Python",
         "Programming Language :: Python :: 3",
         "Programming Language :: Python :: 3 :: Only",
+        "Programming Language :: Python :: 3.9",
         "Programming Language :: Python :: 3.10",
         "Programming Language :: Python :: 3.11",
         "Operating System :: Unix",
         "Operating System :: MacOS",
     ],
     package_dir={"picnic_bio": "src"},
     package_data={"picnic_bio": ["files/models_llps/*", "files/iupred2a/data/*", "files/go/*"]},
-    python_requires=">=3.10",
+    python_requires=">=3.9",
     install_requires=[
         "requests ~=2.31.0",
         "catboost ==1.2.2",
         "matplotlib ~=3.7.2",
         "pandas ~=2.1.0",
         "Bio ~=1.5.2",
         "numpy ~=1.23.5",
```

### Comparing `picnic-bio-1.0.0b2/src/features/calculation_disorder.py` & `picnic_bio-1.0.0b3/src/features/calculation_disorder.py`

 * *Files identical despite different names*

### Comparing `picnic-bio-1.0.0b2/src/features/goterms.py` & `picnic_bio-1.0.0b3/src/features/goterms.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 import json
+from pathlib import Path
 
 import pandas as pd
 import requests
 
 from ..exceptions import NoGoAnnotationFoundError
 
 
@@ -28,31 +29,31 @@
                         go_terms.add(db["id"])
 
     if len(go_terms) == 0:
         raise NoGoAnnotationFoundError(uniprot_id=uniprot_id)
     return go_terms
 
 
-def calculate_3dir_go_one(uniprot_id: str, input_file_dir: str) -> dict:
+def calculate_3dir_go_one(uniprot_id: str, input_file_path: Path) -> dict:
 
     go = {}
     prot = {}
     go["go_terms_molecular_functions"] = "mf_2500_freq_all.json"
     go["go_terms_biological_processes"] = "bp_2500_freq_all.json"
     go["go_terms_cellular_component"] = "cc_2000_freq_all.json"
 
     go2 = {}
     go2["go_terms_molecular_functions"] = "mf_2500_freq.txt"
     go2["go_terms_biological_processes"] = "bp_2500_freq.txt"
     go2["go_terms_cellular_component"] = "cc_2000_freq.txt"
 
     for k, v in go.items():
-        mf = pd.read_csv(input_file_dir + go2[k], sep=" ")
+        mf = pd.read_csv(input_file_path / go2[k], sep=" ")
         mft = set(mf["num"])
-        with open(input_file_dir + v) as json_file:
+        with open(input_file_path / v) as json_file:
             mf = json.load(json_file)
         for kel in mft:
             prot[kel] = 0
 
         map_terms = mf
 
         translated = set()
```

### Comparing `picnic-bio-1.0.0b2/src/features/sequence_complexity.py` & `picnic_bio-1.0.0b3/src/features/sequence_complexity.py`

 * *Files identical despite different names*

### Comparing `picnic-bio-1.0.0b2/src/features/sequence_distance.py` & `picnic_bio-1.0.0b3/src/features/sequence_distance.py`

 * *Files identical despite different names*

### Comparing `picnic-bio-1.0.0b2/src/features/sequence_structure_AF2.py` & `picnic_bio-1.0.0b3/src/features/sequence_structure_AF2.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,13 +1,19 @@
 import collections
 import os
 
 import prody as pr
 import requests
 
+from ..exceptions import (
+    CouldNotDownloadAlphaFoldModelError,
+    CouldNotDownloadFASTAFileError,
+    NoAlphaFoldModelProvidedError,
+)
+
 
 def get_dict():
     aadict = {
         "A": 1,
         "G": 1,
         "V": 1,
         "M": 2,
@@ -41,17 +47,18 @@
     return d
 
 
 def produce_stride_output_af(af_models_path, name, stride_out_path):
 
     forstride = os.listdir(af_models_path)
     result = [i for i in forstride if (i.startswith("AF-" + name + "-") and i.endswith(".pdb"))]
+    if len(result) == 0:
+        raise NoAlphaFoldModelProvidedError(af_models_path)
     for f in result:
-        if f.endswith(".pdb"):
-            pr.execSTRIDE(af_models_path + f, outputname=f, outputdir=stride_out_path)
+        pr.execSTRIDE(af_models_path + f, outputname=f, outputdir=stride_out_path)
     return
 
 
 def get_ordered_dict(result):
     d = dict()
     for r in result:
         nummstr = r[:-13]
@@ -247,36 +254,37 @@
     produce_stride_output_af(af_models_path, uniprot_id, af_models_path)
     stride_af_annotation(af_models_path, [uniprot_id], af_models_path, af_models_path)
     af_fea = stride_af_triads_one(af_models_path, uniprot_id + "f.txt", af_models_path)
 
     return af_fea
 
 
-def get_af_model_from_api(uniprot_id: str, path_file) -> str:
+def send_request_and_write_content_to_file(url: str, file_path: str):
+    with open(file_path, "wb") as f:
+        response = requests.get(url)
+        response.raise_for_status()
+        f.write(response.content)
 
-    try:
-        url = f"https://alphafold.ebi.ac.uk/files/AF-{uniprot_id}-F1-model_v4.pdb"
-        full_path = f"{path_file}AF-{uniprot_id}-F1-model_v4.pdb"
-        with open(full_path, "wb") as f:
-            f.write(requests.get(url).content)
 
+def get_af_model_from_api(uniprot_id: str, path_file) -> str:
+    try:
+        url: str = f"https://alphafold.ebi.ac.uk/files/AF-{uniprot_id}-F1-model_v4.pdb"
+        file_path: str = f"{path_file}AF-{uniprot_id}-F1-model_v4.pdb"
+        send_request_and_write_content_to_file(url, file_path)
     except requests.exceptions.RequestException as err:
-        raise SystemExit(err)
-
-    return full_path
+        raise CouldNotDownloadAlphaFoldModelError(uniprot_id, err)
+    return file_path
 
 
 def get_fasta_from_api(uniprot_id: str, path_file) -> str:
 
     try:
         url = f"https://rest.uniprot.org/uniprotkb/{uniprot_id}.fasta"
-        full_path = f"{path_file}{uniprot_id}.fasta"
-        with open(full_path, "wb") as f:
-            f.write(requests.get(url).content)
+        file_path = f"{path_file}{uniprot_id}.fasta"
+        send_request_and_write_content_to_file(url, file_path)
     except requests.exceptions.RequestException as err:
-        raise SystemExit(err)
-
-    return full_path
+        raise CouldNotDownloadFASTAFileError(uniprot_id, err)
+    return file_path
 
 
 if __name__ == "__main__":
     print("Feature AF")  # noqa: T201
```

### Comparing `picnic-bio-1.0.0b2/src/files/go/bp_2500_freq.txt` & `picnic_bio-1.0.0b3/src/files/go/bp_2500_freq.txt`

 * *Files identical despite different names*

### Comparing `picnic-bio-1.0.0b2/src/files/go/bp_2500_freq_all.json` & `picnic_bio-1.0.0b3/src/files/go/bp_2500_freq_all.json`

 * *Files identical despite different names*

### Comparing `picnic-bio-1.0.0b2/src/files/go/cc_2000_freq.txt` & `picnic_bio-1.0.0b3/src/files/go/cc_2000_freq.txt`

 * *Files identical despite different names*

### Comparing `picnic-bio-1.0.0b2/src/files/go/cc_2000_freq_all.json` & `picnic_bio-1.0.0b3/src/files/go/cc_2000_freq_all.json`

 * *Files identical despite different names*

### Comparing `picnic-bio-1.0.0b2/src/files/go/mf_2500_freq.txt` & `picnic_bio-1.0.0b3/src/files/go/mf_2500_freq.txt`

 * *Files identical despite different names*

### Comparing `picnic-bio-1.0.0b2/src/files/go/mf_2500_freq_all.json` & `picnic_bio-1.0.0b3/src/files/go/mf_2500_freq_all.json`

 * *Files identical despite different names*

### Comparing `picnic-bio-1.0.0b2/src/files/models_llps/keys_llps_withoutgocattrue_92.txt` & `picnic_bio-1.0.0b3/src/files/models_llps/keys_llps_withoutgocattrue_92.txt`

 * *Files identical despite different names*

### Comparing `picnic-bio-1.0.0b2/src/files/models_llps/modelpipe_depth6class1_id_2_llps_withgonocc_retrained_newgo18.sav` & `picnic_bio-1.0.0b3/src/files/models_llps/modelpipe_depth6class1_id_2_llps_withgonocc_retrained_newgo18.sav`

 * *Files identical despite different names*

### Comparing `picnic-bio-1.0.0b2/src/files/models_llps/modelpipe_depth7class1_id_92_llps_withoutgo_24-02.sav` & `picnic_bio-1.0.0b3/src/files/models_llps/modelpipe_depth7class1_id_92_llps_withoutgo_24-02.sav`

 * *Files identical despite different names*

### Comparing `picnic-bio-1.0.0b2/src/main.py` & `picnic_bio-1.0.0b3/src/main.py`

 * *Files 2% similar despite different names*

```diff
@@ -76,24 +76,24 @@
     args = parser.parse_args()
     path_af = args.path_af
     is_automated = args.is_automated
     uniprot_id = args.uniprot_id
     isgo = args.is_go
     if is_automated == "True":
         if isgo == "True":
-            picnic_go = inference_model_with_go_one(path_af, path_af, uniprot_id, True)
+            picnic_go, _ = inference_model_with_go_one(path_af, path_af, uniprot_id, True)
             print("Automated pipeline: Picnic_go score for " + uniprot_id + " = " + str(picnic_go))  # noqa: T201
         else:
-            picnic = inference_model_without_go_one(path_af, path_af, uniprot_id, True)
+            picnic, _ = inference_model_without_go_one(path_af, path_af, uniprot_id, True)
             print("Automated pipeline: Picnic score for " + uniprot_id + " = " + str(picnic))  # noqa: T201
     else:
         fasta_dir = args.path_fasta_file
         if isgo == "True":
-            picnic_go = inference_model_with_go_one(fasta_dir, path_af, uniprot_id, False)
+            picnic_go, _ = inference_model_with_go_one(fasta_dir, path_af, uniprot_id, False)
             print("Manual pipeline: Picnic_go score for " + uniprot_id + " = " + str(picnic_go))  # noqa: T201
         else:
-            picnic = inference_model_without_go_one(fasta_dir, path_af, uniprot_id, False)
+            picnic, _ = inference_model_without_go_one(fasta_dir, path_af, uniprot_id, False)
             print("Manual pipeline: Picnic score for " + uniprot_id + " = " + str(picnic))  # noqa: T201
 
 
 if __name__ == "__main__":
     main()
```

### Comparing `picnic-bio-1.0.0b2/src/prediction/calculation_pipeline.py` & `picnic_bio-1.0.0b3/src/prediction/calculation_pipeline.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,71 +1,69 @@
 import os
+from pathlib import Path
 from typing import Optional
 
 from Bio import SeqIO
 
+from ..exceptions import CouldNotParseFASTAFileError
 from ..features.calculation_disorder import calculate_disorder_one
 from ..features.goterms import calculate_3dir_go_one
 from ..features.sequence_complexity import calculate_k40_k60_complexity_one
 from ..features.sequence_distance import calculate_dist_features_one
 from ..features.sequence_structure_AF2 import (
     calculate_sequence_structure_af_pipe_one_af,
     get_af_model_from_api,
     get_fasta_from_api,
 )
 
 
-def calculate_pipeline_one(path_af: str, name: str, input_fasta, go_flag=False, *args) -> dict:
+def calculate_pipeline_one(path_af: str, name: str, input_fasta, go_flag=False, go_folder_path: Path = None) -> dict:
 
     fasta_sequences = SeqIO.parse(open(input_fasta), "fasta")
     records = []
     for fasta in fasta_sequences:
         records.append(str(fasta.seq))
     sequence = records[0]
     d_af = calculate_sequence_structure_af_pipe_one_af(path_af, name)
     d_disorder = calculate_disorder_one(sequence)
     d_dist = calculate_dist_features_one(sequence)
     d_comp = calculate_k40_k60_complexity_one(sequence)
     if go_flag:
-        path_files = args[0]
-        d_go = calculate_3dir_go_one(name, path_files)
+        d_go = calculate_3dir_go_one(name, go_folder_path)
         allfea = {**d_disorder, **d_dist, **d_go, **d_comp, **d_af}
     else:
         allfea = {**d_disorder, **d_dist, **d_comp, **d_af}
 
     return allfea
 
 
-def calculate_pipeline_automated_one(path_output: str, name: str, go_flag=False, *args) -> Optional[dict]:
+def calculate_pipeline_automated_one(
+    path_output: str, name: str, go_flag=False, go_folder_path: Path = None
+) -> Optional[dict]:
     path_uni = os.path.join(path_output, name + "/")
     if not os.path.isdir(path_uni):
         os.mkdir(path_uni)
-    path_af = get_af_model_from_api(name, path_uni)
+    get_af_model_from_api(name, path_uni)
     input_fasta = get_fasta_from_api(name, path_uni)
-    if path_af is None:
-        return None
-    if input_fasta is None:
-        return None
     fasta_sequences = SeqIO.parse(open(input_fasta), "fasta")
     records = []
     for fasta in fasta_sequences:
         records.append(str(fasta.seq))
     if len(records) > 0:
         sequence = records[0]
         d_af = calculate_sequence_structure_af_pipe_one_af(path_uni, name)
         d_disorder = calculate_disorder_one(sequence)
         d_dist = calculate_dist_features_one(sequence)
         d_comp = calculate_k40_k60_complexity_one(sequence)
         if go_flag:
-            path_files = args[0]
-            d_go = calculate_3dir_go_one(name, path_files)
+            d_go = calculate_3dir_go_one(name, go_folder_path)
             allfea = {**d_disorder, **d_dist, **d_go, **d_comp, **d_af}
         else:
             allfea = {**d_disorder, **d_dist, **d_comp, **d_af}
 
         return allfea
     else:
-        return None
+        raise CouldNotParseFASTAFileError(input_fasta)
 
 
 if __name__ == "__main__":
     print("Calculate pipeline")  # noqa: T201
```

### Comparing `picnic-bio-1.0.0b2/src/prediction/create_model.py` & `picnic_bio-1.0.0b3/src/prediction/create_model.py`

 * *Files identical despite different names*

