# Comparing `tmp/blint-1.0.8.tar.gz` & `tmp/blint-1.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "blint-1.0.8.tar", max compression
+gzip compressed data, was "blint-1.0.9.tar", max compression
```

## Comparing `blint-1.0.8.tar` & `blint-1.0.9.tar`

### file list

```diff
@@ -1,19 +1,20 @@
--rw-r--r--   0        0        0    11357 2021-09-24 18:47:41.133537 blint-1.0.8/LICENSE
--rw-r--r--   0        0        0     2823 2021-11-03 21:13:07.540119 blint-1.0.8/README.md
--rw-r--r--   0        0        0        0 2021-09-24 11:08:37.856853 blint-1.0.8/blint/__init__.py
--rw-r--r--   0        0        0    13736 2021-11-15 19:20:06.655945 blint-1.0.8/blint/analysis.py
--rw-r--r--   0        0        0    34852 2021-11-15 19:20:06.659953 blint-1.0.8/blint/binary.py
--rw-r--r--   0        0        0     2629 2021-11-12 16:40:35.847696 blint-1.0.8/blint/cli.py
--rw-r--r--   0        0        0        0 2021-10-22 11:17:42.634150 blint-1.0.8/blint/data/__init__.py
--rw-r--r--   0        0        0        0 2021-10-22 11:19:37.326346 blint-1.0.8/blint/data/annotations/__init__.py
--rw-r--r--   0        0        0    43147 2021-11-15 19:20:06.659953 blint-1.0.8/blint/data/annotations/review_imports_pe.yml
--rw-r--r--   0        0        0     3839 2021-10-28 08:58:43.436423 blint-1.0.8/blint/data/annotations/review_methods_generic.yml
--rw-r--r--   0        0        0    12854 2021-10-27 13:50:49.372288 blint-1.0.8/blint/data/annotations/review_methods_go.yml
--rw-r--r--   0        0        0    19145 2021-11-15 19:20:06.659953 blint-1.0.8/blint/data/annotations/review_symbols_macho.yml
--rw-r--r--   0        0        0    10425 2021-11-15 19:20:06.659953 blint-1.0.8/blint/data/annotations/review_symbols_rust.yml
--rw-r--r--   0        0        0     8546 2021-11-15 19:20:06.659953 blint-1.0.8/blint/data/rules.yml
--rw-r--r--   0        0        0      741 2021-10-26 20:32:29.570281 blint-1.0.8/blint/logger.py
--rw-r--r--   0        0        0     9546 2021-11-15 19:20:06.659953 blint-1.0.8/blint/utils.py
--rw-r--r--   0        0        0     1270 2021-11-16 12:56:23.650367 blint-1.0.8/pyproject.toml
--rw-r--r--   0        0        0     3723 2021-11-16 12:57:11.329796 blint-1.0.8/setup.py
--rw-r--r--   0        0        0     4060 2021-11-16 12:57:11.330227 blint-1.0.8/PKG-INFO
+-rw-r--r--   0        0        0    11357 2021-09-24 18:47:41.133537 blint-1.0.9/LICENSE
+-rw-r--r--   0        0        0     2823 2021-11-03 21:13:07.540119 blint-1.0.9/README.md
+-rw-r--r--   0        0        0        0 2021-09-24 11:08:37.856853 blint-1.0.9/blint/__init__.py
+-rw-r--r--   0        0        0    13736 2021-11-15 19:20:06.655945 blint-1.0.9/blint/analysis.py
+-rw-r--r--   0        0        0    35072 2021-11-20 13:40:50.721054 blint-1.0.9/blint/binary.py
+-rw-r--r--   0        0        0     2629 2021-11-12 16:40:35.847696 blint-1.0.9/blint/cli.py
+-rw-r--r--   0        0        0        0 2021-10-22 11:17:42.634150 blint-1.0.9/blint/data/__init__.py
+-rw-r--r--   0        0        0        0 2021-10-22 11:19:37.326346 blint-1.0.9/blint/data/annotations/__init__.py
+-rw-r--r--   0        0        0    43147 2021-11-15 19:20:06.659953 blint-1.0.9/blint/data/annotations/review_imports_pe.yml
+-rw-r--r--   0        0        0     3839 2021-10-28 08:58:43.436423 blint-1.0.9/blint/data/annotations/review_methods_generic.yml
+-rw-r--r--   0        0        0    12854 2021-10-27 13:50:49.372288 blint-1.0.9/blint/data/annotations/review_methods_go.yml
+-rw-r--r--   0        0        0     5764 2021-11-20 14:19:17.887332 blint-1.0.9/blint/data/annotations/review_methods_mips.yml
+-rw-r--r--   0        0        0    19145 2021-11-15 19:20:06.659953 blint-1.0.9/blint/data/annotations/review_symbols_macho.yml
+-rw-r--r--   0        0        0    10425 2021-11-15 19:20:06.659953 blint-1.0.9/blint/data/annotations/review_symbols_rust.yml
+-rw-r--r--   0        0        0     8634 2021-11-20 13:44:27.409059 blint-1.0.9/blint/data/rules.yml
+-rw-r--r--   0        0        0      741 2021-10-26 20:32:29.570281 blint-1.0.9/blint/logger.py
+-rw-r--r--   0        0        0     9546 2021-11-15 19:20:06.659953 blint-1.0.9/blint/utils.py
+-rw-r--r--   0        0        0     1270 2021-11-20 14:08:33.339570 blint-1.0.9/pyproject.toml
+-rw-r--r--   0        0        0     3723 2021-11-20 14:22:03.160196 blint-1.0.9/setup.py
+-rw-r--r--   0        0        0     4060 2021-11-20 14:22:03.160468 blint-1.0.9/PKG-INFO
```

### Comparing `blint-1.0.8/LICENSE` & `blint-1.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `blint-1.0.8/README.md` & `blint-1.0.9/README.md`

 * *Files identical despite different names*

### Comparing `blint-1.0.8/blint/analysis.py` & `blint-1.0.9/blint/analysis.py`

 * *Files identical despite different names*

### Comparing `blint-1.0.8/blint/binary.py` & `blint-1.0.9/blint/binary.py`

 * *Files 0% similar despite different names*

```diff
@@ -178,20 +178,24 @@
 def parse_interpreter(parsed_obj):
     try:
         return parsed_obj.interpreter
     except lief.exception:
         return None
 
 
-def detect_exe_type(parsed_obj):
+def detect_exe_type(parsed_obj, metadata):
     try:
         if parsed_obj.has_section(".note.go.buildid"):
             return "gobinary"
         elif parsed_obj.has_section(".note.gnu.build-id"):
             return "genericbinary"
+        if metadata.get("machine_type") and metadata.get("file_type"):
+            return "{}-{}".format(
+                metadata.get("machine_type"), metadata.get("file_type")
+            ).lower()
     except lief.exception:
         return None
 
 
 def guess_exe_type(symbol_name):
     exe_type = None
     if "golang" in symbol_name:
@@ -491,15 +495,15 @@
             metadata["name"] = parsed_obj.name
             metadata["imagebase"] = parsed_obj.imagebase
             metadata["interpreter"] = parse_interpreter(parsed_obj)
             metadata["is_pie"] = parsed_obj.is_pie
             metadata["virtual_size"] = parsed_obj.virtual_size
             metadata["has_nx"] = parsed_obj.has_nx
             metadata["relro"] = parse_relro(parsed_obj)
-            metadata["exe_type"] = detect_exe_type(parsed_obj)
+            metadata["exe_type"] = detect_exe_type(parsed_obj, metadata)
             # Canary check
             canary_sections = ["__stack_chk_fail", "__intel_security_cookie"]
             for section in canary_sections:
                 try:
                     if parsed_obj.get_symbol(section):
                         metadata["has_canary"] = True
                         break
```

### Comparing `blint-1.0.8/blint/cli.py` & `blint-1.0.9/blint/cli.py`

 * *Files identical despite different names*

### Comparing `blint-1.0.8/blint/data/annotations/review_imports_pe.yml` & `blint-1.0.9/blint/data/annotations/review_imports_pe.yml`

 * *Files identical despite different names*

### Comparing `blint-1.0.8/blint/data/annotations/review_methods_generic.yml` & `blint-1.0.9/blint/data/annotations/review_methods_generic.yml`

 * *Files identical despite different names*

### Comparing `blint-1.0.8/blint/data/annotations/review_methods_go.yml` & `blint-1.0.9/blint/data/annotations/review_methods_go.yml`

 * *Files identical despite different names*

### Comparing `blint-1.0.8/blint/data/annotations/review_symbols_macho.yml` & `blint-1.0.9/blint/data/annotations/review_symbols_macho.yml`

 * *Files identical despite different names*

### Comparing `blint-1.0.8/blint/data/annotations/review_symbols_rust.yml` & `blint-1.0.9/blint/data/annotations/review_symbols_rust.yml`

 * *Files identical despite different names*

### Comparing `blint-1.0.8/blint/data/rules.yml` & `blint-1.0.9/blint/data/rules.yml`

 * *Files 2% similar despite different names*

```diff
@@ -13,14 +13,15 @@
   exe_types:
     - genericbinary
     - gobinary
     - PE32
     - PE64
     - dotnetbinary
     - MachO
+    - mips-executable
 - id: CHECK_PIE
   title: Missing Position-Independent Executable (PIE) Protection
   description: |
     `Position-Independent Executable (PIE)` executes properly regardless of its absolute address. PIE binaries are used in some security-focused Linux distributions to allow PaX or Exec Shield to use address space layout randomization to prevent attackers from knowing where existing executable code is during a security attack using exploits that rely on knowing the offset of the executable code in the binary, such as return-to-libc attacks.
     Apple's macOS and iOS fully support PIE executables; a warning is issued when non-PIE iOS executables are submitted for approval to Apple's App Store.
     Android enabled support for PIEs in Jelly Bean and removed non-PIE linker support in Lollipop.
     For go binary builds, enable pie by specifying the buildmode=pie as described in the [documentation](https://pkg.go.dev/cmd/go#hdr-Build_modes). The below command line enables pie along with relro and other protections.
@@ -32,14 +33,15 @@
   exe_types:
     - genericbinary
     - gobinary
     - PE32
     - PE64
     - dotnetbinary
     - MachO
+    - mips-executable
 - id: CHECK_RELRO
   title: Missing Relocation Read-Only (RELRO) Protection
   description: |
     A dynamically linked ELF binary uses a look-up table called the Global Offset Table (GOT) to dynamically resolve functions that are located in shared libraries. Such calls point to the Procedure Linkage Table (PLT), which is present in the .plt section of the binary. The GOT is populated dynamically as the program is running. The first time a shared function is called, the GOT contains a pointer back to the PLT, where the dynamic linker is called to find the actual location of the function in question. Since GOT exists at a predefined place in memory, a program that contains a vulnerability allowing an attacker to write 4 bytes at a controlled place in memory (such as some integer overflows leading to out-of-bounds write), may be exploited to allow arbitrary code execution.
     To prevent the above mentioned security weakness, we need to ensure that the linker resolves all dynamically linked functions at the beginning of the execution, and then makes the GOT read-only.  This technique is called RELRO and ensures that the GOT cannot be overwritten in vulnerable ELF binaries.
 
     RELRO can be turned on when compiling a program by using the following options:
@@ -53,14 +55,15 @@
     ```bash
     go build -buildmode=pie -ldflags -extldflags=-Wl,-z,now,-z,relro
     ```
   severity: high
   exe_types:
     - genericbinary
     - gobinary
+    - mips-executable
 - id: CHECK_CANARY
   title: Missing Canary Protection
   description: |
     Canaries or canary words are known values that are placed between a buffer and control data on the stack to monitor buffer overflows. When the buffer overflows, the first data to be corrupted will usually be the canary, and a failed verification of the canary data will therefore alert of an overflow, which can then be handled, for example, by invalidating the corrupted data.
     Canary can be set in GCC with the following parameters:
     ```bash
     -fstack-protector enables protection, but only inserts protection for functions that have arrays in local variables
@@ -69,14 +72,15 @@
     -fstack-protector-explicit Only protects functions with explicit stack_protect attribute
     -fno-stack-protector Disable protection.
     ```
   severity: medium
   exe_types:
     - genericbinary
     - dotnetbinary
+    - mips-executable
 - id: CHECK_RPATH
   title: Avoid rpath and runpath
   description: |
     The job of the dynamic linker and loader (ld.so) is to resolve the executable's dependencies on shared libraries and to load the required ones at run-time. It relies on the executable's NEEDED headers to find the shared libraries with a matching SONAME (which includes the library name and ABI version). The current library search path:
     - The RPATH binary header (set at build-time) of the library causing the lookup (if any)
     - The RPATH binary header (set at build-time) of the executable
     - The LD_LIBRARY_PATH environment variable (set at run-time)
```

### Comparing `blint-1.0.8/blint/logger.py` & `blint-1.0.9/blint/logger.py`

 * *Files identical despite different names*

### Comparing `blint-1.0.8/blint/utils.py` & `blint-1.0.9/blint/utils.py`

 * *Files identical despite different names*

### Comparing `blint-1.0.8/pyproject.toml` & `blint-1.0.9/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "blint"
-version = "1.0.8"
+version = "1.0.9"
 description = "Linter for binary files powered by lief"
 authors = ["Prabhu Subramanian <prabhu@ngcloud.io>"]
 license = "Apache-2.0"
 readme = "README.md"
 homepage = "https://rosa.cx"
 repository = "https://git.sr.ht/~prabhu/blint"
 keywords = ["linter", "binary", "security", "sast"]
```

### Comparing `blint-1.0.8/setup.py` & `blint-1.0.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 ['PyYAML>=5.4.1,<6.0.0', 'lief>=0.11.5,<0.12.0', 'rich>=10.10.0,<11.0.0']
 
 entry_points = \
 {'console_scripts': ['blint = blint.cli:main']}
 
 setup_kwargs = {
     'name': 'blint',
-    'version': '1.0.8',
+    'version': '1.0.9',
     'description': 'Linter for binary files powered by lief',
     'long_description': "# Introduction\n\n[![builds.sr.ht status](https://builds.sr.ht/~prabhu/blint.svg)](https://builds.sr.ht/~prabhu/blint?)\n\nBLint is a Binary Linter to check the security properties, and capabilities in your executables. It is powered by [lief](https://github.com/lief-project/LIEF)\n\n[![BLint Demo](https://asciinema.org/a/438138.png)](https://asciinema.org/a/438138)\n\nCapabilities review is supported for go and rust binaries. Support for dotnet would be available shortly.\n\nSupported binary formats:\n\n- ELF\n- PE\n- Mach-O\n\nYou can run blint on Linux, Windows and Mac against any of these binary formats.\n\n## Motivation\n\nNowadays, vendors distribute statically linked binaries produced by golang or rust or dotnet tooling. Users are used to running antivirus and anti-malware scans while using these binaries in their local devices. Blint augments these scans by listing the technical capabilities of a binary. For example, whether the binary could use network connections, or can perform file system operations and so on.\n\nThe binary is first parsed using lief framework to identify the various properties such as functions, static, and dynamic symbols present. Thanks to a YAML based [annotations](./blint/data/annotations) data, this information could be matched against capabilities and presented visually using a rich table.\n\nNOTE: The presence of capabilities doesn't imply that the operations are always performed by the binary. Use the output of this tool to get an idea about a binary. Also, this tool is not suitable to review malware and other heavily obfuscated binaries for obvious reasons.\n\n## Use cases\n\nBlint was used at [ShiftLeft](https://shiftleft.io) to review and optimize the distributed cli binary.\n\n## Installation\n\n- Install python 3.8 or 3.9\n\n```bash\npip3 install blint\n```\n\n## Usage\n\n```bash\nusage: blint [-h] [-i SRC_DIR_IMAGE] [-o REPORTS_DIR] [--no-error] [--no-banner] [--no-reviews]\n\nLinting tool for binary files powered by lief.\n\noptional arguments:\n  -h, --help            show this help message and exit\n  -i SRC_DIR_IMAGE, --src SRC_DIR_IMAGE\n                        Source directory or container image or binary file\n  -o REPORTS_DIR, --reports REPORTS_DIR\n                        Reports directory\n  --no-error            Continue on error to prevent build from breaking\n  --no-banner           Do not display banner\n  --no-reviews          Do not perform method reviews\n```\n\nTo test any binary including default commands\n\n```bash\nblint -i /bin/netstat -o /tmp/blint\n```\n\nUse -i to check any other binary. For eg: to check ngrok\n\n```bash\nblint -i ~/ngrok -o /tmp/blint\n```\n\nPowerShell example\n\n![PowerShell](./docs/blint-powershell.jpg)\n\n## References\n\n- [lief examples](https://github.com/lief-project/LIEF/tree/master/examples/python)\n- [checksec](https://github.com/Wenzel/checksec.py)\n",
     'author': 'Prabhu Subramanian',
     'author_email': 'prabhu@ngcloud.io',
     'maintainer': None,
     'maintainer_email': None,
     'url': 'https://rosa.cx',
```

### Comparing `blint-1.0.8/PKG-INFO` & `blint-1.0.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: blint
-Version: 1.0.8
+Version: 1.0.9
 Summary: Linter for binary files powered by lief
 Home-page: https://rosa.cx
 License: Apache-2.0
 Keywords: linter,binary,security,sast
 Author: Prabhu Subramanian
 Author-email: prabhu@ngcloud.io
 Requires-Python: >=3.6.2,<4.0
```

