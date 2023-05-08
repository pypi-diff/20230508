# Comparing `tmp/basic_math_operations-1.0.158.tar.gz` & `tmp/basic_math_operations-1.0.159.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "basic_math_operations-1.0.158.tar", last modified: Wed May  3 18:46:27 2023, max compression
+gzip compressed data, was "basic_math_operations-1.0.159.tar", last modified: Mon May  8 20:23:12 2023, max compression
```

## Comparing `basic_math_operations-1.0.158.tar` & `basic_math_operations-1.0.159.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 18:46:27.825268 basic_math_operations-1.0.158/
--rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-05-03 18:46:12.000000 basic_math_operations-1.0.158/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      195 2023-05-03 18:46:27.825268 basic_math_operations-1.0.158/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5233 2023-05-03 18:46:12.000000 basic_math_operations-1.0.158/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 18:46:27.825268 basic_math_operations-1.0.158/basic_math_operations.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      195 2023-05-03 18:46:27.000000 basic_math_operations-1.0.158/basic_math_operations.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      308 2023-05-03 18:46:27.000000 basic_math_operations-1.0.158/basic_math_operations.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-03 18:46:27.000000 basic_math_operations-1.0.158/basic_math_operations.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       40 2023-05-03 18:46:27.000000 basic_math_operations-1.0.158/basic_math_operations.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-03 18:46:27.829268 basic_math_operations-1.0.158/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2042 2023-05-03 18:46:12.000000 basic_math_operations-1.0.158/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 18:46:27.825268 basic_math_operations-1.0.158/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 18:46:27.825268 basic_math_operations-1.0.158/src/python-module/
--rw-r--r--   0 runner    (1001) docker     (123)    75056 2023-05-03 18:46:27.000000 basic_math_operations-1.0.158/src/python-module/libbasic_math_operations.a
--rw-r--r--   0 runner    (1001) docker     (123)     4166 2023-05-03 18:46:12.000000 basic_math_operations-1.0.158/src/python-module/module.c
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-05-03 18:46:27.000000 basic_math_operations-1.0.158/src/python-module/version.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 20:23:12.782687 basic_math_operations-1.0.159/
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-05-08 20:22:53.000000 basic_math_operations-1.0.159/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      195 2023-05-08 20:23:12.782687 basic_math_operations-1.0.159/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5233 2023-05-08 20:22:53.000000 basic_math_operations-1.0.159/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 20:23:12.778687 basic_math_operations-1.0.159/basic_math_operations.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      195 2023-05-08 20:23:12.000000 basic_math_operations-1.0.159/basic_math_operations.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      308 2023-05-08 20:23:12.000000 basic_math_operations-1.0.159/basic_math_operations.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-08 20:23:12.000000 basic_math_operations-1.0.159/basic_math_operations.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       40 2023-05-08 20:23:12.000000 basic_math_operations-1.0.159/basic_math_operations.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-08 20:23:12.782687 basic_math_operations-1.0.159/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2042 2023-05-08 20:22:53.000000 basic_math_operations-1.0.159/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 20:23:12.774687 basic_math_operations-1.0.159/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 20:23:12.782687 basic_math_operations-1.0.159/src/python-module/
+-rw-r--r--   0 runner    (1001) docker     (123)    75064 2023-05-08 20:23:12.000000 basic_math_operations-1.0.159/src/python-module/libbasic_math_operations.a
+-rw-r--r--   0 runner    (1001) docker     (123)     4166 2023-05-08 20:22:53.000000 basic_math_operations-1.0.159/src/python-module/module.c
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-05-08 20:23:12.000000 basic_math_operations-1.0.159/src/python-module/version.txt
```

### Comparing `basic_math_operations-1.0.158/LICENSE` & `basic_math_operations-1.0.159/LICENSE`

 * *Files identical despite different names*

### Comparing `basic_math_operations-1.0.158/README.md` & `basic_math_operations-1.0.159/README.md`

 * *Files identical despite different names*

### Comparing `basic_math_operations-1.0.158/setup.py` & `basic_math_operations-1.0.159/setup.py`

 * *Files identical despite different names*

### Comparing `basic_math_operations-1.0.158/src/python-module/libbasic_math_operations.a` & `basic_math_operations-1.0.159/src/python-module/libbasic_math_operations.a`

 * *Files 1% similar despite different names*

#### file list

```diff
@@ -12,15 +12,15 @@
 ?rw-r--r--   0        0        0     2528 1970-01-01 00:00:00.000000 subtractp.c.o
 ?rw-r--r--   0        0        0     1888 1970-01-01 00:00:00.000000 subtract.c.o
 ?rw-r--r--   0        0        0     1488 1970-01-01 00:00:00.000000 _multiply_whole.asm.o
 ?rw-r--r--   0        0        0     2552 1970-01-01 00:00:00.000000 multiplyp.c.o
 ?rw-r--r--   0        0        0     2016 1970-01-01 00:00:00.000000 multiply.c.o
 ?rw-r--r--   0        0        0     2880 1970-01-01 00:00:00.000000 _divide_whole_with_remainder.asm.o
 ?rw-r--r--   0        0        0     1936 1970-01-01 00:00:00.000000 divide_whole_with_remainder.c.o
-?rw-r--r--   0        0        0     2104 1970-01-01 00:00:00.000000 divide_whole.c.o
+?rw-r--r--   0        0        0     2112 1970-01-01 00:00:00.000000 divide_whole.c.o
 ?rw-r--r--   0        0        0     2192 1970-01-01 00:00:00.000000 dividep.c.o
 ?rw-r--r--   0        0        0     2024 1970-01-01 00:00:00.000000 divide.c.o
 ?rw-r--r--   0        0        0     1752 1970-01-01 00:00:00.000000 abs_mod.c.o
 ?rw-r--r--   0        0        0      688 1970-01-01 00:00:00.000000 asmalloc.asm.o
 ?rw-r--r--   0        0        0     1072 1970-01-01 00:00:00.000000 multiply_whole.asm.o
 ?rw-r--r--   0        0        0     2512 1970-01-01 00:00:00.000000 addp.c.o
 ?rw-r--r--   0        0        0     1824 1970-01-01 00:00:00.000000 remove_zeroes.c.o
```

#### divide_whole.c.o

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
-  Start of section headers:          1272 (bytes into file)
+  Start of section headers:          1280 (bytes into file)
   Flags:                             0x0
   Size of this header:               64 (bytes)
   Size of program headers:           0 (bytes)
   Number of program headers:         0
   Size of section headers:           64 (bytes)
   Number of section headers:         13
   Section header string table index: 12
```

##### readelf --wide --sections {}

```diff
@@ -1,22 +1,22 @@
-There are 13 section headers, starting at offset 0x4f8:
+There are 13 section headers, starting at offset 0x500:
 
 Section Headers:
   [Nr] Name              Type            Address          Off    Size   ES Flg Lk Inf Al
   [ 0]                   NULL            0000000000000000 000000 000000 00      0   0  0
-  [ 1] .text             PROGBITS        0000000000000000 000040 000105 00  AX  0   0 16
-  [ 2] .rela.text        RELA            0000000000000000 000368 000108 18   I 10   1  8
-  [ 3] .data             PROGBITS        0000000000000000 000145 000000 00  WA  0   0  1
-  [ 4] .bss              NOBITS          0000000000000000 000145 000000 00  WA  0   0  1
-  [ 5] .comment          PROGBITS        0000000000000000 000145 00002c 01  MS  0   0  1
-  [ 6] .note.GNU-stack   PROGBITS        0000000000000000 000171 000000 00      0   0  1
+  [ 1] .text             PROGBITS        0000000000000000 000040 000109 00  AX  0   0 16
+  [ 2] .rela.text        RELA            0000000000000000 000370 000108 18   I 10   1  8
+  [ 3] .data             PROGBITS        0000000000000000 000149 000000 00  WA  0   0  1
+  [ 4] .bss              NOBITS          0000000000000000 000149 000000 00  WA  0   0  1
+  [ 5] .comment          PROGBITS        0000000000000000 000149 00002c 01  MS  0   0  1
+  [ 6] .note.GNU-stack   PROGBITS        0000000000000000 000175 000000 00      0   0  1
   [ 7] .note.gnu.property NOTE            0000000000000000 000178 000020 00   A  0   0  8
-  [ 8] .eh_frame         PROGBITS        0000000000000000 000198 000060 00   A  0   0  8
-  [ 9] .rela.eh_frame    RELA            0000000000000000 000470 000018 18   I 10   8  8
-  [10] .symtab           SYMTAB          0000000000000000 0001f8 000108 18     11   3  8
-  [11] .strtab           STRTAB          0000000000000000 000300 000067 00      0   0  1
-  [12] .shstrtab         STRTAB          0000000000000000 000488 00006c 00      0   0  1
+  [ 8] .eh_frame         PROGBITS        0000000000000000 000198 000068 00   A  0   0  8
+  [ 9] .rela.eh_frame    RELA            0000000000000000 000478 000018 18   I 10   8  8
+  [10] .symtab           SYMTAB          0000000000000000 000200 000108 18     11   3  8
+  [11] .strtab           STRTAB          0000000000000000 000308 000067 00      0   0  1
+  [12] .shstrtab         STRTAB          0000000000000000 000490 00006c 00      0   0  1
 Key to Flags:
   W (write), A (alloc), X (execute), M (merge), S (strings), I (info),
   L (link order), O (extra OS processing required), G (group), T (TLS),
   C (compressed), x (unknown), o (OS specific), E (exclude),
   D (mbind), l (large), p (processor specific)
```

##### readelf --wide --symbols {}

```diff
@@ -1,14 +1,14 @@
 
 Symbol table '.symtab' contains 11 entries:
    Num:    Value          Size Type    Bind   Vis      Ndx Name
      0: 0000000000000000     0 NOTYPE  LOCAL  DEFAULT  UND 
      1: 0000000000000000     0 FILE    LOCAL  DEFAULT  ABS divide_whole.c
      2: 0000000000000000     0 SECTION LOCAL  DEFAULT    1 .text
-     3: 0000000000000000   261 FUNC    GLOBAL DEFAULT    1 divide_whole
+     3: 0000000000000000   265 FUNC    GLOBAL DEFAULT    1 divide_whole
      4: 0000000000000000     0 NOTYPE  GLOBAL DEFAULT  UND strlen_asm
      5: 0000000000000000     0 NOTYPE  GLOBAL DEFAULT  UND calloc
      6: 0000000000000000     0 NOTYPE  GLOBAL DEFAULT  UND memcpy
      7: 0000000000000000     0 NOTYPE  GLOBAL DEFAULT  UND memset
      8: 0000000000000000     0 NOTYPE  GLOBAL DEFAULT  UND _divide_whole_with_remainder
-     9: 0000000000000000     0 NOTYPE  GLOBAL DEFAULT  UND memmove
-    10: 0000000000000000     0 NOTYPE  GLOBAL DEFAULT  UND free
+     9: 0000000000000000     0 NOTYPE  GLOBAL DEFAULT  UND free
+    10: 0000000000000000     0 NOTYPE  GLOBAL DEFAULT  UND memmove
```

##### readelf --wide --relocs {}

```diff
@@ -1,18 +1,18 @@
 
-Relocation section '.rela.text' at offset 0x368 contains 11 entries:
+Relocation section '.rela.text' at offset 0x370 contains 11 entries:
     Offset             Info             Type               Symbol's Value  Symbol's Name + Addend
 0000000000000021  0000000400000004 R_X86_64_PLT32         0000000000000000 strlen_asm - 4
 000000000000002c  0000000400000004 R_X86_64_PLT32         0000000000000000 strlen_asm - 4
 0000000000000045  0000000500000004 R_X86_64_PLT32         0000000000000000 calloc - 4
 000000000000005d  0000000600000004 R_X86_64_PLT32         0000000000000000 memcpy - 4
-0000000000000074  0000000700000004 R_X86_64_PLT32         0000000000000000 memset - 4
+0000000000000075  0000000700000004 R_X86_64_PLT32         0000000000000000 memset - 4
 0000000000000099  0000000500000004 R_X86_64_PLT32         0000000000000000 calloc - 4
 00000000000000b1  0000000800000004 R_X86_64_PLT32         0000000000000000 _divide_whole_with_remainder - 4
-00000000000000b9  0000000400000004 R_X86_64_PLT32         0000000000000000 strlen_asm - 4
-00000000000000da  0000000900000004 R_X86_64_PLT32         0000000000000000 memmove - 4
-00000000000000eb  0000000a00000004 R_X86_64_PLT32         0000000000000000 free - 4
-0000000000000101  0000000a00000004 R_X86_64_PLT32         0000000000000000 free - 4
+00000000000000be  0000000900000004 R_X86_64_PLT32         0000000000000000 free - 4
+00000000000000e4  0000000400000004 R_X86_64_PLT32         0000000000000000 strlen_asm - 4
+0000000000000100  0000000a00000004 R_X86_64_PLT32         0000000000000000 memmove - 4
+00000000000000d4  0000000900000004 R_X86_64_PLT32         0000000000000000 free - 4
 
-Relocation section '.rela.eh_frame' at offset 0x470 contains 1 entry:
+Relocation section '.rela.eh_frame' at offset 0x478 contains 1 entry:
     Offset             Info             Type               Symbol's Value  Symbol's Name + Addend
 0000000000000020  0000000200000002 R_X86_64_PC32          0000000000000000 .text + 0
```

##### readelf --wide --debug-dump=frames {}

```diff
@@ -9,43 +9,51 @@
   Return address column: 16
   Augmentation data:     1b
   DW_CFA_def_cfa: r7 (rsp) ofs 8
   DW_CFA_offset: r16 (rip) at cfa-8
   DW_CFA_nop
   DW_CFA_nop
 
-00000018 0000000000000044 0000001c FDE cie=00000000 pc=0000000000000000..0000000000000105
+00000018 000000000000004c 0000001c FDE cie=00000000 pc=0000000000000000..0000000000000109
   DW_CFA_advance_loc: 6 to 0000000000000006
   DW_CFA_def_cfa_offset: 16
   DW_CFA_offset: r15 (r15) at cfa-16
   DW_CFA_advance_loc: 2 to 0000000000000008
   DW_CFA_def_cfa_offset: 24
   DW_CFA_offset: r14 (r14) at cfa-24
   DW_CFA_advance_loc: 5 to 000000000000000d
   DW_CFA_def_cfa_offset: 32
   DW_CFA_offset: r13 (r13) at cfa-32
-  DW_CFA_advance_loc: 2 to 000000000000000f
+  DW_CFA_advance_loc: 5 to 0000000000000012
   DW_CFA_def_cfa_offset: 40
   DW_CFA_offset: r12 (r12) at cfa-40
-  DW_CFA_advance_loc: 1 to 0000000000000010
+  DW_CFA_advance_loc: 4 to 0000000000000016
   DW_CFA_def_cfa_offset: 48
   DW_CFA_offset: r6 (rbp) at cfa-48
-  DW_CFA_advance_loc: 4 to 0000000000000014
+  DW_CFA_advance_loc: 1 to 0000000000000017
   DW_CFA_def_cfa_offset: 56
   DW_CFA_offset: r3 (rbx) at cfa-56
-  DW_CFA_advance_loc: 7 to 000000000000001b
+  DW_CFA_advance_loc: 4 to 000000000000001b
   DW_CFA_def_cfa_offset: 80
-  DW_CFA_advance_loc1: 216 to 00000000000000f3
+  DW_CFA_advance_loc1: 171 to 00000000000000c6
+  DW_CFA_remember_state
   DW_CFA_def_cfa_offset: 56
-  DW_CFA_advance_loc: 4 to 00000000000000f7
+  DW_CFA_advance_loc: 4 to 00000000000000ca
   DW_CFA_def_cfa_offset: 48
-  DW_CFA_advance_loc: 1 to 00000000000000f8
+  DW_CFA_advance_loc: 1 to 00000000000000cb
   DW_CFA_def_cfa_offset: 40
-  DW_CFA_advance_loc: 2 to 00000000000000fa
+  DW_CFA_advance_loc: 2 to 00000000000000cd
   DW_CFA_def_cfa_offset: 32
-  DW_CFA_advance_loc: 2 to 00000000000000fc
+  DW_CFA_advance_loc: 2 to 00000000000000cf
   DW_CFA_def_cfa_offset: 24
-  DW_CFA_advance_loc: 2 to 00000000000000fe
+  DW_CFA_advance_loc: 2 to 00000000000000d1
   DW_CFA_def_cfa_offset: 16
-  DW_CFA_advance_loc: 2 to 0000000000000100
+  DW_CFA_advance_loc: 2 to 00000000000000d3
   DW_CFA_def_cfa_offset: 8
+  DW_CFA_advance_loc: 13 to 00000000000000e0
+  DW_CFA_restore_state
+  DW_CFA_nop
+  DW_CFA_nop
+  DW_CFA_nop
+  DW_CFA_nop
+  DW_CFA_nop
```

##### objdump --line-numbers --disassemble --demangle --reloc --no-show-raw-insn --section=.text {}

```diff
@@ -4,90 +4,91 @@
 Disassembly of section .text:
 
 0000000000000000 <divide_whole>:
 divide_whole():
 	endbr64
 	push   %r15
 	push   %r14
-	mov    %rsi,%r14
+	mov    %rdx,%r14
 	push   %r13
+	mov    %rsi,%r13
 	push   %r12
+	mov    %rcx,%r12
 	push   %rbp
-	mov    %rdx,%rbp
 	push   %rbx
-	mov    %rcx,%rbx
 	sub    $0x18,%rsp
 	mov    %rdi,0x8(%rsp)
 	call   25 <divide_whole+0x25>
  R_X86_64_PLT32	strlen_asm-0x4
-	mov    %r14,%rdi
+	mov    %r13,%rdi
 	mov    %rax,%r15
 	call   30 <divide_whole+0x30>
  R_X86_64_PLT32	strlen_asm-0x4
 	mov    $0x1,%esi
-	mov    %rax,%r13
-	lea    (%r15,%rbx,1),%rax
+	mov    %rax,%rbx
+	lea    (%r15,%r12,1),%rax
 	lea    0x1(%rax),%rdi
 	mov    %rax,(%rsp)
 	call   49 <divide_whole+0x49>
  R_X86_64_PLT32	calloc-0x4
-	mov    %rax,%r12
+	mov    %rax,%rbp
 	test   %r15,%r15
 	je     61 <divide_whole+0x61>
 	mov    0x8(%rsp),%rsi
 	mov    %r15,%rdx
 	mov    %rax,%rdi
 	call   61 <divide_whole+0x61>
  R_X86_64_PLT32	memcpy-0x4
 	cmp    (%rsp),%r15
-	jae    78 <divide_whole+0x78>
-	lea    (%r12,%r15,1),%rdi
-	mov    %rbx,%rdx
+	jae    79 <divide_whole+0x79>
+	lea    0x0(%rbp,%r15,1),%rdi
+	mov    %r12,%rdx
 	mov    $0x30,%esi
-	call   78 <divide_whole+0x78>
+	call   79 <divide_whole+0x79>
  R_X86_64_PLT32	memset-0x4
 	mov    (%rsp),%rax
-	lea    0x0(%r13,%r13,4),%rdx
+	lea    (%rbx,%rbx,4),%rdx
 	mov    $0x1,%esi
-	lea    0x2(%r13,%rax,1),%rcx
+	lea    0x2(%rbx,%rax,1),%rcx
 	lea    (%rcx,%rcx,4),%rax
 	mov    %rcx,(%rsp)
 	lea    0x17(%rax,%rdx,2),%rdi
 	call   9d <divide_whole+0x9d>
  R_X86_64_PLT32	calloc-0x4
 	mov    (%rsp),%rcx
-	mov    %rbp,%rdx
-	mov    %r14,%rsi
+	mov    %r14,%rdx
+	mov    %r13,%rsi
 	mov    %rax,%r8
-	mov    %r12,%rdi
+	mov    %rbp,%rdi
 	mov    %rax,%r15
 	call   b5 <divide_whole+0xb5>
  R_X86_64_PLT32	_divide_whole_with_remainder-0x4
-	mov    %rbp,%rdi
-	call   bd <divide_whole+0xbd>
- R_X86_64_PLT32	strlen_asm-0x4
-	mov    %rax,%r13
-	test   %rbx,%rbx
-	je     de <divide_whole+0xde>
-	mov    %rax,%rsi
-	sub    %rbx,%rax
-	mov    %rbx,%rdx
-	sub    %rbx,%rsi
-	lea    0x1(%rbp,%rax,1),%rdi
-	add    %rbp,%rsi
-	call   de <divide_whole+0xde>
- R_X86_64_PLT32	memmove-0x4
-	sub    %rbx,%r13
+	test   %r12,%r12
+	jne    e0 <divide_whole+0xe0>
 	mov    %r15,%rdi
-	movb   $0x2e,0x0(%rbp,%r13,1)
-	call   ef <divide_whole+0xef>
+	call   c2 <divide_whole+0xc2>
  R_X86_64_PLT32	free-0x4
 	add    $0x18,%rsp
-	mov    %r12,%rdi
+	mov    %rbp,%rdi
 	pop    %rbx
 	pop    %rbp
 	pop    %r12
 	pop    %r13
 	pop    %r14
 	pop    %r15
-	jmp    105 <divide_whole+0x105>
+	jmp    d8 <divide_whole+0xd8>
  R_X86_64_PLT32	free-0x4
+	nopl   0x0(%rax,%rax,1)
+	mov    %r14,%rdi
+	call   e8 <divide_whole+0xe8>
+ R_X86_64_PLT32	strlen_asm-0x4
+	mov    %r12,%rdx
+	mov    %rax,%rbx
+	sub    %r12,%rax
+	sub    %r12,%rbx
+	lea    0x1(%r14,%rax,1),%rdi
+	add    %r14,%rbx
+	mov    %rbx,%rsi
+	call   104 <divide_whole+0x104>
+ R_X86_64_PLT32	memmove-0x4
+	movb   $0x2e,(%rbx)
+	jmp    ba <divide_whole+0xba>
```

##### readelf --wide --decompress --hex-dump=.eh_frame {}

```diff
@@ -1,10 +1,11 @@
 
 Hex dump of section '.eh_frame':
  NOTE: This section has relocations against it, but these have NOT been applied to this dump.
   0x00000000 14000000 00000000 017a5200 01781001 .........zR..x..
-  0x00000010 1b0c0708 90010000 44000000 1c000000 ........D.......
-  0x00000020 00000000 05010000 00460e10 8f02420e .........F....B.
-  0x00000030 188e0345 0e208d04 420e288c 05410e30 ...E. ..B.(..A.0
-  0x00000040 8606440e 38830747 0e5002d8 0e38440e ..D.8..G.P...8D.
-  0x00000050 30410e28 420e2042 0e18420e 10420e08 0A.(B. B..B..B..
+  0x00000010 1b0c0708 90010000 4c000000 1c000000 ........L.......
+  0x00000020 00000000 09010000 00460e10 8f02420e .........F....B.
+  0x00000030 188e0345 0e208d04 450e288c 05440e30 ...E. ..E.(..D.0
+  0x00000040 8606410e 38830744 0e5002ab 0a0e3844 ..A.8..D.P....8D
+  0x00000050 0e30410e 28420e20 420e1842 0e10420e .0A.(B. B..B..B.
+  0x00000060 084d0b00 00000000                   .M......
```

##### readelf --wide --decompress --hex-dump=.strtab {}

```diff
@@ -1,10 +1,10 @@
 
 Hex dump of section '.strtab':
   0x00000000 00646976 6964655f 77686f6c 652e6300 .divide_whole.c.
   0x00000010 64697669 64655f77 686f6c65 00737472 divide_whole.str
   0x00000020 6c656e5f 61736d00 63616c6c 6f63006d len_asm.calloc.m
   0x00000030 656d6370 79006d65 6d736574 005f6469 emcpy.memset._di
   0x00000040 76696465 5f77686f 6c655f77 6974685f vide_whole_with_
-  0x00000050 72656d61 696e6465 72006d65 6d6d6f76 remainder.memmov
-  0x00000060 65006672 656500                     e.free.
+  0x00000050 72656d61 696e6465 72006672 6565006d remainder.free.m
+  0x00000060 656d6d6f 766500                     emmove.
```

### Comparing `basic_math_operations-1.0.158/src/python-module/module.c` & `basic_math_operations-1.0.159/src/python-module/module.c`

 * *Files identical despite different names*

