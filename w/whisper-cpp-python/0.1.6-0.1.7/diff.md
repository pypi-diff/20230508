# Comparing `tmp/whisper_cpp_python-0.1.6.tar.gz` & `tmp/whisper_cpp_python-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "whisper_cpp_python-0.1.6.tar", max compression
+gzip compressed data, was "whisper_cpp_python-0.1.7.tar", last modified: Mon May  8 18:17:25 2023, max compression
```

## Comparing `whisper_cpp_python-0.1.6.tar` & `whisper_cpp_python-0.1.7.tar`

### file list

```diff
@@ -1,495 +1,531 @@
--rw-r--r--   0        0        0        0 2023-05-07 14:07:06.700808 whisper_cpp_python-0.1.6/README.md
--rw-r--r--   0        0        0     9385 2023-05-07 22:43:08.058726 whisper_cpp_python-0.1.6/build.py
--rw-r--r--   0        0        0      490 2023-05-07 22:40:50.974881 whisper_cpp_python-0.1.6/pyproject.toml
--rw-r--r--   0        0        0       23 2023-05-07 19:25:03.713049 whisper_cpp_python-0.1.6/whisper_cpp_python/__init__.py
--rw-r--r--   0        0        0       47 2023-05-07 21:31:31.523267 whisper_cpp_python-0.1.6/whisper_cpp_python/vendor/pycparser/.git
--rw-r--r--   0        0        0       32 2023-05-07 20:09:25.966528 whisper_cpp_python-0.1.6/whisper_cpp_python/vendor/pycparser/.gitattributes
--rw-r--r--   0        0        0      591 2023-05-07 20:09:25.967293 whisper_cpp_python-0.1.6/whisper_cpp_python/vendor/pycparser/.github/workflows/ci.yml
--rw-r--r--   0        0        0      165 2023-05-07 20:09:25.967460 whisper_cpp_python-0.1.6/whisper_cpp_python/vendor/pycparser/.gitignore
--rw-r--r--   0        0        0      274 2023-05-07 20:09:25.967599 whisper_cpp_python-0.1.6/whisper_cpp_python/vendor/pycparser/.vimrc
--rw-r--r--   0        0        0    11105 2023-05-07 20:09:25.968537 whisper_cpp_python-0.1.6/whisper_cpp_python/vendor/pycparser/CHANGES
--rw-r--r--   0        0        0      598 2023-05-07 20:09:25.968787 whisper_cpp_python-0.1.6/whisper_cpp_python/vendor/pycparser/CONTRIBUTORS
--rw-r--r--   0        0        0     1543 2023-05-07 20:09:25.969095 whisper_cpp_python-0.1.6/whisper_cpp_python/vendor/pycparser/LICENSE
--rw-r--r--   0        0        0      335 2023-05-07 20:09:25.969382 whisper_cpp_python-0.1.6/whisper_cpp_python/vendor/pycparser/MANIFEST.in
--rw-r--r--   0        0        0     7970 2023-05-07 20:09:25.969701 whisper_cpp_python-0.1.6/whisper_cpp_python/vendor/pycparser/README.rst
--rw-r--r--   0        0        0      584 2023-05-07 20:09:25.969867 whisper_cpp_python-0.1.6/whisper_cpp_python/vendor/pycparser/SECURITY.md
--rw-r--r--   0        0        0     1481 2023-05-07 20:09:25.970029 whisper_cpp_python-0.1.6/whisper_cpp_python/vendor/pycparser/TODO.txt
--rw-r--r--   0        0        0      871 2023-05-07 20:09:25.970343 whisper_cpp_python-0.1.6/whisper_cpp_python/vendor/pycparser/_clean_tables.py
--rw-r--r--   0        0        0      393 2023-05-07 20:09:25.970541 whisper_cpp_python-0.1.6/whisper_cpp_python/vendor/pycparser/examples/README.rst
--rw-r--r--   0        0        0      957 2023-05-07 20:09:25.970682 whisper_cpp_python-0.1.6/whisper_cpp_python/vendor/pycparser/examples/c-to-c.py
--rw-r--r--   0        0        0       50 2023-05-07 20:09:25.971247 whisper_cpp_python-0.1.6/whisper_cpp_python/vendor/pycparser/examples/c_files/basic.c
--rw-r--r--   0        0        0      206 2023-05-07 20:09:25.971403 whisper_cpp_python-0.1.6/whisper_cpp_python/vendor/pycparser/examples/c_files/funky.c
--rw-r--r--   0        0        0     3790 2023-05-07 20:09:25.971577 whisper_cpp_python-0.1.6/whisper_cpp_python/vendor/pycparser/examples/c_files/hash.c
--rw-r--r--   0        0        0     5379 2023-05-07 20:09:25.971818 whisper_cpp_python-0.1.6/whisper_cpp_python/vendor/pycparser/examples/c_files/memmgr.c
--rw-r--r--   0        0        0     2882 2023-05-07 20:09:25.972015 whisper_cpp_python-0.1.6/whisper_cpp_python/vendor/pycparser/examples/c_files/memmgr.h
--rw-r--r--   0        0        0      140 2023-05-07 20:09:25.972147 whisper_cpp_python-0.1.6/whisper_cpp_python/vendor/pycparser/examples/c_files/pragmas.c
--rw-r--r--   0        0        0     1109 2023-05-07 20:09:25.972322 whisper_cpp_python-0.1.6/whisper_cpp_python/vendor/pycparser/examples/c_files/year.c
--rw-r--r--   0        0        0     6398 2023-05-07 20:09:25.972487 whisper_cpp_python-0.1.6/whisper_cpp_python/vendor/pycparser/examples/c_json.py
--rw-r--r--   0        0        0     6428 2023-05-07 20:09:25.972651 whisper_cpp_python-0.1.6/whisper_cpp_python/vendor/pycparser/examples/cdecl.py
--rw-r--r--   0        0        0     1033 2023-05-07 20:09:25.972915 whisper_cpp_python-0.1.6/whisper_cpp_python/vendor/pycparser/examples/dump_ast.py
--rw-r--r--   0        0        0     5489 2023-05-07 20:09:25.973110 whisper_cpp_python-0.1.6/whisper_cpp_python/vendor/pycparser/examples/explore_ast.py
--rw-r--r--   0        0        0     1356 2023-05-07 20:09:25.973279 whisper_cpp_python-0.1.6/whisper_cpp_python/vendor/pycparser/examples/func_calls.py
--rw-r--r--   0        0        0     1334 2023-05-07 20:09:25.973412 whisper_cpp_python-0.1.6/whisper_cpp_python/vendor/pycparser/examples/func_defs.py
--rw-r--r--   0        0        0     1622 2023-05-07 20:09:25.973551 whisper_cpp_python-0.1.6/whisper_cpp_python/vendor/pycparser/examples/func_defs_add_param.py
--rw-r--r--   0        0        0      704 2023-05-07 20:09:25.973686 whisper_cpp_python-0.1.6/whisper_cpp_python/vendor/pycparser/examples/rewrite_ast.py
--rw-r--r--   0        0        0      813 2023-05-07 20:09:25.973827 whisper_cpp_python-0.1.6/whisper_cpp_python/vendor/pycparser/examples/serialize_ast.py
--rw-r--r--   0        0        0      871 2023-05-07 20:09:25.974071 whisper_cpp_python-0.1.6/whisper_cpp_python/vendor/pycparser/examples/using_cpp_libc.py
--rw-r--r--   0        0        0      929 2023-05-07 20:09:25.974330 whisper_cpp_python-0.1.6/whisper_cpp_python/vendor/pycparser/examples/using_gcc_E_libc.py
--rw-r--r--   0        0        0     2918 2023-05-07 20:09:25.974604 whisper_cpp_python-0.1.6/whisper_cpp_python/vendor/pycparser/pycparser/__init__.py
--rw-r--r--   0        0        0    10555 2023-05-07 20:09:25.974803 whisper_cpp_python-0.1.6/whisper_cpp_python/vendor/pycparser/pycparser/_ast_gen.py
--rw-r--r--   0        0        0     1087 2023-05-07 20:09:25.974953 whisper_cpp_python-0.1.6/whisper_cpp_python/vendor/pycparser/pycparser/_build_tables.py
--rw-r--r--   0        0        0     4255 2023-05-07 20:09:25.975119 whisper_cpp_python-0.1.6/whisper_cpp_python/vendor/pycparser/pycparser/_c_ast.cfg
--rw-r--r--   0        0        0     5691 2023-05-07 20:09:25.975276 whisper_cpp_python-0.1.6/whisper_cpp_python/vendor/pycparser/pycparser/ast_transforms.py
--rw-r--r--   0        0        0    31445 2023-05-07 20:09:25.975575 whisper_cpp_python-0.1.6/whisper_cpp_python/vendor/pycparser/pycparser/c_ast.py
--rw-r--r--   0        0        0    17772 2023-05-07 20:09:25.975846 whisper_cpp_python-0.1.6/whisper_cpp_python/vendor/pycparser/pycparser/c_generator.py
--rw-r--r--   0        0        0    17186 2023-05-07 20:09:25.976215 whisper_cpp_python-0.1.6/whisper_cpp_python/vendor/pycparser/pycparser/c_lexer.py
--rw-r--r--   0        0        0    74282 2023-05-07 20:09:25.976906 whisper_cpp_python-0.1.6/whisper_cpp_python/vendor/pycparser/pycparser/c_parser.py
--rw-r--r--   0        0        0     1638 2023-05-07 20:09:25.977125 whisper_cpp_python-0.1.6/whisper_cpp_python/vendor/pycparser/pycparser/ply/LICENSE
--rw-r--r--   0        0        0      102 2023-05-07 20:09:25.977236 whisper_cpp_python-0.1.6/whisper_cpp_python/vendor/pycparser/pycparser/ply/__init__.py
--rw-r--r--   0        0        0    33282 2023-05-07 20:09:25.977817 whisper_cpp_python-0.1.6/whisper_cpp_python/vendor/pycparser/pycparser/ply/cpp.py
--rw-r--r--   0        0        0     3177 2023-05-07 20:09:25.978011 whisper_cpp_python-0.1.6/whisper_cpp_python/vendor/pycparser/pycparser/ply/ctokens.py
--rw-r--r--   0        0        0    42918 2023-05-07 20:09:25.978584 whisper_cpp_python-0.1.6/whisper_cpp_python/vendor/pycparser/pycparser/ply/lex.py
--rw-r--r--   0        0        0   137323 2023-05-07 20:09:25.979498 whisper_cpp_python-0.1.6/whisper_cpp_python/vendor/pycparser/pycparser/ply/yacc.py
--rw-r--r--   0        0        0     2251 2023-05-07 20:09:25.979677 whisper_cpp_python-0.1.6/whisper_cpp_python/vendor/pycparser/pycparser/ply/ygen.py
--rw-r--r--   0        0        0     4875 2023-05-07 20:09:25.979877 whisper_cpp_python-0.1.6/whisper_cpp_python/vendor/pycparser/pycparser/plyparser.py
--rw-r--r--   0        0        0       63 2023-05-07 20:09:25.979999 whisper_cpp_python-0.1.6/whisper_cpp_python/vendor/pycparser/setup.cfg
--rw-r--r--   0        0        0     2294 2023-05-07 20:09:25.980128 whisper_cpp_python-0.1.6/whisper_cpp_python/vendor/pycparser/setup.py
--rw-r--r--   0        0        0       68 2023-05-07 20:09:25.980295 whisper_cpp_python-0.1.6/whisper_cpp_python/vendor/pycparser/tests/README.txt
--rw-r--r--   0        0        0        0 2023-05-07 20:09:25.980353 whisper_cpp_python-0.1.6/whisper_cpp_python/vendor/pycparser/tests/__init__.py
--rw-r--r--   0        0        0     1367 2023-05-07 20:09:25.980527 whisper_cpp_python-0.1.6/whisper_cpp_python/vendor/pycparser/tests/c_files/c11.c
--rw-r--r--   0        0        0    35859 2023-05-07 20:09:25.980921 whisper_cpp_python-0.1.6/whisper_cpp_python/vendor/pycparser/tests/c_files/cppd_with_stdio_h.c
--rw-r--r--   0        0        0      114 2023-05-07 20:09:25.981181 whisper_cpp_python-0.1.6/whisper_cpp_python/vendor/pycparser/tests/c_files/empty.h
--rw-r--r--   0        0        0      250 2023-05-07 20:09:25.981369 whisper_cpp_python-0.1.6/whisper_cpp_python/vendor/pycparser/tests/c_files/example_c_file.c
--rw-r--r--   0        0        0       15 2023-05-07 20:09:25.981625 whisper_cpp_python-0.1.6/whisper_cpp_python/vendor/pycparser/tests/c_files/hdir/9/inc.h
--rw-r--r--   0        0        0     5597 2023-05-07 20:09:25.981747 whisper_cpp_python-0.1.6/whisper_cpp_python/vendor/pycparser/tests/c_files/memmgr.c
--rw-r--r--   0        0        0     2998 2023-05-07 20:09:25.981964 whisper_cpp_python-0.1.6/whisper_cpp_python/vendor/pycparser/tests/c_files/memmgr.h
--rw-r--r--   0        0        0     4038 2023-05-07 20:09:25.982173 whisper_cpp_python-0.1.6/whisper_cpp_python/vendor/pycparser/tests/c_files/memmgr_with_h.c
--rw-r--r--   0        0        0       64 2023-05-07 20:09:25.982332 whisper_cpp_python-0.1.6/whisper_cpp_python/vendor/pycparser/tests/c_files/simplemain.c
--rw-r--r--   0        0        0     1281 2023-05-07 20:09:25.982519 whisper_cpp_python-0.1.6/whisper_cpp_python/vendor/pycparser/tests/c_files/year.c
--rw-r--r--   0        0        0     5147 2023-05-07 20:09:25.982847 whisper_cpp_python-0.1.6/whisper_cpp_python/vendor/pycparser/tests/test_c_ast.py
--rw-r--r--   0        0        0    17769 2023-05-07 20:09:25.983221 whisper_cpp_python-0.1.6/whisper_cpp_python/vendor/pycparser/tests/test_c_generator.py
--rw-r--r--   0        0        0    18041 2023-05-07 20:09:25.983735 whisper_cpp_python-0.1.6/whisper_cpp_python/vendor/pycparser/tests/test_c_lexer.py
--rwxr-xr-x   0        0        0    88548 2023-05-07 20:09:25.984351 whisper_cpp_python-0.1.6/whisper_cpp_python/vendor/pycparser/tests/test_c_parser.py
--rw-r--r--   0        0        0      912 2023-05-07 20:09:25.984525 whisper_cpp_python-0.1.6/whisper_cpp_python/vendor/pycparser/tests/test_examples.py
--rw-r--r--   0        0        0     2657 2023-05-07 20:09:25.984666 whisper_cpp_python-0.1.6/whisper_cpp_python/vendor/pycparser/tests/test_general.py
--rw-r--r--   0        0        0     1530 2023-05-07 20:09:25.984804 whisper_cpp_python-0.1.6/whisper_cpp_python/vendor/pycparser/tests/test_util.py
--rw-r--r--   0        0        0      706 2023-05-07 20:09:25.985036 whisper_cpp_python-0.1.6/whisper_cpp_python/vendor/pycparser/utils/benchmark/README.rst
--rw-r--r--   0        0        0     1691 2023-05-07 20:09:25.985174 whisper_cpp_python-0.1.6/whisper_cpp_python/vendor/pycparser/utils/benchmark/benchmark-parse.py
--rw-r--r--   0        0        0   126856 2023-05-07 20:09:25.986738 whisper_cpp_python-0.1.6/whisper_cpp_python/vendor/pycparser/utils/benchmark/inputs/redis.c.ppout
--rw-r--r--   0        0        0   274717 2023-05-07 20:09:25.988932 whisper_cpp_python-0.1.6/whisper_cpp_python/vendor/pycparser/utils/benchmark/inputs/sqlite-btree.c.ppout
--rw-r--r--   0        0        0   207921 2023-05-07 20:09:25.990667 whisper_cpp_python-0.1.6/whisper_cpp_python/vendor/pycparser/utils/benchmark/inputs/tccgen.c.ppout
--rw-r--r--   0        0        0      118 2023-05-07 20:09:25.991092 whisper_cpp_python-0.1.6/whisper_cpp_python/vendor/pycparser/utils/fake_libc_include/X11/Intrinsic.h
--rw-r--r--   0        0        0      118 2023-05-07 20:09:25.991218 whisper_cpp_python-0.1.6/whisper_cpp_python/vendor/pycparser/utils/fake_libc_include/X11/Xlib.h
--rw-r--r--   0        0        0      311 2023-05-07 20:09:25.991352 whisper_cpp_python-0.1.6/whisper_cpp_python/vendor/pycparser/utils/fake_libc_include/X11/_X11_fake_defines.h
--rw-r--r--   0        0        0     1111 2023-05-07 20:09:25.991484 whisper_cpp_python-0.1.6/whisper_cpp_python/vendor/pycparser/utils/fake_libc_include/X11/_X11_fake_typedefs.h
--rw-r--r--   0        0        0       55 2023-05-07 20:09:25.991732 whisper_cpp_python-0.1.6/whisper_cpp_python/vendor/pycparser/utils/fake_libc_include/_ansi.h
--rw-r--r--   0        0        0     5921 2023-05-07 20:09:25.991923 whisper_cpp_python-0.1.6/whisper_cpp_python/vendor/pycparser/utils/fake_libc_include/_fake_defines.h
--rw-r--r--   0        0        0     6547 2023-05-07 20:09:25.992062 whisper_cpp_python-0.1.6/whisper_cpp_python/vendor/pycparser/utils/fake_libc_include/_fake_typedefs.h
--rw-r--r--   0        0        0       55 2023-05-07 20:09:25.992175 whisper_cpp_python-0.1.6/whisper_cpp_python/vendor/pycparser/utils/fake_libc_include/_syslist.h
--rw-r--r--   0        0        0       55 2023-05-07 20:09:25.992282 whisper_cpp_python-0.1.6/whisper_cpp_python/vendor/pycparser/utils/fake_libc_include/aio.h
--rw-r--r--   0        0        0       55 2023-05-07 20:09:25.992380 whisper_cpp_python-0.1.6/whisper_cpp_python/vendor/pycparser/utils/fake_libc_include/alloca.h
--rw-r--r--   0        0        0       55 2023-05-07 20:09:25.992492 whisper_cpp_python-0.1.6/whisper_cpp_python/vendor/pycparser/utils/fake_libc_include/ar.h
--rw-r--r--   0        0        0       55 2023-05-07 20:09:25.992592 whisper_cpp_python-0.1.6/whisper_cpp_python/vendor/pycparser/utils/fake_libc_include/argz.h
--rw-r--r--   0        0        0       55 2023-05-07 20:09:25.992770 whisper_cpp_python-0.1.6/whisper_cpp_python/vendor/pycparser/utils/fake_libc_include/arpa/inet.h
--rw-r--r--   0        0        0       55 2023-05-07 20:09:25.992938 whisper_cpp_python-0.1.6/whisper_cpp_python/vendor/pycparser/utils/fake_libc_include/asm-generic/int-ll64.h
--rw-r--r--   0        0        0       55 2023-05-07 20:09:25.993055 whisper_cpp_python-0.1.6/whisper_cpp_python/vendor/pycparser/utils/fake_libc_include/assert.h
--rw-r--r--   0        0        0       55 2023-05-07 20:09:25.993165 whisper_cpp_python-0.1.6/whisper_cpp_python/vendor/pycparser/utils/fake_libc_include/complex.h
--rw-r--r--   0        0        0       55 2023-05-07 20:09:25.993268 whisper_cpp_python-0.1.6/whisper_cpp_python/vendor/pycparser/utils/fake_libc_include/cpio.h
--rw-r--r--   0        0        0       55 2023-05-07 20:09:25.993445 whisper_cpp_python-0.1.6/whisper_cpp_python/vendor/pycparser/utils/fake_libc_include/ctype.h
--rw-r--r--   0        0        0       55 2023-05-07 20:09:25.993575 whisper_cpp_python-0.1.6/whisper_cpp_python/vendor/pycparser/utils/fake_libc_include/dirent.h
--rw-r--r--   0        0        0       55 2023-05-07 20:09:25.993679 whisper_cpp_python-0.1.6/whisper_cpp_python/vendor/pycparser/utils/fake_libc_include/dlfcn.h
--rw-r--r--   0        0        0       55 2023-05-07 20:09:25.993789 whisper_cpp_python-0.1.6/whisper_cpp_python/vendor/pycparser/utils/fake_libc_include/emmintrin.h
--rw-r--r--   0        0        0       55 2023-05-07 20:09:25.994073 whisper_cpp_python-0.1.6/whisper_cpp_python/vendor/pycparser/utils/fake_libc_include/endian.h
--rw-r--r--   0        0        0       55 2023-05-07 20:09:25.994215 whisper_cpp_python-0.1.6/whisper_cpp_python/vendor/pycparser/utils/fake_libc_include/envz.h
--rw-r--r--   0        0        0       55 2023-05-07 20:09:25.994322 whisper_cpp_python-0.1.6/whisper_cpp_python/vendor/pycparser/utils/fake_libc_include/errno.h
--rw-r--r--   0        0        0       55 2023-05-07 20:09:25.994423 whisper_cpp_python-0.1.6/whisper_cpp_python/vendor/pycparser/utils/fake_libc_include/fastmath.h
--rw-r--r--   0        0        0       55 2023-05-07 20:09:25.994618 whisper_cpp_python-0.1.6/whisper_cpp_python/vendor/pycparser/utils/fake_libc_include/fcntl.h
--rw-r--r--   0        0        0       55 2023-05-07 20:09:25.994756 whisper_cpp_python-0.1.6/whisper_cpp_python/vendor/pycparser/utils/fake_libc_include/features.h
--rw-r--r--   0        0        0       55 2023-05-07 20:09:25.994882 whisper_cpp_python-0.1.6/whisper_cpp_python/vendor/pycparser/utils/fake_libc_include/fenv.h
--rw-r--r--   0        0        0       55 2023-05-07 20:09:25.994991 whisper_cpp_python-0.1.6/whisper_cpp_python/vendor/pycparser/utils/fake_libc_include/float.h
--rw-r--r--   0        0        0       55 2023-05-07 20:09:25.995088 whisper_cpp_python-0.1.6/whisper_cpp_python/vendor/pycparser/utils/fake_libc_include/fmtmsg.h
--rw-r--r--   0        0        0       55 2023-05-07 20:09:25.995189 whisper_cpp_python-0.1.6/whisper_cpp_python/vendor/pycparser/utils/fake_libc_include/fnmatch.h
--rw-r--r--   0        0        0       55 2023-05-07 20:09:25.995290 whisper_cpp_python-0.1.6/whisper_cpp_python/vendor/pycparser/utils/fake_libc_include/ftw.h
--rw-r--r--   0        0        0       55 2023-05-07 20:09:25.995393 whisper_cpp_python-0.1.6/whisper_cpp_python/vendor/pycparser/utils/fake_libc_include/getopt.h
--rw-r--r--   0        0        0       55 2023-05-07 20:09:25.995489 whisper_cpp_python-0.1.6/whisper_cpp_python/vendor/pycparser/utils/fake_libc_include/glob.h
--rw-r--r--   0        0        0       55 2023-05-07 20:09:25.995611 whisper_cpp_python-0.1.6/whisper_cpp_python/vendor/pycparser/utils/fake_libc_include/grp.h
--rw-r--r--   0        0        0       55 2023-05-07 20:09:25.995727 whisper_cpp_python-0.1.6/whisper_cpp_python/vendor/pycparser/utils/fake_libc_include/iconv.h
--rw-r--r--   0        0        0       55 2023-05-07 20:09:25.995838 whisper_cpp_python-0.1.6/whisper_cpp_python/vendor/pycparser/utils/fake_libc_include/ieeefp.h
--rw-r--r--   0        0        0       55 2023-05-07 20:09:25.995955 whisper_cpp_python-0.1.6/whisper_cpp_python/vendor/pycparser/utils/fake_libc_include/immintrin.h
--rw-r--r--   0        0        0       55 2023-05-07 20:09:25.996074 whisper_cpp_python-0.1.6/whisper_cpp_python/vendor/pycparser/utils/fake_libc_include/inttypes.h
--rw-r--r--   0        0        0       55 2023-05-07 20:09:25.996192 whisper_cpp_python-0.1.6/whisper_cpp_python/vendor/pycparser/utils/fake_libc_include/iso646.h
--rw-r--r--   0        0        0       55 2023-05-07 20:09:25.996298 whisper_cpp_python-0.1.6/whisper_cpp_python/vendor/pycparser/utils/fake_libc_include/langinfo.h
--rw-r--r--   0        0        0       55 2023-05-07 20:09:25.996394 whisper_cpp_python-0.1.6/whisper_cpp_python/vendor/pycparser/utils/fake_libc_include/libgen.h
--rw-r--r--   0        0        0       55 2023-05-07 20:09:25.996519 whisper_cpp_python-0.1.6/whisper_cpp_python/vendor/pycparser/utils/fake_libc_include/libintl.h
--rw-r--r--   0        0        0       55 2023-05-07 20:09:25.996639 whisper_cpp_python-0.1.6/whisper_cpp_python/vendor/pycparser/utils/fake_libc_include/limits.h
--rw-r--r--   0        0        0       55 2023-05-07 20:09:25.996792 whisper_cpp_python-0.1.6/whisper_cpp_python/vendor/pycparser/utils/fake_libc_include/linux/socket.h
--rw-r--r--   0        0        0       55 2023-05-07 20:09:25.996899 whisper_cpp_python-0.1.6/whisper_cpp_python/vendor/pycparser/utils/fake_libc_include/linux/version.h
--rw-r--r--   0        0        0       55 2023-05-07 20:09:25.996996 whisper_cpp_python-0.1.6/whisper_cpp_python/vendor/pycparser/utils/fake_libc_include/locale.h
--rw-r--r--   0        0        0       55 2023-05-07 20:09:25.997090 whisper_cpp_python-0.1.6/whisper_cpp_python/vendor/pycparser/utils/fake_libc_include/malloc.h
--rw-r--r--   0        0        0       55 2023-05-07 20:09:25.997185 whisper_cpp_python-0.1.6/whisper_cpp_python/vendor/pycparser/utils/fake_libc_include/math.h
--rw-r--r--   0        0        0       55 2023-05-07 20:09:25.997440 whisper_cpp_python-0.1.6/whisper_cpp_python/vendor/pycparser/utils/fake_libc_include/mir_toolkit/client_types.h
--rw-r--r--   0        0        0       55 2023-05-07 20:09:25.997684 whisper_cpp_python-0.1.6/whisper_cpp_python/vendor/pycparser/utils/fake_libc_include/monetary.h
--rw-r--r--   0        0        0       55 2023-05-07 20:09:25.997859 whisper_cpp_python-0.1.6/whisper_cpp_python/vendor/pycparser/utils/fake_libc_include/mqueue.h
--rw-r--r--   0        0        0       55 2023-05-07 20:09:25.998015 whisper_cpp_python-0.1.6/whisper_cpp_python/vendor/pycparser/utils/fake_libc_include/ndbm.h
--rw-r--r--   0        0        0       55 2023-05-07 20:09:25.998213 whisper_cpp_python-0.1.6/whisper_cpp_python/vendor/pycparser/utils/fake_libc_include/net/if.h
--rw-r--r--   0        0        0       55 2023-05-07 20:09:25.998346 whisper_cpp_python-0.1.6/whisper_cpp_python/vendor/pycparser/utils/fake_libc_include/netdb.h
--rw-r--r--   0        0        0       55 2023-05-07 20:09:25.998515 whisper_cpp_python-0.1.6/whisper_cpp_python/vendor/pycparser/utils/fake_libc_include/netinet/in.h
--rw-r--r--   0        0        0       55 2023-05-07 20:09:25.998615 whisper_cpp_python-0.1.6/whisper_cpp_python/vendor/pycparser/utils/fake_libc_include/netinet/tcp.h
--rw-r--r--   0        0        0       55 2023-05-07 20:09:25.998789 whisper_cpp_python-0.1.6/whisper_cpp_python/vendor/pycparser/utils/fake_libc_include/newlib.h
--rw-r--r--   0        0        0       55 2023-05-07 20:09:25.999040 whisper_cpp_python-0.1.6/whisper_cpp_python/vendor/pycparser/utils/fake_libc_include/nl_types.h
--rw-r--r--   0        0        0       55 2023-05-07 20:09:25.999292 whisper_cpp_python-0.1.6/whisper_cpp_python/vendor/pycparser/utils/fake_libc_include/openssl/err.h
--rw-r--r--   0        0        0       55 2023-05-07 20:09:25.999412 whisper_cpp_python-0.1.6/whisper_cpp_python/vendor/pycparser/utils/fake_libc_include/openssl/evp.h
--rw-r--r--   0        0        0       55 2023-05-07 20:09:25.999518 whisper_cpp_python-0.1.6/whisper_cpp_python/vendor/pycparser/utils/fake_libc_include/openssl/hmac.h
--rw-r--r--   0        0        0       55 2023-05-07 20:09:25.999620 whisper_cpp_python-0.1.6/whisper_cpp_python/vendor/pycparser/utils/fake_libc_include/openssl/ssl.h
--rw-r--r--   0        0        0       55 2023-05-07 20:09:25.999725 whisper_cpp_python-0.1.6/whisper_cpp_python/vendor/pycparser/utils/fake_libc_include/openssl/x509v3.h
--rw-r--r--   0        0        0       55 2023-05-07 20:09:25.999850 whisper_cpp_python-0.1.6/whisper_cpp_python/vendor/pycparser/utils/fake_libc_include/paths.h
--rw-r--r--   0        0        0       55 2023-05-07 20:09:26.000016 whisper_cpp_python-0.1.6/whisper_cpp_python/vendor/pycparser/utils/fake_libc_include/poll.h
--rw-r--r--   0        0        0       55 2023-05-07 20:09:26.000255 whisper_cpp_python-0.1.6/whisper_cpp_python/vendor/pycparser/utils/fake_libc_include/process.h
--rw-r--r--   0        0        0       55 2023-05-07 20:09:26.000413 whisper_cpp_python-0.1.6/whisper_cpp_python/vendor/pycparser/utils/fake_libc_include/pthread.h
--rw-r--r--   0        0        0       55 2023-05-07 20:09:26.000562 whisper_cpp_python-0.1.6/whisper_cpp_python/vendor/pycparser/utils/fake_libc_include/pwd.h
--rw-r--r--   0        0        0       55 2023-05-07 20:09:26.000687 whisper_cpp_python-0.1.6/whisper_cpp_python/vendor/pycparser/utils/fake_libc_include/reent.h
--rw-r--r--   0        0        0       55 2023-05-07 20:09:26.000856 whisper_cpp_python-0.1.6/whisper_cpp_python/vendor/pycparser/utils/fake_libc_include/regdef.h
--rw-r--r--   0        0        0       55 2023-05-07 20:09:26.000970 whisper_cpp_python-0.1.6/whisper_cpp_python/vendor/pycparser/utils/fake_libc_include/regex.h
--rw-r--r--   0        0        0       55 2023-05-07 20:09:26.001109 whisper_cpp_python-0.1.6/whisper_cpp_python/vendor/pycparser/utils/fake_libc_include/sched.h
--rw-r--r--   0        0        0       55 2023-05-07 20:09:26.001255 whisper_cpp_python-0.1.6/whisper_cpp_python/vendor/pycparser/utils/fake_libc_include/search.h
--rw-r--r--   0        0        0       55 2023-05-07 20:09:26.001432 whisper_cpp_python-0.1.6/whisper_cpp_python/vendor/pycparser/utils/fake_libc_include/semaphore.h
--rw-r--r--   0        0        0       55 2023-05-07 20:09:26.001602 whisper_cpp_python-0.1.6/whisper_cpp_python/vendor/pycparser/utils/fake_libc_include/setjmp.h
--rw-r--r--   0        0        0       55 2023-05-07 20:09:26.001710 whisper_cpp_python-0.1.6/whisper_cpp_python/vendor/pycparser/utils/fake_libc_include/signal.h
--rw-r--r--   0        0        0       55 2023-05-07 20:09:26.001847 whisper_cpp_python-0.1.6/whisper_cpp_python/vendor/pycparser/utils/fake_libc_include/smmintrin.h
--rw-r--r--   0        0        0       55 2023-05-07 20:09:26.002001 whisper_cpp_python-0.1.6/whisper_cpp_python/vendor/pycparser/utils/fake_libc_include/spawn.h
--rw-r--r--   0        0        0       55 2023-05-07 20:09:26.002105 whisper_cpp_python-0.1.6/whisper_cpp_python/vendor/pycparser/utils/fake_libc_include/stdalign.h
--rw-r--r--   0        0        0       55 2023-05-07 20:09:26.002241 whisper_cpp_python-0.1.6/whisper_cpp_python/vendor/pycparser/utils/fake_libc_include/stdarg.h
--rw-r--r--   0        0        0       55 2023-05-07 20:09:26.002411 whisper_cpp_python-0.1.6/whisper_cpp_python/vendor/pycparser/utils/fake_libc_include/stdatomic.h
--rw-r--r--   0        0        0       55 2023-05-07 20:09:26.002624 whisper_cpp_python-0.1.6/whisper_cpp_python/vendor/pycparser/utils/fake_libc_include/stdbool.h
--rw-r--r--   0        0        0       55 2023-05-07 20:09:26.002800 whisper_cpp_python-0.1.6/whisper_cpp_python/vendor/pycparser/utils/fake_libc_include/stddef.h
--rw-r--r--   0        0        0       55 2023-05-07 20:09:26.002916 whisper_cpp_python-0.1.6/whisper_cpp_python/vendor/pycparser/utils/fake_libc_include/stdint.h
--rw-r--r--   0        0        0       55 2023-05-07 20:09:26.003025 whisper_cpp_python-0.1.6/whisper_cpp_python/vendor/pycparser/utils/fake_libc_include/stdio.h
--rw-r--r--   0        0        0       55 2023-05-07 20:09:26.003127 whisper_cpp_python-0.1.6/whisper_cpp_python/vendor/pycparser/utils/fake_libc_include/stdlib.h
--rw-r--r--   0        0        0       55 2023-05-07 20:09:26.003228 whisper_cpp_python-0.1.6/whisper_cpp_python/vendor/pycparser/utils/fake_libc_include/stdnoreturn.h
--rw-r--r--   0        0        0       55 2023-05-07 20:09:26.003326 whisper_cpp_python-0.1.6/whisper_cpp_python/vendor/pycparser/utils/fake_libc_include/string.h
--rw-r--r--   0        0        0       55 2023-05-07 20:09:26.003425 whisper_cpp_python-0.1.6/whisper_cpp_python/vendor/pycparser/utils/fake_libc_include/strings.h
--rw-r--r--   0        0        0       55 2023-05-07 20:09:26.003624 whisper_cpp_python-0.1.6/whisper_cpp_python/vendor/pycparser/utils/fake_libc_include/stropts.h
--rw-r--r--   0        0        0       55 2023-05-07 20:09:26.003795 whisper_cpp_python-0.1.6/whisper_cpp_python/vendor/pycparser/utils/fake_libc_include/sys/ioctl.h
--rw-r--r--   0        0        0       55 2023-05-07 20:09:26.003898 whisper_cpp_python-0.1.6/whisper_cpp_python/vendor/pycparser/utils/fake_libc_include/sys/ipc.h
--rw-r--r--   0        0        0       55 2023-05-07 20:09:26.003993 whisper_cpp_python-0.1.6/whisper_cpp_python/vendor/pycparser/utils/fake_libc_include/sys/mman.h
--rw-r--r--   0        0        0       55 2023-05-07 20:09:26.004087 whisper_cpp_python-0.1.6/whisper_cpp_python/vendor/pycparser/utils/fake_libc_include/sys/msg.h
--rw-r--r--   0        0        0       55 2023-05-07 20:09:26.004181 whisper_cpp_python-0.1.6/whisper_cpp_python/vendor/pycparser/utils/fake_libc_include/sys/poll.h
--rw-r--r--   0        0        0       55 2023-05-07 20:09:26.004281 whisper_cpp_python-0.1.6/whisper_cpp_python/vendor/pycparser/utils/fake_libc_include/sys/resource.h
--rw-r--r--   0        0        0       55 2023-05-07 20:09:26.004391 whisper_cpp_python-0.1.6/whisper_cpp_python/vendor/pycparser/utils/fake_libc_include/sys/select.h
--rw-r--r--   0        0        0       55 2023-05-07 20:09:26.004607 whisper_cpp_python-0.1.6/whisper_cpp_python/vendor/pycparser/utils/fake_libc_include/sys/sem.h
--rw-r--r--   0        0        0       55 2023-05-07 20:09:26.004716 whisper_cpp_python-0.1.6/whisper_cpp_python/vendor/pycparser/utils/fake_libc_include/sys/shm.h
--rw-r--r--   0        0        0       55 2023-05-07 20:09:26.004818 whisper_cpp_python-0.1.6/whisper_cpp_python/vendor/pycparser/utils/fake_libc_include/sys/socket.h
--rw-r--r--   0        0        0       55 2023-05-07 20:09:26.004917 whisper_cpp_python-0.1.6/whisper_cpp_python/vendor/pycparser/utils/fake_libc_include/sys/stat.h
--rw-r--r--   0        0        0       55 2023-05-07 20:09:26.005029 whisper_cpp_python-0.1.6/whisper_cpp_python/vendor/pycparser/utils/fake_libc_include/sys/statvfs.h
--rw-r--r--   0        0        0       55 2023-05-07 20:09:26.005140 whisper_cpp_python-0.1.6/whisper_cpp_python/vendor/pycparser/utils/fake_libc_include/sys/sysctl.h
--rw-r--r--   0        0        0       55 2023-05-07 20:09:26.005244 whisper_cpp_python-0.1.6/whisper_cpp_python/vendor/pycparser/utils/fake_libc_include/sys/time.h
--rw-r--r--   0        0        0       55 2023-05-07 20:09:26.005343 whisper_cpp_python-0.1.6/whisper_cpp_python/vendor/pycparser/utils/fake_libc_include/sys/times.h
--rw-r--r--   0        0        0       55 2023-05-07 20:09:26.005498 whisper_cpp_python-0.1.6/whisper_cpp_python/vendor/pycparser/utils/fake_libc_include/sys/types.h
--rw-r--r--   0        0        0       55 2023-05-07 20:09:26.005698 whisper_cpp_python-0.1.6/whisper_cpp_python/vendor/pycparser/utils/fake_libc_include/sys/uio.h
--rw-r--r--   0        0        0       55 2023-05-07 20:09:26.005820 whisper_cpp_python-0.1.6/whisper_cpp_python/vendor/pycparser/utils/fake_libc_include/sys/un.h
--rw-r--r--   0        0        0       55 2023-05-07 20:09:26.005932 whisper_cpp_python-0.1.6/whisper_cpp_python/vendor/pycparser/utils/fake_libc_include/sys/utsname.h
--rw-r--r--   0        0        0       55 2023-05-07 20:09:26.006038 whisper_cpp_python-0.1.6/whisper_cpp_python/vendor/pycparser/utils/fake_libc_include/sys/wait.h
--rw-r--r--   0        0        0       55 2023-05-07 20:09:26.006156 whisper_cpp_python-0.1.6/whisper_cpp_python/vendor/pycparser/utils/fake_libc_include/syslog.h
--rw-r--r--   0        0        0       55 2023-05-07 20:09:26.006260 whisper_cpp_python-0.1.6/whisper_cpp_python/vendor/pycparser/utils/fake_libc_include/tar.h
--rw-r--r--   0        0        0       55 2023-05-07 20:09:26.006381 whisper_cpp_python-0.1.6/whisper_cpp_python/vendor/pycparser/utils/fake_libc_include/termios.h
--rw-r--r--   0        0        0       55 2023-05-07 20:09:26.006489 whisper_cpp_python-0.1.6/whisper_cpp_python/vendor/pycparser/utils/fake_libc_include/tgmath.h
--rw-r--r--   0        0        0       55 2023-05-07 20:09:26.006636 whisper_cpp_python-0.1.6/whisper_cpp_python/vendor/pycparser/utils/fake_libc_include/threads.h
--rw-r--r--   0        0        0       55 2023-05-07 20:09:26.006739 whisper_cpp_python-0.1.6/whisper_cpp_python/vendor/pycparser/utils/fake_libc_include/time.h
--rw-r--r--   0        0        0       55 2023-05-07 20:09:26.006837 whisper_cpp_python-0.1.6/whisper_cpp_python/vendor/pycparser/utils/fake_libc_include/trace.h
--rw-r--r--   0        0        0       55 2023-05-07 20:09:26.006992 whisper_cpp_python-0.1.6/whisper_cpp_python/vendor/pycparser/utils/fake_libc_include/ulimit.h
--rw-r--r--   0        0        0       55 2023-05-07 20:09:26.007105 whisper_cpp_python-0.1.6/whisper_cpp_python/vendor/pycparser/utils/fake_libc_include/unctrl.h
--rw-r--r--   0        0        0       55 2023-05-07 20:09:26.007213 whisper_cpp_python-0.1.6/whisper_cpp_python/vendor/pycparser/utils/fake_libc_include/unistd.h
--rw-r--r--   0        0        0       55 2023-05-07 20:09:26.007319 whisper_cpp_python-0.1.6/whisper_cpp_python/vendor/pycparser/utils/fake_libc_include/utime.h
--rw-r--r--   0        0        0       55 2023-05-07 20:09:26.007418 whisper_cpp_python-0.1.6/whisper_cpp_python/vendor/pycparser/utils/fake_libc_include/utmp.h
--rw-r--r--   0        0        0       55 2023-05-07 20:09:26.007536 whisper_cpp_python-0.1.6/whisper_cpp_python/vendor/pycparser/utils/fake_libc_include/utmpx.h
--rw-r--r--   0        0        0       55 2023-05-07 20:09:26.007687 whisper_cpp_python-0.1.6/whisper_cpp_python/vendor/pycparser/utils/fake_libc_include/wchar.h
--rw-r--r--   0        0        0       55 2023-05-07 20:09:26.008051 whisper_cpp_python-0.1.6/whisper_cpp_python/vendor/pycparser/utils/fake_libc_include/wctype.h
--rw-r--r--   0        0        0       55 2023-05-07 20:09:26.008232 whisper_cpp_python-0.1.6/whisper_cpp_python/vendor/pycparser/utils/fake_libc_include/wordexp.h
--rw-r--r--   0        0        0       55 2023-05-07 20:09:26.008497 whisper_cpp_python-0.1.6/whisper_cpp_python/vendor/pycparser/utils/fake_libc_include/xcb/xcb.h
--rw-r--r--   0        0        0      514 2023-05-07 20:09:26.008689 whisper_cpp_python-0.1.6/whisper_cpp_python/vendor/pycparser/utils/fake_libc_include/zlib.h
--rw-r--r--   0        0        0      121 2023-05-07 20:09:26.009109 whisper_cpp_python-0.1.6/whisper_cpp_python/vendor/pycparser/utils/internal/constptr.c
--rw-r--r--   0        0        0      335 2023-05-07 20:09:26.009304 whisper_cpp_python-0.1.6/whisper_cpp_python/vendor/pycparser/utils/internal/cppify.bat
--rw-r--r--   0        0        0      358 2023-05-07 20:09:26.009550 whisper_cpp_python-0.1.6/whisper_cpp_python/vendor/pycparser/utils/internal/example_c_file.c
--rw-r--r--   0        0        0      381 2023-05-07 20:09:26.009716 whisper_cpp_python-0.1.6/whisper_cpp_python/vendor/pycparser/utils/internal/fake_includes.py
--rw-r--r--   0        0        0      462 2023-05-07 20:09:26.009878 whisper_cpp_python-0.1.6/whisper_cpp_python/vendor/pycparser/utils/internal/make_fake_typedefs.py
--rw-r--r--   0        0        0     3253 2023-05-07 20:09:26.010057 whisper_cpp_python-0.1.6/whisper_cpp_python/vendor/pycparser/utils/internal/memprofiling.py
--rw-r--r--   0        0        0     2992 2023-05-07 20:09:26.010239 whisper_cpp_python-0.1.6/whisper_cpp_python/vendor/pycparser/utils/internal/zc.c
--rw-r--r--   0        0        0      574 2023-05-07 20:09:26.010404 whisper_cpp_python-0.1.6/whisper_cpp_python/vendor/pycparser/utils/internal/zz-ctoc.py
--rw-r--r--   0        0        0      581 2023-05-07 20:09:26.010586 whisper_cpp_python-0.1.6/whisper_cpp_python/vendor/pycparser/utils/internal/zz_parse.py
--rw-r--r--   0        0        0       49 2023-05-07 21:31:31.526790 whisper_cpp_python-0.1.6/whisper_cpp_python/vendor/whisper.cpp/.git
--rw-r--r--   0        0        0      392 2023-05-07 20:09:26.072868 whisper_cpp_python-0.1.6/whisper_cpp_python/vendor/whisper.cpp/.github/workflows/bindings-go.yml
--rw-r--r--   0        0        0      417 2023-05-07 20:09:26.072995 whisper_cpp_python-0.1.6/whisper_cpp_python/vendor/whisper.cpp/.github/workflows/bindings-ruby.yml
--rw-r--r--   0        0        0     9896 2023-05-07 20:09:26.073176 whisper_cpp_python-0.1.6/whisper_cpp_python/vendor/whisper.cpp/.github/workflows/build.yml
--rw-r--r--   0        0        0     1153 2023-05-07 20:09:26.073304 whisper_cpp_python-0.1.6/whisper_cpp_python/vendor/whisper.cpp/.github/workflows/examples.yml
--rw-r--r--   0        0        0      605 2023-05-07 20:09:26.073659 whisper_cpp_python-0.1.6/whisper_cpp_python/vendor/whisper.cpp/.gitignore
--rw-r--r--   0        0        0       96 2023-05-07 20:09:26.073829 whisper_cpp_python-0.1.6/whisper_cpp_python/vendor/whisper.cpp/.gitmodules
--rw-r--r--   0        0        0    10866 2023-05-07 20:09:26.074464 whisper_cpp_python-0.1.6/whisper_cpp_python/vendor/whisper.cpp/CMakeLists.txt
--rw-r--r--   0        0        0     1072 2023-05-07 20:09:26.074689 whisper_cpp_python-0.1.6/whisper_cpp_python/vendor/whisper.cpp/LICENSE
--rw-r--r--   0        0        0    11058 2023-05-07 20:09:26.074905 whisper_cpp_python-0.1.6/whisper_cpp_python/vendor/whisper.cpp/Makefile
--rw-r--r--   0        0        0    28943 2023-05-07 20:09:26.075315 whisper_cpp_python-0.1.6/whisper_cpp_python/vendor/whisper.cpp/README.md
--rw-r--r--   0        0        0      656 2023-05-07 20:09:26.075535 whisper_cpp_python-0.1.6/whisper_cpp_python/vendor/whisper.cpp/bindings/CMakeLists.txt
--rw-r--r--   0        0        0       13 2023-05-07 20:09:26.075705 whisper_cpp_python-0.1.6/whisper_cpp_python/vendor/whisper.cpp/bindings/go/.gitignore
--rw-r--r--   0        0        0     1069 2023-05-07 20:09:26.075803 whisper_cpp_python-0.1.6/whisper_cpp_python/vendor/whisper.cpp/bindings/go/LICENSE
--rw-r--r--   0        0        0      968 2023-05-07 20:09:26.075950 whisper_cpp_python-0.1.6/whisper_cpp_python/vendor/whisper.cpp/bindings/go/Makefile
--rw-r--r--   0        0        0     2821 2023-05-07 20:09:26.076156 whisper_cpp_python-0.1.6/whisper_cpp_python/vendor/whisper.cpp/bindings/go/README.md
--rw-r--r--   0        0        0      143 2023-05-07 20:09:26.076270 whisper_cpp_python-0.1.6/whisper_cpp_python/vendor/whisper.cpp/bindings/go/doc.go
--rw-r--r--   0        0        0      582 2023-05-07 20:09:26.076532 whisper_cpp_python-0.1.6/whisper_cpp_python/vendor/whisper.cpp/bindings/go/examples/go-model-download/context.go
--rw-r--r--   0        0        0     5323 2023-05-07 20:09:26.076697 whisper_cpp_python-0.1.6/whisper_cpp_python/vendor/whisper.cpp/bindings/go/examples/go-model-download/main.go
--rw-r--r--   0        0        0      625 2023-05-07 20:09:26.076866 whisper_cpp_python-0.1.6/whisper_cpp_python/vendor/whisper.cpp/bindings/go/examples/go-whisper/color.go
--rw-r--r--   0        0        0     4614 2023-05-07 20:09:26.077407 whisper_cpp_python-0.1.6/whisper_cpp_python/vendor/whisper.cpp/bindings/go/examples/go-whisper/flags.go
--rw-r--r--   0        0        0      878 2023-05-07 20:09:26.077588 whisper_cpp_python-0.1.6/whisper_cpp_python/vendor/whisper.cpp/bindings/go/examples/go-whisper/main.go
--rw-r--r--   0        0        0     3290 2023-05-07 20:09:26.077727 whisper_cpp_python-0.1.6/whisper_cpp_python/vendor/whisper.cpp/bindings/go/examples/go-whisper/process.go
--rw-r--r--   0        0        0      380 2023-05-07 20:09:26.077843 whisper_cpp_python-0.1.6/whisper_cpp_python/vendor/whisper.cpp/bindings/go/go.mod
--rw-r--r--   0        0        0     2019 2023-05-07 20:09:26.077962 whisper_cpp_python-0.1.6/whisper_cpp_python/vendor/whisper.cpp/bindings/go/go.sum
--rw-r--r--   0        0        0     3408 2023-05-07 20:09:26.078198 whisper_cpp_python-0.1.6/whisper_cpp_python/vendor/whisper.cpp/bindings/go/params.go
--rw-r--r--   0        0        0      799 2023-05-07 20:09:26.078479 whisper_cpp_python-0.1.6/whisper_cpp_python/vendor/whisper.cpp/bindings/go/pkg/whisper/consts.go
--rw-r--r--   0        0        0     7926 2023-05-07 20:09:26.078632 whisper_cpp_python-0.1.6/whisper_cpp_python/vendor/whisper.cpp/bindings/go/pkg/whisper/context.go
--rw-r--r--   0        0        0     1250 2023-05-07 20:09:26.078757 whisper_cpp_python-0.1.6/whisper_cpp_python/vendor/whisper.cpp/bindings/go/pkg/whisper/context_test.go
--rw-r--r--   0        0        0       85 2023-05-07 20:09:26.078857 whisper_cpp_python-0.1.6/whisper_cpp_python/vendor/whisper.cpp/bindings/go/pkg/whisper/doc.go
--rw-r--r--   0        0        0     2904 2023-05-07 20:09:26.078969 whisper_cpp_python-0.1.6/whisper_cpp_python/vendor/whisper.cpp/bindings/go/pkg/whisper/interface.go
--rw-r--r--   0        0        0     2300 2023-05-07 20:09:26.079088 whisper_cpp_python-0.1.6/whisper_cpp_python/vendor/whisper.cpp/bindings/go/pkg/whisper/model.go
--rw-r--r--   0        0        0   352078 2023-05-07 20:09:26.085936 whisper_cpp_python-0.1.6/whisper_cpp_python/vendor/whisper.cpp/bindings/go/samples/jfk.wav
--rw-r--r--   0        0        0    14538 2023-05-07 20:09:26.086328 whisper_cpp_python-0.1.6/whisper_cpp_python/vendor/whisper.cpp/bindings/go/whisper.go
--rw-r--r--   0        0        0     2810 2023-05-07 20:09:26.086550 whisper_cpp_python-0.1.6/whisper_cpp_python/vendor/whisper.cpp/bindings/go/whisper_test.go
--rw-r--r--   0        0        0       76 2023-05-07 21:31:31.528919 whisper_cpp_python-0.1.6/whisper_cpp_python/vendor/whisper.cpp/bindings/ios/.git
--rw-r--r--   0        0        0      320 2023-05-07 20:09:27.686704 whisper_cpp_python-0.1.6/whisper_cpp_python/vendor/whisper.cpp/bindings/ios/.github/workflows/swift.yml
--rw-r--r--   0        0        0       26 2023-05-07 20:09:27.686854 whisper_cpp_python-0.1.6/whisper_cpp_python/vendor/whisper.cpp/bindings/ios/.gitignore
--rw-r--r--   0        0        0     1072 2023-05-07 20:09:27.686976 whisper_cpp_python-0.1.6/whisper_cpp_python/vendor/whisper.cpp/bindings/ios/LICENSE
--rw-r--r--   0        0        0      732 2023-05-07 20:09:27.687105 whisper_cpp_python-0.1.6/whisper_cpp_python/vendor/whisper.cpp/bindings/ios/Makefile
--rw-r--r--   0        0        0      744 2023-05-07 20:09:27.687724 whisper_cpp_python-0.1.6/whisper_cpp_python/vendor/whisper.cpp/bindings/ios/Makefile-tmpl
--rw-r--r--   0        0        0      519 2023-05-07 20:09:27.688011 whisper_cpp_python-0.1.6/whisper_cpp_python/vendor/whisper.cpp/bindings/ios/Package.swift
--rw-r--r--   0        0        0      661 2023-05-07 20:09:27.688213 whisper_cpp_python-0.1.6/whisper_cpp_python/vendor/whisper.cpp/bindings/ios/README.md
--rw-r--r--   0        0        0     1506 2023-05-07 20:09:27.688784 whisper_cpp_python-0.1.6/whisper_cpp_python/vendor/whisper.cpp/bindings/ios/Sources/test-objc/main.m
--rw-r--r--   0        0        0      868 2023-05-07 20:09:27.689038 whisper_cpp_python-0.1.6/whisper_cpp_python/vendor/whisper.cpp/bindings/ios/Sources/test-swift/main.swift
--rw-r--r--   0        0        0   425638 2023-05-07 20:09:27.691165 whisper_cpp_python-0.1.6/whisper_cpp_python/vendor/whisper.cpp/bindings/ios/Sources/whisper/ggml.c
--rw-r--r--   0        0        0    30532 2023-05-07 20:09:27.691934 whisper_cpp_python-0.1.6/whisper_cpp_python/vendor/whisper.cpp/bindings/ios/Sources/whisper/ggml.h
--rw-r--r--   0        0        0    23720 2023-05-07 20:09:27.692253 whisper_cpp_python-0.1.6/whisper_cpp_python/vendor/whisper.cpp/bindings/ios/Sources/whisper/include/whisper.h
--rw-r--r--   0        0        0   183212 2023-05-07 20:09:27.693609 whisper_cpp_python-0.1.6/whisper_cpp_python/vendor/whisper.cpp/bindings/ios/Sources/whisper/whisper.cpp
--rw-r--r--   0        0        0   586836 2023-05-07 20:09:27.698018 whisper_cpp_python-0.1.6/whisper_cpp_python/vendor/whisper.cpp/bindings/ios/models/for-tests-ggml-base.en.bin
--rw-r--r--   0        0        0        0 2023-05-07 20:09:27.698684 whisper_cpp_python-0.1.6/whisper_cpp_python/vendor/whisper.cpp/bindings/ios/publish-trigger
--rw-r--r--   0        0        0       12 2023-05-07 20:09:26.086794 whisper_cpp_python-0.1.6/whisper_cpp_python/vendor/whisper.cpp/bindings/javascript/.gitignore
--rw-r--r--   0        0        0      991 2023-05-07 20:09:26.086950 whisper_cpp_python-0.1.6/whisper_cpp_python/vendor/whisper.cpp/bindings/javascript/CMakeLists.txt
--rw-r--r--   0        0        0     2547 2023-05-07 20:09:26.087128 whisper_cpp_python-0.1.6/whisper_cpp_python/vendor/whisper.cpp/bindings/javascript/README.md
--rw-r--r--   0        0        0     3002 2023-05-07 20:09:26.087372 whisper_cpp_python-0.1.6/whisper_cpp_python/vendor/whisper.cpp/bindings/javascript/emscripten.cpp
--rw-r--r--   0        0        0     3141 2023-05-07 20:09:26.087518 whisper_cpp_python-0.1.6/whisper_cpp_python/vendor/whisper.cpp/bindings/javascript/libwhisper.worker.js
--rw-r--r--   0        0        0      612 2023-05-07 20:09:26.087635 whisper_cpp_python-0.1.6/whisper_cpp_python/vendor/whisper.cpp/bindings/javascript/package-tmpl.json
--rw-r--r--   0        0        0      600 2023-05-07 20:09:26.087804 whisper_cpp_python-0.1.6/whisper_cpp_python/vendor/whisper.cpp/bindings/javascript/package.json
--rw-r--r--   0        0        0   795866 2023-05-07 20:09:26.095616 whisper_cpp_python-0.1.6/whisper_cpp_python/vendor/whisper.cpp/bindings/javascript/whisper.js
--rw-r--r--   0        0        0       69 2023-05-07 20:09:26.096430 whisper_cpp_python-0.1.6/whisper_cpp_python/vendor/whisper.cpp/bindings/ruby/ext/.gitignore
--rw-r--r--   0        0        0      781 2023-05-07 20:09:26.096607 whisper_cpp_python-0.1.6/whisper_cpp_python/vendor/whisper.cpp/bindings/ruby/ext/extconf.rb
--rw-r--r--   0        0        0    15308 2023-05-07 20:09:26.096865 whisper_cpp_python-0.1.6/whisper_cpp_python/vendor/whisper.cpp/bindings/ruby/ext/ruby_whisper.cpp
--rw-r--r--   0        0        0      243 2023-05-07 20:09:26.097011 whisper_cpp_python-0.1.6/whisper_cpp_python/vendor/whisper.cpp/bindings/ruby/ext/ruby_whisper.h
--rw-r--r--   0        0        0     3444 2023-05-07 20:09:26.097277 whisper_cpp_python-0.1.6/whisper_cpp_python/vendor/whisper.cpp/bindings/ruby/tests/test_whisper.rb
--rw-r--r--   0        0        0     2037 2023-05-07 20:09:26.097578 whisper_cpp_python-0.1.6/whisper_cpp_python/vendor/whisper.cpp/cmake/BuildTypes.cmake
--rw-r--r--   0        0        0      437 2023-05-07 20:09:26.097709 whisper_cpp_python-0.1.6/whisper_cpp_python/vendor/whisper.cpp/cmake/DefaultTargetOptions.cmake
--rw-r--r--   0        0        0      717 2023-05-07 20:09:26.097885 whisper_cpp_python-0.1.6/whisper_cpp_python/vendor/whisper.cpp/cmake/GitVars.cmake
--rw-r--r--   0        0        0     7458 2023-05-07 20:09:26.099076 whisper_cpp_python-0.1.6/whisper_cpp_python/vendor/whisper.cpp/coreml/whisper-decoder-impl.h
--rw-r--r--   0        0        0     8817 2023-05-07 20:09:26.099355 whisper_cpp_python-0.1.6/whisper_cpp_python/vendor/whisper.cpp/coreml/whisper-decoder-impl.m
--rw-r--r--   0        0        0     7190 2023-05-07 20:09:26.099659 whisper_cpp_python-0.1.6/whisper_cpp_python/vendor/whisper.cpp/coreml/whisper-encoder-impl.h
--rw-r--r--   0        0        0     8522 2023-05-07 20:09:26.099809 whisper_cpp_python-0.1.6/whisper_cpp_python/vendor/whisper.cpp/coreml/whisper-encoder-impl.m
--rw-r--r--   0        0        0      562 2023-05-07 20:09:26.100946 whisper_cpp_python-0.1.6/whisper_cpp_python/vendor/whisper.cpp/coreml/whisper-encoder.h
--rw-r--r--   0        0        0     2059 2023-05-07 20:09:26.101124 whisper_cpp_python-0.1.6/whisper_cpp_python/vendor/whisper.cpp/coreml/whisper-encoder.mm
--rw-r--r--   0        0        0     1527 2023-05-07 20:09:26.101339 whisper_cpp_python-0.1.6/whisper_cpp_python/vendor/whisper.cpp/examples/CMakeLists.txt
--rw-r--r--   0        0        0       25 2023-05-07 20:09:26.101580 whisper_cpp_python-0.1.6/whisper_cpp_python/vendor/whisper.cpp/examples/addon.node/.gitignore
--rw-r--r--   0        0        0     1291 2023-05-07 20:09:26.101860 whisper_cpp_python-0.1.6/whisper_cpp_python/vendor/whisper.cpp/examples/addon.node/CMakeLists.txt
--rw-r--r--   0        0        0     1001 2023-05-07 20:09:26.101989 whisper_cpp_python-0.1.6/whisper_cpp_python/vendor/whisper.cpp/examples/addon.node/README.md
--rw-r--r--   0        0        0      619 2023-05-07 20:09:26.102158 whisper_cpp_python-0.1.6/whisper_cpp_python/vendor/whisper.cpp/examples/addon.node/__test__/whisper.spec.js
--rw-r--r--   0        0        0    11631 2023-05-07 20:09:26.102341 whisper_cpp_python-0.1.6/whisper_cpp_python/vendor/whisper.cpp/examples/addon.node/addon.cpp
--rw-r--r--   0        0        0      847 2023-05-07 20:09:26.102450 whisper_cpp_python-0.1.6/whisper_cpp_python/vendor/whisper.cpp/examples/addon.node/index.js
--rw-r--r--   0        0        0      288 2023-05-07 20:09:26.102587 whisper_cpp_python-0.1.6/whisper_cpp_python/vendor/whisper.cpp/examples/addon.node/package.json
--rw-r--r--   0        0        0      161 2023-05-07 20:09:26.103610 whisper_cpp_python-0.1.6/whisper_cpp_python/vendor/whisper.cpp/examples/bench/CMakeLists.txt
--rw-r--r--   0        0        0     1978 2023-05-07 20:09:26.103730 whisper_cpp_python-0.1.6/whisper_cpp_python/vendor/whisper.cpp/examples/bench/README.md
--rw-r--r--   0        0        0     4126 2023-05-07 20:09:26.103957 whisper_cpp_python-0.1.6/whisper_cpp_python/vendor/whisper.cpp/examples/bench/bench.cpp
--rw-r--r--   0        0        0     1161 2023-05-07 20:09:26.102757 whisper_cpp_python-0.1.6/whisper_cpp_python/vendor/whisper.cpp/examples/bench.wasm/CMakeLists.txt
--rw-r--r--   0        0        0      502 2023-05-07 20:09:26.102934 whisper_cpp_python-0.1.6/whisper_cpp_python/vendor/whisper.cpp/examples/bench.wasm/README.md
--rw-r--r--   0        0        0     2623 2023-05-07 20:09:26.103261 whisper_cpp_python-0.1.6/whisper_cpp_python/vendor/whisper.cpp/examples/bench.wasm/emscripten.cpp
--rw-r--r--   0        0        0    12516 2023-05-07 20:09:26.103434 whisper_cpp_python-0.1.6/whisper_cpp_python/vendor/whisper.cpp/examples/bench.wasm/index-tmpl.html
--rw-r--r--   0        0        0      240 2023-05-07 20:09:26.106848 whisper_cpp_python-0.1.6/whisper_cpp_python/vendor/whisper.cpp/examples/command/CMakeLists.txt
--rw-r--r--   0        0        0     1766 2023-05-07 20:09:26.107017 whisper_cpp_python-0.1.6/whisper_cpp_python/vendor/whisper.cpp/examples/command/README.md
--rw-r--r--   0        0        0    24877 2023-05-07 20:09:26.107384 whisper_cpp_python-0.1.6/whisper_cpp_python/vendor/whisper.cpp/examples/command/command.cpp
--rw-r--r--   0        0        0       54 2023-05-07 20:09:26.107521 whisper_cpp_python-0.1.6/whisper_cpp_python/vendor/whisper.cpp/examples/command/commands.txt
--rw-r--r--   0        0        0     1181 2023-05-07 20:09:26.104121 whisper_cpp_python-0.1.6/whisper_cpp_python/vendor/whisper.cpp/examples/command.wasm/CMakeLists.txt
--rw-r--r--   0        0        0      585 2023-05-07 20:09:26.104344 whisper_cpp_python-0.1.6/whisper_cpp_python/vendor/whisper.cpp/examples/command.wasm/README.md
--rw-r--r--   0        0        0    10412 2023-05-07 20:09:26.105386 whisper_cpp_python-0.1.6/whisper_cpp_python/vendor/whisper.cpp/examples/command.wasm/emscripten.cpp
--rw-r--r--   0        0        0    16219 2023-05-07 20:09:26.106585 whisper_cpp_python-0.1.6/whisper_cpp_python/vendor/whisper.cpp/examples/command.wasm/index-tmpl.html
--rw-r--r--   0        0        0     8583 2023-05-07 20:09:26.107711 whisper_cpp_python-0.1.6/whisper_cpp_python/vendor/whisper.cpp/examples/common-ggml.cpp
--rw-r--r--   0        0        0      410 2023-05-07 20:09:26.107845 whisper_cpp_python-0.1.6/whisper_cpp_python/vendor/whisper.cpp/examples/common-ggml.h
--rw-r--r--   0        0        0     6626 2023-05-07 20:09:26.108090 whisper_cpp_python-0.1.6/whisper_cpp_python/vendor/whisper.cpp/examples/common-sdl.cpp
--rw-r--r--   0        0        0     1011 2023-05-07 20:09:26.108236 whisper_cpp_python-0.1.6/whisper_cpp_python/vendor/whisper.cpp/examples/common-sdl.h
--rw-r--r--   0        0        0    15650 2023-05-07 20:09:26.108512 whisper_cpp_python-0.1.6/whisper_cpp_python/vendor/whisper.cpp/examples/common.cpp
--rw-r--r--   0        0        0     3346 2023-05-07 20:09:26.108710 whisper_cpp_python-0.1.6/whisper_cpp_python/vendor/whisper.cpp/examples/common.h
--rw-r--r--   0        0        0   241358 2023-05-07 20:09:26.110590 whisper_cpp_python-0.1.6/whisper_cpp_python/vendor/whisper.cpp/examples/dr_wav.h
--rwxr-xr-x   0        0        0     1197 2023-05-07 20:09:26.110875 whisper_cpp_python-0.1.6/whisper_cpp_python/vendor/whisper.cpp/examples/generate-karaoke.sh
--rw-r--r--   0        0        0     6592 2023-05-07 20:09:26.111097 whisper_cpp_python-0.1.6/whisper_cpp_python/vendor/whisper.cpp/examples/helpers.js
--rwxr-xr-x   0        0        0     2955 2023-05-07 20:09:26.111275 whisper_cpp_python-0.1.6/whisper_cpp_python/vendor/whisper.cpp/examples/livestream.sh
--rw-r--r--   0        0        0      166 2023-05-07 20:09:26.111472 whisper_cpp_python-0.1.6/whisper_cpp_python/vendor/whisper.cpp/examples/main/CMakeLists.txt
--rw-r--r--   0        0        0     2711 2023-05-07 20:09:26.111624 whisper_cpp_python-0.1.6/whisper_cpp_python/vendor/whisper.cpp/examples/main/README.md
--rw-r--r--   0        0        0    36271 2023-05-07 20:09:26.112535 whisper_cpp_python-0.1.6/whisper_cpp_python/vendor/whisper.cpp/examples/main/main.cpp
--rw-r--r--   0        0        0      174 2023-05-07 20:09:26.112773 whisper_cpp_python-0.1.6/whisper_cpp_python/vendor/whisper.cpp/examples/quantize/CMakeLists.txt
--rw-r--r--   0        0        0       75 2023-05-07 20:09:26.112910 whisper_cpp_python-0.1.6/whisper_cpp_python/vendor/whisper.cpp/examples/quantize/README.md
--rw-r--r--   0        0        0     7693 2023-05-07 20:09:26.113065 whisper_cpp_python-0.1.6/whisper_cpp_python/vendor/whisper.cpp/examples/quantize/quantize.cpp
--rw-r--r--   0        0        0      237 2023-05-07 20:09:26.114526 whisper_cpp_python-0.1.6/whisper_cpp_python/vendor/whisper.cpp/examples/stream/CMakeLists.txt
--rw-r--r--   0        0        0     1589 2023-05-07 20:09:26.114792 whisper_cpp_python-0.1.6/whisper_cpp_python/vendor/whisper.cpp/examples/stream/README.md
--rw-r--r--   0        0        0    16389 2023-05-07 20:09:26.115290 whisper_cpp_python-0.1.6/whisper_cpp_python/vendor/whisper.cpp/examples/stream/stream.cpp
--rw-r--r--   0        0        0     1162 2023-05-07 20:09:26.113548 whisper_cpp_python-0.1.6/whisper_cpp_python/vendor/whisper.cpp/examples/stream.wasm/CMakeLists.txt
--rw-r--r--   0        0        0      443 2023-05-07 20:09:26.113717 whisper_cpp_python-0.1.6/whisper_cpp_python/vendor/whisper.cpp/examples/stream.wasm/README.md
--rw-r--r--   0        0        0     6142 2023-05-07 20:09:26.113852 whisper_cpp_python-0.1.6/whisper_cpp_python/vendor/whisper.cpp/examples/stream.wasm/emscripten.cpp
--rw-r--r--   0        0        0    16188 2023-05-07 20:09:26.114110 whisper_cpp_python-0.1.6/whisper_cpp_python/vendor/whisper.cpp/examples/stream.wasm/index-tmpl.html
--rw-r--r--   0        0        0       10 2023-05-07 20:09:26.121106 whisper_cpp_python-0.1.6/whisper_cpp_python/vendor/whisper.cpp/examples/talk/.gitignore
--rw-r--r--   0        0        0      240 2023-05-07 20:09:26.121221 whisper_cpp_python-0.1.6/whisper_cpp_python/vendor/whisper.cpp/examples/talk/CMakeLists.txt
--rw-r--r--   0        0        0     1292 2023-05-07 20:09:26.121361 whisper_cpp_python-0.1.6/whisper_cpp_python/vendor/whisper.cpp/examples/talk/README.md
--rw-r--r--   0        0        0      764 2023-05-07 20:09:26.121474 whisper_cpp_python-0.1.6/whisper_cpp_python/vendor/whisper.cpp/examples/talk/eleven-labs.py
--rw-r--r--   0        0        0    27945 2023-05-07 20:09:26.121695 whisper_cpp_python-0.1.6/whisper_cpp_python/vendor/whisper.cpp/examples/talk/gpt-2.cpp
--rw-r--r--   0        0        0      580 2023-05-07 20:09:26.121904 whisper_cpp_python-0.1.6/whisper_cpp_python/vendor/whisper.cpp/examples/talk/gpt-2.h
--rwxr-xr-x   0        0        0      563 2023-05-07 20:09:26.122038 whisper_cpp_python-0.1.6/whisper_cpp_python/vendor/whisper.cpp/examples/talk/speak.sh
--rw-r--r--   0        0        0    14593 2023-05-07 20:09:26.122190 whisper_cpp_python-0.1.6/whisper_cpp_python/vendor/whisper.cpp/examples/talk/talk.cpp
--rw-r--r--   0        0        0       10 2023-05-07 20:09:26.115626 whisper_cpp_python-0.1.6/whisper_cpp_python/vendor/whisper.cpp/examples/talk-llama/.gitignore
--rw-r--r--   0        0        0      733 2023-05-07 20:09:26.115829 whisper_cpp_python-0.1.6/whisper_cpp_python/vendor/whisper.cpp/examples/talk-llama/CMakeLists.txt
--rw-r--r--   0        0        0     2458 2023-05-07 20:09:26.116046 whisper_cpp_python-0.1.6/whisper_cpp_python/vendor/whisper.cpp/examples/talk-llama/README.md
--rw-r--r--   0        0        0      770 2023-05-07 20:09:26.116243 whisper_cpp_python-0.1.6/whisper_cpp_python/vendor/whisper.cpp/examples/talk-llama/eleven-labs.py
--rw-r--r--   0        0        0    12448 2023-05-07 20:09:26.116560 whisper_cpp_python-0.1.6/whisper_cpp_python/vendor/whisper.cpp/examples/talk-llama/llama-util.h
--rw-r--r--   0        0        0    94701 2023-05-07 20:09:26.117600 whisper_cpp_python-0.1.6/whisper_cpp_python/vendor/whisper.cpp/examples/talk-llama/llama.cpp
--rw-r--r--   0        0        0    13325 2023-05-07 20:09:26.117869 whisper_cpp_python-0.1.6/whisper_cpp_python/vendor/whisper.cpp/examples/talk-llama/llama.h
--rw-r--r--   0        0        0      978 2023-05-07 20:09:26.118146 whisper_cpp_python-0.1.6/whisper_cpp_python/vendor/whisper.cpp/examples/talk-llama/prompts/talk-alpaca.txt
--rwxr-xr-x   0        0        0      588 2023-05-07 20:09:26.119003 whisper_cpp_python-0.1.6/whisper_cpp_python/vendor/whisper.cpp/examples/talk-llama/speak.sh
--rw-r--r--   0        0        0    27971 2023-05-07 20:09:26.119417 whisper_cpp_python-0.1.6/whisper_cpp_python/vendor/whisper.cpp/examples/talk-llama/talk-llama.cpp
--rw-r--r--   0        0        0     1171 2023-05-07 20:09:26.119746 whisper_cpp_python-0.1.6/whisper_cpp_python/vendor/whisper.cpp/examples/talk.wasm/CMakeLists.txt
--rw-r--r--   0        0        0     3341 2023-05-07 20:09:26.119961 whisper_cpp_python-0.1.6/whisper_cpp_python/vendor/whisper.cpp/examples/talk.wasm/README.md
--rw-r--r--   0        0        0    12231 2023-05-07 20:09:26.120154 whisper_cpp_python-0.1.6/whisper_cpp_python/vendor/whisper.cpp/examples/talk.wasm/emscripten.cpp
--rw-r--r--   0        0        0    27945 2023-05-07 20:09:26.120559 whisper_cpp_python-0.1.6/whisper_cpp_python/vendor/whisper.cpp/examples/talk.wasm/gpt-2.cpp
--rw-r--r--   0        0        0      580 2023-05-07 20:09:26.120720 whisper_cpp_python-0.1.6/whisper_cpp_python/vendor/whisper.cpp/examples/talk.wasm/gpt-2.h
--rw-r--r--   0        0        0    33143 2023-05-07 20:09:26.120928 whisper_cpp_python-0.1.6/whisper_cpp_python/vendor/whisper.cpp/examples/talk.wasm/index-tmpl.html
--rwxr-xr-x   0        0        0     2757 2023-05-07 20:09:26.122378 whisper_cpp_python-0.1.6/whisper_cpp_python/vendor/whisper.cpp/examples/twitch.sh
--rw-r--r--   0        0        0      225 2023-05-07 20:09:26.122601 whisper_cpp_python-0.1.6/whisper_cpp_python/vendor/whisper.cpp/examples/whisper.android/.gitignore
--rw-r--r--   0        0        0       47 2023-05-07 20:09:26.122831 whisper_cpp_python-0.1.6/whisper_cpp_python/vendor/whisper.cpp/examples/whisper.android/.idea/.gitignore
--rw-r--r--   0        0        0       14 2023-05-07 20:09:26.122978 whisper_cpp_python-0.1.6/whisper_cpp_python/vendor/whisper.cpp/examples/whisper.android/.idea/.name
--rw-r--r--   0        0        0      169 2023-05-07 20:09:26.123220 whisper_cpp_python-0.1.6/whisper_cpp_python/vendor/whisper.cpp/examples/whisper.android/.idea/compiler.xml
--rw-r--r--   0        0        0      680 2023-05-07 20:09:26.123395 whisper_cpp_python-0.1.6/whisper_cpp_python/vendor/whisper.cpp/examples/whisper.android/.idea/gradle.xml
--rw-r--r--   0        0        0      468 2023-05-07 20:09:26.123555 whisper_cpp_python-0.1.6/whisper_cpp_python/vendor/whisper.cpp/examples/whisper.android/.idea/misc.xml
--rw-r--r--   0        0        0      186 2023-05-07 20:09:26.124132 whisper_cpp_python-0.1.6/whisper_cpp_python/vendor/whisper.cpp/examples/whisper.android/.idea/vcs.xml
--rw-r--r--   0        0        0      973 2023-05-07 20:09:26.124291 whisper_cpp_python-0.1.6/whisper_cpp_python/vendor/whisper.cpp/examples/whisper.android/README.md
--rw-r--r--   0        0        0        6 2023-05-07 20:09:26.124472 whisper_cpp_python-0.1.6/whisper_cpp_python/vendor/whisper.cpp/examples/whisper.android/app/.gitignore
--rw-r--r--   0        0        0     2186 2023-05-07 20:09:26.124614 whisper_cpp_python-0.1.6/whisper_cpp_python/vendor/whisper.cpp/examples/whisper.android/app/build.gradle
--rw-r--r--   0        0        0      750 2023-05-07 20:09:26.124740 whisper_cpp_python-0.1.6/whisper_cpp_python/vendor/whisper.cpp/examples/whisper.android/app/proguard-rules.pro
--rw-r--r--   0        0        0      663 2023-05-07 20:09:26.125272 whisper_cpp_python-0.1.6/whisper_cpp_python/vendor/whisper.cpp/examples/whisper.android/app/src/androidTest/java/com/whispercppdemo/ExampleInstrumentedTest.kt
--rw-r--r--   0        0        0     1124 2023-05-07 20:09:26.125456 whisper_cpp_python-0.1.6/whisper_cpp_python/vendor/whisper.cpp/examples/whisper.android/app/src/main/AndroidManifest.xml
--rw-r--r--   0        0        0      694 2023-05-07 20:09:26.125733 whisper_cpp_python-0.1.6/whisper_cpp_python/vendor/whisper.cpp/examples/whisper.android/app/src/main/java/com/whispercppdemo/MainActivity.kt
--rw-r--r--   0        0        0     2053 2023-05-07 20:09:26.125902 whisper_cpp_python-0.1.6/whisper_cpp_python/vendor/whisper.cpp/examples/whisper.android/app/src/main/java/com/whispercppdemo/media/RiffWaveHelper.kt
--rw-r--r--   0        0        0     2711 2023-05-07 20:09:26.126130 whisper_cpp_python-0.1.6/whisper_cpp_python/vendor/whisper.cpp/examples/whisper.android/app/src/main/java/com/whispercppdemo/recorder/Recorder.kt
--rw-r--r--   0        0        0     3537 2023-05-07 20:09:26.126366 whisper_cpp_python-0.1.6/whisper_cpp_python/vendor/whisper.cpp/examples/whisper.android/app/src/main/java/com/whispercppdemo/ui/main/MainScreen.kt
--rw-r--r--   0        0        0     7330 2023-05-07 20:09:26.126515 whisper_cpp_python-0.1.6/whisper_cpp_python/vendor/whisper.cpp/examples/whisper.android/app/src/main/java/com/whispercppdemo/ui/main/MainScreenViewModel.kt
--rw-r--r--   0        0        0      282 2023-05-07 20:09:26.126677 whisper_cpp_python-0.1.6/whisper_cpp_python/vendor/whisper.cpp/examples/whisper.android/app/src/main/java/com/whispercppdemo/ui/theme/Color.kt
--rw-r--r--   0        0        0     2156 2023-05-07 20:09:26.126802 whisper_cpp_python-0.1.6/whisper_cpp_python/vendor/whisper.cpp/examples/whisper.android/app/src/main/java/com/whispercppdemo/ui/theme/Theme.kt
--rw-r--r--   0        0        0      987 2023-05-07 20:09:26.126914 whisper_cpp_python-0.1.6/whisper_cpp_python/vendor/whisper.cpp/examples/whisper.android/app/src/main/java/com/whispercppdemo/ui/theme/Type.kt
--rw-r--r--   0        0        0     5362 2023-05-07 20:09:26.127150 whisper_cpp_python-0.1.6/whisper_cpp_python/vendor/whisper.cpp/examples/whisper.android/app/src/main/java/com/whispercppdemo/whisper/LibWhisper.kt
--rw-r--r--   0        0        0      834 2023-05-07 20:09:26.127373 whisper_cpp_python-0.1.6/whisper_cpp_python/vendor/whisper.cpp/examples/whisper.android/app/src/main/jni/whisper/Android.mk
--rw-r--r--   0        0        0       21 2023-05-07 20:09:26.127477 whisper_cpp_python-0.1.6/whisper_cpp_python/vendor/whisper.cpp/examples/whisper.android/app/src/main/jni/whisper/Application.mk
--rw-r--r--   0        0        0      708 2023-05-07 20:09:26.127584 whisper_cpp_python-0.1.6/whisper_cpp_python/vendor/whisper.cpp/examples/whisper.android/app/src/main/jni/whisper/Whisper.mk
--rw-r--r--   0        0        0     8393 2023-05-07 20:09:26.127731 whisper_cpp_python-0.1.6/whisper_cpp_python/vendor/whisper.cpp/examples/whisper.android/app/src/main/jni/whisper/jni.c
--rw-r--r--   0        0        0     5606 2023-05-07 20:09:26.128095 whisper_cpp_python-0.1.6/whisper_cpp_python/vendor/whisper.cpp/examples/whisper.android/app/src/main/res/drawable/ic_launcher_background.xml
--rw-r--r--   0        0        0     1702 2023-05-07 20:09:26.128414 whisper_cpp_python-0.1.6/whisper_cpp_python/vendor/whisper.cpp/examples/whisper.android/app/src/main/res/drawable/ic_launcher_foreground.xml
--rw-r--r--   0        0        0      272 2023-05-07 20:09:26.128677 whisper_cpp_python-0.1.6/whisper_cpp_python/vendor/whisper.cpp/examples/whisper.android/app/src/main/res/mipmap-anydpi/ic_launcher.xml
--rw-r--r--   0        0        0      378 2023-05-07 20:09:26.128889 whisper_cpp_python-0.1.6/whisper_cpp_python/vendor/whisper.cpp/examples/whisper.android/app/src/main/res/values/colors.xml
--rw-r--r--   0        0        0       76 2023-05-07 20:09:26.129059 whisper_cpp_python-0.1.6/whisper_cpp_python/vendor/whisper.cpp/examples/whisper.android/app/src/main/res/values/strings.xml
--rw-r--r--   0        0        0      156 2023-05-07 20:09:26.129347 whisper_cpp_python-0.1.6/whisper_cpp_python/vendor/whisper.cpp/examples/whisper.android/app/src/main/res/values/themes.xml
--rw-r--r--   0        0        0      478 2023-05-07 20:09:26.129746 whisper_cpp_python-0.1.6/whisper_cpp_python/vendor/whisper.cpp/examples/whisper.android/app/src/main/res/xml/backup_rules.xml
--rw-r--r--   0        0        0      551 2023-05-07 20:09:26.130001 whisper_cpp_python-0.1.6/whisper_cpp_python/vendor/whisper.cpp/examples/whisper.android/app/src/main/res/xml/data_extraction_rules.xml
--rw-r--r--   0        0        0      342 2023-05-07 20:09:26.130557 whisper_cpp_python-0.1.6/whisper_cpp_python/vendor/whisper.cpp/examples/whisper.android/app/src/test/java/com/whispercppdemo/ExampleUnitTest.kt
--rw-r--r--   0        0        0      296 2023-05-07 20:09:26.130760 whisper_cpp_python-0.1.6/whisper_cpp_python/vendor/whisper.cpp/examples/whisper.android/build.gradle
--rw-r--r--   0        0        0    59203 2023-05-07 20:09:26.132292 whisper_cpp_python-0.1.6/whisper_cpp_python/vendor/whisper.cpp/examples/whisper.android/gradle/wrapper/gradle-wrapper.jar
--rw-r--r--   0        0        0      230 2023-05-07 20:09:26.132642 whisper_cpp_python-0.1.6/whisper_cpp_python/vendor/whisper.cpp/examples/whisper.android/gradle/wrapper/gradle-wrapper.properties
--rw-r--r--   0        0        0     1358 2023-05-07 20:09:26.130956 whisper_cpp_python-0.1.6/whisper_cpp_python/vendor/whisper.cpp/examples/whisper.android/gradle.properties
--rwxr-xr-x   0        0        0     5766 2023-05-07 20:09:26.132894 whisper_cpp_python-0.1.6/whisper_cpp_python/vendor/whisper.cpp/examples/whisper.android/gradlew
--rw-r--r--   0        0        0     2763 2023-05-07 20:09:26.133148 whisper_cpp_python-0.1.6/whisper_cpp_python/vendor/whisper.cpp/examples/whisper.android/gradlew.bat
--rw-r--r--   0        0        0      331 2023-05-07 20:09:26.133340 whisper_cpp_python-0.1.6/whisper_cpp_python/vendor/whisper.cpp/examples/whisper.android/settings.gradle
--rw-r--r--   0        0        0     3766 2023-05-07 20:09:26.133666 whisper_cpp_python-0.1.6/whisper_cpp_python/vendor/whisper.cpp/examples/whisper.nvim/README.md
--rwxr-xr-x   0        0        0     2032 2023-05-07 20:09:26.133907 whisper_cpp_python-0.1.6/whisper_cpp_python/vendor/whisper.cpp/examples/whisper.nvim/whisper.nvim
--rw-r--r--   0        0        0     1189 2023-05-07 20:09:26.134220 whisper_cpp_python-0.1.6/whisper_cpp_python/vendor/whisper.cpp/examples/whisper.objc/README.md
--rw-r--r--   0        0        0      183 2023-05-07 20:09:26.135657 whisper_cpp_python-0.1.6/whisper_cpp_python/vendor/whisper.cpp/examples/whisper.objc/whisper.objc/AppDelegate.h
--rw-r--r--   0        0        0     1320 2023-05-07 20:09:26.135843 whisper_cpp_python-0.1.6/whisper_cpp_python/vendor/whisper.cpp/examples/whisper.objc/whisper.objc/AppDelegate.m
--rw-r--r--   0        0        0      123 2023-05-07 20:09:26.136240 whisper_cpp_python-0.1.6/whisper_cpp_python/vendor/whisper.cpp/examples/whisper.objc/whisper.objc/Assets.xcassets/AccentColor.colorset/Contents.json
--rw-r--r--   0        0        0      177 2023-05-07 20:09:26.136510 whisper_cpp_python-0.1.6/whisper_cpp_python/vendor/whisper.cpp/examples/whisper.objc/whisper.objc/Assets.xcassets/AppIcon.appiconset/Contents.json
--rw-r--r--   0        0        0       63 2023-05-07 20:09:26.136622 whisper_cpp_python-0.1.6/whisper_cpp_python/vendor/whisper.cpp/examples/whisper.objc/whisper.objc/Assets.xcassets/Contents.json
--rw-r--r--   0        0        0     1665 2023-05-07 20:09:26.137035 whisper_cpp_python-0.1.6/whisper_cpp_python/vendor/whisper.cpp/examples/whisper.objc/whisper.objc/Base.lproj/LaunchScreen.storyboard
--rw-r--r--   0        0        0     8419 2023-05-07 20:09:26.137225 whisper_cpp_python-0.1.6/whisper_cpp_python/vendor/whisper.cpp/examples/whisper.objc/whisper.objc/Base.lproj/Main.storyboard
--rw-r--r--   0        0        0      806 2023-05-07 20:09:26.137356 whisper_cpp_python-0.1.6/whisper_cpp_python/vendor/whisper.cpp/examples/whisper.objc/whisper.objc/Info.plist
--rw-r--r--   0        0        0      236 2023-05-07 20:09:26.137469 whisper_cpp_python-0.1.6/whisper_cpp_python/vendor/whisper.cpp/examples/whisper.objc/whisper.objc/SceneDelegate.h
--rw-r--r--   0        0        0     2138 2023-05-07 20:09:26.138070 whisper_cpp_python-0.1.6/whisper_cpp_python/vendor/whisper.cpp/examples/whisper.objc/whisper.objc/SceneDelegate.m
--rw-r--r--   0        0        0      761 2023-05-07 20:09:26.139213 whisper_cpp_python-0.1.6/whisper_cpp_python/vendor/whisper.cpp/examples/whisper.objc/whisper.objc/ViewController.h
--rw-r--r--   0        0        0     9377 2023-05-07 20:09:26.139922 whisper_cpp_python-0.1.6/whisper_cpp_python/vendor/whisper.cpp/examples/whisper.objc/whisper.objc/ViewController.m
--rw-r--r--   0        0        0      447 2023-05-07 20:09:26.140228 whisper_cpp_python-0.1.6/whisper_cpp_python/vendor/whisper.cpp/examples/whisper.objc/whisper.objc/main.m
--rw-r--r--   0        0        0    17120 2023-05-07 20:09:26.134833 whisper_cpp_python-0.1.6/whisper_cpp_python/vendor/whisper.cpp/examples/whisper.objc/whisper.objc.xcodeproj/project.pbxproj
--rw-r--r--   0        0        0      135 2023-05-07 20:09:26.135119 whisper_cpp_python-0.1.6/whisper_cpp_python/vendor/whisper.cpp/examples/whisper.objc/whisper.objc.xcodeproj/project.xcworkspace/contents.xcworkspacedata
--rw-r--r--   0        0        0      238 2023-05-07 20:09:26.135385 whisper_cpp_python-0.1.6/whisper_cpp_python/vendor/whisper.cpp/examples/whisper.objc/whisper.objc.xcodeproj/project.xcworkspace/xcshareddata/IDEWorkspaceChecks.plist
--rw-r--r--   0        0        0     1410 2023-05-07 20:09:26.140899 whisper_cpp_python-0.1.6/whisper_cpp_python/vendor/whisper.cpp/examples/whisper.swiftui/README.md
--rw-r--r--   0        0        0     2267 2023-05-07 20:09:26.141623 whisper_cpp_python-0.1.6/whisper_cpp_python/vendor/whisper.cpp/examples/whisper.swiftui/whisper.cpp.swift/LibWhisper.swift
--rw-r--r--   0        0        0      123 2023-05-07 20:09:26.142248 whisper_cpp_python-0.1.6/whisper_cpp_python/vendor/whisper.cpp/examples/whisper.swiftui/whisper.cpp.swift/WhisperCppDemo-Bridging-Header.h
--rw-r--r--   0        0        0     4966 2023-05-07 20:09:26.143602 whisper_cpp_python-0.1.6/whisper_cpp_python/vendor/whisper.cpp/examples/whisper.swiftui/whisper.swiftui.demo/Models/WhisperState.swift
--rw-r--r--   0        0        0        0 2023-05-07 20:09:26.143948 whisper_cpp_python-0.1.6/whisper_cpp_python/vendor/whisper.cpp/examples/whisper.swiftui/whisper.swiftui.demo/Resources/models/.gitignore
--rw-r--r--   0        0        0        0 2023-05-07 20:09:26.144133 whisper_cpp_python-0.1.6/whisper_cpp_python/vendor/whisper.cpp/examples/whisper.swiftui/whisper.swiftui.demo/Resources/samples/.gitignore
--rw-r--r--   0        0        0      123 2023-05-07 20:09:26.144514 whisper_cpp_python-0.1.6/whisper_cpp_python/vendor/whisper.cpp/examples/whisper.swiftui/whisper.swiftui.demo/Supporting files/Assets.xcassets/AccentColor.colorset/Contents.json
--rw-r--r--   0        0        0      999 2023-05-07 20:09:26.144880 whisper_cpp_python-0.1.6/whisper_cpp_python/vendor/whisper.cpp/examples/whisper.swiftui/whisper.swiftui.demo/Supporting files/Assets.xcassets/AppIcon.appiconset/Contents.json
--rw-r--r--   0        0        0       63 2023-05-07 20:09:26.145224 whisper_cpp_python-0.1.6/whisper_cpp_python/vendor/whisper.cpp/examples/whisper.swiftui/whisper.swiftui.demo/Supporting files/Assets.xcassets/Contents.json
--rw-r--r--   0        0        0       63 2023-05-07 20:09:26.145639 whisper_cpp_python-0.1.6/whisper_cpp_python/vendor/whisper.cpp/examples/whisper.swiftui/whisper.swiftui.demo/Supporting files/Preview Content/Preview Assets.xcassets/Contents.json
--rw-r--r--   0        0        0      369 2023-05-07 20:09:26.145966 whisper_cpp_python-0.1.6/whisper_cpp_python/vendor/whisper.cpp/examples/whisper.swiftui/whisper.swiftui.demo/Supporting files/WhisperCppDemo.entitlements
--rw-r--r--   0        0        0     1323 2023-05-07 20:09:26.146205 whisper_cpp_python-0.1.6/whisper_cpp_python/vendor/whisper.cpp/examples/whisper.swiftui/whisper.swiftui.demo/UI/ContentView.swift
--rw-r--r--   0        0        0     1065 2023-05-07 20:09:26.146831 whisper_cpp_python-0.1.6/whisper_cpp_python/vendor/whisper.cpp/examples/whisper.swiftui/whisper.swiftui.demo/Utils/Recorder.swift
--rw-r--r--   0        0        0      394 2023-05-07 20:09:26.147120 whisper_cpp_python-0.1.6/whisper_cpp_python/vendor/whisper.cpp/examples/whisper.swiftui/whisper.swiftui.demo/Utils/RiffWaveUtils.swift
--rw-r--r--   0        0        0      147 2023-05-07 20:09:26.147802 whisper_cpp_python-0.1.6/whisper_cpp_python/vendor/whisper.cpp/examples/whisper.swiftui/whisper.swiftui.demo/WhisperCppDemoApp.swift
--rw-r--r--   0        0        0       12 2023-05-07 20:09:26.148208 whisper_cpp_python-0.1.6/whisper_cpp_python/vendor/whisper.cpp/examples/whisper.swiftui/whisper.swiftui.xcodeproj/.gitignore
--rw-r--r--   0        0        0    21447 2023-05-07 20:09:26.148513 whisper_cpp_python-0.1.6/whisper_cpp_python/vendor/whisper.cpp/examples/whisper.swiftui/whisper.swiftui.xcodeproj/project.pbxproj
--rw-r--r--   0        0        0       25 2023-05-07 20:09:26.148759 whisper_cpp_python-0.1.6/whisper_cpp_python/vendor/whisper.cpp/examples/whisper.swiftui/whisper.swiftui.xcodeproj/project.xcworkspace/.gitignore
--rw-r--r--   0        0        0      238 2023-05-07 20:09:26.149191 whisper_cpp_python-0.1.6/whisper_cpp_python/vendor/whisper.cpp/examples/whisper.swiftui/whisper.swiftui.xcodeproj/project.xcworkspace/xcshareddata/IDEWorkspaceChecks.plist
--rw-r--r--   0        0        0     3896 2023-05-07 20:09:26.149530 whisper_cpp_python-0.1.6/whisper_cpp_python/vendor/whisper.cpp/examples/whisper.swiftui/whisper.swiftui.xcodeproj/xcshareddata/xcschemes/WhisperCppDemo.xcscheme
--rw-r--r--   0        0        0     1162 2023-05-07 20:09:26.149751 whisper_cpp_python-0.1.6/whisper_cpp_python/vendor/whisper.cpp/examples/whisper.wasm/CMakeLists.txt
--rw-r--r--   0        0        0     1802 2023-05-07 20:09:26.149898 whisper_cpp_python-0.1.6/whisper_cpp_python/vendor/whisper.cpp/examples/whisper.wasm/README.md
--rw-r--r--   0        0        0     3614 2023-05-07 20:09:26.150057 whisper_cpp_python-0.1.6/whisper_cpp_python/vendor/whisper.cpp/examples/whisper.wasm/emscripten.cpp
--rw-r--r--   0        0        0    33017 2023-05-07 20:09:26.151045 whisper_cpp_python-0.1.6/whisper_cpp_python/vendor/whisper.cpp/examples/whisper.wasm/index-tmpl.html
--rwxr-xr-x   0        0        0     6932 2023-05-07 20:09:26.152061 whisper_cpp_python-0.1.6/whisper_cpp_python/vendor/whisper.cpp/examples/yt-wsp.sh
--rwxr-xr-x   0        0        0     2459 2023-05-07 20:09:26.152735 whisper_cpp_python-0.1.6/whisper_cpp_python/vendor/whisper.cpp/extra/bench-all.sh
--rwxr-xr-x   0        0        0     2113 2023-05-07 20:09:26.153224 whisper_cpp_python-0.1.6/whisper_cpp_python/vendor/whisper.cpp/extra/bench-wts.sh
--rwxr-xr-x   0        0        0      297 2023-05-07 20:09:26.153392 whisper_cpp_python-0.1.6/whisper_cpp_python/vendor/whisper.cpp/extra/convert-all.sh
--rwxr-xr-x   0        0        0     1152 2023-05-07 20:09:26.153529 whisper_cpp_python-0.1.6/whisper_cpp_python/vendor/whisper.cpp/extra/deploy-wasm.sh
--rwxr-xr-x   0        0        0     2034 2023-05-07 20:09:26.153656 whisper_cpp_python-0.1.6/whisper_cpp_python/vendor/whisper.cpp/extra/quantize-all.sh
--rwxr-xr-x   0        0        0      134 2023-05-07 20:09:26.153775 whisper_cpp_python-0.1.6/whisper_cpp_python/vendor/whisper.cpp/extra/sha-all.sh
--rwxr-xr-x   0        0        0      596 2023-05-07 20:09:26.153912 whisper_cpp_python-0.1.6/whisper_cpp_python/vendor/whisper.cpp/extra/sync-ggml.sh
--rw-r--r--   0        0        0    24594 2023-05-07 20:09:26.154162 whisper_cpp_python-0.1.6/whisper_cpp_python/vendor/whisper.cpp/ggml-cuda.cu
--rw-r--r--   0        0        0      638 2023-05-07 20:09:26.154401 whisper_cpp_python-0.1.6/whisper_cpp_python/vendor/whisper.cpp/ggml-cuda.h
--rw-r--r--   0        0        0    13447 2023-05-07 20:09:26.154811 whisper_cpp_python-0.1.6/whisper_cpp_python/vendor/whisper.cpp/ggml-opencl.c
--rw-r--r--   0        0        0      639 2023-05-07 20:09:26.154988 whisper_cpp_python-0.1.6/whisper_cpp_python/vendor/whisper.cpp/ggml-opencl.h
--rw-r--r--   0        0        0   423265 2023-05-07 20:09:26.158545 whisper_cpp_python-0.1.6/whisper_cpp_python/vendor/whisper.cpp/ggml.c
--rw-r--r--   0        0        0    31202 2023-05-07 20:09:26.158921 whisper_cpp_python-0.1.6/whisper_cpp_python/vendor/whisper.cpp/ggml.h
--rw-r--r--   0        0        0        6 2023-05-07 20:09:26.159128 whisper_cpp_python-0.1.6/whisper_cpp_python/vendor/whisper.cpp/models/.gitignore
--rw-r--r--   0        0        0     3290 2023-05-07 20:09:26.159290 whisper_cpp_python-0.1.6/whisper_cpp_python/vendor/whisper.cpp/models/README.md
--rw-r--r--   0        0        0     7376 2023-05-07 20:09:26.159623 whisper_cpp_python-0.1.6/whisper_cpp_python/vendor/whisper.cpp/models/convert-h5-to-ggml.py
--rw-r--r--   0        0        0     9473 2023-05-07 20:09:26.159819 whisper_cpp_python-0.1.6/whisper_cpp_python/vendor/whisper.cpp/models/convert-pt-to-ggml.py
--rw-r--r--   0        0        0    12853 2023-05-07 20:09:26.160372 whisper_cpp_python-0.1.6/whisper_cpp_python/vendor/whisper.cpp/models/convert-whisper-to-coreml.py
--rwxr-xr-x   0        0        0     2128 2023-05-07 20:09:26.160558 whisper_cpp_python-0.1.6/whisper_cpp_python/vendor/whisper.cpp/models/download-coreml-model.sh
--rw-r--r--   0        0        0     1356 2023-05-07 20:09:26.160707 whisper_cpp_python-0.1.6/whisper_cpp_python/vendor/whisper.cpp/models/download-ggml-model.cmd
--rwxr-xr-x   0        0        0     2010 2023-05-07 20:09:26.160867 whisper_cpp_python-0.1.6/whisper_cpp_python/vendor/whisper.cpp/models/download-ggml-model.sh
--rw-r--r--   0        0        0   575451 2023-05-07 20:09:26.167171 whisper_cpp_python-0.1.6/whisper_cpp_python/vendor/whisper.cpp/models/for-tests-ggml-base.bin
--rw-r--r--   0        0        0   586836 2023-05-07 20:09:26.172634 whisper_cpp_python-0.1.6/whisper_cpp_python/vendor/whisper.cpp/models/for-tests-ggml-base.en.bin
--rw-r--r--   0        0        0   575451 2023-05-07 20:09:26.174562 whisper_cpp_python-0.1.6/whisper_cpp_python/vendor/whisper.cpp/models/for-tests-ggml-large.bin
--rw-r--r--   0        0        0   575451 2023-05-07 20:09:26.176618 whisper_cpp_python-0.1.6/whisper_cpp_python/vendor/whisper.cpp/models/for-tests-ggml-medium.bin
--rw-r--r--   0        0        0   586836 2023-05-07 20:09:26.178801 whisper_cpp_python-0.1.6/whisper_cpp_python/vendor/whisper.cpp/models/for-tests-ggml-medium.en.bin
--rw-r--r--   0        0        0   575451 2023-05-07 20:09:26.180189 whisper_cpp_python-0.1.6/whisper_cpp_python/vendor/whisper.cpp/models/for-tests-ggml-small.bin
--rw-r--r--   0        0        0   586836 2023-05-07 20:09:26.181853 whisper_cpp_python-0.1.6/whisper_cpp_python/vendor/whisper.cpp/models/for-tests-ggml-small.en.bin
--rw-r--r--   0        0        0   575451 2023-05-07 20:09:26.184473 whisper_cpp_python-0.1.6/whisper_cpp_python/vendor/whisper.cpp/models/for-tests-ggml-tiny.bin
--rw-r--r--   0        0        0   586836 2023-05-07 20:09:26.187254 whisper_cpp_python-0.1.6/whisper_cpp_python/vendor/whisper.cpp/models/for-tests-ggml-tiny.en.bin
--rwxr-xr-x   0        0        0     1471 2023-05-07 20:09:26.188135 whisper_cpp_python-0.1.6/whisper_cpp_python/vendor/whisper.cpp/models/generate-coreml-interface.sh
--rwxr-xr-x   0        0        0      769 2023-05-07 20:09:26.188283 whisper_cpp_python-0.1.6/whisper_cpp_python/vendor/whisper.cpp/models/generate-coreml-model.sh
--rw-r--r--   0        0        0        2 2023-05-07 20:09:26.188474 whisper_cpp_python-0.1.6/whisper_cpp_python/vendor/whisper.cpp/samples/.gitignore
--rw-r--r--   0        0        0      367 2023-05-07 20:09:26.188597 whisper_cpp_python-0.1.6/whisper_cpp_python/vendor/whisper.cpp/samples/README.md
--rw-r--r--   0        0        0   352078 2023-05-07 20:09:26.191091 whisper_cpp_python-0.1.6/whisper_cpp_python/vendor/whisper.cpp/samples/jfk.wav
--rw-r--r--   0        0        0       22 2023-05-07 20:09:26.191418 whisper_cpp_python-0.1.6/whisper_cpp_python/vendor/whisper.cpp/tests/.gitignore
--rw-r--r--   0        0        0     2712 2023-05-07 20:09:26.191678 whisper_cpp_python-0.1.6/whisper_cpp_python/vendor/whisper.cpp/tests/CMakeLists.txt
--rw-r--r--   0        0        0     2101 2023-05-07 20:09:26.191809 whisper_cpp_python-0.1.6/whisper_cpp_python/vendor/whisper.cpp/tests/en-0-ref.txt
--rw-r--r--   0        0        0     2221 2023-05-07 20:09:26.191932 whisper_cpp_python-0.1.6/whisper_cpp_python/vendor/whisper.cpp/tests/en-1-ref.txt
--rw-r--r--   0        0        0      957 2023-05-07 20:09:26.192042 whisper_cpp_python-0.1.6/whisper_cpp_python/vendor/whisper.cpp/tests/en-2-ref.txt
--rw-r--r--   0        0        0     1945 2023-05-07 20:09:26.192157 whisper_cpp_python-0.1.6/whisper_cpp_python/vendor/whisper.cpp/tests/es-0-ref.txt
--rwxr-xr-x   0        0        0     3432 2023-05-07 20:09:26.192274 whisper_cpp_python-0.1.6/whisper_cpp_python/vendor/whisper.cpp/tests/run-tests.sh
--rw-r--r--   0        0        0     1645 2023-05-07 20:09:26.192389 whisper_cpp_python-0.1.6/whisper_cpp_python/vendor/whisper.cpp/tests/test-whisper.js
--rw-r--r--   0        0        0   184690 2023-05-07 20:09:26.193308 whisper_cpp_python-0.1.6/whisper_cpp_python/vendor/whisper.cpp/whisper.cpp
--rw-r--r--   0        0        0    23750 2023-05-07 20:09:26.193666 whisper_cpp_python-0.1.6/whisper_cpp_python/vendor/whisper.cpp/whisper.h
--rw-r--r--   0        0        0     1366 2023-05-07 19:25:03.713447 whisper_cpp_python-0.1.6/whisper_cpp_python/whisper.py
--rw-r--r--   0        0        0      457 1970-01-01 00:00:00.000000 whisper_cpp_python-0.1.6/PKG-INFO
+drwxrwxr-x   0 carlos    (1000) carlos    (1000)        0 2023-05-08 18:17:25.330170 whisper_cpp_python-0.1.7/
+-rw-rw-r--   0 carlos    (1000) carlos    (1000)      350 2023-05-08 17:45:44.000000 whisper_cpp_python-0.1.7/CMakeLists.txt
+-rw-rw-r--   0 carlos    (1000) carlos    (1000)      447 2023-05-08 18:17:25.330170 whisper_cpp_python-0.1.7/PKG-INFO
+-rw-rw-r--   0 carlos    (1000) carlos    (1000)        0 2023-05-08 13:27:07.000000 whisper_cpp_python-0.1.7/README.md
+-rw-rw-r--   0 carlos    (1000) carlos    (1000)      602 2023-05-08 17:58:01.000000 whisper_cpp_python-0.1.7/pyproject.toml
+-rw-rw-r--   0 carlos    (1000) carlos    (1000)       38 2023-05-08 18:17:25.330170 whisper_cpp_python-0.1.7/setup.cfg
+-rw-rw-r--   0 carlos    (1000) carlos    (1000)     8551 2023-05-08 18:16:02.000000 whisper_cpp_python-0.1.7/setup.py
+drwxrwxr-x   0 carlos    (1000) carlos    (1000)        0 2023-05-08 18:17:25.274168 whisper_cpp_python-0.1.7/tests/
+-rw-rw-r--   0 carlos    (1000) carlos    (1000)      161 2023-05-08 13:30:10.000000 whisper_cpp_python-0.1.7/tests/test.py
+drwxrwxr-x   0 carlos    (1000) carlos    (1000)        0 2023-05-08 18:17:25.266168 whisper_cpp_python-0.1.7/vendor/
+drwxrwxr-x   0 carlos    (1000) carlos    (1000)        0 2023-05-08 18:17:25.266168 whisper_cpp_python-0.1.7/vendor/pycparser/
+drwxrwxr-x   0 carlos    (1000) carlos    (1000)        0 2023-05-08 18:17:25.266168 whisper_cpp_python-0.1.7/vendor/pycparser/utils/
+drwxrwxr-x   0 carlos    (1000) carlos    (1000)        0 2023-05-08 18:17:25.286168 whisper_cpp_python-0.1.7/vendor/pycparser/utils/fake_libc_include/
+drwxrwxr-x   0 carlos    (1000) carlos    (1000)        0 2023-05-08 18:17:25.286168 whisper_cpp_python-0.1.7/vendor/pycparser/utils/fake_libc_include/X11/
+-rw-rw-r--   0 carlos    (1000) carlos    (1000)      118 2023-05-08 13:31:02.000000 whisper_cpp_python-0.1.7/vendor/pycparser/utils/fake_libc_include/X11/Intrinsic.h
+-rw-rw-r--   0 carlos    (1000) carlos    (1000)      118 2023-05-08 13:31:02.000000 whisper_cpp_python-0.1.7/vendor/pycparser/utils/fake_libc_include/X11/Xlib.h
+-rw-rw-r--   0 carlos    (1000) carlos    (1000)      311 2023-05-08 13:31:02.000000 whisper_cpp_python-0.1.7/vendor/pycparser/utils/fake_libc_include/X11/_X11_fake_defines.h
+-rw-rw-r--   0 carlos    (1000) carlos    (1000)     1111 2023-05-08 13:31:02.000000 whisper_cpp_python-0.1.7/vendor/pycparser/utils/fake_libc_include/X11/_X11_fake_typedefs.h
+-rw-rw-r--   0 carlos    (1000) carlos    (1000)       55 2023-05-08 13:31:02.000000 whisper_cpp_python-0.1.7/vendor/pycparser/utils/fake_libc_include/_ansi.h
+-rw-rw-r--   0 carlos    (1000) carlos    (1000)     5921 2023-05-08 13:31:02.000000 whisper_cpp_python-0.1.7/vendor/pycparser/utils/fake_libc_include/_fake_defines.h
+-rw-rw-r--   0 carlos    (1000) carlos    (1000)     6547 2023-05-08 13:31:02.000000 whisper_cpp_python-0.1.7/vendor/pycparser/utils/fake_libc_include/_fake_typedefs.h
+-rw-rw-r--   0 carlos    (1000) carlos    (1000)       55 2023-05-08 13:31:02.000000 whisper_cpp_python-0.1.7/vendor/pycparser/utils/fake_libc_include/_syslist.h
+-rw-rw-r--   0 carlos    (1000) carlos    (1000)       55 2023-05-08 13:31:02.000000 whisper_cpp_python-0.1.7/vendor/pycparser/utils/fake_libc_include/aio.h
+-rw-rw-r--   0 carlos    (1000) carlos    (1000)       55 2023-05-08 13:31:02.000000 whisper_cpp_python-0.1.7/vendor/pycparser/utils/fake_libc_include/alloca.h
+-rw-rw-r--   0 carlos    (1000) carlos    (1000)       55 2023-05-08 13:31:02.000000 whisper_cpp_python-0.1.7/vendor/pycparser/utils/fake_libc_include/ar.h
+-rw-rw-r--   0 carlos    (1000) carlos    (1000)       55 2023-05-08 13:31:02.000000 whisper_cpp_python-0.1.7/vendor/pycparser/utils/fake_libc_include/argz.h
+drwxrwxr-x   0 carlos    (1000) carlos    (1000)        0 2023-05-08 18:17:25.286168 whisper_cpp_python-0.1.7/vendor/pycparser/utils/fake_libc_include/arpa/
+-rw-rw-r--   0 carlos    (1000) carlos    (1000)       55 2023-05-08 13:31:02.000000 whisper_cpp_python-0.1.7/vendor/pycparser/utils/fake_libc_include/arpa/inet.h
+drwxrwxr-x   0 carlos    (1000) carlos    (1000)        0 2023-05-08 18:17:25.286168 whisper_cpp_python-0.1.7/vendor/pycparser/utils/fake_libc_include/asm-generic/
+-rw-rw-r--   0 carlos    (1000) carlos    (1000)       55 2023-05-08 13:31:02.000000 whisper_cpp_python-0.1.7/vendor/pycparser/utils/fake_libc_include/asm-generic/int-ll64.h
+-rw-rw-r--   0 carlos    (1000) carlos    (1000)       55 2023-05-08 13:31:02.000000 whisper_cpp_python-0.1.7/vendor/pycparser/utils/fake_libc_include/assert.h
+-rw-rw-r--   0 carlos    (1000) carlos    (1000)       55 2023-05-08 13:31:02.000000 whisper_cpp_python-0.1.7/vendor/pycparser/utils/fake_libc_include/complex.h
+-rw-rw-r--   0 carlos    (1000) carlos    (1000)       55 2023-05-08 13:31:02.000000 whisper_cpp_python-0.1.7/vendor/pycparser/utils/fake_libc_include/cpio.h
+-rw-rw-r--   0 carlos    (1000) carlos    (1000)       55 2023-05-08 13:31:02.000000 whisper_cpp_python-0.1.7/vendor/pycparser/utils/fake_libc_include/ctype.h
+-rw-rw-r--   0 carlos    (1000) carlos    (1000)       55 2023-05-08 13:31:02.000000 whisper_cpp_python-0.1.7/vendor/pycparser/utils/fake_libc_include/dirent.h
+-rw-rw-r--   0 carlos    (1000) carlos    (1000)       55 2023-05-08 13:31:02.000000 whisper_cpp_python-0.1.7/vendor/pycparser/utils/fake_libc_include/dlfcn.h
+-rw-rw-r--   0 carlos    (1000) carlos    (1000)       55 2023-05-08 13:31:02.000000 whisper_cpp_python-0.1.7/vendor/pycparser/utils/fake_libc_include/emmintrin.h
+-rw-rw-r--   0 carlos    (1000) carlos    (1000)       55 2023-05-08 13:31:02.000000 whisper_cpp_python-0.1.7/vendor/pycparser/utils/fake_libc_include/endian.h
+-rw-rw-r--   0 carlos    (1000) carlos    (1000)       55 2023-05-08 13:31:02.000000 whisper_cpp_python-0.1.7/vendor/pycparser/utils/fake_libc_include/envz.h
+-rw-rw-r--   0 carlos    (1000) carlos    (1000)       55 2023-05-08 13:31:02.000000 whisper_cpp_python-0.1.7/vendor/pycparser/utils/fake_libc_include/errno.h
+-rw-rw-r--   0 carlos    (1000) carlos    (1000)       55 2023-05-08 13:31:02.000000 whisper_cpp_python-0.1.7/vendor/pycparser/utils/fake_libc_include/fastmath.h
+-rw-rw-r--   0 carlos    (1000) carlos    (1000)       55 2023-05-08 13:31:02.000000 whisper_cpp_python-0.1.7/vendor/pycparser/utils/fake_libc_include/fcntl.h
+-rw-rw-r--   0 carlos    (1000) carlos    (1000)       55 2023-05-08 13:31:02.000000 whisper_cpp_python-0.1.7/vendor/pycparser/utils/fake_libc_include/features.h
+-rw-rw-r--   0 carlos    (1000) carlos    (1000)       55 2023-05-08 13:31:02.000000 whisper_cpp_python-0.1.7/vendor/pycparser/utils/fake_libc_include/fenv.h
+-rw-rw-r--   0 carlos    (1000) carlos    (1000)       55 2023-05-08 13:31:02.000000 whisper_cpp_python-0.1.7/vendor/pycparser/utils/fake_libc_include/float.h
+-rw-rw-r--   0 carlos    (1000) carlos    (1000)       55 2023-05-08 13:31:02.000000 whisper_cpp_python-0.1.7/vendor/pycparser/utils/fake_libc_include/fmtmsg.h
+-rw-rw-r--   0 carlos    (1000) carlos    (1000)       55 2023-05-08 13:31:02.000000 whisper_cpp_python-0.1.7/vendor/pycparser/utils/fake_libc_include/fnmatch.h
+-rw-rw-r--   0 carlos    (1000) carlos    (1000)       55 2023-05-08 13:31:02.000000 whisper_cpp_python-0.1.7/vendor/pycparser/utils/fake_libc_include/ftw.h
+-rw-rw-r--   0 carlos    (1000) carlos    (1000)       55 2023-05-08 13:31:02.000000 whisper_cpp_python-0.1.7/vendor/pycparser/utils/fake_libc_include/getopt.h
+-rw-rw-r--   0 carlos    (1000) carlos    (1000)       55 2023-05-08 13:31:02.000000 whisper_cpp_python-0.1.7/vendor/pycparser/utils/fake_libc_include/glob.h
+-rw-rw-r--   0 carlos    (1000) carlos    (1000)       55 2023-05-08 13:31:02.000000 whisper_cpp_python-0.1.7/vendor/pycparser/utils/fake_libc_include/grp.h
+-rw-rw-r--   0 carlos    (1000) carlos    (1000)       55 2023-05-08 13:31:02.000000 whisper_cpp_python-0.1.7/vendor/pycparser/utils/fake_libc_include/iconv.h
+-rw-rw-r--   0 carlos    (1000) carlos    (1000)       55 2023-05-08 13:31:02.000000 whisper_cpp_python-0.1.7/vendor/pycparser/utils/fake_libc_include/ieeefp.h
+-rw-rw-r--   0 carlos    (1000) carlos    (1000)       55 2023-05-08 13:31:02.000000 whisper_cpp_python-0.1.7/vendor/pycparser/utils/fake_libc_include/immintrin.h
+-rw-rw-r--   0 carlos    (1000) carlos    (1000)       55 2023-05-08 13:31:02.000000 whisper_cpp_python-0.1.7/vendor/pycparser/utils/fake_libc_include/inttypes.h
+-rw-rw-r--   0 carlos    (1000) carlos    (1000)       55 2023-05-08 13:31:02.000000 whisper_cpp_python-0.1.7/vendor/pycparser/utils/fake_libc_include/iso646.h
+-rw-rw-r--   0 carlos    (1000) carlos    (1000)       55 2023-05-08 13:31:02.000000 whisper_cpp_python-0.1.7/vendor/pycparser/utils/fake_libc_include/langinfo.h
+-rw-rw-r--   0 carlos    (1000) carlos    (1000)       55 2023-05-08 13:31:02.000000 whisper_cpp_python-0.1.7/vendor/pycparser/utils/fake_libc_include/libgen.h
+-rw-rw-r--   0 carlos    (1000) carlos    (1000)       55 2023-05-08 13:31:02.000000 whisper_cpp_python-0.1.7/vendor/pycparser/utils/fake_libc_include/libintl.h
+-rw-rw-r--   0 carlos    (1000) carlos    (1000)       55 2023-05-08 13:31:02.000000 whisper_cpp_python-0.1.7/vendor/pycparser/utils/fake_libc_include/limits.h
+drwxrwxr-x   0 carlos    (1000) carlos    (1000)        0 2023-05-08 18:17:25.286168 whisper_cpp_python-0.1.7/vendor/pycparser/utils/fake_libc_include/linux/
+-rw-rw-r--   0 carlos    (1000) carlos    (1000)       55 2023-05-08 13:31:02.000000 whisper_cpp_python-0.1.7/vendor/pycparser/utils/fake_libc_include/linux/socket.h
+-rw-rw-r--   0 carlos    (1000) carlos    (1000)       55 2023-05-08 13:31:02.000000 whisper_cpp_python-0.1.7/vendor/pycparser/utils/fake_libc_include/linux/version.h
+-rw-rw-r--   0 carlos    (1000) carlos    (1000)       55 2023-05-08 13:31:02.000000 whisper_cpp_python-0.1.7/vendor/pycparser/utils/fake_libc_include/locale.h
+-rw-rw-r--   0 carlos    (1000) carlos    (1000)       55 2023-05-08 13:31:02.000000 whisper_cpp_python-0.1.7/vendor/pycparser/utils/fake_libc_include/malloc.h
+-rw-rw-r--   0 carlos    (1000) carlos    (1000)       55 2023-05-08 13:31:02.000000 whisper_cpp_python-0.1.7/vendor/pycparser/utils/fake_libc_include/math.h
+drwxrwxr-x   0 carlos    (1000) carlos    (1000)        0 2023-05-08 18:17:25.286168 whisper_cpp_python-0.1.7/vendor/pycparser/utils/fake_libc_include/mir_toolkit/
+-rw-rw-r--   0 carlos    (1000) carlos    (1000)       55 2023-05-08 13:31:02.000000 whisper_cpp_python-0.1.7/vendor/pycparser/utils/fake_libc_include/mir_toolkit/client_types.h
+-rw-rw-r--   0 carlos    (1000) carlos    (1000)       55 2023-05-08 13:31:02.000000 whisper_cpp_python-0.1.7/vendor/pycparser/utils/fake_libc_include/monetary.h
+-rw-rw-r--   0 carlos    (1000) carlos    (1000)       55 2023-05-08 13:31:02.000000 whisper_cpp_python-0.1.7/vendor/pycparser/utils/fake_libc_include/mqueue.h
+-rw-rw-r--   0 carlos    (1000) carlos    (1000)       55 2023-05-08 13:31:02.000000 whisper_cpp_python-0.1.7/vendor/pycparser/utils/fake_libc_include/ndbm.h
+drwxrwxr-x   0 carlos    (1000) carlos    (1000)        0 2023-05-08 18:17:25.286168 whisper_cpp_python-0.1.7/vendor/pycparser/utils/fake_libc_include/net/
+-rw-rw-r--   0 carlos    (1000) carlos    (1000)       55 2023-05-08 13:31:02.000000 whisper_cpp_python-0.1.7/vendor/pycparser/utils/fake_libc_include/net/if.h
+-rw-rw-r--   0 carlos    (1000) carlos    (1000)       55 2023-05-08 13:31:02.000000 whisper_cpp_python-0.1.7/vendor/pycparser/utils/fake_libc_include/netdb.h
+drwxrwxr-x   0 carlos    (1000) carlos    (1000)        0 2023-05-08 18:17:25.286168 whisper_cpp_python-0.1.7/vendor/pycparser/utils/fake_libc_include/netinet/
+-rw-rw-r--   0 carlos    (1000) carlos    (1000)       55 2023-05-08 13:31:02.000000 whisper_cpp_python-0.1.7/vendor/pycparser/utils/fake_libc_include/netinet/in.h
+-rw-rw-r--   0 carlos    (1000) carlos    (1000)       55 2023-05-08 13:31:02.000000 whisper_cpp_python-0.1.7/vendor/pycparser/utils/fake_libc_include/netinet/tcp.h
+-rw-rw-r--   0 carlos    (1000) carlos    (1000)       55 2023-05-08 13:31:02.000000 whisper_cpp_python-0.1.7/vendor/pycparser/utils/fake_libc_include/newlib.h
+-rw-rw-r--   0 carlos    (1000) carlos    (1000)       55 2023-05-08 13:31:02.000000 whisper_cpp_python-0.1.7/vendor/pycparser/utils/fake_libc_include/nl_types.h
+drwxrwxr-x   0 carlos    (1000) carlos    (1000)        0 2023-05-08 18:17:25.286168 whisper_cpp_python-0.1.7/vendor/pycparser/utils/fake_libc_include/openssl/
+-rw-rw-r--   0 carlos    (1000) carlos    (1000)       55 2023-05-08 13:31:02.000000 whisper_cpp_python-0.1.7/vendor/pycparser/utils/fake_libc_include/openssl/err.h
+-rw-rw-r--   0 carlos    (1000) carlos    (1000)       55 2023-05-08 13:31:02.000000 whisper_cpp_python-0.1.7/vendor/pycparser/utils/fake_libc_include/openssl/evp.h
+-rw-rw-r--   0 carlos    (1000) carlos    (1000)       55 2023-05-08 13:31:02.000000 whisper_cpp_python-0.1.7/vendor/pycparser/utils/fake_libc_include/openssl/hmac.h
+-rw-rw-r--   0 carlos    (1000) carlos    (1000)       55 2023-05-08 13:31:02.000000 whisper_cpp_python-0.1.7/vendor/pycparser/utils/fake_libc_include/openssl/ssl.h
+-rw-rw-r--   0 carlos    (1000) carlos    (1000)       55 2023-05-08 13:31:02.000000 whisper_cpp_python-0.1.7/vendor/pycparser/utils/fake_libc_include/openssl/x509v3.h
+-rw-rw-r--   0 carlos    (1000) carlos    (1000)       55 2023-05-08 13:31:02.000000 whisper_cpp_python-0.1.7/vendor/pycparser/utils/fake_libc_include/paths.h
+-rw-rw-r--   0 carlos    (1000) carlos    (1000)       55 2023-05-08 13:31:02.000000 whisper_cpp_python-0.1.7/vendor/pycparser/utils/fake_libc_include/poll.h
+-rw-rw-r--   0 carlos    (1000) carlos    (1000)       55 2023-05-08 13:31:02.000000 whisper_cpp_python-0.1.7/vendor/pycparser/utils/fake_libc_include/process.h
+-rw-rw-r--   0 carlos    (1000) carlos    (1000)       55 2023-05-08 13:31:02.000000 whisper_cpp_python-0.1.7/vendor/pycparser/utils/fake_libc_include/pthread.h
+-rw-rw-r--   0 carlos    (1000) carlos    (1000)       55 2023-05-08 13:31:02.000000 whisper_cpp_python-0.1.7/vendor/pycparser/utils/fake_libc_include/pwd.h
+-rw-rw-r--   0 carlos    (1000) carlos    (1000)       55 2023-05-08 13:31:02.000000 whisper_cpp_python-0.1.7/vendor/pycparser/utils/fake_libc_include/reent.h
+-rw-rw-r--   0 carlos    (1000) carlos    (1000)       55 2023-05-08 13:31:02.000000 whisper_cpp_python-0.1.7/vendor/pycparser/utils/fake_libc_include/regdef.h
+-rw-rw-r--   0 carlos    (1000) carlos    (1000)       55 2023-05-08 13:31:02.000000 whisper_cpp_python-0.1.7/vendor/pycparser/utils/fake_libc_include/regex.h
+-rw-rw-r--   0 carlos    (1000) carlos    (1000)       55 2023-05-08 13:31:02.000000 whisper_cpp_python-0.1.7/vendor/pycparser/utils/fake_libc_include/sched.h
+-rw-rw-r--   0 carlos    (1000) carlos    (1000)       55 2023-05-08 13:31:02.000000 whisper_cpp_python-0.1.7/vendor/pycparser/utils/fake_libc_include/search.h
+-rw-rw-r--   0 carlos    (1000) carlos    (1000)       55 2023-05-08 13:31:02.000000 whisper_cpp_python-0.1.7/vendor/pycparser/utils/fake_libc_include/semaphore.h
+-rw-rw-r--   0 carlos    (1000) carlos    (1000)       55 2023-05-08 13:31:02.000000 whisper_cpp_python-0.1.7/vendor/pycparser/utils/fake_libc_include/setjmp.h
+-rw-rw-r--   0 carlos    (1000) carlos    (1000)       55 2023-05-08 13:31:02.000000 whisper_cpp_python-0.1.7/vendor/pycparser/utils/fake_libc_include/signal.h
+-rw-rw-r--   0 carlos    (1000) carlos    (1000)       55 2023-05-08 13:31:02.000000 whisper_cpp_python-0.1.7/vendor/pycparser/utils/fake_libc_include/smmintrin.h
+-rw-rw-r--   0 carlos    (1000) carlos    (1000)       55 2023-05-08 13:31:02.000000 whisper_cpp_python-0.1.7/vendor/pycparser/utils/fake_libc_include/spawn.h
+-rw-rw-r--   0 carlos    (1000) carlos    (1000)       55 2023-05-08 13:31:02.000000 whisper_cpp_python-0.1.7/vendor/pycparser/utils/fake_libc_include/stdalign.h
+-rw-rw-r--   0 carlos    (1000) carlos    (1000)       55 2023-05-08 13:31:02.000000 whisper_cpp_python-0.1.7/vendor/pycparser/utils/fake_libc_include/stdarg.h
+-rw-rw-r--   0 carlos    (1000) carlos    (1000)       55 2023-05-08 13:31:02.000000 whisper_cpp_python-0.1.7/vendor/pycparser/utils/fake_libc_include/stdatomic.h
+-rw-rw-r--   0 carlos    (1000) carlos    (1000)       55 2023-05-08 13:31:02.000000 whisper_cpp_python-0.1.7/vendor/pycparser/utils/fake_libc_include/stdbool.h
+-rw-rw-r--   0 carlos    (1000) carlos    (1000)       55 2023-05-08 13:31:02.000000 whisper_cpp_python-0.1.7/vendor/pycparser/utils/fake_libc_include/stddef.h
+-rw-rw-r--   0 carlos    (1000) carlos    (1000)       55 2023-05-08 13:31:02.000000 whisper_cpp_python-0.1.7/vendor/pycparser/utils/fake_libc_include/stdint.h
+-rw-rw-r--   0 carlos    (1000) carlos    (1000)       55 2023-05-08 13:31:02.000000 whisper_cpp_python-0.1.7/vendor/pycparser/utils/fake_libc_include/stdio.h
+-rw-rw-r--   0 carlos    (1000) carlos    (1000)       55 2023-05-08 13:31:02.000000 whisper_cpp_python-0.1.7/vendor/pycparser/utils/fake_libc_include/stdlib.h
+-rw-rw-r--   0 carlos    (1000) carlos    (1000)       55 2023-05-08 13:31:02.000000 whisper_cpp_python-0.1.7/vendor/pycparser/utils/fake_libc_include/stdnoreturn.h
+-rw-rw-r--   0 carlos    (1000) carlos    (1000)       55 2023-05-08 13:31:02.000000 whisper_cpp_python-0.1.7/vendor/pycparser/utils/fake_libc_include/string.h
+-rw-rw-r--   0 carlos    (1000) carlos    (1000)       55 2023-05-08 13:31:02.000000 whisper_cpp_python-0.1.7/vendor/pycparser/utils/fake_libc_include/strings.h
+-rw-rw-r--   0 carlos    (1000) carlos    (1000)       55 2023-05-08 13:31:02.000000 whisper_cpp_python-0.1.7/vendor/pycparser/utils/fake_libc_include/stropts.h
+drwxrwxr-x   0 carlos    (1000) carlos    (1000)        0 2023-05-08 18:17:25.290169 whisper_cpp_python-0.1.7/vendor/pycparser/utils/fake_libc_include/sys/
+-rw-rw-r--   0 carlos    (1000) carlos    (1000)       55 2023-05-08 13:31:02.000000 whisper_cpp_python-0.1.7/vendor/pycparser/utils/fake_libc_include/sys/ioctl.h
+-rw-rw-r--   0 carlos    (1000) carlos    (1000)       55 2023-05-08 13:31:02.000000 whisper_cpp_python-0.1.7/vendor/pycparser/utils/fake_libc_include/sys/ipc.h
+-rw-rw-r--   0 carlos    (1000) carlos    (1000)       55 2023-05-08 13:31:02.000000 whisper_cpp_python-0.1.7/vendor/pycparser/utils/fake_libc_include/sys/mman.h
+-rw-rw-r--   0 carlos    (1000) carlos    (1000)       55 2023-05-08 13:31:02.000000 whisper_cpp_python-0.1.7/vendor/pycparser/utils/fake_libc_include/sys/msg.h
+-rw-rw-r--   0 carlos    (1000) carlos    (1000)       55 2023-05-08 13:31:02.000000 whisper_cpp_python-0.1.7/vendor/pycparser/utils/fake_libc_include/sys/poll.h
+-rw-rw-r--   0 carlos    (1000) carlos    (1000)       55 2023-05-08 13:31:02.000000 whisper_cpp_python-0.1.7/vendor/pycparser/utils/fake_libc_include/sys/resource.h
+-rw-rw-r--   0 carlos    (1000) carlos    (1000)       55 2023-05-08 13:31:02.000000 whisper_cpp_python-0.1.7/vendor/pycparser/utils/fake_libc_include/sys/select.h
+-rw-rw-r--   0 carlos    (1000) carlos    (1000)       55 2023-05-08 13:31:02.000000 whisper_cpp_python-0.1.7/vendor/pycparser/utils/fake_libc_include/sys/sem.h
+-rw-rw-r--   0 carlos    (1000) carlos    (1000)       55 2023-05-08 13:31:02.000000 whisper_cpp_python-0.1.7/vendor/pycparser/utils/fake_libc_include/sys/shm.h
+-rw-rw-r--   0 carlos    (1000) carlos    (1000)       55 2023-05-08 13:31:02.000000 whisper_cpp_python-0.1.7/vendor/pycparser/utils/fake_libc_include/sys/socket.h
+-rw-rw-r--   0 carlos    (1000) carlos    (1000)       55 2023-05-08 13:31:02.000000 whisper_cpp_python-0.1.7/vendor/pycparser/utils/fake_libc_include/sys/stat.h
+-rw-rw-r--   0 carlos    (1000) carlos    (1000)       55 2023-05-08 13:31:02.000000 whisper_cpp_python-0.1.7/vendor/pycparser/utils/fake_libc_include/sys/statvfs.h
+-rw-rw-r--   0 carlos    (1000) carlos    (1000)       55 2023-05-08 13:31:02.000000 whisper_cpp_python-0.1.7/vendor/pycparser/utils/fake_libc_include/sys/sysctl.h
+-rw-rw-r--   0 carlos    (1000) carlos    (1000)       55 2023-05-08 13:31:02.000000 whisper_cpp_python-0.1.7/vendor/pycparser/utils/fake_libc_include/sys/time.h
+-rw-rw-r--   0 carlos    (1000) carlos    (1000)       55 2023-05-08 13:31:02.000000 whisper_cpp_python-0.1.7/vendor/pycparser/utils/fake_libc_include/sys/times.h
+-rw-rw-r--   0 carlos    (1000) carlos    (1000)       55 2023-05-08 13:31:02.000000 whisper_cpp_python-0.1.7/vendor/pycparser/utils/fake_libc_include/sys/types.h
+-rw-rw-r--   0 carlos    (1000) carlos    (1000)       55 2023-05-08 13:31:02.000000 whisper_cpp_python-0.1.7/vendor/pycparser/utils/fake_libc_include/sys/uio.h
+-rw-rw-r--   0 carlos    (1000) carlos    (1000)       55 2023-05-08 13:31:02.000000 whisper_cpp_python-0.1.7/vendor/pycparser/utils/fake_libc_include/sys/un.h
+-rw-rw-r--   0 carlos    (1000) carlos    (1000)       55 2023-05-08 13:31:02.000000 whisper_cpp_python-0.1.7/vendor/pycparser/utils/fake_libc_include/sys/utsname.h
+-rw-rw-r--   0 carlos    (1000) carlos    (1000)       55 2023-05-08 13:31:02.000000 whisper_cpp_python-0.1.7/vendor/pycparser/utils/fake_libc_include/sys/wait.h
+-rw-rw-r--   0 carlos    (1000) carlos    (1000)       55 2023-05-08 13:31:02.000000 whisper_cpp_python-0.1.7/vendor/pycparser/utils/fake_libc_include/syslog.h
+-rw-rw-r--   0 carlos    (1000) carlos    (1000)       55 2023-05-08 13:31:02.000000 whisper_cpp_python-0.1.7/vendor/pycparser/utils/fake_libc_include/tar.h
+-rw-rw-r--   0 carlos    (1000) carlos    (1000)       55 2023-05-08 13:31:02.000000 whisper_cpp_python-0.1.7/vendor/pycparser/utils/fake_libc_include/termios.h
+-rw-rw-r--   0 carlos    (1000) carlos    (1000)       55 2023-05-08 13:31:02.000000 whisper_cpp_python-0.1.7/vendor/pycparser/utils/fake_libc_include/tgmath.h
+-rw-rw-r--   0 carlos    (1000) carlos    (1000)       55 2023-05-08 13:31:02.000000 whisper_cpp_python-0.1.7/vendor/pycparser/utils/fake_libc_include/threads.h
+-rw-rw-r--   0 carlos    (1000) carlos    (1000)       55 2023-05-08 13:31:02.000000 whisper_cpp_python-0.1.7/vendor/pycparser/utils/fake_libc_include/time.h
+-rw-rw-r--   0 carlos    (1000) carlos    (1000)       55 2023-05-08 13:31:02.000000 whisper_cpp_python-0.1.7/vendor/pycparser/utils/fake_libc_include/trace.h
+-rw-rw-r--   0 carlos    (1000) carlos    (1000)       55 2023-05-08 13:31:02.000000 whisper_cpp_python-0.1.7/vendor/pycparser/utils/fake_libc_include/ulimit.h
+-rw-rw-r--   0 carlos    (1000) carlos    (1000)       55 2023-05-08 13:31:02.000000 whisper_cpp_python-0.1.7/vendor/pycparser/utils/fake_libc_include/unctrl.h
+-rw-rw-r--   0 carlos    (1000) carlos    (1000)       55 2023-05-08 13:31:02.000000 whisper_cpp_python-0.1.7/vendor/pycparser/utils/fake_libc_include/unistd.h
+-rw-rw-r--   0 carlos    (1000) carlos    (1000)       55 2023-05-08 13:31:02.000000 whisper_cpp_python-0.1.7/vendor/pycparser/utils/fake_libc_include/utime.h
+-rw-rw-r--   0 carlos    (1000) carlos    (1000)       55 2023-05-08 13:31:02.000000 whisper_cpp_python-0.1.7/vendor/pycparser/utils/fake_libc_include/utmp.h
+-rw-rw-r--   0 carlos    (1000) carlos    (1000)       55 2023-05-08 13:31:02.000000 whisper_cpp_python-0.1.7/vendor/pycparser/utils/fake_libc_include/utmpx.h
+-rw-rw-r--   0 carlos    (1000) carlos    (1000)       55 2023-05-08 13:31:02.000000 whisper_cpp_python-0.1.7/vendor/pycparser/utils/fake_libc_include/wchar.h
+-rw-rw-r--   0 carlos    (1000) carlos    (1000)       55 2023-05-08 13:31:02.000000 whisper_cpp_python-0.1.7/vendor/pycparser/utils/fake_libc_include/wctype.h
+-rw-rw-r--   0 carlos    (1000) carlos    (1000)       55 2023-05-08 13:31:02.000000 whisper_cpp_python-0.1.7/vendor/pycparser/utils/fake_libc_include/wordexp.h
+drwxrwxr-x   0 carlos    (1000) carlos    (1000)        0 2023-05-08 18:17:25.290169 whisper_cpp_python-0.1.7/vendor/pycparser/utils/fake_libc_include/xcb/
+-rw-rw-r--   0 carlos    (1000) carlos    (1000)       55 2023-05-08 13:31:02.000000 whisper_cpp_python-0.1.7/vendor/pycparser/utils/fake_libc_include/xcb/xcb.h
+-rw-rw-r--   0 carlos    (1000) carlos    (1000)      514 2023-05-08 13:31:02.000000 whisper_cpp_python-0.1.7/vendor/pycparser/utils/fake_libc_include/zlib.h
+drwxrwxr-x   0 carlos    (1000) carlos    (1000)        0 2023-05-08 18:17:25.290169 whisper_cpp_python-0.1.7/vendor/whisper.cpp/
+drwxrwxr-x   0 carlos    (1000) carlos    (1000)        0 2023-05-08 18:17:25.266168 whisper_cpp_python-0.1.7/vendor/whisper.cpp/.github/
+drwxrwxr-x   0 carlos    (1000) carlos    (1000)        0 2023-05-08 18:17:25.290169 whisper_cpp_python-0.1.7/vendor/whisper.cpp/.github/workflows/
+-rw-rw-r--   0 carlos    (1000) carlos    (1000)      392 2023-05-08 13:31:02.000000 whisper_cpp_python-0.1.7/vendor/whisper.cpp/.github/workflows/bindings-go.yml
+-rw-rw-r--   0 carlos    (1000) carlos    (1000)      417 2023-05-08 13:31:02.000000 whisper_cpp_python-0.1.7/vendor/whisper.cpp/.github/workflows/bindings-ruby.yml
+-rw-rw-r--   0 carlos    (1000) carlos    (1000)     9896 2023-05-08 13:31:02.000000 whisper_cpp_python-0.1.7/vendor/whisper.cpp/.github/workflows/build.yml
+-rw-rw-r--   0 carlos    (1000) carlos    (1000)     1153 2023-05-08 13:31:02.000000 whisper_cpp_python-0.1.7/vendor/whisper.cpp/.github/workflows/examples.yml
+-rw-rw-r--   0 carlos    (1000) carlos    (1000)      605 2023-05-08 13:31:02.000000 whisper_cpp_python-0.1.7/vendor/whisper.cpp/.gitignore
+-rw-rw-r--   0 carlos    (1000) carlos    (1000)       96 2023-05-08 13:31:02.000000 whisper_cpp_python-0.1.7/vendor/whisper.cpp/.gitmodules
+-rw-rw-r--   0 carlos    (1000) carlos    (1000)    10866 2023-05-08 13:31:02.000000 whisper_cpp_python-0.1.7/vendor/whisper.cpp/CMakeLists.txt
+-rw-rw-r--   0 carlos    (1000) carlos    (1000)     1072 2023-05-08 13:31:02.000000 whisper_cpp_python-0.1.7/vendor/whisper.cpp/LICENSE
+-rw-rw-r--   0 carlos    (1000) carlos    (1000)    11058 2023-05-08 13:31:02.000000 whisper_cpp_python-0.1.7/vendor/whisper.cpp/Makefile
+-rw-rw-r--   0 carlos    (1000) carlos    (1000)    28943 2023-05-08 13:31:02.000000 whisper_cpp_python-0.1.7/vendor/whisper.cpp/README.md
+drwxrwxr-x   0 carlos    (1000) carlos    (1000)        0 2023-05-08 18:17:25.290169 whisper_cpp_python-0.1.7/vendor/whisper.cpp/bindings/
+-rw-rw-r--   0 carlos    (1000) carlos    (1000)      656 2023-05-08 13:31:02.000000 whisper_cpp_python-0.1.7/vendor/whisper.cpp/bindings/CMakeLists.txt
+drwxrwxr-x   0 carlos    (1000) carlos    (1000)        0 2023-05-08 18:17:25.294169 whisper_cpp_python-0.1.7/vendor/whisper.cpp/bindings/go/
+-rw-rw-r--   0 carlos    (1000) carlos    (1000)       13 2023-05-08 13:31:02.000000 whisper_cpp_python-0.1.7/vendor/whisper.cpp/bindings/go/.gitignore
+-rw-rw-r--   0 carlos    (1000) carlos    (1000)     1069 2023-05-08 13:31:02.000000 whisper_cpp_python-0.1.7/vendor/whisper.cpp/bindings/go/LICENSE
+-rw-rw-r--   0 carlos    (1000) carlos    (1000)      968 2023-05-08 13:31:02.000000 whisper_cpp_python-0.1.7/vendor/whisper.cpp/bindings/go/Makefile
+-rw-rw-r--   0 carlos    (1000) carlos    (1000)     2821 2023-05-08 13:31:02.000000 whisper_cpp_python-0.1.7/vendor/whisper.cpp/bindings/go/README.md
+-rw-rw-r--   0 carlos    (1000) carlos    (1000)      143 2023-05-08 13:31:02.000000 whisper_cpp_python-0.1.7/vendor/whisper.cpp/bindings/go/doc.go
+drwxrwxr-x   0 carlos    (1000) carlos    (1000)        0 2023-05-08 18:17:25.266168 whisper_cpp_python-0.1.7/vendor/whisper.cpp/bindings/go/examples/
+drwxrwxr-x   0 carlos    (1000) carlos    (1000)        0 2023-05-08 18:17:25.294169 whisper_cpp_python-0.1.7/vendor/whisper.cpp/bindings/go/examples/go-model-download/
+-rw-rw-r--   0 carlos    (1000) carlos    (1000)      582 2023-05-08 13:31:02.000000 whisper_cpp_python-0.1.7/vendor/whisper.cpp/bindings/go/examples/go-model-download/context.go
+-rw-rw-r--   0 carlos    (1000) carlos    (1000)     5323 2023-05-08 13:31:02.000000 whisper_cpp_python-0.1.7/vendor/whisper.cpp/bindings/go/examples/go-model-download/main.go
+drwxrwxr-x   0 carlos    (1000) carlos    (1000)        0 2023-05-08 18:17:25.294169 whisper_cpp_python-0.1.7/vendor/whisper.cpp/bindings/go/examples/go-whisper/
+-rw-rw-r--   0 carlos    (1000) carlos    (1000)      625 2023-05-08 13:31:02.000000 whisper_cpp_python-0.1.7/vendor/whisper.cpp/bindings/go/examples/go-whisper/color.go
+-rw-rw-r--   0 carlos    (1000) carlos    (1000)     4614 2023-05-08 13:31:02.000000 whisper_cpp_python-0.1.7/vendor/whisper.cpp/bindings/go/examples/go-whisper/flags.go
+-rw-rw-r--   0 carlos    (1000) carlos    (1000)      878 2023-05-08 13:31:02.000000 whisper_cpp_python-0.1.7/vendor/whisper.cpp/bindings/go/examples/go-whisper/main.go
+-rw-rw-r--   0 carlos    (1000) carlos    (1000)     3290 2023-05-08 13:31:02.000000 whisper_cpp_python-0.1.7/vendor/whisper.cpp/bindings/go/examples/go-whisper/process.go
+-rw-rw-r--   0 carlos    (1000) carlos    (1000)      380 2023-05-08 13:31:02.000000 whisper_cpp_python-0.1.7/vendor/whisper.cpp/bindings/go/go.mod
+-rw-rw-r--   0 carlos    (1000) carlos    (1000)     2019 2023-05-08 13:31:02.000000 whisper_cpp_python-0.1.7/vendor/whisper.cpp/bindings/go/go.sum
+-rw-rw-r--   0 carlos    (1000) carlos    (1000)     3408 2023-05-08 13:31:02.000000 whisper_cpp_python-0.1.7/vendor/whisper.cpp/bindings/go/params.go
+drwxrwxr-x   0 carlos    (1000) carlos    (1000)        0 2023-05-08 18:17:25.266168 whisper_cpp_python-0.1.7/vendor/whisper.cpp/bindings/go/pkg/
+drwxrwxr-x   0 carlos    (1000) carlos    (1000)        0 2023-05-08 18:17:25.294169 whisper_cpp_python-0.1.7/vendor/whisper.cpp/bindings/go/pkg/whisper/
+-rw-rw-r--   0 carlos    (1000) carlos    (1000)      799 2023-05-08 13:31:02.000000 whisper_cpp_python-0.1.7/vendor/whisper.cpp/bindings/go/pkg/whisper/consts.go
+-rw-rw-r--   0 carlos    (1000) carlos    (1000)     7926 2023-05-08 13:31:02.000000 whisper_cpp_python-0.1.7/vendor/whisper.cpp/bindings/go/pkg/whisper/context.go
+-rw-rw-r--   0 carlos    (1000) carlos    (1000)     1250 2023-05-08 13:31:02.000000 whisper_cpp_python-0.1.7/vendor/whisper.cpp/bindings/go/pkg/whisper/context_test.go
+-rw-rw-r--   0 carlos    (1000) carlos    (1000)       85 2023-05-08 13:31:02.000000 whisper_cpp_python-0.1.7/vendor/whisper.cpp/bindings/go/pkg/whisper/doc.go
+-rw-rw-r--   0 carlos    (1000) carlos    (1000)     2904 2023-05-08 13:31:02.000000 whisper_cpp_python-0.1.7/vendor/whisper.cpp/bindings/go/pkg/whisper/interface.go
+-rw-rw-r--   0 carlos    (1000) carlos    (1000)     2300 2023-05-08 13:31:02.000000 whisper_cpp_python-0.1.7/vendor/whisper.cpp/bindings/go/pkg/whisper/model.go
+drwxrwxr-x   0 carlos    (1000) carlos    (1000)        0 2023-05-08 18:17:25.294169 whisper_cpp_python-0.1.7/vendor/whisper.cpp/bindings/go/samples/
+-rw-rw-r--   0 carlos    (1000) carlos    (1000)   352078 2023-05-08 13:31:02.000000 whisper_cpp_python-0.1.7/vendor/whisper.cpp/bindings/go/samples/jfk.wav
+-rw-rw-r--   0 carlos    (1000) carlos    (1000)    14538 2023-05-08 13:31:02.000000 whisper_cpp_python-0.1.7/vendor/whisper.cpp/bindings/go/whisper.go
+-rw-rw-r--   0 carlos    (1000) carlos    (1000)     2810 2023-05-08 13:31:02.000000 whisper_cpp_python-0.1.7/vendor/whisper.cpp/bindings/go/whisper_test.go
+drwxrwxr-x   0 carlos    (1000) carlos    (1000)        0 2023-05-08 18:17:25.294169 whisper_cpp_python-0.1.7/vendor/whisper.cpp/bindings/ios/
+drwxrwxr-x   0 carlos    (1000) carlos    (1000)        0 2023-05-08 18:17:25.266168 whisper_cpp_python-0.1.7/vendor/whisper.cpp/bindings/ios/.github/
+drwxrwxr-x   0 carlos    (1000) carlos    (1000)        0 2023-05-08 18:17:25.294169 whisper_cpp_python-0.1.7/vendor/whisper.cpp/bindings/ios/.github/workflows/
+-rw-rw-r--   0 carlos    (1000) carlos    (1000)      320 2023-05-08 13:31:02.000000 whisper_cpp_python-0.1.7/vendor/whisper.cpp/bindings/ios/.github/workflows/swift.yml
+-rw-rw-r--   0 carlos    (1000) carlos    (1000)       26 2023-05-08 13:31:02.000000 whisper_cpp_python-0.1.7/vendor/whisper.cpp/bindings/ios/.gitignore
+-rw-rw-r--   0 carlos    (1000) carlos    (1000)     1072 2023-05-08 13:31:02.000000 whisper_cpp_python-0.1.7/vendor/whisper.cpp/bindings/ios/LICENSE
+-rw-rw-r--   0 carlos    (1000) carlos    (1000)      732 2023-05-08 13:31:02.000000 whisper_cpp_python-0.1.7/vendor/whisper.cpp/bindings/ios/Makefile
+-rw-rw-r--   0 carlos    (1000) carlos    (1000)      744 2023-05-08 13:31:02.000000 whisper_cpp_python-0.1.7/vendor/whisper.cpp/bindings/ios/Makefile-tmpl
+-rw-rw-r--   0 carlos    (1000) carlos    (1000)      519 2023-05-08 13:31:02.000000 whisper_cpp_python-0.1.7/vendor/whisper.cpp/bindings/ios/Package.swift
+-rw-rw-r--   0 carlos    (1000) carlos    (1000)      661 2023-05-08 13:31:02.000000 whisper_cpp_python-0.1.7/vendor/whisper.cpp/bindings/ios/README.md
+drwxrwxr-x   0 carlos    (1000) carlos    (1000)        0 2023-05-08 18:17:25.266168 whisper_cpp_python-0.1.7/vendor/whisper.cpp/bindings/ios/Sources/
+drwxrwxr-x   0 carlos    (1000) carlos    (1000)        0 2023-05-08 18:17:25.294169 whisper_cpp_python-0.1.7/vendor/whisper.cpp/bindings/ios/Sources/test-objc/
+-rw-rw-r--   0 carlos    (1000) carlos    (1000)     1506 2023-05-08 13:31:02.000000 whisper_cpp_python-0.1.7/vendor/whisper.cpp/bindings/ios/Sources/test-objc/main.m
+drwxrwxr-x   0 carlos    (1000) carlos    (1000)        0 2023-05-08 18:17:25.294169 whisper_cpp_python-0.1.7/vendor/whisper.cpp/bindings/ios/Sources/test-swift/
+-rw-rw-r--   0 carlos    (1000) carlos    (1000)      868 2023-05-08 13:31:02.000000 whisper_cpp_python-0.1.7/vendor/whisper.cpp/bindings/ios/Sources/test-swift/main.swift
+drwxrwxr-x   0 carlos    (1000) carlos    (1000)        0 2023-05-08 18:17:25.294169 whisper_cpp_python-0.1.7/vendor/whisper.cpp/bindings/ios/Sources/whisper/
+-rw-rw-r--   0 carlos    (1000) carlos    (1000)   425638 2023-05-08 13:31:02.000000 whisper_cpp_python-0.1.7/vendor/whisper.cpp/bindings/ios/Sources/whisper/ggml.c
+-rw-rw-r--   0 carlos    (1000) carlos    (1000)    30532 2023-05-08 13:31:02.000000 whisper_cpp_python-0.1.7/vendor/whisper.cpp/bindings/ios/Sources/whisper/ggml.h
+drwxrwxr-x   0 carlos    (1000) carlos    (1000)        0 2023-05-08 18:17:25.298169 whisper_cpp_python-0.1.7/vendor/whisper.cpp/bindings/ios/Sources/whisper/include/
+-rw-rw-r--   0 carlos    (1000) carlos    (1000)    23720 2023-05-08 13:31:02.000000 whisper_cpp_python-0.1.7/vendor/whisper.cpp/bindings/ios/Sources/whisper/include/whisper.h
+-rw-rw-r--   0 carlos    (1000) carlos    (1000)   183212 2023-05-08 13:31:02.000000 whisper_cpp_python-0.1.7/vendor/whisper.cpp/bindings/ios/Sources/whisper/whisper.cpp
+drwxrwxr-x   0 carlos    (1000) carlos    (1000)        0 2023-05-08 18:17:25.298169 whisper_cpp_python-0.1.7/vendor/whisper.cpp/bindings/ios/models/
+-rw-rw-r--   0 carlos    (1000) carlos    (1000)   586836 2023-05-08 13:31:02.000000 whisper_cpp_python-0.1.7/vendor/whisper.cpp/bindings/ios/models/for-tests-ggml-base.en.bin
+-rw-rw-r--   0 carlos    (1000) carlos    (1000)        0 2023-05-08 13:31:02.000000 whisper_cpp_python-0.1.7/vendor/whisper.cpp/bindings/ios/publish-trigger
+drwxrwxr-x   0 carlos    (1000) carlos    (1000)        0 2023-05-08 18:17:25.298169 whisper_cpp_python-0.1.7/vendor/whisper.cpp/bindings/javascript/
+-rw-rw-r--   0 carlos    (1000) carlos    (1000)       12 2023-05-08 13:31:02.000000 whisper_cpp_python-0.1.7/vendor/whisper.cpp/bindings/javascript/.gitignore
+-rw-rw-r--   0 carlos    (1000) carlos    (1000)      991 2023-05-08 13:31:02.000000 whisper_cpp_python-0.1.7/vendor/whisper.cpp/bindings/javascript/CMakeLists.txt
+-rw-rw-r--   0 carlos    (1000) carlos    (1000)     2547 2023-05-08 13:31:02.000000 whisper_cpp_python-0.1.7/vendor/whisper.cpp/bindings/javascript/README.md
+-rw-rw-r--   0 carlos    (1000) carlos    (1000)     3002 2023-05-08 13:31:02.000000 whisper_cpp_python-0.1.7/vendor/whisper.cpp/bindings/javascript/emscripten.cpp
+-rw-rw-r--   0 carlos    (1000) carlos    (1000)     3141 2023-05-08 13:31:02.000000 whisper_cpp_python-0.1.7/vendor/whisper.cpp/bindings/javascript/libwhisper.worker.js
+-rw-rw-r--   0 carlos    (1000) carlos    (1000)      612 2023-05-08 13:31:02.000000 whisper_cpp_python-0.1.7/vendor/whisper.cpp/bindings/javascript/package-tmpl.json
+-rw-rw-r--   0 carlos    (1000) carlos    (1000)      600 2023-05-08 13:31:02.000000 whisper_cpp_python-0.1.7/vendor/whisper.cpp/bindings/javascript/package.json
+-rw-rw-r--   0 carlos    (1000) carlos    (1000)   795866 2023-05-08 13:31:02.000000 whisper_cpp_python-0.1.7/vendor/whisper.cpp/bindings/javascript/whisper.js
+drwxrwxr-x   0 carlos    (1000) carlos    (1000)        0 2023-05-08 18:17:25.266168 whisper_cpp_python-0.1.7/vendor/whisper.cpp/bindings/ruby/
+drwxrwxr-x   0 carlos    (1000) carlos    (1000)        0 2023-05-08 18:17:25.298169 whisper_cpp_python-0.1.7/vendor/whisper.cpp/bindings/ruby/ext/
+-rw-rw-r--   0 carlos    (1000) carlos    (1000)       69 2023-05-08 13:31:02.000000 whisper_cpp_python-0.1.7/vendor/whisper.cpp/bindings/ruby/ext/.gitignore
+-rw-rw-r--   0 carlos    (1000) carlos    (1000)      781 2023-05-08 13:31:02.000000 whisper_cpp_python-0.1.7/vendor/whisper.cpp/bindings/ruby/ext/extconf.rb
+-rw-rw-r--   0 carlos    (1000) carlos    (1000)    15308 2023-05-08 13:31:02.000000 whisper_cpp_python-0.1.7/vendor/whisper.cpp/bindings/ruby/ext/ruby_whisper.cpp
+-rw-rw-r--   0 carlos    (1000) carlos    (1000)      243 2023-05-08 13:31:02.000000 whisper_cpp_python-0.1.7/vendor/whisper.cpp/bindings/ruby/ext/ruby_whisper.h
+drwxrwxr-x   0 carlos    (1000) carlos    (1000)        0 2023-05-08 18:17:25.298169 whisper_cpp_python-0.1.7/vendor/whisper.cpp/bindings/ruby/tests/
+-rw-rw-r--   0 carlos    (1000) carlos    (1000)     3444 2023-05-08 13:31:02.000000 whisper_cpp_python-0.1.7/vendor/whisper.cpp/bindings/ruby/tests/test_whisper.rb
+drwxrwxr-x   0 carlos    (1000) carlos    (1000)        0 2023-05-08 18:17:25.298169 whisper_cpp_python-0.1.7/vendor/whisper.cpp/cmake/
+-rw-rw-r--   0 carlos    (1000) carlos    (1000)     2037 2023-05-08 13:31:02.000000 whisper_cpp_python-0.1.7/vendor/whisper.cpp/cmake/BuildTypes.cmake
+-rw-rw-r--   0 carlos    (1000) carlos    (1000)      437 2023-05-08 13:31:02.000000 whisper_cpp_python-0.1.7/vendor/whisper.cpp/cmake/DefaultTargetOptions.cmake
+-rw-rw-r--   0 carlos    (1000) carlos    (1000)      717 2023-05-08 13:31:02.000000 whisper_cpp_python-0.1.7/vendor/whisper.cpp/cmake/GitVars.cmake
+drwxrwxr-x   0 carlos    (1000) carlos    (1000)        0 2023-05-08 18:17:25.298169 whisper_cpp_python-0.1.7/vendor/whisper.cpp/coreml/
+-rw-rw-r--   0 carlos    (1000) carlos    (1000)     7458 2023-05-08 13:31:02.000000 whisper_cpp_python-0.1.7/vendor/whisper.cpp/coreml/whisper-decoder-impl.h
+-rw-rw-r--   0 carlos    (1000) carlos    (1000)     8817 2023-05-08 13:31:02.000000 whisper_cpp_python-0.1.7/vendor/whisper.cpp/coreml/whisper-decoder-impl.m
+-rw-rw-r--   0 carlos    (1000) carlos    (1000)     7190 2023-05-08 13:31:02.000000 whisper_cpp_python-0.1.7/vendor/whisper.cpp/coreml/whisper-encoder-impl.h
+-rw-rw-r--   0 carlos    (1000) carlos    (1000)     8522 2023-05-08 13:31:02.000000 whisper_cpp_python-0.1.7/vendor/whisper.cpp/coreml/whisper-encoder-impl.m
+-rw-rw-r--   0 carlos    (1000) carlos    (1000)      562 2023-05-08 13:31:02.000000 whisper_cpp_python-0.1.7/vendor/whisper.cpp/coreml/whisper-encoder.h
+-rw-rw-r--   0 carlos    (1000) carlos    (1000)     2059 2023-05-08 13:31:02.000000 whisper_cpp_python-0.1.7/vendor/whisper.cpp/coreml/whisper-encoder.mm
+drwxrwxr-x   0 carlos    (1000) carlos    (1000)        0 2023-05-08 18:17:25.302169 whisper_cpp_python-0.1.7/vendor/whisper.cpp/examples/
+-rw-rw-r--   0 carlos    (1000) carlos    (1000)     1527 2023-05-08 13:31:02.000000 whisper_cpp_python-0.1.7/vendor/whisper.cpp/examples/CMakeLists.txt
+drwxrwxr-x   0 carlos    (1000) carlos    (1000)        0 2023-05-08 18:17:25.302169 whisper_cpp_python-0.1.7/vendor/whisper.cpp/examples/addon.node/
+-rw-rw-r--   0 carlos    (1000) carlos    (1000)       25 2023-05-08 13:31:02.000000 whisper_cpp_python-0.1.7/vendor/whisper.cpp/examples/addon.node/.gitignore
+-rw-rw-r--   0 carlos    (1000) carlos    (1000)     1291 2023-05-08 13:31:02.000000 whisper_cpp_python-0.1.7/vendor/whisper.cpp/examples/addon.node/CMakeLists.txt
+-rw-rw-r--   0 carlos    (1000) carlos    (1000)     1001 2023-05-08 13:31:02.000000 whisper_cpp_python-0.1.7/vendor/whisper.cpp/examples/addon.node/README.md
+drwxrwxr-x   0 carlos    (1000) carlos    (1000)        0 2023-05-08 18:17:25.302169 whisper_cpp_python-0.1.7/vendor/whisper.cpp/examples/addon.node/__test__/
+-rw-rw-r--   0 carlos    (1000) carlos    (1000)      619 2023-05-08 13:31:02.000000 whisper_cpp_python-0.1.7/vendor/whisper.cpp/examples/addon.node/__test__/whisper.spec.js
+-rw-rw-r--   0 carlos    (1000) carlos    (1000)    11631 2023-05-08 13:31:02.000000 whisper_cpp_python-0.1.7/vendor/whisper.cpp/examples/addon.node/addon.cpp
+-rw-rw-r--   0 carlos    (1000) carlos    (1000)      847 2023-05-08 13:31:02.000000 whisper_cpp_python-0.1.7/vendor/whisper.cpp/examples/addon.node/index.js
+-rw-rw-r--   0 carlos    (1000) carlos    (1000)      288 2023-05-08 13:31:02.000000 whisper_cpp_python-0.1.7/vendor/whisper.cpp/examples/addon.node/package.json
+drwxrwxr-x   0 carlos    (1000) carlos    (1000)        0 2023-05-08 18:17:25.302169 whisper_cpp_python-0.1.7/vendor/whisper.cpp/examples/bench/
+-rw-rw-r--   0 carlos    (1000) carlos    (1000)      161 2023-05-08 13:31:02.000000 whisper_cpp_python-0.1.7/vendor/whisper.cpp/examples/bench/CMakeLists.txt
+-rw-rw-r--   0 carlos    (1000) carlos    (1000)     1978 2023-05-08 13:31:02.000000 whisper_cpp_python-0.1.7/vendor/whisper.cpp/examples/bench/README.md
+-rw-rw-r--   0 carlos    (1000) carlos    (1000)     4126 2023-05-08 13:31:02.000000 whisper_cpp_python-0.1.7/vendor/whisper.cpp/examples/bench/bench.cpp
+drwxrwxr-x   0 carlos    (1000) carlos    (1000)        0 2023-05-08 18:17:25.302169 whisper_cpp_python-0.1.7/vendor/whisper.cpp/examples/bench.wasm/
+-rw-rw-r--   0 carlos    (1000) carlos    (1000)     1161 2023-05-08 13:31:02.000000 whisper_cpp_python-0.1.7/vendor/whisper.cpp/examples/bench.wasm/CMakeLists.txt
+-rw-rw-r--   0 carlos    (1000) carlos    (1000)      502 2023-05-08 13:31:02.000000 whisper_cpp_python-0.1.7/vendor/whisper.cpp/examples/bench.wasm/README.md
+-rw-rw-r--   0 carlos    (1000) carlos    (1000)     2623 2023-05-08 13:31:02.000000 whisper_cpp_python-0.1.7/vendor/whisper.cpp/examples/bench.wasm/emscripten.cpp
+-rw-rw-r--   0 carlos    (1000) carlos    (1000)    12516 2023-05-08 13:31:02.000000 whisper_cpp_python-0.1.7/vendor/whisper.cpp/examples/bench.wasm/index-tmpl.html
+drwxrwxr-x   0 carlos    (1000) carlos    (1000)        0 2023-05-08 18:17:25.306169 whisper_cpp_python-0.1.7/vendor/whisper.cpp/examples/command/
+-rw-rw-r--   0 carlos    (1000) carlos    (1000)      240 2023-05-08 13:31:02.000000 whisper_cpp_python-0.1.7/vendor/whisper.cpp/examples/command/CMakeLists.txt
+-rw-rw-r--   0 carlos    (1000) carlos    (1000)     1766 2023-05-08 13:31:02.000000 whisper_cpp_python-0.1.7/vendor/whisper.cpp/examples/command/README.md
+-rw-rw-r--   0 carlos    (1000) carlos    (1000)    24877 2023-05-08 13:31:02.000000 whisper_cpp_python-0.1.7/vendor/whisper.cpp/examples/command/command.cpp
+-rw-rw-r--   0 carlos    (1000) carlos    (1000)       54 2023-05-08 13:31:02.000000 whisper_cpp_python-0.1.7/vendor/whisper.cpp/examples/command/commands.txt
+drwxrwxr-x   0 carlos    (1000) carlos    (1000)        0 2023-05-08 18:17:25.306169 whisper_cpp_python-0.1.7/vendor/whisper.cpp/examples/command.wasm/
+-rw-rw-r--   0 carlos    (1000) carlos    (1000)     1181 2023-05-08 13:31:02.000000 whisper_cpp_python-0.1.7/vendor/whisper.cpp/examples/command.wasm/CMakeLists.txt
+-rw-rw-r--   0 carlos    (1000) carlos    (1000)      585 2023-05-08 13:31:02.000000 whisper_cpp_python-0.1.7/vendor/whisper.cpp/examples/command.wasm/README.md
+-rw-rw-r--   0 carlos    (1000) carlos    (1000)    10412 2023-05-08 13:31:02.000000 whisper_cpp_python-0.1.7/vendor/whisper.cpp/examples/command.wasm/emscripten.cpp
+-rw-rw-r--   0 carlos    (1000) carlos    (1000)    16219 2023-05-08 13:31:02.000000 whisper_cpp_python-0.1.7/vendor/whisper.cpp/examples/command.wasm/index-tmpl.html
+-rw-rw-r--   0 carlos    (1000) carlos    (1000)     8583 2023-05-08 13:31:02.000000 whisper_cpp_python-0.1.7/vendor/whisper.cpp/examples/common-ggml.cpp
+-rw-rw-r--   0 carlos    (1000) carlos    (1000)      410 2023-05-08 13:31:02.000000 whisper_cpp_python-0.1.7/vendor/whisper.cpp/examples/common-ggml.h
+-rw-rw-r--   0 carlos    (1000) carlos    (1000)     6626 2023-05-08 13:31:02.000000 whisper_cpp_python-0.1.7/vendor/whisper.cpp/examples/common-sdl.cpp
+-rw-rw-r--   0 carlos    (1000) carlos    (1000)     1011 2023-05-08 13:31:02.000000 whisper_cpp_python-0.1.7/vendor/whisper.cpp/examples/common-sdl.h
+-rw-rw-r--   0 carlos    (1000) carlos    (1000)    15650 2023-05-08 13:31:02.000000 whisper_cpp_python-0.1.7/vendor/whisper.cpp/examples/common.cpp
+-rw-rw-r--   0 carlos    (1000) carlos    (1000)     3346 2023-05-08 13:31:02.000000 whisper_cpp_python-0.1.7/vendor/whisper.cpp/examples/common.h
+-rw-rw-r--   0 carlos    (1000) carlos    (1000)   241358 2023-05-08 13:31:02.000000 whisper_cpp_python-0.1.7/vendor/whisper.cpp/examples/dr_wav.h
+-rwxrwxr-x   0 carlos    (1000) carlos    (1000)     1197 2023-05-08 13:31:02.000000 whisper_cpp_python-0.1.7/vendor/whisper.cpp/examples/generate-karaoke.sh
+-rw-rw-r--   0 carlos    (1000) carlos    (1000)     6592 2023-05-08 13:31:02.000000 whisper_cpp_python-0.1.7/vendor/whisper.cpp/examples/helpers.js
+-rwxrwxr-x   0 carlos    (1000) carlos    (1000)     2955 2023-05-08 13:31:02.000000 whisper_cpp_python-0.1.7/vendor/whisper.cpp/examples/livestream.sh
+drwxrwxr-x   0 carlos    (1000) carlos    (1000)        0 2023-05-08 18:17:25.306169 whisper_cpp_python-0.1.7/vendor/whisper.cpp/examples/main/
+-rw-rw-r--   0 carlos    (1000) carlos    (1000)      166 2023-05-08 13:31:02.000000 whisper_cpp_python-0.1.7/vendor/whisper.cpp/examples/main/CMakeLists.txt
+-rw-rw-r--   0 carlos    (1000) carlos    (1000)     2711 2023-05-08 13:31:02.000000 whisper_cpp_python-0.1.7/vendor/whisper.cpp/examples/main/README.md
+-rw-rw-r--   0 carlos    (1000) carlos    (1000)    36271 2023-05-08 13:31:02.000000 whisper_cpp_python-0.1.7/vendor/whisper.cpp/examples/main/main.cpp
+drwxrwxr-x   0 carlos    (1000) carlos    (1000)        0 2023-05-08 18:17:25.306169 whisper_cpp_python-0.1.7/vendor/whisper.cpp/examples/quantize/
+-rw-rw-r--   0 carlos    (1000) carlos    (1000)      174 2023-05-08 13:31:02.000000 whisper_cpp_python-0.1.7/vendor/whisper.cpp/examples/quantize/CMakeLists.txt
+-rw-rw-r--   0 carlos    (1000) carlos    (1000)       75 2023-05-08 13:31:02.000000 whisper_cpp_python-0.1.7/vendor/whisper.cpp/examples/quantize/README.md
+-rw-rw-r--   0 carlos    (1000) carlos    (1000)     7693 2023-05-08 13:31:02.000000 whisper_cpp_python-0.1.7/vendor/whisper.cpp/examples/quantize/quantize.cpp
+drwxrwxr-x   0 carlos    (1000) carlos    (1000)        0 2023-05-08 18:17:25.306169 whisper_cpp_python-0.1.7/vendor/whisper.cpp/examples/stream/
+-rw-rw-r--   0 carlos    (1000) carlos    (1000)      237 2023-05-08 13:31:02.000000 whisper_cpp_python-0.1.7/vendor/whisper.cpp/examples/stream/CMakeLists.txt
+-rw-rw-r--   0 carlos    (1000) carlos    (1000)     1589 2023-05-08 13:31:02.000000 whisper_cpp_python-0.1.7/vendor/whisper.cpp/examples/stream/README.md
+-rw-rw-r--   0 carlos    (1000) carlos    (1000)    16389 2023-05-08 13:31:02.000000 whisper_cpp_python-0.1.7/vendor/whisper.cpp/examples/stream/stream.cpp
+drwxrwxr-x   0 carlos    (1000) carlos    (1000)        0 2023-05-08 18:17:25.306169 whisper_cpp_python-0.1.7/vendor/whisper.cpp/examples/stream.wasm/
+-rw-rw-r--   0 carlos    (1000) carlos    (1000)     1162 2023-05-08 13:31:02.000000 whisper_cpp_python-0.1.7/vendor/whisper.cpp/examples/stream.wasm/CMakeLists.txt
+-rw-rw-r--   0 carlos    (1000) carlos    (1000)      443 2023-05-08 13:31:02.000000 whisper_cpp_python-0.1.7/vendor/whisper.cpp/examples/stream.wasm/README.md
+-rw-rw-r--   0 carlos    (1000) carlos    (1000)     6142 2023-05-08 13:31:02.000000 whisper_cpp_python-0.1.7/vendor/whisper.cpp/examples/stream.wasm/emscripten.cpp
+-rw-rw-r--   0 carlos    (1000) carlos    (1000)    16188 2023-05-08 13:31:02.000000 whisper_cpp_python-0.1.7/vendor/whisper.cpp/examples/stream.wasm/index-tmpl.html
+drwxrwxr-x   0 carlos    (1000) carlos    (1000)        0 2023-05-08 18:17:25.306169 whisper_cpp_python-0.1.7/vendor/whisper.cpp/examples/talk/
+-rw-rw-r--   0 carlos    (1000) carlos    (1000)       10 2023-05-08 13:31:02.000000 whisper_cpp_python-0.1.7/vendor/whisper.cpp/examples/talk/.gitignore
+-rw-rw-r--   0 carlos    (1000) carlos    (1000)      240 2023-05-08 13:31:02.000000 whisper_cpp_python-0.1.7/vendor/whisper.cpp/examples/talk/CMakeLists.txt
+-rw-rw-r--   0 carlos    (1000) carlos    (1000)     1292 2023-05-08 13:31:02.000000 whisper_cpp_python-0.1.7/vendor/whisper.cpp/examples/talk/README.md
+-rw-rw-r--   0 carlos    (1000) carlos    (1000)      764 2023-05-08 13:31:02.000000 whisper_cpp_python-0.1.7/vendor/whisper.cpp/examples/talk/eleven-labs.py
+-rw-rw-r--   0 carlos    (1000) carlos    (1000)    27945 2023-05-08 13:31:02.000000 whisper_cpp_python-0.1.7/vendor/whisper.cpp/examples/talk/gpt-2.cpp
+-rw-rw-r--   0 carlos    (1000) carlos    (1000)      580 2023-05-08 13:31:02.000000 whisper_cpp_python-0.1.7/vendor/whisper.cpp/examples/talk/gpt-2.h
+-rwxrwxr-x   0 carlos    (1000) carlos    (1000)      563 2023-05-08 13:31:02.000000 whisper_cpp_python-0.1.7/vendor/whisper.cpp/examples/talk/speak.sh
+-rw-rw-r--   0 carlos    (1000) carlos    (1000)    14593 2023-05-08 13:31:02.000000 whisper_cpp_python-0.1.7/vendor/whisper.cpp/examples/talk/talk.cpp
+drwxrwxr-x   0 carlos    (1000) carlos    (1000)        0 2023-05-08 18:17:25.310169 whisper_cpp_python-0.1.7/vendor/whisper.cpp/examples/talk-llama/
+-rw-rw-r--   0 carlos    (1000) carlos    (1000)       10 2023-05-08 13:31:02.000000 whisper_cpp_python-0.1.7/vendor/whisper.cpp/examples/talk-llama/.gitignore
+-rw-rw-r--   0 carlos    (1000) carlos    (1000)      733 2023-05-08 13:31:02.000000 whisper_cpp_python-0.1.7/vendor/whisper.cpp/examples/talk-llama/CMakeLists.txt
+-rw-rw-r--   0 carlos    (1000) carlos    (1000)     2458 2023-05-08 13:31:02.000000 whisper_cpp_python-0.1.7/vendor/whisper.cpp/examples/talk-llama/README.md
+-rw-rw-r--   0 carlos    (1000) carlos    (1000)      770 2023-05-08 13:31:02.000000 whisper_cpp_python-0.1.7/vendor/whisper.cpp/examples/talk-llama/eleven-labs.py
+-rw-rw-r--   0 carlos    (1000) carlos    (1000)    12448 2023-05-08 13:31:02.000000 whisper_cpp_python-0.1.7/vendor/whisper.cpp/examples/talk-llama/llama-util.h
+-rw-rw-r--   0 carlos    (1000) carlos    (1000)    94701 2023-05-08 13:31:02.000000 whisper_cpp_python-0.1.7/vendor/whisper.cpp/examples/talk-llama/llama.cpp
+-rw-rw-r--   0 carlos    (1000) carlos    (1000)    13325 2023-05-08 13:31:02.000000 whisper_cpp_python-0.1.7/vendor/whisper.cpp/examples/talk-llama/llama.h
+drwxrwxr-x   0 carlos    (1000) carlos    (1000)        0 2023-05-08 18:17:25.310169 whisper_cpp_python-0.1.7/vendor/whisper.cpp/examples/talk-llama/prompts/
+-rw-rw-r--   0 carlos    (1000) carlos    (1000)      978 2023-05-08 13:31:02.000000 whisper_cpp_python-0.1.7/vendor/whisper.cpp/examples/talk-llama/prompts/talk-alpaca.txt
+-rwxrwxr-x   0 carlos    (1000) carlos    (1000)      588 2023-05-08 13:31:02.000000 whisper_cpp_python-0.1.7/vendor/whisper.cpp/examples/talk-llama/speak.sh
+-rw-rw-r--   0 carlos    (1000) carlos    (1000)    27971 2023-05-08 13:31:02.000000 whisper_cpp_python-0.1.7/vendor/whisper.cpp/examples/talk-llama/talk-llama.cpp
+drwxrwxr-x   0 carlos    (1000) carlos    (1000)        0 2023-05-08 18:17:25.310169 whisper_cpp_python-0.1.7/vendor/whisper.cpp/examples/talk.wasm/
+-rw-rw-r--   0 carlos    (1000) carlos    (1000)     1171 2023-05-08 13:31:02.000000 whisper_cpp_python-0.1.7/vendor/whisper.cpp/examples/talk.wasm/CMakeLists.txt
+-rw-rw-r--   0 carlos    (1000) carlos    (1000)     3341 2023-05-08 13:31:02.000000 whisper_cpp_python-0.1.7/vendor/whisper.cpp/examples/talk.wasm/README.md
+-rw-rw-r--   0 carlos    (1000) carlos    (1000)    12231 2023-05-08 13:31:02.000000 whisper_cpp_python-0.1.7/vendor/whisper.cpp/examples/talk.wasm/emscripten.cpp
+-rw-rw-r--   0 carlos    (1000) carlos    (1000)    27945 2023-05-08 13:31:02.000000 whisper_cpp_python-0.1.7/vendor/whisper.cpp/examples/talk.wasm/gpt-2.cpp
+-rw-rw-r--   0 carlos    (1000) carlos    (1000)      580 2023-05-08 13:31:02.000000 whisper_cpp_python-0.1.7/vendor/whisper.cpp/examples/talk.wasm/gpt-2.h
+-rw-rw-r--   0 carlos    (1000) carlos    (1000)    33143 2023-05-08 13:31:02.000000 whisper_cpp_python-0.1.7/vendor/whisper.cpp/examples/talk.wasm/index-tmpl.html
+-rwxrwxr-x   0 carlos    (1000) carlos    (1000)     2757 2023-05-08 13:31:02.000000 whisper_cpp_python-0.1.7/vendor/whisper.cpp/examples/twitch.sh
+drwxrwxr-x   0 carlos    (1000) carlos    (1000)        0 2023-05-08 18:17:25.310169 whisper_cpp_python-0.1.7/vendor/whisper.cpp/examples/whisper.android/
+-rw-rw-r--   0 carlos    (1000) carlos    (1000)      225 2023-05-08 13:31:02.000000 whisper_cpp_python-0.1.7/vendor/whisper.cpp/examples/whisper.android/.gitignore
+drwxrwxr-x   0 carlos    (1000) carlos    (1000)        0 2023-05-08 18:17:25.310169 whisper_cpp_python-0.1.7/vendor/whisper.cpp/examples/whisper.android/.idea/
+-rw-rw-r--   0 carlos    (1000) carlos    (1000)       47 2023-05-08 13:31:02.000000 whisper_cpp_python-0.1.7/vendor/whisper.cpp/examples/whisper.android/.idea/.gitignore
+-rw-rw-r--   0 carlos    (1000) carlos    (1000)       14 2023-05-08 13:31:02.000000 whisper_cpp_python-0.1.7/vendor/whisper.cpp/examples/whisper.android/.idea/.name
+-rw-rw-r--   0 carlos    (1000) carlos    (1000)      169 2023-05-08 13:31:02.000000 whisper_cpp_python-0.1.7/vendor/whisper.cpp/examples/whisper.android/.idea/compiler.xml
+-rw-rw-r--   0 carlos    (1000) carlos    (1000)      680 2023-05-08 13:31:02.000000 whisper_cpp_python-0.1.7/vendor/whisper.cpp/examples/whisper.android/.idea/gradle.xml
+-rw-rw-r--   0 carlos    (1000) carlos    (1000)      468 2023-05-08 13:31:02.000000 whisper_cpp_python-0.1.7/vendor/whisper.cpp/examples/whisper.android/.idea/misc.xml
+-rw-rw-r--   0 carlos    (1000) carlos    (1000)      186 2023-05-08 13:31:02.000000 whisper_cpp_python-0.1.7/vendor/whisper.cpp/examples/whisper.android/.idea/vcs.xml
+-rw-rw-r--   0 carlos    (1000) carlos    (1000)      973 2023-05-08 13:31:02.000000 whisper_cpp_python-0.1.7/vendor/whisper.cpp/examples/whisper.android/README.md
+drwxrwxr-x   0 carlos    (1000) carlos    (1000)        0 2023-05-08 18:17:25.310169 whisper_cpp_python-0.1.7/vendor/whisper.cpp/examples/whisper.android/app/
+-rw-rw-r--   0 carlos    (1000) carlos    (1000)        6 2023-05-08 13:31:02.000000 whisper_cpp_python-0.1.7/vendor/whisper.cpp/examples/whisper.android/app/.gitignore
+-rw-rw-r--   0 carlos    (1000) carlos    (1000)     2186 2023-05-08 13:31:02.000000 whisper_cpp_python-0.1.7/vendor/whisper.cpp/examples/whisper.android/app/build.gradle
+-rw-rw-r--   0 carlos    (1000) carlos    (1000)      750 2023-05-08 13:31:02.000000 whisper_cpp_python-0.1.7/vendor/whisper.cpp/examples/whisper.android/app/proguard-rules.pro
+drwxrwxr-x   0 carlos    (1000) carlos    (1000)        0 2023-05-08 18:17:25.270168 whisper_cpp_python-0.1.7/vendor/whisper.cpp/examples/whisper.android/app/src/
+drwxrwxr-x   0 carlos    (1000) carlos    (1000)        0 2023-05-08 18:17:25.270168 whisper_cpp_python-0.1.7/vendor/whisper.cpp/examples/whisper.android/app/src/androidTest/
+drwxrwxr-x   0 carlos    (1000) carlos    (1000)        0 2023-05-08 18:17:25.270168 whisper_cpp_python-0.1.7/vendor/whisper.cpp/examples/whisper.android/app/src/androidTest/java/
+drwxrwxr-x   0 carlos    (1000) carlos    (1000)        0 2023-05-08 18:17:25.270168 whisper_cpp_python-0.1.7/vendor/whisper.cpp/examples/whisper.android/app/src/androidTest/java/com/
+drwxrwxr-x   0 carlos    (1000) carlos    (1000)        0 2023-05-08 18:17:25.310169 whisper_cpp_python-0.1.7/vendor/whisper.cpp/examples/whisper.android/app/src/androidTest/java/com/whispercppdemo/
+-rw-rw-r--   0 carlos    (1000) carlos    (1000)      663 2023-05-08 13:31:02.000000 whisper_cpp_python-0.1.7/vendor/whisper.cpp/examples/whisper.android/app/src/androidTest/java/com/whispercppdemo/ExampleInstrumentedTest.kt
+drwxrwxr-x   0 carlos    (1000) carlos    (1000)        0 2023-05-08 18:17:25.310169 whisper_cpp_python-0.1.7/vendor/whisper.cpp/examples/whisper.android/app/src/main/
+-rw-rw-r--   0 carlos    (1000) carlos    (1000)     1124 2023-05-08 13:31:02.000000 whisper_cpp_python-0.1.7/vendor/whisper.cpp/examples/whisper.android/app/src/main/AndroidManifest.xml
+drwxrwxr-x   0 carlos    (1000) carlos    (1000)        0 2023-05-08 18:17:25.270168 whisper_cpp_python-0.1.7/vendor/whisper.cpp/examples/whisper.android/app/src/main/java/
+drwxrwxr-x   0 carlos    (1000) carlos    (1000)        0 2023-05-08 18:17:25.270168 whisper_cpp_python-0.1.7/vendor/whisper.cpp/examples/whisper.android/app/src/main/java/com/
+drwxrwxr-x   0 carlos    (1000) carlos    (1000)        0 2023-05-08 18:17:25.310169 whisper_cpp_python-0.1.7/vendor/whisper.cpp/examples/whisper.android/app/src/main/java/com/whispercppdemo/
+-rw-rw-r--   0 carlos    (1000) carlos    (1000)      694 2023-05-08 13:31:02.000000 whisper_cpp_python-0.1.7/vendor/whisper.cpp/examples/whisper.android/app/src/main/java/com/whispercppdemo/MainActivity.kt
+drwxrwxr-x   0 carlos    (1000) carlos    (1000)        0 2023-05-08 18:17:25.314169 whisper_cpp_python-0.1.7/vendor/whisper.cpp/examples/whisper.android/app/src/main/java/com/whispercppdemo/media/
+-rw-rw-r--   0 carlos    (1000) carlos    (1000)     2053 2023-05-08 13:31:02.000000 whisper_cpp_python-0.1.7/vendor/whisper.cpp/examples/whisper.android/app/src/main/java/com/whispercppdemo/media/RiffWaveHelper.kt
+drwxrwxr-x   0 carlos    (1000) carlos    (1000)        0 2023-05-08 18:17:25.314169 whisper_cpp_python-0.1.7/vendor/whisper.cpp/examples/whisper.android/app/src/main/java/com/whispercppdemo/recorder/
+-rw-rw-r--   0 carlos    (1000) carlos    (1000)     2711 2023-05-08 13:31:02.000000 whisper_cpp_python-0.1.7/vendor/whisper.cpp/examples/whisper.android/app/src/main/java/com/whispercppdemo/recorder/Recorder.kt
+drwxrwxr-x   0 carlos    (1000) carlos    (1000)        0 2023-05-08 18:17:25.270168 whisper_cpp_python-0.1.7/vendor/whisper.cpp/examples/whisper.android/app/src/main/java/com/whispercppdemo/ui/
+drwxrwxr-x   0 carlos    (1000) carlos    (1000)        0 2023-05-08 18:17:25.314169 whisper_cpp_python-0.1.7/vendor/whisper.cpp/examples/whisper.android/app/src/main/java/com/whispercppdemo/ui/main/
+-rw-rw-r--   0 carlos    (1000) carlos    (1000)     3537 2023-05-08 13:31:02.000000 whisper_cpp_python-0.1.7/vendor/whisper.cpp/examples/whisper.android/app/src/main/java/com/whispercppdemo/ui/main/MainScreen.kt
+-rw-rw-r--   0 carlos    (1000) carlos    (1000)     7330 2023-05-08 13:31:02.000000 whisper_cpp_python-0.1.7/vendor/whisper.cpp/examples/whisper.android/app/src/main/java/com/whispercppdemo/ui/main/MainScreenViewModel.kt
+drwxrwxr-x   0 carlos    (1000) carlos    (1000)        0 2023-05-08 18:17:25.314169 whisper_cpp_python-0.1.7/vendor/whisper.cpp/examples/whisper.android/app/src/main/java/com/whispercppdemo/ui/theme/
+-rw-rw-r--   0 carlos    (1000) carlos    (1000)      282 2023-05-08 13:31:02.000000 whisper_cpp_python-0.1.7/vendor/whisper.cpp/examples/whisper.android/app/src/main/java/com/whispercppdemo/ui/theme/Color.kt
+-rw-rw-r--   0 carlos    (1000) carlos    (1000)     2156 2023-05-08 13:31:02.000000 whisper_cpp_python-0.1.7/vendor/whisper.cpp/examples/whisper.android/app/src/main/java/com/whispercppdemo/ui/theme/Theme.kt
+-rw-rw-r--   0 carlos    (1000) carlos    (1000)      987 2023-05-08 13:31:02.000000 whisper_cpp_python-0.1.7/vendor/whisper.cpp/examples/whisper.android/app/src/main/java/com/whispercppdemo/ui/theme/Type.kt
+drwxrwxr-x   0 carlos    (1000) carlos    (1000)        0 2023-05-08 18:17:25.314169 whisper_cpp_python-0.1.7/vendor/whisper.cpp/examples/whisper.android/app/src/main/java/com/whispercppdemo/whisper/
+-rw-rw-r--   0 carlos    (1000) carlos    (1000)     5362 2023-05-08 13:31:02.000000 whisper_cpp_python-0.1.7/vendor/whisper.cpp/examples/whisper.android/app/src/main/java/com/whispercppdemo/whisper/LibWhisper.kt
+drwxrwxr-x   0 carlos    (1000) carlos    (1000)        0 2023-05-08 18:17:25.270168 whisper_cpp_python-0.1.7/vendor/whisper.cpp/examples/whisper.android/app/src/main/jni/
+drwxrwxr-x   0 carlos    (1000) carlos    (1000)        0 2023-05-08 18:17:25.314169 whisper_cpp_python-0.1.7/vendor/whisper.cpp/examples/whisper.android/app/src/main/jni/whisper/
+-rw-rw-r--   0 carlos    (1000) carlos    (1000)      834 2023-05-08 13:31:02.000000 whisper_cpp_python-0.1.7/vendor/whisper.cpp/examples/whisper.android/app/src/main/jni/whisper/Android.mk
+-rw-rw-r--   0 carlos    (1000) carlos    (1000)       21 2023-05-08 13:31:02.000000 whisper_cpp_python-0.1.7/vendor/whisper.cpp/examples/whisper.android/app/src/main/jni/whisper/Application.mk
+-rw-rw-r--   0 carlos    (1000) carlos    (1000)      708 2023-05-08 13:31:02.000000 whisper_cpp_python-0.1.7/vendor/whisper.cpp/examples/whisper.android/app/src/main/jni/whisper/Whisper.mk
+-rw-rw-r--   0 carlos    (1000) carlos    (1000)     8393 2023-05-08 13:31:02.000000 whisper_cpp_python-0.1.7/vendor/whisper.cpp/examples/whisper.android/app/src/main/jni/whisper/jni.c
+drwxrwxr-x   0 carlos    (1000) carlos    (1000)        0 2023-05-08 18:17:25.270168 whisper_cpp_python-0.1.7/vendor/whisper.cpp/examples/whisper.android/app/src/main/res/
+drwxrwxr-x   0 carlos    (1000) carlos    (1000)        0 2023-05-08 18:17:25.314169 whisper_cpp_python-0.1.7/vendor/whisper.cpp/examples/whisper.android/app/src/main/res/drawable/
+-rw-rw-r--   0 carlos    (1000) carlos    (1000)     5606 2023-05-08 13:31:02.000000 whisper_cpp_python-0.1.7/vendor/whisper.cpp/examples/whisper.android/app/src/main/res/drawable/ic_launcher_background.xml
+-rw-rw-r--   0 carlos    (1000) carlos    (1000)     1702 2023-05-08 13:31:02.000000 whisper_cpp_python-0.1.7/vendor/whisper.cpp/examples/whisper.android/app/src/main/res/drawable/ic_launcher_foreground.xml
+drwxrwxr-x   0 carlos    (1000) carlos    (1000)        0 2023-05-08 18:17:25.314169 whisper_cpp_python-0.1.7/vendor/whisper.cpp/examples/whisper.android/app/src/main/res/mipmap-anydpi/
+-rw-rw-r--   0 carlos    (1000) carlos    (1000)      272 2023-05-08 13:31:02.000000 whisper_cpp_python-0.1.7/vendor/whisper.cpp/examples/whisper.android/app/src/main/res/mipmap-anydpi/ic_launcher.xml
+drwxrwxr-x   0 carlos    (1000) carlos    (1000)        0 2023-05-08 18:17:25.314169 whisper_cpp_python-0.1.7/vendor/whisper.cpp/examples/whisper.android/app/src/main/res/values/
+-rw-rw-r--   0 carlos    (1000) carlos    (1000)      378 2023-05-08 13:31:02.000000 whisper_cpp_python-0.1.7/vendor/whisper.cpp/examples/whisper.android/app/src/main/res/values/colors.xml
+-rw-rw-r--   0 carlos    (1000) carlos    (1000)       76 2023-05-08 13:31:02.000000 whisper_cpp_python-0.1.7/vendor/whisper.cpp/examples/whisper.android/app/src/main/res/values/strings.xml
+-rw-rw-r--   0 carlos    (1000) carlos    (1000)      156 2023-05-08 13:31:02.000000 whisper_cpp_python-0.1.7/vendor/whisper.cpp/examples/whisper.android/app/src/main/res/values/themes.xml
+drwxrwxr-x   0 carlos    (1000) carlos    (1000)        0 2023-05-08 18:17:25.314169 whisper_cpp_python-0.1.7/vendor/whisper.cpp/examples/whisper.android/app/src/main/res/xml/
+-rw-rw-r--   0 carlos    (1000) carlos    (1000)      478 2023-05-08 13:31:02.000000 whisper_cpp_python-0.1.7/vendor/whisper.cpp/examples/whisper.android/app/src/main/res/xml/backup_rules.xml
+-rw-rw-r--   0 carlos    (1000) carlos    (1000)      551 2023-05-08 13:31:02.000000 whisper_cpp_python-0.1.7/vendor/whisper.cpp/examples/whisper.android/app/src/main/res/xml/data_extraction_rules.xml
+drwxrwxr-x   0 carlos    (1000) carlos    (1000)        0 2023-05-08 18:17:25.270168 whisper_cpp_python-0.1.7/vendor/whisper.cpp/examples/whisper.android/app/src/test/
+drwxrwxr-x   0 carlos    (1000) carlos    (1000)        0 2023-05-08 18:17:25.270168 whisper_cpp_python-0.1.7/vendor/whisper.cpp/examples/whisper.android/app/src/test/java/
+drwxrwxr-x   0 carlos    (1000) carlos    (1000)        0 2023-05-08 18:17:25.270168 whisper_cpp_python-0.1.7/vendor/whisper.cpp/examples/whisper.android/app/src/test/java/com/
+drwxrwxr-x   0 carlos    (1000) carlos    (1000)        0 2023-05-08 18:17:25.314169 whisper_cpp_python-0.1.7/vendor/whisper.cpp/examples/whisper.android/app/src/test/java/com/whispercppdemo/
+-rw-rw-r--   0 carlos    (1000) carlos    (1000)      342 2023-05-08 13:31:02.000000 whisper_cpp_python-0.1.7/vendor/whisper.cpp/examples/whisper.android/app/src/test/java/com/whispercppdemo/ExampleUnitTest.kt
+-rw-rw-r--   0 carlos    (1000) carlos    (1000)      296 2023-05-08 13:31:02.000000 whisper_cpp_python-0.1.7/vendor/whisper.cpp/examples/whisper.android/build.gradle
+drwxrwxr-x   0 carlos    (1000) carlos    (1000)        0 2023-05-08 18:17:25.270168 whisper_cpp_python-0.1.7/vendor/whisper.cpp/examples/whisper.android/gradle/
+drwxrwxr-x   0 carlos    (1000) carlos    (1000)        0 2023-05-08 18:17:25.314169 whisper_cpp_python-0.1.7/vendor/whisper.cpp/examples/whisper.android/gradle/wrapper/
+-rw-rw-r--   0 carlos    (1000) carlos    (1000)    59203 2023-05-08 13:31:02.000000 whisper_cpp_python-0.1.7/vendor/whisper.cpp/examples/whisper.android/gradle/wrapper/gradle-wrapper.jar
+-rw-rw-r--   0 carlos    (1000) carlos    (1000)      230 2023-05-08 13:31:02.000000 whisper_cpp_python-0.1.7/vendor/whisper.cpp/examples/whisper.android/gradle/wrapper/gradle-wrapper.properties
+-rw-rw-r--   0 carlos    (1000) carlos    (1000)     1358 2023-05-08 13:31:02.000000 whisper_cpp_python-0.1.7/vendor/whisper.cpp/examples/whisper.android/gradle.properties
+-rwxrwxr-x   0 carlos    (1000) carlos    (1000)     5766 2023-05-08 13:31:02.000000 whisper_cpp_python-0.1.7/vendor/whisper.cpp/examples/whisper.android/gradlew
+-rw-rw-r--   0 carlos    (1000) carlos    (1000)     2763 2023-05-08 13:31:02.000000 whisper_cpp_python-0.1.7/vendor/whisper.cpp/examples/whisper.android/gradlew.bat
+-rw-rw-r--   0 carlos    (1000) carlos    (1000)      331 2023-05-08 13:31:02.000000 whisper_cpp_python-0.1.7/vendor/whisper.cpp/examples/whisper.android/settings.gradle
+drwxrwxr-x   0 carlos    (1000) carlos    (1000)        0 2023-05-08 18:17:25.314169 whisper_cpp_python-0.1.7/vendor/whisper.cpp/examples/whisper.nvim/
+-rw-rw-r--   0 carlos    (1000) carlos    (1000)     3766 2023-05-08 13:31:02.000000 whisper_cpp_python-0.1.7/vendor/whisper.cpp/examples/whisper.nvim/README.md
+-rwxrwxr-x   0 carlos    (1000) carlos    (1000)     2032 2023-05-08 13:31:02.000000 whisper_cpp_python-0.1.7/vendor/whisper.cpp/examples/whisper.nvim/whisper.nvim
+drwxrwxr-x   0 carlos    (1000) carlos    (1000)        0 2023-05-08 18:17:25.314169 whisper_cpp_python-0.1.7/vendor/whisper.cpp/examples/whisper.objc/
+-rw-rw-r--   0 carlos    (1000) carlos    (1000)     1189 2023-05-08 13:31:02.000000 whisper_cpp_python-0.1.7/vendor/whisper.cpp/examples/whisper.objc/README.md
+drwxrwxr-x   0 carlos    (1000) carlos    (1000)        0 2023-05-08 18:17:25.314169 whisper_cpp_python-0.1.7/vendor/whisper.cpp/examples/whisper.objc/whisper.objc/
+-rw-rw-r--   0 carlos    (1000) carlos    (1000)      183 2023-05-08 13:31:02.000000 whisper_cpp_python-0.1.7/vendor/whisper.cpp/examples/whisper.objc/whisper.objc/AppDelegate.h
+-rw-rw-r--   0 carlos    (1000) carlos    (1000)     1320 2023-05-08 13:31:02.000000 whisper_cpp_python-0.1.7/vendor/whisper.cpp/examples/whisper.objc/whisper.objc/AppDelegate.m
+drwxrwxr-x   0 carlos    (1000) carlos    (1000)        0 2023-05-08 18:17:25.318169 whisper_cpp_python-0.1.7/vendor/whisper.cpp/examples/whisper.objc/whisper.objc/Assets.xcassets/
+drwxrwxr-x   0 carlos    (1000) carlos    (1000)        0 2023-05-08 18:17:25.318169 whisper_cpp_python-0.1.7/vendor/whisper.cpp/examples/whisper.objc/whisper.objc/Assets.xcassets/AccentColor.colorset/
+-rw-rw-r--   0 carlos    (1000) carlos    (1000)      123 2023-05-08 13:31:02.000000 whisper_cpp_python-0.1.7/vendor/whisper.cpp/examples/whisper.objc/whisper.objc/Assets.xcassets/AccentColor.colorset/Contents.json
+drwxrwxr-x   0 carlos    (1000) carlos    (1000)        0 2023-05-08 18:17:25.318169 whisper_cpp_python-0.1.7/vendor/whisper.cpp/examples/whisper.objc/whisper.objc/Assets.xcassets/AppIcon.appiconset/
+-rw-rw-r--   0 carlos    (1000) carlos    (1000)      177 2023-05-08 13:31:02.000000 whisper_cpp_python-0.1.7/vendor/whisper.cpp/examples/whisper.objc/whisper.objc/Assets.xcassets/AppIcon.appiconset/Contents.json
+-rw-rw-r--   0 carlos    (1000) carlos    (1000)       63 2023-05-08 13:31:02.000000 whisper_cpp_python-0.1.7/vendor/whisper.cpp/examples/whisper.objc/whisper.objc/Assets.xcassets/Contents.json
+drwxrwxr-x   0 carlos    (1000) carlos    (1000)        0 2023-05-08 18:17:25.318169 whisper_cpp_python-0.1.7/vendor/whisper.cpp/examples/whisper.objc/whisper.objc/Base.lproj/
+-rw-rw-r--   0 carlos    (1000) carlos    (1000)     1665 2023-05-08 13:31:02.000000 whisper_cpp_python-0.1.7/vendor/whisper.cpp/examples/whisper.objc/whisper.objc/Base.lproj/LaunchScreen.storyboard
+-rw-rw-r--   0 carlos    (1000) carlos    (1000)     8419 2023-05-08 13:31:02.000000 whisper_cpp_python-0.1.7/vendor/whisper.cpp/examples/whisper.objc/whisper.objc/Base.lproj/Main.storyboard
+-rw-rw-r--   0 carlos    (1000) carlos    (1000)      806 2023-05-08 13:31:02.000000 whisper_cpp_python-0.1.7/vendor/whisper.cpp/examples/whisper.objc/whisper.objc/Info.plist
+-rw-rw-r--   0 carlos    (1000) carlos    (1000)      236 2023-05-08 13:31:02.000000 whisper_cpp_python-0.1.7/vendor/whisper.cpp/examples/whisper.objc/whisper.objc/SceneDelegate.h
+-rw-rw-r--   0 carlos    (1000) carlos    (1000)     2138 2023-05-08 13:31:02.000000 whisper_cpp_python-0.1.7/vendor/whisper.cpp/examples/whisper.objc/whisper.objc/SceneDelegate.m
+-rw-rw-r--   0 carlos    (1000) carlos    (1000)      761 2023-05-08 13:31:02.000000 whisper_cpp_python-0.1.7/vendor/whisper.cpp/examples/whisper.objc/whisper.objc/ViewController.h
+-rw-rw-r--   0 carlos    (1000) carlos    (1000)     9377 2023-05-08 13:31:02.000000 whisper_cpp_python-0.1.7/vendor/whisper.cpp/examples/whisper.objc/whisper.objc/ViewController.m
+-rw-rw-r--   0 carlos    (1000) carlos    (1000)      447 2023-05-08 13:31:02.000000 whisper_cpp_python-0.1.7/vendor/whisper.cpp/examples/whisper.objc/whisper.objc/main.m
+drwxrwxr-x   0 carlos    (1000) carlos    (1000)        0 2023-05-08 18:17:25.318169 whisper_cpp_python-0.1.7/vendor/whisper.cpp/examples/whisper.objc/whisper.objc.xcodeproj/
+-rw-rw-r--   0 carlos    (1000) carlos    (1000)    17120 2023-05-08 13:31:02.000000 whisper_cpp_python-0.1.7/vendor/whisper.cpp/examples/whisper.objc/whisper.objc.xcodeproj/project.pbxproj
+drwxrwxr-x   0 carlos    (1000) carlos    (1000)        0 2023-05-08 18:17:25.318169 whisper_cpp_python-0.1.7/vendor/whisper.cpp/examples/whisper.objc/whisper.objc.xcodeproj/project.xcworkspace/
+-rw-rw-r--   0 carlos    (1000) carlos    (1000)      135 2023-05-08 13:31:02.000000 whisper_cpp_python-0.1.7/vendor/whisper.cpp/examples/whisper.objc/whisper.objc.xcodeproj/project.xcworkspace/contents.xcworkspacedata
+drwxrwxr-x   0 carlos    (1000) carlos    (1000)        0 2023-05-08 18:17:25.318169 whisper_cpp_python-0.1.7/vendor/whisper.cpp/examples/whisper.objc/whisper.objc.xcodeproj/project.xcworkspace/xcshareddata/
+-rw-rw-r--   0 carlos    (1000) carlos    (1000)      238 2023-05-08 13:31:02.000000 whisper_cpp_python-0.1.7/vendor/whisper.cpp/examples/whisper.objc/whisper.objc.xcodeproj/project.xcworkspace/xcshareddata/IDEWorkspaceChecks.plist
+drwxrwxr-x   0 carlos    (1000) carlos    (1000)        0 2023-05-08 18:17:25.318169 whisper_cpp_python-0.1.7/vendor/whisper.cpp/examples/whisper.swiftui/
+-rw-rw-r--   0 carlos    (1000) carlos    (1000)     1410 2023-05-08 13:31:02.000000 whisper_cpp_python-0.1.7/vendor/whisper.cpp/examples/whisper.swiftui/README.md
+drwxrwxr-x   0 carlos    (1000) carlos    (1000)        0 2023-05-08 18:17:25.318169 whisper_cpp_python-0.1.7/vendor/whisper.cpp/examples/whisper.swiftui/whisper.cpp.swift/
+-rw-rw-r--   0 carlos    (1000) carlos    (1000)     2267 2023-05-08 13:31:02.000000 whisper_cpp_python-0.1.7/vendor/whisper.cpp/examples/whisper.swiftui/whisper.cpp.swift/LibWhisper.swift
+-rw-rw-r--   0 carlos    (1000) carlos    (1000)      123 2023-05-08 13:31:02.000000 whisper_cpp_python-0.1.7/vendor/whisper.cpp/examples/whisper.swiftui/whisper.cpp.swift/WhisperCppDemo-Bridging-Header.h
+drwxrwxr-x   0 carlos    (1000) carlos    (1000)        0 2023-05-08 18:17:25.318169 whisper_cpp_python-0.1.7/vendor/whisper.cpp/examples/whisper.swiftui/whisper.swiftui.demo/
+drwxrwxr-x   0 carlos    (1000) carlos    (1000)        0 2023-05-08 18:17:25.318169 whisper_cpp_python-0.1.7/vendor/whisper.cpp/examples/whisper.swiftui/whisper.swiftui.demo/Models/
+-rw-rw-r--   0 carlos    (1000) carlos    (1000)     4966 2023-05-08 13:31:02.000000 whisper_cpp_python-0.1.7/vendor/whisper.cpp/examples/whisper.swiftui/whisper.swiftui.demo/Models/WhisperState.swift
+drwxrwxr-x   0 carlos    (1000) carlos    (1000)        0 2023-05-08 18:17:25.270168 whisper_cpp_python-0.1.7/vendor/whisper.cpp/examples/whisper.swiftui/whisper.swiftui.demo/Resources/
+drwxrwxr-x   0 carlos    (1000) carlos    (1000)        0 2023-05-08 18:17:25.318169 whisper_cpp_python-0.1.7/vendor/whisper.cpp/examples/whisper.swiftui/whisper.swiftui.demo/Resources/models/
+-rw-rw-r--   0 carlos    (1000) carlos    (1000)        0 2023-05-08 13:31:02.000000 whisper_cpp_python-0.1.7/vendor/whisper.cpp/examples/whisper.swiftui/whisper.swiftui.demo/Resources/models/.gitignore
+drwxrwxr-x   0 carlos    (1000) carlos    (1000)        0 2023-05-08 18:17:25.318169 whisper_cpp_python-0.1.7/vendor/whisper.cpp/examples/whisper.swiftui/whisper.swiftui.demo/Resources/samples/
+-rw-rw-r--   0 carlos    (1000) carlos    (1000)        0 2023-05-08 13:31:02.000000 whisper_cpp_python-0.1.7/vendor/whisper.cpp/examples/whisper.swiftui/whisper.swiftui.demo/Resources/samples/.gitignore
+drwxrwxr-x   0 carlos    (1000) carlos    (1000)        0 2023-05-08 18:17:25.318169 whisper_cpp_python-0.1.7/vendor/whisper.cpp/examples/whisper.swiftui/whisper.swiftui.demo/UI/
+-rw-rw-r--   0 carlos    (1000) carlos    (1000)     1323 2023-05-08 13:31:02.000000 whisper_cpp_python-0.1.7/vendor/whisper.cpp/examples/whisper.swiftui/whisper.swiftui.demo/UI/ContentView.swift
+drwxrwxr-x   0 carlos    (1000) carlos    (1000)        0 2023-05-08 18:17:25.318169 whisper_cpp_python-0.1.7/vendor/whisper.cpp/examples/whisper.swiftui/whisper.swiftui.demo/Utils/
+-rw-rw-r--   0 carlos    (1000) carlos    (1000)     1065 2023-05-08 13:31:02.000000 whisper_cpp_python-0.1.7/vendor/whisper.cpp/examples/whisper.swiftui/whisper.swiftui.demo/Utils/Recorder.swift
+-rw-rw-r--   0 carlos    (1000) carlos    (1000)      394 2023-05-08 13:31:02.000000 whisper_cpp_python-0.1.7/vendor/whisper.cpp/examples/whisper.swiftui/whisper.swiftui.demo/Utils/RiffWaveUtils.swift
+-rw-rw-r--   0 carlos    (1000) carlos    (1000)      147 2023-05-08 13:31:02.000000 whisper_cpp_python-0.1.7/vendor/whisper.cpp/examples/whisper.swiftui/whisper.swiftui.demo/WhisperCppDemoApp.swift
+drwxrwxr-x   0 carlos    (1000) carlos    (1000)        0 2023-05-08 18:17:25.318169 whisper_cpp_python-0.1.7/vendor/whisper.cpp/examples/whisper.swiftui/whisper.swiftui.xcodeproj/
+-rw-rw-r--   0 carlos    (1000) carlos    (1000)       12 2023-05-08 13:31:02.000000 whisper_cpp_python-0.1.7/vendor/whisper.cpp/examples/whisper.swiftui/whisper.swiftui.xcodeproj/.gitignore
+-rw-rw-r--   0 carlos    (1000) carlos    (1000)    21447 2023-05-08 13:31:02.000000 whisper_cpp_python-0.1.7/vendor/whisper.cpp/examples/whisper.swiftui/whisper.swiftui.xcodeproj/project.pbxproj
+drwxrwxr-x   0 carlos    (1000) carlos    (1000)        0 2023-05-08 18:17:25.318169 whisper_cpp_python-0.1.7/vendor/whisper.cpp/examples/whisper.swiftui/whisper.swiftui.xcodeproj/project.xcworkspace/
+-rw-rw-r--   0 carlos    (1000) carlos    (1000)       25 2023-05-08 13:31:02.000000 whisper_cpp_python-0.1.7/vendor/whisper.cpp/examples/whisper.swiftui/whisper.swiftui.xcodeproj/project.xcworkspace/.gitignore
+drwxrwxr-x   0 carlos    (1000) carlos    (1000)        0 2023-05-08 18:17:25.318169 whisper_cpp_python-0.1.7/vendor/whisper.cpp/examples/whisper.swiftui/whisper.swiftui.xcodeproj/project.xcworkspace/xcshareddata/
+-rw-rw-r--   0 carlos    (1000) carlos    (1000)      238 2023-05-08 13:31:02.000000 whisper_cpp_python-0.1.7/vendor/whisper.cpp/examples/whisper.swiftui/whisper.swiftui.xcodeproj/project.xcworkspace/xcshareddata/IDEWorkspaceChecks.plist
+drwxrwxr-x   0 carlos    (1000) carlos    (1000)        0 2023-05-08 18:17:25.274168 whisper_cpp_python-0.1.7/vendor/whisper.cpp/examples/whisper.swiftui/whisper.swiftui.xcodeproj/xcshareddata/
+drwxrwxr-x   0 carlos    (1000) carlos    (1000)        0 2023-05-08 18:17:25.318169 whisper_cpp_python-0.1.7/vendor/whisper.cpp/examples/whisper.swiftui/whisper.swiftui.xcodeproj/xcshareddata/xcschemes/
+-rw-rw-r--   0 carlos    (1000) carlos    (1000)     3896 2023-05-08 13:31:02.000000 whisper_cpp_python-0.1.7/vendor/whisper.cpp/examples/whisper.swiftui/whisper.swiftui.xcodeproj/xcshareddata/xcschemes/WhisperCppDemo.xcscheme
+drwxrwxr-x   0 carlos    (1000) carlos    (1000)        0 2023-05-08 18:17:25.318169 whisper_cpp_python-0.1.7/vendor/whisper.cpp/examples/whisper.wasm/
+-rw-rw-r--   0 carlos    (1000) carlos    (1000)     1162 2023-05-08 13:31:02.000000 whisper_cpp_python-0.1.7/vendor/whisper.cpp/examples/whisper.wasm/CMakeLists.txt
+-rw-rw-r--   0 carlos    (1000) carlos    (1000)     1802 2023-05-08 13:31:02.000000 whisper_cpp_python-0.1.7/vendor/whisper.cpp/examples/whisper.wasm/README.md
+-rw-rw-r--   0 carlos    (1000) carlos    (1000)     3614 2023-05-08 13:31:02.000000 whisper_cpp_python-0.1.7/vendor/whisper.cpp/examples/whisper.wasm/emscripten.cpp
+-rw-rw-r--   0 carlos    (1000) carlos    (1000)    33017 2023-05-08 13:31:02.000000 whisper_cpp_python-0.1.7/vendor/whisper.cpp/examples/whisper.wasm/index-tmpl.html
+-rwxrwxr-x   0 carlos    (1000) carlos    (1000)     6932 2023-05-08 13:31:02.000000 whisper_cpp_python-0.1.7/vendor/whisper.cpp/examples/yt-wsp.sh
+drwxrwxr-x   0 carlos    (1000) carlos    (1000)        0 2023-05-08 18:17:25.318169 whisper_cpp_python-0.1.7/vendor/whisper.cpp/extra/
+-rwxrwxr-x   0 carlos    (1000) carlos    (1000)     2459 2023-05-08 13:31:02.000000 whisper_cpp_python-0.1.7/vendor/whisper.cpp/extra/bench-all.sh
+-rwxrwxr-x   0 carlos    (1000) carlos    (1000)     2113 2023-05-08 13:31:02.000000 whisper_cpp_python-0.1.7/vendor/whisper.cpp/extra/bench-wts.sh
+-rwxrwxr-x   0 carlos    (1000) carlos    (1000)      297 2023-05-08 13:31:02.000000 whisper_cpp_python-0.1.7/vendor/whisper.cpp/extra/convert-all.sh
+-rwxrwxr-x   0 carlos    (1000) carlos    (1000)     1152 2023-05-08 13:31:02.000000 whisper_cpp_python-0.1.7/vendor/whisper.cpp/extra/deploy-wasm.sh
+-rwxrwxr-x   0 carlos    (1000) carlos    (1000)     2034 2023-05-08 13:31:02.000000 whisper_cpp_python-0.1.7/vendor/whisper.cpp/extra/quantize-all.sh
+-rwxrwxr-x   0 carlos    (1000) carlos    (1000)      134 2023-05-08 13:31:02.000000 whisper_cpp_python-0.1.7/vendor/whisper.cpp/extra/sha-all.sh
+-rwxrwxr-x   0 carlos    (1000) carlos    (1000)      596 2023-05-08 13:31:02.000000 whisper_cpp_python-0.1.7/vendor/whisper.cpp/extra/sync-ggml.sh
+-rw-rw-r--   0 carlos    (1000) carlos    (1000)    24594 2023-05-08 13:31:02.000000 whisper_cpp_python-0.1.7/vendor/whisper.cpp/ggml-cuda.cu
+-rw-rw-r--   0 carlos    (1000) carlos    (1000)      638 2023-05-08 13:31:02.000000 whisper_cpp_python-0.1.7/vendor/whisper.cpp/ggml-cuda.h
+-rw-rw-r--   0 carlos    (1000) carlos    (1000)    13447 2023-05-08 13:31:02.000000 whisper_cpp_python-0.1.7/vendor/whisper.cpp/ggml-opencl.c
+-rw-rw-r--   0 carlos    (1000) carlos    (1000)      639 2023-05-08 13:31:02.000000 whisper_cpp_python-0.1.7/vendor/whisper.cpp/ggml-opencl.h
+-rw-rw-r--   0 carlos    (1000) carlos    (1000)   423265 2023-05-08 13:31:02.000000 whisper_cpp_python-0.1.7/vendor/whisper.cpp/ggml.c
+-rw-rw-r--   0 carlos    (1000) carlos    (1000)    31202 2023-05-08 13:31:02.000000 whisper_cpp_python-0.1.7/vendor/whisper.cpp/ggml.h
+drwxrwxr-x   0 carlos    (1000) carlos    (1000)        0 2023-05-08 18:17:25.326170 whisper_cpp_python-0.1.7/vendor/whisper.cpp/models/
+-rw-rw-r--   0 carlos    (1000) carlos    (1000)        6 2023-05-08 13:31:02.000000 whisper_cpp_python-0.1.7/vendor/whisper.cpp/models/.gitignore
+-rw-rw-r--   0 carlos    (1000) carlos    (1000)     3290 2023-05-08 13:31:02.000000 whisper_cpp_python-0.1.7/vendor/whisper.cpp/models/README.md
+-rw-rw-r--   0 carlos    (1000) carlos    (1000)     7376 2023-05-08 13:31:02.000000 whisper_cpp_python-0.1.7/vendor/whisper.cpp/models/convert-h5-to-ggml.py
+-rw-rw-r--   0 carlos    (1000) carlos    (1000)     9473 2023-05-08 13:31:02.000000 whisper_cpp_python-0.1.7/vendor/whisper.cpp/models/convert-pt-to-ggml.py
+-rw-rw-r--   0 carlos    (1000) carlos    (1000)    12853 2023-05-08 13:31:02.000000 whisper_cpp_python-0.1.7/vendor/whisper.cpp/models/convert-whisper-to-coreml.py
+-rwxrwxr-x   0 carlos    (1000) carlos    (1000)     2128 2023-05-08 13:31:02.000000 whisper_cpp_python-0.1.7/vendor/whisper.cpp/models/download-coreml-model.sh
+-rw-rw-r--   0 carlos    (1000) carlos    (1000)     1356 2023-05-08 13:31:02.000000 whisper_cpp_python-0.1.7/vendor/whisper.cpp/models/download-ggml-model.cmd
+-rwxrwxr-x   0 carlos    (1000) carlos    (1000)     2010 2023-05-08 13:31:02.000000 whisper_cpp_python-0.1.7/vendor/whisper.cpp/models/download-ggml-model.sh
+-rw-rw-r--   0 carlos    (1000) carlos    (1000)   575451 2023-05-08 13:31:02.000000 whisper_cpp_python-0.1.7/vendor/whisper.cpp/models/for-tests-ggml-base.bin
+-rw-rw-r--   0 carlos    (1000) carlos    (1000)   586836 2023-05-08 13:31:02.000000 whisper_cpp_python-0.1.7/vendor/whisper.cpp/models/for-tests-ggml-base.en.bin
+-rw-rw-r--   0 carlos    (1000) carlos    (1000)   575451 2023-05-08 13:31:02.000000 whisper_cpp_python-0.1.7/vendor/whisper.cpp/models/for-tests-ggml-large.bin
+-rw-rw-r--   0 carlos    (1000) carlos    (1000)   575451 2023-05-08 13:31:02.000000 whisper_cpp_python-0.1.7/vendor/whisper.cpp/models/for-tests-ggml-medium.bin
+-rw-rw-r--   0 carlos    (1000) carlos    (1000)   586836 2023-05-08 13:31:02.000000 whisper_cpp_python-0.1.7/vendor/whisper.cpp/models/for-tests-ggml-medium.en.bin
+-rw-rw-r--   0 carlos    (1000) carlos    (1000)   575451 2023-05-08 13:31:02.000000 whisper_cpp_python-0.1.7/vendor/whisper.cpp/models/for-tests-ggml-small.bin
+-rw-rw-r--   0 carlos    (1000) carlos    (1000)   586836 2023-05-08 13:31:02.000000 whisper_cpp_python-0.1.7/vendor/whisper.cpp/models/for-tests-ggml-small.en.bin
+-rw-rw-r--   0 carlos    (1000) carlos    (1000)   575451 2023-05-08 13:31:02.000000 whisper_cpp_python-0.1.7/vendor/whisper.cpp/models/for-tests-ggml-tiny.bin
+-rw-rw-r--   0 carlos    (1000) carlos    (1000)   586836 2023-05-08 13:31:02.000000 whisper_cpp_python-0.1.7/vendor/whisper.cpp/models/for-tests-ggml-tiny.en.bin
+-rwxrwxr-x   0 carlos    (1000) carlos    (1000)     1471 2023-05-08 13:31:02.000000 whisper_cpp_python-0.1.7/vendor/whisper.cpp/models/generate-coreml-interface.sh
+-rwxrwxr-x   0 carlos    (1000) carlos    (1000)      769 2023-05-08 13:31:02.000000 whisper_cpp_python-0.1.7/vendor/whisper.cpp/models/generate-coreml-model.sh
+drwxrwxr-x   0 carlos    (1000) carlos    (1000)        0 2023-05-08 18:17:25.326170 whisper_cpp_python-0.1.7/vendor/whisper.cpp/samples/
+-rw-rw-r--   0 carlos    (1000) carlos    (1000)        2 2023-05-08 13:31:02.000000 whisper_cpp_python-0.1.7/vendor/whisper.cpp/samples/.gitignore
+-rw-rw-r--   0 carlos    (1000) carlos    (1000)      367 2023-05-08 13:31:02.000000 whisper_cpp_python-0.1.7/vendor/whisper.cpp/samples/README.md
+-rw-rw-r--   0 carlos    (1000) carlos    (1000)   352078 2023-05-08 13:31:02.000000 whisper_cpp_python-0.1.7/vendor/whisper.cpp/samples/jfk.wav
+drwxrwxr-x   0 carlos    (1000) carlos    (1000)        0 2023-05-08 18:17:25.326170 whisper_cpp_python-0.1.7/vendor/whisper.cpp/tests/
+-rw-rw-r--   0 carlos    (1000) carlos    (1000)       22 2023-05-08 13:31:02.000000 whisper_cpp_python-0.1.7/vendor/whisper.cpp/tests/.gitignore
+-rw-rw-r--   0 carlos    (1000) carlos    (1000)     2712 2023-05-08 13:31:02.000000 whisper_cpp_python-0.1.7/vendor/whisper.cpp/tests/CMakeLists.txt
+-rw-rw-r--   0 carlos    (1000) carlos    (1000)     2101 2023-05-08 13:31:02.000000 whisper_cpp_python-0.1.7/vendor/whisper.cpp/tests/en-0-ref.txt
+-rw-rw-r--   0 carlos    (1000) carlos    (1000)     2221 2023-05-08 13:31:02.000000 whisper_cpp_python-0.1.7/vendor/whisper.cpp/tests/en-1-ref.txt
+-rw-rw-r--   0 carlos    (1000) carlos    (1000)      957 2023-05-08 13:31:02.000000 whisper_cpp_python-0.1.7/vendor/whisper.cpp/tests/en-2-ref.txt
+-rw-rw-r--   0 carlos    (1000) carlos    (1000)     1945 2023-05-08 13:31:02.000000 whisper_cpp_python-0.1.7/vendor/whisper.cpp/tests/es-0-ref.txt
+-rwxrwxr-x   0 carlos    (1000) carlos    (1000)     3432 2023-05-08 13:31:02.000000 whisper_cpp_python-0.1.7/vendor/whisper.cpp/tests/run-tests.sh
+-rw-rw-r--   0 carlos    (1000) carlos    (1000)     1645 2023-05-08 13:31:02.000000 whisper_cpp_python-0.1.7/vendor/whisper.cpp/tests/test-whisper.js
+-rw-rw-r--   0 carlos    (1000) carlos    (1000)   184690 2023-05-08 13:31:02.000000 whisper_cpp_python-0.1.7/vendor/whisper.cpp/whisper.cpp
+-rw-rw-r--   0 carlos    (1000) carlos    (1000)    23750 2023-05-08 13:31:02.000000 whisper_cpp_python-0.1.7/vendor/whisper.cpp/whisper.h
+drwxrwxr-x   0 carlos    (1000) carlos    (1000)        0 2023-05-08 18:17:25.326170 whisper_cpp_python-0.1.7/whisper_cpp_python/
+-rw-rw-r--   0 carlos    (1000) carlos    (1000)       23 2023-05-08 13:35:47.000000 whisper_cpp_python-0.1.7/whisper_cpp_python/__init__.py
+-rw-rw-r--   0 carlos    (1000) carlos    (1000)     1366 2023-05-08 13:35:47.000000 whisper_cpp_python-0.1.7/whisper_cpp_python/whisper.py
+-rw-rw-r--   0 carlos    (1000) carlos    (1000)    30640 2023-05-08 18:17:25.000000 whisper_cpp_python-0.1.7/whisper_cpp_python/whisper_cpp.py
+drwxrwxr-x   0 carlos    (1000) carlos    (1000)        0 2023-05-08 18:17:25.330170 whisper_cpp_python-0.1.7/whisper_cpp_python.egg-info/
+-rw-rw-r--   0 carlos    (1000) carlos    (1000)      447 2023-05-08 18:17:25.000000 whisper_cpp_python-0.1.7/whisper_cpp_python.egg-info/PKG-INFO
+-rw-rw-r--   0 carlos    (1000) carlos    (1000)    22209 2023-05-08 18:17:25.000000 whisper_cpp_python-0.1.7/whisper_cpp_python.egg-info/SOURCES.txt
+-rw-rw-r--   0 carlos    (1000) carlos    (1000)        1 2023-05-08 18:17:25.000000 whisper_cpp_python-0.1.7/whisper_cpp_python.egg-info/dependency_links.txt
+-rw-rw-r--   0 carlos    (1000) carlos    (1000)       22 2023-05-08 18:17:25.000000 whisper_cpp_python-0.1.7/whisper_cpp_python.egg-info/requires.txt
+-rw-rw-r--   0 carlos    (1000) carlos    (1000)       19 2023-05-08 18:17:25.000000 whisper_cpp_python-0.1.7/whisper_cpp_python.egg-info/top_level.txt
```

### Comparing `whisper_cpp_python-0.1.6/build.py` & `whisper_cpp_python-0.1.7/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,16 +1,12 @@
-"""Build script."""
-
+from skbuild import setup
+import skbuild.constants
 import shutil
-from distutils import log as distutils_log
-from pathlib import Path
-from typing import Any, Dict
 
-import skbuild
-import skbuild.constants
+from pathlib import Path
 
 from pycparser import c_ast, parse_file
 
 FILE = '''# auto-generated file
 import sys
 import os
 import ctypes
@@ -89,15 +85,15 @@
     @staticmethod
     def get_nested_type(node, ignore = {c_ast.Decl, c_ast.Typename}):
         typ = type(node)
         if typ in ignore:
             return WhisperCppFileGen.get_nested_type(node.type)
         return typ
 
-    def __init__(self, filename, fake_libc = 'whisper_cpp_python/vendor/pycparser/utils/fake_libc_include'):
+    def __init__(self, filename, fake_libc = 'vendor/pycparser/utils/fake_libc_include'):
         self.ast = parse_file(filename, use_cpp=True, cpp_args=['-E', f'-I{fake_libc}'], cpp_path='gcc')
         self.blocks = []
         self._output = None
         self._process()
 
     def _process(self):
         for node in self.ast:
@@ -205,68 +201,44 @@
         all_types = ', '.join(types)
         ret_f = f' -> {ret}:\n{self.T}return ' if ret else f':\n{self.T}'
         pyfunction = f'def {name}({args_typed}){ret_f}_lib.{name}({all_args})'
         all_block = f'{pyfunction}\n\n_lib.{name}.argtypes = [{all_types}]\n_lib.{name}.restype = {ret if ret else "None"}\n'
         self.blocks.append(all_block)
 
 
-__all__ = ("build",)
-
-
-def build(setup_kwargs: Dict[str, Any]) -> None:
-    """Build C-extensions."""
-    skbuild.setup(**setup_kwargs, script_args=["build_ext"])
-
-    src_dir = Path(skbuild.constants.CMAKE_INSTALL_DIR())
-    lib_dir = src_dir / "lib"
-    dest_dir = Path("whisper_cpp_python")
-    vendor = dest_dir / Path("vendor")
-
-
-    # Delete C-extensions copied in previous runs, just in case.
-    remove_files(dest_dir, "**/*.so")
-    remove_files(dest_dir, "**/*.dll")
-    remove_files(dest_dir, "**/*.dylib")
+if __name__ == '__main__':
+    this_directory = Path(__file__).parent
+    long_description = (this_directory / "README.md").read_text(encoding="utf-8")
 
     # Copy built C-extensions back to the project.
-    copy_files(lib_dir, dest_dir, "**/*.so")
-    copy_files(lib_dir, dest_dir, "**/*.dll")
-    copy_files(lib_dir, dest_dir, "**/*.dylib")
+    setup(
+        name="whisper_cpp_python",
+        description="A Python wrapper for whisper.cpp",
+        long_description=long_description,
+        long_description_content_type="text/markdown",
+        version="0.1.7",
+        author="Carlos Cardoso Dias",
+        author_email="carlosdias.dev@gmail.com",
+        license="MIT",
+        package_dir={"whisper_cpp_python": "whisper_cpp_python"},
+        packages=["whisper_cpp_python"],
+        install_requires=[
+            "librosa>=0.10.0.post2",
+        ],
+        python_requires=">=3.9",
+        classifiers=[
+            "Programming Language :: Python :: 3",
+            "Programming Language :: Python :: 3.9",
+            "Programming Language :: Python :: 3.10",
+            "Programming Language :: Python :: 3.11",
+        ],
+        include_package_data=True,
+        cmake_process_manifest_hook=lambda x: list(filter(lambda y: not y.endswith('.h'), x)),
+    )
 
     # generate whisper_cpp.py with whisper.h header file
-    c_header_file = src_dir / "include" / "whisper.h"
-    file_gen = WhisperCppFileGen(c_header_file, fake_libc = f'{dest_dir}/vendor/pycparser/utils/fake_libc_include')
+    dest_dir = Path("whisper_cpp_python")
+    c_header_file = "vendor/whisper.cpp/whisper.h"
+    file_gen = WhisperCppFileGen(c_header_file)
     file_gen.output(dest_dir / "whisper_cpp.py")
-    shutil.rmtree(vendor)
-
 
-def remove_files(target_dir: Path, pattern: str) -> None:
-    """Delete files matched with a glob pattern in a directory tree."""
-    for path in target_dir.glob(pattern):
-        if path.is_dir():
-            shutil.rmtree(path)
-        else:
-            path.unlink()
-        distutils_log.info(f"removed {path}")
 
-
-def copy_files(src_dir: Path, dest_dir: Path, pattern: str) -> None:
-    """Copy files matched with a glob pattern in a directory tree to another."""
-    for src in src_dir.glob(pattern):
-        dest = dest_dir / src.relative_to(src_dir)
-        if src.is_dir():
-            # NOTE: inefficient if subdirectories also match to the pattern.
-            copy_files(src, dest, "*")
-        else:
-            dest.parent.mkdir(parents=True, exist_ok=True)
-            shutil.copy2(src, dest)
-            distutils_log.info(f"copied {src} to {dest}")
-
-
-if __name__ == "__main__":
-    build({
-        'packages': ['whisper_cpp_python'],
-        'cmake_args': [
-            '-DBUILD_SHARED_LIBS:BOOL=ON',
-        ],
-        'cmake_source_dir': 'whisper_cpp_python/vendor/whisper.cpp',
-    })
```

### Comparing `whisper_cpp_python-0.1.6/whisper_cpp_python/vendor/pycparser/utils/fake_libc_include/X11/_X11_fake_typedefs.h` & `whisper_cpp_python-0.1.7/vendor/pycparser/utils/fake_libc_include/X11/_X11_fake_typedefs.h`

 * *Files identical despite different names*

### Comparing `whisper_cpp_python-0.1.6/whisper_cpp_python/vendor/pycparser/utils/fake_libc_include/_fake_defines.h` & `whisper_cpp_python-0.1.7/vendor/pycparser/utils/fake_libc_include/_fake_defines.h`

 * *Files identical despite different names*

### Comparing `whisper_cpp_python-0.1.6/whisper_cpp_python/vendor/pycparser/utils/fake_libc_include/_fake_typedefs.h` & `whisper_cpp_python-0.1.7/vendor/pycparser/utils/fake_libc_include/_fake_typedefs.h`

 * *Files identical despite different names*

### Comparing `whisper_cpp_python-0.1.6/whisper_cpp_python/vendor/pycparser/utils/fake_libc_include/zlib.h` & `whisper_cpp_python-0.1.7/vendor/pycparser/utils/fake_libc_include/zlib.h`

 * *Files identical despite different names*

### Comparing `whisper_cpp_python-0.1.6/whisper_cpp_python/vendor/whisper.cpp/.github/workflows/build.yml` & `whisper_cpp_python-0.1.7/vendor/whisper.cpp/.github/workflows/build.yml`

 * *Files identical despite different names*

### Comparing `whisper_cpp_python-0.1.6/whisper_cpp_python/vendor/whisper.cpp/.github/workflows/examples.yml` & `whisper_cpp_python-0.1.7/vendor/whisper.cpp/.github/workflows/examples.yml`

 * *Files identical despite different names*

### Comparing `whisper_cpp_python-0.1.6/whisper_cpp_python/vendor/whisper.cpp/.gitignore` & `whisper_cpp_python-0.1.7/vendor/whisper.cpp/.gitignore`

 * *Files identical despite different names*

### Comparing `whisper_cpp_python-0.1.6/whisper_cpp_python/vendor/whisper.cpp/CMakeLists.txt` & `whisper_cpp_python-0.1.7/vendor/whisper.cpp/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `whisper_cpp_python-0.1.6/whisper_cpp_python/vendor/whisper.cpp/LICENSE` & `whisper_cpp_python-0.1.7/vendor/whisper.cpp/LICENSE`

 * *Files identical despite different names*

### Comparing `whisper_cpp_python-0.1.6/whisper_cpp_python/vendor/whisper.cpp/Makefile` & `whisper_cpp_python-0.1.7/vendor/whisper.cpp/Makefile`

 * *Files identical despite different names*

### Comparing `whisper_cpp_python-0.1.6/whisper_cpp_python/vendor/whisper.cpp/README.md` & `whisper_cpp_python-0.1.7/vendor/whisper.cpp/README.md`

 * *Files identical despite different names*

### Comparing `whisper_cpp_python-0.1.6/whisper_cpp_python/vendor/whisper.cpp/bindings/CMakeLists.txt` & `whisper_cpp_python-0.1.7/vendor/whisper.cpp/bindings/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `whisper_cpp_python-0.1.6/whisper_cpp_python/vendor/whisper.cpp/bindings/go/LICENSE` & `whisper_cpp_python-0.1.7/vendor/whisper.cpp/bindings/go/LICENSE`

 * *Files identical despite different names*

### Comparing `whisper_cpp_python-0.1.6/whisper_cpp_python/vendor/whisper.cpp/bindings/go/Makefile` & `whisper_cpp_python-0.1.7/vendor/whisper.cpp/bindings/go/Makefile`

 * *Files identical despite different names*

### Comparing `whisper_cpp_python-0.1.6/whisper_cpp_python/vendor/whisper.cpp/bindings/go/README.md` & `whisper_cpp_python-0.1.7/vendor/whisper.cpp/bindings/go/README.md`

 * *Files identical despite different names*

### Comparing `whisper_cpp_python-0.1.6/whisper_cpp_python/vendor/whisper.cpp/bindings/go/examples/go-model-download/context.go` & `whisper_cpp_python-0.1.7/vendor/whisper.cpp/bindings/go/examples/go-model-download/context.go`

 * *Files identical despite different names*

### Comparing `whisper_cpp_python-0.1.6/whisper_cpp_python/vendor/whisper.cpp/bindings/go/examples/go-model-download/main.go` & `whisper_cpp_python-0.1.7/vendor/whisper.cpp/bindings/go/examples/go-model-download/main.go`

 * *Files identical despite different names*

### Comparing `whisper_cpp_python-0.1.6/whisper_cpp_python/vendor/whisper.cpp/bindings/go/examples/go-whisper/color.go` & `whisper_cpp_python-0.1.7/vendor/whisper.cpp/bindings/go/examples/go-whisper/color.go`

 * *Files identical despite different names*

### Comparing `whisper_cpp_python-0.1.6/whisper_cpp_python/vendor/whisper.cpp/bindings/go/examples/go-whisper/flags.go` & `whisper_cpp_python-0.1.7/vendor/whisper.cpp/bindings/go/examples/go-whisper/flags.go`

 * *Files identical despite different names*

### Comparing `whisper_cpp_python-0.1.6/whisper_cpp_python/vendor/whisper.cpp/bindings/go/examples/go-whisper/main.go` & `whisper_cpp_python-0.1.7/vendor/whisper.cpp/bindings/go/examples/go-whisper/main.go`

 * *Files identical despite different names*

### Comparing `whisper_cpp_python-0.1.6/whisper_cpp_python/vendor/whisper.cpp/bindings/go/examples/go-whisper/process.go` & `whisper_cpp_python-0.1.7/vendor/whisper.cpp/bindings/go/examples/go-whisper/process.go`

 * *Files identical despite different names*

### Comparing `whisper_cpp_python-0.1.6/whisper_cpp_python/vendor/whisper.cpp/bindings/go/go.sum` & `whisper_cpp_python-0.1.7/vendor/whisper.cpp/bindings/go/go.sum`

 * *Files identical despite different names*

### Comparing `whisper_cpp_python-0.1.6/whisper_cpp_python/vendor/whisper.cpp/bindings/go/params.go` & `whisper_cpp_python-0.1.7/vendor/whisper.cpp/bindings/go/params.go`

 * *Files identical despite different names*

### Comparing `whisper_cpp_python-0.1.6/whisper_cpp_python/vendor/whisper.cpp/bindings/go/pkg/whisper/consts.go` & `whisper_cpp_python-0.1.7/vendor/whisper.cpp/bindings/go/pkg/whisper/consts.go`

 * *Files identical despite different names*

### Comparing `whisper_cpp_python-0.1.6/whisper_cpp_python/vendor/whisper.cpp/bindings/go/pkg/whisper/context.go` & `whisper_cpp_python-0.1.7/vendor/whisper.cpp/bindings/go/pkg/whisper/context.go`

 * *Files identical despite different names*

### Comparing `whisper_cpp_python-0.1.6/whisper_cpp_python/vendor/whisper.cpp/bindings/go/pkg/whisper/context_test.go` & `whisper_cpp_python-0.1.7/vendor/whisper.cpp/bindings/go/pkg/whisper/context_test.go`

 * *Files identical despite different names*

### Comparing `whisper_cpp_python-0.1.6/whisper_cpp_python/vendor/whisper.cpp/bindings/go/pkg/whisper/interface.go` & `whisper_cpp_python-0.1.7/vendor/whisper.cpp/bindings/go/pkg/whisper/interface.go`

 * *Files identical despite different names*

### Comparing `whisper_cpp_python-0.1.6/whisper_cpp_python/vendor/whisper.cpp/bindings/go/pkg/whisper/model.go` & `whisper_cpp_python-0.1.7/vendor/whisper.cpp/bindings/go/pkg/whisper/model.go`

 * *Files identical despite different names*

### Comparing `whisper_cpp_python-0.1.6/whisper_cpp_python/vendor/whisper.cpp/bindings/go/samples/jfk.wav` & `whisper_cpp_python-0.1.7/vendor/whisper.cpp/bindings/go/samples/jfk.wav`

 * *Files identical despite different names*

### Comparing `whisper_cpp_python-0.1.6/whisper_cpp_python/vendor/whisper.cpp/bindings/go/whisper.go` & `whisper_cpp_python-0.1.7/vendor/whisper.cpp/bindings/go/whisper.go`

 * *Files identical despite different names*

### Comparing `whisper_cpp_python-0.1.6/whisper_cpp_python/vendor/whisper.cpp/bindings/go/whisper_test.go` & `whisper_cpp_python-0.1.7/vendor/whisper.cpp/bindings/go/whisper_test.go`

 * *Files identical despite different names*

### Comparing `whisper_cpp_python-0.1.6/whisper_cpp_python/vendor/whisper.cpp/bindings/ios/LICENSE` & `whisper_cpp_python-0.1.7/vendor/whisper.cpp/bindings/ios/LICENSE`

 * *Files identical despite different names*

### Comparing `whisper_cpp_python-0.1.6/whisper_cpp_python/vendor/whisper.cpp/bindings/ios/Makefile` & `whisper_cpp_python-0.1.7/vendor/whisper.cpp/bindings/ios/Makefile`

 * *Files identical despite different names*

### Comparing `whisper_cpp_python-0.1.6/whisper_cpp_python/vendor/whisper.cpp/bindings/ios/Makefile-tmpl` & `whisper_cpp_python-0.1.7/vendor/whisper.cpp/bindings/ios/Makefile-tmpl`

 * *Files identical despite different names*

### Comparing `whisper_cpp_python-0.1.6/whisper_cpp_python/vendor/whisper.cpp/bindings/ios/Package.swift` & `whisper_cpp_python-0.1.7/vendor/whisper.cpp/bindings/ios/Package.swift`

 * *Files identical despite different names*

### Comparing `whisper_cpp_python-0.1.6/whisper_cpp_python/vendor/whisper.cpp/bindings/ios/README.md` & `whisper_cpp_python-0.1.7/vendor/whisper.cpp/bindings/ios/README.md`

 * *Files identical despite different names*

### Comparing `whisper_cpp_python-0.1.6/whisper_cpp_python/vendor/whisper.cpp/bindings/ios/Sources/test-objc/main.m` & `whisper_cpp_python-0.1.7/vendor/whisper.cpp/bindings/ios/Sources/test-objc/main.m`

 * *Files identical despite different names*

### Comparing `whisper_cpp_python-0.1.6/whisper_cpp_python/vendor/whisper.cpp/bindings/ios/Sources/test-swift/main.swift` & `whisper_cpp_python-0.1.7/vendor/whisper.cpp/bindings/ios/Sources/test-swift/main.swift`

 * *Files identical despite different names*

### Comparing `whisper_cpp_python-0.1.6/whisper_cpp_python/vendor/whisper.cpp/bindings/ios/Sources/whisper/ggml.c` & `whisper_cpp_python-0.1.7/vendor/whisper.cpp/bindings/ios/Sources/whisper/ggml.c`

 * *Files identical despite different names*

### Comparing `whisper_cpp_python-0.1.6/whisper_cpp_python/vendor/whisper.cpp/bindings/ios/Sources/whisper/ggml.h` & `whisper_cpp_python-0.1.7/vendor/whisper.cpp/bindings/ios/Sources/whisper/ggml.h`

 * *Files identical despite different names*

### Comparing `whisper_cpp_python-0.1.6/whisper_cpp_python/vendor/whisper.cpp/bindings/ios/Sources/whisper/include/whisper.h` & `whisper_cpp_python-0.1.7/vendor/whisper.cpp/bindings/ios/Sources/whisper/include/whisper.h`

 * *Files identical despite different names*

### Comparing `whisper_cpp_python-0.1.6/whisper_cpp_python/vendor/whisper.cpp/bindings/ios/Sources/whisper/whisper.cpp` & `whisper_cpp_python-0.1.7/vendor/whisper.cpp/bindings/ios/Sources/whisper/whisper.cpp`

 * *Files identical despite different names*

### Comparing `whisper_cpp_python-0.1.6/whisper_cpp_python/vendor/whisper.cpp/bindings/ios/models/for-tests-ggml-base.en.bin` & `whisper_cpp_python-0.1.7/vendor/whisper.cpp/bindings/ios/models/for-tests-ggml-base.en.bin`

 * *Files identical despite different names*

### Comparing `whisper_cpp_python-0.1.6/whisper_cpp_python/vendor/whisper.cpp/bindings/javascript/CMakeLists.txt` & `whisper_cpp_python-0.1.7/vendor/whisper.cpp/bindings/javascript/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `whisper_cpp_python-0.1.6/whisper_cpp_python/vendor/whisper.cpp/bindings/javascript/README.md` & `whisper_cpp_python-0.1.7/vendor/whisper.cpp/bindings/javascript/README.md`

 * *Files identical despite different names*

### Comparing `whisper_cpp_python-0.1.6/whisper_cpp_python/vendor/whisper.cpp/bindings/javascript/emscripten.cpp` & `whisper_cpp_python-0.1.7/vendor/whisper.cpp/bindings/javascript/emscripten.cpp`

 * *Files identical despite different names*

### Comparing `whisper_cpp_python-0.1.6/whisper_cpp_python/vendor/whisper.cpp/bindings/javascript/libwhisper.worker.js` & `whisper_cpp_python-0.1.7/vendor/whisper.cpp/bindings/javascript/libwhisper.worker.js`

 * *Files identical despite different names*

### Comparing `whisper_cpp_python-0.1.6/whisper_cpp_python/vendor/whisper.cpp/bindings/javascript/package-tmpl.json` & `whisper_cpp_python-0.1.7/vendor/whisper.cpp/bindings/javascript/package-tmpl.json`

 * *Files identical despite different names*

### Comparing `whisper_cpp_python-0.1.6/whisper_cpp_python/vendor/whisper.cpp/bindings/javascript/package.json` & `whisper_cpp_python-0.1.7/vendor/whisper.cpp/bindings/javascript/package.json`

 * *Files identical despite different names*

### Comparing `whisper_cpp_python-0.1.6/whisper_cpp_python/vendor/whisper.cpp/bindings/javascript/whisper.js` & `whisper_cpp_python-0.1.7/vendor/whisper.cpp/bindings/javascript/whisper.js`

 * *Files identical despite different names*

### Comparing `whisper_cpp_python-0.1.6/whisper_cpp_python/vendor/whisper.cpp/bindings/ruby/ext/extconf.rb` & `whisper_cpp_python-0.1.7/vendor/whisper.cpp/bindings/ruby/ext/extconf.rb`

 * *Files identical despite different names*

### Comparing `whisper_cpp_python-0.1.6/whisper_cpp_python/vendor/whisper.cpp/bindings/ruby/ext/ruby_whisper.cpp` & `whisper_cpp_python-0.1.7/vendor/whisper.cpp/bindings/ruby/ext/ruby_whisper.cpp`

 * *Files identical despite different names*

### Comparing `whisper_cpp_python-0.1.6/whisper_cpp_python/vendor/whisper.cpp/bindings/ruby/tests/test_whisper.rb` & `whisper_cpp_python-0.1.7/vendor/whisper.cpp/bindings/ruby/tests/test_whisper.rb`

 * *Files identical despite different names*

### Comparing `whisper_cpp_python-0.1.6/whisper_cpp_python/vendor/whisper.cpp/cmake/BuildTypes.cmake` & `whisper_cpp_python-0.1.7/vendor/whisper.cpp/cmake/BuildTypes.cmake`

 * *Files identical despite different names*

### Comparing `whisper_cpp_python-0.1.6/whisper_cpp_python/vendor/whisper.cpp/cmake/GitVars.cmake` & `whisper_cpp_python-0.1.7/vendor/whisper.cpp/cmake/GitVars.cmake`

 * *Files identical despite different names*

### Comparing `whisper_cpp_python-0.1.6/whisper_cpp_python/vendor/whisper.cpp/coreml/whisper-decoder-impl.h` & `whisper_cpp_python-0.1.7/vendor/whisper.cpp/coreml/whisper-decoder-impl.h`

 * *Files identical despite different names*

### Comparing `whisper_cpp_python-0.1.6/whisper_cpp_python/vendor/whisper.cpp/coreml/whisper-decoder-impl.m` & `whisper_cpp_python-0.1.7/vendor/whisper.cpp/coreml/whisper-decoder-impl.m`

 * *Files identical despite different names*

### Comparing `whisper_cpp_python-0.1.6/whisper_cpp_python/vendor/whisper.cpp/coreml/whisper-encoder-impl.h` & `whisper_cpp_python-0.1.7/vendor/whisper.cpp/coreml/whisper-encoder-impl.h`

 * *Files identical despite different names*

### Comparing `whisper_cpp_python-0.1.6/whisper_cpp_python/vendor/whisper.cpp/coreml/whisper-encoder-impl.m` & `whisper_cpp_python-0.1.7/vendor/whisper.cpp/coreml/whisper-encoder-impl.m`

 * *Files identical despite different names*

### Comparing `whisper_cpp_python-0.1.6/whisper_cpp_python/vendor/whisper.cpp/coreml/whisper-encoder.h` & `whisper_cpp_python-0.1.7/vendor/whisper.cpp/coreml/whisper-encoder.h`

 * *Files identical despite different names*

### Comparing `whisper_cpp_python-0.1.6/whisper_cpp_python/vendor/whisper.cpp/coreml/whisper-encoder.mm` & `whisper_cpp_python-0.1.7/vendor/whisper.cpp/coreml/whisper-encoder.mm`

 * *Files identical despite different names*

### Comparing `whisper_cpp_python-0.1.6/whisper_cpp_python/vendor/whisper.cpp/examples/CMakeLists.txt` & `whisper_cpp_python-0.1.7/vendor/whisper.cpp/examples/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `whisper_cpp_python-0.1.6/whisper_cpp_python/vendor/whisper.cpp/examples/addon.node/CMakeLists.txt` & `whisper_cpp_python-0.1.7/vendor/whisper.cpp/examples/addon.node/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `whisper_cpp_python-0.1.6/whisper_cpp_python/vendor/whisper.cpp/examples/addon.node/README.md` & `whisper_cpp_python-0.1.7/vendor/whisper.cpp/examples/addon.node/README.md`

 * *Files identical despite different names*

### Comparing `whisper_cpp_python-0.1.6/whisper_cpp_python/vendor/whisper.cpp/examples/addon.node/__test__/whisper.spec.js` & `whisper_cpp_python-0.1.7/vendor/whisper.cpp/examples/addon.node/__test__/whisper.spec.js`

 * *Files identical despite different names*

### Comparing `whisper_cpp_python-0.1.6/whisper_cpp_python/vendor/whisper.cpp/examples/addon.node/addon.cpp` & `whisper_cpp_python-0.1.7/vendor/whisper.cpp/examples/addon.node/addon.cpp`

 * *Files identical despite different names*

### Comparing `whisper_cpp_python-0.1.6/whisper_cpp_python/vendor/whisper.cpp/examples/addon.node/index.js` & `whisper_cpp_python-0.1.7/vendor/whisper.cpp/examples/addon.node/index.js`

 * *Files identical despite different names*

### Comparing `whisper_cpp_python-0.1.6/whisper_cpp_python/vendor/whisper.cpp/examples/bench/README.md` & `whisper_cpp_python-0.1.7/vendor/whisper.cpp/examples/bench/README.md`

 * *Files identical despite different names*

### Comparing `whisper_cpp_python-0.1.6/whisper_cpp_python/vendor/whisper.cpp/examples/bench/bench.cpp` & `whisper_cpp_python-0.1.7/vendor/whisper.cpp/examples/bench/bench.cpp`

 * *Files identical despite different names*

### Comparing `whisper_cpp_python-0.1.6/whisper_cpp_python/vendor/whisper.cpp/examples/bench.wasm/CMakeLists.txt` & `whisper_cpp_python-0.1.7/vendor/whisper.cpp/examples/bench.wasm/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `whisper_cpp_python-0.1.6/whisper_cpp_python/vendor/whisper.cpp/examples/bench.wasm/emscripten.cpp` & `whisper_cpp_python-0.1.7/vendor/whisper.cpp/examples/bench.wasm/emscripten.cpp`

 * *Files identical despite different names*

### Comparing `whisper_cpp_python-0.1.6/whisper_cpp_python/vendor/whisper.cpp/examples/bench.wasm/index-tmpl.html` & `whisper_cpp_python-0.1.7/vendor/whisper.cpp/examples/bench.wasm/index-tmpl.html`

 * *Files identical despite different names*

### Comparing `whisper_cpp_python-0.1.6/whisper_cpp_python/vendor/whisper.cpp/examples/command/README.md` & `whisper_cpp_python-0.1.7/vendor/whisper.cpp/examples/command/README.md`

 * *Files identical despite different names*

### Comparing `whisper_cpp_python-0.1.6/whisper_cpp_python/vendor/whisper.cpp/examples/command/command.cpp` & `whisper_cpp_python-0.1.7/vendor/whisper.cpp/examples/command/command.cpp`

 * *Files identical despite different names*

### Comparing `whisper_cpp_python-0.1.6/whisper_cpp_python/vendor/whisper.cpp/examples/command.wasm/CMakeLists.txt` & `whisper_cpp_python-0.1.7/vendor/whisper.cpp/examples/command.wasm/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `whisper_cpp_python-0.1.6/whisper_cpp_python/vendor/whisper.cpp/examples/command.wasm/README.md` & `whisper_cpp_python-0.1.7/vendor/whisper.cpp/examples/command.wasm/README.md`

 * *Files identical despite different names*

### Comparing `whisper_cpp_python-0.1.6/whisper_cpp_python/vendor/whisper.cpp/examples/command.wasm/emscripten.cpp` & `whisper_cpp_python-0.1.7/vendor/whisper.cpp/examples/command.wasm/emscripten.cpp`

 * *Files identical despite different names*

### Comparing `whisper_cpp_python-0.1.6/whisper_cpp_python/vendor/whisper.cpp/examples/command.wasm/index-tmpl.html` & `whisper_cpp_python-0.1.7/vendor/whisper.cpp/examples/command.wasm/index-tmpl.html`

 * *Files identical despite different names*

### Comparing `whisper_cpp_python-0.1.6/whisper_cpp_python/vendor/whisper.cpp/examples/common-ggml.cpp` & `whisper_cpp_python-0.1.7/vendor/whisper.cpp/examples/common-ggml.cpp`

 * *Files identical despite different names*

### Comparing `whisper_cpp_python-0.1.6/whisper_cpp_python/vendor/whisper.cpp/examples/common-sdl.cpp` & `whisper_cpp_python-0.1.7/vendor/whisper.cpp/examples/common-sdl.cpp`

 * *Files identical despite different names*

### Comparing `whisper_cpp_python-0.1.6/whisper_cpp_python/vendor/whisper.cpp/examples/common-sdl.h` & `whisper_cpp_python-0.1.7/vendor/whisper.cpp/examples/common-sdl.h`

 * *Files identical despite different names*

### Comparing `whisper_cpp_python-0.1.6/whisper_cpp_python/vendor/whisper.cpp/examples/common.cpp` & `whisper_cpp_python-0.1.7/vendor/whisper.cpp/examples/common.cpp`

 * *Files identical despite different names*

### Comparing `whisper_cpp_python-0.1.6/whisper_cpp_python/vendor/whisper.cpp/examples/common.h` & `whisper_cpp_python-0.1.7/vendor/whisper.cpp/examples/common.h`

 * *Files identical despite different names*

### Comparing `whisper_cpp_python-0.1.6/whisper_cpp_python/vendor/whisper.cpp/examples/dr_wav.h` & `whisper_cpp_python-0.1.7/vendor/whisper.cpp/examples/dr_wav.h`

 * *Files identical despite different names*

### Comparing `whisper_cpp_python-0.1.6/whisper_cpp_python/vendor/whisper.cpp/examples/generate-karaoke.sh` & `whisper_cpp_python-0.1.7/vendor/whisper.cpp/examples/generate-karaoke.sh`

 * *Files identical despite different names*

### Comparing `whisper_cpp_python-0.1.6/whisper_cpp_python/vendor/whisper.cpp/examples/helpers.js` & `whisper_cpp_python-0.1.7/vendor/whisper.cpp/examples/helpers.js`

 * *Files identical despite different names*

### Comparing `whisper_cpp_python-0.1.6/whisper_cpp_python/vendor/whisper.cpp/examples/livestream.sh` & `whisper_cpp_python-0.1.7/vendor/whisper.cpp/examples/livestream.sh`

 * *Files identical despite different names*

### Comparing `whisper_cpp_python-0.1.6/whisper_cpp_python/vendor/whisper.cpp/examples/main/README.md` & `whisper_cpp_python-0.1.7/vendor/whisper.cpp/examples/main/README.md`

 * *Files identical despite different names*

### Comparing `whisper_cpp_python-0.1.6/whisper_cpp_python/vendor/whisper.cpp/examples/main/main.cpp` & `whisper_cpp_python-0.1.7/vendor/whisper.cpp/examples/main/main.cpp`

 * *Files identical despite different names*

### Comparing `whisper_cpp_python-0.1.6/whisper_cpp_python/vendor/whisper.cpp/examples/quantize/quantize.cpp` & `whisper_cpp_python-0.1.7/vendor/whisper.cpp/examples/quantize/quantize.cpp`

 * *Files identical despite different names*

### Comparing `whisper_cpp_python-0.1.6/whisper_cpp_python/vendor/whisper.cpp/examples/stream/README.md` & `whisper_cpp_python-0.1.7/vendor/whisper.cpp/examples/stream/README.md`

 * *Files identical despite different names*

### Comparing `whisper_cpp_python-0.1.6/whisper_cpp_python/vendor/whisper.cpp/examples/stream/stream.cpp` & `whisper_cpp_python-0.1.7/vendor/whisper.cpp/examples/stream/stream.cpp`

 * *Files identical despite different names*

### Comparing `whisper_cpp_python-0.1.6/whisper_cpp_python/vendor/whisper.cpp/examples/stream.wasm/CMakeLists.txt` & `whisper_cpp_python-0.1.7/vendor/whisper.cpp/examples/stream.wasm/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `whisper_cpp_python-0.1.6/whisper_cpp_python/vendor/whisper.cpp/examples/stream.wasm/emscripten.cpp` & `whisper_cpp_python-0.1.7/vendor/whisper.cpp/examples/stream.wasm/emscripten.cpp`

 * *Files identical despite different names*

### Comparing `whisper_cpp_python-0.1.6/whisper_cpp_python/vendor/whisper.cpp/examples/stream.wasm/index-tmpl.html` & `whisper_cpp_python-0.1.7/vendor/whisper.cpp/examples/stream.wasm/index-tmpl.html`

 * *Files identical despite different names*

### Comparing `whisper_cpp_python-0.1.6/whisper_cpp_python/vendor/whisper.cpp/examples/talk/README.md` & `whisper_cpp_python-0.1.7/vendor/whisper.cpp/examples/talk/README.md`

 * *Files identical despite different names*

### Comparing `whisper_cpp_python-0.1.6/whisper_cpp_python/vendor/whisper.cpp/examples/talk/eleven-labs.py` & `whisper_cpp_python-0.1.7/vendor/whisper.cpp/examples/talk/eleven-labs.py`

 * *Files identical despite different names*

### Comparing `whisper_cpp_python-0.1.6/whisper_cpp_python/vendor/whisper.cpp/examples/talk/gpt-2.cpp` & `whisper_cpp_python-0.1.7/vendor/whisper.cpp/examples/talk/gpt-2.cpp`

 * *Files identical despite different names*

### Comparing `whisper_cpp_python-0.1.6/whisper_cpp_python/vendor/whisper.cpp/examples/talk/gpt-2.h` & `whisper_cpp_python-0.1.7/vendor/whisper.cpp/examples/talk/gpt-2.h`

 * *Files identical despite different names*

### Comparing `whisper_cpp_python-0.1.6/whisper_cpp_python/vendor/whisper.cpp/examples/talk/speak.sh` & `whisper_cpp_python-0.1.7/vendor/whisper.cpp/examples/talk/speak.sh`

 * *Files identical despite different names*

### Comparing `whisper_cpp_python-0.1.6/whisper_cpp_python/vendor/whisper.cpp/examples/talk/talk.cpp` & `whisper_cpp_python-0.1.7/vendor/whisper.cpp/examples/talk/talk.cpp`

 * *Files identical despite different names*

### Comparing `whisper_cpp_python-0.1.6/whisper_cpp_python/vendor/whisper.cpp/examples/talk-llama/CMakeLists.txt` & `whisper_cpp_python-0.1.7/vendor/whisper.cpp/examples/talk-llama/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `whisper_cpp_python-0.1.6/whisper_cpp_python/vendor/whisper.cpp/examples/talk-llama/README.md` & `whisper_cpp_python-0.1.7/vendor/whisper.cpp/examples/talk-llama/README.md`

 * *Files identical despite different names*

### Comparing `whisper_cpp_python-0.1.6/whisper_cpp_python/vendor/whisper.cpp/examples/talk-llama/eleven-labs.py` & `whisper_cpp_python-0.1.7/vendor/whisper.cpp/examples/talk-llama/eleven-labs.py`

 * *Files identical despite different names*

### Comparing `whisper_cpp_python-0.1.6/whisper_cpp_python/vendor/whisper.cpp/examples/talk-llama/llama-util.h` & `whisper_cpp_python-0.1.7/vendor/whisper.cpp/examples/talk-llama/llama-util.h`

 * *Files identical despite different names*

### Comparing `whisper_cpp_python-0.1.6/whisper_cpp_python/vendor/whisper.cpp/examples/talk-llama/llama.cpp` & `whisper_cpp_python-0.1.7/vendor/whisper.cpp/examples/talk-llama/llama.cpp`

 * *Files identical despite different names*

### Comparing `whisper_cpp_python-0.1.6/whisper_cpp_python/vendor/whisper.cpp/examples/talk-llama/llama.h` & `whisper_cpp_python-0.1.7/vendor/whisper.cpp/examples/talk-llama/llama.h`

 * *Files identical despite different names*

### Comparing `whisper_cpp_python-0.1.6/whisper_cpp_python/vendor/whisper.cpp/examples/talk-llama/prompts/talk-alpaca.txt` & `whisper_cpp_python-0.1.7/vendor/whisper.cpp/examples/talk-llama/prompts/talk-alpaca.txt`

 * *Files identical despite different names*

### Comparing `whisper_cpp_python-0.1.6/whisper_cpp_python/vendor/whisper.cpp/examples/talk-llama/speak.sh` & `whisper_cpp_python-0.1.7/vendor/whisper.cpp/examples/talk-llama/speak.sh`

 * *Files identical despite different names*

### Comparing `whisper_cpp_python-0.1.6/whisper_cpp_python/vendor/whisper.cpp/examples/talk-llama/talk-llama.cpp` & `whisper_cpp_python-0.1.7/vendor/whisper.cpp/examples/talk-llama/talk-llama.cpp`

 * *Files identical despite different names*

### Comparing `whisper_cpp_python-0.1.6/whisper_cpp_python/vendor/whisper.cpp/examples/talk.wasm/CMakeLists.txt` & `whisper_cpp_python-0.1.7/vendor/whisper.cpp/examples/talk.wasm/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `whisper_cpp_python-0.1.6/whisper_cpp_python/vendor/whisper.cpp/examples/talk.wasm/README.md` & `whisper_cpp_python-0.1.7/vendor/whisper.cpp/examples/talk.wasm/README.md`

 * *Files identical despite different names*

### Comparing `whisper_cpp_python-0.1.6/whisper_cpp_python/vendor/whisper.cpp/examples/talk.wasm/emscripten.cpp` & `whisper_cpp_python-0.1.7/vendor/whisper.cpp/examples/talk.wasm/emscripten.cpp`

 * *Files identical despite different names*

### Comparing `whisper_cpp_python-0.1.6/whisper_cpp_python/vendor/whisper.cpp/examples/talk.wasm/gpt-2.cpp` & `whisper_cpp_python-0.1.7/vendor/whisper.cpp/examples/talk.wasm/gpt-2.cpp`

 * *Files identical despite different names*

### Comparing `whisper_cpp_python-0.1.6/whisper_cpp_python/vendor/whisper.cpp/examples/talk.wasm/gpt-2.h` & `whisper_cpp_python-0.1.7/vendor/whisper.cpp/examples/talk.wasm/gpt-2.h`

 * *Files identical despite different names*

### Comparing `whisper_cpp_python-0.1.6/whisper_cpp_python/vendor/whisper.cpp/examples/talk.wasm/index-tmpl.html` & `whisper_cpp_python-0.1.7/vendor/whisper.cpp/examples/talk.wasm/index-tmpl.html`

 * *Files identical despite different names*

### Comparing `whisper_cpp_python-0.1.6/whisper_cpp_python/vendor/whisper.cpp/examples/twitch.sh` & `whisper_cpp_python-0.1.7/vendor/whisper.cpp/examples/twitch.sh`

 * *Files identical despite different names*

### Comparing `whisper_cpp_python-0.1.6/whisper_cpp_python/vendor/whisper.cpp/examples/whisper.android/.idea/gradle.xml` & `whisper_cpp_python-0.1.7/vendor/whisper.cpp/examples/whisper.android/.idea/gradle.xml`

 * *Files identical despite different names*

### Comparing `whisper_cpp_python-0.1.6/whisper_cpp_python/vendor/whisper.cpp/examples/whisper.android/README.md` & `whisper_cpp_python-0.1.7/vendor/whisper.cpp/examples/whisper.android/README.md`

 * *Files identical despite different names*

### Comparing `whisper_cpp_python-0.1.6/whisper_cpp_python/vendor/whisper.cpp/examples/whisper.android/app/build.gradle` & `whisper_cpp_python-0.1.7/vendor/whisper.cpp/examples/whisper.android/app/build.gradle`

 * *Files identical despite different names*

### Comparing `whisper_cpp_python-0.1.6/whisper_cpp_python/vendor/whisper.cpp/examples/whisper.android/app/proguard-rules.pro` & `whisper_cpp_python-0.1.7/vendor/whisper.cpp/examples/whisper.android/app/proguard-rules.pro`

 * *Files identical despite different names*

### Comparing `whisper_cpp_python-0.1.6/whisper_cpp_python/vendor/whisper.cpp/examples/whisper.android/app/src/androidTest/java/com/whispercppdemo/ExampleInstrumentedTest.kt` & `whisper_cpp_python-0.1.7/vendor/whisper.cpp/examples/whisper.android/app/src/androidTest/java/com/whispercppdemo/ExampleInstrumentedTest.kt`

 * *Files identical despite different names*

### Comparing `whisper_cpp_python-0.1.6/whisper_cpp_python/vendor/whisper.cpp/examples/whisper.android/app/src/main/AndroidManifest.xml` & `whisper_cpp_python-0.1.7/vendor/whisper.cpp/examples/whisper.android/app/src/main/AndroidManifest.xml`

 * *Files identical despite different names*

### Comparing `whisper_cpp_python-0.1.6/whisper_cpp_python/vendor/whisper.cpp/examples/whisper.android/app/src/main/java/com/whispercppdemo/MainActivity.kt` & `whisper_cpp_python-0.1.7/vendor/whisper.cpp/examples/whisper.android/app/src/main/java/com/whispercppdemo/MainActivity.kt`

 * *Files identical despite different names*

### Comparing `whisper_cpp_python-0.1.6/whisper_cpp_python/vendor/whisper.cpp/examples/whisper.android/app/src/main/java/com/whispercppdemo/media/RiffWaveHelper.kt` & `whisper_cpp_python-0.1.7/vendor/whisper.cpp/examples/whisper.android/app/src/main/java/com/whispercppdemo/media/RiffWaveHelper.kt`

 * *Files identical despite different names*

### Comparing `whisper_cpp_python-0.1.6/whisper_cpp_python/vendor/whisper.cpp/examples/whisper.android/app/src/main/java/com/whispercppdemo/recorder/Recorder.kt` & `whisper_cpp_python-0.1.7/vendor/whisper.cpp/examples/whisper.android/app/src/main/java/com/whispercppdemo/recorder/Recorder.kt`

 * *Files identical despite different names*

### Comparing `whisper_cpp_python-0.1.6/whisper_cpp_python/vendor/whisper.cpp/examples/whisper.android/app/src/main/java/com/whispercppdemo/ui/main/MainScreen.kt` & `whisper_cpp_python-0.1.7/vendor/whisper.cpp/examples/whisper.android/app/src/main/java/com/whispercppdemo/ui/main/MainScreen.kt`

 * *Files identical despite different names*

### Comparing `whisper_cpp_python-0.1.6/whisper_cpp_python/vendor/whisper.cpp/examples/whisper.android/app/src/main/java/com/whispercppdemo/ui/main/MainScreenViewModel.kt` & `whisper_cpp_python-0.1.7/vendor/whisper.cpp/examples/whisper.android/app/src/main/java/com/whispercppdemo/ui/main/MainScreenViewModel.kt`

 * *Files identical despite different names*

### Comparing `whisper_cpp_python-0.1.6/whisper_cpp_python/vendor/whisper.cpp/examples/whisper.android/app/src/main/java/com/whispercppdemo/ui/theme/Theme.kt` & `whisper_cpp_python-0.1.7/vendor/whisper.cpp/examples/whisper.android/app/src/main/java/com/whispercppdemo/ui/theme/Theme.kt`

 * *Files identical despite different names*

### Comparing `whisper_cpp_python-0.1.6/whisper_cpp_python/vendor/whisper.cpp/examples/whisper.android/app/src/main/java/com/whispercppdemo/ui/theme/Type.kt` & `whisper_cpp_python-0.1.7/vendor/whisper.cpp/examples/whisper.android/app/src/main/java/com/whispercppdemo/ui/theme/Type.kt`

 * *Files identical despite different names*

### Comparing `whisper_cpp_python-0.1.6/whisper_cpp_python/vendor/whisper.cpp/examples/whisper.android/app/src/main/java/com/whispercppdemo/whisper/LibWhisper.kt` & `whisper_cpp_python-0.1.7/vendor/whisper.cpp/examples/whisper.android/app/src/main/java/com/whispercppdemo/whisper/LibWhisper.kt`

 * *Files identical despite different names*

### Comparing `whisper_cpp_python-0.1.6/whisper_cpp_python/vendor/whisper.cpp/examples/whisper.android/app/src/main/jni/whisper/Android.mk` & `whisper_cpp_python-0.1.7/vendor/whisper.cpp/examples/whisper.android/app/src/main/jni/whisper/Android.mk`

 * *Files identical despite different names*

### Comparing `whisper_cpp_python-0.1.6/whisper_cpp_python/vendor/whisper.cpp/examples/whisper.android/app/src/main/jni/whisper/Whisper.mk` & `whisper_cpp_python-0.1.7/vendor/whisper.cpp/examples/whisper.android/app/src/main/jni/whisper/Whisper.mk`

 * *Files identical despite different names*

### Comparing `whisper_cpp_python-0.1.6/whisper_cpp_python/vendor/whisper.cpp/examples/whisper.android/app/src/main/jni/whisper/jni.c` & `whisper_cpp_python-0.1.7/vendor/whisper.cpp/examples/whisper.android/app/src/main/jni/whisper/jni.c`

 * *Files identical despite different names*

### Comparing `whisper_cpp_python-0.1.6/whisper_cpp_python/vendor/whisper.cpp/examples/whisper.android/app/src/main/res/drawable/ic_launcher_background.xml` & `whisper_cpp_python-0.1.7/vendor/whisper.cpp/examples/whisper.android/app/src/main/res/drawable/ic_launcher_background.xml`

 * *Files identical despite different names*

### Comparing `whisper_cpp_python-0.1.6/whisper_cpp_python/vendor/whisper.cpp/examples/whisper.android/app/src/main/res/drawable/ic_launcher_foreground.xml` & `whisper_cpp_python-0.1.7/vendor/whisper.cpp/examples/whisper.android/app/src/main/res/drawable/ic_launcher_foreground.xml`

 * *Files identical despite different names*

### Comparing `whisper_cpp_python-0.1.6/whisper_cpp_python/vendor/whisper.cpp/examples/whisper.android/app/src/main/res/xml/data_extraction_rules.xml` & `whisper_cpp_python-0.1.7/vendor/whisper.cpp/examples/whisper.android/app/src/main/res/xml/data_extraction_rules.xml`

 * *Files identical despite different names*

### Comparing `whisper_cpp_python-0.1.6/whisper_cpp_python/vendor/whisper.cpp/examples/whisper.android/gradle/wrapper/gradle-wrapper.jar` & `whisper_cpp_python-0.1.7/vendor/whisper.cpp/examples/whisper.android/gradle/wrapper/gradle-wrapper.jar`

 * *Files identical despite different names*

### Comparing `whisper_cpp_python-0.1.6/whisper_cpp_python/vendor/whisper.cpp/examples/whisper.android/gradle.properties` & `whisper_cpp_python-0.1.7/vendor/whisper.cpp/examples/whisper.android/gradle.properties`

 * *Files identical despite different names*

### Comparing `whisper_cpp_python-0.1.6/whisper_cpp_python/vendor/whisper.cpp/examples/whisper.android/gradlew` & `whisper_cpp_python-0.1.7/vendor/whisper.cpp/examples/whisper.android/gradlew`

 * *Files identical despite different names*

### Comparing `whisper_cpp_python-0.1.6/whisper_cpp_python/vendor/whisper.cpp/examples/whisper.android/gradlew.bat` & `whisper_cpp_python-0.1.7/vendor/whisper.cpp/examples/whisper.android/gradlew.bat`

 * *Files identical despite different names*

### Comparing `whisper_cpp_python-0.1.6/whisper_cpp_python/vendor/whisper.cpp/examples/whisper.nvim/README.md` & `whisper_cpp_python-0.1.7/vendor/whisper.cpp/examples/whisper.nvim/README.md`

 * *Files identical despite different names*

### Comparing `whisper_cpp_python-0.1.6/whisper_cpp_python/vendor/whisper.cpp/examples/whisper.nvim/whisper.nvim` & `whisper_cpp_python-0.1.7/vendor/whisper.cpp/examples/whisper.nvim/whisper.nvim`

 * *Files identical despite different names*

### Comparing `whisper_cpp_python-0.1.6/whisper_cpp_python/vendor/whisper.cpp/examples/whisper.objc/README.md` & `whisper_cpp_python-0.1.7/vendor/whisper.cpp/examples/whisper.objc/README.md`

 * *Files identical despite different names*

### Comparing `whisper_cpp_python-0.1.6/whisper_cpp_python/vendor/whisper.cpp/examples/whisper.objc/whisper.objc/AppDelegate.m` & `whisper_cpp_python-0.1.7/vendor/whisper.cpp/examples/whisper.objc/whisper.objc/AppDelegate.m`

 * *Files identical despite different names*

### Comparing `whisper_cpp_python-0.1.6/whisper_cpp_python/vendor/whisper.cpp/examples/whisper.objc/whisper.objc/Base.lproj/LaunchScreen.storyboard` & `whisper_cpp_python-0.1.7/vendor/whisper.cpp/examples/whisper.objc/whisper.objc/Base.lproj/LaunchScreen.storyboard`

 * *Files identical despite different names*

### Comparing `whisper_cpp_python-0.1.6/whisper_cpp_python/vendor/whisper.cpp/examples/whisper.objc/whisper.objc/Base.lproj/Main.storyboard` & `whisper_cpp_python-0.1.7/vendor/whisper.cpp/examples/whisper.objc/whisper.objc/Base.lproj/Main.storyboard`

 * *Files identical despite different names*

### Comparing `whisper_cpp_python-0.1.6/whisper_cpp_python/vendor/whisper.cpp/examples/whisper.objc/whisper.objc/Info.plist` & `whisper_cpp_python-0.1.7/vendor/whisper.cpp/examples/whisper.objc/whisper.objc/Info.plist`

 * *Files identical despite different names*

### Comparing `whisper_cpp_python-0.1.6/whisper_cpp_python/vendor/whisper.cpp/examples/whisper.objc/whisper.objc/SceneDelegate.m` & `whisper_cpp_python-0.1.7/vendor/whisper.cpp/examples/whisper.objc/whisper.objc/SceneDelegate.m`

 * *Files identical despite different names*

### Comparing `whisper_cpp_python-0.1.6/whisper_cpp_python/vendor/whisper.cpp/examples/whisper.objc/whisper.objc/ViewController.h` & `whisper_cpp_python-0.1.7/vendor/whisper.cpp/examples/whisper.objc/whisper.objc/ViewController.h`

 * *Files identical despite different names*

### Comparing `whisper_cpp_python-0.1.6/whisper_cpp_python/vendor/whisper.cpp/examples/whisper.objc/whisper.objc/ViewController.m` & `whisper_cpp_python-0.1.7/vendor/whisper.cpp/examples/whisper.objc/whisper.objc/ViewController.m`

 * *Files identical despite different names*

### Comparing `whisper_cpp_python-0.1.6/whisper_cpp_python/vendor/whisper.cpp/examples/whisper.objc/whisper.objc.xcodeproj/project.pbxproj` & `whisper_cpp_python-0.1.7/vendor/whisper.cpp/examples/whisper.objc/whisper.objc.xcodeproj/project.pbxproj`

 * *Files identical despite different names*

### Comparing `whisper_cpp_python-0.1.6/whisper_cpp_python/vendor/whisper.cpp/examples/whisper.swiftui/README.md` & `whisper_cpp_python-0.1.7/vendor/whisper.cpp/examples/whisper.swiftui/README.md`

 * *Files identical despite different names*

### Comparing `whisper_cpp_python-0.1.6/whisper_cpp_python/vendor/whisper.cpp/examples/whisper.swiftui/whisper.cpp.swift/LibWhisper.swift` & `whisper_cpp_python-0.1.7/vendor/whisper.cpp/examples/whisper.swiftui/whisper.cpp.swift/LibWhisper.swift`

 * *Files identical despite different names*

### Comparing `whisper_cpp_python-0.1.6/whisper_cpp_python/vendor/whisper.cpp/examples/whisper.swiftui/whisper.swiftui.demo/Models/WhisperState.swift` & `whisper_cpp_python-0.1.7/vendor/whisper.cpp/examples/whisper.swiftui/whisper.swiftui.demo/Models/WhisperState.swift`

 * *Files identical despite different names*

### Comparing `whisper_cpp_python-0.1.6/whisper_cpp_python/vendor/whisper.cpp/examples/whisper.swiftui/whisper.swiftui.demo/UI/ContentView.swift` & `whisper_cpp_python-0.1.7/vendor/whisper.cpp/examples/whisper.swiftui/whisper.swiftui.demo/UI/ContentView.swift`

 * *Files identical despite different names*

### Comparing `whisper_cpp_python-0.1.6/whisper_cpp_python/vendor/whisper.cpp/examples/whisper.swiftui/whisper.swiftui.demo/Utils/Recorder.swift` & `whisper_cpp_python-0.1.7/vendor/whisper.cpp/examples/whisper.swiftui/whisper.swiftui.demo/Utils/Recorder.swift`

 * *Files identical despite different names*

### Comparing `whisper_cpp_python-0.1.6/whisper_cpp_python/vendor/whisper.cpp/examples/whisper.swiftui/whisper.swiftui.xcodeproj/project.pbxproj` & `whisper_cpp_python-0.1.7/vendor/whisper.cpp/examples/whisper.swiftui/whisper.swiftui.xcodeproj/project.pbxproj`

 * *Files identical despite different names*

### Comparing `whisper_cpp_python-0.1.6/whisper_cpp_python/vendor/whisper.cpp/examples/whisper.swiftui/whisper.swiftui.xcodeproj/xcshareddata/xcschemes/WhisperCppDemo.xcscheme` & `whisper_cpp_python-0.1.7/vendor/whisper.cpp/examples/whisper.swiftui/whisper.swiftui.xcodeproj/xcshareddata/xcschemes/WhisperCppDemo.xcscheme`

 * *Files identical despite different names*

### Comparing `whisper_cpp_python-0.1.6/whisper_cpp_python/vendor/whisper.cpp/examples/whisper.wasm/CMakeLists.txt` & `whisper_cpp_python-0.1.7/vendor/whisper.cpp/examples/whisper.wasm/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `whisper_cpp_python-0.1.6/whisper_cpp_python/vendor/whisper.cpp/examples/whisper.wasm/README.md` & `whisper_cpp_python-0.1.7/vendor/whisper.cpp/examples/whisper.wasm/README.md`

 * *Files identical despite different names*

### Comparing `whisper_cpp_python-0.1.6/whisper_cpp_python/vendor/whisper.cpp/examples/whisper.wasm/emscripten.cpp` & `whisper_cpp_python-0.1.7/vendor/whisper.cpp/examples/whisper.wasm/emscripten.cpp`

 * *Files identical despite different names*

### Comparing `whisper_cpp_python-0.1.6/whisper_cpp_python/vendor/whisper.cpp/examples/whisper.wasm/index-tmpl.html` & `whisper_cpp_python-0.1.7/vendor/whisper.cpp/examples/whisper.wasm/index-tmpl.html`

 * *Files identical despite different names*

### Comparing `whisper_cpp_python-0.1.6/whisper_cpp_python/vendor/whisper.cpp/examples/yt-wsp.sh` & `whisper_cpp_python-0.1.7/vendor/whisper.cpp/examples/yt-wsp.sh`

 * *Files identical despite different names*

### Comparing `whisper_cpp_python-0.1.6/whisper_cpp_python/vendor/whisper.cpp/extra/bench-all.sh` & `whisper_cpp_python-0.1.7/vendor/whisper.cpp/extra/bench-all.sh`

 * *Files identical despite different names*

### Comparing `whisper_cpp_python-0.1.6/whisper_cpp_python/vendor/whisper.cpp/extra/bench-wts.sh` & `whisper_cpp_python-0.1.7/vendor/whisper.cpp/extra/bench-wts.sh`

 * *Files identical despite different names*

### Comparing `whisper_cpp_python-0.1.6/whisper_cpp_python/vendor/whisper.cpp/extra/deploy-wasm.sh` & `whisper_cpp_python-0.1.7/vendor/whisper.cpp/extra/deploy-wasm.sh`

 * *Files identical despite different names*

### Comparing `whisper_cpp_python-0.1.6/whisper_cpp_python/vendor/whisper.cpp/extra/quantize-all.sh` & `whisper_cpp_python-0.1.7/vendor/whisper.cpp/extra/quantize-all.sh`

 * *Files identical despite different names*

### Comparing `whisper_cpp_python-0.1.6/whisper_cpp_python/vendor/whisper.cpp/extra/sync-ggml.sh` & `whisper_cpp_python-0.1.7/vendor/whisper.cpp/extra/sync-ggml.sh`

 * *Files identical despite different names*

### Comparing `whisper_cpp_python-0.1.6/whisper_cpp_python/vendor/whisper.cpp/ggml-cuda.cu` & `whisper_cpp_python-0.1.7/vendor/whisper.cpp/ggml-cuda.cu`

 * *Files identical despite different names*

### Comparing `whisper_cpp_python-0.1.6/whisper_cpp_python/vendor/whisper.cpp/ggml-cuda.h` & `whisper_cpp_python-0.1.7/vendor/whisper.cpp/ggml-cuda.h`

 * *Files identical despite different names*

### Comparing `whisper_cpp_python-0.1.6/whisper_cpp_python/vendor/whisper.cpp/ggml-opencl.c` & `whisper_cpp_python-0.1.7/vendor/whisper.cpp/ggml-opencl.c`

 * *Files identical despite different names*

### Comparing `whisper_cpp_python-0.1.6/whisper_cpp_python/vendor/whisper.cpp/ggml-opencl.h` & `whisper_cpp_python-0.1.7/vendor/whisper.cpp/ggml-opencl.h`

 * *Files identical despite different names*

### Comparing `whisper_cpp_python-0.1.6/whisper_cpp_python/vendor/whisper.cpp/ggml.c` & `whisper_cpp_python-0.1.7/vendor/whisper.cpp/ggml.c`

 * *Files identical despite different names*

### Comparing `whisper_cpp_python-0.1.6/whisper_cpp_python/vendor/whisper.cpp/ggml.h` & `whisper_cpp_python-0.1.7/vendor/whisper.cpp/ggml.h`

 * *Files identical despite different names*

### Comparing `whisper_cpp_python-0.1.6/whisper_cpp_python/vendor/whisper.cpp/models/README.md` & `whisper_cpp_python-0.1.7/vendor/whisper.cpp/models/README.md`

 * *Files identical despite different names*

### Comparing `whisper_cpp_python-0.1.6/whisper_cpp_python/vendor/whisper.cpp/models/convert-h5-to-ggml.py` & `whisper_cpp_python-0.1.7/vendor/whisper.cpp/models/convert-h5-to-ggml.py`

 * *Files identical despite different names*

### Comparing `whisper_cpp_python-0.1.6/whisper_cpp_python/vendor/whisper.cpp/models/convert-pt-to-ggml.py` & `whisper_cpp_python-0.1.7/vendor/whisper.cpp/models/convert-pt-to-ggml.py`

 * *Files identical despite different names*

### Comparing `whisper_cpp_python-0.1.6/whisper_cpp_python/vendor/whisper.cpp/models/convert-whisper-to-coreml.py` & `whisper_cpp_python-0.1.7/vendor/whisper.cpp/models/convert-whisper-to-coreml.py`

 * *Files identical despite different names*

### Comparing `whisper_cpp_python-0.1.6/whisper_cpp_python/vendor/whisper.cpp/models/download-coreml-model.sh` & `whisper_cpp_python-0.1.7/vendor/whisper.cpp/models/download-coreml-model.sh`

 * *Files identical despite different names*

### Comparing `whisper_cpp_python-0.1.6/whisper_cpp_python/vendor/whisper.cpp/models/download-ggml-model.cmd` & `whisper_cpp_python-0.1.7/vendor/whisper.cpp/models/download-ggml-model.cmd`

 * *Files identical despite different names*

### Comparing `whisper_cpp_python-0.1.6/whisper_cpp_python/vendor/whisper.cpp/models/download-ggml-model.sh` & `whisper_cpp_python-0.1.7/vendor/whisper.cpp/models/download-ggml-model.sh`

 * *Files identical despite different names*

### Comparing `whisper_cpp_python-0.1.6/whisper_cpp_python/vendor/whisper.cpp/models/for-tests-ggml-base.bin` & `whisper_cpp_python-0.1.7/vendor/whisper.cpp/models/for-tests-ggml-base.bin`

 * *Files identical despite different names*

### Comparing `whisper_cpp_python-0.1.6/whisper_cpp_python/vendor/whisper.cpp/models/for-tests-ggml-base.en.bin` & `whisper_cpp_python-0.1.7/vendor/whisper.cpp/models/for-tests-ggml-base.en.bin`

 * *Files identical despite different names*

### Comparing `whisper_cpp_python-0.1.6/whisper_cpp_python/vendor/whisper.cpp/models/for-tests-ggml-large.bin` & `whisper_cpp_python-0.1.7/vendor/whisper.cpp/models/for-tests-ggml-large.bin`

 * *Files identical despite different names*

### Comparing `whisper_cpp_python-0.1.6/whisper_cpp_python/vendor/whisper.cpp/models/for-tests-ggml-medium.bin` & `whisper_cpp_python-0.1.7/vendor/whisper.cpp/models/for-tests-ggml-medium.bin`

 * *Files identical despite different names*

### Comparing `whisper_cpp_python-0.1.6/whisper_cpp_python/vendor/whisper.cpp/models/for-tests-ggml-medium.en.bin` & `whisper_cpp_python-0.1.7/vendor/whisper.cpp/models/for-tests-ggml-medium.en.bin`

 * *Files identical despite different names*

### Comparing `whisper_cpp_python-0.1.6/whisper_cpp_python/vendor/whisper.cpp/models/for-tests-ggml-small.bin` & `whisper_cpp_python-0.1.7/vendor/whisper.cpp/models/for-tests-ggml-small.bin`

 * *Files identical despite different names*

### Comparing `whisper_cpp_python-0.1.6/whisper_cpp_python/vendor/whisper.cpp/models/for-tests-ggml-small.en.bin` & `whisper_cpp_python-0.1.7/vendor/whisper.cpp/models/for-tests-ggml-small.en.bin`

 * *Files identical despite different names*

### Comparing `whisper_cpp_python-0.1.6/whisper_cpp_python/vendor/whisper.cpp/models/for-tests-ggml-tiny.bin` & `whisper_cpp_python-0.1.7/vendor/whisper.cpp/models/for-tests-ggml-tiny.bin`

 * *Files identical despite different names*

### Comparing `whisper_cpp_python-0.1.6/whisper_cpp_python/vendor/whisper.cpp/models/for-tests-ggml-tiny.en.bin` & `whisper_cpp_python-0.1.7/vendor/whisper.cpp/models/for-tests-ggml-tiny.en.bin`

 * *Files identical despite different names*

### Comparing `whisper_cpp_python-0.1.6/whisper_cpp_python/vendor/whisper.cpp/models/generate-coreml-interface.sh` & `whisper_cpp_python-0.1.7/vendor/whisper.cpp/models/generate-coreml-interface.sh`

 * *Files identical despite different names*

### Comparing `whisper_cpp_python-0.1.6/whisper_cpp_python/vendor/whisper.cpp/models/generate-coreml-model.sh` & `whisper_cpp_python-0.1.7/vendor/whisper.cpp/models/generate-coreml-model.sh`

 * *Files identical despite different names*

### Comparing `whisper_cpp_python-0.1.6/whisper_cpp_python/vendor/whisper.cpp/samples/jfk.wav` & `whisper_cpp_python-0.1.7/vendor/whisper.cpp/samples/jfk.wav`

 * *Files identical despite different names*

### Comparing `whisper_cpp_python-0.1.6/whisper_cpp_python/vendor/whisper.cpp/tests/CMakeLists.txt` & `whisper_cpp_python-0.1.7/vendor/whisper.cpp/tests/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `whisper_cpp_python-0.1.6/whisper_cpp_python/vendor/whisper.cpp/tests/en-0-ref.txt` & `whisper_cpp_python-0.1.7/vendor/whisper.cpp/tests/en-0-ref.txt`

 * *Files identical despite different names*

### Comparing `whisper_cpp_python-0.1.6/whisper_cpp_python/vendor/whisper.cpp/tests/en-1-ref.txt` & `whisper_cpp_python-0.1.7/vendor/whisper.cpp/tests/en-1-ref.txt`

 * *Files identical despite different names*

### Comparing `whisper_cpp_python-0.1.6/whisper_cpp_python/vendor/whisper.cpp/tests/en-2-ref.txt` & `whisper_cpp_python-0.1.7/vendor/whisper.cpp/tests/en-2-ref.txt`

 * *Files identical despite different names*

### Comparing `whisper_cpp_python-0.1.6/whisper_cpp_python/vendor/whisper.cpp/tests/es-0-ref.txt` & `whisper_cpp_python-0.1.7/vendor/whisper.cpp/tests/es-0-ref.txt`

 * *Files identical despite different names*

### Comparing `whisper_cpp_python-0.1.6/whisper_cpp_python/vendor/whisper.cpp/tests/run-tests.sh` & `whisper_cpp_python-0.1.7/vendor/whisper.cpp/tests/run-tests.sh`

 * *Files identical despite different names*

### Comparing `whisper_cpp_python-0.1.6/whisper_cpp_python/vendor/whisper.cpp/tests/test-whisper.js` & `whisper_cpp_python-0.1.7/vendor/whisper.cpp/tests/test-whisper.js`

 * *Files identical despite different names*

### Comparing `whisper_cpp_python-0.1.6/whisper_cpp_python/vendor/whisper.cpp/whisper.cpp` & `whisper_cpp_python-0.1.7/vendor/whisper.cpp/whisper.cpp`

 * *Files identical despite different names*

### Comparing `whisper_cpp_python-0.1.6/whisper_cpp_python/vendor/whisper.cpp/whisper.h` & `whisper_cpp_python-0.1.7/vendor/whisper.cpp/whisper.h`

 * *Files identical despite different names*

### Comparing `whisper_cpp_python-0.1.6/whisper_cpp_python/whisper.py` & `whisper_cpp_python-0.1.7/whisper_cpp_python/whisper.py`

 * *Files identical despite different names*

