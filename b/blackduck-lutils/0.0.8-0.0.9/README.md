# Comparing `tmp/blackduck_lutils-0.0.8.tar.gz` & `tmp/blackduck_lutils-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, last modified: Sun Feb  2 00:00:00 2020, max compression, original size modulo 2^32 423086080 gzip compressed data, reserved method, ASCII, extra field, has comment, encrypted, from FAT filesystem (MS-DOS, OS/2, NT)
+gzip compressed data, last modified: Sun Feb  2 00:00:00 2020, max compression, original size modulo 2^32 423086080 gzip compressed data, reserved method, has CRC, extra field, has comment, encrypted, from FAT filesystem (MS-DOS, OS/2, NT)
```

## Comparing `blackduck_lutils-0.0.8.tar` & `blackduck_lutils-0.0.9.tar`

### file list

```diff
@@ -1,21 +1,21 @@
--rw-r--r--   0        0        0 86615273 2020-02-02 00:00:00.000000 blackduck_lutils-0.0.8/LicenseConflictTest_LATEST_2024-03-26_164031.csv
--rw-r--r--   0        0        0 86615273 2020-02-02 00:00:00.000000 blackduck_lutils-0.0.8/LicenseConflictTest_LATEST_2024-03-26_164829.csv
--rw-r--r--   0        0        0 86609833 2020-02-02 00:00:00.000000 blackduck_lutils-0.0.8/LicenseConflictTest_LATEST_2024-04-15_084450.csv
--rw-r--r--   0        0        0 74230649 2020-02-02 00:00:00.000000 blackduck_lutils-0.0.8/LicenseConflictTest_LATEST_2024-04-15_103052.csv
--rw-r--r--   0        0        0      262 2020-02-02 00:00:00.000000 blackduck_lutils-0.0.8/environ.sh
--rw-r--r--   0        0        0 15841961 2020-02-02 00:00:00.000000 blackduck_lutils-0.0.8/license_data.json
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 blackduck_lutils-0.0.8/matched
--rw-r--r--   0        0        0 72658599 2020-02-02 00:00:00.000000 blackduck_lutils-0.0.8/nginx.log
--rw-r--r--   0        0        0       73 2020-02-02 00:00:00.000000 blackduck_lutils-0.0.8/process.txt
--rw-r--r--   0        0        0       28 2020-02-02 00:00:00.000000 blackduck_lutils-0.0.8/requirements.txt
--rw-r--r--   0        0        0   418653 2020-02-02 00:00:00.000000 blackduck_lutils-0.0.8/sample.json
--rw-r--r--   0        0        0       20 2020-02-02 00:00:00.000000 blackduck_lutils-0.0.8/src/blackduck_lutils/__about__.py
--rw-r--r--   0        0        0    20028 2020-02-02 00:00:00.000000 blackduck_lutils-0.0.8/src/blackduck_lutils/license_conflicts.py
--rw-r--r--   0        0        0    12617 2020-02-02 00:00:00.000000 blackduck_lutils-0.0.8/src/blackduck_lutils/license_tagging.py
--rw-r--r--   0        0        0     2348 2020-02-02 00:00:00.000000 blackduck_lutils-0.0.8/tests/test_download_license_data.py
--rw-r--r--   0        0        0     2844 2020-02-02 00:00:00.000000 blackduck_lutils-0.0.8/tests/test_license_conflicts.py
--rw-r--r--   0        0        0       75 2020-02-02 00:00:00.000000 blackduck_lutils-0.0.8/tests/test_license_tagging.py
--rw-r--r--   0        0        0    11357 2020-02-02 00:00:00.000000 blackduck_lutils-0.0.8/LICENSE
--rw-r--r--   0        0        0    10135 2020-02-02 00:00:00.000000 blackduck_lutils-0.0.8/README.md
--rw-r--r--   0        0        0     2244 2020-02-02 00:00:00.000000 blackduck_lutils-0.0.8/pyproject.toml
--rw-r--r--   0        0        0    11173 2020-02-02 00:00:00.000000 blackduck_lutils-0.0.8/PKG-INFO
+-rw-r--r--   0        0        0 86615273 2020-02-02 00:00:00.000000 blackduck_lutils-0.0.9/LicenseConflictTest_LATEST_2024-03-26_164031.csv
+-rw-r--r--   0        0        0 86615273 2020-02-02 00:00:00.000000 blackduck_lutils-0.0.9/LicenseConflictTest_LATEST_2024-03-26_164829.csv
+-rw-r--r--   0        0        0 86609833 2020-02-02 00:00:00.000000 blackduck_lutils-0.0.9/LicenseConflictTest_LATEST_2024-04-15_084450.csv
+-rw-r--r--   0        0        0 74230649 2020-02-02 00:00:00.000000 blackduck_lutils-0.0.9/LicenseConflictTest_LATEST_2024-04-15_103052.csv
+-rw-r--r--   0        0        0      262 2020-02-02 00:00:00.000000 blackduck_lutils-0.0.9/environ.sh
+-rw-r--r--   0        0        0 15841961 2020-02-02 00:00:00.000000 blackduck_lutils-0.0.9/license_data.json
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 blackduck_lutils-0.0.9/matched
+-rw-r--r--   0        0        0 72658599 2020-02-02 00:00:00.000000 blackduck_lutils-0.0.9/nginx.log
+-rw-r--r--   0        0        0       73 2020-02-02 00:00:00.000000 blackduck_lutils-0.0.9/process.txt
+-rw-r--r--   0        0        0       28 2020-02-02 00:00:00.000000 blackduck_lutils-0.0.9/requirements.txt
+-rw-r--r--   0        0        0   418653 2020-02-02 00:00:00.000000 blackduck_lutils-0.0.9/sample.json
+-rw-r--r--   0        0        0       20 2020-02-02 00:00:00.000000 blackduck_lutils-0.0.9/src/blackduck_lutils/__about__.py
+-rw-r--r--   0        0        0    20028 2020-02-02 00:00:00.000000 blackduck_lutils-0.0.9/src/blackduck_lutils/license_conflicts.py
+-rw-r--r--   0        0        0    12617 2020-02-02 00:00:00.000000 blackduck_lutils-0.0.9/src/blackduck_lutils/license_tagging.py
+-rw-r--r--   0        0        0     2348 2020-02-02 00:00:00.000000 blackduck_lutils-0.0.9/tests/test_download_license_data.py
+-rw-r--r--   0        0        0     2844 2020-02-02 00:00:00.000000 blackduck_lutils-0.0.9/tests/test_license_conflicts.py
+-rw-r--r--   0        0        0       75 2020-02-02 00:00:00.000000 blackduck_lutils-0.0.9/tests/test_license_tagging.py
+-rw-r--r--   0        0        0    11357 2020-02-02 00:00:00.000000 blackduck_lutils-0.0.9/LICENSE
+-rw-r--r--   0        0        0    10114 2020-02-02 00:00:00.000000 blackduck_lutils-0.0.9/README.md
+-rw-r--r--   0        0        0     2279 2020-02-02 00:00:00.000000 blackduck_lutils-0.0.9/pyproject.toml
+-rw-r--r--   0        0        0    11225 2020-02-02 00:00:00.000000 blackduck_lutils-0.0.9/PKG-INFO
```

### Comparing `blackduck_lutils-0.0.8/LicenseConflictTest_LATEST_2024-03-26_164031.csv` & `blackduck_lutils-0.0.9/LicenseConflictTest_LATEST_2024-03-26_164031.csv`

 * *Files identical despite different names*

### Comparing `blackduck_lutils-0.0.8/LicenseConflictTest_LATEST_2024-03-26_164829.csv` & `blackduck_lutils-0.0.9/LicenseConflictTest_LATEST_2024-03-26_164829.csv`

 * *Files identical despite different names*

### Comparing `blackduck_lutils-0.0.8/LicenseConflictTest_LATEST_2024-04-15_084450.csv` & `blackduck_lutils-0.0.9/LicenseConflictTest_LATEST_2024-04-15_084450.csv`

 * *Files identical despite different names*

### Comparing `blackduck_lutils-0.0.8/LicenseConflictTest_LATEST_2024-04-15_103052.csv` & `blackduck_lutils-0.0.9/LicenseConflictTest_LATEST_2024-04-15_103052.csv`

 * *Files identical despite different names*

### Comparing `blackduck_lutils-0.0.8/license_data.json` & `blackduck_lutils-0.0.9/license_data.json`

 * *Files identical despite different names*

### Comparing `blackduck_lutils-0.0.8/nginx.log` & `blackduck_lutils-0.0.9/nginx.log`

 * *Files identical despite different names*

### Comparing `blackduck_lutils-0.0.8/sample.json` & `blackduck_lutils-0.0.9/sample.json`

 * *Files identical despite different names*

### Comparing `blackduck_lutils-0.0.8/src/blackduck_lutils/license_conflicts.py` & `blackduck_lutils-0.0.9/src/blackduck_lutils/license_conflicts.py`

 * *Files identical despite different names*

### Comparing `blackduck_lutils-0.0.8/src/blackduck_lutils/license_tagging.py` & `blackduck_lutils-0.0.9/src/blackduck_lutils/license_tagging.py`

 * *Files identical despite different names*

### Comparing `blackduck_lutils-0.0.8/tests/test_download_license_data.py` & `blackduck_lutils-0.0.9/tests/test_download_license_data.py`

 * *Files identical despite different names*

### Comparing `blackduck_lutils-0.0.8/tests/test_license_conflicts.py` & `blackduck_lutils-0.0.9/tests/test_license_conflicts.py`

 * *Files identical despite different names*

### Comparing `blackduck_lutils-0.0.8/LICENSE` & `blackduck_lutils-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `blackduck_lutils-0.0.8/README.md` & `blackduck_lutils-0.0.9/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -1,21 +1,23 @@
 # Black Duck License Utilities
 
-## License Conflicts
+This module delivers functionality for 
+* License Conflicts
+* License Tagging
 
-# License Conflicts
+## License Conflicts
 
-## Description
-This is a utility that will generate license conflict report by comparing license terms of the licenses associated with components on the Bill of Materials.
+### Description
+This functionality will generate license conflict report by comparing license terms of the licenses associated with components on the Bill of Materials.
 Project version license will be taken into account and license conflicts for it will be calculated as well.
 
-## How it works
+### How it works
 The process is designed to minimize API calls required to produce a report. This is achieved by putting license information into a local storage file and utilizing SBOM report as the data source for project information.
 
-## Bootstrapping
+### Bootstrapping
 Before using the script, license data would have to be downloaded from the system and stored in to a file. To perform that task execute the following:
 
 ```
 export PYTHONPATH=`pwd`/src:$PYTHONPATH
 python3 tests/test_download_license_data.py -u $BD_URL -t <(echo $API_TOKEN) -nv
 ```
 This will download license data into 'license_data.json` file in the current directory. To place the file into different location use corresponding command line option.
@@ -40,18 +42,18 @@
   -pv PROJECT_VERSION_NAME, --project-version-name PROJECT_VERSION_NAME
                         Project Version Name
   -o OUTPUT_FILE, --output-file OUTPUT_FILE
                         Local Storage file for license information
 
 ```
 
-## Usage
+### Usage
 This utility cam be used in off-line and on-lne modes.
 
-### On-line mode
+#### On-line mode
 In on-line mode the following actions will take place:
 * Issue an API request to generate SBOM report.
 * Wait for report completion
 * Download the report 
 * Generate license conflicts data and write it into CSV file
 
 To use the utility in on-line mode add the following lines should be added to you automation:
@@ -65,15 +67,15 @@
                                                   project_version_name=args.project_version_name,
                                                   license_data_file=args.license_data,
                                                   csv_report_file=args.output_file)
 
 ```
 Note: The folder containing license_conflict_report.py should be included in PYTHONPATH.
 
-### Off-line mode
+#### Off-line mode
 In off-line mode a SBOM report in SPDX format would have to exist.
 The following actions will take place:
 * Load SBOM report from a file
 * Generate license conflict data and write it into a file
 
 To use this utility in off-line mode, the following lines should be added to your automation:
 
@@ -83,15 +85,15 @@
         report = generate_license_conflict_report(sbom=args.sbom, 
                                                   license_data_file=args.license_data,
                                                   csv_report_file=args.output_file)
 
 ```
 Note: The folder containing license_conflict_report.py should be included in PYTHONPATH.
 
-## Example
+### Example
 ```
 tests/test_license_conflicts.py
 ```
 Contains a sample code that will provide a command line to allow both on-line and off-line operations as well as specifying optional parameters like location of license data store file and output file name
 
 Note: The folder containing license_conflict_report.py should be included in PYTHONPATH.
 
@@ -113,55 +115,55 @@
   -sbom SBOM            SBOM File to process
   -ld LICENSE_DATA, --license-data LICENSE_DATA
                         Local license data storage
   -o OUTPUT_FILE, --output-file OUTPUT_FILE
                         CSV file name for output
 ```
 
-## Results
+### Results
 Conflict report will be written into CSV file with one line per license term conflict.
 The following fields will be present in the file:
 * Category
 * ComponentName
 * ComponentLicense
 * ConflictingComponentName
 * ConflictingComponentLicense
 * ConflictingLicenseTerm
 * TermValue
 * ConflictingTermValue
 * TermDescription
 * ConflictingTermDescription
 
-## TODO
+### TODO
 This utility is tested in off-line and online mode and has sufficient functionality for API performance testing.
 
 It is not fully tested against functional specification yet.
 
 
-## License
+### License
 This utility is licenses under Apache 2.0 License.
 
 
-## License Tagging
-## License Tagging and Grouping
+### License Tagging
+### License Tagging and Grouping
 License tagging and grouping to allow easy insertion of arbitrary groups of licenses into policy definitions. 
 
-## Description
+### Description
 When there is a need to add an arbitrary group of licenses into a Black Duck policy
 it requires adding them one by one through the UI. This tool allows to maintain an external data store with Tags ang Tag mappings to the licenses and will allow updating policy definitions with expanded list of licenses.
 
-## Requirements
+### Requirements
 This tool requires python 3.9 or newer with the following packages present
 * argparse
 * blackduck
 * openpyxl
 
 Install necessary packages with `pip install -r requirements.txt`
 
-## Usage
+### Usage
 Tool can be executed as a standalone Python script with the following command line specification:
 ```
 usage: license_tagging.py [-h] -u BASE_URL -t TOKEN_FILE [-nv] [-lsf LICENSE_STORE_FILE] [-nlc]
 
 options:
   -h, --help            show this help message and exit
   -u BASE_URL, --base-url BASE_URL
@@ -171,15 +173,15 @@
   -nv, --no-verify      Disable TLS certificate verification
   -lsf LICENSE_STORE_FILE, --license-store-file LICENSE_STORE_FILE
                         Local license information storage
   -nlc, --no-license-check
                         Skip scanning trough all licenses
 ```
 
-## How it works
+### How it works
 The tool maintains local local data storage as an Excel file with default filename of 'LicenseStorage.xlsx'
 
 This file will contain two worksheets
 - Licenses
 - LicenseTags
 
 Licenses worksheet contains data on all licenses currently present in Black Duck instance. Columns contain data and are used as following:
@@ -188,56 +190,53 @@
 * Column C - License Family
 * Column D - License Family URL
 * Column E - SPDXID
 * Column F and above can contain tags
 
 LicenseTags worksheet contains License Tag Names in the Column A and corresponding URL in column B. 
 
-### Common parameters
+#### Common parameters
 In the example command line there would be references to common paraleters:
 * $BD_URL - environment variable contaqing Blackl Duck instance URL
 * token. - a text file containing valid authentication token
 
-### Bootstrapping
+#### Bootstrapping
 Before using the tool, local storage would have to be initalized.
 That is accomplished by running the script.  If it can not find local license store, it will generate new file with complete internal stuctures and populate Licenses worksheet with data from Black Duck instance.
 
 ```
 python3 license_tagging.py -u $BD_URL -t token -nv
 ```
 
 This will generate a file named LicenseStorage.xlsx in the current folder and populate Licenses worksheet with full complement of licenses from your Blackduck instance.
 
 It will also validate presence of 'TagPlaceholder' and create it as necessary.
 At this point there will be no tags defined yet.
 
-### Defining tags
+#### Defining tags
 User must open the local store excel file and add tags to Column A of LicenseTag worksheet, save the Excel file and run the script again.
 ```
 python3 license_tagging.py -u $BD_URL -t token -nv
 ```
 This action will update the references in Black Duck and get the framework ready to be used.
 
-### Tagging Licenses
+#### Tagging Licenses
 Using Excel as a tool, tag licenses on the License worksheet by putting tag name in the columns F and above. There is no limit on how many tags could be associated with a license. 
 
-### Policy creation
+#### Policy creation
 When creating a policy that would have to reference large number of licences use TagName which will be visible and searchable in the UI.
 
-### Expanding tags to full list of licenses
+#### Expanding tags to full list of licenses
 Execute the script again and the Tags in the policy will be expanded to full list of licenses.
 ```
 python3 license_tagging.py -u $BD_URL -t token -nv
 ```
 This action will iterate through the policies, find policy conditions that have tag name in them and replace them with corresponding list of licenses.
 
-## Example of use
+### Example of use
 See example of use here
 
-## Authors and acknowledgment
-Show your appreciation to those who have contributed to the project.
-
-## License
+### License
 This code is licnsed under Apache 2.0 license.
 
-## Project status
+### Project status
 Active
```

### Comparing `blackduck_lutils-0.0.8/pyproject.toml` & `blackduck_lutils-0.0.9/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -20,15 +20,15 @@
   "Programming Language :: Python :: 3.9",
   "Programming Language :: Python :: 3.10",
   "Programming Language :: Python :: 3.11",
   "Programming Language :: Python :: 3.12",
   "Programming Language :: Python :: Implementation :: CPython",
   "Programming Language :: Python :: Implementation :: PyPy",
 ]
-dependencies = []
+dependencies = ['argparse', 'blackduck', 'openpyxl']
 
 [project.urls]
 Documentation = "https://github.com/blackducksoftware/blackduck-lutils#README.md"
 Issues = "https://github.com/blackducksoftware/blackduck-lutils/issues"
 Source = "https://github.com/blackducksoftware/blackduck-lutils"
 
 [tool.hatch.version]
```

### Comparing `blackduck_lutils-0.0.8/PKG-INFO` & `blackduck_lutils-0.0.9/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: blackduck-lutils
-Version: 0.0.8
+Version: 0.0.9
 Summary: Collection of license related tools. License-tagging, License-conflicts
 Project-URL: Documentation, https://github.com/blackducksoftware/blackduck-lutils#README.md
 Project-URL: Issues, https://github.com/blackducksoftware/blackduck-lutils/issues
 Project-URL: Source, https://github.com/blackducksoftware/blackduck-lutils
 Author-email: Murat Kumykov <kumykov@synopsys.com>
 License-Expression: Apache-2.0
 License-File: LICENSE
@@ -14,30 +14,35 @@
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Requires-Python: >=3.8
+Requires-Dist: argparse
+Requires-Dist: blackduck
+Requires-Dist: openpyxl
 Description-Content-Type: text/markdown
 
 # Black Duck License Utilities
 
-## License Conflicts
+This module delivers functionality for 
+* License Conflicts
+* License Tagging
 
-# License Conflicts
+## License Conflicts
 
-## Description
-This is a utility that will generate license conflict report by comparing license terms of the licenses associated with components on the Bill of Materials.
+### Description
+This functionality will generate license conflict report by comparing license terms of the licenses associated with components on the Bill of Materials.
 Project version license will be taken into account and license conflicts for it will be calculated as well.
 
-## How it works
+### How it works
 The process is designed to minimize API calls required to produce a report. This is achieved by putting license information into a local storage file and utilizing SBOM report as the data source for project information.
 
-## Bootstrapping
+### Bootstrapping
 Before using the script, license data would have to be downloaded from the system and stored in to a file. To perform that task execute the following:
 
 ```
 export PYTHONPATH=`pwd`/src:$PYTHONPATH
 python3 tests/test_download_license_data.py -u $BD_URL -t <(echo $API_TOKEN) -nv
 ```
 This will download license data into 'license_data.json` file in the current directory. To place the file into different location use corresponding command line option.
@@ -62,18 +67,18 @@
   -pv PROJECT_VERSION_NAME, --project-version-name PROJECT_VERSION_NAME
                         Project Version Name
   -o OUTPUT_FILE, --output-file OUTPUT_FILE
                         Local Storage file for license information
 
 ```
 
-## Usage
+### Usage
 This utility cam be used in off-line and on-lne modes.
 
-### On-line mode
+#### On-line mode
 In on-line mode the following actions will take place:
 * Issue an API request to generate SBOM report.
 * Wait for report completion
 * Download the report 
 * Generate license conflicts data and write it into CSV file
 
 To use the utility in on-line mode add the following lines should be added to you automation:
@@ -87,15 +92,15 @@
                                                   project_version_name=args.project_version_name,
                                                   license_data_file=args.license_data,
                                                   csv_report_file=args.output_file)
 
 ```
 Note: The folder containing license_conflict_report.py should be included in PYTHONPATH.
 
-### Off-line mode
+#### Off-line mode
 In off-line mode a SBOM report in SPDX format would have to exist.
 The following actions will take place:
 * Load SBOM report from a file
 * Generate license conflict data and write it into a file
 
 To use this utility in off-line mode, the following lines should be added to your automation:
 
@@ -105,15 +110,15 @@
         report = generate_license_conflict_report(sbom=args.sbom, 
                                                   license_data_file=args.license_data,
                                                   csv_report_file=args.output_file)
 
 ```
 Note: The folder containing license_conflict_report.py should be included in PYTHONPATH.
 
-## Example
+### Example
 ```
 tests/test_license_conflicts.py
 ```
 Contains a sample code that will provide a command line to allow both on-line and off-line operations as well as specifying optional parameters like location of license data store file and output file name
 
 Note: The folder containing license_conflict_report.py should be included in PYTHONPATH.
 
@@ -135,55 +140,55 @@
   -sbom SBOM            SBOM File to process
   -ld LICENSE_DATA, --license-data LICENSE_DATA
                         Local license data storage
   -o OUTPUT_FILE, --output-file OUTPUT_FILE
                         CSV file name for output
 ```
 
-## Results
+### Results
 Conflict report will be written into CSV file with one line per license term conflict.
 The following fields will be present in the file:
 * Category
 * ComponentName
 * ComponentLicense
 * ConflictingComponentName
 * ConflictingComponentLicense
 * ConflictingLicenseTerm
 * TermValue
 * ConflictingTermValue
 * TermDescription
 * ConflictingTermDescription
 
-## TODO
+### TODO
 This utility is tested in off-line and online mode and has sufficient functionality for API performance testing.
 
 It is not fully tested against functional specification yet.
 
 
-## License
+### License
 This utility is licenses under Apache 2.0 License.
 
 
-## License Tagging
-## License Tagging and Grouping
+### License Tagging
+### License Tagging and Grouping
 License tagging and grouping to allow easy insertion of arbitrary groups of licenses into policy definitions. 
 
-## Description
+### Description
 When there is a need to add an arbitrary group of licenses into a Black Duck policy
 it requires adding them one by one through the UI. This tool allows to maintain an external data store with Tags ang Tag mappings to the licenses and will allow updating policy definitions with expanded list of licenses.
 
-## Requirements
+### Requirements
 This tool requires python 3.9 or newer with the following packages present
 * argparse
 * blackduck
 * openpyxl
 
 Install necessary packages with `pip install -r requirements.txt`
 
-## Usage
+### Usage
 Tool can be executed as a standalone Python script with the following command line specification:
 ```
 usage: license_tagging.py [-h] -u BASE_URL -t TOKEN_FILE [-nv] [-lsf LICENSE_STORE_FILE] [-nlc]
 
 options:
   -h, --help            show this help message and exit
   -u BASE_URL, --base-url BASE_URL
@@ -193,15 +198,15 @@
   -nv, --no-verify      Disable TLS certificate verification
   -lsf LICENSE_STORE_FILE, --license-store-file LICENSE_STORE_FILE
                         Local license information storage
   -nlc, --no-license-check
                         Skip scanning trough all licenses
 ```
 
-## How it works
+### How it works
 The tool maintains local local data storage as an Excel file with default filename of 'LicenseStorage.xlsx'
 
 This file will contain two worksheets
 - Licenses
 - LicenseTags
 
 Licenses worksheet contains data on all licenses currently present in Black Duck instance. Columns contain data and are used as following:
@@ -210,56 +215,53 @@
 * Column C - License Family
 * Column D - License Family URL
 * Column E - SPDXID
 * Column F and above can contain tags
 
 LicenseTags worksheet contains License Tag Names in the Column A and corresponding URL in column B. 
 
-### Common parameters
+#### Common parameters
 In the example command line there would be references to common paraleters:
 * $BD_URL - environment variable contaqing Blackl Duck instance URL
 * token. - a text file containing valid authentication token
 
-### Bootstrapping
+#### Bootstrapping
 Before using the tool, local storage would have to be initalized.
 That is accomplished by running the script.  If it can not find local license store, it will generate new file with complete internal stuctures and populate Licenses worksheet with data from Black Duck instance.
 
 ```
 python3 license_tagging.py -u $BD_URL -t token -nv
 ```
 
 This will generate a file named LicenseStorage.xlsx in the current folder and populate Licenses worksheet with full complement of licenses from your Blackduck instance.
 
 It will also validate presence of 'TagPlaceholder' and create it as necessary.
 At this point there will be no tags defined yet.
 
-### Defining tags
+#### Defining tags
 User must open the local store excel file and add tags to Column A of LicenseTag worksheet, save the Excel file and run the script again.
 ```
 python3 license_tagging.py -u $BD_URL -t token -nv
 ```
 This action will update the references in Black Duck and get the framework ready to be used.
 
-### Tagging Licenses
+#### Tagging Licenses
 Using Excel as a tool, tag licenses on the License worksheet by putting tag name in the columns F and above. There is no limit on how many tags could be associated with a license. 
 
-### Policy creation
+#### Policy creation
 When creating a policy that would have to reference large number of licences use TagName which will be visible and searchable in the UI.
 
-### Expanding tags to full list of licenses
+#### Expanding tags to full list of licenses
 Execute the script again and the Tags in the policy will be expanded to full list of licenses.
 ```
 python3 license_tagging.py -u $BD_URL -t token -nv
 ```
 This action will iterate through the policies, find policy conditions that have tag name in them and replace them with corresponding list of licenses.
 
-## Example of use
+### Example of use
 See example of use here
 
-## Authors and acknowledgment
-Show your appreciation to those who have contributed to the project.
-
-## License
+### License
 This code is licnsed under Apache 2.0 license.
 
-## Project status
+### Project status
 Active
```

