# Comparing `tmp/arithmetica-py-1.0.185.tar.gz` & `tmp/arithmetica-py-1.0.186.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "arithmetica-py-1.0.185.tar", last modified: Fri Mar 31 11:46:07 2023, max compression
+gzip compressed data, was "arithmetica-py-1.0.186.tar", last modified: Mon May  8 21:56:02 2023, max compression
```

## Comparing `arithmetica-py-1.0.185.tar` & `arithmetica-py-1.0.186.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 11:46:07.112027 arithmetica-py-1.0.185/
--rw-r--r--   0 runner    (1001) docker     (123)    35823 2023-03-31 11:45:46.000000 arithmetica-py-1.0.185/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      208 2023-03-31 11:46:07.108027 arithmetica-py-1.0.185/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    10391 2023-03-31 11:45:46.000000 arithmetica-py-1.0.185/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 11:46:07.108027 arithmetica-py-1.0.185/arithmetica_py.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      208 2023-03-31 11:46:06.000000 arithmetica-py-1.0.185/arithmetica_py.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      315 2023-03-31 11:46:07.000000 arithmetica-py-1.0.185/arithmetica_py.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-31 11:46:06.000000 arithmetica-py-1.0.185/arithmetica_py.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       30 2023-03-31 11:46:06.000000 arithmetica-py-1.0.185/arithmetica_py.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-31 11:46:07.112027 arithmetica-py-1.0.185/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2635 2023-03-31 11:45:46.000000 arithmetica-py-1.0.185/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 11:46:07.108027 arithmetica-py-1.0.185/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 11:46:07.108027 arithmetica-py-1.0.185/src/python-module/
--rw-r--r--   0 runner    (1001) docker     (123)   166724 2023-03-31 11:46:06.000000 arithmetica-py-1.0.185/src/python-module/libarithmetica.a
--rw-r--r--   0 runner    (1001) docker     (123)    66430 2023-03-31 11:46:06.000000 arithmetica-py-1.0.185/src/python-module/libbasic_math_operations.a
--rw-r--r--   0 runner    (1001) docker     (123)    11654 2023-03-31 11:45:46.000000 arithmetica-py-1.0.185/src/python-module/module.c
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-03-31 11:46:06.000000 arithmetica-py-1.0.185/src/python-module/version.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 21:56:02.335936 arithmetica-py-1.0.186/
+-rw-r--r--   0 runner    (1001) docker     (123)    35823 2023-05-08 21:55:40.000000 arithmetica-py-1.0.186/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      208 2023-05-08 21:56:02.335936 arithmetica-py-1.0.186/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    10391 2023-05-08 21:55:40.000000 arithmetica-py-1.0.186/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 21:56:02.331936 arithmetica-py-1.0.186/arithmetica_py.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      208 2023-05-08 21:56:02.000000 arithmetica-py-1.0.186/arithmetica_py.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      315 2023-05-08 21:56:02.000000 arithmetica-py-1.0.186/arithmetica_py.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-08 21:56:02.000000 arithmetica-py-1.0.186/arithmetica_py.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       30 2023-05-08 21:56:02.000000 arithmetica-py-1.0.186/arithmetica_py.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-08 21:56:02.335936 arithmetica-py-1.0.186/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2635 2023-05-08 21:55:40.000000 arithmetica-py-1.0.186/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 21:56:02.331936 arithmetica-py-1.0.186/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 21:56:02.335936 arithmetica-py-1.0.186/src/python-module/
+-rw-r--r--   0 runner    (1001) docker     (123)   166980 2023-05-08 21:56:02.000000 arithmetica-py-1.0.186/src/python-module/libarithmetica.a
+-rw-r--r--   0 runner    (1001) docker     (123)    66430 2023-05-08 21:56:02.000000 arithmetica-py-1.0.186/src/python-module/libbasic_math_operations.a
+-rw-r--r--   0 runner    (1001) docker     (123)    11654 2023-05-08 21:55:40.000000 arithmetica-py-1.0.186/src/python-module/module.c
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-05-08 21:56:02.000000 arithmetica-py-1.0.186/src/python-module/version.txt
```

### Comparing `arithmetica-py-1.0.185/LICENSE` & `arithmetica-py-1.0.186/LICENSE`

 * *Files identical despite different names*

### Comparing `arithmetica-py-1.0.185/README.md` & `arithmetica-py-1.0.186/README.md`

 * *Files identical despite different names*

### Comparing `arithmetica-py-1.0.185/setup.py` & `arithmetica-py-1.0.186/setup.py`

 * *Files identical despite different names*

### Comparing `arithmetica-py-1.0.185/src/python-module/libarithmetica.a` & `arithmetica-py-1.0.186/src/python-module/libarithmetica.a`

 * *Files 0% similar despite different names*

#### nm -s {}

```diff
@@ -456,14 +456,16 @@
 0000000000000000 r .LC1
                  U calloc
                  U divide
                  U free
                  U igcd
                  U malloc
                  U memcpy
+                 U memmove
+                 U realloc
                  U strlen
 0000000000000000 T terminating_decimal_to_fraction
 
 Fraction.cpp.o:
 0000000000000003 r .LC10
 0000000000000000 r .LC4
 0000000000000000 r .LC9
```

#### file list

```diff
@@ -15,15 +15,15 @@
 ?rw-r--r--   0        0        0     3104 1970-01-01 00:00:00.000000 power.c.o
 ?rw-r--r--   0        0        0     2672 1970-01-01 00:00:00.000000 power_integer.c.o
 ?rw-r--r--   0        0        0     2672 1970-01-01 00:00:00.000000 repeating_decimal_to_fraction.c.o
 ?rw-r--r--   0        0        0    18192 1970-01-01 00:00:00.000000 simplify_arithmetic_expression.c.o
 ?rw-r--r--   0        0        0     4712 1970-01-01 00:00:00.000000 sine.c.o
 ?rw-r--r--   0        0        0     4736 1970-01-01 00:00:00.000000 square_root.c.o
 ?rw-r--r--   0        0        0     1808 1970-01-01 00:00:00.000000 tangent.c.o
-?rw-r--r--   0        0        0     2696 1970-01-01 00:00:00.000000 terminating_decimal_to_fraction.c.o
+?rw-r--r--   0        0        0     2952 1970-01-01 00:00:00.000000 terminating_decimal_to_fraction.c.o
 ?rw-r--r--   0        0        0    18288 1970-01-01 00:00:00.000000 Fraction.cpp.o
 ?rw-r--r--   0        0        0     1896 1970-01-01 00:00:00.000000 fraction.c.o
 ?rw-r--r--   0        0        0     2320 1970-01-01 00:00:00.000000 add_fraction.c.o
 ?rw-r--r--   0        0        0     1944 1970-01-01 00:00:00.000000 multiply_fraction.c.o
 ?rw-r--r--   0        0        0     3464 1970-01-01 00:00:00.000000 parse_fraction.c.o
 ?rw-r--r--   0        0        0     3704 1970-01-01 00:00:00.000000 power_fraction.c.o
 ?rw-r--r--   0        0        0     2736 1970-01-01 00:00:00.000000 simplify_parsed_fraction.c.o
```

#### terminating_decimal_to_fraction.c.o

##### readelf --wide --file-header {}

```diff
@@ -6,15 +6,15 @@
   OS/ABI:                            UNIX - System V
   ABI Version:                       0
   Type:                              REL (Relocatable file)
   Machine:                           Advanced Micro Devices X86-64
   Version:                           0x1
   Entry point address:               0x0
   Start of program headers:          0 (bytes into file)
-  Start of section headers:          1800 (bytes into file)
+  Start of section headers:          2056 (bytes into file)
   Flags:                             0x0
   Size of this header:               64 (bytes)
   Size of program headers:           0 (bytes)
   Number of program headers:         0
   Size of section headers:           64 (bytes)
   Number of section headers:         14
   Section header string table index: 13
```

##### readelf --wide --sections {}

```diff
@@ -1,23 +1,23 @@
-There are 14 section headers, starting at offset 0x708:
+There are 14 section headers, starting at offset 0x808:
 
 Section Headers:
   [Nr] Name              Type            Address          Off    Size   ES Flg Lk Inf Al
   [ 0]                   NULL            0000000000000000 000000 000000 00      0   0  0
-  [ 1] .text             PROGBITS        0000000000000000 000040 00025d 00  AX  0   0 16
-  [ 2] .rela.text        RELA            0000000000000000 000520 000150 18   I 11   1  8
-  [ 3] .data             PROGBITS        0000000000000000 00029d 000000 00  WA  0   0  1
-  [ 4] .bss              NOBITS          0000000000000000 00029d 000000 00  WA  0   0  1
-  [ 5] .rodata.cst16     PROGBITS        0000000000000000 0002a0 000010 10  AM  0   0 16
-  [ 6] .comment          PROGBITS        0000000000000000 0002b0 00002c 01  MS  0   0  1
-  [ 7] .note.GNU-stack   PROGBITS        0000000000000000 0002dc 000000 00      0   0  1
-  [ 8] .note.gnu.property NOTE            0000000000000000 0002e0 000020 00   A  0   0  8
-  [ 9] .eh_frame         PROGBITS        0000000000000000 000300 000068 00   A  0   0  8
-  [10] .rela.eh_frame    RELA            0000000000000000 000670 000018 18   I 11   9  8
-  [11] .symtab           SYMTAB          0000000000000000 000368 000138 18     12   5  8
-  [12] .strtab           STRTAB          0000000000000000 0004a0 00007a 00      0   0  1
-  [13] .shstrtab         STRTAB          0000000000000000 000688 00007a 00      0   0  1
+  [ 1] .text             PROGBITS        0000000000000000 000040 0002b5 00  AX  0   0 16
+  [ 2] .rela.text        RELA            0000000000000000 0005c0 0001b0 18   I 11   1  8
+  [ 3] .data             PROGBITS        0000000000000000 0002f5 000000 00  WA  0   0  1
+  [ 4] .bss              NOBITS          0000000000000000 0002f5 000000 00  WA  0   0  1
+  [ 5] .rodata.cst16     PROGBITS        0000000000000000 000300 000010 10  AM  0   0 16
+  [ 6] .comment          PROGBITS        0000000000000000 000310 00002c 01  MS  0   0  1
+  [ 7] .note.GNU-stack   PROGBITS        0000000000000000 00033c 000000 00      0   0  1
+  [ 8] .note.gnu.property NOTE            0000000000000000 000340 000020 00   A  0   0  8
+  [ 9] .eh_frame         PROGBITS        0000000000000000 000360 000068 00   A  0   0  8
+  [10] .rela.eh_frame    RELA            0000000000000000 000770 000018 18   I 11   9  8
+  [11] .symtab           SYMTAB          0000000000000000 0003c8 000168 18     12   5  8
+  [12] .strtab           STRTAB          0000000000000000 000530 00008a 00      0   0  1
+  [13] .shstrtab         STRTAB          0000000000000000 000788 00007a 00      0   0  1
 Key to Flags:
   W (write), A (alloc), X (execute), M (merge), S (strings), I (info),
   L (link order), O (extra OS processing required), G (group), T (TLS),
   C (compressed), x (unknown), o (OS specific), E (exclude),
   D (mbind), l (large), p (processor specific)
```

##### readelf --wide --symbols {}

```diff
@@ -1,16 +1,18 @@
 
-Symbol table '.symtab' contains 13 entries:
+Symbol table '.symtab' contains 15 entries:
    Num:    Value          Size Type    Bind   Vis      Ndx Name
      0: 0000000000000000     0 NOTYPE  LOCAL  DEFAULT  UND 
      1: 0000000000000000     0 FILE    LOCAL  DEFAULT  ABS terminating_decimal_to_fraction.c
      2: 0000000000000000     0 SECTION LOCAL  DEFAULT    1 .text
      3: 0000000000000000     0 NOTYPE  LOCAL  DEFAULT    5 .LC1
      4: 0000000000000000     0 NOTYPE  LOCAL  DEFAULT    5 .LC0
-     5: 0000000000000000   605 FUNC    GLOBAL DEFAULT    1 terminating_decimal_to_fraction
+     5: 0000000000000000   693 FUNC    GLOBAL DEFAULT    1 terminating_decimal_to_fraction
      6: 0000000000000000     0 NOTYPE  GLOBAL DEFAULT  UND strlen
      7: 0000000000000000     0 NOTYPE  GLOBAL DEFAULT  UND malloc
      8: 0000000000000000     0 NOTYPE  GLOBAL DEFAULT  UND calloc
      9: 0000000000000000     0 NOTYPE  GLOBAL DEFAULT  UND memcpy
     10: 0000000000000000     0 NOTYPE  GLOBAL DEFAULT  UND igcd
     11: 0000000000000000     0 NOTYPE  GLOBAL DEFAULT  UND divide
     12: 0000000000000000     0 NOTYPE  GLOBAL DEFAULT  UND free
+    13: 0000000000000000     0 NOTYPE  GLOBAL DEFAULT  UND realloc
+    14: 0000000000000000     0 NOTYPE  GLOBAL DEFAULT  UND memmove
```

##### readelf --wide --relocs {}

```diff
@@ -1,21 +1,25 @@
 
-Relocation section '.rela.text' at offset 0x520 contains 14 entries:
+Relocation section '.rela.text' at offset 0x5c0 contains 18 entries:
     Offset             Info             Type               Symbol's Value  Symbol's Name + Addend
-000000000000001f  0000000600000004 R_X86_64_PLT32         0000000000000000 strlen - 4
-0000000000000030  0000000700000004 R_X86_64_PLT32         0000000000000000 malloc - 4
-0000000000000040  0000000800000004 R_X86_64_PLT32         0000000000000000 calloc - 4
-0000000000000051  0000000900000004 R_X86_64_PLT32         0000000000000000 memcpy - 4
-00000000000000af  0000000600000004 R_X86_64_PLT32         0000000000000000 strlen - 4
-00000000000000ef  0000000400000002 R_X86_64_PC32          0000000000000000 .LC0 - 4
-000000000000013c  0000000300000002 R_X86_64_PC32          0000000000000000 .LC1 - 4
-00000000000001b6  0000000800000004 R_X86_64_PLT32         0000000000000000 calloc - 4
-00000000000001c7  0000000a00000004 R_X86_64_PLT32         0000000000000000 igcd - 4
-00000000000001d8  0000000b00000004 R_X86_64_PLT32         0000000000000000 divide - 4
-00000000000001e8  0000000b00000004 R_X86_64_PLT32         0000000000000000 divide - 4
-00000000000001f0  0000000c00000004 R_X86_64_PLT32         0000000000000000 free - 4
-00000000000001f8  0000000c00000004 R_X86_64_PLT32         0000000000000000 free - 4
-000000000000020e  0000000c00000004 R_X86_64_PLT32         0000000000000000 free - 4
+000000000000003c  0000000600000004 R_X86_64_PLT32         0000000000000000 strlen - 4
+000000000000004d  0000000700000004 R_X86_64_PLT32         0000000000000000 malloc - 4
+000000000000005d  0000000800000004 R_X86_64_PLT32         0000000000000000 calloc - 4
+000000000000006e  0000000900000004 R_X86_64_PLT32         0000000000000000 memcpy - 4
+00000000000000c9  0000000600000004 R_X86_64_PLT32         0000000000000000 strlen - 4
+0000000000000109  0000000400000002 R_X86_64_PC32          0000000000000000 .LC0 - 4
+0000000000000154  0000000300000002 R_X86_64_PC32          0000000000000000 .LC1 - 4
+00000000000001ce  0000000800000004 R_X86_64_PLT32         0000000000000000 calloc - 4
+00000000000001df  0000000a00000004 R_X86_64_PLT32         0000000000000000 igcd - 4
+00000000000001ef  0000000b00000004 R_X86_64_PLT32         0000000000000000 divide - 4
+0000000000000201  0000000b00000004 R_X86_64_PLT32         0000000000000000 divide - 4
+0000000000000211  0000000c00000004 R_X86_64_PLT32         0000000000000000 free - 4
+0000000000000219  0000000c00000004 R_X86_64_PLT32         0000000000000000 free - 4
+000000000000024c  0000000600000004 R_X86_64_PLT32         0000000000000000 strlen - 4
+0000000000000258  0000000d00000004 R_X86_64_PLT32         0000000000000000 realloc - 4
+0000000000000263  0000000600000004 R_X86_64_PLT32         0000000000000000 strlen - 4
+0000000000000274  0000000e00000004 R_X86_64_PLT32         0000000000000000 memmove - 4
+000000000000022f  0000000c00000004 R_X86_64_PLT32         0000000000000000 free - 4
 
-Relocation section '.rela.eh_frame' at offset 0x670 contains 1 entry:
+Relocation section '.rela.eh_frame' at offset 0x770 contains 1 entry:
     Offset             Info             Type               Symbol's Value  Symbol's Name + Addend
 0000000000000020  0000000200000002 R_X86_64_PC32          0000000000000000 .text + 0
```

##### readelf --wide --debug-dump=frames {}

```diff
@@ -9,50 +9,50 @@
   Return address column: 16
   Augmentation data:     1b
   DW_CFA_def_cfa: r7 (rsp) ofs 8
   DW_CFA_offset: r16 (rip) at cfa-8
   DW_CFA_nop
   DW_CFA_nop
 
-00000018 000000000000004c 0000001c FDE cie=00000000 pc=0000000000000000..000000000000025d
+00000018 000000000000004c 0000001c FDE cie=00000000 pc=0000000000000000..00000000000002b5
   DW_CFA_advance_loc: 6 to 0000000000000006
   DW_CFA_def_cfa_offset: 16
   DW_CFA_offset: r15 (r15) at cfa-16
-  DW_CFA_advance_loc: 5 to 000000000000000b
+  DW_CFA_advance_loc: 2 to 0000000000000008
   DW_CFA_def_cfa_offset: 24
   DW_CFA_offset: r14 (r14) at cfa-24
-  DW_CFA_advance_loc: 5 to 0000000000000010
+  DW_CFA_advance_loc: 2 to 000000000000000a
   DW_CFA_def_cfa_offset: 32
   DW_CFA_offset: r13 (r13) at cfa-32
-  DW_CFA_advance_loc: 2 to 0000000000000012
+  DW_CFA_advance_loc: 5 to 000000000000000f
   DW_CFA_def_cfa_offset: 40
   DW_CFA_offset: r12 (r12) at cfa-40
-  DW_CFA_advance_loc: 1 to 0000000000000013
+  DW_CFA_advance_loc: 4 to 0000000000000013
   DW_CFA_def_cfa_offset: 48
   DW_CFA_offset: r6 (rbp) at cfa-48
   DW_CFA_advance_loc: 1 to 0000000000000014
   DW_CFA_def_cfa_offset: 56
   DW_CFA_offset: r3 (rbx) at cfa-56
-  DW_CFA_advance_loc: 6 to 000000000000001a
-  DW_CFA_def_cfa_offset: 80
-  DW_CFA_advance_loc2: 486 to 0000000000000200
+  DW_CFA_advance_loc: 4 to 0000000000000018
+  DW_CFA_def_cfa_offset: 96
+  DW_CFA_advance_loc2: 521 to 0000000000000221
   DW_CFA_remember_state
   DW_CFA_def_cfa_offset: 56
-  DW_CFA_advance_loc: 4 to 0000000000000204
+  DW_CFA_advance_loc: 4 to 0000000000000225
   DW_CFA_def_cfa_offset: 48
-  DW_CFA_advance_loc: 1 to 0000000000000205
+  DW_CFA_advance_loc: 1 to 0000000000000226
   DW_CFA_def_cfa_offset: 40
-  DW_CFA_advance_loc: 2 to 0000000000000207
+  DW_CFA_advance_loc: 2 to 0000000000000228
   DW_CFA_def_cfa_offset: 32
-  DW_CFA_advance_loc: 2 to 0000000000000209
+  DW_CFA_advance_loc: 2 to 000000000000022a
   DW_CFA_def_cfa_offset: 24
-  DW_CFA_advance_loc: 2 to 000000000000020b
+  DW_CFA_advance_loc: 2 to 000000000000022c
   DW_CFA_def_cfa_offset: 16
-  DW_CFA_advance_loc: 2 to 000000000000020d
+  DW_CFA_advance_loc: 2 to 000000000000022e
   DW_CFA_def_cfa_offset: 8
-  DW_CFA_advance_loc: 11 to 0000000000000218
+  DW_CFA_advance_loc: 10 to 0000000000000238
   DW_CFA_restore_state
   DW_CFA_nop
   DW_CFA_nop
   DW_CFA_nop
   DW_CFA_nop
```

##### objdump --line-numbers --disassemble --demangle --reloc --no-show-raw-insn --section=.text {}

```diff
@@ -3,182 +3,210 @@
 
 Disassembly of section .text:
 
 0000000000000000 <terminating_decimal_to_fraction>:
 terminating_decimal_to_fraction():
 	endbr64
 	push   %r15
-	mov    %rdi,%r15
 	push   %r14
-	mov    %rdx,%r14
 	push   %r13
+	mov    %rdi,%r13
 	push   %r12
+	mov    %rsi,%r12
 	push   %rbp
 	push   %rbx
+	sub    $0x28,%rsp
+	cmpb   $0x2d,(%rdi)
+	mov    %rdx,0x10(%rsp)
+	movl   $0x0,0xc(%rsp)
+	jne    36 <terminating_decimal_to_fraction+0x36>
+	movl   $0x1,0xc(%rsp)
+	add    $0x1,%r13
+	mov    %r13,%rdi
 	xor    %ebx,%ebx
-	sub    $0x18,%rsp
-	mov    %rsi,(%rsp)
-	call   23 <terminating_decimal_to_fraction+0x23>
+	call   40 <terminating_decimal_to_fraction+0x40>
  R_X86_64_PLT32	strlen-0x4
-	lea    0x1(%rax),%r13
-	mov    %rax,0x8(%rsp)
-	mov    %r13,%rdi
-	call   34 <terminating_decimal_to_fraction+0x34>
+	lea    0x1(%rax),%r14
+	mov    %rax,0x18(%rsp)
+	mov    %r14,%rdi
+	call   51 <terminating_decimal_to_fraction+0x51>
  R_X86_64_PLT32	malloc-0x4
 	mov    $0x1,%esi
-	mov    %r13,%rdi
-	mov    %rax,%r12
-	call   44 <terminating_decimal_to_fraction+0x44>
+	mov    %r14,%rdi
+	mov    %rax,%r15
+	call   61 <terminating_decimal_to_fraction+0x61>
  R_X86_64_PLT32	calloc-0x4
-	mov    %r13,%rdx
-	mov    %r15,%rsi
-	mov    %r12,%rdi
+	mov    %r14,%rdx
+	mov    %r13,%rsi
+	mov    %r15,%rdi
 	mov    %rax,%rbp
-	call   55 <terminating_decimal_to_fraction+0x55>
+	call   72 <terminating_decimal_to_fraction+0x72>
  R_X86_64_PLT32	memcpy-0x4
-	mov    0x8(%rsp),%rcx
+	mov    0x18(%rsp),%r9
 	xor    %eax,%eax
 	xor    %edx,%edx
-	test   %rcx,%rcx
-	je     248 <terminating_decimal_to_fraction+0x248>
-	nopw   0x0(%rax,%rax,1)
-	cmpb   $0x2e,(%r15,%rax,1)
-	je     a2 <terminating_decimal_to_fraction+0xa2>
+	test   %r9,%r9
+	je     2a0 <terminating_decimal_to_fraction+0x2a0>
+	nopl   0x0(%rax)
+	cmpb   $0x2e,0x0(%r13,%rax,1)
+	je     bc <terminating_decimal_to_fraction+0xbc>
 	add    $0x1,%rax
-	cmp    %rax,%rcx
-	jbe    218 <terminating_decimal_to_fraction+0x218>
+	cmp    %rax,%r9
+	jbe    238 <terminating_decimal_to_fraction+0x238>
 	test   %dl,%dl
-	je     70 <terminating_decimal_to_fraction+0x70>
-	movzbl (%r12,%rax,1),%edx
+	je     88 <terminating_decimal_to_fraction+0x88>
+	movzbl (%r15,%rax,1),%edx
 	add    $0x1,%rbx
-	cmpb   $0x2e,(%r15,%rax,1)
-	mov    %dl,-0x1(%r12,%rax,1)
+	cmpb   $0x2e,0x0(%r13,%rax,1)
+	mov    %dl,-0x1(%r15,%rax,1)
 	mov    $0x1,%edx
-	jne    77 <terminating_decimal_to_fraction+0x77>
+	jne    90 <terminating_decimal_to_fraction+0x90>
 	add    $0x1,%rax
-	cmp    %rax,%rcx
-	ja     88 <terminating_decimal_to_fraction+0x88>
-	mov    %r12,%rdi
-	call   b3 <terminating_decimal_to_fraction+0xb3>
+	cmp    %rax,%r9
+	ja     a1 <terminating_decimal_to_fraction+0xa1>
+	mov    %r15,%rdi
+	call   cd <terminating_decimal_to_fraction+0xcd>
  R_X86_64_PLT32	strlen-0x4
-	movb   $0x0,-0x1(%r12,%rax,1)
+	movb   $0x0,-0x1(%r15,%rax,1)
 	movb   $0x31,0x0(%rbp)
 	test   %rbx,%rbx
-	je     1ad <terminating_decimal_to_fraction+0x1ad>
+	je     1c5 <terminating_decimal_to_fraction+0x1c5>
 	lea    -0x1(%rbx),%rax
 	cmp    $0xffffffffffffffff,%rbx
-	je     228 <terminating_decimal_to_fraction+0x228>
+	je     280 <terminating_decimal_to_fraction+0x280>
 	cmp    $0x6,%rax
-	jbe    228 <terminating_decimal_to_fraction+0x228>
+	jbe    280 <terminating_decimal_to_fraction+0x280>
 	mov    %rbx,%rcx
 	cmp    $0xe,%rax
-	jbe    251 <terminating_decimal_to_fraction+0x251>
+	jbe    2a9 <terminating_decimal_to_fraction+0x2a9>
 	movdqa 0x0(%rip),%xmm0        
  R_X86_64_PC32	.LC0-0x4
 	shr    $0x4,%rcx
 	xor    %eax,%eax
-	nopl   0x0(%rax)
+	nopl   0x0(%rax,%rax,1)
 	mov    %rax,%rdx
 	add    $0x1,%rax
 	shl    $0x4,%rdx
 	movups %xmm0,0x1(%rbp,%rdx,1)
 	cmp    %rax,%rcx
-	ja     100 <terminating_decimal_to_fraction+0x100>
+	ja     118 <terminating_decimal_to_fraction+0x118>
 	mov    %rbx,%rdx
 	and    $0xfffffffffffffff0,%rdx
 	lea    0x1(%rdx),%rax
 	cmp    %rdx,%rbx
-	je     1ad <terminating_decimal_to_fraction+0x1ad>
+	je     1c5 <terminating_decimal_to_fraction+0x1c5>
 	mov    %rbx,%rcx
 	sub    %rdx,%rcx
 	lea    -0x1(%rcx),%rsi
 	cmp    $0x6,%rsi
-	jbe    154 <terminating_decimal_to_fraction+0x154>
+	jbe    16c <terminating_decimal_to_fraction+0x16c>
 	mov    0x0(%rip),%rsi        
  R_X86_64_PC32	.LC1-0x4
 	mov    %rsi,0x1(%rbp,%rdx,1)
 	mov    %rcx,%rdx
 	and    $0xfffffffffffffff8,%rdx
 	add    %rdx,%rax
 	cmp    %rcx,%rdx
-	je     1ad <terminating_decimal_to_fraction+0x1ad>
+	je     1c5 <terminating_decimal_to_fraction+0x1c5>
 	lea    0x1(%rax),%rdx
 	movb   $0x30,0x0(%rbp,%rax,1)
 	cmp    %rdx,%rbx
-	jb     1ad <terminating_decimal_to_fraction+0x1ad>
+	jb     1c5 <terminating_decimal_to_fraction+0x1c5>
 	lea    0x2(%rax),%rdx
 	movb   $0x30,0x1(%rbp,%rax,1)
 	cmp    %rdx,%rbx
-	jb     1ad <terminating_decimal_to_fraction+0x1ad>
+	jb     1c5 <terminating_decimal_to_fraction+0x1c5>
 	lea    0x3(%rax),%rdx
 	movb   $0x30,0x2(%rbp,%rax,1)
 	cmp    %rdx,%rbx
-	jb     1ad <terminating_decimal_to_fraction+0x1ad>
+	jb     1c5 <terminating_decimal_to_fraction+0x1c5>
 	lea    0x4(%rax),%rdx
 	movb   $0x30,0x3(%rbp,%rax,1)
 	cmp    %rdx,%rbx
-	jb     1ad <terminating_decimal_to_fraction+0x1ad>
+	jb     1c5 <terminating_decimal_to_fraction+0x1c5>
 	lea    0x5(%rax),%rdx
 	movb   $0x30,0x4(%rbp,%rax,1)
 	cmp    %rdx,%rbx
-	jb     1ad <terminating_decimal_to_fraction+0x1ad>
+	jb     1c5 <terminating_decimal_to_fraction+0x1c5>
 	lea    0x6(%rax),%rdx
 	movb   $0x30,0x5(%rbp,%rax,1)
 	cmp    %rdx,%rbx
-	jb     1ad <terminating_decimal_to_fraction+0x1ad>
+	jb     1c5 <terminating_decimal_to_fraction+0x1c5>
 	movb   $0x30,0x6(%rbp,%rax,1)
-	mov    %r13,%rdi
 	mov    $0x1,%esi
-	call   1ba <terminating_decimal_to_fraction+0x1ba>
+	mov    %r14,%rdi
+	call   1d2 <terminating_decimal_to_fraction+0x1d2>
  R_X86_64_PLT32	calloc-0x4
 	mov    %rbp,%rsi
-	mov    %r12,%rdi
+	mov    %r15,%rdi
+	mov    %rax,%rbx
 	mov    %rax,%rdx
-	mov    %rax,%r15
-	call   1cb <terminating_decimal_to_fraction+0x1cb>
+	call   1e3 <terminating_decimal_to_fraction+0x1e3>
  R_X86_64_PLT32	igcd-0x4
-	mov    (%rsp),%rdx
-	mov    %r15,%rsi
-	mov    %r12,%rdi
 	xor    %ecx,%ecx
-	call   1dc <terminating_decimal_to_fraction+0x1dc>
+	mov    %r12,%rdx
+	mov    %rbx,%rsi
+	mov    %r15,%rdi
+	call   1f3 <terminating_decimal_to_fraction+0x1f3>
  R_X86_64_PLT32	divide-0x4
-	mov    %r14,%rdx
-	mov    %r15,%rsi
+	mov    0x10(%rsp),%rdx
 	xor    %ecx,%ecx
+	mov    %rbx,%rsi
 	mov    %rbp,%rdi
-	call   1ec <terminating_decimal_to_fraction+0x1ec>
+	call   205 <terminating_decimal_to_fraction+0x205>
  R_X86_64_PLT32	divide-0x4
-	mov    %r12,%rdi
-	call   1f4 <terminating_decimal_to_fraction+0x1f4>
+	mov    0xc(%rsp),%eax
+	test   %eax,%eax
+	jne    248 <terminating_decimal_to_fraction+0x248>
+	mov    %r15,%rdi
+	call   215 <terminating_decimal_to_fraction+0x215>
  R_X86_64_PLT32	free-0x4
 	mov    %rbp,%rdi
-	call   1fc <terminating_decimal_to_fraction+0x1fc>
+	call   21d <terminating_decimal_to_fraction+0x21d>
  R_X86_64_PLT32	free-0x4
-	add    $0x18,%rsp
-	mov    %r15,%rdi
+	add    $0x28,%rsp
+	mov    %rbx,%rdi
 	pop    %rbx
 	pop    %rbp
 	pop    %r12
 	pop    %r13
 	pop    %r14
 	pop    %r15
-	jmp    212 <terminating_decimal_to_fraction+0x212>
+	jmp    233 <terminating_decimal_to_fraction+0x233>
  R_X86_64_PLT32	free-0x4
-	nopw   0x0(%rax,%rax,1)
+	nopl   0x0(%rax,%rax,1)
 	test   %dl,%dl
-	je     b9 <terminating_decimal_to_fraction+0xb9>
-	jmp    ab <terminating_decimal_to_fraction+0xab>
+	je     d3 <terminating_decimal_to_fraction+0xd3>
+	jmp    c5 <terminating_decimal_to_fraction+0xc5>
 	nopl   (%rax)
+	mov    %r12,%rdi
+	call   250 <terminating_decimal_to_fraction+0x250>
+ R_X86_64_PLT32	strlen-0x4
+	mov    %r12,%rdi
+	lea    0x2(%rax),%rsi
+	call   25c <terminating_decimal_to_fraction+0x25c>
+ R_X86_64_PLT32	realloc-0x4
+	mov    %rax,%rdi
+	mov    %rax,%r12
+	call   267 <terminating_decimal_to_fraction+0x267>
+ R_X86_64_PLT32	strlen-0x4
+	lea    0x1(%r12),%rdi
+	mov    %r12,%rsi
+	lea    0x1(%rax),%rdx
+	call   278 <terminating_decimal_to_fraction+0x278>
+ R_X86_64_PLT32	memmove-0x4
+	movb   $0x2d,(%r12)
+	jmp    20d <terminating_decimal_to_fraction+0x20d>
+	nop
 	mov    $0x1,%eax
 	nopl   (%rax)
 	movb   $0x30,0x0(%rbp,%rax,1)
 	add    $0x1,%rax
 	cmp    %rax,%rbx
-	jae    230 <terminating_decimal_to_fraction+0x230>
-	jmp    1ad <terminating_decimal_to_fraction+0x1ad>
+	jae    288 <terminating_decimal_to_fraction+0x288>
+	jmp    1c5 <terminating_decimal_to_fraction+0x1c5>
 	nopl   0x0(%rax,%rax,1)
 	movb   $0x31,0x0(%rbp)
-	jmp    1ad <terminating_decimal_to_fraction+0x1ad>
+	jmp    1c5 <terminating_decimal_to_fraction+0x1c5>
 	xor    %edx,%edx
 	mov    $0x1,%eax
-	jmp    139 <terminating_decimal_to_fraction+0x139>
+	jmp    151 <terminating_decimal_to_fraction+0x151>
```

##### readelf --wide --decompress --hex-dump=.eh_frame {}

```diff
@@ -1,11 +1,11 @@
 
 Hex dump of section '.eh_frame':
  NOTE: This section has relocations against it, but these have NOT been applied to this dump.
   0x00000000 14000000 00000000 017a5200 01781001 .........zR..x..
   0x00000010 1b0c0708 90010000 4c000000 1c000000 ........L.......
-  0x00000020 00000000 5d020000 00460e10 8f02450e ....]....F....E.
-  0x00000030 188e0345 0e208d04 420e288c 05410e30 ...E. ..B.(..A.0
-  0x00000040 8606410e 38830746 0e5003e6 010a0e38 ..A.8..F.P.....8
+  0x00000020 00000000 b5020000 00460e10 8f02420e .........F....B.
+  0x00000030 188e0342 0e208d04 450e288c 05440e30 ...B. ..E.(..D.0
+  0x00000040 8606410e 38830744 0e600309 020a0e38 ..A.8..D.`.....8
   0x00000050 440e3041 0e28420e 20420e18 420e1042 D.0A.(B. B..B..B
-  0x00000060 0e084b0b 00000000                   ..K.....
+  0x00000060 0e084a0b 00000000                   ..J.....
```

##### readelf --wide --decompress --hex-dump=.strtab {}

```diff
@@ -3,9 +3,10 @@
   0x00000000 00746572 6d696e61 74696e67 5f646563 .terminating_dec
   0x00000010 696d616c 5f746f5f 66726163 74696f6e imal_to_fraction
   0x00000020 2e63002e 4c433100 2e4c4330 00746572 .c..LC1..LC0.ter
   0x00000030 6d696e61 74696e67 5f646563 696d616c minating_decimal
   0x00000040 5f746f5f 66726163 74696f6e 00737472 _to_fraction.str
   0x00000050 6c656e00 6d616c6c 6f630063 616c6c6f len.malloc.callo
   0x00000060 63006d65 6d637079 00696763 64006469 c.memcpy.igcd.di
-  0x00000070 76696465 00667265 6500              vide.free.
+  0x00000070 76696465 00667265 65007265 616c6c6f vide.free.reallo
+  0x00000080 63006d65 6d6d6f76 6500              c.memmove.
```

### Comparing `arithmetica-py-1.0.185/src/python-module/libbasic_math_operations.a` & `arithmetica-py-1.0.186/src/python-module/libbasic_math_operations.a`

 * *Files identical despite different names*

### Comparing `arithmetica-py-1.0.185/src/python-module/module.c` & `arithmetica-py-1.0.186/src/python-module/module.c`

 * *Files identical despite different names*

