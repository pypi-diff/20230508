# Comparing `tmp/mikro_napari-0.1.50.tar.gz` & `tmp/mikro_napari-0.1.51.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mikro_napari-0.1.50.tar", max compression
+gzip compressed data, was "mikro_napari-0.1.51.tar", max compression
```

## Comparing `mikro_napari-0.1.50.tar` & `mikro_napari-0.1.51.tar`

### file list

```diff
@@ -1,18 +1,19 @@
--rw-r--r--   0        0        0     1318 2022-10-11 12:19:03.583911 mikro_napari-0.1.50/README.md
--rw-r--r--   0        0        0    77515 2023-03-03 14:34:51.946512 mikro_napari-0.1.50/mikro_napari/api/schema.py
--rw-r--r--   0        0        0      480 2022-10-11 12:19:03.583911 mikro_napari-0.1.50/mikro_napari/api/structures.py
--rw-r--r--   0        0        0        0 2022-10-11 12:19:03.587911 mikro_napari-0.1.50/mikro_napari/container/__init__.py
--rw-r--r--   0        0        0      299 2023-03-04 18:17:50.027023 mikro_napari-0.1.50/mikro_napari/container/base.py
--rw-r--r--   0        0        0    13673 2023-03-04 18:17:50.027023 mikro_napari-0.1.50/mikro_napari/models/representation.py
--rw-r--r--   0        0        0      289 2023-02-15 17:47:06.550532 mikro_napari-0.1.50/mikro_napari/napari.yaml
--rw-r--r--   0        0        0      443 2023-03-04 18:17:50.027023 mikro_napari-0.1.50/mikro_napari/plugin.py
--rw-r--r--   0        0        0     1028 2023-03-04 18:26:00.707074 mikro_napari-0.1.50/mikro_napari/run.py
--rw-r--r--   0        0        0      701 2022-10-11 12:19:03.587911 mikro_napari-0.1.50/mikro_napari/utils.py
--rw-r--r--   0        0        0        0 2022-03-25 12:04:03.354310 mikro_napari-0.1.50/mikro_napari/widgets/dialogs/__init__.py
--rw-r--r--   0        0        0     2680 2022-03-28 15:11:00.264225 mikro_napari-0.1.50/mikro_napari/widgets/dialogs/open_image.py
--rw-r--r--   0        0        0        0 2022-10-11 12:19:03.587911 mikro_napari-0.1.50/mikro_napari/widgets/dialogs/show_roi.py
--rw-r--r--   0        0        0     8442 2023-03-04 18:17:50.027023 mikro_napari-0.1.50/mikro_napari/widgets/main_widget.py
--rw-r--r--   0        0        0        0 2022-10-11 12:19:03.587911 mikro_napari-0.1.50/mikro_napari/widgets/sidebar/__init__.py
--rw-r--r--   0        0        0     1966 2023-03-04 18:17:50.027023 mikro_napari-0.1.50/mikro_napari/widgets/sidebar/sidebar.py
--rw-r--r--   0        0        0     1881 2023-03-04 18:27:33.347084 mikro_napari-0.1.50/pyproject.toml
--rw-r--r--   0        0        0     2104 1970-01-01 00:00:00.000000 mikro_napari-0.1.50/PKG-INFO
+-rw-r--r--   0        0        0     1318 2023-05-05 21:12:55.597194 mikro_napari-0.1.51/README.md
+-rw-r--r--   0        0        0        0 2023-05-08 18:04:36.280895 mikro_napari-0.1.51/mikro_napari/__init__.py
+-rw-r--r--   0        0        0    99909 2023-05-08 18:04:36.281344 mikro_napari-0.1.51/mikro_napari/api/schema.py
+-rw-r--r--   0        0        0      480 2023-05-05 21:12:55.598314 mikro_napari-0.1.51/mikro_napari/api/structures.py
+-rw-r--r--   0        0        0        0 2023-05-05 21:12:55.598358 mikro_napari-0.1.51/mikro_napari/container/__init__.py
+-rw-r--r--   0        0        0      299 2023-05-05 21:12:55.598412 mikro_napari-0.1.51/mikro_napari/container/base.py
+-rw-r--r--   0        0        0    25874 2023-05-08 18:33:40.432878 mikro_napari-0.1.51/mikro_napari/models/representation.py
+-rw-r--r--   0        0        0      289 2023-05-05 21:12:55.598590 mikro_napari-0.1.51/mikro_napari/napari.yaml
+-rw-r--r--   0        0        0      497 2023-05-08 20:13:38.943805 mikro_napari-0.1.51/mikro_napari/plugin.py
+-rw-r--r--   0        0        0     1028 2023-05-05 21:12:55.598699 mikro_napari-0.1.51/mikro_napari/run.py
+-rw-r--r--   0        0        0      701 2023-05-05 21:12:55.598752 mikro_napari-0.1.51/mikro_napari/utils.py
+-rw-r--r--   0        0        0        0 2023-05-05 21:12:55.598837 mikro_napari-0.1.51/mikro_napari/widgets/dialogs/__init__.py
+-rw-r--r--   0        0        0     2680 2023-05-05 21:12:55.598902 mikro_napari-0.1.51/mikro_napari/widgets/dialogs/open_image.py
+-rw-r--r--   0        0        0        0 2023-05-05 21:12:55.598924 mikro_napari-0.1.51/mikro_napari/widgets/dialogs/show_roi.py
+-rw-r--r--   0        0        0     8437 2023-05-08 18:04:36.281814 mikro_napari-0.1.51/mikro_napari/widgets/main_widget.py
+-rw-r--r--   0        0        0        0 2023-05-05 21:12:55.599062 mikro_napari-0.1.51/mikro_napari/widgets/sidebar/__init__.py
+-rw-r--r--   0        0        0     5926 2023-05-08 18:04:36.281970 mikro_napari-0.1.51/mikro_napari/widgets/sidebar/sidebar.py
+-rw-r--r--   0        0        0     1921 2023-05-08 20:19:30.440575 mikro_napari-0.1.51/pyproject.toml
+-rw-r--r--   0        0        0     2160 1970-01-01 00:00:00.000000 mikro_napari-0.1.51/PKG-INFO
```

### Comparing `mikro_napari-0.1.50/README.md` & `mikro_napari-0.1.51/README.md`

 * *Files identical despite different names*

### Comparing `mikro_napari-0.1.50/mikro_napari/api/schema.py` & `mikro_napari-0.1.51/mikro_napari/api/schema.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,15 +1,23 @@
-from typing import Optional, Iterator, AsyncIterator, Literal, List, Tuple, Dict
-from mikro.funcs import execute, asubscribe, aexecute, subscribe
+from mikro.scalars import Store, AffineMatrix, AssignationID, FeatureValue, MetricValue
+from datetime import datetime
+from mikro.funcs import aexecute, asubscribe, subscribe, execute
 from mikro.rath import MikroRath
-from mikro.traits import Vectorizable, ROI, Representation
-from mikro.scalars import AffineMatrix, FeatureValue, Store
-from pydantic import BaseModel, Field
+from pydantic import Field, BaseModel
+from typing import Iterator, Tuple, Dict, Literal, AsyncIterator, List, Optional
+from mikro.traits import (
+    Vectorizable,
+    PhysicalSize,
+    Stage,
+    Position,
+    Omero,
+    ROI,
+    Representation,
+)
 from rath.scalars import ID
-from datetime import datetime
 from enum import Enum
 
 
 class CommentableModels(str, Enum):
     GRUNNLAG_USERMETA = "GRUNNLAG_USERMETA"
     GRUNNLAG_ANTIBODY = "GRUNNLAG_ANTIBODY"
     GRUNNLAG_OBJECTIVE = "GRUNNLAG_OBJECTIVE"
@@ -21,19 +29,25 @@
     GRUNNLAG_DATALINK = "GRUNNLAG_DATALINK"
     GRUNNLAG_EXPERIMENTALGROUP = "GRUNNLAG_EXPERIMENTALGROUP"
     GRUNNLAG_ANIMAL = "GRUNNLAG_ANIMAL"
     GRUNNLAG_OMEROFILE = "GRUNNLAG_OMEROFILE"
     GRUNNLAG_MODEL = "GRUNNLAG_MODEL"
     GRUNNLAG_SAMPLE = "GRUNNLAG_SAMPLE"
     GRUNNLAG_STAGE = "GRUNNLAG_STAGE"
+    GRUNNLAG_CHANNEL = "GRUNNLAG_CHANNEL"
     GRUNNLAG_POSITION = "GRUNNLAG_POSITION"
+    GRUNNLAG_ERA = "GRUNNLAG_ERA"
+    GRUNNLAG_TIMEPOINT = "GRUNNLAG_TIMEPOINT"
     GRUNNLAG_REPRESENTATION = "GRUNNLAG_REPRESENTATION"
     GRUNNLAG_OMERO = "GRUNNLAG_OMERO"
+    GRUNNLAG_DIMENSIONMAP = "GRUNNLAG_DIMENSIONMAP"
+    GRUNNLAG_VIEW = "GRUNNLAG_VIEW"
     GRUNNLAG_METRIC = "GRUNNLAG_METRIC"
     GRUNNLAG_THUMBNAIL = "GRUNNLAG_THUMBNAIL"
+    GRUNNLAG_VIDEO = "GRUNNLAG_VIDEO"
     GRUNNLAG_ROI = "GRUNNLAG_ROI"
     GRUNNLAG_LABEL = "GRUNNLAG_LABEL"
     GRUNNLAG_FEATURE = "GRUNNLAG_FEATURE"
     BORD_TABLE = "BORD_TABLE"
 
 
 class SharableModels(str, Enum):
@@ -50,19 +64,25 @@
     GRUNNLAG_DATALINK = "GRUNNLAG_DATALINK"
     GRUNNLAG_EXPERIMENTALGROUP = "GRUNNLAG_EXPERIMENTALGROUP"
     GRUNNLAG_ANIMAL = "GRUNNLAG_ANIMAL"
     GRUNNLAG_OMEROFILE = "GRUNNLAG_OMEROFILE"
     GRUNNLAG_MODEL = "GRUNNLAG_MODEL"
     GRUNNLAG_SAMPLE = "GRUNNLAG_SAMPLE"
     GRUNNLAG_STAGE = "GRUNNLAG_STAGE"
+    GRUNNLAG_CHANNEL = "GRUNNLAG_CHANNEL"
     GRUNNLAG_POSITION = "GRUNNLAG_POSITION"
+    GRUNNLAG_ERA = "GRUNNLAG_ERA"
+    GRUNNLAG_TIMEPOINT = "GRUNNLAG_TIMEPOINT"
     GRUNNLAG_REPRESENTATION = "GRUNNLAG_REPRESENTATION"
     GRUNNLAG_OMERO = "GRUNNLAG_OMERO"
+    GRUNNLAG_DIMENSIONMAP = "GRUNNLAG_DIMENSIONMAP"
+    GRUNNLAG_VIEW = "GRUNNLAG_VIEW"
     GRUNNLAG_METRIC = "GRUNNLAG_METRIC"
     GRUNNLAG_THUMBNAIL = "GRUNNLAG_THUMBNAIL"
+    GRUNNLAG_VIDEO = "GRUNNLAG_VIDEO"
     GRUNNLAG_ROI = "GRUNNLAG_ROI"
     GRUNNLAG_LABEL = "GRUNNLAG_LABEL"
     GRUNNLAG_FEATURE = "GRUNNLAG_FEATURE"
     BORD_TABLE = "BORD_TABLE"
 
 
 class LokClientGrantType(str, Enum):
@@ -108,19 +128,25 @@
     GRUNNLAG_DATALINK = "GRUNNLAG_DATALINK"
     GRUNNLAG_EXPERIMENTALGROUP = "GRUNNLAG_EXPERIMENTALGROUP"
     GRUNNLAG_ANIMAL = "GRUNNLAG_ANIMAL"
     GRUNNLAG_OMEROFILE = "GRUNNLAG_OMEROFILE"
     GRUNNLAG_MODEL = "GRUNNLAG_MODEL"
     GRUNNLAG_SAMPLE = "GRUNNLAG_SAMPLE"
     GRUNNLAG_STAGE = "GRUNNLAG_STAGE"
+    GRUNNLAG_CHANNEL = "GRUNNLAG_CHANNEL"
     GRUNNLAG_POSITION = "GRUNNLAG_POSITION"
+    GRUNNLAG_ERA = "GRUNNLAG_ERA"
+    GRUNNLAG_TIMEPOINT = "GRUNNLAG_TIMEPOINT"
     GRUNNLAG_REPRESENTATION = "GRUNNLAG_REPRESENTATION"
     GRUNNLAG_OMERO = "GRUNNLAG_OMERO"
+    GRUNNLAG_DIMENSIONMAP = "GRUNNLAG_DIMENSIONMAP"
+    GRUNNLAG_VIEW = "GRUNNLAG_VIEW"
     GRUNNLAG_METRIC = "GRUNNLAG_METRIC"
     GRUNNLAG_THUMBNAIL = "GRUNNLAG_THUMBNAIL"
+    GRUNNLAG_VIDEO = "GRUNNLAG_VIDEO"
     GRUNNLAG_ROI = "GRUNNLAG_ROI"
     GRUNNLAG_LABEL = "GRUNNLAG_LABEL"
     GRUNNLAG_FEATURE = "GRUNNLAG_FEATURE"
     BORD_TABLE = "BORD_TABLE"
     PLOTQL_PLOT = "PLOTQL_PLOT"
 
 
@@ -135,37 +161,14 @@
     "MSR File"
     CZI = "CZI"
     "Zeiss Microscopy File"
     UNKNOWN = "UNKNOWN"
     "Unwknon File Format"
 
 
-class ROIType(str, Enum):
-    """An enumeration."""
-
-    ELLIPSE = "ELLIPSE"
-    "Ellipse"
-    POLYGON = "POLYGON"
-    "POLYGON"
-    LINE = "LINE"
-    "Line"
-    RECTANGLE = "RECTANGLE"
-    "Rectangle"
-    PATH = "PATH"
-    "Path"
-    UNKNOWN = "UNKNOWN"
-    "Unknown"
-    FRAME = "FRAME"
-    "Frame"
-    SLICE = "SLICE"
-    "Slice"
-    POINT = "POINT"
-    "Point"
-
-
 class RepresentationVarietyInput(str, Enum):
     """Variety expresses the Type of Representation we are dealing with"""
 
     MASK = "MASK"
     "Mask (Value represent Labels)"
     VOXEL = "VOXEL"
     "Voxel (Value represent Intensity)"
@@ -180,14 +183,46 @@
     INT64 = "INT64"
     FLOAT64 = "FLOAT64"
     BOOL = "BOOL"
     CATEGORY = "CATEGORY"
     DATETIME65 = "DATETIME65"
     TIMEDELTA = "TIMEDELTA"
     UNICODE = "UNICODE"
+    DATETIME = "DATETIME"
+    DATETIMEZ = "DATETIMEZ"
+    DATETIMETZ = "DATETIMETZ"
+    DATETIME64 = "DATETIME64"
+    DATETIME64TZ = "DATETIME64TZ"
+    DATETIME64NS = "DATETIME64NS"
+    DATETIME64NSUTC = "DATETIME64NSUTC"
+    DATETIME64NSZ = "DATETIME64NSZ"
+    DATETIME64NSZUTC = "DATETIME64NSZUTC"
+
+
+class ROIType(str, Enum):
+    """An enumeration."""
+
+    ELLIPSE = "ELLIPSE"
+    "Ellipse"
+    POLYGON = "POLYGON"
+    "POLYGON"
+    LINE = "LINE"
+    "Line"
+    RECTANGLE = "RECTANGLE"
+    "Rectangle"
+    PATH = "PATH"
+    "Path"
+    UNKNOWN = "UNKNOWN"
+    "Unknown"
+    FRAME = "FRAME"
+    "Frame"
+    SLICE = "SLICE"
+    "Slice"
+    POINT = "POINT"
+    "Point"
 
 
 class RepresentationVariety(str, Enum):
     """An enumeration."""
 
     MASK = "MASK"
     "Mask (Value represent Labels)"
@@ -195,14 +230,24 @@
     "Voxel (Value represent Intensity)"
     RGB = "RGB"
     "RGB (First three channel represent RGB)"
     UNKNOWN = "UNKNOWN"
     "Unknown"
 
 
+class Dimension(str, Enum):
+    """The dimension of the data"""
+
+    X = "X"
+    Y = "Y"
+    Z = "Z"
+    T = "T"
+    C = "C"
+
+
 class Medium(str, Enum):
     """The medium of the imaging environment
 
     Important for the objective settings"""
 
     AIR = "AIR"
     GLYCEROL = "GLYCEROL"
@@ -298,19 +343,21 @@
 
     Follows closely the omexml model. With a few alterations:
     - The data model of the datasets and experimenters is
     part of the mikro datamodel and are not accessed here.
     - Some parameters are ommited as they are not really used"""
 
     planes: Optional[Tuple[Optional["PlaneInput"], ...]]
+    maps: Optional[Tuple[Optional[ID], ...]]
+    timepoints: Optional[Tuple[Optional[ID], ...]]
     channels: Optional[Tuple[Optional["ChannelInput"], ...]]
     physical_size: Optional["PhysicalSizeInput"] = Field(alias="physicalSize")
     affine_transformation: Optional[AffineMatrix] = Field(alias="affineTransformation")
     scale: Optional[Tuple[Optional[float], ...]]
-    position: Optional[ID]
+    positions: Optional[Tuple[Optional[ID], ...]]
     acquisition_date: Optional[datetime] = Field(alias="acquisitionDate")
     objective_settings: Optional["ObjectiveSettingsInput"] = Field(
         alias="objectiveSettings"
     )
     imaging_environment: Optional["ImagingEnvironmentInput"] = Field(
         alias="imagingEnvironment"
     )
@@ -451,14 +498,50 @@
 
     class Config:
         frozen = True
         extra = "forbid"
         use_enum_values = True
 
 
+class RepresentationViewInput(BaseModel):
+    z_min: Optional[int] = Field(alias="zMin")
+    "The x coord of the position (relative to origin)"
+    z_max: Optional[int] = Field(alias="zMax")
+    "The x coord of the position (relative to origin)"
+    t_min: Optional[int] = Field(alias="tMin")
+    "The x coord of the position (relative to origin)"
+    t_max: Optional[int] = Field(alias="tMax")
+    "The x coord of the position (relative to origin)"
+    c_min: Optional[int] = Field(alias="cMin")
+    "The x coord of the position (relative to origin)"
+    c_max: Optional[int] = Field(alias="cMax")
+    "The x coord of the position (relative to origin)"
+    x_min: Optional[int] = Field(alias="xMin")
+    "The x coord of the position (relative to origin)"
+    x_max: Optional[int] = Field(alias="xMax")
+    "The x coord of the position (relative to origin)"
+    y_min: Optional[int] = Field(alias="yMin")
+    "The x coord of the position (relative to origin)"
+    y_max: Optional[int] = Field(alias="yMax")
+    "The x coord of the position (relative to origin)"
+    channel: Optional[ID]
+    "The channel you want to associate with this map"
+    position: Optional[ID]
+    "The position you want to associate with this map"
+    timepoint: Optional[ID]
+    "The position you want to associate with this map"
+    created_while: Optional[AssignationID] = Field(alias="createdWhile")
+    "The assignation id"
+
+    class Config:
+        frozen = True
+        extra = "forbid"
+        use_enum_values = True
+
+
 class InputVector(Vectorizable, BaseModel):
     x: Optional[float]
     "X-coordinate"
     y: Optional[float]
     "Y-coordinate"
     z: Optional[float]
     "Z-coordinate"
@@ -469,14 +552,52 @@
 
     class Config:
         frozen = True
         extra = "forbid"
         use_enum_values = True
 
 
+class ViewInput(BaseModel):
+    omero: ID
+    "The stage this position belongs to"
+    z_min: Optional[int] = Field(alias="zMin")
+    "The x coord of the position (relative to origin)"
+    z_max: Optional[int] = Field(alias="zMax")
+    "The x coord of the position (relative to origin)"
+    t_min: Optional[int] = Field(alias="tMin")
+    "The x coord of the position (relative to origin)"
+    t_max: Optional[int] = Field(alias="tMax")
+    "The x coord of the position (relative to origin)"
+    c_min: Optional[int] = Field(alias="cMin")
+    "The x coord of the position (relative to origin)"
+    c_max: Optional[int] = Field(alias="cMax")
+    "The x coord of the position (relative to origin)"
+    x_min: Optional[int] = Field(alias="xMin")
+    "The x coord of the position (relative to origin)"
+    x_max: Optional[int] = Field(alias="xMax")
+    "The x coord of the position (relative to origin)"
+    y_min: Optional[int] = Field(alias="yMin")
+    "The x coord of the position (relative to origin)"
+    y_max: Optional[int] = Field(alias="yMax")
+    "The x coord of the position (relative to origin)"
+    channel: Optional[ID]
+    "The channel you want to associate with this map"
+    position: Optional[ID]
+    "The position you want to associate with this map"
+    timepoint: Optional[ID]
+    "The position you want to associate with this map"
+    created_while: Optional[AssignationID] = Field(alias="createdWhile")
+    "The assignation id"
+
+    class Config:
+        frozen = True
+        extra = "forbid"
+        use_enum_values = True
+
+
 class DetailLabelFragmentFeatures(BaseModel):
     """A Feature is a numerical key value pair that is attached to a Label.
 
     You can model it for example as a key value pair of a class instance of a segmentation mask.
     Representation -> Label0 -> Feature0
                              -> Feature1
                    -> Label1 -> Feature0
@@ -782,15 +903,15 @@
     name: str
     "The name of the sample"
 
     class Config:
         frozen = True
 
 
-class RepresentationFragmentOmero(BaseModel):
+class RepresentationFragmentOmero(Omero, BaseModel):
     """Omero is a through model that stores the real world context of an image
 
     This means that it stores the position (corresponding to the relative displacement to
     a stage (Both are models)), objective and other meta data of the image.
 
     """
 
@@ -815,14 +936,314 @@
     "Cleartext name"
     omero: Optional[RepresentationFragmentOmero]
 
     class Config:
         frozen = True
 
 
+class DetailRepresentationFragmentSample(BaseModel):
+    """Samples are storage containers for representations. A Sample is to be understood analogous to a Biological Sample. It existed in Time (the time of acquisiton and experimental procedure), was measured in space (x,y,z) and in different modalities (c). Sample therefore provide a datacontainer where each Representation of the data shares the same dimensions. Every transaction to our image data is still part of the original acuqistion, so also filtered images are refering back to the sample"""
+
+    typename: Optional[Literal["Sample"]] = Field(alias="__typename", exclude=True)
+    id: ID
+    name: str
+    "The name of the sample"
+
+    class Config:
+        frozen = True
+
+
+class DetailRepresentationFragmentOmeroPhysicalsize(PhysicalSize, BaseModel):
+    """Physical size of the image
+
+    Each dimensions of the image has a physical size. This is the size of the
+    pixel in the image. The physical size is given in micrometers on a PIXEL
+    basis. This means that the physical size of the image is the size of the
+    pixel in the image * the number of pixels in the image. For example, if
+    the image is 1000x1000 pixels and the physical size of the image is 3 (x params) x 3 (y params),
+    micrometer, the physical size of the image is 3000x3000 micrometer. If the image
+
+    The t dimension is given in ms, since the time is given in ms.
+    The C dimension is given in nm, since the wavelength is given in nm."""
+
+    typename: Optional[Literal["PhysicalSize"]] = Field(
+        alias="__typename", exclude=True
+    )
+    x: Optional[float]
+    "Physical size of *one* Pixel in the x dimension (in µm)"
+    y: Optional[float]
+    "Physical size of *one* Pixel in the t dimension (in µm)"
+    z: Optional[float]
+    "Physical size of *one* Pixel in the z dimension (in µm)"
+
+    class Config:
+        frozen = True
+
+
+class DetailRepresentationFragmentOmeroPositionsStage(Stage, BaseModel):
+    """An Stage is a set of positions that share a common space on a microscope and can
+    be use to translate.
+
+
+    """
+
+    typename: Optional[Literal["Stage"]] = Field(alias="__typename", exclude=True)
+    name: str
+    "The name of the stage"
+    id: ID
+
+    class Config:
+        frozen = True
+
+
+class DetailRepresentationFragmentOmeroPositions(Position, BaseModel):
+    """The relative position of a sample on a microscope stage"""
+
+    typename: Optional[Literal["Position"]] = Field(alias="__typename", exclude=True)
+    name: str
+    "The name of the possition"
+    id: ID
+    x: float
+    "pixelSize for x in microns"
+    y: float
+    "pixelSize for y in microns"
+    z: float
+    "pixelSize for z in microns"
+    stage: DetailRepresentationFragmentOmeroPositionsStage
+
+    class Config:
+        frozen = True
+
+
+class DetailRepresentationFragmentOmeroTimepointsEra(BaseModel):
+    """Era(id, created_by, created_through, created_while, name, start, end, created_at)"""
+
+    typename: Optional[Literal["Era"]] = Field(alias="__typename", exclude=True)
+    name: str
+    "The name of the era"
+    id: ID
+
+    class Config:
+        frozen = True
+
+
+class DetailRepresentationFragmentOmeroTimepoints(BaseModel):
+    """The relative position of a sample on a microscope stage"""
+
+    typename: Optional[Literal["Timepoint"]] = Field(alias="__typename", exclude=True)
+    name: Optional[str]
+    "The name of the timepoint"
+    id: ID
+    era: DetailRepresentationFragmentOmeroTimepointsEra
+
+    class Config:
+        frozen = True
+
+
+class DetailRepresentationFragmentOmeroViewsChannel(BaseModel):
+    """Channel(id, created_by, created_through, created_while, name, emission_wavelength, excitation_wavelength, acquisition_mode, color)"""
+
+    typename: Optional[Literal["Channel"]] = Field(alias="__typename", exclude=True)
+    name: str
+    "The name of the channel"
+    id: ID
+
+    class Config:
+        frozen = True
+
+
+class DetailRepresentationFragmentOmeroViewsPosition(Position, BaseModel):
+    """The relative position of a sample on a microscope stage"""
+
+    typename: Optional[Literal["Position"]] = Field(alias="__typename", exclude=True)
+    name: str
+    "The name of the possition"
+    id: ID
+    x: float
+    "pixelSize for x in microns"
+    y: float
+    "pixelSize for y in microns"
+    z: float
+    "pixelSize for z in microns"
+
+    class Config:
+        frozen = True
+
+
+class DetailRepresentationFragmentOmeroViewsTimepoint(BaseModel):
+    """The relative position of a sample on a microscope stage"""
+
+    typename: Optional[Literal["Timepoint"]] = Field(alias="__typename", exclude=True)
+    id: ID
+
+    class Config:
+        frozen = True
+
+
+class DetailRepresentationFragmentOmeroViews(BaseModel):
+    """View(id, created_by, created_through, created_while, omero, z_min, z_max, x_min, x_max, y_min, y_max, t_min, t_max, c_min, c_max, channel, position, objective, instrument, timepoint)"""
+
+    typename: Optional[Literal["View"]] = Field(alias="__typename", exclude=True)
+    channel: Optional[DetailRepresentationFragmentOmeroViewsChannel]
+    position: Optional[DetailRepresentationFragmentOmeroViewsPosition]
+    timepoint: Optional[DetailRepresentationFragmentOmeroViewsTimepoint]
+
+    class Config:
+        frozen = True
+
+
+class DetailRepresentationFragmentOmero(Omero, BaseModel):
+    """Omero is a through model that stores the real world context of an image
+
+    This means that it stores the position (corresponding to the relative displacement to
+    a stage (Both are models)), objective and other meta data of the image.
+
+    """
+
+    typename: Optional[Literal["Omero"]] = Field(alias="__typename", exclude=True)
+    physical_size: Optional[DetailRepresentationFragmentOmeroPhysicalsize] = Field(
+        alias="physicalSize"
+    )
+    positions: Tuple[DetailRepresentationFragmentOmeroPositions, ...]
+    timepoints: Optional[
+        Tuple[Optional[DetailRepresentationFragmentOmeroTimepoints], ...]
+    ]
+    "Associated Timepoints"
+    views: Optional[Tuple[Optional[DetailRepresentationFragmentOmeroViews], ...]]
+    "Associated views"
+
+    class Config:
+        frozen = True
+
+
+class DetailRepresentationFragmentMetricsRepresentation(Representation, BaseModel):
+    """A Representation is 5-dimensional representation of an image
+
+    Mikro stores each image as sa 5-dimensional representation. The dimensions are:
+    - t: time
+    - c: channel
+    - z: z-stack
+    - x: x-dimension
+    - y: y-dimension
+
+    This ensures a unified api for all images, regardless of their original dimensions. Another main
+    determining factor for a representation is its variety:
+    A representation can be a raw image representating voxels (VOXEL)
+    or a segmentation mask representing instances of a class. (MASK)
+    It can also representate a human perception of the image (RGB) or a human perception of the mask (RGBMASK)
+
+    # Meta
+
+    Meta information is stored in the omero field which gives access to the omero-meta data. Refer to the omero documentation for more information.
+
+
+    #Origins and Derivations
+
+    Images can be filtered, which means that a new representation is created from the other (original) representations. This new representation is then linked to the original representations. This way, we can always trace back to the original representation.
+    Both are encapsulaed in the origins and derived fields.
+
+    Representations belong to *one* sample. Every transaction to our image data is still part of the original acuqistion, so also filtered images are refering back to the sample
+    Each iamge has also a name, which is used to identify the image. The name is unique within a sample.
+    File and Rois that are used to create images are saved in the file origins and roi origins repectively.
+
+
+    """
+
+    typename: Optional[Literal["Representation"]] = Field(
+        alias="__typename", exclude=True
+    )
+    id: ID
+
+    class Config:
+        frozen = True
+
+
+class DetailRepresentationFragmentMetrics(BaseModel):
+    typename: Optional[Literal["Metric"]] = Field(alias="__typename", exclude=True)
+    id: ID
+    key: str
+    "The Key"
+    value: Optional[MetricValue]
+    "Value"
+    representation: Optional[DetailRepresentationFragmentMetricsRepresentation]
+    "The Representatoin this Metric belongs to"
+
+    class Config:
+        frozen = True
+
+
+class DetailRepresentationFragmentDerived(Representation, BaseModel):
+    """A Representation is 5-dimensional representation of an image
+
+    Mikro stores each image as sa 5-dimensional representation. The dimensions are:
+    - t: time
+    - c: channel
+    - z: z-stack
+    - x: x-dimension
+    - y: y-dimension
+
+    This ensures a unified api for all images, regardless of their original dimensions. Another main
+    determining factor for a representation is its variety:
+    A representation can be a raw image representating voxels (VOXEL)
+    or a segmentation mask representing instances of a class. (MASK)
+    It can also representate a human perception of the image (RGB) or a human perception of the mask (RGBMASK)
+
+    # Meta
+
+    Meta information is stored in the omero field which gives access to the omero-meta data. Refer to the omero documentation for more information.
+
+
+    #Origins and Derivations
+
+    Images can be filtered, which means that a new representation is created from the other (original) representations. This new representation is then linked to the original representations. This way, we can always trace back to the original representation.
+    Both are encapsulaed in the origins and derived fields.
+
+    Representations belong to *one* sample. Every transaction to our image data is still part of the original acuqistion, so also filtered images are refering back to the sample
+    Each iamge has also a name, which is used to identify the image. The name is unique within a sample.
+    File and Rois that are used to create images are saved in the file origins and roi origins repectively.
+
+
+    """
+
+    typename: Optional[Literal["Representation"]] = Field(
+        alias="__typename", exclude=True
+    )
+    id: ID
+    name: Optional[str]
+    "Cleartext name"
+    store: Optional[Store]
+
+    class Config:
+        frozen = True
+
+
+class DetailRepresentationFragment(Representation, BaseModel):
+    typename: Optional[Literal["Representation"]] = Field(
+        alias="__typename", exclude=True
+    )
+    sample: Optional[DetailRepresentationFragmentSample]
+    "The Sample this representation belosngs to"
+    id: ID
+    store: Optional[Store]
+    shape: Optional[Tuple[int, ...]]
+    "The arrays shape format [c,t,z,y,x]"
+    variety: RepresentationVariety
+    "The Representation can have vasrying types, consult your API"
+    name: Optional[str]
+    "Cleartext name"
+    omero: Optional[DetailRepresentationFragmentOmero]
+    metrics: Optional[Tuple[Optional[DetailRepresentationFragmentMetrics], ...]]
+    "Associated metrics of this Imasge"
+    derived: Optional[Tuple[Optional[DetailRepresentationFragmentDerived], ...]]
+    "Derived Images from this Image"
+
+    class Config:
+        frozen = True
+
+
 class RepresentationAndMaskFragmentSample(BaseModel):
     """Samples are storage containers for representations. A Sample is to be understood analogous to a Biological Sample. It existed in Time (the time of acquisiton and experimental procedure), was measured in space (x,y,z) and in different modalities (c). Sample therefore provide a datacontainer where each Representation of the data shares the same dimensions. Every transaction to our image data is still part of the original acuqistion, so also filtered images are refering back to the sample"""
 
     typename: Optional[Literal["Sample"]] = Field(alias="__typename", exclude=True)
     id: ID
     name: str
     "The name of the sample"
@@ -874,15 +1295,15 @@
     name: Optional[str]
     "Cleartext name"
 
     class Config:
         frozen = True
 
 
-class RepresentationAndMaskFragmentOmero(BaseModel):
+class RepresentationAndMaskFragmentOmero(Omero, BaseModel):
     """Omero is a through model that stores the real world context of an image
 
     This means that it stores the position (corresponding to the relative displacement to
     a stage (Both are models)), objective and other meta data of the image.
 
     """
 
@@ -962,15 +1383,15 @@
 class Create_roiMutation(BaseModel):
     create_roi: Optional[ROIFragment] = Field(alias="createROI")
     "Creates a Sample"
 
     class Arguments(BaseModel):
         representation: ID
         vectors: List[Optional[InputVector]]
-        creator: Optional[ID] = None
+        creator: Optional[ID]
         type: RoiTypeInput
 
     class Meta:
         document = "fragment ROI on ROI {\n  id\n  vectors {\n    x\n    y\n    z\n    t\n    c\n  }\n  type\n  representation {\n    id\n  }\n  creator {\n    id\n    color\n  }\n}\n\nmutation create_roi($representation: ID!, $vectors: [InputVector]!, $creator: ID, $type: RoiTypeInput!) {\n  createROI(\n    representation: $representation\n    vectors: $vectors\n    type: $type\n    creator: $creator\n  ) {\n    ...ROI\n  }\n}"
 
 
 class Delete_roiMutationDeleteroi(BaseModel):
@@ -1004,14 +1425,153 @@
         representation: ID
         instance: int
 
     class Meta:
         document = "fragment DetailLabel on Label {\n  id\n  instance\n  name\n  features {\n    id\n    key\n    value\n  }\n}\n\nquery get_label_for($representation: ID!, $instance: Int!) {\n  labelFor(representation: $representation, instance: $instance) {\n    ...DetailLabel\n  }\n}"
 
 
+class Get_image_stageQueryStagePositionsOmerosRepresentation(Representation, BaseModel):
+    """A Representation is 5-dimensional representation of an image
+
+    Mikro stores each image as sa 5-dimensional representation. The dimensions are:
+    - t: time
+    - c: channel
+    - z: z-stack
+    - x: x-dimension
+    - y: y-dimension
+
+    This ensures a unified api for all images, regardless of their original dimensions. Another main
+    determining factor for a representation is its variety:
+    A representation can be a raw image representating voxels (VOXEL)
+    or a segmentation mask representing instances of a class. (MASK)
+    It can also representate a human perception of the image (RGB) or a human perception of the mask (RGBMASK)
+
+    # Meta
+
+    Meta information is stored in the omero field which gives access to the omero-meta data. Refer to the omero documentation for more information.
+
+
+    #Origins and Derivations
+
+    Images can be filtered, which means that a new representation is created from the other (original) representations. This new representation is then linked to the original representations. This way, we can always trace back to the original representation.
+    Both are encapsulaed in the origins and derived fields.
+
+    Representations belong to *one* sample. Every transaction to our image data is still part of the original acuqistion, so also filtered images are refering back to the sample
+    Each iamge has also a name, which is used to identify the image. The name is unique within a sample.
+    File and Rois that are used to create images are saved in the file origins and roi origins repectively.
+
+
+    """
+
+    typename: Optional[Literal["Representation"]] = Field(
+        alias="__typename", exclude=True
+    )
+    id: ID
+    shape: Optional[Tuple[int, ...]]
+    "The arrays shape format [c,t,z,y,x]"
+    store: Optional[Store]
+
+    class Config:
+        frozen = True
+
+
+class Get_image_stageQueryStagePositionsOmerosPhysicalsize(PhysicalSize, BaseModel):
+    """Physical size of the image
+
+    Each dimensions of the image has a physical size. This is the size of the
+    pixel in the image. The physical size is given in micrometers on a PIXEL
+    basis. This means that the physical size of the image is the size of the
+    pixel in the image * the number of pixels in the image. For example, if
+    the image is 1000x1000 pixels and the physical size of the image is 3 (x params) x 3 (y params),
+    micrometer, the physical size of the image is 3000x3000 micrometer. If the image
+
+    The t dimension is given in ms, since the time is given in ms.
+    The C dimension is given in nm, since the wavelength is given in nm."""
+
+    typename: Optional[Literal["PhysicalSize"]] = Field(
+        alias="__typename", exclude=True
+    )
+    x: Optional[float]
+    "Physical size of *one* Pixel in the x dimension (in µm)"
+    y: Optional[float]
+    "Physical size of *one* Pixel in the t dimension (in µm)"
+    z: Optional[float]
+    "Physical size of *one* Pixel in the z dimension (in µm)"
+    t: Optional[float]
+    "Physical size of *one* Pixel in the t dimension (in ms)"
+    c: Optional[float]
+    "Physical size of *one* Pixel in the c dimension (in µm)"
+
+    class Config:
+        frozen = True
+
+
+class Get_image_stageQueryStagePositionsOmeros(Omero, BaseModel):
+    """Omero is a through model that stores the real world context of an image
+
+    This means that it stores the position (corresponding to the relative displacement to
+    a stage (Both are models)), objective and other meta data of the image.
+
+    """
+
+    typename: Optional[Literal["Omero"]] = Field(alias="__typename", exclude=True)
+    id: ID
+    acquisition_date: Optional[datetime] = Field(alias="acquisitionDate")
+    representation: Get_image_stageQueryStagePositionsOmerosRepresentation
+    physical_size: Optional[
+        Get_image_stageQueryStagePositionsOmerosPhysicalsize
+    ] = Field(alias="physicalSize")
+
+    class Config:
+        frozen = True
+
+
+class Get_image_stageQueryStagePositions(Position, BaseModel):
+    """The relative position of a sample on a microscope stage"""
+
+    typename: Optional[Literal["Position"]] = Field(alias="__typename", exclude=True)
+    x: float
+    "pixelSize for x in microns"
+    y: float
+    "pixelSize for y in microns"
+    z: float
+    "pixelSize for z in microns"
+    omeros: Optional[Tuple[Optional[Get_image_stageQueryStagePositionsOmeros], ...]]
+    "Associated images through Omero"
+
+    class Config:
+        frozen = True
+
+
+class Get_image_stageQueryStage(Stage, BaseModel):
+    """An Stage is a set of positions that share a common space on a microscope and can
+    be use to translate.
+
+
+    """
+
+    typename: Optional[Literal["Stage"]] = Field(alias="__typename", exclude=True)
+    positions: Tuple[Get_image_stageQueryStagePositions, ...]
+
+    class Config:
+        frozen = True
+
+
+class Get_image_stageQuery(BaseModel):
+    stage: Optional[Get_image_stageQueryStage]
+    'Get a single experiment by ID"\n    \n    Returns a single experiment by ID. If the user does not have access\n    to the experiment, an error will be raised.\n    \n    '
+
+    class Arguments(BaseModel):
+        id: ID
+        limit: Optional[int]
+
+    class Meta:
+        document = 'query get_image_stage($id: ID!, $limit: Int) {\n  stage(id: $id) {\n    positions {\n      x\n      y\n      z\n      omeros(order: "-acquired", limit: $limit) {\n        id\n        acquisitionDate\n        representation {\n          id\n          shape\n          store\n        }\n        physicalSize {\n          x\n          y\n          z\n          t\n          c\n        }\n      }\n    }\n  }\n}'
+
+
 class Expand_multiscaleQuery(BaseModel):
     sample: Optional[MultiScaleSampleFragment]
     "Get a Sample by ID\n    \n    Returns a single Sample by ID. If the user does not have access\n    to the Sample, an error will be raised.\n    "
 
     class Arguments(BaseModel):
         id: ID
 
@@ -1021,15 +1581,15 @@
 
 class Get_roisQuery(BaseModel):
     rois: Optional[Tuple[Optional[ROIFragment], ...]]
     "All Rois\n    \n    This query returns all Rois that are stored on the platform\n    depending on the user's permissions. Generally, this query will return\n    all Rois that the user has access to. If the user is an amdin\n    or superuser, all Rois will be returned."
 
     class Arguments(BaseModel):
         representation: ID
-        type: Optional[List[Optional[RoiTypeInput]]] = None
+        type: Optional[List[Optional[RoiTypeInput]]]
 
     class Meta:
         document = "fragment ROI on ROI {\n  id\n  vectors {\n    x\n    y\n    z\n    t\n    c\n  }\n  type\n  representation {\n    id\n  }\n  creator {\n    id\n    color\n  }\n}\n\nquery get_rois($representation: ID!, $type: [RoiTypeInput]) {\n  rois(representation: $representation, type: $type) {\n    ...ROI\n  }\n}"
 
 
 class Get_roiQuery(BaseModel):
     roi: Optional[ROIFragment]
@@ -1065,15 +1625,15 @@
 
 class Search_roisQuery(BaseModel):
     options: Optional[Tuple[Optional[Search_roisQueryOptions], ...]]
     "All Rois\n    \n    This query returns all Rois that are stored on the platform\n    depending on the user's permissions. Generally, this query will return\n    all Rois that the user has access to. If the user is an amdin\n    or superuser, all Rois will be returned."
 
     class Arguments(BaseModel):
         search: str
-        values: Optional[List[Optional[ID]]] = None
+        values: Optional[List[Optional[ID]]]
 
     class Meta:
         document = "query search_rois($search: String!, $values: [ID]) {\n  options: rois(repname: $search, ids: $values) {\n    label: id\n    value: id\n  }\n}"
 
 
 class Get_multiscale_repQuery(BaseModel):
     representation: Optional[MultiScaleRepresentationFragment]
@@ -1115,115 +1675,23 @@
     class Arguments(BaseModel):
         pass
 
     class Meta:
         document = 'fragment ListRepresentation on Representation {\n  id\n  name\n  sample {\n    id\n    name\n  }\n}\n\nquery get_some_representations {\n  representations(limit: 10, order: "-created_at") {\n    ...ListRepresentation\n  }\n}'
 
 
-class Get_image_stageQueryStagePositionsOmerosRepresentation(Representation, BaseModel):
-    """A Representation is 5-dimensional representation of an image
-
-    Mikro stores each image as sa 5-dimensional representation. The dimensions are:
-    - t: time
-    - c: channel
-    - z: z-stack
-    - x: x-dimension
-    - y: y-dimension
-
-    This ensures a unified api for all images, regardless of their original dimensions. Another main
-    determining factor for a representation is its variety:
-    A representation can be a raw image representating voxels (VOXEL)
-    or a segmentation mask representing instances of a class. (MASK)
-    It can also representate a human perception of the image (RGB) or a human perception of the mask (RGBMASK)
-
-    # Meta
-
-    Meta information is stored in the omero field which gives access to the omero-meta data. Refer to the omero documentation for more information.
-
-
-    #Origins and Derivations
-
-    Images can be filtered, which means that a new representation is created from the other (original) representations. This new representation is then linked to the original representations. This way, we can always trace back to the original representation.
-    Both are encapsulaed in the origins and derived fields.
-
-    Representations belong to *one* sample. Every transaction to our image data is still part of the original acuqistion, so also filtered images are refering back to the sample
-    Each iamge has also a name, which is used to identify the image. The name is unique within a sample.
-    File and Rois that are used to create images are saved in the file origins and roi origins repectively.
-
-
-    """
-
-    typename: Optional[Literal["Representation"]] = Field(
-        alias="__typename", exclude=True
-    )
-    id: ID
-    shape: Optional[Tuple[int, ...]]
-    "The arrays shape format [c,t,z,y,x]"
-
-    class Config:
-        frozen = True
-
-
-class Get_image_stageQueryStagePositionsOmeros(BaseModel):
-    """Omero is a through model that stores the real world context of an image
-
-    This means that it stores the position (corresponding to the relative displacement to
-    a stage (Both are models)), objective and other meta data of the image.
-
-    """
-
-    typename: Optional[Literal["Omero"]] = Field(alias="__typename", exclude=True)
-    acquisition_date: Optional[datetime] = Field(alias="acquisitionDate")
-    representation: Get_image_stageQueryStagePositionsOmerosRepresentation
-
-    class Config:
-        frozen = True
-
-
-class Get_image_stageQueryStagePositions(BaseModel):
-    """The relative position of a sample on a microscope stage"""
-
-    typename: Optional[Literal["Position"]] = Field(alias="__typename", exclude=True)
-    x: float
-    "pixelSize for x in microns"
-    y: float
-    "pixelSize for y in microns"
-    z: float
-    "pixelSize for z in microns"
-    omeros: Optional[Tuple[Optional[Get_image_stageQueryStagePositionsOmeros], ...]]
-    "Associated images through Omero"
-
-    class Config:
-        frozen = True
-
-
-class Get_image_stageQueryStage(BaseModel):
-    """An Stage is a set of positions that share a common space on a microscope and can
-    be use to translate.
-
-
-    """
-
-    typename: Optional[Literal["Stage"]] = Field(alias="__typename", exclude=True)
-    positions: Tuple[Get_image_stageQueryStagePositions, ...]
-
-    class Config:
-        frozen = True
-
-
-class Get_image_stageQuery(BaseModel):
-    stage: Optional[Get_image_stageQueryStage]
-    'Get a single experiment by ID"\n    \n    Returns a single experiment by ID. If the user does not have access\n    to the experiment, an error will be raised.\n    \n    '
+class DetailRepQuery(BaseModel):
+    representation: Optional[DetailRepresentationFragment]
+    "Get a single Representation by ID\n    \n    Returns a single Representation by ID. If the user does not have access\n    to the Representation, an error will be raised.\n    "
 
     class Arguments(BaseModel):
         id: ID
-        limit: Optional[int] = None
 
     class Meta:
-        document = 'query get_image_stage($id: ID!, $limit: Int) {\n  stage(id: $id) {\n    positions {\n      x\n      y\n      z\n      omeros(order: "-acquired", limit: $limit) {\n        acquisitionDate\n        representation {\n          id\n          shape\n        }\n      }\n    }\n  }\n}'
+        document = "fragment DetailRepresentation on Representation {\n  sample {\n    id\n    name\n  }\n  id\n  store\n  shape\n  variety\n  name\n  omero {\n    physicalSize {\n      x\n      y\n      z\n    }\n    positions {\n      name\n      id\n      x\n      y\n      z\n      stage {\n        name\n        id\n      }\n    }\n    timepoints {\n      name\n      id\n      era {\n        name\n        id\n      }\n    }\n    views {\n      channel {\n        name\n        id\n      }\n      position {\n        name\n        id\n        x\n        y\n        z\n      }\n      timepoint {\n        id\n      }\n    }\n  }\n  metrics(flatten: 3) {\n    id\n    key\n    value\n    representation {\n      id\n    }\n  }\n  derived(flatten: 3) {\n    id\n    name\n    store\n  }\n}\n\nquery DetailRep($id: ID!) {\n  representation(id: $id) {\n    ...DetailRepresentation\n  }\n}"
 
 
 async def awatch_rois(
     representation: ID, rath: MikroRath = None
 ) -> AsyncIterator[Optional[Watch_roisSubscriptionRois]]:
     """watch_rois
 
@@ -1444,14 +1912,62 @@
     return execute(
         Get_label_forQuery,
         {"representation": representation, "instance": instance},
         rath=rath,
     ).label_for
 
 
+async def aget_image_stage(
+    id: ID, limit: Optional[int] = None, rath: MikroRath = None
+) -> Optional[Get_image_stageQueryStage]:
+    """get_image_stage
+
+
+     stage: An Stage is a set of positions that share a common space on a microscope and can
+        be use to translate.
+
+
+
+
+
+    Arguments:
+        id (ID): id
+        limit (Optional[int], optional): limit.
+        rath (mikro.rath.MikroRath, optional): The mikro rath client
+
+    Returns:
+        Optional[Get_image_stageQueryStage]"""
+    return (
+        await aexecute(Get_image_stageQuery, {"id": id, "limit": limit}, rath=rath)
+    ).stage
+
+
+def get_image_stage(
+    id: ID, limit: Optional[int] = None, rath: MikroRath = None
+) -> Optional[Get_image_stageQueryStage]:
+    """get_image_stage
+
+
+     stage: An Stage is a set of positions that share a common space on a microscope and can
+        be use to translate.
+
+
+
+
+
+    Arguments:
+        id (ID): id
+        limit (Optional[int], optional): limit.
+        rath (mikro.rath.MikroRath, optional): The mikro rath client
+
+    Returns:
+        Optional[Get_image_stageQueryStage]"""
+    return execute(Get_image_stageQuery, {"id": id, "limit": limit}, rath=rath).stage
+
+
 async def aexpand_multiscale(
     id: ID, rath: MikroRath = None
 ) -> Optional[MultiScaleSampleFragment]:
     """expand_multiscale
 
 
      sample: Samples are storage containers for representations. A Sample is to be understood analogous to a Biological Sample. It existed in Time (the time of acquisiton and experimental procedure), was measured in space (x,y,z) and in different modalities (c). Sample therefore provide a datacontainer where each Representation of the data shares the same dimensions. Every transaction to our image data is still part of the original acuqistion, so also filtered images are refering back to the sample
@@ -2056,57 +2572,105 @@
         rath (mikro.rath.MikroRath, optional): The mikro rath client
 
     Returns:
         Optional[List[Optional[ListRepresentationFragment]]]"""
     return execute(Get_some_representationsQuery, {}, rath=rath).representations
 
 
-async def aget_image_stage(
-    id: ID, limit: Optional[int] = None, rath: MikroRath = None
-) -> Optional[Get_image_stageQueryStage]:
-    """get_image_stage
+async def adetail_rep(
+    id: ID, rath: MikroRath = None
+) -> Optional[DetailRepresentationFragment]:
+    """DetailRep
 
 
-     stage: An Stage is a set of positions that share a common space on a microscope and can
-        be use to translate.
+     representation: A Representation is 5-dimensional representation of an image
+
+        Mikro stores each image as sa 5-dimensional representation. The dimensions are:
+        - t: time
+        - c: channel
+        - z: z-stack
+        - x: x-dimension
+        - y: y-dimension
+
+        This ensures a unified api for all images, regardless of their original dimensions. Another main
+        determining factor for a representation is its variety:
+        A representation can be a raw image representating voxels (VOXEL)
+        or a segmentation mask representing instances of a class. (MASK)
+        It can also representate a human perception of the image (RGB) or a human perception of the mask (RGBMASK)
+
+        # Meta
+
+        Meta information is stored in the omero field which gives access to the omero-meta data. Refer to the omero documentation for more information.
+
+
+        #Origins and Derivations
+
+        Images can be filtered, which means that a new representation is created from the other (original) representations. This new representation is then linked to the original representations. This way, we can always trace back to the original representation.
+        Both are encapsulaed in the origins and derived fields.
+
+        Representations belong to *one* sample. Every transaction to our image data is still part of the original acuqistion, so also filtered images are refering back to the sample
+        Each iamge has also a name, which is used to identify the image. The name is unique within a sample.
+        File and Rois that are used to create images are saved in the file origins and roi origins repectively.
 
 
 
 
 
     Arguments:
         id (ID): id
-        limit (Optional[int], optional): limit.
         rath (mikro.rath.MikroRath, optional): The mikro rath client
 
     Returns:
-        Optional[Get_image_stageQueryStage]"""
-    return (
-        await aexecute(Get_image_stageQuery, {"id": id, "limit": limit}, rath=rath)
-    ).stage
+        Optional[DetailRepresentationFragment]"""
+    return (await aexecute(DetailRepQuery, {"id": id}, rath=rath)).representation
 
 
-def get_image_stage(
-    id: ID, limit: Optional[int] = None, rath: MikroRath = None
-) -> Optional[Get_image_stageQueryStage]:
-    """get_image_stage
+def detail_rep(
+    id: ID, rath: MikroRath = None
+) -> Optional[DetailRepresentationFragment]:
+    """DetailRep
 
 
-     stage: An Stage is a set of positions that share a common space on a microscope and can
-        be use to translate.
+     representation: A Representation is 5-dimensional representation of an image
+
+        Mikro stores each image as sa 5-dimensional representation. The dimensions are:
+        - t: time
+        - c: channel
+        - z: z-stack
+        - x: x-dimension
+        - y: y-dimension
+
+        This ensures a unified api for all images, regardless of their original dimensions. Another main
+        determining factor for a representation is its variety:
+        A representation can be a raw image representating voxels (VOXEL)
+        or a segmentation mask representing instances of a class. (MASK)
+        It can also representate a human perception of the image (RGB) or a human perception of the mask (RGBMASK)
+
+        # Meta
+
+        Meta information is stored in the omero field which gives access to the omero-meta data. Refer to the omero documentation for more information.
+
+
+        #Origins and Derivations
+
+        Images can be filtered, which means that a new representation is created from the other (original) representations. This new representation is then linked to the original representations. This way, we can always trace back to the original representation.
+        Both are encapsulaed in the origins and derived fields.
+
+        Representations belong to *one* sample. Every transaction to our image data is still part of the original acuqistion, so also filtered images are refering back to the sample
+        Each iamge has also a name, which is used to identify the image. The name is unique within a sample.
+        File and Rois that are used to create images are saved in the file origins and roi origins repectively.
 
 
 
 
 
     Arguments:
         id (ID): id
-        limit (Optional[int], optional): limit.
         rath (mikro.rath.MikroRath, optional): The mikro rath client
 
     Returns:
-        Optional[Get_image_stageQueryStage]"""
-    return execute(Get_image_stageQuery, {"id": id, "limit": limit}, rath=rath).stage
+        Optional[DetailRepresentationFragment]"""
+    return execute(DetailRepQuery, {"id": id}, rath=rath).representation
 
 
 DescendendInput.update_forward_refs()
 OmeroRepresentationInput.update_forward_refs()
```

### Comparing `mikro_napari-0.1.50/mikro_napari/run.py` & `mikro_napari-0.1.51/mikro_napari/run.py`

 * *Files identical despite different names*

### Comparing `mikro_napari-0.1.50/mikro_napari/utils.py` & `mikro_napari-0.1.51/mikro_napari/utils.py`

 * *Files identical despite different names*

### Comparing `mikro_napari-0.1.50/mikro_napari/widgets/dialogs/open_image.py` & `mikro_napari-0.1.51/mikro_napari/widgets/dialogs/open_image.py`

 * *Files identical despite different names*

### Comparing `mikro_napari-0.1.50/mikro_napari/widgets/main_widget.py` & `mikro_napari-0.1.51/mikro_napari/widgets/main_widget.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 import napari
 from rekuest.widgets import SearchWidget
 from koil.qt import QtRunner
 from mikro.api.schema import (
     RepresentationVariety,
+    from_xarray,
     afrom_xarray,
     RepresentationFragment,
 )
 from qtpy import QtWidgets
 from qtpy import QtCore
 from arkitekt.apps.connected import ConnectedApp
 from arkitekt.qt.magic_bar import AppState, MagicBar
@@ -40,15 +41,17 @@
     ward="mikro",
 )
 
 
 class MikroNapariWidget(QtWidgets.QWidget):
     emit_image: QtCore.Signal = QtCore.Signal(object)
 
-    def __init__(self, viewer: napari.Viewer, app: ConnectedApp, *args, **kwargs) -> None:
+    def __init__(
+        self, viewer: napari.Viewer, app: ConnectedApp, *args, **kwargs
+    ) -> None:
         super(MikroNapariWidget, self).__init__(*args, **kwargs)
 
         self.viewer = viewer
 
         self.mylayout = QtWidgets.QVBoxLayout()
 
         self.app = app
@@ -164,15 +167,15 @@
         if self.active_non_mikro_layers and not self.active_mikro_layers:
             self.upload_image_button.setText("Upload Layer")
             self.upload_image_button.setEnabled(self.magic_bar.state == AppState.UP)
         else:
             self.upload_image_button.setText("Upload Layer")
             self.upload_image_button.setEnabled(False)
 
-    async def upload_layer(self, name: str = "") -> RepresentationFragment:
+    def upload_layer(self, name: str = "") -> RepresentationFragment:
         """Upload Napari Layer
 
         Upload the current image to the server.
 
         Args:
             name (str, optional): Overwrite the layer name. Defaults to None.
 
@@ -196,19 +199,17 @@
         if image_layer.ndim == 3:
             xarray = xr.DataArray(image_layer.data, dims=list("zxy"))
 
         if image_layer.ndim == 4:
             xarray = xr.DataArray(image_layer.data, dims=list("tzxy"))
 
         if image_layer.ndim == 5:
-            xarray = xr.DataArray(image_layer.data, dims=list("tzxyc"))
+            xarray = xr.DataArray(image_layer.data, dims=list("ctzyx"))
 
-        return await afrom_xarray(
-            xarray, name=name or image_layer.name, variety=variety
-        )
+        return from_xarray(xarray, name=name or image_layer.name, variety=variety)
 
     def cause_upload(self):
         for image_layer in self.active_non_mikro_layers:
             variety = RepresentationVariety.VOXEL
 
             if image_layer.ndim == 2:
                 if image_layer.rgb:
@@ -230,15 +231,14 @@
             self.upload_image_button.setText(f"Uploading {image_layer.name}...")
             self.upload_image_button.setEnabled(False)
 
     def on_upload_finished(self, image):
         self.on_selection_changed()
 
     def cause_image_load(self):
-
         rep_dialog = OpenImageDialog(self)
         x = rep_dialog.exec()
         if x:
             self.representation_controller.active_representation = (
                 rep_dialog.selected_representation
             )
```

### Comparing `mikro_napari-0.1.50/pyproject.toml` & `mikro_napari-0.1.51/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,21 +1,23 @@
 [tool.poetry]
 name = "mikro-napari"
-version = "0.1.50"
+version = "0.1.51"
 description = "A napari plugin to interact with and provide functionality for a connected arkitekt server"
 readme = "README.md"
 repository = "https://github.com/jhnnsrs/mikro-napari"
 authors = ["jhnnsrs <jhnnsrs@gmail.com>"]
 license = "CC BY-NC 3.0"
 packages = [{ include = "mikro_napari" }]
 classifiers = ["Framework :: napari"]
 
 [tool.poetry.dependencies]
-python = "^3.8"
-arkitekt = "^0.4.48"
+python = ">=3.8,<=3.12"
+arkitekt = "0.4.109"
+numpy = "<1.24"
+koil = "0.2.14"
 
 
 [tool.poetry.scripts]
 mikro-napari = "mikro_napari.run:main"
 
 [tool.mypy]
 exclude = [
```

### Comparing `mikro_napari-0.1.50/PKG-INFO` & `mikro_napari-0.1.51/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,24 +1,26 @@
 Metadata-Version: 2.1
 Name: mikro-napari
-Version: 0.1.50
+Version: 0.1.51
 Summary: A napari plugin to interact with and provide functionality for a connected arkitekt server
 Home-page: https://github.com/jhnnsrs/mikro-napari
 License: CC BY-NC 3.0
 Author: jhnnsrs
 Author-email: jhnnsrs@gmail.com
-Requires-Python: >=3.8,<4.0
+Requires-Python: >=3.8,<=3.12
 Classifier: Framework :: napari
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Requires-Dist: arkitekt (>=0.4.48,<0.5.0)
+Requires-Dist: arkitekt (==0.4.109)
+Requires-Dist: koil (==0.2.14)
+Requires-Dist: numpy (<1.24)
 Project-URL: Repository, https://github.com/jhnnsrs/mikro-napari
 Description-Content-Type: text/markdown
 
 # mikro-napari
 
 [![codecov](https://codecov.io/gh/jhnnsrs/mikro-napari/branch/master/graph/badge.svg?token=UGXEA2THBV)](https://codecov.io/gh/jhnnsrs/mikro-napari)
 [![PyPI version](https://badge.fury.io/py/mikro-napari.svg)](https://pypi.org/project/mikro-napari/)
```

