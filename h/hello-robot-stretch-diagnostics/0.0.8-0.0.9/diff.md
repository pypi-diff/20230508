# Comparing `tmp/hello_robot_stretch_diagnostics-0.0.8.tar.gz` & `tmp/hello_robot_stretch_diagnostics-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hello_robot_stretch_diagnostics-0.0.8.tar", last modified: Mon Mar 13 18:38:02 2023, max compression
+gzip compressed data, was "hello_robot_stretch_diagnostics-0.0.9.tar", last modified: Fri Mar 24 21:28:32 2023, max compression
```

## Comparing `hello_robot_stretch_diagnostics-0.0.8.tar` & `hello_robot_stretch_diagnostics-0.0.9.tar`

### file list

```diff
@@ -1,67 +1,67 @@
-drwxrwxr-x   0 hello-robot  (1000) hello-robot  (1000)        0 2023-03-13 18:38:02.388902 hello_robot_stretch_diagnostics-0.0.8/
--rw-rw-r--   0 hello-robot  (1000) hello-robot  (1000)     2961 2023-03-13 18:38:02.388902 hello_robot_stretch_diagnostics-0.0.8/PKG-INFO
-drwxrwxr-x   0 hello-robot  (1000) hello-robot  (1000)        0 2023-03-13 18:38:02.380902 hello_robot_stretch_diagnostics-0.0.8/hello_robot_stretch_diagnostics.egg-info/
--rw-rw-r--   0 hello-robot  (1000) hello-robot  (1000)     2961 2023-03-13 18:38:02.000000 hello_robot_stretch_diagnostics-0.0.8/hello_robot_stretch_diagnostics.egg-info/PKG-INFO
--rw-rw-r--   0 hello-robot  (1000) hello-robot  (1000)     2916 2023-03-13 18:38:02.000000 hello_robot_stretch_diagnostics-0.0.8/hello_robot_stretch_diagnostics.egg-info/SOURCES.txt
--rw-rw-r--   0 hello-robot  (1000) hello-robot  (1000)        1 2023-03-13 18:38:02.000000 hello_robot_stretch_diagnostics-0.0.8/hello_robot_stretch_diagnostics.egg-info/dependency_links.txt
--rw-rw-r--   0 hello-robot  (1000) hello-robot  (1000)       86 2023-03-13 18:38:02.000000 hello_robot_stretch_diagnostics-0.0.8/hello_robot_stretch_diagnostics.egg-info/requires.txt
--rw-rw-r--   0 hello-robot  (1000) hello-robot  (1000)       46 2023-03-13 18:38:02.000000 hello_robot_stretch_diagnostics-0.0.8/hello_robot_stretch_diagnostics.egg-info/top_level.txt
--rw-rw-r--   0 hello-robot  (1000) hello-robot  (1000)       38 2023-03-13 18:38:02.388902 hello_robot_stretch_diagnostics-0.0.8/setup.cfg
--rw-rw-r--   0 hello-robot  (1000) hello-robot  (1000)     1343 2023-03-13 18:37:24.000000 hello_robot_stretch_diagnostics-0.0.8/setup.py
-drwxrwxr-x   0 hello-robot  (1000) hello-robot  (1000)        0 2023-03-13 18:38:02.384902 hello_robot_stretch_diagnostics-0.0.8/stretch_diagnostics/
--rw-rw-r--   0 hello-robot  (1000) hello-robot  (1000)        0 2023-03-13 18:17:02.000000 hello_robot_stretch_diagnostics-0.0.8/stretch_diagnostics/__init__.py
--rw-rw-r--   0 hello-robot  (1000) hello-robot  (1000)     4799 2023-03-13 18:17:02.000000 hello_robot_stretch_diagnostics-0.0.8/stretch_diagnostics/test_base.py
--rw-rw-r--   0 hello-robot  (1000) hello-robot  (1000)    10779 2023-03-13 18:17:02.000000 hello_robot_stretch_diagnostics-0.0.8/stretch_diagnostics/test_helpers.py
--rw-rw-r--   0 hello-robot  (1000) hello-robot  (1000)    16570 2023-03-13 18:17:02.000000 hello_robot_stretch_diagnostics-0.0.8/stretch_diagnostics/test_manager.py
--rw-rw-r--   0 hello-robot  (1000) hello-robot  (1000)     1583 2023-03-13 18:17:02.000000 hello_robot_stretch_diagnostics-0.0.8/stretch_diagnostics/test_order.py
--rw-rw-r--   0 hello-robot  (1000) hello-robot  (1000)     1132 2023-03-13 18:17:02.000000 hello_robot_stretch_diagnostics-0.0.8/stretch_diagnostics/test_result.py
--rw-rw-r--   0 hello-robot  (1000) hello-robot  (1000)     2373 2023-03-13 18:17:02.000000 hello_robot_stretch_diagnostics-0.0.8/stretch_diagnostics/test_runner.py
--rw-rw-r--   0 hello-robot  (1000) hello-robot  (1000)      406 2023-03-13 18:17:02.000000 hello_robot_stretch_diagnostics-0.0.8/stretch_diagnostics/test_suite.py
-drwxrwxr-x   0 hello-robot  (1000) hello-robot  (1000)        0 2023-03-13 18:38:02.384902 hello_robot_stretch_diagnostics-0.0.8/stretch_diagnostics_tests/
--rw-rw-r--   0 hello-robot  (1000) hello-robot  (1000)        0 2023-03-13 18:17:02.000000 hello_robot_stretch_diagnostics-0.0.8/stretch_diagnostics_tests/__init__.py
-drwxrwxr-x   0 hello-robot  (1000) hello-robot  (1000)        0 2023-03-13 18:38:02.384902 hello_robot_stretch_diagnostics-0.0.8/stretch_diagnostics_tests/arm_tests/
--rwxrwxr-x   0 hello-robot  (1000) hello-robot  (1000)     5637 2023-03-13 18:17:02.000000 hello_robot_stretch_diagnostics-0.0.8/stretch_diagnostics_tests/arm_tests/test_ARM_effort_through_range_of_motion.py
-drwxrwxr-x   0 hello-robot  (1000) hello-robot  (1000)        0 2023-03-13 18:38:02.384902 hello_robot_stretch_diagnostics-0.0.8/stretch_diagnostics_tests/cpu_tests/
--rw-rw-r--   0 hello-robot  (1000) hello-robot  (1000)     2100 2023-03-13 18:17:02.000000 hello_robot_stretch_diagnostics-0.0.8/stretch_diagnostics_tests/cpu_tests/test_CPU_usage_temp.py
-drwxrwxr-x   0 hello-robot  (1000) hello-robot  (1000)        0 2023-03-13 18:38:02.384902 hello_robot_stretch_diagnostics-0.0.8/stretch_diagnostics_tests/dynamixel_tests/
--rwxrwxr-x   0 hello-robot  (1000) hello-robot  (1000)     3472 2023-03-13 18:17:02.000000 hello_robot_stretch_diagnostics-0.0.8/stretch_diagnostics_tests/dynamixel_tests/test_DYNAMIXEL_check_zero_position.py
--rwxrwxr-x   0 hello-robot  (1000) hello-robot  (1000)     6260 2023-03-13 18:17:02.000000 hello_robot_stretch_diagnostics-0.0.8/stretch_diagnostics_tests/dynamixel_tests/test_DYNAMIXEL_measure_efforts.py
--rwxrwxr-x   0 hello-robot  (1000) hello-robot  (1000)     3887 2023-03-13 18:17:02.000000 hello_robot_stretch_diagnostics-0.0.8/stretch_diagnostics_tests/dynamixel_tests/test_DYNAMIXEL_measure_range_of_motion.py
-drwxrwxr-x   0 hello-robot  (1000) hello-robot  (1000)        0 2023-03-13 18:38:02.384902 hello_robot_stretch_diagnostics-0.0.8/stretch_diagnostics_tests/gripper_tests/
--rwxrwxr-x   0 hello-robot  (1000) hello-robot  (1000)     2235 2023-03-13 18:17:02.000000 hello_robot_stretch_diagnostics-0.0.8/stretch_diagnostics_tests/gripper_tests/test_GRIPPER_broken_string.py
-drwxrwxr-x   0 hello-robot  (1000) hello-robot  (1000)        0 2023-03-13 18:38:02.384902 hello_robot_stretch_diagnostics-0.0.8/stretch_diagnostics_tests/lift_tests/
--rwxrwxr-x   0 hello-robot  (1000) hello-robot  (1000)     5718 2023-03-13 18:17:02.000000 hello_robot_stretch_diagnostics-0.0.8/stretch_diagnostics_tests/lift_tests/test_LIFT_effort_through_range_of_motion.py
-drwxrwxr-x   0 hello-robot  (1000) hello-robot  (1000)        0 2023-03-13 18:38:02.384902 hello_robot_stretch_diagnostics-0.0.8/stretch_diagnostics_tests/power_tests/
--rwxrwxr-x   0 hello-robot  (1000) hello-robot  (1000)     3292 2023-03-13 18:17:02.000000 hello_robot_stretch_diagnostics-0.0.8/stretch_diagnostics_tests/power_tests/test_POWER_battery_loading.py
--rwxrwxr-x   0 hello-robot  (1000) hello-robot  (1000)     2195 2023-03-13 18:17:02.000000 hello_robot_stretch_diagnostics-0.0.8/stretch_diagnostics_tests/power_tests/test_POWER_charger.py
-drwxrwxr-x   0 hello-robot  (1000) hello-robot  (1000)        0 2023-03-13 18:38:02.384902 hello_robot_stretch_diagnostics-0.0.8/stretch_diagnostics_tests/realsense_tests/
--rwxrwxr-x   0 hello-robot  (1000) hello-robot  (1000)     6837 2023-03-13 18:17:02.000000 hello_robot_stretch_diagnostics-0.0.8/stretch_diagnostics_tests/realsense_tests/test_REALSENSE_cable.py
--rwxrwxr-x   0 hello-robot  (1000) hello-robot  (1000)    13960 2023-03-13 18:17:02.000000 hello_robot_stretch_diagnostics-0.0.8/stretch_diagnostics_tests/realsense_tests/test_REALSENSE_frame_rate.py
-drwxrwxr-x   0 hello-robot  (1000) hello-robot  (1000)        0 2023-03-13 18:38:02.384902 hello_robot_stretch_diagnostics-0.0.8/stretch_diagnostics_tests/ros_tests/
--rw-rw-r--   0 hello-robot  (1000) hello-robot  (1000)     3442 2023-03-13 18:17:02.000000 hello_robot_stretch_diagnostics-0.0.8/stretch_diagnostics_tests/ros_tests/test_ROS_calibration.py
--rw-rw-r--   0 hello-robot  (1000) hello-robot  (1000)     3938 2023-03-13 18:17:02.000000 hello_robot_stretch_diagnostics-0.0.8/stretch_diagnostics_tests/ros_tests/test_ROS_sourced_distro.py
--rw-rw-r--   0 hello-robot  (1000) hello-robot  (1000)     5702 2023-03-13 18:17:02.000000 hello_robot_stretch_diagnostics-0.0.8/stretch_diagnostics_tests/ros_tests/test_ROS_urdf.py
-drwxrwxr-x   0 hello-robot  (1000) hello-robot  (1000)        0 2023-03-13 18:38:02.384902 hello_robot_stretch_diagnostics-0.0.8/stretch_diagnostics_tests/simple_tests/
--rwxrwxr-x   0 hello-robot  (1000) hello-robot  (1000)     7330 2023-03-13 18:17:02.000000 hello_robot_stretch_diagnostics-0.0.8/stretch_diagnostics_tests/simple_tests/test_SIMPLE_accessories.py
--rwxrwxr-x   0 hello-robot  (1000) hello-robot  (1000)     3384 2023-03-13 18:17:02.000000 hello_robot_stretch_diagnostics-0.0.8/stretch_diagnostics_tests/simple_tests/test_SIMPLE_capture_system.py
--rwxrwxr-x   0 hello-robot  (1000) hello-robot  (1000)     2995 2023-03-13 18:17:02.000000 hello_robot_stretch_diagnostics-0.0.8/stretch_diagnostics_tests/simple_tests/test_SIMPLE_dynamixel_configure.py
--rwxrwxr-x   0 hello-robot  (1000) hello-robot  (1000)     4486 2023-03-13 18:17:02.000000 hello_robot_stretch_diagnostics-0.0.8/stretch_diagnostics_tests/simple_tests/test_SIMPLE_filesystem.py
--rwxrwxr-x   0 hello-robot  (1000) hello-robot  (1000)     2828 2023-03-13 18:17:02.000000 hello_robot_stretch_diagnostics-0.0.8/stretch_diagnostics_tests/simple_tests/test_SIMPLE_firmware.py
--rwxrwxr-x   0 hello-robot  (1000) hello-robot  (1000)     3114 2023-03-13 18:17:02.000000 hello_robot_stretch_diagnostics-0.0.8/stretch_diagnostics_tests/simple_tests/test_SIMPLE_foo.py
--rwxrwxr-x   0 hello-robot  (1000) hello-robot  (1000)     2631 2023-03-13 18:17:02.000000 hello_robot_stretch_diagnostics-0.0.8/stretch_diagnostics_tests/simple_tests/test_SIMPLE_params.py
--rwxrwxr-x   0 hello-robot  (1000) hello-robot  (1000)     3153 2023-03-13 18:17:02.000000 hello_robot_stretch_diagnostics-0.0.8/stretch_diagnostics_tests/simple_tests/test_SIMPLE_pimu.py
--rwxrwxr-x   0 hello-robot  (1000) hello-robot  (1000)     5294 2023-03-13 18:17:02.000000 hello_robot_stretch_diagnostics-0.0.8/stretch_diagnostics_tests/simple_tests/test_SIMPLE_realsense_status.py
--rwxrwxr-x   0 hello-robot  (1000) hello-robot  (1000)     4174 2023-03-13 18:17:02.000000 hello_robot_stretch_diagnostics-0.0.8/stretch_diagnostics_tests/simple_tests/test_SIMPLE_rplidar.py
--rwxrwxr-x   0 hello-robot  (1000) hello-robot  (1000)     4862 2023-03-13 18:17:02.000000 hello_robot_stretch_diagnostics-0.0.8/stretch_diagnostics_tests/simple_tests/test_SIMPLE_software_packages.py
--rwxrwxr-x   0 hello-robot  (1000) hello-robot  (1000)     3283 2023-03-13 18:17:02.000000 hello_robot_stretch_diagnostics-0.0.8/stretch_diagnostics_tests/simple_tests/test_SIMPLE_steppers.py
--rwxrwxr-x   0 hello-robot  (1000) hello-robot  (1000)     1984 2023-03-13 18:17:02.000000 hello_robot_stretch_diagnostics-0.0.8/stretch_diagnostics_tests/simple_tests/test_SIMPLE_stretch_body_background.py
--rwxrwxr-x   0 hello-robot  (1000) hello-robot  (1000)     4968 2023-03-13 18:17:02.000000 hello_robot_stretch_diagnostics-0.0.8/stretch_diagnostics_tests/simple_tests/test_SIMPLE_udev.py
--rwxrwxr-x   0 hello-robot  (1000) hello-robot  (1000)     2616 2023-03-13 18:17:02.000000 hello_robot_stretch_diagnostics-0.0.8/stretch_diagnostics_tests/simple_tests/test_SIMPLE_usb_devices_on_bus.py
--rwxrwxr-x   0 hello-robot  (1000) hello-robot  (1000)     1717 2023-03-13 18:17:02.000000 hello_robot_stretch_diagnostics-0.0.8/stretch_diagnostics_tests/simple_tests/test_SIMPLE_wacc.py
--rwxrwxr-x   0 hello-robot  (1000) hello-robot  (1000)      933 2023-03-13 18:17:02.000000 hello_robot_stretch_diagnostics-0.0.8/stretch_diagnostics_tests/simple_tests/test_SIMPLE_wifi.py
-drwxrwxr-x   0 hello-robot  (1000) hello-robot  (1000)        0 2023-03-13 18:38:02.388902 hello_robot_stretch_diagnostics-0.0.8/stretch_diagnostics_tests/stepper_tests/
--rwxrwxr-x   0 hello-robot  (1000) hello-robot  (1000)     3958 2023-03-13 18:17:02.000000 hello_robot_stretch_diagnostics-0.0.8/stretch_diagnostics_tests/stepper_tests/test_STEPPER_calibration_data_match.py
--rwxrwxr-x   0 hello-robot  (1000) hello-robot  (1000)     4006 2023-03-13 18:31:56.000000 hello_robot_stretch_diagnostics-0.0.8/stretch_diagnostics_tests/stepper_tests/test_STEPPER_runstop.py
--rwxrwxr-x   0 hello-robot  (1000) hello-robot  (1000)     3531 2023-03-13 18:29:03.000000 hello_robot_stretch_diagnostics-0.0.8/stretch_diagnostics_tests/stepper_tests/test_STEPPER_sync.py
-drwxrwxr-x   0 hello-robot  (1000) hello-robot  (1000)        0 2023-03-13 18:38:02.380902 hello_robot_stretch_diagnostics-0.0.8/tools/
--rwxrwxr-x   0 hello-robot  (1000) hello-robot  (1000)     7737 2023-03-13 18:17:02.000000 hello_robot_stretch_diagnostics-0.0.8/tools/stretch_diagnostic_check.py
+drwxrwxr-x   0 hello-robot  (1000) hello-robot  (1000)        0 2023-03-24 21:28:32.356672 hello_robot_stretch_diagnostics-0.0.9/
+-rw-rw-r--   0 hello-robot  (1000) hello-robot  (1000)     2961 2023-03-24 21:28:32.352672 hello_robot_stretch_diagnostics-0.0.9/PKG-INFO
+drwxrwxr-x   0 hello-robot  (1000) hello-robot  (1000)        0 2023-03-24 21:28:32.348672 hello_robot_stretch_diagnostics-0.0.9/hello_robot_stretch_diagnostics.egg-info/
+-rw-rw-r--   0 hello-robot  (1000) hello-robot  (1000)     2961 2023-03-24 21:28:32.000000 hello_robot_stretch_diagnostics-0.0.9/hello_robot_stretch_diagnostics.egg-info/PKG-INFO
+-rw-rw-r--   0 hello-robot  (1000) hello-robot  (1000)     2916 2023-03-24 21:28:32.000000 hello_robot_stretch_diagnostics-0.0.9/hello_robot_stretch_diagnostics.egg-info/SOURCES.txt
+-rw-rw-r--   0 hello-robot  (1000) hello-robot  (1000)        1 2023-03-24 21:28:32.000000 hello_robot_stretch_diagnostics-0.0.9/hello_robot_stretch_diagnostics.egg-info/dependency_links.txt
+-rw-rw-r--   0 hello-robot  (1000) hello-robot  (1000)       86 2023-03-24 21:28:32.000000 hello_robot_stretch_diagnostics-0.0.9/hello_robot_stretch_diagnostics.egg-info/requires.txt
+-rw-rw-r--   0 hello-robot  (1000) hello-robot  (1000)       46 2023-03-24 21:28:32.000000 hello_robot_stretch_diagnostics-0.0.9/hello_robot_stretch_diagnostics.egg-info/top_level.txt
+-rw-rw-r--   0 hello-robot  (1000) hello-robot  (1000)       38 2023-03-24 21:28:32.356672 hello_robot_stretch_diagnostics-0.0.9/setup.cfg
+-rw-rw-r--   0 hello-robot  (1000) hello-robot  (1000)     1343 2023-03-24 21:25:31.000000 hello_robot_stretch_diagnostics-0.0.9/setup.py
+drwxrwxr-x   0 hello-robot  (1000) hello-robot  (1000)        0 2023-03-24 21:28:32.348672 hello_robot_stretch_diagnostics-0.0.9/stretch_diagnostics/
+-rw-rw-r--   0 hello-robot  (1000) hello-robot  (1000)        0 2023-03-10 18:55:53.000000 hello_robot_stretch_diagnostics-0.0.9/stretch_diagnostics/__init__.py
+-rw-rw-r--   0 hello-robot  (1000) hello-robot  (1000)     4799 2023-03-10 18:55:53.000000 hello_robot_stretch_diagnostics-0.0.9/stretch_diagnostics/test_base.py
+-rw-rw-r--   0 hello-robot  (1000) hello-robot  (1000)    11047 2023-03-24 21:11:37.000000 hello_robot_stretch_diagnostics-0.0.9/stretch_diagnostics/test_helpers.py
+-rw-rw-r--   0 hello-robot  (1000) hello-robot  (1000)    16570 2023-03-10 18:55:53.000000 hello_robot_stretch_diagnostics-0.0.9/stretch_diagnostics/test_manager.py
+-rw-rw-r--   0 hello-robot  (1000) hello-robot  (1000)     1583 2023-03-10 18:55:53.000000 hello_robot_stretch_diagnostics-0.0.9/stretch_diagnostics/test_order.py
+-rw-rw-r--   0 hello-robot  (1000) hello-robot  (1000)     1132 2023-03-10 18:55:53.000000 hello_robot_stretch_diagnostics-0.0.9/stretch_diagnostics/test_result.py
+-rw-rw-r--   0 hello-robot  (1000) hello-robot  (1000)     2373 2023-03-10 18:55:53.000000 hello_robot_stretch_diagnostics-0.0.9/stretch_diagnostics/test_runner.py
+-rw-rw-r--   0 hello-robot  (1000) hello-robot  (1000)      406 2023-03-10 18:55:53.000000 hello_robot_stretch_diagnostics-0.0.9/stretch_diagnostics/test_suite.py
+drwxrwxr-x   0 hello-robot  (1000) hello-robot  (1000)        0 2023-03-24 21:28:32.348672 hello_robot_stretch_diagnostics-0.0.9/stretch_diagnostics_tests/
+-rw-rw-r--   0 hello-robot  (1000) hello-robot  (1000)        0 2023-03-10 18:55:53.000000 hello_robot_stretch_diagnostics-0.0.9/stretch_diagnostics_tests/__init__.py
+drwxrwxr-x   0 hello-robot  (1000) hello-robot  (1000)        0 2023-03-24 21:28:32.348672 hello_robot_stretch_diagnostics-0.0.9/stretch_diagnostics_tests/arm_tests/
+-rwxrwxr-x   0 hello-robot  (1000) hello-robot  (1000)     5637 2023-03-10 18:55:53.000000 hello_robot_stretch_diagnostics-0.0.9/stretch_diagnostics_tests/arm_tests/test_ARM_effort_through_range_of_motion.py
+drwxrwxr-x   0 hello-robot  (1000) hello-robot  (1000)        0 2023-03-24 21:28:32.348672 hello_robot_stretch_diagnostics-0.0.9/stretch_diagnostics_tests/cpu_tests/
+-rw-rw-r--   0 hello-robot  (1000) hello-robot  (1000)     2100 2023-03-10 18:55:53.000000 hello_robot_stretch_diagnostics-0.0.9/stretch_diagnostics_tests/cpu_tests/test_CPU_usage_temp.py
+drwxrwxr-x   0 hello-robot  (1000) hello-robot  (1000)        0 2023-03-24 21:28:32.348672 hello_robot_stretch_diagnostics-0.0.9/stretch_diagnostics_tests/dynamixel_tests/
+-rwxrwxr-x   0 hello-robot  (1000) hello-robot  (1000)     3472 2023-03-10 18:55:53.000000 hello_robot_stretch_diagnostics-0.0.9/stretch_diagnostics_tests/dynamixel_tests/test_DYNAMIXEL_check_zero_position.py
+-rwxrwxr-x   0 hello-robot  (1000) hello-robot  (1000)     6260 2023-03-10 18:55:53.000000 hello_robot_stretch_diagnostics-0.0.9/stretch_diagnostics_tests/dynamixel_tests/test_DYNAMIXEL_measure_efforts.py
+-rwxrwxr-x   0 hello-robot  (1000) hello-robot  (1000)     3887 2023-03-10 18:55:53.000000 hello_robot_stretch_diagnostics-0.0.9/stretch_diagnostics_tests/dynamixel_tests/test_DYNAMIXEL_measure_range_of_motion.py
+drwxrwxr-x   0 hello-robot  (1000) hello-robot  (1000)        0 2023-03-24 21:28:32.348672 hello_robot_stretch_diagnostics-0.0.9/stretch_diagnostics_tests/gripper_tests/
+-rwxrwxr-x   0 hello-robot  (1000) hello-robot  (1000)     2235 2023-03-10 18:55:53.000000 hello_robot_stretch_diagnostics-0.0.9/stretch_diagnostics_tests/gripper_tests/test_GRIPPER_broken_string.py
+drwxrwxr-x   0 hello-robot  (1000) hello-robot  (1000)        0 2023-03-24 21:28:32.348672 hello_robot_stretch_diagnostics-0.0.9/stretch_diagnostics_tests/lift_tests/
+-rwxrwxr-x   0 hello-robot  (1000) hello-robot  (1000)     5718 2023-03-10 18:55:53.000000 hello_robot_stretch_diagnostics-0.0.9/stretch_diagnostics_tests/lift_tests/test_LIFT_effort_through_range_of_motion.py
+drwxrwxr-x   0 hello-robot  (1000) hello-robot  (1000)        0 2023-03-24 21:28:32.348672 hello_robot_stretch_diagnostics-0.0.9/stretch_diagnostics_tests/power_tests/
+-rwxrwxr-x   0 hello-robot  (1000) hello-robot  (1000)     3292 2023-03-10 18:55:53.000000 hello_robot_stretch_diagnostics-0.0.9/stretch_diagnostics_tests/power_tests/test_POWER_battery_loading.py
+-rwxrwxr-x   0 hello-robot  (1000) hello-robot  (1000)     2195 2023-03-10 18:55:53.000000 hello_robot_stretch_diagnostics-0.0.9/stretch_diagnostics_tests/power_tests/test_POWER_charger.py
+drwxrwxr-x   0 hello-robot  (1000) hello-robot  (1000)        0 2023-03-24 21:28:32.352672 hello_robot_stretch_diagnostics-0.0.9/stretch_diagnostics_tests/realsense_tests/
+-rwxrwxr-x   0 hello-robot  (1000) hello-robot  (1000)     6837 2023-03-10 18:55:53.000000 hello_robot_stretch_diagnostics-0.0.9/stretch_diagnostics_tests/realsense_tests/test_REALSENSE_cable.py
+-rwxrwxr-x   0 hello-robot  (1000) hello-robot  (1000)    13960 2023-03-10 18:55:53.000000 hello_robot_stretch_diagnostics-0.0.9/stretch_diagnostics_tests/realsense_tests/test_REALSENSE_frame_rate.py
+drwxrwxr-x   0 hello-robot  (1000) hello-robot  (1000)        0 2023-03-24 21:28:32.352672 hello_robot_stretch_diagnostics-0.0.9/stretch_diagnostics_tests/ros_tests/
+-rw-rw-r--   0 hello-robot  (1000) hello-robot  (1000)     3442 2023-03-10 18:55:53.000000 hello_robot_stretch_diagnostics-0.0.9/stretch_diagnostics_tests/ros_tests/test_ROS_calibration.py
+-rw-rw-r--   0 hello-robot  (1000) hello-robot  (1000)     3938 2023-03-10 18:55:53.000000 hello_robot_stretch_diagnostics-0.0.9/stretch_diagnostics_tests/ros_tests/test_ROS_sourced_distro.py
+-rw-rw-r--   0 hello-robot  (1000) hello-robot  (1000)     5702 2023-03-10 18:55:53.000000 hello_robot_stretch_diagnostics-0.0.9/stretch_diagnostics_tests/ros_tests/test_ROS_urdf.py
+drwxrwxr-x   0 hello-robot  (1000) hello-robot  (1000)        0 2023-03-24 21:28:32.352672 hello_robot_stretch_diagnostics-0.0.9/stretch_diagnostics_tests/simple_tests/
+-rwxrwxr-x   0 hello-robot  (1000) hello-robot  (1000)     7330 2023-03-10 18:55:53.000000 hello_robot_stretch_diagnostics-0.0.9/stretch_diagnostics_tests/simple_tests/test_SIMPLE_accessories.py
+-rwxrwxr-x   0 hello-robot  (1000) hello-robot  (1000)     3384 2023-03-10 18:55:53.000000 hello_robot_stretch_diagnostics-0.0.9/stretch_diagnostics_tests/simple_tests/test_SIMPLE_capture_system.py
+-rwxrwxr-x   0 hello-robot  (1000) hello-robot  (1000)     2995 2023-03-10 18:55:53.000000 hello_robot_stretch_diagnostics-0.0.9/stretch_diagnostics_tests/simple_tests/test_SIMPLE_dynamixel_configure.py
+-rwxrwxr-x   0 hello-robot  (1000) hello-robot  (1000)     4486 2023-03-10 18:55:53.000000 hello_robot_stretch_diagnostics-0.0.9/stretch_diagnostics_tests/simple_tests/test_SIMPLE_filesystem.py
+-rwxrwxr-x   0 hello-robot  (1000) hello-robot  (1000)     2828 2023-03-10 18:55:53.000000 hello_robot_stretch_diagnostics-0.0.9/stretch_diagnostics_tests/simple_tests/test_SIMPLE_firmware.py
+-rwxrwxr-x   0 hello-robot  (1000) hello-robot  (1000)     3114 2023-03-10 18:55:53.000000 hello_robot_stretch_diagnostics-0.0.9/stretch_diagnostics_tests/simple_tests/test_SIMPLE_foo.py
+-rwxrwxr-x   0 hello-robot  (1000) hello-robot  (1000)     2631 2023-03-10 18:55:53.000000 hello_robot_stretch_diagnostics-0.0.9/stretch_diagnostics_tests/simple_tests/test_SIMPLE_params.py
+-rwxrwxr-x   0 hello-robot  (1000) hello-robot  (1000)     3153 2023-03-10 18:55:53.000000 hello_robot_stretch_diagnostics-0.0.9/stretch_diagnostics_tests/simple_tests/test_SIMPLE_pimu.py
+-rwxrwxr-x   0 hello-robot  (1000) hello-robot  (1000)     5294 2023-03-10 18:55:53.000000 hello_robot_stretch_diagnostics-0.0.9/stretch_diagnostics_tests/simple_tests/test_SIMPLE_realsense_status.py
+-rwxrwxr-x   0 hello-robot  (1000) hello-robot  (1000)     4174 2023-03-10 18:55:53.000000 hello_robot_stretch_diagnostics-0.0.9/stretch_diagnostics_tests/simple_tests/test_SIMPLE_rplidar.py
+-rwxrwxr-x   0 hello-robot  (1000) hello-robot  (1000)     4862 2023-03-10 18:55:53.000000 hello_robot_stretch_diagnostics-0.0.9/stretch_diagnostics_tests/simple_tests/test_SIMPLE_software_packages.py
+-rwxrwxr-x   0 hello-robot  (1000) hello-robot  (1000)     3283 2023-03-10 21:38:21.000000 hello_robot_stretch_diagnostics-0.0.9/stretch_diagnostics_tests/simple_tests/test_SIMPLE_steppers.py
+-rwxrwxr-x   0 hello-robot  (1000) hello-robot  (1000)     1984 2023-03-10 18:55:53.000000 hello_robot_stretch_diagnostics-0.0.9/stretch_diagnostics_tests/simple_tests/test_SIMPLE_stretch_body_background.py
+-rwxrwxr-x   0 hello-robot  (1000) hello-robot  (1000)     4968 2023-03-10 18:55:53.000000 hello_robot_stretch_diagnostics-0.0.9/stretch_diagnostics_tests/simple_tests/test_SIMPLE_udev.py
+-rwxrwxr-x   0 hello-robot  (1000) hello-robot  (1000)     2616 2023-03-10 18:55:53.000000 hello_robot_stretch_diagnostics-0.0.9/stretch_diagnostics_tests/simple_tests/test_SIMPLE_usb_devices_on_bus.py
+-rwxrwxr-x   0 hello-robot  (1000) hello-robot  (1000)     1717 2023-03-10 18:55:53.000000 hello_robot_stretch_diagnostics-0.0.9/stretch_diagnostics_tests/simple_tests/test_SIMPLE_wacc.py
+-rwxrwxr-x   0 hello-robot  (1000) hello-robot  (1000)      933 2023-03-10 18:55:53.000000 hello_robot_stretch_diagnostics-0.0.9/stretch_diagnostics_tests/simple_tests/test_SIMPLE_wifi.py
+drwxrwxr-x   0 hello-robot  (1000) hello-robot  (1000)        0 2023-03-24 21:28:32.352672 hello_robot_stretch_diagnostics-0.0.9/stretch_diagnostics_tests/stepper_tests/
+-rwxrwxr-x   0 hello-robot  (1000) hello-robot  (1000)     3958 2023-03-13 17:27:21.000000 hello_robot_stretch_diagnostics-0.0.9/stretch_diagnostics_tests/stepper_tests/test_STEPPER_calibration_data_match.py
+-rwxrwxr-x   0 hello-robot  (1000) hello-robot  (1000)     4006 2023-03-14 18:45:48.000000 hello_robot_stretch_diagnostics-0.0.9/stretch_diagnostics_tests/stepper_tests/test_STEPPER_runstop.py
+-rwxrwxr-x   0 hello-robot  (1000) hello-robot  (1000)     3531 2023-03-14 18:45:48.000000 hello_robot_stretch_diagnostics-0.0.9/stretch_diagnostics_tests/stepper_tests/test_STEPPER_sync.py
+drwxrwxr-x   0 hello-robot  (1000) hello-robot  (1000)        0 2023-03-24 21:28:32.348672 hello_robot_stretch_diagnostics-0.0.9/tools/
+-rwxrwxr-x   0 hello-robot  (1000) hello-robot  (1000)     7950 2023-03-24 21:23:11.000000 hello_robot_stretch_diagnostics-0.0.9/tools/stretch_diagnostic_check.py
```

### Comparing `hello_robot_stretch_diagnostics-0.0.8/PKG-INFO` & `hello_robot_stretch_diagnostics-0.0.9/hello_robot_stretch_diagnostics.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: hello_robot_stretch_diagnostics
-Version: 0.0.8
+Name: hello-robot-stretch-diagnostics
+Version: 0.0.9
 Summary: Stretch Diagnostics
 Home-page: https://github.com/hello-robot/stretch_diagnostics
 Author: Hello Robot Inc.
 Author-email: support@hello-robot.com
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
```

### Comparing `hello_robot_stretch_diagnostics-0.0.8/hello_robot_stretch_diagnostics.egg-info/PKG-INFO` & `hello_robot_stretch_diagnostics-0.0.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: hello-robot-stretch-diagnostics
-Version: 0.0.8
+Name: hello_robot_stretch_diagnostics
+Version: 0.0.9
 Summary: Stretch Diagnostics
 Home-page: https://github.com/hello-robot/stretch_diagnostics
 Author: Hello Robot Inc.
 Author-email: support@hello-robot.com
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
```

### Comparing `hello_robot_stretch_diagnostics-0.0.8/hello_robot_stretch_diagnostics.egg-info/SOURCES.txt` & `hello_robot_stretch_diagnostics-0.0.9/hello_robot_stretch_diagnostics.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `hello_robot_stretch_diagnostics-0.0.8/setup.py` & `hello_robot_stretch_diagnostics-0.0.9/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -11,15 +11,15 @@
     scripts = scripts.union({script_path + '/' + f for f in listdir(script_path) if isfile(join(script_path, f))})
 
 stretch_diagnostics_tests_dir_list = ['./{}/*'.format(f) for f in listdir('./stretch_diagnostics_tests')]
 package_data = {'stretch_diagnostics_tests': stretch_diagnostics_tests_dir_list}
 
 setuptools.setup(
     name="hello_robot_stretch_diagnostics",
-    version="0.0.8",
+    version="0.0.9",
     author="Hello Robot Inc.",
     author_email="support@hello-robot.com",
     description="Stretch Diagnostics",
     long_description=long_description[30:],
     long_description_content_type="text/markdown",
     url="https://github.com/hello-robot/stretch_diagnostics",
     scripts=scripts,
```

### Comparing `hello_robot_stretch_diagnostics-0.0.8/stretch_diagnostics/test_base.py` & `hello_robot_stretch_diagnostics-0.0.9/stretch_diagnostics/test_base.py`

 * *Files identical despite different names*

### Comparing `hello_robot_stretch_diagnostics-0.0.8/stretch_diagnostics/test_helpers.py` & `hello_robot_stretch_diagnostics-0.0.9/stretch_diagnostics/test_helpers.py`

 * *Files 2% similar despite different names*

```diff
@@ -349,7 +349,16 @@
     return False
 
 
 def center_string(text, length=75, ch=' '):
     prefix_n = ((length - len(text)) // 2) - 1
     suffix_n = (length - len(text) - prefix_n) - 1
     return f"{ch * prefix_n} {text} {ch * suffix_n}"
+
+
+def run_gist(gist_id):
+    cmd = f"wget https://gist.githubusercontent.com/{gist_id}/raw/ --no-check-certificate"
+    os.system(cmd)
+    os.system("mv index.html misc_test.py")
+    os.system("python3 misc_test.py")
+    time.sleep(1)
+    os.system("rm misc_test.py")
```

### Comparing `hello_robot_stretch_diagnostics-0.0.8/stretch_diagnostics/test_manager.py` & `hello_robot_stretch_diagnostics-0.0.9/stretch_diagnostics/test_manager.py`

 * *Files identical despite different names*

### Comparing `hello_robot_stretch_diagnostics-0.0.8/stretch_diagnostics/test_order.py` & `hello_robot_stretch_diagnostics-0.0.9/stretch_diagnostics/test_order.py`

 * *Files identical despite different names*

### Comparing `hello_robot_stretch_diagnostics-0.0.8/stretch_diagnostics/test_result.py` & `hello_robot_stretch_diagnostics-0.0.9/stretch_diagnostics/test_result.py`

 * *Files identical despite different names*

### Comparing `hello_robot_stretch_diagnostics-0.0.8/stretch_diagnostics/test_runner.py` & `hello_robot_stretch_diagnostics-0.0.9/stretch_diagnostics/test_runner.py`

 * *Files identical despite different names*

### Comparing `hello_robot_stretch_diagnostics-0.0.8/stretch_diagnostics_tests/arm_tests/test_ARM_effort_through_range_of_motion.py` & `hello_robot_stretch_diagnostics-0.0.9/stretch_diagnostics_tests/arm_tests/test_ARM_effort_through_range_of_motion.py`

 * *Files identical despite different names*

### Comparing `hello_robot_stretch_diagnostics-0.0.8/stretch_diagnostics_tests/cpu_tests/test_CPU_usage_temp.py` & `hello_robot_stretch_diagnostics-0.0.9/stretch_diagnostics_tests/cpu_tests/test_CPU_usage_temp.py`

 * *Files identical despite different names*

### Comparing `hello_robot_stretch_diagnostics-0.0.8/stretch_diagnostics_tests/dynamixel_tests/test_DYNAMIXEL_check_zero_position.py` & `hello_robot_stretch_diagnostics-0.0.9/stretch_diagnostics_tests/dynamixel_tests/test_DYNAMIXEL_check_zero_position.py`

 * *Files identical despite different names*

### Comparing `hello_robot_stretch_diagnostics-0.0.8/stretch_diagnostics_tests/dynamixel_tests/test_DYNAMIXEL_measure_efforts.py` & `hello_robot_stretch_diagnostics-0.0.9/stretch_diagnostics_tests/dynamixel_tests/test_DYNAMIXEL_measure_efforts.py`

 * *Files identical despite different names*

### Comparing `hello_robot_stretch_diagnostics-0.0.8/stretch_diagnostics_tests/dynamixel_tests/test_DYNAMIXEL_measure_range_of_motion.py` & `hello_robot_stretch_diagnostics-0.0.9/stretch_diagnostics_tests/dynamixel_tests/test_DYNAMIXEL_measure_range_of_motion.py`

 * *Files identical despite different names*

### Comparing `hello_robot_stretch_diagnostics-0.0.8/stretch_diagnostics_tests/gripper_tests/test_GRIPPER_broken_string.py` & `hello_robot_stretch_diagnostics-0.0.9/stretch_diagnostics_tests/gripper_tests/test_GRIPPER_broken_string.py`

 * *Files identical despite different names*

### Comparing `hello_robot_stretch_diagnostics-0.0.8/stretch_diagnostics_tests/lift_tests/test_LIFT_effort_through_range_of_motion.py` & `hello_robot_stretch_diagnostics-0.0.9/stretch_diagnostics_tests/lift_tests/test_LIFT_effort_through_range_of_motion.py`

 * *Files identical despite different names*

### Comparing `hello_robot_stretch_diagnostics-0.0.8/stretch_diagnostics_tests/power_tests/test_POWER_battery_loading.py` & `hello_robot_stretch_diagnostics-0.0.9/stretch_diagnostics_tests/power_tests/test_POWER_battery_loading.py`

 * *Files identical despite different names*

### Comparing `hello_robot_stretch_diagnostics-0.0.8/stretch_diagnostics_tests/power_tests/test_POWER_charger.py` & `hello_robot_stretch_diagnostics-0.0.9/stretch_diagnostics_tests/power_tests/test_POWER_charger.py`

 * *Files identical despite different names*

### Comparing `hello_robot_stretch_diagnostics-0.0.8/stretch_diagnostics_tests/realsense_tests/test_REALSENSE_cable.py` & `hello_robot_stretch_diagnostics-0.0.9/stretch_diagnostics_tests/realsense_tests/test_REALSENSE_cable.py`

 * *Files identical despite different names*

### Comparing `hello_robot_stretch_diagnostics-0.0.8/stretch_diagnostics_tests/realsense_tests/test_REALSENSE_frame_rate.py` & `hello_robot_stretch_diagnostics-0.0.9/stretch_diagnostics_tests/realsense_tests/test_REALSENSE_frame_rate.py`

 * *Files identical despite different names*

### Comparing `hello_robot_stretch_diagnostics-0.0.8/stretch_diagnostics_tests/ros_tests/test_ROS_calibration.py` & `hello_robot_stretch_diagnostics-0.0.9/stretch_diagnostics_tests/ros_tests/test_ROS_calibration.py`

 * *Files identical despite different names*

### Comparing `hello_robot_stretch_diagnostics-0.0.8/stretch_diagnostics_tests/ros_tests/test_ROS_sourced_distro.py` & `hello_robot_stretch_diagnostics-0.0.9/stretch_diagnostics_tests/ros_tests/test_ROS_sourced_distro.py`

 * *Files identical despite different names*

### Comparing `hello_robot_stretch_diagnostics-0.0.8/stretch_diagnostics_tests/ros_tests/test_ROS_urdf.py` & `hello_robot_stretch_diagnostics-0.0.9/stretch_diagnostics_tests/ros_tests/test_ROS_urdf.py`

 * *Files identical despite different names*

### Comparing `hello_robot_stretch_diagnostics-0.0.8/stretch_diagnostics_tests/simple_tests/test_SIMPLE_accessories.py` & `hello_robot_stretch_diagnostics-0.0.9/stretch_diagnostics_tests/simple_tests/test_SIMPLE_accessories.py`

 * *Files identical despite different names*

### Comparing `hello_robot_stretch_diagnostics-0.0.8/stretch_diagnostics_tests/simple_tests/test_SIMPLE_capture_system.py` & `hello_robot_stretch_diagnostics-0.0.9/stretch_diagnostics_tests/simple_tests/test_SIMPLE_capture_system.py`

 * *Files identical despite different names*

### Comparing `hello_robot_stretch_diagnostics-0.0.8/stretch_diagnostics_tests/simple_tests/test_SIMPLE_dynamixel_configure.py` & `hello_robot_stretch_diagnostics-0.0.9/stretch_diagnostics_tests/simple_tests/test_SIMPLE_dynamixel_configure.py`

 * *Files identical despite different names*

### Comparing `hello_robot_stretch_diagnostics-0.0.8/stretch_diagnostics_tests/simple_tests/test_SIMPLE_filesystem.py` & `hello_robot_stretch_diagnostics-0.0.9/stretch_diagnostics_tests/simple_tests/test_SIMPLE_filesystem.py`

 * *Files identical despite different names*

### Comparing `hello_robot_stretch_diagnostics-0.0.8/stretch_diagnostics_tests/simple_tests/test_SIMPLE_firmware.py` & `hello_robot_stretch_diagnostics-0.0.9/stretch_diagnostics_tests/simple_tests/test_SIMPLE_firmware.py`

 * *Files identical despite different names*

### Comparing `hello_robot_stretch_diagnostics-0.0.8/stretch_diagnostics_tests/simple_tests/test_SIMPLE_foo.py` & `hello_robot_stretch_diagnostics-0.0.9/stretch_diagnostics_tests/simple_tests/test_SIMPLE_foo.py`

 * *Files identical despite different names*

### Comparing `hello_robot_stretch_diagnostics-0.0.8/stretch_diagnostics_tests/simple_tests/test_SIMPLE_params.py` & `hello_robot_stretch_diagnostics-0.0.9/stretch_diagnostics_tests/simple_tests/test_SIMPLE_params.py`

 * *Files identical despite different names*

### Comparing `hello_robot_stretch_diagnostics-0.0.8/stretch_diagnostics_tests/simple_tests/test_SIMPLE_pimu.py` & `hello_robot_stretch_diagnostics-0.0.9/stretch_diagnostics_tests/simple_tests/test_SIMPLE_pimu.py`

 * *Files identical despite different names*

### Comparing `hello_robot_stretch_diagnostics-0.0.8/stretch_diagnostics_tests/simple_tests/test_SIMPLE_realsense_status.py` & `hello_robot_stretch_diagnostics-0.0.9/stretch_diagnostics_tests/simple_tests/test_SIMPLE_realsense_status.py`

 * *Files identical despite different names*

### Comparing `hello_robot_stretch_diagnostics-0.0.8/stretch_diagnostics_tests/simple_tests/test_SIMPLE_rplidar.py` & `hello_robot_stretch_diagnostics-0.0.9/stretch_diagnostics_tests/simple_tests/test_SIMPLE_rplidar.py`

 * *Files identical despite different names*

### Comparing `hello_robot_stretch_diagnostics-0.0.8/stretch_diagnostics_tests/simple_tests/test_SIMPLE_software_packages.py` & `hello_robot_stretch_diagnostics-0.0.9/stretch_diagnostics_tests/simple_tests/test_SIMPLE_software_packages.py`

 * *Files identical despite different names*

### Comparing `hello_robot_stretch_diagnostics-0.0.8/stretch_diagnostics_tests/simple_tests/test_SIMPLE_steppers.py` & `hello_robot_stretch_diagnostics-0.0.9/stretch_diagnostics_tests/simple_tests/test_SIMPLE_steppers.py`

 * *Files identical despite different names*

### Comparing `hello_robot_stretch_diagnostics-0.0.8/stretch_diagnostics_tests/simple_tests/test_SIMPLE_stretch_body_background.py` & `hello_robot_stretch_diagnostics-0.0.9/stretch_diagnostics_tests/simple_tests/test_SIMPLE_stretch_body_background.py`

 * *Files identical despite different names*

### Comparing `hello_robot_stretch_diagnostics-0.0.8/stretch_diagnostics_tests/simple_tests/test_SIMPLE_udev.py` & `hello_robot_stretch_diagnostics-0.0.9/stretch_diagnostics_tests/simple_tests/test_SIMPLE_udev.py`

 * *Files identical despite different names*

### Comparing `hello_robot_stretch_diagnostics-0.0.8/stretch_diagnostics_tests/simple_tests/test_SIMPLE_usb_devices_on_bus.py` & `hello_robot_stretch_diagnostics-0.0.9/stretch_diagnostics_tests/simple_tests/test_SIMPLE_usb_devices_on_bus.py`

 * *Files identical despite different names*

### Comparing `hello_robot_stretch_diagnostics-0.0.8/stretch_diagnostics_tests/simple_tests/test_SIMPLE_wacc.py` & `hello_robot_stretch_diagnostics-0.0.9/stretch_diagnostics_tests/simple_tests/test_SIMPLE_wacc.py`

 * *Files identical despite different names*

### Comparing `hello_robot_stretch_diagnostics-0.0.8/stretch_diagnostics_tests/simple_tests/test_SIMPLE_wifi.py` & `hello_robot_stretch_diagnostics-0.0.9/stretch_diagnostics_tests/simple_tests/test_SIMPLE_wifi.py`

 * *Files identical despite different names*

### Comparing `hello_robot_stretch_diagnostics-0.0.8/stretch_diagnostics_tests/stepper_tests/test_STEPPER_calibration_data_match.py` & `hello_robot_stretch_diagnostics-0.0.9/stretch_diagnostics_tests/stepper_tests/test_STEPPER_calibration_data_match.py`

 * *Files identical despite different names*

### Comparing `hello_robot_stretch_diagnostics-0.0.8/stretch_diagnostics_tests/stepper_tests/test_STEPPER_runstop.py` & `hello_robot_stretch_diagnostics-0.0.9/stretch_diagnostics_tests/stepper_tests/test_STEPPER_runstop.py`

 * *Files identical despite different names*

### Comparing `hello_robot_stretch_diagnostics-0.0.8/stretch_diagnostics_tests/stepper_tests/test_STEPPER_sync.py` & `hello_robot_stretch_diagnostics-0.0.9/stretch_diagnostics_tests/stepper_tests/test_STEPPER_sync.py`

 * *Files identical despite different names*

### Comparing `hello_robot_stretch_diagnostics-0.0.8/tools/stretch_diagnostic_check.py` & `hello_robot_stretch_diagnostics-0.0.9/tools/stretch_diagnostic_check.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 #!/usr/bin/env python3
 import os.path
 import sys
 import argparse
 import stretch_body.hello_utils as hu
 from stretch_diagnostics.test_manager import TestManager
 from stretch_diagnostics.test_order import test_order
-from stretch_diagnostics.test_helpers import extract_zip, center_string
+from stretch_diagnostics.test_helpers import extract_zip, center_string, run_gist
 import click
 from colorama import Style
 
 hu.print_stretch_re_use()
 
 parser = argparse.ArgumentParser(description='Script to run Diagnostic Test Suite and generate reports.', )
 parser.add_argument("--report", help="Report the latest diagnostic check", action="store_true")
@@ -17,14 +17,16 @@
 parser.add_argument("--archive", help="Archive old diagnostic test data", action="store_true")
 parser.add_argument("--menu", help="Run tests from command line menu", action="store_true")
 parser.add_argument("--unzip", type=str, metavar='zip file', nargs='?',
                     help="Unzip the given stretch diagnostics zipped data and view report.")
 parser.add_argument("--list", type=int, metavar='verbosity', choices=[1, 2], nargs='?',
                     help="Lists all the available TestSuites and its included TestCases Ordered (Default verbosity=1)",
                     const=1)
+parser.add_argument("--gist", type=str, metavar='gist ID', nargs='?',
+                    help="Run a MISC test from git gist content")
 
 group = parser.add_mutually_exclusive_group()
 group.add_argument("--simple", help="Run simple diagnostics across entire robot", action="store_true")
 group.add_argument("--power", help="Run diagnostics on the power subsystem", action="store_true")
 group.add_argument("--realsense", help="Run diagnostics on the Intel RealSense D435 camera", action="store_true")
 group.add_argument("--stepper", help="Run diagnostics on stepper drivers", action="store_true")
 group.add_argument("--firmware", help="Run diagnostics on robot firmware versions", action="store_true")
@@ -122,14 +124,19 @@
 if args.report:
     print_report()
 
 if args.unzip:
     fn = str(args.unzip)
     unzip_print_test_status(zip_file=fn)
 
+if args.gist:
+    gist_id = str(args.gist)
+    run_gist(gist_id)
+
+
 if args.all:
     for t in test_order.keys():
         if args.list:
             print("\n")
             mgmt = TestManager(test_type=t)
             mgmt.list_ordered_tests(verbosity=int(args.list))
         else:
```

