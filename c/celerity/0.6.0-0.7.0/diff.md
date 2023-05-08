# Comparing `tmp/celerity-0.6.0.tar.gz` & `tmp/celerity-0.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "celerity-0.6.0.tar", max compression
+gzip compressed data, was "celerity-0.7.0.tar", max compression
```

## Comparing `celerity-0.6.0.tar` & `celerity-0.7.0.tar`

### file list

```diff
@@ -1,16 +1,16 @@
--rw-r--r--   0        0        0     1075 2023-05-06 18:42:31.018552 celerity-0.6.0/LICENSE
--rw-r--r--   0        0        0     5469 2023-05-06 18:42:31.018552 celerity-0.6.0/README.md
--rw-r--r--   0        0        0     1830 2023-05-06 18:42:31.018552 celerity-0.6.0/pyproject.toml
--rw-r--r--   0        0        0      133 2023-05-06 18:42:31.018552 celerity-0.6.0/src/celerity/__init__.py
--rw-r--r--   0        0        0     2501 2023-05-06 18:42:31.018552 celerity-0.6.0/src/celerity/astrometry.py
--rw-r--r--   0        0        0      240 2023-05-06 18:42:31.018552 celerity-0.6.0/src/celerity/common.py
--rw-r--r--   0        0        0      997 2023-05-06 18:42:31.018552 celerity-0.6.0/src/celerity/constants.py
--rw-r--r--   0        0        0     1650 2023-05-06 18:42:31.018552 celerity-0.6.0/src/celerity/coordinates.py
--rw-r--r--   0        0        0      628 2023-05-06 18:42:31.018552 celerity-0.6.0/src/celerity/earth.py
--rw-r--r--   0        0        0      468 2023-05-06 18:42:31.018552 celerity-0.6.0/src/celerity/epoch.py
--rw-r--r--   0        0        0      945 2023-05-06 18:42:31.018552 celerity-0.6.0/src/celerity/moon.py
--rw-r--r--   0        0        0     2092 2023-05-06 18:42:31.018552 celerity-0.6.0/src/celerity/seeing.py
--rw-r--r--   0        0        0     2789 2023-05-06 18:42:31.018552 celerity-0.6.0/src/celerity/sun.py
--rw-r--r--   0        0        0     4129 2023-05-06 18:42:31.018552 celerity-0.6.0/src/celerity/temporal.py
--rw-r--r--   0        0        0      961 2023-05-06 18:42:31.018552 celerity-0.6.0/src/celerity/utilities.py
--rw-r--r--   0        0        0     6102 1970-01-01 00:00:00.000000 celerity-0.6.0/PKG-INFO
+-rw-r--r--   0        0        0     1075 2023-05-08 18:48:19.935014 celerity-0.7.0/LICENSE
+-rw-r--r--   0        0        0     5469 2023-05-08 18:48:19.935014 celerity-0.7.0/README.md
+-rw-r--r--   0        0        0     1846 2023-05-08 18:48:19.935014 celerity-0.7.0/pyproject.toml
+-rw-r--r--   0        0        0      133 2023-05-08 18:48:19.935014 celerity-0.7.0/src/celerity/__init__.py
+-rw-r--r--   0        0        0     2418 2023-05-08 18:48:19.935014 celerity-0.7.0/src/celerity/astrometry.py
+-rw-r--r--   0        0        0      240 2023-05-08 18:48:19.935014 celerity-0.7.0/src/celerity/common.py
+-rw-r--r--   0        0        0      997 2023-05-08 18:48:19.935014 celerity-0.7.0/src/celerity/constants.py
+-rw-r--r--   0        0        0     1354 2023-05-08 18:48:19.935014 celerity-0.7.0/src/celerity/coordinates.py
+-rw-r--r--   0        0        0      632 2023-05-08 18:48:19.935014 celerity-0.7.0/src/celerity/earth.py
+-rw-r--r--   0        0        0      468 2023-05-08 18:48:19.935014 celerity-0.7.0/src/celerity/epoch.py
+-rw-r--r--   0        0        0     2479 2023-05-08 18:48:19.935014 celerity-0.7.0/src/celerity/moon.py
+-rw-r--r--   0        0        0     2049 2023-05-08 18:48:19.935014 celerity-0.7.0/src/celerity/seeing.py
+-rw-r--r--   0        0        0     2688 2023-05-08 18:48:19.935014 celerity-0.7.0/src/celerity/sun.py
+-rw-r--r--   0        0        0     4125 2023-05-08 18:48:19.935014 celerity-0.7.0/src/celerity/temporal.py
+-rw-r--r--   0        0        0      961 2023-05-08 18:48:19.935014 celerity-0.7.0/src/celerity/utilities.py
+-rw-r--r--   0        0        0     6102 1970-01-01 00:00:00.000000 celerity-0.7.0/PKG-INFO
```

### Comparing `celerity-0.6.0/LICENSE` & `celerity-0.7.0/LICENSE`

 * *Files identical despite different names*

### Comparing `celerity-0.6.0/README.md` & `celerity-0.7.0/README.md`

 * *Files identical despite different names*

### Comparing `celerity-0.6.0/pyproject.toml` & `celerity-0.7.0/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "celerity"
-version = "0.6.0"
+version = "0.7.0"
 description = "Celerity is a lightweight, zero-dependency and type-safe Python library for astronomical calculations."
 authors = [
     "Michael J. Roberts <michael@observerly.com>"
 ]
 maintainers = [
     "Michael J. Roberts <michael@observerly.com>"
 ]
@@ -17,14 +17,15 @@
 python = "^3.11"
 
 
 [tool.poetry.group.dev.dependencies]
 ruff = "^0.0.263"
 black = "^23.3.0"
 pytest = "^7.3.1"
+mypy = "^1.2.0"
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.ruff]
 # Enable pycodestyle (`E`) and Pyflakes (`F`) codes by default.
```

### Comparing `celerity-0.6.0/src/celerity/astrometry.py` & `celerity-0.7.0/src/celerity/astrometry.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,9 +1,9 @@
-import math
 from datetime import datetime
+from math import atan2, cos, degrees, pow, radians, sin, tan
 
 from .common import EquatorialCoordinate, GeographicCoordinate
 from .temporal import get_julian_date, get_local_sidereal_time
 
 
 def get_hour_angle(date: datetime, ra: float, longitude: float) -> float:
     """
@@ -38,18 +38,15 @@
     # Get the Julian date:
     JD = get_julian_date(date)
 
     # Calculate the number of centuries since J2000.0:
     T = (JD - 2451545.0) / 36525
 
     # Calculate the obliquity of the ecliptic:
-    return (
-        23.439292
-        - (46.845 * T + 0.00059 * math.pow(T, 2) + 0.001813 * math.pow(T, 3)) / 3600
-    )
+    return 23.439292 - (46.845 * T + 0.00059 * pow(T, 2) + 0.001813 * pow(T, 3)) / 3600
 
 
 def get_parallactic_angle(
     date: datetime,
     observer: GeographicCoordinate,
     target: EquatorialCoordinate,
 ) -> float:
@@ -57,22 +54,21 @@
     Gets the parallactic angle for a particular object for a particular observer at a given datetime
 
     :param date: The datetime object to convert.
     :param observer: The geographic coordinate of the observer.
     :param target: The equatorial coordinate of the observed object.
     :return The parallactic angle in degrees.
     """
-    lat, lon = observer["lat"], observer["lon"]
+    lat, lon = radians(observer["lat"]), observer["lon"]
 
-    ra, dec = target["ra"], target["dec"]
+    dec = radians(target["dec"])
 
     # Get the hour angle for the target:
-    ha = get_hour_angle(date, ra, lon)
+    ha = radians(get_hour_angle(date, target["ra"], lon))
 
     # Calculate the parallactic angle and return in degrees:
-    return math.degrees(
-        math.atan2(
-            math.sin(math.radians(ha)),
-            math.tan(math.radians(lat)) * math.cos(math.radians(dec))
-            - math.sin(math.radians(dec)) * math.cos(math.radians(ha)),
+    return degrees(
+        atan2(
+            sin(ha),
+            tan(lat) * cos(dec) - sin(dec) * cos(ha),
         )
     )
```

### Comparing `celerity-0.6.0/src/celerity/constants.py` & `celerity-0.7.0/src/celerity/constants.py`

 * *Files identical despite different names*

### Comparing `celerity-0.6.0/src/celerity/seeing.py` & `celerity-0.7.0/src/celerity/seeing.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-import math
+from math import pow, radians, sin
 
 
 def get_airmass(altitude: float) -> float:
     """
     Gets the airmass of an object at a given altitude using Pickering's formula.
 
     Airmass is a measure of the amount of air along the line of sight when observing a star
@@ -24,28 +24,23 @@
     or other celestial source from below Earth's atmosphere. It is formulated
     as the integral of air density along the light ray.
 
     :see: Pickering, K. A. (2002). "The Southern Limits of the Ancient Star Catalog" (PDF). DIO. 12 (1): 20-39.
     :param: altitude: The altitude of the object in degrees.
     :return: The airmass of the object.
     """
-    return 1 / math.sin(
-        math.radians(altitude + 244 / (165 + (47 * math.pow(altitude, 1.1))))
-    )
+    return 1 / sin(radians(altitude + 244 / (165 + (47 * pow(altitude, 1.1)))))
 
 
 def get_airmass_karstenyoung(altitude: float) -> float:
     """
     Gets the airmass of an object at a given altitude using Karsten & Young's formula.
 
     Airmass is a measure of the amount of air along the line of sight when observing a star
     or other celestial source from below Earth's atmosphere. It is formulated
     as the integral of air density along the light ray.
 
     :see: Kasten, F.; Young, A. T. (1989). "Revised optical air mass tables and approximation formula". Applied Optics. 28 (22): 4735-4738.
     :param: altitude: The altitude of the object in degrees.
     :return: The airmass of the object.
     """
-    return 1 / (
-        math.sin(math.radians(altitude))
-        + 0.50572 * math.pow(altitude + 6.07995, -1.6364)
-    )
+    return 1 / (sin(radians(altitude)) + 0.50572 * pow(altitude + 6.07995, -1.6364))
```

### Comparing `celerity-0.6.0/src/celerity/sun.py` & `celerity-0.7.0/src/celerity/sun.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,11 +1,10 @@
-import math
 from datetime import datetime
+from math import pow, radians, sin
 
-from .epoch import get_number_of_fractional_days_since_j2000
 from .temporal import get_julian_date
 
 
 def get_equation_of_center(date) -> float:
     """
     The equation of center is the difference between the mean geometric longitude
     and the mean anomaly.
@@ -20,18 +19,17 @@
     T = (JD - 2451545.0) / 36525
 
     # Get the mean anomaly:
     M = get_mean_anomaly(date)
 
     # Calculate the equation of center:
     C = (
-        (1.914602 - 0.004817 * math.pow(T, 2) - 0.000014 * math.pow(T, 3))
-        * math.sin(math.radians(M))
-        + (0.019993 - 0.000101 * math.pow(T, 2)) * math.sin(math.radians(2 * M))
-        + 0.000289 * math.sin(math.radians(3 * M))
+        (1.914602 - 0.004817 * pow(T, 2) - 0.000014 * pow(T, 3)) * sin(radians(M))
+        + (0.019993 - 0.000101 * pow(T, 2)) * sin(radians(2 * M))
+        + 0.000289 * sin(radians(3 * M))
     )
 
     return C
 
 
 def get_mean_anomaly(date: datetime) -> float:
     """
@@ -44,15 +42,15 @@
     # Get the Julian date:
     JD = get_julian_date(date)
 
     # Calculate the number of centuries since J2000.0:
     T = (JD - 2451545.0) / 36525
 
     # Get the Sun's mean anomaly at the current epoch relative to J2000:
-    M = (357.52911 + 35999.05029 * T - 0.0001537 * math.pow(T, 2)) % 360
+    M = (357.52911 + 35999.05029 * T - 0.0001537 * pow(T, 2)) % 360
 
     # Correct for negative angles
     if M < 0:
         M += 360
 
     return M
 
@@ -68,15 +66,15 @@
     # Get the Julian date:
     JD = get_julian_date(date)
 
     # Calculate the number of centuries since J2000.0:
     T = (JD - 2451545.0) / 36525
 
     # Calculate the mean geometric longitude:
-    L = (280.46646 + 36000.76983 * T + 0.0003032 * math.pow(T, 2)) % 360
+    L = (280.46646 + 36000.76983 * T + 0.0003032 * pow(T, 2)) % 360
 
     # Correct for negative angles
     if L < 0:
         L += 360
 
     return L
```

### Comparing `celerity-0.6.0/src/celerity/temporal.py` & `celerity-0.7.0/src/celerity/temporal.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,9 +1,9 @@
-import math
 from datetime import datetime, timezone
+from math import floor, pow
 
 from .constants import J1900, J2000
 
 
 def get_julian_date(date: datetime) -> float:
     """
     The Julian date (JD) of any instant is the Julian day number
@@ -42,21 +42,21 @@
     equinox, the ascending node of the ecliptic on the celestial equator.
 
     :param date: The datetime object to convert.
     :return: The Greenwich Sidereal Time (GST) of the given date normalised to UTC.
     """
     JD = get_julian_date(date)
 
-    JD_0 = math.floor(JD - 0.5) + 0.5
+    JD_0 = floor(JD - 0.5) + 0.5
 
     S = JD_0 - J2000
 
     T = S / 36525.0
 
-    T_0 = (6.697374558 + 2400.051336 * T + 0.000025862 * math.pow(T, 2)) % 24
+    T_0 = (6.697374558 + 2400.051336 * T + 0.000025862 * pow(T, 2)) % 24
 
     if T_0 < 0:
         T_0 += 24
 
     # Ensure that the date is in UTC
     d = date.astimezone(tz=timezone.utc)
 
@@ -81,15 +81,15 @@
     :param longitude: The longitude of the observer.
     :return: The Local Sidereal Time (LST) of the given date normalised to UTC.
     """
     GST = get_greenwhich_sidereal_time(date.astimezone(tz=timezone.utc))
 
     d = (GST + longitude / 15.0) / 24.0
 
-    d = d - math.floor(d)
+    d = d - floor(d)
 
     if d < 0:
         d += 1
 
     return 24.0 * d
 
 
@@ -126,15 +126,15 @@
 
     # Get the number of days since 1st January for the current year:
     days = JD - JD_0
 
     # Get the number of Julian Centuries since 1900:
     T = (JD_0 - J1900) / 36525
 
-    R = 6.6460656 + 2400.051262 * T + 0.00002581 * math.pow(T, 2)
+    R = 6.6460656 + 2400.051262 * T + 0.00002581 * pow(T, 2)
 
     B = 24 - R + 24 * (year - 1900)
 
     T_0 = 0.0657098 * days - B
 
     if T_0 < 0:
         T_0 += 24
```

### Comparing `celerity-0.6.0/src/celerity/utilities.py` & `celerity-0.7.0/src/celerity/utilities.py`

 * *Files identical despite different names*

### Comparing `celerity-0.6.0/PKG-INFO` & `celerity-0.7.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: celerity
-Version: 0.6.0
+Version: 0.7.0
 Summary: Celerity is a lightweight, zero-dependency and type-safe Python library for astronomical calculations.
 Home-page: https://github.com/michaelroberts/celerity
 Keywords: astronomy,astrometry,ephemeris
 Author: Michael J. Roberts
 Author-email: michael@observerly.com
 Maintainer: Michael J. Roberts
 Maintainer-email: michael@observerly.com
```

