# Comparing `tmp/gpas-1.0.1a1.tar.gz` & `tmp/gpas-1.0.1a2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gpas-1.0.1a1.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "gpas-1.0.1a2.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `gpas-1.0.1a1.tar` & `gpas-1.0.1a2.tar`

### file list

```diff
@@ -1,31 +1,32 @@
--rw-r--r--   0        0        0      649 2023-07-26 16:59:25.895776 gpas-1.0.1a1/.github/workflows/test.yml
--rw-r--r--   0        0        0     1818 2023-11-08 11:15:23.309795 gpas-1.0.1a1/.gitignore
--rw-r--r--   0        0        0      142 2023-12-04 08:36:19.634309 gpas-1.0.1a1/.pre-commit-config.yaml
--rw-r--r--   0        0        0      250 2024-02-22 12:09:35.580995 gpas-1.0.1a1/Dockerfile
--rw-r--r--   0        0        0     5788 2023-07-25 15:30:15.808992 gpas-1.0.1a1/LICENSE
--rw-r--r--   0        0        0     7198 2024-03-01 13:37:49.610007 gpas-1.0.1a1/README.md
--rw-r--r--   0        0        0      151 2024-01-25 00:55:55.049980 gpas-1.0.1a1/environment.yml
--rw-r--r--   0        0        0      601 2024-03-01 13:46:39.587834 gpas-1.0.1a1/pyproject.toml
--rw-r--r--   0        0        0       87 2024-03-01 13:55:58.280493 gpas-1.0.1a1/src/gpas/__init__.py
--rw-r--r--   0        0        0     5083 2024-02-26 15:55:55.700969 gpas-1.0.1a1/src/gpas/cli.py
--rw-r--r--   0        0        0    25073 2024-02-26 16:19:40.528047 gpas-1.0.1a1/src/gpas/lib.py
--rw-r--r--   0        0        0     5935 2024-02-21 15:52:53.858005 gpas-1.0.1a1/src/gpas/models.py
--rw-r--r--   0        0        0     6074 2024-03-01 13:49:25.784634 gpas-1.0.1a1/src/gpas/util.py
--rw-r--r--   0        0        0      380 2023-10-23 11:57:53.057433 gpas-1.0.1a1/tests/data/illumina-2.csv
--rw-r--r--   0        0        0      264 2023-12-12 12:55:05.470254 gpas-1.0.1a1/tests/data/illumina.csv
--rw-r--r--   0        0        0      263 2023-11-15 17:36:08.961007 gpas-1.0.1a1/tests/data/invalid/empty-sample-name.csv
--rw-r--r--   0        0        0      271 2023-12-21 21:57:36.218554 gpas-1.0.1a1/tests/data/invalid/invalid-control.csv
--rw-r--r--   0        0        0      273 2023-08-04 17:28:39.752858 gpas-1.0.1a1/tests/data/invalid/invalid-fastq-path.csv
--rw-r--r--   0        0        0      272 2023-12-21 21:57:36.218796 gpas-1.0.1a1/tests/data/invalid/invalid-instrument-platform.csv
--rw-r--r--   0        0        0      264 2023-12-21 21:57:36.219026 gpas-1.0.1a1/tests/data/invalid/invalid-specimen-organism.csv
--rw-r--r--   0        0        0      387 2023-12-21 21:57:36.219251 gpas-1.0.1a1/tests/data/invalid/mixed-instrument-platform.csv
--rw-r--r--   0        0        0      316 2023-12-21 21:57:36.219469 gpas-1.0.1a1/tests/data/ont-2.csv
--rw-r--r--   0        0        0      231 2023-12-21 21:57:36.219695 gpas-1.0.1a1/tests/data/ont.csv
--rw-r--r--   0        0        0      164 2023-07-06 18:18:11.924762 gpas-1.0.1a1/tests/data/reads/human_1_1.fastq.gz
--rw-r--r--   0        0        0      178 2023-07-06 18:18:11.925005 gpas-1.0.1a1/tests/data/reads/human_1_2.fastq.gz
--rw-r--r--   0        0        0      319 2023-07-23 12:01:36.874003 gpas-1.0.1a1/tests/data/reads/sars-cov-2_1_1.fastq
--rw-r--r--   0        0        0      319 2023-07-23 12:01:36.874201 gpas-1.0.1a1/tests/data/reads/sars-cov-2_1_2.fastq
--rw-r--r--   0        0        0      335 2023-07-06 18:18:11.925871 gpas-1.0.1a1/tests/data/reads/tuberculosis_1_1.fastq
--rw-r--r--   0        0        0      335 2023-07-06 18:18:11.926049 gpas-1.0.1a1/tests/data/reads/tuberculosis_1_2.fastq
--rw-r--r--   0        0        0     1845 2024-03-01 13:54:16.718201 gpas-1.0.1a1/tests/test_all.py
--rw-r--r--   0        0        0     7790 1970-01-01 00:00:00.000000 gpas-1.0.1a1/PKG-INFO
+-rw-r--r--   0        0        0      740 2024-04-15 08:18:53.470605 gpas-1.0.1a2/.github/workflows/test.yml
+-rw-r--r--   0        0        0     1818 2024-01-30 14:52:12.197255 gpas-1.0.1a2/.gitignore
+-rw-r--r--   0        0        0      142 2024-01-30 14:52:12.197255 gpas-1.0.1a2/.pre-commit-config.yaml
+-rw-r--r--   0        0        0      250 2024-04-15 09:41:27.960688 gpas-1.0.1a2/Dockerfile
+-rw-r--r--   0        0        0     5728 2024-04-11 12:26:08.345146 gpas-1.0.1a2/LICENSE
+-rw-r--r--   0        0        0     3353 2024-04-11 12:26:08.345146 gpas-1.0.1a2/README.md
+-rw-r--r--   0        0        0     5534 2024-04-11 12:26:08.345146 gpas-1.0.1a2/README_pypi.md
+-rw-r--r--   0        0        0      151 2024-04-15 09:40:34.752324 gpas-1.0.1a2/environment.yml
+-rw-r--r--   0        0        0      626 2024-04-15 09:27:24.638965 gpas-1.0.1a2/pyproject.toml
+-rw-r--r--   0        0        0       88 2024-04-15 09:50:58.384593 gpas-1.0.1a2/src/gpas/__init__.py
+-rw-r--r--   0        0        0     5477 2024-04-15 09:27:24.638965 gpas-1.0.1a2/src/gpas/cli.py
+-rw-r--r--   0        0        0    27235 2024-04-15 08:18:53.470605 gpas-1.0.1a2/src/gpas/lib.py
+-rw-r--r--   0        0        0     5893 2024-03-25 16:00:13.501404 gpas-1.0.1a2/src/gpas/models.py
+-rw-r--r--   0        0        0     8250 2024-04-15 09:28:07.455252 gpas-1.0.1a2/src/gpas/util.py
+-rw-r--r--   0        0        0      380 2024-01-30 14:52:12.201255 gpas-1.0.1a2/tests/data/illumina-2.csv
+-rw-r--r--   0        0        0      264 2024-01-30 14:52:12.201255 gpas-1.0.1a2/tests/data/illumina.csv
+-rw-r--r--   0        0        0      263 2024-01-30 14:52:12.201255 gpas-1.0.1a2/tests/data/invalid/empty-sample-name.csv
+-rw-r--r--   0        0        0      271 2024-01-30 14:52:12.201255 gpas-1.0.1a2/tests/data/invalid/invalid-control.csv
+-rw-r--r--   0        0        0      273 2024-01-30 14:52:12.201255 gpas-1.0.1a2/tests/data/invalid/invalid-fastq-path.csv
+-rw-r--r--   0        0        0      272 2024-01-30 14:52:12.201255 gpas-1.0.1a2/tests/data/invalid/invalid-instrument-platform.csv
+-rw-r--r--   0        0        0      264 2024-01-30 14:52:12.201255 gpas-1.0.1a2/tests/data/invalid/invalid-specimen-organism.csv
+-rw-r--r--   0        0        0      387 2024-01-30 14:52:12.201255 gpas-1.0.1a2/tests/data/invalid/mixed-instrument-platform.csv
+-rw-r--r--   0        0        0      316 2024-01-30 14:52:12.201255 gpas-1.0.1a2/tests/data/ont-2.csv
+-rw-r--r--   0        0        0      231 2024-01-30 14:52:12.201255 gpas-1.0.1a2/tests/data/ont.csv
+-rw-r--r--   0        0        0      164 2024-01-30 14:52:12.201255 gpas-1.0.1a2/tests/data/reads/human_1_1.fastq.gz
+-rw-r--r--   0        0        0      178 2024-01-30 14:52:12.201255 gpas-1.0.1a2/tests/data/reads/human_1_2.fastq.gz
+-rw-r--r--   0        0        0      319 2024-01-30 14:52:12.201255 gpas-1.0.1a2/tests/data/reads/sars-cov-2_1_1.fastq
+-rw-r--r--   0        0        0      319 2024-01-30 14:52:12.201255 gpas-1.0.1a2/tests/data/reads/sars-cov-2_1_2.fastq
+-rw-r--r--   0        0        0      335 2024-01-30 14:52:12.201255 gpas-1.0.1a2/tests/data/reads/tuberculosis_1_1.fastq
+-rw-r--r--   0        0        0      335 2024-01-30 14:52:12.201255 gpas-1.0.1a2/tests/data/reads/tuberculosis_1_2.fastq
+-rw-r--r--   0        0        0     2501 2024-04-15 09:27:24.638965 gpas-1.0.1a2/tests/test_all.py
+-rw-r--r--   0        0        0     6157 1970-01-01 00:00:00.000000 gpas-1.0.1a2/PKG-INFO
```

### Comparing `gpas-1.0.1a1/.github/workflows/test.yml` & `gpas-1.0.1a2/.github/workflows/test.yml`

 * *Files 22% similar despite different names*

```diff
@@ -1,9 +1,16 @@
 name: tests
-on: [push]
+on:
+  push:
+    branches:
+      - main
+  pull_request:
+    branches:
+      - '*'
+  workflow_dispatch:
 
 jobs:
   build:
     runs-on: ${{ matrix.os }}
     strategy:
       matrix:
         os: [ubuntu-22.04, macos-12]
```

### Comparing `gpas-1.0.1a1/.gitignore` & `gpas-1.0.1a2/.gitignore`

 * *Files identical despite different names*

### Comparing `gpas-1.0.1a1/LICENSE` & `gpas-1.0.1a2/LICENSE`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 LICENCE TERMS FOR ACCESS TO SOFTWARE AND DATABASE FOR ACADEMIC USE
 
 These licence terms apply to all licences granted by THE CHANCELLOR, MASTERS AND SCHOLARS OF THE UNIVERSITY
 OF OXFORD whose administrative offices are at University Offices, Wellington Square, Oxford OX1 2JD,
-United Kingdom (the “University”) for use of or access to the gpas-cli software ("the Software")
-through this website https://github.com/GlobalPathogenAnalysisService/gpas-cli (the "Website").
+United Kingdom (the “University”) for use of or access to the client software ("the Software")
+through this website (the "Website").
 
 PLEASE READ THESE LICENCE TERMS CAREFULLY BEFORE USING THE SOFTWARE THROUGH THIS WEBSITE.
 IF YOU DO NOT AGREE TO THESE LICENCE TERMS YOU SHOULD NOT USE THE SOFTWARE.
 
 THIS WEBSITE AND THE SOFTWARE ARE INTENDED FOR ACADEMICS CARRYING OUT RESEARCH AND NOT FOR USE
 BY CONSUMERS OR COMMERCIAL BUSINESSES.
```

### Comparing `gpas-1.0.1a1/README.md` & `gpas-1.0.1a2/README_pypi.md`

 * *Files 19% similar despite different names*

```diff
@@ -153,100 +153,7 @@
 The human genome index used for host decontamination is downloaded automatically when running `gpas upload` for the first time. You may trigger this manually ahead of upload with `gpas download-index`.
 
 
 
 ## Support
 
 For technical support, please open an issue or contact `support@gpas.global`
-
-
-
-***
-
-
-
-## Development
-
-**Development install**
-
-```bash
-git clone https://github.com/GlobalPathogenAnalysisService/cli.git
-cd cli
-conda env create -y -f environment.yml
-pip install --editable '.[dev]'
-pre-commit install
-```
-
-**Updating**
-
-```bash
-git pull origin main
-gpas --version
-```
-
-
-
-### Using an alternate host
-
-1. The stateless way (use `--host` with every command):
-   ```bash
-   gpas auth --host dev.portal.gpas.world
-   gpas upload samples.csv --host dev.portal.gpas.world
-   ```
-
-2. The stateful way (no need to use `--host` with each command):
-   ```bash
-   export GPAS_HOST="dev.portal.gpas.world"
-   ```
-
-   Then, as usual:
-   ```bash
-   gpas auth
-   gpas upload samples.csv
-   ```
-
-   To reset:
-   ```bash
-   unset GPAS_HOST
-   ```
-
-
-
-### Installing a pre-release version
-
-```bash
-conda create --yes -n gpas -c conda-forge -c bioconda hostile
-conda activate gpas
-pip install --pre gpas
-```
-
-
-
-### Using a local development server
-
-```bash
-export GPAS_HOST="localhost:8000"
-export GPAS_PROTOCOL="http"
-```
-To unset:
-```bash
-unset GPAS_HOST
-unset GPAS_PROTOCOL
-```
-
-
-
-### Releasing a new version
-
-Having installed an editable [development environment](https://github.com/GlobalPathogenAnalysisService/client?tab=readme-ov-file#development) (with pre-commit, pytest and flit):
-
-```bash
-pytest
-# Bump version strings inside src/gpas/__init__.py AND Dockerfile
-# Use format e.g. 1.0.0a1 for pre-releases (following example of Pydantic)
-git tag 0.0.0. # e.g.
-git push origin main --tags
-flit build  # Build package
-flit publish  # Authenticate and upload package to PyPI
-# Announce in Slack CLI channel
-# PR gpas/gpas/settings.py with new version
-```
```

### Comparing `gpas-1.0.1a1/pyproject.toml` & `gpas-1.0.1a2/pyproject.toml`

 * *Files 20% similar despite different names*

```diff
@@ -2,24 +2,25 @@
 requires = ["flit_core >=3.2,<4"]
 build-backend = "flit_core.buildapi"
 
 [project]
 name = "gpas"
 authors = [{name = "Bede Constantinides", email = "bedeabc@gmail.com"}]
 license = {file = "LICENSE"}
-readme = "README.md"
+readme = "README_pypi.md"
 dynamic = ["version", "description"]
 requires-python = ">=3.10"
 dependencies = [
   "defopt==6.4.0",
   "httpx>=0.27.0",
   "packaging>=23.2",
   "platformdirs>=3.9.1,<=4.2.0",
   "tqdm==4.66.2",
   "pydantic>=2.6.2,<3",
+  "tenacity==8.2.3"
 ]
 
 [project.scripts]
 gpas = "gpas.cli:main"
 
 [project.optional-dependencies]
 dev = [
```

### Comparing `gpas-1.0.1a1/src/gpas/cli.py` & `gpas-1.0.1a2/src/gpas/cli.py`

 * *Files 5% similar despite different names*

```diff
@@ -147,20 +147,33 @@
 def download_index() -> None:
     """
     Download and cache host decontamination index.
     """
     lib.download_index()
 
 
+def validate(upload_csv: Path, *, host: str | None = None, debug: bool = False) -> None:
+    """Validate a given upload CSV.
+
+    :arg upload_csv: Path of upload csv
+    :arg host: API hostname
+    :arg debug: Enable verbose debug messages
+    """
+    util.configure_debug_logging(debug)
+    host = lib.get_host(host)
+    lib.validate(upload_csv, host=host)
+
+
 def main() -> None:
     defopt.run(
         {
             "auth": auth,
             "upload": upload,
             "download": download,
             "download-index": download_index,
             "query": {"raw": query_raw, "status": query_status},
+            "validate": validate,
         },
         no_negated_flags=True,
         strict_kwonly=True,
         short={},
     )
```

### Comparing `gpas-1.0.1a1/src/gpas/lib.py` & `gpas-1.0.1a2/src/gpas/lib.py`

 * *Files 4% similar despite different names*

```diff
@@ -3,16 +3,18 @@
 import logging
 import os
 
 from pathlib import Path
 
 import httpx
 
+from tenacity import retry, wait_random_exponential, stop_after_attempt
+
 from hostile.lib import ALIGNER, clean_fastqs, clean_paired_fastqs
-from hostile.util import BUCKET_URL, XDG_DATA_DIR
+from hostile.util import BUCKET_URL, CACHE_DIR
 
 from packaging.version import Version
 from pydantic import BaseModel
 from tqdm import tqdm
 
 import gpas
 import hostile
@@ -23,14 +25,27 @@
 logging.getLogger("httpx").setLevel(logging.WARNING)
 
 DEFAULT_HOST = "research.portal.gpas.world"
 DEFAULT_PROTOCOL = "https"
 HOSTILE_INDEX_NAME = "human-t2t-hla-argos985-mycob140"
 
 
+class InvalidPathError(Exception):
+    """Custom exception for giving nice user errors around missing paths."""
+
+    def __init__(self, message: str):
+        """Constructor, used to pass a custom message to user.
+
+        Args:
+            message (str): Message about this path
+        """
+        self.message = message
+        super().__init__(self.message)
+
+
 def get_host(cli_host: str | None) -> str:
     """Return hostname using 1) CLI argument, 2) environment variable, 3) default value"""
     if cli_host:
         return cli_host
     elif "GPAS_HOST" in os.environ:
         env_host = os.environ["GPAS_HOST"]
         return env_host
@@ -86,24 +101,25 @@
             "version": hostile.__version__,
         },
     }
     data = {"telemetry_data": telemetry_data}
     with httpx.Client(
         event_hooks=util.httpx_hooks,
         transport=httpx.HTTPTransport(retries=5),
-        timeout=10,
+        timeout=60,
     ) as client:
         response = client.post(
             f"{get_protocol()}://{host}/api/v1/batches",
             headers={"Authorization": f"Bearer {util.get_access_token(host)}"},
             json=data,
         )
     return response.json()["id"], response.json()["name"]
 
 
+@retry(wait=wait_random_exponential(multiplier=2, max=60), stop=stop_after_attempt(10))
 def create_sample(
     host: str,
     batch_id: str,
     collection_date: str,
     control: bool | None,
     country: str,
     subdivision: str,
@@ -131,30 +147,35 @@
         "checksum": checksum,
         "instrument_platform": instrument_platform,
         "specimen_organism": specimen_organism,
         "host_organism": host_organism,
     }
     headers = {"Authorization": f"Bearer {util.get_access_token(host)}"}
     logging.debug(f"Sample {data=}")
-    with httpx.Client(event_hooks=util.httpx_hooks) as client:
+    with httpx.Client(
+        event_hooks=util.httpx_hooks,
+        transport=httpx.HTTPTransport(retries=5),
+        timeout=60,
+    ) as client:
         response = client.post(
             f"{get_protocol()}://{host}/api/v1/samples",
             headers=headers,
             json=data,
         )
     return response.json()["id"]
 
 
+@retry(wait=wait_random_exponential(multiplier=2, max=60), stop=stop_after_attempt(10))
 def run_sample(sample_id: str, host: str) -> str:
     """Patch sample status, create run, and patch run status to trigger processing"""
     headers = {"Authorization": f"Bearer {util.get_access_token(host)}"}
     with httpx.Client(
         event_hooks=util.httpx_hooks,
         transport=httpx.HTTPTransport(retries=5),
-        timeout=10,
+        timeout=30,
     ) as client:
         client.patch(
             f"{get_protocol()}://{host}/api/v1/samples/{sample_id}",
             headers=headers,
             json={"status": "Ready"},
         )
         post_run_response = client.post(
@@ -200,14 +221,29 @@
             f"{get_protocol()}://{host}/api/v1/batches/validate",
             headers=headers,
             json=data,
         )
     logging.debug(f"{response.json()=}")
 
 
+def validate(upload_csv: Path, host: str = DEFAULT_HOST) -> None:
+    """Validate a given upload CSV and exit.
+
+    Args:
+        upload_csv (Path): Path to the upload CSV
+        host (str, optional): Name of the host to validate against. Defaults to DEFAULT_HOST.
+    """
+    logging.info(f"GPAS client version {gpas.__version__} ({host})")
+    logging.debug("validate()")
+    upload_csv = Path(upload_csv)
+    batch = models.parse_upload_csv(upload_csv)
+    validate_batch(batch=batch, host=host)
+    logging.info(f"Successfully validated {upload_csv}!")
+
+
 def upload(
     upload_csv: Path,
     save: bool = False,
     threads: int | None = None,
     host: str = DEFAULT_HOST,
     dry_run: bool = False,
 ) -> None:
@@ -451,15 +487,18 @@
                 pass  # A failure here doesn't matter since upload is complete
     logging.info(f"Upload complete. Created {batch_name}.mapping.csv (keep this safe)")
 
 
 def fetch_sample(sample_id: str, host: str) -> dict:
     """Fetch sample data from server"""
     headers = {"Authorization": f"Bearer {util.get_access_token(host)}"}
-    with httpx.Client(event_hooks=util.httpx_hooks) as client:
+    with httpx.Client(
+        event_hooks=util.httpx_hooks,
+        transport=httpx.HTTPTransport(retries=5),
+    ) as client:
         response = client.get(
             f"{get_protocol()}://{host}/api/v1/samples/{sample_id}",
             headers=headers,
         )
     return response.json()
 
 
@@ -518,15 +557,18 @@
         samples_status[name] = fetch_sample(sample_id=guid, host=host).get("status")
     return samples_status
 
 
 def fetch_latest_input_files(sample_id: str, host: str) -> dict[str, models.RemoteFile]:
     """Return models.RemoteFile instances for a sample input files"""
     headers = {"Authorization": f"Bearer {util.get_access_token(host)}"}
-    with httpx.Client(event_hooks=util.httpx_hooks) as client:
+    with httpx.Client(
+        event_hooks=util.httpx_hooks,
+        transport=httpx.HTTPTransport(retries=5),
+    ) as client:
         response = client.get(
             f"{get_protocol()}://{host}/api/v1/samples/{sample_id}/latest/input-files",
             headers=headers,
         )
     data = response.json().get("files", [])
     output_files = {
         d["filename"]: models.RemoteFile(
@@ -541,15 +583,18 @@
 
 
 def fetch_output_files(
     sample_id: str, host: str, latest: bool = True
 ) -> dict[str, models.RemoteFile]:
     """Return models.RemoteFile instances for a sample, optionally including only latest run"""
     headers = {"Authorization": f"Bearer {util.get_access_token(host)}"}
-    with httpx.Client(event_hooks=util.httpx_hooks) as client:
+    with httpx.Client(
+        event_hooks=util.httpx_hooks,
+        transport=httpx.HTTPTransport(retries=5),
+    ) as client:
         response = client.get(
             f"{get_protocol()}://{host}/api/v1/samples/{sample_id}/latest/files",
             headers=headers,
         )
     data = response.json().get("files", [])
     output_files = {
         d["filename"]: models.RemoteFile(
@@ -668,40 +713,61 @@
                         filename=filename_fmt,
                         url=url,
                         headers=headers,
                         out_dir=Path(out_dir),
                     )
 
 
+@retry(wait=wait_random_exponential(multiplier=2, max=60), stop=stop_after_attempt(10))
 def download_single(
     client: httpx.Client,
     url: str,
     filename: str,
     headers: dict[str, str],
     out_dir: Path,
 ):
     logging.info(f"Downloading {filename}")
+    check_outdir(out_dir)
     with client.stream("GET", url=url, headers=headers) as r:
         file_size = int(r.headers.get("content-length", 0))
         progress = tqdm(
             total=file_size, unit="B", unit_scale=True, desc=filename, leave=False
         )
         chunk_size = 262_144
-        with Path(out_dir).joinpath(f"{filename}").open("wb") as fh, tqdm(
-            total=file_size,
-            unit="B",
-            unit_scale=True,
-            desc=filename,
-            leave=False,  # Works only if using a context manager
-            position=0,  # Avoids leaving line break with leave=False
-        ) as progress:
+        with (
+            Path(out_dir).joinpath(f"{filename}").open("wb") as fh,
+            tqdm(
+                total=file_size,
+                unit="B",
+                unit_scale=True,
+                desc=filename,
+                leave=False,  # Works only if using a context manager
+                position=0,  # Avoids leaving line break with leave=False
+            ) as progress,
+        ):
             for data in r.iter_bytes(chunk_size):
                 fh.write(data)
                 progress.update(len(data))
     logging.debug(f"Downloaded {filename}")
 
 
 def download_index(name: str = HOSTILE_INDEX_NAME) -> None:
-    logging.info(f"Cache directory: {XDG_DATA_DIR}")
+    logging.info(f"Cache directory: {CACHE_DIR}")
     logging.info(f"Manifest URL: {BUCKET_URL}/manifest.json")
     ALIGNER.minimap2.value.check_index(name)
     ALIGNER.bowtie2.value.check_index(name)
+
+
+def check_outdir(path: Path) -> None:
+    """Given an outdir path, check that it exists (and is a directory).
+
+    Args:
+        path (Path): Outdir path
+    """
+    if path.exists():
+        if path.is_dir():
+            return
+        logging.error(f"Given out dir ({str(path)}) exists, but is a file!")
+        raise InvalidPathError(f"Given out dir ({str(path)}) exists, but is a file!")
+
+    logging.error(f"Given out dir ({str(path)}) does not exist!")
+    raise InvalidPathError(f"Given out dir ({str(path)}) does not exist!")
```

### Comparing `gpas-1.0.1a1/src/gpas/models.py` & `gpas-1.0.1a2/src/gpas/models.py`

 * *Files 0% similar despite different names*

```diff
@@ -7,18 +7,17 @@
 from gpas import util
 
 
 ALLOWED_EXTENSIONS = (".fastq", ".fq", ".fastq.gz", ".fq.gz")
 
 
 def validate_file_extension(
-    filename: str, allowed_extensions: list = ALLOWED_EXTENSIONS
+    filename: str, allowed_extensions: tuple[str] = ALLOWED_EXTENSIONS
 ):
-    filename = str(filename)
-    return True if filename.endswith(allowed_extensions) else False
+    return filename.endswith(allowed_extensions)
 
 
 class UploadSample(BaseModel):
     batch_name: str = Field(
         default=None, description="Batch name (anonymised prior to upload)"
     )
     sample_name: str = Field(
```

### Comparing `gpas-1.0.1a1/PKG-INFO` & `gpas-1.0.1a2/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,20 +1,21 @@
 Metadata-Version: 2.1
 Name: gpas
-Version: 1.0.1a1
+Version: 1.0.1a2
 Summary: The command line and Python client for the GPAS platform
 Author-email: Bede Constantinides <bedeabc@gmail.com>
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 Requires-Dist: defopt==6.4.0
 Requires-Dist: httpx>=0.27.0
 Requires-Dist: packaging>=23.2
 Requires-Dist: platformdirs>=3.9.1,<=4.2.0
 Requires-Dist: tqdm==4.66.2
 Requires-Dist: pydantic>=2.6.2,<3
+Requires-Dist: tenacity==8.2.3
 Requires-Dist: pytest>=8.0.2   ; extra == "dev"
 Requires-Dist: pre-commit>=3.6.2 ; extra == "dev"
 Requires-Dist: flit>=3.9.0 ; extra == "dev"
 Provides-Extra: dev
 
 # GPAS client
 
@@ -172,100 +173,7 @@
 
 
 
 ## Support
 
 For technical support, please open an issue or contact `support@gpas.global`
 
-
-
-***
-
-
-
-## Development
-
-**Development install**
-
-```bash
-git clone https://github.com/GlobalPathogenAnalysisService/cli.git
-cd cli
-conda env create -y -f environment.yml
-pip install --editable '.[dev]'
-pre-commit install
-```
-
-**Updating**
-
-```bash
-git pull origin main
-gpas --version
-```
-
-
-
-### Using an alternate host
-
-1. The stateless way (use `--host` with every command):
-   ```bash
-   gpas auth --host dev.portal.gpas.world
-   gpas upload samples.csv --host dev.portal.gpas.world
-   ```
-
-2. The stateful way (no need to use `--host` with each command):
-   ```bash
-   export GPAS_HOST="dev.portal.gpas.world"
-   ```
-
-   Then, as usual:
-   ```bash
-   gpas auth
-   gpas upload samples.csv
-   ```
-
-   To reset:
-   ```bash
-   unset GPAS_HOST
-   ```
-
-
-
-### Installing a pre-release version
-
-```bash
-conda create --yes -n gpas -c conda-forge -c bioconda hostile
-conda activate gpas
-pip install --pre gpas
-```
-
-
-
-### Using a local development server
-
-```bash
-export GPAS_HOST="localhost:8000"
-export GPAS_PROTOCOL="http"
-```
-To unset:
-```bash
-unset GPAS_HOST
-unset GPAS_PROTOCOL
-```
-
-
-
-### Releasing a new version
-
-Having installed an editable [development environment](https://github.com/GlobalPathogenAnalysisService/client?tab=readme-ov-file#development) (with pre-commit, pytest and flit):
-
-```bash
-pytest
-# Bump version strings inside src/gpas/__init__.py AND Dockerfile
-# Use format e.g. 1.0.0a1 for pre-releases (following example of Pydantic)
-git tag 0.0.0. # e.g.
-git push origin main --tags
-flit build  # Build package
-flit publish  # Authenticate and upload package to PyPI
-# Announce in Slack CLI channel
-# PR gpas/gpas/settings.py with new version
-```
-
```

