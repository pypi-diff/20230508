# Comparing `tmp/adafruit-circuitpython-bluefruitconnect-1.2.8.tar.gz` & `tmp/adafruit-circuitpython-bluefruitconnect-1.2.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "adafruit-circuitpython-bluefruitconnect-1.2.8.tar", last modified: Wed Feb  8 17:39:25 2023, max compression
+gzip compressed data, was "adafruit-circuitpython-bluefruitconnect-1.2.9.tar", last modified: Mon May  8 16:20:59 2023, max compression
```

## Comparing `adafruit-circuitpython-bluefruitconnect-1.2.8.tar` & `adafruit-circuitpython-bluefruitconnect-1.2.9.tar`

### file list

```diff
@@ -1,62 +1,62 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-08 17:39:25.559511 adafruit-circuitpython-bluefruitconnect-1.2.8/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-08 17:39:25.551511 adafruit-circuitpython-bluefruitconnect-1.2.8/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-08 17:39:25.555511 adafruit-circuitpython-bluefruitconnect-1.2.8/.github/PULL_REQUEST_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (123)      880 2023-02-08 17:39:02.000000 adafruit-circuitpython-bluefruitconnect-1.2.8/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-08 17:39:25.555511 adafruit-circuitpython-bluefruitconnect-1.2.8/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      303 2023-02-08 17:39:02.000000 adafruit-circuitpython-bluefruitconnect-1.2.8/.github/workflows/build.yml
--rw-r--r--   0 runner    (1001) docker     (123)      479 2023-02-08 17:39:02.000000 adafruit-circuitpython-bluefruitconnect-1.2.8/.github/workflows/failure-help-text.yml
--rw-r--r--   0 runner    (1001) docker     (123)      482 2023-02-08 17:39:02.000000 adafruit-circuitpython-bluefruitconnect-1.2.8/.github/workflows/release_gh.yml
--rw-r--r--   0 runner    (1001) docker     (123)      475 2023-02-08 17:39:02.000000 adafruit-circuitpython-bluefruitconnect-1.2.8/.github/workflows/release_pypi.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1654 2023-02-08 17:39:02.000000 adafruit-circuitpython-bluefruitconnect-1.2.8/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     1239 2023-02-08 17:39:02.000000 adafruit-circuitpython-bluefruitconnect-1.2.8/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)    13069 2023-02-08 17:39:02.000000 adafruit-circuitpython-bluefruitconnect-1.2.8/.pylintrc
--rw-r--r--   0 runner    (1001) docker     (123)      388 2023-02-08 17:39:02.000000 adafruit-circuitpython-bluefruitconnect-1.2.8/.readthedocs.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     6147 2023-02-08 17:39:02.000000 adafruit-circuitpython-bluefruitconnect-1.2.8/CODE_OF_CONDUCT.md
--rw-r--r--   0 runner    (1001) docker     (123)     1102 2023-02-08 17:39:02.000000 adafruit-circuitpython-bluefruitconnect-1.2.8/LICENSE
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-08 17:39:25.555511 adafruit-circuitpython-bluefruitconnect-1.2.8/LICENSES/
--rw-r--r--   0 runner    (1001) docker     (123)    16814 2023-02-08 17:39:02.000000 adafruit-circuitpython-bluefruitconnect-1.2.8/LICENSES/CC-BY-4.0.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1108 2023-02-08 17:39:02.000000 adafruit-circuitpython-bluefruitconnect-1.2.8/LICENSES/MIT.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1211 2023-02-08 17:39:02.000000 adafruit-circuitpython-bluefruitconnect-1.2.8/LICENSES/Unlicense.txt
--rw-r--r--   0 runner    (1001) docker     (123)     3970 2023-02-08 17:39:25.559511 adafruit-circuitpython-bluefruitconnect-1.2.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3185 2023-02-08 17:39:02.000000 adafruit-circuitpython-bluefruitconnect-1.2.8/README.rst
--rw-r--r--   0 runner    (1001) docker     (123)      108 2023-02-08 17:39:02.000000 adafruit-circuitpython-bluefruitconnect-1.2.8/README.rst.license
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-08 17:39:25.555511 adafruit-circuitpython-bluefruitconnect-1.2.8/adafruit_bluefruit_connect/
--rw-r--r--   0 runner    (1001) docker     (123)      584 2023-02-08 17:39:17.000000 adafruit-circuitpython-bluefruitconnect-1.2.8/adafruit_bluefruit_connect/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1447 2023-02-08 17:39:17.000000 adafruit-circuitpython-bluefruitconnect-1.2.8/adafruit_bluefruit_connect/_xyz_packet.py
--rw-r--r--   0 runner    (1001) docker     (123)      671 2023-02-08 17:39:17.000000 adafruit-circuitpython-bluefruitconnect-1.2.8/adafruit_bluefruit_connect/accelerometer_packet.py
--rw-r--r--   0 runner    (1001) docker     (123)     3003 2023-02-08 17:39:17.000000 adafruit-circuitpython-bluefruitconnect-1.2.8/adafruit_bluefruit_connect/button_packet.py
--rw-r--r--   0 runner    (1001) docker     (123)     2101 2023-02-08 17:39:17.000000 adafruit-circuitpython-bluefruitconnect-1.2.8/adafruit_bluefruit_connect/color_packet.py
--rw-r--r--   0 runner    (1001) docker     (123)      630 2023-02-08 17:39:17.000000 adafruit-circuitpython-bluefruitconnect-1.2.8/adafruit_bluefruit_connect/gyro_packet.py
--rw-r--r--   0 runner    (1001) docker     (123)     1647 2023-02-08 17:39:17.000000 adafruit-circuitpython-bluefruitconnect-1.2.8/adafruit_bluefruit_connect/location_packet.py
--rw-r--r--   0 runner    (1001) docker     (123)      665 2023-02-08 17:39:17.000000 adafruit-circuitpython-bluefruitconnect-1.2.8/adafruit_bluefruit_connect/magnetometer_packet.py
--rw-r--r--   0 runner    (1001) docker     (123)     5649 2023-02-08 17:39:17.000000 adafruit-circuitpython-bluefruitconnect-1.2.8/adafruit_bluefruit_connect/packet.py
--rw-r--r--   0 runner    (1001) docker     (123)     1461 2023-02-08 17:39:17.000000 adafruit-circuitpython-bluefruitconnect-1.2.8/adafruit_bluefruit_connect/quaternion_packet.py
--rw-r--r--   0 runner    (1001) docker     (123)     1431 2023-02-08 17:39:17.000000 adafruit-circuitpython-bluefruitconnect-1.2.8/adafruit_bluefruit_connect/raw_text_packet.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-08 17:39:25.555511 adafruit-circuitpython-bluefruitconnect-1.2.8/adafruit_circuitpython_bluefruitconnect.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3970 2023-02-08 17:39:25.000000 adafruit-circuitpython-bluefruitconnect-1.2.8/adafruit_circuitpython_bluefruitconnect.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1638 2023-02-08 17:39:25.000000 adafruit-circuitpython-bluefruitconnect-1.2.8/adafruit_circuitpython_bluefruitconnect.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-08 17:39:25.000000 adafruit-circuitpython-bluefruitconnect-1.2.8/adafruit_circuitpython_bluefruitconnect.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-02-08 17:39:25.000000 adafruit-circuitpython-bluefruitconnect-1.2.8/adafruit_circuitpython_bluefruitconnect.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       27 2023-02-08 17:39:25.000000 adafruit-circuitpython-bluefruitconnect-1.2.8/adafruit_circuitpython_bluefruitconnect.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-08 17:39:25.559511 adafruit-circuitpython-bluefruitconnect-1.2.8/docs/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-08 17:39:25.559511 adafruit-circuitpython-bluefruitconnect-1.2.8/docs/_static/
--rw-r--r--   0 runner    (1001) docker     (123)     4414 2023-02-08 17:39:02.000000 adafruit-circuitpython-bluefruitconnect-1.2.8/docs/_static/favicon.ico
--rw-r--r--   0 runner    (1001) docker     (123)      105 2023-02-08 17:39:02.000000 adafruit-circuitpython-bluefruitconnect-1.2.8/docs/_static/favicon.ico.license
--rw-r--r--   0 runner    (1001) docker     (123)      926 2023-02-08 17:39:02.000000 adafruit-circuitpython-bluefruitconnect-1.2.8/docs/api.rst
--rw-r--r--   0 runner    (1001) docker     (123)       96 2023-02-08 17:39:02.000000 adafruit-circuitpython-bluefruitconnect-1.2.8/docs/api.rst.license
--rw-r--r--   0 runner    (1001) docker     (123)     5747 2023-02-08 17:39:02.000000 adafruit-circuitpython-bluefruitconnect-1.2.8/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)     1038 2023-02-08 17:39:02.000000 adafruit-circuitpython-bluefruitconnect-1.2.8/docs/examples.rst
--rw-r--r--   0 runner    (1001) docker     (123)       96 2023-02-08 17:39:02.000000 adafruit-circuitpython-bluefruitconnect-1.2.8/docs/examples.rst.license
--rw-r--r--   0 runner    (1001) docker     (123)      981 2023-02-08 17:39:02.000000 adafruit-circuitpython-bluefruitconnect-1.2.8/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)       96 2023-02-08 17:39:02.000000 adafruit-circuitpython-bluefruitconnect-1.2.8/docs/index.rst.license
--rw-r--r--   0 runner    (1001) docker     (123)      123 2023-02-08 17:39:02.000000 adafruit-circuitpython-bluefruitconnect-1.2.8/docs/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-08 17:39:25.559511 adafruit-circuitpython-bluefruitconnect-1.2.8/examples/
--rw-r--r--   0 runner    (1001) docker     (123)     2050 2023-02-08 17:39:17.000000 adafruit-circuitpython-bluefruitconnect-1.2.8/examples/bluefruitconnect_controlpad.py
--rw-r--r--   0 runner    (1001) docker     (123)     2247 2023-02-08 17:39:17.000000 adafruit-circuitpython-bluefruitconnect-1.2.8/examples/bluefruitconnect_sensors.py
--rw-r--r--   0 runner    (1001) docker     (123)     1031 2023-02-08 17:39:17.000000 adafruit-circuitpython-bluefruitconnect-1.2.8/examples/bluefruitconnect_simpletest.py
--rw-r--r--   0 runner    (1001) docker     (123)     1374 2023-02-08 17:39:17.000000 adafruit-circuitpython-bluefruitconnect-1.2.8/examples/bluefruitconnect_simpletest2.py
--rw-r--r--   0 runner    (1001) docker     (123)     1638 2023-02-08 17:39:17.000000 adafruit-circuitpython-bluefruitconnect-1.2.8/examples/bluefruitconnect_uart.py
--rw-r--r--   0 runner    (1001) docker     (123)      108 2023-02-08 17:39:02.000000 adafruit-circuitpython-bluefruitconnect-1.2.8/optional_requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1240 2023-02-08 17:39:17.000000 adafruit-circuitpython-bluefruitconnect-1.2.8/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      125 2023-02-08 17:39:02.000000 adafruit-circuitpython-bluefruitconnect-1.2.8/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-02-08 17:39:25.559511 adafruit-circuitpython-bluefruitconnect-1.2.8/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 16:20:59.292665 adafruit-circuitpython-bluefruitconnect-1.2.9/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 16:20:59.284665 adafruit-circuitpython-bluefruitconnect-1.2.9/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 16:20:59.288665 adafruit-circuitpython-bluefruitconnect-1.2.9/.github/PULL_REQUEST_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (123)      880 2023-05-08 16:20:40.000000 adafruit-circuitpython-bluefruitconnect-1.2.9/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 16:20:59.288665 adafruit-circuitpython-bluefruitconnect-1.2.9/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      303 2023-05-08 16:20:40.000000 adafruit-circuitpython-bluefruitconnect-1.2.9/.github/workflows/build.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      479 2023-05-08 16:20:40.000000 adafruit-circuitpython-bluefruitconnect-1.2.9/.github/workflows/failure-help-text.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      482 2023-05-08 16:20:40.000000 adafruit-circuitpython-bluefruitconnect-1.2.9/.github/workflows/release_gh.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      475 2023-05-08 16:20:40.000000 adafruit-circuitpython-bluefruitconnect-1.2.9/.github/workflows/release_pypi.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1654 2023-05-08 16:20:40.000000 adafruit-circuitpython-bluefruitconnect-1.2.9/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     1239 2023-05-08 16:20:40.000000 adafruit-circuitpython-bluefruitconnect-1.2.9/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)    13069 2023-05-08 16:20:40.000000 adafruit-circuitpython-bluefruitconnect-1.2.9/.pylintrc
+-rw-r--r--   0 runner    (1001) docker     (123)      388 2023-05-08 16:20:40.000000 adafruit-circuitpython-bluefruitconnect-1.2.9/.readthedocs.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     6147 2023-05-08 16:20:40.000000 adafruit-circuitpython-bluefruitconnect-1.2.9/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1102 2023-05-08 16:20:40.000000 adafruit-circuitpython-bluefruitconnect-1.2.9/LICENSE
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 16:20:59.288665 adafruit-circuitpython-bluefruitconnect-1.2.9/LICENSES/
+-rw-r--r--   0 runner    (1001) docker     (123)    16814 2023-05-08 16:20:40.000000 adafruit-circuitpython-bluefruitconnect-1.2.9/LICENSES/CC-BY-4.0.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1108 2023-05-08 16:20:40.000000 adafruit-circuitpython-bluefruitconnect-1.2.9/LICENSES/MIT.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1211 2023-05-08 16:20:40.000000 adafruit-circuitpython-bluefruitconnect-1.2.9/LICENSES/Unlicense.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     3970 2023-05-08 16:20:59.292665 adafruit-circuitpython-bluefruitconnect-1.2.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3185 2023-05-08 16:20:40.000000 adafruit-circuitpython-bluefruitconnect-1.2.9/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      108 2023-05-08 16:20:40.000000 adafruit-circuitpython-bluefruitconnect-1.2.9/README.rst.license
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 16:20:59.288665 adafruit-circuitpython-bluefruitconnect-1.2.9/adafruit_bluefruit_connect/
+-rw-r--r--   0 runner    (1001) docker     (123)      584 2023-05-08 16:20:51.000000 adafruit-circuitpython-bluefruitconnect-1.2.9/adafruit_bluefruit_connect/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1563 2023-05-08 16:20:51.000000 adafruit-circuitpython-bluefruitconnect-1.2.9/adafruit_bluefruit_connect/_xyz_packet.py
+-rw-r--r--   0 runner    (1001) docker     (123)      714 2023-05-08 16:20:51.000000 adafruit-circuitpython-bluefruitconnect-1.2.9/adafruit_bluefruit_connect/accelerometer_packet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3282 2023-05-08 16:20:51.000000 adafruit-circuitpython-bluefruitconnect-1.2.9/adafruit_bluefruit_connect/button_packet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2326 2023-05-08 16:20:51.000000 adafruit-circuitpython-bluefruitconnect-1.2.9/adafruit_bluefruit_connect/color_packet.py
+-rw-r--r--   0 runner    (1001) docker     (123)      673 2023-05-08 16:20:51.000000 adafruit-circuitpython-bluefruitconnect-1.2.9/adafruit_bluefruit_connect/gyro_packet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1770 2023-05-08 16:20:51.000000 adafruit-circuitpython-bluefruitconnect-1.2.9/adafruit_bluefruit_connect/location_packet.py
+-rw-r--r--   0 runner    (1001) docker     (123)      708 2023-05-08 16:20:51.000000 adafruit-circuitpython-bluefruitconnect-1.2.9/adafruit_bluefruit_connect/magnetometer_packet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6017 2023-05-08 16:20:51.000000 adafruit-circuitpython-bluefruitconnect-1.2.9/adafruit_bluefruit_connect/packet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1583 2023-05-08 16:20:51.000000 adafruit-circuitpython-bluefruitconnect-1.2.9/adafruit_bluefruit_connect/quaternion_packet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1499 2023-05-08 16:20:51.000000 adafruit-circuitpython-bluefruitconnect-1.2.9/adafruit_bluefruit_connect/raw_text_packet.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 16:20:59.288665 adafruit-circuitpython-bluefruitconnect-1.2.9/adafruit_circuitpython_bluefruitconnect.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3970 2023-05-08 16:20:59.000000 adafruit-circuitpython-bluefruitconnect-1.2.9/adafruit_circuitpython_bluefruitconnect.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1638 2023-05-08 16:20:59.000000 adafruit-circuitpython-bluefruitconnect-1.2.9/adafruit_circuitpython_bluefruitconnect.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-08 16:20:59.000000 adafruit-circuitpython-bluefruitconnect-1.2.9/adafruit_circuitpython_bluefruitconnect.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-05-08 16:20:59.000000 adafruit-circuitpython-bluefruitconnect-1.2.9/adafruit_circuitpython_bluefruitconnect.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-05-08 16:20:59.000000 adafruit-circuitpython-bluefruitconnect-1.2.9/adafruit_circuitpython_bluefruitconnect.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 16:20:59.288665 adafruit-circuitpython-bluefruitconnect-1.2.9/docs/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 16:20:59.288665 adafruit-circuitpython-bluefruitconnect-1.2.9/docs/_static/
+-rw-r--r--   0 runner    (1001) docker     (123)     4414 2023-05-08 16:20:40.000000 adafruit-circuitpython-bluefruitconnect-1.2.9/docs/_static/favicon.ico
+-rw-r--r--   0 runner    (1001) docker     (123)      105 2023-05-08 16:20:40.000000 adafruit-circuitpython-bluefruitconnect-1.2.9/docs/_static/favicon.ico.license
+-rw-r--r--   0 runner    (1001) docker     (123)      926 2023-05-08 16:20:40.000000 adafruit-circuitpython-bluefruitconnect-1.2.9/docs/api.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       96 2023-05-08 16:20:40.000000 adafruit-circuitpython-bluefruitconnect-1.2.9/docs/api.rst.license
+-rw-r--r--   0 runner    (1001) docker     (123)     5747 2023-05-08 16:20:40.000000 adafruit-circuitpython-bluefruitconnect-1.2.9/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1038 2023-05-08 16:20:40.000000 adafruit-circuitpython-bluefruitconnect-1.2.9/docs/examples.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       96 2023-05-08 16:20:40.000000 adafruit-circuitpython-bluefruitconnect-1.2.9/docs/examples.rst.license
+-rw-r--r--   0 runner    (1001) docker     (123)      981 2023-05-08 16:20:40.000000 adafruit-circuitpython-bluefruitconnect-1.2.9/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       96 2023-05-08 16:20:40.000000 adafruit-circuitpython-bluefruitconnect-1.2.9/docs/index.rst.license
+-rw-r--r--   0 runner    (1001) docker     (123)      123 2023-05-08 16:20:40.000000 adafruit-circuitpython-bluefruitconnect-1.2.9/docs/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 16:20:59.292665 adafruit-circuitpython-bluefruitconnect-1.2.9/examples/
+-rw-r--r--   0 runner    (1001) docker     (123)     2050 2023-05-08 16:20:51.000000 adafruit-circuitpython-bluefruitconnect-1.2.9/examples/bluefruitconnect_controlpad.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2247 2023-05-08 16:20:51.000000 adafruit-circuitpython-bluefruitconnect-1.2.9/examples/bluefruitconnect_sensors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1031 2023-05-08 16:20:51.000000 adafruit-circuitpython-bluefruitconnect-1.2.9/examples/bluefruitconnect_simpletest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1374 2023-05-08 16:20:51.000000 adafruit-circuitpython-bluefruitconnect-1.2.9/examples/bluefruitconnect_simpletest2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1638 2023-05-08 16:20:51.000000 adafruit-circuitpython-bluefruitconnect-1.2.9/examples/bluefruitconnect_uart.py
+-rw-r--r--   0 runner    (1001) docker     (123)      108 2023-05-08 16:20:40.000000 adafruit-circuitpython-bluefruitconnect-1.2.9/optional_requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1240 2023-05-08 16:20:51.000000 adafruit-circuitpython-bluefruitconnect-1.2.9/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      125 2023-05-08 16:20:40.000000 adafruit-circuitpython-bluefruitconnect-1.2.9/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-08 16:20:59.292665 adafruit-circuitpython-bluefruitconnect-1.2.9/setup.cfg
```

### Comparing `adafruit-circuitpython-bluefruitconnect-1.2.8/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md` & `adafruit-circuitpython-bluefruitconnect-1.2.9/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-bluefruitconnect-1.2.8/.gitignore` & `adafruit-circuitpython-bluefruitconnect-1.2.9/.gitignore`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-bluefruitconnect-1.2.8/.pre-commit-config.yaml` & `adafruit-circuitpython-bluefruitconnect-1.2.9/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-bluefruitconnect-1.2.8/.pylintrc` & `adafruit-circuitpython-bluefruitconnect-1.2.9/.pylintrc`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-bluefruitconnect-1.2.8/CODE_OF_CONDUCT.md` & `adafruit-circuitpython-bluefruitconnect-1.2.9/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-bluefruitconnect-1.2.8/LICENSE` & `adafruit-circuitpython-bluefruitconnect-1.2.9/LICENSE`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-bluefruitconnect-1.2.8/LICENSES/CC-BY-4.0.txt` & `adafruit-circuitpython-bluefruitconnect-1.2.9/LICENSES/CC-BY-4.0.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-bluefruitconnect-1.2.8/LICENSES/MIT.txt` & `adafruit-circuitpython-bluefruitconnect-1.2.9/LICENSES/MIT.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-bluefruitconnect-1.2.8/LICENSES/Unlicense.txt` & `adafruit-circuitpython-bluefruitconnect-1.2.9/LICENSES/Unlicense.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-bluefruitconnect-1.2.8/PKG-INFO` & `adafruit-circuitpython-bluefruitconnect-1.2.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: adafruit-circuitpython-bluefruitconnect
-Version: 1.2.8
+Version: 1.2.9
 Summary: CircuitPython library for use with the Adafruit Bluefruit Connect apps.
 Author-email: Adafruit Industries <circuitpython@adafruit.com>
 License: MIT
 Project-URL: Homepage, https://github.com/adafruit/Adafruit_CircuitPython_BluefruitConnect
 Keywords: adafruit,ble,bluefruit,bluetooth,micropython,circuitpython
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Libraries
```

### Comparing `adafruit-circuitpython-bluefruitconnect-1.2.8/README.rst` & `adafruit-circuitpython-bluefruitconnect-1.2.9/README.rst`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-bluefruitconnect-1.2.8/adafruit_bluefruit_connect/__init__.py` & `adafruit-circuitpython-bluefruitconnect-1.2.9/adafruit_bluefruit_connect/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,9 +13,9 @@
 
 * Author(s): Dan Halbert for Adafruit Industries
 
 """
 
 # imports
 
-__version__ = "1.2.8"
+__version__ = "1.2.9"
 __repo__ = "https://github.com/adafruit/Adafruit_CircuitPython_BluefruitConnect.git"
```

### Comparing `adafruit-circuitpython-bluefruitconnect-1.2.8/adafruit_bluefruit_connect/_xyz_packet.py` & `adafruit-circuitpython-bluefruitconnect-1.2.9/adafruit_bluefruit_connect/_xyz_packet.py`

 * *Files 16% similar despite different names*

```diff
@@ -8,49 +8,51 @@
 
 Bluefruit Connect App superclass for all data packets with (x, y, z) values
 
 * Author(s): Dan Halbert for Adafruit Industries
 
 """
 
+from __future__ import annotations
+
 import struct
 
 from .packet import Packet
 
 
 class _XYZPacket(Packet):
     """A packet of x, y, z float values. Used for several different Bluefruit controller packets."""
 
-    _FMT_PARSE = "<xxfffx"
-    PACKET_LENGTH = struct.calcsize(_FMT_PARSE)
+    _FMT_PARSE: str = "<xxfffx"
+    PACKET_LENGTH: int = struct.calcsize(_FMT_PARSE)
     # _FMT_CONSTRUCT doesn't include the trailing checksum byte.
-    _FMT_CONSTRUCT = "<2sfff"
+    _FMT_CONSTRUCT: str = "<2sfff"
     # _TYPE_HEADER is set by each concrete subclass.
 
-    def __init__(self, x, y, z):
+    def __init__(self, x: float, y: float, z: float) -> None:
         # Construct an _XYZPacket subclass object
         # from the given x, y, and z float values, and type character.
         self._x = x
         self._y = y
         self._z = z
 
-    def to_bytes(self):
+    def to_bytes(self) -> bytes:
         """Return the bytes needed to send this packet."""
         partial_packet = struct.pack(
             self._FMT_CONSTRUCT, self._TYPE_HEADER, self._x, self._y, self._z
         )
         return self.add_checksum(partial_packet)
 
     @property
-    def x(self):
+    def x(self) -> float:
         """The x value."""
         return self._x
 
     @property
-    def y(self):
+    def y(self) -> float:
         """The y value."""
         return self._y
 
     @property
-    def z(self):
+    def z(self) -> float:
         """The z value."""
         return self._z
```

### Comparing `adafruit-circuitpython-bluefruitconnect-1.2.8/adafruit_bluefruit_connect/accelerometer_packet.py` & `adafruit-circuitpython-bluefruitconnect-1.2.9/adafruit_bluefruit_connect/accelerometer_packet.py`

 * *Files 16% similar despite different names*

```diff
@@ -8,19 +8,21 @@
 
 Bluefruit Connect App Accelerometer data packet.
 
 * Author(s): Dan Halbert for Adafruit Industries
 
 """
 
+from __future__ import annotations
+
 from ._xyz_packet import _XYZPacket
 
 
 class AccelerometerPacket(_XYZPacket):
     """A packet of x, y, z float values from an accelerometer."""
 
     # Everything else is handled by _XYZPacket.
-    _TYPE_HEADER = b"!A"
+    _TYPE_HEADER: bytes = b"!A"
 
 
 # Register this class with the superclass. This allows the user to import only what is needed.
 AccelerometerPacket.register_packet_type()
```

### Comparing `adafruit-circuitpython-bluefruitconnect-1.2.8/adafruit_bluefruit_connect/button_packet.py` & `adafruit-circuitpython-bluefruitconnect-1.2.9/adafruit_bluefruit_connect/button_packet.py`

 * *Files 18% similar despite different names*

```diff
@@ -9,91 +9,98 @@
 Bluefruit Connect App Button data packet (button_name, pressed/released)
 
 
 * Author(s): Dan Halbert for Adafruit Industries
 
 """
 
+from __future__ import annotations
+
 import struct
 
 from .packet import Packet
 
+try:
+    from typing import Optional  # adjust these as needed
+except ImportError:
+    pass
+
 
 class ButtonPacket(Packet):
     """A packet containing a button name and its state."""
 
-    BUTTON_1 = "1"
+    BUTTON_1: str = "1"
     """Code for Button 1 on the Bluefruit LE Connect app Control Pad screen."""
-    BUTTON_2 = "2"
+    BUTTON_2: str = "2"
     """Button 2."""
-    BUTTON_3 = "3"
+    BUTTON_3: str = "3"
     """Button 3."""
-    BUTTON_4 = "4"
+    BUTTON_4: str = "4"
     """Button 4."""
     # pylint: disable= invalid-name
-    UP = "5"
+    UP: str = "5"
     """Up Button."""
-    DOWN = "6"
+    DOWN: str = "6"
     """Down Button."""
-    LEFT = "7"
+    LEFT: str = "7"
     """Left Button."""
-    RIGHT = "8"
+    RIGHT: str = "8"
     """Right Button."""
 
-    _FMT_PARSE = "<xxssx"
-    PACKET_LENGTH = struct.calcsize(_FMT_PARSE)
+    _FMT_PARSE: str = "<xxssx"
+    PACKET_LENGTH: int = struct.calcsize(_FMT_PARSE)
     # _FMT_CONSTRUCT doesn't include the trailing checksum byte.
-    _FMT_CONSTRUCT = "<2sss"
-    _TYPE_HEADER = b"!B"
+    _FMT_CONSTRUCT: str = "<2sss"
+    _TYPE_HEADER: bytes = b"!B"
 
-    def __init__(self, button, pressed):
+    def __init__(self, button: str, pressed: bool) -> None:
         """Construct a ButtonPacket from a button name and the button's state.
 
         :param str button: a single character denoting the button
         :param bool pressed: ``True`` if button is pressed; ``False`` if it is
                              released.
         """
         # This check will catch wrong length and also non-sequence args (like an int).
         try:
             assert len(button) == 1
             assert isinstance(button, str)
         except Exception as err:
             raise ValueError("Button must be a single char.") from err
 
-        self._button = button
-        self._pressed = pressed
+        self._button: str = button
+        self._pressed: bool = pressed
 
     @classmethod
-    def parse_private(cls, packet):
+    def parse_private(cls, packet: bytes) -> Optional[Packet]:
         """Construct a ButtonPacket from an incoming packet.
         Do not call this directly; call Packet.from_bytes() instead.
         pylint makes it difficult to call this method _parse(), hence the name.
         """
         button, pressed = struct.unpack(cls._FMT_PARSE, packet)
         if not pressed in b"01":
             raise ValueError("Bad button press/release value")
         return cls(chr(button[0]), pressed == b"1")
 
-    def to_bytes(self):
+    def to_bytes(self) -> bytes:
         """Return the bytes needed to send this packet."""
-        partial_packet = struct.pack(
+        partial_packet: bytes = struct.pack(
             self._FMT_CONSTRUCT,
             self._TYPE_HEADER,
             bytes(self._button, "utf-8"),
             b"1" if self._pressed else b"0",
         )
         return self.add_checksum(partial_packet)
 
     @property
-    def button(self):
+    def button(self) -> str:
         """A single character string (not bytes) specifying the button that
         the user pressed or released."""
         return self._button
 
     @property
-    def pressed(self):
+    def pressed(self) -> bool:
         """``True`` if button is pressed, or ``False`` if it is released."""
         return self._pressed
 
 
 # Register this class with the superclass. This allows the user to import only what is needed.
 ButtonPacket.register_packet_type()
```

### Comparing `adafruit-circuitpython-bluefruitconnect-1.2.8/adafruit_bluefruit_connect/color_packet.py` & `adafruit-circuitpython-bluefruitconnect-1.2.9/adafruit_bluefruit_connect/color_packet.py`

 * *Files 9% similar despite different names*

```diff
@@ -8,59 +8,66 @@
 
 Bluefruit Connect App color data packet.
 
 * Author(s): Dan Halbert for Adafruit Industries
 
 """
 
+from __future__ import annotations
+
 import struct
 
 from .packet import Packet
 
+try:
+    from typing import Optional, Tuple  # adjust these as needed
+except ImportError:
+    pass
+
 
 class ColorPacket(Packet):
     """A packet containing an RGB color value."""
 
-    _FMT_PARSE = "<xx3Bx"
-    PACKET_LENGTH = struct.calcsize(_FMT_PARSE)
+    _FMT_PARSE: str = "<xx3Bx"
+    PACKET_LENGTH: int = struct.calcsize(_FMT_PARSE)
     # _FMT_CONSTRUCT doesn't include the trailing checksum byte.
-    _FMT_CONSTRUCT = "<2s3B"
-    _TYPE_HEADER = b"!C"
+    _FMT_CONSTRUCT: str = "<2s3B"
+    _TYPE_HEADER: bytes = b"!C"
 
-    def __init__(self, color):
+    def __init__(self, color: Tuple) -> None:
         """Construct a ColorPacket from a 3-element :class:`tuple` of RGB
         values, or from an int color value 0xRRGGBB.
 
         :param tuple/int color: an RGB :class:`tuple` ``(red, green, blue)``
           or an int color value ``0xRRGGBB``
         """
         if isinstance(color, int):
-            self._color = tuple(color.to_bytes(3, "big"))
+            self._color: Tuple = tuple(color.to_bytes(3, "big"))
         elif len(color) == 3 and all(0 <= c <= 255 for c in color):
             self._color = color
         else:
             raise ValueError("Color must be an integer 0xRRGGBB or a tuple(r,g,b)")
 
     @classmethod
-    def parse_private(cls, packet):
+    def parse_private(cls, packet: bytes) -> Optional[Packet]:
         """Construct a ColorPacket from an incoming packet.
         Do not call this directly; call Packet.from_bytes() instead.
         pylint makes it difficult to call this method _parse(), hence the name.
         """
         return cls(struct.unpack(cls._FMT_PARSE, packet))
 
-    def to_bytes(self):
+    def to_bytes(self) -> bytes:
         """Return the bytes needed to send this packet."""
         partial_packet = struct.pack(
             self._FMT_CONSTRUCT, self._TYPE_HEADER, *self._color
         )
         return self.add_checksum(partial_packet)
 
     @property
-    def color(self):
+    def color(self) -> tuple:
         """A :class:`tuple` ``(red, green blue)`` representing the color the
         user chose in the BlueFruit Connect app."""
         return self._color
 
 
 # Register this class with the superclass. This allows the user to import only what is needed.
 ColorPacket.register_packet_type()
```

### Comparing `adafruit-circuitpython-bluefruitconnect-1.2.8/adafruit_bluefruit_connect/gyro_packet.py` & `adafruit-circuitpython-bluefruitconnect-1.2.9/adafruit_bluefruit_connect/gyro_packet.py`

 * *Files 7% similar despite different names*

```diff
@@ -8,19 +8,21 @@
 
 Bluefruit Connect App Gyro data packet.
 
 * Author(s): Dan Halbert for Adafruit Industries
 
 """
 
+from __future__ import annotations
+
 from ._xyz_packet import _XYZPacket
 
 
 class GyroPacket(_XYZPacket):
     """A packet of x, y, z float values from a gyroscope."""
 
     # Everything else is handled by _XYZPacket.
-    _TYPE_HEADER = b"!G"
+    _TYPE_HEADER: bytes = b"!G"
 
 
 # Register this class with the superclass. This allows the user to import only what is needed.
 GyroPacket.register_packet_type()
```

### Comparing `adafruit-circuitpython-bluefruitconnect-1.2.8/adafruit_bluefruit_connect/location_packet.py` & `adafruit-circuitpython-bluefruitconnect-1.2.9/adafruit_bluefruit_connect/location_packet.py`

 * *Files 10% similar despite different names*

```diff
@@ -8,56 +8,58 @@
 
 Bluefruit Connect App geographical location packet.
 
 * Author(s): Dan Halbert for Adafruit Industries
 
 """
 
+from __future__ import annotations
+
 import struct
 
 from .packet import Packet
 
 
 class LocationPacket(Packet):
     """A packet of latitude, longitude, and altitude values."""
 
-    _FMT_PARSE = "<xxfffx"
-    PACKET_LENGTH = struct.calcsize(_FMT_PARSE)
+    _FMT_PARSE: str = "<xxfffx"
+    PACKET_LENGTH: int = struct.calcsize(_FMT_PARSE)
     # _FMT_CONSTRUCT doesn't include the trailing checksum byte.
-    _FMT_CONSTRUCT = "<2sfff"
-    _TYPE_HEADER = b"!L"
+    _FMT_CONSTRUCT: str = "<2sfff"
+    _TYPE_HEADER: bytes = b"!L"
 
-    def __init__(self, latitude, longitude, altitude):
+    def __init__(self, latitude: float, longitude: float, altitude: float) -> None:
         """Construct a LocationPacket from the given values."""
         self._latitude = latitude
         self._longitude = longitude
         self._altitude = altitude
 
-    def to_bytes(self):
+    def to_bytes(self) -> bytes:
         """Return the bytes needed to send this packet."""
         partial_packet = struct.pack(
             self._FMT_CONSTRUCT,
             self._TYPE_HEADER,
             self._latitude,
             self._longitude,
             self._altitude,
         )
         return self.add_checksum(partial_packet)
 
     @property
-    def latitude(self):
+    def latitude(self) -> float:
         """The latitude value."""
         return self._latitude
 
     @property
-    def longitude(self):
+    def longitude(self) -> float:
         """The longitude value."""
         return self._longitude
 
     @property
-    def altitude(self):
+    def altitude(self) -> float:
         """The altitude value."""
         return self._altitude
 
 
 # Register this class with the superclass. This allows the user to import only what is needed.
 LocationPacket.register_packet_type()
```

### Comparing `adafruit-circuitpython-bluefruitconnect-1.2.8/adafruit_bluefruit_connect/magnetometer_packet.py` & `adafruit-circuitpython-bluefruitconnect-1.2.9/adafruit_bluefruit_connect/magnetometer_packet.py`

 * *Files 22% similar despite different names*

```diff
@@ -8,19 +8,21 @@
 
 Bluefruit Connect App Magnetometer data packet.
 
 * Author(s): Dan Halbert for Adafruit Industries
 
 """
 
+from __future__ import annotations
+
 from ._xyz_packet import _XYZPacket
 
 
 class MagnetometerPacket(_XYZPacket):
     """A packet of x, y, z float values from a magnetometer."""
 
     # Everything else is handled by _XYZPacket.
-    _TYPE_HEADER = b"!M"
+    _TYPE_HEADER: bytes = b"!M"
 
 
 # Register this class with the superclass. This allows the user to import only what is needed.
 MagnetometerPacket.register_packet_type()
```

### Comparing `adafruit-circuitpython-bluefruitconnect-1.2.8/adafruit_bluefruit_connect/packet.py` & `adafruit-circuitpython-bluefruitconnect-1.2.9/adafruit_bluefruit_connect/packet.py`

 * *Files 11% similar despite different names*

```diff
@@ -8,17 +8,26 @@
 
 Bluefruit Connect App packet superclass
 
 * Author(s): Dan Halbert for Adafruit Industries
 
 """
 
+from __future__ import annotations
+
 import struct
 
 
+try:
+    from typing import Optional, Any  # adjust these as needed
+    from io import RawIOBase
+except ImportError:
+    pass
+
+
 class Packet:
     """
     A Bluefruit app controller packet. A packet consists of these bytes, in order:
 
       - '!' - The first byte is always an exclamation point.
       - *type* - A single byte designating the type of packet: b'A', b'B', etc.
       - *data ...* - Multiple bytes of data, varying by packet type.
@@ -27,35 +36,35 @@
 
     This is an abstract class.
     """
 
     # All concrete subclasses should define these class attributes. They're listed here
     # as a reminder and to make pylint happy.
     # _FMT_PARSE is the whole packet.
-    _FMT_PARSE = None
+    _FMT_PARSE: str
     # In each class, set PACKET_LENGTH = struct.calcsize(_FMT_PARSE).
-    PACKET_LENGTH = None
+    PACKET_LENGTH: int
     # _FMT_CONSTRUCT does not include the trailing byte, which is the checksum.
-    _FMT_CONSTRUCT = None
+    _FMT_CONSTRUCT: Optional[str] = None
     # The first byte of the prefix is always b'!'. The second byte is the type code.
-    _TYPE_HEADER = None
+    _TYPE_HEADER: Optional[bytes] = None
 
-    _type_to_class = {}
+    _type_to_class: dict = {}
 
     @classmethod
-    def register_packet_type(cls):
+    def register_packet_type(cls: Any) -> None:
         """Register a new packet type, using this class and its ``cls._TYPE_HEADER``.
         The ``from_bytes()`` and ``from_stream()`` methods will then be able
         to recognize this type of packet.
         """
 
         Packet._type_to_class[cls._TYPE_HEADER] = cls
 
     @classmethod
-    def from_bytes(cls, packet):
+    def from_bytes(cls, packet: bytes) -> Packet:
         """Create an appropriate object of the correct class for the given packet bytes.
         Validate packet type, length, and checksum.
         """
         if len(packet) < 3:
             raise ValueError("Packet too short")
         packet_class = cls._type_to_class.get(packet[0:2], None)
         if not packet_class:
@@ -72,15 +81,15 @@
         if cls.checksum(packet[0:-1]) != packet[-1]:
             raise ValueError("Bad checksum")
 
         # A packet class may do further validation of the data.
         return packet_class.parse_private(packet)
 
     @classmethod
-    def from_stream(cls, stream):
+    def from_stream(cls, stream: RawIOBase) -> Optional[Packet]:
         """Read the next packet from the incoming stream. Wait as long as the timeout
         set on stream, using its own preset timeout.
         Return None if there was no input, otherwise return an instance
         of one of the packet classes registered with ``Packet``.
         Raise an Error if the packet was not recognized or was malformed.
 
         If a packet of type "RT" (like ``RawTextPacket``) is registered, it will be
@@ -116,32 +125,34 @@
 
             # else loop and try again.
 
         header = bytes(start + packet_type)
         packet_class = cls._type_to_class.get(header, None)
         if not packet_class:
             raise ValueError("Unregistered packet type {}".format(header))
-        packet = header + stream.read(packet_class.PACKET_LENGTH - 2)
+        rest = stream.read(packet_class.PACKET_LENGTH - 2)
+        assert rest is not None
+        packet = header + rest
         return cls.from_bytes(packet)
 
     @classmethod
-    def parse_private(cls, packet):
+    def parse_private(cls, packet: bytes) -> Optional[Packet]:
         """Default implementation for subclasses.
         Assumes arguments to ``__init__()`` are exactly the values parsed using
         ``cls._FMT_PARSE``. Subclasses may need to reimplement if that assumption
         is not correct.
 
         Do not call this directly. It's called from ``cls.from_bytes()``.
         pylint makes it difficult to call this method _parse(), hence the name.
         """
         return cls(*struct.unpack(cls._FMT_PARSE, packet))
 
     @staticmethod
-    def checksum(partial_packet):
+    def checksum(partial_packet: bytes) -> int:
         """Compute checksum for bytes, not including the checksum byte itself."""
         return ~sum(partial_packet) & 0xFF
 
-    def add_checksum(self, partial_packet):
+    def add_checksum(self, partial_packet: bytes) -> bytes:
         """Compute the checksum of partial_packet and return a new bytes
         with the checksum appended.
         """
         return partial_packet + bytes((self.checksum(partial_packet),))
```

### Comparing `adafruit-circuitpython-bluefruitconnect-1.2.8/adafruit_bluefruit_connect/quaternion_packet.py` & `adafruit-circuitpython-bluefruitconnect-1.2.9/adafruit_bluefruit_connect/quaternion_packet.py`

 * *Files 16% similar despite different names*

```diff
@@ -8,44 +8,46 @@
 
 Bluefruit Connect App Quaternion data packet.
 
 * Author(s): Dan Halbert for Adafruit Industries
 
 """
 
+from __future__ import annotations
+
 import struct
 
 from ._xyz_packet import _XYZPacket
 
 
 class QuaternionPacket(_XYZPacket):
     """Device Motion data to describe device attitude. This data is derived
     from Accelerometer, Gyro, and Magnetometer readings."""
 
     # Use _XYZPacket to handle x, y, z, and add w.
 
-    _FMT_PARSE = "<xxffffx"
-    PACKET_LENGTH = struct.calcsize(_FMT_PARSE)
+    _FMT_PARSE: str = "<xxffffx"
+    PACKET_LENGTH: int = struct.calcsize(_FMT_PARSE)
     # _FMT_CONSTRUCT doesn't include the trailing checksum byte.
-    _FMT_CONSTRUCT = "<2sffff"
-    _TYPE_HEADER = b"!Q"
+    _FMT_CONSTRUCT: str = "<2sffff"
+    _TYPE_HEADER: bytes = b"!Q"
 
-    def __init__(self, x, y, z, w):
+    def __init__(self, x: float, y: float, z: float, w: float) -> None:
         """Construct a QuaternionPacket from the given x, y, z, and w float values."""
         super().__init__(x, y, z)
         self._w = w
 
-    def to_bytes(self):
+    def to_bytes(self) -> bytes:
         """Return the bytes needed to send this packet."""
         partial_packet = struct.pack(
             self._FMT_CONSTRUCT, self._TYPE_HEADER, self._x, self._y, self._z, self._w
         )
-        return partial_packet + self.checksum(partial_packet)
+        return partial_packet + bytes((self.checksum(partial_packet),))
 
     @property
-    def w(self):
+    def w(self) -> float:
         """The w value."""
         return self._w
 
 
 # Register this class with the superclass. This allows the user to import only what is needed.
 QuaternionPacket.register_packet_type()
```

### Comparing `adafruit-circuitpython-bluefruitconnect-1.2.8/adafruit_bluefruit_connect/raw_text_packet.py` & `adafruit-circuitpython-bluefruitconnect-1.2.9/adafruit_bluefruit_connect/raw_text_packet.py`

 * *Files 12% similar despite different names*

```diff
@@ -18,30 +18,32 @@
 
 Consequently, this packet type is MUCH simpler than the other packet types.
 
 * Author(s): Tony Hansen
 
 """
 
+from __future__ import annotations
+
 from .packet import Packet
 
 
 class RawTextPacket(Packet):
     """A packet containing a text string."""
 
-    _TYPE_HEADER = b"RT"
+    _TYPE_HEADER: bytes = b"RT"
 
-    def __init__(self, text):
+    def __init__(self, text: str) -> None:
         """Construct a RawTextPacket from a binary string."""
         if isinstance(text, bytes):
-            self._text = text.strip()
+            self._text: str = text.strip()
         else:
             raise ValueError("Text must be a bytes string")
 
     @property
-    def text(self):
+    def text(self) -> str:
         """Return the text associated with the object."""
         return self._text
 
 
 # Register this class with the superclass. This allows the user to import only what is needed.
 RawTextPacket.register_packet_type()
```

### Comparing `adafruit-circuitpython-bluefruitconnect-1.2.8/adafruit_circuitpython_bluefruitconnect.egg-info/PKG-INFO` & `adafruit-circuitpython-bluefruitconnect-1.2.9/adafruit_circuitpython_bluefruitconnect.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: adafruit-circuitpython-bluefruitconnect
-Version: 1.2.8
+Version: 1.2.9
 Summary: CircuitPython library for use with the Adafruit Bluefruit Connect apps.
 Author-email: Adafruit Industries <circuitpython@adafruit.com>
 License: MIT
 Project-URL: Homepage, https://github.com/adafruit/Adafruit_CircuitPython_BluefruitConnect
 Keywords: adafruit,ble,bluefruit,bluetooth,micropython,circuitpython
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Libraries
```

### Comparing `adafruit-circuitpython-bluefruitconnect-1.2.8/adafruit_circuitpython_bluefruitconnect.egg-info/SOURCES.txt` & `adafruit-circuitpython-bluefruitconnect-1.2.9/adafruit_circuitpython_bluefruitconnect.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-bluefruitconnect-1.2.8/docs/_static/favicon.ico` & `adafruit-circuitpython-bluefruitconnect-1.2.9/docs/_static/favicon.ico`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-bluefruitconnect-1.2.8/docs/api.rst` & `adafruit-circuitpython-bluefruitconnect-1.2.9/docs/api.rst`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-bluefruitconnect-1.2.8/docs/conf.py` & `adafruit-circuitpython-bluefruitconnect-1.2.9/docs/conf.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-bluefruitconnect-1.2.8/docs/examples.rst` & `adafruit-circuitpython-bluefruitconnect-1.2.9/docs/examples.rst`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-bluefruitconnect-1.2.8/docs/index.rst` & `adafruit-circuitpython-bluefruitconnect-1.2.9/docs/index.rst`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-bluefruitconnect-1.2.8/examples/bluefruitconnect_controlpad.py` & `adafruit-circuitpython-bluefruitconnect-1.2.9/examples/bluefruitconnect_controlpad.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-bluefruitconnect-1.2.8/examples/bluefruitconnect_sensors.py` & `adafruit-circuitpython-bluefruitconnect-1.2.9/examples/bluefruitconnect_sensors.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-bluefruitconnect-1.2.8/examples/bluefruitconnect_simpletest.py` & `adafruit-circuitpython-bluefruitconnect-1.2.9/examples/bluefruitconnect_simpletest.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-bluefruitconnect-1.2.8/examples/bluefruitconnect_simpletest2.py` & `adafruit-circuitpython-bluefruitconnect-1.2.9/examples/bluefruitconnect_simpletest2.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-bluefruitconnect-1.2.8/examples/bluefruitconnect_uart.py` & `adafruit-circuitpython-bluefruitconnect-1.2.9/examples/bluefruitconnect_uart.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-bluefruitconnect-1.2.8/pyproject.toml` & `adafruit-circuitpython-bluefruitconnect-1.2.9/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -8,15 +8,15 @@
     "wheel",
     "setuptools-scm",
 ]
 
 [project]
 name = "adafruit-circuitpython-bluefruitconnect"
 description = "CircuitPython library for use with the Adafruit Bluefruit Connect apps."
-version = "1.2.8"
+version = "1.2.9"
 readme = "README.rst"
 authors = [
     {name = "Adafruit Industries", email = "circuitpython@adafruit.com"}
 ]
 urls = {Homepage = "https://github.com/adafruit/Adafruit_CircuitPython_BluefruitConnect"}
 keywords = [
     "adafruit",
```

