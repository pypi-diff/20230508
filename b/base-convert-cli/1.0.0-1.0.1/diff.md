# Comparing `tmp/base-convert-cli-1.0.0.tar.gz` & `tmp/base-convert-cli-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/base-convert-cli-1.0.0.tar", last modified: Sun Oct 25 21:25:55 2020, max compression
+gzip compressed data, was "/home/kg/proyectos/bs/dist/tmpwf5rvbj_/base-convert-cli-1.0.1.tar", last modified: Mon May  8 15:15:29 2023, max compression
```

## Comparing `base-convert-cli-1.0.0.tar` & `base-convert-cli-1.0.1.tar`

### file list

```diff
@@ -1,15 +1,16 @@
-drwxr-xr-x   0 kevingal  (1000) kevingal  (1000)        0 2020-10-25 21:25:55.000000 base-convert-cli-1.0.0/
-drwxr-xr-x   0 kevingal  (1000) kevingal  (1000)        0 2020-10-25 21:25:55.000000 base-convert-cli-1.0.0/scripts/
--rw-r--r--   0 kevingal  (1000) kevingal  (1000)       68 2020-10-25 21:15:53.000000 base-convert-cli-1.0.0/scripts/bs
--rw-r--r--   0 kevingal  (1000) kevingal  (1000)     2551 2020-10-25 21:25:55.000000 base-convert-cli-1.0.0/PKG-INFO
--rw-r--r--   0 kevingal  (1000) kevingal  (1000)       38 2020-10-25 21:25:55.000000 base-convert-cli-1.0.0/setup.cfg
-drwxr-xr-x   0 kevingal  (1000) kevingal  (1000)        0 2020-10-25 21:25:55.000000 base-convert-cli-1.0.0/src/
-drwxr-xr-x   0 kevingal  (1000) kevingal  (1000)        0 2020-10-25 21:25:55.000000 base-convert-cli-1.0.0/src/baseconvertcli/
--rwxr-xr-x   0 kevingal  (1000) kevingal  (1000)     5335 2020-10-25 21:15:53.000000 base-convert-cli-1.0.0/src/baseconvertcli/__init__.py
-drwxr-xr-x   0 kevingal  (1000) kevingal  (1000)        0 2020-10-25 21:25:55.000000 base-convert-cli-1.0.0/src/base_convert_cli.egg-info/
--rw-r--r--   0 kevingal  (1000) kevingal  (1000)     2551 2020-10-25 21:25:55.000000 base-convert-cli-1.0.0/src/base_convert_cli.egg-info/PKG-INFO
--rw-r--r--   0 kevingal  (1000) kevingal  (1000)      236 2020-10-25 21:25:55.000000 base-convert-cli-1.0.0/src/base_convert_cli.egg-info/SOURCES.txt
--rw-r--r--   0 kevingal  (1000) kevingal  (1000)       15 2020-10-25 21:25:55.000000 base-convert-cli-1.0.0/src/base_convert_cli.egg-info/top_level.txt
--rw-r--r--   0 kevingal  (1000) kevingal  (1000)        1 2020-10-25 21:25:55.000000 base-convert-cli-1.0.0/src/base_convert_cli.egg-info/dependency_links.txt
--rw-r--r--   0 kevingal  (1000) kevingal  (1000)      709 2020-10-25 21:15:53.000000 base-convert-cli-1.0.0/setup.py
--rw-r--r--   0 kevingal  (1000) kevingal  (1000)     1352 2020-10-25 21:15:53.000000 base-convert-cli-1.0.0/README.md
+drwxrwxr-x   0 kg        (1000) kg        (1000)        0 2023-05-08 15:15:29.000000 base-convert-cli-1.0.1/
+-rw-rw-r--   0 kg        (1000) kg        (1000)     2199 2023-05-08 15:15:29.000000 base-convert-cli-1.0.1/PKG-INFO
+-rw-rw-r--   0 kg        (1000) kg        (1000)      709 2023-05-08 15:14:19.000000 base-convert-cli-1.0.1/setup.py
+-rw-r--r--   0 kg        (1000) kg        (1000)     1055 2020-07-26 18:15:45.000000 base-convert-cli-1.0.1/LICENSE.txt
+drwxrwxr-x   0 kg        (1000) kg        (1000)        0 2023-05-08 15:15:29.000000 base-convert-cli-1.0.1/scripts/
+-rw-rw-r--   0 kg        (1000) kg        (1000)       68 2021-12-10 14:15:41.000000 base-convert-cli-1.0.1/scripts/bs
+-rw-rw-r--   0 kg        (1000) kg        (1000)       38 2023-05-08 15:15:29.000000 base-convert-cli-1.0.1/setup.cfg
+-rw-rw-r--   0 kg        (1000) kg        (1000)     1769 2023-05-08 13:35:09.000000 base-convert-cli-1.0.1/README.md
+drwxrwxr-x   0 kg        (1000) kg        (1000)        0 2023-05-08 15:15:29.000000 base-convert-cli-1.0.1/src/
+drwxrwxr-x   0 kg        (1000) kg        (1000)        0 2023-05-08 15:15:29.000000 base-convert-cli-1.0.1/src/base_convert_cli.egg-info/
+-rw-rw-r--   0 kg        (1000) kg        (1000)     2199 2023-05-08 15:15:29.000000 base-convert-cli-1.0.1/src/base_convert_cli.egg-info/PKG-INFO
+-rw-rw-r--   0 kg        (1000) kg        (1000)        1 2023-05-08 15:15:29.000000 base-convert-cli-1.0.1/src/base_convert_cli.egg-info/dependency_links.txt
+-rw-rw-r--   0 kg        (1000) kg        (1000)       15 2023-05-08 15:15:29.000000 base-convert-cli-1.0.1/src/base_convert_cli.egg-info/top_level.txt
+-rw-rw-r--   0 kg        (1000) kg        (1000)      248 2023-05-08 15:15:29.000000 base-convert-cli-1.0.1/src/base_convert_cli.egg-info/SOURCES.txt
+drwxrwxr-x   0 kg        (1000) kg        (1000)        0 2023-05-08 15:15:29.000000 base-convert-cli-1.0.1/src/baseconvertcli/
+-rwxrwxr-x   0 kg        (1000) kg        (1000)     6972 2023-05-08 15:11:15.000000 base-convert-cli-1.0.1/src/baseconvertcli/__init__.py
```

### Comparing `base-convert-cli-1.0.0/src/baseconvertcli/__init__.py` & `base-convert-cli-1.0.1/src/baseconvertcli/__init__.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,55 +1,72 @@
 #!/usr/bin/env python3
 
 import sys
 import re
 import argparse
 
-DIGITS = "0123456789ABCDEF"
+DIGITS = "0123456789ABCDEFGHIJKLMNOPQRSTUVWXYZ"
 
 class InvalidCliArgsError(Exception):
     def __init__(self, message):
         self.message = message
         super().__init__(message)
 
 class Base:
-    def __init__(self, short_names, full_name, size):
+    def __init__(self, short_names, full_name, size, prefix):
         self.names = short_names + [full_name]
         self.full_name = full_name
         self.size = size
-        self.reg = re.compile("^[{}]+$".format(DIGITS[:size]))
+        self.prefix = prefix
+        if prefix:
+            prefix_reg = "(" + prefix + ")?"
+        else:
+            prefix_reg = ""
+        self.reg = re.compile("^{}([{digits}]+)(\\.([{digits}]+))?$".format(prefix_reg, digits=DIGITS[:size]))
 
     def matches(self, s):
         return self.reg.match(s) is not None
 
     def parse(self, s):
         match = self.reg.match(s)
         if not match:
             raise RuntimeError("Failed to parse: {}".format(s))
-        digits = match.group()
-        return sum((self.size**i)*DIGITS.index(d)
-                   for i, d in enumerate(reversed(digits)))
+        if self.prefix:
+            digits = match.group(2)
+            fractional_digits = match.group(3)
+        else:
+            digits = match.group(1)
+            fractional_digits = match.group(2)
+        return (string_to_number(digits, self.size),
+                string_to_number(fractional_digits[1:], self.size) if fractional_digits else None)
 
     def format(self, n):
         if n == 0:
             return "0"
         digits = []
         while n > 0:
             digits.append(DIGITS[n % self.size])
             n = n // self.size
         return "".join(reversed(digits))
 
     def __eq__(self, other):
         return isinstance(other, Base) and other.size == self.size
 
+def string_to_number(s, base_size):
+    return sum((base_size**i)*DIGITS.index(d)
+               for i, d in enumerate(reversed(s))) 
+
 BASES = [
-    Base(["d", "dec"], "decimal", 10),
-    Base(["b", "bin"], "binary", 2),
-    Base(["h", "hex"], "hexadecimal", 16),
-    Base(["o", "oct"], "octal", 8),
+    # Specify prefixes using uppercase letters because input strings
+    # are converted to uppercase first. But from the user perspective,
+    # lowercase letters work.
+    Base(["d", "dec"], "decimal", 10, "0D"),
+    Base(["b", "bin"], "binary", 2, "0B"),
+    Base(["h", "hex"], "hexadecimal", 16, "0X"),
+    Base(["o", "oct"], "octal", 8, "0O"),
 ]
 
 COLOURS = {
     "red": "31"
 }
 
 def show(s, *fmt_args, bold=False, colour=None, newline=True, stream=sys.stdout):
@@ -73,53 +90,62 @@
 def show_error(s, *fmt_args):
     show("ERROR! ", colour="red", newline=False, stream=sys.stderr)
     show(s, *fmt_args, stream=sys.stderr)
 
 def get_parser():
     parser = argparse.ArgumentParser(
         formatter_class=argparse.RawTextHelpFormatter,
-        description="""Convert between number bases up to base-16.
+        description="""Convert between number bases up to base-36.
 
 The more specific the input, the more concise the output. If
 you don't specify the input base or desired output base, then
 the tool will output all possible (common) conversions. If you
 specify the input (using the --from flag) and the output (using
-the --to flag) then it'll just output a single conversion.
+the --to flag) then it'll just output a single conversion. You can
+also specify the input base using the prefixes 0b (binary), 0o (octal),
+0d (decimal) and 0x (hex).
 
 Special bases:
-  n; names
-  2; b, bin, binary
-  8; o, oct, octal
- 10; d, dec, decimal
- 16; h, hex, hexadecimal
+  n | names
+  2 | b, bin, binary
+  8 | o, oct, octal
+ 10 | d, dec, decimal
+ 16 | h, hex, hexadecimal
 
 Examples:
   bs 0                     # many -> many
   bs --from 6 5            # base-6 -> many
   bs --from hexadecimal 5  # hex -> many
+  bs 5 --pad 8             # left-pad with zeros so there are at least 8 digits
   bs --from hex --to dec F # hex -> dec
-  bs -f h -t d F           # short version""")
+  bs -f h -t d F           # short version
+  bs 0xf                   # specify base through prefix
+  bs 1.f                   # fractions""")
     parser.add_argument("n", nargs="?", help="The number to convert. Can also be passed in ASCII/text format through standard input.")
     parser.add_argument("--from", "-f", required=False, dest="fr", help="The input base. Number or name.")
     parser.add_argument("--to", "-t", required=False, help="The output base. Number or name.")
+    parser.add_argument("--pad", default=0, type=int, required=False, help="Whether to add zero padding.")
     return parser
 
 def parse_base(s):
     for base in BASES:
         if s in base.names:
             return base
     try:
         n = int(s)
     except ValueError:
         raise InvalidCliArgsError("Invalid base: {}".format(s))
     if n < 2:
         raise InvalidCliArgsError("Invalid base: {}".format(n))
     if n > len(DIGITS):
-        raise InvalidCliArgsError("Only support up to base-16, but was given: {}".format(n))
-    return Base([], "base-{}".format(n), n)
+        raise InvalidCliArgsError("Only support up to base-36, but given: {}".format(n))
+    for base in BASES:
+        if n == base.size:
+            return base
+    return Base([], "base-{}".format(n), n, "")
 
 def do_conversion(args):
     if args.n:
         s = args.n
     else:
         s = sys.stdin.read()
     s = s.upper()
@@ -127,38 +153,45 @@
         base = parse_base(args.fr)
         if not base.matches(s):
             raise InvalidCliArgsError("Number doesn't match expected base: " + s)
         input_bases = [base]
     else:
         input_bases = [base for base in BASES if base.matches(s)]
         if not input_bases:
-            raise InvalidCliArgsError("Unsupported base, must be <=16.")
+            raise InvalidCliArgsError("Non-standard input base, specify base with --from.")
     if args.to:
         output_bases = [parse_base(args.to)]
     else:
         output_bases = BASES
     if len(input_bases) == 1 and len(output_bases) == 1:
-        n = input_bases[0].parse(s)
-        show(output_bases[0].format(n))
+        n, fractional_n = input_bases[0].parse(s)
+        show(output_bases[0].format(n).zfill(args.pad), newline=False)
+        if fractional_n:
+            show("." + output_bases[0].format(fractional_n), newline=False)
+        show_newline()
     else:
         for i, base in enumerate(input_bases):
-            n = base.parse(s)
+            n, fractional_n = base.parse(s)
             if all(obase == base for obase in output_bases):
                 # Don't print anything if there's only a pointless
                 # conversion (from a base to itself).
                 continue
 
             show("[from {}]", base.full_name, bold=True)
             max_name_length = max(len(base.full_name) for base in output_bases)
             for output_base in output_bases:
                 if output_base != base:
                     show(
                         "  {:<" + str(max_name_length+1) + "}{}",
                         output_base.full_name,
-                        output_base.format(n))
+                        output_base.format(n).zfill(args.pad),
+                        newline=False)
+                    if fractional_n:
+                        show("." + output_base.format(fractional_n), newline=False)
+                    show_newline()
             if i != len(input_bases) - 1:
                 show_newline()
 
 def main():
     parser = get_parser()
     args = parser.parse_args()
     try:
```

### Comparing `base-convert-cli-1.0.0/setup.py` & `base-convert-cli-1.0.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -5,15 +5,15 @@
     long_description = f.read()
 
 setup(
     name="base-convert-cli",
     description="A CLI tool that converts numbers between bases.",
     long_description=long_description,
     long_description_content_type="text/markdown",
-    version="1.0.0",
+    version="1.0.1",
     url="https://github.com/Kevinpgalligan/bs",
     author="Kevin Galligan",
     author_email="galligankevinp@gmail.com",
     scripts=["scripts/bs"],
     packages=find_packages("src"),
     package_dir={'': 'src'},
     classifiers=[
```

### Comparing `base-convert-cli-1.0.0/README.md` & `base-convert-cli-1.0.1/README.md`

 * *Files 17% similar despite different names*

```diff
@@ -8,18 +8,18 @@
   binary      1111111111111110
   octal       177776
 $ bs -t d F
 15
 ```
 
 ## Installation
-This is a Python 3 script, installed from PyPI using pip.
+This is a Python 3 script, installed from [PyPI](https://pypi.org/project/base-convert-cli/) using pip.
 
 ```
-pip3 install baseconvertcli
+pip3 install base-convert-cli
 ```
 
 Hasn't been tested on Windows.
 
 ## Examples
 If you don't specify a base, it does all common conversions.
 
@@ -30,33 +30,45 @@
   hexadecimal 0
   octal       0
 
 [from binary]
 <clipped output here>
 ```
 
+Specify the base through the prefix `0b` for binary, `0o` for octal, `0d` for decimal and `0x` for hex.
+
+```
+$ bs 0xF
+bs 0xF
+[from hexadecimal]
+  decimal     15
+  binary      1111
+  octal       17
+
+```
+
 Specifying base through a flag.
 
 ```
 $ bs --from hex F
 [from hexadecimal]
   decimal     15
   binary      1111
   octal       17
 ```
 
-From base-6.
+From base-36 (the maximum supported base, which uses the digits 0-9 and then a-z).
 
 ```
-$ bs --from 6 54
-[from base-6]
-  decimal     34
-  binary      100010
-  hexadecimal 22
-  octal       42
+$ bs --from 36 zx1
+[from base-36]
+  decimal     46549
+  binary      1011010111010101
+  hexadecimal B5D5
+  octal       132725
 ```
 
 To base-7.
 
 ```
 $ bs --to 7 54
 [from decimal]
@@ -79,14 +91,20 @@
 Shorthand for lazy people.
 
 ```
 $ bs -f h -t d F
 15
 ```
 
+Padding with zeroes.
+
+```
+$ bs --from decimal --to binary --pad 8 14
+```
+
 Aaaaand input through a pipe.
 
 ```
 $ echo '5+10' | bc | bs -t h
 [from decimal]
   hexadecimal F
```

