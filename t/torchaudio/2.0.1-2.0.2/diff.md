# Comparing `tmp/torchaudio-2.0.1-cp39-cp39-win_amd64.whl.zip` & `tmp/torchaudio-2.0.2-cp39-cp39-win_amd64.whl.zip`

## zipinfo -v {}

 * *Differences in extra fields detected; using output from zipinfo -v*

```diff
@@ -1,41 +1,41 @@
 There is no zipfile comment.
 
 End-of-central-directory record:
 -------------------------------
 
-  Zip archive file size:                   2129163 (0000000000207D0Bh)
-  Actual end-cent-dir record offset:       2129141 (0000000000207CF5h)
-  Expected end-cent-dir record offset:     2129141 (0000000000207CF5h)
+  Zip archive file size:                   2129558 (0000000000207E96h)
+  Actual end-cent-dir record offset:       2129536 (0000000000207E80h)
+  Expected end-cent-dir record offset:     2129536 (0000000000207E80h)
   (based on the length of the central directory and its expected offset)
 
   This zipfile constitutes the sole disk of a single-part archive; its
   central directory contains 119 entries.
   The central directory is 12060 (0000000000002F1Ch) bytes long,
   and its (expected) offset in bytes from the beginning of the zipfile
-  is 2117081 (0000000000204DD9h).
+  is 2117476 (0000000000204F64h).
 
 
 Central directory entry #1:
 ---------------------------
 
-  torchaudio-2.0.1.dist-info/
+  torchaudio-2.0.2.dist-info/
 
   offset of local header from start of archive:   0
                                                   (0000000000000000h) bytes
   file system or operating system of origin:      Unix
   version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   1.0
   compression method:                             none (stored)
   file security status:                           not encrypted
   extended local header:                          no
-  file last modified on (DOS date/time):          2023 Mar 15 10:54:56
-  file last modified on (UT extra field modtime): 2023 Mar 15 17:54:56 local
-  file last modified on (UT extra field modtime): 2023 Mar 15 17:54:56 UTC
+  file last modified on (DOS date/time):          2023 May 6 14:35:50
+  file last modified on (UT extra field modtime): 2023 May 6 18:35:50 local
+  file last modified on (UT extra field modtime): 2023 May 6 18:35:50 UTC
   32-bit CRC value (hex):                         00000000
   compressed size:                                0 bytes
   uncompressed size:                              0 bytes
   length of filename:                             27 characters
   length of extra field:                          24 bytes
   length of file comment:                         0 characters
   disk number on which file begins:               disk 1
@@ -43,110 +43,110 @@
   Unix file attributes (040755 octal):            drwxr-xr-x
   MS-DOS file attributes (10 hex):                dir 
 
   The central-directory extra field contains:
   - A subfield with ID 0x5455 (universal time) and 5 data bytes.
     The local extra field has UTC/GMT modification/access times.
   - A subfield with ID 0x7875 (Unix UID/GID (any size)) and 11 data bytes:
-    01 04 e8 03 00 00 04 e8 03 00 00.
+    01 04 f5 01 00 00 04 14 00 00 00.
 
   There is no file comment.
 
 Central directory entry #2:
 ---------------------------
 
-  torchaudio-2.0.1.dist-info/LICENSE
+  torchaudio-2.0.2.dist-info/RECORD
 
   offset of local header from start of archive:   85
                                                   (0000000000000055h) bytes
   file system or operating system of origin:      Unix
   version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               maximum
   file security status:                           not encrypted
   extended local header:                          no
-  file last modified on (DOS date/time):          2023 Mar 15 10:54:56
-  file last modified on (UT extra field modtime): 2023 Mar 15 17:54:56 local
-  file last modified on (UT extra field modtime): 2023 Mar 15 17:54:56 UTC
-  32-bit CRC value (hex):                         fab9958b
-  compressed size:                                724 bytes
-  uncompressed size:                              1363 bytes
-  length of filename:                             34 characters
+  file last modified on (DOS date/time):          2023 May 6 14:35:54
+  file last modified on (UT extra field modtime): 2023 May 6 18:35:53 local
+  file last modified on (UT extra field modtime): 2023 May 6 18:35:53 UTC
+  32-bit CRC value (hex):                         b22d4768
+  compressed size:                                4560 bytes
+  uncompressed size:                              8832 bytes
+  length of filename:                             33 characters
   length of extra field:                          24 bytes
   length of file comment:                         0 characters
   disk number on which file begins:               disk 1
   apparent file type:                             text
-  Unix file attributes (100666 octal):            -rw-rw-rw-
+  Unix file attributes (100664 octal):            -rw-rw-r--
   MS-DOS file attributes (00 hex):                none
 
   The central-directory extra field contains:
   - A subfield with ID 0x5455 (universal time) and 5 data bytes.
     The local extra field has UTC/GMT modification/access times.
   - A subfield with ID 0x7875 (Unix UID/GID (any size)) and 11 data bytes:
-    01 04 e8 03 00 00 04 e8 03 00 00.
+    01 04 f5 01 00 00 04 14 00 00 00.
 
   There is no file comment.
 
 Central directory entry #3:
 ---------------------------
 
-  torchaudio-2.0.1.dist-info/METADATA
+  torchaudio-2.0.2.dist-info/LICENSE
 
-  offset of local header from start of archive:   901
-                                                  (0000000000000385h) bytes
+  offset of local header from start of archive:   4736
+                                                  (0000000000001280h) bytes
   file system or operating system of origin:      Unix
   version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               maximum
   file security status:                           not encrypted
   extended local header:                          no
-  file last modified on (DOS date/time):          2023 Mar 15 10:54:56
-  file last modified on (UT extra field modtime): 2023 Mar 15 17:54:56 local
-  file last modified on (UT extra field modtime): 2023 Mar 15 17:54:56 UTC
-  32-bit CRC value (hex):                         2998569f
-  compressed size:                                524 bytes
-  uncompressed size:                              1198 bytes
-  length of filename:                             35 characters
+  file last modified on (DOS date/time):          2023 May 6 14:35:50
+  file last modified on (UT extra field modtime): 2023 May 6 18:35:50 local
+  file last modified on (UT extra field modtime): 2023 May 6 18:35:50 UTC
+  32-bit CRC value (hex):                         fab9958b
+  compressed size:                                724 bytes
+  uncompressed size:                              1363 bytes
+  length of filename:                             34 characters
   length of extra field:                          24 bytes
   length of file comment:                         0 characters
   disk number on which file begins:               disk 1
   apparent file type:                             text
   Unix file attributes (100666 octal):            -rw-rw-rw-
   MS-DOS file attributes (00 hex):                none
 
   The central-directory extra field contains:
   - A subfield with ID 0x5455 (universal time) and 5 data bytes.
     The local extra field has UTC/GMT modification/access times.
   - A subfield with ID 0x7875 (Unix UID/GID (any size)) and 11 data bytes:
-    01 04 e8 03 00 00 04 e8 03 00 00.
+    01 04 f5 01 00 00 04 14 00 00 00.
 
   There is no file comment.
 
 Central directory entry #4:
 ---------------------------
 
-  torchaudio-2.0.1.dist-info/WHEEL
+  torchaudio-2.0.2.dist-info/WHEEL
 
-  offset of local header from start of archive:   1518
-                                                  (00000000000005EEh) bytes
+  offset of local header from start of archive:   5552
+                                                  (00000000000015B0h) bytes
   file system or operating system of origin:      Unix
   version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               maximum
   file security status:                           not encrypted
   extended local header:                          no
-  file last modified on (DOS date/time):          2023 Mar 15 10:54:56
-  file last modified on (UT extra field modtime): 2023 Mar 15 17:54:56 local
-  file last modified on (UT extra field modtime): 2023 Mar 15 17:54:56 UTC
+  file last modified on (DOS date/time):          2023 May 6 14:35:50
+  file last modified on (UT extra field modtime): 2023 May 6 18:35:50 local
+  file last modified on (UT extra field modtime): 2023 May 6 18:35:50 UTC
   32-bit CRC value (hex):                         1ad59a98
   compressed size:                                96 bytes
   uncompressed size:                              100 bytes
   length of filename:                             32 characters
   length of extra field:                          24 bytes
   length of file comment:                         0 characters
   disk number on which file begins:               disk 1
@@ -154,35 +154,35 @@
   Unix file attributes (100666 octal):            -rw-rw-rw-
   MS-DOS file attributes (00 hex):                none
 
   The central-directory extra field contains:
   - A subfield with ID 0x5455 (universal time) and 5 data bytes.
     The local extra field has UTC/GMT modification/access times.
   - A subfield with ID 0x7875 (Unix UID/GID (any size)) and 11 data bytes:
-    01 04 e8 03 00 00 04 e8 03 00 00.
+    01 04 f5 01 00 00 04 14 00 00 00.
 
   There is no file comment.
 
 Central directory entry #5:
 ---------------------------
 
-  torchaudio-2.0.1.dist-info/top_level.txt
+  torchaudio-2.0.2.dist-info/top_level.txt
 
-  offset of local header from start of archive:   1704
-                                                  (00000000000006A8h) bytes
+  offset of local header from start of archive:   5738
+                                                  (000000000000166Ah) bytes
   file system or operating system of origin:      Unix
   version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   1.0
   compression method:                             none (stored)
   file security status:                           not encrypted
   extended local header:                          no
-  file last modified on (DOS date/time):          2023 Mar 15 10:54:56
-  file last modified on (UT extra field modtime): 2023 Mar 15 17:54:56 local
-  file last modified on (UT extra field modtime): 2023 Mar 15 17:54:56 UTC
+  file last modified on (DOS date/time):          2023 May 6 14:35:50
+  file last modified on (UT extra field modtime): 2023 May 6 18:35:50 local
+  file last modified on (UT extra field modtime): 2023 May 6 18:35:50 UTC
   32-bit CRC value (hex):                         3e903c24
   compressed size:                                11 bytes
   uncompressed size:                              11 bytes
   length of filename:                             40 characters
   length of extra field:                          24 bytes
   length of file comment:                         0 characters
   disk number on which file begins:               disk 1
@@ -190,72 +190,72 @@
   Unix file attributes (100666 octal):            -rw-rw-rw-
   MS-DOS file attributes (00 hex):                none
 
   The central-directory extra field contains:
   - A subfield with ID 0x5455 (universal time) and 5 data bytes.
     The local extra field has UTC/GMT modification/access times.
   - A subfield with ID 0x7875 (Unix UID/GID (any size)) and 11 data bytes:
-    01 04 e8 03 00 00 04 e8 03 00 00.
+    01 04 f5 01 00 00 04 14 00 00 00.
 
   There is no file comment.
 
 Central directory entry #6:
 ---------------------------
 
-  torchaudio-2.0.1.dist-info/RECORD
+  torchaudio-2.0.2.dist-info/METADATA
 
-  offset of local header from start of archive:   1813
-                                                  (0000000000000715h) bytes
+  offset of local header from start of archive:   5847
+                                                  (00000000000016D7h) bytes
   file system or operating system of origin:      Unix
   version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               maximum
   file security status:                           not encrypted
   extended local header:                          no
-  file last modified on (DOS date/time):          2023 Mar 15 10:54:56
-  file last modified on (UT extra field modtime): 2023 Mar 15 17:54:56 local
-  file last modified on (UT extra field modtime): 2023 Mar 15 17:54:56 UTC
-  32-bit CRC value (hex):                         20211eb4
-  compressed size:                                4544 bytes
-  uncompressed size:                              8831 bytes
-  length of filename:                             33 characters
+  file last modified on (DOS date/time):          2023 May 6 14:35:50
+  file last modified on (UT extra field modtime): 2023 May 6 18:35:50 local
+  file last modified on (UT extra field modtime): 2023 May 6 18:35:50 UTC
+  32-bit CRC value (hex):                         54fdc96e
+  compressed size:                                526 bytes
+  uncompressed size:                              1198 bytes
+  length of filename:                             35 characters
   length of extra field:                          24 bytes
   length of file comment:                         0 characters
   disk number on which file begins:               disk 1
   apparent file type:                             text
-  Unix file attributes (100664 octal):            -rw-rw-r--
+  Unix file attributes (100666 octal):            -rw-rw-rw-
   MS-DOS file attributes (00 hex):                none
 
   The central-directory extra field contains:
   - A subfield with ID 0x5455 (universal time) and 5 data bytes.
     The local extra field has UTC/GMT modification/access times.
   - A subfield with ID 0x7875 (Unix UID/GID (any size)) and 11 data bytes:
-    01 04 e8 03 00 00 04 e8 03 00 00.
+    01 04 f5 01 00 00 04 14 00 00 00.
 
   There is no file comment.
 
 Central directory entry #7:
 ---------------------------
 
   torchaudio/
 
-  offset of local header from start of archive:   6448
-                                                  (0000000000001930h) bytes
+  offset of local header from start of archive:   6466
+                                                  (0000000000001942h) bytes
   file system or operating system of origin:      Unix
   version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   1.0
   compression method:                             none (stored)
   file security status:                           not encrypted
   extended local header:                          no
-  file last modified on (DOS date/time):          2023 Mar 15 10:54:56
-  file last modified on (UT extra field modtime): 2023 Mar 15 17:54:56 local
-  file last modified on (UT extra field modtime): 2023 Mar 15 17:54:56 UTC
+  file last modified on (DOS date/time):          2023 May 6 14:35:50
+  file last modified on (UT extra field modtime): 2023 May 6 18:35:50 local
+  file last modified on (UT extra field modtime): 2023 May 6 18:35:50 UTC
   32-bit CRC value (hex):                         00000000
   compressed size:                                0 bytes
   uncompressed size:                              0 bytes
   length of filename:                             11 characters
   length of extra field:                          24 bytes
   length of file comment:                         0 characters
   disk number on which file begins:               disk 1
@@ -263,3350 +263,3350 @@
   Unix file attributes (040755 octal):            drwxr-xr-x
   MS-DOS file attributes (10 hex):                dir 
 
   The central-directory extra field contains:
   - A subfield with ID 0x5455 (universal time) and 5 data bytes.
     The local extra field has UTC/GMT modification/access times.
   - A subfield with ID 0x7875 (Unix UID/GID (any size)) and 11 data bytes:
-    01 04 e8 03 00 00 04 e8 03 00 00.
+    01 04 f5 01 00 00 04 14 00 00 00.
 
   There is no file comment.
 
 Central directory entry #8:
 ---------------------------
 
-  torchaudio/utils/
+  torchaudio/_internal/
 
-  offset of local header from start of archive:   6517
-                                                  (0000000000001975h) bytes
+  offset of local header from start of archive:   6535
+                                                  (0000000000001987h) bytes
   file system or operating system of origin:      Unix
   version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   1.0
   compression method:                             none (stored)
   file security status:                           not encrypted
   extended local header:                          no
-  file last modified on (DOS date/time):          2023 Mar 15 10:54:56
-  file last modified on (UT extra field modtime): 2023 Mar 15 17:54:56 local
-  file last modified on (UT extra field modtime): 2023 Mar 15 17:54:56 UTC
+  file last modified on (DOS date/time):          2023 May 6 14:35:50
+  file last modified on (UT extra field modtime): 2023 May 6 18:35:50 local
+  file last modified on (UT extra field modtime): 2023 May 6 18:35:50 UTC
   32-bit CRC value (hex):                         00000000
   compressed size:                                0 bytes
   uncompressed size:                              0 bytes
-  length of filename:                             17 characters
+  length of filename:                             21 characters
   length of extra field:                          24 bytes
   length of file comment:                         0 characters
   disk number on which file begins:               disk 1
   apparent file type:                             binary
   Unix file attributes (040755 octal):            drwxr-xr-x
   MS-DOS file attributes (10 hex):                dir 
 
   The central-directory extra field contains:
   - A subfield with ID 0x5455 (universal time) and 5 data bytes.
     The local extra field has UTC/GMT modification/access times.
   - A subfield with ID 0x7875 (Unix UID/GID (any size)) and 11 data bytes:
-    01 04 e8 03 00 00 04 e8 03 00 00.
+    01 04 f5 01 00 00 04 14 00 00 00.
 
   There is no file comment.
 
 Central directory entry #9:
 ---------------------------
 
-  torchaudio/utils/sox_utils.py
+  torchaudio/_internal/__init__.py
 
-  offset of local header from start of archive:   6592
-                                                  (00000000000019C0h) bytes
+  offset of local header from start of archive:   6614
+                                                  (00000000000019D6h) bytes
   file system or operating system of origin:      Unix
   version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               maximum
   file security status:                           not encrypted
   extended local header:                          no
-  file last modified on (DOS date/time):          2023 Mar 15 17:25:54
-  file last modified on (UT extra field modtime): 2023 Mar 16 00:25:54 local
-  file last modified on (UT extra field modtime): 2023 Mar 16 00:25:54 UTC
-  32-bit CRC value (hex):                         e066d13d
-  compressed size:                                808 bytes
-  uncompressed size:                              2973 bytes
-  length of filename:                             29 characters
+  file last modified on (DOS date/time):          2023 May 4 22:38:58
+  file last modified on (UT extra field modtime): 2023 May 5 02:38:58 local
+  file last modified on (UT extra field modtime): 2023 May 5 02:38:58 UTC
+  32-bit CRC value (hex):                         55cc8166
+  compressed size:                                95 bytes
+  uncompressed size:                              152 bytes
+  length of filename:                             32 characters
   length of extra field:                          24 bytes
   length of file comment:                         0 characters
   disk number on which file begins:               disk 1
   apparent file type:                             text
   Unix file attributes (100666 octal):            -rw-rw-rw-
   MS-DOS file attributes (00 hex):                none
 
   The central-directory extra field contains:
   - A subfield with ID 0x5455 (universal time) and 5 data bytes.
     The local extra field has UTC/GMT modification/access times.
   - A subfield with ID 0x7875 (Unix UID/GID (any size)) and 11 data bytes:
-    01 04 e8 03 00 00 04 e8 03 00 00.
+    01 04 f5 01 00 00 04 14 00 00 00.
 
   There is no file comment.
 
 Central directory entry #10:
 ---------------------------
 
-  torchaudio/utils/ffmpeg_utils.py
+  torchaudio/_internal/module_utils.py
 
-  offset of local header from start of archive:   7487
-                                                  (0000000000001D3Fh) bytes
+  offset of local header from start of archive:   6799
+                                                  (0000000000001A8Fh) bytes
   file system or operating system of origin:      Unix
   version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               maximum
   file security status:                           not encrypted
   extended local header:                          no
-  file last modified on (DOS date/time):          2023 Mar 15 17:25:54
-  file last modified on (UT extra field modtime): 2023 Mar 16 00:25:54 local
-  file last modified on (UT extra field modtime): 2023 Mar 16 00:25:54 UTC
-  32-bit CRC value (hex):                         9fcc166e
-  compressed size:                                2120 bytes
-  uncompressed size:                              8947 bytes
-  length of filename:                             32 characters
+  file last modified on (DOS date/time):          2023 May 4 22:38:58
+  file last modified on (UT extra field modtime): 2023 May 5 02:38:58 local
+  file last modified on (UT extra field modtime): 2023 May 5 02:38:58 UTC
+  32-bit CRC value (hex):                         32a076ff
+  compressed size:                                1042 bytes
+  uncompressed size:                              2694 bytes
+  length of filename:                             36 characters
   length of extra field:                          24 bytes
   length of file comment:                         0 characters
   disk number on which file begins:               disk 1
   apparent file type:                             text
   Unix file attributes (100666 octal):            -rw-rw-rw-
   MS-DOS file attributes (00 hex):                none
 
   The central-directory extra field contains:
   - A subfield with ID 0x5455 (universal time) and 5 data bytes.
     The local extra field has UTC/GMT modification/access times.
   - A subfield with ID 0x7875 (Unix UID/GID (any size)) and 11 data bytes:
-    01 04 e8 03 00 00 04 e8 03 00 00.
+    01 04 f5 01 00 00 04 14 00 00 00.
 
   There is no file comment.
 
 Central directory entry #11:
 ---------------------------
 
-  torchaudio/utils/download.py
+  torchaudio/version.py
 
-  offset of local header from start of archive:   9697
-                                                  (00000000000025E1h) bytes
+  offset of local header from start of archive:   7935
+                                                  (0000000000001EFFh) bytes
   file system or operating system of origin:      Unix
   version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               maximum
   file security status:                           not encrypted
   extended local header:                          no
-  file last modified on (DOS date/time):          2023 Mar 15 17:25:54
-  file last modified on (UT extra field modtime): 2023 Mar 16 00:25:54 local
-  file last modified on (UT extra field modtime): 2023 Mar 16 00:25:54 UTC
-  32-bit CRC value (hex):                         14935dc0
-  compressed size:                                1165 bytes
-  uncompressed size:                              2928 bytes
-  length of filename:                             28 characters
+  file last modified on (DOS date/time):          2023 May 4 22:41:06
+  file last modified on (UT extra field modtime): 2023 May 5 02:41:06 local
+  file last modified on (UT extra field modtime): 2023 May 5 02:41:06 UTC
+  32-bit CRC value (hex):                         eca756d0
+  compressed size:                                77 bytes
+  uncompressed size:                              85 bytes
+  length of filename:                             21 characters
   length of extra field:                          24 bytes
   length of file comment:                         0 characters
   disk number on which file begins:               disk 1
   apparent file type:                             text
   Unix file attributes (100666 octal):            -rw-rw-rw-
   MS-DOS file attributes (00 hex):                none
 
   The central-directory extra field contains:
   - A subfield with ID 0x5455 (universal time) and 5 data bytes.
     The local extra field has UTC/GMT modification/access times.
   - A subfield with ID 0x7875 (Unix UID/GID (any size)) and 11 data bytes:
-    01 04 e8 03 00 00 04 e8 03 00 00.
+    01 04 f5 01 00 00 04 14 00 00 00.
 
   There is no file comment.
 
 Central directory entry #12:
 ---------------------------
 
-  torchaudio/utils/__init__.py
+  torchaudio/kaldi_io.py
 
-  offset of local header from start of archive:   10948
-                                                  (0000000000002AC4h) bytes
+  offset of local header from start of archive:   8091
+                                                  (0000000000001F9Bh) bytes
   file system or operating system of origin:      Unix
   version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               maximum
   file security status:                           not encrypted
   extended local header:                          no
-  file last modified on (DOS date/time):          2023 Mar 15 17:25:54
-  file last modified on (UT extra field modtime): 2023 Mar 16 00:25:54 local
-  file last modified on (UT extra field modtime): 2023 Mar 16 00:25:54 UTC
-  32-bit CRC value (hex):                         434b998e
-  compressed size:                                94 bytes
-  uncompressed size:                              159 bytes
-  length of filename:                             28 characters
+  file last modified on (DOS date/time):          2023 May 4 22:38:58
+  file last modified on (UT extra field modtime): 2023 May 5 02:38:58 local
+  file last modified on (UT extra field modtime): 2023 May 5 02:38:58 UTC
+  32-bit CRC value (hex):                         982193e9
+  compressed size:                                1149 bytes
+  uncompressed size:                              5217 bytes
+  length of filename:                             22 characters
   length of extra field:                          24 bytes
   length of file comment:                         0 characters
   disk number on which file begins:               disk 1
   apparent file type:                             text
   Unix file attributes (100666 octal):            -rw-rw-rw-
   MS-DOS file attributes (00 hex):                none
 
   The central-directory extra field contains:
   - A subfield with ID 0x5455 (universal time) and 5 data bytes.
     The local extra field has UTC/GMT modification/access times.
   - A subfield with ID 0x7875 (Unix UID/GID (any size)) and 11 data bytes:
-    01 04 e8 03 00 00 04 e8 03 00 00.
+    01 04 f5 01 00 00 04 14 00 00 00.
 
   There is no file comment.
 
 Central directory entry #13:
 ---------------------------
 
-  torchaudio/transforms/
+  torchaudio/datasets/
 
-  offset of local header from start of archive:   11128
-                                                  (0000000000002B78h) bytes
+  offset of local header from start of archive:   9320
+                                                  (0000000000002468h) bytes
   file system or operating system of origin:      Unix
   version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   1.0
   compression method:                             none (stored)
   file security status:                           not encrypted
   extended local header:                          no
-  file last modified on (DOS date/time):          2023 Mar 15 10:54:56
-  file last modified on (UT extra field modtime): 2023 Mar 15 17:54:56 local
-  file last modified on (UT extra field modtime): 2023 Mar 15 17:54:56 UTC
+  file last modified on (DOS date/time):          2023 May 6 14:35:50
+  file last modified on (UT extra field modtime): 2023 May 6 18:35:50 local
+  file last modified on (UT extra field modtime): 2023 May 6 18:35:50 UTC
   32-bit CRC value (hex):                         00000000
   compressed size:                                0 bytes
   uncompressed size:                              0 bytes
-  length of filename:                             22 characters
+  length of filename:                             20 characters
   length of extra field:                          24 bytes
   length of file comment:                         0 characters
   disk number on which file begins:               disk 1
   apparent file type:                             binary
   Unix file attributes (040755 octal):            drwxr-xr-x
   MS-DOS file attributes (10 hex):                dir 
 
   The central-directory extra field contains:
   - A subfield with ID 0x5455 (universal time) and 5 data bytes.
     The local extra field has UTC/GMT modification/access times.
   - A subfield with ID 0x7875 (Unix UID/GID (any size)) and 11 data bytes:
-    01 04 e8 03 00 00 04 e8 03 00 00.
+    01 04 f5 01 00 00 04 14 00 00 00.
 
   There is no file comment.
 
 Central directory entry #14:
 ---------------------------
 
-  torchaudio/transforms/_transforms.py
+  torchaudio/datasets/speechcommands.py
 
-  offset of local header from start of archive:   11208
-                                                  (0000000000002BC8h) bytes
+  offset of local header from start of archive:   9398
+                                                  (00000000000024B6h) bytes
   file system or operating system of origin:      Unix
   version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               maximum
   file security status:                           not encrypted
   extended local header:                          no
-  file last modified on (DOS date/time):          2023 Mar 15 17:25:54
-  file last modified on (UT extra field modtime): 2023 Mar 16 00:25:54 local
-  file last modified on (UT extra field modtime): 2023 Mar 16 00:25:54 UTC
-  32-bit CRC value (hex):                         eda92084
-  compressed size:                                15984 bytes
-  uncompressed size:                              86790 bytes
-  length of filename:                             36 characters
+  file last modified on (DOS date/time):          2023 May 4 22:38:58
+  file last modified on (UT extra field modtime): 2023 May 5 02:38:58 local
+  file last modified on (UT extra field modtime): 2023 May 5 02:38:58 UTC
+  32-bit CRC value (hex):                         585820af
+  compressed size:                                2478 bytes
+  uncompressed size:                              7653 bytes
+  length of filename:                             37 characters
   length of extra field:                          24 bytes
   length of file comment:                         0 characters
   disk number on which file begins:               disk 1
   apparent file type:                             text
   Unix file attributes (100666 octal):            -rw-rw-rw-
   MS-DOS file attributes (00 hex):                none
 
   The central-directory extra field contains:
   - A subfield with ID 0x5455 (universal time) and 5 data bytes.
     The local extra field has UTC/GMT modification/access times.
   - A subfield with ID 0x7875 (Unix UID/GID (any size)) and 11 data bytes:
-    01 04 e8 03 00 00 04 e8 03 00 00.
+    01 04 f5 01 00 00 04 14 00 00 00.
 
   There is no file comment.
 
 Central directory entry #15:
 ---------------------------
 
-  torchaudio/transforms/_multi_channel.py
+  torchaudio/datasets/librilight_limited.py
 
-  offset of local header from start of archive:   27286
-                                                  (0000000000006A96h) bytes
+  offset of local header from start of archive:   11971
+                                                  (0000000000002EC3h) bytes
   file system or operating system of origin:      Unix
   version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               maximum
   file security status:                           not encrypted
   extended local header:                          no
-  file last modified on (DOS date/time):          2023 Mar 15 17:25:54
-  file last modified on (UT extra field modtime): 2023 Mar 16 00:25:54 local
-  file last modified on (UT extra field modtime): 2023 Mar 16 00:25:54 UTC
-  32-bit CRC value (hex):                         626f7039
-  compressed size:                                3979 bytes
-  uncompressed size:                              22688 bytes
-  length of filename:                             39 characters
+  file last modified on (DOS date/time):          2023 May 4 22:38:58
+  file last modified on (UT extra field modtime): 2023 May 5 02:38:58 local
+  file last modified on (UT extra field modtime): 2023 May 5 02:38:58 UTC
+  32-bit CRC value (hex):                         eeddfe87
+  compressed size:                                1657 bytes
+  uncompressed size:                              4279 bytes
+  length of filename:                             41 characters
   length of extra field:                          24 bytes
   length of file comment:                         0 characters
   disk number on which file begins:               disk 1
   apparent file type:                             text
   Unix file attributes (100666 octal):            -rw-rw-rw-
   MS-DOS file attributes (00 hex):                none
 
   The central-directory extra field contains:
   - A subfield with ID 0x5455 (universal time) and 5 data bytes.
     The local extra field has UTC/GMT modification/access times.
   - A subfield with ID 0x7875 (Unix UID/GID (any size)) and 11 data bytes:
-    01 04 e8 03 00 00 04 e8 03 00 00.
+    01 04 f5 01 00 00 04 14 00 00 00.
 
   There is no file comment.
 
 Central directory entry #16:
 ---------------------------
 
-  torchaudio/transforms/__init__.py
+  torchaudio/datasets/dr_vctk.py
 
-  offset of local header from start of archive:   31362
-                                                  (0000000000007A82h) bytes
+  offset of local header from start of archive:   13727
+                                                  (000000000000359Fh) bytes
   file system or operating system of origin:      Unix
   version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               maximum
   file security status:                           not encrypted
   extended local header:                          no
-  file last modified on (DOS date/time):          2023 Mar 15 17:25:54
-  file last modified on (UT extra field modtime): 2023 Mar 16 00:25:54 local
-  file last modified on (UT extra field modtime): 2023 Mar 16 00:25:54 UTC
-  32-bit CRC value (hex):                         cb82ee15
-  compressed size:                                445 bytes
-  uncompressed size:                              1307 bytes
-  length of filename:                             33 characters
+  file last modified on (DOS date/time):          2023 May 4 22:38:58
+  file last modified on (UT extra field modtime): 2023 May 5 02:38:58 local
+  file last modified on (UT extra field modtime): 2023 May 5 02:38:58 UTC
+  32-bit CRC value (hex):                         d86ec8a6
+  compressed size:                                1525 bytes
+  uncompressed size:                              4487 bytes
+  length of filename:                             30 characters
   length of extra field:                          24 bytes
   length of file comment:                         0 characters
   disk number on which file begins:               disk 1
   apparent file type:                             text
   Unix file attributes (100666 octal):            -rw-rw-rw-
   MS-DOS file attributes (00 hex):                none
 
   The central-directory extra field contains:
   - A subfield with ID 0x5455 (universal time) and 5 data bytes.
     The local extra field has UTC/GMT modification/access times.
   - A subfield with ID 0x7875 (Unix UID/GID (any size)) and 11 data bytes:
-    01 04 e8 03 00 00 04 e8 03 00 00.
+    01 04 f5 01 00 00 04 14 00 00 00.
 
   There is no file comment.
 
 Central directory entry #17:
 ---------------------------
 
-  torchaudio/sox_effects/
+  torchaudio/datasets/cmudict.py
 
-  offset of local header from start of archive:   31898
-                                                  (0000000000007C9Ah) bytes
+  offset of local header from start of archive:   15340
+                                                  (0000000000003BECh) bytes
   file system or operating system of origin:      Unix
   version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
-  minimum software version required to extract:   1.0
-  compression method:                             none (stored)
+  minimum software version required to extract:   2.0
+  compression method:                             deflated
+  compression sub-type (deflation):               maximum
   file security status:                           not encrypted
   extended local header:                          no
-  file last modified on (DOS date/time):          2023 Mar 15 10:54:56
-  file last modified on (UT extra field modtime): 2023 Mar 15 17:54:56 local
-  file last modified on (UT extra field modtime): 2023 Mar 15 17:54:56 UTC
-  32-bit CRC value (hex):                         00000000
-  compressed size:                                0 bytes
-  uncompressed size:                              0 bytes
-  length of filename:                             23 characters
+  file last modified on (DOS date/time):          2023 May 4 22:38:58
+  file last modified on (UT extra field modtime): 2023 May 5 02:38:58 local
+  file last modified on (UT extra field modtime): 2023 May 5 02:38:58 UTC
+  32-bit CRC value (hex):                         c75d27fa
+  compressed size:                                2034 bytes
+  uncompressed size:                              6408 bytes
+  length of filename:                             30 characters
   length of extra field:                          24 bytes
   length of file comment:                         0 characters
   disk number on which file begins:               disk 1
-  apparent file type:                             binary
-  Unix file attributes (040755 octal):            drwxr-xr-x
-  MS-DOS file attributes (10 hex):                dir 
+  apparent file type:                             text
+  Unix file attributes (100666 octal):            -rw-rw-rw-
+  MS-DOS file attributes (00 hex):                none
 
   The central-directory extra field contains:
   - A subfield with ID 0x5455 (universal time) and 5 data bytes.
     The local extra field has UTC/GMT modification/access times.
   - A subfield with ID 0x7875 (Unix UID/GID (any size)) and 11 data bytes:
-    01 04 e8 03 00 00 04 e8 03 00 00.
+    01 04 f5 01 00 00 04 14 00 00 00.
 
   There is no file comment.
 
 Central directory entry #18:
 ---------------------------
 
-  torchaudio/sox_effects/sox_effects.py
+  torchaudio/datasets/gtzan.py
 
-  offset of local header from start of archive:   31979
-                                                  (0000000000007CEBh) bytes
+  offset of local header from start of archive:   17462
+                                                  (0000000000004436h) bytes
   file system or operating system of origin:      Unix
   version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               maximum
   file security status:                           not encrypted
   extended local header:                          no
-  file last modified on (DOS date/time):          2023 Mar 15 17:25:54
-  file last modified on (UT extra field modtime): 2023 Mar 16 00:25:54 local
-  file last modified on (UT extra field modtime): 2023 Mar 16 00:25:54 UTC
-  32-bit CRC value (hex):                         c45f60d0
-  compressed size:                                3569 bytes
-  uncompressed size:                              12461 bytes
-  length of filename:                             37 characters
+  file last modified on (DOS date/time):          2023 May 4 22:38:58
+  file last modified on (UT extra field modtime): 2023 May 5 02:38:58 local
+  file last modified on (UT extra field modtime): 2023 May 5 02:38:58 UTC
+  32-bit CRC value (hex):                         ac3f3605
+  compressed size:                                5046 bytes
+  uncompressed size:                              25464 bytes
+  length of filename:                             28 characters
   length of extra field:                          24 bytes
   length of file comment:                         0 characters
   disk number on which file begins:               disk 1
   apparent file type:                             text
   Unix file attributes (100666 octal):            -rw-rw-rw-
   MS-DOS file attributes (00 hex):                none
 
   The central-directory extra field contains:
   - A subfield with ID 0x5455 (universal time) and 5 data bytes.
     The local extra field has UTC/GMT modification/access times.
   - A subfield with ID 0x7875 (Unix UID/GID (any size)) and 11 data bytes:
-    01 04 e8 03 00 00 04 e8 03 00 00.
+    01 04 f5 01 00 00 04 14 00 00 00.
 
   There is no file comment.
 
 Central directory entry #19:
 ---------------------------
 
-  torchaudio/sox_effects/__init__.py
+  torchaudio/datasets/cmuarctic.py
 
-  offset of local header from start of archive:   35643
-                                                  (0000000000008B3Bh) bytes
+  offset of local header from start of archive:   22594
+                                                  (0000000000005842h) bytes
   file system or operating system of origin:      Unix
   version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               maximum
   file security status:                           not encrypted
   extended local header:                          no
-  file last modified on (DOS date/time):          2023 Mar 15 17:25:54
-  file last modified on (UT extra field modtime): 2023 Mar 16 00:25:54 local
-  file last modified on (UT extra field modtime): 2023 Mar 16 00:25:54 UTC
-  32-bit CRC value (hex):                         d35c336b
-  compressed size:                                122 bytes
-  uncompressed size:                              272 bytes
-  length of filename:                             34 characters
+  file last modified on (DOS date/time):          2023 May 4 22:38:58
+  file last modified on (UT extra field modtime): 2023 May 5 02:38:58 local
+  file last modified on (UT extra field modtime): 2023 May 5 02:38:58 UTC
+  32-bit CRC value (hex):                         51c3f4cd
+  compressed size:                                2561 bytes
+  uncompressed size:                              7243 bytes
+  length of filename:                             32 characters
   length of extra field:                          24 bytes
   length of file comment:                         0 characters
   disk number on which file begins:               disk 1
   apparent file type:                             text
   Unix file attributes (100666 octal):            -rw-rw-rw-
   MS-DOS file attributes (00 hex):                none
 
   The central-directory extra field contains:
   - A subfield with ID 0x5455 (universal time) and 5 data bytes.
     The local extra field has UTC/GMT modification/access times.
   - A subfield with ID 0x7875 (Unix UID/GID (any size)) and 11 data bytes:
-    01 04 e8 03 00 00 04 e8 03 00 00.
+    01 04 f5 01 00 00 04 14 00 00 00.
 
   There is no file comment.
 
 Central directory entry #20:
 ---------------------------
 
-  torchaudio/pipelines/
+  torchaudio/datasets/musdb_hq.py
 
-  offset of local header from start of archive:   35857
-                                                  (0000000000008C11h) bytes
+  offset of local header from start of archive:   25245
+                                                  (000000000000629Dh) bytes
   file system or operating system of origin:      Unix
   version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
-  minimum software version required to extract:   1.0
-  compression method:                             none (stored)
+  minimum software version required to extract:   2.0
+  compression method:                             deflated
+  compression sub-type (deflation):               maximum
   file security status:                           not encrypted
   extended local header:                          no
-  file last modified on (DOS date/time):          2023 Mar 15 10:54:56
-  file last modified on (UT extra field modtime): 2023 Mar 15 17:54:56 local
-  file last modified on (UT extra field modtime): 2023 Mar 15 17:54:56 UTC
-  32-bit CRC value (hex):                         00000000
-  compressed size:                                0 bytes
-  uncompressed size:                              0 bytes
-  length of filename:                             21 characters
+  file last modified on (DOS date/time):          2023 May 4 22:38:58
+  file last modified on (UT extra field modtime): 2023 May 5 02:38:58 local
+  file last modified on (UT extra field modtime): 2023 May 5 02:38:58 UTC
+  32-bit CRC value (hex):                         828a85bf
+  compressed size:                                1998 bytes
+  uncompressed size:                              5203 bytes
+  length of filename:                             31 characters
   length of extra field:                          24 bytes
   length of file comment:                         0 characters
   disk number on which file begins:               disk 1
-  apparent file type:                             binary
-  Unix file attributes (040755 octal):            drwxr-xr-x
-  MS-DOS file attributes (10 hex):                dir 
+  apparent file type:                             text
+  Unix file attributes (100666 octal):            -rw-rw-rw-
+  MS-DOS file attributes (00 hex):                none
 
   The central-directory extra field contains:
   - A subfield with ID 0x5455 (universal time) and 5 data bytes.
     The local extra field has UTC/GMT modification/access times.
   - A subfield with ID 0x7875 (Unix UID/GID (any size)) and 11 data bytes:
-    01 04 e8 03 00 00 04 e8 03 00 00.
+    01 04 f5 01 00 00 04 14 00 00 00.
 
   There is no file comment.
 
 Central directory entry #21:
 ---------------------------
 
-  torchaudio/pipelines/_wav2vec2/
+  torchaudio/datasets/snips.py
 
-  offset of local header from start of archive:   35936
-                                                  (0000000000008C60h) bytes
+  offset of local header from start of archive:   27332
+                                                  (0000000000006AC4h) bytes
   file system or operating system of origin:      Unix
   version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
-  minimum software version required to extract:   1.0
-  compression method:                             none (stored)
+  minimum software version required to extract:   2.0
+  compression method:                             deflated
+  compression sub-type (deflation):               maximum
   file security status:                           not encrypted
   extended local header:                          no
-  file last modified on (DOS date/time):          2023 Mar 15 10:54:56
-  file last modified on (UT extra field modtime): 2023 Mar 15 17:54:56 local
-  file last modified on (UT extra field modtime): 2023 Mar 15 17:54:56 UTC
-  32-bit CRC value (hex):                         00000000
-  compressed size:                                0 bytes
-  uncompressed size:                              0 bytes
-  length of filename:                             31 characters
+  file last modified on (DOS date/time):          2023 May 4 22:38:58
+  file last modified on (UT extra field modtime): 2023 May 5 02:38:58 local
+  file last modified on (UT extra field modtime): 2023 May 5 02:38:58 UTC
+  32-bit CRC value (hex):                         48e8a358
+  compressed size:                                1613 bytes
+  uncompressed size:                              5165 bytes
+  length of filename:                             28 characters
   length of extra field:                          24 bytes
   length of file comment:                         0 characters
   disk number on which file begins:               disk 1
-  apparent file type:                             binary
-  Unix file attributes (040755 octal):            drwxr-xr-x
-  MS-DOS file attributes (10 hex):                dir 
+  apparent file type:                             text
+  Unix file attributes (100666 octal):            -rw-rw-rw-
+  MS-DOS file attributes (00 hex):                none
 
   The central-directory extra field contains:
   - A subfield with ID 0x5455 (universal time) and 5 data bytes.
     The local extra field has UTC/GMT modification/access times.
   - A subfield with ID 0x7875 (Unix UID/GID (any size)) and 11 data bytes:
-    01 04 e8 03 00 00 04 e8 03 00 00.
+    01 04 f5 01 00 00 04 14 00 00 00.
 
   There is no file comment.
 
 Central directory entry #22:
 ---------------------------
 
-  torchaudio/pipelines/_wav2vec2/utils.py
+  torchaudio/datasets/commonvoice.py
 
-  offset of local header from start of archive:   36025
-                                                  (0000000000008CB9h) bytes
+  offset of local header from start of archive:   29031
+                                                  (0000000000007167h) bytes
   file system or operating system of origin:      Unix
   version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               maximum
   file security status:                           not encrypted
   extended local header:                          no
-  file last modified on (DOS date/time):          2023 Mar 15 17:25:54
-  file last modified on (UT extra field modtime): 2023 Mar 16 00:25:54 local
-  file last modified on (UT extra field modtime): 2023 Mar 16 00:25:54 UTC
-  32-bit CRC value (hex):                         34ca8d9c
-  compressed size:                                425 bytes
-  uncompressed size:                              3094 bytes
-  length of filename:                             39 characters
+  file last modified on (DOS date/time):          2023 May 4 22:38:58
+  file last modified on (UT extra field modtime): 2023 May 5 02:38:58 local
+  file last modified on (UT extra field modtime): 2023 May 5 02:38:58 UTC
+  32-bit CRC value (hex):                         d1499a8c
+  compressed size:                                1125 bytes
+  uncompressed size:                              2849 bytes
+  length of filename:                             34 characters
   length of extra field:                          24 bytes
   length of file comment:                         0 characters
   disk number on which file begins:               disk 1
   apparent file type:                             text
   Unix file attributes (100666 octal):            -rw-rw-rw-
   MS-DOS file attributes (00 hex):                none
 
   The central-directory extra field contains:
   - A subfield with ID 0x5455 (universal time) and 5 data bytes.
     The local extra field has UTC/GMT modification/access times.
   - A subfield with ID 0x7875 (Unix UID/GID (any size)) and 11 data bytes:
-    01 04 e8 03 00 00 04 e8 03 00 00.
+    01 04 f5 01 00 00 04 14 00 00 00.
 
   There is no file comment.
 
 Central directory entry #23:
 ---------------------------
 
-  torchaudio/pipelines/_wav2vec2/impl.py
+  torchaudio/datasets/__init__.py
 
-  offset of local header from start of archive:   36547
-                                                  (0000000000008EC3h) bytes
+  offset of local header from start of archive:   30248
+                                                  (0000000000007628h) bytes
   file system or operating system of origin:      Unix
   version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               maximum
   file security status:                           not encrypted
   extended local header:                          no
-  file last modified on (DOS date/time):          2023 Mar 15 17:25:54
-  file last modified on (UT extra field modtime): 2023 Mar 16 00:25:54 local
-  file last modified on (UT extra field modtime): 2023 Mar 16 00:25:54 UTC
-  32-bit CRC value (hex):                         0826e2eb
-  compressed size:                                5200 bytes
-  uncompressed size:                              61893 bytes
-  length of filename:                             38 characters
+  file last modified on (DOS date/time):          2023 May 4 22:38:58
+  file last modified on (UT extra field modtime): 2023 May 5 02:38:58 local
+  file last modified on (UT extra field modtime): 2023 May 5 02:38:58 UTC
+  32-bit CRC value (hex):                         55e7bc28
+  compressed size:                                434 bytes
+  uncompressed size:                              1138 bytes
+  length of filename:                             31 characters
   length of extra field:                          24 bytes
   length of file comment:                         0 characters
   disk number on which file begins:               disk 1
   apparent file type:                             text
   Unix file attributes (100666 octal):            -rw-rw-rw-
   MS-DOS file attributes (00 hex):                none
 
   The central-directory extra field contains:
   - A subfield with ID 0x5455 (universal time) and 5 data bytes.
     The local extra field has UTC/GMT modification/access times.
   - A subfield with ID 0x7875 (Unix UID/GID (any size)) and 11 data bytes:
-    01 04 e8 03 00 00 04 e8 03 00 00.
+    01 04 f5 01 00 00 04 14 00 00 00.
 
   There is no file comment.
 
 Central directory entry #24:
 ---------------------------
 
-  torchaudio/pipelines/_wav2vec2/__init__.py
+  torchaudio/datasets/libritts.py
 
-  offset of local header from start of archive:   41843
-                                                  (000000000000A373h) bytes
+  offset of local header from start of archive:   30771
+                                                  (0000000000007833h) bytes
   file system or operating system of origin:      Unix
   version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
-  minimum software version required to extract:   1.0
-  compression method:                             none (stored)
+  minimum software version required to extract:   2.0
+  compression method:                             deflated
+  compression sub-type (deflation):               maximum
   file security status:                           not encrypted
   extended local header:                          no
-  file last modified on (DOS date/time):          2023 Mar 15 17:25:54
-  file last modified on (UT extra field modtime): 2023 Mar 16 00:25:54 local
-  file last modified on (UT extra field modtime): 2023 Mar 16 00:25:54 UTC
-  32-bit CRC value (hex):                         00000000
-  compressed size:                                0 bytes
-  uncompressed size:                              0 bytes
-  length of filename:                             42 characters
+  file last modified on (DOS date/time):          2023 May 4 22:38:58
+  file last modified on (UT extra field modtime): 2023 May 5 02:38:58 local
+  file last modified on (UT extra field modtime): 2023 May 5 02:38:58 UTC
+  32-bit CRC value (hex):                         d4164a08
+  compressed size:                                1991 bytes
+  uncompressed size:                              6027 bytes
+  length of filename:                             31 characters
   length of extra field:                          24 bytes
   length of file comment:                         0 characters
   disk number on which file begins:               disk 1
-  apparent file type:                             binary
+  apparent file type:                             text
   Unix file attributes (100666 octal):            -rw-rw-rw-
   MS-DOS file attributes (00 hex):                none
 
   The central-directory extra field contains:
   - A subfield with ID 0x5455 (universal time) and 5 data bytes.
     The local extra field has UTC/GMT modification/access times.
   - A subfield with ID 0x7875 (Unix UID/GID (any size)) and 11 data bytes:
-    01 04 e8 03 00 00 04 e8 03 00 00.
+    01 04 f5 01 00 00 04 14 00 00 00.
 
   There is no file comment.
 
 Central directory entry #25:
 ---------------------------
 
-  torchaudio/pipelines/_tts/
+  torchaudio/datasets/voxceleb1.py
 
-  offset of local header from start of archive:   41943
-                                                  (000000000000A3D7h) bytes
+  offset of local header from start of archive:   32851
+                                                  (0000000000008053h) bytes
   file system or operating system of origin:      Unix
   version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
-  minimum software version required to extract:   1.0
-  compression method:                             none (stored)
+  minimum software version required to extract:   2.0
+  compression method:                             deflated
+  compression sub-type (deflation):               maximum
   file security status:                           not encrypted
   extended local header:                          no
-  file last modified on (DOS date/time):          2023 Mar 15 10:54:56
-  file last modified on (UT extra field modtime): 2023 Mar 15 17:54:56 local
-  file last modified on (UT extra field modtime): 2023 Mar 15 17:54:56 UTC
-  32-bit CRC value (hex):                         00000000
-  compressed size:                                0 bytes
-  uncompressed size:                              0 bytes
-  length of filename:                             26 characters
+  file last modified on (DOS date/time):          2023 May 4 22:38:58
+  file last modified on (UT extra field modtime): 2023 May 5 02:38:58 local
+  file last modified on (UT extra field modtime): 2023 May 5 02:38:58 UTC
+  32-bit CRC value (hex):                         5232284b
+  compressed size:                                2932 bytes
+  uncompressed size:                              12023 bytes
+  length of filename:                             32 characters
   length of extra field:                          24 bytes
   length of file comment:                         0 characters
   disk number on which file begins:               disk 1
-  apparent file type:                             binary
-  Unix file attributes (040755 octal):            drwxr-xr-x
-  MS-DOS file attributes (10 hex):                dir 
+  apparent file type:                             text
+  Unix file attributes (100666 octal):            -rw-rw-rw-
+  MS-DOS file attributes (00 hex):                none
 
   The central-directory extra field contains:
   - A subfield with ID 0x5455 (universal time) and 5 data bytes.
     The local extra field has UTC/GMT modification/access times.
   - A subfield with ID 0x7875 (Unix UID/GID (any size)) and 11 data bytes:
-    01 04 e8 03 00 00 04 e8 03 00 00.
+    01 04 f5 01 00 00 04 14 00 00 00.
 
   There is no file comment.
 
 Central directory entry #26:
 ---------------------------
 
-  torchaudio/pipelines/_tts/utils.py
+  torchaudio/datasets/tedlium.py
 
-  offset of local header from start of archive:   42027
-                                                  (000000000000A42Bh) bytes
+  offset of local header from start of archive:   35873
+                                                  (0000000000008C21h) bytes
   file system or operating system of origin:      Unix
   version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               maximum
   file security status:                           not encrypted
   extended local header:                          no
-  file last modified on (DOS date/time):          2023 Mar 15 17:25:54
-  file last modified on (UT extra field modtime): 2023 Mar 16 00:25:54 local
-  file last modified on (UT extra field modtime): 2023 Mar 16 00:25:54 UTC
-  32-bit CRC value (hex):                         f2d6b380
-  compressed size:                                1431 bytes
-  uncompressed size:                              4844 bytes
-  length of filename:                             34 characters
+  file last modified on (DOS date/time):          2023 May 4 22:38:58
+  file last modified on (UT extra field modtime): 2023 May 5 02:38:58 local
+  file last modified on (UT extra field modtime): 2023 May 5 02:38:58 UTC
+  32-bit CRC value (hex):                         88c4225a
+  compressed size:                                2660 bytes
+  uncompressed size:                              8905 bytes
+  length of filename:                             30 characters
   length of extra field:                          24 bytes
   length of file comment:                         0 characters
   disk number on which file begins:               disk 1
   apparent file type:                             text
   Unix file attributes (100666 octal):            -rw-rw-rw-
   MS-DOS file attributes (00 hex):                none
 
   The central-directory extra field contains:
   - A subfield with ID 0x5455 (universal time) and 5 data bytes.
     The local extra field has UTC/GMT modification/access times.
   - A subfield with ID 0x7875 (Unix UID/GID (any size)) and 11 data bytes:
-    01 04 e8 03 00 00 04 e8 03 00 00.
+    01 04 f5 01 00 00 04 14 00 00 00.
 
   There is no file comment.
 
 Central directory entry #27:
 ---------------------------
 
-  torchaudio/pipelines/_tts/interface.py
+  torchaudio/datasets/utils.py
 
-  offset of local header from start of archive:   43550
-                                                  (000000000000AA1Eh) bytes
+  offset of local header from start of archive:   38621
+                                                  (00000000000096DDh) bytes
   file system or operating system of origin:      Unix
   version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               maximum
   file security status:                           not encrypted
   extended local header:                          no
-  file last modified on (DOS date/time):          2023 Mar 15 17:25:54
-  file last modified on (UT extra field modtime): 2023 Mar 16 00:25:54 local
-  file last modified on (UT extra field modtime): 2023 Mar 16 00:25:54 UTC
-  32-bit CRC value (hex):                         69a2c421
-  compressed size:                                2497 bytes
-  uncompressed size:                              10479 bytes
-  length of filename:                             38 characters
+  file last modified on (DOS date/time):          2023 May 4 22:38:58
+  file last modified on (UT extra field modtime): 2023 May 5 02:38:58 local
+  file last modified on (UT extra field modtime): 2023 May 5 02:38:58 UTC
+  32-bit CRC value (hex):                         e0a6acad
+  compressed size:                                561 bytes
+  uncompressed size:                              1840 bytes
+  length of filename:                             28 characters
   length of extra field:                          24 bytes
   length of file comment:                         0 characters
   disk number on which file begins:               disk 1
   apparent file type:                             text
   Unix file attributes (100666 octal):            -rw-rw-rw-
   MS-DOS file attributes (00 hex):                none
 
   The central-directory extra field contains:
   - A subfield with ID 0x5455 (universal time) and 5 data bytes.
     The local extra field has UTC/GMT modification/access times.
   - A subfield with ID 0x7875 (Unix UID/GID (any size)) and 11 data bytes:
-    01 04 e8 03 00 00 04 e8 03 00 00.
+    01 04 f5 01 00 00 04 14 00 00 00.
 
   There is no file comment.
 
 Central directory entry #28:
 ---------------------------
 
-  torchaudio/pipelines/_tts/impl.py
+  torchaudio/datasets/ljspeech.py
 
-  offset of local header from start of archive:   46143
-                                                  (000000000000B43Fh) bytes
+  offset of local header from start of archive:   39268
+                                                  (0000000000009964h) bytes
   file system or operating system of origin:      Unix
   version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               maximum
   file security status:                           not encrypted
   extended local header:                          no
-  file last modified on (DOS date/time):          2023 Mar 15 17:25:54
-  file last modified on (UT extra field modtime): 2023 Mar 16 00:25:54 local
-  file last modified on (UT extra field modtime): 2023 Mar 16 00:25:54 UTC
-  32-bit CRC value (hex):                         279c4005
-  compressed size:                                2777 bytes
-  uncompressed size:                              15759 bytes
-  length of filename:                             33 characters
+  file last modified on (DOS date/time):          2023 May 4 22:38:58
+  file last modified on (UT extra field modtime): 2023 May 5 02:38:58 local
+  file last modified on (UT extra field modtime): 2023 May 5 02:38:58 UTC
+  32-bit CRC value (hex):                         ff041fd2
+  compressed size:                                1279 bytes
+  uncompressed size:                              3590 bytes
+  length of filename:                             31 characters
   length of extra field:                          24 bytes
   length of file comment:                         0 characters
   disk number on which file begins:               disk 1
   apparent file type:                             text
   Unix file attributes (100666 octal):            -rw-rw-rw-
   MS-DOS file attributes (00 hex):                none
 
   The central-directory extra field contains:
   - A subfield with ID 0x5455 (universal time) and 5 data bytes.
     The local extra field has UTC/GMT modification/access times.
   - A subfield with ID 0x7875 (Unix UID/GID (any size)) and 11 data bytes:
-    01 04 e8 03 00 00 04 e8 03 00 00.
+    01 04 f5 01 00 00 04 14 00 00 00.
 
   There is no file comment.
 
 Central directory entry #29:
 ---------------------------
 
-  torchaudio/pipelines/_tts/__init__.py
+  torchaudio/datasets/yesno.py
 
-  offset of local header from start of archive:   49011
-                                                  (000000000000BF73h) bytes
+  offset of local header from start of archive:   40636
+                                                  (0000000000009EBCh) bytes
   file system or operating system of origin:      Unix
   version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               maximum
   file security status:                           not encrypted
   extended local header:                          no
-  file last modified on (DOS date/time):          2023 Mar 15 17:25:54
-  file last modified on (UT extra field modtime): 2023 Mar 16 00:25:54 local
-  file last modified on (UT extra field modtime): 2023 Mar 16 00:25:54 UTC
-  32-bit CRC value (hex):                         b3a424bb
-  compressed size:                                159 bytes
-  uncompressed size:                              442 bytes
-  length of filename:                             37 characters
+  file last modified on (DOS date/time):          2023 May 4 22:38:58
+  file last modified on (UT extra field modtime): 2023 May 5 02:38:58 local
+  file last modified on (UT extra field modtime): 2023 May 5 02:38:58 UTC
+  32-bit CRC value (hex):                         f2316e0c
+  compressed size:                                1144 bytes
+  uncompressed size:                              3104 bytes
+  length of filename:                             28 characters
   length of extra field:                          24 bytes
   length of file comment:                         0 characters
   disk number on which file begins:               disk 1
   apparent file type:                             text
   Unix file attributes (100666 octal):            -rw-rw-rw-
   MS-DOS file attributes (00 hex):                none
 
   The central-directory extra field contains:
   - A subfield with ID 0x5455 (universal time) and 5 data bytes.
     The local extra field has UTC/GMT modification/access times.
   - A subfield with ID 0x7875 (Unix UID/GID (any size)) and 11 data bytes:
-    01 04 e8 03 00 00 04 e8 03 00 00.
+    01 04 f5 01 00 00 04 14 00 00 00.
 
   There is no file comment.
 
 Central directory entry #30:
 ---------------------------
 
-  torchaudio/pipelines/rnnt_pipeline.py
+  torchaudio/datasets/fluentcommands.py
 
-  offset of local header from start of archive:   49265
-                                                  (000000000000C071h) bytes
+  offset of local header from start of archive:   41866
+                                                  (000000000000A38Ah) bytes
   file system or operating system of origin:      Unix
   version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               maximum
   file security status:                           not encrypted
   extended local header:                          no
-  file last modified on (DOS date/time):          2023 Mar 15 17:25:54
-  file last modified on (UT extra field modtime): 2023 Mar 16 00:25:54 local
-  file last modified on (UT extra field modtime): 2023 Mar 16 00:25:54 UTC
-  32-bit CRC value (hex):                         7cc5b40f
-  compressed size:                                3683 bytes
-  uncompressed size:                              14129 bytes
+  file last modified on (DOS date/time):          2023 May 4 22:38:58
+  file last modified on (UT extra field modtime): 2023 May 5 02:38:58 local
+  file last modified on (UT extra field modtime): 2023 May 5 02:38:58 UTC
+  32-bit CRC value (hex):                         6c457126
+  compressed size:                                1052 bytes
+  uncompressed size:                              3353 bytes
   length of filename:                             37 characters
   length of extra field:                          24 bytes
   length of file comment:                         0 characters
   disk number on which file begins:               disk 1
   apparent file type:                             text
   Unix file attributes (100666 octal):            -rw-rw-rw-
   MS-DOS file attributes (00 hex):                none
 
   The central-directory extra field contains:
   - A subfield with ID 0x5455 (universal time) and 5 data bytes.
     The local extra field has UTC/GMT modification/access times.
   - A subfield with ID 0x7875 (Unix UID/GID (any size)) and 11 data bytes:
-    01 04 e8 03 00 00 04 e8 03 00 00.
+    01 04 f5 01 00 00 04 14 00 00 00.
 
   There is no file comment.
 
 Central directory entry #31:
 ---------------------------
 
-  torchaudio/pipelines/_source_separation_pipeline.py
+  torchaudio/datasets/librispeech.py
 
-  offset of local header from start of archive:   53043
-                                                  (000000000000CF33h) bytes
+  offset of local header from start of archive:   43013
+                                                  (000000000000A805h) bytes
   file system or operating system of origin:      Unix
   version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               maximum
   file security status:                           not encrypted
   extended local header:                          no
-  file last modified on (DOS date/time):          2023 Mar 15 17:25:54
-  file last modified on (UT extra field modtime): 2023 Mar 16 00:25:54 local
-  file last modified on (UT extra field modtime): 2023 Mar 16 00:25:54 UTC
-  32-bit CRC value (hex):                         19208918
-  compressed size:                                1432 bytes
-  uncompressed size:                              4333 bytes
-  length of filename:                             51 characters
+  file last modified on (DOS date/time):          2023 May 4 22:38:58
+  file last modified on (UT extra field modtime): 2023 May 5 02:38:58 local
+  file last modified on (UT extra field modtime): 2023 May 5 02:38:58 UTC
+  32-bit CRC value (hex):                         0302596a
+  compressed size:                                2146 bytes
+  uncompressed size:                              6474 bytes
+  length of filename:                             34 characters
   length of extra field:                          24 bytes
   length of file comment:                         0 characters
   disk number on which file begins:               disk 1
   apparent file type:                             text
   Unix file attributes (100666 octal):            -rw-rw-rw-
   MS-DOS file attributes (00 hex):                none
 
   The central-directory extra field contains:
   - A subfield with ID 0x5455 (universal time) and 5 data bytes.
     The local extra field has UTC/GMT modification/access times.
   - A subfield with ID 0x7875 (Unix UID/GID (any size)) and 11 data bytes:
-    01 04 e8 03 00 00 04 e8 03 00 00.
+    01 04 f5 01 00 00 04 14 00 00 00.
 
   There is no file comment.
 
 Central directory entry #32:
 ---------------------------
 
-  torchaudio/pipelines/__init__.py
+  torchaudio/datasets/iemocap.py
 
-  offset of local header from start of archive:   54584
-                                                  (000000000000D538h) bytes
+  offset of local header from start of archive:   45251
+                                                  (000000000000B0C3h) bytes
   file system or operating system of origin:      Unix
   version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               maximum
   file security status:                           not encrypted
   extended local header:                          no
-  file last modified on (DOS date/time):          2023 Mar 15 17:25:54
-  file last modified on (UT extra field modtime): 2023 Mar 16 00:25:54 local
-  file last modified on (UT extra field modtime): 2023 Mar 16 00:25:54 UTC
-  32-bit CRC value (hex):                         32d3fccb
-  compressed size:                                557 bytes
-  uncompressed size:                              2554 bytes
-  length of filename:                             32 characters
+  file last modified on (DOS date/time):          2023 May 4 22:38:58
+  file last modified on (UT extra field modtime): 2023 May 5 02:38:58 local
+  file last modified on (UT extra field modtime): 2023 May 5 02:38:58 UTC
+  32-bit CRC value (hex):                         b9d296ed
+  compressed size:                                1523 bytes
+  uncompressed size:                              5077 bytes
+  length of filename:                             30 characters
   length of extra field:                          24 bytes
   length of file comment:                         0 characters
   disk number on which file begins:               disk 1
   apparent file type:                             text
   Unix file attributes (100666 octal):            -rw-rw-rw-
   MS-DOS file attributes (00 hex):                none
 
   The central-directory extra field contains:
   - A subfield with ID 0x5455 (universal time) and 5 data bytes.
     The local extra field has UTC/GMT modification/access times.
   - A subfield with ID 0x7875 (Unix UID/GID (any size)) and 11 data bytes:
-    01 04 e8 03 00 00 04 e8 03 00 00.
+    01 04 f5 01 00 00 04 14 00 00 00.
 
   There is no file comment.
 
 Central directory entry #33:
 ---------------------------
 
-  torchaudio/models/
+  torchaudio/datasets/librimix.py
 
-  offset of local header from start of archive:   55231
-                                                  (000000000000D7BFh) bytes
+  offset of local header from start of archive:   46862
+                                                  (000000000000B70Eh) bytes
   file system or operating system of origin:      Unix
   version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
-  minimum software version required to extract:   1.0
-  compression method:                             none (stored)
+  minimum software version required to extract:   2.0
+  compression method:                             deflated
+  compression sub-type (deflation):               maximum
   file security status:                           not encrypted
   extended local header:                          no
-  file last modified on (DOS date/time):          2023 Mar 15 10:54:56
-  file last modified on (UT extra field modtime): 2023 Mar 15 17:54:56 local
-  file last modified on (UT extra field modtime): 2023 Mar 15 17:54:56 UTC
-  32-bit CRC value (hex):                         00000000
-  compressed size:                                0 bytes
-  uncompressed size:                              0 bytes
-  length of filename:                             18 characters
+  file last modified on (DOS date/time):          2023 May 4 22:38:58
+  file last modified on (UT extra field modtime): 2023 May 5 02:38:58 local
+  file last modified on (UT extra field modtime): 2023 May 5 02:38:58 UTC
+  32-bit CRC value (hex):                         de3d07c5
+  compressed size:                                1726 bytes
+  uncompressed size:                              5249 bytes
+  length of filename:                             31 characters
   length of extra field:                          24 bytes
   length of file comment:                         0 characters
   disk number on which file begins:               disk 1
-  apparent file type:                             binary
-  Unix file attributes (040755 octal):            drwxr-xr-x
-  MS-DOS file attributes (10 hex):                dir 
+  apparent file type:                             text
+  Unix file attributes (100666 octal):            -rw-rw-rw-
+  MS-DOS file attributes (00 hex):                none
 
   The central-directory extra field contains:
   - A subfield with ID 0x5455 (universal time) and 5 data bytes.
     The local extra field has UTC/GMT modification/access times.
   - A subfield with ID 0x7875 (Unix UID/GID (any size)) and 11 data bytes:
-    01 04 e8 03 00 00 04 e8 03 00 00.
+    01 04 f5 01 00 00 04 14 00 00 00.
 
   There is no file comment.
 
 Central directory entry #34:
 ---------------------------
 
-  torchaudio/models/wav2vec2/
+  torchaudio/datasets/quesst14.py
 
-  offset of local header from start of archive:   55307
-                                                  (000000000000D80Bh) bytes
+  offset of local header from start of archive:   48677
+                                                  (000000000000BE25h) bytes
   file system or operating system of origin:      Unix
   version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
-  minimum software version required to extract:   1.0
-  compression method:                             none (stored)
+  minimum software version required to extract:   2.0
+  compression method:                             deflated
+  compression sub-type (deflation):               maximum
   file security status:                           not encrypted
   extended local header:                          no
-  file last modified on (DOS date/time):          2023 Mar 15 10:54:56
-  file last modified on (UT extra field modtime): 2023 Mar 15 17:54:56 local
-  file last modified on (UT extra field modtime): 2023 Mar 15 17:54:56 UTC
-  32-bit CRC value (hex):                         00000000
-  compressed size:                                0 bytes
-  uncompressed size:                              0 bytes
-  length of filename:                             27 characters
+  file last modified on (DOS date/time):          2023 May 4 22:38:58
+  file last modified on (UT extra field modtime): 2023 May 5 02:38:58 local
+  file last modified on (UT extra field modtime): 2023 May 5 02:38:58 UTC
+  32-bit CRC value (hex):                         efb792ea
+  compressed size:                                1617 bytes
+  uncompressed size:                              4580 bytes
+  length of filename:                             31 characters
   length of extra field:                          24 bytes
   length of file comment:                         0 characters
   disk number on which file begins:               disk 1
-  apparent file type:                             binary
-  Unix file attributes (040755 octal):            drwxr-xr-x
-  MS-DOS file attributes (10 hex):                dir 
+  apparent file type:                             text
+  Unix file attributes (100666 octal):            -rw-rw-rw-
+  MS-DOS file attributes (00 hex):                none
 
   The central-directory extra field contains:
   - A subfield with ID 0x5455 (universal time) and 5 data bytes.
     The local extra field has UTC/GMT modification/access times.
   - A subfield with ID 0x7875 (Unix UID/GID (any size)) and 11 data bytes:
-    01 04 e8 03 00 00 04 e8 03 00 00.
+    01 04 f5 01 00 00 04 14 00 00 00.
 
   There is no file comment.
 
 Central directory entry #35:
 ---------------------------
 
-  torchaudio/models/wav2vec2/utils/
+  torchaudio/datasets/vctk.py
 
-  offset of local header from start of archive:   55392
-                                                  (000000000000D860h) bytes
+  offset of local header from start of archive:   50383
+                                                  (000000000000C4CFh) bytes
   file system or operating system of origin:      Unix
   version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
-  minimum software version required to extract:   1.0
-  compression method:                             none (stored)
+  minimum software version required to extract:   2.0
+  compression method:                             deflated
+  compression sub-type (deflation):               maximum
   file security status:                           not encrypted
   extended local header:                          no
-  file last modified on (DOS date/time):          2023 Mar 15 10:54:56
-  file last modified on (UT extra field modtime): 2023 Mar 15 17:54:56 local
-  file last modified on (UT extra field modtime): 2023 Mar 15 17:54:56 UTC
-  32-bit CRC value (hex):                         00000000
-  compressed size:                                0 bytes
-  uncompressed size:                              0 bytes
-  length of filename:                             33 characters
+  file last modified on (DOS date/time):          2023 May 4 22:38:58
+  file last modified on (UT extra field modtime): 2023 May 5 02:38:58 local
+  file last modified on (UT extra field modtime): 2023 May 5 02:38:58 UTC
+  32-bit CRC value (hex):                         583d6082
+  compressed size:                                1922 bytes
+  uncompressed size:                              5831 bytes
+  length of filename:                             27 characters
   length of extra field:                          24 bytes
   length of file comment:                         0 characters
   disk number on which file begins:               disk 1
-  apparent file type:                             binary
-  Unix file attributes (040755 octal):            drwxr-xr-x
-  MS-DOS file attributes (10 hex):                dir 
+  apparent file type:                             text
+  Unix file attributes (100666 octal):            -rw-rw-rw-
+  MS-DOS file attributes (00 hex):                none
 
   The central-directory extra field contains:
   - A subfield with ID 0x5455 (universal time) and 5 data bytes.
     The local extra field has UTC/GMT modification/access times.
   - A subfield with ID 0x7875 (Unix UID/GID (any size)) and 11 data bytes:
-    01 04 e8 03 00 00 04 e8 03 00 00.
+    01 04 f5 01 00 00 04 14 00 00 00.
 
   There is no file comment.
 
 Central directory entry #36:
 ---------------------------
 
-  torchaudio/models/wav2vec2/utils/import_huggingface.py
+  torchaudio/io/
 
-  offset of local header from start of archive:   55483
-                                                  (000000000000D8BBh) bytes
+  offset of local header from start of archive:   52390
+                                                  (000000000000CCA6h) bytes
   file system or operating system of origin:      Unix
   version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
-  minimum software version required to extract:   2.0
-  compression method:                             deflated
-  compression sub-type (deflation):               maximum
+  minimum software version required to extract:   1.0
+  compression method:                             none (stored)
   file security status:                           not encrypted
   extended local header:                          no
-  file last modified on (DOS date/time):          2023 Mar 15 17:25:54
-  file last modified on (UT extra field modtime): 2023 Mar 16 00:25:54 local
-  file last modified on (UT extra field modtime): 2023 Mar 16 00:25:54 UTC
-  32-bit CRC value (hex):                         4527440a
-  compressed size:                                1516 bytes
-  uncompressed size:                              6080 bytes
-  length of filename:                             54 characters
+  file last modified on (DOS date/time):          2023 May 6 14:35:50
+  file last modified on (UT extra field modtime): 2023 May 6 18:35:50 local
+  file last modified on (UT extra field modtime): 2023 May 6 18:35:50 UTC
+  32-bit CRC value (hex):                         00000000
+  compressed size:                                0 bytes
+  uncompressed size:                              0 bytes
+  length of filename:                             14 characters
   length of extra field:                          24 bytes
   length of file comment:                         0 characters
   disk number on which file begins:               disk 1
-  apparent file type:                             text
-  Unix file attributes (100666 octal):            -rw-rw-rw-
-  MS-DOS file attributes (00 hex):                none
+  apparent file type:                             binary
+  Unix file attributes (040755 octal):            drwxr-xr-x
+  MS-DOS file attributes (10 hex):                dir 
 
   The central-directory extra field contains:
   - A subfield with ID 0x5455 (universal time) and 5 data bytes.
     The local extra field has UTC/GMT modification/access times.
   - A subfield with ID 0x7875 (Unix UID/GID (any size)) and 11 data bytes:
-    01 04 e8 03 00 00 04 e8 03 00 00.
+    01 04 f5 01 00 00 04 14 00 00 00.
 
   There is no file comment.
 
 Central directory entry #37:
 ---------------------------
 
-  torchaudio/models/wav2vec2/utils/import_fairseq.py
+  torchaudio/io/_playback.py
 
-  offset of local header from start of archive:   57111
-                                                  (000000000000DF17h) bytes
+  offset of local header from start of archive:   52462
+                                                  (000000000000CCEEh) bytes
   file system or operating system of origin:      Unix
   version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               maximum
   file security status:                           not encrypted
   extended local header:                          no
-  file last modified on (DOS date/time):          2023 Mar 15 17:25:54
-  file last modified on (UT extra field modtime): 2023 Mar 16 00:25:54 local
-  file last modified on (UT extra field modtime): 2023 Mar 16 00:25:54 UTC
-  32-bit CRC value (hex):                         35a405ba
-  compressed size:                                2140 bytes
-  uncompressed size:                              9411 bytes
-  length of filename:                             50 characters
+  file last modified on (DOS date/time):          2023 May 4 22:38:58
+  file last modified on (UT extra field modtime): 2023 May 5 02:38:58 local
+  file last modified on (UT extra field modtime): 2023 May 5 02:38:58 UTC
+  32-bit CRC value (hex):                         e257b81e
+  compressed size:                                949 bytes
+  uncompressed size:                              2391 bytes
+  length of filename:                             26 characters
   length of extra field:                          24 bytes
   length of file comment:                         0 characters
   disk number on which file begins:               disk 1
   apparent file type:                             text
   Unix file attributes (100666 octal):            -rw-rw-rw-
   MS-DOS file attributes (00 hex):                none
 
   The central-directory extra field contains:
   - A subfield with ID 0x5455 (universal time) and 5 data bytes.
     The local extra field has UTC/GMT modification/access times.
   - A subfield with ID 0x7875 (Unix UID/GID (any size)) and 11 data bytes:
-    01 04 e8 03 00 00 04 e8 03 00 00.
+    01 04 f5 01 00 00 04 14 00 00 00.
 
   There is no file comment.
 
 Central directory entry #38:
 ---------------------------
 
-  torchaudio/models/wav2vec2/utils/__init__.py
+  torchaudio/io/__init__.py
 
-  offset of local header from start of archive:   59359
-                                                  (000000000000E7DFh) bytes
+  offset of local header from start of archive:   53495
+                                                  (000000000000D0F7h) bytes
   file system or operating system of origin:      Unix
   version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               maximum
   file security status:                           not encrypted
   extended local header:                          no
-  file last modified on (DOS date/time):          2023 Mar 15 17:25:54
-  file last modified on (UT extra field modtime): 2023 Mar 16 00:25:54 local
-  file last modified on (UT extra field modtime): 2023 Mar 16 00:25:54 UTC
-  32-bit CRC value (hex):                         2cd08f42
-  compressed size:                                88 bytes
-  uncompressed size:                              188 bytes
-  length of filename:                             44 characters
+  file last modified on (DOS date/time):          2023 May 4 22:38:58
+  file last modified on (UT extra field modtime): 2023 May 5 02:38:58 local
+  file last modified on (UT extra field modtime): 2023 May 5 02:38:58 UTC
+  32-bit CRC value (hex):                         84d51e8d
+  compressed size:                                105 bytes
+  uncompressed size:                              200 bytes
+  length of filename:                             25 characters
   length of extra field:                          24 bytes
   length of file comment:                         0 characters
   disk number on which file begins:               disk 1
   apparent file type:                             text
   Unix file attributes (100666 octal):            -rw-rw-rw-
   MS-DOS file attributes (00 hex):                none
 
   The central-directory extra field contains:
   - A subfield with ID 0x5455 (universal time) and 5 data bytes.
     The local extra field has UTC/GMT modification/access times.
   - A subfield with ID 0x7875 (Unix UID/GID (any size)) and 11 data bytes:
-    01 04 e8 03 00 00 04 e8 03 00 00.
+    01 04 f5 01 00 00 04 14 00 00 00.
 
   There is no file comment.
 
 Central directory entry #39:
 ---------------------------
 
-  torchaudio/models/wav2vec2/wavlm_attention.py
+  torchaudio/io/_stream_reader.py
 
-  offset of local header from start of archive:   59549
-                                                  (000000000000E89Dh) bytes
+  offset of local header from start of archive:   53683
+                                                  (000000000000D1B3h) bytes
   file system or operating system of origin:      Unix
   version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               maximum
   file security status:                           not encrypted
   extended local header:                          no
-  file last modified on (DOS date/time):          2023 Mar 15 17:25:54
-  file last modified on (UT extra field modtime): 2023 Mar 16 00:25:54 local
-  file last modified on (UT extra field modtime): 2023 Mar 16 00:25:54 UTC
-  32-bit CRC value (hex):                         aa642cd3
-  compressed size:                                3041 bytes
-  uncompressed size:                              9588 bytes
-  length of filename:                             45 characters
+  file last modified on (DOS date/time):          2023 May 4 22:38:58
+  file last modified on (UT extra field modtime): 2023 May 5 02:38:58 local
+  file last modified on (UT extra field modtime): 2023 May 5 02:38:58 UTC
+  32-bit CRC value (hex):                         87f604c6
+  compressed size:                                8033 bytes
+  uncompressed size:                              32378 bytes
+  length of filename:                             31 characters
   length of extra field:                          24 bytes
   length of file comment:                         0 characters
   disk number on which file begins:               disk 1
   apparent file type:                             text
   Unix file attributes (100666 octal):            -rw-rw-rw-
   MS-DOS file attributes (00 hex):                none
 
   The central-directory extra field contains:
   - A subfield with ID 0x5455 (universal time) and 5 data bytes.
     The local extra field has UTC/GMT modification/access times.
   - A subfield with ID 0x7875 (Unix UID/GID (any size)) and 11 data bytes:
-    01 04 e8 03 00 00 04 e8 03 00 00.
+    01 04 f5 01 00 00 04 14 00 00 00.
 
   There is no file comment.
 
 Central directory entry #40:
 ---------------------------
 
-  torchaudio/models/wav2vec2/model.py
+  torchaudio/io/_compat.py
 
-  offset of local header from start of archive:   62693
-                                                  (000000000000F4E5h) bytes
+  offset of local header from start of archive:   61805
+                                                  (000000000000F16Dh) bytes
   file system or operating system of origin:      Unix
   version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               maximum
   file security status:                           not encrypted
   extended local header:                          no
-  file last modified on (DOS date/time):          2023 Mar 15 17:25:54
-  file last modified on (UT extra field modtime): 2023 Mar 16 00:25:54 local
-  file last modified on (UT extra field modtime): 2023 Mar 16 00:25:54 UTC
-  32-bit CRC value (hex):                         9fb3eaa1
-  compressed size:                                6249 bytes
-  uncompressed size:                              61671 bytes
-  length of filename:                             35 characters
+  file last modified on (DOS date/time):          2023 May 4 22:38:58
+  file last modified on (UT extra field modtime): 2023 May 5 02:38:58 local
+  file last modified on (UT extra field modtime): 2023 May 5 02:38:58 UTC
+  32-bit CRC value (hex):                         df42bfc3
+  compressed size:                                2123 bytes
+  uncompressed size:                              8237 bytes
+  length of filename:                             24 characters
   length of extra field:                          24 bytes
   length of file comment:                         0 characters
   disk number on which file begins:               disk 1
   apparent file type:                             text
   Unix file attributes (100666 octal):            -rw-rw-rw-
   MS-DOS file attributes (00 hex):                none
 
   The central-directory extra field contains:
   - A subfield with ID 0x5455 (universal time) and 5 data bytes.
     The local extra field has UTC/GMT modification/access times.
   - A subfield with ID 0x7875 (Unix UID/GID (any size)) and 11 data bytes:
-    01 04 e8 03 00 00 04 e8 03 00 00.
+    01 04 f5 01 00 00 04 14 00 00 00.
 
   There is no file comment.
 
 Central directory entry #41:
 ---------------------------
 
-  torchaudio/models/wav2vec2/components.py
+  torchaudio/io/_stream_writer.py
 
-  offset of local header from start of archive:   69035
-                                                  (0000000000010DABh) bytes
+  offset of local header from start of archive:   64010
+                                                  (000000000000FA0Ah) bytes
   file system or operating system of origin:      Unix
   version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               maximum
   file security status:                           not encrypted
   extended local header:                          no
-  file last modified on (DOS date/time):          2023 Mar 15 17:25:54
-  file last modified on (UT extra field modtime): 2023 Mar 16 00:25:54 local
-  file last modified on (UT extra field modtime): 2023 Mar 16 00:25:54 UTC
-  32-bit CRC value (hex):                         2db18b5f
-  compressed size:                                9598 bytes
-  uncompressed size:                              49074 bytes
-  length of filename:                             40 characters
+  file last modified on (DOS date/time):          2023 May 4 22:38:58
+  file last modified on (UT extra field modtime): 2023 May 5 02:38:58 local
+  file last modified on (UT extra field modtime): 2023 May 5 02:38:58 UTC
+  32-bit CRC value (hex):                         452d40bb
+  compressed size:                                3296 bytes
+  uncompressed size:                              12107 bytes
+  length of filename:                             31 characters
   length of extra field:                          24 bytes
   length of file comment:                         0 characters
   disk number on which file begins:               disk 1
   apparent file type:                             text
   Unix file attributes (100666 octal):            -rw-rw-rw-
   MS-DOS file attributes (00 hex):                none
 
   The central-directory extra field contains:
   - A subfield with ID 0x5455 (universal time) and 5 data bytes.
     The local extra field has UTC/GMT modification/access times.
   - A subfield with ID 0x7875 (Unix UID/GID (any size)) and 11 data bytes:
-    01 04 e8 03 00 00 04 e8 03 00 00.
+    01 04 f5 01 00 00 04 14 00 00 00.
 
   There is no file comment.
 
 Central directory entry #42:
 ---------------------------
 
-  torchaudio/models/wav2vec2/__init__.py
+  torchaudio/__init__.py
 
-  offset of local header from start of archive:   78731
-                                                  (000000000001338Bh) bytes
+  offset of local header from start of archive:   67395
+                                                  (0000000000010743h) bytes
   file system or operating system of origin:      Unix
   version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               maximum
   file security status:                           not encrypted
   extended local header:                          no
-  file last modified on (DOS date/time):          2023 Mar 15 17:25:54
-  file last modified on (UT extra field modtime): 2023 Mar 16 00:25:54 local
-  file last modified on (UT extra field modtime): 2023 Mar 16 00:25:54 UTC
-  32-bit CRC value (hex):                         93bedda6
-  compressed size:                                252 bytes
-  uncompressed size:                              972 bytes
-  length of filename:                             38 characters
+  file last modified on (DOS date/time):          2023 May 4 22:38:58
+  file last modified on (UT extra field modtime): 2023 May 5 02:38:58 local
+  file last modified on (UT extra field modtime): 2023 May 5 02:38:58 UTC
+  32-bit CRC value (hex):                         e7b0eb74
+  compressed size:                                272 bytes
+  uncompressed size:                              672 bytes
+  length of filename:                             22 characters
   length of extra field:                          24 bytes
   length of file comment:                         0 characters
   disk number on which file begins:               disk 1
   apparent file type:                             text
   Unix file attributes (100666 octal):            -rw-rw-rw-
   MS-DOS file attributes (00 hex):                none
 
   The central-directory extra field contains:
   - A subfield with ID 0x5455 (universal time) and 5 data bytes.
     The local extra field has UTC/GMT modification/access times.
   - A subfield with ID 0x7875 (Unix UID/GID (any size)) and 11 data bytes:
-    01 04 e8 03 00 00 04 e8 03 00 00.
+    01 04 f5 01 00 00 04 14 00 00 00.
 
   There is no file comment.
 
 Central directory entry #43:
 ---------------------------
 
-  torchaudio/models/decoder/
+  torchaudio/pipelines/
 
-  offset of local header from start of archive:   79079
-                                                  (00000000000134E7h) bytes
+  offset of local header from start of archive:   67747
+                                                  (00000000000108A3h) bytes
   file system or operating system of origin:      Unix
   version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   1.0
   compression method:                             none (stored)
   file security status:                           not encrypted
   extended local header:                          no
-  file last modified on (DOS date/time):          2023 Mar 15 10:54:56
-  file last modified on (UT extra field modtime): 2023 Mar 15 17:54:56 local
-  file last modified on (UT extra field modtime): 2023 Mar 15 17:54:56 UTC
+  file last modified on (DOS date/time):          2023 May 6 14:35:50
+  file last modified on (UT extra field modtime): 2023 May 6 18:35:50 local
+  file last modified on (UT extra field modtime): 2023 May 6 18:35:50 UTC
   32-bit CRC value (hex):                         00000000
   compressed size:                                0 bytes
   uncompressed size:                              0 bytes
-  length of filename:                             26 characters
+  length of filename:                             21 characters
   length of extra field:                          24 bytes
   length of file comment:                         0 characters
   disk number on which file begins:               disk 1
   apparent file type:                             binary
   Unix file attributes (040755 octal):            drwxr-xr-x
   MS-DOS file attributes (10 hex):                dir 
 
   The central-directory extra field contains:
   - A subfield with ID 0x5455 (universal time) and 5 data bytes.
     The local extra field has UTC/GMT modification/access times.
   - A subfield with ID 0x7875 (Unix UID/GID (any size)) and 11 data bytes:
-    01 04 e8 03 00 00 04 e8 03 00 00.
+    01 04 f5 01 00 00 04 14 00 00 00.
 
   There is no file comment.
 
 Central directory entry #44:
 ---------------------------
 
-  torchaudio/models/decoder/_ctc_decoder.py
+  torchaudio/pipelines/_source_separation_pipeline.py
 
-  offset of local header from start of archive:   79163
-                                                  (000000000001353Bh) bytes
+  offset of local header from start of archive:   67826
+                                                  (00000000000108F2h) bytes
   file system or operating system of origin:      Unix
   version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               maximum
   file security status:                           not encrypted
   extended local header:                          no
-  file last modified on (DOS date/time):          2023 Mar 15 17:25:54
-  file last modified on (UT extra field modtime): 2023 Mar 16 00:25:54 local
-  file last modified on (UT extra field modtime): 2023 Mar 16 00:25:54 UTC
-  32-bit CRC value (hex):                         6ef0adc7
-  compressed size:                                4936 bytes
-  uncompressed size:                              18544 bytes
-  length of filename:                             41 characters
+  file last modified on (DOS date/time):          2023 May 4 22:38:58
+  file last modified on (UT extra field modtime): 2023 May 5 02:38:58 local
+  file last modified on (UT extra field modtime): 2023 May 5 02:38:58 UTC
+  32-bit CRC value (hex):                         19208918
+  compressed size:                                1432 bytes
+  uncompressed size:                              4333 bytes
+  length of filename:                             51 characters
   length of extra field:                          24 bytes
   length of file comment:                         0 characters
   disk number on which file begins:               disk 1
   apparent file type:                             text
   Unix file attributes (100666 octal):            -rw-rw-rw-
   MS-DOS file attributes (00 hex):                none
 
   The central-directory extra field contains:
   - A subfield with ID 0x5455 (universal time) and 5 data bytes.
     The local extra field has UTC/GMT modification/access times.
   - A subfield with ID 0x7875 (Unix UID/GID (any size)) and 11 data bytes:
-    01 04 e8 03 00 00 04 e8 03 00 00.
+    01 04 f5 01 00 00 04 14 00 00 00.
 
   There is no file comment.
 
 Central directory entry #45:
 ---------------------------
 
-  torchaudio/models/decoder/__init__.py
+  torchaudio/pipelines/_wav2vec2/
 
-  offset of local header from start of archive:   84198
-                                                  (00000000000148E6h) bytes
+  offset of local header from start of archive:   69367
+                                                  (0000000000010EF7h) bytes
   file system or operating system of origin:      Unix
   version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
-  minimum software version required to extract:   2.0
-  compression method:                             deflated
-  compression sub-type (deflation):               maximum
+  minimum software version required to extract:   1.0
+  compression method:                             none (stored)
   file security status:                           not encrypted
   extended local header:                          no
-  file last modified on (DOS date/time):          2023 Mar 15 17:25:54
-  file last modified on (UT extra field modtime): 2023 Mar 16 00:25:54 local
-  file last modified on (UT extra field modtime): 2023 Mar 16 00:25:54 UTC
-  32-bit CRC value (hex):                         7b253cb5
-  compressed size:                                392 bytes
-  uncompressed size:                              783 bytes
-  length of filename:                             37 characters
+  file last modified on (DOS date/time):          2023 May 6 14:35:50
+  file last modified on (UT extra field modtime): 2023 May 6 18:35:50 local
+  file last modified on (UT extra field modtime): 2023 May 6 18:35:50 UTC
+  32-bit CRC value (hex):                         00000000
+  compressed size:                                0 bytes
+  uncompressed size:                              0 bytes
+  length of filename:                             31 characters
   length of extra field:                          24 bytes
   length of file comment:                         0 characters
   disk number on which file begins:               disk 1
-  apparent file type:                             text
-  Unix file attributes (100666 octal):            -rw-rw-rw-
-  MS-DOS file attributes (00 hex):                none
+  apparent file type:                             binary
+  Unix file attributes (040755 octal):            drwxr-xr-x
+  MS-DOS file attributes (10 hex):                dir 
 
   The central-directory extra field contains:
   - A subfield with ID 0x5455 (universal time) and 5 data bytes.
     The local extra field has UTC/GMT modification/access times.
   - A subfield with ID 0x7875 (Unix UID/GID (any size)) and 11 data bytes:
-    01 04 e8 03 00 00 04 e8 03 00 00.
+    01 04 f5 01 00 00 04 14 00 00 00.
 
   There is no file comment.
 
 Central directory entry #46:
 ---------------------------
 
-  torchaudio/models/wavernn.py
+  torchaudio/pipelines/_wav2vec2/__init__.py
 
-  offset of local header from start of archive:   84685
-                                                  (0000000000014ACDh) bytes
+  offset of local header from start of archive:   69456
+                                                  (0000000000010F50h) bytes
   file system or operating system of origin:      Unix
   version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
-  minimum software version required to extract:   2.0
-  compression method:                             deflated
-  compression sub-type (deflation):               maximum
+  minimum software version required to extract:   1.0
+  compression method:                             none (stored)
   file security status:                           not encrypted
   extended local header:                          no
-  file last modified on (DOS date/time):          2023 Mar 15 17:25:54
-  file last modified on (UT extra field modtime): 2023 Mar 16 00:25:54 local
-  file last modified on (UT extra field modtime): 2023 Mar 16 00:25:54 UTC
-  32-bit CRC value (hex):                         fe1c66da
-  compressed size:                                3629 bytes
-  uncompressed size:                              15855 bytes
-  length of filename:                             28 characters
+  file last modified on (DOS date/time):          2023 May 4 22:38:58
+  file last modified on (UT extra field modtime): 2023 May 5 02:38:58 local
+  file last modified on (UT extra field modtime): 2023 May 5 02:38:58 UTC
+  32-bit CRC value (hex):                         00000000
+  compressed size:                                0 bytes
+  uncompressed size:                              0 bytes
+  length of filename:                             42 characters
   length of extra field:                          24 bytes
   length of file comment:                         0 characters
   disk number on which file begins:               disk 1
-  apparent file type:                             text
+  apparent file type:                             binary
   Unix file attributes (100666 octal):            -rw-rw-rw-
   MS-DOS file attributes (00 hex):                none
 
   The central-directory extra field contains:
   - A subfield with ID 0x5455 (universal time) and 5 data bytes.
     The local extra field has UTC/GMT modification/access times.
   - A subfield with ID 0x7875 (Unix UID/GID (any size)) and 11 data bytes:
-    01 04 e8 03 00 00 04 e8 03 00 00.
+    01 04 f5 01 00 00 04 14 00 00 00.
 
   There is no file comment.
 
 Central directory entry #47:
 ---------------------------
 
-  torchaudio/models/wav2letter.py
+  torchaudio/pipelines/_wav2vec2/utils.py
 
-  offset of local header from start of archive:   88400
-                                                  (0000000000015950h) bytes
+  offset of local header from start of archive:   69556
+                                                  (0000000000010FB4h) bytes
   file system or operating system of origin:      Unix
   version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               maximum
   file security status:                           not encrypted
   extended local header:                          no
-  file last modified on (DOS date/time):          2023 Mar 15 17:25:54
-  file last modified on (UT extra field modtime): 2023 Mar 16 00:25:54 local
-  file last modified on (UT extra field modtime): 2023 Mar 16 00:25:54 UTC
-  32-bit CRC value (hex):                         c87531aa
-  compressed size:                                873 bytes
-  uncompressed size:                              3350 bytes
-  length of filename:                             31 characters
+  file last modified on (DOS date/time):          2023 May 4 22:38:58
+  file last modified on (UT extra field modtime): 2023 May 5 02:38:58 local
+  file last modified on (UT extra field modtime): 2023 May 5 02:38:58 UTC
+  32-bit CRC value (hex):                         34ca8d9c
+  compressed size:                                425 bytes
+  uncompressed size:                              3094 bytes
+  length of filename:                             39 characters
   length of extra field:                          24 bytes
   length of file comment:                         0 characters
   disk number on which file begins:               disk 1
   apparent file type:                             text
   Unix file attributes (100666 octal):            -rw-rw-rw-
   MS-DOS file attributes (00 hex):                none
 
   The central-directory extra field contains:
   - A subfield with ID 0x5455 (universal time) and 5 data bytes.
     The local extra field has UTC/GMT modification/access times.
   - A subfield with ID 0x7875 (Unix UID/GID (any size)) and 11 data bytes:
-    01 04 e8 03 00 00 04 e8 03 00 00.
+    01 04 f5 01 00 00 04 14 00 00 00.
 
   There is no file comment.
 
 Central directory entry #48:
 ---------------------------
 
-  torchaudio/models/tacotron2.py
+  torchaudio/pipelines/_wav2vec2/impl.py
 
-  offset of local header from start of archive:   89362
-                                                  (0000000000015D12h) bytes
+  offset of local header from start of archive:   70078
+                                                  (00000000000111BEh) bytes
   file system or operating system of origin:      Unix
   version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               maximum
   file security status:                           not encrypted
   extended local header:                          no
-  file last modified on (DOS date/time):          2023 Mar 15 17:25:54
-  file last modified on (UT extra field modtime): 2023 Mar 16 00:25:54 local
-  file last modified on (UT extra field modtime): 2023 Mar 16 00:25:54 UTC
-  32-bit CRC value (hex):                         68ba1081
-  compressed size:                                8119 bytes
-  uncompressed size:                              46960 bytes
-  length of filename:                             30 characters
+  file last modified on (DOS date/time):          2023 May 4 22:38:58
+  file last modified on (UT extra field modtime): 2023 May 5 02:38:58 local
+  file last modified on (UT extra field modtime): 2023 May 5 02:38:58 UTC
+  32-bit CRC value (hex):                         0826e2eb
+  compressed size:                                5200 bytes
+  uncompressed size:                              61893 bytes
+  length of filename:                             38 characters
   length of extra field:                          24 bytes
   length of file comment:                         0 characters
   disk number on which file begins:               disk 1
   apparent file type:                             text
   Unix file attributes (100666 octal):            -rw-rw-rw-
   MS-DOS file attributes (00 hex):                none
 
   The central-directory extra field contains:
   - A subfield with ID 0x5455 (universal time) and 5 data bytes.
     The local extra field has UTC/GMT modification/access times.
   - A subfield with ID 0x7875 (Unix UID/GID (any size)) and 11 data bytes:
-    01 04 e8 03 00 00 04 e8 03 00 00.
+    01 04 f5 01 00 00 04 14 00 00 00.
 
   There is no file comment.
 
 Central directory entry #49:
 ---------------------------
 
-  torchaudio/models/rnnt_decoder.py
+  torchaudio/pipelines/__init__.py
 
-  offset of local header from start of archive:   97569
-                                                  (0000000000017D21h) bytes
+  offset of local header from start of archive:   75374
+                                                  (000000000001266Eh) bytes
   file system or operating system of origin:      Unix
   version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               maximum
   file security status:                           not encrypted
   extended local header:                          no
-  file last modified on (DOS date/time):          2023 Mar 15 17:25:54
-  file last modified on (UT extra field modtime): 2023 Mar 16 00:25:54 local
-  file last modified on (UT extra field modtime): 2023 Mar 16 00:25:54 UTC
-  32-bit CRC value (hex):                         e77e0b91
-  compressed size:                                3091 bytes
-  uncompressed size:                              13311 bytes
-  length of filename:                             33 characters
+  file last modified on (DOS date/time):          2023 May 4 22:38:58
+  file last modified on (UT extra field modtime): 2023 May 5 02:38:58 local
+  file last modified on (UT extra field modtime): 2023 May 5 02:38:58 UTC
+  32-bit CRC value (hex):                         32d3fccb
+  compressed size:                                557 bytes
+  uncompressed size:                              2554 bytes
+  length of filename:                             32 characters
   length of extra field:                          24 bytes
   length of file comment:                         0 characters
   disk number on which file begins:               disk 1
   apparent file type:                             text
   Unix file attributes (100666 octal):            -rw-rw-rw-
   MS-DOS file attributes (00 hex):                none
 
   The central-directory extra field contains:
   - A subfield with ID 0x5455 (universal time) and 5 data bytes.
     The local extra field has UTC/GMT modification/access times.
   - A subfield with ID 0x7875 (Unix UID/GID (any size)) and 11 data bytes:
-    01 04 e8 03 00 00 04 e8 03 00 00.
+    01 04 f5 01 00 00 04 14 00 00 00.
 
   There is no file comment.
 
 Central directory entry #50:
 ---------------------------
 
-  torchaudio/models/rnnt.py
+  torchaudio/pipelines/_tts/
 
-  offset of local header from start of archive:   100751
-                                                  (000000000001898Fh) bytes
+  offset of local header from start of archive:   76021
+                                                  (00000000000128F5h) bytes
   file system or operating system of origin:      Unix
   version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
-  minimum software version required to extract:   2.0
-  compression method:                             deflated
-  compression sub-type (deflation):               maximum
+  minimum software version required to extract:   1.0
+  compression method:                             none (stored)
   file security status:                           not encrypted
   extended local header:                          no
-  file last modified on (DOS date/time):          2023 Mar 15 17:25:54
-  file last modified on (UT extra field modtime): 2023 Mar 16 00:25:54 local
-  file last modified on (UT extra field modtime): 2023 Mar 16 00:25:54 UTC
-  32-bit CRC value (hex):                         7bb1c586
-  compressed size:                                4925 bytes
-  uncompressed size:                              36357 bytes
-  length of filename:                             25 characters
+  file last modified on (DOS date/time):          2023 May 6 14:35:50
+  file last modified on (UT extra field modtime): 2023 May 6 18:35:50 local
+  file last modified on (UT extra field modtime): 2023 May 6 18:35:50 UTC
+  32-bit CRC value (hex):                         00000000
+  compressed size:                                0 bytes
+  uncompressed size:                              0 bytes
+  length of filename:                             26 characters
   length of extra field:                          24 bytes
   length of file comment:                         0 characters
   disk number on which file begins:               disk 1
-  apparent file type:                             text
-  Unix file attributes (100666 octal):            -rw-rw-rw-
-  MS-DOS file attributes (00 hex):                none
+  apparent file type:                             binary
+  Unix file attributes (040755 octal):            drwxr-xr-x
+  MS-DOS file attributes (10 hex):                dir 
 
   The central-directory extra field contains:
   - A subfield with ID 0x5455 (universal time) and 5 data bytes.
     The local extra field has UTC/GMT modification/access times.
   - A subfield with ID 0x7875 (Unix UID/GID (any size)) and 11 data bytes:
-    01 04 e8 03 00 00 04 e8 03 00 00.
+    01 04 f5 01 00 00 04 14 00 00 00.
 
   There is no file comment.
 
 Central directory entry #51:
 ---------------------------
 
-  torchaudio/models/emformer.py
+  torchaudio/pipelines/_tts/interface.py
 
-  offset of local header from start of archive:   105759
-                                                  (0000000000019D1Fh) bytes
+  offset of local header from start of archive:   76105
+                                                  (0000000000012949h) bytes
   file system or operating system of origin:      Unix
   version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               maximum
   file security status:                           not encrypted
   extended local header:                          no
-  file last modified on (DOS date/time):          2023 Mar 15 17:25:54
-  file last modified on (UT extra field modtime): 2023 Mar 16 00:25:54 local
-  file last modified on (UT extra field modtime): 2023 Mar 16 00:25:54 UTC
-  32-bit CRC value (hex):                         aaa3a3ef
-  compressed size:                                6242 bytes
-  uncompressed size:                              38650 bytes
-  length of filename:                             29 characters
+  file last modified on (DOS date/time):          2023 May 4 22:38:58
+  file last modified on (UT extra field modtime): 2023 May 5 02:38:58 local
+  file last modified on (UT extra field modtime): 2023 May 5 02:38:58 UTC
+  32-bit CRC value (hex):                         69a2c421
+  compressed size:                                2497 bytes
+  uncompressed size:                              10479 bytes
+  length of filename:                             38 characters
   length of extra field:                          24 bytes
   length of file comment:                         0 characters
   disk number on which file begins:               disk 1
   apparent file type:                             text
   Unix file attributes (100666 octal):            -rw-rw-rw-
   MS-DOS file attributes (00 hex):                none
 
   The central-directory extra field contains:
   - A subfield with ID 0x5455 (universal time) and 5 data bytes.
     The local extra field has UTC/GMT modification/access times.
   - A subfield with ID 0x7875 (Unix UID/GID (any size)) and 11 data bytes:
-    01 04 e8 03 00 00 04 e8 03 00 00.
+    01 04 f5 01 00 00 04 14 00 00 00.
 
   There is no file comment.
 
 Central directory entry #52:
 ---------------------------
 
-  torchaudio/models/deepspeech.py
+  torchaudio/pipelines/_tts/__init__.py
 
-  offset of local header from start of archive:   112088
-                                                  (000000000001B5D8h) bytes
+  offset of local header from start of archive:   78698
+                                                  (000000000001336Ah) bytes
   file system or operating system of origin:      Unix
   version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               maximum
   file security status:                           not encrypted
   extended local header:                          no
-  file last modified on (DOS date/time):          2023 Mar 15 17:25:54
-  file last modified on (UT extra field modtime): 2023 Mar 16 00:25:54 local
-  file last modified on (UT extra field modtime): 2023 Mar 16 00:25:54 UTC
-  32-bit CRC value (hex):                         a1897685
-  compressed size:                                843 bytes
-  uncompressed size:                              2830 bytes
-  length of filename:                             31 characters
+  file last modified on (DOS date/time):          2023 May 4 22:38:58
+  file last modified on (UT extra field modtime): 2023 May 5 02:38:58 local
+  file last modified on (UT extra field modtime): 2023 May 5 02:38:58 UTC
+  32-bit CRC value (hex):                         b3a424bb
+  compressed size:                                159 bytes
+  uncompressed size:                              442 bytes
+  length of filename:                             37 characters
   length of extra field:                          24 bytes
   length of file comment:                         0 characters
   disk number on which file begins:               disk 1
   apparent file type:                             text
   Unix file attributes (100666 octal):            -rw-rw-rw-
   MS-DOS file attributes (00 hex):                none
 
   The central-directory extra field contains:
   - A subfield with ID 0x5455 (universal time) and 5 data bytes.
     The local extra field has UTC/GMT modification/access times.
   - A subfield with ID 0x7875 (Unix UID/GID (any size)) and 11 data bytes:
-    01 04 e8 03 00 00 04 e8 03 00 00.
+    01 04 f5 01 00 00 04 14 00 00 00.
 
   There is no file comment.
 
 Central directory entry #53:
 ---------------------------
 
-  torchaudio/models/conv_tasnet.py
+  torchaudio/pipelines/_tts/utils.py
 
-  offset of local header from start of archive:   113020
-                                                  (000000000001B97Ch) bytes
+  offset of local header from start of archive:   78952
+                                                  (0000000000013468h) bytes
   file system or operating system of origin:      Unix
   version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               maximum
   file security status:                           not encrypted
   extended local header:                          no
-  file last modified on (DOS date/time):          2023 Mar 15 17:25:54
-  file last modified on (UT extra field modtime): 2023 Mar 16 00:25:54 local
-  file last modified on (UT extra field modtime): 2023 Mar 16 00:25:54 UTC
-  32-bit CRC value (hex):                         14911e69
-  compressed size:                                3141 bytes
-  uncompressed size:                              12870 bytes
-  length of filename:                             32 characters
+  file last modified on (DOS date/time):          2023 May 4 22:38:58
+  file last modified on (UT extra field modtime): 2023 May 5 02:38:58 local
+  file last modified on (UT extra field modtime): 2023 May 5 02:38:58 UTC
+  32-bit CRC value (hex):                         f2d6b380
+  compressed size:                                1431 bytes
+  uncompressed size:                              4844 bytes
+  length of filename:                             34 characters
   length of extra field:                          24 bytes
   length of file comment:                         0 characters
   disk number on which file begins:               disk 1
   apparent file type:                             text
   Unix file attributes (100666 octal):            -rw-rw-rw-
   MS-DOS file attributes (00 hex):                none
 
   The central-directory extra field contains:
   - A subfield with ID 0x5455 (universal time) and 5 data bytes.
     The local extra field has UTC/GMT modification/access times.
   - A subfield with ID 0x7875 (Unix UID/GID (any size)) and 11 data bytes:
-    01 04 e8 03 00 00 04 e8 03 00 00.
+    01 04 f5 01 00 00 04 14 00 00 00.
 
   There is no file comment.
 
 Central directory entry #54:
 ---------------------------
 
-  torchaudio/models/conformer.py
+  torchaudio/pipelines/_tts/impl.py
 
-  offset of local header from start of archive:   116251
-                                                  (000000000001C61Bh) bytes
+  offset of local header from start of archive:   80475
+                                                  (0000000000013A5Bh) bytes
   file system or operating system of origin:      Unix
   version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               maximum
   file security status:                           not encrypted
   extended local header:                          no
-  file last modified on (DOS date/time):          2023 Mar 15 17:25:54
-  file last modified on (UT extra field modtime): 2023 Mar 16 00:25:54 local
-  file last modified on (UT extra field modtime): 2023 Mar 16 00:25:54 UTC
-  32-bit CRC value (hex):                         b0959519
-  compressed size:                                2054 bytes
-  uncompressed size:                              10361 bytes
-  length of filename:                             30 characters
+  file last modified on (DOS date/time):          2023 May 4 22:38:58
+  file last modified on (UT extra field modtime): 2023 May 5 02:38:58 local
+  file last modified on (UT extra field modtime): 2023 May 5 02:38:58 UTC
+  32-bit CRC value (hex):                         279c4005
+  compressed size:                                2777 bytes
+  uncompressed size:                              15759 bytes
+  length of filename:                             33 characters
   length of extra field:                          24 bytes
   length of file comment:                         0 characters
   disk number on which file begins:               disk 1
   apparent file type:                             text
   Unix file attributes (100666 octal):            -rw-rw-rw-
   MS-DOS file attributes (00 hex):                none
 
   The central-directory extra field contains:
   - A subfield with ID 0x5455 (universal time) and 5 data bytes.
     The local extra field has UTC/GMT modification/access times.
   - A subfield with ID 0x7875 (Unix UID/GID (any size)) and 11 data bytes:
-    01 04 e8 03 00 00 04 e8 03 00 00.
+    01 04 f5 01 00 00 04 14 00 00 00.
 
   There is no file comment.
 
 Central directory entry #55:
 ---------------------------
 
-  torchaudio/models/_hdemucs.py
+  torchaudio/pipelines/rnnt_pipeline.py
 
-  offset of local header from start of archive:   118393
-                                                  (000000000001CE79h) bytes
+  offset of local header from start of archive:   83343
+                                                  (000000000001458Fh) bytes
   file system or operating system of origin:      Unix
   version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               maximum
   file security status:                           not encrypted
   extended local header:                          no
-  file last modified on (DOS date/time):          2023 Mar 15 17:25:54
-  file last modified on (UT extra field modtime): 2023 Mar 16 00:25:54 local
-  file last modified on (UT extra field modtime): 2023 Mar 16 00:25:54 UTC
-  32-bit CRC value (hex):                         31482b45
-  compressed size:                                9941 bytes
-  uncompressed size:                              39250 bytes
-  length of filename:                             29 characters
+  file last modified on (DOS date/time):          2023 May 4 22:38:58
+  file last modified on (UT extra field modtime): 2023 May 5 02:38:58 local
+  file last modified on (UT extra field modtime): 2023 May 5 02:38:58 UTC
+  32-bit CRC value (hex):                         7cc5b40f
+  compressed size:                                3683 bytes
+  uncompressed size:                              14129 bytes
+  length of filename:                             37 characters
   length of extra field:                          24 bytes
   length of file comment:                         0 characters
   disk number on which file begins:               disk 1
   apparent file type:                             text
   Unix file attributes (100666 octal):            -rw-rw-rw-
   MS-DOS file attributes (00 hex):                none
 
   The central-directory extra field contains:
   - A subfield with ID 0x5455 (universal time) and 5 data bytes.
     The local extra field has UTC/GMT modification/access times.
   - A subfield with ID 0x7875 (Unix UID/GID (any size)) and 11 data bytes:
-    01 04 e8 03 00 00 04 e8 03 00 00.
+    01 04 f5 01 00 00 04 14 00 00 00.
 
   There is no file comment.
 
 Central directory entry #56:
 ---------------------------
 
-  torchaudio/models/__init__.py
+  torchaudio/utils/
 
-  offset of local header from start of archive:   128421
-                                                  (000000000001F5A5h) bytes
+  offset of local header from start of archive:   87121
+                                                  (0000000000015451h) bytes
   file system or operating system of origin:      Unix
   version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
-  minimum software version required to extract:   2.0
-  compression method:                             deflated
-  compression sub-type (deflation):               maximum
+  minimum software version required to extract:   1.0
+  compression method:                             none (stored)
   file security status:                           not encrypted
   extended local header:                          no
-  file last modified on (DOS date/time):          2023 Mar 15 17:25:54
-  file last modified on (UT extra field modtime): 2023 Mar 16 00:25:54 local
-  file last modified on (UT extra field modtime): 2023 Mar 16 00:25:54 UTC
-  32-bit CRC value (hex):                         0032e328
-  compressed size:                                469 bytes
-  uncompressed size:                              1733 bytes
-  length of filename:                             29 characters
+  file last modified on (DOS date/time):          2023 May 6 14:35:50
+  file last modified on (UT extra field modtime): 2023 May 6 18:35:50 local
+  file last modified on (UT extra field modtime): 2023 May 6 18:35:50 UTC
+  32-bit CRC value (hex):                         00000000
+  compressed size:                                0 bytes
+  uncompressed size:                              0 bytes
+  length of filename:                             17 characters
   length of extra field:                          24 bytes
   length of file comment:                         0 characters
   disk number on which file begins:               disk 1
-  apparent file type:                             text
-  Unix file attributes (100666 octal):            -rw-rw-rw-
-  MS-DOS file attributes (00 hex):                none
+  apparent file type:                             binary
+  Unix file attributes (040755 octal):            drwxr-xr-x
+  MS-DOS file attributes (10 hex):                dir 
 
   The central-directory extra field contains:
   - A subfield with ID 0x5455 (universal time) and 5 data bytes.
     The local extra field has UTC/GMT modification/access times.
   - A subfield with ID 0x7875 (Unix UID/GID (any size)) and 11 data bytes:
-    01 04 e8 03 00 00 04 e8 03 00 00.
+    01 04 f5 01 00 00 04 14 00 00 00.
 
   There is no file comment.
 
 Central directory entry #57:
 ---------------------------
 
-  torchaudio/lib/
+  torchaudio/utils/download.py
 
-  offset of local header from start of archive:   128977
-                                                  (000000000001F7D1h) bytes
+  offset of local header from start of archive:   87196
+                                                  (000000000001549Ch) bytes
   file system or operating system of origin:      Unix
   version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
-  minimum software version required to extract:   1.0
-  compression method:                             none (stored)
+  minimum software version required to extract:   2.0
+  compression method:                             deflated
+  compression sub-type (deflation):               maximum
   file security status:                           not encrypted
   extended local header:                          no
-  file last modified on (DOS date/time):          2023 Mar 15 10:54:56
-  file last modified on (UT extra field modtime): 2023 Mar 15 17:54:56 local
-  file last modified on (UT extra field modtime): 2023 Mar 15 17:54:56 UTC
-  32-bit CRC value (hex):                         00000000
-  compressed size:                                0 bytes
-  uncompressed size:                              0 bytes
-  length of filename:                             15 characters
+  file last modified on (DOS date/time):          2023 May 4 22:38:58
+  file last modified on (UT extra field modtime): 2023 May 5 02:38:58 local
+  file last modified on (UT extra field modtime): 2023 May 5 02:38:58 UTC
+  32-bit CRC value (hex):                         14935dc0
+  compressed size:                                1165 bytes
+  uncompressed size:                              2928 bytes
+  length of filename:                             28 characters
   length of extra field:                          24 bytes
   length of file comment:                         0 characters
   disk number on which file begins:               disk 1
-  apparent file type:                             binary
-  Unix file attributes (040755 octal):            drwxr-xr-x
-  MS-DOS file attributes (10 hex):                dir 
+  apparent file type:                             text
+  Unix file attributes (100666 octal):            -rw-rw-rw-
+  MS-DOS file attributes (00 hex):                none
 
   The central-directory extra field contains:
   - A subfield with ID 0x5455 (universal time) and 5 data bytes.
     The local extra field has UTC/GMT modification/access times.
   - A subfield with ID 0x7875 (Unix UID/GID (any size)) and 11 data bytes:
-    01 04 e8 03 00 00 04 e8 03 00 00.
+    01 04 f5 01 00 00 04 14 00 00 00.
 
   There is no file comment.
 
 Central directory entry #58:
 ---------------------------
 
-  torchaudio/lib/libtorchaudio_ffmpeg.pyd
+  torchaudio/utils/__init__.py
 
-  offset of local header from start of archive:   129050
-                                                  (000000000001F81Ah) bytes
+  offset of local header from start of archive:   88447
+                                                  (000000000001597Fh) bytes
   file system or operating system of origin:      Unix
   version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               maximum
   file security status:                           not encrypted
   extended local header:                          no
-  file last modified on (DOS date/time):          2023 Mar 15 17:29:30
-  file last modified on (UT extra field modtime): 2023 Mar 16 00:29:30 local
-  file last modified on (UT extra field modtime): 2023 Mar 16 00:29:30 UTC
-  32-bit CRC value (hex):                         e22b1d82
-  compressed size:                                312613 bytes
-  uncompressed size:                              1394688 bytes
-  length of filename:                             39 characters
+  file last modified on (DOS date/time):          2023 May 4 22:38:58
+  file last modified on (UT extra field modtime): 2023 May 5 02:38:58 local
+  file last modified on (UT extra field modtime): 2023 May 5 02:38:58 UTC
+  32-bit CRC value (hex):                         434b998e
+  compressed size:                                94 bytes
+  uncompressed size:                              159 bytes
+  length of filename:                             28 characters
   length of extra field:                          24 bytes
   length of file comment:                         0 characters
   disk number on which file begins:               disk 1
-  apparent file type:                             binary
+  apparent file type:                             text
   Unix file attributes (100666 octal):            -rw-rw-rw-
   MS-DOS file attributes (00 hex):                none
 
   The central-directory extra field contains:
   - A subfield with ID 0x5455 (universal time) and 5 data bytes.
     The local extra field has UTC/GMT modification/access times.
   - A subfield with ID 0x7875 (Unix UID/GID (any size)) and 11 data bytes:
-    01 04 e8 03 00 00 04 e8 03 00 00.
+    01 04 f5 01 00 00 04 14 00 00 00.
 
   There is no file comment.
 
 Central directory entry #59:
 ---------------------------
 
-  torchaudio/lib/libtorchaudio.pyd
+  torchaudio/utils/ffmpeg_utils.py
 
-  offset of local header from start of archive:   441760
-                                                  (000000000006BDA0h) bytes
+  offset of local header from start of archive:   88627
+                                                  (0000000000015A33h) bytes
   file system or operating system of origin:      Unix
   version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               maximum
   file security status:                           not encrypted
   extended local header:                          no
-  file last modified on (DOS date/time):          2023 Mar 15 17:29:00
-  file last modified on (UT extra field modtime): 2023 Mar 16 00:29:00 local
-  file last modified on (UT extra field modtime): 2023 Mar 16 00:29:00 UTC
-  32-bit CRC value (hex):                         d56f702b
-  compressed size:                                229779 bytes
-  uncompressed size:                              876032 bytes
+  file last modified on (DOS date/time):          2023 May 4 22:38:58
+  file last modified on (UT extra field modtime): 2023 May 5 02:38:58 local
+  file last modified on (UT extra field modtime): 2023 May 5 02:38:58 UTC
+  32-bit CRC value (hex):                         9fcc166e
+  compressed size:                                2120 bytes
+  uncompressed size:                              8947 bytes
   length of filename:                             32 characters
   length of extra field:                          24 bytes
   length of file comment:                         0 characters
   disk number on which file begins:               disk 1
-  apparent file type:                             binary
+  apparent file type:                             text
   Unix file attributes (100666 octal):            -rw-rw-rw-
   MS-DOS file attributes (00 hex):                none
 
   The central-directory extra field contains:
   - A subfield with ID 0x5455 (universal time) and 5 data bytes.
     The local extra field has UTC/GMT modification/access times.
   - A subfield with ID 0x7875 (Unix UID/GID (any size)) and 11 data bytes:
-    01 04 e8 03 00 00 04 e8 03 00 00.
+    01 04 f5 01 00 00 04 14 00 00 00.
 
   There is no file comment.
 
 Central directory entry #60:
 ---------------------------
 
-  torchaudio/lib/libflashlight-text.pyd
+  torchaudio/utils/sox_utils.py
 
-  offset of local header from start of archive:   671629
-                                                  (00000000000A3F8Dh) bytes
+  offset of local header from start of archive:   90837
+                                                  (00000000000162D5h) bytes
   file system or operating system of origin:      Unix
   version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               maximum
   file security status:                           not encrypted
   extended local header:                          no
-  file last modified on (DOS date/time):          2023 Mar 15 17:29:04
-  file last modified on (UT extra field modtime): 2023 Mar 16 00:29:04 local
-  file last modified on (UT extra field modtime): 2023 Mar 16 00:29:04 UTC
-  32-bit CRC value (hex):                         17bfaef6
-  compressed size:                                366151 bytes
-  uncompressed size:                              1710592 bytes
-  length of filename:                             37 characters
+  file last modified on (DOS date/time):          2023 May 4 22:38:58
+  file last modified on (UT extra field modtime): 2023 May 5 02:38:58 local
+  file last modified on (UT extra field modtime): 2023 May 5 02:38:58 UTC
+  32-bit CRC value (hex):                         e066d13d
+  compressed size:                                808 bytes
+  uncompressed size:                              2973 bytes
+  length of filename:                             29 characters
   length of extra field:                          24 bytes
   length of file comment:                         0 characters
   disk number on which file begins:               disk 1
-  apparent file type:                             binary
+  apparent file type:                             text
   Unix file attributes (100666 octal):            -rw-rw-rw-
   MS-DOS file attributes (00 hex):                none
 
   The central-directory extra field contains:
   - A subfield with ID 0x5455 (universal time) and 5 data bytes.
     The local extra field has UTC/GMT modification/access times.
   - A subfield with ID 0x7875 (Unix UID/GID (any size)) and 11 data bytes:
-    01 04 e8 03 00 00 04 e8 03 00 00.
+    01 04 f5 01 00 00 04 14 00 00 00.
 
   There is no file comment.
 
 Central directory entry #61:
 ---------------------------
 
-  torchaudio/lib/flashlight_lib_text_dictionary.pyd
+  torchaudio/backend/
 
-  offset of local header from start of archive:   1037875
-                                                  (00000000000FD633h) bytes
+  offset of local header from start of archive:   91732
+                                                  (0000000000016654h) bytes
   file system or operating system of origin:      Unix
   version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
-  minimum software version required to extract:   2.0
-  compression method:                             deflated
-  compression sub-type (deflation):               maximum
+  minimum software version required to extract:   1.0
+  compression method:                             none (stored)
   file security status:                           not encrypted
   extended local header:                          no
-  file last modified on (DOS date/time):          2023 Mar 15 17:29:08
-  file last modified on (UT extra field modtime): 2023 Mar 16 00:29:08 local
-  file last modified on (UT extra field modtime): 2023 Mar 16 00:29:08 UTC
-  32-bit CRC value (hex):                         d80fccec
-  compressed size:                                189046 bytes
-  uncompressed size:                              1290752 bytes
-  length of filename:                             49 characters
+  file last modified on (DOS date/time):          2023 May 6 14:35:50
+  file last modified on (UT extra field modtime): 2023 May 6 18:35:50 local
+  file last modified on (UT extra field modtime): 2023 May 6 18:35:50 UTC
+  32-bit CRC value (hex):                         00000000
+  compressed size:                                0 bytes
+  uncompressed size:                              0 bytes
+  length of filename:                             19 characters
   length of extra field:                          24 bytes
   length of file comment:                         0 characters
   disk number on which file begins:               disk 1
   apparent file type:                             binary
-  Unix file attributes (100666 octal):            -rw-rw-rw-
-  MS-DOS file attributes (00 hex):                none
+  Unix file attributes (040755 octal):            drwxr-xr-x
+  MS-DOS file attributes (10 hex):                dir 
 
   The central-directory extra field contains:
   - A subfield with ID 0x5455 (universal time) and 5 data bytes.
     The local extra field has UTC/GMT modification/access times.
   - A subfield with ID 0x7875 (Unix UID/GID (any size)) and 11 data bytes:
-    01 04 e8 03 00 00 04 e8 03 00 00.
+    01 04 f5 01 00 00 04 14 00 00 00.
 
   There is no file comment.
 
 Central directory entry #62:
 ---------------------------
 
-  torchaudio/lib/flashlight_lib_text_decoder.pyd
+  torchaudio/backend/__init__.py
 
-  offset of local header from start of archive:   1227028
-                                                  (000000000012B914h) bytes
+  offset of local header from start of archive:   91809
+                                                  (00000000000166A1h) bytes
   file system or operating system of origin:      Unix
   version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               maximum
   file security status:                           not encrypted
   extended local header:                          no
-  file last modified on (DOS date/time):          2023 Mar 15 17:29:12
-  file last modified on (UT extra field modtime): 2023 Mar 16 00:29:12 local
-  file last modified on (UT extra field modtime): 2023 Mar 16 00:29:12 UTC
-  32-bit CRC value (hex):                         33cea5fc
-  compressed size:                                322435 bytes
-  uncompressed size:                              1828352 bytes
-  length of filename:                             46 characters
+  file last modified on (DOS date/time):          2023 May 4 22:38:58
+  file last modified on (UT extra field modtime): 2023 May 5 02:38:58 local
+  file last modified on (UT extra field modtime): 2023 May 5 02:38:58 UTC
+  32-bit CRC value (hex):                         1c6c735d
+  compressed size:                                190 bytes
+  uncompressed size:                              454 bytes
+  length of filename:                             30 characters
   length of extra field:                          24 bytes
   length of file comment:                         0 characters
   disk number on which file begins:               disk 1
-  apparent file type:                             binary
+  apparent file type:                             text
   Unix file attributes (100666 octal):            -rw-rw-rw-
   MS-DOS file attributes (00 hex):                none
 
   The central-directory extra field contains:
   - A subfield with ID 0x5455 (universal time) and 5 data bytes.
     The local extra field has UTC/GMT modification/access times.
   - A subfield with ID 0x7875 (Unix UID/GID (any size)) and 11 data bytes:
-    01 04 e8 03 00 00 04 e8 03 00 00.
+    01 04 f5 01 00 00 04 14 00 00 00.
 
   There is no file comment.
 
 Central directory entry #63:
 ---------------------------
 
-  torchaudio/lib/_torchaudio_ffmpeg.pyd
+  torchaudio/backend/sox_io_backend.py
 
-  offset of local header from start of archive:   1549567
-                                                  (000000000017A4FFh) bytes
+  offset of local header from start of archive:   92087
+                                                  (00000000000167B7h) bytes
   file system or operating system of origin:      Unix
   version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               maximum
   file security status:                           not encrypted
   extended local header:                          no
-  file last modified on (DOS date/time):          2023 Mar 15 17:29:34
-  file last modified on (UT extra field modtime): 2023 Mar 16 00:29:34 local
-  file last modified on (UT extra field modtime): 2023 Mar 16 00:29:34 UTC
-  32-bit CRC value (hex):                         fd13a75f
-  compressed size:                                269323 bytes
-  uncompressed size:                              1503744 bytes
-  length of filename:                             37 characters
+  file last modified on (DOS date/time):          2023 May 4 22:38:58
+  file last modified on (UT extra field modtime): 2023 May 5 02:38:58 local
+  file last modified on (UT extra field modtime): 2023 May 5 02:38:58 UTC
+  32-bit CRC value (hex):                         68ce98ac
+  compressed size:                                4258 bytes
+  uncompressed size:                              17860 bytes
+  length of filename:                             36 characters
   length of extra field:                          24 bytes
   length of file comment:                         0 characters
   disk number on which file begins:               disk 1
-  apparent file type:                             binary
+  apparent file type:                             text
   Unix file attributes (100666 octal):            -rw-rw-rw-
   MS-DOS file attributes (00 hex):                none
 
   The central-directory extra field contains:
   - A subfield with ID 0x5455 (universal time) and 5 data bytes.
     The local extra field has UTC/GMT modification/access times.
   - A subfield with ID 0x7875 (Unix UID/GID (any size)) and 11 data bytes:
-    01 04 e8 03 00 00 04 e8 03 00 00.
+    01 04 f5 01 00 00 04 14 00 00 00.
 
   There is no file comment.
 
 Central directory entry #64:
 ---------------------------
 
-  torchaudio/lib/_torchaudio.pyd
+  torchaudio/backend/common.py
 
-  offset of local header from start of archive:   1818985
-                                                  (00000000001BC169h) bytes
+  offset of local header from start of archive:   96439
+                                                  (00000000000178B7h) bytes
   file system or operating system of origin:      Unix
   version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               maximum
   file security status:                           not encrypted
   extended local header:                          no
-  file last modified on (DOS date/time):          2023 Mar 15 17:29:04
-  file last modified on (UT extra field modtime): 2023 Mar 16 00:29:04 local
-  file last modified on (UT extra field modtime): 2023 Mar 16 00:29:04 UTC
-  32-bit CRC value (hex):                         d712e510
-  compressed size:                                172403 bytes
-  uncompressed size:                              788992 bytes
-  length of filename:                             30 characters
+  file last modified on (DOS date/time):          2023 May 4 22:38:58
+  file last modified on (UT extra field modtime): 2023 May 5 02:38:58 local
+  file last modified on (UT extra field modtime): 2023 May 5 02:38:58 UTC
+  32-bit CRC value (hex):                         5db74cb2
+  compressed size:                                698 bytes
+  uncompressed size:                              1983 bytes
+  length of filename:                             28 characters
   length of extra field:                          24 bytes
   length of file comment:                         0 characters
   disk number on which file begins:               disk 1
-  apparent file type:                             binary
+  apparent file type:                             text
   Unix file attributes (100666 octal):            -rw-rw-rw-
   MS-DOS file attributes (00 hex):                none
 
   The central-directory extra field contains:
   - A subfield with ID 0x5455 (universal time) and 5 data bytes.
     The local extra field has UTC/GMT modification/access times.
   - A subfield with ID 0x7875 (Unix UID/GID (any size)) and 11 data bytes:
-    01 04 e8 03 00 00 04 e8 03 00 00.
+    01 04 f5 01 00 00 04 14 00 00 00.
 
   There is no file comment.
 
 Central directory entry #65:
 ---------------------------
 
-  torchaudio/io/
+  torchaudio/backend/utils.py
 
-  offset of local header from start of archive:   1991476
-                                                  (00000000001E6334h) bytes
+  offset of local header from start of archive:   97223
+                                                  (0000000000017BC7h) bytes
   file system or operating system of origin:      Unix
   version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
-  minimum software version required to extract:   1.0
-  compression method:                             none (stored)
+  minimum software version required to extract:   2.0
+  compression method:                             deflated
+  compression sub-type (deflation):               maximum
   file security status:                           not encrypted
   extended local header:                          no
-  file last modified on (DOS date/time):          2023 Mar 15 10:54:56
-  file last modified on (UT extra field modtime): 2023 Mar 15 17:54:56 local
-  file last modified on (UT extra field modtime): 2023 Mar 15 17:54:56 UTC
-  32-bit CRC value (hex):                         00000000
-  compressed size:                                0 bytes
-  uncompressed size:                              0 bytes
-  length of filename:                             14 characters
+  file last modified on (DOS date/time):          2023 May 4 22:38:58
+  file last modified on (UT extra field modtime): 2023 May 5 02:38:58 local
+  file last modified on (UT extra field modtime): 2023 May 5 02:38:58 UTC
+  32-bit CRC value (hex):                         2a3a0008
+  compressed size:                                949 bytes
+  uncompressed size:                              3000 bytes
+  length of filename:                             27 characters
   length of extra field:                          24 bytes
   length of file comment:                         0 characters
   disk number on which file begins:               disk 1
-  apparent file type:                             binary
-  Unix file attributes (040755 octal):            drwxr-xr-x
-  MS-DOS file attributes (10 hex):                dir 
+  apparent file type:                             text
+  Unix file attributes (100666 octal):            -rw-rw-rw-
+  MS-DOS file attributes (00 hex):                none
 
   The central-directory extra field contains:
   - A subfield with ID 0x5455 (universal time) and 5 data bytes.
     The local extra field has UTC/GMT modification/access times.
   - A subfield with ID 0x7875 (Unix UID/GID (any size)) and 11 data bytes:
-    01 04 e8 03 00 00 04 e8 03 00 00.
+    01 04 f5 01 00 00 04 14 00 00 00.
 
   There is no file comment.
 
 Central directory entry #66:
 ---------------------------
 
-  torchaudio/io/_stream_writer.py
+  torchaudio/backend/no_backend.py
 
-  offset of local header from start of archive:   1991548
-                                                  (00000000001E637Ch) bytes
+  offset of local header from start of archive:   98257
+                                                  (0000000000017FD1h) bytes
   file system or operating system of origin:      Unix
   version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               maximum
   file security status:                           not encrypted
   extended local header:                          no
-  file last modified on (DOS date/time):          2023 Mar 15 17:25:54
-  file last modified on (UT extra field modtime): 2023 Mar 16 00:25:54 local
-  file last modified on (UT extra field modtime): 2023 Mar 16 00:25:54 UTC
-  32-bit CRC value (hex):                         452d40bb
-  compressed size:                                3296 bytes
-  uncompressed size:                              12107 bytes
-  length of filename:                             31 characters
+  file last modified on (DOS date/time):          2023 May 4 22:38:58
+  file last modified on (UT extra field modtime): 2023 May 5 02:38:58 local
+  file last modified on (UT extra field modtime): 2023 May 5 02:38:58 UTC
+  32-bit CRC value (hex):                         a08b056d
+  compressed size:                                314 bytes
+  uncompressed size:                              735 bytes
+  length of filename:                             32 characters
   length of extra field:                          24 bytes
   length of file comment:                         0 characters
   disk number on which file begins:               disk 1
   apparent file type:                             text
   Unix file attributes (100666 octal):            -rw-rw-rw-
   MS-DOS file attributes (00 hex):                none
 
   The central-directory extra field contains:
   - A subfield with ID 0x5455 (universal time) and 5 data bytes.
     The local extra field has UTC/GMT modification/access times.
   - A subfield with ID 0x7875 (Unix UID/GID (any size)) and 11 data bytes:
-    01 04 e8 03 00 00 04 e8 03 00 00.
+    01 04 f5 01 00 00 04 14 00 00 00.
 
   There is no file comment.
 
 Central directory entry #67:
 ---------------------------
 
-  torchaudio/io/_stream_reader.py
+  torchaudio/backend/soundfile_backend.py
 
-  offset of local header from start of archive:   1994933
-                                                  (00000000001E70B5h) bytes
+  offset of local header from start of archive:   98661
+                                                  (0000000000018165h) bytes
   file system or operating system of origin:      Unix
   version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               maximum
   file security status:                           not encrypted
   extended local header:                          no
-  file last modified on (DOS date/time):          2023 Mar 15 17:25:54
-  file last modified on (UT extra field modtime): 2023 Mar 16 00:25:54 local
-  file last modified on (UT extra field modtime): 2023 Mar 16 00:25:54 UTC
-  32-bit CRC value (hex):                         87f604c6
-  compressed size:                                8033 bytes
-  uncompressed size:                              32378 bytes
-  length of filename:                             31 characters
+  file last modified on (DOS date/time):          2023 May 4 22:38:58
+  file last modified on (UT extra field modtime): 2023 May 5 02:38:58 local
+  file last modified on (UT extra field modtime): 2023 May 5 02:38:58 UTC
+  32-bit CRC value (hex):                         122b9e90
+  compressed size:                                4821 bytes
+  uncompressed size:                              17617 bytes
+  length of filename:                             39 characters
   length of extra field:                          24 bytes
   length of file comment:                         0 characters
   disk number on which file begins:               disk 1
   apparent file type:                             text
   Unix file attributes (100666 octal):            -rw-rw-rw-
   MS-DOS file attributes (00 hex):                none
 
   The central-directory extra field contains:
   - A subfield with ID 0x5455 (universal time) and 5 data bytes.
     The local extra field has UTC/GMT modification/access times.
   - A subfield with ID 0x7875 (Unix UID/GID (any size)) and 11 data bytes:
-    01 04 e8 03 00 00 04 e8 03 00 00.
+    01 04 f5 01 00 00 04 14 00 00 00.
 
   There is no file comment.
 
 Central directory entry #68:
 ---------------------------
 
-  torchaudio/io/_playback.py
+  torchaudio/models/
 
-  offset of local header from start of archive:   2003055
-                                                  (00000000001E906Fh) bytes
+  offset of local header from start of archive:   103579
+                                                  (000000000001949Bh) bytes
   file system or operating system of origin:      Unix
   version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
-  minimum software version required to extract:   2.0
-  compression method:                             deflated
-  compression sub-type (deflation):               maximum
+  minimum software version required to extract:   1.0
+  compression method:                             none (stored)
   file security status:                           not encrypted
   extended local header:                          no
-  file last modified on (DOS date/time):          2023 Mar 15 17:25:54
-  file last modified on (UT extra field modtime): 2023 Mar 16 00:25:54 local
-  file last modified on (UT extra field modtime): 2023 Mar 16 00:25:54 UTC
-  32-bit CRC value (hex):                         e257b81e
-  compressed size:                                949 bytes
-  uncompressed size:                              2391 bytes
-  length of filename:                             26 characters
+  file last modified on (DOS date/time):          2023 May 6 14:35:50
+  file last modified on (UT extra field modtime): 2023 May 6 18:35:50 local
+  file last modified on (UT extra field modtime): 2023 May 6 18:35:50 UTC
+  32-bit CRC value (hex):                         00000000
+  compressed size:                                0 bytes
+  uncompressed size:                              0 bytes
+  length of filename:                             18 characters
   length of extra field:                          24 bytes
   length of file comment:                         0 characters
   disk number on which file begins:               disk 1
-  apparent file type:                             text
-  Unix file attributes (100666 octal):            -rw-rw-rw-
-  MS-DOS file attributes (00 hex):                none
+  apparent file type:                             binary
+  Unix file attributes (040755 octal):            drwxr-xr-x
+  MS-DOS file attributes (10 hex):                dir 
 
   The central-directory extra field contains:
   - A subfield with ID 0x5455 (universal time) and 5 data bytes.
     The local extra field has UTC/GMT modification/access times.
   - A subfield with ID 0x7875 (Unix UID/GID (any size)) and 11 data bytes:
-    01 04 e8 03 00 00 04 e8 03 00 00.
+    01 04 f5 01 00 00 04 14 00 00 00.
 
   There is no file comment.
 
 Central directory entry #69:
 ---------------------------
 
-  torchaudio/io/_compat.py
+  torchaudio/models/wav2letter.py
 
-  offset of local header from start of archive:   2004088
-                                                  (00000000001E9478h) bytes
+  offset of local header from start of archive:   103655
+                                                  (00000000000194E7h) bytes
   file system or operating system of origin:      Unix
   version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               maximum
   file security status:                           not encrypted
   extended local header:                          no
-  file last modified on (DOS date/time):          2023 Mar 15 17:25:54
-  file last modified on (UT extra field modtime): 2023 Mar 16 00:25:54 local
-  file last modified on (UT extra field modtime): 2023 Mar 16 00:25:54 UTC
-  32-bit CRC value (hex):                         3b75205e
-  compressed size:                                2105 bytes
-  uncompressed size:                              8176 bytes
-  length of filename:                             24 characters
+  file last modified on (DOS date/time):          2023 May 4 22:38:58
+  file last modified on (UT extra field modtime): 2023 May 5 02:38:58 local
+  file last modified on (UT extra field modtime): 2023 May 5 02:38:58 UTC
+  32-bit CRC value (hex):                         c87531aa
+  compressed size:                                873 bytes
+  uncompressed size:                              3350 bytes
+  length of filename:                             31 characters
   length of extra field:                          24 bytes
   length of file comment:                         0 characters
   disk number on which file begins:               disk 1
   apparent file type:                             text
   Unix file attributes (100666 octal):            -rw-rw-rw-
   MS-DOS file attributes (00 hex):                none
 
   The central-directory extra field contains:
   - A subfield with ID 0x5455 (universal time) and 5 data bytes.
     The local extra field has UTC/GMT modification/access times.
   - A subfield with ID 0x7875 (Unix UID/GID (any size)) and 11 data bytes:
-    01 04 e8 03 00 00 04 e8 03 00 00.
+    01 04 f5 01 00 00 04 14 00 00 00.
 
   There is no file comment.
 
 Central directory entry #70:
 ---------------------------
 
-  torchaudio/io/__init__.py
+  torchaudio/models/emformer.py
 
-  offset of local header from start of archive:   2006275
-                                                  (00000000001E9D03h) bytes
+  offset of local header from start of archive:   104617
+                                                  (00000000000198A9h) bytes
   file system or operating system of origin:      Unix
   version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               maximum
   file security status:                           not encrypted
   extended local header:                          no
-  file last modified on (DOS date/time):          2023 Mar 15 17:25:54
-  file last modified on (UT extra field modtime): 2023 Mar 16 00:25:54 local
-  file last modified on (UT extra field modtime): 2023 Mar 16 00:25:54 UTC
-  32-bit CRC value (hex):                         84d51e8d
-  compressed size:                                105 bytes
-  uncompressed size:                              200 bytes
-  length of filename:                             25 characters
+  file last modified on (DOS date/time):          2023 May 4 22:38:58
+  file last modified on (UT extra field modtime): 2023 May 5 02:38:58 local
+  file last modified on (UT extra field modtime): 2023 May 5 02:38:58 UTC
+  32-bit CRC value (hex):                         aaa3a3ef
+  compressed size:                                6242 bytes
+  uncompressed size:                              38650 bytes
+  length of filename:                             29 characters
   length of extra field:                          24 bytes
   length of file comment:                         0 characters
   disk number on which file begins:               disk 1
   apparent file type:                             text
   Unix file attributes (100666 octal):            -rw-rw-rw-
   MS-DOS file attributes (00 hex):                none
 
   The central-directory extra field contains:
   - A subfield with ID 0x5455 (universal time) and 5 data bytes.
     The local extra field has UTC/GMT modification/access times.
   - A subfield with ID 0x7875 (Unix UID/GID (any size)) and 11 data bytes:
-    01 04 e8 03 00 00 04 e8 03 00 00.
+    01 04 f5 01 00 00 04 14 00 00 00.
 
   There is no file comment.
 
 Central directory entry #71:
 ---------------------------
 
-  torchaudio/functional/
+  torchaudio/models/tacotron2.py
 
-  offset of local header from start of archive:   2006463
-                                                  (00000000001E9DBFh) bytes
+  offset of local header from start of archive:   110946
+                                                  (000000000001B162h) bytes
   file system or operating system of origin:      Unix
   version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
-  minimum software version required to extract:   1.0
-  compression method:                             none (stored)
+  minimum software version required to extract:   2.0
+  compression method:                             deflated
+  compression sub-type (deflation):               maximum
   file security status:                           not encrypted
   extended local header:                          no
-  file last modified on (DOS date/time):          2023 Mar 15 10:54:56
-  file last modified on (UT extra field modtime): 2023 Mar 15 17:54:56 local
-  file last modified on (UT extra field modtime): 2023 Mar 15 17:54:56 UTC
-  32-bit CRC value (hex):                         00000000
-  compressed size:                                0 bytes
-  uncompressed size:                              0 bytes
-  length of filename:                             22 characters
+  file last modified on (DOS date/time):          2023 May 4 22:38:58
+  file last modified on (UT extra field modtime): 2023 May 5 02:38:58 local
+  file last modified on (UT extra field modtime): 2023 May 5 02:38:58 UTC
+  32-bit CRC value (hex):                         68ba1081
+  compressed size:                                8119 bytes
+  uncompressed size:                              46960 bytes
+  length of filename:                             30 characters
   length of extra field:                          24 bytes
   length of file comment:                         0 characters
   disk number on which file begins:               disk 1
-  apparent file type:                             binary
-  Unix file attributes (040755 octal):            drwxr-xr-x
-  MS-DOS file attributes (10 hex):                dir 
+  apparent file type:                             text
+  Unix file attributes (100666 octal):            -rw-rw-rw-
+  MS-DOS file attributes (00 hex):                none
 
   The central-directory extra field contains:
   - A subfield with ID 0x5455 (universal time) and 5 data bytes.
     The local extra field has UTC/GMT modification/access times.
   - A subfield with ID 0x7875 (Unix UID/GID (any size)) and 11 data bytes:
-    01 04 e8 03 00 00 04 e8 03 00 00.
+    01 04 f5 01 00 00 04 14 00 00 00.
 
   There is no file comment.
 
 Central directory entry #72:
 ---------------------------
 
-  torchaudio/functional/functional.py
+  torchaudio/models/conv_tasnet.py
 
-  offset of local header from start of archive:   2006543
-                                                  (00000000001E9E0Fh) bytes
+  offset of local header from start of archive:   119153
+                                                  (000000000001D171h) bytes
   file system or operating system of origin:      Unix
   version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               maximum
   file security status:                           not encrypted
   extended local header:                          no
-  file last modified on (DOS date/time):          2023 Mar 15 17:25:54
-  file last modified on (UT extra field modtime): 2023 Mar 16 00:25:54 local
-  file last modified on (UT extra field modtime): 2023 Mar 16 00:25:54 UTC
-  32-bit CRC value (hex):                         6a3e485d
-  compressed size:                                23219 bytes
-  uncompressed size:                              100038 bytes
-  length of filename:                             35 characters
+  file last modified on (DOS date/time):          2023 May 4 22:38:58
+  file last modified on (UT extra field modtime): 2023 May 5 02:38:58 local
+  file last modified on (UT extra field modtime): 2023 May 5 02:38:58 UTC
+  32-bit CRC value (hex):                         14911e69
+  compressed size:                                3141 bytes
+  uncompressed size:                              12870 bytes
+  length of filename:                             32 characters
   length of extra field:                          24 bytes
   length of file comment:                         0 characters
   disk number on which file begins:               disk 1
   apparent file type:                             text
   Unix file attributes (100666 octal):            -rw-rw-rw-
   MS-DOS file attributes (00 hex):                none
 
   The central-directory extra field contains:
   - A subfield with ID 0x5455 (universal time) and 5 data bytes.
     The local extra field has UTC/GMT modification/access times.
   - A subfield with ID 0x7875 (Unix UID/GID (any size)) and 11 data bytes:
-    01 04 e8 03 00 00 04 e8 03 00 00.
+    01 04 f5 01 00 00 04 14 00 00 00.
 
   There is no file comment.
 
 Central directory entry #73:
 ---------------------------
 
-  torchaudio/functional/filtering.py
+  torchaudio/models/decoder/
 
-  offset of local header from start of archive:   2029855
-                                                  (00000000001EF91Fh) bytes
+  offset of local header from start of archive:   122384
+                                                  (000000000001DE10h) bytes
   file system or operating system of origin:      Unix
   version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
-  minimum software version required to extract:   2.0
-  compression method:                             deflated
-  compression sub-type (deflation):               maximum
+  minimum software version required to extract:   1.0
+  compression method:                             none (stored)
   file security status:                           not encrypted
   extended local header:                          no
-  file last modified on (DOS date/time):          2023 Mar 15 17:25:54
-  file last modified on (UT extra field modtime): 2023 Mar 16 00:25:54 local
-  file last modified on (UT extra field modtime): 2023 Mar 16 00:25:54 UTC
-  32-bit CRC value (hex):                         a91bdce6
-  compressed size:                                12639 bytes
-  uncompressed size:                              63877 bytes
-  length of filename:                             34 characters
+  file last modified on (DOS date/time):          2023 May 6 14:35:50
+  file last modified on (UT extra field modtime): 2023 May 6 18:35:50 local
+  file last modified on (UT extra field modtime): 2023 May 6 18:35:50 UTC
+  32-bit CRC value (hex):                         00000000
+  compressed size:                                0 bytes
+  uncompressed size:                              0 bytes
+  length of filename:                             26 characters
   length of extra field:                          24 bytes
   length of file comment:                         0 characters
   disk number on which file begins:               disk 1
-  apparent file type:                             text
-  Unix file attributes (100666 octal):            -rw-rw-rw-
-  MS-DOS file attributes (00 hex):                none
+  apparent file type:                             binary
+  Unix file attributes (040755 octal):            drwxr-xr-x
+  MS-DOS file attributes (10 hex):                dir 
 
   The central-directory extra field contains:
   - A subfield with ID 0x5455 (universal time) and 5 data bytes.
     The local extra field has UTC/GMT modification/access times.
   - A subfield with ID 0x7875 (Unix UID/GID (any size)) and 11 data bytes:
-    01 04 e8 03 00 00 04 e8 03 00 00.
+    01 04 f5 01 00 00 04 14 00 00 00.
 
   There is no file comment.
 
 Central directory entry #74:
 ---------------------------
 
-  torchaudio/functional/__init__.py
+  torchaudio/models/decoder/_ctc_decoder.py
 
-  offset of local header from start of archive:   2042586
-                                                  (00000000001F2ADAh) bytes
+  offset of local header from start of archive:   122468
+                                                  (000000000001DE64h) bytes
   file system or operating system of origin:      Unix
   version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               maximum
   file security status:                           not encrypted
   extended local header:                          no
-  file last modified on (DOS date/time):          2023 Mar 15 17:25:54
-  file last modified on (UT extra field modtime): 2023 Mar 16 00:25:54 local
-  file last modified on (UT extra field modtime): 2023 Mar 16 00:25:54 UTC
-  32-bit CRC value (hex):                         16da4eff
-  compressed size:                                672 bytes
-  uncompressed size:                              2367 bytes
-  length of filename:                             33 characters
+  file last modified on (DOS date/time):          2023 May 4 22:38:58
+  file last modified on (UT extra field modtime): 2023 May 5 02:38:58 local
+  file last modified on (UT extra field modtime): 2023 May 5 02:38:58 UTC
+  32-bit CRC value (hex):                         efb59aa5
+  compressed size:                                5077 bytes
+  uncompressed size:                              18903 bytes
+  length of filename:                             41 characters
   length of extra field:                          24 bytes
   length of file comment:                         0 characters
   disk number on which file begins:               disk 1
   apparent file type:                             text
   Unix file attributes (100666 octal):            -rw-rw-rw-
   MS-DOS file attributes (00 hex):                none
 
   The central-directory extra field contains:
   - A subfield with ID 0x5455 (universal time) and 5 data bytes.
     The local extra field has UTC/GMT modification/access times.
   - A subfield with ID 0x7875 (Unix UID/GID (any size)) and 11 data bytes:
-    01 04 e8 03 00 00 04 e8 03 00 00.
+    01 04 f5 01 00 00 04 14 00 00 00.
 
   There is no file comment.
 
 Central directory entry #75:
 ---------------------------
 
-  torchaudio/datasets/
+  torchaudio/models/decoder/__init__.py
 
-  offset of local header from start of archive:   2043349
-                                                  (00000000001F2DD5h) bytes
+  offset of local header from start of archive:   127644
+                                                  (000000000001F29Ch) bytes
   file system or operating system of origin:      Unix
   version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
-  minimum software version required to extract:   1.0
-  compression method:                             none (stored)
+  minimum software version required to extract:   2.0
+  compression method:                             deflated
+  compression sub-type (deflation):               maximum
   file security status:                           not encrypted
   extended local header:                          no
-  file last modified on (DOS date/time):          2023 Mar 15 10:54:56
-  file last modified on (UT extra field modtime): 2023 Mar 15 17:54:56 local
-  file last modified on (UT extra field modtime): 2023 Mar 15 17:54:56 UTC
-  32-bit CRC value (hex):                         00000000
-  compressed size:                                0 bytes
-  uncompressed size:                              0 bytes
-  length of filename:                             20 characters
+  file last modified on (DOS date/time):          2023 May 4 22:38:58
+  file last modified on (UT extra field modtime): 2023 May 5 02:38:58 local
+  file last modified on (UT extra field modtime): 2023 May 5 02:38:58 UTC
+  32-bit CRC value (hex):                         7b253cb5
+  compressed size:                                392 bytes
+  uncompressed size:                              783 bytes
+  length of filename:                             37 characters
   length of extra field:                          24 bytes
   length of file comment:                         0 characters
   disk number on which file begins:               disk 1
-  apparent file type:                             binary
-  Unix file attributes (040755 octal):            drwxr-xr-x
-  MS-DOS file attributes (10 hex):                dir 
+  apparent file type:                             text
+  Unix file attributes (100666 octal):            -rw-rw-rw-
+  MS-DOS file attributes (00 hex):                none
 
   The central-directory extra field contains:
   - A subfield with ID 0x5455 (universal time) and 5 data bytes.
     The local extra field has UTC/GMT modification/access times.
   - A subfield with ID 0x7875 (Unix UID/GID (any size)) and 11 data bytes:
-    01 04 e8 03 00 00 04 e8 03 00 00.
+    01 04 f5 01 00 00 04 14 00 00 00.
 
   There is no file comment.
 
 Central directory entry #76:
 ---------------------------
 
-  torchaudio/datasets/yesno.py
+  torchaudio/models/rnnt_decoder.py
 
-  offset of local header from start of archive:   2043427
-                                                  (00000000001F2E23h) bytes
+  offset of local header from start of archive:   128131
+                                                  (000000000001F483h) bytes
   file system or operating system of origin:      Unix
   version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               maximum
   file security status:                           not encrypted
   extended local header:                          no
-  file last modified on (DOS date/time):          2023 Mar 15 17:25:54
-  file last modified on (UT extra field modtime): 2023 Mar 16 00:25:54 local
-  file last modified on (UT extra field modtime): 2023 Mar 16 00:25:54 UTC
-  32-bit CRC value (hex):                         f2316e0c
-  compressed size:                                1144 bytes
-  uncompressed size:                              3104 bytes
-  length of filename:                             28 characters
+  file last modified on (DOS date/time):          2023 May 4 22:38:58
+  file last modified on (UT extra field modtime): 2023 May 5 02:38:58 local
+  file last modified on (UT extra field modtime): 2023 May 5 02:38:58 UTC
+  32-bit CRC value (hex):                         e77e0b91
+  compressed size:                                3091 bytes
+  uncompressed size:                              13311 bytes
+  length of filename:                             33 characters
   length of extra field:                          24 bytes
   length of file comment:                         0 characters
   disk number on which file begins:               disk 1
   apparent file type:                             text
   Unix file attributes (100666 octal):            -rw-rw-rw-
   MS-DOS file attributes (00 hex):                none
 
   The central-directory extra field contains:
   - A subfield with ID 0x5455 (universal time) and 5 data bytes.
     The local extra field has UTC/GMT modification/access times.
   - A subfield with ID 0x7875 (Unix UID/GID (any size)) and 11 data bytes:
-    01 04 e8 03 00 00 04 e8 03 00 00.
+    01 04 f5 01 00 00 04 14 00 00 00.
 
   There is no file comment.
 
 Central directory entry #77:
 ---------------------------
 
-  torchaudio/datasets/voxceleb1.py
+  torchaudio/models/__init__.py
 
-  offset of local header from start of archive:   2044657
-                                                  (00000000001F32F1h) bytes
+  offset of local header from start of archive:   131313
+                                                  (00000000000200F1h) bytes
   file system or operating system of origin:      Unix
   version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               maximum
   file security status:                           not encrypted
   extended local header:                          no
-  file last modified on (DOS date/time):          2023 Mar 15 17:25:54
-  file last modified on (UT extra field modtime): 2023 Mar 16 00:25:54 local
-  file last modified on (UT extra field modtime): 2023 Mar 16 00:25:54 UTC
-  32-bit CRC value (hex):                         5232284b
-  compressed size:                                2932 bytes
-  uncompressed size:                              12023 bytes
-  length of filename:                             32 characters
+  file last modified on (DOS date/time):          2023 May 4 22:38:58
+  file last modified on (UT extra field modtime): 2023 May 5 02:38:58 local
+  file last modified on (UT extra field modtime): 2023 May 5 02:38:58 UTC
+  32-bit CRC value (hex):                         0032e328
+  compressed size:                                469 bytes
+  uncompressed size:                              1733 bytes
+  length of filename:                             29 characters
   length of extra field:                          24 bytes
   length of file comment:                         0 characters
   disk number on which file begins:               disk 1
   apparent file type:                             text
   Unix file attributes (100666 octal):            -rw-rw-rw-
   MS-DOS file attributes (00 hex):                none
 
   The central-directory extra field contains:
   - A subfield with ID 0x5455 (universal time) and 5 data bytes.
     The local extra field has UTC/GMT modification/access times.
   - A subfield with ID 0x7875 (Unix UID/GID (any size)) and 11 data bytes:
-    01 04 e8 03 00 00 04 e8 03 00 00.
+    01 04 f5 01 00 00 04 14 00 00 00.
 
   There is no file comment.
 
 Central directory entry #78:
 ---------------------------
 
-  torchaudio/datasets/vctk.py
+  torchaudio/models/deepspeech.py
 
-  offset of local header from start of archive:   2047679
-                                                  (00000000001F3EBFh) bytes
+  offset of local header from start of archive:   131869
+                                                  (000000000002031Dh) bytes
   file system or operating system of origin:      Unix
   version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               maximum
   file security status:                           not encrypted
   extended local header:                          no
-  file last modified on (DOS date/time):          2023 Mar 15 17:25:54
-  file last modified on (UT extra field modtime): 2023 Mar 16 00:25:54 local
-  file last modified on (UT extra field modtime): 2023 Mar 16 00:25:54 UTC
-  32-bit CRC value (hex):                         583d6082
-  compressed size:                                1922 bytes
-  uncompressed size:                              5831 bytes
-  length of filename:                             27 characters
+  file last modified on (DOS date/time):          2023 May 4 22:38:58
+  file last modified on (UT extra field modtime): 2023 May 5 02:38:58 local
+  file last modified on (UT extra field modtime): 2023 May 5 02:38:58 UTC
+  32-bit CRC value (hex):                         a1897685
+  compressed size:                                843 bytes
+  uncompressed size:                              2830 bytes
+  length of filename:                             31 characters
   length of extra field:                          24 bytes
   length of file comment:                         0 characters
   disk number on which file begins:               disk 1
   apparent file type:                             text
   Unix file attributes (100666 octal):            -rw-rw-rw-
   MS-DOS file attributes (00 hex):                none
 
   The central-directory extra field contains:
   - A subfield with ID 0x5455 (universal time) and 5 data bytes.
     The local extra field has UTC/GMT modification/access times.
   - A subfield with ID 0x7875 (Unix UID/GID (any size)) and 11 data bytes:
-    01 04 e8 03 00 00 04 e8 03 00 00.
+    01 04 f5 01 00 00 04 14 00 00 00.
 
   There is no file comment.
 
 Central directory entry #79:
 ---------------------------
 
-  torchaudio/datasets/utils.py
+  torchaudio/models/wav2vec2/
 
-  offset of local header from start of archive:   2049686
-                                                  (00000000001F4696h) bytes
+  offset of local header from start of archive:   132801
+                                                  (00000000000206C1h) bytes
   file system or operating system of origin:      Unix
   version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
-  minimum software version required to extract:   2.0
-  compression method:                             deflated
-  compression sub-type (deflation):               maximum
+  minimum software version required to extract:   1.0
+  compression method:                             none (stored)
   file security status:                           not encrypted
   extended local header:                          no
-  file last modified on (DOS date/time):          2023 Mar 15 17:25:54
-  file last modified on (UT extra field modtime): 2023 Mar 16 00:25:54 local
-  file last modified on (UT extra field modtime): 2023 Mar 16 00:25:54 UTC
-  32-bit CRC value (hex):                         e0a6acad
-  compressed size:                                561 bytes
-  uncompressed size:                              1840 bytes
-  length of filename:                             28 characters
+  file last modified on (DOS date/time):          2023 May 6 14:35:50
+  file last modified on (UT extra field modtime): 2023 May 6 18:35:50 local
+  file last modified on (UT extra field modtime): 2023 May 6 18:35:50 UTC
+  32-bit CRC value (hex):                         00000000
+  compressed size:                                0 bytes
+  uncompressed size:                              0 bytes
+  length of filename:                             27 characters
   length of extra field:                          24 bytes
   length of file comment:                         0 characters
   disk number on which file begins:               disk 1
-  apparent file type:                             text
-  Unix file attributes (100666 octal):            -rw-rw-rw-
-  MS-DOS file attributes (00 hex):                none
+  apparent file type:                             binary
+  Unix file attributes (040755 octal):            drwxr-xr-x
+  MS-DOS file attributes (10 hex):                dir 
 
   The central-directory extra field contains:
   - A subfield with ID 0x5455 (universal time) and 5 data bytes.
     The local extra field has UTC/GMT modification/access times.
   - A subfield with ID 0x7875 (Unix UID/GID (any size)) and 11 data bytes:
-    01 04 e8 03 00 00 04 e8 03 00 00.
+    01 04 f5 01 00 00 04 14 00 00 00.
 
   There is no file comment.
 
 Central directory entry #80:
 ---------------------------
 
-  torchaudio/datasets/tedlium.py
+  torchaudio/models/wav2vec2/wavlm_attention.py
 
-  offset of local header from start of archive:   2050333
-                                                  (00000000001F491Dh) bytes
+  offset of local header from start of archive:   132886
+                                                  (0000000000020716h) bytes
   file system or operating system of origin:      Unix
   version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               maximum
   file security status:                           not encrypted
   extended local header:                          no
-  file last modified on (DOS date/time):          2023 Mar 15 17:25:54
-  file last modified on (UT extra field modtime): 2023 Mar 16 00:25:54 local
-  file last modified on (UT extra field modtime): 2023 Mar 16 00:25:54 UTC
-  32-bit CRC value (hex):                         88c4225a
-  compressed size:                                2660 bytes
-  uncompressed size:                              8905 bytes
-  length of filename:                             30 characters
+  file last modified on (DOS date/time):          2023 May 4 22:38:58
+  file last modified on (UT extra field modtime): 2023 May 5 02:38:58 local
+  file last modified on (UT extra field modtime): 2023 May 5 02:38:58 UTC
+  32-bit CRC value (hex):                         4ec67ce4
+  compressed size:                                3339 bytes
+  uncompressed size:                              11058 bytes
+  length of filename:                             45 characters
   length of extra field:                          24 bytes
   length of file comment:                         0 characters
   disk number on which file begins:               disk 1
   apparent file type:                             text
   Unix file attributes (100666 octal):            -rw-rw-rw-
   MS-DOS file attributes (00 hex):                none
 
   The central-directory extra field contains:
   - A subfield with ID 0x5455 (universal time) and 5 data bytes.
     The local extra field has UTC/GMT modification/access times.
   - A subfield with ID 0x7875 (Unix UID/GID (any size)) and 11 data bytes:
-    01 04 e8 03 00 00 04 e8 03 00 00.
+    01 04 f5 01 00 00 04 14 00 00 00.
 
   There is no file comment.
 
 Central directory entry #81:
 ---------------------------
 
-  torchaudio/datasets/speechcommands.py
+  torchaudio/models/wav2vec2/__init__.py
 
-  offset of local header from start of archive:   2053081
-                                                  (00000000001F53D9h) bytes
+  offset of local header from start of archive:   136328
+                                                  (0000000000021488h) bytes
   file system or operating system of origin:      Unix
   version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               maximum
   file security status:                           not encrypted
   extended local header:                          no
-  file last modified on (DOS date/time):          2023 Mar 15 17:25:54
-  file last modified on (UT extra field modtime): 2023 Mar 16 00:25:54 local
-  file last modified on (UT extra field modtime): 2023 Mar 16 00:25:54 UTC
-  32-bit CRC value (hex):                         585820af
-  compressed size:                                2478 bytes
-  uncompressed size:                              7653 bytes
-  length of filename:                             37 characters
+  file last modified on (DOS date/time):          2023 May 4 22:38:58
+  file last modified on (UT extra field modtime): 2023 May 5 02:38:58 local
+  file last modified on (UT extra field modtime): 2023 May 5 02:38:58 UTC
+  32-bit CRC value (hex):                         93bedda6
+  compressed size:                                252 bytes
+  uncompressed size:                              972 bytes
+  length of filename:                             38 characters
   length of extra field:                          24 bytes
   length of file comment:                         0 characters
   disk number on which file begins:               disk 1
   apparent file type:                             text
   Unix file attributes (100666 octal):            -rw-rw-rw-
   MS-DOS file attributes (00 hex):                none
 
   The central-directory extra field contains:
   - A subfield with ID 0x5455 (universal time) and 5 data bytes.
     The local extra field has UTC/GMT modification/access times.
   - A subfield with ID 0x7875 (Unix UID/GID (any size)) and 11 data bytes:
-    01 04 e8 03 00 00 04 e8 03 00 00.
+    01 04 f5 01 00 00 04 14 00 00 00.
 
   There is no file comment.
 
 Central directory entry #82:
 ---------------------------
 
-  torchaudio/datasets/snips.py
+  torchaudio/models/wav2vec2/utils/
 
-  offset of local header from start of archive:   2055654
-                                                  (00000000001F5DE6h) bytes
+  offset of local header from start of archive:   136676
+                                                  (00000000000215E4h) bytes
   file system or operating system of origin:      Unix
   version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
-  minimum software version required to extract:   2.0
-  compression method:                             deflated
-  compression sub-type (deflation):               maximum
+  minimum software version required to extract:   1.0
+  compression method:                             none (stored)
   file security status:                           not encrypted
   extended local header:                          no
-  file last modified on (DOS date/time):          2023 Mar 15 17:25:54
-  file last modified on (UT extra field modtime): 2023 Mar 16 00:25:54 local
-  file last modified on (UT extra field modtime): 2023 Mar 16 00:25:54 UTC
-  32-bit CRC value (hex):                         48e8a358
-  compressed size:                                1613 bytes
-  uncompressed size:                              5165 bytes
-  length of filename:                             28 characters
+  file last modified on (DOS date/time):          2023 May 6 14:35:50
+  file last modified on (UT extra field modtime): 2023 May 6 18:35:50 local
+  file last modified on (UT extra field modtime): 2023 May 6 18:35:50 UTC
+  32-bit CRC value (hex):                         00000000
+  compressed size:                                0 bytes
+  uncompressed size:                              0 bytes
+  length of filename:                             33 characters
   length of extra field:                          24 bytes
   length of file comment:                         0 characters
   disk number on which file begins:               disk 1
-  apparent file type:                             text
-  Unix file attributes (100666 octal):            -rw-rw-rw-
-  MS-DOS file attributes (00 hex):                none
+  apparent file type:                             binary
+  Unix file attributes (040755 octal):            drwxr-xr-x
+  MS-DOS file attributes (10 hex):                dir 
 
   The central-directory extra field contains:
   - A subfield with ID 0x5455 (universal time) and 5 data bytes.
     The local extra field has UTC/GMT modification/access times.
   - A subfield with ID 0x7875 (Unix UID/GID (any size)) and 11 data bytes:
-    01 04 e8 03 00 00 04 e8 03 00 00.
+    01 04 f5 01 00 00 04 14 00 00 00.
 
   There is no file comment.
 
 Central directory entry #83:
 ---------------------------
 
-  torchaudio/datasets/quesst14.py
+  torchaudio/models/wav2vec2/utils/__init__.py
 
-  offset of local header from start of archive:   2057353
-                                                  (00000000001F6489h) bytes
+  offset of local header from start of archive:   136767
+                                                  (000000000002163Fh) bytes
   file system or operating system of origin:      Unix
   version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               maximum
   file security status:                           not encrypted
   extended local header:                          no
-  file last modified on (DOS date/time):          2023 Mar 15 17:25:54
-  file last modified on (UT extra field modtime): 2023 Mar 16 00:25:54 local
-  file last modified on (UT extra field modtime): 2023 Mar 16 00:25:54 UTC
-  32-bit CRC value (hex):                         efb792ea
-  compressed size:                                1617 bytes
-  uncompressed size:                              4580 bytes
-  length of filename:                             31 characters
+  file last modified on (DOS date/time):          2023 May 4 22:38:58
+  file last modified on (UT extra field modtime): 2023 May 5 02:38:58 local
+  file last modified on (UT extra field modtime): 2023 May 5 02:38:58 UTC
+  32-bit CRC value (hex):                         2cd08f42
+  compressed size:                                88 bytes
+  uncompressed size:                              188 bytes
+  length of filename:                             44 characters
   length of extra field:                          24 bytes
   length of file comment:                         0 characters
   disk number on which file begins:               disk 1
   apparent file type:                             text
   Unix file attributes (100666 octal):            -rw-rw-rw-
   MS-DOS file attributes (00 hex):                none
 
   The central-directory extra field contains:
   - A subfield with ID 0x5455 (universal time) and 5 data bytes.
     The local extra field has UTC/GMT modification/access times.
   - A subfield with ID 0x7875 (Unix UID/GID (any size)) and 11 data bytes:
-    01 04 e8 03 00 00 04 e8 03 00 00.
+    01 04 f5 01 00 00 04 14 00 00 00.
 
   There is no file comment.
 
 Central directory entry #84:
 ---------------------------
 
-  torchaudio/datasets/musdb_hq.py
+  torchaudio/models/wav2vec2/utils/import_huggingface.py
 
-  offset of local header from start of archive:   2059059
-                                                  (00000000001F6B33h) bytes
+  offset of local header from start of archive:   136957
+                                                  (00000000000216FDh) bytes
   file system or operating system of origin:      Unix
   version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               maximum
   file security status:                           not encrypted
   extended local header:                          no
-  file last modified on (DOS date/time):          2023 Mar 15 17:25:54
-  file last modified on (UT extra field modtime): 2023 Mar 16 00:25:54 local
-  file last modified on (UT extra field modtime): 2023 Mar 16 00:25:54 UTC
-  32-bit CRC value (hex):                         828a85bf
-  compressed size:                                1998 bytes
-  uncompressed size:                              5203 bytes
-  length of filename:                             31 characters
+  file last modified on (DOS date/time):          2023 May 4 22:38:58
+  file last modified on (UT extra field modtime): 2023 May 5 02:38:58 local
+  file last modified on (UT extra field modtime): 2023 May 5 02:38:58 UTC
+  32-bit CRC value (hex):                         4527440a
+  compressed size:                                1516 bytes
+  uncompressed size:                              6080 bytes
+  length of filename:                             54 characters
   length of extra field:                          24 bytes
   length of file comment:                         0 characters
   disk number on which file begins:               disk 1
   apparent file type:                             text
   Unix file attributes (100666 octal):            -rw-rw-rw-
   MS-DOS file attributes (00 hex):                none
 
   The central-directory extra field contains:
   - A subfield with ID 0x5455 (universal time) and 5 data bytes.
     The local extra field has UTC/GMT modification/access times.
   - A subfield with ID 0x7875 (Unix UID/GID (any size)) and 11 data bytes:
-    01 04 e8 03 00 00 04 e8 03 00 00.
+    01 04 f5 01 00 00 04 14 00 00 00.
 
   There is no file comment.
 
 Central directory entry #85:
 ---------------------------
 
-  torchaudio/datasets/ljspeech.py
+  torchaudio/models/wav2vec2/utils/import_fairseq.py
 
-  offset of local header from start of archive:   2061146
-                                                  (00000000001F735Ah) bytes
+  offset of local header from start of archive:   138585
+                                                  (0000000000021D59h) bytes
   file system or operating system of origin:      Unix
   version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               maximum
   file security status:                           not encrypted
   extended local header:                          no
-  file last modified on (DOS date/time):          2023 Mar 15 17:25:54
-  file last modified on (UT extra field modtime): 2023 Mar 16 00:25:54 local
-  file last modified on (UT extra field modtime): 2023 Mar 16 00:25:54 UTC
-  32-bit CRC value (hex):                         ff041fd2
-  compressed size:                                1279 bytes
-  uncompressed size:                              3590 bytes
-  length of filename:                             31 characters
+  file last modified on (DOS date/time):          2023 May 4 22:38:58
+  file last modified on (UT extra field modtime): 2023 May 5 02:38:58 local
+  file last modified on (UT extra field modtime): 2023 May 5 02:38:58 UTC
+  32-bit CRC value (hex):                         35a405ba
+  compressed size:                                2140 bytes
+  uncompressed size:                              9411 bytes
+  length of filename:                             50 characters
   length of extra field:                          24 bytes
   length of file comment:                         0 characters
   disk number on which file begins:               disk 1
   apparent file type:                             text
   Unix file attributes (100666 octal):            -rw-rw-rw-
   MS-DOS file attributes (00 hex):                none
 
   The central-directory extra field contains:
   - A subfield with ID 0x5455 (universal time) and 5 data bytes.
     The local extra field has UTC/GMT modification/access times.
   - A subfield with ID 0x7875 (Unix UID/GID (any size)) and 11 data bytes:
-    01 04 e8 03 00 00 04 e8 03 00 00.
+    01 04 f5 01 00 00 04 14 00 00 00.
 
   There is no file comment.
 
 Central directory entry #86:
 ---------------------------
 
-  torchaudio/datasets/libritts.py
+  torchaudio/models/wav2vec2/model.py
 
-  offset of local header from start of archive:   2062514
-                                                  (00000000001F78B2h) bytes
+  offset of local header from start of archive:   140833
+                                                  (0000000000022621h) bytes
   file system or operating system of origin:      Unix
   version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               maximum
   file security status:                           not encrypted
   extended local header:                          no
-  file last modified on (DOS date/time):          2023 Mar 15 17:25:54
-  file last modified on (UT extra field modtime): 2023 Mar 16 00:25:54 local
-  file last modified on (UT extra field modtime): 2023 Mar 16 00:25:54 UTC
-  32-bit CRC value (hex):                         d4164a08
-  compressed size:                                1991 bytes
-  uncompressed size:                              6027 bytes
-  length of filename:                             31 characters
+  file last modified on (DOS date/time):          2023 May 4 22:38:58
+  file last modified on (UT extra field modtime): 2023 May 5 02:38:58 local
+  file last modified on (UT extra field modtime): 2023 May 5 02:38:58 UTC
+  32-bit CRC value (hex):                         9fb3eaa1
+  compressed size:                                6249 bytes
+  uncompressed size:                              61671 bytes
+  length of filename:                             35 characters
   length of extra field:                          24 bytes
   length of file comment:                         0 characters
   disk number on which file begins:               disk 1
   apparent file type:                             text
   Unix file attributes (100666 octal):            -rw-rw-rw-
   MS-DOS file attributes (00 hex):                none
 
   The central-directory extra field contains:
   - A subfield with ID 0x5455 (universal time) and 5 data bytes.
     The local extra field has UTC/GMT modification/access times.
   - A subfield with ID 0x7875 (Unix UID/GID (any size)) and 11 data bytes:
-    01 04 e8 03 00 00 04 e8 03 00 00.
+    01 04 f5 01 00 00 04 14 00 00 00.
 
   There is no file comment.
 
 Central directory entry #87:
 ---------------------------
 
-  torchaudio/datasets/librispeech.py
+  torchaudio/models/wav2vec2/components.py
 
-  offset of local header from start of archive:   2064594
-                                                  (00000000001F80D2h) bytes
+  offset of local header from start of archive:   147175
+                                                  (0000000000023EE7h) bytes
   file system or operating system of origin:      Unix
   version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               maximum
   file security status:                           not encrypted
   extended local header:                          no
-  file last modified on (DOS date/time):          2023 Mar 15 17:25:54
-  file last modified on (UT extra field modtime): 2023 Mar 16 00:25:54 local
-  file last modified on (UT extra field modtime): 2023 Mar 16 00:25:54 UTC
-  32-bit CRC value (hex):                         0302596a
-  compressed size:                                2146 bytes
-  uncompressed size:                              6474 bytes
-  length of filename:                             34 characters
+  file last modified on (DOS date/time):          2023 May 4 22:38:58
+  file last modified on (UT extra field modtime): 2023 May 5 02:38:58 local
+  file last modified on (UT extra field modtime): 2023 May 5 02:38:58 UTC
+  32-bit CRC value (hex):                         0446c642
+  compressed size:                                9419 bytes
+  uncompressed size:                              48631 bytes
+  length of filename:                             40 characters
   length of extra field:                          24 bytes
   length of file comment:                         0 characters
   disk number on which file begins:               disk 1
   apparent file type:                             text
   Unix file attributes (100666 octal):            -rw-rw-rw-
   MS-DOS file attributes (00 hex):                none
 
   The central-directory extra field contains:
   - A subfield with ID 0x5455 (universal time) and 5 data bytes.
     The local extra field has UTC/GMT modification/access times.
   - A subfield with ID 0x7875 (Unix UID/GID (any size)) and 11 data bytes:
-    01 04 e8 03 00 00 04 e8 03 00 00.
+    01 04 f5 01 00 00 04 14 00 00 00.
 
   There is no file comment.
 
 Central directory entry #88:
 ---------------------------
 
-  torchaudio/datasets/librimix.py
+  torchaudio/models/_hdemucs.py
 
-  offset of local header from start of archive:   2066832
-                                                  (00000000001F8990h) bytes
+  offset of local header from start of archive:   156692
+                                                  (0000000000026414h) bytes
   file system or operating system of origin:      Unix
   version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               maximum
   file security status:                           not encrypted
   extended local header:                          no
-  file last modified on (DOS date/time):          2023 Mar 15 17:25:54
-  file last modified on (UT extra field modtime): 2023 Mar 16 00:25:54 local
-  file last modified on (UT extra field modtime): 2023 Mar 16 00:25:54 UTC
-  32-bit CRC value (hex):                         de3d07c5
-  compressed size:                                1726 bytes
-  uncompressed size:                              5249 bytes
-  length of filename:                             31 characters
+  file last modified on (DOS date/time):          2023 May 4 22:38:58
+  file last modified on (UT extra field modtime): 2023 May 5 02:38:58 local
+  file last modified on (UT extra field modtime): 2023 May 5 02:38:58 UTC
+  32-bit CRC value (hex):                         31482b45
+  compressed size:                                9941 bytes
+  uncompressed size:                              39250 bytes
+  length of filename:                             29 characters
   length of extra field:                          24 bytes
   length of file comment:                         0 characters
   disk number on which file begins:               disk 1
   apparent file type:                             text
   Unix file attributes (100666 octal):            -rw-rw-rw-
   MS-DOS file attributes (00 hex):                none
 
   The central-directory extra field contains:
   - A subfield with ID 0x5455 (universal time) and 5 data bytes.
     The local extra field has UTC/GMT modification/access times.
   - A subfield with ID 0x7875 (Unix UID/GID (any size)) and 11 data bytes:
-    01 04 e8 03 00 00 04 e8 03 00 00.
+    01 04 f5 01 00 00 04 14 00 00 00.
 
   There is no file comment.
 
 Central directory entry #89:
 ---------------------------
 
-  torchaudio/datasets/librilight_limited.py
+  torchaudio/models/conformer.py
 
-  offset of local header from start of archive:   2068647
-                                                  (00000000001F90A7h) bytes
+  offset of local header from start of archive:   166720
+                                                  (0000000000028B40h) bytes
   file system or operating system of origin:      Unix
   version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               maximum
   file security status:                           not encrypted
   extended local header:                          no
-  file last modified on (DOS date/time):          2023 Mar 15 17:25:54
-  file last modified on (UT extra field modtime): 2023 Mar 16 00:25:54 local
-  file last modified on (UT extra field modtime): 2023 Mar 16 00:25:54 UTC
-  32-bit CRC value (hex):                         eeddfe87
-  compressed size:                                1657 bytes
-  uncompressed size:                              4279 bytes
-  length of filename:                             41 characters
+  file last modified on (DOS date/time):          2023 May 4 22:38:58
+  file last modified on (UT extra field modtime): 2023 May 5 02:38:58 local
+  file last modified on (UT extra field modtime): 2023 May 5 02:38:58 UTC
+  32-bit CRC value (hex):                         b0959519
+  compressed size:                                2054 bytes
+  uncompressed size:                              10361 bytes
+  length of filename:                             30 characters
   length of extra field:                          24 bytes
   length of file comment:                         0 characters
   disk number on which file begins:               disk 1
   apparent file type:                             text
   Unix file attributes (100666 octal):            -rw-rw-rw-
   MS-DOS file attributes (00 hex):                none
 
   The central-directory extra field contains:
   - A subfield with ID 0x5455 (universal time) and 5 data bytes.
     The local extra field has UTC/GMT modification/access times.
   - A subfield with ID 0x7875 (Unix UID/GID (any size)) and 11 data bytes:
-    01 04 e8 03 00 00 04 e8 03 00 00.
+    01 04 f5 01 00 00 04 14 00 00 00.
 
   There is no file comment.
 
 Central directory entry #90:
 ---------------------------
 
-  torchaudio/datasets/iemocap.py
+  torchaudio/models/wavernn.py
 
-  offset of local header from start of archive:   2070403
-                                                  (00000000001F9783h) bytes
+  offset of local header from start of archive:   168862
+                                                  (000000000002939Eh) bytes
   file system or operating system of origin:      Unix
   version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               maximum
   file security status:                           not encrypted
   extended local header:                          no
-  file last modified on (DOS date/time):          2023 Mar 15 17:25:54
-  file last modified on (UT extra field modtime): 2023 Mar 16 00:25:54 local
-  file last modified on (UT extra field modtime): 2023 Mar 16 00:25:54 UTC
-  32-bit CRC value (hex):                         b9d296ed
-  compressed size:                                1523 bytes
-  uncompressed size:                              5077 bytes
-  length of filename:                             30 characters
+  file last modified on (DOS date/time):          2023 May 4 22:38:58
+  file last modified on (UT extra field modtime): 2023 May 5 02:38:58 local
+  file last modified on (UT extra field modtime): 2023 May 5 02:38:58 UTC
+  32-bit CRC value (hex):                         fe1c66da
+  compressed size:                                3629 bytes
+  uncompressed size:                              15855 bytes
+  length of filename:                             28 characters
   length of extra field:                          24 bytes
   length of file comment:                         0 characters
   disk number on which file begins:               disk 1
   apparent file type:                             text
   Unix file attributes (100666 octal):            -rw-rw-rw-
   MS-DOS file attributes (00 hex):                none
 
   The central-directory extra field contains:
   - A subfield with ID 0x5455 (universal time) and 5 data bytes.
     The local extra field has UTC/GMT modification/access times.
   - A subfield with ID 0x7875 (Unix UID/GID (any size)) and 11 data bytes:
-    01 04 e8 03 00 00 04 e8 03 00 00.
+    01 04 f5 01 00 00 04 14 00 00 00.
 
   There is no file comment.
 
 Central directory entry #91:
 ---------------------------
 
-  torchaudio/datasets/gtzan.py
+  torchaudio/models/rnnt.py
 
-  offset of local header from start of archive:   2072014
-                                                  (00000000001F9DCEh) bytes
+  offset of local header from start of archive:   172577
+                                                  (000000000002A221h) bytes
   file system or operating system of origin:      Unix
   version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               maximum
   file security status:                           not encrypted
   extended local header:                          no
-  file last modified on (DOS date/time):          2023 Mar 15 17:25:54
-  file last modified on (UT extra field modtime): 2023 Mar 16 00:25:54 local
-  file last modified on (UT extra field modtime): 2023 Mar 16 00:25:54 UTC
-  32-bit CRC value (hex):                         ac3f3605
-  compressed size:                                5046 bytes
-  uncompressed size:                              25464 bytes
-  length of filename:                             28 characters
+  file last modified on (DOS date/time):          2023 May 4 22:38:58
+  file last modified on (UT extra field modtime): 2023 May 5 02:38:58 local
+  file last modified on (UT extra field modtime): 2023 May 5 02:38:58 UTC
+  32-bit CRC value (hex):                         7bb1c586
+  compressed size:                                4925 bytes
+  uncompressed size:                              36357 bytes
+  length of filename:                             25 characters
   length of extra field:                          24 bytes
   length of file comment:                         0 characters
   disk number on which file begins:               disk 1
   apparent file type:                             text
   Unix file attributes (100666 octal):            -rw-rw-rw-
   MS-DOS file attributes (00 hex):                none
 
   The central-directory extra field contains:
   - A subfield with ID 0x5455 (universal time) and 5 data bytes.
     The local extra field has UTC/GMT modification/access times.
   - A subfield with ID 0x7875 (Unix UID/GID (any size)) and 11 data bytes:
-    01 04 e8 03 00 00 04 e8 03 00 00.
+    01 04 f5 01 00 00 04 14 00 00 00.
 
   There is no file comment.
 
 Central directory entry #92:
 ---------------------------
 
-  torchaudio/datasets/fluentcommands.py
+  torchaudio/compliance/
 
-  offset of local header from start of archive:   2077146
-                                                  (00000000001FB1DAh) bytes
+  offset of local header from start of archive:   177585
+                                                  (000000000002B5B1h) bytes
   file system or operating system of origin:      Unix
   version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
-  minimum software version required to extract:   2.0
-  compression method:                             deflated
-  compression sub-type (deflation):               maximum
+  minimum software version required to extract:   1.0
+  compression method:                             none (stored)
   file security status:                           not encrypted
   extended local header:                          no
-  file last modified on (DOS date/time):          2023 Mar 15 17:25:54
-  file last modified on (UT extra field modtime): 2023 Mar 16 00:25:54 local
-  file last modified on (UT extra field modtime): 2023 Mar 16 00:25:54 UTC
-  32-bit CRC value (hex):                         6c457126
-  compressed size:                                1052 bytes
-  uncompressed size:                              3353 bytes
-  length of filename:                             37 characters
+  file last modified on (DOS date/time):          2023 May 6 14:35:50
+  file last modified on (UT extra field modtime): 2023 May 6 18:35:50 local
+  file last modified on (UT extra field modtime): 2023 May 6 18:35:50 UTC
+  32-bit CRC value (hex):                         00000000
+  compressed size:                                0 bytes
+  uncompressed size:                              0 bytes
+  length of filename:                             22 characters
   length of extra field:                          24 bytes
   length of file comment:                         0 characters
   disk number on which file begins:               disk 1
-  apparent file type:                             text
-  Unix file attributes (100666 octal):            -rw-rw-rw-
-  MS-DOS file attributes (00 hex):                none
+  apparent file type:                             binary
+  Unix file attributes (040755 octal):            drwxr-xr-x
+  MS-DOS file attributes (10 hex):                dir 
 
   The central-directory extra field contains:
   - A subfield with ID 0x5455 (universal time) and 5 data bytes.
     The local extra field has UTC/GMT modification/access times.
   - A subfield with ID 0x7875 (Unix UID/GID (any size)) and 11 data bytes:
-    01 04 e8 03 00 00 04 e8 03 00 00.
+    01 04 f5 01 00 00 04 14 00 00 00.
 
   There is no file comment.
 
 Central directory entry #93:
 ---------------------------
 
-  torchaudio/datasets/dr_vctk.py
+  torchaudio/compliance/__init__.py
 
-  offset of local header from start of archive:   2078293
-                                                  (00000000001FB655h) bytes
+  offset of local header from start of archive:   177665
+                                                  (000000000002B601h) bytes
   file system or operating system of origin:      Unix
   version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               maximum
   file security status:                           not encrypted
   extended local header:                          no
-  file last modified on (DOS date/time):          2023 Mar 15 17:25:54
-  file last modified on (UT extra field modtime): 2023 Mar 16 00:25:54 local
-  file last modified on (UT extra field modtime): 2023 Mar 16 00:25:54 UTC
-  32-bit CRC value (hex):                         d86ec8a6
-  compressed size:                                1525 bytes
-  uncompressed size:                              4487 bytes
-  length of filename:                             30 characters
+  file last modified on (DOS date/time):          2023 May 4 22:38:58
+  file last modified on (UT extra field modtime): 2023 May 5 02:38:58 local
+  file last modified on (UT extra field modtime): 2023 May 5 02:38:58 UTC
+  32-bit CRC value (hex):                         d8cb8be0
+  compressed size:                                50 bytes
+  uncompressed size:                              53 bytes
+  length of filename:                             33 characters
   length of extra field:                          24 bytes
   length of file comment:                         0 characters
   disk number on which file begins:               disk 1
   apparent file type:                             text
   Unix file attributes (100666 octal):            -rw-rw-rw-
   MS-DOS file attributes (00 hex):                none
 
   The central-directory extra field contains:
   - A subfield with ID 0x5455 (universal time) and 5 data bytes.
     The local extra field has UTC/GMT modification/access times.
   - A subfield with ID 0x7875 (Unix UID/GID (any size)) and 11 data bytes:
-    01 04 e8 03 00 00 04 e8 03 00 00.
+    01 04 f5 01 00 00 04 14 00 00 00.
 
   There is no file comment.
 
 Central directory entry #94:
 ---------------------------
 
-  torchaudio/datasets/commonvoice.py
+  torchaudio/compliance/kaldi.py
 
-  offset of local header from start of archive:   2079906
-                                                  (00000000001FBCA2h) bytes
+  offset of local header from start of archive:   177806
+                                                  (000000000002B68Eh) bytes
   file system or operating system of origin:      Unix
   version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               maximum
   file security status:                           not encrypted
   extended local header:                          no
-  file last modified on (DOS date/time):          2023 Mar 15 17:25:54
-  file last modified on (UT extra field modtime): 2023 Mar 16 00:25:54 local
-  file last modified on (UT extra field modtime): 2023 Mar 16 00:25:54 UTC
-  32-bit CRC value (hex):                         d1499a8c
-  compressed size:                                1125 bytes
-  uncompressed size:                              2849 bytes
-  length of filename:                             34 characters
+  file last modified on (DOS date/time):          2023 May 4 22:38:58
+  file last modified on (UT extra field modtime): 2023 May 5 02:38:58 local
+  file last modified on (UT extra field modtime): 2023 May 5 02:38:58 UTC
+  32-bit CRC value (hex):                         32dcccf8
+  compressed size:                                7678 bytes
+  uncompressed size:                              37479 bytes
+  length of filename:                             30 characters
   length of extra field:                          24 bytes
   length of file comment:                         0 characters
   disk number on which file begins:               disk 1
   apparent file type:                             text
   Unix file attributes (100666 octal):            -rw-rw-rw-
   MS-DOS file attributes (00 hex):                none
 
   The central-directory extra field contains:
   - A subfield with ID 0x5455 (universal time) and 5 data bytes.
     The local extra field has UTC/GMT modification/access times.
   - A subfield with ID 0x7875 (Unix UID/GID (any size)) and 11 data bytes:
-    01 04 e8 03 00 00 04 e8 03 00 00.
+    01 04 f5 01 00 00 04 14 00 00 00.
 
   There is no file comment.
 
 Central directory entry #95:
 ---------------------------
 
-  torchaudio/datasets/cmudict.py
+  torchaudio/_backend/
 
-  offset of local header from start of archive:   2081123
-                                                  (00000000001FC163h) bytes
+  offset of local header from start of archive:   185572
+                                                  (000000000002D4E4h) bytes
   file system or operating system of origin:      Unix
   version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
-  minimum software version required to extract:   2.0
-  compression method:                             deflated
-  compression sub-type (deflation):               maximum
+  minimum software version required to extract:   1.0
+  compression method:                             none (stored)
   file security status:                           not encrypted
   extended local header:                          no
-  file last modified on (DOS date/time):          2023 Mar 15 17:25:54
-  file last modified on (UT extra field modtime): 2023 Mar 16 00:25:54 local
-  file last modified on (UT extra field modtime): 2023 Mar 16 00:25:54 UTC
-  32-bit CRC value (hex):                         c75d27fa
-  compressed size:                                2034 bytes
-  uncompressed size:                              6408 bytes
-  length of filename:                             30 characters
+  file last modified on (DOS date/time):          2023 May 6 14:35:50
+  file last modified on (UT extra field modtime): 2023 May 6 18:35:50 local
+  file last modified on (UT extra field modtime): 2023 May 6 18:35:50 UTC
+  32-bit CRC value (hex):                         00000000
+  compressed size:                                0 bytes
+  uncompressed size:                              0 bytes
+  length of filename:                             20 characters
   length of extra field:                          24 bytes
   length of file comment:                         0 characters
   disk number on which file begins:               disk 1
-  apparent file type:                             text
-  Unix file attributes (100666 octal):            -rw-rw-rw-
-  MS-DOS file attributes (00 hex):                none
+  apparent file type:                             binary
+  Unix file attributes (040755 octal):            drwxr-xr-x
+  MS-DOS file attributes (10 hex):                dir 
 
   The central-directory extra field contains:
   - A subfield with ID 0x5455 (universal time) and 5 data bytes.
     The local extra field has UTC/GMT modification/access times.
   - A subfield with ID 0x7875 (Unix UID/GID (any size)) and 11 data bytes:
-    01 04 e8 03 00 00 04 e8 03 00 00.
+    01 04 f5 01 00 00 04 14 00 00 00.
 
   There is no file comment.
 
 Central directory entry #96:
 ---------------------------
 
-  torchaudio/datasets/cmuarctic.py
+  torchaudio/_backend/__init__.py
 
-  offset of local header from start of archive:   2083245
-                                                  (00000000001FC9ADh) bytes
+  offset of local header from start of archive:   185650
+                                                  (000000000002D532h) bytes
   file system or operating system of origin:      Unix
   version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               maximum
   file security status:                           not encrypted
   extended local header:                          no
-  file last modified on (DOS date/time):          2023 Mar 15 17:25:54
-  file last modified on (UT extra field modtime): 2023 Mar 16 00:25:54 local
-  file last modified on (UT extra field modtime): 2023 Mar 16 00:25:54 UTC
-  32-bit CRC value (hex):                         51c3f4cd
-  compressed size:                                2561 bytes
-  uncompressed size:                              7243 bytes
-  length of filename:                             32 characters
+  file last modified on (DOS date/time):          2023 May 4 22:38:58
+  file last modified on (UT extra field modtime): 2023 May 5 02:38:58 local
+  file last modified on (UT extra field modtime): 2023 May 5 02:38:58 UTC
+  32-bit CRC value (hex):                         078f5d09
+  compressed size:                                77 bytes
+  uncompressed size:                              140 bytes
+  length of filename:                             31 characters
   length of extra field:                          24 bytes
   length of file comment:                         0 characters
   disk number on which file begins:               disk 1
   apparent file type:                             text
   Unix file attributes (100666 octal):            -rw-rw-rw-
   MS-DOS file attributes (00 hex):                none
 
   The central-directory extra field contains:
   - A subfield with ID 0x5455 (universal time) and 5 data bytes.
     The local extra field has UTC/GMT modification/access times.
   - A subfield with ID 0x7875 (Unix UID/GID (any size)) and 11 data bytes:
-    01 04 e8 03 00 00 04 e8 03 00 00.
+    01 04 f5 01 00 00 04 14 00 00 00.
 
   There is no file comment.
 
 Central directory entry #97:
 ---------------------------
 
-  torchaudio/datasets/__init__.py
+  torchaudio/_backend/utils.py
 
-  offset of local header from start of archive:   2085896
-                                                  (00000000001FD408h) bytes
+  offset of local header from start of archive:   185816
+                                                  (000000000002D5D8h) bytes
   file system or operating system of origin:      Unix
   version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               maximum
   file security status:                           not encrypted
   extended local header:                          no
-  file last modified on (DOS date/time):          2023 Mar 15 17:25:54
-  file last modified on (UT extra field modtime): 2023 Mar 16 00:25:54 local
-  file last modified on (UT extra field modtime): 2023 Mar 16 00:25:54 UTC
-  32-bit CRC value (hex):                         55e7bc28
-  compressed size:                                434 bytes
-  uncompressed size:                              1138 bytes
-  length of filename:                             31 characters
+  file last modified on (DOS date/time):          2023 May 4 22:38:58
+  file last modified on (UT extra field modtime): 2023 May 5 02:38:58 local
+  file last modified on (UT extra field modtime): 2023 May 5 02:38:58 UTC
+  32-bit CRC value (hex):                         4f02fd99
+  compressed size:                                3827 bytes
+  uncompressed size:                              21101 bytes
+  length of filename:                             28 characters
   length of extra field:                          24 bytes
   length of file comment:                         0 characters
   disk number on which file begins:               disk 1
   apparent file type:                             text
   Unix file attributes (100666 octal):            -rw-rw-rw-
   MS-DOS file attributes (00 hex):                none
 
   The central-directory extra field contains:
   - A subfield with ID 0x5455 (universal time) and 5 data bytes.
     The local extra field has UTC/GMT modification/access times.
   - A subfield with ID 0x7875 (Unix UID/GID (any size)) and 11 data bytes:
-    01 04 e8 03 00 00 04 e8 03 00 00.
+    01 04 f5 01 00 00 04 14 00 00 00.
 
   There is no file comment.
 
 Central directory entry #98:
 ---------------------------
 
-  torchaudio/compliance/
+  torchaudio/transforms/
 
-  offset of local header from start of archive:   2086419
-                                                  (00000000001FD613h) bytes
+  offset of local header from start of archive:   189729
+                                                  (000000000002E521h) bytes
   file system or operating system of origin:      Unix
   version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   1.0
   compression method:                             none (stored)
   file security status:                           not encrypted
   extended local header:                          no
-  file last modified on (DOS date/time):          2023 Mar 15 10:54:56
-  file last modified on (UT extra field modtime): 2023 Mar 15 17:54:56 local
-  file last modified on (UT extra field modtime): 2023 Mar 15 17:54:56 UTC
+  file last modified on (DOS date/time):          2023 May 6 14:35:50
+  file last modified on (UT extra field modtime): 2023 May 6 18:35:50 local
+  file last modified on (UT extra field modtime): 2023 May 6 18:35:50 UTC
   32-bit CRC value (hex):                         00000000
   compressed size:                                0 bytes
   uncompressed size:                              0 bytes
   length of filename:                             22 characters
   length of extra field:                          24 bytes
   length of file comment:                         0 characters
   disk number on which file begins:               disk 1
@@ -3614,477 +3614,441 @@
   Unix file attributes (040755 octal):            drwxr-xr-x
   MS-DOS file attributes (10 hex):                dir 
 
   The central-directory extra field contains:
   - A subfield with ID 0x5455 (universal time) and 5 data bytes.
     The local extra field has UTC/GMT modification/access times.
   - A subfield with ID 0x7875 (Unix UID/GID (any size)) and 11 data bytes:
-    01 04 e8 03 00 00 04 e8 03 00 00.
+    01 04 f5 01 00 00 04 14 00 00 00.
 
   There is no file comment.
 
 Central directory entry #99:
 ---------------------------
 
-  torchaudio/compliance/kaldi.py
+  torchaudio/transforms/__init__.py
 
-  offset of local header from start of archive:   2086499
-                                                  (00000000001FD663h) bytes
+  offset of local header from start of archive:   189809
+                                                  (000000000002E571h) bytes
   file system or operating system of origin:      Unix
   version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               maximum
   file security status:                           not encrypted
   extended local header:                          no
-  file last modified on (DOS date/time):          2023 Mar 15 17:25:54
-  file last modified on (UT extra field modtime): 2023 Mar 16 00:25:54 local
-  file last modified on (UT extra field modtime): 2023 Mar 16 00:25:54 UTC
-  32-bit CRC value (hex):                         32dcccf8
-  compressed size:                                7678 bytes
-  uncompressed size:                              37479 bytes
-  length of filename:                             30 characters
+  file last modified on (DOS date/time):          2023 May 4 22:38:58
+  file last modified on (UT extra field modtime): 2023 May 5 02:38:58 local
+  file last modified on (UT extra field modtime): 2023 May 5 02:38:58 UTC
+  32-bit CRC value (hex):                         cb82ee15
+  compressed size:                                445 bytes
+  uncompressed size:                              1307 bytes
+  length of filename:                             33 characters
   length of extra field:                          24 bytes
   length of file comment:                         0 characters
   disk number on which file begins:               disk 1
   apparent file type:                             text
   Unix file attributes (100666 octal):            -rw-rw-rw-
   MS-DOS file attributes (00 hex):                none
 
   The central-directory extra field contains:
   - A subfield with ID 0x5455 (universal time) and 5 data bytes.
     The local extra field has UTC/GMT modification/access times.
   - A subfield with ID 0x7875 (Unix UID/GID (any size)) and 11 data bytes:
-    01 04 e8 03 00 00 04 e8 03 00 00.
+    01 04 f5 01 00 00 04 14 00 00 00.
 
   There is no file comment.
 
 Central directory entry #100:
 ---------------------------
 
-  torchaudio/compliance/__init__.py
+  torchaudio/transforms/_transforms.py
 
-  offset of local header from start of archive:   2094265
-                                                  (00000000001FF4B9h) bytes
+  offset of local header from start of archive:   190345
+                                                  (000000000002E789h) bytes
   file system or operating system of origin:      Unix
   version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               maximum
   file security status:                           not encrypted
   extended local header:                          no
-  file last modified on (DOS date/time):          2023 Mar 15 17:25:54
-  file last modified on (UT extra field modtime): 2023 Mar 16 00:25:54 local
-  file last modified on (UT extra field modtime): 2023 Mar 16 00:25:54 UTC
-  32-bit CRC value (hex):                         d8cb8be0
-  compressed size:                                50 bytes
-  uncompressed size:                              53 bytes
-  length of filename:                             33 characters
+  file last modified on (DOS date/time):          2023 May 4 22:38:58
+  file last modified on (UT extra field modtime): 2023 May 5 02:38:58 local
+  file last modified on (UT extra field modtime): 2023 May 5 02:38:58 UTC
+  32-bit CRC value (hex):                         eda92084
+  compressed size:                                15984 bytes
+  uncompressed size:                              86790 bytes
+  length of filename:                             36 characters
   length of extra field:                          24 bytes
   length of file comment:                         0 characters
   disk number on which file begins:               disk 1
   apparent file type:                             text
   Unix file attributes (100666 octal):            -rw-rw-rw-
   MS-DOS file attributes (00 hex):                none
 
   The central-directory extra field contains:
   - A subfield with ID 0x5455 (universal time) and 5 data bytes.
     The local extra field has UTC/GMT modification/access times.
   - A subfield with ID 0x7875 (Unix UID/GID (any size)) and 11 data bytes:
-    01 04 e8 03 00 00 04 e8 03 00 00.
+    01 04 f5 01 00 00 04 14 00 00 00.
 
   There is no file comment.
 
 Central directory entry #101:
 ---------------------------
 
-  torchaudio/backend/
+  torchaudio/transforms/_multi_channel.py
 
-  offset of local header from start of archive:   2094406
-                                                  (00000000001FF546h) bytes
+  offset of local header from start of archive:   206423
+                                                  (0000000000032657h) bytes
   file system or operating system of origin:      Unix
   version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
-  minimum software version required to extract:   1.0
-  compression method:                             none (stored)
+  minimum software version required to extract:   2.0
+  compression method:                             deflated
+  compression sub-type (deflation):               maximum
   file security status:                           not encrypted
   extended local header:                          no
-  file last modified on (DOS date/time):          2023 Mar 15 10:54:56
-  file last modified on (UT extra field modtime): 2023 Mar 15 17:54:56 local
-  file last modified on (UT extra field modtime): 2023 Mar 15 17:54:56 UTC
-  32-bit CRC value (hex):                         00000000
-  compressed size:                                0 bytes
-  uncompressed size:                              0 bytes
-  length of filename:                             19 characters
+  file last modified on (DOS date/time):          2023 May 4 22:38:58
+  file last modified on (UT extra field modtime): 2023 May 5 02:38:58 local
+  file last modified on (UT extra field modtime): 2023 May 5 02:38:58 UTC
+  32-bit CRC value (hex):                         626f7039
+  compressed size:                                3979 bytes
+  uncompressed size:                              22688 bytes
+  length of filename:                             39 characters
   length of extra field:                          24 bytes
   length of file comment:                         0 characters
   disk number on which file begins:               disk 1
-  apparent file type:                             binary
-  Unix file attributes (040755 octal):            drwxr-xr-x
-  MS-DOS file attributes (10 hex):                dir 
+  apparent file type:                             text
+  Unix file attributes (100666 octal):            -rw-rw-rw-
+  MS-DOS file attributes (00 hex):                none
 
   The central-directory extra field contains:
   - A subfield with ID 0x5455 (universal time) and 5 data bytes.
     The local extra field has UTC/GMT modification/access times.
   - A subfield with ID 0x7875 (Unix UID/GID (any size)) and 11 data bytes:
-    01 04 e8 03 00 00 04 e8 03 00 00.
+    01 04 f5 01 00 00 04 14 00 00 00.
 
   There is no file comment.
 
 Central directory entry #102:
 ---------------------------
 
-  torchaudio/backend/utils.py
+  torchaudio/lib/
 
-  offset of local header from start of archive:   2094483
-                                                  (00000000001FF593h) bytes
+  offset of local header from start of archive:   210499
+                                                  (0000000000033643h) bytes
   file system or operating system of origin:      Unix
   version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
-  minimum software version required to extract:   2.0
-  compression method:                             deflated
-  compression sub-type (deflation):               maximum
+  minimum software version required to extract:   1.0
+  compression method:                             none (stored)
   file security status:                           not encrypted
   extended local header:                          no
-  file last modified on (DOS date/time):          2023 Mar 15 17:25:54
-  file last modified on (UT extra field modtime): 2023 Mar 16 00:25:54 local
-  file last modified on (UT extra field modtime): 2023 Mar 16 00:25:54 UTC
-  32-bit CRC value (hex):                         2a3a0008
-  compressed size:                                949 bytes
-  uncompressed size:                              3000 bytes
-  length of filename:                             27 characters
+  file last modified on (DOS date/time):          2023 May 6 14:35:50
+  file last modified on (UT extra field modtime): 2023 May 6 18:35:50 local
+  file last modified on (UT extra field modtime): 2023 May 6 18:35:50 UTC
+  32-bit CRC value (hex):                         00000000
+  compressed size:                                0 bytes
+  uncompressed size:                              0 bytes
+  length of filename:                             15 characters
   length of extra field:                          24 bytes
   length of file comment:                         0 characters
   disk number on which file begins:               disk 1
-  apparent file type:                             text
-  Unix file attributes (100666 octal):            -rw-rw-rw-
-  MS-DOS file attributes (00 hex):                none
+  apparent file type:                             binary
+  Unix file attributes (040755 octal):            drwxr-xr-x
+  MS-DOS file attributes (10 hex):                dir 
 
   The central-directory extra field contains:
   - A subfield with ID 0x5455 (universal time) and 5 data bytes.
     The local extra field has UTC/GMT modification/access times.
   - A subfield with ID 0x7875 (Unix UID/GID (any size)) and 11 data bytes:
-    01 04 e8 03 00 00 04 e8 03 00 00.
+    01 04 f5 01 00 00 04 14 00 00 00.
 
   There is no file comment.
 
 Central directory entry #103:
 ---------------------------
 
-  torchaudio/backend/sox_io_backend.py
+  torchaudio/lib/libtorchaudio_ffmpeg.pyd
 
-  offset of local header from start of archive:   2095517
-                                                  (00000000001FF99Dh) bytes
+  offset of local header from start of archive:   210572
+                                                  (000000000003368Ch) bytes
   file system or operating system of origin:      Unix
   version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               maximum
   file security status:                           not encrypted
   extended local header:                          no
-  file last modified on (DOS date/time):          2023 Mar 15 17:25:54
-  file last modified on (UT extra field modtime): 2023 Mar 16 00:25:54 local
-  file last modified on (UT extra field modtime): 2023 Mar 16 00:25:54 UTC
-  32-bit CRC value (hex):                         68ce98ac
-  compressed size:                                4258 bytes
-  uncompressed size:                              17860 bytes
-  length of filename:                             36 characters
+  file last modified on (DOS date/time):          2023 May 4 22:42:12
+  file last modified on (UT extra field modtime): 2023 May 5 02:42:12 local
+  file last modified on (UT extra field modtime): 2023 May 5 02:42:12 UTC
+  32-bit CRC value (hex):                         eb7110fb
+  compressed size:                                312692 bytes
+  uncompressed size:                              1395712 bytes
+  length of filename:                             39 characters
   length of extra field:                          24 bytes
   length of file comment:                         0 characters
   disk number on which file begins:               disk 1
-  apparent file type:                             text
+  apparent file type:                             binary
   Unix file attributes (100666 octal):            -rw-rw-rw-
   MS-DOS file attributes (00 hex):                none
 
   The central-directory extra field contains:
   - A subfield with ID 0x5455 (universal time) and 5 data bytes.
     The local extra field has UTC/GMT modification/access times.
   - A subfield with ID 0x7875 (Unix UID/GID (any size)) and 11 data bytes:
-    01 04 e8 03 00 00 04 e8 03 00 00.
+    01 04 f5 01 00 00 04 14 00 00 00.
 
   There is no file comment.
 
 Central directory entry #104:
 ---------------------------
 
-  torchaudio/backend/soundfile_backend.py
+  torchaudio/lib/_torchaudio_ffmpeg.pyd
 
-  offset of local header from start of archive:   2099869
-                                                  (0000000000200A9Dh) bytes
+  offset of local header from start of archive:   523361
+                                                  (000000000007FC61h) bytes
   file system or operating system of origin:      Unix
   version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               maximum
   file security status:                           not encrypted
   extended local header:                          no
-  file last modified on (DOS date/time):          2023 Mar 15 17:25:54
-  file last modified on (UT extra field modtime): 2023 Mar 16 00:25:54 local
-  file last modified on (UT extra field modtime): 2023 Mar 16 00:25:54 UTC
-  32-bit CRC value (hex):                         122b9e90
-  compressed size:                                4821 bytes
-  uncompressed size:                              17617 bytes
-  length of filename:                             39 characters
+  file last modified on (DOS date/time):          2023 May 4 22:42:18
+  file last modified on (UT extra field modtime): 2023 May 5 02:42:18 local
+  file last modified on (UT extra field modtime): 2023 May 5 02:42:18 UTC
+  32-bit CRC value (hex):                         10557e9b
+  compressed size:                                269325 bytes
+  uncompressed size:                              1503744 bytes
+  length of filename:                             37 characters
   length of extra field:                          24 bytes
   length of file comment:                         0 characters
   disk number on which file begins:               disk 1
-  apparent file type:                             text
+  apparent file type:                             binary
   Unix file attributes (100666 octal):            -rw-rw-rw-
   MS-DOS file attributes (00 hex):                none
 
   The central-directory extra field contains:
   - A subfield with ID 0x5455 (universal time) and 5 data bytes.
     The local extra field has UTC/GMT modification/access times.
   - A subfield with ID 0x7875 (Unix UID/GID (any size)) and 11 data bytes:
-    01 04 e8 03 00 00 04 e8 03 00 00.
+    01 04 f5 01 00 00 04 14 00 00 00.
 
   There is no file comment.
 
 Central directory entry #105:
 ---------------------------
 
-  torchaudio/backend/no_backend.py
+  torchaudio/lib/libflashlight-text.pyd
 
-  offset of local header from start of archive:   2104787
-                                                  (0000000000201DD3h) bytes
+  offset of local header from start of archive:   792781
+                                                  (00000000000C18CDh) bytes
   file system or operating system of origin:      Unix
   version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               maximum
   file security status:                           not encrypted
   extended local header:                          no
-  file last modified on (DOS date/time):          2023 Mar 15 17:25:54
-  file last modified on (UT extra field modtime): 2023 Mar 16 00:25:54 local
-  file last modified on (UT extra field modtime): 2023 Mar 16 00:25:54 UTC
-  32-bit CRC value (hex):                         a08b056d
-  compressed size:                                314 bytes
-  uncompressed size:                              735 bytes
-  length of filename:                             32 characters
+  file last modified on (DOS date/time):          2023 May 4 22:41:46
+  file last modified on (UT extra field modtime): 2023 May 5 02:41:46 local
+  file last modified on (UT extra field modtime): 2023 May 5 02:41:46 UTC
+  32-bit CRC value (hex):                         7af52cbe
+  compressed size:                                366150 bytes
+  uncompressed size:                              1710592 bytes
+  length of filename:                             37 characters
   length of extra field:                          24 bytes
   length of file comment:                         0 characters
   disk number on which file begins:               disk 1
-  apparent file type:                             text
+  apparent file type:                             binary
   Unix file attributes (100666 octal):            -rw-rw-rw-
   MS-DOS file attributes (00 hex):                none
 
   The central-directory extra field contains:
   - A subfield with ID 0x5455 (universal time) and 5 data bytes.
     The local extra field has UTC/GMT modification/access times.
   - A subfield with ID 0x7875 (Unix UID/GID (any size)) and 11 data bytes:
-    01 04 e8 03 00 00 04 e8 03 00 00.
+    01 04 f5 01 00 00 04 14 00 00 00.
 
   There is no file comment.
 
 Central directory entry #106:
 ---------------------------
 
-  torchaudio/backend/common.py
+  torchaudio/lib/libtorchaudio.pyd
 
-  offset of local header from start of archive:   2105191
-                                                  (0000000000201F67h) bytes
+  offset of local header from start of archive:   1159026
+                                                  (000000000011AF72h) bytes
   file system or operating system of origin:      Unix
   version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               maximum
   file security status:                           not encrypted
   extended local header:                          no
-  file last modified on (DOS date/time):          2023 Mar 15 17:25:54
-  file last modified on (UT extra field modtime): 2023 Mar 16 00:25:54 local
-  file last modified on (UT extra field modtime): 2023 Mar 16 00:25:54 UTC
-  32-bit CRC value (hex):                         5db74cb2
-  compressed size:                                698 bytes
-  uncompressed size:                              1983 bytes
-  length of filename:                             28 characters
+  file last modified on (DOS date/time):          2023 May 4 22:41:44
+  file last modified on (UT extra field modtime): 2023 May 5 02:41:44 local
+  file last modified on (UT extra field modtime): 2023 May 5 02:41:44 UTC
+  32-bit CRC value (hex):                         9dd8fe77
+  compressed size:                                229781 bytes
+  uncompressed size:                              876032 bytes
+  length of filename:                             32 characters
   length of extra field:                          24 bytes
   length of file comment:                         0 characters
   disk number on which file begins:               disk 1
-  apparent file type:                             text
+  apparent file type:                             binary
   Unix file attributes (100666 octal):            -rw-rw-rw-
   MS-DOS file attributes (00 hex):                none
 
   The central-directory extra field contains:
   - A subfield with ID 0x5455 (universal time) and 5 data bytes.
     The local extra field has UTC/GMT modification/access times.
   - A subfield with ID 0x7875 (Unix UID/GID (any size)) and 11 data bytes:
-    01 04 e8 03 00 00 04 e8 03 00 00.
+    01 04 f5 01 00 00 04 14 00 00 00.
 
   There is no file comment.
 
 Central directory entry #107:
 ---------------------------
 
-  torchaudio/backend/__init__.py
+  torchaudio/lib/_torchaudio.pyd
 
-  offset of local header from start of archive:   2105975
-                                                  (0000000000202277h) bytes
+  offset of local header from start of archive:   1388897
+                                                  (0000000000153161h) bytes
   file system or operating system of origin:      Unix
   version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               maximum
   file security status:                           not encrypted
   extended local header:                          no
-  file last modified on (DOS date/time):          2023 Mar 15 17:25:54
-  file last modified on (UT extra field modtime): 2023 Mar 16 00:25:54 local
-  file last modified on (UT extra field modtime): 2023 Mar 16 00:25:54 UTC
-  32-bit CRC value (hex):                         1c6c735d
-  compressed size:                                190 bytes
-  uncompressed size:                              454 bytes
+  file last modified on (DOS date/time):          2023 May 4 22:41:52
+  file last modified on (UT extra field modtime): 2023 May 5 02:41:52 local
+  file last modified on (UT extra field modtime): 2023 May 5 02:41:52 UTC
+  32-bit CRC value (hex):                         81eec647
+  compressed size:                                172404 bytes
+  uncompressed size:                              788992 bytes
   length of filename:                             30 characters
   length of extra field:                          24 bytes
   length of file comment:                         0 characters
   disk number on which file begins:               disk 1
-  apparent file type:                             text
+  apparent file type:                             binary
   Unix file attributes (100666 octal):            -rw-rw-rw-
   MS-DOS file attributes (00 hex):                none
 
   The central-directory extra field contains:
   - A subfield with ID 0x5455 (universal time) and 5 data bytes.
     The local extra field has UTC/GMT modification/access times.
   - A subfield with ID 0x7875 (Unix UID/GID (any size)) and 11 data bytes:
-    01 04 e8 03 00 00 04 e8 03 00 00.
+    01 04 f5 01 00 00 04 14 00 00 00.
 
   There is no file comment.
 
 Central directory entry #108:
 ---------------------------
 
-  torchaudio/_internal/
-
-  offset of local header from start of archive:   2106253
-                                                  (000000000020238Dh) bytes
-  file system or operating system of origin:      Unix
-  version of encoding software:                   3.0
-  minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
-  minimum software version required to extract:   1.0
-  compression method:                             none (stored)
-  file security status:                           not encrypted
-  extended local header:                          no
-  file last modified on (DOS date/time):          2023 Mar 15 10:54:56
-  file last modified on (UT extra field modtime): 2023 Mar 15 17:54:56 local
-  file last modified on (UT extra field modtime): 2023 Mar 15 17:54:56 UTC
-  32-bit CRC value (hex):                         00000000
-  compressed size:                                0 bytes
-  uncompressed size:                              0 bytes
-  length of filename:                             21 characters
-  length of extra field:                          24 bytes
-  length of file comment:                         0 characters
-  disk number on which file begins:               disk 1
-  apparent file type:                             binary
-  Unix file attributes (040755 octal):            drwxr-xr-x
-  MS-DOS file attributes (10 hex):                dir 
-
-  The central-directory extra field contains:
-  - A subfield with ID 0x5455 (universal time) and 5 data bytes.
-    The local extra field has UTC/GMT modification/access times.
-  - A subfield with ID 0x7875 (Unix UID/GID (any size)) and 11 data bytes:
-    01 04 e8 03 00 00 04 e8 03 00 00.
-
-  There is no file comment.
-
-Central directory entry #109:
----------------------------
-
-  torchaudio/_internal/module_utils.py
+  torchaudio/lib/flashlight_lib_text_decoder.pyd
 
-  offset of local header from start of archive:   2106332
-                                                  (00000000002023DCh) bytes
+  offset of local header from start of archive:   1561389
+                                                  (000000000017D32Dh) bytes
   file system or operating system of origin:      Unix
   version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               maximum
   file security status:                           not encrypted
   extended local header:                          no
-  file last modified on (DOS date/time):          2023 Mar 15 17:25:54
-  file last modified on (UT extra field modtime): 2023 Mar 16 00:25:54 local
-  file last modified on (UT extra field modtime): 2023 Mar 16 00:25:54 UTC
-  32-bit CRC value (hex):                         32a076ff
-  compressed size:                                1042 bytes
-  uncompressed size:                              2694 bytes
-  length of filename:                             36 characters
+  file last modified on (DOS date/time):          2023 May 4 22:41:56
+  file last modified on (UT extra field modtime): 2023 May 5 02:41:56 local
+  file last modified on (UT extra field modtime): 2023 May 5 02:41:56 UTC
+  32-bit CRC value (hex):                         62b00972
+  compressed size:                                322438 bytes
+  uncompressed size:                              1828352 bytes
+  length of filename:                             46 characters
   length of extra field:                          24 bytes
   length of file comment:                         0 characters
   disk number on which file begins:               disk 1
-  apparent file type:                             text
+  apparent file type:                             binary
   Unix file attributes (100666 octal):            -rw-rw-rw-
   MS-DOS file attributes (00 hex):                none
 
   The central-directory extra field contains:
   - A subfield with ID 0x5455 (universal time) and 5 data bytes.
     The local extra field has UTC/GMT modification/access times.
   - A subfield with ID 0x7875 (Unix UID/GID (any size)) and 11 data bytes:
-    01 04 e8 03 00 00 04 e8 03 00 00.
+    01 04 f5 01 00 00 04 14 00 00 00.
 
   There is no file comment.
 
-Central directory entry #110:
+Central directory entry #109:
 ---------------------------
 
-  torchaudio/_internal/__init__.py
+  torchaudio/lib/flashlight_lib_text_dictionary.pyd
 
-  offset of local header from start of archive:   2107468
-                                                  (000000000020284Ch) bytes
+  offset of local header from start of archive:   1883931
+                                                  (00000000001CBF1Bh) bytes
   file system or operating system of origin:      Unix
   version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               maximum
   file security status:                           not encrypted
   extended local header:                          no
-  file last modified on (DOS date/time):          2023 Mar 15 17:25:54
-  file last modified on (UT extra field modtime): 2023 Mar 16 00:25:54 local
-  file last modified on (UT extra field modtime): 2023 Mar 16 00:25:54 UTC
-  32-bit CRC value (hex):                         55cc8166
-  compressed size:                                95 bytes
-  uncompressed size:                              152 bytes
-  length of filename:                             32 characters
+  file last modified on (DOS date/time):          2023 May 4 22:41:52
+  file last modified on (UT extra field modtime): 2023 May 5 02:41:52 local
+  file last modified on (UT extra field modtime): 2023 May 5 02:41:52 UTC
+  32-bit CRC value (hex):                         655f47c9
+  compressed size:                                189044 bytes
+  uncompressed size:                              1290752 bytes
+  length of filename:                             49 characters
   length of extra field:                          24 bytes
   length of file comment:                         0 characters
   disk number on which file begins:               disk 1
-  apparent file type:                             text
+  apparent file type:                             binary
   Unix file attributes (100666 octal):            -rw-rw-rw-
   MS-DOS file attributes (00 hex):                none
 
   The central-directory extra field contains:
   - A subfield with ID 0x5455 (universal time) and 5 data bytes.
     The local extra field has UTC/GMT modification/access times.
   - A subfield with ID 0x7875 (Unix UID/GID (any size)) and 11 data bytes:
-    01 04 e8 03 00 00 04 e8 03 00 00.
+    01 04 f5 01 00 00 04 14 00 00 00.
 
   There is no file comment.
 
-Central directory entry #111:
+Central directory entry #110:
 ---------------------------
 
   torchaudio/_extension/
 
-  offset of local header from start of archive:   2107653
-                                                  (0000000000202905h) bytes
+  offset of local header from start of archive:   2073082
+                                                  (00000000001FA1FAh) bytes
   file system or operating system of origin:      Unix
   version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   1.0
   compression method:                             none (stored)
   file security status:                           not encrypted
   extended local header:                          no
-  file last modified on (DOS date/time):          2023 Mar 15 10:54:56
-  file last modified on (UT extra field modtime): 2023 Mar 15 17:54:56 local
-  file last modified on (UT extra field modtime): 2023 Mar 15 17:54:56 UTC
+  file last modified on (DOS date/time):          2023 May 6 14:35:50
+  file last modified on (UT extra field modtime): 2023 May 6 18:35:50 local
+  file last modified on (UT extra field modtime): 2023 May 6 18:35:50 UTC
   32-bit CRC value (hex):                         00000000
   compressed size:                                0 bytes
   uncompressed size:                              0 bytes
   length of filename:                             22 characters
   length of extra field:                          24 bytes
   length of file comment:                         0 characters
   disk number on which file begins:               disk 1
@@ -4092,306 +4056,342 @@
   Unix file attributes (040755 octal):            drwxr-xr-x
   MS-DOS file attributes (10 hex):                dir 
 
   The central-directory extra field contains:
   - A subfield with ID 0x5455 (universal time) and 5 data bytes.
     The local extra field has UTC/GMT modification/access times.
   - A subfield with ID 0x7875 (Unix UID/GID (any size)) and 11 data bytes:
-    01 04 e8 03 00 00 04 e8 03 00 00.
+    01 04 f5 01 00 00 04 14 00 00 00.
 
   There is no file comment.
 
-Central directory entry #112:
+Central directory entry #111:
 ---------------------------
 
-  torchaudio/_extension/utils.py
+  torchaudio/_extension/__init__.py
 
-  offset of local header from start of archive:   2107733
-                                                  (0000000000202955h) bytes
+  offset of local header from start of archive:   2073162
+                                                  (00000000001FA24Ah) bytes
   file system or operating system of origin:      Unix
   version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               maximum
   file security status:                           not encrypted
   extended local header:                          no
-  file last modified on (DOS date/time):          2023 Mar 15 17:25:54
-  file last modified on (UT extra field modtime): 2023 Mar 16 00:25:54 local
-  file last modified on (UT extra field modtime): 2023 Mar 16 00:25:54 UTC
-  32-bit CRC value (hex):                         a2128a4e
-  compressed size:                                1992 bytes
-  uncompressed size:                              5458 bytes
-  length of filename:                             30 characters
+  file last modified on (DOS date/time):          2023 May 4 22:38:58
+  file last modified on (UT extra field modtime): 2023 May 5 02:38:58 local
+  file last modified on (UT extra field modtime): 2023 May 5 02:38:58 UTC
+  32-bit CRC value (hex):                         90590a14
+  compressed size:                                1298 bytes
+  uncompressed size:                              3500 bytes
+  length of filename:                             33 characters
   length of extra field:                          24 bytes
   length of file comment:                         0 characters
   disk number on which file begins:               disk 1
   apparent file type:                             text
   Unix file attributes (100666 octal):            -rw-rw-rw-
   MS-DOS file attributes (00 hex):                none
 
   The central-directory extra field contains:
   - A subfield with ID 0x5455 (universal time) and 5 data bytes.
     The local extra field has UTC/GMT modification/access times.
   - A subfield with ID 0x7875 (Unix UID/GID (any size)) and 11 data bytes:
-    01 04 e8 03 00 00 04 e8 03 00 00.
+    01 04 f5 01 00 00 04 14 00 00 00.
 
   There is no file comment.
 
-Central directory entry #113:
+Central directory entry #112:
 ---------------------------
 
-  torchaudio/_extension/__init__.py
+  torchaudio/_extension/utils.py
 
-  offset of local header from start of archive:   2109813
-                                                  (0000000000203175h) bytes
+  offset of local header from start of archive:   2074551
+                                                  (00000000001FA7B7h) bytes
   file system or operating system of origin:      Unix
   version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               maximum
   file security status:                           not encrypted
   extended local header:                          no
-  file last modified on (DOS date/time):          2023 Mar 15 17:25:54
-  file last modified on (UT extra field modtime): 2023 Mar 16 00:25:54 local
-  file last modified on (UT extra field modtime): 2023 Mar 16 00:25:54 UTC
-  32-bit CRC value (hex):                         90590a14
-  compressed size:                                1298 bytes
-  uncompressed size:                              3500 bytes
-  length of filename:                             33 characters
+  file last modified on (DOS date/time):          2023 May 4 22:38:58
+  file last modified on (UT extra field modtime): 2023 May 5 02:38:58 local
+  file last modified on (UT extra field modtime): 2023 May 5 02:38:58 UTC
+  32-bit CRC value (hex):                         a2128a4e
+  compressed size:                                1992 bytes
+  uncompressed size:                              5458 bytes
+  length of filename:                             30 characters
   length of extra field:                          24 bytes
   length of file comment:                         0 characters
   disk number on which file begins:               disk 1
   apparent file type:                             text
   Unix file attributes (100666 octal):            -rw-rw-rw-
   MS-DOS file attributes (00 hex):                none
 
   The central-directory extra field contains:
   - A subfield with ID 0x5455 (universal time) and 5 data bytes.
     The local extra field has UTC/GMT modification/access times.
   - A subfield with ID 0x7875 (Unix UID/GID (any size)) and 11 data bytes:
-    01 04 e8 03 00 00 04 e8 03 00 00.
+    01 04 f5 01 00 00 04 14 00 00 00.
 
   There is no file comment.
 
-Central directory entry #114:
+Central directory entry #113:
 ---------------------------
 
-  torchaudio/_backend/
+  torchaudio/sox_effects/
 
-  offset of local header from start of archive:   2111202
-                                                  (00000000002036E2h) bytes
+  offset of local header from start of archive:   2076631
+                                                  (00000000001FAFD7h) bytes
   file system or operating system of origin:      Unix
   version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   1.0
   compression method:                             none (stored)
   file security status:                           not encrypted
   extended local header:                          no
-  file last modified on (DOS date/time):          2023 Mar 15 10:54:56
-  file last modified on (UT extra field modtime): 2023 Mar 15 17:54:56 local
-  file last modified on (UT extra field modtime): 2023 Mar 15 17:54:56 UTC
+  file last modified on (DOS date/time):          2023 May 6 14:35:50
+  file last modified on (UT extra field modtime): 2023 May 6 18:35:50 local
+  file last modified on (UT extra field modtime): 2023 May 6 18:35:50 UTC
   32-bit CRC value (hex):                         00000000
   compressed size:                                0 bytes
   uncompressed size:                              0 bytes
-  length of filename:                             20 characters
+  length of filename:                             23 characters
   length of extra field:                          24 bytes
   length of file comment:                         0 characters
   disk number on which file begins:               disk 1
   apparent file type:                             binary
   Unix file attributes (040755 octal):            drwxr-xr-x
   MS-DOS file attributes (10 hex):                dir 
 
   The central-directory extra field contains:
   - A subfield with ID 0x5455 (universal time) and 5 data bytes.
     The local extra field has UTC/GMT modification/access times.
   - A subfield with ID 0x7875 (Unix UID/GID (any size)) and 11 data bytes:
-    01 04 e8 03 00 00 04 e8 03 00 00.
+    01 04 f5 01 00 00 04 14 00 00 00.
 
   There is no file comment.
 
-Central directory entry #115:
+Central directory entry #114:
 ---------------------------
 
-  torchaudio/_backend/utils.py
+  torchaudio/sox_effects/sox_effects.py
 
-  offset of local header from start of archive:   2111280
-                                                  (0000000000203730h) bytes
+  offset of local header from start of archive:   2076712
+                                                  (00000000001FB028h) bytes
   file system or operating system of origin:      Unix
   version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               maximum
   file security status:                           not encrypted
   extended local header:                          no
-  file last modified on (DOS date/time):          2023 Mar 15 17:25:54
-  file last modified on (UT extra field modtime): 2023 Mar 16 00:25:54 local
-  file last modified on (UT extra field modtime): 2023 Mar 16 00:25:54 UTC
-  32-bit CRC value (hex):                         4acbcc5a
-  compressed size:                                3812 bytes
-  uncompressed size:                              21065 bytes
-  length of filename:                             28 characters
+  file last modified on (DOS date/time):          2023 May 4 22:38:58
+  file last modified on (UT extra field modtime): 2023 May 5 02:38:58 local
+  file last modified on (UT extra field modtime): 2023 May 5 02:38:58 UTC
+  32-bit CRC value (hex):                         c45f60d0
+  compressed size:                                3569 bytes
+  uncompressed size:                              12461 bytes
+  length of filename:                             37 characters
   length of extra field:                          24 bytes
   length of file comment:                         0 characters
   disk number on which file begins:               disk 1
   apparent file type:                             text
   Unix file attributes (100666 octal):            -rw-rw-rw-
   MS-DOS file attributes (00 hex):                none
 
   The central-directory extra field contains:
   - A subfield with ID 0x5455 (universal time) and 5 data bytes.
     The local extra field has UTC/GMT modification/access times.
   - A subfield with ID 0x7875 (Unix UID/GID (any size)) and 11 data bytes:
-    01 04 e8 03 00 00 04 e8 03 00 00.
+    01 04 f5 01 00 00 04 14 00 00 00.
 
   There is no file comment.
 
-Central directory entry #116:
+Central directory entry #115:
 ---------------------------
 
-  torchaudio/_backend/__init__.py
+  torchaudio/sox_effects/__init__.py
 
-  offset of local header from start of archive:   2115178
-                                                  (000000000020466Ah) bytes
+  offset of local header from start of archive:   2080376
+                                                  (00000000001FBE78h) bytes
   file system or operating system of origin:      Unix
   version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               maximum
   file security status:                           not encrypted
   extended local header:                          no
-  file last modified on (DOS date/time):          2023 Mar 15 17:25:54
-  file last modified on (UT extra field modtime): 2023 Mar 16 00:25:54 local
-  file last modified on (UT extra field modtime): 2023 Mar 16 00:25:54 UTC
-  32-bit CRC value (hex):                         078f5d09
-  compressed size:                                77 bytes
-  uncompressed size:                              140 bytes
-  length of filename:                             31 characters
+  file last modified on (DOS date/time):          2023 May 4 22:38:58
+  file last modified on (UT extra field modtime): 2023 May 5 02:38:58 local
+  file last modified on (UT extra field modtime): 2023 May 5 02:38:58 UTC
+  32-bit CRC value (hex):                         d35c336b
+  compressed size:                                122 bytes
+  uncompressed size:                              272 bytes
+  length of filename:                             34 characters
   length of extra field:                          24 bytes
   length of file comment:                         0 characters
   disk number on which file begins:               disk 1
   apparent file type:                             text
   Unix file attributes (100666 octal):            -rw-rw-rw-
   MS-DOS file attributes (00 hex):                none
 
   The central-directory extra field contains:
   - A subfield with ID 0x5455 (universal time) and 5 data bytes.
     The local extra field has UTC/GMT modification/access times.
   - A subfield with ID 0x7875 (Unix UID/GID (any size)) and 11 data bytes:
-    01 04 e8 03 00 00 04 e8 03 00 00.
+    01 04 f5 01 00 00 04 14 00 00 00.
+
+  There is no file comment.
+
+Central directory entry #116:
+---------------------------
+
+  torchaudio/functional/
+
+  offset of local header from start of archive:   2080590
+                                                  (00000000001FBF4Eh) bytes
+  file system or operating system of origin:      Unix
+  version of encoding software:                   3.0
+  minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
+  minimum software version required to extract:   1.0
+  compression method:                             none (stored)
+  file security status:                           not encrypted
+  extended local header:                          no
+  file last modified on (DOS date/time):          2023 May 6 14:35:50
+  file last modified on (UT extra field modtime): 2023 May 6 18:35:50 local
+  file last modified on (UT extra field modtime): 2023 May 6 18:35:50 UTC
+  32-bit CRC value (hex):                         00000000
+  compressed size:                                0 bytes
+  uncompressed size:                              0 bytes
+  length of filename:                             22 characters
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
+    01 04 f5 01 00 00 04 14 00 00 00.
 
   There is no file comment.
 
 Central directory entry #117:
 ---------------------------
 
-  torchaudio/version.py
+  torchaudio/functional/filtering.py
 
-  offset of local header from start of archive:   2115344
-                                                  (0000000000204710h) bytes
+  offset of local header from start of archive:   2080670
+                                                  (00000000001FBF9Eh) bytes
   file system or operating system of origin:      Unix
   version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               maximum
   file security status:                           not encrypted
   extended local header:                          no
-  file last modified on (DOS date/time):          2023 Mar 15 17:28:20
-  file last modified on (UT extra field modtime): 2023 Mar 16 00:28:20 local
-  file last modified on (UT extra field modtime): 2023 Mar 16 00:28:20 UTC
-  32-bit CRC value (hex):                         47550a98
-  compressed size:                                77 bytes
-  uncompressed size:                              85 bytes
-  length of filename:                             21 characters
+  file last modified on (DOS date/time):          2023 May 4 22:38:58
+  file last modified on (UT extra field modtime): 2023 May 5 02:38:58 local
+  file last modified on (UT extra field modtime): 2023 May 5 02:38:58 UTC
+  32-bit CRC value (hex):                         a91bdce6
+  compressed size:                                12639 bytes
+  uncompressed size:                              63877 bytes
+  length of filename:                             34 characters
   length of extra field:                          24 bytes
   length of file comment:                         0 characters
   disk number on which file begins:               disk 1
   apparent file type:                             text
   Unix file attributes (100666 octal):            -rw-rw-rw-
   MS-DOS file attributes (00 hex):                none
 
   The central-directory extra field contains:
   - A subfield with ID 0x5455 (universal time) and 5 data bytes.
     The local extra field has UTC/GMT modification/access times.
   - A subfield with ID 0x7875 (Unix UID/GID (any size)) and 11 data bytes:
-    01 04 e8 03 00 00 04 e8 03 00 00.
+    01 04 f5 01 00 00 04 14 00 00 00.
 
   There is no file comment.
 
 Central directory entry #118:
 ---------------------------
 
-  torchaudio/kaldi_io.py
+  torchaudio/functional/__init__.py
 
-  offset of local header from start of archive:   2115500
-                                                  (00000000002047ACh) bytes
+  offset of local header from start of archive:   2093401
+                                                  (00000000001FF159h) bytes
   file system or operating system of origin:      Unix
   version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               maximum
   file security status:                           not encrypted
   extended local header:                          no
-  file last modified on (DOS date/time):          2023 Mar 15 17:25:54
-  file last modified on (UT extra field modtime): 2023 Mar 16 00:25:54 local
-  file last modified on (UT extra field modtime): 2023 Mar 16 00:25:54 UTC
-  32-bit CRC value (hex):                         982193e9
-  compressed size:                                1149 bytes
-  uncompressed size:                              5217 bytes
-  length of filename:                             22 characters
+  file last modified on (DOS date/time):          2023 May 4 22:38:58
+  file last modified on (UT extra field modtime): 2023 May 5 02:38:58 local
+  file last modified on (UT extra field modtime): 2023 May 5 02:38:58 UTC
+  32-bit CRC value (hex):                         16da4eff
+  compressed size:                                672 bytes
+  uncompressed size:                              2367 bytes
+  length of filename:                             33 characters
   length of extra field:                          24 bytes
   length of file comment:                         0 characters
   disk number on which file begins:               disk 1
   apparent file type:                             text
   Unix file attributes (100666 octal):            -rw-rw-rw-
   MS-DOS file attributes (00 hex):                none
 
   The central-directory extra field contains:
   - A subfield with ID 0x5455 (universal time) and 5 data bytes.
     The local extra field has UTC/GMT modification/access times.
   - A subfield with ID 0x7875 (Unix UID/GID (any size)) and 11 data bytes:
-    01 04 e8 03 00 00 04 e8 03 00 00.
+    01 04 f5 01 00 00 04 14 00 00 00.
 
   There is no file comment.
 
 Central directory entry #119:
 ---------------------------
 
-  torchaudio/__init__.py
+  torchaudio/functional/functional.py
 
-  offset of local header from start of archive:   2116729
-                                                  (0000000000204C79h) bytes
+  offset of local header from start of archive:   2094164
+                                                  (00000000001FF454h) bytes
   file system or operating system of origin:      Unix
   version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               maximum
   file security status:                           not encrypted
   extended local header:                          no
-  file last modified on (DOS date/time):          2023 Mar 15 17:25:54
-  file last modified on (UT extra field modtime): 2023 Mar 16 00:25:54 local
-  file last modified on (UT extra field modtime): 2023 Mar 16 00:25:54 UTC
-  32-bit CRC value (hex):                         e7b0eb74
-  compressed size:                                272 bytes
-  uncompressed size:                              672 bytes
-  length of filename:                             22 characters
+  file last modified on (DOS date/time):          2023 May 4 22:38:58
+  file last modified on (UT extra field modtime): 2023 May 5 02:38:58 local
+  file last modified on (UT extra field modtime): 2023 May 5 02:38:58 UTC
+  32-bit CRC value (hex):                         6a3e485d
+  compressed size:                                23219 bytes
+  uncompressed size:                              100038 bytes
+  length of filename:                             35 characters
   length of extra field:                          24 bytes
   length of file comment:                         0 characters
   disk number on which file begins:               disk 1
   apparent file type:                             text
   Unix file attributes (100666 octal):            -rw-rw-rw-
   MS-DOS file attributes (00 hex):                none
 
   The central-directory extra field contains:
   - A subfield with ID 0x5455 (universal time) and 5 data bytes.
     The local extra field has UTC/GMT modification/access times.
   - A subfield with ID 0x7875 (Unix UID/GID (any size)) and 11 data bytes:
-    01 04 e8 03 00 00 04 e8 03 00 00.
+    01 04 f5 01 00 00 04 14 00 00 00.
 
   There is no file comment.
```

## zipnote {}

```diff
@@ -1,358 +1,358 @@
-Filename: torchaudio-2.0.1.dist-info/
+Filename: torchaudio-2.0.2.dist-info/
 Comment: 
 
-Filename: torchaudio-2.0.1.dist-info/LICENSE
+Filename: torchaudio-2.0.2.dist-info/RECORD
 Comment: 
 
-Filename: torchaudio-2.0.1.dist-info/METADATA
+Filename: torchaudio-2.0.2.dist-info/LICENSE
 Comment: 
 
-Filename: torchaudio-2.0.1.dist-info/WHEEL
+Filename: torchaudio-2.0.2.dist-info/WHEEL
 Comment: 
 
-Filename: torchaudio-2.0.1.dist-info/top_level.txt
+Filename: torchaudio-2.0.2.dist-info/top_level.txt
 Comment: 
 
-Filename: torchaudio-2.0.1.dist-info/RECORD
+Filename: torchaudio-2.0.2.dist-info/METADATA
 Comment: 
 
 Filename: torchaudio/
 Comment: 
 
-Filename: torchaudio/utils/
+Filename: torchaudio/_internal/
 Comment: 
 
-Filename: torchaudio/utils/sox_utils.py
+Filename: torchaudio/_internal/__init__.py
 Comment: 
 
-Filename: torchaudio/utils/ffmpeg_utils.py
+Filename: torchaudio/_internal/module_utils.py
 Comment: 
 
-Filename: torchaudio/utils/download.py
+Filename: torchaudio/version.py
 Comment: 
 
-Filename: torchaudio/utils/__init__.py
+Filename: torchaudio/kaldi_io.py
 Comment: 
 
-Filename: torchaudio/transforms/
+Filename: torchaudio/datasets/
 Comment: 
 
-Filename: torchaudio/transforms/_transforms.py
+Filename: torchaudio/datasets/speechcommands.py
 Comment: 
 
-Filename: torchaudio/transforms/_multi_channel.py
+Filename: torchaudio/datasets/librilight_limited.py
 Comment: 
 
-Filename: torchaudio/transforms/__init__.py
+Filename: torchaudio/datasets/dr_vctk.py
 Comment: 
 
-Filename: torchaudio/sox_effects/
+Filename: torchaudio/datasets/cmudict.py
 Comment: 
 
-Filename: torchaudio/sox_effects/sox_effects.py
+Filename: torchaudio/datasets/gtzan.py
 Comment: 
 
-Filename: torchaudio/sox_effects/__init__.py
+Filename: torchaudio/datasets/cmuarctic.py
 Comment: 
 
-Filename: torchaudio/pipelines/
+Filename: torchaudio/datasets/musdb_hq.py
 Comment: 
 
-Filename: torchaudio/pipelines/_wav2vec2/
+Filename: torchaudio/datasets/snips.py
 Comment: 
 
-Filename: torchaudio/pipelines/_wav2vec2/utils.py
+Filename: torchaudio/datasets/commonvoice.py
 Comment: 
 
-Filename: torchaudio/pipelines/_wav2vec2/impl.py
+Filename: torchaudio/datasets/__init__.py
 Comment: 
 
-Filename: torchaudio/pipelines/_wav2vec2/__init__.py
+Filename: torchaudio/datasets/libritts.py
 Comment: 
 
-Filename: torchaudio/pipelines/_tts/
+Filename: torchaudio/datasets/voxceleb1.py
 Comment: 
 
-Filename: torchaudio/pipelines/_tts/utils.py
+Filename: torchaudio/datasets/tedlium.py
 Comment: 
 
-Filename: torchaudio/pipelines/_tts/interface.py
+Filename: torchaudio/datasets/utils.py
 Comment: 
 
-Filename: torchaudio/pipelines/_tts/impl.py
+Filename: torchaudio/datasets/ljspeech.py
 Comment: 
 
-Filename: torchaudio/pipelines/_tts/__init__.py
+Filename: torchaudio/datasets/yesno.py
 Comment: 
 
-Filename: torchaudio/pipelines/rnnt_pipeline.py
+Filename: torchaudio/datasets/fluentcommands.py
 Comment: 
 
-Filename: torchaudio/pipelines/_source_separation_pipeline.py
+Filename: torchaudio/datasets/librispeech.py
 Comment: 
 
-Filename: torchaudio/pipelines/__init__.py
+Filename: torchaudio/datasets/iemocap.py
 Comment: 
 
-Filename: torchaudio/models/
+Filename: torchaudio/datasets/librimix.py
 Comment: 
 
-Filename: torchaudio/models/wav2vec2/
+Filename: torchaudio/datasets/quesst14.py
 Comment: 
 
-Filename: torchaudio/models/wav2vec2/utils/
+Filename: torchaudio/datasets/vctk.py
 Comment: 
 
-Filename: torchaudio/models/wav2vec2/utils/import_huggingface.py
+Filename: torchaudio/io/
 Comment: 
 
-Filename: torchaudio/models/wav2vec2/utils/import_fairseq.py
+Filename: torchaudio/io/_playback.py
 Comment: 
 
-Filename: torchaudio/models/wav2vec2/utils/__init__.py
+Filename: torchaudio/io/__init__.py
 Comment: 
 
-Filename: torchaudio/models/wav2vec2/wavlm_attention.py
+Filename: torchaudio/io/_stream_reader.py
 Comment: 
 
-Filename: torchaudio/models/wav2vec2/model.py
+Filename: torchaudio/io/_compat.py
 Comment: 
 
-Filename: torchaudio/models/wav2vec2/components.py
+Filename: torchaudio/io/_stream_writer.py
 Comment: 
 
-Filename: torchaudio/models/wav2vec2/__init__.py
+Filename: torchaudio/__init__.py
 Comment: 
 
-Filename: torchaudio/models/decoder/
+Filename: torchaudio/pipelines/
 Comment: 
 
-Filename: torchaudio/models/decoder/_ctc_decoder.py
+Filename: torchaudio/pipelines/_source_separation_pipeline.py
 Comment: 
 
-Filename: torchaudio/models/decoder/__init__.py
+Filename: torchaudio/pipelines/_wav2vec2/
 Comment: 
 
-Filename: torchaudio/models/wavernn.py
+Filename: torchaudio/pipelines/_wav2vec2/__init__.py
 Comment: 
 
-Filename: torchaudio/models/wav2letter.py
+Filename: torchaudio/pipelines/_wav2vec2/utils.py
 Comment: 
 
-Filename: torchaudio/models/tacotron2.py
+Filename: torchaudio/pipelines/_wav2vec2/impl.py
 Comment: 
 
-Filename: torchaudio/models/rnnt_decoder.py
+Filename: torchaudio/pipelines/__init__.py
 Comment: 
 
-Filename: torchaudio/models/rnnt.py
+Filename: torchaudio/pipelines/_tts/
 Comment: 
 
-Filename: torchaudio/models/emformer.py
+Filename: torchaudio/pipelines/_tts/interface.py
 Comment: 
 
-Filename: torchaudio/models/deepspeech.py
+Filename: torchaudio/pipelines/_tts/__init__.py
 Comment: 
 
-Filename: torchaudio/models/conv_tasnet.py
+Filename: torchaudio/pipelines/_tts/utils.py
 Comment: 
 
-Filename: torchaudio/models/conformer.py
+Filename: torchaudio/pipelines/_tts/impl.py
 Comment: 
 
-Filename: torchaudio/models/_hdemucs.py
+Filename: torchaudio/pipelines/rnnt_pipeline.py
 Comment: 
 
-Filename: torchaudio/models/__init__.py
+Filename: torchaudio/utils/
 Comment: 
 
-Filename: torchaudio/lib/
+Filename: torchaudio/utils/download.py
 Comment: 
 
-Filename: torchaudio/lib/libtorchaudio_ffmpeg.pyd
+Filename: torchaudio/utils/__init__.py
 Comment: 
 
-Filename: torchaudio/lib/libtorchaudio.pyd
+Filename: torchaudio/utils/ffmpeg_utils.py
 Comment: 
 
-Filename: torchaudio/lib/libflashlight-text.pyd
+Filename: torchaudio/utils/sox_utils.py
 Comment: 
 
-Filename: torchaudio/lib/flashlight_lib_text_dictionary.pyd
+Filename: torchaudio/backend/
 Comment: 
 
-Filename: torchaudio/lib/flashlight_lib_text_decoder.pyd
+Filename: torchaudio/backend/__init__.py
 Comment: 
 
-Filename: torchaudio/lib/_torchaudio_ffmpeg.pyd
+Filename: torchaudio/backend/sox_io_backend.py
 Comment: 
 
-Filename: torchaudio/lib/_torchaudio.pyd
+Filename: torchaudio/backend/common.py
 Comment: 
 
-Filename: torchaudio/io/
+Filename: torchaudio/backend/utils.py
 Comment: 
 
-Filename: torchaudio/io/_stream_writer.py
+Filename: torchaudio/backend/no_backend.py
 Comment: 
 
-Filename: torchaudio/io/_stream_reader.py
+Filename: torchaudio/backend/soundfile_backend.py
 Comment: 
 
-Filename: torchaudio/io/_playback.py
+Filename: torchaudio/models/
 Comment: 
 
-Filename: torchaudio/io/_compat.py
+Filename: torchaudio/models/wav2letter.py
 Comment: 
 
-Filename: torchaudio/io/__init__.py
+Filename: torchaudio/models/emformer.py
 Comment: 
 
-Filename: torchaudio/functional/
+Filename: torchaudio/models/tacotron2.py
 Comment: 
 
-Filename: torchaudio/functional/functional.py
+Filename: torchaudio/models/conv_tasnet.py
 Comment: 
 
-Filename: torchaudio/functional/filtering.py
+Filename: torchaudio/models/decoder/
 Comment: 
 
-Filename: torchaudio/functional/__init__.py
+Filename: torchaudio/models/decoder/_ctc_decoder.py
 Comment: 
 
-Filename: torchaudio/datasets/
+Filename: torchaudio/models/decoder/__init__.py
 Comment: 
 
-Filename: torchaudio/datasets/yesno.py
+Filename: torchaudio/models/rnnt_decoder.py
 Comment: 
 
-Filename: torchaudio/datasets/voxceleb1.py
+Filename: torchaudio/models/__init__.py
 Comment: 
 
-Filename: torchaudio/datasets/vctk.py
+Filename: torchaudio/models/deepspeech.py
 Comment: 
 
-Filename: torchaudio/datasets/utils.py
+Filename: torchaudio/models/wav2vec2/
 Comment: 
 
-Filename: torchaudio/datasets/tedlium.py
+Filename: torchaudio/models/wav2vec2/wavlm_attention.py
 Comment: 
 
-Filename: torchaudio/datasets/speechcommands.py
+Filename: torchaudio/models/wav2vec2/__init__.py
 Comment: 
 
-Filename: torchaudio/datasets/snips.py
+Filename: torchaudio/models/wav2vec2/utils/
 Comment: 
 
-Filename: torchaudio/datasets/quesst14.py
+Filename: torchaudio/models/wav2vec2/utils/__init__.py
 Comment: 
 
-Filename: torchaudio/datasets/musdb_hq.py
+Filename: torchaudio/models/wav2vec2/utils/import_huggingface.py
 Comment: 
 
-Filename: torchaudio/datasets/ljspeech.py
+Filename: torchaudio/models/wav2vec2/utils/import_fairseq.py
 Comment: 
 
-Filename: torchaudio/datasets/libritts.py
+Filename: torchaudio/models/wav2vec2/model.py
 Comment: 
 
-Filename: torchaudio/datasets/librispeech.py
+Filename: torchaudio/models/wav2vec2/components.py
 Comment: 
 
-Filename: torchaudio/datasets/librimix.py
+Filename: torchaudio/models/_hdemucs.py
 Comment: 
 
-Filename: torchaudio/datasets/librilight_limited.py
+Filename: torchaudio/models/conformer.py
 Comment: 
 
-Filename: torchaudio/datasets/iemocap.py
+Filename: torchaudio/models/wavernn.py
 Comment: 
 
-Filename: torchaudio/datasets/gtzan.py
+Filename: torchaudio/models/rnnt.py
 Comment: 
 
-Filename: torchaudio/datasets/fluentcommands.py
+Filename: torchaudio/compliance/
 Comment: 
 
-Filename: torchaudio/datasets/dr_vctk.py
+Filename: torchaudio/compliance/__init__.py
 Comment: 
 
-Filename: torchaudio/datasets/commonvoice.py
+Filename: torchaudio/compliance/kaldi.py
 Comment: 
 
-Filename: torchaudio/datasets/cmudict.py
+Filename: torchaudio/_backend/
 Comment: 
 
-Filename: torchaudio/datasets/cmuarctic.py
+Filename: torchaudio/_backend/__init__.py
 Comment: 
 
-Filename: torchaudio/datasets/__init__.py
+Filename: torchaudio/_backend/utils.py
 Comment: 
 
-Filename: torchaudio/compliance/
+Filename: torchaudio/transforms/
 Comment: 
 
-Filename: torchaudio/compliance/kaldi.py
+Filename: torchaudio/transforms/__init__.py
 Comment: 
 
-Filename: torchaudio/compliance/__init__.py
+Filename: torchaudio/transforms/_transforms.py
 Comment: 
 
-Filename: torchaudio/backend/
+Filename: torchaudio/transforms/_multi_channel.py
 Comment: 
 
-Filename: torchaudio/backend/utils.py
+Filename: torchaudio/lib/
 Comment: 
 
-Filename: torchaudio/backend/sox_io_backend.py
+Filename: torchaudio/lib/libtorchaudio_ffmpeg.pyd
 Comment: 
 
-Filename: torchaudio/backend/soundfile_backend.py
+Filename: torchaudio/lib/_torchaudio_ffmpeg.pyd
 Comment: 
 
-Filename: torchaudio/backend/no_backend.py
+Filename: torchaudio/lib/libflashlight-text.pyd
 Comment: 
 
-Filename: torchaudio/backend/common.py
+Filename: torchaudio/lib/libtorchaudio.pyd
 Comment: 
 
-Filename: torchaudio/backend/__init__.py
+Filename: torchaudio/lib/_torchaudio.pyd
 Comment: 
 
-Filename: torchaudio/_internal/
+Filename: torchaudio/lib/flashlight_lib_text_decoder.pyd
 Comment: 
 
-Filename: torchaudio/_internal/module_utils.py
+Filename: torchaudio/lib/flashlight_lib_text_dictionary.pyd
 Comment: 
 
-Filename: torchaudio/_internal/__init__.py
+Filename: torchaudio/_extension/
 Comment: 
 
-Filename: torchaudio/_extension/
+Filename: torchaudio/_extension/__init__.py
 Comment: 
 
 Filename: torchaudio/_extension/utils.py
 Comment: 
 
-Filename: torchaudio/_extension/__init__.py
+Filename: torchaudio/sox_effects/
 Comment: 
 
-Filename: torchaudio/_backend/
+Filename: torchaudio/sox_effects/sox_effects.py
 Comment: 
 
-Filename: torchaudio/_backend/utils.py
+Filename: torchaudio/sox_effects/__init__.py
 Comment: 
 
-Filename: torchaudio/_backend/__init__.py
+Filename: torchaudio/functional/
 Comment: 
 
-Filename: torchaudio/version.py
+Filename: torchaudio/functional/filtering.py
 Comment: 
 
-Filename: torchaudio/kaldi_io.py
+Filename: torchaudio/functional/__init__.py
 Comment: 
 
-Filename: torchaudio/__init__.py
+Filename: torchaudio/functional/functional.py
 Comment: 
 
 Zip file comment:
```

## torchaudio/models/wav2vec2/wavlm_attention.py

```diff
@@ -69,14 +69,15 @@
             self.rel_attn_embed = nn.Embedding(num_buckets, num_heads)
         else:
             self.rel_attn_embed = None
 
         self.head_dim = embed_dim // num_heads
         assert self.head_dim * num_heads == self.embed_dim, "embed_dim must be divisible by num_heads"
 
+        self.dropout = dropout
         self.attention = nn.MultiheadAttention(embed_dim, num_heads, dropout=dropout, bias=bias, batch_first=True)
 
         self.gru_rel_pos = gru_rel_pos
         if self.gru_rel_pos:
             self.gru_rel_pos_linear = nn.Linear(self.head_dim, 8)
             self.gru_rel_pos_const = nn.Parameter(torch.ones(1, num_heads, 1, 1))
         self.has_position_bias = True
@@ -161,28 +162,53 @@
         """
         bsz, seq_len, embed_dim = query.size()
         assert embed_dim == self.embed_dim
         assert attention_mask is None
 
         if self.rel_attn_embed is not None and position_bias is None:
             position_bias = self.compute_bias(seq_len, seq_len)
-            position_bias = position_bias.unsqueeze(0).repeat(bsz, 1, 1, 1).view(bsz * self.num_heads, seq_len, seq_len)
+            position_bias = position_bias.unsqueeze(0).repeat(bsz, 1, 1, 1)
 
         attn_mask_rel_pos: Optional[Tensor] = None
         if position_bias is not None:
             attn_mask_rel_pos = position_bias
             if self.gru_rel_pos:  # Apply gating on relative position bias
                 query_layer = query.view(bsz, seq_len, self.num_heads, -1)
                 query_layer = query_layer.permute(0, 2, 1, 3)
 
                 gate_a, gate_b = torch.sigmoid(
                     self.gru_rel_pos_linear(query_layer).view(bsz, self.num_heads, seq_len, 2, 4).sum(-1, keepdim=False)
                 ).chunk(2, dim=-1)
                 gate_a_1 = gate_a * (gate_b * self.gru_rel_pos_const - 1.0) + 2.0
-                attn_mask_rel_pos = gate_a_1.view(bsz * self.num_heads, -1, 1) * position_bias
+                attn_mask_rel_pos = gate_a_1.view(bsz, self.num_heads, -1, 1) * position_bias
 
-            attn_mask_rel_pos = attn_mask_rel_pos.view((-1, seq_len, seq_len))
+            attn_mask_rel_pos = attn_mask_rel_pos.view((bsz, self.num_heads, seq_len, seq_len))
 
-        attn_output, _ = self.attention(
-            query, query, query, key_padding_mask=key_padding_mask, attn_mask=attn_mask_rel_pos, need_weights=False
+        if attn_mask_rel_pos is not None and key_padding_mask is not None:
+            key_padding_mask = key_padding_mask.view(bsz, 1, 1, seq_len).expand(-1, self.num_heads, -1, -1)
+            key_padding_mask = torch.nn.functional._canonical_mask(
+                mask=key_padding_mask,
+                mask_name="key_padding_mask",
+                other_type=torch.nn.functional._none_or_dtype(attn_mask_rel_pos),
+                other_name="",
+                target_type=query.dtype,
+            )
+        if attn_mask_rel_pos is not None and key_padding_mask is not None:
+            attn_mask_rel_pos = attn_mask_rel_pos + key_padding_mask
+        query_projected = torch.nn.functional.linear(query, self.attention.in_proj_weight, self.attention.in_proj_bias)
+        query, key, value = query_projected.chunk(3, -1)
+        shape = (bsz, seq_len, self.num_heads, self.head_dim)
+        query = query.view(shape).transpose(2, 1)  # (batch, num_heads, seq_len, head_dim)
+        key = key.view(shape).transpose(2, 1)  # (batch, num_heads, seq_len, head_dim)
+        value = value.view(shape).transpose(2, 1)  # (batch, num_heads, seq_len, head_dim)
+        dropout = self.dropout if self.training else 0.0
+        attn_output = torch.nn.functional.scaled_dot_product_attention(
+            query,
+            key,
+            value,
+            attn_mask=attn_mask_rel_pos,
+            dropout_p=dropout,
+            is_causal=False,
         )
+        attn_output = attn_output.transpose(1, 2).reshape(bsz, -1, self.num_heads * self.head_dim)
+        attn_output = self.attention.out_proj(attn_output)
         return attn_output, position_bias
```

## torchaudio/models/wav2vec2/components.py

```diff
@@ -258,15 +258,15 @@
         super().__init__()
         head_dim = embed_dim // num_heads
         if head_dim * num_heads != embed_dim:
             raise ValueError(f"`embed_dim ({embed_dim})` is not divisible by `num_heads ({num_heads})`")
 
         self.embed_dim = embed_dim
         self.num_heads = num_heads
-        self.dropout = torch.nn.Dropout(dropout)
+        self.dropout = dropout
         self.head_dim = head_dim
 
         self.scaling = self.head_dim**-0.5
 
         self.k_proj = nn.Linear(embed_dim, embed_dim, bias=True)
         self.v_proj = nn.Linear(embed_dim, embed_dim, bias=True)
         self.q_proj = nn.Linear(embed_dim, embed_dim, bias=True)
@@ -300,33 +300,22 @@
         if attention_mask is not None:
             shape_ = (batch_size, 1, length, length)
             if attention_mask.size() != shape_:
                 raise ValueError(f"The expected attention mask shape is {shape_}. " f"Found {attention_mask.size()}.")
 
         shape = (batch_size, length, self.num_heads, self.head_dim)
         q = self.q_proj(x).view(*shape).transpose(2, 1)  # B, nH, L, Hd
-        k = self.k_proj(x).view(*shape).permute(0, 2, 3, 1)  # B, nH, Hd, L
+        k = self.k_proj(x).view(*shape).transpose(2, 1)  # B, nH, L, Hd
         v = self.v_proj(x).view(*shape).transpose(2, 1)  # B, nH, L, Hd
-
-        # scale down q to avoid value overflow.
-        weights = (self.scaling * q) @ k  # B, nH, L, L
-        if attention_mask is not None:
-            weights += attention_mask
-        # subtracting a constant value from the tensor won't change the output of softmax.
-        # apply the subtraction to avoid value overflow in torch.nn.functional.softmax.
-        # for more details, please see Equation 7 in https://arxiv.org/abs/2112.08778
-        weights = weights - weights.max(dim=-1, keepdim=True)[0]
-
-        weights = torch.nn.functional.softmax(weights, dim=-1)
-        weights = self.dropout(weights)
-
-        output = weights @ v  # B, nH, L, Hd
-        output = output.transpose(2, 1).reshape(batch_size, length, embed_dim)
-
-        output = self.out_proj(output)
+        dropout = self.dropout if self.training else 0.0
+        attn_output = torch.nn.functional.scaled_dot_product_attention(
+            q, k, v, attn_mask=attention_mask, dropout_p=dropout, is_causal=False
+        )
+        attn_output = attn_output.transpose(1, 2).reshape(batch_size, -1, self.num_heads * self.head_dim)
+        output = self.out_proj(attn_output)
         return output, None  # Necessary for compatibility with WavLMSelAttention
 
 
 class FeedForward(Module):
     """Layer that follows attention layer in encoder layer."""
 
     def __init__(
```

## torchaudio/models/decoder/_ctc_decoder.py

```diff
@@ -265,14 +265,20 @@
                 self.blank,
                 unk_word,
                 transitions,
                 token_lm,
             )
         else:
             self.decoder = _LexiconFreeDecoder(decoder_options, lm, silence, self.blank, transitions)
+        # https://github.com/pytorch/audio/issues/3218
+        # If lm is passed like rvalue reference, the lm object gets garbage collected,
+        # and later call to the lm fails.
+        # This ensures that lm object is not deleted as long as the decoder is alive.
+        # https://github.com/pybind/pybind11/discussions/4013
+        self.lm = lm
 
     def _get_tokens(self, idxs: torch.IntTensor) -> torch.LongTensor:
         idxs = (g[0] for g in it.groupby(idxs))
         idxs = filter(lambda x: x != self.blank, idxs)
         return torch.LongTensor(list(idxs))
 
     def _get_timesteps(self, idxs: torch.IntTensor) -> torch.IntTensor:
```

## torchaudio/io/_compat.py

```diff
@@ -212,16 +212,19 @@
     sample_rate: int,
     channels_first: bool = True,
     format: Optional[str] = None,
     encoding: Optional[str] = None,
     bits_per_sample: Optional[int] = None,
     buffer_size: int = 4096,
 ) -> None:
-    if hasattr(uri, "write") and format is None:
-        raise RuntimeError("'format' is required when saving to file object.")
+    if hasattr(uri, "write"):
+        if format is None:
+            raise RuntimeError("'format' is required when saving to file object.")
+    else:
+        uri = os.path.normpath(uri)
     s = StreamWriter(uri, format=format, buffer_size=buffer_size)
     if format is None:
         tokens = str(uri).split(".")
         if len(tokens) > 1:
             format = tokens[-1].lower()
 
     if channels_first:
```

## torchaudio/_backend/utils.py

```diff
@@ -78,15 +78,15 @@
 
 class FFmpegBackend(Backend):
     @staticmethod
     def info(uri: Union[BinaryIO, str, os.PathLike], format: Optional[str], buffer_size: int = 4096) -> AudioMetaData:
         if hasattr(uri, "read"):
             metadata = info_audio_fileobj(uri, format, buffer_size=buffer_size)
         else:
-            metadata = info_audio(uri, format)
+            metadata = info_audio(os.path.normpath(uri), format)
         metadata.bits_per_sample = _get_bits_per_sample(metadata.encoding, metadata.bits_per_sample)
         metadata.encoding = _map_encoding(metadata.encoding)
         return metadata
 
     @staticmethod
     def load(
         uri: Union[BinaryIO, str, os.PathLike],
@@ -104,15 +104,15 @@
                 num_frames,
                 normalize,
                 channels_first,
                 format,
                 buffer_size,
             )
         else:
-            return load_audio(uri, frame_offset, num_frames, normalize, channels_first, format)
+            return load_audio(os.path.normpath(uri), frame_offset, num_frames, normalize, channels_first, format)
 
     @staticmethod
     def save(
         uri: Union[BinaryIO, str, os.PathLike],
         src: torch.Tensor,
         sample_rate: int,
         channels_first: bool = True,
```

## torchaudio/version.py

```diff
@@ -1,2 +1,2 @@
-__version__ = '2.0.1+cpu'
-git_version = 'd13d8db49d67d63ef1bcec4399cad73be81d3883'
+__version__ = '2.0.2+cpu'
+git_version = '31de77dad5c89274451b3f5c4bcb630be12787c4'
```

## Comparing `torchaudio-2.0.1.dist-info/LICENSE` & `torchaudio-2.0.2.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `torchaudio-2.0.1.dist-info/METADATA` & `torchaudio-2.0.2.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: torchaudio
-Version: 2.0.1
+Version: 2.0.2
 Summary: An audio package for PyTorch
 Home-page: https://github.com/pytorch/audio
 Author: Soumith Chintala, David Pollack, Sean Naren, Peter Goldsborough, Moto Hira, Caroline Chen, Jeff Hwang, Zhaoheng Ni, Xiaohui Zhang
 Author-email: soumith@pytorch.org
 Maintainer: Moto Hira, Caroline Chen, Jeff Hwang, Zhaoheng Ni, Xiaohui Zhang
 Maintainer-email: moto@meta.com
 Classifier: Environment :: Plugins
@@ -18,9 +18,9 @@
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Topic :: Multimedia :: Sound/Audio
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 License-File: LICENSE
-Requires-Dist: torch (==2.0.0)
+Requires-Dist: torch (==2.0.1)
```

## Comparing `torchaudio-2.0.1.dist-info/RECORD` & `torchaudio-2.0.2.dist-info/RECORD`

 * *Files 4% similar despite different names*

```diff
@@ -1,98 +1,98 @@
-torchaudio/utils/sox_utils.py,sha256=0v0XPyAL2S5wm1RWTv3LBQ-UMGPabWOXiawjFwrFNqI,2973
-torchaudio/utils/ffmpeg_utils.py,sha256=b03-Q8Gm86REZaERGyK60k5MeSkjJMFYfupNjdpR7AQ,8947
-torchaudio/utils/download.py,sha256=OHYPjZ0MB33tg2KVgF7y7yQanJWX3zD4UzSvhhtpzGk,2928
-torchaudio/utils/__init__.py,sha256=QHiAo-HbBsZZiSVnVjRyUQoziKeozSYw-3zT1wB0uiA,159
-torchaudio/transforms/_transforms.py,sha256=-qiRA0jxursXqq63lFxy69nQy9H-nj7I8R17L56kIAI,86790
-torchaudio/transforms/_multi_channel.py,sha256=Musw7dTu25HNjKeIcKHUDuqBmj_GC2e3TaakqJcffW8,22688
-torchaudio/transforms/__init__.py,sha256=M6UIZz0LJkcSYViuWQq7-YHZU62X6pRFxklkRXyMX0s,1307
-torchaudio/sox_effects/sox_effects.py,sha256=nlJbtu-oGvSdmEngei0NOzTepq_jCoqecBEIyh5wKkY,12461
-torchaudio/sox_effects/__init__.py,sha256=NVN6rAkHxizmOsZgLnxjMX5qXcPkABzLE-hvTMaSbEw,272
+torchaudio/_internal/__init__.py,sha256=aGpPV93R6RjNqDMmdhQ2WVxhKF2EZ9n2ep8yOP_I55c,152
+torchaudio/_internal/module_utils.py,sha256=xYW2Lmj9fVB8SiMNYQpAVzxuYyjjiVnmqZL3GqtCUyg,2694
+torchaudio/version.py,sha256=VF_fVA4zbhhnRcZhveRxDVmweqgXAhqK5L4x1J-1Ih0,85
+torchaudio/kaldi_io.py,sha256=acwysr6fASV9IcOTF0AbVPCo_VQTu1M2AOn1SXm3GPE,5217
+torchaudio/datasets/speechcommands.py,sha256=8W4jqj40ap5xXCT7COTYz_f9lw5OgGc1UzP2CnR-RAw,7653
+torchaudio/datasets/librilight_limited.py,sha256=J7RY6pA-QhJ-GIa9-b0awLrA-DRtqmKVXwWN_x5nICc,4279
+torchaudio/datasets/dr_vctk.py,sha256=7mDOK-09jnBf2sOljDVgnPL0F-N7G3SISSiNjoklW2k,4487
+torchaudio/datasets/cmudict.py,sha256=ubD25Yqwpp37K4gs0g0cIxvLksDny48FOaYjXTTEgUA,6408
+torchaudio/datasets/gtzan.py,sha256=6nQhXnXweenWWodfZOQswQY6Ah_9aIMC-QpRIZRIP9A,25464
+torchaudio/datasets/cmuarctic.py,sha256=Jratq2eolFQQ7Pc9igPSycmXRJJbJYL0n__I0ipJrmo,7243
+torchaudio/datasets/musdb_hq.py,sha256=V2X9w0LUZKvb1aneCJfz5yVdESxvpXloHOOTBzStyMs,5203
+torchaudio/datasets/snips.py,sha256=mwVc5KsbMlPQJ87eyYgjnQ5S4EFXoQvm13dO0rXpJuE,5165
+torchaudio/datasets/commonvoice.py,sha256=OcFn-nG4YfBIz0YIpH91xH9rFka8yFJmrxy4vFZkC4I,2849
+torchaudio/datasets/__init__.py,sha256=Eki3xOVwHz3wBEyF_XDMKzk32vEa_BG3I3pz93-GITI,1138
+torchaudio/datasets/libritts.py,sha256=VdY3zh0_YRoeeUMc9GJydzpuKm4scJXuuuMOuAif77g,6027
+torchaudio/datasets/voxceleb1.py,sha256=g-ZrF1jn-gDHNxvHqjQnSV4_wo884XC0wbvEoRjXC5E,12023
+torchaudio/datasets/tedlium.py,sha256=-Q-KZA0SYHpFd4piRC197-VpECEVgvBKBXNbEBFrl3Y,8905
+torchaudio/datasets/utils.py,sha256=I36gtJzUf9gg3WM5ktsK97pETA5556F4yRk8vogzDEo,1840
+torchaudio/datasets/ljspeech.py,sha256=qyrBoj_fXn0Etlk8cp_atrJOw4iQ7ndDoubRBL2qGRk,3590
+torchaudio/datasets/yesno.py,sha256=WUmJhCOQnxGL8Q0aKiCzbOA-ImG9GINxn1lfTmx2cGY,3104
+torchaudio/datasets/fluentcommands.py,sha256=KnmH1Y28k5PhqQX6eV-75MqwTRxiHSUUcvAsa-K954s,3353
+torchaudio/datasets/librispeech.py,sha256=piO22FodwtGEJLzaA29FH_NU4acYBobaCLiBRsjQx2k,6474
+torchaudio/datasets/iemocap.py,sha256=ZMMG_FpcWcMHEbhuRYRQaUWi_DoegjxCrnVyCg5EEVE,5077
+torchaudio/datasets/librimix.py,sha256=AncE671AOl04dRPsajNZW-ZxxI_PwA2sjBftdBg4Q-k,5249
+torchaudio/datasets/quesst14.py,sha256=VnpWGzTGukAcqsQcPSLk_ckbvM9EDTm2w95YjnwZemQ,4580
+torchaudio/datasets/vctk.py,sha256=Z8sUQ2YX7jZTRT1slSgI3jD5UyQ58c0cTsxD_K7_6Aw,5831
+torchaudio/io/_playback.py,sha256=aEP_MTX0Nsy5mGL7L_IZz-ihIwbgo-0lxH4KyMT5dnk,2391
+torchaudio/io/__init__.py,sha256=Ji8At6oLUPiu-5fHizPfVsyKd5F-wNMHF-jF3msGG44,200
+torchaudio/io/_stream_reader.py,sha256=AyjKqgINT-WCFTuU3HdBC9iVMCoO7lkX7hR_ltPFiyA,32378
+torchaudio/io/_compat.py,sha256=6KvM7q2ZQ6RiBzMsqFuZZKmQg_MBMhmvYPe3gb12tGM,8237
+torchaudio/io/_stream_writer.py,sha256=qcLEnJLoMxRP6WGzyEKfpssRivhCuGYiVMZ3fs1qW3s,12107
+torchaudio/__init__.py,sha256=Jzy7sPkE-vTk0SoP2DtTjEEhJn8AY1yag4evhcxHcaU,672
+torchaudio/pipelines/_source_separation_pipeline.py,sha256=WAjiWSlk73VS985GpKweDAfk2aKwQWI6jnGNwYHiRi8,4333
+torchaudio/pipelines/_wav2vec2/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 torchaudio/pipelines/_wav2vec2/utils.py,sha256=dR7lRlR8Mt9CHQESXrJ75vBeVGnXHRXBrrMrKf4-ycc,3094
 torchaudio/pipelines/_wav2vec2/impl.py,sha256=_oDgndwOybrTDT96c_8vX9yQR7LJ23KqJmw6sBpGTzI,61893
-torchaudio/pipelines/_wav2vec2/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
-torchaudio/pipelines/_tts/utils.py,sha256=ZqqD-TXI6zkKvYtdAHlZikKlpEO00otvOKJTTjXFOGI,4844
+torchaudio/pipelines/__init__.py,sha256=GHbAfWm0guJqU3Ma9opy_Aza4CSiqB3-DYjDiCJksXk,2554
 torchaudio/pipelines/_tts/interface.py,sha256=y1mU0446Vy2hHpCwMqRZt1UI4ZXl-C4tJp92EylwHh0,10479
-torchaudio/pipelines/_tts/impl.py,sha256=wwrTyTEEkew22AnzB_ZklapGaAstJSUBawhA7bOcGXM,15759
 torchaudio/pipelines/_tts/__init__.py,sha256=WKc5c06b_M9MvEohJZghJJWAL7vXvfwRIkdy85UCh04,442
+torchaudio/pipelines/_tts/utils.py,sha256=ZqqD-TXI6zkKvYtdAHlZikKlpEO00otvOKJTTjXFOGI,4844
+torchaudio/pipelines/_tts/impl.py,sha256=wwrTyTEEkew22AnzB_ZklapGaAstJSUBawhA7bOcGXM,15759
 torchaudio/pipelines/rnnt_pipeline.py,sha256=S0DLMPbt-lqNBWOcjG5KP2IfU1X_oTv95CVmSjxYJ2g,14129
-torchaudio/pipelines/_source_separation_pipeline.py,sha256=WAjiWSlk73VS985GpKweDAfk2aKwQWI6jnGNwYHiRi8,4333
-torchaudio/pipelines/__init__.py,sha256=GHbAfWm0guJqU3Ma9opy_Aza4CSiqB3-DYjDiCJksXk,2554
-torchaudio/models/wav2vec2/utils/import_huggingface.py,sha256=NMK6YrAIDfOw8j1tV-3XTwx_mwbJHvg8ldTrAWRztIM,6080
-torchaudio/models/wav2vec2/utils/import_fairseq.py,sha256=so7T-otDNCsTUtzJRUFFGWyd0caWl3RY_UbFMxJ4DJE,9411
-torchaudio/models/wav2vec2/utils/__init__.py,sha256=1eowaOEKRbp7JajFNv_r47REJqnMmXidukS7Mrwp_5Q,188
-torchaudio/models/wav2vec2/wavlm_attention.py,sha256=0zTpUkCQkHPniui_H04e3jLyhb3man8Pcx3DzukJ2_8,9588
-torchaudio/models/wav2vec2/model.py,sha256=kP6QKsF1PjleyUMhaPjydi0pCRy4GGUArRWBzfDJmdE,61671
-torchaudio/models/wav2vec2/components.py,sha256=SPH-igq6IZGLPlANQfZfJXmlQFaK8eRI7DBXLD26kL4,49074
-torchaudio/models/wav2vec2/__init__.py,sha256=j5FdQFfuIpdIKYwoMLop4Ba70GGoS-lK61tU-oNG5wg,972
-torchaudio/models/decoder/_ctc_decoder.py,sha256=zn373uARdE0CGi_CYU67xBlFSvryyyd4Uci_IRs4hfE,18544
-torchaudio/models/decoder/__init__.py,sha256=SLTOUXHeVE-7XsuE9JTVSCal71zBtjJOuGtUoTufUvs,783
-torchaudio/models/wavernn.py,sha256=LRgL36jA6WzI1PAzBY6P52oCMGSTOraXB8fEgkwpSxw,15855
+torchaudio/utils/download.py,sha256=OHYPjZ0MB33tg2KVgF7y7yQanJWX3zD4UzSvhhtpzGk,2928
+torchaudio/utils/__init__.py,sha256=QHiAo-HbBsZZiSVnVjRyUQoziKeozSYw-3zT1wB0uiA,159
+torchaudio/utils/ffmpeg_utils.py,sha256=b03-Q8Gm86REZaERGyK60k5MeSkjJMFYfupNjdpR7AQ,8947
+torchaudio/utils/sox_utils.py,sha256=0v0XPyAL2S5wm1RWTv3LBQ-UMGPabWOXiawjFwrFNqI,2973
+torchaudio/backend/__init__.py,sha256=TGcu75uVa3nflPuF_BjY42ZvlE6k4yIEqmm8-24Haf4,454
+torchaudio/backend/sox_io_backend.py,sha256=IorKlsHFvonzX7wxmfI5Spf3Kca-1BQSu4oVbV06A5c,17860
+torchaudio/backend/common.py,sha256=aEXV-dbO6oRKLSUKg2-LoNkvgN056yCVM9as3oRavjE,1983
+torchaudio/backend/utils.py,sha256=vFiGOKH8jMD3F3yXknQjGUP2RKnwsgSvHGLVWzkl-kk,3000
+torchaudio/backend/no_backend.py,sha256=ohVkGt5L51cm7Qz2ekvBQlYKd0aOCqTdBMQRwevZtDY,735
+torchaudio/backend/soundfile_backend.py,sha256=6h4IUOj1bJ5ciaYkMyO9GvrUT6PlB4VRfM43J9Gr4VQ,17617
 torchaudio/models/wav2letter.py,sha256=oetxpH5RG0TadYB75IOmYOrnraaPvSlcSNpRZb2FE_A,3350
+torchaudio/models/emformer.py,sha256=WbaeZcrPFOOLn4igqweE0AfuF_SQZpqg7XPGEhl7C8c,38650
 torchaudio/models/tacotron2.py,sha256=mZ5lLSa75oqc0hgkc3sIm5_gK-knhtgX3dmg9-oLQao,46960
+torchaudio/models/conv_tasnet.py,sha256=D7Y10sOzLe03gygfN1J5R73SIHkIGVQOkqKQ6Ni3o_s,12870
+torchaudio/models/decoder/_ctc_decoder.py,sha256=HAyoq2zMKjqSG8JOt8MLQ3-LhXkctWDMDYVfX-Vksxo,18903
+torchaudio/models/decoder/__init__.py,sha256=SLTOUXHeVE-7XsuE9JTVSCal71zBtjJOuGtUoTufUvs,783
 torchaudio/models/rnnt_decoder.py,sha256=Hdhn6lXel5W1p8iaAxDl9UuNewleNGQ_kFrD97FBwSA,13311
-torchaudio/models/rnnt.py,sha256=PNJpZd3vH6wRq8TEf4UlPtVHbte9wOJ-bRMEug6gp08,36357
-torchaudio/models/emformer.py,sha256=WbaeZcrPFOOLn4igqweE0AfuF_SQZpqg7XPGEhl7C8c,38650
+torchaudio/models/__init__.py,sha256=hINkW0J7YFykk27gpJFDMMqVH0nT6GWUz7a-3r9rALE,1733
 torchaudio/models/deepspeech.py,sha256=nVYc2xwWpFO6gu5CR0mbqLiAzJn8lAfHcdcP92i22mo,2830
-torchaudio/models/conv_tasnet.py,sha256=D7Y10sOzLe03gygfN1J5R73SIHkIGVQOkqKQ6Ni3o_s,12870
-torchaudio/models/conformer.py,sha256=gVrOYeJkPlVaX-4eZpVzNUe_r3k7g1Y6NaaQ8JZP-r4,10361
+torchaudio/models/wav2vec2/wavlm_attention.py,sha256=iYde9grsb_RaEs87FI5ykyN3z0Ix1plqpsMNvakAiWM,11058
+torchaudio/models/wav2vec2/__init__.py,sha256=j5FdQFfuIpdIKYwoMLop4Ba70GGoS-lK61tU-oNG5wg,972
+torchaudio/models/wav2vec2/utils/__init__.py,sha256=1eowaOEKRbp7JajFNv_r47REJqnMmXidukS7Mrwp_5Q,188
+torchaudio/models/wav2vec2/utils/import_huggingface.py,sha256=NMK6YrAIDfOw8j1tV-3XTwx_mwbJHvg8ldTrAWRztIM,6080
+torchaudio/models/wav2vec2/utils/import_fairseq.py,sha256=so7T-otDNCsTUtzJRUFFGWyd0caWl3RY_UbFMxJ4DJE,9411
+torchaudio/models/wav2vec2/model.py,sha256=kP6QKsF1PjleyUMhaPjydi0pCRy4GGUArRWBzfDJmdE,61671
+torchaudio/models/wav2vec2/components.py,sha256=GBM1VDKprce2LkyTefnXo9ZYGx-jb83duN-4ZeK24RQ,48631
 torchaudio/models/_hdemucs.py,sha256=ipAj7965PO_WEZqQwW1om9gQj90UhQOeU6HU3Lpvzwo,39250
-torchaudio/models/__init__.py,sha256=hINkW0J7YFykk27gpJFDMMqVH0nT6GWUz7a-3r9rALE,1733
-torchaudio/lib/libtorchaudio_ffmpeg.pyd,sha256=1ONeqsYQORGBWJS97cVlnsTYI-yv3EWDZgRYSWGSr7Y,1394688
-torchaudio/lib/libtorchaudio.pyd,sha256=RHeQ0qNJ5s0-m3jU_UGB7kkOxd40bST7P9oBh3LifXs,876032
-torchaudio/lib/libflashlight-text.pyd,sha256=JeMi4tUHR19OT_37latk2vItLa8pp3ykf4qIU10izVE,1710592
-torchaudio/lib/flashlight_lib_text_dictionary.pyd,sha256=-Xep3mfT-_oPFq8Z-qKmrEWFHxloi3NdLE8mKq5GKK8,1290752
-torchaudio/lib/flashlight_lib_text_decoder.pyd,sha256=KwIqfqPo8_yX9DquNUzwwDsAkfAZU0U14j77Fweekxg,1828352
-torchaudio/lib/_torchaudio_ffmpeg.pyd,sha256=CvsF1qeD36GSwAHwRUYAibXe5dDlVEkrqDcwb2OSMzg,1503744
-torchaudio/lib/_torchaudio.pyd,sha256=FqeTcZ03QCH_H-RvHFbTKWb_vpRKm6WY0lt7-yNgTv0,788992
-torchaudio/io/_stream_writer.py,sha256=qcLEnJLoMxRP6WGzyEKfpssRivhCuGYiVMZ3fs1qW3s,12107
-torchaudio/io/_stream_reader.py,sha256=AyjKqgINT-WCFTuU3HdBC9iVMCoO7lkX7hR_ltPFiyA,32378
-torchaudio/io/_playback.py,sha256=aEP_MTX0Nsy5mGL7L_IZz-ihIwbgo-0lxH4KyMT5dnk,2391
-torchaudio/io/_compat.py,sha256=KGkEnIaMMeX2QnVcylSS6f3gFk9JpeGZ1OnWV9R-sBI,8176
-torchaudio/io/__init__.py,sha256=Ji8At6oLUPiu-5fHizPfVsyKd5F-wNMHF-jF3msGG44,200
-torchaudio/functional/functional.py,sha256=pu29Ud1uC_wmVPz7evjfROZP8qXRD_KzCt_vk8JQPo4,100038
-torchaudio/functional/filtering.py,sha256=rKAR4xW1fpleK8ggrn3FgqtWlUyxOP2bRd-Vgn2bDfA,63877
-torchaudio/functional/__init__.py,sha256=oi6yA2aSswsGms6uWGt_wOtfhQScFkKqF9F4m6i_gUE,2367
-torchaudio/datasets/yesno.py,sha256=WUmJhCOQnxGL8Q0aKiCzbOA-ImG9GINxn1lfTmx2cGY,3104
-torchaudio/datasets/voxceleb1.py,sha256=g-ZrF1jn-gDHNxvHqjQnSV4_wo884XC0wbvEoRjXC5E,12023
-torchaudio/datasets/vctk.py,sha256=Z8sUQ2YX7jZTRT1slSgI3jD5UyQ58c0cTsxD_K7_6Aw,5831
-torchaudio/datasets/utils.py,sha256=I36gtJzUf9gg3WM5ktsK97pETA5556F4yRk8vogzDEo,1840
-torchaudio/datasets/tedlium.py,sha256=-Q-KZA0SYHpFd4piRC197-VpECEVgvBKBXNbEBFrl3Y,8905
-torchaudio/datasets/speechcommands.py,sha256=8W4jqj40ap5xXCT7COTYz_f9lw5OgGc1UzP2CnR-RAw,7653
-torchaudio/datasets/snips.py,sha256=mwVc5KsbMlPQJ87eyYgjnQ5S4EFXoQvm13dO0rXpJuE,5165
-torchaudio/datasets/quesst14.py,sha256=VnpWGzTGukAcqsQcPSLk_ckbvM9EDTm2w95YjnwZemQ,4580
-torchaudio/datasets/musdb_hq.py,sha256=V2X9w0LUZKvb1aneCJfz5yVdESxvpXloHOOTBzStyMs,5203
-torchaudio/datasets/ljspeech.py,sha256=qyrBoj_fXn0Etlk8cp_atrJOw4iQ7ndDoubRBL2qGRk,3590
-torchaudio/datasets/libritts.py,sha256=VdY3zh0_YRoeeUMc9GJydzpuKm4scJXuuuMOuAif77g,6027
-torchaudio/datasets/librispeech.py,sha256=piO22FodwtGEJLzaA29FH_NU4acYBobaCLiBRsjQx2k,6474
-torchaudio/datasets/librimix.py,sha256=AncE671AOl04dRPsajNZW-ZxxI_PwA2sjBftdBg4Q-k,5249
-torchaudio/datasets/librilight_limited.py,sha256=J7RY6pA-QhJ-GIa9-b0awLrA-DRtqmKVXwWN_x5nICc,4279
-torchaudio/datasets/iemocap.py,sha256=ZMMG_FpcWcMHEbhuRYRQaUWi_DoegjxCrnVyCg5EEVE,5077
-torchaudio/datasets/gtzan.py,sha256=6nQhXnXweenWWodfZOQswQY6Ah_9aIMC-QpRIZRIP9A,25464
-torchaudio/datasets/fluentcommands.py,sha256=KnmH1Y28k5PhqQX6eV-75MqwTRxiHSUUcvAsa-K954s,3353
-torchaudio/datasets/dr_vctk.py,sha256=7mDOK-09jnBf2sOljDVgnPL0F-N7G3SISSiNjoklW2k,4487
-torchaudio/datasets/commonvoice.py,sha256=OcFn-nG4YfBIz0YIpH91xH9rFka8yFJmrxy4vFZkC4I,2849
-torchaudio/datasets/cmudict.py,sha256=ubD25Yqwpp37K4gs0g0cIxvLksDny48FOaYjXTTEgUA,6408
-torchaudio/datasets/cmuarctic.py,sha256=Jratq2eolFQQ7Pc9igPSycmXRJJbJYL0n__I0ipJrmo,7243
-torchaudio/datasets/__init__.py,sha256=Eki3xOVwHz3wBEyF_XDMKzk32vEa_BG3I3pz93-GITI,1138
-torchaudio/compliance/kaldi.py,sha256=bS7qJgS3k8FK1RkMiNEoP3q0xhjeV_V4RHQ9jo_rqOM,37479
+torchaudio/models/conformer.py,sha256=gVrOYeJkPlVaX-4eZpVzNUe_r3k7g1Y6NaaQ8JZP-r4,10361
+torchaudio/models/wavernn.py,sha256=LRgL36jA6WzI1PAzBY6P52oCMGSTOraXB8fEgkwpSxw,15855
+torchaudio/models/rnnt.py,sha256=PNJpZd3vH6wRq8TEf4UlPtVHbte9wOJ-bRMEug6gp08,36357
 torchaudio/compliance/__init__.py,sha256=JNH_-dTQVmm55YwcVMuVvUYFWdXhGn4C__9S8IUsNoU,53
-torchaudio/backend/utils.py,sha256=vFiGOKH8jMD3F3yXknQjGUP2RKnwsgSvHGLVWzkl-kk,3000
-torchaudio/backend/sox_io_backend.py,sha256=IorKlsHFvonzX7wxmfI5Spf3Kca-1BQSu4oVbV06A5c,17860
-torchaudio/backend/soundfile_backend.py,sha256=6h4IUOj1bJ5ciaYkMyO9GvrUT6PlB4VRfM43J9Gr4VQ,17617
-torchaudio/backend/no_backend.py,sha256=ohVkGt5L51cm7Qz2ekvBQlYKd0aOCqTdBMQRwevZtDY,735
-torchaudio/backend/common.py,sha256=aEXV-dbO6oRKLSUKg2-LoNkvgN056yCVM9as3oRavjE,1983
-torchaudio/backend/__init__.py,sha256=TGcu75uVa3nflPuF_BjY42ZvlE6k4yIEqmm8-24Haf4,454
-torchaudio/_internal/module_utils.py,sha256=xYW2Lmj9fVB8SiMNYQpAVzxuYyjjiVnmqZL3GqtCUyg,2694
-torchaudio/_internal/__init__.py,sha256=aGpPV93R6RjNqDMmdhQ2WVxhKF2EZ9n2ep8yOP_I55c,152
-torchaudio/_extension/utils.py,sha256=5kPRC9r8n40e9GlTdJ3VE9kbH4HVlF6JiSl_haxz0Sw,5458
-torchaudio/_extension/__init__.py,sha256=S0TrqvIKsYl4Aqf7HKuPMRb0LJRmjAL5OmCW3NjKHTw,3500
-torchaudio/_backend/utils.py,sha256=b8AukNVA_k2vasTtAJKE63Xw-HgKoZ3AWtayNOQiCys,21065
+torchaudio/compliance/kaldi.py,sha256=bS7qJgS3k8FK1RkMiNEoP3q0xhjeV_V4RHQ9jo_rqOM,37479
 torchaudio/_backend/__init__.py,sha256=1sZ2vFkpseXe14VdMiCAC0nxi6JE_sC_MB5Ls5_L3uM,140
-torchaudio/version.py,sha256=729eTy3ASd8k-bOEVZcU_YW_JGfihv-E1icokTOrbx8,85
-torchaudio/kaldi_io.py,sha256=acwysr6fASV9IcOTF0AbVPCo_VQTu1M2AOn1SXm3GPE,5217
-torchaudio/__init__.py,sha256=Jzy7sPkE-vTk0SoP2DtTjEEhJn8AY1yag4evhcxHcaU,672
-torchaudio-2.0.1.dist-info/LICENSE,sha256=MmOOF5kxv-VR6r9nsOZ6E7SD4Wa1jdcmNjSrf4nzlvU,1363
-torchaudio-2.0.1.dist-info/METADATA,sha256=R_33nbNWa8s7xuCYbsB4ew8TVwg8xzZ3NLj5pM1FO5o,1198
-torchaudio-2.0.1.dist-info/WHEEL,sha256=J_4V_gB-O6Y7Pn6lk91K27JaIhI-q07YM5J8Ufzqla4,100
-torchaudio-2.0.1.dist-info/top_level.txt,sha256=mPKWMIRWWW2JwbJN6wRckeN1gpbjhifapAF0Z9t7SMo,11
-torchaudio-2.0.1.dist-info/RECORD,,
+torchaudio/_backend/utils.py,sha256=QyiNlGImhp7ZdW66Ozy-QNQSkaXx8hPrD77HaGuLfUs,21101
+torchaudio/transforms/__init__.py,sha256=M6UIZz0LJkcSYViuWQq7-YHZU62X6pRFxklkRXyMX0s,1307
+torchaudio/transforms/_transforms.py,sha256=-qiRA0jxursXqq63lFxy69nQy9H-nj7I8R17L56kIAI,86790
+torchaudio/transforms/_multi_channel.py,sha256=Musw7dTu25HNjKeIcKHUDuqBmj_GC2e3TaakqJcffW8,22688
+torchaudio/lib/libtorchaudio_ffmpeg.pyd,sha256=oy5GhpZWyvbTLu5pFgRglUHnwoEOMSv45mEtViyc2Wk,1395712
+torchaudio/lib/_torchaudio_ffmpeg.pyd,sha256=dL4FM3_EZGa2CwtbzlcrMj0o0cZQe9M4_tYWZNa4JY8,1503744
+torchaudio/lib/libflashlight-text.pyd,sha256=T4k8k8G93khNOxGH-wFzUZ91nbBR398K2bOu4D-SfwM,1710592
+torchaudio/lib/libtorchaudio.pyd,sha256=e5sOw88UN8xzFTvSuJpky6eBpugZG2OR-IhWuXyrB5Y,876032
+torchaudio/lib/_torchaudio.pyd,sha256=hbPcNIc7ZwRvWJZaL3nGaVk6d-TUkOsujSCh53mONNQ,788992
+torchaudio/lib/flashlight_lib_text_decoder.pyd,sha256=656VJh8LEZnwb9sBYWoHlUX3I4SHFzGxM50mu3CqovA,1828352
+torchaudio/lib/flashlight_lib_text_dictionary.pyd,sha256=5mm7MirPomAXJ0HLdP4Od7W4qitZuxuw8Aqj9qqkP5Q,1290752
+torchaudio/_extension/__init__.py,sha256=S0TrqvIKsYl4Aqf7HKuPMRb0LJRmjAL5OmCW3NjKHTw,3500
+torchaudio/_extension/utils.py,sha256=5kPRC9r8n40e9GlTdJ3VE9kbH4HVlF6JiSl_haxz0Sw,5458
+torchaudio/sox_effects/sox_effects.py,sha256=nlJbtu-oGvSdmEngei0NOzTepq_jCoqecBEIyh5wKkY,12461
+torchaudio/sox_effects/__init__.py,sha256=NVN6rAkHxizmOsZgLnxjMX5qXcPkABzLE-hvTMaSbEw,272
+torchaudio/functional/filtering.py,sha256=rKAR4xW1fpleK8ggrn3FgqtWlUyxOP2bRd-Vgn2bDfA,63877
+torchaudio/functional/__init__.py,sha256=oi6yA2aSswsGms6uWGt_wOtfhQScFkKqF9F4m6i_gUE,2367
+torchaudio/functional/functional.py,sha256=pu29Ud1uC_wmVPz7evjfROZP8qXRD_KzCt_vk8JQPo4,100038
+torchaudio-2.0.2.dist-info/RECORD,,
+torchaudio-2.0.2.dist-info/LICENSE,sha256=MmOOF5kxv-VR6r9nsOZ6E7SD4Wa1jdcmNjSrf4nzlvU,1363
+torchaudio-2.0.2.dist-info/WHEEL,sha256=J_4V_gB-O6Y7Pn6lk91K27JaIhI-q07YM5J8Ufzqla4,100
+torchaudio-2.0.2.dist-info/top_level.txt,sha256=mPKWMIRWWW2JwbJN6wRckeN1gpbjhifapAF0Z9t7SMo,11
+torchaudio-2.0.2.dist-info/METADATA,sha256=3fqkAqX7xvRrY0IR7S6-u88ZXeGrrc2LYKZ3g2nZNsI,1198
```

