# Comparing `tmp/webint-0.1.8.tar.gz` & `tmp/webint-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "webint-0.1.8.tar", max compression
+gzip compressed data, was "webint-0.1.9.tar", max compression
```

## Comparing `webint-0.1.8.tar` & `webint-0.1.9.tar`

### file list

```diff
@@ -1,318 +1,318 @@
--rw-r--r--   0        0        0      454 2023-01-27 00:43:42.480109 webint-0.1.8/README.md
--rw-r--r--   0        0        0     1754 2023-02-20 21:27:35.124915 webint-0.1.8/pyproject.toml
--rw-r--r--   0        0        0     1287 2023-02-18 00:57:16.443038 webint-0.1.8/web/__init__.py
--rw-r--r--   0        0        0     7748 2023-02-19 02:03:37.006296 webint-0.1.8/web/__main__.py
--rw-r--r--   0        0        0    46838 2023-02-19 01:25:14.719556 webint-0.1.8/web/framework/__init__.py
--rw-r--r--   0        0        0     1233 2023-01-27 00:43:42.876114 webint-0.1.8/web/framework/letsencrypt.py
--rw-r--r--   0        0        0        0 2023-01-27 00:43:42.536109 webint-0.1.8/web/framework/newmath.py
--rw-r--r--   0        0        0    85473 2023-01-27 00:43:42.532109 webint-0.1.8/web/framework/passphrases.json
--rw-r--r--   0        0        0     1339 2023-01-27 00:43:42.536109 webint-0.1.8/web/framework/passphrases.py
--rw-r--r--   0        0        0     2840 2023-01-27 00:43:42.720111 webint-0.1.8/web/framework/static/1133.web.js
--rw-r--r--   0        0        0      387 2023-01-27 00:43:42.756112 webint-0.1.8/web/framework/static/1133.web.js.LICENSE.txt
--rw-r--r--   0        0        0     4935 2023-01-27 00:43:42.768112 webint-0.1.8/web/framework/static/1149.web.js
--rw-r--r--   0        0        0      648 2023-01-27 00:43:42.672111 webint-0.1.8/web/framework/static/1149.web.js.LICENSE.txt
--rw-r--r--   0        0        0    11823 2023-01-27 00:43:42.604110 webint-0.1.8/web/framework/static/1182.web.js
--rw-r--r--   0        0        0      387 2023-01-27 00:43:42.740112 webint-0.1.8/web/framework/static/1182.web.js.LICENSE.txt
--rw-r--r--   0        0        0    16087 2023-01-27 00:43:42.732112 webint-0.1.8/web/framework/static/1322.web.js
--rw-r--r--   0        0        0      387 2023-01-27 00:43:42.868113 webint-0.1.8/web/framework/static/1322.web.js.LICENSE.txt
--rw-r--r--   0        0        0     1850 2023-01-27 00:43:42.844113 webint-0.1.8/web/framework/static/195.web.js
--rw-r--r--   0        0        0      387 2023-01-27 00:43:42.596110 webint-0.1.8/web/framework/static/195.web.js.LICENSE.txt
--rw-r--r--   0        0        0     4183 2023-01-27 00:43:42.868113 webint-0.1.8/web/framework/static/2089.web.js
--rw-r--r--   0        0        0      387 2023-01-27 00:43:42.760112 webint-0.1.8/web/framework/static/2089.web.js.LICENSE.txt
--rw-r--r--   0        0        0     3594 2023-01-27 00:43:42.844113 webint-0.1.8/web/framework/static/2137.web.js
--rw-r--r--   0        0        0      387 2023-01-27 00:43:42.644111 webint-0.1.8/web/framework/static/2137.web.js.LICENSE.txt
--rw-r--r--   0        0        0    32199 2023-01-27 00:43:42.608110 webint-0.1.8/web/framework/static/2153.web.js
--rw-r--r--   0        0        0      387 2023-01-27 00:43:42.776112 webint-0.1.8/web/framework/static/2153.web.js.LICENSE.txt
--rw-r--r--   0        0        0     1124 2023-01-27 00:43:42.740112 webint-0.1.8/web/framework/static/2159.web.js
--rw-r--r--   0        0        0      387 2023-01-27 00:43:42.632110 webint-0.1.8/web/framework/static/2159.web.js.LICENSE.txt
--rw-r--r--   0        0        0     7626 2023-01-27 00:43:42.592110 webint-0.1.8/web/framework/static/2280.web.js
--rw-r--r--   0        0        0      387 2023-01-27 00:43:42.764112 webint-0.1.8/web/framework/static/2280.web.js.LICENSE.txt
--rw-r--r--   0        0        0     1706 2023-01-27 00:43:42.668111 webint-0.1.8/web/framework/static/2384.web.js
--rw-r--r--   0        0        0      387 2023-01-27 00:43:42.552109 webint-0.1.8/web/framework/static/2384.web.js.LICENSE.txt
--rw-r--r--   0        0        0     3096 2023-01-27 00:43:42.652111 webint-0.1.8/web/framework/static/2456.web.js
--rw-r--r--   0        0        0      387 2023-01-27 00:43:42.740112 webint-0.1.8/web/framework/static/2456.web.js.LICENSE.txt
--rw-r--r--   0        0        0    16962 2023-01-27 00:43:42.748112 webint-0.1.8/web/framework/static/2489.web.js
--rw-r--r--   0        0        0      387 2023-01-27 00:43:42.852113 webint-0.1.8/web/framework/static/2489.web.js.LICENSE.txt
--rw-r--r--   0        0        0     5469 2023-01-27 00:43:42.552109 webint-0.1.8/web/framework/static/249.web.js
--rw-r--r--   0        0        0      387 2023-01-27 00:43:42.596110 webint-0.1.8/web/framework/static/249.web.js.LICENSE.txt
--rw-r--r--   0        0        0     5021 2023-01-27 00:43:42.716112 webint-0.1.8/web/framework/static/2755.web.js
--rw-r--r--   0        0        0      387 2023-01-27 00:43:42.752112 webint-0.1.8/web/framework/static/2755.web.js.LICENSE.txt
--rw-r--r--   0        0        0     7879 2023-01-27 00:43:42.688111 webint-0.1.8/web/framework/static/2826.web.js
--rw-r--r--   0        0        0      387 2023-01-27 00:43:42.692111 webint-0.1.8/web/framework/static/2826.web.js.LICENSE.txt
--rw-r--r--   0        0        0     2402 2023-01-27 00:43:42.724112 webint-0.1.8/web/framework/static/2919.web.js
--rw-r--r--   0        0        0      387 2023-01-27 00:43:42.616110 webint-0.1.8/web/framework/static/2919.web.js.LICENSE.txt
--rw-r--r--   0        0        0     3292 2023-01-27 00:43:42.704111 webint-0.1.8/web/framework/static/3241.web.js
--rw-r--r--   0        0        0      387 2023-01-27 00:43:42.548109 webint-0.1.8/web/framework/static/3241.web.js.LICENSE.txt
--rw-r--r--   0        0        0     3579 2023-01-27 00:43:42.648111 webint-0.1.8/web/framework/static/3282.web.js
--rw-r--r--   0        0        0      387 2023-01-27 00:43:42.656111 webint-0.1.8/web/framework/static/3282.web.js.LICENSE.txt
--rw-r--r--   0        0        0     2208 2023-01-27 00:43:42.676111 webint-0.1.8/web/framework/static/3339.web.js
--rw-r--r--   0        0        0      387 2023-01-27 00:43:42.872114 webint-0.1.8/web/framework/static/3339.web.js.LICENSE.txt
--rw-r--r--   0        0        0     6763 2023-01-27 00:43:42.856113 webint-0.1.8/web/framework/static/3374.web.js
--rw-r--r--   0        0        0      387 2023-01-27 00:43:42.776112 webint-0.1.8/web/framework/static/3374.web.js.LICENSE.txt
--rw-r--r--   0        0        0     3600 2023-01-27 00:43:42.744112 webint-0.1.8/web/framework/static/3558.web.js
--rw-r--r--   0        0        0      387 2023-01-27 00:43:42.752112 webint-0.1.8/web/framework/static/3558.web.js.LICENSE.txt
--rw-r--r--   0        0        0     2680 2023-01-27 00:43:42.712111 webint-0.1.8/web/framework/static/3559.web.js
--rw-r--r--   0        0        0      387 2023-01-27 00:43:42.544109 webint-0.1.8/web/framework/static/3559.web.js.LICENSE.txt
--rw-r--r--   0        0        0     4536 2023-01-27 00:43:42.724112 webint-0.1.8/web/framework/static/3657.web.js
--rw-r--r--   0        0        0      387 2023-01-27 00:43:42.728112 webint-0.1.8/web/framework/static/3657.web.js.LICENSE.txt
--rw-r--r--   0        0        0     4935 2023-01-27 00:43:42.620110 webint-0.1.8/web/framework/static/3659.web.js
--rw-r--r--   0        0        0      387 2023-01-27 00:43:42.772112 webint-0.1.8/web/framework/static/3659.web.js.LICENSE.txt
--rw-r--r--   0        0        0    32750 2023-01-27 00:43:42.556110 webint-0.1.8/web/framework/static/3684.web.js
--rw-r--r--   0        0        0      387 2023-01-27 00:43:42.660111 webint-0.1.8/web/framework/static/3684.web.js.LICENSE.txt
--rw-r--r--   0        0        0     1789 2023-01-27 00:43:42.760112 webint-0.1.8/web/framework/static/3788.web.js
--rw-r--r--   0        0        0      387 2023-01-27 00:43:42.868113 webint-0.1.8/web/framework/static/3788.web.js.LICENSE.txt
--rw-r--r--   0        0        0     8050 2023-01-27 00:43:42.676111 webint-0.1.8/web/framework/static/3931.web.js
--rw-r--r--   0        0        0      387 2023-01-27 00:43:42.772112 webint-0.1.8/web/framework/static/3931.web.js.LICENSE.txt
--rw-r--r--   0        0        0     3922 2023-01-27 00:43:42.692111 webint-0.1.8/web/framework/static/3998.web.js
--rw-r--r--   0        0        0      387 2023-01-27 00:43:42.552109 webint-0.1.8/web/framework/static/3998.web.js.LICENSE.txt
--rw-r--r--   0        0        0     2423 2023-01-27 00:43:42.864113 webint-0.1.8/web/framework/static/429.web.js
--rw-r--r--   0        0        0      387 2023-01-27 00:43:42.712111 webint-0.1.8/web/framework/static/429.web.js.LICENSE.txt
--rw-r--r--   0        0        0      870 2023-01-27 00:43:42.600110 webint-0.1.8/web/framework/static/4463.web.js
--rw-r--r--   0        0        0      387 2023-01-27 00:43:42.624110 webint-0.1.8/web/framework/static/4463.web.js.LICENSE.txt
--rw-r--r--   0        0        0     2508 2023-01-27 00:43:42.684111 webint-0.1.8/web/framework/static/4552.web.js
--rw-r--r--   0        0        0      387 2023-01-27 00:43:42.632110 webint-0.1.8/web/framework/static/4552.web.js.LICENSE.txt
--rw-r--r--   0        0        0     1440 2023-01-27 00:43:42.668111 webint-0.1.8/web/framework/static/468.web.js
--rw-r--r--   0        0        0      387 2023-01-27 00:43:42.864113 webint-0.1.8/web/framework/static/468.web.js.LICENSE.txt
--rw-r--r--   0        0        0    14186 2023-01-27 00:43:42.740112 webint-0.1.8/web/framework/static/4776.web.js
--rw-r--r--   0        0        0      387 2023-01-27 00:43:42.716112 webint-0.1.8/web/framework/static/4776.web.js.LICENSE.txt
--rw-r--r--   0        0        0     6435 2023-01-27 00:43:42.636110 webint-0.1.8/web/framework/static/4932.web.js
--rw-r--r--   0        0        0      387 2023-01-27 00:43:42.724112 webint-0.1.8/web/framework/static/4932.web.js.LICENSE.txt
--rw-r--r--   0        0        0     3947 2023-01-27 00:43:42.560109 webint-0.1.8/web/framework/static/501.web.js
--rw-r--r--   0        0        0      387 2023-01-27 00:43:42.644111 webint-0.1.8/web/framework/static/501.web.js.LICENSE.txt
--rw-r--r--   0        0        0    18620 2023-01-27 00:43:42.636110 webint-0.1.8/web/framework/static/5021.web.js
--rw-r--r--   0        0        0      387 2023-01-27 00:43:42.552109 webint-0.1.8/web/framework/static/5021.web.js.LICENSE.txt
--rw-r--r--   0        0        0     8278 2023-01-27 00:43:42.624110 webint-0.1.8/web/framework/static/5289.web.js
--rw-r--r--   0        0        0      387 2023-01-27 00:43:42.848113 webint-0.1.8/web/framework/static/5289.web.js.LICENSE.txt
--rw-r--r--   0        0        0     7172 2023-01-27 00:43:42.608110 webint-0.1.8/web/framework/static/5337.web.js
--rw-r--r--   0        0        0      387 2023-01-27 00:43:42.612110 webint-0.1.8/web/framework/static/5337.web.js.LICENSE.txt
--rw-r--r--   0        0        0     8772 2023-01-27 00:43:42.644111 webint-0.1.8/web/framework/static/5341.web.js
--rw-r--r--   0        0        0      387 2023-01-27 00:43:42.740112 webint-0.1.8/web/framework/static/5341.web.js.LICENSE.txt
--rw-r--r--   0        0        0     3983 2023-01-27 00:43:42.592110 webint-0.1.8/web/framework/static/5466.web.js
--rw-r--r--   0        0        0      387 2023-01-27 00:43:42.708111 webint-0.1.8/web/framework/static/5466.web.js.LICENSE.txt
--rw-r--r--   0        0        0     3829 2023-01-27 00:43:42.640111 webint-0.1.8/web/framework/static/5490.web.js
--rw-r--r--   0        0        0      387 2023-01-27 00:43:42.868113 webint-0.1.8/web/framework/static/5490.web.js.LICENSE.txt
--rw-r--r--   0        0        0     5365 2023-01-27 00:43:42.672111 webint-0.1.8/web/framework/static/5502.web.js
--rw-r--r--   0        0        0      387 2023-01-27 00:43:42.704111 webint-0.1.8/web/framework/static/5502.web.js.LICENSE.txt
--rw-r--r--   0        0        0     6001 2023-01-27 00:43:42.860113 webint-0.1.8/web/framework/static/5528.web.js
--rw-r--r--   0        0        0      387 2023-01-27 00:43:42.544109 webint-0.1.8/web/framework/static/5528.web.js.LICENSE.txt
--rw-r--r--   0        0        0     3611 2023-01-27 00:43:42.732112 webint-0.1.8/web/framework/static/570.web.js
--rw-r--r--   0        0        0      387 2023-01-27 00:43:42.684111 webint-0.1.8/web/framework/static/570.web.js.LICENSE.txt
--rw-r--r--   0        0        0     4851 2023-01-27 00:43:42.552109 webint-0.1.8/web/framework/static/5892.web.js
--rw-r--r--   0        0        0      387 2023-01-27 00:43:42.860113 webint-0.1.8/web/framework/static/5892.web.js.LICENSE.txt
--rw-r--r--   0        0        0     7409 2023-01-27 00:43:42.752112 webint-0.1.8/web/framework/static/5986.web.js
--rw-r--r--   0        0        0      387 2023-01-27 00:43:42.704111 webint-0.1.8/web/framework/static/5986.web.js.LICENSE.txt
--rw-r--r--   0        0        0     1832 2023-01-27 00:43:42.748112 webint-0.1.8/web/framework/static/6259.web.js
--rw-r--r--   0        0        0      387 2023-01-27 00:43:42.560109 webint-0.1.8/web/framework/static/6259.web.js.LICENSE.txt
--rw-r--r--   0        0        0     3154 2023-01-27 00:43:42.704111 webint-0.1.8/web/framework/static/6389.web.js
--rw-r--r--   0        0        0      387 2023-01-27 00:43:42.656111 webint-0.1.8/web/framework/static/6389.web.js.LICENSE.txt
--rw-r--r--   0        0        0     3462 2023-01-27 00:43:42.536109 webint-0.1.8/web/framework/static/6422.web.js
--rw-r--r--   0        0        0      387 2023-01-27 00:43:42.868113 webint-0.1.8/web/framework/static/6422.web.js.LICENSE.txt
--rw-r--r--   0        0        0     9666 2023-01-27 00:43:42.616110 webint-0.1.8/web/framework/static/6425.web.js
--rw-r--r--   0        0        0      387 2023-01-27 00:43:42.780112 webint-0.1.8/web/framework/static/6425.web.js.LICENSE.txt
--rw-r--r--   0        0        0     1892 2023-01-27 00:43:42.852113 webint-0.1.8/web/framework/static/6548.web.js
--rw-r--r--   0        0        0      387 2023-01-27 00:43:42.556110 webint-0.1.8/web/framework/static/6548.web.js.LICENSE.txt
--rw-r--r--   0        0        0     1868 2023-01-27 00:43:42.856113 webint-0.1.8/web/framework/static/6681.web.js
--rw-r--r--   0        0        0      387 2023-01-27 00:43:42.660111 webint-0.1.8/web/framework/static/6681.web.js.LICENSE.txt
--rw-r--r--   0        0        0     4546 2023-01-27 00:43:42.736112 webint-0.1.8/web/framework/static/7050.web.js
--rw-r--r--   0        0        0      387 2023-01-27 00:43:42.872114 webint-0.1.8/web/framework/static/7050.web.js.LICENSE.txt
--rw-r--r--   0        0        0     5376 2023-01-27 00:43:42.548109 webint-0.1.8/web/framework/static/7138.web.js
--rw-r--r--   0        0        0      387 2023-01-27 00:43:42.656111 webint-0.1.8/web/framework/static/7138.web.js.LICENSE.txt
--rw-r--r--   0        0        0     3971 2023-01-27 00:43:42.756112 webint-0.1.8/web/framework/static/7201.web.js
--rw-r--r--   0        0        0      387 2023-01-27 00:43:42.616110 webint-0.1.8/web/framework/static/7201.web.js.LICENSE.txt
--rw-r--r--   0        0        0     2958 2023-01-27 00:43:42.764112 webint-0.1.8/web/framework/static/7318.web.js
--rw-r--r--   0        0        0      387 2023-01-27 00:43:42.648111 webint-0.1.8/web/framework/static/7318.web.js.LICENSE.txt
--rw-r--r--   0        0        0     7341 2023-01-27 00:43:42.728112 webint-0.1.8/web/framework/static/7441.web.js
--rw-r--r--   0        0        0      387 2023-01-27 00:43:42.632110 webint-0.1.8/web/framework/static/7441.web.js.LICENSE.txt
--rw-r--r--   0        0        0    38093 2023-01-27 00:43:42.680111 webint-0.1.8/web/framework/static/7660.web.js
--rw-r--r--   0        0        0      387 2023-01-27 00:43:42.628110 webint-0.1.8/web/framework/static/7660.web.js.LICENSE.txt
--rw-r--r--   0        0        0     2602 2023-01-27 00:43:42.708111 webint-0.1.8/web/framework/static/7730.web.js
--rw-r--r--   0        0        0      387 2023-01-27 00:43:42.544109 webint-0.1.8/web/framework/static/7730.web.js.LICENSE.txt
--rw-r--r--   0        0        0     8528 2023-01-27 00:43:42.604110 webint-0.1.8/web/framework/static/7864.web.js
--rw-r--r--   0        0        0      387 2023-01-27 00:43:42.608110 webint-0.1.8/web/framework/static/7864.web.js.LICENSE.txt
--rw-r--r--   0        0        0     2785 2023-01-27 00:43:42.544109 webint-0.1.8/web/framework/static/788.web.js
--rw-r--r--   0        0        0      387 2023-01-27 00:43:42.848113 webint-0.1.8/web/framework/static/788.web.js.LICENSE.txt
--rw-r--r--   0        0        0     3928 2023-01-27 00:43:42.756112 webint-0.1.8/web/framework/static/8059.web.js
--rw-r--r--   0        0        0      387 2023-01-27 00:43:42.604110 webint-0.1.8/web/framework/static/8059.web.js.LICENSE.txt
--rw-r--r--   0        0        0     3018 2023-01-27 00:43:42.680111 webint-0.1.8/web/framework/static/8106.web.js
--rw-r--r--   0        0        0      387 2023-01-27 00:43:42.756112 webint-0.1.8/web/framework/static/8106.web.js.LICENSE.txt
--rw-r--r--   0        0        0     6214 2023-01-27 00:43:42.752112 webint-0.1.8/web/framework/static/8262.web.js
--rw-r--r--   0        0        0      387 2023-01-27 00:43:42.856113 webint-0.1.8/web/framework/static/8262.web.js.LICENSE.txt
--rw-r--r--   0        0        0     2283 2023-01-27 00:43:42.760112 webint-0.1.8/web/framework/static/8356.web.js
--rw-r--r--   0        0        0      387 2023-01-27 00:43:42.604110 webint-0.1.8/web/framework/static/8356.web.js.LICENSE.txt
--rw-r--r--   0        0        0     2575 2023-01-27 00:43:42.772112 webint-0.1.8/web/framework/static/8416.web.js
--rw-r--r--   0        0        0      387 2023-01-27 00:43:42.708111 webint-0.1.8/web/framework/static/8416.web.js.LICENSE.txt
--rw-r--r--   0        0        0     2023 2023-01-27 00:43:42.688111 webint-0.1.8/web/framework/static/8512.web.js
--rw-r--r--   0        0        0      387 2023-01-27 00:43:42.688111 webint-0.1.8/web/framework/static/8512.web.js.LICENSE.txt
--rw-r--r--   0        0        0     3244 2023-01-27 00:43:42.652111 webint-0.1.8/web/framework/static/8562.web.js
--rw-r--r--   0        0        0      387 2023-01-27 00:43:42.860113 webint-0.1.8/web/framework/static/8562.web.js.LICENSE.txt
--rw-r--r--   0        0        0     5814 2023-01-27 00:43:42.540109 webint-0.1.8/web/framework/static/8670.web.js
--rw-r--r--   0        0        0      387 2023-01-27 00:43:42.588110 webint-0.1.8/web/framework/static/8670.web.js.LICENSE.txt
--rw-r--r--   0        0        0     4273 2023-01-27 00:43:42.780112 webint-0.1.8/web/framework/static/8842.web.js
--rw-r--r--   0        0        0      387 2023-01-27 00:43:42.676111 webint-0.1.8/web/framework/static/8842.web.js.LICENSE.txt
--rw-r--r--   0        0        0     9780 2023-01-27 00:43:42.772112 webint-0.1.8/web/framework/static/888.web.js
--rw-r--r--   0        0        0      387 2023-01-27 00:43:42.672111 webint-0.1.8/web/framework/static/888.web.js.LICENSE.txt
--rw-r--r--   0        0        0     3411 2023-01-27 00:43:42.736112 webint-0.1.8/web/framework/static/8903.web.js
--rw-r--r--   0        0        0      387 2023-01-27 00:43:42.844113 webint-0.1.8/web/framework/static/8903.web.js.LICENSE.txt
--rw-r--r--   0        0        0    13426 2023-01-27 00:43:42.540109 webint-0.1.8/web/framework/static/9338.web.js
--rw-r--r--   0        0        0      387 2023-01-27 00:43:42.716112 webint-0.1.8/web/framework/static/9338.web.js.LICENSE.txt
--rw-r--r--   0        0        0    11276 2023-01-27 00:43:42.600110 webint-0.1.8/web/framework/static/938.web.js
--rw-r--r--   0        0        0      387 2023-01-27 00:43:42.848113 webint-0.1.8/web/framework/static/938.web.js.LICENSE.txt
--rw-r--r--   0        0        0     9067 2023-01-27 00:43:42.720111 webint-0.1.8/web/framework/static/9407.web.js
--rw-r--r--   0        0        0      387 2023-01-27 00:43:42.548109 webint-0.1.8/web/framework/static/9407.web.js.LICENSE.txt
--rw-r--r--   0        0        0     3613 2023-01-27 00:43:42.592110 webint-0.1.8/web/framework/static/9502.web.js
--rw-r--r--   0        0        0      387 2023-01-27 00:43:42.728112 webint-0.1.8/web/framework/static/9502.web.js.LICENSE.txt
--rw-r--r--   0        0        0    10318 2023-01-27 00:43:42.656111 webint-0.1.8/web/framework/static/959.web.js
--rw-r--r--   0        0        0      387 2023-01-27 00:43:42.588110 webint-0.1.8/web/framework/static/959.web.js.LICENSE.txt
--rw-r--r--   0        0        0     2458 2023-01-27 00:43:42.620110 webint-0.1.8/web/framework/static/966.web.js
--rw-r--r--   0        0        0      387 2023-01-27 00:43:42.768112 webint-0.1.8/web/framework/static/966.web.js.LICENSE.txt
--rw-r--r--   0        0        0     3005 2023-01-27 00:43:42.708111 webint-0.1.8/web/framework/static/9721.web.js
--rw-r--r--   0        0        0      387 2023-01-27 00:43:42.592110 webint-0.1.8/web/framework/static/9721.web.js.LICENSE.txt
--rw-r--r--   0        0        0     2146 2023-01-27 00:43:42.688111 webint-0.1.8/web/framework/static/9762.web.js
--rw-r--r--   0        0        0      387 2023-01-27 00:43:42.748112 webint-0.1.8/web/framework/static/9762.web.js.LICENSE.txt
--rw-r--r--   0        0        0    21621 2023-01-27 00:43:42.608110 webint-0.1.8/web/framework/static/9822.web.js
--rw-r--r--   0        0        0    72504 2023-01-27 00:43:42.672111 webint-0.1.8/web/framework/static/b797181c93b3755f4fa1.ttf
--rw-r--r--   0        0        0  4897844 2023-01-27 00:43:42.584110 webint-0.1.8/web/framework/static/css.worker.js
--rw-r--r--   0        0        0      387 2023-01-27 00:43:42.596110 webint-0.1.8/web/framework/static/css.worker.js.LICENSE.txt
--rw-r--r--   0        0        0  1637641 2023-01-27 00:43:42.664111 webint-0.1.8/web/framework/static/editor.worker.js
--rw-r--r--   0        0        0  3399495 2023-01-27 00:43:42.568110 webint-0.1.8/web/framework/static/html.worker.js
--rw-r--r--   0        0        0      387 2023-01-27 00:43:42.620110 webint-0.1.8/web/framework/static/html.worker.js.LICENSE.txt
--rw-r--r--   0        0        0  2332252 2023-01-27 00:43:42.700111 webint-0.1.8/web/framework/static/json.worker.js
--rw-r--r--   0        0        0      387 2023-01-27 00:43:42.724112 webint-0.1.8/web/framework/static/json.worker.js.LICENSE.txt
--rw-r--r--   0        0        0      569 2023-01-27 00:43:42.540109 webint-0.1.8/web/framework/static/measure.png
--rw-r--r--   0        0        0    19132 2023-01-27 00:43:42.708111 webint-0.1.8/web/framework/static/node_modules_monaco-editor_esm_vs_basic-languages_apex_apex_js.web.js
--rw-r--r--   0        0        0     6058 2023-01-27 00:43:42.596110 webint-0.1.8/web/framework/static/node_modules_monaco-editor_esm_vs_basic-languages_azcli_azcli_js.web.js
--rw-r--r--   0        0        0     9006 2023-01-27 00:43:42.588110 webint-0.1.8/web/framework/static/node_modules_monaco-editor_esm_vs_basic-languages_bat_bat_js.web.js
--rw-r--r--   0        0        0    12376 2023-01-27 00:43:42.600110 webint-0.1.8/web/framework/static/node_modules_monaco-editor_esm_vs_basic-languages_bicep_bicep_js.web.js
--rw-r--r--   0        0        0    11717 2023-01-27 00:43:42.684111 webint-0.1.8/web/framework/static/node_modules_monaco-editor_esm_vs_basic-languages_cameligo_cameligo_js.web.js
--rw-r--r--   0        0        0    17396 2023-01-27 00:43:42.684111 webint-0.1.8/web/framework/static/node_modules_monaco-editor_esm_vs_basic-languages_coffee_coffee_js.web.js
--rw-r--r--   0        0        0    24827 2023-01-27 00:43:42.592110 webint-0.1.8/web/framework/static/node_modules_monaco-editor_esm_vs_basic-languages_cpp_cpp_js.web.js
--rw-r--r--   0        0        0    21742 2023-01-27 00:43:42.864113 webint-0.1.8/web/framework/static/node_modules_monaco-editor_esm_vs_basic-languages_csharp_csharp_js.web.js
--rw-r--r--   0        0        0     6491 2023-01-27 00:43:42.712111 webint-0.1.8/web/framework/static/node_modules_monaco-editor_esm_vs_basic-languages_csp_csp_js.web.js
--rw-r--r--   0        0        0    19159 2023-01-27 00:43:42.668111 webint-0.1.8/web/framework/static/node_modules_monaco-editor_esm_vs_basic-languages_css_css_js.web.js
--rw-r--r--   0        0        0    16682 2023-01-27 00:43:42.732112 webint-0.1.8/web/framework/static/node_modules_monaco-editor_esm_vs_basic-languages_cypher_cypher_js.web.js
--rw-r--r--   0        0        0    19293 2023-01-27 00:43:42.748112 webint-0.1.8/web/framework/static/node_modules_monaco-editor_esm_vs_basic-languages_dart_dart_js.web.js
--rw-r--r--   0        0        0    10624 2023-01-27 00:43:42.732112 webint-0.1.8/web/framework/static/node_modules_monaco-editor_esm_vs_basic-languages_dockerfile_dockerfile_js.web.js
--rw-r--r--   0        0        0    25376 2023-01-27 00:43:42.768112 webint-0.1.8/web/framework/static/node_modules_monaco-editor_esm_vs_basic-languages_ecl_ecl_js.web.js
--rw-r--r--   0        0        0     9895 2023-01-27 00:43:42.764112 webint-0.1.8/web/framework/static/node_modules_monaco-editor_esm_vs_basic-languages_flow9_flow9_js.web.js
--rw-r--r--   0        0        0    14428 2023-01-27 00:43:42.780112 webint-0.1.8/web/framework/static/node_modules_monaco-editor_esm_vs_basic-languages_fsharp_fsharp_js.web.js
--rw-r--r--   0        0        0    13553 2023-01-27 00:43:42.672111 webint-0.1.8/web/framework/static/node_modules_monaco-editor_esm_vs_basic-languages_go_go_js.web.js
--rw-r--r--   0        0        0    11277 2023-01-27 00:43:42.844113 webint-0.1.8/web/framework/static/node_modules_monaco-editor_esm_vs_basic-languages_graphql_graphql_js.web.js
--rw-r--r--   0        0        0    15438 2023-01-27 00:43:42.692111 webint-0.1.8/web/framework/static/node_modules_monaco-editor_esm_vs_basic-languages_hcl_hcl_js.web.js
--rw-r--r--   0        0        0    23800 2023-01-27 00:43:42.616110 webint-0.1.8/web/framework/static/node_modules_monaco-editor_esm_vs_basic-languages_html_html_js.web.js
--rw-r--r--   0        0        0     6406 2023-01-27 00:43:42.628110 webint-0.1.8/web/framework/static/node_modules_monaco-editor_esm_vs_basic-languages_ini_ini_js.web.js
--rw-r--r--   0        0        0    15210 2023-01-27 00:43:42.692111 webint-0.1.8/web/framework/static/node_modules_monaco-editor_esm_vs_basic-languages_java_java_js.web.js
--rw-r--r--   0        0        0    16332 2023-01-27 00:43:42.776112 webint-0.1.8/web/framework/static/node_modules_monaco-editor_esm_vs_basic-languages_kotlin_kotlin_js.web.js
--rw-r--r--   0        0        0    16679 2023-01-27 00:43:42.784112 webint-0.1.8/web/framework/static/node_modules_monaco-editor_esm_vs_basic-languages_less_less_js.web.js
--rw-r--r--   0        0        0    12072 2023-01-27 00:43:42.612110 webint-0.1.8/web/framework/static/node_modules_monaco-editor_esm_vs_basic-languages_lexon_lexon_js.web.js
--rw-r--r--   0        0        0    19465 2023-01-27 00:43:42.772112 webint-0.1.8/web/framework/static/node_modules_monaco-editor_esm_vs_basic-languages_liquid_liquid_js.web.js
--rw-r--r--   0        0        0    11332 2023-01-27 00:43:42.628110 webint-0.1.8/web/framework/static/node_modules_monaco-editor_esm_vs_basic-languages_lua_lua_js.web.js
--rw-r--r--   0        0        0    13995 2023-01-27 00:43:42.760112 webint-0.1.8/web/framework/static/node_modules_monaco-editor_esm_vs_basic-languages_m3_m3_js.web.js
--rw-r--r--   0        0        0    17583 2023-01-27 00:43:42.648111 webint-0.1.8/web/framework/static/node_modules_monaco-editor_esm_vs_basic-languages_markdown_markdown_js.web.js
--rw-r--r--   0        0        0    13421 2023-01-27 00:43:42.780112 webint-0.1.8/web/framework/static/node_modules_monaco-editor_esm_vs_basic-languages_mips_mips_js.web.js
--rw-r--r--   0        0        0    22656 2023-01-27 00:43:42.736112 webint-0.1.8/web/framework/static/node_modules_monaco-editor_esm_vs_basic-languages_msdax_msdax_js.web.js
--rw-r--r--   0        0        0    12524 2023-01-27 00:43:42.640111 webint-0.1.8/web/framework/static/node_modules_monaco-editor_esm_vs_basic-languages_objective-c_objective-c_js.web.js
--rw-r--r--   0        0        0    15300 2023-01-27 00:43:42.656111 webint-0.1.8/web/framework/static/node_modules_monaco-editor_esm_vs_basic-languages_pascal_pascal_js.web.js
--rw-r--r--   0        0        0    10923 2023-01-27 00:43:42.660111 webint-0.1.8/web/framework/static/node_modules_monaco-editor_esm_vs_basic-languages_pascaligo_pascaligo_js.web.js
--rw-r--r--   0        0        0     9896 2023-01-27 00:43:42.640111 webint-0.1.8/web/framework/static/node_modules_monaco-editor_esm_vs_basic-languages_pla_pla_js.web.js
--rw-r--r--   0        0        0    17017 2023-01-27 00:43:42.752112 webint-0.1.8/web/framework/static/node_modules_monaco-editor_esm_vs_basic-languages_powershell_powershell_js.web.js
--rw-r--r--   0        0        0    25438 2023-01-27 00:43:42.644111 webint-0.1.8/web/framework/static/node_modules_monaco-editor_esm_vs_basic-languages_pug_pug_js.web.js
--rw-r--r--   0        0        0    18459 2023-01-27 00:43:42.556110 webint-0.1.8/web/framework/static/node_modules_monaco-editor_esm_vs_basic-languages_python_python_js.web.js
--rw-r--r--   0        0        0    15716 2023-01-27 00:43:42.716112 webint-0.1.8/web/framework/static/node_modules_monaco-editor_esm_vs_basic-languages_qsharp_qsharp_js.web.js
--rw-r--r--   0        0        0    15762 2023-01-27 00:43:42.652111 webint-0.1.8/web/framework/static/node_modules_monaco-editor_esm_vs_basic-languages_r_r_js.web.js
--rw-r--r--   0        0        0    17644 2023-01-27 00:43:42.636110 webint-0.1.8/web/framework/static/node_modules_monaco-editor_esm_vs_basic-languages_redis_redis_js.web.js
--rw-r--r--   0        0        0    16271 2023-01-27 00:43:42.676111 webint-0.1.8/web/framework/static/node_modules_monaco-editor_esm_vs_basic-languages_restructuredtext_restructuredtext_js.web.js
--rw-r--r--   0        0        0    20405 2023-01-27 00:43:42.612110 webint-0.1.8/web/framework/static/node_modules_monaco-editor_esm_vs_basic-languages_rust_rust_js.web.js
--rw-r--r--   0        0        0     9291 2023-01-27 00:43:42.624110 webint-0.1.8/web/framework/static/node_modules_monaco-editor_esm_vs_basic-languages_sb_sb_js.web.js
--rw-r--r--   0        0        0     9201 2023-01-27 00:43:42.764112 webint-0.1.8/web/framework/static/node_modules_monaco-editor_esm_vs_basic-languages_scheme_scheme_js.web.js
--rw-r--r--   0        0        0    26294 2023-01-27 00:43:42.864113 webint-0.1.8/web/framework/static/node_modules_monaco-editor_esm_vs_basic-languages_scss_scss_js.web.js
--rw-r--r--   0        0        0    15071 2023-01-27 00:43:42.776112 webint-0.1.8/web/framework/static/node_modules_monaco-editor_esm_vs_basic-languages_shell_shell_js.web.js
--rw-r--r--   0        0        0    13358 2023-01-27 00:43:42.716112 webint-0.1.8/web/framework/static/node_modules_monaco-editor_esm_vs_basic-languages_sophia_sophia_js.web.js
--rw-r--r--   0        0        0    12795 2023-01-27 00:43:42.616110 webint-0.1.8/web/framework/static/node_modules_monaco-editor_esm_vs_basic-languages_sparql_sparql_js.web.js
--rw-r--r--   0        0        0    22397 2023-01-27 00:43:42.636110 webint-0.1.8/web/framework/static/node_modules_monaco-editor_esm_vs_basic-languages_swift_swift_js.web.js
--rw-r--r--   0        0        0    16853 2023-01-27 00:43:42.652111 webint-0.1.8/web/framework/static/node_modules_monaco-editor_esm_vs_basic-languages_tcl_tcl_js.web.js
--rw-r--r--   0        0        0    25948 2023-01-27 00:43:42.640111 webint-0.1.8/web/framework/static/node_modules_monaco-editor_esm_vs_basic-languages_twig_twig_js.web.js
--rw-r--r--   0        0        0    25135 2023-01-27 00:43:42.848113 webint-0.1.8/web/framework/static/node_modules_monaco-editor_esm_vs_basic-languages_typescript_typescript_js.web.js
--rw-r--r--   0        0        0    25134 2023-01-27 00:43:42.588110 webint-0.1.8/web/framework/static/node_modules_monaco-editor_esm_vs_basic-languages_vb_vb_js.web.js
--rw-r--r--   0        0        0    12067 2023-01-27 00:43:42.556110 webint-0.1.8/web/framework/static/node_modules_monaco-editor_esm_vs_basic-languages_xml_xml_js.web.js
--rw-r--r--   0        0        0    18657 2023-01-27 00:43:42.860113 webint-0.1.8/web/framework/static/node_modules_monaco-editor_esm_vs_basic-languages_yaml_yaml_js.web.js
--rw-r--r--   0        0        0     9872 2023-01-27 00:43:42.600110 webint-0.1.8/web/framework/static/solarized-site.css
--rw-r--r--   0        0        0     4743 2023-01-27 00:43:42.872114 webint-0.1.8/web/framework/static/solarized.css
--rw-r--r--   0        0        0 22565048 2023-01-27 00:43:42.836113 webint-0.1.8/web/framework/static/ts.worker.js
--rw-r--r--   0        0        0     1199 2023-01-27 00:43:42.728112 webint-0.1.8/web/framework/static/ts.worker.js.LICENSE.txt
--rw-r--r--   0        0        0    64818 2023-01-27 00:43:42.680111 webint-0.1.8/web/framework/static/vendors-node_modules_monaco-editor_esm_vs_basic-languages_abap_abap_js.web.js
--rw-r--r--   0        0        0    42160 2023-01-27 00:43:42.852113 webint-0.1.8/web/framework/static/vendors-node_modules_monaco-editor_esm_vs_basic-languages_clojure_clojure_js.web.js
--rw-r--r--   0        0        0    40113 2023-01-27 00:43:42.680111 webint-0.1.8/web/framework/static/vendors-node_modules_monaco-editor_esm_vs_basic-languages_elixir_elixir_js.web.js
--rw-r--r--   0        0        0    71501 2023-01-27 00:43:42.736112 webint-0.1.8/web/framework/static/vendors-node_modules_monaco-editor_esm_vs_basic-languages_freemarker2_freemarker2_js.web.js
--rw-r--r--   0        0        0    31775 2023-01-27 00:43:42.640111 webint-0.1.8/web/framework/static/vendors-node_modules_monaco-editor_esm_vs_basic-languages_handlebars_handlebars_js.web.js
--rw-r--r--   0        0        0    31412 2023-01-27 00:43:42.856113 webint-0.1.8/web/framework/static/vendors-node_modules_monaco-editor_esm_vs_basic-languages_javascript_javascript_js.web.js
--rw-r--r--   0        0        0    32008 2023-01-27 00:43:42.848113 webint-0.1.8/web/framework/static/vendors-node_modules_monaco-editor_esm_vs_basic-languages_julia_julia_js.web.js
--rw-r--r--   0        0        0    48644 2023-01-27 00:43:42.768112 webint-0.1.8/web/framework/static/vendors-node_modules_monaco-editor_esm_vs_basic-languages_mysql_mysql_js.web.js
--rw-r--r--   0        0        0    37499 2023-01-27 00:43:42.852113 webint-0.1.8/web/framework/static/vendors-node_modules_monaco-editor_esm_vs_basic-languages_perl_perl_js.web.js
--rw-r--r--   0        0        0    52967 2023-01-27 00:43:42.688111 webint-0.1.8/web/framework/static/vendors-node_modules_monaco-editor_esm_vs_basic-languages_pgsql_pgsql_js.web.js
--rw-r--r--   0        0        0    34711 2023-01-27 00:43:42.712111 webint-0.1.8/web/framework/static/vendors-node_modules_monaco-editor_esm_vs_basic-languages_php_php_js.web.js
--rw-r--r--   0        0        0    36168 2023-01-27 00:43:42.548109 webint-0.1.8/web/framework/static/vendors-node_modules_monaco-editor_esm_vs_basic-languages_postiats_postiats_js.web.js
--rw-r--r--   0        0        0    62249 2023-01-27 00:43:42.632110 webint-0.1.8/web/framework/static/vendors-node_modules_monaco-editor_esm_vs_basic-languages_powerquery_powerquery_js.web.js
--rw-r--r--   0        0        0    38247 2023-01-27 00:43:42.860113 webint-0.1.8/web/framework/static/vendors-node_modules_monaco-editor_esm_vs_basic-languages_protobuf_protobuf_js.web.js
--rw-r--r--   0        0        0    39348 2023-01-27 00:43:42.764112 webint-0.1.8/web/framework/static/vendors-node_modules_monaco-editor_esm_vs_basic-languages_razor_razor_js.web.js
--rw-r--r--   0        0        0    48458 2023-01-27 00:43:42.720111 webint-0.1.8/web/framework/static/vendors-node_modules_monaco-editor_esm_vs_basic-languages_redshift_redshift_js.web.js
--rw-r--r--   0        0        0    36815 2023-01-27 00:43:42.620110 webint-0.1.8/web/framework/static/vendors-node_modules_monaco-editor_esm_vs_basic-languages_ruby_ruby_js.web.js
--rw-r--r--   0        0        0    30240 2023-01-27 00:43:42.744112 webint-0.1.8/web/framework/static/vendors-node_modules_monaco-editor_esm_vs_basic-languages_scala_scala_js.web.js
--rw-r--r--   0        0        0    76292 2023-01-27 00:43:42.604110 webint-0.1.8/web/framework/static/vendors-node_modules_monaco-editor_esm_vs_basic-languages_solidity_solidity_js.web.js
--rw-r--r--   0        0        0    45550 2023-01-27 00:43:42.596110 webint-0.1.8/web/framework/static/vendors-node_modules_monaco-editor_esm_vs_basic-languages_sql_sql_js.web.js
--rw-r--r--   0        0        0    31355 2023-01-27 00:43:42.540109 webint-0.1.8/web/framework/static/vendors-node_modules_monaco-editor_esm_vs_basic-languages_st_st_js.web.js
--rw-r--r--   0        0        0    34466 2023-01-27 00:43:42.612110 webint-0.1.8/web/framework/static/vendors-node_modules_monaco-editor_esm_vs_basic-languages_systemverilog_systemverilog_js.web.js
--rw-r--r--   0        0        0   182429 2023-01-27 00:43:42.724112 webint-0.1.8/web/framework/static/vendors-node_modules_monaco-editor_esm_vs_language_css_cssMode_js.web.js
--rw-r--r--   0        0        0   185207 2023-01-27 00:43:42.648111 webint-0.1.8/web/framework/static/vendors-node_modules_monaco-editor_esm_vs_language_html_htmlMode_js.web.js
--rw-r--r--   0        0        0   222617 2023-01-27 00:43:42.744112 webint-0.1.8/web/framework/static/vendors-node_modules_monaco-editor_esm_vs_language_json_jsonMode_js.web.js
--rw-r--r--   0        0        0   106750 2023-01-27 00:43:42.628110 webint-0.1.8/web/framework/static/vendors-node_modules_monaco-editor_esm_vs_language_typescript_tsMode_js.web.js
--rw-r--r--   0        0        0      853 2023-01-27 00:43:42.628110 webint-0.1.8/web/framework/static/web.css
--rw-r--r--   0        0        0    65758 2023-02-14 18:36:48.533111 webint-0.1.8/web/framework/static/web.js
--rw-r--r--   0        0        0      576 2023-01-27 00:43:42.784112 webint-0.1.8/web/framework/static/web.js.LICENSE.txt
--rw-r--r--   0        0        0      441 2023-01-27 00:43:42.884114 webint-0.1.8/web/framework/templates/__init__.py
--rw-r--r--   0        0        0     2123 2023-01-27 00:43:42.880113 webint-0.1.8/web/framework/templates/nginx.conf
--rw-r--r--   0        0        0     1012 2023-01-27 00:43:42.888114 webint-0.1.8/web/framework/templates/nginx_host.conf
--rw-r--r--   0        0        0      988 2023-01-27 00:43:42.884114 webint-0.1.8/web/framework/templates/nginx_host_body.conf
--rw-r--r--   0        0        0      155 2023-01-27 00:43:42.884114 webint-0.1.8/web/framework/templates/nginx_tor_host.conf
--rw-r--r--   0        0        0      305 2023-01-27 00:43:42.884114 webint-0.1.8/web/framework/templates/redis.conf
--rw-r--r--   0        0        0     1141 2023-01-27 00:43:42.880113 webint-0.1.8/web/framework/templates/supervisor.conf
--rw-r--r--   0        0        0     4679 2023-01-27 00:43:42.888114 webint-0.1.8/web/framework/templates/traceback.html
--rw-r--r--   0        0        0     7283 2023-01-27 00:43:42.536109 webint-0.1.8/web/framework/util.py
--rw-r--r--   0        0        0     4136 2023-01-27 00:43:42.508109 webint-0.1.8/web/headers/__init__.py
--rw-r--r--   0        0        0     2343 2023-01-27 00:43:42.512109 webint-0.1.8/web/headers/entity.py
--rw-r--r--   0        0        0      581 2023-01-27 00:43:42.512109 webint-0.1.8/web/headers/general.py
--rw-r--r--   0        0        0     8623 2023-01-27 00:43:42.508109 webint-0.1.8/web/headers/request.py
--rw-r--r--   0        0        0     1150 2023-01-27 00:43:42.512109 webint-0.1.8/web/headers/response.py
--rw-r--r--   0        0        0      630 2023-01-27 00:43:42.508109 webint-0.1.8/web/headers/util.py
--rw-r--r--   0        0        0    17999 2023-02-18 21:18:16.540773 webint-0.1.8/web/host/__init__.py
--rw-r--r--   0        0        0     4474 2023-02-15 02:18:36.929705 webint-0.1.8/web/host/admin/__init__.py
--rw-r--r--   0        0        0       37 2023-02-15 02:09:57.822778 webint-0.1.8/web/host/admin/templates/__init__.py
--rw-r--r--   0        0        0      403 2023-02-15 19:17:41.914551 webint-0.1.8/web/host/admin/templates/application.html
--rw-r--r--   0        0        0      437 2023-02-15 19:20:01.696109 webint-0.1.8/web/host/admin/templates/choose_domain.html
--rw-r--r--   0        0        0     2394 2023-02-15 20:44:26.037755 webint-0.1.8/web/host/admin/templates/domains.html
--rw-r--r--   0        0        0      377 2023-02-15 02:17:09.944532 webint-0.1.8/web/host/admin/templates/index.html
--rw-r--r--   0        0        0      845 2023-02-15 02:23:12.153431 webint-0.1.8/web/host/admin/templates/template.html
--rw-r--r--   0        0        0     7478 2023-02-12 03:12:55.380982 webint-0.1.8/web/host/providers.py
--rw-r--r--   0        0        0        0 2023-01-27 00:43:42.504109 webint-0.1.8/web/host/templates/__init__.py
--rw-r--r--   0        0        0     2714 2023-02-18 22:43:23.224776 webint-0.1.8/web/host/templates/nginx_conf.conf
--rw-r--r--   0        0        0      653 2023-02-15 06:23:01.293121 webint-0.1.8/web/host/templates/nginx_index.html
--rw-r--r--   0        0        0     3114 2023-01-27 00:43:42.504109 webint-0.1.8/web/host/templates/nginx_site.conf
--rw-r--r--   0        0        0      877 2023-01-27 00:43:42.504109 webint-0.1.8/web/host/test_host.py
--rw-r--r--   0        0        0    42879 2023-01-27 00:43:42.496109 webint-0.1.8/web/markdown/__init__.py
--rw-r--r--   0        0        0   106063 2023-01-27 00:43:42.496109 webint-0.1.8/web/markdown/hyph_en_US.dic
--rw-r--r--   0        0        0     8827 2023-01-27 00:43:42.492109 webint-0.1.8/web/markdown/hyphenator.py
--rw-r--r--   0        0        0     2464 2023-01-27 00:43:42.492109 webint-0.1.8/web/markdown/titlecase.py
--rw-r--r--   0        0        0     1657 2023-01-27 00:43:42.524109 webint-0.1.8/web/response/__init__.py
--rw-r--r--   0        0        0     2501 2023-01-27 00:43:42.524109 webint-0.1.8/web/response/clienterror.py
--rw-r--r--   0        0        0      932 2023-01-27 00:43:42.524109 webint-0.1.8/web/response/informational.py
--rw-r--r--   0        0        0      901 2023-01-27 00:43:42.520109 webint-0.1.8/web/response/redirection.py
--rw-r--r--   0        0        0      427 2023-01-27 00:43:42.524109 webint-0.1.8/web/response/servererror.py
--rw-r--r--   0        0        0     1425 2023-01-27 00:43:42.528109 webint-0.1.8/web/response/success.py
--rw-r--r--   0        0        0      501 2023-01-27 00:43:42.520109 webint-0.1.8/web/response/util.py
--rw-r--r--   0        0        0    11900 2023-01-27 00:43:42.532109 webint-0.1.8/web/slrzd.py
--rw-r--r--   0        0        0     1992 2023-01-27 00:43:42.512109 webint-0.1.8/web/templating/__init__.py
--rw-r--r--   0        0        0      586 2023-01-27 00:43:42.516109 webint-0.1.8/web/templating/__main__.py
--rw-r--r--   0        0        0    25383 2023-01-27 00:43:42.516109 webint-0.1.8/web/templating/parse.py
--rw-r--r--   0        0        0    15402 2023-01-27 00:43:42.512109 webint-0.1.8/web/templating/templating.py
--rw-r--r--   0        0        0      866 2023-01-27 00:43:42.500109 webint-0.1.8/web/util.py
--rw-r--r--   0        0        0  4421355 1970-01-01 00:00:00.000000 webint-0.1.8/setup.py
--rw-r--r--   0        0        0     2084 1970-01-01 00:00:00.000000 webint-0.1.8/PKG-INFO
+-rw-r--r--   0        0        0      454 2023-01-27 00:43:42.480109 webint-0.1.9/README.md
+-rw-r--r--   0        0        0     1754 2023-02-20 22:15:40.645243 webint-0.1.9/pyproject.toml
+-rw-r--r--   0        0        0     1287 2023-02-18 00:57:16.443038 webint-0.1.9/web/__init__.py
+-rw-r--r--   0        0        0     7850 2023-02-20 21:32:24.772943 webint-0.1.9/web/__main__.py
+-rw-r--r--   0        0        0    46837 2023-02-20 22:05:37.072937 webint-0.1.9/web/framework/__init__.py
+-rw-r--r--   0        0        0     1233 2023-01-27 00:43:42.876114 webint-0.1.9/web/framework/letsencrypt.py
+-rw-r--r--   0        0        0        0 2023-01-27 00:43:42.536109 webint-0.1.9/web/framework/newmath.py
+-rw-r--r--   0        0        0    85473 2023-01-27 00:43:42.532109 webint-0.1.9/web/framework/passphrases.json
+-rw-r--r--   0        0        0     1339 2023-01-27 00:43:42.536109 webint-0.1.9/web/framework/passphrases.py
+-rw-r--r--   0        0        0     2840 2023-01-27 00:43:42.720111 webint-0.1.9/web/framework/static/1133.web.js
+-rw-r--r--   0        0        0      387 2023-01-27 00:43:42.756112 webint-0.1.9/web/framework/static/1133.web.js.LICENSE.txt
+-rw-r--r--   0        0        0     4935 2023-01-27 00:43:42.768112 webint-0.1.9/web/framework/static/1149.web.js
+-rw-r--r--   0        0        0      648 2023-01-27 00:43:42.672111 webint-0.1.9/web/framework/static/1149.web.js.LICENSE.txt
+-rw-r--r--   0        0        0    11823 2023-01-27 00:43:42.604110 webint-0.1.9/web/framework/static/1182.web.js
+-rw-r--r--   0        0        0      387 2023-01-27 00:43:42.740112 webint-0.1.9/web/framework/static/1182.web.js.LICENSE.txt
+-rw-r--r--   0        0        0    16087 2023-01-27 00:43:42.732112 webint-0.1.9/web/framework/static/1322.web.js
+-rw-r--r--   0        0        0      387 2023-01-27 00:43:42.868113 webint-0.1.9/web/framework/static/1322.web.js.LICENSE.txt
+-rw-r--r--   0        0        0     1850 2023-01-27 00:43:42.844113 webint-0.1.9/web/framework/static/195.web.js
+-rw-r--r--   0        0        0      387 2023-01-27 00:43:42.596110 webint-0.1.9/web/framework/static/195.web.js.LICENSE.txt
+-rw-r--r--   0        0        0     4183 2023-01-27 00:43:42.868113 webint-0.1.9/web/framework/static/2089.web.js
+-rw-r--r--   0        0        0      387 2023-01-27 00:43:42.760112 webint-0.1.9/web/framework/static/2089.web.js.LICENSE.txt
+-rw-r--r--   0        0        0     3594 2023-01-27 00:43:42.844113 webint-0.1.9/web/framework/static/2137.web.js
+-rw-r--r--   0        0        0      387 2023-01-27 00:43:42.644111 webint-0.1.9/web/framework/static/2137.web.js.LICENSE.txt
+-rw-r--r--   0        0        0    32199 2023-01-27 00:43:42.608110 webint-0.1.9/web/framework/static/2153.web.js
+-rw-r--r--   0        0        0      387 2023-01-27 00:43:42.776112 webint-0.1.9/web/framework/static/2153.web.js.LICENSE.txt
+-rw-r--r--   0        0        0     1124 2023-01-27 00:43:42.740112 webint-0.1.9/web/framework/static/2159.web.js
+-rw-r--r--   0        0        0      387 2023-01-27 00:43:42.632110 webint-0.1.9/web/framework/static/2159.web.js.LICENSE.txt
+-rw-r--r--   0        0        0     7626 2023-01-27 00:43:42.592110 webint-0.1.9/web/framework/static/2280.web.js
+-rw-r--r--   0        0        0      387 2023-01-27 00:43:42.764112 webint-0.1.9/web/framework/static/2280.web.js.LICENSE.txt
+-rw-r--r--   0        0        0     1706 2023-01-27 00:43:42.668111 webint-0.1.9/web/framework/static/2384.web.js
+-rw-r--r--   0        0        0      387 2023-01-27 00:43:42.552109 webint-0.1.9/web/framework/static/2384.web.js.LICENSE.txt
+-rw-r--r--   0        0        0     3096 2023-01-27 00:43:42.652111 webint-0.1.9/web/framework/static/2456.web.js
+-rw-r--r--   0        0        0      387 2023-01-27 00:43:42.740112 webint-0.1.9/web/framework/static/2456.web.js.LICENSE.txt
+-rw-r--r--   0        0        0    16962 2023-01-27 00:43:42.748112 webint-0.1.9/web/framework/static/2489.web.js
+-rw-r--r--   0        0        0      387 2023-01-27 00:43:42.852113 webint-0.1.9/web/framework/static/2489.web.js.LICENSE.txt
+-rw-r--r--   0        0        0     5469 2023-01-27 00:43:42.552109 webint-0.1.9/web/framework/static/249.web.js
+-rw-r--r--   0        0        0      387 2023-01-27 00:43:42.596110 webint-0.1.9/web/framework/static/249.web.js.LICENSE.txt
+-rw-r--r--   0        0        0     5021 2023-01-27 00:43:42.716112 webint-0.1.9/web/framework/static/2755.web.js
+-rw-r--r--   0        0        0      387 2023-01-27 00:43:42.752112 webint-0.1.9/web/framework/static/2755.web.js.LICENSE.txt
+-rw-r--r--   0        0        0     7879 2023-01-27 00:43:42.688111 webint-0.1.9/web/framework/static/2826.web.js
+-rw-r--r--   0        0        0      387 2023-01-27 00:43:42.692111 webint-0.1.9/web/framework/static/2826.web.js.LICENSE.txt
+-rw-r--r--   0        0        0     2402 2023-01-27 00:43:42.724112 webint-0.1.9/web/framework/static/2919.web.js
+-rw-r--r--   0        0        0      387 2023-01-27 00:43:42.616110 webint-0.1.9/web/framework/static/2919.web.js.LICENSE.txt
+-rw-r--r--   0        0        0     3292 2023-01-27 00:43:42.704111 webint-0.1.9/web/framework/static/3241.web.js
+-rw-r--r--   0        0        0      387 2023-01-27 00:43:42.548109 webint-0.1.9/web/framework/static/3241.web.js.LICENSE.txt
+-rw-r--r--   0        0        0     3579 2023-01-27 00:43:42.648111 webint-0.1.9/web/framework/static/3282.web.js
+-rw-r--r--   0        0        0      387 2023-01-27 00:43:42.656111 webint-0.1.9/web/framework/static/3282.web.js.LICENSE.txt
+-rw-r--r--   0        0        0     2208 2023-01-27 00:43:42.676111 webint-0.1.9/web/framework/static/3339.web.js
+-rw-r--r--   0        0        0      387 2023-01-27 00:43:42.872114 webint-0.1.9/web/framework/static/3339.web.js.LICENSE.txt
+-rw-r--r--   0        0        0     6763 2023-01-27 00:43:42.856113 webint-0.1.9/web/framework/static/3374.web.js
+-rw-r--r--   0        0        0      387 2023-01-27 00:43:42.776112 webint-0.1.9/web/framework/static/3374.web.js.LICENSE.txt
+-rw-r--r--   0        0        0     3600 2023-01-27 00:43:42.744112 webint-0.1.9/web/framework/static/3558.web.js
+-rw-r--r--   0        0        0      387 2023-01-27 00:43:42.752112 webint-0.1.9/web/framework/static/3558.web.js.LICENSE.txt
+-rw-r--r--   0        0        0     2680 2023-01-27 00:43:42.712111 webint-0.1.9/web/framework/static/3559.web.js
+-rw-r--r--   0        0        0      387 2023-01-27 00:43:42.544109 webint-0.1.9/web/framework/static/3559.web.js.LICENSE.txt
+-rw-r--r--   0        0        0     4536 2023-01-27 00:43:42.724112 webint-0.1.9/web/framework/static/3657.web.js
+-rw-r--r--   0        0        0      387 2023-01-27 00:43:42.728112 webint-0.1.9/web/framework/static/3657.web.js.LICENSE.txt
+-rw-r--r--   0        0        0     4935 2023-01-27 00:43:42.620110 webint-0.1.9/web/framework/static/3659.web.js
+-rw-r--r--   0        0        0      387 2023-01-27 00:43:42.772112 webint-0.1.9/web/framework/static/3659.web.js.LICENSE.txt
+-rw-r--r--   0        0        0    32750 2023-01-27 00:43:42.556110 webint-0.1.9/web/framework/static/3684.web.js
+-rw-r--r--   0        0        0      387 2023-01-27 00:43:42.660111 webint-0.1.9/web/framework/static/3684.web.js.LICENSE.txt
+-rw-r--r--   0        0        0     1789 2023-01-27 00:43:42.760112 webint-0.1.9/web/framework/static/3788.web.js
+-rw-r--r--   0        0        0      387 2023-01-27 00:43:42.868113 webint-0.1.9/web/framework/static/3788.web.js.LICENSE.txt
+-rw-r--r--   0        0        0     8050 2023-01-27 00:43:42.676111 webint-0.1.9/web/framework/static/3931.web.js
+-rw-r--r--   0        0        0      387 2023-01-27 00:43:42.772112 webint-0.1.9/web/framework/static/3931.web.js.LICENSE.txt
+-rw-r--r--   0        0        0     3922 2023-01-27 00:43:42.692111 webint-0.1.9/web/framework/static/3998.web.js
+-rw-r--r--   0        0        0      387 2023-01-27 00:43:42.552109 webint-0.1.9/web/framework/static/3998.web.js.LICENSE.txt
+-rw-r--r--   0        0        0     2423 2023-01-27 00:43:42.864113 webint-0.1.9/web/framework/static/429.web.js
+-rw-r--r--   0        0        0      387 2023-01-27 00:43:42.712111 webint-0.1.9/web/framework/static/429.web.js.LICENSE.txt
+-rw-r--r--   0        0        0      870 2023-01-27 00:43:42.600110 webint-0.1.9/web/framework/static/4463.web.js
+-rw-r--r--   0        0        0      387 2023-01-27 00:43:42.624110 webint-0.1.9/web/framework/static/4463.web.js.LICENSE.txt
+-rw-r--r--   0        0        0     2508 2023-01-27 00:43:42.684111 webint-0.1.9/web/framework/static/4552.web.js
+-rw-r--r--   0        0        0      387 2023-01-27 00:43:42.632110 webint-0.1.9/web/framework/static/4552.web.js.LICENSE.txt
+-rw-r--r--   0        0        0     1440 2023-01-27 00:43:42.668111 webint-0.1.9/web/framework/static/468.web.js
+-rw-r--r--   0        0        0      387 2023-01-27 00:43:42.864113 webint-0.1.9/web/framework/static/468.web.js.LICENSE.txt
+-rw-r--r--   0        0        0    14186 2023-01-27 00:43:42.740112 webint-0.1.9/web/framework/static/4776.web.js
+-rw-r--r--   0        0        0      387 2023-01-27 00:43:42.716112 webint-0.1.9/web/framework/static/4776.web.js.LICENSE.txt
+-rw-r--r--   0        0        0     6435 2023-01-27 00:43:42.636110 webint-0.1.9/web/framework/static/4932.web.js
+-rw-r--r--   0        0        0      387 2023-01-27 00:43:42.724112 webint-0.1.9/web/framework/static/4932.web.js.LICENSE.txt
+-rw-r--r--   0        0        0     3947 2023-01-27 00:43:42.560109 webint-0.1.9/web/framework/static/501.web.js
+-rw-r--r--   0        0        0      387 2023-01-27 00:43:42.644111 webint-0.1.9/web/framework/static/501.web.js.LICENSE.txt
+-rw-r--r--   0        0        0    18620 2023-01-27 00:43:42.636110 webint-0.1.9/web/framework/static/5021.web.js
+-rw-r--r--   0        0        0      387 2023-01-27 00:43:42.552109 webint-0.1.9/web/framework/static/5021.web.js.LICENSE.txt
+-rw-r--r--   0        0        0     8278 2023-01-27 00:43:42.624110 webint-0.1.9/web/framework/static/5289.web.js
+-rw-r--r--   0        0        0      387 2023-01-27 00:43:42.848113 webint-0.1.9/web/framework/static/5289.web.js.LICENSE.txt
+-rw-r--r--   0        0        0     7172 2023-01-27 00:43:42.608110 webint-0.1.9/web/framework/static/5337.web.js
+-rw-r--r--   0        0        0      387 2023-01-27 00:43:42.612110 webint-0.1.9/web/framework/static/5337.web.js.LICENSE.txt
+-rw-r--r--   0        0        0     8772 2023-01-27 00:43:42.644111 webint-0.1.9/web/framework/static/5341.web.js
+-rw-r--r--   0        0        0      387 2023-01-27 00:43:42.740112 webint-0.1.9/web/framework/static/5341.web.js.LICENSE.txt
+-rw-r--r--   0        0        0     3983 2023-01-27 00:43:42.592110 webint-0.1.9/web/framework/static/5466.web.js
+-rw-r--r--   0        0        0      387 2023-01-27 00:43:42.708111 webint-0.1.9/web/framework/static/5466.web.js.LICENSE.txt
+-rw-r--r--   0        0        0     3829 2023-01-27 00:43:42.640111 webint-0.1.9/web/framework/static/5490.web.js
+-rw-r--r--   0        0        0      387 2023-01-27 00:43:42.868113 webint-0.1.9/web/framework/static/5490.web.js.LICENSE.txt
+-rw-r--r--   0        0        0     5365 2023-01-27 00:43:42.672111 webint-0.1.9/web/framework/static/5502.web.js
+-rw-r--r--   0        0        0      387 2023-01-27 00:43:42.704111 webint-0.1.9/web/framework/static/5502.web.js.LICENSE.txt
+-rw-r--r--   0        0        0     6001 2023-01-27 00:43:42.860113 webint-0.1.9/web/framework/static/5528.web.js
+-rw-r--r--   0        0        0      387 2023-01-27 00:43:42.544109 webint-0.1.9/web/framework/static/5528.web.js.LICENSE.txt
+-rw-r--r--   0        0        0     3611 2023-01-27 00:43:42.732112 webint-0.1.9/web/framework/static/570.web.js
+-rw-r--r--   0        0        0      387 2023-01-27 00:43:42.684111 webint-0.1.9/web/framework/static/570.web.js.LICENSE.txt
+-rw-r--r--   0        0        0     4851 2023-01-27 00:43:42.552109 webint-0.1.9/web/framework/static/5892.web.js
+-rw-r--r--   0        0        0      387 2023-01-27 00:43:42.860113 webint-0.1.9/web/framework/static/5892.web.js.LICENSE.txt
+-rw-r--r--   0        0        0     7409 2023-01-27 00:43:42.752112 webint-0.1.9/web/framework/static/5986.web.js
+-rw-r--r--   0        0        0      387 2023-01-27 00:43:42.704111 webint-0.1.9/web/framework/static/5986.web.js.LICENSE.txt
+-rw-r--r--   0        0        0     1832 2023-01-27 00:43:42.748112 webint-0.1.9/web/framework/static/6259.web.js
+-rw-r--r--   0        0        0      387 2023-01-27 00:43:42.560109 webint-0.1.9/web/framework/static/6259.web.js.LICENSE.txt
+-rw-r--r--   0        0        0     3154 2023-01-27 00:43:42.704111 webint-0.1.9/web/framework/static/6389.web.js
+-rw-r--r--   0        0        0      387 2023-01-27 00:43:42.656111 webint-0.1.9/web/framework/static/6389.web.js.LICENSE.txt
+-rw-r--r--   0        0        0     3462 2023-01-27 00:43:42.536109 webint-0.1.9/web/framework/static/6422.web.js
+-rw-r--r--   0        0        0      387 2023-01-27 00:43:42.868113 webint-0.1.9/web/framework/static/6422.web.js.LICENSE.txt
+-rw-r--r--   0        0        0     9666 2023-01-27 00:43:42.616110 webint-0.1.9/web/framework/static/6425.web.js
+-rw-r--r--   0        0        0      387 2023-01-27 00:43:42.780112 webint-0.1.9/web/framework/static/6425.web.js.LICENSE.txt
+-rw-r--r--   0        0        0     1892 2023-01-27 00:43:42.852113 webint-0.1.9/web/framework/static/6548.web.js
+-rw-r--r--   0        0        0      387 2023-01-27 00:43:42.556110 webint-0.1.9/web/framework/static/6548.web.js.LICENSE.txt
+-rw-r--r--   0        0        0     1868 2023-01-27 00:43:42.856113 webint-0.1.9/web/framework/static/6681.web.js
+-rw-r--r--   0        0        0      387 2023-01-27 00:43:42.660111 webint-0.1.9/web/framework/static/6681.web.js.LICENSE.txt
+-rw-r--r--   0        0        0     4546 2023-01-27 00:43:42.736112 webint-0.1.9/web/framework/static/7050.web.js
+-rw-r--r--   0        0        0      387 2023-01-27 00:43:42.872114 webint-0.1.9/web/framework/static/7050.web.js.LICENSE.txt
+-rw-r--r--   0        0        0     5376 2023-01-27 00:43:42.548109 webint-0.1.9/web/framework/static/7138.web.js
+-rw-r--r--   0        0        0      387 2023-01-27 00:43:42.656111 webint-0.1.9/web/framework/static/7138.web.js.LICENSE.txt
+-rw-r--r--   0        0        0     3971 2023-01-27 00:43:42.756112 webint-0.1.9/web/framework/static/7201.web.js
+-rw-r--r--   0        0        0      387 2023-01-27 00:43:42.616110 webint-0.1.9/web/framework/static/7201.web.js.LICENSE.txt
+-rw-r--r--   0        0        0     2958 2023-01-27 00:43:42.764112 webint-0.1.9/web/framework/static/7318.web.js
+-rw-r--r--   0        0        0      387 2023-01-27 00:43:42.648111 webint-0.1.9/web/framework/static/7318.web.js.LICENSE.txt
+-rw-r--r--   0        0        0     7341 2023-01-27 00:43:42.728112 webint-0.1.9/web/framework/static/7441.web.js
+-rw-r--r--   0        0        0      387 2023-01-27 00:43:42.632110 webint-0.1.9/web/framework/static/7441.web.js.LICENSE.txt
+-rw-r--r--   0        0        0    38093 2023-01-27 00:43:42.680111 webint-0.1.9/web/framework/static/7660.web.js
+-rw-r--r--   0        0        0      387 2023-01-27 00:43:42.628110 webint-0.1.9/web/framework/static/7660.web.js.LICENSE.txt
+-rw-r--r--   0        0        0     2602 2023-01-27 00:43:42.708111 webint-0.1.9/web/framework/static/7730.web.js
+-rw-r--r--   0        0        0      387 2023-01-27 00:43:42.544109 webint-0.1.9/web/framework/static/7730.web.js.LICENSE.txt
+-rw-r--r--   0        0        0     8528 2023-01-27 00:43:42.604110 webint-0.1.9/web/framework/static/7864.web.js
+-rw-r--r--   0        0        0      387 2023-01-27 00:43:42.608110 webint-0.1.9/web/framework/static/7864.web.js.LICENSE.txt
+-rw-r--r--   0        0        0     2785 2023-01-27 00:43:42.544109 webint-0.1.9/web/framework/static/788.web.js
+-rw-r--r--   0        0        0      387 2023-01-27 00:43:42.848113 webint-0.1.9/web/framework/static/788.web.js.LICENSE.txt
+-rw-r--r--   0        0        0     3928 2023-01-27 00:43:42.756112 webint-0.1.9/web/framework/static/8059.web.js
+-rw-r--r--   0        0        0      387 2023-01-27 00:43:42.604110 webint-0.1.9/web/framework/static/8059.web.js.LICENSE.txt
+-rw-r--r--   0        0        0     3018 2023-01-27 00:43:42.680111 webint-0.1.9/web/framework/static/8106.web.js
+-rw-r--r--   0        0        0      387 2023-01-27 00:43:42.756112 webint-0.1.9/web/framework/static/8106.web.js.LICENSE.txt
+-rw-r--r--   0        0        0     6214 2023-01-27 00:43:42.752112 webint-0.1.9/web/framework/static/8262.web.js
+-rw-r--r--   0        0        0      387 2023-01-27 00:43:42.856113 webint-0.1.9/web/framework/static/8262.web.js.LICENSE.txt
+-rw-r--r--   0        0        0     2283 2023-01-27 00:43:42.760112 webint-0.1.9/web/framework/static/8356.web.js
+-rw-r--r--   0        0        0      387 2023-01-27 00:43:42.604110 webint-0.1.9/web/framework/static/8356.web.js.LICENSE.txt
+-rw-r--r--   0        0        0     2575 2023-01-27 00:43:42.772112 webint-0.1.9/web/framework/static/8416.web.js
+-rw-r--r--   0        0        0      387 2023-01-27 00:43:42.708111 webint-0.1.9/web/framework/static/8416.web.js.LICENSE.txt
+-rw-r--r--   0        0        0     2023 2023-01-27 00:43:42.688111 webint-0.1.9/web/framework/static/8512.web.js
+-rw-r--r--   0        0        0      387 2023-01-27 00:43:42.688111 webint-0.1.9/web/framework/static/8512.web.js.LICENSE.txt
+-rw-r--r--   0        0        0     3244 2023-01-27 00:43:42.652111 webint-0.1.9/web/framework/static/8562.web.js
+-rw-r--r--   0        0        0      387 2023-01-27 00:43:42.860113 webint-0.1.9/web/framework/static/8562.web.js.LICENSE.txt
+-rw-r--r--   0        0        0     5814 2023-01-27 00:43:42.540109 webint-0.1.9/web/framework/static/8670.web.js
+-rw-r--r--   0        0        0      387 2023-01-27 00:43:42.588110 webint-0.1.9/web/framework/static/8670.web.js.LICENSE.txt
+-rw-r--r--   0        0        0     4273 2023-01-27 00:43:42.780112 webint-0.1.9/web/framework/static/8842.web.js
+-rw-r--r--   0        0        0      387 2023-01-27 00:43:42.676111 webint-0.1.9/web/framework/static/8842.web.js.LICENSE.txt
+-rw-r--r--   0        0        0     9780 2023-01-27 00:43:42.772112 webint-0.1.9/web/framework/static/888.web.js
+-rw-r--r--   0        0        0      387 2023-01-27 00:43:42.672111 webint-0.1.9/web/framework/static/888.web.js.LICENSE.txt
+-rw-r--r--   0        0        0     3411 2023-01-27 00:43:42.736112 webint-0.1.9/web/framework/static/8903.web.js
+-rw-r--r--   0        0        0      387 2023-01-27 00:43:42.844113 webint-0.1.9/web/framework/static/8903.web.js.LICENSE.txt
+-rw-r--r--   0        0        0    13426 2023-01-27 00:43:42.540109 webint-0.1.9/web/framework/static/9338.web.js
+-rw-r--r--   0        0        0      387 2023-01-27 00:43:42.716112 webint-0.1.9/web/framework/static/9338.web.js.LICENSE.txt
+-rw-r--r--   0        0        0    11276 2023-01-27 00:43:42.600110 webint-0.1.9/web/framework/static/938.web.js
+-rw-r--r--   0        0        0      387 2023-01-27 00:43:42.848113 webint-0.1.9/web/framework/static/938.web.js.LICENSE.txt
+-rw-r--r--   0        0        0     9067 2023-01-27 00:43:42.720111 webint-0.1.9/web/framework/static/9407.web.js
+-rw-r--r--   0        0        0      387 2023-01-27 00:43:42.548109 webint-0.1.9/web/framework/static/9407.web.js.LICENSE.txt
+-rw-r--r--   0        0        0     3613 2023-01-27 00:43:42.592110 webint-0.1.9/web/framework/static/9502.web.js
+-rw-r--r--   0        0        0      387 2023-01-27 00:43:42.728112 webint-0.1.9/web/framework/static/9502.web.js.LICENSE.txt
+-rw-r--r--   0        0        0    10318 2023-01-27 00:43:42.656111 webint-0.1.9/web/framework/static/959.web.js
+-rw-r--r--   0        0        0      387 2023-01-27 00:43:42.588110 webint-0.1.9/web/framework/static/959.web.js.LICENSE.txt
+-rw-r--r--   0        0        0     2458 2023-01-27 00:43:42.620110 webint-0.1.9/web/framework/static/966.web.js
+-rw-r--r--   0        0        0      387 2023-01-27 00:43:42.768112 webint-0.1.9/web/framework/static/966.web.js.LICENSE.txt
+-rw-r--r--   0        0        0     3005 2023-01-27 00:43:42.708111 webint-0.1.9/web/framework/static/9721.web.js
+-rw-r--r--   0        0        0      387 2023-01-27 00:43:42.592110 webint-0.1.9/web/framework/static/9721.web.js.LICENSE.txt
+-rw-r--r--   0        0        0     2146 2023-01-27 00:43:42.688111 webint-0.1.9/web/framework/static/9762.web.js
+-rw-r--r--   0        0        0      387 2023-01-27 00:43:42.748112 webint-0.1.9/web/framework/static/9762.web.js.LICENSE.txt
+-rw-r--r--   0        0        0    21621 2023-01-27 00:43:42.608110 webint-0.1.9/web/framework/static/9822.web.js
+-rw-r--r--   0        0        0    72504 2023-01-27 00:43:42.672111 webint-0.1.9/web/framework/static/b797181c93b3755f4fa1.ttf
+-rw-r--r--   0        0        0  4897844 2023-01-27 00:43:42.584110 webint-0.1.9/web/framework/static/css.worker.js
+-rw-r--r--   0        0        0      387 2023-01-27 00:43:42.596110 webint-0.1.9/web/framework/static/css.worker.js.LICENSE.txt
+-rw-r--r--   0        0        0  1637641 2023-01-27 00:43:42.664111 webint-0.1.9/web/framework/static/editor.worker.js
+-rw-r--r--   0        0        0  3399495 2023-01-27 00:43:42.568110 webint-0.1.9/web/framework/static/html.worker.js
+-rw-r--r--   0        0        0      387 2023-01-27 00:43:42.620110 webint-0.1.9/web/framework/static/html.worker.js.LICENSE.txt
+-rw-r--r--   0        0        0  2332252 2023-01-27 00:43:42.700111 webint-0.1.9/web/framework/static/json.worker.js
+-rw-r--r--   0        0        0      387 2023-01-27 00:43:42.724112 webint-0.1.9/web/framework/static/json.worker.js.LICENSE.txt
+-rw-r--r--   0        0        0      569 2023-01-27 00:43:42.540109 webint-0.1.9/web/framework/static/measure.png
+-rw-r--r--   0        0        0    19132 2023-01-27 00:43:42.708111 webint-0.1.9/web/framework/static/node_modules_monaco-editor_esm_vs_basic-languages_apex_apex_js.web.js
+-rw-r--r--   0        0        0     6058 2023-01-27 00:43:42.596110 webint-0.1.9/web/framework/static/node_modules_monaco-editor_esm_vs_basic-languages_azcli_azcli_js.web.js
+-rw-r--r--   0        0        0     9006 2023-01-27 00:43:42.588110 webint-0.1.9/web/framework/static/node_modules_monaco-editor_esm_vs_basic-languages_bat_bat_js.web.js
+-rw-r--r--   0        0        0    12376 2023-01-27 00:43:42.600110 webint-0.1.9/web/framework/static/node_modules_monaco-editor_esm_vs_basic-languages_bicep_bicep_js.web.js
+-rw-r--r--   0        0        0    11717 2023-01-27 00:43:42.684111 webint-0.1.9/web/framework/static/node_modules_monaco-editor_esm_vs_basic-languages_cameligo_cameligo_js.web.js
+-rw-r--r--   0        0        0    17396 2023-01-27 00:43:42.684111 webint-0.1.9/web/framework/static/node_modules_monaco-editor_esm_vs_basic-languages_coffee_coffee_js.web.js
+-rw-r--r--   0        0        0    24827 2023-01-27 00:43:42.592110 webint-0.1.9/web/framework/static/node_modules_monaco-editor_esm_vs_basic-languages_cpp_cpp_js.web.js
+-rw-r--r--   0        0        0    21742 2023-01-27 00:43:42.864113 webint-0.1.9/web/framework/static/node_modules_monaco-editor_esm_vs_basic-languages_csharp_csharp_js.web.js
+-rw-r--r--   0        0        0     6491 2023-01-27 00:43:42.712111 webint-0.1.9/web/framework/static/node_modules_monaco-editor_esm_vs_basic-languages_csp_csp_js.web.js
+-rw-r--r--   0        0        0    19159 2023-01-27 00:43:42.668111 webint-0.1.9/web/framework/static/node_modules_monaco-editor_esm_vs_basic-languages_css_css_js.web.js
+-rw-r--r--   0        0        0    16682 2023-01-27 00:43:42.732112 webint-0.1.9/web/framework/static/node_modules_monaco-editor_esm_vs_basic-languages_cypher_cypher_js.web.js
+-rw-r--r--   0        0        0    19293 2023-01-27 00:43:42.748112 webint-0.1.9/web/framework/static/node_modules_monaco-editor_esm_vs_basic-languages_dart_dart_js.web.js
+-rw-r--r--   0        0        0    10624 2023-01-27 00:43:42.732112 webint-0.1.9/web/framework/static/node_modules_monaco-editor_esm_vs_basic-languages_dockerfile_dockerfile_js.web.js
+-rw-r--r--   0        0        0    25376 2023-01-27 00:43:42.768112 webint-0.1.9/web/framework/static/node_modules_monaco-editor_esm_vs_basic-languages_ecl_ecl_js.web.js
+-rw-r--r--   0        0        0     9895 2023-01-27 00:43:42.764112 webint-0.1.9/web/framework/static/node_modules_monaco-editor_esm_vs_basic-languages_flow9_flow9_js.web.js
+-rw-r--r--   0        0        0    14428 2023-01-27 00:43:42.780112 webint-0.1.9/web/framework/static/node_modules_monaco-editor_esm_vs_basic-languages_fsharp_fsharp_js.web.js
+-rw-r--r--   0        0        0    13553 2023-01-27 00:43:42.672111 webint-0.1.9/web/framework/static/node_modules_monaco-editor_esm_vs_basic-languages_go_go_js.web.js
+-rw-r--r--   0        0        0    11277 2023-01-27 00:43:42.844113 webint-0.1.9/web/framework/static/node_modules_monaco-editor_esm_vs_basic-languages_graphql_graphql_js.web.js
+-rw-r--r--   0        0        0    15438 2023-01-27 00:43:42.692111 webint-0.1.9/web/framework/static/node_modules_monaco-editor_esm_vs_basic-languages_hcl_hcl_js.web.js
+-rw-r--r--   0        0        0    23800 2023-01-27 00:43:42.616110 webint-0.1.9/web/framework/static/node_modules_monaco-editor_esm_vs_basic-languages_html_html_js.web.js
+-rw-r--r--   0        0        0     6406 2023-01-27 00:43:42.628110 webint-0.1.9/web/framework/static/node_modules_monaco-editor_esm_vs_basic-languages_ini_ini_js.web.js
+-rw-r--r--   0        0        0    15210 2023-01-27 00:43:42.692111 webint-0.1.9/web/framework/static/node_modules_monaco-editor_esm_vs_basic-languages_java_java_js.web.js
+-rw-r--r--   0        0        0    16332 2023-01-27 00:43:42.776112 webint-0.1.9/web/framework/static/node_modules_monaco-editor_esm_vs_basic-languages_kotlin_kotlin_js.web.js
+-rw-r--r--   0        0        0    16679 2023-01-27 00:43:42.784112 webint-0.1.9/web/framework/static/node_modules_monaco-editor_esm_vs_basic-languages_less_less_js.web.js
+-rw-r--r--   0        0        0    12072 2023-01-27 00:43:42.612110 webint-0.1.9/web/framework/static/node_modules_monaco-editor_esm_vs_basic-languages_lexon_lexon_js.web.js
+-rw-r--r--   0        0        0    19465 2023-01-27 00:43:42.772112 webint-0.1.9/web/framework/static/node_modules_monaco-editor_esm_vs_basic-languages_liquid_liquid_js.web.js
+-rw-r--r--   0        0        0    11332 2023-01-27 00:43:42.628110 webint-0.1.9/web/framework/static/node_modules_monaco-editor_esm_vs_basic-languages_lua_lua_js.web.js
+-rw-r--r--   0        0        0    13995 2023-01-27 00:43:42.760112 webint-0.1.9/web/framework/static/node_modules_monaco-editor_esm_vs_basic-languages_m3_m3_js.web.js
+-rw-r--r--   0        0        0    17583 2023-01-27 00:43:42.648111 webint-0.1.9/web/framework/static/node_modules_monaco-editor_esm_vs_basic-languages_markdown_markdown_js.web.js
+-rw-r--r--   0        0        0    13421 2023-01-27 00:43:42.780112 webint-0.1.9/web/framework/static/node_modules_monaco-editor_esm_vs_basic-languages_mips_mips_js.web.js
+-rw-r--r--   0        0        0    22656 2023-01-27 00:43:42.736112 webint-0.1.9/web/framework/static/node_modules_monaco-editor_esm_vs_basic-languages_msdax_msdax_js.web.js
+-rw-r--r--   0        0        0    12524 2023-01-27 00:43:42.640111 webint-0.1.9/web/framework/static/node_modules_monaco-editor_esm_vs_basic-languages_objective-c_objective-c_js.web.js
+-rw-r--r--   0        0        0    15300 2023-01-27 00:43:42.656111 webint-0.1.9/web/framework/static/node_modules_monaco-editor_esm_vs_basic-languages_pascal_pascal_js.web.js
+-rw-r--r--   0        0        0    10923 2023-01-27 00:43:42.660111 webint-0.1.9/web/framework/static/node_modules_monaco-editor_esm_vs_basic-languages_pascaligo_pascaligo_js.web.js
+-rw-r--r--   0        0        0     9896 2023-01-27 00:43:42.640111 webint-0.1.9/web/framework/static/node_modules_monaco-editor_esm_vs_basic-languages_pla_pla_js.web.js
+-rw-r--r--   0        0        0    17017 2023-01-27 00:43:42.752112 webint-0.1.9/web/framework/static/node_modules_monaco-editor_esm_vs_basic-languages_powershell_powershell_js.web.js
+-rw-r--r--   0        0        0    25438 2023-01-27 00:43:42.644111 webint-0.1.9/web/framework/static/node_modules_monaco-editor_esm_vs_basic-languages_pug_pug_js.web.js
+-rw-r--r--   0        0        0    18459 2023-01-27 00:43:42.556110 webint-0.1.9/web/framework/static/node_modules_monaco-editor_esm_vs_basic-languages_python_python_js.web.js
+-rw-r--r--   0        0        0    15716 2023-01-27 00:43:42.716112 webint-0.1.9/web/framework/static/node_modules_monaco-editor_esm_vs_basic-languages_qsharp_qsharp_js.web.js
+-rw-r--r--   0        0        0    15762 2023-01-27 00:43:42.652111 webint-0.1.9/web/framework/static/node_modules_monaco-editor_esm_vs_basic-languages_r_r_js.web.js
+-rw-r--r--   0        0        0    17644 2023-01-27 00:43:42.636110 webint-0.1.9/web/framework/static/node_modules_monaco-editor_esm_vs_basic-languages_redis_redis_js.web.js
+-rw-r--r--   0        0        0    16271 2023-01-27 00:43:42.676111 webint-0.1.9/web/framework/static/node_modules_monaco-editor_esm_vs_basic-languages_restructuredtext_restructuredtext_js.web.js
+-rw-r--r--   0        0        0    20405 2023-01-27 00:43:42.612110 webint-0.1.9/web/framework/static/node_modules_monaco-editor_esm_vs_basic-languages_rust_rust_js.web.js
+-rw-r--r--   0        0        0     9291 2023-01-27 00:43:42.624110 webint-0.1.9/web/framework/static/node_modules_monaco-editor_esm_vs_basic-languages_sb_sb_js.web.js
+-rw-r--r--   0        0        0     9201 2023-01-27 00:43:42.764112 webint-0.1.9/web/framework/static/node_modules_monaco-editor_esm_vs_basic-languages_scheme_scheme_js.web.js
+-rw-r--r--   0        0        0    26294 2023-01-27 00:43:42.864113 webint-0.1.9/web/framework/static/node_modules_monaco-editor_esm_vs_basic-languages_scss_scss_js.web.js
+-rw-r--r--   0        0        0    15071 2023-01-27 00:43:42.776112 webint-0.1.9/web/framework/static/node_modules_monaco-editor_esm_vs_basic-languages_shell_shell_js.web.js
+-rw-r--r--   0        0        0    13358 2023-01-27 00:43:42.716112 webint-0.1.9/web/framework/static/node_modules_monaco-editor_esm_vs_basic-languages_sophia_sophia_js.web.js
+-rw-r--r--   0        0        0    12795 2023-01-27 00:43:42.616110 webint-0.1.9/web/framework/static/node_modules_monaco-editor_esm_vs_basic-languages_sparql_sparql_js.web.js
+-rw-r--r--   0        0        0    22397 2023-01-27 00:43:42.636110 webint-0.1.9/web/framework/static/node_modules_monaco-editor_esm_vs_basic-languages_swift_swift_js.web.js
+-rw-r--r--   0        0        0    16853 2023-01-27 00:43:42.652111 webint-0.1.9/web/framework/static/node_modules_monaco-editor_esm_vs_basic-languages_tcl_tcl_js.web.js
+-rw-r--r--   0        0        0    25948 2023-01-27 00:43:42.640111 webint-0.1.9/web/framework/static/node_modules_monaco-editor_esm_vs_basic-languages_twig_twig_js.web.js
+-rw-r--r--   0        0        0    25135 2023-01-27 00:43:42.848113 webint-0.1.9/web/framework/static/node_modules_monaco-editor_esm_vs_basic-languages_typescript_typescript_js.web.js
+-rw-r--r--   0        0        0    25134 2023-01-27 00:43:42.588110 webint-0.1.9/web/framework/static/node_modules_monaco-editor_esm_vs_basic-languages_vb_vb_js.web.js
+-rw-r--r--   0        0        0    12067 2023-01-27 00:43:42.556110 webint-0.1.9/web/framework/static/node_modules_monaco-editor_esm_vs_basic-languages_xml_xml_js.web.js
+-rw-r--r--   0        0        0    18657 2023-01-27 00:43:42.860113 webint-0.1.9/web/framework/static/node_modules_monaco-editor_esm_vs_basic-languages_yaml_yaml_js.web.js
+-rw-r--r--   0        0        0     9872 2023-01-27 00:43:42.600110 webint-0.1.9/web/framework/static/solarized-site.css
+-rw-r--r--   0        0        0     4743 2023-01-27 00:43:42.872114 webint-0.1.9/web/framework/static/solarized.css
+-rw-r--r--   0        0        0 22565048 2023-01-27 00:43:42.836113 webint-0.1.9/web/framework/static/ts.worker.js
+-rw-r--r--   0        0        0     1199 2023-01-27 00:43:42.728112 webint-0.1.9/web/framework/static/ts.worker.js.LICENSE.txt
+-rw-r--r--   0        0        0    64818 2023-01-27 00:43:42.680111 webint-0.1.9/web/framework/static/vendors-node_modules_monaco-editor_esm_vs_basic-languages_abap_abap_js.web.js
+-rw-r--r--   0        0        0    42160 2023-01-27 00:43:42.852113 webint-0.1.9/web/framework/static/vendors-node_modules_monaco-editor_esm_vs_basic-languages_clojure_clojure_js.web.js
+-rw-r--r--   0        0        0    40113 2023-01-27 00:43:42.680111 webint-0.1.9/web/framework/static/vendors-node_modules_monaco-editor_esm_vs_basic-languages_elixir_elixir_js.web.js
+-rw-r--r--   0        0        0    71501 2023-01-27 00:43:42.736112 webint-0.1.9/web/framework/static/vendors-node_modules_monaco-editor_esm_vs_basic-languages_freemarker2_freemarker2_js.web.js
+-rw-r--r--   0        0        0    31775 2023-01-27 00:43:42.640111 webint-0.1.9/web/framework/static/vendors-node_modules_monaco-editor_esm_vs_basic-languages_handlebars_handlebars_js.web.js
+-rw-r--r--   0        0        0    31412 2023-01-27 00:43:42.856113 webint-0.1.9/web/framework/static/vendors-node_modules_monaco-editor_esm_vs_basic-languages_javascript_javascript_js.web.js
+-rw-r--r--   0        0        0    32008 2023-01-27 00:43:42.848113 webint-0.1.9/web/framework/static/vendors-node_modules_monaco-editor_esm_vs_basic-languages_julia_julia_js.web.js
+-rw-r--r--   0        0        0    48644 2023-01-27 00:43:42.768112 webint-0.1.9/web/framework/static/vendors-node_modules_monaco-editor_esm_vs_basic-languages_mysql_mysql_js.web.js
+-rw-r--r--   0        0        0    37499 2023-01-27 00:43:42.852113 webint-0.1.9/web/framework/static/vendors-node_modules_monaco-editor_esm_vs_basic-languages_perl_perl_js.web.js
+-rw-r--r--   0        0        0    52967 2023-01-27 00:43:42.688111 webint-0.1.9/web/framework/static/vendors-node_modules_monaco-editor_esm_vs_basic-languages_pgsql_pgsql_js.web.js
+-rw-r--r--   0        0        0    34711 2023-01-27 00:43:42.712111 webint-0.1.9/web/framework/static/vendors-node_modules_monaco-editor_esm_vs_basic-languages_php_php_js.web.js
+-rw-r--r--   0        0        0    36168 2023-01-27 00:43:42.548109 webint-0.1.9/web/framework/static/vendors-node_modules_monaco-editor_esm_vs_basic-languages_postiats_postiats_js.web.js
+-rw-r--r--   0        0        0    62249 2023-01-27 00:43:42.632110 webint-0.1.9/web/framework/static/vendors-node_modules_monaco-editor_esm_vs_basic-languages_powerquery_powerquery_js.web.js
+-rw-r--r--   0        0        0    38247 2023-01-27 00:43:42.860113 webint-0.1.9/web/framework/static/vendors-node_modules_monaco-editor_esm_vs_basic-languages_protobuf_protobuf_js.web.js
+-rw-r--r--   0        0        0    39348 2023-01-27 00:43:42.764112 webint-0.1.9/web/framework/static/vendors-node_modules_monaco-editor_esm_vs_basic-languages_razor_razor_js.web.js
+-rw-r--r--   0        0        0    48458 2023-01-27 00:43:42.720111 webint-0.1.9/web/framework/static/vendors-node_modules_monaco-editor_esm_vs_basic-languages_redshift_redshift_js.web.js
+-rw-r--r--   0        0        0    36815 2023-01-27 00:43:42.620110 webint-0.1.9/web/framework/static/vendors-node_modules_monaco-editor_esm_vs_basic-languages_ruby_ruby_js.web.js
+-rw-r--r--   0        0        0    30240 2023-01-27 00:43:42.744112 webint-0.1.9/web/framework/static/vendors-node_modules_monaco-editor_esm_vs_basic-languages_scala_scala_js.web.js
+-rw-r--r--   0        0        0    76292 2023-01-27 00:43:42.604110 webint-0.1.9/web/framework/static/vendors-node_modules_monaco-editor_esm_vs_basic-languages_solidity_solidity_js.web.js
+-rw-r--r--   0        0        0    45550 2023-01-27 00:43:42.596110 webint-0.1.9/web/framework/static/vendors-node_modules_monaco-editor_esm_vs_basic-languages_sql_sql_js.web.js
+-rw-r--r--   0        0        0    31355 2023-01-27 00:43:42.540109 webint-0.1.9/web/framework/static/vendors-node_modules_monaco-editor_esm_vs_basic-languages_st_st_js.web.js
+-rw-r--r--   0        0        0    34466 2023-01-27 00:43:42.612110 webint-0.1.9/web/framework/static/vendors-node_modules_monaco-editor_esm_vs_basic-languages_systemverilog_systemverilog_js.web.js
+-rw-r--r--   0        0        0   182429 2023-01-27 00:43:42.724112 webint-0.1.9/web/framework/static/vendors-node_modules_monaco-editor_esm_vs_language_css_cssMode_js.web.js
+-rw-r--r--   0        0        0   185207 2023-01-27 00:43:42.648111 webint-0.1.9/web/framework/static/vendors-node_modules_monaco-editor_esm_vs_language_html_htmlMode_js.web.js
+-rw-r--r--   0        0        0   222617 2023-01-27 00:43:42.744112 webint-0.1.9/web/framework/static/vendors-node_modules_monaco-editor_esm_vs_language_json_jsonMode_js.web.js
+-rw-r--r--   0        0        0   106750 2023-01-27 00:43:42.628110 webint-0.1.9/web/framework/static/vendors-node_modules_monaco-editor_esm_vs_language_typescript_tsMode_js.web.js
+-rw-r--r--   0        0        0      853 2023-01-27 00:43:42.628110 webint-0.1.9/web/framework/static/web.css
+-rw-r--r--   0        0        0    65758 2023-02-14 18:36:48.533111 webint-0.1.9/web/framework/static/web.js
+-rw-r--r--   0        0        0      576 2023-01-27 00:43:42.784112 webint-0.1.9/web/framework/static/web.js.LICENSE.txt
+-rw-r--r--   0        0        0      441 2023-01-27 00:43:42.884114 webint-0.1.9/web/framework/templates/__init__.py
+-rw-r--r--   0        0        0     2123 2023-01-27 00:43:42.880113 webint-0.1.9/web/framework/templates/nginx.conf
+-rw-r--r--   0        0        0     1012 2023-01-27 00:43:42.888114 webint-0.1.9/web/framework/templates/nginx_host.conf
+-rw-r--r--   0        0        0      988 2023-01-27 00:43:42.884114 webint-0.1.9/web/framework/templates/nginx_host_body.conf
+-rw-r--r--   0        0        0      155 2023-01-27 00:43:42.884114 webint-0.1.9/web/framework/templates/nginx_tor_host.conf
+-rw-r--r--   0        0        0      305 2023-01-27 00:43:42.884114 webint-0.1.9/web/framework/templates/redis.conf
+-rw-r--r--   0        0        0     1141 2023-01-27 00:43:42.880113 webint-0.1.9/web/framework/templates/supervisor.conf
+-rw-r--r--   0        0        0     4679 2023-01-27 00:43:42.888114 webint-0.1.9/web/framework/templates/traceback.html
+-rw-r--r--   0        0        0     7283 2023-01-27 00:43:42.536109 webint-0.1.9/web/framework/util.py
+-rw-r--r--   0        0        0     4136 2023-01-27 00:43:42.508109 webint-0.1.9/web/headers/__init__.py
+-rw-r--r--   0        0        0     2343 2023-01-27 00:43:42.512109 webint-0.1.9/web/headers/entity.py
+-rw-r--r--   0        0        0      581 2023-01-27 00:43:42.512109 webint-0.1.9/web/headers/general.py
+-rw-r--r--   0        0        0     8623 2023-01-27 00:43:42.508109 webint-0.1.9/web/headers/request.py
+-rw-r--r--   0        0        0     1150 2023-01-27 00:43:42.512109 webint-0.1.9/web/headers/response.py
+-rw-r--r--   0        0        0      630 2023-01-27 00:43:42.508109 webint-0.1.9/web/headers/util.py
+-rw-r--r--   0        0        0    18262 2023-02-20 21:29:02.794142 webint-0.1.9/web/host/__init__.py
+-rw-r--r--   0        0        0     4474 2023-02-15 02:18:36.929705 webint-0.1.9/web/host/admin/__init__.py
+-rw-r--r--   0        0        0       37 2023-02-15 02:09:57.822778 webint-0.1.9/web/host/admin/templates/__init__.py
+-rw-r--r--   0        0        0      403 2023-02-15 19:17:41.914551 webint-0.1.9/web/host/admin/templates/application.html
+-rw-r--r--   0        0        0      437 2023-02-15 19:20:01.696109 webint-0.1.9/web/host/admin/templates/choose_domain.html
+-rw-r--r--   0        0        0     2394 2023-02-15 20:44:26.037755 webint-0.1.9/web/host/admin/templates/domains.html
+-rw-r--r--   0        0        0      377 2023-02-15 02:17:09.944532 webint-0.1.9/web/host/admin/templates/index.html
+-rw-r--r--   0        0        0      845 2023-02-15 02:23:12.153431 webint-0.1.9/web/host/admin/templates/template.html
+-rw-r--r--   0        0        0     7478 2023-02-12 03:12:55.380982 webint-0.1.9/web/host/providers.py
+-rw-r--r--   0        0        0        0 2023-01-27 00:43:42.504109 webint-0.1.9/web/host/templates/__init__.py
+-rw-r--r--   0        0        0     2714 2023-02-18 22:43:23.224776 webint-0.1.9/web/host/templates/nginx_conf.conf
+-rw-r--r--   0        0        0      653 2023-02-15 06:23:01.293121 webint-0.1.9/web/host/templates/nginx_index.html
+-rw-r--r--   0        0        0     3114 2023-01-27 00:43:42.504109 webint-0.1.9/web/host/templates/nginx_site.conf
+-rw-r--r--   0        0        0      877 2023-01-27 00:43:42.504109 webint-0.1.9/web/host/test_host.py
+-rw-r--r--   0        0        0    42879 2023-01-27 00:43:42.496109 webint-0.1.9/web/markdown/__init__.py
+-rw-r--r--   0        0        0   106063 2023-01-27 00:43:42.496109 webint-0.1.9/web/markdown/hyph_en_US.dic
+-rw-r--r--   0        0        0     8827 2023-01-27 00:43:42.492109 webint-0.1.9/web/markdown/hyphenator.py
+-rw-r--r--   0        0        0     2464 2023-01-27 00:43:42.492109 webint-0.1.9/web/markdown/titlecase.py
+-rw-r--r--   0        0        0     1657 2023-01-27 00:43:42.524109 webint-0.1.9/web/response/__init__.py
+-rw-r--r--   0        0        0     2501 2023-01-27 00:43:42.524109 webint-0.1.9/web/response/clienterror.py
+-rw-r--r--   0        0        0      932 2023-01-27 00:43:42.524109 webint-0.1.9/web/response/informational.py
+-rw-r--r--   0        0        0      901 2023-01-27 00:43:42.520109 webint-0.1.9/web/response/redirection.py
+-rw-r--r--   0        0        0      427 2023-01-27 00:43:42.524109 webint-0.1.9/web/response/servererror.py
+-rw-r--r--   0        0        0     1425 2023-01-27 00:43:42.528109 webint-0.1.9/web/response/success.py
+-rw-r--r--   0        0        0      501 2023-01-27 00:43:42.520109 webint-0.1.9/web/response/util.py
+-rw-r--r--   0        0        0    11900 2023-01-27 00:43:42.532109 webint-0.1.9/web/slrzd.py
+-rw-r--r--   0        0        0     1992 2023-01-27 00:43:42.512109 webint-0.1.9/web/templating/__init__.py
+-rw-r--r--   0        0        0      586 2023-01-27 00:43:42.516109 webint-0.1.9/web/templating/__main__.py
+-rw-r--r--   0        0        0    25383 2023-01-27 00:43:42.516109 webint-0.1.9/web/templating/parse.py
+-rw-r--r--   0        0        0    15402 2023-01-27 00:43:42.512109 webint-0.1.9/web/templating/templating.py
+-rw-r--r--   0        0        0      866 2023-01-27 00:43:42.500109 webint-0.1.9/web/util.py
+-rw-r--r--   0        0        0  4421355 1970-01-01 00:00:00.000000 webint-0.1.9/setup.py
+-rw-r--r--   0        0        0     2084 1970-01-01 00:00:00.000000 webint-0.1.9/PKG-INFO
```

### Comparing `webint-0.1.8/pyproject.toml` & `webint-0.1.9/pyproject.toml`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "webint"
-version = "0.1.8"
+version = "0.1.9"
 description = "an opinionated web framework that stays out of your way"
 readme = "README.md"
 homepage = "https://ragt.ag/code/projects/webint"
 repository = "https://ragt.ag/code/projects/webint.git"
 documentation = "https://ragt.ag/code/projects/webint/api"
 authors = ["Angelo Gladding <angelo@ragt.ag>"]
 license = "BSD-2-Clause"
@@ -14,15 +14,15 @@
 # admin = "web.host.admin:app"
 
 [tool.poetry.scripts]
 web = "web.__main__:main"
 
 [tool.poetry.dependencies]
 python = ">=3.10,<3.11"
-bgq = ">=0.0.5"
+bgq = ">=0.1.2"
 txtint = ">=0.0.68"
 sqlyte = ">=0.0.50"
 easyuri = ">=0.0.12"
 newmath = ">=0.0.3"
 webagt = ">=0.0.5"
 microformats = ">=0.0.24"
 pendulum = "^2.1.2"
```

### Comparing `webint-0.1.8/web/__init__.py` & `webint-0.1.9/web/__init__.py`

 * *Files identical despite different names*

### Comparing `webint-0.1.8/web/__main__.py` & `webint-0.1.9/web/__main__.py`

 * *Files 1% similar despite different names*

```diff
@@ -159,26 +159,30 @@
         #     return 1
 
         machines = config.get("machines", [])
         if len(machines) == 0:
             # XXX console.print("No machines found")
             versions = web.host.Machine.versions
             start_time = time.time()
-            total_time = 13
-            with console.status(f"[bold green]{total_time} min remaining") as status:
+            total_time = 15
+            with console.status(
+                f"[bold green]around {total_time} minutes remaining"
+            ) as status:
 
                 def update_status():
                     while True:
                         remaining_time = total_time - round(
                             (time.time() - start_time) / 60
                         )
                         if remaining_time < 1:
                             status.update("Finishing up..")
                             return
-                        status.update(f"[bold green]{remaining_time} minutes remaining")
+                        status.update(
+                            f"[bold green]around {remaining_time} minutes remaining"
+                        )
                         gevent.sleep(1)
 
                 gevent.spawn(update_status)
 
                 console.print(f"Spawning virtual machine at {host.__class__.__name__}")
                 machine = web.host.spawn_machine("website", host)
                 console.print("Updating system")
```

### Comparing `webint-0.1.8/web/framework/__init__.py` & `webint-0.1.9/web/framework/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -738,15 +738,15 @@
         if mounts:
             self.mount(*mounts)
 
             def set_data_sources(handler, app):
                 # tx.host.kv = kv.db(tx.request.uri.host, ":", {"jobs": "list"})
                 # cache_db = sqlyte.db(f"cache-{tx.request.uri.host}.db", cache.model)
                 # tx.host.cache = cache(db=cache_db)
-                tx.host.db = sqlyte.db(f"site.db", *models)
+                tx.host.db = sqlyte.db("site.db", *models)
                 # tx.host.db = sqlyte.db(f"site-{tx.request.uri.host}.db", *models)
                 yield
 
             self.wrappers.insert(0, resume_session)  # 2nd position
             self.wrappers.insert(0, set_data_sources)  # 1st position
             models = [sessions_model] + [
                 app._model for _, app in self.mounts if getattr(app, "_model", None)
```

### Comparing `webint-0.1.8/web/framework/letsencrypt.py` & `webint-0.1.9/web/framework/letsencrypt.py`

 * *Files identical despite different names*

### Comparing `webint-0.1.8/web/framework/passphrases.json` & `webint-0.1.9/web/framework/passphrases.json`

 * *Files identical despite different names*

### Comparing `webint-0.1.8/web/framework/passphrases.py` & `webint-0.1.9/web/framework/passphrases.py`

 * *Files identical despite different names*

### Comparing `webint-0.1.8/web/framework/static/1133.web.js` & `webint-0.1.9/web/framework/static/1133.web.js`

 * *Files identical despite different names*

### Comparing `webint-0.1.8/web/framework/static/1149.web.js` & `webint-0.1.9/web/framework/static/1149.web.js`

 * *Files identical despite different names*

### Comparing `webint-0.1.8/web/framework/static/1149.web.js.LICENSE.txt` & `webint-0.1.9/web/framework/static/1149.web.js.LICENSE.txt`

 * *Files identical despite different names*

### Comparing `webint-0.1.8/web/framework/static/1182.web.js` & `webint-0.1.9/web/framework/static/1182.web.js`

 * *Files identical despite different names*

### Comparing `webint-0.1.8/web/framework/static/1322.web.js` & `webint-0.1.9/web/framework/static/1322.web.js`

 * *Files identical despite different names*

### Comparing `webint-0.1.8/web/framework/static/195.web.js` & `webint-0.1.9/web/framework/static/195.web.js`

 * *Files identical despite different names*

### Comparing `webint-0.1.8/web/framework/static/2089.web.js` & `webint-0.1.9/web/framework/static/2089.web.js`

 * *Files identical despite different names*

### Comparing `webint-0.1.8/web/framework/static/2137.web.js` & `webint-0.1.9/web/framework/static/2137.web.js`

 * *Files identical despite different names*

### Comparing `webint-0.1.8/web/framework/static/2153.web.js` & `webint-0.1.9/web/framework/static/2153.web.js`

 * *Files identical despite different names*

### Comparing `webint-0.1.8/web/framework/static/2159.web.js` & `webint-0.1.9/web/framework/static/2159.web.js`

 * *Files identical despite different names*

### Comparing `webint-0.1.8/web/framework/static/2280.web.js` & `webint-0.1.9/web/framework/static/2280.web.js`

 * *Files identical despite different names*

### Comparing `webint-0.1.8/web/framework/static/2384.web.js` & `webint-0.1.9/web/framework/static/2384.web.js`

 * *Files identical despite different names*

### Comparing `webint-0.1.8/web/framework/static/2456.web.js` & `webint-0.1.9/web/framework/static/2456.web.js`

 * *Files identical despite different names*

### Comparing `webint-0.1.8/web/framework/static/2489.web.js` & `webint-0.1.9/web/framework/static/2489.web.js`

 * *Files identical despite different names*

### Comparing `webint-0.1.8/web/framework/static/249.web.js` & `webint-0.1.9/web/framework/static/249.web.js`

 * *Files identical despite different names*

### Comparing `webint-0.1.8/web/framework/static/2755.web.js` & `webint-0.1.9/web/framework/static/2755.web.js`

 * *Files identical despite different names*

### Comparing `webint-0.1.8/web/framework/static/2826.web.js` & `webint-0.1.9/web/framework/static/2826.web.js`

 * *Files identical despite different names*

### Comparing `webint-0.1.8/web/framework/static/2919.web.js` & `webint-0.1.9/web/framework/static/2919.web.js`

 * *Files identical despite different names*

### Comparing `webint-0.1.8/web/framework/static/3241.web.js` & `webint-0.1.9/web/framework/static/3241.web.js`

 * *Files identical despite different names*

### Comparing `webint-0.1.8/web/framework/static/3282.web.js` & `webint-0.1.9/web/framework/static/3282.web.js`

 * *Files identical despite different names*

### Comparing `webint-0.1.8/web/framework/static/3339.web.js` & `webint-0.1.9/web/framework/static/3339.web.js`

 * *Files identical despite different names*

### Comparing `webint-0.1.8/web/framework/static/3374.web.js` & `webint-0.1.9/web/framework/static/3374.web.js`

 * *Files identical despite different names*

### Comparing `webint-0.1.8/web/framework/static/3558.web.js` & `webint-0.1.9/web/framework/static/3558.web.js`

 * *Files identical despite different names*

### Comparing `webint-0.1.8/web/framework/static/3559.web.js` & `webint-0.1.9/web/framework/static/3559.web.js`

 * *Files identical despite different names*

### Comparing `webint-0.1.8/web/framework/static/3657.web.js` & `webint-0.1.9/web/framework/static/3657.web.js`

 * *Files identical despite different names*

### Comparing `webint-0.1.8/web/framework/static/3659.web.js` & `webint-0.1.9/web/framework/static/3659.web.js`

 * *Files identical despite different names*

### Comparing `webint-0.1.8/web/framework/static/3684.web.js` & `webint-0.1.9/web/framework/static/3684.web.js`

 * *Files identical despite different names*

### Comparing `webint-0.1.8/web/framework/static/3788.web.js` & `webint-0.1.9/web/framework/static/3788.web.js`

 * *Files identical despite different names*

### Comparing `webint-0.1.8/web/framework/static/3931.web.js` & `webint-0.1.9/web/framework/static/3931.web.js`

 * *Files identical despite different names*

### Comparing `webint-0.1.8/web/framework/static/3998.web.js` & `webint-0.1.9/web/framework/static/3998.web.js`

 * *Files identical despite different names*

### Comparing `webint-0.1.8/web/framework/static/429.web.js` & `webint-0.1.9/web/framework/static/429.web.js`

 * *Files identical despite different names*

### Comparing `webint-0.1.8/web/framework/static/4463.web.js` & `webint-0.1.9/web/framework/static/4463.web.js`

 * *Files identical despite different names*

### Comparing `webint-0.1.8/web/framework/static/4552.web.js` & `webint-0.1.9/web/framework/static/4552.web.js`

 * *Files identical despite different names*

### Comparing `webint-0.1.8/web/framework/static/468.web.js` & `webint-0.1.9/web/framework/static/468.web.js`

 * *Files identical despite different names*

### Comparing `webint-0.1.8/web/framework/static/4776.web.js` & `webint-0.1.9/web/framework/static/4776.web.js`

 * *Files identical despite different names*

### Comparing `webint-0.1.8/web/framework/static/4932.web.js` & `webint-0.1.9/web/framework/static/4932.web.js`

 * *Files identical despite different names*

### Comparing `webint-0.1.8/web/framework/static/501.web.js` & `webint-0.1.9/web/framework/static/501.web.js`

 * *Files identical despite different names*

### Comparing `webint-0.1.8/web/framework/static/5021.web.js` & `webint-0.1.9/web/framework/static/5021.web.js`

 * *Files identical despite different names*

### Comparing `webint-0.1.8/web/framework/static/5289.web.js` & `webint-0.1.9/web/framework/static/5289.web.js`

 * *Files identical despite different names*

### Comparing `webint-0.1.8/web/framework/static/5337.web.js` & `webint-0.1.9/web/framework/static/5337.web.js`

 * *Files identical despite different names*

### Comparing `webint-0.1.8/web/framework/static/5341.web.js` & `webint-0.1.9/web/framework/static/5341.web.js`

 * *Files identical despite different names*

### Comparing `webint-0.1.8/web/framework/static/5466.web.js` & `webint-0.1.9/web/framework/static/5466.web.js`

 * *Files identical despite different names*

### Comparing `webint-0.1.8/web/framework/static/5490.web.js` & `webint-0.1.9/web/framework/static/5490.web.js`

 * *Files identical despite different names*

### Comparing `webint-0.1.8/web/framework/static/5502.web.js` & `webint-0.1.9/web/framework/static/5502.web.js`

 * *Files identical despite different names*

### Comparing `webint-0.1.8/web/framework/static/5528.web.js` & `webint-0.1.9/web/framework/static/5528.web.js`

 * *Files identical despite different names*

### Comparing `webint-0.1.8/web/framework/static/570.web.js` & `webint-0.1.9/web/framework/static/570.web.js`

 * *Files identical despite different names*

### Comparing `webint-0.1.8/web/framework/static/5892.web.js` & `webint-0.1.9/web/framework/static/5892.web.js`

 * *Files identical despite different names*

### Comparing `webint-0.1.8/web/framework/static/5986.web.js` & `webint-0.1.9/web/framework/static/5986.web.js`

 * *Files identical despite different names*

### Comparing `webint-0.1.8/web/framework/static/6259.web.js` & `webint-0.1.9/web/framework/static/6259.web.js`

 * *Files identical despite different names*

### Comparing `webint-0.1.8/web/framework/static/6389.web.js` & `webint-0.1.9/web/framework/static/6389.web.js`

 * *Files identical despite different names*

### Comparing `webint-0.1.8/web/framework/static/6422.web.js` & `webint-0.1.9/web/framework/static/6422.web.js`

 * *Files identical despite different names*

### Comparing `webint-0.1.8/web/framework/static/6425.web.js` & `webint-0.1.9/web/framework/static/6425.web.js`

 * *Files identical despite different names*

### Comparing `webint-0.1.8/web/framework/static/6548.web.js` & `webint-0.1.9/web/framework/static/6548.web.js`

 * *Files identical despite different names*

### Comparing `webint-0.1.8/web/framework/static/6681.web.js` & `webint-0.1.9/web/framework/static/6681.web.js`

 * *Files identical despite different names*

### Comparing `webint-0.1.8/web/framework/static/7050.web.js` & `webint-0.1.9/web/framework/static/7050.web.js`

 * *Files identical despite different names*

### Comparing `webint-0.1.8/web/framework/static/7138.web.js` & `webint-0.1.9/web/framework/static/7138.web.js`

 * *Files identical despite different names*

### Comparing `webint-0.1.8/web/framework/static/7201.web.js` & `webint-0.1.9/web/framework/static/7201.web.js`

 * *Files identical despite different names*

### Comparing `webint-0.1.8/web/framework/static/7318.web.js` & `webint-0.1.9/web/framework/static/7318.web.js`

 * *Files identical despite different names*

### Comparing `webint-0.1.8/web/framework/static/7441.web.js` & `webint-0.1.9/web/framework/static/7441.web.js`

 * *Files identical despite different names*

### Comparing `webint-0.1.8/web/framework/static/7660.web.js` & `webint-0.1.9/web/framework/static/7660.web.js`

 * *Files identical despite different names*

### Comparing `webint-0.1.8/web/framework/static/7730.web.js` & `webint-0.1.9/web/framework/static/7730.web.js`

 * *Files identical despite different names*

### Comparing `webint-0.1.8/web/framework/static/7864.web.js` & `webint-0.1.9/web/framework/static/7864.web.js`

 * *Files identical despite different names*

### Comparing `webint-0.1.8/web/framework/static/788.web.js` & `webint-0.1.9/web/framework/static/788.web.js`

 * *Files identical despite different names*

### Comparing `webint-0.1.8/web/framework/static/8059.web.js` & `webint-0.1.9/web/framework/static/8059.web.js`

 * *Files identical despite different names*

### Comparing `webint-0.1.8/web/framework/static/8106.web.js` & `webint-0.1.9/web/framework/static/8106.web.js`

 * *Files identical despite different names*

### Comparing `webint-0.1.8/web/framework/static/8262.web.js` & `webint-0.1.9/web/framework/static/8262.web.js`

 * *Files identical despite different names*

### Comparing `webint-0.1.8/web/framework/static/8356.web.js` & `webint-0.1.9/web/framework/static/8356.web.js`

 * *Files identical despite different names*

### Comparing `webint-0.1.8/web/framework/static/8416.web.js` & `webint-0.1.9/web/framework/static/8416.web.js`

 * *Files identical despite different names*

### Comparing `webint-0.1.8/web/framework/static/8512.web.js` & `webint-0.1.9/web/framework/static/8512.web.js`

 * *Files identical despite different names*

### Comparing `webint-0.1.8/web/framework/static/8562.web.js` & `webint-0.1.9/web/framework/static/8562.web.js`

 * *Files identical despite different names*

### Comparing `webint-0.1.8/web/framework/static/8670.web.js` & `webint-0.1.9/web/framework/static/8670.web.js`

 * *Files identical despite different names*

### Comparing `webint-0.1.8/web/framework/static/8842.web.js` & `webint-0.1.9/web/framework/static/8842.web.js`

 * *Files identical despite different names*

### Comparing `webint-0.1.8/web/framework/static/888.web.js` & `webint-0.1.9/web/framework/static/888.web.js`

 * *Files identical despite different names*

### Comparing `webint-0.1.8/web/framework/static/8903.web.js` & `webint-0.1.9/web/framework/static/8903.web.js`

 * *Files identical despite different names*

### Comparing `webint-0.1.8/web/framework/static/9338.web.js` & `webint-0.1.9/web/framework/static/9338.web.js`

 * *Files identical despite different names*

### Comparing `webint-0.1.8/web/framework/static/938.web.js` & `webint-0.1.9/web/framework/static/938.web.js`

 * *Files identical despite different names*

### Comparing `webint-0.1.8/web/framework/static/9407.web.js` & `webint-0.1.9/web/framework/static/9407.web.js`

 * *Files identical despite different names*

### Comparing `webint-0.1.8/web/framework/static/9502.web.js` & `webint-0.1.9/web/framework/static/9502.web.js`

 * *Files identical despite different names*

### Comparing `webint-0.1.8/web/framework/static/959.web.js` & `webint-0.1.9/web/framework/static/959.web.js`

 * *Files identical despite different names*

### Comparing `webint-0.1.8/web/framework/static/966.web.js` & `webint-0.1.9/web/framework/static/966.web.js`

 * *Files identical despite different names*

### Comparing `webint-0.1.8/web/framework/static/9721.web.js` & `webint-0.1.9/web/framework/static/9721.web.js`

 * *Files identical despite different names*

### Comparing `webint-0.1.8/web/framework/static/9762.web.js` & `webint-0.1.9/web/framework/static/9762.web.js`

 * *Files identical despite different names*

### Comparing `webint-0.1.8/web/framework/static/9822.web.js` & `webint-0.1.9/web/framework/static/9822.web.js`

 * *Files identical despite different names*

### Comparing `webint-0.1.8/web/framework/static/b797181c93b3755f4fa1.ttf` & `webint-0.1.9/web/framework/static/b797181c93b3755f4fa1.ttf`

 * *Files identical despite different names*

### Comparing `webint-0.1.8/web/framework/static/css.worker.js` & `webint-0.1.9/web/framework/static/css.worker.js`

 * *Files identical despite different names*

### Comparing `webint-0.1.8/web/framework/static/editor.worker.js` & `webint-0.1.9/web/framework/static/editor.worker.js`

 * *Files identical despite different names*

### Comparing `webint-0.1.8/web/framework/static/html.worker.js` & `webint-0.1.9/web/framework/static/html.worker.js`

 * *Files identical despite different names*

### Comparing `webint-0.1.8/web/framework/static/json.worker.js` & `webint-0.1.9/web/framework/static/json.worker.js`

 * *Files identical despite different names*

### Comparing `webint-0.1.8/web/framework/static/measure.png` & `webint-0.1.9/web/framework/static/measure.png`

 * *Files identical despite different names*

### Comparing `webint-0.1.8/web/framework/static/node_modules_monaco-editor_esm_vs_basic-languages_apex_apex_js.web.js` & `webint-0.1.9/web/framework/static/node_modules_monaco-editor_esm_vs_basic-languages_apex_apex_js.web.js`

 * *Files identical despite different names*

### Comparing `webint-0.1.8/web/framework/static/node_modules_monaco-editor_esm_vs_basic-languages_azcli_azcli_js.web.js` & `webint-0.1.9/web/framework/static/node_modules_monaco-editor_esm_vs_basic-languages_azcli_azcli_js.web.js`

 * *Files identical despite different names*

### Comparing `webint-0.1.8/web/framework/static/node_modules_monaco-editor_esm_vs_basic-languages_bat_bat_js.web.js` & `webint-0.1.9/web/framework/static/node_modules_monaco-editor_esm_vs_basic-languages_bat_bat_js.web.js`

 * *Files identical despite different names*

### Comparing `webint-0.1.8/web/framework/static/node_modules_monaco-editor_esm_vs_basic-languages_bicep_bicep_js.web.js` & `webint-0.1.9/web/framework/static/node_modules_monaco-editor_esm_vs_basic-languages_bicep_bicep_js.web.js`

 * *Files identical despite different names*

### Comparing `webint-0.1.8/web/framework/static/node_modules_monaco-editor_esm_vs_basic-languages_cameligo_cameligo_js.web.js` & `webint-0.1.9/web/framework/static/node_modules_monaco-editor_esm_vs_basic-languages_cameligo_cameligo_js.web.js`

 * *Files identical despite different names*

### Comparing `webint-0.1.8/web/framework/static/node_modules_monaco-editor_esm_vs_basic-languages_coffee_coffee_js.web.js` & `webint-0.1.9/web/framework/static/node_modules_monaco-editor_esm_vs_basic-languages_coffee_coffee_js.web.js`

 * *Files identical despite different names*

### Comparing `webint-0.1.8/web/framework/static/node_modules_monaco-editor_esm_vs_basic-languages_cpp_cpp_js.web.js` & `webint-0.1.9/web/framework/static/node_modules_monaco-editor_esm_vs_basic-languages_cpp_cpp_js.web.js`

 * *Files identical despite different names*

### Comparing `webint-0.1.8/web/framework/static/node_modules_monaco-editor_esm_vs_basic-languages_csharp_csharp_js.web.js` & `webint-0.1.9/web/framework/static/node_modules_monaco-editor_esm_vs_basic-languages_csharp_csharp_js.web.js`

 * *Files identical despite different names*

### Comparing `webint-0.1.8/web/framework/static/node_modules_monaco-editor_esm_vs_basic-languages_csp_csp_js.web.js` & `webint-0.1.9/web/framework/static/node_modules_monaco-editor_esm_vs_basic-languages_csp_csp_js.web.js`

 * *Files identical despite different names*

### Comparing `webint-0.1.8/web/framework/static/node_modules_monaco-editor_esm_vs_basic-languages_css_css_js.web.js` & `webint-0.1.9/web/framework/static/node_modules_monaco-editor_esm_vs_basic-languages_css_css_js.web.js`

 * *Files identical despite different names*

### Comparing `webint-0.1.8/web/framework/static/node_modules_monaco-editor_esm_vs_basic-languages_cypher_cypher_js.web.js` & `webint-0.1.9/web/framework/static/node_modules_monaco-editor_esm_vs_basic-languages_cypher_cypher_js.web.js`

 * *Files identical despite different names*

### Comparing `webint-0.1.8/web/framework/static/node_modules_monaco-editor_esm_vs_basic-languages_dart_dart_js.web.js` & `webint-0.1.9/web/framework/static/node_modules_monaco-editor_esm_vs_basic-languages_dart_dart_js.web.js`

 * *Files identical despite different names*

### Comparing `webint-0.1.8/web/framework/static/node_modules_monaco-editor_esm_vs_basic-languages_dockerfile_dockerfile_js.web.js` & `webint-0.1.9/web/framework/static/node_modules_monaco-editor_esm_vs_basic-languages_dockerfile_dockerfile_js.web.js`

 * *Files identical despite different names*

### Comparing `webint-0.1.8/web/framework/static/node_modules_monaco-editor_esm_vs_basic-languages_ecl_ecl_js.web.js` & `webint-0.1.9/web/framework/static/node_modules_monaco-editor_esm_vs_basic-languages_ecl_ecl_js.web.js`

 * *Files identical despite different names*

### Comparing `webint-0.1.8/web/framework/static/node_modules_monaco-editor_esm_vs_basic-languages_flow9_flow9_js.web.js` & `webint-0.1.9/web/framework/static/node_modules_monaco-editor_esm_vs_basic-languages_flow9_flow9_js.web.js`

 * *Files identical despite different names*

### Comparing `webint-0.1.8/web/framework/static/node_modules_monaco-editor_esm_vs_basic-languages_fsharp_fsharp_js.web.js` & `webint-0.1.9/web/framework/static/node_modules_monaco-editor_esm_vs_basic-languages_fsharp_fsharp_js.web.js`

 * *Files identical despite different names*

### Comparing `webint-0.1.8/web/framework/static/node_modules_monaco-editor_esm_vs_basic-languages_go_go_js.web.js` & `webint-0.1.9/web/framework/static/node_modules_monaco-editor_esm_vs_basic-languages_go_go_js.web.js`

 * *Files identical despite different names*

### Comparing `webint-0.1.8/web/framework/static/node_modules_monaco-editor_esm_vs_basic-languages_graphql_graphql_js.web.js` & `webint-0.1.9/web/framework/static/node_modules_monaco-editor_esm_vs_basic-languages_graphql_graphql_js.web.js`

 * *Files identical despite different names*

### Comparing `webint-0.1.8/web/framework/static/node_modules_monaco-editor_esm_vs_basic-languages_hcl_hcl_js.web.js` & `webint-0.1.9/web/framework/static/node_modules_monaco-editor_esm_vs_basic-languages_hcl_hcl_js.web.js`

 * *Files identical despite different names*

### Comparing `webint-0.1.8/web/framework/static/node_modules_monaco-editor_esm_vs_basic-languages_html_html_js.web.js` & `webint-0.1.9/web/framework/static/node_modules_monaco-editor_esm_vs_basic-languages_html_html_js.web.js`

 * *Files identical despite different names*

### Comparing `webint-0.1.8/web/framework/static/node_modules_monaco-editor_esm_vs_basic-languages_ini_ini_js.web.js` & `webint-0.1.9/web/framework/static/node_modules_monaco-editor_esm_vs_basic-languages_ini_ini_js.web.js`

 * *Files identical despite different names*

### Comparing `webint-0.1.8/web/framework/static/node_modules_monaco-editor_esm_vs_basic-languages_java_java_js.web.js` & `webint-0.1.9/web/framework/static/node_modules_monaco-editor_esm_vs_basic-languages_java_java_js.web.js`

 * *Files identical despite different names*

### Comparing `webint-0.1.8/web/framework/static/node_modules_monaco-editor_esm_vs_basic-languages_kotlin_kotlin_js.web.js` & `webint-0.1.9/web/framework/static/node_modules_monaco-editor_esm_vs_basic-languages_kotlin_kotlin_js.web.js`

 * *Files identical despite different names*

### Comparing `webint-0.1.8/web/framework/static/node_modules_monaco-editor_esm_vs_basic-languages_less_less_js.web.js` & `webint-0.1.9/web/framework/static/node_modules_monaco-editor_esm_vs_basic-languages_less_less_js.web.js`

 * *Files identical despite different names*

### Comparing `webint-0.1.8/web/framework/static/node_modules_monaco-editor_esm_vs_basic-languages_lexon_lexon_js.web.js` & `webint-0.1.9/web/framework/static/node_modules_monaco-editor_esm_vs_basic-languages_lexon_lexon_js.web.js`

 * *Files identical despite different names*

### Comparing `webint-0.1.8/web/framework/static/node_modules_monaco-editor_esm_vs_basic-languages_liquid_liquid_js.web.js` & `webint-0.1.9/web/framework/static/node_modules_monaco-editor_esm_vs_basic-languages_liquid_liquid_js.web.js`

 * *Files identical despite different names*

### Comparing `webint-0.1.8/web/framework/static/node_modules_monaco-editor_esm_vs_basic-languages_lua_lua_js.web.js` & `webint-0.1.9/web/framework/static/node_modules_monaco-editor_esm_vs_basic-languages_lua_lua_js.web.js`

 * *Files identical despite different names*

### Comparing `webint-0.1.8/web/framework/static/node_modules_monaco-editor_esm_vs_basic-languages_m3_m3_js.web.js` & `webint-0.1.9/web/framework/static/node_modules_monaco-editor_esm_vs_basic-languages_m3_m3_js.web.js`

 * *Files identical despite different names*

### Comparing `webint-0.1.8/web/framework/static/node_modules_monaco-editor_esm_vs_basic-languages_markdown_markdown_js.web.js` & `webint-0.1.9/web/framework/static/node_modules_monaco-editor_esm_vs_basic-languages_markdown_markdown_js.web.js`

 * *Files identical despite different names*

### Comparing `webint-0.1.8/web/framework/static/node_modules_monaco-editor_esm_vs_basic-languages_mips_mips_js.web.js` & `webint-0.1.9/web/framework/static/node_modules_monaco-editor_esm_vs_basic-languages_mips_mips_js.web.js`

 * *Files identical despite different names*

### Comparing `webint-0.1.8/web/framework/static/node_modules_monaco-editor_esm_vs_basic-languages_msdax_msdax_js.web.js` & `webint-0.1.9/web/framework/static/node_modules_monaco-editor_esm_vs_basic-languages_msdax_msdax_js.web.js`

 * *Files identical despite different names*

### Comparing `webint-0.1.8/web/framework/static/node_modules_monaco-editor_esm_vs_basic-languages_objective-c_objective-c_js.web.js` & `webint-0.1.9/web/framework/static/node_modules_monaco-editor_esm_vs_basic-languages_objective-c_objective-c_js.web.js`

 * *Files identical despite different names*

### Comparing `webint-0.1.8/web/framework/static/node_modules_monaco-editor_esm_vs_basic-languages_pascal_pascal_js.web.js` & `webint-0.1.9/web/framework/static/node_modules_monaco-editor_esm_vs_basic-languages_pascal_pascal_js.web.js`

 * *Files identical despite different names*

### Comparing `webint-0.1.8/web/framework/static/node_modules_monaco-editor_esm_vs_basic-languages_pascaligo_pascaligo_js.web.js` & `webint-0.1.9/web/framework/static/node_modules_monaco-editor_esm_vs_basic-languages_pascaligo_pascaligo_js.web.js`

 * *Files identical despite different names*

### Comparing `webint-0.1.8/web/framework/static/node_modules_monaco-editor_esm_vs_basic-languages_pla_pla_js.web.js` & `webint-0.1.9/web/framework/static/node_modules_monaco-editor_esm_vs_basic-languages_pla_pla_js.web.js`

 * *Files identical despite different names*

### Comparing `webint-0.1.8/web/framework/static/node_modules_monaco-editor_esm_vs_basic-languages_powershell_powershell_js.web.js` & `webint-0.1.9/web/framework/static/node_modules_monaco-editor_esm_vs_basic-languages_powershell_powershell_js.web.js`

 * *Files identical despite different names*

### Comparing `webint-0.1.8/web/framework/static/node_modules_monaco-editor_esm_vs_basic-languages_pug_pug_js.web.js` & `webint-0.1.9/web/framework/static/node_modules_monaco-editor_esm_vs_basic-languages_pug_pug_js.web.js`

 * *Files identical despite different names*

### Comparing `webint-0.1.8/web/framework/static/node_modules_monaco-editor_esm_vs_basic-languages_python_python_js.web.js` & `webint-0.1.9/web/framework/static/node_modules_monaco-editor_esm_vs_basic-languages_python_python_js.web.js`

 * *Files identical despite different names*

### Comparing `webint-0.1.8/web/framework/static/node_modules_monaco-editor_esm_vs_basic-languages_qsharp_qsharp_js.web.js` & `webint-0.1.9/web/framework/static/node_modules_monaco-editor_esm_vs_basic-languages_qsharp_qsharp_js.web.js`

 * *Files identical despite different names*

### Comparing `webint-0.1.8/web/framework/static/node_modules_monaco-editor_esm_vs_basic-languages_r_r_js.web.js` & `webint-0.1.9/web/framework/static/node_modules_monaco-editor_esm_vs_basic-languages_r_r_js.web.js`

 * *Files identical despite different names*

### Comparing `webint-0.1.8/web/framework/static/node_modules_monaco-editor_esm_vs_basic-languages_redis_redis_js.web.js` & `webint-0.1.9/web/framework/static/node_modules_monaco-editor_esm_vs_basic-languages_redis_redis_js.web.js`

 * *Files identical despite different names*

### Comparing `webint-0.1.8/web/framework/static/node_modules_monaco-editor_esm_vs_basic-languages_restructuredtext_restructuredtext_js.web.js` & `webint-0.1.9/web/framework/static/node_modules_monaco-editor_esm_vs_basic-languages_restructuredtext_restructuredtext_js.web.js`

 * *Files identical despite different names*

### Comparing `webint-0.1.8/web/framework/static/node_modules_monaco-editor_esm_vs_basic-languages_rust_rust_js.web.js` & `webint-0.1.9/web/framework/static/node_modules_monaco-editor_esm_vs_basic-languages_rust_rust_js.web.js`

 * *Files identical despite different names*

### Comparing `webint-0.1.8/web/framework/static/node_modules_monaco-editor_esm_vs_basic-languages_sb_sb_js.web.js` & `webint-0.1.9/web/framework/static/node_modules_monaco-editor_esm_vs_basic-languages_sb_sb_js.web.js`

 * *Files identical despite different names*

### Comparing `webint-0.1.8/web/framework/static/node_modules_monaco-editor_esm_vs_basic-languages_scheme_scheme_js.web.js` & `webint-0.1.9/web/framework/static/node_modules_monaco-editor_esm_vs_basic-languages_scheme_scheme_js.web.js`

 * *Files identical despite different names*

### Comparing `webint-0.1.8/web/framework/static/node_modules_monaco-editor_esm_vs_basic-languages_scss_scss_js.web.js` & `webint-0.1.9/web/framework/static/node_modules_monaco-editor_esm_vs_basic-languages_scss_scss_js.web.js`

 * *Files identical despite different names*

### Comparing `webint-0.1.8/web/framework/static/node_modules_monaco-editor_esm_vs_basic-languages_shell_shell_js.web.js` & `webint-0.1.9/web/framework/static/node_modules_monaco-editor_esm_vs_basic-languages_shell_shell_js.web.js`

 * *Files identical despite different names*

### Comparing `webint-0.1.8/web/framework/static/node_modules_monaco-editor_esm_vs_basic-languages_sophia_sophia_js.web.js` & `webint-0.1.9/web/framework/static/node_modules_monaco-editor_esm_vs_basic-languages_sophia_sophia_js.web.js`

 * *Files identical despite different names*

### Comparing `webint-0.1.8/web/framework/static/node_modules_monaco-editor_esm_vs_basic-languages_sparql_sparql_js.web.js` & `webint-0.1.9/web/framework/static/node_modules_monaco-editor_esm_vs_basic-languages_sparql_sparql_js.web.js`

 * *Files identical despite different names*

### Comparing `webint-0.1.8/web/framework/static/node_modules_monaco-editor_esm_vs_basic-languages_swift_swift_js.web.js` & `webint-0.1.9/web/framework/static/node_modules_monaco-editor_esm_vs_basic-languages_swift_swift_js.web.js`

 * *Files identical despite different names*

### Comparing `webint-0.1.8/web/framework/static/node_modules_monaco-editor_esm_vs_basic-languages_tcl_tcl_js.web.js` & `webint-0.1.9/web/framework/static/node_modules_monaco-editor_esm_vs_basic-languages_tcl_tcl_js.web.js`

 * *Files identical despite different names*

### Comparing `webint-0.1.8/web/framework/static/node_modules_monaco-editor_esm_vs_basic-languages_twig_twig_js.web.js` & `webint-0.1.9/web/framework/static/node_modules_monaco-editor_esm_vs_basic-languages_twig_twig_js.web.js`

 * *Files identical despite different names*

### Comparing `webint-0.1.8/web/framework/static/node_modules_monaco-editor_esm_vs_basic-languages_typescript_typescript_js.web.js` & `webint-0.1.9/web/framework/static/node_modules_monaco-editor_esm_vs_basic-languages_typescript_typescript_js.web.js`

 * *Files identical despite different names*

### Comparing `webint-0.1.8/web/framework/static/node_modules_monaco-editor_esm_vs_basic-languages_vb_vb_js.web.js` & `webint-0.1.9/web/framework/static/node_modules_monaco-editor_esm_vs_basic-languages_vb_vb_js.web.js`

 * *Files identical despite different names*

### Comparing `webint-0.1.8/web/framework/static/node_modules_monaco-editor_esm_vs_basic-languages_xml_xml_js.web.js` & `webint-0.1.9/web/framework/static/node_modules_monaco-editor_esm_vs_basic-languages_xml_xml_js.web.js`

 * *Files identical despite different names*

### Comparing `webint-0.1.8/web/framework/static/node_modules_monaco-editor_esm_vs_basic-languages_yaml_yaml_js.web.js` & `webint-0.1.9/web/framework/static/node_modules_monaco-editor_esm_vs_basic-languages_yaml_yaml_js.web.js`

 * *Files identical despite different names*

### Comparing `webint-0.1.8/web/framework/static/solarized-site.css` & `webint-0.1.9/web/framework/static/solarized-site.css`

 * *Files identical despite different names*

### Comparing `webint-0.1.8/web/framework/static/solarized.css` & `webint-0.1.9/web/framework/static/solarized.css`

 * *Files identical despite different names*

### Comparing `webint-0.1.8/web/framework/static/ts.worker.js` & `webint-0.1.9/web/framework/static/ts.worker.js`

 * *Files identical despite different names*

### Comparing `webint-0.1.8/web/framework/static/ts.worker.js.LICENSE.txt` & `webint-0.1.9/web/framework/static/ts.worker.js.LICENSE.txt`

 * *Files identical despite different names*

### Comparing `webint-0.1.8/web/framework/static/vendors-node_modules_monaco-editor_esm_vs_basic-languages_abap_abap_js.web.js` & `webint-0.1.9/web/framework/static/vendors-node_modules_monaco-editor_esm_vs_basic-languages_abap_abap_js.web.js`

 * *Files identical despite different names*

### Comparing `webint-0.1.8/web/framework/static/vendors-node_modules_monaco-editor_esm_vs_basic-languages_clojure_clojure_js.web.js` & `webint-0.1.9/web/framework/static/vendors-node_modules_monaco-editor_esm_vs_basic-languages_clojure_clojure_js.web.js`

 * *Files identical despite different names*

### Comparing `webint-0.1.8/web/framework/static/vendors-node_modules_monaco-editor_esm_vs_basic-languages_elixir_elixir_js.web.js` & `webint-0.1.9/web/framework/static/vendors-node_modules_monaco-editor_esm_vs_basic-languages_elixir_elixir_js.web.js`

 * *Files identical despite different names*

### Comparing `webint-0.1.8/web/framework/static/vendors-node_modules_monaco-editor_esm_vs_basic-languages_freemarker2_freemarker2_js.web.js` & `webint-0.1.9/web/framework/static/vendors-node_modules_monaco-editor_esm_vs_basic-languages_freemarker2_freemarker2_js.web.js`

 * *Files identical despite different names*

### Comparing `webint-0.1.8/web/framework/static/vendors-node_modules_monaco-editor_esm_vs_basic-languages_handlebars_handlebars_js.web.js` & `webint-0.1.9/web/framework/static/vendors-node_modules_monaco-editor_esm_vs_basic-languages_handlebars_handlebars_js.web.js`

 * *Files identical despite different names*

### Comparing `webint-0.1.8/web/framework/static/vendors-node_modules_monaco-editor_esm_vs_basic-languages_javascript_javascript_js.web.js` & `webint-0.1.9/web/framework/static/vendors-node_modules_monaco-editor_esm_vs_basic-languages_javascript_javascript_js.web.js`

 * *Files identical despite different names*

### Comparing `webint-0.1.8/web/framework/static/vendors-node_modules_monaco-editor_esm_vs_basic-languages_julia_julia_js.web.js` & `webint-0.1.9/web/framework/static/vendors-node_modules_monaco-editor_esm_vs_basic-languages_julia_julia_js.web.js`

 * *Files identical despite different names*

### Comparing `webint-0.1.8/web/framework/static/vendors-node_modules_monaco-editor_esm_vs_basic-languages_mysql_mysql_js.web.js` & `webint-0.1.9/web/framework/static/vendors-node_modules_monaco-editor_esm_vs_basic-languages_mysql_mysql_js.web.js`

 * *Files identical despite different names*

### Comparing `webint-0.1.8/web/framework/static/vendors-node_modules_monaco-editor_esm_vs_basic-languages_perl_perl_js.web.js` & `webint-0.1.9/web/framework/static/vendors-node_modules_monaco-editor_esm_vs_basic-languages_perl_perl_js.web.js`

 * *Files identical despite different names*

### Comparing `webint-0.1.8/web/framework/static/vendors-node_modules_monaco-editor_esm_vs_basic-languages_pgsql_pgsql_js.web.js` & `webint-0.1.9/web/framework/static/vendors-node_modules_monaco-editor_esm_vs_basic-languages_pgsql_pgsql_js.web.js`

 * *Files identical despite different names*

### Comparing `webint-0.1.8/web/framework/static/vendors-node_modules_monaco-editor_esm_vs_basic-languages_php_php_js.web.js` & `webint-0.1.9/web/framework/static/vendors-node_modules_monaco-editor_esm_vs_basic-languages_php_php_js.web.js`

 * *Files identical despite different names*

### Comparing `webint-0.1.8/web/framework/static/vendors-node_modules_monaco-editor_esm_vs_basic-languages_postiats_postiats_js.web.js` & `webint-0.1.9/web/framework/static/vendors-node_modules_monaco-editor_esm_vs_basic-languages_postiats_postiats_js.web.js`

 * *Files identical despite different names*

### Comparing `webint-0.1.8/web/framework/static/vendors-node_modules_monaco-editor_esm_vs_basic-languages_powerquery_powerquery_js.web.js` & `webint-0.1.9/web/framework/static/vendors-node_modules_monaco-editor_esm_vs_basic-languages_powerquery_powerquery_js.web.js`

 * *Files identical despite different names*

### Comparing `webint-0.1.8/web/framework/static/vendors-node_modules_monaco-editor_esm_vs_basic-languages_protobuf_protobuf_js.web.js` & `webint-0.1.9/web/framework/static/vendors-node_modules_monaco-editor_esm_vs_basic-languages_protobuf_protobuf_js.web.js`

 * *Files identical despite different names*

### Comparing `webint-0.1.8/web/framework/static/vendors-node_modules_monaco-editor_esm_vs_basic-languages_razor_razor_js.web.js` & `webint-0.1.9/web/framework/static/vendors-node_modules_monaco-editor_esm_vs_basic-languages_razor_razor_js.web.js`

 * *Files identical despite different names*

### Comparing `webint-0.1.8/web/framework/static/vendors-node_modules_monaco-editor_esm_vs_basic-languages_redshift_redshift_js.web.js` & `webint-0.1.9/web/framework/static/vendors-node_modules_monaco-editor_esm_vs_basic-languages_redshift_redshift_js.web.js`

 * *Files identical despite different names*

### Comparing `webint-0.1.8/web/framework/static/vendors-node_modules_monaco-editor_esm_vs_basic-languages_ruby_ruby_js.web.js` & `webint-0.1.9/web/framework/static/vendors-node_modules_monaco-editor_esm_vs_basic-languages_ruby_ruby_js.web.js`

 * *Files identical despite different names*

### Comparing `webint-0.1.8/web/framework/static/vendors-node_modules_monaco-editor_esm_vs_basic-languages_scala_scala_js.web.js` & `webint-0.1.9/web/framework/static/vendors-node_modules_monaco-editor_esm_vs_basic-languages_scala_scala_js.web.js`

 * *Files identical despite different names*

### Comparing `webint-0.1.8/web/framework/static/vendors-node_modules_monaco-editor_esm_vs_basic-languages_solidity_solidity_js.web.js` & `webint-0.1.9/web/framework/static/vendors-node_modules_monaco-editor_esm_vs_basic-languages_solidity_solidity_js.web.js`

 * *Files identical despite different names*

### Comparing `webint-0.1.8/web/framework/static/vendors-node_modules_monaco-editor_esm_vs_basic-languages_sql_sql_js.web.js` & `webint-0.1.9/web/framework/static/vendors-node_modules_monaco-editor_esm_vs_basic-languages_sql_sql_js.web.js`

 * *Files identical despite different names*

### Comparing `webint-0.1.8/web/framework/static/vendors-node_modules_monaco-editor_esm_vs_basic-languages_st_st_js.web.js` & `webint-0.1.9/web/framework/static/vendors-node_modules_monaco-editor_esm_vs_basic-languages_st_st_js.web.js`

 * *Files identical despite different names*

### Comparing `webint-0.1.8/web/framework/static/vendors-node_modules_monaco-editor_esm_vs_basic-languages_systemverilog_systemverilog_js.web.js` & `webint-0.1.9/web/framework/static/vendors-node_modules_monaco-editor_esm_vs_basic-languages_systemverilog_systemverilog_js.web.js`

 * *Files identical despite different names*

### Comparing `webint-0.1.8/web/framework/static/vendors-node_modules_monaco-editor_esm_vs_language_css_cssMode_js.web.js` & `webint-0.1.9/web/framework/static/vendors-node_modules_monaco-editor_esm_vs_language_css_cssMode_js.web.js`

 * *Files identical despite different names*

### Comparing `webint-0.1.8/web/framework/static/vendors-node_modules_monaco-editor_esm_vs_language_html_htmlMode_js.web.js` & `webint-0.1.9/web/framework/static/vendors-node_modules_monaco-editor_esm_vs_language_html_htmlMode_js.web.js`

 * *Files identical despite different names*

### Comparing `webint-0.1.8/web/framework/static/vendors-node_modules_monaco-editor_esm_vs_language_json_jsonMode_js.web.js` & `webint-0.1.9/web/framework/static/vendors-node_modules_monaco-editor_esm_vs_language_json_jsonMode_js.web.js`

 * *Files identical despite different names*

### Comparing `webint-0.1.8/web/framework/static/vendors-node_modules_monaco-editor_esm_vs_language_typescript_tsMode_js.web.js` & `webint-0.1.9/web/framework/static/vendors-node_modules_monaco-editor_esm_vs_language_typescript_tsMode_js.web.js`

 * *Files identical despite different names*

### Comparing `webint-0.1.8/web/framework/static/web.css` & `webint-0.1.9/web/framework/static/web.css`

 * *Files identical despite different names*

### Comparing `webint-0.1.8/web/framework/static/web.js` & `webint-0.1.9/web/framework/static/web.js`

 * *Files identical despite different names*

### Comparing `webint-0.1.8/web/framework/static/web.js.LICENSE.txt` & `webint-0.1.9/web/framework/static/web.js.LICENSE.txt`

 * *Files identical despite different names*

### Comparing `webint-0.1.8/web/framework/templates/nginx.conf` & `webint-0.1.9/web/framework/templates/nginx.conf`

 * *Files identical despite different names*

### Comparing `webint-0.1.8/web/framework/templates/nginx_host.conf` & `webint-0.1.9/web/framework/templates/nginx_host.conf`

 * *Files identical despite different names*

### Comparing `webint-0.1.8/web/framework/templates/nginx_host_body.conf` & `webint-0.1.9/web/framework/templates/nginx_host_body.conf`

 * *Files identical despite different names*

### Comparing `webint-0.1.8/web/framework/templates/supervisor.conf` & `webint-0.1.9/web/framework/templates/supervisor.conf`

 * *Files identical despite different names*

### Comparing `webint-0.1.8/web/framework/templates/traceback.html` & `webint-0.1.9/web/framework/templates/traceback.html`

 * *Files identical despite different names*

### Comparing `webint-0.1.8/web/framework/util.py` & `webint-0.1.9/web/framework/util.py`

 * *Files identical despite different names*

### Comparing `webint-0.1.8/web/headers/__init__.py` & `webint-0.1.9/web/headers/__init__.py`

 * *Files identical despite different names*

### Comparing `webint-0.1.8/web/headers/entity.py` & `webint-0.1.9/web/headers/entity.py`

 * *Files identical despite different names*

### Comparing `webint-0.1.8/web/headers/general.py` & `webint-0.1.9/web/headers/general.py`

 * *Files identical despite different names*

### Comparing `webint-0.1.8/web/headers/request.py` & `webint-0.1.9/web/headers/request.py`

 * *Files identical despite different names*

### Comparing `webint-0.1.8/web/headers/response.py` & `webint-0.1.9/web/headers/response.py`

 * *Files identical despite different names*

### Comparing `webint-0.1.8/web/headers/util.py` & `webint-0.1.9/web/headers/util.py`

 * *Files identical despite different names*

### Comparing `webint-0.1.8/web/host/__init__.py` & `webint-0.1.9/web/host/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -437,14 +437,21 @@
                     f"{self.runinenv} {env_dir} gunicorn {package}:app "
                     f"-k gevent -w 2 --bind unix:{run_dir}/gunicorn.sock"
                 ),
                 "directory": run_dir,
                 "stopsignal": "INT",
                 "user": "gaea",
             }
+            config["program:queue"] = {
+                "autostart": "true",
+                "command": f"{self.runinenv} {env_dir} bgq run",
+                "directory": run_dir,
+                "stopsignal": "INT",
+                "user": "gaea",
+            }
 
     # def install_project(self, registrar, project_root=Path(".")):
     #     """Install sites from project in `project_root`."""
     #     # TODO install from Git URL
     #     with (project_root / "pyproject.toml").open() as fp:
     #         project = toml.load(fp)["tool"]["poetry"]
     #     try:
```

### Comparing `webint-0.1.8/web/host/admin/__init__.py` & `webint-0.1.9/web/host/admin/__init__.py`

 * *Files identical despite different names*

### Comparing `webint-0.1.8/web/host/admin/templates/domains.html` & `webint-0.1.9/web/host/admin/templates/domains.html`

 * *Files identical despite different names*

### Comparing `webint-0.1.8/web/host/admin/templates/template.html` & `webint-0.1.9/web/host/admin/templates/template.html`

 * *Files identical despite different names*

### Comparing `webint-0.1.8/web/host/providers.py` & `webint-0.1.9/web/host/providers.py`

 * *Files identical despite different names*

### Comparing `webint-0.1.8/web/host/templates/nginx_conf.conf` & `webint-0.1.9/web/host/templates/nginx_conf.conf`

 * *Files identical despite different names*

### Comparing `webint-0.1.8/web/host/templates/nginx_index.html` & `webint-0.1.9/web/host/templates/nginx_index.html`

 * *Files identical despite different names*

### Comparing `webint-0.1.8/web/host/templates/nginx_site.conf` & `webint-0.1.9/web/host/templates/nginx_site.conf`

 * *Files identical despite different names*

### Comparing `webint-0.1.8/web/host/test_host.py` & `webint-0.1.9/web/host/test_host.py`

 * *Files identical despite different names*

### Comparing `webint-0.1.8/web/markdown/__init__.py` & `webint-0.1.9/web/markdown/__init__.py`

 * *Files identical despite different names*

### Comparing `webint-0.1.8/web/markdown/hyph_en_US.dic` & `webint-0.1.9/web/markdown/hyph_en_US.dic`

 * *Files identical despite different names*

### Comparing `webint-0.1.8/web/markdown/hyphenator.py` & `webint-0.1.9/web/markdown/hyphenator.py`

 * *Files identical despite different names*

### Comparing `webint-0.1.8/web/markdown/titlecase.py` & `webint-0.1.9/web/markdown/titlecase.py`

 * *Files identical despite different names*

### Comparing `webint-0.1.8/web/response/__init__.py` & `webint-0.1.9/web/response/__init__.py`

 * *Files identical despite different names*

### Comparing `webint-0.1.8/web/response/clienterror.py` & `webint-0.1.9/web/response/clienterror.py`

 * *Files identical despite different names*

### Comparing `webint-0.1.8/web/response/informational.py` & `webint-0.1.9/web/response/informational.py`

 * *Files identical despite different names*

### Comparing `webint-0.1.8/web/response/redirection.py` & `webint-0.1.9/web/response/redirection.py`

 * *Files identical despite different names*

### Comparing `webint-0.1.8/web/response/success.py` & `webint-0.1.9/web/response/success.py`

 * *Files identical despite different names*

### Comparing `webint-0.1.8/web/slrzd.py` & `webint-0.1.9/web/slrzd.py`

 * *Files identical despite different names*

### Comparing `webint-0.1.8/web/templating/__init__.py` & `webint-0.1.9/web/templating/__init__.py`

 * *Files identical despite different names*

### Comparing `webint-0.1.8/web/templating/__main__.py` & `webint-0.1.9/web/templating/__main__.py`

 * *Files identical despite different names*

### Comparing `webint-0.1.8/web/templating/parse.py` & `webint-0.1.9/web/templating/parse.py`

 * *Files identical despite different names*

### Comparing `webint-0.1.8/web/templating/templating.py` & `webint-0.1.9/web/templating/templating.py`

 * *Files identical despite different names*

### Comparing `webint-0.1.8/web/util.py` & `webint-0.1.9/web/util.py`

 * *Files identical despite different names*

### Comparing `webint-0.1.8/setup.py` & `webint-0.1.9/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -68139,15 +68139,15 @@
                    'static/web.js.LICENSE.txt']}
 
 install_requires = \
 ['PySide6>=6.4.2,<7.0.0',
  'Pygments>=2.14.0,<3.0.0',
  'Unidecode>=1.3.6,<2.0.0',
  'acme-tiny>=5.0.1,<6.0.0',
- 'bgq>=0.0.5',
+ 'bgq>=0.1.2',
  'dnspython>=2.3.0,<3.0.0',
  'easyuri>=0.0.12',
  'emoji>=2.2.0,<3.0.0',
  'gevent>=22.10.2,<23.0.0',
  'gunicorn>=20.1.0,<21.0.0',
  'jsonpatch>=1.32,<2.0',
  'microformats>=0.0.24',
@@ -68167,15 +68167,15 @@
  'webagt>=0.0.5']
 
 entry_points = \
 {'console_scripts': ['web = web.__main__:main']}
 
 setup_kwargs = {
     'name': 'webint',
-    'version': '0.1.8',
+    'version': '0.1.9',
     'description': 'an opinionated web framework that stays out of your way',
     'long_description': '## How to use\n\n### Initialize a project\n\n    poetry init\n\n### Install webint\n\n    poetry add webint\n\n### Create your website\n\n    poetry run web scaffold\n\n### Run your website\n\n    poetry run web run 9999\n\n### Open your website\n\n    open http://localhost:9999\n\n### Modify your website\n\n    ...\n\n### Deploy your website\n\n#### On a cloud server only\n\n#### On a home server through a cloud server (for TLS termination)\n\n#### On a home server only (via tor)\n',
     'author': 'Angelo Gladding',
     'author_email': 'angelo@ragt.ag',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://ragt.ag/code/projects/webint',
```

### Comparing `webint-0.1.8/PKG-INFO` & `webint-0.1.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 Metadata-Version: 2.1
 Name: webint
-Version: 0.1.8
+Version: 0.1.9
 Summary: an opinionated web framework that stays out of your way
 Home-page: https://ragt.ag/code/projects/webint
 License: BSD-2-Clause
 Author: Angelo Gladding
 Author-email: angelo@ragt.ag
 Requires-Python: >=3.10,<3.11
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Requires-Dist: PySide6 (>=6.4.2,<7.0.0)
 Requires-Dist: Pygments (>=2.14.0,<3.0.0)
 Requires-Dist: Unidecode (>=1.3.6,<2.0.0)
 Requires-Dist: acme-tiny (>=5.0.1,<6.0.0)
-Requires-Dist: bgq (>=0.0.5)
+Requires-Dist: bgq (>=0.1.2)
 Requires-Dist: dnspython (>=2.3.0,<3.0.0)
 Requires-Dist: easyuri (>=0.0.12)
 Requires-Dist: emoji (>=2.2.0,<3.0.0)
 Requires-Dist: gevent (>=22.10.2,<23.0.0)
 Requires-Dist: gunicorn (>=20.1.0,<21.0.0)
 Requires-Dist: jsonpatch (>=1.32,<2.0)
 Requires-Dist: microformats (>=0.0.24)
```

