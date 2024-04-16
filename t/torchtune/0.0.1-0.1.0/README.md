# Comparing `tmp/torchtune-0.0.1-py3-none-any.whl.zip` & `tmp/torchtune-0.1.0-py3-none-any.whl.zip`

## zipinfo -v {}

 * *Differences in extra fields detected; using output from zipinfo -v*

```diff
@@ -1,3555 +1,5026 @@
 There is no zipfile comment.
 
 End-of-central-directory record:
 -------------------------------
 
-  Zip archive file size:                    155821 (00000000000260ADh)
-  Actual end-cent-dir record offset:        155799 (0000000000026097h)
-  Expected end-cent-dir record offset:      155799 (0000000000026097h)
+  Zip archive file size:                    192092 (000000000002EE5Ch)
+  Actual end-cent-dir record offset:        192070 (000000000002EE46h)
+  Expected end-cent-dir record offset:      192070 (000000000002EE46h)
   (based on the length of the central directory and its expected offset)
 
   This zipfile constitutes the sole disk of a single-part archive; its
-  central directory contains 122 entries.
-  The central directory is 9809 (0000000000002651h) bytes long,
+  central directory contains 136 entries.
+  The central directory is 13740 (00000000000035ACh) bytes long,
   and its (expected) offset in bytes from the beginning of the zipfile
-  is 145990 (0000000000023A46h).
+  is 178330 (000000000002B89Ah).
 
 
 Central directory entry #1:
 ---------------------------
 
-  tests/__init__.py
+  recipes/
 
   offset of local header from start of archive:   0
                                                   (0000000000000000h) bytes
   file system or operating system of origin:      Unix
-  version of encoding software:                   2.0
+  version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
-  minimum software version required to extract:   2.0
-  compression method:                             deflated
-  compression sub-type (deflation):               normal
+  minimum software version required to extract:   1.0
+  compression method:                             none (stored)
   file security status:                           not encrypted
   extended local header:                          no
-  file last modified on (DOS date/time):          2024 Mar 21 19:57:36
-  32-bit CRC value (hex):                         2ca9d797
-  compressed size:                                150 bytes
-  uncompressed size:                              208 bytes
-  length of filename:                             17 characters
-  length of extra field:                          0 bytes
+  file last modified on (DOS date/time):          2024 Apr 15 20:08:26
+  file last modified on (UT extra field modtime): 2024 Apr 16 03:08:26 local
+  file last modified on (UT extra field modtime): 2024 Apr 16 03:08:26 UTC
+  32-bit CRC value (hex):                         00000000
+  compressed size:                                0 bytes
+  uncompressed size:                              0 bytes
+  length of filename:                             8 characters
+  length of extra field:                          24 bytes
   length of file comment:                         0 characters
   disk number on which file begins:               disk 1
   apparent file type:                             binary
-  Unix file attributes (100664 octal):            -rw-rw-r--
-  MS-DOS file attributes (00 hex):                none
+  Unix file attributes (040755 octal):            drwxr-xr-x
+  MS-DOS file attributes (10 hex):                dir 
+
+  The central-directory extra field contains:
+  - A subfield with ID 0x5455 (universal time) and 5 data bytes.
+    The local extra field has UTC/GMT modification/access times.
+  - A subfield with ID 0x7875 (Unix UID/GID (any size)) and 11 data bytes:
+    01 04 e3 3d 03 00 04 64 00 00 00.
 
   There is no file comment.
 
 Central directory entry #2:
 ---------------------------
 
-  tests/common.py
+  recipes/__init__.py
 
-  offset of local header from start of archive:   197
-                                                  (00000000000000C5h) bytes
+  offset of local header from start of archive:   66
+                                                  (0000000000000042h) bytes
   file system or operating system of origin:      Unix
-  version of encoding software:                   2.0
+  version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
-  compression sub-type (deflation):               normal
+  compression sub-type (deflation):               maximum
   file security status:                           not encrypted
   extended local header:                          no
-  file last modified on (DOS date/time):          2024 Mar 21 19:57:36
-  32-bit CRC value (hex):                         e5e7dbf5
-  compressed size:                                184 bytes
-  uncompressed size:                              246 bytes
-  length of filename:                             15 characters
-  length of extra field:                          0 bytes
+  file last modified on (DOS date/time):          2024 Apr 16 01:12:14
+  file last modified on (UT extra field modtime): 2024 Apr 16 08:12:14 local
+  file last modified on (UT extra field modtime): 2024 Apr 16 08:12:14 UTC
+  32-bit CRC value (hex):                         f8832146
+  compressed size:                                657 bytes
+  uncompressed size:                              1204 bytes
+  length of filename:                             19 characters
+  length of extra field:                          24 bytes
   length of file comment:                         0 characters
   disk number on which file begins:               disk 1
-  apparent file type:                             binary
-  Unix file attributes (100664 octal):            -rw-rw-r--
+  apparent file type:                             text
+  Unix file attributes (100644 octal):            -rw-r--r--
   MS-DOS file attributes (00 hex):                none
 
+  The central-directory extra field contains:
+  - A subfield with ID 0x5455 (universal time) and 5 data bytes.
+    The local extra field has UTC/GMT modification/access times.
+  - A subfield with ID 0x7875 (Unix UID/GID (any size)) and 11 data bytes:
+    01 04 e3 3d 03 00 04 64 00 00 00.
+
   There is no file comment.
 
 Central directory entry #3:
 ---------------------------
 
-  tests/conftest.py
+  recipes/eleuther_eval.py
 
-  offset of local header from start of archive:   426
-                                                  (00000000000001AAh) bytes
+  offset of local header from start of archive:   800
+                                                  (0000000000000320h) bytes
   file system or operating system of origin:      Unix
-  version of encoding software:                   2.0
+  version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
-  compression sub-type (deflation):               normal
+  compression sub-type (deflation):               maximum
   file security status:                           not encrypted
   extended local header:                          no
-  file last modified on (DOS date/time):          2024 Mar 21 19:57:36
-  32-bit CRC value (hex):                         906cf2f5
-  compressed size:                                646 bytes
-  uncompressed size:                              1464 bytes
-  length of filename:                             17 characters
-  length of extra field:                          0 bytes
+  file last modified on (DOS date/time):          2024 Apr 16 01:12:14
+  file last modified on (UT extra field modtime): 2024 Apr 16 08:12:14 local
+  file last modified on (UT extra field modtime): 2024 Apr 16 08:12:14 UTC
+  32-bit CRC value (hex):                         2d1774ea
+  compressed size:                                2428 bytes
+  uncompressed size:                              6999 bytes
+  length of filename:                             24 characters
+  length of extra field:                          24 bytes
   length of file comment:                         0 characters
   disk number on which file begins:               disk 1
-  apparent file type:                             binary
-  Unix file attributes (100664 octal):            -rw-rw-r--
+  apparent file type:                             text
+  Unix file attributes (100644 octal):            -rw-r--r--
   MS-DOS file attributes (00 hex):                none
 
+  The central-directory extra field contains:
+  - A subfield with ID 0x5455 (universal time) and 5 data bytes.
+    The local extra field has UTC/GMT modification/access times.
+  - A subfield with ID 0x7875 (Unix UID/GID (any size)) and 11 data bytes:
+    01 04 e3 3d 03 00 04 64 00 00 00.
+
   There is no file comment.
 
 Central directory entry #4:
 ---------------------------
 
-  tests/test_utils.py
+  recipes/full_finetune_distributed.py
 
-  offset of local header from start of archive:   1119
-                                                  (000000000000045Fh) bytes
+  offset of local header from start of archive:   3310
+                                                  (0000000000000CEEh) bytes
   file system or operating system of origin:      Unix
-  version of encoding software:                   2.0
+  version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
-  compression sub-type (deflation):               normal
+  compression sub-type (deflation):               maximum
   file security status:                           not encrypted
   extended local header:                          no
-  file last modified on (DOS date/time):          2024 Mar 21 19:57:36
-  32-bit CRC value (hex):                         2aa52425
-  compressed size:                                1559 bytes
-  uncompressed size:                              4110 bytes
-  length of filename:                             19 characters
-  length of extra field:                          0 bytes
+  file last modified on (DOS date/time):          2024 Apr 16 01:12:14
+  file last modified on (UT extra field modtime): 2024 Apr 16 08:12:14 local
+  file last modified on (UT extra field modtime): 2024 Apr 16 08:12:14 UTC
+  32-bit CRC value (hex):                         c1d4edb8
+  compressed size:                                6137 bytes
+  uncompressed size:                              21147 bytes
+  length of filename:                             36 characters
+  length of extra field:                          24 bytes
   length of file comment:                         0 characters
   disk number on which file begins:               disk 1
-  apparent file type:                             binary
-  Unix file attributes (100664 octal):            -rw-rw-r--
+  apparent file type:                             text
+  Unix file attributes (100644 octal):            -rw-r--r--
   MS-DOS file attributes (00 hex):                none
 
+  The central-directory extra field contains:
+  - A subfield with ID 0x5455 (universal time) and 5 data bytes.
+    The local extra field has UTC/GMT modification/access times.
+  - A subfield with ID 0x7875 (Unix UID/GID (any size)) and 11 data bytes:
+    01 04 e3 3d 03 00 04 64 00 00 00.
+
   There is no file comment.
 
 Central directory entry #5:
 ---------------------------
 
-  tests/recipes/__init__.py
+  recipes/full_finetune_single_device.py
 
-  offset of local header from start of archive:   2727
-                                                  (0000000000000AA7h) bytes
+  offset of local header from start of archive:   9541
+                                                  (0000000000002545h) bytes
   file system or operating system of origin:      Unix
-  version of encoding software:                   2.0
+  version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
-  compression sub-type (deflation):               normal
+  compression sub-type (deflation):               maximum
   file security status:                           not encrypted
   extended local header:                          no
-  file last modified on (DOS date/time):          2024 Mar 21 19:57:36
-  32-bit CRC value (hex):                         2ca9d797
-  compressed size:                                150 bytes
-  uncompressed size:                              208 bytes
-  length of filename:                             25 characters
-  length of extra field:                          0 bytes
+  file last modified on (DOS date/time):          2024 Apr 16 01:12:14
+  file last modified on (UT extra field modtime): 2024 Apr 16 08:12:14 local
+  file last modified on (UT extra field modtime): 2024 Apr 16 08:12:14 UTC
+  32-bit CRC value (hex):                         aaa08982
+  compressed size:                                6040 bytes
+  uncompressed size:                              21166 bytes
+  length of filename:                             38 characters
+  length of extra field:                          24 bytes
   length of file comment:                         0 characters
   disk number on which file begins:               disk 1
-  apparent file type:                             binary
-  Unix file attributes (100664 octal):            -rw-rw-r--
+  apparent file type:                             text
+  Unix file attributes (100644 octal):            -rw-r--r--
   MS-DOS file attributes (00 hex):                none
 
+  The central-directory extra field contains:
+  - A subfield with ID 0x5455 (universal time) and 5 data bytes.
+    The local extra field has UTC/GMT modification/access times.
+  - A subfield with ID 0x7875 (Unix UID/GID (any size)) and 11 data bytes:
+    01 04 e3 3d 03 00 04 64 00 00 00.
+
   There is no file comment.
 
 Central directory entry #6:
 ---------------------------
 
-  tests/recipes/common.py
+  recipes/generate.py
 
-  offset of local header from start of archive:   2932
-                                                  (0000000000000B74h) bytes
+  offset of local header from start of archive:   15677
+                                                  (0000000000003D3Dh) bytes
   file system or operating system of origin:      Unix
-  version of encoding software:                   2.0
+  version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
-  compression sub-type (deflation):               normal
+  compression sub-type (deflation):               maximum
   file security status:                           not encrypted
   extended local header:                          no
-  file last modified on (DOS date/time):          2024 Mar 21 19:57:36
-  32-bit CRC value (hex):                         6a329f7b
-  compressed size:                                199 bytes
-  uncompressed size:                              276 bytes
-  length of filename:                             23 characters
-  length of extra field:                          0 bytes
+  file last modified on (DOS date/time):          2024 Apr 16 01:12:14
+  file last modified on (UT extra field modtime): 2024 Apr 16 08:12:14 local
+  file last modified on (UT extra field modtime): 2024 Apr 16 08:12:14 UTC
+  32-bit CRC value (hex):                         c50b752c
+  compressed size:                                1714 bytes
+  uncompressed size:                              5144 bytes
+  length of filename:                             19 characters
+  length of extra field:                          24 bytes
   length of file comment:                         0 characters
   disk number on which file begins:               disk 1
-  apparent file type:                             binary
-  Unix file attributes (100664 octal):            -rw-rw-r--
+  apparent file type:                             text
+  Unix file attributes (100644 octal):            -rw-r--r--
   MS-DOS file attributes (00 hex):                none
 
+  The central-directory extra field contains:
+  - A subfield with ID 0x5455 (universal time) and 5 data bytes.
+    The local extra field has UTC/GMT modification/access times.
+  - A subfield with ID 0x7875 (Unix UID/GID (any size)) and 11 data bytes:
+    01 04 e3 3d 03 00 04 64 00 00 00.
+
   There is no file comment.
 
 Central directory entry #7:
 ---------------------------
 
-  tests/recipes/test_alpaca_generate.py
+  recipes/lora_dpo_single_device.py
 
-  offset of local header from start of archive:   3184
-                                                  (0000000000000C70h) bytes
+  offset of local header from start of archive:   17468
+                                                  (000000000000443Ch) bytes
   file system or operating system of origin:      Unix
-  version of encoding software:                   2.0
+  version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
-  compression sub-type (deflation):               normal
+  compression sub-type (deflation):               maximum
   file security status:                           not encrypted
   extended local header:                          no
-  file last modified on (DOS date/time):          2024 Mar 21 19:57:36
-  32-bit CRC value (hex):                         e7374673
-  compressed size:                                726 bytes
-  uncompressed size:                              1575 bytes
-  length of filename:                             37 characters
-  length of extra field:                          0 bytes
+  file last modified on (DOS date/time):          2024 Apr 16 01:12:14
+  file last modified on (UT extra field modtime): 2024 Apr 16 08:12:14 local
+  file last modified on (UT extra field modtime): 2024 Apr 16 08:12:14 UTC
+  32-bit CRC value (hex):                         107ec23d
+  compressed size:                                5746 bytes
+  uncompressed size:                              21497 bytes
+  length of filename:                             33 characters
+  length of extra field:                          24 bytes
   length of file comment:                         0 characters
   disk number on which file begins:               disk 1
-  apparent file type:                             binary
-  Unix file attributes (100664 octal):            -rw-rw-r--
+  apparent file type:                             text
+  Unix file attributes (100644 octal):            -rw-r--r--
   MS-DOS file attributes (00 hex):                none
 
+  The central-directory extra field contains:
+  - A subfield with ID 0x5455 (universal time) and 5 data bytes.
+    The local extra field has UTC/GMT modification/access times.
+  - A subfield with ID 0x7875 (Unix UID/GID (any size)) and 11 data bytes:
+    01 04 e3 3d 03 00 04 64 00 00 00.
+
   There is no file comment.
 
 Central directory entry #8:
 ---------------------------
 
-  tests/recipes/test_configs.py
+  recipes/lora_finetune_distributed.py
 
-  offset of local header from start of archive:   3977
-                                                  (0000000000000F89h) bytes
+  offset of local header from start of archive:   23305
+                                                  (0000000000005B09h) bytes
   file system or operating system of origin:      Unix
-  version of encoding software:                   2.0
+  version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
-  compression sub-type (deflation):               normal
+  compression sub-type (deflation):               maximum
   file security status:                           not encrypted
   extended local header:                          no
-  file last modified on (DOS date/time):          2024 Mar 21 19:57:36
-  32-bit CRC value (hex):                         1e5ece6c
-  compressed size:                                390 bytes
-  uncompressed size:                              722 bytes
-  length of filename:                             29 characters
-  length of extra field:                          0 bytes
+  file last modified on (DOS date/time):          2024 Apr 16 01:12:14
+  file last modified on (UT extra field modtime): 2024 Apr 16 08:12:14 local
+  file last modified on (UT extra field modtime): 2024 Apr 16 08:12:14 UTC
+  32-bit CRC value (hex):                         0b482be3
+  compressed size:                                7188 bytes
+  uncompressed size:                              25790 bytes
+  length of filename:                             36 characters
+  length of extra field:                          24 bytes
   length of file comment:                         0 characters
   disk number on which file begins:               disk 1
-  apparent file type:                             binary
-  Unix file attributes (100664 octal):            -rw-rw-r--
+  apparent file type:                             text
+  Unix file attributes (100644 octal):            -rw-r--r--
   MS-DOS file attributes (00 hex):                none
 
+  The central-directory extra field contains:
+  - A subfield with ID 0x5455 (universal time) and 5 data bytes.
+    The local extra field has UTC/GMT modification/access times.
+  - A subfield with ID 0x7875 (Unix UID/GID (any size)) and 11 data bytes:
+    01 04 e3 3d 03 00 04 64 00 00 00.
+
   There is no file comment.
 
 Central directory entry #9:
 ---------------------------
 
-  tests/recipes/test_full_finetune.py
+  recipes/lora_finetune_single_device.py
 
-  offset of local header from start of archive:   4426
-                                                  (000000000000114Ah) bytes
+  offset of local header from start of archive:   30587
+                                                  (000000000000777Bh) bytes
   file system or operating system of origin:      Unix
-  version of encoding software:                   2.0
+  version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
-  compression sub-type (deflation):               normal
+  compression sub-type (deflation):               maximum
   file security status:                           not encrypted
   extended local header:                          no
-  file last modified on (DOS date/time):          2024 Mar 21 19:57:36
-  32-bit CRC value (hex):                         8738da1e
-  compressed size:                                2716 bytes
-  uncompressed size:                              11309 bytes
-  length of filename:                             35 characters
-  length of extra field:                          0 bytes
+  file last modified on (DOS date/time):          2024 Apr 16 01:12:14
+  file last modified on (UT extra field modtime): 2024 Apr 16 08:12:14 local
+  file last modified on (UT extra field modtime): 2024 Apr 16 08:12:14 UTC
+  32-bit CRC value (hex):                         45f242d3
+  compressed size:                                6050 bytes
+  uncompressed size:                              21491 bytes
+  length of filename:                             38 characters
+  length of extra field:                          24 bytes
   length of file comment:                         0 characters
   disk number on which file begins:               disk 1
-  apparent file type:                             binary
-  Unix file attributes (100664 octal):            -rw-rw-r--
+  apparent file type:                             text
+  Unix file attributes (100644 octal):            -rw-r--r--
   MS-DOS file attributes (00 hex):                none
 
+  The central-directory extra field contains:
+  - A subfield with ID 0x5455 (universal time) and 5 data bytes.
+    The local extra field has UTC/GMT modification/access times.
+  - A subfield with ID 0x7875 (Unix UID/GID (any size)) and 11 data bytes:
+    01 04 e3 3d 03 00 04 64 00 00 00.
+
   There is no file comment.
 
 Central directory entry #10:
 ---------------------------
 
-  tests/recipes/test_lora_finetune.py
+  recipes/quantize.py
 
-  offset of local header from start of archive:   7207
-                                                  (0000000000001C27h) bytes
+  offset of local header from start of archive:   36733
+                                                  (0000000000008F7Dh) bytes
   file system or operating system of origin:      Unix
-  version of encoding software:                   2.0
+  version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
-  compression sub-type (deflation):               normal
+  compression sub-type (deflation):               maximum
   file security status:                           not encrypted
   extended local header:                          no
-  file last modified on (DOS date/time):          2024 Mar 21 19:57:36
-  32-bit CRC value (hex):                         32261fd8
-  compressed size:                                2664 bytes
-  uncompressed size:                              11878 bytes
-  length of filename:                             35 characters
-  length of extra field:                          0 bytes
+  file last modified on (DOS date/time):          2024 Apr 16 01:12:14
+  file last modified on (UT extra field modtime): 2024 Apr 16 08:12:14 local
+  file last modified on (UT extra field modtime): 2024 Apr 16 08:12:14 UTC
+  32-bit CRC value (hex):                         1869dd83
+  compressed size:                                1535 bytes
+  uncompressed size:                              4284 bytes
+  length of filename:                             19 characters
+  length of extra field:                          24 bytes
   length of file comment:                         0 characters
   disk number on which file begins:               disk 1
-  apparent file type:                             binary
-  Unix file attributes (100664 octal):            -rw-rw-r--
+  apparent file type:                             text
+  Unix file attributes (100644 octal):            -rw-r--r--
   MS-DOS file attributes (00 hex):                none
 
+  The central-directory extra field contains:
+  - A subfield with ID 0x5455 (universal time) and 5 data bytes.
+    The local extra field has UTC/GMT modification/access times.
+  - A subfield with ID 0x7875 (Unix UID/GID (any size)) and 11 data bytes:
+    01 04 e3 3d 03 00 04 64 00 00 00.
+
   There is no file comment.
 
 Central directory entry #11:
 ---------------------------
 
-  tests/recipes/utils.py
+  recipes/configs/
 
-  offset of local header from start of archive:   9936
-                                                  (00000000000026D0h) bytes
+  offset of local header from start of archive:   38345
+                                                  (00000000000095C9h) bytes
   file system or operating system of origin:      Unix
-  version of encoding software:                   2.0
+  version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
-  minimum software version required to extract:   2.0
-  compression method:                             deflated
-  compression sub-type (deflation):               normal
+  minimum software version required to extract:   1.0
+  compression method:                             none (stored)
   file security status:                           not encrypted
   extended local header:                          no
-  file last modified on (DOS date/time):          2024 Mar 21 19:57:36
-  32-bit CRC value (hex):                         ec002f7c
-  compressed size:                                1295 bytes
-  uncompressed size:                              4098 bytes
-  length of filename:                             22 characters
-  length of extra field:                          0 bytes
+  file last modified on (DOS date/time):          2024 Apr 15 20:08:26
+  file last modified on (UT extra field modtime): 2024 Apr 16 03:08:26 local
+  file last modified on (UT extra field modtime): 2024 Apr 16 03:08:26 UTC
+  32-bit CRC value (hex):                         00000000
+  compressed size:                                0 bytes
+  uncompressed size:                              0 bytes
+  length of filename:                             16 characters
+  length of extra field:                          24 bytes
   length of file comment:                         0 characters
   disk number on which file begins:               disk 1
   apparent file type:                             binary
-  Unix file attributes (100664 octal):            -rw-rw-r--
-  MS-DOS file attributes (00 hex):                none
+  Unix file attributes (040755 octal):            drwxr-xr-x
+  MS-DOS file attributes (10 hex):                dir 
+
+  The central-directory extra field contains:
+  - A subfield with ID 0x5455 (universal time) and 5 data bytes.
+    The local extra field has UTC/GMT modification/access times.
+  - A subfield with ID 0x7875 (Unix UID/GID (any size)) and 11 data bytes:
+    01 04 e3 3d 03 00 04 64 00 00 00.
 
   There is no file comment.
 
 Central directory entry #12:
 ---------------------------
 
-  tests/torchtune/__init__.py
+  recipes/configs/eleuther_evaluation.yaml
 
-  offset of local header from start of archive:   11283
-                                                  (0000000000002C13h) bytes
+  offset of local header from start of archive:   38419
+                                                  (0000000000009613h) bytes
   file system or operating system of origin:      Unix
-  version of encoding software:                   2.0
+  version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
-  compression sub-type (deflation):               normal
+  compression sub-type (deflation):               maximum
   file security status:                           not encrypted
   extended local header:                          no
-  file last modified on (DOS date/time):          2024 Mar 21 19:57:36
-  32-bit CRC value (hex):                         2ca9d797
-  compressed size:                                150 bytes
-  uncompressed size:                              208 bytes
-  length of filename:                             27 characters
-  length of extra field:                          0 bytes
+  file last modified on (DOS date/time):          2024 Apr 16 01:12:14
+  file last modified on (UT extra field modtime): 2024 Apr 16 08:12:14 local
+  file last modified on (UT extra field modtime): 2024 Apr 16 08:12:14 UTC
+  32-bit CRC value (hex):                         c86a9e2b
+  compressed size:                                442 bytes
+  uncompressed size:                              893 bytes
+  length of filename:                             40 characters
+  length of extra field:                          24 bytes
   length of file comment:                         0 characters
   disk number on which file begins:               disk 1
-  apparent file type:                             binary
-  Unix file attributes (100664 octal):            -rw-rw-r--
+  apparent file type:                             text
+  Unix file attributes (100644 octal):            -rw-r--r--
   MS-DOS file attributes (00 hex):                none
 
+  The central-directory extra field contains:
+  - A subfield with ID 0x5455 (universal time) and 5 data bytes.
+    The local extra field has UTC/GMT modification/access times.
+  - A subfield with ID 0x7875 (Unix UID/GID (any size)) and 11 data bytes:
+    01 04 e3 3d 03 00 04 64 00 00 00.
+
   There is no file comment.
 
 Central directory entry #13:
 ---------------------------
 
-  tests/torchtune/_cli/__init__.py
+  recipes/configs/generation.yaml
 
-  offset of local header from start of archive:   11490
-                                                  (0000000000002CE2h) bytes
+  offset of local header from start of archive:   38959
+                                                  (000000000000982Fh) bytes
   file system or operating system of origin:      Unix
-  version of encoding software:                   2.0
+  version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
-  compression sub-type (deflation):               normal
+  compression sub-type (deflation):               maximum
   file security status:                           not encrypted
   extended local header:                          no
-  file last modified on (DOS date/time):          2024 Mar 21 19:57:36
-  32-bit CRC value (hex):                         2ca9d797
-  compressed size:                                150 bytes
-  uncompressed size:                              208 bytes
-  length of filename:                             32 characters
-  length of extra field:                          0 bytes
+  file last modified on (DOS date/time):          2024 Apr 16 01:12:14
+  file last modified on (UT extra field modtime): 2024 Apr 16 08:12:14 local
+  file last modified on (UT extra field modtime): 2024 Apr 16 08:12:14 UTC
+  32-bit CRC value (hex):                         a8c11fef
+  compressed size:                                428 bytes
+  uncompressed size:                              860 bytes
+  length of filename:                             31 characters
+  length of extra field:                          24 bytes
   length of file comment:                         0 characters
   disk number on which file begins:               disk 1
-  apparent file type:                             binary
-  Unix file attributes (100664 octal):            -rw-rw-r--
+  apparent file type:                             text
+  Unix file attributes (100644 octal):            -rw-r--r--
   MS-DOS file attributes (00 hex):                none
 
+  The central-directory extra field contains:
+  - A subfield with ID 0x5455 (universal time) and 5 data bytes.
+    The local extra field has UTC/GMT modification/access times.
+  - A subfield with ID 0x7875 (Unix UID/GID (any size)) and 11 data bytes:
+    01 04 e3 3d 03 00 04 64 00 00 00.
+
   There is no file comment.
 
 Central directory entry #14:
 ---------------------------
 
-  tests/torchtune/_cli/test_convert_checkpoint.py
+  recipes/configs/quantization.yaml
 
-  offset of local header from start of archive:   11702
-                                                  (0000000000002DB6h) bytes
+  offset of local header from start of archive:   39476
+                                                  (0000000000009A34h) bytes
   file system or operating system of origin:      Unix
-  version of encoding software:                   2.0
+  version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
-  compression sub-type (deflation):               normal
+  compression sub-type (deflation):               maximum
   file security status:                           not encrypted
   extended local header:                          no
-  file last modified on (DOS date/time):          2024 Mar 21 19:57:36
-  32-bit CRC value (hex):                         88674cda
-  compressed size:                                1523 bytes
-  uncompressed size:                              5637 bytes
-  length of filename:                             47 characters
-  length of extra field:                          0 bytes
+  file last modified on (DOS date/time):          2024 Apr 16 01:12:14
+  file last modified on (UT extra field modtime): 2024 Apr 16 08:12:14 local
+  file last modified on (UT extra field modtime): 2024 Apr 16 08:12:14 UTC
+  32-bit CRC value (hex):                         cf16e70e
+  compressed size:                                341 bytes
+  uncompressed size:                              664 bytes
+  length of filename:                             33 characters
+  length of extra field:                          24 bytes
   length of file comment:                         0 characters
   disk number on which file begins:               disk 1
-  apparent file type:                             binary
-  Unix file attributes (100664 octal):            -rw-rw-r--
+  apparent file type:                             text
+  Unix file attributes (100644 octal):            -rw-r--r--
   MS-DOS file attributes (00 hex):                none
 
+  The central-directory extra field contains:
+  - A subfield with ID 0x5455 (universal time) and 5 data bytes.
+    The local extra field has UTC/GMT modification/access times.
+  - A subfield with ID 0x7875 (Unix UID/GID (any size)) and 11 data bytes:
+    01 04 e3 3d 03 00 04 64 00 00 00.
+
   There is no file comment.
 
 Central directory entry #15:
 ---------------------------
 
-  tests/torchtune/_cli/test_cp.py
+  recipes/configs/gemma/
 
-  offset of local header from start of archive:   13302
-                                                  (00000000000033F6h) bytes
+  offset of local header from start of archive:   39908
+                                                  (0000000000009BE4h) bytes
   file system or operating system of origin:      Unix
-  version of encoding software:                   2.0
+  version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
-  minimum software version required to extract:   2.0
-  compression method:                             deflated
-  compression sub-type (deflation):               normal
+  minimum software version required to extract:   1.0
+  compression method:                             none (stored)
   file security status:                           not encrypted
   extended local header:                          no
-  file last modified on (DOS date/time):          2024 Mar 21 19:57:36
-  32-bit CRC value (hex):                         50ae0add
-  compressed size:                                979 bytes
-  uncompressed size:                              3041 bytes
-  length of filename:                             31 characters
-  length of extra field:                          0 bytes
+  file last modified on (DOS date/time):          2024 Apr 15 20:08:26
+  file last modified on (UT extra field modtime): 2024 Apr 16 03:08:26 local
+  file last modified on (UT extra field modtime): 2024 Apr 16 03:08:26 UTC
+  32-bit CRC value (hex):                         00000000
+  compressed size:                                0 bytes
+  uncompressed size:                              0 bytes
+  length of filename:                             22 characters
+  length of extra field:                          24 bytes
   length of file comment:                         0 characters
   disk number on which file begins:               disk 1
   apparent file type:                             binary
-  Unix file attributes (100664 octal):            -rw-rw-r--
-  MS-DOS file attributes (00 hex):                none
+  Unix file attributes (040755 octal):            drwxr-xr-x
+  MS-DOS file attributes (10 hex):                dir 
+
+  The central-directory extra field contains:
+  - A subfield with ID 0x5455 (universal time) and 5 data bytes.
+    The local extra field has UTC/GMT modification/access times.
+  - A subfield with ID 0x7875 (Unix UID/GID (any size)) and 11 data bytes:
+    01 04 e3 3d 03 00 04 64 00 00 00.
 
   There is no file comment.
 
 Central directory entry #16:
 ---------------------------
 
-  tests/torchtune/_cli/test_download.py
+  recipes/configs/gemma/2B_full.yaml
 
-  offset of local header from start of archive:   14342
-                                                  (0000000000003806h) bytes
+  offset of local header from start of archive:   39988
+                                                  (0000000000009C34h) bytes
   file system or operating system of origin:      Unix
-  version of encoding software:                   2.0
+  version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
-  compression sub-type (deflation):               normal
+  compression sub-type (deflation):               maximum
   file security status:                           not encrypted
   extended local header:                          no
-  file last modified on (DOS date/time):          2024 Mar 21 19:57:36
-  32-bit CRC value (hex):                         6d808fd8
-  compressed size:                                562 bytes
-  uncompressed size:                              1228 bytes
-  length of filename:                             37 characters
-  length of extra field:                          0 bytes
+  file last modified on (DOS date/time):          2024 Apr 16 01:12:14
+  file last modified on (UT extra field modtime): 2024 Apr 16 08:12:14 local
+  file last modified on (UT extra field modtime): 2024 Apr 16 08:12:14 UTC
+  32-bit CRC value (hex):                         dd8b71ce
+  compressed size:                                869 bytes
+  uncompressed size:                              1925 bytes
+  length of filename:                             34 characters
+  length of extra field:                          24 bytes
   length of file comment:                         0 characters
   disk number on which file begins:               disk 1
-  apparent file type:                             binary
-  Unix file attributes (100664 octal):            -rw-rw-r--
+  apparent file type:                             text
+  Unix file attributes (100644 octal):            -rw-r--r--
   MS-DOS file attributes (00 hex):                none
 
+  The central-directory extra field contains:
+  - A subfield with ID 0x5455 (universal time) and 5 data bytes.
+    The local extra field has UTC/GMT modification/access times.
+  - A subfield with ID 0x7875 (Unix UID/GID (any size)) and 11 data bytes:
+    01 04 e3 3d 03 00 04 64 00 00 00.
+
   There is no file comment.
 
 Central directory entry #17:
 ---------------------------
 
-  tests/torchtune/_cli/test_ls.py
+  recipes/configs/llama2/
 
-  offset of local header from start of archive:   14971
-                                                  (0000000000003A7Bh) bytes
+  offset of local header from start of archive:   40949
+                                                  (0000000000009FF5h) bytes
   file system or operating system of origin:      Unix
-  version of encoding software:                   2.0
+  version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
-  minimum software version required to extract:   2.0
-  compression method:                             deflated
-  compression sub-type (deflation):               normal
+  minimum software version required to extract:   1.0
+  compression method:                             none (stored)
   file security status:                           not encrypted
   extended local header:                          no
-  file last modified on (DOS date/time):          2024 Mar 21 19:57:36
-  32-bit CRC value (hex):                         28a451ef
-  compressed size:                                533 bytes
-  uncompressed size:                              1141 bytes
-  length of filename:                             31 characters
-  length of extra field:                          0 bytes
+  file last modified on (DOS date/time):          2024 Apr 15 20:08:26
+  file last modified on (UT extra field modtime): 2024 Apr 16 03:08:26 local
+  file last modified on (UT extra field modtime): 2024 Apr 16 03:08:26 UTC
+  32-bit CRC value (hex):                         00000000
+  compressed size:                                0 bytes
+  uncompressed size:                              0 bytes
+  length of filename:                             23 characters
+  length of extra field:                          24 bytes
   length of file comment:                         0 characters
   disk number on which file begins:               disk 1
   apparent file type:                             binary
-  Unix file attributes (100664 octal):            -rw-rw-r--
-  MS-DOS file attributes (00 hex):                none
+  Unix file attributes (040755 octal):            drwxr-xr-x
+  MS-DOS file attributes (10 hex):                dir 
+
+  The central-directory extra field contains:
+  - A subfield with ID 0x5455 (universal time) and 5 data bytes.
+    The local extra field has UTC/GMT modification/access times.
+  - A subfield with ID 0x7875 (Unix UID/GID (any size)) and 11 data bytes:
+    01 04 e3 3d 03 00 04 64 00 00 00.
 
   There is no file comment.
 
 Central directory entry #18:
 ---------------------------
 
-  tests/torchtune/_cli/test_tune.py
+  recipes/configs/llama2/13B_full.yaml
 
-  offset of local header from start of archive:   15565
-                                                  (0000000000003CCDh) bytes
+  offset of local header from start of archive:   41030
+                                                  (000000000000A046h) bytes
   file system or operating system of origin:      Unix
-  version of encoding software:                   2.0
+  version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
-  compression sub-type (deflation):               normal
+  compression sub-type (deflation):               maximum
   file security status:                           not encrypted
   extended local header:                          no
-  file last modified on (DOS date/time):          2024 Mar 21 19:57:36
-  32-bit CRC value (hex):                         ef240144
-  compressed size:                                423 bytes
-  uncompressed size:                              1096 bytes
-  length of filename:                             33 characters
-  length of extra field:                          0 bytes
+  file last modified on (DOS date/time):          2024 Apr 16 01:12:14
+  file last modified on (UT extra field modtime): 2024 Apr 16 08:12:14 local
+  file last modified on (UT extra field modtime): 2024 Apr 16 08:12:14 UTC
+  32-bit CRC value (hex):                         82a1a464
+  compressed size:                                948 bytes
+  uncompressed size:                              2163 bytes
+  length of filename:                             36 characters
+  length of extra field:                          24 bytes
   length of file comment:                         0 characters
   disk number on which file begins:               disk 1
-  apparent file type:                             binary
-  Unix file attributes (100664 octal):            -rw-rw-r--
+  apparent file type:                             text
+  Unix file attributes (100644 octal):            -rw-r--r--
   MS-DOS file attributes (00 hex):                none
 
+  The central-directory extra field contains:
+  - A subfield with ID 0x5455 (universal time) and 5 data bytes.
+    The local extra field has UTC/GMT modification/access times.
+  - A subfield with ID 0x7875 (Unix UID/GID (any size)) and 11 data bytes:
+    01 04 e3 3d 03 00 04 64 00 00 00.
+
   There is no file comment.
 
 Central directory entry #19:
 ---------------------------
 
-  tests/torchtune/_cli/test_validate.py
+  recipes/configs/llama2/13B_lora.yaml
 
-  offset of local header from start of archive:   16051
-                                                  (0000000000003EB3h) bytes
+  offset of local header from start of archive:   42072
+                                                  (000000000000A458h) bytes
   file system or operating system of origin:      Unix
-  version of encoding software:                   2.0
+  version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
-  compression sub-type (deflation):               normal
+  compression sub-type (deflation):               maximum
   file security status:                           not encrypted
   extended local header:                          no
-  file last modified on (DOS date/time):          2024 Mar 21 19:57:36
-  32-bit CRC value (hex):                         fd7bd8ae
-  compressed size:                                617 bytes
-  uncompressed size:                              1673 bytes
-  length of filename:                             37 characters
-  length of extra field:                          0 bytes
+  file last modified on (DOS date/time):          2024 Apr 16 01:12:14
+  file last modified on (UT extra field modtime): 2024 Apr 16 08:12:14 local
+  file last modified on (UT extra field modtime): 2024 Apr 16 08:12:14 UTC
+  32-bit CRC value (hex):                         de028e83
+  compressed size:                                1042 bytes
+  uncompressed size:                              2441 bytes
+  length of filename:                             36 characters
+  length of extra field:                          24 bytes
   length of file comment:                         0 characters
   disk number on which file begins:               disk 1
-  apparent file type:                             binary
-  Unix file attributes (100664 octal):            -rw-rw-r--
+  apparent file type:                             text
+  Unix file attributes (100644 octal):            -rw-r--r--
   MS-DOS file attributes (00 hex):                none
 
+  The central-directory extra field contains:
+  - A subfield with ID 0x5455 (universal time) and 5 data bytes.
+    The local extra field has UTC/GMT modification/access times.
+  - A subfield with ID 0x7875 (Unix UID/GID (any size)) and 11 data bytes:
+    01 04 e3 3d 03 00 04 64 00 00 00.
+
   There is no file comment.
 
 Central directory entry #20:
 ---------------------------
 
-  tests/torchtune/datasets/__init__.py
+  recipes/configs/llama2/7B_full.yaml
 
-  offset of local header from start of archive:   16735
-                                                  (000000000000415Fh) bytes
+  offset of local header from start of archive:   43208
+                                                  (000000000000A8C8h) bytes
   file system or operating system of origin:      Unix
-  version of encoding software:                   2.0
+  version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
-  compression sub-type (deflation):               normal
+  compression sub-type (deflation):               maximum
   file security status:                           not encrypted
   extended local header:                          no
-  file last modified on (DOS date/time):          2024 Mar 21 19:57:36
-  32-bit CRC value (hex):                         2ca9d797
-  compressed size:                                150 bytes
-  uncompressed size:                              208 bytes
-  length of filename:                             36 characters
-  length of extra field:                          0 bytes
+  file last modified on (DOS date/time):          2024 Apr 16 01:12:14
+  file last modified on (UT extra field modtime): 2024 Apr 16 08:12:14 local
+  file last modified on (UT extra field modtime): 2024 Apr 16 08:12:14 UTC
+  32-bit CRC value (hex):                         4814f495
+  compressed size:                                925 bytes
+  uncompressed size:                              2083 bytes
+  length of filename:                             35 characters
+  length of extra field:                          24 bytes
   length of file comment:                         0 characters
   disk number on which file begins:               disk 1
-  apparent file type:                             binary
-  Unix file attributes (100664 octal):            -rw-rw-r--
+  apparent file type:                             text
+  Unix file attributes (100644 octal):            -rw-r--r--
   MS-DOS file attributes (00 hex):                none
 
+  The central-directory extra field contains:
+  - A subfield with ID 0x5455 (universal time) and 5 data bytes.
+    The local extra field has UTC/GMT modification/access times.
+  - A subfield with ID 0x7875 (Unix UID/GID (any size)) and 11 data bytes:
+    01 04 e3 3d 03 00 04 64 00 00 00.
+
   There is no file comment.
 
 Central directory entry #21:
 ---------------------------
 
-  tests/torchtune/datasets/test_alpaca_dataset.py
+  recipes/configs/llama2/7B_full_low_memory.yaml
 
-  offset of local header from start of archive:   16951
-                                                  (0000000000004237h) bytes
+  offset of local header from start of archive:   44226
+                                                  (000000000000ACC2h) bytes
   file system or operating system of origin:      Unix
-  version of encoding software:                   2.0
+  version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
-  compression sub-type (deflation):               normal
+  compression sub-type (deflation):               maximum
   file security status:                           not encrypted
   extended local header:                          no
-  file last modified on (DOS date/time):          2024 Mar 21 19:57:36
-  32-bit CRC value (hex):                         246ed762
-  compressed size:                                1083 bytes
-  uncompressed size:                              4342 bytes
-  length of filename:                             47 characters
-  length of extra field:                          0 bytes
+  file last modified on (DOS date/time):          2024 Apr 16 01:12:14
+  file last modified on (UT extra field modtime): 2024 Apr 16 08:12:14 local
+  file last modified on (UT extra field modtime): 2024 Apr 16 08:12:14 UTC
+  32-bit CRC value (hex):                         2f42912a
+  compressed size:                                926 bytes
+  uncompressed size:                              2117 bytes
+  length of filename:                             46 characters
+  length of extra field:                          24 bytes
   length of file comment:                         0 characters
   disk number on which file begins:               disk 1
-  apparent file type:                             binary
-  Unix file attributes (100664 octal):            -rw-rw-r--
+  apparent file type:                             text
+  Unix file attributes (100644 octal):            -rw-r--r--
   MS-DOS file attributes (00 hex):                none
 
+  The central-directory extra field contains:
+  - A subfield with ID 0x5455 (universal time) and 5 data bytes.
+    The local extra field has UTC/GMT modification/access times.
+  - A subfield with ID 0x7875 (Unix UID/GID (any size)) and 11 data bytes:
+    01 04 e3 3d 03 00 04 64 00 00 00.
+
   There is no file comment.
 
 Central directory entry #22:
 ---------------------------
 
-  tests/torchtune/datasets/test_instruct_dataset.py
+  recipes/configs/llama2/7B_lora.yaml
 
-  offset of local header from start of archive:   18111
-                                                  (00000000000046BFh) bytes
+  offset of local header from start of archive:   45256
+                                                  (000000000000B0C8h) bytes
   file system or operating system of origin:      Unix
-  version of encoding software:                   2.0
+  version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
-  compression sub-type (deflation):               normal
+  compression sub-type (deflation):               maximum
   file security status:                           not encrypted
   extended local header:                          no
-  file last modified on (DOS date/time):          2024 Mar 21 19:57:36
-  32-bit CRC value (hex):                         98c4d82c
-  compressed size:                                1204 bytes
-  uncompressed size:                              4294 bytes
-  length of filename:                             49 characters
-  length of extra field:                          0 bytes
+  file last modified on (DOS date/time):          2024 Apr 16 01:12:14
+  file last modified on (UT extra field modtime): 2024 Apr 16 08:12:14 local
+  file last modified on (UT extra field modtime): 2024 Apr 16 08:12:14 UTC
+  32-bit CRC value (hex):                         58922817
+  compressed size:                                1010 bytes
+  uncompressed size:                              2326 bytes
+  length of filename:                             35 characters
+  length of extra field:                          24 bytes
   length of file comment:                         0 characters
   disk number on which file begins:               disk 1
-  apparent file type:                             binary
-  Unix file attributes (100664 octal):            -rw-rw-r--
+  apparent file type:                             text
+  Unix file attributes (100644 octal):            -rw-r--r--
   MS-DOS file attributes (00 hex):                none
 
+  The central-directory extra field contains:
+  - A subfield with ID 0x5455 (universal time) and 5 data bytes.
+    The local extra field has UTC/GMT modification/access times.
+  - A subfield with ID 0x7875 (Unix UID/GID (any size)) and 11 data bytes:
+    01 04 e3 3d 03 00 04 64 00 00 00.
+
   There is no file comment.
 
 Central directory entry #23:
 ---------------------------
 
-  tests/torchtune/datasets/test_slimorca_dataset.py
+  recipes/configs/llama2/7B_lora_dpo_single_device.yaml
 
-  offset of local header from start of archive:   19394
-                                                  (0000000000004BC2h) bytes
+  offset of local header from start of archive:   46359
+                                                  (000000000000B517h) bytes
   file system or operating system of origin:      Unix
-  version of encoding software:                   2.0
+  version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
-  compression sub-type (deflation):               normal
+  compression sub-type (deflation):               maximum
   file security status:                           not encrypted
   extended local header:                          no
-  file last modified on (DOS date/time):          2024 Mar 21 19:57:36
-  32-bit CRC value (hex):                         5353df81
-  compressed size:                                1579 bytes
-  uncompressed size:                              5652 bytes
-  length of filename:                             49 characters
-  length of extra field:                          0 bytes
+  file last modified on (DOS date/time):          2024 Apr 16 01:12:14
+  file last modified on (UT extra field modtime): 2024 Apr 16 08:12:14 local
+  file last modified on (UT extra field modtime): 2024 Apr 16 08:12:14 UTC
+  32-bit CRC value (hex):                         38438e73
+  compressed size:                                989 bytes
+  uncompressed size:                              2262 bytes
+  length of filename:                             53 characters
+  length of extra field:                          24 bytes
   length of file comment:                         0 characters
   disk number on which file begins:               disk 1
-  apparent file type:                             binary
-  Unix file attributes (100664 octal):            -rw-rw-r--
+  apparent file type:                             text
+  Unix file attributes (100644 octal):            -rw-r--r--
   MS-DOS file attributes (00 hex):                none
 
+  The central-directory extra field contains:
+  - A subfield with ID 0x5455 (universal time) and 5 data bytes.
+    The local extra field has UTC/GMT modification/access times.
+  - A subfield with ID 0x7875 (Unix UID/GID (any size)) and 11 data bytes:
+    01 04 e3 3d 03 00 04 64 00 00 00.
+
   There is no file comment.
 
 Central directory entry #24:
 ---------------------------
 
-  tests/torchtune/generation/__init__.py
+  recipes/configs/llama2/7B_lora_single_device.yaml
 
-  offset of local header from start of archive:   21052
-                                                  (000000000000523Ch) bytes
+  offset of local header from start of archive:   47459
+                                                  (000000000000B963h) bytes
   file system or operating system of origin:      Unix
-  version of encoding software:                   2.0
+  version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
-  compression sub-type (deflation):               normal
+  compression sub-type (deflation):               maximum
   file security status:                           not encrypted
   extended local header:                          no
-  file last modified on (DOS date/time):          2024 Mar 21 19:57:36
-  32-bit CRC value (hex):                         2ca9d797
-  compressed size:                                150 bytes
-  uncompressed size:                              208 bytes
-  length of filename:                             38 characters
-  length of extra field:                          0 bytes
+  file last modified on (DOS date/time):          2024 Apr 16 01:12:14
+  file last modified on (UT extra field modtime): 2024 Apr 16 08:12:14 local
+  file last modified on (UT extra field modtime): 2024 Apr 16 08:12:14 UTC
+  32-bit CRC value (hex):                         74974605
+  compressed size:                                1035 bytes
+  uncompressed size:                              2423 bytes
+  length of filename:                             49 characters
+  length of extra field:                          24 bytes
   length of file comment:                         0 characters
   disk number on which file begins:               disk 1
-  apparent file type:                             binary
-  Unix file attributes (100664 octal):            -rw-rw-r--
+  apparent file type:                             text
+  Unix file attributes (100644 octal):            -rw-r--r--
   MS-DOS file attributes (00 hex):                none
 
+  The central-directory extra field contains:
+  - A subfield with ID 0x5455 (universal time) and 5 data bytes.
+    The local extra field has UTC/GMT modification/access times.
+  - A subfield with ID 0x7875 (Unix UID/GID (any size)) and 11 data bytes:
+    01 04 e3 3d 03 00 04 64 00 00 00.
+
   There is no file comment.
 
 Central directory entry #25:
 ---------------------------
 
-  tests/torchtune/generation/test_generation.py
+  recipes/configs/llama2/7B_qlora_single_device.yaml
 
-  offset of local header from start of archive:   21270
-                                                  (0000000000005316h) bytes
+  offset of local header from start of archive:   48601
+                                                  (000000000000BDD9h) bytes
   file system or operating system of origin:      Unix
-  version of encoding software:                   2.0
+  version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
-  compression sub-type (deflation):               normal
+  compression sub-type (deflation):               maximum
   file security status:                           not encrypted
   extended local header:                          no
-  file last modified on (DOS date/time):          2024 Mar 21 19:57:36
-  32-bit CRC value (hex):                         34f83fb1
-  compressed size:                                2191 bytes
-  uncompressed size:                              9521 bytes
-  length of filename:                             45 characters
-  length of extra field:                          0 bytes
+  file last modified on (DOS date/time):          2024 Apr 16 01:12:14
+  file last modified on (UT extra field modtime): 2024 Apr 16 08:12:14 local
+  file last modified on (UT extra field modtime): 2024 Apr 16 08:12:14 UTC
+  32-bit CRC value (hex):                         a2617633
+  compressed size:                                1097 bytes
+  uncompressed size:                              2528 bytes
+  length of filename:                             50 characters
+  length of extra field:                          24 bytes
   length of file comment:                         0 characters
   disk number on which file begins:               disk 1
-  apparent file type:                             binary
-  Unix file attributes (100664 octal):            -rw-rw-r--
+  apparent file type:                             text
+  Unix file attributes (100644 octal):            -rw-r--r--
   MS-DOS file attributes (00 hex):                none
 
+  The central-directory extra field contains:
+  - A subfield with ID 0x5455 (universal time) and 5 data bytes.
+    The local extra field has UTC/GMT modification/access times.
+  - A subfield with ID 0x7875 (Unix UID/GID (any size)) and 11 data bytes:
+    01 04 e3 3d 03 00 04 64 00 00 00.
+
   There is no file comment.
 
 Central directory entry #26:
 ---------------------------
 
-  tests/torchtune/models/__init__.py
+  recipes/configs/mistral/
 
-  offset of local header from start of archive:   23536
-                                                  (0000000000005BF0h) bytes
+  offset of local header from start of archive:   49806
+                                                  (000000000000C28Eh) bytes
   file system or operating system of origin:      Unix
-  version of encoding software:                   2.0
+  version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
-  minimum software version required to extract:   2.0
-  compression method:                             deflated
-  compression sub-type (deflation):               normal
+  minimum software version required to extract:   1.0
+  compression method:                             none (stored)
   file security status:                           not encrypted
   extended local header:                          no
-  file last modified on (DOS date/time):          2024 Mar 21 19:57:36
-  32-bit CRC value (hex):                         2ca9d797
-  compressed size:                                150 bytes
-  uncompressed size:                              208 bytes
-  length of filename:                             34 characters
-  length of extra field:                          0 bytes
+  file last modified on (DOS date/time):          2024 Apr 15 20:08:26
+  file last modified on (UT extra field modtime): 2024 Apr 16 03:08:26 local
+  file last modified on (UT extra field modtime): 2024 Apr 16 03:08:26 UTC
+  32-bit CRC value (hex):                         00000000
+  compressed size:                                0 bytes
+  uncompressed size:                              0 bytes
+  length of filename:                             24 characters
+  length of extra field:                          24 bytes
   length of file comment:                         0 characters
   disk number on which file begins:               disk 1
   apparent file type:                             binary
-  Unix file attributes (100664 octal):            -rw-rw-r--
-  MS-DOS file attributes (00 hex):                none
+  Unix file attributes (040755 octal):            drwxr-xr-x
+  MS-DOS file attributes (10 hex):                dir 
+
+  The central-directory extra field contains:
+  - A subfield with ID 0x5455 (universal time) and 5 data bytes.
+    The local extra field has UTC/GMT modification/access times.
+  - A subfield with ID 0x7875 (Unix UID/GID (any size)) and 11 data bytes:
+    01 04 e3 3d 03 00 04 64 00 00 00.
 
   There is no file comment.
 
 Central directory entry #27:
 ---------------------------
 
-  tests/torchtune/models/test_lora_llama2.py
+  recipes/configs/mistral/7B_full.yaml
 
-  offset of local header from start of archive:   23750
-                                                  (0000000000005CC6h) bytes
+  offset of local header from start of archive:   49888
+                                                  (000000000000C2E0h) bytes
   file system or operating system of origin:      Unix
-  version of encoding software:                   2.0
+  version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
-  compression sub-type (deflation):               normal
+  compression sub-type (deflation):               maximum
   file security status:                           not encrypted
   extended local header:                          no
-  file last modified on (DOS date/time):          2024 Mar 21 19:57:36
-  32-bit CRC value (hex):                         00c2c075
-  compressed size:                                1389 bytes
-  uncompressed size:                              5343 bytes
-  length of filename:                             42 characters
-  length of extra field:                          0 bytes
+  file last modified on (DOS date/time):          2024 Apr 16 01:12:14
+  file last modified on (UT extra field modtime): 2024 Apr 16 08:12:14 local
+  file last modified on (UT extra field modtime): 2024 Apr 16 08:12:14 UTC
+  32-bit CRC value (hex):                         96dce715
+  compressed size:                                1014 bytes
+  uncompressed size:                              2260 bytes
+  length of filename:                             36 characters
+  length of extra field:                          24 bytes
   length of file comment:                         0 characters
   disk number on which file begins:               disk 1
-  apparent file type:                             binary
-  Unix file attributes (100664 octal):            -rw-rw-r--
+  apparent file type:                             text
+  Unix file attributes (100644 octal):            -rw-r--r--
   MS-DOS file attributes (00 hex):                none
 
+  The central-directory extra field contains:
+  - A subfield with ID 0x5455 (universal time) and 5 data bytes.
+    The local extra field has UTC/GMT modification/access times.
+  - A subfield with ID 0x7875 (Unix UID/GID (any size)) and 11 data bytes:
+    01 04 e3 3d 03 00 04 64 00 00 00.
+
   There is no file comment.
 
 Central directory entry #28:
 ---------------------------
 
-  tests/torchtune/modules/__init__.py
+  recipes/configs/mistral/7B_full_low_memory.yaml
 
-  offset of local header from start of archive:   25211
-                                                  (000000000000627Bh) bytes
+  offset of local header from start of archive:   50996
+                                                  (000000000000C734h) bytes
   file system or operating system of origin:      Unix
-  version of encoding software:                   2.0
+  version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
-  compression sub-type (deflation):               normal
+  compression sub-type (deflation):               maximum
   file security status:                           not encrypted
   extended local header:                          no
-  file last modified on (DOS date/time):          2024 Mar 21 19:57:36
-  32-bit CRC value (hex):                         2ca9d797
-  compressed size:                                150 bytes
-  uncompressed size:                              208 bytes
-  length of filename:                             35 characters
-  length of extra field:                          0 bytes
+  file last modified on (DOS date/time):          2024 Apr 16 01:12:14
+  file last modified on (UT extra field modtime): 2024 Apr 16 08:12:14 local
+  file last modified on (UT extra field modtime): 2024 Apr 16 08:12:14 UTC
+  32-bit CRC value (hex):                         860bb526
+  compressed size:                                1014 bytes
+  uncompressed size:                              2321 bytes
+  length of filename:                             47 characters
+  length of extra field:                          24 bytes
   length of file comment:                         0 characters
   disk number on which file begins:               disk 1
-  apparent file type:                             binary
-  Unix file attributes (100664 octal):            -rw-rw-r--
+  apparent file type:                             text
+  Unix file attributes (100644 octal):            -rw-r--r--
   MS-DOS file attributes (00 hex):                none
 
+  The central-directory extra field contains:
+  - A subfield with ID 0x5455 (universal time) and 5 data bytes.
+    The local extra field has UTC/GMT modification/access times.
+  - A subfield with ID 0x7875 (Unix UID/GID (any size)) and 11 data bytes:
+    01 04 e3 3d 03 00 04 64 00 00 00.
+
   There is no file comment.
 
 Central directory entry #29:
 ---------------------------
 
-  tests/torchtune/modules/test_attention.py
+  recipes/configs/mistral/7B_lora.yaml
 
-  offset of local header from start of archive:   25426
-                                                  (0000000000006352h) bytes
+  offset of local header from start of archive:   52115
+                                                  (000000000000CB93h) bytes
   file system or operating system of origin:      Unix
-  version of encoding software:                   2.0
+  version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
-  compression sub-type (deflation):               normal
+  compression sub-type (deflation):               maximum
   file security status:                           not encrypted
   extended local header:                          no
-  file last modified on (DOS date/time):          2024 Mar 21 19:57:36
-  32-bit CRC value (hex):                         999c150b
-  compressed size:                                1634 bytes
-  uncompressed size:                              12938 bytes
-  length of filename:                             41 characters
-  length of extra field:                          0 bytes
+  file last modified on (DOS date/time):          2024 Apr 16 01:12:14
+  file last modified on (UT extra field modtime): 2024 Apr 16 08:12:14 local
+  file last modified on (UT extra field modtime): 2024 Apr 16 08:12:14 UTC
+  32-bit CRC value (hex):                         ba73a4c0
+  compressed size:                                1107 bytes
+  uncompressed size:                              2502 bytes
+  length of filename:                             36 characters
+  length of extra field:                          24 bytes
   length of file comment:                         0 characters
   disk number on which file begins:               disk 1
-  apparent file type:                             binary
-  Unix file attributes (100664 octal):            -rw-rw-r--
+  apparent file type:                             text
+  Unix file attributes (100644 octal):            -rw-r--r--
   MS-DOS file attributes (00 hex):                none
 
+  The central-directory extra field contains:
+  - A subfield with ID 0x5455 (universal time) and 5 data bytes.
+    The local extra field has UTC/GMT modification/access times.
+  - A subfield with ID 0x7875 (Unix UID/GID (any size)) and 11 data bytes:
+    01 04 e3 3d 03 00 04 64 00 00 00.
+
   There is no file comment.
 
 Central directory entry #30:
 ---------------------------
 
-  tests/torchtune/modules/test_cosine_with_warmup.py
+  recipes/configs/mistral/7B_lora_single_device.yaml
 
-  offset of local header from start of archive:   27131
-                                                  (00000000000069FBh) bytes
+  offset of local header from start of archive:   53316
+                                                  (000000000000D044h) bytes
   file system or operating system of origin:      Unix
-  version of encoding software:                   2.0
+  version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
-  compression sub-type (deflation):               normal
+  compression sub-type (deflation):               maximum
   file security status:                           not encrypted
   extended local header:                          no
-  file last modified on (DOS date/time):          2024 Mar 21 19:57:36
-  32-bit CRC value (hex):                         5fa08d16
-  compressed size:                                526 bytes
-  uncompressed size:                              1942 bytes
+  file last modified on (DOS date/time):          2024 Apr 16 01:12:14
+  file last modified on (UT extra field modtime): 2024 Apr 16 08:12:14 local
+  file last modified on (UT extra field modtime): 2024 Apr 16 08:12:14 UTC
+  32-bit CRC value (hex):                         bf8cdf6c
+  compressed size:                                1132 bytes
+  uncompressed size:                              2618 bytes
   length of filename:                             50 characters
-  length of extra field:                          0 bytes
+  length of extra field:                          24 bytes
   length of file comment:                         0 characters
   disk number on which file begins:               disk 1
-  apparent file type:                             binary
-  Unix file attributes (100664 octal):            -rw-rw-r--
+  apparent file type:                             text
+  Unix file attributes (100644 octal):            -rw-r--r--
   MS-DOS file attributes (00 hex):                none
 
+  The central-directory extra field contains:
+  - A subfield with ID 0x5455 (universal time) and 5 data bytes.
+    The local extra field has UTC/GMT modification/access times.
+  - A subfield with ID 0x7875 (Unix UID/GID (any size)) and 11 data bytes:
+    01 04 e3 3d 03 00 04 64 00 00 00.
+
   There is no file comment.
 
 Central directory entry #31:
 ---------------------------
 
-  tests/torchtune/modules/test_feed_forward.py
+  recipes/configs/mistral/7B_qlora_single_device.yaml
 
-  offset of local header from start of archive:   27737
-                                                  (0000000000006C59h) bytes
+  offset of local header from start of archive:   54556
+                                                  (000000000000D51Ch) bytes
   file system or operating system of origin:      Unix
-  version of encoding software:                   2.0
+  version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
-  compression sub-type (deflation):               normal
+  compression sub-type (deflation):               maximum
   file security status:                           not encrypted
   extended local header:                          no
-  file last modified on (DOS date/time):          2024 Mar 21 19:57:36
-  32-bit CRC value (hex):                         94bbfb6b
-  compressed size:                                674 bytes
-  uncompressed size:                              1666 bytes
-  length of filename:                             44 characters
-  length of extra field:                          0 bytes
+  file last modified on (DOS date/time):          2024 Apr 16 01:12:14
+  file last modified on (UT extra field modtime): 2024 Apr 16 08:12:14 local
+  file last modified on (UT extra field modtime): 2024 Apr 16 08:12:14 UTC
+  32-bit CRC value (hex):                         a0c20492
+  compressed size:                                1136 bytes
+  uncompressed size:                              2624 bytes
+  length of filename:                             51 characters
+  length of extra field:                          24 bytes
   length of file comment:                         0 characters
   disk number on which file begins:               disk 1
-  apparent file type:                             binary
-  Unix file attributes (100664 octal):            -rw-rw-r--
+  apparent file type:                             text
+  Unix file attributes (100644 octal):            -rw-r--r--
   MS-DOS file attributes (00 hex):                none
 
+  The central-directory extra field contains:
+  - A subfield with ID 0x5455 (universal time) and 5 data bytes.
+    The local extra field has UTC/GMT modification/access times.
+  - A subfield with ID 0x7875 (Unix UID/GID (any size)) and 11 data bytes:
+    01 04 e3 3d 03 00 04 64 00 00 00.
+
   There is no file comment.
 
 Central directory entry #32:
 ---------------------------
 
-  tests/torchtune/modules/test_position_embeddings.py
+  torchtune/
 
-  offset of local header from start of archive:   28485
-                                                  (0000000000006F45h) bytes
+  offset of local header from start of archive:   55801
+                                                  (000000000000D9F9h) bytes
   file system or operating system of origin:      Unix
-  version of encoding software:                   2.0
+  version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
-  minimum software version required to extract:   2.0
-  compression method:                             deflated
-  compression sub-type (deflation):               normal
+  minimum software version required to extract:   1.0
+  compression method:                             none (stored)
   file security status:                           not encrypted
   extended local header:                          no
-  file last modified on (DOS date/time):          2024 Mar 21 19:57:36
-  32-bit CRC value (hex):                         d6fb2736
-  compressed size:                                965 bytes
-  uncompressed size:                              2972 bytes
-  length of filename:                             51 characters
-  length of extra field:                          0 bytes
+  file last modified on (DOS date/time):          2024 Apr 15 20:08:26
+  file last modified on (UT extra field modtime): 2024 Apr 16 03:08:26 local
+  file last modified on (UT extra field modtime): 2024 Apr 16 03:08:26 UTC
+  32-bit CRC value (hex):                         00000000
+  compressed size:                                0 bytes
+  uncompressed size:                              0 bytes
+  length of filename:                             10 characters
+  length of extra field:                          24 bytes
   length of file comment:                         0 characters
   disk number on which file begins:               disk 1
   apparent file type:                             binary
-  Unix file attributes (100664 octal):            -rw-rw-r--
-  MS-DOS file attributes (00 hex):                none
+  Unix file attributes (040755 octal):            drwxr-xr-x
+  MS-DOS file attributes (10 hex):                dir 
+
+  The central-directory extra field contains:
+  - A subfield with ID 0x5455 (universal time) and 5 data bytes.
+    The local extra field has UTC/GMT modification/access times.
+  - A subfield with ID 0x7875 (Unix UID/GID (any size)) and 11 data bytes:
+    01 04 e3 3d 03 00 04 64 00 00 00.
 
   There is no file comment.
 
 Central directory entry #33:
 ---------------------------
 
-  tests/torchtune/modules/test_rms_norm.py
+  torchtune/__init__.py
 
-  offset of local header from start of archive:   29531
-                                                  (000000000000735Bh) bytes
+  offset of local header from start of archive:   55869
+                                                  (000000000000DA3Dh) bytes
   file system or operating system of origin:      Unix
-  version of encoding software:                   2.0
+  version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
-  compression sub-type (deflation):               normal
+  compression sub-type (deflation):               maximum
   file security status:                           not encrypted
   extended local header:                          no
-  file last modified on (DOS date/time):          2024 Mar 21 19:57:36
-  32-bit CRC value (hex):                         38ed9f6a
-  compressed size:                                705 bytes
-  uncompressed size:                              2057 bytes
-  length of filename:                             40 characters
-  length of extra field:                          0 bytes
+  file last modified on (DOS date/time):          2024 Apr 16 01:13:22
+  file last modified on (UT extra field modtime): 2024 Apr 16 08:13:22 local
+  file last modified on (UT extra field modtime): 2024 Apr 16 08:13:22 UTC
+  32-bit CRC value (hex):                         5832544b
+  compressed size:                                222 bytes
+  uncompressed size:                              337 bytes
+  length of filename:                             21 characters
+  length of extra field:                          24 bytes
   length of file comment:                         0 characters
   disk number on which file begins:               disk 1
-  apparent file type:                             binary
-  Unix file attributes (100664 octal):            -rw-rw-r--
+  apparent file type:                             text
+  Unix file attributes (100644 octal):            -rw-r--r--
   MS-DOS file attributes (00 hex):                none
 
+  The central-directory extra field contains:
+  - A subfield with ID 0x5455 (universal time) and 5 data bytes.
+    The local extra field has UTC/GMT modification/access times.
+  - A subfield with ID 0x7875 (Unix UID/GID (any size)) and 11 data bytes:
+    01 04 e3 3d 03 00 04 64 00 00 00.
+
   There is no file comment.
 
 Central directory entry #34:
 ---------------------------
 
-  tests/torchtune/modules/test_tokenizer.py
+  torchtune/_recipe_registry.py
 
-  offset of local header from start of archive:   30306
-                                                  (0000000000007662h) bytes
+  offset of local header from start of archive:   56170
+                                                  (000000000000DB6Ah) bytes
   file system or operating system of origin:      Unix
-  version of encoding software:                   2.0
+  version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
-  compression sub-type (deflation):               normal
+  compression sub-type (deflation):               maximum
   file security status:                           not encrypted
   extended local header:                          no
-  file last modified on (DOS date/time):          2024 Mar 21 19:57:36
-  32-bit CRC value (hex):                         f41e900a
-  compressed size:                                585 bytes
-  uncompressed size:                              1783 bytes
-  length of filename:                             41 characters
-  length of extra field:                          0 bytes
+  file last modified on (DOS date/time):          2024 Apr 16 01:12:14
+  file last modified on (UT extra field modtime): 2024 Apr 16 08:12:14 local
+  file last modified on (UT extra field modtime): 2024 Apr 16 08:12:14 UTC
+  32-bit CRC value (hex):                         8bcad319
+  compressed size:                                690 bytes
+  uncompressed size:                              3707 bytes
+  length of filename:                             29 characters
+  length of extra field:                          24 bytes
   length of file comment:                         0 characters
   disk number on which file begins:               disk 1
-  apparent file type:                             binary
-  Unix file attributes (100664 octal):            -rw-rw-r--
+  apparent file type:                             text
+  Unix file attributes (100644 octal):            -rw-r--r--
   MS-DOS file attributes (00 hex):                none
 
+  The central-directory extra field contains:
+  - A subfield with ID 0x5455 (universal time) and 5 data bytes.
+    The local extra field has UTC/GMT modification/access times.
+  - A subfield with ID 0x7875 (Unix UID/GID (any size)) and 11 data bytes:
+    01 04 e3 3d 03 00 04 64 00 00 00.
+
   There is no file comment.
 
 Central directory entry #35:
 ---------------------------
 
-  tests/torchtune/modules/test_transformer_decoder.py
+  torchtune/recipe_interfaces.py
 
-  offset of local header from start of archive:   30962
-                                                  (00000000000078F2h) bytes
+  offset of local header from start of archive:   56947
+                                                  (000000000000DE73h) bytes
   file system or operating system of origin:      Unix
-  version of encoding software:                   2.0
+  version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
-  compression sub-type (deflation):               normal
+  compression sub-type (deflation):               maximum
   file security status:                           not encrypted
   extended local header:                          no
-  file last modified on (DOS date/time):          2024 Mar 21 19:57:36
-  32-bit CRC value (hex):                         c89431ab
-  compressed size:                                1764 bytes
-  uncompressed size:                              9041 bytes
-  length of filename:                             51 characters
-  length of extra field:                          0 bytes
+  file last modified on (DOS date/time):          2024 Apr 16 01:12:14
+  file last modified on (UT extra field modtime): 2024 Apr 16 08:12:14 local
+  file last modified on (UT extra field modtime): 2024 Apr 16 08:12:14 UTC
+  32-bit CRC value (hex):                         6f40e852
+  compressed size:                                925 bytes
+  uncompressed size:                              2986 bytes
+  length of filename:                             30 characters
+  length of extra field:                          24 bytes
   length of file comment:                         0 characters
   disk number on which file begins:               disk 1
-  apparent file type:                             binary
-  Unix file attributes (100664 octal):            -rw-rw-r--
+  apparent file type:                             text
+  Unix file attributes (100644 octal):            -rw-r--r--
   MS-DOS file attributes (00 hex):                none
 
+  The central-directory extra field contains:
+  - A subfield with ID 0x5455 (universal time) and 5 data bytes.
+    The local extra field has UTC/GMT modification/access times.
+  - A subfield with ID 0x7875 (Unix UID/GID (any size)) and 11 data bytes:
+    01 04 e3 3d 03 00 04 64 00 00 00.
+
   There is no file comment.
 
 Central directory entry #36:
 ---------------------------
 
-  tests/torchtune/modules/low_precision/__init__.py
+  torchtune/_cli/
 
-  offset of local header from start of archive:   32807
-                                                  (0000000000008027h) bytes
+  offset of local header from start of archive:   57960
+                                                  (000000000000E268h) bytes
   file system or operating system of origin:      Unix
-  version of encoding software:                   2.0
+  version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
-  minimum software version required to extract:   2.0
-  compression method:                             deflated
-  compression sub-type (deflation):               normal
+  minimum software version required to extract:   1.0
+  compression method:                             none (stored)
   file security status:                           not encrypted
   extended local header:                          no
-  file last modified on (DOS date/time):          2024 Mar 21 19:57:36
-  32-bit CRC value (hex):                         2ca9d797
-  compressed size:                                150 bytes
-  uncompressed size:                              208 bytes
-  length of filename:                             49 characters
-  length of extra field:                          0 bytes
+  file last modified on (DOS date/time):          2024 Apr 15 20:08:26
+  file last modified on (UT extra field modtime): 2024 Apr 16 03:08:26 local
+  file last modified on (UT extra field modtime): 2024 Apr 16 03:08:26 UTC
+  32-bit CRC value (hex):                         00000000
+  compressed size:                                0 bytes
+  uncompressed size:                              0 bytes
+  length of filename:                             15 characters
+  length of extra field:                          24 bytes
   length of file comment:                         0 characters
   disk number on which file begins:               disk 1
   apparent file type:                             binary
-  Unix file attributes (100664 octal):            -rw-rw-r--
-  MS-DOS file attributes (00 hex):                none
+  Unix file attributes (040755 octal):            drwxr-xr-x
+  MS-DOS file attributes (10 hex):                dir 
+
+  The central-directory extra field contains:
+  - A subfield with ID 0x5455 (universal time) and 5 data bytes.
+    The local extra field has UTC/GMT modification/access times.
+  - A subfield with ID 0x7875 (Unix UID/GID (any size)) and 11 data bytes:
+    01 04 e3 3d 03 00 04 64 00 00 00.
 
   There is no file comment.
 
 Central directory entry #37:
 ---------------------------
 
-  tests/torchtune/modules/low_precision/test_nf4_linear.py
+  torchtune/_cli/__init__.py
 
-  offset of local header from start of archive:   33036
-                                                  (000000000000810Ch) bytes
+  offset of local header from start of archive:   58033
+                                                  (000000000000E2B1h) bytes
   file system or operating system of origin:      Unix
-  version of encoding software:                   2.0
+  version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
-  compression sub-type (deflation):               normal
+  compression sub-type (deflation):               maximum
   file security status:                           not encrypted
   extended local header:                          no
-  file last modified on (DOS date/time):          2024 Mar 21 19:57:36
-  32-bit CRC value (hex):                         c3438f8f
-  compressed size:                                1571 bytes
-  uncompressed size:                              5045 bytes
-  length of filename:                             56 characters
-  length of extra field:                          0 bytes
+  file last modified on (DOS date/time):          2024 Apr 16 01:12:14
+  file last modified on (UT extra field modtime): 2024 Apr 16 08:12:14 local
+  file last modified on (UT extra field modtime): 2024 Apr 16 08:12:14 UTC
+  32-bit CRC value (hex):                         2ca9d797
+  compressed size:                                150 bytes
+  uncompressed size:                              208 bytes
+  length of filename:                             26 characters
+  length of extra field:                          24 bytes
   length of file comment:                         0 characters
   disk number on which file begins:               disk 1
-  apparent file type:                             binary
-  Unix file attributes (100664 octal):            -rw-rw-r--
+  apparent file type:                             text
+  Unix file attributes (100644 octal):            -rw-r--r--
   MS-DOS file attributes (00 hex):                none
 
+  The central-directory extra field contains:
+  - A subfield with ID 0x5455 (universal time) and 5 data bytes.
+    The local extra field has UTC/GMT modification/access times.
+  - A subfield with ID 0x7875 (Unix UID/GID (any size)) and 11 data bytes:
+    01 04 e3 3d 03 00 04 64 00 00 00.
+
   There is no file comment.
 
 Central directory entry #38:
 ---------------------------
 
-  tests/torchtune/modules/peft/__init__.py
+  torchtune/_cli/cp.py
 
-  offset of local header from start of archive:   34693
-                                                  (0000000000008785h) bytes
+  offset of local header from start of archive:   58267
+                                                  (000000000000E39Bh) bytes
   file system or operating system of origin:      Unix
-  version of encoding software:                   2.0
+  version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
-  compression sub-type (deflation):               normal
+  compression sub-type (deflation):               maximum
   file security status:                           not encrypted
   extended local header:                          no
-  file last modified on (DOS date/time):          2024 Mar 21 19:57:36
-  32-bit CRC value (hex):                         2ca9d797
-  compressed size:                                150 bytes
-  uncompressed size:                              208 bytes
-  length of filename:                             40 characters
-  length of extra field:                          0 bytes
+  file last modified on (DOS date/time):          2024 Apr 16 01:12:14
+  file last modified on (UT extra field modtime): 2024 Apr 16 08:12:14 local
+  file last modified on (UT extra field modtime): 2024 Apr 16 08:12:14 UTC
+  32-bit CRC value (hex):                         a4eeddd2
+  compressed size:                                1485 bytes
+  uncompressed size:                              4285 bytes
+  length of filename:                             20 characters
+  length of extra field:                          24 bytes
   length of file comment:                         0 characters
   disk number on which file begins:               disk 1
-  apparent file type:                             binary
-  Unix file attributes (100664 octal):            -rw-rw-r--
+  apparent file type:                             text
+  Unix file attributes (100644 octal):            -rw-r--r--
   MS-DOS file attributes (00 hex):                none
 
+  The central-directory extra field contains:
+  - A subfield with ID 0x5455 (universal time) and 5 data bytes.
+    The local extra field has UTC/GMT modification/access times.
+  - A subfield with ID 0x7875 (Unix UID/GID (any size)) and 11 data bytes:
+    01 04 e3 3d 03 00 04 64 00 00 00.
+
   There is no file comment.
 
 Central directory entry #39:
 ---------------------------
 
-  tests/torchtune/modules/peft/test_lora.py
+  torchtune/_cli/download.py
 
-  offset of local header from start of archive:   34913
-                                                  (0000000000008861h) bytes
+  offset of local header from start of archive:   59830
+                                                  (000000000000E9B6h) bytes
   file system or operating system of origin:      Unix
-  version of encoding software:                   2.0
+  version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
-  compression sub-type (deflation):               normal
+  compression sub-type (deflation):               maximum
   file security status:                           not encrypted
   extended local header:                          no
-  file last modified on (DOS date/time):          2024 Mar 21 19:57:36
-  32-bit CRC value (hex):                         372ff49c
-  compressed size:                                891 bytes
-  uncompressed size:                              2313 bytes
-  length of filename:                             41 characters
-  length of extra field:                          0 bytes
+  file last modified on (DOS date/time):          2024 Apr 16 01:12:14
+  file last modified on (UT extra field modtime): 2024 Apr 16 08:12:14 local
+  file last modified on (UT extra field modtime): 2024 Apr 16 08:12:14 UTC
+  32-bit CRC value (hex):                         4114eb4a
+  compressed size:                                1465 bytes
+  uncompressed size:                              4516 bytes
+  length of filename:                             26 characters
+  length of extra field:                          24 bytes
   length of file comment:                         0 characters
   disk number on which file begins:               disk 1
-  apparent file type:                             binary
-  Unix file attributes (100664 octal):            -rw-rw-r--
+  apparent file type:                             text
+  Unix file attributes (100644 octal):            -rw-r--r--
   MS-DOS file attributes (00 hex):                none
 
+  The central-directory extra field contains:
+  - A subfield with ID 0x5455 (universal time) and 5 data bytes.
+    The local extra field has UTC/GMT modification/access times.
+  - A subfield with ID 0x7875 (Unix UID/GID (any size)) and 11 data bytes:
+    01 04 e3 3d 03 00 04 64 00 00 00.
+
   There is no file comment.
 
 Central directory entry #40:
 ---------------------------
 
-  tests/torchtune/modules/peft/test_peft_utils.py
+  torchtune/_cli/ls.py
 
-  offset of local header from start of archive:   35875
-                                                  (0000000000008C23h) bytes
+  offset of local header from start of archive:   61379
+                                                  (000000000000EFC3h) bytes
   file system or operating system of origin:      Unix
-  version of encoding software:                   2.0
+  version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
-  compression sub-type (deflation):               normal
+  compression sub-type (deflation):               maximum
   file security status:                           not encrypted
   extended local header:                          no
-  file last modified on (DOS date/time):          2024 Mar 21 19:57:36
-  32-bit CRC value (hex):                         f3d1cd52
-  compressed size:                                2369 bytes
-  uncompressed size:                              12532 bytes
-  length of filename:                             47 characters
-  length of extra field:                          0 bytes
+  file last modified on (DOS date/time):          2024 Apr 16 01:12:14
+  file last modified on (UT extra field modtime): 2024 Apr 16 08:12:14 local
+  file last modified on (UT extra field modtime): 2024 Apr 16 08:12:14 UTC
+  32-bit CRC value (hex):                         28800142
+  compressed size:                                865 bytes
+  uncompressed size:                              2334 bytes
+  length of filename:                             20 characters
+  length of extra field:                          24 bytes
   length of file comment:                         0 characters
   disk number on which file begins:               disk 1
-  apparent file type:                             binary
-  Unix file attributes (100664 octal):            -rw-rw-r--
+  apparent file type:                             text
+  Unix file attributes (100644 octal):            -rw-r--r--
   MS-DOS file attributes (00 hex):                none
 
+  The central-directory extra field contains:
+  - A subfield with ID 0x5455 (universal time) and 5 data bytes.
+    The local extra field has UTC/GMT modification/access times.
+  - A subfield with ID 0x7875 (Unix UID/GID (any size)) and 11 data bytes:
+    01 04 e3 3d 03 00 04 64 00 00 00.
+
   There is no file comment.
 
 Central directory entry #41:
 ---------------------------
 
-  tests/torchtune/utils/__init__.py
+  torchtune/_cli/run.py
 
-  offset of local header from start of archive:   38321
-                                                  (00000000000095B1h) bytes
+  offset of local header from start of archive:   62322
+                                                  (000000000000F372h) bytes
   file system or operating system of origin:      Unix
-  version of encoding software:                   2.0
+  version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
-  compression sub-type (deflation):               normal
+  compression sub-type (deflation):               maximum
   file security status:                           not encrypted
   extended local header:                          no
-  file last modified on (DOS date/time):          2024 Mar 21 19:57:36
-  32-bit CRC value (hex):                         2ca9d797
-  compressed size:                                150 bytes
-  uncompressed size:                              208 bytes
-  length of filename:                             33 characters
-  length of extra field:                          0 bytes
+  file last modified on (DOS date/time):          2024 Apr 16 01:12:14
+  file last modified on (UT extra field modtime): 2024 Apr 16 08:12:14 local
+  file last modified on (UT extra field modtime): 2024 Apr 16 08:12:14 UTC
+  32-bit CRC value (hex):                         3a529902
+  compressed size:                                2266 bytes
+  uncompressed size:                              7246 bytes
+  length of filename:                             21 characters
+  length of extra field:                          24 bytes
   length of file comment:                         0 characters
   disk number on which file begins:               disk 1
-  apparent file type:                             binary
-  Unix file attributes (100664 octal):            -rw-rw-r--
+  apparent file type:                             text
+  Unix file attributes (100644 octal):            -rw-r--r--
   MS-DOS file attributes (00 hex):                none
 
+  The central-directory extra field contains:
+  - A subfield with ID 0x5455 (universal time) and 5 data bytes.
+    The local extra field has UTC/GMT modification/access times.
+  - A subfield with ID 0x7875 (Unix UID/GID (any size)) and 11 data bytes:
+    01 04 e3 3d 03 00 04 64 00 00 00.
+
   There is no file comment.
 
 Central directory entry #42:
 ---------------------------
 
-  tests/torchtune/utils/test_argparse.py
+  torchtune/_cli/subcommand.py
 
-  offset of local header from start of archive:   38534
-                                                  (0000000000009686h) bytes
+  offset of local header from start of archive:   64667
+                                                  (000000000000FC9Bh) bytes
   file system or operating system of origin:      Unix
-  version of encoding software:                   2.0
+  version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
-  compression sub-type (deflation):               normal
+  compression sub-type (deflation):               maximum
   file security status:                           not encrypted
   extended local header:                          no
-  file last modified on (DOS date/time):          2024 Mar 21 19:57:36
-  32-bit CRC value (hex):                         ef54bac6
-  compressed size:                                699 bytes
-  uncompressed size:                              1614 bytes
-  length of filename:                             38 characters
-  length of extra field:                          0 bytes
+  file last modified on (DOS date/time):          2024 Apr 16 01:12:14
+  file last modified on (UT extra field modtime): 2024 Apr 16 08:12:14 local
+  file last modified on (UT extra field modtime): 2024 Apr 16 08:12:14 UTC
+  32-bit CRC value (hex):                         f6fd0055
+  compressed size:                                247 bytes
+  uncompressed size:                              418 bytes
+  length of filename:                             28 characters
+  length of extra field:                          24 bytes
   length of file comment:                         0 characters
   disk number on which file begins:               disk 1
-  apparent file type:                             binary
-  Unix file attributes (100664 octal):            -rw-rw-r--
+  apparent file type:                             text
+  Unix file attributes (100644 octal):            -rw-r--r--
   MS-DOS file attributes (00 hex):                none
 
+  The central-directory extra field contains:
+  - A subfield with ID 0x5455 (universal time) and 5 data bytes.
+    The local extra field has UTC/GMT modification/access times.
+  - A subfield with ID 0x7875 (Unix UID/GID (any size)) and 11 data bytes:
+    01 04 e3 3d 03 00 04 64 00 00 00.
+
   There is no file comment.
 
 Central directory entry #43:
 ---------------------------
 
-  tests/torchtune/utils/test_checkpoint.py
+  torchtune/_cli/tune.py
 
-  offset of local header from start of archive:   39301
-                                                  (0000000000009985h) bytes
+  offset of local header from start of archive:   65000
+                                                  (000000000000FDE8h) bytes
   file system or operating system of origin:      Unix
-  version of encoding software:                   2.0
+  version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
-  compression sub-type (deflation):               normal
+  compression sub-type (deflation):               maximum
   file security status:                           not encrypted
   extended local header:                          no
-  file last modified on (DOS date/time):          2024 Mar 21 19:57:36
-  32-bit CRC value (hex):                         6f97d641
-  compressed size:                                1633 bytes
-  uncompressed size:                              5946 bytes
-  length of filename:                             40 characters
-  length of extra field:                          0 bytes
+  file last modified on (DOS date/time):          2024 Apr 16 01:12:14
+  file last modified on (UT extra field modtime): 2024 Apr 16 08:12:14 local
+  file last modified on (UT extra field modtime): 2024 Apr 16 08:12:14 UTC
+  32-bit CRC value (hex):                         2b730811
+  compressed size:                                630 bytes
+  uncompressed size:                              1486 bytes
+  length of filename:                             22 characters
+  length of extra field:                          24 bytes
   length of file comment:                         0 characters
   disk number on which file begins:               disk 1
-  apparent file type:                             binary
-  Unix file attributes (100664 octal):            -rw-rw-r--
+  apparent file type:                             text
+  Unix file attributes (100644 octal):            -rw-r--r--
   MS-DOS file attributes (00 hex):                none
 
+  The central-directory extra field contains:
+  - A subfield with ID 0x5455 (universal time) and 5 data bytes.
+    The local extra field has UTC/GMT modification/access times.
+  - A subfield with ID 0x7875 (Unix UID/GID (any size)) and 11 data bytes:
+    01 04 e3 3d 03 00 04 64 00 00 00.
+
   There is no file comment.
 
 Central directory entry #44:
 ---------------------------
 
-  tests/torchtune/utils/test_checkpointable_dataloader.py
+  torchtune/_cli/validate.py
 
-  offset of local header from start of archive:   41004
-                                                  (000000000000A02Ch) bytes
+  offset of local header from start of archive:   65710
+                                                  (00000000000100AEh) bytes
   file system or operating system of origin:      Unix
-  version of encoding software:                   2.0
+  version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
-  compression sub-type (deflation):               normal
+  compression sub-type (deflation):               maximum
   file security status:                           not encrypted
   extended local header:                          no
-  file last modified on (DOS date/time):          2024 Mar 21 19:57:36
-  32-bit CRC value (hex):                         be2c2d82
-  compressed size:                                1786 bytes
-  uncompressed size:                              8706 bytes
-  length of filename:                             55 characters
-  length of extra field:                          0 bytes
+  file last modified on (DOS date/time):          2024 Apr 16 01:12:14
+  file last modified on (UT extra field modtime): 2024 Apr 16 08:12:14 local
+  file last modified on (UT extra field modtime): 2024 Apr 16 08:12:14 UTC
+  32-bit CRC value (hex):                         d945fceb
+  compressed size:                                721 bytes
+  uncompressed size:                              1837 bytes
+  length of filename:                             26 characters
+  length of extra field:                          24 bytes
   length of file comment:                         0 characters
   disk number on which file begins:               disk 1
-  apparent file type:                             binary
-  Unix file attributes (100664 octal):            -rw-rw-r--
+  apparent file type:                             text
+  Unix file attributes (100644 octal):            -rw-r--r--
   MS-DOS file attributes (00 hex):                none
 
+  The central-directory extra field contains:
+  - A subfield with ID 0x5455 (universal time) and 5 data bytes.
+    The local extra field has UTC/GMT modification/access times.
+  - A subfield with ID 0x7875 (Unix UID/GID (any size)) and 11 data bytes:
+    01 04 e3 3d 03 00 04 64 00 00 00.
+
   There is no file comment.
 
 Central directory entry #45:
 ---------------------------
 
-  tests/torchtune/utils/test_checkpointer.py
+  torchtune/_cli/hf_upload/
 
-  offset of local header from start of archive:   42875
-                                                  (000000000000A77Bh) bytes
+  offset of local header from start of archive:   66515
+                                                  (00000000000103D3h) bytes
   file system or operating system of origin:      Unix
-  version of encoding software:                   2.0
+  version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
-  minimum software version required to extract:   2.0
-  compression method:                             deflated
-  compression sub-type (deflation):               normal
+  minimum software version required to extract:   1.0
+  compression method:                             none (stored)
   file security status:                           not encrypted
   extended local header:                          no
-  file last modified on (DOS date/time):          2024 Mar 21 19:57:36
-  32-bit CRC value (hex):                         ba1eece3
-  compressed size:                                2364 bytes
-  uncompressed size:                              11542 bytes
-  length of filename:                             42 characters
-  length of extra field:                          0 bytes
+  file last modified on (DOS date/time):          2024 Apr 15 20:08:26
+  file last modified on (UT extra field modtime): 2024 Apr 16 03:08:26 local
+  file last modified on (UT extra field modtime): 2024 Apr 16 03:08:26 UTC
+  32-bit CRC value (hex):                         00000000
+  compressed size:                                0 bytes
+  uncompressed size:                              0 bytes
+  length of filename:                             25 characters
+  length of extra field:                          24 bytes
   length of file comment:                         0 characters
   disk number on which file begins:               disk 1
   apparent file type:                             binary
-  Unix file attributes (100664 octal):            -rw-rw-r--
-  MS-DOS file attributes (00 hex):                none
+  Unix file attributes (040755 octal):            drwxr-xr-x
+  MS-DOS file attributes (10 hex):                dir 
+
+  The central-directory extra field contains:
+  - A subfield with ID 0x5455 (universal time) and 5 data bytes.
+    The local extra field has UTC/GMT modification/access times.
+  - A subfield with ID 0x7875 (Unix UID/GID (any size)) and 11 data bytes:
+    01 04 e3 3d 03 00 04 64 00 00 00.
 
   There is no file comment.
 
 Central directory entry #46:
 ---------------------------
 
-  tests/torchtune/utils/test_collate.py
+  torchtune/_cli/hf_upload/upload.py
 
-  offset of local header from start of archive:   45311
-                                                  (000000000000B0FFh) bytes
+  offset of local header from start of archive:   66598
+                                                  (0000000000010426h) bytes
   file system or operating system of origin:      Unix
-  version of encoding software:                   2.0
+  version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
-  compression sub-type (deflation):               normal
+  compression sub-type (deflation):               maximum
   file security status:                           not encrypted
   extended local header:                          no
-  file last modified on (DOS date/time):          2024 Mar 21 19:57:36
-  32-bit CRC value (hex):                         19e87685
-  compressed size:                                493 bytes
-  uncompressed size:                              1238 bytes
-  length of filename:                             37 characters
-  length of extra field:                          0 bytes
+  file last modified on (DOS date/time):          2024 Apr 16 01:12:14
+  file last modified on (UT extra field modtime): 2024 Apr 16 08:12:14 local
+  file last modified on (UT extra field modtime): 2024 Apr 16 08:12:14 UTC
+  32-bit CRC value (hex):                         40f9cf58
+  compressed size:                                1232 bytes
+  uncompressed size:                              3702 bytes
+  length of filename:                             34 characters
+  length of extra field:                          24 bytes
   length of file comment:                         0 characters
   disk number on which file begins:               disk 1
-  apparent file type:                             binary
-  Unix file attributes (100664 octal):            -rw-rw-r--
+  apparent file type:                             text
+  Unix file attributes (100644 octal):            -rw-r--r--
   MS-DOS file attributes (00 hex):                none
 
+  The central-directory extra field contains:
+  - A subfield with ID 0x5455 (universal time) and 5 data bytes.
+    The local extra field has UTC/GMT modification/access times.
+  - A subfield with ID 0x7875 (Unix UID/GID (any size)) and 11 data bytes:
+    01 04 e3 3d 03 00 04 64 00 00 00.
+
   There is no file comment.
 
 Central directory entry #47:
 ---------------------------
 
-  tests/torchtune/utils/test_device.py
+  torchtune/config/
 
-  offset of local header from start of archive:   45871
-                                                  (000000000000B32Fh) bytes
+  offset of local header from start of archive:   67922
+                                                  (0000000000010952h) bytes
   file system or operating system of origin:      Unix
-  version of encoding software:                   2.0
+  version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
-  minimum software version required to extract:   2.0
-  compression method:                             deflated
-  compression sub-type (deflation):               normal
+  minimum software version required to extract:   1.0
+  compression method:                             none (stored)
   file security status:                           not encrypted
   extended local header:                          no
-  file last modified on (DOS date/time):          2024 Mar 21 19:57:36
-  32-bit CRC value (hex):                         29da63f4
-  compressed size:                                881 bytes
-  uncompressed size:                              2470 bytes
-  length of filename:                             36 characters
-  length of extra field:                          0 bytes
+  file last modified on (DOS date/time):          2024 Apr 15 20:08:26
+  file last modified on (UT extra field modtime): 2024 Apr 16 03:08:26 local
+  file last modified on (UT extra field modtime): 2024 Apr 16 03:08:26 UTC
+  32-bit CRC value (hex):                         00000000
+  compressed size:                                0 bytes
+  uncompressed size:                              0 bytes
+  length of filename:                             17 characters
+  length of extra field:                          24 bytes
   length of file comment:                         0 characters
   disk number on which file begins:               disk 1
   apparent file type:                             binary
-  Unix file attributes (100664 octal):            -rw-rw-r--
-  MS-DOS file attributes (00 hex):                none
+  Unix file attributes (040755 octal):            drwxr-xr-x
+  MS-DOS file attributes (10 hex):                dir 
+
+  The central-directory extra field contains:
+  - A subfield with ID 0x5455 (universal time) and 5 data bytes.
+    The local extra field has UTC/GMT modification/access times.
+  - A subfield with ID 0x7875 (Unix UID/GID (any size)) and 11 data bytes:
+    01 04 e3 3d 03 00 04 64 00 00 00.
 
   There is no file comment.
 
 Central directory entry #48:
 ---------------------------
 
-  tests/torchtune/utils/test_distributed.py
+  torchtune/config/__init__.py
 
-  offset of local header from start of archive:   46818
-                                                  (000000000000B6E2h) bytes
+  offset of local header from start of archive:   67997
+                                                  (000000000001099Dh) bytes
   file system or operating system of origin:      Unix
-  version of encoding software:                   2.0
+  version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
-  compression sub-type (deflation):               normal
+  compression sub-type (deflation):               maximum
   file security status:                           not encrypted
   extended local header:                          no
-  file last modified on (DOS date/time):          2024 Mar 21 19:57:36
-  32-bit CRC value (hex):                         ee1a0d5d
-  compressed size:                                2487 bytes
-  uncompressed size:                              9585 bytes
-  length of filename:                             41 characters
-  length of extra field:                          0 bytes
+  file last modified on (DOS date/time):          2024 Apr 16 01:12:14
+  file last modified on (UT extra field modtime): 2024 Apr 16 08:12:14 local
+  file last modified on (UT extra field modtime): 2024 Apr 16 08:12:14 UTC
+  32-bit CRC value (hex):                         da7bcc6d
+  compressed size:                                233 bytes
+  uncompressed size:                              417 bytes
+  length of filename:                             28 characters
+  length of extra field:                          24 bytes
   length of file comment:                         0 characters
   disk number on which file begins:               disk 1
-  apparent file type:                             binary
-  Unix file attributes (100664 octal):            -rw-rw-r--
+  apparent file type:                             text
+  Unix file attributes (100644 octal):            -rw-r--r--
   MS-DOS file attributes (00 hex):                none
 
+  The central-directory extra field contains:
+  - A subfield with ID 0x5455 (universal time) and 5 data bytes.
+    The local extra field has UTC/GMT modification/access times.
+  - A subfield with ID 0x7875 (Unix UID/GID (any size)) and 11 data bytes:
+    01 04 e3 3d 03 00 04 64 00 00 00.
+
   There is no file comment.
 
 Central directory entry #49:
 ---------------------------
 
-  tests/torchtune/utils/test_logits_transforms.py
+  torchtune/config/_errors.py
 
-  offset of local header from start of archive:   49376
-                                                  (000000000000C0E0h) bytes
+  offset of local header from start of archive:   68316
+                                                  (0000000000010ADCh) bytes
   file system or operating system of origin:      Unix
-  version of encoding software:                   2.0
+  version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
-  compression sub-type (deflation):               normal
+  compression sub-type (deflation):               maximum
   file security status:                           not encrypted
   extended local header:                          no
-  file last modified on (DOS date/time):          2024 Mar 21 19:57:36
-  32-bit CRC value (hex):                         9bebdec1
-  compressed size:                                657 bytes
-  uncompressed size:                              2501 bytes
-  length of filename:                             47 characters
-  length of extra field:                          0 bytes
+  file last modified on (DOS date/time):          2024 Apr 16 01:12:14
+  file last modified on (UT extra field modtime): 2024 Apr 16 08:12:14 local
+  file last modified on (UT extra field modtime): 2024 Apr 16 08:12:14 UTC
+  32-bit CRC value (hex):                         f1241bb0
+  compressed size:                                475 bytes
+  uncompressed size:                              956 bytes
+  length of filename:                             27 characters
+  length of extra field:                          24 bytes
   length of file comment:                         0 characters
   disk number on which file begins:               disk 1
-  apparent file type:                             binary
-  Unix file attributes (100664 octal):            -rw-rw-r--
+  apparent file type:                             text
+  Unix file attributes (100644 octal):            -rw-r--r--
   MS-DOS file attributes (00 hex):                none
 
+  The central-directory extra field contains:
+  - A subfield with ID 0x5455 (universal time) and 5 data bytes.
+    The local extra field has UTC/GMT modification/access times.
+  - A subfield with ID 0x7875 (Unix UID/GID (any size)) and 11 data bytes:
+    01 04 e3 3d 03 00 04 64 00 00 00.
+
   There is no file comment.
 
 Central directory entry #50:
 ---------------------------
 
-  tests/torchtune/utils/test_metric_logging.py
+  torchtune/config/_instantiate.py
 
-  offset of local header from start of archive:   50110
-                                                  (000000000000C3BEh) bytes
+  offset of local header from start of archive:   68876
+                                                  (0000000000010D0Ch) bytes
   file system or operating system of origin:      Unix
-  version of encoding software:                   2.0
+  version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
-  compression sub-type (deflation):               normal
+  compression sub-type (deflation):               maximum
   file security status:                           not encrypted
   extended local header:                          no
-  file last modified on (DOS date/time):          2024 Mar 21 19:57:36
-  32-bit CRC value (hex):                         0d268cd6
-  compressed size:                                1124 bytes
-  uncompressed size:                              5433 bytes
-  length of filename:                             44 characters
-  length of extra field:                          0 bytes
+  file last modified on (DOS date/time):          2024 Apr 16 01:12:14
+  file last modified on (UT extra field modtime): 2024 Apr 16 08:12:14 local
+  file last modified on (UT extra field modtime): 2024 Apr 16 08:12:14 UTC
+  32-bit CRC value (hex):                         0911f93f
+  compressed size:                                1475 bytes
+  uncompressed size:                              3873 bytes
+  length of filename:                             32 characters
+  length of extra field:                          24 bytes
   length of file comment:                         0 characters
   disk number on which file begins:               disk 1
-  apparent file type:                             binary
-  Unix file attributes (100664 octal):            -rw-rw-r--
+  apparent file type:                             text
+  Unix file attributes (100644 octal):            -rw-r--r--
   MS-DOS file attributes (00 hex):                none
 
+  The central-directory extra field contains:
+  - A subfield with ID 0x5455 (universal time) and 5 data bytes.
+    The local extra field has UTC/GMT modification/access times.
+  - A subfield with ID 0x7875 (Unix UID/GID (any size)) and 11 data bytes:
+    01 04 e3 3d 03 00 04 64 00 00 00.
+
   There is no file comment.
 
 Central directory entry #51:
 ---------------------------
 
-  tests/torchtune/utils/test_precision.py
+  torchtune/config/_parse.py
 
-  offset of local header from start of archive:   51308
-                                                  (000000000000C86Ch) bytes
+  offset of local header from start of archive:   70441
+                                                  (0000000000011329h) bytes
   file system or operating system of origin:      Unix
-  version of encoding software:                   2.0
+  version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
-  compression sub-type (deflation):               normal
+  compression sub-type (deflation):               maximum
   file security status:                           not encrypted
   extended local header:                          no
-  file last modified on (DOS date/time):          2024 Mar 21 19:57:36
-  32-bit CRC value (hex):                         c9d1ea0d
-  compressed size:                                1085 bytes
-  uncompressed size:                              3459 bytes
-  length of filename:                             39 characters
-  length of extra field:                          0 bytes
+  file last modified on (DOS date/time):          2024 Apr 16 01:12:14
+  file last modified on (UT extra field modtime): 2024 Apr 16 08:12:14 local
+  file last modified on (UT extra field modtime): 2024 Apr 16 08:12:14 UTC
+  32-bit CRC value (hex):                         4d72f190
+  compressed size:                                733 bytes
+  uncompressed size:                              1598 bytes
+  length of filename:                             26 characters
+  length of extra field:                          24 bytes
   length of file comment:                         0 characters
   disk number on which file begins:               disk 1
-  apparent file type:                             binary
-  Unix file attributes (100664 octal):            -rw-rw-r--
+  apparent file type:                             text
+  Unix file attributes (100644 octal):            -rw-r--r--
   MS-DOS file attributes (00 hex):                none
 
+  The central-directory extra field contains:
+  - A subfield with ID 0x5455 (universal time) and 5 data bytes.
+    The local extra field has UTC/GMT modification/access times.
+  - A subfield with ID 0x7875 (Unix UID/GID (any size)) and 11 data bytes:
+    01 04 e3 3d 03 00 04 64 00 00 00.
+
   There is no file comment.
 
 Central directory entry #52:
 ---------------------------
 
-  tests/torchtune/utils/test_seed.py
+  torchtune/config/_utils.py
 
-  offset of local header from start of archive:   52462
-                                                  (000000000000CCEEh) bytes
+  offset of local header from start of archive:   71258
+                                                  (000000000001165Ah) bytes
   file system or operating system of origin:      Unix
-  version of encoding software:                   2.0
+  version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
-  compression sub-type (deflation):               normal
+  compression sub-type (deflation):               maximum
   file security status:                           not encrypted
   extended local header:                          no
-  file last modified on (DOS date/time):          2024 Mar 21 19:57:36
-  32-bit CRC value (hex):                         f7b43f36
-  compressed size:                                786 bytes
-  uncompressed size:                              2892 bytes
-  length of filename:                             34 characters
-  length of extra field:                          0 bytes
+  file last modified on (DOS date/time):          2024 Apr 16 01:12:14
+  file last modified on (UT extra field modtime): 2024 Apr 16 08:12:14 local
+  file last modified on (UT extra field modtime): 2024 Apr 16 08:12:14 UTC
+  32-bit CRC value (hex):                         a0c5a13d
+  compressed size:                                2688 bytes
+  uncompressed size:                              8006 bytes
+  length of filename:                             26 characters
+  length of extra field:                          24 bytes
   length of file comment:                         0 characters
   disk number on which file begins:               disk 1
-  apparent file type:                             binary
-  Unix file attributes (100664 octal):            -rw-rw-r--
+  apparent file type:                             text
+  Unix file attributes (100644 octal):            -rw-r--r--
   MS-DOS file attributes (00 hex):                none
 
+  The central-directory extra field contains:
+  - A subfield with ID 0x5455 (universal time) and 5 data bytes.
+    The local extra field has UTC/GMT modification/access times.
+  - A subfield with ID 0x7875 (Unix UID/GID (any size)) and 11 data bytes:
+    01 04 e3 3d 03 00 04 64 00 00 00.
+
   There is no file comment.
 
 Central directory entry #53:
 ---------------------------
 
-  tests/torchtune/utils/test_tensor_utils.py
+  torchtune/config/_validate.py
 
-  offset of local header from start of archive:   53312
-                                                  (000000000000D040h) bytes
+  offset of local header from start of archive:   74030
+                                                  (000000000001212Eh) bytes
   file system or operating system of origin:      Unix
-  version of encoding software:                   2.0
+  version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
-  compression sub-type (deflation):               normal
+  compression sub-type (deflation):               maximum
   file security status:                           not encrypted
   extended local header:                          no
-  file last modified on (DOS date/time):          2024 Mar 21 19:57:36
-  32-bit CRC value (hex):                         5ec3b837
-  compressed size:                                333 bytes
-  uncompressed size:                              697 bytes
-  length of filename:                             42 characters
-  length of extra field:                          0 bytes
+  file last modified on (DOS date/time):          2024 Apr 16 01:12:14
+  file last modified on (UT extra field modtime): 2024 Apr 16 08:12:14 local
+  file last modified on (UT extra field modtime): 2024 Apr 16 08:12:14 UTC
+  32-bit CRC value (hex):                         80c827b9
+  compressed size:                                714 bytes
+  uncompressed size:                              1636 bytes
+  length of filename:                             29 characters
+  length of extra field:                          24 bytes
   length of file comment:                         0 characters
   disk number on which file begins:               disk 1
-  apparent file type:                             binary
-  Unix file attributes (100664 octal):            -rw-rw-r--
+  apparent file type:                             text
+  Unix file attributes (100644 octal):            -rw-r--r--
   MS-DOS file attributes (00 hex):                none
 
+  The central-directory extra field contains:
+  - A subfield with ID 0x5455 (universal time) and 5 data bytes.
+    The local extra field has UTC/GMT modification/access times.
+  - A subfield with ID 0x7875 (Unix UID/GID (any size)) and 11 data bytes:
+    01 04 e3 3d 03 00 04 64 00 00 00.
+
   There is no file comment.
 
 Central directory entry #54:
 ---------------------------
 
-  torchtune/__init__.py
+  torchtune/data/
 
-  offset of local header from start of archive:   53717
-                                                  (000000000000D1D5h) bytes
+  offset of local header from start of archive:   74831
+                                                  (000000000001244Fh) bytes
   file system or operating system of origin:      Unix
-  version of encoding software:                   2.0
+  version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
-  minimum software version required to extract:   2.0
-  compression method:                             deflated
-  compression sub-type (deflation):               normal
+  minimum software version required to extract:   1.0
+  compression method:                             none (stored)
   file security status:                           not encrypted
   extended local header:                          no
-  file last modified on (DOS date/time):          2024 Mar 21 19:57:36
-  32-bit CRC value (hex):                         2ef0d75f
-  compressed size:                                470 bytes
-  uncompressed size:                              1188 bytes
-  length of filename:                             21 characters
-  length of extra field:                          0 bytes
+  file last modified on (DOS date/time):          2024 Apr 15 20:08:26
+  file last modified on (UT extra field modtime): 2024 Apr 16 03:08:26 local
+  file last modified on (UT extra field modtime): 2024 Apr 16 03:08:26 UTC
+  32-bit CRC value (hex):                         00000000
+  compressed size:                                0 bytes
+  uncompressed size:                              0 bytes
+  length of filename:                             15 characters
+  length of extra field:                          24 bytes
   length of file comment:                         0 characters
   disk number on which file begins:               disk 1
   apparent file type:                             binary
-  Unix file attributes (100664 octal):            -rw-rw-r--
-  MS-DOS file attributes (00 hex):                none
+  Unix file attributes (040755 octal):            drwxr-xr-x
+  MS-DOS file attributes (10 hex):                dir 
+
+  The central-directory extra field contains:
+  - A subfield with ID 0x5455 (universal time) and 5 data bytes.
+    The local extra field has UTC/GMT modification/access times.
+  - A subfield with ID 0x7875 (Unix UID/GID (any size)) and 11 data bytes:
+    01 04 e3 3d 03 00 04 64 00 00 00.
 
   There is no file comment.
 
 Central directory entry #55:
 ---------------------------
 
-  torchtune/recipe_interfaces.py
+  torchtune/data/__init__.py
 
-  offset of local header from start of archive:   54238
-                                                  (000000000000D3DEh) bytes
+  offset of local header from start of archive:   74904
+                                                  (0000000000012498h) bytes
   file system or operating system of origin:      Unix
-  version of encoding software:                   2.0
+  version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
-  compression sub-type (deflation):               normal
+  compression sub-type (deflation):               maximum
   file security status:                           not encrypted
   extended local header:                          no
-  file last modified on (DOS date/time):          2024 Mar 21 19:57:36
-  32-bit CRC value (hex):                         5ad6d4db
-  compressed size:                                873 bytes
-  uncompressed size:                              2201 bytes
-  length of filename:                             30 characters
-  length of extra field:                          0 bytes
+  file last modified on (DOS date/time):          2024 Apr 16 01:12:14
+  file last modified on (UT extra field modtime): 2024 Apr 16 08:12:14 local
+  file last modified on (UT extra field modtime): 2024 Apr 16 08:12:14 UTC
+  32-bit CRC value (hex):                         fc2322bc
+  compressed size:                                440 bytes
+  uncompressed size:                              1136 bytes
+  length of filename:                             26 characters
+  length of extra field:                          24 bytes
   length of file comment:                         0 characters
   disk number on which file begins:               disk 1
-  apparent file type:                             binary
-  Unix file attributes (100664 octal):            -rw-rw-r--
+  apparent file type:                             text
+  Unix file attributes (100644 octal):            -rw-r--r--
   MS-DOS file attributes (00 hex):                none
 
+  The central-directory extra field contains:
+  - A subfield with ID 0x5455 (universal time) and 5 data bytes.
+    The local extra field has UTC/GMT modification/access times.
+  - A subfield with ID 0x7875 (Unix UID/GID (any size)) and 11 data bytes:
+    01 04 e3 3d 03 00 04 64 00 00 00.
+
   There is no file comment.
 
 Central directory entry #56:
 ---------------------------
 
-  torchtune/_cli/__init__.py
+  torchtune/data/_chat_formats.py
 
-  offset of local header from start of archive:   55171
-                                                  (000000000000D783h) bytes
+  offset of local header from start of archive:   75428
+                                                  (00000000000126A4h) bytes
   file system or operating system of origin:      Unix
-  version of encoding software:                   2.0
+  version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
-  compression sub-type (deflation):               normal
+  compression sub-type (deflation):               maximum
   file security status:                           not encrypted
   extended local header:                          no
-  file last modified on (DOS date/time):          2024 Mar 21 19:57:36
-  32-bit CRC value (hex):                         b295742d
-  compressed size:                                251 bytes
-  uncompressed size:                              366 bytes
-  length of filename:                             26 characters
-  length of extra field:                          0 bytes
+  file last modified on (DOS date/time):          2024 Apr 16 01:12:14
+  file last modified on (UT extra field modtime): 2024 Apr 16 08:12:14 local
+  file last modified on (UT extra field modtime): 2024 Apr 16 08:12:14 UTC
+  32-bit CRC value (hex):                         f74b7e42
+  compressed size:                                1760 bytes
+  uncompressed size:                              7107 bytes
+  length of filename:                             31 characters
+  length of extra field:                          24 bytes
   length of file comment:                         0 characters
   disk number on which file begins:               disk 1
-  apparent file type:                             binary
-  Unix file attributes (100664 octal):            -rw-rw-r--
+  apparent file type:                             text
+  Unix file attributes (100644 octal):            -rw-r--r--
   MS-DOS file attributes (00 hex):                none
 
+  The central-directory extra field contains:
+  - A subfield with ID 0x5455 (universal time) and 5 data bytes.
+    The local extra field has UTC/GMT modification/access times.
+  - A subfield with ID 0x7875 (Unix UID/GID (any size)) and 11 data bytes:
+    01 04 e3 3d 03 00 04 64 00 00 00.
+
   There is no file comment.
 
 Central directory entry #57:
 ---------------------------
 
-  torchtune/_cli/convert_checkpoint.py
+  torchtune/data/_common.py
 
-  offset of local header from start of archive:   55478
-                                                  (000000000000D8B6h) bytes
+  offset of local header from start of archive:   77277
+                                                  (0000000000012DDDh) bytes
   file system or operating system of origin:      Unix
-  version of encoding software:                   2.0
+  version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
-  compression sub-type (deflation):               normal
+  compression sub-type (deflation):               maximum
   file security status:                           not encrypted
   extended local header:                          no
-  file last modified on (DOS date/time):          2024 Mar 21 19:57:36
-  32-bit CRC value (hex):                         8de1856e
-  compressed size:                                1509 bytes
-  uncompressed size:                              4098 bytes
-  length of filename:                             36 characters
-  length of extra field:                          0 bytes
+  file last modified on (DOS date/time):          2024 Apr 16 01:12:14
+  file last modified on (UT extra field modtime): 2024 Apr 16 08:12:14 local
+  file last modified on (UT extra field modtime): 2024 Apr 16 08:12:14 UTC
+  32-bit CRC value (hex):                         ac21b77c
+  compressed size:                                186 bytes
+  uncompressed size:                              241 bytes
+  length of filename:                             25 characters
+  length of extra field:                          24 bytes
   length of file comment:                         0 characters
   disk number on which file begins:               disk 1
-  apparent file type:                             binary
-  Unix file attributes (100664 octal):            -rw-rw-r--
+  apparent file type:                             text
+  Unix file attributes (100644 octal):            -rw-r--r--
   MS-DOS file attributes (00 hex):                none
 
+  The central-directory extra field contains:
+  - A subfield with ID 0x5455 (universal time) and 5 data bytes.
+    The local extra field has UTC/GMT modification/access times.
+  - A subfield with ID 0x7875 (Unix UID/GID (any size)) and 11 data bytes:
+    01 04 e3 3d 03 00 04 64 00 00 00.
+
   There is no file comment.
 
 Central directory entry #58:
 ---------------------------
 
-  torchtune/_cli/cp.py
+  torchtune/data/_converters.py
 
-  offset of local header from start of archive:   57053
-                                                  (000000000000DEDDh) bytes
+  offset of local header from start of archive:   77546
+                                                  (0000000000012EEAh) bytes
   file system or operating system of origin:      Unix
-  version of encoding software:                   2.0
+  version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
-  compression sub-type (deflation):               normal
+  compression sub-type (deflation):               maximum
   file security status:                           not encrypted
   extended local header:                          no
-  file last modified on (DOS date/time):          2024 Mar 21 19:57:36
-  32-bit CRC value (hex):                         8dfee71f
-  compressed size:                                1352 bytes
-  uncompressed size:                              3518 bytes
-  length of filename:                             20 characters
-  length of extra field:                          0 bytes
+  file last modified on (DOS date/time):          2024 Apr 16 01:12:14
+  file last modified on (UT extra field modtime): 2024 Apr 16 08:12:14 local
+  file last modified on (UT extra field modtime): 2024 Apr 16 08:12:14 UTC
+  32-bit CRC value (hex):                         daa8943c
+  compressed size:                                748 bytes
+  uncompressed size:                              1746 bytes
+  length of filename:                             29 characters
+  length of extra field:                          24 bytes
   length of file comment:                         0 characters
   disk number on which file begins:               disk 1
-  apparent file type:                             binary
-  Unix file attributes (100664 octal):            -rw-rw-r--
+  apparent file type:                             text
+  Unix file attributes (100644 octal):            -rw-r--r--
   MS-DOS file attributes (00 hex):                none
 
+  The central-directory extra field contains:
+  - A subfield with ID 0x5455 (universal time) and 5 data bytes.
+    The local extra field has UTC/GMT modification/access times.
+  - A subfield with ID 0x7875 (Unix UID/GID (any size)) and 11 data bytes:
+    01 04 e3 3d 03 00 04 64 00 00 00.
+
   There is no file comment.
 
 Central directory entry #59:
 ---------------------------
 
-  torchtune/_cli/download.py
+  torchtune/data/_instruct_templates.py
 
-  offset of local header from start of archive:   58455
-                                                  (000000000000E457h) bytes
+  offset of local header from start of archive:   78381
+                                                  (000000000001322Dh) bytes
   file system or operating system of origin:      Unix
-  version of encoding software:                   2.0
+  version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
-  compression sub-type (deflation):               normal
+  compression sub-type (deflation):               maximum
   file security status:                           not encrypted
   extended local header:                          no
-  file last modified on (DOS date/time):          2024 Mar 21 19:57:36
-  32-bit CRC value (hex):                         bf123284
-  compressed size:                                867 bytes
-  uncompressed size:                              2140 bytes
-  length of filename:                             26 characters
-  length of extra field:                          0 bytes
+  file last modified on (DOS date/time):          2024 Apr 16 01:12:14
+  file last modified on (UT extra field modtime): 2024 Apr 16 08:12:14 local
+  file last modified on (UT extra field modtime): 2024 Apr 16 08:12:14 UTC
+  32-bit CRC value (hex):                         ee6cdbb5
+  compressed size:                                1272 bytes
+  uncompressed size:                              5989 bytes
+  length of filename:                             37 characters
+  length of extra field:                          24 bytes
   length of file comment:                         0 characters
   disk number on which file begins:               disk 1
-  apparent file type:                             binary
-  Unix file attributes (100664 octal):            -rw-rw-r--
+  apparent file type:                             text
+  Unix file attributes (100644 octal):            -rw-r--r--
   MS-DOS file attributes (00 hex):                none
 
+  The central-directory extra field contains:
+  - A subfield with ID 0x5455 (universal time) and 5 data bytes.
+    The local extra field has UTC/GMT modification/access times.
+  - A subfield with ID 0x7875 (Unix UID/GID (any size)) and 11 data bytes:
+    01 04 e3 3d 03 00 04 64 00 00 00.
+
   There is no file comment.
 
 Central directory entry #60:
 ---------------------------
 
-  torchtune/_cli/eval.py
+  torchtune/data/_types.py
 
-  offset of local header from start of archive:   59378
-                                                  (000000000000E7F2h) bytes
+  offset of local header from start of archive:   79748
+                                                  (0000000000013784h) bytes
   file system or operating system of origin:      Unix
-  version of encoding software:                   2.0
+  version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
-  compression sub-type (deflation):               normal
+  compression sub-type (deflation):               maximum
   file security status:                           not encrypted
   extended local header:                          no
-  file last modified on (DOS date/time):          2024 Mar 21 19:57:36
-  32-bit CRC value (hex):                         53299fe2
-  compressed size:                                2625 bytes
-  uncompressed size:                              7202 bytes
-  length of filename:                             22 characters
-  length of extra field:                          0 bytes
+  file last modified on (DOS date/time):          2024 Apr 16 01:12:14
+  file last modified on (UT extra field modtime): 2024 Apr 16 08:12:14 local
+  file last modified on (UT extra field modtime): 2024 Apr 16 08:12:14 UTC
+  32-bit CRC value (hex):                         1e3a8812
+  compressed size:                                258 bytes
+  uncompressed size:                              402 bytes
+  length of filename:                             24 characters
+  length of extra field:                          24 bytes
   length of file comment:                         0 characters
   disk number on which file begins:               disk 1
-  apparent file type:                             binary
-  Unix file attributes (100664 octal):            -rw-rw-r--
+  apparent file type:                             text
+  Unix file attributes (100644 octal):            -rw-r--r--
   MS-DOS file attributes (00 hex):                none
 
+  The central-directory extra field contains:
+  - A subfield with ID 0x5455 (universal time) and 5 data bytes.
+    The local extra field has UTC/GMT modification/access times.
+  - A subfield with ID 0x7875 (Unix UID/GID (any size)) and 11 data bytes:
+    01 04 e3 3d 03 00 04 64 00 00 00.
+
   There is no file comment.
 
 Central directory entry #61:
 ---------------------------
 
-  torchtune/_cli/ls.py
+  torchtune/data/_utils.py
 
-  offset of local header from start of archive:   62055
-                                                  (000000000000F267h) bytes
+  offset of local header from start of archive:   80088
+                                                  (00000000000138D8h) bytes
   file system or operating system of origin:      Unix
-  version of encoding software:                   2.0
+  version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
-  compression sub-type (deflation):               normal
+  compression sub-type (deflation):               maximum
   file security status:                           not encrypted
   extended local header:                          no
-  file last modified on (DOS date/time):          2024 Mar 21 19:57:36
-  32-bit CRC value (hex):                         ebf6696b
-  compressed size:                                741 bytes
-  uncompressed size:                              1784 bytes
-  length of filename:                             20 characters
-  length of extra field:                          0 bytes
+  file last modified on (DOS date/time):          2024 Apr 16 01:12:14
+  file last modified on (UT extra field modtime): 2024 Apr 16 08:12:14 local
+  file last modified on (UT extra field modtime): 2024 Apr 16 08:12:14 UTC
+  32-bit CRC value (hex):                         b13d8e7d
+  compressed size:                                929 bytes
+  uncompressed size:                              2401 bytes
+  length of filename:                             24 characters
+  length of extra field:                          24 bytes
   length of file comment:                         0 characters
   disk number on which file begins:               disk 1
-  apparent file type:                             binary
-  Unix file attributes (100664 octal):            -rw-rw-r--
+  apparent file type:                             text
+  Unix file attributes (100644 octal):            -rw-r--r--
   MS-DOS file attributes (00 hex):                none
 
+  The central-directory extra field contains:
+  - A subfield with ID 0x5455 (universal time) and 5 data bytes.
+    The local extra field has UTC/GMT modification/access times.
+  - A subfield with ID 0x7875 (Unix UID/GID (any size)) and 11 data bytes:
+    01 04 e3 3d 03 00 04 64 00 00 00.
+
   There is no file comment.
 
 Central directory entry #62:
 ---------------------------
 
-  torchtune/_cli/tune.py
+  torchtune/datasets/
 
-  offset of local header from start of archive:   62846
-                                                  (000000000000F57Eh) bytes
+  offset of local header from start of archive:   81099
+                                                  (0000000000013CCBh) bytes
   file system or operating system of origin:      Unix
-  version of encoding software:                   2.0
+  version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
-  minimum software version required to extract:   2.0
-  compression method:                             deflated
-  compression sub-type (deflation):               normal
+  minimum software version required to extract:   1.0
+  compression method:                             none (stored)
   file security status:                           not encrypted
   extended local header:                          no
-  file last modified on (DOS date/time):          2024 Mar 21 19:57:36
-  32-bit CRC value (hex):                         c87635d7
-  compressed size:                                1890 bytes
-  uncompressed size:                              5292 bytes
-  length of filename:                             22 characters
-  length of extra field:                          0 bytes
+  file last modified on (DOS date/time):          2024 Apr 15 20:08:26
+  file last modified on (UT extra field modtime): 2024 Apr 16 03:08:26 local
+  file last modified on (UT extra field modtime): 2024 Apr 16 03:08:26 UTC
+  32-bit CRC value (hex):                         00000000
+  compressed size:                                0 bytes
+  uncompressed size:                              0 bytes
+  length of filename:                             19 characters
+  length of extra field:                          24 bytes
   length of file comment:                         0 characters
   disk number on which file begins:               disk 1
   apparent file type:                             binary
-  Unix file attributes (100664 octal):            -rw-rw-r--
-  MS-DOS file attributes (00 hex):                none
+  Unix file attributes (040755 octal):            drwxr-xr-x
+  MS-DOS file attributes (10 hex):                dir 
+
+  The central-directory extra field contains:
+  - A subfield with ID 0x5455 (universal time) and 5 data bytes.
+    The local extra field has UTC/GMT modification/access times.
+  - A subfield with ID 0x7875 (Unix UID/GID (any size)) and 11 data bytes:
+    01 04 e3 3d 03 00 04 64 00 00 00.
 
   There is no file comment.
 
 Central directory entry #63:
 ---------------------------
 
-  torchtune/_cli/validate.py
+  torchtune/datasets/__init__.py
 
-  offset of local header from start of archive:   64788
-                                                  (000000000000FD14h) bytes
+  offset of local header from start of archive:   81176
+                                                  (0000000000013D18h) bytes
   file system or operating system of origin:      Unix
-  version of encoding software:                   2.0
+  version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
-  compression sub-type (deflation):               normal
+  compression sub-type (deflation):               maximum
   file security status:                           not encrypted
   extended local header:                          no
-  file last modified on (DOS date/time):          2024 Mar 21 19:57:36
-  32-bit CRC value (hex):                         a4aaa94d
-  compressed size:                                557 bytes
-  uncompressed size:                              1145 bytes
-  length of filename:                             26 characters
-  length of extra field:                          0 bytes
+  file last modified on (DOS date/time):          2024 Apr 16 01:12:14
+  file last modified on (UT extra field modtime): 2024 Apr 16 08:12:14 local
+  file last modified on (UT extra field modtime): 2024 Apr 16 08:12:14 UTC
+  32-bit CRC value (hex):                         531ebbe6
+  compressed size:                                336 bytes
+  uncompressed size:                              939 bytes
+  length of filename:                             30 characters
+  length of extra field:                          24 bytes
   length of file comment:                         0 characters
   disk number on which file begins:               disk 1
-  apparent file type:                             binary
-  Unix file attributes (100664 octal):            -rw-rw-r--
+  apparent file type:                             text
+  Unix file attributes (100644 octal):            -rw-r--r--
   MS-DOS file attributes (00 hex):                none
 
+  The central-directory extra field contains:
+  - A subfield with ID 0x5455 (universal time) and 5 data bytes.
+    The local extra field has UTC/GMT modification/access times.
+  - A subfield with ID 0x7875 (Unix UID/GID (any size)) and 11 data bytes:
+    01 04 e3 3d 03 00 04 64 00 00 00.
+
   There is no file comment.
 
 Central directory entry #64:
 ---------------------------
 
-  torchtune/config/__init__.py
+  torchtune/datasets/_alpaca.py
 
-  offset of local header from start of archive:   65401
-                                                  (000000000000FF79h) bytes
+  offset of local header from start of archive:   81600
+                                                  (0000000000013EC0h) bytes
   file system or operating system of origin:      Unix
-  version of encoding software:                   2.0
+  version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
-  compression sub-type (deflation):               normal
+  compression sub-type (deflation):               maximum
   file security status:                           not encrypted
   extended local header:                          no
-  file last modified on (DOS date/time):          2024 Mar 21 19:57:36
-  32-bit CRC value (hex):                         acd45f83
-  compressed size:                                216 bytes
-  uncompressed size:                              368 bytes
-  length of filename:                             28 characters
-  length of extra field:                          0 bytes
+  file last modified on (DOS date/time):          2024 Apr 16 01:12:14
+  file last modified on (UT extra field modtime): 2024 Apr 16 08:12:14 local
+  file last modified on (UT extra field modtime): 2024 Apr 16 08:12:14 UTC
+  32-bit CRC value (hex):                         10a8a9e8
+  compressed size:                                1134 bytes
+  uncompressed size:                              2582 bytes
+  length of filename:                             29 characters
+  length of extra field:                          24 bytes
   length of file comment:                         0 characters
   disk number on which file begins:               disk 1
-  apparent file type:                             binary
-  Unix file attributes (100664 octal):            -rw-rw-r--
+  apparent file type:                             text
+  Unix file attributes (100644 octal):            -rw-r--r--
   MS-DOS file attributes (00 hex):                none
 
+  The central-directory extra field contains:
+  - A subfield with ID 0x5455 (universal time) and 5 data bytes.
+    The local extra field has UTC/GMT modification/access times.
+  - A subfield with ID 0x7875 (Unix UID/GID (any size)) and 11 data bytes:
+    01 04 e3 3d 03 00 04 64 00 00 00.
+
   There is no file comment.
 
 Central directory entry #65:
 ---------------------------
 
-  torchtune/config/_errors.py
+  torchtune/datasets/_chat.py
 
-  offset of local header from start of archive:   65675
-                                                  (000000000001008Bh) bytes
+  offset of local header from start of archive:   82821
+                                                  (0000000000014385h) bytes
   file system or operating system of origin:      Unix
-  version of encoding software:                   2.0
+  version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
-  compression sub-type (deflation):               normal
+  compression sub-type (deflation):               maximum
   file security status:                           not encrypted
   extended local header:                          no
-  file last modified on (DOS date/time):          2024 Mar 21 19:57:36
-  32-bit CRC value (hex):                         f1241bb0
-  compressed size:                                475 bytes
-  uncompressed size:                              956 bytes
+  file last modified on (DOS date/time):          2024 Apr 16 01:12:14
+  file last modified on (UT extra field modtime): 2024 Apr 16 08:12:14 local
+  file last modified on (UT extra field modtime): 2024 Apr 16 08:12:14 UTC
+  32-bit CRC value (hex):                         72880111
+  compressed size:                                1914 bytes
+  uncompressed size:                              5940 bytes
   length of filename:                             27 characters
-  length of extra field:                          0 bytes
+  length of extra field:                          24 bytes
   length of file comment:                         0 characters
   disk number on which file begins:               disk 1
-  apparent file type:                             binary
-  Unix file attributes (100664 octal):            -rw-rw-r--
+  apparent file type:                             text
+  Unix file attributes (100644 octal):            -rw-r--r--
   MS-DOS file attributes (00 hex):                none
 
+  The central-directory extra field contains:
+  - A subfield with ID 0x5455 (universal time) and 5 data bytes.
+    The local extra field has UTC/GMT modification/access times.
+  - A subfield with ID 0x7875 (Unix UID/GID (any size)) and 11 data bytes:
+    01 04 e3 3d 03 00 04 64 00 00 00.
+
   There is no file comment.
 
 Central directory entry #66:
 ---------------------------
 
-  torchtune/config/_instantiate.py
+  torchtune/datasets/_grammar.py
 
-  offset of local header from start of archive:   66207
-                                                  (000000000001029Fh) bytes
+  offset of local header from start of archive:   84820
+                                                  (0000000000014B54h) bytes
   file system or operating system of origin:      Unix
-  version of encoding software:                   2.0
+  version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
-  compression sub-type (deflation):               normal
+  compression sub-type (deflation):               maximum
   file security status:                           not encrypted
   extended local header:                          no
-  file last modified on (DOS date/time):          2024 Mar 21 19:57:36
-  32-bit CRC value (hex):                         e40736b1
-  compressed size:                                1478 bytes
-  uncompressed size:                              3873 bytes
-  length of filename:                             32 characters
-  length of extra field:                          0 bytes
+  file last modified on (DOS date/time):          2024 Apr 16 01:12:14
+  file last modified on (UT extra field modtime): 2024 Apr 16 08:12:14 local
+  file last modified on (UT extra field modtime): 2024 Apr 16 08:12:14 UTC
+  32-bit CRC value (hex):                         5e351c01
+  compressed size:                                953 bytes
+  uncompressed size:                              2180 bytes
+  length of filename:                             30 characters
+  length of extra field:                          24 bytes
   length of file comment:                         0 characters
   disk number on which file begins:               disk 1
-  apparent file type:                             binary
-  Unix file attributes (100664 octal):            -rw-rw-r--
+  apparent file type:                             text
+  Unix file attributes (100644 octal):            -rw-r--r--
   MS-DOS file attributes (00 hex):                none
 
+  The central-directory extra field contains:
+  - A subfield with ID 0x5455 (universal time) and 5 data bytes.
+    The local extra field has UTC/GMT modification/access times.
+  - A subfield with ID 0x7875 (Unix UID/GID (any size)) and 11 data bytes:
+    01 04 e3 3d 03 00 04 64 00 00 00.
+
   There is no file comment.
 
 Central directory entry #67:
 ---------------------------
 
-  torchtune/config/_parse.py
+  torchtune/datasets/_instruct.py
 
-  offset of local header from start of archive:   67747
-                                                  (00000000000108A3h) bytes
+  offset of local header from start of archive:   85861
+                                                  (0000000000014F65h) bytes
   file system or operating system of origin:      Unix
-  version of encoding software:                   2.0
+  version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
-  compression sub-type (deflation):               normal
+  compression sub-type (deflation):               maximum
   file security status:                           not encrypted
   extended local header:                          no
-  file last modified on (DOS date/time):          2024 Mar 21 19:57:36
-  32-bit CRC value (hex):                         bfcafdd6
-  compressed size:                                809 bytes
-  uncompressed size:                              1766 bytes
-  length of filename:                             26 characters
-  length of extra field:                          0 bytes
+  file last modified on (DOS date/time):          2024 Apr 16 01:12:14
+  file last modified on (UT extra field modtime): 2024 Apr 16 08:12:14 local
+  file last modified on (UT extra field modtime): 2024 Apr 16 08:12:14 UTC
+  32-bit CRC value (hex):                         05aab416
+  compressed size:                                1994 bytes
+  uncompressed size:                              6793 bytes
+  length of filename:                             31 characters
+  length of extra field:                          24 bytes
   length of file comment:                         0 characters
   disk number on which file begins:               disk 1
-  apparent file type:                             binary
-  Unix file attributes (100664 octal):            -rw-rw-r--
+  apparent file type:                             text
+  Unix file attributes (100644 octal):            -rw-r--r--
   MS-DOS file attributes (00 hex):                none
 
+  The central-directory extra field contains:
+  - A subfield with ID 0x5455 (universal time) and 5 data bytes.
+    The local extra field has UTC/GMT modification/access times.
+  - A subfield with ID 0x7875 (Unix UID/GID (any size)) and 11 data bytes:
+    01 04 e3 3d 03 00 04 64 00 00 00.
+
   There is no file comment.
 
 Central directory entry #68:
 ---------------------------
 
-  torchtune/config/_utils.py
+  torchtune/datasets/_preference.py
 
-  offset of local header from start of archive:   68612
-                                                  (0000000000010C04h) bytes
+  offset of local header from start of archive:   87944
+                                                  (0000000000015788h) bytes
   file system or operating system of origin:      Unix
-  version of encoding software:                   2.0
+  version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
-  compression sub-type (deflation):               normal
+  compression sub-type (deflation):               maximum
   file security status:                           not encrypted
   extended local header:                          no
-  file last modified on (DOS date/time):          2024 Mar 21 19:57:36
-  32-bit CRC value (hex):                         e18ead3f
-  compressed size:                                2037 bytes
-  uncompressed size:                              5819 bytes
-  length of filename:                             26 characters
-  length of extra field:                          0 bytes
+  file last modified on (DOS date/time):          2024 Apr 16 01:12:14
+  file last modified on (UT extra field modtime): 2024 Apr 16 08:12:14 local
+  file last modified on (UT extra field modtime): 2024 Apr 16 08:12:14 UTC
+  32-bit CRC value (hex):                         cf33831d
+  compressed size:                                1711 bytes
+  uncompressed size:                              5038 bytes
+  length of filename:                             33 characters
+  length of extra field:                          24 bytes
   length of file comment:                         0 characters
   disk number on which file begins:               disk 1
-  apparent file type:                             binary
-  Unix file attributes (100664 octal):            -rw-rw-r--
+  apparent file type:                             text
+  Unix file attributes (100644 octal):            -rw-r--r--
   MS-DOS file attributes (00 hex):                none
 
+  The central-directory extra field contains:
+  - A subfield with ID 0x5455 (universal time) and 5 data bytes.
+    The local extra field has UTC/GMT modification/access times.
+  - A subfield with ID 0x7875 (Unix UID/GID (any size)) and 11 data bytes:
+    01 04 e3 3d 03 00 04 64 00 00 00.
+
   There is no file comment.
 
 Central directory entry #69:
 ---------------------------
 
-  torchtune/config/_validate.py
+  torchtune/datasets/_samsum.py
 
-  offset of local header from start of archive:   70705
-                                                  (0000000000011431h) bytes
+  offset of local header from start of archive:   89746
+                                                  (0000000000015E92h) bytes
   file system or operating system of origin:      Unix
-  version of encoding software:                   2.0
+  version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
-  compression sub-type (deflation):               normal
+  compression sub-type (deflation):               maximum
   file security status:                           not encrypted
   extended local header:                          no
-  file last modified on (DOS date/time):          2024 Mar 21 19:57:36
-  32-bit CRC value (hex):                         80c827b9
-  compressed size:                                716 bytes
-  uncompressed size:                              1636 bytes
+  file last modified on (DOS date/time):          2024 Apr 16 01:12:14
+  file last modified on (UT extra field modtime): 2024 Apr 16 08:12:14 local
+  file last modified on (UT extra field modtime): 2024 Apr 16 08:12:14 UTC
+  32-bit CRC value (hex):                         7470b202
+  compressed size:                                937 bytes
+  uncompressed size:                              2086 bytes
   length of filename:                             29 characters
-  length of extra field:                          0 bytes
+  length of extra field:                          24 bytes
   length of file comment:                         0 characters
   disk number on which file begins:               disk 1
-  apparent file type:                             binary
-  Unix file attributes (100664 octal):            -rw-rw-r--
+  apparent file type:                             text
+  Unix file attributes (100644 octal):            -rw-r--r--
   MS-DOS file attributes (00 hex):                none
 
+  The central-directory extra field contains:
+  - A subfield with ID 0x5455 (universal time) and 5 data bytes.
+    The local extra field has UTC/GMT modification/access times.
+  - A subfield with ID 0x7875 (Unix UID/GID (any size)) and 11 data bytes:
+    01 04 e3 3d 03 00 04 64 00 00 00.
+
   There is no file comment.
 
 Central directory entry #70:
 ---------------------------
 
-  torchtune/data/__init__.py
+  torchtune/datasets/_slimorca.py
 
-  offset of local header from start of archive:   71480
-                                                  (0000000000011738h) bytes
+  offset of local header from start of archive:   90770
+                                                  (0000000000016292h) bytes
   file system or operating system of origin:      Unix
-  version of encoding software:                   2.0
+  version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
-  compression sub-type (deflation):               normal
+  compression sub-type (deflation):               maximum
   file security status:                           not encrypted
   extended local header:                          no
-  file last modified on (DOS date/time):          2024 Mar 21 19:57:36
-  32-bit CRC value (hex):                         8aae125b
-  compressed size:                                262 bytes
-  uncompressed size:                              488 bytes
-  length of filename:                             26 characters
-  length of extra field:                          0 bytes
+  file last modified on (DOS date/time):          2024 Apr 16 01:12:14
+  file last modified on (UT extra field modtime): 2024 Apr 16 08:12:14 local
+  file last modified on (UT extra field modtime): 2024 Apr 16 08:12:14 UTC
+  32-bit CRC value (hex):                         2c14800a
+  compressed size:                                1165 bytes
+  uncompressed size:                              2687 bytes
+  length of filename:                             31 characters
+  length of extra field:                          24 bytes
   length of file comment:                         0 characters
   disk number on which file begins:               disk 1
-  apparent file type:                             binary
-  Unix file attributes (100664 octal):            -rw-rw-r--
+  apparent file type:                             text
+  Unix file attributes (100644 octal):            -rw-r--r--
   MS-DOS file attributes (00 hex):                none
 
+  The central-directory extra field contains:
+  - A subfield with ID 0x5455 (universal time) and 5 data bytes.
+    The local extra field has UTC/GMT modification/access times.
+  - A subfield with ID 0x7875 (Unix UID/GID (any size)) and 11 data bytes:
+    01 04 e3 3d 03 00 04 64 00 00 00.
+
   There is no file comment.
 
 Central directory entry #71:
 ---------------------------
 
-  torchtune/data/_templates.py
+  torchtune/datasets/_stack_exchanged_paired.py
 
-  offset of local header from start of archive:   71798
-                                                  (0000000000011876h) bytes
+  offset of local header from start of archive:   92024
+                                                  (0000000000016778h) bytes
   file system or operating system of origin:      Unix
-  version of encoding software:                   2.0
+  version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
-  compression sub-type (deflation):               normal
+  compression sub-type (deflation):               maximum
   file security status:                           not encrypted
   extended local header:                          no
-  file last modified on (DOS date/time):          2024 Mar 21 19:57:36
-  32-bit CRC value (hex):                         77735895
-  compressed size:                                1139 bytes
-  uncompressed size:                              5011 bytes
-  length of filename:                             28 characters
-  length of extra field:                          0 bytes
+  file last modified on (DOS date/time):          2024 Apr 16 01:12:14
+  file last modified on (UT extra field modtime): 2024 Apr 16 08:12:14 local
+  file last modified on (UT extra field modtime): 2024 Apr 16 08:12:14 UTC
+  32-bit CRC value (hex):                         a84f40d8
+  compressed size:                                659 bytes
+  uncompressed size:                              1449 bytes
+  length of filename:                             45 characters
+  length of extra field:                          24 bytes
   length of file comment:                         0 characters
   disk number on which file begins:               disk 1
-  apparent file type:                             binary
-  Unix file attributes (100664 octal):            -rw-rw-r--
+  apparent file type:                             text
+  Unix file attributes (100644 octal):            -rw-r--r--
   MS-DOS file attributes (00 hex):                none
 
+  The central-directory extra field contains:
+  - A subfield with ID 0x5455 (universal time) and 5 data bytes.
+    The local extra field has UTC/GMT modification/access times.
+  - A subfield with ID 0x7875 (Unix UID/GID (any size)) and 11 data bytes:
+    01 04 e3 3d 03 00 04 64 00 00 00.
+
   There is no file comment.
 
 Central directory entry #72:
 ---------------------------
 
-  torchtune/datasets/__init__.py
+  torchtune/models/
 
-  offset of local header from start of archive:   72995
-                                                  (0000000000011D23h) bytes
+  offset of local header from start of archive:   92786
+                                                  (0000000000016A72h) bytes
   file system or operating system of origin:      Unix
-  version of encoding software:                   2.0
+  version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
-  minimum software version required to extract:   2.0
-  compression method:                             deflated
-  compression sub-type (deflation):               normal
+  minimum software version required to extract:   1.0
+  compression method:                             none (stored)
   file security status:                           not encrypted
   extended local header:                          no
-  file last modified on (DOS date/time):          2024 Mar 21 19:57:36
-  32-bit CRC value (hex):                         8f70beb9
-  compressed size:                                240 bytes
-  uncompressed size:                              460 bytes
-  length of filename:                             30 characters
-  length of extra field:                          0 bytes
+  file last modified on (DOS date/time):          2024 Apr 15 20:08:26
+  file last modified on (UT extra field modtime): 2024 Apr 16 03:08:26 local
+  file last modified on (UT extra field modtime): 2024 Apr 16 03:08:26 UTC
+  32-bit CRC value (hex):                         00000000
+  compressed size:                                0 bytes
+  uncompressed size:                              0 bytes
+  length of filename:                             17 characters
+  length of extra field:                          24 bytes
   length of file comment:                         0 characters
   disk number on which file begins:               disk 1
   apparent file type:                             binary
-  Unix file attributes (100664 octal):            -rw-rw-r--
-  MS-DOS file attributes (00 hex):                none
+  Unix file attributes (040755 octal):            drwxr-xr-x
+  MS-DOS file attributes (10 hex):                dir 
+
+  The central-directory extra field contains:
+  - A subfield with ID 0x5455 (universal time) and 5 data bytes.
+    The local extra field has UTC/GMT modification/access times.
+  - A subfield with ID 0x7875 (Unix UID/GID (any size)) and 11 data bytes:
+    01 04 e3 3d 03 00 04 64 00 00 00.
 
   There is no file comment.
 
 Central directory entry #73:
 ---------------------------
 
-  torchtune/datasets/_alpaca.py
+  torchtune/models/__init__.py
 
-  offset of local header from start of archive:   73295
-                                                  (0000000000011E4Fh) bytes
+  offset of local header from start of archive:   92861
+                                                  (0000000000016ABDh) bytes
   file system or operating system of origin:      Unix
-  version of encoding software:                   2.0
+  version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
-  compression sub-type (deflation):               normal
+  compression sub-type (deflation):               maximum
   file security status:                           not encrypted
   extended local header:                          no
-  file last modified on (DOS date/time):          2024 Mar 21 19:57:36
-  32-bit CRC value (hex):                         4c46fa2f
-  compressed size:                                1040 bytes
-  uncompressed size:                              2563 bytes
-  length of filename:                             29 characters
-  length of extra field:                          0 bytes
+  file last modified on (DOS date/time):          2024 Apr 16 01:12:14
+  file last modified on (UT extra field modtime): 2024 Apr 16 08:12:14 local
+  file last modified on (UT extra field modtime): 2024 Apr 16 08:12:14 UTC
+  32-bit CRC value (hex):                         e3929a97
+  compressed size:                                202 bytes
+  uncompressed size:                              286 bytes
+  length of filename:                             28 characters
+  length of extra field:                          24 bytes
   length of file comment:                         0 characters
   disk number on which file begins:               disk 1
-  apparent file type:                             binary
-  Unix file attributes (100664 octal):            -rw-rw-r--
+  apparent file type:                             text
+  Unix file attributes (100644 octal):            -rw-r--r--
   MS-DOS file attributes (00 hex):                none
 
+  The central-directory extra field contains:
+  - A subfield with ID 0x5455 (universal time) and 5 data bytes.
+    The local extra field has UTC/GMT modification/access times.
+  - A subfield with ID 0x7875 (Unix UID/GID (any size)) and 11 data bytes:
+    01 04 e3 3d 03 00 04 64 00 00 00.
+
   There is no file comment.
 
 Central directory entry #74:
 ---------------------------
 
-  torchtune/datasets/_common.py
+  torchtune/models/convert_weights.py
 
-  offset of local header from start of archive:   74394
-                                                  (000000000001229Ah) bytes
+  offset of local header from start of archive:   93149
+                                                  (0000000000016BDDh) bytes
   file system or operating system of origin:      Unix
-  version of encoding software:                   2.0
+  version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
-  compression sub-type (deflation):               normal
+  compression sub-type (deflation):               maximum
   file security status:                           not encrypted
   extended local header:                          no
-  file last modified on (DOS date/time):          2024 Mar 21 19:57:36
-  32-bit CRC value (hex):                         ac21b77c
-  compressed size:                                186 bytes
-  uncompressed size:                              241 bytes
-  length of filename:                             29 characters
-  length of extra field:                          0 bytes
+  file last modified on (DOS date/time):          2024 Apr 16 01:12:14
+  file last modified on (UT extra field modtime): 2024 Apr 16 08:12:14 local
+  file last modified on (UT extra field modtime): 2024 Apr 16 08:12:14 UTC
+  32-bit CRC value (hex):                         48c5044b
+  compressed size:                                1650 bytes
+  uncompressed size:                              7447 bytes
+  length of filename:                             35 characters
+  length of extra field:                          24 bytes
   length of file comment:                         0 characters
   disk number on which file begins:               disk 1
-  apparent file type:                             binary
-  Unix file attributes (100664 octal):            -rw-rw-r--
+  apparent file type:                             text
+  Unix file attributes (100644 octal):            -rw-r--r--
   MS-DOS file attributes (00 hex):                none
 
+  The central-directory extra field contains:
+  - A subfield with ID 0x5455 (universal time) and 5 data bytes.
+    The local extra field has UTC/GMT modification/access times.
+  - A subfield with ID 0x7875 (Unix UID/GID (any size)) and 11 data bytes:
+    01 04 e3 3d 03 00 04 64 00 00 00.
+
   There is no file comment.
 
 Central directory entry #75:
 ---------------------------
 
-  torchtune/datasets/_instruct.py
+  torchtune/models/gemma/
 
-  offset of local header from start of archive:   74639
-                                                  (000000000001238Fh) bytes
+  offset of local header from start of archive:   94892
+                                                  (00000000000172ACh) bytes
   file system or operating system of origin:      Unix
-  version of encoding software:                   2.0
+  version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
-  minimum software version required to extract:   2.0
-  compression method:                             deflated
-  compression sub-type (deflation):               normal
+  minimum software version required to extract:   1.0
+  compression method:                             none (stored)
   file security status:                           not encrypted
   extended local header:                          no
-  file last modified on (DOS date/time):          2024 Mar 21 19:57:36
-  32-bit CRC value (hex):                         867487ef
-  compressed size:                                2111 bytes
-  uncompressed size:                              7153 bytes
-  length of filename:                             31 characters
-  length of extra field:                          0 bytes
+  file last modified on (DOS date/time):          2024 Apr 15 20:08:26
+  file last modified on (UT extra field modtime): 2024 Apr 16 03:08:26 local
+  file last modified on (UT extra field modtime): 2024 Apr 16 03:08:26 UTC
+  32-bit CRC value (hex):                         00000000
+  compressed size:                                0 bytes
+  uncompressed size:                              0 bytes
+  length of filename:                             23 characters
+  length of extra field:                          24 bytes
   length of file comment:                         0 characters
   disk number on which file begins:               disk 1
   apparent file type:                             binary
-  Unix file attributes (100664 octal):            -rw-rw-r--
-  MS-DOS file attributes (00 hex):                none
+  Unix file attributes (040755 octal):            drwxr-xr-x
+  MS-DOS file attributes (10 hex):                dir 
+
+  The central-directory extra field contains:
+  - A subfield with ID 0x5455 (universal time) and 5 data bytes.
+    The local extra field has UTC/GMT modification/access times.
+  - A subfield with ID 0x7875 (Unix UID/GID (any size)) and 11 data bytes:
+    01 04 e3 3d 03 00 04 64 00 00 00.
 
   There is no file comment.
 
 Central directory entry #76:
 ---------------------------
 
-  torchtune/datasets/_slimorca.py
+  torchtune/models/gemma/__init__.py
 
-  offset of local header from start of archive:   76811
-                                                  (0000000000012C0Bh) bytes
+  offset of local header from start of archive:   94973
+                                                  (00000000000172FDh) bytes
   file system or operating system of origin:      Unix
-  version of encoding software:                   2.0
+  version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
-  compression sub-type (deflation):               normal
+  compression sub-type (deflation):               maximum
   file security status:                           not encrypted
   extended local header:                          no
-  file last modified on (DOS date/time):          2024 Mar 21 19:57:36
-  32-bit CRC value (hex):                         82aa01dd
-  compressed size:                                2074 bytes
-  uncompressed size:                              5742 bytes
-  length of filename:                             31 characters
-  length of extra field:                          0 bytes
+  file last modified on (DOS date/time):          2024 Apr 16 01:12:14
+  file last modified on (UT extra field modtime): 2024 Apr 16 08:12:14 local
+  file last modified on (UT extra field modtime): 2024 Apr 16 08:12:14 UTC
+  32-bit CRC value (hex):                         c1a21352
+  compressed size:                                208 bytes
+  uncompressed size:                              319 bytes
+  length of filename:                             34 characters
+  length of extra field:                          24 bytes
   length of file comment:                         0 characters
   disk number on which file begins:               disk 1
-  apparent file type:                             binary
-  Unix file attributes (100664 octal):            -rw-rw-r--
+  apparent file type:                             text
+  Unix file attributes (100644 octal):            -rw-r--r--
   MS-DOS file attributes (00 hex):                none
 
+  The central-directory extra field contains:
+  - A subfield with ID 0x5455 (universal time) and 5 data bytes.
+    The local extra field has UTC/GMT modification/access times.
+  - A subfield with ID 0x7875 (Unix UID/GID (any size)) and 11 data bytes:
+    01 04 e3 3d 03 00 04 64 00 00 00.
+
   There is no file comment.
 
 Central directory entry #77:
 ---------------------------
 
-  torchtune/models/__init__.py
+  torchtune/models/gemma/_component_builders.py
 
-  offset of local header from start of archive:   78946
-                                                  (0000000000013462h) bytes
+  offset of local header from start of archive:   95273
+                                                  (0000000000017429h) bytes
   file system or operating system of origin:      Unix
-  version of encoding software:                   2.0
+  version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
-  compression sub-type (deflation):               normal
+  compression sub-type (deflation):               maximum
   file security status:                           not encrypted
   extended local header:                          no
-  file last modified on (DOS date/time):          2024 Mar 21 19:57:36
-  32-bit CRC value (hex):                         0e4efc81
-  compressed size:                                181 bytes
-  uncompressed size:                              253 bytes
-  length of filename:                             28 characters
-  length of extra field:                          0 bytes
+  file last modified on (DOS date/time):          2024 Apr 16 01:12:14
+  file last modified on (UT extra field modtime): 2024 Apr 16 08:12:14 local
+  file last modified on (UT extra field modtime): 2024 Apr 16 08:12:14 UTC
+  32-bit CRC value (hex):                         253195fd
+  compressed size:                                1598 bytes
+  uncompressed size:                              4617 bytes
+  length of filename:                             45 characters
+  length of extra field:                          24 bytes
   length of file comment:                         0 characters
   disk number on which file begins:               disk 1
-  apparent file type:                             binary
-  Unix file attributes (100664 octal):            -rw-rw-r--
+  apparent file type:                             text
+  Unix file attributes (100644 octal):            -rw-r--r--
   MS-DOS file attributes (00 hex):                none
 
+  The central-directory extra field contains:
+  - A subfield with ID 0x5455 (universal time) and 5 data bytes.
+    The local extra field has UTC/GMT modification/access times.
+  - A subfield with ID 0x7875 (Unix UID/GID (any size)) and 11 data bytes:
+    01 04 e3 3d 03 00 04 64 00 00 00.
+
   There is no file comment.
 
 Central directory entry #78:
 ---------------------------
 
-  torchtune/models/llama2/__init__.py
+  torchtune/models/gemma/_model_builders.py
 
-  offset of local header from start of archive:   79185
-                                                  (0000000000013551h) bytes
+  offset of local header from start of archive:   96974
+                                                  (0000000000017ACEh) bytes
   file system or operating system of origin:      Unix
-  version of encoding software:                   2.0
+  version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
-  compression sub-type (deflation):               normal
+  compression sub-type (deflation):               maximum
   file security status:                           not encrypted
   extended local header:                          no
-  file last modified on (DOS date/time):          2024 Mar 21 19:57:36
-  32-bit CRC value (hex):                         0e44cb34
-  compressed size:                                350 bytes
-  uncompressed size:                              771 bytes
-  length of filename:                             35 characters
-  length of extra field:                          0 bytes
+  file last modified on (DOS date/time):          2024 Apr 16 01:12:14
+  file last modified on (UT extra field modtime): 2024 Apr 16 08:12:14 local
+  file last modified on (UT extra field modtime): 2024 Apr 16 08:12:14 UTC
+  32-bit CRC value (hex):                         227bc1e0
+  compressed size:                                594 bytes
+  uncompressed size:                              1189 bytes
+  length of filename:                             41 characters
+  length of extra field:                          24 bytes
   length of file comment:                         0 characters
   disk number on which file begins:               disk 1
-  apparent file type:                             binary
-  Unix file attributes (100664 octal):            -rw-rw-r--
+  apparent file type:                             text
+  Unix file attributes (100644 octal):            -rw-r--r--
   MS-DOS file attributes (00 hex):                none
 
+  The central-directory extra field contains:
+  - A subfield with ID 0x5455 (universal time) and 5 data bytes.
+    The local extra field has UTC/GMT modification/access times.
+  - A subfield with ID 0x7875 (Unix UID/GID (any size)) and 11 data bytes:
+    01 04 e3 3d 03 00 04 64 00 00 00.
+
   There is no file comment.
 
 Central directory entry #79:
 ---------------------------
 
-  torchtune/models/llama2/_checkpoint_utils.py
+  torchtune/models/gemma/rms_norm.py
 
-  offset of local header from start of archive:   79600
-                                                  (00000000000136F0h) bytes
+  offset of local header from start of archive:   97667
+                                                  (0000000000017D83h) bytes
   file system or operating system of origin:      Unix
-  version of encoding software:                   2.0
+  version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
-  compression sub-type (deflation):               normal
+  compression sub-type (deflation):               maximum
   file security status:                           not encrypted
   extended local header:                          no
-  file last modified on (DOS date/time):          2024 Mar 21 19:57:36
-  32-bit CRC value (hex):                         3306215d
-  compressed size:                                2053 bytes
-  uncompressed size:                              6391 bytes
-  length of filename:                             44 characters
-  length of extra field:                          0 bytes
+  file last modified on (DOS date/time):          2024 Apr 16 01:12:14
+  file last modified on (UT extra field modtime): 2024 Apr 16 08:12:14 local
+  file last modified on (UT extra field modtime): 2024 Apr 16 08:12:14 UTC
+  32-bit CRC value (hex):                         74df2234
+  compressed size:                                505 bytes
+  uncompressed size:                              910 bytes
+  length of filename:                             34 characters
+  length of extra field:                          24 bytes
   length of file comment:                         0 characters
   disk number on which file begins:               disk 1
-  apparent file type:                             binary
-  Unix file attributes (100664 octal):            -rw-rw-r--
+  apparent file type:                             text
+  Unix file attributes (100644 octal):            -rw-r--r--
   MS-DOS file attributes (00 hex):                none
 
+  The central-directory extra field contains:
+  - A subfield with ID 0x5455 (universal time) and 5 data bytes.
+    The local extra field has UTC/GMT modification/access times.
+  - A subfield with ID 0x7875 (Unix UID/GID (any size)) and 11 data bytes:
+    01 04 e3 3d 03 00 04 64 00 00 00.
+
   There is no file comment.
 
 Central directory entry #80:
 ---------------------------
 
-  torchtune/models/llama2/_component_builders.py
+  torchtune/models/gemma/transformer.py
 
-  offset of local header from start of archive:   81727
-                                                  (0000000000013F3Fh) bytes
+  offset of local header from start of archive:   98264
+                                                  (0000000000017FD8h) bytes
   file system or operating system of origin:      Unix
-  version of encoding software:                   2.0
+  version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
-  compression sub-type (deflation):               normal
+  compression sub-type (deflation):               maximum
   file security status:                           not encrypted
   extended local header:                          no
-  file last modified on (DOS date/time):          2024 Mar 21 19:57:36
-  32-bit CRC value (hex):                         7620b8da
-  compressed size:                                2725 bytes
-  uncompressed size:                              14979 bytes
-  length of filename:                             46 characters
-  length of extra field:                          0 bytes
+  file last modified on (DOS date/time):          2024 Apr 16 01:12:14
+  file last modified on (UT extra field modtime): 2024 Apr 16 08:12:14 local
+  file last modified on (UT extra field modtime): 2024 Apr 16 08:12:14 UTC
+  32-bit CRC value (hex):                         90c6c474
+  compressed size:                                1782 bytes
+  uncompressed size:                              5077 bytes
+  length of filename:                             37 characters
+  length of extra field:                          24 bytes
   length of file comment:                         0 characters
   disk number on which file begins:               disk 1
-  apparent file type:                             binary
-  Unix file attributes (100664 octal):            -rw-rw-r--
+  apparent file type:                             text
+  Unix file attributes (100644 octal):            -rw-r--r--
   MS-DOS file attributes (00 hex):                none
 
+  The central-directory extra field contains:
+  - A subfield with ID 0x5455 (universal time) and 5 data bytes.
+    The local extra field has UTC/GMT modification/access times.
+  - A subfield with ID 0x7875 (Unix UID/GID (any size)) and 11 data bytes:
+    01 04 e3 3d 03 00 04 64 00 00 00.
+
   There is no file comment.
 
 Central directory entry #81:
 ---------------------------
 
-  torchtune/models/llama2/_convert_weights.py
+  torchtune/models/llama2/
+
+  offset of local header from start of archive:   100141
+                                                  (000000000001872Dh) bytes
+  file system or operating system of origin:      Unix
+  version of encoding software:                   3.0
+  minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
+  minimum software version required to extract:   1.0
+  compression method:                             none (stored)
+  file security status:                           not encrypted
+  extended local header:                          no
+  file last modified on (DOS date/time):          2024 Apr 15 20:08:26
+  file last modified on (UT extra field modtime): 2024 Apr 16 03:08:26 local
+  file last modified on (UT extra field modtime): 2024 Apr 16 03:08:26 UTC
+  32-bit CRC value (hex):                         00000000
+  compressed size:                                0 bytes
+  uncompressed size:                              0 bytes
+  length of filename:                             24 characters
+  length of extra field:                          24 bytes
+  length of file comment:                         0 characters
+  disk number on which file begins:               disk 1
+  apparent file type:                             binary
+  Unix file attributes (040755 octal):            drwxr-xr-x
+  MS-DOS file attributes (10 hex):                dir 
+
+  The central-directory extra field contains:
+  - A subfield with ID 0x5455 (universal time) and 5 data bytes.
+    The local extra field has UTC/GMT modification/access times.
+  - A subfield with ID 0x7875 (Unix UID/GID (any size)) and 11 data bytes:
+    01 04 e3 3d 03 00 04 64 00 00 00.
+
+  There is no file comment.
+
+Central directory entry #82:
+---------------------------
+
+  torchtune/models/llama2/__init__.py
 
-  offset of local header from start of archive:   84528
-                                                  (0000000000014A30h) bytes
+  offset of local header from start of archive:   100223
+                                                  (000000000001877Fh) bytes
   file system or operating system of origin:      Unix
-  version of encoding software:                   2.0
+  version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
-  compression sub-type (deflation):               normal
+  compression sub-type (deflation):               maximum
   file security status:                           not encrypted
   extended local header:                          no
-  file last modified on (DOS date/time):          2024 Mar 21 19:57:36
-  32-bit CRC value (hex):                         d9fc41cc
-  compressed size:                                1264 bytes
-  uncompressed size:                              5375 bytes
-  length of filename:                             43 characters
-  length of extra field:                          0 bytes
+  file last modified on (DOS date/time):          2024 Apr 16 01:12:14
+  file last modified on (UT extra field modtime): 2024 Apr 16 08:12:14 local
+  file last modified on (UT extra field modtime): 2024 Apr 16 08:12:14 UTC
+  32-bit CRC value (hex):                         c451bc74
+  compressed size:                                338 bytes
+  uncompressed size:                              774 bytes
+  length of filename:                             35 characters
+  length of extra field:                          24 bytes
   length of file comment:                         0 characters
   disk number on which file begins:               disk 1
-  apparent file type:                             binary
-  Unix file attributes (100664 octal):            -rw-rw-r--
+  apparent file type:                             text
+  Unix file attributes (100644 octal):            -rw-r--r--
   MS-DOS file attributes (00 hex):                none
 
+  The central-directory extra field contains:
+  - A subfield with ID 0x5455 (universal time) and 5 data bytes.
+    The local extra field has UTC/GMT modification/access times.
+  - A subfield with ID 0x7875 (Unix UID/GID (any size)) and 11 data bytes:
+    01 04 e3 3d 03 00 04 64 00 00 00.
+
   There is no file comment.
 
-Central directory entry #82:
+Central directory entry #83:
+---------------------------
+
+  torchtune/models/llama2/_checkpoint_utils.py
+
+  offset of local header from start of archive:   100654
+                                                  (000000000001892Eh) bytes
+  file system or operating system of origin:      Unix
+  version of encoding software:                   3.0
+  minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
+  minimum software version required to extract:   2.0
+  compression method:                             deflated
+  compression sub-type (deflation):               maximum
+  file security status:                           not encrypted
+  extended local header:                          no
+  file last modified on (DOS date/time):          2024 Apr 16 01:12:14
+  file last modified on (UT extra field modtime): 2024 Apr 16 08:12:14 local
+  file last modified on (UT extra field modtime): 2024 Apr 16 08:12:14 UTC
+  32-bit CRC value (hex):                         3306215d
+  compressed size:                                2047 bytes
+  uncompressed size:                              6391 bytes
+  length of filename:                             44 characters
+  length of extra field:                          24 bytes
+  length of file comment:                         0 characters
+  disk number on which file begins:               disk 1
+  apparent file type:                             text
+  Unix file attributes (100644 octal):            -rw-r--r--
+  MS-DOS file attributes (00 hex):                none
+
+  The central-directory extra field contains:
+  - A subfield with ID 0x5455 (universal time) and 5 data bytes.
+    The local extra field has UTC/GMT modification/access times.
+  - A subfield with ID 0x7875 (Unix UID/GID (any size)) and 11 data bytes:
+    01 04 e3 3d 03 00 04 64 00 00 00.
+
+  There is no file comment.
+
+Central directory entry #84:
+---------------------------
+
+  torchtune/models/llama2/_component_builders.py
+
+  offset of local header from start of archive:   102803
+                                                  (0000000000019193h) bytes
+  file system or operating system of origin:      Unix
+  version of encoding software:                   3.0
+  minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
+  minimum software version required to extract:   2.0
+  compression method:                             deflated
+  compression sub-type (deflation):               maximum
+  file security status:                           not encrypted
+  extended local header:                          no
+  file last modified on (DOS date/time):          2024 Apr 16 01:12:14
+  file last modified on (UT extra field modtime): 2024 Apr 16 08:12:14 local
+  file last modified on (UT extra field modtime): 2024 Apr 16 08:12:14 UTC
+  32-bit CRC value (hex):                         46be5388
+  compressed size:                                2991 bytes
+  uncompressed size:                              14695 bytes
+  length of filename:                             46 characters
+  length of extra field:                          24 bytes
+  length of file comment:                         0 characters
+  disk number on which file begins:               disk 1
+  apparent file type:                             text
+  Unix file attributes (100644 octal):            -rw-r--r--
+  MS-DOS file attributes (00 hex):                none
+
+  The central-directory extra field contains:
+  - A subfield with ID 0x5455 (universal time) and 5 data bytes.
+    The local extra field has UTC/GMT modification/access times.
+  - A subfield with ID 0x7875 (Unix UID/GID (any size)) and 11 data bytes:
+    01 04 e3 3d 03 00 04 64 00 00 00.
+
+  There is no file comment.
+
+Central directory entry #85:
 ---------------------------
 
   torchtune/models/llama2/_model_builders.py
 
-  offset of local header from start of archive:   85865
-                                                  (0000000000014F69h) bytes
+  offset of local header from start of archive:   105898
+                                                  (0000000000019DAAh) bytes
   file system or operating system of origin:      Unix
-  version of encoding software:                   2.0
+  version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
-  compression sub-type (deflation):               normal
+  compression sub-type (deflation):               maximum
   file security status:                           not encrypted
   extended local header:                          no
-  file last modified on (DOS date/time):          2024 Mar 21 19:57:36
-  32-bit CRC value (hex):                         c43b18fb
-  compressed size:                                1276 bytes
-  uncompressed size:                              3487 bytes
+  file last modified on (DOS date/time):          2024 Apr 16 01:12:14
+  file last modified on (UT extra field modtime): 2024 Apr 16 08:12:14 local
+  file last modified on (UT extra field modtime): 2024 Apr 16 08:12:14 UTC
+  32-bit CRC value (hex):                         5f08b629
+  compressed size:                                1446 bytes
+  uncompressed size:                              6020 bytes
   length of filename:                             42 characters
-  length of extra field:                          0 bytes
+  length of extra field:                          24 bytes
   length of file comment:                         0 characters
   disk number on which file begins:               disk 1
-  apparent file type:                             binary
-  Unix file attributes (100664 octal):            -rw-rw-r--
+  apparent file type:                             text
+  Unix file attributes (100644 octal):            -rw-r--r--
   MS-DOS file attributes (00 hex):                none
 
+  The central-directory extra field contains:
+  - A subfield with ID 0x5455 (universal time) and 5 data bytes.
+    The local extra field has UTC/GMT modification/access times.
+  - A subfield with ID 0x7875 (Unix UID/GID (any size)) and 11 data bytes:
+    01 04 e3 3d 03 00 04 64 00 00 00.
+
   There is no file comment.
 
-Central directory entry #83:
+Central directory entry #86:
 ---------------------------
 
   torchtune/models/llama2/_model_utils.py
 
-  offset of local header from start of archive:   87213
-                                                  (00000000000154ADh) bytes
+  offset of local header from start of archive:   107444
+                                                  (000000000001A3B4h) bytes
   file system or operating system of origin:      Unix
-  version of encoding software:                   2.0
+  version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
-  compression sub-type (deflation):               normal
+  compression sub-type (deflation):               maximum
   file security status:                           not encrypted
   extended local header:                          no
-  file last modified on (DOS date/time):          2024 Mar 21 19:57:36
+  file last modified on (DOS date/time):          2024 Apr 16 01:12:14
+  file last modified on (UT extra field modtime): 2024 Apr 16 08:12:14 local
+  file last modified on (UT extra field modtime): 2024 Apr 16 08:12:14 UTC
   32-bit CRC value (hex):                         146ffb72
   compressed size:                                424 bytes
   uncompressed size:                              902 bytes
   length of filename:                             39 characters
-  length of extra field:                          0 bytes
+  length of extra field:                          24 bytes
+  length of file comment:                         0 characters
+  disk number on which file begins:               disk 1
+  apparent file type:                             text
+  Unix file attributes (100644 octal):            -rw-r--r--
+  MS-DOS file attributes (00 hex):                none
+
+  The central-directory extra field contains:
+  - A subfield with ID 0x5455 (universal time) and 5 data bytes.
+    The local extra field has UTC/GMT modification/access times.
+  - A subfield with ID 0x7875 (Unix UID/GID (any size)) and 11 data bytes:
+    01 04 e3 3d 03 00 04 64 00 00 00.
+
+  There is no file comment.
+
+Central directory entry #87:
+---------------------------
+
+  torchtune/models/mistral/
+
+  offset of local header from start of archive:   107965
+                                                  (000000000001A5BDh) bytes
+  file system or operating system of origin:      Unix
+  version of encoding software:                   3.0
+  minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
+  minimum software version required to extract:   1.0
+  compression method:                             none (stored)
+  file security status:                           not encrypted
+  extended local header:                          no
+  file last modified on (DOS date/time):          2024 Apr 15 20:08:26
+  file last modified on (UT extra field modtime): 2024 Apr 16 03:08:26 local
+  file last modified on (UT extra field modtime): 2024 Apr 16 03:08:26 UTC
+  32-bit CRC value (hex):                         00000000
+  compressed size:                                0 bytes
+  uncompressed size:                              0 bytes
+  length of filename:                             25 characters
+  length of extra field:                          24 bytes
   length of file comment:                         0 characters
   disk number on which file begins:               disk 1
   apparent file type:                             binary
-  Unix file attributes (100664 octal):            -rw-rw-r--
+  Unix file attributes (040755 octal):            drwxr-xr-x
+  MS-DOS file attributes (10 hex):                dir 
+
+  The central-directory extra field contains:
+  - A subfield with ID 0x5455 (universal time) and 5 data bytes.
+    The local extra field has UTC/GMT modification/access times.
+  - A subfield with ID 0x7875 (Unix UID/GID (any size)) and 11 data bytes:
+    01 04 e3 3d 03 00 04 64 00 00 00.
+
+  There is no file comment.
+
+Central directory entry #88:
+---------------------------
+
+  torchtune/models/mistral/__init__.py
+
+  offset of local header from start of archive:   108048
+                                                  (000000000001A610h) bytes
+  file system or operating system of origin:      Unix
+  version of encoding software:                   3.0
+  minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
+  minimum software version required to extract:   2.0
+  compression method:                             deflated
+  compression sub-type (deflation):               maximum
+  file security status:                           not encrypted
+  extended local header:                          no
+  file last modified on (DOS date/time):          2024 Apr 16 01:12:14
+  file last modified on (UT extra field modtime): 2024 Apr 16 08:12:14 local
+  file last modified on (UT extra field modtime): 2024 Apr 16 08:12:14 UTC
+  32-bit CRC value (hex):                         e18f0a27
+  compressed size:                                257 bytes
+  uncompressed size:                              519 bytes
+  length of filename:                             36 characters
+  length of extra field:                          24 bytes
+  length of file comment:                         0 characters
+  disk number on which file begins:               disk 1
+  apparent file type:                             text
+  Unix file attributes (100644 octal):            -rw-r--r--
   MS-DOS file attributes (00 hex):                none
 
+  The central-directory extra field contains:
+  - A subfield with ID 0x5455 (universal time) and 5 data bytes.
+    The local extra field has UTC/GMT modification/access times.
+  - A subfield with ID 0x7875 (Unix UID/GID (any size)) and 11 data bytes:
+    01 04 e3 3d 03 00 04 64 00 00 00.
+
   There is no file comment.
 
-Central directory entry #84:
+Central directory entry #89:
+---------------------------
+
+  torchtune/models/mistral/_component_builders.py
+
+  offset of local header from start of archive:   108399
+                                                  (000000000001A76Fh) bytes
+  file system or operating system of origin:      Unix
+  version of encoding software:                   3.0
+  minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
+  minimum software version required to extract:   2.0
+  compression method:                             deflated
+  compression sub-type (deflation):               maximum
+  file security status:                           not encrypted
+  extended local header:                          no
+  file last modified on (DOS date/time):          2024 Apr 16 01:12:14
+  file last modified on (UT extra field modtime): 2024 Apr 16 08:12:14 local
+  file last modified on (UT extra field modtime): 2024 Apr 16 08:12:14 UTC
+  32-bit CRC value (hex):                         6ee5aa49
+  compressed size:                                2986 bytes
+  uncompressed size:                              14328 bytes
+  length of filename:                             47 characters
+  length of extra field:                          24 bytes
+  length of file comment:                         0 characters
+  disk number on which file begins:               disk 1
+  apparent file type:                             text
+  Unix file attributes (100644 octal):            -rw-r--r--
+  MS-DOS file attributes (00 hex):                none
+
+  The central-directory extra field contains:
+  - A subfield with ID 0x5455 (universal time) and 5 data bytes.
+    The local extra field has UTC/GMT modification/access times.
+  - A subfield with ID 0x7875 (Unix UID/GID (any size)) and 11 data bytes:
+    01 04 e3 3d 03 00 04 64 00 00 00.
+
+  There is no file comment.
+
+Central directory entry #90:
+---------------------------
+
+  torchtune/models/mistral/_model_builders.py
+
+  offset of local header from start of archive:   111490
+                                                  (000000000001B382h) bytes
+  file system or operating system of origin:      Unix
+  version of encoding software:                   3.0
+  minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
+  minimum software version required to extract:   2.0
+  compression method:                             deflated
+  compression sub-type (deflation):               maximum
+  file security status:                           not encrypted
+  extended local header:                          no
+  file last modified on (DOS date/time):          2024 Apr 16 01:12:14
+  file last modified on (UT extra field modtime): 2024 Apr 16 08:12:14 local
+  file last modified on (UT extra field modtime): 2024 Apr 16 08:12:14 UTC
+  32-bit CRC value (hex):                         ca1e120f
+  compressed size:                                1230 bytes
+  uncompressed size:                              3391 bytes
+  length of filename:                             43 characters
+  length of extra field:                          24 bytes
+  length of file comment:                         0 characters
+  disk number on which file begins:               disk 1
+  apparent file type:                             text
+  Unix file attributes (100644 octal):            -rw-r--r--
+  MS-DOS file attributes (00 hex):                none
+
+  The central-directory extra field contains:
+  - A subfield with ID 0x5455 (universal time) and 5 data bytes.
+    The local extra field has UTC/GMT modification/access times.
+  - A subfield with ID 0x7875 (Unix UID/GID (any size)) and 11 data bytes:
+    01 04 e3 3d 03 00 04 64 00 00 00.
+
+  There is no file comment.
+
+Central directory entry #91:
+---------------------------
+
+  torchtune/modules/
+
+  offset of local header from start of archive:   112821
+                                                  (000000000001B8B5h) bytes
+  file system or operating system of origin:      Unix
+  version of encoding software:                   3.0
+  minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
+  minimum software version required to extract:   1.0
+  compression method:                             none (stored)
+  file security status:                           not encrypted
+  extended local header:                          no
+  file last modified on (DOS date/time):          2024 Apr 15 20:08:26
+  file last modified on (UT extra field modtime): 2024 Apr 16 03:08:26 local
+  file last modified on (UT extra field modtime): 2024 Apr 16 03:08:26 UTC
+  32-bit CRC value (hex):                         00000000
+  compressed size:                                0 bytes
+  uncompressed size:                              0 bytes
+  length of filename:                             18 characters
+  length of extra field:                          24 bytes
+  length of file comment:                         0 characters
+  disk number on which file begins:               disk 1
+  apparent file type:                             binary
+  Unix file attributes (040755 octal):            drwxr-xr-x
+  MS-DOS file attributes (10 hex):                dir 
+
+  The central-directory extra field contains:
+  - A subfield with ID 0x5455 (universal time) and 5 data bytes.
+    The local extra field has UTC/GMT modification/access times.
+  - A subfield with ID 0x7875 (Unix UID/GID (any size)) and 11 data bytes:
+    01 04 e3 3d 03 00 04 64 00 00 00.
+
+  There is no file comment.
+
+Central directory entry #92:
 ---------------------------
 
   torchtune/modules/__init__.py
 
-  offset of local header from start of archive:   87706
-                                                  (000000000001569Ah) bytes
+  offset of local header from start of archive:   112897
+                                                  (000000000001B901h) bytes
   file system or operating system of origin:      Unix
-  version of encoding software:                   2.0
+  version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
-  compression sub-type (deflation):               normal
+  compression sub-type (deflation):               maximum
   file security status:                           not encrypted
   extended local header:                          no
-  file last modified on (DOS date/time):          2024 Mar 21 19:57:36
-  32-bit CRC value (hex):                         4a979270
-  compressed size:                                377 bytes
-  uncompressed size:                              873 bytes
+  file last modified on (DOS date/time):          2024 Apr 16 01:12:14
+  file last modified on (UT extra field modtime): 2024 Apr 16 08:12:14 local
+  file last modified on (UT extra field modtime): 2024 Apr 16 08:12:14 UTC
+  32-bit CRC value (hex):                         0eca5a88
+  compressed size:                                422 bytes
+  uncompressed size:                              994 bytes
   length of filename:                             29 characters
-  length of extra field:                          0 bytes
+  length of extra field:                          24 bytes
   length of file comment:                         0 characters
   disk number on which file begins:               disk 1
-  apparent file type:                             binary
-  Unix file attributes (100664 octal):            -rw-rw-r--
+  apparent file type:                             text
+  Unix file attributes (100644 octal):            -rw-r--r--
   MS-DOS file attributes (00 hex):                none
 
+  The central-directory extra field contains:
+  - A subfield with ID 0x5455 (universal time) and 5 data bytes.
+    The local extra field has UTC/GMT modification/access times.
+  - A subfield with ID 0x7875 (Unix UID/GID (any size)) and 11 data bytes:
+    01 04 e3 3d 03 00 04 64 00 00 00.
+
   There is no file comment.
 
-Central directory entry #85:
+Central directory entry #93:
 ---------------------------
 
   torchtune/modules/attention.py
 
-  offset of local header from start of archive:   88142
-                                                  (000000000001584Eh) bytes
+  offset of local header from start of archive:   113406
+                                                  (000000000001BAFEh) bytes
   file system or operating system of origin:      Unix
-  version of encoding software:                   2.0
+  version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
-  compression sub-type (deflation):               normal
+  compression sub-type (deflation):               maximum
   file security status:                           not encrypted
   extended local header:                          no
-  file last modified on (DOS date/time):          2024 Mar 21 19:57:36
-  32-bit CRC value (hex):                         2b0ffc7b
-  compressed size:                                2536 bytes
-  uncompressed size:                              9155 bytes
+  file last modified on (DOS date/time):          2024 Apr 16 01:12:14
+  file last modified on (UT extra field modtime): 2024 Apr 16 08:12:14 local
+  file last modified on (UT extra field modtime): 2024 Apr 16 08:12:14 UTC
+  32-bit CRC value (hex):                         2ecd9041
+  compressed size:                                2532 bytes
+  uncompressed size:                              9266 bytes
   length of filename:                             30 characters
-  length of extra field:                          0 bytes
+  length of extra field:                          24 bytes
   length of file comment:                         0 characters
   disk number on which file begins:               disk 1
-  apparent file type:                             binary
-  Unix file attributes (100664 octal):            -rw-rw-r--
+  apparent file type:                             text
+  Unix file attributes (100644 octal):            -rw-r--r--
   MS-DOS file attributes (00 hex):                none
 
+  The central-directory extra field contains:
+  - A subfield with ID 0x5455 (universal time) and 5 data bytes.
+    The local extra field has UTC/GMT modification/access times.
+  - A subfield with ID 0x7875 (Unix UID/GID (any size)) and 11 data bytes:
+    01 04 e3 3d 03 00 04 64 00 00 00.
+
   There is no file comment.
 
-Central directory entry #86:
+Central directory entry #94:
+---------------------------
+
+  torchtune/modules/common_utils.py
+
+  offset of local header from start of archive:   116026
+                                                  (000000000001C53Ah) bytes
+  file system or operating system of origin:      Unix
+  version of encoding software:                   3.0
+  minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
+  minimum software version required to extract:   2.0
+  compression method:                             deflated
+  compression sub-type (deflation):               maximum
+  file security status:                           not encrypted
+  extended local header:                          no
+  file last modified on (DOS date/time):          2024 Apr 16 01:12:14
+  file last modified on (UT extra field modtime): 2024 Apr 16 08:12:14 local
+  file last modified on (UT extra field modtime): 2024 Apr 16 08:12:14 UTC
+  32-bit CRC value (hex):                         ada73ace
+  compressed size:                                904 bytes
+  uncompressed size:                              2059 bytes
+  length of filename:                             33 characters
+  length of extra field:                          24 bytes
+  length of file comment:                         0 characters
+  disk number on which file begins:               disk 1
+  apparent file type:                             text
+  Unix file attributes (100644 octal):            -rw-r--r--
+  MS-DOS file attributes (00 hex):                none
+
+  The central-directory extra field contains:
+  - A subfield with ID 0x5455 (universal time) and 5 data bytes.
+    The local extra field has UTC/GMT modification/access times.
+  - A subfield with ID 0x7875 (Unix UID/GID (any size)) and 11 data bytes:
+    01 04 e3 3d 03 00 04 64 00 00 00.
+
+  There is no file comment.
+
+Central directory entry #95:
 ---------------------------
 
   torchtune/modules/feed_forward.py
 
-  offset of local header from start of archive:   90738
-                                                  (0000000000016272h) bytes
+  offset of local header from start of archive:   117021
+                                                  (000000000001C91Dh) bytes
   file system or operating system of origin:      Unix
-  version of encoding software:                   2.0
+  version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
-  compression sub-type (deflation):               normal
+  compression sub-type (deflation):               maximum
   file security status:                           not encrypted
   extended local header:                          no
-  file last modified on (DOS date/time):          2024 Mar 21 19:57:36
-  32-bit CRC value (hex):                         e590bb5f
-  compressed size:                                487 bytes
-  uncompressed size:                              1103 bytes
+  file last modified on (DOS date/time):          2024 Apr 16 01:12:14
+  file last modified on (UT extra field modtime): 2024 Apr 16 08:12:14 local
+  file last modified on (UT extra field modtime): 2024 Apr 16 08:12:14 UTC
+  32-bit CRC value (hex):                         17adb7db
+  compressed size:                                509 bytes
+  uncompressed size:                              1200 bytes
   length of filename:                             33 characters
-  length of extra field:                          0 bytes
+  length of extra field:                          24 bytes
   length of file comment:                         0 characters
   disk number on which file begins:               disk 1
-  apparent file type:                             binary
-  Unix file attributes (100664 octal):            -rw-rw-r--
+  apparent file type:                             text
+  Unix file attributes (100644 octal):            -rw-r--r--
   MS-DOS file attributes (00 hex):                none
 
+  The central-directory extra field contains:
+  - A subfield with ID 0x5455 (universal time) and 5 data bytes.
+    The local extra field has UTC/GMT modification/access times.
+  - A subfield with ID 0x7875 (Unix UID/GID (any size)) and 11 data bytes:
+    01 04 e3 3d 03 00 04 64 00 00 00.
+
   There is no file comment.
 
-Central directory entry #87:
+Central directory entry #96:
 ---------------------------
 
   torchtune/modules/kv_cache.py
 
-  offset of local header from start of archive:   91288
-                                                  (0000000000016498h) bytes
+  offset of local header from start of archive:   117621
+                                                  (000000000001CB75h) bytes
   file system or operating system of origin:      Unix
-  version of encoding software:                   2.0
+  version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
-  compression sub-type (deflation):               normal
+  compression sub-type (deflation):               maximum
   file security status:                           not encrypted
   extended local header:                          no
-  file last modified on (DOS date/time):          2024 Mar 21 19:57:36
-  32-bit CRC value (hex):                         253e8ad6
-  compressed size:                                819 bytes
-  uncompressed size:                              2228 bytes
+  file last modified on (DOS date/time):          2024 Apr 16 01:12:14
+  file last modified on (UT extra field modtime): 2024 Apr 16 08:12:14 local
+  file last modified on (UT extra field modtime): 2024 Apr 16 08:12:14 UTC
+  32-bit CRC value (hex):                         2307baee
+  compressed size:                                781 bytes
+  uncompressed size:                              1845 bytes
   length of filename:                             29 characters
-  length of extra field:                          0 bytes
+  length of extra field:                          24 bytes
   length of file comment:                         0 characters
   disk number on which file begins:               disk 1
-  apparent file type:                             binary
-  Unix file attributes (100664 octal):            -rw-rw-r--
+  apparent file type:                             text
+  Unix file attributes (100644 octal):            -rw-r--r--
   MS-DOS file attributes (00 hex):                none
 
+  The central-directory extra field contains:
+  - A subfield with ID 0x5455 (universal time) and 5 data bytes.
+    The local extra field has UTC/GMT modification/access times.
+  - A subfield with ID 0x7875 (Unix UID/GID (any size)) and 11 data bytes:
+    01 04 e3 3d 03 00 04 64 00 00 00.
+
   There is no file comment.
 
-Central directory entry #88:
+Central directory entry #97:
 ---------------------------
 
   torchtune/modules/lr_schedulers.py
 
-  offset of local header from start of archive:   92166
-                                                  (0000000000016806h) bytes
+  offset of local header from start of archive:   118489
+                                                  (000000000001CED9h) bytes
   file system or operating system of origin:      Unix
-  version of encoding software:                   2.0
+  version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
-  compression sub-type (deflation):               normal
+  compression sub-type (deflation):               maximum
   file security status:                           not encrypted
   extended local header:                          no
-  file last modified on (DOS date/time):          2024 Mar 21 19:57:36
-  32-bit CRC value (hex):                         e7a64e99
+  file last modified on (DOS date/time):          2024 Apr 16 01:12:14
+  file last modified on (UT extra field modtime): 2024 Apr 16 08:12:14 local
+  file last modified on (UT extra field modtime): 2024 Apr 16 08:12:14 UTC
+  32-bit CRC value (hex):                         a4a75d39
   compressed size:                                818 bytes
-  uncompressed size:                              1981 bytes
+  uncompressed size:                              1982 bytes
   length of filename:                             34 characters
-  length of extra field:                          0 bytes
+  length of extra field:                          24 bytes
   length of file comment:                         0 characters
   disk number on which file begins:               disk 1
-  apparent file type:                             binary
-  Unix file attributes (100664 octal):            -rw-rw-r--
+  apparent file type:                             text
+  Unix file attributes (100644 octal):            -rw-r--r--
   MS-DOS file attributes (00 hex):                none
 
+  The central-directory extra field contains:
+  - A subfield with ID 0x5455 (universal time) and 5 data bytes.
+    The local extra field has UTC/GMT modification/access times.
+  - A subfield with ID 0x7875 (Unix UID/GID (any size)) and 11 data bytes:
+    01 04 e3 3d 03 00 04 64 00 00 00.
+
   There is no file comment.
 
-Central directory entry #89:
+Central directory entry #98:
 ---------------------------
 
   torchtune/modules/position_embeddings.py
 
-  offset of local header from start of archive:   93048
-                                                  (0000000000016B78h) bytes
+  offset of local header from start of archive:   119399
+                                                  (000000000001D267h) bytes
   file system or operating system of origin:      Unix
-  version of encoding software:                   2.0
+  version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
-  compression sub-type (deflation):               normal
+  compression sub-type (deflation):               maximum
   file security status:                           not encrypted
   extended local header:                          no
-  file last modified on (DOS date/time):          2024 Mar 21 19:57:36
-  32-bit CRC value (hex):                         a984135d
-  compressed size:                                1673 bytes
-  uncompressed size:                              4291 bytes
+  file last modified on (DOS date/time):          2024 Apr 16 01:12:14
+  file last modified on (UT extra field modtime): 2024 Apr 16 08:12:14 local
+  file last modified on (UT extra field modtime): 2024 Apr 16 08:12:14 UTC
+  32-bit CRC value (hex):                         7bee82f5
+  compressed size:                                1800 bytes
+  uncompressed size:                              4621 bytes
   length of filename:                             40 characters
-  length of extra field:                          0 bytes
+  length of extra field:                          24 bytes
   length of file comment:                         0 characters
   disk number on which file begins:               disk 1
-  apparent file type:                             binary
-  Unix file attributes (100664 octal):            -rw-rw-r--
+  apparent file type:                             text
+  Unix file attributes (100644 octal):            -rw-r--r--
   MS-DOS file attributes (00 hex):                none
 
+  The central-directory extra field contains:
+  - A subfield with ID 0x5455 (universal time) and 5 data bytes.
+    The local extra field has UTC/GMT modification/access times.
+  - A subfield with ID 0x7875 (Unix UID/GID (any size)) and 11 data bytes:
+    01 04 e3 3d 03 00 04 64 00 00 00.
+
   There is no file comment.
 
-Central directory entry #90:
+Central directory entry #99:
 ---------------------------
 
   torchtune/modules/rms_norm.py
 
-  offset of local header from start of archive:   94791
-                                                  (0000000000017247h) bytes
+  offset of local header from start of archive:   121297
+                                                  (000000000001D9D1h) bytes
   file system or operating system of origin:      Unix
-  version of encoding software:                   2.0
+  version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
-  compression sub-type (deflation):               normal
+  compression sub-type (deflation):               maximum
   file security status:                           not encrypted
   extended local header:                          no
-  file last modified on (DOS date/time):          2024 Mar 21 19:57:36
+  file last modified on (DOS date/time):          2024 Apr 16 01:12:14
+  file last modified on (UT extra field modtime): 2024 Apr 16 08:12:14 local
+  file last modified on (UT extra field modtime): 2024 Apr 16 08:12:14 UTC
   32-bit CRC value (hex):                         14ada739
   compressed size:                                681 bytes
   uncompressed size:                              1273 bytes
   length of filename:                             29 characters
-  length of extra field:                          0 bytes
+  length of extra field:                          24 bytes
   length of file comment:                         0 characters
   disk number on which file begins:               disk 1
-  apparent file type:                             binary
-  Unix file attributes (100664 octal):            -rw-rw-r--
+  apparent file type:                             text
+  Unix file attributes (100644 octal):            -rw-r--r--
   MS-DOS file attributes (00 hex):                none
 
+  The central-directory extra field contains:
+  - A subfield with ID 0x5455 (universal time) and 5 data bytes.
+    The local extra field has UTC/GMT modification/access times.
+  - A subfield with ID 0x7875 (Unix UID/GID (any size)) and 11 data bytes:
+    01 04 e3 3d 03 00 04 64 00 00 00.
+
   There is no file comment.
 
-Central directory entry #91:
+Central directory entry #100:
 ---------------------------
 
   torchtune/modules/tokenizer.py
 
-  offset of local header from start of archive:   95531
-                                                  (000000000001752Bh) bytes
+  offset of local header from start of archive:   122065
+                                                  (000000000001DCD1h) bytes
   file system or operating system of origin:      Unix
-  version of encoding software:                   2.0
+  version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
-  compression sub-type (deflation):               normal
+  compression sub-type (deflation):               maximum
   file security status:                           not encrypted
   extended local header:                          no
-  file last modified on (DOS date/time):          2024 Mar 21 19:57:36
-  32-bit CRC value (hex):                         cdce9b9a
-  compressed size:                                973 bytes
-  uncompressed size:                              2720 bytes
+  file last modified on (DOS date/time):          2024 Apr 16 01:12:14
+  file last modified on (UT extra field modtime): 2024 Apr 16 08:12:14 local
+  file last modified on (UT extra field modtime): 2024 Apr 16 08:12:14 UTC
+  32-bit CRC value (hex):                         2f9c7ee6
+  compressed size:                                2496 bytes
+  uncompressed size:                              8194 bytes
   length of filename:                             30 characters
-  length of extra field:                          0 bytes
+  length of extra field:                          24 bytes
   length of file comment:                         0 characters
   disk number on which file begins:               disk 1
-  apparent file type:                             binary
-  Unix file attributes (100664 octal):            -rw-rw-r--
+  apparent file type:                             text
+  Unix file attributes (100644 octal):            -rw-r--r--
   MS-DOS file attributes (00 hex):                none
 
+  The central-directory extra field contains:
+  - A subfield with ID 0x5455 (universal time) and 5 data bytes.
+    The local extra field has UTC/GMT modification/access times.
+  - A subfield with ID 0x7875 (Unix UID/GID (any size)) and 11 data bytes:
+    01 04 e3 3d 03 00 04 64 00 00 00.
+
   There is no file comment.
 
-Central directory entry #92:
+Central directory entry #101:
 ---------------------------
 
   torchtune/modules/transformer.py
 
-  offset of local header from start of archive:   96564
-                                                  (0000000000017934h) bytes
+  offset of local header from start of archive:   124649
+                                                  (000000000001E6E9h) bytes
   file system or operating system of origin:      Unix
-  version of encoding software:                   2.0
+  version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
-  compression sub-type (deflation):               normal
+  compression sub-type (deflation):               maximum
   file security status:                           not encrypted
   extended local header:                          no
-  file last modified on (DOS date/time):          2024 Mar 21 19:57:36
-  32-bit CRC value (hex):                         a50ff5ab
-  compressed size:                                1653 bytes
-  uncompressed size:                              5276 bytes
+  file last modified on (DOS date/time):          2024 Apr 16 01:12:14
+  file last modified on (UT extra field modtime): 2024 Apr 16 08:12:14 local
+  file last modified on (UT extra field modtime): 2024 Apr 16 08:12:14 UTC
+  32-bit CRC value (hex):                         afc21cac
+  compressed size:                                2156 bytes
+  uncompressed size:                              7239 bytes
   length of filename:                             32 characters
-  length of extra field:                          0 bytes
+  length of extra field:                          24 bytes
   length of file comment:                         0 characters
   disk number on which file begins:               disk 1
-  apparent file type:                             binary
-  Unix file attributes (100664 octal):            -rw-rw-r--
+  apparent file type:                             text
+  Unix file attributes (100644 octal):            -rw-r--r--
   MS-DOS file attributes (00 hex):                none
 
+  The central-directory extra field contains:
+  - A subfield with ID 0x5455 (universal time) and 5 data bytes.
+    The local extra field has UTC/GMT modification/access times.
+  - A subfield with ID 0x7875 (Unix UID/GID (any size)) and 11 data bytes:
+    01 04 e3 3d 03 00 04 64 00 00 00.
+
   There is no file comment.
 
-Central directory entry #93:
+Central directory entry #102:
 ---------------------------
 
-  torchtune/modules/low_precision/__init__.py
+  torchtune/modules/loss/
 
-  offset of local header from start of archive:   98279
-                                                  (0000000000017FE7h) bytes
+  offset of local header from start of archive:   126895
+                                                  (000000000001EFAFh) bytes
   file system or operating system of origin:      Unix
-  version of encoding software:                   2.0
+  version of encoding software:                   3.0
+  minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
+  minimum software version required to extract:   1.0
+  compression method:                             none (stored)
+  file security status:                           not encrypted
+  extended local header:                          no
+  file last modified on (DOS date/time):          2024 Apr 15 20:08:26
+  file last modified on (UT extra field modtime): 2024 Apr 16 03:08:26 local
+  file last modified on (UT extra field modtime): 2024 Apr 16 03:08:26 UTC
+  32-bit CRC value (hex):                         00000000
+  compressed size:                                0 bytes
+  uncompressed size:                              0 bytes
+  length of filename:                             23 characters
+  length of extra field:                          24 bytes
+  length of file comment:                         0 characters
+  disk number on which file begins:               disk 1
+  apparent file type:                             binary
+  Unix file attributes (040755 octal):            drwxr-xr-x
+  MS-DOS file attributes (10 hex):                dir 
+
+  The central-directory extra field contains:
+  - A subfield with ID 0x5455 (universal time) and 5 data bytes.
+    The local extra field has UTC/GMT modification/access times.
+  - A subfield with ID 0x7875 (Unix UID/GID (any size)) and 11 data bytes:
+    01 04 e3 3d 03 00 04 64 00 00 00.
+
+  There is no file comment.
+
+Central directory entry #103:
+---------------------------
+
+  torchtune/modules/loss/__init__.py
+
+  offset of local header from start of archive:   126976
+                                                  (000000000001F000h) bytes
+  file system or operating system of origin:      Unix
+  version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
-  compression sub-type (deflation):               normal
+  compression sub-type (deflation):               maximum
   file security status:                           not encrypted
   extended local header:                          no
-  file last modified on (DOS date/time):          2024 Mar 21 19:57:36
-  32-bit CRC value (hex):                         e78079ca
-  compressed size:                                202 bytes
-  uncompressed size:                              287 bytes
-  length of filename:                             43 characters
-  length of extra field:                          0 bytes
+  file last modified on (DOS date/time):          2024 Apr 16 01:12:14
+  file last modified on (UT extra field modtime): 2024 Apr 16 08:12:14 local
+  file last modified on (UT extra field modtime): 2024 Apr 16 08:12:14 UTC
+  32-bit CRC value (hex):                         3704f911
+  compressed size:                                187 bytes
+  uncompressed size:                              257 bytes
+  length of filename:                             34 characters
+  length of extra field:                          24 bytes
   length of file comment:                         0 characters
   disk number on which file begins:               disk 1
-  apparent file type:                             binary
-  Unix file attributes (100664 octal):            -rw-rw-r--
+  apparent file type:                             text
+  Unix file attributes (100644 octal):            -rw-r--r--
   MS-DOS file attributes (00 hex):                none
 
+  The central-directory extra field contains:
+  - A subfield with ID 0x5455 (universal time) and 5 data bytes.
+    The local extra field has UTC/GMT modification/access times.
+  - A subfield with ID 0x7875 (Unix UID/GID (any size)) and 11 data bytes:
+    01 04 e3 3d 03 00 04 64 00 00 00.
+
   There is no file comment.
 
-Central directory entry #94:
+Central directory entry #104:
 ---------------------------
 
-  torchtune/modules/low_precision/nf4_linear.py
+  torchtune/modules/loss/dpo.py
 
-  offset of local header from start of archive:   98554
-                                                  (00000000000180FAh) bytes
+  offset of local header from start of archive:   127255
+                                                  (000000000001F117h) bytes
   file system or operating system of origin:      Unix
-  version of encoding software:                   2.0
+  version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
-  compression sub-type (deflation):               normal
+  compression sub-type (deflation):               maximum
   file security status:                           not encrypted
   extended local header:                          no
-  file last modified on (DOS date/time):          2024 Mar 21 19:57:36
-  32-bit CRC value (hex):                         34c66656
-  compressed size:                                1230 bytes
-  uncompressed size:                              2942 bytes
-  length of filename:                             45 characters
-  length of extra field:                          0 bytes
+  file last modified on (DOS date/time):          2024 Apr 16 01:12:14
+  file last modified on (UT extra field modtime): 2024 Apr 16 08:12:14 local
+  file last modified on (UT extra field modtime): 2024 Apr 16 08:12:14 UTC
+  32-bit CRC value (hex):                         f19ae141
+  compressed size:                                1255 bytes
+  uncompressed size:                              4554 bytes
+  length of filename:                             29 characters
+  length of extra field:                          24 bytes
   length of file comment:                         0 characters
   disk number on which file begins:               disk 1
-  apparent file type:                             binary
-  Unix file attributes (100664 octal):            -rw-rw-r--
+  apparent file type:                             text
+  Unix file attributes (100644 octal):            -rw-r--r--
   MS-DOS file attributes (00 hex):                none
 
+  The central-directory extra field contains:
+  - A subfield with ID 0x5455 (universal time) and 5 data bytes.
+    The local extra field has UTC/GMT modification/access times.
+  - A subfield with ID 0x7875 (Unix UID/GID (any size)) and 11 data bytes:
+    01 04 e3 3d 03 00 04 64 00 00 00.
+
   There is no file comment.
 
-Central directory entry #95:
+Central directory entry #105:
+---------------------------
+
+  torchtune/modules/peft/
+
+  offset of local header from start of archive:   128597
+                                                  (000000000001F655h) bytes
+  file system or operating system of origin:      Unix
+  version of encoding software:                   3.0
+  minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
+  minimum software version required to extract:   1.0
+  compression method:                             none (stored)
+  file security status:                           not encrypted
+  extended local header:                          no
+  file last modified on (DOS date/time):          2024 Apr 15 20:08:26
+  file last modified on (UT extra field modtime): 2024 Apr 16 03:08:26 local
+  file last modified on (UT extra field modtime): 2024 Apr 16 03:08:26 UTC
+  32-bit CRC value (hex):                         00000000
+  compressed size:                                0 bytes
+  uncompressed size:                              0 bytes
+  length of filename:                             23 characters
+  length of extra field:                          24 bytes
+  length of file comment:                         0 characters
+  disk number on which file begins:               disk 1
+  apparent file type:                             binary
+  Unix file attributes (040755 octal):            drwxr-xr-x
+  MS-DOS file attributes (10 hex):                dir 
+
+  The central-directory extra field contains:
+  - A subfield with ID 0x5455 (universal time) and 5 data bytes.
+    The local extra field has UTC/GMT modification/access times.
+  - A subfield with ID 0x7875 (Unix UID/GID (any size)) and 11 data bytes:
+    01 04 e3 3d 03 00 04 64 00 00 00.
+
+  There is no file comment.
+
+Central directory entry #106:
 ---------------------------
 
   torchtune/modules/peft/__init__.py
 
-  offset of local header from start of archive:   99859
-                                                  (0000000000018613h) bytes
+  offset of local header from start of archive:   128678
+                                                  (000000000001F6A6h) bytes
   file system or operating system of origin:      Unix
-  version of encoding software:                   2.0
+  version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
-  compression sub-type (deflation):               normal
+  compression sub-type (deflation):               maximum
   file security status:                           not encrypted
   extended local header:                          no
-  file last modified on (DOS date/time):          2024 Mar 21 19:57:36
-  32-bit CRC value (hex):                         e159c2ca
-  compressed size:                                302 bytes
-  uncompressed size:                              544 bytes
+  file last modified on (DOS date/time):          2024 Apr 16 01:12:14
+  file last modified on (UT extra field modtime): 2024 Apr 16 08:12:14 local
+  file last modified on (UT extra field modtime): 2024 Apr 16 08:12:14 UTC
+  32-bit CRC value (hex):                         13939f9c
+  compressed size:                                335 bytes
+  uncompressed size:                              636 bytes
   length of filename:                             34 characters
-  length of extra field:                          0 bytes
+  length of extra field:                          24 bytes
   length of file comment:                         0 characters
   disk number on which file begins:               disk 1
-  apparent file type:                             binary
-  Unix file attributes (100664 octal):            -rw-rw-r--
+  apparent file type:                             text
+  Unix file attributes (100644 octal):            -rw-r--r--
   MS-DOS file attributes (00 hex):                none
 
+  The central-directory extra field contains:
+  - A subfield with ID 0x5455 (universal time) and 5 data bytes.
+    The local extra field has UTC/GMT modification/access times.
+  - A subfield with ID 0x7875 (Unix UID/GID (any size)) and 11 data bytes:
+    01 04 e3 3d 03 00 04 64 00 00 00.
+
   There is no file comment.
 
-Central directory entry #96:
+Central directory entry #107:
 ---------------------------
 
   torchtune/modules/peft/lora.py
 
-  offset of local header from start of archive:   100225
-                                                  (0000000000018781h) bytes
+  offset of local header from start of archive:   129105
+                                                  (000000000001F851h) bytes
   file system or operating system of origin:      Unix
-  version of encoding software:                   2.0
+  version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
-  compression sub-type (deflation):               normal
+  compression sub-type (deflation):               maximum
   file security status:                           not encrypted
   extended local header:                          no
-  file last modified on (DOS date/time):          2024 Mar 21 19:57:36
-  32-bit CRC value (hex):                         2595749f
-  compressed size:                                1705 bytes
-  uncompressed size:                              4447 bytes
+  file last modified on (DOS date/time):          2024 Apr 16 01:12:14
+  file last modified on (UT extra field modtime): 2024 Apr 16 08:12:14 local
+  file last modified on (UT extra field modtime): 2024 Apr 16 08:12:14 UTC
+  32-bit CRC value (hex):                         caafff68
+  compressed size:                                2121 bytes
+  uncompressed size:                              5749 bytes
   length of filename:                             30 characters
-  length of extra field:                          0 bytes
+  length of extra field:                          24 bytes
   length of file comment:                         0 characters
   disk number on which file begins:               disk 1
-  apparent file type:                             binary
-  Unix file attributes (100664 octal):            -rw-rw-r--
+  apparent file type:                             text
+  Unix file attributes (100644 octal):            -rw-r--r--
   MS-DOS file attributes (00 hex):                none
 
+  The central-directory extra field contains:
+  - A subfield with ID 0x5455 (universal time) and 5 data bytes.
+    The local extra field has UTC/GMT modification/access times.
+  - A subfield with ID 0x7875 (Unix UID/GID (any size)) and 11 data bytes:
+    01 04 e3 3d 03 00 04 64 00 00 00.
+
   There is no file comment.
 
-Central directory entry #97:
+Central directory entry #108:
 ---------------------------
 
   torchtune/modules/peft/peft_utils.py
 
-  offset of local header from start of archive:   101990
-                                                  (0000000000018E66h) bytes
+  offset of local header from start of archive:   131314
+                                                  (00000000000200F2h) bytes
   file system or operating system of origin:      Unix
-  version of encoding software:                   2.0
+  version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
-  compression sub-type (deflation):               normal
+  compression sub-type (deflation):               maximum
   file security status:                           not encrypted
   extended local header:                          no
-  file last modified on (DOS date/time):          2024 Mar 21 19:57:36
-  32-bit CRC value (hex):                         f4a608cd
-  compressed size:                                2830 bytes
-  uncompressed size:                              10703 bytes
+  file last modified on (DOS date/time):          2024 Apr 16 01:12:14
+  file last modified on (UT extra field modtime): 2024 Apr 16 08:12:14 local
+  file last modified on (UT extra field modtime): 2024 Apr 16 08:12:14 UTC
+  32-bit CRC value (hex):                         270b8d15
+  compressed size:                                3462 bytes
+  uncompressed size:                              14306 bytes
   length of filename:                             36 characters
-  length of extra field:                          0 bytes
+  length of extra field:                          24 bytes
   length of file comment:                         0 characters
   disk number on which file begins:               disk 1
-  apparent file type:                             binary
-  Unix file attributes (100664 octal):            -rw-rw-r--
+  apparent file type:                             text
+  Unix file attributes (100644 octal):            -rw-r--r--
   MS-DOS file attributes (00 hex):                none
 
+  The central-directory extra field contains:
+  - A subfield with ID 0x5455 (universal time) and 5 data bytes.
+    The local extra field has UTC/GMT modification/access times.
+  - A subfield with ID 0x7875 (Unix UID/GID (any size)) and 11 data bytes:
+    01 04 e3 3d 03 00 04 64 00 00 00.
+
   There is no file comment.
 
-Central directory entry #98:
+Central directory entry #109:
+---------------------------
+
+  torchtune/utils/
+
+  offset of local header from start of archive:   134870
+                                                  (0000000000020ED6h) bytes
+  file system or operating system of origin:      Unix
+  version of encoding software:                   3.0
+  minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
+  minimum software version required to extract:   1.0
+  compression method:                             none (stored)
+  file security status:                           not encrypted
+  extended local header:                          no
+  file last modified on (DOS date/time):          2024 Apr 15 20:08:26
+  file last modified on (UT extra field modtime): 2024 Apr 16 03:08:26 local
+  file last modified on (UT extra field modtime): 2024 Apr 16 03:08:26 UTC
+  32-bit CRC value (hex):                         00000000
+  compressed size:                                0 bytes
+  uncompressed size:                              0 bytes
+  length of filename:                             16 characters
+  length of extra field:                          24 bytes
+  length of file comment:                         0 characters
+  disk number on which file begins:               disk 1
+  apparent file type:                             binary
+  Unix file attributes (040755 octal):            drwxr-xr-x
+  MS-DOS file attributes (10 hex):                dir 
+
+  The central-directory extra field contains:
+  - A subfield with ID 0x5455 (universal time) and 5 data bytes.
+    The local extra field has UTC/GMT modification/access times.
+  - A subfield with ID 0x7875 (Unix UID/GID (any size)) and 11 data bytes:
+    01 04 e3 3d 03 00 04 64 00 00 00.
+
+  There is no file comment.
+
+Central directory entry #110:
 ---------------------------
 
   torchtune/utils/__init__.py
 
-  offset of local header from start of archive:   104886
-                                                  (00000000000199B6h) bytes
+  offset of local header from start of archive:   134944
+                                                  (0000000000020F20h) bytes
   file system or operating system of origin:      Unix
-  version of encoding software:                   2.0
+  version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
-  compression sub-type (deflation):               normal
+  compression sub-type (deflation):               maximum
   file security status:                           not encrypted
   extended local header:                          no
-  file last modified on (DOS date/time):          2024 Mar 21 19:57:36
-  32-bit CRC value (hex):                         d9596ed1
-  compressed size:                                702 bytes
-  uncompressed size:                              1901 bytes
+  file last modified on (DOS date/time):          2024 Apr 16 01:12:14
+  file last modified on (UT extra field modtime): 2024 Apr 16 08:12:14 local
+  file last modified on (UT extra field modtime): 2024 Apr 16 08:12:14 UTC
+  32-bit CRC value (hex):                         884b6e2b
+  compressed size:                                840 bytes
+  uncompressed size:                              2301 bytes
   length of filename:                             27 characters
-  length of extra field:                          0 bytes
+  length of extra field:                          24 bytes
   length of file comment:                         0 characters
   disk number on which file begins:               disk 1
-  apparent file type:                             binary
-  Unix file attributes (100664 octal):            -rw-rw-r--
+  apparent file type:                             text
+  Unix file attributes (100644 octal):            -rw-r--r--
   MS-DOS file attributes (00 hex):                none
 
+  The central-directory extra field contains:
+  - A subfield with ID 0x5455 (universal time) and 5 data bytes.
+    The local extra field has UTC/GMT modification/access times.
+  - A subfield with ID 0x7875 (Unix UID/GID (any size)) and 11 data bytes:
+    01 04 e3 3d 03 00 04 64 00 00 00.
+
   There is no file comment.
 
-Central directory entry #99:
+Central directory entry #111:
+---------------------------
+
+  torchtune/utils/_compile_utils.py
+
+  offset of local header from start of archive:   135869
+                                                  (00000000000212BDh) bytes
+  file system or operating system of origin:      Unix
+  version of encoding software:                   3.0
+  minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
+  minimum software version required to extract:   2.0
+  compression method:                             deflated
+  compression sub-type (deflation):               maximum
+  file security status:                           not encrypted
+  extended local header:                          no
+  file last modified on (DOS date/time):          2024 Apr 16 01:12:14
+  file last modified on (UT extra field modtime): 2024 Apr 16 08:12:14 local
+  file last modified on (UT extra field modtime): 2024 Apr 16 08:12:14 UTC
+  32-bit CRC value (hex):                         abb16159
+  compressed size:                                729 bytes
+  uncompressed size:                              1509 bytes
+  length of filename:                             33 characters
+  length of extra field:                          24 bytes
+  length of file comment:                         0 characters
+  disk number on which file begins:               disk 1
+  apparent file type:                             text
+  Unix file attributes (100644 octal):            -rw-r--r--
+  MS-DOS file attributes (00 hex):                none
+
+  The central-directory extra field contains:
+  - A subfield with ID 0x5455 (universal time) and 5 data bytes.
+    The local extra field has UTC/GMT modification/access times.
+  - A subfield with ID 0x7875 (Unix UID/GID (any size)) and 11 data bytes:
+    01 04 e3 3d 03 00 04 64 00 00 00.
+
+  There is no file comment.
+
+Central directory entry #112:
 ---------------------------
 
   torchtune/utils/_device.py
 
-  offset of local header from start of archive:   105645
-                                                  (0000000000019CADh) bytes
+  offset of local header from start of archive:   136689
+                                                  (00000000000215F1h) bytes
   file system or operating system of origin:      Unix
-  version of encoding software:                   2.0
+  version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
-  compression sub-type (deflation):               normal
+  compression sub-type (deflation):               maximum
   file security status:                           not encrypted
   extended local header:                          no
-  file last modified on (DOS date/time):          2024 Mar 21 19:57:36
+  file last modified on (DOS date/time):          2024 Apr 16 01:12:14
+  file last modified on (UT extra field modtime): 2024 Apr 16 08:12:14 local
+  file last modified on (UT extra field modtime): 2024 Apr 16 08:12:14 UTC
   32-bit CRC value (hex):                         a79d1929
-  compressed size:                                1100 bytes
+  compressed size:                                1097 bytes
   uncompressed size:                              3446 bytes
   length of filename:                             26 characters
-  length of extra field:                          0 bytes
+  length of extra field:                          24 bytes
   length of file comment:                         0 characters
   disk number on which file begins:               disk 1
-  apparent file type:                             binary
-  Unix file attributes (100664 octal):            -rw-rw-r--
+  apparent file type:                             text
+  Unix file attributes (100644 octal):            -rw-r--r--
   MS-DOS file attributes (00 hex):                none
 
+  The central-directory extra field contains:
+  - A subfield with ID 0x5455 (universal time) and 5 data bytes.
+    The local extra field has UTC/GMT modification/access times.
+  - A subfield with ID 0x7875 (Unix UID/GID (any size)) and 11 data bytes:
+    01 04 e3 3d 03 00 04 64 00 00 00.
+
   There is no file comment.
 
-Central directory entry #100:
+Central directory entry #113:
 ---------------------------
 
   torchtune/utils/_distributed.py
 
-  offset of local header from start of archive:   106801
-                                                  (000000000001A131h) bytes
+  offset of local header from start of archive:   137870
+                                                  (0000000000021A8Eh) bytes
   file system or operating system of origin:      Unix
-  version of encoding software:                   2.0
+  version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
-  compression sub-type (deflation):               normal
+  compression sub-type (deflation):               maximum
   file security status:                           not encrypted
   extended local header:                          no
-  file last modified on (DOS date/time):          2024 Mar 21 19:57:36
-  32-bit CRC value (hex):                         ed37aff9
-  compressed size:                                4028 bytes
-  uncompressed size:                              11990 bytes
+  file last modified on (DOS date/time):          2024 Apr 16 01:12:14
+  file last modified on (UT extra field modtime): 2024 Apr 16 08:12:14 local
+  file last modified on (UT extra field modtime): 2024 Apr 16 08:12:14 UTC
+  32-bit CRC value (hex):                         3a756b5b
+  compressed size:                                3842 bytes
+  uncompressed size:                              11462 bytes
   length of filename:                             31 characters
-  length of extra field:                          0 bytes
+  length of extra field:                          24 bytes
   length of file comment:                         0 characters
   disk number on which file begins:               disk 1
-  apparent file type:                             binary
-  Unix file attributes (100664 octal):            -rw-rw-r--
+  apparent file type:                             text
+  Unix file attributes (100644 octal):            -rw-r--r--
   MS-DOS file attributes (00 hex):                none
 
+  The central-directory extra field contains:
+  - A subfield with ID 0x5455 (universal time) and 5 data bytes.
+    The local extra field has UTC/GMT modification/access times.
+  - A subfield with ID 0x7875 (Unix UID/GID (any size)) and 11 data bytes:
+    01 04 e3 3d 03 00 04 64 00 00 00.
+
   There is no file comment.
 
-Central directory entry #101:
+Central directory entry #114:
 ---------------------------
 
-  torchtune/utils/argparse.py
+  torchtune/utils/_generation.py
 
-  offset of local header from start of archive:   110890
-                                                  (000000000001B12Ah) bytes
+  offset of local header from start of archive:   141801
+                                                  (00000000000229E9h) bytes
   file system or operating system of origin:      Unix
-  version of encoding software:                   2.0
+  version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
-  compression sub-type (deflation):               normal
+  compression sub-type (deflation):               maximum
   file security status:                           not encrypted
   extended local header:                          no
-  file last modified on (DOS date/time):          2024 Mar 21 19:57:36
-  32-bit CRC value (hex):                         41256619
-  compressed size:                                1092 bytes
-  uncompressed size:                              2647 bytes
-  length of filename:                             27 characters
-  length of extra field:                          0 bytes
+  file last modified on (DOS date/time):          2024 Apr 16 01:12:14
+  file last modified on (UT extra field modtime): 2024 Apr 16 08:12:14 local
+  file last modified on (UT extra field modtime): 2024 Apr 16 08:12:14 UTC
+  32-bit CRC value (hex):                         b89109d4
+  compressed size:                                1763 bytes
+  uncompressed size:                              5012 bytes
+  length of filename:                             30 characters
+  length of extra field:                          24 bytes
   length of file comment:                         0 characters
   disk number on which file begins:               disk 1
-  apparent file type:                             binary
-  Unix file attributes (100664 octal):            -rw-rw-r--
+  apparent file type:                             text
+  Unix file attributes (100644 octal):            -rw-r--r--
   MS-DOS file attributes (00 hex):                none
 
+  The central-directory extra field contains:
+  - A subfield with ID 0x5455 (universal time) and 5 data bytes.
+    The local extra field has UTC/GMT modification/access times.
+  - A subfield with ID 0x7875 (Unix UID/GID (any size)) and 11 data bytes:
+    01 04 e3 3d 03 00 04 64 00 00 00.
+
   There is no file comment.
 
-Central directory entry #102:
+Central directory entry #115:
 ---------------------------
 
-  torchtune/utils/checkpoint.py
+  torchtune/utils/_profiler.py
 
-  offset of local header from start of archive:   112039
-                                                  (000000000001B5A7h) bytes
+  offset of local header from start of archive:   143652
+                                                  (0000000000023124h) bytes
   file system or operating system of origin:      Unix
-  version of encoding software:                   2.0
+  version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
-  compression sub-type (deflation):               normal
+  compression sub-type (deflation):               maximum
   file security status:                           not encrypted
   extended local header:                          no
-  file last modified on (DOS date/time):          2024 Mar 21 19:57:36
-  32-bit CRC value (hex):                         3a38a824
-  compressed size:                                2447 bytes
-  uncompressed size:                              8552 bytes
-  length of filename:                             29 characters
-  length of extra field:                          0 bytes
+  file last modified on (DOS date/time):          2024 Apr 16 01:12:14
+  file last modified on (UT extra field modtime): 2024 Apr 16 08:12:14 local
+  file last modified on (UT extra field modtime): 2024 Apr 16 08:12:14 UTC
+  32-bit CRC value (hex):                         fd73a7dd
+  compressed size:                                719 bytes
+  uncompressed size:                              1613 bytes
+  length of filename:                             28 characters
+  length of extra field:                          24 bytes
   length of file comment:                         0 characters
   disk number on which file begins:               disk 1
-  apparent file type:                             binary
-  Unix file attributes (100664 octal):            -rw-rw-r--
+  apparent file type:                             text
+  Unix file attributes (100644 octal):            -rw-r--r--
   MS-DOS file attributes (00 hex):                none
 
+  The central-directory extra field contains:
+  - A subfield with ID 0x5455 (universal time) and 5 data bytes.
+    The local extra field has UTC/GMT modification/access times.
+  - A subfield with ID 0x7875 (Unix UID/GID (any size)) and 11 data bytes:
+    01 04 e3 3d 03 00 04 64 00 00 00.
+
   There is no file comment.
 
-Central directory entry #103:
+Central directory entry #116:
 ---------------------------
 
-  torchtune/utils/checkpointable_dataloader.py
+  torchtune/utils/_register_nf4_dispatch_ops.py
 
-  offset of local header from start of archive:   114545
-                                                  (000000000001BF71h) bytes
+  offset of local header from start of archive:   144457
+                                                  (0000000000023449h) bytes
   file system or operating system of origin:      Unix
-  version of encoding software:                   2.0
+  version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
-  compression sub-type (deflation):               normal
+  compression sub-type (deflation):               maximum
   file security status:                           not encrypted
   extended local header:                          no
-  file last modified on (DOS date/time):          2024 Mar 21 19:57:36
-  32-bit CRC value (hex):                         cbcd8fcf
-  compressed size:                                2057 bytes
-  uncompressed size:                              6898 bytes
-  length of filename:                             44 characters
-  length of extra field:                          0 bytes
+  file last modified on (DOS date/time):          2024 Apr 16 01:12:14
+  file last modified on (UT extra field modtime): 2024 Apr 16 08:12:14 local
+  file last modified on (UT extra field modtime): 2024 Apr 16 08:12:14 UTC
+  32-bit CRC value (hex):                         2090881a
+  compressed size:                                739 bytes
+  uncompressed size:                              1785 bytes
+  length of filename:                             45 characters
+  length of extra field:                          24 bytes
   length of file comment:                         0 characters
   disk number on which file begins:               disk 1
-  apparent file type:                             binary
-  Unix file attributes (100664 octal):            -rw-rw-r--
+  apparent file type:                             text
+  Unix file attributes (100644 octal):            -rw-r--r--
   MS-DOS file attributes (00 hex):                none
 
+  The central-directory extra field contains:
+  - A subfield with ID 0x5455 (universal time) and 5 data bytes.
+    The local extra field has UTC/GMT modification/access times.
+  - A subfield with ID 0x7875 (Unix UID/GID (any size)) and 11 data bytes:
+    01 04 e3 3d 03 00 04 64 00 00 00.
+
   There is no file comment.
 
-Central directory entry #104:
+Central directory entry #117:
 ---------------------------
 
-  torchtune/utils/collate.py
+  torchtune/utils/argparse.py
 
-  offset of local header from start of archive:   116676
-                                                  (000000000001C7C4h) bytes
+  offset of local header from start of archive:   145299
+                                                  (0000000000023793h) bytes
   file system or operating system of origin:      Unix
-  version of encoding software:                   2.0
+  version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
-  compression sub-type (deflation):               normal
+  compression sub-type (deflation):               maximum
   file security status:                           not encrypted
   extended local header:                          no
-  file last modified on (DOS date/time):          2024 Mar 21 19:57:36
-  32-bit CRC value (hex):                         7553c9c3
-  compressed size:                                850 bytes
-  uncompressed size:                              2239 bytes
-  length of filename:                             26 characters
-  length of extra field:                          0 bytes
+  file last modified on (DOS date/time):          2024 Apr 16 01:12:14
+  file last modified on (UT extra field modtime): 2024 Apr 16 08:12:14 local
+  file last modified on (UT extra field modtime): 2024 Apr 16 08:12:14 UTC
+  32-bit CRC value (hex):                         aa04875d
+  compressed size:                                1101 bytes
+  uncompressed size:                              2622 bytes
+  length of filename:                             27 characters
+  length of extra field:                          24 bytes
   length of file comment:                         0 characters
   disk number on which file begins:               disk 1
-  apparent file type:                             binary
-  Unix file attributes (100664 octal):            -rw-rw-r--
+  apparent file type:                             text
+  Unix file attributes (100644 octal):            -rw-r--r--
   MS-DOS file attributes (00 hex):                none
 
+  The central-directory extra field contains:
+  - A subfield with ID 0x5455 (universal time) and 5 data bytes.
+    The local extra field has UTC/GMT modification/access times.
+  - A subfield with ID 0x7875 (Unix UID/GID (any size)) and 11 data bytes:
+    01 04 e3 3d 03 00 04 64 00 00 00.
+
   There is no file comment.
 
-Central directory entry #105:
+Central directory entry #118:
 ---------------------------
 
-  torchtune/utils/constants.py
+  torchtune/utils/collate.py
 
-  offset of local header from start of archive:   117582
-                                                  (000000000001CB4Eh) bytes
+  offset of local header from start of archive:   146485
+                                                  (0000000000023C35h) bytes
   file system or operating system of origin:      Unix
-  version of encoding software:                   2.0
+  version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
-  compression sub-type (deflation):               normal
+  compression sub-type (deflation):               maximum
   file security status:                           not encrypted
   extended local header:                          no
-  file last modified on (DOS date/time):          2024 Mar 21 19:57:36
-  32-bit CRC value (hex):                         fb97ad99
-  compressed size:                                378 bytes
-  uncompressed size:                              657 bytes
-  length of filename:                             28 characters
-  length of extra field:                          0 bytes
+  file last modified on (DOS date/time):          2024 Apr 16 01:12:14
+  file last modified on (UT extra field modtime): 2024 Apr 16 08:12:14 local
+  file last modified on (UT extra field modtime): 2024 Apr 16 08:12:14 UTC
+  32-bit CRC value (hex):                         1d2a0e59
+  compressed size:                                1437 bytes
+  uncompressed size:                              4845 bytes
+  length of filename:                             26 characters
+  length of extra field:                          24 bytes
   length of file comment:                         0 characters
   disk number on which file begins:               disk 1
-  apparent file type:                             binary
-  Unix file attributes (100664 octal):            -rw-rw-r--
+  apparent file type:                             text
+  Unix file attributes (100644 octal):            -rw-r--r--
   MS-DOS file attributes (00 hex):                none
 
+  The central-directory extra field contains:
+  - A subfield with ID 0x5455 (universal time) and 5 data bytes.
+    The local extra field has UTC/GMT modification/access times.
+  - A subfield with ID 0x7875 (Unix UID/GID (any size)) and 11 data bytes:
+    01 04 e3 3d 03 00 04 64 00 00 00.
+
   There is no file comment.
 
-Central directory entry #106:
+Central directory entry #119:
 ---------------------------
 
-  torchtune/utils/generation.py
+  torchtune/utils/constants.py
 
-  offset of local header from start of archive:   118018
-                                                  (000000000001CD02h) bytes
+  offset of local header from start of archive:   148006
+                                                  (0000000000024226h) bytes
   file system or operating system of origin:      Unix
-  version of encoding software:                   2.0
+  version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
-  compression sub-type (deflation):               normal
+  compression sub-type (deflation):               maximum
   file security status:                           not encrypted
   extended local header:                          no
-  file last modified on (DOS date/time):          2024 Mar 21 19:57:36
-  32-bit CRC value (hex):                         ea129f66
-  compressed size:                                2853 bytes
-  uncompressed size:                              9479 bytes
-  length of filename:                             29 characters
-  length of extra field:                          0 bytes
+  file last modified on (DOS date/time):          2024 Apr 16 01:12:14
+  file last modified on (UT extra field modtime): 2024 Apr 16 08:12:14 local
+  file last modified on (UT extra field modtime): 2024 Apr 16 08:12:14 UTC
+  32-bit CRC value (hex):                         fb97ad99
+  compressed size:                                378 bytes
+  uncompressed size:                              657 bytes
+  length of filename:                             28 characters
+  length of extra field:                          24 bytes
   length of file comment:                         0 characters
   disk number on which file begins:               disk 1
-  apparent file type:                             binary
-  Unix file attributes (100664 octal):            -rw-rw-r--
+  apparent file type:                             text
+  Unix file attributes (100644 octal):            -rw-r--r--
   MS-DOS file attributes (00 hex):                none
 
+  The central-directory extra field contains:
+  - A subfield with ID 0x5455 (universal time) and 5 data bytes.
+    The local extra field has UTC/GMT modification/access times.
+  - A subfield with ID 0x7875 (Unix UID/GID (any size)) and 11 data bytes:
+    01 04 e3 3d 03 00 04 64 00 00 00.
+
   There is no file comment.
 
-Central directory entry #107:
+Central directory entry #120:
 ---------------------------
 
   torchtune/utils/logging.py
 
-  offset of local header from start of archive:   120930
-                                                  (000000000001D862h) bytes
+  offset of local header from start of archive:   148470
+                                                  (00000000000243F6h) bytes
   file system or operating system of origin:      Unix
-  version of encoding software:                   2.0
+  version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
-  compression sub-type (deflation):               normal
+  compression sub-type (deflation):               maximum
   file security status:                           not encrypted
   extended local header:                          no
-  file last modified on (DOS date/time):          2024 Mar 21 19:57:36
+  file last modified on (DOS date/time):          2024 Apr 16 01:12:14
+  file last modified on (UT extra field modtime): 2024 Apr 16 08:12:14 local
+  file last modified on (UT extra field modtime): 2024 Apr 16 08:12:14 UTC
   32-bit CRC value (hex):                         b18086c6
   compressed size:                                422 bytes
   uncompressed size:                              810 bytes
   length of filename:                             26 characters
-  length of extra field:                          0 bytes
+  length of extra field:                          24 bytes
   length of file comment:                         0 characters
   disk number on which file begins:               disk 1
-  apparent file type:                             binary
-  Unix file attributes (100664 octal):            -rw-rw-r--
+  apparent file type:                             text
+  Unix file attributes (100644 octal):            -rw-r--r--
   MS-DOS file attributes (00 hex):                none
 
+  The central-directory extra field contains:
+  - A subfield with ID 0x5455 (universal time) and 5 data bytes.
+    The local extra field has UTC/GMT modification/access times.
+  - A subfield with ID 0x7875 (Unix UID/GID (any size)) and 11 data bytes:
+    01 04 e3 3d 03 00 04 64 00 00 00.
+
   There is no file comment.
 
-Central directory entry #108:
+Central directory entry #121:
 ---------------------------
 
-  torchtune/utils/logits_transforms.py
+  torchtune/utils/memory.py
 
-  offset of local header from start of archive:   121408
-                                                  (000000000001DA40h) bytes
+  offset of local header from start of archive:   148976
+                                                  (00000000000245F0h) bytes
   file system or operating system of origin:      Unix
-  version of encoding software:                   2.0
+  version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
-  compression sub-type (deflation):               normal
+  compression sub-type (deflation):               maximum
   file security status:                           not encrypted
   extended local header:                          no
-  file last modified on (DOS date/time):          2024 Mar 21 19:57:36
-  32-bit CRC value (hex):                         e85d5888
-  compressed size:                                1052 bytes
-  uncompressed size:                              3171 bytes
-  length of filename:                             36 characters
-  length of extra field:                          0 bytes
+  file last modified on (DOS date/time):          2024 Apr 16 01:12:14
+  file last modified on (UT extra field modtime): 2024 Apr 16 08:12:14 local
+  file last modified on (UT extra field modtime): 2024 Apr 16 08:12:14 UTC
+  32-bit CRC value (hex):                         e02f2652
+  compressed size:                                2383 bytes
+  uncompressed size:                              7480 bytes
+  length of filename:                             25 characters
+  length of extra field:                          24 bytes
   length of file comment:                         0 characters
   disk number on which file begins:               disk 1
-  apparent file type:                             binary
-  Unix file attributes (100664 octal):            -rw-rw-r--
+  apparent file type:                             text
+  Unix file attributes (100644 octal):            -rw-r--r--
   MS-DOS file attributes (00 hex):                none
 
+  The central-directory extra field contains:
+  - A subfield with ID 0x5455 (universal time) and 5 data bytes.
+    The local extra field has UTC/GMT modification/access times.
+  - A subfield with ID 0x7875 (Unix UID/GID (any size)) and 11 data bytes:
+    01 04 e3 3d 03 00 04 64 00 00 00.
+
   There is no file comment.
 
-Central directory entry #109:
+Central directory entry #122:
 ---------------------------
 
-  torchtune/utils/memory.py
+  torchtune/utils/metric_logging.py
 
-  offset of local header from start of archive:   122526
-                                                  (000000000001DE9Eh) bytes
+  offset of local header from start of archive:   151442
+                                                  (0000000000024F92h) bytes
   file system or operating system of origin:      Unix
-  version of encoding software:                   2.0
+  version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
-  compression sub-type (deflation):               normal
+  compression sub-type (deflation):               maximum
   file security status:                           not encrypted
   extended local header:                          no
-  file last modified on (DOS date/time):          2024 Mar 21 19:57:36
-  32-bit CRC value (hex):                         9d7d489a
-  compressed size:                                949 bytes
-  uncompressed size:                              2342 bytes
-  length of filename:                             25 characters
-  length of extra field:                          0 bytes
+  file last modified on (DOS date/time):          2024 Apr 16 01:12:14
+  file last modified on (UT extra field modtime): 2024 Apr 16 08:12:14 local
+  file last modified on (UT extra field modtime): 2024 Apr 16 08:12:14 UTC
+  32-bit CRC value (hex):                         cff285d1
+  compressed size:                                2867 bytes
+  uncompressed size:                              9919 bytes
+  length of filename:                             33 characters
+  length of extra field:                          24 bytes
   length of file comment:                         0 characters
   disk number on which file begins:               disk 1
-  apparent file type:                             binary
-  Unix file attributes (100664 octal):            -rw-rw-r--
+  apparent file type:                             text
+  Unix file attributes (100644 octal):            -rw-r--r--
   MS-DOS file attributes (00 hex):                none
 
+  The central-directory extra field contains:
+  - A subfield with ID 0x5455 (universal time) and 5 data bytes.
+    The local extra field has UTC/GMT modification/access times.
+  - A subfield with ID 0x7875 (Unix UID/GID (any size)) and 11 data bytes:
+    01 04 e3 3d 03 00 04 64 00 00 00.
+
   There is no file comment.
 
-Central directory entry #110:
+Central directory entry #123:
 ---------------------------
 
-  torchtune/utils/metric_logging.py
+  torchtune/utils/precision.py
 
-  offset of local header from start of archive:   123530
-                                                  (000000000001E28Ah) bytes
+  offset of local header from start of archive:   154400
+                                                  (0000000000025B20h) bytes
   file system or operating system of origin:      Unix
-  version of encoding software:                   2.0
+  version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
-  compression sub-type (deflation):               normal
+  compression sub-type (deflation):               maximum
   file security status:                           not encrypted
   extended local header:                          no
-  file last modified on (DOS date/time):          2024 Mar 21 19:57:36
-  32-bit CRC value (hex):                         1c56de41
-  compressed size:                                2372 bytes
-  uncompressed size:                              7930 bytes
-  length of filename:                             33 characters
-  length of extra field:                          0 bytes
+  file last modified on (DOS date/time):          2024 Apr 16 01:12:14
+  file last modified on (UT extra field modtime): 2024 Apr 16 08:12:14 local
+  file last modified on (UT extra field modtime): 2024 Apr 16 08:12:14 UTC
+  32-bit CRC value (hex):                         39fa419f
+  compressed size:                                2245 bytes
+  uncompressed size:                              6399 bytes
+  length of filename:                             28 characters
+  length of extra field:                          24 bytes
   length of file comment:                         0 characters
   disk number on which file begins:               disk 1
-  apparent file type:                             binary
-  Unix file attributes (100664 octal):            -rw-rw-r--
+  apparent file type:                             text
+  Unix file attributes (100644 octal):            -rw-r--r--
   MS-DOS file attributes (00 hex):                none
 
+  The central-directory extra field contains:
+  - A subfield with ID 0x5455 (universal time) and 5 data bytes.
+    The local extra field has UTC/GMT modification/access times.
+  - A subfield with ID 0x7875 (Unix UID/GID (any size)) and 11 data bytes:
+    01 04 e3 3d 03 00 04 64 00 00 00.
+
   There is no file comment.
 
-Central directory entry #111:
+Central directory entry #124:
 ---------------------------
 
-  torchtune/utils/precision.py
+  torchtune/utils/quantization.py
 
-  offset of local header from start of archive:   125965
-                                                  (000000000001EC0Dh) bytes
+  offset of local header from start of archive:   156731
+                                                  (000000000002643Bh) bytes
   file system or operating system of origin:      Unix
-  version of encoding software:                   2.0
+  version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
-  compression sub-type (deflation):               normal
+  compression sub-type (deflation):               maximum
   file security status:                           not encrypted
   extended local header:                          no
-  file last modified on (DOS date/time):          2024 Mar 21 19:57:36
-  32-bit CRC value (hex):                         239d564c
-  compressed size:                                1871 bytes
-  uncompressed size:                              5264 bytes
-  length of filename:                             28 characters
-  length of extra field:                          0 bytes
+  file last modified on (DOS date/time):          2024 Apr 16 01:12:14
+  file last modified on (UT extra field modtime): 2024 Apr 16 08:12:14 local
+  file last modified on (UT extra field modtime): 2024 Apr 16 08:12:14 UTC
+  32-bit CRC value (hex):                         23133d7b
+  compressed size:                                571 bytes
+  uncompressed size:                              1284 bytes
+  length of filename:                             31 characters
+  length of extra field:                          24 bytes
   length of file comment:                         0 characters
   disk number on which file begins:               disk 1
-  apparent file type:                             binary
-  Unix file attributes (100664 octal):            -rw-rw-r--
+  apparent file type:                             text
+  Unix file attributes (100644 octal):            -rw-r--r--
   MS-DOS file attributes (00 hex):                none
 
+  The central-directory extra field contains:
+  - A subfield with ID 0x5455 (universal time) and 5 data bytes.
+    The local extra field has UTC/GMT modification/access times.
+  - A subfield with ID 0x7875 (Unix UID/GID (any size)) and 11 data bytes:
+    01 04 e3 3d 03 00 04 64 00 00 00.
+
   There is no file comment.
 
-Central directory entry #112:
+Central directory entry #125:
 ---------------------------
 
   torchtune/utils/seed.py
 
-  offset of local header from start of archive:   127894
-                                                  (000000000001F396h) bytes
+  offset of local header from start of archive:   157391
+                                                  (00000000000266CFh) bytes
   file system or operating system of origin:      Unix
-  version of encoding software:                   2.0
+  version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
-  compression sub-type (deflation):               normal
+  compression sub-type (deflation):               maximum
   file security status:                           not encrypted
   extended local header:                          no
-  file last modified on (DOS date/time):          2024 Mar 21 19:57:36
+  file last modified on (DOS date/time):          2024 Apr 16 01:12:14
+  file last modified on (UT extra field modtime): 2024 Apr 16 08:12:14 local
+  file last modified on (UT extra field modtime): 2024 Apr 16 08:12:14 UTC
   32-bit CRC value (hex):                         f4be2cf9
   compressed size:                                1345 bytes
   uncompressed size:                              3411 bytes
   length of filename:                             23 characters
-  length of extra field:                          0 bytes
+  length of extra field:                          24 bytes
   length of file comment:                         0 characters
   disk number on which file begins:               disk 1
-  apparent file type:                             binary
-  Unix file attributes (100664 octal):            -rw-rw-r--
+  apparent file type:                             text
+  Unix file attributes (100644 octal):            -rw-r--r--
   MS-DOS file attributes (00 hex):                none
 
+  The central-directory extra field contains:
+  - A subfield with ID 0x5455 (universal time) and 5 data bytes.
+    The local extra field has UTC/GMT modification/access times.
+  - A subfield with ID 0x7875 (Unix UID/GID (any size)) and 11 data bytes:
+    01 04 e3 3d 03 00 04 64 00 00 00.
+
   There is no file comment.
 
-Central directory entry #113:
+Central directory entry #126:
 ---------------------------
 
-  torchtune/utils/tensor_utils.py
+  torchtune/utils/_checkpointing/
 
-  offset of local header from start of archive:   129292
-                                                  (000000000001F90Ch) bytes
+  offset of local header from start of archive:   158817
+                                                  (0000000000026C61h) bytes
   file system or operating system of origin:      Unix
-  version of encoding software:                   2.0
+  version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
-  minimum software version required to extract:   2.0
-  compression method:                             deflated
-  compression sub-type (deflation):               normal
+  minimum software version required to extract:   1.0
+  compression method:                             none (stored)
   file security status:                           not encrypted
   extended local header:                          no
-  file last modified on (DOS date/time):          2024 Mar 21 19:57:36
-  32-bit CRC value (hex):                         f62dc2a1
-  compressed size:                                324 bytes
-  uncompressed size:                              585 bytes
+  file last modified on (DOS date/time):          2024 Apr 15 20:08:26
+  file last modified on (UT extra field modtime): 2024 Apr 16 03:08:26 local
+  file last modified on (UT extra field modtime): 2024 Apr 16 03:08:26 UTC
+  32-bit CRC value (hex):                         00000000
+  compressed size:                                0 bytes
+  uncompressed size:                              0 bytes
   length of filename:                             31 characters
-  length of extra field:                          0 bytes
+  length of extra field:                          24 bytes
   length of file comment:                         0 characters
   disk number on which file begins:               disk 1
   apparent file type:                             binary
-  Unix file attributes (100664 octal):            -rw-rw-r--
-  MS-DOS file attributes (00 hex):                none
+  Unix file attributes (040755 octal):            drwxr-xr-x
+  MS-DOS file attributes (10 hex):                dir 
+
+  The central-directory extra field contains:
+  - A subfield with ID 0x5455 (universal time) and 5 data bytes.
+    The local extra field has UTC/GMT modification/access times.
+  - A subfield with ID 0x7875 (Unix UID/GID (any size)) and 11 data bytes:
+    01 04 e3 3d 03 00 04 64 00 00 00.
 
   There is no file comment.
 
-Central directory entry #114:
+Central directory entry #127:
 ---------------------------
 
   torchtune/utils/_checkpointing/__init__.py
 
-  offset of local header from start of archive:   129677
-                                                  (000000000001FA8Dh) bytes
+  offset of local header from start of archive:   158906
+                                                  (0000000000026CBAh) bytes
   file system or operating system of origin:      Unix
-  version of encoding software:                   2.0
+  version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
-  compression sub-type (deflation):               normal
+  compression sub-type (deflation):               maximum
   file security status:                           not encrypted
   extended local header:                          no
-  file last modified on (DOS date/time):          2024 Mar 21 19:57:36
-  32-bit CRC value (hex):                         8ac12e5e
-  compressed size:                                226 bytes
-  uncompressed size:                              395 bytes
+  file last modified on (DOS date/time):          2024 Apr 16 01:12:14
+  file last modified on (UT extra field modtime): 2024 Apr 16 08:12:14 local
+  file last modified on (UT extra field modtime): 2024 Apr 16 08:12:14 UTC
+  32-bit CRC value (hex):                         e1602d32
+  compressed size:                                242 bytes
+  uncompressed size:                              421 bytes
   length of filename:                             42 characters
-  length of extra field:                          0 bytes
+  length of extra field:                          24 bytes
   length of file comment:                         0 characters
   disk number on which file begins:               disk 1
-  apparent file type:                             binary
-  Unix file attributes (100664 octal):            -rw-rw-r--
+  apparent file type:                             text
+  Unix file attributes (100644 octal):            -rw-r--r--
   MS-DOS file attributes (00 hex):                none
 
+  The central-directory extra field contains:
+  - A subfield with ID 0x5455 (universal time) and 5 data bytes.
+    The local extra field has UTC/GMT modification/access times.
+  - A subfield with ID 0x7875 (Unix UID/GID (any size)) and 11 data bytes:
+    01 04 e3 3d 03 00 04 64 00 00 00.
+
   There is no file comment.
 
-Central directory entry #115:
+Central directory entry #128:
 ---------------------------
 
   torchtune/utils/_checkpointing/_checkpointer.py
 
-  offset of local header from start of archive:   129975
-                                                  (000000000001FBB7h) bytes
+  offset of local header from start of archive:   159248
+                                                  (0000000000026E10h) bytes
   file system or operating system of origin:      Unix
-  version of encoding software:                   2.0
+  version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
-  compression sub-type (deflation):               normal
+  compression sub-type (deflation):               maximum
   file security status:                           not encrypted
   extended local header:                          no
-  file last modified on (DOS date/time):          2024 Mar 21 19:57:36
-  32-bit CRC value (hex):                         9f32e86c
-  compressed size:                                4772 bytes
-  uncompressed size:                              26065 bytes
+  file last modified on (DOS date/time):          2024 Apr 16 01:12:14
+  file last modified on (UT extra field modtime): 2024 Apr 16 08:12:14 local
+  file last modified on (UT extra field modtime): 2024 Apr 16 08:12:14 UTC
+  32-bit CRC value (hex):                         98220525
+  compressed size:                                5003 bytes
+  uncompressed size:                              26322 bytes
   length of filename:                             47 characters
-  length of extra field:                          0 bytes
+  length of extra field:                          24 bytes
   length of file comment:                         0 characters
   disk number on which file begins:               disk 1
-  apparent file type:                             binary
-  Unix file attributes (100664 octal):            -rw-rw-r--
+  apparent file type:                             text
+  Unix file attributes (100644 octal):            -rw-r--r--
   MS-DOS file attributes (00 hex):                none
 
+  The central-directory extra field contains:
+  - A subfield with ID 0x5455 (universal time) and 5 data bytes.
+    The local extra field has UTC/GMT modification/access times.
+  - A subfield with ID 0x7875 (Unix UID/GID (any size)) and 11 data bytes:
+    01 04 e3 3d 03 00 04 64 00 00 00.
+
   There is no file comment.
 
-Central directory entry #116:
+Central directory entry #129:
 ---------------------------
 
   torchtune/utils/_checkpointing/_checkpointer_utils.py
 
-  offset of local header from start of archive:   134824
-                                                  (0000000000020EA8h) bytes
+  offset of local header from start of archive:   164356
+                                                  (0000000000028204h) bytes
   file system or operating system of origin:      Unix
-  version of encoding software:                   2.0
+  version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
-  compression sub-type (deflation):               normal
+  compression sub-type (deflation):               maximum
   file security status:                           not encrypted
   extended local header:                          no
-  file last modified on (DOS date/time):          2024 Mar 21 19:57:36
-  32-bit CRC value (hex):                         35ae77a3
-  compressed size:                                768 bytes
-  uncompressed size:                              1726 bytes
+  file last modified on (DOS date/time):          2024 Apr 16 01:12:14
+  file last modified on (UT extra field modtime): 2024 Apr 16 08:12:14 local
+  file last modified on (UT extra field modtime): 2024 Apr 16 08:12:14 UTC
+  32-bit CRC value (hex):                         8c32a2d2
+  compressed size:                                1420 bytes
+  uncompressed size:                              3861 bytes
   length of filename:                             53 characters
-  length of extra field:                          0 bytes
+  length of extra field:                          24 bytes
   length of file comment:                         0 characters
   disk number on which file begins:               disk 1
-  apparent file type:                             binary
-  Unix file attributes (100664 octal):            -rw-rw-r--
+  apparent file type:                             text
+  Unix file attributes (100644 octal):            -rw-r--r--
   MS-DOS file attributes (00 hex):                none
 
+  The central-directory extra field contains:
+  - A subfield with ID 0x5455 (universal time) and 5 data bytes.
+    The local extra field has UTC/GMT modification/access times.
+  - A subfield with ID 0x7875 (Unix UID/GID (any size)) and 11 data bytes:
+    01 04 e3 3d 03 00 04 64 00 00 00.
+
   There is no file comment.
 
-Central directory entry #117:
+Central directory entry #130:
+---------------------------
+
+  torchtune-0.1.0.dist-info/
+
+  offset of local header from start of archive:   165887
+                                                  (00000000000287FFh) bytes
+  file system or operating system of origin:      Unix
+  version of encoding software:                   3.0
+  minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
+  minimum software version required to extract:   1.0
+  compression method:                             none (stored)
+  file security status:                           not encrypted
+  extended local header:                          no
+  file last modified on (DOS date/time):          2024 Apr 15 20:08:26
+  file last modified on (UT extra field modtime): 2024 Apr 16 03:08:26 local
+  file last modified on (UT extra field modtime): 2024 Apr 16 03:08:26 UTC
+  32-bit CRC value (hex):                         00000000
+  compressed size:                                0 bytes
+  uncompressed size:                              0 bytes
+  length of filename:                             26 characters
+  length of extra field:                          24 bytes
+  length of file comment:                         0 characters
+  disk number on which file begins:               disk 1
+  apparent file type:                             binary
+  Unix file attributes (040755 octal):            drwxr-xr-x
+  MS-DOS file attributes (10 hex):                dir 
+
+  The central-directory extra field contains:
+  - A subfield with ID 0x5455 (universal time) and 5 data bytes.
+    The local extra field has UTC/GMT modification/access times.
+  - A subfield with ID 0x7875 (Unix UID/GID (any size)) and 11 data bytes:
+    01 04 e3 3d 03 00 04 64 00 00 00.
+
+  There is no file comment.
+
+Central directory entry #131:
 ---------------------------
 
-  torchtune-0.0.1.dist-info/LICENSE
+  torchtune-0.1.0.dist-info/LICENSE
 
-  offset of local header from start of archive:   135675
-                                                  (00000000000211FBh) bytes
+  offset of local header from start of archive:   165971
+                                                  (0000000000028853h) bytes
   file system or operating system of origin:      Unix
-  version of encoding software:                   2.0
+  version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
-  compression sub-type (deflation):               normal
+  compression sub-type (deflation):               maximum
   file security status:                           not encrypted
   extended local header:                          no
-  file last modified on (DOS date/time):          2024 Mar 21 20:03:14
+  file last modified on (DOS date/time):          2024 Apr 15 20:08:26
+  file last modified on (UT extra field modtime): 2024 Apr 16 03:08:26 local
+  file last modified on (UT extra field modtime): 2024 Apr 16 03:08:26 UTC
   32-bit CRC value (hex):                         17d7526d
   compressed size:                                786 bytes
   uncompressed size:                              1474 bytes
   length of filename:                             33 characters
-  length of extra field:                          0 bytes
+  length of extra field:                          24 bytes
   length of file comment:                         0 characters
   disk number on which file begins:               disk 1
-  apparent file type:                             binary
-  Unix file attributes (100664 octal):            -rw-rw-r--
+  apparent file type:                             text
+  Unix file attributes (100644 octal):            -rw-r--r--
   MS-DOS file attributes (00 hex):                none
 
+  The central-directory extra field contains:
+  - A subfield with ID 0x5455 (universal time) and 5 data bytes.
+    The local extra field has UTC/GMT modification/access times.
+  - A subfield with ID 0x7875 (Unix UID/GID (any size)) and 11 data bytes:
+    01 04 e3 3d 03 00 04 64 00 00 00.
+
   There is no file comment.
 
-Central directory entry #118:
+Central directory entry #132:
 ---------------------------
 
-  torchtune-0.0.1.dist-info/METADATA
+  torchtune-0.1.0.dist-info/METADATA
 
-  offset of local header from start of archive:   136524
-                                                  (000000000002154Ch) bytes
+  offset of local header from start of archive:   166848
+                                                  (0000000000028BC0h) bytes
   file system or operating system of origin:      Unix
-  version of encoding software:                   2.0
+  version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
-  compression sub-type (deflation):               normal
+  compression sub-type (deflation):               maximum
   file security status:                           not encrypted
   extended local header:                          no
-  file last modified on (DOS date/time):          2024 Mar 21 20:03:14
-  32-bit CRC value (hex):                         976bf118
-  compressed size:                                3824 bytes
-  uncompressed size:                              10767 bytes
+  file last modified on (DOS date/time):          2024 Apr 15 20:08:26
+  file last modified on (UT extra field modtime): 2024 Apr 16 03:08:26 local
+  file last modified on (UT extra field modtime): 2024 Apr 16 03:08:26 UTC
+  32-bit CRC value (hex):                         73856efb
+  compressed size:                                5598 bytes
+  uncompressed size:                              14827 bytes
   length of filename:                             34 characters
-  length of extra field:                          0 bytes
+  length of extra field:                          24 bytes
   length of file comment:                         0 characters
   disk number on which file begins:               disk 1
-  apparent file type:                             binary
-  Unix file attributes (100664 octal):            -rw-rw-r--
+  apparent file type:                             text
+  Unix file attributes (100644 octal):            -rw-r--r--
   MS-DOS file attributes (00 hex):                none
 
+  The central-directory extra field contains:
+  - A subfield with ID 0x5455 (universal time) and 5 data bytes.
+    The local extra field has UTC/GMT modification/access times.
+  - A subfield with ID 0x7875 (Unix UID/GID (any size)) and 11 data bytes:
+    01 04 e3 3d 03 00 04 64 00 00 00.
+
   There is no file comment.
 
-Central directory entry #119:
+Central directory entry #133:
 ---------------------------
 
-  torchtune-0.0.1.dist-info/WHEEL
+  torchtune-0.1.0.dist-info/WHEEL
 
-  offset of local header from start of archive:   140412
-                                                  (000000000002247Ch) bytes
+  offset of local header from start of archive:   172538
+                                                  (000000000002A1FAh) bytes
   file system or operating system of origin:      Unix
-  version of encoding software:                   2.0
+  version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
-  minimum software version required to extract:   2.0
-  compression method:                             deflated
-  compression sub-type (deflation):               normal
+  minimum software version required to extract:   1.0
+  compression method:                             none (stored)
   file security status:                           not encrypted
   extended local header:                          no
-  file last modified on (DOS date/time):          2024 Mar 21 20:03:14
-  32-bit CRC value (hex):                         e0b8491e
+  file last modified on (DOS date/time):          2024 Apr 15 20:08:26
+  file last modified on (UT extra field modtime): 2024 Apr 16 03:08:26 local
+  file last modified on (UT extra field modtime): 2024 Apr 16 03:08:26 UTC
+  32-bit CRC value (hex):                         4b7b0efc
   compressed size:                                92 bytes
   uncompressed size:                              92 bytes
   length of filename:                             31 characters
-  length of extra field:                          0 bytes
+  length of extra field:                          24 bytes
   length of file comment:                         0 characters
   disk number on which file begins:               disk 1
-  apparent file type:                             binary
-  Unix file attributes (100664 octal):            -rw-rw-r--
+  apparent file type:                             text
+  Unix file attributes (100644 octal):            -rw-r--r--
   MS-DOS file attributes (00 hex):                none
 
+  The central-directory extra field contains:
+  - A subfield with ID 0x5455 (universal time) and 5 data bytes.
+    The local extra field has UTC/GMT modification/access times.
+  - A subfield with ID 0x7875 (Unix UID/GID (any size)) and 11 data bytes:
+    01 04 e3 3d 03 00 04 64 00 00 00.
+
   There is no file comment.
 
-Central directory entry #120:
+Central directory entry #134:
 ---------------------------
 
-  torchtune-0.0.1.dist-info/entry_points.txt
+  torchtune-0.1.0.dist-info/entry_points.txt
 
-  offset of local header from start of archive:   140565
-                                                  (0000000000022515h) bytes
+  offset of local header from start of archive:   172719
+                                                  (000000000002A2AFh) bytes
   file system or operating system of origin:      Unix
-  version of encoding software:                   2.0
+  version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
-  compression sub-type (deflation):               normal
+  compression sub-type (deflation):               maximum
   file security status:                           not encrypted
   extended local header:                          no
-  file last modified on (DOS date/time):          2024 Mar 21 20:03:14
+  file last modified on (DOS date/time):          2024 Apr 15 20:08:26
+  file last modified on (UT extra field modtime): 2024 Apr 16 03:08:26 local
+  file last modified on (UT extra field modtime): 2024 Apr 16 03:08:26 UTC
   32-bit CRC value (hex):                         4758c813
   compressed size:                                47 bytes
   uncompressed size:                              50 bytes
   length of filename:                             42 characters
-  length of extra field:                          0 bytes
+  length of extra field:                          24 bytes
   length of file comment:                         0 characters
   disk number on which file begins:               disk 1
-  apparent file type:                             binary
-  Unix file attributes (100664 octal):            -rw-rw-r--
+  apparent file type:                             text
+  Unix file attributes (100644 octal):            -rw-r--r--
   MS-DOS file attributes (00 hex):                none
 
+  The central-directory extra field contains:
+  - A subfield with ID 0x5455 (universal time) and 5 data bytes.
+    The local extra field has UTC/GMT modification/access times.
+  - A subfield with ID 0x7875 (Unix UID/GID (any size)) and 11 data bytes:
+    01 04 e3 3d 03 00 04 64 00 00 00.
+
   There is no file comment.
 
-Central directory entry #121:
+Central directory entry #135:
 ---------------------------
 
-  torchtune-0.0.1.dist-info/top_level.txt
+  torchtune-0.1.0.dist-info/top_level.txt
 
-  offset of local header from start of archive:   140684
-                                                  (000000000002258Ch) bytes
+  offset of local header from start of archive:   172866
+                                                  (000000000002A342h) bytes
   file system or operating system of origin:      Unix
-  version of encoding software:                   2.0
+  version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
-  minimum software version required to extract:   2.0
-  compression method:                             deflated
-  compression sub-type (deflation):               normal
+  minimum software version required to extract:   1.0
+  compression method:                             none (stored)
   file security status:                           not encrypted
   extended local header:                          no
-  file last modified on (DOS date/time):          2024 Mar 21 20:03:14
-  32-bit CRC value (hex):                         ed3c64ed
+  file last modified on (DOS date/time):          2024 Apr 15 20:08:26
+  file last modified on (UT extra field modtime): 2024 Apr 16 03:08:26 local
+  file last modified on (UT extra field modtime): 2024 Apr 16 03:08:26 UTC
+  32-bit CRC value (hex):                         66b09137
   compressed size:                                18 bytes
-  uncompressed size:                              16 bytes
+  uncompressed size:                              18 bytes
   length of filename:                             39 characters
-  length of extra field:                          0 bytes
+  length of extra field:                          24 bytes
   length of file comment:                         0 characters
   disk number on which file begins:               disk 1
-  apparent file type:                             binary
-  Unix file attributes (100664 octal):            -rw-rw-r--
+  apparent file type:                             text
+  Unix file attributes (100644 octal):            -rw-r--r--
   MS-DOS file attributes (00 hex):                none
 
+  The central-directory extra field contains:
+  - A subfield with ID 0x5455 (universal time) and 5 data bytes.
+    The local extra field has UTC/GMT modification/access times.
+  - A subfield with ID 0x7875 (Unix UID/GID (any size)) and 11 data bytes:
+    01 04 e3 3d 03 00 04 64 00 00 00.
+
   There is no file comment.
 
-Central directory entry #122:
+Central directory entry #136:
 ---------------------------
 
-  torchtune-0.0.1.dist-info/RECORD
+  torchtune-0.1.0.dist-info/RECORD
 
-  offset of local header from start of archive:   140771
-                                                  (00000000000225E3h) bytes
+  offset of local header from start of archive:   172981
+                                                  (000000000002A3B5h) bytes
   file system or operating system of origin:      Unix
-  version of encoding software:                   2.0
+  version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
-  compression sub-type (deflation):               normal
+  compression sub-type (deflation):               maximum
   file security status:                           not encrypted
   extended local header:                          no
-  file last modified on (DOS date/time):          2024 Mar 21 20:03:14
-  32-bit CRC value (hex):                         3aeb6d9f
-  compressed size:                                5157 bytes
-  uncompressed size:                              11070 bytes
+  file last modified on (DOS date/time):          2024 Apr 15 20:08:28
+  file last modified on (UT extra field modtime): 2024 Apr 16 03:08:28 local
+  file last modified on (UT extra field modtime): 2024 Apr 16 03:08:28 UTC
+  32-bit CRC value (hex):                         42fab17f
+  compressed size:                                5259 bytes
+  uncompressed size:                              10283 bytes
   length of filename:                             32 characters
-  length of extra field:                          0 bytes
+  length of extra field:                          24 bytes
   length of file comment:                         0 characters
   disk number on which file begins:               disk 1
-  apparent file type:                             binary
+  apparent file type:                             text
   Unix file attributes (100664 octal):            -rw-rw-r--
   MS-DOS file attributes (00 hex):                none
 
+  The central-directory extra field contains:
+  - A subfield with ID 0x5455 (universal time) and 5 data bytes.
+    The local extra field has UTC/GMT modification/access times.
+  - A subfield with ID 0x7875 (Unix UID/GID (any size)) and 11 data bytes:
+    01 04 e3 3d 03 00 04 64 00 00 00.
+
   There is no file comment.
```

## zipnote {}

```diff
@@ -1,262 +1,289 @@
-Filename: tests/__init__.py
+Filename: recipes/
 Comment: 
 
-Filename: tests/common.py
+Filename: recipes/__init__.py
 Comment: 
 
-Filename: tests/conftest.py
+Filename: recipes/eleuther_eval.py
 Comment: 
 
-Filename: tests/test_utils.py
+Filename: recipes/full_finetune_distributed.py
 Comment: 
 
-Filename: tests/recipes/__init__.py
+Filename: recipes/full_finetune_single_device.py
 Comment: 
 
-Filename: tests/recipes/common.py
+Filename: recipes/generate.py
 Comment: 
 
-Filename: tests/recipes/test_alpaca_generate.py
+Filename: recipes/lora_dpo_single_device.py
 Comment: 
 
-Filename: tests/recipes/test_configs.py
+Filename: recipes/lora_finetune_distributed.py
 Comment: 
 
-Filename: tests/recipes/test_full_finetune.py
+Filename: recipes/lora_finetune_single_device.py
 Comment: 
 
-Filename: tests/recipes/test_lora_finetune.py
+Filename: recipes/quantize.py
 Comment: 
 
-Filename: tests/recipes/utils.py
+Filename: recipes/configs/
 Comment: 
 
-Filename: tests/torchtune/__init__.py
+Filename: recipes/configs/eleuther_evaluation.yaml
 Comment: 
 
-Filename: tests/torchtune/_cli/__init__.py
+Filename: recipes/configs/generation.yaml
 Comment: 
 
-Filename: tests/torchtune/_cli/test_convert_checkpoint.py
+Filename: recipes/configs/quantization.yaml
 Comment: 
 
-Filename: tests/torchtune/_cli/test_cp.py
+Filename: recipes/configs/gemma/
 Comment: 
 
-Filename: tests/torchtune/_cli/test_download.py
+Filename: recipes/configs/gemma/2B_full.yaml
 Comment: 
 
-Filename: tests/torchtune/_cli/test_ls.py
+Filename: recipes/configs/llama2/
 Comment: 
 
-Filename: tests/torchtune/_cli/test_tune.py
+Filename: recipes/configs/llama2/13B_full.yaml
 Comment: 
 
-Filename: tests/torchtune/_cli/test_validate.py
+Filename: recipes/configs/llama2/13B_lora.yaml
 Comment: 
 
-Filename: tests/torchtune/datasets/__init__.py
+Filename: recipes/configs/llama2/7B_full.yaml
 Comment: 
 
-Filename: tests/torchtune/datasets/test_alpaca_dataset.py
+Filename: recipes/configs/llama2/7B_full_low_memory.yaml
 Comment: 
 
-Filename: tests/torchtune/datasets/test_instruct_dataset.py
+Filename: recipes/configs/llama2/7B_lora.yaml
 Comment: 
 
-Filename: tests/torchtune/datasets/test_slimorca_dataset.py
+Filename: recipes/configs/llama2/7B_lora_dpo_single_device.yaml
 Comment: 
 
-Filename: tests/torchtune/generation/__init__.py
+Filename: recipes/configs/llama2/7B_lora_single_device.yaml
 Comment: 
 
-Filename: tests/torchtune/generation/test_generation.py
+Filename: recipes/configs/llama2/7B_qlora_single_device.yaml
 Comment: 
 
-Filename: tests/torchtune/models/__init__.py
+Filename: recipes/configs/mistral/
 Comment: 
 
-Filename: tests/torchtune/models/test_lora_llama2.py
+Filename: recipes/configs/mistral/7B_full.yaml
 Comment: 
 
-Filename: tests/torchtune/modules/__init__.py
+Filename: recipes/configs/mistral/7B_full_low_memory.yaml
 Comment: 
 
-Filename: tests/torchtune/modules/test_attention.py
+Filename: recipes/configs/mistral/7B_lora.yaml
 Comment: 
 
-Filename: tests/torchtune/modules/test_cosine_with_warmup.py
+Filename: recipes/configs/mistral/7B_lora_single_device.yaml
 Comment: 
 
-Filename: tests/torchtune/modules/test_feed_forward.py
+Filename: recipes/configs/mistral/7B_qlora_single_device.yaml
 Comment: 
 
-Filename: tests/torchtune/modules/test_position_embeddings.py
+Filename: torchtune/
 Comment: 
 
-Filename: tests/torchtune/modules/test_rms_norm.py
+Filename: torchtune/__init__.py
 Comment: 
 
-Filename: tests/torchtune/modules/test_tokenizer.py
+Filename: torchtune/_recipe_registry.py
 Comment: 
 
-Filename: tests/torchtune/modules/test_transformer_decoder.py
+Filename: torchtune/recipe_interfaces.py
 Comment: 
 
-Filename: tests/torchtune/modules/low_precision/__init__.py
+Filename: torchtune/_cli/
 Comment: 
 
-Filename: tests/torchtune/modules/low_precision/test_nf4_linear.py
+Filename: torchtune/_cli/__init__.py
 Comment: 
 
-Filename: tests/torchtune/modules/peft/__init__.py
+Filename: torchtune/_cli/cp.py
 Comment: 
 
-Filename: tests/torchtune/modules/peft/test_lora.py
+Filename: torchtune/_cli/download.py
 Comment: 
 
-Filename: tests/torchtune/modules/peft/test_peft_utils.py
+Filename: torchtune/_cli/ls.py
 Comment: 
 
-Filename: tests/torchtune/utils/__init__.py
+Filename: torchtune/_cli/run.py
 Comment: 
 
-Filename: tests/torchtune/utils/test_argparse.py
+Filename: torchtune/_cli/subcommand.py
 Comment: 
 
-Filename: tests/torchtune/utils/test_checkpoint.py
+Filename: torchtune/_cli/tune.py
 Comment: 
 
-Filename: tests/torchtune/utils/test_checkpointable_dataloader.py
+Filename: torchtune/_cli/validate.py
 Comment: 
 
-Filename: tests/torchtune/utils/test_checkpointer.py
+Filename: torchtune/_cli/hf_upload/
 Comment: 
 
-Filename: tests/torchtune/utils/test_collate.py
+Filename: torchtune/_cli/hf_upload/upload.py
 Comment: 
 
-Filename: tests/torchtune/utils/test_device.py
+Filename: torchtune/config/
 Comment: 
 
-Filename: tests/torchtune/utils/test_distributed.py
+Filename: torchtune/config/__init__.py
 Comment: 
 
-Filename: tests/torchtune/utils/test_logits_transforms.py
+Filename: torchtune/config/_errors.py
 Comment: 
 
-Filename: tests/torchtune/utils/test_metric_logging.py
+Filename: torchtune/config/_instantiate.py
 Comment: 
 
-Filename: tests/torchtune/utils/test_precision.py
+Filename: torchtune/config/_parse.py
 Comment: 
 
-Filename: tests/torchtune/utils/test_seed.py
+Filename: torchtune/config/_utils.py
 Comment: 
 
-Filename: tests/torchtune/utils/test_tensor_utils.py
+Filename: torchtune/config/_validate.py
 Comment: 
 
-Filename: torchtune/__init__.py
+Filename: torchtune/data/
 Comment: 
 
-Filename: torchtune/recipe_interfaces.py
+Filename: torchtune/data/__init__.py
 Comment: 
 
-Filename: torchtune/_cli/__init__.py
+Filename: torchtune/data/_chat_formats.py
 Comment: 
 
-Filename: torchtune/_cli/convert_checkpoint.py
+Filename: torchtune/data/_common.py
 Comment: 
 
-Filename: torchtune/_cli/cp.py
+Filename: torchtune/data/_converters.py
 Comment: 
 
-Filename: torchtune/_cli/download.py
+Filename: torchtune/data/_instruct_templates.py
 Comment: 
 
-Filename: torchtune/_cli/eval.py
+Filename: torchtune/data/_types.py
 Comment: 
 
-Filename: torchtune/_cli/ls.py
+Filename: torchtune/data/_utils.py
 Comment: 
 
-Filename: torchtune/_cli/tune.py
+Filename: torchtune/datasets/
 Comment: 
 
-Filename: torchtune/_cli/validate.py
+Filename: torchtune/datasets/__init__.py
 Comment: 
 
-Filename: torchtune/config/__init__.py
+Filename: torchtune/datasets/_alpaca.py
 Comment: 
 
-Filename: torchtune/config/_errors.py
+Filename: torchtune/datasets/_chat.py
 Comment: 
 
-Filename: torchtune/config/_instantiate.py
+Filename: torchtune/datasets/_grammar.py
 Comment: 
 
-Filename: torchtune/config/_parse.py
+Filename: torchtune/datasets/_instruct.py
 Comment: 
 
-Filename: torchtune/config/_utils.py
+Filename: torchtune/datasets/_preference.py
 Comment: 
 
-Filename: torchtune/config/_validate.py
+Filename: torchtune/datasets/_samsum.py
 Comment: 
 
-Filename: torchtune/data/__init__.py
+Filename: torchtune/datasets/_slimorca.py
 Comment: 
 
-Filename: torchtune/data/_templates.py
+Filename: torchtune/datasets/_stack_exchanged_paired.py
 Comment: 
 
-Filename: torchtune/datasets/__init__.py
+Filename: torchtune/models/
 Comment: 
 
-Filename: torchtune/datasets/_alpaca.py
+Filename: torchtune/models/__init__.py
 Comment: 
 
-Filename: torchtune/datasets/_common.py
+Filename: torchtune/models/convert_weights.py
 Comment: 
 
-Filename: torchtune/datasets/_instruct.py
+Filename: torchtune/models/gemma/
 Comment: 
 
-Filename: torchtune/datasets/_slimorca.py
+Filename: torchtune/models/gemma/__init__.py
 Comment: 
 
-Filename: torchtune/models/__init__.py
+Filename: torchtune/models/gemma/_component_builders.py
+Comment: 
+
+Filename: torchtune/models/gemma/_model_builders.py
+Comment: 
+
+Filename: torchtune/models/gemma/rms_norm.py
+Comment: 
+
+Filename: torchtune/models/gemma/transformer.py
+Comment: 
+
+Filename: torchtune/models/llama2/
 Comment: 
 
 Filename: torchtune/models/llama2/__init__.py
 Comment: 
 
 Filename: torchtune/models/llama2/_checkpoint_utils.py
 Comment: 
 
 Filename: torchtune/models/llama2/_component_builders.py
 Comment: 
 
-Filename: torchtune/models/llama2/_convert_weights.py
-Comment: 
-
 Filename: torchtune/models/llama2/_model_builders.py
 Comment: 
 
 Filename: torchtune/models/llama2/_model_utils.py
 Comment: 
 
+Filename: torchtune/models/mistral/
+Comment: 
+
+Filename: torchtune/models/mistral/__init__.py
+Comment: 
+
+Filename: torchtune/models/mistral/_component_builders.py
+Comment: 
+
+Filename: torchtune/models/mistral/_model_builders.py
+Comment: 
+
+Filename: torchtune/modules/
+Comment: 
+
 Filename: torchtune/modules/__init__.py
 Comment: 
 
 Filename: torchtune/modules/attention.py
 Comment: 
 
+Filename: torchtune/modules/common_utils.py
+Comment: 
+
 Filename: torchtune/modules/feed_forward.py
 Comment: 
 
 Filename: torchtune/modules/kv_cache.py
 Comment: 
 
 Filename: torchtune/modules/lr_schedulers.py
@@ -270,98 +297,113 @@
 
 Filename: torchtune/modules/tokenizer.py
 Comment: 
 
 Filename: torchtune/modules/transformer.py
 Comment: 
 
-Filename: torchtune/modules/low_precision/__init__.py
+Filename: torchtune/modules/loss/
 Comment: 
 
-Filename: torchtune/modules/low_precision/nf4_linear.py
+Filename: torchtune/modules/loss/__init__.py
+Comment: 
+
+Filename: torchtune/modules/loss/dpo.py
+Comment: 
+
+Filename: torchtune/modules/peft/
 Comment: 
 
 Filename: torchtune/modules/peft/__init__.py
 Comment: 
 
 Filename: torchtune/modules/peft/lora.py
 Comment: 
 
 Filename: torchtune/modules/peft/peft_utils.py
 Comment: 
 
+Filename: torchtune/utils/
+Comment: 
+
 Filename: torchtune/utils/__init__.py
 Comment: 
 
+Filename: torchtune/utils/_compile_utils.py
+Comment: 
+
 Filename: torchtune/utils/_device.py
 Comment: 
 
 Filename: torchtune/utils/_distributed.py
 Comment: 
 
-Filename: torchtune/utils/argparse.py
+Filename: torchtune/utils/_generation.py
 Comment: 
 
-Filename: torchtune/utils/checkpoint.py
+Filename: torchtune/utils/_profiler.py
 Comment: 
 
-Filename: torchtune/utils/checkpointable_dataloader.py
+Filename: torchtune/utils/_register_nf4_dispatch_ops.py
 Comment: 
 
-Filename: torchtune/utils/collate.py
+Filename: torchtune/utils/argparse.py
 Comment: 
 
-Filename: torchtune/utils/constants.py
+Filename: torchtune/utils/collate.py
 Comment: 
 
-Filename: torchtune/utils/generation.py
+Filename: torchtune/utils/constants.py
 Comment: 
 
 Filename: torchtune/utils/logging.py
 Comment: 
 
-Filename: torchtune/utils/logits_transforms.py
-Comment: 
-
 Filename: torchtune/utils/memory.py
 Comment: 
 
 Filename: torchtune/utils/metric_logging.py
 Comment: 
 
 Filename: torchtune/utils/precision.py
 Comment: 
 
+Filename: torchtune/utils/quantization.py
+Comment: 
+
 Filename: torchtune/utils/seed.py
 Comment: 
 
-Filename: torchtune/utils/tensor_utils.py
+Filename: torchtune/utils/_checkpointing/
 Comment: 
 
 Filename: torchtune/utils/_checkpointing/__init__.py
 Comment: 
 
 Filename: torchtune/utils/_checkpointing/_checkpointer.py
 Comment: 
 
 Filename: torchtune/utils/_checkpointing/_checkpointer_utils.py
 Comment: 
 
-Filename: torchtune-0.0.1.dist-info/LICENSE
+Filename: torchtune-0.1.0.dist-info/
+Comment: 
+
+Filename: torchtune-0.1.0.dist-info/LICENSE
 Comment: 
 
-Filename: torchtune-0.0.1.dist-info/METADATA
+Filename: torchtune-0.1.0.dist-info/METADATA
 Comment: 
 
-Filename: torchtune-0.0.1.dist-info/WHEEL
+Filename: torchtune-0.1.0.dist-info/WHEEL
 Comment: 
 
-Filename: torchtune-0.0.1.dist-info/entry_points.txt
+Filename: torchtune-0.1.0.dist-info/entry_points.txt
 Comment: 
 
-Filename: torchtune-0.0.1.dist-info/top_level.txt
+Filename: torchtune-0.1.0.dist-info/top_level.txt
 Comment: 
 
-Filename: torchtune-0.0.1.dist-info/RECORD
+Filename: torchtune-0.1.0.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## filetype from file(1)

```diff
@@ -1 +1 @@
-Zip archive data, at least v2.0 to extract, compression method=deflate
+Zip archive data, at least v1.0 to extract, compression method=store
```

## torchtune/__init__.py

```diff
@@ -1,37 +1,11 @@
 # Copyright (c) Meta Platforms, Inc. and affiliates.
 # All rights reserved.
 #
 # This source code is licensed under the BSD-style license found in the
 # LICENSE file in the root directory of this source tree.
 
-from torchtune import datasets, models, modules, utils
-
-_RECIPE_LIST = [
-    "full_finetune_single_device.py",
-    "full_finetune_distributed.py",
-    "alpaca_generate.py",
-    "lora_finetune_single_device.py",
-    "lora_finetune_distributed.py",
-]
-_CONFIG_LISTS = {
-    "full_finetune_single_device.py": ["full_finetune_single_device.yaml"],
-    "full_finetune_distributed.py": ["full_finetune_distributed.yaml"],
-    "lora_finetune_single_device.py": ["lora_finetune_single_device.yaml"],
-    "lora_finetune_distributed.py": ["lora_finetune_distributed.yaml"],
-    "alpaca_generate.py": ["alpaca_generate.yaml"],
-}
-
-
-def list_recipes():
-    """List of recipes available from the CLI"""
-    return _RECIPE_LIST
-
-
-def list_configs(recipe: str):
-    """List of configs available from the CLI given a recipe"""
-    if recipe not in _CONFIG_LISTS:
-        raise ValueError(f"Unknown recipe: {recipe}")
-    return _CONFIG_LISTS[recipe]
+__version__ = '0.1.0+cpu'
 
+from torchtune import datasets, models, modules, utils
 
 __all__ = [datasets, models, modules, utils]
```

## torchtune/recipe_interfaces.py

```diff
@@ -54,7 +54,34 @@
         ...
 
     def cleanup(self, **kwargs) -> None:
         """
         Any cleaning up needed for the recipe.
         """
         ...
+
+
+class EvalRecipeInterface(Protocol):
+    """
+    This class provides a loose structure which every LLM evaluation recipe
+    should follow. Please note that the interface itself should not be a vehicle for
+    code reuse. TorchTune strictly prohibits implementation inheritance in the codebase.
+    """
+
+    def load_checkpoint(self, **kwargs) -> None:
+        """
+        Responsible for loading ALL of the state for the recipe from the
+        checkpoint file.
+        """
+        ...
+
+    def setup(self, **kwargs) -> None:
+        """
+        Responsible for setting up all of the components necessary for evaluation.
+        """
+        ...
+
+    def evaluate(self, **kwargs) -> None:
+        """
+        All of the evaluation logic, including reporting.
+        """
+        ...
```

## torchtune/_cli/__init__.py

```diff
@@ -1,12 +1,5 @@
 # Copyright (c) Meta Platforms, Inc. and affiliates.
 # All rights reserved.
 #
 # This source code is licensed under the BSD-style license found in the
 # LICENSE file in the root directory of this source tree.
-
-_SCRIPTS = ["download", "convert_checkpoint", "ls", "cp", "eval", "validate"]
-
-
-def list_scripts():
-    """List of available scripts."""
-    return _SCRIPTS
```

## torchtune/_cli/cp.py

```diff
@@ -1,103 +1,116 @@
 # Copyright (c) Meta Platforms, Inc. and affiliates.
 # All rights reserved.
 #
 # This source code is licensed under the BSD-style license found in the
 # LICENSE file in the root directory of this source tree.
-
-"""This script copies a built-in recipe or config to a local path."""
 import argparse
 import shutil
 import textwrap
 from pathlib import Path
 
 import torchtune
-from torchtune import list_configs, list_recipes
+from torchtune._cli.subcommand import Subcommand
+from torchtune._recipe_registry import get_all_recipes
 
+ROOT = Path(torchtune.__file__).parent.parent
 
-def _get_absolute_path(file_name: str) -> Path:
-    pkg_path = Path(torchtune.__file__).parent.parent.absolute()
-    recipes_path = pkg_path / "recipes"
-    if file_name.endswith(".yaml"):
-        path = recipes_path / "configs" / file_name
-    else:
-        assert file_name.endswith(".py"), f"Expected .py file, got {file_name}"
-        path = recipes_path / file_name
-    return path
-
-
-def main(parser):
-    args = parser.parse_args()
-    destination = args.destination
-
-    # Check if recipe/config is valid
-    all_recipes_and_configs = list_recipes() + [
-        config for recipe in list_recipes() for config in list_configs(recipe)
-    ]
-    if args.file not in all_recipes_and_configs:
-        parser.error(
-            f"Invalid file name: {args.file}. Try `tune ls` to see all available files to copy."
-        )
 
-    # Get file path
-    file_name = args.file
-    src = _get_absolute_path(file_name)
-
-    # Copy file
-    try:
-        if args.no_clobber and destination.exists():
-            print(f"File already exists at {destination.absolute()}, not overwriting.")
-        else:
-            if args.make_parents:
-                destination.parent.mkdir(parents=True, exist_ok=True)
-            shutil.copy(src, destination)
-    except FileNotFoundError:
-        parser.error(
-            f"Cannot create regular file: '{destination}'. No such file or directory. "
-            "If the specified destination's parent directory does not exist and you would "
-            "like to create it on-the-fly, use the --make-parents flag."
+class Copy(Subcommand):
+    """Holds all the logic for the `tune cp` subcommand."""
+
+    def __init__(self, subparsers):
+        super().__init__()
+        self._parser = subparsers.add_parser(
+            "cp",
+            prog="tune cp",
+            usage="tune cp <recipe|config> destination [OPTIONS]",
+            help="Copy a built-in recipe or config to a local path.",
+            description="Copy a built-in recipe or config to a local path.",
+            epilog=textwrap.dedent(
+                """\
+            examples:
+                $ tune cp lora_finetune_distributed .
+                Copied file to ./lora_finetune_distributed.py
+
+                $ tune cp llama2/7B_full ./new_dir/my_custom_lora.yaml --make-parents
+                Copyied file to ./new_dir/my_custom_lora.yaml
+
+            Need to see all possible recipes/configs to copy? Try running `tune ls`.
+            """
+            ),
+            formatter_class=argparse.RawTextHelpFormatter,
         )
+        self._add_arguments()
+        self._parser.set_defaults(func=self._cp_cmd)
 
+    def _add_arguments(self) -> None:
+        """Add arguments to the parser."""
+        self._parser.add_argument(
+            "file",
+            type=str,
+            help="Recipe/config to copy. For a list of all possible options, run `tune ls`",
+        )
+        self._parser.add_argument(
+            "destination",
+            type=Path,
+            help="Location to copy the file to",
+        )
+        self._parser.add_argument(
+            "-n",
+            "--no-clobber",
+            action="store_true",
+            help="Do not overwrite destination if it already exists",
+            default=False,
+        )
+        self._parser.add_argument(
+            "--make-parents",
+            action="store_true",
+            help="Create parent directories for destination if they do not exist. "
+            "If not set to True, will error if parent directories do not exist",
+            default=False,
+        )
 
-if __name__ == "__main__":
-    parser = argparse.ArgumentParser(
-        prog="tune cp",
-        usage="tune cp <recipe|config> destination [OPTIONS]",
-        description="Copy a built-in recipe or config to a local path.",
-        epilog=textwrap.dedent(
-            """\
-        examples:
-            $ tune cp lora_finetune_distributed.yaml ./my_custom_llama2_lora.yaml
-            $ tune cp full_finetune_distributed.py ./my_custom_full_finetune.py
-            $ tune cp full_finetune_distributed.py ./new_dir/my_custom_full_finetune.py --make-parents
-
-        Need to see all possible recipes/configs to copy? Try running `tune ls`.
-        And as always, you can also run `tune cp --help` for more information.
-        """
-        ),
-        formatter_class=argparse.RawTextHelpFormatter,
-    )
-    parser.add_argument(
-        "file",
-        type=str,
-        help="Recipe/config to copy. For a list of all possible options, run `tune ls`",
-    )
-    parser.add_argument(
-        "destination",
-        type=Path,
-        help="Location to copy the file to",
-    )
-    parser.add_argument(
-        "-n",
-        "--no-clobber",
-        action="store_true",
-        help="Do not overwrite destination if it already exists",
-        default=False,
-    )
-    parser.add_argument(
-        "--make-parents",
-        action="store_true",
-        help="Create parent directories for destination if they do not exist. "
-        "If not set to True, will error if parent directories do not exist",
-        default=False,
-    )
-    main(parser)
+    def _cp_cmd(self, args: argparse.Namespace):
+        """Copy a recipe or config to a new location."""
+        destination: Path = args.destination
+        src = None
+
+        # Iterate through all recipes and configs
+        for recipe in get_all_recipes():
+            if recipe.name == args.file:
+                src = ROOT / "recipes" / recipe.file_path
+                proper_suffix = ".py"
+                break
+            for config in recipe.configs:
+                if config.name == args.file:
+                    src = ROOT / "recipes" / "configs" / config.file_path
+                    proper_suffix = ".yaml"
+                    break
+
+        # Fail if no file exists
+        if src is None:
+            self._parser.error(
+                f"Invalid file name: {args.file}. Try `tune ls` to see all available files to copy."
+            )
+
+        # Attach proper suffix if needed
+        if destination.name != "" and destination.suffix != proper_suffix:
+            destination = destination.with_suffix(proper_suffix)
+
+        # Copy file
+        try:
+            if args.no_clobber and destination.exists():
+                print(
+                    f"File already exists at {destination.absolute()}, not overwriting."
+                )
+            else:
+                if args.make_parents:
+                    destination.parent.mkdir(parents=True, exist_ok=True)
+                output = shutil.copy(src, destination)
+                print(f"Copied file to {output}")
+        except FileNotFoundError:
+            self._parser.error(
+                f"Cannot create regular file: '{destination}'. No such file or directory. "
+                "If the specified destination's parent directory does not exist and you would "
+                "like to create it on-the-fly, use the --make-parents flag."
+            )
```

## torchtune/_cli/download.py

```diff
@@ -1,73 +1,115 @@
 # Copyright (c) Meta Platforms, Inc. and affiliates.
 # All rights reserved.
 #
 # This source code is licensed under the BSD-style license found in the
 # LICENSE file in the root directory of this source tree.
 
-"""This script downloads a model from the HuggingFace hub."""
-
 import argparse
 import os
+import textwrap
+
 from pathlib import Path
 
 from huggingface_hub import snapshot_download
+from huggingface_hub.utils import GatedRepoError, RepositoryNotFoundError
+from torchtune._cli.subcommand import Subcommand
+
 
+class Download(Subcommand):
+    """Holds all the logic for the `tune download` subcommand."""
+
+    def __init__(self, subparsers: argparse._SubParsersAction):
+        super().__init__()
+        self._parser = subparsers.add_parser(
+            "download",
+            prog="tune download",
+            usage="tune download <repo-id> [OPTIONS]",
+            help="Download a model from the Hugging Face Hub.",
+            description="Download a model from the Hugging Face Hub.",
+            epilog=textwrap.dedent(
+                """\
+            examples:
+                # Download a model from the Hugging Face Hub with a Hugging Face API token
+                $ tune download meta-llama/Llama-2-7b-hf --hf-token <TOKEN> --output-dir /tmp/model
+                Successfully downloaded model repo and wrote to the following locations:
+                ./model/config.json
+                ./model/README.md
+                ./model/consolidated.00.pth
+                ...
+
+                # Download an ungated model from the Hugging Face Hub
+                $ tune download mistralai/Mistral-7B-Instruct-v0.2
+                Successfully downloaded model repo and wrote to the following locations:
+                ./model/config.json
+                ./model/README.md
+                ./model/model-00001-of-00002.bin
+                ...
+
+            For a list of all models, visit the Hugging Face Hub https://huggingface.co/models.
+            """
+            ),
+            formatter_class=argparse.RawTextHelpFormatter,
+        )
+        self._add_arguments()
+        self._parser.set_defaults(func=self._download_cmd)
 
-def download(repo_id: str, output_dir: Path, hf_token: str) -> None:
-    """Downloads a model from the Hugging Face Hub.
+    def _add_arguments(self) -> None:
+        """Add arguments to the parser."""
+        self._parser.add_argument(
+            "repo_id",
+            type=str,
+            help="Name of the repository on Hugging Face Hub.",
+        )
+        self._parser.add_argument(
+            "--output-dir",
+            type=Path,
+            required=False,
+            default="./model",
+            help="Directory in which to save the model.",
+        )
+        self._parser.add_argument(
+            "--hf-token",
+            type=str,
+            required=False,
+            default=os.getenv("HF_TOKEN", None),
+            help="Hugging Face API token. Needed for gated models like Llama2.",
+        )
+        self._parser.add_argument(
+            "--ignore-patterns",
+            type=str,
+            required=False,
+            default="*.safetensors",
+            help="If provided, files matching any of the patterns are not downloaded. Defaults to ignoring "
+            "safetensors files as those are not currently supported in TorchTune.",
+        )
 
-    Args:
-        repo_id (str): Name of the repository on Hugging Face Hub.
-        output_dir (Path): Directory in which to save the model.
-        hf_token (str): Hugging Face API token.
-
-    Raises:
-        ValueError: If the model is not supported.
-    """
-    if "meta-llama" in repo_id and hf_token is None:
-        raise ValueError(
-            "You need to provide a Hugging Face API token to download gated models."
-            "You can find your token by visiting https://huggingface.co/settings/tokens"
-        )
-
-    # Download the tokenizer and PyTorch model files
-    snapshot_download(
-        repo_id,
-        local_dir=output_dir,
-        resume_download=True,
-        token=hf_token,
-    )
-
-    print(
-        "Succesfully downloaded model repo and wrote to the following locations:",
-        *list(output_dir.iterdir()),
-        sep="\n",
-    )
-
-
-if __name__ == "__main__":
-    parser = argparse.ArgumentParser(
-        description="Download a model from the Hugging Face Hub."
-    )
-    parser.add_argument(
-        "--repo-id",
-        type=str,
-        required=True,
-        help="Name of the repository on Hugging Face Hub.",
-    )
-    parser.add_argument(
-        "--output-dir",
-        type=Path,
-        required=False,
-        default="/tmp/model",
-        help="Directory in which to save the model.",
-    )
-    parser.add_argument(
-        "--hf-token",
-        type=str,
-        required=False,
-        default=os.getenv("HF_TOKEN", None),
-        help="Hugging Face API token. Needed for gated models like Llama2.",
-    )
-    args = parser.parse_args()
-    download(args.repo_id, args.output_dir, args.hf_token)
+    def _download_cmd(self, args: argparse.Namespace) -> None:
+        """Downloads a model from the Hugging Face Hub."""
+        # Download the tokenizer and PyTorch model files
+        print(f"Ignoring files matching the following patterns: {args.ignore_patterns}")
+        try:
+            true_output_dir = snapshot_download(
+                args.repo_id,
+                local_dir=args.output_dir,
+                ignore_patterns=args.ignore_patterns,
+                token=args.hf_token,
+            )
+        except GatedRepoError:
+            self._parser.error(
+                "It looks like you are trying to access a gated repository. Please ensure you "
+                "have access to the repository and have provided the proper Hugging Face API token "
+                "using the option `--hf-token` or by running `huggingface-cli login`."
+                "You can find your token by visiting https://huggingface.co/settings/tokens"
+            )
+        except RepositoryNotFoundError:
+            self._parser.error(
+                f"Repository '{args.repo_id}' not found on the Hugging Face Hub."
+            )
+        except Exception as e:
+            self._parser.error(e)
+
+        print(
+            "Successfully downloaded model repo and wrote to the following locations:",
+            *list(Path(true_output_dir).iterdir()),
+            sep="\n",
+        )
```

## torchtune/_cli/ls.py

```diff
@@ -1,58 +1,64 @@
 # Copyright (c) Meta Platforms, Inc. and affiliates.
 # All rights reserved.
 #
 # This source code is licensed under the BSD-style license found in the
 # LICENSE file in the root directory of this source tree.
 
-"""This script lists all built-in recipes/configs"""
-
 import argparse
 import textwrap
 
-from torchtune import list_configs, list_recipes
+from torchtune._cli.subcommand import Subcommand
+
+from torchtune._recipe_registry import get_all_recipes
 
-_NULL_VALUE = "<>"
 
+class List(Subcommand):
+    """Holds all the logic for the `tune ls` subcommand."""
 
-def main():
-    # Print table header
-    header = f"{'RECIPE':<20} {'CONFIG':<15}"
-    print(header)
-
-    # Print recipe/config pairs
-    for recipe in list_recipes():
-        configs = list_configs(recipe)
-        # If there are no configs for a recipe, print a blank config
-        if len(configs) == 0:
-            row = f"{recipe:<20} {_NULL_VALUE:<15}"
-            print(row)
-        for i, config in enumerate(configs):
-            # If there are multiple configs for a single recipe, omit the recipe name
-            # on latter configs
-            if i > 0:
-                recipe = ""
-            row = f"{recipe:<20} {config:<15}"
-            print(row)
-
-
-if __name__ == "__main__":
-    parser = argparse.ArgumentParser(
-        description="List all built-in recipes and configs",
-        usage="tune ls",
-        epilog=textwrap.dedent(
-            """\
-        examples:
-            $ tune ls
-            RECIPE                           CONFIG
-            full_finetune_distributed.py     full_finetune_distributed.yaml
-            lora_finetune_distributed.py     lora_finetune_distributed.yaml
-            alpaca_generate.py               alpaca_generate.yaml
-
-        To run one of these recipes:
-            $ tune full_finetune_single_device --config full_finetune_single_device
-        """
-        ),
-        formatter_class=argparse.RawTextHelpFormatter,
-    )
-    parser.parse_args()
-    main()
+    NULL_VALUE = "<>"
+
+    def __init__(self, subparsers: argparse._SubParsersAction):
+        super().__init__()
+        self._parser = subparsers.add_parser(
+            "ls",
+            prog="tune ls",
+            help="List all built-in recipes and configs",
+            description="List all built-in recipes and configs",
+            epilog=textwrap.dedent(
+                """\
+            examples:
+                $ tune ls
+                RECIPE                                   CONFIG
+                full_finetune_single_device              llama2/7B_full_single_device
+                full_finetune_distributed                llama2/7B_full
+                                                         llama2/13B_full
+                ...
+
+            To run one of these recipes:
+                $ tune run full_finetune_single_device --config full_finetune_single_device
+            """
+            ),
+            formatter_class=argparse.RawTextHelpFormatter,
+        )
+        self._parser.set_defaults(func=self._ls_cmd)
+
+    def _ls_cmd(self, args: argparse.Namespace) -> None:
+        """List all available recipes and configs."""
+        # Print table header
+        header = f"{'RECIPE':<40} {'CONFIG':<40}"
+        print(header)
+
+        # Print recipe/config pairs
+        for recipe in get_all_recipes():
+            # If there are no configs for a recipe, print a blank config
+            recipe_str = recipe.name
+            if len(recipe.configs) == 0:
+                row = f"{recipe_str:<40} {self.NULL_VALUE:<40}"
+                print(row)
+            for i, config in enumerate(recipe.configs):
+                # If there are multiple configs for a single recipe, omit the recipe name
+                # on latter configs
+                if i > 0:
+                    recipe_str = ""
+                row = f"{recipe_str:<40} {config.name:<40}"
+                print(row)
```

## torchtune/_cli/tune.py

```diff
@@ -1,137 +1,53 @@
 # Copyright (c) Meta Platforms, Inc. and affiliates.
 # All rights reserved.
 #
 # This source code is licensed under the BSD-style license found in the
 # LICENSE file in the root directory of this source tree.
 
-# Copyright (c) Facebook, Inc. and its affiliates.
-# All rights reserved.
-#
-# This source code is licensed under the BSD-style license found in the
-# LICENSE file in the root directory of this source tree.
-
-"""
-Launcher and utilities for torchtune recipes
-
-``tune`` provides functionality for launching torchtune recipes as well as local
-recipes. Aside from torchtune recipe utilties it integrates with ``torch.distributed.run``
-to support distributed job launching by default. ``tune`` offers everyting that ``torchrun``
-does with the following additional functionalities:
-
-1. ``tune <recipe> <recipe_args>`` with no optional ``torchrun`` options launches a single python process
-
-2. ``<recipe>`` and recipe arg ``<config>`` can both be passed in as names instead of paths if they're included in torchtune
-
-3. ``tune <path/to/recipe.py> <recipe_args>`` can be used to launch local recipes
-
-4. ``tune <torchrun_options> <recipe> <recipe_args>`` will launch a torchrun job
-
-.. note:: ``tune`` is a python
-          `console script <https://packaging.python.org/en/latest/specifications/entry-points/#use-for-scripts>`_
-          to the main module
-          `scripts.cli_utils.tune <https://github.com/pytorch/torchtune/blob/main/scripts/cli_utils/tune>`_
-          declared in the ``scripts`` configuration in
-          `setup.py <https://github.com/pytorch/torchtune/blob/main/setup.py>`_.
-          It is equivalent to invoking ``python -m scripts.cli_utils.tune``.
-"""
 import argparse
-import runpy
-import sys
-from pathlib import Path
-
-import torchtune
-from torch.distributed.run import get_args_parser, run
-from torchtune import list_recipes
-from torchtune._cli import list_scripts
-from torchtune.utils._distributed import _valid_distributed_single_node_nnodes
-
-
-def _update_parser_help(parser):
-    parser.description = "Torch Tune Recipe Launcher"
-    parser.usage = "tune [options] <recipe> [recipe_args]"
-    parser.formatter_class = argparse.RawDescriptionHelpFormatter
-
-    # Update torchrun argparse name for more accurate CLI help
-    actions = [a.dest for a in parser._actions]
-    # Update training_script help to be recipe
-    idx = actions.index("training_script")
-    parser._actions[idx].dest = "recipe"
-    parser._actions[idx].help = "Name or path to recipe to be launched followed by args"
-
-    # Update training_script_args help to be recipe_args
-    idx = actions.index("training_script_args")
-    parser._actions[idx].dest = "recipe_args"
-
-
-def _is_distributed_args(args):
-    total = len(sys.argv) - 1  # total args minus "tune"
-    script_args = len(args.recipe_args) + 1  # script args + 1 for script name
-    return total > script_args
-
-
-def _validate_distributed_args(args):
-    """
-    Validates nnodes and nproc_per_node are appropriately set for distributed training
-    runs.
-    """
-    if not hasattr(args, "nnodes"):
-        raise RuntimeError("Expect --nnodes to be specified for distributed runs")
-
-    if args.nnodes not in _valid_distributed_single_node_nnodes:
-        raise RuntimeError(
-            f"Expect --nnodes to be one of {_valid_distributed_single_node_nnodes}"
-        )
 
-    if not hasattr(args, "nproc_per_node"):
-        raise RuntimeError(
-            "Expect --nproc_per_node to be specified for distributed runs"
+from torchtune._cli.cp import Copy
+from torchtune._cli.download import Download
+from torchtune._cli.ls import List
+from torchtune._cli.run import Run
+from torchtune._cli.validate import Validate
+
+
+class TuneCLIParser:
+    """Holds all information related to running the CLI"""
+
+    def __init__(self):
+        # Initialize the top-level parser
+        self._parser = argparse.ArgumentParser(
+            prog="tune",
+            description="Welcome to the TorchTune CLI!",
+            add_help=True,
         )
+        # Default command is to print help
+        self._parser.set_defaults(func=lambda args: self._parser.print_help())
 
-    # TODO (rohan-varma): Add check that nproc_per_node <= cuda device count. Currently,
-    # we don't do this since we test on CPUs for distributed. Will update once multi GPU
-    # CI is supported.
+        # Add subcommands
+        subparsers = self._parser.add_subparsers(title="subcommands")
+        Download.create(subparsers)
+        List.create(subparsers)
+        Copy.create(subparsers)
+        Run.create(subparsers)
+        Validate.create(subparsers)
+
+    def parse_args(self) -> argparse.Namespace:
+        """Parse CLI arguments"""
+        return self._parser.parse_args()
+
+    def run(self, args: argparse.Namespace) -> None:
+        """Execute CLI"""
+        args.func(args)
 
 
 def main():
-    parser = get_args_parser()
-    _update_parser_help(parser)
+    parser = TuneCLIParser()
     args = parser.parse_args()
-
-    distributed_args = _is_distributed_args(args)
-    cmd = args.recipe
-    if not cmd.endswith(".py"):
-        pkg_path = Path(torchtune.__file__).parent.absolute()
-        if f"{cmd}.py" in list_recipes():
-            recipes_pkg_path = pkg_path.parent / "recipes"
-            cmd = recipes_pkg_path / f"{cmd}.py"
-            args.recipe = str(cmd)
-
-            # Replace config name with package path if provided
-            if "--config" in args.recipe_args:
-                cfg_idx = args.recipe_args.index("--config") + 1
-                config = args.recipe_args[cfg_idx]
-                if not config.endswith(".yaml"):
-                    args.recipe_args[cfg_idx] = str(
-                        recipes_pkg_path / "configs" / f"{config}.yaml"
-                    )
-        elif cmd in list_scripts():
-            cmd = pkg_path / "_cli" / f"{cmd}.py"
-            args.recipe = str(cmd)
-            assert not distributed_args, "You can't use distributed args with scripts"
-        else:
-            parser.error(
-                f"Unrecognized command '{cmd}'\nTry 'tune --help' for more information."
-            )
-
-    if distributed_args:
-        _validate_distributed_args(args)
-        args.training_script = str(cmd)  # arg names expected by torchrun
-        args.training_script_args = args.recipe_args
-        run(args)
-    else:
-        sys.argv = [str(cmd)] + args.recipe_args
-        runpy.run_path(str(cmd), run_name="__main__")
+    parser.run(args)
 
 
 if __name__ == "__main__":
     main()
```

## torchtune/_cli/validate.py

```diff
@@ -2,37 +2,58 @@
 # All rights reserved.
 #
 # This source code is licensed under the BSD-style license found in the
 # LICENSE file in the root directory of this source tree.
 
 import argparse
 import textwrap
+from pathlib import Path
+
+from omegaconf import OmegaConf
 
-from omegaconf import DictConfig
 from torchtune import config
-from torchtune.config._utils import _merge_yaml_and_cli_args
-from torchtune.utils import TuneArgumentParser
+from torchtune._cli.subcommand import Subcommand
+from torchtune.config._errors import ConfigError
+
 
+class Validate(Subcommand):
+    """Holds all the logic for the `tune validate` subcommand."""
 
-def main(cfg: DictConfig):
-    config.validate(cfg)
-    print("Config is well-formed!")
-
-
-if __name__ == "__main__":
-    parser = TuneArgumentParser(
-        description="Validate a config and ensure that it is well-formed.",
-        usage="tune validate",
-        epilog=textwrap.dedent(
-            """\
-        examples:
-            $ tune validate --config recipes/configs/full_finetune_distributed.yaml
-            Config is well-formed!
-        """
-        ),
-        formatter_class=argparse.RawTextHelpFormatter,
-    )
-    # Get user-specified args from config and CLI and create params for recipe
-    yaml_args, cli_args = parser.parse_known_args()
-    conf = _merge_yaml_and_cli_args(yaml_args, cli_args)
+    def __init__(self, subparsers: argparse._SubParsersAction):
+        super().__init__()
+        self._parser = subparsers.add_parser(
+            "validate",
+            prog="tune validate",
+            help="Validate a config and ensure that it is well-formed.",
+            description="Validate a config and ensure that it is well-formed.",
+            usage="tune validate <config>",
+            epilog=textwrap.dedent(
+                """\
+                examples:
+
+                    $ tune validate recipes/configs/full_finetune_distributed.yaml
+                    Config is well-formed!
+                """
+            ),
+            formatter_class=argparse.RawTextHelpFormatter,
+        )
+        self._add_arguments()
+        self._parser.set_defaults(func=self._validate_cmd)
+
+    def _add_arguments(self) -> None:
+        """Add arguments to the parser."""
+        self._parser.add_argument(
+            "config",
+            type=Path,
+            help="Path to a config to validate.",
+        )
+
+    def _validate_cmd(self, args: argparse.Namespace):
+        """Validate a config file."""
+        cfg = OmegaConf.load(args.config)
+
+        try:
+            config.validate(cfg)
+        except ConfigError as e:
+            self._parser.error(str(e))
 
-    main(conf)
+        print("Config is well-formed!")
```

## torchtune/config/__init__.py

```diff
@@ -2,14 +2,16 @@
 # All rights reserved.
 #
 # This source code is licensed under the BSD-style license found in the
 # LICENSE file in the root directory of this source tree.
 
 from ._instantiate import instantiate
 from ._parse import parse
+from ._utils import log_config
 from ._validate import validate
 
 __all__ = [
     "parse",
     "instantiate",
     "validate",
+    "log_config",
 ]
```

## torchtune/config/_instantiate.py

 * *Ordering differences only*

```diff
@@ -47,14 +47,21 @@
     You can use this function to create the exact instance of a TorchTune object you want
     to use in your recipe using the specification from the config.
 
     This function also supports passing in positional args and keyword args within the
     function call. These are automatically merged with the provided config, with keyword
     args taking precedence.
 
+    Args:
+        config (DictConfig): a single field in the OmegaConf object parsed from the yaml file.
+            This is expected to have a _component_ field specifying the path of the object
+            to instantiate.
+        *args (Tuple[Any, ...]): positional arguments to pass to the object to instantiate.
+        **kwargs (Dict[str, Any]): keyword arguments to pass to the object to instantiate.
+
     Examples:
         >>> config.yaml:
         >>>     model:
         >>>       _component_: torchtune.models.llama2
         >>>       num_layers: 32
         >>>       num_heads: 32
         >>>       num_kv_heads: 32
@@ -62,21 +69,14 @@
         >>> from torchtune import config
         >>> vocab_size = 32000
         >>> # Pass in vocab size as positional argument. Since it is positioned first
         >>> # in llama2(), it must be specified first. Pass in other arguments as kwargs.
         >>> # This will return an nn.Module directly for llama2 with specified args.
         >>> model = config.instantiate(parsed_yaml.model, vocab_size, max_seq_len=4096, embed_dim=4096)
 
-    Args:
-        config (DictConfig): a single field in the OmegaConf object parsed from the yaml file.
-            This is expected to have a _component_ field specifying the path of the object
-            to instantiate.
-        *args (Tuple[Any, ...]): positional arguments to pass to the object to instantiate.
-        **kwargs (Dict[str, Any]): keyword arguments to pass to the object to instantiate.
-
     Returns:
         Any: the instantiated object.
 
     Raises:
         ValueError: if config is not a DictConfig.
     """
```

## torchtune/config/_parse.py

```diff
@@ -6,51 +6,47 @@
 import argparse
 import functools
 import sys
 from typing import Any, Callable
 
 from omegaconf import DictConfig
 from torchtune.config._utils import _merge_yaml_and_cli_args
-from torchtune.utils.argparse import TuneArgumentParser
-from torchtune.utils.logging import get_logger
+from torchtune.utils.argparse import TuneRecipeArgumentParser
 
 
 Recipe = Callable[[DictConfig], Any]
 
 
 def parse(recipe_main: Recipe) -> Callable[[Recipe], Any]:
     """
     Decorator that handles parsing the config file and CLI overrides
     for a recipe. Use it on the recipe's main function.
 
-    Example: in recipe/my_recipe.py,
+    Args:
+        recipe_main (Recipe): The main method that initializes
+            and runs the recipe
+
+    Examples:
         >>> @parse
         >>> def main(cfg: DictConfig):
         >>>     ...
 
-    With the decorator, the parameters will be parsed into cfg when run as:
+        >>> # With the decorator, the parameters will be parsed into cfg when run as:
         >>> tune my_recipe --config config.yaml foo=bar
 
-    Args:
-        recipe_main (Recipe): The main method that initializes
-            and runs the recipe
-
     Returns:
         Callable[[Recipe], Any]: the decorated main
     """
 
     @functools.wraps(recipe_main)
     def wrapper(*args: Any, **kwargs: Any) -> Any:
-        parser = TuneArgumentParser(
+        parser = TuneRecipeArgumentParser(
             description=recipe_main.__doc__,
             formatter_class=argparse.RawDescriptionHelpFormatter,
         )
         # Get user-specified args from config and CLI and create params for recipe
         yaml_args, cli_args = parser.parse_known_args()
         conf = _merge_yaml_and_cli_args(yaml_args, cli_args)
 
-        logger = get_logger("DEBUG")
-        logger.info(msg=f"Running {recipe_main.__name__} with parameters {conf}")
-
         sys.exit(recipe_main(conf))
 
     return wrapper
```

## torchtune/config/_utils.py

```diff
@@ -8,14 +8,34 @@
 from importlib import import_module
 from types import ModuleType
 from typing import Any, Dict, List, Union
 
 from omegaconf import DictConfig, OmegaConf
 
 from torchtune.config._errors import InstantiationError
+from torchtune.data import ChatFormat, InstructTemplate
+from torchtune.utils import get_logger, get_world_size_and_rank
+
+
+def log_config(recipe_name: str, cfg: DictConfig) -> None:
+    """
+    Logs the parsed config to rank zero.
+
+    Args:
+        recipe_name (str): name of the recipe to display
+        cfg (DictConfig): parsed config object
+    """
+    # Log the config only on rank 0
+    _, rank = get_world_size_and_rank()
+    if rank != 0:
+        return
+
+    logger = get_logger("DEBUG")
+    cfg_str = OmegaConf.to_yaml(cfg, resolve=True, sort_keys=True)
+    logger.info(msg=f"Running {recipe_name} with resolved config:\n\n{cfg_str}")
 
 
 def _has_component(node: Union[Dict[str, Any], DictConfig]) -> bool:
     return (OmegaConf.is_dict(node) or isinstance(node, dict)) and "_component_" in node
 
 
 def _get_component_from_path(path: str) -> Any:
@@ -93,18 +113,17 @@
 def _merge_yaml_and_cli_args(yaml_args: Namespace, cli_args: List[str]) -> DictConfig:
     """
     Takes the direct output of argparse's parse_known_args which returns known
     args as a Namespace and unknown args as a dotlist (in our case, yaml args and
     cli args, respectively) and merges them into a single OmegaConf DictConfig.
 
     If a cli arg overrides a yaml arg with a _component_ field, the cli arg can
-    be specified with the parent field directly, i.e.,
-    model=torchtune.models.llama2_7b instead of model._component_=torchtune.models.llama2_7b.
-    Nested fields within the component should be specified with dot notation, i.e.,
-    model.max_batch_size=2.
+    be specified with the parent field directly, e.g., model=torchtune.models.lora_llama2_7b
+    instead of model._component_=torchtune.models.lora_llama2_7b. Nested fields within the
+    component should be specified with dot notation, e.g., model.lora_rank=16.
 
     Example:
         >>> config.yaml:
         >>>     a: 1
         >>>     b:
         >>>       _component_: torchtune.models.my_model
         >>>       c: 3
@@ -144,7 +163,58 @@
 
     # Merge the args
     cli_conf = OmegaConf.from_dotlist(cli_dotlist)
     yaml_conf = OmegaConf.create(yaml_kwargs)
 
     # CLI takes precedence over yaml args
     return OmegaConf.merge(yaml_conf, cli_conf)
+
+
+def _try_get_component(module_path: str, component_name: str, class_type: str) -> Any:
+    """
+    Try-except wrapper around `_get_component_from_path`, used to quickly retrieve
+    a class from a name string with better error handling.
+
+    Args:
+        module_path (str): path string of the file the class resides in
+        component_name (str): name of the class
+        class_type (str): type of the class, only used for more descriptive error message
+
+
+    Returns:
+        Any: the class
+
+    Raises:
+        ValueError: if the string is not a valid class
+    """
+    try:
+        return _get_component_from_path(module_path + "." + component_name)
+    except InstantiationError:
+        raise ValueError(f"Invalid {class_type} class: '{component_name}'") from None
+
+
+def _get_instruct_template(template: str) -> InstructTemplate:
+    """
+    Get the instruct template class from the template string.
+
+    Args:
+        template (str): class name of template, or string with placeholders
+
+    Returns:
+        InstructTemplate: the prompt template class or the same verified string
+    """
+    return _try_get_component(
+        "torchtune.data._instruct_templates", template, "InstructTemplate"
+    )
+
+
+def _get_chat_format(chat_format: str) -> ChatFormat:
+    """
+    Get the chat format class from a string.
+
+    Args:
+        chat_format (str): class name of the ChatFormat
+
+    Returns:
+        ChatFormat: the chat format class
+    """
+    return _try_get_component("torchtune.data._chat_formats", chat_format, "ChatFormat")
```

## torchtune/data/__init__.py

```diff
@@ -1,19 +1,40 @@
 # Copyright (c) Meta Platforms, Inc. and affiliates.
 # All rights reserved.
 #
 # This source code is licensed under the BSD-style license found in the
 # LICENSE file in the root directory of this source tree.
 
-from torchtune.data._templates import (
+from torchtune.data._chat_formats import (
+    ChatFormat,
+    ChatMLFormat,
+    Llama2ChatFormat,
+    MistralChatFormat,
+)
+from torchtune.data._common import CROSS_ENTROPY_IGNORE_IDX
+from torchtune.data._converters import sharegpt_to_llama2_messages
+from torchtune.data._instruct_templates import (
     AlpacaInstructTemplate,
     GrammarErrorCorrectionTemplate,
-    PromptTemplate,
+    InstructTemplate,
+    StackExchangedPairedTemplate,
     SummarizeTemplate,
 )
+from torchtune.data._types import Message
+from torchtune.data._utils import truncate, validate_messages
 
 __all__ = [
     "AlpacaInstructTemplate",
+    "ChatFormat",
+    "CROSS_ENTROPY_IGNORE_IDX",
     "GrammarErrorCorrectionTemplate",
-    "PromptTemplate",
+    "InstructTemplate",
     "SummarizeTemplate",
+    "Llama2ChatFormat",
+    "MistralChatFormat",
+    "ChatMLFormat",
+    "sharegpt_to_llama2_messages",
+    "truncate",
+    "Message",
+    "validate_messages",
+    "StackExchangedPairedTemplate",
 ]
```

## torchtune/datasets/__init__.py

```diff
@@ -1,15 +1,26 @@
 # Copyright (c) Meta Platforms, Inc. and affiliates.
 # All rights reserved.
 #
 # This source code is licensed under the BSD-style license found in the
 # LICENSE file in the root directory of this source tree.
 
-from torchtune.datasets._alpaca import alpaca_dataset
-from torchtune.datasets._instruct import InstructDataset
-from torchtune.datasets._slimorca import SlimOrcaDataset
+from torchtune.datasets._alpaca import alpaca_cleaned_dataset, alpaca_dataset
+from torchtune.datasets._chat import chat_dataset, ChatDataset
+from torchtune.datasets._grammar import grammar_dataset
+from torchtune.datasets._instruct import instruct_dataset, InstructDataset
+from torchtune.datasets._samsum import samsum_dataset
+from torchtune.datasets._slimorca import slimorca_dataset
+from torchtune.datasets._stack_exchanged_paired import stack_exchanged_paired_dataset
 
 __all__ = [
     "alpaca_dataset",
-    "SlimOrcaDataset",
+    "alpaca_cleaned_dataset",
+    "grammar_dataset",
+    "samsum_dataset",
+    "stack_exchanged_paired_dataset",
     "InstructDataset",
+    "slimorca_dataset",
+    "ChatDataset",
+    "instruct_dataset",
+    "chat_dataset",
 ]
```

## torchtune/datasets/_alpaca.py

```diff
@@ -1,60 +1,62 @@
 # Copyright (c) Meta Platforms, Inc. and affiliates.
 # All rights reserved.
 #
 # This source code is licensed under the BSD-style license found in the
 # LICENSE file in the root directory of this source tree.
 
+from functools import partial
+
 from torchtune.data import AlpacaInstructTemplate
 from torchtune.datasets._instruct import InstructDataset
 from torchtune.modules import Tokenizer
 
 
 def alpaca_dataset(
     tokenizer: Tokenizer,
+    source: str = "tatsu-lab/alpaca",
     train_on_input: bool = True,
-    use_clean: bool = False,
+    max_seq_len: int = 512,
 ) -> InstructDataset:
     """
-    Support for the Alpaca dataset and its variants from HuggingFace Datasets.
-    https://huggingface.co/datasets/tatsu-lab/alpaca
-
-    Data input format: https://huggingface.co/datasets/tatsu-lab/alpaca#data-instances
-
-    The input is created using the prompt template from the original alpaca codebase:
-    https://github.com/tatsu-lab/stanford_alpaca/blob/761dc5bfbdeeffa89b8bff5d038781a4055f796a/train.py#L31
-
-    where `instruction`, `input`, and `output` are fields from the dataset.
+    Support for family of Alpaca-style datasets from Hugging Face Datasets using
+    the `data input format <https://huggingface.co/datasets/tatsu-lab/alpaca#data-instances>`_
+    and `prompt template <https://github.com/tatsu-lab/stanford_alpaca/blob/main/train.py#L31>`_
+    from the original alpaca codebase, where `instruction`, `input`, and `output`
+    are fields from the dataset.
 
     Masking of the prompt during training is controlled by the `train_on_input` flag, which is
-    set to `True` by default (ref: https://github.com/tloen/alpaca-lora/blob/main/finetune.py#L49)
+    set to `True` by `default <https://github.com/tloen/alpaca-lora/blob/main/finetune.py#L49>`_
     - If `train_on_input` is True, the prompt is used during training and
     contributes to the loss.
     - If `train_on_input` is False, the prompt is masked out (tokens replaced with -100)
 
-    The version of the dataset used is controlled by the `use_clean` flag which set to False by default.
-    - If `use_clean` is True, then https://huggingface.co/datasets/yahma/alpaca-cleaned is used
-    - If `use_clean` is False, then https://huggingface.co/datasets/tatsu-lab/alpaca is used
-
     Args:
         tokenizer (Tokenizer): Tokenizer used to encode data. Tokenize must implement an `encode` and `decode` method.
+        source (str): path string of dataset, anything supported by Hugging Face's `load_dataset`.
         train_on_input (bool): Whether the model is trained on the prompt or not. Default is True.
-        use_clean (bool): Whether to use the cleaned version of the dataset or not. Default is False.
+        max_seq_len (int): Maximum number of tokens in the returned input and label token id lists.
+            Default is 512, but we recommend setting this to the highest you can fit in memory and
+            is supported by the model. For example, llama2-7B supports up to 4096 for sequence length.
 
     Returns:
-        InstructDataset: dataset configured with Alpaca source data and template
+        InstructDataset: dataset configured with source data and template
 
 
     Example:
         >>> alpaca_ds = alpaca_dataset(tokenizer=tokenizer)
         >>> for batch in Dataloader(alpaca_ds, batch_size=8):
         >>>     print(f"Batch size: {len(batch)}")
         >>> Batch size: 8
     """
 
     return InstructDataset(
         tokenizer=tokenizer,
-        source="yahma/alpaca-cleaned" if use_clean else "tatsu-lab/alpaca",
-        template=AlpacaInstructTemplate(),
+        source=source,
+        template=AlpacaInstructTemplate,
         train_on_input=train_on_input,
+        max_seq_len=max_seq_len,
         split="train",
     )
+
+
+alpaca_cleaned_dataset = partial(alpaca_dataset, source="yahma/alpaca-cleaned")
```

## torchtune/datasets/_instruct.py

```diff
@@ -1,169 +1,150 @@
 # Copyright (c) Meta Platforms, Inc. and affiliates.
 # All rights reserved.
 #
 # This source code is licensed under the BSD-style license found in the
 # LICENSE file in the root directory of this source tree.
 
-import copy
-import re
 from typing import Any, Callable, Dict, List, Mapping, Optional, Tuple
 
+import numpy as np
 from datasets import load_dataset
 from torch.utils.data import Dataset
-from torchtune.config._errors import InstantiationError
-from torchtune.config._utils import _get_component_from_path
+from torchtune.config._utils import _get_instruct_template
+
+from torchtune.data import (
+    CROSS_ENTROPY_IGNORE_IDX,
+    InstructTemplate,
+    Message,
+    validate_messages,
+)
 
-from torchtune.data import PromptTemplate
-from torchtune.datasets._common import CROSS_ENTROPY_IGNORE_IDX
 from torchtune.modules import Tokenizer
 
 
 class InstructDataset(Dataset):
     """
     Class that supports any custom dataset with instruction-based prompts and a
     configurable template.
 
     The general flow from loading a sample to tokenized prompt is:
     load sample -> apply transform -> format into template -> tokenize
 
-    If the column/key names differ from the expected names in the `PromptTemplate`,
+    If the column/key names differ from the expected names in the `InstructTemplate`,
     then the `column_map` argument can be used to provide this mapping.
 
     Masking of the prompt during training is controlled by the `train_on_input` flag, which is
     set to `False` by default.
     - If `train_on_input` is True, the prompt is used during training and
     contributes to the loss.
     - If `train_on_input` is False, the prompt is masked out (tokens replaced with -100)
 
     Args:
         tokenizer (Tokenizer): Tokenizer used to encode data. Tokenize must implement an `encode` and `decode` method.
-        source (str): path string of dataset, anything supported by HuggingFace's `load_dataset`
+        source (str): path string of dataset, anything supported by Hugging Face's `load_dataset`
             (https://huggingface.co/docs/datasets/en/package_reference/loading_methods#datasets.load_dataset.path)
-        template (PromptTemplate): template used to format the prompt. If the placeholder variable
+        template (InstructTemplate): template used to format the prompt. If the placeholder variable
             names in the template do not match the column/key names in the dataset, use `column_map` to map them.
         transform (Optional[Callable]): transform to apply to the sample before formatting to the template.
             Default is None.
         column_map (Optional[Dict[str, str]]): a mapping from the expected placeholder names in the template
             to the column/key names in the sample. If None, assume these are identical.
         train_on_input (bool): Whether the model is trained on the prompt or not. Default is False.
+        max_seq_len (Optional[int]): Maximum number of tokens in the returned input and label token id lists.
+            Default is None, disabling truncation. We recommend setting this to the highest you can fit in memory
+            and is supported by the model. For example, llama2-7B supports up to 4096 for sequence length.
         **load_dataset_kwargs (Dict[str, Any]): additional keyword arguments to pass to `load_dataset`.
     """
 
     def __init__(
         self,
         tokenizer: Tokenizer,
         source: str,
-        template: PromptTemplate,
+        template: InstructTemplate,
         transform: Optional[Callable] = None,
         column_map: Optional[Dict[str, str]] = None,
         train_on_input: bool = False,
+        max_seq_len: Optional[int] = None,
         **load_dataset_kwargs: Dict[str, Any],
     ) -> None:
         self._tokenizer = tokenizer
         self._data = load_dataset(source, **load_dataset_kwargs)
         self.template = template
         self._transform = transform
         self._column_map = column_map
         self.train_on_input = train_on_input
+        self.max_seq_len = max_seq_len
 
     def __len__(self):
         return len(self._data)
 
     def __getitem__(self, index: int) -> Tuple[List[int], List[int]]:
         sample = self._data[index]
         return self._prepare_sample(sample)
 
     def _prepare_sample(self, sample: Mapping[str, Any]) -> Tuple[List[int], List[int]]:
         transformed_sample = self._transform(sample) if self._transform else sample
 
         prompt = self.template.format(transformed_sample, self._column_map)
-        key_output = self._column_map["output"] if self._column_map else "output"
-        prompt_with_response = prompt + sample[key_output]
-
-        encoded_prompt = self._tokenizer.encode(
-            text=prompt, add_bos=True, add_eos=False
+        key_output = (
+            self._column_map["output"]
+            if self._column_map and "output" in self._column_map
+            else "output"
         )
-        encoded_prompt_with_response = self._tokenizer.encode(
-            text=prompt_with_response, add_bos=True, add_eos=True
-        )
-        labels = copy.deepcopy(encoded_prompt_with_response)
+        messages = [
+            Message(role="user", content=prompt, masked=(not self.train_on_input)),
+            Message(role="assistant", content=transformed_sample[key_output]),
+        ]
+
+        validate_messages(messages)
 
-        if not self.train_on_input:
-            labels[: len(encoded_prompt)] = [CROSS_ENTROPY_IGNORE_IDX] * len(
-                encoded_prompt
-            )
+        tokens, mask = self._tokenizer.tokenize_messages(
+            messages, max_seq_len=self.max_seq_len
+        )
 
-        assert len(encoded_prompt_with_response) == len(labels)
+        # Wherever mask == True, set to CROSS_ENTROPY_IGNORE_IDX. Otherwise keep as tokens
+        labels = list(np.where(mask, CROSS_ENTROPY_IGNORE_IDX, tokens))
+        assert len(tokens) == len(labels)
 
-        return encoded_prompt_with_response, labels
+        return tokens, labels
 
 
 def instruct_dataset(
     tokenizer: Tokenizer,
     source: str,
     template: str,
     column_map: Optional[Dict[str, str]] = None,
     train_on_input: bool = False,
+    max_seq_len: Optional[int] = None,
     **load_dataset_kwargs: Dict[str, Any],
 ) -> InstructDataset:
     """
     Build a configurable dataset with instruction prompts. This method should be
     used to configure a custom instruct dataset from the yaml config instead of
     using `InstructDataset` directly, as it is made to be config friendly.
 
     Args:
         tokenizer (Tokenizer): Tokenizer used to encode data. Tokenize must implement an `encode` and `decode` method.
-        source (str): path string of dataset, anything supported by HuggingFace's `load_dataset`
+        source (str): path string of dataset, anything supported by Hugging Face's `load_dataset`
             (https://huggingface.co/docs/datasets/en/package_reference/loading_methods#datasets.load_dataset.path)
-        template (str): class name of template used to format the prompt. If the placeholder variable
+        template (str): class used to format the prompt. If the placeholder variable
             names in the template do not match the column/key names in the dataset, use `column_map` to map them.
         column_map (Optional[Dict[str, str]]): a mapping from the expected placeholder names in the template
             to the column/key names in the sample. If None, assume these are identical.
         train_on_input (bool): Whether the model is trained on the prompt or not. Default is False.
+        max_seq_len (Optional[int]): Maximum number of tokens in the returned input and label token id lists.
+            Default is None, disabling truncation. We recommend setting this to the highest you can fit in memory
+            and is supported by the model. For example, llama2-7B supports up to 4096 for sequence length.
         **load_dataset_kwargs (Dict[str, Any]): additional keyword arguments to pass to `load_dataset`.
 
     Returns:
         InstructDataset: the configured InstructDataset
     """
     return InstructDataset(
         tokenizer=tokenizer,
         source=source,
-        template=_get_template(template),
+        template=_get_instruct_template(template),
         column_map=column_map,
         train_on_input=train_on_input,
+        max_seq_len=max_seq_len,
         **load_dataset_kwargs,
     )
-
-
-def _get_template(template: str) -> PromptTemplate:
-    """
-    Get the prompt template class from the template string.
-
-    String should either be the PromptTemplate class name directly, or a raw
-    string with 1 or more placeholders. If none of these apply, then raise an
-    error.
-
-    Args:
-        template (str): class name of template, or string with placeholders
-
-    Returns:
-        PromptTemplate: the prompt template class or the same verified string
-
-    Raises:
-        ValueError: if the template is not a PromptTemplate class or a proper
-            template string
-    """
-    path = "torchtune.data." + template
-    try:
-        template_class = _get_component_from_path(path)
-        return template_class()
-    except InstantiationError:
-        # Verify that string can be used as a template, should have variable
-        # placeholders
-        pattern = r"\{.+?\}"
-        if not re.search(pattern, template):
-            raise ValueError(
-                f"Invalid template '{template}': "
-                + "Must be a PromptTemplate class or a string with placeholders."
-            ) from None
-        return template
```

## torchtune/datasets/_slimorca.py

```diff
@@ -1,134 +1,70 @@
 # Copyright (c) Meta Platforms, Inc. and affiliates.
 # All rights reserved.
 #
 # This source code is licensed under the BSD-style license found in the
 # LICENSE file in the root directory of this source tree.
 
-from typing import Dict, List, Tuple
+from torchtune.data import Llama2ChatFormat, sharegpt_to_llama2_messages
 
-from datasets import load_dataset
-from torch.utils.data import Dataset
+from torchtune.datasets._chat import ChatDataset
 
-from torchtune.datasets._common import CROSS_ENTROPY_IGNORE_IDX
-
-# Not ideal to import this type here but it's needed for the transform function
 from torchtune.modules import Tokenizer
 
 
-class _Llama2ChatFormatConstants:
-    """
-    Contains constants that are used in Llama2 Chat Format.
-    """
-
-    B_INST, E_INST = "[INST]", "[/INST]"
-    B_SYS, E_SYS = "<<SYS>>\n", "\n<</SYS>>\n\n"
-
-
-class SlimOrcaDataset(Dataset):
+def slimorca_dataset(
+    tokenizer: Tokenizer,
+    source: str = "Open-Orca/SlimOrca-Dedup",
+    max_seq_len: int = 1024,
+    train_on_input: bool = False,
+) -> ChatDataset:
     """
-    PyTorch Representation of the SlimOrca Dataset
-    https://huggingface.co/datasets/Open-Orca/SlimOrca-Dedup
-    from Hugging Face.
+    Support for `SlimOrca-style <https://huggingface.co/datasets/Open-Orca/SlimOrca-Dedup>`_
+    family of conversational datasets.
 
     The data is formatted to adhere to Llama2 Chat Format.
     This format is required if the base model is Llama2 Chat Model.
     The base Llama2 Model doesn't prescribe a particular format.
 
     The returned data is a tuple of input token id list and label token id
-    list. If `max_token_length` keyword argument is provided, the returned
+    list. If `max_seq_len` keyword argument is provided, the returned
     input token id list is ensured (by truncation if necessary) to be within
     that length.
 
-    Data input format: https://huggingface.co/datasets/Open-Orca/SlimOrca-Dedup#dataset-format
-
     Args:
         tokenizer (Tokenizer): Tokenizer used to encode data. Tokenize must implement an `encode` and `decode` method.
-        **kwargs: Additional keyword arguments to pass to the SlimOrca Dataset.
-
-    Keyword Arguments:
-        max_token_length (int): Maximum number of tokens in the returned input and label token id lists. This value needs to be at least 4 though it is generally set to max sequence length accepted by the model. Default is 1024.
+        source (str): path string of dataset, anything supported by Hugging Face's `load_dataset`.
+        max_seq_len (int): Maximum number of tokens in the returned input and label token id lists.
+            This value needs to be at least 4 though it is generally set to max sequence length accepted by the model.
+            Default is 1024.
+        train_on_input (bool): Whether the model is trained on the prompt or not. Default is False.
 
     Raises:
-        ValueError: If `max_token_length` is less than 4.
+        ValueError: If `max_seq_len` is less than 4.
+
+    Returns:
+        ChatDataset: dataset configured with SlimOrca source data and LLaMA2 chat template
 
     Example:
-        >>> ds = SlimOrcaDataset(tokenizer=tokenizer, max_token_length=10)
+        >>> ds = slimorca_dataset(tokenizer=tokenizer, max_seq_len=10)
         >>> for input, label in ds:
         >>>     print(input)
         >>>     print(label)
         >>>
-        >>> Sample Ouput:
+        >>> Sample Output:
         >>> [1, 351, 82, 391, 221, 220, 193, 12, 471, ..., 2]
         >>> [-100, -100, -100, -100, -100, -100, -100, -100, 471, ..., 2]
-    """  # noqa
-
-    def __init__(self, tokenizer: Tokenizer, **kwargs) -> None:
-        self._data = load_dataset("Open-Orca/SlimOrca-Dedup", split="train")
-        self._tokenizer = tokenizer
-        self._max_token_length = kwargs.get("max_token_length", 1024)
-        if self._max_token_length < 4:
-            # Input token needs to have 1 bos, 1 eos,
-            # and 1 token from prompt, 1 from label
-            raise ValueError("max_token_length must be at least 4")
-
-    def __len__(self):
-        return len(self._data)
-
-    def __getitem__(self, index: int) -> Tuple[List[int], List[int]]:
-        data = self._data[index]["conversations"]
-        prompt, label = self._generate_prompt_label(data)
-        return self._generate_tokens(prompt, label)
-
-    def _generate_tokens(self, prompt: str, label: str) -> Tuple[List[int], List[int]]:
-        """
-        Given a prompt string and label string, generate input and label token id lists.
-
-        Tokenizer is used to tokenize both the strings.
-        The prompt token list is truncated to `max_token_length` - 2
-        (so that there is at least one label token, as EOS takes one token).
-
-        The label token list is truncated to `max_token_length` - len(prompt_token_list)
-
-        Finally input token list is the concatenation of prompt and label token lists.
-
-        Label token list is padded with cross entropy ignore idx value to match the length of input token list.
-        """
-        prompt_tokens = self._tokenizer.encode(prompt, add_bos=True, add_eos=False)
-        # Truncate to max token length - 2 (so that there is at least one label token)
-        prompt_tokens = prompt_tokens[: self._max_token_length - 2]
-
-        # Calculate space left for label tokens
-        label_tokens_length = self._max_token_length - len(prompt_tokens)
-        label_tokens = self._tokenizer.encode(label, add_bos=False, add_eos=True)
-
-        # Truncate label tokens
-        label_tokens = label_tokens[: label_tokens_length - 1]
-        if label_tokens[-1] != self._tokenizer.eos_id:
-            label_tokens.append(self._tokenizer.eos_id)
-
-        input = prompt_tokens + label_tokens
-        label = [
-            CROSS_ENTROPY_IGNORE_IDX for _ in range(len(prompt_tokens))
-        ] + label_tokens
-        return input, label
-
-    def _generate_prompt_label(self, data: List[Dict[str, str]]) -> Tuple[str, str]:
-        """
-        Construct prompt and label strings adhering to Llama2 Chat Format.
-        This method supports only back-and-forth conversation per sample (as it is sufficient for SlimOrca dataset).
-        """
-        agent_text_dict = {}
-        # agents can be {system, human, gpt}
-        for conversation in data:
-            agent = conversation["from"]
-            text = conversation["value"]
-            agent_text_dict[agent] = text
-
-        # Llama2 Chat Format - https://github.com/facebookresearch/llama/blob/main/llama/generation.py#L284
-        if "system" in agent_text_dict:
-            prompt = f"{_Llama2ChatFormatConstants.B_INST} {_Llama2ChatFormatConstants.B_SYS}{agent_text_dict['system']}{_Llama2ChatFormatConstants.E_SYS}{agent_text_dict['human']} {_Llama2ChatFormatConstants.E_INST}"  # noqa: B950
-        else:
-            prompt = f"{_Llama2ChatFormatConstants.B_INST} {agent_text_dict['human']} {_Llama2ChatFormatConstants.E_INST}"
-
-        response = f" {agent_text_dict['gpt']} "
-        return prompt, response
+    """
+    if max_seq_len < 4:
+        # Input token needs to have 1 bos, 1 eos,
+        # and 1 token from prompt, 1 from label
+        raise ValueError("max_seq_len must be at least 4")
+
+    return ChatDataset(
+        tokenizer=tokenizer,
+        source=source,
+        convert_to_messages=sharegpt_to_llama2_messages,
+        chat_format=Llama2ChatFormat,
+        max_seq_len=max_seq_len,
+        train_on_input=train_on_input,
+        split="train",
+    )
```

## torchtune/models/__init__.py

```diff
@@ -1,7 +1,7 @@
 # Copyright (c) Meta Platforms, Inc. and affiliates.
 # All rights reserved.
 #
 # This source code is licensed under the BSD-style license found in the
 # LICENSE file in the root directory of this source tree.
 
-from torchtune.models import llama2  # noqa
+from torchtune.models import convert_weights, gemma, llama2, mistral  # noqa
```

## torchtune/models/llama2/__init__.py

```diff
@@ -2,25 +2,30 @@
 # All rights reserved.
 #
 # This source code is licensed under the BSD-style license found in the
 # LICENSE file in the root directory of this source tree.
 
 from ._checkpoint_utils import convert_llama2_fair_format
 from ._component_builders import llama2, lora_llama2
-from ._convert_weights import (  # noqa
-    hf_to_tune_llama2_7b,
-    meta_to_tune_llama2_7b,
-    tune_to_hf_llama2_7b,
-    tune_to_meta_llama2_7b,
+
+from ._model_builders import (  # noqa
+    llama2_13b,
+    llama2_7b,
+    llama2_tokenizer,
+    lora_llama2_13b,
+    lora_llama2_7b,
+    qlora_llama2_13b,
+    qlora_llama2_7b,
 )
-from ._model_builders import llama2_7b, llama2_tokenizer, lora_llama2_7b
 from ._model_utils import scale_hidden_dim_for_mlp
 
 __all__ = [
     "convert_llama2_fair_format",
     "llama2",
     "llama2_7b",
     "llama2_tokenizer",
     "lora_llama2",
     "lora_llama2_7b",
+    "qlora_llama2_7b",
+    "qlora_llama2_13b",
     "scale_hidden_dim_for_mlp",
 ]
```

## torchtune/models/llama2/_component_builders.py

```diff
@@ -1,30 +1,32 @@
 # Copyright (c) Meta Platforms, Inc. and affiliates.
 # All rights reserved.
 #
 # This source code is licensed under the BSD-style license found in the
 # LICENSE file in the root directory of this source tree.
+
+from functools import partial
 from typing import List, Optional
+from torchtune.modules.common_utils import reparametrize_as_dtype_state_dict_post_hook
 
 from torch import nn
 
 from torchtune.models.llama2._model_utils import scale_hidden_dim_for_mlp
 
 from torchtune.modules import (
     CausalSelfAttention,
     FeedForward,
-    KVCache,
     RMSNorm,
     RotaryPositionalEmbeddings,
     TransformerDecoder,
     TransformerDecoderLayer,
 )
 
-from torchtune.modules.peft import LoRALinear, LORA_ATTN_MODULES
 
+from torchtune.modules.peft import LORA_ATTN_MODULES, LoRALinear
 
 """
 Component builders for the Llama2 model and popular variants such as LoRA.
 
 TorchTune provides composable building blocks. Builder functions help
 stitch these building blocks into higher-level components. This design has
 two benefits:
@@ -33,24 +35,24 @@
 - Builder functions expose a set of configurable params which keep the constructors of
 the building blocks simple.
 """
 
 
 # ------------------ Vanilla Llama2 ------------------
 
+
 def llama2(
     vocab_size: int,
     num_layers: int,
     num_heads: int,
     num_kv_heads: int,
     embed_dim: int,
     max_seq_len: int,
     attn_dropout: float = 0.0,
     intermediate_dim: Optional[int] = None,
-    max_batch_size: Optional[int] = None,
     norm_eps: float = 1e-5,
 ) -> TransformerDecoder:
     """
     Build the decoder assoicated with the Llama2 model. This includes:
     - Token embeddings
     - num_layers number of TransformerDecoderLayer blocks
     - RMS Norm layer applied to the output of the transformer
@@ -67,76 +69,71 @@
         embed_dim (int): embedding dimension for self-attention
         max_seq_len (int): maximum sequence length the model will be run with, as used
             by :func:`~torchtune.modules.KVCache`
         attn_dropout (float): dropout value passed onto scaled_dot_product_attention.
             Default: 0.0
         intermediate_dim (Optional[int]): intermediate dimension for MLP. If not specified,
             this is computed using :func:`~torchtune.modules.scale_hidden_dim_for_mlp`
-        max_batch_size (Optional[int]): maximum batch size to be passed to :func:`~torchtune.modules.KVCache`
         norm_eps (float): epsilon in RMS norms.
 
     Returns:
         TransformerDecoder: Instantiation of Llama2 model.
     """
     head_dim = embed_dim // num_heads
     num_kv_heads = num_kv_heads if num_kv_heads else num_heads
-    kv_cache = (
-        KVCache(
-            max_batch_size=max_batch_size,
-            max_seq_len=max_seq_len,
-            n_kv_heads=num_heads,
-            head_dim=head_dim,
-        )
-        if max_batch_size is not None
-        else None
-    )
+
     rope = RotaryPositionalEmbeddings(dim=head_dim, max_seq_len=max_seq_len)
     self_attn = CausalSelfAttention(
         embed_dim=embed_dim,
         num_heads=num_heads,
         num_kv_heads=num_kv_heads,
         head_dim=head_dim,
         q_proj=nn.Linear(embed_dim, num_heads * head_dim, bias=False),
         k_proj=nn.Linear(embed_dim, num_kv_heads * head_dim, bias=False),
         v_proj=nn.Linear(embed_dim, num_kv_heads * head_dim, bias=False),
         output_proj=nn.Linear(embed_dim, embed_dim, bias=False),
         pos_embeddings=rope,
-        kv_cache=kv_cache,
+        kv_cache=None,
         max_seq_len=max_seq_len,
         attn_dropout=attn_dropout,
     )
-    hidden_dim = intermediate_dim if intermediate_dim else scale_hidden_dim_for_mlp(embed_dim)
+    hidden_dim = (
+        intermediate_dim if intermediate_dim else scale_hidden_dim_for_mlp(embed_dim)
+    )
     mlp = llama2_mlp(dim=embed_dim, hidden_dim=hidden_dim)
     layer = TransformerDecoderLayer(
         attn=self_attn,
         mlp=mlp,
         sa_norm=RMSNorm(dim=embed_dim, eps=norm_eps),
         mlp_norm=RMSNorm(dim=embed_dim, eps=norm_eps),
     )
     tok_embeddings = nn.Embedding(vocab_size, embed_dim)
     output_proj = nn.Linear(embed_dim, vocab_size, bias=False)
     return TransformerDecoder(
         tok_embeddings=tok_embeddings,
         layer=layer,
         num_layers=num_layers,
+        max_seq_len=max_seq_len,
+        num_heads=num_heads,
+        head_dim=head_dim,
         norm=RMSNorm(embed_dim, eps=norm_eps),
         output=output_proj,
     )
 
+
 def llama2_mlp(dim: int, hidden_dim: int) -> FeedForward:
     """
     Build the MLP layer associated with the Llama model.
     """
     gate_proj = nn.Linear(dim, hidden_dim, bias=False)
     down_proj = nn.Linear(hidden_dim, dim, bias=False)
     up_proj = nn.Linear(dim, hidden_dim, bias=False)
     return FeedForward(gate_proj=gate_proj, down_proj=down_proj, up_proj=up_proj)
 
 
-
 # ------------------ LoRA Llama2 ------------------
 
 
 def lora_llama2(
     lora_attn_modules: List[LORA_ATTN_MODULES],
     apply_lora_to_mlp: bool = False,
     apply_lora_to_output: bool = False,
@@ -144,21 +141,23 @@
     # llama2 args
     vocab_size: int,
     num_layers: int,
     num_heads: int,
     num_kv_heads: int,
     embed_dim: int,
     max_seq_len: int,
+    intermediate_dim: Optional[int] = None,
     attn_dropout: float = 0.0,
-    max_batch_size: Optional[int] = None,
     norm_eps: float = 1e-5,
     # LoRA args
     lora_rank: int,
     lora_alpha: float,
     lora_dropout: float = 0.0,
+    # Quantization args
+    quantize_base: bool = False,
 ) -> TransformerDecoder:
     """
     Return a version of Llama2 (an instance of :func:`~torchtune.modules.TransformerDecoder`)
     with LoRA applied to some of the linear layers in its self-attention modules.
 
     Args:
         lora_attn_modules (List[LORA_ATTN_MODULES]): list of which linear layers
@@ -176,145 +175,113 @@
             user should ensure `num_heads` % `num_kv_heads` == 0. Default value is
             `None`, in which case this is the same as MHA
         embed_dim (int): embedding dimension for self-attention
         max_seq_len (int): maximum sequence length the model will be run with, as used
             by :func:`~torchtune.modules.KVCache`
         attn_dropout (float): dropout value passed onto scaled_dot_product_attention.
             Default: 0.0
-        max_batch_size (Optional[int]): maximum batch size to be passed to :func:`~torchtune.modules.KVCache`
+        intermediate_dim (Optional[int]): intermediate dimension for MLP. If not specified,
+            this is computed using :func:`~torchtune.modules.scale_hidden_dim_for_mlp`
         norm_eps (float): epsilon in RMS norms.
         lora_rank (int): rank of each low-rank approximation
         lora_alpha (float): scaling factor for the low-rank approximation
         lora_dropout (float): LoRA dropout probability. Default: 0.0
+        quantize_base: (bool): Whether to quantize base model weights or not. Only applied to base
+            weights within linear layers LoRA is applied to. The final output linear projection is not
+            supported for quantization currently.
 
     Returns:
         TransformerDecoder: Instantiation of Llama2 model with LoRA applied to
         a subset of the attention projections in each layer.
 
     """
 
     self_attn = lora_llama2_self_attention(
         lora_modules=lora_attn_modules,
         embed_dim=embed_dim,
         num_heads=num_heads,
         num_kv_heads=num_kv_heads,
         max_seq_len=max_seq_len,
         attn_dropout=attn_dropout,
-        max_batch_size=max_batch_size,
         lora_rank=lora_rank,
         lora_alpha=lora_alpha,
         lora_dropout=lora_dropout,
+        quantize_base=quantize_base,
     )
 
-    hidden_dim = scale_hidden_dim_for_mlp(embed_dim)
+    hidden_dim = (
+        intermediate_dim if intermediate_dim else scale_hidden_dim_for_mlp(embed_dim)
+    )
     if apply_lora_to_mlp:
         mlp = lora_llama2_mlp(
             dim=embed_dim,
             hidden_dim=hidden_dim,
             lora_rank=lora_rank,
             lora_alpha=lora_alpha,
+            quantize_base=quantize_base,
         )
     else:
         mlp = llama2_mlp(dim=embed_dim, hidden_dim=hidden_dim)
 
     layer = TransformerDecoderLayer(
         attn=self_attn,
         mlp=mlp,
         sa_norm=RMSNorm(dim=embed_dim, eps=norm_eps),
         mlp_norm=RMSNorm(dim=embed_dim, eps=norm_eps),
     )
 
     tok_embeddings = nn.Embedding(vocab_size, embed_dim)
 
+    # TODO: quantize_base is not applied to final output_proj currently.
     output_proj = (
         LoRALinear(embed_dim, vocab_size, rank=lora_rank, alpha=lora_alpha)
         if apply_lora_to_output
         else nn.Linear(embed_dim, vocab_size, bias=False)
     )
-    return TransformerDecoder(
+    model = TransformerDecoder(
         tok_embeddings=tok_embeddings,
         layer=layer,
         num_layers=num_layers,
+        max_seq_len=max_seq_len,
+        num_heads=num_heads,
+        head_dim=(embed_dim // num_heads),
         norm=RMSNorm(embed_dim, eps=norm_eps),
         output=output_proj,
     )
 
-
-def lora_llama2_layer(
-    lora_attn_modules: List[LORA_ATTN_MODULES],
-    apply_lora_to_mlp: bool = False,
-    apply_lora_to_output: bool = False,
-    *,
-    # llama2 args
-    vocab_size: int,
-    num_heads: int,
-    num_kv_heads: int,
-    embed_dim: int,
-    max_seq_len: int,
-    attn_dropout: float = 0.0,
-    max_batch_size: Optional[int] = None,
-    norm_eps: float = 1e-5,
-    # LoRA args
-    lora_rank: int,
-    lora_alpha: float,
-    lora_dropout: float = 0.0,
-):
-    """
-    Build the decoder layer for LoRA Llama2. This includes:
-    - The self attention layer which applies LoRA to the relevant layers
-    - MLP layer which applies LoRA to the relevant layers\
-    - Transformer Decoder Layer
-    """
-
-    self_attn = lora_llama2_self_attention(
-        lora_modules=lora_attn_modules,
-        embed_dim=embed_dim,
-        num_heads=num_heads,
-        num_kv_heads=num_kv_heads,
-        max_seq_len=max_seq_len,
-        attn_dropout=attn_dropout,
-        max_batch_size=max_batch_size,
-        lora_rank=lora_rank,
-        lora_alpha=lora_alpha,
-        lora_dropout=lora_dropout,
-    )
-
-    hidden_dim = scale_hidden_dim_for_mlp(embed_dim)
-    if apply_lora_to_mlp:
-        mlp = lora_llama2_mlp(
-            dim=embed_dim,
-            hidden_dim=hidden_dim,
-            lora_rank=lora_rank,
-            lora_alpha=lora_alpha,
+    if quantize_base:
+        # For QLoRA, we reparametrize 4-bit tensors to higher precision, and offload to CPU on the fly
+        # so as to not increase peak memory
+        model._register_state_dict_hook(
+            partial(
+                reparametrize_as_dtype_state_dict_post_hook,
+                # TODO this is clowny, figure out a better way to get what precision the rest
+                # of the model is in
+                dtype=tok_embeddings.weight.dtype,
+                offload_to_cpu=True,
+            )
         )
-    else:
-        mlp = llama2_mlp(dim=embed_dim, hidden_dim=hidden_dim)
 
-    layer = TransformerDecoderLayer(
-        attn=self_attn,
-        mlp=mlp,
-        sa_norm=RMSNorm(dim=embed_dim, eps=norm_eps),
-        mlp_norm=RMSNorm(dim=embed_dim, eps=norm_eps),
-    )
+    return model
 
 
 def lora_llama2_self_attention(
     lora_modules: List[LORA_ATTN_MODULES],
     *,
     # CausalSelfAttention args
     embed_dim: int,
     num_heads: int,
     num_kv_heads: int,
     max_seq_len: int,
     attn_dropout: float = 0.0,
-    max_batch_size: Optional[int] = None,
     # LoRA args
     lora_rank: int,
     lora_alpha: float,
     lora_dropout: float = 0.0,
+    quantize_base: bool = False,
 ) -> CausalSelfAttention:
     """
     Return an instance of :func:`~torchtune.modules.CausalSelfAttention` with LoRA
     applied to a subset of its linear layers
 
     Args:
         lora_modules (List[LORA_ATTN_MODULES]): list of which linear layers
@@ -326,18 +293,19 @@
         num_kv_heads (int): number of key and value heads. If specified,
             user should ensure `num_heads` % `num_kv_heads` == 0. Default value is
             `None`, in which case this is the same as MHA
         max_seq_len (int): maximum sequence length the model will be run with, as used
             by :func:`~torchtune.modules.KVCache`
         attn_dropout (float): dropout value passed onto scaled_dot_product_attention.
             Default: 0.0
-        max_batch_size (Optional[int]): maximum batch size to be passed to :func:`~torchtune.modules.KVCache`
         lora_rank (int): rank of each low-rank approximation
         lora_alpha (float): scaling factor for the low-rank approximation
         lora_dropout (float): LoRA dropout probability. Default: 0.0
+        quantize_base (bool): Whether to quantize base model parameters for linear layers
+            LoRA is being applied to. Default is ``False``.
 
     Returns:
         CausalSelfAttention: instantiation of self-attention module with LoRA
         applied to a subset of Q, K, V, output projections.
 
     Raises:
         ValueError: If lora_modules arg is an empty list
@@ -345,89 +313,107 @@
     if not lora_modules:
         raise ValueError(
             f"Must pass one or more of {LORA_ATTN_MODULES} as lora_modules"
         )
 
     head_dim = embed_dim // num_heads
     num_kv_heads = num_kv_heads if num_kv_heads else num_heads
-    kv_cache = (
-        KVCache(
-            max_batch_size=max_batch_size,
-            max_seq_len=max_seq_len,
-            n_kv_heads=num_heads,
-            head_dim=head_dim,
-        )
-        if max_batch_size is not None
-        else None
-    )
     q_proj = (
-        LoRALinear(embed_dim, num_heads * head_dim, rank=lora_rank, alpha=lora_alpha)
+        LoRALinear(
+            embed_dim,
+            num_heads * head_dim,
+            rank=lora_rank,
+            alpha=lora_alpha,
+            quantize_base=quantize_base,
+        )
         if "q_proj" in lora_modules
         else nn.Linear(embed_dim, num_heads * head_dim, bias=False)
     )
     k_proj = (
-        LoRALinear(embed_dim, num_kv_heads * head_dim, rank=lora_rank, alpha=lora_alpha)
+        LoRALinear(
+            embed_dim,
+            num_kv_heads * head_dim,
+            rank=lora_rank,
+            alpha=lora_alpha,
+            quantize_base=quantize_base,
+        )
         if "k_proj" in lora_modules
         else nn.Linear(embed_dim, num_kv_heads * head_dim, bias=False)
     )
     v_proj = (
-        LoRALinear(embed_dim, num_kv_heads * head_dim, rank=lora_rank, alpha=lora_alpha)
+        LoRALinear(
+            embed_dim,
+            num_kv_heads * head_dim,
+            rank=lora_rank,
+            alpha=lora_alpha,
+            quantize_base=quantize_base,
+        )
         if "v_proj" in lora_modules
         else nn.Linear(embed_dim, num_kv_heads * head_dim, bias=False)
     )
     output_proj = (
-        LoRALinear(embed_dim, embed_dim, rank=lora_rank, alpha=lora_alpha)
+        LoRALinear(
+            embed_dim,
+            embed_dim,
+            rank=lora_rank,
+            alpha=lora_alpha,
+            quantize_base=quantize_base,
+        )
         if "output_proj" in lora_modules
         else nn.Linear(embed_dim, embed_dim, bias=False)
     )
     rope = RotaryPositionalEmbeddings(dim=head_dim, max_seq_len=max_seq_len)
     self_attn = CausalSelfAttention(
         embed_dim=embed_dim,
         num_heads=num_heads,
         num_kv_heads=num_kv_heads,
         head_dim=head_dim,
         q_proj=q_proj,
         k_proj=k_proj,
         v_proj=v_proj,
         output_proj=output_proj,
         pos_embeddings=rope,
-        kv_cache=kv_cache,
+        kv_cache=None,
         max_seq_len=max_seq_len,
         attn_dropout=attn_dropout,
     )
     return self_attn
 
 
 def lora_llama2_mlp(
     *,
     dim: int,
     hidden_dim: int,
     lora_rank: int,
     lora_alpha: float,
     lora_dropout: float = 0.0,
+    quantize_base: bool = False,
 ) -> FeedForward:
     gate_proj = LoRALinear(
         in_dim=dim,
         out_dim=hidden_dim,
         rank=lora_rank,
         alpha=lora_alpha,
         dropout=lora_dropout,
+        quantize_base=quantize_base,
     )
     down_proj = LoRALinear(
         in_dim=hidden_dim,
         out_dim=dim,
         rank=lora_rank,
         alpha=lora_alpha,
         dropout=lora_dropout,
+        quantize_base=quantize_base,
     )
     up_proj = LoRALinear(
         in_dim=dim,
         out_dim=hidden_dim,
         rank=lora_rank,
         alpha=lora_alpha,
         dropout=lora_dropout,
+        quantize_base=quantize_base,
     )
     return FeedForward(
         gate_proj=gate_proj,
         down_proj=down_proj,
         up_proj=up_proj,
     )
```

## torchtune/models/llama2/_model_builders.py

```diff
@@ -1,49 +1,43 @@
 # Copyright (c) Meta Platforms, Inc. and affiliates.
 # All rights reserved.
 #
 # This source code is licensed under the BSD-style license found in the
 # LICENSE file in the root directory of this source tree.
-from typing import List, Optional
-
-from torch import nn
+from typing import List
+from functools import partial
 
 from torchtune.models.llama2._component_builders import llama2, lora_llama2
-from torchtune.models.llama2._model_utils import scale_hidden_dim_for_mlp
 
 from torchtune.modules import Tokenizer, TransformerDecoder
 from torchtune.modules.peft import LORA_ATTN_MODULES
 
 
 """
 Model builders build specific instantiations using component builders. For example
 the llama2_7b model builder uses the llama2 component builder to create the
 llama2 7B model.
 """
 
 
-def llama2_7b(max_batch_size: Optional[int] = None) -> TransformerDecoder:
+def llama2_7b() -> TransformerDecoder:
     """
-    Builder for creating a Llama2 model initialized w/ the default 7b parameter values.
-    From https://arxiv.org/abs/2307.09288, these default values are:
-
-    Args:
-        max_batch_size (Optional[int]): Maximum batch size to be passed to KVCache.
+    Builder for creating a Llama2 model initialized w/ the default 7b parameter values
+    from https://arxiv.org/abs/2307.09288
 
     Returns:
         TransformerDecoder: Instantiation of Llama2 7B model
     """
     return llama2(
         vocab_size=32_000,
         num_layers=32,
         num_heads=32,
         num_kv_heads=32,
         embed_dim=4096,
         max_seq_len=4096,
-        max_batch_size=max_batch_size,
         attn_dropout=0.0,
         norm_eps=1e-5,
     )
 
 
 def llama2_tokenizer(path: str) -> Tokenizer:
     tokenizer = Tokenizer.from_file(path)
@@ -54,18 +48,19 @@
 
 def lora_llama2_7b(
     lora_attn_modules: List[LORA_ATTN_MODULES],
     apply_lora_to_mlp: bool = False,
     apply_lora_to_output: bool = False,
     lora_rank: int = 8,
     lora_alpha: float = 16,
-    max_batch_size: Optional[int] = None,
+    lora_dropout: float = 0.05,
+    quantize_base: bool = False,
 ) -> TransformerDecoder:
     """
-    Builder for creating a Llama2 model with LoRA enabled.
+    Builder for creating a Llama2 7B model with LoRA enabled.
 
     The Llama2 defaults are the same as in :func:`~torchtune.models.llama2.llama2_7b`,
     while LoRA default params are based on
     https://github.com/tloen/alpaca-lora/blob/8bb8579e403dc78e37fe81ffbb253c413007323f/finetune.py#L41-L43.
 
     Args:
         lora_attn_modules (List[LORA_ATTN_MODULES]): list of which linear layers
@@ -73,29 +68,111 @@
             ``{"q_proj", "k_proj", "v_proj", "output_proj"}``.
         apply_lora_to_mlp (bool): whether to apply LoRA to the MLP in each transformer layer.
             Default: False
         apply_lora_to_output (bool): whether to apply LoRA to the model's final output projection.
             Default: False
         lora_rank (int): rank of each low-rank approximation
         lora_alpha (float): scaling factor for the low-rank approximation
-        max_batch_size (Optional[int]): Maximum batch size to be passed to KVCache.
+        quantize_base (bool): Whether to quantize base model weights
 
     Returns:
         TransformerDecoder: Instantiation of Llama2 7B model with LoRA applied
     """
     return lora_llama2(
         lora_attn_modules=lora_attn_modules,
         apply_lora_to_mlp=apply_lora_to_mlp,
         apply_lora_to_output=apply_lora_to_output,
         vocab_size=32_000,
         num_layers=32,
         num_heads=32,
         num_kv_heads=32,
         embed_dim=4096,
         max_seq_len=4096,
-        max_batch_size=max_batch_size,
         attn_dropout=0.0,
         norm_eps=1e-5,
         lora_rank=lora_rank,
         lora_alpha=lora_alpha,
         lora_dropout=0.05,
+        quantize_base=quantize_base,
+    )
+
+qlora_llama2_7b = partial(lora_llama2_7b, quantize_base=True)
+
+qlora_llama2_7b.__doc__ = """
+Builder for creating a Llama2 model with QLoRA enabled. Base model weights in linear layers
+that LoRA is applied to are quantized per the QLoRA paper: https://arxiv.org/abs/2305.14314.
+Please see `lora_llama2_7b` for full API arguments.
+"""
+
+
+def llama2_13b() -> TransformerDecoder:
+    """
+    Builder for creating a Llama2 model initialized w/ the default 13b parameter values
+    from https://arxiv.org/abs/2307.09288
+
+    Returns:
+        TransformerDecoder: Instantiation of Llama2 13B model
+    """
+    return llama2(
+        vocab_size=32_000,
+        num_layers=40,
+        num_heads=40,
+        num_kv_heads=40,
+        embed_dim=5120,
+        intermediate_dim=13824,
+        max_seq_len=4096,
+        attn_dropout=0.0,
+        norm_eps=1e-5,
+    )
+
+
+def lora_llama2_13b(
+    lora_attn_modules: List[LORA_ATTN_MODULES],
+    apply_lora_to_mlp: bool = False,
+    apply_lora_to_output: bool = False,
+    lora_rank: int = 8,
+    lora_alpha: float = 16,
+    quantize_base: bool = False,
+) -> TransformerDecoder:
+    """
+    Builder for creating a Llama2 13B model with LoRA enabled.
+
+    The Llama2 defaults are the same as in :func:`~torchtune.models.llama2.llama2_13b`,
+    while LoRA default params are based on
+    https://github.com/tloen/alpaca-lora/blob/8bb8579e403dc78e37fe81ffbb253c413007323f/finetune.py#L41-L43.
+
+    Args:
+        lora_attn_modules (List[LORA_ATTN_MODULES]): list of which linear layers
+            LoRA should be applied to in each self-attention block. Options are
+            ``{"q_proj", "k_proj", "v_proj", "output_proj"}``.
+        apply_lora_to_mlp (bool): whether to apply LoRA to the MLP in each transformer layer.
+            Default: False
+        apply_lora_to_output (bool): whether to apply LoRA to the model's final output projection.
+            Default: False
+        lora_rank (int): rank of each low-rank approximation
+        lora_alpha (float): scaling factor for the low-rank approximation
+        quantize_base (bool): Whether to quantize base model weights
+
+    Returns:
+        TransformerDecoder: Instantiation of Llama2 13B model with LoRA applied
+    """
+
+    return lora_llama2(
+        lora_attn_modules=lora_attn_modules,
+        apply_lora_to_mlp=apply_lora_to_mlp,
+        apply_lora_to_output=apply_lora_to_output,
+        vocab_size=32_000,
+        num_layers=40,
+        num_heads=40,
+        num_kv_heads=40,
+        embed_dim=5120,
+        max_seq_len=4096,
+        intermediate_dim=13824,
+        attn_dropout=0.0,
+        norm_eps=1e-5,
+        lora_rank=lora_rank,
+        lora_alpha=lora_alpha,
+        lora_dropout=0.05,
+        quantize_base=quantize_base,
     )
+
+qlora_llama2_13b = partial(lora_llama2_13b, quantize_base=True)
```

## torchtune/modules/__init__.py

```diff
@@ -1,14 +1,15 @@
 # Copyright (c) Meta Platforms, Inc. and affiliates.
 # All rights reserved.
 #
 # This source code is licensed under the BSD-style license found in the
 # LICENSE file in the root directory of this source tree.
 
 from .attention import CausalSelfAttention  # noqa
+from .common_utils import reparametrize_as_dtype_state_dict_post_hook
 from .feed_forward import FeedForward  # noqa
 from .kv_cache import KVCache  # noqa
 from .lr_schedulers import get_cosine_schedule_with_warmup  # noqa
 from .position_embeddings import RotaryPositionalEmbeddings  # noqa
 from .rms_norm import RMSNorm  # noqa
 from .tokenizer import Tokenizer  # noqa
 from .transformer import TransformerDecoder, TransformerDecoderLayer  # noqa
@@ -19,8 +20,9 @@
     "get_cosine_schedule_with_warmup",
     "KVCache",
     "RotaryPositionalEmbeddings",
     "RMSNorm",
     "Tokenizer",
     "TransformerDecoder",
     "TransformerDecoderLayer",
+    "reparametrize_as_dtype_state_dict_post_hook",
 ]
```

## torchtune/modules/attention.py

```diff
@@ -118,22 +118,24 @@
         self.output_proj = output_proj
         self.pos_embeddings = pos_embeddings
 
     def forward(
         self,
         x: Tensor,
         mask: Optional[Tensor] = None,
-        curr_pos: int = 0,
+        input_pos: Optional[Tensor] = None,
     ) -> Tensor:
         """
         Args:
             x (Tensor): input tensor with shape
                 [batch_size x seq_length x embed_dim]
-            mask (Optional[Tensor]): boolean mask, defaults to None.
-            curr_pos (int): current position in the sequence, defaults to 0.
+            mask (Optional[Tensor]): Optional tensor which contains the mask.
+                Only used during inference. Default is None.
+            input_pos (Optional[Tensor]): Optional tensor which contains the position
+                of the current token. This is only used during inference. Default is None
 
         Returns:
             Tensor: output tensor with attention applied
 
         Raises:
             ValueError: if seq_len of x is bigger than max_seq_len
 
@@ -145,15 +147,14 @@
             - d: embed dim
             - h_d: head dim
 
         TODO:
             - Return the attention weights
             - Make application of positional embeddings optional
         """
-
         # input has shape [b, s, d]
         bsz, seq_len, _ = x.shape
 
         if seq_len > self.max_seq_len:
             raise ValueError(
                 f"seq_len ({seq_len}) of input tensor should be smaller "
                 f"than max_seq_len ({self.max_seq_len})"
@@ -186,28 +187,26 @@
         # [b, s, n_h, h_d]
         # Reshape the tensors before we apply RoPE
         q = q.reshape(bsz, seq_len, -1, self.head_dim)
         k = k.reshape(bsz, seq_len, -1, self.head_dim)
         v = v.reshape(bsz, seq_len, -1, self.head_dim)
 
         # Apply positional embeddings
-        q = self.pos_embeddings(q, curr_pos)
-        k = self.pos_embeddings(k, curr_pos)
-
-        # Update key-value cache
-        if self.kv_cache is not None:
-            k, v = self.kv_cache.update(
-                bsz=bsz, seq_len=seq_len, curr_pos=curr_pos, k_val=k, v_val=v
-            )
+        q = self.pos_embeddings(q, input_pos)
+        k = self.pos_embeddings(k, input_pos)
 
         # [b, n_h, s, h_d]
         q = q.transpose(1, 2)
         k = k.transpose(1, 2)
         v = v.transpose(1, 2)
 
+        # Update key-value cache
+        if self.kv_cache is not None:
+            k, v = self.kv_cache.update(input_pos, k, v)
+
         # Flash attention from https://pytorch.org/blog/accelerating-large-language-models/
         output = nn.functional.scaled_dot_product_attention(
             q,
             k,
             v,
             attn_mask=mask,
             dropout_p=self.attn_dropout,
```

## torchtune/modules/feed_forward.py

```diff
@@ -1,36 +1,37 @@
 # Copyright (c) Meta Platforms, Inc. and affiliates.
 # All rights reserved.
 #
 # This source code is licensed under the BSD-style license found in the
 # LICENSE file in the root directory of this source tree.
 
-import torch.nn.functional as F
 from torch import nn, Tensor
 
 
 class FeedForward(nn.Module):
     """This class implements the feed-forward network derived from Llama2.
 
     Args:
         gate_proj (nn.Module): Projection from input dim to hidden dim, fed through activation
             and multiplied by up_proj.
         down_proj (nn.Module): Final projection to output dim.
         up_proj (nn.Module): Projection from input dim to hidden dim, multiplied by
             activation(gate_proj).
+        activation (nn.Module): Activation function to use. Default is nn.SiLU().
     """
 
     def __init__(
         self,
         *,
         gate_proj: nn.Module,
         down_proj: nn.Module,
         up_proj: nn.Module,
+        activation: nn.Module = nn.SiLU(),
     ):
         super().__init__()
         self.w1 = gate_proj
         self.w2 = down_proj
         self.w3 = up_proj
-        self.activation = F.silu
+        self.activation = activation
 
     def forward(self, x: Tensor) -> Tensor:
         return self.w2(self.activation(self.w1(x)) * self.w3(x))
```

## torchtune/modules/kv_cache.py

```diff
@@ -13,54 +13,42 @@
 class KVCache(nn.Module):
     """
     Standalone nn.Module containing a kv-cache to cache past key and values during inference.
 
     Args:
         max_batch_size (int): maximum batch size model will be run with
         max_seq_len (int): maximum sequence length model will be run with
-        n_kv_heads (int): number of kv heads
+        num_heads (int): number of heads. We take num_heads instead of num_kv_heads because
+            the cache is created after we've expanded the key and value tensors to have the
+            same shape as the query tensor. See attention.py for more details
         head_dim (int): per-attention head embedding dimension
+        dtype (torch.dtype): dtype for the caches
     """
 
     def __init__(
         self,
         max_batch_size: int,
         max_seq_len: int,
-        n_kv_heads: int,
+        num_heads: int,
         head_dim: int,
-    ):
+        dtype: torch.dtype,
+    ) -> None:
         super().__init__()
-        cache_shape = (max_batch_size, max_seq_len, n_kv_heads, head_dim)
-        self.register_buffer("k_cache", torch.zeros(cache_shape), persistent=False)
-        self.register_buffer("v_cache", torch.zeros(cache_shape), persistent=False)
+        cache_shape = (max_batch_size, num_heads, max_seq_len, head_dim)
+        self.register_buffer(
+            "k_cache", torch.zeros(cache_shape, dtype=dtype), persistent=False
+        )
+        self.register_buffer(
+            "v_cache", torch.zeros(cache_shape, dtype=dtype), persistent=False
+        )
         self.max_batch_size = max_batch_size
 
-    def update(
-        self, bsz: int, seq_len: int, curr_pos: int, k_val: Tensor, v_val: Tensor
-    ) -> Tuple[Tensor, Tensor]:
-        """
-        Updates the kv-cache at curr_pos with the given k_val and v_val.
-
-        Args:
-            bsz (int): Batch size.
-            seq_len (int): Sequence length.
-            curr_pos (int): Current position in sequence.
-            k_val (Tensor): New k value.
-            v_val (Tensor): New v value.
+    def update(self, input_pos, k_val, v_val) -> Tuple[Tensor, Tensor]:
+        # input_pos: [S], k_val: [B, H, S, D]
+        assert input_pos.shape[0] == k_val.shape[2]
+
+        k_out = self.k_cache
+        v_out = self.v_cache
+        k_out[:, :, input_pos] = k_val
+        v_out[:, :, input_pos] = v_val
 
-        Raises:
-            ValueError: if bsz is greater than the ``max_batch_size`` supported by the model
-
-        Returns:
-            Tuple[Tensor, Tensor]: the key-cache and value-cache
-        """
-        if bsz > self.max_batch_size:
-            raise ValueError(
-                f"Batch size {bsz} greater than max batch size {self.max_batch_size}"
-            )
-
-        self.k_cache[:bsz, curr_pos : curr_pos + seq_len] = k_val
-        self.v_cache[:bsz, curr_pos : curr_pos + seq_len] = v_val
-        return (
-            self.k_cache[:bsz, : curr_pos + seq_len],
-            self.v_cache[:bsz, : curr_pos + seq_len],
-        )
+        return k_out, v_out
```

## torchtune/modules/lr_schedulers.py

```diff
@@ -18,15 +18,15 @@
     last_epoch: int = -1,
 ) -> LambdaLR:
     """
     Create a learning rate schedule that linearly increases the learning rate from
     0.0 to lr over num_warmup_steps, then decreases to 0.0 on a cosine schedule over
     the remaining num_training_steps-num_warmup_steps (assuming num_cycles = 0.5).
 
-    This is based on the HuggingFace implementation
+    This is based on the Hugging Face implementation
     https://github.com/huggingface/transformers/blob/v4.23.1/src/transformers/optimization.py#L104.
 
     Args:
         optimizer (torch.optim.Optimizer): The optimizer for which to
             schedule the learning rate.
         num_warmup_steps (int): The number of steps for the warmup phase.
         num_training_steps (int): The total number of training steps.
```

## torchtune/modules/position_embeddings.py

```diff
@@ -1,13 +1,15 @@
 # Copyright (c) Meta Platforms, Inc. and affiliates.
 # All rights reserved.
 #
 # This source code is licensed under the BSD-style license found in the
 # LICENSE file in the root directory of this source tree.
 
+from typing import Optional
+
 import torch
 
 from torch import nn, Tensor
 
 
 class RotaryPositionalEmbeddings(nn.Module):
     """
@@ -66,20 +68,21 @@
         idx_theta = torch.einsum("i, j -> ij", seq_idx, self.theta).float()
 
         # cache includes both the cos and sin components and so the output shape is
         # [max_seq_len, dim // 2, 2]
         cache = torch.stack([torch.cos(idx_theta), torch.sin(idx_theta)], dim=-1)
         self.register_buffer("cache", cache, persistent=False)
 
-    def forward(self, x: Tensor, curr_pos: int = 0) -> Tensor:
+    def forward(self, x: Tensor, input_pos: Optional[Tensor] = None) -> Tensor:
         """
         Args:
             x (Tensor): input tensor with shape
                 [bsz, seq_len, num_heads, head_dim]
-            curr_pos (int): current position in the sequence, defualts to 0.
+            input_pos (Optional[Tensor]): Optional tensor which contains the position
+                of the current token. This is only used during inference. Default is None
 
         Returns:
             Tensor: output tensor with RoPE applied
 
         Notation used for tensor shapes:
             - b: batch size
             - s: sequence length
@@ -87,15 +90,20 @@
             - h_d: head dim
 
         TODO: The implementation below can be made more efficient
         for inference.
         """
         # input tensor has shape [b, s, n_h, n_d]
         seq_len = x.size(1)
-        rope_cache = self.cache[curr_pos : curr_pos + seq_len]
+
+        # extract the values based on whether input_pos is set or not. When
+        # input_pos is provided, we're in inference mode
+        rope_cache = (
+            self.cache[:seq_len] if input_pos is None else self.cache[input_pos]
+        )
 
         # reshape input; the last dimension is used for computing the output.
         # Cast to float to match the reference implementation
         # tensor has shape [b, s, n_h, n_d // 2, 2]
         xshaped = x.float().reshape(*x.shape[:-1], -1, 2)
 
         # reshape the cache for broadcasting
```

## torchtune/modules/tokenizer.py

```diff
@@ -1,16 +1,20 @@
 # Copyright (c) Meta Platforms, Inc. and affiliates.
 # All rights reserved.
 #
 # This source code is licensed under the BSD-style license found in the
 # LICENSE file in the root directory of this source tree.
 
-from typing import List
+from typing import List, Optional, Tuple
 
 from sentencepiece import SentencePieceProcessor
+from torchtune.data._types import Message
+from torchtune.data._utils import truncate
+
+WHITESPACE_CHARS = [" ", "\n", "\t", "\r", "\v"]
 
 
 class Tokenizer:
     """A wrapper around SentencePieceProcessor.
 
     Args:
         spm_model (SentencePieceProcessor): The SentencePiece model.
@@ -37,14 +41,21 @@
     ):
         self.spm_model = spm_model
         self.vocab_size = vocab_size
         self.bos_id = bos_id
         self.eos_id = eos_id
         self.pad_id = pad_id
 
+        # This is used in tokenize_messages: if the tokenizer does not
+        # encode whitespace, then we can more easily split strings
+        # on whitespace characters and encode them separately.
+        self.encodes_whitespace = any(
+            [self.spm_model.encode(c) for c in WHITESPACE_CHARS]
+        )
+
     @classmethod
     def from_file(cls, path: str) -> "Tokenizer":
         """Initialize a `Tokenizer` instance from a SentencePiece model file.
 
         Args:
             path (str): The path to the SentencePiece model file.
 
@@ -56,36 +67,150 @@
         return cls(spm, spm.vocab_size(), spm.bos_id(), spm.eos_id(), spm.pad_id())
 
     def encode(
         self,
         text: str,
         add_bos: bool = True,
         add_eos: bool = True,
+        trim_leading_whitespace: bool = False,
+        prefix: Optional[str] = None,
     ) -> List[int]:
         """Encode text into token IDs.
 
         Args:
             text (str): The input text to be encoded, unbatched.
             add_bos (bool): Whether to prepend BOS to the input, defaults to True.
             add_eos (bool): Whether to append EOS to the input, defaults to True.
-
+            trim_leading_whitespace (bool): Whether to trim leading whitespace from
+                underlying sentencepiece tokenization. Sentencepiece normally prepends
+                whitespace to any tokenized text, which can cause differences where
+                encode(s1) + encode(s2) != encode(s1 + s2) due to leading whitespace
+                added to s2. Default: False
+            prefix (Optional[str]): Optional string to encode for trimming leading
+                whitespaces. Used only if trim_leading_whitespace=True. Default: None
         Returns:
             List[int]: The encoded token IDs.
         """
-        assert type(text) == str, f"Expected string but got {type(text)}"
-        return self.spm_model.encode(
-            text,
-            add_bos=add_bos,
-            add_eos=add_eos,
-            out_type=int,
-        )
+        if trim_leading_whitespace:
+            # Can define our own custom prefix depending on vocab if needed
+            if not hasattr(self, "prefix"):
+                self.prefix = prefix or "\n"
+                self.encoded_prefix = self.spm_model.encode(
+                    self.prefix, add_bos=False, add_eos=False
+                )
+            start_idx = len(self.encoded_prefix) + int(add_bos)
+            return self.spm_model.encode(
+                self.prefix + text,
+                add_bos=add_bos,
+                add_eos=add_eos,
+                out_type=int,
+            )[start_idx:]
+        else:
+            return self.spm_model.encode(
+                text,
+                add_bos=add_bos,
+                add_eos=add_eos,
+                out_type=int,
+            )
 
     def decode(self, ids: List[int]) -> str:
         """Decode token IDs to strings.
 
         Args:
             ids (List[int]): The input token IDs to be decoded.
 
         Returns:
             str: The decoded text.
         """
         return self.spm_model.decode(ids)
+
+    def tokenize_messages(
+        self, messages: List[Message], max_seq_len: Optional[int] = None
+    ) -> Tuple[List[int], List[bool]]:
+        r"""Tokenize a list of messages one at a time then concatenate them,
+        returning a list of tokens and a list of masks.
+
+        Note: llama2 sentencepiece has problems where in general
+        encode(s1 + s2) != encode(s1) + encode(s2) due to whitespace handling.
+        We can get around this by prepending s2 with a known token and slicing the
+        beginning off the tokenized s2.
+
+        Example:
+            >>> tokenizer = Tokenizer.from_file(tokenizer_path)
+            >>> messages = [
+                Message(role="system", content="system message\n", masked=True),
+                Message(role="user", content="user prompt\n", masked=True),
+                Message(role="assistant", content="assistant response\n"),
+                ]
+            # tokenize_messages encodes messages separately and concats
+            >>> tokenizer.tokenize_messages(messages, max_seq_len)[0]
+            [1, 1788, 2643, 13, 1792, 9508, 13, 465, 22137, 2933, 2]
+
+
+            # Same result as encoding the full string in one go
+            >>> tokenizer.encode(''.join([message.content for message in messages]))
+            [1, 1788, 2643, 13, 1792, 9508, 13, 465, 22137, 2933, 2]
+
+
+        Args:
+            messages (List[Message]): A list of messages, each containing role, content,
+                and masked attributes.
+            max_seq_len (Optional[int]): A max sequence length to truncate tokens to.
+                Default: None
+
+        Returns:
+            Tuple[List[int], List[bool]]: The tokenized messages
+        """
+        start_of_turn = True
+        end_of_turn = False
+        prev_ends_with_space = False
+        tokenized_messages = []
+        mask = []
+        for message in messages:
+            # If assistant message, this is the end of a turn
+            end_of_turn = message.role == "assistant"
+
+            # Prepend BOS on start of new turns
+            if start_of_turn:
+                tokenized_messages.append(self.bos_id)
+                mask.append(message.masked)
+
+            # We want to trim leading whitespace on the next message when
+            # (a) it is a continuation of the turn (i.e. not the first message)
+            # (b) the vocabulary explicitly encodes whitespace characters, and
+            # (c) the previous message did not end with a space
+            trim_leading_whitespace = (
+                (not start_of_turn)
+                and self.encodes_whitespace
+                and not prev_ends_with_space
+            )
+
+            # Tokenize current message, append with masks
+            tokens = self.encode(
+                message.content.rstrip(" "),
+                add_bos=False,
+                add_eos=False,
+                trim_leading_whitespace=trim_leading_whitespace,
+            )
+            prev_ends_with_space = message.content.endswith(" ")
+            tokenized_messages.extend(tokens)
+            mask.extend([message.masked] * len(tokens))
+
+            # If assistant message, append EOS at end
+            if end_of_turn:
+                tokenized_messages.append(self.eos_id)
+                mask.append(message.masked)
+                end_of_turn = False
+                start_of_turn = True
+            else:
+                start_of_turn = False
+
+            # Break out early if we reach max_seq_len
+            if max_seq_len and len(tokenized_messages) >= max_seq_len:
+                break
+
+        # Finally, truncate if necessary
+        if max_seq_len:
+            tokenized_messages = truncate(tokenized_messages, max_seq_len, self.eos_id)
+            mask = truncate(mask, max_seq_len, message.masked)
+
+        return tokenized_messages, mask
```

## torchtune/modules/transformer.py

```diff
@@ -5,15 +5,15 @@
 # LICENSE file in the root directory of this source tree.
 import copy
 from typing import Optional
 
 import torch
 from torch import nn, Tensor
 
-from torchtune.modules import CausalSelfAttention
+from torchtune.modules import CausalSelfAttention, KVCache
 
 
 class TransformerDecoderLayer(nn.Module):
     """Transformer layer derived from the Llama2 model. Normalization is applied before the attention **and** FF layer.
 
     Args:
         attn (CausalSelfAttention): Attention module.
@@ -35,22 +35,24 @@
         self.mlp_norm = mlp_norm
         self.mlp = mlp
 
     def forward(
         self,
         x: Tensor,
         mask: Optional[Tensor] = None,
-        curr_pos: int = 0,
+        input_pos: Optional[Tensor] = None,
     ) -> Tensor:
         """
         Args:
             x (Tensor): input tensor with shape
                 [batch_size x seq_length x embed_dim]
-            mask (Optional[Tensor]): mask tensor, defaults to None.
-            curr_pos (int): current position in the seq, defaults to 0.
+            mask (Optional[Tensor]): Optional tensor which contains the mask.
+                Only used during inference. Default is None.
+            input_pos (Optional[Tensor]): Optional tensor which contains the position
+                of the current token. This is only used during inference. Default is None
 
         Returns:
             Tensor: output tensor with same shape as input
                 [batch_size x seq_length x embed_dim]
 
         Notation used for tensor shapes:
             - b: batch size
@@ -59,15 +61,15 @@
 
         TODO:
             - Make position of norm configurable
         """
         # Input tensor and attention output have the same shape
         # [b, s, d]
         # Norm applied before self-attention
-        attn_out = self.attn(self.sa_norm(x), mask, curr_pos)
+        attn_out = self.attn(self.sa_norm(x), mask, input_pos)
 
         # Residual connection; shape: [b, s, d]
         h = attn_out + x
 
         # Norm applied before the feedforward layer
         mlp_out = self.mlp(self.mlp_norm(h))
 
@@ -92,75 +94,118 @@
 
 
 class TransformerDecoder(nn.Module):
     """
     Transformer Decoder derived from the Llama2 architecture.
 
     Args:
-        tok_embeddings (nn.Embedding): PyTorch embedding layer, to be used to move tokens to an embedding space.
+        tok_embeddings (nn.Embedding): PyTorch embedding layer, to be used to move
+            tokens to an embedding space.
         layer (TransformerDecoderLayer): Transformer Decoder layer.
         num_layers (int): Number of Transformer Decoder layers.
-        norm (nn.Module): Callable that applies normalization to the output of the decoder, before final MLP.
-        output (nn.Linear): Callable that applies a linear transformation to the output of the decoder.
+        max_seq_len (int): maximum sequence length the model will be run with, as used
+            by :func:`~torchtune.modules.KVCache`
+        num_heads (int): number of query heads. For MHA this is also the
+            number of heads for key and value. This is used to setup the
+            :func:`~torchtune.modules.KVCache`
+        head_dim (int): embedding dimension for each head in self-attention. This is used
+            to setup the :func:`~torchtune.modules.KVCache`
+        norm (nn.Module): Callable that applies normalization to the output of the decoder,
+            before final MLP.
+        output (nn.Linear): Callable that applies a linear transformation to the output of
+            the decoder.
 
     Note:
         Arg values are checked for correctness (eg: ``attn_dropout`` belongs to [0,1])
         in the module where they are used. This helps reduces the number of raise
         statements in code and improves readability.
     """
 
     def __init__(
         self,
         tok_embeddings: nn.Embedding,
         layer: TransformerDecoderLayer,
         num_layers: int,
+        max_seq_len: int,
+        num_heads: int,
+        head_dim: int,
         norm: nn.Module,
         output: nn.Linear,
     ) -> None:
         super().__init__()
+
         self.tok_embeddings = tok_embeddings
         self.layers = _get_clones(layer, num_layers)
         self.norm = norm
         self.output = output
+        self.max_seq_len = max_seq_len
+        self.num_heads = num_heads
+        self.head_dim = head_dim
+        self.causal_mask = None
 
-    def forward(
-        self, tokens: Tensor, mask: Optional[Tensor] = None, curr_pos: int = 0
-    ) -> Tensor:
+    def setup_caches(self, max_batch_size: int, dtype: torch.dtype) -> None:
+        for layer in self.layers:
+            layer.attn.kv_cache = KVCache(
+                max_batch_size=max_batch_size,
+                max_seq_len=self.max_seq_len,
+                num_heads=self.num_heads,
+                head_dim=self.head_dim,
+                dtype=dtype,
+            )
+
+        # causal_mask is used during inference to ensure we're attending
+        # to the right tokens
+        self.causal_mask = torch.tril(
+            torch.ones(self.max_seq_len, self.max_seq_len, dtype=torch.bool)
+        )
+
+    def forward(self, tokens: Tensor, input_pos: Optional[Tensor] = None) -> Tensor:
         """
         Args:
             tokens (Tensor): input tensor with shape [b x s]
-            mask (Optional[Tensor]): attention mask tensor, defaults to None.
-            curr_pos (int): current position in the seq, defaults to 0.
-                Only relevant when incrementally decoding.
+            input_pos (Optional[Tensor]): Optional tensor which contains the position
+                of the current token. This is only used during inference. Default is None
+
+        Note: At the very first step of inference, when the model is provided with a prompt,
+        ``input_pos`` would contain the positions of all of the tokens in the prompt
+        (eg: ``torch.arange(prompt_length)``). This is because we will need to compute the
+        KV values for each position.
 
         Returns:
             Tensor: output tensor with shape [b x s x v]
 
+        Raises:
+            ValueError: if causal_mask is set but input_pos is None
+
         Notation used for tensor shapes:
             - b: batch size
             - s: sequence length
             - v: vocab size
             - d: embed dim
+            - m_s: max seq len
         """
         # input tensor of shape [b, s]
         bsz, seq_len = tokens.shape
 
         # shape: [b, s, d]
         h = self.tok_embeddings(tokens)
 
-        # TODO: Fix the masking logic to not rely on checking kv_cache
-        if seq_len > 1 and self.layers[0].attn.kv_cache is not None:
-            mask = torch.full(
-                (1, 1, seq_len, seq_len), float("-inf"), device=tokens.device
-            )
-            mask = torch.triu(mask, diagonal=curr_pos + 1)
+        mask = None
+        if self.causal_mask is not None:
+            if input_pos is None:
+                raise ValueError(
+                    "Caches are setup, but the position of input token is missing"
+                )
+            # shape: [1, input_pos_len, m_s]
+            # in most cases input_pos_len should be 1
+            mask = self.causal_mask[None, None, input_pos]
 
         for layer in self.layers:
             # shape: [b, s, d]
-            h = layer(h, mask, curr_pos)
+            h = layer(h, mask, input_pos)
 
         # shape: [b, s, d]
         h = self.norm(h)
 
         # shape: [b, s, v]
         output = self.output(h).float()
         return output
```

## torchtune/modules/peft/__init__.py

```diff
@@ -3,20 +3,23 @@
 #
 # This source code is licensed under the BSD-style license found in the
 # LICENSE file in the root directory of this source tree.
 
 from .lora import LoRALinear
 from .peft_utils import (  # noqa
     AdapterModule,
+    disable_adapter,
     get_adapter_params,
     LORA_ATTN_MODULES,
     set_trainable_params,
     validate_state_dict_for_lora,
 )
 
 __all__ = [
     "LoRALinear",
     "AdapterModule",
     "get_adapter_params",
     "set_trainable_params",
+    "validate_missing_and_unexpected_for_lora",
     "validate_state_dict_for_lora",
+    "disable_adapter",
 ]
```

## torchtune/modules/peft/lora.py

```diff
@@ -6,16 +6,17 @@
 import math
 from typing import List
 
 import torch.nn.functional as F
 
 from torch import nn, Tensor
 
+from torchao.dtypes.nf4tensor import linear_nf4, to_nf4
 from torchtune.modules.peft.peft_utils import AdapterModule
-from torchtune.utils.tensor_utils import _copy_tensor
+from torchtune.utils import _register_nf4_dispatch_ops  # noqa: F401
 
 
 class LoRALinear(nn.Module, AdapterModule):
     """LoRA linear layer as introduced in `LoRA: Low-Rank Adaptation of Large Language Models <https://arxiv.org/abs/2106.09685>`_.
 
     LoRA perturbs a given layer via a low-rank approximation where only
     the rank decomposition matrices are trainable. In a linear layer instead of
@@ -29,38 +30,44 @@
         in_dim (int): input dimension
         out_dim (int): output dimension
         rank (int): rank of the low-rank approximation
         alpha (float): scaling factor for the low-rank approximation
         dropout (float): dropout probability. Default: 0.0
         use_bias (bool): whether to include bias in the original linear layer.
             Default: False
+        quantize_base (bool): Whether to quantize base linear weight or not.
+            Default: False
     """
 
     def __init__(
         self,
         in_dim: int,
         out_dim: int,
         rank: int,
         alpha: float,
         dropout: float = 0.0,
         use_bias: bool = False,
+        quantize_base: bool = False,
     ):
         super().__init__()
         self.in_dim = in_dim
         self.rank = rank
         self.alpha = alpha
         self.out_dim = out_dim
-        linear = nn.Linear(in_features=in_dim, out_features=out_dim, bias=use_bias)
-        # Clone weight / bias directly into the LoRALinear, for 1:1 mapping with how Linear layers are used in
-        # vanilla Transformers.
-        self.register_parameter("weight", nn.Parameter(_copy_tensor(linear.weight)))
-        if use_bias:
-            self.register_parameter("bias", nn.Parameter(_copy_tensor(linear.bias)))
-        else:
-            self.register_parameter("bias", None)
+        self.use_bias = use_bias
+        self._quantize_base = quantize_base
+        weight, bias = self._create_weight_and_bias()
+        # 'self.disabled' is a flag showing whether to turn off LoRA adapters,
+        # this can be used in DPO for treating the lora adapters as the policy model
+        # and disabling it to treat the base model as the reference model
+        self.disabled = False
+        self.register_parameter("weight", nn.Parameter(weight))
+        self.register_parameter(
+            "bias", nn.Parameter(bias) if bias is not None else None
+        )
         self.dropout = nn.Dropout(p=dropout)
         self.lora_a = nn.Linear(in_features=in_dim, out_features=rank, bias=False)
         self.lora_b = nn.Linear(in_features=rank, out_features=out_dim, bias=False)
         self.merged = False
         # Note: FSDP's meta device initialization contract assumes that a module's
         # reset_parameters method only initializes its own parameters (i.e. no child
         # params are initialized, as is done in initialize_parameters below).
@@ -73,32 +80,56 @@
 
     def initialize_parameters(self):
         # Initialize as in
         # https://github.com/microsoft/LoRA/blob/4c0333854cb905966f8cc4e9a74068c1e507c7b7/loralib/layers.py#L119
         _lora_a_init_params(self.lora_a)
         _lora_b_init_params(self.lora_b)
 
+    def _create_weight_and_bias(self):
+        """
+        Creates a linear weight and bias tensor, using NF4 dtype if we're quantizing
+        (indicated via quantize_base=True).
+        """
+        in_dim, out_dim, use_bias = self.in_dim, self.out_dim, self.use_bias
+        linear = nn.Linear(in_features=in_dim, out_features=out_dim, bias=use_bias)
+        weight = linear.weight if not self._quantize_base else to_nf4(linear.weight)
+        bias = None
+        if self.use_bias:
+            if self._quantize_base:
+                raise NotImplementedError(
+                    "Quantized LoRALinear does not support bias at the moment."
+                )
+            bias = linear.bias
+        return weight, bias
+
     def adapter_params(self) -> List[str]:
         """
         Return lora_a.weight and lora_b.weight as adapter params.
         If bias is enabled, also return lora_a.bias and lora_b.bias.
         """
+        # NOTE: this function has to be updated if the names of "lora_a" and "lora_b"
+        # in this module change.
         adapter_params = ["lora_a.weight", "lora_b.weight"]
         return adapter_params
 
     def forward(self, x: Tensor) -> Tensor:
         """
         Args:
             x (Tensor): input tensor with shape ``(..., in_dim)``
 
         Returns:
             Tensor: output tensor with shape ``(..., out_dim)``
 
         """
-        out = F.linear(x, self.weight, self.bias)
+        if self._quantize_base:
+            out = linear_nf4(input=x, weight=self.weight)
+        else:
+            out = F.linear(x, self.weight, self.bias)
+        if self.disabled:
+            return out
         lora_out = self.lora_a(self.dropout(x))
         lora_out = (self.alpha / self.rank) * self.lora_b(lora_out)
         return out + lora_out
 
 
 def _lora_a_init_params(x: nn.Linear) -> None:
     """
```

## torchtune/modules/peft/peft_utils.py

```diff
@@ -1,15 +1,16 @@
 # Copyright (c) Meta Platforms, Inc. and affiliates.
 # All rights reserved.
 #
 # This source code is licensed under the BSD-style license found in the
 # LICENSE file in the root directory of this source tree.
 
+import contextlib
 import functools
-from typing import Any, Dict, List, Literal, Optional, Protocol, Set
+from typing import Any, Dict, Generator, List, Literal, Optional, Protocol, Set
 
 from torch import nn
 
 # Modules from CausalSelfAttention that LoRA can be applied to
 LORA_ATTN_MODULES = Literal["q_proj", "k_proj", "v_proj", "output_proj"]
 
 
@@ -29,25 +30,25 @@
 
         See LoRALinear's :func:`~torchtune.modules.peft.LoRALinear.adapter_params` for an example.
         """
         pass
 
 
 @functools.lru_cache()
-def get_adapter_params(model: nn.Module) -> Dict[str, Any]:
+def get_adapter_params(model: nn.Module) -> Dict[str, nn.Parameter]:
     """
     Return the subset of parameters from a model that correspond to an adapter.
     Assumes that any adapter class has defined the
     :func:`~torchtune.modules.peft.AdapterModule.adapter_params` method.
 
     Args:
         model (nn.Module): Instance of model class containing some adapter params.
 
     Returns:
-        Dict[str, Any]: the subset of model's state dict containing
+        Dict[str, nn.Parameter]: the subset of model's state dict containing
         only adapter parameters.
 
     """
     adapter_params = {}
     for k, v in model.named_modules():
         if hasattr(v, "adapter_params") and callable(v.adapter_params):
             current_adapter_params = v.adapter_params()
@@ -252,7 +253,90 @@
     for module in lora_modules:
         lora_a_weight = state_dict[f"{module}.lora_a.weight"]
         lora_b_weight = state_dict[f"{module}.lora_b.weight"]
         state_dict[f"{module}.weight"] += (alpha / rank) * lora_b_weight @ lora_a_weight
         del state_dict[f"{module}.lora_a.weight"]
         del state_dict[f"{module}.lora_b.weight"]
     return state_dict
+
+
+@contextlib.contextmanager
+def disable_adapter(model: nn.Module) -> Generator[None, None, None]:
+    for _, v in model.named_modules():
+        if (
+            hasattr(v, "adapter_params")
+            and callable(v.adapter_params)
+            and hasattr(v, "disabled")
+        ):
+            v.disabled = True
+    try:
+        yield
+    finally:
+        for _, v in model.named_modules():
+            if (
+                hasattr(v, "adapter_params")
+                and callable(v.adapter_params)
+                and hasattr(v, "disabled")
+            ):
+                v.disabled = False
+
+
+def validate_missing_and_unexpected_for_lora(
+    lora_attn_modules: List[LORA_ATTN_MODULES],
+    apply_lora_to_mlp: bool,
+    apply_lora_to_output: bool,
+    base_missing: Optional[List[str]] = None,
+    base_unexpected: Optional[List[str]] = None,
+    lora_missing: Optional[List[str]] = None,
+    lora_unexpected: Optional[List[str]] = None,
+) -> None:
+    """
+    A more memory-efficient way to validate that LoRA state dict loading was done properly.
+
+    Similar to validate_state_dict_for_lora, this function uses a model's LoRA config to
+    check that LoRA and/or base model weights are loaded into the full model correctly.
+    Unlike that function, this method relies only on the values of missing and unexpected
+    as returned by the load_state_dict API with strict=False. This allows us to do the
+    validation without any additional calls to .state_dict(), which use additional memory.
+    This API should only be used for single-device recipes, or on multi-device after
+    https://github.com/pytorch/pytorch/pull/120600.
+
+    Args:
+        lora_attn_modules (List[LORA_ATTN_MODULES]): list of which linear layers
+            LoRA should be applied to in each self-attention block. Options are
+            ``{"q_proj", "k_proj", "v_proj", "output_proj"}``.
+        apply_lora_to_mlp (bool): whether LoRA is applied to each MLP linear.
+        apply_lora_to_output (bool): whether LoRA is applied to the final output projection.
+        base_missing (Optional[List[str]]): List of missing keys when loading base model weights.
+            Default: None
+        base_unexpected (Optional[List[str]]): List of unexpected keys when loading base model weights.
+            Default: None
+        lora_missing (Optional[List[str]]): List of missing keys when loading LoRA weights.
+            Default: None
+        lora_unexpected (Optional[List[str]]): List of unexpected keys when loading LoRA weights.
+            Default: None
+
+    Returns:
+        None
+
+    Raises:
+        AssertionError: if base_missing contains any base model keys.
+        AssertionError: if base_unexpect is nonempty.
+        AssertionError: if lora_missing contains any LoRA keys.
+        AssertionError: if lora_unexpected is nonempty.
+    """
+    lora_modules = get_lora_module_names(
+        lora_attn_modules, apply_lora_to_mlp, apply_lora_to_output
+    )
+    is_lora_param = lambda x: any([".".join([k, "lora"]) in x for k in lora_modules])
+    if base_missing:
+        for k in base_missing:
+            if not is_lora_param(k):
+                raise AssertionError(f"Missing non-LoRA key {k} from base model dict")
+    if base_unexpected:
+        raise AssertionError("Unexpected key loading base model")
+    if lora_missing:
+        for k in lora_missing:
+            if is_lora_param(k):
+                raise AssertionError(f"Missing LoRA key {k} from adapter state dict")
+    if lora_unexpected:
+        raise AssertionError("Unexpected key loading adapter")
```

## torchtune/utils/__init__.py

```diff
@@ -5,53 +5,60 @@
 # LICENSE file in the root directory of this source tree.
 
 from ._checkpointing import (  # noqa
     FullModelHFCheckpointer,
     FullModelMetaCheckpointer,
     FullModelTorchTuneCheckpointer,
     ModelType,
+    transform_opt_state_dict,
 )
+
+from ._compile_utils import wrap_compile
 from ._device import get_device
 from ._distributed import (  # noqa
     contains_fsdp,
     get_world_size_and_rank,
     init_distributed,
     is_distributed,
     lora_fsdp_wrap_policy,
     prepare_model_for_fsdp_with_meta_device,
     validate_no_params_on_meta_device,
     wrap_fsdp,
 )
-from .argparse import TuneArgumentParser
-from .checkpoint import (  # noqa
-    save_checkpoint,
-    transform_opt_state_dict,
-    validate_checkpoint,
-)
-from .checkpointable_dataloader import CheckpointableDataLoader
-from .collate import padded_collate
+from ._generation import generate, generate_next_token  # noqa
+from ._profiler import profiler
+from .argparse import TuneRecipeArgumentParser
+from .collate import padded_collate, padded_collate_dpo
 from .constants import (  # noqa
     ADAPTER_KEY,
     EPOCHS_KEY,
     MAX_STEPS_KEY,
     MODEL_KEY,
     OPT_KEY,
     SEED_KEY,
     TOTAL_EPOCHS_KEY,
 )
 from .logging import get_logger
-from .memory import memory_stats_log, set_activation_checkpointing  # noqa
+from .memory import (  # noqa
+    cleanup_before_training,
+    create_optim_in_bwd_wrapper,
+    memory_stats_log,
+    OptimizerInBackwardWrapper,
+    register_optim_in_bwd_hooks,
+    set_activation_checkpointing,
+)
 from .precision import (
     get_autocast,
     get_dtype,
     get_gradient_scaler,
     list_dtypes,
     set_default_dtype,
     validate_expected_param_dtype,
 )
+from .quantization import get_quantizer_mode
 from .seed import set_seed
 
 __all__ = [
     "save_checkpoint",
     "transform_opt_state_dict",
     "validate_checkpoint",
     "get_autocast",
@@ -63,14 +70,21 @@
     "get_logger",
     "get_world_size_and_rank",
     "init_distributed",
     "is_distributed",
     "list_dtypes",
     "lora_fsdp_wrap_policy",
     "padded_collate",
+    "padded_collate_dpo",
     "set_activation_checkpointing",
     "set_default_dtype",
     "set_seed",
     "validate_expected_param_dtype",
-    "TuneArgumentParser",
+    "wrap_compile",
+    "TuneRecipeArgumentParser",
     "CheckpointableDataLoader",
+    "OptimizerInBackwardWrapper",
+    "create_optim_in_bwd_wrapper",
+    "register_optim_in_bwd_hooks",
+    "profiler",
+    "get_quantizer_mode",
 ]
```

## torchtune/utils/_distributed.py

```diff
@@ -10,15 +10,14 @@
 from itertools import chain
 from typing import Callable, Dict, Optional, Set, Tuple, Type, Union
 
 import torch
 import torch.distributed as dist
 from torch import nn
 from torch.distributed.fsdp import (
-    CPUOffload,
     FullyShardedDataParallel as FSDP,
     MixedPrecision,
     ShardingStrategy,
 )
 from torch.distributed.fsdp.wrap import ModuleWrapPolicy
 from torchtune.modules.peft.lora import (
     _lora_a_init_params,
@@ -144,15 +143,14 @@
 
 def wrap_fsdp(
     model: nn.Module,
     device: torch.device,
     dtype: torch.dtype,
     strategy: Optional[str] = None,
     auto_wrap_policy: Optional[Union[Set[Type], FSDPPolicyType]] = None,
-    cpu_offload: bool = False,
     use_meta_device: bool = False,
     **kwargs,
 ) -> nn.Module:
     """Utility to setup distributed training using the torch.distributed FullyShardedDataParallel (FSDP) module.
     FSDP allows three primary types of data parallel training (these can be set under "strategy"):
 
     NO_SHARD:
@@ -181,53 +179,44 @@
             Alternatively, this can be a custom callable policy of type FSDPPolicyType, in which case FSDP will
             be wrapped according to the specified policy.
             Please see https://pytorch.org/tutorials/intermediate/FSDP_adavnced_tutorial.html#transformer-wrapping-policy
             for details on FSDP wrapping and writing wrapping policies.
             Default: None. In this case, FSDP is only applied to the top level module. In this
             case, entire model is unsharded during computation and memory is only saved due to
             sharding optimizer states.
-        cpu_offload (bool): Whether to offload sharded parameters to CPU. Default: False
         use_meta_device (bool): Set this to True if the input model has been initialized on meta device.
             If so, we will define the `reset_parameters()` method on all submodules
             to ensure FSDP properly initializes all modules on device given by `device`. Default: False
         **kwargs: additional arguments to pass to FSDP for distributed training.
 
     Returns:
         nn.Module: Model wrapped for distributed training
 
     Raises:
         RuntimeError: If environment not setup for distributed training.
 
-    NOTE:
-        Please use caution if running with cpu_offload=True, as this is known to have
-        significant training performance issues at the moment.
     """
     if dist.is_available() and dist.is_initialized():
         if use_meta_device:
             model = prepare_model_for_fsdp_with_meta_device(model)
         if strategy is None:
             strategy = "FULL_SHARD"
         _validate_device_from_env(device)
         wrap_policy = (
             ModuleWrapPolicy(auto_wrap_policy)
             if isinstance(auto_wrap_policy, set)
             else auto_wrap_policy
         )
         mp = MixedPrecision(param_dtype=dtype, reduce_dtype=dtype, buffer_dtype=dtype)
-        if cpu_offload:
-            _log.warning(
-                "CPU offload will significantly reduce performance. Use with caution."
-            )
         return FSDP(
             model,
             auto_wrap_policy=wrap_policy,
             device_id=device,
             mixed_precision=None,
             sharding_strategy=_get_sharding_strategy(strategy),
-            cpu_offload=CPUOffload(offload_params=True) if cpu_offload else None,
             **kwargs,
         )
     else:
         raise RuntimeError(
             "Distributed environment is not setup. Please run init_distributed() first."
         )
```

## torchtune/utils/argparse.py

```diff
@@ -7,27 +7,26 @@
 import argparse
 from argparse import Namespace
 from typing import List, Tuple
 
 from omegaconf import OmegaConf
 
 
-class TuneArgumentParser(argparse.ArgumentParser):
+class TuneRecipeArgumentParser(argparse.ArgumentParser):
     """
-    TuneArgumentParser is a helpful utility subclass of the argparse ArgumentParser that
-    adds a builtin argument "config". The config argument takes a file path to a yaml file
-    and will load in argument defaults from the yaml file. The yaml file must only contain
+    A helpful utility subclass of the ``argparse.ArgumentParser`` that
+    adds a builtin argument "config". The config argument takes a file path to a YAML file
+    and loads in argument defaults from said file. The YAML file must only contain
     argument names and their values and nothing more, it does not have to include all of the
     arguments. These values will be treated as defaults and can still be overridden from the
     command line. Everything else works the same as the base ArgumentParser and you should
-    consult the docs for more info.
+    consult the docs for more info: https://docs.python.org/3/library/argparse.html.
 
-    https://docs.python.org/3/library/argparse.html
-
-    *Note: This class uses "config" as a builtin argument so it is not available to use*
+    Note:
+        This class uses "config" as a builtin argument so it is not available to use.
     """
 
     def __init__(self, *args, **kwargs) -> None:
         super().__init__(*args, **kwargs)
         super().add_argument(
             "--config",
             type=str,
@@ -36,17 +35,15 @@
         )
 
     def parse_known_args(self, *args, **kwargs) -> Tuple[Namespace, List[str]]:
         """This acts the same as the base parse_known_args but will first load in defaults from
         from the config yaml file if it is provided. The command line args will always take
         precident over the values in the config file. All other parsing method, such as parse_args,
         internally call this method so they will inherit this property too. For more info see
-        the docs for the base method.
-
-        https://docs.python.org/3/library/argparse.html#the-parse-args-method
+        the docs for the base method: https://docs.python.org/3/library/argparse.html#the-parse-args-method.
         """
         namespace, unknown_args = super().parse_known_args(*args, **kwargs)
 
         unknown_flag_args = [arg for arg in unknown_args if arg.startswith("--")]
         if unknown_flag_args:
             raise ValueError(
                 f"Additional flag arguments not supported: {unknown_flag_args}. Please use --config or key=value overrides"
```

## torchtune/utils/collate.py

```diff
@@ -1,27 +1,29 @@
 # Copyright (c) Meta Platforms, Inc. and affiliates.
 # All rights reserved.
 #
 # This source code is licensed under the BSD-style license found in the
 # LICENSE file in the root directory of this source tree.
-from typing import List, Tuple
+from typing import Any, Dict, List, Tuple
 
 import torch
 
 import torch.nn.functional as F
 from torch.nn.utils.rnn import pad_sequence
+from torchtune.data import CROSS_ENTROPY_IGNORE_IDX
+
 
 # TokenPair is a pair (tuple) of two lists: tokenized text inputs and labels.
 TokenPair = Tuple[List[int], List[int]]
 
 
 def padded_collate(
     batch: List[TokenPair],
     padding_idx: int = 0,
-    ignore_idx: int = -100,
+    ignore_idx: int = CROSS_ENTROPY_IGNORE_IDX,
 ) -> Tuple[torch.Tensor, torch.Tensor]:
     """Pad a batch of sequences to the longest sequence length in the batch, and
     convert integer lists to tensors.
 
     Args:
         batch (List[TokenPair]): A list of tuples containing input, label pairs.
         padding_idx (int): Padding index for input ids. Defaults to 0.
@@ -67,7 +69,67 @@
     elif labels_seq_len > input_ids_seq_len:
         input_ids = F.pad(
             input_ids,
             (0, labels_seq_len - input_ids_seq_len),
             value=padding_idx,
         )
     return input_ids, labels
+
+
+def padded_collate_dpo(
+    batch: List[Dict[str, Any]],
+    padding_idx: int = 0,
+    ignore_idx: int = CROSS_ENTROPY_IGNORE_IDX,
+) -> Tuple[torch.Tensor, torch.Tensor]:
+    """Pad a batch of sequences for Direct Preference Optimization (DPO).
+
+    This function takes a batch of sequences, where each sequence is represented
+    as a dictionary with multiple key-value pairs. Each key corresponds to a different
+    sequence component, such as input_ids or labels.
+
+    Args:
+        batch (List[Dict[str, Any]]): A list of dictionaries, where each dictionary
+            represents a sequence with multiple components, 'chosen_input_ids',
+            'chosen_labels', 'rejected_input_ids', and 'rejected_labels' are required.
+        padding_idx (int): Padding index for input ids. Defaults to 0.
+        ignore_idx (int): Padding index for labels. Defaults to -100.
+
+    Returns:
+        Tuple[torch.Tensor, torch.Tensor]: A tuple containing concatenated and padded
+        input ids and labels.
+
+    Example:
+        >>> batch = [
+        >>>    {'chosen_input_ids': [1, 2, 3], 'rejected_input_ids': [4, 5],
+        >>>      'chosen_labels': [6, 7, 8], 'rejected_labels': [9, 10]},
+        >>>    {'chosen_input_ids': [11, 12], 'rejected_input_ids': [13, 14, 15],
+        >>>      'chosen_labels': [16, 17], 'rejected_labels': [18, 19, 20]},
+        >>> ]
+        >>> padded_collate_dpo(batch)
+        >>> (tensor([[ 1,  2,  3],
+        >>>          [11, 12,  0],
+        >>>          [ 4,  5,  0],
+        >>>          [13, 14, 15]]),
+        >>>  tensor([[ 6,  7,  8],
+        >>>          [16, 17, -100],
+        >>>          [ 9, 10, -100],
+        >>>          [18, 19, 20]]))
+    """
+    chosen_input_ids = [torch.tensor(ex["chosen_input_ids"]) for ex in batch]
+    rejected_input_ids = [torch.tensor(ex["rejected_input_ids"]) for ex in batch]
+    chosen_labels = [torch.tensor(ex["chosen_labels"]) for ex in batch]
+    rejected_labels = [torch.tensor(ex["rejected_labels"]) for ex in batch]
+
+    assert len(chosen_input_ids) == len(rejected_input_ids)
+    assert len(chosen_labels) == len(rejected_labels)
+
+    to_pad_input_ids = chosen_input_ids + rejected_input_ids
+    to_pad_labels = chosen_labels + rejected_labels
+
+    concatenated_input_ids = pad_sequence(
+        to_pad_input_ids, batch_first=True, padding_value=padding_idx
+    )
+    concatenated_labels = pad_sequence(
+        to_pad_labels, batch_first=True, padding_value=ignore_idx
+    )
+
+    return concatenated_input_ids, concatenated_labels
```

## torchtune/utils/memory.py

```diff
@@ -1,14 +1,16 @@
 # Copyright (c) Meta Platforms, Inc. and affiliates.
 # All rights reserved.
 #
 # This source code is licensed under the BSD-style license found in the
 # LICENSE file in the root directory of this source tree.
 
-from typing import Optional, Set
+import gc
+
+from typing import Any, Dict, Optional, Set
 
 import torch
 
 from torch import nn
 from torch.distributed.algorithms._checkpoint.checkpoint_wrapper import (
     apply_activation_checkpointing,
 )
@@ -25,41 +27,172 @@
         auto_wrap_policy (Optional[Set[nn.Module]]): Policy to wrap module.
         **kwargs: additional arguments to pass to torch.distributed activation checkpointing.
     """
     wrap_policy = ModuleWrapPolicy(auto_wrap_policy or set())
     apply_activation_checkpointing(model, auto_wrap_policy=wrap_policy, **kwargs)
 
 
-def memory_stats_log(
-    prefix: str, device: torch.device, reset_stats: bool = True
+def cleanup_before_training() -> None:
+    gc.collect()
+    torch.cuda.empty_cache()
+    torch.cuda.reset_peak_memory_stats()
+
+
+class OptimizerInBackwardWrapper:
+    """
+    A bare-bones class meant for checkpoint save and load for optimizers running
+    in backward. Usage is limited to the following:
+
+    optim_dict = {
+        p: config.instantiate(cfg_optimizer, [p])
+        for p in self._model.parameters()
+    }
+    # Save checkpoint
+    ckpt = OptimizerInBackwardWrapper(optim_dict).state_dict()
+    torch.save("/tmp/optim_ckpt", ckpt)
+    # Load checkpoint
+    placeholder_optim_dict = {
+        p: config.instantiate(cfg_optimizer, [p])
+        for p in self._model.parameters()
+    }
+    wrapper = OptimInBackwardWrapper(placeholder_optim_dict)
+    # load_state_dict expects a dict produced by this class's
+    # state_dict method.
+    wrapper.load_state_dict(torch.load("/tmp/optim_ckpt"))
+    # placeholder_optim_dict now has updated optimizer states.
+
+    NOTE: This wrapper is only meant to be used for single-device use cases.
+        Distributed use cases such as FSDP, which require specialized
+        optimizer state checkpointing, are not supported.
+
+    Args:
+        optim_map (Dict[str, torch.optim.Optimizer]): Mapping from parameter names to optimizers.
+
+    """
+
+    def __init__(self, optim_map: Dict[str, torch.optim.Optimizer]):
+        self.optim_map = optim_map
+
+    def state_dict(self) -> Dict[str, Any]:
+        """
+        Returns a state dict mapping parameter names to optimizer states. This
+        state_dict is only loadable by this same class.
+
+        Returns:
+            Dict[str, Any]: state dict mapping parameter names to optimizer states.
+        """
+        return {p: opt.state_dict() for p, opt in self.optim_map.items()}
+
+    def load_state_dict(self, optim_ckpt_map: Dict[str, Any]):
+        """
+        Load optimizer states from a state dict produced by this class's
+        state_dict method.
+
+        Args:
+            optim_ckpt_map (Dict[str, Any]): state dict mapping parameter names to optimizer states.
+
+        Raises:
+            RuntimeError: If the optimizer state dict does not contain all the expected parameters.
+        """
+        params_covered = set()
+        for param_name in optim_ckpt_map.keys():
+            if param_name not in self.optim_map:
+                raise RuntimeError(
+                    f"Trying to load optimizer state for unexpected param {param_name}"
+                )
+            self.optim_map[param_name].load_state_dict(optim_ckpt_map[param_name])
+            params_covered.add(param_name)
+        # Ensure all params have been loaded into, report missing params
+        missing_params = set(self.optim_map.keys()) - params_covered
+        if missing_params:
+            raise RuntimeError(
+                f"Expected to load optimizer state for params {missing_params}!"
+            )
+
+    def get_optim_key(self, key: str) -> Any:
+        """
+        Returns value of key from an arbitrary optimizer running in backward. Note that
+        this assumes all optimizer in backwards have the same value for the key, i.e.,
+        are initialized with the same hyperparameters.
+        """
+        return list(self.optim_map.values())[0].param_groups[0][key]
+
+
+def create_optim_in_bwd_wrapper(
+    model: torch.nn.Module, optim_dict: Dict[torch.nn.Parameter, torch.optim.Optimizer]
+) -> OptimizerInBackwardWrapper:
+    """
+    Create a wrapper for optimizer step running in backward.
+
+    Args:
+        model (torch.nn.Module): Model that contains parameters that are being optimized. For now,
+            it is assumed that all parameters being optimized belong to a single top-level model.
+            `named_parameters` attribute of `model` will be accessed to look up parameter names for
+            parameters being optimized.
+        optim_dict (Dict[torch.nn.Parameter, torch.optim.Optimizer]): Mapping from
+            parameters to optimizers.
+
+    Returns:
+        ``OptimizerInBackwardWrapper``: Wrapper for optimizer states running in backward.
+    """
+    return OptimizerInBackwardWrapper(
+        {n: optim_dict[p] for n, p in model.named_parameters()}
+    )
+
+
+def register_optim_in_bwd_hooks(
+    model: torch.nn.Module, optim_dict: Dict[torch.nn.Parameter, torch.optim.Optimizer]
 ) -> None:
     """
-    Print a memory summary for the passed in device. If ``reset_stats`` is ``True``, this will
+    Register hooks for optimizer step running in backward.
+
+    Args:
+        model (torch.nn.Module): Model whose parameters will be optimized. Note that currently
+            hooks for ALL parameters in the model will be registered.
+        optim_dict (Dict[torch.nn.Parameter, torch.optim.Optimizer]): Mapping from
+            parameters to optimizers.
+    """
+
+    def optim_step(param) -> None:
+        optim_dict[param].step()
+        optim_dict[param].zero_grad()
+
+    for p in model.parameters():
+        p.register_post_accumulate_grad_hook(optim_step)
+
+
+def memory_stats_log(device: torch.device, reset_stats: bool = True) -> dict:
+    """
+    Computes a memory summary for the passed in device. If ``reset_stats`` is ``True``, this will
     also reset CUDA's peak memory tracking. This is useful to get data around relative use of peak
     memory (i.e. peak memory during model init, during forward, etc) and optimize memory for
     individual sections of training.
 
     Args:
-        prefix (str): Prefix to prepend to the printed summary.
         device (torch.device): Device to get memory summary for. Only CUDA devices are supported.
         reset_stats (bool): Whether to reset CUDA's peak memory tracking.
 
     Returns:
-        None
+        Dict[str, float]: A dictionary containing the peak memory active, peak memory allocated,
+        and peak memory reserved. This dict is useful for logging memory stats.
+
+    Raises:
+        ValueError: If the passed in device is not CUDA.
     """
     if device.type != "cuda":
-        return
+        raise ValueError(
+            f"Logging memory stats is only supported on CUDA devices, got {device}"
+        )
+
     peak_memory_active = torch.cuda.memory_stats().get("active_bytes.all.peak", 0) / 1e9
     peak_mem_alloc = torch.cuda.max_memory_allocated(device) / 1e9
     peak_mem_reserved = torch.cuda.max_memory_reserved(device) / 1e9
 
-    ret = f"""
-    {prefix}:
-    GPU peak memory allocation: {peak_mem_alloc:.2f} GB
-    GPU peak memory reserved: {peak_mem_reserved:.2f} GB
-    GPU peak memory active: {peak_memory_active:.2f} GB
-    """
-
     if reset_stats:
         torch.cuda.reset_peak_memory_stats(device)
 
-    return ret
+    memory_stats = {
+        "peak_memory_active": peak_memory_active,
+        "peak_memory_alloc": peak_mem_alloc,
+        "peak_memory_reserved": peak_mem_reserved,
+    }
+    return memory_stats
```

## torchtune/utils/metric_logging.py

```diff
@@ -7,21 +7,25 @@
 import sys
 import time
 from pathlib import Path
 
 from typing import Mapping, Optional, Union
 
 from numpy import ndarray
+from omegaconf import DictConfig, OmegaConf
 from torch import Tensor
 
+from torchtune.utils import get_logger
 from torchtune.utils._distributed import get_world_size_and_rank
 from typing_extensions import Protocol
 
 Scalar = Union[Tensor, ndarray, int, float]
 
+log = get_logger("DEBUG")
+
 
 class MetricLoggerInterface(Protocol):
     """Abstract metric logger."""
 
     def log(
         self,
         name: str,
@@ -33,14 +37,22 @@
         Args:
             name (str): tag name used to group scalars
             data (Scalar): scalar data to log
             step (int): step value to record
         """
         pass
 
+    def log_config(self, config: DictConfig) -> None:
+        """Logs the config
+
+        Args:
+            config (DictConfig): config to log
+        """
+        pass
+
     def log_dict(self, payload: Mapping[str, Scalar], step: int) -> None:
         """Log multiple scalar values.
 
         Args:
             payload (Mapping[str, Scalar]): dictionary of tag name and scalar value
             step (int): step value to record
         """
@@ -55,28 +67,32 @@
 
 
 class DiskLogger(MetricLoggerInterface):
     """Logger to disk.
 
     Args:
         log_dir (str): directory to store logs
+        filename (Optional[str]): optional filename to write logs to.
+            Default: None, in which case log_{unixtimestamp}.txt will be used.
         **kwargs: additional arguments
 
     Warning:
         This logger is not thread-safe.
 
     Note:
         This logger creates a new file based on the current time.
     """
 
-    def __init__(self, log_dir: str, **kwargs):
+    def __init__(self, log_dir: str, filename: Optional[str] = None, **kwargs):
         self.log_dir = Path(log_dir)
         self.log_dir.mkdir(parents=True, exist_ok=True)
-        unix_timestamp = int(time.time())
-        self._file_name = self.log_dir / f"log_{unix_timestamp}.txt"
+        if not filename:
+            unix_timestamp = int(time.time())
+            filename = f"log_{unix_timestamp}.txt"
+        self._file_name = self.log_dir / filename
         self._file = open(self._file_name, "a")
         print(f"Writing logs to {self._file_name}")
 
     def path_to_log_file(self) -> Path:
         return self._file_name
 
     def log(self, name: str, data: Scalar, step: int) -> None:
@@ -139,47 +155,84 @@
         You can install it with `pip install wandb`.
         In order to use the logger, you need to login to your WandB account.
         You can do this by running `wandb login` in your terminal.
     """
 
     def __init__(
         self,
-        project: str,
+        project: str = "torchtune",
         entity: Optional[str] = None,
         group: Optional[str] = None,
         **kwargs,
     ):
         try:
             import wandb
         except ImportError as e:
             raise ImportError(
                 "``wandb`` package not found. Please install wandb using `pip install wandb` to use WandBLogger."
                 "Alternatively, use the ``StdoutLogger``, which can be specified by setting metric_logger_type='stdout'."
             ) from e
         self._wandb = wandb
-        self._wandb.init(
-            project=project,
-            entity=entity,
-            group=group,
-            reinit=True,
-            resume="allow",
-            config=kwargs,
-        )
+
+        _, self.rank = get_world_size_and_rank()
+
+        if self.rank == 0:
+            self._wandb.init(
+                project=project,
+                entity=entity,
+                group=group,
+                reinit=True,
+                resume="allow",
+                **kwargs,
+            )
+
+    def log_config(self, config: DictConfig) -> None:
+        """Saves the config locally and also logs the config to W&B. The config is
+        stored in the same directory as the checkpoint. You can
+        see an example of the logged config to W&B in the following link:
+        https://wandb.ai/capecape/torchtune/runs/6053ofw0/files/torchtune_config_j67sb73v.yaml
+
+        Args:
+            config (DictConfig): config to log
+        """
+        if self._wandb.run:
+            resolved = OmegaConf.to_container(config, resolve=True)
+            self._wandb.config.update(resolved)
+
+            output_config_fname = Path(
+                os.path.join(
+                    config.checkpointer.checkpoint_dir,
+                    f"torchtune_config_{self._wandb.run.id}.yaml",
+                )
+            )
+            OmegaConf.save(config, output_config_fname)
+            try:
+                log.info(f"Logging {output_config_fname} to W&B under Files")
+                self._wandb.save(
+                    output_config_fname, base_path=output_config_fname.parent
+                )
+
+            except Exception as e:
+                log.warning(f"Error saving {output_config_fname} to W&B.\nError: \n{e}")
 
     def log(self, name: str, data: Scalar, step: int) -> None:
-        self._wandb.log({name: data}, step=step)
+        if self._wandb.run:
+            self._wandb.log({name: data}, step=step)
 
     def log_dict(self, payload: Mapping[str, Scalar], step: int) -> None:
-        self._wandb.log(payload, step=step)
+        if self._wandb.run:
+            self._wandb.log(payload, step=step)
 
     def __del__(self) -> None:
-        self._wandb.finish()
+        if self._wandb.run:
+            self._wandb.finish()
 
     def close(self) -> None:
-        self._wandb.finish()
+        if self._wandb.run:
+            self._wandb.finish()
 
 
 class TensorBoardLogger(MetricLoggerInterface):
     """Logger for use w/ PyTorch's implementation of TensorBoard (https://pytorch.org/docs/stable/tensorboard.html).
 
     Args:
         log_dir (str): TensorBoard log directory
```

## torchtune/utils/precision.py

```diff
@@ -1,17 +1,27 @@
 # Copyright (c) Meta Platforms, Inc. and affiliates.
 # All rights reserved.
 #
 # This source code is licensed under the BSD-style license found in the
 # LICENSE file in the root directory of this source tree.
 
 import contextlib
-from typing import ContextManager, Dict, Generator, List, Optional, Union
+from typing import (
+    ContextManager,
+    Dict,
+    Generator,
+    Iterable,
+    List,
+    Optional,
+    Tuple,
+    Union,
+)
 
 import torch
+import torch.nn as nn
 from pkg_resources import packaging
 
 from torch.cuda.amp import GradScaler
 from torch.distributed.fsdp.sharded_grad_scaler import ShardedGradScaler
 
 from torchtune.utils._device import _validate_device_from_env
 from torchtune.utils.logging import get_logger
@@ -61,42 +71,61 @@
         and torch.cuda.is_bf16_supported()
         and packaging.version.parse(torch.version.cuda).release >= (11, 0)
         and torch.distributed.is_nccl_available()
         and torch.cuda.nccl.version() >= (2, 10)
     )
 
 
-def get_dtype(dtype: Optional[str] = None) -> torch.dtype:
+def get_dtype(
+    dtype: Optional[str] = None, device: Optional[torch.device] = None
+) -> torch.dtype:
     """Get the torch.dtype corresponding to the given precision string.
 
-    Args:
-        dtype (Optional[str]): The precision dtype.
+    Note:
+        If bf16 precision is requested with a CUDA device, we verify whether the device indeed supports
+        bf16 kernels. If not, a ``RuntimeError`` is raised.
 
+    Args:
+        dtype (Optional[str]): The precision dtype. Default: ``None``, in which we default to torch.float32
+        device (Optional[torch.device]): Device in use for training. Only CUDA and CPU
+            devices are supported. If a CUDA device is passed in, additional checking is done
+            to ensure that the device supports the requested precision. Default: ``None``, in which case
+            a CUDA device is assumed.
     Raises:
         ValueError: if precision isn't supported by the precision utils
+        RuntimeError: if bf16 precision is requested but not available on this hardware.
 
     Returns:
         torch.dtype: The corresponding torch.dtype.
+
     """
+
     # None defaults to float32
     if dtype is None:
         return torch.float32
 
     # Convert to torch.dtype
     torch_dtype = PRECISION_STR_TO_DTYPE.get(dtype, dtype)
 
     # dtype must be one of the supported precisions
     if torch_dtype not in PRECISION_STR_TO_DTYPE.values():
         raise ValueError(
             f"Dtype {torch_dtype} must be one of {', '.join(list_dtypes())} for finetuning."
         )
 
-    if torch_dtype == torch.bfloat16 and not verify_bf16_support():
-        log.info("BF16 not supported on this hardware. Setting dtype to float32")
-        torch_dtype = torch.float32
+    # TODO (rohan-varma): prefer to use get_default_device() here to figure out whether user is training on
+    # CPU or GPU, but it is not supported in versions of torch we test.
+    if (
+        torch_dtype == torch.bfloat16
+        and device != torch.device("cpu")
+        and not verify_bf16_support()
+    ):
+        raise RuntimeError(
+            "bf16 precision was requested but not available on this hardware. Please use fp32 precision instead."
+        )
 
     return torch_dtype
 
 
 def get_gradient_scaler(fsdp: bool = False) -> Union[GradScaler, ShardedGradScaler]:
     """
     Returns a gradient scaler for mixed-precision training.
@@ -141,21 +170,25 @@
     torch.set_default_dtype(dtype)
     try:
         yield
     finally:
         torch.set_default_dtype(old_dtype)
 
 
-def validate_expected_param_dtype(model: torch.nn.Module, dtype: torch.dtype) -> None:
+def validate_expected_param_dtype(
+    named_params: Iterable[Tuple[str, nn.Parameter]], dtype: torch.dtype
+) -> None:
     """
-    Validates that all parameters in the model have the expected dtype.
+    Validates that all input parameters have the expected dtype.
 
     Args:
-        model (torch.nn.Module): Model to validate.
+        named_params (Iterable[Tuple[str, nn.Parameter]]): Iterable of named parameters.
         dtype (torch.dtype): Expected dtype.
 
     Raises:
-        ValueError: If any parameter in the model has a different dtype than `dtype`.
+        ValueError: If any parameter has a different dtype than `dtype`.
     """
-    for name, param in model.named_parameters():
+    for name, param in named_params:
         if param.dtype != dtype:
-            raise ValueError(f"Parameter {name} has dtype {param.dtype}")
+            raise ValueError(
+                f"Parameter {name} has dtype {param.dtype}, but expected {dtype}"
+            )
```

## torchtune/utils/_checkpointing/__init__.py

```diff
@@ -5,8 +5,8 @@
 # LICENSE file in the root directory of this source tree.
 
 from ._checkpointer import (  # noqa
     FullModelHFCheckpointer,
     FullModelMetaCheckpointer,
     FullModelTorchTuneCheckpointer,
 )
-from ._checkpointer_utils import ModelType  # noqa
+from ._checkpointer_utils import ModelType, transform_opt_state_dict  # noqa
```

## torchtune/utils/_checkpointing/_checkpointer.py

```diff
@@ -10,19 +10,20 @@
 
 from pathlib import Path
 from typing import Any, Dict, List, Optional, Protocol
 
 import torch
 from torchtune import utils
 
-from torchtune.models import llama2
+from torchtune.models import convert_weights
 from torchtune.utils._checkpointing._checkpointer_utils import (
     get_path,
     ModelType,
     safe_torch_load,
+    save_config,
 )
 from torchtune.utils.logging import get_logger
 
 logger = get_logger("DEBUG")
 
 
 class _CheckpointerInterface(Protocol):
@@ -91,15 +92,15 @@
 
     def save_checkpoint(self, state_dict: Dict[str, Any], **kwargs) -> None:
         ...
 
 
 class FullModelTorchTuneCheckpointer(_CheckpointerInterface):
     """
-    Checkpointer which reads and writes "full-model" checkpoints in a format compatible with
+    Checkpointer which reads and writes checkpoints in a format compatible with
     TorchTune. No conversion of weights is required.
 
     Currently this supports reading a single checkpoint file only. This will likely change as
     we add support for larger models.
     """
 
     def __init__(
@@ -144,31 +145,40 @@
         if self._resume_from_checkpoint:
             if recipe_checkpoint is None:
                 raise ValueError(
                     "If resume_from_checkpoint is True, recipe_checkpoint file must be provided."
                 )
             self._recipe_checkpoint = get_path(self._checkpoint_dir, recipe_checkpoint)
 
-    def load_checkpoint(self) -> Dict[str, Any]:
+    def load_checkpoint(self, weights_only: bool = True) -> Dict[str, Any]:
         """
         Load TorchTune checkpoint from file. Currently only loading from a single file is supported.
 
         The output state_dict has the following format, with keys other than "model" only present if
         ``resume_from_checkpoint`` is True:
             {
                 "model": {
                     "key_1": weight
                     ...
                 },
                 "optimizer": ...,
                 ...
             }
+
+        Args:
+            weights_only (bool): flag passed down to torch.load. We expose this, because quantized models
+                cannot be loaded with weights_only=True
+
+        Returns:
+            Dict[str, Any]: state_dict from the input checkpoint
         """
         state_dict: Dict[str:Any] = {}
-        state_dict[utils.MODEL_KEY] = safe_torch_load(self._checkpoint_path)
+        state_dict[utils.MODEL_KEY] = safe_torch_load(
+            self._checkpoint_path, weights_only=weights_only
+        )
 
         if self._adapter_checkpoint:
             adapter_state_dict = safe_torch_load(self._adapter_checkpoint)
             state_dict[utils.ADAPTER_KEY] = adapter_state_dict
 
         if self._resume_from_checkpoint:
             recipe_state = safe_torch_load(self._recipe_checkpoint)
@@ -241,35 +251,38 @@
                 f"{os.path.getsize(output_path) / 1000**3:.2f} GB "
                 f"saved to {output_path}"
             )
 
 
 class FullModelHFCheckpointer(_CheckpointerInterface):
     """
-    Checkpointer which reads and writes "full-model" checkpoints in HF's format. Example includes
+    Checkpointer which reads and writes checkpoints in HF's format. Example includes
     the Llama-2-7b-hf model from the meta-llama repo (https://huggingface.co/meta-llama/Llama-2-7b-hf)
 
-    For this checkpointer to work correctly, we assume that checkpoint_dir contains the necessary
-    checkpoint and json files. The easiest way to make sure everything works correctly is to use
-    the following flow:
-
-        1. Download the model from the HF repo using tune download
-        tune download --repo-id meta-llama/Llama-2-7b-hf \
-        --output-dir <checkpoint_dir> \
-        --hf-token <hf-token>
-
-        2. Use the directory created in 1. as the checkpoint_dir
-
     A few notes about the checkpoint reading logic:
-        - HF checkpoint names usually oredered by ID (eg: 0001_of_0003, 0002_of_0003, etc.) To ensure
-            we read the files in the right order, we sort the checkpoint file names before reading
-        - Checkpoint conversion to and from HF's format requires access to model params which are
-            read directly from the "config.json" file. This helps ensure we either load the weights
-            correctly or error out in case of discrepancy between the HF checkpoint file and TorchTune's
-            model implementations.
+    - HF checkpoint names usually ordered by ID (eg: 0001_of_0003, 0002_of_0003, etc.) To ensure
+    we read the files in the right order, we sort the checkpoint file names before reading
+    - Checkpoint conversion to and from HF's format requires access to model params which are
+    read directly from the "config.json" file. This helps ensure we either load the weights
+    correctly or error out in case of discrepancy between the HF checkpoint file and TorchTune's
+    model implementations.
+
+    Args:
+        checkpoint_dir (str): Directory containing the checkpoint files
+        checkpoint_files (List[str]): List of checkpoint files to load. Since the checkpointer takes care
+            of sorting by file ID, the order in this list does not matter
+        model_type (ModelType): Model type of the model for which the checkpointer is being loaded
+        output_dir (str): Directory to save the checkpoint files
+        adapter_checkpoint (Optional[str]): Path to the adapter weights. Default is None
+        recipe_checkpoint (Optional[str]): Path to the recipe state checkpoint file. Default is None
+        resume_from_checkpoint (bool): If True, the checkpointer will load the additional checkpoint files to
+            resume training from a previous run. Default is False
+
+    Raises:
+        ValueError: If ``resume_from_checkpoint`` is True but ``recipe_checkpoint`` is None
     """
 
     def __init__(
         self,
         checkpoint_dir: str,
         checkpoint_files: List[str],
         model_type: ModelType,
@@ -296,14 +309,17 @@
         self._weight_map: Dict[str, str] = None
 
         # the config.json file contains model params needed for state dict conversion
         self._config = json.loads(
             Path.joinpath(self._checkpoint_dir, "config.json").read_text()
         )
 
+        # save config.json to output_dir
+        save_config(self._output_dir, self._config)
+
         # recipe_checkpoint contains the recipe state. This should be available if
         # resume_from_checkpoint is True
         self._recipe_checkpoint = None
         if self._resume_from_checkpoint:
             if recipe_checkpoint is None:
                 raise ValueError(
                     "If resume_from_checkpoint is True, recipe_checkpoint file must be provided."
@@ -322,29 +338,18 @@
 
     def load_checkpoint(self) -> Dict[str, Any]:
         """
         Load TorchTune checkpoint from file.
 
         The keys and weights from across all checkpoint files are merged into a single state_dict.
         We preserve the "state_dict key" <-> "checkpoint file mapping" in weight_map so we can
-        weite the state dict correctly in ``save_checkpoint``.
+        write the state dict correctly in ``save_checkpoint``.
 
         Before returning, the model state dict is converted to a TorchTune compatible format using.
 
-        The output state_dict has the following format, with keys other than "model" only present if
-        ``resume_from_checkpoint`` is True:
-            {
-                "model": {
-                    "key_1": weight
-                    ...
-                },
-                "optimizer": ...,
-                ...
-            }
-
         Returns:
             state_dict (Dict[str, Any]): TorchTune checkpoint state dict
 
         Raises:
             ValueError: If the values in the input state_dict are not Tensors
         """
         self._weight_map = {}
@@ -372,15 +377,15 @@
                 self._weight_map[key] = f"{cpt_idx+1:04}"
             merged_state_dict.update(state_dict)
 
             # delete the state_dict to free up memory; TODO check if this del is needed
             del state_dict
             gc.collect()
 
-        converted_state_dict[utils.MODEL_KEY] = llama2.hf_to_tune_llama2_7b(
+        converted_state_dict[utils.MODEL_KEY] = convert_weights.hf_to_tune(
             merged_state_dict,
             num_heads=self._config["num_attention_heads"],
             num_kv_heads=self._config["num_key_value_heads"],
             dim=self._config["hidden_size"],
         )
 
         if self._adapter_checkpoint:
@@ -402,33 +407,24 @@
         Save TorchTune checkpoint to file. If ``intermediate_checkpoint`` is True, an additional
         checkpoint file ``recipe_state.pt`` is created in ``_output_dir`` which contains the recipe
         state.
 
         The state_dict is first converted back to the HF format and then paritioned based on the
         ``_weight_map`` into separate checkpoint files.
 
-        The output state dicts have the following formats:
-
-            Model:
-                {
-                    "key_1": weight
-                    ...
-                }
-
-            Recipe State:
-                {
-                    "optimizer": ...,
-                    "epoch": ...,
-                    ...
-                }
+        Args:
+            state_dict (Dict[str, Any]): Checkpoint state dict to be written out to file
+            epoch (int): Epoch number. Used to create the checkpoint file name
+            intermediate_checkpoint (bool): If True, an additional checkpoint files for recipe state
+                and (if applicable) adapter weights are created. Default is False
         """
         self._output_dir.mkdir(exist_ok=True)
 
         # convert the state_dict back to hf format; do this inplace
-        state_dict[utils.MODEL_KEY] = llama2.tune_to_hf_llama2_7b(
+        state_dict[utils.MODEL_KEY] = convert_weights.tune_to_hf(
             state_dict[utils.MODEL_KEY],
             num_heads=self._config["num_attention_heads"],
             num_kv_heads=self._config["num_key_value_heads"],
             dim=self._config["hidden_size"],
         )
 
         # split the state_dict into separate dicts, one for each output checkpoint file
@@ -474,30 +470,34 @@
                 f"{os.path.getsize(output_path) / 1000**3:.2f} GB "
                 f"saved to {output_path}"
             )
 
 
 class FullModelMetaCheckpointer(_CheckpointerInterface):
     """
-    Checkpointer which reads and writes "full-model" checkpoints in Meta's format. Example includes
+    Checkpointer which reads and writes checkpoints in Meta's format. Example includes
     the Llama-2-7b model from the meta-llama repo (https://huggingface.co/meta-llama/Llama-2-7b)
 
-    For this checkpointer to work correctly, we assume that checkpoint_dir contains the necessary
-    checkpoint and json files. The easiest way to make sure everything works correctly is to use
-    the following flow:
-
-        1. Download the model from the HF repo using tune download
-        tune download --repo-id meta-llama/Llama-2-7b \
-        --output-dir <checkpoint_dir> \
-        --hf-token <hf-token>
-
-        2. Use the directory created in 1. as the checkpoint_dir
-
     Currently we support reading from a single checkpoint file only. Support for reading from
     sharded checkpoints is WIP.
+
+    Args:
+        checkpoint_dir (str): Directory containing the checkpoint files
+        checkpoint_files (List[str]): List of checkpoint files to load. Currently this checkpointer only
+            supports loading a single checkpoint file.
+        model_type (ModelType): Model type of the model for which the checkpointer is being loaded
+        output_dir (str): Directory to save the checkpoint files
+        adapter_checkpoint (Optional[str]): Path to the adapter weights. Default is None
+        recipe_checkpoint (Optional[str]): Path to the recipe state checkpoint file. Default is None
+        resume_from_checkpoint (bool): If True, the checkpointer will load the additional checkpoint files to
+            resume training from a previous run. Default is False
+
+    Raises:
+        ValueError: If ``checkpoint_files`` is not a list of length 1
+        ValueError: If ``resume_from_checkpoint`` is True but ``recipe_checkpoint`` is None
     """
 
     def __init__(
         self,
         checkpoint_dir: str,
         checkpoint_files: List[str],
         model_type: ModelType,
@@ -535,29 +535,18 @@
                     "If resume_from_checkpoint is True, recipe_checkpoint file must be provided."
                 )
             self._recipe_checkpoint = get_path(self._checkpoint_dir, recipe_checkpoint)
 
     def load_checkpoint(self) -> Dict[str, Any]:
         """
         Load TorchTune checkpoint from file. Currently only loading from a single file is supported.
-
-        The output state_dict has the following format, with keys other than "model" only present if
-        ``resume_from_checkpoint`` is True:
-            {
-                "model": {
-                    "key_1": weight
-                    ...
-                },
-                "optimizer": ...,
-                ...
-            }
         """
         state_dict: Dict[str:Any] = {}
         model_state_dict = safe_torch_load(self._checkpoint_path)
-        state_dict[utils.MODEL_KEY] = llama2.meta_to_tune_llama2_7b(model_state_dict)
+        state_dict[utils.MODEL_KEY] = convert_weights.meta_to_tune(model_state_dict)
 
         if self._adapter_checkpoint:
             adapter_state_dict = safe_torch_load(self._adapter_checkpoint)
             state_dict[utils.ADAPTER_KEY] = adapter_state_dict
 
         if self._resume_from_checkpoint:
             recipe_state = safe_torch_load(self._recipe_checkpoint)
@@ -569,39 +558,25 @@
         state_dict: Dict[str, Any],
         epoch: int,
         intermediate_checkpoint: bool = False,
     ) -> None:
         """
         Save TorchTune checkpoint to file. If ``intermediate_checkpoint`` is True, an additional
         checkpoint file ``recipe_state.pt`` is created in ``_output_dir`` which contains the recipe
-        state. The output state dicts have the following formats:
-
-            Model:
-                {
-                    "key_1": weight
-                    ...
-                }
-
-            Recipe State:
-                {
-                    "optimizer": ...,
-                    "epoch": ...,
-                    ...
-                }
+        state.
 
         Args:
-            state_dict (Dict[str, Any]): State dict with model and (optionally) recipe state
-            epoch (int): Current epoch number. This is added to the checkpoint file name to ensure
-                we're not overwriting intermediate checkpoint files
-            intermediate_checkpoint (bool): If True, save an additional checkpoint file with the
-                recipe state
+            state_dict (Dict[str, Any]): Checkpoint state dict to be written out to file
+            epoch (int): Epoch number. Used to create the checkpoint file name
+            intermediate_checkpoint (bool): If True, an additional checkpoint files for recipe state
+                and (if applicable) adapter weights are created. Default is False
         """
         self._output_dir.mkdir(exist_ok=True)
         model_state_dict = state_dict[utils.MODEL_KEY]
-        state_dict[utils.MODEL_KEY] = llama2.tune_to_meta_llama2_7b(model_state_dict)
+        state_dict[utils.MODEL_KEY] = convert_weights.tune_to_meta(model_state_dict)
 
         # Output file is always a .pt file with the epoch number in the name
         checkpoint_file = Path.joinpath(
             self._output_dir, f"meta_model_{epoch}"
         ).with_suffix(".pt")
         torch.save(state_dict[utils.MODEL_KEY], checkpoint_file)
         logger.info(
```

## torchtune/utils/_checkpointing/_checkpointer_utils.py

```diff
@@ -1,22 +1,31 @@
 # Copyright (c) Meta Platforms, Inc. and affiliates.
 # All rights reserved.
 #
 # This source code is licensed under the BSD-style license found in the
 # LICENSE file in the root directory of this source tree.
 
+import json
 from enum import Enum
 from pathlib import Path
 from typing import Any, Dict
 
 import torch
+import torch.nn as nn
+import torch.optim as optim
+from safetensors import safe_open
+from torch.distributed.fsdp import FullyShardedDataParallel as FSDP
+
+from torchtune.utils._distributed import contains_fsdp
 
 
 class ModelType(Enum):
     LLAMA2 = "llama2"
+    MISTRAL = "mistral"
+    GEMMA = "gemma"
 
 
 def get_path(input_dir: Path, filename: str, missing_ok: bool = False) -> Path:
     """
     Utility to recover and validate the path for a given file within a given directory.
 
     Args:
@@ -37,20 +46,73 @@
 
     # If missing_ok is False, raise an error if the path is invalid
     if not missing_ok and not file_path.is_file():
         raise ValueError(f"No file with name: {filename} found in {input_dir}.")
     return file_path
 
 
-def safe_torch_load(checkpoint_path: Path) -> Dict[str, Any]:
+def safe_torch_load(checkpoint_path: Path, weights_only: bool = True) -> Dict[str, Any]:
     """
     Utility to load a checkpoint file in a safe manner.
     """
     try:
         # convert the path into a string since pathlib Path and mmap don't work
         # well together
-        state_dict = torch.load(
-            str(checkpoint_path), map_location="cpu", mmap=True, weights_only=True
+        is_safetensors_file = (
+            True if str(checkpoint_path).endswith(".safetensors") else False
         )
+        if is_safetensors_file:
+            result = {}
+            with safe_open(checkpoint_path, framework="pt", device="cpu") as f:
+                for k in f.keys():
+                    result[k] = f.get_tensor(k)
+            state_dict = result
+        else:
+            state_dict = torch.load(
+                str(checkpoint_path),
+                map_location="cpu",
+                mmap=True,
+                weights_only=weights_only,
+            )
     except Exception as e:
         raise ValueError(f"Unable to load checkpoint from {checkpoint_path}. ") from e
     return state_dict
+
+
+def transform_opt_state_dict(
+    opt_state_dict: Dict[str, Any], model: nn.Module, optimizer: optim.Optimizer
+) -> Dict[str, Any]:
+    """
+    Transforms the optimizer state dict for FSDP using the ``optim_state_dict_to_load``
+    from distributed library within PyTorch. If FSDP is not used, the optimizer state dict is returned as is.
+
+    Args:
+        opt_state_dict (Dict[str, Any]): Optimizer state dict extracted from the checkpoint
+        model (nn.Module): Model that checkpoint will be loaded into.
+        optimizer (optim.Optimizer): Optimizer that optimizer state checkpoints will be loaded into.
+
+    Returns:
+        ckpt_dict (Dict[str, Any]): Transformed optimizer state dict.
+    """
+    optim_state_dict_to_load = (
+        FSDP.optim_state_dict_to_load(model, optimizer, opt_state_dict)
+        if contains_fsdp(model)
+        else opt_state_dict
+    )
+
+    return optim_state_dict_to_load
+
+
+def save_config(path: Path, config: Dict[str, Any]) -> None:
+    """
+    Save a configuration dictionary to a file.
+
+    Args:
+        path (Path): Path to save the configuration file.
+        config (Dict[str, Any]): Configuration dictionary to save.
+    """
+    if not path.is_dir():
+        path.mkdir(exist_ok=True)
+    file_path = Path.joinpath(path, "config.json")
+    if not file_path.exists():
+        with open(file_path, "w") as f:
+            json.dump(config, f)
```

## Comparing `tests/torchtune/datasets/test_slimorca_dataset.py` & `torchtune/datasets/_chat.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,124 +1,142 @@
 # Copyright (c) Meta Platforms, Inc. and affiliates.
 # All rights reserved.
 #
 # This source code is licensed under the BSD-style license found in the
 # LICENSE file in the root directory of this source tree.
-from unittest.mock import patch
 
-import pytest
+from typing import Any, Callable, Dict, List, Mapping, Tuple
 
-from tests.test_utils import get_assets_path
+import numpy as np
 
-from torchtune.datasets._slimorca import _Llama2ChatFormatConstants, SlimOrcaDataset
-from torchtune.modules.tokenizer import Tokenizer
-
-
-class TestSlimOrcaDataset:
-    @pytest.fixture
-    def tokenizer(self):
-        # m.model is a pretrained Sentencepiece model using the following command:
-        # spm.SentencePieceTrainer.train('--input=<TRAIN_FILE> --model_prefix=m --vocab_size=2000')
-        return Tokenizer.from_file(str(get_assets_path() / "m.model"))
-
-    @patch("torchtune.datasets._slimorca.load_dataset")
-    def test_prompt_label_generation(self, load_dataset, tokenizer):
-        load_dataset.return_value = []
-        dataset = SlimOrcaDataset(tokenizer=tokenizer)
-        sample = [
-            {
-                "from": "system",
-                "value": "hi",
-            },
+from datasets import load_dataset
+from torch.utils.data import Dataset
+from torchtune.config._utils import _get_chat_format
+from torchtune.data import (
+    ChatFormat,
+    CROSS_ENTROPY_IGNORE_IDX,
+    Message,
+    sharegpt_to_llama2_messages,
+    validate_messages,
+)
+from torchtune.modules import Tokenizer
+
+
+class ChatDataset(Dataset):
+    """
+    Class that supports any custom dataset with multiturn conversations.
+
+    The general flow from loading a sample to tokenized prompt is:
+    load sample -> apply transform -> foreach turn{format into template -> tokenize}
+
+    If the column/key names differ from the expected names in the `ChatFormat`,
+    then the `column_map` argument can be used to provide this mapping.
+
+    Use `convert_to_messages` to prepare your dataset into the llama conversation format
+    and roles:
+        [
             {
-                "from": "human",
-                "value": "mid",
-            },
-            {
-                "from": "gpt",
-                "value": "lo",
+                "role": <system|user|assistant>,
+                "content": <message>,
             },
+            ...
         ]
-        prompt, label = dataset._generate_prompt_label(sample)
-        assert (
-            prompt
-            == f"{_Llama2ChatFormatConstants.B_INST} {_Llama2ChatFormatConstants.B_SYS}hi{_Llama2ChatFormatConstants.E_SYS}mid {_Llama2ChatFormatConstants.E_INST}"  # noqa: B950
-        )
-        assert label == " lo "
 
-        sample = [
-            {
-                "from": "human",
-                "value": "mid",
-            },
-            {
-                "from": "gpt",
-                "value": "lo",
-            },
-        ]
-        prompt, label = dataset._generate_prompt_label(sample)
-        assert (
-            prompt
-            == f"{_Llama2ChatFormatConstants.B_INST} mid {_Llama2ChatFormatConstants.E_INST}"
-        )
-        assert label == " lo "
+    This class supports multi-turn conversations. If a tokenizer sample with multiple
+    turns does not fit within `max_seq_len` then it is truncated.
 
-    @patch("torchtune.datasets._slimorca.load_dataset")
-    def test_token_generation(self, load_dataset, tokenizer):
-        load_dataset.return_value = []
-        dataset = SlimOrcaDataset(tokenizer=tokenizer, max_token_length=4096)
-        input, label = dataset._generate_tokens("Hello ", "world!")
-        assert input == [tokenizer.bos_id, 12, 1803, 1024, 103, tokenizer.eos_id]
-        assert label == ([-100] * 3 + [1024, 103, tokenizer.eos_id])
-
-    @patch("torchtune.datasets._slimorca.load_dataset")
-    def test_truncated_token_generation(self, load_dataset, tokenizer):
-        load_dataset.return_value = []
-        dataset = SlimOrcaDataset(tokenizer=tokenizer, max_token_length=5)
-        # 5 is enough for full prompt, but not for label
-        input, label = dataset._generate_tokens("Hello ", "world!")
-        assert input == [tokenizer.bos_id, 12, 1803, 1024, tokenizer.eos_id]
-        assert label == ([-100] * 3 + [1024, tokenizer.eos_id])
-
-        # 4 is not enough for full prompt nor response but truncation
-        # is still feasible
-        dataset = SlimOrcaDataset(tokenizer=tokenizer, max_token_length=4)
-        input, label = dataset._generate_tokens("Hello ", "world!")
-        assert input == [tokenizer.bos_id, 12, 1024, tokenizer.eos_id]
-        assert label == ([-100] * 2 + [1024, tokenizer.eos_id])
-
-    @patch("torchtune.datasets._slimorca.load_dataset")
-    def test_value_error(self, load_dataset, tokenizer):
-        load_dataset.return_value = []
-        with pytest.raises(ValueError):
-            SlimOrcaDataset(tokenizer=tokenizer, max_token_length=3)
-
-    @patch("torchtune.datasets._slimorca.load_dataset")
-    @pytest.mark.parametrize("max_token_length", [128, 512, 1024, 4096])
-    def test_dataset_get_item(self, load_dataset, tokenizer, max_token_length):
-        # Sample data from slimorca dataset
-        load_dataset.return_value = [
-            {
-                "conversations": [
-                    {
-                        "from": "system",
-                        "value": "You are an AI assistant. User will you give you a task. Your goal is to complete the task as faithfully as you can. While performing the task think step-by-step and justify your steps.",  # noqa: B950
-                    },
-                    {
-                        "from": "human",
-                        "value": "Please briefly summarize this news article:\n\nAOL.com Video - Father Lets 8-Year-Old Drive On Icy Road\n\nDescription:Would you let your 8-year-old drive your car? How about on an icy road? Well one father in Russia did just that, and recorded the entire thing. To her credit, the child seemed to be doing a great job. (0:44)\n\nTags: 8-year-old driver , caught on camera , child driver , pix11\n\nSummary:",  # noqa: B950
-                    },
-                    {
-                        "from": "gpt",
-                        "value": "A father in Russia allowed his 8-year-old child to drive his car on an icy road and recorded the event. The child appeared to be handling the situation well, showcasing their driving skills despite the challenging conditions.",  # noqa: B950
-                    },
-                ]
-            }
-        ]
-        ds = SlimOrcaDataset(tokenizer=tokenizer, max_token_length=max_token_length)
-        input, label = ds[0]
-        assert len(input) <= max_token_length
-        assert len(label) <= max_token_length
-        assert len(input) == len(label)
-        assert input[0] == tokenizer.bos_id
-        assert input[-1] == tokenizer.eos_id
-        assert label[-1] == tokenizer.eos_id
+    Args:
+        tokenizer (Tokenizer): Tokenizer used to encode data. Tokenize must implement an `encode` and `decode` method.
+        source (str): path string of dataset, anything supported by Hugging Face's `load_dataset`
+            (https://huggingface.co/docs/datasets/en/package_reference/loading_methods#datasets.load_dataset.path)
+        convert_to_messages (Callable[[Mapping[str, Any]], List[Message]]): function that keys into the desired field in the sample
+            and converts to a list of `Messages` that follows the llama format with the expected keys
+        chat_format (ChatFormat): template used to format the chat. If the placeholder variable
+            names in the template do not match the column/key names in the dataset, use `column_map` to map them.
+        max_seq_len (int): Maximum number of tokens in the returned input and label token id lists.
+        train_on_input (bool): Whether the model is trained on the prompt or not. Default is False.
+        **load_dataset_kwargs (Dict[str, Any]): additional keyword arguments to pass to `load_dataset`.
+    """
+
+    def __init__(
+        self,
+        tokenizer: Tokenizer,
+        source: str,
+        convert_to_messages: Callable[[Mapping[str, Any]], List[Message]],
+        chat_format: ChatFormat,
+        max_seq_len: int,
+        train_on_input: bool = False,
+        **load_dataset_kwargs: Dict[str, Any],
+    ) -> None:
+        self._tokenizer = tokenizer
+        self._data = load_dataset(source, **load_dataset_kwargs)
+        self._convert_to_messages = convert_to_messages
+        self.chat_format = chat_format
+        self.max_seq_len = max_seq_len
+        self.train_on_input = train_on_input
+
+    def __len__(self):
+        return len(self._data)
+
+    def __getitem__(self, index: int) -> Tuple[List[int], List[int]]:
+        sample = self._data[index]
+        return self._prepare_sample(sample)
+
+    def _prepare_sample(self, sample: Mapping[str, Any]) -> Tuple[List[int], List[int]]:
+        messages = self._convert_to_messages(sample, self.train_on_input)
+        messages = self.chat_format.format(messages)
+        validate_messages(messages)
+        tokens, mask = self._tokenizer.tokenize_messages(
+            messages, max_seq_len=self.max_seq_len
+        )
+        # Wherever mask == True, set to CROSS_ENTROPY_IGNORE_IDX. Otherwise keep as tokens
+        labels = list(np.where(mask, CROSS_ENTROPY_IGNORE_IDX, tokens))
+        assert len(tokens) == len(labels)
+
+        return tokens, labels
+
+
+def chat_dataset(
+    tokenizer: Tokenizer,
+    source: str,
+    conversation_style: str,
+    chat_format: str,
+    max_seq_len: int,
+    train_on_input: bool = False,
+    **load_dataset_kwargs: Dict[str, Any],
+) -> ChatDataset:
+    """
+    Build a configurable dataset with conversations. This method should be
+    used to configure a custom chat dataset from the yaml config instead of
+    using `ChatDataset` directly, as it is made to be config friendly.
+
+    Args:
+        tokenizer (Tokenizer): Tokenizer used to encode data. Tokenize must implement an `encode` and `decode` method.
+        source (str): path string of dataset, anything supported by Hugging Face's `load_dataset`
+            (https://huggingface.co/docs/datasets/en/package_reference/loading_methods#datasets.load_dataset.path)
+        conversation_style (str): string specifying expected style of conversations in the dataset
+            for automatic conversion to the llama style. Supported styles are: "sharegpt"
+        chat_format (str): name of ChatFormat class used to format the messages.
+        max_seq_len (int): Maximum number of tokens in the returned input and label token id lists.
+        train_on_input (bool): Whether the model is trained on the prompt or not. Default is False.
+        **load_dataset_kwargs (Dict[str, Any]): additional keyword arguments to pass to `load_dataset`.
+
+    Returns:
+        ChatDataset: the configured ChatDataset
+
+    Raises:
+        ValueError: if the conversation format is not supported
+    """
+    if conversation_style == "sharegpt":
+        convert_to_messages = sharegpt_to_llama2_messages
+    else:
+        raise ValueError(f"Unsupported conversation style: {conversation_style}")
+
+    return ChatDataset(
+        tokenizer=tokenizer,
+        source=source,
+        convert_to_messages=convert_to_messages,
+        chat_format=_get_chat_format(chat_format),
+        max_seq_len=max_seq_len,
+        train_on_input=train_on_input,
+        **load_dataset_kwargs,
+    )
```

## Comparing `torchtune/_cli/eval.py` & `recipes/eleuther_eval.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,231 +1,210 @@
 # Copyright (c) Meta Platforms, Inc. and affiliates.
 # All rights reserved.
 #
 # This source code is licensed under the BSD-style license found in the
 # LICENSE file in the root directory of this source tree.
 
-# Copyright (c) Meta Platforms, Inc. and affiliates.
-# All rights reserved.
-
-# This source code is licensed under the license found in the
-# LICENSE file in the root directory of this source tree.
 import sys
 import time
-from typing import Any, Dict, List, Optional
 
-import lm_eval
+from typing import Any, Dict, List
 
 import torch
-import torchtune.utils as utils
-from lm_eval.evaluator import evaluate
-from lm_eval.models.huggingface import HFLM
-from lm_eval.tasks import get_task_dict
 from omegaconf import DictConfig
-from torchtune import config
+
+from torch import nn
+
+from torchtune import config, utils
 from torchtune.modules import Tokenizer, TransformerDecoder
-from torchtune.utils import get_logger
+from torchtune.recipe_interfaces import EvalRecipeInterface
 
 
-logger = get_logger("DEBUG")
+logger = utils.get_logger("DEBUG")
 
-_default_tasks = ["hellaswag"]
+try:
+    import lm_eval
+    from lm_eval.evaluator import evaluate
+    from lm_eval.models.huggingface import HFLM
+    from lm_eval.tasks import get_task_dict
+except ImportError:
+    logger.error(
+        "Recipe requires EleutherAI Eval Harness v0.4. Please install with `pip install lm_eval==0.4.*`"
+    )
+    sys.exit(1)
 
 
 class _EvalWrapper(HFLM):
-    """
-    An EvalWrapper for EleutherAI's eval harness based on fast-gpt's
+    """An EvalWrapper for EleutherAI's eval harness based on gpt-fast's
     EvalWrapper: https://github.com/pytorch-labs/gpt-fast/blob/main/eval.py.
+
+    Args:
+        model (TransformerDecoder): The model to evaluate.
+        tokenizer (Tokenizer): The tokenizer to use.
+        device (torch.device): The device to use.
+        max_seq_length (int): The maximum sequence length to use.
+        batch_size (int): The batch size per GPU to use.
     """
 
     def __init__(
         self,
-        model,
-        tokenizer,
-        device,
-        max_seq_length,
+        model: TransformerDecoder,
+        tokenizer: Tokenizer,
+        *,
+        device: torch.device,
+        max_seq_length: int = 4096,
+        batch_size: int = 32,
     ):
         super().__init__(device=str(device))
         self._model = model
         self._tokenizer = tokenizer
         self._max_seq_length = max_seq_length
+        self._batch_size = batch_size
 
     @property
     def eot_token_id(self):
-        return self._tokenizer.eos_id()
+        return self._tokenizer.eos_id
 
     @property
     def max_length(self):
         return self._max_seq_length
 
     @property
     def max_gen_toks(self):
-        # Sample text from model undergoing eval until this maximum output length. Using
-        # 256 for now for parity with what eleuther does by default for HF models
-        # (https://github.com/EleutherAI/lm-evaluation-harness/blob/96d185fa6232a5ab685ba7c43e45d1dbb3bb906d/lm_eval/models/huggingface.py#L376),
-        # and we benchmark against HF llama-2 7b for correctness.
         return 256
 
     @property
     def batch_size(self):
-        # batch size used for evaluation
-        return 32
+        return self._batch_size
 
     @property
     def device(self):
         return self._device
 
-    def tok_encode(self, string: str, **kwargs):
+    def tok_encode(self, text: str, **kwargs) -> List[int]:
         # Note on add_bos flag: setting to False as this gives better results, for example
         # +1% on truthfulqa_mc2 with a LoRA finetune. lit-gpt also sets this to False,
         # see https://github.com/Lightning-AI/lit-gpt/blob/main/eval/lm_eval_harness.py#L66,
         # though notably fast-gpt does the opposite
         # https://github.com/pytorch-labs/gpt-fast/blob/main/eval.py#L123.
-        encoded = self._tokenizer.encode(text=string, add_bos=False, add_eos=False)
-        return encoded
-
-    def tok_decode(self, tokens):
-        decoded = self._tokenizer.decode(tokens)
-        return decoded
-
-    def _model_call(self, inps):
-        logits = self._model(inps)
-        return logits
-
-
-@torch.no_grad()
-def eval(
-    model: TransformerDecoder,
-    tokenizer: Tokenizer,
-    tasks: List[str],
-    limit: Optional[int] = None,
-    max_seq_length: Optional[int] = 4096,
-    device: torch.device = torch.device("cpu"),
-) -> Dict[str, Any]:
-    """
-    Evaluates a language model on a specified task using the lm-evaluation-harness library. Based
-    off of fast-gpt's evaluation wrapper: https://github.com/pytorch-labs/gpt-fast/blob/main/eval.py
+        return self._tokenizer.encode(text=text, add_bos=False, add_eos=False)
 
-    Args:
-        model (TransformerDecoder): The pre-trained or finetuned language model to evaluate.
-        tokenizer (Tokenizer): The tokenizer to use for encoding/decoding text.
-        tasks (List[str]): List of tasks to perform evaluation on.
-        limit (Optional[int]): The maximum number of samples to evaluate (None for all available).
-        max_seq_length (Optional[int]): The maximum sequence length allowed for input text. Defaults to 4096.
-        device (torch.device): torch.device indicating device to run eval on.
+    def tok_decode(self, tokens: List[int], **kwargs) -> str:
+        return self._tokenizer.decode(tokens)
 
-    Returns:
-        eval_results (Dict[str, Any]): A dictionary of evaluation results for the specified task(s).
-    """
+    def _model_call(self, inps: torch.Tensor, **kwargs) -> torch.Tensor:
+        return self._model(inps)
 
-    model_eval_wrapper = _EvalWrapper(
-        model,
-        tokenizer,
-        device,
-        max_seq_length,
-    )
+    def _model_generate(self, *args, **kwargs):
+        raise RuntimeError(
+            "This recipe does not currently support tasks that evaluate free generation,"
+            "e.g. `truthfulqa_gen` or `bigbench_color_generate_until`."
+        )
 
-    lm_eval.tasks.initialize_tasks()
 
-    task_dict = get_task_dict(tasks)
-    eval_results = evaluate(
-        model_eval_wrapper,
-        task_dict,
-        limit=limit,
-    )
-    return eval_results
+class EleutherEvalRecipe(EvalRecipeInterface):
+    """
+    This recipe runs evaluation on a trained model using EleutherAI's eval harness.
+    This assumes the user has the EleutherAI eval harness installed. See
+    https://github.com/EleutherAI/lm-evaluation-harness for more details.
 
+    Features:
+        - Single GPU evaluation. Multi-GPU evaluation is currently not supported.
+        - Loading model in fp32 or bf16. Fp16 is currently not supported.
+        - Any task from the EleutherAI eval harness that is *not* free generation
 
-def _load_checkpoint(checkpoint_path: str):
-    """
-    Loads a checkpoint from a given path.
-    TODO: checkpoint validation.
-    """
-    return torch.load(checkpoint_path, map_location="cpu", weights_only=True)
+    We recommend launching evaluation using the tune CLI:
 
+        tune run eleuther_eval --config llama2_eleuther_eval \
+        tasks=["truthfulqa_mc2","hellaswag"]
 
-def _setup_model(
-    cfg_model: DictConfig,
-    device: torch.device,
-    model_checkpoint: str,
-):
-    """
-    Sets up the model via passed in config, including loading checkpoint.
+    Args:
+        cfg (DictConfig): OmegaConf object parsed from YAML file
     """
-    # Load state_dicts from file.
-    base_model_state_dict = _load_checkpoint(model_checkpoint)
-
-    # Create model.
-    with device:
-        model = config.instantiate(cfg_model)
-
-    # Load state_dicts into model.
-    # TODO: Improve validation such as in training recipes.
-
-    # TODO: recent refactor removed "model", but some old checkpoints to test parity still have
-    # this key. Remove once full testing / validation is complete, or we re-write those checkpoints
-    # to remove "Model" key.
-    base_model_state_dict = (
-        base_model_state_dict["model"]
-        if "model" in base_model_state_dict
-        else base_model_state_dict
-    )
-    missing, unexpected = model.load_state_dict(base_model_state_dict, strict=False)
-    assert not unexpected, f"Unexpected keys {unexpected}"
-    assert not missing, f"Missing keys {missing}"
 
-    return model
+    def __init__(self, cfg: DictConfig) -> None:
+        self._cfg = cfg
 
+    def setup(self) -> None:
+        self._device = utils.get_device(device=self._cfg.device)
+        self._dtype = utils.get_dtype(dtype=self._cfg.dtype)
+        self._limit = self._cfg.limit
+        self._tasks = list(self._cfg.tasks)
+        self._quantizer = config.instantiate(self._cfg.quantizer)
+        self._quantization_mode = utils.get_quantizer_mode(self._quantizer)
+
+        utils.set_seed(seed=self._cfg.seed)
+
+        checkpointer = config.instantiate(self._cfg.checkpointer)
+        if self._quantization_mode is None:
+            ckpt_dict = checkpointer.load_checkpoint()
+        else:
+            # weights_only needs to be False when loading a quantized model
+            # currently loading a quantized model is only supported with the
+            # FullModelTorchTuneCheckpointer
+            ckpt_dict = checkpointer.load_checkpoint(weights_only=False)
+
+        self._model = self._setup_model(
+            model_cfg=self._cfg.model,
+            model_state_dict=ckpt_dict[utils.MODEL_KEY],
+        )
+        self._tokenizer = config.instantiate(self._cfg.tokenizer)
+        logger.info("Tokenizer is initialized from file.")
 
-@config.parse
-def main(
-    cfg: DictConfig,
-) -> None:
-    """
-    Main entry point for running evaluation on finetuned models. Sets up the environment,
-    loads in the model + checkpoint, and runs evaluation.
-
-    Example usage: tune eval --config eval_configs/full_finetune_eval_config.yaml --override limit=100 tasks=["truthfulqa_mc2"]
-    Please see eval_configs/ for example configs.
-    """
-    # Set up environment incl. device and random seed.
-    device = utils.get_device(device=cfg.device)
-    if cfg.seed is not None:
-        torch.manual_seed(cfg.seed)
-
-    # Set up model per configuration.
-    model = _setup_model(
-        cfg_model=cfg.model,
-        device=device,
-        model_checkpoint=cfg.model_checkpoint,
-    )
+    def _setup_model(
+        self,
+        model_cfg: DictConfig,
+        model_state_dict: Dict[str, Any],
+    ) -> nn.Module:
+        with utils.set_default_dtype(self._dtype), self._device:
+            model = config.instantiate(model_cfg)
+        if self._quantization_mode is not None:
+            model = self._quantizer.quantize(model)
+            model = model.to(device=self._device, dtype=self._dtype)
+
+        model.load_state_dict(model_state_dict)
+        # Validate model was loaded in with the expected dtype.
+        utils.validate_expected_param_dtype(model.named_parameters(), dtype=self._dtype)
+        logger.info(f"Model is initialized with precision {self._dtype}.")
+        return model
+
+    @torch.no_grad()
+    def evaluate(self) -> None:
+        t1 = time.time()
+
+        model_eval_wrapper = _EvalWrapper(
+            self._model,
+            self._tokenizer,
+            device=self._device,
+            max_seq_length=self._cfg.max_seq_length,
+        )
+
+        # Task initialization API changed between v0.4.1 and 0.4.2
+        try:
+            lm_eval.tasks.initialize_tasks()
+        except Exception:
+            pass
+
+        task_dict = get_task_dict(self._tasks)
+        logger.info(f"Running evaluation on {self._tasks} tasks.")
+        eleuther_output = evaluate(
+            model_eval_wrapper,
+            task_dict,
+            limit=self._limit,
+        )
+
+        logger.info(f"Eval completed in {time.time() - t1:.02f} seconds.")
+        for task, res in eleuther_output["results"].items():
+            logger.info(f"{task}: {res}")
 
-    # Set up tokenizer per configuration.
-    tokenizer = config.instantiate(cfg.tokenizer)
 
-    # Set up Eleuther tasks per configuration.
-    if not cfg.tasks:
-        task_list = _default_tasks
-    else:
-        # TODO: Is there a better way for Omega to instantiate list?
-        task_list = [task for task in cfg.tasks]
-
-    logger.info(f"Initialized model and tokenizer. Running eval on {task_list}.")
-
-    # Run evaluation.
-    t1 = time.time()
-    result = eval(
-        model=model,
-        tokenizer=tokenizer,
-        tasks=task_list,
-        limit=cfg.limit,
-        device=device,
-    )
-    # Report results.
-    logger.info(f"Time to run eval: {time.time() - t1:.02f} seconds.")
-    logger.info(f"For model {cfg.model_checkpoint}")
-    for task, res in result["results"].items():
-        print(f"{task}: {res}")
+@config.parse
+def recipe_main(cfg: DictConfig) -> None:
+    """Entry point for the recipe."""
+    config.log_config(recipe_name="EleutherEvalRecipe", cfg=cfg)
+    recipe = EleutherEvalRecipe(cfg=cfg)
+    recipe.setup()
+    recipe.evaluate()
 
 
 if __name__ == "__main__":
-    sys.exit(main())
+    sys.exit(recipe_main())
```

## Comparing `torchtune/data/_templates.py` & `torchtune/data/_instruct_templates.py`

 * *Files 20% similar despite different names*

```diff
@@ -4,44 +4,46 @@
 # This source code is licensed under the BSD-style license found in the
 # LICENSE file in the root directory of this source tree.
 
 from abc import ABC, abstractmethod
 from typing import Any, Dict, Mapping, Optional
 
 
-class PromptTemplate(ABC):
+class InstructTemplate(ABC):
     """
-    Interface for prompt templates. Each template should include the template
+    Interface for instruction templates. Each template should include the template
     prompt with placeholders for the data inputs.
     """
 
     template = ""
 
+    @classmethod
     @abstractmethod
     def format(
-        self, sample: Mapping[str, Any], column_map: Optional[Dict[str, str]] = None
+        cls, sample: Mapping[str, Any], column_map: Optional[Dict[str, str]] = None
     ) -> str:
         """
         Format the prompt template with the given arguments.
 
         Args:
             sample (Mapping[str, Any]): a single data sample with various fields
             column_map (Optional[Dict[str, str]]): a mapping from the expected
                 placeholder names in the template to the column names in the sample.
-                If None, assume these are identical.
+                If None, assume these are identical. Note: if the sample output is not named
+                as "output" in the dataset, you always need to map it to "output" in column_map.
 
         Returns:
             The formatted prompt
         """
         pass
 
 
-class AlpacaInstructTemplate(PromptTemplate):
+class AlpacaInstructTemplate(InstructTemplate):
     """
-    Prompt template for the Alpaca dataset. Template prompt changes slightly depending
+    Prompt template for Alpaca-style datasets. Template prompt changes slightly depending
     on if there's an instruction + input or just an instruction.
     """
 
     template = {
         "prompt_input": (
             "Below is an instruction that describes a task, paired with an input that provides further context. "
             "Write a response that appropriately completes the request.\n\n"
@@ -50,100 +52,126 @@
         "prompt_no_input": (
             "Below is an instruction that describes a task. "
             "Write a response that appropriately completes the request.\n\n"
             "### Instruction:\n{instruction}\n\n### Response:\n"
         ),
     }
 
+    @classmethod
     def format(
-        self, sample: Mapping[str, Any], column_map: Optional[Dict[str, str]] = None
+        cls, sample: Mapping[str, Any], column_map: Optional[Dict[str, str]] = None
     ) -> str:
         """
         Generate prompt from instruction and input.
 
         Args:
             sample (Mapping[str, Any]): a single data sample with instruction
             column_map (Optional[Dict[str, str]]): a mapping from the expected
                 placeholder names in the template to the column names in the sample.
                 If None, assume these are identical.
 
         Returns:
             The formatted prompt
         """
-        if column_map is not None:
-            key_input = column_map["input"]
-            key_instruction = column_map["instruction"]
-        else:
-            key_input = "input"
-            key_instruction = "instruction"
+        column_map = column_map or {}
+        key_input = column_map.get("input", "input")
+        key_instruction = column_map.get("instruction", "instruction")
 
         if key_input in sample and sample[key_input]:
-            prompt = self.template["prompt_input"].format(
+            prompt = cls.template["prompt_input"].format(
                 instruction=sample[key_instruction], input=sample[key_input]
             )
         else:
-            prompt = self.template["prompt_no_input"].format(
+            prompt = cls.template["prompt_no_input"].format(
                 instruction=sample[key_instruction]
             )
         return prompt
 
 
-class GrammarErrorCorrectionTemplate(PromptTemplate):
+class GrammarErrorCorrectionTemplate(InstructTemplate):
     """
-    Prompt template for the Grammar dataset.
+    Prompt template for grammar correction datasets.
     """
 
     template = "Correct this to standard English: {sentence}\n---\nCorrected: "
 
+    @classmethod
     def format(
-        self, sample: Mapping[str, Any], column_map: Optional[Dict[str, str]] = None
+        cls, sample: Mapping[str, Any], column_map: Optional[Dict[str, str]] = None
     ) -> str:
         """
         Generate prompt from sentence.
 
         Args:
             sample (Mapping[str, Any]): a single data sample with sentence
             column_map (Optional[Dict[str, str]]): a mapping from the expected
                 placeholder names in the template to the column names in the sample.
                 If None, assume these are identical.
 
         Returns:
             The formatted prompt
         """
-        if column_map is not None and "sentence" in column_map:
-            key_sentence = column_map["sentence"]
-        else:
-            key_sentence = "sentence"
+        column_map = column_map or {}
+        key_sentence = column_map.get("sentence", "sentence")
 
-        prompt = self.template.format(sentence=sample[key_sentence])
+        prompt = cls.template.format(sentence=sample[key_sentence])
         return prompt
 
 
-class SummarizeTemplate(PromptTemplate):
+class SummarizeTemplate(InstructTemplate):
     """
     Prompt template to format datasets for summarization tasks.
     """
 
     template = "Summarize this dialogue:\n{dialogue}\n---\nSummary:\n"
 
+    @classmethod
     def format(
-        self, sample: Mapping[str, Any], column_map: Optional[Dict[str, str]] = None
+        cls, sample: Mapping[str, Any], column_map: Optional[Dict[str, str]] = None
     ) -> str:
         """
         Generate prompt from dialogue.
 
         Args:
             sample (Mapping[str, Any]): a single data sample with dialog
             column_map (Optional[Dict[str, str]]): a mapping from the expected
                 placeholder names in the template to the column names in the sample.
                 If None, assume these are identical.
 
         Returns:
             The formatted prompt
         """
-        if column_map is not None and "dialogue" in column_map:
-            key_dialogue = column_map["dialogue"]
-        else:
-            key_dialogue = "dialogue"
+        column_map = column_map or {}
+        key_dialogue = column_map.get("dialogue", "dialogue")
+
+        prompt = cls.template.format(dialogue=sample[key_dialogue])
+        return prompt
+
+
+class StackExchangedPairedTemplate(InstructTemplate):
+    """
+    Prompt template for preference datasets similar to StackExchangedPaired.
+    """
+
+    template = "Question: {question}\n\nAnswer: "
+
+    @classmethod
+    def format(
+        cls, sample: Mapping[str, Any], column_map: Optional[Dict[str, str]] = None
+    ) -> str:
+        """
+        Generate prompt from instruction and input.
+
+        Args:
+            sample (Mapping[str, Any]): a single data sample with instruction
+            column_map (Optional[Dict[str, str]]): a mapping from the expected
+                placeholder names in the template to the column names in the sample.
+                If None, assume these are identical.
+
+        Returns:
+            The formatted prompt
+        """
+        column_map = column_map or {}
+        key_prompt = column_map.get("prompt", "prompt")
+        prompt = cls.template.format(question=sample[key_prompt])
 
-        prompt = self.template.format(dialogue=sample[key_dialogue])
         return prompt
```

## Comparing `torchtune-0.0.1.dist-info/LICENSE` & `torchtune-0.1.0.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `torchtune-0.0.1.dist-info/RECORD` & `torchtune-0.1.0.dist-info/RECORD`

 * *Files 26% similar despite different names*

```diff
@@ -1,122 +1,115 @@
-tests/__init__.py,sha256=Md3cCHD7Ano9kV15PqGbicgUO-RMdh4aVy1yKiDt_xE,208
-tests/common.py,sha256=xWJRo_UJB9KjgtgXEfsEirLgrfizHz1hWmOwxrCRlTA,246
-tests/conftest.py,sha256=KLE8HNITMWrD1JJsskVaGllWZxiOxQ7LQ2REqertCOQ,1464
-tests/test_utils.py,sha256=RsNVj-FD0ASGgANhvhvd9OzDqNhNfxmOvM5QklPPNgs,4110
-tests/recipes/__init__.py,sha256=Md3cCHD7Ano9kV15PqGbicgUO-RMdh4aVy1yKiDt_xE,208
-tests/recipes/common.py,sha256=1mto9yy-j5wwEfTJACIOiGl8DHf6QeY-a1NwXhZFzvk,276
-tests/recipes/test_alpaca_generate.py,sha256=tbWOThTdC_zSDvlI0pJ3somtfBKUwI4abrCkTkpNXVI,1575
-tests/recipes/test_configs.py,sha256=CKSlaa4QsS6sNJ1_JaKOdT8Zm3i0G9nCp5ss-RjgCFo,722
-tests/recipes/test_full_finetune.py,sha256=eMfsmvhRlTiRxCanTgv4AJi3wwBgdIru8s-N_SAu39E,11309
-tests/recipes/test_lora_finetune.py,sha256=IhG84ith0GeWnX3DIr26ks3-1cCDjjbk6gUOVCgWALM,11878
-tests/recipes/utils.py,sha256=NBYBZmLIyPpaI4Dw7nqp5rBUMIStH--jntdNu6oe4wU,4098
-tests/torchtune/__init__.py,sha256=Md3cCHD7Ano9kV15PqGbicgUO-RMdh4aVy1yKiDt_xE,208
-tests/torchtune/_cli/__init__.py,sha256=Md3cCHD7Ano9kV15PqGbicgUO-RMdh4aVy1yKiDt_xE,208
-tests/torchtune/_cli/test_convert_checkpoint.py,sha256=imUuD88jOm085QAwiGK1Sa9tKl22V1n74avP13kYbDo,5637
-tests/torchtune/_cli/test_cp.py,sha256=y1y8-MWcDFUr7pQ_CKdvTu6nJ2cF0p0IDjP6hjvtFY8,3041
-tests/torchtune/_cli/test_download.py,sha256=NXOk6-SzHvlT9_Aza48kp1129IU0QrNb9hqdqEpcLXQ,1228
-tests/torchtune/_cli/test_ls.py,sha256=B-ThuzemirK0QIoBNvLW0qSoQgvZlutuZLBH9-XsvXI,1141
-tests/torchtune/_cli/test_tune.py,sha256=nHhGyo3twj9f8UXTggLwTev6SdKmIGmn35sL_fZksAc,1096
-tests/torchtune/_cli/test_validate.py,sha256=C_7n2C2w9t_meeIWU7l9f-j2qDQiH7UDUg9jKKcMfDk,1673
-tests/torchtune/datasets/__init__.py,sha256=Md3cCHD7Ano9kV15PqGbicgUO-RMdh4aVy1yKiDt_xE,208
-tests/torchtune/datasets/test_alpaca_dataset.py,sha256=taqSG9YiFLYOfGJUGW-To-hrjE0msdneD4XHk-L7jrY,4342
-tests/torchtune/datasets/test_instruct_dataset.py,sha256=JM3EvzXP52SktbGPiqVi9XF1qoXREFHEqnk8TSaaKXc,4294
-tests/torchtune/datasets/test_slimorca_dataset.py,sha256=YRDAaY_npYNG_XJib-Jc3P5COtphJ4AYZqaxrkiJt4o,5652
-tests/torchtune/generation/__init__.py,sha256=Md3cCHD7Ano9kV15PqGbicgUO-RMdh4aVy1yKiDt_xE,208
-tests/torchtune/generation/test_generation.py,sha256=wM2Ose8WJwyifHm99T67tZ3hWW0F6IEcjZ9KP9nN7zA,9521
-tests/torchtune/models/__init__.py,sha256=Md3cCHD7Ano9kV15PqGbicgUO-RMdh4aVy1yKiDt_xE,208
-tests/torchtune/models/test_lora_llama2.py,sha256=mPuMCZt8QQ9v3o-YS5xyUzL2Wdhe8-qbphDaHBo2F3g,5343
-tests/torchtune/modules/__init__.py,sha256=Md3cCHD7Ano9kV15PqGbicgUO-RMdh4aVy1yKiDt_xE,208
-tests/torchtune/modules/test_attention.py,sha256=ZhqT8O-dHHIHxEP-BuXmRng5kRrUgKFQotmRZ9hbjN0,12938
-tests/torchtune/modules/test_cosine_with_warmup.py,sha256=z3cTmAg39GgPDtINqAUf9Fb1w5qn9Z3FWDNz1fb02tw,1942
-tests/torchtune/modules/test_feed_forward.py,sha256=IXNG39g8yRuo2zcvILxJQ1EtyizjTJTSAnDXqQjOXmE,1666
-tests/torchtune/modules/test_position_embeddings.py,sha256=9hiBt-fsHIySsKNnMCjygEGBz-X0bB6v4_DWzgiUnKg,2972
-tests/torchtune/modules/test_rms_norm.py,sha256=8Y9AOp9Wqx6-cm3ZlqHLZRKCzF_60DcgXZhK47yHXxI,2057
-tests/torchtune/modules/test_tokenizer.py,sha256=94xoIgqZpCvfpIfRVHGK2qKBNz7zQ23_kD3fcCjA0es,1783
-tests/torchtune/modules/test_transformer_decoder.py,sha256=fPa2BIFAd9vum8SjJQfuDbHz9BGpRuTzVj92d9cEm94,9041
-tests/torchtune/modules/low_precision/__init__.py,sha256=Md3cCHD7Ano9kV15PqGbicgUO-RMdh4aVy1yKiDt_xE,208
-tests/torchtune/modules/low_precision/test_nf4_linear.py,sha256=_Z1IiDc6GsAqmVRzkPIzhMNKwWwZyrrgnLRMka7g6cM,5045
-tests/torchtune/modules/peft/__init__.py,sha256=Md3cCHD7Ano9kV15PqGbicgUO-RMdh4aVy1yKiDt_xE,208
-tests/torchtune/modules/peft/test_lora.py,sha256=elZm01YBCBJlpFRXZ9dilPb7ccMvlAYKq07670zrnVE,2313
-tests/torchtune/modules/peft/test_peft_utils.py,sha256=g6fy8xpV3zSXi_2p4frjRvv_voJhlQr8YaLnreet9ls,12532
-tests/torchtune/utils/__init__.py,sha256=Md3cCHD7Ano9kV15PqGbicgUO-RMdh4aVy1yKiDt_xE,208
-tests/torchtune/utils/test_argparse.py,sha256=Ztcsz8qU9J692Hn6oNJH0JdftiMYZhcPvBblx_I6mvM,1614
-tests/torchtune/utils/test_checkpoint.py,sha256=kfHMGxWQbcwiL1-6EzZqASasINS_qbIQKT5IiolinvY,5946
-tests/torchtune/utils/test_checkpointable_dataloader.py,sha256=XIo7ZfSCyitu8eK6P7O8ZK6xMlQfbaKq4h0eaaXIJkI,8706
-tests/torchtune/utils/test_checkpointer.py,sha256=yYYrDXn347hiHk8TDTvvvQP2baAg4X92oBkfXDIn7Ko,11542
-tests/torchtune/utils/test_collate.py,sha256=PmpESjHvolXFPdLaX9c3_jnPnIT8bEASs7VB8zk9cwI,1238
-tests/torchtune/utils/test_device.py,sha256=4V2xifGT80_p9_EDf0FbqfxZqVKTPPadHoBXUWg0qV8,2470
-tests/torchtune/utils/test_distributed.py,sha256=NVyNQmqEu7-H3DMNLgIDjjPzTnTQCMv8JLUJrGNh9AY,9585
-tests/torchtune/utils/test_logits_transforms.py,sha256=X2DXV3EP6AuRVSk1ulDO6enZfSRl9R73LlqGcjb4nzY,2501
-tests/torchtune/utils/test_metric_logging.py,sha256=ncFMeKSY2yxsGC3B_F8QOZYA64JaYOruQNkuCym5ph4,5433
-tests/torchtune/utils/test_precision.py,sha256=ypXq6N-wgugf4CgS4rreHFFL7hPJY4N1ghynwiYlDNo,3459
-tests/torchtune/utils/test_seed.py,sha256=xHcWNdbccm345Muc9fi0DFa0xTIj-tBRbaJite4YkCA,2892
-tests/torchtune/utils/test_tensor_utils.py,sha256=TCKAAbawNbgpLyqzYVrdWJUMAS4oCebSJFuSVL5sws0,697
-torchtune/__init__.py,sha256=DUe9iWi0I0rSfoy6c5YqHxLvDBdGKWQITv3gOJy5oco,1188
-torchtune/recipe_interfaces.py,sha256=qKlp5kdfu79Lc-ZWuJBBj4Iq0bwM1Xrc82zlCvWk_FA,2201
-torchtune/_cli/__init__.py,sha256=WODosiG0mJMUHb_YLLP30jwuvv4p-t9sOEMDwTERAnc,366
-torchtune/_cli/convert_checkpoint.py,sha256=8L-pQ0vnADmRDkV4wu7yiQEyGvv7mUYLFBT64JlaWe4,4098
-torchtune/_cli/cp.py,sha256=8tvLnGoqNVmdTQBWG_IoQ5_pZbeB6QtLU4--evKZ4mM,3518
-torchtune/_cli/download.py,sha256=RD8gggramZf1Jf_4UvwWTcxp118msRJ379G161DFpiw,2140
-torchtune/_cli/eval.py,sha256=FSz-2Lc9TuBgxBJHIG__S-FnkpUIr8snur_CGEJWx94,7202
-torchtune/_cli/ls.py,sha256=ugo-AJayRwaR_d-V4oJ9Ia40V1EZRYrEb5DTIlLUprI,1784
-torchtune/_cli/tune.py,sha256=8IsOQGvcuSkueJJEnx-271AXdoeHCicUbKg-WfzUsOQ,5292
-torchtune/_cli/validate.py,sha256=sSXGehOLb7lA_QKVncM4xdB5Vsw7__p8q1ehbllo6x8,1145
-torchtune/config/__init__.py,sha256=_w5hmY1zD9FGVEVoJwUYznjP0h_8aggUA7CnKjUW8c0,368
+recipes/__init__.py,sha256=no8aE2zRiWMAkoPaKlysg0zZa1T3lRkYrceTFI5kxjs,1204
+recipes/eleuther_eval.py,sha256=qotaF8eSoUldYrbUFM8H8RuDsSp1qNZ5bJb989SQNQY,6999
+recipes/full_finetune_distributed.py,sha256=tGW9r6SOCCfcF0IHOUoaooX557Juy6I9tvhipTZlAT0,21147
+recipes/full_finetune_single_device.py,sha256=lRC2up9WfmteetFv6lN_c-DDNBEJgxo7-LvsdYuIRXE,21166
+recipes/generate.py,sha256=QMMxWyb2h2wFuTTsN70Bkaq2n9TRjDOIGT8XhbLPJqY,5144
+recipes/lora_dpo_single_device.py,sha256=MSU2m3nF-p_JvNglUSfL6H1ymxs11ByCkX-w8sTOt08,21497
+recipes/lora_finetune_distributed.py,sha256=fXA8F__AInV9vFEW_N6Kqnc4mBxuWFpR0Sf-RvaA6-w,25790
+recipes/lora_finetune_single_device.py,sha256=qRGChnpnxk6kwo4IOjUYbmM19_rXeuOHKK1dlm37-Rw,21491
+recipes/quantize.py,sha256=J0lIIESz-k7CcZ-BoUJMyeCgmcv3ccjzwbEA2r-9ycQ,4284
+recipes/configs/eleuther_evaluation.yaml,sha256=kbw8igAJy1Rn4j_ep7CZWDR9RhvbW4grUmro6zzgQDE,893
+recipes/configs/generation.yaml,sha256=-_NlKW9r2TCc_ytO2tjjBwTLNE1gpoihV2MyjqMLB7I,860
+recipes/configs/quantization.yaml,sha256=RWYyn3upYtNLgpitYGHz_vnhpcvhyizepq9Px14LWPk,664
+recipes/configs/gemma/2B_full.yaml,sha256=pHpwTsDUrRexEI-ivjDk4oiOQS2e2vBfnEPnZk5i668,1925
+recipes/configs/llama2/13B_full.yaml,sha256=3S-o7260e5BwmAGuB-i5jcBGg43DyIH6wmnTd0xnFC0,2163
+recipes/configs/llama2/13B_lora.yaml,sha256=VbzsK8cdNwJATWGYBAfE_ryCX6xDa2pDDmAf6BdONkQ,2441
+recipes/configs/llama2/7B_full.yaml,sha256=xMqrXS0r_uaff2tO6_jyfoUqJ3spVl8gai1Za8sR1x0,2083
+recipes/configs/llama2/7B_full_low_memory.yaml,sha256=giZeXJFVTAc0hPBa6SQ1gs5EqxhX-p972dl6zlmX3WU,2117
+recipes/configs/llama2/7B_lora.yaml,sha256=FzgupI16spliKSSq3WBMRIGWEGjJQZUFd9-TvXHvb6A,2326
+recipes/configs/llama2/7B_lora_dpo_single_device.yaml,sha256=ejg5X2jcTkFFFq0-AJ2CcwmFSvG9IdbRWUCdQ59iDH8,2262
+recipes/configs/llama2/7B_lora_single_device.yaml,sha256=2qIFFKnPoq3wTxVRwd7o1CVaNWxeiduFILD9z9TNhGQ,2423
+recipes/configs/llama2/7B_qlora_single_device.yaml,sha256=EHC7bwjzjmA6wjv9rruO6OKz2n3NJHEKBMtH22OlrKM,2528
+recipes/configs/mistral/7B_full.yaml,sha256=jDn1BFkj50J2hRh1P7kE89yFRf-AXjkPARdS9GjFW9s,2260
+recipes/configs/mistral/7B_full_low_memory.yaml,sha256=eaPMhASABLYRKEogOQVCchQ2fG1hjEAG1BBfhDtOniw,2321
+recipes/configs/mistral/7B_lora.yaml,sha256=KocHmgxTi-19QgRJzwdzMZjWP8ShLhnZEYTQY1I-0QQ,2502
+recipes/configs/mistral/7B_lora_single_device.yaml,sha256=29o-KdHrdB4yscORHjWt1IlosNvqyzZgHx8ni1RzmMY,2618
+recipes/configs/mistral/7B_qlora_single_device.yaml,sha256=J9n9j0xEtt_SmE4bicY8sytLPlCB4VnhSpilN5BE37U,2624
+torchtune/__init__.py,sha256=k-a9Z-LZSfEErv1rAUFE_aa7VkrHiltu3XC_sC9laD8,337
+torchtune/_recipe_registry.py,sha256=l03wiVYgbn9FAIUcMS6C94E3ocVq78Oy4hc6lNTcxRU,3707
+torchtune/recipe_interfaces.py,sha256=dZlJqmMuPVeaVRTWYKQeFHYDG2eTT0Thid9XXdrYm0M,2986
+torchtune/_cli/__init__.py,sha256=Md3cCHD7Ano9kV15PqGbicgUO-RMdh4aVy1yKiDt_xE,208
+torchtune/_cli/cp.py,sha256=K7lHVYYBYnUeL57ezg6GOfNkvTm9X3O1aLnx9aaAsYA,4285
+torchtune/_cli/download.py,sha256=jrGjNQbRgQbApc-sYTRM-3WUFVjbq_VZj-tirykMVYw,4516
+torchtune/_cli/ls.py,sha256=MZIEbLG-zDKkWqJLDWYtKBDx5zOLEeDMUJrEUmHwVIE,2334
+torchtune/_cli/run.py,sha256=HiAGXynG9MU1c9GZetRLgk2phxt5dGzEoo9zYpT_adI,7246
+torchtune/_cli/subcommand.py,sha256=jNSPqghuwu4iinHmuLRLJLF61dfQFMhHh6p4De_k22c,418
+torchtune/_cli/tune.py,sha256=xigrRZ7rThlo3EBRDfJELhYRzxjezckAV3YwlJM4Ico,1486
+torchtune/_cli/validate.py,sha256=q9ac66SVHgMTj4YBCkM3ijnTpjKl0td2wZwoJRt939Q,1837
+torchtune/_cli/hf_upload/upload.py,sha256=NHdIGKzsDLh7TXNC5yIwOzno04cCKdWZmbZGMRVfSuo,3702
+torchtune/config/__init__.py,sha256=Nw5DMSiF7P1jNxToKN01K-8BkFrXFUd2Q55hHf6wFzw,417
 torchtune/config/_errors.py,sha256=jwWwQr_b9MFo6llwo_DcoPz8aYL2N_6VMDGNxS4epAU,956
-torchtune/config/_instantiate.py,sha256=zry1B8mXJyhFEw8eNSC41_9YDM9gKvfF0R15O1NQEqc,3873
-torchtune/config/_parse.py,sha256=2ScvEkRXW5QKjE6ugi9cYQ09LiNci5tA4WrY99L7jlU,1766
-torchtune/config/_utils.py,sha256=9TwzlBT9TqSAiBjx3pFYVjZHotLWBbbzYxDpy1dqJxs,5819
+torchtune/config/_instantiate.py,sha256=gxETa_27u9-6rZdm2CN4W9iU3OmJDNzYoiSzogOweg8,3873
+torchtune/config/_parse.py,sha256=UV0iCINngaEb2PzFwnTJLq40oVMdBcpoEXVsO1AD1Z8,1598
+torchtune/config/_utils.py,sha256=6trOd21TK3wa2f9yYeP0g_6prjr48HyFPbS6MfkfJrY,8006
 torchtune/config/_validate.py,sha256=nLJZHy_GkL8kWJTmb42QQd-zQEih_yflpEooUS7ecLM,1636
-torchtune/data/__init__.py,sha256=I_kMbSt6N6yX7fcBI7glMlE3puB_KKq76tve-Wlqw3M,488
-torchtune/data/_templates.py,sha256=4dtU89TDbmSWIBmbtZZZrmZlHzKXWMg6BZuzDsZh9h4,5011
-torchtune/datasets/__init__.py,sha256=eUabFlkOgcrgU-csPGHMBvJGOenJ7F3cGYU3HyScE8c,460
-torchtune/datasets/_alpaca.py,sha256=4I63TdIQjCkyKqsYZT9B4WL2RxMnX21hbb25-qMezto,2563
-torchtune/datasets/_common.py,sha256=Ctlddql8czaLac8fIfeDn65gCsvhpckfuN8sieV1-0c,241
-torchtune/datasets/_instruct.py,sha256=uqnZk2mURuB0h4Mqtsc-kk1xq8MDVmHAvQkF_4g3x18,7153
-torchtune/datasets/_slimorca.py,sha256=K9gMajYup_Gc99lNmJIsU4EHKU1uPd1KkSk-F-kO4FI,5742
-torchtune/models/__init__.py,sha256=fFbSEL_M84VoWT_N8hKd8spA9iwYI0wzmuGUqVtI4ug,253
-torchtune/models/llama2/__init__.py,sha256=gX1_W3vVBdVT5522fStIrrDxBstFQJKx7UrZDvn2SIQ,771
+torchtune/data/__init__.py,sha256=6eMBug1N1MCOBSfk9b38Bhhflp1Lu0aIEVwvD0Un2tw,1136
+torchtune/data/_chat_formats.py,sha256=k_HymaLTPlz4V7AmGU6bDctVtMANrW3TwS0YiMZ2S4w,7107
+torchtune/data/_common.py,sha256=Ctlddql8czaLac8fIfeDn65gCsvhpckfuN8sieV1-0c,241
+torchtune/data/_converters.py,sha256=xNbDi3zJqhVq2dgBgGPPZXsIilxYO0H34AmbtvPWV00,1746
+torchtune/data/_instruct_templates.py,sha256=Fh3VrV6qlVw852na4ZJL46CeLpv8aFkM5sv7nH8oQTo,5989
+torchtune/data/_types.py,sha256=dgMN1AY5BU1QqmqKgaMemW_mRxNDtdYPrY8FA1LQo6w,402
+torchtune/data/_utils.py,sha256=D8LI8c9XylzC3Q4MSSRJuIHmA_bTNrvOUuP1lhiW19M,2401
+torchtune/datasets/__init__.py,sha256=luVSpZ0PmQJktQd4EOsaGw7dkIVuiyog9DBvJAHw0YI,939
+torchtune/datasets/_alpaca.py,sha256=gFauIYiRVerxWoyppRJ6WCPgfI1BIbewCs5PfUYzYQ0,2582
+torchtune/datasets/_chat.py,sha256=LUZDYoVkepFq7ggUF1roTwjnDiexHZ21h69WF-fc1hg,5940
+torchtune/datasets/_grammar.py,sha256=AazilwDw1dykxzkChkJwyYceJh1kxA8bXJGrb1ijgVs,2180
+torchtune/datasets/_instruct.py,sha256=kd6IpD8Dx7C84YPgMDovxOV055YPzq8rkfmCqg0U1_o,6793
+torchtune/datasets/_preference.py,sha256=QZrbSwFLxUoEJtsDMxaVlKyqJLF7_OnhV1hhGIQK91w,5038
+torchtune/datasets/_samsum.py,sha256=X_XfxhDKwv4uN-IyNDKdnZaSyX1I6fC1Zw4J_rVVH4Q,2086
+torchtune/datasets/_slimorca.py,sha256=xFhtcm-Bhz0CrqtELBFEhqhET7ptKmd7CPLKejKlG1U,2687
+torchtune/datasets/_stack_exchanged_paired.py,sha256=6nPyB0gZzNNp9lyUcw_Fl7jjmfHLptCLXU3n49ojJ_4,1449
+torchtune/models/__init__.py,sha256=8Y3tcvEUgMSZWt9PlwpgV717r7dTtnMcFExSAAZMkZc,286
+torchtune/models/convert_weights.py,sha256=J2hZUrMcxkPXjNXg3mBC_8La4FFhBGgjT6jdfwr9O2o,7447
+torchtune/models/gemma/__init__.py,sha256=yR7Vb15zV2JE2mslcw2YxLu4uYPwDks4LyXMsCZ2ad4,319
+torchtune/models/gemma/_component_builders.py,sha256=07PPo7emXEXTd6c0NOBbRvorYt8iBacmGSqk9P2exLk,4617
+torchtune/models/gemma/_model_builders.py,sha256=iAi4HJ5FbCF5-LKmuNZWOvra-mrJyK2CHY22B_cvzLw,1189
+torchtune/models/gemma/rms_norm.py,sha256=XcZepZ_6RsCQLnmu5snrTMSxwkMGKzXcE924gqZgo7o,910
+torchtune/models/gemma/transformer.py,sha256=UmbgnqM_2GoGgKCIzrEy8GeDr52258yI5MNk_fTsR5M,5077
+torchtune/models/llama2/__init__.py,sha256=ExJZbkjeD23UIapx7O0VSvFXLy1uAAuKHmpF7yFu6sM,774
 torchtune/models/llama2/_checkpoint_utils.py,sha256=WFpsQhDDmhg1u28mTYp8Aj1rXo6_uKBywupBRCzNtM4,6391
-torchtune/models/llama2/_component_builders.py,sha256=7IK0ASlYS4kWGTaBQWuOjPO8Psk_p3w58ZFPDqdw2u0,14979
-torchtune/models/llama2/_convert_weights.py,sha256=vx-t2HWAK4gxJ1vaBYoIXG5T5BLO1B2yxFrW8nWMQI0,5375
-torchtune/models/llama2/_model_builders.py,sha256=A77S-zsulGN2zaVWIyH_uwhAD7q7YuIinWfw6jXe8CM,3487
+torchtune/models/llama2/_component_builders.py,sha256=Us7sNgBi1GuZE_6jKCOeyIsKJvLtpAuAMU4P5yowYFI,14695
+torchtune/models/llama2/_model_builders.py,sha256=zVfdwdbk17vj1ztKcCAzzKGTJVKG2e1kv10ec46QZ80,6020
 torchtune/models/llama2/_model_utils.py,sha256=tz0Dxc-Lf_V2FZTcihLR7s1dT7Trsc0u3ZG3dpmZOuA,902
-torchtune/modules/__init__.py,sha256=CS-LXMit6WYbPReGRX3tAfwMvUYnLmSwknB4Gyoh0Jk,873
-torchtune/modules/attention.py,sha256=A_amdbLjFyB_CuZtdBUmrjxUHaMJwThKWDQrzMi7J3w,9155
-torchtune/modules/feed_forward.py,sha256=Kad70wx1PNOrfXQsyl8cdH11mBxNglnXFW6UytbXRpM,1103
-torchtune/modules/kv_cache.py,sha256=hfCYmvZTSziv6M3RpXCsRVSZ1YUktKLQLYC3n06ZYhI,2228
-torchtune/modules/lr_schedulers.py,sha256=PFZGJqTGn_f7Y_7ihJbIstAHCJ3HErzJGI0jj4FqU0k,1981
-torchtune/modules/position_embeddings.py,sha256=pHQCnPQR7bgMQrCJJInJ9VOeZfVhyIHdXtkeitJbCYA,4291
+torchtune/models/mistral/__init__.py,sha256=4HyA_kfuREzx1azO8PbWuAfnxsKNEotKdJeF_Engz30,519
+torchtune/models/mistral/_component_builders.py,sha256=4iLp7oI5pw3RumHUUyjk3uQQdpSwM0M4vCvI0Sn1Ak8,14328
+torchtune/models/mistral/_model_builders.py,sha256=ZtWWEfCu6_bWu6zzgCYtaMJ4-rnQCWDiyV2Qty7xEUk,3391
+torchtune/modules/__init__.py,sha256=0uBoLkAnyMr667EkLsryAK_NL-bGHRrpZ7_tvMKBr68,994
+torchtune/modules/attention.py,sha256=2MDfDGNW1R_jvV3P5MUju2ss-ZsFRxRorFriqGdZRTo,9266
+torchtune/modules/common_utils.py,sha256=YMDfO6e4MOOD8OJVYe0cX7Pi-nfcrYsOVVILQaU2dKw,2059
+torchtune/modules/feed_forward.py,sha256=ZevFfZOoZ-lcvPXFpbZL04ctNcTVF6BegTjr_v-Tf8Y,1200
+torchtune/modules/kv_cache.py,sha256=DCM3zuWQIXB_U9jczUdxaxQ687BQHhT7E8WpwuJIWkg,1845
+torchtune/modules/lr_schedulers.py,sha256=N7n7V1mvX-BNEp6uf-lDrLFPE1RqxR0bwd2HFcwym9s,1982
+torchtune/modules/position_embeddings.py,sha256=2ABqyXoyLx6CXRvTVN5JmYl0fCVJSoY4feAexXY9BP4,4621
 torchtune/modules/rms_norm.py,sha256=TbDCFRsgVtso4_PQ8sCt8kfs8APcZa8Ly0D8QtoFTHo,1273
-torchtune/modules/tokenizer.py,sha256=xOILO92UWj2aUHnM9kzYMjnf0Q9M5aMgnAlM6PfeEvQ,2720
-torchtune/modules/transformer.py,sha256=h7tUKFdlzb5HeyhA7JDyJhphWHFLw55W7W2adUgKJ9E,5276
-torchtune/modules/low_precision/__init__.py,sha256=Wc3aB5qCCYdxhj_oV3TpqhJiOYnEzics5AbXTxdXW9c,287
-torchtune/modules/low_precision/nf4_linear.py,sha256=RkzGPGTxONuRRps-A9uq2FUgtZ0SaPL0tnr5IrbwKTc,2942
-torchtune/modules/peft/__init__.py,sha256=uKZ9UNOM8RBXIHlm27Xe4BoN4LERoxmonSEDEKzEYjg,544
-torchtune/modules/peft/lora.py,sha256=Wx5fV7wZAoU0frHO4UPl_P6YisECheIog1HpsjvwBuE,4447
-torchtune/modules/peft/peft_utils.py,sha256=NIa1E7Q80CjMOzS9VxQV10AhazidHMwuQlf_FenGCyU,10703
-torchtune/utils/__init__.py,sha256=r23GCyjR449M4UdnnUETi2i6P8mllPtCA2nYEW5GEzU,1901
+torchtune/modules/tokenizer.py,sha256=6uCETYMHqrApVncumGJs0mZYcikpojI4cf4IH6pUxVA,8194
+torchtune/modules/transformer.py,sha256=RODa2pnyACMUb14XKbC16_L3mX52If4gtBEYCgdK354,7239
+torchtune/modules/loss/__init__.py,sha256=e_Gk5d8UTcsBatstAjbDAUmwPbD8KvSqom-pFWtEwSM,257
+torchtune/modules/loss/dpo.py,sha256=bjms-scq7QrN-8nHxT32oQaUhlDpjNwngE4cp_HgHlw,4554
+torchtune/modules/peft/__init__.py,sha256=-iMifYv2Hqko3mLl5oOcYbs_wY4RD0hBFqYELwwiDXo,636
+torchtune/modules/peft/lora.py,sha256=5aori-GLn7qm1qdq5jQZVdE9_N6GTPunH2PqZhcrYng,5749
+torchtune/modules/peft/peft_utils.py,sha256=9B61J-QDT1By-euQmAyn28uPCKfQSleuvfPCxn3W5fo,14306
+torchtune/utils/__init__.py,sha256=gIstF1M1jpAzDPWG-hH-1IjhYr7uH8NbCTD3pQvF1CM,2301
+torchtune/utils/_compile_utils.py,sha256=AfiAIgoJbKRNE9irI6K_PrWe7qlJ48LtDQ7YGuzkgsM,1509
 torchtune/utils/_device.py,sha256=MZIcGGnIxrqUkPBs7PJam4J5Gx_zQBagV6iUakIjv8I,3446
-torchtune/utils/_distributed.py,sha256=SCeErqGNPOW_Vex-OABrZLCgHCrLokYVplakO2i9TVY,11990
-torchtune/utils/argparse.py,sha256=TWIe_74DrCo6EBfEqLAwSdEWohF90pk8PpBkq4aVda8,2647
-torchtune/utils/checkpoint.py,sha256=dbFSAVmkckKRpnq3dP1KJUbzaFt82mq_PInCVGbNyLA,8552
-torchtune/utils/checkpointable_dataloader.py,sha256=SVyIZlFzBeylBYajxcaXUfeGbGbULCLqHNLN2ryPJO8,6898
-torchtune/utils/collate.py,sha256=Y5p0kfhMT1n4DZyRTuYptAN55qSnMXRBuOKvr7cAyzY,2239
+torchtune/utils/_distributed.py,sha256=aVIwWIffq_1sObFVX5UBm1EGExjUIeF5vRIu6XJp-PA,11462
+torchtune/utils/_generation.py,sha256=6qwK5zQga4Qbw1WgTosiwujjdsytvjfef33xrsoVN8M,5012
+torchtune/utils/_profiler.py,sha256=WWrPuyoCVGqO4PXssXpCw4ImDVPxVlKP6aqqreRFuyQ,1613
+torchtune/utils/_register_nf4_dispatch_ops.py,sha256=J2awWNb5lYxxR_QS8n3tDM6X_abPKXXJeETt-a4GLOE,1785
+torchtune/utils/argparse.py,sha256=EOHT5pEx_jmxJPrEtLZeSb3K9ezGO0Nm_viJZTcx7XY,2622
+torchtune/utils/collate.py,sha256=eIYIqChJpR7LDWKkq8l7WlCYh4Lu-D5tRD_3Posu7Wg,4845
 torchtune/utils/constants.py,sha256=E2Fi4xBCc1btiX9ti7X55f-h-6rHKl3DboCm9OoNcnQ,657
-torchtune/utils/generation.py,sha256=9gGmRNPiOu6exgdvDiBFV47G1fwBS-mid04OcHVVY5A,9479
 torchtune/utils/logging.py,sha256=k-qe0VoR30AF6dtkLvby6nzYkLYNT3hEyV-BbKIJQ6s,810
-torchtune/utils/logits_transforms.py,sha256=GneGfCEmQobS6W9Bf9YZiGfuzURIdFYPZp0ltxG8Sl0,3171
-torchtune/utils/memory.py,sha256=g6_P1LOJ3tMxMYI2__NgM9tk6IvnKC0GuyoPVdG4Bbs,2342
-torchtune/utils/metric_logging.py,sha256=JAnbhcGtVEJMR5BCLBEp92nP57_DSVZU7DQzYEt3nYk,7930
-torchtune/utils/precision.py,sha256=LMIY-bLxKc5E46LXKJ5Uup7Q5DSqIwE_BY0pYTp__uU,5264
+torchtune/utils/memory.py,sha256=fXhfVFtOKpqP8yZu5Pgrsytxuh7tSia-kx5Af_FokxA,7480
+torchtune/utils/metric_logging.py,sha256=zLHB-Nvnm7hfZ5Sr_Dwm6z189dMCZeHpI2n5M2pXQt4,9919
+torchtune/utils/precision.py,sha256=Iq5bVjwSh1mUlq6toZ_iq0vuxu10hWivf233Me89lz0,6399
+torchtune/utils/quantization.py,sha256=_oyKZKsxszFsZoktYv-YFFLnNC9d6czNY_KawHoteIg,1284
 torchtune/utils/seed.py,sha256=gCRaoyYNUcLM4Yeq2MDnZhEC5oqyvAQVpg2atdkO77k,3411
-torchtune/utils/tensor_utils.py,sha256=bo9Y7kbIcdMQDRsKUD6UMU0AquxtjRlbTMgZTSBsFnk,585
-torchtune/utils/_checkpointing/__init__.py,sha256=3eX6Yx1emi61ctO3uUOGwk2Z83RWL6QNO19HkVJuLTY,395
-torchtune/utils/_checkpointing/_checkpointer.py,sha256=YZJEXo5VbnpCm2c-2XdUTS0G__5orL638sxD7OBr7KY,26065
-torchtune/utils/_checkpointing/_checkpointer_utils.py,sha256=PgjeWSi4IhdafRH3zD3vDxu8xFLDsdAeer8qL0TVmEE,1726
-torchtune-0.0.1.dist-info/LICENSE,sha256=jveMLW54exA6BUjnO6LP5ovEabWw5vXn22SfExL08qY,1474
-torchtune-0.0.1.dist-info/METADATA,sha256=LzI6wKoY0seZJMTH4MpoZc_WhmiPusbAoT6cHZamSq8,10767
-torchtune-0.0.1.dist-info/WHEEL,sha256=yQN5g4mg4AybRjkgi-9yy4iQEFibGQmlz78Pik5Or-A,92
-torchtune-0.0.1.dist-info/entry_points.txt,sha256=V6VpdiAZzL1MrHve8PgY5rg975NIJfbdehu4Itk659Y,50
-torchtune-0.0.1.dist-info/top_level.txt,sha256=yPQv2H7yaoC_PZYCP1bhlXrYqGlR0UWVNJLevV3paTU,16
-torchtune-0.0.1.dist-info/RECORD,,
+torchtune/utils/_checkpointing/__init__.py,sha256=FEAB_MOI3fN2XgZ02WQr1uqTzVRHABgd5MhiRoSg7ZA,421
+torchtune/utils/_checkpointing/_checkpointer.py,sha256=b7r6H22zrFoIxZTi53VqCDe614whyspeopcey46hc_k,26322
+torchtune/utils/_checkpointing/_checkpointer_utils.py,sha256=4wzw7qrFnUOYigIteUDQ5W8LkWkWYGEuBJ4kKdVNbnE,3861
+torchtune-0.1.0.dist-info/LICENSE,sha256=jveMLW54exA6BUjnO6LP5ovEabWw5vXn22SfExL08qY,1474
+torchtune-0.1.0.dist-info/METADATA,sha256=tPNgPn6HZ8JiuWrffjDmDU331ukVPNUkAjaN1ywspdI,14827
+torchtune-0.1.0.dist-info/WHEEL,sha256=GJ7t_kWBFywbagK5eo9IoUwLW6oyOeTKmQ-9iHFVNxQ,92
+torchtune-0.1.0.dist-info/entry_points.txt,sha256=V6VpdiAZzL1MrHve8PgY5rg975NIJfbdehu4Itk659Y,50
+torchtune-0.1.0.dist-info/top_level.txt,sha256=e5HCz8F_XvIfggkyjYEGQr1dn9QbRi6Lvny7UV4jIY0,18
+torchtune-0.1.0.dist-info/RECORD,,
```

