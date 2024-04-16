# Comparing `tmp/rdf_doctor-1.1.0rc2-py3-none-any.whl.zip` & `tmp/rdf_doctor-1.1.0rc3-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,14 +1,14 @@
-Zip file size: 59803 bytes, number of entries: 12
--rw-r--r--  2.0 unx       25 b- defN 24-Apr-12 04:53 doctor/__init__.py
+Zip file size: 59874 bytes, number of entries: 12
+-rw-r--r--  2.0 unx       25 b- defN 24-Apr-16 02:41 doctor/__init__.py
 -rw-r--r--  2.0 unx     1754 b- defN 24-Mar-29 08:43 doctor/consts.py
--rw-r--r--  2.0 unx    80863 b- defN 24-Apr-12 03:03 doctor/doctor.py
+-rw-r--r--  2.0 unx    81777 b- defN 24-Apr-16 02:29 doctor/doctor.py
 -rw-r--r--  2.0 unx   134314 b- defN 24-Mar-12 04:38 doctor/reference/prefixes.tsv
 -rw-r--r--  2.0 unx       90 b- defN 24-Mar-06 07:08 doctor/reference/refine-class-uris.tsv
 -rw-r--r--  2.0 unx      577 b- defN 24-Mar-06 07:13 doctor/reference/refine-prefix-uris.tsv
--rw-r--r--  2.0 unx     1061 b- defN 24-Apr-12 04:57 rdf_doctor-1.1.0rc2.dist-info/LICENSE
--rw-r--r--  2.0 unx    10690 b- defN 24-Apr-12 04:57 rdf_doctor-1.1.0rc2.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 24-Apr-12 04:57 rdf_doctor-1.1.0rc2.dist-info/WHEEL
--rw-r--r--  2.0 unx       52 b- defN 24-Apr-12 04:57 rdf_doctor-1.1.0rc2.dist-info/entry_points.txt
--rw-r--r--  2.0 unx        7 b- defN 24-Apr-12 04:57 rdf_doctor-1.1.0rc2.dist-info/top_level.txt
--rw-rw-r--  2.0 unx     1013 b- defN 24-Apr-12 04:57 rdf_doctor-1.1.0rc2.dist-info/RECORD
-12 files, 230538 bytes uncompressed, 58087 bytes compressed:  74.8%
+-rw-r--r--  2.0 unx     1061 b- defN 24-Apr-16 04:24 rdf_doctor-1.1.0rc3.dist-info/LICENSE
+-rw-r--r--  2.0 unx    10653 b- defN 24-Apr-16 04:24 rdf_doctor-1.1.0rc3.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 24-Apr-16 04:24 rdf_doctor-1.1.0rc3.dist-info/WHEEL
+-rw-r--r--  2.0 unx       52 b- defN 24-Apr-16 04:24 rdf_doctor-1.1.0rc3.dist-info/entry_points.txt
+-rw-r--r--  2.0 unx        7 b- defN 24-Apr-16 04:24 rdf_doctor-1.1.0rc3.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx     1013 b- defN 24-Apr-16 04:24 rdf_doctor-1.1.0rc3.dist-info/RECORD
+12 files, 231415 bytes uncompressed, 58158 bytes compressed:  74.9%
```

## zipnote {}

```diff
@@ -12,26 +12,26 @@
 
 Filename: doctor/reference/refine-class-uris.tsv
 Comment: 
 
 Filename: doctor/reference/refine-prefix-uris.tsv
 Comment: 
 
-Filename: rdf_doctor-1.1.0rc2.dist-info/LICENSE
+Filename: rdf_doctor-1.1.0rc3.dist-info/LICENSE
 Comment: 
 
-Filename: rdf_doctor-1.1.0rc2.dist-info/METADATA
+Filename: rdf_doctor-1.1.0rc3.dist-info/METADATA
 Comment: 
 
-Filename: rdf_doctor-1.1.0rc2.dist-info/WHEEL
+Filename: rdf_doctor-1.1.0rc3.dist-info/WHEEL
 Comment: 
 
-Filename: rdf_doctor-1.1.0rc2.dist-info/entry_points.txt
+Filename: rdf_doctor-1.1.0rc3.dist-info/entry_points.txt
 Comment: 
 
-Filename: rdf_doctor-1.1.0rc2.dist-info/top_level.txt
+Filename: rdf_doctor-1.1.0rc3.dist-info/top_level.txt
 Comment: 
 
-Filename: rdf_doctor-1.1.0rc2.dist-info/RECORD
+Filename: rdf_doctor-1.1.0rc3.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## doctor/__init__.py

```diff
@@ -1 +1 @@
-__version__ = "1.1.0rc2"
+__version__ = "1.1.0rc3"
```

## doctor/doctor.py

```diff
@@ -40,32 +40,33 @@
         print(error_msg)
         return
 
     # Generate temporary directory for compressed file decompression
     with tempfile.TemporaryDirectory(dir=args.tmp_dir) as temp_dir:
 
         input_file_2d_list = []
-        # If the option is specified to separate results for each input file
-        if args.each:
-            if args.output is None:
-                print("The --each option should be used with the --output option.")
+        # If the option to merge results by input file type is specified
+        if args.merge:
+            # Retrieve input files in dictionary format by type
+            input_file_2d_list, exists_file_types, error_msg = get_input_files_by_type(args.input, temp_dir, args.tmp_dir_disk_usage_limit)
+            if error_msg is not None:
+                print(error_msg)
                 return
 
+        else:
+            # if args.output is None:
+            #     print("The --each option should be used with the --output option.")
+            #     return
+
             # Get an array containing each file to be processed
             # Acquire as a two-dimensional array for compatibility with subsequent processing
             input_file_2d_list, exists_file_types, error_msg = get_input_files_each(args.input, temp_dir, args.tmp_dir_disk_usage_limit)
             if error_msg is not None:
                 print(error_msg)
                 return
-        else:
-            # Retrieve input files in dictionary format by type
-            input_file_2d_list, exists_file_types, error_msg = get_input_files_by_type(args.input, temp_dir, args.tmp_dir_disk_usage_limit)
-            if error_msg is not None:
-                print(error_msg)
-                return
 
         if args.type:
             if args.type == "all":
                 target_file_types = exists_file_types
             else:
                 target_file_types = args.type.split(",")
         else:
@@ -91,35 +92,37 @@
             for input_file_list in input_file_2d_list:
                 if is_target_file(input_file_list, target_file_types) == False:
                     continue
 
                 compression_mode = input_file_list[1]
                 input_format = input_file_list[2]
 
+                if args.verbose:
+                    print_overwrite(get_dt_now() + " -- Start processing [" + ", ".join(str(input_file) for input_file in input_file_list[0]) + "]")
+
                 executor_calc.submit(get_shex_result, args, input_file_list[0], input_format, compression_mode, result_queue)
 
             executor_calc.shutdown()
             if args.verbose:
                 is_displaying_spinner = False
                 executor_spinner.shutdown()
 
             while not result_queue.empty():
                 result_output = result_queue.get()
                 if type(result_output) is list:
                     # Normal case
                     if args.output is None:
                         # Standard output
                         print_overwrite("".join(result_output[0]))
+
+                        if args.verbose:
+                            print_overwrite(get_dt_now() + " -- Done! [" + ", ".join(str(input_file) for input_file in result_output[1]) + "]")
                     else:
                         # Output to file
-                        if args.each:
-                            #with open(args.output + "/" + os.path.basename(input_file_list[0][0]) + ".shex", "w", encoding="utf-8") as f:
-                            with open(args.output + "/" + Path(result_output[1][0]).name + ".shex", "w", encoding="utf-8") as f:
-                                f.write("".join(result_output[0]))
-                        else:
+                        if args.merge:
                             # Output one result file for each type of file processed(Turtle, N-triples, and RDF/XML)
                             # turtle.shex, nt.shex, rdf.shex
                             if result_output[2] == TURTLE:
                                 output_file_name = TURTLE
                             elif result_output[2] == NT:
                                 output_file_name = "n-triples"
                             elif result_output[2] == RDF_XML:
@@ -129,16 +132,20 @@
                                 compression_exetention = ""
                             else:
                                 compression_exetention = "." + result_output[3]
 
                             with open(args.output + "/" + output_file_name + compression_exetention + ".shex", "w", encoding="utf-8") as f:
                                 f.write("".join(result_output[0]))
 
-                    if args.verbose:
-                        print_overwrite(get_dt_now() + " -- Done!")
+                        else:
+                            with open(args.output + "/" + Path(result_output[1][0]).name + ".shex", "w", encoding="utf-8") as f:
+                                f.write("".join(result_output[0]))
+
+                        if args.verbose:
+                            print_overwrite(get_dt_now() + " -- Done! [" + ", ".join(str(input_file) for input_file in result_output[1]) + "] Output file: [" + str(Path(args.output + "/" + Path(result_output[1][0]).name)) + ".shex]")
 
                 elif type(result_output) in [ValueError, IndexError, MemoryError, Exception]:
                     # Error case
                     raise result_output
 
                 else:
                     # Else case does not occur.
@@ -195,16 +202,16 @@
             return line.split(delim)[1]
     else:
         raise RuntimeError("Unable to find version string.")
 
 
 # Parse command line arguments and get them as ArgumentParser
 def get_command_line_args(args):
-    parser = argparse.ArgumentParser(description="Home page: https://github.com/dbcls/rdf-doctor",
-                                    usage="rdf-doctor -i RDF-FILE [Options]",
+    parser = argparse.ArgumentParser(description="version: " + get_version(VERSION_FILE) +"\n\nhome page: https://github.com/dbcls/rdf-doctor",
+                                    usage="rdf-doctor -i RDF-FILE or DIRECTORY [Options]",
                                     formatter_class=argparse.RawDescriptionHelpFormatter)
 
     # Version info(-V, --version)
     parser.add_argument("-V","--version",
                         action="version",
                         version="%(prog)s " + get_version(VERSION_FILE))
 
@@ -237,18 +244,18 @@
     # Target class(-c、--classes [URL1, URL2,...]、default: all、Multiple can be specified.)
     parser.add_argument("-c","--classes", type=str,
                         default=[TARGET_CLASS_ALL],
                         nargs="+",
                         help="set the target classes to be inspected to one of: all (defalut) or URL1 URL2...",
                         metavar="URL")
 
-    # Separate results by file when multiple files are specified (-e、--each)
-    parser.add_argument("-e","--each",
+    # Merge results by input file format (-m、--merge)
+    parser.add_argument("-m","--merge",
                         action="store_true",
-                        help="separate results by file when multiple files are specified")
+                        help="merge results by input file format")
 
     # Temporary directory (--tmp-dir [DIRECTORY]、default: Platform-dependent default temporary directory)
     parser.add_argument("--tmp-dir", type=str,
                         default=None,
                         help='Temporary directory where the unzipped contents are placed when processing tar.gz or zip (default: Platform-dependent default temporary directory)',
                         metavar="DIRECTORY")
 
@@ -880,15 +887,15 @@
         # Get Prefix when input file is turtle format
         if input_format == NT:
             input_prefixes = []
             duplicated_prefixes = []
             namespaces_dict = get_default_namespaces_dict()
         else:
             if args.verbose:
-                print_overwrite(get_dt_now() + " -- Getting prefixes from input file...")
+                print_overwrite(get_dt_now() + " -- Getting prefixes from input file... [" + ", ".join(str(input_file) for input_file in input_file_list) + "]")
 
             if input_format == TURTLE:
                 input_prefixes, duplicated_prefixes, duplicated_prefixes_dict = get_input_prefixes_turtle(input_file_list, compression_mode)
             elif input_format == RDF_XML:
                 input_prefixes, duplicated_prefixes, duplicated_prefixes_dict = get_input_prefixes_rdf_xml(input_file_list, compression_mode)
             else:
                 raise ValueError('Invalid input format: ' + str(input_format))
@@ -898,28 +905,28 @@
         shaper_result = get_shaper_result(args, input_file_list, input_format, compression_mode, namespaces_dict)
 
         report_result = []
         # Output only if report output option is specified
         if args.report:
             # Prefixes with the same Namespace but different URIs at the same time
             if args.verbose:
-                print_overwrite(get_dt_now() + " -- Checking for duplicate prefixes...")
+                print_overwrite(get_dt_now() + " -- Checking for duplicate prefixes... [" + ", ".join(str(input_file) for input_file in input_file_list) + "]")
 
             result_duplicated_prefixes = []
             if len(duplicated_prefixes) != 0:
                 result_duplicated_prefixes.append("# Duplicate prefixes found.\n")
                 result_duplicated_prefixes.append("# ```\n")
                 result_duplicated_prefixes.append("# Input-Namespace\tInput-prefix-URI\n")
                 result_duplicated_prefixes.extend(["# " + s for s in duplicated_prefixes])
                 result_duplicated_prefixes.append("# ```\n")
                 result_duplicated_prefixes.append("# \n# \n")
 
             # Suggest Namespace based on URI of validation expression output by sheXer and prefixes.tsv
             if args.verbose:
-                print_overwrite(get_dt_now() + " -- Creating suggestions for Namespace...")
+                print_overwrite(get_dt_now() + " -- Creating suggestions for Namespace... [" + ", ".join(str(input_file) for input_file in input_file_list) + "]")
 
             result_widely_used_namespace_and_uri = []
             widely_used_namespace_and_uri = get_widely_used_namespace_and_uri_result(shaper_result, input_prefixes, widely_used_prefixes_dict, args.prefix_uri_dict)
             if len(widely_used_namespace_and_uri) != 0:
                 result_widely_used_namespace_and_uri.append("# There is a more widely used Namespace and URI.\n")
                 result_widely_used_namespace_and_uri.append("# (For each of Namespace and URI, output only if the input value differs from the widely used value.)\n")
                 # When prefix list is explicitly specified
@@ -934,37 +941,37 @@
                 result_widely_used_namespace_and_uri.extend(["# " + s for s in widely_used_namespace_and_uri])
                 result_widely_used_namespace_and_uri.append("# ```\n")
                 result_widely_used_namespace_and_uri.append("# \n# \n")
 
             # Output results previously output in markdown mode=========================================
             # Get list for result output about prefix reuse percentage
             if args.verbose:
-                print_overwrite(get_dt_now() + " -- Calculating prefix reuse percentage...")
+                print_overwrite(get_dt_now() + " -- Calculating prefix reuse percentage... [" + ", ".join(str(input_file) for input_file in input_file_list) + "]")
 
             result_prefix_reuse_percentage = []
             result_prefix_reuse_percentage.append("# ## Prefix reuse percentage ([?](" + HELP_LINK_URL + "))\n# \n")
             result_prefix_reuse_percentage.append("# Percentage of prefixes used in the input file that are included in the predefined prefix list inside rdf-doctor.\n")
             result_prefix_reuse_percentage.append("# ```\n")
             prefix_reuse_percentage = get_prefix_reuse_percentage(input_prefixes, widely_used_prefixes_dict)
             if prefix_reuse_percentage is None:
                 result_prefix_reuse_percentage.append("# Not calculated because there is no prefix defined.\n")
             else:
                 result_prefix_reuse_percentage.append("# " + str(prefix_reuse_percentage) + "%\n")
             result_prefix_reuse_percentage.append("# ```\n# \n# \n")
 
             if args.verbose:
-                print_overwrite(get_dt_now() + " -- Getting classes from input file...")
+                print_overwrite(get_dt_now() + " -- Getting classes from input file... [" + ", ".join(str(input_file) for input_file in input_file_list) + "]")
 
             # Processing related to classes -------------------
             input_classes = get_input_classes(input_file_list, input_format, compression_mode, args.classes)
 
             # Refers to the class URIs dictionary, acquires the list for result output that candidate pairs of URI rewrite source and rewrite destinations,
             # and generate the class corresponding to each key in fingerprint format stored in dictionary format.
             if args.verbose:
-                print_overwrite(get_dt_now() + " -- Comparing with class URIs dictionary...")
+                print_overwrite(get_dt_now() + " -- Comparing with class URIs dictionary... [" + ", ".join(str(input_file) for input_file in input_file_list) + "]")
 
             result_refine_class_uris = []
             class_comparison_result, fingerprint_class_dict = get_class_comparison_result(input_classes, args.class_uri_dict)
             # When there is data to output
             if len(class_comparison_result) != 0:
                 result_refine_class_uris.append("# Found a more widely used one for the class URI inputed.\n")
                 # When class URI dictionary is explicitly specified
@@ -975,15 +982,15 @@
                 result_refine_class_uris.append("# Input-class-URI\tSuggested-class-URI\n")
                 result_refine_class_uris.extend(["# " + s for s in class_comparison_result])
                 result_refine_class_uris.append("# ```\n")
                 result_refine_class_uris.append("# \n# \n")
 
             # Get a result output list to notify about different class strings with the same key as a result of fingerprinting
             if args.verbose:
-                print_overwrite(get_dt_now() + " -- Comparing with fingerprint method results...")
+                print_overwrite(get_dt_now() + " -- Comparing with fingerprint method results...[" + ", ".join(str(input_file) for input_file in input_file_list) + "]")
 
             result_class_fingerprint = []
             fingerprint_comparison_result = get_fingerprint_comparison_result(fingerprint_class_dict)
             # When there is data to output
             if len(fingerprint_comparison_result) != 0:
                 result_class_fingerprint.append("# Found multiple strings that appear to represent the same class.\n")
                 result_class_fingerprint.append("# ```\n# ")
```

## Comparing `rdf_doctor-1.1.0rc2.dist-info/LICENSE` & `rdf_doctor-1.1.0rc3.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `rdf_doctor-1.1.0rc2.dist-info/METADATA` & `rdf_doctor-1.1.0rc3.dist-info/METADATA`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rdf-doctor
-Version: 1.1.0rc2
+Version: 1.1.0rc3
 Summary: Validate RDF data, report problems, and support creation of more accurate data
 Home-page: https://github.com/dbcls/rdf-doctor
 Author: DBCLS
 License: MIT
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
@@ -43,44 +43,43 @@
 ```
 pip install rdf-doctor
 ```
 
 ## Command Line Interface
 ```
 $ rdf-doctor --help
-usage: rdf-doctor -i RDF-FILE [Options]
+usage: rdf-doctor -i RDF-FILE or DIRECTORY [Options]
 
-Home page: https://github.com/dbcls/rdf-doctor
+version: 1.1.0
+
+home page: https://github.com/dbcls/rdf-doctor
 
 options:
   -h, --help            show this help message and exit
   -V, --version         show program's version number and exit
   -v, --verbose         show progress while processing
   -i RDF-FILE or DIRECTORY [RDF-FILE or DIRECTORY ...], --input RDF-FILE or DIRECTORY [RDF-FILE or DIRECTORY ...]
                         input RDF file or directory (Turtle(.ttl), N-Triples(.nt), RDF/XML(.rdf, .xml, .owl) and their compressed versions are supported)
   -t TYPE, --type TYPE  specifies the type of the input file ("all" or individually from the following Multiple types can be specified by separating them with a comma. ttl, nt, rdf_xml, ttl_gz, nt_gz, rdf_xml_gz, ttl_zip, nt_zip, rdf_xml_zip)
   -r, --report          add report to results
   -o DIRECTORY, --output DIRECTORY
                         directory to output results (standard output if not specified)
   -c URL [URL ...], --classes URL [URL ...]
                         set the target classes to be inspected to one of: all (defalut) or URL1 URL2...
-  -e, --each            separate results by file when multiple files are specified
-  --tmp-dir DIRECTORY   Temporary directory where the unzipped contents are placed when processing tar.gz or zipped directory
+  -m, --merge           merge results by input file format
+  --tmp-dir DIRECTORY   Temporary directory where the unzipped contents are placed when processing tar.gz or zip (default: Platform-dependent default temporary directory)
   --tmp-dir-disk-usage-limit PERCENTAGE
-                        Percentage of disk usage that contains the temporary directory where unzipped contents are placed when processing tar.gz or zipped directory. Interrupt processing when the specified usage percentage is exceeded (1-100 default: 95)
+                        Percentage of disk usage that contains the temporary directory where unzipped contents are placed when processing tar.gz or zip. Interrupt processing when the specified usage percentage is exceeded (1-100 default: 95)
   --prefix-uri-dict FILE
-                        path to a tab delimited file listing candidate pairs of URI rewrite source and rewrite destination for the prefix (default: predefined file in rdf-doctor: https://github.com/dbcls/rdf-
-                        doctor/blob/main/doctor/reference/refine-prefix-uris.tsv)
+                        path to a tab delimited file listing candidate pairs of URI rewrite source and rewrite destination for the prefix (default: predefined file in rdf-doctor: https://github.com/dbcls/rdf-doctor/blob/main/doctor/reference/refine-prefix-uris.tsv)
   --class-uri-dict FILE
-                        path to a tab delimited file listing candidate pairs of URI rewrite source and rewrite destination for the class (default: predefined file in rdf-doctor: https://github.com/dbcls/rdf-
-                        doctor/blob/main/doctor/reference/refine-class-uris.tsv)
+                        path to a tab delimited file listing candidate pairs of URI rewrite source and rewrite destination for the class (default: predefined file in rdf-doctor: https://github.com/dbcls/rdf-doctor/blob/main/doctor/reference/refine-class-uris.tsv)
   --prefix-list FILE    list of prefixes (default: predefined file in rdf-doctor: https://github.com/dbcls/rdf-doctor/blob/main/doctor/reference/prefixes.tsv)
   --force-format INPUT-FORMAT
-                        This option should not normally be used. Because the input format is automatically determined by the file extension. Use it only when you want to force specification. If used, "turtle", "nt" and
-                        "xml"(=RDF/XML) can be specified.
+                        This option should not normally be used. Because the input format is automatically determined by the file extension. Use it only when you want to force specification. If used, "turtle", "nt" and "xml"(=RDF/XML) can be specified.
 ```
 
 ## See Also
 - [1] https://github.com/DaniFdezAlvarez/shexer
 - [2] http://shex.io/shex-primer/#combined-constraints
 - [3] https://openrefine.org/docs/technical-reference/clustering-in-depth#fingerprint
```

## Comparing `rdf_doctor-1.1.0rc2.dist-info/RECORD` & `rdf_doctor-1.1.0rc3.dist-info/RECORD`

 * *Files 17% similar despite different names*

```diff
@@ -1,12 +1,12 @@
-doctor/__init__.py,sha256=2DW4CDF3GisId6QRWoUv6R9Y8dfyAxXlpENtY6pGBd4,25
+doctor/__init__.py,sha256=cL9JVkp_7v5vXYtfMPakVSDg98hX-MyIO3n3MYdTdYI,25
 doctor/consts.py,sha256=U8KOzdPFgMuf_nMul1Vw9qtAvKtZbu8WLwkiYD49IAs,1754
-doctor/doctor.py,sha256=F46476QuaWxPNoUKP20H-CZUYTFUaeVrhLLixxlYKfw,80863
+doctor/doctor.py,sha256=YQhN_-SN5efT5E9-S0LikSFiREf52Fg_lAsA25h6twY,81777
 doctor/reference/prefixes.tsv,sha256=_1hW0wBl6K1YvcM8stdiEdD4elzST_ecJqQEvhD9Auk,134314
 doctor/reference/refine-class-uris.tsv,sha256=pd_nOSjR7bia96u9hhcjhBg9J6LUAuDFlyy-JE9tsys,90
 doctor/reference/refine-prefix-uris.tsv,sha256=KY5PZ4WCaLeB0APNBjAWq7_Q5Whc6FLg9ncX7BSPeuw,577
-rdf_doctor-1.1.0rc2.dist-info/LICENSE,sha256=e5qMQtuffizvdi23h6MoQ37f3xmNY0VBq8V0tgWuZNg,1061
-rdf_doctor-1.1.0rc2.dist-info/METADATA,sha256=1gso0ycDN5DIGl9Vo0PLXup2xIY-wukgP2dNMFveVCs,10690
-rdf_doctor-1.1.0rc2.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
-rdf_doctor-1.1.0rc2.dist-info/entry_points.txt,sha256=1vHyYdY5pMK7zOINHh2ymwU_Uid1YzZx7Vte5tjHCls,52
-rdf_doctor-1.1.0rc2.dist-info/top_level.txt,sha256=8awHkjBkPxJ8N_ygAwmuUTUz5ZKfy9aqNcWTSI_Ma_8,7
-rdf_doctor-1.1.0rc2.dist-info/RECORD,,
+rdf_doctor-1.1.0rc3.dist-info/LICENSE,sha256=e5qMQtuffizvdi23h6MoQ37f3xmNY0VBq8V0tgWuZNg,1061
+rdf_doctor-1.1.0rc3.dist-info/METADATA,sha256=EmzWBa2kTqF4zsvQdoHYiu5UiceT-fQhFDL8qKlO7Kw,10653
+rdf_doctor-1.1.0rc3.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
+rdf_doctor-1.1.0rc3.dist-info/entry_points.txt,sha256=1vHyYdY5pMK7zOINHh2ymwU_Uid1YzZx7Vte5tjHCls,52
+rdf_doctor-1.1.0rc3.dist-info/top_level.txt,sha256=8awHkjBkPxJ8N_ygAwmuUTUz5ZKfy9aqNcWTSI_Ma_8,7
+rdf_doctor-1.1.0rc3.dist-info/RECORD,,
```

