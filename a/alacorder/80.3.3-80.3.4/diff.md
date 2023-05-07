# Comparing `tmp/alacorder-80.3.3.tar.gz` & `tmp/alacorder-80.3.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "alacorder-80.3.3.tar", max compression
+gzip compressed data, was "alacorder-80.3.4.tar", max compression
```

## Comparing `alacorder-80.3.3.tar` & `alacorder-80.3.4.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0     1066 2023-02-07 05:47:31.000000 alacorder-80.3.3/LICENSE
--rw-r--r--   0        0        0     6789 2023-05-07 22:01:18.137829 alacorder-80.3.3/README.md
--rw-r--r--   0        0        0      697 2023-05-07 21:59:36.126679 alacorder-80.3.3/pyproject.toml
--rw-r--r--   0        0        0        0 2023-05-02 17:21:37.916960 alacorder-80.3.3/src/alacorder/__init__.py
--rw-r--r--   0        0        0   221073 2023-05-07 22:00:07.188277 alacorder-80.3.3/src/alacorder/__main__.py
--rw-r--r--   0        0        0   221073 2023-05-07 22:00:11.679171 alacorder-80.3.3/src/alacorder/alac.py
--rw-r--r--   0        0        0     7718 1970-01-01 00:00:00.000000 alacorder-80.3.3/PKG-INFO
+-rw-r--r--   0        0        0     1066 2023-02-07 05:47:31.000000 alacorder-80.3.4/LICENSE
+-rw-r--r--   0        0        0     6786 2023-05-07 22:10:54.002102 alacorder-80.3.4/README.md
+-rw-r--r--   0        0        0      697 2023-05-07 22:11:59.124818 alacorder-80.3.4/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-05-02 17:21:37.916960 alacorder-80.3.4/src/alacorder/__init__.py
+-rw-r--r--   0        0        0   221073 2023-05-07 22:11:33.793994 alacorder-80.3.4/src/alacorder/__main__.py
+-rw-r--r--   0        0        0   221073 2023-05-07 22:11:26.874563 alacorder-80.3.4/src/alacorder/alac.py
+-rw-r--r--   0        0        0     7715 1970-01-01 00:00:00.000000 alacorder-80.3.4/PKG-INFO
```

### Comparing `alacorder-80.3.3/LICENSE` & `alacorder-80.3.4/LICENSE`

 * *Files identical despite different names*

### Comparing `alacorder-80.3.3/README.md` & `alacorder-80.3.4/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -332,94 +332,94 @@
 000014b0: 792c 2074 6261 6c2c 2070 7472 5d5d 0a0a  y, tbal, ptr]]..
 000014c0: 6361 7365 7320 3d20 706c 2e44 6174 6146  cases = pl.DataF
 000014d0: 7261 6d65 2872 6f77 7329 0a0a 6361 7365  rame(rows)..case
 000014e0: 732e 7772 6974 655f 6578 6365 6c28 222f  s.write_excel("/
 000014f0: 5573 6572 732f 6372 696d 736f 6e2f 4465  Users/crimson/De
 00001500: 736b 746f 702f 5475 7477 696c 6572 2f73  sktop/Tutwiler/s
 00001510: 756d 6d61 7279 2e78 6c73 7822 290a 0a60  ummary.xlsx")..`
-00001520: 6060 0a0a 2323 2045 7874 656e 6469 6e67  ``..## Extending
-00001530: 2041 6c61 636f 7264 6572 2077 6974 6820   Alacorder with 
-00001540: 6070 6f6c 6172 7360 2061 6e64 206f 7468  `polars` and oth
-00001550: 6572 2074 6f6f 6c73 0a0a 416c 6163 6f72  er tools..Alacor
-00001560: 6465 7220 7275 6e73 206f 6e20 5b60 706f  der runs on [`po
-00001570: 6c61 7273 605d 2868 7474 7073 3a2f 2f67  lars`](https://g
-00001580: 6974 6875 622e 636f 6d2f 706f 6c61 2d72  ithub.com/pola-r
-00001590: 732f 706f 6c61 7273 292c 2061 2064 6174  s/polars), a dat
-000015a0: 6166 7261 6d65 7320 6c69 6272 6172 7920  aframes library 
-000015b0: 796f 7520 6361 6e20 7573 6520 746f 2077  you can use to w
-000015c0: 6f72 6b20 7769 7468 2061 6e64 2061 6e61  ork with and ana
-000015d0: 6c79 7a65 2074 6162 756c 6172 2064 6174  lyze tabular dat
-000015e0: 612e 2060 706f 6c61 7273 6020 6361 6e20  a. `polars` can 
-000015f0: 7265 6164 2066 726f 6d20 616e 6420 7772  read from and wr
-00001600: 6974 6520 746f 2061 6c6c 206d 616a 6f72  ite to all major
-00001610: 2064 6174 6120 7374 6f72 6167 6520 666f   data storage fo
-00001620: 726d 6174 732e 2049 7420 6361 6e20 636f  rmats. It can co
-00001630: 6e6e 6563 7420 746f 2061 2077 6964 6520  nnect to a wide 
-00001640: 7661 7269 6574 7920 6f66 2073 6572 7669  variety of servi
-00001650: 6365 7320 746f 2070 726f 7669 6465 2066  ces to provide f
-00001660: 6f72 2065 6173 7920 696d 706f 7274 2061  or easy import a
-00001670: 6e64 2065 7870 6f72 742e 0a0a 6060 6070  nd export...```p
-00001680: 7974 686f 6e0a 696d 706f 7274 2070 6f6c  ython.import pol
-00001690: 6172 7320 6173 2070 6c0a 636f 6e74 656e  ars as pl.conten
-000016a0: 7473 203d 2070 6c2e 7265 6164 5f6a 736f  ts = pl.read_jso
-000016b0: 6e28 222f 7061 7468 2f74 6f2f 6172 6368  n("/path/to/arch
-000016c0: 6976 652e 6a73 6f6e 2229 0a60 6060 0a0a  ive.json").```..
-000016d0: 4966 2079 6f75 2077 6f75 6c64 206c 696b  If you would lik
-000016e0: 6520 746f 2076 6973 7561 6c69 7a65 2064  e to visualize d
-000016f0: 6174 6120 7769 7468 6f75 7420 6578 706f  ata without expo
-00001700: 7274 696e 6720 746f 2045 7863 656c 206f  rting to Excel o
-00001710: 7220 616e 6f74 6865 7220 666f 726d 6174  r another format
-00001720: 2c20 6372 6561 7465 2061 2060 6a75 7079  , create a `jupy
-00001730: 7465 7220 6e6f 7465 626f 6f6b 6020 616e  ter notebook` an
-00001740: 6420 696e 7374 616c 6c20 746f 6f6c 7320  d install tools 
-00001750: 6c69 6b65 2060 6d61 7470 6c6f 746c 6962  like `matplotlib
-00001760: 602c 2060 7461 6275 6c61 7465 602c 2061  `, `tabulate`, a
-00001770: 6e64 2060 6974 6162 6c65 7360 2074 6f20  nd `itables` to 
-00001780: 6765 7420 7374 6172 7465 642e 205b 4a75  get started. [Ju
-00001790: 7079 7465 7220 4e6f 7465 626f 6f6b 5d28  pyter Notebook](
-000017a0: 6874 7470 733a 2f2f 646f 6373 2e6a 7570  https://docs.jup
-000017b0: 7974 6572 2e6f 7267 2f65 6e2f 6c61 7465  yter.org/en/late
-000017c0: 7374 2f73 7461 7274 2f69 6e64 6578 2e68  st/start/index.h
-000017d0: 746d 6c29 2069 7320 6120 5079 7468 6f6e  tml) is a Python
-000017e0: 2070 726f 6a65 6374 2079 6f75 2063 616e   project you can
-000017f0: 2075 7365 2074 6f20 6372 6561 7465 2069   use to create i
-00001800: 6e74 6572 6163 7469 7665 206e 6f74 6562  nteractive noteb
-00001810: 6f6f 6b73 2066 6f72 2064 6174 6120 616e  ooks for data an
-00001820: 616c 7973 6973 2061 6e64 206f 7468 6572  alysis and other
-00001830: 2070 7572 706f 7365 732e 2049 7420 6361   purposes. It ca
-00001840: 6e20 6265 2069 6e73 7461 6c6c 6564 2075  n be installed u
-00001850: 7369 6e67 2060 7069 7020 696e 7374 616c  sing `pip instal
-00001860: 6c20 6a75 7079 7465 7260 206f 7220 6070  l jupyter` or `p
-00001870: 6970 3320 696e 7374 616c 6c20 6a75 7079  ip3 install jupy
-00001880: 7465 7260 2061 6e64 206c 6175 6e63 6865  ter` and launche
-00001890: 6420 7573 696e 6720 606a 7570 7974 6572  d using `jupyter
-000018a0: 206e 6f74 6562 6f6f 6b60 2e20 596f 7572   notebook`. Your
-000018b0: 2064 6576 6963 6520 6d61 7920 616c 7265   device may alre
-000018c0: 6164 7920 6265 2065 7175 6970 7065 6420  ady be equipped 
-000018d0: 746f 2076 6965 7720 602e 6970 796e 6260  to view `.ipynb`
-000018e0: 206e 6f74 6562 6f6f 6b73 2e20 0a0a 2323   notebooks. ..##
-000018f0: 202a 2a52 6573 6f75 7263 6573 2a2a 0a2a   **Resources**.*
-00001900: 205b 6070 6f6c 6172 7360 2075 7365 7220   [`polars` user 
-00001910: 6775 6964 655d 2868 7474 7073 3a2f 2f70  guide](https://p
-00001920: 6f6c 612d 7273 2e67 6974 6875 622e 696f  ola-rs.github.io
-00001930: 2f70 6f6c 6172 732d 626f 6f6b 2f75 7365  /polars-book/use
-00001940: 722d 6775 6964 652f 696e 6465 782e 6874  r-guide/index.ht
-00001950: 6d6c 290a 2a20 5b72 6567 6578 2063 6865  ml).* [regex che
-00001960: 6174 2073 6865 6574 5d28 6874 7470 733a  at sheet](https:
-00001970: 2f2f 7777 772e 7265 7865 6767 2e63 6f6d  //www.rexegg.com
-00001980: 2f72 6567 6578 2d71 7569 636b 7374 6172  /regex-quickstar
-00001990: 742e 6874 6d6c 290a 2a20 5b41 6e61 636f  t.html).* [Anaco
-000019a0: 6e64 6120 2874 7574 6f72 6961 6c73 206f  nda (tutorials o
-000019b0: 6e20 7079 7468 6f6e 2064 6174 6120 616e  n python data an
-000019c0: 616c 7973 6973 295d 2868 7474 7073 3a2f  alysis)](https:/
-000019d0: 2f77 7777 2e61 6e61 636f 6e64 612e 636f  /www.anaconda.co
-000019e0: 6d2f 6f70 656e 2d73 6f75 7263 6529 0a2a  m/open-source).*
-000019f0: 205b 5468 6520 5079 7468 6f6e 2054 7574   [The Python Tut
-00001a00: 6f72 6961 6c5d 2868 7474 7073 3a2f 2f64  orial](https://d
-00001a10: 6f63 732e 7079 7468 6f6e 2e6f 7267 2f33  ocs.python.org/3
-00001a20: 2f74 7574 6f72 6961 6c2f 290a 2a20 5b4a  /tutorial/).* [J
-00001a30: 7570 7974 6572 204e 6f74 6562 6f6f 6b20  upyter Notebook 
-00001a40: 696e 7472 6f64 7563 7469 6f6e 5d28 6874  introduction](ht
-00001a50: 7470 733a 2f2f 7265 616c 7079 7468 6f6e  tps://realpython
-00001a60: 2e63 6f6d 2f6a 7570 7974 6572 2d6e 6f74  .com/jupyter-not
-00001a70: 6562 6f6f 6b2d 696e 7472 6f64 7563 7469  ebook-introducti
-00001a80: 6f6e 2f29 0a                             on/).
+00001520: 6060 0a0a 2323 2045 7874 656e 6420 416c  ``..## Extend Al
+00001530: 6163 6f72 6465 7220 7769 7468 2060 706f  acorder with `po
+00001540: 6c61 7273 6020 616e 6420 6f74 6865 7220  lars` and other 
+00001550: 746f 6f6c 730a 0a41 6c61 636f 7264 6572  tools..Alacorder
+00001560: 2072 756e 7320 6f6e 205b 6070 6f6c 6172   runs on [`polar
+00001570: 7360 5d28 6874 7470 733a 2f2f 6769 7468  s`](https://gith
+00001580: 7562 2e63 6f6d 2f70 6f6c 612d 7273 2f70  ub.com/pola-rs/p
+00001590: 6f6c 6172 7329 2c20 6120 6461 7461 6672  olars), a datafr
+000015a0: 616d 6573 206c 6962 7261 7279 2079 6f75  ames library you
+000015b0: 2063 616e 2075 7365 2074 6f20 776f 726b   can use to work
+000015c0: 2077 6974 6820 616e 6420 616e 616c 797a   with and analyz
+000015d0: 6520 7461 6275 6c61 7220 6461 7461 2e20  e tabular data. 
+000015e0: 6070 6f6c 6172 7360 2063 616e 2072 6561  `polars` can rea
+000015f0: 6420 6672 6f6d 2061 6e64 2077 7269 7465  d from and write
+00001600: 2074 6f20 616c 6c20 6d61 6a6f 7220 6461   to all major da
+00001610: 7461 2073 746f 7261 6765 2066 6f72 6d61  ta storage forma
+00001620: 7473 2e20 4974 2063 616e 2063 6f6e 6e65  ts. It can conne
+00001630: 6374 2074 6f20 6120 7769 6465 2076 6172  ct to a wide var
+00001640: 6965 7479 206f 6620 7365 7276 6963 6573  iety of services
+00001650: 2074 6f20 7072 6f76 6964 6520 666f 7220   to provide for 
+00001660: 6561 7379 2069 6d70 6f72 7420 616e 6420  easy import and 
+00001670: 6578 706f 7274 2e0a 0a60 6060 7079 7468  export...```pyth
+00001680: 6f6e 0a69 6d70 6f72 7420 706f 6c61 7273  on.import polars
+00001690: 2061 7320 706c 0a63 6f6e 7465 6e74 7320   as pl.contents 
+000016a0: 3d20 706c 2e72 6561 645f 6a73 6f6e 2822  = pl.read_json("
+000016b0: 2f70 6174 682f 746f 2f61 7263 6869 7665  /path/to/archive
+000016c0: 2e6a 736f 6e22 290a 6060 600a 0a49 6620  .json").```..If 
+000016d0: 796f 7520 776f 756c 6420 6c69 6b65 2074  you would like t
+000016e0: 6f20 7669 7375 616c 697a 6520 6461 7461  o visualize data
+000016f0: 2077 6974 686f 7574 2065 7870 6f72 7469   without exporti
+00001700: 6e67 2074 6f20 4578 6365 6c20 6f72 2061  ng to Excel or a
+00001710: 6e6f 7468 6572 2066 6f72 6d61 742c 2063  nother format, c
+00001720: 7265 6174 6520 6120 606a 7570 7974 6572  reate a `jupyter
+00001730: 206e 6f74 6562 6f6f 6b60 2061 6e64 2069   notebook` and i
+00001740: 6e73 7461 6c6c 2074 6f6f 6c73 206c 696b  nstall tools lik
+00001750: 6520 606d 6174 706c 6f74 6c69 6260 2c20  e `matplotlib`, 
+00001760: 6074 6162 756c 6174 6560 2c20 616e 6420  `tabulate`, and 
+00001770: 6069 7461 626c 6573 6020 746f 2067 6574  `itables` to get
+00001780: 2073 7461 7274 6564 2e20 5b4a 7570 7974   started. [Jupyt
+00001790: 6572 204e 6f74 6562 6f6f 6b5d 2868 7474  er Notebook](htt
+000017a0: 7073 3a2f 2f64 6f63 732e 6a75 7079 7465  ps://docs.jupyte
+000017b0: 722e 6f72 672f 656e 2f6c 6174 6573 742f  r.org/en/latest/
+000017c0: 7374 6172 742f 696e 6465 782e 6874 6d6c  start/index.html
+000017d0: 2920 6973 2061 2050 7974 686f 6e20 7072  ) is a Python pr
+000017e0: 6f6a 6563 7420 796f 7520 6361 6e20 7573  oject you can us
+000017f0: 6520 746f 2063 7265 6174 6520 696e 7465  e to create inte
+00001800: 7261 6374 6976 6520 6e6f 7465 626f 6f6b  ractive notebook
+00001810: 7320 666f 7220 6461 7461 2061 6e61 6c79  s for data analy
+00001820: 7369 7320 616e 6420 6f74 6865 7220 7075  sis and other pu
+00001830: 7270 6f73 6573 2e20 4974 2063 616e 2062  rposes. It can b
+00001840: 6520 696e 7374 616c 6c65 6420 7573 696e  e installed usin
+00001850: 6720 6070 6970 2069 6e73 7461 6c6c 206a  g `pip install j
+00001860: 7570 7974 6572 6020 6f72 2060 7069 7033  upyter` or `pip3
+00001870: 2069 6e73 7461 6c6c 206a 7570 7974 6572   install jupyter
+00001880: 6020 616e 6420 6c61 756e 6368 6564 2075  ` and launched u
+00001890: 7369 6e67 2060 6a75 7079 7465 7220 6e6f  sing `jupyter no
+000018a0: 7465 626f 6f6b 602e 2059 6f75 7220 6465  tebook`. Your de
+000018b0: 7669 6365 206d 6179 2061 6c72 6561 6479  vice may already
+000018c0: 2062 6520 6571 7569 7070 6564 2074 6f20   be equipped to 
+000018d0: 7669 6577 2060 2e69 7079 6e62 6020 6e6f  view `.ipynb` no
+000018e0: 7465 626f 6f6b 732e 200a 0a23 2320 2a2a  tebooks. ..## **
+000018f0: 5265 736f 7572 6365 732a 2a0a 2a20 5b60  Resources**.* [`
+00001900: 706f 6c61 7273 6020 7573 6572 2067 7569  polars` user gui
+00001910: 6465 5d28 6874 7470 733a 2f2f 706f 6c61  de](https://pola
+00001920: 2d72 732e 6769 7468 7562 2e69 6f2f 706f  -rs.github.io/po
+00001930: 6c61 7273 2d62 6f6f 6b2f 7573 6572 2d67  lars-book/user-g
+00001940: 7569 6465 2f69 6e64 6578 2e68 746d 6c29  uide/index.html)
+00001950: 0a2a 205b 7265 6765 7820 6368 6561 7420  .* [regex cheat 
+00001960: 7368 6565 745d 2868 7474 7073 3a2f 2f77  sheet](https://w
+00001970: 7777 2e72 6578 6567 672e 636f 6d2f 7265  ww.rexegg.com/re
+00001980: 6765 782d 7175 6963 6b73 7461 7274 2e68  gex-quickstart.h
+00001990: 746d 6c29 0a2a 205b 416e 6163 6f6e 6461  tml).* [Anaconda
+000019a0: 2028 7475 746f 7269 616c 7320 6f6e 2070   (tutorials on p
+000019b0: 7974 686f 6e20 6461 7461 2061 6e61 6c79  ython data analy
+000019c0: 7369 7329 5d28 6874 7470 733a 2f2f 7777  sis)](https://ww
+000019d0: 772e 616e 6163 6f6e 6461 2e63 6f6d 2f6f  w.anaconda.com/o
+000019e0: 7065 6e2d 736f 7572 6365 290a 2a20 5b54  pen-source).* [T
+000019f0: 6865 2050 7974 686f 6e20 5475 746f 7269  he Python Tutori
+00001a00: 616c 5d28 6874 7470 733a 2f2f 646f 6373  al](https://docs
+00001a10: 2e70 7974 686f 6e2e 6f72 672f 332f 7475  .python.org/3/tu
+00001a20: 746f 7269 616c 2f29 0a2a 205b 4a75 7079  torial/).* [Jupy
+00001a30: 7465 7220 4e6f 7465 626f 6f6b 2069 6e74  ter Notebook int
+00001a40: 726f 6475 6374 696f 6e5d 2868 7474 7073  roduction](https
+00001a50: 3a2f 2f72 6561 6c70 7974 686f 6e2e 636f  ://realpython.co
+00001a60: 6d2f 6a75 7079 7465 722d 6e6f 7465 626f  m/jupyter-notebo
+00001a70: 6f6b 2d69 6e74 726f 6475 6374 696f 6e2f  ok-introduction/
+00001a80: 290a                                     ).
```

### Comparing `alacorder-80.3.3/src/alacorder/__main__.py` & `alacorder-80.3.4/src/alacorder/__main__.py`

 * *Files 0% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 
 Dependencies: python 3.9+, brotli 1.0.9, click 8.1.3, polars 0.17.6, PyMuPDF 1.21.1, PySimpleGUI 4.60.4, selenium 4.8.3, tqdm 4.65.0, xlsx2csv 0.8.1, XlsxWriter 3.0.9
 
 """
 
 name = "ALACORDER"
 long_version = "snowpalace"
-version = "80.3.3"
+version = "80.3.4"
 
 _autoload_graphical_user_interface = False
 
 import polars as pl
 import os, sys, time, glob, re, math
 import click, fitz, selenium, xlsxwriter
 from tqdm.auto import tqdm
```

### Comparing `alacorder-80.3.3/src/alacorder/alac.py` & `alacorder-80.3.4/src/alacorder/alac.py`

 * *Files 0% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 
 Dependencies: python 3.9+, brotli 1.0.9, click 8.1.3, polars 0.17.6, PyMuPDF 1.21.1, PySimpleGUI 4.60.4, selenium 4.8.3, tqdm 4.65.0, xlsx2csv 0.8.1, XlsxWriter 3.0.9
 
 """
 
 name = "ALACORDER"
 long_version = "snowpalace"
-version = "80.3.3"
+version = "80.3.4"
 
 _autoload_graphical_user_interface = False
 
 import polars as pl
 import os, sys, time, glob, re, math
 import click, fitz, selenium, xlsxwriter
 from tqdm.auto import tqdm
```

### Comparing `alacorder-80.3.3/PKG-INFO` & `alacorder-80.3.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alacorder
-Version: 80.3.3
+Version: 80.3.4
 Summary: Alacorder collects and processes Alacourt case detail PDFs into data tables suitable for research purposes.
 License: MIT
 Author: Sam Robson
 Author-email: sbrobson@crimson.ua.edu
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
@@ -135,15 +135,15 @@
 
 cases = pl.DataFrame(rows)
 
 cases.write_excel("/Users/crimson/Desktop/Tutwiler/summary.xlsx")
 
 ```
 
-## Extending Alacorder with `polars` and other tools
+## Extend Alacorder with `polars` and other tools
 
 Alacorder runs on [`polars`](https://github.com/pola-rs/polars), a dataframes library you can use to work with and analyze tabular data. `polars` can read from and write to all major data storage formats. It can connect to a wide variety of services to provide for easy import and export.
 
 ```python
 import polars as pl
 contents = pl.read_json("/path/to/archive.json")
 ```
```

